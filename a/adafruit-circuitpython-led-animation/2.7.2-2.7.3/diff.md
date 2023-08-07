# Comparing `tmp/adafruit-circuitpython-led-animation-2.7.2.tar.gz` & `tmp/adafruit-circuitpython-led-animation-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-led-animation-2.7.2.tar", last modified: Fri May 26 16:10:55 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-led-animation-2.7.3.tar", last modified: Mon Aug  7 01:08:26 2023, max compression
```

## Comparing `adafruit-circuitpython-led-animation-2.7.2.tar` & `adafruit-circuitpython-led-animation-2.7.3.tar`

### file list

```diff
@@ -1,87 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.413671 adafruit-circuitpython-led-animation-2.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.405671 adafruit-circuitpython-led-animation-2.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.409670 adafruit-circuitpython-led-animation-2.7.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.409670 adafruit-circuitpython-led-animation-2.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.409670 adafruit-circuitpython-led-animation-2.7.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-26 16:10:55.413671 adafruit-circuitpython-led-animation-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.409670 adafruit-circuitpython-led-animation-2.7.2/adafruit_circuitpython_led_animation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-26 16:10:55.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_circuitpython_led_animation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-26 16:10:55.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_circuitpython_led_animation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:10:55.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_circuitpython_led_animation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:10:55.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_circuitpython_led_animation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 16:10:55.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_circuitpython_led_animation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.409670 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.413671 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/blink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/chase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/colorcycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/customcolorchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/grid_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/multicolor_comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/pulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/rainbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/rainbowchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/rainbowcomet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/rainbowsparkle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/solid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/sparkle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/sparklepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.413671 adafruit-circuitpython-led-animation-2.7.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.413671 adafruit-circuitpython-led-animation-2.7.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:55.413671 adafruit-circuitpython-led-animation-2.7.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_all_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_basic_animations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_blink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_chase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_customcolorchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_cycle_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_freeze_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_multicolor_comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_pixel_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_rainbow_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_resume_animation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_samd21_reset_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_sparkle_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_sparkle_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-26 16:10:47.000000 adafruit-circuitpython-led-animation-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:10:36.000000 adafruit-circuitpython-led-animation-2.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:10:55.413671 adafruit-circuitpython-led-animation-2.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.326182 adafruit-circuitpython-led-animation-2.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.314181 adafruit-circuitpython-led-animation-2.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.314181 adafruit-circuitpython-led-animation-2.7.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.314181 adafruit-circuitpython-led-animation-2.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.318181 adafruit-circuitpython-led-animation-2.7.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-08-07 01:08:26.326182 adafruit-circuitpython-led-animation-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.318181 adafruit-circuitpython-led-animation-2.7.3/adafruit_circuitpython_led_animation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-08-07 01:08:26.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_circuitpython_led_animation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-07 01:08:26.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_circuitpython_led_animation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 01:08:26.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_circuitpython_led_animation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 01:08:26.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_circuitpython_led_animation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 01:08:26.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_circuitpython_led_animation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.318181 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.322182 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/blink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/chase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/colorcycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/customcolorchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/grid_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/multicolor_comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/rainbowchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/rainbowcomet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/rainbowsparkle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/solid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/sparkle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/sparklepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/timedsequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.322182 adafruit-circuitpython-led-animation-2.7.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.322182 adafruit-circuitpython-led-animation-2.7.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:08:26.326182 adafruit-circuitpython-led-animation-2.7.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_all_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_basic_animations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_blink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_chase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_customcolorchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_cycle_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_freeze_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_multicolor_comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_pixel_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_rainbow_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_resume_animation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_samd21_reset_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_sparkle_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_sparkle_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_timedsequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-07 01:08:17.000000 adafruit-circuitpython-led-animation-2.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-07 01:08:07.000000 adafruit-circuitpython-led-animation-2.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 01:08:26.326182 adafruit-circuitpython-led-animation-2.7.3/setup.cfg
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-led-animation-2.7.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/.gitignore` & `adafruit-circuitpython-led-animation-2.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/.pre-commit-config.yaml` & `adafruit-circuitpython-led-animation-2.7.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/.pylintrc` & `adafruit-circuitpython-led-animation-2.7.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-led-animation-2.7.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/LICENSE` & `adafruit-circuitpython-led-animation-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-led-animation-2.7.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/LICENSES/MIT.txt` & `adafruit-circuitpython-led-animation-2.7.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-led-animation-2.7.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/PKG-INFO` & `adafruit-circuitpython-led-animation-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-led-animation
-Version: 2.7.2
+Version: 2.7.3
 Summary: CircuitPython helper for LED colors and animations.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation
 Keywords: adafruit,blinka,circuitpython,micropython,led,animation,led,colors,animations
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/README.rst` & `adafruit-circuitpython-led-animation-2.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_circuitpython_led_animation.egg-info/PKG-INFO` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_circuitpython_led_animation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-led-animation
-Version: 2.7.2
+Version: 2.7.3
 Summary: CircuitPython helper for LED colors and animations.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation
 Keywords: adafruit,blinka,circuitpython,micropython,led,animation,led,colors,animations
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_circuitpython_led_animation.egg-info/SOURCES.txt` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_circuitpython_led_animation.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 adafruit_circuitpython_led_animation.egg-info/top_level.txt
 adafruit_led_animation/__init__.py
 adafruit_led_animation/color.py
 adafruit_led_animation/grid.py
 adafruit_led_animation/group.py
 adafruit_led_animation/helper.py
 adafruit_led_animation/sequence.py
+adafruit_led_animation/timedsequence.py
 adafruit_led_animation/animation/__init__.py
 adafruit_led_animation/animation/blink.py
 adafruit_led_animation/animation/chase.py
 adafruit_led_animation/animation/colorcycle.py
 adafruit_led_animation/animation/comet.py
 adafruit_led_animation/animation/customcolorchase.py
 adafruit_led_animation/animation/grid_rain.py
@@ -40,14 +41,15 @@
 adafruit_led_animation/animation/rainbow.py
 adafruit_led_animation/animation/rainbowchase.py
 adafruit_led_animation/animation/rainbowcomet.py
 adafruit_led_animation/animation/rainbowsparkle.py
 adafruit_led_animation/animation/solid.py
 adafruit_led_animation/animation/sparkle.py
 adafruit_led_animation/animation/sparklepulse.py
+adafruit_led_animation/animation/volume.py
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
@@ -67,8 +69,10 @@
 examples/led_animation_pixel_map.py
 examples/led_animation_rainbow_animations.py
 examples/led_animation_resume_animation.py
 examples/led_animation_samd21_reset_interval.py
 examples/led_animation_sequence.py
 examples/led_animation_simpletest.py
 examples/led_animation_sparkle_animations.py
-examples/led_animation_sparkle_mask.py
+examples/led_animation_sparkle_mask.py
+examples/led_animation_timedsequence.py
+examples/led_animation_volume.py
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/__init__.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/__init__.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
-__version__ = "2.7.2"
+__version__ = "2.7.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 from adafruit_led_animation import MS_PER_SECOND, monotonic_ms
 
 
 class Animation:
     # pylint: disable=too-many-instance-attributes
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/blink.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/blink.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/chase.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/chase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/colorcycle.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/colorcycle.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/comet.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/comet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/customcolorchase.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/customcolorchase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/grid_rain.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/grid_rain.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   https://circuitpython.org/downloads
 
 """
 
 import random
 from adafruit_led_animation.animation import Animation
 
-__version__ = "2.7.2"
+__version__ = "2.7.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 from adafruit_led_animation.color import BLACK, colorwheel, calculate_intensity, GREEN
 
 
 class Rain(Animation):
     """
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/multicolor_comet.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/multicolor_comet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/pulse.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/pulse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/rainbow.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/rainbow.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 """
 
 from adafruit_led_animation.animation import Animation
 from adafruit_led_animation.color import BLACK, colorwheel
 from adafruit_led_animation import MS_PER_SECOND, monotonic_ms
 
-__version__ = "2.7.2"
+__version__ = "2.7.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 
 class Rainbow(Animation):
     """
     The classic rainbow color wheel.
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/rainbowchase.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/rainbowchase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/rainbowcomet.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/rainbowcomet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/rainbowsparkle.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/rainbowsparkle.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/solid.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/solid.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/sparkle.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/sparkle.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   https://circuitpython.org/downloads
 
 """
 
 import random
 from adafruit_led_animation.animation import Animation
 
-__version__ = "2.7.2"
+__version__ = "2.7.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 
 class Sparkle(Animation):
     """
     Sparkle animation of a single color.
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/animation/sparklepulse.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/animation/sparklepulse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/color.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/color.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/grid.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/grid.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/group.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
-__version__ = "2.7.2"
+__version__ = "2.7.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 from adafruit_led_animation.animation import Animation
 
 
 class AnimationGroup:
     """
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/helper.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/helper.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/adafruit_led_animation/sequence.py` & `adafruit-circuitpython-led-animation-2.7.3/adafruit_led_animation/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 """
 
 import random
 from adafruit_led_animation.color import BLACK
 from . import MS_PER_SECOND, monotonic_ms
 
-__version__ = "2.7.2"
+__version__ = "2.7.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 
 class AnimationSequence:
     """
     A sequence of Animations to run in succession, looping forever.
     Advances manually, or at the specified interval.
```

### Comparing `adafruit-circuitpython-led-animation-2.7.2/docs/_static/favicon.ico` & `adafruit-circuitpython-led-animation-2.7.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/docs/api.rst` & `adafruit-circuitpython-led-animation-2.7.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/docs/conf.py` & `adafruit-circuitpython-led-animation-2.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/docs/examples.rst` & `adafruit-circuitpython-led-animation-2.7.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/docs/index.rst` & `adafruit-circuitpython-led-animation-2.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_all_animations.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_all_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_basic_animations.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_basic_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_blink.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_blink.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_chase.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_chase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_comet.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_comet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_customcolorchase.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_customcolorchase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_cycle_animations.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_cycle_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_freeze_animation.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_freeze_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_group.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_group.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_multicolor_comet.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_multicolor_comet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_pixel_map.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_pixel_map.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_rainbow_animations.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_rainbow_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_resume_animation.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_resume_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_samd21_reset_interval.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_samd21_reset_interval.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_sequence.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_sequence.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_simpletest.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_sparkle_animations.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_sparkle_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/examples/led_animation_sparkle_mask.py` & `adafruit-circuitpython-led-animation-2.7.3/examples/led_animation_sparkle_mask.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.2/pyproject.toml` & `adafruit-circuitpython-led-animation-2.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-led-animation"
 description = "CircuitPython helper for LED colors and animations."
-version = "2.7.2"
+version = "2.7.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation"}
 keywords = [
     "adafruit",
```

