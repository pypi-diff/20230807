# Comparing `tmp/MyOverlay-0.2.2.tar.gz` & `tmp/MyOverlay-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.2.2.tar", last modified: Thu Aug  3 10:45:04 2023, max compression
+gzip compressed data, was "MyOverlay-0.2.3.tar", last modified: Mon Aug  7 06:53:14 2023, max compression
```

## Comparing `MyOverlay-0.2.2.tar` & `MyOverlay-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.321579 MyOverlay-0.2.2/
--rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      745 2023-08-03 10:45:04.321579 MyOverlay-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.2.2/README.md
--rw-rw-rw-   0        0        0      649 2023-08-03 10:44:31.000000 MyOverlay-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 10:45:04.322584 MyOverlay-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.280603 MyOverlay-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.300655 MyOverlay-0.2.2/src/MyOverlay/
--rw-rw-rw-   0        0        0      409 2023-08-02 14:16:50.000000 MyOverlay-0.2.2/src/MyOverlay/Overlay.py
--rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.2.2/src/MyOverlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.320587 MyOverlay-0.2.2/src/MyOverlay/funcs/
--rw-rw-rw-   0        0        0     5484 2023-08-03 10:13:51.000000 MyOverlay-0.2.2/src/MyOverlay/funcs/myfunctions.py
-drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.313608 MyOverlay-0.2.2/src/MyOverlay.egg-info/
--rw-rw-rw-   0        0        0      745 2023-08-03 10:45:04.000000 MyOverlay-0.2.2/src/MyOverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-08-03 10:45:04.000000 MyOverlay-0.2.2/src/MyOverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 10:45:04.000000 MyOverlay-0.2.2/src/MyOverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 10:45:04.000000 MyOverlay-0.2.2/src/MyOverlay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:14.729828 MyOverlay-0.2.3/
+-rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-08-07 06:53:14.729828 MyOverlay-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.2.3/README.md
+-rw-rw-rw-   0        0        0      649 2023-08-07 06:52:51.000000 MyOverlay-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 06:53:14.729828 MyOverlay-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:14.703907 MyOverlay-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:14.714828 MyOverlay-0.2.3/src/MyOverlay/
+-rw-rw-rw-   0        0        0      409 2023-08-02 14:16:50.000000 MyOverlay-0.2.3/src/MyOverlay/Overlay.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.2.3/src/MyOverlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:14.728829 MyOverlay-0.2.3/src/MyOverlay/funcs/
+-rw-rw-rw-   0        0        0     5216 2023-08-07 06:52:21.000000 MyOverlay-0.2.3/src/MyOverlay/funcs/myfunctions.py
+-rw-rw-rw-   0        0        0        0 2023-08-07 06:43:53.000000 MyOverlay-0.2.3/src/MyOverlay/funcs/test.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:14.726828 MyOverlay-0.2.3/src/MyOverlay.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-08-07 06:53:14.000000 MyOverlay-0.2.3/src/MyOverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-08-07 06:53:14.000000 MyOverlay-0.2.3/src/MyOverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 06:53:14.000000 MyOverlay-0.2.3/src/MyOverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-07 06:53:14.000000 MyOverlay-0.2.3/src/MyOverlay.egg-info/top_level.txt
```

### Comparing `MyOverlay-0.2.2/LICENSE` & `MyOverlay-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MyOverlay-0.2.2/PKG-INFO` & `MyOverlay-0.2.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.2.2
+Version: 0.2.3
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MyOverlay-0.2.2/pyproject.toml` & `MyOverlay-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "MyOverlay"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Erik Reimann", email="erikreimann28@gmail.com" },
 ]
 description = "Customized Text Only Screen Overlay"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `MyOverlay-0.2.2/src/MyOverlay/funcs/myfunctions.py` & `MyOverlay-0.2.3/src/MyOverlay/funcs/myfunctions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from win32api import GetSystemMetrics
 import pygame
 import win32api
 import win32con
 import win32gui
 import ctypes
-import time
 from thefuzz import fuzz
 
-OverlayRunning = False
+
 white = (255, 255, 255)
 black = (0, 0, 0)
 fuchsia = (255, 0, 128)
 GWL_EXSTYLE = -20
 WS_EX_APPWINDOW = 0x00040000
 WS_EX_TOOLWINDOW = 0x00000080
 
 _circle_cache = {}
+
+
 def _circlepoints(r):
     r = int(round(r))
     if r in _circle_cache:
         return _circle_cache[r]
     x, y, e = r, 0, 1 - r
     _circle_cache[r] = points = []
     while x >= y:
@@ -53,86 +54,68 @@
         surf.blit(osurf, (dx + opx, dy + opx))
 
     surf.blit(textsurface, (opx, opx))
     return surf
 
 
 def StartOverlay():
-    global OverlayRunning
-    if not OverlayRunning:
+    if not pygame.display.get_active():
         global text
         global textRect
         global screen
-        OverlayRunning = True
         screen_width = GetSystemMetrics(win32con.SM_CXSCREEN)
         screen_height = GetSystemMetrics(win32con.SM_CYSCREEN)
         pygame.init()
         screen = pygame.display.set_mode((screen_width, screen_height), pygame.NOFRAME)
         hwnd = pygame.display.get_wm_info()["window"]
         style = ctypes.windll.user32.GetWindowLongW(hwnd, GWL_EXSTYLE)
-        
+
         style = style & ~WS_EX_APPWINDOW
         style = style | WS_EX_TOOLWINDOW
         style = ctypes.windll.user32.GetWindowLongW(hwnd, GWL_EXSTYLE)
-        
+
         style = style & ~WS_EX_APPWINDOW
         style = style | WS_EX_TOOLWINDOW
         ctypes.windll.user32.SetWindowLongW(hwnd, GWL_EXSTYLE, style)
         win32gui.SetWindowLong(hwnd, win32con.GWL_EXSTYLE,
                                win32gui.GetWindowLong(hwnd,
                                                       win32con.GWL_EXSTYLE) | win32con.WS_EX_LAYERED | win32con.WS_EX_TOPMOST)
-                                                      
+
         win32gui.SetWindowPos(hwnd, win32con.HWND_TOPMOST, 0, 0, screen_width, screen_height, 0)
-        win32gui.SetLayeredWindowAttributes(hwnd, win32api.RGB(*fuchsia), 0, win32con.LWA_COLORKEY)  
+        win32gui.SetLayeredWindowAttributes(hwnd, win32api.RGB(*fuchsia), 0, win32con.LWA_COLORKEY)
         screen.fill(fuchsia)
         pygame.display.update()
-        
-        
-           
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
+
         return True
     else:
         return False
 
 
+def settext(text: str, PosX: int, PosY: int):
+    if pygame.display.get_active():
+        font = pygame.font.SysFont('Segoe UI Semibold', 30, False)
+        screen.fill(fuchsia)  # Transparent background
+        lines = str(text).splitlines()
+        for i, l in enumerate(lines):
+            screen.blit(render(l, font), (PosX // 2, PosY // 2 + 30 * i))
+        pygame.display.update()
 
 
-def settext(text: str, PosX: int, PosY: int):
-    global OverlayRunning
-    for event in pygame.event.get():
-        if event.type == pygame.QUIT:
-            OverlayRunning = 0
-    font = pygame.font.SysFont('Segoe UI Semibold', 30, False)
-    screen.fill(fuchsia)  # Transparent background
-    lines = str(text).splitlines()
-    for i, l in enumerate(lines):
-        screen.blit(render(l, font), (PosX // 2, PosY // 2 + 30 * i))
-    pygame.display.update()
-    
 def KillOverlay():
     pygame.display.quit()
-    OverlayRunning = False
-    
+
+
 def StatusOverlay():
-    return OverlayRunning
+    return pygame.display.get_active()
 
 
 def GetJobDirectory(JobName: str):
     database = ['Airline Pilot', 'Bus Driver', 'Business', 'Cargo Pilot', 'EMS', 'Farmer', 'Firefighter', 'Fisherman',
                 'Gambling', 'Garbage', 'Helicopter Pilot',
-                'Hunter', 'Mechanic', 'Miner', 'Player', 'Racer', 'Strength', 'Train Conductor', 'Trucking',   'PostOP']
+                'Hunter', 'Mechanic', 'Miner', 'Player', 'Racer', 'Strength', 'Train Conductor', 'Trucking', 'PostOP']
     score = 0
     for f in database:
         tempscore = fuzz.partial_ratio(f, JobName)
         if tempscore > score:
             score = tempscore
             AJobName = f
     match AJobName:
@@ -174,7 +157,15 @@
             return 'train train'
         case 'Trucking':
             return 'trucking trucking'
         case 'PostOP':
             return 'trucking postop'
     return None
 
+
+StartOverlay()
+
+print(pygame.display.get_active())
+
+KillOverlay()
+
+print(pygame.display.get_active())
```

### Comparing `MyOverlay-0.2.2/src/MyOverlay.egg-info/PKG-INFO` & `MyOverlay-0.2.3/src/MyOverlay.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.2.2
+Version: 0.2.3
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

