# Comparing `tmp/PySideSix-Frameless-Window-0.1.2.tar.gz` & `tmp/PySideSix-Frameless-Window-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySideSix-Frameless-Window-0.1.2.tar", last modified: Tue Aug  1 03:47:21 2023, max compression
+gzip compressed data, was "dist\PySideSix-Frameless-Window-0.3.0.tar", last modified: Mon Aug  7 07:30:54 2023, max compression
```

## Comparing `PySideSix-Frameless-Window-0.1.2.tar` & `PySideSix-Frameless-Window-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.105693 PySideSix-Frameless-Window-0.1.2/
--rw-rw-rw-   0        0        0     7815 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5542 2023-08-01 03:47:21.105693 PySideSix-Frameless-Window-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.070856 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5542 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 03:47:20.000000 PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4927 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.073021 PySideSix-Frameless-Window-0.1.2/qframelesswindow/
--rw-rw-rw-   0        0        0     1614 2023-08-01 03:44:50.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.077719 PySideSix-Frameless-Window-0.1.2/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.081891 PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     4320 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     3147 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.085743 PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     4529 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4549 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.089379 PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5062 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.097688 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8093 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:47:21.103691 PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     8379 2023-08-01 03:45:56.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     9369 2023-08-01 03:44:09.000000 PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-08-01 03:47:21.106694 PySideSix-Frameless-Window-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-08-01 03:44:44.000000 PySideSix-Frameless-Window-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.892009 PySideSix-Frameless-Window-0.3.0/
+-rw-rw-rw-   0        0        0     7815 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5672 2023-08-07 07:30:54.890999 PySideSix-Frameless-Window-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.856305 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5672 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5057 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.865691 PySideSix-Frameless-Window-0.3.0/qframelesswindow/
+-rw-rw-rw-   0        0        0     1628 2023-08-07 07:26:28.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.868705 PySideSix-Frameless-Window-0.3.0/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.871705 PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     4320 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3147 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.875223 PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     4529 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4549 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.879027 PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5208 2023-08-07 07:19:54.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.884198 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8093 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.889612 PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     8379 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     9369 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:30:54.892009 PySideSix-Frameless-Window-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-08-07 07:26:35.000000 PySideSix-Frameless-Window-0.3.0/setup.py
```

### Comparing `PySideSix-Frameless-Window-0.1.2/LICENSE` & `PySideSix-Frameless-Window-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/PKG-INFO` & `PySideSix-Frameless-Window-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.1.2
+Version: 0.3.0
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Platform: UNKNOWN
@@ -120,14 +120,15 @@
 
 
 ## See Also
 Here are some projects that use PyQt-Frameless-Window:
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
 * [**zhiyiYo/PyQt-Fluent-Widgets**: A fluent design widgets library based on PyQt5](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)
+* [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PySide](https://github.com/zhiyiYo/QMaterialWidgets)
 
 ## Reference
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PySide6-Frameless-Window is licensed under [LGPLv3](./LICENSE).
```

### Comparing `PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/PKG-INFO` & `PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.1.2
+Version: 0.3.0
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Platform: UNKNOWN
@@ -120,14 +120,15 @@
 
 
 ## See Also
 Here are some projects that use PyQt-Frameless-Window:
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
 * [**zhiyiYo/PyQt-Fluent-Widgets**: A fluent design widgets library based on PyQt5](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)
+* [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PySide](https://github.com/zhiyiYo/QMaterialWidgets)
 
 ## Reference
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PySide6-Frameless-Window is licensed under [LGPLv3](./LICENSE).
```

### Comparing `PySideSix-Frameless-Window-0.1.2/PySideSix_Frameless_Window.egg-info/SOURCES.txt` & `PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/README.md` & `PySideSix-Frameless-Window-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 
 
 ## See Also
 Here are some projects that use PyQt-Frameless-Window:
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
 * [**zhiyiYo/PyQt-Fluent-Widgets**: A fluent design widgets library based on PyQt5](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)
+* [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PySide](https://github.com/zhiyiYo/QMaterialWidgets)
 
 ## Reference
 * [**wangwenx190/framelesshelper**: Frameless windows for Qt Widgets and Qt Quick applications. Support Win32, X11, Wayland and macOS](https://github.com/wangwenx190/framelesshelper)
 * [**libxcb**: Basic Graphics Programming With The XCB Library](https://www.x.org/releases/X11R7.5/doc/libxcb/tutorial)
 
 ## License
 PySide6-Frameless-Window is licensed under [LGPLv3](./LICENSE).
```

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/__init__.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.2"
+__version__ = "0.3.0"
 
 import sys
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QMainWindow
 
-from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
+from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar, TitleBarBase
 
 if sys.platform == "win32":
     from .windows import AcrylicWindow
     from .windows import WindowsFramelessWindow as FramelessWindow
     from .windows import WindowsFramelessMainWindow as FramelessMainWindow
     from .windows import WindowsFramelessDialog as FramelessDialog
     from .windows import WindowsWindowEffect as WindowEffect
```

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/_rc/resource.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/__init__.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/linux/window_effect.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/__init__.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/mac/window_effect.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/__init__.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,37 +10,28 @@
 from PySide6.QtWidgets import QLabel, QHBoxLayout, QWidget
 
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
 
@@ -101,14 +92,32 @@
         ----------
         isEnabled: bool
             whether to enable double click
         """
         self._isDoubleClickEnabled = isEnabled
 
 
+
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

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/titlebar/title_bar_buttons.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/__init__.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/linux_utils.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/mac_utils.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/utils/win32_utils.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/__init__.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/c_structures.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/qframelesswindow/windows/window_effect.py` & `PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.1.2/setup.py` & `PySideSix-Frameless-Window-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySideSix-Frameless-Window",
-    version="0.1.2",
+    version="0.3.0",
     keywords="pyside6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

