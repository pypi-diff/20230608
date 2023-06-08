# Comparing `tmp/flama-1.3.0.tar.gz` & `tmp/flama-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flama-1.3.0.tar", max compression
+gzip compressed data, was "flama-1.4.0.tar", max compression
```

## Comparing `flama-1.3.0.tar` & `flama-1.4.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0    11393 2023-03-17 19:17:51.766032 flama-1.3.0/LICENSE
--rw-r--r--   0        0        0     4288 2023-03-17 19:17:51.766032 flama-1.3.0/README.md
--rw-r--r--   0        0        0      406 2023-03-17 19:17:51.766032 flama-1.3.0/flama/__init__.py
--rw-r--r--   0        0        0    12437 2023-03-17 19:17:51.766032 flama-1.3.0/flama/applications.py
--rw-r--r--   0        0        0     2820 2023-03-17 19:17:51.766032 flama-1.3.0/flama/asgi.py
--rw-r--r--   0        0        0      404 2023-03-17 19:17:51.766032 flama-1.3.0/flama/authentication.py
--rw-r--r--   0        0        0     2998 2023-03-17 19:17:51.766032 flama-1.3.0/flama/background.py
--rw-r--r--   0        0        0      149 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/__init__.py
--rw-r--r--   0        0        0      689 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/__main__.py
--rw-r--r--   0        0        0        0 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/commands/__init__.py
--rw-r--r--   0        0        0     3660 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/commands/model.py
--rw-r--r--   0        0        0      829 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/commands/run.py
--rw-r--r--   0        0        0      734 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/commands/serve.py
--rw-r--r--   0        0        0     1044 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/commands/start.py
--rw-r--r--   0        0        0        0 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/config/__init__.py
--rw-r--r--   0        0        0     5201 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/config/app.py
--rw-r--r--   0        0        0     2595 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/config/config.py
--rw-r--r--   0        0        0    16250 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/config/uvicorn.py
--rw-r--r--   0        0        0      363 2023-03-17 19:17:51.766032 flama-1.3.0/flama/cli/templates/app.py.j2
--rw-r--r--   0        0        0      126 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/__init__.py
--rw-r--r--   0        0        0      713 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/base.py
--rw-r--r--   0        0        0      189 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/http/__init__.py
--rw-r--r--   0        0        0      485 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/http/jsondata.py
--rw-r--r--   0        0        0      260 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/http/multipart.py
--rw-r--r--   0        0        0      284 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/http/urlencoded.py
--rw-r--r--   0        0        0      207 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/websockets/__init__.py
--rw-r--r--   0        0        0      433 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/websockets/bytes.py
--rw-r--r--   0        0        0      606 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/websockets/json.py
--rw-r--r--   0        0        0      427 2023-03-17 19:17:51.766032 flama-1.3.0/flama/codecs/websockets/text.py
--rw-r--r--   0        0        0     1488 2023-03-17 19:17:51.766032 flama-1.3.0/flama/concurrency.py
--rw-r--r--   0        0        0        0 2023-03-17 19:17:51.766032 flama-1.3.0/flama/debug/__init__.py
--rw-r--r--   0        0        0     5551 2023-03-17 19:17:51.766032 flama-1.3.0/flama/debug/data_structures.py
--rw-r--r--   0        0        0     7911 2023-03-17 19:17:51.766032 flama-1.3.0/flama/debug/middleware.py
--rw-r--r--   0        0        0      350 2023-03-17 19:17:51.766032 flama-1.3.0/flama/debug/types.py
--rw-r--r--   0        0        0     5935 2023-03-17 19:17:51.770032 flama-1.3.0/flama/endpoints.py
--rw-r--r--   0        0        0     1000 2023-03-17 19:17:51.770032 flama-1.3.0/flama/events.py
--rw-r--r--   0        0        0     3904 2023-03-17 19:17:51.770032 flama-1.3.0/flama/exceptions.py
--rw-r--r--   0        0        0     7114 2023-03-17 19:17:51.770032 flama-1.3.0/flama/http.py
--rw-r--r--   0        0        0      192 2023-03-17 19:17:51.770032 flama-1.3.0/flama/injection/__init__.py
--rw-r--r--   0        0        0     3708 2023-03-17 19:17:51.770032 flama-1.3.0/flama/injection/components.py
--rw-r--r--   0        0        0      800 2023-03-17 19:17:51.770032 flama-1.3.0/flama/injection/exceptions.py
--rw-r--r--   0        0        0     2591 2023-03-17 19:17:51.770032 flama-1.3.0/flama/injection/injector.py
--rw-r--r--   0        0        0     7324 2023-03-17 19:17:51.770032 flama-1.3.0/flama/injection/resolver.py
--rw-r--r--   0        0        0      144 2023-03-17 19:17:51.770032 flama-1.3.0/flama/injection/types.py
--rw-r--r--   0        0        0     2105 2023-03-17 19:17:51.770032 flama-1.3.0/flama/lifespan.py
--rw-r--r--   0        0        0     3425 2023-03-17 19:17:51.770032 flama-1.3.0/flama/middleware.py
--rw-r--r--   0        0        0      173 2023-03-17 19:17:51.770032 flama-1.3.0/flama/models/__init__.py
--rw-r--r--   0        0        0      508 2023-03-17 19:17:51.770032 flama-1.3.0/flama/models/base.py
--rw-r--r--   0        0        0     1736 2023-03-17 19:17:51.770032 flama-1.3.0/flama/models/components.py
--rw-r--r--   0        0        0        0 2023-03-17 19:17:51.770032 flama-1.3.0/flama/models/models/__init__.py
--rw-r--r--   0        0        0      526 2023-03-17 19:17:51.770032 flama-1.3.0/flama/models/models/pytorch.py
--rw-r--r--   0        0        0      342 2023-03-17 19:17:51.770032 flama-1.3.0/flama/models/models/sklearn.py
--rw-r--r--   0        0        0      555 2023-03-17 19:17:51.770032 flama-1.3.0/flama/models/models/tensorflow.py
--rw-r--r--   0        0        0     1856 2023-03-17 19:17:51.770032 flama-1.3.0/flama/models/modules.py
--rw-r--r--   0        0        0     4513 2023-03-17 19:17:51.770032 flama-1.3.0/flama/models/resource.py
--rw-r--r--   0        0        0     1568 2023-03-17 19:17:51.770032 flama-1.3.0/flama/modules.py
--rw-r--r--   0        0        0     1660 2023-03-17 19:17:51.770032 flama-1.3.0/flama/negotiation.py
--rw-r--r--   0        0        0      271 2023-03-17 19:17:51.770032 flama-1.3.0/flama/pagination/__init__.py
--rw-r--r--   0        0        0     4800 2023-03-17 19:17:51.770032 flama-1.3.0/flama/pagination/limit_offset.py
--rw-r--r--   0        0        0     5065 2023-03-17 19:17:51.770032 flama-1.3.0/flama/pagination/page_number.py
--rw-r--r--   0        0        0        0 2023-03-17 19:17:51.770032 flama-1.3.0/flama/py.typed
--rw-r--r--   0        0        0      139 2023-03-17 19:17:51.770032 flama-1.3.0/flama/resources/__init__.py
--rw-r--r--   0        0        0    10859 2023-03-17 19:17:51.770032 flama-1.3.0/flama/resources/crud.py
--rw-r--r--   0        0        0     1325 2023-03-17 19:17:51.770032 flama-1.3.0/flama/resources/data_structures.py
--rw-r--r--   0        0        0      704 2023-03-17 19:17:51.770032 flama-1.3.0/flama/resources/exceptions.py
--rw-r--r--   0        0        0     1237 2023-03-17 19:17:51.770032 flama-1.3.0/flama/resources/modules.py
--rw-r--r--   0        0        0     5219 2023-03-17 19:17:51.770032 flama-1.3.0/flama/resources/resource.py
--rw-r--r--   0        0        0     5345 2023-03-17 19:17:51.770032 flama-1.3.0/flama/resources/rest.py
--rw-r--r--   0        0        0     1526 2023-03-17 19:17:51.770032 flama-1.3.0/flama/resources/routing.py
--rw-r--r--   0        0        0    28254 2023-03-17 19:17:51.770032 flama-1.3.0/flama/routing.py
--rw-r--r--   0        0        0     2116 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/__init__.py
--rw-r--r--   0        0        0      339 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/marshmallow/__init__.py
--rw-r--r--   0        0        0     5013 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/marshmallow/adapter.py
--rw-r--r--   0        0        0      437 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/marshmallow/fields.py
--rw-r--r--   0        0        0     2993 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/marshmallow/schemas.py
--rw-r--r--   0        0        0      321 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/pydantic/__init__.py
--rw-r--r--   0        0        0     4156 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/pydantic/adapter.py
--rw-r--r--   0        0        0       13 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/pydantic/fields.py
--rw-r--r--   0        0        0     2093 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/pydantic/schemas.py
--rw-r--r--   0        0        0      331 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/typesystem/__init__.py
--rw-r--r--   0        0        0     3422 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/typesystem/adapter.py
--rw-r--r--   0        0        0      419 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/typesystem/fields.py
--rw-r--r--   0        0        0     2968 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/_libs/typesystem/schemas.py
--rw-r--r--   0        0        0     2599 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/adapter.py
--rw-r--r--   0        0        0     8146 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/data_structures.py
--rw-r--r--   0        0        0      464 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/exceptions.py
--rw-r--r--   0        0        0    20432 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/generator.py
--rw-r--r--   0        0        0     2776 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/modules.py
--rw-r--r--   0        0        0     9520 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/openapi.py
--rw-r--r--   0        0        0     2318 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/routing.py
--rw-r--r--   0        0        0     1603 2023-03-17 19:17:51.770032 flama-1.3.0/flama/schemas/validation.py
--rw-r--r--   0        0        0      176 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/__init__.py
--rw-r--r--   0        0        0      513 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/base.py
--rw-r--r--   0        0        0     9723 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/data_structures.py
--rw-r--r--   0        0        0     1434 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/dump.py
--rw-r--r--   0        0        0      112 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/exceptions.py
--rw-r--r--   0        0        0      436 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/load.py
--rw-r--r--   0        0        0        0 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/serializers/__init__.py
--rw-r--r--   0        0        0     1493 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/serializers/pytorch.py
--rw-r--r--   0        0        0     1021 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/serializers/sklearn.py
--rw-r--r--   0        0        0     1938 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/serializers/tensorflow.py
--rw-r--r--   0        0        0      193 2023-03-17 19:17:51.770032 flama-1.3.0/flama/serialize/types.py
--rw-r--r--   0        0        0     1463 2023-03-17 19:17:51.770032 flama-1.3.0/flama/sqlalchemy.py
--rw-r--r--   0        0        0   187325 2023-03-17 19:18:38.395062 flama-1.3.0/flama/templates/debug/error_404.html
--rw-r--r--   0        0        0   277094 2023-03-17 19:18:38.395062 flama-1.3.0/flama/templates/debug/error_500.html
--rw-r--r--   0        0        0   170529 2023-03-17 19:18:38.395062 flama-1.3.0/flama/templates/schemas/docs.html
--rw-r--r--   0        0        0       70 2023-03-17 19:17:51.770032 flama-1.3.0/flama/testclient.py
--rw-r--r--   0        0        0      164 2023-03-17 19:17:51.770032 flama-1.3.0/flama/types/__init__.py
--rw-r--r--   0        0        0     2265 2023-03-17 19:17:51.770032 flama-1.3.0/flama/types/asgi.py
--rw-r--r--   0        0        0     1311 2023-03-17 19:17:51.770032 flama-1.3.0/flama/types/http.py
--rw-r--r--   0        0        0     1130 2023-03-17 19:17:51.770032 flama-1.3.0/flama/types/schema.py
--rw-r--r--   0        0        0      162 2023-03-17 19:17:51.770032 flama-1.3.0/flama/types/websockets.py
--rw-r--r--   0        0        0     7674 2023-03-17 19:17:51.770032 flama-1.3.0/flama/url.py
--rw-r--r--   0        0        0     4925 2023-03-17 19:17:51.770032 flama-1.3.0/flama/validation.py
--rw-r--r--   0        0        0     1413 2023-03-17 19:17:51.770032 flama-1.3.0/flama/websockets.py
--rw-r--r--   0        0        0     5786 2023-03-17 19:18:13.970508 flama-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6527 1970-01-01 00:00:00.000000 flama-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11393 2023-06-08 13:29:50.254627 flama-1.4.0/LICENSE
+-rw-r--r--   0        0        0     4287 2023-06-08 13:29:50.254627 flama-1.4.0/README.md
+-rw-r--r--   0        0        0      406 2023-06-08 13:29:50.254627 flama-1.4.0/flama/__init__.py
+-rw-r--r--   0        0        0    12622 2023-06-08 13:29:50.254627 flama-1.4.0/flama/applications.py
+-rw-r--r--   0        0        0     2820 2023-06-08 13:29:50.254627 flama-1.4.0/flama/asgi.py
+-rw-r--r--   0        0        0      404 2023-06-08 13:29:50.254627 flama-1.4.0/flama/authentication.py
+-rw-r--r--   0        0        0     2998 2023-06-08 13:29:50.254627 flama-1.4.0/flama/background.py
+-rw-r--r--   0        0        0      149 2023-06-08 13:29:50.254627 flama-1.4.0/flama/cli/__init__.py
+-rw-r--r--   0        0        0      722 2023-06-08 13:29:50.254627 flama-1.4.0/flama/cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:29:50.254627 flama-1.4.0/flama/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3586 2023-06-08 13:29:50.254627 flama-1.4.0/flama/cli/commands/model.py
+-rw-r--r--   0        0        0      889 2023-06-08 13:29:50.254627 flama-1.4.0/flama/cli/commands/run.py
+-rw-r--r--   0        0        0      794 2023-06-08 13:29:50.254627 flama-1.4.0/flama/cli/commands/serve.py
+-rw-r--r--   0        0        0     1104 2023-06-08 13:29:50.258627 flama-1.4.0/flama/cli/commands/start.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:29:50.258627 flama-1.4.0/flama/cli/config/__init__.py
+-rw-r--r--   0        0        0     5201 2023-06-08 13:29:50.258627 flama-1.4.0/flama/cli/config/app.py
+-rw-r--r--   0        0        0     2595 2023-06-08 13:29:50.258627 flama-1.4.0/flama/cli/config/config.py
+-rw-r--r--   0        0        0    16250 2023-06-08 13:29:50.258627 flama-1.4.0/flama/cli/config/uvicorn.py
+-rw-r--r--   0        0        0      363 2023-06-08 13:29:50.258627 flama-1.4.0/flama/cli/templates/app.py.j2
+-rw-r--r--   0        0        0      126 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/__init__.py
+-rw-r--r--   0        0        0      713 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/base.py
+-rw-r--r--   0        0        0      189 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/http/__init__.py
+-rw-r--r--   0        0        0      485 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/http/jsondata.py
+-rw-r--r--   0        0        0      260 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/http/multipart.py
+-rw-r--r--   0        0        0      284 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/http/urlencoded.py
+-rw-r--r--   0        0        0      207 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/websockets/__init__.py
+-rw-r--r--   0        0        0      433 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/websockets/bytes.py
+-rw-r--r--   0        0        0      606 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/websockets/json.py
+-rw-r--r--   0        0        0      427 2023-06-08 13:29:50.258627 flama-1.4.0/flama/codecs/websockets/text.py
+-rw-r--r--   0        0        0     1488 2023-06-08 13:29:50.258627 flama-1.4.0/flama/concurrency.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:29:50.258627 flama-1.4.0/flama/debug/__init__.py
+-rw-r--r--   0        0        0     5551 2023-06-08 13:29:50.258627 flama-1.4.0/flama/debug/data_structures.py
+-rw-r--r--   0        0        0     7909 2023-06-08 13:29:50.258627 flama-1.4.0/flama/debug/middleware.py
+-rw-r--r--   0        0        0      350 2023-06-08 13:29:50.258627 flama-1.4.0/flama/debug/types.py
+-rw-r--r--   0        0        0     5935 2023-06-08 13:29:50.258627 flama-1.4.0/flama/endpoints.py
+-rw-r--r--   0        0        0     1000 2023-06-08 13:29:50.258627 flama-1.4.0/flama/events.py
+-rw-r--r--   0        0        0     3904 2023-06-08 13:29:50.258627 flama-1.4.0/flama/exceptions.py
+-rw-r--r--   0        0        0     7151 2023-06-08 13:29:50.258627 flama-1.4.0/flama/http.py
+-rw-r--r--   0        0        0      192 2023-06-08 13:29:50.258627 flama-1.4.0/flama/injection/__init__.py
+-rw-r--r--   0        0        0     3708 2023-06-08 13:29:50.258627 flama-1.4.0/flama/injection/components.py
+-rw-r--r--   0        0        0      800 2023-06-08 13:29:50.258627 flama-1.4.0/flama/injection/exceptions.py
+-rw-r--r--   0        0        0     2591 2023-06-08 13:29:50.258627 flama-1.4.0/flama/injection/injector.py
+-rw-r--r--   0        0        0     7324 2023-06-08 13:29:50.258627 flama-1.4.0/flama/injection/resolver.py
+-rw-r--r--   0        0        0      144 2023-06-08 13:29:50.258627 flama-1.4.0/flama/injection/types.py
+-rw-r--r--   0        0        0     2105 2023-06-08 13:29:50.258627 flama-1.4.0/flama/lifespan.py
+-rw-r--r--   0        0        0     3421 2023-06-08 13:29:50.258627 flama-1.4.0/flama/middleware.py
+-rw-r--r--   0        0        0      173 2023-06-08 13:29:50.258627 flama-1.4.0/flama/models/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-08 13:29:50.258627 flama-1.4.0/flama/models/base.py
+-rw-r--r--   0        0        0     1736 2023-06-08 13:29:50.258627 flama-1.4.0/flama/models/components.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:29:50.258627 flama-1.4.0/flama/models/models/__init__.py
+-rw-r--r--   0        0        0      526 2023-06-08 13:29:50.258627 flama-1.4.0/flama/models/models/pytorch.py
+-rw-r--r--   0        0        0      342 2023-06-08 13:29:50.258627 flama-1.4.0/flama/models/models/sklearn.py
+-rw-r--r--   0        0        0      555 2023-06-08 13:29:50.258627 flama-1.4.0/flama/models/models/tensorflow.py
+-rw-r--r--   0        0        0     2560 2023-06-08 13:29:50.258627 flama-1.4.0/flama/models/modules.py
+-rw-r--r--   0        0        0     4511 2023-06-08 13:29:50.258627 flama-1.4.0/flama/models/resource.py
+-rw-r--r--   0        0        0     1568 2023-06-08 13:29:50.258627 flama-1.4.0/flama/modules.py
+-rw-r--r--   0        0        0     1660 2023-06-08 13:29:50.258627 flama-1.4.0/flama/negotiation.py
+-rw-r--r--   0        0        0      271 2023-06-08 13:29:50.258627 flama-1.4.0/flama/pagination/__init__.py
+-rw-r--r--   0        0        0     4811 2023-06-08 13:29:50.258627 flama-1.4.0/flama/pagination/limit_offset.py
+-rw-r--r--   0        0        0     5076 2023-06-08 13:29:50.258627 flama-1.4.0/flama/pagination/page_number.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:29:50.258627 flama-1.4.0/flama/py.typed
+-rw-r--r--   0        0        0      139 2023-06-08 13:29:50.258627 flama-1.4.0/flama/resources/__init__.py
+-rw-r--r--   0        0        0    10853 2023-06-08 13:29:50.258627 flama-1.4.0/flama/resources/crud.py
+-rw-r--r--   0        0        0     1323 2023-06-08 13:29:50.258627 flama-1.4.0/flama/resources/data_structures.py
+-rw-r--r--   0        0        0      704 2023-06-08 13:29:50.258627 flama-1.4.0/flama/resources/exceptions.py
+-rw-r--r--   0        0        0     1620 2023-06-08 13:29:50.258627 flama-1.4.0/flama/resources/modules.py
+-rw-r--r--   0        0        0     5219 2023-06-08 13:29:50.258627 flama-1.4.0/flama/resources/resource.py
+-rw-r--r--   0        0        0     5345 2023-06-08 13:29:50.258627 flama-1.4.0/flama/resources/rest.py
+-rw-r--r--   0        0        0     1900 2023-06-08 13:29:50.258627 flama-1.4.0/flama/resources/routing.py
+-rw-r--r--   0        0        0    28590 2023-06-08 13:29:50.258627 flama-1.4.0/flama/routing.py
+-rw-r--r--   0        0        0     2116 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/__init__.py
+-rw-r--r--   0        0        0      339 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/marshmallow/__init__.py
+-rw-r--r--   0        0        0     5006 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/marshmallow/adapter.py
+-rw-r--r--   0        0        0      437 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/marshmallow/fields.py
+-rw-r--r--   0        0        0     2993 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/marshmallow/schemas.py
+-rw-r--r--   0        0        0      321 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/pydantic/__init__.py
+-rw-r--r--   0        0        0     4149 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/pydantic/adapter.py
+-rw-r--r--   0        0        0       13 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/pydantic/fields.py
+-rw-r--r--   0        0        0     2093 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/pydantic/schemas.py
+-rw-r--r--   0        0        0      331 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/typesystem/__init__.py
+-rw-r--r--   0        0        0     3415 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/typesystem/adapter.py
+-rw-r--r--   0        0        0      419 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/typesystem/fields.py
+-rw-r--r--   0        0        0     2968 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/_libs/typesystem/schemas.py
+-rw-r--r--   0        0        0     2622 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/adapter.py
+-rw-r--r--   0        0        0     7954 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/data_structures.py
+-rw-r--r--   0        0        0      464 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/exceptions.py
+-rw-r--r--   0        0        0    20432 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/generator.py
+-rw-r--r--   0        0        0     2776 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/modules.py
+-rw-r--r--   0        0        0     9521 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/openapi.py
+-rw-r--r--   0        0        0     2318 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/routing.py
+-rw-r--r--   0        0        0     1603 2023-06-08 13:29:50.258627 flama-1.4.0/flama/schemas/validation.py
+-rw-r--r--   0        0        0      176 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/__init__.py
+-rw-r--r--   0        0        0      513 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/base.py
+-rw-r--r--   0        0        0    11320 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/data_structures.py
+-rw-r--r--   0        0        0     1434 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/dump.py
+-rw-r--r--   0        0        0      112 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/exceptions.py
+-rw-r--r--   0        0        0      436 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/load.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/serializers/__init__.py
+-rw-r--r--   0        0        0     1493 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/serializers/pytorch.py
+-rw-r--r--   0        0        0     1531 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/serializers/sklearn.py
+-rw-r--r--   0        0        0     1938 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/serializers/tensorflow.py
+-rw-r--r--   0        0        0      193 2023-06-08 13:29:50.258627 flama-1.4.0/flama/serialize/types.py
+-rw-r--r--   0        0        0     1463 2023-06-08 13:29:50.258627 flama-1.4.0/flama/sqlalchemy.py
+-rw-r--r--   0        0        0   187325 2023-06-08 13:30:36.170369 flama-1.4.0/flama/templates/debug/error_404.html
+-rw-r--r--   0        0        0   277094 2023-06-08 13:30:36.170369 flama-1.4.0/flama/templates/debug/error_500.html
+-rw-r--r--   0        0        0   170529 2023-06-08 13:30:36.170369 flama-1.4.0/flama/templates/schemas/docs.html
+-rw-r--r--   0        0        0       70 2023-06-08 13:29:50.258627 flama-1.4.0/flama/testclient.py
+-rw-r--r--   0        0        0      375 2023-06-08 13:29:50.258627 flama-1.4.0/flama/types/__init__.py
+-rw-r--r--   0        0        0     2281 2023-06-08 13:29:50.258627 flama-1.4.0/flama/types/asgi.py
+-rw-r--r--   0        0        0     1311 2023-06-08 13:29:50.258627 flama-1.4.0/flama/types/http.py
+-rw-r--r--   0        0        0      966 2023-06-08 13:29:50.258627 flama-1.4.0/flama/types/schema.py
+-rw-r--r--   0        0        0      162 2023-06-08 13:29:50.258627 flama-1.4.0/flama/types/websockets.py
+-rw-r--r--   0        0        0     7674 2023-06-08 13:29:50.258627 flama-1.4.0/flama/url.py
+-rw-r--r--   0        0        0     4925 2023-06-08 13:29:50.258627 flama-1.4.0/flama/validation.py
+-rw-r--r--   0        0        0     1413 2023-06-08 13:29:50.258627 flama-1.4.0/flama/websockets.py
+-rw-r--r--   0        0        0     5667 2023-06-08 13:30:13.674509 flama-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6526 1970-01-01 00:00:00.000000 flama-1.4.0/PKG-INFO
```

### Comparing `flama-1.3.0/LICENSE` & `flama-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/README.md` & `flama-1.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 @app.route("/")
 def home():
     """
     tags:
         - Salute
     summary:
-        Returns a warming message.
+        Returns a warming message
     description:
         This is a more detailed description of the method itself.
         Here we can give all the details required and they will appear
         automatically in the auto-generated docs.
     responses:
         200:
             description: Warming hello message!
```

### Comparing `flama-1.3.0/flama/applications.py` & `flama-1.4.0/flama/applications.py`

 * *Files 10% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         self,
         path: t.Optional[str] = None,
         endpoint: t.Optional[types.HTTPHandler] = None,
         methods: t.Optional[t.List[str]] = None,
         name: t.Optional[str] = None,
         include_in_schema: bool = True,
         route: t.Optional["Route"] = None,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> "Route":
         """Register a new HTTP route or endpoint under given path.
 
         :param path: URL path.
         :param endpoint: HTTP endpoint.
         :param methods: List of valid HTTP methods (only applies for routes).
         :param name: Endpoint or route name.
@@ -175,86 +175,86 @@
             path,
             endpoint,
             methods=methods,
             name=name,
             include_in_schema=include_in_schema,
             route=route,
             root=self,
-            **tags,
+            tags=tags,
         )
 
     def route(
         self,
         path: str,
         methods: t.Optional[t.List[str]] = None,
         name: t.Optional[str] = None,
         include_in_schema: bool = True,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> t.Callable[[types.HTTPHandler], types.HTTPHandler]:
         """Decorator version for registering a new HTTP route in this router under given path.
 
         :param path: URL path.
         :param methods: List of valid HTTP methods (only applies for routes).
         :param name: Endpoint or route name.
         :param include_in_schema: True if this route or endpoint should be declared as part of the API schema.
         :param tags: Tags to add to the route.
         :return: Decorated route.
         """
         return self.router.route(
-            path, methods=methods, name=name, include_in_schema=include_in_schema, root=self, **tags
+            path, methods=methods, name=name, include_in_schema=include_in_schema, root=self, tags=tags
         )
 
     def add_websocket_route(
         self,
         path: t.Optional[str] = None,
         endpoint: t.Optional[types.WebSocketHandler] = None,
         name: t.Optional[str] = None,
         route: t.Optional["WebSocketRoute"] = None,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> "WebSocketRoute":
         """Register a new websocket route or endpoint under given path.
 
         :param path: URL path.
         :param endpoint: Websocket endpoint.
         :param name: Endpoint or route name.
         :param route: Websocket route.
         :param tags: Tags to add to the websocket route.
         """
-        return self.router.add_websocket_route(path, endpoint, name=name, route=route, root=self, **tags)
+        return self.router.add_websocket_route(path, endpoint, name=name, route=route, root=self, tags=tags)
 
     def websocket_route(
-        self, path: str, name: t.Optional[str] = None, **tags: t.Any
+        self, path: str, name: t.Optional[str] = None, tags: t.Optional[t.Dict[str, types.Tag]] = None
     ) -> t.Callable[[types.WebSocketHandler], types.WebSocketHandler]:
         """Decorator version for registering a new websocket route in this router under given path.
 
         :param path: URL path.
         :param name: Websocket route name.
         :param tags: Tags to add to the websocket route.
         :return: Decorated route.
         """
-        return self.router.websocket_route(path, name=name, root=self, **tags)
+        return self.router.websocket_route(path, name=name, root=self, tags=tags)
 
     def mount(
         self,
         path: t.Optional[str] = None,
         app: t.Optional[types.App] = None,
         name: t.Optional[str] = None,
         mount: t.Optional["Mount"] = None,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> "Mount":
         """Register a new mount point containing an ASGI app in this router under given path.
 
         :param path: URL path.
         :param app: ASGI app to mount.
         :param name: Application name.
         :param mount: Mount.
         :param tags: Tags to add to the mount.
         :return: Mount.
         """
-        return self.router.mount(path, app, name=name, mount=mount, root=self, **tags)
+        return self.router.mount(path, app, name=name, mount=mount, root=self, tags=tags)
 
     @property
     def injector(self) -> injection.Injector:
         """Components dependency injector.
 
         :return: Injector instance.
         """
```

### Comparing `flama-1.3.0/flama/asgi.py` & `flama-1.4.0/flama/asgi.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/background.py` & `flama-1.4.0/flama/background.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/cli/__main__.py` & `flama-1.4.0/flama/cli/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from flama.cli.commands.serve import command as serve_command
 from flama.cli.commands.start import command as start_command
 
 
 @click.group()
 @click.version_option(
     package_name="Flama",
+    message="Flama %(version)s",
     help="Check the version of your locally installed Flama",
 )
 @click.help_option(help="Get help about how to use Flama CLI")
 def cli():
     """
     Fire up your models with Flama 🔥
     """
```

### Comparing `flama-1.3.0/flama/cli/commands/model.py` & `flama-1.4.0/flama/cli/commands/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 import functools
 import json
+import typing as t
 
 import click
 
 from flama.http import EnhancedJSONEncoder
 from flama.models import ModelComponentBuilder
 
+if t.TYPE_CHECKING:
+    from flama.models import ModelComponent
+
 __all__ = ["model", "command"]
 
 
 @click.group(name="model")
-@click.argument("model-path", envvar="FLAMA_MODEL_PATH")
-def command(model_path: str):
+@click.argument("flama-model-path", envvar="FLAMA_MODEL_PATH")
+@click.pass_context
+def command(ctx: click.Context, flama_model_path: str):
     """Interact with an ML model without server.
 
     This command is used to directly interact with an ML model without the need of a server. This command can be used
     to perform any operation that is supported by the model, such as inspect, or predict.
     <FLAMA_MODEL_PATH> is the path of the model to be used, e.g. 'path/to/model.flm'. This can be passed
     directly as argument of the command line, or by environment variable.
     """
-    ...
+    try:
+        ctx.obj = ModelComponentBuilder.load(flama_model_path)
+    except FileNotFoundError:
+        raise click.BadParameter("Model file not found.")
 
 
 @command.command(name="inspect", context_settings={"auto_envvar_prefix": "FLAMA"})
 @click.option("-p", "--pretty", is_flag=True, default=False, help="Pretty print the model inspection.")
-@click.pass_context
-def inspect(ctx: click.Context, pretty: bool):
+@click.pass_obj
+def inspect(model: "ModelComponent", pretty: bool):
     """Inspect an ML model.
 
     This command is used to inspect an ML model without the need of a server. This command can be used to extract the
     ML model metadata, including the ID, time when the model was created, information of the
     framework, and the model info; and the list of artifacts packaged with the model.
     """
-    try:
-        model = ModelComponentBuilder.load(ctx.parent.params["model_path"])  # type: ignore[union-attr]
-    except FileNotFoundError:
-        raise click.BadParameter("Model file not found.")
-
     dump_func = functools.partial(json.dumps, cls=EnhancedJSONEncoder)
     if pretty:
         dump_func = functools.partial(dump_func, sort_keys=True, indent=4)
 
     click.echo(dump_func(model.model.inspect()))
 
 
@@ -57,17 +60,17 @@
     "-o",
     "--output",
     "output_file",
     type=click.File("w"),
     default="-",
     help="File to be used as output for the model prediction in JSON format. (default: stdout).",
 )
-@click.option("-p", "--pretty", is_flag=True, default=False, help="Pretty print the model inspection.")
-@click.pass_context
-def predict(ctx: click.Context, input_file, output_file, pretty: bool):
+@click.option("-p", "--pretty", is_flag=True, default=False, help="Pretty print the model prediction.")
+@click.pass_obj
+def predict(model: "ModelComponent", input_file, output_file, pretty: bool):
     """Make a prediction using an ML model.
 
     This command is used to make a prediction using an ML model without the need of a server. It can be used for
     batch predictions, so both input and output arguments must be json files containing a list of input values, each
     input value being a list of values associated to the input of the model. The output will be the list of predictions
     associated to the input, with each prediction being a list of values representing the output of the model.
 
@@ -76,24 +79,19 @@
     - input.json:
     [[0, 0], [0, 1], [1, 0], [1, 1]]
 
     - output.json:
     [[0], [1], [1], [0]]
     """
     try:
-        model = ModelComponentBuilder.load(ctx.parent.params["model_path"])  # type: ignore[union-attr]
-    except FileNotFoundError:
-        raise click.BadParameter("Model file not found.")
-
-    try:
         data = json.load(input_file)
     except json.JSONDecodeError:
         raise click.BadParameter("Input file must be a valid json file.")
 
     dump_func = functools.partial(json.dumps, cls=EnhancedJSONEncoder)
     if pretty:
         dump_func = functools.partial(dump_func, sort_keys=True, indent=4)
 
     click.echo(dump_func(model.model.predict(data)), output_file)
 
 
-model = command.callback
+model: t.Callable = command.callback  # type: ignore[assignment]
```

### Comparing `flama-1.3.0/flama/cli/commands/run.py` & `flama-1.4.0/flama/cli/commands/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing as t
+
 import click
 
 from flama.cli.config.app import App
 from flama.cli.config.config import Config
 from flama.cli.config.config import options as config_options
 from flama.cli.config.uvicorn import Uvicorn
 from flama.cli.config.uvicorn import options as uvicorn_options
@@ -17,8 +19,8 @@
     """Run a Flama Application based on a route.
 
     <FLAMA_APP> is the route to the Flama object to be served, e.g. 'examples.hello_flama:app'. This can be passed
     directly as argument of the command line, or by environment variable."""
     Config(app=App.build(flama_app), server=uvicorn).run()
 
 
-run = command.callback
+run: t.Callable = command.callback  # type: ignore[assignment]
```

### Comparing `flama-1.3.0/flama/cli/commands/serve.py` & `flama-1.4.0/flama/cli/commands/serve.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing as t
+
 import click
 
 from flama.cli.config.app import App
 from flama.cli.config.app import options as app_options
 from flama.cli.config.config import Config
 from flama.cli.config.config import options as config_options
 from flama.cli.config.uvicorn import Uvicorn
@@ -17,8 +19,8 @@
 def command(app: App, uvicorn: Uvicorn):
     """Serve an ML model file within a Flama Application.
 
     Serve the ML model file specified by <MODEL_PATH> within a Flama Application."""
     Config(app=app, server=uvicorn).run()
 
 
-serve = command.callback
+serve: t.Callable = command.callback  # type: ignore[assignment]
```

### Comparing `flama-1.3.0/flama/cli/commands/start.py` & `flama-1.4.0/flama/cli/commands/start.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing as t
+
 import click
 
 from flama.cli.config.config import Config, ExampleConfig
 
 __all__ = ["start", "command"]
 
 
@@ -26,8 +28,8 @@
 
     with open(flama_config, "r") as fs:
         config = Config.load(fs)  # type: ignore[arg-type]
 
     config.run()
 
 
-start = command.callback
+start: t.Callable = command.callback  # type: ignore[assignment]
```

### Comparing `flama-1.3.0/flama/cli/config/app.py` & `flama-1.4.0/flama/cli/config/app.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/cli/config/config.py` & `flama-1.4.0/flama/cli/config/config.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/cli/config/uvicorn.py` & `flama-1.4.0/flama/cli/config/uvicorn.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/codecs/base.py` & `flama-1.4.0/flama/codecs/base.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/codecs/websockets/json.py` & `flama-1.4.0/flama/codecs/websockets/json.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/concurrency.py` & `flama-1.4.0/flama/concurrency.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/debug/data_structures.py` & `flama-1.4.0/flama/debug/data_structures.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/debug/middleware.py` & `flama-1.4.0/flama/debug/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import dataclasses
 import inspect
 import typing as t
 from pathlib import Path
 
 import starlette.exceptions
 
-from flama import concurrency, exceptions, http, websockets
+from flama import concurrency, exceptions, http, types, websockets
 from flama.debug.data_structures import ErrorContext, NotFoundContext
 
 if t.TYPE_CHECKING:
-    from flama import types
     from flama.debug.types import Handler
 
 __all__ = ["ServerErrorMiddleware", "ExceptionMiddleware"]
 
 TEMPLATES_PATH = Path(__file__).parents[1].resolve() / "templates" / "debug"
 
 
-class BaseErrorMiddleware(abc.ABC):
+class BaseErrorMiddleware(types.MiddlewareAsyncClass):
     def __init__(self, app: "types.App", debug: bool = False) -> None:
         self.app = app
         self.debug = debug
 
     async def __call__(self, scope: "types.Scope", receive: "types.Receive", send: "types.Send") -> None:
         response_started = False
```

### Comparing `flama-1.3.0/flama/endpoints.py` & `flama-1.4.0/flama/endpoints.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/events.py` & `flama-1.4.0/flama/events.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/exceptions.py` & `flama-1.4.0/flama/exceptions.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/http.py` & `flama-1.4.0/flama/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pathlib import Path
 
 import jinja2
 import starlette.requests
 import starlette.responses
 import starlette.schemas
 
+import flama.types
 from flama import schemas, types
 from flama.exceptions import HTTPException, SerializationError
 
 if t.TYPE_CHECKING:
     from flama.types.schema import _T_Schema
 
 __all__ = [
@@ -189,27 +190,27 @@
                 "variable_start_string": "||@",
                 "variable_end_string": "@||",
             },
         )
 
         self.filters["safe_json"] = self.safe_json
 
-    def _escape(self, value: types.JSONField) -> types.JSONField:
+    def _escape(self, value: flama.types.JSONField) -> flama.types.JSONField:
         if isinstance(value, (list, tuple)):
             return [self._escape(x) for x in value]
 
         if isinstance(value, dict):
             return {k: self._escape(v) for k, v in value.items()}
 
         if isinstance(value, str):
             return html.escape(value).replace("\n", "&#13;")
 
         return value
 
-    def safe_json(self, value: types.JSONField):
+    def safe_json(self, value: flama.types.JSONField):
         return json.dumps(self._escape(value)).replace('"', '\\"')
 
 
 class _ReactTemplateResponse(HTMLTemplateResponse):
     templates = _ReactTemplatesEnvironment(
         loader=jinja2.ChoiceLoader(
             [jinja2.FileSystemLoader(Path(os.curdir) / "templates"), jinja2.PackageLoader("flama", "templates")]
```

### Comparing `flama-1.3.0/flama/injection/components.py` & `flama-1.4.0/flama/injection/components.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/injection/exceptions.py` & `flama-1.4.0/flama/injection/exceptions.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/injection/injector.py` & `flama-1.4.0/flama/injection/injector.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/injection/resolver.py` & `flama-1.4.0/flama/injection/resolver.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/lifespan.py` & `flama-1.4.0/flama/lifespan.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/middleware.py` & `flama-1.4.0/flama/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 class Middleware:
     def __init__(self, middleware: "types.Middleware", **kwargs: t.Any) -> None:
         self.middleware = middleware
         self.kwargs = kwargs
 
     def __call__(self, app: "types.App"):
-        return self.middleware(app=app, **self.kwargs)
+        return self.middleware(app, **self.kwargs)
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
         middleware_name = (
             self.middleware.__name__ if inspect.isfunction(self.middleware) else self.middleware.__class__.__name__
         )
         args = ", ".join([middleware_name] + [f"{key}={value!r}" for key, value in self.kwargs.items()])
```

### Comparing `flama-1.3.0/flama/models/components.py` & `flama-1.4.0/flama/models/components.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/models/models/pytorch.py` & `flama-1.4.0/flama/models/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/models/models/tensorflow.py` & `flama-1.4.0/flama/models/models/tensorflow.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/models/modules.py` & `flama-1.4.0/flama/resources/modules.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,52 @@
-import os
-import typing
+import inspect
+import typing as t
 
-from flama.models.resource import ModelResource, ModelResourceType
 from flama.modules import Module
+from flama.resources.routing import ResourceRoute
 
-__all__ = ["ModelsModule"]
-
-
-class ModelsModule(Module):
-    name = "models"
-
-    def add_model(self, path: str, model: typing.Union[str, os.PathLike], name: str, *args, **kwargs):
-        """Adds a model to this application, setting its endpoints.
+if t.TYPE_CHECKING:
+    from flama import types
+    from flama.resources.resource import BaseResource
+
+__all__ = ["ResourcesModule"]
+
+
+class ResourcesModule(Module):
+    name = "resources"
+
+    def add_resource(
+        self,
+        path: str,
+        resource: t.Union["BaseResource", t.Type["BaseResource"]],
+        tags: t.Optional[t.Dict[str, t.Dict[str, "types.Tag"]]] = None,
+        *args,
+        **kwargs
+    ) -> "BaseResource":
+        """Adds a resource to this application, setting its endpoints.
 
         :param path: Resource base path.
-        :param model: Model path.
-        :param name: Model name.
+        :param tags: Tags to add to the resource.
+        :param resource: Resource class.
         """
+        # Handle class or instance objects
+        resource_instance: "BaseResource" = resource(*args, **kwargs) if inspect.isclass(resource) else resource
 
-        name_ = name
-        model_ = model
+        self.app.mount(mount=ResourceRoute(path, resource_instance, tags))
 
-        class Resource(ModelResource, metaclass=ModelResourceType):
-            name = name_
-            model_path = model_
-
-        resource = Resource()
-        self.app.add_component(resource.component)
-        self.app.resources.add_resource(path, resource)  # type: ignore[attr-defined]
+        return resource_instance
 
-    def model(self, path: str, *args, **kwargs) -> typing.Callable:
-        """Decorator for ModelResource classes for adding them to the application.
+    def resource(
+        self, path: str, tags: t.Optional[t.Dict[str, t.Dict[str, "types.Tag"]]] = None, *args, **kwargs
+    ) -> t.Callable:
+        """Decorator for Resources classes for adding them to the application.
 
         :param path: Resource base path.
+        :param tags: Tags to add to the resource.
         :return: Decorated resource class.
         """
 
-        def decorator(resource: typing.Type[ModelResource]) -> typing.Type[ModelResource]:
-            self.app.add_component(resource.component)
-            self.app.resources.add_resource(path, resource, *args, **kwargs)  # type: ignore[attr-defined]
+        def decorator(resource: t.Type["BaseResource"]) -> t.Type["BaseResource"]:
+            self.add_resource(path, resource, tags, *args, **kwargs)
             return resource
 
         return decorator
-
-    def add_model_resource(
-        self, path: str, resource: typing.Union[ModelResource, typing.Type[ModelResource]], *args, **kwargs
-    ):
-        """Adds a resource to this application, setting its endpoints.
-
-        :param path: Resource base path.
-        :param resource: Resource class.
-        """
-        self.app.add_component(resource.component)
-        self.app.resources.add_resource(path, resource, *args, **kwargs)  # type: ignore[attr-defined]
```

### Comparing `flama-1.3.0/flama/models/resource.py` & `flama-1.4.0/flama/models/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         async def inspect(self, model: model_model_type):  # type: ignore[valid-type]
             return model.inspect()  # type: ignore[attr-defined]
 
         inspect.__doc__ = f"""
             tags:
                 - {verbose_name}
             summary:
-                Retrieve the model.
+                Retrieve the model
             description:
                 Retrieve the model from this resource.
             responses:
                 200:
                     description:
                         The model.
         """
@@ -54,15 +54,15 @@
         ) -> types.Schema[flama.schemas.schemas.MLModelOutput]:  # type: ignore[type-arg]
             return types.Schema({"output": model.predict(data["input"])})  # type: ignore[attr-defined]
 
         predict.__doc__ = f"""
             tags:
                 - {verbose_name}
             summary:
-                Generate a prediction.
+                Generate a prediction
             description:
                 Generate a prediction using the model from this resource.
             responses:
                 200:
                     description:
                         The prediction generated by the model.
         """
```

### Comparing `flama-1.3.0/flama/modules.py` & `flama-1.4.0/flama/modules.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/negotiation.py` & `flama-1.4.0/flama/negotiation.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/pagination/limit_offset.py` & `flama-1.4.0/flama/pagination/limit_offset.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
             forge_revision_list = (
                 forge.copy(func),
                 forge.insert(forge.arg("limit", default=None, type=t.Optional[int]), index=-1),
                 forge.insert(forge.arg("offset", default=None, type=t.Optional[int]), index=-1),
                 forge.insert(forge.arg("count", default=True, type=bool), index=-1),
                 forge.delete("kwargs"),
-                forge.returns(types.Schema[schema]),  # type: ignore[index]
+                forge.returns(types.Schema[schema]),  # type: ignore[index,valid-type]
             )
 
             try:
                 if asyncio.iscoroutinefunction(func):
 
                     @forge.compose(*forge_revision_list)
                     @functools.wraps(func)
```

### Comparing `flama-1.3.0/flama/pagination/page_number.py` & `flama-1.4.0/flama/pagination/page_number.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
             forge_revision_list = (
                 forge.copy(func),
                 forge.insert(forge.arg("page", default=None, type=t.Optional[int]), index=-1),
                 forge.insert(forge.arg("page_size", default=None, type=t.Optional[int]), index=-1),
                 forge.insert(forge.arg("count", default=True, type=bool), index=-1),
                 forge.delete("kwargs"),
-                forge.returns(types.Schema[schema]),  # type: ignore[index]
+                forge.returns(types.Schema[schema]),  # type: ignore[index,valid-type]
             )
 
             try:
                 if asyncio.iscoroutinefunction(func):
 
                     @forge.compose(*forge_revision_list)
                     @functools.wraps(func)
```

### Comparing `flama-1.3.0/flama/resources/crud.py` & `flama-1.4.0/flama/resources/crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 status_code=201,
             )
 
         create.__doc__ = f"""
             tags:
                 - {verbose_name}
             summary:
-                Create a new document.
+                Create a new document
             description:
                 Create a new document in this resource.
             responses:
                 201:
                     description:
                         Document created successfully.
         """
@@ -100,15 +100,15 @@
 
             return types.Schema(element._asdict())
 
         retrieve.__doc__ = f"""
             tags:
                 - {verbose_name}
             summary:
-                Retrieve a document.
+                Retrieve a document
             description:
                 Retrieve a document from this resource.
             responses:
                 200:
                     description:
                         Document found.
                 404:
@@ -161,15 +161,15 @@
 
             return types.Schema({rest_model.primary_key.name: element_id, **clean_element})
 
         update.__doc__ = f"""
             tags:
                 - {verbose_name}
             summary:
-                Update a document.
+                Update a document
             description:
                 Update a document in this resource.
             responses:
                 200:
                     description:
                         Document updated successfully.
                 404:
@@ -207,15 +207,15 @@
 
             return http.APIResponse(status_code=204)
 
         delete.__doc__ = f"""
             tags:
                 - {verbose_name}
             summary:
-                Delete a document.
+                Delete a document
             description:
                 Delete a document in this resource.
             responses:
                 204:
                     description:
                         Document deleted successfully.
                 404:
@@ -251,15 +251,15 @@
 
             return await self._filter(app)  # type: ignore[no-any-return,return-value]
 
         list.__doc__ = f"""
             tags:
                 - {verbose_name}
             summary:
-                List collection.
+                List collection
             description:
                 List resource collection.
             responses:
                 200:
                     description:
                         List collection items.
         """
@@ -284,15 +284,15 @@
                 schema=flama.schemas.schemas.DropCollection, content={"deleted": result.rowcount}, status_code=204
             )
 
         drop.__doc__ = f"""
             tags:
                 - {verbose_name}
             summary:
-                Drop collection.
+                Drop collection
             description:
                 Drop resource collection.
             responses:
                 204:
                     description:
                         Collection dropped successfully.
         """
```

### Comparing `flama-1.3.0/flama/resources/data_structures.py` & `flama-1.4.0/flama/resources/data_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 
 
 @dataclasses.dataclass
 class MethodMetadata:
     path: str
     methods: typing.Set[str] = dataclasses.field(default_factory=lambda: {"GET"})
     name: typing.Optional[str] = None
-    kwargs: typing.Dict[str, typing.Any] = dataclasses.field(default_factory=dict)
+    tags: typing.Dict[str, typing.Any] = dataclasses.field(default_factory=dict)
```

### Comparing `flama-1.3.0/flama/resources/exceptions.py` & `flama-1.4.0/flama/resources/exceptions.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/resources/resource.py` & `flama-1.4.0/flama/resources/resource.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/resources/rest.py` & `flama-1.4.0/flama/resources/rest.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/routing.py` & `flama-1.4.0/flama/routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,30 +178,30 @@
     def __init__(
         self,
         path: t.Union[str, url.RegexPath],
         app: types.App,
         *,
         name: t.Optional[str] = None,
         include_in_schema: bool = True,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ):
         """A route definition of a http endpoint.
 
         :param path: URL path.
         :param app: ASGI application.
         :param name: Route name.
         :param include_in_schema: True if this route must be listed as part of the App schema.
         :param tags: Route tags.
         """
         self.path = url.RegexPath(path)
         self.app = app
         self.endpoint = app.handler if isinstance(app, EndpointWrapper) else app
         self.name = name
         self.include_in_schema = include_in_schema
-        self.tags = tags
+        self.tags = tags or {}
         super().__init__()
 
     async def __call__(self, scope: types.Scope, receive: types.Receive, send: types.Send) -> None:
         await self.handle(types.Scope({**scope, **self.route_scope(scope)}), receive, send)
 
     def __eq__(self, other: t.Any) -> bool:
         return (
@@ -287,15 +287,15 @@
         self,
         path: str,
         endpoint: t.Union[t.Callable, t.Type[endpoints.HTTPEndpoint]],
         *,
         methods: t.Optional[t.Union[t.Set[str], t.Sequence[str]]] = None,
         name: t.Optional[str] = None,
         include_in_schema: bool = True,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> None:
         """A route definition of a http endpoint.
 
         :param path: URL path.
         :param endpoint: HTTP endpoint or function.
         :param methods: List of valid HTTP methods.
         :param name: Route name.
@@ -317,15 +317,15 @@
         name = endpoint.__name__ if name is None else name
 
         super().__init__(
             path,
             EndpointWrapper(endpoint, EndpointWrapper.type.http),
             name=name,
             include_in_schema=include_in_schema,
-            **tags,
+            tags=tags,
         )
 
         self.app: EndpointWrapper
 
     def __eq__(self, other: t.Any) -> bool:
         return super().__eq__(other) and isinstance(other, Route) and self.methods == other.methods
 
@@ -374,15 +374,15 @@
     def __init__(
         self,
         path: str,
         endpoint: t.Union[t.Callable, t.Type[endpoints.WebSocketEndpoint]],
         *,
         name: t.Optional[str] = None,
         include_in_schema: bool = True,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ):
         """A route definition of a websocket endpoint.
 
         :param path: URL path.
         :param endpoint: Websocket endpoint or function.
         :param name: Route name.
         :param include_in_schema: True if this route must be listed as part of the App schema.
@@ -396,15 +396,15 @@
         name = endpoint.__name__ if name is None else name
 
         super().__init__(
             path,
             EndpointWrapper(endpoint, EndpointWrapper.type.websocket),
             name=name,
             include_in_schema=include_in_schema,
-            **tags,
+            tags=tags,
         )
 
         self.app: EndpointWrapper
 
     def __eq__(self, other: t.Any) -> bool:
         return super().__eq__(other) and isinstance(other, WebSocketRoute)
 
@@ -443,15 +443,15 @@
         self,
         path: str,
         app: t.Optional[types.App] = None,
         *,
         routes: t.Optional[t.Sequence[BaseRoute]] = None,
         components: t.Optional[t.Sequence[Component]] = None,
         name: t.Optional[str] = None,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ):
         """A mount point for adding a nested ASGI application or a list of routes.
 
         :param path: URL path.
         :param app: ASGI application.
         :param routes: List of routes.
         :param components: Components registered under this mount point.
@@ -459,15 +459,15 @@
         :param tags: Mount tags.
         """
         assert app is not None or routes is not None, "Either 'app' or 'routes' must be specified"
 
         if app is None:
             app = Router(routes=routes, components=components)
 
-        super().__init__(url.RegexPath(path.rstrip("/") + "{path:path}"), app, name=name, **tags)
+        super().__init__(url.RegexPath(path.rstrip("/") + "{path:path}"), app, name=name, tags=tags)
 
     def __eq__(self, other: t.Any) -> bool:
         return super().__eq__(other) and isinstance(other, Mount)
 
     def build(self, app: t.Optional["Flama"] = None) -> None:
         """Build step for routes.
 
@@ -628,15 +628,15 @@
         path: t.Optional[str] = None,
         endpoint: t.Optional[types.HTTPHandler] = None,
         methods: t.Optional[t.List[str]] = None,
         name: t.Optional[str] = None,
         include_in_schema: bool = True,
         route: t.Optional[Route] = None,
         root: t.Optional["Flama"] = None,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> Route:
         """Register a new HTTP route in this router under given path.
 
         :param path: URL path.
         :param endpoint: HTTP endpoint.
         :param methods: List of valid HTTP methods (only applies for routes).
         :param name: Endpoint or route name.
@@ -644,15 +644,15 @@
         :param route: HTTP route.
         :param root: Flama application.
         :param tags: Tags to add to the route or endpoint.
         :return: Route.
         """
         if path is not None and endpoint is not None:
             route = Route(
-                path, endpoint=endpoint, methods=methods, name=name, include_in_schema=include_in_schema, **tags
+                path, endpoint=endpoint, methods=methods, name=name, include_in_schema=include_in_schema, tags=tags
             )
 
         assert route is not None, "Either 'path' and 'endpoint' or 'route' variables are needed"
 
         self.routes.append(route)
 
         route.build(root)
@@ -662,108 +662,108 @@
     def route(
         self,
         path: str,
         methods: t.Optional[t.List[str]] = None,
         name: t.Optional[str] = None,
         include_in_schema: bool = True,
         root: t.Optional["Flama"] = None,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> t.Callable[[types.HTTPHandler], types.HTTPHandler]:
         """Decorator version for registering a new HTTP route in this router under given path.
 
         :param path: URL path.
         :param methods: List of valid HTTP methods (only applies for routes).
         :param name: Endpoint or route name.
         :param include_in_schema: True if this route or endpoint should be declared as part of the API schema.
         :param root: Flama application.
         :param tags: Tags to add to the endpoint.
         :return: Decorated route.
         """
 
         def decorator(func: types.HTTPHandler) -> types.HTTPHandler:
             self.add_route(
-                path, func, methods=methods, name=name, include_in_schema=include_in_schema, root=root, **tags
+                path, func, methods=methods, name=name, include_in_schema=include_in_schema, root=root, tags=tags
             )
             return func
 
         return decorator
 
     def add_websocket_route(
         self,
         path: t.Optional[str] = None,
         endpoint: t.Optional[types.WebSocketHandler] = None,
         name: t.Optional[str] = None,
         route: t.Optional[WebSocketRoute] = None,
         root: t.Optional["Flama"] = None,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> WebSocketRoute:
         """Register a new websocket route in this router under given path.
 
         :param path: URL path.
         :param endpoint: Websocket function or endpoint.
         :param name: Websocket route name.
         :param route: Specific route class.
         :param root: Flama application.
         :param tags: Tags to add to the websocket route.
         :return: Websocket route.
         """
         if path is not None and endpoint is not None:
-            route = WebSocketRoute(path, endpoint=endpoint, name=name, **tags)
+            route = WebSocketRoute(path, endpoint=endpoint, name=name, tags=tags)
 
         assert route is not None, "Either 'path' and 'endpoint' or 'route' variables are needed"
 
         self.routes.append(route)
 
         route.build(root)
 
         return route
 
     def websocket_route(
         self,
         path: str,
         name: t.Optional[str] = None,
         root: t.Optional["Flama"] = None,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> t.Callable[[types.WebSocketHandler], types.WebSocketHandler]:
         """Decorator version for registering a new websocket route in this router under given path.
 
         :param path: URL path.
         :param name: Websocket route name.
         :param root: Flama application.
         :param tags: Tags to add to the websocket route.
         :return: Decorated websocket route.
         """
 
         def decorator(func: types.WebSocketHandler) -> types.WebSocketHandler:
-            self.add_websocket_route(path, func, name=name, root=root, **tags)
+            self.add_websocket_route(path, func, name=name, root=root, tags=tags)
             return func
 
         return decorator
 
     def mount(
         self,
         path: t.Optional[str] = None,
         app: t.Optional[types.App] = None,
         name: t.Optional[str] = None,
         mount: t.Optional[Mount] = None,
         root: t.Optional["Flama"] = None,
-        **tags: t.Any,
+        tags: t.Optional[t.Dict[str, types.Tag]] = None,
     ) -> Mount:
         """Register a new mount point containing an ASGI app in this router under given path.
 
         :param path: URL path.
         :param app: ASGI app to mount.
         :param name: Route name.
         :param mount: Mount.
         :param root: Flama application.
         :param tags: Tags to add to the mount.
         :return: Mount.
         """
         if path is not None and app is not None:
-            mount = Mount(path, app=app, name=name, **tags)
+            mount = Mount(path, app=app, name=name, tags=tags)
 
         assert mount is not None, "Either 'path' and 'app' or 'mount' variables are needed"
 
         self.routes.append(mount)
 
         mount.build(root)
```

### Comparing `flama-1.3.0/flama/schemas/__init__.py` & `flama-1.4.0/flama/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/schemas/_libs/marshmallow/adapter.py` & `flama-1.4.0/flama/schemas/_libs/marshmallow/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from apispec import APISpec
 from apispec.ext.marshmallow import MarshmallowPlugin, resolve_schema_cls
 
 from flama.injection import Parameter
 from flama.schemas._libs.marshmallow.fields import MAPPING
 from flama.schemas.adapter import Adapter
 from flama.schemas.exceptions import SchemaGenerationError, SchemaValidationError
-from flama.types.schema import JSONSchema
+from flama.types import JSONSchema
 
 if sys.version_info < (3, 10):  # PORT: Remove when stop supporting 3.9 # pragma: no cover
     from typing_extensions import TypeGuard
 
     t.TypeGuard = TypeGuard
 
 if t.TYPE_CHECKING:
```

### Comparing `flama-1.3.0/flama/schemas/_libs/marshmallow/schemas.py` & `flama-1.4.0/flama/schemas/_libs/marshmallow/schemas.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/schemas/_libs/pydantic/adapter.py` & `flama-1.4.0/flama/schemas/_libs/pydantic/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pydantic
 from pydantic.fields import ModelField
 from pydantic.schema import field_schema, model_schema
 
 from flama.injection import Parameter
 from flama.schemas.adapter import Adapter
 from flama.schemas.exceptions import SchemaGenerationError, SchemaValidationError
-from flama.types.schema import JSONSchema
+from flama.types import JSONSchema
 
 if sys.version_info < (3, 10):  # PORT: Remove when stop supporting 3.9 # pragma: no cover
     from typing_extensions import TypeGuard
 
     t.TypeGuard = TypeGuard
 
 __all__ = ["PydanticAdapter"]
```

### Comparing `flama-1.3.0/flama/schemas/_libs/pydantic/schemas.py` & `flama-1.4.0/flama/schemas/_libs/pydantic/schemas.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/schemas/_libs/typesystem/adapter.py` & `flama-1.4.0/flama/schemas/_libs/typesystem/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import typesystem
 
 from flama.injection import Parameter
 from flama.schemas._libs.typesystem.fields import MAPPING
 from flama.schemas.adapter import Adapter
 from flama.schemas.exceptions import SchemaGenerationError, SchemaValidationError
-from flama.types.schema import JSONSchema
+from flama.types import JSONSchema
 
 if sys.version_info < (3, 10):  # PORT: Remove when stop supporting 3.9 # pragma: no cover
     from typing_extensions import TypeGuard
 
     t.TypeGuard = TypeGuard
 
 __all__ = ["TypesystemAdapter"]
```

### Comparing `flama-1.3.0/flama/schemas/_libs/typesystem/schemas.py` & `flama-1.4.0/flama/schemas/_libs/typesystem/schemas.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/schemas/adapter.py` & `flama-1.4.0/flama/schemas/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 import sys
 import typing as t
 
-from flama.types.schema import JSONSchema, _T_Field, _T_Schema
+from flama.types import JSONSchema
+from flama.types.schema import _T_Field, _T_Schema
 
 if sys.version_info < (3, 10):  # PORT: Remove when stop supporting 3.9 # pragma: no cover
     from typing_extensions import TypeGuard
 
     t.TypeGuard = TypeGuard
```

### Comparing `flama-1.3.0/flama/schemas/data_structures.py` & `flama-1.4.0/flama/schemas/data_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 import enum
 import sys
 import typing as t
 
+import flama.types
 from flama import schemas, types
 from flama.injection.resolver import Parameter as InjectionParameter
 
 if sys.version_info < (3, 8):  # PORT: Remove when stop supporting 3.7 # pragma: no cover
     from typing_extensions import get_args, get_origin
 
     t.get_args = get_args
@@ -82,15 +83,15 @@
         return (
             (type_ in types.PARAMETERS_TYPES)
             or (origin is t.Union and len(args) == 2 and args[0] in types.PARAMETERS_TYPES and args[1] is NoneType)
             or (origin is list and args[0] in types.PARAMETERS_TYPES)
         )
 
     @property
-    def json_schema(self) -> types.JSONSchema:
+    def json_schema(self) -> flama.types.JSONSchema:
         return schemas.adapter.to_json_schema(self.field)
 
 
 @dataclasses.dataclass(frozen=True)
 class Schema:
     schema: t.Any = dataclasses.field(hash=False, compare=False)
 
@@ -200,22 +201,14 @@
             else:
                 schema = None
                 field = Field(self.name, self.type, required=self.required, default=self.default)
 
         object.__setattr__(self, "schema", schema)
         object.__setattr__(self, "field", field)
 
-    @property
-    def is_field(self) -> t.TypeGuard[Field]:
-        return isinstance(self.schema, Field)
-
-    @property
-    def is_schema(self) -> t.TypeGuard[Schema]:
-        return isinstance(self.schema, Schema)
-
     @classmethod
     def build(cls, type_: str, parameter: InjectionParameter):
         return {
             "path": cls._build_path_parameter,
             "query": cls._build_query_parameter,
             "body": cls._build_body_parameter,
             "response": cls._build_response_parameter,
```

### Comparing `flama-1.3.0/flama/schemas/generator.py` & `flama-1.4.0/flama/schemas/generator.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/schemas/modules.py` & `flama-1.4.0/flama/schemas/modules.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/schemas/openapi.py` & `flama-1.4.0/flama/schemas/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import dataclasses
 import typing as t
 
-from flama import types
+import flama.types
 
 __all__ = [
     "Schema",
     "Reference",
     "Contact",
     "License",
     "ExternalDocs",
@@ -28,15 +28,15 @@
     "Path",
     "Paths",
     "Components",
     "OpenAPI",
     "OpenAPISpec",
 ]
 
-Schema = t.NewType("Schema", types.JSONSchema)
+Schema = t.NewType("Schema", flama.types.JSONSchema)
 
 
 @dataclasses.dataclass(frozen=True)
 class Reference:
     ref: str
```

### Comparing `flama-1.3.0/flama/schemas/routing.py` & `flama-1.4.0/flama/schemas/routing.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/schemas/validation.py` & `flama-1.4.0/flama/schemas/validation.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/serialize/base.py` & `flama-1.4.0/flama/serialize/base.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/serialize/data_structures.py` & `flama-1.4.0/flama/serialize/data_structures.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import codecs
 import dataclasses
 import datetime
 import enum
 import importlib
 import inspect
 import json
+import logging
 import os
+import shutil
 import tarfile
 import tempfile
 import typing as t
 import uuid
 import warnings
+import weakref
 from pathlib import Path
 
 from flama.serialize.base import Serializer
 from flama.serialize.exceptions import FrameworkVersionWarning
 from flama.serialize.types import Framework
 
 __all__ = ["ModelArtifact", "Compression"]
 
+logger = logging.getLogger(__name__)
+
 
 class Compression(enum.Enum):
     fast = "gz"
     standard = "bz2"
     high = "xz"
 
 
@@ -169,21 +174,64 @@
             "extra": self.extra,
         }
 
 
 Artifacts = t.Dict[str, t.Union[str, os.PathLike]]
 
 
+class _ModelDirectory:
+    def __init__(
+        self,
+        model_file: t.Union[str, os.PathLike],
+        path: t.Optional[t.Union[str, os.PathLike]] = None,
+        delete: bool = True,
+    ):
+        """Generate a model directory from a model file.
+
+        :param model_file: Model file path.
+        :param path: Directory path. Create a temporary directory if None.
+        :return: Model directory loaded.
+        """
+        self.directory = Path(path) if path else Path(tempfile.mkdtemp())
+
+        with tarfile.open(model_file, "r") as tar:
+            tar.extractall(self.directory)
+
+        self.model = self.directory / "model"
+        self.artifacts: Artifacts = {artifact.name: artifact for artifact in self.directory.glob("artifacts/*")}
+
+        logger.debug("Model '%s' extracted in directory '%s'", model_file, self.directory)
+
+        self._finalizer = weakref.finalize(self, self._cleanup) if delete else None
+
+    def _cleanup(self):
+        logger.debug("Model directory '%s' clean", self.directory)
+        shutil.rmtree(self.directory)
+
+    def exists(self) -> bool:
+        """Check if the model directory exists.
+
+        :return: True if the directory exists.
+        """
+        return os.path.exists(self.directory)
+
+    def cleanup(self):
+        """Clean the model directory by removing it."""
+        if (self._finalizer and self._finalizer.detach()) or self.exists():
+            self._cleanup()
+
+
 @dataclasses.dataclass(frozen=True)
 class ModelArtifact:
     """ML Model wrapper to provide mechanisms for serialization and deserialization using Flama format."""
 
     model: t.Any
     meta: Metadata
     artifacts: t.Optional[Artifacts] = None
+    _directory: t.Optional[_ModelDirectory] = dataclasses.field(default=None, repr=False, compare=False)
 
     @classmethod
     def from_model(
         cls,
         model: t.Any,
         *,
         model_id: t.Optional[t.Union[str, uuid.UUID]] = None,
@@ -253,14 +301,15 @@
     ) -> None:
         """Serialize model artifact into a file.
 
         :param path: Model file path.
         :param compression: Compression type.
         :param kwargs: Keyword arguments passed to library dump method.
         """
+        logger.info("Dump model '%s'", path)
         compression = Compression[compression] if isinstance(compression, str) else compression
         with tarfile.open(path, f"w:{compression.value}") as tar:
             if self.artifacts:
                 for name, path in self.artifacts.items():
                     tar.add(path, f"artifacts/{name}")
 
             with tempfile.NamedTemporaryFile("wb") as model:
@@ -271,21 +320,19 @@
     def load(cls, path: t.Union[str, os.PathLike], **kwargs) -> "ModelArtifact":
         """Deserialize model artifact from a file.
 
         :param path: Model file path.
         :param kwargs: Keyword arguments passed to library load method.
         :return: Model artifact loaded.
         """
-        tmp = tempfile.TemporaryDirectory()
-        tmp_path = Path(tmp.name)
-
-        with tarfile.open(path, "r") as tar:
-            tar.extractall(tmp_path)
+        logger.info("Load model '%s'", path)
+        model_directory = _ModelDirectory(path)
 
-        with open(tmp_path / "model", "rb") as f:
+        with open(model_directory.model, "rb") as f:
             model_artifact = cls.from_bytes(f.read(), **kwargs)
 
         return cls(
             model=model_artifact.model,
             meta=model_artifact.meta,
-            artifacts={artifact.name: artifact for artifact in tmp_path.glob("artifacts/*")} or None,
+            artifacts=model_directory.artifacts or None,
+            _directory=model_directory,
         )
```

### Comparing `flama-1.3.0/flama/serialize/dump.py` & `flama-1.4.0/flama/serialize/dump.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/serialize/serializers/pytorch.py` & `flama-1.4.0/flama/serialize/serializers/pytorch.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/serialize/serializers/sklearn.py` & `flama-1.4.0/flama/serialize/serializers/sklearn.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import codecs
+import math
 import pickle
 import sys
 import typing as t
 import warnings
 
 from flama.serialize.base import Serializer
 from flama.serialize.types import Framework
@@ -26,13 +27,31 @@
     def load(self, model: bytes, **kwargs) -> t.Any:
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             model = pickle.loads(codecs.decode(model, "base64"))
 
         return model
 
+    def _info(self, data):
+        if isinstance(data, (int, bool, str)):
+            return data
+
+        if isinstance(data, float):
+            return None if math.isnan(data) else data
+
+        if isinstance(data, dict):
+            return {k: self._info(v) for k, v in data.items()}
+
+        if isinstance(data, (list, tuple, set)):
+            return [self._info(i) for i in data]
+
+        try:
+            return self._info(data.get_params())
+        except:  # noqa
+            return None
+
     def info(self, model: t.Any) -> t.Dict[str, t.Any]:
-        model_info: t.Dict[str, t.Any] = model.get_params()
+        model_info: t.Dict[str, t.Any] = self._info(model)
         return model_info
 
     def version(self) -> str:
         return importlib.metadata.version("scikit-learn")
```

### Comparing `flama-1.3.0/flama/serialize/serializers/tensorflow.py` & `flama-1.4.0/flama/serialize/serializers/tensorflow.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/sqlalchemy.py` & `flama-1.4.0/flama/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/templates/debug/error_404.html` & `flama-1.4.0/flama/templates/debug/error_404.html`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/templates/debug/error_500.html` & `flama-1.4.0/flama/templates/debug/error_500.html`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/templates/schemas/docs.html` & `flama-1.4.0/flama/templates/schemas/docs.html`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/types/asgi.py` & `flama-1.4.0/flama/types/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,11 +76,11 @@
 class MiddlewareAsyncClass(AppAsyncClass):
     def __init__(self, app: App, *args: P.args, **kwargs: P.kwargs):
         ...
 
 
 MiddlewareFunction = t.Callable[t.Concatenate[App, P], App]  # type: ignore[valid-type,misc]
 MiddlewareAsyncFunction = t.Callable[t.Concatenate[App, P], t.Awaitable[App]]  # type: ignore[valid-type,misc]
-Middleware = t.Union[MiddlewareClass, MiddlewareAsyncClass, MiddlewareFunction, MiddlewareAsyncFunction]
+Middleware = t.Union[t.Type[MiddlewareClass], t.Type[MiddlewareAsyncClass], MiddlewareFunction, MiddlewareAsyncFunction]
 
 HTTPHandler = t.Union[AppFunction, t.Type["endpoints.HTTPEndpoint"]]
 WebSocketHandler = t.Union[AppFunction, t.Type["endpoints.WebSocketEndpoint"]]
```

### Comparing `flama-1.3.0/flama/types/http.py` & `flama-1.4.0/flama/types/http.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/types/schema.py` & `flama-1.4.0/flama/types/schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import typing as t
 
 if sys.version_info < (3, 10):  # PORT: Remove when stop supporting 3.9 # pragma: no cover
     from typing_extensions import TypeGuard
 
     t.TypeGuard = TypeGuard
 
-__all__ = ["JSONField", "JSONSchema", "Schema", "is_schema", "is_schema"]
+__all__ = ["Schema", "is_schema"]
 
 _T_Field = t.TypeVar("_T_Field")
 _T_Schema = t.TypeVar("_T_Schema")
 
 
 def is_schema(obj: t.Any) -> t.TypeGuard[t.Type["Schema"]]:
     return inspect.isclass(obj) and issubclass(obj, Schema)
@@ -21,16 +21,12 @@
     def __eq__(self, other) -> bool:
         return is_schema(other) and self.schema == other.schema  # type: ignore[attr-defined]
 
     def __hash__(self) -> int:
         return id(self)
 
 
-class Schema(dict, metaclass=_SchemaMeta):  # type: ignore[misc]
+class Schema(dict, t.Generic[_T_Schema], metaclass=_SchemaMeta):  # type: ignore[misc]
     schema: t.ClassVar[t.Any] = None
 
-    def __class_getitem__(cls, schema_cls: _T_Schema) -> "Schema":  # type: ignore[override]
+    def __class_getitem__(cls, schema_cls: _T_Schema):  # type: ignore[override]
         return _SchemaMeta("_SchemaAlias", (Schema,), {"schema": schema_cls})  # type: ignore[return-value]
-
-
-JSONField = t.Union[str, int, float, bool, None, t.List["JSONField"], t.Dict[str, "JSONField"]]
-JSONSchema = t.Dict[str, JSONField]
```

### Comparing `flama-1.3.0/flama/url.py` & `flama-1.4.0/flama/url.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/validation.py` & `flama-1.4.0/flama/validation.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/flama/websockets.py` & `flama-1.4.0/flama/websockets.py`

 * *Files identical despite different names*

### Comparing `flama-1.3.0/pyproject.toml` & `flama-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flama"
-version = "1.3.0"
+version = "1.4.0"
 description = "Fire up your models with the flame 🔥"
 authors = [
     "José Antonio Perdiguero López <perdy@perdy.io>",
     "Miguel A. Durán Olivencia <migduroli@gmail.com>"
 ]
 maintainers = [
     "José Antonio Perdiguero López <perdy@perdy.io>",
@@ -31,15 +31,15 @@
 include = ["flama/py.typed", "flama/templates/**/*"]
 exclude = []
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 starlette = ">=0.21.0,<1.0.0"
 click = "^8.1"
-uvicorn = "^0.19"
+uvicorn = "^0.22"
 Jinja2 = "^3.1.2"
 typing-extensions = { version = "^4.4", python = "<3.10" }
 importlib-metadata = { version = "^4.2", python = "<3.8" }
 pydantic = { version = "^1.10", optional = true }
 marshmallow = { version = "^3.0", optional = true }
 python-forge = { version = "^18.6", optional = true }
 apispec = { version = "^6.0", optional = true }
@@ -68,15 +68,15 @@
 pytest-asyncio = "^0.20"
 ipython = [
     { version = "^7.0", python = ">=3.7,<3.8" },
     { version = "^8.0", python = ">=3.8" }
 ]
 isort = "^5.10"
 ruff = "^0.0.231"
-mypy = "^0.991"
+mypy = "^1.2"
 black = { version = "^22.3", extras = ["d"] }
 pre-commit = "^2.20"
 python-multipart = "^0.0.5"
 uvicorn = { version = ">=0.19.0,<1.0.0", extras = ["standard"] }
 httpx = ">=0.23,<1.0.0"
 aiosqlite = ">=0.11.0,<1.0.0"
 requests = "^2.22"
@@ -95,24 +95,18 @@
 apispec = "^6.0"
 typesystem = "^0.4"
 
 [tool.poetry.group.ml]
 optional = true
 
 [tool.poetry.group.ml.dependencies]
-numpy = [
-    { version = "^1.21.0", python = ">=3.7,<3.8" },
-    { version = "^1.23", python = ">=3.8" }
-]
-scikit-learn = [
-    { version = "^1.0.0", python = ">=3.7,<3.8" },
-    { version = "^1.1", python = ">=3.8" }
-]
-tensorflow-cpu = { version = "^2.11", python = ">=3.7,<3.11" }
-torch = { version = "^1.13", python = ">=3.7" }
+numpy = { version = "^1.23.0", python = ">=3.8" }
+scikit-learn = { version = "^1.1.0", python = ">=3.8" }
+tensorflow-cpu = { version = "^2.12.0", python = ">=3.8" }
+torch = { version = "^1.13.0", python = ">=3.8" }
 
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
@@ -206,15 +200,15 @@
     "flama/middleware.py",
     "flama/testclient.py",
 ]
 
 [tool.coverage.report]
 show_missing = true
 ignore_errors = true
-fail_under = 95
+fail_under = 90
 exclude_lines = [
     "noqa",
     "pragma: no cover",
     "pass",
     "\\.\\.\\.",
     "raise AssertionError",
     "raise NotImplementedError",
```

### Comparing `flama-1.3.0/PKG-INFO` & `flama-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flama
-Version: 1.3.0
+Version: 1.4.0
 Summary: Fire up your models with the flame 🔥
 Home-page: https://flama.dev
 License: MIT
 Keywords: machine-learning,ml,ml-ops,mlops,api,rest,restful,openapi,tensorflow,pytorch,sklearn
 Author: José Antonio Perdiguero López
 Author-email: perdy@perdy.io
 Maintainer: José Antonio Perdiguero López
@@ -37,15 +37,15 @@
 Requires-Dist: marshmallow (>=3.0,<4.0) ; extra == "marshmallow" or extra == "full"
 Requires-Dist: pydantic (>=1.10,<2.0) ; extra == "pydantic" or extra == "full"
 Requires-Dist: python-forge (>=18.6,<19.0) ; extra == "pagination" or extra == "full"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: starlette (>=0.21.0,<1.0.0)
 Requires-Dist: typesystem (>=0.4.1,<0.5.0) ; extra == "typesystem" or extra == "full"
 Requires-Dist: typing-extensions (>=4.4,<5.0) ; python_version < "3.10"
-Requires-Dist: uvicorn (>=0.19,<0.20)
+Requires-Dist: uvicorn (>=0.22,<0.23)
 Project-URL: Documentation, https://flama.dev/docs/
 Project-URL: Repository, https://github.com/vortico/flama
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://flama.dev"><img src="https://raw.githubusercontent.com/vortico/flama/master/.github/logo.png" alt='Flama'></a>
 </p>
@@ -128,15 +128,15 @@
 
 @app.route("/")
 def home():
     """
     tags:
         - Salute
     summary:
-        Returns a warming message.
+        Returns a warming message
     description:
         This is a more detailed description of the method itself.
         Here we can give all the details required and they will appear
         automatically in the auto-generated docs.
     responses:
         200:
             description: Warming hello message!
```

