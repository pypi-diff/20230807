# Comparing `tmp/gamey-0.5.tar.gz` & `tmp/gamey-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamey-0.5.tar", max compression
+gzip compressed data, was "gamey-0.6.tar", max compression
```

## Comparing `gamey-0.5.tar` & `gamey-0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       51 2023-08-06 19:53:31.483350 gamey-0.5/README.md
--rw-r--r--   0        0        0     3613 2023-08-07 11:58:57.630110 gamey-0.5/gamey/__init__.py
--rw-r--r--   0        0        0      307 2023-08-07 11:35:06.473418 gamey-0.5/pyproject.toml
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 gamey-0.5/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-08-06 19:53:31.483350 gamey-0.6/README.md
+-rw-r--r--   0        0        0     5176 2023-08-07 17:09:03.190001 gamey-0.6/gamey/__init__.py
+-rw-r--r--   0        0        0      307 2023-08-07 17:07:56.596667 gamey-0.6/pyproject.toml
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 gamey-0.6/PKG-INFO
```

### Comparing `gamey-0.5/gamey/__init__.py` & `gamey-0.6/gamey/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -63,30 +63,86 @@
 
 	def __init__(self, image_path, x=0, y=0):
 		self.image = p.image.load(image_path)
 		self.x = x
 		self.y = y
 		self.width = self.image.get_width()
 		self.height = self.image.get_height()
+		self.direction = 0
+
 		last_window.sprites.append(self)
 
 	def set_size(self, width, height=None):
 		if not height:
 			height = width
 		self.width = width
 		self.height = height
 		self.image = p.transform.scale(self.image, (self.width, self.height))
+	
+	def goto(self, x, y):
+		self.x = x
+		self.y = y
+
+	def change_x(self, distance):
+		self.x += distance
+
+	def change_y(self, distance):
+		self.y += distance
+	
+	def move(self, x, y):
+		self.change_x(x)
+		self.change_y(y)
+
+	def move_left(self, distance):
+		self.change_x(-distance)
+
+	def move_right(self, distance):
+		self.change_x(distance)
+
+	def move_up(self, distance):
+		self.change_y(-distance)
+
+	def move_down(self, distance):
+		self.change_y(distance)
+
+	def step(self, distance, direction="optional"):
+		if direction == "optional":
+			direction = self.direction
+		if direction == 0:
+			self.move_right(distance)
+		if direction == 1:
+			self.move_down(distance)
+		if direction == 2:
+			self.move_left(distance)
+		if direction == 3:
+			self.move_up(distance)
+
+	def look(self, direction=0):
+		self.direction = direction
+
+	def look_right(self):
+		self.look(0)
+
+	def look_down(self):
+		self.look(1)
+
+	def look_left(self):
+		self.look(2)
+
+	def look_up(self):
+		self.look(3)
 
 class Player:
 
-	def __init__(self, sprite, movement_speed=100):
+	def __init__(self, sprite, controller="default", movement_speed=100):
 		last_window.add_event(p.KEYDOWN, self.keydown)
 		last_window.add_event(p.KEYUP, self.keyup)
 		self.sprite = sprite
 		self.speed = movement_speed / FPS
+		self.controller = controller
 
 		self.KEYS_UP     =  [p.K_w, p.K_UP]
 		self.KEYS_DOWN   =  [p.K_s, p.K_DOWN]
 		self.KEYS_LEFT   =  [p.K_a, p.K_LEFT]
 		self.KEYS_RIGHT  =  [p.K_d, p.K_RIGHT]
 
 		self.MOVING_UP = self.MOVING_DOWN = self.MOVING_LEFT = self.MOVING_RIGHT = False
@@ -110,43 +166,64 @@
 			self.MOVING_DOWN = False
 		if event.key in self.KEYS_LEFT:
 			self.MOVING_LEFT = False
 		if event.key in self.KEYS_RIGHT:
 			self.MOVING_RIGHT = False
 
 	def check_motion(self):
-		old_pos = (self.sprite.x, self.sprite.y)
-		if self.MOVING_UP:
-			self.sprite.y -= self.speed
-		if self.MOVING_DOWN:
-			self.sprite.y += self.speed
-		if self.MOVING_LEFT:
-			self.sprite.x -= self.speed
-		if self.MOVING_RIGHT:
-			self.sprite.x += self.speed
+
+		if self.controller == "default":
+			old_pos = (self.sprite.x, self.sprite.y)
+			if self.MOVING_UP:
+				self.sprite.y -= self.speed
+			if self.MOVING_DOWN:
+				self.sprite.y += self.speed
+			if self.MOVING_LEFT:
+				self.sprite.x -= self.speed
+			if self.MOVING_RIGHT:
+				self.sprite.x += self.speed
+				
+		if self.controller == "look":
+			if self.MOVING_UP:
+				self.sprite.y -= self.speed
+			if self.MOVING_DOWN:
+				self.sprite.y += self.speed
+			if self.MOVING_LEFT:
+				self.sprite.x -= self.speed
+			if self.MOVING_RIGHT:
+				self.sprite.x += self.speed
 
 		x = self.sprite.x
 		y = self.sprite.y
 		xr = x + self.sprite.width
 		yb = y + self.sprite.height
-
-		
 		
 		for obj in last_window.objects:
 
+			if not obj.on_collision == "block":
+				continue
+
 			obj.x_left = obj.sprite.x
 			obj.x_right = obj.sprite.x + obj.sprite.width
 			obj.y_top = obj.sprite.y
 			obj.y_bottom = obj.sprite.y + obj.sprite.height
 
 			if x > obj.x_left and x < obj.x_right:
 				if y > obj.y_top and y < obj.y_bottom:
 					self.sprite.x, self.sprite.y = old_pos
 			if xr > obj.x_left and xr < obj.x_right:
 				print(obj.y_bottom)
 				if yb > obj.y_top and yb < obj.y_bottom:
 					self.sprite.x, self.sprite.y = old_pos
 
 class Object:
-	def __init__(self, sprite):
+
+	def __init__(self, sprite, on_collision="block"):
 		self.sprite = sprite
+		self.on_collision = on_collision
 		last_window.objects.append(self)
+
+class TileMap:
+
+	def __init__(self, width=16, height=12):
+		self.width = width
+		self.height = height
```

### Comparing `gamey-0.5/PKG-INFO` & `gamey-0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamey
-Version: 0.5
+Version: 0.6
 Summary: An simple, powerful game engine built on pygame
 Author: Dylan Rogers
 Author-email: opendylan@proton.me
 Requires-Python: >=3,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

