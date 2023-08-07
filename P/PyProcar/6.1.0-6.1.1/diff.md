# Comparing `tmp/PyProcar-6.1.0.tar.gz` & `tmp/PyProcar-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProcar-6.1.0.tar", last modified: Mon Aug  7 06:55:51 2023, max compression
+gzip compressed data, was "PyProcar-6.1.1.tar", last modified: Mon Aug  7 07:56:13 2023, max compression
```

## Comparing `PyProcar-6.1.0.tar` & `PyProcar-6.1.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.730232 PyProcar-6.1.0/
--rw-rw-rw-   0        0        0     1655 2023-05-08 12:33:46.000000 PyProcar-6.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0    43233 2023-05-08 12:33:46.000000 PyProcar-6.1.0/LICENSE
--rw-rw-rw-   0        0        0       62 2023-05-08 12:33:46.000000 PyProcar-6.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      633 2023-08-07 06:55:51.731232 PyProcar-6.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.570087 PyProcar-6.1.0/PyProcar.egg-info/
--rw-rw-rw-   0        0        0      633 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3477 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-07 06:55:51.000000 PyProcar-6.1.0/PyProcar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9896 2023-08-07 06:48:50.000000 PyProcar-6.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.575090 PyProcar-6.1.0/pyprocar/
--rw-rw-rw-   0        0        0     2531 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.593107 PyProcar-6.1.0/pyprocar/core/
--rw-rw-rw-   0        0        0      520 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/__init__.py
--rw-rw-rw-   0        0        0    11350 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/bandstructure2D.py
--rw-rw-rw-   0        0        0     7424 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/brillouin_zone.py
--rw-rw-rw-   0        0        0    12198 2023-05-25 16:01:56.000000 PyProcar-6.1.0/pyprocar/core/dos.py
--rw-rw-rw-   0        0        0    46780 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/ebs.py
--rw-rw-rw-   0        0        0    19863 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/fermisurface.py
--rw-rw-rw-   0        0        0    14186 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/fermisurface3D.py
--rw-rw-rw-   0        0        0    14086 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/isosurface.py
--rw-rw-rw-   0        0        0    10122 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/kpath.py
--rw-rw-rw-   0        0        0     8578 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarselect.py
--rw-rw-rw-   0        0        0     8712 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarsymmetry.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.603115 PyProcar-6.1.0/pyprocar/core/procarunfold/
--rw-rw-rw-   0        0        0       45 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/__init__.py
--rw-rw-rw-   0        0        0    24502 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/_bak.procarparser.py
--rw-rw-rw-   0        0        0     5383 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/fatband.py
--rw-rw-rw-   0        0        0     4532 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/procar_unfolder.py
--rw-rw-rw-   0        0        0     5154 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/core/procarunfold/unfolder.py
--rw-rw-rw-   0        0        0    15028 2023-07-02 20:40:25.000000 PyProcar-6.1.0/pyprocar/core/structure.py
--rw-rw-rw-   0        0        0    11061 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/core/surface.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.619131 PyProcar-6.1.0/pyprocar/io/
--rw-rw-rw-   0        0        0      904 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/io/__init__.py
--rw-rw-rw-   0        0        0    21922 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/io/abinit.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.623134 PyProcar-6.1.0/pyprocar/io/abinitparser/
--rw-rw-rw-   0        0        0       41 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/abinitparser/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/abinitparser/abinitparser.py
--rw-rw-rw-   0        0        0     5879 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/bxsf.py
--rw-rw-rw-   0        0        0    14822 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/elk.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.626137 PyProcar-6.1.0/pyprocar/io/elkparser/
--rw-rw-rw-   0        0        0       34 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/elkparser/__init__.py
--rw-rw-rw-   0        0        0    11433 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/elkparser/elkparser.py
--rw-rw-rw-   0        0        0     3124 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/frmsf.py
--rw-rw-rw-   0        0        0    33353 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobster.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.632142 PyProcar-6.1.0/pyprocar/io/lobsterparser/
--rw-rw-rw-   0        0        0      145 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobsterparser/__init__.py
--rw-rw-rw-   0        0        0    21053 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobsterparser/lobster_doscar_parser.py
--rw-rw-rw-   0        0        0    15675 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobsterparser/lobsterfermiparser.py
--rw-rw-rw-   0        0        0    15388 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/lobsterparser/lobsterparser.py
--rw-rw-rw-   0        0        0     7146 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/io/parser.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.635145 PyProcar-6.1.0/pyprocar/io/procarparser/
--rw-rw-rw-   0        0        0       74 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/procarparser/__init__.py
--rw-rw-rw-   0        0        0    31346 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/procarparser/procarparser.py
--rw-rw-rw-   0        0        0    44082 2023-05-25 18:06:53.000000 PyProcar-6.1.0/pyprocar/io/qe.py
--rw-rw-rw-   0        0        0     9911 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/siesta.py
--rw-rw-rw-   0        0        0    81939 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/io/vasp.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.638147 PyProcar-6.1.0/pyprocar/io/vaspxml/
--rw-rw-rw-   0        0        0       55 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/vaspxml/__init__.py
--rw-rw-rw-   0        0        0    25252 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/io/vaspxml/vaspxml.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.648157 PyProcar-6.1.0/pyprocar/plotter/
--rw-rw-rw-   0        0        0      259 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/__init__.py
--rw-rw-rw-   0        0        0    24628 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/bs_2d_plot.py
--rw-rw-rw-   0        0        0    51396 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/dos_plot.py
--rw-rw-rw-   0        0        0    21705 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/ebs_plot.py
--rw-rw-rw-   0        0        0    45163 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/plotter/fermi3d_plot.py
--rw-rw-rw-   0        0        0    14084 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/plotter/procarplot.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.677184 PyProcar-6.1.0/pyprocar/pyposcar/
--rw-rw-rw-   0        0        0      177 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/__init__.py
--rw-rw-rw-   0        0        0     1425 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/analize.py
--rw-rw-rw-   0        0        0    19751 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/chg_raw.py
--rw-rw-rw-   0        0        0    11407 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/clusters.py
--rw-rw-rw-   0        0        0      961 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/db.py
--rw-rw-rw-   0        0        0     4077 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/dbCovalentBond.py
--rw-rw-rw-   0        0        0    14105 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/defects.py
--rw-rw-rw-   0        0        0      803 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/generalUtils.py
--rw-rw-rw-   0        0        0    11870 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/honeycomb.py
--rw-rw-rw-   0        0        0     6195 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/latticeUtils.py
--rw-rw-rw-   0        0        0     1885 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/outcarParser.py
--rw-rw-rw-   0        0        0     5191 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/plot3d.py
--rw-rw-rw-   0        0        0     5647 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/plotbands.py
--rw-rw-rw-   0        0        0    15418 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/poscar.py
--rw-rw-rw-   0        0        0    27247 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/poscarUtils.py
--rw-rw-rw-   0        0        0     7039 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/pyposcar/rdf.py
--rw-rw-rw-   0        0        0    12574 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/relax-cell-2d.py
--rw-rw-rw-   0        0        0      190 2023-07-01 06:22:02.000000 PyProcar-6.1.0/pyprocar/pyposcar/test.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.708212 PyProcar-6.1.0/pyprocar/scripts/
--rw-rw-rw-   0        0        0      808 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/depreciated_scriptVector.py
--rw-rw-rw-   0        0        0     1552 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandGap.py
--rw-rw-rw-   0        0        0     6603 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandStructure2DHandler.py
--rw-rw-rw-   0        0        0     8920 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandsDosplot.py
--rw-rw-rw-   0        0        0     8610 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandsplot.py
--rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptBandsplot_2d.py
--rw-rw-rw-   0        0        0    10120 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptCat.py
--rw-rw-rw-   0        0        0    13416 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptDosplot.py
--rw-rw-rw-   0        0        0     8872 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptFermi2D.py
--rw-rw-rw-   0        0        0    33281 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptFermi3D.py
--rw-rw-rw-   0        0        0    13173 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/scripts/scriptFermiHandler.py
--rw-rw-rw-   0        0        0     3238 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptFilter.py
--rw-rw-rw-   0        0        0     1333 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptKmesh2D.py
--rw-rw-rw-   0        0        0     3977 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptKpath.py
--rw-rw-rw-   0        0        0      526 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptRepair.py
--rw-rw-rw-   0        0        0     7841 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptSpin_asymmetry.py
--rw-rw-rw-   0        0        0    11385 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptUnfold.py
--rw-rw-rw-   0        0        0    25137 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_new.py
--rw-rw-rw-   0        0        0     2986 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_old.py
--rw-rw-rw-   0        0        0     6675 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_v2.py
--rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/scripts/scriptVector.py
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.727229 PyProcar-6.1.0/pyprocar/utils/
--rw-rw-rw-   0        0        0     1562 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/utils/__init__.py
--rw-rw-rw-   0        0        0     1739 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/utils/default_settings.ini
--rw-rw-rw-   0        0        0     3183 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/defaults.py
--rw-rw-rw-   0        0        0     5790 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/utils/download_examples.py
--rw-rw-rw-   0        0        0     4891 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/elements.py
--rw-rw-rw-   0        0        0     2403 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/info.py
--rw-rw-rw-   0        0        0     2994 2023-08-07 06:46:20.000000 PyProcar-6.1.0/pyprocar/utils/mathematics.py
--rw-rw-rw-   0        0        0    18332 2023-08-06 22:53:59.000000 PyProcar-6.1.0/pyprocar/utils/procarfilefilter.py
--rw-rw-rw-   0        0        0    28441 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/scriptFermi3D.py
--rw-rw-rw-   0        0        0      403 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/sorting.py
--rw-rw-rw-   0        0        0      975 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/splash.py
--rw-rw-rw-   0        0        0     6062 2023-08-06 21:34:44.000000 PyProcar-6.1.0/pyprocar/utils/unfolder.py
--rw-rw-rw-   0        0        0    10954 2023-05-08 12:33:47.000000 PyProcar-6.1.0/pyprocar/utils/utilsprocar.py
--rw-rw-rw-   0        0        0      688 2023-08-07 06:55:51.000000 PyProcar-6.1.0/pyprocar/version.py
--rw-rw-rw-   0        0        0      103 2023-08-07 06:46:20.000000 PyProcar-6.1.0/requirements.txt
--rw-rw-rw-   0        0        0      259 2023-08-07 06:55:41.000000 PyProcar-6.1.0/requirements_docs.txt
-drwxrwxrwx   0        0        0        0 2023-08-07 06:55:51.729230 PyProcar-6.1.0/scripts/
--rw-rw-rw-   0        0        0    33462 2023-05-08 12:33:47.000000 PyProcar-6.1.0/scripts/procar.py
--rw-rw-rw-   0        0        0       86 2023-08-07 06:55:51.733234 PyProcar-6.1.0/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-08-07 06:53:31.000000 PyProcar-6.1.0/setup.json
--rw-rw-rw-   0        0        0     1643 2023-08-07 06:46:20.000000 PyProcar-6.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.095854 PyProcar-6.1.1/
+-rw-rw-rw-   0        0        0     1655 2023-05-08 12:33:46.000000 PyProcar-6.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0    43233 2023-05-08 12:33:46.000000 PyProcar-6.1.1/LICENSE
+-rw-rw-rw-   0        0        0       62 2023-05-08 12:33:46.000000 PyProcar-6.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      633 2023-08-07 07:56:13.095854 PyProcar-6.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.925622 PyProcar-6.1.1/PyProcar.egg-info/
+-rw-rw-rw-   0        0        0      633 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3477 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 07:56:12.000000 PyProcar-6.1.1/PyProcar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9936 2023-08-07 07:54:40.000000 PyProcar-6.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.933630 PyProcar-6.1.1/pyprocar/
+-rw-rw-rw-   0        0        0     2531 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.952646 PyProcar-6.1.1/pyprocar/core/
+-rw-rw-rw-   0        0        0      520 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/__init__.py
+-rw-rw-rw-   0        0        0    11350 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/bandstructure2D.py
+-rw-rw-rw-   0        0        0     7424 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/brillouin_zone.py
+-rw-rw-rw-   0        0        0    12198 2023-05-25 16:01:56.000000 PyProcar-6.1.1/pyprocar/core/dos.py
+-rw-rw-rw-   0        0        0    46780 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/ebs.py
+-rw-rw-rw-   0        0        0    19863 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/fermisurface.py
+-rw-rw-rw-   0        0        0    14186 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/fermisurface3D.py
+-rw-rw-rw-   0        0        0    14086 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/isosurface.py
+-rw-rw-rw-   0        0        0    10122 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/kpath.py
+-rw-rw-rw-   0        0        0     8578 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarselect.py
+-rw-rw-rw-   0        0        0     8712 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarsymmetry.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.959653 PyProcar-6.1.1/pyprocar/core/procarunfold/
+-rw-rw-rw-   0        0        0       45 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/__init__.py
+-rw-rw-rw-   0        0        0    24502 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/_bak.procarparser.py
+-rw-rw-rw-   0        0        0     5383 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/fatband.py
+-rw-rw-rw-   0        0        0     4532 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/procar_unfolder.py
+-rw-rw-rw-   0        0        0     5154 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/core/procarunfold/unfolder.py
+-rw-rw-rw-   0        0        0    15028 2023-07-02 20:40:25.000000 PyProcar-6.1.1/pyprocar/core/structure.py
+-rw-rw-rw-   0        0        0    11061 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/core/surface.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.975113 PyProcar-6.1.1/pyprocar/io/
+-rw-rw-rw-   0        0        0      904 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/io/__init__.py
+-rw-rw-rw-   0        0        0    21922 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/io/abinit.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.978117 PyProcar-6.1.1/pyprocar/io/abinitparser/
+-rw-rw-rw-   0        0        0       41 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/abinitparser/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/abinitparser/abinitparser.py
+-rw-rw-rw-   0        0        0     5879 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/bxsf.py
+-rw-rw-rw-   0        0        0    14822 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/elk.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.980118 PyProcar-6.1.1/pyprocar/io/elkparser/
+-rw-rw-rw-   0        0        0       34 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/elkparser/__init__.py
+-rw-rw-rw-   0        0        0    11433 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/elkparser/elkparser.py
+-rw-rw-rw-   0        0        0     3124 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/frmsf.py
+-rw-rw-rw-   0        0        0    33353 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobster.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.989126 PyProcar-6.1.1/pyprocar/io/lobsterparser/
+-rw-rw-rw-   0        0        0      145 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobsterparser/__init__.py
+-rw-rw-rw-   0        0        0    21053 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobsterparser/lobster_doscar_parser.py
+-rw-rw-rw-   0        0        0    15675 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobsterparser/lobsterfermiparser.py
+-rw-rw-rw-   0        0        0    15388 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/lobsterparser/lobsterparser.py
+-rw-rw-rw-   0        0        0     7146 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/io/parser.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.993130 PyProcar-6.1.1/pyprocar/io/procarparser/
+-rw-rw-rw-   0        0        0       74 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/procarparser/__init__.py
+-rw-rw-rw-   0        0        0    31346 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/procarparser/procarparser.py
+-rw-rw-rw-   0        0        0    44082 2023-05-25 18:06:53.000000 PyProcar-6.1.1/pyprocar/io/qe.py
+-rw-rw-rw-   0        0        0     9911 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/siesta.py
+-rw-rw-rw-   0        0        0    81931 2023-08-07 07:29:04.000000 PyProcar-6.1.1/pyprocar/io/vasp.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:12.998134 PyProcar-6.1.1/pyprocar/io/vaspxml/
+-rw-rw-rw-   0        0        0       55 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/vaspxml/__init__.py
+-rw-rw-rw-   0        0        0    25252 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/io/vaspxml/vaspxml.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.008144 PyProcar-6.1.1/pyprocar/plotter/
+-rw-rw-rw-   0        0        0      259 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/__init__.py
+-rw-rw-rw-   0        0        0    24628 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/bs_2d_plot.py
+-rw-rw-rw-   0        0        0    51396 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/dos_plot.py
+-rw-rw-rw-   0        0        0    21705 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/ebs_plot.py
+-rw-rw-rw-   0        0        0    45163 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/plotter/fermi3d_plot.py
+-rw-rw-rw-   0        0        0    14084 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/plotter/procarplot.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.037170 PyProcar-6.1.1/pyprocar/pyposcar/
+-rw-rw-rw-   0        0        0      177 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/__init__.py
+-rw-rw-rw-   0        0        0     1425 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/analize.py
+-rw-rw-rw-   0        0        0    19751 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/chg_raw.py
+-rw-rw-rw-   0        0        0    11407 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/clusters.py
+-rw-rw-rw-   0        0        0      961 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/db.py
+-rw-rw-rw-   0        0        0     4077 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/dbCovalentBond.py
+-rw-rw-rw-   0        0        0    14105 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/defects.py
+-rw-rw-rw-   0        0        0      803 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/generalUtils.py
+-rw-rw-rw-   0        0        0    11870 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/honeycomb.py
+-rw-rw-rw-   0        0        0     6195 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/latticeUtils.py
+-rw-rw-rw-   0        0        0     1885 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/outcarParser.py
+-rw-rw-rw-   0        0        0     5191 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/plot3d.py
+-rw-rw-rw-   0        0        0     5647 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/plotbands.py
+-rw-rw-rw-   0        0        0    15418 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/poscar.py
+-rw-rw-rw-   0        0        0    27247 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/poscarUtils.py
+-rw-rw-rw-   0        0        0     7039 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/pyposcar/rdf.py
+-rw-rw-rw-   0        0        0    12574 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/relax-cell-2d.py
+-rw-rw-rw-   0        0        0      190 2023-07-01 06:22:02.000000 PyProcar-6.1.1/pyprocar/pyposcar/test.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.073834 PyProcar-6.1.1/pyprocar/scripts/
+-rw-rw-rw-   0        0        0      808 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/depreciated_scriptVector.py
+-rw-rw-rw-   0        0        0     1552 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandGap.py
+-rw-rw-rw-   0        0        0     6603 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandStructure2DHandler.py
+-rw-rw-rw-   0        0        0     8920 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandsDosplot.py
+-rw-rw-rw-   0        0        0     8610 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandsplot.py
+-rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptBandsplot_2d.py
+-rw-rw-rw-   0        0        0    10120 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptCat.py
+-rw-rw-rw-   0        0        0    13416 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptDosplot.py
+-rw-rw-rw-   0        0        0     8872 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptFermi2D.py
+-rw-rw-rw-   0        0        0    33281 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptFermi3D.py
+-rw-rw-rw-   0        0        0    13173 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/scripts/scriptFermiHandler.py
+-rw-rw-rw-   0        0        0     3238 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptFilter.py
+-rw-rw-rw-   0        0        0     1333 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptKmesh2D.py
+-rw-rw-rw-   0        0        0     3977 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptKpath.py
+-rw-rw-rw-   0        0        0      526 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptRepair.py
+-rw-rw-rw-   0        0        0     7841 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptSpin_asymmetry.py
+-rw-rw-rw-   0        0        0    11385 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptUnfold.py
+-rw-rw-rw-   0        0        0    25137 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_new.py
+-rw-rw-rw-   0        0        0     2986 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_old.py
+-rw-rw-rw-   0        0        0     6675 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_v2.py
+-rw-rw-rw-   0        0        0     3379 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/scripts/scriptVector.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.092851 PyProcar-6.1.1/pyprocar/utils/
+-rw-rw-rw-   0        0        0     1562 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1739 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/utils/default_settings.ini
+-rw-rw-rw-   0        0        0     3183 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/defaults.py
+-rw-rw-rw-   0        0        0     5790 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/utils/download_examples.py
+-rw-rw-rw-   0        0        0     4891 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/elements.py
+-rw-rw-rw-   0        0        0     2403 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/info.py
+-rw-rw-rw-   0        0        0     2994 2023-08-07 06:46:20.000000 PyProcar-6.1.1/pyprocar/utils/mathematics.py
+-rw-rw-rw-   0        0        0    18332 2023-08-06 22:53:59.000000 PyProcar-6.1.1/pyprocar/utils/procarfilefilter.py
+-rw-rw-rw-   0        0        0    28441 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/scriptFermi3D.py
+-rw-rw-rw-   0        0        0      403 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/sorting.py
+-rw-rw-rw-   0        0        0      975 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/splash.py
+-rw-rw-rw-   0        0        0     6062 2023-08-06 21:34:44.000000 PyProcar-6.1.1/pyprocar/utils/unfolder.py
+-rw-rw-rw-   0        0        0    10954 2023-05-08 12:33:47.000000 PyProcar-6.1.1/pyprocar/utils/utilsprocar.py
+-rw-rw-rw-   0        0        0      688 2023-08-07 07:56:12.000000 PyProcar-6.1.1/pyprocar/version.py
+-rw-rw-rw-   0        0        0      103 2023-08-07 06:46:20.000000 PyProcar-6.1.1/requirements.txt
+-rw-rw-rw-   0        0        0      259 2023-08-07 06:55:41.000000 PyProcar-6.1.1/requirements_docs.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 07:56:13.093852 PyProcar-6.1.1/scripts/
+-rw-rw-rw-   0        0        0    33462 2023-05-08 12:33:47.000000 PyProcar-6.1.1/scripts/procar.py
+-rw-rw-rw-   0        0        0       86 2023-08-07 07:56:13.102860 PyProcar-6.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-08-07 07:46:29.000000 PyProcar-6.1.1/setup.json
+-rw-rw-rw-   0        0        0     1643 2023-08-07 06:46:20.000000 PyProcar-6.1.1/setup.py
```

### Comparing `PyProcar-6.1.0/AUTHORS.rst` & `PyProcar-6.1.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/LICENSE` & `PyProcar-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/PKG-INFO` & `PyProcar-6.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: PyProcar
-Version: 6.1.0
+Version: 6.1.1
 Summary: A Python library for electronic structure pre/post-processing. 
 Home-page: https://github.com/romerogroup/pyprocar
 Author: Francisco MuÃ±oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
 Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
 License: LICENSE
-Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.0.tar.gz
+Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.1.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `PyProcar-6.1.0/PyProcar.egg-info/PKG-INFO` & `PyProcar-6.1.1/PyProcar.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: PyProcar
-Version: 6.1.0
+Version: 6.1.1
 Summary: A Python library for electronic structure pre/post-processing. 
 Home-page: https://github.com/romerogroup/pyprocar
 Author: Francisco MuÃ±oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah
 Author-email: fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com
 License: LICENSE
-Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.0.tar.gz
+Download-URL: https://github.com/romerogroup/pyprocar/archive/6.1.1.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `PyProcar-6.1.0/PyProcar.egg-info/SOURCES.txt` & `PyProcar-6.1.1/PyProcar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/README.md` & `PyProcar-6.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 5. Lobster (Stll in development)
 
 ![](welcome.png)
 
 Documentation
 -------------
 
-For versions 6.1.0 and above, the documentation is found here:
+For versions 6.1.1 and above, the documentation is found here:
 https://romerogroup.github.io/pyprocar/
 
 
 The prior documentation is found here:
 https://romerogroup.github.io/pyprocar5.6.6/
 
 
@@ -117,14 +117,15 @@
 
     procar.py -h
 
 will bring a help menu.
 
 Changelog
 --------------
+v6.1.1 Aug 7th, 2023 -- Bug fix <br />
 v6.1.0 Aug 7th, 2023 -- Bug fixes, doc update, config files <br />
 v6.0.0 Jun 10th, 2023 -- Major code base changes. <br />
 v5.6.6 Mar 6th, 2022 -- QE, bandsplot, dosplot, fermi surface, and band unfolding bug fixes. Directory change, parsers are now in the io directory. <br />
 v5.6.5 Jun 10th, 2021 -- Fermi surface object and fermi surface plotter bug fixes <br />
 v5.6.4 May 6th, 2021 -- Updates to Fermi surface plotter. <br />
 v5.6.3 Mar 5th, 2021 -- QE and elk bug fixes. <br />
 v5.6.2 Jan 11th, 2021 -- Updates and bugfixes to fermi surface and dos plotter. <br />
```

### Comparing `PyProcar-6.1.0/pyprocar/__init__.py` & `PyProcar-6.1.1/pyprocar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/__init__.py` & `PyProcar-6.1.1/pyprocar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/bandstructure2D.py` & `PyProcar-6.1.1/pyprocar/core/bandstructure2D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/brillouin_zone.py` & `PyProcar-6.1.1/pyprocar/core/brillouin_zone.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/dos.py` & `PyProcar-6.1.1/pyprocar/core/dos.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/ebs.py` & `PyProcar-6.1.1/pyprocar/core/ebs.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/fermisurface.py` & `PyProcar-6.1.1/pyprocar/core/fermisurface.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/fermisurface3D.py` & `PyProcar-6.1.1/pyprocar/core/fermisurface3D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/isosurface.py` & `PyProcar-6.1.1/pyprocar/core/isosurface.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/kpath.py` & `PyProcar-6.1.1/pyprocar/core/kpath.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/procarselect.py` & `PyProcar-6.1.1/pyprocar/core/procarselect.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/procarsymmetry.py` & `PyProcar-6.1.1/pyprocar/core/procarsymmetry.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/procarunfold/_bak.procarparser.py` & `PyProcar-6.1.1/pyprocar/core/procarunfold/_bak.procarparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/procarunfold/fatband.py` & `PyProcar-6.1.1/pyprocar/core/procarunfold/fatband.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/procarunfold/procar_unfolder.py` & `PyProcar-6.1.1/pyprocar/core/procarunfold/procar_unfolder.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/procarunfold/unfolder.py` & `PyProcar-6.1.1/pyprocar/core/procarunfold/unfolder.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/structure.py` & `PyProcar-6.1.1/pyprocar/core/structure.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/core/surface.py` & `PyProcar-6.1.1/pyprocar/core/surface.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/__init__.py` & `PyProcar-6.1.1/pyprocar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/abinit.py` & `PyProcar-6.1.1/pyprocar/io/abinit.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/abinitparser/abinitparser.py` & `PyProcar-6.1.1/pyprocar/io/abinitparser/abinitparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/bxsf.py` & `PyProcar-6.1.1/pyprocar/io/bxsf.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/elk.py` & `PyProcar-6.1.1/pyprocar/io/elk.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/elkparser/elkparser.py` & `PyProcar-6.1.1/pyprocar/io/elkparser/elkparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/frmsf.py` & `PyProcar-6.1.1/pyprocar/io/frmsf.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/lobster.py` & `PyProcar-6.1.1/pyprocar/io/lobster.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/lobsterparser/lobster_doscar_parser.py` & `PyProcar-6.1.1/pyprocar/io/lobsterparser/lobster_doscar_parser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/lobsterparser/lobsterfermiparser.py` & `PyProcar-6.1.1/pyprocar/io/lobsterparser/lobsterfermiparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/lobsterparser/lobsterparser.py` & `PyProcar-6.1.1/pyprocar/io/lobsterparser/lobsterparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/parser.py` & `PyProcar-6.1.1/pyprocar/io/parser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/procarparser/procarparser.py` & `PyProcar-6.1.1/pyprocar/io/procarparser/procarparser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/qe.py` & `PyProcar-6.1.1/pyprocar/io/qe.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/siesta.py` & `PyProcar-6.1.1/pyprocar/io/siesta.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/io/vasp.py` & `PyProcar-6.1.1/pyprocar/io/vasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         ----------
         filename : Union[str, Path], optional
             The OUTCAR filename. If not provided, defaults to "OUTCAR".
         """
         
         self.variables: dict = {}
         self.filename: Path = Path(filename)
-                self._get_axes_nk()
+        self._get_axes_nk()
 
         with open(self.filename, "r") as rf:
             self.file_str: str = rf.read()
     def _get_axes_nk(self):
         """
         n_kx
```

### Comparing `PyProcar-6.1.0/pyprocar/io/vaspxml/vaspxml.py` & `PyProcar-6.1.1/pyprocar/io/vaspxml/vaspxml.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/plotter/bs_2d_plot.py` & `PyProcar-6.1.1/pyprocar/plotter/bs_2d_plot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/plotter/dos_plot.py` & `PyProcar-6.1.1/pyprocar/plotter/dos_plot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/plotter/ebs_plot.py` & `PyProcar-6.1.1/pyprocar/plotter/ebs_plot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/plotter/fermi3d_plot.py` & `PyProcar-6.1.1/pyprocar/plotter/fermi3d_plot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/plotter/procarplot.py` & `PyProcar-6.1.1/pyprocar/plotter/procarplot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/analize.py` & `PyProcar-6.1.1/pyprocar/pyposcar/analize.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/chg_raw.py` & `PyProcar-6.1.1/pyprocar/pyposcar/chg_raw.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/clusters.py` & `PyProcar-6.1.1/pyprocar/pyposcar/clusters.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/db.py` & `PyProcar-6.1.1/pyprocar/pyposcar/db.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/dbCovalentBond.py` & `PyProcar-6.1.1/pyprocar/pyposcar/dbCovalentBond.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/defects.py` & `PyProcar-6.1.1/pyprocar/pyposcar/defects.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/generalUtils.py` & `PyProcar-6.1.1/pyprocar/pyposcar/generalUtils.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/honeycomb.py` & `PyProcar-6.1.1/pyprocar/pyposcar/honeycomb.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/latticeUtils.py` & `PyProcar-6.1.1/pyprocar/pyposcar/latticeUtils.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/outcarParser.py` & `PyProcar-6.1.1/pyprocar/pyposcar/outcarParser.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/plot3d.py` & `PyProcar-6.1.1/pyprocar/pyposcar/plot3d.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/plotbands.py` & `PyProcar-6.1.1/pyprocar/pyposcar/plotbands.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/poscar.py` & `PyProcar-6.1.1/pyprocar/pyposcar/poscar.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/poscarUtils.py` & `PyProcar-6.1.1/pyprocar/pyposcar/poscarUtils.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/rdf.py` & `PyProcar-6.1.1/pyprocar/pyposcar/rdf.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/pyposcar/relax-cell-2d.py` & `PyProcar-6.1.1/pyprocar/pyposcar/relax-cell-2d.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/__init__.py` & `PyProcar-6.1.1/pyprocar/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/depreciated_scriptVector.py` & `PyProcar-6.1.1/pyprocar/scripts/depreciated_scriptVector.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptBandGap.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptBandGap.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptBandStructure2DHandler.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptBandStructure2DHandler.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptBandsDosplot.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptBandsDosplot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptBandsplot.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptBandsplot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptBandsplot_2d.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptBandsplot_2d.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptCat.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptCat.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptDosplot.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptDosplot.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptFermi2D.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptFermi2D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptFermi3D.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptFermi3D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptFermiHandler.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptFermiHandler.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptFilter.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptFilter.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptKmesh2D.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptKmesh2D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptKpath.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptKpath.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptRepair.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptRepair.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptSpin_asymmetry.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptSpin_asymmetry.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptUnfold.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptUnfold.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_new.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_new.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_old.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_old.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptUnfold_v2.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptUnfold_v2.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/scripts/scriptVector.py` & `PyProcar-6.1.1/pyprocar/scripts/scriptVector.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/__init__.py` & `PyProcar-6.1.1/pyprocar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/default_settings.ini` & `PyProcar-6.1.1/pyprocar/utils/default_settings.ini`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/defaults.py` & `PyProcar-6.1.1/pyprocar/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/download_examples.py` & `PyProcar-6.1.1/pyprocar/utils/download_examples.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/elements.py` & `PyProcar-6.1.1/pyprocar/utils/elements.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/info.py` & `PyProcar-6.1.1/pyprocar/utils/info.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/mathematics.py` & `PyProcar-6.1.1/pyprocar/utils/mathematics.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/procarfilefilter.py` & `PyProcar-6.1.1/pyprocar/utils/procarfilefilter.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/scriptFermi3D.py` & `PyProcar-6.1.1/pyprocar/utils/scriptFermi3D.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/splash.py` & `PyProcar-6.1.1/pyprocar/utils/splash.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/unfolder.py` & `PyProcar-6.1.1/pyprocar/utils/unfolder.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/utils/utilsprocar.py` & `PyProcar-6.1.1/pyprocar/utils/utilsprocar.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/pyprocar/version.py` & `PyProcar-6.1.1/pyprocar/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # THIS FILE IS GENERATED FROM PYPROCAR SETUP.PY.
 name = 'PyProcar'
-version = '6.1.0'
+version = '6.1.1'
 description = 'A Python library for electronic structure pre/post-processing. '
 author = 'Francisco Muñoz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah'
 email = 'fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com'
 url = 'https://github.com/romerogroup/pyprocar'
-download_url = 'https://github.com/romerogroup/pyprocar/archive/6.1.0.tar.gz'
+download_url = 'https://github.com/romerogroup/pyprocar/archive/6.1.1.tar.gz'
 status = 'development'
 copyright = 'Copyright 2021'
 date = 'Jun 10th, 2021'
```

### Comparing `PyProcar-6.1.0/scripts/procar.py` & `PyProcar-6.1.1/scripts/procar.py`

 * *Files identical despite different names*

### Comparing `PyProcar-6.1.0/setup.json` & `PyProcar-6.1.1/setup.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'download_url'": "'https://github.com/romerogroup/pyprocar/archive/6.1.1.tar.gz'",*

 * * "'version'": "'6.1.1'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "author": "Francisco Mu\u00f1oz, Aldo Romero, Sobhit Singh, Uthpala Herath, Pedram Tavadze, Eric Bousquet, Xu He, Reese Boucher, Logan Lang, Freddy Farah",
     "copyright": "Copyright 2021",
     "date": "Jun 10th, 2021",
     "description": "A Python library for electronic structure pre/post-processing. ",
-    "download_url": "https://github.com/romerogroup/pyprocar/archive/6.1.0.tar.gz",
+    "download_url": "https://github.com/romerogroup/pyprocar/archive/6.1.1.tar.gz",
     "email": "fvmunoz@gmail.com, alromero@mail.wvu.edu, smsingh@mix.wvu.edu, ukh0001@mix.wvu.edu, petavazohi@mix.wvu.edu, eric.bousquet@uliege.be, mailhexu@gmail.com",
     "name": "PyProcar",
     "status": "development",
     "url": "https://github.com/romerogroup/pyprocar",
-    "version": "6.1.0"
+    "version": "6.1.1"
 }
```

### Comparing `PyProcar-6.1.0/setup.py` & `PyProcar-6.1.1/setup.py`

 * *Files identical despite different names*

