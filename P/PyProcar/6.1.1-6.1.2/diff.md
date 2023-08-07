# Comparing `tmp/PyProcar-6.1.1.tar.gz` & `tmp/PyProcar-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProcar-6.1.1.tar", last modified: Mon Aug  7 07:56:13 2023, max compression
+gzip compressed data, was "PyProcar-6.1.2.tar", last modified: Mon Aug  7 19:13:32 2023, max compression
```

## Comparing `PyProcar-6.1.1.tar` & `PyProcar-6.1.2.tar`

### file list

```diff
@@ -1,133 +1,140 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.095854 PyProcar-6.1.1/
--rw-rw-rw-   0        0        0     1655 2023-05-08 12:33:46.000000 PyProcar-6.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0    43233 2023-05-08 12:33:46.000000 PyProcar-6.1.1/LICENSE
--rw-rw-rw-   0        0        0       62 2023-05-08 12:33:46.000000 PyProcar-6.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      633 2023-08-07 07:56:13.095854 PyProcar-6.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.925622 PyProcar-6.1.1/PyProcar.egg-info/
--rw-rw-rw-   0        0        0      633 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3477 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9936 2023-08-07 07:54:40.000000 PyProcar-6.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.933630 PyProcar-6.1.1/pyprocar/
--rw-rw-rw-   0        0        0     2531 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.952646 PyProcar-6.1.1/pyprocar/core/
--rw-rw-rw-   0        0        0      520 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/__init__.py
--rw-rw-rw-   0        0        0    11350 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/bandstructure2D.py
--rw-rw-rw-   0        0        0     7424 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/brillouin_zone.py
--rw-rw-rw-   0        0        0    12198 2023-05-25 16:01:56.000000 PyProcar-6.1.1/pyprocar/core/dos.py
--rw-rw-rw-   0        0        0    46780 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/ebs.py
--rw-rw-rw-   0        0        0    19863 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/fermisurface.py
--rw-rw-rw-   0        0        0    14186 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/fermisurface3D.py
--rw-rw-rw-   0        0        0    14086 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/isosurface.py
--rw-rw-rw-   0        0        0    10122 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/kpath.py
--rw-rw-rw-   0        0        0     8578 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarselect.py
--rw-rw-rw-   0        0        0     8712 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarsymmetry.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.959653 PyProcar-6.1.1/pyprocar/core/procarunfold/
--rw-rw-rw-   0        0        0       45 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/__init__.py
--rw-rw-rw-   0        0        0    24502 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/_bak.procarparser.py
--rw-rw-rw-   0        0        0     5383 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/fatband.py
--rw-rw-rw-   0        0        0     4532 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/procar_unfolder.py
--rw-rw-rw-   0        0        0     5154 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/unfolder.py
--rw-rw-rw-   0        0        0    15028 2023-07-02 20:40:25.000000 PyProcar-6.1.1/pyprocar/core/structure.py
--rw-rw-rw-   0        0        0    11061 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/surface.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.975113 PyProcar-6.1.1/pyprocar/io/
--rw-rw-rw-   0        0        0      904 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/io/__init__.py
--rw-rw-rw-   0        0        0    21922 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/io/abinit.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.978117 PyProcar-6.1.1/pyprocar/io/abinitparser/
--rw-rw-rw-   0        0        0       41 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/abinitparser/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/abinitparser/abinitparser.py
--rw-rw-rw-   0        0        0     5879 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/bxsf.py
--rw-rw-rw-   0        0        0    14822 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/elk.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.980118 PyProcar-6.1.1/pyprocar/io/elkparser/
--rw-rw-rw-   0        0        0       34 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/elkparser/__init__.py
--rw-rw-rw-   0        0        0    11433 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/elkparser/elkparser.py
--rw-rw-rw-   0        0        0     3124 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/frmsf.py
--rw-rw-rw-   0        0        0    33353 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobster.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.989126 PyProcar-6.1.1/pyprocar/io/lobsterparser/
--rw-rw-rw-   0        0        0      145 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobsterparser/__init__.py
--rw-rw-rw-   0        0        0    21053 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobsterparser/lobster_doscar_parser.py
--rw-rw-rw-   0        0        0    15675 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobsterparser/lobsterfermiparser.py
--rw-rw-rw-   0        0        0    15388 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobsterparser/lobsterparser.py
--rw-rw-rw-   0        0        0     7146 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/io/parser.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.993130 PyProcar-6.1.1/pyprocar/io/procarparser/
--rw-rw-rw-   0        0        0       74 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/procarparser/__init__.py
--rw-rw-rw-   0        0        0    31346 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/procarparser/procarparser.py
--rw-rw-rw-   0        0        0    44082 2023-05-25 18:06:53.000000 PyProcar-6.1.1/pyprocar/io/qe.py
--rw-rw-rw-   0        0        0     9911 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/siesta.py
--rw-rw-rw-   0        0        0    81931 2023-08-07 07:29:04.000000 PyProcar-6.1.1/pyprocar/io/vasp.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.998134 PyProcar-6.1.1/pyprocar/io/vaspxml/
--rw-rw-rw-   0        0        0       55 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/vaspxml/__init__.py
--rw-rw-rw-   0        0        0    25252 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/vaspxml/vaspxml.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.008144 PyProcar-6.1.1/pyprocar/plotter/
--rw-rw-rw-   0        0        0      259 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/__init__.py
--rw-rw-rw-   0        0        0    24628 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/bs_2d_plot.py
--rw-rw-rw-   0        0        0    51396 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/dos_plot.py
--rw-rw-rw-   0        0        0    21705 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/ebs_plot.py
--rw-rw-rw-   0        0        0    45163 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/fermi3d_plot.py
--rw-rw-rw-   0        0        0    14084 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/plotter/procarplot.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.037170 PyProcar-6.1.1/pyprocar/pyposcar/
--rw-rw-rw-   0        0        0      177 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/__init__.py
--rw-rw-rw-   0        0        0     1425 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/analize.py
--rw-rw-rw-   0        0        0    19751 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/chg_raw.py
--rw-rw-rw-   0        0        0    11407 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/clusters.py
--rw-rw-rw-   0        0        0      961 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/db.py
--rw-rw-rw-   0        0        0     4077 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/dbCovalentBond.py
--rw-rw-rw-   0        0        0    14105 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/defects.py
--rw-rw-rw-   0        0        0      803 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/generalUtils.py
--rw-rw-rw-   0        0        0    11870 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/honeycomb.py
--rw-rw-rw-   0        0        0     6195 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/latticeUtils.py
--rw-rw-rw-   0        0        0     1885 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/outcarParser.py
--rw-rw-rw-   0        0        0     5191 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/plot3d.py
--rw-rw-rw-   0        0        0     5647 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/plotbands.py
--rw-rw-rw-   0        0        0    15418 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/poscar.py
--rw-rw-rw-   0        0        0    27247 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/poscarUtils.py
--rw-rw-rw-   0        0        0     7039 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/rdf.py
--rw-rw-rw-   0        0        0    12574 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/relax-cell-2d.py
--rw-rw-rw-   0        0        0      190 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/test.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.073834 PyProcar-6.1.1/pyprocar/scripts/
--rw-rw-rw-   0        0        0      808 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/depreciated_scriptVector.py
--rw-rw-rw-   0        0        0     1552 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandGap.py
--rw-rw-rw-   0        0        0     6603 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandStructure2DHandler.py
--rw-rw-rw-   0        0        0     8920 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandsDosplot.py
--rw-rw-rw-   0        0        0     8610 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandsplot.py
--rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandsplot_2d.py
--rw-rw-rw-   0        0        0    10120 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptCat.py
--rw-rw-rw-   0        0        0    13416 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptDosplot.py
--rw-rw-rw-   0        0        0     8872 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptFermi2D.py
--rw-rw-rw-   0        0        0    33281 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptFermi3D.py
--rw-rw-rw-   0        0        0    13173 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptFermiHandler.py
--rw-rw-rw-   0        0        0     3238 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptFilter.py
--rw-rw-rw-   0        0        0     1333 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptKmesh2D.py
--rw-rw-rw-   0        0        0     3977 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptKpath.py
--rw-rw-rw-   0        0        0      526 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptRepair.py
--rw-rw-rw-   0        0        0     7841 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptSpin_asymmetry.py
--rw-rw-rw-   0        0        0    11385 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptUnfold.py
--rw-rw-rw-   0        0        0    25137 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_new.py
--rw-rw-rw-   0        0        0     2986 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_old.py
--rw-rw-rw-   0        0        0     6675 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_v2.py
--rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptVector.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.092851 PyProcar-6.1.1/pyprocar/utils/
--rw-rw-rw-   0        0        0     1562 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/utils/__init__.py
--rw-rw-rw-   0        0        0     1739 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/utils/default_settings.ini
--rw-rw-rw-   0        0        0     3183 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/defaults.py
--rw-rw-rw-   0        0        0     5790 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/utils/download_examples.py
--rw-rw-rw-   0        0        0     4891 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/elements.py
--rw-rw-rw-   0        0        0     2403 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/info.py
--rw-rw-rw-   0        0        0     2994 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/utils/mathematics.py
--rw-rw-rw-   0        0        0    18332 2023-08-06 22:53:59.000000 PyProcar-6.1.1/pyprocar/utils/procarfilefilter.py
--rw-rw-rw-   0        0        0    28441 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/scriptFermi3D.py
--rw-rw-rw-   0        0        0      403 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/sorting.py
--rw-rw-rw-   0        0        0      975 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/splash.py
--rw-rw-rw-   0        0        0     6062 2023-08-06 21:34:44.000000 PyProcar-6.1.1/pyprocar/utils/unfolder.py
--rw-rw-rw-   0        0        0    10954 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/utilsprocar.py
--rw-rw-rw-   0        0        0      688 2023-08-07 07:56:12.000000 PyProcar-6.1.1/pyprocar/version.py
--rw-rw-rw-   0        0        0      103 2023-08-07 06:46:20.000000 PyProcar-6.1.1/requirements.txt
--rw-rw-rw-   0        0        0      259 2023-08-07 06:55:41.000000 PyProcar-6.1.1/requirements_docs.txt
-drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.093852 PyProcar-6.1.1/scripts/
--rw-rw-rw-   0        0        0    33462 2023-05-08 12:33:47.000000 PyProcar-6.1.1/scripts/procar.py
--rw-rw-rw-   0        0        0       86 2023-08-07 07:56:13.102860 PyProcar-6.1.1/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-08-07 07:46:29.000000 PyProcar-6.1.1/setup.json
--rw-rw-rw-   0        0        0     1643 2023-08-07 06:46:20.000000 PyProcar-6.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.359401 PyProcar-6.1.2/
+-rw-rw-rw-   0        0        0     1655 2023-05-08 12:33:46.000000 PyProcar-6.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0    43233 2023-05-08 12:33:46.000000 PyProcar-6.1.2/LICENSE
+-rw-rw-rw-   0        0        0       62 2023-05-08 12:33:46.000000 PyProcar-6.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      633 2023-08-07 19:13:32.359401 PyProcar-6.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.163223 PyProcar-6.1.2/PyProcar.egg-info/
+-rw-rw-rw-   0        0        0      633 2023-08-07 19:13:31.000000 PyProcar-6.1.2/PyProcar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3658 2023-08-07 19:13:32.000000 PyProcar-6.1.2/PyProcar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 19:13:31.000000 PyProcar-6.1.2/PyProcar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-08-07 19:13:31.000000 PyProcar-6.1.2/PyProcar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 19:13:31.000000 PyProcar-6.1.2/PyProcar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9991 2023-08-07 19:12:15.000000 PyProcar-6.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.174233 PyProcar-6.1.2/pyprocar/
+-rw-rw-rw-   0        0        0     2531 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.183241 PyProcar-6.1.2/pyprocar/cfg/
+-rw-rw-rw-   0        0        0        0 2023-08-07 18:56:07.000000 PyProcar-6.1.2/pyprocar/cfg/__init__.py
+-rw-rw-rw-   0        0        0     2446 2023-08-07 17:20:51.000000 PyProcar-6.1.2/pyprocar/cfg/band_structure.yml
+-rw-rw-rw-   0        0        0     3749 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/cfg/band_structure_2d.yml
+-rw-rw-rw-   0        0        0     3239 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/cfg/dos.yml
+-rw-rw-rw-   0        0        0     1441 2023-08-07 17:20:51.000000 PyProcar-6.1.2/pyprocar/cfg/fermi_surface_2d.yml
+-rw-rw-rw-   0        0        0     3804 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/cfg/fermi_surface_3d.yml
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.205260 PyProcar-6.1.2/pyprocar/core/
+-rw-rw-rw-   0        0        0      520 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/core/__init__.py
+-rw-rw-rw-   0        0        0    11350 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/core/bandstructure2D.py
+-rw-rw-rw-   0        0        0     7424 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/core/brillouin_zone.py
+-rw-rw-rw-   0        0        0    12198 2023-05-25 16:01:56.000000 PyProcar-6.1.2/pyprocar/core/dos.py
+-rw-rw-rw-   0        0        0    46780 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/core/ebs.py
+-rw-rw-rw-   0        0        0    19931 2023-08-07 17:20:51.000000 PyProcar-6.1.2/pyprocar/core/fermisurface.py
+-rw-rw-rw-   0        0        0    14186 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/core/fermisurface3D.py
+-rw-rw-rw-   0        0        0    14086 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/core/isosurface.py
+-rw-rw-rw-   0        0        0    10122 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/core/kpath.py
+-rw-rw-rw-   0        0        0     8578 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/core/procarselect.py
+-rw-rw-rw-   0        0        0     8712 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/core/procarsymmetry.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.214269 PyProcar-6.1.2/pyprocar/core/procarunfold/
+-rw-rw-rw-   0        0        0       45 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/core/procarunfold/__init__.py
+-rw-rw-rw-   0        0        0    24502 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/core/procarunfold/_bak.procarparser.py
+-rw-rw-rw-   0        0        0     5383 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/core/procarunfold/fatband.py
+-rw-rw-rw-   0        0        0     4532 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/core/procarunfold/procar_unfolder.py
+-rw-rw-rw-   0        0        0     5154 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/core/procarunfold/unfolder.py
+-rw-rw-rw-   0        0        0    15028 2023-07-02 20:40:25.000000 PyProcar-6.1.2/pyprocar/core/structure.py
+-rw-rw-rw-   0        0        0    11061 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/core/surface.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.231284 PyProcar-6.1.2/pyprocar/io/
+-rw-rw-rw-   0        0        0      904 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/io/__init__.py
+-rw-rw-rw-   0        0        0    21922 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/io/abinit.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.235289 PyProcar-6.1.2/pyprocar/io/abinitparser/
+-rw-rw-rw-   0        0        0       41 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/abinitparser/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/abinitparser/abinitparser.py
+-rw-rw-rw-   0        0        0     5879 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/bxsf.py
+-rw-rw-rw-   0        0        0    14822 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/elk.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.238290 PyProcar-6.1.2/pyprocar/io/elkparser/
+-rw-rw-rw-   0        0        0       34 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/elkparser/__init__.py
+-rw-rw-rw-   0        0        0    11433 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/elkparser/elkparser.py
+-rw-rw-rw-   0        0        0     3124 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/frmsf.py
+-rw-rw-rw-   0        0        0    33353 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/lobster.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.245297 PyProcar-6.1.2/pyprocar/io/lobsterparser/
+-rw-rw-rw-   0        0        0      145 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/lobsterparser/__init__.py
+-rw-rw-rw-   0        0        0    21053 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/lobsterparser/lobster_doscar_parser.py
+-rw-rw-rw-   0        0        0    15675 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/lobsterparser/lobsterfermiparser.py
+-rw-rw-rw-   0        0        0    15388 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/lobsterparser/lobsterparser.py
+-rw-rw-rw-   0        0        0     7146 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/io/parser.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.249300 PyProcar-6.1.2/pyprocar/io/procarparser/
+-rw-rw-rw-   0        0        0       74 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/procarparser/__init__.py
+-rw-rw-rw-   0        0        0    31346 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/procarparser/procarparser.py
+-rw-rw-rw-   0        0        0    44082 2023-05-25 18:06:53.000000 PyProcar-6.1.2/pyprocar/io/qe.py
+-rw-rw-rw-   0        0        0     9911 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/siesta.py
+-rw-rw-rw-   0        0        0    81931 2023-08-07 17:20:51.000000 PyProcar-6.1.2/pyprocar/io/vasp.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.253304 PyProcar-6.1.2/pyprocar/io/vaspxml/
+-rw-rw-rw-   0        0        0       55 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/vaspxml/__init__.py
+-rw-rw-rw-   0        0        0    25252 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/io/vaspxml/vaspxml.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.263313 PyProcar-6.1.2/pyprocar/plotter/
+-rw-rw-rw-   0        0        0      259 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/plotter/__init__.py
+-rw-rw-rw-   0        0        0    24628 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/plotter/bs_2d_plot.py
+-rw-rw-rw-   0        0        0    51396 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/plotter/dos_plot.py
+-rw-rw-rw-   0        0        0    21773 2023-08-07 17:20:51.000000 PyProcar-6.1.2/pyprocar/plotter/ebs_plot.py
+-rw-rw-rw-   0        0        0    45163 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/plotter/fermi3d_plot.py
+-rw-rw-rw-   0        0        0    14084 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/plotter/procarplot.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.295342 PyProcar-6.1.2/pyprocar/pyposcar/
+-rw-rw-rw-   0        0        0      177 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/pyposcar/__init__.py
+-rw-rw-rw-   0        0        0     1425 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/analize.py
+-rw-rw-rw-   0        0        0    19751 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/chg_raw.py
+-rw-rw-rw-   0        0        0    11407 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/clusters.py
+-rw-rw-rw-   0        0        0      961 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/pyposcar/db.py
+-rw-rw-rw-   0        0        0     4077 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/dbCovalentBond.py
+-rw-rw-rw-   0        0        0    14105 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/defects.py
+-rw-rw-rw-   0        0        0      803 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/generalUtils.py
+-rw-rw-rw-   0        0        0    11870 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/honeycomb.py
+-rw-rw-rw-   0        0        0     6195 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/pyposcar/latticeUtils.py
+-rw-rw-rw-   0        0        0     1885 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/outcarParser.py
+-rw-rw-rw-   0        0        0     5191 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/plot3d.py
+-rw-rw-rw-   0        0        0     5647 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/plotbands.py
+-rw-rw-rw-   0        0        0    15418 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/pyposcar/poscar.py
+-rw-rw-rw-   0        0        0    27247 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/pyposcar/poscarUtils.py
+-rw-rw-rw-   0        0        0     7039 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/pyposcar/rdf.py
+-rw-rw-rw-   0        0        0    12574 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/relax-cell-2d.py
+-rw-rw-rw-   0        0        0      190 2023-07-01 06:22:02.000000 PyProcar-6.1.2/pyprocar/pyposcar/test.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.332424 PyProcar-6.1.2/pyprocar/scripts/
+-rw-rw-rw-   0        0        0      808 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/depreciated_scriptVector.py
+-rw-rw-rw-   0        0        0     1552 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptBandGap.py
+-rw-rw-rw-   0        0        0     6605 2023-08-07 17:20:51.000000 PyProcar-6.1.2/pyprocar/scripts/scriptBandStructure2DHandler.py
+-rw-rw-rw-   0        0        0     8920 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/scripts/scriptBandsDosplot.py
+-rw-rw-rw-   0        0        0     8269 2023-08-07 17:20:51.000000 PyProcar-6.1.2/pyprocar/scripts/scriptBandsplot.py
+-rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptBandsplot_2d.py
+-rw-rw-rw-   0        0        0    10120 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptCat.py
+-rw-rw-rw-   0        0        0    13416 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/scripts/scriptDosplot.py
+-rw-rw-rw-   0        0        0     8870 2023-08-07 17:20:51.000000 PyProcar-6.1.2/pyprocar/scripts/scriptFermi2D.py
+-rw-rw-rw-   0        0        0    33281 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/scripts/scriptFermi3D.py
+-rw-rw-rw-   0        0        0    13173 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/scripts/scriptFermiHandler.py
+-rw-rw-rw-   0        0        0     3238 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptFilter.py
+-rw-rw-rw-   0        0        0     1333 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptKmesh2D.py
+-rw-rw-rw-   0        0        0     3977 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptKpath.py
+-rw-rw-rw-   0        0        0      526 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptRepair.py
+-rw-rw-rw-   0        0        0     7841 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptSpin_asymmetry.py
+-rw-rw-rw-   0        0        0    11385 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptUnfold.py
+-rw-rw-rw-   0        0        0    25137 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptUnfold_new.py
+-rw-rw-rw-   0        0        0     2986 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptUnfold_old.py
+-rw-rw-rw-   0        0        0     6675 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptUnfold_v2.py
+-rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/scripts/scriptVector.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.356398 PyProcar-6.1.2/pyprocar/utils/
+-rw-rw-rw-   0        0        0     1562 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1739 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/utils/default_settings.ini
+-rw-rw-rw-   0        0        0     3183 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/utils/defaults.py
+-rw-rw-rw-   0        0        0     5790 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/utils/download_examples.py
+-rw-rw-rw-   0        0        0     4891 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/utils/elements.py
+-rw-rw-rw-   0        0        0     2403 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/utils/info.py
+-rw-rw-rw-   0        0        0     2994 2023-08-07 06:46:20.000000 PyProcar-6.1.2/pyprocar/utils/mathematics.py
+-rw-rw-rw-   0        0        0    18332 2023-08-06 22:53:59.000000 PyProcar-6.1.2/pyprocar/utils/procarfilefilter.py
+-rw-rw-rw-   0        0        0    28441 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/utils/scriptFermi3D.py
+-rw-rw-rw-   0        0        0      403 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/utils/sorting.py
+-rw-rw-rw-   0        0        0      975 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/utils/splash.py
+-rw-rw-rw-   0        0        0     6062 2023-08-06 21:34:44.000000 PyProcar-6.1.2/pyprocar/utils/unfolder.py
+-rw-rw-rw-   0        0        0    10954 2023-05-08 12:33:47.000000 PyProcar-6.1.2/pyprocar/utils/utilsprocar.py
+-rw-rw-rw-   0        0        0      688 2023-08-07 19:13:31.000000 PyProcar-6.1.2/pyprocar/version.py
+-rw-rw-rw-   0        0        0      103 2023-08-07 06:46:20.000000 PyProcar-6.1.2/requirements.txt
+-rw-rw-rw-   0        0        0      259 2023-08-07 17:20:51.000000 PyProcar-6.1.2/requirements_docs.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 19:13:32.357399 PyProcar-6.1.2/scripts/
+-rw-rw-rw-   0        0        0    33462 2023-05-08 12:33:47.000000 PyProcar-6.1.2/scripts/procar.py
+-rw-rw-rw-   0        0        0       86 2023-08-07 19:13:32.361402 PyProcar-6.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-08-07 18:57:44.000000 PyProcar-6.1.2/setup.json
+-rw-rw-rw-   0        0        0     1651 2023-08-07 18:56:07.000000 PyProcar-6.1.2/setup.py
```

### Comparing `PyProcar-6.1.1/AUTHORS.rst` & `PyProcar-6.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/LICENSE` & `PyProcar-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/PKG-INFO` & `PyProcar-6.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: PyProcar
-Version: 6.1.1
+Version: 6.1.2
 Summary: A Python library for electronic structure pre/post-processing. 
 Home-page: https://github.com/romerogroup/pyprocar
 Author: Francisco MuÃ±oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
 Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
 License: LICENSE
-Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.1.tar.gz
+Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.2.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `PyProcar-6.1.1/PyProcar.egg-info/PKG-INFO` & `PyProcar-6.1.2/PyProcar.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: PyProcar
-Version: 6.1.1
+Version: 6.1.2
 Summary: A Python library for electronic structure pre/post-processing. 
 Home-page: https://github.com/romerogroup/pyprocar
 Author: Francisco MuÃ±oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
 Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
 License: LICENSE
-Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.1.tar.gz
+Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.2.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `PyProcar-6.1.1/PyProcar.egg-info/SOURCES.txt` & `PyProcar-6.1.2/PyProcar.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 PyProcar.egg-info/PKG-INFO
 PyProcar.egg-info/SOURCES.txt
 PyProcar.egg-info/dependency_links.txt
 PyProcar.egg-info/requires.txt
 PyProcar.egg-info/top_level.txt
 pyprocar/__init__.py
 pyprocar/version.py
+pyprocar/cfg/__init__.py
+pyprocar/cfg/band_structure.yml
+pyprocar/cfg/band_structure_2d.yml
+pyprocar/cfg/dos.yml
+pyprocar/cfg/fermi_surface_2d.yml
+pyprocar/cfg/fermi_surface_3d.yml
 pyprocar/core/__init__.py
 pyprocar/core/bandstructure2D.py
 pyprocar/core/brillouin_zone.py
 pyprocar/core/dos.py
 pyprocar/core/ebs.py
 pyprocar/core/fermisurface.py
 pyprocar/core/fermisurface3D.py
```

### Comparing `PyProcar-6.1.1/README.md` & `PyProcar-6.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 5. Lobster (Stll in development)
 
 ![](welcome.png)
 
 Documentation
 -------------
 
-For versions 6.1.1 and above, the documentation is found here:
+For versions 6.1.2 and above, the documentation is found here:
 https://romerogroup.github.io/pyprocar/
 
 
 The prior documentation is found here:
 https://romerogroup.github.io/pyprocar5.6.6/
 
 
@@ -117,14 +117,15 @@
 
     procar.py -h
 
 will bring a help menu.
 
 Changelog
 --------------
+v6.1.2 Aug 7th, 2023 -- Bug fix and doc update <br />
 v6.1.1 Aug 7th, 2023 -- Bug fix <br />
 v6.1.0 Aug 7th, 2023 -- Bug fixes, doc update, config files <br />
 v6.0.0 Jun 10th, 2023 -- Major code base changes. <br />
 v5.6.6 Mar 6th, 2022 -- QE, bandsplot, dosplot, fermi surface, and band unfolding bug fixes. Directory change, parsers are now in the io directory. <br />
 v5.6.5 Jun 10th, 2021 -- Fermi surface object and fermi surface plotter bug fixes <br />
 v5.6.4 May 6th, 2021 -- Updates to Fermi surface plotter. <br />
 v5.6.3 Mar 5th, 2021 -- QE and elk bug fixes. <br />
```

### Comparing `PyProcar-6.1.1/pyprocar/__init__.py` & `PyProcar-6.1.2/pyprocar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/__init__.py` & `PyProcar-6.1.2/pyprocar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/bandstructure2D.py` & `PyProcar-6.1.2/pyprocar/core/bandstructure2D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/brillouin_zone.py` & `PyProcar-6.1.2/pyprocar/core/brillouin_zone.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/dos.py` & `PyProcar-6.1.2/pyprocar/core/dos.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/ebs.py` & `PyProcar-6.1.2/pyprocar/core/ebs.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/fermisurface.py` & `PyProcar-6.1.2/pyprocar/core/fermisurface.py`

 * *Files 5% similar despite different names*

```diff
@@ -195,28 +195,27 @@
 
             # Normalizing
             vmin=self.plot_opt['clim']['value'][0]
             vmax=self.plot_opt['clim']['value'][1]
             if vmin is None:
                 vmin=spd.min()
             if vmax is None:
-                vmax = spd.max()           
+                vmax=spd.max()           
             norm = mpcolors.Normalize(vmin, vmax)
 
             # Interpolating band energies on to new grid
             bnew = []
             for i_band, band in enumerate(bands):
                 self.log.debug("Interpolating ...")
                 bnew.append(griddata((x, y), band, (xnew, ynew), method="cubic"))
             bnew = np.array(bnew)
 
             # Generates colors per band
             
             n_bands = bands.shape[0]
-            norm = mpcolors.Normalize(vmin=0, vmax=1)
             cmap = cm.get_cmap(self.plot_opt['cmap']['value'])
             if i_spin == 1:
                 factor = 0.25
             else:
                 factor = 0
             solid_color_surface = np.arange(n_bands) / n_bands + factor
             band_colors = np.array([cmap(norm(x)) for x in solid_color_surface[:]]).reshape(-1, 4)
@@ -309,29 +308,38 @@
             bands = self.bands[:,self.band_indices[0],0].transpose()
 
             band_labels = np.unique(self.band_indices[0])
             sx = sx[:,self.band_indices[0]].transpose()
             sy = sy[:,self.band_indices[0]].transpose()
             sz = sz[:,self.band_indices[0]].transpose()
 
-
+       
         # and new, interpolated component
         xmax, xmin = x.max(), x.min()
         ymax, ymin = y.max(), y.min()
         self.log.debug("xlim = " + str([xmin, xmax]) + "  ylim = " + str([ymin, ymax]))
         xnew, ynew = np.mgrid[
             xmin : xmax : interpolation * 1j, ymin : ymax : interpolation * 1j
         ]
 
         # interpolation
         bnew = []
         for band in bands:
             self.log.debug("Interpolating ...")
             bnew.append(griddata((x, y), band, (xnew, ynew), method="cubic"))
 
+        # Normalizing
+        vmin=self.plot_opt['clim']['value'][0]
+        vmax=self.plot_opt['clim']['value'][1]
+        if vmin is None:
+            vmin=-0.5
+        if vmax is None:
+            vmax=0.5          
+        norm = mpcolors.Normalize(vmin, vmax)
+
 
         cont = [
             plt.contour(
                 xnew,
                 ynew,
                 z,
                 [self.energy],
@@ -339,110 +347,108 @@
                 colors="k",
                 linestyles="solid",
             )
             for z in bnew
         ]
 
         plt.axis("equal")
-
         for i_band, (contour, spinX, spinY, spinZ) in enumerate(zip(cont, sx, sy, sz)):
             # The previous interp. yields the level curves, nothing more is
             # useful from there
             paths = contour.collections[0].get_paths()
             if paths:
                 verts=[path.vertices for path in paths]
                 points = np.concatenate(verts)
 
 
                 self.log.debug("Fermi surf. points.shape: " + str(points.shape))
-
                 newSx = griddata((x, y), spinX, (points[:, 0], points[:, 1]))
                 newSy = griddata((x, y), spinY, (points[:, 0], points[:, 1]))
                 newSz = griddata((x, y), spinZ, (points[:, 0], points[:, 1]))
-
                 self.log.info("newSx.shape: " + str(newSx.shape))
                 if self.plot_opt['arrow_size']['value'] is not None:
                     scale  = self.plot_opt['arrow_size']['value']
                     scale_units = "xy"
                     angles="xy"
                 else:
                     scale=None
                     scale_units = "xy"
                     angles="xy"
 
+                if self.plot_opt['spin_projection']['value'] == 'z':
+                    color = newSz[::self.plot_opt['arrow_density']['value']]
+                elif self.plot_opt['spin_projection']['value'] == 'y':
+                    color = newSy[::self.plot_opt['arrow_density']['value']]
+                elif self.plot_opt['spin_projection']['value'] == 'x':
+                    color = newSx[::self.plot_opt['arrow_density']['value']]
+                elif self.plot_opt['spin_projection']['value'] == 'x^2':
+                    color = newSx[::self.plot_opt['arrow_density']['value']]**2
+                elif self.plot_opt['spin_projection']['value'] == 'y^2':
+                    color = newSy[::self.plot_opt['arrow_density']['value']]**2
+                elif self.plot_opt['spin_projection']['value'] == 'z^2':
+                    color = newSz[::self.plot_opt['arrow_density']['value']]**2
+
                 if self.plot_opt['no_arrow']['value']:
                     # a dictionary to select the right spin component
-                    spinDict = {0: newSx[::self.plot_opt['arrow_density']['value']], 
-                                1: newSy[::self.plot_opt['arrow_density']['value']], 
-                                2: newSz[::self.plot_opt['arrow_density']['value']]}
+                    # spinDict = {0: newSx[::self.plot_opt['arrow_density']['value']], 
+                    #             1: newSy[::self.plot_opt['arrow_density']['value']], 
+                    #             2: newSz[::self.plot_opt['arrow_density']['value']]}
+                        
                     plt.scatter(
                         points[::self.plot_opt['arrow_density']['value'], 0],
                         points[::self.plot_opt['arrow_density']['value'], 1],
-                        c=spinDict[spin],
+                        c=color,
+                        # spinDict[spin],
                         s=50,
                         edgecolor="none",
                         alpha=1.0,
                         marker=self.plot_opt['marker']['value'],
                         cmap=self.plot_opt['cmap']['value'],
-                        norm=colors.Normalize(-0.5, 0.5),
+                        norm=norm,
                     )
 
                 else:
                     if self.plot_opt['arrow_color']['value'] is not None or self.band_colors is not None:
                         if self.band_colors is not None:
                             c = self.band_colors[0][i_band]
                         if self.plot_opt['arrow_color']['value'] is not None:
                             c = self.plot_opt['arrow_color']['value']
-                            print('reee')
                         plt.quiver(
                             points[::self.plot_opt['arrow_density']['value'], 0],  # Arrow position x-component
                             points[::self.plot_opt['arrow_density']['value'], 1],  # Arrow position y-component
                             newSx[::self.plot_opt['arrow_density']['value']],      # Arrow direction x-component
                             newSy[::self.plot_opt['arrow_density']['value']],      # Arrow direction y-component
                             scale=scale,
                             scale_units=scale_units,
                             angles=angles,
                             color=c
                         )
                     else:
-                        if self.plot_opt['arrow_projection']['value'] == 'z':
-                            color = newSz[::self.plot_opt['arrow_density']['value']]
-                        elif self.plot_opt['arrow_projection']['value'] == 'y':
-                            color = newSy[::self.plot_opt['arrow_density']['value']]
-                        elif self.plot_opt['arrow_projection']['value'] == 'x':
-                            color = newSx[::self.plot_opt['arrow_density']['value']]
-                        elif self.plot_opt['arrow_projection']['value'] == 'x^2':
-                            color = newSx[::self.plot_opt['arrow_density']['value']]**2
-                        elif self.plot_opt['arrow_projection']['value'] == 'y^2':
-                            color = newSy[::self.plot_opt['arrow_density']['value']]**2
-                        elif self.plot_opt['arrow_projection']['value'] == 'z^2':
-                            color = newSz[::self.plot_opt['arrow_density']['value']]**2
-
-                        
+ 
                         plt.quiver(
                             points[::self.plot_opt['arrow_density']['value'], 0],  # Arrow position x-component
                             points[::self.plot_opt['arrow_density']['value'], 1],  # Arrow position y-component
                             newSx[::self.plot_opt['arrow_density']['value']],      # Arrow direction x-component
                             newSy[::self.plot_opt['arrow_density']['value']],      # Arrow direction y-component
                             color,                           # Color for each arrow
                             scale=scale,
                             scale_units=scale_units,
                             angles=angles,
                             cmap=self.plot_opt['cmap']['value'],
-                            norm=colors.Normalize(-0.5, 0.5),
+                            norm=norm,
                         )
                 
             
         if self.plot_opt['plot_color_bar']['value']:
             cbar = plt.colorbar()
-            if len(self.plot_opt['arrow_projection']['value'].split('^')) == 2:
-                tmp = self.plot_opt['arrow_projection']['value'].split('^')
+            if len(self.plot_opt['spin_projection']['value'].split('^')) == 2:
+                tmp = self.plot_opt['spin_projection']['value'].split('^')
                 label = f'S$_{tmp[0]}^{tmp[1]}$ projection'
             else:
-                tmp = self.plot_opt['arrow_projection']['value'].split('^')
+                tmp = self.plot_opt['spin_projection']['value'].split('^')
                 label = f'S$_{tmp[0]}$ projection'
             cbar.ax.set_ylabel(label, rotation=270)
         plt.axis("equal")
         font = {"size": 16}
         plt.rc("font", **font)
 
         self.log.debug("st: ...Done")
```

### Comparing `PyProcar-6.1.1/pyprocar/core/fermisurface3D.py` & `PyProcar-6.1.2/pyprocar/core/fermisurface3D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/isosurface.py` & `PyProcar-6.1.2/pyprocar/core/isosurface.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/kpath.py` & `PyProcar-6.1.2/pyprocar/core/kpath.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/procarselect.py` & `PyProcar-6.1.2/pyprocar/core/procarselect.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/procarsymmetry.py` & `PyProcar-6.1.2/pyprocar/core/procarsymmetry.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/procarunfold/_bak.procarparser.py` & `PyProcar-6.1.2/pyprocar/core/procarunfold/_bak.procarparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/procarunfold/fatband.py` & `PyProcar-6.1.2/pyprocar/core/procarunfold/fatband.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/procarunfold/procar_unfolder.py` & `PyProcar-6.1.2/pyprocar/core/procarunfold/procar_unfolder.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/procarunfold/unfolder.py` & `PyProcar-6.1.2/pyprocar/core/procarunfold/unfolder.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/structure.py` & `PyProcar-6.1.2/pyprocar/core/structure.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/core/surface.py` & `PyProcar-6.1.2/pyprocar/core/surface.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/__init__.py` & `PyProcar-6.1.2/pyprocar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/abinit.py` & `PyProcar-6.1.2/pyprocar/io/abinit.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/abinitparser/abinitparser.py` & `PyProcar-6.1.2/pyprocar/io/abinitparser/abinitparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/bxsf.py` & `PyProcar-6.1.2/pyprocar/io/bxsf.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/elk.py` & `PyProcar-6.1.2/pyprocar/io/elk.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/elkparser/elkparser.py` & `PyProcar-6.1.2/pyprocar/io/elkparser/elkparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/frmsf.py` & `PyProcar-6.1.2/pyprocar/io/frmsf.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/lobster.py` & `PyProcar-6.1.2/pyprocar/io/lobster.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/lobsterparser/lobster_doscar_parser.py` & `PyProcar-6.1.2/pyprocar/io/lobsterparser/lobster_doscar_parser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/lobsterparser/lobsterfermiparser.py` & `PyProcar-6.1.2/pyprocar/io/lobsterparser/lobsterfermiparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/lobsterparser/lobsterparser.py` & `PyProcar-6.1.2/pyprocar/io/lobsterparser/lobsterparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/parser.py` & `PyProcar-6.1.2/pyprocar/io/parser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/procarparser/procarparser.py` & `PyProcar-6.1.2/pyprocar/io/procarparser/procarparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/qe.py` & `PyProcar-6.1.2/pyprocar/io/qe.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/siesta.py` & `PyProcar-6.1.2/pyprocar/io/siesta.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/vasp.py` & `PyProcar-6.1.2/pyprocar/io/vasp.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/io/vaspxml/vaspxml.py` & `PyProcar-6.1.2/pyprocar/io/vaspxml/vaspxml.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/plotter/bs_2d_plot.py` & `PyProcar-6.1.2/pyprocar/plotter/bs_2d_plot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/plotter/dos_plot.py` & `PyProcar-6.1.2/pyprocar/plotter/dos_plot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/plotter/ebs_plot.py` & `PyProcar-6.1.2/pyprocar/plotter/ebs_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
                     ax:mpl.axes.Axes=None, 
                     spins:List[int]=None, 
                     **kwargs):
 
         with open(os.path.join(ROOT,'pyprocar','cfg','band_structure.yml'), 'r') as file:
             self.plot_opt = yaml.safe_load(file)
         self.update_config(kwargs)
-
         self.ebs = ebs
         self.kpath = kpath
         self.spins = spins
         if self.spins is None:
             self.spins = range(self.ebs.nspins)
         self.nspins = len(self.spins)
         if self.ebs.is_non_collinear:
@@ -523,55 +522,54 @@
         """A method to set the title
 
         Parameters
         ----------
         title : str, optional
             String for the title, by default "Band Structure"
         """
-        self.ax.set_title(label=title)
+        if self.plot_opt['title']['value']:
+            self.ax.set_title(label=self.plot_opt['title']['value'])
 
     def legend(self, labels:List[str]=None):
         """A methdo to plot the legend
 
         Parameters
         ----------
         labels : List[str], optional
             A list of strings for the labels of each element for the legend, by default None
         """
         if labels == None:
             labels = self.plot_opt['label']['value']
-        self.ax.legend(self.handles, labels)
 
-    def draw_fermi(self, 
-                fermi_level:float=0, 
-                color:str="blue", 
-                linestyle:str="dotted", 
-                linewidth:float=1):
+        if self.plot_opt['legend']['value']:
+            self.ax.legend(self.handles, labels)
+
+    def draw_fermi(self, fermi_level:float=0, ):
         """A method to draw the fermi line
 
         Parameters
         ----------
-        color : str, optional
-            The color of the fermi line, by default "blue"
-        linestyle : str, optional
-            The linestyle, by default "dotted"
-        linewidth : float, optional
-            The linewidth, by default 1
+        fermi_level : str, optional
+            The energy level to draw the line
         """
-        self.ax.axhline(y=fermi_level, color=color, linestyle=linestyle, linewidth=linewidth)
+        self.ax.axhline(y=fermi_level, 
+                        color=self.plot_opt['fermi_color']['value'], 
+                        linestyle=self.plot_opt['fermi_linestyle']['value'], 
+                        linewidth=self.plot_opt['fermi_linewidth']['value'])
 
     def grid(self):
         """A method to plot a grid
         """
-        self.ax.grid(
-            self.plot_opt['grid']['value'],
-            which=self.plot_opt['grid_which']['value'],
-            color=self.plot_opt['grid_color']['value'],
-            linestyle=self.plot_opt['grid_linestlye']['value'],
-            linewidth=self.plot_opt['grid_linewidth']['value'])
+        if self.plot_opt['grid']['value']:
+            self.ax.grid(
+                self.plot_opt['grid']['value'],
+                which=self.plot_opt['grid_which']['value'],
+                color=self.plot_opt['grid_color']['value'],
+                linestyle=self.plot_opt['grid_linestlye']['value'],
+                linewidth=self.plot_opt['grid_linewidth']['value'])
     
     def show(self):
         """A method to show the plot
         """
         plt.show()
 
     def save(self, filename:str='bands.pdf'):
```

### Comparing `PyProcar-6.1.1/pyprocar/plotter/fermi3d_plot.py` & `PyProcar-6.1.2/pyprocar/plotter/fermi3d_plot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/plotter/procarplot.py` & `PyProcar-6.1.2/pyprocar/plotter/procarplot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/analize.py` & `PyProcar-6.1.2/pyprocar/pyposcar/analize.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/chg_raw.py` & `PyProcar-6.1.2/pyprocar/pyposcar/chg_raw.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/clusters.py` & `PyProcar-6.1.2/pyprocar/pyposcar/clusters.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/db.py` & `PyProcar-6.1.2/pyprocar/pyposcar/db.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/dbCovalentBond.py` & `PyProcar-6.1.2/pyprocar/pyposcar/dbCovalentBond.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/defects.py` & `PyProcar-6.1.2/pyprocar/pyposcar/defects.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/generalUtils.py` & `PyProcar-6.1.2/pyprocar/pyposcar/generalUtils.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/honeycomb.py` & `PyProcar-6.1.2/pyprocar/pyposcar/honeycomb.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/latticeUtils.py` & `PyProcar-6.1.2/pyprocar/pyposcar/latticeUtils.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/outcarParser.py` & `PyProcar-6.1.2/pyprocar/pyposcar/outcarParser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/plot3d.py` & `PyProcar-6.1.2/pyprocar/pyposcar/plot3d.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/plotbands.py` & `PyProcar-6.1.2/pyprocar/pyposcar/plotbands.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/poscar.py` & `PyProcar-6.1.2/pyprocar/pyposcar/poscar.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/poscarUtils.py` & `PyProcar-6.1.2/pyprocar/pyposcar/poscarUtils.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/rdf.py` & `PyProcar-6.1.2/pyprocar/pyposcar/rdf.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/pyposcar/relax-cell-2d.py` & `PyProcar-6.1.2/pyprocar/pyposcar/relax-cell-2d.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/__init__.py` & `PyProcar-6.1.2/pyprocar/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/depreciated_scriptVector.py` & `PyProcar-6.1.2/pyprocar/scripts/depreciated_scriptVector.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptBandGap.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptBandGap.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptBandStructure2DHandler.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptBandStructure2DHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # from pyprocar.fermisurface3d import fermisurface3D
 from pyprocar.plotter import BandStructure2DataHandler, BandStructure2DVisualizer
 from pyprocar.utils import ROOT
 from .. import io
 
 
 np.set_printoptions(threshold=sys.maxsize)
-
+# 
 class BandStructure2DHandler:
 
     def __init__(self, 
             code:str,
             dirname:str="",
             repair:bool=False,
             apply_symmetry:bool=True,):
```

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptBandsDosplot.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptBandsDosplot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptBandsplot.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptBandsplot.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     ebs.bands -= ebs.efermi
     if fermi:
         ebs.bands += fermi
         fermi_level = fermi
     else:
         fermi_level = 0
 
-    ebs_plot = EBSPlot(ebs, kpath, ax, spins)
+    ebs_plot = EBSPlot(ebs, kpath, ax, spins ,**kwargs)
 
  
     labels = []
     if mode == "plain":
         ebs_plot.plot_bands()
 
     elif mode in ["overlay", "overlay_species", "overlay_orbitals"]:
@@ -220,27 +220,20 @@
         else:
             print("Selected mode %s not valid. Please check the spelling " % mode)
             
     ebs_plot.set_xticks(kticks, knames)
     ebs_plot.set_yticks(interval=elimit)
     ebs_plot.set_xlim()
     ebs_plot.set_ylim(elimit)
-    ebs_plot.draw_fermi(
-        fermi_level=fermi_level,
-        color=plot_opt['fermi_color']['value'],
-        linestyle=plot_opt['fermi_linestyle']['value'],
-        linewidth=plot_opt['fermi_linewidth']['value'],
-    )
+    ebs_plot.draw_fermi(fermi_level=fermi_level)
     ebs_plot.set_ylabel()
 
-    if plot_opt['title']['value']:
-        ebs_plot.set_title(title=plot_opt['title']['value'])
-    if plot_opt['grid']['value']:
-        ebs_plot.grid()
-    if plot_opt['legend']['value'] and len(labels) != 0:
-        ebs_plot.legend(labels)
+
+    ebs_plot.set_title()
+    ebs_plot.grid()
+    ebs_plot.legend(labels)
     if savefig is not None:
         ebs_plot.save(savefig)
     if show:
         ebs_plot.show()
         
     return ebs_plot
```

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptBandsplot_2d.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptBandsplot_2d.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptCat.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptCat.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptDosplot.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptDosplot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptFermi2D.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptFermi2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,14 @@
         ebsY.projected = ebsY.ebs_sum(spins=spins, atoms=atoms, orbitals=orbitals, sum_noncolinear=False)
         ebsZ.projected = ebsZ.ebs_sum(spins=spins, atoms=atoms, orbitals=orbitals, sum_noncolinear=False)
 
         ebsX.projected = ebsX.projected[:,:,[1]][:,:,0]
         ebsY.projected = ebsY.projected[:,:,[2]][:,:,0]
         ebsZ.projected = ebsZ.projected[:,:,[3]][:,:,0]
 
-
         stData.append(ebsX.projected )
         stData.append(ebsY.projected )
         stData.append(ebsZ.projected )
 
         
         projected = ebs.ebs_sum(spins=spins , atoms=atoms, orbitals=orbitals, sum_noncolinear=False)
     # Once the PROCAR is parsed and reduced to 2x2 arrays, we can apply
```

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptFermi3D.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptFermi3D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptFermiHandler.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptFermiHandler.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptFilter.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptFilter.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptKmesh2D.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptKmesh2D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptKpath.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptKpath.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptRepair.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptRepair.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptSpin_asymmetry.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptSpin_asymmetry.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptUnfold.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptUnfold.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_new.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptUnfold_new.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_old.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptUnfold_old.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_v2.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptUnfold_v2.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/scripts/scriptVector.py` & `PyProcar-6.1.2/pyprocar/scripts/scriptVector.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/__init__.py` & `PyProcar-6.1.2/pyprocar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/default_settings.ini` & `PyProcar-6.1.2/pyprocar/utils/default_settings.ini`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/defaults.py` & `PyProcar-6.1.2/pyprocar/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/download_examples.py` & `PyProcar-6.1.2/pyprocar/utils/download_examples.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/elements.py` & `PyProcar-6.1.2/pyprocar/utils/elements.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/info.py` & `PyProcar-6.1.2/pyprocar/utils/info.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/mathematics.py` & `PyProcar-6.1.2/pyprocar/utils/mathematics.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/procarfilefilter.py` & `PyProcar-6.1.2/pyprocar/utils/procarfilefilter.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/scriptFermi3D.py` & `PyProcar-6.1.2/pyprocar/utils/scriptFermi3D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/splash.py` & `PyProcar-6.1.2/pyprocar/utils/splash.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/unfolder.py` & `PyProcar-6.1.2/pyprocar/utils/unfolder.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/utils/utilsprocar.py` & `PyProcar-6.1.2/pyprocar/utils/utilsprocar.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/pyprocar/version.py` & `PyProcar-6.1.2/pyprocar/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # THIS FILE IS GENERATED FROM PYPROCAR SETUP.PY.
 name = 'PyProcar'
-version = '6.1.1'
+version = '6.1.2'
 description = 'A Python library for electronic structure pre/post-processing. '
 author = 'Francisco Muñoz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah'
 email = 'fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com'
 url = 'https://github.com/romerogroup/pyprocar'
-download_url = 'https://github.com/romerogroup/pyprocar/archive/6.1.1.tar.gz'
+download_url = 'https://github.com/romerogroup/pyprocar/archive/6.1.2.tar.gz'
 status = 'development'
 copyright = 'Copyright 2021'
 date = 'Jun 10th, 2021'
```

### Comparing `PyProcar-6.1.1/scripts/procar.py` & `PyProcar-6.1.2/scripts/procar.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.1/setup.json` & `PyProcar-6.1.2/setup.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'download_url'": "'https://github.com/romerogroup/pyprocar/archive/6.1.2.tar.gz'",*

 * * "'version'": "'6.1.2'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "author": "Francisco Mu\u00f1oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah",
     "copyright": "Copyright 2021",
     "date": "Jun 10th, 2021",
     "description": "A Python library for electronic structure pre/post-processing. ",
-    "download_url": "https://github.com/romerogroup/pyprocar/archive/6.1.1.tar.gz",
+    "download_url": "https://github.com/romerogroup/pyprocar/archive/6.1.2.tar.gz",
     "email": "fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com",
     "name": "PyProcar",
     "status": "development",
     "url": "https://github.com/romerogroup/pyprocar",
-    "version": "6.1.1"
+    "version": "6.1.2"
 }
```

### Comparing `PyProcar-6.1.1/setup.py` & `PyProcar-6.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,11 +49,11 @@
         'spglib',
         'trimesh',
         'ase',
         'sympy',
         'PyYAML',
     ],
     data_files=[("", ["LICENSE"])],
-    package_data={"": ["setup.json", '*.ini']},
+    package_data={"": ["setup.json", '*.ini','*.yml']},
     scripts=["scripts/procar.py"],
     packages=find_packages(exclude=["scripts"]),
 )
```

