# Comparing `tmp/fern_seam-0.0.8.tar.gz` & `tmp/fern_seam-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_seam-0.0.8.tar", max compression
+gzip compressed data, was "fern_seam-0.0.9.tar", max compression
```

## Comparing `fern_seam-0.0.8.tar` & `fern_seam-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1630 2023-05-16 05:15:57.411589 fern_seam-0.0.8/README.md
--rw-r--r--   0        0        0      368 2023-05-16 05:15:57.411589 fern_seam-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      913 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/__init__.py
--rw-r--r--   0        0        0     1056 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/base_client.py
--rw-r--r--   0        0        0     3453 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/client.py
--rw-r--r--   0        0        0      348 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      160 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/environment.py
--rw-r--r--   0        0        0        0 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/py.typed
--rw-r--r--   0        0        0      889 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/__init__.py
--rw-r--r--   0        0        0      437 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/__init__.py
--rw-r--r--   0        0        0     9385 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/client.py
--rw-r--r--   0        0        0      610 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/types/__init__.py
--rw-r--r--   0        0        0     1871 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/types/access_code.py
--rw-r--r--   0        0        0      782 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/types/access_code_error.py
--rw-r--r--   0        0        0      103 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/types/access_code_id.py
--rw-r--r--   0        0        0     1002 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/types/access_code_status.py
--rw-r--r--   0        0        0      784 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/types/access_code_warning.py
--rw-r--r--   0        0        0      910 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/types/create_access_code_response.py
--rw-r--r--   0        0        0      846 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/access_codes/types/update_access_code_response.py
--rw-r--r--   0        0        0      219 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/action_attempts/__init__.py
--rw-r--r--   0        0        0     2718 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/action_attempts/client.py
--rw-r--r--   0        0        0      308 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/action_attempts/types/__init__.py
--rw-r--r--   0        0        0      995 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/action_attempts/types/action_attempt.py
--rw-r--r--   0        0        0      106 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/action_attempts/types/action_attempt_id.py
--rw-r--r--   0        0        0      633 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/action_attempts/types/action_status.py
--rw-r--r--   0        0        0     1150 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/action_attempts/types/action_type.py
--rw-r--r--   0        0        0      164 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/commons/__init__.py
--rw-r--r--   0        0        0      203 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      250 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/commons/errors/bad_request_error.py
--rw-r--r--   0        0        0      248 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/commons/errors/not_found_error.py
--rw-r--r--   0        0        0      117 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/devices/__init__.py
--rw-r--r--   0        0        0      121 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/devices/types/__init__.py
--rw-r--r--   0        0        0       99 2023-05-16 05:15:57.411589 fern_seam-0.0.8/src/seam/resources/devices/types/device_id.py
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 fern_seam-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1630 2023-05-16 05:45:16.170194 fern_seam-0.0.9/README.md
+-rw-r--r--   0        0        0      368 2023-05-16 05:45:16.170194 fern_seam-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      913 2023-05-16 05:45:16.170194 fern_seam-0.0.9/src/seam/__init__.py
+-rw-r--r--   0        0        0     1056 2023-05-16 05:45:16.170194 fern_seam-0.0.9/src/seam/base_client.py
+-rw-r--r--   0        0        0     3350 2023-05-16 05:45:16.170194 fern_seam-0.0.9/src/seam/client.py
+-rw-r--r--   0        0        0      348 2023-05-16 05:45:16.170194 fern_seam-0.0.9/src/seam/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-16 05:45:16.170194 fern_seam-0.0.9/src/seam/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-16 05:45:16.170194 fern_seam-0.0.9/src/seam/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-16 05:45:16.170194 fern_seam-0.0.9/src/seam/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      160 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/environment.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/py.typed
+-rw-r--r--   0        0        0      889 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/__init__.py
+-rw-r--r--   0        0        0      437 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/__init__.py
+-rw-r--r--   0        0        0     9385 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/client.py
+-rw-r--r--   0        0        0      610 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/types/__init__.py
+-rw-r--r--   0        0        0     1871 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/types/access_code.py
+-rw-r--r--   0        0        0      782 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/types/access_code_error.py
+-rw-r--r--   0        0        0      103 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/types/access_code_id.py
+-rw-r--r--   0        0        0     1002 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/types/access_code_status.py
+-rw-r--r--   0        0        0      784 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/types/access_code_warning.py
+-rw-r--r--   0        0        0      910 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/types/create_access_code_response.py
+-rw-r--r--   0        0        0      846 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/access_codes/types/update_access_code_response.py
+-rw-r--r--   0        0        0      219 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/action_attempts/__init__.py
+-rw-r--r--   0        0        0     2718 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/action_attempts/client.py
+-rw-r--r--   0        0        0      308 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/action_attempts/types/__init__.py
+-rw-r--r--   0        0        0      995 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/action_attempts/types/action_attempt.py
+-rw-r--r--   0        0        0      106 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/action_attempts/types/action_attempt_id.py
+-rw-r--r--   0        0        0      633 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/action_attempts/types/action_status.py
+-rw-r--r--   0        0        0     1150 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/action_attempts/types/action_type.py
+-rw-r--r--   0        0        0      164 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/commons/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      250 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      248 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0      117 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/devices/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/devices/types/__init__.py
+-rw-r--r--   0        0        0       99 2023-05-16 05:45:16.174193 fern_seam-0.0.9/src/seam/resources/devices/types/device_id.py
+-rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 fern_seam-0.0.9/PKG-INFO
```

### Comparing `fern_seam-0.0.8/README.md` & `fern_seam-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/__init__.py` & `fern_seam-0.0.9/src/seam/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/base_client.py` & `fern_seam-0.0.9/src/seam/base_client.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/client.py` & `fern_seam-0.0.9/src/seam/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import typing
 import datetime as dt
 import time
 
 from .base_client import Seam as BaseClient
 from .environment import SeamEnvironment
 from .resources.access_codes.client import AccessCodesClient
-from .resources.action_attempts.client import ActionAttemptsClient
-from . import UpdateAccessCodeResponse, ActionAttemptId, ActionAttempt, AccessCode
+from . import ActionAttemptId, ActionAttempt, AccessCode
 
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class Seam(BaseClient):
+class Seam:
     def __init__(self, *, environment: SeamEnvironment = SeamEnvironment.PRODUCTION, token: str):
-        super().__init__(environment=environment, token=token)
+        self._client = BaseClient(environment=environment, token=token)
+        self.action_attempts = self._client.action_attempts
         self.access_codes = AccessCodes(
-            environment=self._environment,
-            token=self._token,
-            action_attempts_client=self.action_attempts,
+            environment=environment,
+            token=token,
+            base_client=self._client,
         )
 
 
 class AccessCodes(AccessCodesClient):
-    def __init__(self, *, environment: SeamEnvironment, token: str, action_attempts_client: ActionAttemptsClient):
+    def __init__(self, *, environment: SeamEnvironment, token: str, base_client: BaseClient):
         super().__init__(environment=environment, token=token)
-        self._action_attempts_client = action_attempts_client
+        self._base_client = base_client
 
-    def update_and_wait_until_ready(  # type: ignore
+    def update(  # type: ignore
         self,
         *,
         access_code_id: str,
         name: typing.Optional[str] = OMIT,
         code: typing.Optional[str] = OMIT,
         starts_at: typing.Optional[dt.datetime] = OMIT,
         ends_at: typing.Optional[dt.datetime] = OMIT,
     ) -> AccessCode:
-        res = super().update(
+        res = self._base_client.access_codes.update(
             access_code_id=access_code_id,
             name=name,
             code=code,
             starts_at=starts_at,
             ends_at=ends_at
         )
 
@@ -53,15 +53,15 @@
 
     def _poll_until_ready(self, action_attempt: ActionAttemptId) -> ActionAttempt:
         updated_action_attempt: typing.Optional[ActionAttempt] = None
         while (
             updated_action_attempt is None
             or updated_action_attempt.status == "pending"
         ):
-            updated_action_attempt = self._action_attempts_client.get(action_attempt_id=action_attempt)
+            updated_action_attempt = self._base_client.action_attempts.get(action_attempt_id=action_attempt)
             time.sleep(0.25)
 
         if updated_action_attempt.status == "error":
             error_type = None
             error_message = None
             if updated_action_attempt.error is not None:
                 error_type = updated_action_attempt.error.type
```

### Comparing `fern_seam-0.0.8/src/seam/core/datetime_utils.py` & `fern_seam-0.0.9/src/seam/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/core/jsonable_encoder.py` & `fern_seam-0.0.9/src/seam/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/__init__.py` & `fern_seam-0.0.9/src/seam/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/access_codes/client.py` & `fern_seam-0.0.9/src/seam/resources/access_codes/client.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/access_codes/types/__init__.py` & `fern_seam-0.0.9/src/seam/resources/access_codes/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/access_codes/types/access_code.py` & `fern_seam-0.0.9/src/seam/resources/access_codes/types/access_code.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/access_codes/types/access_code_error.py` & `fern_seam-0.0.9/src/seam/resources/access_codes/types/access_code_error.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/access_codes/types/access_code_status.py` & `fern_seam-0.0.9/src/seam/resources/access_codes/types/access_code_status.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/access_codes/types/access_code_warning.py` & `fern_seam-0.0.9/src/seam/resources/access_codes/types/access_code_warning.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/access_codes/types/create_access_code_response.py` & `fern_seam-0.0.9/src/seam/resources/access_codes/types/create_access_code_response.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/access_codes/types/update_access_code_response.py` & `fern_seam-0.0.9/src/seam/resources/access_codes/types/update_access_code_response.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/action_attempts/client.py` & `fern_seam-0.0.9/src/seam/resources/action_attempts/client.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/action_attempts/types/action_attempt.py` & `fern_seam-0.0.9/src/seam/resources/action_attempts/types/action_attempt.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/action_attempts/types/action_status.py` & `fern_seam-0.0.9/src/seam/resources/action_attempts/types/action_status.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/src/seam/resources/action_attempts/types/action_type.py` & `fern_seam-0.0.9/src/seam/resources/action_attempts/types/action_type.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.8/PKG-INFO` & `fern_seam-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-seam
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

