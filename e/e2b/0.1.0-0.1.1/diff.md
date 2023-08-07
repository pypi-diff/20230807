# Comparing `tmp/e2b-0.1.0.tar.gz` & `tmp/e2b-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b-0.1.0.tar", max compression
+gzip compressed data, was "e2b-0.1.1.tar", max compression
```

## Comparing `e2b-0.1.0.tar` & `e2b-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     2679 2023-08-06 22:39:31.631750 e2b-0.1.0/README.md
--rw-r--r--   0        0        0      322 2023-08-06 23:47:49.267488 e2b-0.1.0/e2b/__init__.py
--rw-r--r--   0        0        0     1608 2023-08-06 13:23:14.759810 e2b-0.1.0/e2b/api/.openapi-generator/FILES
--rw-r--r--   0        0        0        5 2023-08-06 13:23:14.755109 e2b-0.1.0/e2b/api/.openapi-generator/VERSION
--rw-r--r--   0        0        0     1040 2023-08-05 20:15:21.115495 e2b-0.1.0/e2b/api/.openapi-generator-ignore
--rw-r--r--   0        0        0        0 2023-08-06 13:23:14.743801 e2b-0.1.0/e2b/api/__init__.py
--rw-r--r--   0        0        0     1723 2023-08-06 13:23:14.983213 e2b-0.1.0/e2b/api/client/__init__.py
--rw-r--r--   0        0        0      205 2023-08-06 13:23:14.982169 e2b-0.1.0/e2b/api/client/api/__init__.py
--rw-r--r--   0        0        0     6652 2023-08-06 13:23:15.039880 e2b-0.1.0/e2b/api/client/api/default_api.py
--rw-r--r--   0        0        0    52514 2023-08-06 13:23:15.187017 e2b-0.1.0/e2b/api/client/api/envs_api.py
--rw-r--r--   0        0        0    28662 2023-08-06 13:23:15.120733 e2b-0.1.0/e2b/api/client/api/sessions_api.py
--rw-r--r--   0        0        0    28991 2023-08-06 13:23:15.164691 e2b-0.1.0/e2b/api/client/api_client.py
--rw-r--r--   0        0        0      805 2023-08-06 13:23:15.009027 e2b-0.1.0/e2b/api/client/api_response.py
--rw-r--r--   0        0        0    16423 2023-08-06 13:23:15.106630 e2b-0.1.0/e2b/api/client/configuration.py
--rw-r--r--   0        0        0     1650 2023-08-06 13:23:14.648521 e2b-0.1.0/e2b/api/client/docs/DefaultApi.md
--rw-r--r--   0        0        0    14912 2023-08-06 13:23:14.681786 e2b-0.1.0/e2b/api/client/docs/EnvsApi.md
--rw-r--r--   0        0        0     8210 2023-08-06 13:23:14.701381 e2b-0.1.0/e2b/api/client/docs/SessionsApi.md
--rw-r--r--   0        0        0     5000 2023-08-06 13:23:15.061920 e2b-0.1.0/e2b/api/client/exceptions.py
--rw-r--r--   0        0        0     1021 2023-08-06 13:23:15.032370 e2b-0.1.0/e2b/api/client/models/__init__.py
--rw-r--r--   0        0        0     2232 2023-08-06 13:23:15.043529 e2b-0.1.0/e2b/api/client/models/environment.py
--rw-r--r--   0        0        0      688 2023-08-06 13:23:15.055033 e2b-0.1.0/e2b/api/client/models/environment_state.py
--rw-r--r--   0        0        0     2135 2023-08-06 13:23:15.058779 e2b-0.1.0/e2b/api/client/models/environment_state_update.py
--rw-r--r--   0        0        0     2095 2023-08-06 13:23:15.064434 e2b-0.1.0/e2b/api/client/models/environment_title_update.py
--rw-r--r--   0        0        0     2340 2023-08-06 13:23:15.070187 e2b-0.1.0/e2b/api/client/models/envs_get200_response_inner.py
--rw-r--r--   0        0        0     2049 2023-08-06 13:23:15.084397 e2b-0.1.0/e2b/api/client/models/error.py
--rw-r--r--   0        0        0     2134 2023-08-06 13:23:15.072077 e2b-0.1.0/e2b/api/client/models/new_environment.py
--rw-r--r--   0        0        0     2574 2023-08-06 13:23:15.078473 e2b-0.1.0/e2b/api/client/models/new_session.py
--rw-r--r--   0        0        0     2769 2023-08-06 13:23:15.090178 e2b-0.1.0/e2b/api/client/models/session.py
--rw-r--r--   0        0        0     2949 2023-08-06 13:23:15.091525 e2b-0.1.0/e2b/api/client/models/sessions_get200_response_inner.py
--rw-r--r--   0        0        0      747 2023-08-06 20:29:50.352399 e2b-0.1.0/e2b/api/client/models/template.py
--rw-r--r--   0        0        0     9445 2023-08-06 13:23:15.131742 e2b-0.1.0/e2b/api/client/rest.py
--rw-r--r--   0        0        0        0 2023-08-06 13:23:14.748186 e2b-0.1.0/e2b/api/client/test/__init__.py
--rw-r--r--   0        0        0      725 2023-08-06 13:23:15.087647 e2b-0.1.0/e2b/api/client/test/test_default_api.py
--rw-r--r--   0        0        0     1452 2023-08-06 13:23:15.095204 e2b-0.1.0/e2b/api/client/test/test_environment.py
--rw-r--r--   0        0        0      729 2023-08-06 13:23:15.093499 e2b-0.1.0/e2b/api/client/test/test_environment_state.py
--rw-r--r--   0        0        0     1558 2023-08-06 13:23:15.095048 e2b-0.1.0/e2b/api/client/test/test_environment_state_update.py
--rw-r--r--   0        0        0     1514 2023-08-06 13:23:15.098814 e2b-0.1.0/e2b/api/client/test/test_environment_title_update.py
--rw-r--r--   0        0        0     1381 2023-08-06 13:23:15.104415 e2b-0.1.0/e2b/api/client/test/test_envs_api.py
--rw-r--r--   0        0        0     1611 2023-08-06 13:23:15.098483 e2b-0.1.0/e2b/api/client/test/test_envs_get200_response_inner.py
--rw-r--r--   0        0        0     1384 2023-08-06 13:23:15.101575 e2b-0.1.0/e2b/api/client/test/test_error.py
--rw-r--r--   0        0        0     1470 2023-08-06 13:23:15.107253 e2b-0.1.0/e2b/api/client/test/test_new_environment.py
--rw-r--r--   0        0        0     1445 2023-08-06 13:23:15.104656 e2b-0.1.0/e2b/api/client/test/test_new_session.py
--rw-r--r--   0        0        0     1576 2023-08-06 13:23:15.108483 e2b-0.1.0/e2b/api/client/test/test_session.py
--rw-r--r--   0        0        0     1069 2023-08-06 13:23:15.114978 e2b-0.1.0/e2b/api/client/test/test_sessions_api.py
--rw-r--r--   0        0        0     1831 2023-08-06 13:23:15.113464 e2b-0.1.0/e2b/api/client/test/test_sessions_get200_response_inner.py
--rw-r--r--   0        0        0      672 2023-08-06 13:23:15.110017 e2b-0.1.0/e2b/api/client/test/test_template.py
--rw-r--r--   0        0        0     4174 2023-08-06 13:23:14.722313 e2b-0.1.0/e2b/api/client_README.md
--rw-r--r--   0        0        0      300 2023-08-05 20:23:20.177266 e2b-0.1.0/e2b/api/main.py
--rw-r--r--   0        0        0      142 2023-08-04 16:14:53.404699 e2b-0.1.0/e2b/constants.py
--rw-r--r--   0        0        0      407 2023-08-06 23:47:44.398712 e2b-0.1.0/e2b/session/__init__.py
--rw-r--r--   0        0        0     2997 2023-08-06 22:02:53.757300 e2b-0.1.0/e2b/session/code_snippet.py
--rw-r--r--   0        0        0       50 2023-08-03 14:22:24.009772 e2b-0.1.0/e2b/session/env_vars.py
--rw-r--r--   0        0        0     3513 2023-08-06 23:27:10.913790 e2b-0.1.0/e2b/session/filesystem.py
--rw-r--r--   0        0        0     2130 2023-08-06 22:33:03.077251 e2b-0.1.0/e2b/session/filesystem_watcher.py
--rw-r--r--   0        0        0     4617 2023-08-06 23:58:08.179303 e2b-0.1.0/e2b/session/main.py
--rw-r--r--   0        0        0      404 2023-08-04 11:26:11.925873 e2b-0.1.0/e2b/session/out.py
--rw-r--r--   0        0        0     5941 2023-08-06 23:49:34.070659 e2b-0.1.0/e2b/session/process.py
--rw-r--r--   0        0        0     7933 2023-08-06 23:54:04.427139 e2b-0.1.0/e2b/session/session_connection.py
--rw-r--r--   0        0        0     5171 2023-08-06 23:50:57.268570 e2b-0.1.0/e2b/session/session_daemon.py
--rw-r--r--   0        0        0     5699 2023-08-06 23:55:14.502754 e2b-0.1.0/e2b/session/terminal.py
--rw-r--r--   0        0        0     1109 2023-08-06 23:29:22.554609 e2b-0.1.0/e2b/utils/future.py
--rw-r--r--   0        0        0      166 2023-08-06 09:14:59.416758 e2b-0.1.0/e2b/utils/id.py
--rw-r--r--   0        0        0       34 2023-08-04 08:33:23.591710 e2b-0.1.0/e2b/utils/noop.py
--rw-r--r--   0        0        0      729 2023-08-06 23:06:07.050870 e2b-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 e2b-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2833 2023-08-07 00:01:49.152853 e2b-0.1.1/README.md
+-rw-r--r--   0        0        0      322 2023-08-06 23:47:49.267488 e2b-0.1.1/e2b/__init__.py
+-rw-r--r--   0        0        0     1608 2023-08-06 13:23:14.759810 e2b-0.1.1/e2b/api/.openapi-generator/FILES
+-rw-r--r--   0        0        0        5 2023-08-06 13:23:14.755109 e2b-0.1.1/e2b/api/.openapi-generator/VERSION
+-rw-r--r--   0        0        0     1040 2023-08-05 20:15:21.115495 e2b-0.1.1/e2b/api/.openapi-generator-ignore
+-rw-r--r--   0        0        0        0 2023-08-06 13:23:14.743801 e2b-0.1.1/e2b/api/__init__.py
+-rw-r--r--   0        0        0     1723 2023-08-06 13:23:14.983213 e2b-0.1.1/e2b/api/client/__init__.py
+-rw-r--r--   0        0        0      205 2023-08-06 13:23:14.982169 e2b-0.1.1/e2b/api/client/api/__init__.py
+-rw-r--r--   0        0        0     6652 2023-08-06 13:23:15.039880 e2b-0.1.1/e2b/api/client/api/default_api.py
+-rw-r--r--   0        0        0    52514 2023-08-06 13:23:15.187017 e2b-0.1.1/e2b/api/client/api/envs_api.py
+-rw-r--r--   0        0        0    28662 2023-08-06 13:23:15.120733 e2b-0.1.1/e2b/api/client/api/sessions_api.py
+-rw-r--r--   0        0        0    28991 2023-08-06 13:23:15.164691 e2b-0.1.1/e2b/api/client/api_client.py
+-rw-r--r--   0        0        0      805 2023-08-06 13:23:15.009027 e2b-0.1.1/e2b/api/client/api_response.py
+-rw-r--r--   0        0        0    16423 2023-08-06 13:23:15.106630 e2b-0.1.1/e2b/api/client/configuration.py
+-rw-r--r--   0        0        0     1650 2023-08-06 13:23:14.648521 e2b-0.1.1/e2b/api/client/docs/DefaultApi.md
+-rw-r--r--   0        0        0    14912 2023-08-06 13:23:14.681786 e2b-0.1.1/e2b/api/client/docs/EnvsApi.md
+-rw-r--r--   0        0        0     8210 2023-08-06 13:23:14.701381 e2b-0.1.1/e2b/api/client/docs/SessionsApi.md
+-rw-r--r--   0        0        0     5000 2023-08-06 13:23:15.061920 e2b-0.1.1/e2b/api/client/exceptions.py
+-rw-r--r--   0        0        0     1021 2023-08-06 13:23:15.032370 e2b-0.1.1/e2b/api/client/models/__init__.py
+-rw-r--r--   0        0        0     2232 2023-08-06 13:23:15.043529 e2b-0.1.1/e2b/api/client/models/environment.py
+-rw-r--r--   0        0        0      688 2023-08-06 13:23:15.055033 e2b-0.1.1/e2b/api/client/models/environment_state.py
+-rw-r--r--   0        0        0     2135 2023-08-06 13:23:15.058779 e2b-0.1.1/e2b/api/client/models/environment_state_update.py
+-rw-r--r--   0        0        0     2095 2023-08-06 13:23:15.064434 e2b-0.1.1/e2b/api/client/models/environment_title_update.py
+-rw-r--r--   0        0        0     2340 2023-08-06 13:23:15.070187 e2b-0.1.1/e2b/api/client/models/envs_get200_response_inner.py
+-rw-r--r--   0        0        0     2049 2023-08-06 13:23:15.084397 e2b-0.1.1/e2b/api/client/models/error.py
+-rw-r--r--   0        0        0     2134 2023-08-06 13:23:15.072077 e2b-0.1.1/e2b/api/client/models/new_environment.py
+-rw-r--r--   0        0        0     2574 2023-08-06 13:23:15.078473 e2b-0.1.1/e2b/api/client/models/new_session.py
+-rw-r--r--   0        0        0     2769 2023-08-06 13:23:15.090178 e2b-0.1.1/e2b/api/client/models/session.py
+-rw-r--r--   0        0        0     2949 2023-08-06 13:23:15.091525 e2b-0.1.1/e2b/api/client/models/sessions_get200_response_inner.py
+-rw-r--r--   0        0        0      747 2023-08-06 20:29:50.352399 e2b-0.1.1/e2b/api/client/models/template.py
+-rw-r--r--   0        0        0     9445 2023-08-06 13:23:15.131742 e2b-0.1.1/e2b/api/client/rest.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:23:14.748186 e2b-0.1.1/e2b/api/client/test/__init__.py
+-rw-r--r--   0        0        0      725 2023-08-06 13:23:15.087647 e2b-0.1.1/e2b/api/client/test/test_default_api.py
+-rw-r--r--   0        0        0     1452 2023-08-06 13:23:15.095204 e2b-0.1.1/e2b/api/client/test/test_environment.py
+-rw-r--r--   0        0        0      729 2023-08-06 13:23:15.093499 e2b-0.1.1/e2b/api/client/test/test_environment_state.py
+-rw-r--r--   0        0        0     1558 2023-08-06 13:23:15.095048 e2b-0.1.1/e2b/api/client/test/test_environment_state_update.py
+-rw-r--r--   0        0        0     1514 2023-08-06 13:23:15.098814 e2b-0.1.1/e2b/api/client/test/test_environment_title_update.py
+-rw-r--r--   0        0        0     1381 2023-08-06 13:23:15.104415 e2b-0.1.1/e2b/api/client/test/test_envs_api.py
+-rw-r--r--   0        0        0     1611 2023-08-06 13:23:15.098483 e2b-0.1.1/e2b/api/client/test/test_envs_get200_response_inner.py
+-rw-r--r--   0        0        0     1384 2023-08-06 13:23:15.101575 e2b-0.1.1/e2b/api/client/test/test_error.py
+-rw-r--r--   0        0        0     1470 2023-08-06 13:23:15.107253 e2b-0.1.1/e2b/api/client/test/test_new_environment.py
+-rw-r--r--   0        0        0     1445 2023-08-06 13:23:15.104656 e2b-0.1.1/e2b/api/client/test/test_new_session.py
+-rw-r--r--   0        0        0     1576 2023-08-06 13:23:15.108483 e2b-0.1.1/e2b/api/client/test/test_session.py
+-rw-r--r--   0        0        0     1069 2023-08-06 13:23:15.114978 e2b-0.1.1/e2b/api/client/test/test_sessions_api.py
+-rw-r--r--   0        0        0     1831 2023-08-06 13:23:15.113464 e2b-0.1.1/e2b/api/client/test/test_sessions_get200_response_inner.py
+-rw-r--r--   0        0        0      672 2023-08-06 13:23:15.110017 e2b-0.1.1/e2b/api/client/test/test_template.py
+-rw-r--r--   0        0        0     4174 2023-08-06 13:23:14.722313 e2b-0.1.1/e2b/api/client_README.md
+-rw-r--r--   0        0        0      300 2023-08-05 20:23:20.177266 e2b-0.1.1/e2b/api/main.py
+-rw-r--r--   0        0        0      142 2023-08-04 16:14:53.404699 e2b-0.1.1/e2b/constants.py
+-rw-r--r--   0        0        0      407 2023-08-06 23:47:44.398712 e2b-0.1.1/e2b/session/__init__.py
+-rw-r--r--   0        0        0     2997 2023-08-06 22:02:53.757300 e2b-0.1.1/e2b/session/code_snippet.py
+-rw-r--r--   0        0        0       50 2023-08-03 14:22:24.009772 e2b-0.1.1/e2b/session/env_vars.py
+-rw-r--r--   0        0        0     3513 2023-08-06 23:27:10.913790 e2b-0.1.1/e2b/session/filesystem.py
+-rw-r--r--   0        0        0     2130 2023-08-06 22:33:03.077251 e2b-0.1.1/e2b/session/filesystem_watcher.py
+-rw-r--r--   0        0        0     4617 2023-08-06 23:58:08.179303 e2b-0.1.1/e2b/session/main.py
+-rw-r--r--   0        0        0      404 2023-08-04 11:26:11.925873 e2b-0.1.1/e2b/session/out.py
+-rw-r--r--   0        0        0     5941 2023-08-06 23:49:34.070659 e2b-0.1.1/e2b/session/process.py
+-rw-r--r--   0        0        0     7933 2023-08-06 23:54:04.427139 e2b-0.1.1/e2b/session/session_connection.py
+-rw-r--r--   0        0        0     5171 2023-08-06 23:50:57.268570 e2b-0.1.1/e2b/session/session_daemon.py
+-rw-r--r--   0        0        0     5699 2023-08-06 23:55:14.502754 e2b-0.1.1/e2b/session/terminal.py
+-rw-r--r--   0        0        0     1109 2023-08-06 23:29:22.554609 e2b-0.1.1/e2b/utils/future.py
+-rw-r--r--   0        0        0      166 2023-08-06 09:14:59.416758 e2b-0.1.1/e2b/utils/id.py
+-rw-r--r--   0        0        0       34 2023-08-04 08:33:23.591710 e2b-0.1.1/e2b/utils/noop.py
+-rw-r--r--   0        0        0      731 2023-08-07 00:02:29.395699 e2b-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3799 1970-01-01 00:00:00.000000 e2b-0.1.1/PKG-INFO
```

### Comparing `e2b-0.1.0/README.md` & `e2b-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 ```
 
 ## Usage
 
 ### Initialize new cloud environment session
 ```python
 from e2b import Session
-
+# You can use some of the predefined environments by using specific id:
+# 'Nodejs', 'Bash', 'Python', 'Java', 'Go', 'Rust', 'PHP', 'Perl', 'DotNET'
 session = Session(id="Nodejs", on_scan_ports=lambda ports: print("Open ports", ports))
 
 # Start a session and create a connection to it
 await session.open()
 
 ...
 
@@ -79,15 +80,15 @@
 
 await proc.kill()
 
 # Wait for process to finish
 await proc.finished
 ```
 
-### Create interactive terminal cloud environment
+### Create interactive terminal inside cloud environment
 ```python
 term = await session.terminal.create_session(
     on_data=lambda data: print("Data", data),
     cols=80,
     rows=24,
     rootdir="/code",
     # If you specify a command, the terminal will be closed after the command finishes.
```

### Comparing `e2b-0.1.0/e2b/api/.openapi-generator/FILES` & `e2b-0.1.1/e2b/api/.openapi-generator/FILES`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/.openapi-generator-ignore` & `e2b-0.1.1/e2b/api/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/__init__.py` & `e2b-0.1.1/e2b/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/api/default_api.py` & `e2b-0.1.1/e2b/api/client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/api/envs_api.py` & `e2b-0.1.1/e2b/api/client/api/envs_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/api/sessions_api.py` & `e2b-0.1.1/e2b/api/client/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/api_client.py` & `e2b-0.1.1/e2b/api/client/api_client.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/api_response.py` & `e2b-0.1.1/e2b/api/client/api_response.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/configuration.py` & `e2b-0.1.1/e2b/api/client/configuration.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/docs/DefaultApi.md` & `e2b-0.1.1/e2b/api/client/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/docs/EnvsApi.md` & `e2b-0.1.1/e2b/api/client/docs/EnvsApi.md`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/docs/SessionsApi.md` & `e2b-0.1.1/e2b/api/client/docs/SessionsApi.md`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/exceptions.py` & `e2b-0.1.1/e2b/api/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/__init__.py` & `e2b-0.1.1/e2b/api/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/environment.py` & `e2b-0.1.1/e2b/api/client/models/environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/environment_state.py` & `e2b-0.1.1/e2b/api/client/models/environment_state.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/environment_state_update.py` & `e2b-0.1.1/e2b/api/client/models/environment_state_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/environment_title_update.py` & `e2b-0.1.1/e2b/api/client/models/environment_title_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/envs_get200_response_inner.py` & `e2b-0.1.1/e2b/api/client/models/envs_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/error.py` & `e2b-0.1.1/e2b/api/client/models/error.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/new_environment.py` & `e2b-0.1.1/e2b/api/client/models/new_environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/new_session.py` & `e2b-0.1.1/e2b/api/client/models/new_session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/session.py` & `e2b-0.1.1/e2b/api/client/models/session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/sessions_get200_response_inner.py` & `e2b-0.1.1/e2b/api/client/models/sessions_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/models/template.py` & `e2b-0.1.1/e2b/api/client/models/template.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/rest.py` & `e2b-0.1.1/e2b/api/client/rest.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_default_api.py` & `e2b-0.1.1/e2b/api/client/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_environment.py` & `e2b-0.1.1/e2b/api/client/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_environment_state.py` & `e2b-0.1.1/e2b/api/client/test/test_environment_state.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_environment_state_update.py` & `e2b-0.1.1/e2b/api/client/test/test_environment_state_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_environment_title_update.py` & `e2b-0.1.1/e2b/api/client/test/test_environment_title_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_envs_api.py` & `e2b-0.1.1/e2b/api/client/test/test_envs_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_envs_get200_response_inner.py` & `e2b-0.1.1/e2b/api/client/test/test_envs_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_error.py` & `e2b-0.1.1/e2b/api/client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_new_environment.py` & `e2b-0.1.1/e2b/api/client/test/test_new_environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_new_session.py` & `e2b-0.1.1/e2b/api/client/test/test_new_session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_session.py` & `e2b-0.1.1/e2b/api/client/test/test_session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_sessions_api.py` & `e2b-0.1.1/e2b/api/client/test/test_sessions_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_sessions_get200_response_inner.py` & `e2b-0.1.1/e2b/api/client/test/test_sessions_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client/test/test_template.py` & `e2b-0.1.1/e2b/api/client/test/test_template.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/api/client_README.md` & `e2b-0.1.1/e2b/api/client_README.md`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/session/code_snippet.py` & `e2b-0.1.1/e2b/session/code_snippet.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/session/filesystem.py` & `e2b-0.1.1/e2b/session/filesystem.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/session/filesystem_watcher.py` & `e2b-0.1.1/e2b/session/filesystem_watcher.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/session/main.py` & `e2b-0.1.1/e2b/session/main.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/session/process.py` & `e2b-0.1.1/e2b/session/process.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/session/session_connection.py` & `e2b-0.1.1/e2b/session/session_connection.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/session/session_daemon.py` & `e2b-0.1.1/e2b/session/session_daemon.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/session/terminal.py` & `e2b-0.1.1/e2b/session/terminal.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/e2b/utils/future.py` & `e2b-0.1.1/e2b/utils/future.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.0/PKG-INFO` & `e2b-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: e2b
-Version: 0.1.0
-Summary: SDK for managing e2b environment sessions
+Version: 0.1.1
+Summary: E2B SDK that give agents cloud environments
 Home-page: https://e2b.dev/
 License: MIT
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -45,15 +45,16 @@
 ```
 
 ## Usage
 
 ### Initialize new cloud environment session
 ```python
 from e2b import Session
-
+# You can use some of the predefined environments by using specific id:
+# 'Nodejs', 'Bash', 'Python', 'Java', 'Go', 'Rust', 'PHP', 'Perl', 'DotNET'
 session = Session(id="Nodejs", on_scan_ports=lambda ports: print("Open ports", ports))
 
 # Start a session and create a connection to it
 await session.open()
 
 ...
 
@@ -105,15 +106,15 @@
 
 await proc.kill()
 
 # Wait for process to finish
 await proc.finished
 ```
 
-### Create interactive terminal cloud environment
+### Create interactive terminal inside cloud environment
 ```python
 term = await session.terminal.create_session(
     on_data=lambda data: print("Data", data),
     cols=80,
     rows=24,
     rootdir="/code",
     # If you specify a command, the terminal will be closed after the command finishes.
```

