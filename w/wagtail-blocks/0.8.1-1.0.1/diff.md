# Comparing `tmp/wagtail_blocks-0.8.1.tar.gz` & `tmp/wagtail_blocks-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_blocks-0.8.1.tar", last modified: Sat Jul 16 20:10:11 2022, max compression
+gzip compressed data, was "wagtail_blocks-1.0.1.tar", last modified: Mon Aug  7 14:04:56 2023, max compression
```

## Comparing `wagtail_blocks-0.8.1.tar` & `wagtail_blocks-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.197475 wagtail_blocks-0.8.1/
--rw-r--r--   0 ibrahim    (501) staff       (20)     1069 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/LICENSE
--rw-r--r--   0 ibrahim    (501) staff       (20)      106 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/MANIFEST.in
--rw-r--r--   0 ibrahim    (501) staff       (20)     4457 2022-07-16 20:10:11.197551 wagtail_blocks-0.8.1/PKG-INFO
--rw-r--r--   0 ibrahim    (501) staff       (20)     3195 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/README.md
--rw-r--r--   0 ibrahim    (501) staff       (20)       41 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/requirements.txt
--rw-r--r--   0 ibrahim    (501) staff       (20)       79 2022-07-16 20:10:11.197781 wagtail_blocks-0.8.1/setup.cfg
--rw-r--r--   0 ibrahim    (501) staff       (20)     2000 2022-07-16 20:06:25.000000 wagtail_blocks-0.8.1/setup.py
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.190700 wagtail_blocks-0.8.1/wagtail_blocks/
--rw-r--r--   0 ibrahim    (501) staff       (20)       22 2022-07-16 20:09:46.000000 wagtail_blocks-0.8.1/wagtail_blocks/__init__.py
--rw-r--r--   0 ibrahim    (501) staff       (20)     5463 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/blocks.py
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.189138 wagtail_blocks-0.8.1/wagtail_blocks/static/
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.193611 wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/
--rw-r--r--   0 ibrahim    (501) staff       (20)   155758 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/bootstrap.min.css
--rw-r--r--   0 ibrahim    (501) staff       (20)     1591 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/cropped_images_with_text.css
--rw-r--r--   0 ibrahim    (501) staff       (20)     1912 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/image_slider.css
--rw-r--r--   0 ibrahim    (501) staff       (20)      576 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/image_text_overlay.css
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.194669 wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/js/
--rw-r--r--   0 ibrahim    (501) staff       (20)   210419 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/js/Chart.bundle.min.js
--rw-r--r--   0 ibrahim    (501) staff       (20)    78635 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/js/bootstrap.bundle.min.js
--rw-r--r--   0 ibrahim    (501) staff       (20)      761 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/list_with_images.css
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.189286 wagtail_blocks-0.8.1/wagtail_blocks/templates/
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.196900 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.197071 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/admin_blocks/
--rw-r--r--   0 ibrahim    (501) staff       (20)     2444 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/admin_blocks/map.html
--rw-r--r--   0 ibrahim    (501) staff       (20)     2963 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/chart.html
--rw-r--r--   0 ibrahim    (501) staff       (20)      756 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/cropped_images_with_text.html
--rw-r--r--   0 ibrahim    (501) staff       (20)       92 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/header.html
--rw-r--r--   0 ibrahim    (501) staff       (20)      984 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/image_slider.html
--rw-r--r--   0 ibrahim    (501) staff       (20)      648 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/image_text_overlay.html
--rw-r--r--   0 ibrahim    (501) staff       (20)      129 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/list.html
--rw-r--r--   0 ibrahim    (501) staff       (20)     1382 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/list_with_images.html
--rw-r--r--   0 ibrahim    (501) staff       (20)     1878 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/map.html
--rw-r--r--   0 ibrahim    (501) staff       (20)      563 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/thumbnail_gallery.html
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.197335 wagtail_blocks-0.8.1/wagtail_blocks/templatetags/
--rw-r--r--   0 ibrahim    (501) staff       (20)        0 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templatetags/__init__.py
--rw-r--r--   0 ibrahim    (501) staff       (20)      515 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/templatetags/wagtail_html_support.py
--rw-r--r--   0 ibrahim    (501) staff       (20)       56 2022-07-16 19:57:09.000000 wagtail_blocks-0.8.1/wagtail_blocks/test_dummy.py
-drwxr-xr-x   0 ibrahim    (501) staff       (20)        0 2022-07-16 20:10:11.191599 wagtail_blocks-0.8.1/wagtail_blocks.egg-info/
--rw-r--r--   0 ibrahim    (501) staff       (20)     4457 2022-07-16 20:10:10.000000 wagtail_blocks-0.8.1/wagtail_blocks.egg-info/PKG-INFO
--rw-r--r--   0 ibrahim    (501) staff       (20)     1425 2022-07-16 20:10:11.000000 wagtail_blocks-0.8.1/wagtail_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahim    (501) staff       (20)        1 2022-07-16 20:10:10.000000 wagtail_blocks-0.8.1/wagtail_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahim    (501) staff       (20)       59 2022-07-16 20:10:11.000000 wagtail_blocks-0.8.1/wagtail_blocks.egg-info/requires.txt
--rw-r--r--   0 ibrahim    (501) staff       (20)       15 2022-07-16 20:10:11.000000 wagtail_blocks-0.8.1/wagtail_blocks.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.527554 wagtail_blocks-1.0.1/
+-rw-rw-rw-   0        0        0     1069 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      106 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4303 2023-08-07 14:04:56.527554 wagtail_blocks-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2850 2023-08-07 13:51:36.000000 wagtail_blocks-1.0.1/README.md
+-rw-rw-rw-   0        0        0       38 2023-08-07 13:43:49.000000 wagtail_blocks-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-08-07 14:04:56.529546 wagtail_blocks-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2067 2023-08-07 13:43:49.000000 wagtail_blocks-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.477034 wagtail_blocks-1.0.1/wagtail_blocks/
+-rw-rw-rw-   0        0        0       22 2023-08-07 14:04:46.000000 wagtail_blocks-1.0.1/wagtail_blocks/__init__.py
+-rw-rw-rw-   0        0        0     5320 2023-08-07 13:43:49.000000 wagtail_blocks-1.0.1/wagtail_blocks/blocks.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.458035 wagtail_blocks-1.0.1/wagtail_blocks/static/
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.505037 wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/
+-rw-rw-rw-   0        0        0   155758 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1591 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/cropped_images_with_text.css
+-rw-rw-rw-   0        0        0     1912 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/image_slider.css
+-rw-rw-rw-   0        0        0      576 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/image_text_overlay.css
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.508035 wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/js/
+-rw-rw-rw-   0        0        0   210419 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/js/Chart.bundle.min.js
+-rw-rw-rw-   0        0        0    78635 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0      761 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/list_with_images.css
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.459035 wagtail_blocks-1.0.1/wagtail_blocks/templates/
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.523542 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.524547 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/admin_blocks/
+-rw-rw-rw-   0        0        0     2444 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/admin_blocks/map.html
+-rw-rw-rw-   0        0        0     2963 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/chart.html
+-rw-rw-rw-   0        0        0      756 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/cropped_images_with_text.html
+-rw-rw-rw-   0        0        0       92 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/header.html
+-rw-rw-rw-   0        0        0      984 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/image_slider.html
+-rw-rw-rw-   0        0        0      648 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/image_text_overlay.html
+-rw-rw-rw-   0        0        0      129 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/list.html
+-rw-rw-rw-   0        0        0     1382 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/list_with_images.html
+-rw-rw-rw-   0        0        0     1878 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/map.html
+-rw-rw-rw-   0        0        0      563 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/thumbnail_gallery.html
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.526554 wagtail_blocks-1.0.1/wagtail_blocks/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      515 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/templatetags/wagtail_html_support.py
+-rw-rw-rw-   0        0        0       56 2023-08-07 13:38:43.000000 wagtail_blocks-1.0.1/wagtail_blocks/test_dummy.py
+-rw-rw-rw-   0        0        0      390 2023-08-07 13:43:49.000000 wagtail_blocks-1.0.1/wagtail_blocks/wagtail_hooks.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:56.496034 wagtail_blocks-1.0.1/wagtail_blocks.egg-info/
+-rw-rw-rw-   0        0        0     4303 2023-08-07 14:04:56.000000 wagtail_blocks-1.0.1/wagtail_blocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1457 2023-08-07 14:04:56.000000 wagtail_blocks-1.0.1/wagtail_blocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 14:04:56.000000 wagtail_blocks-1.0.1/wagtail_blocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-08-07 14:04:56.000000 wagtail_blocks-1.0.1/wagtail_blocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-07 14:04:56.000000 wagtail_blocks-1.0.1/wagtail_blocks.egg-info/top_level.txt
```

### Comparing `wagtail_blocks-0.8.1/LICENSE` & `wagtail_blocks-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/PKG-INFO` & `wagtail_blocks-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,124 @@
-Metadata-Version: 2.1
-Name: wagtail_blocks
-Version: 0.8.1
-Summary: A Collection of awesome Wagtail CMS stream-field blocks and Charts
-Home-page: https://github.com/ibrahimawadhamid/wagtail_blocks/
-Author: IbrahimAwadHamid
-Author-email: ibrahim.a.hamid@gmail.com
-License: MIT
-Keywords: WAGTAIL,STREAMFIELD,WAGTAIL_BLOCKS,WAGTAIL CMS
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: docs
-License-File: LICENSE
-
-# wagtail_blocks ![wagtail](https://img.shields.io/badge/CMS-Wagtail-green.svg)
-[![PyPI](https://img.shields.io/pypi/v/wagtail-blocks.svg)](https://pypi.python.org/pypi/wagtail-blocks) ![Build](https://img.shields.io/pypi/status/wagtail-blocks.svg) [![Documentation Status](https://readthedocs.org/projects/wagtail-blocks/badge/?version=latest)](https://wagtail-blocks.readthedocs.io/en/latest/?badge=latest) ![PyPI - License](https://img.shields.io/pypi/l/wagtail-blocks.svg)
-
-![Downloads](https://static.pepy.tech/badge/wagtail-blocks) ![Downloads Month](https://static.pepy.tech/badge/wagtail-blocks/month) ![Downloads Week](https://static.pepy.tech/badge/wagtail-blocks/week)
-
-A Collection of awesome Wagtail CMS stream-field blocks and Charts.
-
-*Check out [Awesome Wagtail](https://github.com/springload/awesome-wagtail) for more awesome packages and resources from the Wagtail community.*
-
-## Note
-**This project is still early on in its development lifecycle. It is possible for breaking changes to occur between versions until reaching a stable 1.0**, however we will clearly note any breaking changes between releases if applicable. Feedback and pull requests are welcome.
-
-## Quickstart
-
-You must have your [Wagtail](https://wagtail.io/) project up and running:
-
-```sh
-pip install wagtail_blocks
-```
-Add the following enteries to your `settings.py` in the INSTALLED_APPS section:
-
-```python
-'wagtailfontawesome',
-'wagtail_blocks',
-```
-
-## Sample Usage
-```python
-from wagtail_blocks.blocks import HeaderBlock, ListBlock, ImageTextOverlayBlock, CroppedImagesWithTextBlock, \
-    ListWithImagesBlock, ThumbnailGalleryBlock, ChartBlock, MapBlock, ImageSliderBlock
-
-class HomePage(Page):
-    body = StreamField([
-        ('header', HeaderBlock()),
-        ('list', ListBlock()),
-        ('image_text_overlay', ImageTextOverlayBlock()),
-        ('cropped_images_with_text', CroppedImagesWithTextBlock()),
-        ('list_with_images', ListWithImagesBlock()),
-        ('thumbnail_gallery', ThumbnailGalleryBlock()),
-        ('chart', ChartBlock()),
-        ('map', MapBlock()),
-        ('image_slider', ImageSliderBlock()),
-    ], blank=True)
-
-    content_panels = Page.content_panels + [
-        StreamFieldPanel("body", classname="Full"),
-    ]
-
-```
-### For HomePage template, blocks should be rendered with IDs to function properly
-```
-{% for block in page.body %}
-    {% include_block block with block_id=block.id %}
-{% endfor %}
-```
-
-## Available Blocks
-Check Showcase for [Standard Blocks](https://wagtail-blocks.readthedocs.io/en/latest/showcase/standard-blocks/) 
-or [Charts](https://wagtail-blocks.readthedocs.io/en/latest/showcase/chart/)
-or [Maps](https://wagtail-blocks.readthedocs.io/en/latest/showcase/map/)
-![streamfield](https://wagtail-blocks.readthedocs.io/en/latest/showcase/screenshots/streamfield.PNG)
- 
-> - Header (H1, H2, H3, H4, H5, H6)
-> - List (Unordered List)
-> - Image with Text Overlay
-> - Cropped Images with Text
-> - List with Images and Links
-> - Thumbnail Gallery
-> - Image Slider
-> - Chart (Bar - Pie - Line - Area - Radar)
-> - Map (Marker with rich text description)
-
-## Supported Versions
-> - Python 3.6 and higher
-> - Wagtail 2 and higher
-> - Bootstrap 4
-
+Metadata-Version: 2.1
+Name: wagtail_blocks
+Version: 1.0.1
+Summary: A Collection of awesome Wagtail CMS stream-field blocks and Charts
+Home-page: https://github.com/ibrahimawadhamid/wagtail_blocks/
+Author: IbrahimAwadHamid
+Author-email: ibrahim.a.hamid@gmail.com
+License: MIT
+Keywords: WAGTAIL,STREAMFIELD,WAGTAIL_BLOCKS,WAGTAIL CMS
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: docs
+License-File: LICENSE
+
+# wagtail_blocks ![wagtail](https://img.shields.io/badge/CMS-Wagtail-green.svg)
+
+[![PyPI](https://img.shields.io/pypi/v/wagtail-blocks.svg)](https://pypi.python.org/pypi/wagtail-blocks) ![Build](https://img.shields.io/pypi/status/wagtail-blocks.svg) [![Documentation Status](https://readthedocs.org/projects/wagtail-blocks/badge/?version=latest)](https://wagtail-blocks.readthedocs.io/en/latest/?badge=latest) ![PyPI - License](https://img.shields.io/pypi/l/wagtail-blocks.svg)
+
+![Downloads](https://static.pepy.tech/badge/wagtail-blocks) ![Downloads Month](https://static.pepy.tech/badge/wagtail-blocks/month) ![Downloads Week](https://static.pepy.tech/badge/wagtail-blocks/week)
+
+A Collection of awesome Wagtail CMS stream-field blocks and Charts.
+
+*Check out [Awesome Wagtail](https://github.com/springload/awesome-wagtail) for more awesome packages and resources from the Wagtail community.*
+
+## Quickstart
+
+You must have your [Wagtail](https://wagtail.io/) project up and running:
+
+```sh
+pip install wagtail_blocks
+```
+
+Add the following enteries to your `settings.py` in the INSTALLED_APPS section:
+
+```python
+'wagtailfontawesomesvg',
+'wagtail_blocks',
+```
+
+## Sample Usage
+
+```python
+from wagtail.fields import StreamField
+from wagtail.admin.panels import FieldPanel
+
+from wagtail_blocks.blocks import (
+    HeaderBlock,
+    ListBlock,
+    ImageTextOverlayBlock,
+    CroppedImagesWithTextBlock,
+    ListWithImagesBlock,
+    ThumbnailGalleryBlock,
+    ChartBlock,
+    MapBlock,
+    ImageSliderBlock,
+)
+
+class HomePage(Page):
+    body = StreamField([
+        ('header', HeaderBlock()),
+        ('list', ListBlock()),
+        ('image_text_overlay', ImageTextOverlayBlock()),
+        ('cropped_images_with_text', CroppedImagesWithTextBlock()),
+        ('list_with_images', ListWithImagesBlock()),
+        ('thumbnail_gallery', ThumbnailGalleryBlock()),
+        ('chart', ChartBlock()),
+        ('map', MapBlock()),
+        ('image_slider', ImageSliderBlock()),
+    ], blank=True, use_json_field=True)
+
+    content_panels = Page.content_panels + [
+        FieldPanel("body"),
+    ]
+```
+
+### For HomePage template, blocks should be rendered with IDs to function properly
+
+```html
+{% for block in page.body %}
+    {% include_block block with block_id=block.id %}
+{% endfor %}
+```
+
+## Available Blocks
+
+Check Showcase for [Standard Blocks](docs/showcase/standard-blocks.md) or [Charts](docs/showcase/chart.md) or [Maps](docs/showcase/map.md)
+
+![streamfield](docs/showcase/screenshots/streamfield-v5.PNG)
+
+- Header (H1, H2, H3, H4, H5, H6)
+- List (Unordered List)
+- Image with Text Overlay
+- Cropped Images with Text
+- List with Images and Links
+- Thumbnail Gallery
+- Image Slider
+- Chart (Bar - Pie - Line - Area - Radar)
+- Map (Marker with rich text description)
+
+## Supported Versions
+
+- Python 3.8 and higher
+- Wagtail 4.1 and higher
+- Bootstrap 4
```

### Comparing `wagtail_blocks-0.8.1/README.md` & `wagtail_blocks-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,90 @@
 # wagtail_blocks ![wagtail](https://img.shields.io/badge/CMS-Wagtail-green.svg)
+
 [![PyPI](https://img.shields.io/pypi/v/wagtail-blocks.svg)](https://pypi.python.org/pypi/wagtail-blocks) ![Build](https://img.shields.io/pypi/status/wagtail-blocks.svg) [![Documentation Status](https://readthedocs.org/projects/wagtail-blocks/badge/?version=latest)](https://wagtail-blocks.readthedocs.io/en/latest/?badge=latest) ![PyPI - License](https://img.shields.io/pypi/l/wagtail-blocks.svg)
 
 ![Downloads](https://static.pepy.tech/badge/wagtail-blocks) ![Downloads Month](https://static.pepy.tech/badge/wagtail-blocks/month) ![Downloads Week](https://static.pepy.tech/badge/wagtail-blocks/week)
 
 A Collection of awesome Wagtail CMS stream-field blocks and Charts.
 
 *Check out [Awesome Wagtail](https://github.com/springload/awesome-wagtail) for more awesome packages and resources from the Wagtail community.*
 
-## Note
-**This project is still early on in its development lifecycle. It is possible for breaking changes to occur between versions until reaching a stable 1.0**, however we will clearly note any breaking changes between releases if applicable. Feedback and pull requests are welcome.
-
 ## Quickstart
 
 You must have your [Wagtail](https://wagtail.io/) project up and running:
 
 ```sh
 pip install wagtail_blocks
 ```
+
 Add the following enteries to your `settings.py` in the INSTALLED_APPS section:
 
 ```python
-'wagtailfontawesome',
+'wagtailfontawesomesvg',
 'wagtail_blocks',
 ```
 
 ## Sample Usage
+
 ```python
-from wagtail_blocks.blocks import HeaderBlock, ListBlock, ImageTextOverlayBlock, CroppedImagesWithTextBlock, \
-    ListWithImagesBlock, ThumbnailGalleryBlock, ChartBlock, MapBlock, ImageSliderBlock
+from wagtail.fields import StreamField
+from wagtail.admin.panels import FieldPanel
+
+from wagtail_blocks.blocks import (
+    HeaderBlock,
+    ListBlock,
+    ImageTextOverlayBlock,
+    CroppedImagesWithTextBlock,
+    ListWithImagesBlock,
+    ThumbnailGalleryBlock,
+    ChartBlock,
+    MapBlock,
+    ImageSliderBlock,
+)
 
 class HomePage(Page):
     body = StreamField([
         ('header', HeaderBlock()),
         ('list', ListBlock()),
         ('image_text_overlay', ImageTextOverlayBlock()),
         ('cropped_images_with_text', CroppedImagesWithTextBlock()),
         ('list_with_images', ListWithImagesBlock()),
         ('thumbnail_gallery', ThumbnailGalleryBlock()),
         ('chart', ChartBlock()),
         ('map', MapBlock()),
         ('image_slider', ImageSliderBlock()),
-    ], blank=True)
+    ], blank=True, use_json_field=True)
 
     content_panels = Page.content_panels + [
-        StreamFieldPanel("body", classname="Full"),
+        FieldPanel("body"),
     ]
-
 ```
+
 ### For HomePage template, blocks should be rendered with IDs to function properly
-```
+
+```html
 {% for block in page.body %}
     {% include_block block with block_id=block.id %}
 {% endfor %}
 ```
 
 ## Available Blocks
-Check Showcase for [Standard Blocks](https://wagtail-blocks.readthedocs.io/en/latest/showcase/standard-blocks/) 
-or [Charts](https://wagtail-blocks.readthedocs.io/en/latest/showcase/chart/)
-or [Maps](https://wagtail-blocks.readthedocs.io/en/latest/showcase/map/)
-![streamfield](https://wagtail-blocks.readthedocs.io/en/latest/showcase/screenshots/streamfield.PNG)
- 
-> - Header (H1, H2, H3, H4, H5, H6)
-> - List (Unordered List)
-> - Image with Text Overlay
-> - Cropped Images with Text
-> - List with Images and Links
-> - Thumbnail Gallery
-> - Image Slider
-> - Chart (Bar - Pie - Line - Area - Radar)
-> - Map (Marker with rich text description)
+
+Check Showcase for [Standard Blocks](docs/showcase/standard-blocks.md) or [Charts](docs/showcase/chart.md) or [Maps](docs/showcase/map.md)
+
+![streamfield](docs/showcase/screenshots/streamfield-v5.PNG)
+
+- Header (H1, H2, H3, H4, H5, H6)
+- List (Unordered List)
+- Image with Text Overlay
+- Cropped Images with Text
+- List with Images and Links
+- Thumbnail Gallery
+- Image Slider
+- Chart (Bar - Pie - Line - Area - Radar)
+- Map (Marker with rich text description)
 
 ## Supported Versions
-> - Python 3.6 and higher
-> - Wagtail 2 and higher
-> - Bootstrap 4
 
+- Python 3.8 and higher
+- Wagtail 4.1 and higher
+- Bootstrap 4
```

### Comparing `wagtail_blocks-0.8.1/setup.py` & `wagtail_blocks-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # Package dependencies
 install_requires = [
-    "wagtail>=2.15",
-    "wagtailfontawesome>=1.1.4",
+    "wagtail>=4.1,<6.0",
+    "wagtail-font-awesome-svg"
 ]
 
 # Testing dependencies
 testing_extras = [
 ]
 
 # Documentation dependencies
@@ -34,22 +34,24 @@
     author='IbrahimAwadHamid',
     author_email='ibrahim.a.hamid@gmail.com',
     keywords=['WAGTAIL', 'STREAMFIELD', 'WAGTAIL_BLOCKS', 'WAGTAIL CMS'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Framework :: Wagtail',
-        'Framework :: Wagtail :: 2',
-        'Framework :: Wagtail :: 3',
+        'Framework :: Wagtail :: 4',
+        'Framework :: Wagtail :: 5',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development',
```

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/blocks.py` & `wagtail_blocks-1.0.1/wagtail_blocks/blocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import json
 
 from django import forms
-from wagtail import VERSION as WAGTAIL_VERSION
 from wagtail.images.blocks import ImageChooserBlock
 
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail import blocks
-else:
-    from wagtail.core import blocks
+from wagtail import blocks
 
 
 class HeaderChoiceBlock(blocks.ChoiceBlock):
     choices = (
         ('h1', 'H1'),
         ('h2', 'H2'),
         ('h3', 'H3'),
@@ -53,15 +49,15 @@
     text = blocks.CharBlock(
         label='Text',
         max_length=200,
     )
 
     class Meta:
         template = 'wagtail_blocks/image_text_overlay.html'
-        icon = 'fa-image'
+        icon = 'image'
 
 
 class SingleImageWithText(blocks.StructBlock):
     image = ImageChooserBlock(
         label='Image',
     )
     text = blocks.CharBlock(
@@ -74,15 +70,15 @@
     image_items = blocks.ListBlock(
         SingleImageWithText(),
         label="Image Item",
     )
 
     class Meta:
         template = 'wagtail_blocks/cropped_images_with_text.html'
-        icon = 'fa-camera-retro'
+        icon = 'camera-retro'
 
 
 class SingleListImage(blocks.StructBlock):
     image = ImageChooserBlock(
         label='Image',
     )
     title = blocks.CharBlock(
@@ -109,15 +105,15 @@
     list_items = blocks.ListBlock(
         SingleListImage(),
         label="List Item",
     )
 
     class Meta:
         template = 'wagtail_blocks/list_with_images.html'
-        icon = 'fa-id-card-o'
+        icon = 'id-card-alt'
 
 
 class SingleThumbnail(blocks.StructBlock):
     image = ImageChooserBlock(
         label='Image',
     )
 
@@ -126,15 +122,15 @@
     image_items = blocks.ListBlock(
         SingleThumbnail(),
         label="Image",
     )
 
     class Meta:
         template = 'wagtail_blocks/thumbnail_gallery.html'
-        icon = 'fa-object-ungroup'
+        icon = 'object-ungroup'
 
 
 class ChartChoiceBlock(blocks.ChoiceBlock):
     choices = (
         ('bar', 'Bar'),
         ('horizontalBar', 'Horizontal Bar'),
         ('pie', 'Pie'),
@@ -180,15 +176,15 @@
     def get_context(self, value, parent_context=None):
         context = super().get_context(value, parent_context=parent_context)
         value['datasets'] = json.dumps(value['datasets'])
         return context
 
     class Meta:
         template = 'wagtail_blocks/chart.html'
-        icon = 'fa-bar-chart'
+        icon = 'chart-bar'
 
 
 class MapBlock(blocks.StructBlock):
     marker_title = blocks.CharBlock(max_length=120,
                                     default="Marker Title 'This will be updated after you save changes.'")
     marker_description = blocks.RichTextBlock()
     zoom_level = blocks.IntegerBlock(min_value=0, max_value=18, default='2', required=False)
@@ -203,15 +199,15 @@
             js=["https://unpkg.com/leaflet@1.4.0/dist/leaflet.js"],
             css={'all': ["https://unpkg.com/leaflet@1.4.0/dist/leaflet.css"]}
         )
 
     class Meta:
         form_template = 'wagtail_blocks/admin_blocks/map.html'
         template = 'wagtail_blocks/map.html'
-        icon = "fa-globe"
+        icon = "globe"
 
 
 class SingleImageSlide(blocks.StructBlock):
     image = ImageChooserBlock(
         label='Image',
     )
 
@@ -220,8 +216,8 @@
     image_items = blocks.ListBlock(
         SingleImageSlide(),
         label="Image",
     )
 
     class Meta:
         template = 'wagtail_blocks/image_slider.html'
-        icon = 'fa-slideshare'
+        icon = 'sliders-h'
```

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/bootstrap.min.css` & `wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/cropped_images_with_text.css` & `wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/cropped_images_with_text.css`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/image_slider.css` & `wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/image_slider.css`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/image_text_overlay.css` & `wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/image_text_overlay.css`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/js/Chart.bundle.min.js` & `wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/js/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/js/bootstrap.bundle.min.js` & `wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/static/wagtail_blocks/list_with_images.css` & `wagtail_blocks-1.0.1/wagtail_blocks/static/wagtail_blocks/list_with_images.css`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/admin_blocks/map.html` & `wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/admin_blocks/map.html`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/chart.html` & `wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/chart.html`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/cropped_images_with_text.html` & `wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/cropped_images_with_text.html`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/image_slider.html` & `wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/image_slider.html`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/image_text_overlay.html` & `wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/image_text_overlay.html`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/list_with_images.html` & `wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/list_with_images.html`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/map.html` & `wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/map.html`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/templates/wagtail_blocks/thumbnail_gallery.html` & `wagtail_blocks-1.0.1/wagtail_blocks/templates/wagtail_blocks/thumbnail_gallery.html`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks/templatetags/wagtail_html_support.py` & `wagtail_blocks-1.0.1/wagtail_blocks/templatetags/wagtail_html_support.py`

 * *Files identical despite different names*

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks.egg-info/PKG-INFO` & `wagtail_blocks-1.0.1/wagtail_blocks.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,124 @@
-Metadata-Version: 2.1
-Name: wagtail-blocks
-Version: 0.8.1
-Summary: A Collection of awesome Wagtail CMS stream-field blocks and Charts
-Home-page: https://github.com/ibrahimawadhamid/wagtail_blocks/
-Author: IbrahimAwadHamid
-Author-email: ibrahim.a.hamid@gmail.com
-License: MIT
-Keywords: WAGTAIL,STREAMFIELD,WAGTAIL_BLOCKS,WAGTAIL CMS
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: docs
-License-File: LICENSE
-
-# wagtail_blocks ![wagtail](https://img.shields.io/badge/CMS-Wagtail-green.svg)
-[![PyPI](https://img.shields.io/pypi/v/wagtail-blocks.svg)](https://pypi.python.org/pypi/wagtail-blocks) ![Build](https://img.shields.io/pypi/status/wagtail-blocks.svg) [![Documentation Status](https://readthedocs.org/projects/wagtail-blocks/badge/?version=latest)](https://wagtail-blocks.readthedocs.io/en/latest/?badge=latest) ![PyPI - License](https://img.shields.io/pypi/l/wagtail-blocks.svg)
-
-![Downloads](https://static.pepy.tech/badge/wagtail-blocks) ![Downloads Month](https://static.pepy.tech/badge/wagtail-blocks/month) ![Downloads Week](https://static.pepy.tech/badge/wagtail-blocks/week)
-
-A Collection of awesome Wagtail CMS stream-field blocks and Charts.
-
-*Check out [Awesome Wagtail](https://github.com/springload/awesome-wagtail) for more awesome packages and resources from the Wagtail community.*
-
-## Note
-**This project is still early on in its development lifecycle. It is possible for breaking changes to occur between versions until reaching a stable 1.0**, however we will clearly note any breaking changes between releases if applicable. Feedback and pull requests are welcome.
-
-## Quickstart
-
-You must have your [Wagtail](https://wagtail.io/) project up and running:
-
-```sh
-pip install wagtail_blocks
-```
-Add the following enteries to your `settings.py` in the INSTALLED_APPS section:
-
-```python
-'wagtailfontawesome',
-'wagtail_blocks',
-```
-
-## Sample Usage
-```python
-from wagtail_blocks.blocks import HeaderBlock, ListBlock, ImageTextOverlayBlock, CroppedImagesWithTextBlock, \
-    ListWithImagesBlock, ThumbnailGalleryBlock, ChartBlock, MapBlock, ImageSliderBlock
-
-class HomePage(Page):
-    body = StreamField([
-        ('header', HeaderBlock()),
-        ('list', ListBlock()),
-        ('image_text_overlay', ImageTextOverlayBlock()),
-        ('cropped_images_with_text', CroppedImagesWithTextBlock()),
-        ('list_with_images', ListWithImagesBlock()),
-        ('thumbnail_gallery', ThumbnailGalleryBlock()),
-        ('chart', ChartBlock()),
-        ('map', MapBlock()),
-        ('image_slider', ImageSliderBlock()),
-    ], blank=True)
-
-    content_panels = Page.content_panels + [
-        StreamFieldPanel("body", classname="Full"),
-    ]
-
-```
-### For HomePage template, blocks should be rendered with IDs to function properly
-```
-{% for block in page.body %}
-    {% include_block block with block_id=block.id %}
-{% endfor %}
-```
-
-## Available Blocks
-Check Showcase for [Standard Blocks](https://wagtail-blocks.readthedocs.io/en/latest/showcase/standard-blocks/) 
-or [Charts](https://wagtail-blocks.readthedocs.io/en/latest/showcase/chart/)
-or [Maps](https://wagtail-blocks.readthedocs.io/en/latest/showcase/map/)
-![streamfield](https://wagtail-blocks.readthedocs.io/en/latest/showcase/screenshots/streamfield.PNG)
- 
-> - Header (H1, H2, H3, H4, H5, H6)
-> - List (Unordered List)
-> - Image with Text Overlay
-> - Cropped Images with Text
-> - List with Images and Links
-> - Thumbnail Gallery
-> - Image Slider
-> - Chart (Bar - Pie - Line - Area - Radar)
-> - Map (Marker with rich text description)
-
-## Supported Versions
-> - Python 3.6 and higher
-> - Wagtail 2 and higher
-> - Bootstrap 4
-
+Metadata-Version: 2.1
+Name: wagtail-blocks
+Version: 1.0.1
+Summary: A Collection of awesome Wagtail CMS stream-field blocks and Charts
+Home-page: https://github.com/ibrahimawadhamid/wagtail_blocks/
+Author: IbrahimAwadHamid
+Author-email: ibrahim.a.hamid@gmail.com
+License: MIT
+Keywords: WAGTAIL,STREAMFIELD,WAGTAIL_BLOCKS,WAGTAIL CMS
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: docs
+License-File: LICENSE
+
+# wagtail_blocks ![wagtail](https://img.shields.io/badge/CMS-Wagtail-green.svg)
+
+[![PyPI](https://img.shields.io/pypi/v/wagtail-blocks.svg)](https://pypi.python.org/pypi/wagtail-blocks) ![Build](https://img.shields.io/pypi/status/wagtail-blocks.svg) [![Documentation Status](https://readthedocs.org/projects/wagtail-blocks/badge/?version=latest)](https://wagtail-blocks.readthedocs.io/en/latest/?badge=latest) ![PyPI - License](https://img.shields.io/pypi/l/wagtail-blocks.svg)
+
+![Downloads](https://static.pepy.tech/badge/wagtail-blocks) ![Downloads Month](https://static.pepy.tech/badge/wagtail-blocks/month) ![Downloads Week](https://static.pepy.tech/badge/wagtail-blocks/week)
+
+A Collection of awesome Wagtail CMS stream-field blocks and Charts.
+
+*Check out [Awesome Wagtail](https://github.com/springload/awesome-wagtail) for more awesome packages and resources from the Wagtail community.*
+
+## Quickstart
+
+You must have your [Wagtail](https://wagtail.io/) project up and running:
+
+```sh
+pip install wagtail_blocks
+```
+
+Add the following enteries to your `settings.py` in the INSTALLED_APPS section:
+
+```python
+'wagtailfontawesomesvg',
+'wagtail_blocks',
+```
+
+## Sample Usage
+
+```python
+from wagtail.fields import StreamField
+from wagtail.admin.panels import FieldPanel
+
+from wagtail_blocks.blocks import (
+    HeaderBlock,
+    ListBlock,
+    ImageTextOverlayBlock,
+    CroppedImagesWithTextBlock,
+    ListWithImagesBlock,
+    ThumbnailGalleryBlock,
+    ChartBlock,
+    MapBlock,
+    ImageSliderBlock,
+)
+
+class HomePage(Page):
+    body = StreamField([
+        ('header', HeaderBlock()),
+        ('list', ListBlock()),
+        ('image_text_overlay', ImageTextOverlayBlock()),
+        ('cropped_images_with_text', CroppedImagesWithTextBlock()),
+        ('list_with_images', ListWithImagesBlock()),
+        ('thumbnail_gallery', ThumbnailGalleryBlock()),
+        ('chart', ChartBlock()),
+        ('map', MapBlock()),
+        ('image_slider', ImageSliderBlock()),
+    ], blank=True, use_json_field=True)
+
+    content_panels = Page.content_panels + [
+        FieldPanel("body"),
+    ]
+```
+
+### For HomePage template, blocks should be rendered with IDs to function properly
+
+```html
+{% for block in page.body %}
+    {% include_block block with block_id=block.id %}
+{% endfor %}
+```
+
+## Available Blocks
+
+Check Showcase for [Standard Blocks](docs/showcase/standard-blocks.md) or [Charts](docs/showcase/chart.md) or [Maps](docs/showcase/map.md)
+
+![streamfield](docs/showcase/screenshots/streamfield-v5.PNG)
+
+- Header (H1, H2, H3, H4, H5, H6)
+- List (Unordered List)
+- Image with Text Overlay
+- Cropped Images with Text
+- List with Images and Links
+- Thumbnail Gallery
+- Image Slider
+- Chart (Bar - Pie - Line - Area - Radar)
+- Map (Marker with rich text description)
+
+## Supported Versions
+
+- Python 3.8 and higher
+- Wagtail 4.1 and higher
+- Bootstrap 4
```

### Comparing `wagtail_blocks-0.8.1/wagtail_blocks.egg-info/SOURCES.txt` & `wagtail_blocks-1.0.1/wagtail_blocks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 requirements.txt
 setup.cfg
 setup.py
 wagtail_blocks/__init__.py
 wagtail_blocks/blocks.py
 wagtail_blocks/test_dummy.py
+wagtail_blocks/wagtail_hooks.py
 wagtail_blocks.egg-info/PKG-INFO
 wagtail_blocks.egg-info/SOURCES.txt
 wagtail_blocks.egg-info/dependency_links.txt
 wagtail_blocks.egg-info/requires.txt
 wagtail_blocks.egg-info/top_level.txt
 wagtail_blocks/static/wagtail_blocks/bootstrap.min.css
 wagtail_blocks/static/wagtail_blocks/cropped_images_with_text.css
```

