# Comparing `tmp/upkie-1.3.1.tar.gz` & `tmp/upkie-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upkie-1.3.1.tar", last modified: Fri Jul 28 17:56:55 2023, max compression
+gzip compressed data, was "upkie-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `upkie-1.3.1.tar` & `upkie-1.3.2.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0     8557 2023-07-28 17:56:55.319436 upkie-1.3.1/README.md
--rw-r--r--   0        0        0     1942 2023-07-28 17:56:55.315436 upkie-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      695 2023-07-28 17:56:55.315436 upkie-1.3.1/upkie/__init__.py
--rw-r--r--   0        0        0     1079 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/BUILD
--rw-r--r--   0        0        0     1275 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/__init__.py
--rw-r--r--   0        0        0     2809 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/standing_reward.py
--rw-r--r--   0        0        0      549 2023-07-28 17:56:55.291436 upkie-1.3.1/upkie/envs/tests/BUILD
--rw-r--r--   0        0        0     2555 2023-07-28 17:56:55.291436 upkie-1.3.1/upkie/envs/tests/upkie_base_env_test.py
--rw-r--r--   0        0        0     2465 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/tests/upkie_servos_env_test.py
--rw-r--r--   0        0        0     2349 2023-07-28 17:56:55.291436 upkie-1.3.1/upkie/envs/tests/upkie_wheels_env_test.py
--rw-r--r--   0        0        0     9575 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/upkie_base_env.py
--rw-r--r--   0        0        0     7657 2023-07-28 17:56:55.291436 upkie-1.3.1/upkie/envs/upkie_servos_env.py
--rw-r--r--   0        0        0     7387 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/upkie_wheels_env.py
--rw-r--r--   0        0        0      356 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/BUILD
--rw-r--r--   0        0        0      902 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/__init__.py
--rw-r--r--   0        0        0     5612 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/base_pitch.py
--rw-r--r--   0        0        0      305 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/tests/BUILD
--rw-r--r--   0        0        0     3105 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/tests/base_pitch_test.py
--rw-r--r--   0        0        0     1201 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/BUILD
--rw-r--r--   0        0        0     1896 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/clamp.py
--rw-r--r--   0        0        0     1137 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/datetime_now_string.h
--rw-r--r--   0        0        0      803 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/exceptions.py
--rw-r--r--   0        0        0     2815 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/filters.py
--rw-r--r--   0        0        0     2433 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/pinocchio.py
--rw-r--r--   0        0        0     1430 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/raspi.py
--rw-r--r--   0        0        0     1900 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/rotations.py
--rw-r--r--   0        0        0     1983 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/spdlog.py
--rw-r--r--   0        0        0      634 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/tests/BUILD
--rw-r--r--   0        0        0     1303 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/tests/clamp_test.py
--rw-r--r--   0        0        0      986 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/tests/datetime_now_string_test.cpp
--rw-r--r--   0        0        0     2232 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/tests/pinocchio_test.py
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 upkie-1.3.1/setup.py
--rw-r--r--   0        0        0     9991 1970-01-01 00:00:00.000000 upkie-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     8557 2023-08-07 09:20:22.235779 upkie-1.3.2/README.md
+-rw-r--r--   0        0        0     1942 2023-08-07 09:20:22.231779 upkie-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/__init__.py
+-rw-r--r--   0        0        0      332 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/config/BUILD
+-rw-r--r--   0        0        0      796 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/config/__init__.py
+-rw-r--r--   0        0        0      478 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/config/spine.yaml
+-rw-r--r--   0        0        0     1079 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/BUILD
+-rw-r--r--   0        0        0     1275 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/__init__.py
+-rw-r--r--   0        0        0     2809 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/standing_reward.py
+-rw-r--r--   0        0        0      549 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/tests/BUILD
+-rw-r--r--   0        0        0     2555 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/tests/upkie_base_env_test.py
+-rw-r--r--   0        0        0     2465 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/tests/upkie_servos_env_test.py
+-rw-r--r--   0        0        0     2349 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/tests/upkie_wheels_env_test.py
+-rw-r--r--   0        0        0     9575 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/upkie_base_env.py
+-rw-r--r--   0        0        0     7657 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/upkie_servos_env.py
+-rw-r--r--   0        0        0     7387 2023-08-07 09:20:22.227779 upkie-1.3.2/upkie/envs/upkie_wheels_env.py
+-rw-r--r--   0        0        0      356 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/observers/base_pitch/BUILD
+-rw-r--r--   0        0        0      902 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/observers/base_pitch/__init__.py
+-rw-r--r--   0        0        0     5612 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/observers/base_pitch/base_pitch.py
+-rw-r--r--   0        0        0      305 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/observers/base_pitch/tests/BUILD
+-rw-r--r--   0        0        0     3105 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/observers/base_pitch/tests/base_pitch_test.py
+-rw-r--r--   0        0        0     1201 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/BUILD
+-rw-r--r--   0        0        0     1896 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/clamp.py
+-rw-r--r--   0        0        0     1137 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/datetime_now_string.h
+-rw-r--r--   0        0        0      803 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/exceptions.py
+-rw-r--r--   0        0        0     2815 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/filters.py
+-rw-r--r--   0        0        0     2433 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/pinocchio.py
+-rw-r--r--   0        0        0     1430 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/raspi.py
+-rw-r--r--   0        0        0     1900 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/rotations.py
+-rw-r--r--   0        0        0     1983 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/spdlog.py
+-rw-r--r--   0        0        0      634 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/tests/BUILD
+-rw-r--r--   0        0        0     1303 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/tests/clamp_test.py
+-rw-r--r--   0        0        0      986 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/tests/datetime_now_string_test.cpp
+-rw-r--r--   0        0        0     2232 2023-08-07 09:20:22.231779 upkie-1.3.2/upkie/utils/tests/pinocchio_test.py
+-rw-r--r--   0        0        0     9991 1970-01-01 00:00:00.000000 upkie-1.3.2/PKG-INFO
```

### Comparing `upkie-1.3.1/README.md` & `upkie-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/pyproject.toml` & `upkie-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/__init__.py` & `upkie-1.3.2/upkie/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python module to control Upkie wheeled bipeds."""
 
-__version__ = "1.3.1"
+__version__ = "1.3.2"
```

### Comparing `upkie-1.3.1/upkie/envs/BUILD` & `upkie-1.3.2/upkie/envs/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/envs/__init__.py` & `upkie-1.3.2/upkie/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/envs/standing_reward.py` & `upkie-1.3.2/upkie/envs/standing_reward.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/envs/tests/BUILD` & `upkie-1.3.2/upkie/envs/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/envs/tests/upkie_base_env_test.py` & `upkie-1.3.2/upkie/envs/tests/upkie_base_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/envs/tests/upkie_servos_env_test.py` & `upkie-1.3.2/upkie/envs/tests/upkie_servos_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/envs/tests/upkie_wheels_env_test.py` & `upkie-1.3.2/upkie/envs/tests/upkie_wheels_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/envs/upkie_base_env.py` & `upkie-1.3.2/upkie/envs/upkie_base_env.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/envs/upkie_servos_env.py` & `upkie-1.3.2/upkie/envs/upkie_servos_env.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/envs/upkie_wheels_env.py` & `upkie-1.3.2/upkie/envs/upkie_wheels_env.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/observers/base_pitch/__init__.py` & `upkie-1.3.2/upkie/observers/base_pitch/__init__.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/observers/base_pitch/base_pitch.py` & `upkie-1.3.2/upkie/observers/base_pitch/base_pitch.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/observers/base_pitch/tests/base_pitch_test.py` & `upkie-1.3.2/upkie/observers/base_pitch/tests/base_pitch_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/BUILD` & `upkie-1.3.2/upkie/utils/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/clamp.py` & `upkie-1.3.2/upkie/utils/clamp.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/datetime_now_string.h` & `upkie-1.3.2/upkie/utils/datetime_now_string.h`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/exceptions.py` & `upkie-1.3.2/upkie/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/filters.py` & `upkie-1.3.2/upkie/utils/filters.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/pinocchio.py` & `upkie-1.3.2/upkie/utils/pinocchio.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/raspi.py` & `upkie-1.3.2/upkie/utils/raspi.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/rotations.py` & `upkie-1.3.2/upkie/utils/rotations.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/spdlog.py` & `upkie-1.3.2/upkie/utils/spdlog.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/tests/BUILD` & `upkie-1.3.2/upkie/utils/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/tests/clamp_test.py` & `upkie-1.3.2/upkie/utils/tests/clamp_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/tests/datetime_now_string_test.cpp` & `upkie-1.3.2/upkie/utils/tests/datetime_now_string_test.cpp`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/upkie/utils/tests/pinocchio_test.py` & `upkie-1.3.2/upkie/utils/tests/pinocchio_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.1/PKG-INFO` & `upkie-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upkie
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python module to control Upkie wheeled bipeds.
 Keywords: wheeled,biped,robot,balance,motion,control,robotics
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
```

