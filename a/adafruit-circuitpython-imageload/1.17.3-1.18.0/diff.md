# Comparing `tmp/adafruit-circuitpython-imageload-1.17.3.tar.gz` & `tmp/adafruit-circuitpython-imageload-1.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-imageload-1.17.3.tar", last modified: Fri May 26 16:23:35 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-imageload-1.18.0.tar", last modified: Mon Aug  7 16:18:48 2023, max compression
```

## Comparing `adafruit-circuitpython-imageload-1.17.3.tar` & `adafruit-circuitpython-imageload-1.18.0.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.762229 adafruit-circuitpython-imageload-1.17.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.726227 adafruit-circuitpython-imageload-1.17.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.734227 adafruit-circuitpython-imageload-1.17.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:23:14.000000 adafruit-circuitpython-imageload-1.17.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.734227 adafruit-circuitpython-imageload-1.17.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:23:14.000000 adafruit-circuitpython-imageload-1.17.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.734227 adafruit-circuitpython-imageload-1.17.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-26 16:23:35.762229 adafruit-circuitpython-imageload-1.17.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.738227 adafruit-circuitpython-imageload-1.17.3/adafruit_circuitpython_imageload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-26 16:23:35.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_circuitpython_imageload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-26 16:23:35.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_circuitpython_imageload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:23:35.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_circuitpython_imageload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 16:23:35.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_circuitpython_imageload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 16:23:35.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_circuitpython_imageload.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.738227 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.738227 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/bmp/
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/bmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10096 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/bmp/indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/bmp/negative_height_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/displayio_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/png.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.738227 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pbm_ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pbm_binary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.742227 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pgm/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pgm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pgm/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pgm/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/ppm_ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/ppm_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/tilegrid_inflator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.746228 adafruit-circuitpython-imageload-1.17.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.746228 adafruit-circuitpython-imageload-1.17.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/developing.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.746228 adafruit-circuitpython-imageload-1.17.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/examples/imageload_colorwheel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/examples/imageload_from_web.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/examples/imageload_magtag_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/examples/imageload_netpbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/examples/imageload_png_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/examples/imageload_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/examples/imageload_tilegrid_inflator_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.754228 adafruit-circuitpython-imageload-1.17.3/examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/1bit-not-byte-aligned.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/1bit-not-byte-aligned.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/1bit.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/1bit.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/2bit.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/2bit.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/4bit.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/4bit.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/4bit_rle.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/4bit_rle.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/8bit_rle.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/8bit_rle.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/castle_spritesheet.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/castle_spritesheet.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)    77880 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/color_wheel.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/color_wheel.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/color_wheel_rle.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/color_wheel_rle.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/magtag_2x2_test.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/magtag_2x2_test.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p1_mono_ascii.pbm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p1_mono_ascii.pbm.license
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p2_ascii.pgm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p2_ascii.pgm.license
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p3_rgb_ascii.ppm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p3_rgb_ascii.ppm.license
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p4_mono_binary.pbm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p4_mono_binary.pbm.license
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p4_mono_large.pbm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p4_mono_large.pbm.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p5_binary.pgm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p5_binary.pgm.license
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p6_binary.ppm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p6_binary.ppm.license
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/test_image.png
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/examples/images/test_image.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:23:35.762229 adafruit-circuitpython-imageload-1.17.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:35.762229 adafruit-circuitpython-imageload-1.17.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/tests/__init__.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/tests/displayio_shared_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/tests/displayio_shared_bindings.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_bitmap_c_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_bitmap_c_interface.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_bmp_indexed_load.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_bmp_indexed_load.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_palette_c_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_palette_c_interface.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_pbm_load.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_pbm_load.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_pgm_load.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_pgm_load.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-26 16:23:26.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_ppm_load.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:23:15.000000 adafruit-circuitpython-imageload-1.17.3/tests/test_ppm_load.py.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.749859 adafruit-circuitpython-imageload-1.18.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.725859 adafruit-circuitpython-imageload-1.18.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.729859 adafruit-circuitpython-imageload-1.18.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.729859 adafruit-circuitpython-imageload-1.18.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.729859 adafruit-circuitpython-imageload-1.18.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-07 16:18:48.749859 adafruit-circuitpython-imageload-1.18.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.729859 adafruit-circuitpython-imageload-1.18.0/adafruit_circuitpython_imageload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-07 16:18:48.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_circuitpython_imageload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-08-07 16:18:48.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_circuitpython_imageload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:18:48.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_circuitpython_imageload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 16:18:48.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_circuitpython_imageload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 16:18:48.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_circuitpython_imageload.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.733859 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.733859 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/bmp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2908 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/bmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10096 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/bmp/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/bmp/negative_height_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3321 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/bmp/truecolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/displayio_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/png.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.733859 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pbm_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pbm_binary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.733859 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pgm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pgm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pgm/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pgm/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/ppm_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/ppm_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/tilegrid_inflator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.737859 adafruit-circuitpython-imageload-1.18.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.737859 adafruit-circuitpython-imageload-1.18.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/developing.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.737859 adafruit-circuitpython-imageload-1.18.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/examples/imageload_colorwheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/examples/imageload_from_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/examples/imageload_magtag_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/examples/imageload_netpbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/examples/imageload_png_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/examples/imageload_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/examples/imageload_tilegrid_inflator_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.745859 adafruit-circuitpython-imageload-1.18.0/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/1bit-not-byte-aligned.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/1bit-not-byte-aligned.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/1bit.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/1bit.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/2bit.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/2bit.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/4bit.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/4bit.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/4bit_rle.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/4bit_rle.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/8bit_rle.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/8bit_rle.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/castle_spritesheet.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/castle_spritesheet.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)    77880 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/color_wheel.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/color_wheel.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/color_wheel_rle.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/color_wheel_rle.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/magtag_2x2_test.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/magtag_2x2_test.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p1_mono_ascii.pbm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p1_mono_ascii.pbm.license
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p2_ascii.pgm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p2_ascii.pgm.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p3_rgb_ascii.ppm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p3_rgb_ascii.ppm.license
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p4_mono_binary.pbm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p4_mono_binary.pbm.license
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p4_mono_large.pbm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p4_mono_large.pbm.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p5_binary.pgm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p5_binary.pgm.license
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p6_binary.ppm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p6_binary.ppm.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/test_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/examples/images/test_image.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:18:48.749859 adafruit-circuitpython-imageload-1.18.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:18:48.749859 adafruit-circuitpython-imageload-1.18.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/tests/__init__.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/tests/displayio_shared_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/tests/displayio_shared_bindings.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_bitmap_c_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_bitmap_c_interface.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_bmp_indexed_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_bmp_indexed_load.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_palette_c_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_palette_c_interface.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_pbm_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_pbm_load.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_pgm_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_pgm_load.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-07 16:18:39.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_ppm_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 16:18:28.000000 adafruit-circuitpython-imageload-1.18.0/tests/test_ppm_load.py.license
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-imageload-1.18.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/.gitignore` & `adafruit-circuitpython-imageload-1.18.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/.pre-commit-config.yaml` & `adafruit-circuitpython-imageload-1.18.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/.pylintrc` & `adafruit-circuitpython-imageload-1.18.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-imageload-1.18.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/LICENSE` & `adafruit-circuitpython-imageload-1.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-imageload-1.18.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/LICENSES/MIT.txt` & `adafruit-circuitpython-imageload-1.18.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-imageload-1.18.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/PKG-INFO` & `adafruit-circuitpython-imageload-1.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-imageload
-Version: 1.17.3
+Version: 1.18.0
 Summary: Displays text using CircuitPython's displayio.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad
 Keywords: adafruit,blinka,circuitpython,micropython,bitmap,fonts,text,display,tft,lcd,displayio,imageload,image
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/README.rst` & `adafruit-circuitpython-imageload-1.18.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_circuitpython_imageload.egg-info/PKG-INFO` & `adafruit-circuitpython-imageload-1.18.0/adafruit_circuitpython_imageload.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-imageload
-Version: 1.17.3
+Version: 1.18.0
 Summary: Displays text using CircuitPython's displayio.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad
 Keywords: adafruit,blinka,circuitpython,micropython,bitmap,fonts,text,display,tft,lcd,displayio,imageload,image
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_circuitpython_imageload.egg-info/SOURCES.txt` & `adafruit-circuitpython-imageload-1.18.0/adafruit_circuitpython_imageload.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 adafruit_imageload/displayio_types.py
 adafruit_imageload/gif.py
 adafruit_imageload/png.py
 adafruit_imageload/tilegrid_inflator.py
 adafruit_imageload/bmp/__init__.py
 adafruit_imageload/bmp/indexed.py
 adafruit_imageload/bmp/negative_height_check.py
+adafruit_imageload/bmp/truecolor.py
 adafruit_imageload/pnm/__init__.py
 adafruit_imageload/pnm/pbm_ascii.py
 adafruit_imageload/pnm/pbm_binary.py
 adafruit_imageload/pnm/ppm_ascii.py
 adafruit_imageload/pnm/ppm_binary.py
 adafruit_imageload/pnm/pgm/__init__.py
 adafruit_imageload/pnm/pgm/ascii.py
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/__init__.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     )
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from .displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file_or_filename: Union[str, BufferedReader],
     *,
     bitmap: Optional[BitmapConstructor] = None,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/bmp/__init__.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/bmp/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from typing import Tuple, Optional, Set, List
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from ..displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     *,
     bitmap: Optional[BitmapConstructor] = None,
@@ -58,20 +58,28 @@
     file.seek(0x1C)  # Number of bits per pixel
     color_depth = int.from_bytes(file.read(2), "little")
     file.seek(0x1E)  # Compression type
     compression = int.from_bytes(file.read(2), "little")
     file.seek(0x2E)  # Number of colors in the color palette
     colors = int.from_bytes(file.read(4), "little")
 
-    if colors == 0 and color_depth >= 16:
-        raise NotImplementedError("True color BMP unsupported")
-
     if compression > 2:
         raise NotImplementedError("bitmask compression unsupported")
 
+    if colors == 0 and color_depth >= 16:
+        from . import truecolor
+
+        return truecolor.load(
+            file,
+            _width,
+            _height,
+            data_start,
+            color_depth,
+            bitmap=bitmap,
+        )
     if colors == 0:
         colors = 2**color_depth
     from . import indexed
 
     return indexed.load(
         file,
         _width,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/bmp/indexed.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/bmp/indexed.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 try:
     from bitmaptools import readinto as _bitmap_readinto
 except ImportError:
     _bitmap_readinto = None  # pylint: disable=invalid-name  # type: Callable
 
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/displayio_types.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/displayio_types.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,9 +18,9 @@
     from displayio import Palette, Bitmap
 
     PaletteConstructor = Callable[[int], Palette]
     BitmapConstructor = Callable[[int, int, int], Bitmap]
 except ImportError:
     pass
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/gif.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/gif.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from typing import Tuple, Iterator, Optional, List
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from .displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     *,
     bitmap: BitmapConstructor,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/png.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/png.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/__init__.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     )
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from ..displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     header: bytes,
     *,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pbm_ascii.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pbm_ascii.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 try:
     from typing import Tuple, Optional
     from io import BufferedReader
     from displayio import Palette, Bitmap
 except ImportError:
     pass
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pbm_binary.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pbm_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 try:
     from typing import Tuple, Optional, Iterator
     from io import BufferedReader
     from displayio import Palette, Bitmap
 except ImportError:
     pass
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pgm/__init__.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pgm/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pgm/ascii.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pgm/ascii.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/pgm/binary.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/pgm/binary.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/ppm_ascii.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/ppm_ascii.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Load pixel values (indices or colors) into a bitmap and for an ascii ppm,
 return None for pallet.
 
 * Author(s):  Matt Land, Brooke Storm, Sam McGahan
 
 """
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 try:
     from typing import (
         Tuple,
         Iterator,
         Optional,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/pnm/ppm_binary.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/pnm/ppm_binary.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     from typing import Tuple, Optional, Set
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from ..displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/adafruit_imageload/tilegrid_inflator.py` & `adafruit-circuitpython-imageload-1.18.0/adafruit_imageload/tilegrid_inflator.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 try:
     from typing import Tuple, Optional, List, Union
     from displayio import Palette, Bitmap, OnDiskBitmap, TileGrid
 except ImportError:
     pass
 
-__version__ = "1.17.3"
+__version__ = "1.18.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def inflate_tilegrid(
     bmp_path: Optional[str] = None,
     target_size: Tuple[int, int] = (3, 3),
     tile_size: Optional[List[int]] = None,
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/docs/_static/favicon.ico` & `adafruit-circuitpython-imageload-1.18.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/docs/api.rst` & `adafruit-circuitpython-imageload-1.18.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/docs/conf.py` & `adafruit-circuitpython-imageload-1.18.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/docs/developing.rst` & `adafruit-circuitpython-imageload-1.18.0/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/docs/examples.rst` & `adafruit-circuitpython-imageload-1.18.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/docs/index.rst` & `adafruit-circuitpython-imageload-1.18.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/imageload_from_web.py` & `adafruit-circuitpython-imageload-1.18.0/examples/imageload_from_web.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/imageload_magtag_simpletest.py` & `adafruit-circuitpython-imageload-1.18.0/examples/imageload_magtag_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/imageload_netpbm.py` & `adafruit-circuitpython-imageload-1.18.0/examples/imageload_netpbm.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/imageload_png_simpletest.py` & `adafruit-circuitpython-imageload-1.18.0/examples/imageload_png_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/1bit-not-byte-aligned.bmp` & `adafruit-circuitpython-imageload-1.18.0/examples/images/1bit-not-byte-aligned.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/8bit_rle.bmp` & `adafruit-circuitpython-imageload-1.18.0/examples/images/8bit_rle.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/castle_spritesheet.bmp` & `adafruit-circuitpython-imageload-1.18.0/examples/images/castle_spritesheet.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/color_wheel.bmp` & `adafruit-circuitpython-imageload-1.18.0/examples/images/color_wheel.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/color_wheel_rle.bmp` & `adafruit-circuitpython-imageload-1.18.0/examples/images/color_wheel_rle.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/magtag_2x2_test.bmp` & `adafruit-circuitpython-imageload-1.18.0/examples/images/magtag_2x2_test.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p1_mono_ascii.pbm` & `adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p1_mono_ascii.pbm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p3_rgb_ascii.ppm` & `adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p3_rgb_ascii.ppm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p4_mono_large.pbm` & `adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p4_mono_large.pbm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/netpbm_p6_binary.ppm` & `adafruit-circuitpython-imageload-1.18.0/examples/images/netpbm_p6_binary.ppm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/examples/images/test_image.png` & `adafruit-circuitpython-imageload-1.18.0/examples/images/test_image.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/pyproject.toml` & `adafruit-circuitpython-imageload-1.18.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-imageload"
 description = "Displays text using CircuitPython's displayio."
-version = "1.17.3"
+version = "1.18.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-imageload-1.17.3/tests/__init__.py` & `adafruit-circuitpython-imageload-1.18.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/tests/displayio_shared_bindings.py` & `adafruit-circuitpython-imageload-1.18.0/tests/displayio_shared_bindings.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/tests/test_bitmap_c_interface.py` & `adafruit-circuitpython-imageload-1.18.0/tests/test_bitmap_c_interface.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/tests/test_bmp_indexed_load.py` & `adafruit-circuitpython-imageload-1.18.0/tests/test_bmp_indexed_load.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/tests/test_palette_c_interface.py` & `adafruit-circuitpython-imageload-1.18.0/tests/test_palette_c_interface.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/tests/test_pbm_load.py` & `adafruit-circuitpython-imageload-1.18.0/tests/test_pbm_load.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/tests/test_pgm_load.py` & `adafruit-circuitpython-imageload-1.18.0/tests/test_pgm_load.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.3/tests/test_ppm_load.py` & `adafruit-circuitpython-imageload-1.18.0/tests/test_ppm_load.py`

 * *Files identical despite different names*

