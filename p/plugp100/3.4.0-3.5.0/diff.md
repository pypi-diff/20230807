# Comparing `tmp/plugp100-3.4.0.tar.gz` & `tmp/plugp100-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugp100-3.4.0.tar", last modified: Mon Jul 31 19:46:32 2023, max compression
+gzip compressed data, was "plugp100-3.5.0.tar", last modified: Mon Aug  7 21:13:01 2023, max compression
```

## Comparing `plugp100-3.4.0.tar` & `plugp100-3.5.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.096267 plugp100-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 19:46:20.000000 plugp100-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 19:46:20.000000 plugp100-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-31 19:46:32.096267 plugp100-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-31 19:46:20.000000 plugp100-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.088266 plugp100-3.4.0/plugp100/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/api/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/hub_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/hub_device_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/s200b_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/t100_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/t110_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/hub/t31x_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/ledstrip_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/light_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/light_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/light_effect_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/plug_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/power_strip_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/api/tapo_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/common/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/functional/either.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/state_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/common/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/discover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/encryption/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/encryption/key_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/encryption/tp_link_cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/handshake_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/requests/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/internal/snowflake_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/login_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/secure_passthrough_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.092266 plugp100-3.4.0/plugp100/requests/set_device_info/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/play_alarm_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/set_light_color_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/set_light_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/set_device_info/set_plug_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/tapo_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/requests/trigger_logs_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.096267 plugp100-3.4.0/plugp100/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/alarm_type_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/child_device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/energy_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.096267 plugp100-3.4.0/plugp100/responses/hub_childs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/s200b_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/t100_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/t110_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/t31x_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/hub_childs/trigger_log_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/power_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/tapo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-31 19:46:20.000000 plugp100-3.4.0/plugp100/responses/tapo_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:32.088266 plugp100-3.4.0/plugp100.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 19:46:32.000000 plugp100-3.4.0/plugp100.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 19:46:20.000000 plugp100-3.4.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-31 19:46:20.000000 plugp100-3.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 19:46:32.096267 plugp100-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-31 19:46:20.000000 plugp100-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.538558 plugp100-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 21:12:52.000000 plugp100-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 21:12:52.000000 plugp100-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-07 21:13:01.538558 plugp100-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-07 21:12:52.000000 plugp100-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.534558 plugp100-3.5.0/plugp100/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.534558 plugp100-3.5.0/plugp100/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/base_tapo_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.534558 plugp100-3.5.0/plugp100/api/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/hub/hub_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/hub/hub_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/hub/s200b_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/hub/t100_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/hub/t110_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/hub/t31x_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/ledstrip_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/light_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/light_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/light_effect_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/plug_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/power_strip_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/api/tapo_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.534558 plugp100-3.5.0/plugp100/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.534558 plugp100-3.5.0/plugp100/common/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/common/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/common/functional/either.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/common/state_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.534558 plugp100-3.5.0/plugp100/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/common/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/common/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/discover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.534558 plugp100-3.5.0/plugp100/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/encryption/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/encryption/key_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/encryption/tp_link_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.538558 plugp100-3.5.0/plugp100/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/handshake_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.538558 plugp100-3.5.0/plugp100/requests/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/internal/snowflake_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/login_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/secure_passthrough_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.538558 plugp100-3.5.0/plugp100/requests/set_device_info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/set_device_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/set_device_info/play_alarm_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/set_device_info/set_light_color_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/set_device_info/set_light_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/set_device_info/set_plug_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/tapo_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/requests/trigger_logs_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.538558 plugp100-3.5.0/plugp100/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/alarm_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/child_device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/device_usage_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/energy_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.538558 plugp100-3.5.0/plugp100/responses/hub_childs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/hub_childs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/hub_childs/s200b_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/hub_childs/t100_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/hub_childs/t110_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/hub_childs/t31x_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/hub_childs/trigger_log_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/power_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/tapo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-07 21:12:52.000000 plugp100-3.5.0/plugp100/responses/tapo_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:13:01.534558 plugp100-3.5.0/plugp100.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-07 21:13:01.000000 plugp100-3.5.0/plugp100.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-07 21:13:01.000000 plugp100-3.5.0/plugp100.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:13:01.000000 plugp100-3.5.0/plugp100.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 21:13:01.000000 plugp100-3.5.0/plugp100.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 21:13:01.000000 plugp100-3.5.0/plugp100.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 21:12:52.000000 plugp100-3.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-07 21:12:52.000000 plugp100-3.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-07 21:13:01.538558 plugp100-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-07 21:12:52.000000 plugp100-3.5.0/setup.py
```

### Comparing `plugp100-3.4.0/LICENSE` & `plugp100-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/PKG-INFO` & `plugp100-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 3.4.0
+Version: 3.5.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-3.4.0/README.md` & `plugp100-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/__init__.py` & `plugp100-3.5.0/plugp100/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         sys.path.append(os.path.join(vendor_dir, vendor_path))
 
 from plugp100.responses import *
 from plugp100.requests import *
 from plugp100.api import *
 from plugp100.common import *
 
-__version__ = "3.4.0"
+__version__ = "3.5.0"
```

### Comparing `plugp100-3.4.0/plugp100/api/hub/hub_device.py` & `plugp100-3.5.0/plugp100/api/hub/hub_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,38 @@
 import asyncio
 import logging
 from asyncio import iscoroutinefunction
 from logging import Logger
 from typing import Callable, Any, List, cast
 
+from plugp100.api.base_tapo_device import _BaseTapoDevice
 from plugp100.api.hub.hub_device_tracker import HubConnectedDeviceTracker, HubDeviceEvent
 from plugp100.api.tapo_client import TapoClient, Json
 from plugp100.common.functional.either import Either, Right, Left
 from plugp100.common.utils.json_utils import dataclass_encode_json
 from plugp100.requests.set_device_info.play_alarm_params import PlayAlarmParams
 from plugp100.requests.tapo_request import TapoRequest
 from plugp100.responses.alarm_type_list import AlarmTypeList
 from plugp100.responses.child_device_list import ChildDeviceList
 from plugp100.responses.device_state import HubDeviceState
 
 HubSubscription = Callable[[], Any]
 
 
 # The HubDevice class is a blueprint for creating hub devices.
-class HubDevice:
+class HubDevice(_BaseTapoDevice):
 
     def __init__(self, api: TapoClient, address: str, logger: Logger = None):
-        self._api = api
-        self._address = address
+        super().__init__(api, address)
         self._tracker = HubConnectedDeviceTracker(logger)
         self._is_tracking = False
         self._tracking_tasks: List[asyncio.Task] = []
         self._tracking_subscriptions: List[Callable[[HubDeviceEvent], Any]] = []
         self._logger = logger if logger is not None else logging.getLogger("HubDevice")
 
-    async def login(self) -> Either[True, Exception]:
-        """
-        The function `login` attempts to log in to an API using a given address and returns either `True` if successful or
-        an `Exception` if there is an error.
-        @return: The login method is returning an Either type, which can either be True or an Exception.
-        """
-        return await self._api.login(self._address)
-
     async def turn_alarm_on(self, alarm: PlayAlarmParams = None) -> Either[True, Exception]:
         request = TapoRequest(method='play_alarm', params=dataclass_encode_json(alarm) if alarm is not None else None)
         return (await self._api.execute_raw_request(request)).map(lambda _: True)
 
     async def turn_alarm_off(self) -> Either[True, Exception]:
         return (await self._api.execute_raw_request(TapoRequest(method='stop_alarm', params=None))).map(lambda _: True)
```

### Comparing `plugp100-3.4.0/plugp100/api/hub/hub_device_tracker.py` & `plugp100-3.5.0/plugp100/api/hub/hub_device_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/api/hub/s200b_device.py` & `plugp100-3.5.0/plugp100/api/hub/s200b_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/api/hub/t100_device.py` & `plugp100-3.5.0/plugp100/api/hub/t100_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/api/hub/t110_device.py` & `plugp100-3.5.0/plugp100/api/hub/t110_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/api/hub/t31x_device.py` & `plugp100-3.5.0/plugp100/api/hub/t31x_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/api/ledstrip_device.py` & `plugp100-3.5.0/plugp100/api/ledstrip_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,21 @@
+from plugp100.api.base_tapo_device import _BaseTapoDevice
 from plugp100.api.light_effect import LightEffect
-from plugp100.api.tapo_client import TapoClient, Json
+from plugp100.api.tapo_client import TapoClient
 from plugp100.common.functional.either import Either
 from plugp100.requests.set_device_info.set_light_color_info_params import LightColorDeviceInfoParams
 from plugp100.requests.set_device_info.set_light_info_params import LightDeviceInfoParams
 from plugp100.requests.set_device_info.set_plug_info_params import SetPlugInfoParams
 from plugp100.responses.device_state import LedStripDeviceState
 
 
-class LedStripDevice:
+class LedStripDevice(_BaseTapoDevice):
 
     def __init__(self, api: TapoClient, address: str):
-        self._api = api
-        self._address = address
-
-    async def login(self) -> Either[True, Exception]:
-        return await self._api.login(self._address)
+        super().__init__(api, address)
 
     async def get_state(self) -> Either[LedStripDeviceState, Exception]:
         return (await self._api.get_device_info()) | LedStripDeviceState.try_from_json
 
     async def on(self) -> Either[True, Exception]:
         return await self._api.set_device_info(SetPlugInfoParams(True))
 
@@ -33,9 +30,12 @@
 
     async def set_color_temperature(self, color_temperature: int) -> Either[True, Exception]:
         return await self._api.set_device_info(LightColorDeviceInfoParams(color_temp=color_temperature))
 
     async def set_light_effect(self, effect: LightEffect) -> Either[True, Exception]:
         return await self._api.set_lighting_effect(effect)
 
-    async def get_state_as_json(self) -> Either[Json, Exception]:
-        return await self._api.get_device_info()
+    async def set_light_effect_brightness(self, effect: LightEffect, brightness: int) -> Either[True, Exception]:
+        effect.brightness=brightness
+        effect.bAdjusted = 1
+        effect.enable = 1
+        return await self._api.set_lighting_effect(effect)
```

### Comparing `plugp100-3.4.0/plugp100/api/light_device.py` & `plugp100-3.5.0/plugp100/api/light_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-from plugp100.api.tapo_client import TapoClient, Json
+from plugp100.api.base_tapo_device import _BaseTapoDevice
+from plugp100.api.tapo_client import TapoClient
+from plugp100.common.functional.either import Either
 from plugp100.requests.set_device_info.set_light_color_info_params import LightColorDeviceInfoParams
 from plugp100.requests.set_device_info.set_light_info_params import LightDeviceInfoParams
-from plugp100.responses.device_state import LightDeviceState
-from plugp100.common.functional.either import Either
 from plugp100.requests.set_device_info.set_plug_info_params import SetPlugInfoParams
+from plugp100.responses.device_state import LightDeviceState
 
 
-class LightDevice:
+class LightDevice(_BaseTapoDevice):
 
     def __init__(self, api: TapoClient, address: str):
-        self._api = api
-        self._address = address
-
-    async def login(self) -> Either[True, Exception]:
-        """
-        The function `login` attempts to log in to an API using the provided address and returns either `True` if successful
-        or an `Exception` if there is an error.
-        @return: The login method is returning an Either type, which can either be True or an Exception.
-        """
-        return await self._api.login(self._address)
+        super().__init__(api, address)
 
     async def get_state(self) -> Either[LightDeviceState, Exception]:
         """
         The function `get_state` asynchronously retrieves the device information from an API and returns either the device
         state or an exception.
         @return: an instance of the `Either` class, which can hold either a `LightDeviceState` object or an `Exception`
         object.
@@ -79,10 +71,7 @@
         @param color_temperature: The `color_temperature` parameter is an integer that represents the desired color
         temperature for a light. Color temperature is typically measured in Kelvin and is used to describe the color
         appearance of a light source. A lower color temperature (e.g., 2700K) produces a warm, yellowish light,
         @type color_temperature: int
         @return: an `Either` object, which can either be `True` or an `Exception`.
         """
         return await self._api.set_device_info(LightColorDeviceInfoParams(color_temp=color_temperature))
-
-    async def get_state_as_json(self) -> Either[Json, Exception]:
-        return await self._api.get_device_info()
```

### Comparing `plugp100-3.4.0/plugp100/api/light_effect.py` & `plugp100-3.5.0/plugp100/api/light_effect.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/api/light_effect_preset.py` & `plugp100-3.5.0/plugp100/api/light_effect_preset.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/api/plug_device.py` & `plugp100-3.5.0/plugp100/api/plug_device.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-from plugp100.api.tapo_client import TapoClient, Json
-from plugp100.responses.device_state import PlugDeviceState
+from plugp100.api.base_tapo_device import _BaseTapoDevice
+from plugp100.api.tapo_client import TapoClient
 from plugp100.common.functional.either import Either
 from plugp100.requests.set_device_info.set_plug_info_params import SetPlugInfoParams
+from plugp100.responses.device_state import PlugDeviceState
 from plugp100.responses.energy_info import EnergyInfo
 from plugp100.responses.power_info import PowerInfo
 
 
-class PlugDevice:
+class PlugDevice(_BaseTapoDevice):
 
     def __init__(self, api: TapoClient, address: str):
-        self._api = api
-        self._address = address
-
-    async def login(self) -> Either[True, Exception]:
-        """
-        The function `login` attempts to log in to an API using a given address and returns either `True` if successful or
-        an `Exception` if there is an error.
-        @return: The login method is returning an Either type, which can either be True or an Exception.
-        """
-        return await self._api.login(self._address)
+        super().__init__(api, address)
 
     async def get_state(self) -> Either[PlugDeviceState, Exception]:
         """
         The function `get_state` asynchronously retrieves device information and returns either the device state or an
         exception.
         @return: an instance of the `Either` class, which can hold either a `PlugDeviceState` object or an `Exception`
         object.
@@ -54,10 +46,7 @@
     async def get_current_power(self) -> Either[PowerInfo, Exception]:
         """
         The function `get_current_power` asynchronously retrieves the current power information using an API and returns
         either the power information or an exception.
         @return: an instance of the `Either` class, which can contain either a `PowerInfo` object or an `Exception` object.
         """
         return await self._api.get_current_power()
-
-    async def get_state_as_json(self) -> Either[Json, Exception]:
-        return await self._api.get_device_info()
```

### Comparing `plugp100-3.4.0/plugp100/api/power_strip_device.py` & `plugp100-3.5.0/plugp100/api/power_strip_device.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,21 @@
+from plugp100.api.base_tapo_device import _BaseTapoDevice
 from plugp100.api.tapo_client import TapoClient, Json
 from plugp100.common.functional.either import Either
 from plugp100.common.utils.json_utils import dataclass_encode_json
 from plugp100.requests.set_device_info.set_plug_info_params import SetPlugInfoParams
 from plugp100.requests.tapo_request import TapoRequest
 from plugp100.responses.child_device_list import ChildDeviceList
 from plugp100.responses.device_state import PlugDeviceState
 
 
-class PowerStripDevice:
+class PowerStripDevice(_BaseTapoDevice):
 
     def __init__(self, api: TapoClient, address: str):
-        self._api = api
-        self._address = address
-
-    async def login(self) -> Either[True, Exception]:
-        """
-        The function `login` attempts to log in to an API using a given address and returns either `True` if successful or
-        an `Exception` if there is an error.
-        @return: The login method is returning an Either type, which can either be True or an Exception.
-        """
-        return await self._api.login(self._address)
+        super().__init__(api, address)
 
     async def get_state(self) -> Either[PlugDeviceState, Exception]:
         """
         The function `get_state` asynchronously retrieves device information and returns either the device state or an
         exception.
         @return: an instance of the `Either` class, which can hold either a `PlugDeviceState` object or an `Exception`
         object.
@@ -39,10 +31,7 @@
 
     async def off(self, child_device_id: str) -> Either[True, Exception]:
         request = TapoRequest.set_device_info(dataclass_encode_json(SetPlugInfoParams(device_on=False)))
         return (await self._control_child(child_device_id, request)).map(lambda _: True)
 
     async def _control_child(self, device_id: str, request: TapoRequest) -> Either[Json, Exception]:
         return await self._api.control_child(device_id, request)
-
-    async def get_state_as_json(self) -> Either[Json, Exception]:
-        return await self._api.get_device_info()
```

### Comparing `plugp100-3.4.0/plugp100/api/tapo_client.py` & `plugp100-3.5.0/plugp100/api/tapo_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from plugp100.api.light_effect import LightEffect
 from plugp100.common.functional.either import Either, Right, Left
 from plugp100.common.utils.http_client import AsyncHttp
 from plugp100.common.utils.json_utils import dataclass_encode_json, Json
 from plugp100.requests.handshake_params import HandshakeParams
 from plugp100.requests.internal.snowflake_id import SnowflakeId
-from plugp100.requests.login_device import LoginDeviceParams
+from plugp100.requests.login_device import LoginDeviceParams, LoginDeviceParamsV2
 from plugp100.requests.secure_passthrough_params import SecurePassthroughParams
 from plugp100.requests.tapo_request import TapoRequest, MultipleRequestParams
 from plugp100.responses.child_device_list import ChildDeviceList
 from plugp100.responses.energy_info import EnergyInfo
 from plugp100.responses.power_info import PowerInfo
 from plugp100.responses.tapo_response import TapoResponse
 from plugp100.encryption.key_pair import KeyPair
@@ -49,27 +49,29 @@
         self._http = AsyncHttp(aiohttp.ClientSession() if http_session is None else http_session)
         self._session = None
         self._request_id_generator = SnowflakeId(1, 1)
 
     async def close(self):
         await self._http.close()
 
-    async def login(self, url: str) -> Either[True, Exception]:
+    async def login(self, url: str, use_v2: bool = False) -> Either[True, Exception]:
         """
         The `login` function performs a handshake with a given URL, and if successful, sends a login request with a username
         and password, returning a token if successful or an exception if not.
 
         @param url: The `url` parameter is a string that represents the URL of the login endpoint
         @type url: str
+        @param use_v2: If should login by using v2 api
+        @type use_v2: bool
         @return: The login function returns an Either type, which can either be a Right containing True if the login is
         successful, or a Right containing an Exception if there is an error during the login process.
         """
         handshake = await self._handshake(url)
         if isinstance(handshake, Right):
-            token_or_error = await self._login_request(self._username, self._password)
+            token_or_error = await self._login_request(self._username, self._password, use_v2)
             self._session.token = token_or_error.value if isinstance(token_or_error, Right) else None
             return token_or_error.map(lambda _: True)
 
         return handshake
 
     async def execute_raw_request(self, request: 'TapoRequest') -> Either[Json, Exception]:
         request.with_terminal_uuid(self._session.terminal_uuid).with_request_time_millis(round(time() * 1000))
@@ -189,16 +191,17 @@
                     return Right(responses[0]['result'])
                 else:
                     return Left(Exception("Empty responses from child"))
             except Exception as e:
                 return Left(e)
         return cast(Left, response)
 
-    async def _login_request(self, username: str, password: str) -> Either[str, Exception]:
-        login_device_params = LoginDeviceParams(username, password)
+    async def _login_request(self, username: str, password: str, v2: bool = False) -> Either[str, Exception]:
+        login_device_params = LoginDeviceParams(username, password) if v2 is False else LoginDeviceParamsV2(username,
+                                                                                                            password)
         login_request = TapoRequest.login(login_device_params) \
             .with_request_time_millis(round(time() * 1000))
         response_as_dict = await self._execute_with_passthrough(login_request)
         return response_as_dict.map(lambda x: x.result['token'])
 
     async def _handshake(self, url: str) -> Either[True, Exception]:
         logger.debug("Will perform handshaking...")
@@ -224,25 +227,27 @@
             cookie_token = response.cookies.get('TP_SESSIONID').value
             logger.debug(f"Got TP_SESSIONID token: ...{cookie_token[5:]}")
 
             logger.debug("Decoding handshake key...")
             handshake_key = resp_dict['result']['key']
             tp_link_cipher = TpLinkCipherCryptography.create_from_keypair(handshake_key, key_pair)
 
-            self._session = Session(url, key_pair, tp_link_cipher, cookie_token, token=None, terminal_uuid=str(uuid.uuid4()))
+            self._session = Session(url, key_pair, tp_link_cipher, cookie_token, token=None,
+                                    terminal_uuid=str(uuid.uuid4()))
             return Right(True)
         else:
             return response_or_error
 
     async def _execute_with_passthrough(
             self,
             request: TapoRequest,
             require_token: bool = False
     ) -> Either[TapoResponse[Json], Exception]:
-        request.with_request_id(self._request_id_generator.generate_id()).with_terminal_uuid(self._session.terminal_uuid)
+        request.with_request_id(self._request_id_generator.generate_id()).with_terminal_uuid(
+            self._session.terminal_uuid)
         encrypted_request = self._session.chiper.encrypt(jsons.dumps(request))
         passthrough_request = TapoRequest.secure_passthrough(SecurePassthroughParams(encrypted_request))
         request_body = jsons.loads(jsons.dumps(passthrough_request))
 
         logger.debug(f"Request body: {request_body}")
 
         response_encrypted = await self._http.async_make_post_cookie(
```

### Comparing `plugp100-3.4.0/plugp100/common/functional/either.py` & `plugp100-3.5.0/plugp100/common/functional/either.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/common/state_tracker.py` & `plugp100-3.5.0/plugp100/common/state_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/common/utils/http_client.py` & `plugp100-3.5.0/plugp100/common/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/encryption/key_pair.py` & `plugp100-3.5.0/plugp100/encryption/key_pair.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/encryption/tp_link_cipher.py` & `plugp100-3.5.0/plugp100/encryption/tp_link_cipher.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/example.py` & `plugp100-3.5.0/plugp100/example.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/requests/internal/snowflake_id.py` & `plugp100-3.5.0/plugp100/requests/internal/snowflake_id.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/requests/tapo_request.py` & `plugp100-3.5.0/plugp100/requests/tapo_request.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/alarm_type_list.py` & `plugp100-3.5.0/plugp100/responses/alarm_type_list.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/child_device_list.py` & `plugp100-3.5.0/plugp100/responses/child_device_list.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/device_state.py` & `plugp100-3.5.0/plugp100/responses/device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/energy_info.py` & `plugp100-3.5.0/plugp100/responses/energy_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/hub_childs/s200b_device_state.py` & `plugp100-3.5.0/plugp100/responses/hub_childs/s200b_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/hub_childs/t100_device_state.py` & `plugp100-3.5.0/plugp100/responses/hub_childs/t100_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/hub_childs/t110_device_state.py` & `plugp100-3.5.0/plugp100/responses/hub_childs/t110_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/hub_childs/t31x_device_state.py` & `plugp100-3.5.0/plugp100/responses/hub_childs/t31x_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/hub_childs/trigger_log_response.py` & `plugp100-3.5.0/plugp100/responses/hub_childs/trigger_log_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/tapo_exception.py` & `plugp100-3.5.0/plugp100/responses/tapo_exception.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100/responses/tapo_response.py` & `plugp100-3.5.0/plugp100/responses/tapo_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.4.0/plugp100.egg-info/PKG-INFO` & `plugp100-3.5.0/plugp100.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 3.4.0
+Version: 3.5.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-3.4.0/plugp100.egg-info/SOURCES.txt` & `plugp100-3.5.0/plugp100.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 plugp100/example.py
 plugp100.egg-info/PKG-INFO
 plugp100.egg-info/SOURCES.txt
 plugp100.egg-info/dependency_links.txt
 plugp100.egg-info/requires.txt
 plugp100.egg-info/top_level.txt
 plugp100/api/__init__.py
+plugp100/api/base_tapo_device.py
 plugp100/api/ledstrip_device.py
 plugp100/api/light_device.py
 plugp100/api/light_effect.py
 plugp100/api/light_effect_preset.py
 plugp100/api/plug_device.py
 plugp100/api/power_strip_device.py
 plugp100/api/tapo_client.py
@@ -52,14 +53,15 @@
 plugp100/requests/set_device_info/set_light_color_info_params.py
 plugp100/requests/set_device_info/set_light_info_params.py
 plugp100/requests/set_device_info/set_plug_info_params.py
 plugp100/responses/__init__.py
 plugp100/responses/alarm_type_list.py
 plugp100/responses/child_device_list.py
 plugp100/responses/device_state.py
+plugp100/responses/device_usage_info.py
 plugp100/responses/energy_info.py
 plugp100/responses/power_info.py
 plugp100/responses/tapo_exception.py
 plugp100/responses/tapo_response.py
 plugp100/responses/hub_childs/__init__.py
 plugp100/responses/hub_childs/s200b_device_state.py
 plugp100/responses/hub_childs/t100_device_state.py
```

### Comparing `plugp100-3.4.0/setup.py` & `plugp100-3.5.0/setup.py`

 * *Files identical despite different names*

