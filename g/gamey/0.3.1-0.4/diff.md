# Comparing `tmp/gamey-0.3.1.tar.gz` & `tmp/gamey-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamey-0.3.1.tar", max compression
+gzip compressed data, was "gamey-0.4.tar", max compression
```

## Comparing `gamey-0.3.1.tar` & `gamey-0.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       51 2023-08-06 19:53:31.483350 gamey-0.3.1/README.md
--rw-r--r--   0        0        0     1327 2023-08-07 10:25:39.146677 gamey-0.3.1/gamey/__init__.py
--rw-r--r--   0        0        0      309 2023-08-07 10:25:58.696678 gamey-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 gamey-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-08-06 19:53:31.483350 gamey-0.4/README.md
+-rw-r--r--   0        0        0     2865 2023-08-07 11:28:50.566745 gamey-0.4/gamey/__init__.py
+-rw-r--r--   0        0        0      307 2023-08-07 11:30:38.430080 gamey-0.4/pyproject.toml
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 gamey-0.4/PKG-INFO
```

### Comparing `gamey-0.3.1/gamey/__init__.py` & `gamey-0.4/gamey/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import pygame as p
 
 p.init()
 
 last_window = None
 
+FPS = 60
+clock = p.time.Clock()
+
 class Window:
 
 	def __init__(self, title="Gamie Window", width=800, height=600):
 		global last_window
 
 		self.window = p.display.set_mode((width, height))
 		p.display.set_caption(title)
 
 		self.background = (255, 255, 255)
 
 		self.sprites = []
-
 		self.events = {}
+		self.runlist = []
+		
 		self.add_default_events()
 
 		last_window = self
 
 	def add_event(self, event_type, callback):
 		if str(event_type) not in self.events:
 			self.events[str(event_type)] = []
@@ -37,27 +41,85 @@
 					for callback in self.events[str(event.type)]:
 						callback(event)
 
 			self.window.fill(self.background)
 
 			for sprite in self.sprites:
 				self.window.blit(sprite.image, (sprite.x, sprite.y))
-			
+
+			for i in self.runlist:
+				i()
+
 			p.display.flip()
 			p.display.update()
 
+			clock.tick(FPS)
+
 	def close(self, event):
 		p.quit()
 		quit()
 
 class Sprite:
 
+	
+
 	def __init__(self, image_path, x=0, y=0):
 		self.image = p.image.load(image_path)
 		self.x = x
 		self.y = y
+		self.width = self.image.get_width()
+		self.height = self.image.get_height()
 		last_window.sprites.append(self)
 
 	def set_size(self, width, height=None):
 		if not height:
 			height = width
-		self.image = p.transform.scale(self.image, (width, height))
+		self.width = width
+		self.height = height
+		self.image = p.transform.scale(self.image, (self.width, self.height))
+
+class Player:
+
+	def __init__(self, sprite, movement_speed=100):
+		last_window.add_event(p.KEYDOWN, self.keydown)
+		last_window.add_event(p.KEYUP, self.keyup)
+		self.sprite = sprite
+		self.speed = movement_speed / FPS
+
+		self.KEYS_UP     =  [p.K_w, p.K_UP]
+		self.KEYS_DOWN   =  [p.K_s, p.K_DOWN]
+		self.KEYS_LEFT   =  [p.K_a, p.K_LEFT]
+		self.KEYS_RIGHT  =  [p.K_d, p.K_RIGHT]
+
+		self.MOVING_UP = self.MOVING_DOWN = self.MOVING_LEFT = self.MOVING_RIGHT = False
+	
+		last_window.runlist.append(self.check_motion)
+	
+	def keydown(self, event):
+		if event.key in self.KEYS_UP:
+			self.MOVING_UP = True
+		if event.key in self.KEYS_DOWN:
+			self.MOVING_DOWN = True
+		if event.key in self.KEYS_LEFT:
+			self.MOVING_LEFT = True
+		if event.key in self.KEYS_RIGHT:
+			self.MOVING_RIGHT = True
+
+	def keyup(self, event):
+		if event.key in self.KEYS_UP:
+			self.MOVING_UP = False
+		if event.key in self.KEYS_DOWN:
+			self.MOVING_DOWN = False
+		if event.key in self.KEYS_LEFT:
+			self.MOVING_LEFT = False
+		if event.key in self.KEYS_RIGHT:
+			self.MOVING_RIGHT = False
+
+	def check_motion(self):
+		if self.MOVING_UP:
+			self.sprite.y -= self.speed
+		if self.MOVING_DOWN:
+			self.sprite.y += self.speed
+		if self.MOVING_LEFT:
+			self.sprite.x -= self.speed
+		if self.MOVING_RIGHT:
+			self.sprite.x += self.speed
```

### Comparing `gamey-0.3.1/PKG-INFO` & `gamey-0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamey
-Version: 0.3.1
+Version: 0.4
 Summary: An simple, powerful game engine built on pygame
 Author: Dylan Rogers
 Author-email: opendylan@proton.me
 Requires-Python: >=3,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

