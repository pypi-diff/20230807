# Comparing `tmp/gamey-0.4.tar.gz` & `tmp/gamey-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamey-0.4.tar", max compression
+gzip compressed data, was "gamey-0.5.tar", max compression
```

## Comparing `gamey-0.4.tar` & `gamey-0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       51 2023-08-06 19:53:31.483350 gamey-0.4/README.md
--rw-r--r--   0        0        0     2865 2023-08-07 11:28:50.566745 gamey-0.4/gamey/__init__.py
--rw-r--r--   0        0        0      307 2023-08-07 11:30:38.430080 gamey-0.4/pyproject.toml
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 gamey-0.4/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-08-06 19:53:31.483350 gamey-0.5/README.md
+-rw-r--r--   0        0        0     3613 2023-08-07 11:58:57.630110 gamey-0.5/gamey/__init__.py
+-rw-r--r--   0        0        0      307 2023-08-07 11:35:06.473418 gamey-0.5/pyproject.toml
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 gamey-0.5/PKG-INFO
```

### Comparing `gamey-0.4/gamey/__init__.py` & `gamey-0.5/gamey/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 		self.window = p.display.set_mode((width, height))
 		p.display.set_caption(title)
 
 		self.background = (255, 255, 255)
 
 		self.sprites = []
+		self.objects = []
 		self.events = {}
 		self.runlist = []
 		
 		self.add_default_events()
 
 		last_window = self
 
@@ -56,16 +57,14 @@
 
 	def close(self, event):
 		p.quit()
 		quit()
 
 class Sprite:
 
-	
-
 	def __init__(self, image_path, x=0, y=0):
 		self.image = p.image.load(image_path)
 		self.x = x
 		self.y = y
 		self.width = self.image.get_width()
 		self.height = self.image.get_height()
 		last_window.sprites.append(self)
@@ -111,15 +110,43 @@
 			self.MOVING_DOWN = False
 		if event.key in self.KEYS_LEFT:
 			self.MOVING_LEFT = False
 		if event.key in self.KEYS_RIGHT:
 			self.MOVING_RIGHT = False
 
 	def check_motion(self):
+		old_pos = (self.sprite.x, self.sprite.y)
 		if self.MOVING_UP:
 			self.sprite.y -= self.speed
 		if self.MOVING_DOWN:
 			self.sprite.y += self.speed
 		if self.MOVING_LEFT:
 			self.sprite.x -= self.speed
 		if self.MOVING_RIGHT:
 			self.sprite.x += self.speed
+
+		x = self.sprite.x
+		y = self.sprite.y
+		xr = x + self.sprite.width
+		yb = y + self.sprite.height
+
+		
+		
+		for obj in last_window.objects:
+
+			obj.x_left = obj.sprite.x
+			obj.x_right = obj.sprite.x + obj.sprite.width
+			obj.y_top = obj.sprite.y
+			obj.y_bottom = obj.sprite.y + obj.sprite.height
+
+			if x > obj.x_left and x < obj.x_right:
+				if y > obj.y_top and y < obj.y_bottom:
+					self.sprite.x, self.sprite.y = old_pos
+			if xr > obj.x_left and xr < obj.x_right:
+				print(obj.y_bottom)
+				if yb > obj.y_top and yb < obj.y_bottom:
+					self.sprite.x, self.sprite.y = old_pos
+
+class Object:
+	def __init__(self, sprite):
+		self.sprite = sprite
+		last_window.objects.append(self)
```

### Comparing `gamey-0.4/PKG-INFO` & `gamey-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamey
-Version: 0.4
+Version: 0.5
 Summary: An simple, powerful game engine built on pygame
 Author: Dylan Rogers
 Author-email: opendylan@proton.me
 Requires-Python: >=3,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

