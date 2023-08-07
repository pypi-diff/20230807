# Comparing `tmp/shepherd_core-2023.6.5.tar.gz` & `tmp/shepherd_core-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2023.6.5.tar", last modified: Mon Jun 19 10:58:09 2023, max compression
+gzip compressed data, was "shepherd_core-2023.8.1.tar", last modified: Mon Aug  7 13:55:14 2023, max compression
```

## Comparing `shepherd_core-2023.6.5.tar` & `shepherd_core-2023.8.1.tar`

### file list

```diff
@@ -1,123 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.440589 shepherd_core-2023.6.5/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/calibration_hw_def.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.440589 shepherd_core-2023.6.5/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.440589 shepherd_core-2023.6.5/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/cal_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.444590 shepherd_core-2023.6.5/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/energy_environment_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/firmware_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_source_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/doc_virtual_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.444590 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/experiment/target_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.444590 shepherd_core-2023.6.5/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/harvest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/programming.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.444590 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/cape_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/gpio_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/mcu_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/observer_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/target_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/testbed.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/data_models/testbed/testbed_fixture.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.448591 shepherd_core-2023.6.5/shepherd_core/fw_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/fw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/fw_tools/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/fw_tools/patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/fw_tools/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.448591 shepherd_core-2023.6.5/shepherd_core/testbed_client/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/testbed_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/testbed_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/testbed_client/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/testbed_client/user_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.448591 shepherd_core-2023.6.5/shepherd_core/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/vsource/virtual_converter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/vsource/virtual_harvester_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/vsource/virtual_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:58:09.000000 shepherd_core-2023.6.5/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.448591 shepherd_core-2023.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/tests/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_data_faulty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_meas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_meas_faulty1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_cal_meas_faulty2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_emulator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_experiment_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_harvester.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_testbed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/example_config_virtsource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_content_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_task_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_task_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_testbed_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/data_models/test_testbed_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/tests/fw_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/fw_tools/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_cal_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:58:09.452593 shepherd_core-2023.6.5/tests/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/vsource/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/vsource/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-19 10:57:57.000000 shepherd_core-2023.6.5/tests/vsource/test_harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.869520 shepherd_core-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-08-07 13:55:14.869520 shepherd_core-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-07 13:55:14.869520 shepherd_core-2023.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.857519 shepherd_core-2023.8.1/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.857519 shepherd_core-2023.8.1/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.857519 shepherd_core-2023.8.1/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.857519 shepherd_core-2023.8.1/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/content/firmware_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/content/virtual_source_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/doc_virtual_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.861519 shepherd_core-2023.8.1/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/experiment/target_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.861519 shepherd_core-2023.8.1/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.861519 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/data_models/testbed/testbed_fixture.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.861519 shepherd_core-2023.8.1/shepherd_core/decoder_waveform/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/decoder_waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/decoder_waveform/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.861519 shepherd_core-2023.8.1/shepherd_core/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/fw_tools/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/fw_tools/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/fw_tools/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.861519 shepherd_core-2023.8.1/shepherd_core/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/inventory/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/inventory/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/inventory/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.865520 shepherd_core-2023.8.1/shepherd_core/testbed_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/testbed_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/testbed_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/testbed_client/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/testbed_client/user_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.865520 shepherd_core-2023.8.1/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.869520 shepherd_core-2023.8.1/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-08-07 13:55:14.000000 shepherd_core-2023.8.1/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-08-07 13:55:14.000000 shepherd_core-2023.8.1/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:55:14.000000 shepherd_core-2023.8.1/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-07 13:55:14.000000 shepherd_core-2023.8.1/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 13:55:14.000000 shepherd_core-2023.8.1/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:55:14.000000 shepherd_core-2023.8.1/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.865520 shepherd_core-2023.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.865520 shepherd_core-2023.8.1/tests/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_cal_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_cal_data_faulty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_cal_meas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_cal_meas_faulty1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_cal_meas_faulty2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_config_emulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_config_harvester.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_config_testbed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/example_config_virtsource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/data_models/test_testbed_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.869520 shepherd_core-2023.8.1/tests/decoder_waveform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/decoder_waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/decoder_waveform/test_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.869520 shepherd_core-2023.8.1/tests/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/fw_tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/fw_tools/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/fw_tools/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/fw_tools/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.869520 shepherd_core-2023.8.1/tests/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/inventory/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.869520 shepherd_core-2023.8.1/tests/testbed_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/testbed_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:14.869520 shepherd_core-2023.8.1/tests/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/vsource/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/vsource/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/vsource/test_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 13:55:05.000000 shepherd_core-2023.8.1/tests/vsource/test_z.py
```

### Comparing `shepherd_core-2023.6.5/PKG-INFO` & `shepherd_core-2023.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2023.6.5
+Version: 2023.8.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: elf
+Provides-Extra: inventory
 Provides-Extra: dev
 Provides-Extra: test
 
 # Shepherd - Core
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
 [![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
@@ -57,16 +58,17 @@
 - read and write shepherds h5-files
 - create, read, write and convert experiments for the testbed (all data-models included)
 - simulate the virtual source, including virtual harvesters
 - connect and query the testbed via a webclient (TestbedClient)
 - work with target-firmwares
   - embed, modify, verify, convert
   - **Note**: working with ELF-files requires external dependencies, see ``Installation``-Chapter
+- decode waveforms -> uart
 
-see [examples](/examples) for more details.
+see [examples](./examples) for more details.
 
 # Installation
 
 The Library is available via PyPI and can be installed with
 
 ```shell
   pip install shepherd-core
@@ -84,7 +86,13 @@
 For more advanced work with ``.elf``-files (modify value of symbols / target-ID) you should install
 
 ```shell
   pip install shepherd-core[elf]
 ```
 
 and also make sure the prereqs for the [pwntools](https://docs.pwntools.com/en/stable/install.html) are met.
+
+For creating an inventory of the host-system you should install
+
+```shell
+  pip install shepherd-core[inventory]
+```
```

### Comparing `shepherd_core-2023.6.5/README.md` & `shepherd_core-2023.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 - read and write shepherds h5-files
 - create, read, write and convert experiments for the testbed (all data-models included)
 - simulate the virtual source, including virtual harvesters
 - connect and query the testbed via a webclient (TestbedClient)
 - work with target-firmwares
   - embed, modify, verify, convert
   - **Note**: working with ELF-files requires external dependencies, see ``Installation``-Chapter
+- decode waveforms -> uart
 
-see [examples](/examples) for more details.
+see [examples](./examples) for more details.
 
 # Installation
 
 The Library is available via PyPI and can be installed with
 
 ```shell
   pip install shepherd-core
@@ -48,7 +49,13 @@
 For more advanced work with ``.elf``-files (modify value of symbols / target-ID) you should install
 
 ```shell
   pip install shepherd-core[elf]
 ```
 
 and also make sure the prereqs for the [pwntools](https://docs.pwntools.com/en/stable/install.html) are met.
+
+For creating an inventory of the host-system you should install
+
+```shell
+  pip install shepherd-core[inventory]
+```
```

### Comparing `shepherd_core-2023.6.5/setup.cfg` & `shepherd_core-2023.8.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 	tqdm
 	scipy
 	intelhex
 
 [options.extras_require]
 elf = 
 	pwntools
+inventory = 
+	psutil
 dev = 
 	black
 	pylint
 	flake8
 	twine
 	pre-commit
 	pyright
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/__init__.py` & `shepherd_core-2023.8.1/shepherd_core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 from .data_models.base.calibration import Calc_t
 from .data_models.base.calibration import CalibrationCape
 from .data_models.base.calibration import CalibrationEmulator
 from .data_models.base.calibration import CalibrationHarvester
 from .data_models.base.calibration import CalibrationPair
 from .data_models.base.calibration import CalibrationSeries
 from .data_models.task import Compression
+from .inventory import Inventory
 from .logger import get_verbose_level
 from .logger import logger
 from .logger import set_verbose_level
 from .reader import BaseReader
 from .testbed_client.client import TestbedClient
 from .testbed_client.client import tb_client
 from .writer import BaseWriter
 
-__version__ = "2023.6.5"
+__version__ = "2023.8.1"
 
 __all__ = [
     "BaseReader",
     "BaseWriter",
     "get_verbose_level",
     "set_verbose_level",
     "logger",
@@ -33,8 +34,9 @@
     "CalibrationEmulator",
     "CalibrationHarvester",
     "CalibrationPair",
     "Calc_t",
     "Compression",
     "TestbedClient",
     "tb_client",  # using this (instead of the Class) is the cleaner, but less pythonic way
+    "Inventory",
 ]
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/calibration_hw_def.py` & `shepherd_core-2023.8.1/shepherd_core/calibration_hw_def.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,31 +33,29 @@
 
 
 def adc_current_to_raw(current: float) -> int:
     # voltage on input of adc
     val_adc = G_INST_AMP * R_SHT * current
     # digital value according to ADC gain
     val_raw = int(val_adc * (2**M_ADC) / (G_ADC_I * V_REF_ADC))
-    val_raw = min(max(val_raw, 0), 2**M_ADC - 1)
-    return val_raw
+    return min(max(val_raw, 0), 2**M_ADC - 1)
 
 
 def adc_raw_to_current(value: int) -> float:
     value = min(max(value, 0), 2**M_ADC - 1)
     # voltage on input of adc
     val_adc = float(value) * (G_ADC_I * V_REF_ADC) / (2**M_ADC)
     # current according to adc value
     return val_adc / (R_SHT * G_INST_AMP)
 
 
 def adc_voltage_to_raw(voltage: float) -> int:
     # digital value according to ADC gain
     val_raw = int(voltage * (2**M_ADC) / (G_ADC_V * V_REF_ADC))
-    val_raw = min(max(val_raw, 0), 2**M_ADC - 1)
-    return val_raw
+    return min(max(val_raw, 0), 2**M_ADC - 1)
 
 
 def adc_raw_to_voltage(value: int) -> float:
     value = min(max(value, 0), 2**M_ADC - 1)
     # voltage according to ADC value
     return float(value) * (G_ADC_V * V_REF_ADC) / (2**M_ADC)
 
@@ -65,9 +63,8 @@
 def dac_raw_to_voltage(value: int) -> float:
     value = min(max(value, 0), 2**M_DAC - 1)
     return float(value) * (V_REF_DAC * G_DAC) / (2**M_DAC)
 
 
 def dac_voltage_to_raw(voltage: float) -> int:
     val_raw = int(voltage * (2**M_DAC) / (V_REF_DAC * G_DAC))
-    val_raw = min(max(val_raw, 0), 2**M_DAC - 1)
-    return val_raw
+    return min(max(val_raw, 0), 2**M_DAC - 1)
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/__init__.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,8 +42,8 @@
     "GpioActuation",
     "GpioEvent",
     "GpioLevel",
     "EnergyEnvironment",
     "EnergyDType",
     "VirtualSourceConfig",
     "VirtualHarvesterConfig",
-]
+]  # TODO: for pydantic 2 add @classmethod after @root_validator for cleaner type-checking
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/base/cal_measurement.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/base/cal_measurement.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from .. import CalibrationCape
 from .. import CalibrationEmulator
 from .. import CalibrationHarvester
 from .. import CalibrationPair
 from .shepherd import ShpModel
 
-# TODO: move to shepherd_data to remove scipy-dependency
+# TODO: move to shepherd_data to remove scipy-dependency from _core
 
 
 class CalMeasurementPair(ShpModel):
     shepherd_raw: PositiveFloat
     reference_si: float = 0
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/base/calibration.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/base/calibration.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/base/content.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/base/content.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/base/shepherd.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/base/shepherd.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/content/energy_environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 from pathlib import Path
+from typing import Optional
 
 from pydantic import PositiveFloat
 from pydantic import root_validator
 
 from ...testbed_client import tb_client
 from ..base.content import ContentModel
 
@@ -26,12 +27,17 @@
 
     duration: PositiveFloat
     energy_Ws: PositiveFloat
     valid: bool = False
 
     # TODO: scale up/down voltage/current
 
+    # additional descriptive metadata
+    light_source: Optional[str] = None
+    weather_conditions: Optional[str] = None
+    indoor: Optional[bool] = None
+    location: Optional[str] = None
+
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
-        values = tb_client.fill_in_user_data(values)
-        return values
+        return tb_client.fill_in_user_data(values)
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/content/energy_environment_fixture.yaml` & `shepherd_core-2023.8.1/shepherd_core/data_models/content/energy_environment_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/content/firmware.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/content/firmware.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,15 @@
     data_type: FirmwareDType
 
     # TODO: a data-hash would be awesome
 
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
-        values = tb_client.fill_in_user_data(values)
-        return values
+        return tb_client.fill_in_user_data(values)
 
     @classmethod
     def from_firmware(cls, file: Path, **kwargs):
         """embeds firmware and tries to fill parameters
         ELF -> mcu und data_type are deducted
         HEX -> must supply mcu manually
         """
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/content/firmware_fixture.yaml` & `shepherd_core-2023.8.1/shepherd_core/data_models/content/firmware_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_harvester.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/content/virtual_harvester.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     def calc_algorithm_num(self, for_emu: bool) -> int:
         num = algo_to_num.get(self.algorithm)
         if for_emu and self.get_datatype() != EnergyDType.ivsample:
             raise ValueError(
                 f"[{self.name}] Select valid harvest-algorithm for emulator, "
                 f"current usage = {self.algorithm}",
             )
-        elif num < algo_to_num["isc_voc"]:
+        if num < algo_to_num["isc_voc"]:
             raise ValueError(
                 f"[{self.name}] Select valid harvest-algorithm for harvester, "
                 f"current usage = {self.algorithm}",
             )
         return num
 
     def calc_timings_ms(self, for_emu: bool) -> Tuple[float, float]:
@@ -141,21 +141,21 @@
 
     def calc_window_size(
         self, for_emu: bool, dtype_in: Optional[EnergyDType] = EnergyDType.ivsample
     ) -> int:
         if for_emu:
             if dtype_in == EnergyDType.ivcurve:
                 return self.samples_n * (1 + self.wait_cycles)
-            elif dtype_in == EnergyDType.ivsample:
+            if dtype_in == EnergyDType.ivsample:
                 return 0
             # isc_voc: 2 * (1 + wait_cycles), noqa
             raise ValueError("Not Implemented")
-        else:
-            # only used by ivcurve algo (in ADC-Mode)
-            return self.samples_n
+
+        # only used by ivcurve algo (in ADC-Mode)
+        return self.samples_n
 
 
 u32 = conint(ge=0, lt=2**32)
 
 
 # Currently implemented harvesters
 # NOTE: numbers have meaning and will be tested ->
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_harvester_fixture.yaml` & `shepherd_core-2023.8.1/shepherd_core/data_models/content/virtual_harvester_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_source.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/content/virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/content/virtual_source_fixture.yaml` & `shepherd_core-2023.8.1/shepherd_core/data_models/content/virtual_source_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/doc_virtual_source.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/doc_virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/experiment/observer_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,16 +106,15 @@
             raise ValueError(
                 f"GPIO '{values.get('gpio').name}' in actuation-event not controllable by user"
             )
         return values
 
     def get_events(self) -> np.ndarray:
         stop = self.delay + self.count * self.period
-        timings = np.arange(self.delay, stop, self.period)
-        return timings
+        return np.arange(self.delay, stop, self.period)
 
 
 class GpioActuation(ShpModel, title="Config for GPIO-Actuation"):
     """Configuration for a GPIO-Actuation-Sequence
     TODO: not implemented ATM:
         - decide if pru control sys-gpio or
         - reverses pru-gpio (preferred if possible)
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/experiment/target_config.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/task/emulation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/task/firmware_mod.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/task/harvest.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/task/harvest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/task/observer_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/task/programming.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/task/programming.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/cape.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/cape.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/cape_fixture.yaml` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/cape_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/gpio.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/gpio_fixture.yaml` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/gpio_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/mcu.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/mcu_fixture.yaml` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/mcu_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/observer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/observer_fixture.yaml` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/observer_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/target.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/target.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/target_fixture.yaml` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/target_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2023.8.1/shepherd_core/data_models/testbed/testbed.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/fw_tools/__init__.py` & `shepherd_core-2023.8.1/shepherd_core/fw_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/fw_tools/converter.py` & `shepherd_core-2023.8.1/shepherd_core/fw_tools/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     if not file_hex:
         file_hex = file_elf.resolve().with_suffix(".hex")
     cmd = ["objcopy", "-O", "ihex", file_elf.resolve().as_posix(), file_hex.as_posix()]
     # TODO: observe - maybe $ARCH-Versions of objcopy are needed
     #  (hex of nRF / msp identical between the 3 $arch-versions)
     try:
         ret = subprocess.run(cmd)  # noqa: S603
-    except FileNotFoundError:
+    except FileNotFoundError as err:
         raise RuntimeError(
             "Objcopy not found -> are binutils or build-essential installed?"
-        )
+        ) from err
     if ret.returncode != 0:
         raise RuntimeError("Objcopy failed to convert ELF to iHEX")
     return file_hex
 
 
 @validate_arguments
 def file_to_base64(file_path: Path) -> str:
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/fw_tools/patcher.py` & `shepherd_core-2023.8.1/shepherd_core/fw_tools/patcher.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/fw_tools/validation.py` & `shepherd_core-2023.8.1/shepherd_core/fw_tools/validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,14 +59,20 @@
         if ih.get_memory_size() >= 1310720:
             # conservative test for now - should be well below 1 MB + 256 kB
             return False
         return True
     return False
 
 
+# TODO: elf-workflow needs work -> construct experiments without external dependencies
+#  - remove conversion to hex
+#  - use elftools to verify magic-bytes and similar things done for the hex
+#  https://github.com/eliben/pyelftools/wiki/User's-guide
+
+
 @validate_arguments
 def is_elf(file: Path) -> bool:
     if not os.path.isfile(file):
         return False
     try:
         _ = ELF(path=file)
     except ELFError:
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/logger.py` & `shepherd_core-2023.8.1/shepherd_core/logger.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/reader.py` & `shepherd_core-2023.8.1/shepherd_core/reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/testbed_client/client.py` & `shepherd_core-2023.8.1/shepherd_core/testbed_client/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -70,35 +70,31 @@
         else:
             self._fixtures.insert_model(wrap)
         return True
 
     def query_ids(self, model_type: str) -> list:
         if self._connected:
             raise RuntimeError("Not Implemented, TODO")
-        else:
-            return list(self._fixtures[model_type].elements_by_id.keys())
+        return list(self._fixtures[model_type].elements_by_id.keys())
 
     def query_names(self, model_type: str) -> list:
         if self._connected:
             raise RuntimeError("Not Implemented, TODO")
-        else:
-            return list(self._fixtures[model_type].elements_by_name.keys())
+        return list(self._fixtures[model_type].elements_by_name.keys())
 
     def query_item(
         self, model_type: str, uid: Optional[int] = None, name: Optional[str] = None
     ) -> dict:
         if self._connected:
             raise RuntimeError("Not Implemented, TODO")
-        else:
-            if uid:
-                return self._fixtures[model_type].query_id(uid)
-            if name:
-                return self._fixtures[model_type].query_name(name)
-            else:
-                raise ValueError("Query needs either uid or name of object")
+        if uid:
+            return self._fixtures[model_type].query_id(uid)
+        if name:
+            return self._fixtures[model_type].query_name(name)
+        raise ValueError("Query needs either uid or name of object")
 
     def _query_session_key(self) -> bool:
         if self._server:
             r = requests.get(self._server + "/session_key", timeout=2)
             r.raise_for_status()
             self._key = r.json()["value"]  # TODO: not finished
             return True
@@ -112,16 +108,15 @@
             self._user = User(**r.json())
             return True
         return False
 
     def try_inheritance(self, model_type: str, values: dict) -> (dict, list):
         if self._connected:
             raise RuntimeError("Not Implemented, TODO")
-        else:
-            return self._fixtures[model_type].inheritance(values)
+        return self._fixtures[model_type].inheritance(values)
 
     def try_completing_model(self, model_type: str, values: dict) -> (dict, list):
         """init by name/id, for none existing instances raise Exception"""
         if len(values) == 1 and list(values.keys())[0] in ["id", "name"]:
             value = list(values.values())[0]
             if (
                 isinstance(value, str)
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/testbed_client/fixtures.py` & `shepherd_core-2023.8.1/shepherd_core/testbed_client/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import os
 from pathlib import Path
 from typing import Dict
+from typing import List
 from typing import Optional
 
 import yaml
 
 from ..data_models.base.wrapper import Wrapper
 from ..logger import logger
 
@@ -132,26 +133,24 @@
             # keep previous entries
             base[key] = value
         return base
 
     def query_id(self, _id: int) -> dict:
         if isinstance(_id, int) and _id in self.elements_by_id:
             return self.elements_by_id[_id]
-        else:
-            raise ValueError(
-                f"Initialization of {self.model_type} by ID failed - {_id} is unknown!"
-            )
+        raise ValueError(
+            f"Initialization of {self.model_type} by ID failed - {_id} is unknown!"
+        )
 
     def query_name(self, name: str):
         if isinstance(name, str) and name.lower() in self.elements_by_name:
             return self.elements_by_name[name.lower()]
-        else:
-            raise ValueError(
-                f"Initialization of {self.model_type} by name failed - {name} is unknown!"
-            )
+        raise ValueError(
+            f"Initialization of {self.model_type} by name failed - {name} is unknown!"
+        )
 
 
 class Fixtures:
     suffix = ".yaml"
 
     def __init__(self, file_path: Optional[Path] = None):
         if file_path is None:
@@ -191,31 +190,32 @@
             return self.components[key]
         raise ValueError(f"Component '{key}' not found!")
 
     def keys(self):  # -> _dict_keys[Any, Any]:
         return self.components.keys()
 
     def to_file(self, file: Path):
-        raise RuntimeError("Not Implemented, TODO")
+        raise RuntimeError(f"Not Implemented, TODO (val={file})")
 
 
-def get_files(start_path: Path, suffix: str, recursion_depth: int = 0) -> list:
+def get_files(start_path: Path, suffix: str, recursion_depth: int = 0) -> List[Path]:
     if recursion_depth == 0:
         suffix = suffix.lower().split(".")[-1]
     dir_items = os.scandir(start_path)
     recursion_depth += 1
     files = []
 
     for item in dir_items:
         if item.is_dir():
-            files += get_files(item.path, suffix, recursion_depth)
+            files += get_files(Path(item.path), suffix, recursion_depth)
             continue
-        else:
-            item_name = str(item.name).lower()
-            item_ext = item_name.split(".")[-1]
-            if item_ext == suffix and item_ext != item_name:
-                files.append(item.path)
-            if suffix == "" and item_ext == item_name:
-                files.append(item.path)
+
+        item_name = str(item.name).lower()
+        item_ext = item_name.split(".")[-1]
+        if item_ext == suffix and item_ext != item_name:
+            files.append(Path(item.path))
+        if suffix == "" and item_ext == item_name:
+            files.append(Path(item.path))
+
     if recursion_depth == 1 and len(files) > 0:
         logger.debug(" -> got %s files with the suffix '%s'", len(files), suffix)
     return files
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/testbed_client/user_model.py` & `shepherd_core-2023.8.1/shepherd_core/testbed_client/user_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/vsource/virtual_converter_model.py` & `shepherd_core-2023.8.1/shepherd_core/vsource/virtual_converter_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.cal = cal_emu if cal_emu else CalibrationEmulator()
 
     def conv_adc_raw_to_nA(self, current_raw: int) -> float:
         return self.cal.adc_C_A.raw_to_si(current_raw) * (10**9)
         # TODO: add feature "negative residue compensation" to here
 
     def conv_adc_raw_to_uV(self, voltage_raw: int) -> float:
-        raise RuntimeError("This Fn should not been used")
+        raise RuntimeError(f"This Fn should not been used (val={voltage_raw})")
 
     def conv_uV_to_dac_raw(self, voltage_uV: float) -> int:
         dac_raw = self.cal.dac_V_A.si_to_raw(float(voltage_uV) / (10**6))
         if dac_raw > (2**16) - 1:
             dac_raw = (2**16) - 1
         return dac_raw
 
@@ -111,24 +111,23 @@
             if input_voltage_uV > self.V_mid_uV:
                 input_voltage_uV = self.V_mid_uV
         elif not self.enable_storage:
             # direct connection
             self.V_mid_uV = input_voltage_uV
             input_voltage_uV = 0.0
             # ⤷ input current (& power) is not evaluated
-        else:
-            if input_voltage_uV > self.V_mid_uV:
-                V_diff_uV = input_voltage_uV - self.V_mid_uV
-                V_drop_uV = input_current_nA * self.R_input_kOhm
-                if V_drop_uV > V_diff_uV:
-                    input_voltage_uV = self.V_mid_uV
-                else:
-                    input_voltage_uV -= V_drop_uV
+        elif input_voltage_uV > self.V_mid_uV:
+            V_diff_uV = input_voltage_uV - self.V_mid_uV
+            V_drop_uV = input_current_nA * self.R_input_kOhm
+            if V_drop_uV > V_diff_uV:
+                input_voltage_uV = self.V_mid_uV
             else:
-                input_voltage_uV = 0.0
+                input_voltage_uV -= V_drop_uV
+        else:
+            input_voltage_uV = 0.0
 
         if self.enable_boost:
             eta_inp = self.get_input_efficiency(input_voltage_uV, input_current_nA)
         else:
             eta_inp = 1.0
 
         self.P_inp_fW = eta_inp * input_voltage_uV * input_current_nA
@@ -181,27 +180,25 @@
         check_thresholds = self.sample_count >= self._cfg.interval_check_thresholds_n
 
         if check_thresholds:
             self.sample_count = 0
             if self.is_outputting:
                 if self.V_mid_uV < self.V_disable_output_threshold_uV:
                     self.is_outputting = False
-            else:
-                if self.V_mid_uV >= self.V_enable_output_threshold_uV:
-                    self.is_outputting = True
-                    self.V_mid_uV -= self.dV_enable_output_uV
+            elif self.V_mid_uV >= self.V_enable_output_threshold_uV:
+                self.is_outputting = True
+                self.V_mid_uV -= self.dV_enable_output_uV
 
         if check_thresholds or self._cfg.immediate_pwr_good_signal:
             # generate power-good-signal
             if self.power_good:
                 if self.V_mid_uV <= self._cfg.V_pwr_good_disable_threshold_uV:
                     self.power_good = False
-            else:
-                if self.V_mid_uV >= self._cfg.V_pwr_good_enable_threshold_uV:
-                    self.power_good = self.is_outputting
+            elif self.V_mid_uV >= self._cfg.V_pwr_good_enable_threshold_uV:
+                self.power_good = self.is_outputting
             # set batok pin to state ... TODO?
 
         if self.is_outputting or self.interval_startup_disabled_drain_n > 0:
             if (not self.enable_buck) or (
                 self.V_mid_uV <= self._cfg.V_output_uV + self._cfg.V_buck_drop_uV
             ):
                 if self.V_mid_uV > self._cfg.V_buck_drop_uV:
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/vsource/virtual_harvester_model.py` & `shepherd_core-2023.8.1/shepherd_core/vsource/virtual_harvester_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     HRV_MPPT_OPT: int = 2**14
 
     def __init__(self, cfg: HarvesterPRUConfig):
         self._cfg: HarvesterPRUConfig = cfg
 
         # INIT global vars: shared states
         self.voltage_set_uV: int = self._cfg.voltage_uV + 1
-        # self.settle_steps: int = 0  # adc_ivcurve, noqa: E800
+        # self.settle_steps: int = 0  # adc_ivcurve, noqa: E800, ERA001
         self.interval_step: int = 2**30
 
         self.is_rising: bool = (self._cfg.hrv_mode & (2**1)) != 0
 
         # PO-Relevant, iv & adc
         self.volt_step_uV: int = self._cfg.voltage_step_uV
 
-        # self.power_last_raw: int = 0  # adc_mppt_po, noqa: E800
+        # self.power_last_raw: int = 0  # adc_mppt_po, noqa: E800, ERA001
 
         # globals for iv_cv
         self.voltage_hold: int = 0
         self.current_hold: int = 0
         self.voltage_step_x4_uV: int = self._cfg.voltage_step_uV * 4
 
         # INIT static vars: CV
@@ -139,26 +139,25 @@
             power_now = _voltage_uV * _current_nA
             if power_now > self.power_last:
                 if self.is_rising:
                     self.voltage_set_uV += self.volt_step_uV
                 else:
                     self.voltage_set_uV -= self.volt_step_uV
                 self.volt_step_uV *= 2
+            elif (power_now <= 0) and (self.voltage_set_uV > 0):
+                self.is_rising = True
+                self.volt_step_uV = self._cfg.voltage_step_uV
+                self.voltage_set_uV -= self.voltage_step_x4_uV
             else:
-                if (power_now <= 0) and (self.voltage_set_uV > 0):
-                    self.is_rising = True
-                    self.volt_step_uV = self._cfg.voltage_step_uV
-                    self.voltage_set_uV -= self.voltage_step_x4_uV
+                self.is_rising = not self.is_rising
+                self.volt_step_uV = self._cfg.voltage_step_uV
+                if self.is_rising:
+                    self.voltage_set_uV += self.volt_step_uV
                 else:
-                    self.is_rising = not self.is_rising
-                    self.volt_step_uV = self._cfg.voltage_step_uV
-                    if self.is_rising:
-                        self.voltage_set_uV += self.volt_step_uV
-                    else:
-                        self.voltage_set_uV -= self.volt_step_uV
+                    self.voltage_set_uV -= self.volt_step_uV
 
             self.power_last = power_now
 
             if self.voltage_set_uV >= self._cfg.voltage_max_uV:
                 self.voltage_set_uV = self._cfg.voltage_max_uV
                 self.is_rising = False
                 self.volt_step_uV = self._cfg.voltage_step_uV
```

### Comparing `shepherd_core-2023.6.5/shepherd_core/vsource/virtual_source_model.py` & `shepherd_core-2023.8.1/shepherd_core/vsource/virtual_source_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core/writer.py` & `shepherd_core-2023.8.1/shepherd_core/writer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2023.8.1/shepherd_core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-core
-Version: 2023.6.5
+Version: 2023.8.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: elf
+Provides-Extra: inventory
 Provides-Extra: dev
 Provides-Extra: test
 
 # Shepherd - Core
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
 [![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
@@ -57,16 +58,17 @@
 - read and write shepherds h5-files
 - create, read, write and convert experiments for the testbed (all data-models included)
 - simulate the virtual source, including virtual harvesters
 - connect and query the testbed via a webclient (TestbedClient)
 - work with target-firmwares
   - embed, modify, verify, convert
   - **Note**: working with ELF-files requires external dependencies, see ``Installation``-Chapter
+- decode waveforms -> uart
 
-see [examples](/examples) for more details.
+see [examples](./examples) for more details.
 
 # Installation
 
 The Library is available via PyPI and can be installed with
 
 ```shell
   pip install shepherd-core
@@ -84,7 +86,13 @@
 For more advanced work with ``.elf``-files (modify value of symbols / target-ID) you should install
 
 ```shell
   pip install shepherd-core[elf]
 ```
 
 and also make sure the prereqs for the [pwntools](https://docs.pwntools.com/en/stable/install.html) are met.
+
+For creating an inventory of the host-system you should install
+
+```shell
+  pip install shepherd-core[inventory]
+```
```

### Comparing `shepherd_core-2023.6.5/shepherd_core.egg-info/SOURCES.txt` & `shepherd_core-2023.8.1/shepherd_core.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -44,18 +44,24 @@
 ./shepherd_core/data_models/testbed/mcu_fixture.yaml
 ./shepherd_core/data_models/testbed/observer.py
 ./shepherd_core/data_models/testbed/observer_fixture.yaml
 ./shepherd_core/data_models/testbed/target.py
 ./shepherd_core/data_models/testbed/target_fixture.yaml
 ./shepherd_core/data_models/testbed/testbed.py
 ./shepherd_core/data_models/testbed/testbed_fixture.yaml
+./shepherd_core/decoder_waveform/__init__.py
+./shepherd_core/decoder_waveform/uart.py
 ./shepherd_core/fw_tools/__init__.py
 ./shepherd_core/fw_tools/converter.py
 ./shepherd_core/fw_tools/patcher.py
 ./shepherd_core/fw_tools/validation.py
+./shepherd_core/inventory/__init__.py
+./shepherd_core/inventory/python.py
+./shepherd_core/inventory/system.py
+./shepherd_core/inventory/target.py
 ./shepherd_core/testbed_client/__init__.py
 ./shepherd_core/testbed_client/client.py
 ./shepherd_core/testbed_client/fixtures.py
 ./shepherd_core/testbed_client/user_model.py
 ./shepherd_core/vsource/__init__.py
 ./shepherd_core/vsource/virtual_converter_model.py
 ./shepherd_core/vsource/virtual_harvester_model.py
@@ -85,23 +91,29 @@
 ./tests/data_models/test_content_models.py
 ./tests/data_models/test_examples.py
 ./tests/data_models/test_experiment_models.py
 ./tests/data_models/test_task_generation.py
 ./tests/data_models/test_task_models.py
 ./tests/data_models/test_testbed_fixtures.py
 ./tests/data_models/test_testbed_models.py
+./tests/decoder_waveform/__init__.py
+./tests/decoder_waveform/test_decoder.py
 ./tests/fw_tools/__init__.py
 ./tests/fw_tools/conftest.py
 ./tests/fw_tools/test_converter.py
 ./tests/fw_tools/test_patcher.py
 ./tests/fw_tools/test_validation.py
+./tests/inventory/__init__.py
+./tests/inventory/test_inventory.py
+./tests/testbed_client/__init__.py
 ./tests/vsource/__init__.py
 ./tests/vsource/conftest.py
 ./tests/vsource/test_converter.py
 ./tests/vsource/test_harvester.py
+./tests/vsource/test_z.py
 shepherd_core.egg-info/PKG-INFO
 shepherd_core.egg-info/SOURCES.txt
 shepherd_core.egg-info/dependency_links.txt
 shepherd_core.egg-info/requires.txt
 shepherd_core.egg-info/top_level.txt
 shepherd_core.egg-info/zip-safe
 tests/test_cal_hw.py
```

### Comparing `shepherd_core-2023.6.5/tests/conftest.py` & `shepherd_core-2023.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/example_cal_data.yaml` & `shepherd_core-2023.8.1/tests/data_models/example_cal_data.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/example_cal_data_faulty.yaml` & `shepherd_core-2023.8.1/tests/data_models/example_cal_data_faulty.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/example_cal_meas.yaml` & `shepherd_core-2023.8.1/tests/data_models/example_cal_meas.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/example_cal_meas_faulty1.yaml` & `shepherd_core-2023.8.1/tests/data_models/example_cal_meas_faulty1.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/example_cal_meas_faulty2.yaml` & `shepherd_core-2023.8.1/tests/data_models/example_cal_meas_faulty2.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/example_config_emulator.yaml` & `shepherd_core-2023.8.1/tests/data_models/example_config_emulator.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/example_config_harvester.yaml` & `shepherd_core-2023.8.1/tests/data_models/example_config_harvester.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/example_config_virtsource.yaml` & `shepherd_core-2023.8.1/tests/data_models/example_config_virtsource.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/test_base_models.py` & `shepherd_core-2023.8.1/tests/data_models/test_base_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/test_content_fixtures.py` & `shepherd_core-2023.8.1/tests/data_models/test_content_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/test_examples.py` & `shepherd_core-2023.8.1/tests/data_models/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/test_experiment_models.py` & `shepherd_core-2023.8.1/tests/data_models/test_experiment_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/test_task_generation.py` & `shepherd_core-2023.8.1/tests/data_models/test_task_generation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/test_task_models.py` & `shepherd_core-2023.8.1/tests/data_models/test_task_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/test_testbed_fixtures.py` & `shepherd_core-2023.8.1/tests/data_models/test_testbed_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/data_models/test_testbed_models.py` & `shepherd_core-2023.8.1/tests/data_models/test_testbed_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/fw_tools/test_converter.py` & `shepherd_core-2023.8.1/tests/fw_tools/test_converter.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 import pytest
 
 from shepherd_core import fw_tools
 
 from .conftest import files_elf
 
 
+@pytest.fixture()
+def path_hex(tmp_path: Path) -> Path:
+    path_elf = files_elf[0]
+    path_hex = (tmp_path / (path_elf.stem + ".hex")).resolve()
+    return fw_tools.elf_to_hex(path_elf, path_hex)
+
+
 @pytest.mark.parametrize("path_elf", files_elf)
 def test_elf_to_hex(path_elf: Path, tmp_path: Path) -> None:
     path_hex = (tmp_path / (path_elf.stem + ".hex")).resolve()
     path_gen = fw_tools.elf_to_hex(path_elf, path_hex)
     assert path_hex.exists()
     assert path_hex.as_posix() == path_gen.as_posix()
```

### Comparing `shepherd_core-2023.6.5/tests/fw_tools/test_patcher.py` & `shepherd_core-2023.8.1/tests/fw_tools/test_patcher.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/fw_tools/test_validation.py` & `shepherd_core-2023.8.1/tests/fw_tools/test_validation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/test_cal_hw.py` & `shepherd_core-2023.8.1/tests/test_cal_hw.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/test_examples.py` & `shepherd_core-2023.8.1/tests/test_examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 def example_path() -> Path:
     path = Path(__file__).resolve().parent.parent / "examples"
     os.chdir(path)
     return path
 
 
 examples = [
+    "inventory.py",
     "model_tester.py",
+    "uart_decode_waveform.py",
     "vsource_simulation.py",
     "vharvester_simulation.py",
     "firmware_modification.py",
     "firmware_model.py",
 ]
```

### Comparing `shepherd_core-2023.6.5/tests/test_reader.py` & `shepherd_core-2023.8.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/test_writer.py` & `shepherd_core-2023.8.1/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/vsource/conftest.py` & `shepherd_core-2023.8.1/tests/vsource/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,7 +38,14 @@
 def file_ivsample(file_ivonne: Path) -> Path:
     path = file_ivonne.parent / "jogging_10m_ivsample.h5"
     if not path.exists():
         with ivonne.Reader(file_ivonne) as db:
             tr_opt = mppt.OptimalTracker()
             db.convert_2_ivsamples(path, tracker=tr_opt, duration_s=1)
     return path
+
+
+@pytest.fixture
+def file_cleanup(file_isc_voc: Path, file_ivcurve: Path, file_ivsample: Path) -> None:
+    os.remove(file_isc_voc)
+    os.remove(file_ivcurve)
+    os.remove(file_ivsample)
```

### Comparing `shepherd_core-2023.6.5/tests/vsource/test_converter.py` & `shepherd_core-2023.8.1/tests/vsource/test_converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.5/tests/vsource/test_harvester.py` & `shepherd_core-2023.8.1/tests/vsource/test_harvester.py`

 * *Files identical despite different names*

