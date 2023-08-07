# Comparing `tmp/gnssrefl-1.4.6.tar.gz` & `tmp/gnssrefl-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.4.6.tar", last modified: Thu Aug  3 18:58:11 2023, max compression
+gzip compressed data, was "gnssrefl-1.4.8.tar", last modified: Mon Aug  7 19:18:53 2023, max compression
```

## Comparing `gnssrefl-1.4.6.tar` & `gnssrefl-1.4.8.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:58:11.422471 gnssrefl-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 18:57:53.000000 gnssrefl-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 18:57:53.000000 gnssrefl-1.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-03 18:58:11.422471 gnssrefl-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-03 18:57:53.000000 gnssrefl-1.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:58:11.398471 gnssrefl-1.4.6/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:58:11.398471 gnssrefl-1.4.6/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_qld.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35040 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   183744 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/make_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/nyquist_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:58:11.398471 gnssrefl-1.4.6/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-03 18:58:11.000000 gnssrefl-1.4.6/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-03 18:58:11.000000 gnssrefl-1.4.6/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:58:11.000000 gnssrefl-1.4.6/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-03 18:58:11.000000 gnssrefl-1.4.6/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 18:58:11.000000 gnssrefl-1.4.6/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 18:58:11.000000 gnssrefl-1.4.6/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 18:58:11.422471 gnssrefl-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:58:11.422471 gnssrefl-1.4.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 18:57:54.000000 gnssrefl-1.4.6/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:53.028655 gnssrefl-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-07 19:18:53.028655 gnssrefl-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:53.004655 gnssrefl-1.4.8/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:53.008655 gnssrefl-1.4.8/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_qld.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35040 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   183744 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/make_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/nyquist_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:53.008655 gnssrefl-1.4.8/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-07 19:18:52.000000 gnssrefl-1.4.8/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-07 19:18:52.000000 gnssrefl-1.4.8/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:18:52.000000 gnssrefl-1.4.8/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-07 19:18:52.000000 gnssrefl-1.4.8/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 19:18:52.000000 gnssrefl-1.4.8/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 19:18:52.000000 gnssrefl-1.4.8/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:18:53.028655 gnssrefl-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:53.028655 gnssrefl-1.4.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 19:18:38.000000 gnssrefl-1.4.8/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.4.6/LICENSE` & `gnssrefl-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/PKG-INFO` & `gnssrefl-1.4.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.6
+Version: 1.4.8
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.4.6** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.8** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+
+August 7, 2023, again
 
 August 2, 2023: Updated azimuth outputs for gnssir and quickLook so that the azimuth of the 
 rising or setting part of the arc is reported rather than the average average, as was done in the older versions.
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
```

### Comparing `gnssrefl-1.4.6/README.md` & `gnssrefl-1.4.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # gnssrefl
 
-**github version: 1.4.6** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.8** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+
+August 7, 2023, again
 
 August 2, 2023: Updated azimuth outputs for gnssir and quickLook so that the azimuth of the 
 rising or setting part of the arc is reported rather than the average average, as was done in the older versions.
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
```

### Comparing `gnssrefl-1.4.6/gnssrefl/EGM96.py` & `gnssrefl-1.4.8/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/check_rinex_file.py` & `gnssrefl-1.4.8/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/computemp1mp2.py` & `gnssrefl-1.4.8/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/daily_avg.py` & `gnssrefl-1.4.8/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.4.8/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.4.8/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/decipher_argt.py` & `gnssrefl-1.4.8/gnssrefl/decipher_argt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_ioc.py` & `gnssrefl-1.4.8/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_noaa.py` & `gnssrefl-1.4.8/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_orbits.py` & `gnssrefl-1.4.8/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_psmsl.py` & `gnssrefl-1.4.8/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_qld.py` & `gnssrefl-1.4.8/gnssrefl/download_qld.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_rinex.py` & `gnssrefl-1.4.8/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_teqc.py` & `gnssrefl-1.4.8/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_tides.py` & `gnssrefl-1.4.8/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_unr.py` & `gnssrefl-1.4.8/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/download_wsv.py` & `gnssrefl-1.4.8/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/filesizes.py` & `gnssrefl-1.4.8/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gnssir.py` & `gnssrefl-1.4.8/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gnssir_cl.py` & `gnssrefl-1.4.8/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gnssir_input.py` & `gnssrefl-1.4.8/gnssrefl/gnssir_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gnssir_v2.py` & `gnssrefl-1.4.8/gnssrefl/gnssir_v2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gnsssnr.f` & `gnssrefl-1.4.8/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.4.8/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gps.py` & `gnssrefl-1.4.8/gnssrefl/gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gpssnr.f` & `gnssrefl-1.4.8/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gpsweek.py` & `gnssrefl-1.4.8/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.4.8/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/highrate.py` & `gnssrefl-1.4.8/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/installexe_cl.py` & `gnssrefl-1.4.8/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/invsnr_cl.py` & `gnssrefl-1.4.8/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/invsnr_input.py` & `gnssrefl-1.4.8/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/karnak_libraries.py` & `gnssrefl-1.4.8/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/kelly.py` & `gnssrefl-1.4.8/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/llh2xyz.py` & `gnssrefl-1.4.8/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/make_json_input.py` & `gnssrefl-1.4.8/gnssrefl/make_json_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/make_meta.py` & `gnssrefl-1.4.8/gnssrefl/make_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     parser.add_argument(
         "-lon",
         help="Longitude (deg), if station not in database",
         type=float,
         default=None,
     )
     parser.add_argument(
-        "-ht",
+        "-height",
         help="Ellipsoidal height (m) if station not in database",
         type=float,
         default=None,
     )
     parser.add_argument(
         "-read_offset",
         default=None,
@@ -67,15 +67,15 @@
     return {key: value for key, value in args.items() if value is not None}
 
 
 def make_meta(
     station: str,
     lat: float = None,
     lon: float = None,
-    ht: float = None,
+    height: float = None,
     man_input: bool = True,
     read_offset: bool = False,
     overwrite: bool = False,
 ):
     """
     Make a json file that includes equipment metadata information.
     It saves your inputs to a json file saved in REFL_CODE/input/<station>_meta.json.
@@ -92,15 +92,15 @@
 
     Examples
     --------
     make_meta p038
         makes json meta file for p038; uses UNR coords and will request user manually populate meta info.
         If meta json already exists for p038, will append to existing file.
 
-    make_meta test -lat 39.7417583 -lon -105.0706972 -ht 1655
+    make_meta test -lat 39.7417583 -lon -105.0706972 -height 1655
         makes json meta file for test; uses manually input coords and will request ueser manually populate meta info
 
     make_meta p038 -man_input False -read_offset True -overwrite True
         makes json meta file for p038; uses UNR coords, will not request user manually populate meta info but will
         extract available meta info from GAGE offset file.
         Will overwrite any existing meta json file for p038
 
@@ -111,15 +111,15 @@
 
     lat : float, optional
         latitude in deg
 
     lon : float, optional
         longitude in deg
 
-    ht : float, optional
+    height : float, optional
         ellipsoidal height in m
 
     read_offset : bool, optional
         set to True to parse GAGE offset file. default is False.
 
     man_input : bool, optional
         set to True to manually input equipment metadata. default is True.
@@ -142,76 +142,77 @@
     # If no overwrite and a file already exists, read in existing meta json
     if (overwrite is False) and (os.path.isfile(outputfile)):
         with open(outputfile) as json_file:
             comp_dict = json.load(json_file)
             meta_dict = comp_dict["meta"]
 
     else:  # initialize empty meta_dict
-        comp_dict = get_coords(station, lat, lon, ht)
+        comp_dict = get_coords(station, lat, lon, height)
         meta_dict = {}
 
     # read in gage metadata file
     if read_offset:
         meta_dict = check_offsets(station, meta_dict)
 
     if man_input:
         meta_dict = meta_man_input(meta_dict)
 
     # sort by date
     meta_dict = collections.OrderedDict(sorted(meta_dict.items()))
 
     # add metad to complete dictionary
     comp_dict["meta"] = meta_dict
+    
+    print('writing meta json out to:', outputfile)
     with open(outputfile, "w+") as outfile:
         json.dump(comp_dict, outfile, indent=3)
 
-
-def get_coords(station, lat, lon, ht):
+def get_coords(station, lat, lon, height):
     """
     initializes metadata dictionary with lat lon ht keys, either from UNR database (default) or user entered
 
     Parameters
     ----------
     station : str
         4 character station ID.
 
     lat : float, optional, default is None
         latitude in deg
 
     lon : float, optional, default is None
         longitude in deg
 
-    ht : float, optional, default is None
+    height : float, optional, default is None
         ellipsoidal height in m
 
     Returns
     ----------
     comp_dict : dict
         dictionary of metadata; keys 'lat','lon','ht' 'meta'.
 
     """
 
     if (lat is None) & (lon is None):
         # check the station coordinates in our database from the station name
-        lat, lon, ht = g.queryUNR_modern(station)
+        lat, lon, height = g.queryUNR_modern(station)
         if (lat == 0) and (lon == 0):
             print(
                 "Manually input coords using -lat -lon -ht args for make_meta. \n Exiting."
             )
             sys.exit()
         else:
-            print("Using inputs:", lat, lon, ht)
+            print("Using inputs:", lat, lon, height)
     else:
-        print("Using inputs:", lat, lon, ht)
+        print("Using inputs:", lat, lon, height)
 
     comp_dict = {
         "station": station,
         "lat": "{:.4f}".format(lat),
         "lon": "{:.4f}".format(lon),
-        "ht": "{:.4f}".format(ht),
+        "ht": "{:.4f}".format(height),
         "meta": {},
     }
     return comp_dict
 
 
 def meta_man_input(meta_dict):
     """
```

### Comparing `gnssrefl-1.4.6/gnssrefl/nmea2snr.py` & `gnssrefl-1.4.8/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.4.8/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/nyquist_cl.py` & `gnssrefl-1.4.8/gnssrefl/nyquist_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/nyquist_libs.py` & `gnssrefl-1.4.8/gnssrefl/nyquist_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/phase_functions.py` & `gnssrefl-1.4.8/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/prn2gps.py` & `gnssrefl-1.4.8/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/query_unr.py` & `gnssrefl-1.4.8/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/quickLook_cl.py` & `gnssrefl-1.4.8/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/quickLook_function.py` & `gnssrefl-1.4.8/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/quickLook_function2.py` & `gnssrefl-1.4.8/gnssrefl/quickLook_function2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/quickPhase.py` & `gnssrefl-1.4.8/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/quicklib.py` & `gnssrefl-1.4.8/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/quickplt.py` & `gnssrefl-1.4.8/gnssrefl/quickplt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/read_snr_files.py` & `gnssrefl-1.4.8/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/refl_zones.py` & `gnssrefl-1.4.8/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.4.8/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/refraction.py` & `gnssrefl-1.4.8/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/rh_plot.py` & `gnssrefl-1.4.8/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/rinex2snr.py` & `gnssrefl-1.4.8/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.4.8/gnssrefl/rinex2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.4.8/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/rinex3_snr.py` & `gnssrefl-1.4.8/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/rinpy.py` & `gnssrefl-1.4.8/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.4.8/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/smoosh.py` & `gnssrefl-1.4.8/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/smoosh_snr.py` & `gnssrefl-1.4.8/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/snow_functions.py` & `gnssrefl-1.4.8/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.4.8/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/spline_functions.py` & `gnssrefl-1.4.8/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/subdaily.py` & `gnssrefl-1.4.8/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/subdaily_cl.py` & `gnssrefl-1.4.8/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/utils.py` & `gnssrefl-1.4.8/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/veg_multiyr.py` & `gnssrefl-1.4.8/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/vwc.py` & `gnssrefl-1.4.8/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/vwc_cl.py` & `gnssrefl-1.4.8/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/vwc_input.py` & `gnssrefl-1.4.8/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/xnmeasnr.f` & `gnssrefl-1.4.8/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/xyz2llh.py` & `gnssrefl-1.4.8/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/ydoy.py` & `gnssrefl-1.4.8/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl/ymd.py` & `gnssrefl-1.4.8/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.4.8/gnssrefl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.6
+Version: 1.4.8
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.4.6** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.8** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+
+August 7, 2023, again
 
 August 2, 2023: Updated azimuth outputs for gnssir and quickLook so that the azimuth of the 
 rising or setting part of the arc is reported rather than the average average, as was done in the older versions.
 
 July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
 While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
 using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
```

### Comparing `gnssrefl-1.4.6/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.4.8/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.4.8/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/pyproject.toml` & `gnssrefl-1.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.6/setup.py` & `gnssrefl-1.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "progress",
     "astropy",
     "simplekml",
     "earthscope-sdk",
 ]
 setup(
     name="gnssrefl",
-    version="1.4.6",
+    version="1.4.8",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-1.4.6/test/test_gps.py` & `gnssrefl-1.4.8/test/test_gps.py`

 * *Files identical despite different names*

