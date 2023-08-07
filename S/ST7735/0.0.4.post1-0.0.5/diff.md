# Comparing `tmp/ST7735-0.0.4.post1.tar.gz` & `tmp/ST7735-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ST7735-0.0.4.post1.tar", last modified: Mon Sep  6 12:54:28 2021, max compression
+gzip compressed data, was "ST7735-0.0.5.tar", last modified: Mon Aug  7 10:35:49 2023, max compression
```

## Comparing `ST7735-0.0.4.post1.tar` & `ST7735-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 phil      (1000) phil      (1000)        0 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/
--rwxrwxrwx   0 phil      (1000) phil      (1000)      514 2021-09-06 12:41:32.000000 ST7735-0.0.4.post1/CHANGELOG.txt
--rwxrwxrwx   0 phil      (1000) phil      (1000)     1091 2021-09-06 11:43:55.000000 ST7735-0.0.4.post1/LICENSE.txt
--rwxrwxrwx   0 phil      (1000) phil      (1000)      112 2021-09-06 11:43:55.000000 ST7735-0.0.4.post1/MANIFEST.in
--rwxrwxrwx   0 phil      (1000) phil      (1000)     4800 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/PKG-INFO
--rwxrwxrwx   0 phil      (1000) phil      (1000)     3345 2021-09-06 12:43:54.000000 ST7735-0.0.4.post1/README.md
--rwxrwxrwx   0 phil      (1000) phil      (1000)     1065 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/setup.cfg
--rwxrwxrwx   0 phil      (1000) phil      (1000)     1415 2021-09-06 11:43:55.000000 ST7735-0.0.4.post1/setup.py
-drwxrwxrwx   0 phil      (1000) phil      (1000)        0 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/ST7735/
--rwxrwxrwx   0 phil      (1000) phil      (1000)    13474 2021-09-06 11:43:55.000000 ST7735-0.0.4.post1/ST7735/__init__.py
-drwxrwxrwx   0 phil      (1000) phil      (1000)        0 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/ST7735.egg-info/
--rwxrwxrwx   0 phil      (1000) phil      (1000)        1 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/ST7735.egg-info/dependency_links.txt
--rwxrwxrwx   0 phil      (1000) phil      (1000)     4800 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/ST7735.egg-info/PKG-INFO
--rwxrwxrwx   0 phil      (1000) phil      (1000)       12 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/ST7735.egg-info/requires.txt
--rwxrwxrwx   0 phil      (1000) phil      (1000)      234 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/ST7735.egg-info/SOURCES.txt
--rwxrwxrwx   0 phil      (1000) phil      (1000)        7 2021-09-06 12:54:28.000000 ST7735-0.0.4.post1/ST7735.egg-info/top_level.txt
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-08-07 10:35:49.596035 ST7735-0.0.5/
+-rw-r--r--   0 phil      (1000) phil      (1000)      599 2023-08-07 10:33:42.000000 ST7735-0.0.5/CHANGELOG.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)     1070 2023-08-07 08:25:42.000000 ST7735-0.0.5/LICENSE.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)      107 2023-08-07 08:25:42.000000 ST7735-0.0.5/MANIFEST.in
+-rw-r--r--   0 phil      (1000) phil      (1000)     4958 2023-08-07 10:35:49.596035 ST7735-0.0.5/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)     3363 2023-08-07 10:35:44.000000 ST7735-0.0.5/README.md
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-08-07 10:35:49.592035 ST7735-0.0.5/ST7735/
+-rw-r--r--   0 phil      (1000) phil      (1000)    13514 2023-08-07 10:34:10.000000 ST7735-0.0.5/ST7735/__init__.py
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-08-07 10:35:49.596035 ST7735-0.0.5/ST7735.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     4958 2023-08-07 10:35:49.000000 ST7735-0.0.5/ST7735.egg-info/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)      234 2023-08-07 10:35:49.000000 ST7735-0.0.5/ST7735.egg-info/SOURCES.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)        1 2023-08-07 10:35:49.000000 ST7735-0.0.5/ST7735.egg-info/dependency_links.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)       12 2023-08-07 10:35:49.000000 ST7735-0.0.5/ST7735.egg-info/requires.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)        7 2023-08-07 10:35:49.000000 ST7735-0.0.5/ST7735.egg-info/top_level.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)     1108 2023-08-07 10:35:49.596035 ST7735-0.0.5/setup.cfg
+-rw-r--r--   0 phil      (1000) phil      (1000)     1385 2023-08-07 08:25:42.000000 ST7735-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ST7735-0.0.4.post1/LICENSE.txt` & `ST7735-0.0.5/LICENSE.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 Pimoroni Ltd.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2018 Pimoroni Ltd.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ST7735-0.0.4.post1/PKG-INFO` & `ST7735-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ST7735
-Version: 0.0.4.post1
+Version: 0.0.5
 Summary: Library to control an ST7735 168x80 TFT LCD display.
 Home-page: https://www.pimoroni.com
 Author: Philip Howard
 Author-email: phil@pimoroni.com
 License: MIT
 Project-URL: GitHub, https://www.github.com/pimoroni/st7735-python
 Description: # Python ST7735
@@ -72,14 +72,20 @@
         Adafruit invests time and resources providing this open source code, please support Adafruit and open-source hardware by purchasing products from Adafruit!
         
         Modified from 'Modified from 'Adafruit Python ILI9341' written by Tony DiCola for Adafruit Industries.' written by Clement Skau.
         
         MIT license, all text above must be included in any redistribution
         
         # Changelog
+        0.0.5
+        -----
+        
+        * Add support for choosing between BGR/RGB displays
+        * Add methods for display power and sleep control
+        
         0.0.4-post1
         -----------
         
         * Repackage with Markdown README/setup.cfg
         * Fix `__version__` to 0.0.4
         * Update dependencies in README
```

### Comparing `ST7735-0.0.4.post1/README.md` & `ST7735-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,106 @@
-# Python ST7735
-
-[![Build Status](https://travis-ci.com/pimoroni/st7735-python.svg?branch=master)](https://travis-ci.com/pimoroni/st7735-python)
-[![Coverage Status](https://coveralls.io/repos/github/pimoroni/st7735-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/st7735-python?branch=master)
-[![PyPi Package](https://img.shields.io/pypi/v/st7735.svg)](https://pypi.python.org/pypi/st7735)
-[![Python Versions](https://img.shields.io/pypi/pyversions/st7735.svg)](https://pypi.python.org/pypi/st7735)
-
-
-Python library to control an ST7735 TFT LCD display. Allows simple drawing on the display without installing a kernel module.
-
-Designed specifically to work with a ST7735 based 160x80 pixel TFT SPI display. (Specifically the 0.96" SPI LCD from Pimoroni).
-
-## Installing
-
-### Python 2
-
-Make sure you have the following dependencies:
-
-````
-sudo apt update
-sudo apt install python-rpi.gpio python-spidev python-pip python-pil python-numpy
-````
-
-Install this library by running:
-
-````
-sudo pip install st7735
-````
-
-### Python 3
-
-Make sure you have the following dependencies:
-
-````
-sudo apt update
-sudo apt install python3-rpi.gpio python3-spidev python3-pip python3-pil python3-numpy
-````
-
-Install this library by running:
-
-````
-sudo python3 -m pip install st7735
-````
-
-See example of usage in the examples folder.
-
-
-# Licensing & History
-
-This library is a modification of a modification of code originally written by Tony DiCola for Adafruit Industries, and modified to work with the ST7735 by Clement Skau.
-
-It has been modified by Pimoroni to include support for their 160x80 SPI LCD breakout, and hopefully also generalised enough so that it will support other ST7735-powered displays.
-
-## Modifications include:
-
-* PIL/Pillow has been removed from the underlying display driver to separate concerns- you should create your own PIL image and display it using `display(image)`
-* `width`, `height`, `rotation`, `invert`, `offset_left` and `offset_top` parameters can be passed into `__init__` for alternate displays
-* `Adafruit_GPIO` has been replaced with `RPi.GPIO` and `spidev` to closely align with our other software (IE: Raspberry Pi only)
-* Test fixtures have been added to keep this library stable
-
-Pimoroni invests time and resources forking and modifying this open source code, please support Pimoroni and open-source software by purchasing products from us, too!
-
-Adafruit invests time and resources providing this open source code, please support Adafruit and open-source hardware by purchasing products from Adafruit!
-
-Modified from 'Modified from 'Adafruit Python ILI9341' written by Tony DiCola for Adafruit Industries.' written by Clement Skau.
-
-MIT license, all text above must be included in any redistribution
+# Python ST7735
+
+[![Build Status](https://travis-ci.com/pimoroni/st7735-python.svg?branch=master)](https://travis-ci.com/pimoroni/st7735-python)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/st7735-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/st7735-python?branch=master)
+[![PyPi Package](https://img.shields.io/pypi/v/st7735.svg)](https://pypi.python.org/pypi/st7735)
+[![Python Versions](https://img.shields.io/pypi/pyversions/st7735.svg)](https://pypi.python.org/pypi/st7735)
+
+
+Python library to control an ST7735 TFT LCD display. Allows simple drawing on the display without installing a kernel module.
+
+Designed specifically to work with a ST7735 based 160x80 pixel TFT SPI display. (Specifically the 0.96" SPI LCD from Pimoroni).
+
+## Installing
+
+### Python 2
+
+Make sure you have the following dependencies:
+
+````
+sudo apt update
+sudo apt install python-rpi.gpio python-spidev python-pip python-pil python-numpy
+````
+
+Install this library by running:
+
+````
+sudo pip install st7735
+````
+
+### Python 3
+
+Make sure you have the following dependencies:
+
+````
+sudo apt update
+sudo apt install python3-rpi.gpio python3-spidev python3-pip python3-pil python3-numpy
+````
+
+Install this library by running:
+
+````
+sudo python3 -m pip install st7735
+````
+
+See example of usage in the examples folder.
+
+
+# Licensing & History
+
+This library is a modification of a modification of code originally written by Tony DiCola for Adafruit Industries, and modified to work with the ST7735 by Clement Skau.
+
+It has been modified by Pimoroni to include support for their 160x80 SPI LCD breakout, and hopefully also generalised enough so that it will support other ST7735-powered displays.
+
+## Modifications include:
+
+* PIL/Pillow has been removed from the underlying display driver to separate concerns- you should create your own PIL image and display it using `display(image)`
+* `width`, `height`, `rotation`, `invert`, `offset_left` and `offset_top` parameters can be passed into `__init__` for alternate displays
+* `Adafruit_GPIO` has been replaced with `RPi.GPIO` and `spidev` to closely align with our other software (IE: Raspberry Pi only)
+* Test fixtures have been added to keep this library stable
+
+Pimoroni invests time and resources forking and modifying this open source code, please support Pimoroni and open-source software by purchasing products from us, too!
+
+Adafruit invests time and resources providing this open source code, please support Adafruit and open-source hardware by purchasing products from Adafruit!
+
+Modified from 'Modified from 'Adafruit Python ILI9341' written by Tony DiCola for Adafruit Industries.' written by Clement Skau.
+
+MIT license, all text above must be included in any redistribution
 
 # Changelog
-0.0.4-post1
------------
-
-* Repackage with Markdown README/setup.cfg
-* Fix `__version__` to 0.0.4
-* Update dependencies in README
-
-0.0.4
------
-
-* Depend upon spidev==3.4.0 for stability fixes
-* Switch from manual data chunking to spidev.xfer3()
-
-
-0.0.3
------
-
-* Fixed backlight pin
-* Added `set_backlight`
-* Added constants BG_SPI_CS_FRONT and BG_SPI_CS_BACK
-* Added module `__version__`
-
-0.0.2
------
-
-* Support for multiple display sizes/orientations
-
-0.0.1
------
-
-* Initial Release
+0.0.5
+-----
+
+* Add support for choosing between BGR/RGB displays
+* Add methods for display power and sleep control
+
+0.0.4-post1
+-----------
+
+* Repackage with Markdown README/setup.cfg
+* Fix `__version__` to 0.0.4
+* Update dependencies in README
+
+0.0.4
+-----
+
+* Depend upon spidev==3.4.0 for stability fixes
+* Switch from manual data chunking to spidev.xfer3()
+
+
+0.0.3
+-----
+
+* Fixed backlight pin
+* Added `set_backlight`
+* Added constants BG_SPI_CS_FRONT and BG_SPI_CS_BACK
+* Added module `__version__`
+
+0.0.2
+-----
+
+* Support for multiple display sizes/orientations
+
+0.0.1
+-----
+
+* Initial Release
```

### Comparing `ST7735-0.0.4.post1/setup.cfg` & `ST7735-0.0.5/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ST7735
-version = 0.0.4-post1
+version = 0.0.5
 author = Philip Howard
 author_email = phil@pimoroni.com
 description = Library to control an ST7735 168x80 TFT LCD display.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Raspberry Pi
 url = https://www.pimoroni.com
@@ -40,14 +40,17 @@
 
 [pimoroni]
 py3only = false
 py2deps = 
 	python-pil
 py3deps = 
 	python3-pil
+	python3-numpy
+	python3-spidev
+	python3-rpi.gpio
 configtxt = 
 commands = 
 	printf "Setting up SPI...\n"
 	raspi-config nonint do_spi 0
 
 [egg_info]
 tag_build =
```

### Comparing `ST7735-0.0.4.post1/setup.py` & `ST7735-0.0.5/setup.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-Copyright (c) 2016 Pimoroni
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from setuptools import setup, __version__
-from pkg_resources import parse_version
-
-minimum_version = parse_version('30.4.0')
-
-if parse_version(__version__) < minimum_version:
-    raise RuntimeError("Package setuptools must be at least version {}".format(minimum_version))
-
-setup()
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""
+Copyright (c) 2016 Pimoroni
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from setuptools import setup, __version__
+from pkg_resources import parse_version
+
+minimum_version = parse_version('30.4.0')
+
+if parse_version(__version__) < minimum_version:
+    raise RuntimeError("Package setuptools must be at least version {}".format(minimum_version))
+
+setup()
```

### Comparing `ST7735-0.0.4.post1/ST7735/__init__.py` & `ST7735-0.0.5/ST7735/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,400 +1,416 @@
-# Copyright (c) 2014 Adafruit Industries
-# Author: Tony DiCola
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-# THE SOFTWARE.
-import numbers
-import time
-import numpy as np
-
-import spidev
-import RPi.GPIO as GPIO
-
-
-__version__ = '0.0.4'
-
-BG_SPI_CS_BACK = 0
-BG_SPI_CS_FRONT = 1
-
-SPI_CLOCK_HZ = 16000000
-
-# Constants for interacting with display registers.
-ST7735_TFTWIDTH = 80
-ST7735_TFTHEIGHT = 160
-
-ST7735_COLS = 132
-ST7735_ROWS = 162
-
-ST7735_NOP = 0x00
-ST7735_SWRESET = 0x01
-ST7735_RDDID = 0x04
-ST7735_RDDST = 0x09
-
-ST7735_SLPIN = 0x10
-ST7735_SLPOUT = 0x11
-ST7735_PTLON = 0x12
-ST7735_NORON = 0x13
-
-ST7735_INVOFF = 0x20
-ST7735_INVON = 0x21
-ST7735_DISPOFF = 0x28
-ST7735_DISPON = 0x29
-
-ST7735_CASET = 0x2A
-ST7735_RASET = 0x2B
-ST7735_RAMWR = 0x2C
-ST7735_RAMRD = 0x2E
-
-ST7735_PTLAR = 0x30
-ST7735_MADCTL = 0x36
-ST7735_COLMOD = 0x3A
-
-ST7735_FRMCTR1 = 0xB1
-ST7735_FRMCTR2 = 0xB2
-ST7735_FRMCTR3 = 0xB3
-ST7735_INVCTR = 0xB4
-ST7735_DISSET5 = 0xB6
-
-
-ST7735_PWCTR1 = 0xC0
-ST7735_PWCTR2 = 0xC1
-ST7735_PWCTR3 = 0xC2
-ST7735_PWCTR4 = 0xC3
-ST7735_PWCTR5 = 0xC4
-ST7735_VMCTR1 = 0xC5
-
-ST7735_RDID1 = 0xDA
-ST7735_RDID2 = 0xDB
-ST7735_RDID3 = 0xDC
-ST7735_RDID4 = 0xDD
-
-ST7735_GMCTRP1 = 0xE0
-ST7735_GMCTRN1 = 0xE1
-
-ST7735_PWCTR6 = 0xFC
-
-# Colours for convenience
-ST7735_BLACK = 0x0000  # 0b 00000 000000 00000
-ST7735_BLUE = 0x001F  # 0b 00000 000000 11111
-ST7735_GREEN = 0x07E0  # 0b 00000 111111 00000
-ST7735_RED = 0xF800  # 0b 11111 000000 00000
-ST7735_CYAN = 0x07FF  # 0b 00000 111111 11111
-ST7735_MAGENTA = 0xF81F  # 0b 11111 000000 11111
-ST7735_YELLOW = 0xFFE0  # 0b 11111 111111 00000
-ST7735_WHITE = 0xFFFF  # 0b 11111 111111 11111
-
-
-def color565(r, g, b):
-    """Convert red, green, blue components to a 16-bit 565 RGB value. Components
-    should be values 0 to 255.
-    """
-    return ((r & 0xF8) << 8) | ((g & 0xFC) << 3) | (b >> 3)
-
-
-def image_to_data(image, rotation=0):
-    """Generator function to convert a PIL image to 16-bit 565 RGB bytes."""
-    # NumPy is much faster at doing this. NumPy code provided by:
-    # Keith (https://www.blogger.com/profile/02555547344016007163)
-    pb = np.rot90(np.array(image.convert('RGB')), rotation // 90).astype('uint16')
-    color = ((pb[:, :, 0] & 0xF8) << 8) | ((pb[:, :, 1] & 0xFC) << 3) | (pb[:, :, 2] >> 3)
-    return np.dstack(((color >> 8) & 0xFF, color & 0xFF)).flatten().tolist()
-
-
-class ST7735(object):
-    """Representation of an ST7735 TFT LCD."""
-
-    def __init__(self, port, cs, dc, backlight=None, rst=None, width=ST7735_TFTWIDTH,
-                 height=ST7735_TFTHEIGHT, rotation=90, offset_left=None, offset_top=None, invert=True, spi_speed_hz=4000000):
-        """Create an instance of the display using SPI communication.
-
-        Must provide the GPIO pin number for the D/C pin and the SPI driver.
-
-        Can optionally provide the GPIO pin number for the reset pin as the rst parameter.
-
-        :param port: SPI port number
-        :param cs: SPI chip-select number (0 or 1 for BCM
-        :param backlight: Pin for controlling backlight
-        :param rst: Reset pin for ST7735
-        :param width: Width of display connected to ST7735
-        :param height: Height of display connected to ST7735
-        :param rotation: Rotation of display connected to ST7735
-        :param offset_left: COL offset in ST7735 memory
-        :param offset_top: ROW offset in ST7735 memory
-        :param invert: Invert display
-        :param spi_speed_hz: SPI speed (in Hz)
-
-        """
-
-        GPIO.setwarnings(False)
-        GPIO.setmode(GPIO.BCM)
-
-        self._spi = spidev.SpiDev(port, cs)
-        self._spi.mode = 0
-        self._spi.lsbfirst = False
-        self._spi.max_speed_hz = spi_speed_hz
-
-        self._dc = dc
-        self._rst = rst
-        self._width = width
-        self._height = height
-        self._rotation = rotation
-        self._invert = invert
-
-        # Default left offset to center display
-        if offset_left is None:
-            offset_left = (ST7735_COLS - width) // 2
-
-        self._offset_left = offset_left
-
-        # Default top offset to center display
-        if offset_top is None:
-            offset_top = (ST7735_ROWS - height) // 2
-
-        self._offset_top = offset_top
-
-        # Set DC as output.
-        GPIO.setup(dc, GPIO.OUT)
-
-        # Setup backlight as output (if provided).
-        self._backlight = backlight
-        if backlight is not None:
-            GPIO.setup(backlight, GPIO.OUT)
-            GPIO.output(backlight, GPIO.LOW)
-            time.sleep(0.1)
-            GPIO.output(backlight, GPIO.HIGH)
-
-        # Setup reset as output (if provided).
-        if rst is not None:
-            GPIO.setup(rst, GPIO.OUT)
-
-        self.reset()
-        self._init()
-
-    def send(self, data, is_data=True, chunk_size=4096):
-        """Write a byte or array of bytes to the display. Is_data parameter
-        controls if byte should be interpreted as display data (True) or command
-        data (False).  Chunk_size is an optional size of bytes to write in a
-        single SPI transaction, with a default of 4096.
-        """
-        # Set DC low for command, high for data.
-        GPIO.output(self._dc, is_data)
-        # Convert scalar argument to list so either can be passed as parameter.
-        if isinstance(data, numbers.Number):
-            data = [data & 0xFF]
-        self._spi.xfer3(data)
-
-    def set_backlight(self, value):
-        """Set the backlight on/off."""
-        if self._backlight is not None:
-            GPIO.output(self._backlight, value)
-
-    @property
-    def width(self):
-        return self._width if self._rotation == 0 or self._rotation == 180 else self._height
-
-    @property
-    def height(self):
-        return self._height if self._rotation == 0 or self._rotation == 180 else self._width
-
-    def command(self, data):
-        """Write a byte or array of bytes to the display as command data."""
-        self.send(data, False)
-
-    def data(self, data):
-        """Write a byte or array of bytes to the display as display data."""
-        self.send(data, True)
-
-    def reset(self):
-        """Reset the display, if reset pin is connected."""
-        if self._rst is not None:
-            GPIO.output(self._rst, 1)
-            time.sleep(0.500)
-            GPIO.output(self._rst, 0)
-            time.sleep(0.500)
-            GPIO.output(self._rst, 1)
-            time.sleep(0.500)
-
-    def _init(self):
-        # Initialize the display.
-
-        self.command(ST7735_SWRESET)    # Software reset
-        time.sleep(0.150)               # delay 150 ms
-
-        self.command(ST7735_SLPOUT)     # Out of sleep mode
-        time.sleep(0.500)               # delay 500 ms
-
-        self.command(ST7735_FRMCTR1)    # Frame rate ctrl - normal mode
-        self.data(0x01)                 # Rate = fosc/(1x2+40) * (LINE+2C+2D)
-        self.data(0x2C)
-        self.data(0x2D)
-
-        self.command(ST7735_FRMCTR2)    # Frame rate ctrl - idle mode
-        self.data(0x01)                 # Rate = fosc/(1x2+40) * (LINE+2C+2D)
-        self.data(0x2C)
-        self.data(0x2D)
-
-        self.command(ST7735_FRMCTR3)    # Frame rate ctrl - partial mode
-        self.data(0x01)                 # Dot inversion mode
-        self.data(0x2C)
-        self.data(0x2D)
-        self.data(0x01)                 # Line inversion mode
-        self.data(0x2C)
-        self.data(0x2D)
-
-        self.command(ST7735_INVCTR)     # Display inversion ctrl
-        self.data(0x07)                 # No inversion
-
-        self.command(ST7735_PWCTR1)     # Power control
-        self.data(0xA2)
-        self.data(0x02)                 # -4.6V
-        self.data(0x84)                 # auto mode
-
-        self.command(ST7735_PWCTR2)     # Power control
-        self.data(0x0A)                 # Opamp current small
-        self.data(0x00)                 # Boost frequency
-
-        self.command(ST7735_PWCTR4)     # Power control
-        self.data(0x8A)                 # BCLK/2, Opamp current small & Medium low
-        self.data(0x2A)
-
-        self.command(ST7735_PWCTR5)     # Power control
-        self.data(0x8A)
-        self.data(0xEE)
-
-        self.command(ST7735_VMCTR1)     # Power control
-        self.data(0x0E)
-
-        if self._invert:
-            self.command(ST7735_INVON)   # Invert display
-        else:
-            self.command(ST7735_INVOFF)  # Don't invert display
-
-        self.command(ST7735_MADCTL)     # Memory access control (directions)
-        self.data(0xC8)                 # row addr/col addr, bottom to top refresh
-
-        self.command(ST7735_COLMOD)     # set color mode
-        self.data(0x05)                 # 16-bit color
-
-        self.command(ST7735_CASET)      # Column addr set
-        self.data(0x00)                 # XSTART = 0
-        self.data(self._offset_left)
-        self.data(0x00)                 # XEND = ROWS - height
-        self.data(self._width + self._offset_left - 1)
-
-        self.command(ST7735_RASET)      # Row addr set
-        self.data(0x00)                 # XSTART = 0
-        self.data(self._offset_top)
-        self.data(0x00)                 # XEND = COLS - width
-        self.data(self._height + self._offset_top - 1)
-
-        self.command(ST7735_GMCTRP1)    # Set Gamma
-        self.data(0x02)
-        self.data(0x1c)
-        self.data(0x07)
-        self.data(0x12)
-        self.data(0x37)
-        self.data(0x32)
-        self.data(0x29)
-        self.data(0x2d)
-        self.data(0x29)
-        self.data(0x25)
-        self.data(0x2B)
-        self.data(0x39)
-        self.data(0x00)
-        self.data(0x01)
-        self.data(0x03)
-        self.data(0x10)
-
-        self.command(ST7735_GMCTRN1)    # Set Gamma
-        self.data(0x03)
-        self.data(0x1d)
-        self.data(0x07)
-        self.data(0x06)
-        self.data(0x2E)
-        self.data(0x2C)
-        self.data(0x29)
-        self.data(0x2D)
-        self.data(0x2E)
-        self.data(0x2E)
-        self.data(0x37)
-        self.data(0x3F)
-        self.data(0x00)
-        self.data(0x00)
-        self.data(0x02)
-        self.data(0x10)
-
-        self.command(ST7735_NORON)      # Normal display on
-        time.sleep(0.10)                # 10 ms
-
-        self.command(ST7735_DISPON)     # Display on
-        time.sleep(0.100)               # 100 ms
-
-    def begin(self):
-        """Set up the display
-
-        Deprecated. Included in __init__.
-
-        """
-        pass
-
-    def set_window(self, x0=0, y0=0, x1=None, y1=None):
-        """Set the pixel address window for proceeding drawing commands. x0 and
-        x1 should define the minimum and maximum x pixel bounds.  y0 and y1
-        should define the minimum and maximum y pixel bound.  If no parameters
-        are specified the default will be to update the entire display from 0,0
-        to width-1,height-1.
-        """
-        if x1 is None:
-            x1 = self._width - 1
-
-        if y1 is None:
-            y1 = self._height - 1
-
-        y0 += self._offset_top
-        y1 += self._offset_top
-
-        x0 += self._offset_left
-        x1 += self._offset_left
-
-        self.command(ST7735_CASET)       # Column addr set
-        self.data(x0 >> 8)
-        self.data(x0)                    # XSTART
-        self.data(x1 >> 8)
-        self.data(x1)                    # XEND
-        self.command(ST7735_RASET)       # Row addr set
-        self.data(y0 >> 8)
-        self.data(y0)                    # YSTART
-        self.data(y1 >> 8)
-        self.data(y1)                    # YEND
-        self.command(ST7735_RAMWR)       # write to RAM
-
-    def display(self, image):
-        """Write the provided image to the hardware.
-
-        :param image: Should be RGB format and the same dimensions as the display hardware.
-
-        """
-        # Set address bounds to entire display.
-        self.set_window()
-        # Convert image to array of 16bit 565 RGB data bytes.
-        # Unfortunate that this copy has to occur, but the SPI byte writing
-        # function needs to take an array of bytes and PIL doesn't natively
-        # store images in 16-bit 565 RGB format.
-        pixelbytes = list(image_to_data(image, self._rotation))
-        # Write data to hardware.
-        self.data(pixelbytes)
+# Copyright (c) 2014 Adafruit Industries
+# Author: Tony DiCola
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+# THE SOFTWARE.
+import numbers
+import time
+import numpy as np
+
+import spidev
+import RPi.GPIO as GPIO
+
+
+__version__ = '0.0.5'
+
+BG_SPI_CS_BACK = 0
+BG_SPI_CS_FRONT = 1
+
+SPI_CLOCK_HZ = 16000000
+
+# Constants for interacting with display registers.
+ST7735_TFTWIDTH = 80
+ST7735_TFTHEIGHT = 160
+
+ST7735_COLS = 132
+ST7735_ROWS = 162
+
+ST7735_NOP = 0x00
+ST7735_SWRESET = 0x01
+ST7735_RDDID = 0x04
+ST7735_RDDST = 0x09
+
+ST7735_SLPIN = 0x10
+ST7735_SLPOUT = 0x11
+ST7735_PTLON = 0x12
+ST7735_NORON = 0x13
+
+ST7735_INVOFF = 0x20
+ST7735_INVON = 0x21
+ST7735_DISPOFF = 0x28
+ST7735_DISPON = 0x29
+
+ST7735_CASET = 0x2A
+ST7735_RASET = 0x2B
+ST7735_RAMWR = 0x2C
+ST7735_RAMRD = 0x2E
+
+ST7735_PTLAR = 0x30
+ST7735_MADCTL = 0x36
+ST7735_COLMOD = 0x3A
+
+ST7735_FRMCTR1 = 0xB1
+ST7735_FRMCTR2 = 0xB2
+ST7735_FRMCTR3 = 0xB3
+ST7735_INVCTR = 0xB4
+ST7735_DISSET5 = 0xB6
+
+
+ST7735_PWCTR1 = 0xC0
+ST7735_PWCTR2 = 0xC1
+ST7735_PWCTR3 = 0xC2
+ST7735_PWCTR4 = 0xC3
+ST7735_PWCTR5 = 0xC4
+ST7735_VMCTR1 = 0xC5
+
+ST7735_RDID1 = 0xDA
+ST7735_RDID2 = 0xDB
+ST7735_RDID3 = 0xDC
+ST7735_RDID4 = 0xDD
+
+ST7735_GMCTRP1 = 0xE0
+ST7735_GMCTRN1 = 0xE1
+
+ST7735_PWCTR6 = 0xFC
+
+# Colours for convenience
+ST7735_BLACK = 0x0000  # 0b 00000 000000 00000
+ST7735_BLUE = 0x001F  # 0b 00000 000000 11111
+ST7735_GREEN = 0x07E0  # 0b 00000 111111 00000
+ST7735_RED = 0xF800  # 0b 11111 000000 00000
+ST7735_CYAN = 0x07FF  # 0b 00000 111111 11111
+ST7735_MAGENTA = 0xF81F  # 0b 11111 000000 11111
+ST7735_YELLOW = 0xFFE0  # 0b 11111 111111 00000
+ST7735_WHITE = 0xFFFF  # 0b 11111 111111 11111
+
+
+def color565(r, g, b):
+    """Convert red, green, blue components to a 16-bit 565 RGB value. Components
+    should be values 0 to 255.
+    """
+    return ((r & 0xF8) << 8) | ((g & 0xFC) << 3) | (b >> 3)
+
+
+def image_to_data(image, rotation=0):
+    """Generator function to convert a PIL image to 16-bit 565 RGB bytes."""
+    # NumPy is much faster at doing this. NumPy code provided by:
+    # Keith (https://www.blogger.com/profile/02555547344016007163)
+    pb = np.rot90(np.array(image.convert('RGB')), rotation // 90).astype('uint16')
+    color = ((pb[:, :, 0] & 0xF8) << 8) | ((pb[:, :, 1] & 0xFC) << 3) | (pb[:, :, 2] >> 3)
+    return np.dstack(((color >> 8) & 0xFF, color & 0xFF)).flatten().tolist()
+
+
+class ST7735(object):
+    """Representation of an ST7735 TFT LCD."""
+
+    def __init__(self, port, cs, dc, backlight=None, rst=None, width=ST7735_TFTWIDTH,
+                 height=ST7735_TFTHEIGHT, rotation=90, offset_left=None, offset_top=None, invert=True, bgr=True, spi_speed_hz=4000000):
+        """Create an instance of the display using SPI communication.
+
+        Must provide the GPIO pin number for the D/C pin and the SPI driver.
+
+        Can optionally provide the GPIO pin number for the reset pin as the rst parameter.
+
+        :param port: SPI port number
+        :param cs: SPI chip-select number (0 or 1 for BCM
+        :param backlight: Pin for controlling backlight
+        :param rst: Reset pin for ST7735
+        :param width: Width of display connected to ST7735
+        :param height: Height of display connected to ST7735
+        :param rotation: Rotation of display connected to ST7735
+        :param offset_left: COL offset in ST7735 memory
+        :param offset_top: ROW offset in ST7735 memory
+        :param invert: Invert display
+        :param spi_speed_hz: SPI speed (in Hz)
+
+        """
+
+        GPIO.setwarnings(False)
+        GPIO.setmode(GPIO.BCM)
+
+        self._spi = spidev.SpiDev(port, cs)
+        self._spi.mode = 0
+        self._spi.lsbfirst = False
+        self._spi.max_speed_hz = spi_speed_hz
+
+        self._dc = dc
+        self._rst = rst
+        self._width = width
+        self._height = height
+        self._rotation = rotation
+        self._invert = invert
+        self._bgr = bgr
+
+        # Default left offset to center display
+        if offset_left is None:
+            offset_left = (ST7735_COLS - width) // 2
+
+        self._offset_left = offset_left
+
+        # Default top offset to center display
+        if offset_top is None:
+            offset_top = (ST7735_ROWS - height) // 2
+
+        self._offset_top = offset_top
+
+        # Set DC as output.
+        GPIO.setup(dc, GPIO.OUT)
+
+        # Setup backlight as output (if provided).
+        self._backlight = backlight
+        if backlight is not None:
+            GPIO.setup(backlight, GPIO.OUT)
+            GPIO.output(backlight, GPIO.LOW)
+            time.sleep(0.1)
+            GPIO.output(backlight, GPIO.HIGH)
+
+        # Setup reset as output (if provided).
+        if rst is not None:
+            GPIO.setup(rst, GPIO.OUT)
+
+        self.reset()
+        self._init()
+
+    def send(self, data, is_data=True, chunk_size=4096):
+        """Write a byte or array of bytes to the display. Is_data parameter
+        controls if byte should be interpreted as display data (True) or command
+        data (False).  Chunk_size is an optional size of bytes to write in a
+        single SPI transaction, with a default of 4096.
+        """
+        # Set DC low for command, high for data.
+        GPIO.output(self._dc, is_data)
+        # Convert scalar argument to list so either can be passed as parameter.
+        if isinstance(data, numbers.Number):
+            data = [data & 0xFF]
+        self._spi.xfer3(data)
+
+    def set_backlight(self, value):
+        """Set the backlight on/off."""
+        if self._backlight is not None:
+            GPIO.output(self._backlight, value)
+
+    def display_off(self):
+        self.command(ST7735_DISPOFF)
+
+    def display_on(self):
+        self.command(ST7735_DISPON)
+
+    def sleep(self):
+        self.command(ST7735_SLPIN)
+
+    def wake(self):
+        self.command(ST7735_SLPOUT)
+
+    @property
+    def width(self):
+        return self._width if self._rotation == 0 or self._rotation == 180 else self._height
+
+    @property
+    def height(self):
+        return self._height if self._rotation == 0 or self._rotation == 180 else self._width
+
+    def command(self, data):
+        """Write a byte or array of bytes to the display as command data."""
+        self.send(data, False)
+
+    def data(self, data):
+        """Write a byte or array of bytes to the display as display data."""
+        self.send(data, True)
+
+    def reset(self):
+        """Reset the display, if reset pin is connected."""
+        if self._rst is not None:
+            GPIO.output(self._rst, 1)
+            time.sleep(0.500)
+            GPIO.output(self._rst, 0)
+            time.sleep(0.500)
+            GPIO.output(self._rst, 1)
+            time.sleep(0.500)
+
+    def _init(self):
+        # Initialize the display.
+
+        self.command(ST7735_SWRESET)    # Software reset
+        time.sleep(0.150)               # delay 150 ms
+
+        self.command(ST7735_SLPOUT)     # Out of sleep mode
+        time.sleep(0.500)               # delay 500 ms
+
+        self.command(ST7735_FRMCTR1)    # Frame rate ctrl - normal mode
+        self.data(0x01)                 # Rate = fosc/(1x2+40) * (LINE+2C+2D)
+        self.data(0x2C)
+        self.data(0x2D)
+
+        self.command(ST7735_FRMCTR2)    # Frame rate ctrl - idle mode
+        self.data(0x01)                 # Rate = fosc/(1x2+40) * (LINE+2C+2D)
+        self.data(0x2C)
+        self.data(0x2D)
+
+        self.command(ST7735_FRMCTR3)    # Frame rate ctrl - partial mode
+        self.data(0x01)                 # Dot inversion mode
+        self.data(0x2C)
+        self.data(0x2D)
+        self.data(0x01)                 # Line inversion mode
+        self.data(0x2C)
+        self.data(0x2D)
+
+        self.command(ST7735_INVCTR)     # Display inversion ctrl
+        self.data(0x07)                 # No inversion
+
+        self.command(ST7735_PWCTR1)     # Power control
+        self.data(0xA2)
+        self.data(0x02)                 # -4.6V
+        self.data(0x84)                 # auto mode
+
+        self.command(ST7735_PWCTR2)     # Power control
+        self.data(0x0A)                 # Opamp current small
+        self.data(0x00)                 # Boost frequency
+
+        self.command(ST7735_PWCTR4)     # Power control
+        self.data(0x8A)                 # BCLK/2, Opamp current small & Medium low
+        self.data(0x2A)
+
+        self.command(ST7735_PWCTR5)     # Power control
+        self.data(0x8A)
+        self.data(0xEE)
+
+        self.command(ST7735_VMCTR1)     # Power control
+        self.data(0x0E)
+
+        if self._invert:
+            self.command(ST7735_INVON)   # Invert display
+        else:
+            self.command(ST7735_INVOFF)  # Don't invert display
+
+        self.command(ST7735_MADCTL)     # Memory access control (directions)
+        if self._bgr:
+            self.data(0xC8)             # row addr/col addr, bottom to top refresh; Set D3 RGB Bit to 1 for format BGR
+        else:
+            self.data(0xC0)             # row addr/col addr, bottom to top refresh; Set D3 RGB Bit to 0 for format RGB
+
+        self.command(ST7735_COLMOD)     # set color mode
+        self.data(0x05)                 # 16-bit color
+
+        self.command(ST7735_CASET)      # Column addr set
+        self.data(0x00)                 # XSTART = 0
+        self.data(self._offset_left)
+        self.data(0x00)                 # XEND = ROWS - height
+        self.data(self._width + self._offset_left - 1)
+
+        self.command(ST7735_RASET)      # Row addr set
+        self.data(0x00)                 # XSTART = 0
+        self.data(self._offset_top)
+        self.data(0x00)                 # XEND = COLS - width
+        self.data(self._height + self._offset_top - 1)
+
+        self.command(ST7735_GMCTRP1)    # Set Gamma
+        self.data(0x02)
+        self.data(0x1c)
+        self.data(0x07)
+        self.data(0x12)
+        self.data(0x37)
+        self.data(0x32)
+        self.data(0x29)
+        self.data(0x2d)
+        self.data(0x29)
+        self.data(0x25)
+        self.data(0x2B)
+        self.data(0x39)
+        self.data(0x00)
+        self.data(0x01)
+        self.data(0x03)
+        self.data(0x10)
+
+        self.command(ST7735_GMCTRN1)    # Set Gamma
+        self.data(0x03)
+        self.data(0x1d)
+        self.data(0x07)
+        self.data(0x06)
+        self.data(0x2E)
+        self.data(0x2C)
+        self.data(0x29)
+        self.data(0x2D)
+        self.data(0x2E)
+        self.data(0x2E)
+        self.data(0x37)
+        self.data(0x3F)
+        self.data(0x00)
+        self.data(0x00)
+        self.data(0x02)
+        self.data(0x10)
+
+        self.command(ST7735_NORON)      # Normal display on
+        time.sleep(0.10)                # 10 ms
+
+        self.display_on()
+        time.sleep(0.100)               # 100 ms
+
+    def begin(self):
+        """Set up the display
+
+        Deprecated. Included in __init__.
+
+        """
+        pass
+
+    def set_window(self, x0=0, y0=0, x1=None, y1=None):
+        """Set the pixel address window for proceeding drawing commands. x0 and
+        x1 should define the minimum and maximum x pixel bounds.  y0 and y1
+        should define the minimum and maximum y pixel bound.  If no parameters
+        are specified the default will be to update the entire display from 0,0
+        to width-1,height-1.
+        """
+        if x1 is None:
+            x1 = self._width - 1
+
+        if y1 is None:
+            y1 = self._height - 1
+
+        y0 += self._offset_top
+        y1 += self._offset_top
+
+        x0 += self._offset_left
+        x1 += self._offset_left
+
+        self.command(ST7735_CASET)       # Column addr set
+        self.data(x0 >> 8)
+        self.data(x0)                    # XSTART
+        self.data(x1 >> 8)
+        self.data(x1)                    # XEND
+        self.command(ST7735_RASET)       # Row addr set
+        self.data(y0 >> 8)
+        self.data(y0)                    # YSTART
+        self.data(y1 >> 8)
+        self.data(y1)                    # YEND
+        self.command(ST7735_RAMWR)       # write to RAM
+
+    def display(self, image):
+        """Write the provided image to the hardware.
+
+        :param image: Should be RGB format and the same dimensions as the display hardware.
+
+        """
+        # Set address bounds to entire display.
+        self.set_window()
+        # Convert image to array of 16bit 565 RGB data bytes.
+        # Unfortunate that this copy has to occur, but the SPI byte writing
+        # function needs to take an array of bytes and PIL doesn't natively
+        # store images in 16-bit 565 RGB format.
+        pixelbytes = list(image_to_data(image, self._rotation))
+        # Write data to hardware.
+        self.data(pixelbytes)
```

### Comparing `ST7735-0.0.4.post1/ST7735.egg-info/PKG-INFO` & `ST7735-0.0.5/ST7735.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ST7735
-Version: 0.0.4.post1
+Version: 0.0.5
 Summary: Library to control an ST7735 168x80 TFT LCD display.
 Home-page: https://www.pimoroni.com
 Author: Philip Howard
 Author-email: phil@pimoroni.com
 License: MIT
 Project-URL: GitHub, https://www.github.com/pimoroni/st7735-python
 Description: # Python ST7735
@@ -72,14 +72,20 @@
         Adafruit invests time and resources providing this open source code, please support Adafruit and open-source hardware by purchasing products from Adafruit!
         
         Modified from 'Modified from 'Adafruit Python ILI9341' written by Tony DiCola for Adafruit Industries.' written by Clement Skau.
         
         MIT license, all text above must be included in any redistribution
         
         # Changelog
+        0.0.5
+        -----
+        
+        * Add support for choosing between BGR/RGB displays
+        * Add methods for display power and sleep control
+        
         0.0.4-post1
         -----------
         
         * Repackage with Markdown README/setup.cfg
         * Fix `__version__` to 0.0.4
         * Update dependencies in README
```

