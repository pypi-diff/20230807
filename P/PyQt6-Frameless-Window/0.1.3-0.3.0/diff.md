# Comparing `tmp/PyQt6-Frameless-Window-0.1.3.tar.gz` & `tmp/PyQt6-Frameless-Window-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt6-Frameless-Window-0.1.3.tar", last modified: Tue Aug  1 03:43:45 2023, max compression
+gzip compressed data, was "dist\PyQt6-Frameless-Window-0.3.0.tar", last modified: Mon Aug  7 07:41:00 2023, max compression
```

## Comparing `PyQt6-Frameless-Window-0.1.3.tar` & `PyQt6-Frameless-Window-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.924931 PyQt6-Frameless-Window-0.1.3/
--rw-rw-rw-   0        0        0    35823 2023-07-08 13:18:44.000000 PyQt6-Frameless-Window-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     5603 2023-08-01 03:43:45.923741 PyQt6-Frameless-Window-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.886735 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5603 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 03:43:45.000000 PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5007 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.897214 PyQt6-Frameless-Window-0.1.3/qframelesswindow/
--rw-rw-rw-   0        0        0     1678 2023-08-01 03:42:22.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.900316 PyQt6-Frameless-Window-0.1.3/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.903414 PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     3110 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     3149 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.906507 PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3015 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4563 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.909841 PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5083 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9205 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.916234 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0      644 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8352 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:43:45.921299 PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6760 2023-08-01 03:34:35.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     9413 2023-08-01 03:33:00.000000 PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-08-01 03:43:45.924931 PyQt6-Frameless-Window-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-08-01 03:42:26.000000 PyQt6-Frameless-Window-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.137366 PyQt6-Frameless-Window-0.3.0/
+-rw-rw-rw-   0        0        0    35823 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5603 2023-08-07 07:41:00.136355 PyQt6-Frameless-Window-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.099927 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5603 2023-08-07 07:40:59.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-08-07 07:41:00.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:40:59.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-07 07:40:59.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-07 07:40:59.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5007 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.109857 PyQt6-Frameless-Window-0.3.0/qframelesswindow/
+-rw-rw-rw-   0        0        0     1692 2023-08-07 07:38:21.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.113252 PyQt6-Frameless-Window-0.3.0/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.116649 PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     3110 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3149 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.120211 PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3015 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4563 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.123614 PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5235 2023-08-07 07:37:45.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9205 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.129851 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0      644 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8352 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.135348 PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     6760 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     9413 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:41:00.137366 PyQt6-Frameless-Window-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-08-07 07:39:13.000000 PyQt6-Frameless-Window-0.3.0/setup.py
```

### Comparing `PyQt6-Frameless-Window-0.1.3/LICENSE` & `PyQt6-Frameless-Window-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/PKG-INFO` & `PyQt6-Frameless-Window-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.1.3
+Version: 0.3.0
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
 Platform: UNKNOWN
```

### Comparing `PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/PKG-INFO` & `PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.1.3
+Version: 0.3.0
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
 Platform: UNKNOWN
```

### Comparing `PyQt6-Frameless-Window-0.1.3/PyQt6_Frameless_Window.egg-info/SOURCES.txt` & `PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/README.md` & `PyQt6-Frameless-Window-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/__init__.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.3"
+__version__ = "0.3.0"
 
 import sys
 
 from PyQt6.QtWidgets import QDialog, QMainWindow
 
-from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
+from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar, TitleBarBase
 
 if sys.platform == "win32":
     from .windows import AcrylicWindow
     from .windows import WindowsFramelessWindow as FramelessWindow
     from .windows import WindowsWindowEffect as WindowEffect
 elif sys.platform == "darwin":
     from .mac import AcrylicWindow
```

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/_rc/resource.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/__init__.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/linux/window_effect.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/__init__.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/mac/window_effect.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/__init__.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,37 +6,28 @@
 from PyQt6.QtWidgets import QLabel, QHBoxLayout, QWidget
 
 from ..utils import startSystemMove
 from .title_bar_buttons import (CloseButton, MaximizeButton, MinimizeButton,
                                 SvgTitleBarButton, TitleBarButton)
 
 
-class TitleBar(QWidget):
-    """ Title bar """
+class TitleBarBase(QWidget):
+    """ Title bar base class """
 
     def __init__(self, parent):
         super().__init__(parent)
         self.minBtn = MinimizeButton(parent=self)
         self.closeBtn = CloseButton(parent=self)
         self.maxBtn = MaximizeButton(parent=self)
-        self.hBoxLayout = QHBoxLayout(self)
+
         self._isDoubleClickEnabled = True
 
         self.resize(200, 32)
         self.setFixedHeight(32)
 
-        # add buttons to layout
-        self.hBoxLayout.setSpacing(0)
-        self.hBoxLayout.setContentsMargins(0, 0, 0, 0)
-        self.hBoxLayout.setAlignment(Qt.AlignmentFlag.AlignVCenter | Qt.AlignmentFlag.AlignLeft)
-        self.hBoxLayout.addStretch(1)
-        self.hBoxLayout.addWidget(self.minBtn, 0, Qt.AlignmentFlag.AlignRight)
-        self.hBoxLayout.addWidget(self.maxBtn, 0, Qt.AlignmentFlag.AlignRight)
-        self.hBoxLayout.addWidget(self.closeBtn, 0, Qt.AlignmentFlag.AlignRight)
-
         # connect signal to slot
         self.minBtn.clicked.connect(self.window().showMinimized)
         self.maxBtn.clicked.connect(self.__toggleMaxState)
         self.closeBtn.clicked.connect(self.window().close)
 
         self.window().installEventFilter(self)
 
@@ -98,14 +89,31 @@
         ----------
         isEnabled: bool
             whether to enable double click
         """
         self._isDoubleClickEnabled = isEnabled
 
 
+class TitleBar(TitleBarBase):
+    """ Title bar """
+
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.hBoxLayout = QHBoxLayout(self)
+
+        # add buttons to layout
+        self.hBoxLayout.setSpacing(0)
+        self.hBoxLayout.setContentsMargins(0, 0, 0, 0)
+        self.hBoxLayout.setAlignment(Qt.AlignmentFlag.AlignVCenter | Qt.AlignmentFlag.AlignLeft)
+        self.hBoxLayout.addStretch(1)
+        self.hBoxLayout.addWidget(self.minBtn, 0, Qt.AlignmentFlag.AlignRight)
+        self.hBoxLayout.addWidget(self.maxBtn, 0, Qt.AlignmentFlag.AlignRight)
+        self.hBoxLayout.addWidget(self.closeBtn, 0, Qt.AlignmentFlag.AlignRight)
+        
+
 class StandardTitleBar(TitleBar):
     """ Title bar with icon and title """
 
     def __init__(self, parent):
         super().__init__(parent)
         # add window icon
         self.iconLabel = QLabel(self)
```

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/__init__.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/linux_utils.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/mac_utils.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/utils/win32_utils.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/__init__.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/c_structures.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/qframelesswindow/windows/window_effect.py` & `PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.1.3/setup.py` & `PyQt6-Frameless-Window-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt6-Frameless-Window",
-    version="0.1.3",
+    version="0.3.0",
     keywords="pyqt6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

