# Comparing `tmp/PyProcar-6.0.0.tar.gz` & `tmp/PyProcar-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyProcar-6.0.0.tar", last modified: Sat Jun 10 16:58:20 2023, max compression
+gzip compressed data, was "PyProcar-6.1.0.tar", last modified: Mon Aug  7 06:55:51 2023, max compression
```

## Comparing `PyProcar-6.0.0.tar` & `PyProcar-6.1.0.tar`

### file list

```diff
@@ -1,110 +1,133 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.860260 PyProcar-6.0.0/
--rw-rw-rw-   0        0        0     1655 2023-05-08 12:33:46.000000 PyProcar-6.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0    43233 2023-05-08 12:33:46.000000 PyProcar-6.0.0/LICENSE
--rw-rw-rw-   0        0        0       62 2023-05-08 12:33:46.000000 PyProcar-6.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      674 2023-06-10 16:58:20.861262 PyProcar-6.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.733145 PyProcar-6.0.0/PyProcar.egg-info/
--rw-rw-rw-   0        0        0      674 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2785 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 16:58:20.000000 PyProcar-6.0.0/PyProcar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8913 2023-06-10 16:55:55.000000 PyProcar-6.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.736147 PyProcar-6.0.0/pyprocar/
--rw-rw-rw-   0        0        0     2507 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.755166 PyProcar-6.0.0/pyprocar/core/
--rw-rw-rw-   0        0        0      456 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/__init__.py
--rw-rw-rw-   0        0        0     4408 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/brillouin_zone.py
--rw-rw-rw-   0        0        0    12198 2023-05-25 16:01:56.000000 PyProcar-6.0.0/pyprocar/core/dos.py
--rw-rw-rw-   0        0        0    38748 2023-05-25 15:22:33.000000 PyProcar-6.0.0/pyprocar/core/ebs.py
--rw-rw-rw-   0        0        0    18179 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/fermisurface.py
--rw-rw-rw-   0        0        0    37312 2023-05-23 18:08:09.000000 PyProcar-6.0.0/pyprocar/core/fermisurface3D.py
--rw-rw-rw-   0        0        0    14082 2023-05-23 14:16:14.000000 PyProcar-6.0.0/pyprocar/core/isosurface.py
--rw-rw-rw-   0        0        0    10122 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/kpath.py
--rw-rw-rw-   0        0        0     8578 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarselect.py
--rw-rw-rw-   0        0        0     8712 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarsymmetry.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.762171 PyProcar-6.0.0/pyprocar/core/procarunfold/
--rw-rw-rw-   0        0        0       45 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/__init__.py
--rw-rw-rw-   0        0        0    24502 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/_bak.procarparser.py
--rw-rw-rw-   0        0        0     5383 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/fatband.py
--rw-rw-rw-   0        0        0     4532 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/procar_unfolder.py
--rw-rw-rw-   0        0        0     5154 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/procarunfold/unfolder.py
--rw-rw-rw-   0        0        0    15028 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/structure.py
--rw-rw-rw-   0        0        0    11039 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/core/surface.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.778186 PyProcar-6.0.0/pyprocar/io/
--rw-rw-rw-   0        0        0      885 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/__init__.py
--rw-rw-rw-   0        0        0    15461 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/abinit.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.781189 PyProcar-6.0.0/pyprocar/io/abinitparser/
--rw-rw-rw-   0        0        0       41 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/abinitparser/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/abinitparser/abinitparser.py
--rw-rw-rw-   0        0        0     5879 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/bxsf.py
--rw-rw-rw-   0        0        0    14822 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/elk.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.785192 PyProcar-6.0.0/pyprocar/io/elkparser/
--rw-rw-rw-   0        0        0       34 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/elkparser/__init__.py
--rw-rw-rw-   0        0        0    11433 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/elkparser/elkparser.py
--rw-rw-rw-   0        0        0     3124 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/frmsf.py
--rw-rw-rw-   0        0        0    33353 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobster.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.791198 PyProcar-6.0.0/pyprocar/io/lobsterparser/
--rw-rw-rw-   0        0        0      145 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobsterparser/__init__.py
--rw-rw-rw-   0        0        0    21053 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobsterparser/lobster_doscar_parser.py
--rw-rw-rw-   0        0        0    15675 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobsterparser/lobsterfermiparser.py
--rw-rw-rw-   0        0        0    15388 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/lobsterparser/lobsterparser.py
--rw-rw-rw-   0        0        0     6099 2023-05-23 13:49:31.000000 PyProcar-6.0.0/pyprocar/io/parser.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.794200 PyProcar-6.0.0/pyprocar/io/procarparser/
--rw-rw-rw-   0        0        0       74 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/procarparser/__init__.py
--rw-rw-rw-   0        0        0    31346 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/procarparser/procarparser.py
--rw-rw-rw-   0        0        0    44082 2023-05-25 18:06:53.000000 PyProcar-6.0.0/pyprocar/io/qe.py
--rw-rw-rw-   0        0        0     9911 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/siesta.py
--rw-rw-rw-   0        0        0    79901 2023-05-25 16:59:57.000000 PyProcar-6.0.0/pyprocar/io/vasp.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.797203 PyProcar-6.0.0/pyprocar/io/vaspxml/
--rw-rw-rw-   0        0        0       55 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/vaspxml/__init__.py
--rw-rw-rw-   0        0        0    25252 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/io/vaspxml/vaspxml.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.803208 PyProcar-6.0.0/pyprocar/plotter/
--rw-rw-rw-   0        0        0      123 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/plotter/__init__.py
--rw-rw-rw-   0        0        0    51559 2023-05-25 18:16:18.000000 PyProcar-6.0.0/pyprocar/plotter/dos_plot.py
--rw-rw-rw-   0        0        0    21401 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/plotter/ebs_plot.py
--rw-rw-rw-   0        0        0    14084 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/plotter/procarplot.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.838240 PyProcar-6.0.0/pyprocar/scripts/
--rw-rw-rw-   0        0        0      744 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/depreciated_scriptVector.py
--rw-rw-rw-   0        0        0     1552 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptBandGap.py
--rw-rw-rw-   0        0        0     9000 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptBandsDosplot.py
--rw-rw-rw-   0        0        0     8223 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptBandsplot.py
--rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptBandsplot_2d.py
--rw-rw-rw-   0        0        0    10120 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptCat.py
--rw-rw-rw-   0        0        0    17304 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptDosplot.py
--rw-rw-rw-   0        0        0    11769 2023-05-25 19:52:39.000000 PyProcar-6.0.0/pyprocar/scripts/scriptFermi2D.py
--rw-rw-rw-   0        0        0    33276 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptFermi3D.py
--rw-rw-rw-   0        0        0    90799 2023-05-25 16:53:05.000000 PyProcar-6.0.0/pyprocar/scripts/scriptFermiHandler.py
--rw-rw-rw-   0        0        0     3238 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptFilter.py
--rw-rw-rw-   0        0        0     1333 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptKmesh2D.py
--rw-rw-rw-   0        0        0     3977 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptKpath.py
--rw-rw-rw-   0        0        0      526 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptRepair.py
--rw-rw-rw-   0        0        0     7841 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptSpin_asymmetry.py
--rw-rw-rw-   0        0        0    11385 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptUnfold.py
--rw-rw-rw-   0        0        0    25137 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptUnfold_new.py
--rw-rw-rw-   0        0        0     2986 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptUnfold_old.py
--rw-rw-rw-   0        0        0     6675 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptUnfold_v2.py
--rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/scripts/scriptVector.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.857258 PyProcar-6.0.0/pyprocar/utils/
--rw-rw-rw-   0        0        0      273 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/__init__.py
--rw-rw-rw-   0        0        0     1738 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/default_settings.ini
--rw-rw-rw-   0        0        0     3183 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/defaults.py
--rw-rw-rw-   0        0        0     5433 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/download_examples.py
--rw-rw-rw-   0        0        0     4891 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/elements.py
--rw-rw-rw-   0        0        0     2403 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/info.py
--rw-rw-rw-   0        0        0     2038 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/mathematics.py
--rw-rw-rw-   0        0        0    18332 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/procarfilefilter.py
--rw-rw-rw-   0        0        0    28441 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/scriptFermi3D.py
--rw-rw-rw-   0        0        0      403 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/sorting.py
--rw-rw-rw-   0        0        0      975 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/splash.py
--rw-rw-rw-   0        0        0     6062 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/unfolder.py
--rw-rw-rw-   0        0        0    10954 2023-05-08 12:33:47.000000 PyProcar-6.0.0/pyprocar/utils/utilsprocar.py
--rw-rw-rw-   0        0        0      688 2023-06-10 16:58:19.000000 PyProcar-6.0.0/pyprocar/version.py
--rw-rw-rw-   0        0        0       81 2023-05-08 12:33:47.000000 PyProcar-6.0.0/requirements.txt
--rw-rw-rw-   0        0        0     1740 2023-05-08 12:33:47.000000 PyProcar-6.0.0/requirements_docs.txt
-drwxrwxrwx   0        0        0        0 2023-06-10 16:58:20.859259 PyProcar-6.0.0/scripts/
--rw-rw-rw-   0        0        0    33462 2023-05-08 12:33:47.000000 PyProcar-6.0.0/scripts/procar.py
--rw-rw-rw-   0        0        0       86 2023-06-10 16:58:20.866266 PyProcar-6.0.0/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-05-23 14:24:52.000000 PyProcar-6.0.0/setup.json
--rw-rw-rw-   0        0        0     1590 2023-05-23 14:48:41.000000 PyProcar-6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.730232 PyProcar-6.1.0/
+-rw-rw-rw-   0        0        0     1655 2023-05-08 12:33:46.000000 PyProcar-6.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0    43233 2023-05-08 12:33:46.000000 PyProcar-6.1.0/LICENSE
+-rw-rw-rw-   0        0        0       62 2023-05-08 12:33:46.000000 PyProcar-6.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      633 2023-08-07 06:55:51.731232 PyProcar-6.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.570087 PyProcar-6.1.0/PyProcar.egg-info/
+-rw-rw-rw-   0        0        0      633 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3477 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9896 2023-08-07 06:48:50.000000 PyProcar-6.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.575090 PyProcar-6.1.0/pyprocar/
+-rw-rw-rw-   0        0        0     2531 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.593107 PyProcar-6.1.0/pyprocar/core/
+-rw-rw-rw-   0        0        0      520 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/__init__.py
+-rw-rw-rw-   0        0        0    11350 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/bandstructure2D.py
+-rw-rw-rw-   0        0        0     7424 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/brillouin_zone.py
+-rw-rw-rw-   0        0        0    12198 2023-05-25 16:01:56.000000 PyProcar-6.1.0/pyprocar/core/dos.py
+-rw-rw-rw-   0        0        0    46780 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/ebs.py
+-rw-rw-rw-   0        0        0    19863 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/fermisurface.py
+-rw-rw-rw-   0        0        0    14186 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/fermisurface3D.py
+-rw-rw-rw-   0        0        0    14086 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/isosurface.py
+-rw-rw-rw-   0        0        0    10122 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/kpath.py
+-rw-rw-rw-   0        0        0     8578 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarselect.py
+-rw-rw-rw-   0        0        0     8712 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarsymmetry.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.603115 PyProcar-6.1.0/pyprocar/core/procarunfold/
+-rw-rw-rw-   0        0        0       45 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/__init__.py
+-rw-rw-rw-   0        0        0    24502 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/_bak.procarparser.py
+-rw-rw-rw-   0        0        0     5383 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/fatband.py
+-rw-rw-rw-   0        0        0     4532 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/procar_unfolder.py
+-rw-rw-rw-   0        0        0     5154 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/unfolder.py
+-rw-rw-rw-   0        0        0    15028 2023-07-02 20:40:25.000000 PyProcar-6.1.0/pyprocar/core/structure.py
+-rw-rw-rw-   0        0        0    11061 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/surface.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.619131 PyProcar-6.1.0/pyprocar/io/
+-rw-rw-rw-   0        0        0      904 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/io/__init__.py
+-rw-rw-rw-   0        0        0    21922 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/io/abinit.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.623134 PyProcar-6.1.0/pyprocar/io/abinitparser/
+-rw-rw-rw-   0        0        0       41 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/abinitparser/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/abinitparser/abinitparser.py
+-rw-rw-rw-   0        0        0     5879 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/bxsf.py
+-rw-rw-rw-   0        0        0    14822 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/elk.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.626137 PyProcar-6.1.0/pyprocar/io/elkparser/
+-rw-rw-rw-   0        0        0       34 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/elkparser/__init__.py
+-rw-rw-rw-   0        0        0    11433 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/elkparser/elkparser.py
+-rw-rw-rw-   0        0        0     3124 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/frmsf.py
+-rw-rw-rw-   0        0        0    33353 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobster.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.632142 PyProcar-6.1.0/pyprocar/io/lobsterparser/
+-rw-rw-rw-   0        0        0      145 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobsterparser/__init__.py
+-rw-rw-rw-   0        0        0    21053 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobsterparser/lobster_doscar_parser.py
+-rw-rw-rw-   0        0        0    15675 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobsterparser/lobsterfermiparser.py
+-rw-rw-rw-   0        0        0    15388 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobsterparser/lobsterparser.py
+-rw-rw-rw-   0        0        0     7146 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/io/parser.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.635145 PyProcar-6.1.0/pyprocar/io/procarparser/
+-rw-rw-rw-   0        0        0       74 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/procarparser/__init__.py
+-rw-rw-rw-   0        0        0    31346 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/procarparser/procarparser.py
+-rw-rw-rw-   0        0        0    44082 2023-05-25 18:06:53.000000 PyProcar-6.1.0/pyprocar/io/qe.py
+-rw-rw-rw-   0        0        0     9911 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/siesta.py
+-rw-rw-rw-   0        0        0    81939 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/io/vasp.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.638147 PyProcar-6.1.0/pyprocar/io/vaspxml/
+-rw-rw-rw-   0        0        0       55 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/vaspxml/__init__.py
+-rw-rw-rw-   0        0        0    25252 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/vaspxml/vaspxml.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.648157 PyProcar-6.1.0/pyprocar/plotter/
+-rw-rw-rw-   0        0        0      259 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/__init__.py
+-rw-rw-rw-   0        0        0    24628 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/bs_2d_plot.py
+-rw-rw-rw-   0        0        0    51396 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/dos_plot.py
+-rw-rw-rw-   0        0        0    21705 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/ebs_plot.py
+-rw-rw-rw-   0        0        0    45163 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/fermi3d_plot.py
+-rw-rw-rw-   0        0        0    14084 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/plotter/procarplot.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.677184 PyProcar-6.1.0/pyprocar/pyposcar/
+-rw-rw-rw-   0        0        0      177 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/__init__.py
+-rw-rw-rw-   0        0        0     1425 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/analize.py
+-rw-rw-rw-   0        0        0    19751 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/chg_raw.py
+-rw-rw-rw-   0        0        0    11407 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/clusters.py
+-rw-rw-rw-   0        0        0      961 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/db.py
+-rw-rw-rw-   0        0        0     4077 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/dbCovalentBond.py
+-rw-rw-rw-   0        0        0    14105 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/defects.py
+-rw-rw-rw-   0        0        0      803 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/generalUtils.py
+-rw-rw-rw-   0        0        0    11870 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/honeycomb.py
+-rw-rw-rw-   0        0        0     6195 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/latticeUtils.py
+-rw-rw-rw-   0        0        0     1885 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/outcarParser.py
+-rw-rw-rw-   0        0        0     5191 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/plot3d.py
+-rw-rw-rw-   0        0        0     5647 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/plotbands.py
+-rw-rw-rw-   0        0        0    15418 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/poscar.py
+-rw-rw-rw-   0        0        0    27247 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/poscarUtils.py
+-rw-rw-rw-   0        0        0     7039 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/rdf.py
+-rw-rw-rw-   0        0        0    12574 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/relax-cell-2d.py
+-rw-rw-rw-   0        0        0      190 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/test.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.708212 PyProcar-6.1.0/pyprocar/scripts/
+-rw-rw-rw-   0        0        0      808 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/depreciated_scriptVector.py
+-rw-rw-rw-   0        0        0     1552 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandGap.py
+-rw-rw-rw-   0        0        0     6603 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandStructure2DHandler.py
+-rw-rw-rw-   0        0        0     8920 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandsDosplot.py
+-rw-rw-rw-   0        0        0     8610 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandsplot.py
+-rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandsplot_2d.py
+-rw-rw-rw-   0        0        0    10120 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptCat.py
+-rw-rw-rw-   0        0        0    13416 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptDosplot.py
+-rw-rw-rw-   0        0        0     8872 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptFermi2D.py
+-rw-rw-rw-   0        0        0    33281 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptFermi3D.py
+-rw-rw-rw-   0        0        0    13173 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptFermiHandler.py
+-rw-rw-rw-   0        0        0     3238 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptFilter.py
+-rw-rw-rw-   0        0        0     1333 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptKmesh2D.py
+-rw-rw-rw-   0        0        0     3977 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptKpath.py
+-rw-rw-rw-   0        0        0      526 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptRepair.py
+-rw-rw-rw-   0        0        0     7841 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptSpin_asymmetry.py
+-rw-rw-rw-   0        0        0    11385 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptUnfold.py
+-rw-rw-rw-   0        0        0    25137 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_new.py
+-rw-rw-rw-   0        0        0     2986 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_old.py
+-rw-rw-rw-   0        0        0     6675 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_v2.py
+-rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptVector.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.727229 PyProcar-6.1.0/pyprocar/utils/
+-rw-rw-rw-   0        0        0     1562 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1739 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/utils/default_settings.ini
+-rw-rw-rw-   0        0        0     3183 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/defaults.py
+-rw-rw-rw-   0        0        0     5790 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/utils/download_examples.py
+-rw-rw-rw-   0        0        0     4891 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/elements.py
+-rw-rw-rw-   0        0        0     2403 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/info.py
+-rw-rw-rw-   0        0        0     2994 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/utils/mathematics.py
+-rw-rw-rw-   0        0        0    18332 2023-08-06 22:53:59.000000 PyProcar-6.1.0/pyprocar/utils/procarfilefilter.py
+-rw-rw-rw-   0        0        0    28441 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/scriptFermi3D.py
+-rw-rw-rw-   0        0        0      403 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/sorting.py
+-rw-rw-rw-   0        0        0      975 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/splash.py
+-rw-rw-rw-   0        0        0     6062 2023-08-06 21:34:44.000000 PyProcar-6.1.0/pyprocar/utils/unfolder.py
+-rw-rw-rw-   0        0        0    10954 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/utilsprocar.py
+-rw-rw-rw-   0        0        0      688 2023-08-07 06:55:51.000000 PyProcar-6.1.0/pyprocar/version.py
+-rw-rw-rw-   0        0        0      103 2023-08-07 06:46:20.000000 PyProcar-6.1.0/requirements.txt
+-rw-rw-rw-   0        0        0      259 2023-08-07 06:55:41.000000 PyProcar-6.1.0/requirements_docs.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.729230 PyProcar-6.1.0/scripts/
+-rw-rw-rw-   0        0        0    33462 2023-05-08 12:33:47.000000 PyProcar-6.1.0/scripts/procar.py
+-rw-rw-rw-   0        0        0       86 2023-08-07 06:55:51.733234 PyProcar-6.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-08-07 06:53:31.000000 PyProcar-6.1.0/setup.json
+-rw-rw-rw-   0        0        0     1643 2023-08-07 06:46:20.000000 PyProcar-6.1.0/setup.py
```

### Comparing `PyProcar-6.0.0/AUTHORS.rst` & `PyProcar-6.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/LICENSE` & `PyProcar-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/PKG-INFO` & `PyProcar-6.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: PyProcar
-Version: 6.0.0
+Version: 6.1.0
 Summary: A Python library for electronic structure pre/post-processing. 
 Home-page: https://github.com/romerogroup/pyprocar
 Author: Francisco MuÃ±oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
 Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
 License: LICENSE
-Download-URL: https://github.com/romerogroup/pyprocar/archive/6.0.0.tar.gz
+Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.0.tar.gz
+Description: UNKNOWN
 Platform: UNKNOWN
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-UNKNOWN
-
```

### Comparing `PyProcar-6.0.0/PyProcar.egg-info/PKG-INFO` & `PyProcar-6.1.0/PyProcar.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: PyProcar
-Version: 6.0.0
+Version: 6.1.0
 Summary: A Python library for electronic structure pre/post-processing. 
 Home-page: https://github.com/romerogroup/pyprocar
 Author: Francisco MuÃ±oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
 Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
 License: LICENSE
-Download-URL: https://github.com/romerogroup/pyprocar/archive/6.0.0.tar.gz
+Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.0.tar.gz
+Description: UNKNOWN
 Platform: UNKNOWN
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-UNKNOWN
-
```

### Comparing `PyProcar-6.0.0/PyProcar.egg-info/SOURCES.txt` & `PyProcar-6.1.0/PyProcar.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 PyProcar.egg-info/SOURCES.txt
 PyProcar.egg-info/dependency_links.txt
 PyProcar.egg-info/requires.txt
 PyProcar.egg-info/top_level.txt
 pyprocar/__init__.py
 pyprocar/version.py
 pyprocar/core/__init__.py
+pyprocar/core/bandstructure2D.py
 pyprocar/core/brillouin_zone.py
 pyprocar/core/dos.py
 pyprocar/core/ebs.py
 pyprocar/core/fermisurface.py
 pyprocar/core/fermisurface3D.py
 pyprocar/core/isosurface.py
 pyprocar/core/kpath.py
@@ -50,20 +51,41 @@
 pyprocar/io/lobsterparser/lobsterfermiparser.py
 pyprocar/io/lobsterparser/lobsterparser.py
 pyprocar/io/procarparser/__init__.py
 pyprocar/io/procarparser/procarparser.py
 pyprocar/io/vaspxml/__init__.py
 pyprocar/io/vaspxml/vaspxml.py
 pyprocar/plotter/__init__.py
+pyprocar/plotter/bs_2d_plot.py
 pyprocar/plotter/dos_plot.py
 pyprocar/plotter/ebs_plot.py
+pyprocar/plotter/fermi3d_plot.py
 pyprocar/plotter/procarplot.py
+pyprocar/pyposcar/__init__.py
+pyprocar/pyposcar/analize.py
+pyprocar/pyposcar/chg_raw.py
+pyprocar/pyposcar/clusters.py
+pyprocar/pyposcar/db.py
+pyprocar/pyposcar/dbCovalentBond.py
+pyprocar/pyposcar/defects.py
+pyprocar/pyposcar/generalUtils.py
+pyprocar/pyposcar/honeycomb.py
+pyprocar/pyposcar/latticeUtils.py
+pyprocar/pyposcar/outcarParser.py
+pyprocar/pyposcar/plot3d.py
+pyprocar/pyposcar/plotbands.py
+pyprocar/pyposcar/poscar.py
+pyprocar/pyposcar/poscarUtils.py
+pyprocar/pyposcar/rdf.py
+pyprocar/pyposcar/relax-cell-2d.py
+pyprocar/pyposcar/test.py
 pyprocar/scripts/__init__.py
 pyprocar/scripts/depreciated_scriptVector.py
 pyprocar/scripts/scriptBandGap.py
+pyprocar/scripts/scriptBandStructure2DHandler.py
 pyprocar/scripts/scriptBandsDosplot.py
 pyprocar/scripts/scriptBandsplot.py
 pyprocar/scripts/scriptBandsplot_2d.py
 pyprocar/scripts/scriptCat.py
 pyprocar/scripts/scriptDosplot.py
 pyprocar/scripts/scriptFermi2D.py
 pyprocar/scripts/scriptFermi3D.py
```

### Comparing `PyProcar-6.0.0/README.md` & `PyProcar-6.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 [![PyPI version](https://badge.fury.io/py/pyprocar.svg)](https://badge.fury.io/py/pyprocar)
 [![conda-forge version](https://img.shields.io/conda/v/conda-forge/pyprocar.svg?label=conda-forge&colorB=027FD5)](https://anaconda.org/conda-forge/pyprocar)
 [![Build Status](https://travis-ci.org/romerogroup/pyprocar.svg?branch=master)](https://travis-ci.org/romerogroup/pyprocar)
 [![HitCount](http://hits.dwyl.com/uthpalaherath/romerogroup/pyprocar.svg)](http://hits.dwyl.com/uthpalaherath/romerogroup/pyprocar)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyprocar)
 
+Notice
+===========
+- **New Release** We recently updated to a new version 'v6.0.0'. This update encompasses a significant overhaul of the codebase and documentation.
+- **Support for Previous Versions**: For users who prefer to continue with an older version, we have conveniently archived the previous releases on GitHub, and provided a link to the corresponding documentation.
+
+
 PyProcar
 ===========
 
 PyProcar is a robust, open-source Python library used for pre- and post-processing of the electronic structure data coming from DFT calculations. PyProcar provides a set of functions that manage data obtained from the PROCAR format. Basically, the PROCAR format is a projection of the Kohn-Sham states over atomic orbitals. That projection is performed to every k-point in the considered mesh, every energy band and every atom. PyProcar is capable of performing a multitude of tasks including plotting plain and spin/atom/orbital projected band structures and Fermi surfaces- both in 2D and 3D, Fermi velocity plots, unfolding bands of a super  cell, comparing band structures from multiple DFT calculations, plotting partial density of states and generating a k-path for a given crystal structure.
 
 Currently supports:
 
@@ -18,16 +24,22 @@
 5. Lobster (Stll in development)
 
 ![](welcome.png)
 
 Documentation
 -------------
 
+For versions 6.1.0 and above, the documentation is found here:
 https://romerogroup.github.io/pyprocar/
 
+
+The prior documentation is found here:
+https://romerogroup.github.io/pyprocar5.6.6/
+
+
 Developers
 ------------
 Francisco Muñoz <br />
 Aldo Romero <br />
 Sobhit Singh <br />
 Uthpala Herath <br />
 Pedram Tavadze <br />
@@ -90,27 +102,33 @@
     conda install -c conda-forge pyprocar
 
 Usage
 -----
 Typical use is as follows
 
     import pyprocar
-    pyprocar.bandsplot('PROCAR',outcar='OUTCAR',mode='plain',code='vasp')
+    pyprocar.bandsplot(code='vasp',mode='plain', dirname='bands')
+
+Previously, bandsplot would accept the OUTCAR and PROCAR file paths as inputs,
+in v6.0.0 we moved to specifying the directory where the bands calculation took place.
 
 Refer to the documentation for further details.
 
 Stand-alone mode:
 
     procar.py -h
 
 will bring a help menu.
 
 Changelog
 --------------
-v6.0.0 May 6th, 2021 -- Directory changes. This version is not backwards compatible. <br />
+v6.1.0 Aug 7th, 2023 -- Bug fixes, doc update, config files <br />
+v6.0.0 Jun 10th, 2023 -- Major code base changes. <br />
+v5.6.6 Mar 6th, 2022 -- QE, bandsplot, dosplot, fermi surface, and band unfolding bug fixes. Directory change, parsers are now in the io directory. <br />
+v5.6.5 Jun 10th, 2021 -- Fermi surface object and fermi surface plotter bug fixes <br />
 v5.6.4 May 6th, 2021 -- Updates to Fermi surface plotter. <br />
 v5.6.3 Mar 5th, 2021 -- QE and elk bug fixes. <br />
 v5.6.2 Jan 11th, 2021 -- Updates and bugfixes to fermi surface and dos plotter. <br />
 v5.6.1 Dec 7th, 2020 -- Fixed bug in PyProcar.cat() for merging parallel Abinit files for spin polarized calculations. Converted units Ha to eV. <br />
 v5.6.0 Nov 30th, 2020 -- Repairs PROCAR file by default. Set flag repair=False to disable. <br />
 v5.5.8 Nov 24th, 2020 -- Updates to parametric band structure plotting. Ability to change linewidths with ``linewidth`` flag. <br />
 v5.4.4 Oct 23rd, 2020 -- Updates to DOS plotting, Fermi3D and bxsf parser and other bugfixes. <br />
```

### Comparing `PyProcar-6.0.0/pyprocar/__init__.py` & `PyProcar-6.1.0/pyprocar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 from .scripts import *
 from .io import *
 from . import io
 from . import core
 from . import utils
 from . import plotter
+from . import pyposcar
 from .utils.download_examples import download_examples, download_example, download_dev_data
 from .utils.defaults import Settings
 from .utils import welcome
 
 
 PROJECT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
```

### Comparing `PyProcar-6.0.0/pyprocar/core/dos.py` & `PyProcar-6.1.0/pyprocar/core/dos.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/core/ebs.py` & `PyProcar-6.1.0/pyprocar/core/ebs.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: Freddy Farah
 
 """
 
 # from . import Structure
 from typing import List
 import itertools
-
+import copy
 from scipy.interpolate import CubicSpline
 
 import numpy as np
 import networkx as nx
 from matplotlib import pylab as plt
 import pyvista
 
@@ -55,14 +55,17 @@
     """
 
     def __init__(
         self,
         kpoints:np.ndarray,
         bands:np.ndarray,
         efermi:float,
+        n_kx:int=None,
+        n_ky:int=None,
+        n_kz:int=None,
         projected:np.ndarray = None,
         projected_phase:np.ndarray =None,
         weights:np.ndarray=None,
         kpath:KPath=None,
         labels:List=None,
         reciprocal_lattice:np.ndarray=None,
         ):
@@ -80,59 +83,79 @@
             self.has_phase = True
         else:
             self.has_phase = False
         self.labels = labels
         self.weights = weights
         self.graph = None
 
+        self._n_kx=n_kx
+        self._n_ky=n_ky
+        self._n_kz=n_kz
         
+        self._index_mesh=None
+        self._kpoints_mesh=None
+        self._kpoints_cartesian_mesh=None
+        self._bands_mesh=None
+        self._projected_mesh=None
+        self._projected_phase_mesh=None
+        self._weights_mesh=None
+        self._bands_gradient_mesh=None
+        self._bands_hessian_mesh=None
+        self._fermi_velocity_mesh=None
+        self._harmonic_average_effective_mass_mesh=None
+        self._fermi_speed_mesh=None
+
+        self._bands_gradient=None
+        self._bands_hessian=None
+        self._fermi_velocity=None
+        self._effective_mass=None
+        self._fermi_speed=None
+        self._harmonic_average_effective_mass=None
         
-        self._index_mesh = None
-        self._kpoints_mesh = None
-        self._kpoints_cartesian_mesh = None
-        self._bands_mesh = None
-        self._projected_mesh = None
-        self._projected_phase_mesh = None
-        self._weights_mesh = None
-        self._bands_gradient_mesh = None
-        self._bands_hessian_mesh = None
 
             
     @property
     def n_kx(self):
         """The number of unique kpoints in kx direction in the reduced basis
 
         Returns
         -------
         int
             The number of unique kpoints in kx direction in the reduced basis
         """
-        return len( np.unique(self.kpoints[:,0]) )
+
+        if self._n_kx==None:
+            self._n_kx=len( np.unique(self.kpoints[:,0]) )
+        return self._n_kx
     
     @property
     def n_ky(self):
         """The number of unique kpoints in kx direction in the reduced basis
 
         Returns
         -------
         int
             The number of unique kpoints in kx direction in the reduced basis
         """
-        return len( np.unique(self.kpoints[:,1]) )
+        if self._n_ky==None:
+            self._n_ky=len( np.unique(self.kpoints[:,1]) )
+        return self._n_ky
     
     @property
     def n_kz(self):
         """The number of unique kpoints in ky direction in the reduced basis
 
         Returns
         -------
         int
             The number of unique kpoints in ky direction in the reduced basis
         """
-        return len( np.unique(self.kpoints[:,2]) )
+        if self._n_kz==None:
+            self._n_kz=len( np.unique(self.kpoints[:,2]) )
+        return self._n_kz
 
     @property
     def nkpoints(self):
         """The number of k points
 
         Returns
         -------
@@ -233,14 +256,106 @@
 
         Returns
         -------
         np.ndarray
             Returns the kpoints in fractional basis
         """
         return self.kpoints
+    
+    @property
+    def bands_gradient(self):
+        """
+        Bands gradient is a numpy array that stores each band gradient a list that corresponds to the self.kpoints
+        Shape = [n_kpoints,3,n_bands], where the second dimension represents d/dx,d/dy,d/dz  
+        
+        Returns
+        -------
+        np.ndarray
+            Bands fradient is a numpy array that stores each band gradient in a list that corresponds to the self.kpoints
+            Shape = [n_kpoints,3,n_bands], 
+            where the second dimension represents d/dx,d/dy,d/dz  
+        """
+
+        if self._bands_gradient is None:
+            self._bands_gradient = self.mesh_to_array(mesh=self.bands_gradient_mesh)
+        return self._bands_gradient
+    
+    @property
+    def bands_hessian(self):
+        """
+        Bands hessian is a numpy array that stores each band hessian in a list that corresponds to the self.kpoints   
+        Shape = [n_kpoints,3,3,n_bands], 
+        where the second and third dimension represent d/dx,d/dy,d/dz  
+        
+        Returns
+        -------
+        np.ndarray
+            Bands hessian is a numpy array that stores each band hessian in a list that corresponds to the self.kpoints
+            Shape = [n_kpoints,3,3,n_bands], 
+            where the second and third dimension represent d/dx,d/dy,d/dz  
+        """
+
+        if self._bands_hessian is None:
+            self._bands_hessian = self.mesh_to_array(mesh=self.bands_hessian_mesh)
+        return self._bands_hessian
+
+    @property
+    def fermi_velocity(self):
+        """
+        fermi_velocity is a numpy array that stores each fermi_velocity a list that corresponds to the self.kpoints
+        Shape = [n_kpoints,3,n_bands], where the second dimension represents d/dx,d/dy,d/dz  
+        
+        Returns
+        -------
+        np.ndarray
+            fermi_velocity is a numpy array that stores each fermi_velocity in a list that corresponds to the self.kpoints
+            Shape = [n_kpoints,3,n_bands], 
+            where the second dimension represents d/dx,d/dy,d/dz  
+        """
+
+        if self._fermi_velocity is None:
+            self._fermi_velocity = self.mesh_to_array(mesh=self.fermi_velocity_mesh)
+        return self._fermi_velocity
+    
+    @property
+    def fermi_speed(self):
+        """
+        fermi speed is a numpy array that stores each fermi speed a list that corresponds to the self.kpoints
+        Shape = [n_kpoints,n_bands] 
+        
+        Returns
+        -------
+        np.ndarray
+            fermi speed is a numpy array that stores each fermi speed 
+            in a list that corresponds to the self.kpoints
+            Shape = [n_kpoints,n_bands], 
+        """
+
+        if self._fermi_speed is None:
+            self._fermi_speed = self.mesh_to_array(mesh=self.fermi_speed_mesh)
+        return self._fermi_speed
+
+    @property
+    def harmonic_average_effective_mass(self):
+        """
+        harmonic average effective mass is a numpy array that stores 
+        each harmonic average effective mass in a list that corresponds to the self.kpoints   
+        Shape = [n_kpoints,n_bands], 
+        
+        Returns
+        -------
+        np.ndarray
+            harmonic average effective mass is a numpy array that stores 
+            each harmonic average effective mass in a list that corresponds to the self.kpoints
+            Shape = [n_kpoints,n_bands],
+        """
+
+        if self._harmonic_average_effective_mass is None:
+            self._harmonic_average_effective_mass=self.mesh_to_array(mesh=self.harmonic_average_effective_mass_mesh)
+        return self._harmonic_average_effective_mass
 
     @property
     def index_mesh(self):
         """
         Index mesh stores the the kpoints index in 
         kpoints list at a particular grid point . 
         Shape = [n_kx,n_ky,n_kz]
@@ -249,58 +364,84 @@
         -------
         np.ndarray
             Index mesh stores the the kpoints index in 
             kpoints list at a particular grid point .  Shape = [n_kx,n_ky,n_kz]
 
         """
         if self._index_mesh is None:
-            self.update_index_mesh()
+            kx_unique = np.unique(self.kpoints[:,0])
+            ky_unique = np.unique(self.kpoints[:,1])
+            kz_unique = np.unique(self.kpoints[:,2])
+            n_kx = len(kx_unique)
+            n_ky = len(ky_unique)
+            n_kz = len(kz_unique)
+            self._index_mesh = np.zeros((n_kx,n_ky,n_kz),dtype=int)
+
+            for k in range(n_kz):
+                for j in range(n_ky):
+                    for i in range(n_kx):
+
+                        kx = kx_unique[i]
+                        ky = ky_unique[j]
+                        kz = kz_unique[k]
+
+                        where_x_true_indices = np.where(self.kpoints[:,0] == kx)[0]
+                        where_x_true_points = self.kpoints[where_x_true_indices]
+
+                        where_xy_true_indices = np.where(where_x_true_points[:,1] == ky)[0]
+                        where_xy_true_points = where_x_true_points[where_xy_true_indices]
+
+                        where_xyz_true_indices = np.where(where_xy_true_points[:,2] == kz)[0]
+                        where_xyz_true_points = where_xy_true_points[where_xyz_true_indices]
+
+                        original_index = where_x_true_indices[where_xy_true_indices[where_xyz_true_indices]]
+                        # print(original_index)
+                        self._index_mesh[i,j,k] = original_index
         return self._index_mesh
     
     @property
     def kpoints_mesh(self):
         """Kpoint mesh representation of the kpoints grid. Shape = [3,n_kx,n_ky,n_kz]
         Returns
         -------
         np.ndarray
             Kpoint mesh representation of the kpoints grid. Shape = [3,n_kx,n_ky,n_kz]
         """
 
         if self._kpoints_mesh is None:
-            self.update_kpoints_mesh()
+            self._kpoints_mesh = self.create_nd_mesh(nd_list = self.kpoints)
         return self._kpoints_mesh
     
     @property
     def kpoints_cartesian_mesh(self):
         """Kpoint cartesian mesh representation of the kpoints grid. Shape = [3,n_kx,n_ky,n_kz]
         Returns
         -------
         np.ndarray
             Kpoint cartesian mesh representation of the kpoints grid. Shape = [3,n_kx,n_ky,n_kz]
         """
-
         if self._kpoints_cartesian_mesh is None:
-            self.update_kpoints_cartesian_mesh()
+            self._kpoints_cartesian_mesh = self.create_nd_mesh(nd_list = self.kpoints_cartesian)
         return self._kpoints_cartesian_mesh
     
     @property
-    def bands_mesh(self):
+    def bands_mesh(self,force_update=False):
         """
         Bands mesh is a numpy array that stores each band in a mesh grid.   
         Shape = [n_bands,n_kx,n_ky,n_kz]
 
         Returns
         -------
         np.ndarray
             Bands mesh is a numpy array that stores each band in a mesh grid. 
             Shape = [n_bands,n_kx,n_ky,n_kz]
         """
 
-        if self._bands_mesh is None:
-            self.update_bands_mesh()
+        if self._bands_mesh is None or force_update:
+            self._bands_mesh = self.create_nd_mesh(nd_list = self.bands)
         return self._bands_mesh
     
     @property
     def projected_mesh(self):
         """
         projected mesh is a numpy array that stores each projection in a mesh grid.   
         Shape = [n_bands,n_spins,n_atoms,n_orbitals,n_kx,n_ky,n_kz]
@@ -309,15 +450,15 @@
         -------
         np.ndarray
             Projection mesh is a numpy array that stores each projection in a mesh grid. 
             Shape = [n_bands,n_spins,n_atoms,n_orbitals,n_kx,n_ky,n_kz]
         """
 
         if self._projected_mesh is None:
-            self.update_projected_mesh()
+            self._projected_mesh = self.create_nd_mesh(nd_list = self.projected)
         return self._projected_mesh
     
     @property
     def projected_phase_mesh(self):
         """
         projected phase mesh is a numpy array that stores each projection phases in a mesh grid.   
         Shape = [n_bands,n_spins,n_atoms,n_orbitals,n_kx,n_ky,n_kz]
@@ -326,15 +467,15 @@
         -------
         np.ndarray
             projected phase mesh is a numpy array that stores each projection phases in a mesh grid.  
             Shape = [n_bands,n_spins,n_atoms,n_orbitals,n_kx,n_ky,n_kz]
         """
 
         if self._projected_phase_mesh is None:
-            self.update_projected_phase_mesh()
+            self._projected_phase_mesh = self.create_nd_mesh(nd_list = self.projected_phase)
         return self._projected_phase_mesh
 
     @property
     def weights_mesh(self):
         """
         weights mesh is a numpy array that stores each weights in a mesh grid.   
         Shape = [1,n_kx,n_ky,n_kz]
@@ -343,15 +484,15 @@
         -------
         np.ndarray
             weights mesh is a numpy array that stores each weights in a mesh grid. 
             Shape = [1,n_kx,n_ky,n_kz]
         """
 
         if self._weights_mesh is None:
-            self.update_weights_mesh()
+            self._weights_mesh = self.create_nd_mesh(nd_list = self.weights)
         return self._weights_mesh
 
     @property
     def bands_gradient_mesh(self):
         """
         Bands gradient mesh is a numpy array that stores each band gradient in a mesh grid.   
         Shape = [3,n_bands,n_kx,n_ky,n_kz], where the first dimension represents d/dx,d/dy,d/dz  
@@ -361,240 +502,198 @@
         np.ndarray
             Bands fradient mesh is a numpy array that stores each band gradient in a mesh grid.
             Shape = [3,n_bands,n_kx,n_ky,n_kz], 
             where the first dimension represents d/dx,d/dy,d/dz  
         """
 
         if self._bands_gradient_mesh is None:
-            self.update_bands_gradient_mesh()
+            n_bands, n_spins, n_i, n_j, n_k = self.bands_mesh.shape
+
+            band_gradients = np.zeros((3, n_bands, n_spins, n_i, n_j, n_k))
+
+            for i_band in range(n_bands):
+                for i_spin in range(n_spins):
+                    band_gradients[:,i_band,i_spin,:,:,:] = self.calculate_scalar_gradient(scalar_mesh = self.bands_mesh[i_band,i_spin,:,:,:])
+            
+            band_gradients *= METER_ANGSTROM
+            self._bands_gradient_mesh = band_gradients
         return self._bands_gradient_mesh
     
     @property
     def bands_hessian_mesh(self):
         """
         Bands hessian mesh is a numpy array that stores each band hessian in a mesh grid.   
-        Shape = [3,3,n_bands,n_kx,n_ky,n_kz], 
+        Shape = [3,3,n_bands,n_spin,n_kx,n_ky,n_kz], 
         where the first and second dimension represent d/dx,d/dy,d/dz  
         
         Returns
         -------
         np.ndarray
             Bands hessian mesh is a numpy array that stores each band hessian in a mesh grid.
-            Shape = [3,3,n_bands,n_kx,n_ky,n_kz], 
+            Shape = [3,3,n_bands,n_spin,n_kx,n_ky,n_kz], 
             where the first and second dimension represent d/dx,d/dy,d/dz  
         """
 
         if self._bands_hessian_mesh is None:
-            self.update_bands_hessian_mesh()
-        return self._bands_hessian_mesh
+            n_dim, n_bands, n_spins, n_i, n_j, n_k = self.bands_gradient_mesh.shape
 
-    def update_kpoints_mesh(self):
-        """This method will update the kpoints mesh representation
+            band_hessians = np.zeros((3, 3,n_bands, n_spins, n_i, n_j, n_k))
 
-        Returns
-        -------
-        np.ndarray
-            Updated the kpoints mesh
-        """
-        self._kpoints_mesh = self.create_nd_mesh(nd_list = self.kpoints)
-        return self._kpoints_mesh
-
-    def update_kpoints_cartesian_mesh(self):
-        """This method will update the kpoints mesh representation
-
-        Returns
-        -------
-        np.ndarray
-            Updated the kpoints mesh
-        """
-        self._kpoints_cartesian_mesh = self.create_nd_mesh(nd_list = self.kpoints_cartesian)
-        return self._kpoints_cartesian_mesh
+            for i_dim in range(n_dim):
+                for i_band in range(n_bands):
+                    for i_spin in range(n_spins):
+                        band_hessians[:,i_dim,i_band,i_spin,:,:,:] = self.calculate_scalar_gradient(scalar_mesh = self.bands_gradient_mesh[i_dim,i_band,i_spin,:,:,:])
+            
+            band_hessians *= METER_ANGSTROM
+            self._bands_hessian_mesh = band_hessians
+        return self._bands_hessian_mesh
     
-    def update_bands_mesh(self):
-        """This method will update the bands mesh representation
-
-        Returns
-        -------
-        np.ndarray
-            Updated the bands mesh
+    @property
+    def fermi_velocity_mesh(self):
         """
-        self._bands_mesh = self.create_nd_mesh(nd_list = self.bands)
-        return self._bands_mesh
-    
-    def update_projected_mesh(self):
-        """This method will update the projected mesh representation
-
+        Fermi Velocity mesh is a numpy array that stores each  Fermi Velocity in a mesh grid.   
+        Shape = [3,n_bands,n_kx,n_ky,n_kz], where the first dimension represents d/dx,d/dy,d/dz  
+        
         Returns
         -------
         np.ndarray
-            Updated the projected mesh
+            Fermi Velocity mesh is a numpy array that stores each  Fermi Velocity in a mesh grid.
+            Shape = [3,n_bands,n_kx,n_ky,n_kz], 
+            where the first dimension represents d/dx,d/dy,d/dz  
         """
-        self._projected_mesh = self.create_nd_mesh(nd_list = self.projected)
-        return self._projected_mesh
-    
-    def update_projected_phase_mesh(self):
-        """This method will update the projected phase mesh representation
 
-        Returns
-        -------
-        np.ndarray
-            Updated the projected_phase mesh
-        """
-        self._projected_phase_mesh = self.create_nd_mesh(nd_list = self.projected_phase)
-        return self._projected_phase_mesh
+        if self._fermi_velocity_mesh is None:
+            self._fermi_velocity_mesh =  self.bands_gradient_mesh / HBAR_EV
+        return self._fermi_velocity_mesh
     
-    def update_weights_mesh(self):
-        """This method will update the weights mesh representation
-
-        Returns
-        -------
-        np.ndarray
-            Updated the weights mesh
+    @property
+    def fermi_speed_mesh(self):
         """
-        self._weights_mesh = self.create_nd_mesh(nd_list = self.weights)
-        return self._weights_mesh
-
-    def update_bands_gradient_mesh(self):
-        """This method will update the bands_gradient mesh representation
-
+        Fermi speed mesh is a numpy array that stores each  Fermi Velocity in a mesh grid.   
+        Shape = [n_bands,n_kx,n_ky,n_kz],
+        
         Returns
         -------
         np.ndarray
-            Updated the bands_gradient
+            Fermi speed mesh is a numpy array that stores each  Fermi Velocity in a mesh grid.
+            Shape = [n_bands,n_kx,n_ky,n_kz], 
         """
-        n_bands, n_spins, n_i, n_j, n_k = self.bands_mesh.shape
 
-        band_gradients = np.zeros((3, n_bands, n_spins, n_i, n_j, n_k))
+        if self._fermi_speed_mesh is None:
+            n_grad_1, n_bands, n_spins, n_i, n_j, n_k = self.fermi_velocity_mesh.shape
 
-        for i_band in range(n_bands):
-            for i_spin in range(n_spins):
-                band_gradients[:,i_band,i_spin,:,:,:] = self.calculate_scalar_gradient(scalar_mesh = self.bands_mesh[i_band,i_spin,:,:,:])
-        
-        band_gradients /= HBAR_EV
-        band_gradients *= METER_ANGSTROM
-        self._bands_gradient_mesh = band_gradients
-        return self._bands_gradient_mesh
+            self._fermi_speed_mesh = np.zeros(shape=(n_bands, n_spins, n_i, n_j, n_k))
+            for iband in range(n_bands):
+                for ispin in range(n_spins):
+                    for k in range(n_k):
+                        for j in range(n_j):
+                            for i in range(n_i):
+                                self._fermi_speed_mesh[iband,ispin,i,j,k] =  np.linalg.norm(self.fermi_velocity_mesh[:,iband,ispin,i,j,k])
+        return self._fermi_speed_mesh
     
-    def update_bands_hessian_mesh(self):
-        """This method will update the bands_hessian mesh representation
-
-        Returns
-        -------
-        np.ndarray
-            Updated the bands_hessian
+    @property
+    def harmonic_average_effective_mass_mesh(self):
         """
-        n_dim, n_bands, n_spins, n_i, n_j, n_k = self.bands_gradient_mesh.shape
-
-        band_hessians = np.zeros((3, 3,n_bands, n_spins, n_i, n_j, n_k))
-
-        for i_dim in range(n_dim):
-            for i_band in range(n_bands):
-                for i_spin in range(n_spins):
-                    band_hessians[:,i_dim,i_band,i_spin,:,:,:] = self.calculate_scalar_gradient(scalar_mesh = self.bands_gradient_mesh[i_dim,i_band,i_spin,:,:,:])
+        harmonic average effective mass mesh is a numpy array that stores each 
+        harmonic average effective mass mesh in a mesh grid.   
+        Shape = [n_bands,n_kx,n_ky,n_kz], 
         
-        band_hessians *= METER_ANGSTROM
-        self._bands_hessian_mesh = band_hessians
-        return self._bands_hessian_mesh
-
-    def update_index_mesh(self):
-        """This method will update the index mesh
-
         Returns
         -------
         np.ndarray
-            Updated the kpoints mesh
-        """
-
-        kx_unique = np.unique(self.kpoints[:,0])
-        ky_unique = np.unique(self.kpoints[:,1])
-        kz_unique = np.unique(self.kpoints[:,2])
-
-        n_kx = len(kx_unique)
-        n_ky = len(ky_unique)
-        n_kz = len(kz_unique)
-
-        self._index_mesh = np.zeros((n_kx,n_ky,n_kz),dtype=int)
-
-        for k in range(n_kz):
-            for j in range(n_ky):
-                for i in range(n_kx):
-
-                    kx = kx_unique[i]
-                    ky = ky_unique[j]
-                    kz = kz_unique[k]
-
-                    where_x_true_indices = np.where(self.kpoints[:,0] == kx)[0]
-                    where_x_true_points = self.kpoints[where_x_true_indices]
-
-                    where_xy_true_indices = np.where(where_x_true_points[:,1] == ky)[0]
-                    where_xy_true_points = where_x_true_points[where_xy_true_indices]
-
-                    where_xyz_true_indices = np.where(where_xy_true_points[:,2] == kz)[0]
-                    where_xyz_true_points = where_xy_true_points[where_xyz_true_indices]
-
-                    original_index = where_x_true_indices[where_xy_true_indices[where_xyz_true_indices]]
-
-                    self._index_mesh[i,j,k] = original_index
-
-        return self._index_mesh
-        
+            harmonic average effective mass mesh is a numpy array that stores 
+            each harmonic average effective mass in a mesh grid.
+            Shape = [n_bands,n_kx,n_ky,n_kz], 
+        """
+
+        if self._harmonic_average_effective_mass_mesh is None:
+            n_grad_1,n_grad_2, n_bands, n_spins, n_i, n_j, n_k = self.bands_hessian_mesh.shape
+
+            self._harmonic_average_effective_mass_mesh = np.zeros(shape=(n_bands, n_spins, n_i, n_j, n_k))
+
+            for iband in range(n_bands):
+                for ispin in range(n_spins):
+                    for k in range(n_k):
+                        for j in range(n_j):
+                            for i in range(n_i):
+                                hessian = self.bands_hessian_mesh[...,iband,ispin,i,j,k] * EV_TO_J/ HBAR_J**2
+                                self._harmonic_average_effective_mass_mesh[iband,ispin,i,j,k] = harmonic_average_effective_mass(hessian)
+        return self._harmonic_average_effective_mass_mesh
+    
     def calculate_scalar_gradient(self,scalar_mesh):
         """Calculates the scalar gradient over the k mesh grid in cartesian coordinates
 
         Parameters
         ----------
         scalar_mesh : np.ndarray
             The scalar mesh. shape = [n_kx,n_ky,n_kz]
 
         Returns
         -------
         np.ndarray
             scalar_gradient_mesh shape = [3,n_kx,n_ky,n_kz]
         """
-        nx,ny,nz = self.n_kx,self.n_ky,self.n_kz
-
-        scalar_gradients =  np.zeros((3,nx,ny,nz))
+        n_kx=len(np.unique(self.kpoints[:,0]))
+        n_ky=len(np.unique(self.kpoints[:,1]))
+        n_kz=len(np.unique(self.kpoints[:,2]))
+        scalar_gradients =  np.zeros((3,n_kx,n_ky,n_kz))
 
         # Calculate cartesian separations along each crystal direction
-        sep_vectors_i = np.abs(self.kpoints_cartesian[self.index_mesh[[0]*nx, :, :], :] - self.kpoints_cartesian[self.index_mesh[[1]*nx, :, :], :])
-        sep_vectors_j = np.abs(self.kpoints_cartesian[self.index_mesh[:, [0]*ny, :], :] - self.kpoints_cartesian[self.index_mesh[:, [1]*ny, :], :])
-        sep_vectors_k = np.abs(self.kpoints_cartesian[self.index_mesh[:, :, [0]*nz], :] - self.kpoints_cartesian[self.index_mesh[:, :, [1]*nz], :])
+        sep_vectors_i = np.abs(self.kpoints_cartesian[self.index_mesh[[0]*n_kx, :, :], :] - self.kpoints_cartesian[self.index_mesh[[1]*n_kx, :, :], :])
+        sep_vectors_j = np.abs(self.kpoints_cartesian[self.index_mesh[:, [0]*n_ky, :], :] - self.kpoints_cartesian[self.index_mesh[:, [1]*n_ky, :], :])
+
+        if n_kz>1:
+            sep_vectors_k = np.abs(self.kpoints_cartesian[self.index_mesh[:, :, [0]*n_kz], :] - self.kpoints_cartesian[self.index_mesh[:, :, [1]*n_kz], :])
+        else:
+            sep_vectors_k=copy.copy(sep_vectors_j)
+            sep_vectors_k[:,:,:,:]=0
 
         # Calculate indices with periodic boundary conditions
-        plus_one_indices_x = np.arange(nx) + 1
-        plus_one_indices_y = np.arange(ny) + 1
-        plus_one_indices_z = np.arange(nz) + 1
-
-        minus_one_indices_x = np.arange(nx) - 1
-        minus_one_indices_y = np.arange(ny) - 1
-        minus_one_indices_z = np.arange(nz) - 1
+        plus_one_indices_x = np.arange(n_kx) + 1
+        plus_one_indices_y = np.arange(n_ky) + 1
+        plus_one_indices_z = np.arange(n_kz) + 1
+
+        minus_one_indices_x = np.arange(n_kx) - 1
+        minus_one_indices_y = np.arange(n_ky) - 1
+        minus_one_indices_z = np.arange(n_kz) - 1
 
         plus_one_indices_x[-1] = 0
         plus_one_indices_y[-1] = 0
         plus_one_indices_z[-1] = 0
 
-        minus_one_indices_x[0] = nx - 1
-        minus_one_indices_y[0] = ny - 1
-        minus_one_indices_z[0] = nz - 1
+        minus_one_indices_x[0] = n_kx - 1
+        minus_one_indices_y[0] = n_ky - 1
+        minus_one_indices_z[0] = n_kz - 1
 
         scalar_diffs_i = scalar_mesh[plus_one_indices_x,:,:] - scalar_mesh[minus_one_indices_x,:,:]
         scalar_diffs_j = scalar_mesh[:,plus_one_indices_y,:] - scalar_mesh[:,minus_one_indices_y,:]
         scalar_diffs_k = scalar_mesh[:,:,plus_one_indices_z] - scalar_mesh[:,:,minus_one_indices_z]
         
         # Calculating gradients
         sep_vectors = [sep_vectors_i,sep_vectors_j,sep_vectors_k]
         energy_diffs = [scalar_diffs_i,scalar_diffs_j,scalar_diffs_k]
+
+        # Calculate gradients
+        # sep_vectors = [sep_vectors_i,sep_vectors_j]
+        # energy_diffs = [scalar_diffs_i,scalar_diffs_j]
+        # if n_kz > 1:  # Only add sep_vectors_k and scalar_diffs_k in 3D
+        #     sep_vectors.append(sep_vectors_k)
+        #     energy_diffs.append(scalar_diffs_k)
+
         for sep_vector,energy_diff in zip(sep_vectors,energy_diffs):
             for i_coord in range(3):
                 
                 dx = sep_vector[:, :, :, i_coord]
                 tmp_grad = energy_diff / (2 * dx)
                 # Changing infinities to 0
                 tmp_grad = np.nan_to_num(tmp_grad, neginf=0,posinf=0) 
                 scalar_gradients[i_coord, :, :, :] += tmp_grad
+
+        if n_kz == 1:
+            scalar_gradients[2,:,:,:]=0
         return scalar_gradients
     
     def calculate_scalar_integral(self,scalar_mesh):
         """Calculate the scalar integral"""
 
 
         edge1 = abs(self.kpoints_cartesian[self.index_mesh[1, 0, 0], :] - self.kpoints_cartesian[self.index_mesh[0, 0, 0], :])
@@ -613,25 +712,29 @@
         return integral
 
     def create_nd_mesh(self, nd_list):
 
         if nd_list is not  None:
 
             nd_shape = list(nd_list.shape[1:])
-            nd_shape.append(self.n_kx)
-            nd_shape.append(self.n_ky)
-            nd_shape.append(self.n_kz)
 
+
+            n_kx=len(np.unique(self.kpoints[:,0]))
+            n_ky=len(np.unique(self.kpoints[:,1]))
+            n_kz=len(np.unique(self.kpoints[:,2]))
+            nd_shape.append(n_kx)
+            nd_shape.append(n_ky)
+            nd_shape.append(n_kz)
             nd_mesh = np.zeros(nd_shape,dtype=nd_list.dtype)
             non_grid_dims = nd_shape[:-3]
             for i_dim, non_grid_dim in enumerate(non_grid_dims):
                 for i in range(non_grid_dim):
-                    for x in range(self.n_kx):
-                        for y in range(self.n_ky):
-                            for z in range(self.n_kz):
+                    for x in range(n_kx):
+                        for y in range(n_ky):
+                            for z in range(n_kz):
                                 # Forming slicing tuples for mesh
                                 mesh_idx = [ np.s_[:]]*nd_mesh.ndim
                                 mesh_idx[i_dim] = i
                                 mesh_idx[-3] = x
                                 mesh_idx[-2] = y
                                 mesh_idx[-1] = z
 
@@ -653,14 +756,38 @@
         return vector_mesh
     
     def create_scaler_mesh(self, scalar_list):
         scalar_mesh = np.zeros((1,self.n_kx,self.n_ky,self.n_kz),dtype=float)
         scalar_mesh[0,:,:,:]= scalar_list[ self.index_mesh ]
         return scalar_mesh
 
+    def mesh_to_array(self, mesh):
+        """
+        Converts a mesh to a list that corresponds to ebs.kpoints  
+
+        Parameters
+        ----------
+        mesh : np.ndarray
+            The mesh to convert to a list
+        Returns
+        -------
+        np.ndarray
+           lsit
+        """
+        nkx, nky, nkz = mesh.shape[-3:]
+        tmp_shape=[nkx*nky*nkz]
+        tmp_shape.extend(mesh.shape[:-3])
+        tmp_array=np.zeros(shape=tmp_shape)
+        for k in range(nkz):
+            for j in range(nky):
+                for i in range(nkx):
+                    index=self.index_mesh[i,j,k]
+                    tmp_array[index,...]=mesh[...,i,j,k]
+        return tmp_array
+
     def ebs_sum(self, 
                 atoms:List[int]=None, 
                 principal_q_numbers:List[int]=[-1], 
                 orbitals:List[int]=None, 
                 spins:List[int]=None, 
                 sum_noncolinear:bool=True):
         """_summary_
@@ -701,30 +828,14 @@
         # in non-mag, non-colin nspin=1, in colin nspin=2
         if self.is_non_collinear and sum_noncolinear:
             ret = np.sum(ret[:, :, spins], axis=-1).reshape(
                 self.nkpoints, self.nbands, 1
             )
         return ret
 
-    def update_weights(self, weights):
-        """Updates the weights corresponding to the kpoints
-
-        Parameters
-        ----------
-        weights : List[float]
-            A list of weights corresponding to the kpoints
-
-        Returns
-        -------
-        None
-            None
-        """
-        self.weights = weights
-        return None
-
     def unfold(self, transformation_matrix=None, structure=None):
         """The method helps unfold the bands. This is done by using the unfolder to find the new kpoint weights.
         The current weights are then updated
 
         Parameters
         ----------
         transformation_matrix : np.ndarray, optional
@@ -833,76 +944,116 @@
 
         Parameters
         ----------
         rotations : np.ndarray
             The point symmetry operations of the lattice
         """
         
-        klist = []
-        plist = []
-        bandslist = []
-        weights=[]
-        projected_phases=[]
+        full_kpoints=[]
+        full_projected=[]
+        full_bands=[]
+        full_weights=[]
+        full_projected_phases=[]
 
+        # Used for indexing full_kpoints
+        ik=0
         # for each symmetry operation
         for i, rotation in enumerate(rotations):
             # for each point
             for j, kpoint in enumerate(self.kpoints):
                 # apply symmetry operation to kpoint
-
                 
-                sympoint_vector = rotation.dot(kpoint)
+                new_kp = rotation.dot(kpoint)
                 # apply boundary conditions
-                bound_ops = -1.0*(sympoint_vector > 0.5) + 1.0*(sympoint_vector <= -0.5)
-                sympoint_vector += bound_ops
-
-                sympoint_vector=np.around(sympoint_vector,decimals=6)
-                sympoint = sympoint_vector.tolist()
-
-                if sympoint not in klist:
-                    klist.append(sympoint)
+                new_kp = -np.fmod(new_kp + 6.5, 1 ) + 0.5
+                new_kp = np.around(new_kp,decimals=6)
+                new_kp=new_kp.tolist()
+                if new_kp not in full_kpoints:
+                    full_kpoints.append(new_kp)
                     if self.bands is not None:
                         band = self.bands[j].tolist()
-                        bandslist.append(band)
+                        full_bands.append(band)
                     if self.projected is not None:
                         projection = self.projected[j].tolist()
-                        plist.append(projection)
+                        full_projected.append(projection)
                     if self.weights is not None:
                         weight = self.weights[j].tolist()
-                        weights.append(weight)
-                    if self.weights is not None:
-                        weight = self.weights[j].tolist()
-                        weights.append(weight)
+                        full_weights.append(weight)
                     if self.projected_phase is not None:
                         projected_phase = self.projected_phase[j].tolist()
-                        projected_phases.append(projected_phase)
-
-        self.kpoints = np.array(klist)
-        self.bands = np.array(bandslist)
+                        full_projected_phases.append(projected_phase)
+        self.kpoints = np.array(full_kpoints)
+        self.bands = np.array(full_bands)
 
         if self.projected is not None:
-            self.projected = np.array(plist)
+            self.projected = np.array(full_projected)
         if self.projected_phase is not None:
-            self.projected_phase = np.array(projected_phases)
+            self.projected_phase = np.array(full_projected_phases)
         if self.weights is not None:
-            self.weights = np.array(weights)
-        # self.sort_bands_and_kpoints()
+            self.weights = np.array(full_weights)
 
+        nk=self.kpoints.shape[0]
+        if self.n_kx:
+            if nk != self.n_kx*self.n_ky*self.n_kz:
+
+                err_text="""
+                        nkpoints != n_kx*n_ky*n_kz
+                        Error trying to symmetrize the irreducible kmesh. 
+                        This is issue is most likely related to 
+                        how the DFT code using symmetry operations to reduce the kmesh.
+                        Check the recommendations for k-mesh type for the crystal system.
+                        If all else fails turn off symmetry.
+                        """
+                raise ValueError(err_text)
+
+    def interpolate_mesh_grid(self, mesh_grid,interpolation_factor=2):
+        """This function will interpolate an Nd, 3d mesh grid
+        [...,nx,ny,nz]
 
-        
+        Parameters
+        ----------
+        mesh_grid : np.ndarray
+            The mesh grid to interpolate
+        """
+        scalar_dims=mesh_grid.shape[:-3]
+        new_mesh=None
+        for i, idx in enumerate(np.ndindex(scalar_dims)):
+            # Creating slicing list. idx are the scalar dimensions, last 3 are the grid
+            mesh_idx = list(idx)
+            tmp = [slice(None)]*3
+            mesh_idx.extend(tmp)
+            new_grid = mathematics.fft_interpolate(mesh_grid[mesh_idx], interpolation_factor=interpolation_factor)
+            
+            if i==0:
+                new_dim = np.append(scalar_dims,new_grid.shape,axis=0)
+                new_mesh=np.zeros(shape=(new_dim))
+
+            new_mesh[mesh_idx]=new_grid
+        return new_mesh
+    
+    def ravel_array(self,mesh_grid):
+        shape = mesh_grid.shape
+        mesh_grid=mesh_grid.reshape(shape[:-3] + (-1,))
+        mesh_grid=np.moveaxis(mesh_grid,-1,0)
+        return mesh_grid
 
     def __str__(self):
         ret = 'Enectronic Band Structure     \n'
         ret += '------------------------     \n'
         ret += 'Total number of kpoints  = {}\n'.format(self.nkpoints)
         ret += 'Total number of bands    = {}\n'.format(self.nbands)
         ret += 'Total number of atoms    = {}\n'.format(self.natoms)
         ret += 'Total number of orbitals = {}\n'.format(self.norbitals)
         return ret
-        
+
+def harmonic_average_effective_mass(tensor):
+    inv_effective_mass_tensor = tensor
+    e_mass = 3*(inv_effective_mass_tensor[0,0] + inv_effective_mass_tensor[1,1] + inv_effective_mass_tensor[2,2])**-1 /FREE_ELECTRON_MASS
+    return e_mass
+
     # def reorder(self, plot=True, cutoff=0.2):
     #     nspins = self.nspins
     #     if self.is_non_collinear:
     #         nspins = 1
     #         # projected = np.sum(self.projected, axis=-1).reshape(self.nkpoints,
     #         #                                                     self.nbands,
     #         #                                                     self.natoms,
```

### Comparing `PyProcar-6.0.0/pyprocar/core/isosurface.py` & `PyProcar-6.1.0/pyprocar/core/isosurface.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
                 verts[:, ix] *= self.dxyz[ix]
             mins = verts.min(axis=0)
             maxs = verts.max(axis=0)
 
             return [(mins[0], maxs[0]), (mins[1], maxs[1]), (mins[2], maxs[2])]
         except Exception as e:
             # print(e)
-            print("No isosurface for this band")
+            # print("No isosurface for this band")
             return None
 
     def _get_isosurface(self, interp_factor:float=1):
         """
         The helper method will try to find the iso surface by using the marching cubes algorithm
 
         Parameters
@@ -335,15 +335,15 @@
         try:
             verts, faces, normals, values = measure.marching_cubes(
                 eigen_matrix, self.isovalue
             )
 
         except Exception as e:
             # print(e)
-            print("No isosurface for this band")
+            # print("No isosurface for this band")
             return None, None, None, None
             
         # recenter
         for ix in range(3):
             verts[:, ix] -= verts[:, ix].min()
             verts[:, ix] -= (verts[:, ix].max() -
                                 verts[:, ix].min()) / 2
```

### Comparing `PyProcar-6.0.0/pyprocar/core/kpath.py` & `PyProcar-6.1.0/pyprocar/core/kpath.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/core/procarselect.py` & `PyProcar-6.1.0/pyprocar/core/procarselect.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/core/procarsymmetry.py` & `PyProcar-6.1.0/pyprocar/core/procarsymmetry.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/core/procarunfold/_bak.procarparser.py` & `PyProcar-6.1.0/pyprocar/core/procarunfold/_bak.procarparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/core/procarunfold/fatband.py` & `PyProcar-6.1.0/pyprocar/core/procarunfold/fatband.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/core/procarunfold/procar_unfolder.py` & `PyProcar-6.1.0/pyprocar/core/procarunfold/procar_unfolder.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/core/procarunfold/unfolder.py` & `PyProcar-6.1.0/pyprocar/core/procarunfold/unfolder.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/core/structure.py` & `PyProcar-6.1.0/pyprocar/core/structure.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/core/surface.py` & `PyProcar-6.1.0/pyprocar/core/surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,17 +199,17 @@
         """
 
         def mag(vectors):
             return np.array([(vector[0]**2 + vector[1]**2 + vector[2]**2)**0.5 for vector in vectors])
         vectors = np.vstack([vectors_X, vectors_Y, vectors_Z]).T
         
         
-        self[vectors_name] = vectors
+        self.point_data[vectors_name] = vectors
         
-        self[vectors_name + "_magnitude"] = mag(vectors)
+        self.point_data[vectors_name + "_magnitude"] = mag(vectors)
         # self.set_active_scalars('vectors')
         return None
 
     def set_color_with_cmap(self, 
                             cmap:str="viridis", 
                             vmin:float=None, 
                             vmax:float=None):
```

### Comparing `PyProcar-6.0.0/pyprocar/io/__init__.py` & `PyProcar-6.1.0/pyprocar/io/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from . import vasp 
 from . import qe
 from . import lobster
 from . import abinit
 from . import siesta
+from . import elk
 # from . import bsxf
 # from . import frmsf
 
 from .parser import Parser
 
 from .procarparser import ProcarParser
 from .abinitparser import AbinitParser
```

### Comparing `PyProcar-6.0.0/pyprocar/io/abinit.py` & `PyProcar-6.1.0/pyprocar/pyposcar/poscar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,436 +1,459 @@
+#!/usr/bin/env python
+from __future__ import annotations
+import sys
 import re
-from numpy import array
-from ..core import Structure, DensityOfStates, ElectronicBandStructure, KPath
-from ..utils import elements
-from .vasp import Procar, Kpoints
 import numpy as np
-import glob
-import collections
-import os
-import sys
+import argparse
+
+class Poscar:
+  """A low-level class to store a crystal structure input (tailored for
+    VASP). 
+
+    If modified manually, the 'Cartesian' and 'direct' coords must be
+    updated together all the time by using `_set_cartesian` or
+    `_set_direct`.
+
+    The scaling factor, is internally set to 1.0, always. ie, the
+    scaling is included into the lattice.
+
+    The units are Angstroms.
+
+    Methods:
+
+    parse(self)                    # loads the whole file
+    _set_cartesian(self)           # set direct -> cartesian (internal)
+    _set_direct(self)              # set cartesian -> direct (internal)
+    _unparse(self, direct)         # data to string, use `write()` instead
+    write(self, filename, direct)  # saves the class to a POSCAR-like file
+    xyz(self, filename)            # saves a xyz file from the data
+    sort(self)                     # sorts the atoms, grouping them by element
+    remove()                       # removes one or more atoms from poscar
+    add(position, element, direct) # add one atom, only one each the time
+
+  """
+
+  def __init__(self,
+               filename:str,
+               verbose:bool=False):
+    """The file is not automatically loaded, you need to run
+    `self.parse()`
+    
+    Parameters
+    ----------
+
+    filename : str,
+        POSCAR-like file
+    verbose: bool,
+        verbosity level, for debugging. Default: False
+
+    Attributes:
+
+    self.verbose
+    self.filename
+    self.poscar:str str with the full POSCAR file
+    self.cpos: np.nadarray, Cartesian coordinates
+    self.dpos: np.ndarray, direct coordinates
+    self.lat: np.ndarray (3x3), the  lattice
+    self.typeSp: list, aame of atomic species, ordered
+    self.numberSp: np.ndarray, number of atoms per specie
+    self.Ntotal: int, total number of atoms in system
+    self.elm: list, element of each atoms one-by-one.
+    self.selective: bool, Selective dynamics?
+    self.selectFlags: None or nd.array(str), flags of selective dynamics
+    self.volume: float, the box product of the lattice
+
+    """
+    self.verbose = verbose
+    self.filename = filename
+    self.poscar:str = None
+    self.cpos:np.ndarray = None # cartesian coordinates
+    self.dpos:np.ndarray = None # direct coordinates
+    self.lat:np.ndarray = None # lattice
+    self.typeSp:List[str] = None # Name of atomic species
+    self.numberSp:nd.array = None # Number of atoms per specie
+    self.Ntotal:int = None # Total atoms in system
+    self.elm:List[str] = None # Element of each atoms one-by-one.
+    self.selective:bool = None # Selective dynamics
+    self.selectFlags:np.ndarray = None # all the T,F from selective dynamics
+    self.volume:float = None
+    self.loaded:bool = False # was the POSCAR-file loaded? i.e. self.parse()
+    return
+    
+  def parse(self, fromString:str = None):
+    """Loads into memory all the content of the POSCAR file.
+
+    Parameters
+    ----------
+    
+    fromString : str 
+      If present, instead of loading a file, it uses
+      this variable to populate the class. Default=None
+
+    """
+    if fromString and isinstance(fromString, str):
+      self.poscar = fromString.split('\n')
+    elif fromString and isinstance(fromString, list):
+      self.poscar = fromString
+    else:
+      self.poscar = open(self.filename, 'r')
+      self.poscar = self.poscar.readlines()
+
+    # getting the scale factor
+    scale = re.findall(r'[.\d]+', self.poscar[1])
+    scale = float(scale[0])
+    if self.verbose:
+      print('scaling factor: ', scale)
+    
+    # parsing the lattice
+    self.lat = re.findall(r'[-.\d]+\s+[-.\d]+\s+[-.\d]+\s*\n*', ''.join(self.poscar[2:5]))
+    self.lat = np.array([x.split() for x in self.lat], dtype=float)*scale
+    if self.verbose:
+      print( 'lattice:\n', self.lat)
+
+    # type of atoms and number of atoms per type
+    self.typeSp = re.findall(r'(\w+)\s*', self.poscar[5])
+    if len(self.typeSp) == 0:
+      raise RuntimeError("No data about the atomic species found. Correct it.")
+    if self.verbose:
+      print( 'atoms per species:\n', self.typeSp)
+    self.numberSp = re.findall(r'(\d+)\s*', self.poscar[6])
+    self.numberSp = np.array(self.numberSp, dtype=int)
+    self.Ntotal = np.sum(self.numberSp)
+    if self.verbose:
+      print( 'atomic species:\n', self.numberSp)
+      print( 'The total is ' + str(self.Ntotal) + ' atoms')
+    
+    # selective dynamics? setting a offset
+    if re.findall(r'^\s*[sS]', self.poscar[7]) :
+      self.selective = True
+      offset = 1
+      if self.verbose:
+        print( "Selective Dynamics")
+    else:
+      self.selective = False
+      offset = 0
+      
+    # Direct coordinates unless otherwise
+    direct = True
+    if not re.findall(r'^\s*[Dd]', self.poscar[7+offset]) :
+      direct = False
+      if self.verbose:
+        print('Positions in Cartesian coordinates')
+    else:
+      if self.verbose:
+        print('Positions in Direct coordinates')
+
+    # parsing the positions
+    start, end = 8+offset, 8+offset+ self.Ntotal
+    string = r'([-.\d]+)\s+([-.\d]+)\s+([-.\d]+)\s*'
+    pos = re.findall(string, ''.join(self.poscar[start:end]))
+    if direct:
+      self.dpos = np.array(pos, dtype=float)
+      self._set_cartesian()
+    else:
+      self.cpos = np.array(pos, dtype=float)
+      self._set_direct()
+    if self.verbose:
+      print( "Atomic positions (direct)\n", self.dpos)
+      print( "Atomic positions (cartesian)\n", self.cpos)
+
+    # parsing selective dynamics
+    if self.selective == True:
+      string = r'([TF]+)\s+([TF]+)\s+([TF]+)\s+'
+      selectFlags = re.findall(string, ''.join(self.poscar[start:end]))
+      self.selectFlags = np.array(selectFlags)
+      print('Flags of selective dynamics:\n', self.selectFlags)
+      
+    # setting a list of elements:
+    elementList = zip(self.typeSp, self.numberSp)
+    self.elm = ' '.join([' '.join([x]*y) for x,y in elementList]).split()
+    if self.verbose:
+      print('Elements: ', self.elm)
+
+    # setting the volume, just as an utility
+    self.volume = np.linalg.det(self.lat)
+    self.loaded = True
+    return
+
+  def _set_cartesian(self):
+    """set the cartesian positions (self.cpos) from direct positions (self.dpos).
+    """
+    cart = np.dot(self.lat.T, self.dpos.T)
+    cart = cart.T
+    self.cpos = cart
+    
+  def _set_direct(self):
+    """set the direct positions (self.dpos) from Cartesian positions (self.cpos).
+    """
+    inverse = np.linalg.inv(self.lat)
+    direct = np.dot(inverse.T, self.cpos.T)
+    direct = direct.T
+    self.dpos = direct
+    
+  def _unparse(self, direct:bool=True):
+    """Internal method to be used previously to to writing a POSCAR
+    file. It group together all the information in a single str,
+    `self.poscar`. The information is as it is. No PBC are applied,
+    and no checks are performed at this stage.  The scaling factor is
+    1.0, always.
+
+
+    Parameters
+    ----------
+
+    direct: bool
+        direct positons is True, Cartesian is Falsepositions. Default is True
 
+    """
+
+    # We will start with getting the positions
+    if direct == True:
+      pos = self.dpos
+    else:
+      pos = self.cpos
+      
+    # creating a list of text lines with positions
+    pos = [' '.join([str(coord) for coord in line]) for line in pos]
+
+    # Now we will look whether selective dynamics are used
+    if self.selective == True:
+      # a list of text lines with flags
+      flags = [' '.join([flag for flag in line]) for line in pos]
+      pos = [pos + ' ' + flag for (pos, flag) in zip(pos,flags)]
+
+    pos = '\n'.join(pos)
+
+    # Creating the POSCAR text string
+    self.poscar = "poscar.py\n"
+    self.poscar += "1.0\n"
+    self.poscar += '\n'.join([' '.join([str(y) for y in x]) for x in self.lat]) + '\n'
+    self.poscar += ' '.join(self.typeSp) + '\n'
+    self.poscar += ' '.join([str(x) for x in self.numberSp]) + '\n'
+    if self.selective:
+      self.poscar += 'Selective Dynamics\n'
+    if direct == False:
+      self.poscar += 'Cartesian\n'
+    else:
+      self.poscar += 'Direct\n'
+    self.poscar += pos # already set with the the T, F -if needed
+    self.poscar += '\n'
+    
+    if self.verbose:
+      print("\n\n unparsed POSCAR\n\n")
+      print('unparse, self.poscar\n', self.poscar)
+
+
+  def write(self, filename:str='POSCAR.out', direct:bool=True):
+    """Writes a poscar file with the information stored in the class.
+
+    Parameters
+    ----------
+
+    filename : str
+        default='POSCAR.out', name of the output file.
+    direct : bool
+        direct positons is True, Cartesian is Falsepositions. Default is True
+    """
+    self._unparse(direct=direct)
+    fout = open(filename, 'w')
+    fout.write(self.poscar)
+    if self.verbose:
+      print('File '  + filename + ' written.')
+    return
+      
+  def xyz(self, filename:str):
+    """Writes an xyz file, the lattice is written as a comment line
+
+    Parameters
+    ----------
 
-class Output(collections.abc.Mapping):
-    """This class contains methods to parse the fermi energy, reciprocal
-    lattice vectors and structure from the Abinit output file.
-    """
-
-    def __init__(self, abinit_output=None):
-
-        # variables
-        self.abinit_output = abinit_output
-        self.fermi = None
-        self.reclat = None  # reciprocal lattice vectors
-        self.nspin = None  # spin
-        self.coordinates = None  # reduced atomic coordinates
-        self.variables = {}
-
-        # call parsing functions
-        self._readFermi()
-        self._readRecLattice()
-        self._readCoordinates()
-        self._readLattice()
-        self._readAtoms()
-
-        # creating structure object
-        self.structure = Structure(
-            atoms=self.atoms,
-            fractional_coordinates=self.coordinates,
-            lattice=self.lattice,
-        )
-
-        return
-
-    def _readFermi(self):
-        """Reads the Fermi energy from the Abinit output file."""
-
-        with open(self.abinit_output, "r") as rf:
-            data = rf.read()
-            self.fermi = float(
-                re.findall(
-                    r"Fermi\w*.\(\w*.HOMO\)\s*\w*\s*\(\w*\)\s*\=\s*([0-9.+-]*)", data
-                )[0]
-            )
-
-            # Converting from Hartree to eV
-            self.fermi = 27.211396641308 * self.fermi
-
-            # read spin (nsppol)
-            self.nspin = re.findall(r"nsppol\s*=\s*([1-9]*)", data)[0]
-
-            return
-
-    def _readRecLattice(self):
-        """Reads the reciprocal lattice vectors
-        from the Abinit output file. This is used to calculate
-        the k-path in cartesian coordinates if required."""
-
-        with open(self.abinit_output, "r") as rf:
-            data = rf.read()
-            lattice_block = re.findall(r"G\([1,2,3]\)=\s*([0-9.\s-]*)", data)
-            lattice_block = lattice_block[3:]
-            self.reclat = array(
-                [lattice_block[0:3][i].split() for i in range(len(lattice_block))],
-                dtype=float,
-            )
-
-            return
-
-    def _readCoordinates(self):
-        """Reads the coordinates as given by the xred keyword."""
-
-        with open(self.abinit_output, "r") as rf:
-            data = rf.read()
-            coordinate_block = re.findall(r"xred\s*([+-.0-9E\s]*)", data)[-1].split()
-            coordinate_list = np.array([float(x) for x in coordinate_block])
-            self.coordinates = coordinate_list.reshape(len(coordinate_list) // 3, 3)
-
-            return
-
-    def _readLattice(self):
-        """Reads the lattice vectors from rprim keyword and scales with acell."""
-
-        with open(self.abinit_output, "r") as rf:
-            data = rf.read()
-
-            # acell
-            acell = re.findall(r"acell\s*([+-.0-9E\s]*)", data)[-1].split()
-            acell = np.array([float(x) for x in acell])
-
-            # convert acell from Bohr to Angstrom
-            acell = 0.529177 * acell
-
-            # rprim
-            rprim_block = re.findall(r"rprim\s*([+-.0-9E\s]*)", data)[-1].split()
-            rprim_list = np.array([float(x) for x in rprim_block])
-            rprim = rprim_list.reshape(len(rprim_list) // 3, 3)
-
-            # lattice
-            self.lattice = np.zeros(shape=(3, 3))
-            for i in range(len(acell)):
-                self.lattice[i, :] = acell[i] * rprim[i, :]
-
-            return
-
-    def _readAtoms(self):
-        """Reads atomic elements used and puts them in an array according to their composition."""
-
-        with open(self.abinit_output, "r") as rf:
-            data = rf.read()
-
-            # Getting typat and znucl
-            typat = re.findall(r"typat\s*([+-.0-9E\s]*)", data)[-1].split()
-            typat = [int(x) for x in typat]
-
-            znucl = re.findall(r"znucl\s*([+-.0-9E\s]*)", data)[-1].split()
-            znucl = [int(float(x)) for x in znucl]
-
-            self.atoms = [elements.atomic_symbol(znucl[x - 1]) for x in typat]
-
-    def __contains__(self, x):
-        return x in self.variables
-
-    def __getitem__(self, x):
-        return self.variables.__getitem__(x)
-
-    def __iter__(self):
-        return self.variables.__iter__()
-
-    def __len__(self):
-        return self.variables.__len__()
-
-
-class AbinitKpoints(collections.abc.Mapping):
-    """This class parses the k-point information."""
-
-    def __init__(self, filename="KPOINTS", has_time_reversal=True):
-        self.variables = {}
-
-        # calling parser
-        self._parse_kpoints()
-        self.kpath = KPath(
-            knames=self.abinitkpointsobject.knames,
-            special_kpoints=self.abinitkpointsobject.special_kpoints,
-            ngrids=self.abinitkpointsobject.ngrids,
-            has_time_reversal=has_time_reversal,
-        )
-
-    def _parse_kpoints(self):
-        """Reads KPOINTS file.
-        Abinit has multiple way of defining the
-        k-path. For the time being, we suggest to use
-        a KPOINTS file similar to VASP to obtain the
-        k-path for PyProcar from an Abinit calculation.
-        """
-        self.abinitkpointsobject = Kpoints(filename="KPOINTS", has_time_reversal=True)
-
-    def __contains__(self, x):
-        return x in self.variables
-
-    def __getitem__(self, x):
-        return self.variables.__getitem__(x)
-
-    def __iter__(self):
-        return self.variables.__iter__()
-
-    def __len__(self):
-        return self.variables.__len__()
-
-
-class AbinitProcar(collections.abc.Mapping):
-    """This class has functions to parse the PROCAR file
-    generated from Abinit. Unlike, VASP here the PROCAR files
-    need to be merged and fixed for formatting issues prior to
-    further processing.
-    """
-
-    def __init__(
-        self,
-        inFiles=None,
-        abinit_output=None,
-        reciprocal_lattice=None,
-        kpath=None,
-        efermi=None,
-    ):
-        self.variables = {}
-        self.inFiles = inFiles
-        self.abinit_output = abinit_output
-        self.reciprocal_lattice = reciprocal_lattice
-        self.kpath = kpath
-        self.efermi = efermi
-
-        # Preparing files for merging
-        # reading in all PROCAR_* files and putting it into a list if not provided.
-        if inFiles is None:
-            inFiles = sorted(glob.glob("PROCAR_*"))
-        else:
-            inFiles = inFiles
-
-        if isinstance(inFiles, list):
-            self._mergeparallel(
-                inputfiles=inFiles,
-                outputfile="PROCAR",
-                abinit_output=self.abinit_output,
-            )
-        else:
-            pass
-
-        # Use VASP Procar parser following PROCAR merge
-        self.abinitprocarobject = Procar(
-            filename="PROCAR",
-            structure=None,
-            reciprocal_lattice=self.reciprocal_lattice,
-            kpath=self.kpath,
-            kpoints=None,
-            efermi=self.efermi,
-            interpolation_factor=1,
-        )
-
-    def _mergeparallel(self, inputfiles=None, outputfile=None, abinit_output=None):
-        """This merges Procar files seperated between k-point ranges.
-        Happens with parallel Abinit runs.
-        """
-        print("Merging parallel files...")
-        filenames = sorted(inputfiles)
-        print(filenames)
-
-        # creating an instance of the AbinitParser class
-        if abinit_output:
-            abinitparserobject = Output(abinit_output=abinit_output)
-            nspin = int(abinitparserobject.nspin)
-        else:
-            raise IOError("Abinit output file not found.")
-
-        if nspin != 2:
-            with open(outputfile, "w") as outfile:
-                for fname in filenames:
-                    with open(fname) as infile:
-                        for line in infile:
-                            outfile.write(line)
-
-        elif nspin == 2:
-            # for spin polarized calculations the spin down segments are saved in the
-            # second half of the PROCAR's but in reverse k-point order. So we have to
-            # fix the order and merge the second half of the PROCAR's.
-            spinup_list = filenames[: int(len(filenames) / 2)]
-            spindown_list = filenames[int(len(filenames) / 2) :]
-
-            # reading the second line of the header to set as the separating line
-            # in the colinear spin PROCAR.
-            fp = open(spinup_list[0], "r")
-            header1 = fp.readline()
-            header2 = fp.readline()
-            fp.close()
-
-            # second half of PROCAR files in reverse order.
-            spindown_list.reverse()
-
-            # Writing new PROCAR with first spin up, header2 and then
-            # spin down (reversed).
-            with open(outputfile, "w") as outfile:
-                for spinupfile in spinup_list:
-                    with open(spinupfile) as infile:
-                        for line in infile:
-                            outfile.write(line)
-                outfile.write("\n")
-                outfile.write(header2)
-                outfile.write("\n")
-                for spindownfile in spindown_list:
-                    with open(spindownfile) as infile:
-                        for line in infile:
-                            outfile.write(line)
-
-    def _fixformat(self, inputfile=None, outputfile=None):
-
-        """Fixes the formatting of Abinit's Procar
-        when the tot projection is not summed and spin directions
-        not seperated.
-        """
-        print("Fixing formatting errors...")
-        # removing existing temporary fixed file
-        if os.path.exists(outputfile):
-            os.remove(outputfile)
-
-        ####### Fixing the parallel PROCARs from Abinit ##########
-
-        rf = open(inputfile, "r")
-        data = rf.read()
-        rf.close()
-
-        # reading headers
-        rffl = open(inputfile, "r")
-        first_line = rffl.readline()
-        rffl.close()
-
-        # header
-        header = re.findall("#\sof\s.*", data)[0]
-
-        # writing to PROCAR
-        fp = open(outputfile, "a")
-        fp.write(first_line)
-        fp.write(str(header) + "\n\n")
-
-        # get all the k-point line headers
-        kpoints_raw = re.findall("k-point\s*[0-9]\s*:*.*", data)
-
-        for kpoint_counter in range(len(kpoints_raw)):
-
-            if kpoint_counter == (len(kpoints_raw) - 1):
-                # get bands of last k point
-                bands_raw = re.findall(
-                    kpoints_raw[kpoint_counter] + "([a-z0-9\s\n.+#-]*)", data
-                )[0]
-
-            else:
-                # get bands between k point n and n+1
-                bands_raw = re.findall(
-                    kpoints_raw[kpoint_counter]
-                    + "([a-z0-9\s\n.+#-]*)"
-                    + kpoints_raw[kpoint_counter + 1],
-                    data,
-                )[0]
-
-            # get the bands headers for a certain k point
-            raw_bands = re.findall("band\s*[0-9]*.*", bands_raw)
-
-            # writing k point header to file
-            fp.write(kpoints_raw[kpoint_counter] + "\n\n")
-
-            for band_counter in range(len(raw_bands)):
-
-                if band_counter == (len(raw_bands) - 1):
-                    # the last band
-                    single_band = re.findall(
-                        raw_bands[band_counter] + "([a-z0-9.+\s\n-]*)", bands_raw
-                    )[0]
-
-                else:
-                    # get a single band
-                    single_band = re.findall(
-                        raw_bands[band_counter]
-                        + "([a-z0-9.+\s\n-]*)"
-                        + raw_bands[band_counter + 1],
-                        bands_raw,
-                    )[0]
-
-                # get the column headers for ion, orbitals and total
-                column_header = re.findall("ion\s.*tot", single_band)[0]
-
-                # get number of ions using PROCAR file
-                nion_raw = re.findall("#\s*of\s*ions:\s*[0-9]*", data)[0]
-                nion = int(nion_raw.split(" ")[-1])
-
-                # the first column of the band. Same as ions
-                first_column = []
-                for x in single_band.split("\n"):
-                    if x != "":
-                        if x != " ":
-                            if x.split()[0] != "ion":
-                                first_column.append(x.split()[0])
-
-                # number of spin orientations
-                norient = int(len(first_column) / nion)
-
-                # calculate the number of orbital headers (s,p,d etc.)
-                for x in single_band.split("\n"):
-                    if x != "":
-                        if x != " ":
-                            if x.split()[0] == "ion":
-                                norbital = len(x.split()) - 2
-
-                # array to store a single band data as seperate lines
-                single_band_lines = []
-                for x in single_band.split("\n"):
-                    if x != "":
-                        if x != " ":
-                            if x.split()[0] != "ion":
-                                single_band_lines.append(x)
-
-                # create empty array to store data (the orbitals + tot)
-                bands_orb = np.zeros(shape=(norient, nion, norbital + 1))
-
-                # enter data into bands_orb
-                iion = 0
-                iorient = 0
-                for x in single_band.split("\n"):
-                    if x != "" and x != " " and x.split()[0] != "ion":
-                        iline = x.split()
-                        if iion > 1:
-                            iion = 0
-                            iorient += 1
-                        for iorb in range(0, norbital + 1):
-                            bands_orb[iorient, iion, iorb] = float(iline[iorb + 1])
-                        iion += 1
-
-                # create an array to store the total values
-                tot = np.zeros(shape=(norient, norbital + 1))
-
-                # entering data into tot array
-                for iorient in range(norient):
-                    tot[iorient, :] = np.sum(bands_orb[iorient, :, :], axis=0)
-
-                # writing data
-                fp.write(raw_bands[band_counter] + "\n\n")
-                fp.write(column_header + "\n")
-
-                band_iterator = 0
-                total_count = 0
-                for orientations_count in range(norient):
-                    for ions_count in range(nion):
-                        fp.write(single_band_lines[band_iterator] + "\n")
-                        band_iterator += 1
-                    fp.write("tot  " + " ".join(map(str, tot[total_count, :])) + "\n\n")
-                    total_count += 1
-        fp.close()
-
-    def __contains__(self, x):
-        return x in self.variables
+    filename: str
+        the name of the .xyz file, The .xyz extension is not automatically added
+    """
+    xyzf = open(filename, 'w')
+    xyzf.write(str(self.Ntotal) + '\n')
+
+    # The comment line has the lettice
+    latStr = np.array(self.lat, dtype=str).flatten()
+    latStr = ' '.join(latStr)
+    xyzf.write('Lattice="'  + latStr + '"\n')
+    
+    # continuing with the positions
+    pos = self.cpos
+    pos = np.array(pos, dtype=str)
+    pos = [' '.join(x) for x in pos]
+    elm = list(self.elm)
+    xyzstr = '\n'.join( [ x + ' ' + y for x,y in zip(elm, pos) ] )
+    xyzf.write(xyzstr)
+    xyzf.write('\n')
+    xyzf.close()
+    if self.verbose:
+      print(filename + ' written as xyz')
+      
+  def sort(self):
+    """This method updates the internal arrays related to elements and
+    atoms per element. Automatically used when using `self.add`
+    """
+    #
+    # self.typeSp, self.elem, self.dpos
+    # must be present and updated (they can be disordered)
+    #
+    from collections import OrderedDict
+    # getting the different element's names, without repetitions
+    self.typeSp = list(OrderedDict.fromkeys(self.typeSp))
+    if self.verbose:
+      print('The list of elements is ', self.typeSp)
+    # lists of ordered atoms
+    atoms = []
+    elements = []
+    if self.verbose:
+      print('to sort: ', self.elm, '\n', self.dpos)
+    
+    # ordering the positions accordiong to its element.
+    for thiselem in self.typeSp:
+      # Joining each element with its position
+      for elem, pos in zip(self.elm, self.dpos):
+        if thiselem == elem:
+          atoms.append(pos)
+          elements.append(elem)
+    if self.verbose:
+      print('sorted: ', elements, '\n', np.array(atoms))
+
+    self.elm = elements
+    # setting the position's list in direct coords.
+    self.dpos = np.array(atoms)
+    # and in cartesian coords as well
+    self._set_cartesian()
+
+    # How many atoms by element?
+    from collections import Counter
+    # a dict of elements and its repetitions
+    counter = Counter(elements)
+    self.numberSp = [counter[x] for x in self.typeSp]
+    
+    self.Ntotal = sum(self.numberSp)
+    if self.verbose:
+      print ("N atoms per specie, ", self.numberSp, '. Total: ', self.Ntotal)
 
-    def __getitem__(self, x):
-        return self.variables.__getitem__(x)
+  def remove(self, atoms:list|int):
+    """
+    Remove one or more atoms.
+
+    Parameters:
+
+    atoms : int|list
+        removes the atom(s) with given indexes (0-based)
+    """
+    # atoms maybe (or not) just one atom (an int, not a one-sized list)
+    if self.verbose:
+      print('going to delete the following atom(s):', atoms)
+    try:
+      iterator = iter(atoms)
+    except TypeError:
+      atoms = [atoms]
+      
+    # we will populate a list with the atoms to keep
+    keep = [True]*self.Ntotal
+    for atom in atoms:
+      if atom >= self.Ntotal:
+        raise RuntimeError('Error: atom index is larger than the atom number')
+      keep[atom] = False
+    # creating new arrays without the removed elements
+    self.cpos = self.cpos[keep]
+    self.dpos = self.dpos[keep]
+    self.Ntotal = len(self.cpos)
+    
+    # self.elm is a list, I am not sure why, but I will cast it back to list
+    self.elm = np.array(self.elm)
+    self.elm = self.elm[keep]
+    self.elm = list(self.elm)
+    
+    if self.selective:
+      self.selectFlags = self.selectFlags[keep]
+    # the atoms types and their number can be modified, we need to
+    # count them from self.elm
+    # Also I want to keep the order of elements
+    from collections import OrderedDict
+    self.typeSp = list(OrderedDict.fromkeys(self.elm).keys())
+    self.numberSp = [self.elm.count(x) for x in self.typeSp]
+    if self.verbose:
+      print('Elements', self.elm)
+      print(self.typeSp, self.numberSp)
+    # no need to sort, deleting doesn't alters the occurence
+    return
+
+  def add(self,
+          position:np.ndarray,
+          element:str,
+          direct:bool=True,
+          selectiveFlags:np.ndarray=None):
+    """Adds one atom to the class. Only one atom at the time
+
+    Parameters
+    ----------
+
+    position : np.ndarray
+        (3 or 1x3) the positions of new atom
+    element : str
+        Name of the element of the new atom
+    direct : bool
+        are the positions given  direct (True) or Cartesian (False) 
+        coordinates? Default is True
+    selectiveFlags : np.ndarray(str)
+        only of `self.selective == True`
+
+    """
+    position = np.array(position, dtype=float)
+    position.shape = (1,3)
+    if self.verbose:
+      print('going to add an ' +element+  ' atom at', position, end=',')
+      if direct:
+        print('in direct coordinates')
+      else:
+        print('in Cartesian coordiantes')
+    # setting the data
+    if direct:
+      self.dpos = np.concatenate((self.dpos, position))
+    else:
+      self.cpos = np.concatenate((self.cpos, position))
+    self.Ntotal = self.Ntotal + 1
+    self.elm.append(element)
+    if self.selective and selectiveFlags:
+      if self.verbose:
+        print('selective flag found.')
+      selectiveFlags = np.array(selectiveFlags, dtype=str)
+      self.selectFlags = np.concatenate(self.selectFlags, selectiveFlags)
+    # setting the other data
+    if direct:
+      self._set_cartesian()
+    else:
+      self._set_direct()
+    # the atoms types and their number can be modified, we need to
+    # count them from self.elm
+    # Also I want to keep the order of elements
+    from collections import OrderedDict
+    self.typeSp = list(OrderedDict.fromkeys(self.elm).keys())
+    self.numberSp = [self.elm.count(x) for x in self.typeSp]
+    if self.verbose:
+      print('Elements', self.elm)
+      print(self.typeSp, self.numberSp)
+    # sorting the data
+    self.sort()
+    return
+
+    
+        
+      
+if __name__ == '__main__':
+  parser = argparse.ArgumentParser()
+  parser.add_argument("inputfile", type=str, help="input file")
+  parser.add_argument('-v', '--verbose', action='store_true')
+  parser.add_argument('--xyz', action='store_true')
+  
+  args = parser.parse_args()
 
-    def __iter__(self):
-        return self.variables.__iter__()
+  p = Poscar(args.inputfile, verbose=args.verbose)
+  p.parse()
 
-    def __len__(self):
-        return self.variables.__len__()
+  if args.xyz:
+    p.xyz(args.inputfile + '.xyz')
```

### Comparing `PyProcar-6.0.0/pyprocar/io/abinitparser/abinitparser.py` & `PyProcar-6.1.0/pyprocar/io/abinitparser/abinitparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/bxsf.py` & `PyProcar-6.1.0/pyprocar/io/bxsf.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/elk.py` & `PyProcar-6.1.0/pyprocar/io/elk.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/elkparser/elkparser.py` & `PyProcar-6.1.0/pyprocar/io/elkparser/elkparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/frmsf.py` & `PyProcar-6.1.0/pyprocar/io/frmsf.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/lobster.py` & `PyProcar-6.1.0/pyprocar/io/lobster.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/lobsterparser/lobster_doscar_parser.py` & `PyProcar-6.1.0/pyprocar/io/lobsterparser/lobster_doscar_parser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/lobsterparser/lobsterfermiparser.py` & `PyProcar-6.1.0/pyprocar/io/lobsterparser/lobsterfermiparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/lobsterparser/lobsterparser.py` & `PyProcar-6.1.0/pyprocar/io/lobsterparser/lobsterparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/parser.py` & `PyProcar-6.1.0/pyprocar/io/parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 
 from ..core import ElectronicBandStructure
 from ..core import DensityOfStates
 from ..core import Structure
 from ..utils import UtilsProcar
 
-from . import vasp, qe, abinit, lobster, siesta, frmsf, bxsf
+from . import vasp, qe, abinit, lobster, siesta, frmsf, bxsf, elk
 
 class Parser:
     """
     The parser class will be the main object to be used through out the code. 
     This class will handle getting the main inputs (ebs,dos,structure,kpath,reciprocal_lattice) from the various dft parsers.
     """
     code : str = None
@@ -44,34 +44,50 @@
 
         elif self.code == "siesta":
             self.parse_siesta()
 
         elif self.code == "vasp":
             self.parse_vasp()
 
-        self.ebs.bands += self.ebs.efermi
+        elif self.code == "elk":
+            self.parse_elk()
+
+        if self.ebs:
+            self.ebs.bands += self.ebs.efermi
 
         return None
 
     def parse_abinit(self):
         """parses abinit files
 
         Returns
         -------
         None
             None
         """
         outfile = f"{self.dir}{os.sep}abinit.out"
         kpointsfile = f"{self.dir}{os.sep}KPOINTS"
+        abinit_output = abinit.Output(abinit_output=outfile)
+        abinit_kpoints = abinit.AbinitKpoints(filename=kpointsfile)
 
-        parser = abinit.Output(abinit_output=outfile)
+        parser =  abinit.AbinitProcar(  
+                                        dirname=self.dir,
+                                        abinit_output=outfile,
+                                        kpath=abinit_kpoints.kpath,
+                                        reciprocal_lattice=abinit_output.reclat,
+                                        efermi=abinit_output.fermi
+                                        )
         
+        abinit_dos = abinit.AbinitDOSParser(dirname=self.dir)
+
+        self.dos = abinit_dos.dos
         self.ebs = parser.abinitprocarobject.ebs
         self.kpath = parser.abinitprocarobject.ebs.kpath
-        self.structure = parser.abinitprocarobject.structure
+        self.structure = abinit_output.structure
+        
 
         return None
     
     def parse_bxsf(self):
         """parses bxsf files.
 
         Returns
@@ -86,14 +102,28 @@
         self.ebs = parser.ebs
         self.kpath = parser.kpath
         self.structure = parser.structure
         self.dos = parser.dos
 
         return None
     
+    def parse_elk(self):
+        """parses bxsf files.
+
+        Returns
+        -------
+        None
+            None
+        """
+        
+        dos = elk.read_dos(path = self.dir)
+        self.dos = dos
+
+        return None
+    
     def parse_frmsf(self):
         """parses frmsf files. Needs to be finished
 
         Returns
         -------
         None
             None
@@ -194,28 +224,30 @@
         outcar = vasp.Outcar(outcar)
 
         try:
             poscar = vasp.Poscar(poscar,rotations = outcar.rotations)
         except:
             poscar = vasp.Poscar(poscar,rotations = None)
 
-            
         try:
             kpoints = vasp.Kpoints(kpoints)
             self.kpath = kpoints.kpath
         except:
-            self.kpath = None
+            self.kpath=None
 
         
 
         procar = vasp.Procar(
                             filename=procar,
                             structure=poscar.structure,
                             reciprocal_lattice=poscar.structure.reciprocal_lattice,
                             kpath=self.kpath,
+                            n_kx=outcar.n_kx,
+                            n_ky=outcar.n_ky,
+                            n_kz=outcar.n_kz,
                             efermi=outcar.efermi,
                             interpolation_factor=1
                             )
         
         try:
             vasprun = vasp.VaspXML(filename = vasprun)
         except:
@@ -223,12 +255,11 @@
         
         self.ebs = procar.ebs
         self.structure = poscar.structure
 
         try:
             self.dos = vasprun.dos
         except Exception as e:
-            print(e)
             self.dos = None
 
         return None
```

### Comparing `PyProcar-6.0.0/pyprocar/io/procarparser/procarparser.py` & `PyProcar-6.1.0/pyprocar/io/procarparser/procarparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/qe.py` & `PyProcar-6.1.0/pyprocar/io/qe.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/siesta.py` & `PyProcar-6.1.0/pyprocar/io/siesta.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/io/vasp.py` & `PyProcar-6.1.0/pyprocar/io/vasp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,52 +1,100 @@
 import os
 import re
 import xml.etree.ElementTree as ET
 import collections
 import gzip
+from typing import List, Tuple, Union, Dict, Any, Optional
+from pathlib import Path
+from functools import cached_property
 
 import numpy as np
 from numpy import array
 
 from ..core import Structure, DensityOfStates, ElectronicBandStructure, KPath
 
 
 class Outcar(collections.abc.Mapping):
     """
-    A class to parse the OUTCAR
+    A class to parse the OUTCAR file from a VASP run and extract electronic structure data.
+
+    The OUTCAR file provides detailed output of a VASP run, including a summary of used input parameters, 
+    information about electronic steps and KS-eigenvalues, stress tensors, forces on atoms, local charges 
+    and magnetic moments, and dielectric properties. The amount of output written onto the OUTCAR file can 
+    be chosen by modifying the NWRITE tag in the INCAR file.
+    
+    The Outcar class acts as a Mapping, providing key-value access to the variables parsed from the OUTCAR file.
 
     Parameters
     ----------
-    filename : str, optional
-        The OURCAR filename, by default "OUTCAR"
+    filename : Union[str, Path], optional
+        The OUTCAR filename. If not provided, defaults to "OUTCAR".
+        
+    Attributes
+    ----------
+    variables : dict
+        A dictionary storing variables parsed from the OUTCAR file.
+    filename : Path
+        The path to the OUTCAR file.
+    file_str : str
+        The full string content of the OUTCAR file.
     """
-    def __init__(self, filename="OUTCAR"):
+    
+    def __init__(self, filename: Union[str, Path] = "OUTCAR"):
+        """
+        Constructor method to initialize an Outcar object. Reads the file specified by filename and stores its content.
+
+        Parameters
+        ----------
+        filename : Union[str, Path], optional
+            The OUTCAR filename. If not provided, defaults to "OUTCAR".
+        """
         
-        self.variables = {}
-        self.filename = filename
+        self.variables: dict = {}
+        self.filename: Path = Path(filename)
+                self._get_axes_nk()
 
         with open(self.filename, "r") as rf:
-            self.file_str = rf.read()
+            self.file_str: str = rf.read()
+    def _get_axes_nk(self):
+        """
+        n_kx
 
+        Returns
+        -------
+        n_kx
+            n_kx
+        """
+        try:
+            raw_text=re.findall("generate\s*k-points\s*for:\s*(.*)", self.file_str)[-1]
+            self.n_kx=int(raw_text.split()[0])
+            self.n_ky=int(raw_text.split()[1])
+            self.n_kz=int(raw_text.split()[2])
+        except:
+            self.n_kx=None
+            self.n_ky=None
+            self.n_kz=None
+            
+        return None
 
 
-    @property
+    @cached_property
     def efermi(self):
         """
         Just finds all E-fermi fields in the outcar file and keeps the
         last one (if more than one found).
 
         Returns
         -------
         fermi
             the fermi energy
         """
         return float(re.findall(r"E-fermi\s*:\s*(-?\d+.\d+)", self.file_str)[-1])
 
-    @property
+    @cached_property
     def reciprocal_lattice(self):
         """
         Finds and return the reciprocal lattice vectors, if more than
         one set present, it return just the last one.
 
         Returns
         -------
@@ -61,29 +109,28 @@
         reciprocal_lattice = np.array(reciprocal_lattice, dtype=float)
         # up to now I have, both direct and rec. lattices (3+3=6 columns)
         reciprocal_lattice = np.reshape(reciprocal_lattice, (3, 6))
         reciprocal_lattice = reciprocal_lattice[:, 3:]
         return reciprocal_lattice
 
 
-    @property
+    @cached_property
     def rotations(self):
         """
         Finds the point symmetry operations included in the OUTCAR file
         and returns them in matrix form.
 
         Returns
         -------
         np.ndarray
             The rotation matrices
         """
 
 
-        with open(self.filename) as f:
-            txt = f.readlines()
+        txt = self.file_str.split('\n')
 
         has_new_rotation_format = False
         i_rotation_lines=[]
         for i, line in enumerate(txt):
             if 'isymop' in line:
                 has_new_rotation_format = True
                 i_rotation_lines.append(i)
@@ -152,17 +199,16 @@
                 # R = self.reciprocal_lattice.dot(R).dot(np.linalg.inv(self.reciprocal_lattice))
                 R = np.linalg.inv(self.reciprocal_lattice.T).dot(R).dot(self.reciprocal_lattice.T)
                 R = np.round_(R, decimals=3)
                 rotations.append(R)
         return np.array(rotations)
 
     def get_symmetry_operations(self):
-        with open(self.filename) as f:
-            txt = f.readlines()
 
+        txt = self.file_str.split('\n')
         has_new_rotation_format = False
         i_rotation_lines=[]
         for i, line in enumerate(txt):
             if 'isymop' in line:
                 has_new_rotation_format = True
                 i_rotation_lines.append(i)
             if 'irot' in line:
@@ -338,21 +384,21 @@
         self.kshift = None
         self.ngrids = None
         self.special_kpoints = None
         self.knames = None
         self.cartesian = False
         self.automatic = False
         self._parse_kpoints()
-        self.kpath = KPath(
-            knames=self.knames,
-            special_kpoints=self.special_kpoints,
-            ngrids=self.ngrids,
-            has_time_reversal=has_time_reversal,
-        )
-
+        if self.knames is not None:
+            self.kpath = KPath(
+                knames=self.knames,
+                special_kpoints=self.special_kpoints,
+                ngrids=self.ngrids,
+                has_time_reversal=has_time_reversal,
+            )
 
     def _parse_kpoints(self):
         """A helper method to parse the KOINTS file
         """
         with open(self.filename, "r") as rf:
             self.comment = rf.readline()
             grids = rf.readline()
@@ -501,15 +547,17 @@
         """
     def __init__(
         self,
         filename:str="PROCAR",
         structure:Structure=None,
         reciprocal_lattice:np.ndarray=None,
         kpath:KPath=None,
-        kpoints:np.ndarray=None,
+        n_kx:int=None,
+        n_ky:int=None,
+        n_kz:int=None,
         efermi:float=None,
         interpolation_factor:float=1,
     ):
         
         self.variables = {}
         self.filename = filename
         self.meta_lines = []
@@ -569,14 +617,17 @@
         # self.bands -= efermi
         self.ebs = ElectronicBandStructure(
             kpoints=self.kpoints,
             bands=self.bands,
             projected=self._spd2projected(self.spd),
             efermi=efermi,
             kpath=kpath,
+            n_kx=n_kx,
+            n_ky=n_ky,
+            n_kz=n_kz,
             projected_phase=self._spd2projected(self.spd_phase),
             labels=self.orbitalNames[:-1],
             reciprocal_lattice=reciprocal_lattice,
 
         )
 
     def repair(self):
@@ -639,15 +690,15 @@
 
         # checking if fileName is just a path and needs a "PROCAR to " be
         # appended
         if os.path.isdir(self.filename):
             if self.filename[-1] != r"/":
                 self.filename += "/"
             self.filename += "PROCAR"
-
+        
         # checking that the file exist
         if os.path.isfile(self.filename):
             # Checking if compressed
             if self.filename[-2:] == "gz":
                 in_file = gzip.open(self.filename, mode="rt")
             else:
                 in_file = open(self.filename, "r")
```

### Comparing `PyProcar-6.0.0/pyprocar/io/vaspxml/vaspxml.py` & `PyProcar-6.1.0/pyprocar/io/vaspxml/vaspxml.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/plotter/dos_plot.py` & `PyProcar-6.1.0/pyprocar/plotter/dos_plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 __author__ = "Pedram Tavadze and Logan Lang"
 __maintainer__ = "Pedram Tavadze and Logan Lang"
 __email__ = "petavazohi@mail.wvu.edu, lllang@mix.wvu.edu"
 __date__ = "March 31, 2020"
 
+import os
+import yaml
 from typing import List
 
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pylab as plt
 from matplotlib.collections import LineCollection
 from matplotlib.ticker import MultipleLocator, FormatStrFormatter, AutoMinorLocator
 
+from pyprocar.utils import ROOT
 from ..utils.defaults import settings
 from ..core import Structure, DensityOfStates
 
 np.seterr(divide="ignore", invalid="ignore")
 
-# TODO add python typing to all of the functions
 # TODO Generalize orientation to remove if statments
 
 class DOSPlot:
     """
     Class to plot an electronic band structure.
 
     Parameters
@@ -35,44 +37,38 @@
         The default is None.
 
     Returns
     -------
     None.
 
     """
+    
     def __init__(self, 
                     dos:DensityOfStates=None, 
                     structure:Structure=None, 
                     ax:mpl.axes.Axes=None, 
                     **kwargs):
-        settings.modify(kwargs)
+        
+        with open(os.path.join(ROOT,'pyprocar','cfg','dos.yml'), 'r') as file:
+            self.plot_opt = yaml.safe_load(file)
+        self.update_config(kwargs)  
 
         self.dos = dos
         self.structure = structure
-        
-        # if spins is None:
-        #     self.spins = np.arange(self.dos.n_spins, dtype=int)
-        #     self.nspins = len(self.spins)
-        # else:
-        #     self.spins = spins
-        #     self.nspins = len(self.spins)
-
-
         self.handles = []
         self.labels = []
         if ax is None:
-            self.fig = plt.figure(figsize=tuple(settings.general.figure_size),)
+            self.fig = plt.figure(figsize=tuple(self.plot_opt['figure_size']['value']),)
             self.ax = self.fig.add_subplot(111)
         else:
             self.fig = plt.gcf()
             self.ax = ax
     
         return None
 
-
     def plot_dos(self,
                 spins:List[int]=None, 
                 orientation:str = 'horizontal'):
         """
         Plot the plain density of states.
 
         Parameters
@@ -94,73 +90,59 @@
                 spins = range(self.dos.n_spins)
         if self.dos.is_non_collinear:
             spins = [0]
 
         # plots over the different dos energies for spin polarized
         for ispin in spins:
             if orientation == 'horizontal':
-                self.set_xlabel('Energy (eV)')
-                self.set_ylabel('DOS')
+                self.set_xlabel(self.plot_opt['x_label']['value'])
+                self.set_ylabel(self.plot_opt['y_label']['value'])
                 self.set_xlim([self.dos.energies.min(),self.dos.energies.max()])
-                self.set_ylim([self.dos.total[ispin,:].min(),self.dos.total[ispin,:].max()])
-
+                self.set_ylim([self.dos.total.min(),self.dos.total.max()])
                 handle = self.ax.plot(
-                    self.dos.energies, self.dos.total[ispin, :], color=settings.dos.spin_colors[ispin], alpha=settings.dos.opacity[
-                        ispin], linestyle=settings.dos.linestyle[ispin], label=settings.dos.spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                    self.dos.energies, self.dos.total[ispin, :], 
+                    color=self.plot_opt['spin_colors']['value'][ispin], 
+                    alpha=self.plot_opt['opacity']['value'][ispin], 
+                    linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                    label=self.plot_opt['spin_labels']['value'][ispin], 
+                    linewidth=self.plot_opt['linewidth']['value'][ispin],
                 )
             elif orientation == 'vertical':
-                self.set_xlabel('DOS')
-                self.set_ylabel('Energy (eV)')
-                self.set_xlim([self.dos.total[ispin,:].min(),self.dos.total[ispin,:].max()])
+                self.set_xlabel(self.plot_opt['y_label']['value'])
+                self.set_ylabel(self.plot_opt['x_label']['value'])
+                self.set_xlim([self.dos.total.min(),self.dos.total.max()])
                 self.set_ylim([self.dos.energies.min(),self.dos.energies.max()])
                 handle = self.ax.plot(
-                        self.dos.total[ispin, :], self.dos.energies, color=settings.dos.spin_colors[ispin], alpha=settings.dos.opacity[
-                        ispin], linestyle=settings.dos.linestyle[ispin], label= settings.dos.spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                        self.dos.total[ispin, :], self.dos.energies, 
+                        color=self.plot_opt['spin_colors']['value'][ispin], 
+                        alpha=self.plot_opt['opacity']['value'][ispin], 
+                        linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                        label=self.plot_opt['spin_labels']['value'][ispin], 
+                        linewidth=self.plot_opt['linewidth']['value'][ispin],
                 )
             self.handles.append(handle)
 
     def plot_parametric(self,
                         atoms:List[int]=None,
                         orbitals:List[int]=None,
                         spins:List[int]=None,
                         principal_q_numbers:List[int]=[-1],
-                        spin_colors:List[str] or List[List[float]] =None,
-                        spin_labels:List[str]=None,
-                        cmap:str="jet",
-                        vmin:float=0,
-                        vmax:float=1,
-                        plot_total:bool=True,
-                        plot_bar:bool=True,
                         orientation:str='horizontal'):
         """The method will plot the parametric density of states
 
         Parameters
         ----------
         atoms : List[int], optional
             A list of atoms, by default None
         orbitals : List[int], optional
             A list of orbitals, by default None
         spins : List[int], optional
             A list of spins, by default None
         principal_q_numbers : List[int], optional
             A list of principal quantum numbers, by default [-1]
-        spin_colors : List[str] or List[List[float]], optional
-            List of spin colors, by default None
-        spin_labels : List[str], optional
-            A list of spin labels, by default None
-        cmap : str, optional
-            The color map to use, by default "jet"
-        vmin : float, optional
-            Value to normalize the minimum projection value., by default 0
-        vmax : float, optional
-            Value to normalize the maximum projection value., by default 1
-        plot_total : bool, optional
-            Boolean to plot the total dos, by default True
-        plot_bar : bool, optional
-            Boolean to include colorbas, by default True
         orientation : str, optional
             String to plot horizontal or vertical plot, by default 'horizontal'
         """
         if spins is None:
             if self.dos.is_non_collinear:
                 spins = [0,1,2]
             else:
@@ -170,37 +152,39 @@
         # This covers the non-colinear case when spins only represent projections.  
         if self.dos.is_non_collinear:
             spins = [0]
 
         dos_total = np.array(self.dos.total)
         dos_total_projected = self.dos.dos_sum()
         dos_projected = self.dos.dos_sum(atoms=atoms,
-                               principal_q_numbers=principal_q_numbers,
-                               orbitals=orbitals,
-                               spins=spin_projections)
-        # print(np.where(np.logical_and( self.dos.energies>-51, self.dos.energies<-50)))
-        if spin_colors is None:
-            spin_colors = settings.dos.spin_colors
-        if spin_labels is None:
-            spin_labels = settings.dos.spin_labels
+                                        principal_q_numbers=principal_q_numbers,
+                                        orbitals=orbitals,
+                                        spins=spin_projections)
 
+        if self.plot_opt['clim']['value']:
+            vmin=self.plot_opt['clim']['value'][0]
+            vmax=self.plot_opt['clim']['value'][1]
+        else:
+            vmin=None
+            vmax=None
+        cmap=self.plot_opt['cmap']['value']
         if vmin is None:
             vmin = (dos_projected.min() / dos_total_projected.max())
         if vmax is None:
             vmax = (dos_projected.max() / dos_total_projected.max())
 
         cmap = mpl.cm.get_cmap(cmap)
-        if plot_bar:
+        if self.plot_opt['plot_bar']['value']:
             norm = mpl.colors.Normalize(vmin=vmin, vmax=vmax)
             self.fig.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap), ax=self.ax)
 
 
         if orientation == 'horizontal':
-            self.set_xlabel('Energy (eV)')
-            self.set_ylabel('DOS')
+            self.set_xlabel(self.plot_opt['x_label']['value'])
+            self.set_ylabel(self.plot_opt['y_label']['value'])
             self.set_xlim([self.dos.energies.min(),self.dos.energies.max()])
 
             if len(spins) == 2:
                 self.set_ylim([-self.dos.total.max(),self.dos.total.max()])
             else:
                 self.set_ylim([0,self.dos.total.max()])
 
@@ -222,29 +206,35 @@
                     bar_color.append(cmap(y / (y_total_projected )))#* (vmax - vmin))))
 
                 for idos in range(len(x) - 1):
                     self.ax.fill_between([x[idos], x[idos + 1]],
                                     [y_total[idos], y_total[idos + 1]],
                                     color=bar_color[idos])
                 
-                if plot_total == True:
+                if self.plot_opt['plot_total']['value'] == True:
                     if spins_index == 0:
                         self.ax.plot(
-                                self.dos.energies, self.dos.total[ispin, :], color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                self.dos.energies, self.dos.total[ispin, :], color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin], 
+                                linewidth=self.plot_opt['linewidth']['value'][ispin], 
                             )
                     else:
                         self.ax.plot(
-                                self.dos.energies, -self.dos.total[ispin, :], color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                self.dos.energies, -self.dos.total[ispin, :], color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin], 
+                                linewidth=self.plot_opt['linewidth']['value'][ispin], 
                             )
 
         elif orientation == 'vertical':
-            self.set_xlabel('DOS')
-            self.set_ylabel('Energy (eV)')
+            self.set_xlabel(self.plot_opt['y_label']['value'])
+            self.set_ylabel(self.plot_opt['x_label']['value'])
 
             if len(spins) == 2:
                 self.set_xlim([-self.dos.total.max(),self.dos.total.max()])
             else:
                 self.set_xlim([0,self.dos.total.max()])
 
             for spins_index , ispin in enumerate(spins):
@@ -265,72 +255,55 @@
 
 
                 for idos in range(len(x) - 1):
                     self.ax.fill_betweenx([x[idos], x[idos + 1]],
                                     [y_total[idos], y_total[idos + 1]],
                                     color=bar_color[idos])
 
-                if plot_total == True:
+                if self.plot_opt['plot_total']['value'] == True:
                     if spins_index == 0:
                         self.ax.plot(
-                                self.dos.total[ispin, :], self.dos.energies, color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                self.dos.total[ispin, :], self.dos.energies, color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin], 
+                                linewidth=self.plot_opt['linewidth']['value'][ispin], 
                             )
                     else:
                         self.ax.plot(
-                                -self.dos.total[ispin, :], self.dos.energies, color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                -self.dos.total[ispin, :], self.dos.energies, color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin], 
+                                linewidth=self.plot_opt['linewidth']['value'][ispin], 
                             )
                     
     def plot_parametric_line(self,
                              atoms:List[int]=None,
                              spins:List[int]=None,
                              principal_q_numbers:List[int]=[-1],
                              orbitals:List[int]=None,
-                             spin_colors:List[str] or List[List[float]] =None,
-                             spin_labels:List[str]=None,
-                             vmin:float=None,
-                             vmax:float=None,
-                             plot_bar:bool=True,
-                             cmap:str='jet',
                              orientation:str="horizontal",
                              ):
         """A method to plot the parametric line plot
 
         Parameters
         ----------
         atoms : List[int], optional
             A list of atoms, by default None
         spins : List[int], optional
             A list of spins, by default None
         principal_q_numbers : List[int], optional
             A list of principal quantum numbers, by default [-1]
         orbitals : List[int], optional
             A list of orbitals, by default None
-        spin_colors : List[str] or List[List[float]], optional
-            A list of spins colors, by default None
-        spin_labels : List[str], optional
-            A list of spin labels, by default None
-        vmin : float, optional
-            Value to normalize the minimum projection value., by default None
-        vmax : float, optional
-            Value to normalize the mmaximum projection value., by default None
-        plot_bar : bool, optional
-            Boolean to plot the colorbar, by default True
-        cmap : str, optional
-            The colormap to use, by default 'jet'
         orientation : str, optional
             String to plot vertical or horizontal, by default "horizontal"
         """
 
-        if spin_colors is None:
-            spin_colors = settings.dos.spin_colors
-        if spin_labels is None:
-            spin_labels = settings.dos.spin_labels
-
         if spins is None:
             if self.dos.is_non_collinear:
                 spins = [0,1,2]
             else:
                 spins = range(self.dos.n_spins)
         spin_projections = spins
         # This covers the non-colinear case when spins only represent projections.  
@@ -341,109 +314,101 @@
         dos_projected = self.dos.dos_sum(atoms=atoms,
                                principal_q_numbers=principal_q_numbers,
                                orbitals=orbitals,
                                spins=spin_projections)
 
         projections_weights = np.divide(dos_projected,dos_total_projected)
 
+
+        if self.plot_opt['clim']['value']:
+            vmin=self.plot_opt['clim']['value'][0]
+            vmax=self.plot_opt['clim']['value'][1]
+        else:
+            vmin=None
+            vmax=None
+        cmap=self.plot_opt['cmap']['value']
         if vmin is None:
             vmin = (dos_projected.min() / dos_total_projected.max())
         if vmax is None:
             vmax = (dos_projected.max() / dos_total_projected.max())
-        if plot_bar:
+        if self.plot_opt['plot_bar']['value']:
             norm = mpl.colors.Normalize(vmin=vmin, vmax=vmax)
             self.fig.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap), ax=self.ax)
 
         if orientation == 'horizontal':
 
-            self.set_xlabel('Energy (eV)')
-            self.set_ylabel('DOS')
+            self.set_xlabel(self.plot_opt['x_label']['value'])
+            self.set_ylabel(self.plot_opt['y_label']['value'])
             self.set_xlim([self.dos.energies.min(),self.dos.energies.max()])
             if len(spins) == 2:
                 self.set_ylim([-self.dos.total.max(),self.dos.total.max()])
             else:
                 self.set_ylim([0,self.dos.total.max()])
 
             for spins_index , ispin in enumerate(spins):
                 if len(spins)>1 and spins_index:
                     points = np.array( [self.dos.energies, -1 * self.dos.total[ispin, :]]).T.reshape(-1, 1, 2)
                 else:
                     points = np.array( [self.dos.energies, self.dos.total[ispin, :]]).T.reshape(-1, 1, 2)
 
                 segments = np.concatenate([points[:-1], points[1:]], axis=1)
-                lc = LineCollection(segments, cmap=plt.get_cmap(settings.ebs.color_map), norm=norm)
+                lc = LineCollection(segments, cmap=plt.get_cmap(self.plot_opt['cmap']['value']), norm=norm)
                 lc.set_array(projections_weights[ispin,:])
                 handle = self.ax.add_collection(lc)
                 
-                lc.set_linewidth(settings.dos.linewidth[ispin])
-                lc.set_linestyle(settings.dos.linestyle[ispin])
+                lc.set_linewidth(self.plot_opt['linewidth']['value'][ispin])
+                lc.set_linestyle(self.plot_opt['linestyle']['value'][ispin])
 
                 self.handles.append(handle)
 
         elif orientation == 'vertical':
-            self.set_xlabel('DOS')
-            self.set_ylabel('Energy (eV)')
+            self.set_xlabel(self.plot_opt['y_label']['value'])
+            self.set_ylabel(self.plot_opt['x_label']['value'])
 
             if len(spins) == 2:
                 self.set_xlim([-self.dos.total.max(),self.dos.total.max()])
             else:
                 self.set_xlim([0,self.dos.total.max()])
 
             for spins_index , ispin in enumerate(spins):
                 if len(spins)>1 and spins_index:
                     points = np.array( [ -1 * self.dos.total[ispin, :], self.dos.energies]).T.reshape(-1, 1, 2)
                 else:
                     points = np.array( [self.dos.total[ispin, :], self.dos.energies]).T.reshape(-1, 1, 2)
 
                 segments = np.concatenate([points[:-1], points[1:]], axis=1)
-                lc = LineCollection(segments, cmap=plt.get_cmap(settings.ebs.color_map), norm=norm)
+                lc = LineCollection(segments, cmap=plt.get_cmap(self.plot_opt['cmap']['value']), norm=norm)
                 lc.set_array(projections_weights[ispin,:])
                 handle = self.ax.add_collection(lc)
                 
-                lc.set_linewidth(settings.dos.linewidth[ispin])
-                lc.set_linestyle(settings.dos.linestyle[ispin])
+                lc.set_linewidth(self.plot_opt['linewidth']['value'][ispin])
+                lc.set_linestyle(self.plot_opt['linestyle']['value'][ispin])
                 self.handles.append(handle)
 
     def plot_stack_species(
             self,
             principal_q_numbers:List[int]=[-1],
             orbitals:List[int]=None,
             spins:List[int]=None,
-            spin_colors:List[str] or List[List[float]] =None,
-            spin_labels:List[str] = None,
-            colors:List[str] or List[List[float]] =None,
-            plot_total:bool=False,
             orientation:str="horizontal",
         ):
         """A method to plot the dos with the species contribution stacked on eachother
 
         Parameters
         ----------
         principal_q_numbers : List[int], optional
             A list of principal quantum numbers, by default [-1]
         orbitals : List[int], optional
             A list of orbitals, by default None
         spins : List[int], optional
             A list of spins, by default None
-        spin_colors : List[str] or List[List[float]], optional
-            A list of spin colors, by default None
-        spin_labels : List[str], optional
-            A list of spin labels, by default None
-        colors : List[str] or List[List[float]], optional
-            A list of colors, by default None
-        plot_total : bool, optional
-            Boolean to plot the total dos, by default False
         orientation : str, optional
             String to plot horizontal or vertical plot, by default "horizontal"
         """
         
-        if spin_colors is None:
-            spin_colors = settings.dos.spin_colors
-        if spin_labels is None:
-            spin_labels = settings.dos.spin_labels
 
         if spins is None:
             spins = range(self.dos.n_spins)
             if self.dos.is_non_collinear:
                 spins = [0,1,2]
             else:
                 spins = range(self.dos.n_spins)
@@ -489,24 +454,22 @@
                 if len(self.dos.projected[0][0]) == 1 + 3 + 5:
                     label = "-spd"
                 elif len(self.dos.projected[0][0]) == 1 + 3 + 5 + 7:
                     label = "-spdf"
                 else:
                     label = "-"
 
-        if colors is None:
-            colors = settings.dos.colors
 
         dos_total = self.dos.total
         dos_projected_total = self.dos.dos_sum()
 
 
         if orientation == 'horizontal':
-            self.set_xlabel('Energy (eV)')
-            self.set_ylabel('DOS Cumlative')
+            self.set_xlabel(self.plot_opt['x_label']['value'])
+            self.set_ylabel(self.plot_opt['stack_y_label']['value'])
             self.set_xlim([self.dos.energies.min(),self.dos.energies.max()])
             self.set_ylim([self.dos.total.min(),self.dos.total.max()])
             if len(spins) == 1:
                 self.set_ylim([0,self.dos.total.max()])
             else:
                 self.set_ylim([-self.dos.total.max(),self.dos.total.max()])
 
@@ -526,44 +489,50 @@
                     y = (dos_projected[ispin]  / dos_projected_total[ispin] ) * dos_total[ispin]
 
                     if ispin > 0 and len(spins) > 1:
                         y *= -1
                         handle = self.ax.fill_between(x,
                                         bottom + y,
                                         bottom,
-                                        color=colors[specie],
+                                        color=self.plot_opt['colors']['value'][specie],
                                         )
                     else:
                         handle = self.ax.fill_between(
                             x,
                             bottom + y,
                             bottom,
-                            color=colors[specie],
+                            color=self.plot_opt['colors']['value'][specie],
                         )
                     self.handles.append(handle)
-                    self.labels.append(self.structure.species[specie] + label + spin_labels[ispin])
+                    label=self.structure.species[specie] + label + self.plot_opt['spin_labels']['value'][ispin]
+                    self.labels.append(label)
                     bottom += y
 
-                if plot_total == True:
                     if spins_index == 0:
                         self.ax.plot(
-                                self.dos.energies, self.dos.total[ispin, :], color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                self.dos.energies, self.dos.total[ispin, :], color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin],
+                                linewidth=self.plot_opt['linewidth']['value'][ispin],
                             )
                     else:
                         self.ax.plot(
-                                self.dos.energies, -self.dos.total[ispin, :], color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                self.dos.energies, -self.dos.total[ispin, :], color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin],
+                                linewidth=self.plot_opt['linewidth']['value'][ispin],
                             )
 
 
 
         elif orientation == 'vertical':
-            self.set_xlabel('DOS Cumlative')
-            self.set_ylabel('Energy (eV)')
+            self.set_xlabel(self.plot_opt['stack_y_label']['value'])
+            self.set_ylabel(self.plot_opt['x_label']['value'])
             self.set_xlim([self.dos.total.min(),self.dos.total.max()])
             if len(spins) == 1:
                 self.set_xlim([0,self.dos.total.max()])
             else:
                 self.set_xlim([-self.dos.total.max(),self.dos.total.max()])
             self.set_ylim([self.dos.energies.min(),self.dos.energies.max()])
 
@@ -583,77 +552,65 @@
                     y = (dos[ispin] * dos_total[ispin]) / dos_projected_total[ispin]
 
                     if ispin > 0 and len(spins) > 1:
                         y *= -1
                         handle = self.ax.fill_betweenx(x,
                                         bottom + y,
                                         bottom,
-                                        color=colors[specie],
+                                        color=self.plot_opt['colors']['value'][specie],
                                         )
                     else:
                          handle = self.ax.fill_betweenx(x,
                                         bottom + y,
                                         bottom,
-                                        color=colors[specie],
+                                        color=self.plot_opt['colors']['value'][specie],
                                         )
                     self.handles.append(handle)
-                    self.labels.append(self.structure.species[specie] + label + spin_labels[ispin])     
+                    label=self.structure.species[specie] + label + self.plot_opt['spin_labels']['value'][ispin]
+                    self.labels.append(label)     
                     bottom += y 
 
-                if plot_total == True:
+                if self.plot_opt['plot_total']['value'] == True:
                     if spins_index == 0:
                         self.ax.plot(
-                                self.dos.total[ispin, :], self.dos.energies, color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                self.dos.total[ispin, :], self.dos.energies, color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin],
+                                linewidth=self.plot_opt['linewidth']['value'][ispin],
                             )
                     else:
                         self.ax.plot(
-                                -self.dos.total[ispin, :], self.dos.energies,color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                -self.dos.total[ispin, :], self.dos.energies,color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin],
+                                linewidth=self.plot_opt['linewidth']['value'][ispin],
                             )
 
-
     def plot_stack_orbitals(self,
             atoms:List[int]=None,
             spins:List[int]=None,
             principal_q_numbers:List[int]=[-1],
-            spin_colors:List[str] or List[List[float]] =None,
-            spin_labels:List[str] = None,
-            colors:List[str] or List[List[float]] =None,
-            plot_total:bool= True,
             orientation:str="horizontal",
         ):
         """A method to plot dos orbitals contribution stacked.
 
         Parameters
         ----------
         atoms : List[int], optional
             A list of atoms, by default None
         spins : List[int], optional
             A list of spins, by default None
         principal_q_numbers : List[int], optional
             A list of principal quantum numbers, by default [-1]
-        spin_colors : List[str] or List[List[float]], optional
-            A list of spin colors, by default None
-        spin_labels : List[str], optional
-            A list of spin labels, by default None
-        colors : List[str] or List[List[float]], optional
-            A list of colors, by default None
-        plot_total : bool, optional
-            Boolean to plot the total dos, by default True
         orientation : str, optional
             String to plot horizontal or vertical, by default "horizontal"
         """
 
-
-        if spin_colors is None:
-            spin_colors = settings.dos.spin_colors
-        if spin_labels is None:
-            spin_labels = settings.dos.spin_labels
-
         if spins is None:
             spins = range(self.dos.n_spins)
             if self.dos.is_non_collinear:
                 spins = [0,1,2]
             else:
                 spins = range(self.dos.n_spins)
         spin_projections = spins
@@ -678,23 +635,21 @@
         if self.dos.is_non_collinear and len(self.dos.projected[0][0]) == 2 + 2 + 4 + 4 + 6:
             orb_names = ["s-j=0.5", "p-j=0.5", "p-j=1.5", "d-j=1.5", "d-j=2.5"]
             orb_l = [[0,1], [2,3], [4, 5, 6, 7], [8,9,10,11], [12,13,14,15,16,17]]
         else:
             orb_names = ["s", "p", "d"]
             orb_l = [[0], [1, 2, 3], [4, 5, 6, 7, 8]]
 
-        if colors is None:
-            colors = settings.dos.colors
-        
+
         dos_total = self.dos.total
         dos_projected_total = self.dos.dos_sum()
 
         if  orientation == 'horizontal':
-            self.set_xlabel('Energy (eV)')
-            self.set_ylabel('DOS Cumlative')
+            self.set_xlabel(self.plot_opt['x_label']['value'])
+            self.set_ylabel(self.plot_opt['stack_y_label']['value'])
             self.set_xlim([self.dos.energies.min(),self.dos.energies.max()])
             self.set_ylim([self.dos.total.min(),self.dos.total.max()])
             if len(spins) == 1:
                 self.set_ylim([0,self.dos.total.max()])
             else:
                 self.set_ylim([-self.dos.total.max(),self.dos.total.max()])
 
@@ -712,38 +667,44 @@
                     y = np.nan_to_num(y, 0)
 
                     if ispin > 0 and len(spins) > 1:
                         y *= -1
                         handle =  self.ax.fill_between(x,
                                         bottom + y,
                                         bottom,
-                                        color=colors[iorb])
+                                        color=self.plot_opt['colors']['value'][iorb])
                         
                     else:
                         handle = self.ax.fill_between(
                             x,
                             bottom + y,
                             bottom,
-                            color=colors[iorb],
+                            color=self.plot_opt['colors']['value'][iorb],
                         )
                         
 
-                    self.labels.append(atom_names + orb_names[iorb] + spin_labels[ispin])
+                    self.labels.append(atom_names + orb_names[iorb] + self.plot_opt['spin_labels']['value'][ispin])
                     self.handles.append(handle)
                     bottom += y
-            if plot_total == True:
+            if self.plot_opt['plot_total']['value'] == True:
                 if ispin == 0:
                     self.ax.plot(
-                            self.dos.energies, self.dos.total[ispin, :], color= 'black', alpha=settings.dos.opacity[ispin], 
-                            linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                            self.dos.energies, self.dos.total[ispin, :], color= 'black', 
+                            alpha=self.plot_opt['opacity']['value'][ispin], 
+                            linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                            label=self.plot_opt['spin_labels']['value'][ispin],
+                            linewidth=self.plot_opt['linewidth']['value'][ispin],
                         )
                 else:
                     self.ax.plot(
-                            self.dos.energies, -self.dos.total[ispin, :], color= 'black', alpha=settings.dos.opacity[ispin], 
-                            linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                            self.dos.energies, -self.dos.total[ispin, :], color= 'black', 
+                            alpha=self.plot_opt['opacity']['value'][ispin], 
+                            linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                            label=self.plot_opt['spin_labels']['value'][ispin],
+                            linewidth=self.plot_opt['linewidth']['value'][ispin],
                         )
 
         elif orientation == 'vertical':
             self.set_xlabel('DOS Cumlative')
             self.set_ylabel('Energy (eV)')
             self.set_xlim([self.dos.total.min(),self.dos.total.max()])
             if len(spins) == 1:
@@ -766,79 +727,70 @@
                     y = np.nan_to_num(y, 0)
 
                     if ispin > 0 and len(spins) > 1:
                         y *= -1
                         handle =  self.ax.fill_betweenx(x,
                                         bottom + y,
                                         bottom,
-                                        color=colors[iorb])
+                                        color=self.plot_opt['colors']['value'][iorb])
                         
                     else:
                         handle = self.ax.fill_betweenx(
                             x,
                             bottom + y,
                             bottom,
-                            color=colors[iorb],
+                            color=self.plot_opt['colors']['value'][iorb],
                         )
                         
 
-                    self.labels.append(atom_names + orb_names[iorb] + spin_labels[ispin])
+                    self.labels.append(atom_names + orb_names[iorb] + self.plot_opt['spin_labels']['value'][ispin])
                     self.handles.append(handle)
                     bottom += y
-            if plot_total == True:
+            if self.plot_opt['plot_total']['value'] == True:
                 if ispin == 0:
                     self.ax.plot(
-                            self.dos.total[ispin, :], self.dos.energies, color= 'black', alpha=settings.dos.opacity[ispin], 
-                            linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                            self.dos.total[ispin, :], self.dos.energies, color= 'black', 
+                            alpha=self.plot_opt['opacity']['value'][ispin], 
+                            linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                            label=self.plot_opt['spin_labels']['value'][ispin],
+                            linewidth=self.plot_opt['linewidth']['value'][ispin],
                         )
                 else:
                     self.ax.plot(
-                            -self.dos.total[ispin, :], self.dos.energies, color= 'black', alpha=settings.dos.opacity[ispin], 
-                            linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                            -self.dos.total[ispin, :], self.dos.energies, color= 'black', 
+                            alpha=self.plot_opt['opacity']['value'][ispin], 
+                            linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                            label=self.plot_opt['spin_labels']['value'][ispin],
+                            linewidth=self.plot_opt['linewidth']['value'][ispin],
                         )
             
     def plot_stack(self,
                 items:dict=None,
                 spins:List[int]=None,
-                spin_colors:List[str] or List[List[float]] =None,
-                spin_labels:List[str]=None,
-                colors:List[str] or List[List[float]] =None,
                 plot_total:bool= True,
                 orientation:str='horizontal',
         ):
         """A method to plot dos contributions stacked.
 
         Parameters
         ----------
         items : dict, optional
             A dictionary where the keys represent the atom and the 
             values are the orbital contributions to include for that item, by default None
         spins : List[int], optional
             A list of spins, by default None
-        spin_colors : List[str] or List[List[float]], optional
-            A list of spin colors, by default None
-        spin_labels : List[str], optional
-            A list of spin labels, by default None
-        colors : List[str] or List[List[float]], optional
-            A list of colors, by default None
-        plot_total : bool, optional
-            Boolean to plot the total dos, by default True
         orientation : str, optional
             String to plot horizontal or vertical, by default "horizontal"
         """
             
         if len(items) is None:
             print("""Please provide the stacking items in which you want
                 to plot, example : {'Sr':[1,2,3],'O':[4,5,6,7,8]}
                 will plot the stacked plots of p orbitals of Sr and
                 d orbitals of Oxygen.""")
-        if spin_colors is None:
-            spin_colors = settings.dos.spin_colors
-        if spin_labels is None:
-            spin_labels = settings.dos.spin_labels
         
         if spins is None:
             spins = range(self.dos.n_spins)
             if self.dos.is_non_collinear:
                 spins = [0,1,2]
             else:
                 spins = range(self.dos.n_spins)
@@ -855,29 +807,27 @@
             if len(self.dos.projected[0][0]) == (1 + 3 + 5):
                 all_orbitals = "spd"
             elif len(self.dos.projected[0][0]) == (1 + 3 + 5 + 7):
                 all_orbitals = "spdf"
             else:
                 all_orbitals = ""
 
-        if colors is None:
-            colors = settings.dos.colors
         counter = 0
         colors_dict = {}
         for specie in items:
-            colors_dict[specie] = colors[counter]
+            colors_dict[specie] = self.plot_opt['colors']['value'][counter]
             counter += 1
         
         
         dos_total = self.dos.total
         dos_projected_total = self.dos.dos_sum()
 
         if orientation=='horizontal':
-            self.set_xlabel('Energy (eV)')
-            self.set_ylabel('DOS Cumlative')
+            self.set_xlabel(self.plot_opt['x_label']['value'])
+            self.set_ylabel(self.plot_opt['stack_y_label']['value'])
             self.set_xlim([self.dos.energies.min(),self.dos.energies.max()])
             self.set_ylim([self.dos.total.min(),self.dos.total.max()])
             if self.dos.n_spins == 2:
                 self.set_ylim([-self.dos.total.max(),self.dos.total.max()])
             else:
                 self.set_ylim([0,self.dos.total.max()])
 
@@ -935,31 +885,37 @@
                         handle = self.ax.fill_between(
                                 x,
                                 bottom + y,
                                 bottom,
                                 color=colors_dict[specie],
                             )
                     self.handles.append(handle)
-                    self.labels.append(specie + label + spin_labels[ispin])
+                    self.labels.append(specie + label + self.plot_opt['spin_labels']['value'][ispin])
                     bottom += y
                 if plot_total == True:
                     if ispin == 0:
                         self.ax.plot(
-                                self.dos.energies, self.dos.total[ispin, :], color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                self.dos.energies, self.dos.total[ispin, :], color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin],
+                                linewidth=self.plot_opt['linewidth']['value'][ispin],
                             )
                     else:
                         self.ax.plot(
-                                    self.dos.energies, -self.dos.total[ispin, :], color= 'black', alpha=settings.dos.opacity[ispin], 
-                                    linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                    self.dos.energies, -self.dos.total[ispin, :], color= 'black', 
+                                    alpha=self.plot_opt['opacity']['value'][ispin], 
+                                    linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                    label=self.plot_opt['spin_labels']['value'][ispin],
+                                    linewidth=self.plot_opt['linewidth']['value'][ispin],
                                 )
 
         elif orientation=='vertical':
-            self.set_xlabel('DOS Cumlative')
-            self.set_ylabel('Energy (eV)')
+            self.set_xlabel(self.plot_opt['stack_y_label']['value'])
+            self.set_ylabel(self.plot_opt['x_label']['value'])
             self.set_xlim([self.dos.total.min(),self.dos.total.max()])
             if self.dos.n_spins == 2:
                 self.set_xlim([-self.dos.total.max(),self.dos.total.max()])
             else:
                 self.set_xlim([0,self.dos.total.max()])
                 
             self.set_ylim([self.dos.energies.min(),self.dos.energies.max()])
@@ -1015,35 +971,39 @@
                                         bottom,
                                         color=colors_dict[specie])
                     else:
                         handle = self.ax.fill_betweenx(
                                 x,
                                 bottom + y,
                                 bottom,
-                                color=colors_dict[specie],
+                                color=self.plot_opt['colors']['value'][specie],
                             )
                     self.handles.append(handle)
-                    self.labels.append(specie + label + spin_labels[ispin])
+                    self.labels.append(specie + label + self.plot_opt['spin_labels']['value'][ispin])
                     bottom += y
 
                 if plot_total == True:
                     if ispin == 0:
                         self.ax.plot(
-                                self.dos.total[ispin, :], self.dos.energies, color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                self.dos.total[ispin, :], self.dos.energies, color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin],
+                                linewidth=self.plot_opt['linewidth']['value'][ispin],
                             )
                     else:
                         self.ax.plot(
-                                -self.dos.total[ispin, :], self.dos.energies, color= 'black', alpha=settings.dos.opacity[ispin], 
-                                linestyle=settings.dos.linestyle[ispin], label=spin_labels[ispin], linewidth=settings.dos.linewidth[ispin],
+                                -self.dos.total[ispin, :], self.dos.energies, color= 'black', 
+                                alpha=self.plot_opt['opacity']['value'][ispin], 
+                                linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                                label=self.plot_opt['spin_labels']['value'][ispin],
+                                linewidth=self.plot_opt['linewidth']['value'][ispin],
                             )
         return None
 
-
-
     def set_xticks(self, 
                 tick_positions:List[int]=None, 
                 tick_names:List[str]=None):
         """A method to set the xticks of the plot
 
         Parameters
         ----------
@@ -1055,14 +1015,15 @@
         """
 
         if tick_positions is not None:
             self.ax.set_xticks(tick_positions)
         if tick_names is not None:
             self.ax.set_xticklabels(tick_names)
         return None
+    
     def set_yticks(self,  
                     tick_positions:List[int]=None, 
                     tick_names:List[str]=None):
         """A method to set the yticks of the plot
 
         Parameters
         ----------
@@ -1178,28 +1139,29 @@
             None
         """
         if orientation == 'horizontal':
             self.ax.axvline(x=0, color=color, linestyle=linestyle, linewidth=linewidth)
         elif orientation == 'vertical':
             self.ax.axhline(y=0, color=color, linestyle=linestyle, linewidth=linewidth)
         return None
+    
     def grid(self):
         """A method to include a grid on the plot.
 
         Returns
         -------
         None
             None
         """
         self.ax.grid(
-            settings.dos.grid,
-            which=settings.dos.grid_which,
-            color=settings.dos.grid_color,
-            linestyle=settings.dos.grid_linestyle,
-            linewidth=settings.dos.grid_linewidth)
+            self.plot_opt['grid']['value'],
+            which=self.plot_opt['grid_which']['value'],
+            color=self.plot_opt['grid_color']['value'],
+            linestyle=self.plot_opt['grid_linestyle']['value'],
+            linewidth=self.plot_opt['grid_linewidth']['value'])
         return None
 
     def show(self):
         """A method to show the plot
 
         Returns
         -------
@@ -1220,13 +1182,16 @@
 
         Returns
         -------
         None
             None
         """
 
-        plt.savefig(filename, bbox_inches="tight")
+        plt.savefig(filename,dpi=self.plot_opt['dpi']['value'], bbox_inches="tight")
         plt.clf()
         return None
     
-        
+    def update_config(self, config_dict):
+        for key,value in config_dict.items():
+            self.plot_opt[key]['value']=value
+
```

### Comparing `PyProcar-6.0.0/pyprocar/plotter/ebs_plot.py` & `PyProcar-6.1.0/pyprocar/plotter/ebs_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 __author__ = "Pedram Tavadze and Logan Lang"
 __maintainer__ = "Pedram Tavadze and Logan Lang"
 __email__ = "petavazohi@mail.wvu.edu, lllang@mix.wvu.edu"
 __date__ = "March 31, 2020"
 
+import os 
+import yaml
 from typing import List
 
 import numpy as np
 
 import matplotlib.pyplot as plt
 from matplotlib.collections import LineCollection
 import matplotlib as mpl
 from matplotlib.ticker import MultipleLocator, FormatStrFormatter, AutoMinorLocator
 
-from ..utils.defaults import settings
+from ..utils import ROOT
 from ..core import ElectronicBandStructure, KPath
 
+
 class EBSPlot:
     """
     A class to plot an electronic band structure.
 
     Parameters
     ----------
     ebs : ElectronicBandStructure
@@ -40,28 +43,30 @@
     def __init__(self, 
                     ebs:ElectronicBandStructure, 
                     kpath:KPath=None, 
                     ax:mpl.axes.Axes=None, 
                     spins:List[int]=None, 
                     **kwargs):
 
-        
+        with open(os.path.join(ROOT,'pyprocar','cfg','band_structure.yml'), 'r') as file:
+            self.plot_opt = yaml.safe_load(file)
+        self.update_config(kwargs)
+
         self.ebs = ebs
         self.kpath = kpath
         self.spins = spins
         if self.spins is None:
             self.spins = range(self.ebs.nspins)
         self.nspins = len(self.spins)
         if self.ebs.is_non_collinear:
             self.spins = [0]
         self.handles = []
-        settings.modify(kwargs)
 
         
-        figsize=tuple(settings.general.figure_size)
+        figsize=tuple(self.plot_opt['figure_size']['value'])
         if ax is None:
             self.fig = plt.figure(figsize=figsize)
             self.ax = self.fig.add_subplot(111)
         else:
             self.fig = plt.gcf()
             self.ax = ax
         # need to initiate kpath if kpath is not defined.
@@ -87,15 +92,14 @@
         Returns
         -------
         np.ndarray
             x-axis data.
 
         """
         pos = 0
-
         if self.kpath is not None and self.kpath.nsegments == len(self.kpath.ngrids):
             for isegment in range(self.kpath.nsegments):
                 kstart, kend = self.kpath.special_kpoints[isegment]
 
                 distance = np.linalg.norm(kend - kstart)
                 if isegment == 0:
                     x = np.linspace(pos, pos + distance,
@@ -118,159 +122,153 @@
         Plot the plain band structure.
 
         Returns
         -------
         None.
 
         """
+
         
         for ispin in self.spins:
+            if len(self.spins)==1:
+                color=self.plot_opt['color']['value']
+            else:
+                color=self.plot_opt['spin_colors']['value'][ispin]
+            
             for iband in range(self.ebs.nbands):
                 handle = self.ax.plot(
-                    self.x, self.ebs.bands[:, iband, ispin], color=settings.ebs.color[ispin], alpha=settings.ebs.opacity[
-                        ispin], linestyle=settings.ebs.linestyle[ispin], label=settings.ebs.label[ispin], linewidth=settings.ebs.linewidth[ispin],
+                    self.x, self.ebs.bands[:, iband, ispin], 
+                    color=color, 
+                    alpha=self.plot_opt['opacity']['value'][ispin], 
+                    linestyle=self.plot_opt['linestyle']['value'][ispin], 
+                    label=self.plot_opt['label']['value'][ispin], 
+                    linewidth=self.plot_opt['linewidth']['value'][ispin],
                 )
                 self.handles.append(handle)
 
-
-    # def plot_order(self):
-    #     for ispin in range(self.ebs.bands.shape[2]):
-    #         for iband in range(self.ebs.nbands):
-    #             self.ax.plot(
-    #                 self.x, self.ebs.bands[:, iband, ispin], alpha=self.opacities[
-    #                     ispin],  linewidth=self.linewidths[ispin],
-    #             )
-
-
     def plot_scatter(self,
                      width_mask:np.ndarray=None,
                      color_mask:np.ndarray=None,
-                     vmin:float=None,
-                     vmax:float=None,
                      spins:List[int]=None,
                      width_weights:np.ndarray=None,
                      color_weights:np.ndarray=None,
                      ):
         """A method to plot a scatter plot
 
         Parameters
         ----------
         width_mask : np.ndarray, optional
             The width mask, by default None
         color_mask : np.ndarray, optional
             The color mask, by default None
-        vmin : float, optional
-            Value to normalize the minimum projection value., by default None
-        vmax : float, optional
-            Value to normalize the maximum projection value., by default None
         spins : List[int], optional
             A list of spins, by default None
         width_weights : np.ndarray, optional
             The width weight of each point, by default None
         color_weights : np.ndarray, optional
             The color weights at each point, by default None
         """
         if spins is None:
             spins = range(self.ebs.nspins)
         if self.ebs.is_non_collinear:
             spins = [0]
         
         if width_weights is None:
             width_weights = np.ones_like(self.ebs.bands)
-            markersize = settings.ebs.markersize
+            markersize = self.plot_opt['markersize']['value']
         else:
-            markersize =[l*30 for l in settings.ebs.markersize]
+            markersize =[l*30 for l in self.plot_opt['markersize']['value']]
 
 
         if width_mask is not None or color_mask is not None:
             if width_mask is not None:
                 mbands = np.ma.masked_array(
                     self.ebs.bands, np.abs(width_weights) < width_mask)
             if color_mask is not None:
                 mbands = np.ma.masked_array(
                     self.ebs.bands, np.abs(color_weights) < color_mask)
         else:
             # Faking a mask, all elemtnet are included
             mbands = np.ma.masked_array(self.ebs.bands, False)
 
         if color_weights is not None:
+            vmin=self.plot_opt['clim']['value'][0]
+            vmax=self.plot_opt['clim']['value'][1]
             if vmin is None: 
                 vmin = color_weights.min()
             if vmax is None:
                 vmax = color_weights.max()
 
         for ispin in spins:
             for iband in range(self.ebs.nbands):
+                if len(self.spins)==1:
+                    color=self.plot_opt['color']['value']
+                else:
+                    color=self.plot_opt['spin_colors']['value'][ispin]
                 if color_weights is None:
                     sc = self.ax.scatter(
                         self.x,
                         mbands[:, iband, ispin],
-                        c=settings.ebs.color[ispin],
+                        c=color,
                         s=width_weights[:, iband, ispin].round(
                             2)*markersize[ispin],
                         # edgecolors="none",
-                        linewidths=settings.ebs.linewidth[ispin],
-                        cmap=settings.ebs.color_map,
+                        linewidths=self.plot_opt['linewidth']['value'][ispin],
+                        cmap=self.plot_opt['cmap']['value'],
                         vmin=vmin,
                         vmax=vmax,
-                        marker=settings.ebs.marker[ispin],
-                        alpha=settings.ebs.opacity[ispin],
+                        marker=self.plot_opt['marker']['value'][ispin],
+                        alpha=self.plot_opt['opacity']['value'][ispin],
                     )
                 else:
                     sc = self.ax.scatter(
                         self.x,
                         mbands[:, iband, ispin],
                         c=color_weights[:, iband, ispin].round(2),
                         s=width_weights[:, iband, ispin].round(2)*markersize[ispin],
                         # edgecolors="none",
-                        linewidths=settings.ebs.linewidth[ispin],
-                        cmap=settings.ebs.color_map,
+                        linewidths=self.plot_opt['linewidth']['value'][ispin],
+                        cmap=self.plot_opt['cmap']['value'],
                         vmin=vmin,
                         vmax=vmax,
-                        marker=settings.ebs.marker[ispin],
-                        alpha=settings.ebs.opacity[ispin],
+                        marker=self.plot_opt['marker']['value'][ispin],
+                        alpha=self.plot_opt['opacity']['value'][ispin],
                     )
-        if settings.ebs.plot_color_bar and color_weights is not None:
+        if self.plot_opt['plot_color_bar']['value'] and color_weights is not None:
             cb = self.fig.colorbar(sc, ax=self.ax)
             cb.ax.tick_params(labelsize=20)
 
     def plot_parameteric(
         self,
         spins:List[int]=None,
-        vmin:float=None,
-        vmax:float=None,
         width_mask:np.ndarray=None,
         color_mask:np.ndarray=None,
         width_weights:np.ndarray=None,
         color_weights:np.ndarray=None,
         ):
         """A method to plot a scatter plot
 
         Parameters
         ----------
         spins : List[int], optional
             A list of spins, by default None
-        vmin : float, optional
-            Value to normalize the minimum projection value., by default None
-        vmax : float, optional
-            Value to normalize the maximum projection value., by default None
         width_mask : np.ndarray, optional
             The width mask, by default None
         color_mask : np.ndarray, optional
             The color mask, by default None
         width_weights : np.ndarray, optional
             The width weight of each point, by default None
         color_weights : np.ndarray, optional
             The color weights at each point, by default None
         """
         if width_weights is None:
             width_weights = np.ones_like(self.ebs.bands)
-            linewidth = settings.ebs.linewidth
+            linewidth = self.plot_opt['linewidth']['value']
         else:
-            linewidth = [l*5 for l in settings.ebs.linewidth]
+            linewidth = [l*5 for l in self.plot_opt['linewidth']['value']]
 
         if spins is None:
             spins = range(self.ebs.nspins)
         if self.ebs.is_non_collinear:
             spins = [0]
         
         
@@ -282,85 +280,85 @@
                 mbands = np.ma.masked_array(
                     self.ebs.bands, np.abs(color_weights) < color_mask)
         else:
             # Faking a mask, all elemtnet are included
             mbands = np.ma.masked_array(self.ebs.bands, False)
 
         if color_weights is not None:
-
+            vmin=self.plot_opt['clim']['value'][0]
+            vmax=self.plot_opt['clim']['value'][1]
             if vmin is None:
                 vmin = color_weights.min()
             if vmax is None:
                 vmax = color_weights.max()
                 
             norm = mpl.colors.Normalize(vmin, vmax)
 
         for ispin in spins:
             for iband in range(self.ebs.nbands):
+                if len(self.spins)==1:
+                    color=self.plot_opt['color']['value']
+                else:
+                    color=self.plot_opt['spin_colors']['value'][ispin]
                 points = np.array(
                     [self.x, mbands[:, iband, ispin]]).T.reshape(-1, 1, 2)
                 segments = np.concatenate([points[:-1], points[1:]], axis=1)
                 
                 # this is to delete the segments on the high sym points
                 x = self.x
                 # segments = np.delete(
                 #     segments, np.where(x[1:] == x[:-1])[0], axis=0)
                 if color_weights is None:
                     lc = LineCollection(
-                        segments, colors=settings.ebs.color[ispin], linestyle=settings.ebs.linestyle[ispin])
+                        segments, colors=color, 
+                        linestyle=self.plot_opt['linestyle']['value'][ispin])
                 else:
                     lc = LineCollection(
-                        segments, cmap=plt.get_cmap(settings.ebs.color_map), norm=norm)
+                        segments, cmap=plt.get_cmap(self.plot_opt['cmap']['value']), norm=norm)
                     lc.set_array(color_weights[:, iband, ispin])
                 lc.set_linewidth(
                     width_weights[:, iband, ispin]*linewidth[ispin])
-                lc.set_linestyle(settings.ebs.linestyle[ispin])
+                lc.set_linestyle(self.plot_opt['linestyle']['value'][ispin])
                 handle = self.ax.add_collection(lc)
             # if color_weights is not None:
             #     handle.set_color(color_map[iweight][:-1].lower())
             handle.set_linewidth(linewidth)
             self.handles.append(handle)
 
-        if settings.ebs.plot_color_bar and color_weights is not None:
+        if self.plot_opt['plot_color_bar']['value'] and color_weights is not None:
             cb = self.fig.colorbar(lc, ax=self.ax)
             cb.ax.tick_params(labelsize=20)
 
     def plot_parameteric_overlay(self,
                                  spins:List[int]=None,
-                                 vmin:float=None,
-                                 vmax:float=None,
                                  weights:np.ndarray=None,
-                                 plot_color_bar:bool=False,
                                  ):
         """A method to plot the parametric overlay
 
         Parameters
         ----------
         spins : List[int], optional
             A list of spins, by default None
-        vmin : float, optional
-            Value to normalize the minimum projection value, by default None
-        vmax : float, optional
-            Value to normalize the maximum projection value, by default None
         weights : np.ndarray, optional
             The weights of each point, by default None
-        plot_color_bar : bool, optional
-            Boolean to plot the color bar, by default False
         """
         
-        linewidth = [l*7 for l in settings.ebs.linewidth]
-        if type(settings.ebs.color_map) is str:
+        linewidth = [l*7 for l in self.plot_opt['linewidth']['value']]
+        if type(self.plot_opt['cmap']['value']) is str:
             color_map = ['Reds', "Blues", "Greens",
                      "Purples", "Oranges", "Greys"]
+        else:
+            color_map=self.plot_opt['cmap']['value']
         if spins is None:
             spins = range(self.ebs.nspins)
         if self.ebs.is_non_collinear:
             spins = [0]
         for iweight, weight in enumerate(weights):
-
+            vmin=self.plot_opt['clim']['value'][0]
+            vmax=self.plot_opt['clim']['value'][1]
             if vmin is None:
                 vmin = 0
             if vmax is None:
                 vmax = 1
             norm = mpl.colors.Normalize(vmin, vmax)
             for ispin in spins:
                 # plotting
@@ -370,24 +368,24 @@
                     segments = np.concatenate(
                         [points[:-1], points[1:]], axis=1)
                     # this is to delete the segments on the high sym points
                     x = self.x
                     segments = np.delete(
                         segments, np.where(x[1:] == x[:-1])[0], axis=0)
                     lc = LineCollection(
-                        segments, cmap=plt.get_cmap(color_map[iweight]), norm=norm, alpha=settings.ebs.opacity[0])
+                        segments, cmap=plt.get_cmap(color_map[iweight]), norm=norm, 
+                        alpha=self.plot_opt['opacity']['value'][ispin])
                     lc.set_array(weight[:, iband, ispin])
-                    lc.set_linewidth(
-                        weight[:, iband, ispin]*linewidth[ispin])
+                    lc.set_linewidth(weight[:, iband, ispin]*linewidth[ispin])
                     handle = self.ax.add_collection(lc)
             handle.set_color(color_map[iweight][:-1].lower())
             handle.set_linewidth(linewidth)
             self.handles.append(handle)
 
-            if settings.ebs.plot_color_bar:
+            if self.plot_opt['plot_color_bar']['value']:
                 cb = self.fig.colorbar(lc, ax=self.ax)
                 cb.ax.tick_params(labelsize=20)
 
     def set_xticks(self, 
         tick_positions:List[int]=None, 
         tick_names:List[str]=None, 
         color:str="black"):
@@ -536,15 +534,15 @@
 
         Parameters
         ----------
         labels : List[str], optional
             A list of strings for the labels of each element for the legend, by default None
         """
         if labels == None:
-            labels = settings.ebs.label
+            labels = self.plot_opt['label']['value']
         self.ax.legend(self.handles, labels)
 
     def draw_fermi(self, 
                 fermi_level:float=0, 
                 color:str="blue", 
                 linestyle:str="dotted", 
                 linewidth:float=1):
@@ -557,35 +555,37 @@
         linestyle : str, optional
             The linestyle, by default "dotted"
         linewidth : float, optional
             The linewidth, by default 1
         """
         self.ax.axhline(y=fermi_level, color=color, linestyle=linestyle, linewidth=linewidth)
 
-
     def grid(self):
         """A method to plot a grid
         """
         self.ax.grid(
-            settings.ebs.grid,
-            which=settings.ebs.grid_which,
-            color=settings.ebs.grid_color,
-            linestyle=settings.ebs.grid_linestyle,
-            linewidth=settings.ebs.grid_linewidth)
-        
-        
+            self.plot_opt['grid']['value'],
+            which=self.plot_opt['grid_which']['value'],
+            color=self.plot_opt['grid_color']['value'],
+            linestyle=self.plot_opt['grid_linestlye']['value'],
+            linewidth=self.plot_opt['grid_linewidth']['value'])
+    
     def show(self):
         """A method to show the plot
         """
         plt.show()
 
     def save(self, filename:str='bands.pdf'):
         """A method to save the plot
 
         Parameters
         ----------
         filename : str, optional
             A string for the file name, by default 'bands.pdf'
         """
-        plt.savefig(filename, bbox_inches="tight")
+        plt.savefig(filename, dpi=self.plot_opt['dpi']['value'], bbox_inches="tight")
         plt.clf()
     
+    def update_config(self, config_dict):
+        for key,value in config_dict.items():
+            self.plot_opt[key]['value']=value
+
```

### Comparing `PyProcar-6.0.0/pyprocar/plotter/procarplot.py` & `PyProcar-6.1.0/pyprocar/plotter/procarplot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/__init__.py` & `PyProcar-6.1.0/pyprocar/scripts/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .scriptDosplot import dosplot
 from .scriptBandsplot_2d import bandsplot_2d
 from .scriptCat import cat
 
 from .scriptFermi2D import fermi2D
 from .scriptFermi3D import fermi3D
 from .scriptFermiHandler import FermiHandler
-
+from .scriptBandStructure2DHandler import BandStructure2DHandler
 
 from .scriptSpin_asymmetry import spin_asymmetry
 from .scriptFilter import filter
 from .scriptKmesh2D import generate2dkmesh
 from .scriptKpath import kpath
 from .scriptRepair import repair
 from .scriptUnfold import unfold
```

### Comparing `PyProcar-6.0.0/pyprocar/scripts/depreciated_scriptVector.py` & `PyProcar-6.1.0/pyprocar/scripts/depreciated_scriptVector.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptBandGap.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptBandGap.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptBandsDosplot.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptBandsDosplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,14 @@
 
     welcome()
 
 
     #inital settings
     bands_settings['code'] = code
     dos_settings['code'] = code
-    bands_settings['lobster'] = lobster
-    dos_settings['lobster'] = lobster
     dos_settings['orientation'] = 'vertical'
     bands_settings['show'] = False
     dos_settings['show'] = False
 
     # parses old elements
     bands_settings, dos_settings = parse_kwargs(kwargs,bands_settings, dos_settings)
```

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptBandsplot.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptBandsplot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 __author__ = "Pedram Tavadze and Logan Lang"
 __maintainer__ = "Pedram Tavadze and Logan Lang"
 __email__ = "petavazohi@mail.wvu.edu, lllang@mix.wvu.edu"
 __date__ = "March 31, 2020"
 
 from typing import List
 import os
+import yaml
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from ..utils.info import orbital_names
 from .. import io
 from ..plotter import EBSPlot
-from ..utils import welcome
-from ..utils.defaults import settings
+from ..utils import welcome, ROOT
 
 
-# TODO What is the type is for projection mask?
-# TODO Needs abinit parsing
-# TODO Needs elk parsing
+with open(os.path.join(ROOT,'pyprocar','cfg','band_structure.yml'), 'r') as file:
+    plot_opt = yaml.safe_load(file)
+    
 
 def bandsplot(
     code: str,
     dirname: str,
     mode:str="plain",
     spins:List[int]=None,
     atoms:List[int]=None,
     orbitals:List[int]=None,
     items:dict={},
     fermi:float=None,
     interpolation_factor:int=1,
     interpolation_type:str="cubic",
     projection_mask:np.ndarray=None,
-    vmax:float=None,
-    vmin:float=None,
     kticks=None,
     knames=None,
     elimit: List[float]=None,
     ax:plt.Axes=None,
-    title:str=None,
     show:bool=True,
     savefig:str=None,
-    **kwargs,
+    print_plot_opts:bool=False,
+    **kwargs
     ):
     """A function to plot the band structutre
 
     Parameters
     ----------
     code : str, optional
         String to of the code used, by default "vasp"
@@ -65,35 +63,46 @@
         Float for the fermi energy, by default None
     interpolation_factor : int, optional
         The interpolation_factor, by default 1
     interpolation_type : str, optional
         The interpolation type, by default "cubic"
     projection_mask : np.ndarray, optional
         A custom projection mask, by default None
-    vmax : float, optional
-        Value to normalize the minimum projection value., by default None, by default None
-    vmin : float, optional
-        Value to normalize the maximum projection value., by default None, by default None
     kticks : _type_, optional
         A list of kticks, by default None
     knames : _type_, optional
         A list of kanems, by default None
     elimit : List[float], optional
         A list of floats to decide the energy window, by default None
     ax : plt.Axes, optional
         A matplotlib axes, by default None
-    title : str, optional
-        String for the title name, by default None
     show : bool, optional
         Boolean if to show the plot, by default True
     savefig : str, optional
         String to save the plot, by default None
+    print_plot_opts: bool, optional
+        Boolean to print the plotting options
     """
 
-    settings.modify(kwargs)
+    modes=["plain","parametric","scatter",
+           "overlay", "overlay_species", "overlay_orbitals"]
+    modes_txt=' , '.join(modes)
+    message=f"""
+            --------------------------------------------------------
+            There are additional plot options that are defined in a configuration file. 
+            You can change these configurations by passing the keyword argument to the function
+            To print a list of plot options set print_plot_opts=True
+
+            Here is a list modes : {modes_txt}
+            --------------------------------------------------------
+            """
+    print(message)
+    if print_plot_opts:
+        for key,value in plot_opt.items():
+            print(key,':',value)
 
     parser = io.Parser(code = code, dir = dirname)
     ebs = parser.ebs
     structure = parser.structure
     kpath = parser.kpath
 
     # shifting fermi to 0
@@ -158,17 +167,15 @@
                         w = ebs_plot.ebs.ebs_sum(
                             atoms=atoms,
                             principal_q_numbers=[-1],
                             orbitals=orbitals,
                             spins=spins,
                         )
                         weights.append(w)
-        ebs_plot.plot_parameteric_overlay(
-            spins=spins, vmin=vmin, vmax=vmax, weights=weights
-        )
+        ebs_plot.plot_parameteric_overlay(spins=spins,weights=weights)
     else:
         if atoms is not None and isinstance(atoms[0], str):
             atoms_str = atoms
             atoms = []
             for iatom in np.unique(atoms_str):
                 atoms = np.append(atoms, np.where(structure.atoms == iatom)[0]).astype(
                     np.int
@@ -179,65 +186,61 @@
 
             orbitals = []
             for iorb in orbital_str:
                 orbitals = np.append(orbitals, orbital_names[iorb]).astype(np.int)
 
 
         weights = ebs_plot.ebs.ebs_sum(atoms=atoms, principal_q_numbers=[-1], orbitals=orbitals, spins=spins)
-        if settings.ebs.weighted_color:
+        if plot_opt['weighted_color']['value']:
             color_weights = weights
         else:
             color_weights = None
-        if settings.ebs.weighted_width:
+        if plot_opt['weighted_width']['value']:
             width_weights = weights
         else:
             width_weights = None
         color_mask = projection_mask
         width_mask = projection_mask
         if mode == "parametric":
             ebs_plot.plot_parameteric(
                 color_weights=color_weights,
                 width_weights=width_weights,
                 color_mask=color_mask,
                 width_mask=width_mask,
-                vmin=vmin,
-                vmax=vmax,
                 spins=spins
                 )
         elif mode == "scatter":
             ebs_plot.plot_scatter(
                 color_weights=color_weights,
                 width_weights=width_weights,
                 color_mask=color_mask,
                 width_mask=width_mask,
-                spins=spins,
-                vmin=vmin,
-                vmax=vmax,
+                spins=spins
             )
 
         else:
             print("Selected mode %s not valid. Please check the spelling " % mode)
             
     ebs_plot.set_xticks(kticks, knames)
     ebs_plot.set_yticks(interval=elimit)
     ebs_plot.set_xlim()
     ebs_plot.set_ylim(elimit)
     ebs_plot.draw_fermi(
         fermi_level=fermi_level,
-        color=settings.ebs.fermi_color,
-        linestyle=settings.ebs.fermi_linestyle,
-        linewidth=settings.ebs.fermi_linewidth,
+        color=plot_opt['fermi_color']['value'],
+        linestyle=plot_opt['fermi_linestyle']['value'],
+        linewidth=plot_opt['fermi_linewidth']['value'],
     )
     ebs_plot.set_ylabel()
 
-    if title:
-        ebs_plot.set_title(title=title)
-    if settings.ebs.grid:
+    if plot_opt['title']['value']:
+        ebs_plot.set_title(title=plot_opt['title']['value'])
+    if plot_opt['grid']['value']:
         ebs_plot.grid()
-    if settings.ebs.legend and len(labels) != 0:
+    if plot_opt['legend']['value'] and len(labels) != 0:
         ebs_plot.legend(labels)
     if savefig is not None:
         ebs_plot.save(savefig)
     if show:
         ebs_plot.show()
         
     return ebs_plot
```

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptBandsplot_2d.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptBandsplot_2d.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptCat.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptCat.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptDosplot.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptDosplot.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,60 +2,48 @@
 __author__ = "Pedram Tavadze and Logan Lang"
 __maintainer__ = "Pedram Tavadze and Logan Lang"
 __email__ = "petavazohi@mail.wvu.edu, lllang@mix.wvu.edu"
 __date__ = "March 31, 2020"
 
 import os
 from typing import List, Tuple
+import yaml
 
 import numpy as np
 import matplotlib.pyplot as plt
 
-from ..utils import welcome
+from ..utils import welcome, ROOT
 from .. import io
 from ..utils.info import orbital_names
 from ..plotter import DOSPlot
-from ..utils.defaults import settings
 
+with open(os.path.join(ROOT,'pyprocar','cfg','dos.yml'), 'r') as file:
+    plot_opts = yaml.safe_load(file)
 
 def dosplot(
-        filename:str="vasprun.xml",
         dirname:str=None,
-        poscar:str='POSCAR',
-        procar:str="PROCAR",
-        outcar:str='OUTCAR',
         mode:str="plain",
         interpolation_factor:int=1,
         orientation:str="horizontal",
-        spin_colors:List[str] or List[Tuple[int,int,int]]=None,
-        spin_labels:List[str]=None,
-        colors:List[str] or List[Tuple[int,int,int]]=None,
         spins:List[int]=None,
         atoms:List[int]=None,
         orbitals:List[int]=None,
         items:dict={},
         fermi:float=None,
         elimit:List[float]=None,
         dos_limit:List[float]=None,
-        cmap:str="jet",
-        linewidth:float=1,
-        vmax:float=None,
-        vmin:float=None,
         grid:bool=False,
         savefig:str=None,
-        title:str=None,
-        plot_total:bool=True,
         projection_mask=None,
         code:str="vasp",
-        lobster:bool=False,
-        labels:List[str]=None, 
         ax:plt.Axes=None,
         verbose:bool=True,
-        old:bool=False,
-        show:bool=True
+        print_plot_opts:bool=False,
+        show:bool=True,
+        **kwargs
     ):
 
     """
     This function plots the density of states in different formats
 
     Parameters
     ----------
@@ -93,55 +81,23 @@
 
     orientation : str, optional (default ``horizontal'``)
         The orientation of the DOS plot.  options are
         ``'horizontal', 'vertical'``
 
         e.g. ``orientation='vertical'``
 
-    spin_colors : list str or tuples, (optional ``spin_colors=['blue','red']``)
-        **spin_colors** represent the colors the different spin
-        ploarizations are going to be represented in the DOS
-        plot. These colors can be chosen from any type of color
-        acceptable by matplotlib(string,rgb,html).
-
-        e.g. ``spin_colors=['blue','red']``,
-        ``spin_colors=[(0, 0, 1),(1, 0,0 )]``,
-        ``spin_colors=['#0000ff','#ff0000']``
-
-        .. caution:: 
-        
-            If the calculation is spin polarized one has to
-            provide two colors even if one is plotting one spin. I
-            disregard this cation if using default.
-
-    colors : list str or tuples, optional (default, optional)
-        ``colors`` defines the color of plots filling the area under
-        the curve of Total density of states. This is only important in the
-        ``mode=stack``, ``mode=stack_species``,
-        ``mode=stack_orbitals``. To have a better sense of this
-        parameter refer to the stack plots of  SrVO\ :sub:`3`\. These
-        colors can be chosen from any type of color acceptable by
-        matplotlib(string,rgb,html).
-
-        e.g. ``colors=['red', 'blue', 'green', 'magenta', 'cyan']``
-
     spins : list int, optional
         ``spins`` defines plotting of different spins channels present
         in the calculation, If the calculation is spin non-polorized
         the spins will be set by default to ``spins=[0]``. if the
         calculation is spin polorized this parameter can be set to 0
         or 1 or both.
 
         e.g. ``spins=[0, 1]``
 
-    spin_labels : list str, optional
-        ``spin_labels`` defines labels to use to represent spin 
-        in the legend of the plot.
-        e.g. ``spin_labels=['up','down']``
-
     atoms : list int, optional
         ``atoms`` define the projection of the atoms in the Density of
         States. In other words it selects only the contribution of the
         atoms provided. Atoms has to be a python list(or numpy array)
         containing the atom indices. Atom indices has to be order of
         the input files of DFT package. ``atoms`` is only relevant in
         ``mode='parametric'``, ``mode='parametric_line'``,
@@ -206,87 +162,36 @@
     dos_limit : list float, optional
        ``dos_limit`` defines the density of states axis limits on the
        graph. It is automatically set to select 10% higher than the
        maximum of density of states in the specified energy window.
 
        e.g. ``dos_limit=[0, 30]``
 
-    cmap : str , optional (default 'jet')
-        The color map used for color coding the projections. ``cmap``
-        is only relevant in ``mode='parametric'``. a full list of
-        color maps in matplotlib are provided in this web
-        page. `https://matplotlib.org/2.0.1/users/colormaps.html
-        <https://matplotlib.org/2.0.1/users/colormaps.html>`_
-
-        e.g. ``cmap='plasma'``
-
-    linewidth : float, optional (default 1)
-        The line width with which the total DOS is ploted
-
-        e.g. linewidth=2
-
-    vmax : float, optional
-        The maximum value in the color bar. ``cmap`` is only relevant
-        in ``mode='parametric'``.
-
-        e.g. ``vmax=1.0``
-
-    vmin : float, optional
-        The maximum value in the color bar. ``cmap`` is only relevant
-        in ``mode='parametric'``.
-
-        e.g. ``vmin=-1.0``
-
-    grid : bool, optional (default Flase)
-        Defines If a grid is plotted in the plot. The entry should be
-        python boolian.
-
-        e.g. ``grid=True``
-
     savefig : str , optional (default None)
         ``savefig`` defines the file that the plot is going to be
         saved in. ``savefig`` accepts all the formats accepted by
         matplotlib such as png, pdf, jpg, ...
         If not provided the plot will be shown in the
         interactive matplotlib mode.
 
         e.g. ``savefig='DOS.png'``, ``savefig='DOS.pdf'``
 
-    title : str, optional
-        Defines the plot title asked to be added above the plot. If
-        ``title`` is not defined, PyProcar will not add any title.
-
-        e.g. ``title="Total Density of States SrVO_$3$"``. One can use
-        LaTex format as well.
-
     plot_total : bool, optional (default ``True``)
         If the total density of states is plotted as well as other
         options. The entry should be python boolian.
 
         e.g. ``plot_total=True``
 
     code : str, optional (default ``'vasp'``)
         Defines the Density Functional Theory code used for the
         calculation. The default of this argument is vasp, so if the
         cal is done in vasp one does not need to define this argumnet.
 
         e.g. ``code=vasp``, ``code=elk``, ``code=abinit``
 
-    labels : list str, optional
-        ``labels`` define the legends plotted in defining each spin.
-
-        e.g.  ``labels=['Oxygen-Up','Oxygen-Down']``,
-        ``labels=['Oxygen-'+r'$\\uparrow$','Oxygen-'+r'$\\downarrow$']``
-        Side means the string will be treated as raw string. This has
-        to be used if LaTex formating is used.
-        No default is used in the ``mode=plain``, ``mode=parametric``,
-        ``mode=parametric_line``. In ``mode=stack``, `ack_species``,
-        ``mode=stack_orbitals`` the labels are generated automatically
-        based on the other parameters such as atoms and orbitals.
-
     items : dict, optional
         ``items`` is only relavent for ``mode='stack'``. stack will
         plot the items defined with stacked filled areas under
         curve. For clarification visit the examples in the
         tutorial. ``items`` need to be provided as a python
         dictionary, with keys being specific species and values being
         projections of ``orbitals``. The following examples can
@@ -335,28 +240,47 @@
 
         >>> fig, ax = pyprocar.dosplot(mode='plain', plt_show=False)
         >>> ax.set_ylim(-2,2)
         >>> fig.show()
 
     """
     
+    modes=['plain','parametric',
+           'parametric_line', 'stack', 
+           'stack_orbitals', 'stack_species']
+    modes_txt=' , '.join(modes)
+    message=f"""
+            --------------------------------------------------------
+            There are additional plot options that are defined in a configuration file. 
+            You can change these configurations by passing the keyword argument to the function
+            To print a list of plot options set print_plot_opts=True
+
+            Here is a list modes : {modes_txt}
+            --------------------------------------------------------
+            """
+    print(message)
+    if print_plot_opts:
+        for key,value in plot_opts.items():
+            print(key,':',value)
+    
+
     if orientation[0].lower() == 'h':
         orientation = 'horizontal'
     elif orientation[0].lower() == 'v':
         orientation = 'vertical'
 
     
     parser = io.Parser(code = code, dir = dirname)
     dos = parser.dos
     structure = parser.structure
 
     if elimit is None:
         elimit = [dos.energies.min(), dos.energies.max()]
     
-    edos_plot = DOSPlot(dos = dos, structure = structure, orientation = orientation)
+    edos_plot = DOSPlot(dos = dos, structure = structure, **kwargs)
     
     if mode == "plain":
         edos_plot.plot_dos(spins=spins, orientation = orientation)
 
     elif mode == "parametric":
         if atoms is None:
             atoms = list(np.arange(edos_plot.structure.natoms, dtype=int))
@@ -365,97 +289,74 @@
         if orbitals is None:
             orbitals = list(np.arange(len(edos_plot.dos.projected[0][0]), dtype=int))
         edos_plot.plot_parametric(
                         atoms=atoms,
                         principal_q_numbers=[-1],
                         orbitals=orbitals,
                         spins=spins,
-                        spin_colors=spin_colors,
-                        spin_labels=spin_labels,
-                        cmap=cmap,
-                        vmin=vmin,
-                        vmax=vmax,
-                        orientation = orientation,
-                        plot_total=plot_total,
-                        plot_bar=True)
+                        orientation=orientation)
 
     elif mode == "parametric_line":
         if atoms is None:
             atoms = list(np.arange(edos_plot.structure.natoms, dtype=int))
         if spins is None:
             spins = list(np.arange(len(edos_plot.dos.total)))
         if orbitals is None:
             orbitals = list(np.arange(len(edos_plot.dos.projected[0][0]), dtype=int))
         
         edos_plot.plot_parametric_line(
                         atoms=atoms,
                         principal_q_numbers=[-1],
                         spins=spins,
                         orbitals=orbitals,
-                        spin_colors=spin_colors,
-                        vmax=vmax,
-                        vmin=vmin,
-                        cmap=cmap,
                         orientation=orientation
                         )
 
     elif mode == "stack_species":
         edos_plot.plot_stack_species(
             spins=spins,
             orbitals=orbitals,
-            spin_colors=spin_colors,
-            spin_labels = spin_labels,
-            colors = colors,
-            plot_total = plot_total,
             orientation=orientation,
         )
 
     elif mode == "stack_orbitals":
         edos_plot.plot_stack_orbitals(
             spins=spins,
             atoms=atoms,
-            spin_colors=spin_colors,
-            spin_labels = spin_labels,
-            colors = colors,
-            plot_total = plot_total,
             orientation=orientation,
         )
 
     elif mode == "stack":
         edos_plot.plot_stack(
             spins=spins,
             items=items,
-            spin_colors=spin_colors,
-            spin_labels = spin_labels,
-            colors=colors,
             orientation=orientation,
-            plot_total = plot_total,
         )
     else:
         raise ValueError("The mode needs to be in the List [plain,parametric,parametric_line,stack_species,stack_orbitals,stack]")
 
     edos_plot.draw_fermi(
             orientation = orientation,
-            color=settings.dos.fermi_color,
-            linestyle=settings.dos.fermi_linestyle,
-            linewidth=settings.dos.fermi_linewidth,
+            color=plot_opts['fermi_color']['value'],
+            linestyle=plot_opts['fermi_linestyle']['value'],
+            linewidth=plot_opts['fermi_linewidth']['value'],
         )
     if orientation == 'horizontal':
         if elimit is not None:
             edos_plot.set_xlim(elimit)
         if dos_limit is not None:
             edos_plot.set_ylim(dos_limit)
     elif orientation == 'vertical' :
         if elimit is not None:
             edos_plot.set_ylim(elimit)
         if dos_limit is not None:
             edos_plot.set_xlim(dos_limit)
 
-    if settings.dos.grid or grid:
+    if plot_opts['grid']['value']:
         edos_plot.grid()
-    if settings.dos.legend and len(edos_plot.labels) != 0:
+    if plot_opts['legend']['value'] and len(edos_plot.labels) != 0:
         edos_plot.legend(edos_plot.labels)
     if savefig is not None:
         edos_plot.save(savefig)
     if show:
         edos_plot.show()
     return edos_plot
```

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptFermi2D.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptFermi2D.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 __author__ = "Pedram Tavadze and Logan Lang"
 __maintainer__ = "Pedram Tavadze and Logan Lang"
 __email__ = "petavazohi@mail.wvu.edu, lllang@mix.wvu.edu"
 __date__ = "December 01, 2020"
+
 import os
 from typing import List
-
+import yaml 
 import numpy as np
 import copy
 import matplotlib.pyplot as plt
 from matplotlib import colors as mpcolors
 from matplotlib import cm
 
 from ..core import ProcarSymmetry, FermiSurface
-from ..utils import welcome
+from ..utils import welcome, ROOT
 from .. import io
 
+with open(os.path.join(ROOT,'pyprocar','cfg','fermi_surface_2d.yml'), 'r') as file:
+    plot_opt = yaml.safe_load(file)
 
 def fermi2D(
     code:str,
     dirname:str,
     mode:str='plain',
     band_indices:List[List]=None,
     band_colors:List[List]=None,
-    lobster:bool=False,
     spins:List[int]=None,
     atoms:List[int]=None,
     orbitals:List[int]=None,
     energy:float=None,
     k_z_plane:float=0.0,
+    k_z_plane_tol:float=0.01,
     rot_symm=1,
     translate:List[int]=[0, 0, 0],
     rotation:List[int]=[0, 0, 0, 1],
-    savefig:str=None,
     spin_texture:bool=False,
-    arrow_projection:str='z',
-    arrow_size:float=None,
-    arrow_color:List[int] or str=None,
-    arrow_density:float=6,
-    no_arrow:bool=False,
-    cmap = 'jet',
-    color_bar:bool=False,
-    add_axes_labels:bool=True,
-    add_legend:bool=False,
     exportplt:bool=False,
-    
-    repair:bool=True,
+    savefig:str=None,
+    print_plot_opts:bool=False,
+    **kwargs
     ):
     """This function plots the 2d fermi surface in the z = 0 plane
 
     Parameters
     ----------
     code : str, 
         This parameter sets the code to parse, by default "vasp"
@@ -79,61 +73,33 @@
         Matrix to translate the kpoints, by default [0, 0, 0]
     rotation : List[int], optional
          Matrix to rotate the kpoints, by default [0, 0, 0, 1]
     savefig : str, optional
         The filename to save the plot as., by default None
     spin_texture : bool, optional
         Boolean value to determine if spin arrows are plotted, by default False
-    arrow_size : float, optional
-        Inversely determines the arrow size, by default None
-    arrow_color : List[int] or str, optional
-        Either a list for the rbg value or a string for the color, by default None
-    arrow_density : float, optional
-        Inversely determines the arrow density
-    no_arrow : bool, optional
-        A boolean value to determine if arrows or a heat map is produced for spins, by default False
-    add_axes_labels : bool, optional
-        Boolean value to add axes labels, by default True
-    add_legend : bool, optional
-        Boolean value to add legend, by default True
     exportplt : bool, optional
         Boolean value where to return the matplotlib.pyplot state plt, by default False
-    color_bar : bool, optional
-        Boolean value to plot the color bar, by default False
-    cmap : bool, optional
-        The colormap to be used, by default False
-    repair : bool, optional
-        Option for vasp to repair the procar file, by default True
+    print_plot_opts: bool, optional
+        Boolean to print the plotting options
 
     Returns
     -------
     matplotlib.pyplot
         Returns the matplotlib.pyplot state plt
 
     Raises
     ------
     RuntimeError
         invalid option --translate
     """
     welcome()
-
     # Turn interactive plotting off
     plt.ioff()
 
-    if atoms is None:
-        atoms = [-1]
-        
-
-    if orbitals is None:
-        orbitals = [-1]
-
-    
-
-
-
     if len(translate) != 3 and len(translate) != 1:
         print("Error: --translate option is invalid! (", translate, ")")
         raise RuntimeError("invalid option --translate")
 
     print("dirname         : ", dirname)
     print("bands           : ", band_indices)
     print("atoms           : ", atoms)
@@ -141,17 +107,33 @@
     print("spin comp.      : ", spins)
     print("energy          : ", energy)
     print("rot. symmetry   : ", rot_symm)
     print("origin (trasl.) : ", translate)
     print("rotation        : ", rotation)
     print("save figure     : ", savefig)
     print("spin_texture    : ", spin_texture)
-    print("no_arrows       : ", no_arrow)
 
-    
+
+    modes=["plain","plain_bands","parametric"]
+    modes_txt=' , '.join(modes)
+    message=f"""
+            --------------------------------------------------------
+            There are additional plot options that are defined in a configuration file. 
+            You can change these configurations by passing the keyword argument to the function
+            To print a list of plot options set print_plot_opts=True
+
+            Here is a list modes : {modes_txt}
+            --------------------------------------------------------
+            """
+    print(message)
+    if print_plot_opts:
+        for key,value in plot_opt.items():
+            print(key,':',value)
+
+
     parser = io.Parser(code = code, dir = dirname)
     ebs = parser.ebs
     structure = parser.structure
     ebs.bands -= ebs.efermi
 
     if structure.rotations is not None:
         ebs.ibz2fbz(structure.rotations)
@@ -161,29 +143,30 @@
     ebs.kpoints = ebs.kpoints + bound_ops
     kpoints = ebs.kpoints_cartesian
 
     if spins is None:
         spins = np.arange(ebs.bands.shape[-1])
     if energy is None:
         energy = 0
-    ### End of parsing ###
 
+    ### End of parsing ###
     # Selecting kpoints in a constant k_z plane
-    i_kpoints_near_z_0 = np.where(np.logical_and(kpoints[:,2]< k_z_plane + 0.01, kpoints[:,2] > k_z_plane - 0.01) )
+    i_kpoints_near_z_0 = np.where(np.logical_and(kpoints[:,2] < k_z_plane + k_z_plane_tol, 
+                                                 kpoints[:,2] > k_z_plane - k_z_plane_tol) )
     kpoints = kpoints[i_kpoints_near_z_0,:][0]
     ebs.bands = ebs.bands[i_kpoints_near_z_0,:][0]
     ebs.projected = ebs.projected[i_kpoints_near_z_0,:][0]
     print('_____________________________________________________')
     for i_spin in spins:
         indices = np.where( np.logical_and(ebs.bands[:,:,i_spin].min(axis=0) < energy, ebs.bands[:,:,i_spin].max(axis=0) > energy))
         if len(indices) != 0:
             print(f"Useful band indices for spin-{i_spin} : {indices[0]}")
 
 
-    if spin_texture is not True:
+    if spin_texture is False:
         # processing the data
         if orbitals is None and ebs.projected is not None:
             orbitals = np.arange(ebs.norbitals, dtype=int)
         if atoms is None and ebs.projected is not None:
             atoms = np.arange(ebs.natoms, dtype=int)
         projected = ebs.ebs_sum(spins=spins , atoms=atoms, orbitals=orbitals, sum_noncolinear=False)
         projected = projected[:,:,spins]
@@ -213,107 +196,47 @@
     # symmetry operations to unfold the Brillouin Zone
     # kpoints = data.kpoints
     # bands = data.bands
     # character = data.spd
 
     bands = ebs.bands
     character = projected
+
     if spin_texture is True:
         sx, sy, sz = stData[0], stData[1], stData[2]
         symm = ProcarSymmetry(kpoints, bands, sx=sx, sy=sy, sz=sz, character=character)
     else:
         symm = ProcarSymmetry(kpoints, bands, character=character)
         symm.translate(translate)
         symm.general_rotation(rotation[0], rotation[1:])
         # symm.MirrorX()
         symm.rot_symmetry_z(rot_symm)
-    fs = FermiSurface(symm.kpoints, symm.bands, symm.character, cmap = cmap,  band_indices=band_indices, band_colors=band_colors)
+
+    fs = FermiSurface(symm.kpoints, symm.bands, symm.character,  
+                      band_indices=band_indices, 
+                      band_colors=band_colors,**kwargs)
     fs.find_energy(energy)
 
     if not spin_texture:
         fs.plot(mode=mode, interpolation=300)
     else:
         fs.spin_texture(sx=symm.sx, 
                         sy=symm.sy, 
                         sz=symm.sz, 
-                        arrow_projection=arrow_projection,
-                        no_arrow=no_arrow, 
-                        spin=spins[0], 
-                        arrow_size = arrow_size,
-                        arrow_color = arrow_color,
-                        arrow_density=arrow_density,
-                        color_bar=color_bar
-                        )
+                        spin=spins[0])
 
-    if add_axes_labels:
+    if plot_opt['add_axes_labels']['value']:
         fs.add_axes_labels()
 
-    if add_legend:
+    if plot_opt['add_legend']['value']:
         fs.add_legend()
 
     if exportplt:
         return plt
 
     else:
         if savefig:
-            plt.savefig(savefig, bbox_inches="tight")
+            plt.savefig(savefig,dpi=plot_opt['dpi']['value'], bbox_inches="tight")
             plt.close()  # Added by Nicholas Pike to close memory issue of looping and creating many figures
         else:
             plt.show()
         return
-
-
-# def parse(code:str='vasp',
-#           lobster:bool=False,
-#           repair:bool=False,
-#           dirname:str="",
-#           apply_symmetry:bool=True):
-#         if code == "vasp" or code == "abinit":
-#             if repair:
-#                 repairhandle = UtilsProcar()
-#                 repairhandle.ProcarRepair(procar, procar)
-#                 print("PROCAR repaired. Run with repair=False next time.")
-
-#         if code == "vasp":
-#             outcar = f"{dirname}{os.sep}OUTCAR"
-#             poscar = f"{dirname}{os.sep}POSCAR"
-#             procar = f"{dirname}{os.sep}PROCAR"
-#             kpoints = f"{dirname}{os.sep}KPOINTS"
-#             filename = f"{dirname}{os.sep}{filename}"
-#             outcar = io.vasp.Outcar(filename=outcar)
-        
-#             e_fermi = outcar.efermi
-        
-#             poscar = io.vasp.Poscar(filename=poscar)
-#             structure = poscar.structure
-#             reciprocal_lattice = poscar.structure.reciprocal_lattice
-
-#             parser = io.vasp.Procar(filename=procar,
-#                                     structure=structure,
-#                                     reciprocal_lattice=reciprocal_lattice,
-#                                     efermi=e_fermi,
-#                                     )
-
-#             if apply_symmetry:                       
-#                 ebs.ibz2fbz(rotations)
-
-#             bound_ops = -1.0*(ebs.kpoints > 0.5) + 1.0*(ebs.kpoints <= -0.5)
-#             kpoints_cart = kpoints.dot(reciprocal_lattice)
-
-#         elif code == "qe":
-
-#             if dirname is None:
-#                 dirname = "bands"
-#             parser = io.qe.QEParser(dirname = dirname, scf_in_filename = "scf.in", bands_in_filename = "bands.in", 
-#                                     pdos_in_filename = "pdos.in", kpdos_in_filename = "kpdos.in", atomic_proj_xml = "atomic_proj.xml")
-#             reciprocal_lattice = reciprocal_lattice
-
-#             e_fermi = efermi
-
-#             if apply_symmetry:
-#                 ebs.ibz2fbz(rotations)
-
-#             bound_ops = -1.0*(ebs.kpoints > 0.5) + 1.0*(ebs.kpoints <= -0.5)
-#             kpoints = ebs.kpoints  + bound_ops
-#             kpoints_cart = kpoints.dot(reciprocal_lattice) * (alat/(2*np.pi))
-
-#         return parser, kpoints_cart, reciprocal_lattice, e_fermi
```

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptFermi3D.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptFermi3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import copy
 
 import numpy as np
 from matplotlib import colors as mpcolors
 from matplotlib import cm
 import vtk
 import pyvista
-from pyvista.utilities import NORMALS, generate_plane, get_array, try_callback
+from pyvista.core.utilities import NORMALS, generate_plane, get_array, try_callback
 
 
 from ..core import FermiSurface3D
 from ..utils import welcome
 from ..utils import UtilsProcar
 from ..io.procarparser import ProcarParser
 from ..io.lobsterparser import LobsterFermiParser
```

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptFilter.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptFilter.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptKmesh2D.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptKmesh2D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptKpath.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptKpath.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptRepair.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptRepair.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptSpin_asymmetry.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptSpin_asymmetry.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptUnfold.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptUnfold.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptUnfold_new.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_new.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptUnfold_old.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_old.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptUnfold_v2.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_v2.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/scripts/scriptVector.py` & `PyProcar-6.1.0/pyprocar/scripts/scriptVector.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/utils/default_settings.ini` & `PyProcar-6.1.0/pyprocar/utils/default_settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -42,68 +42,68 @@
 00000290: 0d0a 7370 696e 5f63 6f6c 6f72 733d 626c  ..spin_colors=bl
 000002a0: 6163 6b2c 2072 6564 0d0a 7370 696e 5f6c  ack, red..spin_l
 000002b0: 6162 656c 733d 245c 7570 6172 726f 7724  abels=$\uparrow$
 000002c0: 2c24 5c64 6f77 6e61 7272 6f77 240d 0a63  ,$\downarrow$..c
 000002d0: 6f6c 6f72 7320 3d20 7265 642c 2067 7265  olors = red, gre
 000002e0: 656e 2c20 626c 7565 2c20 6379 616e 2c20  en, blue, cyan, 
 000002f0: 6d61 6765 6e74 612c 2079 656c 6c6f 772c  magenta, yellow,
-00000300: 206f 7261 6e67 652c 7075 7270 6c65 2c20   orange,purple, 
-00000310: 6272 6f77 6e2c 206e 6176 792c 206d 6172  brown, navy, mar
-00000320: 6f6f 6e2c 206f 6c69 7665 0d0a 6f70 6163  oon, olive..opac
-00000330: 6974 793d 312e 302c 2031 2e30 0d0a 636f  ity=1.0, 1.0..co
-00000340: 6c6f 725f 6d61 703d 6a65 740d 0a23 2073  lor_map=jet..# s
-00000350: 6361 7474 6572 206f 7074 696f 6e73 0d0a  catter options..
-00000360: 6d61 726b 6572 7369 7a65 3d30 2e32 2c30  markersize=0.2,0
-00000370: 2e32 0d0a 6d61 726b 6572 3d6f 2c76 2c5e  .2..marker=o,v,^
-00000380: 2c44 0d0a 2320 6665 726d 690d 0a66 6572  ,D..# fermi..fer
-00000390: 6d69 5f63 6f6c 6f72 3d62 6c61 636b 0d0a  mi_color=black..
-000003a0: 6665 726d 695f 6c69 6e65 7374 796c 653d  fermi_linestyle=
-000003b0: 646f 7474 6564 0d0a 6665 726d 695f 6c69  dotted..fermi_li
-000003c0: 6e65 7769 6474 683d 310d 0a23 2067 7269  newidth=1..# gri
-000003d0: 6420 6f70 7469 6f6e 730d 0a67 7269 643d  d options..grid=
-000003e0: 4661 6c73 650d 0a67 7269 645f 7768 6963  False..grid_whic
-000003f0: 683d 6d61 6a6f 7220 0d0a 6772 6964 5f61  h=major ..grid_a
-00000400: 7869 733d 626f 7468 200d 0a67 7269 645f  xis=both ..grid_
-00000410: 636f 6c6f 723d 6772 6579 0d0a 6772 6964  color=grey..grid
-00000420: 5f6c 696e 6573 7479 6c65 3d73 6f6c 6964  _linestyle=solid
-00000430: 0d0a 6772 6964 5f6c 696e 6577 6964 7468  ..grid_linewidth
-00000440: 3d31 0d0a 2320 7765 6967 6874 206f 7074  =1..# weight opt
-00000450: 696f 6e73 0d0a 7765 6967 6874 6564 5f77  ions..weighted_w
-00000460: 6964 7468 3d46 616c 7365 0d0a 7765 6967  idth=False..weig
-00000470: 6874 6564 5f63 6f6c 6f72 3d54 7275 650d  hted_color=True.
-00000480: 0a6c 6567 656e 643d 5472 7565 0d0a 7361  .legend=True..sa
-00000490: 7665 6669 673d 4e6f 6e65 0d0a 706c 6f74  vefig=None..plot
-000004a0: 5f63 6f6c 6f72 5f62 6172 3d54 7275 650d  _color_bar=True.
-000004b0: 0a74 6974 6c65 3d4e 6f6e 650d 0a0d 0a0d  .title=None.....
-000004c0: 0a5b 756e 666f 6c64 5d0d 0a23 206c 696e  .[unfold]..# lin
-000004d0: 6520 6f70 7469 6f6e 732c 200d 0a6c 696e  e options, ..lin
-000004e0: 6573 7479 6c65 3d73 6f6c 6964 2c20 6461  estyle=solid, da
-000004f0: 7368 6564 200d 0a6c 696e 6577 6964 7468  shed ..linewidth
-00000500: 3d31 2c31 0d0a 636f 6c6f 723d 626c 6163  =1,1..color=blac
-00000510: 6b2c 2062 6c61 636b 0d0a 6c61 6265 6c3d  k, black..label=
-00000520: 245c 7570 6172 726f 7724 2c24 5c64 6f77  $\uparrow$,$\dow
-00000530: 6e61 7272 6f77 240d 0a6f 7061 6369 7479  narrow$..opacity
-00000540: 3d30 2e33 2c20 302e 330d 0a63 6f6c 6f72  =0.3, 0.3..color
-00000550: 5f6d 6170 3d52 6564 730d 0a23 2073 6361  _map=Reds..# sca
-00000560: 7474 6572 206f 7074 696f 6e73 0d0a 6d61  tter options..ma
-00000570: 726b 6572 7369 7a65 3d30 2e32 2c30 2e32  rkersize=0.2,0.2
-00000580: 0d0a 6d61 726b 6572 3d6f 2c76 2c5e 2c44  ..marker=o,v,^,D
-00000590: 0d0a 2320 6665 726d 690d 0a66 6572 6d69  ..# fermi..fermi
-000005a0: 5f63 6f6c 6f72 3d62 6c75 650d 0a66 6572  _color=blue..fer
-000005b0: 6d69 5f6c 696e 6573 7479 6c65 3d64 6f74  mi_linestyle=dot
-000005c0: 7465 640d 0a66 6572 6d69 5f6c 696e 6577  ted..fermi_linew
-000005d0: 6964 7468 3d31 0d0a 2320 6772 6964 206f  idth=1..# grid o
-000005e0: 7074 696f 6e73 0d0a 6772 6964 3d46 616c  ptions..grid=Fal
-000005f0: 7365 0d0a 6772 6964 5f77 6869 6368 3d6d  se..grid_which=m
-00000600: 616a 6f72 200d 0a67 7269 645f 6178 6973  ajor ..grid_axis
-00000610: 3d62 6f74 6820 0d0a 6772 6964 5f63 6f6c  =both ..grid_col
-00000620: 6f72 3d67 7265 790d 0a67 7269 645f 6c69  or=grey..grid_li
-00000630: 6e65 7374 796c 653d 736f 6c69 640d 0a67  nestyle=solid..g
-00000640: 7269 645f 6c69 6e65 7769 6474 683d 310d  rid_linewidth=1.
-00000650: 0a23 2077 6569 6768 7420 6f70 7469 6f6e  .# weight option
-00000660: 730d 0a77 6569 6768 7465 645f 7769 6474  s..weighted_widt
-00000670: 683d 4661 6c73 650d 0a77 6569 6768 7465  h=False..weighte
-00000680: 645f 636f 6c6f 723d 5472 7565 0d0a 6c65  d_color=True..le
-00000690: 6765 6e64 3d54 7275 650d 0a73 6176 6566  gend=True..savef
-000006a0: 6967 3d4e 6f6e 650d 0a70 6c6f 745f 636f  ig=None..plot_co
-000006b0: 6c6f 725f 6261 723d 5472 7565 0d0a 7469  lor_bar=True..ti
-000006c0: 746c 653d 4e6f 6e65 0d0a                 tle=None..
+00000300: 206f 7261 6e67 652c 2070 7572 706c 652c   orange, purple,
+00000310: 2062 726f 776e 2c20 6e61 7679 2c20 6d61   brown, navy, ma
+00000320: 726f 6f6e 2c20 6f6c 6976 650d 0a6f 7061  roon, olive..opa
+00000330: 6369 7479 3d31 2e30 2c20 312e 300d 0a63  city=1.0, 1.0..c
+00000340: 6f6c 6f72 5f6d 6170 3d6a 6574 0d0a 2320  olor_map=jet..# 
+00000350: 7363 6174 7465 7220 6f70 7469 6f6e 730d  scatter options.
+00000360: 0a6d 6172 6b65 7273 697a 653d 302e 322c  .markersize=0.2,
+00000370: 302e 320d 0a6d 6172 6b65 723d 6f2c 762c  0.2..marker=o,v,
+00000380: 5e2c 440d 0a23 2066 6572 6d69 0d0a 6665  ^,D..# fermi..fe
+00000390: 726d 695f 636f 6c6f 723d 626c 6163 6b0d  rmi_color=black.
+000003a0: 0a66 6572 6d69 5f6c 696e 6573 7479 6c65  .fermi_linestyle
+000003b0: 3d64 6f74 7465 640d 0a66 6572 6d69 5f6c  =dotted..fermi_l
+000003c0: 696e 6577 6964 7468 3d31 0d0a 2320 6772  inewidth=1..# gr
+000003d0: 6964 206f 7074 696f 6e73 0d0a 6772 6964  id options..grid
+000003e0: 3d46 616c 7365 0d0a 6772 6964 5f77 6869  =False..grid_whi
+000003f0: 6368 3d6d 616a 6f72 200d 0a67 7269 645f  ch=major ..grid_
+00000400: 6178 6973 3d62 6f74 6820 0d0a 6772 6964  axis=both ..grid
+00000410: 5f63 6f6c 6f72 3d67 7265 790d 0a67 7269  _color=grey..gri
+00000420: 645f 6c69 6e65 7374 796c 653d 736f 6c69  d_linestyle=soli
+00000430: 640d 0a67 7269 645f 6c69 6e65 7769 6474  d..grid_linewidt
+00000440: 683d 310d 0a23 2077 6569 6768 7420 6f70  h=1..# weight op
+00000450: 7469 6f6e 730d 0a77 6569 6768 7465 645f  tions..weighted_
+00000460: 7769 6474 683d 4661 6c73 650d 0a77 6569  width=False..wei
+00000470: 6768 7465 645f 636f 6c6f 723d 5472 7565  ghted_color=True
+00000480: 0d0a 6c65 6765 6e64 3d54 7275 650d 0a73  ..legend=True..s
+00000490: 6176 6566 6967 3d4e 6f6e 650d 0a70 6c6f  avefig=None..plo
+000004a0: 745f 636f 6c6f 725f 6261 723d 5472 7565  t_color_bar=True
+000004b0: 0d0a 7469 746c 653d 4e6f 6e65 0d0a 0d0a  ..title=None....
+000004c0: 0d0a 5b75 6e66 6f6c 645d 0d0a 2320 6c69  ..[unfold]..# li
+000004d0: 6e65 206f 7074 696f 6e73 2c20 0d0a 6c69  ne options, ..li
+000004e0: 6e65 7374 796c 653d 736f 6c69 642c 2064  nestyle=solid, d
+000004f0: 6173 6865 6420 0d0a 6c69 6e65 7769 6474  ashed ..linewidt
+00000500: 683d 312c 310d 0a63 6f6c 6f72 3d62 6c61  h=1,1..color=bla
+00000510: 636b 2c20 626c 6163 6b0d 0a6c 6162 656c  ck, black..label
+00000520: 3d24 5c75 7061 7272 6f77 242c 245c 646f  =$\uparrow$,$\do
+00000530: 776e 6172 726f 7724 0d0a 6f70 6163 6974  wnarrow$..opacit
+00000540: 793d 302e 332c 2030 2e33 0d0a 636f 6c6f  y=0.3, 0.3..colo
+00000550: 725f 6d61 703d 5265 6473 0d0a 2320 7363  r_map=Reds..# sc
+00000560: 6174 7465 7220 6f70 7469 6f6e 730d 0a6d  atter options..m
+00000570: 6172 6b65 7273 697a 653d 302e 322c 302e  arkersize=0.2,0.
+00000580: 320d 0a6d 6172 6b65 723d 6f2c 762c 5e2c  2..marker=o,v,^,
+00000590: 440d 0a23 2066 6572 6d69 0d0a 6665 726d  D..# fermi..ferm
+000005a0: 695f 636f 6c6f 723d 626c 7565 0d0a 6665  i_color=blue..fe
+000005b0: 726d 695f 6c69 6e65 7374 796c 653d 646f  rmi_linestyle=do
+000005c0: 7474 6564 0d0a 6665 726d 695f 6c69 6e65  tted..fermi_line
+000005d0: 7769 6474 683d 310d 0a23 2067 7269 6420  width=1..# grid 
+000005e0: 6f70 7469 6f6e 730d 0a67 7269 643d 4661  options..grid=Fa
+000005f0: 6c73 650d 0a67 7269 645f 7768 6963 683d  lse..grid_which=
+00000600: 6d61 6a6f 7220 0d0a 6772 6964 5f61 7869  major ..grid_axi
+00000610: 733d 626f 7468 200d 0a67 7269 645f 636f  s=both ..grid_co
+00000620: 6c6f 723d 6772 6579 0d0a 6772 6964 5f6c  lor=grey..grid_l
+00000630: 696e 6573 7479 6c65 3d73 6f6c 6964 0d0a  inestyle=solid..
+00000640: 6772 6964 5f6c 696e 6577 6964 7468 3d31  grid_linewidth=1
+00000650: 0d0a 2320 7765 6967 6874 206f 7074 696f  ..# weight optio
+00000660: 6e73 0d0a 7765 6967 6874 6564 5f77 6964  ns..weighted_wid
+00000670: 7468 3d46 616c 7365 0d0a 7765 6967 6874  th=False..weight
+00000680: 6564 5f63 6f6c 6f72 3d54 7275 650d 0a6c  ed_color=True..l
+00000690: 6567 656e 643d 5472 7565 0d0a 7361 7665  egend=True..save
+000006a0: 6669 673d 4e6f 6e65 0d0a 706c 6f74 5f63  fig=None..plot_c
+000006b0: 6f6c 6f72 5f62 6172 3d54 7275 650d 0a74  olor_bar=True..t
+000006c0: 6974 6c65 3d4e 6f6e 650d 0a              itle=None..
```

### Comparing `PyProcar-6.0.0/pyprocar/utils/defaults.py` & `PyProcar-6.1.0/pyprocar/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/utils/download_examples.py` & `PyProcar-6.1.0/pyprocar/utils/download_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,28 @@
                             'bands':'',
                             'dos':'',
                             'fermi':''}
                         }
 
 
                     },
+
+                "BiSb_monolayer" :
+                    {"vasp": 
+                        {
+                        'non-colinear':
+                            {
+                            'bands':'',
+                            'dos':'',
+                            'fermi':'192XJLLpd7knvazhJPbhcV0Jb75NZM7OF'},
+
+
+                    },
                 }
+    }
 
 
 def download_examples(save_dir=''):
     if save_dir != '':
         output = f"{save_dir}{os.sep}examples.zip"
         to = f"{save_dir}{os.sep}examples{os.sep}"
     else:
@@ -83,15 +96,15 @@
     project_dir = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
     data_dir = os.path.join(project_dir, 'data')
 
     material_name = 'Fe'
 
     print('Storing development data in', data_dir)
     if not os.path.exists(data_dir):
-        os.mkdirs(data_dir) 
+        os.mkdir(data_dir) 
 
     # output = f"{data_dir}{os.sep}{examples_dirname}"
     to = f"{data_dir}{os.sep}{examples_dirname}{os.sep}{material_name}"
 
     print('___Starting download___')
     url  = f'https://drive.google.com/drive/folders/1FQ5suC2e-Wp9LfWQqeb_2pRJDO00QQvQ'
     gdown.download_folder(url=url, output=to,use_cookies=False,remaining_ok=True)
```

### Comparing `PyProcar-6.0.0/pyprocar/utils/elements.py` & `PyProcar-6.1.0/pyprocar/utils/elements.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/utils/info.py` & `PyProcar-6.1.0/pyprocar/utils/info.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/utils/procarfilefilter.py` & `PyProcar-6.1.0/pyprocar/utils/procarfilefilter.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/utils/scriptFermi3D.py` & `PyProcar-6.1.0/pyprocar/utils/scriptFermi3D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/utils/splash.py` & `PyProcar-6.1.0/pyprocar/utils/splash.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/utils/unfolder.py` & `PyProcar-6.1.0/pyprocar/utils/unfolder.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/utils/utilsprocar.py` & `PyProcar-6.1.0/pyprocar/utils/utilsprocar.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/pyprocar/version.py` & `PyProcar-6.1.0/pyprocar/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # THIS FILE IS GENERATED FROM PYPROCAR SETUP.PY.
 name = 'PyProcar'
-version = '6.0.0'
+version = '6.1.0'
 description = 'A Python library for electronic structure pre/post-processing. '
 author = 'Francisco Muñoz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah'
 email = 'fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com'
 url = 'https://github.com/romerogroup/pyprocar'
-download_url = 'https://github.com/romerogroup/pyprocar/archive/6.0.0.tar.gz'
+download_url = 'https://github.com/romerogroup/pyprocar/archive/6.1.0.tar.gz'
 status = 'development'
 copyright = 'Copyright 2021'
 date = 'Jun 10th, 2021'
```

### Comparing `PyProcar-6.0.0/scripts/procar.py` & `PyProcar-6.1.0/scripts/procar.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.0.0/setup.json` & `PyProcar-6.1.0/setup.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'download_url'": "'https://github.com/romerogroup/pyprocar/archive/6.1.0.tar.gz'",*

 * * "'version'": "'6.1.0'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "author": "Francisco Mu\u00f1oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah",
     "copyright": "Copyright 2021",
     "date": "Jun 10th, 2021",
     "description": "A Python library for electronic structure pre/post-processing. ",
-    "download_url": "https://github.com/romerogroup/pyprocar/archive/6.0.0.tar.gz",
+    "download_url": "https://github.com/romerogroup/pyprocar/archive/6.1.0.tar.gz",
     "email": "fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com",
     "name": "PyProcar",
     "status": "development",
     "url": "https://github.com/romerogroup/pyprocar",
-    "version": "6.0.0"
+    "version": "6.1.0"
 }
```

### Comparing `PyProcar-6.0.0/setup.py` & `PyProcar-6.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,13 +44,16 @@
         'numpy',
         'pyvista',
         'scikit-image',
         'scipy',
         'seekpath',
         'spglib',
         'trimesh',
+        'ase',
+        'sympy',
+        'PyYAML',
     ],
     data_files=[("", ["LICENSE"])],
     package_data={"": ["setup.json", '*.ini']},
     scripts=["scripts/procar.py"],
     packages=find_packages(exclude=["scripts"]),
 )
```

