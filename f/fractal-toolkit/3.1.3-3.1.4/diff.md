# Comparing `tmp/fractal-toolkit-3.1.3.tar.gz` & `tmp/fractal_toolkit-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-toolkit-3.1.3.tar", last modified: Fri Mar 31 12:24:02 2023, max compression
+gzip compressed data, was "fractal_toolkit-3.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal-toolkit-3.1.3.tar` & `fractal_toolkit-3.1.4.tar`

### file list

```diff
@@ -1,168 +1,169 @@
--rw-r--r--   0        0        0      187 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/.coveragerc
--rw-r--r--   0        0        0      100 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/.flake8
--rw-r--r--   0        0        0      943 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/.gitignore
--rw-r--r--   0        0        0      161 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/.isort.cfg
--rw-r--r--   0        0        0     1964 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1062 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/LICENSE
--rw-r--r--   0        0        0     1542 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/Makefile
--rw-r--r--   0        0        0    15008 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/README.md
--rw-r--r--   0        0        0      780 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/align_version.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/examples/basic/app/adapters/__init__.py
--rw-r--r--   0        0        0      245 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/examples/basic/app/adapters/products.py
--rw-r--r--   0        0        0      701 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/examples/basic/app/context.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/examples/basic/app/domain/__init__.py
--rw-r--r--   0        0        0      317 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/examples/basic/app/domain/products.py
--rw-r--r--   0        0        0      204 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/examples/basic/app/main.py
--rw-r--r--   0        0        0      369 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/examples/basic/app/settings.py
--rw-r--r--   0        0        0      720 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/fractal/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/fractal/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/fractal/contrib/django/__init__.py
--rw-r--r--   0        0        0     1660 2023-03-31 12:23:35.361860 fractal-toolkit-3.1.3/fractal/contrib/django/middleware.py
--rw-r--r--   0        0        0      778 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/django/projectors.py
--rw-r--r--   0        0        0     3339 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/django/repositories.py
--rw-r--r--   0        0        0       27 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/django/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/exceptions/__init__.py
--rw-r--r--   0        0        0       95 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/exceptions/error_message.py
--rw-r--r--   0        0        0     2297 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/install.py
--rw-r--r--   0        0        0       68 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/requirements.txt
--rw-r--r--   0        0        0       48 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/routers/__init__.py
--rw-r--r--   0        0        0     8979 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/routers/default.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/routers/domain/__init__.py
--rw-r--r--   0        0        0      207 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/routers/domain/models.py
--rw-r--r--   0        0        0     2931 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/routers/tokens.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/utils/__init__.py
--rw-r--r--   0        0        0      298 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/fastapi/utils/json_encoder.py
--rw-r--r--   0        0        0      216 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/cloudstorage/__init__.py
--rw-r--r--   0        0        0     2450 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/cloudstorage/repositories.py
--rw-r--r--   0        0        0       21 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/cloudstorage/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0      320 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/firestore/event_store.py
--rw-r--r--   0        0        0     5223 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/firestore/repositories.py
--rw-r--r--   0        0        0       38 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/firestore/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/pubsub/__init__.py
--rw-r--r--   0        0        0     3056 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/pubsub/event_bus.py
--rw-r--r--   0        0        0     2447 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/pubsub/projectors.py
--rw-r--r--   0        0        0       20 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/gcp/pubsub/requirements.txt
--rw-r--r--   0        0        0     1192 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/kafka/README.md
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/kafka/__init__.py
--rw-r--r--   0        0        0     1293 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/kafka/docker-compose.yml
--rw-r--r--   0        0        0     2233 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/kafka/event_bus.py
--rw-r--r--   0        0        0     1596 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/kafka/projectors.py
--rw-r--r--   0        0        0       13 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/kafka/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     3260 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/mongo/repositories.py
--rw-r--r--   0        0        0        8 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/mongo/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3176 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/rabbitmq/event_bus.py
--rw-r--r--   0        0        0     1937 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/rabbitmq/projectors.py
--rw-r--r--   0        0        0        5 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/rabbitmq/requirements.txt
--rw-r--r--   0        0        0      603 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/rabbitmq/utils.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11231 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/contrib/sqlalchemy/repositories.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/command_bus/__init__.py
--rw-r--r--   0        0        0       71 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/command_bus/command.py
--rw-r--r--   0        0        0     1077 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/command_bus/command_bus.py
--rw-r--r--   0        0        0      376 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/command_bus/command_handler.py
--rw-r--r--   0        0        0      576 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/command_bus/commands.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/__init__.py
--rw-r--r--   0        0        0      982 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/event.py
--rw-r--r--   0        0        0       52 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/event_bus.py
--rw-r--r--   0        0        0      297 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/event_projector.py
--rw-r--r--   0        0        0      907 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/event_publisher.py
--rw-r--r--   0        0        0     6377 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/event_store.py
--rw-r--r--   0        0        0      303 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/event_stream.py
--rw-r--r--   0        0        0      228 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/message.py
--rw-r--r--   0        0        0      397 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/models.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/projectors/__init__.py
--rw-r--r--   0        0        0      985 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/projectors/command_bus_projector.py
--rw-r--r--   0        0        0      588 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/projectors/event_store_projector.py
--rw-r--r--   0        0        0      769 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/projectors/print_projector.py
--rw-r--r--   0        0        0     1623 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/event_sourcing/repositories.py
--rw-r--r--   0        0        0      968 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/exceptions/__init__.py
--rw-r--r--   0        0        0     1928 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/process/__init__.py
--rw-r--r--   0        0        0      195 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/process/action.py
--rw-r--r--   0        0        0     3205 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/process/actions/__init__.py
--rw-r--r--   0        0        0     1582 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/process/actions/control_flow.py
--rw-r--r--   0        0        0      473 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/process/process.py
--rw-r--r--   0        0        0      613 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/process/process_scope.py
--rw-r--r--   0        0        0     1531 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/repositories/__init__.py
--rw-r--r--   0        0        0     1175 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/repositories/external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0     2676 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/repositories/file_repository_mixin.py
--rw-r--r--   0        0        0     1268 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/repositories/filter_repository_mixin.py
--rw-r--r--   0        0        0     2948 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/repositories/inmemory_repository_mixin.py
--rw-r--r--   0        0        0      225 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/services/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/utils/__init__.py
--rw-r--r--   0        0        0     9463 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/utils/application_context.py
--rw-r--r--   0        0        0      411 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/utils/fractal.py
--rw-r--r--   0        0        0      636 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/utils/json_encoder.py
--rw-r--r--   0        0        0      447 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/utils/loggers.py
--rw-r--r--   0        0        0     1296 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/utils/settings.py
--rw-r--r--   0        0        0     1414 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/utils/string.py
--rw-r--r--   0        0        0      144 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/fractal/core/utils/subclasses.py
--rw-r--r--   0        0        0     1660 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/pyproject.toml
--rw-r--r--   0        0        0       69 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/setup.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/__init__.py
--rw-r--r--   0        0        0       45 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/fastapi/__init__.py
--rw-r--r--   0        0        0     2158 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/fastapi/test_routers.py
--rw-r--r--   0        0        0      451 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/fastapi/test_tokens.py
--rw-r--r--   0        0        0      392 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/fastapi/test_utils.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/mongo/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11148 2023-03-31 12:23:35.365861 fractal-toolkit-3.1.3/tests/contrib/sqlalchemy/test_repositories.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/command_bus/__init__.py
--rw-r--r--   0        0        0      844 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/command_bus/test_command_bus.py
--rw-r--r--   0        0        0      113 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/command_bus/test_command_handler.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/event_sourcing/__init__.py
--rw-r--r--   0        0        0      376 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/event_sourcing/test_event_publisher.py
--rw-r--r--   0        0        0     1675 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/event_sourcing/test_event_store.py
--rw-r--r--   0        0        0      294 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/event_sourcing/test_projectors.py
--rw-r--r--   0        0        0     1529 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/event_sourcing/test_repositories.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/models/__init__.py
--rw-r--r--   0        0        0     2554 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/models/test_models.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/repositories/__init__.py
--rw-r--r--   0        0        0     1154 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/repositories/test_external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0     2248 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/repositories/test_filter_repository_mixin.py
--rw-r--r--   0        0        0     3748 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/repositories/test_inmemory_repository_mixin.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/services/__init__.py
--rw-r--r--   0        0        0      237 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/services/test_service.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/utils/__init__.py
--rw-r--r--   0        0        0     1638 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/utils/test_application_context.py
--rw-r--r--   0        0        0      850 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/utils/test_json_encoder.py
--rw-r--r--   0        0        0      542 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/utils/test_settings.py
--rw-r--r--   0        0        0      507 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/core/utils/test_string.py
--rw-r--r--   0        0        0      103 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      420 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/django/__init__.py
--rw-r--r--   0        0        0     2163 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/fastapi.py
--rw-r--r--   0        0        0       67 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/mongo/__init__.py
--rw-r--r--   0        0        0       68 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/roles/__init__.py
--rw-r--r--   0        0        0      619 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/roles/services.py
--rw-r--r--   0        0        0       77 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     7257 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/sqlalchemy/repositories.py
--rw-r--r--   0        0        0      203 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/tokens/__init__.py
--rw-r--r--   0        0        0      485 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/tokens/fractal.py
--rw-r--r--   0        0        0      195 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/tokens/services.py
--rw-r--r--   0        0        0     1388 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/contrib/tokens/utils.py
--rw-r--r--   0        0        0      363 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/core/__init__.py
--rw-r--r--   0        0        0     1048 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/core/command_bus.py
--rw-r--r--   0        0        0     3935 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/core/event_sourcing.py
--rw-r--r--   0        0        0     1230 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/core/fractal.py
--rw-r--r--   0        0        0     1389 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/core/repositories.py
--rw-r--r--   0        0        0      457 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/core/services.py
--rw-r--r--   0        0        0     1762 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tests/fixtures/core/utils.py
--rw-r--r--   0        0        0      620 2023-03-31 12:23:35.369861 fractal-toolkit-3.1.3/tox.ini
--rw-r--r--   0        0        0    15932 1970-01-01 00:00:00.000000 fractal-toolkit-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/.coveragerc
+-rw-r--r--   0        0        0      100 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/.flake8
+-rw-r--r--   0        0        0      943 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/.gitignore
+-rw-r--r--   0        0        0      161 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/.isort.cfg
+-rw-r--r--   0        0        0     1964 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1062 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/LICENSE
+-rw-r--r--   0        0        0     1563 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/Makefile
+-rw-r--r--   0        0        0    15008 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/README.md
+-rw-r--r--   0        0        0      780 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/align_version.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/examples/basic/app/adapters/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/examples/basic/app/adapters/products.py
+-rw-r--r--   0        0        0      701 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/examples/basic/app/context.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/examples/basic/app/domain/__init__.py
+-rw-r--r--   0        0        0      317 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/examples/basic/app/domain/products.py
+-rw-r--r--   0        0        0      204 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/examples/basic/app/main.py
+-rw-r--r--   0        0        0      369 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/examples/basic/app/settings.py
+-rw-r--r--   0        0        0      720 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/django/__init__.py
+-rw-r--r--   0        0        0     1660 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/django/middleware.py
+-rw-r--r--   0        0        0      778 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/django/projectors.py
+-rw-r--r--   0        0        0     3339 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/django/repositories.py
+-rw-r--r--   0        0        0       27 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/django/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/exceptions/__init__.py
+-rw-r--r--   0        0        0       95 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/exceptions/error_message.py
+-rw-r--r--   0        0        0     2297 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/install.py
+-rw-r--r--   0        0        0       68 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/requirements.txt
+-rw-r--r--   0        0        0       48 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/routers/__init__.py
+-rw-r--r--   0        0        0     8979 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/routers/default.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/routers/domain/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/routers/domain/models.py
+-rw-r--r--   0        0        0     2935 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/routers/tokens.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/utils/__init__.py
+-rw-r--r--   0        0        0      298 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/fastapi/utils/json_encoder.py
+-rw-r--r--   0        0        0      216 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/cloudstorage/__init__.py
+-rw-r--r--   0        0        0     2450 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/cloudstorage/repositories.py
+-rw-r--r--   0        0        0       21 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/cloudstorage/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/firestore/event_store.py
+-rw-r--r--   0        0        0     5223 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/firestore/repositories.py
+-rw-r--r--   0        0        0       38 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/firestore/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/pubsub/__init__.py
+-rw-r--r--   0        0        0     3056 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/pubsub/event_bus.py
+-rw-r--r--   0        0        0     2466 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/pubsub/projectors.py
+-rw-r--r--   0        0        0       20 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/gcp/pubsub/requirements.txt
+-rw-r--r--   0        0        0     1192 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/kafka/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/kafka/__init__.py
+-rw-r--r--   0        0        0     1293 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/kafka/docker-compose.yml
+-rw-r--r--   0        0        0     2233 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/kafka/event_bus.py
+-rw-r--r--   0        0        0     1670 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/kafka/projectors.py
+-rw-r--r--   0        0        0       13 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/kafka/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     3260 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/mongo/repositories.py
+-rw-r--r--   0        0        0        8 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/mongo/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3176 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/rabbitmq/event_bus.py
+-rw-r--r--   0        0        0     2011 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/rabbitmq/projectors.py
+-rw-r--r--   0        0        0        5 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/rabbitmq/requirements.txt
+-rw-r--r--   0        0        0      603 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/rabbitmq/utils.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11231 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/contrib/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/core/command_bus/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/core/command_bus/command.py
+-rw-r--r--   0        0        0     1077 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/core/command_bus/command_bus.py
+-rw-r--r--   0        0        0      376 2023-06-07 11:59:35.703293 fractal_toolkit-3.1.4/fractal/core/command_bus/command_handler.py
+-rw-r--r--   0        0        0      576 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/command_bus/commands.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/__init__.py
+-rw-r--r--   0        0        0      982 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/event.py
+-rw-r--r--   0        0        0       52 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/event_bus.py
+-rw-r--r--   0        0        0      297 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/event_projector.py
+-rw-r--r--   0        0        0      907 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/event_publisher.py
+-rw-r--r--   0        0        0     6423 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/event_store.py
+-rw-r--r--   0        0        0      303 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/event_stream.py
+-rw-r--r--   0        0        0      274 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/message.py
+-rw-r--r--   0        0        0      397 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/models.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/projectors/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/projectors/command_bus_projector.py
+-rw-r--r--   0        0        0      588 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/projectors/event_store_projector.py
+-rw-r--r--   0        0        0      769 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/projectors/print_projector.py
+-rw-r--r--   0        0        0     1623 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/event_sourcing/repositories.py
+-rw-r--r--   0        0        0      968 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     1928 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/process/__init__.py
+-rw-r--r--   0        0        0      195 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/process/action.py
+-rw-r--r--   0        0        0     3752 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/process/actions/__init__.py
+-rw-r--r--   0        0        0     1671 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/process/actions/control_flow.py
+-rw-r--r--   0        0        0      473 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/process/process.py
+-rw-r--r--   0        0        0      613 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/process/process_scope.py
+-rw-r--r--   0        0        0     1531 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/repositories/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/repositories/external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0     2676 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/repositories/file_repository_mixin.py
+-rw-r--r--   0        0        0     1268 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/repositories/filter_repository_mixin.py
+-rw-r--r--   0        0        0     2948 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/repositories/inmemory_repository_mixin.py
+-rw-r--r--   0        0        0      225 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/utils/__init__.py
+-rw-r--r--   0        0        0     9463 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/utils/application_context.py
+-rw-r--r--   0        0        0      411 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/utils/fractal.py
+-rw-r--r--   0        0        0      636 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/utils/json_encoder.py
+-rw-r--r--   0        0        0      447 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/utils/loggers.py
+-rw-r--r--   0        0        0     1296 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/utils/settings.py
+-rw-r--r--   0        0        0     1414 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/utils/string.py
+-rw-r--r--   0        0        0      144 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/core/utils/subclasses.py
+-rw-r--r--   0        0        0       77 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/fractal/py.typed
+-rw-r--r--   0        0        0     1688 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/setup.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/__init__.py
+-rw-r--r--   0        0        0       45 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/fastapi/__init__.py
+-rw-r--r--   0        0        0     2158 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/fastapi/test_routers.py
+-rw-r--r--   0        0        0      451 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/fastapi/test_tokens.py
+-rw-r--r--   0        0        0      392 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/fastapi/test_utils.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11148 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/contrib/sqlalchemy/test_repositories.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/command_bus/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/command_bus/test_command_bus.py
+-rw-r--r--   0        0        0      113 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/command_bus/test_command_handler.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/event_sourcing/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/event_sourcing/test_event_publisher.py
+-rw-r--r--   0        0        0     1675 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/event_sourcing/test_event_store.py
+-rw-r--r--   0        0        0      294 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/event_sourcing/test_projectors.py
+-rw-r--r--   0        0        0     1529 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/event_sourcing/test_repositories.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/models/__init__.py
+-rw-r--r--   0        0        0     2554 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/models/test_models.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/repositories/__init__.py
+-rw-r--r--   0        0        0     1154 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/repositories/test_external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0     2248 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/repositories/test_filter_repository_mixin.py
+-rw-r--r--   0        0        0     3748 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/repositories/test_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/services/__init__.py
+-rw-r--r--   0        0        0      237 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/services/test_service.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/utils/__init__.py
+-rw-r--r--   0        0        0     1638 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/utils/test_application_context.py
+-rw-r--r--   0        0        0      850 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/utils/test_json_encoder.py
+-rw-r--r--   0        0        0      542 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/utils/test_settings.py
+-rw-r--r--   0        0        0      507 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/core/utils/test_string.py
+-rw-r--r--   0        0        0      103 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      420 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2163 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/fastapi.py
+-rw-r--r--   0        0        0       67 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/roles/__init__.py
+-rw-r--r--   0        0        0      619 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/roles/services.py
+-rw-r--r--   0        0        0       77 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     7257 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0      203 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/tokens/__init__.py
+-rw-r--r--   0        0        0      485 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/tokens/fractal.py
+-rw-r--r--   0        0        0      195 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/tokens/services.py
+-rw-r--r--   0        0        0     1388 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/contrib/tokens/utils.py
+-rw-r--r--   0        0        0      363 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/core/__init__.py
+-rw-r--r--   0        0        0     1048 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/core/command_bus.py
+-rw-r--r--   0        0        0     3935 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/core/event_sourcing.py
+-rw-r--r--   0        0        0     1230 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/core/fractal.py
+-rw-r--r--   0        0        0     1389 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/core/repositories.py
+-rw-r--r--   0        0        0      457 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/core/services.py
+-rw-r--r--   0        0        0     1781 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tests/fixtures/core/utils.py
+-rw-r--r--   0        0        0      645 2023-06-07 11:59:35.707293 fractal_toolkit-3.1.4/tox.ini
+-rw-r--r--   0        0        0    15968 1970-01-01 00:00:00.000000 fractal_toolkit-3.1.4/PKG-INFO
```

### Comparing `fractal-toolkit-3.1.3/.github/workflows/build.yml` & `fractal_toolkit-3.1.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/.github/workflows/publish.yml` & `fractal_toolkit-3.1.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/.gitignore` & `fractal_toolkit-3.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/.pre-commit-config.yaml` & `fractal_toolkit-3.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/LICENSE` & `fractal_toolkit-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/Makefile` & `fractal_toolkit-3.1.4/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 coverage:  ## Run tests with coverage
 	rm .coverage ||:
 	rm coverage.xml ||:
 	pytest --cov fractal --cov-report=xml
 
 deps:  ## Install dependencies
 	python -m pip install --upgrade pip
-	python -m pip install autoflake black coverage django fastapi flake8 flit fractal-roles fractal-specifications fractal-tokens httpx isort mccabe mypy pre-commit pylint pytest pytest-cov pytest-asyncio pytest-lazy-fixture python-dotenv python-jose requests 'sqlalchemy<2.0' tox tox-gh-actions
+	python -m pip install autoflake black coverage django fastapi flake8 flit fractal-repositories fractal-roles fractal-specifications fractal-tokens httpx isort mccabe mypy pre-commit pylint pytest pytest-cov pytest-asyncio pytest-lazy-fixture python-dotenv python-jose requests 'sqlalchemy<2.0' tox tox-gh-actions
 	python -m pip install cryptography
 
 lint:  ## Lint and static-check
 	pre-commit run --all-files
 
 publish:  ## Publish to PyPi
 	python -m flit publish
```

### Comparing `fractal-toolkit-3.1.3/README.md` & `fractal_toolkit-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/align_version.py` & `fractal_toolkit-3.1.4/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/examples/basic/app/context.py` & `fractal_toolkit-3.1.4/examples/basic/app/context.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/__init__.py` & `fractal_toolkit-3.1.4/fractal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Fractal is a scaffolding toolkit for building SOLID logic for your Python applications."""
 
-__version__ = "3.1.3"
+__version__ = "3.1.4"
 
 from abc import ABC
 
 from fractal.core.utils.application_context import ApplicationContext
 from fractal.core.utils.settings import Settings
```

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/django/middleware.py` & `fractal_toolkit-3.1.4/fractal/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/django/projectors.py` & `fractal_toolkit-3.1.4/fractal/contrib/django/projectors.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/django/repositories.py` & `fractal_toolkit-3.1.4/fractal/contrib/django/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/fastapi/install.py` & `fractal_toolkit-3.1.4/fractal/contrib/fastapi/install.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/fastapi/routers/default.py` & `fractal_toolkit-3.1.4/fractal/contrib/fastapi/routers/default.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/fastapi/routers/tokens.py` & `fractal_toolkit-3.1.4/fractal/contrib/fastapi/routers/tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import List, Optional
 
 from fastapi import Depends
 from fastapi.security import OAuth2PasswordBearer
 from fractal_roles.models import Role, TokenPayloadRolesMixin
 from fractal_roles.services import RolesService as BaseRolesService
 from fractal_tokens.services.dummy import DummyJsonTokenService
+from fractal_tokens.services.generic import TokenPayload as BaseTokenPayload
 from fractal_tokens.services.generic import TokenService
-from fractal_tokens.services.jwt import TokenPayload as BaseTokenPayload
 from fractal_tokens.services.jwt.automatic import AutomaticJwtTokenService
 
 from fractal import ApplicationContext, Fractal
 from fractal.core.models import Model
 from fractal.core.services import Service
 
 oauth2_scheme = OAuth2PasswordBearer(tokenUrl="login")
```

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/gcp/cloudstorage/repositories.py` & `fractal_toolkit-3.1.4/fractal/contrib/gcp/cloudstorage/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/gcp/firestore/repositories.py` & `fractal_toolkit-3.1.4/fractal/contrib/gcp/firestore/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/gcp/pubsub/event_bus.py` & `fractal_toolkit-3.1.4/fractal/contrib/gcp/pubsub/event_bus.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/gcp/pubsub/projectors.py` & `fractal_toolkit-3.1.4/fractal/contrib/gcp/pubsub/projectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 from dataclasses import asdict
-from datetime import datetime
+from datetime import datetime, timezone
 from json import JSONEncoder
 from typing import Optional, Type
 
 from google.cloud import pubsub_v1
 
 from fractal.core.event_sourcing.event import BasicSendingEvent
 from fractal.core.event_sourcing.event_projector import EventProjector
@@ -43,15 +43,15 @@
             for t in self.publisher.list_topics(request={"project": self.project_path})
         ]:
             logger.error(f"Topic doesn't exist '{topic_path}'")
 
         # Wrap event in a message
         message = Message(
             id=id,
-            occurred_on=datetime.utcnow(),
+            occurred_on=datetime.now(timezone.utc),
             event=event.__class__.__name__,
             data=json.dumps(asdict(event), cls=self.json_encoder),
             object_id=event.object_id,
             aggregate_root_id=event.aggregate_root_id,
         )
 
         # Data must be a bytestring
```

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/kafka/README.md` & `fractal_toolkit-3.1.4/fractal/contrib/kafka/README.md`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/kafka/docker-compose.yml` & `fractal_toolkit-3.1.4/fractal/contrib/kafka/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/kafka/event_bus.py` & `fractal_toolkit-3.1.4/fractal/contrib/kafka/event_bus.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/kafka/projectors.py` & `fractal_toolkit-3.1.4/fractal/contrib/kafka/projectors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 from dataclasses import asdict
-from datetime import datetime
+from datetime import datetime, timezone
 from json import JSONEncoder
 from typing import List, Type
 
 from kafka import KafkaProducer
 
 from fractal.core.event_sourcing.event import BasicSendingEvent
 from fractal.core.event_sourcing.event_projector import EventProjector
@@ -34,18 +34,19 @@
 
     def project(self, id: str, event: BasicSendingEvent):
         if type(event) not in self.event_classes:
             return
 
         message = Message(
             id=id,
-            occurred_on=datetime.utcnow(),
+            occurred_on=datetime.now(timezone.utc),
             event=event.__class__.__name__,
             data=json.dumps(asdict(event), cls=self.json_encoder),
             object_id=event.object_id,
+            aggregate_root_id=event.aggregate_root_id,
         )
 
         producer = KafkaProducer(bootstrap_servers=self.bootstrap_servers)
         producer.send(
             f"{self.service_name}.{self.aggregate}",
             json.dumps(asdict(message), cls=self.json_encoder).encode(),
         )
```

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/mongo/repositories.py` & `fractal_toolkit-3.1.4/fractal/contrib/mongo/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/rabbitmq/event_bus.py` & `fractal_toolkit-3.1.4/fractal/contrib/rabbitmq/event_bus.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/rabbitmq/projectors.py` & `fractal_toolkit-3.1.4/fractal/contrib/rabbitmq/projectors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 from dataclasses import asdict
-from datetime import datetime
+from datetime import datetime, timezone
 from json import JSONEncoder
 from typing import List, Type
 
 import pika
 
 from fractal.contrib.rabbitmq.utils import setup_rabbitmq_connection
 from fractal.core.event_sourcing.event import BasicSendingEvent
@@ -38,18 +38,19 @@
                 exchange_type="fanout",
                 durable=True,
             )
 
     def project(self, id: str, event: BasicSendingEvent):
         message = Message(
             id=id,
-            occurred_on=datetime.utcnow(),
+            occurred_on=datetime.now(timezone.utc),
             event=event.__class__.__name__,
             data=json.dumps(asdict(event), cls=self.json_encoder),
             object_id=event.object_id,
+            aggregate_root_id=event.aggregate_root_id,
         )
 
         self.channel.basic_publish(
             exchange=message.event,
             routing_key="",
             body=json.dumps(asdict(message), cls=self.json_encoder).encode(),
             properties=pika.BasicProperties(
```

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/rabbitmq/utils.py` & `fractal_toolkit-3.1.4/fractal/contrib/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/contrib/sqlalchemy/repositories.py` & `fractal_toolkit-3.1.4/fractal/contrib/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/command_bus/command_bus.py` & `fractal_toolkit-3.1.4/fractal/core/command_bus/command_bus.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/command_bus/commands.py` & `fractal_toolkit-3.1.4/fractal/core/command_bus/commands.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/event_sourcing/event.py` & `fractal_toolkit-3.1.4/fractal/core/event_sourcing/event.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/event_sourcing/event_publisher.py` & `fractal_toolkit-3.1.4/fractal/core/event_sourcing/event_publisher.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/event_sourcing/event_store.py` & `fractal_toolkit-3.1.4/fractal/core/event_sourcing/event_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 from abc import ABC, abstractmethod
 from dataclasses import asdict
-from datetime import datetime
+from datetime import datetime, timezone
 from json import JSONEncoder
 from typing import List, Optional, Type
 
 from fractal_specifications.generic.specification import Specification
 
 from fractal.core.event_sourcing.event import BasicSendingEvent
 from fractal.core.event_sourcing.event_stream import EventStream
@@ -60,15 +60,15 @@
 
 class ObjectEventStore(BasicEventStore):
     def commit(self, event_stream: EventStream, aggregate: str, version: int):
         for event in event_stream.events:
             self.event_store_repository.add(
                 Message(
                     id=str(uuid.uuid4()),
-                    occurred_on=datetime.utcnow(),
+                    occurred_on=datetime.now(timezone.utc),
                     event=event.__class__.__name__,
                     data=event,
                     object_id=event.object_id,
                     aggregate_root_id=event.aggregate_root_id,
                 )
             )
 
@@ -92,15 +92,15 @@
         self.events = {e.__name__: e for e in events}
 
     def commit(self, event_stream: EventStream, aggregate: str, version: int):
         for event in event_stream.events:
             self.event_store_repository.add(
                 Message(
                     id=str(uuid.uuid4()),
-                    occurred_on=datetime.utcnow(),
+                    occurred_on=datetime.now(timezone.utc),
                     event=event.__class__.__name__,
                     data=asdict(event),
                     object_id=event.object_id,
                     aggregate_root_id=event.aggregate_root_id,
                 )
             )
 
@@ -130,15 +130,15 @@
     def commit(self, event_stream: EventStream, aggregate: str, version: int):
         import json
 
         for event in event_stream.events:
             self.event_store_repository.add(
                 Message(
                     id=str(uuid.uuid4()),
-                    occurred_on=datetime.utcnow(),
+                    occurred_on=datetime.now(timezone.utc),
                     event=event.__class__.__name__,
                     data=json.dumps(asdict(event), cls=self.json_encoder),
                     object_id=event.object_id,
                     aggregate_root_id=event.aggregate_root_id,
                 )
             )
 
@@ -168,15 +168,15 @@
     def commit(self, event_stream: EventStream, aggregate: str, version: int):
         import pickle
 
         for event in event_stream.events:
             self.event_store_repository.add(
                 Message(
                     id=str(uuid.uuid4()),
-                    occurred_on=datetime.utcnow(),
+                    occurred_on=datetime.now(timezone.utc),
                     event=event.__class__.__name__,
                     data=pickle.dumps(event),
                     object_id=event.object_id,
                     aggregate_root_id=event.aggregate_root_id,
                 )
             )
```

### Comparing `fractal-toolkit-3.1.3/fractal/core/event_sourcing/projectors/command_bus_projector.py` & `fractal_toolkit-3.1.4/fractal/core/event_sourcing/projectors/command_bus_projector.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/event_sourcing/projectors/event_store_projector.py` & `fractal_toolkit-3.1.4/fractal/core/event_sourcing/projectors/event_store_projector.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/event_sourcing/projectors/print_projector.py` & `fractal_toolkit-3.1.4/fractal/core/event_sourcing/projectors/print_projector.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/event_sourcing/repositories.py` & `fractal_toolkit-3.1.4/fractal/core/event_sourcing/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/exceptions/__init__.py` & `fractal_toolkit-3.1.4/fractal/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/models/__init__.py` & `fractal_toolkit-3.1.4/fractal/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/process/process_scope.py` & `fractal_toolkit-3.1.4/fractal/core/process/process_scope.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/repositories/__init__.py` & `fractal_toolkit-3.1.4/fractal/core/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/repositories/external_data_inmemory_repository_mixin.py` & `fractal_toolkit-3.1.4/fractal/core/repositories/external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/repositories/file_repository_mixin.py` & `fractal_toolkit-3.1.4/fractal/core/repositories/file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/repositories/filter_repository_mixin.py` & `fractal_toolkit-3.1.4/fractal/core/repositories/filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/repositories/inmemory_repository_mixin.py` & `fractal_toolkit-3.1.4/fractal/core/repositories/inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/utils/application_context.py` & `fractal_toolkit-3.1.4/fractal/core/utils/application_context.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/utils/json_encoder.py` & `fractal_toolkit-3.1.4/fractal/core/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/utils/settings.py` & `fractal_toolkit-3.1.4/fractal/core/utils/settings.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/fractal/core/utils/string.py` & `fractal_toolkit-3.1.4/fractal/core/utils/string.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/pyproject.toml` & `fractal_toolkit-3.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-toolkit"
-version = "3.1.3"
+version = "3.1.4"
 description = "Fractal is a scaffolding toolkit for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
 
@@ -21,14 +21,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
 ]
 description-file = "README.md"
 requires = [
+    "fractal-repositories",
     "fractal-roles",
     "fractal-specifications",
     "fractal-tokens",
     "python-dotenv",
 ]
 requires-python=">=3.8"
```

### Comparing `fractal-toolkit-3.1.3/tests/contrib/fastapi/test_routers.py` & `fractal_toolkit-3.1.4/tests/contrib/fastapi/test_routers.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/contrib/sqlalchemy/test_repositories.py` & `fractal_toolkit-3.1.4/tests/contrib/sqlalchemy/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/command_bus/test_command_bus.py` & `fractal_toolkit-3.1.4/tests/core/command_bus/test_command_bus.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/event_sourcing/test_event_store.py` & `fractal_toolkit-3.1.4/tests/core/event_sourcing/test_event_store.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/event_sourcing/test_repositories.py` & `fractal_toolkit-3.1.4/tests/core/event_sourcing/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/models/test_models.py` & `fractal_toolkit-3.1.4/tests/core/models/test_models.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/repositories/test_external_data_inmemory_repository_mixin.py` & `fractal_toolkit-3.1.4/tests/core/repositories/test_external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/repositories/test_filter_repository_mixin.py` & `fractal_toolkit-3.1.4/tests/core/repositories/test_filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/repositories/test_inmemory_repository_mixin.py` & `fractal_toolkit-3.1.4/tests/core/repositories/test_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/utils/test_application_context.py` & `fractal_toolkit-3.1.4/tests/core/utils/test_application_context.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/utils/test_json_encoder.py` & `fractal_toolkit-3.1.4/tests/core/utils/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/core/utils/test_settings.py` & `fractal_toolkit-3.1.4/tests/core/utils/test_settings.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/fixtures/contrib/fastapi.py` & `fractal_toolkit-3.1.4/tests/fixtures/contrib/fastapi.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/fixtures/contrib/roles/services.py` & `fractal_toolkit-3.1.4/tests/fixtures/contrib/roles/services.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/fixtures/contrib/sqlalchemy/repositories.py` & `fractal_toolkit-3.1.4/tests/fixtures/contrib/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/fixtures/contrib/tokens/utils.py` & `fractal_toolkit-3.1.4/tests/fixtures/contrib/tokens/utils.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/fixtures/core/command_bus.py` & `fractal_toolkit-3.1.4/tests/fixtures/core/command_bus.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/fixtures/core/event_sourcing.py` & `fractal_toolkit-3.1.4/tests/fixtures/core/event_sourcing.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/fixtures/core/fractal.py` & `fractal_toolkit-3.1.4/tests/fixtures/core/fractal.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/fixtures/core/repositories.py` & `fractal_toolkit-3.1.4/tests/fixtures/core/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-toolkit-3.1.3/tests/fixtures/core/utils.py` & `fractal_toolkit-3.1.4/tests/fixtures/core/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from datetime import datetime
+from datetime import datetime, timezone
 
 import pytest
 
 
 @pytest.fixture
 def settings_class():
     from fractal.core.utils.settings import Settings
@@ -59,8 +59,8 @@
         settings = settings_class()
 
     return EmptyApplicationContext()
 
 
 @pytest.fixture
 def now():
-    return datetime.utcnow()
+    return datetime.now(timezone.utc)
```

### Comparing `fractal-toolkit-3.1.3/tox.ini` & `fractal_toolkit-3.1.4/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 deps =
     black
     coverage
     cryptography
     django
     fastapi
     flake8
+    fractal-repositories
     fractal-roles
     fractal-specifications
     fractal-tokens
     httpx
     isort
     mccabe
     mypy
```

### Comparing `fractal-toolkit-3.1.3/PKG-INFO` & `fractal_toolkit-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: fractal-toolkit
-Version: 3.1.3
+Version: 3.1.4
 Summary: Fractal is a scaffolding toolkit for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
+Requires-Dist: fractal-repositories
 Requires-Dist: fractal-roles
 Requires-Dist: fractal-specifications
 Requires-Dist: fractal-tokens
 Requires-Dist: python-dotenv
 Requires-Dist: black ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: isort ; extra == "test"
```

