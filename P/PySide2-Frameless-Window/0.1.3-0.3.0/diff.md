# Comparing `tmp/PySide2-Frameless-Window-0.1.3.tar.gz` & `tmp/PySide2-Frameless-Window-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Frameless-Window-0.1.3.tar", last modified: Tue Aug  1 03:51:13 2023, max compression
+gzip compressed data, was "dist\PySide2-Frameless-Window-0.3.0.tar", last modified: Mon Aug  7 07:43:47 2023, max compression
```

## Comparing `PySide2-Frameless-Window-0.1.3.tar` & `PySide2-Frameless-Window-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.834451 PySide2-Frameless-Window-0.1.3/
--rw-rw-rw-   0        0        0     7815 2023-08-01 03:44:09.000000 PySide2-Frameless-Window-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     5649 2023-08-01 03:51:13.833439 PySide2-Frameless-Window-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.804192 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5649 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 03:51:13.000000 PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5036 2023-08-01 03:50:45.000000 PySide2-Frameless-Window-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.805435 PySide2-Frameless-Window-0.1.3/qframelesswindow/
--rw-rw-rw-   0        0        0     2314 2023-08-01 03:49:25.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.808873 PySide2-Frameless-Window-0.1.3/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2730 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.812587 PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2878 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.816031 PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3024 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4314 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.819507 PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4942 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.825691 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     7973 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:51:13.830943 PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     7214 2023-08-01 03:49:09.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4013 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8810 2023-08-01 03:47:54.000000 PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-08-01 03:51:13.834451 PySide2-Frameless-Window-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1001 2023-08-01 03:49:22.000000 PySide2-Frameless-Window-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.217928 PySide2-Frameless-Window-0.3.0/
+-rw-rw-rw-   0        0        0     7815 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5649 2023-08-07 07:43:47.216270 PySide2-Frameless-Window-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.186791 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5649 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5036 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.189996 PySide2-Frameless-Window-0.3.0/qframelesswindow/
+-rw-rw-rw-   0        0        0     2328 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.192946 PySide2-Frameless-Window-0.3.0/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2730 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.196346 PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2878 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.199549 PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3024 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4314 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.203735 PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5086 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.210261 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     7973 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.215269 PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     7214 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4013 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8810 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:43:47.217928 PySide2-Frameless-Window-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/setup.py
```

### Comparing `PySide2-Frameless-Window-0.1.3/LICENSE` & `PySide2-Frameless-Window-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/PKG-INFO` & `PySide2-Frameless-Window-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.1.3
+Version: 0.3.0
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
 Platform: UNKNOWN
```

### Comparing `PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/PKG-INFO` & `PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.1.3
+Version: 0.3.0
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
 Platform: UNKNOWN
```

### Comparing `PySide2-Frameless-Window-0.1.3/PySide2_Frameless_Window.egg-info/SOURCES.txt` & `PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/README.md` & `PySide2-Frameless-Window-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/__init__.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.3"
+__version__ = "0.3.0"
 
 import sys
 
 from PySide2.QtWidgets import QDialog, QMainWindow
 
-from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
+from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar, TitleBarBase
 
 if sys.platform == "win32":
     from .windows import AcrylicWindow as AcrylicWindowBase
     from .windows import WindowsFramelessWindow as FramelessWindowBase
     from .windows import WindowsWindowEffect as WindowEffect
 elif sys.platform == "darwin":
     from .mac import AcrylicWindow as AcrylicWindowBase
```

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/_rc/resource.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/__init__.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/linux/window_effect.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/__init__.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/mac/window_effect.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/__init__.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,37 +6,28 @@
 from PySide2.QtWidgets import QLabel, QHBoxLayout, QWidget
 
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
 
@@ -97,14 +88,31 @@
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

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/titlebar/title_bar_buttons.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/__init__.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/linux_utils.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/mac_utils.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/utils/win32_utils.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/__init__.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/c_structures.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/qframelesswindow/windows/window_effect.py` & `PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.3/setup.py` & `PySide2-Frameless-Window-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Frameless-Window",
-    version="0.1.3",
+    version="0.3.0",
     keywords="pyside2 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

