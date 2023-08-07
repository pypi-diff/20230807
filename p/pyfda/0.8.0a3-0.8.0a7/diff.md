# Comparing `tmp/pyfda-0.8.0a3.tar.gz` & `tmp/pyfda-0.8.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfda-0.8.0a3.tar", last modified: Mon Aug  7 11:36:49 2023, max compression
+gzip compressed data, was "pyfda-0.8.0a7.tar", last modified: Mon Aug  7 16:58:01 2023, max compression
```

## Comparing `pyfda-0.8.0a3.tar` & `pyfda-0.8.0a7.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.622222 pyfda-0.8.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    10407 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/LICENSE_GPLv3.md
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-08-07 11:36:49.622222 pyfda-0.8.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/README_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.598220 pyfda-0.8.0a3/pyfda/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.598220 pyfda-0.8.0a3/pyfda/filter_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/bessel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/butter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/cheby1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/cheby2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/ellip.py
--rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/ellip_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/equiripple.py
--rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/firwin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filter_widgets/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/filterbroker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.598220 pyfda-0.8.0a3/pyfda/fixpoint_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/default_fx_img.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.598220 pyfda-0.8.0a3/pyfda/fixpoint_widgets/fir_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/fir_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/fir_df/fir_df.png
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    23218 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/fx_ui_wq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.602221 pyfda-0.8.0a3/pyfda/fixpoint_widgets/iir_df1/
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/iir_df1/iir_df1.png
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/fixpoint_widgets/no_fx_filter.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.590220 pyfda-0.8.0a3/pyfda/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.602221 pyfda-0.8.0a3/pyfda/images/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.610221 pyfda-0.8.0a3/pyfda/images/icons/dark/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/action-redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/action-undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/appbar.disk.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/appbar.from_clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/appbar.list.add.above.svg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/appbar.list.delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/appbar.to_clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/brush.svg
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/circle-check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/circle-x.svg
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/cog.svg
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/data-transfer-download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/data-transfer-upload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/density_large.svg
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/density_medium.svg
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/density_small.svg
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/ellipses_h.svg
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/ellipses_v.svg
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/fullscreen-enter.svg
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/graph_90.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/grid_coarse.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/grid_fine.svg
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/grid_none.svg
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/ic_help_24px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/ic_pause_48px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/ic_play_arrow_48px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/ic_stop_48px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/ic_volume_up_48px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/ic_volume_up_48px_90.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/lock-locked.svg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/lock-unlocked.svg
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/magnifying-glass.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/map-marker.svg
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/move.svg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/quantize.svg
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/sort-ascending.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/dark/trash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/fft.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.610221 pyfda-0.8.0a3/pyfda/images/icons/light/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/light/ic_pause_48px_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/light/ic_play_arrow_48px_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/plot_style-line-mkr.png
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/plot_style-line.png
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/plot_style-mkr.png
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/plot_style-none.png
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/plot_style-stem-mkr.png
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/plot_style-stem.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/plot_style-steps-mkr.png
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/plot_style-steps.png
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_128.png
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_16.png
--rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_48.png
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_64.png
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_nobg.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.610221 pyfda-0.8.0a3/pyfda/images/unused/
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/appbar.base.select_grey.svg
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/appbar.list.add.above_grey.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.614221 pyfda-0.8.0a3/pyfda/images/unused/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/audio_90.odg
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/audio_90.png
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/audio_90.svg
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/ic_fiber_manual_record_48px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/ic_forward_10_48px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/ic_mic_48px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/ic_skip_next_48px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/media-pause-4x.png
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/media-play-4x.png
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/media-record-4x.png
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/media-skip-backward-4x.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/media-skip-forward-4x.png
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/media-step-backward-4x.png
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/media-step-forward-4x.png
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/audio/media-stop-4x.png
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/camera-slr.svg
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/graph_90.odg
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/graph_90.png
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/grid-four-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/grid-three-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/grid-two-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/ic_volume_mute_48px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/question-mark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/square_outlined.svg
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/table_chart_outlined.svg
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/images/unused/table_outlined.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.614221 pyfda-0.8.0a3/pyfda/input_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/amplitude_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/freq_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21020 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/freq_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    44265 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/input_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/input_coeffs_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    37825 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/input_fixpoint_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/input_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/input_info_about.py
--rw-r--r--   0 runner    (1001) docker     (123)    36469 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/input_pz.py
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/input_pz_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/input_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/input_tab_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/select_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/target_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/input_widgets/weight_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.618222 pyfda-0.8.0a3/pyfda/libs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/csv_option_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/frozendict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/pyfda_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/pyfda_fft_windows_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    44490 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/pyfda_fix_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    62234 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/pyfda_io_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    59886 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/pyfda_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/pyfda_log_template.conf
--rw-r--r--   0 runner    (1001) docker     (123)    27531 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/pyfda_qt_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    28819 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/pyfda_sig_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/pyfda_template.conf
--rw-r--r--   0 runner    (1001) docker     (123)    30964 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/libs/tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/license_info.md
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/module_versions.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.618222 pyfda-0.8.0a3/pyfda/plot_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36450 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/mpl_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    29100 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/plot_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    27085 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/plot_fft_win.py
--rw-r--r--   0 runner    (1001) docker     (123)    35131 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/plot_hf.py
--rw-r--r--   0 runner    (1001) docker     (123)    92610 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/plot_impz.py
--rw-r--r--   0 runner    (1001) docker     (123)    35609 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/plot_impz_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/plot_phi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/plot_pz.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/plot_tab_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/plot_tau_g.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.622222 pyfda-0.8.0a3/pyfda/plot_widgets/tran/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/tran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25296 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/tran/plot_tran_stim.py
--rw-r--r--   0 runner    (1001) docker     (123)    48691 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/tran/plot_tran_stim_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/tran/tran_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/plot_widgets/tran/tran_io_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/pyfda.qrc
--rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/pyfda_rc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/pyfdax.py
--rw-r--r--   0 runner    (1001) docker     (123)   129275 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/qrc_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.622222 pyfda-0.8.0a3/pyfda/widget_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/widget_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.622222 pyfda-0.8.0a3/pyfda/widget_templates/filter_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/widget_templates/filter_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/widget_templates/filter_widgets/my_filter_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.622222 pyfda-0.8.0a3/pyfda/widget_templates/fixpoint_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/widget_templates/fixpoint_widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.622222 pyfda-0.8.0a3/pyfda/widget_templates/input_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/widget_templates/input_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/widget_templates/input_widgets/my_input_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.622222 pyfda-0.8.0a3/pyfda/widget_templates/plot_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/widget_templates/plot_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfda/widget_templates/plot_widgets/myplot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:36:49.598220 pyfda-0.8.0a3/pyfda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-08-07 11:36:49.000000 pyfda-0.8.0a3/pyfda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-08-07 11:36:49.000000 pyfda-0.8.0a3/pyfda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:36:49.000000 pyfda-0.8.0a3/pyfda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-07 11:36:49.000000 pyfda-0.8.0a3/pyfda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 11:36:49.000000 pyfda-0.8.0a3/pyfda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-07 11:36:49.000000 pyfda-0.8.0a3/pyfda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/pyfdax.spec
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 11:36:49.622222 pyfda-0.8.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-08-07 11:36:40.000000 pyfda-0.8.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10407 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/LICENSE_GPLv3.md
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/README_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.630228 pyfda-0.8.0a7/pyfda/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.634228 pyfda-0.8.0a7/pyfda/filter_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/bessel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/butter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/cheby1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/cheby2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/ellip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/ellip_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/equiripple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/firwin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filter_widgets/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/filterbroker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.634228 pyfda-0.8.0a7/pyfda/fixpoint_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/default_fx_img.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.634228 pyfda-0.8.0a7/pyfda/fixpoint_widgets/fir_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/fir_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/fir_df/fir_df.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23218 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/fx_ui_wq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.634228 pyfda-0.8.0a7/pyfda/fixpoint_widgets/iir_df1/
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/iir_df1/iir_df1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/fixpoint_widgets/no_fx_filter.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.626227 pyfda-0.8.0a7/pyfda/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.638228 pyfda-0.8.0a7/pyfda/images/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.642228 pyfda-0.8.0a7/pyfda/images/icons/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/action-redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/action-undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/appbar.disk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/appbar.from_clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/appbar.list.add.above.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/appbar.list.delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/appbar.to_clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/brush.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/circle-check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/circle-x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/cog.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/data-transfer-download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/data-transfer-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/density_large.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/density_medium.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/density_small.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/ellipses_h.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/ellipses_v.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/fullscreen-enter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/graph_90.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/grid_coarse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/grid_fine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/grid_none.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/ic_help_24px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/ic_pause_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/ic_play_arrow_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/ic_stop_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/ic_volume_up_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/ic_volume_up_48px_90.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/lock-locked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/lock-unlocked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/magnifying-glass.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/map-marker.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/move.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/quantize.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/sort-ascending.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/dark/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/fft.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.642228 pyfda-0.8.0a7/pyfda/images/icons/light/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/light/ic_pause_48px_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/light/ic_play_arrow_48px_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/plot_style-line-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/plot_style-line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/plot_style-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/plot_style-none.png
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/plot_style-stem-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/plot_style-stem.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/plot_style-steps-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/plot_style-steps.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_nobg.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.646227 pyfda-0.8.0a7/pyfda/images/unused/
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/appbar.base.select_grey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/appbar.list.add.above_grey.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.646227 pyfda-0.8.0a7/pyfda/images/unused/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/audio_90.odg
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/audio_90.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/audio_90.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/ic_fiber_manual_record_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/ic_forward_10_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/ic_mic_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/ic_skip_next_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/media-pause-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/media-play-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/media-record-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/media-skip-backward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/media-skip-forward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/media-step-backward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/media-step-forward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/audio/media-stop-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/camera-slr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/graph_90.odg
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/graph_90.png
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/grid-four-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/grid-three-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/grid-two-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/ic_volume_mute_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/question-mark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/square_outlined.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/table_chart_outlined.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/images/unused/table_outlined.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.650227 pyfda-0.8.0a7/pyfda/input_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/amplitude_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/freq_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21020 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/freq_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44265 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/input_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/input_coeffs_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37825 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/input_fixpoint_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/input_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/input_info_about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36469 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/input_pz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/input_pz_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/input_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/input_tab_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/select_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/target_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/input_widgets/weight_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.650227 pyfda-0.8.0a7/pyfda/libs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/csv_option_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/frozendict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/pyfda_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/pyfda_fft_windows_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44490 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/pyfda_fix_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62234 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/pyfda_io_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59886 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/pyfda_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/pyfda_log_template.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    27531 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/pyfda_qt_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28819 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/pyfda_sig_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/pyfda_template.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    30964 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/libs/tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/license_info.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/module_versions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/pyfda/plot_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36450 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/mpl_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29100 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/plot_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27085 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/plot_fft_win.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35131 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/plot_hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92610 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/plot_impz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35609 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/plot_impz_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/plot_phi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/plot_pz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/plot_tab_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/plot_tau_g.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/pyfda/plot_widgets/tran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/tran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25296 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/tran/plot_tran_stim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48691 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/tran/plot_tran_stim_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/tran/tran_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/plot_widgets/tran/tran_io_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/pyfda.qrc
+-rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/pyfda_rc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/pyfdax.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129275 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/qrc_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/pyfda/widget_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/widget_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/pyfda/widget_templates/filter_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/widget_templates/filter_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/widget_templates/filter_widgets/my_filter_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/pyfda/widget_templates/fixpoint_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/widget_templates/fixpoint_widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/pyfda/widget_templates/input_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/widget_templates/input_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/widget_templates/input_widgets/my_input_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/pyfda/widget_templates/plot_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/widget_templates/plot_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfda/widget_templates/plot_widgets/myplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:58:01.634228 pyfda-0.8.0a7/pyfda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-08-07 16:58:01.000000 pyfda-0.8.0a7/pyfda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-08-07 16:58:01.000000 pyfda-0.8.0a7/pyfda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:58:01.000000 pyfda-0.8.0a7/pyfda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-07 16:58:01.000000 pyfda-0.8.0a7/pyfda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 16:58:01.000000 pyfda-0.8.0a7/pyfda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-07 16:58:01.000000 pyfda-0.8.0a7/pyfda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/pyfdax.spec
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:58:01.654228 pyfda-0.8.0a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-08-07 16:57:51.000000 pyfda-0.8.0a7/setup.py
```

### Comparing `pyfda-0.8.0a3/AUTHORS.md` & `pyfda-0.8.0a7/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/CHANGELOG.md` & `pyfda-0.8.0a7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/INSTALLATION.md` & `pyfda-0.8.0a7/INSTALLATION.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/LICENSE.md` & `pyfda-0.8.0a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/LICENSE_GPLv3.md` & `pyfda-0.8.0a7/LICENSE_GPLv3.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/MANIFEST.in` & `pyfda-0.8.0a7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/PKG-INFO` & `pyfda-0.8.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfda
-Version: 0.8.0a3
+Version: 0.8.0a7
 Summary: Design and analyse discrete time DSP filters with a user-friendly GUI tool. Fixpoint filters in time and frequency domain, too.
 Home-page: https://github.com/chipmuenk/pyFDA
 Author: Christian Muenker
 Author-email: mail07@chipmuenk.de
 License: MIT
 Keywords: digital,discrete time,filter design,IIR,FIR,GUI
 Platform: any
```

### Comparing `pyfda-0.8.0a3/README.md` & `pyfda-0.8.0a7/README.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/README_PYPI.md` & `pyfda-0.8.0a7/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_factory.py` & `pyfda-0.8.0a7/pyfda/filter_factory.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/bessel.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/bessel.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/butter.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/butter.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/cheby1.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/cheby1.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/cheby2.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/cheby2.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/common.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/common.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/delay.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/delay.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/ellip.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/ellip.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/ellip_zero.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/ellip_zero.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/equiripple.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/equiripple.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/firwin.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/firwin.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/ma.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/ma.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filter_widgets/manual.py` & `pyfda-0.8.0a7/pyfda/filter_widgets/manual.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/filterbroker.py` & `pyfda-0.8.0a7/pyfda/filterbroker.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/fixpoint_widgets/default_fx_img.png` & `pyfda-0.8.0a7/pyfda/fixpoint_widgets/default_fx_img.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/fixpoint_widgets/fir_df/fir_df.png` & `pyfda-0.8.0a7/pyfda/fixpoint_widgets/fir_df/fir_df.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py` & `pyfda-0.8.0a7/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py` & `pyfda-0.8.0a7/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/fixpoint_widgets/fx_ui_wq.py` & `pyfda-0.8.0a7/pyfda/fixpoint_widgets/fx_ui_wq.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/fixpoint_widgets/iir_df1/iir_df1.png` & `pyfda-0.8.0a7/pyfda/fixpoint_widgets/iir_df1/iir_df1.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py` & `pyfda-0.8.0a7/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py` & `pyfda-0.8.0a7/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/fixpoint_widgets/no_fx_filter.png` & `pyfda-0.8.0a7/pyfda/fixpoint_widgets/no_fx_filter.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/dark/appbar.from_clipboard.svg` & `pyfda-0.8.0a7/pyfda/images/icons/dark/appbar.from_clipboard.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/dark/appbar.list.add.above.svg` & `pyfda-0.8.0a7/pyfda/images/icons/dark/appbar.list.add.above.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/dark/appbar.list.delete.svg` & `pyfda-0.8.0a7/pyfda/images/icons/dark/appbar.list.delete.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/dark/appbar.to_clipboard.svg` & `pyfda-0.8.0a7/pyfda/images/icons/dark/appbar.to_clipboard.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/dark/cog.svg` & `pyfda-0.8.0a7/pyfda/images/icons/dark/cog.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/dark/grid_coarse.svg` & `pyfda-0.8.0a7/pyfda/images/icons/dark/grid_coarse.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/dark/grid_fine.svg` & `pyfda-0.8.0a7/pyfda/images/icons/dark/grid_fine.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/dark/grid_none.svg` & `pyfda-0.8.0a7/pyfda/images/icons/dark/grid_none.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/dark/quantize.svg` & `pyfda-0.8.0a7/pyfda/images/icons/dark/quantize.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/fft.svg` & `pyfda-0.8.0a7/pyfda/images/icons/fft.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon.png` & `pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon.svg` & `pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_128.png` & `pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_128.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_16.png` & `pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_16.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_256.png` & `pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_256.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_32.png` & `pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_32.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_48.png` & `pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_48.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_64.png` & `pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_64.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/icons/pyfda_icon_nobg.svg` & `pyfda-0.8.0a7/pyfda/images/icons/pyfda_icon_nobg.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/unused/appbar.base.select_grey.svg` & `pyfda-0.8.0a7/pyfda/images/unused/appbar.base.select_grey.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/unused/appbar.list.add.above_grey.svg` & `pyfda-0.8.0a7/pyfda/images/unused/appbar.list.add.above_grey.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/unused/audio/audio.svg` & `pyfda-0.8.0a7/pyfda/images/unused/audio/audio.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/unused/audio/audio_90.odg` & `pyfda-0.8.0a7/pyfda/images/unused/audio/audio_90.odg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/unused/audio/audio_90.png` & `pyfda-0.8.0a7/pyfda/images/unused/audio/audio_90.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/unused/audio/audio_90.svg` & `pyfda-0.8.0a7/pyfda/images/unused/audio/audio_90.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/unused/audio/ic_forward_10_48px.svg` & `pyfda-0.8.0a7/pyfda/images/unused/audio/ic_forward_10_48px.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/unused/graph_90.odg` & `pyfda-0.8.0a7/pyfda/images/unused/graph_90.odg`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/images/unused/graph_90.png` & `pyfda-0.8.0a7/pyfda/images/unused/graph_90.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/amplitude_specs.py` & `pyfda-0.8.0a7/pyfda/input_widgets/amplitude_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/freq_specs.py` & `pyfda-0.8.0a7/pyfda/input_widgets/freq_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/freq_units.py` & `pyfda-0.8.0a7/pyfda/input_widgets/freq_units.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/input_coeffs.py` & `pyfda-0.8.0a7/pyfda/input_widgets/input_coeffs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/input_coeffs_ui.py` & `pyfda-0.8.0a7/pyfda/input_widgets/input_coeffs_ui.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/input_fixpoint_specs.py` & `pyfda-0.8.0a7/pyfda/input_widgets/input_fixpoint_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/input_info.py` & `pyfda-0.8.0a7/pyfda/input_widgets/input_info.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/input_info_about.py` & `pyfda-0.8.0a7/pyfda/input_widgets/input_info_about.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/input_pz.py` & `pyfda-0.8.0a7/pyfda/input_widgets/input_pz.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/input_pz_ui.py` & `pyfda-0.8.0a7/pyfda/input_widgets/input_pz_ui.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/input_specs.py` & `pyfda-0.8.0a7/pyfda/input_widgets/input_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/input_tab_widgets.py` & `pyfda-0.8.0a7/pyfda/input_widgets/input_tab_widgets.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/select_filter.py` & `pyfda-0.8.0a7/pyfda/input_widgets/select_filter.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/target_specs.py` & `pyfda-0.8.0a7/pyfda/input_widgets/target_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/input_widgets/weight_specs.py` & `pyfda-0.8.0a7/pyfda/input_widgets/weight_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/compat.py` & `pyfda-0.8.0a7/pyfda/libs/compat.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/csv_option_box.py` & `pyfda-0.8.0a7/pyfda/libs/csv_option_box.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/frozendict.py` & `pyfda-0.8.0a7/pyfda/libs/frozendict.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/pyfda_dirs.py` & `pyfda-0.8.0a7/pyfda/libs/pyfda_dirs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/pyfda_fft_windows_lib.py` & `pyfda-0.8.0a7/pyfda/libs/pyfda_fft_windows_lib.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/pyfda_fix_lib.py` & `pyfda-0.8.0a7/pyfda/libs/pyfda_fix_lib.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/pyfda_io_lib.py` & `pyfda-0.8.0a7/pyfda/libs/pyfda_io_lib.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/pyfda_lib.py` & `pyfda-0.8.0a7/pyfda/libs/pyfda_lib.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/pyfda_log_template.conf` & `pyfda-0.8.0a7/pyfda/libs/pyfda_log_template.conf`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/pyfda_qt_lib.py` & `pyfda-0.8.0a7/pyfda/libs/pyfda_qt_lib.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/pyfda_sig_lib.py` & `pyfda-0.8.0a7/pyfda/libs/pyfda_sig_lib.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/pyfda_template.conf` & `pyfda-0.8.0a7/pyfda/libs/pyfda_template.conf`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/libs/tree_builder.py` & `pyfda-0.8.0a7/pyfda/libs/tree_builder.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/license_info.md` & `pyfda-0.8.0a7/pyfda/license_info.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/module_versions.md` & `pyfda-0.8.0a7/pyfda/module_versions.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/mpl_widget.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/mpl_widget.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/plot_3d.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/plot_3d.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/plot_fft_win.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/plot_fft_win.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/plot_hf.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/plot_hf.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/plot_impz.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/plot_impz.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/plot_impz_ui.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/plot_impz_ui.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/plot_phi.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/plot_phi.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/plot_pz.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/plot_pz.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/plot_tab_widgets.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/plot_tab_widgets.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/plot_tau_g.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/plot_tau_g.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/tran/plot_tran_stim.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/tran/plot_tran_stim.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/tran/plot_tran_stim_ui.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/tran/plot_tran_stim_ui.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/tran/tran_io.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/tran/tran_io.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/plot_widgets/tran/tran_io_ui.py` & `pyfda-0.8.0a7/pyfda/plot_widgets/tran/tran_io_ui.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/pyfda.qrc` & `pyfda-0.8.0a7/pyfda/pyfda.qrc`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/pyfda_rc.py` & `pyfda-0.8.0a7/pyfda/pyfda_rc.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/pyfdax.py` & `pyfda-0.8.0a7/pyfda/pyfdax.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/qrc_resources.py` & `pyfda-0.8.0a7/pyfda/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/widget_templates/filter_widgets/my_filter_widget.py` & `pyfda-0.8.0a7/pyfda/widget_templates/filter_widgets/my_filter_widget.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/widget_templates/input_widgets/my_input_widget.py` & `pyfda-0.8.0a7/pyfda/widget_templates/input_widgets/my_input_widget.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda/widget_templates/plot_widgets/myplot.py` & `pyfda-0.8.0a7/pyfda/widget_templates/plot_widgets/myplot.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfda.egg-info/PKG-INFO` & `pyfda-0.8.0a7/pyfda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfda
-Version: 0.8.0a3
+Version: 0.8.0a7
 Summary: Design and analyse discrete time DSP filters with a user-friendly GUI tool. Fixpoint filters in time and frequency domain, too.
 Home-page: https://github.com/chipmuenk/pyFDA
 Author: Christian Muenker
 Author-email: mail07@chipmuenk.de
 License: MIT
 Keywords: digital,discrete time,filter design,IIR,FIR,GUI
 Platform: any
```

### Comparing `pyfda-0.8.0a3/pyfda.egg-info/SOURCES.txt` & `pyfda-0.8.0a7/pyfda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/pyfdax.spec` & `pyfda-0.8.0a7/pyfdax.spec`

 * *Files identical despite different names*

### Comparing `pyfda-0.8.0a3/setup.py` & `pyfda-0.8.0a7/setup.py`

 * *Files identical despite different names*

