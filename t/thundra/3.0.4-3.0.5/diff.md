# Comparing `tmp/thundra-3.0.4.tar.gz` & `tmp/thundra-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thundra-3.0.4.tar", last modified: Tue Jun  6 06:54:02 2023, max compression
+gzip compressed data, was "thundra-3.0.5.tar", last modified: Thu Jun  8 12:21:41 2023, max compression
```

## Comparing `thundra-3.0.4.tar` & `thundra-3.0.5.tar`

### file list

```diff
@@ -1,250 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.372961 thundra-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-06 06:53:44.000000 thundra-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 06:54:02.372961 thundra-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30786 2023-06-06 06:53:44.000000 thundra-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.348961 thundra-3.0.4/foresight/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.348961 thundra-3.0.4/foresight/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/constants/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.348961 thundra-3.0.4/foresight/context/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/context/test_case_execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/context/test_suite_execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.348961 thundra-3.0.4/foresight/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.348961 thundra-3.0.4/foresight/environment/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/azure/azure_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.348961 thundra-3.0.4/foresight/environment/bitbucket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/bitbucket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/bitbucket/bitbucket_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.348961 thundra-3.0.4/foresight/environment/circleci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/circleci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/circleci/circleci_environment_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/environment_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/environment_info_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.348961 thundra-3.0.4/foresight/environment/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/git/git_env_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/git/git_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/git/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.348961 thundra-3.0.4/foresight/environment/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/github/github_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.352961 thundra-3.0.4/foresight/environment/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/gitlab/gitlab_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.352961 thundra-3.0.4/foresight/environment/jenkins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/jenkins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/jenkins/jenkins_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.352961 thundra-3.0.4/foresight/environment/travisci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/travisci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/environment/travisci/travisci_environment_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/foresight_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.352961 thundra-3.0.4/foresight/model/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/model/terminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/model/test_run_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/model/test_run_finish.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/model/test_run_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/model/test_run_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/model/test_run_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/model/test_run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.352961 thundra-3.0.4/foresight/pytest_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/pytest_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/pytest_integration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/pytest_integration/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/pytest_integration/pytest_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/pytest_integration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.352961 thundra-3.0.4/foresight/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/sampler/max_count_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/test_runner_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/test_runner_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/test_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.352961 thundra-3.0.4/foresight/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/utils/handler_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/utils/test_runner_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-06 06:53:44.000000 thundra-3.0.4/foresight/utils/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 06:54:02.372961 thundra-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-06 06:53:44.000000 thundra-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.352961 thundra-3.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-06 06:53:44.000000 thundra-3.0.4/tests/test_application_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-06-06 06:53:44.000000 thundra-3.0.4/tests/test_lambda_event_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-06 06:53:44.000000 thundra-3.0.4/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-06 06:53:44.000000 thundra-3.0.4/tests/test_thundra_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-06 06:53:44.000000 thundra-3.0.4/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.356962 thundra-3.0.4/thundra/
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.356962 thundra-3.0.4/thundra/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/application/application_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/application/application_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/application/global_application_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/composite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.356962 thundra-3.0.4/thundra/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/config/config_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/config/config_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/config/config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    20828 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.356962 thundra-3.0.4/thundra/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/context/context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/context/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/context/execution_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/context/global_execution_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/context/plugin_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/context/tracing_execution_context_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.356962 thundra-3.0.4/thundra/debug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/debug/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.360962 thundra-3.0.4/thundra/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.360962 thundra-3.0.4/thundra/integrations/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/aiohttp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/base_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    38459 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/botocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.360962 thundra-3.0.4/thundra/integrations/handler_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/handler_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/handler_wrappers/chalice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.360962 thundra-3.0.4/thundra/integrations/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/botocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/django.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/modules/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/postgre.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/rdb_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/integrations/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.364961 thundra-3.0.4/thundra/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/listeners/composite_span_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/listeners/error_injector_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/listeners/filtering_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/listeners/latency_injector_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/listeners/security_aware_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/listeners/tag_injector_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/listeners/thundra_span_filterer.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/listeners/thundra_span_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.364961 thundra-3.0.4/thundra/opentracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/opentracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.364961 thundra-3.0.4/thundra/opentracing/propagation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/opentracing/propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/opentracing/propagation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/opentracing/propagation/propagator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/opentracing/propagation/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/opentracing/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/opentracing/span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/opentracing/span_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/opentracing/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.364961 thundra-3.0.4/thundra/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.364961 thundra-3.0.4/thundra/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/config/base_plugin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/config/log_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/config/metric_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/config/thundra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/config/trace_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.364961 thundra-3.0.4/thundra/plugins/invocation/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/invocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/invocation/invocation_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/invocation/invocation_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/invocation/invocation_trace_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.364961 thundra-3.0.4/thundra/plugins/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/log/log_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/log/log_support.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/log/thundra_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/log/thundra_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.364961 thundra-3.0.4/thundra/plugins/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/metric/metric_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/metric/metric_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.364961 thundra-3.0.4/thundra/plugins/trace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/trace/patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/trace/trace_aware_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/trace/trace_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/trace/trace_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/plugins/trace/traceable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.368961 thundra-3.0.4/thundra/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/samplers/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/samplers/composite_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/samplers/count_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/samplers/duration_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/samplers/error_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/samplers/time_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/thundra_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.368961 thundra-3.0.4/thundra/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.368961 thundra-3.0.4/thundra/wrappers/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/aws_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/aws_lambda/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/aws_lambda/lambda_application_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/aws_lambda/lambda_event_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/aws_lambda/lambda_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/aws_lambda/lambda_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/base_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.368961 thundra-3.0.4/thundra/wrappers/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/django/django_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/django/django_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.368961 thundra-3.0.4/thundra/wrappers/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/fastapi/fastapi_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/fastapi/fastapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/fastapi/fastapi_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/fastapi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.368961 thundra-3.0.4/thundra/wrappers/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/flask/flask_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/flask/flask_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/flask/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.368961 thundra-3.0.4/thundra/wrappers/tornado/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/tornado/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/tornado/tornado_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/tornado/tornado_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/web_wrapper_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/wrapper_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-06 06:53:44.000000 thundra-3.0.4/thundra/wrappers/wrapper_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:54:02.356962 thundra-3.0.4/thundra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 06:54:02.000000 thundra-3.0.4/thundra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-06 06:54:02.000000 thundra-3.0.4/thundra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:54:02.000000 thundra-3.0.4/thundra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 06:54:02.000000 thundra-3.0.4/thundra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-06 06:54:02.000000 thundra-3.0.4/thundra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 06:54:02.000000 thundra-3.0.4/thundra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:54:02.000000 thundra-3.0.4/thundra.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.411552 thundra-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-08 12:21:20.000000 thundra-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-08 12:21:41.411552 thundra-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30786 2023-06-08 12:21:20.000000 thundra-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.383551 thundra-3.0.5/foresight/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.383551 thundra-3.0.5/foresight/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/constants/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.383551 thundra-3.0.5/foresight/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/context/test_case_execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/context/test_suite_execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/environment/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/azure/azure_environment_info_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/environment/bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/bitbucket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/bitbucket/bitbucket_environment_info_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/environment/circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/circleci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/circleci/circleci_environment_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/environment_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/environment_info_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/environment/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/git/git_env_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/git/git_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/git/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/environment/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/github/github_environment_info_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/environment/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/gitlab/gitlab_environment_info_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/environment/jenkins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/jenkins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/jenkins/jenkins_environment_info_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/environment/travisci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/travisci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/environment/travisci/travisci_environment_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/foresight_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.387551 thundra-3.0.5/foresight/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/model/terminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/model/test_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/model/test_run_finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/model/test_run_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/model/test_run_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/model/test_run_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/model/test_run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.391551 thundra-3.0.5/foresight/pytest_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/pytest_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/pytest_integration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/pytest_integration/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/pytest_integration/pytest_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/pytest_integration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.391551 thundra-3.0.5/foresight/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/sampler/max_count_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/test_runner_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/test_runner_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/test_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.391551 thundra-3.0.5/foresight/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/utils/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/utils/handler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/utils/test_runner_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-08 12:21:20.000000 thundra-3.0.5/foresight/utils/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 12:21:41.411552 thundra-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-08 12:21:20.000000 thundra-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.391551 thundra-3.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-08 12:21:20.000000 thundra-3.0.5/tests/test_application_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-06-08 12:21:20.000000 thundra-3.0.5/tests/test_lambda_event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-08 12:21:20.000000 thundra-3.0.5/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-08 12:21:20.000000 thundra-3.0.5/tests/test_thundra_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-08 12:21:20.000000 thundra-3.0.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.391551 thundra-3.0.5/thundra/
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.395551 thundra-3.0.5/thundra/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/application/application_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/application/application_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/application/global_application_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/composite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.395551 thundra-3.0.5/thundra/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/config/config_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/config/config_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/config/config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21869 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.395551 thundra-3.0.5/thundra/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/context/context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/context/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/context/execution_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/context/global_execution_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/context/plugin_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/context/tracing_execution_context_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.395551 thundra-3.0.5/thundra/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/debug/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.395551 thundra-3.0.5/thundra/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.395551 thundra-3.0.5/thundra/integrations/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/aiohttp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/base_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38459 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/botocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.399551 thundra-3.0.5/thundra/integrations/handler_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/handler_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/handler_wrappers/chalice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.399551 thundra-3.0.5/thundra/integrations/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/botocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/modules/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/postgre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/rdb_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/integrations/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.399551 thundra-3.0.5/thundra/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/listeners/composite_span_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/listeners/error_injector_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/listeners/filtering_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/listeners/latency_injector_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/listeners/security_aware_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/listeners/tag_injector_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/listeners/thundra_span_filterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/listeners/thundra_span_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.399551 thundra-3.0.5/thundra/opentracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/opentracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.403551 thundra-3.0.5/thundra/opentracing/propagation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/opentracing/propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/opentracing/propagation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/opentracing/propagation/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/opentracing/propagation/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/opentracing/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/opentracing/span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/opentracing/span_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/opentracing/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.403551 thundra-3.0.5/thundra/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.403551 thundra-3.0.5/thundra/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/config/base_plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/config/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/config/metric_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/config/thundra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/config/trace_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.403551 thundra-3.0.5/thundra/plugins/invocation/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/invocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/invocation/invocation_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/invocation/invocation_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/invocation/invocation_trace_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.403551 thundra-3.0.5/thundra/plugins/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/log/log_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/log/log_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/log/thundra_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/log/thundra_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.403551 thundra-3.0.5/thundra/plugins/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/metric/metric_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/metric/metric_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.403551 thundra-3.0.5/thundra/plugins/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/trace/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/trace/trace_aware_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/trace/trace_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/trace/trace_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/plugins/trace/traceable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.407552 thundra-3.0.5/thundra/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/samplers/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/samplers/composite_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/samplers/count_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/samplers/duration_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/samplers/error_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/samplers/time_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/thundra_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.407552 thundra-3.0.5/thundra/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.407552 thundra-3.0.5/thundra/wrappers/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/aws_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/aws_lambda/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/aws_lambda/lambda_application_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/aws_lambda/lambda_event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/aws_lambda/lambda_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/aws_lambda/lambda_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/cp_wrapper_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.407552 thundra-3.0.5/thundra/wrappers/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/django/django_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/django/django_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.407552 thundra-3.0.5/thundra/wrappers/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/fastapi/fastapi_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/fastapi/fastapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/fastapi/fastapi_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/fastapi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.407552 thundra-3.0.5/thundra/wrappers/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/flask/flask_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/flask/flask_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/flask/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.411552 thundra-3.0.5/thundra/wrappers/tornado/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/tornado/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/tornado/tornado_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/tornado/tornado_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/web_wrapper_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/wrapper_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-08 12:21:20.000000 thundra-3.0.5/thundra/wrappers/wrapper_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:41.395551 thundra-3.0.5/thundra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-08 12:21:41.000000 thundra-3.0.5/thundra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-06-08 12:21:41.000000 thundra-3.0.5/thundra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:21:41.000000 thundra-3.0.5/thundra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 12:21:41.000000 thundra-3.0.5/thundra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 12:21:41.000000 thundra-3.0.5/thundra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 12:21:41.000000 thundra-3.0.5/thundra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:21:41.000000 thundra-3.0.5/thundra.egg-info/zip-safe
```

### Comparing `thundra-3.0.4/LICENSE` & `thundra-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/PKG-INFO` & `thundra-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thundra
-Version: 3.0.4
+Version: 3.0.5
 Summary: Thundra Python agent
 Home-page: https://github.com/thundra-agent-python
 Author: Thundra
 Author-email: python@thundra.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `thundra-3.0.4/README.md` & `thundra-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/context/test_case_execution_context.py` & `thundra-3.0.5/foresight/context/test_case_execution_context.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/context/test_suite_execution_context.py` & `thundra-3.0.5/foresight/context/test_suite_execution_context.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/azure/azure_environment_info_provider.py` & `thundra-3.0.5/foresight/environment/azure/azure_environment_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/bitbucket/bitbucket_environment_info_provider.py` & `thundra-3.0.5/foresight/environment/bitbucket/bitbucket_environment_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/circleci/circleci_environment_info_provider.py` & `thundra-3.0.5/foresight/environment/circleci/circleci_environment_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/environment_info.py` & `thundra-3.0.5/foresight/environment/environment_info.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/environment_info_support.py` & `thundra-3.0.5/foresight/environment/environment_info_support.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/git/git_env_info_provider.py` & `thundra-3.0.5/foresight/environment/git/git_env_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/git/git_helper.py` & `thundra-3.0.5/foresight/environment/git/git_helper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/git/utils.py` & `thundra-3.0.5/foresight/environment/git/utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/github/github_environment_info_provider.py` & `thundra-3.0.5/foresight/environment/github/github_environment_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/gitlab/gitlab_environment_info_provider.py` & `thundra-3.0.5/foresight/environment/gitlab/gitlab_environment_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/jenkins/jenkins_environment_info_provider.py` & `thundra-3.0.5/foresight/environment/jenkins/jenkins_environment_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/environment/travisci/travisci_environment_info_provider.py` & `thundra-3.0.5/foresight/environment/travisci/travisci_environment_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/foresight_executor.py` & `thundra-3.0.5/foresight/foresight_executor.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/model/__init__.py` & `thundra-3.0.5/foresight/model/__init__.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/model/terminator.py` & `thundra-3.0.5/foresight/model/terminator.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/model/test_run_context.py` & `thundra-3.0.5/foresight/model/test_run_context.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/model/test_run_finish.py` & `thundra-3.0.5/foresight/model/test_run_finish.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/model/test_run_monitoring.py` & `thundra-3.0.5/foresight/model/test_run_monitoring.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/model/test_run_result.py` & `thundra-3.0.5/foresight/model/test_run_result.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/model/test_run_start.py` & `thundra-3.0.5/foresight/model/test_run_start.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/model/test_run_status.py` & `thundra-3.0.5/foresight/model/test_run_status.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/pytest_integration/plugin.py` & `thundra-3.0.5/foresight/pytest_integration/plugin.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/pytest_integration/pytest_helper.py` & `thundra-3.0.5/foresight/pytest_integration/pytest_helper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/pytest_integration/utils.py` & `thundra-3.0.5/foresight/pytest_integration/utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/test_runner_support.py` & `thundra-3.0.5/foresight/test_runner_support.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/test_runner_tags.py` & `thundra-3.0.5/foresight/test_runner_tags.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/test_status.py` & `thundra-3.0.5/foresight/test_status.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/utils/handler_utils.py` & `thundra-3.0.5/foresight/utils/handler_utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/utils/test_runner_utils.py` & `thundra-3.0.5/foresight/utils/test_runner_utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/foresight/utils/test_wrapper.py` & `thundra-3.0.5/foresight/utils/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/setup.py` & `thundra-3.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/tests/test_application_support.py` & `thundra-3.0.5/tests/test_application_support.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/tests/test_lambda_event_utils.py` & `thundra-3.0.5/tests/test_lambda_event_utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/tests/test_thundra_agent.py` & `thundra-3.0.5/tests/test_thundra_agent.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/tests/test_utils.py` & `thundra-3.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/__init__.py` & `thundra-3.0.5/thundra/__init__.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/application/application_info.py` & `thundra-3.0.5/thundra/application/application_info.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/application/application_info_provider.py` & `thundra-3.0.5/thundra/application/application_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/application/global_application_info_provider.py` & `thundra-3.0.5/thundra/application/global_application_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/compat.py` & `thundra-3.0.5/thundra/compat.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/composite.py` & `thundra-3.0.5/thundra/composite.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/config/config_metadata.py` & `thundra-3.0.5/thundra/config/config_metadata.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/config/config_names.py` & `thundra-3.0.5/thundra/config/config_names.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/config/config_provider.py` & `thundra-3.0.5/thundra/config/config_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/constants.py` & `thundra-3.0.5/thundra/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 HOST = "https://api.thundra.io/v1"
 PATH = "/monitoring-data"
 COMPOSITE_DATA_PATH = "/composite-monitoring-data"
 
 THUNDRA_AGENT_VERSION = __version__
 TEST_RUN_EVENTS_DATA_VERSION = "1.0"
 
+DEFAULT_APPLICATION_NAME = 'catchpoint-app'
 LAMBDA_APPLICATION_DOMAIN_NAME = 'API'
 LAMBDA_APPLICATION_CLASS_NAME = 'AWS-Lambda'
 LAMBDA_APPLICATION_PLATFORM = 'AWS Lambda'
 
 TRIGGER_OPERATION_NAME_KEY = 'x-catchpoint-trigger-operation-name'
 TRIGGER_CLASS_NAME_KEY = 'x-catchpoint-trigger-class-name'
 TRIGGER_DOMAIN_NAME_KEY = 'x-catchpoint-trigger-domain-name'
@@ -720,7 +721,43 @@
     ])
 }
 
 AwsEventBridgeTags = {
     'SERVICE_REQUEST': 'AWSEventBridgeRequest',
     'ENTRIES': 'aws.eventbridge.entries'
 }
+
+CatchpointTags = {
+    'REGION_NAME': 'catchpoint.region.name',
+    'COUNTRY_NAME': 'catchpoint.country.name',
+    'CITY_NAME': 'catchpoint.city.name',
+    'TEST_ID': 'catchpoint.test.id'
+}
+
+HTTPHeaders = {
+    'USER_AGENT': 'User-Agent',
+    'CONTENT_TYPE': 'Content-Type',
+    'AUTHORIZATION': 'Authorization'
+}
+
+CatchpointHeaders = {
+    'REGION_NAME': 'x-catchpoint-region-name',
+    'COUNTRY_NAME': 'x-catchpoint-country-name',
+    'CITY_NAME': 'x-catchpoint-city-name',
+    'TEST_ID': 'x-catchpoint-test-id',
+    'TIME': 'x-catchpoint-time'
+}
+
+CatchpointProperties = {
+    'DEFAULT_APP_NAME': 'Catchpoint',
+    'APP_DOMAIN_NAME': 'Monitoring',
+    'APP_CLASS_NAME': 'Catchpoint',
+    'APP_REGION_PLACEHOLDER': '${cp-app-region}',
+    'APP_NAME_PLACEHOLDER': '${cp-app-name}',
+    'APP_ID_TEMPLATE': ':catchpoint:${cp-app-region}:${cp-app-name}',
+    'HTTP_REQUEST_DOMAIN_NAME': 'API',
+    'HTTP_REQUEST_CLASS_NAME': 'HTTP',
+    'TIME_MAX_DIFF': 30000,
+    'AGENT_VERSION': 'Catchpoint'
+}
+
+
```

### Comparing `thundra-3.0.4/thundra/context/execution_context.py` & `thundra-3.0.5/thundra/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/context/execution_context_manager.py` & `thundra-3.0.5/thundra/context/execution_context_manager.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/context/tracing_execution_context_provider.py` & `thundra-3.0.5/thundra/context/tracing_execution_context_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/debug/bridge.py` & `thundra-3.0.5/thundra/debug/bridge.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/handler.py` & `thundra-3.0.5/thundra/handler.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/aiohttp/client.py` & `thundra-3.0.5/thundra/integrations/aiohttp/client.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/base_integration.py` & `thundra-3.0.5/thundra/integrations/base_integration.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/botocore.py` & `thundra-3.0.5/thundra/integrations/botocore.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/django.py` & `thundra-3.0.5/thundra/integrations/django.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/elasticsearch.py` & `thundra-3.0.5/thundra/integrations/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/handler_wrappers/__init__.py` & `thundra-3.0.5/thundra/integrations/handler_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/handler_wrappers/chalice.py` & `thundra-3.0.5/thundra/integrations/handler_wrappers/chalice.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/__init__.py` & `thundra-3.0.5/thundra/integrations/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/aiohttp.py` & `thundra-3.0.5/thundra/integrations/modules/aiohttp.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/botocore.py` & `thundra-3.0.5/thundra/integrations/modules/botocore.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/db.py` & `thundra-3.0.5/thundra/integrations/modules/db.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/django.py` & `thundra-3.0.5/thundra/integrations/modules/django.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/elasticsearch.py` & `thundra-3.0.5/thundra/integrations/modules/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/fastapi.py` & `thundra-3.0.5/thundra/integrations/modules/fastapi.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/flask.py` & `thundra-3.0.5/thundra/integrations/modules/flask.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/mysql.py` & `thundra-3.0.5/thundra/integrations/modules/mysql.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/psycopg2.py` & `thundra-3.0.5/thundra/integrations/modules/psycopg2.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/pymongo.py` & `thundra-3.0.5/thundra/integrations/modules/pymongo.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/redis.py` & `thundra-3.0.5/thundra/integrations/modules/redis.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/requests.py` & `thundra-3.0.5/thundra/integrations/modules/requests.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/sqlalchemy.py` & `thundra-3.0.5/thundra/integrations/modules/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/modules/tornado.py` & `thundra-3.0.5/thundra/integrations/modules/tornado.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/mongodb.py` & `thundra-3.0.5/thundra/integrations/mongodb.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/mysql.py` & `thundra-3.0.5/thundra/integrations/mysql.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/postgre.py` & `thundra-3.0.5/thundra/integrations/postgre.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/redis.py` & `thundra-3.0.5/thundra/integrations/redis.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/requests.py` & `thundra-3.0.5/thundra/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/integrations/sqlalchemy.py` & `thundra-3.0.5/thundra/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/listeners/composite_span_filter.py` & `thundra-3.0.5/thundra/listeners/composite_span_filter.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/listeners/error_injector_span_listener.py` & `thundra-3.0.5/thundra/listeners/error_injector_span_listener.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/listeners/filtering_span_listener.py` & `thundra-3.0.5/thundra/listeners/filtering_span_listener.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/listeners/latency_injector_span_listener.py` & `thundra-3.0.5/thundra/listeners/latency_injector_span_listener.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/listeners/security_aware_span_listener.py` & `thundra-3.0.5/thundra/listeners/security_aware_span_listener.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/listeners/tag_injector_span_listener.py` & `thundra-3.0.5/thundra/listeners/tag_injector_span_listener.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/listeners/thundra_span_filterer.py` & `thundra-3.0.5/thundra/listeners/thundra_span_filterer.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/listeners/thundra_span_listener.py` & `thundra-3.0.5/thundra/listeners/thundra_span_listener.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/opentracing/propagation/http.py` & `thundra-3.0.5/thundra/opentracing/propagation/http.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/opentracing/propagation/text.py` & `thundra-3.0.5/thundra/opentracing/propagation/text.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/opentracing/span.py` & `thundra-3.0.5/thundra/opentracing/span.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/opentracing/span_context.py` & `thundra-3.0.5/thundra/opentracing/span_context.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/opentracing/tracer.py` & `thundra-3.0.5/thundra/opentracing/tracer.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/config/thundra_config.py` & `thundra-3.0.5/thundra/plugins/config/thundra_config.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/invocation/invocation_plugin.py` & `thundra-3.0.5/thundra/plugins/invocation/invocation_plugin.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/invocation/invocation_support.py` & `thundra-3.0.5/thundra/plugins/invocation/invocation_support.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/invocation/invocation_trace_support.py` & `thundra-3.0.5/thundra/plugins/invocation/invocation_trace_support.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/log/log_plugin.py` & `thundra-3.0.5/thundra/plugins/log/log_plugin.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/log/thundra_log_handler.py` & `thundra-3.0.5/thundra/plugins/log/thundra_log_handler.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/log/thundra_logger.py` & `thundra-3.0.5/thundra/plugins/log/thundra_logger.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/metric/metric_plugin.py` & `thundra-3.0.5/thundra/plugins/metric/metric_plugin.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/trace/patcher.py` & `thundra-3.0.5/thundra/plugins/trace/patcher.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/trace/trace_aware_wrapper.py` & `thundra-3.0.5/thundra/plugins/trace/trace_aware_wrapper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/trace/trace_plugin.py` & `thundra-3.0.5/thundra/plugins/trace/trace_plugin.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/trace/trace_support.py` & `thundra-3.0.5/thundra/plugins/trace/trace_support.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/plugins/trace/traceable.py` & `thundra-3.0.5/thundra/plugins/trace/traceable.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/samplers/composite_sampler.py` & `thundra-3.0.5/thundra/samplers/composite_sampler.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/samplers/count_aware_sampler.py` & `thundra-3.0.5/thundra/samplers/count_aware_sampler.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/samplers/time_aware_sampler.py` & `thundra-3.0.5/thundra/samplers/time_aware_sampler.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/timeout.py` & `thundra-3.0.5/thundra/timeout.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/utils.py` & `thundra-3.0.5/thundra/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from __future__ import absolute_import
 import logging
 import os
 import re
+import uuid
 
 from thundra import constants
 from thundra.compat import urlparse
 from opentracing.scope_managers import ThreadLocalScopeManager
 
 logger = logging.getLogger(__name__)
 
 
+def generate_id():
+    return str(uuid.uuid4())
+
+
+def generate_id_from(value):
+    return str(uuid.uuid5(uuid.NAMESPACE_OID, value))
+
+
 def get_env_variable(key, default=None):
     return os.environ.get(key, default)
 
 
 def get_aws_function_name(arn):
     return get_arn_part(arn, 6)
```

### Comparing `thundra-3.0.4/thundra/wrappers/aws_lambda/handler.py` & `thundra-3.0.5/thundra/wrappers/aws_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/aws_lambda/lambda_application_info_provider.py` & `thundra-3.0.5/thundra/wrappers/aws_lambda/lambda_application_info_provider.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/aws_lambda/lambda_event_utils.py` & `thundra-3.0.5/thundra/wrappers/aws_lambda/lambda_event_utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/aws_lambda/lambda_executor.py` & `thundra-3.0.5/thundra/wrappers/aws_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/aws_lambda/lambda_wrapper.py` & `thundra-3.0.5/thundra/wrappers/aws_lambda/lambda_wrapper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/base_wrapper.py` & `thundra-3.0.5/thundra/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/django/django_executor.py` & `thundra-3.0.5/thundra/wrappers/django/django_executor.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/django/django_wrapper.py` & `thundra-3.0.5/thundra/wrappers/django/django_wrapper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/django/middleware.py` & `thundra-3.0.5/thundra/wrappers/django/middleware.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/fastapi/fastapi_executor.py` & `thundra-3.0.5/thundra/wrappers/fastapi/fastapi_executor.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/fastapi/fastapi_utils.py` & `thundra-3.0.5/thundra/wrappers/fastapi/fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/fastapi/fastapi_wrapper.py` & `thundra-3.0.5/thundra/wrappers/fastapi/fastapi_wrapper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/fastapi/middleware.py` & `thundra-3.0.5/thundra/wrappers/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/flask/flask_executor.py` & `thundra-3.0.5/thundra/wrappers/flask/flask_executor.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/flask/flask_wrapper.py` & `thundra-3.0.5/thundra/wrappers/flask/flask_wrapper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/flask/middleware.py` & `thundra-3.0.5/thundra/wrappers/flask/middleware.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/tornado/middleware.py` & `thundra-3.0.5/thundra/wrappers/tornado/middleware.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/tornado/tornado_executor.py` & `thundra-3.0.5/thundra/wrappers/tornado/tornado_executor.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/tornado/tornado_wrapper.py` & `thundra-3.0.5/thundra/wrappers/tornado/tornado_wrapper.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra/wrappers/web_wrapper_utils.py` & `thundra-3.0.5/thundra/wrappers/web_wrapper_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from opentracing import Format
 
 from thundra import constants
 from thundra.config import config_names
 from thundra.config.config_provider import ConfigProvider
 from thundra.plugins.invocation import invocation_support, invocation_trace_support
 from thundra.utils import get_normalized_path
+import thundra.wrappers.cp_wrapper_utils as cp_wrapper_utils
 
 Logger = logging.getLogger(__name__)
 
 def start_trace(execution_context, tracer, class_name, domain_name, request, request_route_path=None):
     propagated_span_context = tracer.extract(Format.HTTP_HEADERS, request.get('headers'))
     trace_id = str(uuid.uuid4())
     incoming_span_id = None
@@ -90,14 +91,16 @@
 
 
 def finish_trace(execution_context):
     root_span = execution_context.root_span
     scope = execution_context.scope
     try:
         root_span.finish(f_time=execution_context.finish_timestamp)
+        cp_wrapper_utils.on_finish(execution_context, execution_context.platform_data["request"],
+                                   execution_context.response, root_span)
     except Exception:
         # TODO: handle root span finish errors
         pass
     finally:
         try:
             scope.close()
         except Exception as e:
```

### Comparing `thundra-3.0.4/thundra/wrappers/wrapper_utils.py` & `thundra-3.0.5/thundra/wrappers/wrapper_utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.4/thundra.egg-info/PKG-INFO` & `thundra-3.0.5/thundra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thundra
-Version: 3.0.4
+Version: 3.0.5
 Summary: Thundra Python agent
 Home-page: https://github.com/thundra-agent-python
 Author: Thundra
 Author-email: python@thundra.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `thundra-3.0.4/thundra.egg-info/SOURCES.txt` & `thundra-3.0.5/thundra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 thundra/samplers/composite_sampler.py
 thundra/samplers/count_aware_sampler.py
 thundra/samplers/duration_aware_sampler.py
 thundra/samplers/error_aware_sampler.py
 thundra/samplers/time_aware_sampler.py
 thundra/wrappers/__init__.py
 thundra/wrappers/base_wrapper.py
+thundra/wrappers/cp_wrapper_utils.py
 thundra/wrappers/web_wrapper_utils.py
 thundra/wrappers/wrapper_factory.py
 thundra/wrappers/wrapper_utils.py
 thundra/wrappers/aws_lambda/__init__.py
 thundra/wrappers/aws_lambda/handler.py
 thundra/wrappers/aws_lambda/lambda_application_info_provider.py
 thundra/wrappers/aws_lambda/lambda_event_utils.py
```

