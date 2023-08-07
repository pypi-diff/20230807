# Comparing `tmp/strawberry_django_auth-0.375.0.tar.gz` & `tmp/strawberry_django_auth-0.376.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_auth-0.375.0.tar", max compression
+gzip compressed data, was "strawberry_django_auth-0.376.0.tar", max compression
```

## Comparing `strawberry_django_auth-0.375.0.tar` & `strawberry_django_auth-0.376.0.tar`

### file list

```diff
@@ -1,56 +1,51 @@
--rw-r--r--   0        0        0     1075 2023-07-10 04:00:36.059143 strawberry_django_auth-0.375.0/LICENSE
--rw-r--r--   0        0        0     3820 2023-07-10 04:00:36.059143 strawberry_django_auth-0.375.0/README.md
--rw-r--r--   0        0        0       24 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/__init__.py
--rw-r--r--   0        0        0      168 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/admin.py
--rw-r--r--   0        0        0      215 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/apps.py
--rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/__init__.py
--rw-r--r--   0        0        0     1267 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/captcha_factorty.py
--rw-r--r--   0        0        0     6618 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/create.py
--rw-r--r--   0        0        0    16724 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/Nehama.ttf
--rw-r--r--   0        0        0   221328 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
--rw-r--r--   0        0        0    45448 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/pltwide.ttf
--rwxr-xr-x   0        0        0    22768 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/stam.ttf
--rw-r--r--   0        0        0     3248 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/models.py
--rw-r--r--   0        0        0      448 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/types_.py
--rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/__init__.py
--rw-r--r--   0        0        0     1995 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/constants.py
--rw-r--r--   0        0        0      910 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/directives.py
--rw-r--r--   0        0        0     1093 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/exceptions.py
--rw-r--r--   0        0        0      231 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/interfaces.py
--rw-r--r--   0        0        0     4662 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/middlewares.py
--rw-r--r--   0        0        0     1453 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/mixins.py
--rw-r--r--   0        0        0     1516 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/scalars.py
--rw-r--r--   0        0        0      857 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/types_.py
--rw-r--r--   0        0        0     4063 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/jwt/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/jwt/tools.py
--rw-r--r--   0        0        0     7498 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/jwt/types_.py
--rw-r--r--   0        0        0     2969 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/0001_initial.py
--rw-r--r--   0        0        0      355 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/0002_alter_userstatus_options.py
--rw-r--r--   0        0        0      301 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/0003_delete_captcha.py
--rw-r--r--   0        0        0     1062 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/0004_captcha.py
--rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/models.py
--rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/py.typed
--rw-r--r--   0        0        0      649 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/settings.py
--rw-r--r--   0        0        0     9825 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/settings_type.py
--rw-r--r--   0        0        0      171 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/templates/email/activation_email.html
--rw-r--r--   0        0        0       41 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/templates/email/activation_subject.txt
--rw-r--r--   0        0        0   176202 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
--rw-r--r--   0        0        0   100933 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
--rw-r--r--   0        0        0      162 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/password_reset_email.html
--rw-r--r--   0        0        0       39 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/password_reset_subject.txt
--rw-r--r--   0        0        0      160 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/password_set_email.html
--rw-r--r--   0        0        0       37 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/password_set_subject.txt
--rw-r--r--   0        0        0        0 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/__init__.py
--rw-r--r--   0        0        0     2177 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/arg_mutations.py
--rw-r--r--   0        0        0     1628 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/forms.py
--rw-r--r--   0        0        0     1281 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/helpers.py
--rw-r--r--   0        0        0     1111 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/queries.py
--rw-r--r--   0        0        0     2277 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/relay.py
--rw-r--r--   0        0        0    19506 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/resolvers.py
--rw-r--r--   0        0        0      450 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/signals.py
--rw-r--r--   0        0        0     2005 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/types_.py
--rw-r--r--   0        0        0      119 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/views.py
--rw-r--r--   0        0        0     3205 2023-07-10 04:00:56.620680 strawberry_django_auth-0.375.0/pyproject.toml
--rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 strawberry_django_auth-0.375.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-08-07 11:12:40.533162 strawberry_django_auth-0.376.0/LICENSE
+-rw-r--r--   0        0        0     3820 2023-08-07 11:12:40.533162 strawberry_django_auth-0.376.0/README.md
+-rw-r--r--   0        0        0       24 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/__init__.py
+-rw-r--r--   0        0        0      168 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/admin.py
+-rw-r--r--   0        0        0      215 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/apps.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/captcha/__init__.py
+-rw-r--r--   0        0        0     1267 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/captcha/captcha_factorty.py
+-rw-r--r--   0        0        0     6606 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/captcha/create.py
+-rw-r--r--   0        0        0    16724 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/captcha/fonts/Nehama.ttf
+-rw-r--r--   0        0        0   221328 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
+-rw-r--r--   0        0        0    45448 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/captcha/fonts/pltwide.ttf
+-rwxr-xr-x   0        0        0    22768 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/captcha/fonts/stam.ttf
+-rw-r--r--   0        0        0     3413 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/captcha/models.py
+-rw-r--r--   0        0        0      549 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/captcha/types_.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/__init__.py
+-rw-r--r--   0        0        0     1995 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/constants.py
+-rw-r--r--   0        0        0      910 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/directives.py
+-rw-r--r--   0        0        0     1093 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/exceptions.py
+-rw-r--r--   0        0        0      231 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/interfaces.py
+-rw-r--r--   0        0        0     3972 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/middlewares.py
+-rw-r--r--   0        0        0     1453 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/mixins.py
+-rw-r--r--   0        0        0     1516 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/scalars.py
+-rw-r--r--   0        0        0      857 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/types_.py
+-rw-r--r--   0        0        0     4062 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/core/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/jwt/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/jwt/tools.py
+-rw-r--r--   0        0        0     7646 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/jwt/types_.py
+-rw-r--r--   0        0        0     7328 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/models.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/py.typed
+-rw-r--r--   0        0        0      649 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/settings.py
+-rw-r--r--   0        0        0     9825 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/settings_type.py
+-rw-r--r--   0        0        0      171 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/templates/email/activation_email.html
+-rw-r--r--   0        0        0       41 2023-08-07 11:12:40.585162 strawberry_django_auth-0.376.0/gqlauth/templates/email/activation_subject.txt
+-rw-r--r--   0        0        0   176202 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
+-rw-r--r--   0        0        0   100933 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
+-rw-r--r--   0        0        0      162 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/templates/email/password_reset_email.html
+-rw-r--r--   0        0        0       39 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/templates/email/password_reset_subject.txt
+-rw-r--r--   0        0        0      160 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/templates/email/password_set_email.html
+-rw-r--r--   0        0        0       37 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/templates/email/password_set_subject.txt
+-rw-r--r--   0        0        0        0 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/__init__.py
+-rw-r--r--   0        0        0     2177 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/arg_mutations.py
+-rw-r--r--   0        0        0     1628 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/forms.py
+-rw-r--r--   0        0        0     1281 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/helpers.py
+-rw-r--r--   0        0        0     1111 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/queries.py
+-rw-r--r--   0        0        0     2277 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/relay.py
+-rw-r--r--   0        0        0    19506 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/resolvers.py
+-rw-r--r--   0        0        0      450 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/signals.py
+-rw-r--r--   0        0        0     2005 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/types_.py
+-rw-r--r--   0        0        0      119 2023-08-07 11:12:40.589161 strawberry_django_auth-0.376.0/gqlauth/user/views.py
+-rw-r--r--   0        0        0     3239 2023-08-07 11:13:04.301081 strawberry_django_auth-0.376.0/pyproject.toml
+-rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 strawberry_django_auth-0.376.0/PKG-INFO
```

### Comparing `strawberry_django_auth-0.375.0/LICENSE` & `strawberry_django_auth-0.376.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/README.md` & `strawberry_django_auth-0.376.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/captcha/captcha_factorty.py` & `strawberry_django_auth-0.376.0/gqlauth/captcha/captcha_factorty.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/captcha/create.py` & `strawberry_django_auth-0.376.0/gqlauth/captcha/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,16 @@
         return image
 
     def create_captcha_image(self, chars, color, background):
         """Create the CAPTCHA image itself.
 
         :param chars: text to be generated.
         :param color: color of the text.
-        :param background: color of the background.         The color
-                should be a tuple of 3 numbers, such as (0, 255, 255).
+        :param background: color of the background. The color should be
+            a tuple of 3 numbers, such as (0, 255, 255).
         """
         image = Image.new("RGB", (self._width, self._height), background)
         draw = Draw(image)
 
         def _draw_character(c):
             # if hebrew
             direction = "ltr"
```

### Comparing `strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/Nehama.ttf` & `strawberry_django_auth-0.376.0/gqlauth/captcha/fonts/Nehama.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/OpenSans-Semibold.ttf` & `strawberry_django_auth-0.376.0/gqlauth/captcha/fonts/OpenSans-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/pltwide.ttf` & `strawberry_django_auth-0.376.0/gqlauth/captcha/fonts/pltwide.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/stam.ttf` & `strawberry_django_auth-0.376.0/gqlauth/captcha/fonts/stam.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/captcha/models.py` & `strawberry_django_auth-0.376.0/gqlauth/captcha/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,37 @@
+import importlib.util
 import io
 import uuid
 
 from django.db import models
 from django.utils import timezone
 
 from gqlauth.captcha.captcha_factorty import CaptchaInstanceType, generate_captcha_text
 from gqlauth.core.constants import Messages
 from gqlauth.settings import gqlauth_settings as app_settings
 
+PILLOW_INSTALLED = False
+if importlib.util.find_spec("PIL"):
+    PILLOW_INSTALLED = True
+
 
 class Captcha(models.Model):
     instance: CaptchaInstanceType
     uuid = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     text = models.CharField(max_length=50, editable=False)
     insert_time = models.DateTimeField(auto_now_add=True, editable=False)
     tries = models.IntegerField(default=0)
-    image = models.ImageField(
-        blank=False,
-        null=False,
-        upload_to="captcha/%Y/%m/%d/",
-        editable=False,
-        help_text="url for the captcha image",
-    )
+    if PILLOW_INSTALLED:
+        image = models.ImageField(
+            blank=False,
+            null=False,
+            upload_to="captcha/%Y/%m/%d/",
+            editable=False,
+            help_text="url for the captcha image",
+        )
 
     @staticmethod
     def _format(text: str):
         return text.lower().replace(" ", "")
 
     @classmethod
     def create_captcha(cls):
```

### Comparing `strawberry_django_auth-0.375.0/gqlauth/core/constants.py` & `strawberry_django_auth-0.376.0/gqlauth/core/constants.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/core/directives.py` & `strawberry_django_auth-0.376.0/gqlauth/core/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/core/exceptions.py` & `strawberry_django_auth-0.376.0/gqlauth/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/core/middlewares.py` & `strawberry_django_auth-0.376.0/gqlauth/core/middlewares.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
+
 import asyncio
-from typing import TYPE_CHECKING, Callable, Optional, Union
+from typing import TYPE_CHECKING, Callable
 
 from asgiref.sync import sync_to_async
-from django.contrib.auth import login
 from django.contrib.auth.models import AnonymousUser
 from django.http import HttpRequest
 from django.utils.decorators import sync_and_async_middleware
 from strawberry import Schema
 
 from gqlauth.core.exceptions import TokenExpired
 from gqlauth.core.types_ import GQLAuthError, GQLAuthErrors
@@ -18,81 +19,65 @@
 if TYPE_CHECKING:
     pass
 
 
 class UserOrError:
     __slots__ = ("user", "error")
 
-    def __init__(self, user: USER_UNION = anon_user, error: Optional[Exception] = None):
+    def __init__(self, user: USER_UNION = anon_user, error: Exception | None = None):
         self.user = user
         self.error = error
 
-    def authorized_user(self) -> Optional[USER_UNION]:
-        if self.user.is_authenticated:  # real django user model always returns true.
-            return self.user
-        return None
-
 
 USER_OR_ERROR_KEY = UserOrError.__name__
 
 
-def get_user_or_error(scope_or_request: Union[dict, HttpRequest]) -> UserOrError:
+def get_user_or_error(scope_or_request: dict | HttpRequest) -> UserOrError:
     user_or_error = UserOrError()
     if token_str := app_settings.JWT_TOKEN_FINDER(scope_or_request):
         try:
             token = TokenType.from_token(token=token_str)
             user = token.get_user_instance()
             user_or_error.user = user
 
         except PyJWTError:  # raised by python-jwt
             user_or_error.error = GQLAuthError(code=GQLAuthErrors.INVALID_TOKEN)
 
         except TokenExpired:
             user_or_error.error = GQLAuthError(code=GQLAuthErrors.EXPIRED_TOKEN)
-        except Exception as exc:  # pragma: no cover
-            import traceback
 
-            traceback.print_tb(exc.__traceback__)
-            print(exc)
-            raise exc
     else:
         user_or_error.error = GQLAuthError(code=GQLAuthErrors.MISSING_TOKEN)
 
     return user_or_error
 
 
 def channels_jwt_middleware(inner: Callable):
-    from channels.auth import (
-        login as channels_login,  # deferred import for users that don't use channels.
-    )
+    from channels.db import database_sync_to_async
 
     if asyncio.iscoroutinefunction(inner):
-        get_user_or_error_async = sync_to_async(get_user_or_error)
+        get_user_or_error_async = database_sync_to_async(get_user_or_error)
 
         async def middleware(scope, receive, send):
             if not scope.get(USER_OR_ERROR_KEY, None):
                 user_or_error: UserOrError = await get_user_or_error_async(scope)
                 scope[USER_OR_ERROR_KEY] = user_or_error
-                if user := user_or_error.authorized_user():
-                    await channels_login(scope, user)
             return await inner(scope, receive, send)
 
     else:  # pragma: no cover
         raise NotImplementedError("sync channels middleware is not supported yet.")
     return middleware
 
 
 @sync_and_async_middleware
 def django_jwt_middleware(get_response):
     def logic(request: HttpRequest) -> None:
         if not hasattr(request, USER_OR_ERROR_KEY):
             user_or_error: UserOrError = get_user_or_error(request)
             setattr(request, USER_OR_ERROR_KEY, user_or_error)
-            if user := user_or_error.authorized_user():
-                login(request, user)  # type: ignore
 
     if asyncio.iscoroutinefunction(get_response):
         async_logic = sync_to_async(logic)
 
         async def middleware(request: HttpRequest):
             await async_logic(request)
             return await get_response(request)
@@ -113,18 +98,17 @@
         self._inject_user_and_errors(kwargs)
         return super().execute_sync(*args, **kwargs)
 
     async def execute(self, *args, **kwargs):
         self._inject_user_and_errors(kwargs)
         return await super().execute(*args, **kwargs)
 
-    def subscribe(self, *args, **kwargs):
+    async def subscribe(self, *args, **kwargs):
         self._inject_user_and_errors(kwargs)
-        res = super().subscribe(*args, **kwargs)
-        return res
+        return await super().subscribe(*args, **kwargs)
 
     @staticmethod
     def _inject_user_and_errors(kwargs: dict) -> UserOrError:
         context = kwargs.get("context_value")
         # channels compat
         if isinstance(context, dict):
             request = context["request"]
```

### Comparing `strawberry_django_auth-0.375.0/gqlauth/core/mixins.py` & `strawberry_django_auth-0.376.0/gqlauth/core/mixins.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/core/scalars.py` & `strawberry_django_auth-0.376.0/gqlauth/core/scalars.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/core/types_.py` & `strawberry_django_auth-0.376.0/gqlauth/core/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/core/utils.py` & `strawberry_django_auth-0.376.0/gqlauth/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
     return wrapped
 
 
 def inject_arguments(args: Dict[str, type]):
     """Injects arguments to the decorated resolver.
 
-    :param args: `dict[name, type]` of arguments to be injected.,
+    :param args:`dict[name, type]` of arguments to be injected.,
     """
 
     def wrapped(fn):
         sig = inspect.signature(fn)
         params = {
             inspect.Parameter(name, inspect.Parameter.POSITIONAL_OR_KEYWORD, annotation=type_)
             for name, type_ in args.items()
```

### Comparing `strawberry_django_auth-0.375.0/gqlauth/jwt/types_.py` & `strawberry_django_auth-0.376.0/gqlauth/jwt/types_.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, Optional, cast
 from uuid import UUID
 
 import strawberry
 import strawberry_django
 from django.contrib.auth import authenticate
 from django.core.exceptions import PermissionDenied
+from django.utils.timezone import localtime
 from strawberry import auto
 from strawberry.types import Info
 
 from gqlauth.core.constants import Messages
 from gqlauth.core.exceptions import TokenExpired
 from gqlauth.core.interfaces import OutputInterface
 from gqlauth.core.scalars import ExpectedErrorType
@@ -166,22 +167,25 @@
             "password": input_.password,
         }
         try:
             # authenticate against django authentication backends.
             user: Optional["UserProto"]
             if not (user := authenticate(info.context.request, **args)):  # type: ignore
                 return ObtainJSONWebTokenType(success=False, errors=Messages.INVALID_CREDENTIALS)
+
             from gqlauth.models import UserStatus
 
             status: UserStatus = getattr(user, "status")  # noqa: B009
             # gqlauth logic
             if status.archived is True:  # un-archive on login
                 UserStatus.unarchive(user)
             if status.verified or app_settings.ALLOW_LOGIN_NOT_VERIFIED:
                 # successful login.
+                user.last_login = localtime()
+                user.save(update_fields=("last_login",))
                 return ObtainJSONWebTokenType.from_user(user)
             else:
                 return ObtainJSONWebTokenType(success=False, errors=Messages.NOT_VERIFIED)
 
         except PermissionDenied:
             # one of the authentication backends rejected the user.
             return ObtainJSONWebTokenType(success=False, errors=Messages.UNAUTHENTICATED)
```

### Comparing `strawberry_django_auth-0.375.0/gqlauth/models.py` & `strawberry_django_auth-0.376.0/gqlauth/models.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/settings.py` & `strawberry_django_auth-0.376.0/gqlauth/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/settings_type.py` & `strawberry_django_auth-0.376.0/gqlauth/settings_type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg` & `strawberry_django_auth-0.376.0/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg` & `strawberry_django_auth-0.376.0/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/user/arg_mutations.py` & `strawberry_django_auth-0.376.0/gqlauth/user/arg_mutations.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/user/forms.py` & `strawberry_django_auth-0.376.0/gqlauth/user/forms.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/user/helpers.py` & `strawberry_django_auth-0.376.0/gqlauth/user/helpers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/user/queries.py` & `strawberry_django_auth-0.376.0/gqlauth/user/queries.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/user/relay.py` & `strawberry_django_auth-0.376.0/gqlauth/user/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/user/resolvers.py` & `strawberry_django_auth-0.376.0/gqlauth/user/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/gqlauth/user/types_.py` & `strawberry_django_auth-0.376.0/gqlauth/user/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.375.0/pyproject.toml` & `strawberry_django_auth-0.376.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-auth"
-version = "0.375.0"
+version = "0.376.0"
 description = "Graphql authentication system with Strawberry for Django."
 license = "MIT"
 authors = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 readme = "README.md"
 classifiers = [
     'Environment :: Web Environment',
@@ -23,26 +23,27 @@
     { include = "gqlauth" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 Django = ">=3.2,<4.3"
 PyJWT = ">=2.6.0,<3.0"
-pillow = {version = "^9.5.0", extras = ["captcha"]}
+pillow = {version = ">=9.5,<11.0", extras = ["captcha"]}
 django-stubs = {extras = ["compatible-mypy"], version = "^4.2.0"}
 strawberry-graphql-django = ">=0.10.5"
 
 [tool.poetry.extras]
 captcha = ["pillow"]
 
-[tool.poetry.dev-dependencies]
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.3.3"
 coverage = "^7.2"
 pytest = "^7.2"
 pytest-cov = "^4.0"
-pytest-django = "^4.0.0"
 types-cryptography = "^3.3.23"
 django-mock-queries = "^2.1.7"
 types-mock = "^5.0.0"
 types-jwt = "^0.1.0"
 types-pkg-resources = "^0.1.0"
 mkdocs = ">=1.3.0"
 mkdocs-markdownextradata-plugin = ">=0.2.5"
@@ -51,14 +52,15 @@
 pymdown-extensions = ">=9.9"
 Markdown = ">=3.4.1"
 Faker = ">=18.2.0"
 pytest-asyncio = ">=0.21.0"
 pydoc-markdown = {extras = ["novella"], version = ">=4.6.4"}
 setuptools = ">=67.6.0"
 channels = {extras = ["daphne"], version = ">=4.0.0"}
+pytest-django = "^4.5.2"
 
 
 [tool.pytest.ini_options]
 django_find_project = false
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
```

### Comparing `strawberry_django_auth-0.375.0/PKG-INFO` & `strawberry_django_auth-0.376.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-auth
-Version: 0.375.0
+Version: 0.376.0
 Summary: Graphql authentication system with Strawberry for Django.
 License: MIT
 Author: Nir.J Benlulu
 Author-email: nrbnlulu@gmail.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: captcha
 Requires-Dist: Django (>=3.2,<4.3)
 Requires-Dist: PyJWT (>=2.6.0,<3.0)
 Requires-Dist: django-stubs[compatible-mypy] (>=4.2.0,<5.0.0)
-Requires-Dist: pillow[captcha] (>=9.5.0,<10.0.0) ; extra == "captcha"
+Requires-Dist: pillow[captcha] (>=9.5,<11.0) ; extra == "captcha"
 Requires-Dist: strawberry-graphql-django (>=0.10.5)
 Project-URL: Documentation, https://nrbnlulu.github.io/strawberry-django-auth/
 Project-URL: Homepage, https://github.com/nrbnlulu/strawberry-django-auth
 Description-Content-Type: text/markdown
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/nrbnlulu/strawberry-django-auth/tests.yml?label=Tests&style=for-the-badge)](https://github.com/nrbnlulu/strawberry-django-auth/actions/workflows/tests.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/nrbnlulu/strawberry-django-auth?style=for-the-badge)](https://app.codecov.io/gh/nrbnlulu/strawberry-django-auth)
```

