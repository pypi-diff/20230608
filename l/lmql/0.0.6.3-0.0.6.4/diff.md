# Comparing `tmp/lmql-0.0.6.3.tar.gz` & `tmp/lmql-0.0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.6.3.tar", last modified: Thu May 11 15:59:16 2023, max compression
+gzip compressed data, was "lmql-0.0.6.4.tar", last modified: Thu Jun  8 15:29:16 2023, max compression
```

## Comparing `lmql-0.0.6.3.tar` & `lmql-0.0.6.4.tar`

### file list

```diff
@@ -1,257 +1,292 @@
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.141824 lmql-0.0.6.3/.github/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/.github/workflows/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2285 2023-05-11 15:18:25.000000 lmql-0.0.6.3/.github/workflows/lmql-web.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-11 15:13:38.000000 lmql-0.0.6.3/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.3/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6.3/MANIFEST.in
--rw-rw-r--   0 luca      (1000) luca      (1000)     4988 2023-05-11 15:59:16.165824 lmql-0.0.6.3/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     4538 2023-05-11 15:13:38.000000 lmql-0.0.6.3/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.6.3/TODO.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/
--rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/Makefile
--rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6.3/docs/RELEASE.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/make.bat
--rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_ext/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/_ext/lmql_snippets.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.141824 lmql-0.0.6.3/docs/source/_static/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_static/css/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/_static/css/lmql-docs.css
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_static/images/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/_static/images/lmql.svg
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_static/js/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/_static/js/lmql-playground.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_templates/
--rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/_templates/layout.html
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/blog/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/blog/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1444 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/blog/release-0.0.6.1.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1887 2023-05-11 15:59:04.000000 lmql-0.0.6.3/docs/source/blog/release-0.0.6.3.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/blog/release-0.0.6.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6.3/docs/source/conf.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/dev-setup.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     2780 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/index.rst
--rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/installation.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/language/constraints.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6.3/docs/source/language/decoders.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/language/functions.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8310 2023-05-11 15:34:04.000000 lmql-0.0.6.3/docs/source/language/models.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/language/overview.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/language/scripted_prompts.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/logo.png
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/python/
--rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/python/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/langchain.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/llama_index.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/python/lmql.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)     7458 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/output.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/pandas.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/python.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/quickstart.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/releases/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2263 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/releases/misc-snippets.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6.3/docs/source/releases/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/todo.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6.3/pyproject.toml
--rw-rw-r--   0 luca      (1000) luca      (1000)       74 2023-05-11 15:26:02.000000 lmql-0.0.6.3/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/scripts/
--rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6.3/scripts/activate-dev.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/scripts/conda/
--rw-rw-r--   0 luca      (1000) luca      (1000)      198 2023-05-11 15:26:02.000000 lmql-0.0.6.3/scripts/conda/requirements-no-gpu.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      332 2023-05-11 15:26:02.000000 lmql-0.0.6.3/scripts/conda/requirements.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6.3/scripts/pypi-release.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6.3/scripts/wheel.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      866 2023-05-11 15:59:16.165824 lmql-0.0.6.3/setup.cfg
--rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-05-10 14:35:25.000000 lmql-0.0.6.3/setup.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/src/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/
--rw-rw-r--   0 luca      (1000) luca      (1000)     6208 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/__init__.py
--rwxrwxr-x   0 luca      (1000) luca      (1000)     8142 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/cli.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/demo.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/http.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/language/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    24147 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/language/compiler.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/language/fragment_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/language/qstrings.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/language/validator.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/model/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/model/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/model/async_generation_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/model/local_client.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18118 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/model/serve.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8052 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/model/served_model.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/ops/
--rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ops/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ops/follow_map.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    41664 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ops/ops.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    20806 2023-05-11 15:34:49.000000 lmql-0.0.6.3/src/lmql/ops/token_set.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/output/
--rw-rw-r--   0 luca      (1000) luca      (1000)       57 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/output/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2334 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/output/http.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1889 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/output/sse.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2282 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/output/ws.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/runtime/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/runtime/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/runtime/bopenai/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/bopenai/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    28384 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/bopenai/batched_openai.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    17221 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/bopenai/openai_api.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1906 2023-05-11 15:26:02.000000 lmql-0.0.6.3/src/lmql/runtime/caching.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/runtime/dclib/
--rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18631 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_array.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    27728 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_global.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21721 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_model.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_rewrite.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    30560 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_seq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    20827 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/decoders.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/trie_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/hf_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    34822 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/interpreter.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/runtime/interrupt.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/runtime/langchain.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6367 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/lmql_runtime.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/runtime/maiohttp.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/masks.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/runtime/model_registry.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/multi_head_interpretation.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    42592 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/openai_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/openai_secret.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4042 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/output_writer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/runtime/postprocessing/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/runtime/postprocessing/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/postprocessing/group_by.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/program_state.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/stats.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     9778 2023-05-11 15:26:02.000000 lmql-0.0.6.3/src/lmql/runtime/tokenizer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/tests/
--rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/tests/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     5667 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/tests/expr_test_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1314 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/fin_and.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/tests/outdated/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/mask_product_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/monotonicity.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/one_of_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/sentences_op.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/starts_with_op_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/stops_at.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/str_in_str_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/test_multi_head.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/token_set_test.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/tests/system/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/tests/system/basic_use_cases.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      971 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/tail_token_set.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      788 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_back2back_caching.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2382 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_eq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      457 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_orop.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2481 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_sample_queries.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1720 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_scoping.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3572 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_stopping.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/ui/
--rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/ui/live/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/live/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/live/live.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3334 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/ui/live/live.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/live/livelib.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/live/package.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/live/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.157824 lmql-0.0.6.3/src/lmql/ui/playground/
--rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/.dockerignore
--rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/.env
--rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/Dockerfile
--rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.157824 lmql-0.0.6.3/src/lmql/ui/playground/public/
--rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/_headers
--rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/favicon.ico
--rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/index.html
--rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/manifest.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.161824 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/
--rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/calc.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/chat.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/cot.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/hello.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/joke.json
--rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/kv.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/list.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/meta.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/translation.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/robots.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.161824 lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/
--rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   184008 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/ref.py
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/run-in-docker.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/playground/src/
--rw-rw-r--   0 luca      (1000) luca      (1000)    69135 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/App.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/App.test.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/Configuration.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/DataListView.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    21319 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/DecoderGraph.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/DecodingTree.js
--rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/Embed.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/Explore.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/SharedState.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4819 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/State.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5871 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/browser_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/build_info.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/playground/src/editor/
--rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/editor/theme.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/explore.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/graph-layout.css
--rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/index.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/index.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/logo.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/queries.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/remote_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/reportWebVitals.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/screenshot.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/setupTests.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/spinner.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/tagged-model-result.js
--rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/.gitattributes
--rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/.gitignore
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/vscode/.vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/.vscode/launch.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/.vscodeignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/vscode/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/vscode/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/language-configuration.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/vscode/lmql-vscode.png
--rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/vscode/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/
--rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/utils/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/utils/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/utils/docstring_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4933 2023-05-11 15:26:02.000000 lmql-0.0.6.3/src/lmql/utils/graph.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/utils/nputil.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-05-11 15:59:11.000000 lmql-0.0.6.3/src/lmql/version.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql.egg-info/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4988 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     7212 2023-05-11 15:59:16.000000 lmql-0.0.6.3/src/lmql.egg-info/SOURCES.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/dependency_links.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/entry_points.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       94 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/requires.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/top_level.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.459840 lmql-0.0.6.4/.github/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/.github/workflows/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2285 2023-06-02 17:03:48.000000 lmql-0.0.6.4/.github/workflows/lmql-web.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-11 15:13:38.000000 lmql-0.0.6.4/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.4/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6.4/MANIFEST.in
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4991 2023-06-08 15:29:16.487840 lmql-0.0.6.4/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4541 2023-06-07 20:54:49.000000 lmql-0.0.6.4/README.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/docs/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/Makefile
+-rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6.4/docs/RELEASE.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/make.bat
+-rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/docs/source/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/docs/source/_ext/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5543 2023-05-11 20:52:54.000000 lmql-0.0.6.4/docs/source/_ext/lmql_snippets.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.459840 lmql-0.0.6.4/docs/source/_static/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/docs/source/_static/css/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/_static/css/lmql-docs.css
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/_static/images/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/_static/images/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/_static/js/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2252 2023-05-11 20:52:54.000000 lmql-0.0.6.4/docs/source/_static/js/lmql-playground.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/_templates/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/_templates/layout.html
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/blog/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/blog/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1444 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/blog/release-0.0.6.1.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2068 2023-05-11 20:52:54.000000 lmql-0.0.6.4/docs/source/blog/release-0.0.6.3.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/blog/release-0.0.6.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6.4/docs/source/conf.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/dev-setup.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2333 2023-05-22 15:02:40.000000 lmql-0.0.6.4/docs/source/docker-setup.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/images/
+-rw-rw-r--   0 luca      (1000) luca      (1000)   125712 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/images/inference.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2798 2023-05-22 15:02:40.000000 lmql-0.0.6.4/docs/source/index.rst
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2563 2023-05-22 15:02:40.000000 lmql-0.0.6.4/docs/source/installation.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1382 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/language/azure.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/language/constraints.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6.4/docs/source/language/decoders.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/language/functions.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3967 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/language/hf.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      753 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/language/models.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5710 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/language/openai.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/language/overview.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/language/scripted_prompts.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/logo.png
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/pending/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3550 2023-05-11 20:52:54.000000 lmql-0.0.6.4/docs/source/pending/release-next.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/python/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/python/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    11193 2023-06-08 13:00:38.000000 lmql-0.0.6.4/docs/source/python/langchain.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1157 2023-06-08 13:00:38.000000 lmql-0.0.6.4/docs/source/python/lc.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/python/llama_index.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/python/lmql.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7458 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/python/output.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/python/pandas.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/python/python.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/quickstart.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/releases/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2263 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/releases/misc-snippets.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6.4/docs/source/releases/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/todo.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6.4/pyproject.toml
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/scripts/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      577 2023-05-22 15:02:40.000000 lmql-0.0.6.4/scripts/Dockerfile
+-rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6.4/scripts/activate-dev.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/scripts/conda/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      198 2023-05-11 15:26:02.000000 lmql-0.0.6.4/scripts/conda/requirements-no-gpu.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      332 2023-05-11 15:26:02.000000 lmql-0.0.6.4/scripts/conda/requirements.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6.4/scripts/pypi-release.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3897 2023-06-07 20:54:49.000000 lmql-0.0.6.4/scripts/serve-all.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6.4/scripts/wheel.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      868 2023-06-08 15:29:16.487840 lmql-0.0.6.4/setup.cfg
+-rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-05-10 14:35:25.000000 lmql-0.0.6.4/setup.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/src/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/src/lmql/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6821 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/algorithms/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       45 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/algorithms/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2556 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/algorithms/cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      916 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/algorithms/functools.py
+-rwxrwxr-x   0 luca      (1000) luca      (1000)     8222 2023-06-08 13:11:14.000000 lmql-0.0.6.4/src/lmql/cli.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/demo.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/http.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/language/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    24626 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/language/compiler.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-06-08 14:18:51.000000 lmql-0.0.6.4/src/lmql/language/fragment_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1374 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/language/qstrings.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/language/validator.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/models/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/models/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/models/lmtp/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6156 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/models/lmtp/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5726 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_client.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    19104 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_dcmodel.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18111 2023-06-07 20:59:25.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_inference_server.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5514 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_multiprocessing.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      298 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4445 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_serve.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3562 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_threading.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      465 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/models/lmtp/utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3230 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/models/model.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/ops/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ops/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/ops/follow_map.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    41664 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/ops/ops.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21151 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/ops/token_set.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/output/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       57 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/output/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2334 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/output/http.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1889 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/output/sse.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2282 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/output/ws.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/runtime/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/runtime/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/runtime/bopenai/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/runtime/bopenai/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29480 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/bopenai/batched_openai.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21244 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/bopenai/openai_api.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2096 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/caching.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/runtime/dclib/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18839 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_array.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    26228 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      592 2023-06-08 13:11:09.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_global.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4971 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_model.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_rewrite.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    32272 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_seq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21200 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/decoders.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    36788 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/interpreter.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/runtime/interrupt.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1231 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/langchain.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8241 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/lmql_runtime.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1840 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/loop.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1245 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/maiohttp.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/runtime/masks.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2783 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/model_registry.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5943 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/multi_head_interpretation.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    44712 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/openai_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/runtime/openai_secret.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4042 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/runtime/output_writer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/runtime/postprocessing/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/runtime/postprocessing/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3543 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/runtime/postprocessing/group_by.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2067 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/program_state.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/runtime/stats.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2116 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/token_distribution.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10709 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/tokenizer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/runtime/tokenizers/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3027 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/tokenizers/hf_tokenizer.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3415 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/tokenizers/pure_python_tokenizer.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3207 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/tests/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/tests/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5899 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/tests/expr_test_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1314 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/fin_and.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      879 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/tests/local_model_python.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/tests/outdated/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/mask_product_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/monotonicity.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/one_of_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/sentences_op.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/starts_with_op_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/stops_at.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/str_in_str_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/test_multi_head.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/token_set_test.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/tests/queryargs/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4489 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_args.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2072 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_args_query_str.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1095 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_args_run.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1066 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_sync.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1092 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_var_errors.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/tests/system/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/tests/system/basic_use_cases.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      842 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/tests/tail_token_set.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      788 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_back2back_caching.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2382 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_eq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1139 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/tests/test_multibyte_characters.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1140 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/tests/test_multibyte_local_models.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      457 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_orop.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      448 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/test_query_args.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2639 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/tests/test_sample_queries.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1720 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_scoping.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3572 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_stopping.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      707 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/tests/tiktoken_tsets.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/ui/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.479840 lmql-0.0.6.4/src/lmql/ui/live/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/live/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/live/live.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3313 2023-06-06 10:45:15.000000 lmql-0.0.6.4/src/lmql/ui/live/live.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/live/livelib.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/live/package.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/live/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.479840 lmql-0.0.6.4/src/lmql/ui/playground/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/.dockerignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/.env
+-rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/Dockerfile
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.479840 lmql-0.0.6.4/src/lmql/ui/playground/public/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/_headers
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/favicon.ico
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/index.html
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/manifest.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.483840 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    22895 2023-06-08 13:49:28.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-05-23 11:41:29.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/list.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/robots.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.483840 lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/
+-rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   184008 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/ref.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/run-in-docker.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/playground/src/
+-rw-rw-r--   0 luca      (1000) luca      (1000)    69705 2023-06-08 15:24:40.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/App.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/App.test.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-06-02 17:03:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/Configuration.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/DataListView.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21617 2023-06-08 15:27:15.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/DecodingTree.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/Embed.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-06-02 17:03:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/Explore.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/SharedState.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4819 2023-06-08 15:09:20.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/State.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5871 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/browser_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/build_info.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/playground/src/editor/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-06-02 17:03:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/editor/theme.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/explore.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/graph-layout.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-05-25 08:49:26.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/index.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/index.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/logo.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8152 2023-06-08 13:54:23.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/queries.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/remote_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/screenshot.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/setupTests.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/spinner.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3181 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/.gitattributes
+-rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/.gitignore
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/vscode/.vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/.vscode/launch.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/.vscodeignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/vscode/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/vscode/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/language-configuration.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/vscode/lmql-vscode.png
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/vscode/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/utils/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/utils/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/utils/docstring_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4933 2023-05-11 15:26:02.000000 lmql-0.0.6.4/src/lmql/utils/graph.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2592 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/utils/nputil.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-06-08 15:29:11.000000 lmql-0.0.6.4/src/lmql/version.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql.egg-info/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4991 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8328 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/SOURCES.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/dependency_links.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/entry_points.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       95 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/requires.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/top_level.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql.svg
```

### Comparing `lmql-0.0.6.3/.github/workflows/lmql-web.yml` & `lmql-0.0.6.4/.github/workflows/lmql-web.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/.gitignore` & `lmql-0.0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/LICENSE` & `lmql-0.0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/PKG-INFO` & `lmql-0.0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -95,15 +95,15 @@
 
 > **Operating System**: The GPU-enabled version of LMQL was tested to work on Ubuntu 22.04 with CUDA 12.0 and Windows 10 via WSL2 and CUDA 11.7. The no-GPU version (see below) was tested to work on Ubuntu 22.04 and macOS 13.2 Ventura or Windows 10 via WSL2.
 
 ### Development without GPU
 
 This section outlines how to setup an LMQL development environment without local GPU support. Note that LMQL without local GPU support only supports the use of API-integrated models like `openai/text-davinci-003`. Please see the OpenAI API documentation (https://platform.openai.com/docs/models/gpt-3-5) to learn more about the set of available models.
 
-To setup a `conda` environment for LMQL with GPU support, run the following commands:
+To setup a `conda` environment for LMQL with no GPU support, run the following commands:
 
 ```
 # prepare conda environment
 conda env create -f scripts/conda/requirements-no-gpu.yml -n lmql-no-gpu
 conda activate lmql-no-gpu
 
 # registers the `lmql` command in the current shell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.3 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.4 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
@@ -53,12 +53,12 @@
 Ubuntu 22.04 with CUDA 12.0 and Windows 10 via WSL2 and CUDA 11.7. The no-GPU
 version (see below) was tested to work on Ubuntu 22.04 and macOS 13.2 Ventura
 or Windows 10 via WSL2. ### Development without GPU This section outlines how
 to setup an LMQL development environment without local GPU support. Note that
 LMQL without local GPU support only supports the use of API-integrated models
 like `openai/text-davinci-003`. Please see the OpenAI API documentation (https:
 //platform.openai.com/docs/models/gpt-3-5) to learn more about the set of
-available models. To setup a `conda` environment for LMQL with GPU support, run
-the following commands: ``` # prepare conda environment conda env create -
+available models. To setup a `conda` environment for LMQL with no GPU support,
+run the following commands: ``` # prepare conda environment conda env create -
 f scripts/conda/requirements-no-gpu.yml -n lmql-no-gpu conda activate lmql-no-
 gpu # registers the `lmql` command in the current shell source scripts/
 activate-dev.sh ```
```

### Comparing `lmql-0.0.6.3/README.md` & `lmql-0.0.6.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 > **Operating System**: The GPU-enabled version of LMQL was tested to work on Ubuntu 22.04 with CUDA 12.0 and Windows 10 via WSL2 and CUDA 11.7. The no-GPU version (see below) was tested to work on Ubuntu 22.04 and macOS 13.2 Ventura or Windows 10 via WSL2.
 
 ### Development without GPU
 
 This section outlines how to setup an LMQL development environment without local GPU support. Note that LMQL without local GPU support only supports the use of API-integrated models like `openai/text-davinci-003`. Please see the OpenAI API documentation (https://platform.openai.com/docs/models/gpt-3-5) to learn more about the set of available models.
 
-To setup a `conda` environment for LMQL with GPU support, run the following commands:
+To setup a `conda` environment for LMQL with no GPU support, run the following commands:
 
 ```
 # prepare conda environment
 conda env create -f scripts/conda/requirements-no-gpu.yml -n lmql-no-gpu
 conda activate lmql-no-gpu
 
 # registers the `lmql` command in the current shell
```

#### html2text {}

```diff
@@ -47,12 +47,12 @@
 Ubuntu 22.04 with CUDA 12.0 and Windows 10 via WSL2 and CUDA 11.7. The no-GPU
 version (see below) was tested to work on Ubuntu 22.04 and macOS 13.2 Ventura
 or Windows 10 via WSL2. ### Development without GPU This section outlines how
 to setup an LMQL development environment without local GPU support. Note that
 LMQL without local GPU support only supports the use of API-integrated models
 like `openai/text-davinci-003`. Please see the OpenAI API documentation (https:
 //platform.openai.com/docs/models/gpt-3-5) to learn more about the set of
-available models. To setup a `conda` environment for LMQL with GPU support, run
-the following commands: ``` # prepare conda environment conda env create -
+available models. To setup a `conda` environment for LMQL with no GPU support,
+run the following commands: ``` # prepare conda environment conda env create -
 f scripts/conda/requirements-no-gpu.yml -n lmql-no-gpu conda activate lmql-no-
 gpu # registers the `lmql` command in the current shell source scripts/
 activate-dev.sh ```
```

### Comparing `lmql-0.0.6.3/docs/Makefile` & `lmql-0.0.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/make.bat` & `lmql-0.0.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/_ext/lmql_snippets.py` & `lmql-0.0.6.4/docs/source/_ext/lmql_snippets.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
         "var",
         "sample",
         "FROM",
         "from",
         "WHERE",
         "where",
         "DISTRIBUTION",
-        "distribution")
-    )
+        "distribution",
+        "class"
+    ))
 
     def get_tokens_unprocessed(self, text):
         for index, token, value in PythonLexer.get_tokens_unprocessed(self, text):
             if token is Name and value in self.EXTRA_KEYWORDS:
                 yield index, Keyword.Pseudo, value
             else:
                 yield index, token, value
```

### Comparing `lmql-0.0.6.3/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.6.4/docs/source/_static/css/lmql-docs.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/_static/images/lmql.svg` & `lmql-0.0.6.4/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.6.4/docs/source/_static/js/lmql-playground.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,16 @@
 var openPlaygroundElement = null;
 
-function getPlaygroundUrl() {
+function getPlaygroundUrl(next) {
     const host = window.location.host;
+
+    if (next) {
+        return "https://next.lmql.ai/playground";
+    }
+
     if (host === "docs.lmql.ai") {
         return "https://lmql.ai/playground";
     } else if (host.startsWith("localhost") || host.startsWith("127.0.0.1")) {
         return "http://localhost:3000/playground";
     } else {
         return "https://lbeurerkellner.github.io/green-gold-dachshund-web/playground";
     }
@@ -30,16 +35,15 @@
         openPlaygroundElement = null;
     }
 }
 
 function openPlaygroundSnippet(link, snippet) {
     closePlaygroundSnippet();
 
-    const playground = getPlaygroundUrl();
-    console.log("playground url: " + playground);
+    const playground = getPlaygroundUrl(snippet.includes("next-"));
 
     // this is a that was clicked, replace parent div with iframe (temporarily)
     const container = link.parentElement;
     container.classList.add('playground');
     const iframe = document.createElement('iframe');
     iframe.src = ""
     iframe.src = playground + '?embed=' + snippet + ".json"
```

### Comparing `lmql-0.0.6.3/docs/source/blog/release-0.0.5.md` & `lmql-0.0.6.4/docs/source/blog/release-0.0.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/blog/release-0.0.6.1.md` & `lmql-0.0.6.4/docs/source/blog/release-0.0.6.1.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/blog/release-0.0.6.3.md` & `lmql-0.0.6.4/docs/source/blog/release-0.0.6.3.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 metadata:release: 2023-05-11 18:00:00 +0000
 metadata:authors: team
 
 # LMQL v0.0.6.3
 
 Today, we are releasing LMQL v0.0.6.3. This update contains several bug fixes and improvements. The most notable changes are:
 
-* **Lighter Runtime** As part of our continued efforts, we made LMQL much lighter (no more mandatory `transformers` dependency).
+* **Lighter Runtime** As part of our continued efforts, we made LMQL much lighter (no more mandatory `transformers` dependency). By default LMQL now no longer requires `transformers` or PyTorch. If you rely on local models, just install LMQL via `pip install lmql[hf]` to get full Transformers integration.
 
-* **Token Constraints** A new function `TOKENS(...)` was added to the LMQL constraint language, allowing you to specify lower and upper bounds or the exact number of tokens to generate for given variable.
+* **Token Constraints** A new function `TOKENS(...)` was added to the LMQL constraint language, allowing you to specify lower and upper bounds or the exact number of tokens to generate for a given variable.
     
     ```{lmql}
     name::token_constraints
     argmax 
         "A 10 token response[WHO]" 
     from 
         "openai/text-ada-001" 
     where 
         len(TOKENS(WHO)) == 10
     ```
 
 * **Conditional Stopping** `STOPS_AT` can now be combined with additional side conditions. This allows you to specify stopping phrases that are only enforced, once other conditions are met. 
 
-    For example below, we stop when the generated text hits a newline character, but only if the overall variable output is already at least 10 tokens long.
+    For example, below, we stop when the generated text hits a newline character, but only if the overall variable output is already at least 10 tokens long.
 
     ```{lmql}
     name::conditional_stopping 
     argmax 
         "Hello[WHO]" 
     from 
         "openai/text-ada-001"
```

#### html2text {}

```diff
@@ -1,23 +1,25 @@
 metadata:release: 2023-05-11 18:00:00 +0000 metadata:authors: team # LMQL
 v0.0.6.3 Today, we are releasing LMQL v0.0.6.3. This update contains several
 bug fixes and improvements. The most notable changes are: * **Lighter Runtime**
 As part of our continued efforts, we made LMQL much lighter (no more mandatory
-`transformers` dependency). * **Token Constraints** A new function `TOKENS
-(...)` was added to the LMQL constraint language, allowing you to specify lower
-and upper bounds or the exact number of tokens to generate for given variable.
-```{lmql} name::token_constraints argmax "A 10 token response[WHO]" from
-"openai/text-ada-001" where len(TOKENS(WHO)) == 10 ``` * **Conditional
-Stopping** `STOPS_AT` can now be combined with additional side conditions. This
-allows you to specify stopping phrases that are only enforced, once other
-conditions are met. For example below, we stop when the generated text hits a
-newline character, but only if the overall variable output is already at least
-10 tokens long. ```{lmql} name::conditional_stopping argmax "Hello[WHO]" from
-"openai/text-ada-001" where len(TOKENS(WHO)) > 10 and STOPS_AT(WHO, "\n") ``` *
-**lmql.run**: Improved input validation for `lmql.run` as contributed by
-@lfegray. More specifically, `lmql.run` wil now provide more helpful error
-messages when client logic does not specify input values for all required query
-parameters. * **Automatic Cache Invalidation**: LMQL's tokenizer cache at
-`~/.cache/lmql` is now invalidated automatically when upgrading to a new
-version. This should prevent issues with outdated cache files. > Note: Version
-0.0.6.2 was skipped and yanked from pypi.org, as an invalid release was pushed
-accidentally.
+`transformers` dependency). By default LMQL now no longer requires
+`transformers` or PyTorch. If you rely on local models, just install LMQL via
+`pip install lmql[hf]` to get full Transformers integration. * **Token
+Constraints** A new function `TOKENS(...)` was added to the LMQL constraint
+language, allowing you to specify lower and upper bounds or the exact number of
+tokens to generate for a given variable. ```{lmql} name::token_constraints
+argmax "A 10 token response[WHO]" from "openai/text-ada-001" where len(TOKENS
+(WHO)) == 10 ``` * **Conditional Stopping** `STOPS_AT` can now be combined with
+additional side conditions. This allows you to specify stopping phrases that
+are only enforced, once other conditions are met. For example, below, we stop
+when the generated text hits a newline character, but only if the overall
+variable output is already at least 10 tokens long. ```{lmql} name::
+conditional_stopping argmax "Hello[WHO]" from "openai/text-ada-001" where len
+(TOKENS(WHO)) > 10 and STOPS_AT(WHO, "\n") ``` * **lmql.run**: Improved input
+validation for `lmql.run` as contributed by @lfegray. More specifically,
+`lmql.run` wil now provide more helpful error messages when client logic does
+not specify input values for all required query parameters. * **Automatic Cache
+Invalidation**: LMQL's tokenizer cache at `~/.cache/lmql` is now invalidated
+automatically when upgrading to a new version. This should prevent issues with
+outdated cache files. > Note: Version 0.0.6.2 was skipped and yanked from
+pypi.org, as an invalid release was pushed accidentally.
```

### Comparing `lmql-0.0.6.3/docs/source/blog/release-0.0.6.md` & `lmql-0.0.6.4/docs/source/blog/release-0.0.6.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/conf.py` & `lmql-0.0.6.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/dev-setup.md` & `lmql-0.0.6.4/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/index.rst` & `lmql-0.0.6.4/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -87,10 +87,11 @@
     python/output.md
    
 .. toctree::
     :maxdepth: 1
     :caption: 💬 Contribute
     
     dev-setup
+    docker-setup
     Discord <https://discord.gg/7eJP4fcyNT>
     GitHub Issues <https://github.com/eth-sri/lmql/issues>
-    E-Mail <mailto:hello@lmql.ai>
+    E-Mail <mailto:hello@lmql.ai>
```

#### html2text {}

```diff
@@ -21,11 +21,12 @@
 Contents -------- .. toctree:: :maxdepth: 1 quickstart installation â¡ï¸
 Playground IDE
 lmql.ai/playground> .. toctree:: :maxdepth: 1 :caption: ð LMQL Language
 language/overview.md language/scripted_prompts.md language/constraints.md
 language/decoders.md language/models.md language/functions.md .. toctree:: :
 maxdepth: 1 :caption: ð Python Integration python/python.ipynb python/
 langchain.ipynb python/llama_index.ipynb python/pandas.ipynb python/output.md
-.. toctree:: :maxdepth: 1 :caption: ð¬ Contribute dev-setup Discord
+.. toctree:: :maxdepth: 1 :caption: ð¬ Contribute dev-setup docker-setup
+Discord
 discord.gg/7eJP4fcyNT> GitHub Issues
 github.com/eth-sri/lmql/issues> E-Mail
 lmql.ai>
```

### Comparing `lmql-0.0.6.3/docs/source/installation.md` & `lmql-0.0.6.4/docs/source/installation.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 To install the latest version of LMQL locally, run the following command with Python >=3.10 installed.
 
 ```
 pip install lmql
 ```
 
-**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. [https://pytorch.org/get-started/locally/]()).
+**Local GPU Support:** If you want to run models on a local GPU, make sure to install LMQL in an environment with a GPU-enabled installation of PyTorch >= 1.11 (cf. [https://pytorch.org/get-started/locally/]()). To install GPU dependencies via pip, install LMQL via `pip install lmql[hf]`.
 
 ## Running LMQL Programs
 
 **Playground**
 
 After installation, you can launch a local instance of the Playground IDE using the following command:
 
@@ -32,15 +32,15 @@
 
 LMQL can also be used directly from within Python. To use LMQL in Python, you can import the `lmql` package, run query code via `lmql.run` or use a decorator `@lmql.query` for LMQL query functions.
 
 For more details, please see the [Python Integration](./python/python.ipynb) chapter.
 
 ## Self-Hosted Models
 
-Note that when using local [🤗 Transformers](https://huggingface.co/transformers) models in the Playground IDE or via `lmql run`, you have to first launch an instance of the LMQL Inference API for the corresponding model via the command `lmql serve-model`. For more details, please see [Models](./language/models.md) chapter.
+Note that when using local [🤗 Transformers](https://huggingface.co/transformers) models in the Playground IDE or via `lmql run`, you have to first launch an instance of the LMQL Inference API for the corresponding model via the command `lmql serve-model`. For more details, please see [🤗 Models](./language/hf.md) chapter.
 
 ## Configuring OpenAI API Credentials
 
 If you want to use OpenAI models, you have to configure your API credentials. To do so you can either define the `OPENAI_API_KEY` environment variable or create a file `api.env` in the active working directory, with the following contents.
 
 ```
 openai-org: <org identifier>
```

### Comparing `lmql-0.0.6.3/docs/source/language/constraints.md` & `lmql-0.0.6.4/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/language/decoders.md` & `lmql-0.0.6.4/docs/source/language/decoders.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/language/functions.md` & `lmql-0.0.6.4/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/language/overview.md` & `lmql-0.0.6.4/docs/source/language/overview.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/language/scripted_prompts.md` & `lmql-0.0.6.4/docs/source/language/scripted_prompts.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/lmql.svg` & `lmql-0.0.6.4/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/logo.png` & `lmql-0.0.6.4/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/python/langchain.ipynb` & `lmql-0.0.6.4/docs/source/python/langchain.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9769066220238095%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 2: "*

 * *            "{'attachments': OrderedDict()}, 3: {'attachments': OrderedDict()}, 6: {'attachments': "*

 * *            "OrderedDict()}, 7: {'outputs': []}, 8: {'attachments': OrderedDict()}, 10: "*

 * *            "{'attachments': OrderedDict()}, 11: {'attachments': OrderedDict()}, 12: "*

 * *            "{'attachments': OrderedDict()}, 13: {'execution_count': 7}, 14: {'attachments': "*

 * *            "OrderedDict()}, 15: {'execution_count […]*

```diff
@@ -1,31 +1,35 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# LangChain Integration \ud83e\udd9c\ud83d\udd17 "
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "LMQL can also be used together with the [\ud83e\udd9c\ud83d\udd17 LangChain](https://python.langchain.com/en/latest/index.html#) python library. Both, using langchain libraries from LMQL code and using LMQL queries as part of chains are supported."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Using LangChain from LMQL"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We first consider the case, where one may want to use LangChain modules as part of an LMQL query.\n",
                 "\n",
                 "In this example, we want to leverage the LangChain `Chroma` retrieval model, to enable question answering about a text document (the LMQL paper in this case).\n",
                 "\n",
@@ -61,47 +65,41 @@
                 "import lmql\n",
                 "import asyncio\n",
                 "from langchain.embeddings.openai import OpenAIEmbeddings\n",
                 "from langchain.vectorstores import Chroma"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Next, we load and embed the text of the relevant document (`lmql.txt` in our case)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Using embedded DuckDB with persistence: data will be stored in: lmql-index\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "# load text of LMQL paper\n",
                 "with open(\"lmql.txt\") as f:\n",
                 "    contents = f.read()\n",
                 "texts = []\n",
                 "for i in range(0, len(contents), 120):\n",
                 "    texts.append(contents[i:i+120])\n",
                 "\n",
                 "embeddings = OpenAIEmbeddings()\n",
                 "docsearch = Chroma.from_texts(texts, embeddings, \n",
                 "    metadatas=[{\"text\": t} for t in texts], persist_directory=\"lmql-index\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We then construct a chatbot function, using a simple LMQL query, that first prompts the user for a question via `await input(...)`, retrieves relevant text paragraphs using LangChain and then produces an answer using `openai/gpt-3.5-turbo` (ChatGPT)."
             ]
         },
         {
@@ -145,64 +143,68 @@
                 "    \"openai/gpt-3.5-turbo\"\n",
                 "        '''\n",
                 "\n",
                 "await chatbot(output_writer=lmql.stream(variable=\"RESPONSE\"))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As shown in the query, inline LMQL code appearing in a Python script can access the outer scope containing e.g. the `docsearch` variable, and access any relevant utility functions and object defined in Python."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Using LMQL from LangChain"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In addition to using langchain utilities in LMQL query code, LMQL queries can also seamlessly be integrated as a `langchain` `Chain` component. \n",
                 "\n",
                 "For this consider, the sequential prompting example from the `langchain` documentation, where we first prompt the language model to propose a company name for a given product, and then ask it for a catchphrase.\n",
                 "\n",
                 "To get started, we first import the relevant langchain components, as well as LMQL."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from langchain import LLMChain, PromptTemplate\n",
                 "from langchain.chat_models import ChatOpenAI\n",
                 "from langchain.prompts.chat import (ChatPromptTemplate,HumanMessagePromptTemplate)\n",
                 "from langchain.llms import OpenAI\n",
                 "\n",
                 "import lmql"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Our chain has two stages: (1) Asking the model for a company name, and (2) asking the model for a catchphrase. For the sake of this example, we will implement (1) in with a langchain prompt and (2) with an LMQL query. \n",
                 "\n",
                 "First, we define the langchain prompt for the company name and instantiate the resulting `LLMChain`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# setup the LM to be used by langchain\n",
                 "llm = OpenAI(temperature=0.9)\n",
                 "\n",
                 "human_message_prompt = HumanMessagePromptTemplate(\n",
@@ -213,105 +215,110 @@
                 "    )\n",
                 "chat_prompt_template = ChatPromptTemplate.from_messages([human_message_prompt])\n",
                 "chat = ChatOpenAI(temperature=0.9)\n",
                 "chain = LLMChain(llm=chat, prompt=chat_prompt_template)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This can already be executed to produce a company name:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'Rainbow Socks Inc.'"
+                            "'Rainbow Socks Co.'"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "chain.run(\"colorful socks\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Next, we define prompt (2) in LMQL, i.e. the LMQL query generating the catchphrase:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "@lmql.query\n",
                 "async def write_catch_phrase(company_name: str):\n",
                 "    '''\n",
                 "    argmax \"Write a catchphrase for the following company: {company_name}. [catchphrase]\" from \"chatgpt\"\n",
                 "    '''"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Again, we can run this part in isolation, like so:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "' \"Step up your style with Socks Inc.\"'"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "(await write_catch_phrase(\"Socks Inc\"))[0].variables[\"catchphrase\"]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To chain the two prompts together, we can use a `SimpleSequentialChain` from `langchain`:"
+                "To chain the two prompts together, we can use a `SimpleSequentialChain` from `langchain`. To make an LMQL query compatible for use with `langchain`, just call `.aschain()` on it, before passing it to the `SimpleSequentialChain` constructor."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from langchain.chains import SimpleSequentialChain\n",
-                "overall_chain = SimpleSequentialChain(chains=[chain, write_catch_phrase], verbose=True)"
+                "overall_chain = SimpleSequentialChain(chains=[chain, write_catch_phrase.aschain()], verbose=True)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now, we can run the overall chain, relying both on LMQL and langchain components:"
             ]
         },
         {
@@ -324,28 +331,30 @@
             "source": [
                 "# Run the chain specifying only the input variable for the first chain.\n",
                 "catchphrase = overall_chain.run(\"colorful socks\")\n",
                 "print(catchphrase)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "```\n",
                 "> Entering new SimpleSequentialChain chain...\n",
                 "RainbowSocks Co.\n",
                 " \"Step into a world of color with RainbowSocks Co.!\"\n",
                 "\n",
                 "> Finished chain.\n",
                 " \"Step into a world of color with RainbowSocks Co.!\"\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> Note that the full chain currently only works when run outside a Jupyter environment (in a script), due to the way langchain and LMQL rely on async vs. sequential calls. With further improvements to the `langchain` async API, this limitation can be expected to be removed."
             ]
         }
     ],
```

### Comparing `lmql-0.0.6.3/docs/source/python/llama_index.ipynb` & `lmql-0.0.6.4/docs/source/python/llama_index.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/python/lmql.txt` & `lmql-0.0.6.4/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/python/output.ipynb` & `lmql-0.0.6.4/docs/source/python/output.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/python/pandas.ipynb` & `lmql-0.0.6.4/docs/source/python/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/python/python.ipynb` & `lmql-0.0.6.4/docs/source/python/python.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/quickstart.md` & `lmql-0.0.6.4/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/docs/source/releases/misc-snippets.md` & `lmql-0.0.6.4/docs/source/releases/misc-snippets.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/scripts/wheel.sh` & `lmql-0.0.6.4/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/setup.cfg` & `lmql-0.0.6.4/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.6.3
+version = 0.0.6.4
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls = 
@@ -20,15 +20,16 @@
 include_package_data = True
 python_requires = >=3.10
 install_requires = 
 	astunparse ==1.6.3
 	openai
 	termcolor
 	numpy
-	gpt3_tokenizer
+	tiktoken
+	psutil
 
 [options.extras_require]
 hf = transformers >=4.28.1; accelerate
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `lmql-0.0.6.3/src/lmql/cli.py` & `lmql-0.0.6.4/src/lmql/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import lmql.version as version_info
 
 project_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 def cmd_serve_model():
     """emoji:🏄 Serve a 🤗 Transformers model via the LMQL inference API"""
     os.chdir(project_root)
-    os.system("python -m lmql.model.serve " + " ".join(sys.argv[2:]))
+    os.system("python -m lmql.models.lmtp.lmtp_serve " + " ".join(sys.argv[2:]))
 
 def cmd_run():
     """
     emoji:🏃 run a LMQL script (e.g. "lmql run latest/hello.lmql")
     """
     import asyncio
     import time
@@ -174,14 +174,16 @@
         code_local = """
     argmax "Hello[WHO]" from "local:gpt2-medium" where len(WHO) < 10    
     """
         print("[Greeting 🤗 Transformers]")
         asyncio.run(lmql.run(code_local, output_writer=lmql.printing))
     
     if backend is None or backend == "openai":
+        import lmql.runtime.dclib as dc
+        dc.clear_tokenizer()
         print("[Greeting OpenAI]")
         code_openai = """
     argmax "Hello[WHO]" from "openai/text-ada-001" where len(WHO) < 10    
     """
         asyncio.run(lmql.run(code_openai, output_writer=lmql.printing))
 
 def basic_samples():
```

### Comparing `lmql-0.0.6.3/src/lmql/demo.py` & `lmql-0.0.6.4/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/http.py` & `lmql-0.0.6.4/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/language/compiler.py` & `lmql-0.0.6.4/src/lmql/language/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,39 +119,50 @@
             self.defined_vars.add(v)
             self.written_vars.add(v)
             if v in self.free_vars: self.free_vars.remove(v)
 
         # capture set of format vars (exclude {{ and }})
         # replace {{ and }} with escape sequence \u007b and \u007d 
         qstring = qstring.replace("{{", "__curly_open__").replace("}}", "__curly_close__")
+        # same for [[ and ]]
+        qstring = qstring.replace("[[", "__square_open__").replace("]]", "__square_close__")
+
         used_fstring_expr = [v[1:-1] for v in re.findall("\{[^\}\{]+\}", qstring)]
         for v in used_fstring_expr:
             if v.startswith(":"):
                 continue
             try:
                 parsed = ast.parse(v).body[0].value
                 self.visit(parsed)
             except:
-                raise RuntimeError("Failed to parse fstring expression: ", v)
+                print("info: failed to parse fstring expression: ", v)
+                # raise RuntimeError("Failed to parse fstring expression: ", v)
+                return super().visit_Constant(node)
 
         # put double curly braces back in
         qstring = qstring.replace("__curly_open__", "{{").replace("__curly_close__", "}}")
-                
+        qstring = qstring.replace("__square_open__", "[[").replace("__square_close__", "]]")
+        
         template_tags = [v[1:-1] for v in re.findall("\{:[A-z0-9]+\}", qstring)]
         for tt in template_tags:
             qstring = qstring.replace(f"{{{tt}}}", f"{{lmql.tag('{tt[1:]}')}}")
         
+        # replace other {} with lmql.escape
+        qstring = re.sub("\{[^\}]+\}", lambda m: f"{{lmql.lmql_runtime.f_escape({m.group(0)[1:-1]})}}", qstring)
+
         node.value = qstring
 
         return super().visit_Constant(node)
 
     def exclude_identifier(self, name):
         # make sure "input" can be intercepted
         if name in ["input"]:
             return False
+        if name in ["lmql"]:
+            return True
         if name in self.free_vars:
             return True
         if name in self.written_vars:
             return True
         # exclude LMQL built-ins
         if get_builtin_name(name) is not None:
             return True
@@ -621,22 +632,21 @@
                 model_name = "'" + model_name_aliases[model_name[1:-1]] + "'"
 
             # resulting code
             code = None
             output_variables = "output_variables=[" + ", ".join([f'"{v}"' for v in scope.defined_vars]) + "]"
 
             # generate function that runs query
-            parameters = list(sorted(list(scope.free_vars.union(set(["context"])))))
+            parameters = list(sorted(list(scope.free_vars)))
 
             with PythonFunctionWriter("query", output_file, parameters, 
                 q.prologue, decorators=["lmql.compiled_query"], decorators_args=[output_variables]) as writer:
                 
+                writer.add(yield_call("set_decoder", astunparse.unparse(q.decode.method).strip(), unparse_list(q.decode.decoding_args)))                
                 writer.add(yield_call("set_model", model_name))
-                # writer.add(f"context.set_decoder({})")
-                writer.add(yield_call("set_decoder", astunparse.unparse(q.decode.method).strip(), unparse_list(q.decode.decoding_args)))
                 writer.add("# where")
                 writer.add(q.where)
                 writer.add(yield_call("set_where_clause", q.where_expr))
                 writer.add("# prompt")
                 writer.add(astunparse.unparse(q.prompt))
                 if q.distribution:
                     writer.add("# distribution")
```

### Comparing `lmql-0.0.6.3/src/lmql/language/fragment_parser.py` & `lmql-0.0.6.4/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/language/validator.py` & `lmql-0.0.6.4/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/model/serve.py` & `lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_dcmodel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,504 +1,442 @@
 """
-Serves a transformers model as LMQL inference API.
+LMQL model implementation that uses the LMTP protocol to communicate with a
+hosted model server, or a model running in a separate process.
 """
 
-from dataclasses import dataclass, field
-from collections import defaultdict
-
-import json
-from http.server import BaseHTTPRequestHandler, HTTPServer
-from multiprocessing import Queue as MPQueue
-from queue import Empty
-from queue import Queue
-import multiprocessing
-from typing import Dict
-import requests
+from lmql.runtime.dclib.dclib_model import DcModel
+from lmql.runtime.tokenizer import load_tokenizer
+from .lmtp_client import LMTPWebSocketClient
+from .lmtp_multiprocessing import LMTPMultiProcessingClient
+from .lmtp_threading import LMTPThreadedClient
+from .lmtp_inference_server import Scheduler
+import lmql.runtime.dclib as dc
 import asyncio
-import sys
-import atexit
-import argparse
-import time
-import os
-import subprocess
-
-from transformers import AutoModelForCausalLM, AutoTokenizer, pipeline
-import torch
-
-@dataclass
-class InferenceServerState:
-    model_identifier : str
-    tokenizer_descriptor : str
-    dtype: str
-
-    queue: Queue
-    tokenize_queue: Queue
-    all_results_queue : Queue
-    
-    sample_count: int = 0
-    client_results_queues: Dict[str,Queue] = field(default_factory=dict)
-    
-    exit: bool = False
+import numpy as np
+import aiohttp
+import lmql.utils.nputil as nputil
+import lmql.runtime.masks as masks
+from lmql.runtime.token_distribution import TokenDistribution
+
+from typing import Any, List, Union
+
+class LMTPModel(DcModel):
+    def __init__(self, model, tokenizer, endpoint, inprocess=False, truncation_threshold=-3e+38, init_workers=True, lmtp_server_kwargs=None, inprocess_client_constructor=None, **kwargs):
+        super().__init__(model, tokenizer, truncation_threshold, init_workers, **kwargs)
+
+        self.model.chunk_size = kwargs.get("chunksize", 16)
+
+        # LMTP client object (can be inprocess or websocket)
+        self.client = None
+        # asyncio task for client loop
+        self._client_loop = None
+        # set once self.client is set up
+        self.connected_signal = asyncio.Event()
+        # set to termiante self._client_loop
+        self.close_signal = asyncio.Event()
+        # error signal
+        self.error_signal = asyncio.Event()
+        
+        # endpoint in case of remote model
+        self.endpoint = endpoint
+        if endpoint is not None and not self.endpoint.startswith("http"):
+            self.endpoint = "http://" + self.endpoint
+
+        self.inprocess = inprocess
+        self.lmtp_server_kwargs = lmtp_server_kwargs
+        assert self.inprocess or  lmtp_server_kwargs is None, "LMTP server kwargs can only be set when using lmql.inprocess mode"
+        if inprocess:
+            self.inprocess_client_constructor = inprocess_client_constructor or LMTPMultiProcessingClient
+
+        # model statistics
+        self.requests = 0
+        self.tokens = 0
+
+    async def inprocess_client_loop(self):
+        self.client = self.inprocess_client_constructor(self.model.model_identifier, **self.lmtp_server_kwargs)
+
+        self.connected_signal.set()
+        await self.close_signal.wait()
+        await self.client.close()
+        self.client = None
 
-class TokenizerProcessor:
-    def __init__(self, state: InferenceServerState, ready_event: multiprocessing.Event = None):
-        self.model_identifier = state.tokenizer_descriptor
-        self.queue = state.tokenize_queue
-        self.state = state
-        self.ready_event = ready_event
-
-    def shutdown(self):
-        self.state.exit = True
-
-    def tokenize(self, tokenizer, sample_id, client_id, item):
-        text = item["text"]
-
-        if text == "<EOS>":
-            input_ids = [tokenizer.eos_token_id]
-        elif text == "<BOS>":
-            input_ids = [tokenizer.bos_token_id]
-        else:
-            input_ids = tokenizer(text)["input_ids"]
-
-        self.state.all_results_queue.put({
-            "sample_id": sample_id,
-            "client_id": client_id,
-            "input_ids": input_ids
-        })
-
-    def detokenize(self, tokenizer, sample_id, client_id, item):
-        input_ids = item["input_ids"]
-
-        text = tokenizer.decode(input_ids)
-        self.state.all_results_queue.put({
-            "sample_id": sample_id,
-            "client_id": client_id,
-            "text": text
-        })
-
-    def run(self, index):
-        # load tokenizer
-        tokenizer = AutoTokenizer.from_pretrained(self.model_identifier)
-        print("Tokenizer #{} {} ready!".format(index, self.model_identifier))
-
-        if self.ready_event:
-            self.ready_event.set()
-
-        while not self.state.exit:
-            item = self.queue.get()
-            if item is None:
-                time.sleep(0.1)
-                continue
-
-            sample_id = item["sample_id"]
-            client_id = item["client_id"]
-            action = item["action"]
-
-            if action == "tokenize":
-                self.tokenize(tokenizer, sample_id, client_id, item)
-            elif action == "detokenize":
-                self.detokenize(tokenizer, sample_id, client_id, item)
-            else:
-                print("error: unknown TokenizerProcessor action {}".format(action))
-        
-        print("Tokenizer #{} shut down.".format(index))
+    async def ws_client_loop(self):
+        try:
+            async with aiohttp.ClientSession() as session:
+                async with session.ws_connect(self.endpoint) as ws:
+                    self.client = LMTPWebSocketClient(self.model.model_identifier, ws)
+                    self.client.connect()
+                    
+                    self.connected_signal.set()
+                    await self.close_signal.wait()
+        except Exception as e:
+            print("Failed to communicate with lmtp endpoint: {}".format(self.endpoint), flush=True)
+            self.error_signal.set()
+            self.connected_signal.set()
+
+    def make_cache_entry(self, s, payload, sampling_mode):
+        scores = {}
+        for t, score in payload["top_logprobs"].items():
+            scores[int(t)] = score
+        
+        if sampling_mode == "top-1":
+            scores[int(payload["token"])] = payload["logprob"]
+
+        top_entries = list(sorted(scores.items(), key=lambda x: x[1], reverse=True))
+        tokens = [t for t, _ in top_entries]
+        scores = [s for _, s in top_entries]
+        edge_type = ["top-{}".format(i+1) for i in range(len(top_entries))]
+        
+        # for non argmax sampling modes, add the sampled token
+        if sampling_mode != "top-1":
+            tokens = [payload["token"]] + tokens
+            scores = [payload["logprob"]] + scores
+            edge_type = [sampling_mode] + edge_type
+
+        tokens = self.tokenizer.decode_bytes(tokens)
+
+        return (s, tokens, scores, edge_type, {})
+
+    async def stream_and_return_first(self, s, iterator, sampling_mode):
+        buffer = []
+        for i in range(4):
+            try:
+                buffer += [await anext(iterator)]
+            except StopAsyncIteration:
+                break
+        self.requests += 1
 
-    def run_in_parallel(self, n=2):
-        atexit.register(self.shutdown)
-        
-        workers = []
+        async def token_stream():
+            nonlocal buffer
 
-        for i in range(n):
-            p = multiprocessing.Process(target=self.run, args=(i,))
-            p.start()
-            workers.append(p)
-        
-        return workers
-
-class ModelProcessor:
-    def __init__(self, state: InferenceServerState, cuda: bool = False, cache: str = None, ready_event: multiprocessing.Event = None):
-        self.model_identifier = state.model_identifier
-        self.queue = state.queue
-        self.state = state
-        self.cuda = cuda
-        self.ready_event = ready_event
-        
-        self.cache = None
-        if cache is not None:
-            from rocksdict import Rdict
-            self.cache = Rdict(cache)
+            self.tokens += 1
             
-        self.request_count = 0
-        self.requests_cached = 0
-        self.last_report = time.time()
-        self.last_request_count = 0
+            for item in buffer:
+                yield self.make_cache_entry(s, item, sampling_mode)
+
+            while True:
+                try:
+                    self.tokens += 1
+                    item = await anext(iterator)
+                    yield self.make_cache_entry(s, item, sampling_mode)
+                except StopAsyncIteration:
+                    is_done = True
+                    break
+        
+        async def do_register():
+            self.register_token_stream(token_stream)
+        asyncio.ensure_future(do_register())
+        
+        return buffer[0]
+
+    async def ensure_connected(self):
+        if self.error_signal.is_set():
+            raise RuntimeError("LMTP client encountered an error")
+
+        if self.client is None:
+            if not self.inprocess:
+                self._client_loop = asyncio.create_task(self.ws_client_loop())
+            else:
+                self._client_loop = asyncio.create_task(self.inprocess_client_loop())
         
-        try:
-            self.nvidia_logging = subprocess.Popen(["nvidia-smi"], stdout=subprocess.PIPE).wait() == 0
-        except:
-            self.nvidia_logging = False
+        await self.connected_signal.wait()
+        
+        # double check for errors
+        if self.error_signal.is_set():
+            raise RuntimeError("LMTP client encountered an error")
+
+    # on deinit
+    def close(self):
+        self.close_signal.set()
 
-    def shutdown(self):
-        self.state.exit = True
-    
     def __del__(self):
-        if self.cache is not None:
-            self.cache.close()
-        
-    def print_stats(self):
-        if self.nvidia_logging:
-            visible_devices = os.environ.get("CUDA_VISIBLE_DEVICES", None)
-            cmds = ["nvidia-smi"]
-            if visible_devices is not None:
-                cmds.append("-i={}".format(visible_devices))
-            cmds += ["--query-gpu=name,memory.used,memory.total,utilization.gpu", "--format=csv,noheader"]
-            output = [l.split(", ") for l in subprocess.check_output(cmds).decode("utf-8").split("\n") if l.strip() != ""]
-            gpu_usage = ["GPU {} {}, util {}".format(i, row[1] + "/" + row[2], row[3]) for i, row in enumerate(output)]
-        else:
-            gpu_usage = ["GPU monitoring not available on non-CUDA systems"]
-        
-        print(" " * 100, end="\r")
-        # fancy unicode based terminal spinner
-        terminal_spinner_chars = ["⠋", "⠙", "⠹", "⠸", "⠼", "⠴", "⠦", "⠧", "⠇", "⠏"]
-        throughput = (self.request_count - self.last_request_count) / (time.time() - self.last_report)
-        self.last_report = time.time()
-        self.last_request_count = self.request_count
-        
-        # format throughput to two decimal places
-        print("{} {:.2f} calls/s, Requests Served: {}, Queue: {} [{}]".format(
-            terminal_spinner_chars[self.request_count % len(terminal_spinner_chars)], 
-            throughput,
-            self.request_count, 
-            self.state.queue.qsize(), 
-            ", ".join(gpu_usage)), end="\r")
-
-    def run(self):
-        dtype = self.state.dtype
-        load_in_8bit = dtype == "8bit"
-        if dtype == "float16":
-            dtype = torch.float16
-        else:
-            dtype = None
-        
-        # load model
-        if not self.cuda:
-            print("Loading {} (CPU)".format(self.model_identifier))
-            self.model = AutoModelForCausalLM.from_pretrained(self.model_identifier, torch_dtype=dtype, resume_download=True)
-        else:
-            print("Loading {} (Multi-GPU)".format(self.model_identifier))
-            self.model = AutoModelForCausalLM.from_pretrained(self.model_identifier, torch_dtype=dtype, resume_download=True, load_in_8bit=load_in_8bit, device_map="auto")
-        self.model.eval()
-        
-        print("Ready!".format(self.model_identifier))
-
-        if self.ready_event:
-            self.ready_event.set()
-
-        while not self.state.exit:
-            self.print_stats()
-            # wait for self.queue to have an item
-            try:
-                item = self.queue.get(timeout=1.0)
-            except Empty:
-                continue
-            except KeyboardInterrupt:
-                break
+        self.close_signal.set()
 
-            if item is None: 
-                time.sleep(0.1)
-                continue
-
-            self.request_count += 1
-        
-            device = "cuda" if self.cuda else "cpu"
-
-            sample_id = item["sample_id"]
-            client_id = item["client_id"]
-            input_ids = torch.tensor(item["input_ids"], dtype=torch.long).to(device)
-            attention_mask = item.get("attention_mask", None)
+    def make_logits(self, payload):
+        scores = {}
+        for t, score in payload["top_logprobs"].items():
+            scores[int(t)] = score
+        scores[int(payload["token"])] = payload["logprob"]
+        scores = scores.items()
+
+        logits = np.ones(self.tokenizer.vocab_size) * self.truncation_threshold
+        logits[[t for t, _ in scores]] = [s for _, s in scores]
+
+        return logits
+
+    async def singleton_result(self, token, score):
+        yield {"token": token, "logprob": score, "top_logprobs": {token: score}}
+
+    async def generate(self, s, temperature, top_logprobs = 1, chunk_size=None, **kwargs):
+        if chunk_size is None:
+            chunk_size = self.model.chunk_size
+        kwargs = {**self.model_args, **kwargs}
+
+        constrained_seqs = np.array([s.is_query_constrained], dtype=np.bool_)
+        logits_mask_result = await self.compute_logits_mask(s.input_ids.reshape(1, -1), [s.user_data], constrained_seqs, [s], **kwargs)
+
+        mask = logits_mask_result.logits_mask[0]
+
+        if mask is not None:
+            num_allowed = masks.mask_num_allowed(mask)
+            if num_allowed == 1:
+                only_allowed_id = masks.mask_get_only_allowed(mask)
+                return self.singleton_result(only_allowed_id, 0.0)
             
-            if attention_mask is None:
-                attention_mask = torch.ones_like(input_ids).to(device)
-            else:
-                attention_mask = torch.tensor(attention_mask, dtype=torch.long).to(device)
+            assert nputil.is_array(mask), "logit_mask_or_fixed_id must be a LongTensor not a " + str(type(mask))
+            invert = num_allowed < self.tokenizer.vocab_size - num_allowed
 
-            if self.cache is not None:
-                key = "IDs:" + str(input_ids.tolist()) + " MASK:" + str(attention_mask.tolist())
-                if key in self.cache:
-                    self.requests_cached += 1
-                    self.state.all_results_queue.put({
-                        "client_id": client_id,
-                        "sample_id": sample_id,
-                        "next_token_logits": self.cache[key]
-                    })
-                    continue
-            
-            res = self.model.forward(input_ids=input_ids, attention_mask=attention_mask)
+            if invert: masked = (mask >= 0)
+            else: masked = (mask < 0)
+            mask_value = 100 if invert else -100
+            mask = {int(idx): mask_value for idx in np.nonzero(masked)[0]}
+
+        ids = self.tokenizer.convert_bytes_to_ids(s.input_ids)
+
+        return self.client.generate(ids, max_tokens=chunk_size, temperature=temperature, logit_bias=mask, top_logprobs=top_logprobs)
+
+    async def argmax(self, sequences: dc.DataArray, **kwargs):
+        return await self.sample(sequences, temperature=0.0, **kwargs)
+
+    async def sample(self, sequences: dc.DataArray, temperature, **kwargs):
+        await self.ensure_connected()
+        
+        sampling_mode = "top-1" if temperature == 0.0 else "sample-{}".format(temperature)
+
+        assert kwargs.get("num_samples", 1) == 1, "LMTPModel does not support num_samples != 1"
+
+        async def op_sample(seqs):
+            if len(seqs) == 0:
+                return []
             
-            if input_ids.ndimension() == 2:
-                next_token_logits = res.logits[:,-1]
-            else:
-                next_token_logits = res.logits[-1]
+            if all(type(s) is dc.DeterministicDecoderSequence for s in seqs) and all(len(s.next_ids) > 0 for s in seqs):
+                next_token_ids = np.array([s.next_ids[0] for s in seqs])
+                next_token_scores = np.array([s.next_logprobs[0] for s in seqs])
+                next_token_ids = np.array([self.tokenizer.decode_bytes([t])[0] for t in next_token_ids])
+                return [s.make_successors(next_token_ids[i].reshape(1), next_token_scores[i], logits=None) for i,s in enumerate(seqs)]
             
-            if self.cache is not None:
-                key = "IDs:" + str(input_ids.tolist()) + " MASK:" + str(attention_mask.tolist())
-                self.cache[key] = next_token_logits.tolist()
-
-            self.state.all_results_queue.put({
-                "client_id": client_id,
-                "sample_id": sample_id,
-                "next_token_logits": next_token_logits.detach().tolist()
-            })
-        
-        print("Processor shut down")
+            self.model.num_queries += len(seqs)
+            tokens = await asyncio.gather(*[self.stream_and_return_first(s, await self.generate(s, temperature=temperature, **kwargs), sampling_mode) for s in seqs])
 
-    def oom_reloading_run(self):
-        while True:
-            try:
-                self.run()
-                return
-            except RuntimeError as e:
-                if "CUDA out of memory" in str(e):
-                    print("Crashed due to OOM, reloading model.")
-                    continue
-                else:
-                    import traceback
-                    traceback.print_exc()
-                    print("Crashed with", e, "reloading model...")
-                    continue
-
-    def run_in_parallel(self):
-        atexit.register(self.shutdown)
-
-        p = multiprocessing.Process(target=self.oom_reloading_run)
-        p.start()
-        return p
-
-class LMQLInferenceAPIHandler(BaseHTTPRequestHandler):
-    def __init__(self, *args, **kwargs):
-        self._client_id = None
-        super().__init__(*args, **kwargs)
-
-    # disable logging
-    def log_message(self, format, *args):
-        return
-
-    @property
-    def state(self) -> InferenceServerState:
-        return self.server.state
-    
-    @property
-    def client_id(self) -> str:
-        if self._client_id is None:
-            self.error_bad_request(msg="client_id not set (please provide the client_id in POST payload or in query.")
-            raise Exception("client_id not set")
-        return self._client_id
-
-    def error_bad_request(self, msg="Bad request."):
-        self.send_response(400)
-        self.send_header('Content-type', 'text/plain')
-        self.end_headers()
-        self.wfile.write(msg.encode("utf-8"))
+            next_token_ids = np.array([t['token'] for t in tokens], dtype=np.int64)
+            next_token_scores = np.array([t['logprob'] for t in tokens], dtype=np.float32)
+            next_logits = np.array([self.make_logits(t) for t in tokens], dtype=np.float32)
 
-    def process_some_all_results(self, max=10):
-        all_results_queue = self.state.all_results_queue
-        i = 0
+            next_tokens = np.array([self.tokenizer.decode_bytes([t])[0] for t in next_token_ids])
+
+            return [s.make_successors(next_tokens[i].reshape(1), next_token_scores[i], logits=next_logits[i]) for i,s in enumerate(seqs)]
         
-        while not all_results_queue.empty() and i < max:
-            result = all_results_queue.get()
+        return await sequences.aelement_wise(op_sample)
 
-            result_client_id = result["client_id"]
-            
-            if result_client_id not in self.state.client_results_queues:
-                self.state.client_results_queues[result_client_id] = Queue()
-            self.state.client_results_queues[result_client_id].put(result)
+    async def topk_continuations(self, sequences, k, **kwargs):
+        await self.ensure_connected()
 
-            i += 1
+        kwargs = {**self.model_args, **kwargs}
 
-    def do_GET_results(self):
-        request_client_id = self.path.split("/")[2]
-        self._client_id = f"{self.client_address[0]}-{request_client_id}"
-
-        self.send_response(200)
-        self.send_header('Content-type', 'application/json')
-        self.end_headers()
+        async def op_topk(seqs, k):
+            if len(seqs) == 0:
+                return []
 
-        # process some results from the model and group them by client_id
-        self.process_some_all_results()
+            if all(type(s) is dc.DeterministicDecoderSequence for s in seqs) and all(len(s.next_ids) > 0 for s in seqs):
+                next_token_ids = np.array([s.next_ids[0] for s in seqs])
+                next_token_scores = np.array([s.next_logprobs[0] for s in seqs])
+                next_token_ids = np.array([self.tokenizer.decode_bytes([t])[0] for t in next_token_ids])
+                return [s.make_successors(next_token_ids[i].reshape(1), next_token_scores[i], logits=None) for i,s in enumerate(seqs)]
 
-        if self.client_id not in self.state.client_results_queues.keys():
-            self.wfile.write(b'[]')
-            return
+            self.model.num_queries += len(seqs)
+            result = await asyncio.gather(*[self.stream_and_return_first(s, await self.generate(s, temperature=0.0, top_logprobs=k, chunk_size=None if k == 1 else 1, **kwargs), "top-1") for s in seqs])
 
-        # return all results for self.client_id currently available
-        self.wfile.write("[".encode())
-        while not self.state.client_results_queues[self.client_id].empty():
-            result = self.state.client_results_queues[self.client_id].get()
-            self.wfile.write(json.dumps(result).encode())
-            
-            # omit last colon
-            if self.state.client_results_queues[self.client_id].empty(): break
-            else: self.wfile.write(b",")
-        self.wfile.write(b"]")
-
-    def do_queue_forward(self, payload, sample_id):
-        try: 
-            input_ids = payload['input_ids']
-            attention_mask = payload.get('attention_mask', None)
-            model_identifier = payload['model_identifier']
-
-            if model_identifier != self.state.model_identifier:
-                self.error_bad_request("The inference API serves model {} not {}.".format(self.state.model_identifier, model_identifier))
-                return
-
-            self._client_id = f"{self.client_address[0]}-{payload['client_id']}"
-
-            assert type(input_ids) == list # and all([type(i) == int for i in input_ids])
-
-            self.state.queue.put({
-                'client_id': self.client_id,
-                'sample_id': sample_id,
-                'input_ids': input_ids,
-                'attention_mask': attention_mask
-            })
-
-            self.send_response(200)
-            self.send_header('Content-type', 'application/json')
-            self.end_headers()
-            self.wfile.write(json.dumps({'sample_id': sample_id}).encode())
-        except Exception as e: 
-            self.error_bad_request()
-
-    def do_queue_tokenize(self, payload, sample_id):
-        try: 
-            text = payload['text']
-            self._client_id = f"{self.client_address[0]}-{payload['client_id']}"
-
-            assert type(text) == str
-
-            self.state.tokenize_queue.put({
-                'client_id': self.client_id,
-                'sample_id': sample_id,
-                'action': 'tokenize',
-                'text': text
-            })
-
-            self.send_response(200)
-            self.send_header('Content-type', 'application/json')
-            self.end_headers()
-            self.wfile.write(json.dumps({'sample_id': sample_id}).encode())
-        except Exception as e: 
-            self.error_bad_request()
-        
-    def do_queue_detokenize(self, payload, sample_id):
-        try: 
-            input_ids = payload['input_ids']
-            self._client_id = f"{self.client_address[0]}-{payload['client_id']}"
-
-            assert type(input_ids) == list and all([type(i) == int for i in input_ids])
-
-            self.state.tokenize_queue.put({
-                'client_id': self.client_id,
-                'sample_id': sample_id,
-                'action': 'detokenize',
-                'input_ids': input_ids
-            })
-
-            self.send_response(200)
-            self.send_header('Content-type', 'application/json')
-            self.end_headers()
-            self.wfile.write(json.dumps({'sample_id': sample_id}).encode())
-        except Exception as e: 
-            self.error_bad_request()
-
-    def do_POST_queue(self):
-        # handle POST to /queue
-        payload = self.rfile.read(int(self.headers['Content-Length']))
-        payload = json.loads(payload)
-        # get client address and port
-        sample_id = payload["sample_id"]
-
-        action = payload['action']
-
-        if action == "forward":
-            self.do_queue_forward(payload, sample_id)
-        elif action == "tokenize":
-            self.do_queue_tokenize(payload, sample_id)
-        elif action == "detokenize":
-            self.do_queue_detokenize(payload, sample_id)
-        else:
-            self.error_bad_request("Unknown action: {}".format(action))
-
-    def do_POST(self):
-        if self.path == "/queue":
-            self.do_POST_queue()
-            return
-        else:
-            self.send_error(404)
-            return
+            logits = []
+            next_token_ids = []
+            next_token_scores = []
 
-    def do_GET(self):
-        if self.path.startswith("/results"):
-            self.do_GET_results()
-            return
-        else:
-            self.send_error(404)
+            for i, s in enumerate(seqs):
+                # prepare distribution
+                distribution = TokenDistribution()
+                logprob_items = result[i]["top_logprobs"].items()
+                
+                logprobs = [logprob for _, logprob in logprob_items]
+                tokens = [int(token) for token, _ in logprob_items]                
+                chosen_token = result[i]["token"]
+                chosen_logprob = result[i]["logprob"]
+                tokens += [chosen_token]
+                logprobs += [chosen_logprob]
+                
+                tokens = np.array([self.tokenizer.decode_bytes([t])[0] for t in tokens])
+
+                distribution[tokens] = logprobs
+
+                # make sure all token_ids are unique
+                tokens = np.array(list(set(tokens)))
+
+                tokens, logprobs = distribution.topk(k)
+
+                next_token_ids.append(tokens)
+                next_token_scores.append(logprobs)
+                logits.append(distribution)
+
+            return [s.make_successors(next_token_ids[i], next_token_scores[i], logits=logits[i], user_data=None) for i,s in enumerate(seqs)]
+
+        return await sequences.aelement_wise(op_topk, k=k)
+
+    def report_stats(self, printer, decoder_step=None):
+        if printer is None:
             return
+        if hasattr(printer, "report_model_stats"):
+            data = {
+                "tokens": self.tokens,
+                "model": self.model_identifier,
+                "req.": self.requests,
+                "avb": 0,
+            }
+            if decoder_step is not None:
+                data["_step"] = decoder_step
+            printer.report_model_stats(**data)
+
+    async def _score_next_tokens(self, s, next_tokens, noscore=False):
+        if noscore:
+            return np.zeros(len(next_tokens), dtype=np.float32)
+        
+        scores = []
+        i = 0
+        
+        ids = self.tokenizer.convert_bytes_to_ids(s.input_ids)
+        next_tokens = self.tokenizer.convert_bytes_to_ids(next_tokens)
 
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
-    parser.add_argument("model", type=str)
-    parser.add_argument("--tokenizer", type=str, default=None)
-    parser.add_argument("--port", type=int, default=8080)
-    parser.add_argument("--host", type=str, default="localhost")
-    parser.add_argument("--cuda", action="store_true", default=False)
-    parser.add_argument("--cache", type=str, default=None)
-    parser.add_argument("--dtype", type=str, default="none", help="What format to load the model weights. Options: 'float16' (not available on all models), '8bit' (requires bitsandbytes)")
-    parser.add_argument("--wait_until_ready", action="store_true", default=False, help="Whether the server should start only after the model and tokenizer have been loaded.")
-    parser.add_argument("--num-tokenizer-processes", type=int, default=2, dest="num_tokenizer_processes")
-    
-    args = parser.parse_args()
+        async for token in self.client.score(ids, next_tokens):
+            t = next_tokens[i]
+            assert token["token"] == t, "Expected token {}, got {}".format(t, token["token"])
+            scores.append(token["logprob"])
+            i += 1
+        assert len(scores) == len(next_tokens), "Expected {} scores, got {}".format(len(next_tokens), len(scores))
+        
+        return np.array(scores, dtype=np.float32)
     
-    manager = multiprocessing.Manager()
+    async def score(self, sqs: List[dc.DecoderSequence], tokens: List[List[int]], max_batch_size=4, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False, internal=False):
+        await self.ensure_connected()
+        
+        assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
+
+        def make_detseq(s, token_score, completion):
+            # compose deterministic flags
+            if type(deterministic) is bool:
+                deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])])
+                next_deterministic = np.array([deterministic] * len(completion[1:]))
+            else:
+                assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored, but is {} and {}".format(deterministic, completion)
+                deterministic_flags = np.concatenate([s.deterministic, np.array(deterministic[:1])])
+                next_deterministic = np.array(deterministic[1:])
+
+            return dc.detseq(ids=np.concatenate([s.input_ids, completion[:1]], axis=0), 
+                    next_ids=completion[1:],
+                    logprobs=np.concatenate([s.logprobs, token_score[:1]], axis=0),
+                    next_logprobs=token_score[1:],
+                    deterministic=deterministic_flags,
+                    next_deterministic=next_deterministic,
+                    predecessor=s,
+                    user_data=user_data,
+                    stop_phrase=np.concatenate([s.stop_phrase, np.array([stop_phrase])]),
+                    needs_rewrite=needs_rewrite,
+                    sticky_user_data_keys=s.sticky_user_data_keys,
+                    internal=internal
+            )
+        results = []
+
+        async for (s, tokens, scores) in self.score_tokens(sqs, tokens, max_batch_size=max_batch_size, noscore=noscore):
+            results.append(make_detseq(s, scores, tokens))
+
+        return results
     
-    # prepare configuration
-    model_descriptor = args.model
-    tokenizer_descriptor = args.tokenizer
-    if tokenizer_descriptor is None:
-        tokenizer_descriptor = model_descriptor
-    state = InferenceServerState(model_descriptor, 
-                                 tokenizer_descriptor, 
-                                 args.dtype, 
-                                 queue=manager.Queue(), 
-                                 tokenize_queue=manager.Queue(),
-                                 all_results_queue=manager.Queue())
-
-    # run model in separate process
-    processor = ModelProcessor(state, cuda=args.cuda, cache=args.cache, ready_event=(multiprocessing.Event() if args.wait_until_ready else None))
-    processor.run_in_parallel()
-
-    # run tokenizers in separate process
-    tokenizer_processor = TokenizerProcessor(state, ready_event=(multiprocessing.Event() if args.wait_until_ready else None))
-    tokenizer_processor.run_in_parallel(n=args.num_tokenizer_processes)
-
-    # don't serve until the model and tokenizer are ready
-    if args.wait_until_ready:
-        processor.ready_event.wait()
-        tokenizer_processor.ready_event.wait()
-
-    # run inference API server in this process
-    server_address = (args.host, args.port)
-    httpd = HTTPServer(server_address, LMQLInferenceAPIHandler)
-    httpd.state = state
+    async def score_tokens(self, sqs: List[dc.DecoderSequence], tokens: List[List[int]], max_batch_size=None, noscore=False):
+        completion = [np.array(cont) for cont in tokens]
+
+        for s, tokens, scores in zip(sqs, completion, await asyncio.gather(*(self._score_next_tokens(s, compl, noscore=noscore) for s, compl in zip(sqs, completion)))):
+            yield (s, tokens, scores)
+
+class lmtp_model:
+    """
+    Factory class for LMTPModelCls client instances.
+
+    In case of inprocess=True, lmtp_model keeps a reference to the internally instantiated 
+    LMTPMultiProcessingClient to share it between all uses of the resulting LMTPModelCls 
+    across several queries.
+    """
+    def __init__(self, model_identifier, inprocess=False, endpoint=None, **kwargs):
+        self.model_identifier = model_identifier
+        self.tokenizer_identifier = kwargs.pop("tokenizer", self.model_identifier)
+
+        self.inprocess = inprocess
+        self.endpoint = endpoint
+        self.kwargs = kwargs
+
+        self.lmtp_inprocess_client = None
     
-    try:
-        print("Serving LMQL inference API on {}:{}".format(args.host, args.port))
-        httpd.serve_forever()
-    except KeyboardInterrupt:
-        # terminate server
-        httpd.shutdown()
-        httpd.server_close()
-        print("Server stopped")
-
-    # terminate processors
-    processor.shutdown()
-    tokenizer_processor.shutdown()
+    # ensures that all inprocess lmtp models instantiated via this class 
+    # share the same underlying LMTPMultiProcessingClient instance
+    # (uses reference counting to ensure that the client is only shut down 
+    # once all LMTPModel instances have closed)
+    def inprocess_client_constructor_factory(self, identifier, **kwargs):
+        assert identifier == self.model_identifier, "Model identifier mismatch: {} vs {}".format(self.model_identifier, identifier)
+        
+        if self.lmtp_inprocess_client is None:
+            # ref owned by self
+            self.lmtp_inprocess_client = LMTPMultiProcessingClient(identifier, **kwargs).ref()
+            # ref owned by caller
+            return self.lmtp_inprocess_client.ref()
+        
+        # ref owned by caller
+        return self.lmtp_inprocess_client.ref()
+
+    def __del__(self):
+        if self.lmtp_inprocess_client is not None:
+            asyncio.ensure_future(self.lmtp_inprocess_client.close())
+            # print("closing shared LMTPMultiProcessingClient instance for model {}".format(self.model_identifier), self.lmtp_inprocess_client.refs, flush=True)
+
+    def __call__(self):
+        # reference to factory instance
+        this = self
+
+        class LMTPModelCls:
+            def __init__(self) -> None:
+                self.model_identifier = this.model_identifier
+                self.served_model = None
+                self._tokenizer = None
+
+                self.decoder_args = {}
+
+                self.num_queries = 0
+
+            def get_tokenizer(self):
+                if self._tokenizer is None:
+                    self._tokenizer = load_tokenizer(this.tokenizer_identifier)
+                self.served_model = self
+                return self._tokenizer
+
+            def get_dclib_model(self):
+                bos_token_id = self.get_tokenizer().bos_token_id
+                eos_token_id = self.get_tokenizer().eos_token_id
+
+                dc.set_dclib_tokenizer(self.get_tokenizer())
+
+                inprocess_client_constructor = None
+
+                if this.inprocess:
+                    lmtp_server_kwargs = this.kwargs
+                    inprocess_client_constructor = this.inprocess_client_constructor_factory
+                else:
+                    lmtp_server_kwargs = None
+
+                return LMTPModel(self, self.get_tokenizer(), inprocess=this.inprocess, endpoint=this.endpoint, lmtp_server_kwargs=lmtp_server_kwargs, inprocess_client_constructor=inprocess_client_constructor, **self.decoder_args)
+
+            async def tokenize(self, text):
+                return self.get_tokenizer().tokenize(text, asbytes=True)
+            
+            async def detokenize(self, input_ids):
+                return self.get_tokenizer().decode(input_ids)
+
+            def sync_tokenize(self, text):
+                return self.get_tokenizer()(text)["input_ids"]
+            
+            def report_metrics(self, metrics):
+                pass
+
+        return LMTPModelCls()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lmql-0.0.6.3/src/lmql/ops/follow_map.py` & `lmql-0.0.6.4/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ops/ops.py` & `lmql-0.0.6.4/src/lmql/ops/ops.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ops/token_set.py` & `lmql-0.0.6.4/src/lmql/ops/token_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         if VocabularyMatcher._instance is not None:
             return
 
         # first try to load pickled matcher from cache (faster)
         import pickle
 
         cache_identifier = tokenizer.model_identifier.replace("/", "-")
+        cache_identifier += "-" + type(tokenizer.tokenizer_impl).__name__.replace("[^a-z0-9]", "")
         cache_path = f"token-mask-cache-{cache_identifier}.pkl"
         matcher_path = f"matcher-{cache_identifier}.pkl"
 
         try:
             with cachefile(matcher_path, "rb") as f:
                 VocabularyMatcher._instance = pickle.load(f)
                 VocabularyMatcher._instance.stats = Stats("VocabularyMatcher")
@@ -65,15 +66,16 @@
 
         atexit.register(lambda: VocabularyMatcher._instance.save())
 
     def save(self):
         # save cache to disk
         import pickle
 
-        cache_identifier = self.model_identifier.replace("/", "-")
+        cache_identifier = self.tokenizer.model_identifier.replace("/", "-")
+        cache_identifier += "-" + type(self.tokenizer.tokenizer_impl).__name__.replace("[^a-z0-9]", "")
         cache_path = f"token-mask-cache-{cache_identifier}.pkl"
         matcher_path = f"matcher-{cache_identifier}.pkl"
 
         with cachefile(matcher_path, "wb") as f:
             stats = self.stats
             self.stats = None
             pickle.dump(self, f)
@@ -110,15 +112,15 @@
             for k in keys:
                 VocabularyMatcher.cache[k] = result
             return result
 
     def mask_cache_name(self, tokens=None, regex=None, minus=None, prefix=None, exact=None, charlen=None, name=None):
         keys = ["named:" + name] if name is not None else []
         if regex is not None:
-            return keys + ["regex:"]
+            return keys + ["regex:" + regex]
         elif charlen is not None:
             return keys + ["charlen:" + str(charlen)]
         else:
             assert tokens is not None
             t = ("prefix " if prefix else "") + ("* \ " if minus else "") + "|".join(sorted(list(tokens)))
             return keys + [t]
 
@@ -183,14 +185,15 @@
                     mask[t] = True
             else:
                 if any(t for t in tokens if t != "eos") > 0:
                     def process(t):
                         t = t.replace(".", "\\.")
                         t = t.replace(" ", self.space_repr)
                         t = t.replace("\n", self.nl_repr)
+                        t = re.escape(t)
                         return t
                     if exact: 
                         # only allow exact matches
                         pattern = "|".join(f"({process(t)})" for t in tokens if t != "eos")
                         pattern = re.compile(pattern, re.UNICODE)
                         matcher = pattern.fullmatch
                     else:
@@ -537,15 +540,18 @@
 
 def charlen_tsets():
     l1 = tset(charlen=1)
     token_lengths = VocabularyMatcher.instance().token_lengths
     assert token_lengths is not None, "VocabularyMatcher.instance().token_lengths is None even though it should be fully initialized."
     # get unique values in token_lengths (numpy)
     length_values = np.unique(token_lengths)
-    return {int(l): tset(charlen=l) for l in length_values}
+    tsets = {int(l): tset(charlen=l) for l in length_values}
+    # only eos should have charlen 0
+    tsets[0] = tset("eos") 
+    return tsets
 
 def ntset(*tokens):
     if len(tokens) == 1 and type(tokens[0]) is set:
         return TokenSet(set(list(tokens[0])), minus=True)
     return TokenSet(set(tokens), minus=True)
 
 class ArgTuple(tuple):
```

### Comparing `lmql-0.0.6.3/src/lmql/output/http.py` & `lmql-0.0.6.4/src/lmql/output/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/output/sse.py` & `lmql-0.0.6.4/src/lmql/output/sse.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/output/ws.py` & `lmql-0.0.6.4/src/lmql/output/ws.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.6.4/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.6.4/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,22 +86,32 @@
         self.tasks = []
 
 def make_request_args(tasks):
     prompts = [t["prompt"] for t in tasks]
     futures = [t["future"] for t in tasks]
     request_ids = [t["request_id"] for t in tasks]
 
+    api_configs = [t.get("api_config", None) for t in tasks if t.get("api_config") is not None]
+    api_config = api_configs[0] if len(api_configs) > 0 else None
+
+    timeouts = [t.get("timeout", None) for t in tasks if t.get("timeout") is not None]
+    timeout = max(timeouts) if len(timeouts) > 0 else None
+
     # construct request arguments
     request_args = tasks[0].copy()
     del request_args["future"]
     
     request_args["prompt"] = prompts
     request_args["futures"] = futures
     request_args["request_id"] = request_ids
     request_args["stream"] = True
+    request_args["timeout"] = timeout
+    
+    if api_config is not None: 
+        request_args["api_config"] = api_config
 
     return request_args
 
 @dataclass
 class Stats:
     prompt_tokens: int = 0
     tokens: int = 0
@@ -304,16 +314,14 @@
                     break
         return _aiter()
 
     async def get(self, i):
         while self.num_tokens <= i and self.iterator is not None:
             try:
                 chunk = await anext(self.iterator)
-                chunk["logprobs"]["tokens"] = await self.tokenizer(chunk["logprobs"]["tokens"])
-                # self.tokenizer(data["logprobs"]["tokens"])
                 self._append(chunk)
             except StopAsyncIteration:
                 break
         if i >= self.num_tokens:
             raise IndexError(f"index {i} out of bounds for response_buffer of length {self.num_tokens}. Iterator is {self.iterator}")
 
         text_start = self.logprobs["text_offset"][i]
@@ -350,20 +358,25 @@
     def __init__(self, slice):
         self.slice = slice
         self.retries = 0
         self.text = ""
         self.consumed_tokens = []
         self.n = 0
 
+        self.waiting_tasks = []
+
     async def recover(self):
         recovery_kwargs = self.slice.kwargs.copy()
         # reconstruct the prompt by tokenizing the consumed tokens
         if len(self.consumed_tokens) > 0:
             prompt = self.consumed_tokens
-            recovery_kwargs["prompt"] = [t[0] for t in prompt]
+            if type(prompt[0]) is str:
+                recovery_kwargs["prompt"] = "".join([t for t in prompt])
+            else:
+                recovery_kwargs["prompt"] = [t[0] for t in prompt]
         
         # issue new completion call
         new_slice = await self.slice.stream.scheduler.complete(**recovery_kwargs)
         new_it = ResponseStreamSliceIterator(new_slice)
         new_it.retries = self.retries + 1
 
         # print("recovery for request with ID", recovery_kwargs["request_id"])
@@ -392,41 +405,56 @@
                 
                 return partial_data
         self.text = new_it.text
         self.consumed_tokens = new_it.consumed_tokens
         self.slice = new_slice
         # otherwise the chunking aligns with the old stream, so we return the next chunk
         return await self.__anext__()
+    
+    def __del__(self):
+        """Make sure to clean up any pending tasks."""
+        for t in self.waiting_tasks:
+            try:
+                loop = asyncio.get_event_loop()
+                if not t.done() and not loop.is_closed():
+                    t.cancel()
+            except RuntimeError:
+                pass
 
     async def get_next(self):
         if self.slice.done.is_set(): 
             if self.n == 0:
                 return RecoveryAttempt(self.slice.kwargs, TimeoutError(), self.slice.maximum_retries)
             raise StopAsyncIteration
-        check_done_task = asyncio.create_task(self.slice.done.wait())
+        check_done_task = asyncio.create_task(self.slice.done.wait(), name="check_done_task")
+        self.waiting_tasks.append(check_done_task)
+        
         get_next_item_task = asyncio.create_task(self.slice.data_queue.get())
         done, pending = await asyncio.wait([get_next_item_task, check_done_task], 
-            return_when=asyncio.FIRST_COMPLETED, timeout=2.0)
-        
+            return_when=asyncio.FIRST_COMPLETED, timeout=5.0)
+    
+        self.waiting_tasks.remove(check_done_task)
 
         if check_done_task in done:
             # this indicates the end of this response stream
             for t in pending: t.cancel()
             if self.n == 0:
                 return RecoveryAttempt(self.slice.kwargs, TimeoutError(), self.slice.maximum_retries)
             raise StopAsyncIteration
         elif len(done) > 0:
             assert get_next_item_task in done, f"expected get_next_item_task to be done, but only {done} is done."
             # cancel self.done waiting task
             for t in pending: t.cancel()
+            check_done_task.cancel()
             # return with new data chunk
             self.n += 1
             return get_next_item_task.result()
         else:
             for t in pending: t.cancel()
+            check_done_task.cancel()
             # if after timeout this response has been fully consumed, we are done
             if self.slice.done.is_set() and self.n > 0:
                 raise StopAsyncIteration
             # otherwise return a RecoveryAttempt for retrying this request
             return RecoveryAttempt(self.slice.kwargs, TimeoutError(), self.slice.maximum_retries)
 
     async def __anext__(self):
@@ -657,15 +685,17 @@
                         res = await self._create(**kwargs)
                         break
                     except Exception as e:
                         if type(e) is AssertionError:
                             raise e
                         self.stats.errors += 1
                         retries -= 1            
-                        print("Failed to call complete endpoint", type(e), e, flush=True)
+                        print("OpenAI:", str(e), '"' + str(type(e)) + '"', flush=True)
+                        if kwargs.get("api_config", {}).get("errors", None) == "raise":
+                            raise e
                         await asyncio.sleep(0.5)
                         if retries <= 0 or self.is_definitive_error(e):
                             raise e
                         if type(e) is TimeoutError or type(e) is OpenAIRateLimitError:
                             t = (2.0 * random.random()) ** (self.maximum_retries - retries)
                             print("Backing off for", t , "seconds")
                             await asyncio.sleep(t)
@@ -706,15 +736,14 @@
             else:
                 biases = biases[:300]
             global logit_bias_logging
             if logit_bias_logging:
                 print("warning: the required logit_bias is too large to be handled by the OpenAI API and will be limited to the first 300 tokens. This can lead to the violation of the provided constraints or undesired model output. To avoid this use less broad or no constraints.", file=sys.stderr)
             kwargs["logit_bias"] = {t:b for t,b in biases}
 
-
         assert kwargs.get("echo", False), f"bopenai requires echo=True for to enable proper error recovery. Please handle proper prompt removal in client code."
 
         r = RequestQueueItem(kwargs, request_id)
         await self.complete_api_call_queue.put(r)
         self.request_ctr += 1
         if not self.is_available():
             raise APIShutDownException(f"bopenai requires at least one worker to be running to issue new complete requests.")
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.6.4/src/lmql/runtime/bopenai/openai_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 
 if "LMQL_BROWSER" in os.environ:
+    # use mocked aiohttp for browser (redirects to JS for network requests)
     import lmql.runtime.maiohttp as aiohttp
 else:
+    # use real aiohttp for python
     import aiohttp
 
-
 import json
 import time
 import asyncio
 
 from lmql.runtime.tokenizer import load_tokenizer
 from lmql.runtime.stats import Stats
 
@@ -57,79 +58,136 @@
         async for r in chat_api(**kwargs): yield r
     else:
         async for r in completion_api(**kwargs): yield r
 
 global tokenizer
 tokenizer = None
 
-def tokenize(text):
+def tokenize_ids(text):
     global tokenizer
     if tokenizer is None:
         tokenizer = load_tokenizer("gpt2")
-    return tokenizer(text)["input_ids"]
+    ids = tokenizer(text)["input_ids"]
+    return ids
 
-def detokenize(input_ids):
+def tokenize(text, openai_byte_encoding=False):
     global tokenizer
     if tokenizer is None:
         tokenizer = load_tokenizer("gpt2")
-        
-    while len(input_ids) > 0 and input_ids[0] == tokenizer.bos_token_id:
-        input_ids = input_ids[1:]
-    while len(input_ids) > 0 and input_ids[-1] == tokenizer.eos_token_id:
-        input_ids = input_ids[:-1]
-        
-    if len(input_ids) == 0:
-        return ""
-        
-    return tokenizer.decode(input_ids)
+    ids = tokenizer(text)["input_ids"]
+    raw = tokenizer.decode_bytes(ids)
+    if openai_byte_encoding:
+        raw = [str(t)[2:-1] for t in raw]
+        return [t.encode("utf-8").decode("unicode_escape") if not "\\x" in t else "bytes:" + t for t in raw]
+    else:
+        return raw
 
 def tagged_segments(s):
     import re
     segments = []
     current_tag = None
     offset = 0
     for m in re.finditer(r"<lmql:(.*?)\/>", s):
         if m.start() - offset > 0:
             segments.append({"tag": current_tag, "text": s[offset:m.start()]})
         current_tag = m.group(1)
         offset = m.end()
     segments.append({"tag": current_tag, "text": s[offset:]})
     return segments
 
-async def chat_api(**kwargs):
+
+def get_azure_config(model, api_config):
+    endpoint = api_config.get("endpoint", None)
+
+    # first check endpoint configuration
+    if endpoint is not None and endpoint.startswith("azure:"):
+        endpoint = "https:" + endpoint[6:]
+        env_name = model.upper().replace(".", "_")
+        
+        azure_key = api_config.get("azure_api_key", None)
+        if azure_key is None:
+            assert "AZURE_OPENAI_" + env_name + "_KEY" in os.environ, f"Please set the environment variable AZURE_OPENAI_{env_name}_KEY to your Azure API key, or specify it in code as 'lmql.model(..., azure_api_key=...')"
+            azure_key = os.environ["AZURE_OPENAI_" + env_name + "_KEY"]
+        
+        headers = {
+            "Content-Type": "application/json",
+            "api-key": azure_key,
+        }
+
+        return endpoint, headers
+
+    # then check env
+    if os.environ.get("OPENAI_API_TYPE", 'openai') == 'azure':
+        model_env_name = model.upper().replace(".", "_")
+        endpoint = os.environ[f"AZURE_OPENAI_{model_env_name}_ENDPOINT"]
+        assert "AZURE_OPENAI_" + model_env_name + "_KEY" in os.environ, f"Please set the environment variable AZURE_OPENAI_{model_env_name}_KEY to your Azure API key, or specify it in code as 'lmql.model(..., azure_api_key=...')"
+        key = os.environ[f"AZURE_OPENAI_{model_env_name}_KEY"]
+        headers = {
+            "Content-Type": "application/json",
+            "api-key": key,
+        }
+        return endpoint, headers
+
+def get_endpoint_and_headers(kwargs):
+    model = kwargs["model"]
+    api_config = kwargs.pop("api_config", {})
+    endpoint = api_config.get("endpoint", None)
+
+    # try to get azure config from endpoint or env
+    azure_config = get_azure_config(model, api_config)
+    if azure_config is not None:
+        return azure_config
+    
+    # otherwise use custom endpoint as plain URL without authorization
+    if endpoint is not None:
+        if not endpoint.endswith("http"):
+            endpoint = f"http://{endpoint}"
+        return endpoint + "/completions", {
+            "Content-Type": "application/json"
+        }
+    
+    # use standard public API config
     from lmql.runtime.openai_secret import openai_secret, openai_org
+    if kwargs["model"].startswith("gpt-3.5-turbo") or "gpt-4" in kwargs["model"]:
+        endpoint = "https://api.openai.com/v1/chat/completions"
+    else:
+        endpoint = "https://api.openai.com/v1/completions"
+    return endpoint, {
+        "Authorization": f"Bearer {openai_secret}",
+        "Content-Type": "application/json",
+    }
+
+async def chat_api(**kwargs):
     global stream_semaphore
 
     num_prompts = len(kwargs["prompt"])
     max_tokens = kwargs.get("max_tokens", 0)
 
     assert "logit_bias" not in kwargs.keys(), f"Chat API models do not support advanced constraining of the output, please use no or less complicated constraints."
-        
+    prompt_tokens = tokenize(kwargs["prompt"][0], openai_byte_encoding=True)
 
-    # transform prompt into chat API format
-    prompt_ids = kwargs["prompt"]
-    kwargs["prompt"] = [detokenize(p) for p in kwargs["prompt"]]
+    timeout = kwargs.pop("timeout", 1.5)
     
     echo = kwargs.pop("echo")
-    
+
     if echo:
         data = {
             "choices": [
                 {
-                    "text": p,
-                    "index": i,
+                    "text": kwargs["prompt"][0],
+                    "index": 0,
                     "finish_reason": None,
                     "logprobs": {
                         "text_offset": [0 for t in prompt_tokens],
                         "token_logprobs": [0.0 for t in prompt_tokens],
-                        "tokens": [[t] for t in prompt_tokens],
+                        "tokens": prompt_tokens,
                         "top_logprobs": [{t: 0.0} for t in prompt_tokens]
                     }
                 }
-             for i,(p,prompt_tokens) in enumerate(zip(kwargs["prompt"], prompt_ids)) ]
+            ]
         }
         yield data
     
     if max_tokens == 0:
         return
     
     assert len(kwargs["prompt"]) == 1, f"chat API models do not support batched processing"
@@ -161,68 +219,72 @@
 
     async with CapacitySemaphore(num_prompts * max_tokens):
         
         current_chunk = ""
         stream_start = time.time()
         
         async with aiohttp.ClientSession() as session:
+            endpoint, headers = get_endpoint_and_headers(kwargs)
             async with session.post(
-                "https://api.openai.com/v1/chat/completions",
-                headers={
-                    "Authorization": f"Bearer {openai_secret}",
-                    "Content-Type": "application/json",
-                },
-                json={**kwargs},
+                    endpoint,
+                    headers=headers,
+                    json={**kwargs},
             ) as resp:
                 last_chunk_time = time.time()
                 sum_chunk_times = 0
                 n_chunks = 0
                 current_chunk_time = 0
 
                 async def chunk_timer():
                     nonlocal last_chunk_time, sum_chunk_times, n_chunks, current_chunk_time
                     while True:
                         await asyncio.sleep(0.5)
                         current_chunk_time = time.time() - last_chunk_time
                         # print("Average chunk time:", sum_chunk_times / n_chunks, "Current chunk time:", current_chunk_time)
                         # print("available capacity", Capacity.total - Capacity.reserved, "reserved capacity", Capacity.reserved, "total capacity", Capacity.total, flush=True)
 
-                        if current_chunk_time > 1.5:
+                        if current_chunk_time > timeout:
                             print("Token stream took too long to produce next chunk, re-issuing completion request. Average chunk time:", sum_chunk_times / max(1,n_chunks), "Current chunk time:", current_chunk_time, flush=True)
                             resp.close()
                             raise OpenAIStreamError("Token stream took too long to produce next chunk.")
 
                 received_text = ""
 
                 with concurrent(chunk_timer()):
                     async for chunk in resp.content.iter_any():
                         chunk = chunk.decode("utf-8")
                         current_chunk += chunk
                         is_done = current_chunk.strip().endswith("[DONE]")
                         
                         while "data: " in current_chunk:
-                            chunks = current_chunk.split("data: ")
+                            chunks = current_chunk.split("\ndata: ")
                             while len(chunks[0]) == 0:
                                 chunks = chunks[1:]
                             if len(chunks) == 1:
                                 # last chunk may be incomplete
                                 break
                             complete_chunk = chunks[0].strip()
-                            current_chunk = "data: ".join(chunks[1:])
+                            current_chunk = "\ndata: ".join(chunks[1:])
+
+                            if complete_chunk.startswith("data: "):
+                                complete_chunk = complete_chunk[len("data: "):]
 
                             if len(complete_chunk.strip()) == 0: 
                                 continue
                             if complete_chunk == "[DONE]": 
                                 return
 
                             n_chunks += 1
                             sum_chunk_times += time.time() - last_chunk_time
                             last_chunk_time = time.time()
                             
-                            data = json.loads(complete_chunk)
+                            try:
+                                data = json.loads(complete_chunk)
+                            except json.decoder.JSONDecodeError:
+                                print("Failed to decode JSON:", [complete_chunk])
 
                             if "error" in data.keys():
                                 message = data["error"]["message"]
                                 if "rate limit" in message.lower():
                                     raise OpenAIRateLimitError(message + "local client capacity" + str(Capacity.reserved))
                                 else:
                                     raise OpenAIStreamError(message + " (after receiving " + str(n_chunks) + " chunks. Current chunk time: " + str(time.time() - last_chunk_time) + " Average chunk time: " + str(sum_chunk_times / max(1, n_chunks)) + ")", "Stream duration:", time.time() - stream_start)
@@ -242,26 +304,28 @@
                                                 "token_logprobs": [],
                                                 "tokens": [],
                                                 "top_logprobs": []
                                             }
                                         })
                                     continue
                                 text = delta["content"]
-                                tokens = tokenize((" " if received_text == "" else "") + text)
+                                tokens = tokenize((" " if received_text == "" else "") + text, openai_byte_encoding=True)
                                 received_text += text
-                                # print([text], [received_text])
+
+                                # convert tokens to OpenAI format
+                                tokens = [str(t) for t in tokens]
                                 
                                 choices.append({
                                     "text": text,
                                     "index": c["index"],
                                     "finish_reason": c["finish_reason"],
                                     "logprobs": {
                                         "text_offset": [0 for _ in range(len(tokens))],
                                         "token_logprobs": [0.0 for _ in range(len(tokens))],
-                                        "tokens": [[t] for t in tokens],
+                                        "tokens": tokens,
                                         "top_logprobs": [{t: 0.0} for t in tokens]
                                     }
                                 })
                             data["choices"] = choices
 
                             yield data
                         
@@ -272,88 +336,92 @@
                 if current_chunk.strip() == "[DONE]":
                     return
                 try:
                     last_message = json.loads(current_chunk.strip())
                     message = last_message.get("error", {}).get("message", "")
                     if "rate limit" in message.lower():
                         raise OpenAIRateLimitError(message + "local client capacity" + str(Capacity.reserved))
-                    else:
-                        raise OpenAIStreamError(last_message["error"]["message"] + " (after receiving " + str(n_chunks) + " chunks. Current chunk time: " + str(time.time() - last_chunk_time) + " Average chunk time: " + str(sum_chunk_times / max(1, n_chunks)) + ")", "Stream duration:", time.time() - stream_start)
-                        # raise OpenAIStreamError(last_message["error"]["message"])
+                    else:   
+                        raise OpenAIStreamError(message + " (after receiving " + str(n_chunks) + " chunks. Current chunk time: " + str(time.time() - last_chunk_time) + " Average chunk time: " + str(sum_chunk_times / max(1, n_chunks)) + ")", "Stream duration:", time.time() - stream_start)
                 except json.decoder.JSONDecodeError:
-                    raise OpenAIStreamError("Token stream ended unexpectedly.", current_chunk)
+                    raise OpenAIStreamError("Error in API response:", current_chunk)
     
 async def completion_api(**kwargs):
-    from lmql.runtime.openai_secret import openai_secret, openai_org
     global stream_semaphore
 
     num_prompts = len(kwargs["prompt"])
     max_tokens = kwargs.get("max_tokens", 0)
 
+    timeout = kwargs.pop("timeout", 1.5)
+
     async with CapacitySemaphore(num_prompts * max_tokens):
         
         current_chunk = ""
         stream_start = time.time()
         
         async with aiohttp.ClientSession() as session:
+            endpoint, headers = get_endpoint_and_headers(kwargs)
             async with session.post(
-                "https://api.openai.com/v1/completions",
-                headers={
-                    "Authorization": f"Bearer {openai_secret}",
-                    "Content-Type": "application/json",
-                },
-                json={**kwargs},
+                    endpoint,
+                    headers=headers,
+                    json={**kwargs},
             ) as resp:
                 last_chunk_time = time.time()
                 sum_chunk_times = 0
                 n_chunks = 0
                 current_chunk_time = 0
 
                 async def chunk_timer():
                     nonlocal last_chunk_time, sum_chunk_times, n_chunks, current_chunk_time
                     while True:
                         await asyncio.sleep(0.5)
                         current_chunk_time = time.time() - last_chunk_time
                         # print("Average chunk time:", sum_chunk_times / n_chunks, "Current chunk time:", current_chunk_time)
                         # print("available capacity", Capacity.total - Capacity.reserved, "reserved capacity", Capacity.reserved, "total capacity", Capacity.total, flush=True)
 
-                        if current_chunk_time > 1.5:
+                        if current_chunk_time > timeout:
                             print("Token stream took too long to produce next chunk, re-issuing completion request. Average chunk time:", sum_chunk_times / max(1,n_chunks), "Current chunk time:", current_chunk_time, flush=True)
                             resp.close()
                             raise OpenAIStreamError("Token stream took too long to produce next chunk.")
 
                 with concurrent(chunk_timer()):
                     async for chunk in resp.content.iter_any():
                         chunk = chunk.decode("utf-8")
                         current_chunk += chunk
                         is_done = current_chunk.strip().endswith("[DONE]")
                         
                         while "data: " in current_chunk:
-                            chunks = current_chunk.split("data: ")
+                            chunks = current_chunk.split("\ndata: ")
                             while len(chunks[0]) == 0:
                                 chunks = chunks[1:]
                             if len(chunks) == 1:
                                 # last chunk may be incomplete
                                 break
                             complete_chunk = chunks[0].strip()
-                            current_chunk = "data: ".join(chunks[1:])
+                            current_chunk = "\ndata: ".join(chunks[1:])
+                            
+                            if complete_chunk.startswith("data: "):
+                                complete_chunk = complete_chunk[len("data: "):]
 
                             if len(complete_chunk.strip()) == 0: 
                                 continue
                             if complete_chunk == "[DONE]":
                                 return
                             
                             if n_chunks == 0:
                                 api_stats.times["first-chunk-latency"] = api_stats.times.get("first-chunk-latency", 0) + (time.time() - stream_start)
 
                             n_chunks += 1
                             sum_chunk_times += time.time() - last_chunk_time
                             last_chunk_time = time.time()
                             
-                            data = json.loads(complete_chunk)
+                            try:
+                                data = json.loads(complete_chunk)
+                            except json.decoder.JSONDecodeError:
+                                print("Failed to decode JSON:", [complete_chunk])
 
                             if "error" in data.keys():
                                 message = data["error"]["message"]
                                 if "rate limit" in message.lower():
                                     raise OpenAIRateLimitError(message + "local client capacity" + str(Capacity.reserved))
                                 else:
                                     raise OpenAIStreamError(message + " (after receiving " + str(n_chunks) + " chunks. Current chunk time: " + str(time.time() - last_chunk_time) + " Average chunk time: " + str(sum_chunk_times / max(1, n_chunks)) + ")", "Stream duration:", time.time() - stream_start)
@@ -369,27 +437,58 @@
                 
                 try:
                     last_message = json.loads(current_chunk.strip())
                     message = last_message.get("error", {}).get("message", "")
                     if "rate limit" in message.lower():
                         raise OpenAIRateLimitError(message + "local client capacity" + str(Capacity.reserved))
                     else:
-                        raise OpenAIStreamError(last_message["error"]["message"] + " (after receiving " + str(n_chunks) + " chunks. Current chunk time: " + str(time.time() - last_chunk_time) + " Average chunk time: " + str(sum_chunk_times / max(1, n_chunks)) + ")", "Stream duration:", time.time() - stream_start)
+                        raise OpenAIStreamError((message or str(last_message)) + " (after receiving " + str(n_chunks) + " chunks. Current chunk time: " + str(time.time() - last_chunk_time) + " Average chunk time: " + str(sum_chunk_times / max(1, n_chunks)) + ")", "Stream duration:", time.time() - stream_start)
                         # raise OpenAIStreamError(last_message["error"]["message"])
                 except json.decoder.JSONDecodeError:
-                    raise OpenAIStreamError("Token stream ended unexpectedly.", current_chunk)
+                    raise OpenAIStreamError("Error in API response:", current_chunk)
 
 async def main():
+    import sys
+    # Not sure if this should work, but prompt needs tokenizing I think
+    """
     kwargs = {
         "model": "text-davinci-003",
         "prompt": "Say this is a test",
         "max_tokens": 7,
         "temperature": 0,
         "stream": True
     }
 
     async for chunk in complete(**kwargs):
-        print(chunk)
+                print(chunk)"""
+
+    """
+     Tested working with these environment variables:
+        Azure config for GPT-3.5-Turbo:
+            OPENAI_API_TYPE = azure
+            AZURE_OPENAI_GPT-3_5-TURBO_ENDPOINT = https://{service}.openai.azure.com/openai/deployments/{gpt3.5-turbo-deployment}/chat/completions?api-version=2023-03-15-preview
+            AZURE_OPENAI_GPT-3_5-TURBO_KEY = XXXXXXXXX
+        Regular OpenAI credentials for GPT-3.5-Turbo:
+            OPENAI_API_TYPE = openai
+            OPENAI_API_KEY = XXXXXXXXX
+    """
+
+    kwargs = {
+        "model": "gpt-3.5-turbo",
+        "prompt": [
+            tokenize("<lmql:system/> You are a helpful assistant.<lmql:user/>Hi, tell me all you know about GPT-2.")],
+        "max_tokens": 512,
+        "temperature": 0.,
+        "stream": True,
+        "echo": False,
+        "logprobs": None,
+    }
+
+    async for chunk in chat_api(**kwargs):
+        if len(chunk["choices"]) > 0:
+            sys.stdout.write(chunk["choices"][0]["text"])
+
 
 if __name__ == "__main__":
     import asyncio
-    asyncio.run(main())
+
+    asyncio.run(main())
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/caching.py` & `lmql-0.0.6.4/src/lmql/runtime/caching.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Utility function to manage cached (serialized)
 LMQL runtime components.
 """
 import os
 import pathlib
 
-CACHE_VERSION = 1
+CACHE_VERSION = 3
 CACHE_DIR = pathlib.Path.home() / ".cache" / "lmql"
 
 def prepare_cache_access():
     if not CACHE_DIR.exists():
         CACHE_DIR.mkdir(parents=True, exist_ok=True)
 
         with open(os.path.join(CACHE_DIR, "cache-version"), "w") as f:
@@ -32,14 +32,16 @@
         print("LMQL cache directory ({}) format is outdated, clearing cache (existing: v{}, runtime: v{})...".format(CACHE_DIR, cache_version, CACHE_VERSION))
         for f in os.listdir(CACHE_DIR):
             os.remove(os.path.join(CACHE_DIR, f))
         with open(os.path.join(CACHE_DIR, "cache-version"), "w") as f:
             f.write(str(CACHE_VERSION))
 
 def cache_file_exists(path):
+    if "NO_CACHE" in os.environ.keys():
+        return False
     prepare_cache_access()
     return os.path.exists(path)
 
 class CacheDirFile:
     def __init__(self, path, mode):
         assert not os.path.isabs(path), "CacheDirFile path must be relative"
         self.path = os.path.join(CACHE_DIR, path)
@@ -53,8 +55,10 @@
     
     def __exit__(self, exc_type, exc_value, traceback):
         self.filehandle.close()
         with open(os.path.join(CACHE_DIR, "cache-version"), "w") as f:
             f.write(str(CACHE_VERSION))
 
 def cachefile(path, mode):
+    if not cache_file_exists(path) and "r" in mode:
+        raise FileNotFoundError("Cache file {} does not exist".format(path))
     return CacheDirFile(path, mode)
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,21 @@
         scorer = alpha_length_normalized()
 
     def op_max_score(seqs, score):
         return np.array([score] + [scorer(s.logprobs, s) for s in seqs]).min()
 
     return ar.reduce(op_max_score, np.finfo(np.float32).max)
 
+def array_sorted(ar, key, name=None):
+    def op_sorted(seqs):
+        if len(seqs) == 0: 
+            return None
+        return list(sorted(seqs, key=key))
+    return ar.element_wise(op_sorted, name=name)
+
 def topk(ar, k, scorer: Optional[topk_scorer]=None, name=None):
     if scorer is None:
         scorer = alpha_length_normalized()
     
     def op_topk(seqs):
         if len(seqs) == 0: 
             return None
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_cache.py` & `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,31 +8,29 @@
 
 from .dclib_array import DataArray
 from .dclib_seq import DecoderSequence, Continuation, DeterministicDecoderSequence, deepcopy, deepmerge, detseq
 from .dclib_model import DcModel, CacheDelegate
 from .dclib_rewrite import DcModelRewriteMixin
 import lmql.runtime.masks as masks
 from lmql.utils.nputil import ensure_iterable
+from concurrent.futures import ThreadPoolExecutor
 
 class CacheFile:
     def __init__(self, filename, initial_ids, model):
         self.filename = filename
         self.initial_ids = initial_ids
         self.model = model
     
     def load(self):
         if self.filename is not None and os.path.exists(self.filename):
             with open(self.filename, "rb") as f:
                 cache = pickle.load(f)
                 if cache.get("model") != self.model:
                     print("warning: cache file is from a different model. Its contents will be overwritten. {} != {}".format(cache["model"], self.model))
                 else:
-                    if not str(self.initial_ids) in cache.keys():
-                        print(str(self.initial_ids))
-                        print("cache miss for", self.filename, cache.keys())
                     return cache.get(str(self.initial_ids), {})
         return {}
     
     def save(self, cache):
         if os.path.exists(self.filename):
             with open(self.filename, "rb") as f:
                 existing_cache = pickle.load(f)
@@ -86,33 +84,39 @@
             mc.cache = CacheFile(cache_file, initial_prompt_ids, delegate.model_identifier).load()
         except Exception as e:
             print("error: failed to load token cache from file", e)
             pass
 
         return mc
     
-    def close(self):
-        self.model.cache_delegate = None
-        for ts in self.token_streams:
-            ts.cancel()
-        self.token_streams = []
+    @property
+    def tokenizer(self):
+        return self.delegate.tokenizer
 
-    def save(self):
+    def close(self):
         if self.cache_file is not None:
             cf = CacheFile(self.cache_file, self.initial_ids, self.delegate.model_identifier)
             try:
                 cf.save(self.cache)
             except Exception as e:
                 print("error: failed to save token cache to file", e, flush=True)
                 pass
+
+        self.model.cache_delegate = None
+        for ts in self.token_streams:
+            ts.cancel()
+        self.token_streams = []
+
+        if hasattr(self.delegate, "close"):
+            self.delegate.close()
     
     def base_key(self, ids, *args):
         if isinstance(ids, DecoderSequence):
             return self.base_key(ids.input_ids)
-        return str(ids[self.input_id_key_offset:])
+        return str(ids)
 
     async def get_mask(self, s: DecoderSequence, **kwargs):
         if s.id in self.mask_cache:
             return self.mask_cache[s.id]
         if hasattr(s, "logits_mask"):
             return s.logits_mask
 
@@ -150,17 +154,16 @@
                     if edge_type == "top-1":
                         argmax_token, argmax_score = self.cache.get((self.base_key(s), "top-1"), (None, None))
                         if type(argmax_token) is int and argmax_token in mask:
                             keys.append((self.base_key(s), str(argmax_token)))
                 else:
                     keys.append((self.base_key(s), edge_type, "-".join([str(i) for i in np.where(mask >= 0)[0]])))
         else:
-            if edge_type != "sample":
-                # standard key is sequence id + edge type
-                keys.append((self.base_key(s), edge_type))
+            # standard key is sequence id + edge type
+            keys.append((self.base_key(s), edge_type))
 
         return keys
     
     async def get_cache(self, s: DecoderSequence, edge_type: str, user_data=False, **kwargs):
         keys = await self.get_keys(s, edge_type, **kwargs)
 
         for k in keys:
@@ -245,15 +248,18 @@
         return await arr.aelement_wise(op_argmax)
 
     async def sample(self, arr: DataArray, num_samples=1, **kwargs):
         async def op_sample(seqs):
             self.calls += len(seqs)
 
             # check cache for all
-            cache_entries = [await self.get_cache(s, 'sample', **kwargs) for s in seqs]
+            temperature = kwargs.get('temperature', 1.0)
+            sampling_mode = "top-1" if temperature == 0.0 else "sample-{}".format(temperature)
+            
+            cache_entries = [await self.get_cache(s, sampling_mode, **kwargs) for s in seqs]
             cached_tokens = [e[1] for e in cache_entries]
             cache_keys = [e[0] for e in cache_entries]
             
             # apply operation for non-cached
             non_cached = [s for s, c in zip(seqs, cached_tokens) if c is None]
             # generator over new results
             non_cached_sample = iter((await self.delegate.sample(DataArray(non_cached), num_samples=num_samples, **kwargs)).items())
@@ -371,58 +377,25 @@
             sq = sq.extend(c, internal=True)
             tok = tok[1:]
             if len(tok) == 0:
                 break
 
         if len(tok) == 0: return
         # do actual scoring with delegate model
+        self.calls += 1
         sq, tokens, scores = await anext(self.delegate.score_tokens([sq], [tok], noscore=noscore))
         self.save_cached(sq.input_ids, tokens, scores, user_data)
         
-    def save_cached(self, ids: List[int], tokens, scores, user_data):
+    def save_cached(self, ids: List[bytes], tokens, scores, user_data):
         # add cache entries along pre-scored trajectory
         for tok, score in zip(tokens, scores):
             value = (np.array(tok).reshape(1), np.array(score).reshape(1))
-            self.set_cache([(self.base_key(ids, user_data), str(int(tok)))], value)
+            self.set_cache([(self.base_key(ids, user_data), tok)], value)
             ids = np.append(ids, tok)
 
-    # async def prescore(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, 
-    #                 deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, 
-    #                 user_data=None, noscore=False):
-    #     async def op_score(sq, tok, max_batch_size, det, stop_phrase, needs_rewrite, user_data, noscore):
-    #         assert len(user_data) == len(tok)
-    #         sq, tok, det, user_data = self.expand_through_cache(sq, tok, det, user_data)
-
-    #         # handle short and fully cached sequences
-    #         if len(tok) == 0:
-    #             return [sq]
-    #         elif len(tok) <= 1 and not noscore:
-    #             return
-
-    #         # do actual scoring with delegate model
-    #         result = await self.delegate.score([sq], [tok], max_batch_size, det, stop_phrase, needs_rewrite, None, noscore, internal=True)
-
-    #         # add initial cache entry
-    #         s = result[0]
-    #         s.user_data = user_data[0]
-    #         c = Continuation(np.array([s.input_ids[-1]]), np.array([s.logprobs[-1]]), [user_data[0]])
-    #         self.set_cache([(self.base_key(sq), str(int(s.input_ids[-1])))], c)
-    #         user_data_offset = 1
-            
-    #         # add additional cache entries for deterministic tokens
-    #         while type(s) is DeterministicDecoderSequence and len(s.next_ids) > 0:
-    #             c = Continuation(np.array([s.next_ids[0]]), np.array([s.next_logprobs[0]]), [user_data[user_data_offset]])
-    #             sq = s
-    #             s = sq.extend(c)
-    #             user_data_offset += 1
-    #             self.set_cache([(self.base_key(sq), str(s.input_ids[-1]))], c)
-        
-    #     assert len(sqs) == len(tokens)
-    #     return await asyncio.gather(*[op_score(sq, tok, max_batch_size, det, stop_phrase, needs_rewrite, ud, noscore) for sq, tok, det, ud in zip(sqs, tokens, deterministic, user_data)])
-    
     @property
     def model_args(self):
         return self.delegate.model_args
 
     @property
     def bos_token_id(self):
         return self.delegate.bos_token_id
@@ -461,14 +434,15 @@
             # create continuation sequence at cache boundary
             continued_seq, tok, det, _ = self.expand_through_cache(sq, tok, deterministic, [user_data for _ in tok])
 
             if len(tok) == 0:
                 completion = np.array(unexpanded_tok)
                 token_scores = continued_seq.logprobs[-len(completion):]
             else:
+                self.calls += 1
                 # run actual score() call for remaining non-cached part of 'tokens' (tok)
                 result: DeterministicDecoderSequence = (await self.delegate.score([continued_seq], [tok], max_batch_size, det, stop_phrase, needs_rewrite=needs_rewrite, user_data=user_data, noscore=noscore, internal=True))[0]
                 
                 # extract scores and tokens for new, scored part of 'tokens'
                 token_scores = np.array(result.logprobs[len(sq.input_ids):].tolist() + result.next_logprobs.tolist())
                 completion = np.array(unexpanded_tok)
                 assert len(token_scores) == len(completion), f"Expected {len(completion)} scores, but got {len(token_scores)}"
@@ -510,60 +484,63 @@
             try:
                 ids = None
                 keys = None
                 sq = None
                 waiting_token_keys = []
 
                 async for (s, tokens, scores, edge_types, user_data) in itr():
-                    if type(tokens) is int or len(tokens) == 1:
-                        tokens = ensure_iterable(tokens)
-                        scores = ensure_iterable(scores)
-                        if type(edge_types) is str or edge_types is None:
-                            edge_types = [edge_types]
-                    else:
-                        assert len(tokens) == len(scores) == len(edge_types), f"token_consumer: expected all lists to have the same length, but got {len(tokens)}, {len(scores)}, {len(edge_type)}"
-                        # print("setting entries for", edge_types)
-                    
-                    waiting_token_keys = []
-                    
                     async with self.cache_lock:
-                        for token, score, edge_type in zip(tokens, scores, edge_types):
+                        if type(tokens) is int or len(tokens) == 1:
+                            tokens = ensure_iterable(tokens)
+                            scores = ensure_iterable(scores)
+                            if type(edge_types) is str or edge_types is None:
+                                edge_types = [edge_types]
+                        else:
+                            assert len(tokens) == len(scores) == len(edge_types), f"token_consumer: expected all lists to have the same length, but got {len(tokens)}, {len(scores)}, {len(edge_type)}"
+                            # print("setting entries for", edge_types)
+                        
+                        waiting_token_keys = []
+                        
+                        for token, score, edge_type in reversed(list(zip(tokens, scores, edge_types))):
                             assert type(edge_type) is str or edge_type is None, "edge_types is {}".format(edge_types)
-                            
+
                             if ids is None:
                                 ids = s.input_ids
                                 keys = await self.get_keys(s, edge_type, **self.model_args)
                                 sq = s
+                            
                             token_keys = [(self.base_key(ids), edge_type, *k[2:]) for k in keys]
                             token_keys += [(self.base_key(ids), str(token))]
                             # filter out keys with edge_type=None
                             token_keys = [k for k in token_keys if k[1] is not None]
 
                             # for tk in token_keys:
                             #     if tk in self.cache and type(self.cache[tk][0]) is not asyncio.Future:
                             #         print("token_consumer: token for {} from stream already in cache ({} streams): {}".format(tk, len(self.token_streams), self.cache[tk]))
 
-                            self.set_cache(token_keys, (np.array(token).reshape(1), np.array(score).reshape(1)), user_data=user_data)
+                            self.set_cache(token_keys, (np.array(token).reshape(1), np.array(score).reshape(1)), user_data=user_data, verbose=False)
 
                             if self.show_speculative:
                                 c = Continuation(np.array(token), np.array(score), None)
-                                sq = sq.extend(c)
+                                cs = sq.extend(c)
+                                if edge_type == "top-1":
+                                    sq = cs
+
+                            if edge_type is not None and (edge_type == "top-1" or "top" not in edge_type):
+                                # set future for next token (so get_cache can wait for it if needed)
+                                fut_keys = [(self.base_key(np.append(ids, token)), edge_type, *k[2:]) for k in keys]
+                                waiting_token_keys.append(fut_keys)
+                                # set future for next token (if k is not already set)
+                                fut = asyncio.Future()
+                                unset_keys = [k for k in fut_keys if k not in self.cache]
+                                self.set_cache(unset_keys, (fut, fut))
+                        
+                        # extend ids
+                        ids = np.append(ids, tokens[0])
 
-                            # set future for next token (so get_cache can wait for it if needed)
-                            fut_keys = [(self.base_key(ids), edge_type, *k[2:]) for k in keys]
-                            waiting_token_keys.append(fut_keys)
-                            # set future for next token (if k is not already set)
-                            fut = asyncio.Future()
-                            unset_keys = [k for k in fut_keys if k not in self.cache]
-                            self.set_cache(unset_keys, (fut, fut))
-
-                    # extend ids
-                    ids = np.append(ids, tokens[0])
-                        # print(waiting_token_keys)
-                
                 # remove last waiting token entry (since it will not be provided by this stream)
                 for future_keys in waiting_token_keys:
                     for k in future_keys:
                         fut = self.cache.get(k, (None, None))[0]
                         if type(fut) is asyncio.Future:
                             # resolve future as invalid (handled in get_cache)
                             fut.set_result(None)
@@ -571,15 +548,17 @@
             except Exception as e:
                 print("DcCachedModel: token_consumer failed with:", e)
                 import traceback
                 traceback.print_exc()
                 raise e
 
         self.token_streams = [s for s in self.token_streams if not s.done()]
-        self.token_streams.append(asyncio.create_task(token_consumer(token_iterator)))
+
+        task = token_consumer(token_iterator)
+        self.token_streams.append(asyncio.ensure_future(task))
         
     async def wait_for_active_streams(self):
         """
         Waits until all active cache streams have been processed.
         """
         caches = self.token_streams
         # remove all done cache streams
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_global.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,13 +4,16 @@
 DcGlobal.tokenizer = None
 
 stats = Stats("dclib")
 
 def get_tokenizer():
     return DcGlobal.tokenizer
 
+def clear_tokenizer():
+    DcGlobal.tokenizer = None
+
 def set_dclib_tokenizer(tokenizer):
     assert DcGlobal.tokenizer is None or DcGlobal.tokenizer.name == tokenizer.name, f"Cannot set dclib tokenizer to {tokenizer.name} because it is already set to {DcGlobal.tokenizer.name} (cannot use multiple tokenizers in the same process for now)"
     DcGlobal.tokenizer = tokenizer
     
 def get_tokenizer():
     return DcGlobal.tokenizer
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_rewrite.py` & `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_rewrite.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,17 +193,38 @@
 
     @property
     def num_tokens(self):
         return len(self.input_ids) - self.prompt_len
 
     async def detokenized(self, name):
         async def seqtext_provider():
-            return str([await get_tokenizer().decode(self.input_ids[1:])][0])
+            t = str([get_tokenizer().decode(self.input_ids)][0])
+            t = str(t.encode("utf-8"))[2:-1]
+            return t
         async def text_provider():
-            return str([await get_tokenizer().decode(self.input_ids[-1:])])[2:-2]
+            t = str([get_tokenizer().decode(self.input_ids[-1:])])[2:-2]
+            INVALID_CHARACTER = "\uFFFD"
+            if INVALID_CHARACTER in t:
+                # use token id
+                if type(self.input_ids[-1]) is int:
+                    t = "token:" + str(self.input_ids[-1])
+                elif type(self.input_ids[-1]) is bytes or type(self.input_ids[-1]) is np.bytes_:
+                    # best effort solution to decode multibyte characters in the UI
+                    for i in range(4):
+                        if not INVALID_CHARACTER in get_tokenizer().decode([self.input_ids[-i-1]]):
+                            break
+                        t = get_tokenizer().decode(self.input_ids[-i-1:])
+                        if INVALID_CHARACTER not in t:
+                            return t
+                    t = ""
+                    # t = str(byte_value)[2:-1]
+                else:
+                    t = str(self.input_ids[-1])
+                    t = str(t.encode("utf-8"))[2:-1]
+            return t
         providers = {
             "seqtext": seqtext_provider,
             "text": text_provider
         }
         
         if not hasattr(self, "tokenizer_cache"):
             self.tokenizer_cache = {}
@@ -327,15 +348,15 @@
         new_stop_phrase = np.concatenate([old_stop_phrase, np.array([False])])
         
         stop_phrases = self.data("head").stopping_phrases["tokenized"] if self.data("head") is not None else []
 
         if stop_phrases is None:
             return new_stop_phrase
 
-        ids = np.concatenate([self.input_ids, continuation.token.reshape(1)]),
+        ids = np.concatenate([self.input_ids, continuation.token.reshape(1)])
         for stop in stop_phrases:
             len_stop = len(stop)
             if ids[-len_stop:] == stop:
                 new_stop_phrase[-len_stop:] = True
                 break
 
         return new_stop_phrase
@@ -346,41 +367,50 @@
     def __repr__(self) -> str:
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
         return f"<seq token_len={len(self.input_ids)} ids=[... {ids}]>"
 
     async def text(self, offset:int=None, limit:int=None, pretty=True) -> str:
         offset = offset or 0
         limit = limit or len(self.input_ids)
-        raw_text = await get_tokenizer().decode(self.input_ids[offset:limit])
+        raw_text = get_tokenizer().decode(self.input_ids[offset:limit])
         if not pretty: 
             return raw_text
         else:
             return str([raw_text])[2:-2]
 
     async def str(self, full=False) -> str:
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
         if detokenize_seqs:
-            s = await get_tokenizer().decode(self.input_ids)
+            s = get_tokenizer().decode(self.input_ids)
             if not full:
                 s = "..." + s[-40:]
             return f"<seq token_len={len(self.input_ids)} s={str([s])[1:-1]} ids=[... {ids}]>"
         else:
             return f"<seq token_len={len(self.input_ids)} ids=[... {ids}]>"
 
     def __str__(self):
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
         return f"<seq token_len={len(self.input_ids)} ids=[... {ids}]>"
 
     def is_done(self):
-        return self.input_ids[-1] == get_tokenizer().eos_token_id
+        return self.input_ids[-1] == get_tokenizer().eos_token_id or self.input_ids[-1] == str(get_tokenizer().eos_token_id).encode() or self.input_ids[-1] == b"<|endoftext|>"
 
     def make_successors(self, next_tokens, next_token_scores, logits, user_data=None):
         # remove very low scoring tokens (likely they were masked and therefore score low)
-        next_tokens = np.stack([t for t, s in zip(next_tokens, next_token_scores) if s > DecoderSequence.truncation_threshold], axis=0)
-        next_token_scores = np.stack([s for s in next_token_scores if s > DecoderSequence.truncation_threshold], axis=0)
+        next_tokens = nputil.ensure_iterable(next_tokens)
+        next_token_scores = nputil.ensure_iterable(next_token_scores)
+        
+        tokens = [t for t, s in zip(next_tokens, next_token_scores) if s > DecoderSequence.truncation_threshold]
+        scores = [s for s in next_token_scores if s > DecoderSequence.truncation_threshold]
+        if len(tokens) == 0:
+            print("WARNING: all continuation token fall below truncation threshold. This is likely due to a too small truncation factor. Try increasing it. Continuing with the top 1 token.")
+            tokens = [t for t, s in zip(next_tokens, next_token_scores)][:1]
+            scores = [s for s in next_token_scores][:1]
+        next_tokens = np.stack(tokens, axis=0)
+        next_token_scores = np.stack(scores, axis=0)
 
         return Continuation(next_tokens, next_token_scores, user_data)
 # global counter for all sequences created in this process for identification purposes
 DecoderSequence.seq_ctr = 0
 
 DecoderSequence.graph = None
 # tokens with a logprob lower than this will be ignored and not expanded during decoding
@@ -438,15 +468,15 @@
         self.next_ids = next_ids
         self.next_logprobs = next_logprobs
         self.next_deterministic = next_deterministic
 
         self.needs_rewrite = needs_rewrite
         self.internal = internal
 
-        if next_logprobs is not None: assert len(next_logprobs) == len(next_ids), "Length of deterministic continuation did not match length of provided logprobs"
+        if next_logprobs is not None: assert len(next_logprobs) == len(next_ids), "Length of deterministic continuation did not match length of provided logprobs. Provided logprobs: {}, Provided IDs: {}".format(len(next_logprobs), next_ids)
         if next_deterministic is not None: assert len(next_deterministic) == len(next_ids), "Length of determinism status did not match length of provided logrprobs"
 
         self.align_user_data()
 
     # async def text(self, offset: int = None, limit: int = None, pretty=True) -> str:
     #     return "<detseq> " + await super().text(offset, limit, pretty)
 
@@ -575,15 +605,15 @@
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
         if (len(self.next_ids) > 0): 
             ids = "... " + ids
         next_ids = ", ".join([str(i) for i in self.next_ids[:10]])
         if len(self.next_ids) > 10: 
             next_ids = "..." + next_ids
         if detokenize_seqs:
-            s = await get_tokenizer().decode(self.input_ids)
+            s = get_tokenizer().decode(self.input_ids)
             if not full:
                 s = "..." + s[-40:]
             return f"<detseq token_len={len(self.input_ids)} s={str([s])[1:-1]} ids=[{ids}] next_ids=[{next_ids}]>"
         else:
             return f"<detseq token_len={len(self.input_ids)} ids=[{ids}] next_ids=[{next_ids}]>"
 
     def make_successors(self, next_tokens, next_token_scores, logits, user_data=None):
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.6.4/src/lmql/runtime/dclib/decoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     dc.finish(done)
 
 @dc.decoder
 async def beam_sample(prompt_ids: np.ndarray, n=4, max_len=None, temperature=None, **kwargs):
     n = kwargs.get("num_beams", n)
     max_len = max_len or 2048
     model = dc.model(**kwargs)
+    temperature = temperature or 1.0
 
     # keep track of active beams and finished sequences
     h = dc.seqs([dc.seq(prompt_ids)] * 1)
     done = dc.seqs()
 
     # stopping criteria for the beam search
     not_done = dc.logical_and(dc.logical_not(dc.eos), dc.lt(max_len))
@@ -172,15 +173,15 @@
     dc.finish(done)
 
     yield (h, done)
 
 dc.decoder(beam_search, "beam")
 
 @dc.decoder
-async def beam_var(prompt_ids: np.ndarray, n=4, max_len=None, inject_stop=False, prune=None, **kwargs):
+async def beam_var(prompt_ids: np.ndarray, n=4, max_len=None, inject_stop=False, prune=None, return_first=False, **kwargs):
     s = Stats("beam_var")
 
     n = kwargs.get("num_beams", n)
     max_len = max_len or 2048
     model = dc.model(**kwargs)
     alpha = kwargs.get("alpha", 0.7)
     scorer = alpha_length_normalized_det(alpha=alpha)
@@ -250,19 +251,24 @@
             if len(nondet_h) > 0:
                 nondet_h = post_vilar_allocation(nondet_h, n, scorer=scorer, num_steps=num_steps)
             h = det_h + nondet_h
             # h = post_vilar_allocation(h, n, scorer=scorer, num_steps=num_steps)
 
             done = dc.topk(done, n, scorer=scorer, name="done_" + str(num_steps))
 
+        if len(done) > 0 and return_first:
+            break
+
         yield (h, done)
     
     done.name("final result")
     yield done
-    dc.finish(done)
+
+    # sort done by score
+    dc.finish(dc.array_sorted(done.flatten(), key=lambda s: -s.logprobs.sum()))
 
 
 def post_vilar_allocation(h, k, scorer=None, num_steps=0):
     """
     Restricts h to a set of candidate sequences according to the criteria in Post 
     and Vilar (Fast Lexically Constrained Decoding with Dynamic Beam Allocation for Neural Machine Translation)
 
@@ -409,14 +415,15 @@
     seqs: sequences to extend
     active_variable: active variable that should be decoded
     b: number of continuation candidates to generate per sequence
     """
     active = seqs.reshape(lambda s: s.id)
     variable_done = dc.seqs()
     active_variable.set(None)
+    sample = method == "sample"
 
     def is_active_variable(s):
         v = s.data("head.variable")
         if v is None: return False
         if active_variable.get() is None: 
             active_variable.set(v)
             return True
@@ -462,15 +469,15 @@
                 s.data("eos_score", regular_scorer(s.logprobs))
 
             active = await model.rewrite(active)
 
             active, variable_done = (active + variable_done).separate_by(is_active_variable)
             active = dc.topk(active, b)
 
-            top_variable_done, _ = dc.seperate_topk(variable_done, b, scorer=nw_score)
+            top_variable_done, _ = dc.seperate_topk(variable_done, b, scorer=regular_scorer)
 
             active.name(str(active_variable.get()) + "[" + str(i) + "]_")
             i += 1
             
             yield active
     elif method == "sample":
         active = active.element_wise(lambda s: s.copy() * b)
@@ -495,15 +502,15 @@
 @dc.decoder
 async def bsseq(prompt_ids: np.ndarray, b=2, max_len=384, **kwargs):
     kwargs.pop("n", None)
     async for s in var(prompt_ids, b=b, n=1, max_len=max_len, subdecoder="beam_seq", **kwargs):
         yield s
 
 @dc.decoder
-async def var(prompt_ids: np.ndarray, b=2, n=None, max_len=384, subdecoder="sample", temperature=1.0, **kwargs):
+async def var(prompt_ids: np.ndarray, b=2, n=None, max_len=384, subdecoder="sample", temperature=1.0, return_first=False, **kwargs):
     """
     sample: 
         if True, uses beam_sample variable-local-decoding, otherwise uses beam_search-like decoding
     var_temperature: 
         sampling temperature to use to obtain multiple variable values
     """
     model = dc.model(**kwargs)
@@ -549,18 +556,20 @@
         
         if len(variable_done) == 0: break
 
         variable_done = dc.topk(variable_done, n)
         variable_done.name("candidates_" + active_variable.get())
 
         yield variable_done
+
+        if len(done) > 0 and return_first: break
         # variable_done = non_det
 
     done = dc.topk(done, len(done))
     done.name("final result")
     yield done
     
-    dc.finish(done)
+    dc.finish(dc.array_sorted(done.flatten(), key=lambda s: -s.logprobs.sum()))
 
 def is_seq_beams_search_done(active_hypotheses, done_hypotheses, num_beams, scorer=None):
     return len(active_hypotheses) == 0 or (len(done_hypotheses) == num_beams and dc.max_score(active_hypotheses, scorer=scorer) < dc.min_score(done_hypotheses, scorer=scorer))
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/interpreter.py` & `lmql-0.0.6.4/src/lmql/runtime/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 import numpy as np
 from lmql.runtime.multi_head_interpretation import InterpretationHead, InterpreterCall, InterpretationHeadDone
 from lmql.runtime.program_state import ProgramState
 import lmql.runtime.dclib as dc
 from lmql.runtime.stats import Stats
 from lmql.runtime.tokenizer import LMQLTokenizer
 from lmql.runtime.interrupt import interrupt
-from lmql.language.qstrings import qstring_to_stmts, TemplateVariable, DistributionVariable
+from lmql.language.qstrings import qstring_to_stmts, TemplateVariable, DistributionVariable, unescape_qstring
 from lmql.utils.nputil import replace_inf_nan_with_str
 
 from lmql.ops.token_set import VocabularyMatcher, has_tail
 from lmql.runtime.model_registry import LMQLModelRegistry
+from lmql.models.model import LMQLModel
 
 from lmql.ops.token_set import tset
 import lmql.ops.ops as ops
 
 class _DCLibDebugPrinter: pass
 _DCLibDebugPrinter.printer = None
 
@@ -77,14 +78,22 @@
         self.program_state.runtime = interpreter
 
     async def json(self):
         return self.program_state
 
     # LMQL runtime API
 
+    @property
+    def num_calls(self):
+        dcmodel = self.interpreter.dcmodel
+        if hasattr(dcmodel, 'calls'):
+            return dcmodel.calls - dcmodel.hits
+        else:
+            return 0
+
     async def get_var(self, name):
         return self.program_state.get_program_value(name)
 
     async def query(self, qstring):
         return InterpreterCall(qstring, loc=None)
 
     async def set_model(self, model_name):
@@ -176,20 +185,46 @@
             self.output_writer = kwargs["output_writer"]
         self.extra_kwargs.update(kwargs)
 
     def set_decoder(self, method, **kwargs):
         self.decoder_kwargs = kwargs
         self.decoder_kwargs["decoder"] = method
 
+        if "backend" in kwargs:
+            LMQLModelRegistry.backend_configuration = kwargs["backend"]
+
     def set_model(self, model_name):
+        model_args = {}
+
+        if type(model_name) is not str:
+            assert isinstance(model_name, LMQLModel), "Not a supported LMQL model '{}' of type '{}'".format(model_name, type(model_name))
+            model_object = model_name
+
+            if model_name.model is not None:
+                model_object = model_name.model
+                # if model_object is a type reference, we can use the model_identifier
+                if callable(model_object):
+                    model_object = model_object()
+
+                self.model_identifier = model_object.model_identifier
+                self.model = model_object
+
+                # setup the VocabularyMatcher to use the concrete vocabulary of the model
+                VocabularyMatcher.init(self.model.get_tokenizer())
+
+                return
+            else:
+                model_name = model_object.model_identifier
+                model_args = model_object.kwargs
+
         if self.model is None:
             self.model = model_name
             self.model_identifier = model_name
 
-        client = LMQLModelRegistry.get(self.model)
+        client = LMQLModelRegistry.get(self.model, **model_args)
 
         # setup the VocabularyMatcher to use the concrete vocabulary of the model
         VocabularyMatcher.init(client.get_tokenizer())
         
         # for OpenAI models we optimize for compact logit masks
         if self.model.startswith("openai/"):
             self.prefers_compact_mask = True
@@ -231,15 +266,15 @@
             while variable is None and query_head.result is None:
                 if len(stmt_buffer) == 0 and variable is None:
                     await continue_for_more_prompt_stmts()
 
                 s = stmt_buffer[0]
 
                 if type(s) is str:
-                    prompt += s
+                    prompt += unescape_qstring(s)
                     stmt_buffer = stmt_buffer[1:]
                     # keep latest prompt in transient state
                     state = state.updated(prompt=prompt)
                 elif type(s) is TemplateVariable:
                     variable = s.name
                     # keep track of number of times a variable with this name has been decoded
                     if variable not in state.recurring_variable_counter.keys():
@@ -288,15 +323,15 @@
 
     async def where_for_sequence(self, s: dc.DecoderSequence, needs_masking, seqidx, **kwargs):
         mask, logit_mask, state = await self.where_step_for_sequence(s, needs_masking, seqidx, **kwargs)
 
         # check for tail and prescore
         if hasattr(self.dcmodel, "prescore_tokens"):
             if has_tail(mask):
-                tail_tokenized = self.tokenizer(mask.tail)["input_ids"]
+                tail_tokenized = self.tokenizer.tokenize(mask.tail, asbytes=True)
                 await self.dcmodel.prescore_tokens(s, tail_tokenized, noscore=kwargs.get("noscore", False))
         
         return logit_mask, state
 
         # eager follow map expansion (w/o) model prediction in between
 
         # # if we cannot predict the next token deterministically
@@ -395,15 +430,15 @@
             # print(id(self), self.variable, [text], "mask", follow_map)
             mask = ops.create_mask(follow_map, valid, is_final)
 
             if mask == "*": 
                 logit_mask = None
             else:
                 logit_mask = mask.mask
-            
+
             # check stopping conditions
             stopping_conditions: List[ops.StopAtOp] = ops.execute_op_stops_at_only(state.variable, self.where, trace)
             for sc in stopping_conditions:
                 stop_trace = trace.copy()
                 del stop_trace[sc]
                 # check if stopping phrase applies in this step
                 if ops.execute_op(sc, stop_trace, context=program_state, semantics="stop"):
@@ -488,15 +523,14 @@
         if seq.is_done() and state.variable is not None:
             program_state = state.program_state.copy()
             variable = state.variable
             
             text = (await seq.text(offset=state.variable_offset, limit=-1, pretty=False))
             text_diff = text[len(await seq.text(state.variable_offset, limit=-2, pretty=False)):]
             
-            assert seq.input_ids[-1] == self.tokenizer.eos_token_id, "last token must be eos token"
             variable_value = text
             # set raw variable value
             program_state.set(variable, variable_value, scores=(), diff=text_diff, montonicity="fin")
             
             # apply postprocessing, if constraints specify it
             # - variable_value is the postprocessed, converted value (does not have to be a string)
             # - postprocessed_prompt is the string in the prompt that corresponds to the variable value
@@ -545,14 +579,31 @@
                 value_offset = state.variable_offset + len(value_ids)
                 
                 combined_new_ids = seq.input_ids[:-n_tokens_to_strip].tolist() + appended_ids
                 variable_offset = len(combined_new_ids)
 
                 rewritten_state = state.updated(variable_offset=variable_offset, variable="__done__" if state.variable is None else state.variable + ":before")
 
+
+                if type(combined_new_ids[0]) is bytes:
+                    res = []
+                    i = 0
+                    while i < len(combined_new_ids):
+                        if type(combined_new_ids[i]) is bytes:
+                            res += [combined_new_ids[i]]
+                            i += 1
+                        else:
+                            j = i+1
+                            while j < len(combined_new_ids) and type(combined_new_ids[j]) is not bytes:
+                                j += 1
+                            r = self.tokenizer.decode_bytes(combined_new_ids[i:j])
+                            res += r
+                            i = j
+                    combined_new_ids = np.array(res, dtype=np.bytes_)
+
                 # appended input ids are now a full replacement for input ids
                 return RewrittenInputIds(
                     appended_input_ids=combined_new_ids, 
                     strip_eos=-n_tokens_to_strip,
                     value_offset=value_offset,
                     user_data=self.interpreter_state_user_data(state),
                     rewritten_seq_user_data=self.interpreter_state_user_data(rewritten_state)
@@ -591,24 +642,24 @@
     async def input(self, *args):
         """Uses the output_writer input() implementation if available."""
         if hasattr(self.output_writer, "input"):
             return await self.output_writer.input(*args)
         else:
             return input(*args)
 
-    async def run(self, fct, **kwargs):
+    async def run(self, fct, *args, **kwargs):
         self.fct = fct
 
         # intercept symbol table entry for input
         if "input" in kwargs.keys() and kwargs["input"] == input:
             kwargs["input"] = self.input
 
         # prepare initial program state
         context = LMQLContext(self, None)
-        query_head = InterpretationHead(fct, context, None, kwargs)
+        query_head = InterpretationHead(fct, context, args, kwargs)
         self.root_state = PromptState(variable=None, prompt="", stmt_buffer=[],
             query_head=query_head, program_state=context.program_state,
             recurring_variable_counter={}, variable_offset=0,
             valid=None, final=None, mask=None, 
             stopping_phrases=None, where=None)
         self.root_state = await self.advance(self.root_state)
 
@@ -634,15 +685,17 @@
         if return_prompt_string:
             return self.root_state.prompt
 
         # tokenize initial prompt
         prompt_ids = await self.tokenize(self.root_state.prompt)
         if self.dcmodel.bos_token_id is not None:
             prompt_ids = [self.dcmodel.bos_token_id] + prompt_ids
-        n = len(prompt_ids)
+        
+        prompt = self.tokenizer.tokenize(self.root_state.prompt, asbytes=True)
+        n = len(prompt)
         
         # make sure that the initial prompt is not considered part of a variable
         self.root_state = self.root_state.updated(variable_offset=n)
 
         decoder_args = decoder_args.copy()
 
         # pass processor as decoder argument
@@ -713,15 +766,15 @@
 
         try:
             import time
 
             self.decoder_step = 0
             average_step_time = None
             start = time.time()
-            async for _ in decoder_fct(prompt_ids, **decoder_args):
+            async for _ in decoder_fct(prompt, **decoder_args):
                 await debug_out(self.decoder_step)
                 self.decoder_step += 1
 
                 if step_budget is not None and self.decoder_step >= step_budget:
                     print("warning: step budget exceeded")
                     break
 
@@ -770,22 +823,19 @@
                     assert state.query_head.result is not None, "decoder designates sequence {} as finished but the underyling query program has not produced a result. This is likekly a decoder bug. Decoder in use {}".format(await s.str(), decoder_args["decoder"])
                     results.append(state.query_head.result)
             
             # set decoder step +1, for all stats logging that happens in postprocessing
             self.decoder_step += 1
 
             return results
-        finally:
-            # make sure token cache is saved if possible
-            self.dcmodel.save()
-            if hasattr(self.dcmodel, "close"):
-                self.dcmodel.close()
 
     def validate_args(self, decoder_args, decoder_fct):
-        INTERNAL_ARGS = ["decoder", "dcmodel", "modern_rewriter", "modern_logits_processor", "dclib_additional_logits_processor", "input_id_rewriter", "output_writer", "chatty_openai", "distribution_batch_size", "openai_chunksize", "step_budget", "stats", "performance_stats", "cache", "show_speculative", "openai_nonstop"]
+        INTERNAL_ARGS = ["decoder", "dcmodel", "modern_rewriter", "modern_logits_processor", "dclib_additional_logits_processor", "input_id_rewriter", "output_writer", 
+                         "chunk_timeout", "chatty_openai", "distribution_batch_size", "openai_chunksize", "step_budget", "stats", "performance_stats", "cache", 
+                         "show_speculative", "openai_nonstop", "chunksize"]
 
         # get all arg names and kwarg names of decoder function
         decoder_arg_names = inspect.getfullargspec(decoder_fct).args
         decoder_kwarg_names = inspect.getfullargspec(decoder_fct).kwonlyargs
         for k in decoder_args.keys():
             if k not in decoder_arg_names and k not in decoder_kwarg_names and k not in INTERNAL_ARGS:
                 raise ValueError("Unknown decoder argument: {}".format(k))
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.6.4/src/lmql/tests/expr_test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,192 +1,189 @@
-"""
-Runtime support used by compiled LMQL query code.
-"""
-
+import sys
+import ast
+import asyncio
+import types
+import astunparse
 import inspect
-from dataclasses import dataclass
-from typing import Any, Dict, Optional
-
-from lmql.ops.ops import *
-from lmql.runtime.langchain import LMQLChainMixIn
-from lmql.runtime.model_registry import LMQLModelRegistry
-from lmql.runtime.output_writer import silent
-from lmql.runtime.interpreter import PromptInterpreter
-from lmql.runtime.postprocessing.conditional_prob import \
-    ConditionalDistributionPostprocessor
-from lmql.runtime.postprocessing.group_by import GroupByPostprocessor
-
-
-def register_model(identifier, ModelClass):
-    LMQLModelRegistry.registry[identifier] = ModelClass
-
-class LMQLInputVariableScope:
-    def __init__(self, f, calling_frame):
-        self.fct = f
-        
-        self.builtins = __builtins__
-        self.globals =  calling_frame.frame.f_globals
-        self.locals = calling_frame.frame.f_locals
-    
-    def resolve(self, name):
-        if name in self.locals.keys():
-            return self.locals[name]
-        elif name in self.globals.keys():
-            return self.globals[name]
-        elif name in self.builtins.keys():
-            return self.builtins[name]
-        else:
-            return None
-            # assert False, "Failed to resolve variable '" + name + "' in @lmql.query " + str(self.fct)
-
-@dataclass
-class FunctionContext:
-    argnames: List[str]
-    args_of_query: List[str]
-    scope: LMQLInputVariableScope
-
-
-class LMQLQueryFunction(LMQLChainMixIn):
-    fct: Any
-    output_variables: List[str]
-    postprocessors: List[Any]
-    scope: Any
-
-    output_writer: Optional[Any] = None
-    args: Optional[List[str]] = None
-    model: Optional[Any] = None
-    function_context: Optional[FunctionContext] = None
-
-    is_langchain_use: bool = False
-
-    lmql_code: str = None
-    
-    def __init__(self, fct, output_variables, postprocessors, scope, *args, **kwargs):
-        # check for pydantic base class and do kw initialization then
-        if hasattr(self, "schema_json"):
-            super().__init__(fct=fct, output_variables=output_variables, postprocessors=postprocessors, scope=scope, *args, **kwargs)
-        else:
-            # otherwise, do standard initialization
-            self.fct = fct
-            self.output_variables = output_variables
-            self.postprocessors = postprocessors
-            self.scope = scope
-        
-        self.output_writer = None
-        self.args = [a for a in inspect.getfullargspec(fct).args if a != "context"]
-        self.model = None
-        # only set if the query is defined inline of a Python file
-        self.function_context = None
-
-    @property
-    def input_keys(self) -> List[str]:
-        self.is_langchain_use = True
-        return self.args
-    
-    def __getattribute__(self, __name: str) -> Any:
-        return super().__getattribute__(__name)
-
-    @property
-    def output_keys(self) -> List[str]:
-        return self.output_variables
-
-    def force_model(self, model):
-        self.model = model
-
-    def make_kwargs(self, *args, **kwargs):
-        if self.function_context is None:
-            return kwargs
-        else:
-            argnames = self.function_context.argnames
-            args_of_query = self.function_context.args_of_query
-            scope = self.function_context.scope
-
-        # do not consider kwargs that are already set
-        argnames = [a for a in argnames if a not in kwargs.keys()]
-
-        assert len(args) == len(argnames), f"@lmql.query {self.fct.__name__} expects {len(argnames)} positional arguments, but got {len(args)}."
-        captured_variables = set(args_of_query)
-        for name, value in zip(argnames, args):
-            if name in args_of_query:
-                kwargs[name] = value
-                captured_variables.remove(name)
-
-        # resolve remaining unset args from scope
-        for v in captured_variables:
-            if not v in kwargs:
-                kwargs[v] = scope.resolve(v)
-        
-        if "output_writer" in kwargs:
-            self.output_writer = kwargs["output_writer"]
-            del kwargs["output_writer"]
-        else:
-            self.output_writer = silent
-
-        return kwargs
-
-    def __call__(self, *args, **kwargs):
-        if not self.is_langchain_use:
-            return self.__acall__(*args, **kwargs)
-        else:
-            return super().__call__(*args, **kwargs)
-
-    async def __acall__(self, *args, **kwargs):
-        kwargs = self.make_kwargs(*args, **kwargs)
-
-        interpreter = PromptInterpreter(force_model=self.model)
-        
-        if self.output_writer is not None:
-            kwargs["output_writer"] = self.output_writer
-        interpreter.set_extra_args(**kwargs)
-
-        query_kwargs = {}
-        for a in self.args:
-            if a in kwargs.keys():
-                query_kwargs[a] = kwargs[a]
+import termcolor
+from lmql.language.fragment_parser import LMQLQuery
+from lmql.language.compiler import PromptScope, SNFList, WhereClauseTransformation
+from lmql.ops.ops import NextToken, digest
+from lmql.runtime.program_state import ProgramState
+from lmql.runtime.lmql_runtime import LMQLQueryFunction
+
+
+global show_transformed
+show_transformed = False
+
+SEQ = "<SEQ placeholder>"
+
+class LMQLExpr: 
+    def __init__(self, node):
+        self.node = node
+    
+    def follow(self, seq, variable_name="SEQ"):
+        for (result, final), follow_map in self.digest(seq, variable_name=variable_name, return_follow_map=True):
+            yield follow_map
+
+    def digest(self, seq, variable_name="SEQ", return_follow_map=False, debug=False):
+        sequence = seq
+        if type(sequence) is str:
+            sequence = sequence.split(" ")
+        full_text = ""
+
+        program_variables = ProgramState()
+        
+        digested = []
+        results = []
+
+        for tok in sequence:
+            added = (" " if len(full_text) > 0 else "") + tok
+            full_text += added
+            text = full_text
+
+            # current context
+            program_variables = program_variables.copy()
+            program_variables.set(variable_name, text, "inc")
+
+            # follow context
+            follow_program_variables = program_variables.copy()
+            follow_program_variables.set(variable_name, text + NextToken, "inc")
+
+            # digest token with where expr
+            result, is_final, trace, follow_trace = digest(self.node,
+                context=program_variables,
+                follow_context=follow_program_variables
+            )
+
+            if type(result) is list: 
+                result = tuple(result)
+            
+            if return_follow_map:
+                yield (result, is_final), self.node.follow_map
             else:
-                query_kwargs[a] = self.scope.resolve(a)
-        
-        # execute main prompt
-        results = await interpreter.run(self.fct, **query_kwargs)
-
-        # applies distribution postprocessor if required
-        results = await (ConditionalDistributionPostprocessor(interpreter).process(results))
-
-        # apply remaining postprocessors
-        if self.postprocessors is not None:
-            for postprocessor in self.postprocessors:
-                results = await postprocessor.process(results, self.output_writer)
-        
-        interpreter.print_stats()
-        interpreter.dcmodel.save()
-
-        return results
-
-def context_call(fct_name, *args, **kwargs):
-    return ("call:" + fct_name, args, kwargs)
-
-def interrupt_call(fct_name, *args, **kwargs):
-    return ("interrupt:" + fct_name, args, kwargs)
-
-def tag(t):
-    return f"<lmql:{t}/>"
-
-def compiled_query(output_variables=None, group_by=None):
-    if output_variables is None:
-        output_variables = []
-    
-    postprocessors = []
-    
-    calling_frame = inspect.stack()[1]
-    
-    if group_by is not None:
-        postprocessors.append(GroupByPostprocessor(group_by))
-    
-    # TODO validate that only one postprocessor is used
-
-    def func_transformer(fct):
-        return LMQLQueryFunction(fct, 
-                                 output_variables=output_variables, 
-                                 postprocessors=postprocessors, 
-                                 scope=LMQLInputVariableScope(fct, calling_frame))
-    return func_transformer
-    
+                if debug:
+                    print(full_text, result, is_final)
+                yield (result, is_final)
+
+class LMQLExpressionCompiler(ast.NodeTransformer):
+    def __init__(self, expr_compiler):
+        self.expr_compiler: WhereClauseTransformation = expr_compiler
+        self.expr_compiler.scope.defined_vars.add("SEQ")
+
+    def visit_Assert(self, node):
+        if node.msg is None:
+            node.msg = ast.Constant(f"Line {node.lineno}: Assertion '{astunparse.unparse(node).strip()}' failed.", kind="str")
+        return node
+    
+    def visit_Call(self, node):
+        translated_calls = set(["inc", "dec", "fin", "var"])
+        if type(node.func) is ast.Name and node.func.id in translated_calls:
+            return ast.Call(
+                ast.Name("raw_constant"),
+                node.args + [ast.Constant(node.func.id, "str")],
+                []
+            )
+        node.args = [self.visit(a) for a in node.args]
+
+        return node
+
+    def visit_Assign(self, node: ast.Assign):
+        if type(node.value) is ast.Call:
+            if type(node.value.func) is ast.Name and node.value.func.id == "LMQLExpr":
+                call = self.visit(node.value)
+                snf = SNFList()
+                
+                direct_result = self.expr_compiler.transform_node(call.args[0], snf)
+                value = ast.Name(snf.last_var()) if snf.var_counter > 0 else ast.parse(direct_result.strip())
+
+                return ast.copy_location(ast.Expr([
+                    # ast.parse("import lmql.runtime.lmql_runtime as lmql"),
+                    snf.ast(),
+                    ast.Assign(
+                        node.targets, 
+                        ast.Call(ast.Name("LMQLExpr"), [value], [])
+                    )
+                ]), node)
+        
+        return node
+
+def lmql_test(fct):
+    source = inspect.getsource(fct)
+    startline = inspect.getsourcelines(fct)[1]
+    source = '\n'.join(source.splitlines()[1:])
+    source = " \n" * startline + source
+
+    bogus_query = LMQLQuery()
+    bogus_query.scope = PromptScope()
+    bogus_query.scope.defined_vars = set()
+    expr_compiler = WhereClauseTransformation(bogus_query)
+    compiler = LMQLExpressionCompiler(expr_compiler)
+
+    m = ast.parse(source)
+    m = compiler.visit(m)
+
+    code = astunparse.unparse(m)
+
+    global show_transformed
+    if show_transformed: print(code.strip())
+    
+    recompiled = compile(code, fct.__code__.co_filename, 'exec')
+    return types.FunctionType(recompiled.co_consts[0], fct.__globals__)
+
+def fin(v):
+    return (v, "fin")
+
+def var(v):
+    return (v, "var")
+
+def inc(v):
+    return (v, "inc")
+
+def dec(v):
+    return (v, "dec")
+
+def run_all_tests(g):
+    g = g.copy()
+    num_errors = 0
+    loop = asyncio.get_event_loop()
+
+    for k in list(g.keys()):
+        try:
+            if k.startswith("test"): 
+                print("Running", k, "." * (40 - len(k)), end=" ")
+                
+                if type(g[k]) is LMQLQueryFunction:
+                    loop.run_until_complete(g[k]())
+                elif inspect.iscoroutinefunction(g[k]):
+                    loop.run_until_complete(g[k]())
+                else:
+                    g[k]()
+                termcolor.cprint("OK", "green")
+        except AssertionError as e:
+            print(e)
+            num_errors += 1
+            termcolor.cprint("FAILED", "red")
+
+    # wait for all tasks to finish
+    try:
+        for t in asyncio.all_tasks(loop=loop):
+            if t.done(): continue
+            try:
+                t.cancel()
+                loop.run_until_complete(t)
+            except asyncio.CancelledError:
+                pass
+        loop.close()
+    except RuntimeError:
+        pass
+
+    if num_errors != 0: 
+        print(num_errors, "test(s) failed.")
+        sys.exit(1)
+    else: 
+        print("All tests passed.")
+        sys.exit(0)
+
+def enable_show_transformed():
+    global show_transformed
+    show_transformed =True
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/maiohttp.py` & `lmql-0.0.6.4/src/lmql/runtime/maiohttp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Mocked aiohttp client session for use in pyodide.
+"""
+
 import asyncio
 import js
 from pyodide.ffi import to_js
 import json
 
 class EndStream: pass
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/masks.py` & `lmql-0.0.6.4/src/lmql/runtime/masks.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.0.6.4/src/lmql/runtime/multi_head_interpretation.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         self.trace.append(result)
         self.current_args = await self.iterator_fct().asend(result)
         await self.handle_current_arg()
 
     async def materialize_copy_if_necessary(self):
         # materialize lazy copy if not yet done
         if self._iterator_fct is None:
+            if "__self__" in self.kwargs:
+                self.kwargs["self"] = self.kwargs.pop("__self__")
             self._iterator_fct = self.fct(*self.args, **self.kwargs)
 
             if len(self.future_trace) > 0:
                 await self.fast_forward()
 
     async def handle_current_arg(self):
         if type(self.current_args) is tuple and len(self.current_args) >= 2 and self.current_args[0].startswith("call:"):
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/openai_integration.py` & `lmql-0.0.6.4/src/lmql/runtime/openai_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,34 +12,25 @@
 import lmql.runtime.dclib as dc
 import lmql.utils.nputil as nputil
 from lmql.runtime.dclib.dclib_model import DcModel
 from lmql.runtime.dclib.dclib_seq import (DecoderSequence, deepcopy, deepmerge,
                                           detseq, is_deterministic)
 from lmql.runtime.stats import Stats
 from lmql.runtime.tokenizer import load_tokenizer
+from lmql.runtime.tokenizers.tiktoken_tokenizer import TiktokenTokenizer
 from lmql.utils import nputil
+from lmql.runtime.token_distribution import TokenDistribution
 
 
 def is_allowed(m): 
     """
     Given a logits mask, sets tensor cell value to True iff the corresponding token is allowed according to the mask.
     """
     return np.isclose(m, 0, atol=1e-8)
 
-def openai_complete_create(*args, **kwargs):
-    if kwargs.get("chaos", False):
-        import random
-        if random.random() < 0.5:
-            if random.random() < 0.5:
-                raise openai.error.ServiceUnavailableError("Chaos monkey error", 500, "Chaos monkey error")
-            else:
-                raise openai.error.APIError("Chaos monkey error", 500, "Chaos monkey error")
-
-    return openai.Completion.create(*args, **kwargs)
-
 @dataclass
 class CompleteTask:
     op: Callable
     result: Any
     continuation_type: str
     logit_mask_or_fixed_id: Optional[Union[np.ndarray, int]] = None
 
@@ -97,32 +88,39 @@
             mask_key_segment = [f"{id}={value}" for id, value in sorted(api_mask.items(), key=lambda x: x[0])]
             mask_key_segment = "-".join(mask_key_segment)
         else:
             mask_key_segment = "*"
         return f"{parameter_values_key_segment}-{mask_key_segment}"
 
 class DclibOpenAiModel(DcModel):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, truncation_threshold=-120, init_workers=False, **kwargs)
+    def __init__(self, *args, endpoint=None, **kwargs):
+        super().__init__(*args, truncation_threshold=-12000, init_workers=False, **kwargs)
+        
+        self.mock = kwargs.get("mock", False)
 
         # if available, store reference to output writer for eager stats reporting
         self.output_writer = None
         if "output_writer" in kwargs:
             self.output_writer = kwargs["output_writer"]
         
         self.model_identifier = "openai/" + self.model.model_identifier
 
-        self.model.chunk_size = kwargs.get("openai_chunksize", 64)
+        self.model.chunk_size = kwargs.get("openai_chunksize", 64 if not self.mock else 8)
         self.model.nostop = kwargs.get("openai_nonstop", False)
         self.num_billed_tokens = {}
         self.num_requests = 0
+        
+        self.api_config = {**({"endpoint": endpoint}  if endpoint is not None else {}), **kwargs}
+        self.timeout = kwargs.get("chunk_timeout", 1.5 if not self.mock else 4.5)
 
         self.stats = Stats("openai")
         openai.AsyncConfiguration.set_tokenizer(self.tokenize)
 
+        assert not "hf-" in self.tokenizer.name, "OpenAI models are not compatible with HuggingFace tokenizers. Please use 'tiktoken' or 'gpt3_tokenizer' instead."
+
     def log_billable_tokens(self, n: int):
         pass # openai keeps track of billable tokens vai bopenai
     
     def log_queries(self, n: int):
         pass # openai keeps track of queries via bopenai
 
     def prepare_completion_call(self, s, mask, **kwargs):
@@ -141,59 +139,94 @@
             return CompletionCall("*", None, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
 
         invert = False
         num_allowed = masks.mask_num_allowed(mask)
         assert num_allowed > 0, "DclibOpenAiModel: encountered logits mask with no allowed tokens: mask: {} mask type:{}".format(mask, type(mask))
 
         if num_allowed == 1:
+            token_id = masks.mask_get_only_allowed(mask)
+            token = self.tokenizer.decode_bytes([token_id])[0]
+
             # check for <eos> case
             if masks.mask_is_allowed(mask, self.eos_token_id):
-                return CompletionCall("fixed", self.eos_token_id, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
+                return CompletionCall("fixed", token, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
             else:
                 # otherwise we can treat this as a score call
-                return CompletionCall("fixed", masks.mask_get_only_allowed(mask), s.input_ids, kwargs, stopping_phrases=stopping_phrases)
+                return CompletionCall("fixed", token, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
         elif num_allowed < self.tokenizer.vocab_size:
             if self.tokenizer.vocab_size - num_allowed > num_allowed:
                 # if we have to mask more than half of the tokens, we should just invert the masking
                 invert = True
         else: # num_allowed == mask.shape[-1] (full vocabulary)
             return CompletionCall("*", None, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
 
         # num_allowed < mask.shape[-1] and num_allowed > 1 (needs mask)
         return CompletionCall("complete", mask, s.input_ids, kwargs, invert=invert, stopping_phrases=stopping_phrases)
 
     async def api_score(self, input_ids, offset):
+        if input_ids[0] == self.tokenizer.bos_token_id:
+            input_ids = input_ids[1:]
+
+        prompt_str = self.tokenizer.convert_bytes_to_string(input_ids)
+
+        # rstripped_eos = False
+        # if prompt_str.endswith("<|endoftext|>"):
+        #     rstripped_eos = True
+        #     prompt_str = prompt_str[:-13]
+        if "<|endoftext|>" in prompt_str:
+            # tokenize
+            prompt_str = await self.tokenize(prompt_str)
+
         kwargs = {
             "model": self.model.model_identifier,
-            "prompt": input_ids.tolist(),
+            "prompt": prompt_str,
             "max_tokens": 0,
             "temperature": 0,
             "logprobs": 1,
             "user": "lmql",
-            "echo": True
+            "echo": True,
+            **({"api_config": self.api_config} if self.api_config is not None else {}),
+            **({"timeout": self.timeout} if self.timeout is not None else {}),
         }
 
+        if self.model_args.get("chatty_openai", False):
+            args = kwargs.copy()
+            # args["prompt"] = str([await self.detokenize(kwargs["prompt"])])[2:-2]
+            print(f"openai score: {args}", flush=True)
+
         logprobs = []
         async for data in await openai.Completion.create(**kwargs):
             logprobs += data["logprobs"]["token_logprobs"]
         return np.array(logprobs[offset:], dtype=np.float32)
 
     async def queue_api_score(self, kwargs):
         # put task in self.score_queue and await result
         loop = asyncio.get_running_loop()
         result_fut = loop.create_future()
         self.score_queue.put_nowait((kwargs,result_fut))
         return await result_fut
 
     async def _score_next_tokens(self, s, next_tokens, noscore=False):
-        if noscore:
-            return np.zeros(len(next_tokens), dtype=np.float32)
-        return (await self.api_score(np.concatenate([s.input_ids, next_tokens], axis=0), len(s.input_ids)))
+        if noscore: return np.zeros(len(next_tokens), dtype=np.float32)
+        
+        prompt_str = self.tokenizer.convert_bytes_to_string(s.input_ids)
+        tokenized_input_ids = await self.tokenize(prompt_str)
+
+        res = await self.api_score(np.concatenate([s.input_ids, next_tokens], axis=0), len(tokenized_input_ids))
+
+        server_side_swallowed_tokens = 0
+        while len(res) < len(next_tokens):
+            res = np.append(res, 0.0)
+            server_side_swallowed_tokens += 1
+        if server_side_swallowed_tokens > 0:
+            print("warning: The OpenAI API has merged {} token(s) server-side, which will reflect in inaccurate 0.0 scores in the decoding tree".format(server_side_swallowed_tokens))
+
+        return res
     
-    async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=4, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False, internal=False):
+    async def score(self, sqs: List[DecoderSequence], tokens: List[List[bytes]], max_batch_size=4, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False, internal=False):
         assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
 
         def make_detseq(s, token_score, completion):
             # compose deterministic flags
             if type(deterministic) is bool:
                 deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])])
                 next_deterministic = np.array([deterministic] * len(completion[1:]))
@@ -218,82 +251,89 @@
         results = []
 
         async for (s, tokens, scores) in self.score_tokens(sqs, tokens, max_batch_size=max_batch_size, noscore=noscore):
             results.append(make_detseq(s, scores, tokens))
 
         return results
     
-    async def score_tokens(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, noscore=False):
+    async def score_tokens(self, sqs: List[DecoderSequence], tokens: List[List[bytes]], max_batch_size=None, noscore=False):
         completion = [np.array(cont) for cont in tokens]
 
         for s, tokens,scores in zip(sqs, completion, await asyncio.gather(*(self._score_next_tokens(s, compl, noscore=noscore) for s, compl in zip(sqs, completion)))):
             yield (s, tokens, scores)
 
     async def async_complete(self, completion_call: Union[CompletionCall, List[CompletionCall]], **kwargs) -> openai.response_buffer:
         assert type(completion_call) is CompletionCall
 
         batch_size = 1
         input_ids = completion_call.input_ids.reshape(-1)
-        assert input_ids.ndim == 1, f"_complete expects input_ids to be a 1D tensor when only one completion_call is passed, got {input_ids.ndim}D tensor."
+        prompt_str = self.tokenizer.convert_bytes_to_string(input_ids)
+        tokenized_input_ids = await self.tokenize(prompt_str)
+
+        # do not include bos token in prompt for request
+        if input_ids[0] == self.tokenizer.bos_token_id:
+            input_ids = input_ids[1:]
 
         temperature = completion_call.kwargs.get("temperature", 0.0)
         logprobs = completion_call.kwargs.get("logprobs", 5)
         noscore = completion_call.kwargs.get("noscore", False)
 
         kwargs = {
             "model": self.model.model_identifier,
-            "prompt": input_ids.tolist(), # no more batching at this point
+            "prompt": prompt_str, # no more batching at this point
             "max_tokens": self.model.chunk_size,
             "temperature": temperature,
             "logprobs": logprobs,
             "user": "lmql",
             "stream": True,
-            "echo": True
+            "echo": True,
+            **({"api_config": self.api_config} if self.api_config is not None else {}),
+            **({"timeout": self.timeout} if self.timeout is not None else {}),
         }
 
         mode = completion_call.mode
         
         if mode == "*": # complete without mask
             pass
         elif mode == "complete": # complete with mask
             logit_bias = completion_call.api_mask
             # reduce chunk size, if logit mask seems very sparse
             if len(logit_bias) > 0 and max(logit_bias.values()) == 100 and len(logit_bias) < 10:
                 kwargs["max_tokens"] = min(kwargs["max_tokens"], 4)
             kwargs.update({"logit_bias": logit_bias})
         elif mode == "fixed": # complete with fixed token
             fixed_next_token = completion_call.logit_mask_or_fixed_id # special return value case for prepare function
-            # TODO revisit this, what kind of probability do we want here (masked or unmasked/scored)
-            if fixed_next_token == self.eos_token_id:
+
+            if fixed_next_token == self.eos:
                 return CompletionResult(openai.response_buffer.singleton(token=fixed_next_token, token_logprob=0), completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
             else:
-                fixed_next_token = nputil.ensure_array(fixed_next_token, dtype=np.int64)
                 if noscore: logprob = 0.0
-                else: logprob = (await self.api_score(np.concatenate([input_ids, fixed_next_token.reshape(1)], axis=0), len(input_ids)))
-                return CompletionResult(openai.response_buffer.singleton(token=fixed_next_token, token_logprob=logprob), completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
+                else: logprob = (await self.api_score(np.append(input_ids, fixed_next_token, axis=0), len(tokenized_input_ids)))
+                return CompletionResult(openai.response_buffer.singleton(token=fixed_next_token, token_logprob=logprob), 
+                                        completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
         else:
             assert False, f"Internal openai API dispatcher returned an unknown completion mode {mode}"
 
         if len(completion_call.stopping_phrases) > 0:
             if len(completion_call.stopping_phrases) > 4:
                 # same but blaming it more on OpenAI
                 print("warning: the number of stopping phrases that would need to be passed to the OpenAI API is greater than 4. Since the OpenAI API only supports up to 4 stopping phrases, the first 4 stopping phrases will be passed to the API. Other stopping phrases will also be enforced, but may lead to an increase in the number of tokens billed to the user.")
             # skip stopping phrases for more speculative execution
             if not self.model.nostop:
                 kwargs.update({"stop": completion_call.stopping_phrases[:4]})
 
         # TODO: we are now overestimate the number of tokens billed to the user since we are not account for stopping phrases for the sake of streaming
-        self.count_billed_tokens(input_ids.size + kwargs.get("max_tokens") * batch_size, self.model_identifier)
+        self.count_billed_tokens(len(tokenized_input_ids) + kwargs.get("max_tokens") * batch_size, self.model_identifier)
         
         if self.model_args.get("chatty_openai", False):
             args = kwargs.copy()
-            args["prompt"] = str([await self.detokenize(kwargs["prompt"])])[2:-2]
-            print(f"openai complete: {args}")
-
-        return CompletionResult((await openai.async_buffer(await openai.Completion.create(**kwargs), tokenizer=self.tokenize_list))[input_ids.size:], completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
+            # args["prompt"] = str([await self.detokenize(kwargs["prompt"])])[2:-2]
+            print(f"openai complete: {args}", flush=True)
+        
+        return CompletionResult((await openai.async_buffer(await openai.Completion.create(**kwargs), tokenizer=self.tokenize_list))[len(tokenized_input_ids):], completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
     
     async def tokenize_list(self, tokens: List[str]):
         if len(tokens) > 0 and type(tokens[0]) is str:
             return [[t[0]] for t in await self.model.tokenize(tokens)]
         return tokens
     
     async def openai_cache_delegate(self, kwargs, tokens, scores):
@@ -344,64 +384,84 @@
                     None,
                     None,
                 )
 
             completion_result = await self.async_complete(completion_call)
             # eagerly expand and cache full completion if a cache_delegate is available
             if self.cache_delegate is not None:
-                await self.expand_and_cache(s, completion_result, "top-1", logprobs=kwargs.get("logprobs", 1))
+                await self.expand_and_cache(s, completion_result, 
+                                            "top-1" if temperature == 0.0 else f"sample-{temperature}",
+                                            logprobs=kwargs.get("logprobs", 1))
             
-            assert not await completion_result.buffer.empty(), "Completion result is empty on arrival"
+            assert not await completion_result.buffer.empty(), "Completion result is empty on arrival: {}".format(str([await self.detokenize(completion_call.input_ids)]))
             return completion_result
 
         return await asyncio.gather(*[get_buffer(i, s) for i, s in enumerate(seqs)])
 
-    async def expand_and_cache(self, s: DecoderSequence, completion_result: CompletionResult, edge_type, logprobs=1):
+    async def expand_and_cache(self, s: DecoderSequence, completion_result: CompletionResult, sampling_mode, logprobs=1):
         async def token_stream():
-            nonlocal edge_type, s, completion_result
+            nonlocal sampling_mode, s, completion_result
             response_buffer = completion_result.buffer
             
             try:
                 tokens = []
                 scores = []
 
                 while True:
                     try:
                         if await response_buffer.empty():
                             break
-
                         res = await response_buffer.get(0)
-                        tokens = nputil.ensure_iterable(res["logprobs"]["tokens"])
-                        scores = res["logprobs"]["token_logprobs"]
-
+                        
+                        # prepare top_entries
+                        top_entries = {}
                         topprobs = res["logprobs"]["top_logprobs"]
                         if topprobs is not None and logprobs > 1:
                             topk_tokens = list(topprobs.items())
-                            topk_tokens = [(tok[0], score) for (tok_str, score), tok in zip(topk_tokens, await self.tokenize_list([s for s,_ in topk_tokens]))]
+                            topk_tokens = [(tok, score) for (tok_str, score), tok in zip(topk_tokens, [s for s,_ in topk_tokens])]
                             topk_tokens += [(tokens[0], scores)]
                             topk_tokens = list(dict.fromkeys(topk_tokens))
                             topk_tokens = sorted(topk_tokens, key=lambda x: x[1], reverse=True)
                             topk_tokens = topk_tokens[:logprobs]
-                            
-                            tokens = [tok for tok, _ in topk_tokens]
-                            scores = [score for _, score in topk_tokens]
-                            edge_type = ["top-{}".format(i+1) for i in range(len(topk_tokens))]
-                        
+                            top_entries = {tok: score for tok, score in topk_tokens}
+
+                        scores = {}
+                        for t, s in top_entries:
+                            scores[t] = s
+                        if sampling_mode == "top-1":
+                            scores[res["logprobs"]["tokens"]] = res["logprobs"]["token_logprobs"]
+
+                        top_entries = list(sorted(scores.items(), key=lambda x: x[1], reverse=True))
+                        tokens = [t for t, _ in top_entries]
+                        scores = [s for _, s in top_entries]
+                        edge_type = ["top-{}".format(i+1) for i in range(len(tokens))]
+
+                        # for non argmax sampling modes, add the sampled token to the beginning of the list
+                        if sampling_mode != "top-1":
+                            tokens = [res["logprobs"]["tokens"]] + tokens
+                            scores = [res["logprobs"]["token_logprobs"]] + scores
+                            edge_type = [sampling_mode] + edge_type
+
+                        # convert tokens to bytes
+                        tokens = self.convert(tokens)
+
                         # future continuation
                         response_buffer = response_buffer[1:]
                         continuation = CompletionResult(response_buffer, completion_result.continuation_type, completion_result.logit_mask_or_fixed_id)
 
                         if continuation.continuation_type is None:
                             edge_type = None
 
                         user_data = {
                             "openai-continuations": {
                                 continuation.continuation_type: continuation
                             }
                         }
+                        # print("token stream gives", result_id, tokens, scores, edge_type, flush=True)
+
                         yield (s, tokens, scores, edge_type, user_data)
                     except IndexError:
                         break
                 # print("fully expanded speculativate continuation:", [await self.detokenize(tokens)], flush=True)
                 # if len(tokens) > 1:
                 #     await self.cache(s, tokens, scores, edge_type)
             except Exception as e:
@@ -431,15 +491,15 @@
     async def sample(self, sequences, num_samples=1, **kwargs):
         """
         Returns a pool with `n` sampled successor nodes per node in the pool.
         """
         kwargs = {**self.model_args, **kwargs}
 
         async def op_sample(seqs):
-            completions: List[CompletionResult] = await self.completion_buffer(seqs, logprobs=1, **kwargs)
+            completions: List[CompletionResult] = await self.completion_buffer(seqs, logprobs=num_samples, **kwargs)
             
             next_token_ids = []
             next_token_scores = []
             logits = []
             continuation_buffers: List[CompletionResult] = []
 
             for s, completion in zip(seqs, completions):
@@ -448,64 +508,61 @@
 
                 # store pointer to continuation buffers in newly expanded nodes
                 continuation = CompletionResult(completion.buffer[1:], completion.continuation_type, completion.logit_mask_or_fixed_id)
                 continuation_buffers.append(continuation)
 
                 # detect fixed results (i.e. deterministic tokens)
                 if "fixed" in complete_data.keys():
-                    next_token = complete_data["logprobs"]["tokens"]
+                    next_token = [complete_data["logprobs"]["tokens"]]
                     next_token_score = complete_data["logprobs"]["token_logprobs"]
-                    next_token_ids.append(np.array([next_token], dtype=np.int64))
+                    next_token_ids.append(np.array([next_token]))
                     next_token_scores.append(np.array([next_token_score], dtype=np.float32))
                     
-                    full_logits = np.ones(self.model.get_tokenizer().vocab_size) * np.finfo(np.float32).min
-                    if next_token < len(full_logits):
-                        full_logits[next_token] = next_token_score
+                    full_logits = TokenDistribution()
+                    full_logits[next_token] = next_token_score
                     # else: 
                     #  next_token is a special token, which is not in the vocab
                     logits.append(full_logits)
                     continue
 
                 # get sampled token and score
-                next_token = complete_data["logprobs"]["tokens"][0]
+                next_token = complete_data["logprobs"]["tokens"]
                 next_token_score = complete_data["logprobs"]["token_logprobs"]
                 
                 probs = sorted(list(complete_data["logprobs"]["top_logprobs"].items()))
                 logprobs = [p[1] for p in probs]
                 tokens = [p[0] for p in probs]
-                prob_tokens = await self.tokenize_list(tokens)
-                token_ids = np.array(prob_tokens, dtype=np.int64).reshape(-1)
 
-                full_logits = np.ones(self.model.get_tokenizer().vocab_size) * np.finfo(np.float32).min
-                full_logits[token_ids] = np.array(logprobs)
-                full_logits[next_token] = np.finfo(np.float32).min
-                assert kwargs.get("temperature", 1.0) != 0.0 or np.all(full_logits < next_token_score), "next token score is not the highest"
+                distribution = TokenDistribution()
+                distribution[tokens] = logprobs
+                distribution[next_token] = np.finfo(np.float32).min
 
                 # retroactively apply logits mask to logits
                 mask = completion.logit_mask_or_fixed_id
                 if mask is None:
                     pass
                 elif type(mask) is int: 
-                    full_logits[mask] = np.finfo(np.float32).min
+                    distribution[mask] = np.finfo(np.float32).min
                 else: 
-                    full_logits[mask < 0] = np.finfo(np.float32).min
+                    distribution[mask < 0] = np.finfo(np.float32).min
 
-                additional_sampled_token_ids, _ = nputil.multinomial(full_logits, num_samples=num_samples - 1)
+                additional_sampled_token_ids, _ = distribution.sample(num_samples=num_samples - 1)
 
-                seq_next_token_ids = np.concatenate([np.array(next_token).reshape(1), additional_sampled_token_ids], axis=0)
-                full_logits[next_token] = next_token_score
-                # seq_next_token_scores = full_logits.gather(-1, seq_next_token_ids)
-                seq_next_token_scores = np.take_along_axis(full_logits, seq_next_token_ids, axis=-1)
+                seq_next_token_ids = [next_token] + additional_sampled_token_ids
+                distribution[next_token] = next_token_score
+                seq_next_token_scores = distribution.score(seq_next_token_ids)
 
                 next_token_ids.append(seq_next_token_ids)
                 next_token_scores.append(seq_next_token_scores)
-                logits.append(full_logits)
+                logits.append(distribution)
+
+            token_ids = [self.convert(t) for t in next_token_ids]
 
             logits = logits
-            next_token_ids = next_token_ids
+            next_token_ids = token_ids
             next_token_scores = next_token_scores
 
             def successor_user_data(continuation_buffer: SequenceResult, num_successors):
                 default_user_data = {}
                 if continuation_buffer.continuation_type is None:
                     return [default_user_data.copy()] * num_successors
                 continuation_as_user_data = {
@@ -517,14 +574,39 @@
                 return [continuation_as_user_data] + [default_user_data.copy()] * (num_successors - 1)
 
             return [s.make_successors(next_token_ids[i], next_token_scores[i], logits=logits[i], 
                 user_data=successor_user_data(continuation_buffers[i], len(next_token_ids[i]))) for i,s in enumerate(seqs)]
         with self.stats.timer("sample"):
             return await sequences.aelement_wise(op_sample)
 
+    def frombytes(self, s):
+        r = []
+        i = 0
+        while i < len(s):
+            if s[i:i+2] == "\\x":
+                r += [int(s[i+2:i+4], 16)]
+                i += 4
+            else:
+                r += [ord(s[i])]
+                i += 1
+        return bytes(r)
+
+    def convert(self, token):
+        result = []
+        for t in token:
+            if type(t) is int or (type(t) is np.ndarray and t.dtype != np.str_):
+                result.append(t)
+            elif type(t) is bytes:
+                result.append(t)
+            elif t.startswith("bytes:"):
+                result.append(self.frombytes(t[6:]))
+            else:
+                result.append(t.encode("utf-8"))
+        return result
+
     async def topk_continuations(self, sequences, k, **kwargs):
         """
         Returns a pool with `n` sampled successor nodes per node in the pool.
         """
         assert k <= 5, "The OpenAI API only supports topk probabilities with k <= 5"
         assert k >= 1, "topk_continuations() requires k >= 1"
         
@@ -545,71 +627,73 @@
                 complete_data = (await completion.buffer.get(0))
                 # store pointer to continuation buffers in newly expanded nodes
                 continuation = CompletionResult(completion.buffer[1:], completion.continuation_type, completion.logit_mask_or_fixed_id)
                 continuation_buffers.append(continuation)
 
                 # detect fixed results (i.e. deterministic tokens)
                 if "fixed" in complete_data.keys():
-                    next_token = complete_data["logprobs"]["tokens"]
+                    next_token = [complete_data["logprobs"]["tokens"]]
                     next_token_score = complete_data["logprobs"]["token_logprobs"]
-                    next_token_ids.append(np.array([next_token], dtype=np.int64))
+                    next_token_ids.append(np.array([next_token]))
                     next_token_scores.append(np.array([next_token_score], dtype=np.float32))
                     
-                    full_logits = np.ones(self.model.get_tokenizer().vocab_size) * np.finfo(np.float32).min
-                    full_logits[next_token] = next_token_score
-                    logits.append(full_logits)
+                    distribution = TokenDistribution()
+                    distribution[next_token] = next_token_score
+                    logits.append(distribution)
                     continue
 
                 # get sampled token and score
-                next_token = complete_data["logprobs"]["tokens"][0]
+                next_token = complete_data["logprobs"]["tokens"]
                 next_token_score = complete_data["logprobs"]["token_logprobs"]
                 
                 probs = sorted(list(complete_data["logprobs"]["top_logprobs"].items()), key=lambda x: x[1], reverse=True)
                 logprobs = [p[1] for p in probs]
                 tokens = [p[0] for p in probs]
-                token_ids = np.array([self.model.get_tokenizer()(t)["input_ids"][0] for t in tokens], dtype=np.int64)
-
-                assert token_ids[0] == next_token, f"top1 logprob token is not the same as the predicted token {token_ids[0]} (top1) != {next_token} (predicted)"
 
-                full_logits = np.ones(self.model.get_tokenizer().vocab_size) * np.finfo(np.float32).min
-                full_logits[token_ids] = np.array(logprobs)
+                distribution = TokenDistribution()
+                distribution[tokens] = logprobs
 
                 # retroactively apply logits mask to logits
                 mask = completion.logit_mask_or_fixed_id
                 if mask is None: pass
-                elif type(mask) is int: full_logits[mask] = np.finfo(np.float32).min
-                else: full_logits[mask < 0] = np.finfo(np.float32).min
+                elif type(mask) is int: distribution[mask] = np.finfo(np.float32).min
+                else: distribution[mask < 0] = np.finfo(np.float32).min
                 
                 # make sure all token_ids are unique
-                token_ids = np.array(list(set(token_ids)))
+                tokens = np.array(list(set(tokens)))
 
                 # re-determine logprobs with logits mask applied
-                logprobs = np.take_along_axis(full_logits, token_ids, axis=-1)
+                logprobs = distribution.score(tokens)
 
-                next_token_ids.append(token_ids)
+                next_token_ids.append(tokens)
                 next_token_scores.append(logprobs)
-                logits.append(full_logits)
+                logits.append(distribution)
+
+            next_token_ids = [self.convert(t) for t in next_token_ids]
 
             def successor_user_data(continuation_buffer: SequenceResult, num_successors):
                 default_user_data = {}
                 if continuation_buffer.continuation_type is None:
                     return [default_user_data.copy()] * num_successors
                 continuation_as_user_data = {
                     "openai-continuations": {
                         continuation_buffer.continuation_type: continuation_buffer
                     },
                     **(default_user_data.copy())
                 }
                 return [continuation_as_user_data] + [default_user_data.copy()] * (num_successors - 1)
 
             return [s.make_successors(next_token_ids[i], next_token_scores[i], logits=logits[i], 
-                user_data=successor_user_data(continuation_buffers[i], len(logits[i]))) for i,s in enumerate(seqs)]
+                user_data=successor_user_data(continuation_buffers[i], len(next_token_ids[i]))) for i,s in enumerate(seqs)]
         
         with self.stats.timer("topk"):
             return await sequences.aelement_wise(op_topk)
+        
+    def close(self):
+        pass
 
 class Struct:
     def __init__(self, **entries):
         for k, v in entries.items():
             if isinstance(v, dict):
                 entries[k] = Struct(**v)
             if isinstance(v, list):
@@ -842,36 +926,14 @@
         return await asyncio.get_event_loop().run_in_executor(None, task)
     
     async def detokenize(self, *args, **kwargs):
         def task():
             return self.tokenizer.decode(*args, **kwargs)
         return await asyncio.get_event_loop().run_in_executor(None, task)
         # return self.tokenizer.decode(*args, **kwargs)
-
-    def _complete(self, input_ids, temperature=0, logprobs=1):
-        assert len(input_ids) == 1, f"openai model only supports batch size of 1 with logit masks, provided {len(input_ids)}."
-
-        kwargs = {}
-        if self.logits_mask[-1] is not None:
-            kwargs["logit_bias"] = self.logits_mask[-1]
-
-        kwargs = {
-            "model": self.model_identifier,
-            "prompt": input_ids.tolist(),
-            "max_tokens": self.chunk_size,
-            "temperature": temperature,
-            "logprobs": logprobs,
-            "user": "lmql",
-            "stream": True,
-            **kwargs
-        }
-
-        complete_op = lambda: openai_complete_create(**kwargs)
-        return CompleteTask(complete_op, None, continuation_type=None).run(retries=3)
-        
     
     async def tokenize(self, text):
         return self.tokenizer(text)["input_ids"]
 
     async def __aenter__(self):
         self.previous_context_model = OptimisticChunkBasedOpenAIModel.context_model
 
@@ -905,41 +967,42 @@
     
     def reset_stats(self):
         openai.AsyncConfiguration.get_stats().reset()
 
     def cost_estimate(self, model):
         return openai.AsyncConfiguration.get_stats().cost_estimate(model)
 
-def openai_model(model_identifier):
+def openai_model(model_identifier, endpoint=None, mock=False, **kwargs):
     # make sure openai org and secret are available
-    import lmql.runtime.openai_secret
-    
+    if not mock: from lmql.runtime.openai_secret import openai_secret, openai_org
     class OpenAIModel:
         def __init__(self) -> None:
             self.model_identifier = model_identifier
             self.served_model = None
             self._tokenizer = None
 
-            self.decoder_args = {
-                "openai_chunksize": 64
-            }
+            self.decoder_args = {}
 
         def get_tokenizer(self):
             if self._tokenizer is None:
-                self._tokenizer = load_tokenizer("gpt2")
+                if not mock:
+                    self._tokenizer = load_tokenizer("gpt2")
+                else:
+                    self._tokenizer = load_tokenizer(self.model_identifier)
             self.served_model = self
             return self._tokenizer
 
         def get_dclib_model(self):
             bos_token_id = self.get_tokenizer().bos_token_id
             eos_token_id = self.get_tokenizer().eos_token_id
 
-            dc.set_dclib_tokenizer(dc.tokenizer("lmql-adapter-tokenizer", self.tokenize, self.detokenize, bos_token_id, eos_token_id))
+            dc.set_dclib_tokenizer(self.get_tokenizer())
 
-            return DclibOpenAiModel(self, self.get_tokenizer(), **self.decoder_args)
+            full_args = {**kwargs, **self.decoder_args}
+            return DclibOpenAiModel(self, self.get_tokenizer(), endpoint=endpoint, mock=mock, **full_args)
 
         async def tokenize(self, text):
             return self.get_tokenizer()(text)["input_ids"]
         
         async def detokenize(self, input_ids):
             return self.get_tokenizer().decode(input_ids)
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/openai_secret.py` & `lmql-0.0.6.4/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/runtime/output_writer.py` & `lmql-0.0.6.4/src/lmql/runtime/output_writer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.0.6.4/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 
 class ConditionalDistributionPostprocessor:
     def __init__(self, interpreter):
         self.interpreter = interpreter
         self.output_writer = interpreter.output_writer
 
     async def score(self, prompt: str, values, dcmodel: dc.DcModel):
-        prompt_seq = dc.seq([dcmodel.bos_token_id] + await dcmodel.tokenize(prompt))
-        value_ids = [await dcmodel.tokenize(value) for value in values]
+        prompt_seq = dc.seq(dcmodel.tokenizer.tokenize(prompt, asbytes=True))
+        value_ids = [dcmodel.tokenizer.tokenize(value, asbytes=True) for value in values]
 
         dcmodel.log_billable_tokens(sum(len(ids) + 1 for ids in value_ids) + len(value_ids) * (len(prompt_seq.input_ids)))
         dcmodel.log_queries(sum(len(ids) + 1 for ids in value_ids))
 
         value_scores = []
+
         scoring_results = await dcmodel.score([prompt_seq] * len(value_ids), value_ids)
         for s, value in zip(scoring_results, value_ids):
             s = s.expand()
             value_score = s.logprobs[-len(value):]
             value_scores.append(value_score)
 
         return [np.array(s) for s in value_scores]
@@ -55,15 +56,15 @@
                 print("warning: result {} has no distribution variable set even though a DISTRIBUTION clause is given".format(i))
                 continue
 
             scores = await self.score(result.prompt, distribution_values, model)
 
             # print("Computing P({} | {}) for result {}...".format(distribution_variable, result.prompt[:10] + "...", i))
 
-            scores = np.stack([s.sum() for s in scores], axis=0)
+            scores = np.stack([s.mean() for s in scores], axis=0)
             log_probs = nputil.log_softmax(scores)
             probs = np.exp(log_probs)
             
             distribution = [(value, prob, prompt) for value, prob, prompt in zip(distribution_values, probs, prompts)]
             log_distribution = [(value, log_prob, prompt) for value, log_prob, prompt in zip(distribution_values, log_probs, prompts)]
 
             result.variables[distribution_variable] = max(distribution, key=lambda x: x[1])[0]
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/program_state.py` & `lmql-0.0.6.4/src/lmql/runtime/program_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 class ProgramState:
+    """
+    Program state tracked by the interpreter during program execution.
+    """
     def __init__(self, runtime=None):
         self.variable_values = {}
         # postprocessed, converted variable values if not just str (e.g. objects, int)
         self.variable_program_values = {}
         self.variable_diffs = {}
         self.variable_scores = {}
         self.variable_monotonicity = {}
```

### Comparing `lmql-0.0.6.3/src/lmql/runtime/stats.py` & `lmql-0.0.6.4/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/runtime/tokenizer.py` & `lmql-0.0.6.4/src/lmql/runtime/tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,62 @@
-import asyncio
-from lmql.runtime.caching import cache_file_exists, cachefile
-
-class PythonBackedTokenizer:
-    """ Custom tokenizer to be used only in a browser environment. This tokenizer only supports GPT tokenization. """
-    def __init__(self, model_identifier):
-        import gpt3_tokenizer
-        assert "gpt" in model_identifier, "PythonBackedTokenizer only supports GPT family models"
-
-        self.bos_token_id = 50256
-        self.eos_token_id = 50256
-        self._vocab = None
-
-    @property
-    def vocab_size(self):
-        return len(self.vocab)
-
-    @property
-    def vocab(self):
-        if self._vocab is None:
-            import gpt3_tokenizer
-            self._vocab = gpt3_tokenizer._entry._encoder
-        return self._vocab
+"""
+Tokenizer interface required by LMQL. 
 
-    def convert_tokens_to_string(self, tokens):
-        import gpt3_tokenizer
-        text_with_bytes = "".join(tokens)
-        textarr = [int(gpt3_tokenizer._entry._byte_decoder[x]) for x in list(text_with_bytes)]
-        text = bytearray(textarr).decode("utf-8")
-        return text
-
-    def tokenize(self, s):
-        if ("<|endoftext|>" in s):
-            return [50256];
-        import gpt3_tokenizer
-        unpack = False
-        if type(s) is not list:
-            s = [s]
-            unpack = True
-
-        tokens = [[gpt3_tokenizer._entry._decoder[i] for i in gpt3_tokenizer.encode(se)] for se in s]
-
-        if unpack:
-            return tokens[0]
-        else:
-            return tokens
-        
-    def decode(self, input_ids, clean_up_tokenization_spaces=None):
-        import gpt3_tokenizer
-        return gpt3_tokenizer.decode(input_ids)
+See .tokenizers for concrete implementations.
+"""
 
-    def __call__(self, s: str, add_special_tokens=False):
-        import gpt3_tokenizer
-        
+import os
+import pickle
+import numpy as np
+from lmql.runtime.caching import cache_file_exists, cachefile
 
-        unpack = False
-        if type(s) is not list:
-            s = [s]
-            unpack = True
-        
-        input_ids = [gpt3_tokenizer.encode(se) if se != "<|endoftext|>" else [self.eos_token_id] for se in s]
-        
-        if unpack:
-            return {"input_ids": input_ids[0]}
-        else:
-            return {"input_ids": input_ids}
+from lmql.runtime.tokenizers.pure_python_tokenizer import PythonBackedTokenizer
+from lmql.runtime.tokenizers.tiktoken_tokenizer import TiktokenTokenizer
+from threading import Thread
 
 global special_token_mappings
 special_token_mappings = {}
 global reverse_special_token_mappings
 reverse_special_token_mappings = {}
 
 class LMQLTokenizer:
     INVALID_CHARACTER = "\uFFFD"
 
-    def __init__(self, tokenizer_impl, model_identifier):
-        self.tokenizer_impl = tokenizer_impl
+    def __init__(self, model_identifier, tokenizer_impl=None, loader=None):
+        self._tokenizer_impl = None
+        self.loader_thread = None
+
+        if loader is not None:
+            def load():
+                t = loader()
+                self._tokenizer_impl = t
+                self.loader_thread = None
+            self.loader_thread = Thread(target=load)
+            self.loader_thread.start()
+        else:
+            self._tokenizer_impl = tokenizer_impl
+
         self.model_identifier = model_identifier
         self.detokenizer_cache = {}
 
         self._vocab = get_vocab(self.tokenizer_impl)
-        self.vocab_range = max(self._vocab.values()) + 1
+        self.vocab_range = max(max(self._vocab.values()) + 1, self.tokenizer_impl.vocab_size)
+
+        if "FORCE_TIKTOKEN" in os.environ:
+            assert type(self.tokenizer_impl) is TiktokenTokenizer
+
+    @property
+    def tokenizer_impl(self):
+        if self._tokenizer_impl is None:
+            self.loader_thread.join()
+        return self._tokenizer_impl
+    
+    @property
+    def name(self):
+        return self.tokenizer_impl.name
 
     @property
     def vocab_size(self):
         # in LMQL vocab_size is the vocab_range (the highest vocabulary ID + 1)
         # this allows us to use a dense one hot array where no IDs are skipped
         return self.vocab_range
 
@@ -98,57 +71,74 @@
     @property
     def vocab(self):
         return self.tokenizer_impl.vocab
 
     def convert_tokens_to_string(self, tokens):
         return self.tokenizer_impl.convert_tokens_to_string(tokens)
 
-    def tokenize(self, s):
+    def tokenize(self, s, asbytes=False):
         tokens = []
         for s in self.chunk_out_by_tags(s, tokenize=False):
             if s.startswith("lmql:"):
-                tokens.append(s)
+                if asbytes:
+                    tokens.append(f"<{s}/>".encode("utf-8"))
+                else:
+                    tokens.append(s)
             else:
-                tokens += self.tokenizer_impl.tokenize(s)
+                tokens += self.tokenizer_impl.tokenize(s, asbytes=asbytes)
+
         return tokens
+    
+    def decode_bytes(self, input_ids):
+        """
+        Transforms a list of input ids into a byte sequences.
+        """
+        chunk = []
+        result = []
+        global reverse_special_token_mappings
         
+        for i in input_ids:
+            if i in reverse_special_token_mappings.keys():
+                chunk_result = self.tokenizer_impl.decode_tokens_bytes(chunk)
+                result += chunk_result
+                result.append(reverse_special_token_mappings[i].encode("utf-8"))
+                chunk = []
+            else:
+                chunk.append(i)
+
+        if len(chunk) > 0:
+            result += self.tokenizer_impl.decode_tokens_bytes(chunk)
+
+        return result
+
+    def convert_bytes_to_ids(self, token_bytes):
+        """
+        Transforms text into a tokenized byte sequence.
+        """
+        # TODO: handle special IDs, i.e. tags (only relevant for tag use with LMTP backend)
+        return self.tokenizer_impl.convert_token_bytes_to_ids(token_bytes)
+
+    def convert_bytes_to_string(self, token_bytes):
+        """
+        Transforms token bytes into a text.
+        """
+        # TODO: handle special IDs, i.e. tags (only relevant for tag use with LMTP backend)
+        return self.tokenizer_impl.convert_bytes_to_string(token_bytes)
+
     def decode(self, input_ids):
-        key = str(input_ids)
-        n = len(input_ids)
-        if n in self.detokenizer_cache.keys():
-            if key in self.detokenizer_cache[n].keys():
-                # print("cache hit")
-                return self.detokenizer_cache[n][key]
-        if n-1 in self.detokenizer_cache.keys():
-            key = str(input_ids[:-1])
-            if key in self.detokenizer_cache[n-1].keys():
-                global reverse_special_token_mappings
-                # print("secondary cache hit")
-                if input_ids[-1] >= self.vocab_size:
-                    extended = self.detokenizer_cache[n-1][key] + "<" + reverse_special_token_mappings[input_ids[-1]] + "/>"
-                else:
-                    extended = self.detokenizer_cache[n-1][key] + self.tokenizer_impl.decode([input_ids[-1]], clean_up_tokenization_spaces=False)
-                    if self.INVALID_CHARACTER in extended:
-                        return self.detokenizer_cache[n-1][key]
-                if not n in self.detokenizer_cache.keys():
-                    self.detokenizer_cache[n] = {}
-                self.detokenizer_cache[n][str(input_ids)] = extended
-                return extended
+        if len(input_ids) > 0 and type(input_ids[0]) is np.bytes_:
+            return self.convert_bytes_to_string(input_ids)
 
         s = ""
         for chunk in self.chunk_out_by_special_ids(input_ids):
             if type(chunk) is str:
                 s += chunk
             else:
                 s += self.tokenizer_impl.decode(chunk, clean_up_tokenization_spaces=False)
 
-        if not n in self.detokenizer_cache.keys():
-            self.detokenizer_cache[n] = {}
-        self.detokenizer_cache[n][key] = s
-
         return s
 
     def __call__(self, s: str, add_special_tokens=False):
         input_ids = []
         unpack = False
         if type(s) is not list:
             s = [s]
@@ -208,59 +198,93 @@
             if tokenize:
                 segments.append(self.special_token_id("lmql:" + m.group(1)))
             else:
                 segments.append("lmql:" + m.group(1))
             offset = m.end()
         segments.append(s[offset:])
         return segments
+            
 
 def load_tokenizer_notransformers(model_identifier):
+    if not "SLOW_TOKENIZER_OK" in os.environ.keys():
+        print("warning: using slow python-backed tokenizer as no other tokenizer is available for {} (transformers or tiktoken)".format(model_identifier))
+    assert PythonBackedTokenizer.is_available(), "PythonBackedTokenizer not available. Please make sure the 'gpt3_tokenizer' package is installed."
+    
     return PythonBackedTokenizer(model_identifier)
 
-def load_tokenizer(model_identifier):
-    import os
-
-    # first try to load pickled tokenizer from cache (faster)
-    import pickle
-    import pathlib
-
+def load_tokenizer(model_identifier, type="auto"):
     cache_identifier = model_identifier.replace("/", "-")
     cache_path = f"tokenizer-{cache_identifier}.pkl"
 
+    if type in ["auto", "tiktoken"]:
+        tiktoken_available = False
+        # for GPT models we force non-HF tokenizers (tiktoken or python-backed)
+        try:
+            if TiktokenTokenizer.is_available(model_identifier):
+                tiktoken_available = True
+        except:
+            tiktoken_available = False
+        
+        if tiktoken_available:
+            def loader():
+                if cache_file_exists(cache_path):
+                    with cachefile(cache_path, "rb") as f:
+                        return LMQLTokenizer(model_identifier, pickle.load(f))
+                else:
+                    t = TiktokenTokenizer(model_identifier)
+
+                    with cachefile(cache_path, "wb") as f:
+                        pickle.dump(t, f)
+                return t
+            
+            return LMQLTokenizer(model_identifier, loader=loader)
+
     try:
-        import torch
-        from transformers import AutoTokenizer
+        assert type in ["auto", "hf"]
 
-        if cache_file_exists(cache_path):
-            with cachefile(cache_path, "rb") as f:
-                return LMQLTokenizer(pickle.load(f), model_identifier)
-        else:
-            t = AutoTokenizer.from_pretrained(model_identifier)
+        def loader():
+            import os
+            os.environ["TOKENIZERS_PARALLELISM"] = "true"
+
+            import torch
+            from lmql.runtime.tokenizers.hf_tokenizer import TransformersTokenizer
+
+            assert TransformersTokenizer.is_available(model_identifier), "TransformersTokenizer not available. Please make sure the 'transformers' package is installed."
+
+            if cache_file_exists(cache_path):
+                with cachefile(cache_path, "rb") as f:
+                    return LMQLTokenizer(pickle.load(f), model_identifier)
+            else:
+                t = TransformersTokenizer(model_identifier)
 
-            with cachefile(cache_path, "wb") as f:
-                pickle.dump(t, f)
+                with cachefile(cache_path, "wb") as f:
+                    pickle.dump(t, f)
+            return t
+        return LMQLTokenizer(model_identifier, loader=loader)
     except Exception as e:
-        # print("info: trying to use python-based tokenizer as 'transformers' is not available")
         # fallback to non-transformers tokenizer
         t = load_tokenizer_notransformers(model_identifier)
 
-    return LMQLTokenizer(t, model_identifier)
+        return LMQLTokenizer(model_identifier, t)
 
 def get_vocab(tokenizer):
     if hasattr(tokenizer, "vocab"):
         return tokenizer.vocab
     elif hasattr(tokenizer, "get_vocab"):
         return tokenizer.get_vocab()
     elif hasattr(tokenizer, "tokenizer_impl"):
         return get_vocab(tokenizer.tokenizer_impl)
+    elif hasattr(tokenizer, "tokenizer"):
+        return get_vocab(tokenizer.tokenizer)
     else:
         assert False, "Could not obtain full vocabulary from unknown tokenizer type: {}".format(type(tokenizer))
 
 if __name__ == "__main__":
     import sys
+    import torch
 
     model_identifier = sys.argv[1]
     t = load_tokenizer(model_identifier)
 
     to_tokenize = sys.argv[2]
 
     if to_tokenize.startswith("["):
```

### Comparing `lmql-0.0.6.3/src/lmql/tests/fin_and.py` & `lmql-0.0.6.4/src/lmql/tests/fin_and.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/outdated/mask_product_test.py` & `lmql-0.0.6.4/src/lmql/tests/outdated/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/outdated/monotonicity.py` & `lmql-0.0.6.4/src/lmql/tests/outdated/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/outdated/one_of_tests.py` & `lmql-0.0.6.4/src/lmql/tests/outdated/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/outdated/sentences_op.py` & `lmql-0.0.6.4/src/lmql/tests/outdated/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/outdated/starts_with_op_test.py` & `lmql-0.0.6.4/src/lmql/tests/outdated/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/outdated/stops_at.py` & `lmql-0.0.6.4/src/lmql/tests/outdated/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/outdated/str_in_str_tests.py` & `lmql-0.0.6.4/src/lmql/tests/outdated/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/outdated/test_multi_head.py` & `lmql-0.0.6.4/src/lmql/tests/outdated/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/outdated/token_set_test.py` & `lmql-0.0.6.4/src/lmql/tests/outdated/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.6.4/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/tail_token_set.py` & `lmql-0.0.6.4/src/lmql/tests/tail_token_set.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,12 +18,8 @@
 
 def test_different_tails():
     p1 = tset("Sun dscreen and Volleyball", prefix=True)
     p2 = tset("Sunscreen and Drinks", prefix=True)
     r = intersect(p1, p2)
     assert r.tail is None, f"Expected None, got '{r.tail}'"
 
-def test_notail_single_token():
-    p1 = tset("Sun", prefix=True)
-    assert p1.tail is None, f"Expected None, got '{p1.tail}'"
-
 run_all_tests(globals())
```

### Comparing `lmql-0.0.6.3/src/lmql/tests/test_back2back_caching.py` & `lmql-0.0.6.4/src/lmql/tests/test_back2back_caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/test_eq.py` & `lmql-0.0.6.4/src/lmql/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/test_sample_queries.py` & `lmql-0.0.6.4/src/lmql/tests/test_sample_queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import tempfile
 import sys
 import time
 import io
 import termcolor
 
+from lmql.runtime.tokenizer import load_tokenizer
 from lmql.runtime.stats import Stats
 
 # load queries by executing ../ui/playground/src/queries.js via node and getting the object of module.exports
 
 def load_queries():
     # file dir
     cwd = os.path.dirname(os.path.realpath(__file__))
@@ -33,14 +34,16 @@
     return json.loads(queries)
 
 
 async def main():
     print("Loading example queries from ../ui/playground/src/queries.js...")
     queries = load_queries()
     stderr = sys.stderr
+
+    print("\nTokenizer Backend: ", type(load_tokenizer("text-davinci-003").tokenizer_impl).__name__, "\n")
     
     api_stats = Stats("openai-api")
 
     for category in queries:
         print(f"{category['category']}")
         
         if "requires_input" in category.keys() and category["requires_input"]:
```

### Comparing `lmql-0.0.6.3/src/lmql/tests/test_scoping.py` & `lmql-0.0.6.4/src/lmql/tests/test_scoping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/tests/test_stopping.py` & `lmql-0.0.6.4/src/lmql/tests/test_stopping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/live/live.js` & `lmql-0.0.6.4/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/live/live.py` & `lmql-0.0.6.4/src/lmql/ui/live/live.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     result = await lmql.run(code, output_writer=output_writer)
 
     for r in (result if type(result) is list else [result]):
         if r is None:
             continue
 
         if type(r) is not lmql.LMQLResult:
-            print(r)
             continue
         
         for v in [v for v in r.variables if v.startswith("P(")]:
             distribution = r.variables[v]
             max_prob = max([p for _,p in distribution])
             labels = []
             for value, prob in distribution:
```

### Comparing `lmql-0.0.6.3/src/lmql/ui/live/livelib.py` & `lmql-0.0.6.4/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/live/yarn.lock` & `lmql-0.0.6.4/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/README.md` & `lmql-0.0.6.4/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/package.json` & `lmql-0.0.6.4/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.6.4/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/index.html` & `lmql-0.0.6.4/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.6.4/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.6.4/src/lmql/ui/playground/src/App.jsx`

 * *Files 1% similar despite different names*

```diff
@@ -914,15 +914,15 @@
 `
 
 class Truncated extends React.Component {
   constructor(props) {
     super(props)
     
     this.state = {
-      typingOffset: 0,
+      typingOffset: 1024,
       expandedText: ""
     }
     this.stepper = null
   }
 
   componentDidMount() {
     this.stepper = setInterval(() => {
@@ -978,14 +978,31 @@
   }
 
   renderContent(content) {
     // make sure to render model output control characters
     content = content.replace(/\\n/g, "\n")
     content = content.replace(/\\t/g, "\t")
 
+    /* convert text to char code */
+    let bytes = []
+    for (let i = 0; i < content.length; i++) {
+      /* check for \xXX and parse charcode from hex */
+      if (content[i] == "\\") {
+        if (content[i + 1] == "x") {
+          let hex = content.substring(i + 2, i + 4)
+          let charCode = parseInt(hex, 16)
+          bytes.push(charCode)
+          i += 3
+          continue;
+        }
+      }
+      bytes = bytes.concat(Array.from(new TextEncoder("utf-8").encode(content[i])))
+    }
+    content = new TextDecoder("utf-8").decode(new Uint8Array(bytes))
+
     let EXPLICIT_CHARS = {
       "\n": "⏎",
       "\t": "⇥",
     }
 
     let elements = []
     let text = ""
```

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.0.6.4/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -212,14 +212,16 @@
 
 function initDecoderGraphCy(element) {
     return cytoscape({
         container: element,
         maxZoom: 2.0,
         boxSelectionEnabled: false,
         autounselectify: true,
+        // dpi scale
+        pixelRatio: 3,
 
         style: [{
                 selector: 'node',
                 style: {
                     // very light gray
                     'background-color': '#f5f5f5',
                     'label': 'data(label)',
@@ -504,29 +506,34 @@
         })
     }, [graphElementRef])
 
     React.useEffect(() => {
         const cy = cyRef.current
         if (cy) {
             if (cyData) {
-                // cy.nodes().remove()
-                // cy.edges().remove()
-
                 // collect unique edges
                 const uniqueEdges = new Map()
                 cyData.edges.forEach(e => {
                     let edge = uniqueEdges.get(e[0])
                     if (!edge) {
                         edge = new Set()
                         uniqueEdges.set(e[0], edge)
                     }
                     edge.add(e[1])
                 })
 
                 function strLabel(label) {
+                    // unpack arrays
+                    if (Array.isArray(label)) {
+                        return label.map(strLabel).join(", ")
+                    }
+                    if (label.startsWith("bytes:")) {
+                        label = label.substring(6)
+                        return label
+                    }
                     if (label === "") {
                         // epsilon
                         return "\u03b5"
                     }
                     if (!label) {
                         return ""
                     }
```

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.6.4/src/lmql/ui/playground/src/Explore.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/State.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.6.4/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.6.4/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.6.4/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.6.4/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/index.css` & `lmql-0.0.6.4/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.6.4/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/queries.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,20 @@
 
         {
             category: "Introductory Examples",
             queries: [{
                 // hello world
                 name: "👋 Hello World",
                 description: "Who This?",
-                code: `argmax "Hello[WHO]" from "openai/text-ada-001" where len(WHO) < 10`,
+                code: `argmax 
+   "Say 'this is a test':[RESPONSE]" 
+from 
+   "openai/text-ada-001" 
+where 
+   len(TOKENS(RESPONSE)) < 10`,
                 state: 'precomputed/hello.json'
             }, {
                 name: "👴 Tell A Joke",
                 description: "Few-Shot Samples & Constraints",
                 code: `argmax
    """A list of good dad jokes. A indicates the punchline
    Q: How does a penguin build its house?
```

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.0.6.4/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.6.4/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.6.4/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,24 @@
 export function reconstructTaggedModelResult(nodes) {
     if (nodes == null) {
         return []
     }
 
+    function unescapeBytes(s) {
+        if (s.length == 1) {
+            // unpack array
+            if (s[0].startsWith("bytes:")) {
+                return [s[0].substring(6)]
+            } else {
+                return [s]
+            }
+        }
+        return s
+    }
+
     let results = []
 
     for (let node of nodes) {
         if (node == null) {
             continue
         }
 
@@ -16,15 +28,15 @@
         let text = []
         while (n != null) {
             if (!n.data("user_data.head.variable")) {
                 return []
             }
             if (n.incomers().length > 0) {
                 text.push({
-                    text: n.data("text"),
+                    text: unescapeBytes(n.data("text")),
                     variable: n.data("deterministic") ? "__prompt__" : n.data("user_data.head.variable"),
                     pool: n.data("pool"),
                 })
             }
             let next = n;
             next.incomers().forEach(p => {
                 next = p
```

### Comparing `lmql-0.0.6.3/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.6.4/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.6.4/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.6.4/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.6.4/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.0.6.4/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/vscode/package.json` & `lmql-0.0.6.4/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/utils/docstring_parser.py` & `lmql-0.0.6.4/src/lmql/utils/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/utils/graph.py` & `lmql-0.0.6.4/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.3/src/lmql/utils/nputil.py` & `lmql-0.0.6.4/src/lmql/utils/nputil.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def ensure_array(v, dtype=None):
     if v is None: return None
     if is_array(v): return v
     else: return np.array(v, dtype=dtype)
 
 def ensure_iterable(v):
-    if type(v) is np.float32 or type(v) is np.float64 or type(v) is np.int32 or type(v) is np.int64 or type(v) is float or type(v) is int:
+    if type(v) is np.float32 or type(v) is np.float64 or type(v) is np.int32 or type(v) is np.int64 or type(v) is float or type(v) is int or type(v) is str:
         return [v]
     elif type(v) is np.ndarray:
         if v.ndim == 0:
             return [v.item()]
         else:
             return v
     elif type(v) is list:
@@ -27,15 +27,20 @@
     elif hasattr(v, "numpy"):
         return ensure_iterable(v.numpy())
     else:
         assert False, f"ensure_iterable(): type {type(v)} cannot be converted to iterable"
 
 
 def log_softmax(a):
-    return a - np.log(np.sum(np.exp(a)))
+    # check for log div by zero
+    normalizer = np.sum(np.exp(a))
+    if normalizer == 0:
+        # assign 1.0 to max value
+        return np.where(a == np.max(a), 0.0, -np.inf)
+    return a - np.log(normalizer)
 
 def topk(a, k:int, sorted: bool = False, axis=-1):
     assert k > 0, "topk(): k must be > 0"
     idx = np.argpartition(a, -k, axis=axis)[..., -k:]
     if sorted: 
         index_values = np.take_along_axis(a, idx, axis=axis)
         idx = np.take_along_axis(idx, np.argsort(index_values, axis=axis), axis=axis)
```

### Comparing `lmql-0.0.6.3/src/lmql.egg-info/PKG-INFO` & `lmql-0.0.6.4/src/lmql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -95,15 +95,15 @@
 
 > **Operating System**: The GPU-enabled version of LMQL was tested to work on Ubuntu 22.04 with CUDA 12.0 and Windows 10 via WSL2 and CUDA 11.7. The no-GPU version (see below) was tested to work on Ubuntu 22.04 and macOS 13.2 Ventura or Windows 10 via WSL2.
 
 ### Development without GPU
 
 This section outlines how to setup an LMQL development environment without local GPU support. Note that LMQL without local GPU support only supports the use of API-integrated models like `openai/text-davinci-003`. Please see the OpenAI API documentation (https://platform.openai.com/docs/models/gpt-3-5) to learn more about the set of available models.
 
-To setup a `conda` environment for LMQL with GPU support, run the following commands:
+To setup a `conda` environment for LMQL with no GPU support, run the following commands:
 
 ```
 # prepare conda environment
 conda env create -f scripts/conda/requirements-no-gpu.yml -n lmql-no-gpu
 conda activate lmql-no-gpu
 
 # registers the `lmql` command in the current shell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.3 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.4 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
@@ -53,12 +53,12 @@
 Ubuntu 22.04 with CUDA 12.0 and Windows 10 via WSL2 and CUDA 11.7. The no-GPU
 version (see below) was tested to work on Ubuntu 22.04 and macOS 13.2 Ventura
 or Windows 10 via WSL2. ### Development without GPU This section outlines how
 to setup an LMQL development environment without local GPU support. Note that
 LMQL without local GPU support only supports the use of API-integrated models
 like `openai/text-davinci-003`. Please see the OpenAI API documentation (https:
 //platform.openai.com/docs/models/gpt-3-5) to learn more about the set of
-available models. To setup a `conda` environment for LMQL with GPU support, run
-the following commands: ``` # prepare conda environment conda env create -
+available models. To setup a `conda` environment for LMQL with no GPU support,
+run the following commands: ``` # prepare conda environment conda env create -
 f scripts/conda/requirements-no-gpu.yml -n lmql-no-gpu conda activate lmql-no-
 gpu # registers the `lmql` command in the current shell source scripts/
 activate-dev.sh ```
```

### Comparing `lmql-0.0.6.3/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.6.4/src/lmql.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
-TODO.md
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
 .github/workflows/lmql-web.yml
 docs/Makefile
 docs/RELEASE.md
 docs/make.bat
 docs/requirements.txt
 docs/todo.md
 docs/source/conf.py
 docs/source/dev-setup.md
+docs/source/docker-setup.md
 docs/source/index.rst
 docs/source/installation.md
 docs/source/lmql.svg
 docs/source/logo.png
 docs/source/quickstart.md
 docs/source/_ext/lmql_snippets.py
 docs/source/_static/css/lmql-docs.css
 docs/source/_static/images/lmql.svg
 docs/source/_static/js/lmql-playground.js
 docs/source/_templates/layout.html
 docs/source/blog/release-0.0.5.md
 docs/source/blog/release-0.0.6.1.md
 docs/source/blog/release-0.0.6.3.md
 docs/source/blog/release-0.0.6.md
+docs/source/images/inference.svg
+docs/source/language/azure.md
 docs/source/language/constraints.md
 docs/source/language/decoders.md
 docs/source/language/functions.md
+docs/source/language/hf.md
 docs/source/language/models.md
+docs/source/language/openai.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
+docs/source/pending/release-next.md
 docs/source/python/.gitignore
 docs/source/python/langchain.ipynb
+docs/source/python/lc.py
 docs/source/python/llama_index.ipynb
 docs/source/python/lmql.txt
 docs/source/python/output.ipynb
 docs/source/python/pandas.ipynb
 docs/source/python/python.ipynb
 docs/source/releases/misc-snippets.md
 docs/source/releases/release-0.0.5.md
+scripts/Dockerfile
 scripts/activate-dev.sh
 scripts/pypi-release.sh
+scripts/serve-all.py
 scripts/wheel.sh
 scripts/conda/requirements-no-gpu.yml
 scripts/conda/requirements.yml
 src/lmql.svg
 src/lmql/__init__.py
 src/lmql/cli.py
 src/lmql/demo.py
@@ -57,83 +64,105 @@
 src/lmql/version.py
 src/lmql.egg-info/PKG-INFO
 src/lmql.egg-info/SOURCES.txt
 src/lmql.egg-info/dependency_links.txt
 src/lmql.egg-info/entry_points.txt
 src/lmql.egg-info/requires.txt
 src/lmql.egg-info/top_level.txt
+src/lmql/algorithms/__init__.py
+src/lmql/algorithms/cache.py
+src/lmql/algorithms/functools.py
 src/lmql/language/__init__.py
 src/lmql/language/compiler.py
 src/lmql/language/fragment_parser.py
 src/lmql/language/qstrings.py
 src/lmql/language/validator.py
-src/lmql/model/__init__.py
-src/lmql/model/async_generation_utils.py
-src/lmql/model/local_client.py
-src/lmql/model/serve.py
-src/lmql/model/served_model.py
+src/lmql/models/__init__.py
+src/lmql/models/model.py
+src/lmql/models/lmtp/README.md
+src/lmql/models/lmtp/lmtp_client.py
+src/lmql/models/lmtp/lmtp_dcmodel.py
+src/lmql/models/lmtp/lmtp_inference_server.py
+src/lmql/models/lmtp/lmtp_multiprocessing.py
+src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
+src/lmql/models/lmtp/lmtp_serve.py
+src/lmql/models/lmtp/lmtp_threading.py
+src/lmql/models/lmtp/utils.py
 src/lmql/ops/__init__.py
 src/lmql/ops/follow_map.py
 src/lmql/ops/ops.py
 src/lmql/ops/token_set.py
 src/lmql/output/__init__.py
 src/lmql/output/http.py
 src/lmql/output/sse.py
 src/lmql/output/ws.py
 src/lmql/runtime/__init__.py
 src/lmql/runtime/caching.py
-src/lmql/runtime/hf_integration.py
 src/lmql/runtime/interpreter.py
 src/lmql/runtime/interrupt.py
 src/lmql/runtime/langchain.py
 src/lmql/runtime/lmql_runtime.py
+src/lmql/runtime/loop.py
 src/lmql/runtime/maiohttp.py
 src/lmql/runtime/masks.py
 src/lmql/runtime/model_registry.py
 src/lmql/runtime/multi_head_interpretation.py
 src/lmql/runtime/openai_integration.py
 src/lmql/runtime/openai_secret.py
 src/lmql/runtime/output_writer.py
 src/lmql/runtime/program_state.py
 src/lmql/runtime/stats.py
+src/lmql/runtime/token_distribution.py
 src/lmql/runtime/tokenizer.py
 src/lmql/runtime/bopenai/__init__.py
 src/lmql/runtime/bopenai/batched_openai.py
 src/lmql/runtime/bopenai/openai_api.py
 src/lmql/runtime/dclib/__init__.py
 src/lmql/runtime/dclib/dclib_array.py
 src/lmql/runtime/dclib/dclib_cache.py
 src/lmql/runtime/dclib/dclib_global.py
 src/lmql/runtime/dclib/dclib_model.py
 src/lmql/runtime/dclib/dclib_rewrite.py
 src/lmql/runtime/dclib/dclib_seq.py
 src/lmql/runtime/dclib/decoders.py
-src/lmql/runtime/dclib/trie_cache.py
 src/lmql/runtime/postprocessing/__init__.py
 src/lmql/runtime/postprocessing/conditional_prob.py
 src/lmql/runtime/postprocessing/group_by.py
+src/lmql/runtime/tokenizers/hf_tokenizer.py
+src/lmql/runtime/tokenizers/pure_python_tokenizer.py
+src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
 src/lmql/tests/README.md
 src/lmql/tests/expr_test_utils.py
 src/lmql/tests/fin_and.py
+src/lmql/tests/local_model_python.py
 src/lmql/tests/tail_token_set.py
 src/lmql/tests/test_back2back_caching.py
 src/lmql/tests/test_eq.py
+src/lmql/tests/test_multibyte_characters.py
+src/lmql/tests/test_multibyte_local_models.py
 src/lmql/tests/test_orop.py
+src/lmql/tests/test_query_args.py
 src/lmql/tests/test_sample_queries.py
 src/lmql/tests/test_scoping.py
 src/lmql/tests/test_stopping.py
+src/lmql/tests/tiktoken_tsets.py
 src/lmql/tests/outdated/mask_product_test.py
 src/lmql/tests/outdated/monotonicity.py
 src/lmql/tests/outdated/one_of_tests.py
 src/lmql/tests/outdated/sentences_op.py
 src/lmql/tests/outdated/starts_with_op_test.py
 src/lmql/tests/outdated/stops_at.py
 src/lmql/tests/outdated/str_in_str_tests.py
 src/lmql/tests/outdated/test_multi_head.py
 src/lmql/tests/outdated/token_set_test.py
+src/lmql/tests/queryargs/test_args.py
+src/lmql/tests/queryargs/test_args_query_str.py
+src/lmql/tests/queryargs/test_args_run.py
+src/lmql/tests/queryargs/test_sync.py
+src/lmql/tests/queryargs/test_var_errors.py
 src/lmql/tests/system/basic_use_cases.py
 src/lmql/ui/.gitignore
 src/lmql/ui/__init__.py
 src/lmql/ui/live/__init__.py
 src/lmql/ui/live/live.js
 src/lmql/ui/live/live.py
 src/lmql/ui/live/livelib.py
```

### Comparing `lmql-0.0.6.3/src/lmql.svg` & `lmql-0.0.6.4/src/lmql.svg`

 * *Files identical despite different names*

