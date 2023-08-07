# Comparing `tmp/boneIO-0.7.0.dev1.tar.gz` & `tmp/boneIO-0.7.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boneIO-0.7.0.dev1.tar", last modified: Fri Aug  4 20:09:07 2023, max compression
+gzip compressed data, was "boneIO-0.7.0.dev2.tar", last modified: Mon Aug  7 20:43:45 2023, max compression
```

## Comparing `boneIO-0.7.0.dev1.tar` & `boneIO-0.7.0.dev2.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0    35149 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/LICENSE
--rw-r--r--   0        0        0      474 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/README.md
--rw-r--r--   0        0        0      147 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/__init__.py
--rw-r--r--   0        0        0     3341 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/bonecli.py
--rw-r--r--   0        0        0     2947 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/const.py
--rw-r--r--   0        0        0     8454 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/cover.py
--rw-r--r--   0        0        0        0 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/__init__.py
--rw-r--r--   0        0        0      168 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/adc_v0_4.yaml
--rw-r--r--   0        0        0      238 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/binary_sensor.yaml
--rw-r--r--   0        0        0      369 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/config.yaml
--rw-r--r--   0        0        0      150 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/cover.yaml
--rw-r--r--   0        0        0     2644 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/event.yaml
--rw-r--r--   0        0        0     3392 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/led32x4A.yaml
--rw-r--r--   0        0        0     1691 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/output24x16A.yaml
--rw-r--r--   0        0        0     1713 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/output24x16A_v0.3.yaml
--rw-r--r--   0        0        0     2403 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/output32x5A.yaml
--rw-r--r--   0        0        0    19372 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/fonts/danube__.ttf
--rw-r--r--   0        0        0     2039 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/__init__.py
--rw-r--r--   0        0        0      985 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/async_updater.py
--rw-r--r--   0        0        0     1138 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/click_timer.py
--rw-r--r--   0        0        0     2321 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/config.py
--rw-r--r--   0        0        0     7494 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/events.py
--rw-r--r--   0        0        0      717 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/exceptions.py
--rw-r--r--   0        0        0      885 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/filter.py
--rw-r--r--   0        0        0     3249 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/gpio.py
--rw-r--r--   0        0        0     6359 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/ha_discovery.py
--rw-r--r--   0        0        0    14895 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/loader.py
--rw-r--r--   0        0        0     1801 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/logger.py
--rw-r--r--   0        0        0      765 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/mqtt.py
--rw-r--r--   0        0        0      351 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/oled.py
--rw-r--r--   0        0        0     2430 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/onewire/W1ThermSensor.py
--rw-r--r--   0        0        0      448 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/onewire/__init__.py
--rw-r--r--   0        0        0     5169 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/onewire/ds2482.py
--rw-r--r--   0        0        0     2497 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/onewire/onewire.py
--rw-r--r--   0        0        0     1066 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/queue.py
--rw-r--r--   0        0        0     1994 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/state_manager.py
--rw-r--r--   0        0        0     5853 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/stats.py
--rw-r--r--   0        0        0     5806 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/timeperiod.py
--rw-r--r--   0        0        0      508 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/util.py
--rw-r--r--   0        0        0    11304 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/yaml_util.py
--rw-r--r--   0        0        0      178 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/input/__init__.py
--rw-r--r--   0        0        0     2611 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/input/gpio.py
--rw-r--r--   0        0        0     3133 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/input/gpio_beta.py
--rw-r--r--   0        0        0    21785 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/manager.py
--rw-r--r--   0        0        0     4176 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/modbus.py
--rw-r--r--   0        0        0     8302 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/mqtt_client.py
--rw-r--r--   0        0        0     5244 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/oled.py
--rw-r--r--   0        0        0      181 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/__init__.py
--rw-r--r--   0        0        0     2623 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/basic.py
--rw-r--r--   0        0        0     1163 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/gpio.py
--rw-r--r--   0        0        0     2669 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/mcp.py
--rw-r--r--   0        0        0     4873 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/pca.py
--rw-r--r--   0        0        0     2653 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/runner.py
--rw-r--r--   0        0        0     1030 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/actions.yaml
--rw-r--r--   0        0        0      124 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/actions_sensor.yaml
--rw-r--r--   0        0        0      129 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/actions_switch.yaml
--rw-r--r--   0        0        0      286 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/filters.yaml
--rw-r--r--   0        0        0      304 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/filters_adc.yaml
--rw-r--r--   0        0        0       75 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/id.yaml
--rw-r--r--   0        0        0    15072 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/schema.yaml
--rw-r--r--   0        0        0       65 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/temp_unit.yaml
--rw-r--r--   0        0        0      133 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/schema/update_interval.yaml
--rw-r--r--   0        0        0      538 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/__init__.py
--rw-r--r--   0        0        0     1328 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/adc.py
--rw-r--r--   0        0        0     1296 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/gpio.py
--rw-r--r--   0        0        0     1284 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/gpio_beta.py
--rw-r--r--   0        0        0     8520 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/__init__.py
--rw-r--r--   0        0        0     8810 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/dts1964_3f.json
--rw-r--r--   0        0        0      526 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/pt100.json
--rw-r--r--   0        0        0     2735 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/r4dcb08.json
--rw-r--r--   0        0        0     4145 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/sdm120.json
--rw-r--r--   0        0        0    10969 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/sdm630.json
--rw-r--r--   0        0        0     5592 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/sofar.json
--rw-r--r--   0        0        0     1808 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/temp/__init__.py
--rw-r--r--   0        0        0     2485 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/temp/dallas.py
--rw-r--r--   0        0        0      243 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/temp/lm75.py
--rw-r--r--   0        0        0      271 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/temp/mcp9808.py
--rw-r--r--   0        0        0       41 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/version.py
--rw-r--r--   0        0        0     1871 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      166 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/tests/32_5_config.yaml
--rw-r--r--   0        0        0      224 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/tests/bandit.yaml
--rw-r--r--   0        0        0     1070 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/tests/relay_32_5.py
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.7.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/LICENSE
+-rw-r--r--   0        0        0      474 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/README.md
+-rw-r--r--   0        0        0      147 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/__init__.py
+-rw-r--r--   0        0        0     3341 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/bonecli.py
+-rw-r--r--   0        0        0     3049 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/const.py
+-rw-r--r--   0        0        0     8454 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/cover.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/__init__.py
+-rw-r--r--   0        0        0      168 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/adc_v0_4.yaml
+-rw-r--r--   0        0        0      238 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/binary_sensor.yaml
+-rw-r--r--   0        0        0      369 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/config.yaml
+-rw-r--r--   0        0        0      150 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/cover.yaml
+-rw-r--r--   0        0        0     2644 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/event.yaml
+-rw-r--r--   0        0        0     3392 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/led32x4A.yaml
+-rw-r--r--   0        0        0     1691 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/output24x16A.yaml
+-rw-r--r--   0        0        0     1713 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/output24x16A_v0.3.yaml
+-rw-r--r--   0        0        0     2403 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/example_config/output32x5A.yaml
+-rw-r--r--   0        0        0    19372 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/fonts/danube__.ttf
+-rw-r--r--   0        0        0     2039 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/__init__.py
+-rw-r--r--   0        0        0      985 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/async_updater.py
+-rw-r--r--   0        0        0     1138 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/click_timer.py
+-rw-r--r--   0        0        0     2321 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/config.py
+-rw-r--r--   0        0        0     7592 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/events.py
+-rw-r--r--   0        0        0      717 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/exceptions.py
+-rw-r--r--   0        0        0      885 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/filter.py
+-rw-r--r--   0        0        0     3249 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/gpio.py
+-rw-r--r--   0        0        0     6359 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/ha_discovery.py
+-rw-r--r--   0        0        0    14687 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/loader.py
+-rw-r--r--   0        0        0     1801 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/logger.py
+-rw-r--r--   0        0        0      765 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/mqtt.py
+-rw-r--r--   0        0        0      351 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/oled.py
+-rw-r--r--   0        0        0     2430 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/onewire/W1ThermSensor.py
+-rw-r--r--   0        0        0      448 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/onewire/__init__.py
+-rw-r--r--   0        0        0     5169 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/onewire/ds2482.py
+-rw-r--r--   0        0        0     2497 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/onewire/onewire.py
+-rw-r--r--   0        0        0     1066 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/queue.py
+-rw-r--r--   0        0        0     1994 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/state_manager.py
+-rw-r--r--   0        0        0     5853 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/stats.py
+-rw-r--r--   0        0        0     5806 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/timeperiod.py
+-rw-r--r--   0        0        0      508 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/util.py
+-rw-r--r--   0        0        0    11304 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/helper/yaml_util.py
+-rw-r--r--   0        0        0      178 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/input/__init__.py
+-rw-r--r--   0        0        0     2611 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/input/gpio.py
+-rw-r--r--   0        0        0     3133 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/input/gpio_beta.py
+-rw-r--r--   0        0        0    22339 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/manager.py
+-rw-r--r--   0        0        0     4176 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/modbus.py
+-rw-r--r--   0        0        0     8645 2023-08-07 20:43:08.219418 boneIO-0.7.0.dev2/boneio/mqtt_client.py
+-rw-r--r--   0        0        0     5244 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/oled.py
+-rw-r--r--   0        0        0      181 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/relay/__init__.py
+-rw-r--r--   0        0        0     2798 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/relay/basic.py
+-rw-r--r--   0        0        0     1163 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/relay/gpio.py
+-rw-r--r--   0        0        0     2506 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/relay/mcp.py
+-rw-r--r--   0        0        0     4871 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/relay/pca.py
+-rw-r--r--   0        0        0     2504 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/relay/pcf.py
+-rw-r--r--   0        0        0     2876 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/runner.py
+-rw-r--r--   0        0        0     1030 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/schema/actions.yaml
+-rw-r--r--   0        0        0      124 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/schema/actions_sensor.yaml
+-rw-r--r--   0        0        0      129 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/schema/actions_switch.yaml
+-rw-r--r--   0        0        0      286 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/schema/filters.yaml
+-rw-r--r--   0        0        0      304 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/schema/filters_adc.yaml
+-rw-r--r--   0        0        0       75 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/schema/id.yaml
+-rw-r--r--   0        0        0    15072 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/schema/schema.yaml
+-rw-r--r--   0        0        0       65 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/schema/temp_unit.yaml
+-rw-r--r--   0        0        0      133 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/schema/update_interval.yaml
+-rw-r--r--   0        0        0      538 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/__init__.py
+-rw-r--r--   0        0        0     1328 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/adc.py
+-rw-r--r--   0        0        0     1296 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/gpio.py
+-rw-r--r--   0        0        0     1291 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/gpio_beta.py
+-rw-r--r--   0        0        0     8520 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/modbus/__init__.py
+-rw-r--r--   0        0        0     8810 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/modbus/dts1964_3f.json
+-rw-r--r--   0        0        0      526 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/modbus/pt100.json
+-rw-r--r--   0        0        0     2735 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/modbus/r4dcb08.json
+-rw-r--r--   0        0        0     4145 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/modbus/sdm120.json
+-rw-r--r--   0        0        0    10969 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/modbus/sdm630.json
+-rw-r--r--   0        0        0     5592 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/modbus/sofar.json
+-rw-r--r--   0        0        0     1808 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/temp/__init__.py
+-rw-r--r--   0        0        0     2485 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/temp/dallas.py
+-rw-r--r--   0        0        0      243 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/temp/lm75.py
+-rw-r--r--   0        0        0      271 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/sensor/temp/mcp9808.py
+-rw-r--r--   0        0        0       41 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/boneio/version.py
+-rw-r--r--   0        0        0     1883 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/tests/32_5_config.yaml
+-rw-r--r--   0        0        0      224 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/tests/bandit.yaml
+-rw-r--r--   0        0        0     1070 2023-08-07 20:43:08.223418 boneIO-0.7.0.dev2/tests/relay_32_5.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.7.0.dev2/PKG-INFO
```

### Comparing `boneIO-0.7.0.dev1/LICENSE` & `boneIO-0.7.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/bonecli.py` & `boneIO-0.7.0.dev2/boneio/bonecli.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/const.py` & `boneIO-0.7.0.dev2/boneio/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -100,18 +100,21 @@
 OFFLINE = "offline"
 TOPIC = "topic"
 TOPIC_PREFIX = "topic_prefix"
 
 # I2C, PCA and MCP CONST
 ADDRESS = "address"
 MCP23017 = "mcp23017"
+PCF8575 = "pcf8575"
 PCA9685 = "pca9685"
 MCP = "mcp"
+PCF = "pcf"
 MCP_ID = "mcp_id"
 PCA_ID = "pca_id"
+PCF_ID = "pcf_id"
 INIT_SLEEP = "init_sleep"
 
 # SENSOR CONST
 TEMPERATURE = "temperature"
 EVENT_ENTITY = "event"
 SENSOR = "sensor"
 BINARY_SENSOR = "binary_sensor"
@@ -137,10 +140,11 @@
 
 # TYPING
 ClickTypes = Literal[SINGLE, DOUBLE, LONG, PRESSED, RELEASED]
 OledDataTypes = Literal[UPTIME, NETWORK, CPU, DISK, MEMORY, SWAP, OUTPUT]
 Gpio_States = Literal[HIGH, LOW]
 Gpio_Edges = Literal[BOTH, FALLING]
 InputTypes = Literal[INPUT, INPUT_SENSOR]
+ExpanderTypes = Literal[MCP23017, PCA9685, PCF8575]
 DEVICE_CLASS = "device_class"
 DallasBusTypes = Literal[DS2482, DALLAS]
 FILTERS = "filters"
```

### Comparing `boneIO-0.7.0.dev1/boneio/cover.py` & `boneIO-0.7.0.dev2/boneio/cover.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/example_config/event.yaml` & `boneIO-0.7.0.dev2/boneio/example_config/event.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/example_config/led32x4A.yaml` & `boneIO-0.7.0.dev2/boneio/example_config/led32x4A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/example_config/output24x16A.yaml` & `boneIO-0.7.0.dev2/boneio/example_config/output24x16A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/example_config/output24x16A_v0.3.yaml` & `boneIO-0.7.0.dev2/boneio/example_config/output24x16A_v0.3.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/example_config/output32x5A.yaml` & `boneIO-0.7.0.dev2/boneio/example_config/output32x5A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/fonts/danube__.ttf` & `boneIO-0.7.0.dev2/boneio/fonts/danube__.ttf`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/__init__.py` & `boneIO-0.7.0.dev2/boneio/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/async_updater.py` & `boneIO-0.7.0.dev2/boneio/helper/async_updater.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/click_timer.py` & `boneIO-0.7.0.dev2/boneio/helper/click_timer.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/config.py` & `boneIO-0.7.0.dev2/boneio/helper/config.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/events.py` & `boneIO-0.7.0.dev2/boneio/helper/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,42 +73,46 @@
         """Return handle."""
         return self._handle
 
 
 class EventBus:
     """Simple event bus which ticks every second."""
 
-    def __init__(self, loop: asyncio.AbstractEventLoop) -> None:
+    def __init__(self, last_will_mqtt = Callable) -> None:
         """Initialize handler"""
-        self._loop = loop or asyncio.get_event_loop()
+        self._loop = asyncio.get_event_loop()
+        self._last_will = last_will_mqtt
+
         self._listeners = {}
         self._sigterm_listeners = []
         self._haonline_listeners = []
         self._timer_handle = _async_create_timer(self._loop, self._run_second_event)
         for signame in {"SIGINT", "SIGTERM"}:
             self._loop.add_signal_handler(
                 getattr(signal, signame),
-                self.ask_exit,
+                lambda: asyncio.create_task(self.ask_exit()),
             )
 
     def _run_second_event(self, time):
         """Run event every second."""
         for key, listener in self._listeners.items():
             if listener.target:
                 self._listeners[key].add_handle(
                     self._loop.call_soon(listener.target, time)
                 )
 
-    def ask_exit(self):
+    async def ask_exit(self):
         """Function to call on exit. Should invoke all sigterm listeners."""
         _LOGGER.debug("Exiting process started.")
         self._listeners = {}
         for target in self._sigterm_listeners:
             target()
         self._timer_handle()
+
+        await self._last_will()
         _LOGGER.info("Shutdown gracefully.")
         raise GracefulExit(code=0)
 
     def add_listener(self, name, target):
         """Add listener on every second job."""
         self._listeners[name] = ListenerJob(target=target)
         return self._listeners[name]
```

### Comparing `boneIO-0.7.0.dev1/boneio/helper/exceptions.py` & `boneIO-0.7.0.dev2/boneio/helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/filter.py` & `boneIO-0.7.0.dev2/boneio/helper/filter.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/gpio.py` & `boneIO-0.7.0.dev2/boneio/helper/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/ha_discovery.py` & `boneIO-0.7.0.dev2/boneio/helper/ha_discovery.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/loader.py` & `boneIO-0.7.0.dev2/boneio/helper/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import time
 from collections import namedtuple
 from typing import TYPE_CHECKING, Any, Callable, Dict, Union
 
 from adafruit_mcp230xx.mcp23017 import MCP23017
 from adafruit_pca9685 import PCA9685
+from adafruit_pcf8575 import PCF8575
 
 from boneio.const import (
     ACTIONS,
     ADDRESS,
     BINARY_SENSOR,
     COVER,
     DEVICE_CLASS,
@@ -33,15 +34,19 @@
     PIN,
     RELAY,
     RESTORE_STATE,
     SENSOR,
     SHOW_HA,
     UPDATE_INTERVAL,
     DallasBusTypes,
-    EVENT_ENTITY
+    EVENT_ENTITY,
+    ExpanderTypes,
+    PCF,
+    PCA,
+    PCF_ID
 )
 from boneio.cover import Cover
 from boneio.helper import (
     GPIOInputException,
     GPIOOutputException,
     I2CError,
     StateManager,
@@ -144,61 +149,48 @@
             unit_of_measurement=config.get("unit_of_measurement", "°C"),
         )
         return temp_sensor
     except I2CError as err:
         _LOGGER.error("Can't configure Temp sensor. %s", err)
         pass
 
-
-def create_mcp23017(
-    manager: Manager,
-    mcp23017: list,
-    i2cbusio: I2C,
+expander_class = {
+    MCP: MCP23017,
+    PCA: PCA9685,
+    PCF: PCF8575
+}
+
+def create_expander(
+        expander_dict: dict,
+        expander_config: list,
+        exp_type: ExpanderTypes,
+        i2cbusio: I2C
 ) -> dict:
-    """Create MCP23017."""
     grouped_outputs = {}
-    for mcp in mcp23017:
-        id = mcp[ID] or mcp[ADDRESS]
+    for expander in expander_config:
+        id = expander[ID] or expander[ADDRESS]
         try:
-            manager._mcp[id] = MCP23017(i2c=i2cbusio, address=mcp[ADDRESS], reset=False)
-            sleep_time = mcp.get(INIT_SLEEP, TimePeriod(seconds=0))
-            _LOGGER.debug(
-                f"Sleeping for {sleep_time.total_seconds}s while MCP {id} is initializing."
-            )
-            time.sleep(sleep_time.total_seconds)
+            expander_dict[id] = expander_class[exp_type](i2c=i2cbusio, address=expander[ADDRESS], reset=False)
+            sleep_time = expander.get(INIT_SLEEP, TimePeriod(seconds=0))
+            if sleep_time.total_seconds > 0:
+                _LOGGER.debug(
+                    f"Sleeping for {sleep_time.total_seconds}s while {exp_type} {id} is initializing."
+                )
+                time.sleep(sleep_time.total_seconds)
+            else:
+                _LOGGER.debug(
+                    f"{exp_type} {id} is initializing."
+                )
             grouped_outputs[id] = {}
         except TimeoutError as err:
-            _LOGGER.error("Can't connect to MCP %s. %s", id, err)
+            _LOGGER.error("Can't connect to %s %s. %s", exp_type, id, err)
             pass
     return grouped_outputs
 
 
-def create_pca9685(
-    manager: Manager,
-    pca9685: list,
-    i2cbusio: I2C,
-) -> dict:
-    """Create MCP23017."""
-    grouped_outputs = {}
-    for pca in pca9685:
-        id = pca[ID] or pca[ADDRESS]
-        try:
-            manager._pca[id] = PCA9685(i2c_bus=i2cbusio, address=pca[ADDRESS])
-            manager._pca[id].frequency = 500
-            sleep_time = pca.get(INIT_SLEEP, TimePeriod(seconds=0))
-            _LOGGER.debug(
-                f"Sleeping for {sleep_time.total_seconds}s while PCA {id} is initializing."
-            )
-            time.sleep(sleep_time.total_seconds)
-            grouped_outputs[id] = {}
-        except TimeoutError as err:
-            _LOGGER.error("Can't connect to PCA %s. %s", id, err)
-            pass
-    return grouped_outputs
-
 
 def create_modbus_sensors(manager: Manager, sensors, **kwargs) -> None:
     """Create Modbus sensor for each device."""
     from boneio.sensor.modbus import ModbusSensor
 
     for sensor in sensors:
         name = sensor.get(ID)
@@ -232,14 +224,17 @@
         output_id = config.pop(MCP_ID, None)
         return OutputEntry(MCPRelay, MCP, output_id)
     elif output_kind == GPIO:
         return OutputEntry(GpioRelay, GPIO, GPIO)
     elif output_kind == PCA:
         output_id = config.pop(PCA_ID, None)
         return OutputEntry(PWMPCA, PCA, output_id)
+    elif output_kind == PCF:
+        output_id = config.pop(PCF_ID, None)
+        return OutputEntry(PWMPCA, PCF, output_id)
     else:
         raise GPIOOutputException(f"""Output type {output_kind} dont exists""")
 
 
 def configure_relay(
     manager: Manager,
     state_manager: StateManager,
@@ -369,15 +364,15 @@
     pin: str,
     press_callback: Callable,
     send_ha_autodiscovery: Callable,
 ) -> str:
     """Configure input sensor or button."""
     try:
         GpioInputBinarySensorClass = GpioInputBinarySensor if gpio.get("detection_type", "stable") == "stable" else GpioInputBinarySensorBeta
-        GpioInputBinarySensor(
+        GpioInputBinarySensorClass(
             pin=pin,
             press_callback=lambda x, i: press_callback(
                 x=x,
                 inpin=i,
                 actions=gpio.get(ACTIONS, {}).get(x, []),
                 input_type=INPUT_SENSOR,
                 empty_message_after=gpio.get("clear_message", False)
```

### Comparing `boneIO-0.7.0.dev1/boneio/helper/logger.py` & `boneIO-0.7.0.dev2/boneio/helper/logger.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/mqtt.py` & `boneIO-0.7.0.dev2/boneio/helper/mqtt.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/onewire/W1ThermSensor.py` & `boneIO-0.7.0.dev2/boneio/helper/onewire/W1ThermSensor.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/onewire/ds2482.py` & `boneIO-0.7.0.dev2/boneio/helper/onewire/ds2482.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/onewire/onewire.py` & `boneIO-0.7.0.dev2/boneio/helper/onewire/onewire.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/queue.py` & `boneIO-0.7.0.dev2/boneio/helper/queue.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/state_manager.py` & `boneIO-0.7.0.dev2/boneio/helper/state_manager.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/stats.py` & `boneIO-0.7.0.dev2/boneio/helper/stats.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/timeperiod.py` & `boneIO-0.7.0.dev2/boneio/helper/timeperiod.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/helper/yaml_util.py` & `boneIO-0.7.0.dev2/boneio/helper/yaml_util.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/input/gpio.py` & `boneIO-0.7.0.dev2/boneio/input/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/input/gpio_beta.py` & `boneIO-0.7.0.dev2/boneio/input/gpio_beta.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/manager.py` & `boneIO-0.7.0.dev2/boneio/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     ClickTypes,
     InputTypes,
     relay_actions,
     DS2482,
     LIGHT,
     LED,
     SET_BRIGHTNESS,
+    MCP,
+    PCA,
+    PCF
 )
 from boneio.helper import (
     GPIOInputException,
     HostData,
     I2CError,
     StateManager,
     ha_button_availabilty_message,
@@ -53,16 +56,15 @@
 from boneio.helper.exceptions import ModbusUartException
 from boneio.helper.loader import (
     configure_cover,
     configure_event_sensor,
     configure_binary_sensor,
     configure_relay,
     create_dallas_sensor,
-    create_mcp23017,
-    create_pca9685,
+    create_expander,
     create_temp_sensor,
 )
 from boneio.helper.logger import configure_logger
 from boneio.helper.yaml_util import load_config_from_file
 from boneio.modbus import Modbus
 
 from w1thermsensor.errors import KernelModuleLoadError
@@ -80,22 +82,24 @@
 
     def __init__(
         self,
         send_message: Callable[[str, Union[str, dict], bool], None],
         stop_client: Callable[[], Awaitable[None]],
         state_manager: StateManager,
         config_helper: ConfigHelper,
+        event_bus: EventBus,
         config_file_path: str,
         relay_pins: List = [],
         event_pins: List = [],
         binary_pins: List = [],
         sensors: dict = {},
         modbus: dict = {},
         pca9685: list = [],
         mcp23017: list = [],
+        pcf8575: list = [],
         ds2482: Optional[List] = [],
         dallas: Optional[dict] = None,
         oled: dict = {},
         adc: Optional[List] = None,
         cover: list = [],
     ) -> None:
         """Initialize the manager."""
@@ -103,22 +107,23 @@
 
         self._loop = asyncio.get_event_loop()
 
         self._config_helper = config_helper
         self._host_data = None
         self._config_file_path = config_file_path
         self._state_manager = state_manager
-        self._event_bus = EventBus(self._loop)
+        self._event_bus = event_bus
 
         self.send_message = send_message
         self.stop_client = stop_client
         self._event_pins = event_pins
         self._binary_pins = binary_pins
         self._i2cbusio = I2C(SCL, SDA)
         self._mcp = {}
+        self._pcf = {}
         self._pca = {}
         self._output = {}
         self._oled = None
         self._tasks: List[asyncio.Task] = []
         self._covers = {}
         self._temp_sensors = []
         self._modbus = None
@@ -128,19 +133,35 @@
         self._configure_temp_sensors(sensors=sensors)
 
         self._configure_modbus_sensors(sensors=sensors)
         self._configure_sensors(
             dallas=dallas, ds2482=ds2482, sensors=sensors.get(ONEWIRE)
         )
 
-        self.grouped_outputs = create_mcp23017(
-            manager=self, mcp23017=mcp23017, i2cbusio=self._i2cbusio
+        self.grouped_outputs = create_expander(
+            expander_dict=self._mcp,
+            expander_config=mcp23017,
+            exp_type=MCP,
+            i2cbusio=self._i2cbusio
         )
         self.grouped_outputs.update(
-            create_pca9685(manager=self, pca9685=pca9685, i2cbusio=self._i2cbusio)
+            create_expander(
+            expander_dict=self._pcf,
+            expander_config=pcf8575,
+            exp_type=PCF,
+            i2cbusio=self._i2cbusio
+        )
+        )
+        self.grouped_outputs.update(
+            create_expander(
+            expander_dict=self._pca,
+            expander_config=pca9685,
+            exp_type=PCA,
+            i2cbusio=self._i2cbusio
+        )
         )
 
         self._configure_adc(adc_list=adc)
 
         for _config in relay_pins:
             _id = _config[ID].replace(" ", "")
             out = configure_relay(
@@ -452,14 +473,19 @@
         """Get MCP by it's id."""
         return self._mcp
 
     @property
     def pca(self):
         """Get PCA by it's id."""
         return self._pca
+    
+    @property
+    def pcf(self):
+        """Get PCF by it's id."""
+        return self._pcf
 
     def press_callback(
         self, x: ClickTypes, inpin: str, actions: List, input_type: InputTypes = INPUT, empty_message_after: bool = False
     ) -> None:
         """Press callback to use in input gpio.
         If relay input map is provided also toggle action on relay or cover or mqtt."""
         topic = f"{self._config_helper.topic_prefix}/{input_type}/{inpin}"
```

### Comparing `boneIO-0.7.0.dev1/boneio/modbus.py` & `boneIO-0.7.0.dev2/boneio/modbus.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/mqtt_client.py` & `boneIO-0.7.0.dev2/boneio/mqtt_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Any, Callable, Optional, Set, Union, Awaitable
 
 import paho.mqtt.client as mqtt
 from aiomqtt import Client as AsyncioClient, MqttError, Will
 from paho.mqtt.properties import Properties
 from paho.mqtt.subscribeoptions import SubscribeOptions
 
-from boneio.const import ONLINE, PAHO, STATE
+from boneio.const import ONLINE, OFFLINE, PAHO, STATE
 from boneio.helper import UniqueQueue
 from boneio.helper.config import ConfigHelper
 from boneio.manager import Manager
 from boneio.helper.exceptions import RestartRequestException
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -124,15 +124,15 @@
         params: dict = {"timeout": timeout}
         if properties:
             params["properties"] = properties
 
         await self.asyncio_client.unsubscribe(topic=topics, **params)
 
     def send_message(
-        self, topic: str, payload: Union[str, dict, None], retain: bool = False
+        self, topic: str, payload: Union[str, int, dict, None], retain: bool = False
     ) -> None:
         """Send a message from the manager options."""
         to_publish = (
             topic,
             json.dumps(payload) if type(payload) == dict else payload,
             retain,
         )
@@ -157,20 +157,27 @@
                     "MQTT error: %s. Reconnecting in %s seconds",
                     err,
                     self.reconnect_interval,
                 )
                 self._connection_established = False
                 await asyncio.sleep(self.reconnect_interval)
                 self.create_client()  # reset connect/reconnect futures
+            except asyncio.CancelledError:
+                _LOGGER.info("MQTT client task canceled.")
 
     async def stop_client(self) -> None:
         await self.unsubscribe(
             topics=self._topics
         )
         raise RestartRequestException("Restart requested.")
+    
+    async def last_will_mqtt(self) -> None:
+        _LOGGER.info("Sending offline state.")
+        topic = f"{self._config_helper.topic_prefix}/{STATE}"
+        self.send_message(topic=topic, payload=OFFLINE, retain=True)
 
     async def _subscribe_manager(self, manager: Manager) -> None:
         """Connect and subscribe to manager topics + host stats."""
         async with AsyncExitStack() as stack:
             tasks: Set[asyncio.Task] = set()
 
             # Connect to the MQTT broker.
```

### Comparing `boneIO-0.7.0.dev1/boneio/oled.py` & `boneIO-0.7.0.dev2/boneio/oled.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/relay/basic.py` & `boneIO-0.7.0.dev2/boneio/relay/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Basic Relay module."""
 
 import asyncio
 import logging
 from typing import Callable
-
+from boneio.helper.util import callback
 from boneio.const import LIGHT, NONE, OFF, ON, RELAY, STATE, SWITCH
 from boneio.helper import BasicMqtt
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class BasicRelay(BasicMqtt):
@@ -78,14 +78,19 @@
         """Toggle relay."""
         _LOGGER.debug("Toggle relay.")
         if self.is_active:
             self.turn_off()
         else:
             self.turn_on()
 
+    @callback
+    def _momentary_callback(self, time, action):
+        _LOGGER.info("Momentary callback at %s", time)
+        action()
+
     @property
     def is_active(self) -> bool:
         """Is active check."""
         raise NotImplementedError
 
     def turn_on(self) -> None:
         """Call turn on action."""
```

### Comparing `boneIO-0.7.0.dev1/boneio/relay/gpio.py` & `boneIO-0.7.0.dev2/boneio/relay/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/relay/mcp.py` & `boneIO-0.7.0.dev2/boneio/relay/mcp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """MCP23017 Relay module."""
 
 import logging
 
 from adafruit_mcp230xx.mcp23017 import MCP23017, DigitalInOut
 
-from boneio.const import NONE, SWITCH
+from boneio.const import NONE, SWITCH, MCP
 from boneio.helper.events import async_track_point_in_time, utcnow
-from boneio.helper.util import callback
 from boneio.relay.basic import BasicRelay
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class MCPRelay(BasicRelay):
     """Represents MCP Relay output"""
@@ -30,47 +29,42 @@
             """Just in case to not restore state of covers etc."""
             restored_state = False
         self._pin.switch_to_output(value=restored_state)
         super().__init__(
             **kwargs, output_type=output_type, restored_state=restored_state
         )
         self._pin_id = pin
-        self._mcp_id = mcp_id
+        self._expander_id = mcp_id
         _LOGGER.debug("Setup MCP with pin %s", self._pin_id)
 
     @property
-    def is_mcp_type(self) -> bool:
-        """Check if relay is mcp type."""
-        return True
+    def expander_type(self) -> str:
+        """Check expander type."""
+        return MCP
 
     @property
-    def pin_id(self) -> str:
+    def pin_id(self) -> int:
         """Return PIN id."""
         return self._pin_id
 
     @property
-    def mcp_id(self) -> str:
+    def expander_id(self) -> str:
         """Retrieve parent MCP ID."""
-        return self._mcp_id
+        return self._expander_id
 
     @property
     def is_active(self) -> bool:
         """Is relay active."""
         return self.pin.value
 
     @property
     def pin(self) -> str:
         """PIN of the relay"""
         return self._pin
 
-    @callback
-    def _momentary_callback(self, time, action):
-        _LOGGER.info("Momentary callback at %s", time)
-        action()
-
     def turn_on(self) -> None:
         """Call turn on action."""
         self.pin.value = True
         if self._momentary_turn_on:
             async_track_point_in_time(
                 loop=self._loop,
                 action=lambda x: self._momentary_callback(time=x, action=self.turn_off),
```

### Comparing `boneIO-0.7.0.dev1/boneio/relay/pca.py` & `boneIO-0.7.0.dev2/boneio/relay/pca.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 from typing import Callable
 from adafruit_pca9685 import PCA9685, PCAChannels
 
 from boneio.helper.events import async_track_point_in_time, utcnow
 from boneio.helper.util import callback
 
-from boneio.const import LED, NONE, OFF, ON, STATE, SWITCH, BRIGHTNESS, RELAY
+from boneio.const import LED, NONE, OFF, ON, STATE, SWITCH, BRIGHTNESS, RELAY, PCA
 from boneio.helper import BasicMqtt
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PWMPCA(BasicMqtt):
     """Initialize PWMPCA."""
@@ -54,17 +54,17 @@
         self._callback = callback
         self._loop = asyncio.get_running_loop()
 
         self._pin_id = pin
         _LOGGER.debug("Setup PCA with pin %s", self._pin_id)
 
     @property
-    def is_pca_type(self) -> bool:
-        """Check if relay is pca type."""
-        return True
+    def expander_type(self) -> str:
+        """Check expander type."""
+        return PCA
 
     @property
     def output_type(self) -> str:
         """HA type."""
         return self._output_type
 
     @property
```

### Comparing `boneIO-0.7.0.dev1/boneio/runner.py` & `boneIO-0.7.0.dev2/boneio/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     DS2482,
     ENABLED,
     HA_DISCOVERY,
     HOST,
     EVENT_ENTITY,
     LM75,
     MCP23017,
+    PCF8575,
     PCA9685,
     MCP_TEMP_9808,
     MODBUS,
     MQTT,
     OLED,
     ONEWIRE,
     OUTPUT,
@@ -30,19 +31,21 @@
     TOPIC_PREFIX,
     USERNAME,
 )
 from boneio.helper import StateManager
 from boneio.helper.config import ConfigHelper
 from boneio.manager import Manager
 from boneio.mqtt_client import MQTTClient
+from boneio.helper.events import EventBus
 
 _LOGGER = logging.getLogger(__name__)
 
 config_modules = [
     {"name": MCP23017, "default": []},
+    {"name": PCF8575, "default": []},
     {"name": PCA9685, "default": []},
     {"name": DS2482, "default": []},
     {"name": ADC, "default": []},
     {"name": COVER, "default": []},
     {"name": MODBUS, "default": {}},
     {"name": OLED, "default": {}},
     {"name": DALLAS, "default": None},
@@ -52,36 +55,39 @@
 async def async_run(
     config: dict,
     config_file: str,
     mqttusername: str = "",
     mqttpassword: str = "",
 ) -> list[Any]:
     """Run BoneIO."""
+    _loop = asyncio.get_event_loop()
 
     _config_helper = ConfigHelper(
         topic_prefix=config[MQTT].pop(TOPIC_PREFIX),
         ha_discovery=config[MQTT][HA_DISCOVERY].pop(ENABLED),
         ha_discovery_prefix=config[MQTT][HA_DISCOVERY].pop(TOPIC_PREFIX),
     )
 
     client = MQTTClient(
         host=config[MQTT][HOST],
         username=config[MQTT].get(USERNAME, mqttusername),
         password=config[MQTT].get(PASSWORD, mqttpassword),
         port=config[MQTT].get(PORT, 1883),
         config_helper=_config_helper,
     )
+    event_bus =  EventBus(last_will_mqtt=client.last_will_mqtt)
     manager_kwargs = {
         item["name"]: config.get(item["name"], item["default"])
         for item in config_modules
     }
 
     manager = Manager(
         send_message=client.send_message,
         stop_client=client.stop_client,
+        event_bus=event_bus,
         relay_pins=config.get(OUTPUT, []),
         event_pins=config.get(EVENT_ENTITY, []),
         binary_pins=config.get(BINARY_SENSOR, []),
         config_file_path=config_file,
         state_manager=StateManager(
             state_file=f"{os.path.split(config_file)[0]}state.json"
         ),
```

### Comparing `boneIO-0.7.0.dev1/boneio/schema/actions.yaml` & `boneIO-0.7.0.dev2/boneio/schema/actions.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/schema/schema.yaml` & `boneIO-0.7.0.dev2/boneio/schema/schema.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/__init__.py` & `boneIO-0.7.0.dev2/boneio/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/adc.py` & `boneIO-0.7.0.dev2/boneio/sensor/adc.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/gpio.py` & `boneIO-0.7.0.dev2/boneio/sensor/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/gpio_beta.py` & `boneIO-0.7.0.dev2/boneio/sensor/gpio_beta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """GpioInputBinarySensor to receive signals."""
 import logging
 from functools import partial
-from boneio.const import PRESSED, RELEASED
+from boneio.const import PRESSED, RELEASED, BOTH
 from boneio.helper import GpioBaseClass
 from boneio.helper.gpio import add_event_callback, add_event_detect
+
 _LOGGER = logging.getLogger(__name__)
 
 
 class GpioInputBinarySensorBeta(GpioBaseClass):
     """Represent Gpio sensor on input boards."""
 
     def __init__(self, **kwargs) -> None:
```

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/modbus/__init__.py` & `boneIO-0.7.0.dev2/boneio/sensor/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/modbus/dts1964_3f.json` & `boneIO-0.7.0.dev2/boneio/sensor/modbus/dts1964_3f.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/modbus/pt100.json` & `boneIO-0.7.0.dev2/boneio/sensor/modbus/pt100.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/modbus/r4dcb08.json` & `boneIO-0.7.0.dev2/boneio/sensor/modbus/r4dcb08.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/modbus/sdm120.json` & `boneIO-0.7.0.dev2/boneio/sensor/modbus/sdm120.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/modbus/sdm630.json` & `boneIO-0.7.0.dev2/boneio/sensor/modbus/sdm630.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/modbus/sofar.json` & `boneIO-0.7.0.dev2/boneio/sensor/modbus/sofar.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/temp/__init__.py` & `boneIO-0.7.0.dev2/boneio/sensor/temp/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/boneio/sensor/temp/dallas.py` & `boneIO-0.7.0.dev2/boneio/sensor/temp/dallas.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/pyproject.toml` & `boneIO-0.7.0.dev2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -22,32 +22,31 @@
     "pyserial-asyncio>=0.6",
     "PyYAML>=6.0.1",
     "Adafruit-BBIO>=1.2.0",
     "psutil>=5.9.5",
     "adafruit-circuitpython-onewire>=2.0.5",
     "w1thermsensor[async]>=2.0.0",
     "adafruit-circuitpython-pca9685>=3.4.10",
+    "adafruit-circuitpython-pcf8575>=1.0.2",
 ]
 requires-python = ">=3.7"
-version = "0.7.0.dev1"
+version = "0.7.0.dev2"
 
 [project.license]
 text = "GNU General Public License v3.0"
 
 [project.urls]
 Homepage = "https://boneio.eu"
 Repository = "https://github.com/boneIO-eu/app_bbb"
 Documentation = "https://boneio.eu/docs/intro/"
 Changelog = "https://github.com/boneIO-eu/app_bbb/releases"
 
 [project.scripts]
 boneio = "boneio.bonecli:main"
 
-[project.optional-dependencies]
-
 [tool.pdm.version]
 from = "boneio/version.py"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=23.3.0",
     "isort>=5.11.5",
```

### Comparing `boneIO-0.7.0.dev1/tests/relay_32_5.py` & `boneIO-0.7.0.dev2/tests/relay_32_5.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.7.0.dev1/PKG-INFO` & `boneIO-0.7.0.dev2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boneIO
-Version: 0.7.0.dev1
+Version: 0.7.0.dev2
 Summary: Python App for BoneIO
 License: GNU General Public License v3.0
 Author-email: Paweł Szafer <pszafer@gmail.com>
 Requires-Python: >=3.7
 Project-URL: Changelog, https://github.com/boneIO-eu/app_bbb/releases
 Project-URL: Documentation, https://boneio.eu/docs/intro/
 Project-URL: Homepage, https://boneio.eu
```

