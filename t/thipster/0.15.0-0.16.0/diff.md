# Comparing `tmp/thipster-0.15.0.tar.gz` & `tmp/thipster-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.15.0.tar", last modified: Wed Jun  7 15:19:35 2023, max compression
+gzip compressed data, was "thipster-0.16.0.tar", last modified: Thu Jun  8 15:18:49 2023, max compression
```

## Comparing `thipster-0.15.0.tar` & `thipster-0.16.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-07 15:19:32.000000 thipster-0.15.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-07 15:19:32.000000 thipster-0.15.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4003 2023-06-07 15:19:35.599076 thipster-0.15.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3390 2023-06-07 15:19:32.000000 thipster-0.15.0/README.md
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-07 15:19:32.000000 thipster-0.15.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-07 15:19:32.000000 thipster-0.15.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 15:19:35.599076 thipster-0.15.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1372 2023-06-07 15:19:32.000000 thipster-0.15.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.591076 thipster-0.15.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.591076 thipster-0.15.0/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.591076 thipster-0.15.0/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15548 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     6934 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4125 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10326 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13708 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17264 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    19125 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2254 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6275 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19903 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4003 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.810503 thipster-0.16.0/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-08 15:18:45.000000 thipster-0.16.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-08 15:18:45.000000 thipster-0.16.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-06-08 15:18:49.810503 thipster-0.16.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-06-08 15:18:45.000000 thipster-0.16.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-08 15:18:45.000000 thipster-0.16.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-08 15:18:45.000000 thipster-0.16.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 15:18:49.810503 thipster-0.16.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-08 15:18:46.000000 thipster-0.16.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15548 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     6952 2023-06-08 15:18:45.000000 thipster-0.16.0/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.802502 thipster-0.16.0/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.806502 thipster-0.16.0/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.806502 thipster-0.16.0/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.806502 thipster-0.16.0/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.810503 thipster-0.16.0/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13708 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17264 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    19125 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.810503 thipster-0.16.0/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.810503 thipster-0.16.0/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20189 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-06-08 15:18:45.000000 thipster-0.16.0/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 15:18:49.806502 thipster-0.16.0/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 15:18:49.000000 thipster-0.16.0/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.15.0/LICENSE` & `thipster-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/PKG-INFO` & `thipster-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.15.0
+Version: 0.16.0
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.15.0/README.md` & `thipster-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/pyproject.toml` & `thipster-0.16.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/setup.py` & `thipster-0.16.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.15.0'
+__version__ = '0.16.0'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
```

### Comparing `thipster-0.15.0/tests/engine/test_engine.py` & `thipster-0.16.0/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.16.0/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/tests/parser/dsl_parser/test_ast.py` & `thipster-0.16.0/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.16.0/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/tests/parser/dsl_parser/test_token.py` & `thipster-0.16.0/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.16.0/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/tests/parser/test_ParserFactory.py` & `thipster-0.16.0/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/tests/parser/test_YAMLParser.py` & `thipster-0.16.0/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/tests/parser/test_parsedfile.py` & `thipster-0.16.0/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/tests/test_e2e.py` & `thipster-0.16.0/tests/test_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,19 +210,20 @@
 
 subnetwork lb-subnet:
 \tnetwork: lb-net
 \tregion: europe-west1b
 \tip_range: 10.0.1.0/24
 
 loadbalancer my-lb:
+\tnetwork: lb-net
 \tload_balancing_scheme: EXTERNAL
     """,
     )
 
-    assert_number_of_resource_type_is('google_compute_network', 3)
+    assert_number_of_resource_type_is('google_compute_network', 1)
     assert_resource_created('google_compute_network', 'lb-net')
 
     assert_number_of_resource_type_is('google_compute_subnetwork', 1)
     assert_resource_created('google_compute_subnetwork', 'lb-subnet')
 
 
 def test_internal_object():
```

### Comparing `thipster-0.15.0/thipster/auth/google.py` & `thipster-0.16.0/thipster/auth/google.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from thipster.engine import I_Auth
 
 
 class GoogleAuth(I_Auth):
     """Authenticate to Google Cloud Platform (GCP) projects
 
-    To use this module, you need to have a GCP account and a project created. 
+    To use this module, you need to have a GCP account and a project created.
     You also need to have gcloud installed : https://cloud.google.com/sdk/docs/install
     Then login using glcloud : gcloud auth application-default login
     """
 
     def __init__(self) -> None:
         return GoogleAuth
```

### Comparing `thipster-0.15.0/thipster/engine/engine.py` & `thipster-0.16.0/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/engine/i_parser.py` & `thipster-0.16.0/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/engine/i_repository.py` & `thipster-0.16.0/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/engine/i_terraform.py` & `thipster-0.16.0/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/engine/parsed_file.py` & `thipster-0.16.0/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/engine/resource_model.py` & `thipster-0.16.0/thipster/engine/resource_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         self.__optional = optional
         self.__is_list = is_list
 
     @property
     def default(self):
         return self.__default.value if self.__default else None
 
+    @default.setter
+    def default(self, value):
+        self.__default = value
+
     @property
     def cdk_name(self):
         return self.__cdk_name
 
     @property
     def optional(self):
         return self.__optional
```

### Comparing `thipster-0.15.0/thipster/parser/dsl_parser/ast.py` & `thipster-0.16.0/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.16.0/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.16.0/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/parser/dsl_parser/lexer.py` & `thipster-0.16.0/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.16.0/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/parser/dsl_parser/parser.py` & `thipster-0.16.0/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/parser/dsl_parser/token.py` & `thipster-0.16.0/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.16.0/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/parser/parser_factory.py` & `thipster-0.16.0/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/parser/yaml_parser.py` & `thipster-0.16.0/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/repository/github.py` & `thipster-0.16.0/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/repository/json.py` & `thipster-0.16.0/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster/terraform/cdk.py` & `thipster-0.16.0/thipster/terraform/cdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 class CDK(I_Terraform):
     _models = []
     _parent_resources_stack = []
     _imported_packages = []
 
+    _inherited_attributes: list[pf.ParsedAttribute] = []
     _created_resources = {}
     _logger = Logger(__name__)
 
     def apply(self, plan_file_path: str | None = None):
         """Applies generated Terraform plan
 
         Parameters
@@ -204,16 +205,31 @@
                 CDK._parent_resources_stack,
             )
 
         CDK._parent_resources_stack.append(resource_type)
 
         model = CDK._models[resource_type]
 
-        # Checks that all attributes are optional
-        if no_modif and not all(map(lambda x: x.optional, model.attributes.values())):
+        attributes = copy.deepcopy(model.attributes)
+
+        for a in CDK._inherited_attributes:
+            if a.name in attributes.keys():
+                attributes[a.name].default = rm.Model_Literal(a.value)
+
+            else:
+                attributes[a.name] = rm.Model_Attribute(
+                    cdk_name=a.name,
+                    default=rm.Model_Literal(a.value),
+                )
+
+        # Checks that all attributes have a default value
+        if (
+            no_modif
+            and not all(map(lambda x: x.default is not None, attributes.values()))
+        ):
             raise cdk_exceptions.CDKMissingAttributeInDependency(resource_type)
 
         # Import package and class
         CDK._pip_install(model.cdk_provider)
         resource_class = CDK._import(
             model.cdk_provider, model.cdk_module, model.cdk_name,
         )
@@ -222,22 +238,32 @@
         dependencies = copy.deepcopy(model.dependencies)
         resource_args = {}
 
         name = f'{parent_name}-{uuid.uuid4()}'
         if model.name_key:
             resource_args[model.name_key] = name
 
-        for _, v in model.attributes.items():
-            resource_args[v.cdk_name] = v.default
+        for attribute_name, attribute_value in attributes.items():
+
+            if not no_dependencies and attribute_name in dependencies:
+
+                CDK._check_explicit_dependency(
+                    self, resource_args, dependencies[attribute_name]['resource'],
+                    attribute_value.default, attribute_name,
+                )
+
+                del dependencies[attribute_name]
+
+            if attribute_name in model.attributes:
+                resource_args[attribute_value.cdk_name] = attribute_value.default
 
         # Create default defendencies if needed
         if not no_dependencies:
             CDK._generate_default_dependencies(
-                self, dependencies,
-                model, resource_args, name,
+                self, dependencies, model, resource_args, parent_name,
             )
 
         CDK._logger.debug('Created default %s named %s', resource_class, name)
 
         return (resource_class, name, resource_args)
 
     def _create_resource(self, resource_args: object, resource_type: str = None):
@@ -253,16 +279,14 @@
             type of the resource to create, default None
 
         Returns
         -------
         object :
             the created resource
         """
-        if isinstance(resource_args, dict):
-            return CDK._create_resource_from_dict(self, resource_type, resource_args)
 
         if isinstance(resource_args, pf.ParsedResource):
             return CDK._create_resource_from_resource(self, resource_args)
 
         return CDK._create_resource_from_args(self, resource_type, resource_args)
 
     def _create_resource_from_args(
@@ -290,82 +314,36 @@
             no_modif=False,
             no_dependencies=True,
         )
         model = CDK._models[resource_type]
 
         # Process attributes
         dependencies = copy.deepcopy(model.dependencies)
-        for attribute in input_args:
-            if attribute.name and model.name_key:
-                resource_args[model.name_key] = attribute.name
-
-            CDK._process_attribute(
-                self, model, attribute, resource_args, dependencies,
-            )
-
-        CDK._generate_default_dependencies(
-            self, dependencies, model, resource_args, resource_name,
-        )
-
-        # Create resource
-        CDK._parent_resources_stack.remove(resource_type)
-
-        CDK._logger.debug(
-            'Created default %s named %s',
-            resource_class, resource_name,
-        )
 
-        if not model.name_key:
-            return resource_class(**resource_args)
-        return resource_class(self, resource_name, **resource_args)
+        def attributes(attribute_list):
+            for attribute in attribute_list:
+                if attribute.name and model.name_key:
+                    resource_args[model.name_key] = attribute.name
 
-    def _create_resource_from_dict(
-        self, resource_type: str, input_args: dict | None,
-    ):
-        """Create a resource from a dictionnary
-
-        Parameters
-        ----------
-        self : _ResourceStack
-            Terraform CDK stack that contains the resource
-        resource_type : str, optional
-            type of the resource to create, default None
-        input_args : dict
-            data source to create the resource
-
-        Returns
-        -------
-        object :
-            the created resource
-        """
-        resource_class, resource_name, resource_args = CDK._create_default_resource(
-            self,
-            resource_type,
-            no_modif=False,
-            no_dependencies=True,
-        )
-        model = CDK._models[resource_type]
+                CDK._process_attribute(
+                    self, model, attribute, resource_args, dependencies,
+                )
 
-        # Process attributes
-        dependencies = copy.deepcopy(model.dependencies)
-        for name, value in input_args.items():
-            if name and model.name_key:
-                resource_args[model.name_key] = name
-
-            CDK._process_attribute(
-                self, model,
-                pf.ParsedAttribute(
-                    name, None, pf.ParsedLiteral(value),
-                ),
-                resource_args, dependencies,
-            )
+        attributes(input_args)
+        attributes(CDK._inherited_attributes)
 
+        CDK._inherited_attributes += input_args
         CDK._generate_default_dependencies(
             self, dependencies, model, resource_args, resource_name,
         )
+        CDK._inherited_attributes = CDK._inherited_attributes[
+            :-len(
+                input_args,
+            )
+        ]
 
         # Create resource
         CDK._parent_resources_stack.remove(resource_type)
 
         CDK._logger.debug(
             'Created default %s named %s',
             resource_class, resource_name,
@@ -400,26 +378,37 @@
         model = CDK._models[resource.type]
 
         if model.name_key:
             resource_args[model.name_key] = resource.name
 
         # Process attributes
         dependencies = copy.deepcopy(model.dependencies)
-        for attribute in resource.attributes:
-            CDK._process_attribute(
-                self,
-                model,
-                attribute,
-                resource_args,
-                dependencies,
-            )
 
+        def attributes(attribute_list):
+            for attribute in attribute_list:
+                CDK._process_attribute(
+                    self,
+                    model,
+                    attribute,
+                    resource_args,
+                    dependencies,
+                )
+
+        attributes(resource.attributes)
+        attributes(CDK._inherited_attributes)
+
+        CDK._inherited_attributes += resource.attributes
         CDK._generate_default_dependencies(
             self, dependencies, model, resource_args, resource.name,
         )
+        CDK._inherited_attributes = CDK._inherited_attributes[
+            :-len(
+                resource.attributes,
+            )
+        ]
 
         # Create resource
         CDK._parent_resources_stack.remove(resource.type)
 
         CDK._logger.debug(
             'Created resource %s named %s',
             resource_class, resource.name,
@@ -446,33 +435,18 @@
             attribute to handle
         resource_args : object
             data source needed to create the resource
         dependencies : dict[str, dict[str, object]]
             dependencies needed to create the resource
         """
         if attribute.name in dependencies:
-            created_name = f"{dependencies[attribute.name]['resource']}/"\
-                           f'{attribute.value}'
-
-            # Checks if attribute is an explicit dependency
-            if created_name not in CDK._created_resources.keys():
-
-                if isinstance(attribute.value, str):
-                    raise cdk_exceptions.CDKDependencyNotDeclared(
-                        attribute.name, attribute.value,
-                    )
-
-                # Creates explicit dependency
-                CDK._create_dependency(
-                    self, attribute.name, attribute.value,
-                    resource_args, attribute.name,
-                )
-
-            resource_args[attribute.name] = CDK._created_resources[created_name]
-
+            CDK._check_explicit_dependency(
+                self, resource_args, dependencies[attribute.name]['resource'],
+                attribute.value, attribute.name,
+            )
             del dependencies[attribute.name]
             return
 
         # Checks if attribute is an internal object
         if attribute.name in model.internal_objects:
             resource_args = CDK._create_internal_object(
                 self,
@@ -481,17 +455,15 @@
                 attribute.value,
                 resource_args,
             )
             return
 
         # Checks if attribute is expected as an attibute
         if attribute.name not in model.attributes:
-            raise cdk_exceptions.CDKInvalidAttribute(
-                attribute.name, model.type,
-            )
+            return
 
         # Processes list attribute
         attribute_value = attribute.value
         if model.attributes[attribute.name].is_list:
             if type(attribute.value) is list:
                 attribute_value = [i.value for i in attribute.value]
             else:
@@ -527,15 +499,25 @@
             CDK._create_dependency(
                 self, dependency_name, dependency_object, resource_args, resource_name,
             )
 
         # Create default internal objects if needed
         for internal_object_name, internal_object in model.internal_objects.items():
             if internal_object_name not in resource_args:
-                for default_args in internal_object['defaults']:
+                for default_args_json in internal_object['defaults']:
+
+                    # Transform in list of ParsedAttributes
+                    default_args = []
+                    for arg_key, arg_value in default_args_json.items():
+                        default_args.append(
+                            pf.ParsedAttribute(
+                                arg_key, None, pf.ParsedLiteral(arg_value),
+                            ),
+                        )
+
                     CDK._create_internal_object(
                         self,
                         internal_object_name,
                         model.internal_objects[internal_object_name],
                         default_args,
                         resource_args,
                     )
@@ -620,7 +602,29 @@
         )
 
         id = class_(self, class_name, **class_attributes).id
         if dep_name:
             resource_args[dep_name] = id
 
         CDK._parent_resources_stack.remove(dep_value['resource'])
+
+    def _check_explicit_dependency(
+        self, resource_args, dependency_type, dependency_value, attribute_name,
+    ):
+        created_name = f'{dependency_type}/'\
+            f'{dependency_value}'
+
+        # Checks if attribute is an explicit dependency
+        if created_name not in CDK._created_resources.keys():
+
+            if isinstance(dependency_value, str):
+                raise cdk_exceptions.CDKDependencyNotDeclared(
+                    attribute_name, dependency_value,
+                )
+
+            # Creates explicit dependency
+            CDK._create_dependency(
+                self, attribute_name, dependency_value,
+                resource_args, attribute_name,
+            )
+
+        resource_args[attribute_name] = CDK._created_resources[created_name]
```

### Comparing `thipster-0.15.0/thipster/terraform/exceptions.py` & `thipster-0.16.0/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.15.0/thipster.egg-info/PKG-INFO` & `thipster-0.16.0/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.15.0
+Version: 0.16.0
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.15.0/thipster.egg-info/SOURCES.txt` & `thipster-0.16.0/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

