# Comparing `tmp/python-negar-1.2.5.tar.gz` & `tmp/python-negar-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-negar-1.2.5.tar", last modified: Fri Jul 14 10:08:12 2023, max compression
+gzip compressed data, was "python-negar-1.2.6.tar", last modified: Mon Aug  7 07:26:47 2023, max compression
```

## Comparing `python-negar-1.2.5.tar` & `python-negar-1.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-07-14 10:08:12.206168 python-negar-1.2.5/
--rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2.5/AUTHORS
--rw-r--r--   0 javad     (1000) javad     (1000)     6863 2023-07-14 08:12:22.000000 python-negar-1.2.5/Changelog.txt
--rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2.5/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1000)      125 2023-06-15 16:17:35.000000 python-negar-1.2.5/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-07-14 10:08:12.206168 python-negar-1.2.5/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2.5/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-07-14 10:08:12.206168 python-negar-1.2.5/negar/
--rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2.5/negar/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)     5047 2023-07-14 08:12:53.000000 python-negar-1.2.5/negar/constants.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-07-14 10:08:12.206168 python-negar-1.2.5/negar/data/
--rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2.5/negar/data/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2.5/negar/data/untouchable.dat
--rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2.5/negar/gui.py
--rw-r--r--   0 javad     (1000) javad     (1000)    15106 2023-07-14 10:03:34.000000 python-negar-1.2.5/negar/virastar.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-07-14 10:08:12.206168 python-negar-1.2.5/python_negar.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)      396 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       42 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/entry_points.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/requires.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-07-14 10:08:12.206168 python-negar-1.2.5/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1000)     1541 2022-05-30 08:43:57.000000 python-negar-1.2.5/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-08-07 07:26:47.974760 python-negar-1.2.6/
+-rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2.6/AUTHORS
+-rw-r--r--   0 javad     (1000) javad     (1000)     6962 2023-08-07 07:23:03.000000 python-negar-1.2.6/Changelog.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2.6/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1000)      125 2023-06-15 16:17:35.000000 python-negar-1.2.6/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-08-07 07:26:47.974760 python-negar-1.2.6/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2.6/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-08-07 07:26:47.974760 python-negar-1.2.6/negar/
+-rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2.6/negar/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     5164 2023-08-07 07:22:13.000000 python-negar-1.2.6/negar/constants.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-08-07 07:26:47.974760 python-negar-1.2.6/negar/data/
+-rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2.6/negar/data/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2.6/negar/data/untouchable.dat
+-rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2.6/negar/gui.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    15255 2023-08-06 20:42:54.000000 python-negar-1.2.6/negar/virastar.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-08-07 07:26:47.974760 python-negar-1.2.6/python_negar.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-08-07 07:26:47.000000 python-negar-1.2.6/python_negar.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)      396 2023-08-07 07:26:47.000000 python-negar-1.2.6/python_negar.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-08-07 07:26:47.000000 python-negar-1.2.6/python_negar.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       42 2023-08-07 07:26:47.000000 python-negar-1.2.6/python_negar.egg-info/entry_points.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-08-07 07:26:47.000000 python-negar-1.2.6/python_negar.egg-info/requires.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-08-07 07:26:47.000000 python-negar-1.2.6/python_negar.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-08-07 07:26:47.974760 python-negar-1.2.6/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1000)     1543 2023-08-06 20:39:57.000000 python-negar-1.2.6/setup.py
```

### Comparing `python-negar-1.2.5/Changelog.txt` & `python-negar-1.2.6/Changelog.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+1.2.6 - 2023-08-07
+-- Better location for saving user defined untouchable data under Windows OS. 
+
 1.2.5 - 2023-07-14
 -- Fix issues with texts that include backslashes as part of their context, such as LaTeX source code.
 
 1.2.4 - 2023-06-15
 -- Fix the issue with multiple ! and ? and extra space after parantheses at the end of line
 
 1.2.2 - 2023-06-13
```

### Comparing `python-negar-1.2.5/LICENSE` & `python-negar-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.5/PKG-INFO` & `python-negar-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2.5
+Version: 1.2.6
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2.5/README.md` & `python-negar-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.5/negar/constants.py` & `python-negar-1.2.6/negar/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import platform
 from pathlib import Path
 
-__version__ = "1.2.5"
+__version__ = "1.2.6"
 
 DATAFILE = Path(__file__).parent.absolute() / "data/untouchable.dat"
-USERFILE = Path.home() / ".python-negar"
+APPDATA = "AppData/Roaming/" if platform.system() == "Windows" else ""
+USERFILE = Path.home() / f"{APPDATA}.python-negar"
 
 INFO = f"""قابلیت های ویراستار ' نگار  ' -- نسخه {__version__} :
 * جایگزینی
 	╛═ خط تیره های پیاپی نظیر (--) و (---) با معادل های استاندارد شان
 	╛═ سه نقطه ی پیاپی (...) با کاراکتر استانداردش در زبان فارسی
 	╛═ علایمی نظیر کتیشن فارسی با گیومه ؛  'نگار'
 	╛═ اعداد عربی '١٢٣٤٥٦٧٨٩٠' و انگلیسی '1234567890'  با معادل فارسی
@@ -28,18 +30,18 @@
 (							# Capture 1: entire matched URL
   (?:
     https?|ftp:				# URL protocol and colon
     (?:
       /{1,3}						# 1-3 slashes
       |								#   or
       [a-z0-9%]						# Single letter or digit or '%'
-      								# (Trying not to match e.g. "URI::Escape")
+                          # (Trying not to match e.g. "URI::Escape")
     )
     |							#   or
-    							# looks like domain name followed by a slash:
+                  # looks like domain name followed by a slash:
     [a-z0-9.\-]+[.]
     (?:[a-z]{2,4}) #com|net|org|edu|gov|mil|aero|asia|biz|cat|coop|info|int|jobs|mobi|museum|name|post|pro|tel|travel|xxx|io|ac|ad|ae|af|ag|ai|al|am|an|ao|aq|ar|as|at|au|aw|ax|az|ba|bb|bd|be|bf|bg|bh|bi|bj|bm|bn|bo|br|bs|bt|bv|bw|by|bz|ca|cc|cd|cf|cg|ch|ci|ck|cl|cm|cn|co|cr|cs|cu|cv|cx|cy|cz|dd|de|dj|dk|dm|do|dz|ec|ee|eg|eh|er|es|et|eu|fi|fj|fk|fm|fo|fr|ga|gb|gd|ge|gf|gg|gh|gi|gl|gm|gn|gp|gq|gr|gs|gt|gu|gw|gy|hk|hm|hn|hr|ht|hu|id|ie|il|im|in|io|iq|ir|is|it|je|jm|jo|jp|ke|kg|kh|ki|km|kn|kp|kr|kw|ky|kz|la|lb|lc|li|lk|lr|ls|lt|lu|lv|ly|ma|mc|md|me|mg|mh|mk|ml|mm|mn|mo|mp|mq|mr|ms|mt|mu|mv|mw|mx|my|mz|na|nc|ne|nf|ng|ni|nl|no|np|nr|nu|nz|om|pa|pe|pf|pg|ph|pk|pl|pm|pn|pr|ps|pt|pw|py|qa|re|ro|rs|ru|rw|sa|sb|sc|sd|se|sg|sh|si|sj| Ja|sk|sl|sm|sn|so|sr|ss|st|su|sv|sx|sy|sz|tc|td|tf|tg|th|tj|tk|tl|tm|tn|to|tp|tr|tt|tv|tw|tz|ua|ug|uk|us|uy|uz|va|vc|ve|vg|vi|vn|vu|wf|ws|ye|yt|yu|za|zm|zw)
     [/?]
   )
   (?:							# One or more:
     [^\s()<>{}\[\]]+						# Run of non-space, non-()<>{}[]
     |								#   or
@@ -52,15 +54,15 @@
     |
     \([^\s]+?\)							# balanced parens, non-recursive: (…)
     |									#   or
     [^\s`!()\[\]{};:'".,<>?«»“”‘’]		# not a space or one of these punct chars
   )
   |					# OR, the following to match naked domains:
   (?:
-  	(?<!@)			# not preceded by a @, avoid matching foo@_gmail.com_
+    (?<!@)			# not preceded by a @, avoid matching foo@_gmail.com_
     [a-z0-9]+
     (?:[.\-][a-z0-9]+)*
     [.]
     (?:[a-z]{2,4}) #com|net|org|edu|gov|mil|aero|asia|biz|cat|coop|info|int|jobs|mobi|museum|name|post|pro|tel|travel|xxx|ac|ad|ae|af|ag|ai|al|am|an|ao|aq|ar|as|at|au|aw|ax|az|ba|bb|bd|be|bf|bg|bh|bi|bj|bm|bn|bo|br|bs|bt|bv|bw|by|bz|ca|cc|cd|cf|cg|ch|ci|ck|cl|cm|cn|co|cr|cs|cu|cv|cx|cy|cz|dd|de|dj|dk|dm|do|dz|ec|ee|eg|eh|er|es|et|eu|fi|fj|fk|fm|fo|fr|ga|gb|gd|ge|gf|gg|gh|gi|gl|gm|gn|gp|gq|gr|gs|gt|gu|gw|gy|hk|hm|hn|hr|ht|hu|id|ie|il|im|in|io|iq|ir|is|it|je|jm|jo|jp|ke|kg|kh|ki|km|kn|kp|kr|kw|ky|kz|la|lb|lc|li|lk|lr|ls|lt|lu|lv|ly|ma|mc|md|me|mg|mh|mk|ml|mm|mn|mo|mp|mq|mr|ms|mt|mu|mv|mw|mx|my|mz|na|nc|ne|nf|ng|ni|nl|no|np|nr|nu|nz|om|pa|pe|pf|pg|ph|pk|pl|pm|pn|pr|ps|pt|pw|py|qa|re|ro|rs|ru|rw|sa|sb|sc|sd|se|sg|sh|si|sj| Ja|sk|sl|sm|sn|so|sr|ss|st|su|sv|sx|sy|sz|tc|td|tf|tg|th|tj|tk|tl|tm|tn|to|tp|tr|tt|tv|tw|tz|ua|ug|uk|us|uy|uz|va|vc|ve|vg|vi|vn|vu|wf|ws|ye|yt|yu|za|zm|zw)
     \b
     /?
     (?!@)			# not succeeded by a @, avoid matching "foo.na" in "foo.na@example.com"
```

### Comparing `python-negar-1.2.5/negar/data/untouchable.dat` & `python-negar-1.2.6/negar/data/untouchable.dat`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.5/negar/virastar.py` & `python-negar-1.2.6/negar/virastar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,304 +1,312 @@
 #!/usr/bin/env python
 
+import enum
 import re
-import regex
 import sys
-import enum
 from pathlib import Path
+
+import regex
+
 sys.path.append(Path(__file__).parent.parent.as_posix()) # https://stackoverflow.com/questions/16981921
-from negar.constants import DATAFILE, USERFILE, URLREGX, INFO
+from negar.constants import DATAFILE, INFO, URLREGX, USERFILE # noqa: E402
+
 
 class State(enum.Enum):
     save = 1
     restore = 2
 
 class PersianEditor:
-    """
-    Persian Text Editor for some sanitiztion task called Virastary in Persian
-    """
+    """Persian Text Editor for some sanitiztion task called Virastary in Persian."""
 
     def __init__(self, text, *args):
         # Check to see if `arg` exists in `args` or not
-        parse_args = lambda arg: arg not in args
-        self._prepositions = "از|در|به|با|بر|برای|بی|درباره|تا|را|جز|بدون|چون|مانند|مثل|زیر|روی|همراه|مگر|الا|اندر|زی|برت|الا|زی|چو|سوای|پایین|پشت|پهلوی|پس|پیش|بالای|بیرون|درون|توی|غیر|کنار|مقابل|بهر"
+        parse_args = lambda arg: arg not in args # noqa: E731
+        self._prepositions = \
+            "از|در|به|با|بر|برای|بی|درباره|تا|را|جز|بدون|چون|مانند|مثل" \
+            "|زیر|روی|همراه|مگر|الا|اندر|زی|برت|الا|زی|چو|سوای|پایین" \
+            "|پشت|پهلوی|پس|پیش|بالای|بیرون|درون|توی|غیر|کنار|مقابل|بهر"
         self.text = text
         self._cleanup_zwnj                      = False
         # checking for undesired options
-        self._aggresive                         = parse_args('aggresive')
-        self._fix_hamzeh                        = parse_args('fix-hamzeh')
-        self._fix_dashes                        = parse_args('fix-dashes')
-        self._fix_three_dots                    = parse_args('fix-three-dots')
-        self._hamzeh_with_yeh                   = parse_args('hamzeh-with-yeh')
-        self._fix_prefix_spacing                = parse_args('fix-p-spacing')
-        self._fix_prefix_separate               = parse_args('fix-p-separate')
-        self._fix_suffix_spacing                = parse_args('fix-s-spacing')
-        self._fix_suffix_separate               = parse_args('fix-s-separate')
-        self._fix_english_quotes                = parse_args('fix-english-quotes')
-        self._fix_arabic_numbers                = parse_args('fix-arabic-num')
-        self._fix_english_numbers               = parse_args('fix-english-num')
-        self._cleanup_spacing                   = parse_args('cleanup-spacing')
-        self._cleanup_kashidas                  = parse_args('cleanup-kashidas')
-        self._cleanup_extra_marks               = parse_args('cleanup-ex-marks')
-        self._exaggerating_zwnj                 = parse_args('exaggerating-zwnj')
-        self._fix_misc_non_persian_chars        = parse_args('fix-non-persian-chars')
-        self._fix_spacing_for_braces_and_quotes = parse_args('fix-spacing-bq')
-        self._trim_leading_trailing_whitespaces = parse_args('trim-lt-whitespaces')
+        self._aggresive                         = parse_args("aggresive")
+        self._fix_hamzeh                        = parse_args("fix-hamzeh")
+        self._fix_dashes                        = parse_args("fix-dashes")
+        self._fix_three_dots                    = parse_args("fix-three-dots")
+        self._hamzeh_with_yeh                   = parse_args("hamzeh-with-yeh")
+        self._fix_prefix_spacing                = parse_args("fix-p-spacing")
+        self._fix_prefix_separate               = parse_args("fix-p-separate")
+        self._fix_suffix_spacing                = parse_args("fix-s-spacing")
+        self._fix_suffix_separate               = parse_args("fix-s-separate")
+        self._fix_english_quotes                = parse_args("fix-english-quotes")
+        self._fix_arabic_numbers                = parse_args("fix-arabic-num")
+        self._fix_english_numbers               = parse_args("fix-english-num")
+        self._cleanup_spacing                   = parse_args("cleanup-spacing")
+        self._cleanup_kashidas                  = parse_args("cleanup-kashidas")
+        self._cleanup_extra_marks               = parse_args("cleanup-ex-marks")
+        self._exaggerating_zwnj                 = parse_args("exaggerating-zwnj")
+        self._fix_misc_non_persian_chars        = parse_args("fix-non-persian-chars")
+        self._fix_spacing_for_braces_and_quotes = parse_args("fix-spacing-bq")
+        self._trim_leading_trailing_whitespaces = parse_args("trim-lt-whitespaces")
 
         UnTouchable() # to generate the untouchable words
         self.cleanup()
 
     def cleanup(self):
         self._handle_urls(State.save)
         # fix punctuation spaces at first
         # : ; , ! ? and their Persian counterparts should have one space after and no space before
         # An exception is triple dots, which should be handled first
         self.fix_three_dots()       if self._fix_three_dots else None
         self.aggressive()           if self._aggresive else None
         self.text = re.sub(
-            r'[ ‌ ]*([:;,؛،.؟!]{1})[ ‌ ]*',
-            r'\1 ',
-            self.text
+            r"[ ‌ ]*([:;,؛،.؟!]{1})[ ‌ ]*",
+            r"\1 ",
+            self.text,
         )
         if self._trim_leading_trailing_whitespaces:
-            self.text = '\n'.join([line.strip() for line in self.text.split('\n')])
+            self.text = "\n".join([line.strip() for line in self.text.split("\n")])
         self.fix_dashes()           if self._fix_dashes else None
         self.fix_english_quotes()   if self._fix_english_quotes else None
         self.fix_hamzeh()           if self._fix_hamzeh else None
         self.cleanup_zwnj()         if self._cleanup_zwnj else None
         self.char_validator()       if self._fix_misc_non_persian_chars else None
         self.fix_arabic_numbers()   if self._fix_arabic_numbers else None
         self.fix_english_numbers()  if self._fix_english_numbers else None
         self.fix_prefix_spacing()   if self._fix_prefix_spacing else None
         self.fix_prefix_separate()  if self._fix_prefix_separate else None
         self.fix_suffix_spacing()   if self._fix_suffix_spacing else None
         self.fix_suffix_separate()  if self._fix_suffix_separate else None
-        self.fix_spacing_for_braces_and_quotes() if self._fix_spacing_for_braces_and_quotes else None
+        self.fix_spacing_for_braces_and_quotes() \
+            if self._fix_spacing_for_braces_and_quotes else None
         self.cleanup_redundant_zwnj()
         self.cleanup_spacing()      if self._cleanup_spacing else None
         self._handle_urls(State.restore)
         return self.text
 
     def __repr__(self):
         return self.text
 
     __str__ = __repr__
 
     def _handle_urls(self, state):
-        """Removing URLs and putting them back at the end of the process"""
+        """Remove URLs and putting them back at the end of the process."""
         if state == State.save:
             self.urls = list(set(re.findall(URLREGX, self.text, re.M|re.I|re.X)))
             self.urls.sort(key=lambda x: len(x), reverse=True)
             for i, url in enumerate(self.urls):
-                self.text = regex.sub(rf"{re.escape(url)}", rf'__URL__#{i}__', self.text)
+                self.text = regex.sub(rf"{re.escape(url)}", rf"__URL__#{i}__", self.text)
         if state == State.restore:
             for i, url in enumerate(self.urls):
-                self.text = re.sub(f'__URL__#{i}__', url, self.text)
+                self.text = re.sub(f"__URL__#{i}__", url, self.text)
 
     def fix_dashes(self):
-        """Replaces double and triple dashes with `ndash` and `mdash`, respectively."""
-        self.text = re.sub(r'-{3}', r'—', self.text)
-        self.text = re.sub(r'-{2}', r'–', self.text)
+        """Replace double and triple dashes with `ndash` and `mdash`, respectively."""
+        self.text = re.sub(r"-{3}", r"—", self.text)
+        self.text = re.sub(r"-{2}", r"–", self.text)
 
     def fix_three_dots(self):
-        """Replaces three dots with an ellipsis."""
-        self.text = re.sub(r'\s*\.{3,}', r'…', self.text)
+        """Replace three dots with an ellipsis."""
+        self.text = re.sub(r"\s*\.{3,}", r"…", self.text)
 
     def fix_english_quotes(self):
-        """Replaces English quotes with their Persian counterparts."""
-        self.text = re.sub(r"([\"'`]+)(.+?)(\1)", r'«\2»', self.text)
+        """Replace English quotes with their Persian counterparts."""
+        self.text = re.sub(r"([\"'`]+)(.+?)(\1)", r"«\2»", self.text)
 
     def fix_hamzeh(self):
-        """Replaces trailing 'ه ی' with 'هٔ' or 'ه‌ی'--the last one is achievable if hamzeh_with_yeh set."""
+        """Replace trailing 'ه ی' with 'هٔ' or 'ه‌ی'.
+
+        --the last one is achievable if hamzeh_with_yeh set.
+        """
         if self._hamzeh_with_yeh:
-            self.text = re.sub(r'(\S)(ه[\s]+[یي])(\b)',r'\1ه‌ی\3',self.text)
+            self.text = re.sub(r"(\S)(ه[\s]+[یي])(\b)",r"\1ه‌ی\3",self.text)
         else:
-            self.text = re.sub(r'(\S)(ه[\s]+[یي])(\b)',r'\1هٔ\3', self.text)
+            self.text = re.sub(r"(\S)(ه[\s]+[یي])(\b)",r"\1هٔ\3", self.text)
 
     def cleanup_zwnj(self):
-        """Removes unnecessary ZWNJ that are succeeded/preceded by a space."""
-        self.text = re.sub(r'\s+|\s+', r' ', self.text)
+        """Remove unnecessary ZWNJ that are succeeded/preceded by a space."""
+        self.text = re.sub(r"\s+|\s+", r" ", self.text)
 
     def cleanup_redundant_zwnj(self):
-        """Removes unwanted ZWNJs which are added by some sanitization tasks."""
-        self.text = re.sub(r'([ءاأدذرزژوؤ])‌+', r'\1', self.text)
-        self.text = re.sub(r'(‌)+', r'\1', self.text)
+        """Remove unwanted ZWNJs which are added by some sanitization tasks."""
+        self.text = re.sub(r"([ءاأدذرزژوؤ])‌+", r"\1", self.text)
+        self.text = re.sub(r"(‌)+", r"\1", self.text)
 
     def char_validator(self):
-        """Replaces invalid characters with valid ones."""
+        """Replace invalid characters with valid ones."""
         bad_chars  = ",;%يةك"
         good_chars = "،؛٪یهک"
         self.text = self.char_translator(bad_chars, good_chars, self.text)
 
     def fix_arabic_numbers(self):
-        """Translates Arabic numbers to their Persian counterparts."""
+        """Translate Arabic numbers to their Persian counterparts."""
         persian_numbers = "۱۲۳۴۵۶۷۸۹۰"
         arabic_numbers = "١٢٣٤٥٦٧٨٩٠"
         self.text = self.char_translator(
             arabic_numbers,
             persian_numbers,
-            self.text
+            self.text,
         )
 
     def fix_english_numbers(self):
-        """Translates English numbers to their Persian counterparts."""
+        """Translate English numbers to their Persian counterparts."""
         persian_numbers = "۱۲۳۴۵۶۷۸۹۰"
         english_numbers = "1234567890"
         self.text = self.char_translator(
             english_numbers,
             persian_numbers,
-            self.text
+            self.text,
         )
 
         # Avoids to change English numbers in strings like 'Text12', 'Text_12', or 'A4'
         self.text = re.sub(
-            r'[۰-۹]+[a-zA-Z_]{1,}[۰-۹]+|[a-zA-Z_]{1,}[۰-۹]+|[۰-۹]+[a-zA-Z_]{1,}',
+            r"[۰-۹]+[a-zA-Z_]{1,}[۰-۹]+|[a-zA-Z_]{1,}[۰-۹]+|[۰-۹]+[a-zA-Z_]{1,}",
             lambda m:
             self.char_translator(persian_numbers, english_numbers, m.group()),
-            self.text
+            self.text,
         )
 
     def fix_prefix_spacing(self):
-        """Puts ZWNJ between a word and its prefix (mi* nemi* bi* na*)"""
-        self.text = re.sub(r"\b(بی|نا)‌*(\s+)(?!(می)\b)",r'\1‌', self.text)
+        """Put ZWNJ between a word and its prefix (mi* nemi* bi* na*)."""
+        self.text = re.sub(r"\b(بی|نا)‌*(\s+)(?!(می)\b)",r"\1‌", self.text)
         # the following case is for the mi(n.) and nami(n.)
-        self.text = re.sub(rf"\b(ن?می)‌*(\s+)(?!(.|{self._prepositions})\b)",r'\1‌', self.text)
+        self.text = re.sub(rf"\b(ن?می)‌*(\s+)(?!(.|{self._prepositions})\b)",r"\1‌", self.text)
 
     def fix_prefix_separate(self):
-        """Puts ZWNJ between a word and its prefix (mi* nemi* bi*)"""
+        """Put ZWNJ between a word and its prefix (mi* nemi* bi*)."""
         # regx = re.compile(r"\b(بی|ن?می)‌*([^\[\]\(\)\s]+)") #  \b for words like سهمیه
         regx = regex.compile(r"""
         \b(بی|ن?می)‌*
         ([^\[\]\(\)\s]+)
         (?<!های|هایی|ها|شناس|شناسی|گذار|گذاری)\b
         """, re.VERBOSE) #  \b for words like سهمیه
 
         # Replace backslashes with a temporary placeholder
-        text = self.text.replace('\\', 'PN__BACKSLASH__PN')
+        text = self.text.replace("\\", "PN__BACKSLASH__PN")
         wlist = text.split(" ")
         for word in wlist:
             regx_iter = regx.finditer(word)
             for p in regx_iter:
                 # Checks that the prefix (mi* nemi* bi*) is part a a word or not, like میلاد.
                 if p.group() not in UnTouchable.words:
                     text = re.sub(
                         re.escape( p.group() ),
                         p.group(1) + "\u200c" + p.group(2) ,
-                        text
+                        text,
                     )
         # Restore the original backslashes
-        self.text = text.replace('PN__BACKSLASH__PN', '\\')
+        self.text = text.replace("PN__BACKSLASH__PN", "\\")
 
     def fix_suffix_spacing(self):
-        """Puts ZWNJ between a word and its suffix (*ha[ye] *tar[in])"""
+        """Put ZWNJ between a word and its suffix (*ha[ye] *tar[in])."""
         regx = re.compile(
             r"""\s+
             (تر(ی(ن)?)?
             |[تمش]ان
             |ا[متش]
             |ا((ی(م|د)?)|ند)
             |ها(ی(ی|ت|م|ش|تان|شان)?)?
             |شناس(ی)?
             |گذار(ی)?|گزار(ی)?
             |مند|ور|پور
-            )\b""", re.VERBOSE
+            )\b""", re.VERBOSE,
         )
-        self.text = re.sub(regx, r'‌\1', self.text)
+        self.text = re.sub(regx, r"‌\1", self.text)
 
         # Some special cases like و شان خود
         regx = re.compile(r"\b(\w)‌([تمش]ان)\b", re.VERBOSE)
-        self.text = re.sub(regx, r'\1 \2', self.text)
+        self.text = re.sub(regx, r"\1 \2", self.text)
 
         # Ash(=اش) at the end of some words like خانه‌اش or پایانی‌اش
         regx = re.compile(r"\b(\w+)(ه|ی)\s+(اش)\b", re.VERBOSE)
-        self.text = re.sub(regx, r'\1\2‌\3', self.text)
+        self.text = re.sub(regx, r"\1\2‌\3", self.text)
 
     def fix_suffix_separate(self):
-        """Puts ZWNJ between a word with its suffix (haye, ...)"""
+        """Put ZWNJ between a word with its suffix (haye, ...)."""
         exag = r"""
             تر(ی(ن)?)?|
             [تمش]ان|
-            ها(ی(ی|ت|م|ش|تان|شان)?)?|""" if self._exaggerating_zwnj else ''
+            ها(ی(ی|ت|م|ش|تان|شان)?)?|""" if self._exaggerating_zwnj else ""
         regx = re.compile(
             rf"""(\S+?) # not-greedy fetch to handle some case like هایشان instead شان
             ({exag}
             # تر(ی(ن)?)?
             # [تمش]ان|
             # ها(ی(ی|ت|م|ش|تان|شان)?)?|
             شناس(ی)?|
             گذار(ی)?|گزار(ی)?
-            )\b""", re.VERBOSE
+            )\b""", re.VERBOSE,
         )
         # Replace backslashes with a temporary placeholder
-        text = self.text.replace('\\', 'PN__BACKSLASH__PN')
+        text = self.text.replace("\\", "PN__BACKSLASH__PN")
         wlist = text.split(" ")
         for word in wlist:
             regx_iter = regx.finditer(word)
             for p in regx_iter:
                 # Checks that the suffix (tar* haye*) is part of a word or not, like بهتر.
                 if p.group() not in UnTouchable.words:
                     text = re.sub(
                         re.escape( p.group() ),
-                        p.group(1) + "\u200c" + p.group(2) ,
-                        text
+                        p.group(1) + "\u200c" + p.group(2),
+                        text,
                     )
         # Restore the original backslashes
-        self.text = text.replace('PN__BACKSLASH__PN', '\\')
+        self.text = text.replace("PN__BACKSLASH__PN", "\\")
 
     def aggressive(self):
-        """Reduces Aggressive Punctuation to one sign."""
+        """Reduce Aggressive Punctuation to one sign."""
         if self._cleanup_extra_marks:
-            self.text = re.sub(r'(؟){2,}', r'\1', self.text)
-            self.text = re.sub(r'(!){2,}', r'\1', self.text)
+            self.text = re.sub(r"(؟){2,}", r"\1", self.text)
+            self.text = re.sub(r"(!){2,}", r"\1", self.text)
 
         if self._cleanup_kashidas:
-            self.text = re.sub(r'ـ+', "", self.text)
+            self.text = re.sub(r"ـ+", "", self.text)
 
     def fix_spacing_for_braces_and_quotes(self):
-        """Fixes the braces and quotes spacing problems."""
+        """Fix the braces and quotes spacing problems."""
         # ()[]{}""«» should have one space before and no space after (inside)
-        for begin, end in zip(['\(','\[','\{','"','«'], ['\)','\]','\}','"','»']):
-            self.text = re.sub(rf'[ ‌]*({begin})\s*([^{end}]+?)\s*?({end})[ ‌]*',
-                r' \1\2\3 ', self.text )
+        for begin, end in zip(["\(","\[","\{",'"',"«"], ["\)","\]","\}",'"',"»"]):
+            self.text = re.sub(rf"[ ‌]*({begin})\s*([^{end}]+?)\s*?({end})[ ‌]*",
+                r" \1\2\3 ", self.text )
         # # : ; , ! ? and their Persian counterparts should have one space after and no space before
         self.text = re.sub(
-            r'[ ‌ ]*([:;,؛،.؟!]{1})[ ‌ ]*',
-            r'\1 ',
-            self.text
+            r"[ ‌ ]*([:;,؛،.؟!]{1})[ ‌ ]*",
+            r"\1 ",
+            self.text,
         )
         # special case for versioning numbers like 1.2.7
-        self.text = re.sub(r'([\d])([.])\s([\d])([.])\s([\d])', r'\1\2\3\4\5', self.text)
+        self.text = re.sub(r"([\d])([.])\s([\d])([.])\s([\d])", r"\1\2\3\4\5", self.text)
         # special case for floating-point numbers like 12.7
-        self.text = re.sub(r'([\d])([.])\s([\d])', r'\1\2\3', self.text)
+        self.text = re.sub(r"([\d])([.])\s([\d])", r"\1\2\3", self.text)
         self.text = re.sub(
-            r'[ ‌ ]*((؟\s+!){1})[ ‌ ]*',
-            r'؟! ',
-            self.text
+            r"[ ‌ ]*((؟\s+!){1})[ ‌ ]*",
+            r"؟! ",
+            self.text,
         )
         self.text = re.sub(
-            r'([۰-۹]+):\s+([۰-۹]+)',
-            r'\1:\2',
-            self.text
+            r"([۰-۹]+):\s+([۰-۹]+)",
+            r"\1:\2",
+            self.text,
         )
         self.text = re.sub(
-            r'(\d+):\s+(\d+)',
-            r'\1:\2',
-            self.text
+            r"(\d+):\s+(\d+)",
+            r"\1:\2",
+            self.text,
         )
 
     def cleanup_spacing(self):
-        """Reduces multiple consecutive spaces to one."""
-        self.text = re.sub(r'([ \t])+', r' ', self.text)
+        """Reduce multiple consecutive spaces to one."""
+        self.text = re.sub(r"([ \t])+", r" ", self.text)
         # self.text = re.sub(r'([\n]+)[ ‌]', r'\1', self.text)
-        self.text = re.sub(r'\n{2,}', r'\n\n', self.text)
-        self.text = re.sub(r'[ \t]+(\n|$)', r'\1', self.text, re.MULTILINE)
+        self.text = re.sub(r"\n{2,}", r"\n\n", self.text)
+        self.text = re.sub(r"[ \t]+(\n|$)", r"\1", self.text, re.MULTILINE)
 
     @classmethod
     def char_translator(cls, fromchar, tochar, string):
-        """Translates the 'string' character by character from 'fromchar' to 'tochar'."""
+        """Translate the 'string' character by character from 'fromchar' to 'tochar'."""
         newstring = string
         for fc, tc in zip(fromchar, tochar):
             newstring = re.sub(fc, tc, newstring)
         return newstring
 
 
 class UnTouchable:
@@ -311,43 +319,44 @@
 
     @classmethod
     def get(cls):
         return cls.words
 
     @classmethod
     def add(cls, word_list):
-        with (USERFILE/"untouchable.dat").open('a', encoding="utf8") as f:
+        with (USERFILE/"untouchable.dat").open("a", encoding="utf8") as f:
             for word in word_list:
                 if word not in cls.words:
                     f.write(word+"\n")
                     cls.words.add(word)
 
     @classmethod
     def generate(cls):
-        """
+        """Make a list from untoucahle words.
+
         A Unicode list from 'data/untouchable.dat' and '~/.python-negar/untouchable.dat'
         containing such words like 'بهتر' or 'میلاد' won't receive any modifications.
         """
         with DATAFILE.open(encoding="utf8") as f:
             for line in f:
                 cls.words.add(line.strip())
         try:
             with (USERFILE/"untouchable.dat").open(encoding="utf8") as f:
                 for line in f:
                     cls.words.add(line.strip())
-        except:
+        except FileNotFoundError:
             pass
 
 if __name__ == "__main__":
     print( "I'm a module. If you'd like the GUI, use ``negar'' instead. ;-)")
 
     print(f"""\nUsage:
     from virastar import PersianEditor
     args = []
     # append your desired options
     modifedText = PersianEditor(text, *args))
 
     e.g.
     text = {INFO}
-    print(PersianEditor(text, *['trim-lt-whitespaces',]))
+    print(PersianEditor(text, *['trim-lt-whitespaces']))
     """)
-    print(PersianEditor(f"{INFO}", *['trim-lt-whitespaces',]))
+    print(PersianEditor(f"{INFO}", *["trim-lt-whitespaces"]))
```

### Comparing `python-negar-1.2.5/python_negar.egg-info/PKG-INFO` & `python-negar-1.2.6/python_negar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2.5
+Version: 1.2.6
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2.5/setup.py` & `python-negar-1.2.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import re
 
 from setuptools import setup, find_packages
 
 version = re.search(
     r'(__version__ = "(\d\.\d(\.\d+)?)")',
     open("negar/constants.py", encoding="utf8").read(),
-    re.M
+    re.M,
 ).group(2)
 
 setup(
     name="python-negar",
     version=version,
     author="Shahin Azad",
     author_email="ishahinism@gmail.com",
     maintainer="Javad Razavian, Alireza Savand",
     maintainer_email="javadr@gmail.com, alireza.savand@gmail.com",
     include_package_data=True,
-    packages=find_packages() + ['negar'],
+    packages=find_packages() + ["negar"],
     install_requires=[
-        'regex'
+        "regex",
     ],
-    package_dir={'negar': 'negar'},
-    package_data={'negar/data': ['data/*.dat']},
+    package_dir={"negar": "negar"},
+    package_data={"negar/data": ["data/*.dat"]},
     description="Negar is a spell corrector and Persian text editor",
     license="GPL",
     keywords="spellcheck Persian editor",
     url="http://github.com/shahinism/python-negar",
     entry_points={
-        'console_scripts': [
-            'negar = negar.gui:main',
+        "console_scripts": [
+            "negar = negar.gui:main",
         ],
     },
     long_description_content_type="text/markdown",
     long_description=open("README.md", encoding="utf8").read(),
     python_requires=">=3.6",
     classifiers=[
         "Environment :: Console",
```

