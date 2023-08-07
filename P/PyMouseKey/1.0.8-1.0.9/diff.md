# Comparing `tmp/PyMouseKey-1.0.8-py3-none-any.whl.zip` & `tmp/PyMouseKey-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 6644 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    21517 b- defN 23-Aug-04 06:41 pymousekey/__init__.py
--rw-rw-rw-  2.0 fat      470 b- defN 23-Aug-04 06:42 PyMouseKey-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 06:42 PyMouseKey-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-04 06:42 PyMouseKey-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      389 b- defN 23-Aug-04 06:42 PyMouseKey-1.0.8.dist-info/RECORD
-5 files, 22479 bytes uncompressed, 5918 bytes compressed:  73.7%
+Zip file size: 7046 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    23266 b- defN 23-Aug-07 08:28 pymousekey/__init__.py
+-rw-rw-rw-  2.0 fat      470 b- defN 23-Aug-07 08:28 PyMouseKey-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-07 08:28 PyMouseKey-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-07 08:28 PyMouseKey-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      389 b- defN 23-Aug-07 08:28 PyMouseKey-1.0.9.dist-info/RECORD
+5 files, 24228 bytes uncompressed, 6320 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: pymousekey/__init__.py
 Comment: 
 
-Filename: PyMouseKey-1.0.8.dist-info/METADATA
+Filename: PyMouseKey-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: PyMouseKey-1.0.8.dist-info/WHEEL
+Filename: PyMouseKey-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: PyMouseKey-1.0.8.dist-info/top_level.txt
+Filename: PyMouseKey-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: PyMouseKey-1.0.8.dist-info/RECORD
+Filename: PyMouseKey-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymousekey/__init__.py

```diff
@@ -163,20 +163,86 @@
     'winright': 0xDC + 1024,
     'apps': 0xDD + 1024,
     'right ctrl': 0x9D + 1024,
     'up arrow': ctypes.windll.user32.MapVirtualKeyW(0x26, 0),
     'left arrow': ctypes.windll.user32.MapVirtualKeyW(0x25, 0),
     'down arrow': ctypes.windll.user32.MapVirtualKeyW(0x28, 0),
     'right arrow': ctypes.windll.user32.MapVirtualKeyW(0x27, 0),
-    'xbutton1': 0x0001,
-    'xbutton2': 0x0002,
 }
 
-# For future use?
 VK_KEYS = {
+    "a": 0x41,
+    "b": 0x42,
+    "c": 0x43,
+    "d": 0x44,
+    "e": 0x45,
+    "f": 0x46,
+    "g": 0x47,
+    "h": 0x48,
+    "i": 0x49,
+    "j": 0x4a,
+    "k": 0x4b,
+    "l": 0x4c,
+    "m": 0x4d,
+    "n": 0x4e,
+    "o": 0x4f,
+    "p": 0x50,
+    "q": 0x51,
+    "r": 0x52,
+    "s": 0x53,
+    "t": 0x54,
+    "u": 0x55,
+    "v": 0x56,
+    "w": 0x57,
+    "x": 0x58,
+    "y": 0x59,
+    "z": 0x5a,
+    "1": 0x31,
+    "2": 0x32,
+    "3": 0x33,
+    "4": 0x34,
+    "5": 0x35,
+    "6": 0x36,
+    "7": 0x37,
+    "8": 0x38,
+    "9": 0x39,
+    "0": 0x30,
+    "-": 0xbd,
+    "=": 0xbb,
+    "!": 0x131,
+    "@": 0x132,
+    "#": 0x133,
+    "$": 0x134,
+    "%": 0x135,
+    "^": 0x136,
+    "&": 0x137,
+    "*": 0x138,
+    "(": 0x139,
+    ")": 0x130,
+    "_": 0x1bd,
+    "+": 0x1bb,
+    "[": 0xdb,
+    "]": 0xdd,
+    "\\": 0xdc,
+    "{": 0x1db,
+    "}": 0x1dd,
+    "|": 0x1dc,
+    ";": 0xba,
+    "'": 0xde,
+    ":": 0x1ba,
+    '"': 0x1de,
+    ",": 0xbc,
+    ".": 0xbe,
+    "/": 0xbf,
+    "<": 0x1bc,
+    ">": 0x1be,
+    "?": 0x1bf,
+    "*": 0x138,
+    "`": 0xc0,
+    "~": 0x1c0,
     'backspace': 0x08,
     'tab': 0x09,
     'clear': 0x0C,
     'enter': 0x0D,
     'shift': 0x10,
     'ctrl': 0x11,
     'alt': 0x12,
@@ -197,67 +263,26 @@
     'execute': 0x2B,
     'print screen': 0x2C,
     'prt sc': 0x2C,
     'prntsc': 0x2C,
     'ins': 0x2D,
     'del': 0x2E,
     'help': 0x2F,
-    '0': 0x30,
-    '1': 0x31,
-    '2': 0x32,
-    '3': 0x33,
-    '4': 0x34,
-    '5': 0x35,
-    '6': 0x36,
-    '7': 0x37,
-    '8': 0x38,
-    '9': 0x39,
-    'a': 0x41,
-    'b': 0x42,
-    'c': 0x43,
-    'd': 0x44,
-    'e': 0x45,
-    'f': 0x46,
-    'g': 0x47,
-    'h': 0x48,
-    'i': 0x49,
-    'j': 0x4A,
-    'k': 0x4B,
-    'l': 0x4C,
-    'm': 0x4D,
-    'n': 0x4E,
-    'o': 0x4F,
-    'p': 0x50,
-    'q': 0x51,
-    'r': 0x52,
-    's': 0x53,
-    't': 0x54,
-    'u': 0x55,
-    'v': 0x56,
-    'w': 0x57,
-    'x': 0x58,
-    'y': 0x59,
-    'z': 0x5A,
     'numpad 0': 0x60,
     'numpad 1': 0x61,
     'numpad 2': 0x62,
     'numpad 3': 0x63,
     'numpad 4': 0x64,
     'numpad 5': 0x65,
     'numpad 6': 0x66,
     'numpad 7': 0x67,
     'numpad 8': 0x68,
     'numpad 9': 0x69,
     'multiply': 0x6A,
-    'add': 0x6B,
-    '+': 0xBB,
-    ',': 0xBC,	
     'minus': 0xBD,
-    '-': 0xBD,
-    '.': 0xBE,
     'seperator': 0x6C,
     'subtract': 0x6D,
     'decimal': 0x6E,
     'divide': 0x6F,
     'f1': 0x70,
     'f2': 0x71,
     'f3': 0x72,
@@ -281,37 +306,26 @@
     'f21': 0x84,
     'f22': 0x85,
     'f23': 0x86,
     'f24': 0x87,
     'num lock': 0x90,
     'scroll lock': 0x91,
     'lshift': 0xA0,
-    'left shift': 0xA0,
     'rshift': 0xA1,
-    'right shift': 0xA1,
     'lcontrol': 0xA2,
     'lctrl': 0xA2,
-    'left control': 0xA2,
     'rcontrol': 0xA3,
     'rctrl': 0xA3,
-    'right control': 0xA3,
     'lalt': 0xA4,
-    'left alt': 0xA4,
     'ralt': 0xA5,
-    'right alt': 0xA5,
-    '?': 0xBF,
     'tilde': 0xC0,
-    '[': 0xDB,
-    '\\': 0xDC,
-    ']': 0xDD,
-    '"': 0xDE,
-    "'": 0xDE,
     'clear': 0xFE,
 }
 
+
 class KeyBdInput(ctypes.Structure):
     _fields_ = [("wVk", ctypes.c_ushort),
                 ("wScan", ctypes.c_ushort),
                 ("dwFlags", ctypes.c_ulong),
                 ("time", ctypes.c_ulong),
                 ("dwExtraInfo", ctypes.POINTER(ctypes.c_ulong))]
 
@@ -554,67 +568,99 @@
     ii_.ki = KeyBdInput(0, KEYS[key.lower()], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
     x = Input(ctypes.c_ulong(1), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
 
 def add_hotkey(key, callback, args=(), suppress=True):
     """
     Registers a system wide hotkey with optional args using ctypes and GetMessageW starting it in a seperate daemon thread\n
-    If suppress is true then block the original function of the key
-
-    """
-    def add_hotkey_thread(key, callback, args=()):
-        key_id = len(registered_hotkeys) + 1
-        registered_hotkeys[VK_KEYS[key]] = key_id
-        hotkey_threads[VK_KEYS[key]] = hotkey_thread.native_id
+    If suppress is true then block the original function of the key\n
+    If the specified key is already a registered hotkey the function returns nothing\n
+    Usage of how to add hotkeys:
+    -
+    add_hotkey("ctrl + shift + g")\n
+    add_hotkey("shift + numpad 5") (for shift + numpad keys dont actually work because of something to do with numlock and its secondary function)\n
+    add_hotkey("h")\n
+    """
+    def add_hotkey_thread():
+        if 'shift' in key or 'ctrl' in key or 'alt' in key:
+            registered_key = key.rsplit('+', 1)[1].strip()
+            key_id = len(registered_hotkeys) + 1
+            registered_hotkeys[key] = key_id, VK_KEYS[registered_key]
+            hotkey_threads[key] = hotkey_thread.native_id
+            if 'alt' in key and not 'ctrl' in key and not 'shift' in key:
+                fsModifiers = 0x0001
+            elif 'ctrl' in key and not 'alt' in key and not 'shift' in key:
+                fsModifiers = 0x0002
+            elif 'shift' in key and not 'ctrl' in key and not 'alt' in key:
+                fsModifiers = 0x0004
+            elif 'alt' in key and 'ctrl' in key:
+                fsModifiers = 0x0001 | 0x0002
+            elif 'alt' in key and 'shift' in key:
+                fsModifiers = 0x0001 | 0x0004
+            elif 'shift' in key and 'ctrl' in key:
+                fsModifiers = 0x0004 | 0x0002
+        else:
+            registered_key = key
+            key_id = len(registered_hotkeys) + 1
+            registered_hotkeys[key] = key_id, VK_KEYS[registered_key]
+            hotkey_threads[registered_key] = hotkey_thread.native_id
+            fsModifiers = None
 
-        ctypes.windll.user32.RegisterHotKey(None, key_id , None, VK_KEYS[key])
+        ctypes.windll.user32.RegisterHotKey(None, key_id , fsModifiers, VK_KEYS[registered_key])
         
         msg = ctypes.wintypes.MSG()
 
         while ctypes.windll.user32.GetMessageW(ctypes.byref(msg), 0, 0, 0) != 0:
             if msg.message == WM_HOTKEY:
                 if args:
                     callback(args)
                 else:
                     callback()
                 if not suppress:
-                    ctypes.windll.user32.UnregisterHotKey(None, key_id , None, VK_KEYS[key])
+                    ctypes.windll.user32.UnregisterHotKey(None, key_id , fsModifiers, VK_KEYS[registered_key])
                     press(key, 0, False)
-                    ctypes.windll.user32.RegisterHotKey(None, key_id , None, VK_KEYS[key])
+                    ctypes.windll.user32.RegisterHotKey(None, key_id , fsModifiers, VK_KEYS[registered_key])
                 ctypes.windll.user32.TranslateMessage(ctypes.byref(msg))
                 ctypes.windll.user32.DispatchMessageW(ctypes.byref(msg))
-        
         try:
-            ctypes.windll.user32.UnregisterHotKey(None, registered_hotkeys[VK_KEYS[key]])
+            ctypes.windll.user32.UnregisterHotKey(None, registered_hotkeys[key][0])
         except(KeyError):
             pass
-    if key in VK_KEYS:
-        hotkey_thread = threading.Thread(target=add_hotkey_thread, args=[key, callback, args])
+
+    if key in registered_hotkeys:
+        return
+
+    elif key in VK_KEYS:
+        hotkey_thread = threading.Thread(target=add_hotkey_thread)
+        hotkey_thread.daemon = True
+        hotkey_thread.start()
+    elif key.rsplit('+', 1)[1].strip() in VK_KEYS:
+        hotkey_thread = threading.Thread(target=add_hotkey_thread)
         hotkey_thread.daemon = True
         hotkey_thread.start()
 
 
 def remove_hotkey(key):
     """
     Unregisters and removes the specified hotkey if it was registered previously
 
     """
-    if VK_KEYS[key] in registered_hotkeys:
-        ctypes.windll.user32.UnregisterHotKey(None, registered_hotkeys[VK_KEYS[key]])
-        ctypes.windll.user32.PostThreadMessageW(hotkey_threads[VK_KEYS[key]], WM_QUIT, 0, 0)
-        del registered_hotkeys[VK_KEYS[key]]
-        del hotkey_threads[VK_KEYS[key]]
+    if key in registered_hotkeys:
+        ctypes.windll.user32.UnregisterHotKey(None, registered_hotkeys[key][0])
+        ctypes.windll.user32.PostThreadMessageW(hotkey_threads[key], WM_QUIT, 0, 0)
+        del registered_hotkeys[key]
+        del hotkey_threads[key]
 
 def remove_all_hotkeys():
     """
     Unregisters and removes all currently registered hotkeys
     
     """
     for key in registered_hotkeys.values():
-        ctypes.windll.user32.UnregisterHotKey(None, key)
+        ctypes.windll.user32.UnregisterHotKey(None, key[0])
         
     for threads in hotkey_threads.values():
         ctypes.windll.user32.PostThreadMessageW(threads, WM_QUIT, 0, 0)
 
     registered_hotkeys.clear()
     hotkey_threads.clear()
 
@@ -653,15 +699,15 @@
     rgbColor = red, green, blue
     return hexColor, rgbColor
 
 
 def controlSend(key=None, className=None, windowTitle=None, lparam=None):
     """
     Sends software keyboard inputs to any inactive window/control by sending the WM_ACTIVATE msg and WA_ACTIVE wParam then sending the WH_CHAR message with the key you specified\n
-    key(string): The key is being sent using ord() so only 1 length strings are allowed such as "a" or ";"\n
+    key(string): The key is being sent using ord() so only no modifier keys are allowed only keys such as "a" ";" "1" etc\n
     
     Note:
     -------
     Some games/windows only take the hardware inputs as an option so if you dont see any results this is why
 
     """
     handle = ctypes.windll.user32.FindWindowW(className, windowTitle)
```

