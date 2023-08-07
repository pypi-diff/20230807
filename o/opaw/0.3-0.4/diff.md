# Comparing `tmp/opaw-0.3.tar.gz` & `tmp/opaw-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opaw-0.3.tar", last modified: Fri Aug  4 17:58:51 2023, max compression
+gzip compressed data, was "opaw-0.4.tar", last modified: Mon Aug  7 11:41:08 2023, max compression
```

## Comparing `opaw-0.3.tar` & `opaw-0.4.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 17:58:51.492965 opaw-0.3/
--rw-rw-rw-   0        0        0      405 2023-08-04 17:58:51.494068 opaw-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-08-04 14:53:26.000000 opaw-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 17:58:51.423498 opaw-0.3/opaw/
--rw-rw-rw-   0        0        0        0 2023-08-04 15:52:21.000000 opaw-0.3/opaw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 17:58:51.467924 opaw-0.3/opaw/examples/
--rw-rw-rw-   0        0        0      110 2023-08-04 17:27:47.000000 opaw-0.3/opaw/examples/__init__.py
--rw-rw-rw-   0        0        0      520 2023-08-04 17:27:47.000000 opaw-0.3/opaw/examples/audio.py
--rw-rw-rw-   0        0        0      864 2023-08-04 17:48:41.000000 opaw-0.3/opaw/examples/basic.py
--rw-rw-rw-   0        0        0      428 2023-08-04 17:40:26.000000 opaw-0.3/opaw/examples/chat.py
--rw-rw-rw-   0        0        0      370 2023-08-04 17:30:39.000000 opaw-0.3/opaw/examples/completion.py
--rw-rw-rw-   0        0        0      420 2023-08-04 17:30:39.000000 opaw-0.3/opaw/examples/edit.py
--rw-rw-rw-   0        0        0      404 2023-08-04 17:30:39.000000 opaw-0.3/opaw/examples/embedding.py
--rw-rw-rw-   0        0        0      624 2023-08-04 17:30:39.000000 opaw-0.3/opaw/examples/file.py
--rw-rw-rw-   0        0        0      497 2023-08-04 17:30:39.000000 opaw-0.3/opaw/examples/finetune.py
--rw-rw-rw-   0        0        0      659 2023-08-04 17:30:39.000000 opaw-0.3/opaw/examples/function_call.py
--rw-rw-rw-   0        0        0      389 2023-08-04 17:30:39.000000 opaw-0.3/opaw/examples/image.py
--rw-rw-rw-   0        0        0      606 2023-08-04 17:30:39.000000 opaw-0.3/opaw/examples/moderation.py
--rw-rw-rw-   0        0        0       29 2023-08-03 17:18:41.000000 opaw-0.3/opaw/main.py
-drwxrwxrwx   0        0        0        0 2023-08-04 17:58:51.485105 opaw-0.3/opaw/model/
--rw-rw-rw-   0        0        0        0 2023-07-31 12:07:48.000000 opaw-0.3/opaw/model/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-08-04 16:20:25.000000 opaw-0.3/opaw/model/audio.py
--rw-rw-rw-   0        0        0     1320 2023-08-03 11:13:00.000000 opaw-0.3/opaw/model/bot.py
--rw-rw-rw-   0        0        0     2310 2023-08-04 16:20:25.000000 opaw-0.3/opaw/model/chat.py
--rw-rw-rw-   0        0        0      635 2023-08-04 16:20:25.000000 opaw-0.3/opaw/model/completion.py
--rw-rw-rw-   0        0        0      638 2023-08-04 16:20:25.000000 opaw-0.3/opaw/model/edit.py
--rw-rw-rw-   0        0        0      634 2023-08-04 16:20:25.000000 opaw-0.3/opaw/model/embedding.py
--rw-rw-rw-   0        0        0     1040 2023-08-04 16:20:25.000000 opaw-0.3/opaw/model/file.py
--rw-rw-rw-   0        0        0     1107 2023-08-04 16:20:25.000000 opaw-0.3/opaw/model/finetune.py
--rw-rw-rw-   0        0        0     1287 2023-08-04 16:20:25.000000 opaw-0.3/opaw/model/image.py
--rw-rw-rw-   0        0        0      663 2023-08-04 16:20:25.000000 opaw-0.3/opaw/model/moderation.py
-drwxrwxrwx   0        0        0        0 2023-08-04 17:58:51.488099 opaw-0.3/opaw/tool/
--rw-rw-rw-   0        0        0      553 2023-08-04 16:20:25.000000 opaw-0.3/opaw/tool/__init__.py
--rw-rw-rw-   0        0        0      226 2023-07-30 07:02:06.000000 opaw-0.3/opaw/tool/stock.py
-drwxrwxrwx   0        0        0        0 2023-08-04 17:58:51.491090 opaw-0.3/opaw/util/
--rw-rw-rw-   0        0        0      967 2023-08-04 17:49:35.000000 opaw-0.3/opaw/util/__init__.py
--rw-rw-rw-   0        0        0      828 2023-08-04 16:03:00.000000 opaw-0.3/opaw/util/log.py
-drwxrwxrwx   0        0        0        0 2023-08-04 17:58:51.446478 opaw-0.3/opaw.egg-info/
--rw-rw-rw-   0        0        0      405 2023-08-04 17:58:51.000000 opaw-0.3/opaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-08-04 17:58:51.000000 opaw-0.3/opaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 17:58:51.000000 opaw-0.3/opaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 17:58:51.000000 opaw-0.3/opaw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-04 17:58:51.000000 opaw-0.3/opaw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-08-04 17:58:51.495912 opaw-0.3/setup.cfg
--rw-rw-rw-   0        0        0      604 2023-08-04 17:58:49.000000 opaw-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:41:08.492166 opaw-0.4/
+-rw-rw-rw-   0        0        0     1085 2023-08-06 16:29:18.000000 opaw-0.4/LICENSE
+-rw-rw-rw-   0        0        0     1644 2023-08-07 11:41:08.492842 opaw-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-08-07 10:48:35.000000 opaw-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 11:41:08.385269 opaw-0.4/opaw/
+-rw-rw-rw-   0        0        0        0 2023-08-04 15:52:21.000000 opaw-0.4/opaw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:41:08.445536 opaw-0.4/opaw/examples/
+-rw-rw-rw-   0        0        0      110 2023-08-04 17:27:47.000000 opaw-0.4/opaw/examples/__init__.py
+-rw-rw-rw-   0        0        0      589 2023-08-07 06:42:53.000000 opaw-0.4/opaw/examples/audio.py
+-rw-rw-rw-   0        0        0     1058 2023-08-07 07:02:30.000000 opaw-0.4/opaw/examples/basic.py
+-rw-rw-rw-   0        0        0      548 2023-08-07 06:54:13.000000 opaw-0.4/opaw/examples/chat.py
+-rw-rw-rw-   0        0        0      457 2023-08-07 06:56:50.000000 opaw-0.4/opaw/examples/completion.py
+-rw-rw-rw-   0        0        0      574 2023-08-07 09:46:04.000000 opaw-0.4/opaw/examples/edit.py
+-rw-rw-rw-   0        0        0      476 2023-08-07 06:58:39.000000 opaw-0.4/opaw/examples/embedding.py
+-rw-rw-rw-   0        0        0      658 2023-08-07 06:59:42.000000 opaw-0.4/opaw/examples/file.py
+-rw-rw-rw-   0        0        0      601 2023-08-07 07:04:07.000000 opaw-0.4/opaw/examples/finetune.py
+-rw-rw-rw-   0        0        0      743 2023-08-07 09:09:21.000000 opaw-0.4/opaw/examples/funcs.py
+-rw-rw-rw-   0        0        0      775 2023-08-07 09:09:21.000000 opaw-0.4/opaw/examples/function_call.py
+-rw-rw-rw-   0        0        0      453 2023-08-07 07:05:59.000000 opaw-0.4/opaw/examples/image.py
+-rw-rw-rw-   0        0        0      510 2023-08-07 07:06:55.000000 opaw-0.4/opaw/examples/load-chat.py
+-rw-rw-rw-   0        0        0      718 2023-08-07 06:25:24.000000 opaw-0.4/opaw/examples/moderation.py
+-rw-rw-rw-   0        0        0        0 2023-08-07 06:24:33.000000 opaw-0.4/opaw/main.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:41:08.476327 opaw-0.4/opaw/model/
+-rw-rw-rw-   0        0        0        0 2023-08-07 05:55:31.000000 opaw-0.4/opaw/model/__init__.py
+-rw-rw-rw-   0        0        0     1189 2023-08-06 14:28:25.000000 opaw-0.4/opaw/model/audio.py
+-rw-rw-rw-   0        0        0     2062 2023-08-06 14:16:59.000000 opaw-0.4/opaw/model/bot.py
+-rw-rw-rw-   0        0        0     3432 2023-08-07 09:05:54.000000 opaw-0.4/opaw/model/chat.py
+-rw-rw-rw-   0        0        0      629 2023-08-06 08:24:20.000000 opaw-0.4/opaw/model/completion.py
+-rw-rw-rw-   0        0        0      736 2023-08-07 09:49:15.000000 opaw-0.4/opaw/model/edit.py
+-rw-rw-rw-   0        0        0      625 2023-08-06 14:28:25.000000 opaw-0.4/opaw/model/embedding.py
+-rw-rw-rw-   0        0        0     1215 2023-08-06 15:34:39.000000 opaw-0.4/opaw/model/file.py
+-rw-rw-rw-   0        0        0     1003 2023-08-06 14:28:25.000000 opaw-0.4/opaw/model/finetune.py
+-rw-rw-rw-   0        0        0     1242 2023-08-06 14:05:06.000000 opaw-0.4/opaw/model/image.py
+-rw-rw-rw-   0        0        0      633 2023-08-06 14:28:25.000000 opaw-0.4/opaw/model/moderation.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:41:08.483078 opaw-0.4/opaw/test/
+-rw-rw-rw-   0        0        0        0 2023-07-31 12:07:48.000000 opaw-0.4/opaw/test/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-07 05:57:37.000000 opaw-0.4/opaw/test/test.py
+-rw-rw-rw-   0        0        0       47 2023-08-06 07:05:13.000000 opaw-0.4/opaw/test/test2.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:41:08.489243 opaw-0.4/opaw/util/
+-rw-rw-rw-   0        0        0     1057 2023-08-07 07:08:55.000000 opaw-0.4/opaw/util/__init__.py
+-rw-rw-rw-   0        0        0     1096 2023-08-07 06:27:22.000000 opaw-0.4/opaw/util/log.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:41:08.406378 opaw-0.4/opaw.egg-info/
+-rw-rw-rw-   0        0        0     1644 2023-08-07 11:41:08.000000 opaw-0.4/opaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-08-07 11:41:08.000000 opaw-0.4/opaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 11:41:08.000000 opaw-0.4/opaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 11:41:08.000000 opaw-0.4/opaw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-07 11:41:08.000000 opaw-0.4/opaw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-08-07 11:41:08.496666 opaw-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-08-07 11:28:06.000000 opaw-0.4/setup.py
```

### Comparing `opaw-0.3/opaw/model/audio.py` & `opaw-0.4/opaw/model/audio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 import openai
 from opaw.model.bot import Bot
 
-
 class AudioBot(Bot):
     """
     https://platform.openai.com/docs/api-reference/audio
     """
 
     def __init__(self, model="whisper-1"):
         super().__init__(model, "audio")
 
-    def create(self, prompt, **kargs):
+    def create(self, file, **kargs):
         """
         :kargs: select task "stt(transcript)" or "mt(translation)"
 
         language (stt): https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes
         """
-        if prompt is None or not kargs.get("task"):
+        if file is None or not kargs.get("task"):
             return None
-        file = prompt
-
-        request = {
-            "model": self.model,
-            "file": open(file, "rb"),
-            **kargs
-        }
-        self._history_req(file, kargs)
-
 
         model = openai.Audio
         methods = {
             "transcript": model.transcribe,
             "stt": model.transcribe,
             "translation": model.translate,
             "mt": model.translate,
         }
 
         # remove task from request
-        task = request.pop('task')
+        task = kargs.pop('task')
         if task not in methods:
             return None
 
+        request = {
+            "model": self.model,
+            "file": file,
+            **kargs
+        }
+        self._history_req(request)
 
+        request["file"] = open(file, "rb")
         response = methods[task](**request)
         self._history_res(response)
         return response
-
```

### Comparing `opaw-0.3/opaw/model/completion.py` & `opaw-0.4/opaw/model/completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
         request = {
             "model": self.model,
             "prompt": prompt,
             **kargs
         }
 
-        self._history_req(prompt, kargs)
+        self._history_req(request)
         response = openai.Completion.create(**request)
         self._history_res(response)
         return response
```

### Comparing `opaw-0.3/opaw/model/edit.py` & `opaw-0.4/opaw/model/edit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import openai
 from opaw.model.bot import Bot
 
 
 class EditBot(Bot):
     """
+    Deprecated model
+
     https://platform.openai.com/docs/api-reference/edits
     """
 
     def __init__(self, model="text-davinci-edit-001"):
+        """
+        Deprecated model
+        """
         super().__init__(model, "edit")
 
-    def create(self, prompt, **kargs):
-        input = prompt
+    def create(self, input, **kargs):
+        """
+        Deprecated model
+        """
         if input is None:
             return None
 
         request = {
             "model": self.model,
             "input": input,
             **kargs
         }
 
-        self._history_req(input, kargs)
+        self._history_req(request)
         response = openai.Edit.create(**request)
         self._history_res(response)
         return response
```

### Comparing `opaw-0.3/opaw/model/file.py` & `opaw-0.4/opaw/model/finetune.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import openai
 from opaw.model.bot import Bot
 
 
-class FileBot(Bot):
+class FinetuneBot(Bot):
     """
-    https://platform.openai.com/docs/api-reference/files
+    https://platform.openai.com/docs/api-reference/fine-tunes
     """
 
-    def __init__(self):
-        super().__init__("bot", "file")
+    def __init__(self, model="curie"):
+        super().__init__(model, "finetune")
 
-    def create(self, prompt=None, **kargs):
+    def create(self, _=None, **kargs):
         """
-        :param prompt: is not used for model, just memo in history (use kargs)
+        :param _: is not used (use kargs instead)
         """
         if not kargs.get("task"):
             return None
-        memo = prompt
 
-        request = {
-            **kargs
-        }
-        self._history_req(memo, kargs)
-
-        model = openai.File
+        model = openai.FineTune
         methods = {
+            "create": model.create,
             "list": model.list,
-            "upload": model.create,
-            "delete": model.delete,
             "retrieve": model.retrieve,
-            "download": model.download,
+            "cancel": model.cancel,
+            "delete": model.delete,
         }
 
-        # remove task from request
-        task = request.pop('task')
+        task = kargs.pop('task')
         if task not in methods:
             return None
 
+        request = {
+            "model": self.model,
+            **kargs
+        }
+        self._history_req(request)
+
         response = methods[task](**request)
         self._history_res(response)
         return response
```

### Comparing `opaw-0.3/opaw/model/finetune.py` & `opaw-0.4/opaw/model/moderation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,26 @@
 import openai
 from opaw.model.bot import Bot
 
 
-class FinetuneBot(Bot):
+class ModerationBot(Bot):
     """
-    https://platform.openai.com/docs/api-reference/fine-tunes
+    https://platform.openai.com/docs/api-reference/moderations
     """
 
-    def __init__(self, model="curie"):
-        super().__init__(model, "finetune")
+    def __init__(self, model="text-moderation-latest"):
+        super().__init__(model, "moderation")
 
-    def create(self, prompt, **kargs):
-        """
-        :param prompt: is not used for model. just for memo in history
-        """
-        if prompt is None or not kargs.get("task"):
+    def create(self, input, **kargs):
+        if input is None:
             return None
-        memo = prompt
 
         request = {
             "model": self.model,
+            "input": input,
             **kargs
         }
-        self._history_req(memo, kargs)
 
-        model = openai.FineTune
-        methods = {
-            "create": model.create,
-            "list": model.list,
-            "retrieve": model.retrieve,
-            "cancel": model.cancel,
-            "delete": model.delete,
-        }
-
-        # remove task from request
-        task = request.pop('task')
-        if task not in methods:
-            return None
-
-        response = methods[task](**request)
+        self._history_req(request)
+        response = openai.Moderation.create(**request)
         self._history_res(response)
         return response
```

### Comparing `opaw-0.3/opaw/model/image.py` & `opaw-0.4/opaw/model/image.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,38 +13,37 @@
     def create(self, prompt, **kargs):
         """
         :kargs: select task "create" or "edit" or "variation"
         """
         if prompt is None or not kargs.get("task"):
             return None
 
-        request = {
-            "model": self.model,
-            "prompt": prompt,
-            **kargs
-        }
-
-        self._history_req(prompt, kargs)
-
         model = openai.Image
         methods = {
             "create": model.create,
             "edit": model.create_edit,
             "variation": model.create_variation
         }
 
-        # remove task from request
-        task = request.pop('task')
+        task = kargs.pop('task')
         if task not in methods:
             return None
 
-        # remove model key from request
-        request.pop("model")
+        request = {
+            "prompt": prompt,
+            **kargs
+        }
+
+        if task == "variation":  # remove prompt when variation
+            request.pop("prompt")
+
+        self._history_req(request)
+
         response = methods[task](**request)
         self._history_res(response)
         return response
 
     def img_format(self, img):
         """
         img could be url or data scheme encoded in base64
         """
-        return "url" if img.startswith("http") else "data"
+        return "url" if img.startswith("http") else "data"
```

### Comparing `opaw-0.3/opaw.egg-info/SOURCES.txt` & `opaw-0.4/opaw.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 opaw/__init__.py
 opaw/main.py
 opaw.egg-info/PKG-INFO
 opaw.egg-info/SOURCES.txt
@@ -13,25 +14,28 @@
 opaw/examples/basic.py
 opaw/examples/chat.py
 opaw/examples/completion.py
 opaw/examples/edit.py
 opaw/examples/embedding.py
 opaw/examples/file.py
 opaw/examples/finetune.py
+opaw/examples/funcs.py
 opaw/examples/function_call.py
 opaw/examples/image.py
+opaw/examples/load-chat.py
 opaw/examples/moderation.py
 opaw/model/__init__.py
 opaw/model/audio.py
 opaw/model/bot.py
 opaw/model/chat.py
 opaw/model/completion.py
 opaw/model/edit.py
 opaw/model/embedding.py
 opaw/model/file.py
 opaw/model/finetune.py
 opaw/model/image.py
 opaw/model/moderation.py
-opaw/tool/__init__.py
-opaw/tool/stock.py
+opaw/test/__init__.py
+opaw/test/test.py
+opaw/test/test2.py
 opaw/util/__init__.py
 opaw/util/log.py
```

### Comparing `opaw-0.3/setup.py` & `opaw-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
+# pypi long description
+with open("README.md", encoding="utf-8") as f:
+    long_description = f.read()
+
 setup(
     name='opaw',
     packages=find_packages(),
-    version='0.3',
+    version='0.4',
     license='MIT',
     description='Unofficial python wrapper of OpenAI API.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='hiimanget',
     author_email='hiimanget@gmail.com',
     url='https://github.com/hiimanget/openai-pw',
     keywords=['openai', 'python', 'api', 'wrapper'],
     install_requires=['openai'],
     classifiers=[
         "Programming Language :: Python :: 3",
```

