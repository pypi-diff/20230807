# Comparing `tmp/firexkit-4.7.9.tar.gz` & `tmp/firexkit-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firexkit-4.7.9.tar", last modified: Fri Jan 21 15:58:50 2022, max compression
+gzip compressed data, was "firexkit-5.0.0.tar", last modified: Mon Aug  7 18:52:29 2023, max compression
```

## Comparing `firexkit-4.7.9.tar` & `firexkit-5.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2022-01-21 15:58:50.100314 firexkit-4.7.9/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1592 2022-01-21 15:58:38.000000 firexkit-4.7.9/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       73 2022-01-21 15:58:38.000000 firexkit-4.7.9/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      262 2022-01-21 15:58:50.100314 firexkit-4.7.9/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       38 2022-01-21 15:58:38.000000 firexkit-4.7.9/README.md
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2022-01-21 15:58:50.100314 firexkit-4.7.9/firexkit/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/__init__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2022-01-21 15:58:50.100314 firexkit-4.7.9/firexkit/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11172 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/argument_conversion.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5031 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/bag_of_goodies.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2957 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/broker.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8007 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/chain.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1023 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/firex_exceptions.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1004 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/firexkit_common.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3056 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/inspect.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2022-01-21 15:58:50.098313 firexkit-4.7.9/firexkit/install_resources/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      482 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/install_resources/cloud-ci-install-configs.json
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       82 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/permissions.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3275 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/proc_utils.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2022-01-21 15:58:50.099313 firexkit-4.7.9/firexkit/resources/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2969 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/resources/firex.css
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7676 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/resources/firex_logo.png
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      836 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/resources.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    28876 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/result.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3358 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/revoke.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    57491 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/task.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2022-01-21 15:58:50.099313 firexkit-4.7.9/firexkit/templates/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      300 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/templates/link.html
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2874 2022-01-21 15:58:38.000000 firexkit-4.7.9/firexkit/templates/log_template.html
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2022-01-21 15:58:50.098313 firexkit-4.7.9/firexkit.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      262 2022-01-21 15:58:49.000000 firexkit-4.7.9/firexkit.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      808 2022-01-21 15:58:49.000000 firexkit-4.7.9/firexkit.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2022-01-21 15:58:49.000000 firexkit-4.7.9/firexkit.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       34 2022-01-21 15:58:49.000000 firexkit-4.7.9/firexkit.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       21 2022-01-21 15:58:49.000000 firexkit-4.7.9/firexkit.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        9 2022-01-21 15:58:49.000000 firexkit-4.7.9/firexkit.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2022-01-21 15:58:49.000000 firexkit-4.7.9/firexkit.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      267 2022-01-21 15:58:50.100314 firexkit-4.7.9/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      681 2022-01-21 15:58:38.000000 firexkit-4.7.9/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2022-01-21 15:58:38.000000 firexkit-4.7.9/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 18:52:29.226633 firexkit-5.0.0/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2023-08-07 18:52:07.000000 firexkit-5.0.0/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       73 2023-08-07 18:52:07.000000 firexkit-5.0.0/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      262 2023-08-07 18:52:29.226633 firexkit-5.0.0/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       38 2023-08-07 18:52:07.000000 firexkit-5.0.0/README.md
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 18:52:29.226633 firexkit-5.0.0/firexkit/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/__init__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-08-07 18:52:29.226633 firexkit-5.0.0/firexkit/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11172 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/argument_conversion.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6941 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/bag_of_goodies.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2957 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/broker.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8370 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/chain.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1327 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/firex_exceptions.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1004 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/firexkit_common.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3056 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/inspect.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 18:52:29.225633 firexkit-5.0.0/firexkit/install_resources/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      482 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/install_resources/cloud-ci-install-configs.json
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       82 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/permissions.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3315 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/proc_utils.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 18:52:29.225633 firexkit-5.0.0/firexkit/resources/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3448 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/resources/firex.css
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7676 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/resources/firex_logo.png
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      836 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/resources.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    30496 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/result.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3358 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/revoke.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    64075 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/task.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 18:52:29.226633 firexkit-5.0.0/firexkit/templates/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      300 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/templates/link.html
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2874 2023-08-07 18:52:07.000000 firexkit-5.0.0/firexkit/templates/log_template.html
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 18:52:29.224633 firexkit-5.0.0/firexkit.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      262 2023-08-07 18:52:29.000000 firexkit-5.0.0/firexkit.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      808 2023-08-07 18:52:29.000000 firexkit-5.0.0/firexkit.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 18:52:29.000000 firexkit-5.0.0/firexkit.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       34 2023-08-07 18:52:29.000000 firexkit-5.0.0/firexkit.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       21 2023-08-07 18:52:29.000000 firexkit-5.0.0/firexkit.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        9 2023-08-07 18:52:29.000000 firexkit-5.0.0/firexkit.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 18:52:29.000000 firexkit-5.0.0/firexkit.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      267 2023-08-07 18:52:29.226633 firexkit-5.0.0/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      681 2023-08-07 18:52:07.000000 firexkit-5.0.0/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-07 18:52:07.000000 firexkit-5.0.0/versioneer.py
```

### Comparing `firexkit-4.7.9/LICENSE` & `firexkit-5.0.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-Unless otherwise noted, code on the FireXKit GitHub is licensed under the terms of the following BSD license terms:
+BSD 3-Clause License
 
+Copyright (c) 2022, FireX
+All rights reserved.
 
-Copyright (c) 2018 Cisco and/or its affiliates
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
 
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
-following conditions are met:
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
-1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following
-disclaimer.
-2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following
-disclaimer in the documentation and/or other materials provided with the distribution.
-3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products
-derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
-INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
-WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `firexkit-4.7.9/firexkit/argument_conversion.py` & `firexkit-5.0.0/firexkit/argument_conversion.py`

 * *Files identical despite different names*

### Comparing `firexkit-4.7.9/firexkit/bag_of_goodies.py` & `firexkit-5.0.0/firexkit/bag_of_goodies.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,51 +2,56 @@
 from inspect import Signature
 
 
 class BagOfGoodies(object):
     # Special Char to denote indirect parameter references
     INDIRECT_ARG_CHAR = '@'
 
-    def __init__(self, sig: Signature, args, kwargs):
+    def __init__(self, sig: Signature, args, kwargs, has_returns_from_previous_task=True):
+        self.sig = sig
         args = tuple(args)
+        args = self.resolve_circular_indirect_references(sig, args, has_returns_from_previous_task)
         kwargs = dict(kwargs)
-        self.sig = sig
 
         params = sig.parameters
         # Check if the method signature contains
         # any VAR_KEYWORD (i.e., **kwargs)
         self.varkeyword = False
         for param in params.values():
             if param.kind == param.VAR_KEYWORD:
                 self.varkeyword = True
 
         add_later = {}
         try:
             # If the first positional argument is a
             # dict (i.e., result of a previous task), we need to process it.
-            if isinstance(args[0], dict):
+            if isinstance(args[0], dict) and has_returns_from_previous_task:
                 original_args = args[0]
                 # Remove the RETURN_KEYS_KEY entry
                 if RETURN_KEYS_KEY in original_args:
                     del original_args[RETURN_KEYS_KEY]
                 # Partially bind the remaining arguments
                 ba = sig.bind_partial(*args[1:]).arguments
                 for k, v in original_args.items():
                     # Add k,v pairs from the dictionary that are not in the
                     # partially bound args
                     if k not in ba:
                         # But only if the keys exist in the arguments of the
                         # method signature, or if a varkeyword(e.g. **kwargs)
                         # appeared in the signature
                         if (k in params) or self.varkeyword:
-                            if k not in kwargs:
+                            # if x='@x', and x was present in the original args, we must use it
+                            indirect_to_self = k in kwargs \
+                                               and self._is_indirect(kwargs[k]) \
+                                               and self._get_indirect_key(kwargs[k]) == k
+                            if k not in kwargs or indirect_to_self:
                                 kwargs[k] = v
                         else:
                             # Otherwise, we still need to add this parameter
-                            # later, adter the method is called
+                            # later, after the method is called
                             add_later[k] = v
                 # Remove the dict from the positional arguments
                 args = args[1:]
         except IndexError:
             pass
 
         remove_from_kwargs = {}
@@ -56,23 +61,41 @@
         # Pass in the kwargs that don't appear in the original app signature
         # to be later used possibly by other apps
         add_later.update(remove_from_kwargs)
         # and remove them from the kwargs
         for k in remove_from_kwargs.keys():
             del kwargs[k]
 
+        # remove keys from kwargs that are bound by the positional args
+        bound_args = sig.bind_partial(*args).arguments
+        for k in bound_args.keys():
+            if k in kwargs:
+                del kwargs[k]
+
         self.args = args
         self.kwargs = kwargs
 
         self.return_args = dict(kwargs)
-        self.return_args.update(sig.bind_partial(*args).arguments)
+        self.return_args.update(bound_args)
         self.return_args.update(add_later)
 
         self._apply_indirect()
 
+    def resolve_circular_indirect_references(self, sig: Signature, args: tuple,
+                                             has_returns_from_previous_task: bool) -> tuple:
+        # Handle cases when '@x' is passed positionally to the argument x
+        if len(args) and isinstance(args[0], dict) and has_returns_from_previous_task:
+            bound_args = sig.bind_partial(*args[1:]).arguments
+            for k, v in bound_args.items():
+                if self._is_indirect(v) and self._get_indirect_key(v) == k and k in args[0]:
+                    bound_args[k] = args[0][k]
+            return (args[0],) + tuple(bound_args.values())
+        else:
+            return args
+
     def get_bag(self) -> {}:
         return self.return_args
 
     def update(self, updates: {}):
         self._update(updates)
         self._apply_indirect()
 
@@ -81,15 +104,29 @@
 
         arguments = self.sig.bind_partial(*self.args).arguments
         for k, v in updates.items():
             if k in arguments:
                 arguments[k] = v
             elif k in self.sig.parameters or self.varkeyword:
                 self.kwargs[k] = v
-        self.args = list(arguments.values())
+
+        new_args = []
+        for arg, val in arguments.items():
+            param = self.sig.parameters[arg]
+
+            if param.kind != param.VAR_POSITIONAL:
+                new_args.append(val)
+            else:
+                try:
+                    new_args.extend(val)
+                except TypeError as e:
+                    #  Did we update() a VAR_POSITIONAL arg with a non-iterable arg? Don't do that!
+                    raise ValueError(f'VAR_POSITIONAL argument {arg} should always be an iterable') from e
+
+        self.args = new_args
 
     def split_for_signature(self) -> ([], {}):
         return self.args, self.kwargs
 
     @classmethod
     def _is_indirect(cls, value):
         return hasattr(value, 'startswith') and value.startswith(cls.INDIRECT_ARG_CHAR)
```

### Comparing `firexkit-4.7.9/firexkit/broker.py` & `firexkit-5.0.0/firexkit/broker.py`

 * *Files identical despite different names*

### Comparing `firexkit-4.7.9/firexkit/chain.py` & `firexkit-5.0.0/firexkit/chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,35 +49,36 @@
 
 class InjectArgs(object):
     def __init__(self, **kwargs):
         self.injectArgs = kwargs
 
     def __or__(self, other) -> Union[chain, Signature]:
         if isinstance(other, InjectArgs):
-            self.injectArgs.update(other.injectArgs)
+            r = InjectArgs(**(self.injectArgs | other.injectArgs))
         else:
+            r = other.clone()
             # chains and signatures are both handled by this
-            _inject_args_into_signature(other, **self.injectArgs)
-        return other
-
-    def __ior__(self, other: Union[chain, Signature]) -> Union[chain, Signature]:
-        return self | other
+            _inject_args_into_signature(r, **self.injectArgs)
+        return r
 
 
 def _inject_args_into_signature(sig, **kwargs):
     try:
         # This might be a chain
         task = sig.tasks[0]
     except AttributeError:
         # This might be a Task
         task = sig
 
     existing = task.kwargs.keys()
     subset = {k: v for k, v in kwargs.items() if k not in existing}
-    task.kwargs.update(subset)
+
+    # Don't update kwargs in-place, because that may change the kwargs in the original object
+    # even where the object was cloned in __ior__ above (kwargs isn't copied and is still the same object)
+    task.kwargs = task.kwargs | subset
 
 
 Signature.injectArgs = _inject_args_into_signature
 
 
 def verify_chain_arguments(sig: Signature):
     """
@@ -186,14 +187,19 @@
     """Set arbitrary executions options in every task in the :attr:`sig`"""
     try:
         [task.set(**options) for task in sig.tasks]
     except AttributeError:
         sig.set(**options)
 
 
+def set_use_cache(sig: Signature, use_cache: bool):
+    """Set the :attr:`use_cache` execution option in every task in :attr:`sig`"""
+    set_execution_options(sig, use_cache=use_cache)
+
+
 def set_priority(sig: Signature, priority: int):
     """Set the :attr:`priority` execution option in every task in :attr:`sig`"""
     set_execution_options(sig, priority=priority)
 
 
 def set_queue(sig: Signature, queue):
     """Set the :attr:`queue` execution option in every task in :attr:`sig`"""
@@ -217,12 +223,13 @@
             return '|'.join([task.name for task in sig.tasks])
         except AttributeError:
             return sig.name
 
 
 Signature.set_execution_options = set_execution_options
 Signature.set_priority = set_priority
+Signature.set_use_cache = set_use_cache
 Signature.set_queue = set_queue
 Signature.set_soft_time_limit = set_soft_time_limit
 Signature.set_label = set_label
 Signature.get_label = get_label
 Signature.enqueue = _enqueue
```

### Comparing `firexkit-4.7.9/firexkit/firex_exceptions.py` & `firexkit-5.0.0/firexkit/firex_exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import subprocess
+from signal import Signals
 
 
 def shorten_long_output(output, max_output_str_len=8000):
     if len(output) > max_output_str_len:
         mssg = '\nOutput (last %s chars):\n%s' % (max_output_str_len, output[-max_output_str_len:])
     else:
         mssg = '\nOutput:\n%s' % output
     return mssg
 
 
 class FireXCalledProcessError(subprocess.CalledProcessError):
     def __str__(self):
-        mssg = ("Command '%s' returned non-zero exit status %d. " %
-                (self.cmd, self.returncode))
+        if self.returncode < 0:
+            # POSIX says this is a signal
+            try:
+                signame = Signals(-self.returncode).name
+            except ValueError:
+                signame = -self.returncode
+
+            status = f'signal {signame}'
+        else:
+            status = f'exit code {self.returncode}'
+
+        mssg = f'Command {self.cmd} exited with {status}.'
         if self.output:
             mssg += shorten_long_output(self.output)
         return mssg
 
 
 class FireXInactivityTimeoutExpired(subprocess.TimeoutExpired):
     # When instantiating the exception, make sure you provide the necessary positional args as args, not kwargs.
```

### Comparing `firexkit-4.7.9/firexkit/firexkit_common.py` & `firexkit-5.0.0/firexkit/firexkit_common.py`

 * *Files identical despite different names*

### Comparing `firexkit-4.7.9/firexkit/inspect.py` & `firexkit-5.0.0/firexkit/inspect.py`

 * *Files identical despite different names*

### Comparing `firexkit-4.7.9/firexkit/proc_utils.py` & `firexkit-5.0.0/firexkit/proc_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,29 +17,29 @@
         found = re.findall(firex_uid_dir, i)
         matches += found
     return list(set(matches))
 
 
 def kill_old_procs(proc_name, keepalive=2*24*60*60, regexstr=None):
     all_firex_ids = []
-    for proc in find_current_user_recent_procs(proc_name, keepalive, regexstr):
+    for proc in find_recent_procs(proc_name, keepalive, regexstr):
         try:
             msg = 'Killing %s' % proc.pid
             firex_ids = get_firex_id_from_cmdline(proc.cmdline())
             all_firex_ids += firex_ids
             if firex_ids:
                 msg += ' [%s]' % ', '.join(firex_ids)
             logger.debug(msg)
             proc.kill()
         except Exception as e:
             logger.debug('------ FAILED %r' % e)
     return list(set(all_firex_ids))
 
 
-def find_current_user_recent_procs(proc_name, max_age=2 * 24 * 60 * 60, regexstr=None):
+def find_recent_procs(proc_name, max_age=2*24*60*60, regexstr=None, limit_to_current_user_only=True):
 
     proclist = []
     if regexstr:
         regex = re.compile(regexstr)
     else:
         regex = None
     first_time = True
@@ -71,15 +71,15 @@
                     if elapsed >= max_age:
                         if first_time:
                             keepalive_str = str(timedelta(seconds=max_age))
                             logger.debug('[%s] Processes older than %s:' % (pinfo['name'], keepalive_str))
                             first_time = False
 
                         elapsed_str = str(timedelta(seconds=elapsed))
-                        if pinfo['username'] == username:
+                        if pinfo['username'] == username or limit_to_current_user_only is False:
                             proclist.append(proc)
                             logger.debug('---- pid %s has been active for %s; cmdline=%s' %
                                          (pinfo['pid'], elapsed_str, pinfo['cmdline']))
                         else:
                             logger.debug('---- pid %s has been active for %s but owned by %s, cmdline=%s' %
                                          (pinfo['pid'], elapsed_str, pinfo['username'], pinfo['cmdline']))
     return proclist
```

### Comparing `firexkit-4.7.9/firexkit/resources/firex.css` & `firexkit-5.0.0/firexkit/resources/firex.css`

 * *Files 4% similar despite different names*

```diff
@@ -140,8 +140,37 @@
   text-decoration: none;
   font-family: 'Source Sans Pro',sans-serif;
   cursor: pointer;
   color: #000;
 }
 .header-link a:hover {
   color: #2980ff;
-}
+}
+
+.wrap-collapsible > input[type='checkbox'] { display: none; }
+
+.lbl-toggle::before {
+  content: '[+]';
+}
+
+.wrap-collapsible {
+  display: inline;
+}
+
+.collapsible-content {
+  display: none;
+  max-height: 0px;
+  overflow: hidden;
+}
+
+.wrap-collapsible > .toggle:checked + .lbl-toggle + span + .collapsible-content {
+  display: inline;
+  max-height: 100%;
+}
+
+.wrap-collapsible > .toggle:checked + .lbl-toggle::before {
+  content: '[-]';
+}
+
+.non-collapsing {
+  padding-left: 23px;
+}
```

### Comparing `firexkit-4.7.9/firexkit/resources/firex_logo.png` & `firexkit-5.0.0/firexkit/resources/firex_logo.png`

 * *Files identical despite different names*

### Comparing `firexkit-4.7.9/firexkit/resources.py` & `firexkit-5.0.0/firexkit/resources.py`

 * *Files identical despite different names*

### Comparing `firexkit-4.7.9/firexkit/result.py` & `firexkit-5.0.0/firexkit/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import copy
 import time
 from collections import namedtuple
 import weakref
 
-import traceback
 from pprint import pformat
 from typing import Union, Iterator
 
 from celery import current_app
 from celery.result import AsyncResult
 from celery.signals import before_task_publish, task_prerun, task_postrun
 from celery.states import FAILURE, REVOKED, PENDING, STARTED, RECEIVED, RETRY, SUCCESS, READY_STATES
@@ -325,15 +324,15 @@
 def wait_for_running_tasks_from_results(results, max_wait=2*60, sleep_between_iterations=0.05):
     run_states = set(READY_STATES) | {STARTED, RETRY}
     running_tasks = []
     for result in results:
         if result.state in run_states and not get_task_postrun_info(result):
             running_tasks.append(result)
 
-    max_sleep = sleep_between_iterations * 20  # Somewhat arbitrary
+    max_sleep = sleep_between_iterations * 60  # Somewhat arbitrary
     start_time = last_debug_output = time.monotonic()
     while running_tasks:
         time_now = time.monotonic()
 
         if time_now - last_debug_output >= 30:
             logger.debug(f'Waiting for running task(s): {get_tasks_names_from_results(running_tasks)}')
             last_debug_output = time_now
@@ -415,16 +414,18 @@
                     if sleep_between_iterations*1.01 < max_sleep else max_sleep  # Exponential backoff
 
             # If failure happened in a chain, raise from the failing task within the chain
             _check_for_failure_in_parents(result)
 
             result_state = handle_broker_timeout(getattr, args=(result, 'state'))
             if result_state == REVOKED:
-                #  wait for revoked tasks to actually finish running
-                wait_for_running_tasks_from_results([result])
+                # Wait for revoked tasks to actually finish running
+                # Somewhat long max_wait in case a task does work when revoked, like
+                # killing a child run launched by the task.
+                wait_for_running_tasks_from_results([result], max_wait=5*60)
                 raise ChainRevokedException(task_id=str(result),
                                             task_name=get_task_name_from_result(result))
             if result_state == PENDING:
                 # Pending tasks can be in revoke list. State will still be PENDING.
                 raise ChainRevokedPreRunException(task_id=str(result),
                                                   task_name=get_task_name_from_result(result))
             if result_state == FAILURE:
@@ -557,40 +558,60 @@
         return_keys = results[RETURN_KEYS_KEY]
     except KeyError:
         return {}
     else:
         return {k: results[k] for k in return_keys} if return_keys else {}
 
 
+def get_tasks_inputs_from_result(results: dict) -> dict:
+    # Returns a dict of key-value pairs of inputs passed down in the async result object
+    try:
+        return_keys = list(results[RETURN_KEYS_KEY])
+    except KeyError:
+        return results
+    else:
+        return_keys.append(RETURN_KEYS_KEY)
+        return {k: v for k, v in results.items() if k not in return_keys}
+
+
 def _get_results(result: AsyncResult, return_keys_only=True, merge_children_results=False) -> dict:
+    # Generally,
+    #   1.	Apply inputs from current result
+    #   2.	Apply child results (and inputs) from children (if merge_children_results is True)
+    #   3.	Apply output from current result
+
     results = {}
+    returned_values = {}
     if not result:
         return results
     try:
         if result.successful():
             _results = copy.deepcopy(result.result) if isinstance(result.result, dict) else result.result
             if _results:
-                if return_keys_only:
-                    results = get_task_results(_results)
-                else:
-                    # Delete the RETURN_KEYS_KEY
-                    _results.pop(RETURN_KEYS_KEY, None)
-                    results = _results
+                # these will need to be updated only after the children results are extracted
+                # i.e., node results are applied after children results
+                returned_values = get_task_results(_results)
+                if not return_keys_only:
+                    # Only relevant if merge_children_results is True:
+                    #   If return_keys_only us False, we need to apply the inputs first
+                    #   before applying the results(and inputs) of the children
+                    results = get_tasks_inputs_from_result(_results)
 
         if merge_children_results:
             children = result.children
             if children:
                 for child in children:
                     child_results = get_results(child,
                                                 return_keys_only=return_keys_only,
                                                 merge_children_results=merge_children_results)
                     results.update(child_results)
+
+        results.update(returned_values)
     except Exception as e:
-        logger.error(e)
-        logger.error(traceback.format_exc())
+        logger.exception(e)
 
     return results
 
 
 def results2tuple(results: dict, return_keys: Union[str, tuple]) -> tuple:
     from firexkit.task import FireXTask
     if isinstance(return_keys, str):
@@ -659,14 +680,30 @@
     from firexkit.task import FireXTask
     if not return_keys or return_keys == FireXTask.DYNAMIC_RETURN or return_keys == (FireXTask.DYNAMIC_RETURN,):
         return extracted_dict
     else:
         return results2tuple(extracted_dict, return_keys)
 
 
+def get_results_with_default(result: AsyncResult,
+                             default=None,
+                             error_msg: str = None,
+                             **kwargs):
+    if result.successful():
+        return get_results(result, **kwargs)
+    else:
+        if isinstance(getattr(result, 'result'), Exception):
+            exc_info = result.result
+        else:
+            exc_info = None
+        error_msg = error_msg or f'Unable to get result from {result}'
+        logger.error(error_msg, exc_info=exc_info)
+        return default
+
+
 FIREX_AR_REFS_ATTR = '__firex_ar_refs__'
 
 
 def is_async_result_monkey_patched_to_track():
     return hasattr(AsyncResult, FIREX_AR_REFS_ATTR)
```

### Comparing `firexkit-4.7.9/firexkit/revoke.py` & `firexkit-5.0.0/firexkit/revoke.py`

 * *Files identical despite different names*

### Comparing `firexkit-4.7.9/firexkit/task.py` & `firexkit-5.0.0/firexkit/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 import textwrap
 from collections import OrderedDict
 import inspect
 from functools import partial
 from typing import Callable, Iterable, Optional, Union
 from urllib.parse import urljoin
 from copy import deepcopy
+import dataclasses
 
-from celery.canvas import Signature
+from celery.canvas import Signature, _chain
 from celery.result import AsyncResult
 from celery.states import REVOKED
 from contextlib import contextmanager
 from enum import Enum
 from logging.handlers import WatchedFileHandler
-from types import MethodType
+from types import MethodType, MappingProxyType
 from abc import abstractmethod
 from celery.app.task import Task
 from celery.local import PromiseProxy
 from celery.signals import task_prerun, task_postrun, task_revoked
 from celery.utils.log import get_task_logger, get_logger
 from firexkit.bag_of_goodies import BagOfGoodies
 from firexkit.argument_conversion import ConverterRegister
@@ -35,14 +36,36 @@
 import time
 
 REPLACEMENT_TASK_NAME_POSTFIX = '_orig'
 FIREX_REVOKE_COMPLETE_EVENT_TYPE = 'task-firex-revoked'
 
 logger = get_task_logger(__name__)
 
+################################################################
+# Monkey patching
+_orig_chain_apply_async__ = _chain.apply_async
+
+
+def _chain_apply_async(self: _chain, *args: tuple, **kwargs: dict) -> AsyncResult:
+    try:
+        chain_depth = 0
+        for task in self.tasks:
+            task.kwargs['chain_depth'] = chain_depth
+            chain_depth += 1
+    except AttributeError:
+        pass
+    return _orig_chain_apply_async__(self, *args, **kwargs)
+
+
+_chain.apply_async = _chain_apply_async
+
+
+class NotInCache(Exception):
+    pass
+
 
 class TaskContext:
     pass
 
 
 class PendingChildStrategy(Enum):
     """
@@ -170,14 +193,61 @@
 
 
 def _set_taskid_in_db_key(result: AsyncResult, db, db_key):
     db.set(db_key, result.id)
     logger.debug(f'Key {db_key} set to {result.id}')
 
 
+class DictWillNotAllowWrites(dict):
+    def __init__(self, _instrumentation_context=None, **kwargs):
+        self.context = _instrumentation_context
+        super().__init__(**kwargs)
+
+    def warn(self):
+        if self.context:
+            try:
+                self.context.send_task_instrumentation_event(abog_written_to=True)
+            except Exception:
+                logger.exception('Could not send instrumentation event')
+        try:
+            raise DeprecationWarning('DEPRECATION NOTICE: self.bog does not allow assignment. '
+                                     'Please use self.abog.copy() to create a copy of the abog that you can write to. '
+                                     'This will become an aborting failure starting January 1, 2023.')
+        except DeprecationWarning as e:
+            logger.exception(e)
+
+    def __setitem__(self, *args, **kwargs):
+        self.warn()
+        super().__setitem__(*args, **kwargs)
+
+    def __delitem__(self, *args, **kwargs):
+        self.warn()
+        super().__delitem__(*args, **kwargs)
+
+    def pop(self, *args, **kwargs):
+        self.warn()
+        return super().pop(*args, **kwargs)
+
+    def popitem(self):
+        self.warn()
+        return super().popitem()
+
+    def clear(self):
+        self.warn()
+        super().clear()
+
+    def setdefault(self, *args, **kwargs):
+        self.warn()
+        return super().setdefault(*args, **kwargs)
+
+    def update(self, *args, **kwargs):
+        self.warn()
+        super().update(*args, **kwargs)
+
+
 class FireXTask(Task):
     """
     Task object that facilitates passing of arguments and return values from one task to another, to be used in chains
     """
     DYNAMIC_RETURN = '__DYNAMIC_RETURN__'
     RETURN_KEYS_KEY = RETURN_KEYS_KEY
 
@@ -283,19 +353,21 @@
     def from_plugin(self, value):
         self._from_plugin = value
 
     def initialize_context(self):
         self.context.enqueued_children = {}
         self.context.bog = None
 
-        # Favour @app.task(flame=...) driven-style when present over @flame() annotation style.
         # Flame configs need to be on self.context b/c they write to flame_data_configs[k]['on_next'] for collapse ops.
         # Might make more sense to rework that to avoid flame data on context.
-        self.context.flame_configs = self.get_task_flame_configs() or deepcopy(getattr(self.undecorated,
-                                                                                       "flame_data_configs", {}))
+        self.context.flame_configs = (
+            deepcopy(getattr(self.undecorated, "flame_data_configs", {}))
+            # Overwrite @app.task(flame=...) driven-style when present over @flame() annotation style.
+            | self.get_task_flame_configs()
+        )
 
     def get_module_file_location(self):
         return sys.modules[self.__module__].__file__
 
     @classmethod
     def is_dynamic_return(cls, value):
         return hasattr(value, 'startswith') and value.startswith(cls.DYNAMIC_RETURN)
@@ -355,25 +427,29 @@
         return re.sub(f"({REPLACEMENT_TASK_NAME_POSTFIX})*$", "", task_name)
 
     @staticmethod
     def get_short_name(task_name):
         # Task name of first task in chain. (I.E. 'task1' in module1.task1|module2.task2)
         return task_name.split('|')[0].split('.')[-1]
 
+    @classmethod
+    def get_short_name_without_orig(cls, task_name):
+        return cls.strip_orig_from_name(cls.get_short_name(task_name))
+
     @property
     def name_without_orig(self):
         return self.strip_orig_from_name(self.name)
 
     @property
     def short_name(self):
         return self.get_short_name(self.name)
 
     @property
     def short_name_without_orig(self):
-        return self.strip_orig_from_name(self.short_name)
+        return self.get_short_name_without_orig(self.name)
 
     @property
     def called_as_orig(self):
         return True if self.name.endswith(REPLACEMENT_TASK_NAME_POSTFIX) else False
 
     @abstractmethod
     def pre_task_run(self, extra_events: Optional[dict] = None):
@@ -526,60 +602,142 @@
         exception_string = str(e)
         if exception_string:
             mssg += f': {exception_string}'
         logger.error(mssg, exc_info=e, extra=extra)
         if raise_exception:
             raise e
 
-    def _process_arguments_and_run(self, *args, **kwargs):
-        # Organise the input args by creating a BagOfGoodies
-        self.context.bog = BagOfGoodies(self.sig, args, kwargs)
-
-        # run any "pre" converters attached to this task
-        converted = ConverterRegister.task_convert(task_name=self.name, pre_task=True, **self.bag)
-        self.context.bog.update(converted)
-
-        # give sub-classes a chance to do something with the args
-        self.pre_task_run()
-
-        result = super(FireXTask, self).__call__(*self.args, **self.kwargs)
-
-        if not self._decorated_return_keys and self._task_return_keys:
-            result = self.convert_returns_to_dict(self._task_return_keys, result)
-
+    def _process_result(self, result, extra_events: Optional[dict] = None):
         # Need to update the dict with the results, if @results was used
         if isinstance(result, dict):
             self.context.bog.update(result)
 
         # run any post converters attached to this task
-        converted = ConverterRegister.task_convert(task_name=self.name, pre_task=False, **self.bag)
+        converted = ConverterRegister.task_convert(task_name=self.name, pre_task=False, **self.bag.copy())
         self.context.bog.update(converted)
 
         if isinstance(result, dict):
             # update the results with changes from converters
             result = {k: v for k, v in self.bag.items() if k in result}
 
-        # give sub-classes a change to do something with the results
-        self.post_task_run(result)
+        # give sub-classes a chance to do something with the results
+        self.post_task_run(result, extra_events=extra_events)
+
+        return self.bag.copy()
+
+    def convert_results_if_returns_defined_by_task_definition(self, result):
+        # If @returns decorator was used, we don't need to convert since that's taken care by the decorator
+        if not self._decorated_return_keys and self._task_return_keys:
+            # This is only used if the @app.task(returns=) is used
+            result = self.convert_returns_to_dict(self._task_return_keys, result)
+        return result
+
+    def _get_cache_key(self):
+        # Need a sting hash of name + all_args
+        return str((self.name,) + tuple(sorted(self.all_args.items())))
+
+    def _cache_get(self, cache_key):
+        cached_uuid = self.backend.get(cache_key)
+        if cached_uuid is None:
+            raise NotInCache()
+        cached_uuid = cached_uuid.decode()
+        logger.info(f'[Caching] found entry for key {cache_key!r} at {cached_uuid!r}')
+        return cached_uuid
+
+    def _cache_set(self, cache_key, uuid):
+        # We need to just store a reference  to the uuid (no need to store the result again)
+        logger.debug(f'[Caching] storing entry for key {cache_key!r} -> {uuid!r}')
+        self.backend.set(cache_key, uuid)
+
+    @classmethod
+    def _run_from_cache(cls, cached_uuid):
+        # Retrieve the result of the original cached uuid from the backend
+        result = cls.app.backend.get_result(cached_uuid)
+        cleaned_result = cls.convert_cached_results(result)
+        return cleaned_result
+
+    @classmethod
+    def convert_cached_results(cls, result):
+        return_keys = result.get('__task_return_keys', ()) + ('__task_return_keys',)
+        return {k: v for k, v in result.items() if k in return_keys}
+
+    @property
+    def default_use_cache(self):
+        return getattr(self, 'use_cache', None)
+
+    def is_cache_enabled(self):
+        use_cache_value = self.default_use_cache
+        if not self.request.called_directly:
+            try:
+                request_use_cache = self.request.properties['use_cache']
+            except KeyError:
+                pass
+            else:
+                if request_use_cache is not None:
+                    if request_use_cache != self.default_use_cache:
+                        logger.debug(f'use_cache default value of {self.default_use_cache!r} for task {self.name!r} '
+                                     f'was overridden by enqueue to {request_use_cache!r}')
+                    use_cache_value = request_use_cache
+        return bool(use_cache_value)
+
+    def cache_call(self):
+        cache_key = self._get_cache_key()
+        try:
+            cached_uuid = self._cache_get(cache_key)
+        except NotInCache:
+            logger.debug(f'[Caching] No entry found for key {cache_key!r}')
+            result = self.real_call()
+            self._cache_set(cache_key, self.request.id)
+            return result
+        else:
+            result = self._run_from_cache(cached_uuid)
+            converted_result = self.convert_cached_results(result)
+            return self._process_result(converted_result,
+                                        extra_events={'cached_result_from': cached_uuid})
+
+    def real_call(self):
+        result = super(FireXTask, self).__call__(*self.args, **self.kwargs)
+        converted_result = self.convert_results_if_returns_defined_by_task_definition(result)
+        return self._process_result(converted_result)
 
-        return self.bag
+    def final_call(self, *args, **kwargs):
+        if self.is_cache_enabled():
+            return self.cache_call()
+        else:
+            return self.real_call()
+
+    def _process_arguments_and_run(self, *args, **kwargs):
+        # Organise the input args by creating a BagOfGoodies
+        self.context.bog = BagOfGoodies(self.sig,
+                                        args,
+                                        kwargs,
+                                        has_returns_from_previous_task=kwargs.get('chain_depth', 0) > 0)
+
+        # run any "pre" converters attached to this task
+        converted = ConverterRegister.task_convert(task_name=self.name, pre_task=True, **self.bag.copy())
+        self.context.bog.update(converted)
+
+        # give sub-classes a chance to do something with the args
+        self.pre_task_run()
+
+        return self.final_call(*self.args, **self.kwargs)
 
     def retry(self, *args, **kwargs):
         # Adds some logging to the original task retry
 
         if not self.request.called_directly:
             if self.request.retries == self.max_retries:
                 logger.error(f'{self.short_name} failed all {self.max_retries} retry attempts')
             else:
                 logger.warning(f'{self.short_name} failed and retrying {self.request.retries+1}/{self.max_retries}')
         super(FireXTask, self).retry(*args, **kwargs)
 
     @property
-    def bag(self) -> dict:
-        return self.context.bog.get_bag()
+    def bag(self) -> MappingProxyType:
+        return MappingProxyType(self.context.bog.get_bag())
 
     @property
     def required_args(self) -> list:
         """
         :return: list of required arguments to the microservice.
         """
         if self._in_required is None:
@@ -602,15 +760,19 @@
     @staticmethod
     def _get_default_bound_args(sig, bound_args) -> dict:
         # Find and store the remaining default arguments for debugging purposes
         default_bound_args = OrderedDict()
         params = sig.parameters
         for param in params.values():
             if param.name not in bound_args:
-                default_bound_args[param.name] = param.default
+                if param.default == param.empty and param.kind == param.VAR_POSITIONAL:
+                    # The param.default is set to param.empty in such cases, and need to be a tuple instead
+                    default_bound_args[param.name] = tuple()
+                else:
+                    default_bound_args[param.name] = param.default
         return default_bound_args
 
     @property
     def args(self) -> list:
         return self.context.bog.args
 
     @property
@@ -622,30 +784,33 @@
         return self._get_bound_args(self.sig, self.args, self.kwargs)
 
     @property
     def default_bound_args(self) -> dict:
         return self._get_default_bound_args(self.sig, self.bound_args)
 
     def map_input_args_kwargs(self, *args, **kwargs) -> ((), {}):
-        b = BagOfGoodies(self.sig, *args, **kwargs)
+        b = BagOfGoodies(self.sig,
+                         *args,
+                         **kwargs,
+                         has_returns_from_previous_task=kwargs.get('chain_depth', 0) > 0)
         return b.args, b.kwargs
 
     def map_args(self, *args, **kwargs) -> dict:
         args, kwargs = self.map_input_args_kwargs(args, kwargs)
         bound_args = self._get_bound_args(self.sig, args, kwargs)
         default_bound_args = self._get_default_bound_args(self.sig, bound_args)
         return {**bound_args, **default_bound_args}
 
     @property
-    def all_args(self) -> dict:
-        return {**self.bound_args, **self.default_bound_args}
+    def all_args(self) -> MappingProxyType:
+        return MappingProxyType({**self.bound_args, **self.default_bound_args})
 
     @property
-    def abog(self) -> dict:
-        return {**self.bag, **self.default_bound_args}
+    def abog(self) -> DictWillNotAllowWrites:
+        return DictWillNotAllowWrites(_instrumentation_context=self, **{**self.bag, **self.default_bound_args})
 
     #######################
     # Enqueuing child tasks
 
     _STATE_KEY = 'state'
     _PENDING = 'pending'
     _UNBLOCKED = 'unblocked'
@@ -887,15 +1052,15 @@
 
         task_uid = uid_of_enqueued_task.decode()
         logger.info(f'{enqueue_once_key} is enqueued with task-id: {task_uid}')
         self._send_flame_additional_child(task_uid)
 
         result = AsyncResult(task_uid)
         if block:
-            logger.print(f'Waiting for results of non-child task {get_result_logging_name(result)}')
+            logger.debug(f'Waiting for results of non-child task {get_result_logging_name(result)}')
             wait_on_async_results_and_maybe_raise(results=result, caller_task=self, **kwargs)
         return result
 
     def enqueue_child_once_and_extract(self,
                                        *args,
                                        enqueue_once_key: str,
                                        **kwargs) -> [tuple, dict]:
@@ -910,28 +1075,28 @@
 
         return self._enqueue_child_and_extract(*args,
                                                enqueue_once_key=enqueue_once_key,
                                                extract_from_parents=False,
                                                **kwargs)
 
     def enqueue_in_parallel(self, chains, max_parallel_chains=15, wait_for_completion=True,
-                            raise_exception_on_failure=False):
+                            raise_exception_on_failure=False, **kwargs):
         """ This method executes the provided list of Signatures/Chains in parallel
         and returns the associated list of "async_result" objects.
         The results are returned in the same order as the input Signatures/Chains."""
         promises = []
         scheduled = []
         for c in chains:
             if len(scheduled) >= max_parallel_chains:
                 # Reach the max allowed parallel chains, wait for one to complete before scheduling the next one.
                 async_res = next(wait_for_any_results(scheduled, raise_exception_on_failure=raise_exception_on_failure))
                 scheduled.remove(async_res)
             # Schedule the next child
             logger.debug(f'Enqueueing: {c.get_label()}')
-            promise = self.enqueue_child(c)
+            promise = self.enqueue_child(c, **kwargs)
             scheduled.append(promise)
             promises.append(promise)
         if wait_for_completion or raise_exception_on_failure:
             # Wait for all children to complete
             self.wait_for_specific_children(promises, raise_exception_on_failure=raise_exception_on_failure)
         return promises
 
@@ -1108,15 +1273,15 @@
             return
 
         if getattr(self.context, 'flame_configs', False):
             def safe_format(formatter, fromatter_args, formatter_kwargs):
                 try:
                     return formatter(*fromatter_args, **formatter_kwargs)
                 except Exception as e:
-                    logger.error(e)
+                    logger.exception(e)
                     return None
 
             formatted_data = {}
             for flame_key, flame_config in self.context.flame_configs.items():
                 # Data can be sent either because it is supplied in the input or if data was registered to be sent
                 # 'on_next' during flame_data_config registration.
                 if flame_key in data \
@@ -1281,14 +1446,20 @@
 
     return None
 
 def convert_to_serializable(obj, max_recursive_depth=10, _depth=0):
     if hasattr(obj, 'firex_serializable'):
         return obj.firex_serializable()
 
+    if dataclasses.is_dataclass(obj):
+        try:
+            obj = dataclasses.asdict(obj)
+        except TypeError:
+            pass # e.g. enums
+
     if is_jsonable(obj):
         return obj
 
     # recursive reference guard.
     if _depth < max_recursive_depth:
         # Full object isn't jsonable, but some contents might be. Try walking the structure to get jsonable parts.
         if isinstance(obj, dict):
```

### Comparing `firexkit-4.7.9/firexkit/templates/log_template.html` & `firexkit-5.0.0/firexkit/templates/log_template.html`

 * *Files identical despite different names*

### Comparing `firexkit-4.7.9/firexkit.egg-info/SOURCES.txt` & `firexkit-5.0.0/firexkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firexkit-4.7.9/setup.py` & `firexkit-5.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,14 @@
       license='BSD-3-Clause',
       packages=['firexkit', ],
       package_data={
             'firexkit': ['resources/*', 'templates/*', 'install_resources/*']
       },
       zip_safe=True,
       install_requires=[
-            "celery==5.2.0",
+            "celery==5.3.1",
             "jinja2",
       ],
       entry_points={
             'firex.core': 'firexkit = firexkit'
       },
      )
```

### Comparing `firexkit-4.7.9/versioneer.py` & `firexkit-5.0.0/versioneer.py`

 * *Files identical despite different names*

