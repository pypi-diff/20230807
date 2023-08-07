# Comparing `tmp/xplorts-0.7.tar.gz` & `tmp/xplorts-0.8.tar.gz`

## Comparing `xplorts-0.7.tar` & `xplorts-0.8.tar`

### file list

```diff
@@ -1,76 +1,105 @@
--rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 xplorts-0.7/_NOTES.ipynb
--rw-r--r--   0        0        0  1246655 2020-02-02 00:00:00.000000 xplorts-0.7/tt.html
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 xplorts-0.7/data/.~lock.totalpspreferencetables2020.xlsx#
--rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 xplorts-0.7/data/oph annual bespoke.csv
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 xplorts-0.7/data/oph annual by division.csv
--rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 xplorts-0.7/data/oph annual by section.csv
--rw-r--r--   0        0        0    93088 2020-02-02 00:00:00.000000 xplorts-0.7/data/oph quarterly by section.csv
--rw-r--r--   0        0        0  2542592 2020-02-02 00:00:00.000000 xplorts-0.7/data/outputperhourworked.xls
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 xplorts-0.7/data/psp non-quality adjusted.csv
--rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 xplorts-0.7/data/psp quality adjusted.csv
--rw-r--r--   0        0        0    79893 2020-02-02 00:00:00.000000 xplorts-0.7/data/totalpspreferencetables2020.xlsx
--rw-r--r--   0        0        0  1285776 2020-02-02 00:00:00.000000 xplorts-0.7/docs/html/xplor_lprod oph annual by section.html
--rw-r--r--   0        0        0  1775672 2020-02-02 00:00:00.000000 xplorts-0.7/docs/html/xplor_lprod oph quarterly by section.html
--rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/slideselect_date.png
--rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/slideselect_industry.png
--rw-r--r--   0        0        0    46598 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/xplor_lprod_lines_thumbnail_large.png
--rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/xplor_lprod_snapcomp_thumbnail_large.png
--rw-r--r--   0        0        0    20261 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/xplor_lprod_thumbnail.png
--rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/xplor_lprod_tscomp_thumbnail_large.png
--rw-r--r--   0        0        0   947883 2020-02-02 00:00:00.000000 xplorts-0.7/src/tt.html
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 xplorts-0.7/src/tt.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/__init__.py
--rw-r--r--   0        0        0    32735 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/base.ipynb
--rw-r--r--   0        0        0    16670 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/base.py
--rw-r--r--   0        0        0    11905 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dutils.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/ghostbokeh.py
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/slideselect.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/__main__.py
--rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/dblprod.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/prodgrowsnap.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/prodgrowts.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/prodlines.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/xpdblprod.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/heatmap/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/heatmap/__main__.py
--rw-r--r--   0        0        0    11819 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/heatmap/heatmap.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/heatmap/xpheatmap.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/lines/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/lines/__main__.py
--rw-r--r--   0        0        0    13921 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/lines/lines.py
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/lines/xplines.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/scatter/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/scatter/__main__.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/scatter/scatter.py
--rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/scatter/xpscatter.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/snapcomp/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/snapcomp/__main__.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/snapcomp/snapcomp.py
--rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/snapcomp/xpsnapcomp.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/__main__.py
--rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/bokeh_stacks.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/stacks.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/stacks_util.py
--rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/xpstacks.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/tscomp/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/tscomp/__main__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/tscomp/tscomp.py
--rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/tscomp/xptscomp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/utils/__init__.py
--rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/utils/ukons_lprod_to_csv.py
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/utils/ukons_psp_to_csv.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 xplorts-0.7/tests/conftest.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_dblprod.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_heatmap.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_lines.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_scatter.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_snapcomp.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_stacks.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_tscomp.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xplorts-0.7/.gitignore
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 xplorts-0.7/LICENSE
--rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 xplorts-0.7/README.md
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 xplorts-0.7/pyproject.toml
--rw-r--r--   0        0        0    16364 2020-02-02 00:00:00.000000 xplorts-0.7/PKG-INFO
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 xplorts-0.8/_NOTES.ipynb
+-rw-r--r--   0        0        0  1246655 2020-02-02 00:00:00.000000 xplorts-0.8/tt.html
+-rw-r--r--   0        0        0    32786 2020-02-02 00:00:00.000000 xplorts-0.8/data/labourcostslabourshare.csv
+-rw-r--r--   0        0        0   274646 2020-02-02 00:00:00.000000 xplorts-0.8/data/labourcostslabourshare.xlsx
+-rw-r--r--   0        0        0    32786 2020-02-02 00:00:00.000000 xplorts-0.8/data/lcli index.csv
+-rw-r--r--   0        0        0    31803 2020-02-02 00:00:00.000000 xplorts-0.8/data/lcli level.csv
+-rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 xplorts-0.8/data/oph annual bespoke.csv
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 xplorts-0.8/data/oph annual by division.csv
+-rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 xplorts-0.8/data/oph annual by section.csv
+-rw-r--r--   0        0        0    93088 2020-02-02 00:00:00.000000 xplorts-0.8/data/oph quarterly by section.csv
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 xplorts-0.8/data/outputperhourworked.csv
+-rw-r--r--   0        0        0  2542592 2020-02-02 00:00:00.000000 xplorts-0.8/data/outputperhourworked.xls
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 xplorts-0.8/data/psp non-quality adjusted.csv
+-rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 xplorts-0.8/data/psp quality adjusted.csv
+-rw-r--r--   0        0        0    79893 2020-02-02 00:00:00.000000 xplorts-0.8/data/totalpspreferencetables2020.xlsx
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/.~lock.outputperhourworked.xls#
+-rw-r--r--   0        0        0    31803 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/labourcostslabourshare.csv
+-rw-r--r--   0        0        0   274646 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/labourcostslabourshare.xlsx
+-rw-r--r--   0        0        0    32786 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/lcli index.csv
+-rw-r--r--   0        0        0  1662154 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/lcli index.html
+-rw-r--r--   0        0        0    31803 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/lcli level.csv
+-rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/oph annual bespoke.csv
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/oph annual by division.csv
+-rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/oph annual by section.csv
+-rw-r--r--   0        0        0  1344529 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/oph annual by section.html
+-rw-r--r--   0        0        0    93088 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/oph quarterly by section.csv
+-rw-r--r--   0        0        0  1408591 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/oph quarterly by section.html
+-rw-r--r--   0        0        0   360454 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/outputperhourworked.csv
+-rw-r--r--   0        0        0  2542592 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/outputperhourworked.xls
+-rw-r--r--   0        0        0    95059 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/outputperjob.csv
+-rw-r--r--   0        0        0  1126619 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/outputperjob.xlsx
+-rw-r--r--   0        0        0    13442 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/outputperworker.csv
+-rw-r--r--   0        0        0   124931 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/outputperworker.xlsx
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/psp non-quality adjusted.csv
+-rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/psp quality adjusted.csv
+-rw-r--r--   0        0        0  1271967 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/psp quality adjusted.html
+-rw-r--r--   0        0        0     8786 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/totalpspreferencetables2020.csv
+-rw-r--r--   0        0        0    79893 2020-02-02 00:00:00.000000 xplorts-0.8/data (local)/totalpspreferencetables2020.xlsx
+-rw-r--r--   0        0        0  1285776 2020-02-02 00:00:00.000000 xplorts-0.8/docs/html/xplor_lprod oph annual by section.html
+-rw-r--r--   0        0        0  1775672 2020-02-02 00:00:00.000000 xplorts-0.8/docs/html/xplor_lprod oph quarterly by section.html
+-rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 xplorts-0.8/docs/png/slideselect_date.png
+-rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 xplorts-0.8/docs/png/slideselect_industry.png
+-rw-r--r--   0        0        0    46598 2020-02-02 00:00:00.000000 xplorts-0.8/docs/png/xplor_lprod_lines_thumbnail_large.png
+-rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 xplorts-0.8/docs/png/xplor_lprod_snapcomp_thumbnail_large.png
+-rw-r--r--   0        0        0    20261 2020-02-02 00:00:00.000000 xplorts-0.8/docs/png/xplor_lprod_thumbnail.png
+-rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 xplorts-0.8/docs/png/xplor_lprod_tscomp_thumbnail_large.png
+-rw-r--r--   0        0        0   947883 2020-02-02 00:00:00.000000 xplorts-0.8/src/tt.html
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 xplorts-0.8/src/tt.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/__init__.py
+-rw-r--r--   0        0        0    32735 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/base.ipynb
+-rw-r--r--   0        0        0    16670 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/base.py
+-rw-r--r--   0        0        0    10312 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/dutils.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/ghostbokeh.py
+-rw-r--r--   0        0        0    13258 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/growthcomps.py
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/slideselect.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/dashboard/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/dashboard/__main__.py
+-rw-r--r--   0        0        0    13496 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/dashboard/xpdashboard.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/dblprod/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/dblprod/__main__.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/dblprod/xpdblprod.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/heatmap/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/heatmap/__main__.py
+-rw-r--r--   0        0        0    11819 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/heatmap/heatmap.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/heatmap/xpheatmap.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/lines/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/lines/__main__.py
+-rw-r--r--   0        0        0    14013 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/lines/lines.py
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/lines/xplines.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/scatter/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/scatter/__main__.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/scatter/scatter.py
+-rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/scatter/xpscatter.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/snapcomp/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/snapcomp/__main__.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/snapcomp/snapcomp.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/snapcomp/xpsnapcomp.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/stacks/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/stacks/__main__.py
+-rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/stacks/bokeh_stacks.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/stacks/stacks.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/stacks/stacks_util.py
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/stacks/xpstacks.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/tscomp/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/tscomp/__main__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/tscomp/tscomp.py
+-rw-r--r--   0        0        0     8830 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/tscomp/xptscomp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/utils/__init__.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/utils/ukons_lcli_to_csv.py
+-rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/utils/ukons_lprod_to_csv.py
+-rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 xplorts-0.8/src/xplorts/utils/ukons_psp_to_csv.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 xplorts-0.8/tests/conftest.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 xplorts-0.8/tests/test_dashboard.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 xplorts-0.8/tests/test_dblprod.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 xplorts-0.8/tests/test_heatmap.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 xplorts-0.8/tests/test_lines.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 xplorts-0.8/tests/test_scatter.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 xplorts-0.8/tests/test_snapcomp.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 xplorts-0.8/tests/test_stacks.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 xplorts-0.8/tests/test_tscomp.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xplorts-0.8/.gitignore
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 xplorts-0.8/LICENSE
+-rw-r--r--   0        0        0    10589 2020-02-02 00:00:00.000000 xplorts-0.8/README.md
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 xplorts-0.8/pyproject.toml
+-rw-r--r--   0        0        0    17112 2020-02-02 00:00:00.000000 xplorts-0.8/PKG-INFO
```

### Comparing `xplorts-0.7/_NOTES.ipynb` & `xplorts-0.8/_NOTES.ipynb`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/tt.html` & `xplorts-0.8/tt.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/data/oph annual bespoke.csv` & `xplorts-0.8/data/oph annual bespoke.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/data/oph annual by division.csv` & `xplorts-0.8/data/oph annual by division.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/data/oph annual by section.csv` & `xplorts-0.8/data/oph annual by section.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/data/oph quarterly by section.csv` & `xplorts-0.8/data/oph quarterly by section.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/data/outputperhourworked.xls` & `xplorts-0.8/data/outputperhourworked.xls`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/data/psp non-quality adjusted.csv` & `xplorts-0.8/data/psp non-quality adjusted.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/data/psp quality adjusted.csv` & `xplorts-0.8/data/psp quality adjusted.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/data/totalpspreferencetables2020.xlsx` & `xplorts-0.8/data/totalpspreferencetables2020.xlsx`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/docs/html/xplor_lprod oph annual by section.html` & `xplorts-0.8/docs/html/xplor_lprod oph annual by section.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/docs/html/xplor_lprod oph quarterly by section.html` & `xplorts-0.8/docs/html/xplor_lprod oph quarterly by section.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/docs/png/slideselect_date.png` & `xplorts-0.8/docs/png/slideselect_date.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/docs/png/slideselect_industry.png` & `xplorts-0.8/docs/png/slideselect_industry.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/docs/png/xplor_lprod_lines_thumbnail_large.png` & `xplorts-0.8/docs/png/xplor_lprod_lines_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/docs/png/xplor_lprod_snapcomp_thumbnail_large.png` & `xplorts-0.8/docs/png/xplor_lprod_snapcomp_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/docs/png/xplor_lprod_thumbnail.png` & `xplorts-0.8/docs/png/xplor_lprod_thumbnail.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/docs/png/xplor_lprod_tscomp_thumbnail_large.png` & `xplorts-0.8/docs/png/xplor_lprod_tscomp_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/tt.html` & `xplorts-0.8/src/tt.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/tt.py` & `xplorts-0.8/src/tt.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/__init__.py` & `xplorts-0.8/src/xplorts/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
 
 Modules (exported by the package)
 ---------------------------------
 base
     Miscellaneous helper functions and classes.
 
+dutils
+    Miscellaneous data manipulation helpers.
+
 ghostbokeh
     Define an abstract base class to a build pseudo-subclass of a Bokeh class.
 
 heatmap
     Functions to create a heatmap showing data values as a function of
     horizontal and vertical categorical variables.
```

### Comparing `xplorts-0.7/src/xplorts/base.ipynb` & `xplorts-0.8/src/xplorts/base.ipynb`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/base.py` & `xplorts-0.8/src/xplorts/base.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/dutils.py` & `xplorts-0.8/src/xplorts/heatmap/heatmap.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,361 +1,399 @@
 """
-dutils
----------
-Miscellaneous data manipulation helpers
+Make standalone interactive heatmaps for categorical time series data
 
 Functions
 ---------
-accumulate_list
-    Initial subsequences of increasing length from list of items.
-
-cumulative_growth
-    Percentage growth of dataframe columns relative to earliest date.
-
-date_tuples
-    Coerce monthly, quarterly, or annual dates to tuples.
-
-dict_fill
-    Map keys to values, recycling values as necessary.
+figheatmap
+    Make a heatmap figure, with color bar
 
-growth_pct_from
-    Percentage growth for a series relative to a baseline value.
+heatmap
+    Add a heatmap to a figure, with color map and hover tooltip.
 
-growth_vars
-    Calculate growth for columns in a dataframe.
+jscb_set_from_selection
+    Set object's .value dynamically in the browser from a source selection
 
-index_to
-    Scale data by constant so a baseline value maps to a target value.
+ts_categorical_figure
+    Make empty bokeh Figure with time series x and categorical y axis
 
-pairwise
-    Stand-in for future `itertools.pairwise()` if `itertools` is old.
 """
+# See https://docs.bokeh.org/en/latest/docs/user_guide/topics/categorical.html#heatmaps
 
-#%%
 
-from itertools import cycle, tee
+#%%
 
-import numpy as np
+from math import pi
 import pandas as pd
-import re
-
-try:
-    from itertools import pairwise
-except ImportError:
-    # Define local pairwise(), since itertools is too old to have it.
-    #
-    # Function is derived from
-    #   https://docs.python.org/3/library/itertools.html#itertools.pairwise
-    # "Copyright © 2001-2023 Python Software Foundation; All Rights Reserved"
-    # Used here under the ZERO-CLAUSE BSD LICENSE FOR CODE IN THE PYTHON 3.11.3 DOCUMENTATION
-    #   https://docs.python.org/3/license.html#bsd0
-    def pairwise(iterable):
-        """
-        Stand-in for itertools.pairwise()
-
-        pairwise('ABCDEFG') --> AB BC CD DE EF FG.
-        """
-
-        a, b = tee(iterable)
-        next(b, None)  # Remove first item of second sequence.
-        return zip(a, b)  # Pairs until second sequence is exhausted.
 
+from bokeh.models import (BasicTicker, ColumnDataSource, CustomJS, FactorRange)
+from bokeh.plotting import figure
+from bokeh.transform import linear_cmap, log_cmap
+
+## Imports from this package
+from ..base import tf_margins_only
+from ..dutils import date_tuples
 
 #%%
 
-def accumulate_list(items):
-    """
-    Initial subsequences of increasing length from list of items
+# Suppress quarterly or monthly axis labels for time series longer than this.
+DATE_THRESHOLD = 40
 
-    Generator of lists.
+#%%
 
-    Examples
-    --------
-    gen = accumulate_list([1, 2])
-    list(gen)
-    # [[], [1], [1, 2]]
-    """
-    for i in range(len(items) + 1):
-        yield items[:i]
+# Make a FactorRange from categorical scalars or tuples, with uniform padding.
+def _simple_factor_range(factor_values, *, padding=0.2, reverse=False):
+    axis_range = pd.Series(factor_values).unique()  # Do not sort.
+    if reverse:
+        axis_range = list(reversed(axis_range))
+    return FactorRange(factors=axis_range,
+                       factor_padding = padding,
+                       group_padding = padding,
+                       subgroup_padding = padding)
 
+#%%
 
-def cumulative_growth(data, columns, date_var="date"):
+def ts_categorical_figure(data,
+            x,
+            y,
+            values,
+            *,
+            x_hover=None,
+            title="(untitled)",
+            suppress_factors=False,
+            **kwargs):
     """
-    Growth of specified dataframe columns relative to earliest date
-
-    The row containing the minimum value of `date_var` provides baseline
-    values for calculating growth of the columns named by `columns`.
+    Make empty bokeh Figure with time series x and categorical y axis
 
     Parameters
     ----------
-    data: DataFrame
-        Dataframe including a date column and one or more columns for which
-        to calculate growth.
-
-    columns: str or list
-        Names of columns for which to calculate growth.
-
-    date_var: str, default "date"
-        Name of column whose minimum value determines the baseline row of data.
+    data: dict, DataFrame, or ColumnDataSource
+        Data, including x, y, and values.
+    x: str
+        Name of data variable specifying date values for the horizontal
+        axis.
+    y: str
+        Name of data variable specifying categorical values for the vertical
+        axis.
+    values: str
+        Name of data variable specifying numerical values for each combination
+        of x and y.
+    x_hover: str, optional
+        Name of data variable specifying pretty x values to display in hover
+        tool.  If not given, x will be used.
+    title: str
+        Title to display above figure.
+    suppress_factors: bool, default False
+        X axis tick labels omit lowest level from hierarchical tuple
+        categories, which are only displayed for the first and last ticks.
+        For example, if x values are like (2021, "Q1"), the years would be
+        shown but the quarters would mostly be suppressed to reduce clutter.
+    kwargs
+        Passed to bokeh.plotting.figure().
 
     Returns
     -------
-    DataFrame with same index as `data`, and columns from `columns`.
+    Bokeh Figure
     """
-    # Wrap single column name in a list, for convenience.
-    columns = [columns] if isinstance(columns, str) else columns
 
-    # Classify each row as having the earliest date or not.
-    is_min_date = data[date_var] == data[date_var].min()
+    # Convert data to CDS if necessary.
+    if isinstance(data, (dict, pd.DataFrame)):
+        source = ColumnDataSource(data)
+    else:
+        # Use presumed ColumnDataSource directly.
+        source = data
 
-    # Calculate baseline for each column from row with earliest date.
-    baseline = data.loc[is_min_date, columns] \
-        .reindex(index=data.index, method="nearest")  # Broadcast baseline to match shape of data.
-    return growth_pct_from(data[columns],
-                           baseline)
+    # Define categories for horizontal time axis.
+    x_range = _simple_factor_range(source.data[x], padding=0)
 
+    # Define categories for vertical axis.
+    y_range = _simple_factor_range(source.data[y], reverse=True)
 
-def date_tuples(dates, length_threshold = np.inf):
-    """
-    Coerce monthly, quarterly, or annual dates to tuples
+    TOOLS = "hover,tap,save,pan,box_zoom,reset,wheel_zoom"
+
+    if x_hover is None:
+        x_hover = x
+    tooltips = tooltips=[(f'{y}', f'@{y}'),
+                      (f'{x_hover}', f'@{x_hover}'),
+                      (f'{values}', f'@{values}')]
+
+    fopts = dict(
+        title=title,
+        x_range=x_range,
+        y_range=y_range,
+        x_axis_location="above",
+        #width=900, height=400,
+        tools=TOOLS, toolbar_location='below',
+        tooltips=tooltips,
+        )
+    fopts.update(kwargs)
+
+    fig = figure(**fopts)
+    fig.toolbar.logo = None  # Hide bokeh logo.
+
+    fig.grid.grid_line_color = None
+
+    axis = fig.axis
+    axis.axis_line_color = None
+    axis.major_tick_line_color = None
+    axis.major_label_text_font_size = "9px"
+    axis.major_label_standoff = 0
+
+    if suppress_factors:
+        # Suppress most lowest level categorical tick labels.
+        # If tick labels are tuples, higher levels will be displayed
+        # as normal.
+        fig.xaxis[0].formatter = tf_margins_only
+    elif len(x_range.factors) > 10:
+        # Rotate labels to reduce crowding
+        fig.xaxis.major_label_orientation = pi / 3
 
-    Tuples (if converted to a list) are suitable for `bokeh` categorical axis
+    # Arrange for tap to select one cell of the figure source data.
+    # fig.select(type=TapTool)
 
-    Parameters
-    dates : Sequence of str
-        Dates which may be annual ('2021'), quarterly ('2021 Q3'), or
-        monthly ('March 2021' or anything recognised by Pandas
-        `.to_period()`).
-    length_threshold : integer, default np.inf
-        If the number of unique `dates` exceeds this threshold, only the
-        last two digits of years are used.  The default is to always
-        use four-digit years.  If 0 is given, only the last two digits
-        of years will be used, regardless of how many different `dates`
-        there are.
-    """
+    return fig
 
-    dates = pd.Series(dates)
-
-    sample_date = dates[0]
-    n_dates = len(dates.unique())
+#%%
 
-    if re.fullmatch("\d{4}", sample_date):
-        # Annual like '2019', use as is.
-        if n_dates > length_threshold:
-            # Keep only last two digits of year.
-            tdate = [year[-2:] for year in dates]
+# Apply a color mapper.
+def _color_mapper(source, values, *, mapper=None, palette=None):
+    if palette is None:
+        palette = "Viridis256"
+    if mapper is None or mapper == "linear":
+        mapper = linear_cmap
+    elif mapper == "log":
+        mapper = log_cmap
+
+    data = pd.Series(source.data[values])
+    low, high = data.min(), data.max()
+
+    # Avoid degenerate range of values.
+    if low == high:
+        if high < 0:
+            high = 0  # low..0
+        elif low > 0:
+            low = 0  # 0..high
         else:
-            tdate = list(dates)
-        return tdate
-
-    if re.fullmatch("\d{4} ?Q\d", sample_date.upper()):
-        # Quarterly like '2019Q3' or '2019 Q3'.
-        # Wrap in a tuple for Bokeh categorical axis.
-        tdate = dates.str.split(" ").apply(tuple)
-    else:
-        # Maybe monthly will work.
-        # Create canonical (year, Mmm) category via datetime.
-        dt_dates = pd.to_datetime(dates).dt.to_period("M")
-        tdate = list(zip(dt_dates.dt.year.astype(str), dt_dates.dt.month.apply('M{:02d}'.format)))
-
-    if n_dates > length_threshold:
-        # Keep only last two digits of year.
-        tdate = [(year[-2:], _) for (year, _) in tdate]
-    return tdate
-
-
-def dict_fill(keys, values):
-    """
-    Map keys to values, recycling values as necessary
-    """
-
-    return dict(zip(keys, cycle(values)))
+            high = 1  # 0..1
 
-
-def growth_pct_from(data, baseline):
+    color_map = mapper(values, palette,
+                        low=low,
+                        high=high)
+    return color_map
+
+
+def heatmap(fig,
+            data,
+            x,
+            y,
+            values,
+            *,
+            color_map=None,
+            palette=None,
+            mapper=None,
+            **kwargs):
     """
-    Percentage growth relative to baseline value
+    Make interactive heatmap of categorical data
 
     Parameters
     ----------
-    data: numeric, Series or DataFrame
-        Data for which to calculate growth
-
-    baseline: numeric, Series or DataFrame
-        Value or values to calculate growth relative to.
+    fig: Bokeh Figure
+        Glyph rectangles are added to the figure to create a heatmap.
+    data: dict, DataFrame, or ColumnDataSource
+        Data, including x, y, and values.
+    x: str
+        Name of data variable specifying date values for the horizontal
+        axis.
+    y: str
+        Name of data variable specifying categorical values for the vertical
+        axis.
+    values: str
+        Name of data variable specifying numerical values for each combination
+        of x and y.
+    color_map: Bokeh color map, optional
+        Maps data values to colors.  If not given, a linear_cmap will be
+        created.
+    palette: Bokeh color palette, default "Viridis256"
+        Used to create a color map.  Ignored if color_map is specified.
+    mapper: "linear", "log", or callable
+        Used to create a color map.  Ignored if color_map is specified.
+    kwargs
+        Passed to fig.rect().
 
     Returns
     -------
-    Same shape as `data`, calculated as `(data / baseline - 1) * 100`, which
-    is often written as `100 * (data - baseline)/baseline`.
-
-    Examples
-    --------
-    ## Single value
-    growth_pct_from(110, 100)
-    # 10
-
-    ## Year on year growth
-    df = pd.DataFrame(dict(year=[2000, 2001, 2002], jobs=[40, 50, 20]))
-    baseline = df.jobs[df.year == 2001].values[0]
-    df["jobs_yoy"] = growth_pct_from(df, baseline)
-
-    ## Cumulative growth for two columns
-    df = pd.DataFrame(dict(
-        year=[2000, 2001, 2002],
-        jobs=[40, 50, 20],
-        gva=[200, 250, 275]))
-    baseline = df.loc[df.year == df.year.min(),
-                      ("jobs", "gva")].reindex(index=df.index,
-                                               method="nearest")
-    df[["jobs_growth", "gva_growth"]] = growth_pct_from(df[["jobs", "gva"]],
-                                                        baseline)
-    df
+    Bokeh Figure
     """
 
-    return (data / baseline - 1) * 100
+    # Convert data to CDS if necessary.
+    if isinstance(data, (dict, pd.DataFrame)):
+        source = ColumnDataSource(data)
+    else:
+        # Use presumed ColumnDataSource directly.
+        source = data
 
+    if color_map is None:
+        color_map = _color_mapper(source, values,
+                                  palette=palette,
+                                  mapper=mapper)
+
+    r = fig.rect(x=x, y=y, width=1, height=1, source=source,
+               fill_color=color_map,
+               line_color=None,
+               nonselection_alpha=0.5,
+               **kwargs,
+               )
+
+    return r
+
+#%%
 
-def growth_vars(data, columns=[], date_var=None, by=None,
-                periods=1, baseline=None):
+def figheatmap(data,
+            x,
+            y,
+            values,
+            *,
+            title="(untitled)",
+            x_widget=None, y_widget=None,
+            figure_options={},
+            **kwargs):
     """
-    Calculate growth for columns in a dataframe
+    Make a heatmap figure, with color bar
 
     Parameters
     ----------
-    data: DataFrame
-        Dataframe including a date column and one or more columns for which
-        to calculate growth.
-
-    columns: str or list
-        Names of columns for which to calculate growth.
-
-    date_var: str, optional
-        Name of column whose values determine temporal order among data rows.
-
-    by: str, optional
-        Name of column used to determine groups for `groupby`.
-
-    periods: int, default 1
-        Lag, in number of rows, for calculating growth within time series.
-        Ignored if `baseline` is specified.
-
-    baseline: "first", numeric, Series or DataFrame
-        Value or values to calculate growth relative to.  If "first",
-        cumulative growth is calculated relative to the row with the smallest
-        value of `date_var`.  If `baseline` is not given, growth is
-        calculated within each time series.
+    data: dict, DataFrame, or ColumnDataSource
+        Data, including x, y, and values.
+    x: str
+        Name of data variable specifying date values for the horizontal
+        axis.
+    y: str
+        Name of data variable specifying categorical values for the vertical
+        axis.
+    values: str
+        Name of data variable specifying numerical values for each combination
+        of x and y.
+    title: str, optional
+        Title to display above figure.  The default is "(untitled)".
+    x_widget : Bokeh widget, optional
+        Tapping on the heatmap sets the .value property of this widget to
+        the x coordinate of the selected (tapped) cell.
+    y_widget : Bokeh widget, optional
+        Tapping on the heatmap sets the .value property of this widget to
+        the y coordinate of the selected (tapped) cell.
+    figure_options : dict, optional
+        Passed as keyword arguments to bokeh.plotting.fig().
+    **kwargs
+        Keyword arguments for Figure.rect().
 
     Returns
     -------
-    DataFrame with same index as `data`, and columns from `columns`.
-
-    Examples
-    --------
-    # Period-on-period
-    growth_vars(df, columns=["gva"], date_var="date", periods=1)
-
-    # Cumulative growth
-    growth_vars(df, columns=["gva"], date_var="date", baseline="first")
-
-    # Growth relative to single date.
-    growth_vars(df, columns=["gva"], date_var="date", baseline="2019 Q4")
-
-    # Revisions from comparable dataframe.
-    growth_vars(df, columns=["gva"], baseline=df_baseline)
-
-
-    # Growth relative to single date, with a split factor.
-    growth_vars(df, columns=["gva"], date_var="date", by="industry", baseline="2019 Q4")
-
-    # Same as:
-    baseline = data.loc[df["date"]==min(df["date"]), :].groupby("industry")["gva"].first()
-    growth_vars(df, columns=["gva"], date_var="date", baseline=baseline)
-
-
-    # Relative to calculated baseline for each level of `by`
-    baseline = data.loc[data["year"]=="2019", :].groupby("industry")["gva"].mean()
-    growth_vars(df, columns=["gva"], by="industry", baseline=baseline)
+    fig : bokeh.plotting.Figure
+        Heatmap figure.
     """
 
-    # Ensure data columns include the ones we need.
-    if date_var is not None:
-        assert date_var in data.columns
-    if by is not None:
-        assert by in data.columns
-    assert all(col in data.columns for col in columns), \
-        f"Some of {columns} are missing from data columns {data.columns}"
-
-
-    # Make placeholder copy of data ready to inject results into `columns`.
-    result = data.copy()
-    result[columns] = np.nan
-
-    # Expand baseline shortcuts ("first" or a value to match data[date_var]).
-    if baseline == "first":
-        # Put baseline at earliest date value to get cumulative growth.
-        if by is not None:
-            baseline = data.loc[data[date_var]==min(data[date_var]), :].groupby(by)[columns].first()
-        else:
-            baseline = data.loc[data[date_var]==min(data[date_var]), :]
-    elif baseline is not None and not isinstance(baseline, pd.DataFrame):
-        # Find column values from date_var == baseline.
-        df_baseline_columns = columns + [by] if by is not None else columns
-        df_baseline_raw = data.set_index(date_var).loc[baseline, df_baseline_columns]
-        if by is not None:
-            # Take mean for each of the columns at each level of `by`.
-            baseline = df_baseline_raw.groupby(by).mean()
-        else:
-            # Take mean for each of the columns.
-            baseline = df_baseline_raw.mean()
-    elif isinstance(baseline, pd.DataFrame):
-        # Expect baseline dataframe to have a value for each column, with optional `by` splits.
-        pass
+    # Convert data to CDS if necessary.
+    if isinstance(data, (dict, pd.DataFrame)):
+        source = ColumnDataSource(data)
     else:
-        assert baseline is None
+        # Use presumed ColumnDataSource directly.
+        source = data
 
-    if isinstance(baseline, pd.DataFrame):
-        # Get relative change of data compared to baseline dataframe.
+    # Transform monthly and quarterly dates to nested categories.
+    source.data["_date_factor"] = date_tuples(source.data[x],
+                                             length_threshold=DATE_THRESHOLD)
+
+    # Prepare to suppress most quarters or months on axis if lots of them.
+    n_dates = len(pd.unique(source.data[x]))
+    suppress_factors = n_dates > DATE_THRESHOLD
+
+    # growth_source = fig_growth_snapshot.select(StackUp)[0].source
+    fig = ts_categorical_figure(
+            source,
+            x="_date_factor",  # Use tuple dates on figure axis.
+            y=y,
+            values=values,
+            x_hover = x,  # Use original x dates for hover info.
+            suppress_factors=suppress_factors,
+            title=title,
+            **figure_options
+        )
+
+    hm_rect = heatmap(
+            fig,
+            source,
+            x="_date_factor",
+            y=y,
+            values=values,
+            **kwargs
+        )
+
+    color_bar = hm_rect.construct_color_bar(
+        major_label_text_font_size="8px",
+        ticker=BasicTicker(#desired_num_ticks=len(palette)
+                           ),
+        #formatter=PrintfTickFormatter(format="%d%%"),
+        label_standoff=6,
+        border_line_color=None,
+        padding=5
+    )
+
+    fig.add_layout(color_bar, 'right')
+
+    if x_widget is not None:
+        jscb_set_from_selection(x_widget,
+                                source=source,
+                                column=x)
+
+    if y_widget is not None:
+        jscb_set_from_selection(y_widget,
+                                source=source,
+                                column=y)
 
-        assert all(col in baseline.columns for col in columns), \
-            f"Some of {columns} are missing from baseline columns {baseline.columns}"
+    return fig
 
-        if by is not None and date_var not in baseline.columns:
-            # Use `by` to look up baseline rows to find baseline values for columns.
-            #  `by` dataframe should have index of `by` levels.
-            baseline_values = baseline.loc[data[by], columns].values
-        else:
-            # Align baseline to data, and compare baseline dataframe to columns.
-            join_columns = [date_var, by] if by is not None else [date_var]
-            join_keys = list(pd.MultiIndex.from_frame(data[join_columns]))
-            baseline_values = baseline.set_index(join_columns).loc[join_keys, columns].values
-
-        result[columns] = growth_pct_from(data[columns],
-                                          baseline=baseline_values)
-    else:
-        # Do period-on-period growth with each column.
-        if by is not None:
-            sorted_data = data.sort_values(date_var).groupby(by)[columns]
-        else:
-            sorted_data = data[columns].sort_values(date_var)
-        result[columns] = 100 * sorted_data.pct_change(periods=periods)
-    return result
+#%%
 
+_JSCB_SET_FROM_LAST_SELECTED = """
+    // Set .value property from last selected index a data source.
+    /* args
+        tgt: Object whose .value property will be assigned a value from
+            `source[column]` in the last selected row of the data source.
+        source: ColumnDataSource
+        column: Name of column supplying potential target values
+    */
+    var indices = source.selected.indices;
+    if (indices.length) {
+        var last_selected_index = indices[indices.length - 1];
+        var new_value = source.data[column][last_selected_index];
+        tgt.value = new_value;
+        console.log("Updating " + (tgt.name || "unnamed target"),
+                    new_value);
+    }
+    """
+
+def jscb_set_from_selection(obj, source, column):
+    """
+    Set object's .value dynamically in the browser from a source selection
+
+    Arguments
+    ---------
+    tgt: Bokeh object
+        The object's .value property will be assigned from `source[column]`,
+        indexed by the last of the source's selected indices.
+    source: ColumnDataSource
+    column: str
+        Name of column supplying potential values for the target.
 
-def index_to(data, baseline, to=100):
-    """
-    Scale data so values at `baseline` map to `to`
+    Returns
+    -------
+    None
 
-    Examples
-    --------
-    # Index (2001 = 100)
-    df = pd.DataFrame(dict(year=[2000, 2001, 2002], jobs=[40, 50, 20]))
-    baseline = df.jobs[df.year == 2001].values[0]
-    df["jobs_index"] = index_to(df.jobs, baseline)
-    df
-    #    year  jobs  jobs_index
-    # 0  2000    40        80.0
-    # 1  2001    50       100.0
-    # 2  2002    20        40.0
-    """
+    Side effects
+    ------------
+    Sets a CustomJS callback to trigger when source's selection changes.
+    """
+    callback = CustomJS(args={"tgt": obj,
+                              "source": source,
+                              "column": column},
+                        code=_JSCB_SET_FROM_LAST_SELECTED)
+    source.selected.js_on_change('indices', callback)
 
-    return data / baseline * to
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xplorts-0.7/src/xplorts/ghostbokeh.py` & `xplorts-0.8/src/xplorts/ghostbokeh.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/slideselect.py` & `xplorts-0.8/src/xplorts/slideselect.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/dblprod/xpdblprod.py` & `xplorts-0.8/src/xplorts/tscomp/xptscomp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,78 @@
 """
-Make standalone interactive charts for time series productivity data
+Make standalone interactive chart showing time series components and total
 
 When run from the command line, reads data from a CSV file and
-creates an HTML document that displays time series levels and cumulative
-growth components for one level of a split factor at a time, as well as
-a snapshot of growth components across all levels of the split factor for
-one time period.
+creates an HTML document that displays time series
+growth components for one level of a split factor at a time.
 
     In the CSV file, the first row of data defines column names.
     The file should include:
         - a column of dates (annual, quarterly or monthly),
-        - a column of category names, and
-        - one or more columns of data values to be plotted against dates.
+        - a column of category names for the split factor,
+        - a column of data values for totals at each date, and
+        - one or more columns of growth components at each date.
 
     An interactive chart is created, with widgets to select one of the
-    category names (from a pulldown list or a slider).  The chart shows
-    one line for each value column, with dates plotted along the horizontal
-    axis.
+    category names (from a pulldown list or a slider).  The chart plots
+    dates along the horizontal axis, with growth components shown as stacked
+    bars and totals shown as a time series line.
 
     The interactive chart is saved as an HTML file which requires
     a web browser to view, but does not need an active internet connection.
     Once created, the HTML file does not require Python,
     so it is easy to share the interactive chart.
 
 Command line interface
 ----------------------
-usage: dblprod.py [-h] [-b BY] [-d DATE] [-p LPROD] [-v GVA] [-l LABOUR]
-                      [-g ARGS] [-t SAVE] [-s]
-                      datafile
+usage: tscomp.py [-h] [-b BY] [-d DATE] [-l LINE] [-y BARS [BARS ...]]
+                 [-g ARGS] [-t SAVE] [-s]
+                 datafile
 
-Create interactive visualiser for labour productivity levels with a split
-factor
+Create interactive time series chart for growth components with a split factor
 
 positional arguments:
   datafile              File (CSV) with data series and split factor
 
 optional arguments:
-  -h, --help            Show this help message and exit
+  -h, --help            show this help message and exit
   -b BY, --by BY        Factor variable for splits
   -d DATE, --date DATE  Date variable
-  -p LPROD, --lprod LPROD
-                        Productivity variable
-  -v GVA, --gva GVA     Gross value added (GVA) variable
-  -l LABOUR, --labour LABOUR
-                        Labour variable (e.g. jobs or hours worked)
-  -g ARGS, --args ARGS  Keyword arguments.  YAML mapping of mappings.  The
-                        keys 'lines', 'growth_series' and 'growth_snapshot'
-                        can provide keyword arguments to pass to
-                        `prod_ts_lines`, `prod_ts_growth` and
-                        `prod_growth_snapshot`, respectively.
+  -l LINE, --line LINE  Variable to show as time series line
+  -y BARS [BARS ...], --bars BARS [BARS ...]
+                        Variables to show as stacked bars
+  -g ARGS, --args ARGS  Keyword arguments. YAML mapping of mappings. The keys
+                        'lines' and 'bars' can provide keyword arguments to
+                        pass to `ts_components_figure()`.
   -t SAVE, --save SAVE  Interactive .html to save, if different from the
                         datafile base
   -s, --show            Show interactive .html
 """
 
 #%%
-# Bokeh imports.
-from bokeh.layouts import column, layout, row
-from bokeh.models import TabPanel, Tabs
-from bokeh.models.widgets import Div
+from bokeh.layouts import layout
 from bokeh.io import save, show
+from bokeh.models.widgets import Div
 from bokeh import palettes
 
-# Other external imports.
 import argparse
 from collections import defaultdict
-import pandas as pd
 from pathlib import Path
+import pandas as pd
 import sys
-import textwrap
 import yaml
 
-# Internal imports.
-from ..base import (filter_widget,
+## Imports from this package
+from xplorts.tscomp import link_widget_to_tscomp_figure, ts_components_figure
+from xplorts.base import (filter_widget,
+                          iv_dv_figure,
                           set_output_file, unpack_data_varnames,
                           variables_cmap)
-from ..dutils import growth_vars
-from ..heatmap import figheatmap
-from . import figprodgrowsnap, figprodlines, figprodgrowts
+from xplorts.dutils import date_tuples
+
 
 #%%
 
 def _parse_args():
     """
     Parse command line arguments
 
@@ -96,196 +87,174 @@
 
     Resources
     ---------
     [argparse — Parser for command-line options, arguments and sub-commands](https://docs.python.org/3/library/argparse.html#dest)
     """
     # Check command line arguments.
     parser = argparse.ArgumentParser(
-        prog="python -m xplorts.dblprod",
-        description="Create interactive visualiser for labour productivity levels with a split factor"
+        prog="python -m xplorts.tscomp",
+        description="Create interactive time series chart for growth components with a split factor"
     )
     parser.add_argument("datafile",
                         help="File (CSV) with data series and split factor")
     parser.add_argument("-b", "--by", type=str,
                         help="Factor variable for splits")
 
     parser.add_argument("-d", "--date", type=str,
                         help="Date variable")
-    parser.add_argument("-p", "--lprod", type=str,
-                        help="Productivity variable")
-    parser.add_argument("-v", "--gva",
-                        type=str,
-                        help="Gross value added (GVA) variable")
-    parser.add_argument("-l", "--labour",
-                        type=str,
-                        help="Labour variable (e.g. jobs or hours worked)")
+
+    parser.add_argument("-l", "--line", type=str,
+                        help="Variable to show as time series line")
+    parser.add_argument("-y", "--bars",
+                        nargs="+", type=str,
+                        help="Variables to show as stacked bars")
     parser.add_argument("-g", "--args",
                         type=str,
                         help="""Keyword arguments.  YAML mapping of mappings.  The
-                            keys 'lines', 'growth_series' and 'growth_snapshot'
+                            keys 'lines' and 'bars'
                             can provide keyword arguments to pass to
-                            `prod_ts_lines`, `prod_ts_growth` and
-                            `prod_growth_snapshot`, respectively.""")
+                            `ts_components_figure()`.""")
 
     parser.add_argument("-t", "--save", type=str,
                         help="Interactive .html to save, if different from the datafile base")
 
     parser.add_argument("-s", "--show", action="store_true",
                         help="Show interactive .html")
 
     args = parser.parse_args()
 
-    # Unpack YAML args into dict of dict of keyword args for various figures.
+    # Unpack YAML args into dict of keyword args for ts_components_figure().
     # Will return an empty dict for keys not specified in --args option.
     args.args = {} if args.args is None else yaml.safe_load(args.args)
     args.args = defaultdict(dict, args.args)
-
     return(args)
 
 #%%
 
 # Suppress quarterly or monthly axis labels for time series longer than this.
 DATE_THRESHOLD = 40
 
+def figtscomp(data, *,
+                date,
+                by,
+                bars=None,
+                line=None,
+                widget=None,
+                color_map=None,
+                iv_dv_args=dict(),
+                **kwargs):
+
+    # Transform monthly and quarterly dates to nested categories.
+    data_local = data.copy()
+    data_local["_date_factor"] = date_tuples(data_local[date],
+                                             length_threshold=DATE_THRESHOLD)
+
+    # Prepare to suppress most quarters or months on axis if lots of them.
+    suppress_factors = (isinstance(data_local["_date_factor"][0],
+                                   tuple)
+                        and len(data_local["_date_factor"].unique())
+                            > DATE_THRESHOLD)
+
+    ## Show time series growth components (bars) and total (line).
+    fig = iv_dv_figure(
+        iv_data = data_local["_date_factor"],
+        iv_axis = "x",
+        suppress_factors = suppress_factors,
+        x_axis_label = iv_dv_args.pop("x_axis_label", date),
+        y_axis_label = iv_dv_args.pop("y_axis_label", "Value"),
+        **iv_dv_args
+    )
+
+    if isinstance(bars, str):
+        # Put single string in a list as a convenience.
+        bars = [bars]
+    dependent_variables = bars if line is None else [line] + bars
+
+    if color_map is None:
+        # Use special color for line.
+        c20 = palettes.Category20_20
+        category_colors = c20[2:3] + c20[:2] + c20[4:]
+        color_map = variables_cmap(dependent_variables,
+                                   category_colors)
+    palette = [color_map[var] for var in dependent_variables]
+
+    ts_components_figure(
+        fig,
+        data_local,
+        date_variable=dict(plot="_date_factor", hover=date),
+        bar_variables=bars,
+        line_variable=line,
+        by=by,
+        line_args = {} if line is None else {"color": palette[0]},
+        bar_args = {"color": palette if line is None else palette[1:]},
+        **kwargs,
+    )
+
+    if widget is not None:
+        link_widget_to_tscomp_figure(widget, fig)
+
+    return fig
+
+#%%
+
 def main():
+    # Running from command line.
+
     args = _parse_args()
 
-    # Read the data as is.
     data = pd.read_csv(args.datafile, dtype=str)
 
     # Unpack args specifying which data columns to use.
     varnames = unpack_data_varnames(
         args,
-        ["date", "by", "lprod", "gva", "labour"],
+        ["date", "by", "line", "bars"],
         data.columns)
 
-    datevar = varnames["date"]
-    dependent_variables = [varnames[var] for var in ("lprod", "gva", "labour")]
-
-    title = "xplor lprod: " + Path(args.datafile).stem
+    title = "tscomp: " + Path(args.datafile).stem
 
     # Configure output file for interactive html.
     set_output_file(
         args.save or args.datafile,
         title = title
     )
 
-    # Make palettes.
-    color_map = variables_cmap(["labour", "gva", "lprod"],
-                               palettes.Category20_3)
-
     # Convert str to float so we can plot the data.
+    bars = varnames["bars"]
+    if isinstance(bars, str):
+        # Put single string in a list as a convenience.
+        bars = [bars]
+    line = varnames["line"]
+    dependent_variables = bars if line is None else [line] + bars
     data[dependent_variables] = data[dependent_variables].astype(float)
 
-
     # Widget for `by`.
-    split_widget = filter_widget(data[varnames["by"]], title=varnames["by"])
-
-    # Widget for date.
-    date_widget = filter_widget(data[datevar], start_value="last")
+    widget = filter_widget(data[varnames["by"]], title=varnames["by"])
+    # link_widget_to_tscomp_figure(widget, fig)
 
-    fig_index_lines = figprodlines(
-        data,
-        varnames=varnames,
-        color_map=color_map,
-        widget=split_widget,
-        height=300, width=600,
-        **args.args["lines"])
-
-
-    # Calculate cumulative growth.
-    df_growth_cum = growth_vars(data,
-                            date_var=datevar,
-                            columns=dependent_variables,
-                            by=varnames["by"],
-                            baseline="first",
-                           )
-
-    fig_ts_growth = figprodgrowts(
-        df_growth_cum,
-        varnames=varnames,
-        color_map=color_map,
-        widget=split_widget,
-        height=300, width=600,
-        **args.args["growth_series"])
-
-
-    # Calculate period-on-period growth.
-    df_growth = growth_vars(data,
-                            date_var=datevar,
-                            columns=dependent_variables,
-                            by=varnames["by"],
-                            periods=1,
-                           )
-
-    # Truncate long levels of `by`, for axis labels.
-    by_var = varnames["by"]
-    df_growth[by_var] = df_growth[by_var].apply(
-        textwrap.shorten, args=(15,), placeholder='..'
-    )
-
-    fig_growth_snapshot = figprodgrowsnap(
-        df_growth,
-        varnames=varnames,
-        color_map=color_map,
-        widget=date_widget,
-        height=600, width=300,
-        **args.args["growth_snapshot"])
-
-    # Put level and growth charts, with widgets, on a tab.
-    ts_charts = column(split_widget, fig_index_lines, fig_ts_growth)
-    snapshot = column(date_widget, fig_growth_snapshot)
-    tab_levels = TabPanel(
-        title="Levels",
-        child=layout([
-            [ts_charts, snapshot],
-            ]))
-
-
-    ## Growth heatmap tab.
-    growth_heatmap = figheatmap(
-        df_growth,
-        x=varnames["date"],
-        y=varnames["by"],
-        values=varnames["lprod"],
-        x_widget=date_widget.handle,
-        y_widget=split_widget.handle,
-        title=varnames["lprod"] + " growth",
-        figure_options=dict(width=900, height=600),
-        )
-    tab_growth = TabPanel(
-        title="Growth heatmap",
-        child=row([growth_heatmap, fig_growth_snapshot, date_widget.handle]),
-        )
-
-
-    ## Cumulative growth heatmap tab.
-    cum_growth_heatmap = figheatmap(
-        df_growth_cum,
-        x=varnames["date"],
-        y=varnames["by"],
-        values=varnames["lprod"],
-        x_widget=date_widget.handle,
-        y_widget=split_widget.handle,
-        title=varnames["lprod"] + " cumulative growth",
-        figure_options=dict(width=900, height=600),
-        )
-    tab_cum_growth = TabPanel(
-        title="Cum growth heatmap",
-        child=column([cum_growth_heatmap, fig_ts_growth, split_widget.handle]),
-        )
+    fig = figtscomp(data,
+                date=varnames["date"],
+                by=varnames["by"],
+                bars=varnames["bars"],
+                line=varnames["line"],
+                widget=widget,
+                iv_dv_args = {
+                    "title": "Time series components and total",
+                    },
+                color_map = args.args.pop("color_map", None),
+                **args.args
+                )
 
-    # Make app that shows tabs of various charts.
+    # Make app that shows widget and chart.
     app = layout([
         Div(text="<h1>" + title),  # Show title as level 1 heading.
-        Tabs(tabs=[tab_levels, tab_growth, tab_cum_growth])])
+        [widget],
+        [fig]
+    ])
 
     if args.show:
         show(app)  # Save file and display in web browser.
     else:
         save(app)  # Save file.
 
-#%%
 
 if __name__ == "__main__":
-    # Running from command line (or in Notebook?).
     sys.exit(main())
```

### Comparing `xplorts-0.7/src/xplorts/heatmap/__init__.py` & `xplorts-0.8/src/xplorts/heatmap/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/heatmap/xpheatmap.py` & `xplorts-0.8/src/xplorts/heatmap/xpheatmap.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/lines/lines.py` & `xplorts-0.8/src/xplorts/lines/lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,16 @@
     cds_options: dict, default {}
        Mapping from column names to lists, to specify plotting attributes
        for multi_lines.  Each list should have a value for each of the
        data_variables, in the same order.
     tool_tips: list, default []
         Pre-existing tooltips to add to the hover tool in addition to the
         default tooltips.
+    kwargs: dict, optional
+        Additional keyword arguments are passed to multi_line().
     """
 
     if data_variables in (None, []):
         # Return empty list of renderers.
         return []
 
     # Wrap single data variable in list if necessary.
```

### Comparing `xplorts-0.7/src/xplorts/lines/xplines.py` & `xplorts-0.8/src/xplorts/lines/xplines.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 """
 Make standalone interactive line charts for time series data.
 
 When run from the command line, `xplines` reads data from a `csv` file and
 creates an HTML document that displays an interactive line chart.
-      
-    In the `csv` file, the first row of data defines column names.  
+
+    In the `csv` file, the first row of data defines column names.
     The file should include:
-        - a column of dates (annual, quarterly or monthly), 
-        - a column of category names, and 
-        - one or more columns of data values to be plotted against dates.  
+        - a column of dates (annual, quarterly or monthly),
+        - a column of category names, and
+        - one or more columns of data values to be plotted against dates.
 
     An interactive chart is created, with widgets to select one of the
     category names (from a pulldown list or a slider).  The chart shows
     one line for each value column, with dates plotted along the horizontal
     axis.
 
+Functions
+---------
+figlines
+    Make interactive line chart of time series data with split factor
+
+Constants
+---------
+DATE_THRESHOLD
+    Suppress quarterly or monthly axis labels for time series longer than this
+
 
 Command line interface
 ----------------------
 usage: xplines.py [-h] [-b BY] [-d DATEVAR] [-l LINES [LINES ...]]
                                [-g ARGS] [-p PALETTE] [-t SAVE | -T] [-s]
                                 datafile
 
@@ -53,61 +63,61 @@
 from pathlib import Path
 import sys
 import yaml
 
 # Internal imports.
 from xplorts.lines import grouped_multi_lines, link_widget_to_lines
 
-from xplorts.base import (filter_widget, iv_dv_figure, 
-                          set_output_file, unpack_data_varnames, 
+from xplorts.base import (filter_widget, iv_dv_figure,
+                          set_output_file, unpack_data_varnames,
                           variables_cmap)
 from xplorts.dutils import date_tuples
 
 #%%
 
 def _parse_args():
     """
     Parse command line arguments
-    
+
     Returns
     -------
     `argparse.Namespace` object
-    
+
     Examples
     --------
     args = _parse_args()
     data = pd.read_csv(args.datafile)
-    
+
     Resources
     ---------
     [argparse — Parser for command-line options, arguments and sub-commands](https://docs.python.org/3/library/argparse.html#dest)
     """
     # Check command line arguments.
     parser = argparse.ArgumentParser(
         prog="python -m xplorts.lines",
         description="Create interactive line charts for time series data with a split factor"
     )
-    parser.add_argument("datafile", 
+    parser.add_argument("datafile",
                         help="File (CSV) with data series and split factor")
     parser.add_argument("-b", "--by", type=str,
                         help="Factor variable for splits")
 
     parser.add_argument("-d", "--date", type=str,
                         help="Date variable")
-    parser.add_argument("-l", "--lines", 
+    parser.add_argument("-l", "--lines",
                         nargs="+", type=str,
                         help="Variables to show as time series lines")
-    parser.add_argument("-g", "--args", 
+    parser.add_argument("-g", "--args",
                         type=str,
                         help="Keyword arguments for grouped_multi_lines(), specified as YAML mapping")
 
-    parser.add_argument("-t", "--save", type=str, 
+    parser.add_argument("-t", "--save", type=str,
                         help="Name of interactive .html to save, if different from the datafile base")
 
-    parser.add_argument("-s", "--show", action="store_true", 
+    parser.add_argument("-s", "--show", action="store_true",
                         help="Show interactive .html")
 
     args = parser.parse_args()
 
     # Unpack YAML args into dict of keyword args for grouped_multi_lines().
     args.args = {} if args.args is None else yaml.safe_load(args.args)
     return(args)
@@ -116,95 +126,156 @@
 #%%
 
 # Suppress quarterly or monthly axis labels for time series longer than this.
 DATE_THRESHOLD = 40
 
 #%%
 
+def figlines(data, *,
+            date,
+            by,
+            data_variables,
+            widget=None,
+            color_map=None,
+            line_dash=None,
+            iv_dv_args=dict(),
+            **kwargs):
+    """
+    Make interactive line chart of time series data with split factor
+
+    Parameters
+    ----------
+    data : DataFrame
+        Including columns to be plotted, which are named in other parameters.
+    date : str
+        Name of column containing time series dates to plot along the horizontal
+        chart axis.
+    by : str
+        Name of column containing split levels.  The chart displays a single split
+        level at a time.
+    data_variables : list
+        List of column names to be plotted as time series lines.
+    widget : Bokeh widget, optional
+        The `value` attribute will be linked to the chart to make visible one
+        value of the `by` variable.
+    color_map : dict of colors, optional
+        Map data_variables to colors.
+    line_dash : list of line dash specifications, optional
+        For corresponding data_variables.
+    iv_dv_args : mapping
+        Keyword arguments passed to `iv_dv_figure()`.
+    kwargs : mapping
+        Keyword arguments passed to `grouped_multi_lines()`.
+
+    Returns
+    -------
+    Bokeh figure.
+    """
+
+    # Transform monthly and quarterly dates to nested categories.
+    data_local = data.copy()
+    data_local["_date_factor"] = date_tuples(data_local[date],
+                                             length_threshold=DATE_THRESHOLD)
+
+    # Prepare to suppress most quarters or months on axis if lots of them.
+    suppress_factors = (isinstance(data_local["_date_factor"][0],
+                                   tuple)
+                        and len(data_local["_date_factor"].unique())
+                            > DATE_THRESHOLD)
+
+    # Make empty figure for time series line chart.
+    fig_index_lines = iv_dv_figure(
+        iv_data = data_local["_date_factor"],
+        iv_axis = "x",
+        suppress_factors = suppress_factors,
+        title = "Time series levels",
+        # Use our own default label for y axis if none given.
+        y_axis_label = iv_dv_args.pop("y_axis_label", "Value"),
+        **iv_dv_args
+    )
+
+    if color_map is None:
+        color_map = variables_cmap(data_variables,
+                                   "Category20_20")
+    palette = [color_map[var] for var in data_variables]
+
+    if line_dash is None:
+        # Use dash for alternating line colors (but last one is always solid).
+        line_dash = ["solid"] * len(data_variables)
+        line_dash[0:-1:2] = ["dashed"] * len(data_variables[0:-1:2])
+
+    cds_options = {
+        "color": palette,
+        "line_dash": line_dash}
+
+    index_lines = grouped_multi_lines(
+        fig_index_lines,
+        data_local,
+        iv_variable=dict(plot="_date_factor", hover=date),
+        data_variables=data_variables,
+        by=by,
+        # default keyword args can be overridden by kwargs.
+        cds_options = kwargs.pop("cds_options", cds_options),
+        color = kwargs.pop("color", "color"),
+        line_dash = kwargs.pop("line_dash", "line_dash"),
+        line_alpha = kwargs.pop("line_alpha", 0.8),
+        hover_line_alpha = kwargs.pop("hover_line_alpha", 1),
+        line_width = kwargs.pop("line_width", 2),
+        hover_line_width = kwargs.pop("hover_line_width", 4),
+        **kwargs
+    )
+
+    if widget is not None:
+        link_widget_to_lines(widget, index_lines)
+    return fig_index_lines
+
+
+#%%
+
 def main():
     args = _parse_args()
 
     data = pd.read_csv(args.datafile, dtype=str)
-    
+
     # Unpack args specifying which data columns to use.
     varnames = unpack_data_varnames(
         args,
         ["date", "by", "lines"],
         data.columns)
     datavars = varnames["lines"]
-    
+
     title = "lines: " + Path(args.datafile).stem
-    
+
     # Configure output file for interactive html.
     set_output_file(
         args.save or args.datafile,
         title = title
     )
-    
+
     # Convert str to float so we can plot the data.
     data[datavars] = data[datavars].astype(float)
-    
+
     # Make a slide-select widget to choose industry.
     split_widget = filter_widget(data[varnames["by"]], title=varnames["by"])
-     
-    # Transform monthly and quarterly dates to nested categories.
-    datevar = varnames["date"]
-    data_local = data.copy()
-    data_local["_date_factor"] = date_tuples(data_local[datevar],
-                                             length_threshold=DATE_THRESHOLD)
-
-    # Prepare to suppress most quarters or months on axis if lots of them.
-    suppress_factors = (isinstance(data_local["_date_factor"][0], tuple)
-                        and len(data_local["_date_factor"].unique()) > DATE_THRESHOLD)
 
-    fig = iv_dv_figure(
-        iv_axis = "x",
-        iv_data = data_local["_date_factor"],
-        suppress_factors = suppress_factors,
-        y_axis_label = "Value"
-    )
-    
-    default_color_map = variables_cmap(datavars,
-                                       "Category20_20")
-    default_line_colors = [default_color_map[var] for var in datavars]
-    
-    # Use dash for alternating line colors within each similar pair.
-    default_line_dash = ["solid"] * len(datavars)
-    default_line_dash[0:-1:2] = ["dashed"] * len(datavars[0:-1:2])
-    
-    default_args = dict(
-        line_alpha=0.8,
-        hover_line_alpha=1,
-        line_width=2,
-        hover_line_width=4,
-        cds_options=dict(color=default_line_colors,
-                         line_dash=default_line_dash),
-        color="color",
-        line_dash="line_dash"
-    )
-    
-    lines = grouped_multi_lines(
-        fig,
-        data_local,
-        iv_variable=dict(plot="_date_factor", hover=datevar),
-        data_variables=datavars,
-        by=varnames["by"],
-        **{**default_args, **args.args}
-    )
 
-    link_widget_to_lines(split_widget, lines)
+    fig = figlines(data,
+                    widget=split_widget,
+                    date=varnames["date"],
+                    by=varnames["by"],
+                    data_variables=datavars)
 
     # Make app that shows widget and chart.
     app = layout([
         Div(text="<h1>" + title),  # Show title as level 1 heading.
         [split_widget],
         [fig]
     ])
-    
+
     if args.show:
         show(app)  # Save file and display in web browser.
     else:
         save(app)  # Save file.
 
-    
+
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `xplorts-0.7/src/xplorts/scatter/scatter.py` & `xplorts-0.8/src/xplorts/scatter/scatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/scatter/xpscatter.py` & `xplorts-0.8/src/xplorts/scatter/xpscatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/snapcomp/__init__.py` & `xplorts-0.8/src/xplorts/snapcomp/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 Command line interface
 ----------------------
 > python -m xplorts.snapcomp --help
 """
 
 # Export names from .snapcomp.snapcomp.
 from .snapcomp import components_figure, link_widget_to_snapcomp_figure
+from .xpsnapcomp import figsnapcomp
 
-__all__ = ["components_figure", "link_widget_to_snapcomp_figure"]
+__all__ = ["components_figure", "figsnapcomp", "link_widget_to_snapcomp_figure"]
```

### Comparing `xplorts-0.7/src/xplorts/snapcomp/snapcomp.py` & `xplorts-0.8/src/xplorts/snapcomp/snapcomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/snapcomp/xpsnapcomp.py` & `xplorts-0.8/src/xplorts/dblprod/xpdblprod.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,86 @@
 """
-Make standalone chart showing horizontal snapshot components and total.
+Make standalone interactive charts for time series productivity data
 
 When run from the command line, reads data from a CSV file and
-creates an HTML document that displays snapshot
-components for one level of a split factor at a time.
+creates an HTML document that displays time series levels and cumulative
+growth components for one level of a split factor at a time, as well as
+a snapshot of growth components across all levels of the split factor for
+one time period.
 
     In the CSV file, the first row of data defines column names.
     The file should include:
-        - a column of category names for the vertical chart axis,
-        - a column of category names for the split factor
-        - a column of data totals at each level along the vertical axis, and
-        - one or more columns of value components for each total.
+        - a column of dates (annual, quarterly or monthly),
+        - a column of category names, and
+        - one or more columns of data values to be plotted against dates.
 
     An interactive chart is created, with widgets to select one of the
-    split factor levels (from a pulldown list or a slider).  The chart plots
-    value components as horizontal stacked bars with a marker for each total.
+    category names (from a pulldown list or a slider).  The chart shows
+    one line for each value column, with dates plotted along the horizontal
+    axis.
 
     The interactive chart is saved as an HTML file which requires
     a web browser to view, but does not need an active internet connection.
     Once created, the HTML file does not require Python,
     so it is easy to share the interactive chart.
 
 Command line interface
 ----------------------
-usage: snapcomp.py [-h] [-b BY] [-y IV] [-m MARKERS] [-x BARS [BARS ...]] [-L]
-                   [-g ARGS] [-t SAVE] [-s]
-                   datafile
+usage: dblprod.py [-h] [-b BY] [-d DATE] [-p LPROD] [-v GVA] [-l LABOUR]
+                      [-g ARGS] [-t SAVE] [-s]
+                      datafile
 
-Create interactive horizontal bar chart for snapshot components with a split
+Create interactive visualiser for labour productivity levels with a split
 factor
 
 positional arguments:
   datafile              File (CSV) with data series and split factor
 
 optional arguments:
-  -h, --help            show this help message and exit
+  -h, --help            Show this help message and exit
   -b BY, --by BY        Factor variable for splits
-  -y IV, --iv IV        Name of independent categorical variable for vertical
-                        axis
-  -m MARKERS, --markers MARKERS
-                        Variable to show as marker points
-  -x BARS [BARS ...], --bars BARS [BARS ...]
-                        Variables to show as horizontal stacked bars
-  -L, --last            Initial chart shows last level of `by` variable
-  -g ARGS, --args ARGS  Keyword arguments. YAML mapping of mappings. The keys
-                        'lines' and 'bars' can provide keyword arguments to
-                        pass to `components_figure()`.
+  -d DATE, --date DATE  Date variable
+  -p LPROD, --lprod LPROD
+                        Productivity variable
+  -v GVA, --gva GVA     Gross value added (GVA) variable
+  -l LABOUR, --labour LABOUR
+                        Labour variable (e.g. jobs or hours worked)
+  -g ARGS, --args ARGS  Keyword arguments.  YAML mapping of mappings.  The
+                        keys 'lines', 'growth_series' and 'growth_snapshot'
+                        can provide keyword arguments to pass to
+                        `prod_ts_lines`, `prod_ts_growth` and
+                        `prod_growth_snapshot`, respectively.
   -t SAVE, --save SAVE  Interactive .html to save, if different from the
                         datafile base
   -s, --show            Show interactive .html
-
 """
 
 #%%
-
+# Bokeh imports.
 from bokeh.layouts import layout
-from bokeh.io import save, show
+from bokeh.models import Tabs
 from bokeh.models.widgets import Div
-from bokeh import palettes
+from bokeh.io import save, show
 
+# Other external imports.
 import argparse
-from pathlib import Path
+from collections import defaultdict
 import pandas as pd
+from pathlib import Path
 import sys
 import yaml
 
-## Imports from this package
-from xplorts.snapcomp import components_figure, link_widget_to_snapcomp_figure
-from xplorts.base import (iv_dv_figure, filter_widget,
-                          set_output_file,
-                          unpack_data_varnames, variables_cmap)
+# Internal imports.
+from ..base import (set_output_file, unpack_data_varnames)
+from ..dashboard import dashboard_tabs
+from ..growthcomps import GrowthComponent, SignReversedComponent
+# from ..heatmap import figheatmap
+# from ..lines import figlines
+# from ..tscomp import figtscomp
+# from ..snapcomp import figsnapcomp
 
 #%%
 
 def _parse_args():
     """
     Parse command line arguments
 
@@ -88,133 +95,105 @@
 
     Resources
     ---------
     [argparse — Parser for command-line options, arguments and sub-commands](https://docs.python.org/3/library/argparse.html#dest)
     """
     # Check command line arguments.
     parser = argparse.ArgumentParser(
-        prog="python -m xplorts.snapcomp",
-        description="Create interactive horizontal bar chart for snapshot components with a split factor"
+        prog="python -m xplorts.dblprod",
+        description="Create interactive visualiser for labour productivity levels with a split factor"
     )
     parser.add_argument("datafile",
                         help="File (CSV) with data series and split factor")
     parser.add_argument("-b", "--by", type=str,
                         help="Factor variable for splits")
 
-    parser.add_argument("-y", "--iv", type=str,
-                        help="Name of independent categorical variable for vertical axis")
-
-    parser.add_argument("-m", "--markers", type=str,
-                        help="Variable to show as marker points")
-    parser.add_argument("-x", "--bars",
-                        nargs="+", type=str,
-                        help="Variables to show as horizontal stacked bars")
-
-    parser.add_argument("-L", "--last", action="store_true",
-                        help="Initial chart shows last level of `by` variable")
-
+    parser.add_argument("-d", "--date", type=str,
+                        help="Date variable")
+    parser.add_argument("-p", "--lprod", type=str,
+                        help="Productivity variable")
+    parser.add_argument("-v", "--gva",
+                        type=str,
+                        help="Gross value added (GVA) variable")
+    parser.add_argument("-l", "--labour",
+                        type=str,
+                        help="Labour variable (e.g. jobs or hours worked)")
     parser.add_argument("-g", "--args",
                         type=str,
                         help="""Keyword arguments.  YAML mapping of mappings.  The
-                            keys 'lines' and 'bars'
+                            keys 'lines', 'growth_series' and 'growth_snapshot'
                             can provide keyword arguments to pass to
-                            `components_figure()`.""")
+                            `prod_ts_lines`, `prod_ts_growth` and
+                            `prod_growth_snapshot`, respectively.""")
 
     parser.add_argument("-t", "--save", type=str,
                         help="Interactive .html to save, if different from the datafile base")
 
     parser.add_argument("-s", "--show", action="store_true",
                         help="Show interactive .html")
 
     args = parser.parse_args()
 
-    # Unpack YAML args into dict of keyword args for ts_components_figure().
+    # Unpack YAML args into dict of dict of keyword args for various figures.
+    # Will return an empty dict for keys not specified in --args option.
     args.args = {} if args.args is None else yaml.safe_load(args.args)
+    args.args = defaultdict(dict, args.args)
+
     return(args)
 
 #%%
 
+# Suppress quarterly or monthly axis labels for time series longer than this.
+DATE_THRESHOLD = 40
+
 def main():
-    # Running from command line.
     args = _parse_args()
 
+    # Read the data as is.
     data = pd.read_csv(args.datafile, dtype=str)
 
-    title = "snapcomp: " + Path(args.datafile).stem
+    # Unpack args specifying which data columns to use.
+    varnames = unpack_data_varnames(
+        args,
+        ["date", "by", "lprod", "gva", "labour"],
+        data.columns)
+
+    title = "xplor lprod: " + Path(args.datafile).stem
 
     # Configure output file for interactive html.
     set_output_file(
         args.save or args.datafile,
         title = title
     )
 
-    # Unpack args specifying which data columns to use.
-    varnames = unpack_data_varnames(
-        args,
-        ["iv", "by", "markers", "bars"],
-        data.columns)
-
-    # Make list of dependent variables for bars plus markers, if any.
-    markervar = varnames["markers"]
-    dependent_variables = varnames["bars"].copy()
-    if markervar is not None:
-        dependent_variables.insert(0, markervar)
-
     # Convert str to float so we can plot the data.
+    dependent_variables = [varnames[var] for var in ("lprod", "gva", "labour")]
     data[dependent_variables] = data[dependent_variables].astype(float)
 
-    default_color_map = variables_cmap(dependent_variables[::-1],
-                                       palettes.Category20_20)
-    default_bar_colors = [default_color_map[var] for var in varnames["bars"]]
-
-    fig = iv_dv_figure(
-        iv_data = reversed(data[varnames["iv"]].unique()),
-        iv_axis = "y",
-    )
+    components = [
+        GrowthComponent(varnames["gva"]),
+        SignReversedComponent(varnames["labour"]),
+        ]
+
+    tabs = dashboard_tabs(data,
+                           by=varnames["by"],
+                           date=varnames["date"],
+                           dv=varnames["lprod"],
+                           components=components,
+                           )
 
-    if markervar is None:
-        scatter_args = {}
-    else:
-        # Use specified scatter_args, else defaults.
-        scatter_args = args.args.pop(
-            "scatter_args",
-            {"color": default_color_map[markervar]})
-
-    # Use specified bar_args, else defaults.
-    bar_args = args.args.pop(
-        "bar_args",
-        {"color": default_bar_colors})
-
-    # Make chart, and link widget to make one factor level visible.
-    renderers = components_figure(
-        fig,
-        data,
-        by=varnames["by"],
-        marker_variable=varnames["markers"],
-        y=varnames["iv"],
-        bar_variables=varnames["bars"],
-        scatter_args=scatter_args,
-        bar_args=bar_args,
-        **args.args)
-
-    # Widget for `by`.
-    byvar = varnames["by"]
-    widget = filter_widget(data[byvar], title=byvar)
-    if args.last:
-        widget.value = widget.options[-1]
-    link_widget_to_snapcomp_figure(widget, fig)
-
-    # Make app that shows widget and chart.
+    # Make app that shows tabs of various charts.
     app = layout([
         Div(text="<h1>" + title),  # Show title as level 1 heading.
-        [widget],
-        [fig]
-    ])
+        Tabs(tabs=list(tabs.values()))
+        ])
 
     if args.show:
         show(app)  # Save file and display in web browser.
     else:
         save(app)  # Save file.
 
 #%%
+
 if __name__ == "__main__":
+    # Running from command line (or in Notebook?).
     sys.exit(main())
```

### Comparing `xplorts-0.7/src/xplorts/stacks/bokeh_stacks.py` & `xplorts-0.8/src/xplorts/stacks/bokeh_stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/stacks/stacks.py` & `xplorts-0.8/src/xplorts/stacks/stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/stacks/stacks_util.py` & `xplorts-0.8/src/xplorts/stacks/stacks_util.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/stacks/xpstacks.py` & `xplorts-0.8/src/xplorts/stacks/xpstacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/tscomp/__init__.py` & `xplorts-0.8/src/xplorts/tscomp/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 Command line interface
 ----------------------
 > python -m xplorts.tscomp --help
 """
 
 # Export names from .tscomp.tscomp.
 from .tscomp import link_widget_to_tscomp_figure, ts_components_figure
+from .xptscomp import figtscomp
 
-__all__ = ["link_widget_to_tscomp_figure", "ts_components_figure"]
+__all__ = ["figtscomp", "link_widget_to_tscomp_figure", "ts_components_figure"]
```

### Comparing `xplorts-0.7/src/xplorts/tscomp/tscomp.py` & `xplorts-0.8/src/xplorts/tscomp/tscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/src/xplorts/utils/ukons_lprod_to_csv.py` & `xplorts-0.8/src/xplorts/utils/ukons_lprod_to_csv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Save CSV with quarterly OPH CVM index by industry division, with GVA and hours index series
+Save CSV with labour productivity data by industry
 
 Can be imported as a module, or run from the command line as a Python script.
 
 When run from the command line, `ukons_lprod_to_csv` reads an Excel file
 containing UK Office for National Statistics (ONS) labour productivity data,
 and creates a `.csv` file with either annual or quarterly time series of
 productivity, gross value added, and labour index values.
@@ -33,152 +33,199 @@
   -t SAVE, --save SAVE  Save file (.csv), if different from the datafile base
 
 
 Application program interface (API)
 -----------------------------------
 GVA_TABLE_MAP
     Mapping of mappings to worksheet names.  The main keys are "annual" and
-    "quarterly".  The value for each is a mapping from keys "balanced", 
+    "quarterly".  The value for each is a mapping from keys "balanced",
     "bespoke", "section" or "division" to a worksheet name for the
     corresponding gross value added (GVA) chain volume index (CVM) data.
 
 read_lprod
     Read ONS labour productivity data.
 """
 
 import argparse
-import pandas as pd
 import re
 import yaml
 
 from collections import defaultdict
 from pathlib import Path
 
+from xplorts.dutils import find_in_metadata, read_sheet
+
 #%%
-    
-GVA_TABLE_MAP = {
+
+# Map granularity to names of GVA worksheets in OpH dataset.
+_OPH_GVA_TABLE_MAP = {
     "annual": {
         "balanced": "Table_1",
         "bespoke": "Table_7",
         "section": "Table_14",
         "division": "Table_21"
     },
     "quarterly": {
         "balanced": "Table_28",
         "bespoke": "Table_34",
         "section": "Table_42",
         "division": "Table_50"
     }
 }
 
+# Map granularity to names of GVA worksheets in OpJ dataset.
+_OPJ_GVA_TABLE_MAP = {
+    "annual": {
+        "balanced": "Table_1",
+        "bespoke": "Table_7",
+        "section": "Table_14",
+        "division": "Table_21"
+    },
+    "quarterly": {
+        "balanced": "Table_28",
+        "bespoke": "Table_34",
+        "section": "Table_42",
+        # No quarterly division tables
+    }
+}
+
+# Map granularity to names of GVA worksheets in OpW dataset.
+_OPW_GVA_TABLE_MAP = {
+    "annual": {
+        "balanced": "Table_1",
+        "bespoke": "Table_7",
+        # No annual section tables
+        # No annual division tables
+    },
+    "quarterly": {
+        "balanced": "Table_13",
+        "bespoke": "Table_19",
+        # No annual section tables
+        # No annual division tables
+    }
+}
+
 #%%
 
-def read_lprod(io, sheet_name, value_name, n_digits=4, **kwargs):
+def parse_lprod(data, name=None):
     """
-    Read ONS labour productivity data
-    
-    Reads a data table from an Excel file like "Output per hour worked",
+    Parse ONS labour productivity data
+
+    Parse a dataframe containing raw content of a worksheet from
+    an Excel file like "Output per hour worked",
     "Output per job" or "Output per worker".
-    
+
     Parameters
     ----------
-    io : as for pandas `read_excel`
-        Filename.
-    sheet_name : str
-        Worksheet to read.
-    value_name : str
-        Name to assign to data values.  Typically reflects the
-        content of the table, e.g. "gva" or "hours worked", etc.
-    n_digits : int, None
-        Number of data digits to keep.  Defaults to 4, making values
-        like "102.1234" or "0.1234".  If None, all digits are kept.
-    kwargs : mapping
-        Additional keyword arguments are passed to `read_excel`.
-        
+    data : dataframe
+        Worksheet containing data of interest, as strings.
+    name : str
+        Name to assign to the returned frame.  Typically reflects the
+        content of the table, e.g. "gva", "hours", etc.  If not given,
+        a name is derived from metadata in the top left corner of the
+        worksheet.
+
     Returns
     -------
-    Dataframe with three columns of str values, "date", "industry"
-    and `value_name`.
+    Dataframe in wide format, with `frame.index.name` set to "date",
+    `frame.columns.name set to "industry", and `frame.name` set to
+    `name`.
     """
-    
-    print(f"reading {value_name} from {sheet_name}")
-    data = pd.read_excel(io, sheet_name=sheet_name, 
-                         #engine="openpyxl",
-                         header=None, dtype=str, **kwargs)
-    # Find "SIC 2007 division" in column A.
+
+    ID_VAR = "date"
+    VAR_NAME = "industry"
+
+    if name is None:
+        # Identify content from cell A1 metadata.
+        metadata = data.iloc[0, 0].lower()
+
+        # Map substrings to measure names.
+        METADATA_MAP = {
+            "output per hour": "oph",
+            "output per job": "opj",
+            "output per worker": "opw",
+            "gross value added": "gva",
+            "hours worked": "hours",
+            "jobs": "jobs",
+            "workers": "workers",
+            }
+        substring = find_in_metadata(METADATA_MAP, metadata)
+        name = None if substring is None else METADATA_MAP[substring]
+
+    # Find "SIC 2007" in column A.
     has_sic2007 = data[0].str.startswith("SIC 2007")
     headers = data.loc[has_sic2007, :].set_index(0).T
     headers.columns = ["section", "division"]
+
+    # Join headers into single string for each column.
     headers = headers.section + ": " + headers.division
-    headers = headers.str.replace("A to T: 01 to 98", "WE")         .str.replace("Part of (.*): ", r"\1.")
-    
+    headers = headers.str.replace("A to T: 01 to 98", "WE") \
+        .str.replace("Part of (.*): ", r"\1.")  # "Part of C: blah" => "C.blah"
+
     last_header_row = data.index[has_sic2007].values[-1]
     df = data.iloc[last_header_row + 2:, :]
-    df.columns = ["date", *headers]
-
-    df_long = df.melt(id_vars="date", var_name="industry", value_name=value_name)
-    if n_digits is not None:
-        # Round off the data to reduce size a little.
-        df_long[value_name] = df_long[value_name].astype(float).round(n_digits).astype(str)
-    df_long.set_index(["date", "industry"], inplace=True)
-    return df_long
+    df.columns = [ID_VAR, *headers]
+    df.set_index(ID_VAR, inplace=True)
+    df.columns.name = VAR_NAME
+    df.name = name
+    return df
 
 #%%
 
 def _parse_args():
     """
     Parse command line arguments
-    
+
     Returns
     -------
     `argparse.Namespace` object
-    
+
     Examples
     --------
     args = _parse_args()
     data = pd.read_csv(args.datafile)
-    
+
     Resources
     ---------
     [argparse — Parser for command-line options, arguments and sub-commands](https://docs.python.org/3/library/argparse.html#dest)
     """
     # Check command line arguments.
     parser = argparse.ArgumentParser(
         description="Get corresponding labour productivity, gross value added and labour data"
     )
-    parser.add_argument("datafile", 
+    parser.add_argument("datafile",
                         help="File (.xls) formatted like ONS 'Output per hour' dataset")
-    
+
     period_group = parser.add_mutually_exclusive_group(required=True)
-    period_group.add_argument("-A", "--annual", action="store_true", 
+    period_group.add_argument("-A", "--annual", action="store_true",
                         help="Annual series")
-    period_group.add_argument("-Q", "--quarterly", action="store_true", 
+    period_group.add_argument("-Q", "--quarterly", action="store_true",
                         help="Quarterly series")
-    
-    
+
+
     gdp_group = parser.add_mutually_exclusive_group(required=False)
     gdp_group.add_argument("-b", "--balanced", action="store_true",
                            help="Balanced GVA (whole economy only)")
     gdp_group.add_argument("-o", "--output", action="store_true",
                            help="Output approach (low level aggregates) (default)")
-    
-    
+
+
     granularity_group = parser.add_mutually_exclusive_group(required=False)
     granularity_group.add_argument("-S", "--section", action="store_true",
                         help="By SIC industry section (default)")
     granularity_group.add_argument("-D", "--division", action="store_true",
                         help="By SIC industry division")
     granularity_group.add_argument("-B", "--bespoke", action="store_true",
                         help="Bespoke industry aggregations")
 
-    parser.add_argument("-g", "--args", 
+    parser.add_argument("-g", "--args",
                         type=str,
                         help="Keyword arguments(?)")
 
-    parser.add_argument("-t", "--save", type=str, 
+    parser.add_argument("-t", "--save", type=str,
                         help="Save file (.csv), if different from the datafile base")
 
     args = parser.parse_args()
 
     # Unpack YAML args into dict of dict of keyword args for various figures.
     # Will return an empty dict if no --args option specified.
     args.args = {} if args.args is None else yaml.safe_load(args.args)
@@ -188,40 +235,61 @@
 
 #%%
 
 # Make class that supports adding increment to a table name.
 class _TableName():
     def __init__(self, name):
         self.name = name
-    
+
     def __add__(self, inc):
         return re.sub(r"_(.*)$", lambda match: f"_{int(match.group(1)) + inc}", self.name)
 
 #%%
 
 if __name__ == "__main__":
     # Running from command line.
-    
+
     args = _parse_args()
     print(args)
 
     filepath = Path(args.datafile)
 
     period = "annual" if args.annual else "quarterly"
     gdp_type = "balanced" if args.balanced else "output"
     granularity = "bespoke" if args.bespoke else (
         "division" if args.division else "section"
     )
-    
+
+    # Determine whether dataset is oph, opj, or opw.
+    df_annual_bespoke_lprod = read_sheet(
+        args.datafile,
+        sheet_name="Table_11",
+        sheet_parser=parse_lprod)
+    dataset = df_annual_bespoke_lprod.name
+
+    # Get mapping from granularity to the dataset's GVA worksheet.
+    gva_table_map = {
+        "oph": _OPH_GVA_TABLE_MAP,
+        "opj": _OPJ_GVA_TABLE_MAP,
+        "opw": _OPW_GVA_TABLE_MAP
+        }[dataset]
+
+    # Identify which set of annual or quarterly data is specified.
     gva_key2 = "balanced" if args.balanced else granularity
-    worksheets = {"gva": GVA_TABLE_MAP[period][gva_key2]}
+
+    # Make mapping from gva, labour and lprod to worksheets.
+    worksheets = {"gva": gva_table_map[period][gva_key2]}
     worksheets["labour"] = _TableName(worksheets["gva"]) + 2
     worksheets["lprod"] = _TableName(worksheets["gva"]) + 4
 
-    df_map = {measure: read_lprod(args.datafile, worksheets[measure], value_name=measure)
-              for measure in ("lprod", "gva", "labour")}
+    df_map = {measure: read_sheet(args.datafile,
+                                  sheet_name=worksheet,
+                                  sheet_parser=parse_lprod)
+              for measure, worksheet in worksheets.items()}
+    # df_map = {measure: read_lprod(args.datafile, worksheets[measure], value_name=measure)
+    #           for measure in ("lprod", "gva", "labour")}
 
     lprod_long = df_map["lprod"].join([df_map[key] for key in ("gva", "labour")])         .reset_index()
     print(lprod_long.head())
 
     outfile = args.save if args.save is not None else filepath.with_suffix(".csv")
     lprod_long.to_csv(outfile, index=False)
```

### Comparing `xplorts-0.7/src/xplorts/utils/ukons_psp_to_csv.py` & `xplorts-0.8/src/xplorts/utils/ukons_psp_to_csv.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,21 +34,21 @@
     a worksheet name for the corresponding data.
 
 read_psp
     Read ONS total public service productivity data.
 """
 
 import argparse
-import pandas as pd
-import re
 import yaml
 
 from collections import defaultdict
 from pathlib import Path
 
+from xplorts.dutils import find_in_metadata, read_sheet
+
 #%%
 
 TABLE_MAP = {
     "adjusted": {
         "productivity": "3",
         "inputs": "7",
         "outputs": "5",
@@ -58,62 +58,67 @@
         "inputs": "7",
         "outputs": "6",
     }
 }
 
 #%%
 
-def read_psp(io, sheet_name, value_name, n_digits=4, **kwargs):
+def parse_psp(data, name=None):
     """
     Read ONS total public service productivity data
 
     Reads a data table from an Excel file like "totalpspreferencetables2020".
 
     Parameters
     ----------
-    io : as for pandas `read_excel`
-        Filename.
-    sheet_name : str
-        Worksheet to read.
-    value_name : str
-        Name to assign to data values.  Typically reflects the
-        content of the table, e.g. "productivity" or "inputs", etc.
-    n_digits : int, None
-        Number of data digits to keep.  Defaults to 4, making values
-        like "102.1234" or "0.1234".  If None, all digits are kept.
-    kwargs : mapping
-        Additional keyword arguments are passed to `read_excel`.
+    data : dataframe
+        Worksheet containing data of interest, as strings.
+    name : str
+        Name to assign to the returned frame.  Typically reflects the
+        content of the table, e.g. "alch", "ucl", etc.  If not given,
+        a name is derived from metadata in the top left corner of the
+        worksheet.
 
     Returns
     -------
-    Dataframe with three columns of str values, "date", "service"
-    and `value_name`.
+    Dataframe in wide format, with `frame.index.name` set to "date",
+    `frame.columns.name set to "service", and `frame.name` set to
+    `name`.
     """
 
-    print(f"reading {value_name} from {sheet_name}")
-    data = pd.read_excel(io, sheet_name=sheet_name,
-                         #engine="openpyxl",
-                         header=None, dtype=str, **kwargs)
+    ID_VAR = "date"
+    VAR_NAME = "service"
+
+    if name is None:
+        # Identify content from cell A1 metadata.
+        metadata = data.iloc[0, 0].lower()
+
+        # Map substrings to measure names.
+        METADATA_MAP = {
+            "productivity": "psp",
+            "output": "output",
+            "input": "input",
+            }
+        substring = find_in_metadata(METADATA_MAP, metadata)
+        name = None if substring is None else METADATA_MAP[substring]
+
     # Find "Year" in column A.
     has_year = data[0].str.startswith("Year")
     headers = data.loc[has_year, :].set_index(0).T
     headers.columns = ["service"]
     headers = headers.service
     headers = headers.str.replace(r"\[note .*\]", "", regex=True).str.strip()
 
     last_header_row = data.index[has_year].values[-1]
     df = data.iloc[last_header_row + 2:, :]
-    df.columns = ["date", *headers]
-
-    df_long = df.melt(id_vars="date", var_name="service", value_name=value_name)
-    if n_digits is not None:
-        # Round off the data to reduce size a little.
-        df_long[value_name] = df_long[value_name].astype(float).round(n_digits).astype(str)
-    df_long.set_index(["date", "service"], inplace=True)
-    return df_long
+    df.columns = [ID_VAR, *headers]
+    df.set_index(ID_VAR, inplace=True)
+    df.columns.name = VAR_NAME
+    df.name = name
+    return df
 
 #%%
 
 def _parse_args():
     """
     Parse command line arguments
 
@@ -168,17 +173,19 @@
     print(args)
 
     filepath = Path(args.datafile)
 
     adjustment = "adjusted" if args.adjusted else "nonadjusted"
     worksheets = TABLE_MAP[adjustment]
 
-    df_map = {measure: read_psp(args.datafile, worksheets[measure], value_name=measure)
+    df_map = {measure: read_sheet(args.datafile,
+                                  sheet_name=worksheets[measure],
+                                  sheet_parser=parse_psp)
               for measure in worksheets}
 
-    psp_long = df_map["productivity"].join([df_map[key]
+    data = df_map["productivity"].join([df_map[key]
                                             for key in ("inputs", "outputs")]) \
         .reset_index()
-    print(psp_long.head())
+    print(data.head())
 
     outfile = args.save if args.save is not None else filepath.with_suffix(".csv")
-    psp_long.to_csv(outfile, index=False)
+    data.to_csv(outfile, index=False)
```

### Comparing `xplorts-0.7/tests/conftest.py` & `xplorts-0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/tests/test_dblprod.py` & `xplorts-0.8/tests/test_dblprod.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/tests/test_heatmap.py` & `xplorts-0.8/tests/test_heatmap.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/tests/test_lines.py` & `xplorts-0.8/tests/test_lines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/tests/test_scatter.py` & `xplorts-0.8/tests/test_scatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/tests/test_stacks.py` & `xplorts-0.8/tests/test_stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/tests/test_tscomp.py` & `xplorts-0.8/tests/test_tscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/.gitignore` & `xplorts-0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `xplorts-0.7/LICENSE` & `xplorts-0.8/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -77,10 +77,13 @@
 ## Licenses and acknowledgements for incorporated data
 
 This section is a list of licenses and acknowledgements for third-party data included in the xplorts distribution.
 
 
 ### Output per hour worked
 
-The datasets `oph annual bespoke.csv`, `oph annual by division.csv`, `oph annual by section.csv`, `oph quarterly by section.csv` are extracts from `outputperhourworked.xls`, which was downloaded from [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk).
+The datasets `oph annual bespoke.csv`, `oph annual by division.csv`,
+`oph annual by section.csv`, `oph quarterly by section.csv` are extracts from
+`outputperhourworked.xls`, which was downloaded from
+[Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk).
 
 Source: Office for National Statistics licensed under the Open Government Licence v.3.0
```

### Comparing `xplorts-0.7/README.md` & `xplorts-0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -99,23 +99,26 @@
 ```
 
 ### Modules
 
 Module | Description
 --- | ---
 base | Miscellaneous helper functions and classes.
-dblprod | Modify a Bokeh Figure by adding charts to show labour productivity levels or growth components.
+dutils | Miscellaneous data manipulation helpers.
+dashboard | Multi-tab dashboard showing levels, growth components, and growth heatmaps.
+dblprod | Show labour productivity levels or growth components.
 ghostbokeh | Define an abstract base class to a build pseudo-subclass of a Bokeh class.
+growthcomps | Growth of time series and their contribution to growth of derived series.
 heatmap | Functions to create a heatmap of data values as a function of horizontal and vertical categorical variables.
-lines | Modify a Bokeh Figure by adding line charts to show several time series with a split factor.
-scatter | Modify a Bokeh Figure by adding scatter charts to show one or more categorical series with a split factor.
-slideselect | Defines a class combining select and slider widgets, with support for javascript linking to other objects.
-snapcomp | Modify a Bokeh Figure by adding a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and markers showing overall growth for each stack of bars.
-stacks | Modify a Bokeh Figure by adding a horizontal or vertical stacked bar chart showing several data series with a split factor.
-tscomp | Modify a Bokeh Figure by adding a time series growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.
+lines | Line charts to show several time series with a split factor.
+scatter | Scatter charts to show one or more categorical series with a split factor.
+slideselect | Class combining select and slider widgets, with support for javascript linking to other objects.
+snapcomp | Snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and markers showing overall growth for each stack of bars.
+stacks | Horizontal or vertical stacked bar chart showing several data series with a split factor.
+tscomp | Growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.
 </details>
 
 <details>
    <summary>
 
 ## Using `xplorts` on the command line
    </summary>
@@ -129,27 +132,27 @@
     ```activate my_env```
 
     On Mac:
 
     ```conda activate my_env```
 - Execute an `xplorts` module entry point
   ```
-  xp-dblprod ...
+  xp-dashboard ...
   ```
 - Or tell `python` explicitly to run an `xplorts` module
 
   ```
-  python -m xplorts.dblprod ...
+  python -m xplorts.dashboard ...
   ```
 
 ### Getting help about command line options
 
 Pass the option `-h` to any `xplorts` script to get help.  For example:
   ```
-  xp-dblprod -h
+  xp-dashboard -h
   ```
 
 Or
   ```
   python -m xplorts.dblprod -h
   ```
 
@@ -183,16 +186,19 @@
 >   -s, --show            Show interactive .html
 </pre>
 
 ### `xplorts` scripts
 
 Script | Entry point | Description
 --- | --- | ---
+dashboard | xp-dashboard | Multi-tab dashboard showing levels, growth components, and growth heatmaps.</li>
 dblprod | xp-dblprod | Create a labour productivity dashboard, with three charts including: <ul><li>a lines chart showing levels of labour productivity, gross value added, and labour,</li> <li>a time series growth components chart showing cumulative growth in labour productivity, gross value added, and labour, and</li> <li>a snapshot growth components chart showing period-on-period growth in labour productivity, gross value added, and labour.</li>
 heatmap | xp-heatmap | Create a heatmap of values as a function of two categorical variables.
 lines | xp-lines | Create a line chart showing several time series with a split factor.  Widgets select one split factor category at a time.
 scatter | xp-scatter | Create scatter chart showing one or more time series with a split factor.  Widgets select one split factor category at a time.
 snapcomp | xp-snapcomp | Create a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and a line showing overall growth.  A widget selects one time period at a time.
 stacks | xp-stacks | Create stacked bar chart showing several data series with a split factor.  Widgets select one split factor at a time (or one time period at a time if the split factor is plotted as a chart axis).
 tscomp | xp-tscomp | Create a time series growth components chart, with time periods along the horizontal axis, vertical stacked bars showing growth components, and a line showing overall growth.  Widgets select one split factor category at a time.
+utils.ukons_lcli_to_csv |  | Extract data from ONS [labour costs and labour income dataset](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/labourcostsandlabourshare), in a format suitable for use with `xplorts` charts.
 utils.ukons_lprod_to_csv |  | Extract data from ONS labour productivity datasets such as [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk), in a format suitable for use with `xplorts` charts.
+utils.ukons_psp_to_csv |  | Extract data from ONS dataset [Public service productivity estimates: total public service](https://www.ons.gov.uk/economy/economicoutputandproductivity/publicservicesproductivity/datasets/publicserviceproductivityestimatestotalpublicservice), in a format suitable for use with `xplorts` charts.
 </details>
```

### Comparing `xplorts-0.7/pyproject.toml` & `xplorts-0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xplorts"
-version = "0.7"
+version = "0.8"
 authors = [
-  { name="Todd M Bailey", email="tmb@baileywick.plus.com" },
+  { name="Todd M Bailey", email="tmb@baileywick.plus.com" }
 ]
 description = "Make standalone interactive HTML charts to explore time series datasets"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
     "bokeh >= 2.3.2",
     "numpy >= 1.19.2",
     "pandas >= 1.1.5",
     "pyyaml >= 5.4.1",
+    "xlrd >= 2.0.1"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 3 - Alpha'
 ]
 
 [project.scripts]
+xp-dashboard = "xplorts.dblprod.xpdashboard:main"
 xp-dblprod = "xplorts.dblprod.xpdblprod:main"
 xp-heatmap = "xplorts.heatmap.xpheatmap:main"
 xp-lines = "xplorts.lines.xplines:main"
 xp-scatter = "xplorts.scatter.xpscatter:main"
 xp-snapcomp = "xplorts.snapcomp.xpsnapcomp:main"
 xp-stacks = "xplorts.stacks.xpstacks:main"
 xp-tscomp = "xplorts.tscomp.xptscomp:main"
@@ -37,9 +39,9 @@
 [project.urls]
 "Homepage" = "https://github.com/xplorts/xplorts"
 "Bug Tracker" = "https://github.com/xplorts/xplorts/issues"
 
 [tool.hatch.build]
 exclude = [
   "zz *",
-  "data/*.html",
+  "data/*.html"
 ]
```

### Comparing `xplorts-0.7/PKG-INFO` & `xplorts-0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplorts
-Version: 0.7
+Version: 0.8
 Summary: Make standalone interactive HTML charts to explore time series datasets
 Project-URL: Homepage, https://github.com/xplorts/xplorts
 Project-URL: Bug Tracker, https://github.com/xplorts/xplorts/issues
 Author-email: Todd M Bailey <tmb@baileywick.plus.com>
 License: Copyright 2023 Todd Bailey
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
@@ -84,27 +84,31 @@
         ## Licenses and acknowledgements for incorporated data
         
         This section is a list of licenses and acknowledgements for third-party data included in the xplorts distribution.
         
         
         ### Output per hour worked
         
-        The datasets `oph annual bespoke.csv`, `oph annual by division.csv`, `oph annual by section.csv`, `oph quarterly by section.csv` are extracts from `outputperhourworked.xls`, which was downloaded from [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk).
+        The datasets `oph annual bespoke.csv`, `oph annual by division.csv`,
+        `oph annual by section.csv`, `oph quarterly by section.csv` are extracts from
+        `outputperhourworked.xls`, which was downloaded from
+        [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk).
         
         Source: Office for National Statistics licensed under the Open Government Licence v.3.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: bokeh>=2.3.2
 Requires-Dist: numpy>=1.19.2
 Requires-Dist: pandas>=1.1.5
 Requires-Dist: pyyaml>=5.4.1
+Requires-Dist: xlrd>=2.0.1
 Description-Content-Type: text/markdown
 
 
 <!-- This document uses
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/) -->
 
 # Explore time series datasets
@@ -204,23 +208,26 @@
 ```
 
 ### Modules
 
 Module | Description
 --- | ---
 base | Miscellaneous helper functions and classes.
-dblprod | Modify a Bokeh Figure by adding charts to show labour productivity levels or growth components.
+dutils | Miscellaneous data manipulation helpers.
+dashboard | Multi-tab dashboard showing levels, growth components, and growth heatmaps.
+dblprod | Show labour productivity levels or growth components.
 ghostbokeh | Define an abstract base class to a build pseudo-subclass of a Bokeh class.
+growthcomps | Growth of time series and their contribution to growth of derived series.
 heatmap | Functions to create a heatmap of data values as a function of horizontal and vertical categorical variables.
-lines | Modify a Bokeh Figure by adding line charts to show several time series with a split factor.
-scatter | Modify a Bokeh Figure by adding scatter charts to show one or more categorical series with a split factor.
-slideselect | Defines a class combining select and slider widgets, with support for javascript linking to other objects.
-snapcomp | Modify a Bokeh Figure by adding a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and markers showing overall growth for each stack of bars.
-stacks | Modify a Bokeh Figure by adding a horizontal or vertical stacked bar chart showing several data series with a split factor.
-tscomp | Modify a Bokeh Figure by adding a time series growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.
+lines | Line charts to show several time series with a split factor.
+scatter | Scatter charts to show one or more categorical series with a split factor.
+slideselect | Class combining select and slider widgets, with support for javascript linking to other objects.
+snapcomp | Snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and markers showing overall growth for each stack of bars.
+stacks | Horizontal or vertical stacked bar chart showing several data series with a split factor.
+tscomp | Growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.
 </details>
 
 <details>
    <summary>
 
 ## Using `xplorts` on the command line
    </summary>
@@ -234,27 +241,27 @@
     ```activate my_env```
 
     On Mac:
 
     ```conda activate my_env```
 - Execute an `xplorts` module entry point
   ```
-  xp-dblprod ...
+  xp-dashboard ...
   ```
 - Or tell `python` explicitly to run an `xplorts` module
 
   ```
-  python -m xplorts.dblprod ...
+  python -m xplorts.dashboard ...
   ```
 
 ### Getting help about command line options
 
 Pass the option `-h` to any `xplorts` script to get help.  For example:
   ```
-  xp-dblprod -h
+  xp-dashboard -h
   ```
 
 Or
   ```
   python -m xplorts.dblprod -h
   ```
 
@@ -288,16 +295,19 @@
 >   -s, --show            Show interactive .html
 </pre>
 
 ### `xplorts` scripts
 
 Script | Entry point | Description
 --- | --- | ---
+dashboard | xp-dashboard | Multi-tab dashboard showing levels, growth components, and growth heatmaps.</li>
 dblprod | xp-dblprod | Create a labour productivity dashboard, with three charts including: <ul><li>a lines chart showing levels of labour productivity, gross value added, and labour,</li> <li>a time series growth components chart showing cumulative growth in labour productivity, gross value added, and labour, and</li> <li>a snapshot growth components chart showing period-on-period growth in labour productivity, gross value added, and labour.</li>
 heatmap | xp-heatmap | Create a heatmap of values as a function of two categorical variables.
 lines | xp-lines | Create a line chart showing several time series with a split factor.  Widgets select one split factor category at a time.
 scatter | xp-scatter | Create scatter chart showing one or more time series with a split factor.  Widgets select one split factor category at a time.
 snapcomp | xp-snapcomp | Create a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and a line showing overall growth.  A widget selects one time period at a time.
 stacks | xp-stacks | Create stacked bar chart showing several data series with a split factor.  Widgets select one split factor at a time (or one time period at a time if the split factor is plotted as a chart axis).
 tscomp | xp-tscomp | Create a time series growth components chart, with time periods along the horizontal axis, vertical stacked bars showing growth components, and a line showing overall growth.  Widgets select one split factor category at a time.
+utils.ukons_lcli_to_csv |  | Extract data from ONS [labour costs and labour income dataset](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/labourcostsandlabourshare), in a format suitable for use with `xplorts` charts.
 utils.ukons_lprod_to_csv |  | Extract data from ONS labour productivity datasets such as [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk), in a format suitable for use with `xplorts` charts.
+utils.ukons_psp_to_csv |  | Extract data from ONS dataset [Public service productivity estimates: total public service](https://www.ons.gov.uk/economy/economicoutputandproductivity/publicservicesproductivity/datasets/publicserviceproductivityestimatestotalpublicservice), in a format suitable for use with `xplorts` charts.
 </details>
```

