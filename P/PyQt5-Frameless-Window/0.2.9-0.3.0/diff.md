# Comparing `tmp/PyQt5-Frameless-Window-0.2.9.tar.gz` & `tmp/PyQt5-Frameless-Window-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.9.tar", last modified: Tue Aug  1 03:30:35 2023, max compression
+gzip compressed data, was "dist\PyQt5-Frameless-Window-0.3.0.tar", last modified: Mon Aug  7 07:16:45 2023, max compression
```

## Comparing `PyQt5-Frameless-Window-0.2.9.tar` & `PyQt5-Frameless-Window-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.769915 PyQt5-Frameless-Window-0.2.9/
--rw-rw-rw-   0        0        0    35823 2023-07-08 13:18:44.000000 PyQt5-Frameless-Window-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     5932 2023-08-01 03:30:35.768914 PyQt5-Frameless-Window-0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.731007 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5932 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 03:30:35.000000 PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5341 2023-08-01 03:27:51.000000 PyQt5-Frameless-Window-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.741038 PyQt5-Frameless-Window-0.2.9/qframelesswindow/
--rw-rw-rw-   0        0        0     1679 2023-08-01 03:20:49.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.744632 PyQt5-Frameless-Window-0.2.9/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.747135 PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2891 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     3119 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.750756 PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     2994 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4334 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.754417 PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4984 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9057 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.761485 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-08-01 03:04:10.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-08-01 03:04:11.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8352 2023-08-01 03:04:11.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:30:35.767915 PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     7084 2023-08-01 03:18:28.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4263 2023-08-01 03:04:11.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8987 2023-08-01 03:04:11.000000 PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-08-01 03:30:35.769915 PyQt5-Frameless-Window-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-08-01 03:20:42.000000 PyQt5-Frameless-Window-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:16:45.797701 PyQt5-Frameless-Window-0.3.0/
+-rw-rw-rw-   0        0        0    35823 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5932 2023-08-07 07:16:45.797701 PyQt5-Frameless-Window-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 07:16:45.756058 PyQt5-Frameless-Window-0.3.0/PyQt5_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5932 2023-08-07 07:16:45.000000 PyQt5-Frameless-Window-0.3.0/PyQt5_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-08-07 07:16:45.000000 PyQt5-Frameless-Window-0.3.0/PyQt5_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:16:45.000000 PyQt5-Frameless-Window-0.3.0/PyQt5_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-08-07 07:16:45.000000 PyQt5-Frameless-Window-0.3.0/PyQt5_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-07 07:16:45.000000 PyQt5-Frameless-Window-0.3.0/PyQt5_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5341 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:16:45.765663 PyQt5-Frameless-Window-0.3.0/qframelesswindow/
+-rw-rw-rw-   0        0        0     1693 2023-08-07 07:10:04.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:16:45.767921 PyQt5-Frameless-Window-0.3.0/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:16:45.771970 PyQt5-Frameless-Window-0.3.0/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2891 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3119 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:16:45.775483 PyQt5-Frameless-Window-0.3.0/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     2994 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4334 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:16:45.780137 PyQt5-Frameless-Window-0.3.0/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5130 2023-08-07 07:05:35.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9057 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:16:45.790932 PyQt5-Frameless-Window-0.3.0/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8352 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:16:45.795206 PyQt5-Frameless-Window-0.3.0/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     7084 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4263 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8987 2023-08-01 03:52:32.000000 PyQt5-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:16:45.797701 PyQt5-Frameless-Window-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-08-07 07:10:11.000000 PyQt5-Frameless-Window-0.3.0/setup.py
```

### Comparing `PyQt5-Frameless-Window-0.2.9/LICENSE` & `PyQt5-Frameless-Window-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/PKG-INFO` & `PyQt5-Frameless-Window-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.9
+Version: 0.3.0
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
 Platform: UNKNOWN
```

### Comparing `PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/PKG-INFO` & `PyQt5-Frameless-Window-0.3.0/PyQt5_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.9
+Version: 0.3.0
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
 Platform: UNKNOWN
```

### Comparing `PyQt5-Frameless-Window-0.2.9/PyQt5_Frameless_Window.egg-info/SOURCES.txt` & `PyQt5-Frameless-Window-0.3.0/PyQt5_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/README.md` & `PyQt5-Frameless-Window-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/__init__.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/master/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.2.9"
+__version__ = "0.3.0"
 
 import sys
 
 from PyQt5.QtWidgets import QDialog, QMainWindow
 
-from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
+from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar, TitleBarBase
 
 if sys.platform == "win32":
     from .windows import AcrylicWindow
     from .windows import WindowsFramelessWindow as FramelessWindow
     from .windows import WindowsWindowEffect as WindowEffect
 elif sys.platform == "darwin":
     from .mac import AcrylicWindow
```

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/_rc/resource.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/__init__.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/linux/window_effect.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/__init__.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/mac/window_effect.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/__init__.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,37 +6,28 @@
 from PyQt5.QtWidgets import QHBoxLayout, QLabel, QWidget
 
 from ..utils import startSystemMove
 from .title_bar_buttons import (CloseButton, MaximizeButton, MinimizeButton,
                                 SvgTitleBarButton, TitleBarButton)
 
 
-class TitleBar(QWidget):
-    """ Title bar with minimize, maximum and close button """
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
-        self.hBoxLayout.setAlignment(Qt.AlignVCenter | Qt.AlignLeft)
-        self.hBoxLayout.addStretch(1)
-        self.hBoxLayout.addWidget(self.minBtn, 0, Qt.AlignRight)
-        self.hBoxLayout.addWidget(self.maxBtn, 0, Qt.AlignRight)
-        self.hBoxLayout.addWidget(self.closeBtn, 0, Qt.AlignRight)
-
         # connect signal to slot
         self.minBtn.clicked.connect(self.window().showMinimized)
         self.maxBtn.clicked.connect(self.__toggleMaxState)
         self.closeBtn.clicked.connect(self.window().close)
 
         self.window().installEventFilter(self)
 
@@ -98,14 +89,32 @@
         ----------
         isEnabled: bool
             whether to enable double click
         """
         self._isDoubleClickEnabled = isEnabled
 
 
+
+class TitleBar(TitleBarBase):
+    """ Title bar with minimize, maximum and close button """
+
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.hBoxLayout = QHBoxLayout(self)
+
+        # add buttons to layout
+        self.hBoxLayout.setSpacing(0)
+        self.hBoxLayout.setContentsMargins(0, 0, 0, 0)
+        self.hBoxLayout.setAlignment(Qt.AlignVCenter | Qt.AlignLeft)
+        self.hBoxLayout.addStretch(1)
+        self.hBoxLayout.addWidget(self.minBtn, 0, Qt.AlignRight)
+        self.hBoxLayout.addWidget(self.maxBtn, 0, Qt.AlignRight)
+        self.hBoxLayout.addWidget(self.closeBtn, 0, Qt.AlignRight)
+
+
 class StandardTitleBar(TitleBar):
     """ Title bar with icon and title """
 
     def __init__(self, parent):
         super().__init__(parent)
         # add window icon
         self.iconLabel = QLabel(self)
```

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/__init__.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/linux_utils.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/mac_utils.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/utils/win32_utils.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/__init__.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/c_structures.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/qframelesswindow/windows/window_effect.py` & `PyQt5-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.9/setup.py` & `PyQt5-Frameless-Window-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt5-Frameless-Window",
-    version="0.2.9",
+    version="0.3.0",
     keywords="pyqt frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

