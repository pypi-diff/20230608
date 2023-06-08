# Comparing `tmp/boneIO-0.6.2.tar.gz` & `tmp/boneIO-0.6.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boneIO-0.6.2.tar", last modified: Tue May 23 19:48:50 2023, max compression
+gzip compressed data, was "boneIO-0.6.3.dev1.tar", last modified: Thu Jun  8 19:30:47 2023, max compression
```

## Comparing `boneIO-0.6.2.tar` & `boneIO-0.6.3.dev1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    35149 2023-05-23 19:48:17.600596 boneIO-0.6.2/LICENSE
--rw-r--r--   0        0        0      474 2023-05-23 19:48:17.600596 boneIO-0.6.2/README.md
--rw-r--r--   0        0        0      147 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/__init__.py
--rw-r--r--   0        0        0     3341 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/bonecli.py
--rw-r--r--   0        0        0     2924 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/const.py
--rw-r--r--   0        0        0     8454 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/cover.py
--rw-r--r--   0        0        0        0 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/example_config/__init__.py
--rw-r--r--   0        0        0      168 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/example_config/adc.yaml
--rw-r--r--   0        0        0      326 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/example_config/config.yaml
--rw-r--r--   0        0        0      150 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/example_config/cover.yaml
--rw-r--r--   0        0        0     2883 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/example_config/input.yaml
--rw-r--r--   0        0        0     3392 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/example_config/led32x4A.yaml
--rw-r--r--   0        0        0     1691 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/example_config/output24x16A.yaml
--rw-r--r--   0        0        0     2403 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/example_config/output32x5A.yaml
--rw-r--r--   0        0        0    19372 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/fonts/danube__.ttf
--rw-r--r--   0        0        0     2039 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/__init__.py
--rw-r--r--   0        0        0      985 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/async_updater.py
--rw-r--r--   0        0        0     1169 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/click_timer.py
--rw-r--r--   0        0        0     2277 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/config.py
--rw-r--r--   0        0        0     7494 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/events.py
--rw-r--r--   0        0        0      717 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/exceptions.py
--rw-r--r--   0        0        0      885 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/filter.py
--rw-r--r--   0        0        0     2718 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/gpio.py
--rw-r--r--   0        0        0     6278 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/ha_discovery.py
--rw-r--r--   0        0        0    13547 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/loader.py
--rw-r--r--   0        0        0     1801 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/logger.py
--rw-r--r--   0        0        0      765 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/mqtt.py
--rw-r--r--   0        0        0      351 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/oled.py
--rw-r--r--   0        0        0     2430 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/onewire/W1ThermSensor.py
--rw-r--r--   0        0        0      448 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/onewire/__init__.py
--rw-r--r--   0        0        0     5169 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/onewire/ds2482.py
--rw-r--r--   0        0        0     2497 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/onewire/onewire.py
--rw-r--r--   0        0        0     1066 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/queue.py
--rw-r--r--   0        0        0     1994 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/state_manager.py
--rw-r--r--   0        0        0     5853 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/stats.py
--rw-r--r--   0        0        0     5806 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/timeperiod.py
--rw-r--r--   0        0        0      508 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/util.py
--rw-r--r--   0        0        0    11304 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/helper/yaml_util.py
--rw-r--r--   0        0        0       99 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/input/__init__.py
--rw-r--r--   0        0        0     2597 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/input/gpio.py
--rw-r--r--   0        0        0    20922 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/manager.py
--rw-r--r--   0        0        0     4176 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/modbus.py
--rw-r--r--   0        0        0     8331 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/mqtt_client.py
--rw-r--r--   0        0        0     5244 2023-05-23 19:48:17.600596 boneIO-0.6.2/boneio/oled.py
--rw-r--r--   0        0        0      181 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/relay/__init__.py
--rw-r--r--   0        0        0     2623 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/relay/basic.py
--rw-r--r--   0        0        0     1163 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/relay/gpio.py
--rw-r--r--   0        0        0     2669 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/relay/mcp.py
--rw-r--r--   0        0        0     4873 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/relay/pca.py
--rw-r--r--   0        0        0     2569 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/runner.py
--rw-r--r--   0        0        0     1030 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/schema/actions.yaml
--rw-r--r--   0        0        0      124 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/schema/actions_sensor.yaml
--rw-r--r--   0        0        0      129 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/schema/actions_switch.yaml
--rw-r--r--   0        0        0      286 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/schema/filters.yaml
--rw-r--r--   0        0        0      304 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/schema/filters_adc.yaml
--rw-r--r--   0        0        0       75 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/schema/id.yaml
--rw-r--r--   0        0        0    12988 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/schema/schema.yaml
--rw-r--r--   0        0        0       65 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/schema/temp_unit.yaml
--rw-r--r--   0        0        0      133 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/schema/update_interval.yaml
--rw-r--r--   0        0        0      431 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/__init__.py
--rw-r--r--   0        0        0     1281 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/adc.py
--rw-r--r--   0        0        0     1303 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/gpio.py
--rw-r--r--   0        0        0     8520 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/modbus/__init__.py
--rw-r--r--   0        0        0     8810 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/modbus/dts1964_3f.json
--rw-r--r--   0        0        0      526 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/modbus/pt100.json
--rw-r--r--   0        0        0     2735 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/modbus/r4dcb08.json
--rw-r--r--   0        0        0     4145 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/modbus/sdm120.json
--rw-r--r--   0        0        0    10969 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/modbus/sdm630.json
--rw-r--r--   0        0        0     5592 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/modbus/sofar.json
--rw-r--r--   0        0        0     1808 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/temp/__init__.py
--rw-r--r--   0        0        0     2485 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/temp/dallas.py
--rw-r--r--   0        0        0      243 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/temp/lm75.py
--rw-r--r--   0        0        0      271 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/sensor/temp/mcp9808.py
--rw-r--r--   0        0        0       37 2023-05-23 19:48:17.604597 boneIO-0.6.2/boneio/version.py
--rw-r--r--   0        0        0     1868 2023-05-23 19:48:17.604597 boneIO-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      166 2023-05-23 19:48:17.604597 boneIO-0.6.2/tests/32_5_config.yaml
--rw-r--r--   0        0        0      224 2023-05-23 19:48:17.604597 boneIO-0.6.2/tests/bandit.yaml
--rw-r--r--   0        0        0     1070 2023-05-23 19:48:17.604597 boneIO-0.6.2/tests/relay_32_5.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 boneIO-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/LICENSE
+-rw-r--r--   0        0        0      474 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/README.md
+-rw-r--r--   0        0        0      147 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/__init__.py
+-rw-r--r--   0        0        0     3341 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/bonecli.py
+-rw-r--r--   0        0        0     2924 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/const.py
+-rw-r--r--   0        0        0     8454 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/cover.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/example_config/__init__.py
+-rw-r--r--   0        0        0      168 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/example_config/adc.yaml
+-rw-r--r--   0        0        0      326 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/example_config/config.yaml
+-rw-r--r--   0        0        0      150 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/example_config/cover.yaml
+-rw-r--r--   0        0        0     2883 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/example_config/input.yaml
+-rw-r--r--   0        0        0     3392 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/example_config/led32x4A.yaml
+-rw-r--r--   0        0        0     1691 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/example_config/output24x16A.yaml
+-rw-r--r--   0        0        0     2403 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/example_config/output32x5A.yaml
+-rw-r--r--   0        0        0    19372 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/fonts/danube__.ttf
+-rw-r--r--   0        0        0     2039 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/async_updater.py
+-rw-r--r--   0        0        0     1169 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/click_timer.py
+-rw-r--r--   0        0        0     2277 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/config.py
+-rw-r--r--   0        0        0     7494 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/events.py
+-rw-r--r--   0        0        0      717 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/exceptions.py
+-rw-r--r--   0        0        0      885 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/filter.py
+-rw-r--r--   0        0        0     2719 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/gpio.py
+-rw-r--r--   0        0        0     6278 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/ha_discovery.py
+-rw-r--r--   0        0        0    13547 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/loader.py
+-rw-r--r--   0        0        0     1801 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/logger.py
+-rw-r--r--   0        0        0      765 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/mqtt.py
+-rw-r--r--   0        0        0      351 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/oled.py
+-rw-r--r--   0        0        0     2430 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/onewire/W1ThermSensor.py
+-rw-r--r--   0        0        0      448 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/onewire/__init__.py
+-rw-r--r--   0        0        0     5169 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/onewire/ds2482.py
+-rw-r--r--   0        0        0     2497 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/onewire/onewire.py
+-rw-r--r--   0        0        0     1066 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/queue.py
+-rw-r--r--   0        0        0     1994 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/state_manager.py
+-rw-r--r--   0        0        0     5853 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/stats.py
+-rw-r--r--   0        0        0     5806 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/timeperiod.py
+-rw-r--r--   0        0        0      508 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/util.py
+-rw-r--r--   0        0        0    11304 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/helper/yaml_util.py
+-rw-r--r--   0        0        0       99 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/input/__init__.py
+-rw-r--r--   0        0        0     2515 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/input/gpio.py
+-rw-r--r--   0        0        0    20922 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/manager.py
+-rw-r--r--   0        0        0     4176 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/modbus.py
+-rw-r--r--   0        0        0     8331 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/mqtt_client.py
+-rw-r--r--   0        0        0     5244 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/oled.py
+-rw-r--r--   0        0        0      181 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/relay/__init__.py
+-rw-r--r--   0        0        0     2623 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/relay/basic.py
+-rw-r--r--   0        0        0     1163 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/relay/gpio.py
+-rw-r--r--   0        0        0     2669 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/relay/mcp.py
+-rw-r--r--   0        0        0     4873 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/relay/pca.py
+-rw-r--r--   0        0        0     2569 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/runner.py
+-rw-r--r--   0        0        0     1030 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/schema/actions.yaml
+-rw-r--r--   0        0        0      124 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/schema/actions_sensor.yaml
+-rw-r--r--   0        0        0      129 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/schema/actions_switch.yaml
+-rw-r--r--   0        0        0      286 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/schema/filters.yaml
+-rw-r--r--   0        0        0      304 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/schema/filters_adc.yaml
+-rw-r--r--   0        0        0       75 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/schema/id.yaml
+-rw-r--r--   0        0        0    12989 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/schema/schema.yaml
+-rw-r--r--   0        0        0       65 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/schema/temp_unit.yaml
+-rw-r--r--   0        0        0      133 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/schema/update_interval.yaml
+-rw-r--r--   0        0        0      431 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/__init__.py
+-rw-r--r--   0        0        0     1281 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/adc.py
+-rw-r--r--   0        0        0     1303 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/gpio.py
+-rw-r--r--   0        0        0     8520 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/modbus/__init__.py
+-rw-r--r--   0        0        0     8810 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/modbus/dts1964_3f.json
+-rw-r--r--   0        0        0      526 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/modbus/pt100.json
+-rw-r--r--   0        0        0     2735 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/modbus/r4dcb08.json
+-rw-r--r--   0        0        0     4145 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/modbus/sdm120.json
+-rw-r--r--   0        0        0    10969 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/modbus/sdm630.json
+-rw-r--r--   0        0        0     5592 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/modbus/sofar.json
+-rw-r--r--   0        0        0     1808 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/temp/__init__.py
+-rw-r--r--   0        0        0     2485 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/temp/dallas.py
+-rw-r--r--   0        0        0      243 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/temp/lm75.py
+-rw-r--r--   0        0        0      271 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/sensor/temp/mcp9808.py
+-rw-r--r--   0        0        0       42 2023-06-08 19:30:17.937630 boneIO-0.6.3.dev1/boneio/version.py
+-rw-r--r--   0        0        0     1873 2023-06-08 19:30:17.941630 boneIO-0.6.3.dev1/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-06-08 19:30:17.941630 boneIO-0.6.3.dev1/tests/32_5_config.yaml
+-rw-r--r--   0        0        0      224 2023-06-08 19:30:17.941630 boneIO-0.6.3.dev1/tests/bandit.yaml
+-rw-r--r--   0        0        0     1070 2023-06-08 19:30:17.941630 boneIO-0.6.3.dev1/tests/relay_32_5.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.6.3.dev1/PKG-INFO
```

### Comparing `boneIO-0.6.2/LICENSE` & `boneIO-0.6.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/bonecli.py` & `boneIO-0.6.3.dev1/boneio/bonecli.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/const.py` & `boneIO-0.6.3.dev1/boneio/const.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/cover.py` & `boneIO-0.6.3.dev1/boneio/cover.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/example_config/input.yaml` & `boneIO-0.6.3.dev1/boneio/example_config/input.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/example_config/led32x4A.yaml` & `boneIO-0.6.3.dev1/boneio/example_config/led32x4A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/example_config/output24x16A.yaml` & `boneIO-0.6.3.dev1/boneio/example_config/output24x16A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/example_config/output32x5A.yaml` & `boneIO-0.6.3.dev1/boneio/example_config/output32x5A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/fonts/danube__.ttf` & `boneIO-0.6.3.dev1/boneio/fonts/danube__.ttf`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/__init__.py` & `boneIO-0.6.3.dev1/boneio/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/async_updater.py` & `boneIO-0.6.3.dev1/boneio/helper/async_updater.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/click_timer.py` & `boneIO-0.6.3.dev1/boneio/helper/click_timer.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/config.py` & `boneIO-0.6.3.dev1/boneio/helper/config.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/events.py` & `boneIO-0.6.3.dev1/boneio/helper/events.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/exceptions.py` & `boneIO-0.6.3.dev1/boneio/helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/filter.py` & `boneIO-0.6.3.dev1/boneio/helper/filter.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/gpio.py` & `boneIO-0.6.3.dev1/boneio/helper/gpio.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     def __init__(
         self, pin: str, press_callback: Callable[[ClickTypes, str], None], **kwargs
     ) -> None:
         """Setup GPIO Input Button"""
         self._pin = pin
         gpio_mode = kwargs.get(GPIO_MODE, GPIO_STR)
-        self._bounce_time = kwargs.get("bounce_time", TimePeriod(milliseconds=10))
+        self._bounce_time = kwargs.get("bounce_time", TimePeriod(milliseconds=120))
         self._loop = asyncio.get_running_loop()
         self._press_callback = press_callback
         setup_input(pin=self._pin, pull_mode=gpio_mode)
 
     @property
     def is_pressed(self) -> bool:
         """Is button pressed."""
```

### Comparing `boneIO-0.6.2/boneio/helper/ha_discovery.py` & `boneIO-0.6.3.dev1/boneio/helper/ha_discovery.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/loader.py` & `boneIO-0.6.3.dev1/boneio/helper/loader.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/logger.py` & `boneIO-0.6.3.dev1/boneio/helper/logger.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/mqtt.py` & `boneIO-0.6.3.dev1/boneio/helper/mqtt.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/onewire/W1ThermSensor.py` & `boneIO-0.6.3.dev1/boneio/helper/onewire/W1ThermSensor.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/onewire/ds2482.py` & `boneIO-0.6.3.dev1/boneio/helper/onewire/ds2482.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/onewire/onewire.py` & `boneIO-0.6.3.dev1/boneio/helper/onewire/onewire.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/queue.py` & `boneIO-0.6.3.dev1/boneio/helper/queue.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/state_manager.py` & `boneIO-0.6.3.dev1/boneio/helper/state_manager.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/stats.py` & `boneIO-0.6.3.dev1/boneio/helper/stats.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/timeperiod.py` & `boneIO-0.6.3.dev1/boneio/helper/timeperiod.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/helper/yaml_util.py` & `boneIO-0.6.3.dev1/boneio/helper/yaml_util.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/input/gpio.py` & `boneIO-0.6.3.dev1/boneio/input/gpio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """GPIOInputButton to receive signals."""
 from __future__ import annotations
 import logging
 import asyncio
-from datetime import timedelta
 from functools import partial
 from boneio.const import DOUBLE, LONG, SINGLE, ClickTypes
 from boneio.helper import GpioBaseClass, ClickTimer
 
 
 # TIMINGS FOR BUTTONS
 
-DEBOUNCE_DURATION = timedelta(microseconds=150000)
 DOUBLE_CLICK_DURATION_MS = 350
-LONG_PRESS_DURATION_MS = 700
+LONG_PRESS_DURATION_MS = 600
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class GpioInputButton(GpioBaseClass):
     """Represent Gpio input switch."""
```

### Comparing `boneIO-0.6.2/boneio/manager.py` & `boneIO-0.6.3.dev1/boneio/manager.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/modbus.py` & `boneIO-0.6.3.dev1/boneio/modbus.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/mqtt_client.py` & `boneIO-0.6.3.dev1/boneio/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/oled.py` & `boneIO-0.6.3.dev1/boneio/oled.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/relay/basic.py` & `boneIO-0.6.3.dev1/boneio/relay/basic.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/relay/gpio.py` & `boneIO-0.6.3.dev1/boneio/relay/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/relay/mcp.py` & `boneIO-0.6.3.dev1/boneio/relay/mcp.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/relay/pca.py` & `boneIO-0.6.3.dev1/boneio/relay/pca.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/runner.py` & `boneIO-0.6.3.dev1/boneio/runner.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/schema/actions.yaml` & `boneIO-0.6.3.dev1/boneio/schema/actions.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/schema/schema.yaml` & `boneIO-0.6.3.dev1/boneio/schema/schema.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
         type:
           - string
           - timeperiod
         coerce:
           - str
           - positive_time_period
         required: True
-        default: "25ms"
+        default: "120ms"
         meta:
           label: Bounce time for GPIO in miliseconds. Only for advanced usage.
       show_in_ha:
         type: boolean
         required: True
         default: True
         meta:
```

### Comparing `boneIO-0.6.2/boneio/sensor/adc.py` & `boneIO-0.6.3.dev1/boneio/sensor/adc.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/gpio.py` & `boneIO-0.6.3.dev1/boneio/sensor/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/modbus/__init__.py` & `boneIO-0.6.3.dev1/boneio/sensor/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/modbus/dts1964_3f.json` & `boneIO-0.6.3.dev1/boneio/sensor/modbus/dts1964_3f.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/modbus/pt100.json` & `boneIO-0.6.3.dev1/boneio/sensor/modbus/pt100.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/modbus/r4dcb08.json` & `boneIO-0.6.3.dev1/boneio/sensor/modbus/r4dcb08.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/modbus/sdm120.json` & `boneIO-0.6.3.dev1/boneio/sensor/modbus/sdm120.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/modbus/sdm630.json` & `boneIO-0.6.3.dev1/boneio/sensor/modbus/sdm630.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/modbus/sofar.json` & `boneIO-0.6.3.dev1/boneio/sensor/modbus/sofar.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/temp/__init__.py` & `boneIO-0.6.3.dev1/boneio/sensor/temp/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/boneio/sensor/temp/dallas.py` & `boneIO-0.6.3.dev1/boneio/sensor/temp/dallas.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/pyproject.toml` & `boneIO-0.6.3.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Adafruit-BBIO>=1.2.0",
     "psutil>=5.9.5",
     "adafruit-circuitpython-onewire>=2.0.4",
     "w1thermsensor[async]>=2.0.0",
     "adafruit-circuitpython-pca9685>=3.4.8",
 ]
 requires-python = ">=3.7"
-version = "0.6.2"
+version = "0.6.3.dev1"
 
 [project.license]
 text = "GNU General Public License v3.0"
 
 [project.urls]
 Homepage = "https://boneio.eu"
 Repository = "https://github.com/boneIO-eu/app_bbb"
```

### Comparing `boneIO-0.6.2/tests/relay_32_5.py` & `boneIO-0.6.3.dev1/tests/relay_32_5.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.2/PKG-INFO` & `boneIO-0.6.3.dev1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boneIO
-Version: 0.6.2
+Version: 0.6.3.dev1
 Summary: Python App for BoneIO
 License: GNU General Public License v3.0
 Author-email: Paweł Szafer <pszafer@gmail.com>
 Requires-Python: >=3.7
 Project-URL: Changelog, https://github.com/boneIO-eu/app_bbb/releases
 Project-URL: Documentation, https://boneio.eu/docs/intro/
 Project-URL: Homepage, https://boneio.eu
```

