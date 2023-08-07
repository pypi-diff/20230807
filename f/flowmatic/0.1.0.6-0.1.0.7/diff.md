# Comparing `tmp/flowmatic-0.1.0.6.tar.gz` & `tmp/flowmatic-0.1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowmatic-0.1.0.6.tar", max compression
+gzip compressed data, was "flowmatic-0.1.0.7.tar", max compression
```

## Comparing `flowmatic-0.1.0.6.tar` & `flowmatic-0.1.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       46 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/README.md
--rw-r--r--   0        0        0       51 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/README.md
--rw-r--r--   0        0        0     1678 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/__init__.py
--rw-r--r--   0        0        0     2089 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/flowmatic.py
--rw-r--r--   0        0        0       23 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/flows/__init__.py
--rw-r--r--   0        0        0      911 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/flows/flow.py
--rw-r--r--   0        0        0       61 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/__init__.py
--rw-r--r--   0        0        0      129 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/__init__.py
--rw-r--r--   0        0        0      632 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/field.py
--rw-r--r--   0        0        0     5760 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/file_field.py
--rw-r--r--   0        0        0     1381 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/radio_group.py
--rw-r--r--   0        0        0     1575 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/text_field.py
--rw-r--r--   0        0        0      665 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/validation.py
--rw-r--r--   0        0        0      230 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/__init__.py
--rw-r--r--   0        0        0       34 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/elements/__init__.py
--rw-r--r--   0        0        0      114 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/elements/element_infos.py
--rw-r--r--   0        0        0      761 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/gui.py
--rw-r--r--   0        0        0      141 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/__init__.py
--rw-r--r--   0        0        0     3769 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/form_screen.py
--rw-r--r--   0        0        0      773 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/menu_screen.py
--rw-r--r--   0        0        0      830 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/screen.py
--rw-r--r--   0        0        0      690 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/title_screen.py
--rw-r--r--   0        0        0       99 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/style/__init__.py
--rw-r--r--   0        0        0     2886 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/tkgui.py
--rw-r--r--   0        0        0       56 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/server.py
--rw-r--r--   0        0        0      209 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/__init__.py
--rw-r--r--   0        0        0      568 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/exceptions.py
--rw-r--r--   0        0        0     1135 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/icons.py
--rw-r--r--   0        0        0     1442 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/saved_class.py
--rw-r--r--   0        0        0       77 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/settings.py
--rw-r--r--   0        0        0      225 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/singleton.py
--rw-r--r--   0        0        0       73 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/user.py
--rw-r--r--   0        0        0      366 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/pyproject.toml
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 flowmatic-0.1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       46 2023-08-07 11:41:17.364816 flowmatic-0.1.0.7/README.md
+-rw-r--r--   0        0        0       51 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/README.md
+-rw-r--r--   0        0        0     1678 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/__init__.py
+-rw-r--r--   0        0        0     2089 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/flowmatic.py
+-rw-r--r--   0        0        0       23 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/flows/__init__.py
+-rw-r--r--   0        0        0      911 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/flows/flow.py
+-rw-r--r--   0        0        0       61 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/forms/__init__.py
+-rw-r--r--   0        0        0      129 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/forms/fields/__init__.py
+-rw-r--r--   0        0        0      632 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/forms/fields/field.py
+-rw-r--r--   0        0        0     5760 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/forms/fields/file_field.py
+-rw-r--r--   0        0        0     1381 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/forms/fields/radio_group.py
+-rw-r--r--   0        0        0     1575 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/forms/fields/text_field.py
+-rw-r--r--   0        0        0      665 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/forms/validation.py
+-rw-r--r--   0        0        0      230 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/__init__.py
+-rw-r--r--   0        0        0       34 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/elements/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/elements/element_infos.py
+-rw-r--r--   0        0        0      761 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/gui.py
+-rw-r--r--   0        0        0      141 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/screens/__init__.py
+-rw-r--r--   0        0        0     3927 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/screens/form_screen.py
+-rw-r--r--   0        0        0      773 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/screens/menu_screen.py
+-rw-r--r--   0        0        0     2134 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/screens/screen.py
+-rw-r--r--   0        0        0      690 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/screens/title_screen.py
+-rw-r--r--   0        0        0       99 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/style/__init__.py
+-rw-r--r--   0        0        0     2886 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/gui/tkgui.py
+-rw-r--r--   0        0        0       56 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/server.py
+-rw-r--r--   0        0        0      209 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/util/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/util/exceptions.py
+-rw-r--r--   0        0        0     1135 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/util/icons.py
+-rw-r--r--   0        0        0     1442 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/util/saved_class.py
+-rw-r--r--   0        0        0       77 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/util/settings.py
+-rw-r--r--   0        0        0      225 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/util/singleton.py
+-rw-r--r--   0        0        0       73 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/flowmatic/util/user.py
+-rw-r--r--   0        0        0      366 2023-08-07 11:41:17.368816 flowmatic-0.1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 flowmatic-0.1.0.7/PKG-INFO
```

### Comparing `flowmatic-0.1.0.6/flowmatic/__init__.py` & `flowmatic-0.1.0.7/flowmatic/__init__.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/flowmatic.py` & `flowmatic-0.1.0.7/flowmatic/flowmatic.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/flows/flow.py` & `flowmatic-0.1.0.7/flowmatic/flows/flow.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/forms/fields/field.py` & `flowmatic-0.1.0.7/flowmatic/forms/fields/field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/forms/fields/file_field.py` & `flowmatic-0.1.0.7/flowmatic/forms/fields/file_field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/forms/fields/radio_group.py` & `flowmatic-0.1.0.7/flowmatic/forms/fields/radio_group.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/forms/fields/text_field.py` & `flowmatic-0.1.0.7/flowmatic/forms/fields/text_field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/forms/validation.py` & `flowmatic-0.1.0.7/flowmatic/forms/validation.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/gui/gui.py` & `flowmatic-0.1.0.7/flowmatic/gui/gui.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/gui/screens/form_screen.py` & `flowmatic-0.1.0.7/flowmatic/gui/screens/form_screen.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,16 +87,20 @@
                 on_submit()
 
         # Title
         ctk.CTkLabel(self.master, text=title).pack(**gui.pack_defaults)
 
         # Fields
         if self.field_list:
-            fields_frame = ctk.CTkScrollableFrame(
-                self.master, height=gui.HEIGHT - 150, width=gui.WIDTH
+            fields_frame = (
+                ctk.CTkScrollableFrame(
+                    self.master, height=gui.HEIGHT - 150, width=gui.WIDTH
+                )
+                if not isinstance(self.master, ctk.CTkScrollableFrame)
+                else ctk.CTkFrame(self.master)
             )
             fields_frame.pack(**gui.pack_defaults)
             for field in self.field_list:
                 self.fields[field.label] = field(fields_frame).build(
                     **gui.pack_defaults
                 )
```

### Comparing `flowmatic-0.1.0.6/flowmatic/gui/screens/menu_screen.py` & `flowmatic-0.1.0.7/flowmatic/gui/screens/menu_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/gui/screens/title_screen.py` & `flowmatic-0.1.0.7/flowmatic/gui/screens/title_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/gui/tkgui.py` & `flowmatic-0.1.0.7/flowmatic/gui/tkgui.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/util/exceptions.py` & `flowmatic-0.1.0.7/flowmatic/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/util/icons.py` & `flowmatic-0.1.0.7/flowmatic/util/icons.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.6/flowmatic/util/saved_class.py` & `flowmatic-0.1.0.7/flowmatic/util/saved_class.py`

 * *Files identical despite different names*

