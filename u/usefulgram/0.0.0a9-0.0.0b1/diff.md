# Comparing `tmp/usefulgram-0.0.0a9.tar.gz` & `tmp/usefulgram-0.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usefulgram-0.0.0a9.tar", max compression
+gzip compressed data, was "usefulgram-0.0.0b1.tar", max compression
```

## Comparing `usefulgram-0.0.0a9.tar` & `usefulgram-0.0.0b1.tar`

### file list

```diff
@@ -1,27 +1,35 @@
--rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a9/LICENSE
--rw-r--r--   0        0        0      751 2023-07-27 03:00:09.647123 usefulgram-0.0.0a9/pyproject.toml
--rw-r--r--   0        0        0     3053 2023-07-21 00:40:55.695271 usefulgram-0.0.0a9/README.md
--rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a9/usefulgram/__init__.py
--rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a9/usefulgram/enums/__init__.py
--rw-r--r--   0        0        0      289 2023-07-20 23:58:44.461878 usefulgram-0.0.0a9/usefulgram/enums/const.py
--rw-r--r--   0        0        0      309 2023-07-20 23:10:48.507629 usefulgram-0.0.0a9/usefulgram/exceptions/__init__.py
--rw-r--r--   0        0        0      869 2023-07-20 23:10:48.511619 usefulgram-0.0.0a9/usefulgram/exceptions/exceptions.py
--rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a9/usefulgram/filters/__init__.py
--rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a9/usefulgram/filters/database_filters.py
--rw-r--r--   0        0        0     6685 2023-07-26 18:02:46.375010 usefulgram-0.0.0a9/usefulgram/filters/parse_filters.py
--rw-r--r--   0        0        0      123 2023-07-20 20:45:03.943904 usefulgram-0.0.0a9/usefulgram/keyboard/__init__.py
--rw-r--r--   0        0        0     3673 2023-07-27 00:54:59.805545 usefulgram-0.0.0a9/usefulgram/keyboard/builder.py
--rw-r--r--   0        0        0     2761 2023-07-20 20:15:49.534299 usefulgram-0.0.0a9/usefulgram/keyboard/buttons.py
--rw-r--r--   0        0        0      515 2023-07-20 20:15:49.549286 usefulgram-0.0.0a9/usefulgram/keyboard/rows.py
--rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a9/usefulgram/lazy/__init__.py
--rw-r--r--   0        0        0     2048 2023-07-27 02:58:17.509549 usefulgram-0.0.0a9/usefulgram/lazy/editor.py
--rw-r--r--   0        0        0     8253 2023-07-27 02:54:10.225180 usefulgram-0.0.0a9/usefulgram/lazy/lazy_editing.py
--rw-r--r--   0        0        0     1756 2023-07-27 02:54:10.216965 usefulgram-0.0.0a9/usefulgram/lazy/sender.py
--rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a9/usefulgram/middlewares/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-20 23:55:38.146961 usefulgram-0.0.0a9/usefulgram/middlewares/stacker.py
--rw-r--r--   0        0        0     1510 2023-07-19 23:25:39.503139 usefulgram-0.0.0a9/usefulgram/middlewares/trottling.py
--rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a9/usefulgram/parsing/__init__.py
--rw-r--r--   0        0        0     3946 2023-07-20 21:32:27.645449 usefulgram-0.0.0a9/usefulgram/parsing/decode.py
--rw-r--r--   0        0        0     2774 2023-07-19 21:09:49.679939 usefulgram-0.0.0a9/usefulgram/parsing/encode.py
--rw-r--r--   0        0        0        0 2023-07-27 00:03:27.735654 usefulgram-0.0.0a9/usefulgram/utils/__init__.py
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 usefulgram-0.0.0a9/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0b1/LICENSE
+-rw-r--r--   0        0        0      735 2023-08-07 00:40:11.266535 usefulgram-0.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2171 2023-08-07 01:10:02.999992 usefulgram-0.0.0b1/README.md
+-rw-r--r--   0        0        0      249 2023-07-31 22:39:48.937877 usefulgram-0.0.0b1/usefulgram/__init__.py
+-rw-r--r--   0        0        0       66 2023-08-06 23:33:56.315513 usefulgram-0.0.0b1/usefulgram/enums/__init__.py
+-rw-r--r--   0        0        0      123 2023-08-06 23:27:18.165995 usefulgram-0.0.0b1/usefulgram/enums/calendar.py
+-rw-r--r--   0        0        0      298 2023-07-28 15:07:37.521185 usefulgram-0.0.0b1/usefulgram/enums/const.py
+-rw-r--r--   0        0        0      329 2023-08-04 23:48:29.696770 usefulgram-0.0.0b1/usefulgram/exceptions/__init__.py
+-rw-r--r--   0        0        0      916 2023-08-04 23:48:29.684803 usefulgram-0.0.0b1/usefulgram/exceptions/exceptions.py
+-rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0b1/usefulgram/filters/__init__.py
+-rw-r--r--   0        0        0      790 2023-07-29 00:59:10.296938 usefulgram-0.0.0b1/usefulgram/filters/database_filters.py
+-rw-r--r--   0        0        0     6695 2023-08-06 23:41:38.396437 usefulgram-0.0.0b1/usefulgram/filters/parse_filters.py
+-rw-r--r--   0        0        0      123 2023-07-20 20:45:03.943904 usefulgram-0.0.0b1/usefulgram/keyboard/__init__.py
+-rw-r--r--   0        0        0     3673 2023-07-27 00:54:59.805545 usefulgram-0.0.0b1/usefulgram/keyboard/builder.py
+-rw-r--r--   0        0        0     2759 2023-08-06 23:16:09.572525 usefulgram-0.0.0b1/usefulgram/keyboard/buttons.py
+-rw-r--r--   0        0        0      515 2023-07-20 20:15:49.549286 usefulgram-0.0.0b1/usefulgram/keyboard/rows.py
+-rw-r--r--   0        0        0       78 2023-08-04 23:48:29.714723 usefulgram-0.0.0b1/usefulgram/lazy/__init__.py
+-rw-r--r--   0        0        0      712 2023-08-07 00:32:20.905500 usefulgram-0.0.0b1/usefulgram/lazy/callback_responder.py
+-rw-r--r--   0        0        0     2048 2023-07-27 02:58:17.509549 usefulgram-0.0.0b1/usefulgram/lazy/editor.py
+-rw-r--r--   0        0        0     7933 2023-08-07 00:32:20.901509 usefulgram-0.0.0b1/usefulgram/lazy/lazy_editor.py
+-rw-r--r--   0        0        0     3151 2023-08-07 00:34:36.019548 usefulgram-0.0.0b1/usefulgram/lazy/lazy_sender.py
+-rw-r--r--   0        0        0     1756 2023-07-27 02:54:10.216965 usefulgram-0.0.0b1/usefulgram/lazy/sender.py
+-rw-r--r--   0        0        0      721 2023-08-07 00:39:11.994259 usefulgram-0.0.0b1/usefulgram/lazy/stable_wait.py
+-rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0b1/usefulgram/middlewares/__init__.py
+-rw-r--r--   0        0        0     1986 2023-08-05 21:28:19.261207 usefulgram-0.0.0b1/usefulgram/middlewares/stacker.py
+-rw-r--r--   0        0        0     1510 2023-07-19 23:25:39.503139 usefulgram-0.0.0b1/usefulgram/middlewares/trottling.py
+-rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0b1/usefulgram/parsing/__init__.py
+-rw-r--r--   0        0        0     6496 2023-08-06 23:51:11.465659 usefulgram-0.0.0b1/usefulgram/parsing/decode.py
+-rw-r--r--   0        0        0     2921 2023-08-06 00:36:41.188176 usefulgram-0.0.0b1/usefulgram/parsing/encode.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:03:27.735654 usefulgram-0.0.0b1/usefulgram/utils/__init__.py
+-rw-r--r--   0        0        0      205 2023-08-05 23:26:20.689682 usefulgram-0.0.0b1/usefulgram/utils/calendar_manager/__init__.py
+-rw-r--r--   0        0        0      559 2023-08-06 23:33:56.309528 usefulgram-0.0.0b1/usefulgram/utils/calendar_manager/filters.py
+-rw-r--r--   0        0        0      389 2023-08-07 01:00:37.460047 usefulgram-0.0.0b1/usefulgram/utils/calendar_manager/model.py
+-rw-r--r--   0        0        0     5759 2023-08-07 00:11:43.839463 usefulgram-0.0.0b1/usefulgram/utils/calendar_manager/views.py
+-rw-r--r--   0        0        0     2947 1970-01-01 00:00:00.000000 usefulgram-0.0.0b1/PKG-INFO
```

### Comparing `usefulgram-0.0.0a9/LICENSE` & `usefulgram-0.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a9/pyproject.toml` & `usefulgram-0.0.0b1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "usefulgram"
-version = "0.0.0a9"
+version = "0.0.0b1"
 description = "Like aiogram but more easy"
 license = "MIT"
 authors = ["Alexandr Bortnik <sambonsttt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/Sethis/usefulgram"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aiogram = "^3.0.0b8"
+aiogram = "^3.0.0rc1"
 cachetools ="^4.0.0"
-pydantic ="^2.0.0"
-pytz ="^2020.3"
+pydantic ="^2.1.0"
 
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Sethis/usefulgram/issues"
```

### Comparing `usefulgram-0.0.0a9/usefulgram/exceptions/exceptions.py` & `usefulgram-0.0.0b1/usefulgram/exceptions/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 NoOneButtonParamIsFilled = ValueError("No one button parameters is filled")
 
 DifferentButtonsInMatrix = ValueError("Only one type of button is allowed in the markup")
 
 UnknownButtonType = ValueError("UnknownButtonType")
 
-TooMoreCharacters = ValueError("The callback data can be only 64 bytes"
-                               "(~62 or less characters because separator)")
+TooMoreCharacters = ValueError(
+    "The callback data can be only 64 bytes"
+    "(~62 or less characters because separator)"
+)
 
 RecursionObjectParse = ValueError("Now objects cannot contain objects")
 
 WrongObjectType = ValueError("Wrong object type in the decode")
 
 CantEditMedia = ValueError("Error for edit message media")
 
 BotIsUndefined = ValueError("Bot is not defined in StakerMiddleware")
 
 MessageTooOld = ValueError("Message too old and has not message param")
 
 MessageTextIsNone = ValueError("Message text is None")
 
 UndefinedMagicFilterModel = ValueError("Magic filter model is undefined")
+
+UndefinedType = ValueError("Error event type in a middleware")
```

### Comparing `usefulgram-0.0.0a9/usefulgram/filters/database_filters.py` & `usefulgram-0.0.0b1/usefulgram/filters/database_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     _data: Dict[str, Any]
 
     def __init__(self, prefix: str, **kwargs):
         self._prefix = prefix
         self._data = kwargs
 
     async def __call__(self, _event: TelegramObject):
-        prefix = self.get_prefix(self._data)
+        prefix = await self.get_prefix(self._data)
 
         return prefix == self._prefix
 
     @abstractmethod
     async def get_prefix(self, data: Dict[str, Any]) -> str:
         """
         This method should be overridden
```

### Comparing `usefulgram-0.0.0a9/usefulgram/filters/parse_filters.py` & `usefulgram-0.0.0b1/usefulgram/filters/parse_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             decoder: DecodeCallbackData,
             fields_name: Iterable[str]
     ) -> Union[bool, Dict[str, Any]]:
 
         try:
             callback_data_model = decoder.to_format(type(self), add_prefix=True)
 
-        except (AttributeError, ValueError, IndexError):
+        except (AttributeError, ValueError, IndexError, KeyError):
             return False
 
         for item_name in fields_name:
             if item_name == "_magic_filter":
                 continue
 
             filter_value = self.__getattribute__(item_name)
```

### Comparing `usefulgram-0.0.0a9/usefulgram/keyboard/builder.py` & `usefulgram-0.0.0b1/usefulgram/keyboard/builder.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a9/usefulgram/keyboard/buttons.py` & `usefulgram-0.0.0b1/usefulgram/keyboard/buttons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 
-
 from typing import Optional, Any, Union
 
 from aiogram.types import (
     InlineKeyboardButton,
     KeyboardButton,
     WebAppInfo,
     KeyboardButtonRequestChat,
```

### Comparing `usefulgram-0.0.0a9/usefulgram/keyboard/rows.py` & `usefulgram-0.0.0b1/usefulgram/keyboard/rows.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a9/usefulgram/lazy/editor.py` & `usefulgram-0.0.0b1/usefulgram/lazy/editor.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a9/usefulgram/lazy/lazy_editing.py` & `usefulgram-0.0.0b1/usefulgram/lazy/lazy_editor.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,492 +25,472 @@
 00000180: 6e73 2069 6d70 6f72 7420 4d65 7373 6167  ns import Messag
 00000190: 6554 6f6f 4f6c 640d 0a66 726f 6d20 7573  eTooOld..from us
 000001a0: 6566 756c 6772 616d 2e6c 617a 792e 6564  efulgram.lazy.ed
 000001b0: 6974 6f72 2069 6d70 6f72 7420 4d65 7373  itor import Mess
 000001c0: 6167 6545 6469 746f 720d 0a66 726f 6d20  ageEditor..from 
 000001d0: 7573 6566 756c 6772 616d 2e6c 617a 792e  usefulgram.lazy.
 000001e0: 7365 6e64 6572 2069 6d70 6f72 7420 4d65  sender import Me
-000001f0: 7373 6167 6553 656e 6465 720d 0a0d 0a0d  ssageSender.....
-00000200: 0a63 6c61 7373 204c 617a 7945 6469 7469  .class LazyEditi
-00000210: 6e67 3a0d 0a20 2020 2063 616c 6c62 6163  ng:..    callbac
-00000220: 6b3a 2043 616c 6c62 6163 6b51 7565 7279  k: CallbackQuery
-00000230: 0d0a 2020 2020 626f 743a 2042 6f74 0d0a  ..    bot: Bot..
-00000240: 2020 2020 7374 6162 6c65 3a20 626f 6f6c      stable: bool
-00000250: 0d0a 0d0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
-00000260: 6974 5f5f 2873 656c 662c 2063 616c 6c62  it__(self, callb
-00000270: 6163 6b3a 2043 616c 6c62 6163 6b51 7565  ack: CallbackQue
-00000280: 7279 2c20 626f 743a 2042 6f74 2c20 7374  ry, bot: Bot, st
-00000290: 6162 6c65 3a20 626f 6f6c 203d 2046 616c  able: bool = Fal
-000002a0: 7365 293a 0d0a 2020 2020 2020 2020 7365  se):..        se
-000002b0: 6c66 2e63 616c 6c62 6163 6b20 3d20 6361  lf.callback = ca
-000002c0: 6c6c 6261 636b 0d0a 2020 2020 2020 2020  llback..        
-000002d0: 7365 6c66 2e62 6f74 203d 2062 6f74 0d0a  self.bot = bot..
-000002e0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-000002f0: 626c 6520 3d20 7374 6162 6c65 0d0a 0d0a  ble = stable....
-00000300: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-00000310: 640d 0a20 2020 2064 6566 205f 6765 745f  d..    def _get_
-00000320: 7465 7874 5f62 795f 6361 7074 696f 6e28  text_by_caption(
-00000330: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
-00000340: 7874 3a20 4f70 7469 6f6e 616c 5b73 7472  xt: Optional[str
-00000350: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00000360: 6361 7074 696f 6e3a 204f 7074 696f 6e61  caption: Optiona
-00000370: 6c5b 7374 725d 0d0a 2020 2020 2920 2d3e  l[str]..    ) ->
-00000380: 204f 7074 696f 6e61 6c5b 7374 725d 3a0d   Optional[str]:.
-00000390: 0a0d 0a20 2020 2020 2020 2069 6620 7465  ...        if te
-000003a0: 7874 2069 7320 4e6f 6e65 206f 7220 6361  xt is None or ca
-000003b0: 7074 696f 6e20 6973 206e 6f74 204e 6f6e  ption is not Non
-000003c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000003d0: 7265 7475 726e 2063 6170 7469 6f6e 0d0a  return caption..
-000003e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000003f0: 2074 6578 740d 0a0d 0a20 2020 2040 7374   text....    @st
-00000400: 6174 6963 6d65 7468 6f64 0d0a 2020 2020  aticmethod..    
-00000410: 6465 6620 5f67 6574 5f6d 6573 7361 6765  def _get_message
-00000420: 5f74 6578 7428 7465 7874 3a20 4f70 7469  _text(text: Opti
-00000430: 6f6e 616c 5b73 7472 5d2c 206d 6573 7361  onal[str], messa
-00000440: 6765 3a20 4d65 7373 6167 6529 202d 3e20  ge: Message) -> 
-00000450: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0d0a  Optional[str]:..
-00000460: 2020 2020 2020 2020 6966 2074 6578 7420          if text 
-00000470: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00000480: 2020 2020 2020 7265 7475 726e 206d 6573        return mes
-00000490: 7361 6765 2e74 6578 740d 0a0d 0a20 2020  sage.text....   
-000004a0: 2020 2020 2072 6574 7572 6e20 7465 7874       return text
-000004b0: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-000004c0: 6574 686f 640d 0a20 2020 2064 6566 205f  ethod..    def _
-000004d0: 6765 745f 6461 7461 5f63 6861 6e67 6573  get_data_changes
-000004e0: 5f73 7461 7475 7328 0d0a 2020 2020 2020  _status(..      
-000004f0: 2020 2020 2020 6d65 7373 6167 653a 204d        message: M
-00000500: 6573 7361 6765 2c0d 0a20 2020 2020 2020  essage,..       
-00000510: 2020 2020 2074 6578 743a 204f 7074 696f       text: Optio
-00000520: 6e61 6c5b 7374 725d 2c0d 0a20 2020 2020  nal[str],..     
-00000530: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
-00000540: 6b75 703a 204f 7074 696f 6e61 6c5b 496e  kup: Optional[In
-00000550: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
-00000560: 7570 5d2c 0d0a 2020 2020 2020 2020 2020  up],..          
-00000570: 2020 7669 6465 6f3a 204f 7074 696f 6e61    video: Optiona
-00000580: 6c5b 4653 496e 7075 7446 696c 655d 2c0d  l[FSInputFile],.
-00000590: 0a20 2020 2020 2020 2020 2020 2070 686f  .            pho
-000005a0: 746f 3a20 4f70 7469 6f6e 616c 5b46 5349  to: Optional[FSI
-000005b0: 6e70 7574 4669 6c65 5d29 202d 3e20 626f  nputFile]) -> bo
-000005c0: 6f6c 3a0d 0a0d 0a20 2020 2020 2020 2069  ol:....        i
-000005d0: 6620 6d65 7373 6167 652e 7465 7874 2021  f message.text !
-000005e0: 3d20 7465 7874 3a0d 0a20 2020 2020 2020  = text:..       
-000005f0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00000600: 0d0a 0d0a 2020 2020 2020 2020 6966 206d  ....        if m
-00000610: 6573 7361 6765 2e72 6570 6c79 5f6d 6172  essage.reply_mar
-00000620: 6b75 7020 213d 2072 6570 6c79 5f6d 6172  kup != reply_mar
-00000630: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-00000640: 2020 7265 7475 726e 2054 7275 650d 0a0d    return True...
-00000650: 0a20 2020 2020 2020 2069 6620 6d65 7373  .        if mess
-00000660: 6167 652e 7669 6465 6f20 213d 2076 6964  age.video != vid
-00000670: 656f 3a0d 0a20 2020 2020 2020 2020 2020  eo:..           
-00000680: 2072 6574 7572 6e20 5472 7565 0d0a 0d0a   return True....
-00000690: 2020 2020 2020 2020 6966 206d 6573 7361          if messa
-000006a0: 6765 2e70 686f 746f 2021 3d20 7068 6f74  ge.photo != phot
-000006b0: 6f3a 0d0a 2020 2020 2020 2020 2020 2020  o:..            
-000006c0: 7265 7475 726e 2054 7275 650d 0a0d 0a20  return True.... 
-000006d0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000006e0: 6c73 650d 0a0d 0a20 2020 2040 7374 6174  lse....    @stat
-000006f0: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
-00000700: 6620 5f67 6574 5f74 696d 655f 6265 7477  f _get_time_betw
-00000710: 6565 6e5f 6375 7272 656e 745f 616e 645f  een_current_and_
-00000720: 6d65 7373 6167 6528 0d0a 2020 2020 2020  message(..      
-00000730: 2020 2020 2020 6d65 7373 6167 655f 6461        message_da
-00000740: 7465 3a20 6461 7465 7469 6d65 0d0a 2020  te: datetime..  
-00000750: 2020 2920 2d3e 2074 696d 6564 656c 7461    ) -> timedelta
-00000760: 3a0d 0a0d 0a20 2020 2020 2020 2063 7572  :....        cur
-00000770: 7265 6e74 203d 2064 6174 6574 696d 652e  rent = datetime.
-00000780: 6e6f 7728 747a 3d70 7974 7a2e 5554 4329  now(tz=pytz.UTC)
-00000790: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-000007a0: 726e 2063 7572 7265 6e74 202d 206d 6573  rn current - mes
-000007b0: 7361 6765 5f64 6174 650d 0a0d 0a20 2020  sage_date....   
-000007c0: 2040 7374 6174 6963 6d65 7468 6f64 0d0a   @staticmethod..
-000007d0: 2020 2020 6465 6620 5f67 6574 5f74 696d      def _get_tim
-000007e0: 655f 616c 6c6f 7765 645f 6564 6974 5f73  e_allowed_edit_s
-000007f0: 7461 7475 7328 6d65 7373 6167 653a 204d  tatus(message: M
-00000800: 6573 7361 6765 2920 2d3e 2062 6f6f 6c3a  essage) -> bool:
-00000810: 0d0a 2020 2020 2020 2020 636f 6e73 745f  ..        const_
-00000820: 6465 6c74 6120 3d20 7469 6d65 6465 6c74  delta = timedelt
-00000830: 6128 686f 7572 733d 436f 6e73 742e 414c  a(hours=Const.AL
-00000840: 4c4f 575f 4544 4954 494e 475f 4445 4c54  LOW_EDITING_DELT
-00000850: 4129 0d0a 0d0a 2020 2020 2020 2020 6465  A)....        de
-00000860: 6c74 6120 3d20 4c61 7a79 4564 6974 696e  lta = LazyEditin
-00000870: 672e 5f67 6574 5f74 696d 655f 6265 7477  g._get_time_betw
-00000880: 6565 6e5f 6375 7272 656e 745f 616e 645f  een_current_and_
-00000890: 6d65 7373 6167 6528 0d0a 2020 2020 2020  message(..      
-000008a0: 2020 2020 2020 6d65 7373 6167 652e 6461        message.da
-000008b0: 7465 0d0a 2020 2020 2020 2020 290d 0a0d  te..        )...
-000008c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000008d0: 6465 6c74 6120 3c20 636f 6e73 745f 6465  delta < const_de
-000008e0: 6c74 610d 0a0d 0a20 2020 2040 7374 6174  lta....    @stat
-000008f0: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
-00000900: 6620 5f67 6574 5f6d 6573 7361 6765 5f69  f _get_message_i
-00000910: 6e5f 6368 6174 5f73 7461 7475 7328 6d65  n_chat_status(me
-00000920: 7373 6167 653a 204d 6573 7361 6765 2920  ssage: Message) 
-00000930: 2d3e 2062 6f6f 6c3a 0d0a 2020 2020 2020  -> bool:..      
-00000940: 2020 6966 206d 6573 7361 6765 2e63 6861    if message.cha
-00000950: 742e 7479 7065 203d 3d20 4368 6174 5479  t.type == ChatTy
-00000960: 7065 2e43 4841 4e4e 454c 3a0d 0a20 2020  pe.CHANNEL:..   
-00000970: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000980: 5472 7565 0d0a 0d0a 2020 2020 2020 2020  True....        
-00000990: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
-000009a0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-000009b0: 640d 0a20 2020 2064 6566 205f 6765 745f  d..    def _get_
-000009c0: 6d65 7373 6167 655f 6d65 6469 615f 6973  message_media_is
-000009d0: 5f63 6f72 7265 6374 5f73 7461 7475 7328  _correct_status(
-000009e0: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
-000009f0: 7373 6167 653a 204d 6573 7361 6765 2c0d  ssage: Message,.
-00000a00: 0a20 2020 2020 2020 2020 2020 2070 686f  .            pho
-00000a10: 746f 3a20 4f70 7469 6f6e 616c 5b46 5349  to: Optional[FSI
-00000a20: 6e70 7574 4669 6c65 5d2c 0d0a 2020 2020  nputFile],..    
-00000a30: 2020 2020 2020 2020 7669 6465 6f3a 204f          video: O
-00000a40: 7074 696f 6e61 6c5b 4653 496e 7075 7446  ptional[FSInputF
-00000a50: 696c 655d 0d0a 2020 2020 2920 2d3e 2062  ile]..    ) -> b
-00000a60: 6f6f 6c3a 0d0a 0d0a 2020 2020 2020 2020  ool:....        
-00000a70: 6d65 7373 6167 655f 6861 735f 7068 6f74  message_has_phot
-00000a80: 6f5f 6f72 5f76 6964 656f 203d 206d 6573  o_or_video = mes
-00000a90: 7361 6765 2e70 686f 746f 206f 7220 6d65  sage.photo or me
-00000aa0: 7373 6167 652e 7669 6465 6f0d 0a0d 0a20  ssage.video.... 
-00000ab0: 2020 2020 2020 2069 6620 7068 6f74 6f20         if photo 
-00000ac0: 616e 6420 6e6f 7420 6d65 7373 6167 655f  and not message_
-00000ad0: 6861 735f 7068 6f74 6f5f 6f72 5f76 6964  has_photo_or_vid
-00000ae0: 656f 3a0d 0a20 2020 2020 2020 2020 2020  eo:..           
-00000af0: 2072 6574 7572 6e20 4661 6c73 650d 0a0d   return False...
-00000b00: 0a20 2020 2020 2020 2065 6c69 6620 7669  .        elif vi
-00000b10: 6465 6f20 616e 6420 6e6f 7420 6d65 7373  deo and not mess
-00000b20: 6167 655f 6861 735f 7068 6f74 6f5f 6f72  age_has_photo_or
-00000b30: 5f76 6964 656f 3a0d 0a20 2020 2020 2020  _video:..       
-00000b40: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00000b50: 650d 0a0d 0a20 2020 2020 2020 2072 6574  e....        ret
-00000b60: 7572 6e20 5472 7565 0d0a 0d0a 2020 2020  urn True....    
-00000b70: 6465 6620 5f67 6574 5f62 6f74 5f61 6c6c  def _get_bot_all
-00000b80: 6f77 5f65 6469 745f 7374 6174 7573 280d  ow_edit_status(.
-00000b90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00000ba0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
-00000bb0: 6d65 7373 6167 653a 204d 6573 7361 6765  message: Message
-00000bc0: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
-00000bd0: 686f 746f 3a20 4f70 7469 6f6e 616c 5b46  hoto: Optional[F
-00000be0: 5349 6e70 7574 4669 6c65 5d2c 0d0a 2020  SInputFile],..  
-00000bf0: 2020 2020 2020 2020 2020 7669 6465 6f3a            video:
-00000c00: 204f 7074 696f 6e61 6c5b 4653 496e 7075   Optional[FSInpu
-00000c10: 7446 696c 655d 2c0d 0a20 2020 2029 202d  tFile],..    ) -
-00000c20: 3e20 626f 6f6c 3a0d 0a0d 0a20 2020 2020  > bool:....     
-00000c30: 2020 2069 6620 7365 6c66 2e5f 6765 745f     if self._get_
-00000c40: 6d65 7373 6167 655f 696e 5f63 6861 745f  message_in_chat_
-00000c50: 7374 6174 7573 286d 6573 7361 6765 293a  status(message):
-00000c60: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000c70: 7475 726e 2054 7275 650d 0a0d 0a20 2020  turn True....   
-00000c80: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00000c90: 2e5f 6765 745f 7469 6d65 5f61 6c6c 6f77  ._get_time_allow
-00000ca0: 6564 5f65 6469 745f 7374 6174 7573 286d  ed_edit_status(m
-00000cb0: 6573 7361 6765 293a 0d0a 2020 2020 2020  essage):..      
-00000cc0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00000cd0: 7365 0d0a 0d0a 2020 2020 2020 2020 6966  se....        if
-00000ce0: 206e 6f74 2073 656c 662e 5f67 6574 5f6d   not self._get_m
-00000cf0: 6573 7361 6765 5f6d 6564 6961 5f69 735f  essage_media_is_
-00000d00: 636f 7272 6563 745f 7374 6174 7573 280d  correct_status(.
-00000d10: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-00000d20: 7361 6765 3d6d 6573 7361 6765 2c20 7068  sage=message, ph
-00000d30: 6f74 6f3d 7068 6f74 6f2c 2076 6964 656f  oto=photo, video
-00000d40: 3d76 6964 656f 0d0a 2020 2020 2020 2020  =video..        
-00000d50: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00000d60: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
-00000d70: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00000d80: 7275 650d 0a0d 0a20 2020 2040 7374 6174  rue....    @stat
-00000d90: 6963 6d65 7468 6f64 0d0a 2020 2020 6173  icmethod..    as
-00000da0: 796e 6320 6465 6620 5f61 7574 6f5f 6361  ync def _auto_ca
-00000db0: 6c6c 6261 636b 5f61 6e73 7765 7228 0d0a  llback_answer(..
-00000dc0: 2020 2020 2020 2020 2020 2020 626f 743a              bot:
-00000dd0: 2042 6f74 2c0d 0a20 2020 2020 2020 2020   Bot,..         
-00000de0: 2020 2063 616c 6c62 6163 6b5f 6964 3a20     callback_id: 
-00000df0: 7374 722c 0d0a 2020 2020 2020 2020 2020  str,..          
-00000e00: 2020 6175 746f 616e 7377 6572 3a20 626f    autoanswer: bo
-00000e10: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
-00000e20: 2020 2020 2020 2020 616e 7377 6572 5f74          answer_t
-00000e30: 6578 743a 204f 7074 696f 6e61 6c5b 7374  ext: Optional[st
-00000e40: 725d 203d 204e 6f6e 652c 0d0a 2020 2020  r] = None,..    
-00000e50: 2020 2020 2020 2020 616e 7377 6572 5f73          answer_s
-00000e60: 686f 775f 616c 6572 743a 2062 6f6f 6c20  how_alert: bool 
-00000e70: 3d20 4661 6c73 650d 0a20 2020 2029 202d  = False..    ) -
-00000e80: 3e20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  > Optional[bool]
-00000e90: 3a0d 0a0d 0a20 2020 2020 2020 2069 6620  :....        if 
-00000ea0: 6e6f 7420 6175 746f 616e 7377 6572 3a0d  not autoanswer:.
-00000eb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00000ec0: 7572 6e20 4e6f 6e65 0d0a 0d0a 2020 2020  urn None....    
-00000ed0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00000ee0: 2062 6f74 2e61 6e73 7765 725f 6361 6c6c   bot.answer_call
-00000ef0: 6261 636b 5f71 7565 7279 280d 0a20 2020  back_query(..   
-00000f00: 2020 2020 2020 2020 2063 616c 6c62 6163           callbac
-00000f10: 6b5f 7175 6572 795f 6964 3d63 616c 6c62  k_query_id=callb
-00000f20: 6163 6b5f 6964 2c0d 0a20 2020 2020 2020  ack_id,..       
-00000f30: 2020 2020 2074 6578 743d 616e 7377 6572       text=answer
-00000f40: 5f74 6578 742c 0d0a 2020 2020 2020 2020  _text,..        
-00000f50: 2020 2020 7368 6f77 5f61 6c65 7274 3d61      show_alert=a
-00000f60: 6e73 7765 725f 7368 6f77 5f61 6c65 7274  nswer_show_alert
-00000f70: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
-00000f80: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00000f90: 0d0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00000fa0: 5f73 656e 645f 6f72 5f65 6469 7428 0d0a  _send_or_edit(..
-00000fb0: 2020 2020 2020 2020 2020 2020 626f 743a              bot:
-00000fc0: 2042 6f74 2c0d 0a20 2020 2020 2020 2020   Bot,..         
-00000fd0: 2020 2063 616e 5f65 6469 743a 2062 6f6f     can_edit: boo
-00000fe0: 6c2c 0d0a 2020 2020 2020 2020 2020 2020  l,..            
-00000ff0: 6d65 7373 6167 653a 204d 6573 7361 6765  message: Message
-00001000: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-00001010: 6578 743a 204f 7074 696f 6e61 6c5b 7374  ext: Optional[st
-00001020: 725d 2c0d 0a20 2020 2020 2020 2020 2020  r],..           
-00001030: 2070 686f 746f 3a20 4f70 7469 6f6e 616c   photo: Optional
-00001040: 5b46 5349 6e70 7574 4669 6c65 5d2c 0d0a  [FSInputFile],..
-00001050: 2020 2020 2020 2020 2020 2020 7669 6465              vide
-00001060: 6f3a 204f 7074 696f 6e61 6c5b 4653 496e  o: Optional[FSIn
-00001070: 7075 7446 696c 655d 2c0d 0a20 2020 2020  putFile],..     
-00001080: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
-00001090: 6b75 703a 204f 7074 696f 6e61 6c5b 496e  kup: Optional[In
-000010a0: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
-000010b0: 7570 5d2c 0d0a 2020 2020 2020 2020 2020  up],..          
-000010c0: 2020 7061 7273 655f 6d6f 6465 3a20 556e    parse_mode: Un
-000010d0: 696f 6e5b 7374 725d 2c0d 0a20 2020 2020  ion[str],..     
-000010e0: 2020 2020 2020 2064 6973 6162 6c65 5f77         disable_w
-000010f0: 6562 5f70 6167 655f 7072 6576 6965 773a  eb_page_preview:
-00001100: 2062 6f6f 6c2c 0d0a 2020 2020 2920 2d3e   bool,..    ) ->
-00001110: 2055 6e69 6f6e 5b4d 6573 7361 6765 2c20   Union[Message, 
-00001120: 626f 6f6c 5d3a 0d0a 0d0a 2020 2020 2020  bool]:....      
-00001130: 2020 6966 206e 6f74 2063 616e 5f65 6469    if not can_edi
-00001140: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00001150: 7465 7874 203d 204c 617a 7945 6469 7469  text = LazyEditi
-00001160: 6e67 2e5f 6765 745f 6d65 7373 6167 655f  ng._get_message_
-00001170: 7465 7874 2874 6578 742c 206d 6573 7361  text(text, messa
-00001180: 6765 3d6d 6573 7361 6765 290d 0a0d 0a20  ge=message).... 
-00001190: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000011a0: 6e20 6177 6169 7420 4d65 7373 6167 6553  n await MessageS
-000011b0: 656e 6465 722e 7365 6e64 280d 0a20 2020  ender.send(..   
-000011c0: 2020 2020 2020 2020 2020 2020 2062 6f74               bot
-000011d0: 3d62 6f74 2c0d 0a20 2020 2020 2020 2020  =bot,..         
-000011e0: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
-000011f0: 6573 7361 6765 2e63 6861 742e 6964 2c0d  essage.chat.id,.
-00001200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001210: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
-00001220: 6964 3d6d 6573 7361 6765 2e6d 6573 7361  id=message.messa
-00001230: 6765 5f74 6872 6561 645f 6964 2c0d 0a20  ge_thread_id,.. 
-00001240: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001250: 6578 743d 7465 7874 2c0d 0a20 2020 2020  ext=text,..     
-00001260: 2020 2020 2020 2020 2020 2070 686f 746f             photo
-00001270: 3d70 686f 746f 2c0d 0a20 2020 2020 2020  =photo,..       
-00001280: 2020 2020 2020 2020 2076 6964 656f 3d76           video=v
-00001290: 6964 656f 2c0d 0a20 2020 2020 2020 2020  ideo,..         
-000012a0: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
-000012b0: 6b75 703d 7265 706c 795f 6d61 726b 7570  kup=reply_markup
-000012c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000012d0: 2020 2070 6172 7365 5f6d 6f64 653d 7061     parse_mode=pa
-000012e0: 7273 655f 6d6f 6465 2c0d 0a20 2020 2020  rse_mode,..     
-000012f0: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-00001300: 6c65 5f77 6562 5f70 6167 655f 7072 6576  le_web_page_prev
-00001310: 6965 773d 6469 7361 626c 655f 7765 625f  iew=disable_web_
-00001320: 7061 6765 5f70 7265 7669 6577 0d0a 2020  page_preview..  
-00001330: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
-00001340: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-00001350: 6169 7420 4d65 7373 6167 6545 6469 746f  ait MessageEdito
-00001360: 722e 6564 6974 280d 0a20 2020 2020 2020  r.edit(..       
-00001370: 2020 2020 2062 6f74 3d62 6f74 2c0d 0a20       bot=bot,.. 
-00001380: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-00001390: 6964 3d6d 6573 7361 6765 2e63 6861 742e  id=message.chat.
-000013a0: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
-000013b0: 206d 6573 7361 6765 5f69 643d 6d65 7373   message_id=mess
-000013c0: 6167 652e 6d65 7373 6167 655f 6964 2c0d  age.message_id,.
-000013d0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-000013e0: 743d 7465 7874 2c0d 0a20 2020 2020 2020  t=text,..       
-000013f0: 2020 2020 2070 686f 746f 3d70 686f 746f       photo=photo
-00001400: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
-00001410: 6964 656f 3d76 6964 656f 2c0d 0a20 2020  ideo=video,..   
-00001420: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
-00001430: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
-00001440: 7570 2c0d 0a20 2020 2020 2020 2020 2020  up,..           
-00001450: 2070 6172 7365 5f6d 6f64 653d 7061 7273   parse_mode=pars
-00001460: 655f 6d6f 6465 2c0d 0a20 2020 2020 2020  e_mode,..       
-00001470: 2020 2020 2064 6973 6162 6c65 5f77 6562       disable_web
-00001480: 5f70 6167 655f 7072 6576 6965 773d 6469  _page_preview=di
-00001490: 7361 626c 655f 7765 625f 7061 6765 5f70  sable_web_page_p
-000014a0: 7265 7669 6577 0d0a 2020 2020 2020 2020  review..        
-000014b0: 290d 0a0d 0a20 2020 2064 6566 205f 6765  )....    def _ge
-000014c0: 745f 6361 6e5f 6564 6974 5f73 7461 7475  t_can_edit_statu
-000014d0: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-000014e0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-000014f0: 2020 206d 6573 7361 6765 3a20 4d65 7373     message: Mess
-00001500: 6167 652c 0d0a 2020 2020 2020 2020 2020  age,..          
-00001510: 2020 7068 6f74 6f3a 204f 7074 696f 6e61    photo: Optiona
-00001520: 6c5b 4653 496e 7075 7446 696c 655d 2c0d  l[FSInputFile],.
-00001530: 0a20 2020 2020 2020 2020 2020 2076 6964  .            vid
-00001540: 656f 3a20 4f70 7469 6f6e 616c 5b46 5349  eo: Optional[FSI
-00001550: 6e70 7574 4669 6c65 5d2c 0d0a 2020 2020  nputFile],..    
-00001560: 2920 2d3e 2062 6f6f 6c3a 0d0a 0d0a 2020  ) -> bool:....  
-00001570: 2020 2020 2020 6966 206d 6573 7361 6765        if message
-00001580: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00001590: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000015a0: 6c73 650d 0a0d 0a20 2020 2020 2020 2069  lse....        i
-000015b0: 6620 6e6f 7420 7365 6c66 2e5f 6765 745f  f not self._get_
-000015c0: 626f 745f 616c 6c6f 775f 6564 6974 5f73  bot_allow_edit_s
-000015d0: 7461 7475 7328 0d0a 2020 2020 2020 2020  tatus(..        
-000015e0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-000015f0: 6d65 7373 6167 652c 0d0a 2020 2020 2020  message,..      
-00001600: 2020 2020 2020 2020 2020 7068 6f74 6f3d            photo=
-00001610: 7068 6f74 6f2c 0d0a 2020 2020 2020 2020  photo,..        
-00001620: 2020 2020 2020 2020 7669 6465 6f3d 7669          video=vi
-00001630: 6465 6f0d 0a20 2020 2020 2020 2029 3a0d  deo..        ):.
-00001640: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001650: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-00001660: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00001670: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-00001680: 6574 686f 640d 0a20 2020 2064 6566 205f  ethod..    def _
-00001690: 6765 745f 7374 6162 6c65 5f77 6169 745f  get_stable_wait_
-000016a0: 7469 6d65 286d 6573 7361 6765 3a20 4d65  time(message: Me
-000016b0: 7373 6167 6529 202d 3e20 666c 6f61 743a  ssage) -> float:
-000016c0: 0d0a 2020 2020 2020 2020 6966 206d 6573  ..        if mes
-000016d0: 7361 6765 2e65 6469 745f 6461 7465 3a0d  sage.edit_date:.
-000016e0: 0a20 2020 2020 2020 2020 2020 2064 7420  .            dt 
-000016f0: 3d20 6461 7465 7469 6d65 2e66 726f 6d74  = datetime.fromt
-00001700: 696d 6573 7461 6d70 286d 6573 7361 6765  imestamp(message
-00001710: 2e65 6469 745f 6461 7465 2c20 747a 3d70  .edit_date, tz=p
-00001720: 7974 7a2e 5554 4329 0d0a 0d0a 2020 2020  ytz.UTC)....    
-00001730: 2020 2020 2020 2020 6465 6c74 6120 3d20          delta = 
-00001740: 4c61 7a79 4564 6974 696e 672e 5f67 6574  LazyEditing._get
-00001750: 5f74 696d 655f 6265 7477 6565 6e5f 6375  _time_between_cu
-00001760: 7272 656e 745f 616e 645f 6d65 7373 6167  rrent_and_messag
-00001770: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
-00001780: 2020 2020 6d65 7373 6167 655f 6461 7465      message_date
-00001790: 3d64 740d 0a20 2020 2020 2020 2020 2020  =dt..           
-000017a0: 2029 0d0a 2020 2020 2020 2020 656c 7365   )..        else
-000017b0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-000017c0: 656c 7461 203d 204c 617a 7945 6469 7469  elta = LazyEditi
-000017d0: 6e67 2e5f 6765 745f 7469 6d65 5f62 6574  ng._get_time_bet
-000017e0: 7765 656e 5f63 7572 7265 6e74 5f61 6e64  ween_current_and
-000017f0: 5f6d 6573 7361 6765 280d 0a20 2020 2020  _message(..     
-00001800: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00001810: 6765 5f64 6174 653d 6d65 7373 6167 652e  ge_date=message.
-00001820: 6461 7465 0d0a 2020 2020 2020 2020 2020  date..          
-00001830: 2020 290d 0a0d 0a20 2020 2020 2020 2074    )....        t
-00001840: 6f74 616c 5f73 6563 6f6e 6473 203d 2064  otal_seconds = d
-00001850: 656c 7461 2e74 6f74 616c 5f73 6563 6f6e  elta.total_secon
-00001860: 6473 2829 0d0a 0d0a 2020 2020 2020 2020  ds()....        
-00001870: 7761 6974 5f74 696d 6520 3d20 436f 6e73  wait_time = Cons
-00001880: 742e 5354 4142 4c45 5f57 4149 545f 5449  t.STABLE_WAIT_TI
-00001890: 4d45 5f53 4543 4f4e 4453 202d 2074 6f74  ME_SECONDS - tot
-000018a0: 616c 5f73 6563 6f6e 6473 0d0a 2020 2020  al_seconds..    
-000018b0: 2020 2020 7265 7475 726e 2072 6f75 6e64      return round
-000018c0: 2877 6169 745f 7469 6d65 2c20 3329 0d0a  (wait_time, 3)..
-000018d0: 0d0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-000018e0: 6564 6974 280d 0a20 2020 2020 2020 2020  edit(..         
-000018f0: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
-00001900: 2020 2020 2020 7465 7874 3a20 4f70 7469        text: Opti
-00001910: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00001920: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
-00001930: 686f 746f 3a20 4f70 7469 6f6e 616c 5b46  hoto: Optional[F
-00001940: 5349 6e70 7574 4669 6c65 5d20 3d20 4e6f  SInputFile] = No
-00001950: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-00001960: 2076 6964 656f 3a20 4f70 7469 6f6e 616c   video: Optional
-00001970: 5b46 5349 6e70 7574 4669 6c65 5d20 3d20  [FSInputFile] = 
-00001980: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
-00001990: 2020 2072 6570 6c79 5f6d 6172 6b75 703a     reply_markup:
-000019a0: 204f 7074 696f 6e61 6c5b 496e 6c69 6e65   Optional[Inline
-000019b0: 4b65 7962 6f61 7264 4d61 726b 7570 5d20  KeyboardMarkup] 
-000019c0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-000019d0: 2020 2020 2070 6172 7365 5f6d 6f64 653a       parse_mode:
-000019e0: 2055 6e69 6f6e 5b73 7472 5d20 3d20 554e   Union[str] = UN
-000019f0: 5345 545f 5041 5253 455f 4d4f 4445 2c0d  SET_PARSE_MODE,.
-00001a00: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00001a10: 6162 6c65 5f77 6562 5f70 6167 655f 7072  able_web_page_pr
-00001a20: 6576 6965 773a 2062 6f6f 6c20 3d20 4661  eview: bool = Fa
-00001a30: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-00001a40: 2020 616e 7377 6572 5f74 6578 743a 204f    answer_text: O
-00001a50: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00001a60: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00001a70: 2020 616e 7377 6572 5f73 686f 775f 616c    answer_show_al
-00001a80: 6572 743a 2062 6f6f 6c20 3d20 4661 6c73  ert: bool = Fals
-00001a90: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00001aa0: 6175 746f 616e 7377 6572 3a20 626f 6f6c  autoanswer: bool
-00001ab0: 203d 2054 7275 650d 0a20 2020 2029 202d   = True..    ) -
-00001ac0: 3e20 556e 696f 6e5b 4d65 7373 6167 652c  > Union[Message,
-00001ad0: 2062 6f6f 6c5d 3a0d 0a0d 0a20 2020 2020   bool]:....     
-00001ae0: 2020 2063 616c 6c62 6163 6b20 3d20 7365     callback = se
-00001af0: 6c66 2e63 616c 6c62 6163 6b0d 0a20 2020  lf.callback..   
-00001b00: 2020 2020 206d 6573 7361 6765 203d 2063       message = c
-00001b10: 616c 6c62 6163 6b2e 6d65 7373 6167 650d  allback.message.
-00001b20: 0a0d 0a20 2020 2020 2020 2069 6620 6d65  ...        if me
-00001b30: 7373 6167 6520 6973 204e 6f6e 653a 0d0a  ssage is None:..
-00001b40: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00001b50: 7420 6361 6c6c 6261 636b 2e61 6e73 7765  t callback.answe
-00001b60: 7228 224d 6573 7361 6765 2074 6f6f 206f  r("Message too o
-00001b70: 6c64 2229 0d0a 0d0a 2020 2020 2020 2020  ld")....        
-00001b80: 2020 2020 7261 6973 6520 4d65 7373 6167      raise Messag
-00001b90: 6554 6f6f 4f6c 640d 0a0d 0a20 2020 2020  eTooOld....     
-00001ba0: 2020 2069 6620 7365 6c66 2e73 7461 626c     if self.stabl
-00001bb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001bc0: 6177 6169 7420 6173 796e 6369 6f2e 736c  await asyncio.sl
-00001bd0: 6565 7028 7365 6c66 2e5f 6765 745f 7374  eep(self._get_st
-00001be0: 6162 6c65 5f77 6169 745f 7469 6d65 286d  able_wait_time(m
-00001bf0: 6573 7361 6765 2929 0d0a 0d0a 2020 2020  essage))....    
-00001c00: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00001c10: 5f67 6574 5f64 6174 615f 6368 616e 6765  _get_data_change
-00001c20: 735f 7374 6174 7573 280d 0a20 2020 2020  s_status(..     
-00001c30: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00001c40: 6765 3d6d 6573 7361 6765 2c0d 0a20 2020  ge=message,..   
-00001c50: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-00001c60: 743d 7465 7874 2c0d 0a20 2020 2020 2020  t=text,..       
-00001c70: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
-00001c80: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
-00001c90: 7570 2c0d 0a20 2020 2020 2020 2020 2020  up,..           
-00001ca0: 2020 2020 2076 6964 656f 3d76 6964 656f       video=video
-00001cb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001cc0: 2020 2070 686f 746f 3d70 686f 746f 0d0a     photo=photo..
-00001cd0: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
-00001ce0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-00001cf0: 6573 7361 6765 0d0a 0d0a 2020 2020 2020  essage....      
-00001d00: 2020 6361 6e5f 6564 6974 203d 2073 656c    can_edit = sel
-00001d10: 662e 5f67 6574 5f63 616e 5f65 6469 745f  f._get_can_edit_
-00001d20: 7374 6174 7573 280d 0a20 2020 2020 2020  status(..       
-00001d30: 2020 2020 206d 6573 7361 6765 3d6d 6573       message=mes
-00001d40: 7361 6765 2c0d 0a20 2020 2020 2020 2020  sage,..         
-00001d50: 2020 2070 686f 746f 3d70 686f 746f 2c0d     photo=photo,.
-00001d60: 0a20 2020 2020 2020 2020 2020 2076 6964  .            vid
-00001d70: 656f 3d76 6964 656f 2c0d 0a20 2020 2020  eo=video,..     
-00001d80: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
-00001d90: 7265 7375 6c74 203d 2061 7761 6974 2073  result = await s
-00001da0: 656c 662e 5f73 656e 645f 6f72 5f65 6469  elf._send_or_edi
-00001db0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-00001dc0: 626f 743d 7365 6c66 2e62 6f74 2c0d 0a20  bot=self.bot,.. 
-00001dd0: 2020 2020 2020 2020 2020 2063 616e 5f65             can_e
-00001de0: 6469 743d 6361 6e5f 6564 6974 2c0d 0a20  dit=can_edit,.. 
-00001df0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00001e00: 6765 3d6d 6573 7361 6765 2c0d 0a20 2020  ge=message,..   
-00001e10: 2020 2020 2020 2020 2074 6578 743d 7465           text=te
-00001e20: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
-00001e30: 2070 686f 746f 3d70 686f 746f 2c0d 0a20   photo=photo,.. 
-00001e40: 2020 2020 2020 2020 2020 2076 6964 656f             video
-00001e50: 3d76 6964 656f 2c0d 0a20 2020 2020 2020  =video,..       
-00001e60: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
-00001e70: 703d 7265 706c 795f 6d61 726b 7570 2c0d  p=reply_markup,.
-00001e80: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-00001e90: 7365 5f6d 6f64 653d 7061 7273 655f 6d6f  se_mode=parse_mo
-00001ea0: 6465 2c0d 0a20 2020 2020 2020 2020 2020  de,..           
-00001eb0: 2064 6973 6162 6c65 5f77 6562 5f70 6167   disable_web_pag
-00001ec0: 655f 7072 6576 6965 773d 6469 7361 626c  e_preview=disabl
-00001ed0: 655f 7765 625f 7061 6765 5f70 7265 7669  e_web_page_previ
-00001ee0: 6577 2c0d 0a20 2020 2020 2020 2029 0d0a  ew,..        )..
-00001ef0: 0d0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
-00001f00: 6173 796e 6369 6f2e 736c 6565 7028 436f  asyncio.sleep(Co
-00001f10: 6e73 742e 5345 434f 4e44 535f 4245 5457  nst.SECONDS_BETW
-00001f20: 4545 4e5f 4f50 4552 4154 494f 4e29 0d0a  EEN_OPERATION)..
-00001f30: 0d0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
-00001f40: 7365 6c66 2e5f 6175 746f 5f63 616c 6c62  self._auto_callb
-00001f50: 6163 6b5f 616e 7377 6572 280d 0a20 2020  ack_answer(..   
-00001f60: 2020 2020 2020 2020 2062 6f74 3d73 656c           bot=sel
-00001f70: 662e 626f 742c 0d0a 2020 2020 2020 2020  f.bot,..        
-00001f80: 2020 2020 6361 6c6c 6261 636b 5f69 643d      callback_id=
-00001f90: 6361 6c6c 6261 636b 2e69 642c 0d0a 2020  callback.id,..  
-00001fa0: 2020 2020 2020 2020 2020 6175 746f 616e            autoan
-00001fb0: 7377 6572 3d61 7574 6f61 6e73 7765 722c  swer=autoanswer,
-00001fc0: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
-00001fd0: 7377 6572 5f74 6578 743d 616e 7377 6572  swer_text=answer
-00001fe0: 5f74 6578 742c 0d0a 2020 2020 2020 2020  _text,..        
-00001ff0: 2020 2020 616e 7377 6572 5f73 686f 775f      answer_show_
-00002000: 616c 6572 743d 616e 7377 6572 5f73 686f  alert=answer_sho
-00002010: 775f 616c 6572 740d 0a20 2020 2020 2020  w_alert..       
-00002020: 2029 0d0a 0d0a 2020 2020 2020 2020 7265   )....        re
-00002030: 7475 726e 2072 6573 756c 740d 0a         turn result..
+000001f0: 7373 6167 6553 656e 6465 720d 0a66 726f  ssageSender..fro
+00000200: 6d20 7573 6566 756c 6772 616d 2e6c 617a  m usefulgram.laz
+00000210: 792e 7374 6162 6c65 5f77 6169 7420 696d  y.stable_wait im
+00000220: 706f 7274 2053 7461 626c 6557 6169 7465  port StableWaite
+00000230: 720d 0a66 726f 6d20 7573 6566 756c 6772  r..from usefulgr
+00000240: 616d 2e6c 617a 792e 6361 6c6c 6261 636b  am.lazy.callback
+00000250: 5f72 6573 706f 6e64 6572 2069 6d70 6f72  _responder impor
+00000260: 7420 4361 6c6c 6261 636b 416e 7377 6572  t CallbackAnswer
+00000270: 0d0a 0d0a 0d0a 636c 6173 7320 4c61 7a79  ......class Lazy
+00000280: 4564 6974 6f72 3a0d 0a20 2020 205f 6361  Editor:..    _ca
+00000290: 6c6c 6261 636b 3a20 4361 6c6c 6261 636b  llback: Callback
+000002a0: 5175 6572 790d 0a20 2020 205f 626f 743a  Query..    _bot:
+000002b0: 2042 6f74 0d0a 2020 2020 5f73 7461 626c   Bot..    _stabl
+000002c0: 653a 2062 6f6f 6c0d 0a0d 0a20 2020 2064  e: bool....    d
+000002d0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000002e0: 2c20 6361 6c6c 6261 636b 3a20 4361 6c6c  , callback: Call
+000002f0: 6261 636b 5175 6572 792c 2062 6f74 3a20  backQuery, bot: 
+00000300: 426f 742c 2073 7461 626c 653a 2062 6f6f  Bot, stable: boo
+00000310: 6c20 3d20 4661 6c73 6529 3a0d 0a20 2020  l = False):..   
+00000320: 2020 2020 2073 656c 662e 5f63 616c 6c62       self._callb
+00000330: 6163 6b20 3d20 6361 6c6c 6261 636b 0d0a  ack = callback..
+00000340: 2020 2020 2020 2020 7365 6c66 2e5f 626f          self._bo
+00000350: 7420 3d20 626f 740d 0a20 2020 2020 2020  t = bot..       
+00000360: 2073 656c 662e 5f73 7461 626c 6520 3d20   self._stable = 
+00000370: 7374 6162 6c65 0d0a 0d0a 2020 2020 4073  stable....    @s
+00000380: 7461 7469 636d 6574 686f 640d 0a20 2020  taticmethod..   
+00000390: 2064 6566 205f 6765 745f 7465 7874 5f62   def _get_text_b
+000003a0: 795f 6361 7074 696f 6e28 0d0a 2020 2020  y_caption(..    
+000003b0: 2020 2020 2020 2020 7465 7874 3a20 4f70          text: Op
+000003c0: 7469 6f6e 616c 5b73 7472 5d2c 0d0a 2020  tional[str],..  
+000003d0: 2020 2020 2020 2020 2020 6361 7074 696f            captio
+000003e0: 6e3a 204f 7074 696f 6e61 6c5b 7374 725d  n: Optional[str]
+000003f0: 0d0a 2020 2020 2920 2d3e 204f 7074 696f  ..    ) -> Optio
+00000400: 6e61 6c5b 7374 725d 3a0d 0a0d 0a20 2020  nal[str]:....   
+00000410: 2020 2020 2069 6620 7465 7874 2069 7320       if text is 
+00000420: 4e6f 6e65 206f 7220 6361 7074 696f 6e20  None or caption 
+00000430: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00000440: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000450: 2063 6170 7469 6f6e 0d0a 0d0a 2020 2020   caption....    
+00000460: 2020 2020 7265 7475 726e 2074 6578 740d      return text.
+00000470: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+00000480: 7468 6f64 0d0a 2020 2020 6465 6620 5f67  thod..    def _g
+00000490: 6574 5f6d 6573 7361 6765 5f74 6578 7428  et_message_text(
+000004a0: 7465 7874 3a20 4f70 7469 6f6e 616c 5b73  text: Optional[s
+000004b0: 7472 5d2c 206d 6573 7361 6765 3a20 4d65  tr], message: Me
+000004c0: 7373 6167 6529 202d 3e20 4f70 7469 6f6e  ssage) -> Option
+000004d0: 616c 5b73 7472 5d3a 0d0a 2020 2020 2020  al[str]:..      
+000004e0: 2020 6966 2074 6578 7420 6973 204e 6f6e    if text is Non
+000004f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000500: 7265 7475 726e 206d 6573 7361 6765 2e74  return message.t
+00000510: 6578 740d 0a0d 0a20 2020 2020 2020 2072  ext....        r
+00000520: 6574 7572 6e20 7465 7874 0d0a 0d0a 2020  eturn text....  
+00000530: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
+00000540: 0a20 2020 2064 6566 205f 6765 745f 6461  .    def _get_da
+00000550: 7461 5f63 6861 6e67 6573 5f73 7461 7475  ta_changes_statu
+00000560: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
+00000570: 6d65 7373 6167 653a 204d 6573 7361 6765  message: Message
+00000580: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00000590: 6578 743a 204f 7074 696f 6e61 6c5b 7374  ext: Optional[st
+000005a0: 725d 2c0d 0a20 2020 2020 2020 2020 2020  r],..           
+000005b0: 2072 6570 6c79 5f6d 6172 6b75 703a 204f   reply_markup: O
+000005c0: 7074 696f 6e61 6c5b 496e 6c69 6e65 4b65  ptional[InlineKe
+000005d0: 7962 6f61 7264 4d61 726b 7570 5d2c 0d0a  yboardMarkup],..
+000005e0: 2020 2020 2020 2020 2020 2020 7669 6465              vide
+000005f0: 6f3a 204f 7074 696f 6e61 6c5b 4653 496e  o: Optional[FSIn
+00000600: 7075 7446 696c 655d 2c0d 0a20 2020 2020  putFile],..     
+00000610: 2020 2020 2020 2070 686f 746f 3a20 4f70         photo: Op
+00000620: 7469 6f6e 616c 5b46 5349 6e70 7574 4669  tional[FSInputFi
+00000630: 6c65 5d29 202d 3e20 626f 6f6c 3a0d 0a0d  le]) -> bool:...
+00000640: 0a20 2020 2020 2020 2069 6620 6d65 7373  .        if mess
+00000650: 6167 652e 7465 7874 2021 3d20 7465 7874  age.text != text
+00000660: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00000670: 6574 7572 6e20 5472 7565 0d0a 0d0a 2020  eturn True....  
+00000680: 2020 2020 2020 6966 206d 6573 7361 6765        if message
+00000690: 2e72 6570 6c79 5f6d 6172 6b75 7020 213d  .reply_markup !=
+000006a0: 2072 6570 6c79 5f6d 6172 6b75 703a 0d0a   reply_markup:..
+000006b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000006c0: 726e 2054 7275 650d 0a0d 0a20 2020 2020  rn True....     
+000006d0: 2020 2069 6620 6d65 7373 6167 652e 7669     if message.vi
+000006e0: 6465 6f20 213d 2076 6964 656f 3a0d 0a20  deo != video:.. 
+000006f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000700: 6e20 5472 7565 0d0a 0d0a 2020 2020 2020  n True....      
+00000710: 2020 6966 206d 6573 7361 6765 2e70 686f    if message.pho
+00000720: 746f 2021 3d20 7068 6f74 6f3a 0d0a 2020  to != photo:..  
+00000730: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000740: 2054 7275 650d 0a0d 0a20 2020 2020 2020   True....       
+00000750: 2072 6574 7572 6e20 4661 6c73 650d 0a0d   return False...
+00000760: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00000770: 6f64 0d0a 2020 2020 6465 6620 5f67 6574  od..    def _get
+00000780: 5f64 656c 7461 5f62 6574 7765 656e 5f63  _delta_between_c
+00000790: 7572 7265 6e74 5f61 6e64 5f6d 6573 7361  urrent_and_messa
+000007a0: 6765 280d 0a20 2020 2020 2020 2020 2020  ge(..           
+000007b0: 206d 6573 7361 6765 5f64 6174 653a 2064   message_date: d
+000007c0: 6174 6574 696d 650d 0a20 2020 2029 202d  atetime..    ) -
+000007d0: 3e20 7469 6d65 6465 6c74 613a 0d0a 0d0a  > timedelta:....
+000007e0: 2020 2020 2020 2020 6375 7272 656e 7420          current 
+000007f0: 3d20 6461 7465 7469 6d65 2e6e 6f77 2874  = datetime.now(t
+00000800: 7a3d 7079 747a 2e55 5443 290d 0a0d 0a20  z=pytz.UTC).... 
+00000810: 2020 2020 2020 2072 6574 7572 6e20 6375         return cu
+00000820: 7272 656e 7420 2d20 6d65 7373 6167 655f  rrent - message_
+00000830: 6461 7465 0d0a 0d0a 2020 2020 4073 7461  date....    @sta
+00000840: 7469 636d 6574 686f 640d 0a20 2020 2064  ticmethod..    d
+00000850: 6566 205f 6765 745f 7469 6d65 5f61 6c6c  ef _get_time_all
+00000860: 6f77 6564 5f65 6469 745f 7374 6174 7573  owed_edit_status
+00000870: 286d 6573 7361 6765 3a20 4d65 7373 6167  (message: Messag
+00000880: 6529 202d 3e20 626f 6f6c 3a0d 0a20 2020  e) -> bool:..   
+00000890: 2020 2020 2063 6f6e 7374 5f64 656c 7461       const_delta
+000008a0: 203d 2074 696d 6564 656c 7461 2868 6f75   = timedelta(hou
+000008b0: 7273 3d43 6f6e 7374 2e41 4c4c 4f57 5f45  rs=Const.ALLOW_E
+000008c0: 4449 5449 4e47 5f44 454c 5441 290d 0a0d  DITING_DELTA)...
+000008d0: 0a20 2020 2020 2020 2064 656c 7461 203d  .        delta =
+000008e0: 204c 617a 7945 6469 746f 722e 5f67 6574   LazyEditor._get
+000008f0: 5f64 656c 7461 5f62 6574 7765 656e 5f63  _delta_between_c
+00000900: 7572 7265 6e74 5f61 6e64 5f6d 6573 7361  urrent_and_messa
+00000910: 6765 280d 0a20 2020 2020 2020 2020 2020  ge(..           
+00000920: 206d 6573 7361 6765 2e64 6174 650d 0a20   message.date.. 
+00000930: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+00000940: 2020 2020 7265 7475 726e 2064 656c 7461      return delta
+00000950: 203c 2063 6f6e 7374 5f64 656c 7461 0d0a   < const_delta..
+00000960: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00000970: 686f 640d 0a20 2020 2064 6566 205f 6765  hod..    def _ge
+00000980: 745f 6d65 7373 6167 655f 696e 5f63 6861  t_message_in_cha
+00000990: 745f 7374 6174 7573 286d 6573 7361 6765  t_status(message
+000009a0: 3a20 4d65 7373 6167 6529 202d 3e20 626f  : Message) -> bo
+000009b0: 6f6c 3a0d 0a20 2020 2020 2020 2069 6620  ol:..        if 
+000009c0: 6d65 7373 6167 652e 6368 6174 2e74 7970  message.chat.typ
+000009d0: 6520 3d3d 2043 6861 7454 7970 652e 4348  e == ChatType.CH
+000009e0: 414e 4e45 4c3a 0d0a 2020 2020 2020 2020  ANNEL:..        
+000009f0: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
+00000a00: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00000a10: 6e20 4661 6c73 650d 0a0d 0a20 2020 2040  n False....    @
+00000a20: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
+00000a30: 2020 6465 6620 5f67 6574 5f6d 6573 7361    def _get_messa
+00000a40: 6765 5f6d 6564 6961 5f69 735f 636f 7272  ge_media_is_corr
+00000a50: 6563 745f 7374 6174 7573 280d 0a20 2020  ect_status(..   
+00000a60: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00000a70: 3a20 4d65 7373 6167 652c 0d0a 2020 2020  : Message,..    
+00000a80: 2020 2020 2020 2020 7068 6f74 6f3a 204f          photo: O
+00000a90: 7074 696f 6e61 6c5b 4653 496e 7075 7446  ptional[FSInputF
+00000aa0: 696c 655d 2c0d 0a20 2020 2020 2020 2020  ile],..         
+00000ab0: 2020 2076 6964 656f 3a20 4f70 7469 6f6e     video: Option
+00000ac0: 616c 5b46 5349 6e70 7574 4669 6c65 5d0d  al[FSInputFile].
+00000ad0: 0a20 2020 2029 202d 3e20 626f 6f6c 3a0d  .    ) -> bool:.
+00000ae0: 0a0d 0a20 2020 2020 2020 206d 6573 7361  ...        messa
+00000af0: 6765 5f68 6173 5f70 686f 746f 5f6f 725f  ge_has_photo_or_
+00000b00: 7669 6465 6f20 3d20 6d65 7373 6167 652e  video = message.
+00000b10: 7068 6f74 6f20 6f72 206d 6573 7361 6765  photo or message
+00000b20: 2e76 6964 656f 0d0a 0d0a 2020 2020 2020  .video....      
+00000b30: 2020 6966 2070 686f 746f 2061 6e64 206e    if photo and n
+00000b40: 6f74 206d 6573 7361 6765 5f68 6173 5f70  ot message_has_p
+00000b50: 686f 746f 5f6f 725f 7669 6465 6f3a 0d0a  hoto_or_video:..
+00000b60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000b70: 726e 2046 616c 7365 0d0a 0d0a 2020 2020  rn False....    
+00000b80: 2020 2020 656c 6966 2076 6964 656f 2061      elif video a
+00000b90: 6e64 206e 6f74 206d 6573 7361 6765 5f68  nd not message_h
+00000ba0: 6173 5f70 686f 746f 5f6f 725f 7669 6465  as_photo_or_vide
+00000bb0: 6f3a 0d0a 2020 2020 2020 2020 2020 2020  o:..            
+00000bc0: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
+00000bd0: 2020 2020 2020 2020 656c 6966 2028 6e6f          elif (no
+00000be0: 7420 7669 6465 6f20 6f72 206e 6f74 2070  t video or not p
+00000bf0: 686f 746f 2920 616e 6420 6d65 7373 6167  hoto) and messag
+00000c00: 655f 6861 735f 7068 6f74 6f5f 6f72 5f76  e_has_photo_or_v
+00000c10: 6964 656f 3a0d 0a20 2020 2020 2020 2020  ideo:..         
+00000c20: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+00000c30: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00000c40: 6e20 5472 7565 0d0a 0d0a 2020 2020 6465  n True....    de
+00000c50: 6620 5f67 6574 5f62 6f74 5f61 6c6c 6f77  f _get_bot_allow
+00000c60: 5f65 6469 745f 7374 6174 7573 280d 0a20  _edit_status(.. 
+00000c70: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00000c80: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
+00000c90: 7373 6167 653a 204d 6573 7361 6765 2c0d  ssage: Message,.
+00000ca0: 0a20 2020 2020 2020 2020 2020 2070 686f  .            pho
+00000cb0: 746f 3a20 4f70 7469 6f6e 616c 5b46 5349  to: Optional[FSI
+00000cc0: 6e70 7574 4669 6c65 5d2c 0d0a 2020 2020  nputFile],..    
+00000cd0: 2020 2020 2020 2020 7669 6465 6f3a 204f          video: O
+00000ce0: 7074 696f 6e61 6c5b 4653 496e 7075 7446  ptional[FSInputF
+00000cf0: 696c 655d 2c0d 0a20 2020 2029 202d 3e20  ile],..    ) -> 
+00000d00: 626f 6f6c 3a0d 0a0d 0a20 2020 2020 2020  bool:....       
+00000d10: 2069 6620 7365 6c66 2e5f 6765 745f 6d65   if self._get_me
+00000d20: 7373 6167 655f 696e 5f63 6861 745f 7374  ssage_in_chat_st
+00000d30: 6174 7573 286d 6573 7361 6765 293a 0d0a  atus(message):..
+00000d40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000d50: 726e 2054 7275 650d 0a0d 0a20 2020 2020  rn True....     
+00000d60: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
+00000d70: 6765 745f 7469 6d65 5f61 6c6c 6f77 6564  get_time_allowed
+00000d80: 5f65 6469 745f 7374 6174 7573 286d 6573  _edit_status(mes
+00000d90: 7361 6765 293a 0d0a 2020 2020 2020 2020  sage):..        
+00000da0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00000db0: 0d0a 0d0a 2020 2020 2020 2020 6966 206e  ....        if n
+00000dc0: 6f74 2073 656c 662e 5f67 6574 5f6d 6573  ot self._get_mes
+00000dd0: 7361 6765 5f6d 6564 6961 5f69 735f 636f  sage_media_is_co
+00000de0: 7272 6563 745f 7374 6174 7573 280d 0a20  rrect_status(.. 
+00000df0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00000e00: 6765 3d6d 6573 7361 6765 2c20 7068 6f74  ge=message, phot
+00000e10: 6f3d 7068 6f74 6f2c 2076 6964 656f 3d76  o=photo, video=v
+00000e20: 6964 656f 0d0a 2020 2020 2020 2020 293a  ideo..        ):
+00000e30: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00000e40: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
+00000e50: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00000e60: 650d 0a0d 0a20 2020 2040 7374 6174 6963  e....    @static
+00000e70: 6d65 7468 6f64 0d0a 2020 2020 6173 796e  method..    asyn
+00000e80: 6320 6465 6620 5f73 656e 645f 6f72 5f65  c def _send_or_e
+00000e90: 6469 7428 0d0a 2020 2020 2020 2020 2020  dit(..          
+00000ea0: 2020 626f 743a 2042 6f74 2c0d 0a20 2020    bot: Bot,..   
+00000eb0: 2020 2020 2020 2020 2063 616e 5f65 6469           can_edi
+00000ec0: 743a 2062 6f6f 6c2c 0d0a 2020 2020 2020  t: bool,..      
+00000ed0: 2020 2020 2020 6d65 7373 6167 653a 204d        message: M
+00000ee0: 6573 7361 6765 2c0d 0a20 2020 2020 2020  essage,..       
+00000ef0: 2020 2020 2074 6578 743a 204f 7074 696f       text: Optio
+00000f00: 6e61 6c5b 7374 725d 2c0d 0a20 2020 2020  nal[str],..     
+00000f10: 2020 2020 2020 2070 686f 746f 3a20 4f70         photo: Op
+00000f20: 7469 6f6e 616c 5b46 5349 6e70 7574 4669  tional[FSInputFi
+00000f30: 6c65 5d2c 0d0a 2020 2020 2020 2020 2020  le],..          
+00000f40: 2020 7669 6465 6f3a 204f 7074 696f 6e61    video: Optiona
+00000f50: 6c5b 4653 496e 7075 7446 696c 655d 2c0d  l[FSInputFile],.
+00000f60: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+00000f70: 6c79 5f6d 6172 6b75 703a 204f 7074 696f  ly_markup: Optio
+00000f80: 6e61 6c5b 496e 6c69 6e65 4b65 7962 6f61  nal[InlineKeyboa
+00000f90: 7264 4d61 726b 7570 5d2c 0d0a 2020 2020  rdMarkup],..    
+00000fa0: 2020 2020 2020 2020 7061 7273 655f 6d6f          parse_mo
+00000fb0: 6465 3a20 556e 696f 6e5b 7374 725d 2c0d  de: Union[str],.
+00000fc0: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00000fd0: 6162 6c65 5f77 6562 5f70 6167 655f 7072  able_web_page_pr
+00000fe0: 6576 6965 773a 2062 6f6f 6c2c 0d0a 2020  eview: bool,..  
+00000ff0: 2020 2920 2d3e 2055 6e69 6f6e 5b4d 6573    ) -> Union[Mes
+00001000: 7361 6765 2c20 626f 6f6c 5d3a 0d0a 0d0a  sage, bool]:....
+00001010: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00001020: 616e 5f65 6469 743a 0d0a 2020 2020 2020  an_edit:..      
+00001030: 2020 2020 2020 7465 7874 203d 204c 617a        text = Laz
+00001040: 7945 6469 746f 722e 5f67 6574 5f6d 6573  yEditor._get_mes
+00001050: 7361 6765 5f74 6578 7428 7465 7874 2c20  sage_text(text, 
+00001060: 6d65 7373 6167 653d 6d65 7373 6167 6529  message=message)
+00001070: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001080: 7265 7475 726e 2061 7761 6974 204d 6573  return await Mes
+00001090: 7361 6765 5365 6e64 6572 2e73 656e 6428  sageSender.send(
+000010a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000010b0: 2020 626f 743d 626f 742c 0d0a 2020 2020    bot=bot,..    
+000010c0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+000010d0: 5f69 643d 6d65 7373 6167 652e 6368 6174  _id=message.chat
+000010e0: 2e69 642c 0d0a 2020 2020 2020 2020 2020  .id,..          
+000010f0: 2020 2020 2020 6d65 7373 6167 655f 7468        message_th
+00001100: 7265 6164 5f69 643d 6d65 7373 6167 652e  read_id=message.
+00001110: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
+00001120: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+00001130: 2020 2020 7465 7874 3d74 6578 742c 0d0a      text=text,..
+00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001150: 7068 6f74 6f3d 7068 6f74 6f2c 0d0a 2020  photo=photo,..  
+00001160: 2020 2020 2020 2020 2020 2020 2020 7669                vi
+00001170: 6465 6f3d 7669 6465 6f2c 0d0a 2020 2020  deo=video,..    
+00001180: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+00001190: 795f 6d61 726b 7570 3d72 6570 6c79 5f6d  y_markup=reply_m
+000011a0: 6172 6b75 702c 0d0a 2020 2020 2020 2020  arkup,..        
+000011b0: 2020 2020 2020 2020 7061 7273 655f 6d6f          parse_mo
+000011c0: 6465 3d70 6172 7365 5f6d 6f64 652c 0d0a  de=parse_mode,..
+000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011e0: 6469 7361 626c 655f 7765 625f 7061 6765  disable_web_page
+000011f0: 5f70 7265 7669 6577 3d64 6973 6162 6c65  _preview=disable
+00001200: 5f77 6562 5f70 6167 655f 7072 6576 6965  _web_page_previe
+00001210: 770d 0a20 2020 2020 2020 2020 2020 2029  w..            )
+00001220: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+00001230: 726e 2061 7761 6974 204d 6573 7361 6765  rn await Message
+00001240: 4564 6974 6f72 2e65 6469 7428 0d0a 2020  Editor.edit(..  
+00001250: 2020 2020 2020 2020 2020 626f 743d 626f            bot=bo
+00001260: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
+00001270: 6368 6174 5f69 643d 6d65 7373 6167 652e  chat_id=message.
+00001280: 6368 6174 2e69 642c 0d0a 2020 2020 2020  chat.id,..      
+00001290: 2020 2020 2020 6d65 7373 6167 655f 6964        message_id
+000012a0: 3d6d 6573 7361 6765 2e6d 6573 7361 6765  =message.message
+000012b0: 5f69 642c 0d0a 2020 2020 2020 2020 2020  _id,..          
+000012c0: 2020 7465 7874 3d74 6578 742c 0d0a 2020    text=text,..  
+000012d0: 2020 2020 2020 2020 2020 7068 6f74 6f3d            photo=
+000012e0: 7068 6f74 6f2c 0d0a 2020 2020 2020 2020  photo,..        
+000012f0: 2020 2020 7669 6465 6f3d 7669 6465 6f2c      video=video,
+00001300: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00001310: 706c 795f 6d61 726b 7570 3d72 6570 6c79  ply_markup=reply
+00001320: 5f6d 6172 6b75 702c 0d0a 2020 2020 2020  _markup,..      
+00001330: 2020 2020 2020 7061 7273 655f 6d6f 6465        parse_mode
+00001340: 3d70 6172 7365 5f6d 6f64 652c 0d0a 2020  =parse_mode,..  
+00001350: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+00001360: 655f 7765 625f 7061 6765 5f70 7265 7669  e_web_page_previ
+00001370: 6577 3d64 6973 6162 6c65 5f77 6562 5f70  ew=disable_web_p
+00001380: 6167 655f 7072 6576 6965 770d 0a20 2020  age_preview..   
+00001390: 2020 2020 2029 0d0a 0d0a 2020 2020 6465       )....    de
+000013a0: 6620 5f67 6574 5f63 616e 5f65 6469 745f  f _get_can_edit_
+000013b0: 7374 6174 7573 280d 0a20 2020 2020 2020  status(..       
+000013c0: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
+000013d0: 2020 2020 2020 2020 6d65 7373 6167 653a          message:
+000013e0: 204d 6573 7361 6765 2c0d 0a20 2020 2020   Message,..     
+000013f0: 2020 2020 2020 2070 686f 746f 3a20 4f70         photo: Op
+00001400: 7469 6f6e 616c 5b46 5349 6e70 7574 4669  tional[FSInputFi
+00001410: 6c65 5d2c 0d0a 2020 2020 2020 2020 2020  le],..          
+00001420: 2020 7669 6465 6f3a 204f 7074 696f 6e61    video: Optiona
+00001430: 6c5b 4653 496e 7075 7446 696c 655d 2c0d  l[FSInputFile],.
+00001440: 0a20 2020 2029 202d 3e20 626f 6f6c 3a0d  .    ) -> bool:.
+00001450: 0a0d 0a20 2020 2020 2020 2069 6620 6d65  ...        if me
+00001460: 7373 6167 6520 6973 204e 6f6e 653a 0d0a  ssage is None:..
+00001470: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001480: 726e 2046 616c 7365 0d0a 0d0a 2020 2020  rn False....    
+00001490: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+000014a0: 5f67 6574 5f62 6f74 5f61 6c6c 6f77 5f65  _get_bot_allow_e
+000014b0: 6469 745f 7374 6174 7573 280d 0a20 2020  dit_status(..   
+000014c0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+000014d0: 7361 6765 3d6d 6573 7361 6765 2c0d 0a20  sage=message,.. 
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000014f0: 686f 746f 3d70 686f 746f 2c0d 0a20 2020  hoto=photo,..   
+00001500: 2020 2020 2020 2020 2020 2020 2076 6964               vid
+00001510: 656f 3d76 6964 656f 0d0a 2020 2020 2020  eo=video..      
+00001520: 2020 293a 0d0a 2020 2020 2020 2020 2020    ):..          
+00001530: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+00001540: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001550: 2054 7275 650d 0a0d 0a20 2020 2040 7374   True....    @st
+00001560: 6174 6963 6d65 7468 6f64 0d0a 2020 2020  aticmethod..    
+00001570: 6465 6620 5f67 6574 5f73 7461 626c 655f  def _get_stable_
+00001580: 7761 6974 5f74 696d 6528 6d65 7373 6167  wait_time(messag
+00001590: 653a 204d 6573 7361 6765 2920 2d3e 2066  e: Message) -> f
+000015a0: 6c6f 6174 3a0d 0a20 2020 2020 2020 2069  loat:..        i
+000015b0: 6620 6d65 7373 6167 652e 6564 6974 5f64  f message.edit_d
+000015c0: 6174 653a 0d0a 2020 2020 2020 2020 2020  ate:..          
+000015d0: 2020 6474 203d 2064 6174 6574 696d 652e    dt = datetime.
+000015e0: 6672 6f6d 7469 6d65 7374 616d 7028 6d65  fromtimestamp(me
+000015f0: 7373 6167 652e 6564 6974 5f64 6174 652c  ssage.edit_date,
+00001600: 2074 7a3d 7079 747a 2e55 5443 290d 0a0d   tz=pytz.UTC)...
+00001610: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00001620: 2020 2020 2020 2020 2020 2020 6474 203d              dt =
+00001630: 206d 6573 7361 6765 2e64 6174 650d 0a0d   message.date...
+00001640: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001650: 5374 6162 6c65 5761 6974 6572 2e67 6574  StableWaiter.get
+00001660: 5f73 7461 626c 655f 7761 6974 5f74 696d  _stable_wait_tim
+00001670: 6528 6474 290d 0a0d 0a20 2020 2061 7379  e(dt)....    asy
+00001680: 6e63 2064 6566 2065 6469 7428 0d0a 2020  nc def edit(..  
+00001690: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+000016a0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+000016b0: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
+000016c0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+000016d0: 2020 2020 2020 7068 6f74 6f3a 204f 7074        photo: Opt
+000016e0: 696f 6e61 6c5b 4653 496e 7075 7446 696c  ional[FSInputFil
+000016f0: 655d 203d 204e 6f6e 652c 0d0a 2020 2020  e] = None,..    
+00001700: 2020 2020 2020 2020 7669 6465 6f3a 204f          video: O
+00001710: 7074 696f 6e61 6c5b 4653 496e 7075 7446  ptional[FSInputF
+00001720: 696c 655d 203d 204e 6f6e 652c 0d0a 2020  ile] = None,..  
+00001730: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00001740: 6d61 726b 7570 3a20 4f70 7469 6f6e 616c  markup: Optional
+00001750: 5b49 6e6c 696e 654b 6579 626f 6172 644d  [InlineKeyboardM
+00001760: 6172 6b75 705d 203d 204e 6f6e 652c 0d0a  arkup] = None,..
+00001770: 2020 2020 2020 2020 2020 2020 7061 7273              pars
+00001780: 655f 6d6f 6465 3a20 556e 696f 6e5b 7374  e_mode: Union[st
+00001790: 725d 203d 2055 4e53 4554 5f50 4152 5345  r] = UNSET_PARSE
+000017a0: 5f4d 4f44 452c 0d0a 2020 2020 2020 2020  _MODE,..        
+000017b0: 2020 2020 6469 7361 626c 655f 7765 625f      disable_web_
+000017c0: 7061 6765 5f70 7265 7669 6577 3a20 626f  page_preview: bo
+000017d0: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
+000017e0: 2020 2020 2020 2020 2061 6e73 7765 725f           answer_
+000017f0: 7465 7874 3a20 4f70 7469 6f6e 616c 5b73  text: Optional[s
+00001800: 7472 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  tr] = None,..   
+00001810: 2020 2020 2020 2020 2061 6e73 7765 725f           answer_
+00001820: 7368 6f77 5f61 6c65 7274 3a20 626f 6f6c  show_alert: bool
+00001830: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+00001840: 2020 2020 2020 2061 7574 6f61 6e73 7765         autoanswe
+00001850: 723a 2062 6f6f 6c20 3d20 5472 7565 0d0a  r: bool = True..
+00001860: 2020 2020 2920 2d3e 2055 6e69 6f6e 5b4d      ) -> Union[M
+00001870: 6573 7361 6765 2c20 626f 6f6c 5d3a 0d0a  essage, bool]:..
+00001880: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00001890: 2020 2020 2053 6d61 7274 2065 6469 7420       Smart edit 
+000018a0: 6d65 6e61 6765 720d 0a20 2020 2020 2020  menager..       
+000018b0: 203a 7061 7261 6d20 7465 7874 3a0d 0a20   :param text:.. 
+000018c0: 2020 2020 2020 203a 7061 7261 6d20 7068         :param ph
+000018d0: 6f74 6f3a 0d0a 2020 2020 2020 2020 3a70  oto:..        :p
+000018e0: 6172 616d 2076 6964 656f 3a0d 0a20 2020  aram video:..   
+000018f0: 2020 2020 203a 7061 7261 6d20 7265 706c       :param repl
+00001900: 795f 6d61 726b 7570 3a0d 0a20 2020 2020  y_markup:..     
+00001910: 2020 203a 7061 7261 6d20 7061 7273 655f     :param parse_
+00001920: 6d6f 6465 3a0d 0a20 2020 2020 2020 203a  mode:..        :
+00001930: 7061 7261 6d20 6469 7361 626c 655f 7765  param disable_we
+00001940: 625f 7061 6765 5f70 7265 7669 6577 3a0d  b_page_preview:.
+00001950: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001960: 616e 7377 6572 5f74 6578 743a 0d0a 2020  answer_text:..  
+00001970: 2020 2020 2020 3a70 6172 616d 2061 6e73        :param ans
+00001980: 7765 725f 7368 6f77 5f61 6c65 7274 3a0d  wer_show_alert:.
+00001990: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000019a0: 6175 746f 616e 7377 6572 3a0d 0a20 2020  autoanswer:..   
+000019b0: 2020 2020 203a 7265 7475 726e 3a0d 0a20       :return:.. 
+000019c0: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
+000019d0: 2020 2020 2020 6361 6c6c 6261 636b 203d        callback =
+000019e0: 2073 656c 662e 5f63 616c 6c62 6163 6b0d   self._callback.
+000019f0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+00001a00: 203d 2063 616c 6c62 6163 6b2e 6d65 7373   = callback.mess
+00001a10: 6167 650d 0a0d 0a20 2020 2020 2020 2069  age....        i
+00001a20: 6620 6d65 7373 6167 6520 6973 204e 6f6e  f message is Non
+00001a30: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001a40: 6177 6169 7420 6361 6c6c 6261 636b 2e61  await callback.a
+00001a50: 6e73 7765 7228 224d 6573 7361 6765 2074  nswer("Message t
+00001a60: 6f6f 206f 6c64 2229 0d0a 0d0a 2020 2020  oo old")....    
+00001a70: 2020 2020 2020 2020 7261 6973 6520 4d65          raise Me
+00001a80: 7373 6167 6554 6f6f 4f6c 640d 0a0d 0a20  ssageTooOld.... 
+00001a90: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00001aa0: 7374 6162 6c65 3a0d 0a20 2020 2020 2020  stable:..       
+00001ab0: 2020 2020 2061 7761 6974 2061 7379 6e63       await async
+00001ac0: 696f 2e73 6c65 6570 2873 656c 662e 5f67  io.sleep(self._g
+00001ad0: 6574 5f73 7461 626c 655f 7761 6974 5f74  et_stable_wait_t
+00001ae0: 696d 6528 6d65 7373 6167 6529 290d 0a0d  ime(message))...
+00001af0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00001b00: 7365 6c66 2e5f 6765 745f 6461 7461 5f63  self._get_data_c
+00001b10: 6861 6e67 6573 5f73 7461 7475 7328 0d0a  hanges_status(..
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b30: 6d65 7373 6167 653d 6d65 7373 6167 652c  message=message,
+00001b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001b50: 2020 7465 7874 3d74 6578 742c 0d0a 2020    text=text,..  
+00001b60: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00001b70: 706c 795f 6d61 726b 7570 3d72 6570 6c79  ply_markup=reply
+00001b80: 5f6d 6172 6b75 702c 0d0a 2020 2020 2020  _markup,..      
+00001b90: 2020 2020 2020 2020 2020 7669 6465 6f3d            video=
+00001ba0: 7669 6465 6f2c 0d0a 2020 2020 2020 2020  video,..        
+00001bb0: 2020 2020 2020 2020 7068 6f74 6f3d 7068          photo=ph
+00001bc0: 6f74 6f0d 0a20 2020 2020 2020 2029 3a0d  oto..        ):.
+00001bd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00001be0: 7572 6e20 6d65 7373 6167 650d 0a0d 0a20  urn message.... 
+00001bf0: 2020 2020 2020 2063 616e 5f65 6469 7420         can_edit 
+00001c00: 3d20 7365 6c66 2e5f 6765 745f 6361 6e5f  = self._get_can_
+00001c10: 6564 6974 5f73 7461 7475 7328 0d0a 2020  edit_status(..  
+00001c20: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00001c30: 653d 6d65 7373 6167 652c 0d0a 2020 2020  e=message,..    
+00001c40: 2020 2020 2020 2020 7068 6f74 6f3d 7068          photo=ph
+00001c50: 6f74 6f2c 0d0a 2020 2020 2020 2020 2020  oto,..          
+00001c60: 2020 7669 6465 6f3d 7669 6465 6f2c 0d0a    video=video,..
+00001c70: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
+00001c80: 2020 2020 2072 6573 756c 7420 3d20 6177       result = aw
+00001c90: 6169 7420 7365 6c66 2e5f 7365 6e64 5f6f  ait self._send_o
+00001ca0: 725f 6564 6974 280d 0a20 2020 2020 2020  r_edit(..       
+00001cb0: 2020 2020 2062 6f74 3d73 656c 662e 5f62       bot=self._b
+00001cc0: 6f74 2c0d 0a20 2020 2020 2020 2020 2020  ot,..           
+00001cd0: 2063 616e 5f65 6469 743d 6361 6e5f 6564   can_edit=can_ed
+00001ce0: 6974 2c0d 0a20 2020 2020 2020 2020 2020  it,..           
+00001cf0: 206d 6573 7361 6765 3d6d 6573 7361 6765   message=message
+00001d00: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00001d10: 6578 743d 7465 7874 2c0d 0a20 2020 2020  ext=text,..     
+00001d20: 2020 2020 2020 2070 686f 746f 3d70 686f         photo=pho
+00001d30: 746f 2c0d 0a20 2020 2020 2020 2020 2020  to,..           
+00001d40: 2076 6964 656f 3d76 6964 656f 2c0d 0a20   video=video,.. 
+00001d50: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+00001d60: 5f6d 6172 6b75 703d 7265 706c 795f 6d61  _markup=reply_ma
+00001d70: 726b 7570 2c0d 0a20 2020 2020 2020 2020  rkup,..         
+00001d80: 2020 2070 6172 7365 5f6d 6f64 653d 7061     parse_mode=pa
+00001d90: 7273 655f 6d6f 6465 2c0d 0a20 2020 2020  rse_mode,..     
+00001da0: 2020 2020 2020 2064 6973 6162 6c65 5f77         disable_w
+00001db0: 6562 5f70 6167 655f 7072 6576 6965 773d  eb_page_preview=
+00001dc0: 6469 7361 626c 655f 7765 625f 7061 6765  disable_web_page
+00001dd0: 5f70 7265 7669 6577 2c0d 0a20 2020 2020  _preview,..     
+00001de0: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+00001df0: 6177 6169 7420 4361 6c6c 6261 636b 416e  await CallbackAn
+00001e00: 7377 6572 2e61 7574 6f5f 6361 6c6c 6261  swer.auto_callba
+00001e10: 636b 5f61 6e73 7765 7228 0d0a 2020 2020  ck_answer(..    
+00001e20: 2020 2020 2020 2020 626f 743d 7365 6c66          bot=self
+00001e30: 2e5f 626f 742c 0d0a 2020 2020 2020 2020  ._bot,..        
+00001e40: 2020 2020 6361 6c6c 6261 636b 5f69 643d      callback_id=
+00001e50: 6361 6c6c 6261 636b 2e69 642c 0d0a 2020  callback.id,..  
+00001e60: 2020 2020 2020 2020 2020 6175 746f 616e            autoan
+00001e70: 7377 6572 3d61 7574 6f61 6e73 7765 722c  swer=autoanswer,
+00001e80: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+00001e90: 7377 6572 5f74 6578 743d 616e 7377 6572  swer_text=answer
+00001ea0: 5f74 6578 742c 0d0a 2020 2020 2020 2020  _text,..        
+00001eb0: 2020 2020 616e 7377 6572 5f73 686f 775f      answer_show_
+00001ec0: 616c 6572 743d 616e 7377 6572 5f73 686f  alert=answer_sho
+00001ed0: 775f 616c 6572 740d 0a20 2020 2020 2020  w_alert..       
+00001ee0: 2029 0d0a 0d0a 2020 2020 2020 2020 7265   )....        re
+00001ef0: 7475 726e 2072 6573 756c 740d 0a         turn result..
```

### Comparing `usefulgram-0.0.0a9/usefulgram/lazy/sender.py` & `usefulgram-0.0.0b1/usefulgram/lazy/sender.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a9/usefulgram/middlewares/trottling.py` & `usefulgram-0.0.0b1/usefulgram/middlewares/trottling.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a9/usefulgram/parsing/encode.py` & `usefulgram-0.0.0b1/usefulgram/parsing/encode.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,25 +5,33 @@
 from typing import Any
 
 from enum import Enum
 from decimal import Decimal
 
 from datetime import date, time, datetime
 
-from usefulgram.exceptions import TooMoreCharacters, RecursionObjectParse
+from pydantic import BaseModel
+
+from usefulgram.exceptions import TooMoreCharacters
 from usefulgram.enums import Const
 
 
 class _Additional:
     @staticmethod
     def _add_separator(item: str, separator: str = "&") -> str:
         return f"{item}{separator}"
 
     def _object_to_str(self, item: object) -> str:
-        annotations_keys = list(item.__annotations__.keys())
+        if isinstance(item, BaseModel):
+            fields = item.model_fields
+
+        else:
+            fields = item.__annotations__
+
+        annotations_keys = list(fields.keys())
 
         result = ""
 
         for key in annotations_keys:
             if key == "prefix":
                 continue
 
@@ -51,15 +59,15 @@
         if isinstance(item, (datetime, date, time)):
             return item.strftime(Const.DATETIME_FORMAT)
 
         if isinstance(item, Enum):
             return item.name
 
         if is_recursion:
-            raise RecursionObjectParse
+            return self._object_to_str(item)
 
         try:
             return self._object_to_str(item)
 
         except AttributeError:
             return f"{item}"
```

