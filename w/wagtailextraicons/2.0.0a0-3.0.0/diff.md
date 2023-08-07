# Comparing `tmp/wagtailextraicons-2.0.0a0.tar.gz` & `tmp/wagtailextraicons-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailextraicons-2.0.0a0.tar", last modified: Mon Feb 21 01:58:18 2022, max compression
+gzip compressed data, was "wagtailextraicons-3.0.0.tar", last modified: Mon Aug  7 04:30:20 2023, max compression
```

## Comparing `wagtailextraicons-2.0.0a0.tar` & `wagtailextraicons-3.0.0.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2022-02-21 01:58:18.233610 wagtailextraicons-2.0.0a0/
--rw-r--r--   0 pat        (501) staff       (20)     1506 2022-02-21 01:24:17.000000 wagtailextraicons-2.0.0a0/LICENSE
--rw-r--r--   0 pat        (501) staff       (20)       73 2022-02-21 01:36:55.000000 wagtailextraicons-2.0.0a0/MANIFEST.in
--rw-r--r--   0 pat        (501) staff       (20)     3164 2022-02-21 01:58:18.233741 wagtailextraicons-2.0.0a0/PKG-INFO
--rw-r--r--   0 pat        (501) staff       (20)     2305 2022-02-21 01:05:55.000000 wagtailextraicons-2.0.0a0/README.md
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2022-02-21 01:58:18.193651 wagtailextraicons-2.0.0a0/docs/
--rw-r--r--   0 pat        (501) staff       (20)     6130 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/docs/icons.md
--rw-r--r--   0 pat        (501) staff       (20)      788 2022-02-21 01:58:18.234322 wagtailextraicons-2.0.0a0/setup.cfg
--rw-r--r--   0 pat        (501) staff       (20)     3362 2022-02-21 01:57:53.000000 wagtailextraicons-2.0.0a0/setup.py
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2022-02-21 01:58:18.195990 wagtailextraicons-2.0.0a0/wagtailextraicons/
--rw-r--r--   0 pat        (501) staff       (20)       98 2022-02-21 01:00:04.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/__init__.py
--rw-r--r--   0 pat        (501) staff       (20)      145 2022-02-17 22:21:14.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/apps.py
--rw-r--r--   0 pat        (501) staff       (20)     1908 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/icon_register.py
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2022-02-21 01:58:18.198094 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/
--rw-r--r--   0 pat        (501) staff       (20)     6148 2022-02-21 01:58:02.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/.DS_Store
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2022-02-21 01:58:18.233332 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/
--rw-r--r--   0 pat        (501) staff       (20)        0 2022-02-21 00:22:00.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/.keep
--rw-r--r--   0 pat        (501) staff       (20)      287 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--2-col-heading-text.svg
--rw-r--r--   0 pat        (501) staff       (20)      180 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--2-col-lg.svg
--rw-r--r--   0 pat        (501) staff       (20)      200 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--2-col-paragraph.svg
--rw-r--r--   0 pat        (501) staff       (20)      290 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--2-col-right-small.svg
--rw-r--r--   0 pat        (501) staff       (20)      309 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--2-col-video.svg
--rw-r--r--   0 pat        (501) staff       (20)      253 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--2-col-with-links.svg
--rw-r--r--   0 pat        (501) staff       (20)      163 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--2-col.svg
--rw-r--r--   0 pat        (501) staff       (20)      283 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--3-col-links.svg
--rw-r--r--   0 pat        (501) staff       (20)      251 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--3-col.svg
--rw-r--r--   0 pat        (501) staff       (20)      211 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--4-col-heading.svg
--rw-r--r--   0 pat        (501) staff       (20)      276 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--4-col.svg
--rw-r--r--   0 pat        (501) staff       (20)      364 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--banner.svg
--rw-r--r--   0 pat        (501) staff       (20)      151 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--basic-field.svg
--rw-r--r--   0 pat        (501) staff       (20)      170 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--block-quote.svg
--rw-r--r--   0 pat        (501) staff       (20)      101 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--button.svg
--rw-r--r--   0 pat        (501) staff       (20)      371 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--cards.svg
--rw-r--r--   0 pat        (501) staff       (20)      234 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--checkbox.svg
--rw-r--r--   0 pat        (501) staff       (20)      683 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--checkboxes.svg
--rw-r--r--   0 pat        (501) staff       (20)      226 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--cta-inverted.svg
--rw-r--r--   0 pat        (501) staff       (20)      161 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--cta-with-button.svg
--rw-r--r--   0 pat        (501) staff       (20)      148 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--cta.svg
--rw-r--r--   0 pat        (501) staff       (20)      215 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--date.svg
--rw-r--r--   0 pat        (501) staff       (20)      240 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--dropdown.svg
--rw-r--r--   0 pat        (501) staff       (20)      306 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--email.svg
--rw-r--r--   0 pat        (501) staff       (20)      147 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--heading-icon.svg
--rw-r--r--   0 pat        (501) staff       (20)      257 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--hidden.svg
--rw-r--r--   0 pat        (501) staff       (20)      448 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--image-gallery.svg
--rw-r--r--   0 pat        (501) staff       (20)      212 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--image.svg
--rw-r--r--   0 pat        (501) staff       (20)      516 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--large-list.svg
--rw-r--r--   0 pat        (501) staff       (20)      892 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--logos.svg
--rw-r--r--   0 pat        (501) staff       (20)      469 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--map-and-content.svg
--rw-r--r--   0 pat        (501) staff       (20)      289 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--map-pin.svg
--rw-r--r--   0 pat        (501) staff       (20)      355 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--map.svg
--rw-r--r--   0 pat        (501) staff       (20)      632 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--money.svg
--rw-r--r--   0 pat        (501) staff       (20)      388 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--multi-select.svg
--rw-r--r--   0 pat        (501) staff       (20)      380 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--multiple-items.svg
--rw-r--r--   0 pat        (501) staff       (20)      220 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--notice.svg
--rw-r--r--   0 pat        (501) staff       (20)      967 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--number.svg
--rw-r--r--   0 pat        (501) staff       (20)      202 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--paragraph.svg
--rw-r--r--   0 pat        (501) staff       (20)      223 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--paragraphs.svg
--rw-r--r--   0 pat        (501) staff       (20)      542 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--people.svg
--rw-r--r--   0 pat        (501) staff       (20)      269 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--person-solo.svg
--rw-r--r--   0 pat        (501) staff       (20)      253 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--person.svg
--rw-r--r--   0 pat        (501) staff       (20)      147 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--quote.svg
--rw-r--r--   0 pat        (501) staff       (20)      479 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--radio.svg
--rw-r--r--   0 pat        (501) staff       (20)      206 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--sign-up.svg
--rw-r--r--   0 pat        (501) staff       (20)      414 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--small-list.svg
--rw-r--r--   0 pat        (501) staff       (20)      249 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--table.svg
--rw-r--r--   0 pat        (501) staff       (20)      199 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--tabs.svg
--rw-r--r--   0 pat        (501) staff       (20)      245 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--testimonial.svg
--rw-r--r--   0 pat        (501) staff       (20)      346 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--text-box.svg
--rw-r--r--   0 pat        (501) staff       (20)      412 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--three-items.svg
--rw-r--r--   0 pat        (501) staff       (20)      669 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--url.svg
--rw-r--r--   0 pat        (501) staff       (20)      565 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--useful-links.svg
--rw-r--r--   0 pat        (501) staff       (20)      277 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--video.svg
--rw-r--r--   0 pat        (501) staff       (20)      571 2022-02-21 01:50:59.000000 wagtailextraicons-2.0.0a0/wagtailextraicons/wagtail_hooks.py
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2022-02-21 01:58:18.197686 wagtailextraicons-2.0.0a0/wagtailextraicons.egg-info/
--rw-r--r--   0 pat        (501) staff       (20)     3164 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons.egg-info/PKG-INFO
--rw-r--r--   0 pat        (501) staff       (20)     3990 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons.egg-info/SOURCES.txt
--rw-r--r--   0 pat        (501) staff       (20)        1 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons.egg-info/dependency_links.txt
--rw-r--r--   0 pat        (501) staff       (20)       18 2022-02-21 01:58:17.000000 wagtailextraicons-2.0.0a0/wagtailextraicons.egg-info/top_level.txt
+drwxrwxr-x   0 jelle     (1000) jelle     (1000)        0 2023-08-07 04:30:20.475332 wagtailextraicons-3.0.0/
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)     1506 2023-08-07 03:09:40.000000 wagtailextraicons-3.0.0/LICENSE.txt
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)       73 2023-07-27 02:12:53.000000 wagtailextraicons-3.0.0/MANIFEST.in
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)     3274 2023-08-07 04:30:20.475332 wagtailextraicons-3.0.0/PKG-INFO
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)     2543 2023-08-07 03:09:40.000000 wagtailextraicons-3.0.0/README.md
+drwxrwxr-x   0 jelle     (1000) jelle     (1000)        0 2023-08-07 04:30:20.471332 wagtailextraicons-3.0.0/docs/
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)     6130 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/docs/icons.md
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      813 2023-08-07 04:30:20.475332 wagtailextraicons-3.0.0/setup.cfg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)     3347 2023-08-07 04:17:19.000000 wagtailextraicons-3.0.0/setup.py
+drwxrwxr-x   0 jelle     (1000) jelle     (1000)        0 2023-08-07 04:30:20.471332 wagtailextraicons-3.0.0/wagtailextraicons/
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)       22 2023-08-07 03:09:40.000000 wagtailextraicons-3.0.0/wagtailextraicons/__init__.py
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      144 2023-08-07 03:09:40.000000 wagtailextraicons-3.0.0/wagtailextraicons/apps.py
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)     1908 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/icon_register.py
+drwxrwxr-x   0 jelle     (1000) jelle     (1000)        0 2023-08-07 04:30:20.471332 wagtailextraicons-3.0.0/wagtailextraicons/templates/
+drwxrwxr-x   0 jelle     (1000) jelle     (1000)        0 2023-08-07 04:30:20.475332 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      287 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--2-col-heading-text.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      180 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--2-col-lg.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      200 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--2-col-paragraph.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      290 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--2-col-right-small.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      309 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--2-col-video.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      253 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--2-col-with-links.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      163 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--2-col.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      283 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--3-col-links.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      251 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--3-col.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      211 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--4-col-heading.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      276 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--4-col.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      364 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--banner.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      151 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--basic-field.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      170 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--block-quote.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      101 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--button.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      371 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--cards.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      234 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--checkbox.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      683 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--checkboxes.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      226 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--cta-inverted.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      161 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--cta-with-button.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      148 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--cta.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      215 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--date.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      240 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--dropdown.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      306 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--email.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      147 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--heading-icon.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      257 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--hidden.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      448 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--image-gallery.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      212 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--image.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      516 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--large-list.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      892 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--logos.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      469 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--map-and-content.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      289 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--map-pin.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      355 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--map.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      632 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--money.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      388 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--multi-select.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      380 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--multiple-items.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      220 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--notice.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      967 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--number.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      202 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--paragraph.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      223 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--paragraphs.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      542 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--people.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      269 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--person-solo.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      253 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--person.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      147 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--quote.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      479 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--radio.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      206 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--sign-up.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      414 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--small-list.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      249 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--table.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      199 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--tabs.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      245 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--testimonial.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      346 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--text-box.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      412 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--three-items.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      669 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--url.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      565 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--useful-links.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      277 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--video.svg
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)      396 2023-08-07 03:09:40.000000 wagtailextraicons-3.0.0/wagtailextraicons/wagtail_hooks.py
+drwxrwxr-x   0 jelle     (1000) jelle     (1000)        0 2023-08-07 04:30:20.471332 wagtailextraicons-3.0.0/wagtailextraicons.egg-info/
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)     3274 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons.egg-info/PKG-INFO
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)     3951 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons.egg-info/SOURCES.txt
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)        1 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons.egg-info/dependency_links.txt
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)       13 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons.egg-info/requires.txt
+-rw-rw-r--   0 jelle     (1000) jelle     (1000)       18 2023-08-07 04:30:20.000000 wagtailextraicons-3.0.0/wagtailextraicons.egg-info/top_level.txt
```

### Comparing `wagtailextraicons-2.0.0a0/LICENSE` & `wagtailextraicons-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/PKG-INFO` & `wagtailextraicons-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: wagtailextraicons
-Version: 2.0.0a0
+Version: 3.0.0
 Summary: Add extra icons to your Wagtail project.
 Home-page: https://github.com/octavenz/wagtailextraicons
 Author: Sam Costigan (Octave)
-Author-email: sam@octave.nz
+Author-email: support@octave.nz
 License: BSD-3-Clause
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Framework :: Django
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # Wagtail Extra Icons
 
 Add extra icons to your Wagtail project.
 
 ## Versions
 
+#### Version 3.X.X
+Is for use with Wagtail versions 3.0 and above. This uses Wagtail's updated module paths from version 3.0.
+
 #### Version 2.X.X
 Is for use with Wagtail versions 2.15 and above. This version uses wagtail's new Svg icon system. 
 
+This version works with Wagtail versions 3.0 and 4.*, but is deprecated for those.
+
 #### Version 1.X.X
 Is for use with Wagtail versions below 2.15. This version uses wagtail's old Icon font system. 
 
 ---
 
 ## Install
 
@@ -54,34 +55,34 @@
 ## Usage
 
 The full list of icons is available at [docs/icons.md](https://github.com/octavenz/wagtailextraicons/blob/master/docs/icons.md). 
 All icons are namespaced as `extraicons--` to avoid clashing with existing Wagtail icons. You can add the extra icons to 
 your StreamField blocks like any other:
 
 ```python
-content = StreamField([
-    (
-        'paragraph',
-        blocks.RichTextBlock(icon='extraicons--paragraph')
-    ),
-])
+content = StreamField(
+    [
+        ('paragraph', blocks.RichTextBlock(icon='extraicons--paragraph')),
+    ],
+    use_json_field=True,    
+)
 ```
 
 You can also add the extra icons to your own custom `StructBlock` classes:
 
 ```python
 class PersonBlock(blocks.StructBlock):
     person = SnippetChooserBlock('app.Person')
     text = blocks.RichTextBlock()
 
     class Meta:
         icon = 'extraicons--person'
 ```
 
-Reference the [Wagtail docs](http://docs.wagtail.io/en/latest/topics/streamfield.html) for all the ways to include icons.  
+Reference the [Wagtail docs](https://docs.wagtail.org/en/latest/topics/streamfield.html) for all the ways to include icons.  
 
 ## Authors
 
 * **Sam Costigan** [Octave](https://github.com/octavenz)
 
 ## Contributing
 
@@ -95,10 +96,8 @@
 so prefer paths where possible.
 * Don't set colours on your SVG.
 
 Code pull requests are also welcome.
 
 ## License
 
-This project is licensed under the BSD License - see the [LICENSE.md](LICENSE.md) file for details
-
-
+This project is licensed under the BSD License - see the [LICENSE.txt](LICENSE.txt) file for details.
```

### Comparing `wagtailextraicons-2.0.0a0/README.md` & `wagtailextraicons-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # Wagtail Extra Icons
 
 Add extra icons to your Wagtail project.
 
 ## Versions
 
+#### Version 3.X.X
+Is for use with Wagtail versions 3.0 and above. This uses Wagtail's updated module paths from version 3.0.
+
 #### Version 2.X.X
 Is for use with Wagtail versions 2.15 and above. This version uses wagtail's new Svg icon system. 
 
+This version works with Wagtail versions 3.0 and 4.*, but is deprecated for those.
+
 #### Version 1.X.X
 Is for use with Wagtail versions below 2.15. This version uses wagtail's old Icon font system. 
 
 ---
 
 ## Install
 
@@ -30,34 +35,34 @@
 ## Usage
 
 The full list of icons is available at [docs/icons.md](https://github.com/octavenz/wagtailextraicons/blob/master/docs/icons.md). 
 All icons are namespaced as `extraicons--` to avoid clashing with existing Wagtail icons. You can add the extra icons to 
 your StreamField blocks like any other:
 
 ```python
-content = StreamField([
-    (
-        'paragraph',
-        blocks.RichTextBlock(icon='extraicons--paragraph')
-    ),
-])
+content = StreamField(
+    [
+        ('paragraph', blocks.RichTextBlock(icon='extraicons--paragraph')),
+    ],
+    use_json_field=True,    
+)
 ```
 
 You can also add the extra icons to your own custom `StructBlock` classes:
 
 ```python
 class PersonBlock(blocks.StructBlock):
     person = SnippetChooserBlock('app.Person')
     text = blocks.RichTextBlock()
 
     class Meta:
         icon = 'extraicons--person'
 ```
 
-Reference the [Wagtail docs](http://docs.wagtail.io/en/latest/topics/streamfield.html) for all the ways to include icons.  
+Reference the [Wagtail docs](https://docs.wagtail.org/en/latest/topics/streamfield.html) for all the ways to include icons.  
 
 ## Authors
 
 * **Sam Costigan** [Octave](https://github.com/octavenz)
 
 ## Contributing
 
@@ -71,8 +76,8 @@
 so prefer paths where possible.
 * Don't set colours on your SVG.
 
 Code pull requests are also welcome.
 
 ## License
 
-This project is licensed under the BSD License - see the [LICENSE.md](LICENSE.md) file for details
+This project is licensed under the BSD License - see the [LICENSE.txt](LICENSE.txt) file for details.
```

### Comparing `wagtailextraicons-2.0.0a0/docs/icons.md` & `wagtailextraicons-3.0.0/docs/icons.md`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/setup.cfg` & `wagtailextraicons-3.0.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [metadata]
-description-file = README.md
 name = wagtailextraicons
+version = 3.0.0
 description = Add extra icons to your Wagtail project.
+description-file = README.md
 long_description = file: README.md
 long_description_content_type = text/markdown
+url = https://github.com/octavenz/wagtailextraicons
 author = Sam Costigan (Octave)
-author_email = sam@octave.nz
+author_email = support@octave.nz
 license = BSD-3-Clause
 classifiers = 
-	Development Status :: 3 - Alpha
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
-	Framework :: Django
-	Framework :: Wagtail
-	Framework :: Wagtail :: 2
+	Framework :: Wagtail :: 3
+	Framework :: Wagtail :: 4
 	Operating System :: OS Independent
-	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Site Management
 
 [options]
 include_package_data = true
 packages = find:
+install_requires = 
+	wagtail>=3.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wagtailextraicons-2.0.0a0/setup.py` & `wagtailextraicons-3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-import os
-from bs4 import BeautifulSoup
 import glob
-
-
-from setuptools import find_packages, setup
-from setuptools.command.sdist import sdist as base_sdist
+import os
+from setuptools import setup
 from setuptools.command.bdist_egg import bdist_egg as base_bdist_egg
+from setuptools.command.sdist import sdist as base_sdist
+
+from bs4 import BeautifulSoup
 
 from wagtailextraicons import __version__
 
 
 url = 'https://github.com/octavenz/wagtailextraicons'
 icon_src_dir = 'lib/icons'
 
 
 class IconsDocMixin:
-    def build_icons_doc(self):
+
+    @staticmethod
+    def build_icons_doc():
         extraicons = os.listdir(icon_src_dir)
 
         with open('docs/icons.md', 'w') as file:
             file.write('| Icon | Name |\n')
             file.write('| --- | --- |\n')
             for icon_file in sorted(extraicons):
                 icon_name = icon_file.split('.')[0]
                 icon_image_url = '{0}/blob/master/{1}/{2}'.format(url, icon_src_dir, icon_file)
                 file.write(
                     '| ![{name}]({url}) | {name} |\n'.format(name=icon_name, url=icon_image_url)
                 )
 
 
 class IconRegisterMixin:
+
     icon_register = []
     icon_paths = []
     icon_dest_dir = 'wagtailextraicons/templates/extraicons'
     icon_register_path = 'wagtailextraicons/icon_register.py'
 
     def register_icons(self):
         self.icon_paths = glob.glob(f'{icon_src_dir}/*.svg')
@@ -56,33 +58,32 @@
                 else:
                     print(f'No Svg Found - {icon_path}')
 
     @staticmethod
     def convert_svg_to_symbol(file_contents, name):
         soup = BeautifulSoup(file_contents, 'html.parser')
         svg = soup.find('svg')
+        if not svg:
+            return None
 
-        if svg:
-            svg.name = 'symbol'
-            svg.attrs = {
-                'id': f'icon-{name}',
-                'viewbox': svg['viewbox']
-            }
-            return svg
-
-        return None
+        svg.name = 'symbol'
+        svg.attrs = {
+            'id': f'icon-{name}',
+            'viewbox': svg['viewbox'],
+        }
+        return svg
 
     def write_symbol_to_template(self, symbol, file_name):
-        html = symbol.prettify("utf-8")
+        html = symbol.prettify('utf-8')
 
-        with open(f"{self.icon_dest_dir}/{file_name}", "wb") as file:
+        with open(f'{self.icon_dest_dir}/{file_name}', 'wb') as file:
             file.write(html)
 
     def write_icon_register_module(self):
-        with open(self.icon_register_path, "w") as file:
+        with open(self.icon_register_path, 'w') as file:
             output = "# This file is generated. Don't edit directly\n"
             icons_str = ''
 
             for icon_name in self.icon_register:
                 icons_str += f"\n    '{icon_name}', "
 
             output += f'icons = [{ icons_str }\n]\n'
@@ -104,10 +105,10 @@
 
 
 setup(
     url=url,
     version=__version__,
     cmdclass={
         'sdist': sdist,
-        'bdist_egg': bdist_egg
+        'bdist_egg': bdist_egg,
     },
 )
```

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons/icon_register.py` & `wagtailextraicons-3.0.0/wagtailextraicons/icon_register.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # This file is generated. Don't edit directly
 icons = [
-    'extraicons--cta-with-button.svg', 
-    'extraicons--2-col-paragraph.svg', 
-    'extraicons--testimonial.svg', 
-    'extraicons--multiple-items.svg', 
+    'extraicons--logos.svg', 
+    'extraicons--checkbox.svg', 
+    'extraicons--2-col-right-small.svg', 
     'extraicons--person.svg', 
+    'extraicons--basic-field.svg', 
     'extraicons--hidden.svg', 
+    'extraicons--tabs.svg', 
+    'extraicons--map-and-content.svg', 
     'extraicons--map.svg', 
-    'extraicons--person-solo.svg', 
-    'extraicons--2-col-lg.svg', 
-    'extraicons--4-col.svg', 
-    'extraicons--banner.svg', 
-    'extraicons--2-col-video.svg', 
-    'extraicons--checkboxes.svg', 
-    'extraicons--2-col-with-links.svg', 
+    'extraicons--sign-up.svg', 
+    'extraicons--image.svg', 
     'extraicons--paragraphs.svg', 
-    'extraicons--three-items.svg', 
-    'extraicons--number.svg', 
-    'extraicons--radio.svg', 
-    'extraicons--paragraph.svg', 
-    'extraicons--tabs.svg', 
-    'extraicons--small-list.svg', 
-    'extraicons--email.svg', 
+    'extraicons--quote.svg', 
+    'extraicons--image-gallery.svg', 
+    'extraicons--3-col.svg', 
     'extraicons--people.svg', 
-    'extraicons--button.svg', 
-    'extraicons--image.svg', 
-    'extraicons--basic-field.svg', 
-    'extraicons--table.svg', 
-    'extraicons--sign-up.svg', 
-    'extraicons--2-col-right-small.svg', 
-    'extraicons--notice.svg', 
-    'extraicons--cta-inverted.svg', 
-    'extraicons--checkbox.svg', 
-    'extraicons--map-and-content.svg', 
-    'extraicons--large-list.svg', 
-    'extraicons--dropdown.svg', 
-    'extraicons--3-col-links.svg', 
-    'extraicons--money.svg', 
     'extraicons--text-box.svg', 
+    'extraicons--multiple-items.svg', 
+    'extraicons--money.svg', 
+    'extraicons--paragraph.svg', 
+    'extraicons--multi-select.svg', 
+    'extraicons--cta.svg', 
+    'extraicons--three-items.svg', 
+    'extraicons--3-col-links.svg', 
+    'extraicons--cta-inverted.svg', 
+    'extraicons--date.svg', 
+    'extraicons--notice.svg', 
+    'extraicons--2-col-with-links.svg', 
+    'extraicons--2-col-lg.svg', 
+    'extraicons--2-col-heading-text.svg', 
+    'extraicons--cta-with-button.svg', 
+    'extraicons--2-col-video.svg', 
+    'extraicons--2-col-paragraph.svg', 
+    'extraicons--cards.svg', 
+    'extraicons--table.svg', 
     'extraicons--video.svg', 
+    'extraicons--number.svg', 
+    'extraicons--large-list.svg', 
+    'extraicons--email.svg', 
+    'extraicons--block-quote.svg', 
+    'extraicons--small-list.svg', 
     'extraicons--map-pin.svg', 
     'extraicons--4-col-heading.svg', 
-    'extraicons--useful-links.svg', 
-    'extraicons--3-col.svg', 
-    'extraicons--quote.svg', 
-    'extraicons--logos.svg', 
-    'extraicons--heading-icon.svg', 
-    'extraicons--image-gallery.svg', 
-    'extraicons--date.svg', 
-    'extraicons--block-quote.svg', 
-    'extraicons--multi-select.svg', 
+    'extraicons--checkboxes.svg', 
+    'extraicons--dropdown.svg', 
+    'extraicons--banner.svg', 
+    'extraicons--person-solo.svg', 
     'extraicons--2-col.svg', 
-    'extraicons--2-col-heading-text.svg', 
-    'extraicons--cards.svg', 
+    'extraicons--heading-icon.svg', 
     'extraicons--url.svg', 
-    'extraicons--cta.svg', 
+    'extraicons--radio.svg', 
+    'extraicons--button.svg', 
+    'extraicons--testimonial.svg', 
+    'extraicons--useful-links.svg', 
+    'extraicons--4-col.svg', 
 ]
```

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--checkboxes.svg` & `wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--checkboxes.svg`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--large-list.svg` & `wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--large-list.svg`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--logos.svg` & `wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--logos.svg`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--money.svg` & `wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--money.svg`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--number.svg` & `wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--number.svg`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--people.svg` & `wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--people.svg`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--url.svg` & `wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--url.svg`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons/templates/extraicons/extraicons--useful-links.svg` & `wagtailextraicons-3.0.0/wagtailextraicons/templates/extraicons/extraicons--useful-links.svg`

 * *Files identical despite different names*

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons.egg-info/PKG-INFO` & `wagtailextraicons-3.0.0/wagtailextraicons.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: wagtailextraicons
-Version: 2.0.0a0
+Version: 3.0.0
 Summary: Add extra icons to your Wagtail project.
 Home-page: https://github.com/octavenz/wagtailextraicons
 Author: Sam Costigan (Octave)
-Author-email: sam@octave.nz
+Author-email: support@octave.nz
 License: BSD-3-Clause
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Framework :: Django
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # Wagtail Extra Icons
 
 Add extra icons to your Wagtail project.
 
 ## Versions
 
+#### Version 3.X.X
+Is for use with Wagtail versions 3.0 and above. This uses Wagtail's updated module paths from version 3.0.
+
 #### Version 2.X.X
 Is for use with Wagtail versions 2.15 and above. This version uses wagtail's new Svg icon system. 
 
+This version works with Wagtail versions 3.0 and 4.*, but is deprecated for those.
+
 #### Version 1.X.X
 Is for use with Wagtail versions below 2.15. This version uses wagtail's old Icon font system. 
 
 ---
 
 ## Install
 
@@ -54,34 +55,34 @@
 ## Usage
 
 The full list of icons is available at [docs/icons.md](https://github.com/octavenz/wagtailextraicons/blob/master/docs/icons.md). 
 All icons are namespaced as `extraicons--` to avoid clashing with existing Wagtail icons. You can add the extra icons to 
 your StreamField blocks like any other:
 
 ```python
-content = StreamField([
-    (
-        'paragraph',
-        blocks.RichTextBlock(icon='extraicons--paragraph')
-    ),
-])
+content = StreamField(
+    [
+        ('paragraph', blocks.RichTextBlock(icon='extraicons--paragraph')),
+    ],
+    use_json_field=True,    
+)
 ```
 
 You can also add the extra icons to your own custom `StructBlock` classes:
 
 ```python
 class PersonBlock(blocks.StructBlock):
     person = SnippetChooserBlock('app.Person')
     text = blocks.RichTextBlock()
 
     class Meta:
         icon = 'extraicons--person'
 ```
 
-Reference the [Wagtail docs](http://docs.wagtail.io/en/latest/topics/streamfield.html) for all the ways to include icons.  
+Reference the [Wagtail docs](https://docs.wagtail.org/en/latest/topics/streamfield.html) for all the ways to include icons.  
 
 ## Authors
 
 * **Sam Costigan** [Octave](https://github.com/octavenz)
 
 ## Contributing
 
@@ -95,10 +96,8 @@
 so prefer paths where possible.
 * Don't set colours on your SVG.
 
 Code pull requests are also welcome.
 
 ## License
 
-This project is licensed under the BSD License - see the [LICENSE.md](LICENSE.md) file for details
-
-
+This project is licensed under the BSD License - see the [LICENSE.txt](LICENSE.txt) file for details.
```

### Comparing `wagtailextraicons-2.0.0a0/wagtailextraicons.egg-info/SOURCES.txt` & `wagtailextraicons-3.0.0/wagtailextraicons.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-LICENSE
+LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 docs/icons.md
 wagtailextraicons/__init__.py
 wagtailextraicons/apps.py
 wagtailextraicons/icon_register.py
 wagtailextraicons/wagtail_hooks.py
 wagtailextraicons.egg-info/PKG-INFO
 wagtailextraicons.egg-info/SOURCES.txt
 wagtailextraicons.egg-info/dependency_links.txt
+wagtailextraicons.egg-info/requires.txt
 wagtailextraicons.egg-info/top_level.txt
-wagtailextraicons/templates/.DS_Store
-wagtailextraicons/templates/extraicons/.keep
 wagtailextraicons/templates/extraicons/extraicons--2-col-heading-text.svg
 wagtailextraicons/templates/extraicons/extraicons--2-col-lg.svg
 wagtailextraicons/templates/extraicons/extraicons--2-col-paragraph.svg
 wagtailextraicons/templates/extraicons/extraicons--2-col-right-small.svg
 wagtailextraicons/templates/extraicons/extraicons--2-col-video.svg
 wagtailextraicons/templates/extraicons/extraicons--2-col-with-links.svg
 wagtailextraicons/templates/extraicons/extraicons--2-col.svg
```

