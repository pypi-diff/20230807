# Comparing `tmp/flowmatic-0.1.0.5.tar.gz` & `tmp/flowmatic-0.1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowmatic-0.1.0.5.tar", max compression
+gzip compressed data, was "flowmatic-0.1.0.6.tar", max compression
```

## Comparing `flowmatic-0.1.0.5.tar` & `flowmatic-0.1.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       46 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/README.md
--rw-r--r--   0        0        0       51 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/README.md
--rw-r--r--   0        0        0     1309 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/__init__.py
--rw-r--r--   0        0        0     1441 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/flowmatic.py
--rw-r--r--   0        0        0       23 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/flows/__init__.py
--rw-r--r--   0        0        0      911 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/flows/flow.py
--rw-r--r--   0        0        0       61 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/forms/__init__.py
--rw-r--r--   0        0        0      129 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/forms/fields/__init__.py
--rw-r--r--   0        0        0      632 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/forms/fields/field.py
--rw-r--r--   0        0        0     4856 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/forms/fields/file_field.py
--rw-r--r--   0        0        0     1381 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/forms/fields/radio_group.py
--rw-r--r--   0        0        0     1575 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/forms/fields/text_field.py
--rw-r--r--   0        0        0      665 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/forms/validation.py
--rw-r--r--   0        0        0      230 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/__init__.py
--rw-r--r--   0        0        0       34 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/elements/__init__.py
--rw-r--r--   0        0        0      114 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/elements/element_infos.py
--rw-r--r--   0        0        0      620 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/gui.py
--rw-r--r--   0        0        0      141 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/screens/__init__.py
--rw-r--r--   0        0        0     3549 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/screens/form_screen.py
--rw-r--r--   0        0        0      773 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/screens/menu_screen.py
--rw-r--r--   0        0        0      830 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/screens/screen.py
--rw-r--r--   0        0        0      690 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/screens/title_screen.py
--rw-r--r--   0        0        0       99 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/style/__init__.py
--rw-r--r--   0        0        0     1864 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/gui/tkgui.py
--rw-r--r--   0        0        0       56 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/server.py
--rw-r--r--   0        0        0      209 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/util/__init__.py
--rw-r--r--   0        0        0      568 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/util/exceptions.py
--rw-r--r--   0        0        0     1135 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/util/icons.py
--rw-r--r--   0        0        0     1442 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/util/saved_class.py
--rw-r--r--   0        0        0       77 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/util/settings.py
--rw-r--r--   0        0        0      225 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/util/singleton.py
--rw-r--r--   0        0        0       73 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/flowmatic/util/user.py
--rw-r--r--   0        0        0      366 2023-08-04 14:05:22.570224 flowmatic-0.1.0.5/pyproject.toml
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 flowmatic-0.1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       46 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/README.md
+-rw-r--r--   0        0        0       51 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/README.md
+-rw-r--r--   0        0        0     1678 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/__init__.py
+-rw-r--r--   0        0        0     2089 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/flowmatic.py
+-rw-r--r--   0        0        0       23 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/flows/__init__.py
+-rw-r--r--   0        0        0      911 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/flows/flow.py
+-rw-r--r--   0        0        0       61 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/__init__.py
+-rw-r--r--   0        0        0      129 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/__init__.py
+-rw-r--r--   0        0        0      632 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/field.py
+-rw-r--r--   0        0        0     5760 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/file_field.py
+-rw-r--r--   0        0        0     1381 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/radio_group.py
+-rw-r--r--   0        0        0     1575 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/fields/text_field.py
+-rw-r--r--   0        0        0      665 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/forms/validation.py
+-rw-r--r--   0        0        0      230 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/__init__.py
+-rw-r--r--   0        0        0       34 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/elements/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/elements/element_infos.py
+-rw-r--r--   0        0        0      761 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/gui.py
+-rw-r--r--   0        0        0      141 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/__init__.py
+-rw-r--r--   0        0        0     3769 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/form_screen.py
+-rw-r--r--   0        0        0      773 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/menu_screen.py
+-rw-r--r--   0        0        0      830 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/screen.py
+-rw-r--r--   0        0        0      690 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/screens/title_screen.py
+-rw-r--r--   0        0        0       99 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/style/__init__.py
+-rw-r--r--   0        0        0     2886 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/gui/tkgui.py
+-rw-r--r--   0        0        0       56 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/server.py
+-rw-r--r--   0        0        0      209 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/exceptions.py
+-rw-r--r--   0        0        0     1135 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/icons.py
+-rw-r--r--   0        0        0     1442 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/saved_class.py
+-rw-r--r--   0        0        0       77 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/settings.py
+-rw-r--r--   0        0        0      225 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/singleton.py
+-rw-r--r--   0        0        0       73 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/flowmatic/util/user.py
+-rw-r--r--   0        0        0      366 2023-08-07 10:13:21.559285 flowmatic-0.1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 flowmatic-0.1.0.6/PKG-INFO
```

### Comparing `flowmatic-0.1.0.5/flowmatic/flows/flow.py` & `flowmatic-0.1.0.6/flowmatic/flows/flow.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/forms/fields/field.py` & `flowmatic-0.1.0.6/flowmatic/forms/fields/field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/forms/fields/file_field.py` & `flowmatic-0.1.0.6/flowmatic/forms/fields/file_field.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import os
+import platform
 import tkinter as tk
-from typing import Literal, Self
+from typing import Iterable, Literal, Self
 
 import customtkinter as ctk
 from PIL import Image
-from tkinterdnd2 import DND_FILES  # type: ignore # pylint: disable=import-error
+from tkinterdnd2 import DND_FILES
 
 import flowmatic
 from flowmatic import gui
 from flowmatic.util import Icons
 from flowmatic.util.exceptions import TooManyFilesError
 
+MAX_COLUMNS = 4
+IMAGE_WIDTH = 130
+
 
 class FileField:
     master: tk.Frame
     frame: tk.Frame
     label: str
     __value: list[str]
     __msg: tk.StringVar
     max_files: int
     width: int
     height: int
     drop_frame: ctk.CTkFrame
-    image_width: int = 100
+    image_width: int = IMAGE_WIDTH
+    columns: int
+    rows: int
 
     @property
     def value(self) -> list[str]:
         return self.files
 
     @value.setter
     def value(self, value) -> None:
@@ -56,21 +62,23 @@
         *,
         max_files: int = 1,
         files: list[str] | None = None,
     ) -> None:
         self.label = label
         self.__value = files or []
         self.__msg = tk.StringVar(value="")
-        self.max_files = max_files
+        self.max_files = max_files if max_files >= 1 else 1
+        self.columns = MAX_COLUMNS if self.max_files > MAX_COLUMNS else self.max_files
+        self.rows = (self.max_files - 1) // MAX_COLUMNS + 1
         self.width = (
-            (self.max_files % 4) * self.image_width
+            self.columns * self.image_width
             if self.max_files < 4
             else 4 * self.image_width
         )
-        self.height = (self.max_files // 4 + 1) * self.image_width
+        self.height = self.rows * self.image_width
 
     def __call__(self, master: tk.Frame) -> Self:
         self.master = master
         self.frame = ctk.CTkFrame(
             self.master,
             height=self.height,
             fg_color=ctk.ThemeManager.theme["CTkFrame"]["fg_color"],
@@ -92,77 +100,95 @@
         kwargs.pop("expand", True)
         self.drop_frame = ctk.CTkFrame(
             self.frame,
             width=self.width,
             height=self.height,
         )
         build_method(
-            self.drop_frame, side=tk.LEFT, fill=tk.BOTH, expand=False, **kwargs
+            self.drop_frame,
+            propagate=False,
+            side=tk.LEFT,
+            fill=tk.BOTH,
+            expand=False,
+            **kwargs,
         )
         self.drop_frame.drop_target_register(DND_FILES)  # type: ignore # pylint: disable=no-member
         self.drop_frame.dnd_bind("<<Drop>>", lambda file: self.add_file(file.data))  # type: ignore  # pylint: disable=no-member
         # Message
         build_method(
             ctk.CTkLabel(self.master, textvariable=self.__msg), **gui.pack_defaults
         )
 
         button_frame = ctk.CTkFrame(
             self.frame, fg_color=ctk.ThemeManager.theme["CTkFrame"]["fg_color"]
         )
         build_method(button_frame, side=tk.RIGHT, **kwargs)
 
-        # TODO: Add file dialog
-        # ctk.CTkButton(
-        #     button_frame,
-        #     text="Browse",
-        #     command=lambda: self.add_file(
-        #         appy.file_dialog(
-        #             title="Select File",
-        #             filetypes=[("All Files", "*.*")],
-        #         )
-        #     ),
-        # ).pack(**kwargs)
+        if platform.system() != "Darwin":
+            ctk.CTkButton(
+                button_frame,
+                text="Browse",
+                command=lambda: self.add_files(
+                    flowmatic.file_dialog(
+                        title="Select File",
+                        max_files=self.max_files,
+                        filetypes=[("All Files", "*.*")],
+                    )
+                ),
+            ).pack(**kwargs)
 
         ctk.CTkButton(
             button_frame,
             text="Clear",
             command=self.clear_files,
         ).pack(**kwargs)
 
         return self
 
     def pack(self, element: tk.Widget, **kwargs) -> None:
+        if kwargs.pop("propagate", None) is False:
+            element.pack_propagate(False)
+            element.grid_propagate(False)
         element.pack(**kwargs)
 
+    def add_files(self, files: Iterable[str]) -> None:
+        for file in files:
+            self.add_file(file)
+
     def add_file(self, file: str) -> None:
         try:
             self.files += [file]
         except TooManyFilesError as exc:
             self.message = str(exc)
         else:
             self.message = ""
             file_frame = ctk.CTkFrame(
                 self.drop_frame,
-                width=100,
-                height=100,
+                width=self.image_width,
+                height=self.image_width,
                 fg_color=ctk.ThemeManager.theme["CTkFrame"]["top_fg_color"],
             )
-            file_frame.pack(side=tk.LEFT, fill=tk.BOTH, expand=False)
+            index = len(self.files) - 1
+            column, row = self.get_position(index)
+            file_frame.grid(column=column, row=row)
+            file_frame.master.grid_columnconfigure(column, weight=1)
 
             your_image = ctk.CTkImage(
                 light_image=Image.open(os.path.join(Icons.path, Icons.get_icon(file))),
                 size=(72, 97),
             )
-            ctk.CTkLabel(master=file_frame, image=your_image, text="").pack()
+            ctk.CTkLabel(master=file_frame, image=your_image, text="").pack(expand=True)
             ctk.CTkLabel(file_frame, text=os.path.split(file)[-1]).pack(
                 **gui.pack_defaults
             )
 
-        finally:
-            flowmatic.update_gui()
+    def get_position(self, index: int) -> tuple[int, int]:
+        column = index % self.columns
+        row = index // self.columns
+        return column, row
 
     def clear_files(self) -> None:
         self.files = []
         self.message = ""
         for widget in self.drop_frame.winfo_children():
             widget.destroy()
-        flowmatic.update_gui()
+        # flowmatic.update_gui()
```

### Comparing `flowmatic-0.1.0.5/flowmatic/forms/fields/radio_group.py` & `flowmatic-0.1.0.6/flowmatic/forms/fields/radio_group.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/forms/fields/text_field.py` & `flowmatic-0.1.0.6/flowmatic/forms/fields/text_field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/forms/validation.py` & `flowmatic-0.1.0.6/flowmatic/forms/validation.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/gui/screens/form_screen.py` & `flowmatic-0.1.0.6/flowmatic/gui/screens/form_screen.py`

 * *Files 20% similar despite different names*

```diff
@@ -84,30 +84,38 @@
                 self.message = str(error)
                 flowmatic.update_gui()
             else:
                 on_submit()
 
         # Title
         ctk.CTkLabel(self.master, text=title).pack(**gui.pack_defaults)
+
         # Fields
         if self.field_list:
-            fields_frame = ctk.CTkFrame(self.master, width=gui.WIDTH)
+            fields_frame = ctk.CTkScrollableFrame(
+                self.master, height=gui.HEIGHT - 150, width=gui.WIDTH
+            )
             fields_frame.pack(**gui.pack_defaults)
             for field in self.field_list:
                 self.fields[field.label] = field(fields_frame).build(
                     **gui.pack_defaults
                 )
+
         # Message
         ctk.CTkLabel(self.master, textvariable=self.__message).pack(**gui.pack_defaults)
+
         # Buttons
-        ctk.CTkButton(self.master, text=submit_text, command=validate_command).pack(
+        pack_args = gui.pack_defaults  # | {"pady": (10, 20)}
+        button_frame = ctk.CTkFrame(self.master)
+        button_frame.pack(**pack_args)
+        ctk.CTkButton(button_frame, text=submit_text, command=validate_command).pack(
             **gui.pack_defaults, side=tk.RIGHT
         )
         if back_command:
-            ctk.CTkButton(self.master, text="Back", command=back_command).pack(
+            ctk.CTkButton(button_frame, text="Back", command=back_command).pack(
                 **gui.pack_defaults, side=tk.LEFT
             )
 
 
 class FlowFormScreen(FormScreen, FlowScreen):
     def __init__(self, flow: Flow) -> None:
         self.flow = flow
```

### Comparing `flowmatic-0.1.0.5/flowmatic/gui/screens/menu_screen.py` & `flowmatic-0.1.0.6/flowmatic/gui/screens/menu_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/gui/screens/screen.py` & `flowmatic-0.1.0.6/flowmatic/gui/screens/screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/gui/screens/title_screen.py` & `flowmatic-0.1.0.6/flowmatic/gui/screens/title_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/util/exceptions.py` & `flowmatic-0.1.0.6/flowmatic/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/util/icons.py` & `flowmatic-0.1.0.6/flowmatic/util/icons.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.5/flowmatic/util/saved_class.py` & `flowmatic-0.1.0.6/flowmatic/util/saved_class.py`

 * *Files identical despite different names*

