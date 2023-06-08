# Comparing `tmp/langflow-0.0.86.tar.gz` & `tmp/langflow-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-0.0.86.tar", max compression
+gzip compressed data, was "langflow-0.0.87.tar", max compression
```

## Comparing `langflow-0.0.86.tar` & `langflow-0.0.87.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1065 2023-06-08 03:48:13.331432 langflow-0.0.86/LICENSE
--rw-r--r--   0        0        0    10199 2023-06-08 03:48:13.331432 langflow-0.0.86/README.md
--rw-r--r--   0        0        0     2042 2023-06-08 03:48:13.351432 langflow-0.0.86/pyproject.toml
--rw-r--r--   0        0        0      152 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/__init__.py
--rw-r--r--   0        0        0     3851 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/__main__.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/api/__init__.py
--rw-r--r--   0        0        0     2032 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/api/base.py
--rw-r--r--   0        0        0     1124 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/api/callback.py
--rw-r--r--   0        0        0      776 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/api/chat.py
--rw-r--r--   0        0        0     8558 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/api/chat_manager.py
--rw-r--r--   0        0        0     1246 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/api/endpoints.py
--rw-r--r--   0        0        0     1443 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/api/schemas.py
--rw-r--r--   0        0        0     1765 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/api/validate.py
--rw-r--r--   0        0        0       57 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/cache/__init__.py
--rw-r--r--   0        0        0     4329 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/cache/base.py
--rw-r--r--   0        0        0     4478 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/cache/manager.py
--rw-r--r--   0        0        0     2580 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/config.yaml
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/custom/__init__.py
--rw-r--r--   0        0        0     1213 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/custom/customs.py
--rw-r--r--   0        0        0      889 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg
--rw-r--r--   0        0        0     2521 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg
--rw-r--r--   0        0        0     3513 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg
--rw-r--r--   0        0        0     1578 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg
--rw-r--r--   0        0        0     1705 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg
--rw-r--r--   0        0        0     7249 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg
--rw-r--r--   0        0        0     1106 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg
--rw-r--r--   0        0        0     2007 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg
--rw-r--r--   0        0        0     6783 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/bing-60c0c591.svg
--rw-r--r--   0        0        0      622 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/chroma-65ceac37.svg
--rw-r--r--   0        0        0     1450 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/cohere-f09153b9.svg
--rw-r--r--   0        0        0     1667 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg
--rw-r--r--   0        0        0    11568 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/froze-flow-494453cf.png
--rw-r--r--   0        0        0     1111 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg
--rw-r--r--   0        0        0      688 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/google-0cf576a5.svg
--rw-r--r--   0        0        0    35286 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg
--rw-r--r--   0        0        0      789 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg
--rw-r--r--   0        0        0  4102261 2023-06-08 03:49:15.475403 langflow-0.0.86/src/backend/langflow/frontend/assets/index-639f6f6b.js
--rw-r--r--   0        0        0    82705 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/index-c2ccece6.css
--rw-r--r--   0        0        0     2212 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg
--rw-r--r--   0        0        0     2509 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/openAI-2c85883b.svg
--rw-r--r--   0        0        0     1539 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg
--rw-r--r--   0        0        0     4310 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0   104188 2023-06-08 03:49:15.471403 langflow-0.0.86/src/backend/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      622 2023-06-08 03:49:15.475403 langflow-0.0.86/src/backend/langflow/frontend/index.html
--rw-r--r--   0        0        0      119 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/graph/__init__.py
--rw-r--r--   0        0        0    11139 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/graph/base.py
--rw-r--r--   0        0        0       72 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/graph/constants.py
--rw-r--r--   0        0        0     6217 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/graph/graph.py
--rw-r--r--   0        0        0     6444 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/graph/nodes.py
--rw-r--r--   0        0        0      420 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     1843 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/agents/base.py
--rw-r--r--   0        0        0    10017 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1447 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     2991 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     2008 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4084 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0     1979 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     5759 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1445 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0      171 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     4811 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0     1668 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1355 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/llms/base.py
--rw-r--r--   0        0        0    13821 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/loading.py
--rw-r--r--   0        0        0       88 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     1541 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/memories/base.py
--rw-r--r--   0        0        0       87 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2459 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2618 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0    10020 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     2309 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.351432 langflow-0.0.86/src/backend/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2447 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5402 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      823 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0      811 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4328 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/tools/util.py
--rw-r--r--   0        0        0     1813 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     2294 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     1640 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1813 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0       29 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/jcloud.yml
--rw-r--r--   0        0        0      362 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/lcserve.py
--rw-r--r--   0        0        0      816 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/main.py
--rw-r--r--   0        0        0      579 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/server.py
--rw-r--r--   0        0        0     2128 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/settings.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/field/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/field/base.py
--rw-r--r--   0        0        0      291 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/__init__.py
--rw-r--r--   0        0        0     6631 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/agents.py
--rw-r--r--   0        0        0     7516 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/base.py
--rw-r--r--   0        0        0     4720 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/chains.py
--rw-r--r--   0        0        0      683 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/constants.py
--rw-r--r--   0        0        0     1680 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/embeddings.py
--rw-r--r--   0        0        0     1889 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/llms.py
--rw-r--r--   0        0        0      648 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/memories.py
--rw-r--r--   0        0        0     3535 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/prompts.py
--rw-r--r--   0        0        0     2374 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/tools.py
--rw-r--r--   0        0        0      823 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/utilities.py
--rw-r--r--   0        0        0     2648 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/frontend_node/vectorstores.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/template/__init__.py
--rw-r--r--   0        0        0      819 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/template/template/base.py
--rw-r--r--   0        0        0        0 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/utils/__init__.py
--rw-r--r--   0        0        0      364 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/utils/constants.py
--rw-r--r--   0        0        0      914 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/utils/logger.py
--rw-r--r--   0        0        0     3169 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/utils/payload.py
--rw-r--r--   0        0        0    10983 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/utils/util.py
--rw-r--r--   0        0        0     5311 2023-06-08 03:48:13.355432 langflow-0.0.86/src/backend/langflow/utils/validate.py
--rw-r--r--   0        0        0    12535 1970-01-01 00:00:00.000000 langflow-0.0.86/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-08 20:12:44.563754 langflow-0.0.87/LICENSE
+-rw-r--r--   0        0        0    10199 2023-06-08 20:12:44.563754 langflow-0.0.87/README.md
+-rw-r--r--   0        0        0     2042 2023-06-08 20:12:44.579754 langflow-0.0.87/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/__init__.py
+-rw-r--r--   0        0        0     3851 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/api/__init__.py
+-rw-r--r--   0        0        0     2032 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/api/base.py
+-rw-r--r--   0        0        0     1124 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/api/callback.py
+-rw-r--r--   0        0        0      776 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/api/chat.py
+-rw-r--r--   0        0        0     8558 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/api/chat_manager.py
+-rw-r--r--   0        0        0     1246 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/api/endpoints.py
+-rw-r--r--   0        0        0     1443 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/api/schemas.py
+-rw-r--r--   0        0        0     1765 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/api/validate.py
+-rw-r--r--   0        0        0       57 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/cache/__init__.py
+-rw-r--r--   0        0        0     4329 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/cache/base.py
+-rw-r--r--   0        0        0     4478 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/cache/manager.py
+-rw-r--r--   0        0        0     2580 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/custom/__init__.py
+-rw-r--r--   0        0        0     1213 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/custom/customs.py
+-rw-r--r--   0        0        0      889 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg
+-rw-r--r--   0        0        0     2521 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg
+-rw-r--r--   0        0        0     3513 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg
+-rw-r--r--   0        0        0     1578 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg
+-rw-r--r--   0        0        0     1705 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg
+-rw-r--r--   0        0        0     7249 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg
+-rw-r--r--   0        0        0     1106 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg
+-rw-r--r--   0        0        0     2007 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg
+-rw-r--r--   0        0        0     6783 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/bing-60c0c591.svg
+-rw-r--r--   0        0        0      622 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/chroma-65ceac37.svg
+-rw-r--r--   0        0        0     1450 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/cohere-f09153b9.svg
+-rw-r--r--   0        0        0     1667 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg
+-rw-r--r--   0        0        0    11568 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/froze-flow-494453cf.png
+-rw-r--r--   0        0        0     1111 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg
+-rw-r--r--   0        0        0      688 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/google-0cf576a5.svg
+-rw-r--r--   0        0        0    35286 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg
+-rw-r--r--   0        0        0      789 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg
+-rw-r--r--   0        0        0    82705 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/index-c2ccece6.css
+-rw-r--r--   0        0        0  4102271 2023-06-08 20:13:42.220913 langflow-0.0.87/src/backend/langflow/frontend/assets/index-c5e2a1aa.js
+-rw-r--r--   0        0        0     2212 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg
+-rw-r--r--   0        0        0     2509 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/openAI-2c85883b.svg
+-rw-r--r--   0        0        0     1539 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg
+-rw-r--r--   0        0        0     4310 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0   104188 2023-06-08 20:13:42.216913 langflow-0.0.87/src/backend/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      622 2023-06-08 20:13:42.220913 langflow-0.0.87/src/backend/langflow/frontend/index.html
+-rw-r--r--   0        0        0      119 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/graph/__init__.py
+-rw-r--r--   0        0        0    11139 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/graph/base.py
+-rw-r--r--   0        0        0       72 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/graph/constants.py
+-rw-r--r--   0        0        0     6217 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/graph/graph.py
+-rw-r--r--   0        0        0     6444 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/graph/nodes.py
+-rw-r--r--   0        0        0      420 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/agents/__init__.py
+-rw-r--r--   0        0        0     1843 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/agents/base.py
+-rw-r--r--   0        0        0    10017 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/agents/custom.py
+-rw-r--r--   0        0        0     1447 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/agents/prebuilt.py
+-rw-r--r--   0        0        0     2991 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/base.py
+-rw-r--r--   0        0        0       84 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/chains/__init__.py
+-rw-r--r--   0        0        0     2008 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/chains/base.py
+-rw-r--r--   0        0        0     4084 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/chains/custom.py
+-rw-r--r--   0        0        0     1979 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/custom_lists.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/document_loaders/__init__.py
+-rw-r--r--   0        0        0     5759 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/document_loaders/base.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/embeddings/__init__.py
+-rw-r--r--   0        0        0     1445 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/embeddings/base.py
+-rw-r--r--   0        0        0      171 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0     4811 2023-06-08 20:12:44.579754 langflow-0.0.87/src/backend/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0     1668 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/listing.py
+-rw-r--r--   0        0        0       78 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/llms/__init__.py
+-rw-r--r--   0        0        0     1355 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/llms/base.py
+-rw-r--r--   0        0        0    13821 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/loading.py
+-rw-r--r--   0        0        0       88 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/memories/__init__.py
+-rw-r--r--   0        0        0     1541 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/memories/base.py
+-rw-r--r--   0        0        0       87 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/prompts/__init__.py
+-rw-r--r--   0        0        0     2459 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/prompts/base.py
+-rw-r--r--   0        0        0     2618 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/prompts/custom.py
+-rw-r--r--   0        0        0    10020 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/run.py
+-rw-r--r--   0        0        0      106 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/text_splitters/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/text_splitters/base.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/toolkits/__init__.py
+-rw-r--r--   0        0        0     2447 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/toolkits/custom.py
+-rw-r--r--   0        0        0       81 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/tools/__init__.py
+-rw-r--r--   0        0        0     5402 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/tools/base.py
+-rw-r--r--   0        0        0      823 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/tools/constants.py
+-rw-r--r--   0        0        0      811 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/tools/custom.py
+-rw-r--r--   0        0        0     4328 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/tools/util.py
+-rw-r--r--   0        0        0     1813 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/types.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/utilities/__init__.py
+-rw-r--r--   0        0        0     2294 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/utilities/base.py
+-rw-r--r--   0        0        0     1640 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/vector_store/__init__.py
+-rw-r--r--   0        0        0     1813 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/vector_store/base.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/wrappers/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/interface/wrappers/base.py
+-rw-r--r--   0        0        0       29 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/jcloud.yml
+-rw-r--r--   0        0        0      362 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/lcserve.py
+-rw-r--r--   0        0        0      816 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/main.py
+-rw-r--r--   0        0        0      579 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/server.py
+-rw-r--r--   0        0        0     2128 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/settings.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/field/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/field/base.py
+-rw-r--r--   0        0        0      291 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/__init__.py
+-rw-r--r--   0        0        0     6631 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/agents.py
+-rw-r--r--   0        0        0     7516 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/base.py
+-rw-r--r--   0        0        0     4720 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/chains.py
+-rw-r--r--   0        0        0      683 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/constants.py
+-rw-r--r--   0        0        0     1680 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/embeddings.py
+-rw-r--r--   0        0        0     1889 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/llms.py
+-rw-r--r--   0        0        0      648 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/memories.py
+-rw-r--r--   0        0        0     3535 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/prompts.py
+-rw-r--r--   0        0        0     2374 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/tools.py
+-rw-r--r--   0        0        0      823 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/utilities.py
+-rw-r--r--   0        0        0     2648 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/frontend_node/vectorstores.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/template/__init__.py
+-rw-r--r--   0        0        0      819 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/template/template/base.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/utils/__init__.py
+-rw-r--r--   0        0        0      364 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/utils/constants.py
+-rw-r--r--   0        0        0      914 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3169 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/utils/payload.py
+-rw-r--r--   0        0        0    10983 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/utils/util.py
+-rw-r--r--   0        0        0     5311 2023-06-08 20:12:44.583754 langflow-0.0.87/src/backend/langflow/utils/validate.py
+-rw-r--r--   0        0        0    12535 1970-01-01 00:00:00.000000 langflow-0.0.87/PKG-INFO
```

### Comparing `langflow-0.0.86/LICENSE` & `langflow-0.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/README.md` & `langflow-0.0.87/README.md`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/pyproject.toml` & `langflow-0.0.87/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "0.0.86"
+version = "0.0.87"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Ibis Prevedello <ibiscp@gmail.com>",
     "Lucas Eduoli <lucaseduoli@gmail.com>",
     "Otávio Anovazzi <otavio2204@gmail.com>",
```

### Comparing `langflow-0.0.86/src/backend/langflow/__main__.py` & `langflow-0.0.87/src/backend/langflow/__main__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/api/base.py` & `langflow-0.0.87/src/backend/langflow/api/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/api/callback.py` & `langflow-0.0.87/src/backend/langflow/api/callback.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/api/chat.py` & `langflow-0.0.87/src/backend/langflow/api/chat.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/api/chat_manager.py` & `langflow-0.0.87/src/backend/langflow/api/chat_manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/api/endpoints.py` & `langflow-0.0.87/src/backend/langflow/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/api/schemas.py` & `langflow-0.0.87/src/backend/langflow/api/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/api/validate.py` & `langflow-0.0.87/src/backend/langflow/api/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/cache/base.py` & `langflow-0.0.87/src/backend/langflow/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/cache/manager.py` & `langflow-0.0.87/src/backend/langflow/cache/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/config.yaml` & `langflow-0.0.87/src/backend/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/custom/customs.py` & `langflow-0.0.87/src/backend/langflow/custom/customs.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/bing-60c0c591.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/bing-60c0c591.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/chroma-65ceac37.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/chroma-65ceac37.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/cohere-f09153b9.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/cohere-f09153b9.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/froze-flow-494453cf.png` & `langflow-0.0.87/src/backend/langflow/frontend/assets/froze-flow-494453cf.png`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/google-0cf576a5.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/google-0cf576a5.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/index-639f6f6b.js` & `langflow-0.0.87/src/backend/langflow/frontend/assets/index-c5e2a1aa.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -26903,23 +26903,23 @@
         })))
     }
     R.useEffect(() => {
         let S = window.localStorage.getItem("tabsData");
         if (S && Object.keys(u).length > 0) {
             let _ = JSON.parse(S);
             _.flows.forEach(A => {
-                A.data.edges.forEach(L => {
+                A.data && (A.data.edges.forEach(L => {
                     L.className = "", L.style = {
                         stroke: "#555555"
                     }
                 }), A.data.nodes.forEach(L => {
                     Object.keys(u[L.data.type].template).length > 0 && (L.data.node.base_classes = u[L.data.type].base_classes, A.data.edges.forEach(C => {
                         C.source === L.id && (C.sourceHandle = C.sourceHandle.split("|").slice(0, 2).concat(u[L.data.type].base_classes).join("|"))
                     }), L.data.node.description = u[L.data.type].description, L.data.node.template = _D(u[L.data.type].template, L.data.node.template))
-                })
+                }))
             }), r(_.tabIndex), o(_.flows), s(_.id)
         }
     }, [u]), R.useEffect(() => {
         console.log(a), f()
     }, [i, a, n, l]);
 
     function h() {
```

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/index-c2ccece6.css` & `langflow-0.0.87/src/backend/langflow/frontend/assets/index-c2ccece6.css`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/openAI-2c85883b.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/openAI-2c85883b.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg` & `langflow-0.0.87/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow-0.0.87/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/favicon.ico` & `langflow-0.0.87/src/backend/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/frontend/index.html` & `langflow-0.0.87/src/backend/langflow/frontend/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <link rel="icon" href="/favicon.ico" />
     <title>LangFlow</title>
-  <script type="module" crossorigin src="/assets/index-639f6f6b.js"></script>
+  <script type="module" crossorigin src="/assets/index-c5e2a1aa.js"></script>
   <link rel="stylesheet" href="/assets/index-c2ccece6.css">
 </head>
 <body id='body' style="width: 100%; height:100%">
     <noscript>You need to enable JavaScript to run this app.</noscript>
     <div style="width: 100vw; height:100vh" id='root'></div>
     
 </body>
```

### Comparing `langflow-0.0.86/src/backend/langflow/graph/base.py` & `langflow-0.0.87/src/backend/langflow/graph/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/graph/graph.py` & `langflow-0.0.87/src/backend/langflow/graph/graph.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/graph/nodes.py` & `langflow-0.0.87/src/backend/langflow/graph/nodes.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/agents/base.py` & `langflow-0.0.87/src/backend/langflow/interface/agents/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/agents/custom.py` & `langflow-0.0.87/src/backend/langflow/interface/agents/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/agents/prebuilt.py` & `langflow-0.0.87/src/backend/langflow/interface/agents/prebuilt.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/base.py` & `langflow-0.0.87/src/backend/langflow/interface/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/chains/base.py` & `langflow-0.0.87/src/backend/langflow/interface/chains/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/chains/custom.py` & `langflow-0.0.87/src/backend/langflow/interface/chains/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/custom_lists.py` & `langflow-0.0.87/src/backend/langflow/interface/custom_lists.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/document_loaders/base.py` & `langflow-0.0.87/src/backend/langflow/interface/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/embeddings/base.py` & `langflow-0.0.87/src/backend/langflow/interface/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/importing/utils.py` & `langflow-0.0.87/src/backend/langflow/interface/importing/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/listing.py` & `langflow-0.0.87/src/backend/langflow/interface/listing.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/llms/base.py` & `langflow-0.0.87/src/backend/langflow/interface/llms/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/loading.py` & `langflow-0.0.87/src/backend/langflow/interface/loading.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/memories/base.py` & `langflow-0.0.87/src/backend/langflow/interface/memories/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/prompts/base.py` & `langflow-0.0.87/src/backend/langflow/interface/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/prompts/custom.py` & `langflow-0.0.87/src/backend/langflow/interface/prompts/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/run.py` & `langflow-0.0.87/src/backend/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/text_splitters/base.py` & `langflow-0.0.87/src/backend/langflow/interface/text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/toolkits/base.py` & `langflow-0.0.87/src/backend/langflow/interface/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/tools/base.py` & `langflow-0.0.87/src/backend/langflow/interface/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/tools/constants.py` & `langflow-0.0.87/src/backend/langflow/interface/tools/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/tools/custom.py` & `langflow-0.0.87/src/backend/langflow/interface/tools/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/tools/util.py` & `langflow-0.0.87/src/backend/langflow/interface/tools/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/types.py` & `langflow-0.0.87/src/backend/langflow/interface/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/utilities/base.py` & `langflow-0.0.87/src/backend/langflow/interface/utilities/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/utils.py` & `langflow-0.0.87/src/backend/langflow/interface/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/vector_store/base.py` & `langflow-0.0.87/src/backend/langflow/interface/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/interface/wrappers/base.py` & `langflow-0.0.87/src/backend/langflow/interface/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/main.py` & `langflow-0.0.87/src/backend/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/server.py` & `langflow-0.0.87/src/backend/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/settings.py` & `langflow-0.0.87/src/backend/langflow/settings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/field/base.py` & `langflow-0.0.87/src/backend/langflow/template/field/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/agents.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/agents.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/base.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/chains.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/chains.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/constants.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/embeddings.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/embeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/llms.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/llms.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/memories.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/memories.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/prompts.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/prompts.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/tools.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/tools.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/utilities.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/utilities.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/frontend_node/vectorstores.py` & `langflow-0.0.87/src/backend/langflow/template/frontend_node/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/template/template/base.py` & `langflow-0.0.87/src/backend/langflow/template/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/utils/logger.py` & `langflow-0.0.87/src/backend/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/utils/payload.py` & `langflow-0.0.87/src/backend/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/utils/util.py` & `langflow-0.0.87/src/backend/langflow/utils/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/src/backend/langflow/utils/validate.py` & `langflow-0.0.87/src/backend/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.86/PKG-INFO` & `langflow-0.0.87/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 0.0.86
+Version: 0.0.87
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Gabriel Almeida
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langflow Version: 0.0.86 Summary: A Python package
+Metadata-Version: 2.1 Name: langflow Version: 0.0.87 Summary: A Python package
 with a built-in web application Home-page: https://github.com/logspace-ai/
 langflow License: MIT Keywords: nlp,langchain,openai,gpt,gui Author: Logspace
 Author-email: contact@logspace.ai Maintainer: Gabriel Almeida Maintainer-email:
 gabriel@logspace.ai Requires-Python: >=3.9,<3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

