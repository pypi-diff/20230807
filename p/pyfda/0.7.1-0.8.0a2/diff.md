# Comparing `tmp/pyfda-0.7.1.tar.gz` & `tmp/pyfda-0.8.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfda-0.7.1.tar", last modified: Wed Oct  5 10:20:39 2022, max compression
+gzip compressed data, was "pyfda-0.8.0a2.tar", last modified: Mon Aug  7 09:31:45 2023, max compression
```

## Comparing `pyfda-0.7.1.tar` & `pyfda-0.8.0a2.tar`

### file list

```diff
@@ -1,244 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-10-05 10:20:30.000000 pyfda-0.7.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)    14872 2022-10-05 10:20:30.000000 pyfda-0.7.1/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (121)    10407 2022-10-05 10:20:30.000000 pyfda-0.7.1/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-10-05 10:20:30.000000 pyfda-0.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)    34916 2022-10-05 10:20:30.000000 pyfda-0.7.1/LICENSE_GPLv3.md
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-10-05 10:20:30.000000 pyfda-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4063 2022-10-05 10:20:39.435194 pyfda-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10805 2022-10-05 10:20:30.000000 pyfda-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3009 2022-10-05 10:20:30.000000 pyfda-0.7.1/README_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.415194 pyfda-0.7.1/bak/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.415194 pyfda-0.7.1/bak/delay/
--rw-r--r--   0 runner    (1001) docker     (121)     5989 2022-10-05 10:20:30.000000 pyfda-0.7.1/bak/delay/fx_delay.py
--rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-10-05 10:20:30.000000 pyfda-0.7.1/bak/iir_df1_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.411194 pyfda-0.7.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.415194 pyfda-0.7.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.411194 pyfda-0.7.1/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.415194 pyfda-0.7.1/docs/source/_static/ideas/
--rw-r--r--   0 runner    (1001) docker     (121)    10120 2022-10-05 10:20:30.000000 pyfda-0.7.1/docs/source/_static/ideas/mpl_pyqt4_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)    10381 2022-10-05 10:20:30.000000 pyfda-0.7.1/docs/source/_static/ideas/plotTest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6580 2022-10-05 10:20:30.000000 pyfda-0.7.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.415194 pyfda-0.7.1/pyfda/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11597 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.419194 pyfda-0.7.1/pyfda/filter_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12391 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/bessel.py
--rw-r--r--   0 runner    (1001) docker     (121)    12065 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/butter.py
--rw-r--r--   0 runner    (1001) docker     (121)    10167 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/cheby1.py
--rw-r--r--   0 runner    (1001) docker     (121)    10187 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/cheby2.py
--rw-r--r--   0 runner    (1001) docker     (121)    10071 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     7218 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/delay.py
--rw-r--r--   0 runner    (1001) docker     (121)    11123 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/ellip.py
--rw-r--r--   0 runner    (1001) docker     (121)    25674 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/ellip_zero.py
--rw-r--r--   0 runner    (1001) docker     (121)    18533 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/equiripple.py
--rw-r--r--   0 runner    (1001) docker     (121)    25234 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/firwin.py
--rw-r--r--   0 runner    (1001) docker     (121)    15638 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/ma.py
--rw-r--r--   0 runner    (1001) docker     (121)     8332 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filter_widgets/manual.py
--rw-r--r--   0 runner    (1001) docker     (121)    14810 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/filterbroker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.419194 pyfda-0.7.1/pyfda/fixpoint_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9698 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/default_fx_img.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.419194 pyfda-0.7.1/pyfda/fixpoint_widgets/fir_df/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/fir_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10087 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/fir_df/fir_df.png
--rw-r--r--   0 runner    (1001) docker     (121)     7611 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py
--rw-r--r--   0 runner    (1001) docker     (121)    10307 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)    23228 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/fx_ui_wq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.419194 pyfda-0.7.1/pyfda/fixpoint_widgets/iir_df1/
--rw-r--r--   0 runner    (1001) docker     (121)    14526 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/iir_df1/iir_df1.png
--rw-r--r--   0 runner    (1001) docker     (121)    10369 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py
--rw-r--r--   0 runner    (1001) docker     (121)    14136 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)    15201 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/fixpoint_widgets/no_fx_filter.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.411194 pyfda-0.7.1/pyfda/images/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.419194 pyfda-0.7.1/pyfda/images/icons/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.427194 pyfda-0.7.1/pyfda/images/icons/dark/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/action-redo.svg
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/action-undo.svg
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/appbar.disk.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/appbar.from_clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/appbar.list.add.above.svg
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/appbar.list.delete.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/appbar.to_clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10910 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/audio_90.odg
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/brush.svg
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/camera-slr.svg
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/circle-check.svg
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/circle-x.svg
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/cog.svg
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/data-transfer-download.svg
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/data-transfer-upload.svg
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ellipses_h.svg
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ellipses_v.svg
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/file.svg
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/fullscreen-enter.svg
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/graph.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9027 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/graph_90.odg
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/graph_90.png
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/grid-four-up.svg
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/grid-three-up.svg
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/grid-two-up.svg
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/home.svg
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_fiber_manual_record_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_forward_10_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_hearing_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_help_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_help_outline_24px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_mic_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_pause_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_play_arrow_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_skip_next_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_stop_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_volume_mute_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_volume_up_48px.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/ic_volume_up_48px_90.svg
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/lock-locked.svg
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/lock-unlocked.svg
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/magnifying-glass.svg
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/map-marker.svg
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/media-pause-4x.png
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/media-play-4x.png
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/media-record-4x.png
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/media-skip-backward-4x.png
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/media-skip-forward-4x.png
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/media-step-backward-4x.png
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/media-step-forward-4x.png
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/media-stop-4x.png
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/move.svg
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/quantize.svg
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/question-mark.svg
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/sort-ascending.svg
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/dark/trash.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6909 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/fft.svg
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/graph.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/grid_coarse.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6228 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/grid_fine.svg
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/grid_man.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/grid_none.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/help.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.427194 pyfda-0.7.1/pyfda/images/icons/light/
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/light/appbar.base.select_grey.svg
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/light/appbar.list.add.above_grey.svg
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/light/ic_pause_48px_white.svg
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/light/ic_play_arrow_48px_white.svg
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/plot_style-line-mkr.png
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/plot_style-line.png
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/plot_style-mkr.png
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/plot_style-none.png
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/plot_style-stem-mkr.png
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/plot_style-stem.png
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/plot_style-steps-mkr.png
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/plot_style-steps.png
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/pyfda_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)     7356 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/pyfda_icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9898 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/pyfda_icon_128.png
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/pyfda_icon_16.png
--rw-r--r--   0 runner    (1001) docker     (121)    20271 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/pyfda_icon_256.png
--rw-r--r--   0 runner    (1001) docker     (121)     2677 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/pyfda_icon_32.png
--rw-r--r--   0 runner    (1001) docker     (121)     3944 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/pyfda_icon_48.png
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/pyfda_icon_64.png
--rw-r--r--   0 runner    (1001) docker     (121)     7171 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/icons/pyfda_icon_nobg.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.427194 pyfda-0.7.1/pyfda/images/unused/
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/unused/audio.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/unused/audio_90.png
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/images/unused/audio_90.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.431194 pyfda-0.7.1/pyfda/input_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13543 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/amplitude_specs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17325 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/freq_specs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17252 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/freq_units.py
--rw-r--r--   0 runner    (1001) docker     (121)    44460 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/input_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (121)    18306 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/input_coeffs_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)    37825 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/input_fixpoint_specs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22453 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/input_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    11027 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/input_info_about.py
--rw-r--r--   0 runner    (1001) docker     (121)    35005 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/input_pz.py
--rw-r--r--   0 runner    (1001) docker     (121)    14534 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/input_pz_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)    18026 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/input_specs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6600 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/input_tab_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    20844 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/select_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6502 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/target_specs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11838 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/input_widgets/weight_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.431194 pyfda-0.7.1/pyfda/libs/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5764 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     7682 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/csv_option_box.py
--rw-r--r--   0 runner    (1001) docker     (121)     6629 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/frozendict.py
--rw-r--r--   0 runner    (1001) docker     (121)    12156 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/pyfda_dirs.py
--rw-r--r--   0 runner    (1001) docker     (121)    39198 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/pyfda_fft_windows_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)    44490 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/pyfda_fix_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)    54511 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/pyfda_io_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)    57628 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/pyfda_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     6791 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/pyfda_log_template.conf
--rw-r--r--   0 runner    (1001) docker     (121)    24707 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/pyfda_qt_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)    28147 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/pyfda_sig_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     5661 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/pyfda_template.conf
--rw-r--r--   0 runner    (1001) docker     (121)    30964 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/libs/tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/license_info.md
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/module_versions.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.431194 pyfda-0.7.1/pyfda/plot_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29804 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/mpl_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)    28823 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/plot_3d.py
--rw-r--r--   0 runner    (1001) docker     (121)    27054 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/plot_fft_win.py
--rw-r--r--   0 runner    (1001) docker     (121)    31880 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/plot_hf.py
--rw-r--r--   0 runner    (1001) docker     (121)    86667 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/plot_impz.py
--rw-r--r--   0 runner    (1001) docker     (121)    32111 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/plot_impz_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     9728 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/plot_phi.py
--rw-r--r--   0 runner    (1001) docker     (121)    24001 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/plot_pz.py
--rw-r--r--   0 runner    (1001) docker     (121)     8979 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/plot_tab_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)     9821 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/plot_tau_g.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/plot_widgets/tran/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/tran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18714 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/tran/plot_tran_stim.py
--rw-r--r--   0 runner    (1001) docker     (121)    45858 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/tran/plot_tran_stim_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     4060 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/tran/tran_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     5080 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/plot_widgets/tran/tran_io_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/pyfda.qrc
--rw-r--r--   0 runner    (1001) docker     (121)    21558 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/pyfda_rc.py
--rw-r--r--   0 runner    (1001) docker     (121)    13937 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/pyfdax.py
--rw-r--r--   0 runner    (1001) docker     (121)   177185 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/qrc_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5698 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/test_fir_df.py
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/test_fixpoint_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    24879 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/test_pyfda_fix_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     8401 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/test_uniqueroots.py
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/test_uniqueroots_time.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/tests/widgets/input_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/widgets/input_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9629 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/widgets/input_widgets/test_input_coeffs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/tests/widgets/plot_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/tests/widgets/plot_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/widget_templates/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/widget_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/widget_templates/filter_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/widget_templates/filter_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8486 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/widget_templates/filter_widgets/my_filter_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/widget_templates/fixpoint_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/widget_templates/fixpoint_widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/widget_templates/input_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/widget_templates/input_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4125 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/widget_templates/input_widgets/my_input_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/pyfda/widget_templates/plot_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/widget_templates/plot_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfda/widget_templates/plot_widgets/myplot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.415194 pyfda-0.7.1/pyfda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4063 2022-10-05 10:20:39.000000 pyfda-0.7.1/pyfda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-10-05 10:20:39.000000 pyfda-0.7.1/pyfda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 10:20:39.000000 pyfda-0.7.1/pyfda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-05 10:20:39.000000 pyfda-0.7.1/pyfda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-05 10:20:39.000000 pyfda-0.7.1/pyfda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-05 10:20:39.000000 pyfda-0.7.1/pyfda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6059 2022-10-05 10:20:30.000000 pyfda-0.7.1/pyfdax.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 10:20:39.435194 pyfda-0.7.1/recipe/
--rw-r--r--   0 runner    (1001) docker     (121)     5598 2022-10-05 10:20:30.000000 pyfda-0.7.1/recipe/pyfdax.spec_bak.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-10-05 10:20:30.000000 pyfda-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-05 10:20:39.435194 pyfda-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5165 2022-10-05 10:20:30.000000 pyfda-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.071939 pyfda-0.8.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10407 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/LICENSE_GPLv3.md
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-08-07 09:31:45.071939 pyfda-0.8.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/README_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.047940 pyfda-0.8.0a2/pyfda/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.051940 pyfda-0.8.0a2/pyfda/filter_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/bessel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/butter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/cheby1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/cheby2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/ellip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/ellip_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/equiripple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/firwin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filter_widgets/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/filterbroker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.051940 pyfda-0.8.0a2/pyfda/fixpoint_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/default_fx_img.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.051940 pyfda-0.8.0a2/pyfda/fixpoint_widgets/fir_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/fir_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/fir_df/fir_df.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23218 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/fx_ui_wq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.051940 pyfda-0.8.0a2/pyfda/fixpoint_widgets/iir_df1/
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/iir_df1/iir_df1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/fixpoint_widgets/no_fx_filter.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.047940 pyfda-0.8.0a2/pyfda/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.055940 pyfda-0.8.0a2/pyfda/images/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.059939 pyfda-0.8.0a2/pyfda/images/icons/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/action-redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/action-undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/appbar.disk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/appbar.from_clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/appbar.list.add.above.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/appbar.list.delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/appbar.to_clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/brush.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/circle-check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/circle-x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/cog.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/data-transfer-download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/data-transfer-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/density_large.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/density_medium.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/density_small.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/ellipses_h.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/ellipses_v.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/fullscreen-enter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/graph_90.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/grid_coarse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/grid_fine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/grid_none.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/ic_help_24px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/ic_pause_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/ic_play_arrow_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/ic_stop_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/ic_volume_up_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/ic_volume_up_48px_90.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/lock-locked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/lock-unlocked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/magnifying-glass.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/map-marker.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/move.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/quantize.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/sort-ascending.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/dark/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/fft.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.059939 pyfda-0.8.0a2/pyfda/images/icons/light/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/light/ic_pause_48px_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/light/ic_play_arrow_48px_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/plot_style-line-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/plot_style-line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/plot_style-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/plot_style-none.png
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/plot_style-stem-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/plot_style-stem.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/plot_style-steps-mkr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/plot_style-steps.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_nobg.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.059939 pyfda-0.8.0a2/pyfda/images/unused/
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/appbar.base.select_grey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/appbar.list.add.above_grey.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.063939 pyfda-0.8.0a2/pyfda/images/unused/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/audio_90.odg
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/audio_90.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/audio_90.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/ic_fiber_manual_record_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/ic_forward_10_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/ic_mic_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/ic_skip_next_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/media-pause-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/media-play-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/media-record-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/media-skip-backward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/media-skip-forward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/media-step-backward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/media-step-forward-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/audio/media-stop-4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/camera-slr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/graph_90.odg
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/graph_90.png
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/grid-four-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/grid-three-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/grid-two-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/ic_volume_mute_48px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/question-mark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/square_outlined.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/table_chart_outlined.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/images/unused/table_outlined.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.063939 pyfda-0.8.0a2/pyfda/input_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/amplitude_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/freq_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21020 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/freq_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44265 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/input_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/input_coeffs_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37825 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/input_fixpoint_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/input_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/input_info_about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36469 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/input_pz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/input_pz_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/input_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/input_tab_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/select_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/target_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/input_widgets/weight_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.067939 pyfda-0.8.0a2/pyfda/libs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/csv_option_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/frozendict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/pyfda_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/pyfda_fft_windows_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44490 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/pyfda_fix_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62234 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/pyfda_io_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59886 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/pyfda_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/pyfda_log_template.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    27531 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/pyfda_qt_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28819 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/pyfda_sig_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/pyfda_template.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    30964 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/libs/tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/license_info.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/module_versions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.067939 pyfda-0.8.0a2/pyfda/plot_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36450 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/mpl_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29100 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/plot_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27085 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/plot_fft_win.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35131 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/plot_hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92610 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/plot_impz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35609 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/plot_impz_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/plot_phi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/plot_pz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/plot_tab_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/plot_tau_g.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.067939 pyfda-0.8.0a2/pyfda/plot_widgets/tran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/tran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25296 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/tran/plot_tran_stim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48691 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/tran/plot_tran_stim_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/tran/tran_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/plot_widgets/tran/tran_io_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/pyfda.qrc
+-rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/pyfda_rc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/pyfdax.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129275 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/qrc_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.067939 pyfda-0.8.0a2/pyfda/widget_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/widget_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.071939 pyfda-0.8.0a2/pyfda/widget_templates/filter_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/widget_templates/filter_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/widget_templates/filter_widgets/my_filter_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.071939 pyfda-0.8.0a2/pyfda/widget_templates/fixpoint_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/widget_templates/fixpoint_widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.071939 pyfda-0.8.0a2/pyfda/widget_templates/input_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/widget_templates/input_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/widget_templates/input_widgets/my_input_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.071939 pyfda-0.8.0a2/pyfda/widget_templates/plot_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/widget_templates/plot_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfda/widget_templates/plot_widgets/myplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:31:45.051940 pyfda-0.8.0a2/pyfda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-08-07 09:31:45.000000 pyfda-0.8.0a2/pyfda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-08-07 09:31:45.000000 pyfda-0.8.0a2/pyfda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:31:45.000000 pyfda-0.8.0a2/pyfda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-07 09:31:45.000000 pyfda-0.8.0a2/pyfda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 09:31:45.000000 pyfda-0.8.0a2/pyfda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-07 09:31:45.000000 pyfda-0.8.0a2/pyfda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/pyfdax.spec
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:31:45.071939 pyfda-0.8.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-08-07 09:31:30.000000 pyfda-0.8.0a2/setup.py
```

### Comparing `pyfda-0.7.1/AUTHORS.md` & `pyfda-0.8.0a2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/CHANGELOG.md` & `pyfda-0.8.0a2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
-## [v0.7.1](https://github.com/chipmuenk/pyfda/tree/v0.7.0) (2022-10-xx)
+## [v0.7.2](https://github.com/chipmuenk/pyfda/tree/v0.7.2) (2023-02-xx)
+### Bugfixes
+- Various crashes related to file imports
+
+### New features
+- Allow plotting magnitude, real and imaginary part of H(F) at the same time
+- Add legend for H(F) plot
+- Show interpolated waveform x(t) for discrete time stimuli (mainly for didactic
+  purposes)
+- Make UI for y[n] cleaner
+- Allow hiding the control options for maximum plotting area via a new button in the toolbar
+
+## [v0.7.1](https://github.com/chipmuenk/pyfda/tree/v0.7.1) (2022-10-05)
 ### Bugfixes
 - Fix crash in 'y[n]' tab when no file is loaded
 - Remove some superfluous files in pip package
 
 ## [v0.7](https://github.com/chipmuenk/pyfda/tree/v0.7.0) (2022-10-04)
 
 ### Bugfixes
```

### Comparing `pyfda-0.7.1/INSTALLATION.md` & `pyfda-0.8.0a2/INSTALLATION.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/LICENSE.md` & `pyfda-0.8.0a2/LICENSE.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ### MIT License
 
 
-**Copyright (c) 2013 - 2021** pyFDA Development Team and others (see AUTHORS.md)
+**Copyright (c) 2013 - 2023** pyFDA Development Team and others (see AUTHORS.md)
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the
```

### Comparing `pyfda-0.7.1/LICENSE_GPLv3.md` & `pyfda-0.8.0a2/LICENSE_GPLv3.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/MANIFEST.in` & `pyfda-0.8.0a2/MANIFEST.in`

 * *Files 25% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 
 include requirements.txt
 include pyfdax.spec
 include pyfda/*.qrc
 
 # exclude byte-code files
 global-exclude *.py[cod]
-exclude bak
-exclude tests
-exclude docs
-exclude recipe
+prune bak
+prune pyfda/tests
+prune docs
+prune recipe
```

### Comparing `pyfda-0.7.1/PKG-INFO` & `pyfda-0.8.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfda
-Version: 0.7.1
+Version: 0.8.0a2
 Summary: Design and analyse discrete time DSP filters with a user-friendly GUI tool. Fixpoint filters in time and frequency domain, too.
 Home-page: https://github.com/chipmuenk/pyFDA
 Author: Christian Muenker
 Author-email: mail07@chipmuenk.de
 License: MIT
 Keywords: digital,discrete time,filter design,IIR,FIR,GUI
 Platform: any
```

### Comparing `pyfda-0.7.1/README.md` & `pyfda-0.8.0a2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 pyfda
 ======
 ## Python Filter Design Analysis Tool
 
 [![PyPI version](https://badge.fury.io/py/pyfda.svg)](https://badge.fury.io/py/pyfda)
 [![Downloads/mo.](https://pepy.tech/badge/pyfda/month)](https://pepy.tech/project/pyfda)
-[![Join the chat at https://gitter.im/chipmuenk/pyFDA](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/chipmuenk/pyFDA?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+![Total Github Downloads](https://img.shields.io/github/downloads/chipmuenk/pyfda/total?label=Total%20Github%20Downloads)<!-- [![Join the chat at https://gitter.im/chipmuenk/pyFDA](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/chipmuenk/pyFDA?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) -->
 [![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
 [![ReadTheDocs](https://readthedocs.org/projects/pyfda/badge/?version=latest)](https://readthedocs.org/projects/pyfda/?badge=latest)
 [![build_pyinstaller](https://github.com/chipmuenk/pyfda/actions/workflows/build_pyinstaller.yml/badge.svg)](https://github.com/chipmuenk/pyfda/actions/workflows/build_pyinstaller.yml)
+[![build_flatpak](https://github.com/chipmuenk/pyfda/actions/workflows/build_flatpak.yml/badge.svg)](https://github.com/chipmuenk/pyfda/actions/workflows/build_flatpak.yml)
 
-**pyfda** is tool written in Python / Qt for analysing and designing discrete time filters with a user-friendly GUI. Fixpoint filter implementations (for some filter types) can be simulated and tested for overflow and quantization behaviour in the time and frequency domain.
+**pyfda** is a tool written in Python / Qt for analyzing and designing discrete time filters with a user-friendly GUI. Fixpoint filter implementations (for some filter types) can be simulated and tested for overflow and quantization behaviour in the time and frequency domain.
 
 ![Screenshot](img/pyfda_screenshot_3.png)
 
 <table>
     <tr>
         <td><img src = "img/pyfda_screenshot_3d_4.png" alt="Screenshot" width=300px></td>
         <td><img src = "img/pyfda_screenshot_hn.png" alt="Screenshot" width=300px></td>
@@ -31,20 +32,18 @@
   <tr>
 </table>
 
 ## License
 pyfda source code ist distributed under a permissive MIT license, binaries / bundles come with a GPLv3 license due to bundled components with stricter licenses.
 
 ## Binaries / Bundles
-Currently, binaries (created with **[pyInstaller](https://www.pyinstaller.org/))** are provided for 64 bit Win 7 ... 10 and for 64 bit Ubuntu (created with 2020.04). The binaries may or may not work with other systems, too. The binaries don't modify the system (except for two ASCII configuration files and a log file), they self-extract to a temporary directory that is automatically deleted when pyfda is terminated (except when it crashes). No additionaly software / libraries need to be installed. For details, see [INSTALLATION.md](INSTALLATION.md).
+Currently, binaries (created with **[pyInstaller](https://www.pyinstaller.org/))** are provided for 64 bit Windows and for OS X. The binaries don't modify the system (except for two ASCII configuration files and a log file), they self-extract to a temporary directory that is automatically deleted when pyfda is terminated (except when it crashes). No additionaly software / libraries need to be installed. For details, see [INSTALLATION.md](INSTALLATION.md).
 
 A flatpak (Linux only) for pyfda is available on **[Flathub](https://flathub.org/apps/details/com.github.chipmuenk.pyfda)**. Some Linux distros have built-in flatpak support, for others it's easy to install with e.g. `sudo apt install flatpak`. For details check the [Flatpak](https://www.flatpak.org/) home page.
 
-Help needed for generation of a MacOS binary! 
-
 ## Prerequisites
 
 * Python versions: **3.7 ... 3.10**
 * All operating systems - there should be no OS specific requirements.
 ### Libraries ###
 The following libraries are required and automatically installed by pip when missing.
 * [**PyQt**](https://www.riverbankcomputing.com/software/pyqt/) and [**Qt5**](https://qt.io/)
```

#### html2text {}

```diff
@@ -1,62 +1,61 @@
 pyfda ====== ## Python Filter Design Analysis Tool [![PyPI version](https://
 badge.fury.io/py/pyfda.svg)](https://badge.fury.io/py/pyfda) [![Downloads/mo.]
-(https://pepy.tech/badge/pyfda/month)](https://pepy.tech/project/pyfda) [![Join
-the chat at https://gitter.im/chipmuenk/pyFDA](https://badges.gitter.im/
-Join%20Chat.svg)](https://gitter.im/chipmuenk/
-pyFDA?utm_source=badge&utm_medium=badge&utm_campaign=pr-
-badge&utm_content=badge) [![MIT licensed](https://img.shields.io/badge/license-
-MIT-blue.svg)](./LICENSE) [![ReadTheDocs](https://readthedocs.org/projects/
-pyfda/badge/?version=latest)](https://readthedocs.org/projects/pyfda/
-?badge=latest) [![build_pyinstaller](https://github.com/chipmuenk/pyfda/
-actions/workflows/build_pyinstaller.yml/badge.svg)](https://github.com/
-chipmuenk/pyfda/actions/workflows/build_pyinstaller.yml) **pyfda** is tool
-written in Python / Qt for analysing and designing discrete time filters with a
-user-friendly GUI. Fixpoint filter implementations (for some filter types) can
-be simulated and tested for overflow and quantization behaviour in the time and
-frequency domain. ![Screenshot](img/pyfda_screenshot_3.png)
+(https://pepy.tech/badge/pyfda/month)](https://pepy.tech/project/pyfda) ![Total
+Github Downloads](https://img.shields.io/github/downloads/chipmuenk/pyfda/
+total?label=Total%20Github%20Downloads) [![MIT licensed](https://
+img.shields.io/badge/license-MIT-blue.svg)](./LICENSE) [![ReadTheDocs](https://
+readthedocs.org/projects/pyfda/badge/?version=latest)](https://readthedocs.org/
+projects/pyfda/?badge=latest) [![build_pyinstaller](https://github.com/
+chipmuenk/pyfda/actions/workflows/build_pyinstaller.yml/badge.svg)](https://
+github.com/chipmuenk/pyfda/actions/workflows/build_pyinstaller.yml) [!
+[build_flatpak](https://github.com/chipmuenk/pyfda/actions/workflows/
+build_flatpak.yml/badge.svg)](https://github.com/chipmuenk/pyfda/actions/
+workflows/build_flatpak.yml) **pyfda** is a tool written in Python / Qt for
+analyzing and designing discrete time filters with a user-friendly GUI.
+Fixpoint filter implementations (for some filter types) can be simulated and
+tested for overflow and quantization behaviour in the time and frequency
+domain. ![Screenshot](img/pyfda_screenshot_3.png)
 [Screenshot] [Screenshot] [Screenshot]
 [Screenshot] [Screenshot] [Screenshot]
 [Screenshot] [Screenshot] [Screenshot]
 ## License pyfda source code ist distributed under a permissive MIT license,
 binaries / bundles come with a GPLv3 license due to bundled components with
 stricter licenses. ## Binaries / Bundles Currently, binaries (created with **
-[pyInstaller](https://www.pyinstaller.org/))** are provided for 64 bit Win 7
-... 10 and for 64 bit Ubuntu (created with 2020.04). The binaries may or may
-not work with other systems, too. The binaries don't modify the system (except
-for two ASCII configuration files and a log file), they self-extract to a
-temporary directory that is automatically deleted when pyfda is terminated
-(except when it crashes). No additionaly software / libraries need to be
-installed. For details, see [INSTALLATION.md](INSTALLATION.md). A flatpak
-(Linux only) for pyfda is available on **[Flathub](https://flathub.org/apps/
-details/com.github.chipmuenk.pyfda)**. Some Linux distros have built-in flatpak
+[pyInstaller](https://www.pyinstaller.org/))** are provided for 64 bit Windows
+and for OS X. The binaries don't modify the system (except for two ASCII
+configuration files and a log file), they self-extract to a temporary directory
+that is automatically deleted when pyfda is terminated (except when it
+crashes). No additionaly software / libraries need to be installed. For
+details, see [INSTALLATION.md](INSTALLATION.md). A flatpak (Linux only) for
+pyfda is available on **[Flathub](https://flathub.org/apps/details/
+com.github.chipmuenk.pyfda)**. Some Linux distros have built-in flatpak
 support, for others it's easy to install with e.g. `sudo apt install flatpak`.
-For details check the [Flatpak](https://www.flatpak.org/) home page. Help
-needed for generation of a MacOS binary! ## Prerequisites * Python versions:
-**3.7 ... 3.10** * All operating systems - there should be no OS specific
-requirements. ### Libraries ### The following libraries are required and
-automatically installed by pip when missing. * [**PyQt**](https://
-www.riverbankcomputing.com/software/pyqt/) and [**Qt5**](https://qt.io/) *
-[**numpy**](https://numpy.org/) * [**numexpr**](https://github.com/pydata/
-numexpr) * [**scipy**](https://scipy.org/): **1.2.0** or higher *
-[**matplotlib**](https://matplotlib.org/): **3.1** or higher * [**Markdown**]
-(https://github.com/Python-Markdown/markdown) ### Optional libraries: *
-[**mplcursors**](https://mplcursors.readthedocs.io/) for annotating cursors *
-[**docutils**](https://docutils.sourceforge.io) for rich text in documentation
-* **xlwt** and / or **XlsxWriter** for exporting filter coefficients as *.xls
-(x) files ## Installing pyfda Unless running a binary, you need to have a
-working Python installation on your computer, preferrably including the
-libraries listed above. There is only one version of pyfda for all supported
-operating systems, Python and Qt versions. As pyfda is a pure Python project
-(no binaries, no compilation required), you can install pyfda using one of the
-following options: ### pip Installation from PyPI works the usual way, required
-libraries are installed automatically if missing: > pip3 install pyfda Upgrade
-using > pip3 install pyfda -U If you have cloned `pyfda` to your local drive
-you can install the local copy (i.e. create local config files and the `pyfdax`
-starter script) via > pip3 install -e
+For details check the [Flatpak](https://www.flatpak.org/) home page. ##
+Prerequisites * Python versions: **3.7 ... 3.10** * All operating systems -
+there should be no OS specific requirements. ### Libraries ### The following
+libraries are required and automatically installed by pip when missing. *
+[**PyQt**](https://www.riverbankcomputing.com/software/pyqt/) and [**Qt5**]
+(https://qt.io/) * [**numpy**](https://numpy.org/) * [**numexpr**](https://
+github.com/pydata/numexpr) * [**scipy**](https://scipy.org/): **1.2.0** or
+higher * [**matplotlib**](https://matplotlib.org/): **3.1** or higher *
+[**Markdown**](https://github.com/Python-Markdown/markdown) ### Optional
+libraries: * [**mplcursors**](https://mplcursors.readthedocs.io/) for
+annotating cursors * [**docutils**](https://docutils.sourceforge.io) for rich
+text in documentation * **xlwt** and / or **XlsxWriter** for exporting filter
+coefficients as *.xls(x) files ## Installing pyfda Unless running a binary, you
+need to have a working Python installation on your computer, preferrably
+including the libraries listed above. There is only one version of pyfda for
+all supported operating systems, Python and Qt versions. As pyfda is a pure
+Python project (no binaries, no compilation required), you can install pyfda
+using one of the following options: ### pip Installation from PyPI works the
+usual way, required libraries are installed automatically if missing: > pip3
+install pyfda Upgrade using > pip3 install pyfda -U If you have cloned `pyfda`
+to your local drive you can install the local copy (i.e. create local config
+files and the `pyfdax` starter script) via > pip3 install -e
 py> For more details and options see [INSTALLATION.md](INSTALLATION.md). ###
 setup.py You can also download the zip file and extract it to a temp directory
 of your choice. Install it either to your `/Lib/site-packages` subdirectory
 (this creates a copy) using > python setup.py install or just create a link to
 where you have copied the python source files (for testing / development) using
 > python setup.py develop ### git For development purposes, you should fork the
 latest version of pyfda from https://github.com/chipmuenk/pyfda.git and create
```

### Comparing `pyfda-0.7.1/README_PYPI.md` & `pyfda-0.8.0a2/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_factory.py` & `pyfda-0.8.0a2/pyfda/filter_factory.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/bessel.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/bessel.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/butter.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/butter.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/cheby1.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/cheby1.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/cheby2.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/cheby2.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/common.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/common.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/delay.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/delay.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/ellip.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/ellip.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/ellip_zero.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/ellip_zero.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/equiripple.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/equiripple.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/firwin.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/firwin.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,31 +70,31 @@
 
     def __init__(self):
         QWidget.__init__(self)
 
         self.ft = 'FIR'
 
         win_names_list = ["Boxcar", "Rectangular", "Barthann", "Bartlett", "Blackman",
-                          "Blackmanharris", "Bohman", "Cosine", "Dolph-Chebyshev",
+                          "Blackmanharris", "Bohman", "Cosine", "Dolph-Chebyshev", "DPSS",
                           "Flattop", "General Gaussian", "Gauss", "Hamming", "Hann",
-                          "Kaiser", "Nuttall", "Parzen", "Slepian", "Triangular", "Tukey"]
+                          "Kaiser", "Nuttall", "Parzen", "Triangular", "Tukey"]
         self.cur_win_name = "Kaiser"  # set initial window type
         self.alg = "ichige"
 
         # initialize windows dict with the list above for firwin window settings
         self.win_dict = get_windows_dict(
             win_names_list=win_names_list,
             cur_win_name=self.cur_win_name)
 
         # get initial / last setting from dictionary, updating self.win_dict
         self._load_dict()
 
         # instantiate FFT window with windows dict
         self.fft_widget = Plot_FFT_win(
-            self, win_dict=self.win_dict, sym=True, title="pyFDA FIR Window Viewer")
+            win_dict=self.win_dict, sym=True, title="pyFDA FIR Window Viewer")
         # hide window initially, this is modeless i.e. a non-blocking popup window
         self.fft_widget.hide()
 
         c = Common()
         self.rt_dict = c.rt_base_iir
 
         self.rt_dict_add = {
@@ -171,15 +171,15 @@
         self.cmb_firwin_alg = QComboBox(self)
         self.cmb_firwin_alg.setObjectName('wdg_cmb_firwin_alg')
         self.cmb_firwin_alg.addItems(['ichige', 'kaiser', 'herrmann'])
         # Minimum size, can be changed in the upper hierarchy levels using layouts:
         self.cmb_firwin_alg.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         self.cmb_firwin_alg.hide()
 
-        self.qfft_win_select = QFFTWinSelector(self, self.win_dict)
+        self.qfft_win_select = QFFTWinSelector(self.win_dict)
         # Minimum size, can be changed in the upper hierarchy levels using layouts:
         # self.qfft_win_select.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
         self.but_fft_wdg = QPushButton(self)
         self.but_fft_wdg.setIcon(QIcon(":/fft.svg"))
         but_height = self.qfft_win_select.sizeHint().height()
         self.but_fft_wdg.setIconSize(QSize(but_height, but_height))
```

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/ma.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/ma.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
                       QVBoxLayout, QHBoxLayout)
 
 import numpy as np
 
 import pyfda.filterbroker as fb
 from pyfda.libs.pyfda_lib import fil_save, fil_convert, ceil_odd, safe_eval
 from pyfda.libs.pyfda_qt_lib import qfilter_warning
+from pyfda.libs.pyfda_sig_lib import zeros_with_val
 
 __version__ = "2.2"
 
 classes = {'MA':'Moving Average'} #: Dict containing class name : display name
 
 class MA(QWidget):
 
@@ -342,16 +343,18 @@
 
         # normalize filter to |H_max| = 1 if checked:
         if self.chk_norm.isChecked():
             b = b / (norm ** self.stages)
             k = 1./norm ** self.stages
         p = np.zeros(len(z))
 
+        gain = zeros_with_val(len(z), k)
+
         # store in class attributes for the _save method
-        self.zpk = [z,p,k]
+        self.zpk = [z,p,gain]
         self.b = b
         self._save(fil_dict)
 
 
     def LPman(self, fil_dict):
         self._get_params(fil_dict)
         self.calc_ma(fil_dict, rt = 'LP')
```

### Comparing `pyfda-0.7.1/pyfda/filter_widgets/manual.py` & `pyfda-0.8.0a2/pyfda/filter_widgets/manual.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/filterbroker.py` & `pyfda-0.8.0a2/pyfda/filterbroker.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,24 +215,24 @@
                           }
                 }
         }
     })
 
 # -----------------------------------------------------------------------------
 # Dictionary containing current filter type, specifications, design and some
-# auxiliary information, the initial definition here is overwritten by
-# input widgets and design routines:
+# auxiliary information, the initial definition here is copied into fil[0]
+# and can be overwritten by input widgets and design routines
 # ------------------------------------------------------------------------------
 fil_init = {'rt': 'LP', 'ft': 'IIR', 'fc': 'Cheby1', 'fo': 'man',  # filter type
             'N': 10,  # filter order
             'f_S': 1, 'T_S': 1,  # current sampling frequency and period
-            'f_S_wav': 16000,  # sampling frequency for wav files
+            # 'f_s_wav': 16000,  # sampling frequency for wav files
             'f_S_prev': 1,  # previous sampling frequency
             'freq_locked': False,  # don't update absolute frequencies when f_S is changed
-            'f_S_scale': 1,  #
+            'f_s_scale': 1,  #
             'f_max': 1,
             'freqSpecsRangeType': 'Half',
             'freqSpecsRange': [0, 0.5],
             'freq_specs_sort': True,  # sort freq. specs in ascending order
             'freq_specs_unit': 'f_S',
             'plt_fLabel': r'$F = 2f \, / \, f_S = \Omega \, / \, \mathrm{\pi} \; \rightarrow$',
             'plt_fUnit': 'f_S',
@@ -240,16 +240,17 @@
             'plt_tUnit': 's',
             'A_PB': 0.02, 'A_PB2': 0.01, 'F_PB': 0.1, 'F_PB2': 0.4, 'F_C': 0.2, 'F_N': 0.2,
             'A_SB': 0.001, 'A_SB2': 0.0001, 'F_SB': 0.2, 'F_SB2': 0.3, 'F_C2': 0.4, 'F_N2': 0.4,
             'W_PB': 1, 'W_PB2': 1, 'W_SB': 1, 'W_SB2': 1,
             #
             'ba': ([1, 1, 1], [1, 0.1, 0.5]),  # (bb, aa) tuple coefficient lists
             # causal zeros/poles/gain
-            'zpk': ([-0.5 + 3**0.5/2.j, -0.5 - 3**0.5/2.j],
-                   [(2./3)**0.5 * 1j, -(2./3)**0.5 * 1j], 1),
+            'zpk': [[-0.5 + 3**0.5/2.j, -0.5 - 3**0.5/2.j],
+                   [(2./3)**0.5 * 1j, -(2./3)**0.5 * 1j],
+                   [1, 0]],
             #
             'sos': [],
             # input, output, accu, coeffs, ... fixpoint word formats and quantizer
             # settings:
             'fxqc':
                 {'QI': {'WI': 0, 'WF': 15, 'W': 16, 'ovfl': 'sat',  'quant': 'round'},
                  'QO': {'WI': 0, 'WF': 15, 'W': 16, 'ovfl': 'wrap', 'quant': 'floor'},
```

### Comparing `pyfda-0.7.1/pyfda/fixpoint_widgets/default_fx_img.png` & `pyfda-0.8.0a2/pyfda/fixpoint_widgets/default_fx_img.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/fixpoint_widgets/fir_df/fir_df.png` & `pyfda-0.8.0a2/pyfda/fixpoint_widgets/fir_df/fir_df.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py` & `pyfda-0.8.0a2/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py` & `pyfda-0.8.0a2/pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/fixpoint_widgets/fx_ui_wq.py` & `pyfda-0.8.0a2/pyfda/fixpoint_widgets/fx_ui_wq.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         self.ledWF.setToolTip(dict_ui['tip_WF'])
         self.ledWF.setMaxLength(dict_ui['WI_len'])  # maximum of 2 digits
         self.ledWF.setFixedWidth(dict_ui['max_led_width'])  # width of lineedit in points
         self.ledWF.setVisible(dict_ui['fractional'])
         self.ledWF.setObjectName("WF")
 
         self.count_ovfl_vis = dict_ui['count_ovfl_vis']
-        self.lbl_ovfl_count = QLabel(to_html("N_ov = 0", frmt='i'))
+        self.lbl_ovfl_count = QLabel(to_html("N_ov = 0"))
         self.lbl_ovfl_count.setAutoFillBackground(True)
 
         self.MSB_LSB_vis = dict_ui['MSB_LSB_vis']
 
         # -------------------------------------------------------------------
         # MSB / LSB size
         # ---------------------------------------------------------------------
@@ -363,15 +363,15 @@
         elif self.count_ovfl_vis == 'auto' and self.q_dict['N_over'] == 0:
             self.lbl_ovfl_count.setVisible(False)
         elif self.count_ovfl_vis == 'on' or\
                 self.count_ovfl_vis == 'auto' and self.q_dict['N_over'] > 0:
 
             self.lbl_ovfl_count.setVisible(True)
             self.lbl_ovfl_count.setText(
-                to_html(f"<b><i>&nbsp;&nbsp;N</i>_ov = </b>{self.q_dict['N_over']}"))
+                to_html(f"<b><i>&nbsp;&nbsp;N_ov </i>= {self.q_dict['N_over']}</b>"))
             if self.q_dict['N_over'] == 0:
                 qstyle_widget(self.lbl_ovfl_count, "normal")
             else:
                 qstyle_widget(self.lbl_ovfl_count, "failed")
         else:
             logger.error(f"Unknown option count_ovfl_vis = '{self.count_ovfl_vis}'")
         return
```

### Comparing `pyfda-0.7.1/pyfda/fixpoint_widgets/iir_df1/iir_df1.png` & `pyfda-0.8.0a2/pyfda/fixpoint_widgets/iir_df1/iir_df1.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py` & `pyfda-0.8.0a2/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py` & `pyfda-0.8.0a2/pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/fixpoint_widgets/no_fx_filter.png` & `pyfda-0.8.0a2/pyfda/fixpoint_widgets/no_fx_filter.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/appbar.from_clipboard.svg` & `pyfda-0.8.0a2/pyfda/images/icons/dark/appbar.from_clipboard.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/appbar.list.add.above.svg` & `pyfda-0.8.0a2/pyfda/images/icons/dark/appbar.list.add.above.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/appbar.list.delete.svg` & `pyfda-0.8.0a2/pyfda/images/icons/dark/appbar.list.delete.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/appbar.to_clipboard.svg` & `pyfda-0.8.0a2/pyfda/images/icons/dark/appbar.to_clipboard.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/audio_90.odg` & `pyfda-0.8.0a2/pyfda/images/unused/audio/audio_90.odg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/cog.svg` & `pyfda-0.8.0a2/pyfda/images/icons/dark/cog.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/graph_90.odg` & `pyfda-0.8.0a2/pyfda/images/unused/graph_90.odg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/graph_90.png` & `pyfda-0.8.0a2/pyfda/images/unused/graph_90.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/ic_forward_10_48px.svg` & `pyfda-0.8.0a2/pyfda/images/unused/audio/ic_forward_10_48px.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/dark/quantize.svg` & `pyfda-0.8.0a2/pyfda/images/icons/dark/quantize.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/fft.svg` & `pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_nobg.svg`

 * *Files 27% similar despite different names*

```diff
@@ -1,432 +1,449 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0a3c 7376 670a 2020 2078  "no"?>.<svg.   x
-00000040: 6d6c 6e73 3a6f 6f6f 3d22 6874 7470 3a2f  mlns:ooo="http:/
-00000050: 2f78 6d6c 2e6f 7065 6e6f 6666 6963 652e  /xml.openoffice.
-00000060: 6f72 672f 7376 672f 6578 706f 7274 220a  org/svg/export".
-00000070: 2020 2078 6d6c 6e73 3a64 633d 2268 7474     xmlns:dc="htt
-00000080: 703a 2f2f 7075 726c 2e6f 7267 2f64 632f  p://purl.org/dc/
-00000090: 656c 656d 656e 7473 2f31 2e31 2f22 0a20  elements/1.1/". 
-000000a0: 2020 786d 6c6e 733a 6363 3d22 6874 7470    xmlns:cc="http
-000000b0: 3a2f 2f63 7265 6174 6976 6563 6f6d 6d6f  ://creativecommo
-000000c0: 6e73 2e6f 7267 2f6e 7323 220a 2020 2078  ns.org/ns#".   x
-000000d0: 6d6c 6e73 3a72 6466 3d22 6874 7470 3a2f  mlns:rdf="http:/
-000000e0: 2f77 7777 2e77 332e 6f72 672f 3139 3939  /www.w3.org/1999
-000000f0: 2f30 322f 3232 2d72 6466 2d73 796e 7461  /02/22-rdf-synta
-00000100: 782d 6e73 2322 0a20 2020 786d 6c6e 733a  x-ns#".   xmlns:
-00000110: 7376 673d 2268 7474 703a 2f2f 7777 772e  svg="http://www.
-00000120: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
-00000130: 0a20 2020 786d 6c6e 733d 2268 7474 703a  .   xmlns="http:
-00000140: 2f2f 7777 772e 7733 2e6f 7267 2f32 3030  //www.w3.org/200
-00000150: 302f 7376 6722 0a20 2020 786d 6c6e 733a  0/svg".   xmlns:
-00000160: 736f 6469 706f 6469 3d22 6874 7470 3a2f  sodipodi="http:/
-00000170: 2f73 6f64 6970 6f64 692e 736f 7572 6365  /sodipodi.source
-00000180: 666f 7267 652e 6e65 742f 4454 442f 736f  forge.net/DTD/so
-00000190: 6469 706f 6469 2d30 2e64 7464 220a 2020  dipodi-0.dtd".  
-000001a0: 2078 6d6c 6e73 3a69 6e6b 7363 6170 653d   xmlns:inkscape=
-000001b0: 2268 7474 703a 2f2f 7777 772e 696e 6b73  "http://www.inks
-000001c0: 6361 7065 2e6f 7267 2f6e 616d 6573 7061  cape.org/namespa
-000001d0: 6365 732f 696e 6b73 6361 7065 220a 2020  ces/inkscape".  
-000001e0: 2076 6572 7369 6f6e 3d22 312e 3222 0a20   version="1.2". 
-000001f0: 2020 7769 6474 683d 2238 2e34 376d 6d22    width="8.47mm"
-00000200: 0a20 2020 6865 6967 6874 3d22 382e 3437  .   height="8.47
-00000210: 6d6d 220a 2020 2076 6965 7742 6f78 3d22  mm".   viewBox="
-00000220: 3020 3020 3834 3720 3834 3722 0a20 2020  0 0 847 847".   
-00000230: 7072 6573 6572 7665 4173 7065 6374 5261  preserveAspectRa
-00000240: 7469 6f3d 2278 4d69 6459 4d69 6422 0a20  tio="xMidYMid". 
-00000250: 2020 6669 6c6c 2d72 756c 653d 2265 7665    fill-rule="eve
-00000260: 6e6f 6464 220a 2020 2073 7472 6f6b 652d  nodd".   stroke-
-00000270: 7769 6474 683d 2232 382e 3232 3222 0a20  width="28.222". 
-00000280: 2020 7374 726f 6b65 2d6c 696e 656a 6f69    stroke-linejoi
-00000290: 6e3d 2272 6f75 6e64 220a 2020 2078 6d6c  n="round".   xml
-000002a0: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-000002b0: 220a 2020 2069 643d 2273 7667 3934 220a  ".   id="svg94".
-000002c0: 2020 2073 6f64 6970 6f64 693a 646f 636e     sodipodi:docn
-000002d0: 616d 653d 2266 6674 5f32 2e73 7667 220a  ame="fft_2.svg".
-000002e0: 2020 2069 6e6b 7363 6170 653a 7665 7273     inkscape:vers
-000002f0: 696f 6e3d 2231 2e30 2e31 2028 3362 6332  ion="1.0.1 (3bc2
-00000300: 6538 3133 6635 2c20 3230 3230 2d30 392d  e813f5, 2020-09-
-00000310: 3037 2922 3e3c 6d65 7461 6461 7461 0a20  07)"><metadata. 
-00000320: 2020 6964 3d22 6d65 7461 6461 7461 3938    id="metadata98
-00000330: 223e 3c72 6466 3a52 4446 3e3c 6363 3a57  "><rdf:RDF><cc:W
-00000340: 6f72 6b0a 2020 2020 2020 2072 6466 3a61  ork.       rdf:a
-00000350: 626f 7574 3d22 223e 3c64 633a 666f 726d  bout=""><dc:form
-00000360: 6174 3e69 6d61 6765 2f73 7667 2b78 6d6c  at>image/svg+xml
-00000370: 3c2f 6463 3a66 6f72 6d61 743e 3c64 633a  </dc:format><dc:
-00000380: 7479 7065 0a20 2020 2020 2020 2020 7264  type.         rd
-00000390: 663a 7265 736f 7572 6365 3d22 6874 7470  f:resource="http
-000003a0: 3a2f 2f70 7572 6c2e 6f72 672f 6463 2f64  ://purl.org/dc/d
-000003b0: 636d 6974 7970 652f 5374 696c 6c49 6d61  cmitype/StillIma
-000003c0: 6765 2220 2f3e 3c64 633a 7469 746c 6520  ge" /><dc:title 
-000003d0: 2f3e 3c2f 6363 3a57 6f72 6b3e 3c2f 7264  /></cc:Work></rd
-000003e0: 663a 5244 463e 3c2f 6d65 7461 6461 7461  f:RDF></metadata
-000003f0: 3e3c 736f 6469 706f 6469 3a6e 616d 6564  ><sodipodi:named
-00000400: 7669 6577 0a20 2020 7061 6765 636f 6c6f  view.   pagecolo
-00000410: 723d 2223 6666 6666 6666 220a 2020 2062  r="#ffffff".   b
-00000420: 6f72 6465 7263 6f6c 6f72 3d22 2336 3636  ordercolor="#666
-00000430: 3636 3622 0a20 2020 626f 7264 6572 6f70  666".   borderop
-00000440: 6163 6974 793d 2231 220a 2020 206f 626a  acity="1".   obj
-00000450: 6563 7474 6f6c 6572 616e 6365 3d22 3130  ecttolerance="10
-00000460: 220a 2020 2067 7269 6474 6f6c 6572 616e  ".   gridtoleran
-00000470: 6365 3d22 3130 220a 2020 2067 7569 6465  ce="10".   guide
-00000480: 746f 6c65 7261 6e63 653d 2231 3022 0a20  tolerance="10". 
-00000490: 2020 696e 6b73 6361 7065 3a70 6167 656f    inkscape:pageo
-000004a0: 7061 6369 7479 3d22 3022 0a20 2020 696e  pacity="0".   in
-000004b0: 6b73 6361 7065 3a70 6167 6573 6861 646f  kscape:pageshado
-000004c0: 773d 2232 220a 2020 2069 6e6b 7363 6170  w="2".   inkscap
-000004d0: 653a 7769 6e64 6f77 2d77 6964 7468 3d22  e:window-width="
-000004e0: 3139 3138 220a 2020 2069 6e6b 7363 6170  1918".   inkscap
-000004f0: 653a 7769 6e64 6f77 2d68 6569 6768 743d  e:window-height=
-00000500: 2239 3931 220a 2020 2069 643d 226e 616d  "991".   id="nam
-00000510: 6564 7669 6577 3936 220a 2020 2073 686f  edview96".   sho
-00000520: 7767 7269 643d 2266 616c 7365 220a 2020  wgrid="false".  
-00000530: 2069 6e6b 7363 6170 653a 7a6f 6f6d 3d22   inkscape:zoom="
-00000540: 3235 2e36 3737 3339 220a 2020 2069 6e6b  25.67739".   ink
-00000550: 7363 6170 653a 6378 3d22 342e 3733 3137  scape:cx="4.7317
-00000560: 3839 3622 0a20 2020 696e 6b73 6361 7065  896".   inkscape
-00000570: 3a63 793d 2231 342e 3434 3835 3039 220a  :cy="14.448509".
-00000580: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
-00000590: 6f77 2d78 3d22 3022 0a20 2020 696e 6b73  ow-x="0".   inks
-000005a0: 6361 7065 3a77 696e 646f 772d 793d 2230  cape:window-y="0
-000005b0: 220a 2020 2069 6e6b 7363 6170 653a 7769  ".   inkscape:wi
-000005c0: 6e64 6f77 2d6d 6178 696d 697a 6564 3d22  ndow-maximized="
-000005d0: 3022 0a20 2020 696e 6b73 6361 7065 3a63  0".   inkscape:c
-000005e0: 7572 7265 6e74 2d6c 6179 6572 3d22 7376  urrent-layer="sv
-000005f0: 6739 3422 0a20 2020 696e 6b73 6361 7065  g94".   inkscape
-00000600: 3a64 6f63 756d 656e 742d 726f 7461 7469  :document-rotati
-00000610: 6f6e 3d22 3022 202f 3e0a 203c 6465 6673  on="0" />. <defs
-00000620: 0a20 2020 636c 6173 733d 2243 6c69 7050  .   class="ClipP
-00000630: 6174 6847 726f 7570 220a 2020 2069 643d  athGroup".   id=
-00000640: 2264 6566 7338 223e 0a20 203c 636c 6970  "defs8">.  <clip
-00000650: 5061 7468 0a20 2020 6964 3d22 7072 6573  Path.   id="pres
-00000660: 656e 7461 7469 6f6e 5f63 6c69 705f 7061  entation_clip_pa
-00000670: 7468 220a 2020 2063 6c69 7050 6174 6855  th".   clipPathU
-00000680: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00000690: 6e55 7365 223e 0a20 2020 3c72 6563 740a  nUse">.   <rect.
-000006a0: 2020 2078 3d22 3022 0a20 2020 793d 2230     x="0".   y="0
-000006b0: 220a 2020 2077 6964 7468 3d22 3834 3722  ".   width="847"
-000006c0: 0a20 2020 6865 6967 6874 3d22 3834 3722  .   height="847"
-000006d0: 0a20 2020 6964 3d22 7265 6374 3222 202f  .   id="rect2" /
-000006e0: 3e0a 2020 3c2f 636c 6970 5061 7468 3e0a  >.  </clipPath>.
-000006f0: 2020 3c63 6c69 7050 6174 680a 2020 2069    <clipPath.   i
-00000700: 643d 2270 7265 7365 6e74 6174 696f 6e5f  d="presentation_
-00000710: 636c 6970 5f70 6174 685f 7368 7269 6e6b  clip_path_shrink
-00000720: 220a 2020 2063 6c69 7050 6174 6855 6e69  ".   clipPathUni
-00000730: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
-00000740: 7365 223e 0a20 2020 3c72 6563 740a 2020  se">.   <rect.  
-00000750: 2078 3d22 3022 0a20 2020 793d 2230 220a   x="0".   y="0".
-00000760: 2020 2077 6964 7468 3d22 3834 3622 0a20     width="846". 
-00000770: 2020 6865 6967 6874 3d22 3834 3622 0a20    height="846". 
-00000780: 2020 6964 3d22 7265 6374 3522 202f 3e0a    id="rect5" />.
-00000790: 2020 3c2f 636c 6970 5061 7468 3e0a 200a    </clipPath>. .
-000007a0: 2020 0a20 0a20 2020 0a20 200a 2020 2020    . .   .  .    
-000007b0: 0a20 2020 0a20 2020 2020 0a20 2020 200a  .   .     .    .
-000007c0: 2020 2020 2020 0a20 2020 2020 200a 2020        .      .  
-000007d0: 2020 2020 0a20 2020 2020 3c2f 6465 6673      .     </defs
-000007e0: 3e0a 203c 6465 6673 0a20 2020 636c 6173  >. <defs.   clas
-000007f0: 733d 2254 6578 7453 6861 7065 496e 6465  s="TextShapeInde
-00000800: 7822 0a20 2020 6964 3d22 6465 6673 3132  x".   id="defs12
-00000810: 223e 0a20 203c 670a 2020 206f 6f6f 3a73  ">.  <g.   ooo:s
-00000820: 6c69 6465 3d22 6964 3122 0a20 2020 6f6f  lide="id1".   oo
-00000830: 6f3a 6964 2d6c 6973 743d 2269 6433 2069  o:id-list="id3 i
-00000840: 6434 2069 6435 2069 6436 2069 6437 220a  d4 id5 id6 id7".
-00000850: 2020 2069 643d 2267 3130 2220 2f3e 0a20     id="g10" />. 
-00000860: 3c2f 6465 6673 3e0a 203c 6465 6673 0a20  </defs>. <defs. 
-00000870: 2020 636c 6173 733d 2245 6d62 6564 6465    class="Embedde
-00000880: 6442 756c 6c65 7443 6861 7273 220a 2020  dBulletChars".  
-00000890: 2069 643d 2264 6566 7334 3422 3e0a 2020   id="defs44">.  
-000008a0: 3c67 0a20 2020 6964 3d22 6275 6c6c 6574  <g.   id="bullet
-000008b0: 2d63 6861 722d 7465 6d70 6c61 7465 2d35  -char-template-5
-000008c0: 3733 3536 220a 2020 2074 7261 6e73 666f  7356".   transfo
-000008d0: 726d 3d22 7363 616c 6528 302e 3030 3034  rm="scale(0.0004
-000008e0: 3838 3238 3132 352c 2d30 2e30 3030 3438  8828125,-0.00048
-000008f0: 3832 3831 3235 2922 3e0a 2020 203c 7061  828125)">.   <pa
-00000900: 7468 0a20 2020 643d 224d 2035 3830 2c31  th.   d="M 580,1
-00000910: 3134 3120 4c20 3131 3633 2c35 3731 2035  141 L 1163,571 5
-00000920: 3830 2c30 202d 342c 3537 3120 3538 302c  80,0 -4,571 580,
-00000930: 3131 3431 205a 220a 2020 2069 643d 2270  1141 Z".   id="p
-00000940: 6174 6831 3422 202f 3e0a 2020 3c2f 673e  ath14" />.  </g>
-00000950: 0a20 203c 670a 2020 2069 643d 2262 756c  .  <g.   id="bul
-00000960: 6c65 742d 6368 6172 2d74 656d 706c 6174  let-char-templat
-00000970: 652d 3537 3335 3422 0a20 2020 7472 616e  e-57354".   tran
-00000980: 7366 6f72 6d3d 2273 6361 6c65 2830 2e30  sform="scale(0.0
-00000990: 3030 3438 3832 3831 3235 2c2d 302e 3030  0048828125,-0.00
-000009a0: 3034 3838 3238 3132 3529 223e 0a20 2020  048828125)">.   
-000009b0: 3c70 6174 680a 2020 2064 3d22 4d20 382c  <path.   d="M 8,
-000009c0: 3131 3238 204c 2031 3133 372c 3131 3238  1128 L 1137,1128
-000009d0: 2031 3133 372c 3020 382c 3020 382c 3131   1137,0 8,0 8,11
-000009e0: 3238 205a 220a 2020 2069 643d 2270 6174  28 Z".   id="pat
-000009f0: 6831 3722 202f 3e0a 2020 3c2f 673e 0a20  h17" />.  </g>. 
-00000a00: 203c 670a 2020 2069 643d 2262 756c 6c65   <g.   id="bulle
-00000a10: 742d 6368 6172 2d74 656d 706c 6174 652d  t-char-template-
-00000a20: 3130 3134 3622 0a20 2020 7472 616e 7366  10146".   transf
-00000a30: 6f72 6d3d 2273 6361 6c65 2830 2e30 3030  orm="scale(0.000
-00000a40: 3438 3832 3831 3235 2c2d 302e 3030 3034  48828125,-0.0004
-00000a50: 3838 3238 3132 3529 223e 0a20 2020 3c70  8828125)">.   <p
-00000a60: 6174 680a 2020 2064 3d22 4d20 3137 342c  ath.   d="M 174,
-00000a70: 3020 4c20 3630 322c 3733 3920 3137 342c  0 L 602,739 174,
-00000a80: 3134 3831 2031 3435 362c 3733 3920 3137  1481 1456,739 17
-00000a90: 342c 3020 5a20 4d20 3133 3538 2c37 3339  4,0 Z M 1358,739
-00000aa0: 204c 2033 3039 2c31 3334 3620 3635 392c   L 309,1346 659,
-00000ab0: 3733 3920 3133 3538 2c37 3339 205a 220a  739 1358,739 Z".
-00000ac0: 2020 2069 643d 2270 6174 6832 3022 202f     id="path20" /
-00000ad0: 3e0a 2020 3c2f 673e 0a20 203c 670a 2020  >.  </g>.  <g.  
-00000ae0: 2069 643d 2262 756c 6c65 742d 6368 6172   id="bullet-char
-00000af0: 2d74 656d 706c 6174 652d 3130 3133 3222  -template-10132"
-00000b00: 0a20 2020 7472 616e 7366 6f72 6d3d 2273  .   transform="s
-00000b10: 6361 6c65 2830 2e30 3030 3438 3832 3831  cale(0.000488281
-00000b20: 3235 2c2d 302e 3030 3034 3838 3238 3132  25,-0.0004882812
-00000b30: 3529 223e 0a20 2020 3c70 6174 680a 2020  5)">.   <path.  
-00000b40: 2064 3d22 4d20 3230 3135 2c37 3339 204c   d="M 2015,739 L
-00000b50: 2031 3237 362c 3020 3731 372c 3020 3132   1276,0 717,0 12
-00000b60: 3630 2c35 3433 2031 3734 2c35 3433 2031  60,543 174,543 1
-00000b70: 3734 2c39 3336 2031 3236 302c 3933 3620  74,936 1260,936 
-00000b80: 3731 372c 3134 3831 2031 3237 342c 3134  717,1481 1274,14
-00000b90: 3831 2032 3031 352c 3733 3920 5a22 0a20  81 2015,739 Z". 
-00000ba0: 2020 6964 3d22 7061 7468 3233 2220 2f3e    id="path23" />
-00000bb0: 0a20 203c 2f67 3e0a 2020 3c67 0a20 2020  .  </g>.  <g.   
-00000bc0: 6964 3d22 6275 6c6c 6574 2d63 6861 722d  id="bullet-char-
-00000bd0: 7465 6d70 6c61 7465 2d31 3030 3037 220a  template-10007".
-00000be0: 2020 2074 7261 6e73 666f 726d 3d22 7363     transform="sc
-00000bf0: 616c 6528 302e 3030 3034 3838 3238 3132  ale(0.0004882812
-00000c00: 352c 2d30 2e30 3030 3438 3832 3831 3235  5,-0.00048828125
-00000c10: 2922 3e0a 2020 203c 7061 7468 0a20 2020  )">.   <path.   
-00000c20: 643d 224d 2030 2c2d 3220 4320 2d37 2c31  d="M 0,-2 C -7,1
-00000c30: 3420 2d31 362c 3237 202d 3235 2c33 3720  4 -16,27 -25,37 
-00000c40: 4c20 3335 362c 3536 3720 4320 3236 322c  L 356,567 C 262,
-00000c50: 3832 3320 3231 352c 3935 3220 3231 352c  823 215,952 215,
-00000c60: 3935 3420 3231 352c 3937 3920 3232 382c  954 215,979 228,
-00000c70: 3939 3220 3235 352c 3939 3220 3236 342c  992 255,992 264,
-00000c80: 3939 3220 3237 362c 3939 3020 3238 392c  992 276,990 289,
-00000c90: 3938 3720 3331 302c 3939 3120 3333 312c  987 310,991 331,
-00000ca0: 3939 3920 3335 342c 3130 3132 204c 2033  999 354,1012 L 3
-00000cb0: 3831 2c39 3939 2034 3932 2c37 3438 2037  81,999 492,748 7
-00000cc0: 3732 2c31 3034 3920 3833 362c 3130 3234  72,1049 836,1024
-00000cd0: 2038 3630 2c31 3034 3920 4320 3838 312c   860,1049 C 881,
-00000ce0: 3130 3339 2039 3031 2c31 3032 3520 3932  1039 901,1025 92
-00000cf0: 322c 3130 3036 2038 3836 2c39 3337 2038  2,1006 886,937 8
-00000d00: 3335 2c38 3633 2037 3730 2c37 3834 2037  35,863 770,784 7
-00000d10: 3639 2c37 3833 2037 3130 2c37 3136 2035  69,783 710,716 5
-00000d20: 3934 2c35 3834 204c 2037 3734 2c32 3233  94,584 L 774,223
-00000d30: 2043 2037 3734 2c31 3936 2037 3533 2c31   C 774,196 753,1
-00000d40: 3638 2037 3131 2c31 3339 204c 2037 3237  68 711,139 L 727
-00000d50: 2c31 3139 2043 2037 3137 2c39 3020 3639  ,119 C 717,90 69
-00000d60: 392c 3736 2036 3732 2c37 3620 3634 312c  9,76 672,76 641,
-00000d70: 3736 2035 3730 2c31 3738 2034 3537 2c33  76 570,178 457,3
-00000d80: 3831 204c 2031 3634 2c2d 3736 2043 2031  81 L 164,-76 C 1
-00000d90: 3432 2c2d 3131 3020 3131 312c 2d31 3237  42,-110 111,-127
-00000da0: 2037 322c 2d31 3237 2033 302c 2d31 3237   72,-127 30,-127
-00000db0: 2039 2c2d 3131 3020 382c 2d37 3620 312c   9,-110 8,-76 1,
-00000dc0: 2d36 3720 2d32 2c2d 3532 202d 322c 2d33  -67 -2,-52 -2,-3
-00000dd0: 3220 2d32 2c2d 3233 202d 312c 2d31 3320  2 -2,-23 -1,-13 
-00000de0: 302c 2d32 205a 220a 2020 2069 643d 2270  0,-2 Z".   id="p
-00000df0: 6174 6832 3622 202f 3e0a 2020 3c2f 673e  ath26" />.  </g>
-00000e00: 0a20 203c 670a 2020 2069 643d 2262 756c  .  <g.   id="bul
-00000e10: 6c65 742d 6368 6172 2d74 656d 706c 6174  let-char-templat
-00000e20: 652d 3130 3030 3422 0a20 2020 7472 616e  e-10004".   tran
-00000e30: 7366 6f72 6d3d 2273 6361 6c65 2830 2e30  sform="scale(0.0
-00000e40: 3030 3438 3832 3831 3235 2c2d 302e 3030  0048828125,-0.00
-00000e50: 3034 3838 3238 3132 3529 223e 0a20 2020  048828125)">.   
-00000e60: 3c70 6174 680a 2020 2064 3d22 4d20 3238  <path.   d="M 28
-00000e70: 352c 2d33 3320 4320 3138 322c 2d33 3320  5,-33 C 182,-33 
-00000e80: 3131 312c 3330 2037 342c 3135 3620 3532  111,30 74,156 52
-00000e90: 2c32 3238 2034 312c 3333 3320 3431 2c34  ,228 41,333 41,4
-00000ea0: 3731 2034 312c 3534 3920 3535 2c36 3136  71 41,549 55,616
-00000eb0: 2038 322c 3637 3220 3131 362c 3734 3320   82,672 116,743 
-00000ec0: 3136 392c 3737 3820 3234 302c 3737 3820  169,778 240,778 
-00000ed0: 3239 332c 3737 3820 3332 382c 3734 3720  293,778 328,747 
-00000ee0: 3334 362c 3638 3420 4c20 3336 392c 3530  346,684 L 369,50
-00000ef0: 3820 4320 3337 372c 3434 3420 3339 372c  8 C 377,444 397,
-00000f00: 3431 3120 3432 382c 3431 3020 4c20 3131  411 428,410 L 11
-00000f10: 3633 2c31 3131 3620 4320 3131 3734 2c31  63,1116 C 1174,1
-00000f20: 3132 3720 3131 3936 2c31 3133 3320 3132  127 1196,1133 12
-00000f30: 3239 2c31 3133 3320 3132 3731 2c31 3133  29,1133 1271,113
-00000f40: 3320 3132 3932 2c31 3131 3820 3132 3932  3 1292,1118 1292
-00000f50: 2c31 3038 3720 4c20 3132 3932 2c39 3635  ,1087 L 1292,965
-00000f60: 2043 2031 3239 322c 3932 3920 3132 3832   C 1292,929 1282
-00000f70: 2c39 3031 2031 3236 322c 3838 3120 4c20  ,901 1262,881 L 
-00000f80: 3434 322c 3437 2043 2033 3930 2c2d 3620  442,47 C 390,-6 
-00000f90: 3333 382c 2d33 3320 3238 352c 2d33 3320  338,-33 285,-33 
-00000fa0: 5a22 0a20 2020 6964 3d22 7061 7468 3239  Z".   id="path29
-00000fb0: 2220 2f3e 0a20 203c 2f67 3e0a 2020 3c67  " />.  </g>.  <g
-00000fc0: 0a20 2020 6964 3d22 6275 6c6c 6574 2d63  .   id="bullet-c
-00000fd0: 6861 722d 7465 6d70 6c61 7465 2d39 3637  har-template-967
-00000fe0: 3922 0a20 2020 7472 616e 7366 6f72 6d3d  9".   transform=
-00000ff0: 2273 6361 6c65 2830 2e30 3030 3438 3832  "scale(0.0004882
-00001000: 3831 3235 2c2d 302e 3030 3034 3838 3238  8125,-0.00048828
-00001010: 3132 3529 223e 0a20 2020 3c70 6174 680a  125)">.   <path.
-00001020: 2020 2064 3d22 4d20 3831 332c 3020 4320     d="M 813,0 C 
-00001030: 3633 322c 3020 3438 392c 3534 2033 3833  632,0 489,54 383
-00001040: 2c31 3631 2032 3736 2c32 3638 2032 3233  ,161 276,268 223
-00001050: 2c34 3131 2032 3233 2c35 3932 2032 3233  ,411 223,592 223
-00001060: 2c37 3733 2032 3736 2c39 3136 2033 3833  ,773 276,916 383
-00001070: 2c31 3032 3320 3438 392c 3131 3330 2036  ,1023 489,1130 6
-00001080: 3332 2c31 3138 3420 3831 332c 3131 3834  32,1184 813,1184
-00001090: 2039 3932 2c31 3138 3420 3131 3336 2c31   992,1184 1136,1
-000010a0: 3133 3020 3132 3435 2c31 3032 3320 3133  130 1245,1023 13
-000010b0: 3533 2c39 3136 2031 3430 372c 3737 3220  53,916 1407,772 
-000010c0: 3134 3037 2c35 3932 2031 3430 372c 3431  1407,592 1407,41
-000010d0: 3220 3133 3533 2c32 3638 2031 3234 352c  2 1353,268 1245,
-000010e0: 3136 3120 3131 3336 2c35 3420 3939 322c  161 1136,54 992,
-000010f0: 3020 3831 332c 3020 5a22 0a20 2020 6964  0 813,0 Z".   id
-00001100: 3d22 7061 7468 3332 2220 2f3e 0a20 203c  ="path32" />.  <
-00001110: 2f67 3e0a 2020 3c67 0a20 2020 6964 3d22  /g>.  <g.   id="
-00001120: 6275 6c6c 6574 2d63 6861 722d 7465 6d70  bullet-char-temp
-00001130: 6c61 7465 2d38 3232 3622 0a20 2020 7472  late-8226".   tr
-00001140: 616e 7366 6f72 6d3d 2273 6361 6c65 2830  ansform="scale(0
-00001150: 2e30 3030 3438 3832 3831 3235 2c2d 302e  .00048828125,-0.
-00001160: 3030 3034 3838 3238 3132 3529 223e 0a20  00048828125)">. 
-00001170: 2020 3c70 6174 680a 2020 2064 3d22 4d20    <path.   d="M 
-00001180: 3334 362c 3435 3720 4320 3237 332c 3435  346,457 C 273,45
-00001190: 3720 3230 392c 3438 3320 3135 352c 3533  7 209,483 155,53
-000011a0: 3520 3130 312c 3538 3620 3734 2c36 3439  5 101,586 74,649
-000011b0: 2037 342c 3732 3320 3734 2c37 3936 2031   74,723 74,796 1
-000011c0: 3031 2c38 3539 2031 3535 2c39 3131 2032  01,859 155,911 2
-000011d0: 3039 2c39 3633 2032 3733 2c39 3839 2033  09,963 273,989 3
-000011e0: 3436 2c39 3839 2034 3139 2c39 3839 2034  46,989 419,989 4
-000011f0: 3830 2c39 3633 2035 3331 2c39 3130 2035  80,963 531,910 5
-00001200: 3832 2c38 3539 2036 3038 2c37 3936 2036  82,859 608,796 6
-00001210: 3038 2c37 3233 2036 3038 2c36 3438 2035  08,723 608,648 5
-00001220: 3833 2c35 3836 2035 3332 2c35 3335 2034  83,586 532,535 4
-00001230: 3832 2c34 3833 2034 3230 2c34 3537 2033  82,483 420,457 3
-00001240: 3436 2c34 3537 205a 220a 2020 2069 643d  46,457 Z".   id=
-00001250: 2270 6174 6833 3522 202f 3e0a 2020 3c2f  "path35" />.  </
-00001260: 673e 0a20 203c 670a 2020 2069 643d 2262  g>.  <g.   id="b
-00001270: 756c 6c65 742d 6368 6172 2d74 656d 706c  ullet-char-templ
-00001280: 6174 652d 3832 3131 220a 2020 2074 7261  ate-8211".   tra
-00001290: 6e73 666f 726d 3d22 7363 616c 6528 302e  nsform="scale(0.
-000012a0: 3030 3034 3838 3238 3132 352c 2d30 2e30  00048828125,-0.0
-000012b0: 3030 3438 3832 3831 3235 2922 3e0a 2020  0048828125)">.  
-000012c0: 203c 7061 7468 0a20 2020 643d 224d 202d   <path.   d="M -
-000012d0: 342c 3435 3920 4c20 3131 3335 2c34 3539  4,459 L 1135,459
-000012e0: 2031 3133 352c 3630 3620 2d34 2c36 3036   1135,606 -4,606
-000012f0: 202d 342c 3435 3920 5a22 0a20 2020 6964   -4,459 Z".   id
-00001300: 3d22 7061 7468 3338 2220 2f3e 0a20 203c  ="path38" />.  <
-00001310: 2f67 3e0a 2020 3c67 0a20 2020 6964 3d22  /g>.  <g.   id="
-00001320: 6275 6c6c 6574 2d63 6861 722d 7465 6d70  bullet-char-temp
-00001330: 6c61 7465 2d36 3135 3438 220a 2020 2074  late-61548".   t
-00001340: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
-00001350: 302e 3030 3034 3838 3238 3132 352c 2d30  0.00048828125,-0
-00001360: 2e30 3030 3438 3832 3831 3235 2922 3e0a  .00048828125)">.
-00001370: 2020 203c 7061 7468 0a20 2020 643d 224d     <path.   d="M
-00001380: 2031 3733 2c37 3430 2043 2031 3733 2c39   173,740 C 173,9
-00001390: 3033 2032 3331 2c31 3034 3320 3334 362c  03 231,1043 346,
-000013a0: 3131 3539 2034 3632 2c31 3237 3420 3630  1159 462,1274 60
-000013b0: 312c 3133 3332 2037 3635 2c31 3333 3220  1,1332 765,1332 
-000013c0: 3932 382c 3133 3332 2031 3036 372c 3132  928,1332 1067,12
-000013d0: 3734 2031 3138 332c 3131 3539 2031 3239  74 1183,1159 129
-000013e0: 392c 3130 3433 2031 3335 372c 3930 3320  9,1043 1357,903 
-000013f0: 3133 3537 2c37 3430 2031 3335 372c 3537  1357,740 1357,57
-00001400: 3720 3132 3939 2c34 3337 2031 3138 332c  7 1299,437 1183,
-00001410: 3332 3220 3130 3637 2c32 3036 2039 3238  322 1067,206 928
-00001420: 2c31 3438 2037 3635 2c31 3438 2036 3031  ,148 765,148 601
-00001430: 2c31 3438 2034 3632 2c32 3036 2033 3436  ,148 462,206 346
-00001440: 2c33 3232 2032 3331 2c34 3337 2031 3733  ,322 231,437 173
-00001450: 2c35 3737 2031 3733 2c37 3430 205a 220a  ,577 173,740 Z".
-00001460: 2020 2069 643d 2270 6174 6834 3122 202f     id="path41" /
-00001470: 3e0a 2020 3c2f 673e 0a20 3c2f 6465 6673  >.  </g>. </defs
-00001480: 3e0a 203c 670a 2020 2069 643d 2267 3439  >. <g.   id="g49
-00001490: 223e 0a20 203c 670a 2020 2069 643d 2269  ">.  <g.   id="i
-000014a0: 6432 220a 2020 2063 6c61 7373 3d22 4d61  d2".   class="Ma
-000014b0: 7374 6572 5f53 6c69 6465 223e 0a20 2020  ster_Slide">.   
-000014c0: 3c67 0a20 2020 6964 3d22 6267 2d69 6432  <g.   id="bg-id2
-000014d0: 220a 2020 2063 6c61 7373 3d22 4261 636b  ".   class="Back
-000014e0: 6772 6f75 6e64 2220 2f3e 0a20 2020 3c67  ground" />.   <g
-000014f0: 0a20 2020 6964 3d22 626f 2d69 6432 220a  .   id="bo-id2".
-00001500: 2020 2063 6c61 7373 3d22 4261 636b 6772     class="Backgr
-00001510: 6f75 6e64 4f62 6a65 6374 7322 202f 3e0a  oundObjects" />.
-00001520: 2020 3c2f 673e 0a20 3c2f 673e 0a20 3c67    </g>. </g>. <g
-00001530: 0a20 2020 636c 6173 733d 2263 6f6d 2e73  .   class="com.s
-00001540: 756e 2e73 7461 722e 6472 6177 696e 672e  un.star.drawing.
-00001550: 506f 6c79 506f 6c79 676f 6e53 6861 7065  PolyPolygonShape
-00001560: 220a 2020 2069 643d 2267 3631 223e 0a20  ".   id="g61">. 
-00001570: 2020 2020 2020 3c67 0a20 2020 6964 3d22        <g.   id="
-00001580: 6964 3422 3e0a 2020 2020 2020 2020 3c72  id4">.        <r
-00001590: 6563 740a 2020 2063 6c61 7373 3d22 426f  ect.   class="Bo
-000015a0: 756e 6469 6e67 426f 7822 0a20 2020 7374  undingBox".   st
-000015b0: 726f 6b65 3d22 6e6f 6e65 220a 2020 2066  roke="none".   f
-000015c0: 696c 6c3d 226e 6f6e 6522 0a20 2020 783d  ill="none".   x=
-000015d0: 2230 220a 2020 2079 3d22 3022 0a20 2020  "0".   y="0".   
-000015e0: 7769 6474 683d 2238 3439 220a 2020 2068  width="849".   h
-000015f0: 6569 6768 743d 2238 3439 220a 2020 2069  eight="849".   i
-00001600: 643d 2272 6563 7435 3822 202f 3e0a 2020  d="rect58" />.  
-00001610: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
-00001620: 3c2f 673e 3c67 0a20 2020 636c 6173 733d  </g><g.   class=
-00001630: 2247 726f 7570 220a 2020 2069 643d 2267  "Group".   id="g
-00001640: 3834 223e 0a20 2020 2020 2020 3c67 0a20  84">.       <g. 
-00001650: 2020 636c 6173 733d 2263 6f6d 2e73 756e    class="com.sun
-00001660: 2e73 7461 722e 6472 6177 696e 672e 506f  .star.drawing.Po
-00001670: 6c79 506f 6c79 676f 6e53 6861 7065 220a  lyPolygonShape".
-00001680: 2020 2069 643d 2267 3638 223e 0a20 2020     id="g68">.   
-00001690: 2020 2020 203c 670a 2020 2069 643d 2269       <g.   id="i
-000016a0: 6435 223e 0a20 2020 2020 2020 2020 3c72  d5">.         <r
-000016b0: 6563 740a 2020 2063 6c61 7373 3d22 426f  ect.   class="Bo
-000016c0: 756e 6469 6e67 426f 7822 0a20 2020 7374  undingBox".   st
-000016d0: 726f 6b65 3d22 6e6f 6e65 220a 2020 2066  roke="none".   f
-000016e0: 696c 6c3d 226e 6f6e 6522 0a20 2020 783d  ill="none".   x=
-000016f0: 2231 3337 220a 2020 2079 3d22 3138 3722  "137".   y="187"
-00001700: 0a20 2020 7769 6474 683d 2231 3631 220a  .   width="161".
-00001710: 2020 2068 6569 6768 743d 2234 3837 220a     height="487".
-00001720: 2020 2069 643d 2272 6563 7436 3322 202f     id="rect63" /
-00001730: 3e0a 2020 2020 2020 2020 203c 7061 7468  >.         <path
-00001740: 0a20 2020 6669 6c6c 3d22 2330 3030 3030  .   fill="#00000
-00001750: 3022 0a20 2020 7374 726f 6b65 3d22 6e6f  0".   stroke="no
-00001760: 6e65 220a 2020 2064 3d22 4d20 3133 372c  ne".   d="M 137,
-00001770: 3637 3320 5620 3138 3720 6820 3135 3920  673 V 187 h 159 
-00001780: 7620 3932 2048 2031 3931 2076 2031 3138  v 92 H 191 v 118
-00001790: 2068 2039 3920 7620 3931 2068 202d 3939   h 99 v 91 h -99
-000017a0: 2076 2031 3835 207a 220a 2020 2069 643d   v 185 z".   id=
-000017b0: 2270 6174 6836 3522 202f 3e0a 2020 2020  "path65" />.    
-000017c0: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
-000017d0: 3c2f 673e 0a20 2020 2020 2020 3c67 0a20  </g>.       <g. 
-000017e0: 2020 636c 6173 733d 2263 6f6d 2e73 756e    class="com.sun
-000017f0: 2e73 7461 722e 6472 6177 696e 672e 506f  .star.drawing.Po
-00001800: 6c79 506f 6c79 676f 6e53 6861 7065 220a  lyPolygonShape".
-00001810: 2020 2069 643d 2267 3735 223e 0a20 2020     id="g75">.   
-00001820: 2020 2020 203c 670a 2020 2069 643d 2269       <g.   id="i
-00001830: 6436 223e 0a20 2020 2020 2020 2020 3c72  d6">.         <r
-00001840: 6563 740a 2020 2063 6c61 7373 3d22 426f  ect.   class="Bo
-00001850: 756e 6469 6e67 426f 7822 0a20 2020 7374  undingBox".   st
-00001860: 726f 6b65 3d22 6e6f 6e65 220a 2020 2066  roke="none".   f
-00001870: 696c 6c3d 226e 6f6e 6522 0a20 2020 783d  ill="none".   x=
-00001880: 2233 3337 220a 2020 2079 3d22 3138 3722  "337".   y="187"
-00001890: 0a20 2020 7769 6474 683d 2231 3632 220a  .   width="162".
-000018a0: 2020 2068 6569 6768 743d 2234 3837 220a     height="487".
-000018b0: 2020 2069 643d 2272 6563 7437 3022 202f     id="rect70" /
-000018c0: 3e0a 2020 2020 2020 2020 203c 7061 7468  >.         <path
-000018d0: 0a20 2020 6669 6c6c 3d22 2330 3030 3030  .   fill="#00000
-000018e0: 3022 0a20 2020 7374 726f 6b65 3d22 6e6f  0".   stroke="no
-000018f0: 6e65 220a 2020 2064 3d22 4d20 3333 382c  ne".   d="M 338,
-00001900: 3637 3320 5620 3138 3720 6820 3135 3920  673 V 187 h 159 
-00001910: 7620 3932 2048 2033 3932 2076 2031 3138  v 92 H 392 v 118
-00001920: 2068 2039 3920 7620 3931 2068 202d 3939   h 99 v 91 h -99
-00001930: 2076 2031 3835 207a 220a 2020 2069 643d   v 185 z".   id=
-00001940: 2270 6174 6837 3222 202f 3e0a 2020 2020  "path72" />.    
-00001950: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
-00001960: 3c2f 673e 0a20 2020 2020 2020 3c67 0a20  </g>.       <g. 
-00001970: 2020 636c 6173 733d 2263 6f6d 2e73 756e    class="com.sun
-00001980: 2e73 7461 722e 6472 6177 696e 672e 506f  .star.drawing.Po
-00001990: 6c79 506f 6c79 676f 6e53 6861 7065 220a  lyPolygonShape".
-000019a0: 2020 2069 643d 2267 3832 223e 0a20 2020     id="g82">.   
-000019b0: 2020 2020 203c 670a 2020 2069 643d 2269       <g.   id="i
-000019c0: 6437 223e 0a20 2020 2020 2020 2020 3c72  d7">.         <r
-000019d0: 6563 740a 2020 2063 6c61 7373 3d22 426f  ect.   class="Bo
-000019e0: 756e 6469 6e67 426f 7822 0a20 2020 7374  undingBox".   st
-000019f0: 726f 6b65 3d22 6e6f 6e65 220a 2020 2066  roke="none".   f
-00001a00: 696c 6c3d 226e 6f6e 6522 0a20 2020 783d  ill="none".   x=
-00001a10: 2235 3234 220a 2020 2079 3d22 3138 3722  "524".   y="187"
-00001a20: 0a20 2020 7769 6474 683d 2231 3837 220a  .   width="187".
-00001a30: 2020 2068 6569 6768 743d 2234 3837 220a     height="487".
-00001a40: 2020 2069 643d 2272 6563 7437 3722 202f     id="rect77" /
-00001a50: 3e0a 2020 2020 2020 2020 203c 7061 7468  >.         <path
-00001a60: 0a20 2020 6669 6c6c 3d22 2330 3030 3030  .   fill="#00000
-00001a70: 3022 0a20 2020 7374 726f 6b65 3d22 6e6f  0".   stroke="no
-00001a80: 6e65 220a 2020 2064 3d22 4d20 3539 302c  ne".   d="M 590,
-00001a90: 3637 3320 5620 3237 3920 6820 2d36 3620  673 V 279 h -66 
-00001aa0: 7620 2d39 3220 6820 3138 3520 7620 3932  v -92 h 185 v 92
-00001ab0: 2068 202d 3636 2076 2033 3934 207a 220a   h -66 v 394 z".
-00001ac0: 2020 2069 643d 2270 6174 6837 3922 202f     id="path79" /
-00001ad0: 3e0a 2020 2020 2020 2020 3c2f 673e 0a20  >.        </g>. 
-00001ae0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
-00001af0: 203c 2f67 3e0a 3c2f 7376 673e 0a          </g>.</svg>.
+00000020: 462d 3822 3f3e 0a3c 2144 4f43 5459 5045  F-8"?>.<!DOCTYPE
+00000030: 2073 7667 2050 5542 4c49 4320 222d 2f2f   svg PUBLIC "-//
+00000040: 5733 432f 2f44 5444 2053 5647 2031 2e31  W3C//DTD SVG 1.1
+00000050: 2f2f 454e 2220 2268 7474 703a 2f2f 7777  //EN" "http://ww
+00000060: 772e 7733 2e6f 7267 2f47 7261 7068 6963  w.w3.org/Graphic
+00000070: 732f 5356 472f 312e 312f 4454 442f 7376  s/SVG/1.1/DTD/sv
+00000080: 6731 312e 6474 6422 3e0a 3c73 7667 2076  g11.dtd">.<svg v
+00000090: 6572 7369 6f6e 3d22 312e 3222 2077 6964  ersion="1.2" wid
+000000a0: 7468 3d22 3334 2e30 316d 6d22 2068 6569  th="34.01mm" hei
+000000b0: 6768 743d 2233 342e 3031 6d6d 2220 7669  ght="34.01mm" vi
+000000c0: 6577 426f 783d 2231 3237 3030 2031 3739  ewBox="12700 179
+000000d0: 3030 2033 3430 3120 3334 3031 2220 7072  00 3401 3401" pr
+000000e0: 6573 6572 7665 4173 7065 6374 5261 7469  eserveAspectRati
+000000f0: 6f3d 2278 4d69 6459 4d69 6422 2066 696c  o="xMidYMid" fil
+00000100: 6c2d 7275 6c65 3d22 6576 656e 6f64 6422  l-rule="evenodd"
+00000110: 2073 7472 6f6b 652d 7769 6474 683d 2232   stroke-width="2
+00000120: 382e 3232 3222 2073 7472 6f6b 652d 6c69  8.222" stroke-li
+00000130: 6e65 6a6f 696e 3d22 726f 756e 6422 2078  nejoin="round" x
+00000140: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+00000150: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
+00000160: 2220 786d 6c6e 733a 6f6f 6f3d 2268 7474  " xmlns:ooo="htt
+00000170: 703a 2f2f 786d 6c2e 6f70 656e 6f66 6669  p://xml.openoffi
+00000180: 6365 2e6f 7267 2f73 7667 2f65 7870 6f72  ce.org/svg/expor
+00000190: 7422 2078 6d6c 6e73 3a78 6c69 6e6b 3d22  t" xmlns:xlink="
+000001a0: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+000001b0: 672f 3139 3939 2f78 6c69 6e6b 2220 786d  g/1999/xlink" xm
+000001c0: 6c6e 733a 7072 6573 656e 7461 7469 6f6e  lns:presentation
+000001d0: 3d22 6874 7470 3a2f 2f73 756e 2e63 6f6d  ="http://sun.com
+000001e0: 2f78 6d6c 6e73 2f73 7461 726f 6666 6963  /xmlns/staroffic
+000001f0: 652f 7072 6573 656e 7461 7469 6f6e 2220  e/presentation" 
+00000200: 786d 6c6e 733a 736d 696c 3d22 6874 7470  xmlns:smil="http
+00000210: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
+00000220: 3031 2f53 4d49 4c32 302f 2220 786d 6c6e  01/SMIL20/" xmln
+00000230: 733a 616e 696d 3d22 7572 6e3a 6f61 7369  s:anim="urn:oasi
+00000240: 733a 6e61 6d65 733a 7463 3a6f 7065 6e64  s:names:tc:opend
+00000250: 6f63 756d 656e 743a 786d 6c6e 733a 616e  ocument:xmlns:an
+00000260: 696d 6174 696f 6e3a 312e 3022 2078 6d6c  imation:1.0" xml
+00000270: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
+00000280: 223e 0a20 3c64 6566 7320 636c 6173 733d  ">. <defs class=
+00000290: 2245 6d62 6564 6465 6442 756c 6c65 7443  "EmbeddedBulletC
+000002a0: 6861 7273 223e 0a20 203c 6720 6964 3d22  hars">.  <g id="
+000002b0: 6275 6c6c 6574 2d63 6861 722d 7465 6d70  bullet-char-temp
+000002c0: 6c61 7465 2d35 3733 3536 2220 7472 616e  late-57356" tran
+000002d0: 7366 6f72 6d3d 2273 6361 6c65 2830 2e30  sform="scale(0.0
+000002e0: 3030 3438 3832 3831 3235 2c2d 302e 3030  0048828125,-0.00
+000002f0: 3034 3838 3238 3132 3529 223e 0a20 2020  048828125)">.   
+00000300: 3c70 6174 6820 643d 224d 2035 3830 2c31  <path d="M 580,1
+00000310: 3134 3120 4c20 3131 3633 2c35 3731 2035  141 L 1163,571 5
+00000320: 3830 2c30 202d 342c 3537 3120 3538 302c  80,0 -4,571 580,
+00000330: 3131 3431 205a 222f 3e0a 2020 3c2f 673e  1141 Z"/>.  </g>
+00000340: 0a20 203c 6720 6964 3d22 6275 6c6c 6574  .  <g id="bullet
+00000350: 2d63 6861 722d 7465 6d70 6c61 7465 2d35  -char-template-5
+00000360: 3733 3534 2220 7472 616e 7366 6f72 6d3d  7354" transform=
+00000370: 2273 6361 6c65 2830 2e30 3030 3438 3832  "scale(0.0004882
+00000380: 3831 3235 2c2d 302e 3030 3034 3838 3238  8125,-0.00048828
+00000390: 3132 3529 223e 0a20 2020 3c70 6174 6820  125)">.   <path 
+000003a0: 643d 224d 2038 2c31 3132 3820 4c20 3131  d="M 8,1128 L 11
+000003b0: 3337 2c31 3132 3820 3131 3337 2c30 2038  37,1128 1137,0 8
+000003c0: 2c30 2038 2c31 3132 3820 5a22 2f3e 0a20  ,0 8,1128 Z"/>. 
+000003d0: 203c 2f67 3e0a 2020 3c67 2069 643d 2262   </g>.  <g id="b
+000003e0: 756c 6c65 742d 6368 6172 2d74 656d 706c  ullet-char-templ
+000003f0: 6174 652d 3130 3134 3622 2074 7261 6e73  ate-10146" trans
+00000400: 666f 726d 3d22 7363 616c 6528 302e 3030  form="scale(0.00
+00000410: 3034 3838 3238 3132 352c 2d30 2e30 3030  048828125,-0.000
+00000420: 3438 3832 3831 3235 2922 3e0a 2020 203c  48828125)">.   <
+00000430: 7061 7468 2064 3d22 4d20 3137 342c 3020  path d="M 174,0 
+00000440: 4c20 3630 322c 3733 3920 3137 342c 3134  L 602,739 174,14
+00000450: 3831 2031 3435 362c 3733 3920 3137 342c  81 1456,739 174,
+00000460: 3020 5a20 4d20 3133 3538 2c37 3339 204c  0 Z M 1358,739 L
+00000470: 2033 3039 2c31 3334 3620 3635 392c 3733   309,1346 659,73
+00000480: 3920 3133 3538 2c37 3339 205a 222f 3e0a  9 1358,739 Z"/>.
+00000490: 2020 3c2f 673e 0a20 203c 6720 6964 3d22    </g>.  <g id="
+000004a0: 6275 6c6c 6574 2d63 6861 722d 7465 6d70  bullet-char-temp
+000004b0: 6c61 7465 2d31 3031 3332 2220 7472 616e  late-10132" tran
+000004c0: 7366 6f72 6d3d 2273 6361 6c65 2830 2e30  sform="scale(0.0
+000004d0: 3030 3438 3832 3831 3235 2c2d 302e 3030  0048828125,-0.00
+000004e0: 3034 3838 3238 3132 3529 223e 0a20 2020  048828125)">.   
+000004f0: 3c70 6174 6820 643d 224d 2032 3031 352c  <path d="M 2015,
+00000500: 3733 3920 4c20 3132 3736 2c30 2037 3137  739 L 1276,0 717
+00000510: 2c30 2031 3236 302c 3534 3320 3137 342c  ,0 1260,543 174,
+00000520: 3534 3320 3137 342c 3933 3620 3132 3630  543 174,936 1260
+00000530: 2c39 3336 2037 3137 2c31 3438 3120 3132  ,936 717,1481 12
+00000540: 3734 2c31 3438 3120 3230 3135 2c37 3339  74,1481 2015,739
+00000550: 205a 222f 3e0a 2020 3c2f 673e 0a20 203c   Z"/>.  </g>.  <
+00000560: 6720 6964 3d22 6275 6c6c 6574 2d63 6861  g id="bullet-cha
+00000570: 722d 7465 6d70 6c61 7465 2d31 3030 3037  r-template-10007
+00000580: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
+00000590: 6c65 2830 2e30 3030 3438 3832 3831 3235  le(0.00048828125
+000005a0: 2c2d 302e 3030 3034 3838 3238 3132 3529  ,-0.00048828125)
+000005b0: 223e 0a20 2020 3c70 6174 6820 643d 224d  ">.   <path d="M
+000005c0: 2030 2c2d 3220 4320 2d37 2c31 3420 2d31   0,-2 C -7,14 -1
+000005d0: 362c 3237 202d 3235 2c33 3720 4c20 3335  6,27 -25,37 L 35
+000005e0: 362c 3536 3720 4320 3236 322c 3832 3320  6,567 C 262,823 
+000005f0: 3231 352c 3935 3220 3231 352c 3935 3420  215,952 215,954 
+00000600: 3231 352c 3937 3920 3232 382c 3939 3220  215,979 228,992 
+00000610: 3235 352c 3939 3220 3236 342c 3939 3220  255,992 264,992 
+00000620: 3237 362c 3939 3020 3238 392c 3938 3720  276,990 289,987 
+00000630: 3331 302c 3939 3120 3333 312c 3939 3920  310,991 331,999 
+00000640: 3335 342c 3130 3132 204c 2033 3831 2c39  354,1012 L 381,9
+00000650: 3939 2034 3932 2c37 3438 2037 3732 2c31  99 492,748 772,1
+00000660: 3034 3920 3833 362c 3130 3234 2038 3630  049 836,1024 860
+00000670: 2c31 3034 3920 4320 3838 312c 3130 3339  ,1049 C 881,1039
+00000680: 2039 3031 2c31 3032 3520 3932 322c 3130   901,1025 922,10
+00000690: 3036 2038 3836 2c39 3337 2038 3335 2c38  06 886,937 835,8
+000006a0: 3633 2037 3730 2c37 3834 2037 3639 2c37  63 770,784 769,7
+000006b0: 3833 2037 3130 2c37 3136 2035 3934 2c35  83 710,716 594,5
+000006c0: 3834 204c 2037 3734 2c32 3233 2043 2037  84 L 774,223 C 7
+000006d0: 3734 2c31 3936 2037 3533 2c31 3638 2037  74,196 753,168 7
+000006e0: 3131 2c31 3339 204c 2037 3237 2c31 3139  11,139 L 727,119
+000006f0: 2043 2037 3137 2c39 3020 3639 392c 3736   C 717,90 699,76
+00000700: 2036 3732 2c37 3620 3634 312c 3736 2035   672,76 641,76 5
+00000710: 3730 2c31 3738 2034 3537 2c33 3831 204c  70,178 457,381 L
+00000720: 2031 3634 2c2d 3736 2043 2031 3432 2c2d   164,-76 C 142,-
+00000730: 3131 3020 3131 312c 2d31 3237 2037 322c  110 111,-127 72,
+00000740: 2d31 3237 2033 302c 2d31 3237 2039 2c2d  -127 30,-127 9,-
+00000750: 3131 3020 382c 2d37 3620 312c 2d36 3720  110 8,-76 1,-67 
+00000760: 2d32 2c2d 3532 202d 322c 2d33 3220 2d32  -2,-52 -2,-32 -2
+00000770: 2c2d 3233 202d 312c 2d31 3320 302c 2d32  ,-23 -1,-13 0,-2
+00000780: 205a 222f 3e0a 2020 3c2f 673e 0a20 203c   Z"/>.  </g>.  <
+00000790: 6720 6964 3d22 6275 6c6c 6574 2d63 6861  g id="bullet-cha
+000007a0: 722d 7465 6d70 6c61 7465 2d31 3030 3034  r-template-10004
+000007b0: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
+000007c0: 6c65 2830 2e30 3030 3438 3832 3831 3235  le(0.00048828125
+000007d0: 2c2d 302e 3030 3034 3838 3238 3132 3529  ,-0.00048828125)
+000007e0: 223e 0a20 2020 3c70 6174 6820 643d 224d  ">.   <path d="M
+000007f0: 2032 3835 2c2d 3333 2043 2031 3832 2c2d   285,-33 C 182,-
+00000800: 3333 2031 3131 2c33 3020 3734 2c31 3536  33 111,30 74,156
+00000810: 2035 322c 3232 3820 3431 2c33 3333 2034   52,228 41,333 4
+00000820: 312c 3437 3120 3431 2c35 3439 2035 352c  1,471 41,549 55,
+00000830: 3631 3620 3832 2c36 3732 2031 3136 2c37  616 82,672 116,7
+00000840: 3433 2031 3639 2c37 3738 2032 3430 2c37  43 169,778 240,7
+00000850: 3738 2032 3933 2c37 3738 2033 3238 2c37  78 293,778 328,7
+00000860: 3437 2033 3436 2c36 3834 204c 2033 3639  47 346,684 L 369
+00000870: 2c35 3038 2043 2033 3737 2c34 3434 2033  ,508 C 377,444 3
+00000880: 3937 2c34 3131 2034 3238 2c34 3130 204c  97,411 428,410 L
+00000890: 2031 3136 332c 3131 3136 2043 2031 3137   1163,1116 C 117
+000008a0: 342c 3131 3237 2031 3139 362c 3131 3333  4,1127 1196,1133
+000008b0: 2031 3232 392c 3131 3333 2031 3237 312c   1229,1133 1271,
+000008c0: 3131 3333 2031 3239 322c 3131 3138 2031  1133 1292,1118 1
+000008d0: 3239 322c 3130 3837 204c 2031 3239 322c  292,1087 L 1292,
+000008e0: 3936 3520 4320 3132 3932 2c39 3239 2031  965 C 1292,929 1
+000008f0: 3238 322c 3930 3120 3132 3632 2c38 3831  282,901 1262,881
+00000900: 204c 2034 3432 2c34 3720 4320 3339 302c   L 442,47 C 390,
+00000910: 2d36 2033 3338 2c2d 3333 2032 3835 2c2d  -6 338,-33 285,-
+00000920: 3333 205a 222f 3e0a 2020 3c2f 673e 0a20  33 Z"/>.  </g>. 
+00000930: 203c 6720 6964 3d22 6275 6c6c 6574 2d63   <g id="bullet-c
+00000940: 6861 722d 7465 6d70 6c61 7465 2d39 3637  har-template-967
+00000950: 3922 2074 7261 6e73 666f 726d 3d22 7363  9" transform="sc
+00000960: 616c 6528 302e 3030 3034 3838 3238 3132  ale(0.0004882812
+00000970: 352c 2d30 2e30 3030 3438 3832 3831 3235  5,-0.00048828125
+00000980: 2922 3e0a 2020 203c 7061 7468 2064 3d22  )">.   <path d="
+00000990: 4d20 3831 332c 3020 4320 3633 322c 3020  M 813,0 C 632,0 
+000009a0: 3438 392c 3534 2033 3833 2c31 3631 2032  489,54 383,161 2
+000009b0: 3736 2c32 3638 2032 3233 2c34 3131 2032  76,268 223,411 2
+000009c0: 3233 2c35 3932 2032 3233 2c37 3733 2032  23,592 223,773 2
+000009d0: 3736 2c39 3136 2033 3833 2c31 3032 3320  76,916 383,1023 
+000009e0: 3438 392c 3131 3330 2036 3332 2c31 3138  489,1130 632,118
+000009f0: 3420 3831 332c 3131 3834 2039 3932 2c31  4 813,1184 992,1
+00000a00: 3138 3420 3131 3336 2c31 3133 3020 3132  184 1136,1130 12
+00000a10: 3435 2c31 3032 3320 3133 3533 2c39 3136  45,1023 1353,916
+00000a20: 2031 3430 372c 3737 3220 3134 3037 2c35   1407,772 1407,5
+00000a30: 3932 2031 3430 372c 3431 3220 3133 3533  92 1407,412 1353
+00000a40: 2c32 3638 2031 3234 352c 3136 3120 3131  ,268 1245,161 11
+00000a50: 3336 2c35 3420 3939 322c 3020 3831 332c  36,54 992,0 813,
+00000a60: 3020 5a22 2f3e 0a20 203c 2f67 3e0a 2020  0 Z"/>.  </g>.  
+00000a70: 3c67 2069 643d 2262 756c 6c65 742d 6368  <g id="bullet-ch
+00000a80: 6172 2d74 656d 706c 6174 652d 3832 3236  ar-template-8226
+00000a90: 2220 7472 616e 7366 6f72 6d3d 2273 6361  " transform="sca
+00000aa0: 6c65 2830 2e30 3030 3438 3832 3831 3235  le(0.00048828125
+00000ab0: 2c2d 302e 3030 3034 3838 3238 3132 3529  ,-0.00048828125)
+00000ac0: 223e 0a20 2020 3c70 6174 6820 643d 224d  ">.   <path d="M
+00000ad0: 2033 3436 2c34 3537 2043 2032 3733 2c34   346,457 C 273,4
+00000ae0: 3537 2032 3039 2c34 3833 2031 3535 2c35  57 209,483 155,5
+00000af0: 3335 2031 3031 2c35 3836 2037 342c 3634  35 101,586 74,64
+00000b00: 3920 3734 2c37 3233 2037 342c 3739 3620  9 74,723 74,796 
+00000b10: 3130 312c 3835 3920 3135 352c 3931 3120  101,859 155,911 
+00000b20: 3230 392c 3936 3320 3237 332c 3938 3920  209,963 273,989 
+00000b30: 3334 362c 3938 3920 3431 392c 3938 3920  346,989 419,989 
+00000b40: 3438 302c 3936 3320 3533 312c 3931 3020  480,963 531,910 
+00000b50: 3538 322c 3835 3920 3630 382c 3739 3620  582,859 608,796 
+00000b60: 3630 382c 3732 3320 3630 382c 3634 3820  608,723 608,648 
+00000b70: 3538 332c 3538 3620 3533 322c 3533 3520  583,586 532,535 
+00000b80: 3438 322c 3438 3320 3432 302c 3435 3720  482,483 420,457 
+00000b90: 3334 362c 3435 3720 5a22 2f3e 0a20 203c  346,457 Z"/>.  <
+00000ba0: 2f67 3e0a 2020 3c67 2069 643d 2262 756c  /g>.  <g id="bul
+00000bb0: 6c65 742d 6368 6172 2d74 656d 706c 6174  let-char-templat
+00000bc0: 652d 3832 3131 2220 7472 616e 7366 6f72  e-8211" transfor
+00000bd0: 6d3d 2273 6361 6c65 2830 2e30 3030 3438  m="scale(0.00048
+00000be0: 3832 3831 3235 2c2d 302e 3030 3034 3838  828125,-0.000488
+00000bf0: 3238 3132 3529 223e 0a20 2020 3c70 6174  28125)">.   <pat
+00000c00: 6820 643d 224d 202d 342c 3435 3920 4c20  h d="M -4,459 L 
+00000c10: 3131 3335 2c34 3539 2031 3133 352c 3630  1135,459 1135,60
+00000c20: 3620 2d34 2c36 3036 202d 342c 3435 3920  6 -4,606 -4,459 
+00000c30: 5a22 2f3e 0a20 203c 2f67 3e0a 2020 3c67  Z"/>.  </g>.  <g
+00000c40: 2069 643d 2262 756c 6c65 742d 6368 6172   id="bullet-char
+00000c50: 2d74 656d 706c 6174 652d 3631 3534 3822  -template-61548"
+00000c60: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
+00000c70: 6528 302e 3030 3034 3838 3238 3132 352c  e(0.00048828125,
+00000c80: 2d30 2e30 3030 3438 3832 3831 3235 2922  -0.00048828125)"
+00000c90: 3e0a 2020 203c 7061 7468 2064 3d22 4d20  >.   <path d="M 
+00000ca0: 3137 332c 3734 3020 4320 3137 332c 3930  173,740 C 173,90
+00000cb0: 3320 3233 312c 3130 3433 2033 3436 2c31  3 231,1043 346,1
+00000cc0: 3135 3920 3436 322c 3132 3734 2036 3031  159 462,1274 601
+00000cd0: 2c31 3333 3220 3736 352c 3133 3332 2039  ,1332 765,1332 9
+00000ce0: 3238 2c31 3333 3220 3130 3637 2c31 3237  28,1332 1067,127
+00000cf0: 3420 3131 3833 2c31 3135 3920 3132 3939  4 1183,1159 1299
+00000d00: 2c31 3034 3320 3133 3537 2c39 3033 2031  ,1043 1357,903 1
+00000d10: 3335 372c 3734 3020 3133 3537 2c35 3737  357,740 1357,577
+00000d20: 2031 3239 392c 3433 3720 3131 3833 2c33   1299,437 1183,3
+00000d30: 3232 2031 3036 372c 3230 3620 3932 382c  22 1067,206 928,
+00000d40: 3134 3820 3736 352c 3134 3820 3630 312c  148 765,148 601,
+00000d50: 3134 3820 3436 322c 3230 3620 3334 362c  148 462,206 346,
+00000d60: 3332 3220 3233 312c 3433 3720 3137 332c  322 231,437 173,
+00000d70: 3537 3720 3137 332c 3734 3020 5a22 2f3e  577 173,740 Z"/>
+00000d80: 0a20 203c 2f67 3e0a 203c 2f64 6566 733e  .  </g>. </defs>
+00000d90: 0a20 3c67 2063 6c61 7373 3d22 5061 6765  . <g class="Page
+00000da0: 223e 0a20 203c 6720 636c 6173 733d 2247  ">.  <g class="G
+00000db0: 726f 7570 223e 0a20 2020 3c67 2063 6c61  roup">.   <g cla
+00000dc0: 7373 3d22 636f 6d2e 7375 6e2e 7374 6172  ss="com.sun.star
+00000dd0: 2e64 7261 7769 6e67 2e43 7573 746f 6d53  .drawing.CustomS
+00000de0: 6861 7065 223e 0a20 2020 203c 6720 6964  hape">.    <g id
+00000df0: 3d22 6964 3322 3e0a 2020 2020 203c 7265  ="id3">.     <re
+00000e00: 6374 2063 6c61 7373 3d22 426f 756e 6469  ct class="Boundi
+00000e10: 6e67 426f 7822 2073 7472 6f6b 653d 226e  ngBox" stroke="n
+00000e20: 6f6e 6522 2066 696c 6c3d 226e 6f6e 6522  one" fill="none"
+00000e30: 2078 3d22 3132 3730 3022 2079 3d22 3137   x="12700" y="17
+00000e40: 3930 3022 2077 6964 7468 3d22 3334 3031  900" width="3401
+00000e50: 2220 6865 6967 6874 3d22 3334 3031 222f  " height="3401"/
+00000e60: 3e0a 2020 2020 3c2f 673e 0a20 2020 3c2f  >.    </g>.   </
+00000e70: 673e 0a20 2020 3c67 2063 6c61 7373 3d22  g>.   <g class="
+00000e80: 4772 6f75 7022 3e0a 2020 2020 3c67 2063  Group">.    <g c
+00000e90: 6c61 7373 3d22 4772 6f75 7022 3e0a 2020  lass="Group">.  
+00000ea0: 2020 203c 6720 636c 6173 733d 2263 6f6d     <g class="com
+00000eb0: 2e73 756e 2e73 7461 722e 6472 6177 696e  .sun.star.drawin
+00000ec0: 672e 4f70 656e 4265 7a69 6572 5368 6170  g.OpenBezierShap
+00000ed0: 6522 3e0a 2020 2020 2020 3c67 2069 643d  e">.      <g id=
+00000ee0: 2269 6434 223e 0a20 2020 2020 2020 3c72  "id4">.       <r
+00000ef0: 6563 7420 636c 6173 733d 2242 6f75 6e64  ect class="Bound
+00000f00: 696e 6742 6f78 2220 7374 726f 6b65 3d22  ingBox" stroke="
+00000f10: 6e6f 6e65 2220 6669 6c6c 3d22 6e6f 6e65  none" fill="none
+00000f20: 2220 783d 2231 3238 3232 2220 793d 2231  " x="12822" y="1
+00000f30: 3739 3931 2220 7769 6474 683d 2232 3031  7991" width="201
+00000f40: 2220 6865 6967 6874 3d22 3939 3722 2f3e  " height="997"/>
+00000f50: 0a20 2020 2020 2020 3c70 6174 6820 6669  .       <path fi
+00000f60: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
+00000f70: 3d22 7267 6228 3130 322c 3130 322c 3130  ="rgb(102,102,10
+00000f80: 3229 2220 7374 726f 6b65 2d77 6964 7468  2)" stroke-width
+00000f90: 3d22 3230 3022 2073 7472 6f6b 652d 6c69  ="200" stroke-li
+00000fa0: 6e65 6a6f 696e 3d22 726f 756e 6422 2073  nejoin="round" s
+00000fb0: 7472 6f6b 652d 6c69 6e65 6361 703d 2273  troke-linecap="s
+00000fc0: 7175 6172 6522 2064 3d22 4d20 3132 3932  quare" d="M 1292
+00000fd0: 322c 3138 3039 3120 4c20 3132 3932 322c  2,18091 L 12922,
+00000fe0: 3138 3838 3622 2f3e 0a20 2020 2020 203c  18886"/>.      <
+00000ff0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
+00001000: 2020 203c 6720 636c 6173 733d 2263 6f6d     <g class="com
+00001010: 2e73 756e 2e73 7461 722e 6472 6177 696e  .sun.star.drawin
+00001020: 672e 4f70 656e 4265 7a69 6572 5368 6170  g.OpenBezierShap
+00001030: 6522 3e0a 2020 2020 2020 3c67 2069 643d  e">.      <g id=
+00001040: 2269 6435 223e 0a20 2020 2020 2020 3c72  "id5">.       <r
+00001050: 6563 7420 636c 6173 733d 2242 6f75 6e64  ect class="Bound
+00001060: 696e 6742 6f78 2220 7374 726f 6b65 3d22  ingBox" stroke="
+00001070: 6e6f 6e65 2220 6669 6c6c 3d22 6e6f 6e65  none" fill="none
+00001080: 2220 783d 2231 3433 3131 2220 793d 2231  " x="14311" y="1
+00001090: 3739 3932 2220 7769 6474 683d 2232 3031  7992" width="201
+000010a0: 2220 6865 6967 6874 3d22 3231 3334 222f  " height="2134"/
+000010b0: 3e0a 2020 2020 2020 203c 7061 7468 2066  >.       <path f
+000010c0: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
+000010d0: 653d 2272 6762 2831 3032 2c31 3032 2c31  e="rgb(102,102,1
+000010e0: 3032 2922 2073 7472 6f6b 652d 7769 6474  02)" stroke-widt
+000010f0: 683d 2232 3030 2220 7374 726f 6b65 2d6c  h="200" stroke-l
+00001100: 696e 656a 6f69 6e3d 2272 6f75 6e64 2220  inejoin="round" 
+00001110: 7374 726f 6b65 2d6c 696e 6563 6170 3d22  stroke-linecap="
+00001120: 7371 7561 7265 2220 643d 224d 2031 3434  square" d="M 144
+00001130: 3131 2c31 3830 3932 204c 2031 3434 3131  11,18092 L 14411
+00001140: 2c32 3030 3235 222f 3e0a 2020 2020 2020  ,20025"/>.      
+00001150: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
+00001160: 2020 2020 3c67 2063 6c61 7373 3d22 636f      <g class="co
+00001170: 6d2e 7375 6e2e 7374 6172 2e64 7261 7769  m.sun.star.drawi
+00001180: 6e67 2e45 6c6c 6970 7365 5368 6170 6522  ng.EllipseShape"
+00001190: 3e0a 2020 2020 2020 3c67 2069 643d 2269  >.      <g id="i
+000011a0: 6436 223e 0a20 2020 2020 2020 3c72 6563  d6">.       <rec
+000011b0: 7420 636c 6173 733d 2242 6f75 6e64 696e  t class="Boundin
+000011c0: 6742 6f78 2220 7374 726f 6b65 3d22 6e6f  gBox" stroke="no
+000011d0: 6e65 2220 6669 6c6c 3d22 6e6f 6e65 2220  ne" fill="none" 
+000011e0: 783d 2231 3333 3134 2220 793d 2231 3830  x="13314" y="180
+000011f0: 3130 2220 7769 6474 683d 2237 3036 2220  10" width="706" 
+00001200: 6865 6967 6874 3d22 3135 3431 222f 3e0a  height="1541"/>.
+00001210: 2020 2020 2020 203c 7061 7468 2066 696c         <path fil
+00001220: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+00001230: 2272 6762 2831 3032 2c31 3032 2c31 3032  "rgb(102,102,102
+00001240: 2922 2073 7472 6f6b 652d 7769 6474 683d  )" stroke-width=
+00001250: 2232 3030 2220 7374 726f 6b65 2d6c 696e  "200" stroke-lin
+00001260: 656a 6f69 6e3d 2272 6f75 6e64 2220 643d  ejoin="round" d=
+00001270: 224d 2031 3336 3637 2c31 3934 3530 2043  "M 13667,19450 C
+00001280: 2031 3336 3232 2c31 3934 3530 2031 3335   13622,19450 135
+00001290: 3739 2c31 3934 3139 2031 3335 3430 2c31  79,19419 13540,1
+000012a0: 3933 3630 2031 3335 3032 2c31 3933 3031  9360 13502,19301
+000012b0: 2031 3334 3730 2c31 3932 3137 2031 3334   13470,19217 134
+000012c0: 3438 2c31 3931 3135 2031 3334 3236 2c31  48,19115 13426,1
+000012d0: 3930 3133 2031 3334 3134 2c31 3838 3938  9013 13414,18898
+000012e0: 2031 3334 3134 2c31 3837 3830 2031 3334   13414,18780 134
+000012f0: 3134 2c31 3836 3632 2031 3334 3236 2c31  14,18662 13426,1
+00001300: 3835 3437 2031 3334 3438 2c31 3834 3435  8547 13448,18445
+00001310: 2031 3334 3730 2c31 3833 3433 2031 3335   13470,18343 135
+00001320: 3032 2c31 3832 3539 2031 3335 3430 2c31  02,18259 13540,1
+00001330: 3832 3030 2031 3335 3739 2c31 3831 3431  8200 13579,18141
+00001340: 2031 3336 3232 2c31 3831 3130 2031 3336   13622,18110 136
+00001350: 3637 2c31 3831 3130 2031 3337 3131 2c31  67,18110 13711,1
+00001360: 3831 3130 2031 3337 3534 2c31 3831 3431  8110 13754,18141
+00001370: 2031 3337 3933 2c31 3832 3030 2031 3338   13793,18200 138
+00001380: 3331 2c31 3832 3539 2031 3338 3633 2c31  31,18259 13863,1
+00001390: 3833 3433 2031 3338 3835 2c31 3834 3435  8343 13885,18445
+000013a0: 2031 3339 3037 2c31 3835 3437 2031 3339   13907,18547 139
+000013b0: 3139 2c31 3836 3632 2031 3339 3139 2c31  19,18662 13919,1
+000013c0: 3837 3830 2031 3339 3139 2c31 3838 3938  8780 13919,18898
+000013d0: 2031 3339 3037 2c31 3930 3133 2031 3338   13907,19013 138
+000013e0: 3835 2c31 3931 3135 2031 3338 3633 2c31  85,19115 13863,1
+000013f0: 3932 3137 2031 3338 3331 2c31 3933 3031  9217 13831,19301
+00001400: 2031 3337 3933 2c31 3933 3630 2031 3337   13793,19360 137
+00001410: 3534 2c31 3934 3139 2031 3337 3131 2c31  54,19419 13711,1
+00001420: 3934 3530 2031 3336 3637 2c31 3934 3530  9450 13667,19450
+00001430: 205a 222f 3e0a 2020 2020 2020 3c2f 673e   Z"/>.      </g>
+00001440: 0a20 2020 2020 3c2f 673e 0a20 2020 2020  .     </g>.     
+00001450: 3c67 2063 6c61 7373 3d22 636f 6d2e 7375  <g class="com.su
+00001460: 6e2e 7374 6172 2e64 7261 7769 6e67 2e45  n.star.drawing.E
+00001470: 6c6c 6970 7365 5368 6170 6522 3e0a 2020  llipseShape">.  
+00001480: 2020 2020 3c67 2069 643d 2269 6437 223e      <g id="id7">
+00001490: 0a20 2020 2020 2020 3c72 6563 7420 636c  .       <rect cl
+000014a0: 6173 733d 2242 6f75 6e64 696e 6742 6f78  ass="BoundingBox
+000014b0: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
+000014c0: 6669 6c6c 3d22 6e6f 6e65 2220 783d 2231  fill="none" x="1
+000014d0: 3437 3633 2220 793d 2231 3830 3130 2220  4763" y="18010" 
+000014e0: 7769 6474 683d 2237 3836 2220 6865 6967  width="786" heig
+000014f0: 6874 3d22 3235 3030 222f 3e0a 2020 2020  ht="2500"/>.    
+00001500: 2020 203c 7061 7468 2066 696c 6c3d 226e     <path fill="n
+00001510: 6f6e 6522 2073 7472 6f6b 653d 2272 6762  one" stroke="rgb
+00001520: 2831 3032 2c31 3032 2c31 3032 2922 2073  (102,102,102)" s
+00001530: 7472 6f6b 652d 7769 6474 683d 2232 3030  troke-width="200
+00001540: 2220 7374 726f 6b65 2d6c 696e 656a 6f69  " stroke-linejoi
+00001550: 6e3d 2272 6f75 6e64 2220 643d 224d 2031  n="round" d="M 1
+00001560: 3531 3536 2c32 3034 3039 2043 2031 3531  5156,20409 C 151
+00001570: 3034 2c32 3034 3039 2031 3530 3534 2c32  04,20409 15054,2
+00001580: 3033 3536 2031 3530 3039 2c32 3032 3535  0356 15009,20255
+00001590: 2031 3439 3635 2c32 3031 3534 2031 3439   14965,20154 149
+000015a0: 3238 2c32 3030 3039 2031 3439 3032 2c31  28,20009 14902,1
+000015b0: 3938 3334 2031 3438 3737 2c31 3936 3630  9834 14877,19660
+000015c0: 2031 3438 3633 2c31 3934 3631 2031 3438   14863,19461 148
+000015d0: 3633 2c31 3932 3630 2031 3438 3633 2c31  63,19260 14863,1
+000015e0: 3930 3538 2031 3438 3737 2c31 3838 3539  9058 14877,18859
+000015f0: 2031 3439 3032 2c31 3836 3835 2031 3439   14902,18685 149
+00001600: 3238 2c31 3835 3130 2031 3439 3635 2c31  28,18510 14965,1
+00001610: 3833 3635 2031 3530 3039 2c31 3832 3634  8365 15009,18264
+00001620: 2031 3530 3534 2c31 3831 3633 2031 3531   15054,18163 151
+00001630: 3034 2c31 3831 3130 2031 3531 3536 2c31  04,18110 15156,1
+00001640: 3831 3130 2031 3532 3037 2c31 3831 3130  8110 15207,18110
+00001650: 2031 3532 3537 2c31 3831 3633 2031 3533   15257,18163 153
+00001660: 3032 2c31 3832 3634 2031 3533 3436 2c31  02,18264 15346,1
+00001670: 3833 3635 2031 3533 3833 2c31 3835 3130  8365 15383,18510
+00001680: 2031 3534 3039 2c31 3836 3835 2031 3534   15409,18685 154
+00001690: 3334 2c31 3838 3539 2031 3534 3438 2c31  34,18859 15448,1
+000016a0: 3930 3538 2031 3534 3438 2c31 3932 3630  9058 15448,19260
+000016b0: 2031 3534 3438 2c31 3934 3631 2031 3534   15448,19461 154
+000016c0: 3334 2c31 3936 3630 2031 3534 3039 2c31  34,19660 15409,1
+000016d0: 3938 3334 2031 3533 3833 2c32 3030 3039  9834 15383,20009
+000016e0: 2031 3533 3436 2c32 3031 3534 2031 3533   15346,20154 153
+000016f0: 3032 2c32 3032 3535 2031 3532 3537 2c32  02,20255 15257,2
+00001700: 3033 3536 2031 3532 3037 2c32 3034 3039  0356 15207,20409
+00001710: 2031 3531 3536 2c32 3034 3039 205a 222f   15156,20409 Z"/
+00001720: 3e0a 2020 2020 2020 3c2f 673e 0a20 2020  >.      </g>.   
+00001730: 2020 3c2f 673e 0a20 2020 2020 3c67 2063    </g>.     <g c
+00001740: 6c61 7373 3d22 636f 6d2e 7375 6e2e 7374  lass="com.sun.st
+00001750: 6172 2e64 7261 7769 6e67 2e4c 696e 6553  ar.drawing.LineS
+00001760: 6861 7065 223e 0a20 2020 2020 203c 6720  hape">.      <g 
+00001770: 6964 3d22 6964 3822 3e0a 2020 2020 2020  id="id8">.      
+00001780: 203c 7265 6374 2063 6c61 7373 3d22 426f   <rect class="Bo
+00001790: 756e 6469 6e67 426f 7822 2073 7472 6f6b  undingBox" strok
+000017a0: 653d 226e 6f6e 6522 2066 696c 6c3d 226e  e="none" fill="n
+000017b0: 6f6e 6522 2078 3d22 3135 3830 3022 2079  one" x="15800" y
+000017c0: 3d22 3137 3939 3122 2077 6964 7468 3d22  ="17991" width="
+000017d0: 3230 3122 2068 6569 6768 743d 2233 3137  201" height="317
+000017e0: 3622 2f3e 0a20 2020 2020 2020 3c70 6174  6"/>.       <pat
+000017f0: 6820 6669 6c6c 3d22 6e6f 6e65 2220 7374  h fill="none" st
+00001800: 726f 6b65 3d22 7267 6228 3130 322c 3130  roke="rgb(102,10
+00001810: 322c 3130 3229 2220 7374 726f 6b65 2d77  2,102)" stroke-w
+00001820: 6964 7468 3d22 3230 3022 2073 7472 6f6b  idth="200" strok
+00001830: 652d 6c69 6e65 6a6f 696e 3d22 726f 756e  e-linejoin="roun
+00001840: 6422 2073 7472 6f6b 652d 6c69 6e65 6361  d" stroke-lineca
+00001850: 703d 2273 7175 6172 6522 2064 3d22 4d20  p="square" d="M 
+00001860: 3135 3930 302c 3138 3039 3120 4c20 3135  15900,18091 L 15
+00001870: 3930 302c 3231 3036 3622 2f3e 0a20 2020  900,21066"/>.   
+00001880: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
+00001890: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
+000018a0: 6720 636c 6173 733d 2263 6f6d 2e73 756e  g class="com.sun
+000018b0: 2e73 7461 722e 6472 6177 696e 672e 4f70  .star.drawing.Op
+000018c0: 656e 4265 7a69 6572 5368 6170 6522 3e0a  enBezierShape">.
+000018d0: 2020 2020 203c 6720 6964 3d22 6964 3922       <g id="id9"
+000018e0: 3e0a 2020 2020 2020 3c72 6563 7420 636c  >.      <rect cl
+000018f0: 6173 733d 2242 6f75 6e64 696e 6742 6f78  ass="BoundingBox
+00001900: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
+00001910: 6669 6c6c 3d22 6e6f 6e65 2220 783d 2231  fill="none" x="1
+00001920: 3238 3235 2220 793d 2231 3930 3231 2220  2825" y="19021" 
+00001930: 7769 6474 683d 2232 3934 3822 2068 6569  width="2948" hei
+00001940: 6768 743d 2232 3136 3422 2f3e 0a20 2020  ght="2164"/>.   
+00001950: 2020 203c 7061 7468 2066 696c 6c3d 226e     <path fill="n
+00001960: 6f6e 6522 2073 7472 6f6b 653d 2272 6762  one" stroke="rgb
+00001970: 2831 3834 2c30 2c37 3129 2220 7374 726f  (184,0,71)" stro
+00001980: 6b65 2d77 6964 7468 3d22 3135 3022 2073  ke-width="150" s
+00001990: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3d22  troke-linejoin="
+000019a0: 726f 756e 6422 2064 3d22 4d20 3135 3639  round" d="M 1569
+000019b0: 372c 3230 3939 3320 4320 3135 3630 322c  7,20993 C 15602,
+000019c0: 3231 3136 3320 3135 3535 392c 3231 3039  21163 15559,2109
+000019d0: 3020 3135 3439 352c 3230 3936 3720 3135  0 15495,20967 15
+000019e0: 3433 312c 3230 3834 3420 3135 3339 302c  431,20844 15390,
+000019f0: 3230 3732 3620 3135 3239 352c 3230 3933  20726 15295,2093
+00001a00: 3820 3135 3230 312c 3231 3230 3020 3135  8 15201,21200 15
+00001a10: 3135 382c 3231 3038 3820 3135 3039 332c  158,21088 15093,
+00001a20: 3230 3930 3220 3135 3032 382c 3230 3731  20902 15028,2071
+00001a30: 3620 3134 3938 362c 3230 3534 3320 3134  6 14986,20543 14
+00001a40: 3839 342c 3230 3836 3320 4c20 3134 3839  894,20863 L 1489
+00001a50: 342c 3230 3835 3520 4320 3134 3830 312c  4,20855 C 14801,
+00001a60: 3231 3234 3420 3134 3735 382c 3231 3038  21244 14758,2108
+00001a70: 3020 3134 3639 322c 3230 3831 3020 3134  0 14692,20810 14
+00001a80: 3632 362c 3230 3533 3820 3134 3538 352c  626,20538 14585,
+00001a90: 3230 3239 3120 3134 3439 332c 3230 3735  20291 14493,2075
+00001aa0: 3520 3134 3339 392c 3231 3330 3720 3134  5 14399,21307 14
+00001ab0: 3337 372c 3231 3039 3320 3134 3239 322c  377,21093 14292,
+00001ac0: 3230 3639 3520 3134 3232 372c 3230 3331  20695 14227,2031
+00001ad0: 3120 3134 3138 322c 3139 3937 3520 3134  1 14182,19975 14
+00001ae0: 3039 312c 3230 3632 3620 4c20 3134 3039  091,20626 L 1409
+00001af0: 312c 3230 3632 3320 4320 3134 3030 302c  1,20623 C 14000,
+00001b00: 3231 3338 3620 3133 3939 392c 3231 3136  21386 13999,2116
+00001b10: 3620 3133 3839 322c 3230 3534 3520 3133  6 13892,20545 13
+00001b20: 3832 382c 3230 3032 3620 3133 3738 332c  828,20026 13783,
+00001b30: 3139 3535 3620 3133 3639 322c 3230 3434  19556 13692,2044
+00001b40: 3020 3133 3630 302c 3231 3436 3820 3133  0 13600,21468 13
+00001b50: 3537 332c 3231 3136 3620 3133 3439 322c  573,21166 13492,
+00001b60: 3230 3334 3220 3133 3432 372c 3139 3634  20342 13427,1964
+00001b70: 3520 3133 3338 362c 3139 3035 3320 3133  5 13386,19053 13
+00001b80: 3239 322c 3230 3233 3320 3133 3230 302c  292,20233 13200,
+00001b90: 3231 3438 3020 3133 3230 302c 3231 3238  21480 13200,2128
+00001ba0: 3620 3133 3039 352c 3230 3131 3120 3133  6 13095,20111 13
+00001bb0: 3033 352c 3139 3230 3020 3132 3939 342c  035,19200 12994,
+00001bc0: 3138 3433 3920 3132 3930 302c 3139 3937  18439 12900,1997
+00001bd0: 3922 2f3e 0a20 2020 2020 3c2f 673e 0a20  9"/>.     </g>. 
+00001be0: 2020 203c 2f67 3e0a 2020 203c 2f67 3e0a     </g>.   </g>.
+00001bf0: 2020 3c2f 673e 0a20 3c2f 673e 0a3c 2f73    </g>. </g>.</s
+00001c00: 7667 3e                                  vg>
```

### Comparing `pyfda-0.7.1/pyfda/images/icons/light/appbar.base.select_grey.svg` & `pyfda-0.8.0a2/pyfda/images/unused/appbar.base.select_grey.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/light/appbar.list.add.above_grey.svg` & `pyfda-0.8.0a2/pyfda/images/unused/appbar.list.add.above_grey.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/pyfda_icon.png` & `pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/pyfda_icon.svg` & `pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/pyfda_icon_128.png` & `pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_128.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/pyfda_icon_16.png` & `pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_16.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/pyfda_icon_256.png` & `pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_256.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/pyfda_icon_32.png` & `pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_32.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/pyfda_icon_48.png` & `pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_48.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/icons/pyfda_icon_64.png` & `pyfda-0.8.0a2/pyfda/images/icons/pyfda_icon_64.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/unused/audio.svg` & `pyfda-0.8.0a2/pyfda/images/unused/audio/audio.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/unused/audio_90.png` & `pyfda-0.8.0a2/pyfda/images/unused/audio/audio_90.png`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/images/unused/audio_90.svg` & `pyfda-0.8.0a2/pyfda/images/unused/audio/audio_90.svg`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/input_widgets/amplitude_specs.py` & `pyfda-0.8.0a2/pyfda/input_widgets/amplitude_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/input_widgets/freq_specs.py` & `pyfda-0.8.0a2/pyfda/input_widgets/freq_specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 from pyfda.libs.pyfda_qt_lib import qstyle_widget
 from pyfda.pyfda_rc import params  # FMT string for QLineEdit fields, e.g. '{:.3g}'
 
 import logging
 logger = logging.getLogger(__name__)
 
 MIN_FREQ_STEP = 1e-4
-MIN_FREQ = 0.0  # min. frequency
-MAX_FREQ = 0.5  # max. frequency (normalize w.r.t. f_S)
-
 
 class FreqSpecs(QWidget):
     """
     Build and update widget for entering the frequency
     specifications like F_sb, F_pb etc.
     """
     # class variables (shared between instances if more than one exists)
@@ -58,15 +55,14 @@
         if dict_sig['id'] == id(self):
             # logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
             return
         elif 'specs_changed' in dict_sig and dict_sig['specs_changed'] == 'f_specs':
             self.sort_dict_freqs()
         elif 'view_changed' in dict_sig and dict_sig['view_changed'] == 'f_S':
             self.recalc_freqs()
-            # self.load_dict()
 
 # -------------------------------------------------------------
     def _construct_UI(self):
         """
         Construct the User Interface
         """
         bfont = QFont()
@@ -254,24 +250,25 @@
         else:
             unit_frmt = 'b'
         self.lblUnit.setText(" in " + to_html(unit, frmt=unit_frmt))
 
 # -------------------------------------------------------------
     def load_dict(self):
         """
-        Reload textfields from filter dictionary
-        Transform the displayed frequency spec input fields according to the units
-        setting (i.e. f_S). Spec entries are always stored normalized w.r.t. f_S
-        in the dictionary; when f_S or the unit are changed, only the displayed values
-        of the frequency entries are updated, not the dictionary!
+        - Reload textfields from filter dictionary
+
+        - Transform the displayed frequency spec input fields according to the units
+          setting (i.e. f_S). Spec entries are always stored normalized w.r.t. f_S
+          in the dictionary; when f_S or the unit are changed, only the displayed values
+          of the frequency entries are updated, not the dictionary!
 
-        Update the displayed frequency unit
+        - Update the displayed frequency unit
 
-        load_dict is called during init and when the frequency unit or the
-        sampling frequency have been changed.
+        `load_dict()` is called during init and when the frequency unit or the
+          sampling frequency have been changed.
 
         It should be called when `specs_changed` or `data_changed` is emitted
         at another place, indicating that a reload is required.
         """
 
         # recalculate displayed freq spec values for (maybe) changed f_S
         logger.debug("exec load_dict")
@@ -280,15 +277,15 @@
         for i in range(len(self.qlineedit)):
             f_name = str(self.qlineedit[i].objectName()).split(":", 1)
             f_label = f_name[0]
             f_value = fb.fil[0][f_label] * fb.fil[0]['f_S']
 
             if not self.qlineedit[i].hasFocus():
                 # widget has no focus, round the display
-                self.qlineedit[i].setText(params['FMT'].format(f_value))  # TODO: WTF?!
+                self.qlineedit[i].setText(params['FMT'].format(f_value))
             else:
                 # widget has focus, show full precision
                 self.qlineedit[i].setText(str(f_value))
 
 # ------------------------------------------------------------------------
     def _show_entries(self, num_new_labels):
         """
@@ -350,31 +347,25 @@
                    for i in range(self.n_cur_labels)]
         if fb.fil[0]['freq_specs_sort']:
             f_specs.sort()
 
         # Make sure normalized freqs are in the range ]0, 0.5[ and are different
         # by at least MIN_FREQ_STEP
         for i in range(self.n_cur_labels):
-            if f_specs[i] <= MIN_FREQ:
+            if f_specs[i] <= 0:
                 logger.warning(
-                    "Frequencies must be > 0, changed {0} from {1:.4g} to {2:.4g}."
-                    .format(str(self.qlineedit[i].objectName()),
-                            f_specs[i]*fb.fil[0]['f_S'],
-                            (MIN_FREQ + MIN_FREQ_STEP)*fb.fil[0]['f_S']))
-                f_specs[i] = MIN_FREQ + MIN_FREQ_STEP
-
-            if f_specs[i] >= MAX_FREQ:
+                    f"Frequency {str(self.qlineedit[i].objectName())} has to be >= 0")
+                self.qlineedit[i].setProperty("state", 'failed')
+            elif f_specs[i] >= 0.5:
                 logger.warning(
-                    "Frequencies must be < f_S /2, changed {0} from {1:.4g} to {2:.4g}."
-                    .format(str(self.qlineedit[i].objectName()),
-                            f_specs[i]*fb.fil[0]['f_S'],
-                            (MAX_FREQ - MIN_FREQ_STEP)*fb.fil[0]['f_S']))
-                f_specs[i] = MAX_FREQ - MIN_FREQ_STEP
-
-            fb.fil[0][str(self.qlineedit[i].objectName())] = f_specs[i]
+                    f"Frequency {str(self.qlineedit[i].objectName())} has to be < f_S /2.")
+                qstyle_widget(self.qlineedit[i], 'failed')
+            else:
+                fb.fil[0][str(self.qlineedit[i].objectName())] = f_specs[i]
+                qstyle_widget(self.qlineedit[i], 'normal')
 
         # check for (nearly) identical elements:
         _, mult = unique_roots(f_specs, tol=MIN_FREQ_STEP)
         ident = [x for x in mult if x > 1]
         if ident:
             logger.warning("Frequencies must differ by at least {0:.4g}"
                            .format(MIN_FREQ_STEP * fb.fil[0]['f_S']))
```

### Comparing `pyfda-0.7.1/pyfda/input_widgets/freq_units.py` & `pyfda-0.8.0a2/pyfda/input_widgets/freq_units.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 """
 import sys
 from pyfda.libs.compat import (
     QtCore, QWidget, QLabel, QLineEdit, QComboBox, QFrame, QFont, QToolButton,
     QIcon, QVBoxLayout, QHBoxLayout, QGridLayout, pyqtSignal, QEvent)
 
 import pyfda.filterbroker as fb
-from pyfda.libs.pyfda_lib import to_html, safe_eval
-from pyfda.libs.pyfda_qt_lib import qget_cmb_box
+from pyfda.libs.pyfda_lib import to_html, safe_eval, pprint_log
+from pyfda.libs.pyfda_qt_lib import qget_cmb_box, qset_cmb_box, qcmb_box_populate
 from pyfda.pyfda_rc import params  # FMT string for QLineEdit fields, e.g. '{:.3g}'
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 class FreqUnits(QWidget):
@@ -39,127 +39,174 @@
         - `'plt_tUnit'`: time unit as string
         - `'plt_fLabel'`: label for frequency axis
         - `'plt_tLabel'`: label for time axis
 
     """
 
     # class variables (shared between instances if more than one exists)
+    # incoming:
+    sig_rx = pyqtSignal(object)
+    # outgoing: from various and when normalized frequencies have been changed
     sig_tx = pyqtSignal(object)  # outgoing
     from pyfda.libs.pyfda_qt_lib import emit
 
     def __init__(self, parent=None, title="Frequency Units"):
 
         super(FreqUnits, self).__init__(parent)
         self.title = title
         self.spec_edited = False  # flag whether QLineEdit field has been edited
 
+        # combobox tooltip + data / text / tooltip for frequency unit
+        self.cmb_f_unit_items = [
+            "<span>Select whether frequencies are specified w.r.t. the sampling "
+            "frequency " + to_html("f_S", frmt = 'i') + ", to the Nyquist frequency "
+            + to_html("f_Ny = f_S", frmt='i') + "/2 or as absolute values."
+            "'<i>k</i>' specifies frequencies w.r.t. " + to_html("f_S", frmt = 'i') +
+            " but plots graphs over the frequency index <i>k</i>.</span>",
+            ("fs", "f_S", "Relative to sampling frequency, "
+             + to_html("F = f / f_S", frmt='i')),
+            ("fny", "f_Ny", "Relative to Nyquist frequency, "
+             + to_html("F = f / f_Ny", frmt='i')),
+            ("k", "k", "Frequency index " + to_html("k = 0 ... N_FFT - 1", frmt='i')),
+            ("mhz", "mHz", "Absolute sampling frequency in mHz"),
+            ("hz", "Hz", "Absolute sampling frequency in Hz"),
+            ("khz", "kHz", "Absolute sampling frequency in kHz"),
+            ("meghz", "MHz", "Absolute sampling frequency in MHz"),
+            ("ghz", "GHz", "Absolute sampling frequency in GHz")
+        ]
+        self.cmb_f_unit_init = "fs"
+
+        self.cmb_f_range_items = [
+            "Select one- or two-sided spectrum and symmetry around <i>f</i> = 0",
+            ("half", "0...½", "One-sided spectrum"),
+            ("whole", "0...1", "Two-sided spectrum, starting at <i>f</i> = 0"),
+            ("sym", "-½...½", "Two-sided spectrum, symmetrical around <i>f</i> = 0")
+            ]
+        self.cmb_f_range_init = "half"
+
+        # t_units and f_scale have the same index as the f_unit_items
+        self.t_units = ['T_S', 'T_S', '', 'ks', 's', 'ms', r'$\mu$s', 'ns']
+        self.f_scale = [1, 1, 1, 1e-3, 1, 1e3, 1e6, 1e9]
+
         self._construct_UI()
 
+# ------------------------------------------------------------------------------
+    def process_sig_rx(self, dict_sig=None):
+        """
+        Process signals coming from
+        - FFT window widget
+        - qfft_win_select
+        """
+
+        # logger.warning("PROCESS_SIG_RX - vis: {0}\n{1}"
+        #            .format(self.isVisible(), pprint_log(dict_sig)))
+
+        if 'id' in dict_sig and dict_sig['id'] == id(self):
+            logger.debug("Stopped infinite loop")
+            return
+        elif ('view_changed' in dict_sig and dict_sig['view_changed'] == 'f_S')\
+            or 'data_changed' in dict_sig:
+            self.update_UI(emit=False)
+
+# ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Construct the User Interface
         """
         self.layVMain = QVBoxLayout() # Widget main layout
 
-        f_units = ['k','f_S', 'f_Ny', 'Hz', 'kHz', 'MHz', 'GHz']
-        self.t_units = ['', 'T_S', 'T_S', 's', 'ms', r'$\mu$s', 'ns']
-
         bfont = QFont()
         bfont.setBold(True)
 
         self.lblUnits = QLabel(self)
         self.lblUnits.setText("Freq. Unit")
         self.lblUnits.setFont(bfont)
 
-        self.fs_old = fb.fil[0]['f_S']  # store current sampling frequency
+        self.f_s_old = fb.fil[0]['f_S']  # store current sampling frequency
 
-        self.lblF_S = QLabel(self)
-        self.lblF_S.setText(to_html("f_S =", frmt='bi'))
+        self.lbl_f_s = QLabel(self)
+        self.lbl_f_s.setText(to_html("f_S =", frmt='bi'))
 
-        self.ledF_S = QLineEdit()
-        self.ledF_S.setText(str(fb.fil[0]["f_S"]))
-        self.ledF_S.setObjectName("f_S")
-        self.ledF_S.installEventFilter(self)  # filter events
+        self.led_f_s = QLineEdit()
+        self.led_f_s.setText(str(fb.fil[0]["f_S"]))
+        self.led_f_s.setObjectName("f_S")
+        self.led_f_s.installEventFilter(self)  # filter events
 
         self.butLock = QToolButton(self)
         self.butLock.setIcon(QIcon(':/lock-unlocked.svg'))
         self.butLock.setCheckable(True)
         self.butLock.setChecked(False)
         self.butLock.setToolTip(
             "<span><b>Unlocked:</b> When f_S is changed, all frequency related "
             "widgets are updated, normalized frequencies stay the same.<br />"
             "<b>Locked:</b> When f_S is changed, displayed absolute frequency "
             "values don't change but normalized frequencies do.</span>")
-        # self.butLock.setStyleSheet("QToolButton:checked {font-weight:bold}")
 
         layHF_S = QHBoxLayout()
-        layHF_S.addWidget(self.ledF_S)
+        layHF_S.addWidget(self.led_f_s)
         layHF_S.addWidget(self.butLock)
 
-        self.cmbUnits = QComboBox(self)
-        self.cmbUnits.setObjectName("cmbUnits")
-        self.cmbUnits.addItems(f_units)
-        self.cmbUnits.setToolTip(
-        'Select whether frequencies are specified w.r.t. \n'
-        'the sampling frequency "f_S", to the Nyquist frequency \n'
-        'f_Ny = f_S/2 or as absolute values. "k" specifies frequencies w.r.t. f_S '
-        'but plots graphs over the frequency index k.')
-        self.cmbUnits.setCurrentIndex(1)
-#        self.cmbUnits.setItemData(0, (0,QColor("#FF333D"),Qt.BackgroundColorRole))#
-#        self.cmbUnits.setItemData(0, (QFont('Verdana', bold=True), Qt.FontRole)
-
-        fRanges = [("0...½", "half"), ("0...1","whole"), ("-½...½", "sym")]
-        self.cmbFRange = QComboBox(self)
-        self.cmbFRange.setObjectName("cmbFRange")
-        for f in fRanges:
-            self.cmbFRange.addItem(f[0],f[1])
-        self.cmbFRange.setToolTip("Select frequency range (whole or half).")
-        self.cmbFRange.setCurrentIndex(0)
+        self.cmb_f_units = QComboBox(self)
+        self.cmb_f_units.setObjectName("cmb_f_units")
+        qcmb_box_populate(self.cmb_f_units, self.cmb_f_unit_items, self.cmb_f_unit_init)
+#        self.cmb_f_units.setItemData(0, (0,QColor("#FF333D"),Qt.BackgroundColorRole))#
+#        self.cmb_f_units.setItemData(0, (QFont('Verdana', bold=True), Qt.FontRole)
+
+        self.cmb_f_range = QComboBox(self)
+        self.cmb_f_range.setObjectName("cmb_f_range")
+        qcmb_box_populate(self.cmb_f_range, self.cmb_f_range_items,
+                          self.cmb_f_range_init)
 
         # Combobox resizes with longest entry
-        self.cmbUnits.setSizeAdjustPolicy(QComboBox.AdjustToContents)
-        self.cmbFRange.setSizeAdjustPolicy(QComboBox.AdjustToContents)
+        self.cmb_f_units.setSizeAdjustPolicy(QComboBox.AdjustToContents)
+        self.cmb_f_range.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
         self.butSort = QToolButton(self)
         self.butSort.setText("Sort")
         self.butSort.setIcon(QIcon(':/sort-ascending.svg'))
         #self.butDelCells.setIconSize(q_icon_size)
         self.butSort.setCheckable(True)
         self.butSort.setChecked(True)
         self.butSort.setToolTip("Sort frequencies in ascending order when pushed.")
         self.butSort.setStyleSheet("QToolButton:checked {font-weight:bold}")
 
         self.layHUnits = QHBoxLayout()
-        self.layHUnits.addWidget(self.cmbUnits)
-        self.layHUnits.addWidget(self.cmbFRange)
+        self.layHUnits.addWidget(self.cmb_f_units)
+        self.layHUnits.addWidget(self.cmb_f_range)
         self.layHUnits.addWidget(self.butSort)
 
         # Create a gridLayout consisting of QLabel and QLineEdit fields
         # for setting f_S, the units and the actual frequency specs:
         self.layGSpecWdg = QGridLayout()  # sublayout for spec fields
-        self.layGSpecWdg.addWidget(self.lblF_S, 1, 0)
-        # self.layGSpecWdg.addWidget(self.ledF_S,1,1)
+        self.layGSpecWdg.addWidget(self.lbl_f_s, 1, 0)
+        # self.layGSpecWdg.addWidget(self.led_f_s,1,1)
         self.layGSpecWdg.addLayout(layHF_S, 1, 1)
         self.layGSpecWdg.addWidget(self.lblUnits, 0, 0)
         self.layGSpecWdg.addLayout(self.layHUnits, 0, 1)
 
         frmMain = QFrame(self)
         frmMain.setLayout(self.layGSpecWdg)
 
         self.layVMain.addWidget(frmMain)
         self.layVMain.setContentsMargins(*params['wdg_margins'])
 
         self.setLayout(self.layVMain)
 
         #----------------------------------------------------------------------
+        # GLOBAL SIGNALS & SLOTs
+        #----------------------------------------------------------------------
+        self.sig_rx.connect(self.process_sig_rx)
+
+        #----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs
         #----------------------------------------------------------------------
-        self.cmbUnits.currentIndexChanged.connect(self.update_UI)
+        # swallow index passed by "IndexChanged":
+        self.cmb_f_units.currentIndexChanged.connect(lambda: self.update_UI(self))
         self.butLock.clicked.connect(self._lock_freqs)
-        self.cmbFRange.currentIndexChanged.connect(self._freq_range)
+        self.cmb_f_range.currentIndexChanged.connect(self._freq_range)
         self.butSort.clicked.connect(self._store_sort_flag)
         # ----------------------------------------------------------------------
 
         self.update_UI()  # first-time initialization
 
 # -------------------------------------------------------------
     def _lock_freqs(self):
@@ -175,58 +222,68 @@
         When the effect of varying the sampling frequency is to be analyzed, the
         displayed values in the widgets can be locked by pressing the Lock button.
         After changing the sampling frequency, normalized frequencies have to be
         rescaled like `f_a *= fb.fil[0]['f_S_prev'] / fb.fil[0]['f_S']` to maintain
         the displayed value `f_a * f_S`.
 
         This has to be accomplished by each frequency widget (currently, these are
-        freq_specs and freq_units).
+        freq_specs and plot_tran_stim) when receiving the signal {'view_changed': 'f_S'}.
 
-        The setting is stored as bool in the global dict entry `fb.fil[0]['freq_locked'`,
-        the signal 'view_changed':'f_S' is emitted.
+        The setting is stored as bool in the global dict entry `fb.fil[0]['freq_locked'`.
+        No signal is emitted because there is no immediate need for action, all the values
+        remain unchanged.
         """
 
         if self.butLock.isChecked():
             # Lock has been activated, keep displayed frequencies locked
             fb.fil[0]['freq_locked'] = True
             self.butLock.setIcon(QIcon(':/lock-locked.svg'))
         else:
             # Lock has been unlocked, scale displayed frequencies with f_S
             fb.fil[0]['freq_locked'] = False
             self.butLock.setIcon(QIcon(':/lock-unlocked.svg'))
 
-        self.emit({'view_changed': 'f_S'})
-
 # -------------------------------------------------------------
-    def update_UI(self):
+    def update_UI(self, emit=True):
         """
         update_UI is called
         - during init
         - when the unit combobox is changed
+        - when the signal {'view_changed': 'f_S'} has been received. In this case,
+          the UI is updated from the fb.fil[0] dictionary and no signal is emitted.
 
         Set various scale factors and labels depending on the setting of the unit
         combobox.
 
         Update the freqSpecsRange and finally, emit 'view_changed':'f_S' signal
         """
-        f_unit = str(self.cmbUnits.currentText())  # selected frequency unit
-        idx = self.cmbUnits.currentIndex()  # and its index
+        if not emit:  # triggered from outside
+            self.led_f_s.setText(str(fb.fil[0]['f_S']))
+            idx = qset_cmb_box(self.cmb_f_units, fb.fil[0]['freq_specs_unit'],
+                               caseSensitive=True)
+            if idx == -1:
+                logger.warning(
+                    f"Unknown frequency unit {fb.fil[0]['freq_specs_unit']}, "
+                    "using 'f_S'.")
+            qset_cmb_box(self.cmb_f_range, fb.fil[0]['freqSpecsRangeType'],
+                         data=True, fireSignals=True)
+
+        f_unit = qget_cmb_box(self.cmb_f_units, data=False)  # selected frequency unit,
+        idx = self.cmb_f_units.currentIndex()  # its index
+        f_s_scale = self.f_scale[idx]  # and its scaling factor
 
         is_normalized_freq = f_unit in {"f_S", "f_Ny", "k"}
 
-        self.ledF_S.setVisible(not is_normalized_freq)  # only vis. when
-        self.lblF_S.setVisible(not is_normalized_freq)  # not normalized
+        self.led_f_s.setVisible(not is_normalized_freq)  # only vis. when
+        self.lbl_f_s.setVisible(not is_normalized_freq)  # not normalized
         self.butLock.setVisible(not is_normalized_freq)
-        f_S_scale = 1  # default setting for f_S scale
 
         if is_normalized_freq:
             # store current sampling frequency to restore it when returning to
             # unnormalized frequencies
-            self.fs_old = fb.fil[0]['f_S']
-
             if f_unit == "f_S":  # normalized to f_S
                 fb.fil[0]['f_S'] = fb.fil[0]['f_max'] = 1.
                 fb.fil[0]['T_S'] = 1.
                 f_label = r"$F = f\, /\, f_S = \Omega \, /\,  2 \mathrm{\pi} \; \rightarrow$"
                 t_label = r"$n = t\, /\, T_S \; \rightarrow$"
             elif f_unit == "f_Ny":  # normalized to f_nyq = f_S / 2
                 fb.fil[0]['f_S'] = fb.fil[0]['f_max'] = 2.
@@ -236,57 +293,68 @@
             else: # frequency index k,
                 fb.fil[0]['f_S'] = 1.
                 fb.fil[0]['T_S'] = 1.
                 fb.fil[0]['f_max'] = params['N_FFT']
                 f_label = r"$k \; \rightarrow$"
                 t_label = r"$n\; \rightarrow$"
 
-            self.ledF_S.setText(params['FMT'].format(fb.fil[0]['f_S']))
-
         else:  # Hz, kHz, ...
-            # Restore sampling frequency when returning from f_S / f_Ny / k
+            # Restore sampling frequency when user selected an absolute sampling frequency,
+            # returning from f_S / f_Ny / k
             if fb.fil[0]['freq_specs_unit'] in {"f_S", "f_Ny", "k"}:  # previous setting normalized?
-                fb.fil[0]['f_S'] = fb.fil[0]['f_max'] = self.fs_old  # yes, restore prev.
-                fb.fil[0]['T_S'] = 1./self.fs_old  # settings for sampling frequency
-                self.ledF_S.setText(params['FMT'].format(fb.fil[0]['f_S']))
-
-            if f_unit == "Hz":
-                f_S_scale = 1.
-            elif f_unit == "kHz":
-                f_S_scale = 1.e3
-            elif f_unit == "MHz":
-                f_S_scale = 1.e6
-            elif f_unit == "GHz":
-                f_S_scale = 1.e9
+                fb.fil[0]['f_S'] = fb.fil[0]['f_max'] = self.f_s_old  # yes, restore prev. f_S
+
+            # --- try to pick the most suitable unit for f_S --------------
+            f_S = fb.fil[0]['f_S'] * f_s_scale
+            if f_S >= 1e9:
+                f_unit = "GHz"
+            elif f_S >= 1e6:
+                f_unit = "MHz"
+            elif f_S >= 1e3:
+                f_unit = "kHz"
+            elif f_S >= 1:
+                f_unit = "Hz"
             else:
-                logger.warning("Unknown frequency unit {0}".format(f_unit))
+                f_unit = "mHz"
+
+            new_idx = qset_cmb_box(self.cmb_f_units, f_unit, caseSensitive=True)
+            if new_idx != idx:  # sampling frequency needs to be scaled
+                idx = new_idx
+                f_s_scale = self.f_scale[idx]
+                fb.fil[0]['f_S'] = f_S / f_s_scale
+                emit = True
+            # -------------------------------------------------------------
+            self.f_s_old = fb.fil[0]['f_S']
+            self.led_f_s.setText(params['FMT'].format(fb.fil[0]['f_S']))
 
             f_label = r"$f$ in " + f_unit + r"$\; \rightarrow$"
             t_label = r"$t$ in " + self.t_units[idx] + r"$\; \rightarrow$"
 
         if f_unit == "k":
             plt_f_unit = "f_S"
         else:
             plt_f_unit = f_unit
 
-        fb.fil[0].update({'f_S_scale': f_S_scale})  # scale factor for f_S (Hz, kHz, ...)
+        fb.fil[0]['T_S'] = 1./fb.fil[0]['f_S']
+
+        fb.fil[0].update({'f_s_scale': f_s_scale})  # scale factor for f_S (Hz, kHz, ...)
         fb.fil[0].update({'freq_specs_unit': f_unit})  # frequency unit
         # time and frequency unit as string e.g. for plot axis labeling
         fb.fil[0].update({"plt_fUnit": plt_f_unit})
         fb.fil[0].update({"plt_tUnit": self.t_units[idx]})
         # complete plot axis labels including unit and arrow
         fb.fil[0].update({"plt_fLabel": f_label})
         fb.fil[0].update({"plt_tLabel": t_label})
 
         self._freq_range(emit=False)  # update f_lim setting without emitting signal
 
-        self.emit({'view_changed': 'f_S'})
+        if emit:  # UI was updated by user or a rescaling of f_S
+            self.emit({'view_changed': 'f_S'})
 
 # ------------------------------------------------------------------------------
-
     def eventFilter(self, source, event):
 
         """
         Filter all events generated by the QLineEdit `f_S` widget. Source and type
         of all events generated by monitored objects are passed to this eventFilter,
         evaluated and passed on to the next hierarchy level.
 
@@ -309,28 +377,27 @@
                                                    sign='pos')})
                 fb.fil[0].update({'T_S': 1./fb.fil[0]['f_S']})
                 fb.fil[0].update({'f_max': fb.fil[0]['f_S']})
 
                 self._freq_range(emit=False)  # update plotting range
                 self.emit({'view_changed': 'f_S'})
                 self.spec_edited = False  # reset flag, changed entry has been saved
-
+        # ----------------------
         if source.objectName() == 'f_S':
             if event.type() == QEvent.FocusIn:
                 self.spec_edited = False
                 source.setText(str(fb.fil[0]['f_S']))  # full precision
             elif event.type() == QEvent.KeyPress:
                 self.spec_edited = True  # entry has been changed
                 key = event.key()
                 if key in {QtCore.Qt.Key_Return, QtCore.Qt.Key_Enter}:
                     _store_entry()
                 elif key == QtCore.Qt.Key_Escape:  # revert changes
                     self.spec_edited = False
                     source.setText(str(fb.fil[0]['f_S']))  # full precision
-
             elif event.type() == QEvent.FocusOut:
                 _store_entry()
                 source.setText(params['FMT'].format(fb.fil[0]['f_S']))  # reduced prec.
         # Call base class method to continue normal event processing:
         return super(FreqUnits, self).eventFilter(source, event)
 
     # -------------------------------------------------------------
@@ -340,15 +407,15 @@
         or for double-sided spectrum between -f_S/2 and f_S/2
 
         Emit 'view_changed':'f_range' when `emit=True`
         """
         if type(emit) == int:  # signal was emitted by combobox
             emit = True
 
-        rangeType = qget_cmb_box(self.cmbFRange)
+        rangeType = qget_cmb_box(self.cmb_f_range)
 
         fb.fil[0].update({'freqSpecsRangeType': rangeType})
         f_max = fb.fil[0]["f_max"]
 
         if rangeType == 'whole':
             f_lim = [0, f_max]
         elif rangeType == 'sym':
@@ -362,30 +429,30 @@
             self.emit({'view_changed': 'f_range'})
 
     # -------------------------------------------------------------
     def load_dict(self):
         """
         Reload comboBox settings and textfields from filter dictionary
         Block signals during update of combobox / lineedit widgets
+        This is called from `input_specs.load_dict()`
         """
-        self.ledF_S.setText(params['FMT'].format(fb.fil[0]['f_S']))
+        # self.led_f_s.setText(params['FMT'].format(fb.fil[0]['f_S']))
 
-        self.cmbUnits.blockSignals(True)
-        idx = self.cmbUnits.findText(fb.fil[0]['freq_specs_unit'])  # get and set
-        self.cmbUnits.setCurrentIndex(idx)  # index for freq. unit combo box
-        self.cmbUnits.blockSignals(False)
-
-        self.cmbFRange.blockSignals(True)
-        idx = self.cmbFRange.findData(fb.fil[0]['freqSpecsRangeType'])
-        self.cmbFRange.setCurrentIndex(idx)  # set frequency range
-        self.cmbFRange.blockSignals(False)
-
-        self.butSort.blockSignals(True)
-        self.butSort.setChecked(fb.fil[0]['freq_specs_sort'])
-        self.butSort.blockSignals(False)
+        # qset_cmb_box(self.cmb_f_units, fb.fil[0]['freq_specs_unit'])
+        # is_normalized_freq = fb.fil[0]['freq_specs_unit'] in {"f_S", "f_Ny", "k"}
+        # self.led_f_s.setVisible(not is_normalized_freq)  # only vis. when
+        # self.lbl_f_s.setVisible(not is_normalized_freq)  # not normalized
+        # self.butLock.setVisible(not is_normalized_freq)
+
+        # qset_cmb_box(self.cmb_f_range, fb.fil[0]['freqSpecsRangeType'])
+
+        # self.butSort.blockSignals(True)
+        # self.butSort.setChecked(fb.fil[0]['freq_specs_sort'])
+        # self.butSort.blockSignals(False)
+        self.update_UI(emit=False)
 
 # -------------------------------------------------------------
     def _store_sort_flag(self):
         """
         Store sort flag in filter dict and emit 'specs_changed':'f_sort'
         when sort button is checked.
         """
```

### Comparing `pyfda-0.7.1/pyfda/input_widgets/input_coeffs.py` & `pyfda-0.8.0a2/pyfda/input_widgets/input_coeffs.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 from pyfda.libs.compat import (
     Qt, QtCore, QWidget, QLineEdit, QApplication, QIcon, QSize, QTableWidget,
     QTableWidgetItem, QVBoxLayout, pyqtSignal, QStyledItemDelegate, QColor, QBrush)
 import numpy as np
 
 import pyfda.filterbroker as fb  # importing filterbroker initializes all its globals
-from pyfda.libs.pyfda_lib import fil_save, safe_eval
+from pyfda.libs.pyfda_lib import fil_save, safe_eval, pprint_log
 from pyfda.libs.pyfda_qt_lib import (
     qstyle_widget, qset_cmb_box, qget_cmb_box, qget_selected)
-from pyfda.libs.pyfda_io_lib import qtable2text, qtext2table, export_csv_data
+from pyfda.libs.pyfda_io_lib import qtable2text, qtext2table, save_data_csv
 from pyfda.libs.csv_option_box import CSV_option_box
 
 from pyfda.pyfda_rc import params
 
 from .input_coeffs_ui import Input_Coeffs_UI
 
 import logging
@@ -127,25 +127,25 @@
             option.backgroundBrush.setColor(QColor(100, 100, 100, 200))
             # don't continue with default initStyleOption... display routine ends here
         else:
             # continue with the original `initStyleOption()` and call displayText()
             super(ItemDelegate, self).initStyleOption(option, index)
 
     # -------------------------------------------------------------------------
-    def text(self, item):
-        """
-        Return item text as string transformed by self.displayText()
-
-        Used a.o. in `libs.pyfda_fix_lib` as `text += table.itemDelegate().text(item)`
-
-        TODO: Still needed?
-        """
-        dtext = str(self.displayText(item.text(), QtCore.QLocale()))
-        # logger.warning(f"dtext={dtext}")
-        return dtext
+    # def text(self, item):
+    #     """
+    #     Return item text as string transformed by self.displayText()
+
+    #     Used a.o. in `libs.pyfda_fix_lib` as `text += table.itemDelegate().text(item)`
+
+    #     TODO: Still needed?
+    #     """
+    #     dtext = str(self.displayText(item.text(), QtCore.QLocale()))
+    #     # logger.warning(f"dtext={dtext}")
+    #     return dtext
 
     # -------------------------------------------------------------------------
     def displayText(self, text, locale):
         """
         Display `text` with selected fixpoint base and number of places
 
         text:   string / QVariant from QTableWidget to be rendered
@@ -179,20 +179,14 @@
         line_edit = QLineEdit(parent)
         H = int(round(line_edit.sizeHint().height()))
         W = int(round(line_edit.sizeHint().width()))
         line_edit.setMinimumSize(QSize(W, H))  # (160, 25));
 
         return line_edit
 
-#    def updateEditorGeometry(self, editor, option, index):
-#        """
-#        Updates the editor for the item specified by index according to the option given
-#        """
-#        super(ItemDelegate, self).updateEditorGeometry(editor, option, index) # default
-
     # -------------------------------------------------------------------------
     def setEditorData(self, editor, index):
         """
         Pass the data to be edited to the editor:
         - retrieve data with full accuracy from self.ba (in float format)
         - requantize data according to settings in fixpoint object
         - represent it in the selected format (int, hex, ...)
@@ -297,16 +291,16 @@
         self._construct_UI()
 
     # -------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming from sig_rx
         """
-        # logger.debug("process_sig_rx(): vis={0}\n{1}"\
-        #             .format(self.isVisible(), pprint_log(dict_sig)))
+        logger.debug("process_sig_rx(): vis={0}\n{1}"\
+                     .format(self.isVisible(), pprint_log(dict_sig)))
 
         if dict_sig['id'] == id(self):
             # logger.warning(f'Stopped infinite loop: "{first_item(dict_sig)}"')
             return
 
         if 'ui_global_changed' in dict_sig\
                 and dict_sig['ui_global_changed'] == 'csv':
@@ -471,26 +465,26 @@
         self.ui.wdg_wq_coeffs_a.update_disp()
 
 # ------------------------------------------------------------------------------
     def quant_coeffs_save(self):
         """
         - Store selected / all quantized coefficients in `self.ba`
         - Refresh table (for the case that anything weird happens during quantization)
-        - Reset Overflow counters
+        - Reset Overflow flags `self.ba_q[2]` and `self.ba_q[3]`
         - Save quantized `self.ba` to filter dict (in `_save_dict()`). This emits
           {'data_changed': 'input_coeffs'}
         """
         idx = qget_selected(self.tblCoeff)['idx']  # get all selected indices
         # returns e.g. [[0, 0], [0, 6]]
 
         if not idx:  # nothing selected, quantize all elements
             self.ba[0] = self.QObj[0].frmt2float(self.ba_q[0])
             self.ba[1] = self.QObj[1].frmt2float(self.ba_q[1])
-            self.ba_q[2] = np.zeros(len(self.ba_q[2]))
-            self.ba_q[3] = np.zeros(len(self.ba_q[3]))
+            self.ba_q[2] = np.zeros(len(self.ba_q[0]))
+            self.ba_q[3] = np.zeros(len(self.ba_q[1]))
             # idx = [[j, i] for i in range(self.num_rows) for j in range(self.num_cols)]
         else:
             try:
                 idx.remove([1, 0])  # don't process '1' of recursive filters
             except ValueError:
                 pass
             for i in idx:
@@ -545,14 +539,15 @@
             item.setText(str(self.ba_q[col][row]).strip('()'))
         else:  # no, construct it:
             item = QTableWidgetItem(str(self.ba_q[col][row]).strip('()'))
             self.tblCoeff.setItem(row, col, item)
 
         brush = QBrush(Qt.SolidPattern)
         brush.setColor(QColor(255, 255, 255, 0))  # transparent white
+
         if self.ba_q[col + 2][row] > 0:
             # Color item backgrounds with pos. Overflows red
             brush.setColor(QColor(100, 0, 0, 80))
 
         elif self.ba_q[col + 2][row] < 0:
             # Color item backgrounds with neg. Overflows blue
             brush.setColor(QColor(0, 0, 100, 80))
@@ -660,22 +655,22 @@
 
         self.qdict2ui()  # set quantization UI from dictionary
 
         self.refresh_table()
 
         qstyle_widget(self.ui.butSave, 'normal')
 
-    # --------------------------------------------------------------------------
-    def _copy_options(self):
-        """
-        Set options for copying to/from clipboard or file.
-        """
-        self.opt_widget = CSV_option_box(self)  # Handle must be class attribute!
-        # self.opt_widget.show() # modeless dialog, i.e. non-blocking
-        self.opt_widget.exec_()  # modal dialog (blocking)
+    # # --------------------------------------------------------------------------
+    # def _copy_options(self):
+    #     """
+    #     Set options for copying to/from clipboard or file.
+    #     """
+    #     self.opt_widget = CSV_option_box(self)  # Handle must be class attribute!
+    #     # self.opt_widget.show() # modeless dialog, i.e. non-blocking
+    #     self.opt_widget.exec_()  # modal dialog (blocking)
 
     # --------------------------------------------------------------------------
     def _export(self):
         """
         Export data from coefficient table `self.tblCoeff` to clipboard / file in
         CSV format.
         """
@@ -701,15 +696,15 @@
                     text += str(safe_eval(sos_coeffs[r][c], return_type='auto')) + delim
                 text = text.rstrip(delim) + cr
             text = text.rstrip(cr)  # delete last CR
 
             if params['CSV']['clipboard']:
                 fb.clipboard.setText(text)
             else:
-                export_csv_data(self, text, title="Export in CMSIS DSP SOS format",
+                save_data_csv(self, text, title="Export in CMSIS DSP SOS format",
                                 file_types=('csv',))
 
     # --------------------------------------------------------------------------
     def _import(self):
         """
         Import data from clipboard / file and copy it to `self.ba` as float / cmplx.
```

### Comparing `pyfda-0.7.1/pyfda/input_widgets/input_coeffs_ui.py` & `pyfda-0.8.0a2/pyfda/input_widgets/input_coeffs_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,19 +77,17 @@
         Process signals coming from the CSV pop-up window
         """
         # logger.debug("PROCESS_SIG_RX:\n{0}".format(pprint_log(dict_sig)))
 
         if 'closeEvent' in dict_sig:
             self._close_csv_win()
             self.emit({'ui_global_changed': 'csv'})
-            return
         elif 'ui_global_changed' in dict_sig:
             self._set_load_save_icons()  # update icons file <-> clipboard
-            # inform e.g. the p/z input widget about changes in CSV options
-            self.emit({'ui_global_changed': 'csv'})
+            # set state of CSV options button according to state of CSV popup handle
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Intitialize the widget, consisting of:
         - top chkbox row
         - coefficient table
@@ -321,34 +319,32 @@
         self.but_csv_options.clicked.connect(self._open_csv_win)
 
     # --------------------------------------------------------------------------
     def _open_csv_win(self):
         """
         Pop-up window for CSV options
         """
-        if self.but_csv_options.isChecked():
-            qstyle_widget(self.but_csv_options, "changed")
-        else:
-            qstyle_widget(self.but_csv_options, "normal")
+        # if self.but_csv_options.isChecked():
+        #     qstyle_widget(self.but_csv_options, "changed")
+        # else:
+        #     qstyle_widget(self.but_csv_options, "normal")
 
         if dirs.csv_options_handle is None:
             # no handle to the window? Create a new instance
             if self.but_csv_options.isChecked():
                 # Important: Handle to window must be class attribute, otherwise it
                 # (and the attached window) is deleted immediately when it goes
                 # out of scope
                 dirs.csv_options_handle = CSV_option_box(self)
                 dirs.csv_options_handle.sig_tx.connect(self.process_sig_rx)
                 dirs.csv_options_handle.show()  # modeless i.e. non-blocking popup window
-        else:
-            if not self.but_csv_options.isChecked():  # this should not happen
-                if dirs.csv_options_handle is None:
-                    logger.warning("CSV options window is already closed!")
-                else:
-                    dirs.csv_options_handle.close()
+
+        else:  # close window, delete handle
+            dirs.csv_options_handle.close()
+            self.but_csv_options.setChecked(False)
 
         self.emit({'ui_global_changed': 'csv'})
 
     # ------------------------------------------------------------------------------
     def _close_csv_win(self):
         dirs.csv_options_handle = None
         self.but_csv_options.setChecked(False)
@@ -383,20 +379,16 @@
 
             self.butToTable.setIcon(QIcon(':/file.svg'))
             self.butToTable.setToolTip(
                 "<span>Load table from file. Table data format (e.g. 'Hex') has to "
                 "match the data format in the file, otherwise data may be imported "
                 "incorrectly without warning.</span>")
 
-        if dirs.csv_options_handle is None:
-            qstyle_widget(self.but_csv_options, "normal")
-            self.but_csv_options.setChecked(False)
-        else:
-            qstyle_widget(self.but_csv_options, "changed")
-            self.but_csv_options.setChecked(True)
+        # set state of CSV options button according to state of handle
+        self.but_csv_options.setChecked(not dirs.csv_options_handle is None)
 
 
 # ------------------------------------------------------------------------------
 if __name__ == '__main__':
     """ Test with python -m pyfda.input_widgets.input_coeffs_ui """
     import sys
     from pyfda.libs.compat import QApplication
```

### Comparing `pyfda-0.7.1/pyfda/input_widgets/input_fixpoint_specs.py` & `pyfda-0.8.0a2/pyfda/input_widgets/input_fixpoint_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/input_widgets/input_info.py` & `pyfda-0.8.0a2/pyfda/input_widgets/input_info.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/input_widgets/input_info_about.py` & `pyfda-0.8.0a2/pyfda/input_widgets/input_info_about.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                           This info is always visible.
 
         `self.about_str`: OS, user name, directories, versions of installed software
         """
 
         self.info_str = (
             "<b><a href=https://www.github.com/chipmuenk/pyfda>pyfda</a> "
-            f"Version {version.__version__} (c) 2013 - 2022 Christian Münker</b><br />"
+            f"Version {version.__version__} (c) 2013 - 2023 Christian Münker</b><br />"
             "Design, analyze and synthesize digital filters. Docs @ "
             "<a href=https://pyfda.rtfd.org>pyfda.rtfd.org</a>"
             " (<a href=https://media.readthedocs.org/pdf/pyfda/latest/pyfda.pdf>pdf</a>)"
             "<br />")
 
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `pyfda-0.7.1/pyfda/input_widgets/input_pz.py` & `pyfda-0.8.0a2/pyfda/input_widgets/input_pz.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from pyfda.libs.compat import (
     QtCore, QWidget, QLineEdit, pyqtSignal, QEvent, QIcon,
     QBrush, QColor, QSize, QStyledItemDelegate, QApplication,
     QTableWidget, QTableWidgetItem, Qt, QVBoxLayout)
 
 from pyfda.libs.pyfda_qt_lib import qget_cmb_box, qstyle_widget
 from pyfda.libs.pyfda_io_lib import qtable2text, qtext2table
+from pyfda.libs.pyfda_sig_lib import zeros_with_val
 
 import numpy as np
 from scipy.signal import freqz, zpk2tf
 
 import pyfda.filterbroker as fb  # importing filterbroker initializes all its globals
 from pyfda.libs.pyfda_lib import qstr, fil_save, safe_eval, pprint_log
 from pyfda.pyfda_rc import params
@@ -51,51 +52,50 @@
     def __init__(self, parent):
         """
         Pass instance `parent` of parent class (Input_PZ)
         """
         super(ItemDelegate, self).__init__(parent)
         self.parent = parent  # instance of the parent (not the base) class
 
+    # --------------------------------------------------------------------------
     def initStyleOption(self, option, index):
         """
         Initialize `option` with the values using the `index` index. All items are
         passed to the original `initStyleOption()` which then calls `displayText()`.
 
         Afterwards, check whether a pole (index.column() == 1 )is outside the
         UC and color item background accordingly (not implemented yet).
         """
         # continue with the original `initStyleOption()` and call displayText()
         super(ItemDelegate, self).initStyleOption(option, index)
-        # test whether fixpoint conversion during displayText() created an overflow:
+        # test for poles with magnitude > 1
         if index.column() == 1 and False:
-            # Color item backgrounds with pos. Overflows red
+            # Color item backgrounds with poles outside the UC red
             option.backgroundBrush = QBrush(Qt.SolidPattern)
             option.backgroundBrush.setColor(QColor(100, 0, 0, 80))
 
-    def text(self, item):
-        """
-        Return item text as string transformed by self.displayText()
-        """
-        # return qstr(item.text()) # convert to "normal" string
-        return qstr(self.displayText(item.text(), QtCore.QLocale()))
+    # --------------------------------------------------------------------------
+    # def text(self, item):
+    #     """
+    #     Return item text as string transformed by self.displayText()
+    #     """
+    #     return qstr(self.displayText(item.text(), QtCore.QLocale()))
 
+    # --------------------------------------------------------------------------
     def displayText(self, text, locale):
         """
         Display `text` with selected format (cartesian / polar)
         and number of places
 
         text:   string / QVariant from QTableWidget to be rendered
         locale: locale for the text
         """
-
         return self.parent.cmplx2frmt(text, places=params['FMT_pz'])
-        # r, phi = np.absolute(data), np.angle(data, deg=False)
-        # return "{0:.{2}g} * {3}{1:.{2}g} rad".format(r, phi, params['FMT_pz'],
-        #    self.angle_char)
 
+    # --------------------------------------------------------------------------
     def createEditor(self, parent, options, index):
         """
         Neet to set editor explicitly, otherwise QDoubleSpinBox instance is
         created when space is not sufficient?!
         editor:  instance of e.g. QLineEdit (default)
         index:   instance of QModelIndex
         options: instance of QStyleOptionViewItemV4
@@ -103,28 +103,29 @@
         line_edit = QLineEdit(parent)
         H = int(round(line_edit.sizeHint().height()))
         W = int(round(line_edit.sizeHint().width()))
         line_edit.setMinimumSize(QSize(W, H))  # (160, 25));
 
         return line_edit
 
+    # --------------------------------------------------------------------------
     def setEditorData(self, editor, index):
         """
         Pass the data to be edited to the editor:
         - retrieve data with full accuracy (`places=-1`) from `zpk` (in float format)
         - represent it in the selected format (Cartesian, polar, ...)
 
         editor: instance of e.g. QLineEdit
         index:  instance of QModelIndex
         """
-#        data = qstr(index.data()) # get data from QTableWidget
         data = self.parent.zpk[index.column()][index.row()]
-        data_str = self.parent.cmplx2frmt(data, places=-1)  # qstr(safe_eval(data, return_type="auto"))
+        data_str = self.parent.cmplx2frmt(data, places=-1)
         editor.setText(data_str)
 
+    # --------------------------------------------------------------------------
     def setModelData(self, editor, model, index):
         """
         When editor has finished, read the updated data from the editor,
         convert it to complex format and store it in both the model
         (= QTableWidget) and in `zpk`. Finally, refresh the table item to
         display it in the selected format (via `to be defined`) and normalize
         the gain.
@@ -147,36 +148,15 @@
                                       self.parent.zpk[index.column()][index.row()])
         model.setData(index, data)                          # store in QTableWidget
         self.parent.zpk[index.column()][index.row()] = data  # and in self.ba
         qstyle_widget(self.parent.ui.butSave, 'changed')
         self.parent._refresh_table_item(index.row(), index.column())  # refresh table entry
         self.parent._normalize_gain()  # recalculate gain
 
-
-class ItemDelegateAnti(QStyledItemDelegate):
-    """
-    The following methods are subclassed to replace display and editor of the
-    QTableWidget.
-
-    `displayText()` displays number with n_digits without sacrificing precision of
-    the data stored in the table.
-    """
-    def __init__(self, parent):
-        """
-        Pass instance `parent` of parent class (Input_PZ)
-        """
-        super(ItemDelegateAnti, self).__init__(parent)
-        self.parent = parent  # instance of the parent (not the base) class
-
-    def displayText(self, text, locale):
-        return "{:.{n_digits}g}".format(safe_eval(qstr(text), return_type='cmplx'),
-                                        n_digits=params['FMT_pz'])
-
-
-# ------------------------------------------------------------------------------
+# ===================================================================================
 class Input_PZ(QWidget):
     """
     Create the window for entering exporting / importing and saving / loading data
     """
     sig_rx = pyqtSignal(object)  # incoming from input_tab_widgets
     sig_tx = pyqtSignal(object)  # emitted when filter has been saved
     from pyfda.libs.pyfda_qt_lib import emit
@@ -184,37 +164,33 @@
     def __init__(self, parent=None):
         super(Input_PZ, self).__init__(parent)
 
         self.data_changed = True  # initialize flag: filter data has been changed
 
         self.Hmax_last = 1  # initial setting for maximum gain
         self.angle_char = "\u2220"
+        self.pi_char = "pi" # "\u03C0" looks ugly
 
         self.tab_label = "P/Z"
         self.tool_tip = "Display and edit filter poles and zeros."
 
-        self.ui = Input_PZ_UI(self)  # create the UI part with buttons etc.
+        self.ui = Input_PZ_UI(self)  # create the UI control part
         self.norm_last = qget_cmb_box(self.ui.cmbNorm, data=False)  # initial setting of cmbNorm
         self._construct_UI()  # construct the rest of the UI
 
-        self.load_dict()  # initialize table from filterbroker
-        self._refresh_table()  # initialize table with values
-
-        self.setup_signal_slot()  # setup signal-slot connections and eventFilters
-
 # ------------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming from sig_rx
         """
         # logger.debug(f"SIG_RX - data_changed = {self.data_changed}, vis = "
         #              f"{self.isVisible()}\n{pprint_log(dict_sig)}")
-    
+
         if dict_sig['id'] == id(self):
-            logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
+            # logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
             return
 
         if 'ui_global_changed' in dict_sig and dict_sig['ui_global_changed'] == 'csv':
             self.ui._set_load_save_icons()
             # self.emit(dict_sig)
 
         elif self.isVisible():
@@ -225,15 +201,16 @@
             # TODO: draw wouldn't be necessary for 'view_changed', only update view
             if 'data_changed' in dict_sig:
                 self.data_changed = True
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
-        Intitialize the widget
+        Construct the UI from the table widget and the control part (`self.ui`),
+        initialize the widget and setup signal-slot connections and event filters
         """
         self.tblPZ = QTableWidget(self)
 #        self.tblPZ.setEditTriggers(QTableWidget.AllEditTriggers) # make everything editable
         self.tblPZ.setAlternatingRowColors(True)  # alternating row colors)
         self.tblPZ.setObjectName("tblPZ")
 
         # highlight when selected:
@@ -251,18 +228,17 @@
         layVMain.addWidget(self.ui)
         layVMain.addWidget(self.tblPZ)
 
         layVMain.setContentsMargins(*params['wdg_margins'])
 
         self.setLayout(layVMain)
 
-    def setup_signal_slot(self):
-        """
-        Setup setup signal-slot connections
-        """
+        self.load_dict()  # initialize table from filterbroker
+        self._refresh_table()  # initialize table with values
+
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         self.sig_rx.connect(self.process_sig_rx)
         self.ui.sig_tx.connect(self.sig_tx)
 
         # ----------------------------------------------------------------------
@@ -294,16 +270,15 @@
         # Every time a table item is edited, call self._copy_item to copy the
         # item content to self.zpk. This is triggered by the itemChanged signal.
         # The event filter monitors the focus of the input fields.
 
         # signal itemChanged is also triggered programmatically,
         # itemSelectionChanged is only triggered when entering cell
 
-# ------------------------------------------------------------------------------
-
+    # ------------------------------------------------------------------------------
     def eventFilter(self, source, event):
         """
         Filter all events generated by the QLineEdit widgets. Source and type
         of all events generated by monitored objects are passed to this eventFilter,
         evaluated and passed on to the next hierarchy level.
 
         - When a QLineEdit widget gains input focus (`QEvent.FocusIn`), display
@@ -337,23 +312,23 @@
             elif event.type() == QEvent.FocusOut:  # 9
                 self._store_gain(source)
                 self._restore_gain(source)  # display in desired format
                 return True
 
         return super(Input_PZ, self).eventFilter(source, event)
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _store_gain(self, source):
         """
         When the textfield of `source` has been edited (flag `self.spec_edited` =  True),
         store it in the shadow dict. This is triggered by `QEvent.focusOut` or
         RETURN key.
         """
         if self.spec_edited:
-            self.zpk[2] = safe_eval(source.text(), alt_expr=str(self.zpk[2]))
+            self.zpk[2][0] = safe_eval(source.text(), alt_expr=str(self.zpk[2][0]))
             qstyle_widget(self.ui.butSave, 'changed')
             self.spec_edited = False  # reset flag
 
 # ------------------------------------------------------------------------------
     def _normalize_gain(self):
         """
         Normalize the gain factor so that the maximum of |H(f)| stays 1 or a
@@ -362,81 +337,82 @@
         Called by setModelData() and when cmbNorm is activated
 
         """
         norm = qget_cmb_box(self.ui.cmbNorm, data=False)
         self.ui.ledGain.setEnabled(norm == 'None')
         if norm != self.norm_last:
             qstyle_widget(self.ui.butSave, 'changed')
-        if not np.isfinite(self.zpk[2]):
-            self.zpk[2] = 1.
-        self.zpk[2] = np.real_if_close(self.zpk[2]).item()
-        if np.iscomplex(self.zpk[2]):
+        if not np.isfinite(self.zpk[2][0]):
+            self.zpk[2][0] = 1.
+        self.zpk[2][0] = np.real_if_close(self.zpk[2][0]).item()
+        if np.iscomplex(self.zpk[2][0]):
             logger.warning("Casting complex to real for gain k!")
-            self.zpk[2] = np.abs(self.zpk[2])
+            self.zpk[2][0] = np.abs(self.zpk[2][0])
 
         if norm != "None":
-            b, a = zpk2tf(self.zpk[0], self.zpk[1], self.zpk[2])
+            b, a = zpk2tf(self.zpk[0], self.zpk[1], self.zpk[2][0])
             [w, H] = freqz(b, a, whole=True)
             Hmax = max(abs(H))
             if not np.isfinite(Hmax) or Hmax > 1e4 or Hmax < 1e-4:
                 Hmax = 1.
             if norm == "1":
-                self.zpk[2] = self.zpk[2] / Hmax  # normalize to 1
+                self.zpk[2][0] = self.zpk[2][0] / Hmax  # normalize to 1
             elif norm == "Max":
                 if norm != self.norm_last:  # setting has been changed -> 'Max'
                     self.Hmax_last = Hmax  # use current design to set Hmax_last
-                self.zpk[2] = self.zpk[2] / Hmax * self.Hmax_last
+                self.zpk[2][0] = self.zpk[2][0] / Hmax * self.Hmax_last
         self.norm_last = norm  # store current setting of combobox
 
         self._restore_gain()
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _restore_gain(self, source=None):
         """
         Update QLineEdit with either full (has focus) or reduced precision (no focus)
 
         Called by eventFilter, _normalize_gain() and _refresh_table()
         """
 
         if self.ui.butEnable.isChecked():
-            if len(self.zpk) == 3:
+            if len(self.zpk) == 3:  # number of rows
                 pass
             elif len(self.zpk) == 2:  # k is missing in zpk:
-                self.zpk.append(1.)  # use k = 1
+                self.zpk.append(zeros_with_val(len(self.zpk[0])))  # add a row with k = 1
             else:
-                logger.error("P/Z list zpk has wrong length {0}".format(len(self.zpk)))
+                logger.error(f"P/Z array 'self.zpk' has wrong number of rows = {len(self.zpk)}")
+                logger.error(self.zpk)
 
-            k = safe_eval(self.zpk[2], return_type='auto')
+            k = safe_eval(self.zpk[2][0], return_type='auto')
 
             if not self.ui.ledGain.hasFocus():  # no focus, round the gain
                 self.ui.ledGain.setText(str(params['FMT'].format(k)))
             else:  # widget has focus, show gain with full precision
                 self.ui.ledGain.setText(str(k))
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _refresh_table_item(self, row, col):
         """
         Refresh the table item with the index `row, col` from self.zpk
         """
         item = self.tblPZ.item(row, col)
         if item:  # does item exist?
             item.setText(str(self.zpk[col][row]).strip('()'))
         else:  # no, construct it:
             self.tblPZ.setItem(row, col, QTableWidgetItem(
                   str(self.zpk[col][row]).strip('()')))
         self.tblPZ.item(row, col).setTextAlignment(Qt.AlignRight | Qt.AlignCenter)
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _refresh_table(self):
         """
         (Re-)Create the displayed table from self.zpk with the
         desired number format.
 
         TODO:
-        Update zpk[2]?
+        Update zpk[2][0]?
 
         Called by: load_dict(), _clear_table(), _zero_PZ(), _delete_cells(),
                 add_row(), _import()
         """
 
         params['FMT_pz'] = int(self.ui.spnDigits.text())
 
@@ -445,31 +421,30 @@
         if self.ui.butEnable.isChecked():
 
             self.ui.butEnable.setIcon(QIcon(':/circle-check.svg'))
 
             self._restore_gain()
 
             self.tblPZ.setHorizontalHeaderLabels(["Zeros", "Poles"])
-            self.tblPZ.setRowCount(max(len(self.zpk[0]), len(self.zpk[1])))
+            self.tblPZ.setRowCount(len(self.zpk[0]))
 
             self.tblPZ.blockSignals(True)
             for col in range(2):
                 for row in range(len(self.zpk[col])):
                     self._refresh_table_item(row, col)
-
             self.tblPZ.blockSignals(False)
 
             self.tblPZ.resizeColumnsToContents()
             self.tblPZ.resizeRowsToContents()
             self.tblPZ.clearSelection()
 
         else:  # disable widgets
             self.ui.butEnable.setIcon(QIcon(':/circle-x.svg'))
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def load_dict(self):
         """
         Load all entries from filter dict fb.fil[0]['zpk'] into the Zero/Pole/Gain list
         self.zpk and update the display via `self._refresh_table()`.
         The explicit np.array( ... ) statement enforces a deep copy of fb.fil[0],
         otherwise the filter dict would be modified inadvertedly. `dtype=object`
         needs to be specified to create a numpy array from the nested lists with
@@ -477,28 +452,52 @@
 
         "Creating an ndarray from ragged nested sequences (which is a list-or-tuple of
         lists-or-tuples-or ndarrays with different lengths or shapes) is deprecated."
 
         The filter dict fb.fil[0]['zpk'] is a list of numpy float ndarrays for z / p / k
         values `self.zpk` is an array of float ndarrays with different lengths of
         z / p / k subarrays to allow adding / deleting items.
+
+        Format is: [array[zeros, ...], array[poles, ...], k]
         """
-        self.zpk = np.array(fb.fil[0]['zpk'], dtype=object)  # this enforces a deep copy
+        if not type(fb.fil[0]['zpk']) is np.ndarray:
+            logger.warning(f"fb.fil[0]['zpk'] is of type {type(fb.fil[0]['zpk'])} "
+                           f"with len = {len(fb.fil[0]['zpk'])}")
+
+        zpk = list(fb.fil[0]['zpk'])
+
+        if len(zpk) == 3:  # number of rows
+            if np.isscalar(zpk[2]):
+                logger.warning("Gain is scalar, converting to proper format!")
+                zpk[2] = zeros_with_val(len(zpk[0]), zpk[2])  # add a row gain
+            elif len(zpk[2]) != len(zpk[0]):
+                zpk[2] = zeros_with_val(len(zpk[0]), zpk[2][0])
+        elif len(zpk) == 2:  # k is missing in zpk:
+            zpk.append(zeros_with_val(len(zpk[0])))  # add a row with k = 1
+        else:
+            logger.error("P/Z array 'fb.fil[0]['zpk']' has wrong number of "
+                         f"rows = {len(zpk)}")
+            logger.error(zpk)
+            return
+
+        if len(zpk[0]) != len(zpk[1]):
+            logger.warning("fb.fil[0]['zpk'] has differing row lengths, "
+                           f"{len(fb.fil[0]['zpk'][0])} != {len(fb.fil[0]['zpk'][1])}")
+            return
+        # logger.warning(f"New shape (zpk) = {np.shape(zpk)}")
+        self.zpk = np.array(zpk)  # this enforces a deep copy
         qstyle_widget(self.ui.butSave, 'normal')
         self._refresh_table()
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _save_entries(self):
         """
         Save the values from self.zpk to the filter PZ dict,
         the QLineEdit for setting the gain has to be treated separately.
         """
-
-        logger.debug("_save_entries called")
-
         fb.fil[0]['N'] = len(self.zpk[0])
         if np.any(self.zpk[1]):  # any non-zero poles?
             fb.fil[0]['fc'] = 'Manual_IIR'
         else:
             fb.fil[0]['fc'] = 'Manual_FIR'
 
         try:
@@ -512,33 +511,30 @@
             self.load_dict()  # only needed for stand-alone test
 
         self.emit({'data_changed': 'input_pz'})
         # -> input_tab_widgets
 
         qstyle_widget(self.ui.butSave, 'normal')
 
-        logger.debug("b,a = {0}\n\n"
-                     "zpk = {1}\n"
-                     .format(pformat(fb.fil[0]['ba']), pformat(fb.fil[0]['zpk'])
-                             ))
+        logger.debug(f"b,a = {fb.fil[0]['ba']}\n\n"
+                     f"zpk = {pformat(fb.fil[0]['zpk'])}\n")
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _clear_table(self):
         """
         Clear & initialize table and zpk for two poles and zeros @ origin,
         P = Z = [0; 0], k = 1
         """
-        self.zpk = np.array([[0, 0], [0, 0], 1], dtype=object)
+        self.zpk = np.array([[0, 0], [0, 0], [1, 0]])
         self.Hmax_last = 1.0
-        self.anti = False
 
         qstyle_widget(self.ui.butSave, 'changed')
         self._refresh_table()
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _get_selected(self, table):
         """
         get selected cells and return:
         - indices of selected cells
         - selected colums
         - selected rows
         - current cell
@@ -549,77 +545,82 @@
         cols = sorted(list({i[0] for i in idx}))
         rows = sorted(list({i[1] for i in idx}))
         cur = (table.currentColumn(), table.currentRow())
         # cur_idx_row = table.currentIndex().row()
 
         return {'idx': idx, 'cols': cols, 'rows': rows, 'cur': cur}
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _delete_cells(self):
         """
         Delete all selected elements by:
         - determining the indices of all selected cells in the P and Z arrays
         - deleting elements with those indices
         - equalizing the lengths of P and Z array by appending the required
           number of zeros.
         - deleting all P/Z pairs
         Finally, the table is refreshed from self.zpk.
         """
-        sel = self._get_selected(self.tblPZ)['idx']  # get all selected indices
-        Z = [s[1] for s in sel if s[0] == 0]  # all selected indices in 'Z' column
-        P = [s[1] for s in sel if s[0] == 1]  # all selected indices in 'P' column
+        sel = self._get_selected(self.tblPZ)['idx']  # get all selected indices as 2D list
+        sel_z = [s[1] for s in sel if s[0] == 0]  # list with selected indices in 'Z' column
+        sel_p = [s[1] for s in sel if s[0] == 1]  # list with selected indices in 'P' column
+
+        k = self.zpk[2][0]
 
         # Delete array entries with selected indices. If nothing is selected
         # (Z and P are empty), delete the last row.
-        if len(Z) < 1 and len(P) < 1:
-            Z = [len(self.zpk[0])-1]
-            P = [len(self.zpk[1])-1]
-        self.zpk[0] = np.delete(self.zpk[0], Z)
-        self.zpk[1] = np.delete(self.zpk[1], P)
+        if len(sel_z) < 1 and len(sel_p) < 1:
+            sel_z = [len(self.zpk[0])-1]
+            sel_p = [len(self.zpk[1])-1]
+        zeros = np.delete(self.zpk[0], sel_z)
+        poles = np.delete(self.zpk[1], sel_p)
 
         # test and equalize if P and Z array have different lengths:
-        D = len(self.zpk[0]) - len(self.zpk[1])
+        D = len(zeros) - len(poles)
         if D > 0:
-            self.zpk[1] = np.append(self.zpk[1], np.zeros(D))
+            poles = np.append(poles, np.zeros(D))
         elif D < 0:
-            self.zpk[0] = np.append(self.zpk[0], np.zeros(-D))
+            zeros = np.append(zeros, np.zeros(-D))
+
+        gain = zeros_with_val(max(len(poles), len(zeros)), k)
+
+        # reconstruct array with new number of rows
+        self.zpk = np.array([zeros, poles, gain])
 
         self._delete_PZ_pairs()
         self._normalize_gain()
         qstyle_widget(self.ui.butSave, 'changed')
         self._refresh_table()
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _add_rows(self):
         """
         Add the number of selected rows to the table and fill new cells with
         zeros. If nothing is selected, add one row.
         """
         row = self.tblPZ.currentRow()
         sel = len(self._get_selected(self.tblPZ)['rows'])
-        # TODO: evaluate and create non-contiguous selections as well?
 
         if sel == 0:  # nothing selected ->
             sel = 1  # add at least one row ...
-            row = min(len(self.zpk[0]), len(self.zpk[1]))  # ... at the bottom
+            row = len(self.zpk[0]) # ... at the bottom
 
-        self.zpk[0] = np.insert(self.zpk[0], row, np.zeros(sel))
-        self.zpk[1] = np.insert(self.zpk[1], row, np.zeros(sel))
+        self.zpk = np.insert(self.zpk, row, np.zeros((sel, 1)), axis=1)
 
         self._refresh_table()
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _set_eps(self):
         """
         Set tolerance value
         """
         self.ui.eps = safe_eval(self.ui.ledEps.text(), alt_expr=self.ui.eps, sign='pos')
         self.ui.ledEps.setText(str(self.ui.eps))
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _zero_PZ(self):
         """
         Set all P/Zs = 0 with a magnitude less than eps and delete P/Z pairs
         afterwards.
         """
         changed = False
         targ_val = 0.
@@ -649,131 +650,153 @@
 
         self._delete_PZ_pairs()
         self._normalize_gain()
         if changed:
             qstyle_widget(self.ui.butSave, 'changed')  # mark save button as changed
         self._refresh_table()
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def _delete_PZ_pairs(self):
         """
         Find and delete pairs of poles and zeros in self.zpk
         The filter dict and the table have to be updated afterwards.
         """
-        for z in range(len(self.zpk[0])-1, -1, -1):  # start at the bottom
-            for p in range(len(self.zpk[1])-1, -1, -1):
-                if np.isclose(self.zpk[0][z], self.zpk[1][p], rtol=0, atol=self.ui.eps):
-                    self.zpk[0] = np.delete(self.zpk[0], z)
-                    self.zpk[1] = np.delete(self.zpk[1], p)
+        zeros = self.zpk[0]
+        poles = self.zpk[1]
+        gain = self.zpk[2]
+        changed = False
+        for z in range(len(zeros)-1, -1, -1):  # start at the bottom
+            for p in range(len(poles)-1, -1, -1):
+                if np.isclose(zeros[z], poles[p], rtol=0, atol=self.ui.eps):
+                    # zeros / poles to be deleted have values != 0, mark as changed
+                    if zeros[z] != 0 and poles[p] != 0:
+                        changed = True
+                    zeros = np.delete(zeros, z)
+                    poles = np.delete(poles, p)
+                    gain = np.delete(gain, -1)  # delete last element (= 0)
                     break  # ... out of loop
 
-        if len(self.zpk[0]) < 1:  # no P / Z, add 1 row
-            self.zpk[0] = np.append(self.zpk[0], 0.)
-            self.zpk[1] = np.append(self.zpk[1], 0.)
+        if len(zeros) < 1:  # no P / Z, add 1 row
+            zeros = [0]
+            poles = [0]
+            gain = [1]
+
+        self.zpk = np.array((zeros, poles, gain))
+
+        if changed:
+            qstyle_widget(self.ui.butSave, 'changed')  # mark save button as changed
 
     # ------------------------------------------------------------------------------
     def cmplx2frmt(self, text, places=-1):
         """
         Convert number "text" (real or complex or string) to the format defined
         by cmbPZFrmt.
 
         Returns:
             string
         """
         # convert to "normal" string and prettify via safe_eval:
-        data = safe_eval(qstr(text), return_type='auto')
+        data = safe_eval(text, return_type='auto')
         frmt = qget_cmb_box(self.ui.cmbPZFrmt)  # get selected format
-
+        # logger.warning(f"{text} -> {data}")
         if places == -1:
             full_prec = True
         else:
             full_prec = False
 
         if frmt == 'cartesian' or not (type(data) == complex):
             if full_prec:
                 return "{0}".format(data)
             else:
                 return "{0:.{plcs}g}".format(data, plcs=places)
 
         elif frmt == 'polar_rad':
             r, phi = np.absolute(data), np.angle(data, deg=False)
             if full_prec:
-                return "{r} * {angle_char}{p} rad"\
-                    .format(r=r, p=phi, angle_char=self.angle_char)
+                return f"{r} {self.angle_char}{phi} rad"
             else:
-                return "{r:.{plcs}g} * {angle_char}{p:.{plcs}g} rad"\
+                return "{r:.{plcs}g} {angle_char}{p:.{plcs}g} rad"\
                     .format(r=r, p=phi, plcs=places, angle_char=self.angle_char)
 
         elif frmt == 'polar_deg':
             r, phi = np.absolute(data), np.angle(data, deg=True)
             if full_prec:
-                return "{r} * {angle_char}{p}°"\
-                    .format(r=r, p=phi, angle_char=self.angle_char)
+                return f"{r} {self.angle_char}{phi}°"
             else:
-                return "{r:.{plcs}g} * {angle_char}{p:.{plcs}g}°"\
+                return "{r:.{plcs}g} {angle_char}{p:.{plcs}g}°"\
                     .format(r=r, p=phi, plcs=places, angle_char=self.angle_char)
 
         elif frmt == 'polar_pi':
             r, phi = np.absolute(data), np.angle(data, deg=False) / np.pi
             if full_prec:
-                return "{r} * {angle_char}{p} pi"\
-                    .format(r=r, p=phi, angle_char=self.angle_char)
+                return f"{r} {self.angle_char}{phi} {self.pi_char}"
             else:
-                return "{r:.{plcs}g} * {angle_char}{p:.{plcs}g} pi"\
-                    .format(r=r, p=phi, plcs=places, angle_char=self.angle_char)
+                return "{r:.{plcs}g} {angle_char}{p:.{plcs}g} {pi_char}"\
+                    .format(r=r, p=phi, plcs=places, angle_char=self.angle_char,
+                            pi_char=self.pi_char)
 
         else:
             logger.error("Unknown format {0}.".format(frmt))
 
     # ------------------------------------------------------------------------------
-    def frmt2cmplx(self, text, default=0.):
+    def frmt2cmplx(self, string, default=0.):
         """
-        Convert format defined by cmbPZFrmt to real or complex
+        Convert string to real or complex, try to find out the format (cartesian,
+        polar with various angle formats)
         """
-        conv_error = False
-        text = qstr(text).replace(" ", "")  # convert to "proper" string without blanks
+        def str2angle_rad(string: str) -> float:
+            """
+            Try to convert `string` to a corresponding angle in rad
+                Use the following regular expressions:
+                - '$' : matches the end of the string
+                - '|' : combine multiple matches with OR
+            """
+            if re.search('°$|o$', string):
+                # "°" in polar_str[1] or "o" in polar_str[1]:
+                scale = np.pi / 180.  # angle in degrees
+                string = re.sub('o|°', '', string)
+            elif re.search('π$|pi$|p$', string):
+                scale = np.pi
+                string = re.sub('π$|pi$|p$', '', string)
+            else:
+                scale = 1.  # angle in rad
+                string = re.sub('rad', '', string)
+
+            phi = safe_eval(string) * scale
+            return phi
+        # -------------------------------------------
+
+        string = str(string).replace(" ", "")  # remove all blanks
         if qget_cmb_box(self.ui.cmbPZFrmt) == 'cartesian':
-            return safe_eval(text, default, return_type='auto')
+            return safe_eval(string, default, return_type='auto')
         else:
-            # try to split text string at "*<" or the angle character
-            polar_str = text.replace(self.angle_char, '<').split('*<', 1)
-
-            if len(polar_str) < 2:  # input is real or imaginary
-                # remove special characters
-                r = safe_eval(
-                    re.sub('['+self.angle_char+'<∠°]', '', text), default,
-                    return_type='auto')
+            # convert angle character to "<" and try to split string at "*<"
+            # When the "<" character is not found, this returns a list with 1 item!
+            polar_str = string.replace(self.angle_char, '<').replace('*', '')
+            polar_str = polar_str.split('<', 1)
+
+            if len(polar_str) == 2 and polar_str[0] == "": # pure angle
+                phi = str2angle_rad(polar_str[1])
+                x = np.cos(phi)
+                y = np.sin(phi)
+            elif len(polar_str) == 1:  # no angle found; real / imag / cartesian complex
+                r = safe_eval(string, default, return_type='auto')
                 x = r.real
                 y = r.imag
-            else:
+            else:  # r and angle found
                 r = safe_eval(polar_str[0], sign='pos')
-                if safe_eval.err > 0:
-                    conv_error = True
+                phi = str2angle_rad(polar_str[1])
 
-                if "°" in polar_str[1]:
-                    scale = np.pi / 180.  # angle in degrees
-                elif re.search('π$|pi$', polar_str[1]):
-                    scale = np.pi
-                else:
-                    scale = 1.  # angle in rad
-
-                # remove right-most special characters (regex $)
-                polar_str[1] = re.sub(
-                    '['+self.angle_char+'<∠°π]$|rad$|pi$', '', polar_str[1])
-                phi = safe_eval(polar_str[1]) * scale
-                if safe_eval.err > 0:
-                    conv_error = True
-
-                if not conv_error:
-                    x = r * np.cos(phi)
-                    y = r * np.sin(phi)
-                else:
-                    x = default.real
-                    y = default.imag
-                    logger.error("Expression {0} could not be evaluated.".format(text))
+                x = r * np.cos(phi)
+                y = r * np.sin(phi)
+
+            if safe_eval.err > 0:
+                x = default.real
+                y = default.imag
+                logger.warning(f"Expression {string} could not be evaluated.")
             return x + 1j * y
 
     # --------------------------------------------------------------------------
     def _export(self):
         """
         Export data from coefficient table `self.tblCoeff` to clipboard in CSV format
         or to file using a selected format
@@ -801,60 +824,59 @@
             num_rows = len(data_str)
             num_cols = 1
             orientation_horiz = False
         else:
             logger.error("Imported data is a single value or None.")
             return None
         logger.debug("_import: c x r:", num_cols, num_rows)
+        zpk = [[], [], []]
         if orientation_horiz:
-            self.zpk = [[], []]
             for c in range(num_cols):
-                self.zpk[0].append(conv(data_str[c][0]))
+                zpk[0].append(conv(data_str[c][0]))
                 if num_rows > 1:
-                    self.zpk[1].append(conv(data_str[c][1]))
+                    zpk[1].append(conv(data_str[c][1]))
+                if num_rows > 2:
+                    zpk[2].append(conv(data_str[c][2]))
         else:
-            self.zpk[0] = [conv(s) for s in data_str[0]]
-            if num_cols > 1:
-                self.zpk[1] = [conv(s) for s in data_str[1]]
-            else:
-                self.zpk[1] = [1]
-
-        self.zpk[0] = np.asarray(self.zpk[0])
-        self.zpk[1] = np.asarray(self.zpk[1])
+            zpk[0] = [conv(s) for s in data_str[0]]
+            if num_cols == 1:
+                zpk[1] = [1]
+            elif num_cols > 1:
+                zpk[1] = [conv(s) for s in data_str[1]]
+            if num_cols > 2:
+                zpk[2] = [conv(s) for s in data_str[2]]
 
-        self._equalize_columns()
-        qstyle_widget(self.ui.butSave, 'changed')
-        self._refresh_table()
 
-# ------------------------------------------------------------------------------
-    def _equalize_columns(self):
-        """
-        test and equalize if P and Z subarray have different lengths:
-        """
+        # test and equalize if P and Z lists have different lengths:
         try:
-            p_len = len(self.zpk[1])
+            p_len = len(zpk[1])
         except IndexError:
             p_len = 0
-
         try:
-            z_len = len(self.zpk[0])
+            z_len = len(zpk[0])
         except IndexError:
             z_len = 0
 
         D = z_len - p_len
-
         if D > 0:  # more zeros than poles
-            self.zpk[1] = np.append(self.zpk[1], np.zeros(D))
+            zpk[1] = np.append(self.zpk[1], np.zeros(D))
         elif D < 0:  # more poles than zeros
-            self.zpk[0] = np.append(self.zpk[0], np.zeros(-D))
-#            if fb.fil[0]['ft'] == 'IIR':
-#                self.zpk[0] = np.append(self.zpk[0], np.zeros(-D))
-#            else:
-#                self.zpk[1] = self.zpk[1][:D] # discard last D elements of a
+            zpk[0] = np.append(self.zpk[0], np.zeros(-D))
 
+        if len(zpk[2] > 0):
+            k = zpk[2][0]  # read gain
+        else:
+            k = 1  # or set = 1
+
+        zpk[2] = zeros_with_val(len(zpk[0]), k)
+
+        self.zpk = np.asarray(zpk)
+
+        qstyle_widget(self.ui.butSave, 'changed')
+        self._refresh_table()
 
 # ------------------------------------------------------------------------------
 if __name__ == '__main__':
     """ Run widget standalone with `python -m pyfda.input_widgets.input_pz` """
     from pyfda import pyfda_rc as rc
     app = QApplication(sys.argv)
     app.setStyleSheet(rc.qss_rc)
```

### Comparing `pyfda-0.7.1/pyfda/input_widgets/input_pz_ui.py` & `pyfda-0.8.0a2/pyfda/input_widgets/input_pz_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,21 +38,30 @@
         Pass instance `parent` of parent class (FilterCoeffs)
         """
         super(Input_PZ_UI, self).__init__(parent)
 #        self.parent = parent # instance of the parent (not the base) class
         self.eps = 1.e-4  # tolerance value for e.g. setting P/Z to zero
 
         # Items for PZ-format combobox (data, display text, tool tip):
-        self.cmb_pz_frmt_list = [
+        self.cmb_pz_frmt_items = [
             """<span>Set display format for poles and zeros to
-            either cartesian (x + jy) or polar (r * &ang; &Omega;)."
-            Type 'o' for '&deg;', '&lt;' for '&ang;' and 'pi' for '&pi;'.</span>""",
+            either cartesian (x + jy) or polar (r * &ang; &Omega;).
+            Type 'o' for '&deg;', '&lt;' for '&ang;' and 'pi' for '&pi;'.
+            Typing just the angle '&lt;45 o' creates a pole or zero on the
+            unit circle (<i>r = 1</i>).</span>""",
             #
-            ('cartesian', 'Cartesian'), ('polar_rad', 'Polar (rad)'),
-            ('polar_pi', 'Polar (pi)'), ('polar_deg', 'Polar (°)')]
+            ("cartesian", "Cartesian", "Cartesian coordinates (x + jy)"),
+            ("polar_rad", "Polar (rad)",
+             "Polar coordinates (r * &ang; &Omega;) with &ang; in rad."),
+            ('polar_pi', 'Polar (pi)',
+             "<span>Polar coordinates (r * &ang; &Omega;) with &ang; in multiples "
+             "of &pi;, type 'pi' instead of &pi;.</span>"),
+            ('polar_deg', 'Polar (°)',
+            "<span>Polar coordinates (r * &ang; &Omega;) with &ang; in degrees, "
+            "use 'o' or '°' as the degree sign.</span>"),]
         # π: u'3C0, °: u'B0, ∠: u'2220
         self.cmb_pz_frmt_init = 'polar_deg'  # initial setting
 
         self._construct_UI()
 
 # ------------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
@@ -60,19 +69,17 @@
         Process signals coming from the CSV pop-up window
         """
         # logger.debug("PROCESS_SIG_RX\n{0}".format(pprint_log(dict_sig)))
 
         if 'closeEvent' in dict_sig:
             self._close_csv_win()
             self.emit({'ui_global_changed': 'csv'})
-            return  # probably not needed
         elif 'ui_global_changed' in dict_sig:
             self._set_load_save_icons()  # update icons file <-> clipboard
-            # inform e.g. the p/z input widget about changes in CSV options
-            self.emit({'ui_global_changed': 'csv'})
+            # set state of CSV options button according to state of CSV popup handle
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """
         Intitialize the widget, consisting of:
         - top chkbox row
         - coefficient table
@@ -93,15 +100,15 @@
         # self.butEnable.setIconSize(q_icon_size)  # and set the size
         self.butEnable.setToolTip(
             "<span>Show / hide poles and zeros in an editable table."
             " For high order systems, the table display might be slow.</span>")
 
         self.cmbPZFrmt = QComboBox(self)
         qcmb_box_populate(
-            self.cmbPZFrmt, self.cmb_pz_frmt_list, self.cmb_pz_frmt_init)
+            self.cmbPZFrmt, self.cmb_pz_frmt_items, self.cmb_pz_frmt_init)
 
         self.spnDigits = QSpinBox(self)
         self.spnDigits.setRange(0, 16)
         self.spnDigits.setToolTip("Number of digits to display.")
         self.lblDigits = QLabel("Digits", self)
         self.lblDigits.setFont(self.bifont)
 
@@ -216,23 +223,24 @@
         layHButtonsCoeffs1.addStretch()
 
         # -------------------------------------------------------------------
         #   Eps / set zero settings
         # ---------------------------------------------------------------------
         self.butSetZero = QPushButton("= 0", self)
         self.butSetZero.setToolTip(
-            "<span>Set selected poles / zeros = 0 with a magnitude &lt; &epsilon;. "
+            "<span>Check whether selected poles / zeros are equal or zero with a "
+            "tolerance oe &lt; &epsilon;. "
             "When nothing is selected, test the whole table.</span>")
         self.butSetZero.setIconSize(q_icon_size)
 
         lblEps = QLabel(self)
         lblEps.setText("<b><i>for &epsilon;</i> &lt;</b>")
 
         self.ledEps = QLineEdit(self)
-        self.ledEps.setToolTip("Specify tolerance value.")
+        self.ledEps.setToolTip("Specify absolute tolerance value.")
 
         layHButtonsCoeffs2 = QHBoxLayout()
         layHButtonsCoeffs2.addWidget(self.butSetZero)
         layHButtonsCoeffs2.addWidget(lblEps)
         layHButtonsCoeffs2.addWidget(self.ledEps)
         layHButtonsCoeffs2.addStretch()
 
@@ -262,34 +270,28 @@
         self.but_csv_options.clicked.connect(self._open_csv_win)
 
     # ------------------------------------------------------------------------------
     def _open_csv_win(self):
         """
         Pop-up window for CSV options
         """
-        if self.but_csv_options.isChecked():
-            qstyle_widget(self.but_csv_options, "changed")
-        else:
-            qstyle_widget(self.but_csv_options, "normal")
-
         if dirs.csv_options_handle is None:
             # no handle to the window? Create a new instance!
             if self.but_csv_options.isChecked():
                 # Important: Handle to window must be class attribute otherwise it (and
                 # the attached window) is deleted immediately when it goes out of scope
                 dirs.csv_options_handle = CSV_option_box(self)
                 dirs.csv_options_handle.sig_tx.connect(self.process_sig_rx)
                 dirs.csv_options_handle.show()  # modeless i.e. non-blocking popup window
-        else:
-            if not self.but_csv_options.isChecked():  # this should not happen
-                if dirs.csv_options_handle is None:
-                    logger.warning("CSV options window is already closed!")
-                else:
-                    dirs.csv_options_handle.close()
 
+        else:  # close window, delete handle
+            dirs.csv_options_handle.close()
+            self.but_csv_options.setChecked(False)
+
+        # alert other widgets that csv options / visibility have changed
         self.emit({'ui_global_changed': 'csv'})
 
     # ------------------------------------------------------------------------------
     def _close_csv_win(self):
         dirs.csv_options_handle = None
         self.but_csv_options.setChecked(False)
         qstyle_widget(self.but_csv_options, "normal")
@@ -315,20 +317,16 @@
                 "<span>Save table to file, SELECTED items are copied as "
                 "displayed. When nothing is selected, the whole table "
                 "is copied with full precision in decimal format.</span>")
 
             self.butToTable.setIcon(QIcon(':/file.svg'))
             self.butToTable.setToolTip("<span>Load table from file.</span>")
 
-        if dirs.csv_options_handle is None:
-            qstyle_widget(self.but_csv_options, "normal")
-            self.but_csv_options.setChecked(False)
-        else:
-            qstyle_widget(self.but_csv_options, "changed")
-            self.but_csv_options.setChecked(True)
+        # set state of CSV options button according to state of handle
+        self.but_csv_options.setChecked(not dirs.csv_options_handle is None)
 
 
 # ------------------------------------------------------------------------------
 if __name__ == '__main__':
     """ Run widget standalone with `python -m pyfda.input_widgets.input_pz_ui` """
 
     import sys
```

### Comparing `pyfda-0.7.1/pyfda/input_widgets/input_specs.py` & `pyfda-0.8.0a2/pyfda/input_widgets/input_specs.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         All signals terminate here unless the flag `propagate=True`.
 
         The sender name of signals coming in from local subwidgets is changed to
         its parent widget (`input_specs`) to prevent infinite loops.
 
         """
-        # logger.debug(f"SIG_RX: {pprint_log(dict_sig)}")
+        logger.debug(f"SIG_RX: {pprint_log(dict_sig)}")
         if dict_sig['id'] == id(self):
             # logger.warning(f"Stopped infinite loop:\n\tPropagate = {propagate}\
             #               \n{pprint_log(dict_sig)}")
             return
         elif 'view_changed' in dict_sig:
             self.f_specs.load_dict()
             self.t_specs.load_dict()
@@ -121,47 +121,43 @@
         layHButtons2.addWidget(self.butQuit)        # <Quit> button
         layHButtons2.setContentsMargins(*params['wdg_margins'])
 
         # Subwidget for selecting filter with response type rt (LP, ...),
         #    filter type ft (IIR, ...) and filter class fc (cheby1, ...)
         self.sel_fil = select_filter.SelectFilter(self)
         self.sel_fil.setObjectName("select_filter")
-        self.sel_fil.sig_tx.connect(self.sig_rx_local)
 
         # Subwidget for selecting the frequency unit and range
         self.f_units = freq_units.FreqUnits(self)
         self.f_units.setObjectName("freq_units")
-        self.f_units.sig_tx.connect(self.sig_rx_local)
 
         # Changing the frequency unit requires re-display of frequency specs
         # but it does not influence the actual specs (no specsChanged )
         # Activating the "Sort" button emits 'view_changed'?specs_changed'?, requiring
         # sorting and storing the frequency entries
 
         # Changing filter parameters / specs requires reloading of parameters
         # in other hierarchy levels, e.g. in the plot tabs
 
         # Subwidget for Frequency Specs
         self.f_specs = freq_specs.FreqSpecs(self)
         self.f_specs.setObjectName("freq_specs")
-        self.f_specs.sig_tx.connect(self.sig_rx_local)
-        self.sig_tx.connect(self.f_specs.sig_rx)
+
         # Subwidget for Amplitude Specs
         self.a_specs = amplitude_specs.AmplitudeSpecs(self)
         self.a_specs.setObjectName("amplitude_specs")
-        self.a_specs.sig_tx.connect(self.sig_rx_local)
+
         # Subwidget for Weight Specs
         self.w_specs = weight_specs.WeightSpecs(self)
         self.w_specs.setObjectName("weight_specs")
-        self.w_specs.sig_tx.connect(self.sig_rx_local)
+
         # Subwidget for target specs (frequency and amplitude)
         self.t_specs = target_specs.TargetSpecs(self, title="Target Specifications")
         self.t_specs.setObjectName("target_specs")
-        self.t_specs.sig_tx.connect(self.sig_rx_local)
-        self.sig_tx.connect(self.t_specs.sig_rx)
+
         # Subwidget for displaying infos on the design method
         self.lblMsg = QLabel(self)
         self.lblMsg.setWordWrap(True)
         layVMsg = QVBoxLayout()
         layVMsg.addWidget(self.lblMsg)
 
         self.frmMsg = QFrame(self)
@@ -190,19 +186,32 @@
 
         self.setLayout(layVMain)  # main layout of widget
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         self.sig_rx.connect(self.process_sig_rx)
+        self.sig_rx.connect(self.f_units.sig_rx)
+        self.sig_rx_local.connect(self.process_sig_rx_local)
+
+        self.sig_tx.connect(self.f_specs.sig_rx)
+        self.sig_tx.connect(self.t_specs.sig_rx)
+        self.sig_tx.connect(self.f_units.sig_rx)
+
+        self.sel_fil.sig_tx.connect(self.sig_rx_local)
+        self.f_specs.sig_tx.connect(self.sig_rx_local)
+        self.a_specs.sig_tx.connect(self.sig_rx_local)
+        self.t_specs.sig_tx.connect(self.sig_rx_local)
+        self.w_specs.sig_tx.connect(self.sig_rx_local)
+        self.f_units.sig_tx.connect(self.sig_rx_local)
+
         # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
-        self.sig_rx_local.connect(self.process_sig_rx_local)
-        self.butLoadFilt.clicked.connect(lambda: load_filter(self))
+        self.butLoadFilt.clicked.connect(self._load_filter)
         self.butSaveFilt.clicked.connect(lambda: save_filter(self))
         self.butDesignFilt.clicked.connect(self.start_design_filt)
         self.butQuit.clicked.connect(self.quit_program)  # emit 'quit_program'
         # ----------------------------------------------------------------------
 
         self.update_UI()  # first time initialization
         self.start_design_filt()  # design first filter using default values
@@ -287,14 +296,25 @@
             self.frmMsg.hide()
 
         # Update state of "DESIGN FILTER" button
         # It is disabled for "Manual_IIR" and "Manual_FIR" filter classes
         self.color_design_button("changed")
 
 # ------------------------------------------------------------------------------
+    def _load_filter(self):
+        ret = load_filter(self)
+        if ret == 0:
+            self.load_dict()
+            self.emit({'data_changed': 'filter_loaded'})
+        elif ret == -1:
+            return  # error occurred, do nothing
+        else:
+            logger.error(f'Unknown return code "{ret}"!')
+
+# ------------------------------------------------------------------------------
     def load_dict(self):
         """
         Reload all specs/parameters entries from global dict fb.fil[0],
         using the "load_dict" methods of the individual classes
         """
         self.sel_fil.load_dict()  # select filter widget
         self.f_units.load_dict()  # frequency units widget
```

### Comparing `pyfda-0.7.1/pyfda/input_widgets/input_tab_widgets.py` & `pyfda-0.8.0a2/pyfda/input_widgets/input_tab_widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,16 +86,18 @@
                 continue  # with next widget
             if hasattr(inst, 'tab_label'):
                 tabWidget.addTab(inst, inst.tab_label)
             else:
                 tabWidget.addTab(inst, "not set")
             if hasattr(inst, 'tool_tip'):
                 tabWidget.setTabToolTip(n_wdg, inst.tool_tip)
+            # collect all instance tx signals in self.sig_tx
             if hasattr(inst, 'sig_tx'):
                 inst.sig_tx.connect(self.sig_tx)
+            # distribute self.sig_rx signal to all instance rx signals
             if hasattr(inst, 'sig_rx'):
                 self.sig_rx.connect(inst.sig_rx)
 
             n_wdg += 1  # successfully instantiated one more widget
             inst_wdg_str += '\t' + mod_fq_name + "." + input_class + '\n'
 
         if len(inst_wdg_str) == 0:
@@ -111,15 +113,16 @@
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         # self.sig_rx.connect(inst.sig_rx) # happens in _construct_UI()
         # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
-        self.sig_tx.connect(self.sig_rx)  # loop back to local inputs
+        # connect collected tx signals to all rx signal inputs
+        self.sig_tx.connect(self.sig_rx)
         # self.sig_rx.connect(self.log_rx) # enable for debugging
         # When user has selected a different tab, trigger a redraw of current tab
         tabWidget.currentChanged.connect(self.current_tab_changed)
         # The following does not work: maybe current scope must be left?
         # tabWidget.currentChanged.connect(tabWidget.currentWidget().redraw)
 
         layVMain = QVBoxLayout()
```

### Comparing `pyfda-0.7.1/pyfda/input_widgets/select_filter.py` & `pyfda-0.8.0a2/pyfda/input_widgets/select_filter.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/input_widgets/target_specs.py` & `pyfda-0.8.0a2/pyfda/input_widgets/target_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/input_widgets/weight_specs.py` & `pyfda-0.8.0a2/pyfda/input_widgets/weight_specs.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/libs/compat.py` & `pyfda-0.8.0a2/pyfda/libs/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         self.__lbl.setAttribute(Qt.WA_TranslucentBackground)
         self.__lbl.setAttribute(Qt.WA_TransparentForMouseEvents)
         self.__lbl.setSizePolicy(
             QSizePolicy.Expanding,
             QSizePolicy.Expanding,
         )
         self.__lbl.setTextFormat(Qt.RichText)
-        self.__lyt.addWidget(self.__lbl)
+        self.__lyt.addWidget(self.__lbl, Qt.AlignHCenter)
         return
 
     def setText(self, text):
         self.__lbl.setText(text)
         self.updateGeometry()
         return
```

### Comparing `pyfda-0.7.1/pyfda/libs/csv_option_box.py` & `pyfda-0.8.0a2/pyfda/libs/csv_option_box.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 # (see file LICENSE in root directory for details)
 
 """
 Library with classes and functions for file and text IO
 """
 # TODO: import data from files doesn't update FIR / IIR and data changed
 
-from .pyfda_qt_lib import qget_cmb_box, qset_cmb_box, qwindow_stay_on_top
+from .pyfda_qt_lib import (qget_cmb_box, qset_cmb_box, qcmb_box_populate,
+                           qwindow_stay_on_top)
 from pyfda.pyfda_rc import params
 from .compat import (QLabel, QComboBox, QDialog, QPushButton, QRadioButton,
                      QCheckBox, QVBoxLayout, QGridLayout, pyqtSignal)
 
 import logging
 logger = logging.getLogger(__name__)
 
@@ -26,16 +27,23 @@
     Create a pop-up widget for setting CSV options. This is needed when storing /
     reading Comma-Separated Value (CSV) files containing coefficients or poles
     and zeros.
     """
     sig_tx = pyqtSignal(object)  # outgoing  # was: (dict)
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent):
+    def __init__(self, parent, has_cmsis=True):
         super(CSV_option_box, self).__init__(parent)
+
+        self.has_cmsis = has_cmsis
+        self.cmb_delimiter_default = "auto"
+        self.cmb_terminator_default = "auto"
+        self.cmb_orientation_default = "auto"
+        self.cmb_header_default = "auto"
+
         self._construct_UI()
         qwindow_stay_on_top(self, True)
 
 # ------------------------------------------------------------------------------
     def closeEvent(self, event):
         """
         Override closeEvent (user has tried to close the window) and send a
@@ -45,126 +53,155 @@
         self.emit({'closeEvent': ''})
         event.accept()
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         """ initialize the User Interface """
         self.setWindowTitle("CSV Options")
-        lblDelimiter = QLabel("CSV-Delimiter", self)
-        delim = [('Auto', 'auto'), ('< , >', ','), ('< ; >', ';'), ('<TAB>', '\t'),
-                 ('<SPACE>', ' '), ('< | >', '|')]
-        self.cmbDelimiter = QComboBox(self)
-        for d in delim:
-            self.cmbDelimiter.addItem(d[0], d[1])
-        self.cmbDelimiter.setToolTip("Delimiter between data fields.")
-
-        lblTerminator = QLabel("Line Terminator", self)
-        terminator = [('Auto', 'auto'), ('CRLF (Win)', '\r\n'),
-                      ('CR (Mac)', '\r'), ('LF (Unix)', '\n'), ('None', '\a')]
-        self.cmbLineTerminator = QComboBox(self)
-        self.cmbLineTerminator.setToolTip(
-            "<span>Terminator at the end of a data row."
-            " (depending on the operating system). 'None' can be used for a single "
-            "row of data with added line breaks.</span>")
-        for t in terminator:
-            self.cmbLineTerminator.addItem(t[0], t[1])
+
+        lbl_delimiter = QLabel("CSV delimiter", self)
+        cmb_delimiter_items = ["<span>Select delimiter between data fields for im- and export."
+                       "</span>",
+            ("auto", "Auto / ','", "<span>Detect the delimiter automatically for import, "
+             "use ',' for exporting data.</span>"),
+            (',', '< , >', "<span>Use ',' as delimiter between data fields.</span>"),
+            (';', '< ; >', "<span>Use ';' as delimiter between data fields.</span>"),
+            ( '\t', '<TAB>', "<span>Use &lt;TAB&gt; as delimiter between data fields."
+             "</span>"),
+            ( ' ', '<SPACE>', "<span>Use &lt;SPACE&gt; as delimiter between data "
+             "fields.</span>"),
+            ( '|', '< | >',"<span>Use '|' as delimiter between data fields.</span>")
+            ]
+        self.cmb_delimiter = QComboBox(self)
+        qcmb_box_populate(self.cmb_delimiter, cmb_delimiter_items,
+                          self.cmb_delimiter_default)
+
+
+        lbl_terminator = QLabel("Line terminator", self)
+        cmb_terminator_items = [
+            "<span>Terminator at the end of a data row, depending on the operating "
+            "system. 'None' can be used for a single row of data with added line breaks.</span>",
+            ('auto', 'Auto',
+             "<span>Use operating system's default line terminator.</span>"),
+            ('\r\n', 'CRLF (Win)', 'Use &lt;CRLF&gt; as line terminator (Windows '
+             'convention)</span>'),
+            ('\r', 'CR (Mac)', 'Use &lt;CR&gt; as line terminator (MacOS '
+             'convention)</span>'),
+            ('\n', 'LF (Unix)', 'Use &lt;LF&gt; as line terminator (Unix '
+             'convention)</span>'),
+            ('\a', 'None', '<span>No line terminator, use for single row data</span>')
+            ]
+        self.cmb_terminator = QComboBox(self)
+        qcmb_box_populate(self.cmb_terminator, cmb_terminator_items,
+                          self.cmb_terminator_default)
 
         butClose = QPushButton(self)
         butClose.setText("Close")
 
-        lblOrientation = QLabel("Table orientation", self)
-        orientation = [('Auto/Horz.', 'auto'),
-                       ('Vertical', 'vert'), ('Horizontal', 'horiz')]
-        self.cmbOrientation = QComboBox(self)
-        self.cmbOrientation.setToolTip("<span>Select orientation of table.</span>")
-        for o in orientation:
-            self.cmbOrientation.addItem(o[0], o[1])
-
-        lblHeader = QLabel("Enable header", self)
-        header = [('Auto', 'auto'), ('On', 'on'), ('Off', 'off')]
-        self.cmbHeader = QComboBox(self)
-        self.cmbHeader.setToolTip("First row is a header.")
-        for h in header:
-            self.cmbHeader.addItem(h[0], h[1])
+        lbl_orientation = QLabel("Table mode", self)
+        cmb_orientation_items = [
+            "<span>Select row / column mode of table.</span>",
+            ('auto', 'Auto/Cols.', "<span>Detect table orientation automatically "
+             "during import; use column format for exporting data.</span>"),
+            ('cols', 'Columns', "<span>Import / export data in columns.</span>"),
+            ('rows', 'Rows', "<span>Import / export data in rows.</span>")
+            ]
+        self.cmb_orientation = QComboBox(self)
+        qcmb_box_populate(self.cmb_orientation, cmb_orientation_items,
+                          self.cmb_orientation_default)
+
+        lbl_header = QLabel("Use header", self)
+        cmb_header_items = [
+            "<span>Interpret first row resp. column as header.</span>",
+            ('auto', 'Auto/Off', "<span>Detect header automatically during import; "
+             "turn off header during export.</span>"),
+            ('on', 'On', "<span>Turn on header.</span>"),
+            ('off', 'Off', "<span>Turn off.</span>")
+            ]
+        self.cmb_header = QComboBox(self)
+        qcmb_box_populate(self.cmb_header, cmb_header_items,
+                          self.cmb_header_default)
 
         lbl_cmsis = QLabel("CMSIS SOS format", self)
+        lbl_cmsis.setVisible(self.has_cmsis)
         self.chk_cmsis = QCheckBox()
         self.chk_cmsis.setChecked(False)
         self.chk_cmsis.setToolTip(
             "<span>Use CMSIS DSP second-order sections format "
-            "(only for coefficients).</span>")
+            "(only for IIR coefficients).</span>")
+        self.chk_cmsis.setVisible(self.has_cmsis)
 
         self.radClipboard = QRadioButton("Clipboard", self)
         self.radClipboard.setChecked(False)
         self.radFile = QRadioButton("File", self)
         # setting is read later on from params['CSV']['clipboard']
         self.radFile.setChecked(True)
 
         lay_grid = QGridLayout()
-        lay_grid.addWidget(lblDelimiter, 1, 1)
-        lay_grid.addWidget(self.cmbDelimiter, 1, 2)
-        lay_grid.addWidget(lblTerminator, 2, 1)
-        lay_grid.addWidget(self.cmbLineTerminator, 2, 2)
-        lay_grid.addWidget(lblOrientation, 3, 1)
-        lay_grid.addWidget(self.cmbOrientation, 3, 2)
-        lay_grid.addWidget(lblHeader, 4, 1)
-        lay_grid.addWidget(self.cmbHeader, 4, 2)
+        lay_grid.addWidget(lbl_delimiter, 1, 1)
+        lay_grid.addWidget(self.cmb_delimiter, 1, 2)
+        lay_grid.addWidget(lbl_terminator, 2, 1)
+        lay_grid.addWidget(self.cmb_terminator, 2, 2)
+        lay_grid.addWidget(lbl_orientation, 3, 1)
+        lay_grid.addWidget(self.cmb_orientation, 3, 2)
+        lay_grid.addWidget(lbl_header, 4, 1)
+        lay_grid.addWidget(self.cmb_header, 4, 2)
         lay_grid.addWidget(lbl_cmsis, 5, 1)
         lay_grid.addWidget(self.chk_cmsis, 5, 2)
         lay_grid.addWidget(self.radClipboard, 6, 1)
         lay_grid.addWidget(self.radFile, 6, 2)
 
         layVMain = QVBoxLayout()
         # layVMain.setAlignment(Qt.AlignTop) # only affects first widget (intended here)
         layVMain.addLayout(lay_grid)
         layVMain.addWidget(butClose)
         layVMain.setContentsMargins(*params['wdg_margins'])
         self.setLayout(layVMain)
 
-        self._load_settings()
+        self.load_settings()
 
         # ============== Signals & Slots ================================
         butClose.clicked.connect(self.close)
-        self.cmbOrientation.currentIndexChanged.connect(self._store_settings)
-        self.cmbDelimiter.currentIndexChanged.connect(self._store_settings)
-        self.cmbLineTerminator.currentIndexChanged.connect(self._store_settings)
-        self.cmbHeader.currentIndexChanged.connect(self._store_settings)
-        self.chk_cmsis.clicked.connect(self._store_settings)
-        self.radClipboard.clicked.connect(self._store_settings)
-        self.radFile.clicked.connect(self._store_settings)
+        self.cmb_orientation.currentIndexChanged.connect(self.store_settings)
+        self.cmb_delimiter.currentIndexChanged.connect(self.store_settings)
+        self.cmb_terminator.currentIndexChanged.connect(self.store_settings)
+        self.cmb_header.currentIndexChanged.connect(self.store_settings)
+        self.chk_cmsis.clicked.connect(self.store_settings)
+        self.radClipboard.clicked.connect(self.store_settings)
+        self.radFile.clicked.connect(self.store_settings)
 
-    def _store_settings(self):
+    def store_settings(self):
         """
         Store settings of CSV options widget in ``pyfda_rc.params``.
         """
 
         try:
-            params['CSV']['orientation'] = qget_cmb_box(self.cmbOrientation, data=True)
-            params['CSV']['delimiter'] = qget_cmb_box(self.cmbDelimiter, data=True)
-            params['CSV']['lineterminator'] = qget_cmb_box(self.cmbLineTerminator,
+            params['CSV']['orientation'] = qget_cmb_box(self.cmb_orientation, data=True)
+            params['CSV']['delimiter'] = qget_cmb_box(self.cmb_delimiter, data=True)
+            params['CSV']['lineterminator'] = qget_cmb_box(self.cmb_terminator,
                                                            data=True)
-            params['CSV']['header'] = qget_cmb_box(self.cmbHeader, data=True)
+            params['CSV']['header'] = qget_cmb_box(self.cmb_header, data=True)
             params['CSV']['cmsis'] = self.chk_cmsis.isChecked()
             params['CSV']['clipboard'] = self.radClipboard.isChecked()
 
             self.emit({'ui_global_changed': 'csv'})
 
         except KeyError as e:
             logger.error(e)
 
-    def _load_settings(self):
+    def load_settings(self):
         """
         Load settings of CSV options widget from ``pyfda_rc.params``.
         """
         try:
-            qset_cmb_box(self.cmbOrientation, params['CSV']['orientation'], data=True)
-            qset_cmb_box(self.cmbDelimiter, params['CSV']['delimiter'], data=True)
-            qset_cmb_box(self.cmbLineTerminator, params['CSV']['lineterminator'],
+            qset_cmb_box(self.cmb_orientation, params['CSV']['orientation'], data=True)
+            qset_cmb_box(self.cmb_delimiter, params['CSV']['delimiter'], data=True)
+            qset_cmb_box(self.cmb_terminator, params['CSV']['lineterminator'],
                          data=True)
-            qset_cmb_box(self.cmbHeader, params['CSV']['header'], data=True)
+            qset_cmb_box(self.cmb_header, params['CSV']['header'], data=True)
             self.chk_cmsis.setChecked(params['CSV']['cmsis'])
 
             self.radClipboard.setChecked(params['CSV']['clipboard'])
             self.radFile.setChecked(not params['CSV']['clipboard'])
 
         except KeyError as e:
             logger.error(f"Unknown key {e}")
```

### Comparing `pyfda-0.7.1/pyfda/libs/frozendict.py` & `pyfda-0.8.0a2/pyfda/libs/frozendict.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/libs/pyfda_dirs.py` & `pyfda-0.8.0a2/pyfda/libs/pyfda_dirs.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,9 +317,13 @@
 # ------------------------------------------------------------------------------
 """ Place holder for storing the name of the last file"""
 last_file_name = ""
 """ Place holder for storing the directory location of the last file"""
 last_file_dir = HOME_DIR
 """ Place holder for file type selected (e.g. "csv") in last file dialog"""
 last_file_type = ''
-""" Global handle to pop-up window for CSV options """
+"""
+Global handle to pop-up window for CSV options - this window must be closed
+before opening another pop-up window! Otherwise, the second window becomes
+unaccessible (?) and pyfda becomes unresponsive.
+"""
 csv_options_handle = None
```

### Comparing `pyfda-0.7.1/pyfda/libs/pyfda_fft_windows_lib.py` & `pyfda-0.8.0a2/pyfda/libs/pyfda_fft_windows_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -265,29 +265,29 @@
             It can be constructed by convolving a rectangular window four times
             (or multiplying its frequency response four times).
             <br /><br />
 
             See also: Boxcar and Triangular / Bartlett windows.
             </span>'''
             },
-    'Slepian': {
-        'fn_name': 'slepian',
-        'par': [{
-             'name': 'BW', 'name_tex': r'$BW$',
-             'val': 0.3, 'min': 0, 'max': 100,
-             'tooltip': '<span>Bandwidth</span>'}],
-        'info':
-            '''<span>
-            Used to maximize the energy concentration in the main lobe.
-            Also called the digital prolate spheroidal sequence (DPSS).
-            <br /><br />
-
-            See also: Kaiser window.
-            </span>'''
-        },
+    # 'Slepian': {
+    #     'fn_name': 'slepian',
+    #     'par': [{
+    #          'name': 'BW', 'name_tex': r'$BW$',
+    #          'val': 0.3, 'min': 0, 'max': 100,
+    #          'tooltip': '<span>Bandwidth</span>'}],
+    #     'info':
+    #         '''<span>
+    #         Used to maximize the energy concentration in the main lobe.
+    #         Also called the digital prolate spheroidal sequence (DPSS).
+    #         <br /><br />
+
+    #         See also: Kaiser window.
+    #         </span>'''
+    #     },
     'Triangular': {
         'fn_name': 'triang',
         'info': bartlett_info
         },
     'Tukey': {
         'fn_name': 'tukey',
         'par': [{
@@ -307,15 +307,15 @@
             &alpha; = 0.25). Amplitudes of transient events are less likely to be
             altered by this window than e.g. by a Hann window.
             </span>'''
         },
     'Ultraspherical': {
         'fn_name': 'pyfda.libs.pyfda_fft_windows_lib.ultraspherical',
         'par': [{
-            'name': '&mu;', 'name_tex': r'$\mu',
+            'name': '&mu;', 'name_tex': r'$\mu$',
             'val': 0.5, 'min': -0.5, 'max': 10,
             'tooltip': '<span>Shape parameter &mu; or &alpha;</span>'
             },
             {
             'name': 'x0', 'name_tex': r'$x_0$',
             'val': 1, 'min': -10, 'max': 10,
             'tooltip': '<span>Amplitude</span>'}
@@ -547,16 +547,16 @@
     # instance. This is not a problem as signals are distinguished by the attached
     # dict with the payload
     sig_rx = pyqtSignal(object)  # incoming
     sig_tx = pyqtSignal(object)  # outgoing
 
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent, win_dict):
-        super(QFFTWinSelector, self).__init__(parent)
+    def __init__(self, win_dict):
+        super().__init__()
 
         self.win_dict = win_dict
         self.err = False  # error flag for window calculation
         self._construct_UI()
         self.set_window_name()  # initialize win_dict
         self.ui2dict_win()
 
@@ -778,15 +778,15 @@
         win_fnct = self.win_dict[win_name]['win_fnct']
         fn_name = self.win_dict[win_name]['fn_name']
         n_par = self.win_dict[win_name]['n_par']
 
         try:
             if fn_name == 'dpss':
                 logger.info("dpss!")
-                w = scipy.signal.windows.dpss(N, self.in_dict[win_name]['par'][0]['val'],
+                w = scipy.signal.windows.dpss(N, self.win_dict[win_name]['par'][0]['val'],
                                               sym=sym)
             elif n_par == 0:
                 w = win_fnct(N, sym=sym)
             elif n_par == 1:
                 w = win_fnct(N, self.win_dict[win_name]['par'][0]['val'], sym=sym)
             elif n_par == 2:
                 w = win_fnct(N, self.win_dict[win_name]['par'][0]['val'],
@@ -970,7 +970,22 @@
                 self.cmb_win_par_1.setToolTip(self.win_dict[cur]['par'][1]['tooltip'])
                 self.cmb_win_par_1.blockSignals(False)
             else:
                 self.led_win_par_1.setVisible(True)
                 self.cmb_win_par_1.setVisible(False)
                 self.led_win_par_1.setText(str(self.win_dict[cur]['par'][1]['val']))
                 self.led_win_par_1.setToolTip(self.win_dict[cur]['par'][1]['tooltip'])
+
+# ------------------------------------------------------------------------------
+
+if __name__ == "__main__":
+    """ Run widget standalone with `python -m pyfda.libs.pyfda_fft_windows` """
+    import sys
+    from pyfda.libs.compat import QApplication
+    from pyfda import pyfda_rc as rc
+
+    app = QApplication(sys.argv)
+    app.setStyleSheet(rc.qss_rc)
+    mainw = QFFTWinSelector(all_windows_dict)
+    app.setActiveWindow(mainw)
+    mainw.show()
+    sys.exit(app.exec_())
```

### Comparing `pyfda-0.7.1/pyfda/libs/pyfda_fix_lib.py` & `pyfda-0.8.0a2/pyfda/libs/pyfda_fix_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,19 +477,19 @@
         self.frmt2float_vec = np.vectorize(self.frmt2float_scalar, excluded='self')
 
     def verify_q_dict_keys(self, q_dict: dict) -> None:
         """
         Check against the merged `self.q_dict_default` and `self.q_dict_default_ro`
         dictionaries whether all keys in the passed `q_dict` dictionary are valid.
 
-        Unknown keys raise an exception.
+        Unknown keys throw an error message
         """
         for k in q_dict.keys():
             if k not in {**self.q_dict_default, **self.q_dict_default_ro}.keys():
-                raise Exception(u'Unknown Key "{0:s}"!'.format(k))
+                logger.error(u'Unknown Key "{0:s}"!'.format(k))
 
     def set_qdict(self, d: dict) -> None:
         """
         Update the instance quantization dict `self.q_dict` from parameter `d`:
 
         * Transform dict entries for `WF`, `WI`, `W` and `Q` into each other
```

### Comparing `pyfda-0.7.1/pyfda/libs/pyfda_io_lib.py` & `pyfda-0.8.0a2/pyfda/libs/pyfda_io_lib.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,22 +7,33 @@
 # (see file LICENSE in root directory for details)
 
 """
 Library with classes and functions for file and text IO
 """
 import os, re, io
 import csv
+import wave
 import datetime
-from typing import TextIO
+import warnings
+from typing import TextIO, Tuple  # replace by built-in tuple from Py 3.9
 
 import pickle
 
 import numpy as np
 from scipy.io import loadmat, savemat, wavfile
 
+try:
+    import xlwt
+except ImportError:
+    xlwt = None
+try:
+    import xlsx
+except ImportError:
+    xlsx = None
+
 from .pyfda_lib import safe_eval, lin2unit, pprint_log
 from .pyfda_qt_lib import qget_selected
 
 import pyfda.libs.pyfda_fix_lib as fx
 from pyfda.pyfda_rc import params
 import pyfda.libs.pyfda_dirs as dirs
 import pyfda.filterbroker as fb  # importing filterbroker initializes all its globals
@@ -42,17 +53,24 @@
     'csv': 'Comma / Tab Separated Values',
     'mat': 'Matlab-Workspace',
     'npy': 'Binary Numpy Array',
     'npz': 'Zipped Binary Numpy Array',
     'pkl': 'Pickled data',
     'txt': 'Microsemi FIR coefficient format',
     'vhd': 'VHDL package or architecture',
-    'wav': 'WAV audio format'
+    'wav': 'WAV audio format',
+    'xls': 'Excel Worksheet',
+    'xlsx': 'Excel 2007 Worksheet'
     }
 
+# regex pattern that yields true in a re.search() when only the specified
+#  characters (numeric, "eEjJ(),.+-" and blank / line breaks) are contained
+pattern_num_chars = re.compile('[eEjJ()0-9,\.\+\-\s]+$')
+# regex pattern that identifies characters and their position *not* specified
+pattern_no_num = re.compile('(?![eEjJ()0-9,\.\+\-\s])')
 
 # ------------------------------------------------------------------------------
 def prune_file_ext(file_type: str) -> str:
     """
     Prune file extension, e.g. 'Text file' from 'Text file (\*.txt)' returned
     by QFileDialog file type description.
 
@@ -75,47 +93,174 @@
     -----
     Syntax of python regex: ``re.sub(pattern, replacement, string)``
 
     This returns the string obtained by replacing the leftmost non-overlapping
     occurrences of ``pattern`` in ``string`` by ``replacement``.
 
     - '.' means any character
-
     - '+' means one or more
-
     - '[^a]' means except for 'a'
-
     - '([^)]+)' : match '(', gobble up all characters except ')' till ')'
-
     - '(' must be escaped as '\\\('
-
     """
 
     return re.sub('\([^\)]+\)', '', file_type)
 
 
-
 # ------------------------------------------------------------------------------
 def extract_file_ext(file_type: str) -> str:
     """
     Extract list with file extension(s), e.g. '.vhd' from type description
-    'VHDL (\*.vhd)' returned by QFileDialog
+    'VHDL (\*.vhd)' returned by QFileDialog. Depending on the OS, this may be the
+    full file type description or just the extension like '(\*.vhd)'.
+
+    When `file_type` contains no '(', the passed string is returned unchanged.
+
+    For an explanation of the RegEx, see the docstring for `prune_file_ext`.
+
+    Parameters
+    ----------
+    file_type : str
+
+    Returns
+    -------
+    str
+        The file extension between ( ... ) or the unchanged input argument
+        `file_type` when no '('  was contained.
 
-    Depending on the OS, this may be the full file type description
-    or just the extension. When `file_type` contains no '(', the passed string is
-    returned unchanged.
     """
     if "(" in file_type:
         ext_list = re.findall('\([^\)]+\)', file_type)  # extract '(*.txt)'
         return [t.strip('(*)') for t in ext_list]  # remove '(*)'
     else:
         return file_type
 
 
 # ------------------------------------------------------------------------------
+def create_file_filters(file_types: tuple, file_filters: str = ""):
+    """
+    Create a string with file filters for QFileDialog object from `file_types`,
+    a tuple of file extensions and the global `file_filters_dict`.
+
+    When the file extension stored after last QFileDialog operation is in the tuple
+    of file types, return this file extension for e.g. preselecting the file type
+    in QFileDialog.
+
+    Parameters
+    ----------
+    file_types : tuple of str
+        list of file extensions which are used to create a file filter.
+
+    file_filters : str
+        String with file filters for QFileDialog object with the form
+        "Comma / Tab Separated Values (*.csv);; Audio (*.wav *.mp3)". By default,
+        this string is empty, but it can be used to add file filters not contained
+        in the global `file_filters_dict`.
+
+    Returns
+    -------
+    file_filters : str
+        String containing file filters for a QFileDialog object
+
+    last_file_filter : str
+        Single file filter to setup the default file extension in QFileDialog
+
+    """
+    for t in file_types:
+        if t in file_filters_dict:
+            file_filters += file_filters_dict[t] + f" (*.{t});;"
+        else:
+            logger.warning(f"Unknown file extension '.{t}'")
+    # remove trailing ';;', otherwise file filter '*' is appended
+    file_filters = file_filters.rstrip(';;')
+
+    if dirs.last_file_type and dirs.last_file_type in file_filters_dict:
+        last_file_filter =\
+            file_filters_dict[dirs.last_file_type] + f" (*.{dirs.last_file_type})"
+    else:
+        last_file_filter = ""
+
+    return file_filters, last_file_filter
+
+
+# ------------------------------------------------------------------------------
+def select_file(parent: object, title: str = "", mode: str = "r",
+                file_types: Tuple[str, ...] = ('csv', 'txt')) -> Tuple[str, str]:
+    """
+    Select a file from a file dialog box for either reading or writing and return
+    the selected file name and type.
+
+    Parameters
+    ----------
+    title : str
+        title string for the file dialog box (e.g. "Filter Coefficients"),
+
+    mode : str
+        file access mode, must be either "r" or "w" for read / write access
+
+    file_types : tuple of str
+        supported file types, e.g. `('txt', 'npy', 'mat') which need to be keys
+        of `file_filters_dict`
+
+    Returns
+    -------
+    file_name: str
+        Fully qualified name of selected file. `None` when operation has been
+        cancelled.
+
+    file_type: str
+        File type, e.g. 'wav'. `None` when operation has been cancelled.
+    """
+
+    file_filters, last_file_filter = create_file_filters(file_types=file_types)
+
+    dlg = QFileDialog(parent)  # create instance for QFileDialog
+    dlg.setDirectory(dirs.last_file_dir)
+    if mode in {"r", "rb"}:
+        if title == "":
+            title = "Import"
+        dlg.setWindowTitle(title)
+        dlg.setAcceptMode(QFileDialog.AcceptOpen)  # set dialog to "file open" mode
+        dlg.setFileMode(QFileDialog.ExistingFile)
+    elif mode in {"w", "wb"}:
+        if title == "":
+            title = "Export"
+        dlg.setWindowTitle(title)
+        dlg.setAcceptMode(QFileDialog.AcceptSave) # set dialog to "file save" mode
+        dlg.setFileMode(QFileDialog.AnyFile)
+    else:
+        logger.error(f"Unknown mode '{mode}'")
+        return None, None
+
+    dlg.setNameFilter(file_filters)  # pass available file filters
+    # dlg.setDefaultSuffix(file_types[0])  # default suffix when none is given
+    if last_file_filter:
+        dlg.selectNameFilter(last_file_filter)  # filter selected in last file dialog
+
+    if dlg.exec_() == QFileDialog.Accepted:
+        file_name = dlg.selectedFiles()[0]  # pick only first selected file
+        file_type = os.path.splitext(file_name)[-1].strip('.')
+        sel_filt = dlg.selectedNameFilter()  # selected file filter
+
+        if file_type == "":
+            # No file type specified, add the type from the file filter
+            file_type = extract_file_ext(sel_filt)[0].strip('.')
+            file_name = file_name + '.' + file_type
+
+        dirs.last_file_name = file_name
+        dirs.last_file_dir = os.path.dirname(file_name)
+        dirs.last_file_type = file_type
+    else:  # operation cancelled
+        file_name = None
+        file_type = None
+
+    return file_name, file_type
+
+
+# ------------------------------------------------------------------------------
 def qtable2text(table: object, data: np.ndarray, parent: object,
                 fkey: str, frmt: str = 'float', title: str = "Export"):
     """
     Transform table to CSV formatted text and copy to clipboard or file
 
     Parameters
     -----------
@@ -166,31 +311,27 @@
 
     :'clipboard': bool (default: True),
             when ``clipboard = True``, copy data to clipboard, else use a file.
 
     Returns
     -------
     None
-        Nothing, text is exported to clipboard or to file via ``export_csv_data``
+        Nothing, text is exported to clipboard or to file via ``save_data_csv``
     """
 
     text = ""
     if params['CSV']['header'] in {'auto', 'on'}:
         use_header = True
     elif params['CSV']['header'] == 'off':
         use_header = False
     else:
         logger.error(
             f"Unknown key '{params['CSV']['header']}' for params['CSV']['header']")
 
-    if params['CSV']['orientation'] in {'horiz', 'auto'}:
-        orientation_horiz = True
-    elif params['CSV']['orientation'] == 'vert':
-        orientation_horiz = False
-    else:
+    if not params['CSV']['orientation'] in {'rows', 'cols', 'auto'}:
         logger.error(
             f"Unknown key '{params['CSV']['orientation']}' for "
             "params['CSV']['orientation']")
 
     delim = params['CSV']['delimiter'].lower()
     if delim == 'auto':  # 'auto' doesn't make sense when exporting
         delim = ","
@@ -208,57 +349,57 @@
     if not np.any(sel) and frmt != 'float':
         sel = qget_selected(table, reverse=False, select_all=True)['sel']
 
     # ==========================================================================
     # Nothing selected, copy complete table from the model (data) in float format:
     # ==========================================================================
     if not np.any(sel):
-        if orientation_horiz:  # rows are horizontal
+        if params['CSV']['orientation'] in {'rows', 'auto'}:  # write table in row(s)
             for c in range(num_cols):
-                if use_header:  # add the table header
+                if use_header:  # add the table header at the beginning of the row(s)
                     text += table.horizontalHeaderItem(c).text() + delim
                 for r in range(num_rows):
                     text += str(safe_eval(data[c][r], return_type='auto')) + delim
                 text = text.rstrip(delim) + cr
             text = text.rstrip(cr)  # delete last CR
-        else:  # rows are vertical
-            if use_header:  # add the table header
+        else:  # write table in column(s)
+            if use_header:  # add the table header at the top of the column(s)
                 for c in range(num_cols):
                     text += table.horizontalHeaderItem(c).text() + delim
                 text = text.rstrip(delim) + cr
             for r in range(num_rows):
                 for c in range(num_cols):
                     text += str(safe_eval(data[c][r], return_type='auto')) + delim
                 text = text.rstrip(delim) + cr
             text = text.rstrip(cr)  # delete CR after last row
 
     # =======================================================================
     # Copy only selected cells in displayed format:
     # =======================================================================
     else:
-        if orientation_horiz:  # horizontal orientation, one or two rows
-            if use_header:  # add the table header
+        if params['CSV']['orientation'] in {'rows', 'auto'}:  # write table in row(s)
+            if use_header:  # insert table header at the beginning of row 1
                 text += table.horizontalHeaderItem(0).text() + delim
             if sel[0]:
                 for r in sel[0]:
                     item = table.item(r, 0)
                     if item and item.text() != "":
                         text += table.itemDelegate().text(item).lstrip(" ") + delim
                 text = text.rstrip(delim)  # remove last tab delimiter again
 
             if sel[1]:  # returns False for []
                 text += cr  # add a CRLF when there are two columns
-                if use_header:  # add the table header
+                if use_header:  # insert table header at the beginning of row 2
                     text += table.horizontalHeaderItem(1).text() + delim
                 for r in sel[1]:
                     item = table.item(r, 1)
                     if item and item.text() != "":
                         text += table.itemDelegate().text(item) + delim
                 text = text.rstrip(delim)  # remove last tab delimiter again
-        else:  # vertical orientation, one or two columns
+        else:  # write table in column(s)
             sel_c = []
             if sel[0]:
                 sel_c.append(0)
             if sel[1]:
                 sel_c.append(1)
 
             if use_header:
@@ -276,15 +417,15 @@
                             text += table.itemDelegate().text(item).lstrip(" ") + delim
                 text = text.rstrip(delim) + cr
             text.rstrip(cr)
 
     if params['CSV']['clipboard']:
         fb.clipboard.setText(text)
     else:
-        export_csv_data(parent, text, fkey, title=title)
+        save_data_csv(parent, text, fkey, title=title)
 
 # ==============================================================================
 #     # Here 'a' is the name of numpy array and 'file' is the variable to write in a file.
 #     ##if you want to write in column:
 #
 #     for x in np.nditer(a.T, order='C'):
 #             file.write(str(x))
@@ -355,542 +496,648 @@
             f"Importing data from clipboard:\n{np.shape(text)}\n{text}")
         # pass handle to text and convert to numpy array:
         data_arr = csv2array(io.StringIO(text))
         if isinstance(data_arr, str):  # returned an error message instead of numpy data
             logger.error("Error importing clipboard data:\n\t{0}".format(data_arr))
             return None
     else:  # data from file
-        data_arr = import_data(
-            parent, fkey, title=title, file_types=('csv', 'mat', 'npy', 'npz'))
-        # pass data as numpy array
-        logger.debug("Imported data from file. shape = {0} | {1}\n{2}"
-                     .format(np.shape(data_arr), np.ndim(data_arr), data_arr))
-        if type(data_arr) == int and data_arr == -1:  # file operation cancelled
-            data_arr = None
+        file_name, file_type = select_file(parent, title=title, mode="r",
+                                   file_types=('csv', 'mat', 'npy', 'npz'))
+        if file_name is None:  # operation cancelled or error
+            return None
+        else:
+            data_arr = load_data_np(file_name, file_type)
+            # pass data as numpy array
+            logger.debug("Imported data from file. shape = {0} | {1}\n{2}"
+                        .format(np.shape(data_arr), np.ndim(data_arr), data_arr))
+            if type(data_arr) == int and data_arr == -1:  # file operation cancelled
+                data_arr = None
     return data_arr
 
-
 # ------------------------------------------------------------------------------
 def csv2array(f: TextIO):
     """
     Convert comma-separated values from file or text
-    to numpy array, taking into accout the settings of the CSV dict.
+    to numpy array, taking into accout the settings of the CSV dict:
+
+    Read data as it is, splitting each row into the column items when:
+    - `CSV_dict['orientation'] == cols` or
+    - `CSV_dict['orientation'] == auto` and cols <= rows:
+
+    Transpose data when:
+    - `CSV_dict['orientation'] == rows` or
+    - `CSV_dict['orientation'] == auto` and cols > rows:
+
+    `np.shape(data)` returns rows, columns
 
     Parameters
     ----------
 
     f: handle to file or file-like object
         e.g.
 
         >>> f = open(file_name, 'r') # or
         >>> f = io.StringIO(text)
 
     Returns
     -------
 
-    ndarray
-        numpy array containing table data from file or text when import was
+    data_arr: ndarray
+        numpy array of str with table data from file or text when import was
         successful
 
+    OR
+
     io_error: str
         String with the error message when import was unsuccessful
+
+    -----------------------------
+    While opening a file, the `newline` parameter can be used to
+    control how universal newlines works (it only applies to text mode).
+    It can be None, '', '\n', '\r', and '\r\n'. It works as follows:
+
+    - Input: If `newline == None`, universal newlines mode is enabled. Lines in
+      the input can end in '\n', '\r', or '\r\n', and these are translated into
+      '\n' before being returned to the caller. If it is '', universal newline
+      mode is enabled, but line endings are returned to the caller untranslated.
+      If it has any of the other legal values, input lines are only terminated
+      by the given string, and the line ending is returned to the caller untranslated.
+
+    - On output, if newline is None, any '\n' characters written are translated
+      to the system default line separator, os.linesep. If newline is '',
+      no translation takes place. If newline is any of the other legal values,
+      any '\n' characters written are translated to the given string.
+
+      Example: convert from Windows-style line endings to Linux:
+
+      fileContents = open(filename,"r").read()
+      f = open(filename,"w", newline="\n")
+      f.write(fileContents)
+      f.close()
+
+      https://pythonconquerstheuniverse.wordpress.com/2011/05/08/newline-conversion-in-python-3/
     """
-    # throw an error (instead of a deprecation warning) when trying to create a numpy
-    # array from nested ragged sequences. This error can then be caught easily.
-    np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)
+
+    # throw an error (instead of just issueing a deprecation warning) when trying to
+    # create a numpy array from nested ragged sequences. This error can then be
+    # caught easily.
+    warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)
     # ------------------------------------------------------------------------------
     # Get CSV parameter settings
     # ------------------------------------------------------------------------------
     io_error = ""  # initialize string for I/O error messages
+    csv2array.info_str = ""  # initialize function attribute
     CSV_dict = params['CSV']
     try:
         header = CSV_dict['header'].lower()
         if header in {'auto', 'on', 'off'}:
             pass
         else:
             header = 'auto'
             logger.warning(
                 f"Unknown key '{CSV_dict['header']}' for CSV_dict['header'], "
                 f"using {header} instead.")
 
-        orientation_horiz = CSV_dict['orientation'].lower()
-        if orientation_horiz in {'auto', 'vert', 'horiz'}:
-            pass
-        else:
-            orientation_horiz = 'vert'
-            logger.warning(
+        if not CSV_dict['orientation'].lower() in {'auto', 'cols', 'rows'}:
+            logger.error(
                 f"Unknown key '{CSV_dict['orientation']}' for CSV_dict['orientation'], "
-                f"using {orientation_horiz} instead.")
+                "using column mode.")
 
         tab = CSV_dict['delimiter'].lower()
         cr = CSV_dict['lineterminator'].lower()
 
     except KeyError as e:
         io_error = "Dict 'params':\n{0}".format(e)
         return io_error
 
-    try:
-        # ------------------------------------------------------------------------------
-        # Analyze CSV object
-        # ------------------------------------------------------------------------------
-        if header == 'auto' or tab == 'auto' or cr == 'auto':
-            # test the first line for delimiters (of the given selection)
-            dialect = csv.Sniffer().sniff(f.readline(),
-                                          delimiters=['\t', ';', ',', '|', ' '])
-            f.seek(0)                               # and reset the file pointer
-        else:
-            # fall back, alternatives: 'excel', 'unix':
-            dialect = csv.get_dialect('excel-tab')
-
-        if header == "auto":
-            # True when header detected:
-            use_header = csv.Sniffer().has_header(f.read(1000))
-            f.seek(0)
+    sample = ""
 
-    except csv.Error as e:
-        logger.warning("Error during CSV analysis:\n{0},\n"
-                       "continuing with format 'excel-tab'".format(e))
-        dialect = csv.get_dialect('excel-tab')  # fall back
-        use_header = False
+    # ------------------------------------------------------------------------------
+    # Analyze CSV object
+    # ------------------------------------------------------------------------------
+    if header == 'auto' or tab == 'auto' or cr == 'auto':
+        # test the first line for delimiters (of the given selection)
+        sample = f.readline()
+        f.seek(0)  # and reset the file pointer
+        try:
+            dialect = csv.Sniffer().sniff(sample, delimiters=['\t', ';', ',', '|', ' '])
+        except csv.Error as e:
+            logger.warning(f'CSV sniffing reported "{e}",\n'
+                        'continuing with format "excel-tab"')
+            dialect = csv.get_dialect('excel-tab')
+    else:
+        # fall back, alternatives: 'excel', 'unix':
+        dialect = csv.get_dialect('excel-tab')
 
-    if header == 'on':
+    if header == "auto":
+        # yields True when a non-numeric character is detected, indicating a header:
+        use_header = not pattern_num_chars.search(sample)
+    elif header == 'on':
         use_header = True
-    if header == 'off':
+    else:
         use_header = False
-    # case 'auto' has been treated above
 
     delimiter = dialect.delimiter
     lineterminator = dialect.lineterminator
     quotechar = dialect.quotechar
 
     if tab != 'auto':
         delimiter = str(tab)
 
     if cr != 'auto':
         lineterminator = str(cr)
 
-    logger.info("Parsing CSV data with \n"
-                "\tHeader = {0} | Delim. = {1} | Lineterm. = {2} | Quotechar = ' {3} '"
-                # "\n\tType of passed text: '{4}'"
-                .format(use_header, repr(delimiter), repr(lineterminator),
-                        quotechar))  # ,f.__class__.__name__))
+    logger.info(f"Parsing CSV data with header = '{use_header}'\n"
+                f"\tDelimiter = {repr(delimiter)} | Lineterm. = {repr(lineterminator)} "
+                f"| quotechar = ' {quotechar} as '{f.__class__.__name__}'")
+
     # --------------------------------------------------------------------------
     # finally, create iterator from csv data
     data_iter = csv.reader(f, dialect=dialect, delimiter=delimiter,
                            lineterminator=lineterminator)  # returns an iterator
     # --------------------------------------------------------------------------
 # =============================================================================
 #     with open('/your/path/file') as f:
 #         for line in f:
 #             process(line)
 #
 #     Where you define your process function any way you want. For example:
 #
-#         def process(line):
-#             if 'save the world' in line.lower():
-#                 superman.save_the_world()
+#    data_list = []
+#    def process(line):
+#        # split into lines (if not split yet):
+#        data_list.append(line.split(lineterminator))
 #
 #     This will work nicely for any file size and you go through your file in just 1 pass.
 #     This is typically how generic parsers will work.
 #     (https://stackoverflow.com/questions/3277503/how-to-read-a-file-line-by-line-into-a-list)
 # =============================================================================
 
     if use_header:
-        logger.info("Headers:\n{0}".format(next(data_iter, None)))  # py3 and py2
+        logger.info("Header detected:\n{0}".format(next(data_iter, None)))
+
+    csv2array.info_str = f"'{repr(lineterminator)}' # '{repr(delimiter)}'"
 
+    # ------- Read CSV file into a list --------------------
     data_list = []
     try:
         for row in data_iter:
             logger.debug("{0}".format(row))
-            data_list.append(row)
+            if row:  # only append non-empty rows
+                data_list.append(row)
     except csv.Error as e:
         io_error = f"Error during CSV import:\n{e}"
         return io_error
 
-    try:
-        if data_list is None:
-            return "Imported data is None."
-        try:
-            data_arr = np.array(data_list)
-        except np.VisibleDeprecationWarning:
-            # prevent creation of numpy arrays from nested ragged sequences
-            return "Columns with different number of elements."
-
-        if np.ndim(data_arr) == 0 or (np.ndim(data_arr) == 1 and len(data_arr) < 2):
-            return f"Imported data is a scalar: '{data_arr}'"
-        elif np.ndim(data_arr) == 1:
-            if len(data_arr) < 2:
-                return f"Not enough data: '{data_arr}'"
-            else:
-                return data_arr
-        elif np.ndim(data_arr) == 2:
-            cols, rows = np.shape(data_arr)
-            logger.debug(f"cols = {cols}, rows = {rows}, data_arr = {data_arr}\n")
-            if cols > 2 and rows > 2:
-                return f"Unsuitable data shape {np.shape(data_arr)}"
-            elif cols > rows:
-                return data_arr.T
-            else:
-                return data_arr
-        else:
-            return "Unsuitable data shape: ndim = {0}, shape = {1}"\
-                .format(np.ndim(data_arr), np.shape(data_arr))
+    if data_list == [] or data_list ==[""]:
+            return "Imported data is empty."
 
+    # ------- Try to convert list to an array of str --------------------
+    try:
+        data_arr = np.array(data_list)
+    except np.VisibleDeprecationWarning:
+        # prevent creation of numpy arrays from nested ragged sequences
+        return "Can't convert to array, columns have different lengths."
     except (TypeError, ValueError) as e:
-        io_error = "{0}\nFormat = {1}\n{2}".format(e, np.shape(data_arr), data_list)
+        io_error = f"{e}\nData = {pprint_log(data_list)}"
         return io_error
 
-# =============================================================================
-#     try:
-#         data_arr = np.array(data_list)
-#         cols, rows = np.shape(data_arr)
-#         logger.debug("cols = {0}, rows = {1}, data_arr = {2}\n"
-#                       .format(cols, rows, data_arr))
-#         if params['CSV']['orientation'] == 'vert':
-#             return data_arr.T
-#         else:
-#             return data_arr
-#
-#     except (TypeError, ValueError) as e:
-#         io_error = "{0}\nFormat = {1}\n{2}".format(e, np.shape(data_arr), data_list)
-#         return io_error
-#
-# =============================================================================
-
-
-# ------------------------------------------------------------------------------
-def csv2array_new(f: TextIO):
-    """
-    Convert comma-separated values from file or text
-    to numpy array, taking into accout the settings of the CSV dict.
-
-    Parameters
-    ----------
-
-    f: handle to file or file-like object
-        e.g.
+    if np.ndim(data_arr) == 0:
+        return f"Imported data is a scalar: '{data_arr}'"
 
-        >>> f = open(file_name, 'r') # or
-        >>> f = io.StringIO(text)
-
-    Returns
-    -------
-
-    ndarray
-        numpy array containing table data from file or text when import was
-        successful
-
-    io_error: str
-        String with the error message when import was unsuccessful
-    """
-    # ------------------------------------------------------------------------------
-    # Get CSV parameter settings
-    # ------------------------------------------------------------------------------
-    io_error = ""  # initialize string for I/O error messages
-    CSV_dict = params['CSV']
-    logger.warning("Fileobject format: {0}".format(type(f).__name__))
-    try:
-        header = CSV_dict['header'].lower()
-        if header in {'auto', 'on', 'off'}:
-            pass
+    elif np.ndim(data_arr) == 1:
+        if len(data_arr) < 2:
+            return f"Not enough data: '{data_arr}'"
         else:
-            header = 'auto'
-            logger.warning(
-                f"Unknown key '{CSV_dict['header']}' for CSV_dict['header'], "
-                f"using {header} instead.")
-
-        orientation_horiz = CSV_dict['orientation'].lower()
-        if orientation_horiz in {'auto', 'vert', 'horiz'}:
-            pass
-        else:
-            orientation_horiz = 'vert'
-            logger.warning(
-                f"Unknown key '{CSV_dict['orientation']}' for CSV_dict['orientation'], "
-                f"using {orientation_horiz} instead.")
-
-        tab = CSV_dict['delimiter'].lower()
-        cr = CSV_dict['lineterminator'].lower()
-
-    except KeyError as e:
-        io_error = "Dict 'params':\n{0}".format(e)
-        return io_error
+            return data_arr
 
-    try:
-        # ------------------------------------------------------------------------------
-        # Analyze CSV object
-        # ------------------------------------------------------------------------------
-        if header == 'auto' or tab == 'auto' or cr == 'auto':
-            # test the first line for delimiters (of the given selection)
-            dialect = csv.Sniffer().sniff(f.readline(),
-                                          delimiters=['\t', ';', ',', '|', ' '])
-            f.seek(0)                               # and reset the file pointer
+    elif np.ndim(data_arr) == 2:
+        rows, cols = np.shape(data_arr)
+        # logger.info(f"cols = {cols}, rows = {rows}, data_arr = {data_arr}\n")
+        if cols > 2 and rows > 2:
+            return f"Unsuitable data shape {np.shape(data_arr)}"
+        elif params['CSV']['orientation'] == 'rows'\
+                or params['CSV']['orientation'] == 'auto' and cols > rows:
+            # returned table is transposed, swap cols and rows
+            logger.info(f"Building transposed table with {cols} row(s) and {rows} columns.")
+            csv2array.info_str = "T:" + csv2array.info_str
+            return data_arr.T
         else:
-            # fall back, alternatives: 'excel', 'unix':
-            dialect = csv.get_dialect('excel-tab')
+            logger.info(f"Building table with {cols} column(s) and {rows} rows.")
+            return data_arr
+    else:
+        return "Unsuitable data shape: ndim = {0}, shape = {1}"\
+            .format(np.ndim(data_arr), np.shape(data_arr))
 
-        if header == "auto":
-            # True when header detected:
-            use_header = csv.Sniffer().has_header(f.read(1000))
-            f.seek(0)
+#-------------------------------------------------------------------------------
+def read_csv_info_old(filename):
+#-------------------------------------------------------------------------------
+    """
+    DON'T USE ANYMORE!
+    Get infos about the size of a csv file without actually loading the whole
+    file into memory.
+
+    See
+    https://stackoverflow.com/questions/64744161/best-way-to-find-out-number-of-rows-in-csv-without-loading-the-full-thing
+    """
+    file_size = os.path.getsize(filename)
+    logger.info(f"File Size is {file_size} bytes")
+
+    sniffer = csv.Sniffer()
+
+    with open(filename) as f:
+        first_line = f.readline()
+        sample = first_line + f.readline()
+        # pattern search returns true when only allowed characters are found
+        # when the first line contains other characters, it is assumed that this
+        # is a header
+        has_header = not pattern_num_chars.search(sample)
+        # if has_header:
+        #      logger.warning(pattern_no_num.search(sample))
+        dialect = sniffer.sniff(sample)
+        delimiter = dialect.delimiter
+        lineterminator = repr(dialect.lineterminator)
+
+        nchans = first_line.count(delimiter) + 1  # number of columns
+        # count rows in file
+        f.seek(0)
+        N = sum(1 for row in f)  # f isfileobject (csv.reader)  # number of rows
 
-    except csv.Error as e:
-        logger.warning("Error during CSV analysis:\n{0},\n"
-                       "continuing with format 'excel-tab'".format(e))
-        dialect = csv.get_dialect('excel-tab')  # fall back
-        use_header = False
+    del f
 
-    if header == 'on':
-        use_header = True
-    elif header == 'off':
-        use_header = False
-    # case 'auto' has been treated above
+    logger.info(f"Terminator = '{lineterminator}', Delimiter = '{delimiter}', "
+                f"RowCount = {N}, Header={has_header}")
 
-    delimiter = dialect.delimiter
-    lineterminator = dialect.lineterminator
-    quotechar = dialect.quotechar
-
-    if tab != 'auto':
-        delimiter = str(tab)
+    if not params['CSV']['orientation'] in {'rows', 'cols', 'auto'}:
+        logger.error(
+            f"Unknown key '{params['CSV']['orientation']}' for "
+            "params['CSV']['orientation']")
+    if params['CSV']['orientation'] == 'auto' and (N < nchans)\
+        or params['CSV']['orientation'] == 'rows':  # swap rows and columns
+        N, nchans = nchans, N
+        row_mode = True
+        transpose = "T #"
+    else:
+        row_mode = False
+        transpose = ""
 
-    if cr != 'auto':
-        lineterminator = str(cr)
+    if N < 2:
+        logger.error(f"No suitable CSV file, has only {N} data entries.")
+        return -1
 
-    logger.info("Parsing CSV data with header = '{0}'\n"
-                "\tDelimiter = {1} | Lineterm. = {2} | quotechar = ' {3} '\n"
-                "\tType of passed text: '{4}'"
-                .format(use_header, repr(delimiter), repr(lineterminator),
-                        quotechar, f.__class__.__name__))
-    # ------------------------------------------------
-    # finally, create iterator from csv data
-    data_iter = csv.reader(f, dialect=dialect, delimiter=delimiter,
-                           lineterminator=lineterminator)
-    # ------------------------------------------------
-# =============================================================================
-    """
-    newline controls how universal newlines works (it only applies to text mode).
-    It can be None, '', '\n', '\r', and '\r\n'. It works as follows:
+    # file is ok, copy local variables to function attributes
+    read_csv_info.row_mode = row_mode
+    read_csv_info.file_size = file_size
+    read_csv_info.N = N
+    read_csv_info.nchans = nchans
+    read_csv_info.info_str = f"{transpose} '{lineterminator}' # '{delimiter}'"
+
+    return 0
+
+#-------------------------------------------------------------------------------
+def read_wav_info(file):
+    """
+    Get infos about the following properties of a wav file without actually
+    loading the whole file into memory. This is achieved by reading the
+    header.
+    """
+    # https://wavefilegem.com/how_wave_files_work.html
+    # https://stackoverflow.com/questions/7833807/get-wav-file-length-or-duration
+    # http://soundfile.sapp.org/doc/WaveFormat/
+    # https://ccrma.stanford.edu/courses/422/projects/WaveFormat/
+    def str2int(s: str) -> int:
+        """ convert argument from str `s` in little endian format to int """
+        int = 0
+        for i in range(len(s)):
+             int = int + ord(s[i]) * pow(256, i)
+        return int
+
+    f = open(file,'r', encoding='latin-1')
+    # Get the file size in bytes
+    file_size = os.path.getsize(file)
+    if file_size < 44:  # minimum length for WAV file due to header
+        logger.error(f"Not a wav file: Filesize is only {file_size} bytes!")
+        return -1
+    HEADER = f.read(44)  # read complete header
 
-    - On input, if newline is None, universal newlines mode is enabled. Lines in
-      the input can end in '\n', '\r', or '\r\n', and these are translated into
-      '\n' before being returned to the caller. If it is '', universal newline
-      mode is enabled, but line endings are returned to the caller untranslated.
-      If it has any of the other legal values, input lines are only terminated
-      by the given string, and the line ending is returned to the caller untranslated.
+    RIFF = HEADER[:4]  # file pos. 0
+    WAVE = HEADER[8:12]  # pos. 8
+    if RIFF != "RIFF" or WAVE != "WAVE":
+        logger.error("Not a wav file: 'RIFF' or 'WAVE' id missing in file header.")
+        return -1
 
-    - On output, if newline is None, any '\n' characters written are translated
-      to the system default line separator, os.linesep. If newline is '',
-      no translation takes place. If newline is any of the other legal values,
-      any '\n' characters written are translated to the given string.
+    # Pos. 12: String 'fmt ' marks beginning of format subchunk
+    FMT = HEADER[12:16]  # f.read(4)
+    if FMT != "fmt ":  # pos. 12
+        logger.error(f"Invalid format header '{FMT}' instead of 'fmt'!")
+        return -1
 
-      Example: convert from Windows-style line endings to Linux:
-      fileContents = open(filename,"r").read()
-      f = open(filename,"w", newline="\n")
-      f.write(fileContents)
-      f.close()
-      https://pythonconquerstheuniverse.wordpress.com/2011/05/08/newline-conversion-in-python-3/
-     """
+    # Pos. 16: Size of subchunk with format infos in bytes, 16 for Int., 18 for float
+    fmt_chnk_size1 = str2int(HEADER[16:20])
+    if fmt_chnk_size1 not in {16, 18}:
+        logger.error(f"Invalid size {fmt_chnk_size1} of format subchunk!")
+        return -1
 
-    data_list = []
+    # Pos. 20: Audio encoding format, must be 1 for uncompressed PCM
+    encoding = str2int(HEADER[20:22])
+    if encoding == 1:
+        sample_format = "int"  # Integer PCM
+    elif encoding == 3:
+        sample_format = "float"  # IEEE Float PCM
+    else:
+        logger.error(f"Invalid audio encoding {encoding}, only uncompressed "
+                     "PCM supported!")
+        sample_format = ""
+        return -1
 
-    def process(line):
-        # split into lines (if not split yet):
-        data_list.append(line.split(lineterminator))
-
-    # with open(fo) as f:
-    for line in f:
-        process(line)
-
-    for e in data_list:
-        pass
-
-    # Where you define your process function any way you want. For example:
-
-    # This will work nicely for any file size and you go through your file in just 1 pass.
-    # This is typically how generic parsers will work.
-    # (https://stackoverflow.com/questions/3277503/how-to-read-a-file-line-by-line-into-a-list)
-# =============================================================================
+    # Pos. 22: Number of channels
+    nchans = str2int(HEADER[22:24])
 
-# =============================================================================
-#     if use_header:
-#         logger.info("Headers:\n{0}".format(next(data_iter, None))) # py3 and py2
-#
-#     try:
-#         for row in data_iter:
-#             logger.debug("{0}".format(row))
-#             data_list.append(row)
-#     except csv.Error as e:
-#         io_error = "Error during CSV reading:\n{0}".format(e)
-#         return io_error
-# =============================================================================
+    f.seek(24)
+    # Pos. 24: Sampling rate f_S
+    f_S = str2int(f.read(4))
+
+    # Pos. 28: Byte rate = f_S * n_chans * Bytes per sample
+    byte_rate = str2int(f.read(4))
+
+    # Pos. 32: Block align, # of bytes per sample incl. all channels
+    block_align = str2int(f.read(2))
+
+    # Pos. 34: Bits per sample, WL = wordlength in bytes
+    bits_per_sample = str2int(f.read(2))
+
+    if sample_format == "float":
+        # Format subchunk is 18 bytes long for float samples, hence file pointer
+        # has to be advanced by two bytes
+        _ = f.read(2)
+
+        # ###################### FACT Subchunk ###################################
+        # The fact chunk indicates how many sample frames are in the file. For
+        # integer formats the tag it’s optional; otherwise it’s required. For float
+        # PCM, calculation is performed exactly as for integer PCM, hence, it is not
+        # evaluated here.
+        FACT = f.read(12)
+
+    # ###################### DATA Subchunk #######################################
+    # String 'data' marks beginning of data subchunk
+    DATA = f.read(4)
+    if DATA != "data":
+        logger.error(f"Invalid data header '{DATA}' instead of 'data'!")
+        return -1
 
-    try:
-        if data_list is None:
-            return "Imported data is None."
-        data_arr = np.array(data_list)
-        if np.ndim(data_arr) == 0 or (np.ndim(data_arr) == 1 and len(data_arr) < 2):
-            return f"Imported data is a scalar: '{data_arr}'"
-        elif np.ndim(data_arr) == 1:
-            return data_arr
-        elif np.ndim(data_arr) == 2:
-            cols, rows = np.shape(data_arr)
-            logger.debug(f"cols = {cols}, rows = {rows}, data_arr = {data_arr}\n")
-            if cols > 2 and rows > 2:
-                return "Unsuitable data shape {0}".format(np.shape(data_arr))
-            elif cols > rows:
-                return data_arr.T
-            else:
-                return data_arr
+    # -- Function attributes that are accessible from outside
+    # ------------------------------------------------------------
+    read_wav_info.file_size = file_size
+
+    if sample_format == "int":
+        if bits_per_sample == 8:
+            read_wav_info.sample_format = "uint8"
+        elif bits_per_sample == 16:
+            read_wav_info.sample_format = "int16"
+        elif bits_per_sample == 24:
+            read_wav_info.sample_format = "int24"
+        elif bits_per_sample == 32:
+            read_wav_info.sample_format = "int32"
         else:
-            return "Unsuitable data shape: ndim = {0}, shape = {1}"\
-                .format(np.ndim(data_arr), np.shape(data_arr))
-
-    except (TypeError, ValueError) as e:
-        io_error = f"{e}\nFormat = {np.shape(data_arr)}\n{data_list}"
-        return io_error
-
-
-# ------------------------------------------------------------------------------
-def create_file_filters(file_types: tuple, file_filters: str = ""):
-    """
-    Create a string with file filters for QFileDialog object from `file_types`,
-    a tuple of file extensions and the global `file_filters_dict`.
-
-    When the file extension stored after last QFileDialog operation is in the tuple
-    of file types, return this file extension for e.g. preselecting the file type
-    in QFileDialog.
-
-    Parameters
-    ----------
-    file_types : tuple of str
-        list of file extensions which are used to create a file filter.
-
-    file_filters : str
-        String with file filters for QFileDialog object with the form
-        "Comma / Tab Separated Values (*.csv);; Audio (*.wav *.mp3)". By default,
-        this string is empty, but it can be used to add file filters not contained
-        in the global `file_filters_dict`.
+            logger.error("Unsupported integer sample format with {bits_per_sample} "
+                         "bits per sample.")
+            return -1
+    else:
+        if bits_per_sample == 32:
+            read_wav_info.sample_format = "Float32"
+        elif bits_per_sample == 64:
+            read_wav_info.sample_format = "Float64"
+        else:
+            logger.error("Unsupported float sample format with {bits_per_sample} "
+                         "bits per sample.")
+            return -1
 
-    Returns
-    -------
-    file_filters : str
-        String containing file filters for a QFileDialog object
+    read_wav_info.WL = bits_per_sample // 8  # Wordlength in bytes
 
-    last_file_filter : str
-        Single file filter to setup the default file extension in QFileDialog
+    # Pos. 40 or 42: Total number of samples per channel
+    read_wav_info.N = str2int(f.read(4)) // (nchans * read_wav_info.WL)
 
-    """
-    for t in file_types:
-        if t in file_filters_dict:
-            file_filters += file_filters_dict[t] + f" (*.{t});;"
-        else:
-            logger.warning(f"Unknown file extension '.{t}'")
-    # remove trailing ';;', otherwise file filter '*' is appended
-    file_filters = file_filters.rstrip(';;')
+    read_wav_info.nchans = nchans  # number of channels
 
-    if dirs.last_file_type and dirs.last_file_type in file_filters_dict:
-        last_file_filter =\
-            file_filters_dict[dirs.last_file_type] + f" (*.{dirs.last_file_type})"
-    else:
-        last_file_filter = ""
+    read_wav_info.f_S = f_S  # sampling rate in Hz
 
-    return file_filters, last_file_filter
+    # duration of the data in milliseconds
+    read_wav_info.ms = read_wav_info.N * 1000 / (f_S * nchans)
 
+    return 0
 
 # ------------------------------------------------------------------------------
-def import_data(parent, fkey=None, title="Import",
-                file_types=('csv', 'mat', 'npy', 'npz')):
+def load_data_np(file_name: str, file_type: str, fkey: str = "")-> np.ndarray:
     """
     Import data from a file and convert it to a numpy array.
 
     Parameters
     ----------
-    parent : handle to calling instance
+    file_name: str
+        Full path and name of the file to be imported
+
+    file_type: str
+        File type (e.g. 'wav')
 
     fkey : str
         Key for accessing data in *.npz or Matlab workspace (*.mat) file with
         multiple entries.
 
-    title : str
-        title string for the file dialog box (e.g. "Filter Coefficients")
-
-    file_types : tuple of str
-        supported file types, e.g. `('txt', 'npy', 'mat') which need to be keys
-        of `file_filters_dict`
-
     Returns
     -------
-    ndarray
-        Data from the file
+    ndarray of float or int
+        Data from the file (ndarray) or None (error), -1 for file cancel
     """
-    file_filters, last_file_filter = create_file_filters(file_types=file_types)
-
-    dlg = QFileDialog(parent)  # create instance for QFileDialog
-    dlg.setWindowTitle(title)
-    dlg.setDirectory(dirs.last_file_dir)
-    dlg.setAcceptMode(QFileDialog.AcceptOpen)  # set dialog to "file open" mode
-    dlg.setNameFilter(file_filters)  # pass available file filters
-    dlg.setDefaultSuffix('csv')  # default suffix when none is given
-    if last_file_filter:
-        dlg.selectNameFilter(last_file_filter)  # filter selected in last file dialog
-
-    if dlg.exec_() == QFileDialog.Accepted:
-        file_name = dlg.selectedFiles()[0]  # pick only first selected file
-        file_type = os.path.splitext(file_name)[-1].strip('.')
-    else:
-        return -1  # operation cancelled
+    load_data_np.info_str = "" # function attribute for file infos
+    if file_name is None:  # error or operation cancelled
+        return -1
 
     err = False
     try:
         if file_type == 'wav':
             f_S, data_arr = wavfile.read(file_name, mmap=False)
-            fb.fil[0]['f_S_wav'] = f_S
+            # data_arr is 1D for single channel (mono) files and
+            # 2D otherwise (n_chans, n_samples)
+            fb.fil[0]['f_s_wav'] = f_S
+
         elif file_type in {'csv', 'txt'}:
             with open(file_name, 'r', newline=None) as f:
                 data_arr = csv2array(f)
+                load_data_np.info_str = csv2array.info_str
                 # data_arr = np.loadtxt(f, delimiter=params['CSV']['delimiter'].lower())
                 if isinstance(data_arr, str):
                     # returned an error message instead of numpy data:
+                    load_data_np.info_str = ""
                     logger.error(f"Error loading file '{file_name}':\n{data_arr}")
                     return None
         else:
             with open(file_name, 'rb') as f:
                 if file_type == 'mat':
                     data_arr = loadmat(f)[fkey]
                 elif file_type == 'npy':
                     data_arr = np.load(f)
                     # contains only one array
                 elif file_type == 'npz':
                     fdict = np.load(f)
-                    if fkey not in fdict:
+                    if fkey in{"", None}:
+                        data_arr = fdict  # pick the whole array
+                    elif fkey not in fdict:
                         err = True
                         raise IOError(
-                            "Key '{0}' not in file '{1}'.\nKeys found: {2}"
-                            .format(fkey, file_name, fdict.files))
+                            f"Key '{fkey}' not in file '{file_name}'.\n"
+                            f"Keys found: {fdict.files}")
                     else:
                         data_arr = fdict[fkey]  # pick the array `fkey` from the dict
                 else:
                     logger.error('Unknown file type "{0}"'.format(file_type))
                     err = True
 
         if not err:
+            try:  # try to convert array elements to float
+                data_arr = data_arr.astype(float)
+            except ValueError as e:
+                try:
+                    data_arr = data_arr.astype(complex)
+                except ValueError:
+                    logger.error(f"{e},\n\tconversion to complex also failed.")
+                    return None
             logger.info(
-                f'Imported file "{file_name}"\n{pprint_log(data_arr, N=3)}')
-            dirs.last_file_name = file_name
-            dirs.last_file_dir = os.path.dirname(file_name)
-            dirs.last_file_type = file_type
-            return data_arr  # returns numpy array
+                f'Imported file "{file_name}"\n{pprint_log(data_arr, N=5)}')
+            return data_arr  # returns numpy array of type float
 
     except IOError as e:
         logger.error("Failed loading {0}!\n{1}".format(file_name, e))
         return None
 
 
 # ------------------------------------------------------------------------------
-def export_csv_data(parent: object, data: str, fkey: str = "", title: str = "Export",
-                file_types=('csv', 'mat', 'npy', 'npz')):
+def save_data_np(file_name: str, file_type: str, data: np.ndarray,
+                 f_S: int = 1, fmt: str = '%f') -> int:
+    """
+    Save numpy data to a file in wav or csv format
+
+    Parameters
+    ----------
+    file_name: str
+        Full path and name of the file to be imported
+
+    file_type: str
+        File type (e.g. 'wav')
+
+    data : np.ndarray
+        Data to be saved to a file. The data dtype (uint8, int16, int32, float32)
+        determines the bits-per-sample and PCM/float of the WAV file
+
+    f_S : int (optional)
+        Sampling frequency (only used for WAV file format), only integer sampling
+        frequencies are supported by the WAV format.
+
+    fmt : str (optional)
+        Optional, default '%f'. Format string, only used for exporting data in CSV
+        format. Other options are e.g. '%1.2f' for reduced number of digits, '%d' for
+        integer format or '%s' for strings.
+
+    Returns
+    -------
+    0 for success, -1 for file cancel or error
+    """
+    # file_name, file_type = select_file(parent, title=title, mode='wb', file_types=('wav'))
+
+    if file_name is None:  # error or operation cancelled
+        return -1
+    elif np.ndim(data) < 1 or np.ndim(data) > 2:
+        logger.error(f"Unsuitable data format for a wav file, ndim = {np.ndim(data)}.")
+        logger.error(data)
+        return -1
+    try:
+        if file_type == 'wav':
+            f_S_int = int(abs(f_S))
+            if f_S_int == 0:
+                f_S_int = 1
+            if f_S != f_S_int:
+                logger.warning(
+                    "Only integer sampling frequencies can be used for WAV files,\n"
+                    f"sampling frequency has been changed to f_S = {f_S_int}")
+
+            # audio = data.T  # transpose data, needed?
+            wavfile.write(file_name, f_S_int, data)
+            # To write multiple-channels, use a 2-D array of shape (Nsamples, Nchannels).
+
+        elif file_type == 'csv':
+            delimiter = params['CSV']['delimiter'].lower()
+            if delimiter == 'auto':
+                delimiter = ','
+            np.savetxt(file_name, data, fmt=fmt, delimiter=delimiter)
+            # TODO: Integer formats like int16 should be stored as integers
+        else:
+            logger.error(f"File type {file_type} not supported!")
+            return -1
+
+        logger.info(f'Saved data as\n\t"{file_name}".')
+        return 0
+
+
+    except IOError as e:
+        logger.error(f'Failed saving "{file_name}"!\n{e}\n')
+        return -1
+
+# ------------------------------------------------------------------------------
+def write_wav_frame(parent, file_name, data: np.array, f_S = 1,
+                    title: str = "Export"):
+    """
+    Export a frame of data in wav format
+
+    Parameters
+    ----------
+    parent: handle to calling instance for creating file dialog instance
+
+    data: np.array
+        data to be exported
+
+    title: str
+        title string for the file dialog box (e.g. "audio data ")
+
+    """
+    file_name, file_type = select_file(parent, title=title, mode='wb', file_types=('wav'))
+    if file_name is None:
+        return None  # file operation cancelled or other error
+
+    try:
+        if np.ndim(data) == 1:  # mono
+            audio = data
+            n_chan = 1
+        elif np.ndim(data) != 2:
+            logger.error(f"Unsuitable data format, ndim = {np.ndim(data)}.")
+            return
+        elif np.shape(data)[1] != 2:
+            logger.error(f"Unsuitable number of channels = {np.shape(data)[1]}")
+            return
+        else:
+            audio = data.T  # transpose data
+            n_chan = np.shape(data)[1]
+            # audio = np.array([left_channel, right_channel]).T
+        with wave.open(file_name, "w") as f:
+            # 2 Channels.
+            f.setnchannels(n_chan)
+            # 2 bytes per sample.
+            f.setsampwidth(2)
+            f.setframerate(f_S)
+            f.writeframes(audio.tobytes())
+        with open(file_name, 'w', encoding="utf8", newline='') as f:
+                        f.write(data)
+
+        logger.info(f'Filter saved as\n\t"{file_name}"')
+
+    except IOError as e:
+        logger.error('Failed saving "{0}"!\n{1}\n'.format(file_name, e))
+
+
+# ------------------------------------------------------------------------------
+def save_data_csv(parent: object, data: str, fkey: str = "", title: str = "Export",
+                file_types: Tuple[str, ...] = ('csv', 'mat', 'npy', 'npz')):
     """
     Export coefficients or pole/zero data in various formats
 
     Parameters
     ----------
     parent: handle to calling instance for creating file dialog instance
 
@@ -906,52 +1153,30 @@
         title string for the file dialog box (e.g. "filter coefficients ")
 
     file_types: tuple of strings
         file extension (e.g. `(csv)` or list of file extensions (e.g. `(csv, txt)`
         which are used to create a file filter.
     """
     logger.debug(
-        f"imported data: type{type(data)}|dim{np.ndim(data)}|"
+        f"export data: type{type(data)}|dim{np.ndim(data)}|"
         f"shape{np.shape(data)}\n{data}")
 
     # add file types for FIR filter coefficients
     if fb.fil[0]['ft'] == 'FIR':
         file_types += ('coe', 'vhd', 'txt')
-
-    file_filters, last_file_filter = create_file_filters(file_types=file_types)
-
-#        # Add further file types when modules are available:
-#        if XLWT:
-#            file_filters += ";;Excel Worksheet (.xls)"
-#        if XLSX:
-#            file_filters += ";;Excel 2007 Worksheet (.xlsx)"
-
-    # return selected file name (with or without extension) and filter (Linux: full text)
-    dlg = QFileDialog(parent)  # create instance for QFileDialog
-    dlg.setWindowTitle(title)
-    dlg.setDirectory(dirs.last_file_dir)
-    dlg.setAcceptMode(QFileDialog.AcceptSave)  # set dialog to "file save" mode
-    dlg.setNameFilter(file_filters)  # set the list with all available file formats
-    # dlg.setDefaultSuffix()  # does not work, need to specify the suffix
-
-    if last_file_filter:
-        dlg.selectNameFilter(last_file_filter)  # filter selected in last file dialog
-
-    if dlg.exec_() == QFileDialog.Accepted:
-        file_name = dlg.selectedFiles()[0]   # convert list (with single entry?) to item
-        sel_filt = dlg.selectedNameFilter()  # selected file filter
-    else:
-        return -1
-
-    # Slice off file extension
-    file_type = os.path.splitext(file_name)[-1].strip('.')
-    if file_type == "":
-        # No file type specified, add the type from the file filter
-        file_type = extract_file_ext(sel_filt)[0].strip('.')
-        file_name = file_name + '.' + file_type
+    # Add file types when Excel modules are available:
+    if xlwt is not None:
+        file_types += ('xls',)
+    if xlsx is not None:
+        file_types += ('xlsx',)
+
+    file_name, file_type = select_file(parent,title=title, mode='wb',
+                                       file_types=file_types)
+    if file_name is None:
+        return None  # file operation cancelled or other error
 
     err = False
 
     try:
         if file_type == 'csv':
             with open(file_name, 'w', encoding="utf8", newline='') as f:
                 f.write(data)
@@ -1011,42 +1236,39 @@
                     # Write labels with formatting.
                     worksheet.write('A1', 'b', bold)
                     worksheet.write('B1', 'a', bold)
 
                     # Write some numbers, with row/column notation.
                     for col in range(2):
                         for row in range(np.shape(data)[1]):
-                            worksheet.write(row+1, col, data[col][row])  # vertical
-        #                    worksheet.write(row, col, coeffs[col][row])  # horizontal
+                            worksheet.write(row+1, col, data[col][row])  # columns
+        #                    worksheet.write(row, col, coeffs[col][row])  # rows
 
                     # Insert an image - useful for documentation export ?!.
         #            worksheet.insert_image('B5', 'logo.png')
 
                     workbook.close()
 
                 else:
                     logger.error('Unknown file type "{0}"'.format(file_type))
                     err = True
 
         if not err:
             logger.info(f'Filter saved as\n\t"{file_name}"')
-            dirs.last_file_name = file_name
-            dirs.last_file_dir = os.path.dirname(file_name)  # save new dir
-            dirs.last_file_type = file_type  # save file type
 
     except IOError as e:
         logger.error('Failed saving "{0}"!\n{1}\n'.format(file_name, e))
 
         # Download the Simple ods py module:
         # http://simple-odspy.sourceforge.net/
         # http://codextechnicanum.blogspot.de/2014/02/write-ods-for-libreoffice-calc-from_1.html
 
 
 # ------------------------------------------------------------------------------
-def generate_header(title: str) -> str:
+def coe_header(title: str) -> str:
     """
     Generate a file header (comment) for various FPGA FIR coefficient export formats
     with information on the filter type, corner frequencies, ripple etc
 
     Parameters
     ----------
     title: str
@@ -1141,15 +1363,15 @@
         header += "\t" + lf + " = " + str(f) + " " + unit + " : " + la + " = "
         header += str(a) + " dB\n"
     header += "-" * 85 + "\n"
     return header
 
 
 # ------------------------------------------------------------------------------
-def export_coe_xilinx(f: TextIO):
+def export_coe_xilinx(f: TextIO) -> None:
     """
     Save FIR filter coefficients in Xilinx coefficient format as file '\*.coe', specifying
     the number base and the quantized coefficients (decimal or hex integer).
     """
     qc = fx.Fixed(fb.fil[0]['fxqc']['QCB'])  # instantiate fixpoint object
     logger.debug("scale = {0}, WF = {1}".format(qc.q_dict['scale'], qc.q_dict['WF']))
 
@@ -1167,15 +1389,15 @@
                        'using decimal format.')
         qc.set_qdict({'fx_base': 'dec'})  # select decimal format in all other cases
         coe_radix = 10
 
     # Quantize coefficients to decimal / hex integer format, returning an array of strings
     bq = qc.float2frmt(fb.fil[0]['ba'][0])
 
-    exp_str = "; " + generate_header(
+    exp_str = "; " + coe_header(
         "XILINX CORE Generator(tm) Distributed Arithmetic FIR filter coefficient (.COE) file").replace("\n", "\n; ")
 
     exp_str += "\nRadix = {0};\n".format(coe_radix)
     exp_str += f"Coefficient_width = {qc.q_dict['W']};\n"  # quantized wordlength
     coeff_str = "CoefData = "
     for b in bq:
         coeff_str += str(b) + ",\n"
@@ -1183,15 +1405,15 @@
 
     f.write(exp_str)
 
     return False
 
 
 # ------------------------------------------------------------------------------
-def export_coe_microsemi(f: TextIO):
+def export_coe_microsemi(f: TextIO) -> None:
     """
     Save FIR filter coefficients in Microsemi coefficient format as file '\*.txt'.
     Coefficients have to be in integer format, the last line has to be empty.
     For (anti)symmetric filter only one half of the coefficients must be
     specified?
     """
     qc = fx.Fixed(fb.fil[0]['fxqc']['QCB'])  # instantiate fixpoint object
@@ -1199,31 +1421,31 @@
     if qc.q_dict['WF'] != 0:
         # Set the fixpoint format to integer (WF=0) with the original wordlength:
         qc.set_qdict({'W': qc.q_dict['W'], 'scale': 1 << qc.q_dict['W']-1})
         logger.warning("Fractional formats are not supported, using integer format.")
 
     if qc.q_dict['fx_base'] != 'dec':
         qc.set_qdict({'fx_base': 'dec'})  # select decimal format in all other cases
-        logger.warning('Only coefficients in "dec" format are supported,'
-                       'using decimal format.')
+        logger.warning('Switching to decimal coefficient format, other numeric formats '
+                       'are not supported by Microsemi tools.')
 
     # Quantize coefficients to decimal integer format, returning an array of strings
     bq = qc.float2frmt(fb.fil[0]['ba'][0])
 
     coeff_str = "coefficient_set_1\n"
     for b in bq:
         coeff_str += str(b) + "\n"
 
     f.write(coeff_str)
 
     return False
 
 
 # ------------------------------------------------------------------------------
-def export_coe_vhdl_package(f: TextIO):
+def export_coe_vhdl_package(f: TextIO) -> None:
     """
     Save FIR filter coefficients as a VHDL package '\*.vhd', specifying
     the number base and the quantized coefficients (decimal or hex integer).
     """
     qc = fx.Fixed(fb.fil[0]['fxqc']['QCB'])  # instantiate fixpoint object
     if not qc.q_dict['fx_base'] == 'float' and qc.q_dict['WF'] != 0:
         # Set the fixpoint format to integer (WF=0) with the original wordlength
@@ -1247,15 +1469,15 @@
         post = ""
         logger.warning('Coefficients in "{0}" format are currently not supported, '
                        'using decimal format.'.format(qc.q_dict['fx_base']))
 
     # Quantize coefficients to selected fixpoint format, returning an array of strings
     bq = qc.float2frmt(fb.fil[0]['ba'][0])
 
-    exp_str = "-- " + generate_header(
+    exp_str = "-- " + coe_header(
         "VHDL FIR filter coefficient package file").replace("\n", "\n-- ")
 
     exp_str += "\nlibrary IEEE;\n"
     if qc.q_dict['fx_base'] == 'float':
         exp_str += "use IEEE.math_real.all;\n"
     exp_str += "USE IEEE.std_logic_1164.all;\n\n"
     exp_str += "package coeff_package is\n"
@@ -1276,15 +1498,15 @@
 
     f.write(exp_str)
 
     return False
 
 
 # ------------------------------------------------------------------------------
-def export_coe_TI(f: TextIO):
+def export_coe_TI(f: TextIO) -> None:
     """
     Save FIR filter coefficients in TI coefficient format
     Coefficient have to be specified by an identifier 'b0 ... b191' followed
     by the coefficient in normalized fractional format, e.g.
 
     b0 .053647
     b1 -.27485
@@ -1293,36 +1515,24 @@
 
     ** not implemented yet **
     """
     pass
 
 
 # ==============================================================================
-def load_filter(self):
+def load_filter(self) -> int:
     """
     Load filter from zipped binary numpy array or (c)pickled object to
-    filter dictionary and update input and plot widgets
+    filter dictionary
     """
-    file_types = ("npz", "pkl")
-    file_filters, last_file_filter = create_file_filters(file_types)
+    file_name, file_type = select_file(
+        self, title="Load Filter", mode="rb", file_types = ("npz", "pkl"))
 
-    dlg = QFileDialog(self)
-    dlg.setWindowTitle("Load Filter")
-    dlg.setDirectory(dirs.last_file_dir)
-    dlg.setAcceptMode(QFileDialog.AcceptOpen)  # set dialog to "file open" mode
-    dlg.setNameFilter(file_filters)  # pass available file filters
-    # dlg.setDefaultSuffix('csv')  # default suffix when none is given
-    if last_file_filter:
-        dlg.selectNameFilter(last_file_filter)  # filter selected in last file dialog
-
-    if dlg.exec_() == QFileDialog.Accepted:
-        file_name = dlg.selectedFiles()[0]  # pick only first selected file
-        file_type = os.path.splitext(file_name)[-1].strip('.')
-    else:
-        return -1  # operation cancelled
+    if file_name is None:
+        return -1  # operation cancelled or some other error
 
     err = False
     fb.fil[1] = fb.fil[0].copy()  # backup filter dict
     try:
         with io.open(file_name, 'rb') as f:
             if file_type == 'npz':
                 # array containing dict, dtype 'object':
@@ -1349,58 +1559,61 @@
                 # sanitize values in filter dictionary, keys are ok by now
                 for k in fb.fil[0]:
                     # Bytes need to be decoded for py3 to be used as keys later on
                     if type(fb.fil[0][k]) == bytes:
                         fb.fil[0][k] = fb.fil[0][k].decode('utf-8')
                     if fb.fil[0][k] is None:
                         logger.warning("Entry fb.fil[0][{0}] is empty!".format(k))
+                if 'ba' not in fb.fil[0]\
+                    or type(fb.fil[0]['ba']) not in {list, np.ndarray}\
+                        or np.ndim(fb.fil[0]['ba']) != 2\
+                        or (np.shape(fb.fil[0]['ba'][0]) != 2
+                            and np.shape(fb.fil[0]['ba'])[1] < 3):
+                    logger.error("Missing key 'ba' or wrong data type!")
+                    return -1
+                elif 'zpk' not in fb.fil[0]\
+                    or type(fb.fil[0]['zpk']) not in {list, np.ndarray}\
+                        or np.ndim(fb.fil[0]['zpk']) != 2:
+                    logger.error("Missing key 'zpk' or wrong data type!")
+                    return -1
+                elif 'sos' not in fb.fil[0]\
+                        or type(fb.fil[0]['sos']) not in {list, np.ndarray}:
+                    logger.error("Missing key 'sos' or wrong data type!")
+                    return -1
 
                 logger.info('Successfully loaded filter\n\t"{0}"'.format(file_name))
                 dirs.last_file_name = file_name
                 dirs.last_file_dir = os.path.dirname(file_name)  # update working dir
                 dirs.last_file_type = file_type  # save file type
-                # emit signal -> filter loaded
-                self.emit({'data_changed': 'filter_loaded'})
+                return 0
 
     except IOError as e:
         logger.error("Failed loading {0}!\n{1}".format(file_name, e))
+        return -1
     except Exception as e:
         logger.error("Unexpected error:\n{0}".format(e))
         fb.fil[0] = fb.fil[1]  # restore backup
+        return -1
 
 
 # ------------------------------------------------------------------------------
 def save_filter(self):
     """
     Save filter as zipped binary numpy array or pickle object
     """
-    file_types = ("npz", "pkl")
-    file_filters, last_file_filter = create_file_filters(file_types)
-
-    dlg = QFileDialog(self)
-    dlg.setWindowTitle("Save filter as")
-    dlg.setDirectory(dirs.last_file_dir)
-    dlg.setAcceptMode(QFileDialog.AcceptSave)  # set dialog to "file save" mode
-    dlg.setNameFilter(file_filters)
-
-    if last_file_filter:
-        dlg.selectNameFilter(last_file_filter)  # filter selected in last file dialog
-
-    if dlg.exec_() == QFileDialog.Accepted:
-        file_name = dlg.selectedFiles()[0]  # pick only first selected file
-        # sel_filt = dlg.selectedNameFilter()  # selected file filter
-    else:
-        return -1  # operation cancelled
-
-    file_type = os.path.splitext(file_name)[-1].strip('.')  # slice off file extension
+    file_name, file_type = select_file(
+        self, title="Save Filter", mode='wb', file_types = ("npz", "pkl"))
 
+    if file_name is None:
+        return -1  # operation cancelled or other error
     err = False
     try:
         with io.open(file_name, 'wb') as f:
             if file_type == 'npz':
+                logger.warning(pprint_log(fb.fil[0]))
                 np.savez(f, **fb.fil[0])
             elif file_type == 'pkl':
                 pickle.dump(fb.fil[0], f)  # save in default pickle version
             else:
                 err = True
                 logger.error('Unknown file type "{0}"'.format(file_type))
```

### Comparing `pyfda-0.7.1/pyfda/libs/pyfda_lib.py` & `pyfda-0.8.0a2/pyfda/libs/pyfda_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import numexpr
 import markdown
 
 import scipy.signal as sig
 
 from distutils.version import LooseVersion
 import pyfda.libs.pyfda_dirs as dirs
+from pyfda.libs.pyfda_sig_lib import zeros_with_val
 
 # ###### VERSIONS and related stuff ############################################
 # ================ Required Modules ============================
 # ==
 # == When one of the following imports fails, terminate the program
 from scipy import __version__ as V_SCI
 from matplotlib import __version__ as V_MPL
@@ -278,20 +279,24 @@
     """
     Remove non-ASCII-characters (outside range 0 ... x7F) from `arg` when it
     is a `str`. Otherwise, return `arg` unchanged.
 
     Parameters
     ----------
     arg: str
-        This is a unicode string under Python 3 and a "normal" string under Python 2.
+        This is a unicode string under Python 3
 
     Returns
     -------
     arg: str
-         Input string, cleaned from non-ASCII characters
+         Input string, cleaned from non-ASCII characters when `arg` is a string
+
+         or
+
+         Unchanged parameter `arg` when not a string
 
     """
     if isinstance(arg, str):
         return re.sub(r'[^\x00-\x7f]', r'', arg)
     else:
         return arg
 
@@ -346,14 +351,33 @@
     else:
         a_type = type(a)
 
     return a_type
 
 
 # -----------------------------------------------------------------------------
+def np_shape(data):
+    """
+    Return the shape of `data` as tuple (rows, columns) for up to
+    2-dimensional data. Otherwise, return None
+    """
+    d = np.ndim(data)
+    if d == 0:
+        return (0, 0)
+    elif d == 1:
+        return(len(data), 1)
+    elif  d == 2:
+        return np.shape(data)
+    else:
+        logger.warning("Unsuitable data shape with "
+        f"{d} dimensions.")
+        return (None, None)
+
+
+# -----------------------------------------------------------------------------
 def set_dict_defaults(d: dict, default_dict: dict) -> None:
     """
     Add the key:value pairs of `default_dict` to dictionary `d` for all missing
     keys
     """
     if d is None or d == {}:
         d = default_dict
@@ -415,37 +439,59 @@
                 s += cr + tab
             if type(d[k]) in {list, np.ndarray}:
                 s += k + ' (L=' + str(len(d[k])) + '): '\
                                 + str(d[k][: min(N-1, len(d[k]))]) + ' ...'
             else:
                 s += k + ' : ' + str(d[k])
             first = False
-    elif type(d) in {list, np.ndarray}:
+        return s
+    if type(d) in {list, tuple}:
+        try:
+            _ = np.asarray(d)
+        except (TypeError, ValueError) as e:
+            logger.warning(f"pprint_log(): Could not transform data to array:\n{e}")
+            return ""
+
+    if type(d) in {list, np.ndarray, tuple}:
         if np.ndim(d) == 1:
-            s += ('Type: {0} of {1}, Shape =  ({2} x 1)' + cr + tab)\
-                .format(type(d).__name__, type(d[0]).__name__, len(d))
+            s += (f'Type: {type(d).__name__} of {type(d[0]).__name__}, '
+                  f'shape =  ({len(d)},)' + cr + tab)
             s += str(d[: min(N-1, len(d))])
             if len(d) > N-1:
                 s += ' ...'
         elif np.ndim(d) == 2:
-            cols, rows = np.shape(d)  # (outer, inner), inner (rows)is 1 or 2
-            s += (f'Type: {type(d).__name__} of {type(d[0][0]).__name__} '
-                  f'({d[0][0].dtype}), Shape = ({rows} x {cols})' + cr + tab)
+            rows, cols = np.shape(d)
+            s += (f'Type: {type(d).__name__} of {type(d[0][0]).__name__}, '
+                  f'shape = (r{rows} x c{cols})' + cr + tab)
             #  x.dtype.kind returns general information on numpy data (e.g. "iufc","SU")
-            for c in range(min(N-1, cols)):
+            for r in range(min(N, rows)):
                 if not first:
                     s += cr + tab
                 # logger.warning(f'rows={rows}; min(N-1, rows)={min(N, rows)}\n'
                 #                f'd={d[c][:min(N, rows)]}')
-                s += str(d[c][:min(N, rows)])
-                if rows > N-1:
+                s += str(d[r][:min(N, cols)])
+                if cols > N-1:
                     s += ' ...'
                 first = False
+            if rows > N-1:
+                    s += cr + tab + ' ...'
+        else:
+            logger.warning(f"pprint_log(): Object with ndim = {np.ndim(d)} cannot be processed.")
+            return ""
+    else:  # scalar, string or None
+        if type(d) is None:
+            s += ('Type: None')
+        elif type(d) is str:
+            s += (f' Type: str, length = {len(d)}' +  cr + tab + d[: min(N-1, len(d))])
+            if len(d) > N-1:
+                s += ' ...'
+        elif np.isscalar(d):
+            s += (f'Type: {type(d).__name__}' + cr + tab + str(d))
         else:
-            logger.warning(f"Object with ndim = {np.ndim(d)} cannot be processed.")
+            s += (f'Type: {type(d).__name__}')
     return s
 
 
 # ------------------------------------------------------------------------------
 def safe_numexpr_eval(expr: str, fallback=None,
                       local_dict: dict = {}) -> ndarray:
     """
@@ -468,76 +514,90 @@
 
     Returns
     -------
     np_expr : array-like
         `expr` converted to a numpy array or scalar
 
     """
+    safe_numexpr_eval.err = 0  # function attribute, providing some sort of "memory"
     local_dict.update({'j': 1j, 'None': 0})
     if type(fallback) == tuple:
         np_expr = np.zeros(fallback)  # fallback defines the shape
         fallback_shape = fallback
     else:
         np_expr = fallback  # fallback is the default numpy return value or None
         fallback_shape = np.shape(fallback)
 
     if type(expr) != str or expr == "None":
         logger.warning(f"numexpr: Unsuitable input '{expr}' of type "
                        f"'{type(expr).__name__}', replacing with zero.")
+        safe_numexpr_eval.err = 10
         expr = "0.0"
 
-    expr = expr.lstrip('0')  # remove trailing zeros which cannot be processed
+    # Find one or more redundant zeros '0+' at the beginning '^' leading a number [0-9]
+    # Group the number(s) '(...)' and write it '\1' to the resulting string.
+    expr = re.sub(r'^0+([0-9])', r'\1', expr)
     if len(expr) == 0:
         expr = "0"
     else:
         expr = expr.replace(',', '.')  # ',' -> '.' for German-style numbers
         if expr[0] == '.':  # prepend '0' when the number starts with '.'
             expr = "0" + expr
     try:
         np_expr = numexpr.evaluate(expr.strip(), local_dict=local_dict)
     except SyntaxError as e:
         logger.warning(f"numexpr: Syntax error:\n\t{e}")
+        safe_numexpr_eval.err = 1
+    except AttributeError as e:
+        logger.warning(f"numexpr: Attribute error:\n\t{e}")
+        safe_numexpr_eval.err = 2
     except KeyError as e:
         logger.warning(f"numexpr: Unknown variable {e}")
+        safe_numexpr_eval.err = 3
     except TypeError as e:
         logger.warning(f"numexpr: Type error\n\t{e}")
-    except AttributeError as e:
-        logger.warning(f"numexpr: Attribute error:\n\t{e}")
+        safe_numexpr_eval.err = 4
     except ValueError as e:
         logger.warning(f"numexpr: Value error:\n\t{e}")
+        safe_numexpr_eval.err = 5
     except ZeroDivisionError:
         logger.warning("numexpr: Zero division error in formula.")
+        safe_numexpr_eval.err = 6
 
     if np_expr is None:
         return None  # no fallback, no error checking!
 
     # check if dimensions of converted string agrees with expected dimensions
     elif np.ndim(np_expr) != np.ndim(fallback):
         if np.ndim(np_expr) == 0:
             # np_expr is scalar, return array with shape of fallback of constant values
             np_expr = np.ones(fallback_shape) * np_expr
         else:
             # return array of zeros in the shape of the fallback
             logger.warning(
                 f"numexpr: Expression has unexpected dimension {np.ndim(np_expr)}!")
+            safe_numexpr_eval.err = 11
+
             np_expr = np.zeros(fallback_shape)
 
     if np.shape(np_expr) != fallback_shape:
         logger.warning(
             f"numexpr: Expression has unsuitable length {np.shape(np_expr)[0]}!")
+        safe_numexpr_eval.err = 12
+
         np_expr = np.zeros(fallback_shape)
 
     if not type(np_expr.item(0)) in {float, complex}:
         np_expr = np_expr.astype(float)
 
     return np_expr
 
 
 # ------------------------------------------------------------------------------
-def safe_eval(expr, alt_expr=0, return_type="float", sign=None):
+def safe_eval(expr, alt_expr=0, return_type: str = "float", sign: str = None) -> str:
     """
     Try ... except wrapper around numexpr to catch various errors
     When evaluation fails or returns `None`, try evaluating `alt_expr`.
     When this also fails, return 0 to avoid errors further downstream.
 
     Parameters
     ----------
@@ -559,17 +619,17 @@
     -------
     the evaluated result or 0 when both arguments fail: float (default) / complex / int
 
 
     Function attribute `err` contains number of errors that have occurred during
     evaluation (0 / 1 / 2)
     """
-    # convert to str (PY3) resp. unicode (PY2) and remove non-ascii characters
-    expr = clean_ascii(qstr(expr))
-    alt_expr = clean_ascii(qstr(alt_expr))
+    # convert to str and remove non-ascii characters
+    expr = clean_ascii(str(expr))
+    alt_expr = clean_ascii(str(alt_expr))
 
     result = None
     fallback = ""
     safe_eval.err = 0  # initialize function attribute
 
     for ex in [expr, alt_expr]:
         if ex == "":
@@ -691,23 +751,19 @@
         html = "<i>" + html + "</i>"
     if frmt in {'b', 'bi', 'ib'}:
         html = "<b>" + html + "</b>"
     if frmt is None:
         html = "<span>" + html + "</span>"
 
     if frmt != 'log':  # this is a label, not a logger message
-        # replace _xxx (terminated by whitespace) by <sub> xxx </sub> ()
-        html = re.sub(r'([<>a-zA-Z;])_(\w+)', r'\1<sub>\2</sub>', html)
-        # don't render numbers as italic
-#        if "<i>" in html:
-#            html = re.sub(r'([<>a-zA-Z;_])([0-9]+)',
-#                           r'\1<span class="font-style:normal">\2</span>', html)
-
-    # (^|\s+)(\w{1})_(\w*)  # check for line start or one or more whitespaces
-    # Replace group using $1$2<sub>$3</sub> (Py RegEx: \1\2<sub>\3</sub>)
+        # replace _xxx (where xxx are alphanumeric, non-space characters \w) by <sub> xxx </sub> ()
+        if "<i>" in html:  # make subscripts non-talic
+            html = re.sub(r'_(\w+)', r'</i><sub>\1</sub><i>', html)
+        else:
+            html = re.sub(r'_(\w+)', r'<sub>\1</sub>', html)
 
     return html
 
 
 # ##############################################################################
 # ###     Scipy-like    ########################################################
 # ##############################################################################
@@ -1345,38 +1401,53 @@
     """
 
     if format_in == 'sos':
         fil_dict['sos'] = arg
         fil_dict['ft'] = 'IIR'
 
     elif format_in == 'zpk':
-        if any(isinstance(el, list) for el in arg):
-            frmt = "lol"  # list or ndarray or tuple of lists
+        if isinstance(arg, np.ndarray) and np.ndim(arg) == 1:
+            frmt = "nd1"
+            logger.info(f"Format (zpk) is '{frmt}', shape = {np.shape(arg)}")
+        elif isinstance(arg, np.ndarray) and np.ndim(arg) == 2:
+            frmt = "nd2"
+            logger.info(f"Format (zpk) is '{frmt}', shape = {np.shape(arg)}")
+        # elif any(isinstance(el, list) for el in arg):
+        #     frmt = "lol"  # list or ndarray or tuple of lists
         elif any(isinstance(el, np.ndarray) for el in arg):
-            frmt = "lon"  # list or ndarray or tuple of ndarrays
-        elif isinstance(arg, list):
-            frmt = "lst"
-        elif isinstance(arg, np.ndarray):
-            frmt = "nd"
+            frmt = "lon"  # list or tuple of ndarrays
+            logger.warning(f"Format (zpk) is '{frmt}'.")
+        # elif isinstance(arg, list):
+        #     frmt = "lst"
+
         format_error = False
 
-        if frmt in {'lst', 'nd'}:  # list / array with z only -> FIR
+        if frmt == "nd2":
+            fil_dict['zpk'] = arg
+            if np.any(arg[1]):  # non-zero poles -> IIR
+                fil_dict['ft'] = 'IIR'
+            else:
+                fil_dict['ft'] = 'FIR'
+
+        elif frmt == 'nd1':  # list / array with z only -> FIR
             z = arg
             p = np.zeros(len(z))
-            k = 1
-            fil_dict['zpk'] = [z, p, k]
+            gain = zeros_with_val(len(z))  # create gain vector [1, 0, 0, ...]
+            fil_dict['zpk'] = np.array([z, p, gain])
             fil_dict['ft'] = 'FIR'
-        elif frmt in {'lol', 'lon'}:  # list of lists
+
+        elif frmt == 'lon':  # list of  ndarrays
             if len(arg) == 3:
-                fil_dict['zpk'] = [arg[0], arg[1], arg[2]]
+                fil_dict['zpk'] = np.array([arg[0], arg[1], arg[2]])
                 if np.any(arg[1]):  # non-zero poles -> IIR
                     fil_dict['ft'] = 'IIR'
                 else:
                     fil_dict['ft'] = 'FIR'
             else:
+                logger.error(f"{len(arg)} rows instead of 3!")
                 format_error = True
         else:
             format_error = True
 
 # =============================================================================
 #         if np.ndim(arg) == 1:
 #             if np.ndim(arg[0]) == 0: # list / array with z only -> FIR
@@ -1443,22 +1514,14 @@
 
     else:
         raise ValueError("\t'fil_save()':Unknown input format {0:s}".format(format_in))
 
     fil_dict['creator'] = (format_in, sender)
     fil_dict['timestamp'] = time.time()
 
-    # Remove any antiCausal zero/poles
-    if 'zpkA' in fil_dict:
-        fil_dict.pop('zpkA')
-    if 'baA' in fil_dict:
-        fil_dict.pop('baA')
-    if 'rpk' in fil_dict:
-        fil_dict.pop('rpk')
-
     if convert:
         fil_convert(fil_dict, format_in)
 
 
 # ------------------------------------------------------------------------------
 def fil_convert(fil_dict: dict, format_in) -> None:
     """
@@ -1503,24 +1566,27 @@
                 a1 = chk[section, 3:]
                 if ((np.amin(b1)) < 1e-14 and np.amin(b1) > 0):
                     raise ValueError(
                         "\t'fil_convert()': Bad coefficients, Order N is too high!")
 
         if 'zpk' not in format_in:
             try:
-                fil_dict['zpk'] = list(sig.sos2zpk(fil_dict['sos']))
+                # returns a tuple (zeros, poles, gain) where gain is scalar:
+                zpk = list(sig.sos2zpk(fil_dict['sos']))
             except Exception as e:
                 raise ValueError(e)
             # check whether sos conversion has created a additional (superfluous)
             # pole and zero at the origin and delete them:
-            z_0 = np.where(fil_dict['zpk'][0] == 0)[0]
-            p_0 = np.where(fil_dict['zpk'][1] == 0)[0]
+            z_0 = np.where(zpk[0] == 0)[0]
+            p_0 = np.where(zpk[1] == 0)[0]
             if p_0 and z_0:  # eliminate z = 0 and p = 0 from list:
-                fil_dict['zpk'][0] = np.delete(fil_dict['zpk'][0], z_0)
-                fil_dict['zpk'][1] = np.delete(fil_dict['zpk'][1], p_0)
+                zpk[0] = np.delete(zpk[0], z_0)
+                zpk[1] = np.delete(zpk[1], p_0)
+            fil_dict['zpk'] = np.array(
+                [zpk[0], zpk[1], zeros_with_val(len(zpk[0]), zpk[2])], dtype=complex)
 
         if 'ba' not in format_in:
             try:
                 fil_dict['ba'] = list(sig.sos2tf(fil_dict['sos']))
             except Exception as e:
                 raise ValueError(e)
             # check whether sos conversion has created additional (superfluous)
@@ -1529,33 +1595,34 @@
                 fil_dict['ba'][0] = np.delete(fil_dict['ba'][0], -1)
                 fil_dict['ba'][1] = np.delete(fil_dict['ba'][1], -1)
 
     elif 'zpk' in format_in:  # z, p, k have been generated,convert to other formats
         zpk = fil_dict['zpk']
         if 'ba' not in format_in:
             try:
-                fil_dict['ba'] = sig.zpk2tf(zpk[0], zpk[1], zpk[2])
+                fil_dict['ba'] = sig.zpk2tf(zpk[0], zpk[1], zpk[2][0])
             except Exception as e:
                 raise ValueError(e)
         if 'sos' not in format_in:
             fil_dict['sos'] = []  # don't convert zpk -> SOS due to numerical inaccuracies
 #            try:
 #                fil_dict['sos'] = sig.zpk2sos(zpk[0], zpk[1], zpk[2])
 #            except ValueError:
 #                fil_dict['sos'] = []
 #                logger.warning("Complex-valued coefficients, could not convert to SOS.")
 
     elif 'ba' in format_in:  # arg = [b,a]
         b, a = fil_dict['ba'][0], fil_dict['ba'][1]
         if np.all(np.isfinite([b, a])):
             zpk = sig.tf2zpk(b, a)
-            fil_dict['zpk'] = [np.nan_to_num(zpk[0]).astype(complex),
-                               np.nan_to_num(zpk[1]).astype(complex),
-                               np.nan_to_num(zpk[2])
-                               ]
+            fil_dict['zpk'] = np.array(
+                [np.nan_to_num(zpk[0]).astype(complex),
+                 np.nan_to_num(zpk[1]).astype(complex),
+                 np.nan_to_num(zeros_with_val(len(zpk[0]), zpk[2]))
+                ], dtype=complex)
         else:
             raise ValueError(
                 "\t'fil_convert()': Cannot convert coefficients with NaN or Inf elements "
                 "to zpk format!")
             zpk = None
         fil_dict['sos'] = []  # don't convert ba -> SOS due to numerical inaccuracies
 #        if SOS_AVAIL:
```

### Comparing `pyfda-0.7.1/pyfda/libs/pyfda_log_template.conf` & `pyfda-0.8.0a2/pyfda/libs/pyfda_log_template.conf`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/libs/pyfda_qt_lib.py` & `pyfda-0.8.0a2/pyfda/libs/pyfda_qt_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 Library with various helper functions for Qt widgets
 """
 from .pyfda_lib import qstr, pprint_log
 
 from .compat import (
     Qt, QtGui, QtCore, QFrame, QMessageBox, QPushButton, QLabel, QComboBox, QDialog,
-    QFont, QSize, QFontMetrics, QIcon)
+    QFont, QSize, QFontMetrics, QIcon, QEvent)
 from .pyfda_dirs import OS, OS_VER
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------
@@ -25,25 +25,29 @@
     """
     Emit a signal `self.<sig_name>` (defined as a class attribute) with a
     dict `dict_sig` using Qt's `emit()`.
     - Add the keys `'id'` and `'class'` with id resp. class name of the calling
       instance if not contained in the dict
     - If key 'ttl' is in the dict and its value is less than one, terminate the
       signal. Otherwise, reduce the value by one.
+    - If the sender has passed an objectName, add it with the key "sender_name"
+      to the dict.
     """
     if 'id' not in dict_sig:
         dict_sig.update({'id': id(self)})
     if 'class' not in dict_sig:
         dict_sig.update({'class': self.__class__.__name__})
     # Count down time-to-live counter and terminate the signal when ttl < 1
     if 'ttl' in dict_sig:
         if dict_sig['ttl'] < 1:
             return
         else:
             dict_sig.update({'ttl': dict_sig['ttl'] - 1})
+    if self.sender() and self.sender().objectName():
+        dict_sig.update({'sender_name': self.sender().objectName()})
     # Get signal (default name: `sig_tx`) from calling instance and emit it
     signal = getattr(self, sig_name)
     signal.emit(dict_sig)
 
 
 # # ------------------------------------------------------------------------------
 # def sig_loop(self, dict_sig: dict, logger, **kwargs) -> int:
@@ -125,27 +129,64 @@
     cmb_box.clear()
     if type(items_list[0]) is str:  # combo box tool tipp (optional)
         cmb_box.setToolTip(cmb_box.tr(items_list[0]))
     for i in range(1, len(items_list)):
         if type(items_list[i][1]) == QtGui.QIcon:
             cmb_box.addItem("", items_list[i][0])
             cmb_box.setItemIcon(i-1, items_list[i][1])
-            # cmb_box.setItemData(i-1, items_list[i][0])
         else:
             cmb_box.addItem(cmb_box.tr(items_list[i][1]), items_list[i][0])
         if len(items_list[i]) == 3:  # add item tool tip (optional)
             cmb_box.setItemData(i-1, cmb_box.tr(items_list[i][2]), Qt.ToolTipRole)
     qset_cmb_box(cmb_box, item_init, data=True)
 
     """ icon = QIcon('logo.png')
     # adding icon to the given index
     self.combo_box.setItemIcon(i, icon)
     size = QSize(10, 10)
     self.combo_box.setIconSize(size)  """
 
+# ------------------------------------------------------------------------------
+def qcmb_box_add_items(cmb_box: QComboBox, items_list: list) -> None:
+    """
+    Add items to combo box `cmb_box` with text, data and tooltip from the list
+    `items_list`.
+
+    Text and tooltip are prepared for translation via `self.tr()`
+
+    Parameters
+    ----------
+
+    cmb_box: instance of QComboBox
+        Combobox to be populated
+
+    items_list: list
+        List of combobox entries, in the format
+         ("data 1st item", "text 1st item", "tooltip for 1st item" # [optional]),
+         ("data 2nd item", "text 2nd item", "tooltip for 2nd item")]
+
+    Returns
+    -------
+    None
+    """
+    for i in range(0, len(items_list)):
+        if type(items_list[i][1]) == QtGui.QIcon:
+            cmb_box.addItem("", items_list[i][0])
+            cmb_box.setItemIcon(i-1, items_list[i][1])
+        else:
+            cmb_box.addItem(cmb_box.tr(items_list[i][1]), items_list[i][0])
+        if len(items_list[i]) == 3:  # add item tool tip (optional)
+            cmb_box.setItemData(i-1, cmb_box.tr(items_list[i][2]), Qt.ToolTipRole)
+
+    """ icon = QIcon('logo.png')
+    # adding icon to the given index
+    self.combo_box.setItemIcon(i, icon)
+    size = QSize(10, 10)
+    self.combo_box.setIconSize(size)  """
+
 
 # ------------------------------------------------------------------------------
 def qget_cmb_box(cmb_box: QComboBox, data: bool = True) -> str:
     """
     Get current itemData or Text of comboBox and convert it to string.
 
     In Python 3, python Qt objects are automatically converted to QVariant
@@ -341,15 +382,15 @@
 
 # ------------------------------------------------------------------------------
 def qstyle_widget(widget, state):
     """
     Apply the "state" defined in pyfda_rc.py to the widget, e.g.:
     Color the >> DESIGN FILTER << button according to the filter design state.
 
-    This requires settinng the property, "unpolishing" and "polishing" the widget
+    This requires setting the property, "unpolishing" and "polishing" the widget
     and finally forcing an update.
 
     - "normal": default, no color styling
     - "ok":  green, filter has been designed, everything ok
     - "changed": yellow, filter specs have been changed
     - "running": orange, simulation is running
     - "error" : red, an error has occurred during filter design
@@ -363,14 +404,15 @@
         state = "unused"
         # *[state="unused"], *[state="u"]{background-color:white; color:darkgrey}
     elif state == 'a':
         state = "active"
     elif state == 'd':
         state = "disabled"
         # QLineEdit:disabled{background-color:darkgrey;}
+    # widget.setAttribute(Qt.WA_StyledBackground, True)
     widget.setProperty("state", state)
     widget.style().unpolish(widget)
     widget.style().polish(widget)
     widget.update()
 
 
 # ----------------------------------------------------------------------------
@@ -530,14 +572,48 @@
     #     wdg.contentsMargins().left() + wdg.contentsMargins().left() +\
     #     8  # 2 * horizontalMargin() + 2 * frame margin.
 
     # fm = QFontMetrics(loggerWin.font())
     # row4_height = fm.lineSpacing() * 4
     # fm_size = fm.size(0, text)
 
+# ----------------------------------------------------------------------------
+class EventTypes:
+    """
+    https://stackoverflow.com/questions/62196835/how-to-get-string-name-for-qevent-in-pyqt5
+    Events in Qt5: https://doc.qt.io/qt-5/qevent.html
+
+    Stores a string name for each event type.
+
+    With PySide2 str() on the event type gives a nice string name,
+    but with PyQt5 it does not. So this method works with both systems.
+
+    Example usage (simultaneous initialization and method call / translation)
+    > event_str = EventTypes().as_string(QEvent.UpdateRequest)
+    > assert event_str == "UpdateRequest"
+
+    Example usage, separate initialization and method call
+    > event types = EventTypes()
+    > event_str = event_types.as_string(event.type())
+    """
+
+    def __init__(self):
+        """Create mapping for all known event types."""
+        self.string_name = {}
+        for name in vars(QEvent):
+            attribute = getattr(QEvent, name)
+            if type(attribute) == QEvent.Type:
+                self.string_name[attribute] = name
+
+    def as_string(self, event: QEvent.Type) -> str:
+        """Return the string name for this event."""
+        try:
+            return self.string_name[event]
+        except KeyError:
+            return f"UnknownEvent:{event}"
 
 # ----------------------------------------------------------------------------
 class QHLine(QFrame):
     """
     Create a thin horizontal line utilizing the HLine property of QFrames
     Usage:
         myline = QHLine()
```

### Comparing `pyfda-0.7.1/pyfda/libs/pyfda_sig_lib.py` & `pyfda-0.8.0a2/pyfda/libs/pyfda_sig_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,17 +90,42 @@
     hn = np.array(sig.lfilter(b, a, impulse))  # calculate impulse response
     td = np.arange(len(hn)) / FS
 
     if step:  # calculate step response
         hn = np.cumsum(hn)
 
     return hn, td
+# --------------------------------------------------------------------------
+def zeros_with_val(N: int, val: float = 1., pos: int = 0):
+    """
+    Create a 1D array of `N` zeros where the element at position `pos` has the
+    value `val`.
+
+    Parameters
+    ----------
 
+    N: int
+        number of elements
+    val: scalar
+        value to be inserted at position `pos` (default: 1)
+    pos: int
+        Position of `val` to be inserted (default: 0)
+
+    Returns
+    -------
+    arr: np.ndarray
+       Array with zeros except for element at position `pos`
+    """
+    if pos >= N or -pos > N:
+        raise(IndexError)
+    a = np.zeros(N)
+    a[pos] = val
+    return a
 
-# ------------------------------------------------------------------------------
+# ------------------- -----------------------------------------------------------
 def angle_zero(X, n_eps=1e3, mode='auto', wrapped='auto'):
 
     """
     Calculate angle of argument `X` when abs(X) > `n_eps` * machine resolution.
     Otherwise, zero is returned.
     """
```

### Comparing `pyfda-0.7.1/pyfda/libs/pyfda_template.conf` & `pyfda-0.8.0a2/pyfda/libs/pyfda_template.conf`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/libs/tree_builder.py` & `pyfda-0.8.0a2/pyfda/libs/tree_builder.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/license_info.md` & `pyfda-0.8.0a2/pyfda/license_info.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/module_versions.md` & `pyfda-0.8.0a2/pyfda/module_versions.md`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/mpl_widget.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/mpl_widget.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 from matplotlib import rcParams
 from matplotlib import lines
 from matplotlib.pyplot import setp
 
 try:
     MPL_CURS = True
     import mplcursors
-    if cmp_version('matplotlib', '3.1') < 0:
-        MPL_CURS = False
 except ImportError:
     MPL_CURS = False
+
 try:
     import matplotlib.backends.qt_editor.figureoptions as figureoptions
 except ImportError:
     figureoptions = None
 
 from pyfda.libs.compat import (
-    QtCore, QtGui, QWidget, QLabel, pyqtSignal, QSizePolicy, QIcon, QImage, QVBoxLayout,
-    QHBoxLayout, QInputDialog, FigureCanvas, NavigationToolbar, pyqtSlot, QtWidgets)
+    Qt, QtCore, QtGui, QWidget, QLabel, pyqtSignal, QSizePolicy, QIcon, QImage, QVBoxLayout,
+    QHBoxLayout, QInputDialog, FigureCanvas, NavigationToolbar, pyqtSlot, QtWidgets, QEvent)
+
+from pyfda.libs.pyfda_qt_lib import EventTypes
 
 from pyfda import pyfda_rc
 import pyfda.filterbroker as fb
 from pyfda import qrc_resources  # contains all icons
 
 import logging
 logger = logging.getLogger(__name__)
@@ -101,111 +102,130 @@
     """
     Construct a subwidget consisting of a Matplotlib canvas and a subclassed
     NavigationToolbar.
     """
 
     def __init__(self, parent):
         super(MplWidget, self).__init__(parent)
+
+        # initialize dict for translation of events to strings
+        self.event_types = EventTypes()
+
         # Create the mpl figure and subplot (white bg, 100 dots-per-inch).
         # Construct the canvas with the figure:
         self.plt_lim = []  # define variable for x,y plot limits
 
-        if cmp_version("matplotlib", "2.2.0") >= 0:
-            self.fig = Figure(constrained_layout=True)
-        else:
-            self.fig = Figure()
+        self.fig = Figure(constrained_layout=True)
 
         self.canvas = FigureCanvas(self.fig)
         self.canvas.setSizePolicy(QSizePolicy.Expanding,
                                   QSizePolicy.Expanding)
 
         # Needed for mouse modifiers (x,y, <CTRL>, ...):
         #    Key press events in general are not processed unless you
         #    "activate the focus of Qt onto your mpl canvas"
         # http://stackoverflow.com/questions/22043549/matplotlib-and-qt-mouse-press-event-key-is-always-none
-
-        self.canvas.setFocusPolicy(QtCore.Qt.ClickFocus)
-        self.canvas.setFocus()
+        self.canvas.setFocusPolicy(Qt.ClickFocus)  # Qt.StrongFocus
+        # self.canvas.setFocus()
 
         self.canvas.updateGeometry()
 
+        self.canvas.installEventFilter(self)
+
         # Create a custom navigation toolbar, tied to the canvas and
-        # initialize toolbar settings
+        # initialize toolbar settings. Send events through event filter
         #
         self.mplToolbar = MplToolbar(self.canvas, self)
         self.mplToolbar.zoom_locked = False
         self.mplToolbar.cursor_enabled = False
-        # self.mplToolbar.enable_plot(state = True)
-        self.mplToolbar.sig_tx.connect(self.process_signals)
+        self.mplToolbar.plot_enabled = True
+        self.mplToolbar.save_button_states()  # store initial setting of buttons
+
+        # self.mplToolbar.sig_rx.connect(self.sig_rx)  # TODO: Doesn't exist yet
+
         layHToolbar = QHBoxLayout()
-        layHToolbar.addWidget(self.mplToolbar, 1, QtCore.Qt.AlignLeft)
+        layHToolbar.addWidget(self.mplToolbar, 1, Qt.AlignLeft)
         layHToolbar.addStretch(1)
 
         # =============================================
         # Main plot widget layout
         # =============================================
         self.layVMainMpl = QVBoxLayout()
         self.layVMainMpl.addLayout(layHToolbar)
         self.layVMainMpl.addWidget(self.canvas)
 
         self.setLayout(self.layVMainMpl)
 
 # ------------------------------------------------------------------------------
-    @pyqtSlot(object)
-    def process_signals(self, dict_sig):
-        """
-        Process sig
+    def eventFilter(self, source, event):
         """
-#        if 'enabled' in dict_sig:
-#            self.clear_disabled_figure(dict_sig['enabled'])
-#        else:
-        pass
+        Filter all events generated by the monitored widgets (self).
+        Source and type of all events generated by monitored objects are passed
+         to this eventFilter, evaluated and passed on to the next hierarchy level.
+        """
+        modifiers = QtWidgets.QApplication.keyboardModifiers()
+        # if event.type() in {QEvent.KeyPress, QEvent.Wheel, QtGui.QMouseEvent.MouseButtonPress,
+        #                     QEvent.KeyRelease}:
+        #     logger.info(self.event_types.as_string(event.type()))
+        if event.type() == QEvent.KeyPress:
+            key = event.key()
+            # logger.warning(key)
+            # check for "normal" keys, skip x and y (used as mouse modifiers)
+            if key < 256 and key != 88 and key != 89:
+                modifiers = event.modifiers()
+                meta = modifiers & Qt.AltModifier == Qt.AltModifier\
+                    or modifiers & Qt.MetaModifier == Qt.MetaModifier
+                ctrl = modifiers & Qt.ControlModifier == Qt.ControlModifier
+                shift = modifiers & Qt.ShiftModifier == Qt.ShiftModifier
+
+                # logger.warning(f"Key = {key}, meta = {meta}, ctrl = {ctrl}, shift = {shift}")
+                if key == 67 and ctrl:  # "ctrl-c"
+                    self.mplToolbar.mpl2Clip(key_event=True)
+
+        # elif event.type() == QtGui.QMouseEvent.MouseButtonPress:
+        #     logger.warning("Mouse Event")
+        # if event.type() == QEvent.Wheel:
+        #     logger.warning(event.angleDelta().y())
+
+        # else:
+        #     # do other weird things
+        #     pass
+
+        # Call base class method to continue normal event processing:
+        return super().eventFilter(source, event)
 
 # ------------------------------------------------------------------------------
     def save_limits(self):
         """
         Save x- and y-limits of all axes in self.limits when zoom is unlocked
         """
         if not self.mplToolbar.zoom_locked:
             for ax in self.fig.axes:
                 self.limits = ax.axis()  # save old limits
 
 # ------------------------------------------------------------------------------
     def redraw(self):
         """
-        Redraw the figure with new properties (grid, linewidth)
+        Redraw the figure with new properties (grid, linewidth) and restore the plot
+        limits when `zoom_locked` is True
+
+        When zoom lock is used and / or plot limits shall be pushed into the queue,
+        you need to call redraw()
         """
-        # only execute when at least one axis exists -> tight_layout crashes otherwise
         if self.fig.axes:
             self.mplToolbar.cycle_draw_grid(cycle=False, axes=self.fig.axes)
             for ax in self.fig.axes:
 
                 if self.mplToolbar.zoom_locked:
                     ax.axis(self.limits)  # restore old limits
                 else:
                     self.limits = ax.axis()  # save old limits
 
-#            try:
-#                # tight_layout() crashes with small figure sizes
-#               self.fig.tight_layout(pad = 0.1)
-#            except(ValueError, np.linalg.linalg.LinAlgError):
-#                logger.debug("error in tight_layout")
         self.canvas.draw()  # now (re-)draw the figure
 
-# ------------------------------------------------------------------------------
-#    def clear_disabled_figure(self, enabled):
-#        """
-#        Clear the figure when it is disabled in the mplToolbar
-#        """
-#        if not enabled:
-#            self.fig.clf()
-#            self.pltCanv.draw()
-#        else:
-#            self.redraw()
-
 # ----------------------------------------------------------------------------
     def plt_full_view(self):
         """
         Zoom to full extent of data if axes is set to "navigationable"
         by the navigation toolbar
         """
         # Add current view limits to view history to enable "back to previous view"
@@ -241,15 +261,16 @@
             self.mplToolbar.cursor_enabled = not self.mplToolbar.cursor_enabled
             if self.mplToolbar.cursor_enabled:
                 if hasattr(self, "cursors"):  # dangling references to old cursors?
                     for i in range(len(self.cursors)):
                         self.cursors[i].remove()         # yes, remove them!
                 self.cursors = []
                 for ax in self.fig.axes:
-                    if ax.__class__.__name__ in {"AxesSubplot", "Axes3DSubplot"}:
+                    if ax.__class__.__name__ in {"AxesSubplot", "Axes3DSubplot",
+                                                 "Axes", "Axes3D"}:
                         self.cursors.append(mplcursors.cursor(ax, hover=True))
             else:
                 for i in range(len(self.cursors)):
                     self.cursors[i].remove()
 
         # see https://stackoverflow.com/questions/59800059/how-to-use-two-mplcursors-simultaneously-for-a-scatter-plot-of-two-sets
 
@@ -280,14 +301,20 @@
     http://stackoverflow.com/questions/15876011/add-information-to-matplotlib-navigation-toolbar-status-bar
     https://stackoverflow.com/questions/53099295/matplotlib-navigationtoolbar-advanced-figure-options
 
     Using Tool Manager
     https://matplotlib.org/3.1.1/gallery/user_interfaces/toolmanager_sgskip.html
     https://stackoverflow.com/questions/52971285/add-toolbar-button-icon-matplotlib
 
+    Documentation on QKeySequences:
+    https://doc.qt.io/qt-6/qkeysequence.html
+
+    Construct a shortcut string:
+    logger.info(QtGui.QKeySequence.toString(QtGui.QKeySequence(Qt.SHIFT|Qt.CTRL|Qt.Key_Z)))
+
     """
 
     toolitems = ()  # remove original icons and actions
 #    toolitems = (
 #        ('Home', 'Reset original view', 'home', 'home'),
 #        ('Back', 'Back to  previous view', 'action-undo', 'back'),
 #        ('Forward', 'Forward to next view', 'action-redo', 'forward'),
@@ -301,187 +328,224 @@
 
 # subclass NavigationToolbar, passing through arguments:
     # def __init__(self, canvas, parent, coordinates=True):
 
     sig_tx = pyqtSignal(object)  # general signal, containing a dict
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def _init_toolbar(self): pass  # needed for backward compatibility with mpl < 3.3
+    def _init_toolbar(self):
+        pass  # needed for backward compatibility with mpl < 3.3
 
-    # disable coordinate display when mplcursors is available
-    if MPL_CURS:
-        def set_message(self, msg): pass
+    # turn off coordinate display
+    def set_message(self, msg):
+        pass
 
     def __init__(self, canv, mpl_widget, *args, **kwargs):
         NavigationToolbar.__init__(self, canv, mpl_widget, *args, **kwargs)
 
-        # self.canvas = canv
-        self.mpl_widget = mpl_widget
+        self.mpl_widget = mpl_widget  # create a reference to the parent
 
     # --------------------------------------------------------------------------
     # ----  Construct Toolbar using QRC icons -------------------
 
         # ---------------------------------------------
-        # ENABLE:
+        # Enable Plot:
         # ---------------------------------------------
         self.a_en = self.addAction(QIcon(':/circle-check.svg'), 'Enable Update',
                                    self.enable_plot)
         self.a_en.setToolTip('Enable / disable plot')
         self.a_en.setCheckable(True)
         self.a_en.setChecked(True)
-        self.a_en.setVisible(False)
+        self.a_en.setVisible(False)  # invisible by default, only needed by y[n]
 
-        # self.addSeparator()
+        # ---------------------------------------------
+        # UI Detail Level:
+        # ---------------------------------------------
+        self.a_ui = self.addAction(
+            QIcon(':/ui_level_max'), 'UI detail', self.cycle_ui_level)
+        self.a_ui.setToolTip('Show / hide UI elements (CTRL-U)')
+        self.a_ui_num_levels = 3
+        self.a_ui_level = 0  # 0: full ui, 1: reduced, 2: compact ui
+        self.a_ui.setShortcut('Ctrl+U')
+
+        # ---------------------------------------------
+        self.addSeparator()
+        # ---------------------------------------------
 
         # ---------------------------------------------
         # HOME:
         # ---------------------------------------------
         self.a_ho = self.addAction(QIcon(':/home.svg'), 'Home', self.home)
-        self.a_ho.setToolTip('Reset zoom')
+        self.a_ho.setToolTip('Home zoom setting (Ctrl+H)')
+        self.a_ho.setShortcut('Ctrl+H')
+
+        # ---------------------------------------------
         # BACK:
+        # ---------------------------------------------
+        # self.ba = QtWidgets.QAction(QIcon(':/action-undo.svg'), '&Undo', self)
+        # self.ba.setIcon(QIcon(':/action-undo.svg'))
+        # self.ba.setShortcut('Ctrl+Z')
+        # self.ba.triggered.connect(self.back)
+        # self.addAction(self.ba)
         self.a_ba = self.addAction(QIcon(':/action-undo.svg'), 'Back', self.back)
-        self.a_ba.setToolTip('Back to previous zoom')
+        self.a_ba.setToolTip('Back to previous zoom (CTRL+Z)')
+        self.a_ba.setShortcut('Ctrl+Z')
 
         # ---------------------------------------------
         # FORWARD:
         # ---------------------------------------------
         self.a_fw = self.addAction(QIcon(':/action-redo.svg'), 'Forward', self.forward)
-        self.a_fw.setToolTip('Forward to next zoom')
+        self.a_fw.setToolTip('Forward to next zoom (CTRL+SHIFT+Z or CTRL+Y)')
+        self.a_fw.setShortcuts(['Ctrl+Shift+Z', 'Ctrl+Y'])
+        # self.a_fw.setShortcut(QtGui.QKeySequence(Qt.SHIFT|Qt.CTRL|Qt.Key_Z))
 
         # ---------------------------------------------
         self.addSeparator()
         # ---------------------------------------------
 
         # ---------------------------------------------
         # PAN:
         # ---------------------------------------------
         self.a_pa = self.addAction(QIcon(':/move.svg'), 'Pan', self.pan)
         self.a_pa.setToolTip(
-            "Pan axes with left mouse button, zoom with right,\npressing x / y / CTRL "
+            "Pan axes (Ctrl+P) with left mouse button, zoom with right,\npressing x / y / CTRL "
             "keys constrains to horizontal / vertical / diagonal movements.")
         self._actions['pan'] = self.a_pa
         self.a_pa.setCheckable(True)
+        self.a_pa.setShortcut('Ctrl+P')
 
         # ---------------------------------------------
         # ZOOM RECTANGLE:
         # ---------------------------------------------
         self.a_zo = self.addAction(QIcon(':/magnifying-glass.svg'), 'Zoom', self.zoom)
         self.a_zo.setToolTip(
-            "Zoom in / out to rectangle with left / right mouse button,\n"
+            "Zoom in / out to rectangle (Ctrl+O) with left / right mouse button,\n"
             "pressing x / y keys constrains zoom to horizontal / vertical direction.")
         self._actions['zoom'] = self.a_zo
         self.a_zo.setCheckable(True)
+        self.a_zo.setShortcut('Ctrl+O')
 
         # ---------------------------------------------
         # FULL VIEW:
         # ---------------------------------------------
         self.a_fv = self.addAction(
             QIcon(':/fullscreen-enter.svg'),
             'Zoom full extent', self.mpl_widget.plt_full_view)
-        self.a_fv.setToolTip('Zoom to full extent')
+        self.a_fv.setToolTip('Zoom to full extent (Ctrl+F)')
+        self.a_fv.setShortcut("Ctrl+F")
 
         # ---------------------------------------------
         # LOCK ZOOM:
         # ---------------------------------------------
         self.a_lk = self.addAction(QIcon(':/lock-unlocked.svg'),
                                    'Lock zoom', self.toggle_lock_zoom)
         self.a_lk.setCheckable(True)
         self.a_lk.setChecked(False)
-        self.a_lk.setToolTip('Lock / unlock current zoom setting')
+        self.a_lk.setToolTip('Lock / unlock current zoom setting (Ctrl+L)')
+        self.a_lk.setShortcut("Ctrl+L")
 
         # ---------------------------------------------
         # TRACKING CURSOR:
         # ---------------------------------------------
         if MPL_CURS:
             self.a_cr = self.addAction(QIcon(':/map-marker.svg'),
                                        'Cursor', self.mpl_widget.toggle_cursor)
             self.a_cr.setCheckable(True)
             self.a_cr.setChecked(False)
-            self.a_cr.setToolTip('Tracking Cursor')
+            self.a_cr.setToolTip('Tracking Cursor (Ctrl+T)')
+            self.a_cr.setShortcut("Ctrl+T")
 
         # --------------------------------------
         self.addSeparator()
         # --------------------------------------
 
         # ---------------------------------------------
         # GRID:
         # ---------------------------------------------
         self.a_gr = self.addAction(
             QIcon(':/grid_coarse.svg'), 'Grid', self.cycle_draw_grid)
-        self.a_gr.setToolTip('Cycle grid: Off / coarse / fine')
+        self.a_gr.setToolTip('Cycle grid: Off / coarse / fine (Ctrl+G)')
         self.a_gr_state = 2  # 0: off, 1: major, 2: minor
+        self.a_gr.setShortcut("Ctrl+G")
 
         # ---------------------------------------------
         # REDRAW:
         # ---------------------------------------------
         # self.a_rd = self.addAction(QIcon(':/brush.svg'), 'Redraw', self.mpl_widget.redraw)
         # self.a_rd.setToolTip('Redraw Plot')
 
         # --------------------------------------
         # SAVE:
         # --------------------------------------
         self.a_sv = self.addAction(QIcon(':/save.svg'), 'Save', self._save_figure)
-        self.a_sv.setToolTip('<span>Save the figure in various file formats. '
-                             'Press &lt;ALT&gt; to hide title.</span>')
-        self.cb = fb.clipboard
+        self.a_sv.setToolTip('<span>Save the figure in various file formats (Ctrl+S). '
+                             'Press &lt;SHIFT&gt; to hide title.</span>')
+        self.a_sv.setShortcut("Ctrl+S")
 
         # --------------------------------------
         # Copy to clipboard:
         # --------------------------------------
+        self.cb = fb.clipboard
         self.a_cb = self.addAction(
             QIcon(':/clipboard.svg'), 'To Clipboard', self.mpl2Clip)
         self.a_cb.setToolTip(
-            '<span>Copy figure to clipboard in png format.'
-            '<ul><li>Press &lt;ALT&gt; to hide title.</li>'
-            '<li>Press &lt;SHIFT&gt; for base64 '
+            '<span>Copy figure to clipboard in png format (CTRL+C). '
+            'Modifiers:'
+            '<ul><li>&lt;SHIFT&gt; to hide title.</li> '
+            '<li>&lt;ALT&gt; (keyboard) resp. &lt;CTRL&gt; (mouse) for base64 '
             'encoded png format (e.g. for Jupyter Notebooks).</li> '
-            '<li>Press &lt;CTRL&gt; to '
-            'embed base64 encoded PNG in &lt;img&gt; tag.</li></ul></span>')
-        self.a_cb.setShortcut("Ctrl+C")
+            '</ul></span>')
+        # Don't set a shortcut here, as this jumps to `self.mpl2Clip` and
+        # interprets the CTRL key as a modifier!
+        # Decoding "CTRL+C" is performed in the event filter instead
 
         # --------------------------------------
         self.addSeparator()
         # --------------------------------------
 
         # --------------------------------------
         # SETTINGS:
         # --------------------------------------
         if figureoptions is not None:
             self.a_op = self.addAction(
                 QIcon(':/settings.svg'), 'Customize', self.edit_parameters)
-            self.a_op.setToolTip('Edit curves line and axes parameters')
+            self.a_op.setToolTip(self.tr('Edit curves line and axes parameters (Ctrl+E)'))
+            self.a_op.setShortcut(self.tr('Ctrl+E'))
 
 #        self.buttons = {}
 
-        # --------------------------------------
-        # PRINT COORDINATES (only when mplcursors is not available):
-        # --------------------------------------
-        # Add the x,y location widget at the right side of the toolbar
-        # The stretch factor is 1 which means any resizing of the toolbar
-        # will resize this label instead of the buttons.
-        # --------------------------------------
-        if not MPL_CURS and self.coordinates:
-            self.addSeparator()
-            self.locLabel = QLabel("", self)
-            self.locLabel.setAlignment(
-                    QtCore.Qt.AlignRight | QtCore.Qt.AlignTop)
-            self.locLabel.setSizePolicy(
-                QSizePolicy(QSizePolicy.Expanding,
-                            QSizePolicy.Ignored))
-            labelAction = self.addWidget(self.locLabel)
-            labelAction.setVisible(True)
+        # # --------------------------------------
+        # # PRINT COORDINATES (only when mplcursors is not available):
+        # # --------------------------------------
+        # # Add the x,y location widget at the right side of the toolbar
+        # # The stretch factor is 1 which means any resizing of the toolbar
+        # # will resize this label instead of the buttons.
+        # # --------------------------------------
+        # if not MPL_CURS and self.coordinates:
+        #     self.addSeparator()
+        #     self.locLabel = QLabel("", self)
+        #     self.locLabel.setAlignment(
+        #             Qt.AlignRight | Qt.AlignTop)
+        #     self.locLabel.setSizePolicy(
+        #         QSizePolicy(QSizePolicy.Expanding,
+        #                     QSizePolicy.Ignored))
+        #     labelAction = self.addWidget(self.locLabel)
+        #     labelAction.setVisible(True)
 
         # ---------------------------------------------
         # HELP:
         # ---------------------------------------------
         self.a_he = self.addAction(QIcon(':/help.svg'), 'help', self.help)
         self.a_he.setToolTip('Open help page from https://pyfda.rtfd.org in browser')
         self.a_he.setDisabled(True)
+        self.a_he.setShortcut(self.tr('F1'))
+# ------- end of __init__() ----------------------------------------------------------
+# ====================================================================================
+# ------------------------------------------------------------------------------------
 
-# ------------------------------------------------------------------------------
     if figureoptions is not None:
         def edit_parameters(self):
             allaxes = self.canvas.figure.get_axes()
             if len(allaxes) == 1:
                 axes = allaxes[0]
             else:
                 titles = []
@@ -515,16 +579,16 @@
 # ------------------------------------------------------------------------------
     def home(self):
         """
         Reset zoom to default settings (defined by plotting widget).
         This method shadows `home()` inherited from NavigationToolbar.
         """
         self.push_current()
-        self.emit({'home': ''})  # only the key is used by the slot
-        self.mpl_widget.redraw()
+        self.emit({'mpl_toolbar': 'home'})
+        self.mpl_widget.redraw()  # Redraw with saving / restoring plot limit
 
 # ------------------------------------------------------------------------------
     def help(self):
         """
         Open help page from https://pyfda.rtfd.org in browser
         """
 
@@ -536,14 +600,23 @@
             # if url.isLocalFile()
         QtGui.QDesktopServices.openUrl(url)
 
         # https://stackoverflow.com/questions/28494571/how-in-qt5-to-check-if-url-is-available
         # https://stackoverflow.com/questions/16778435/python-check-if-website-exists
 
 # ------------------------------------------------------------------------------
+    def save_button_states(self):
+        # Save enabled state of the following zoom-related UI elements
+        self.a_ho_prev_state = self.a_ho.isEnabled()  # home
+        self.a_pa_prev_state = self.a_pa.isEnabled()  # pan
+        self.a_zo_prev_state = self.a_zo.isEnabled()  # zoom
+        self.a_fv_prev_state = self.a_fv.isEnabled()  # full view
+        self.a_ho_prev_state = self.a_lk.isEnabled()  # lock zoom
+
+# ------------------------------------------------------------------------------
     def cycle_draw_grid(self, cycle=True, axes=None):
         """
         Cycle the grid of all axes through the states 'off', 'coarse' and 'fine'
         and redraw the figure.
 
         Parameters
         ----------
@@ -554,40 +627,70 @@
             When none is passed, use local `self.mpl_widget.fig.axes`
 
         Returns
         -------
         None.
 
         """
-
         if cycle:
             self.a_gr_state = (self.a_gr_state + 1) % 3
 
         if not axes:
             axes = self.mpl_widget.fig.axes
 
         for ax in self.mpl_widget.fig.axes:
             if hasattr(ax, "is_twin"):  # the axis is a twinx() system, suppress the gridlines
                 ax.grid(False)
             else:
                 if self.a_gr_state == 0:
                     ax.grid(False, which='both')
-
                     self.a_gr.setIcon(QIcon(':/grid_none.svg'))
                 elif self.a_gr_state == 1:
                     ax.grid(True, which='major', lw=0.75, ls='-')
                     ax.grid(False, which='minor')
                     self.a_gr.setIcon(QIcon(':/grid_coarse.svg'))
                 else:
                     ax.grid(True, which='major', lw=0.75, ls='-')
                     ax.grid(True, which='minor')
                     self.a_gr.setIcon(QIcon(':/grid_fine.svg'))
 
         if cycle:
-            self.canvas.draw()  # don't use self.draw(), use FigureCanvasQTAgg.draw()
+            self.canvas.draw()   # Redraw without saving / restoring plot limits
+
+# ------------------------------------------------------------------------------
+    def cycle_ui_level(self, ui_level : int = -1) -> None:
+        """
+        Cycle the UI level: UI elements fully / partially / invisible)
+
+        Parameters
+        ----------
+        ui_level : int, optional
+            Set the ui level and the icon accordingly when ui_level != -1,
+            (was not passed as a parameter), cycle through the `self.ai_num_levels`
+            and emit `{'mpl_toolbar': 'ui_level', 'value': self.a_ui_level}`
+
+        Returns
+        -------
+        None
+
+        """
+        if ui_level == -1:
+            self.a_ui_level = (self.a_ui_level + 1) % self.a_ui_num_levels
+        else:
+            self.a_ui_level = ui_level
+
+        if self.a_ui_level == 0:
+            self.a_ui.setIcon(QIcon(':/ui_level_max'))
+        elif self.a_ui_level == self.a_ui_num_levels - 1:
+            self.a_ui.setIcon(QIcon(':/ui_level_min'))
+        else:
+            self.a_ui.setIcon(QIcon(':/ui_level_mid'))
+
+        if ui_level == -1:
+            self.emit({'mpl_toolbar': 'ui_level', 'value': self.a_ui_level})
 
 # ------------------------------------------------------------------------------
     def toggle_lock_zoom(self):
         """
         Toggle the lock zoom settings and save the plot limits in any case:
             when previously unlocked, settings need to be saved
             when previously locked, current settings can be saved without effect
@@ -609,108 +712,137 @@
         else:
             self.a_lk.setIcon(QIcon(':/lock-unlocked.svg'))
             self.a_zo.setEnabled(True)
             self.a_pa.setEnabled(True)
             self.a_fv.setEnabled(True)
             self.a_ho.setEnabled(True)
 
-        self.emit({'lock_zoom': self.zoom_locked})
+        self.emit({'mpl_toolbar': 'lock_zoom', 'value': self.zoom_locked})  # unused?
 
 # ------------------------------------------------------------------------------
     def enable_plot(self, state=None):
         """
-        Toggle the enable button and setting
+        Toggle the plot enable button, enable / disable other plot buttons accordingly
+        and emit
         """
         if state is not None:
-            self.enabled = state
+            self.plot_enabled = state
         else:
-            self.enabled = not self.enabled
+            self.plot_enabled = not self.plot_enabled
 
-        if self.enabled:
+        if self.plot_enabled:
             self.a_en.setIcon(QIcon(':/circle-check.svg'))
+            # These UI elements can be enabled / disabled elsewhere,
+            # restore their previous state
+            self.a_ho.setEnabled(self.a_ho_prev_state)  # home
+            self.a_pa.setEnabled(self.a_pa_prev_state)  # pan
+            self.a_zo.setEnabled(self.a_zo_prev_state)  # zoom
+            self.a_fv.setEnabled(self.a_fv_prev_state)  # full view
+            self.a_lk.setEnabled(self.a_ho_prev_state)  # lock zoom
         else:
             self.a_en.setIcon(QIcon(':/circle-x.svg'))
+            # Some UI elements can be enabled / disabled elsewhere,
+            # save their state before disabling them
+            self.save_button_states()
+
+            self.a_ho.setEnabled(False)  # home
+            self.a_pa.setEnabled(False)  # pan
+            self.a_zo.setEnabled(False)  # zoom
+            self.a_fv.setEnabled(False)  # full view
+            self.a_lk.setEnabled(False)  # lock zoom
+
+            # Clear the Matplotlib canvas
+            self.mpl_widget.fig.clf()
+            self.mpl_widget.redraw() # redraw the canvas to remove old plot
+
+        # These UI elements are always enabled (if not disabled here),
+        # no need to save their state
+        self.a_ba.setEnabled(self.plot_enabled)  # back
+        self.a_fw.setEnabled(self.plot_enabled)  # forward
+        self.a_gr.setEnabled(self.plot_enabled)  # grid
+        self.a_sv.setEnabled(self.plot_enabled)  # save
+        self.a_cr.setEnabled(self.plot_enabled)  # cursor
+        self.a_cb.setEnabled(self.plot_enabled)  # clipboard
+        self.a_op.setEnabled(self.plot_enabled)  # options
+
+        self.emit({'mpl_toolbar': 'enable_plot', 'value': self.plot_enabled})
 
-#         self.a_ho.setEnabled(self.enabled)
-#         self.a_ba.setEnabled(self.enabled)
-#         self.a_fw.setEnabled(self.enabled)
-#         self.a_pa.setEnabled(self.enabled)
-#         self.a_zo.setEnabled(self.enabled)
-#         self.a_fv.setEnabled(self.enabled)
-#         self.a_lk.setEnabled(self.enabled)
-#         self.a_gr.setEnabled(self.enabled)
-#         #self.a_rd.setEnabled(self.enabled)
-#         self.a_sv.setEnabled(self.enabled)
-#         self.a_cb.setEnabled(self.enabled)
-#         self.a_op.setEnabled(self.enabled)
-#
-#         self.emit({'enabled':self.enabled})
-#
 # =============================================================================
 # ------------------------------------------------------------------------------
     def _save_figure(self):
         """
-        Save current figure using matplotlib's `save_figure()`. When <ALT> key is
+        Save current figure using matplotlib's `save_figure()`. When <SHIFT> key is
         pressed, remove the title before saving.
         """
-        if QtWidgets.QApplication.keyboardModifiers() == QtCore.Qt.AltModifier:
+        if QtWidgets.QApplication.keyboardModifiers() & Qt.ShiftModifier\
+                == Qt.ShiftModifier:
             title = self.mpl_widget.fig.get_axes()[0].get_title()  # store title text
             self.mpl_widget.fig.get_axes()[0].set_title("")  # and remove it from plot
             self.canvas.draw()  # redraw plot without title
             self.save_figure()
             self.mpl_widget.fig.get_axes()[0].set_title(title)  # restore title
             self.canvas.draw()  # and redraw once more
         else:
             self.save_figure()
 
 # ------------------------------------------------------------------------------
-    def mpl2Clip(self):
+    def mpl2Clip(self, key_event = False):
         """
         Copy current figure to the clipboard, either directly as PNG file or as
-        base64 encoded PNG file.
+        base64 encoded PNG file, with or without title.
 
         Qt.ShiftModifier = 0x02000000 # Shift key pressed
         Qt.ControlModifier = 0x04000000 # Control key
-        Qt.AltModifier   = 0x08000000 # Alt key
+        Qt.AltModifier   = 0x08000000 # Alt key, doesn't work under Linux?
         Qt.MetaModifier  = 0x10000000 # Meta key
+
+        When `key_event == True`, the trigger was a CTRL+C keypress and the Control
+        modifier has to be blanked out.
+
+        ALT-key doesn't work as a mouse modifier because it shifts the focus from the
+              toolbar to the menubar (? not implemented here)
         """
         try:
             modifiers = QtWidgets.QApplication.keyboardModifiers()
-            title_info = ""
-            if modifiers & QtCore.Qt.AltModifier == QtCore.Qt.AltModifier:
-                # logger.warning(f"suptitle {self.mpl_widget.fig._suptitle.get_text()}")
-                modifiers = modifiers & ~QtCore.Qt.AltModifier  # blank out AltMod. bit
-                title_info = "(no title) "
-                title = self.mpl_widget.fig.get_axes()[0].get_title()  # store title text
+            if key_event: # blank out ControlModifier
+                modifiers = modifiers &~ Qt.ControlModifier
+            else: # blank out ALT / META modifier
+                modifiers = modifiers & ~Qt.AltModifier & ~Qt.MetaModifier
+
+            title = self.mpl_widget.fig.get_axes()[0].get_title()  # store title text
+            title_info = f'"{title}"'
+            # SHIFT modifier detected -> remove title
+            if modifiers & Qt.ShiftModifier == Qt.ShiftModifier:
+                title_info = "without title"
                 self.mpl_widget.fig.get_axes()[0].set_title("")  # and remove it from plot
                 self.canvas.draw()  # redraw plot without title
                 img = QImage(self.canvas.grab())  # and grab it
                 self.mpl_widget.fig.get_axes()[0].set_title(title)  # restore title
                 self.canvas.draw()  # and redraw once more
             else:
                 img = QImage(self.canvas.grab())  # grab original screen
 
-            if modifiers in {QtCore.Qt.ShiftModifier, QtCore.Qt.ControlModifier}:
+            if modifiers & Qt.AltModifier == Qt.AltModifier\
+                    or modifiers & Qt.MetaModifier == Qt.MetaModifier\
+                    or modifiers & Qt.ControlModifier == Qt.ControlModifier:
                 ba = QtCore.QByteArray()
                 buffer = QtCore.QBuffer(ba)  # create buffer of ByteArray
                 buffer.open(QtCore.QIODevice.WriteOnly)  # ... open it
                 img.save(buffer, 'PNG')  # ... save image data to buffer
                 # ... convert to base64 bytes -> str -> strip b' ... '
                 base64_str = str(ba.toBase64().data()).lstrip("b'").rstrip("'")
                 # ... and copy as string to clipboard after removing b' ... '
-                if modifiers == QtCore.Qt.ShiftModifier:
-                    self.cb.setText(base64_str)
-                    logger.info(
-                        f'Copied plot {title_info}as base64 encoded PNG image '
-                        'to Clipboard.')
-                elif modifiers == QtCore.Qt.ControlModifier:
-                    self.cb.setText(
-                        '<img src="data:image/png;base64,' + base64_str + '"/>')
-                    logger.info(f'Copied plot {title_info}as base64 encoded PNG image '
-                                'with <img> tag to Clipboard.')
-                # elif modifiers == (QtCore.Qt.ControlModifier | QtCore.Qt.ShiftModifier):
-                #     logger.warning('Control+Shift+Click')
+
+                self.cb.setText(base64_str)
+                logger.info(
+                    f'Copied plot {title_info} as base64 encoded PNG image '
+                    'to Clipboard.')
+                # elif modifiers == Qt.ControlModifier:
+                #     self.cb.setText(
+                #         '<img src="data:image/png;base64,' + base64_str + '"/>')
+                #     logger.info(f'Copied plot {title_info}as base64 encoded PNG image '
+                #                 'with <img> tag to Clipboard.')
             else:
                 self.cb.setImage(img)
-                logger.info(f'Copied plot {title_info}as PNG image to Clipboard.')
+                logger.info(f'Copied plot {title_info} as PNG image to Clipboard.')
         except:
             logger.error('Error copying figure to clipboard:\n{0}'.format(sys.exc_info()))
```

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/plot_3d.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/plot_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,21 @@
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming from the navigation toolbar and from ``sig_rx``
         """
         # logger.debug("Processing {0} | data_changed = {1}, visible = {2}"\
         #              .format(dict_sig, self.data_changed, self.isVisible()))
         if self.isVisible():
-            if 'data_changed' in dict_sig or 'home' in dict_sig or self.data_changed:
+            if 'data_changed' in dict_sig or self.data_changed\
+                    or ('mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'home'):
                 self.draw()
                 self.data_changed = False
+            elif 'mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'ui_level':
+                self.frmControls.setVisible(dict_sig['value'] == 0)
+
         else:
             if 'data_changed' in dict_sig:
                 self.data_changed = True
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
         self.but_log = PushButton("dB", checked=False)
@@ -213,14 +217,15 @@
         # ----------------------------------------------------------------------
         # This is the plot pane widget, encompassing the other widgets
         self.mplwidget = MplWidget(self)
         self.mplwidget.layVMainMpl.addWidget(self.frmControls)
         self.mplwidget.layVMainMpl.setContentsMargins(*params['mpl_margins'])
         self.mplwidget.mplToolbar.a_he.setEnabled(True)
         self.mplwidget.mplToolbar.a_he.info = "manual/plot_3d.html"
+        self.mplwidget.mplToolbar.a_ui_num_levels = 2
         self.setLayout(self.mplwidget.layVMainMpl)
 
         self._init_grid()  # initialize grid and do initial plot
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
```

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/plot_fft_win.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/plot_fft_win.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,17 @@
     - `self.draw()`: calculate window and FFT and draw both
     - `get_win(N)` : Get the window array
     """
     sig_rx = pyqtSignal(object)  # incoming
     sig_tx = pyqtSignal(object)  # outgoing
     from pyfda.libs.pyfda_qt_lib import emit
 
-    def __init__(self, parent, win_dict, sym=False,
+    def __init__(self, win_dict, sym=False,
                  title='pyFDA Window Viewer', ignore_close_event=True):
-        super(Plot_FFT_win, self).__init__(parent)
+        super().__init__()
         # make window stay on top
         qwindow_stay_on_top(self, True)
 
         self.win_dict = win_dict
         self.sym = sym
         self.ignore_close_event = ignore_close_event
         self.setWindowTitle(title)
@@ -140,15 +140,15 @@
 
         elif 'view_changed' in dict_sig and 'fft_win' in dict_sig['view_changed']\
                 or self.needs_calc:
 
             self.calc_win_draw()
             self.needs_calc = False
 
-        elif 'home' in dict_sig:
+        elif  'mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'home':
             self.update_view()
 
         else:
             logger.error("Unknown content of dict_sig: {0}".format(dict_sig))
 
 # ------------------------------------------------------------------------------
     def _construct_UI(self):
@@ -156,15 +156,15 @@
         Intitialize the widget, consisting of:
         - Matplotlib widget with NavigationToolbar
         - Frame with control elements
         """
         self.bfont = QFont()
         self.bfont.setBold(True)
 
-        self.qfft_win_select = QFFTWinSelector(self, self.win_dict)
+        self.qfft_win_select = QFFTWinSelector(self.win_dict)
 
         self.lbl_N = QLabel(to_html("N =", frmt='bi'))
         self.led_N = QLineEdit(self)
         self.led_N.setText(str(self.N_view))
         self.led_N.setMaximumWidth(qtext_width(N_x=8))
         self.led_N.setToolTip(
             "<span>Number of window data points to display.</span>")
@@ -664,23 +664,24 @@
     from pyfda.libs.compat import QApplication
     from pyfda.libs.pyfda_fft_windows_lib import get_windows_dict
     from pyfda import pyfda_rc as rc
 
     app = QApplication(sys.argv)
     app.setStyleSheet(rc.qss_rc)
     fb.clipboard = QApplication.clipboard()  # create clipboard instance
-    win_names_list = ["Boxcar", "Rectangular", "Barthann", "Bartlett", "Blackman",
-                      "Blackmanharris", "Bohman", "Cosine", "Dolph-Chebyshev",
-                      "Flattop", "General Gaussian", "Gauss", "Hamming", "Hann",
-                      "Kaiser", "Nuttall", "Parzen", "Slepian", "Triangular", "Tukey"]
+    # win_names_list = ["Boxcar", "Rectangular", "Barthann", "Bartlett", "Blackman",
+    #                   "Blackmanharris", "Bohman", "Cosine", "Dolph-Chebyshev", "DPSS",
+    #                   "Flattop", "General Gaussian", "Gauss", "Hamming", "Hann",
+    #                   "Kaiser", "Nuttall", "Parzen", "Triangular", "Tukey"]
+    win_names_list = []
 
     # initialize windows dict with the list above and an initial window
     win_dict = get_windows_dict(
         win_names_list=win_names_list,
         cur_win_name="Hann")
 
-    mainw = Plot_FFT_win(None, win_dict, ignore_close_event=False)
+    mainw = Plot_FFT_win(win_dict, ignore_close_event=False)
 
     app.setActiveWindow(mainw)
     mainw.show()
 
     sys.exit(app.exec_())
```

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/plot_hf.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/plot_hf.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 The ``Plot_Hf`` class constructs the widget to plot the magnitude
 frequency response \|H(f)\| of the filter either in linear or logarithmic
 scale. Optionally, the magnitude specifications and the phase
 can be overlayed.
 """
 from pyfda.libs.compat import (QCheckBox, QWidget, QComboBox, QLabel, QLineEdit,
-                               QFrame, QHBoxLayout, pyqtSlot, pyqtSignal)
+                               QFrame, QHBoxLayout, QGridLayout, pyqtSlot, pyqtSignal)
 import numpy as np
 from matplotlib.patches import Rectangle
 from matplotlib import rcParams
 import matplotlib.ticker as ticker
 from matplotlib.ticker import AutoMinorLocator
 
 import pyfda.filterbroker as fb
@@ -65,38 +65,55 @@
         Process signals coming from the navigation toolbar and from sig_rx
         """
         # logger.debug("SIG_RX - needs_calc = {0}, vis = {1}\n{2}"\
         #              .format(self.needs_calc, self.isVisible(), pprint_log(dict_sig)))
 
         if self.isVisible():
             if 'data_changed' in dict_sig or 'specs_changed' in dict_sig\
-                    or 'home' in dict_sig or self.needs_calc:
+                    or ('mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'home')\
+                         or self.needs_calc:
                 self.draw()
                 self.needs_calc = False
                 self.needs_draw = False
             if 'view_changed' in dict_sig or self.needs_draw:
                 self.update_view()
                 self.needs_draw = False
+            elif 'mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'ui_level':
+                self.frmControls.setVisible(dict_sig['value'] == 0)
+
         else:
             if 'data_changed' in dict_sig or 'specs_changed' in dict_sig:
                 self.needs_calc = True
             if 'view_changed' in dict_sig:
                 self.needs_draw = True
 
     def _construct_ui(self):
         """
         Define and construct the subwidgets
         """
-        modes = ['| H |', 're{H}', 'im{H}']
-        self.cmbShowH = QComboBox(self)
-        self.cmbShowH.addItems(modes)
-        self.cmbShowH.setObjectName("cmbUnitsH")
-        self.cmbShowH.setToolTip("Show magnitude, real / imag. part of H or H \n"
-                                 "without linear phase (acausal system).")
-        self.cmbShowH.setCurrentIndex(0)
+        self.lbl_show_H_abs = QLabel(to_html('| H | ', frmt='b'))
+        self.chk_show_H_abs = QCheckBox(self)
+        self.chk_show_H_abs.setChecked(True)
+        self.chk_show_H_abs.setToolTip("Show magnitude of H(F)")
+        self.lbl_show_H_re = QLabel(to_html('re{H}&nbsp;', frmt='b'))
+        self.chk_show_H_re = QCheckBox(self)
+        self.chk_show_H_re.setToolTip("Show real part of H(F)")
+        self.lbl_show_H_im = QLabel(to_html('im{H}', frmt='b'))
+        self.chk_show_H_im = QCheckBox(self)
+        self.chk_show_H_im.setToolTip("Show imaginary part of H(F)")
+
+        layG_show_H = QGridLayout()
+        layG_show_H.addWidget(self.lbl_show_H_abs, 0, 0)
+        layG_show_H.addWidget(self.chk_show_H_abs, 0, 1)
+        layG_show_H.addWidget(self.lbl_show_H_re, 1, 0)
+        layG_show_H.addWidget(self.chk_show_H_re, 1, 1)
+        layG_show_H.addWidget(self.lbl_show_H_im, 2, 0)
+        layG_show_H.addWidget(self.chk_show_H_im, 2, 1)
+        layG_show_H.setContentsMargins(0,0,10,0)
+        layG_show_H.setSpacing(0)
 
         self.lblIn = QLabel(to_html("Unit:", frmt="b"), self)
 
         self.cmb_units_a = QComboBox(self)
         qcmb_box_populate(self.cmb_units_a, self.cmb_units_a_items,
                           self.cmb_units_a_default)
         self.cmb_units_a.setObjectName("cmbUnitsA")
@@ -105,15 +122,14 @@
         self.led_log_bottom = QLineEdit(self)
         self.led_log_bottom.setText(str(self.log_bottom))
         self.led_log_bottom.setMaximumWidth(qtext_width(N_x=8))
         self.led_log_bottom.setToolTip(
             "<span>Minimum display value for dB. scale.</span>")
         self.lbl_log_unit = QLabel("dB", self)
 
-        self.cmbShowH.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         self.cmb_units_a.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
         self.but_zerophase = PushButton(" Zero phase ", checked=False)
         self.but_zerophase.setToolTip(
             "<span>Remove linear phase calculated from filter order.\n"
             "Attention: This makes no sense for a non-linear phase system!</span>")
 
@@ -139,15 +155,15 @@
 
         # ----------------------------------------------------------------------
         #               ### frmControls ###
         #
         # This widget encompasses all control subwidgets
         # ----------------------------------------------------------------------
         layHControls = QHBoxLayout()
-        layHControls.addWidget(self.cmbShowH)
+        layHControls.addLayout(layG_show_H)
         layHControls.addWidget(self.lblIn)
         layHControls.addWidget(self.cmb_units_a)
         layHControls.addStretch(1)
         layHControls.addWidget(self.lbl_log_bottom)
         layHControls.addWidget(self.led_log_bottom)
         layHControls.addWidget(self.lbl_log_unit)
         layHControls.addStretch(1)
@@ -172,14 +188,16 @@
         # main widget, encompassing the other widgets
         # ----------------------------------------------------------------------
         self.mplwidget = MplWidget(self)
         self.mplwidget.layVMainMpl.addWidget(self.frmControls)
         self.mplwidget.layVMainMpl.setContentsMargins(*params['mpl_margins'])
         self.mplwidget.mplToolbar.a_he.setEnabled(True)
         self.mplwidget.mplToolbar.a_he.info = "manual/plot_hf.html"
+        self.mplwidget.mplToolbar.a_ui.setEnabled(True)
+        self.mplwidget.mplToolbar.a_ui_num_levels = 2
         self.setLayout(self.mplwidget.layVMainMpl)
 
         self.init_axes()
 
         self.draw()  # calculate and draw |H(f)|
 
         # ----------------------------------------------------------------------
@@ -187,15 +205,17 @@
         # ----------------------------------------------------------------------
         self.sig_rx.connect(self.process_sig_rx)
         # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         self.cmb_units_a.currentIndexChanged.connect(self.draw)
         self.led_log_bottom.editingFinished.connect(self.update_view)
-        self.cmbShowH.currentIndexChanged.connect(self.draw)
+        self.chk_show_H_abs.clicked.connect(self.draw)
+        self.chk_show_H_re.clicked.connect(self.draw)
+        self.chk_show_H_im.clicked.connect(self.draw)
 
         self.but_zerophase.clicked.connect(self.draw)
         self.cmbInset.currentIndexChanged.connect(self.draw_inset)
 
         self.but_specs.clicked.connect(self.draw)
         self.but_phase.clicked.connect(self.draw)
         self.but_align.clicked.connect(self.draw)
@@ -482,18 +502,23 @@
                 extent = self.mplwidget.get_full_extent(self.ax_i, pad=0.0)
                 # Transform this back to figure coordinates - otherwise, it
                 #  won't behave correctly when the size of the plot is changed:
                 extent = extent.transformed(self.mplwidget.fig.transFigure.inverted())
                 rect = Rectangle((extent.xmin, extent.ymin), extent.width,
                         extent.height, facecolor=rcParams['figure.facecolor'], edgecolor='none',
                         transform=self.mplwidget.fig.transFigure, zorder=-1)
-                self.ax_i.patches.append(rect)
+                self.ax_i.add_patch(rect)
 
                 self.ax_i.set_xlim(fb.fil[0]['freqSpecsRange'])
-                self.ax_i.plot(self.F, self.H_plt)
+                if self.chk_show_H_abs.isChecked():
+                    self.ax_i.plot(self.F, self.H_plt_abs)
+                if self.chk_show_H_re.isChecked():
+                    self.ax_i.plot(self.F, self.H_plt_re)
+                if self.chk_show_H_im.isChecked():
+                    self.ax_i.plot(self.F, self.H_plt_im)
 
             if self.cmbInset.currentIndex() == 1: # edit / navigate inset
                 self.ax_i.set_navigate(True)
                 self.ax.set_navigate(False)
                 if self.but_specs.isChecked():
                     self.plot_spec_limits(self.ax_i)
             else: # edit / navigate main plot
@@ -539,15 +564,15 @@
                 scale = 180./np.pi
 
             # replace nan and inf by finite values, otherwise np.unwrap yields
             # an array full of nans
             phi = np.angle(np.nan_to_num(self.H_c))
         # -----------------------------------------------------------
             self.ax_p.plot(self.F, np.unwrap(phi)*scale,
-                           'g-.', label="Phase")
+                           'g-.', label=r"$\angle\,H(F)$")
         # -----------------------------------------------------------
             self.ax_p.set_ylabel(phi_str)
 
 #------------------------------------------------------------------------------
     def calc_hf(self):
         """
         (Re-)Calculate the complex frequency response H_cmplx(W) (complex)
@@ -638,60 +663,76 @@
             # only use the first half of H and F
             self.H_c = self.H_cmplx[0:params['N_FFT']//2]
             self.F = self.F[0:params['N_FFT']//2]
         else:  # fb.fil[0]['freqSpecsRangeType'] == 'whole'
             # use H and F as calculated
             self.H_c = self.H_cmplx
 
-        # now calculate mag / real / imaginary part of H_c:
-        if self.but_zerophase.isChecked():  # remove the linear phase
+        # remove linear phase if button is checked
+        if self.but_zerophase.isChecked():
             self.H_c = self.H_c * np.exp(1j * self.W[0:len(self.F)] * fb.fil[0]["N"]/2.)
 
-        if self.cmbShowH.currentIndex() == 0:  # show magnitude of H
-            H = abs(self.H_c)
-            H_str = r'$|H(\mathrm{e}^{\mathrm{j} \Omega})|$'
-        elif self.cmbShowH.currentIndex() == 1: # show real part of H
-            H = self.H_c.real
-            H_str = r'$\Re \{H(\mathrm{e}^{\mathrm{j} \Omega})\}$'
-        else:  # show imag. part of H
-            H = self.H_c.imag
-            H_str = r'$\Im \{H(\mathrm{e}^{\mathrm{j} \Omega})\}$'
+        H_str = r'$H(\mathrm{e}^{\mathrm{j} \Omega})$'
 
         # ================ Main Plotting Routine =========================
         # ===  clear the axes and (re)draw the plot (if selectable)
         if self.ax.get_navigate():
+            #-----------------------------------------------------------
+            self.ax.clear()
+            # Select abs / real / imaginary part and scale according to selected unit
+            if self.chk_show_H_abs.isChecked():
+                if self.unitA == 'dB':
+                    self.H_plt_abs = np.maximum(20*np.log10(np.abs(self.H_c)), self.log_bottom)
+                elif self.unitA == 'V':
+                    self.H_plt_abs = np.abs(self.H_c)
+                elif self.unitA == 'W':
+                    self.H_plt_abs =  np.abs(self.H_c) * np.abs(self.H_c)
+                self.ax.plot(self.F, self.H_plt_abs, label = '$|H(f)|$')
+            if self.chk_show_H_re.isChecked():
+                if self.unitA == 'dB':
+                    self.H_plt_re = np.maximum(20*np.log10(np.abs(self.H_c.real)), self.log_bottom)
+                elif self.unitA == 'V':
+                    self.H_plt_re = self.H_c.real
+                elif self.unitA == 'W':
+                    self.H_plt_re =  self.H_c.real * self.H_c.real
+                self.ax.plot(self.F, self.H_plt_re, label = r'$\Re\{H(F)\}$')
+            if self.chk_show_H_im.isChecked():
+                if self.unitA == 'dB':
+                    self.H_plt_im = np.maximum(20*np.log10(np.abs(self.H_c.imag)), self.log_bottom)
+                elif self.unitA == 'V':
+                    self.H_plt_im = self.H_c.imag
+                elif self.unitA == 'W':
+                    self.H_plt_im =  self.H_c.imag * self.H_c.imag
+                self.ax.plot(self.F, self.H_plt_im, label = r'$\Im\{H(F)\}$')
 
+            # calculate limits for selected curves depending on selected unit
             if self.unitA == 'dB':
                 self.log_bottom = safe_eval(
                     self.led_log_bottom.text(), self.log_bottom,
                     return_type='float', sign='neg')
                 self.led_log_bottom.setText(str(self.log_bottom))
-
-                self.H_plt = np.maximum(20*np.log10(abs(H)), self.log_bottom)
                 A_lim = [self.log_bottom, 2]
                 H_str += ' in dB ' + r'$\rightarrow$'
+
             elif self.unitA == 'V':  #  'lin'
-                self.H_plt = H
-                if self.cmbShowH.currentIndex() != 0:  # H can be less than zero
-                    A_min = max(self.lin_neg_bottom, np.nanmin(self.H_plt[np.isfinite(self.H_plt)]))
-                else:
-                    A_min = 0
+                A_min = 0
+                if self.chk_show_H_re.isChecked():  # H can be less than zero
+                    A_min = min(A_min, np.nanmin(self.H_plt_re[np.isfinite(self.H_c)]))
+                if self.chk_show_H_im.isChecked():  # H can be less than zero
+                    A_min = min(A_min, np.nanmin(self.H_plt_im[np.isfinite(self.H_c)]))
+
+                A_min = max(A_min, self.lin_neg_bottom)
                 A_lim = [A_min, (1.05 + A_max)]
                 H_str +=' in V ' + r'$\rightarrow $'
                 self.ax.axhline(linewidth=1, color='k') # horizontal line at 0
+
             else: # unit is W
                 A_lim = [0, (1.03 + A_max)**2.]
-                self.H_plt = H * H.conj()
                 H_str += ' in W ' + r'$\rightarrow $'
 
-            #logger.debug("lim: {0}, min: {1}, max: {2} - {3}".format(A_lim, A_min, A_max, self.H_plt[0]))
-
-            #-----------------------------------------------------------
-            self.ax.clear()
-            self.ax.plot(self.F, self.H_plt, label = 'H(f)')
             # TODO: self.draw_inset() # this gives an infinite recursion
             self.draw_phase(self.ax)
             #-----------------------------------------------------------
 
             #============= Set Limits and draw specs =========================
             if self.but_specs.isChecked():
                 self.plot_spec_limits(self.ax)
@@ -699,21 +740,41 @@
             #     self.ax_bounds = [self.ax.get_ybound()[0], self.ax.get_ybound()[1]]#, self.ax.get]
             self.ax.set_xlim(f_lim)
             self.ax.set_ylim(A_lim)
             # logger.warning("set limits")
 
             self.ax.set_xlabel(fb.fil[0]['plt_fLabel'])
             self.ax.set_ylabel(H_str)
+
+            title_str = ""
+            if self.chk_show_H_abs.isChecked():
+                title_str = "Magnitude "
+            elif self.chk_show_H_re.isChecked() or self.chk_show_H_im.isChecked():
+                title_str = "Amplitude "
             if self.but_phase.isChecked():
-                self.ax.set_title(r'Magnitude and Phase Frequency Response')
-            else:
-                self.ax.set_title(r'Magnitude Frequency Response')
+                if title_str != "":
+                    title_str += "and Phase "
+                else:
+                    title_str += "Phase "
+            if title_str != "":
+                self.ax.set_title(f'{title_str}Frequency Response')
+
             self.ax.xaxis.set_minor_locator(AutoMinorLocator()) # enable minor ticks
             self.ax.yaxis.set_minor_locator(AutoMinorLocator()) # enable minor ticks
 
+            if hasattr(self, "ax_p"):  # if phase is visible, add label to legend
+                lines, labels = self.ax.get_legend_handles_labels()
+                lines2, labels2 = self.ax_p.get_legend_handles_labels()
+                self.ax.legend(lines + lines2, labels + labels2, loc='best',
+                               fontsize='small', fancybox=True, framealpha=0.7)
+            # only show legend if at least one label is visible
+            elif self.ax.get_legend_handles_labels()[1]:
+                self.ax.legend(loc='best', fontsize='small', fancybox=True,
+                               framealpha=0.7)
+
             np.seterr(**old_settings_seterr)
 
         self.redraw()
 
 #------------------------------------------------------------------------------
     def redraw(self):
         """
```

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/plot_impz.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/plot_impz.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,16 +50,19 @@
     sig_rx = pyqtSignal(object)  # incoming
     sig_tx = pyqtSignal(object)  # outgoing, e.g. when stimulus has been calculated
     from pyfda.libs.pyfda_qt_lib import emit
 
     def __init__(self):
         super().__init__()
 
-        self.ACTIVE_3D = False
-        self.ui = PlotImpz_UI()  # create the UI part with buttons etc.
+        # arrays that need to be passed to subwidgets
+        self.x = self.y = self.x_q = None
+
+        # create the UI part with buttons etc.
+        self.ui = PlotImpz_UI()
 
         # initial settings
         # ==================
         # flag whether specs have been changed and plots need to be recalculated
         self.needs_calc = True
         # same when fixpoint specs have been changed, only needed in Fixpoint mode
         self.needs_calc_fx = True
@@ -73,14 +76,16 @@
         # markersize=None, markeredgewidth=None, markeredgecolor=None,
         # markerfacecolor=None, markerfacecoloralt='none', fillstyle=None,
         self.fmt_mkr_size = 8
         self.fmt_plot_resp = {'color': 'red', 'linewidth': 2, 'alpha': 0.5}
         self.fmt_mkr_resp = {'marker': 'o', 'color': 'red', 'alpha': 0.5,
                              'ms': self.fmt_mkr_size}
         self.fmt_plot_stim = {'color': 'blue', 'linewidth': 2, 'alpha': 0.5}
+        self.fmt_plot_stim_interp = {'color': 'black', 'linewidth': 1, 'alpha': 0.5}
+
         self.fmt_mkr_stim = {'marker': 's', 'color': 'blue', 'alpha': 0.5,
                              'ms': self.fmt_mkr_size}
         self.fmt_plot_stmq = {'color': 'darkgreen', 'linewidth': 2, 'alpha': 0.5}
         self.fmt_mkr_stmq = {'marker': 'D', 'color': 'darkgreen', 'alpha': 0.5,
                              'ms': self.fmt_mkr_size}
 
         self._construct_UI()
@@ -103,25 +108,29 @@
         # Tabbed layout with vertical tabs ("west") for time and frequency domain
         # ----------------------------------------------------------------------
         # ---------- MplWidget for TIME domain plots ---------------------------
         self.mplwidget_t = MplWidget(self)
         self.mplwidget_t.setObjectName("mplwidget_t1")
         self.mplwidget_t.layVMainMpl.addWidget(self.ui.wdg_ctrl_time)
         self.mplwidget_t.layVMainMpl.setContentsMargins(*params['mpl_margins'])
+        self.mplwidget_t.mplToolbar.a_en.setVisible(True)
         self.mplwidget_t.mplToolbar.a_he.setEnabled(True)
         self.mplwidget_t.mplToolbar.a_he.info = "manual/plot_impz.html"
+        self.mplwidget_t.mplToolbar.a_ui_num_levels = 4
         self.mplwidget_t.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
         # ---------- MplWidget for FREQUENCY domain plots ----------------------
         self.mplwidget_f = MplWidget(self)
         self.mplwidget_f.setObjectName("mplwidget_f1")
         self.mplwidget_f.layVMainMpl.addWidget(self.ui.wdg_ctrl_freq)
         self.mplwidget_f.layVMainMpl.setContentsMargins(*params['mpl_margins'])
+        self.mplwidget_f.mplToolbar.a_en.setVisible(True)
         self.mplwidget_f.mplToolbar.a_he.setEnabled(True)
         self.mplwidget_f.mplToolbar.a_he.info = "manual/plot_impz.html"
+        self.mplwidget_f.mplToolbar.a_ui_num_levels = 4
         self.mplwidget_f.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
         # ----------- Construct TabWidget with time and frequency plot widgets
         self.tab_mpl_w = QTabWidget(self)
         self.tab_mpl_w.setTabPosition(QTabWidget.West)
         self.tab_mpl_w.setObjectName("tab_mpl_w")
         self.tab_mpl_w.addTab(self.mplwidget_t, "Time")
@@ -132,29 +141,42 @@
         # list with mplwidgets
         self.tab_mplwidget_list = ["mplwidget_t", "mplwidget_f"]
 
         # ----------------------------------------------------------------------
         # Tabbed layout with vertical tabs ("west") for stimulus and audio
         # ----------------------------------------------------------------------
         self.stim_wdg = Plot_Tran_Stim()
-        self.file_io_wdg = Tran_IO()
+        # set "Stim:" label width to same width as "Plots:" label:
+        self.stim_wdg.ui.lbl_title_stim.setFixedWidth(
+            self.ui.lbl_title_plot_time.sizeHint().width())
+        self.file_io_wdg = Tran_IO(self)
+        # set "File:" label width to same width as "Plots:" label:
+        self.file_io_wdg.ui.lbl_title_io_file.setFixedWidth(
+            self.ui.lbl_title_plot_time.sizeHint().width())
+
+        # This places the combo box for adding / using file data to the
+        # run control toolbar:
+        self.ui.frm_file_io.setLayout(self.stim_wdg.ui.layH_file_io)
+        # self.color = self.ui.frm_file_io.palette().color(QPalette.Background)
+        # logger.warning(f"color = {self.color.red()}, {self.color.green()}, {self.color.blue()}")
+        # self.stim_wdg.ui.cmb_file_io.setStyleSheet("border: 2px solid red;")
 
         self.tab_stim_w = QTabWidget(self)
         self.tab_stim_w.setObjectName("tab_stim_w")
         self.tab_stim_w.setTabPosition(QTabWidget.West)
-        self.tab_stim_w.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Preferred)
+        self.tab_stim_w.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         tab_w = 30  # needs to fit with the tab size defined in pyfda_rc.py
         # tab_w = self.tab_mpl_w.tabBar().tabSizeHint(0).width()  # crashes under Linux
         self.tab_stim_w.setIconSize(QSize(tab_w, tab_w))
-        self.tab_stim_w.addTab(self.stim_wdg, QIcon(":/graph_90.png"), "")
+        self.tab_stim_w.addTab(self.stim_wdg, QIcon(":/graph_90.svg"), "")
         self.tab_stim_w.setTabToolTip(0, "Stimuli")
 
         self.tab_stim_w.addTab(self.file_io_wdg, QIcon(":/file.svg"), "")
-        self.tab_stim_w.setTabToolTip(1, "I/O")
+        self.tab_stim_w.setTabToolTip(1, "File I/O")
 
         self.resize_stim_tab_widget()
         # ----------------------------------------------------------------------
         # ---------------- GLOBAL LAYOUT ---------------------------------------
         # ----------------------------------------------------------------------
         layVMain = QVBoxLayout()
         layVMain.addWidget(self.tab_mpl_w)
@@ -164,40 +186,42 @@
 
         self.setLayout(layVMain)
         self.updateGeometry()
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
+        # connect rx global events to process_sig_rx() and to listening subwidgets
         self.sig_rx.connect(self.process_sig_rx)
-        # connect UI to widgets and signals upstream:
+        self.sig_rx.connect(self.stim_wdg.sig_rx)
+        self.sig_rx.connect(self.file_io_wdg.sig_rx)
+        # connect UI and subwidgets tx events to process_sig_rx()
         self.ui.sig_tx.connect(self.process_sig_rx)
-
         self.stim_wdg.sig_tx.connect(self.process_sig_rx)
-        self.sig_rx.connect(self.stim_wdg.sig_rx)
         self.file_io_wdg.sig_tx.connect(self.process_sig_rx)
         self.mplwidget_t.mplToolbar.sig_tx.connect(self.process_sig_rx)
         self.mplwidget_f.mplToolbar.sig_tx.connect(self.process_sig_rx)
         # self.mplwidget.mplToolbar.enable_plot(state = False) # disable initially
+
         # When user has selected a different local tab, trigger a redraw of current tab
         self.tab_mpl_w.currentChanged.connect(self.draw)  # passes # of active tab
-
         # ---------------------------------------------------------------------
         # UI SIGNALS & SLOTs
         # ---------------------------------------------------------------------
         self.tab_stim_w.currentChanged.connect(self.resize_stim_tab_widget)
         # --- run control ---
         self.ui.cmb_sim_select.currentIndexChanged.connect(self.toggle_fx_setting)
         self.ui.but_run.clicked.connect(self.impz_init)
         self.ui.but_auto_run.clicked.connect(self.calc_auto)
         self.ui.but_fx_scale.clicked.connect(self.draw)
-        self.ui.but_toggle_stim_options.clicked.connect(self.toggle_stim_options)
+        self.stim_wdg.ui.but_file_io.clicked.connect(self.set_N_to_file_len)
         # --- time domain plotting --------------------------------------------
         self.ui.cmb_plt_time_resp.currentIndexChanged.connect(self.draw)
         self.ui.cmb_plt_time_stim.currentIndexChanged.connect(self.draw)
+        self.ui.chk_plt_time_stim_interp.clicked.connect(self.draw)
         self.ui.cmb_plt_time_stmq.currentIndexChanged.connect(self.draw)
         self.ui.cmb_plt_time_spgr.currentIndexChanged.connect(self._spgr_cmb)
         self.ui.but_log_time.clicked.connect(self.draw)
         self.ui.led_log_bottom_time.editingFinished.connect(self.draw)
         self.ui.but_log_spgr_time.clicked.connect(self.draw)
         self.ui.led_time_nfft_spgr.editingFinished.connect(self._spgr_ui2params)
         self.ui.led_time_ovlp_spgr.editingFinished.connect(self._spgr_ui2params)
@@ -211,22 +235,53 @@
         self.ui.cmb_plt_freq_stmq.currentIndexChanged.connect(self.draw)
         self.ui.but_Hf.clicked.connect(self.draw)
         self.ui.cmb_freq_display.currentIndexChanged.connect(self.draw)
         self.ui.but_log_freq.clicked.connect(self.draw)
         self.ui.led_log_bottom_freq.editingFinished.connect(self.draw)
         self.ui.but_freq_norm_impz.clicked.connect(self.draw)
         self.ui.but_freq_show_info.clicked.connect(self.draw)
+        # --- subwidgets
 
 # ------------------------------------------------------------------------------
     def toggle_stim_options(self):
         """
         Toggle visibility of stimulus options, depending on the state of the
         "Stimuli" button
         """
-        self.tab_stim_w.setVisible(self.ui.but_toggle_stim_options.isChecked())
+        self.tab_stim_w.setVisible(qget_cmb_box(self.ui.cmb_ui_select) in {"stim", "plot_stim"})
+        self.ui.wdg_ctrl_freq.setVisible(qget_cmb_box(self.ui.cmb_ui_select) in {"plot", "plot_stim"})
+        self.ui.wdg_ctrl_time.setVisible(qget_cmb_box(self.ui.cmb_ui_select) in {"plot", "plot_stim"})
+
+# ------------------------------------------------------------------------------
+    def set_ui_level(self, ui_level):
+        """
+        Sync time and frequency subwidget and set their ui display level
+        """
+        self.mplwidget_f.mplToolbar.cycle_ui_level(ui_level)
+        self.mplwidget_t.mplToolbar.cycle_ui_level(ui_level)
+        if ui_level == 0:
+            self.ui.wdg_ctrl_time.setVisible(True)
+            self.ui.wdg_ctrl_freq.setVisible(True)
+            self.tab_stim_w.setVisible(True)
+            self.ui.wdg_ctrl_run.setVisible(True)
+        elif ui_level == 1:
+            self.ui.wdg_ctrl_time.setVisible(False)
+            self.ui.wdg_ctrl_freq.setVisible(False)
+            self.tab_stim_w.setVisible(True)
+            self.ui.wdg_ctrl_run.setVisible(True)
+        elif ui_level == 2:
+            self.ui.wdg_ctrl_time.setVisible(False)
+            self.ui.wdg_ctrl_freq.setVisible(False)
+            self.tab_stim_w.setVisible(False)
+            self.ui.wdg_ctrl_run.setVisible(True)
+        elif ui_level == 3:
+            self.ui.wdg_ctrl_time.setVisible(False)
+            self.ui.wdg_ctrl_freq.setVisible(False)
+            self.tab_stim_w.setVisible(False)
+            self.ui.wdg_ctrl_run.setVisible(False)
 
 # ------------------------------------------------------------------------------
     def resize_stim_tab_widget(self):
         """
         Resize active tab of stimulus Tab widget to fit the height of the contained
         widget. This is triggered by:
         - initialization in `_construct_UI()`
@@ -234,35 +289,36 @@
         - an 'ui-changed' - signal (`process_signal_rx()`)
         """
         # logger.warning(f"w = {self.tab_stim_w.tabBar().width()}, "
         #                f"h = {self.tab_stim_w.tabBar().height()}")
         # logger.warning(f"w = {self.tab_mpl_w.tabBar().width()}, "
         #                f"h = {self.tab_mpl_w.tabBar().height()}")
         # tabBar height is also the width / hight of the tab icons
+
         h_min = self.tab_stim_w.tabBar().height()
         # logger.warning(f"min hint = {self.stim_wdg.minimumSizeHint()}, h_min = {h_min}")
         if self.tab_stim_w.currentWidget() is None:
             logger.warning("no embedded widget!")
             h = 0
         else:
             h = self.tab_stim_w.currentWidget().minimumSizeHint().height()
         self.tab_stim_w.setMaximumHeight(max(h, h_min))
         self.tab_stim_w.setMinimumHeight(max(h, h_min))
 
-# ------------------------------------------------------------------------------
+    # ------------------------------------------------------------------------------
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming from
         - the navigation toolbars (time and freq.)
         - local widgets (impz_ui) and
         - plot_tab_widgets() (global signals)
         """
-        logger.debug("SIG_RX - needs_calc: {0} | vis: {1}\n{2}\n\tfx_sim = {3}: cmb = {4}"
-                    .format(self.needs_calc, self.isVisible(), pprint_log(dict_sig),
-                            fb.fil[0]['fx_sim'], qget_cmb_box(self.ui.cmb_sim_select)))
+        # logger.warning(
+        #     f"SIG_RX - needs_calc: {self.needs_calc} | vis: {self.isVisible()}\n"
+        #     f"{pprint_log(dict_sig)}\n")
         # logger.debug(f'SIG_RX: "{first_item(dict_sig)}"')
 
         if dict_sig['id'] == id(self):
             # logger.debug(f'Stopped infinite loop: "{first_item(dict_sig)}"')
             return
 
         if 'fx_sim' in dict_sig:
@@ -338,94 +394,111 @@
             else:
                 logger.error('Unknown value "{0}" for "fx_sim" key\n'
                              '\treceived from "{1}"'.format(dict_sig['fx_sim'],
                                                             dict_sig['class']))
 
         # --- widget is visible, handle all signals except 'fx_sim' -----------
         elif self.isVisible():
-            if 'data_changed' in dict_sig or 'specs_changed' in dict_sig\
+            if 'data_changed' in dict_sig \
                     or self.needs_calc or (fb.fil[0]['fx_sim'] and self.needs_calc_fx):
-
-                N_end = 0
-                # new file has been loaded
+                # a file has been loaded or unloaded:
                 if 'data_changed' in dict_sig and dict_sig['data_changed'] == 'file_io':
                     # make file data available to stimulus widget and modify number of
                     # data points to be used:
-                    self.file_loaded()
+                    self.file_io()
 
                 # update number of data points in impz_ui and FFT window
                 # needed when e.g. FIR filter order has been changed, requiring
                 # a different number of data points for simulation. Don't emit a signal.
                 self.ui.update_N(emit=False)
                 self.needs_calc = True
                 # Highlight "RUN" button
                 self.ui.but_run.setIcon(QIcon(":/play.svg"))
                 qstyle_widget(self.ui.but_run, "changed")
                 self.impz_init()
 
+            elif 'mpl_toolbar' in dict_sig:
+                if dict_sig['mpl_toolbar'] == 'ui_level':
+                    self.set_ui_level(dict_sig['value'])
+                elif dict_sig['mpl_toolbar'] == 'home':
+                    self.zoom_home()
+                    self.needs_redraw[self.tab_mpl_w.currentIndex()] = False
+                elif dict_sig['mpl_toolbar'] == 'enable_plot'\
+                        and dict_sig['value']:  # enabled is True
+                    self.draw()
+
             elif 'ui_local_changed' in dict_sig:
-                # treat all local UI events here
-                self.resize_stim_tab_widget()
-                self.needs_calc = True
-                # make file data available to stimulus widget and modify number of
-                # data points to be used:
-                self.file_loaded()
-                self.impz_init()
+                if dict_sig['ui_local_changed'] == 'csv':
+                    # CSV options window has been closed, propagate the event
+                    self.emit({'ui_global_changed': 'csv'})
+                else:
+                    # treat all other local UI events here
+                    self.needs_calc = True
+                    # make file data available to stimulus widget:
+                    self.file_io()
+                    self.impz_init()
 
             elif 'view_changed' in dict_sig:
-                if dict_sig['view_changed'] == 'f_S':
-                    self.stim_wdg.ui.recalc_freqs()
-                self.draw()
-
-            elif 'home' in dict_sig:
-                self.redraw()
-                self.needs_redraw[self.tab_mpl_w.currentIndex()] = False
+                if 'f_S' in dict_sig['view_changed']:
+                    self.emit({'view_changed': 'f_S', 'id': id(self)})
+                self.draw()  # redraw a.o. changed axes scaling
 
         else:  # invisible
-            if 'data_changed' in dict_sig or 'specs_changed' in dict_sig:
+            if 'data_changed' in dict_sig:
                 self.needs_calc = True
-
             elif 'view_changed' in dict_sig:
                 # update frequency related widgets (visible or not)
                 if dict_sig['view_changed'] == 'f_S':
-                    self.stim_wdg.ui.recalc_freqs()
+                    self.emit({'view_changed': 'f_S', 'id': id(self)})
             elif 'ui_local_changed' in dict_sig:
                 self.needs_redraw = [True] * 2
 
-    def file_loaded(self):
+    # ------------------------------------------------------------------------------
+    def set_N_to_file_len(self):
         """
         Check status of file_io widget:
-        - if no file is loaded or `cmb_file_io == 'off'`, do nothing and return 0
-        - if `cmb_file_io == 'add'`, map the file data to `self.stim_wdg.x_file`
-          to make it accessible from the stimulus widget
-        - if `cmb_file_io == 'use'` do the same and set N_end = len(file_data) in th UI
-        """
-        # logger.info(
-        #     f"File loaded with {self.file_io_wdg.n_chan} channel(s) and "
-        #     f"{self.file_io_wdg.N} samples.")
+        - if no file is loaded, do nothing. This shouldn't happen (check to be sure ...)
+        - else set N_end = len(file_data) in the UI
+        """
         if not hasattr(self.file_io_wdg, 'N') or self.file_io_wdg.N == 0:
-            qset_cmb_box(self.stim_wdg.ui.cmb_file_io, "off", data=True)
-            self.stim_wdg.ui.cmb_file_io.setEnabled(False)
+            self.ui.frm_file_io.setEnabled(False)
+            logger.warning("No data loaded, you shouldn't see this message!")
+        # File is loaded, copy file length to N_end
         else:
-            self.stim_wdg.ui.cmb_file_io.setEnabled(True)
-            if qget_cmb_box(self.stim_wdg.ui.cmb_file_io) == "off":
-                return
+            self.ui.update_N(N_end = self.file_io_wdg.N)
 
-            # map data from file io widget to stimulus widget:
-            self.stim_wdg.x_file = self.file_io_wdg.x
-            if qget_cmb_box(self.stim_wdg.ui.cmb_file_io) == "use":
-                # override ui setting of N_end
-                self.ui.update_N(emit=False, N_end = self.file_io_wdg.N)
-            else:  # qget_cmb_box(self.stim_wdg.ui.cmb_file_io) == "add":
-                pass
-        return
-
-# =============================================================================
-# Simulation: Calculate stimulus, response and draw them
-# =============================================================================
+    # ------------------------------------------------------------------------------
+    def file_io(self):
+        """
+        Check status of file_io widget:
+        - if no file is loaded, do nothing and return 0, disable `cmb_file_io` and
+          the option to transfer the number of samples to N
+        - else map the file data to `self.stim_wdg.x_file` to make it accessible
+           from the stimulus widget. If `cmb_file_io == `use`, disable the widget to
+           modify stimuli
+        """
+        # No file has been loaded or number of data points is zero
+        #    -> disable file_io combobox:
+        if self.file_io_wdg.ui.but_load.property("state") != "ok" or\
+            not self.file_io_wdg.ui.but_load.isEnabled() or\
+                not hasattr(self.file_io_wdg, 'x') or self.file_io_wdg.x is None:
+            self.ui.frm_file_io.setEnabled(False)
+            self.stim_wdg.ui.wdg_stim.setEnabled(True)
+
+        # File is loaded, enable file_io combobox, disable stimulus and formula
+        # widget if file_io is set to "use" (in contrast to "add")
+        else:
+            self.ui.frm_file_io.setEnabled(True)
+            self.stim_wdg.x_file = self.file_io_wdg.x_file
+            self.stim_wdg.ui.wdg_stim.setEnabled(
+                qget_cmb_box(self.stim_wdg.ui.cmb_file_io) != "use")
+
+    # =========================================================================
+    # Simulation: Calculate stimulus, response and draw them
+    # =========================================================================
     def calc_auto(self, autorun=None):
         """
         Triggered when checkbox "Autorun" is clicked.
 
         When Autorun has been pushed (`but_auto_run.isChecked() == True`) and
         calculation is required, automatically run `impz_init()`.
         """
@@ -442,28 +515,29 @@
             - Activating "Autorun" via `self.calc_auto()`
             - Autorun (when something relevant in the UI has been updated)
             - 'fx_sim' : 'specs_changed'
 
         The following tasks are performed:
             - Enable energy scaling for impulse stimuli when requirements are met
             - check for and enable fixpoint settings
+            - resize stimulus widget
             - when triggered by `but_run` or when `Auto`== pressed and
               `self.needs_calc == True`, continue with calculating stimulus / response
             - When in fixpoint mode, initialize quantized stimulus `x_q` and input
               quantizer and emit {'fx_sim':'init'}
         """
-
         # allow scaling the frequency response from pure impulse (no DC, noise or file)
         # button is only visible for impulse-shaped stimuli
+        self.resize_stim_tab_widget()
         self.ui.but_freq_norm_impz.setEnabled(
             (self.stim_wdg.ui.noi == 0 or
-             self.stim_wdg.ui.cmbNoise.currentText() == 'None')
+             self.stim_wdg.ui.cmb_stim_noise.currentText() == 'None')
             and self.stim_wdg.ui.DC == 0
             and self.stim_wdg.ui.cmb_stim == "impulse"
-            and qget_cmb_box(self.stim_wdg.ui.cmb_file_io) == "off"
+            and self.file_io_wdg.ui.but_load.property("state") != "ok"
             )
         self.ui.but_freq_norm_impz.setVisible(self.stim_wdg.ui.cmb_stim == "impulse")
 
         self.error = False
         self.needs_redraw = [True] * 2
 
         # check for fixpoint setting (fb.fil[0]['fx_sim']) and update UI if needed
@@ -471,46 +545,67 @@
 
         if type(arg) == bool:
             self.needs_calc = True  # but_run has been pressed -> force run
         elif not self.ui.but_auto_run.isChecked():  # "Auto" is not active, return
             return
 
         if self.needs_calc:
-            # set title and axis string and calculate 10 samples to determine ndtype
-            x_test = self.stim_wdg.calc_stimulus_frame(init=True)
+            # Test whether stimulus or filter coefficients are complex and set flag
+            #  correspondingly, additionally calculate up to 10 samples to test for
+            # complex values:
+            self.N_first = 0  # initialize frame index
+            x_test = np.zeros(10, dtype=complex)
+            # TODO: For stimuli that become complex only after the 10th sample,
+            #       the test fails
+            # TODO: np.iscomplexobj() returns true for an array with dtype complex
+            #       although each item is real.
+            self.stim_wdg.calc_stimulus_frame(x_test, N_frame = min(10, self.ui.N_end))
+
+            # convert from np.bool to bool to avoid deprecation warning concerning
+            # 'np.bool_' scalars to be interpreted as an index.
+            self.cmplx = bool(\
+                (self.stim_wdg.ui.ledDC.isVisible and type(self.stim_wdg.ui.DC) == complex)\
+                    or (self.stim_wdg.ui.ledAmp1.isVisible and type(self.stim_wdg.ui.A1) == complex)\
+                or (self.stim_wdg.ui.ledAmp2.isVisible and type(self.stim_wdg.ui.A2) == complex)\
+                    or np.any(np.iscomplex(np.asarray(fb.fil[0]['ba'])))\
+                or self.file_io_wdg.ui.but_load.property("state") == 'ok'\
+                    and np.iscomplexobj(self.file_io_wdg.x)\
+                or np.any(np.iscomplex(x_test)))
+
+            self.ui.lbl_stim_cmplx_warn.setVisible(self.cmplx)
+
+            # set title and axis string
+            self.stim_wdg.init_labels_stim()
             self.title_str = self.stim_wdg.title_str
 
-            self.N_first = 0  # initialize frame index
             self.n = np.arange(self.ui.N_end, dtype=float)
-            self.x = np.empty(self.ui.N_end, dtype=x_test.dtype)  # stimulus
-            # Test whether stimulus or filter coefficients are complex and set
-            # flag and UI field correspondingly
-            self.cmplx = bool(
-                np.any(np.any(np.iscomplex(x_test))
-                       or np.any(np.iscomplex(np.asarray(fb.fil[0]['ba'])))))
+
+            # initialize arrays for stimulus and response
             if self.cmplx:
-                self.y = np.empty_like(self.x, dtype=complex)  # always complex
+                self.x = np.zeros(self.ui.N_end, dtype=complex)
+                self.y = np.zeros(self.ui.N_end, dtype=complex)
             else:
-                self.y = np.empty_like(self.x)  # same type as self.x
-            self.ui.lbl_stim_cmplx_warn.setVisible(self.cmplx)
+                self.x = np.zeros(self.ui.N_end, dtype=float)
+                self.y = np.zeros(self.ui.N_end, dtype=float)
 
             # initialize progress bar
             self.ui.prg_wdg.setMaximum(self.ui.N_end)
             self.ui.prg_wdg.setValue(0)
             self.ui.but_run.setIcon(QIcon(":/stop.svg"))
             qstyle_widget(self.ui.but_run, "running")
 
             self.t_start = time.process_time()  # store starting time
 
             if fb.fil[0]['fx_sim']:
                 # - update plot title string
                 # - setup input quantizer self.q_i
                 # - emit {'fx_sim': 'init'} to listening widgets (input_fixpoint_specs)
                 self.title_str = r'$Fixpoint$ ' + self.title_str
-                self.x_q = np.empty_like(self.x, dtype=np.float64)  # quantized stimulus
+                 # initialize array for quantized stimulus
+                self.x_q = np.empty_like(self.x, dtype=np.float64)
                 if np.any(np.iscomplex(x_test)):
                     logger.warning(
                         "Complex stimulus: Only its real part is used for the "
                         "fixpoint filter!")
                 # setup and initialize input quantizer
                 self.q_i = fx.Fixed(fb.fil[0]['fxqc']['QI'])
                 # always use integer decimal format for input quantizer
@@ -554,30 +649,17 @@
             L_frame = min(self.ui.N_frame, self.ui.N_end - self.N_first)
             # Define slicing expression for the current frame
             frame = slice(self.N_first, self.N_first + L_frame)
 
             # ------------------------------------------------------------------
             # ---- calculate stimuli for current frame -------------------------
             # ------------------------------------------------------------------
-            # self.stim_wdg = Plot_Tran_Stim()
-            # self.file_io_wdg = Tran_IO()
-            # TODO: Use file data here, limit to one channel
-            x_io = self.file_io_wdg.x
-            if qget_cmb_box(self.stim_wdg.ui.cmb_file_io) == 'use':
-                self.ui.update_N(emit=False, N_end=len(x_io))
-                self.x[frame] = self.stim_wdg.calc_stimulus_frame(
-                    N_first=self.N_first, N_frame=L_frame, N_end=self.ui.N_end)
-            #
-            elif qget_cmb_box(self.stim_wdg.ui.cmb_file_io) == 'add':
-                self.x[frame] = self.stim_wdg.calc_stimulus_frame(
-                    N_first=self.N_first, N_frame=L_frame, N_end=self.ui.N_end)
-            #
-            else:
-                self.x[frame] = self.stim_wdg.calc_stimulus_frame(
-                    N_first=self.N_first, N_frame=L_frame, N_end=self.ui.N_end)
+            # self.x[frame] = self.stim_wdg.calc_stimulus_frame(
+            self.stim_wdg.calc_stimulus_frame(
+                self.x, N_first=self.N_first, N_frame=L_frame, N_end=self.ui.N_end)
 
             # ------------------------------------------------------------------
             # ---- calculate fixpoint or floating point response for current frame
             # ------------------------------------------------------------------
             if fb.fil[0]['fx_sim']:  # fixpoint filter
                 self.x_q[frame] = self.q_i.fixp(self.x[frame].real)  # quantize stimulus
                 # --------------------------------------------------------------
@@ -631,14 +713,15 @@
         has finished:
 
         - Calculate step error if selected
         - Check for complex stimulus or response
         - Calculate simulation time
         - Draw the signals
         - Reset Run Icon to normal state, reset `needs_calc` flag
+        - Update File IO save combo boxes
 
         """
         # step error calculation: calculate system DC response and subtract it
         # from the response
         if self.stim_wdg.ui.stim == "step" and self.stim_wdg.ui.chk_step_err.isChecked():
             if len(self.sos) > 0:  # has second order sections
                 dc = sig.sosfreqz(self.sos, [0])  # yields (w(0), H(0))
@@ -657,14 +740,16 @@
         # self.needs_redraw[self.tab_mpl_w.currentIndex()] = False
         self.needs_calc = False
         self.needs_calc_fx = False
         logger.info('[{0:5.4g} ms]: Plotted transient {1}response'
                     .format((time.process_time() - self.t_resp)*1000, self.fx_str))
         self.ui.but_run.setIcon(QIcon(":/play.svg"))
         qstyle_widget(self.ui.but_run, "normal")
+        # update Tran_IO ui, depending on complex and fixpoint status
+        self.file_io_wdg.ui.update_ui(cmplx=self.cmplx, fx=fb.fil[0]['fx_sim'])
 
         if fb.fil[0]['fx_sim']:
             self.emit({'fx_sim': 'finish'})
 
 # =============================================================================
     def toggle_fx_setting(self):
         """ Triggered by changing `self.ui.cmb_sim_select` """
@@ -820,17 +905,19 @@
                 logger.error(
                     "Type error: 'fxqc_dict'={0},\n{1}".format(fb.fil[0]['fxqc'], e))
             except ValueError as e:
                 logger.error("Value error: {0}".format(e))
 
         idx = self.tab_mpl_w.currentIndex()
 
-        if idx == 0 and self.needs_redraw[0]:
+        if idx == 0 and self.needs_redraw[0]\
+                and self.mplwidget_t.mplToolbar.plot_enabled:
             self.draw_time(N_start=self.ui.N_start, N_end=self.ui.N_end)
-        elif idx == 1 and self.needs_redraw[1]:
+        elif idx == 1 and self.needs_redraw[1]\
+                and self.mplwidget_f.mplToolbar.plot_enabled:
             self.draw_freq()
 
     # ------------------------------------------------------------------------
     def _spgr_ui2params(self):
         """
         Update overlap and nfft parameters for spectrogram from UI
         """
@@ -854,24 +941,16 @@
         self.draw()
 
 # ----------------------------------------------------------------------------
     def _spgr_cmb(self):
         """
         Update spectrogram UI when signal selection combobox has been changed
         """
-        spgr_en = qget_cmb_box(self.ui.cmb_plt_time_spgr) != 'none'
-
-        self.ui.but_log_spgr_time.setVisible(spgr_en)
-        self.ui.lbl_time_nfft_spgr.setVisible(spgr_en)
-        self.ui.led_time_nfft_spgr.setVisible(spgr_en)
-        self.ui.lbl_time_ovlp_spgr.setVisible(spgr_en)
-        self.ui.led_time_ovlp_spgr.setVisible(spgr_en)
-        self.ui.cmb_mode_spgr_time.setVisible(spgr_en)
-        self.ui.lbl_byfs_spgr_time.setVisible(spgr_en)
-        self.ui.chk_byfs_spgr_time.setVisible(spgr_en)
+        self.ui.wdg_ctrl_time_spgr.setVisible(
+            qget_cmb_box(self.ui.cmb_plt_time_spgr) != 'none')
 
         self.draw()
 
     # ------------------------------------------------------------------------
     def _log_mode_time(self):
         """
         Select / deselect log. mode for time domain and update self.ui.bottom_t
@@ -909,16 +988,17 @@
                                          self.ui.bottom_f, return_type='float',
                                          sign='neg')
             self.ui.led_log_bottom_freq.setText(str(self.ui.bottom_f))
         else:
             self.ui.bottom_f = 0
 
     # ------------------------------------------------------------------------
-    def draw_data(self, plt_style, ax, x, y, bottom=0, label='',
-                  plt_fmt={}, mkr_fmt={}, **args):
+    def draw_data(self, plt_style: str, ax: object, x: np.ndarray, y:np.ndarray,
+                  bottom: float = 0, label: str = '',
+                  plt_fmt: dict = {}, mkr_fmt: dict = {}, **args):
         """
         Plot x, y data (numpy arrays with equal length) in a plot style defined
         by `plt_style`.
 
         Parameters
         ----------
         plt_style : str
@@ -970,16 +1050,18 @@
         return handle
 
     # ================ Plotting routine time domain =========================
     def _init_axes_time(self):
         """
         Clear and initialize the axes of the time domain matplotlib widgets
         """
+        # calculate time vector from index n and T_S
         self.t = self.n * fb.fil[0]['T_S']
 
+        # Read out combo boxes with plotting styles and remove the '*' for markers
         self.plt_time_resp = qget_cmb_box(self.ui.cmb_plt_time_resp).replace("*", "")
         self.plt_time_stim = qget_cmb_box(self.ui.cmb_plt_time_stim).replace("*", "")
         self.plt_time_stmq = qget_cmb_box(self.ui.cmb_plt_time_stmq).replace("*", "")
         self.plt_time_spgr = qget_cmb_box(self.ui.cmb_plt_time_spgr)
         self.spgr = self.plt_time_spgr != "none"
 
         self.plt_time_enabled = self.plt_time_resp != "none"\
@@ -1001,32 +1083,34 @@
             self.ax_i = self.axes_time[1]
             self.ax_i.cla()
             self.mplwidget_t.fig.align_ylabels()
 
         if self.spgr:
             self.ax_s = self.axes_time[-1]  # assign last axis
 
-        if self.ACTIVE_3D:  # not implemented / tested yet
+        if False:  # not implemented / tested yet: complex data as 3D plot
             self.ax3d = self.mplwidget_t.fig.add_subplot(111, projection='3d')
 
         for ax in self.axes_time:
             ax.xaxis.tick_bottom()  # remove axis ticks on top
             ax.yaxis.tick_left()  # remove axis ticks right
             ax.xaxis.set_minor_locator(AutoMinorLocator())  # enable minor ticks
             ax.yaxis.set_minor_locator(AutoMinorLocator())
 
     # ------------------------------------------------------------------------
-    def draw_time(self, N_start, N_end):
+    def draw_time(self, N_start=0, N_end=0):
         """
         (Re-)draw the time domain mplwidget
         """
         if self.y is None:  # safety net for empty responses
             for ax in self.mplwidget_t.fig.get_axes():  # remove all axes
                 self.mplwidget_t.fig.delaxes(ax)
             return
+        if N_end == 0:
+            N_end = self.ui.N_end
 
         H_str = self.stim_wdg.H_str
 
         self._init_axes_time()
         self._log_mode_time()
 
         # '$h... = some impulse response, don't change
@@ -1061,14 +1145,24 @@
             if self.ui.but_log_time.isChecked():
                 x_q = np.maximum(20 * np.log10(abs(x_q)), self.ui.bottom_t)
 
             # logger.warning("self.scale I:{0} O:{1}".format(self.scale_i, self.scale_o))
         else:
             x_q = None
 
+        # Create finer grid for plotting interpolated waveforms
+        if self.ui.chk_plt_time_stim_interp.isChecked():
+            I = 20
+            # self.t_interp = np.linspace(self.t[0], self.t[-1], (len(self.t) - 1) * I + 1)
+            # self.x_interp = np.interp(self.t_interp, self.t, self.x, left=None, right=None,
+            #                      period=None)
+            self.x_interp = sig.resample_poly(self.x, I, 1, axis=0, window=('kaiser', 5.0),
+                                              padtype='line', cval=None)
+            self.t_interp = np.linspace(self.n[0], self.n[-1] + 1, len(self.n) * I, endpoint=False) * fb.fil[0]['T_S']
+
         t = self.t[N_start:N_end]
         x = self.x[N_start:N_end] * self.scale_i
         y = self.y[N_start:N_end] * self.scale_o
         win = self.ui.qfft_win_select.get_window(self.ui.N)
         if self.cmplx:
             x_r = x.real
             x_i = x.imag
@@ -1081,14 +1175,15 @@
         else:
             x_r = x.real
             x_i = None
             y_r = y
             y_i = None
             lbl_x_r = "$x[n]$"
             lbl_y_r = "$y[n]$"
+        lbl_x_r_interp = "$x(t)$"
 
         # log. scale for stimulus / response time domain:
         if self.ui.but_log_time.isChecked():
             bottom_t = self.ui.bottom_t
             win = np.maximum(20 * np.log10(
                 abs(self.ui.qfft_win_select.get_window(self.ui.N))), self.ui.bottom_t)
             x_r = np.maximum(20 * np.log10(abs(x_r)), self.ui.bottom_t)
@@ -1127,14 +1222,22 @@
         if self.plt_time_stim != "none":
             h_r.append(self.draw_data(
                 self.plt_time_stim, self.ax_r, t,
                 x_r, label=lbl_x_r, bottom=bottom_t,
                 plt_fmt=self.fmt_plot_stim, mkr_fmt=fmt_mkr_stim))
             l_r += [lbl_x_r]
 
+            if self.ui.chk_plt_time_stim_interp.isChecked():
+                # add interpolated waveform
+                h_r.append(self.draw_data(
+                    "line", self.ax_r, self.t_interp,
+                    self.x_interp, label=lbl_x_r_interp, bottom=bottom_t,
+                    plt_fmt=self.fmt_plot_stim_interp, mkr_fmt={'marker': ''}))
+                l_r += [lbl_x_r_interp]
+
         # -------------- Stimulus <q> plot ------------------------------------
         if x_q is not None and self.plt_time_stmq != "none":
             h_r.append(self.draw_data(
                 self.plt_time_stmq, self.ax_r, t,
                 x_q, label='$x_q[n]$', bottom=bottom_t,
                 plt_fmt=self.fmt_plot_stmq, mkr_fmt=fmt_mkr_stmq))
             l_r += ['$x_q[n]$']
@@ -1330,15 +1433,15 @@
                 cbar = self.mplwidget_t.fig.colorbar(col_mesh, ax=self.ax_s, aspect=30,
                                                      pad=0.005)
                 cbar.ax.set_ylabel(spgr_pre + spgr_symb + spgr_args + spgr_unit)
 
                 self.ax_s.set_ylabel(fb.fil[0]['plt_fLabel'])
 
         # --------------- 3D Complex  -----------------------------------------
-        if self.ACTIVE_3D:  # not implemented / tested yet
+        if False:  # not implemented / tested yet: complex data as 3D plot
             # plotting the stems
             for i in range(self.ui.N_start, self.ui.N_end):
                 self.ax3d.plot([self.t[i], self.t[i]], [y_r[i], y_r[i]], [0, y_i[i]],
                                '-', linewidth=2, alpha=.5)
 
             # plotting a circle on the top of each stem
             self.ax3d.plot(
@@ -1844,25 +1947,33 @@
         self.redraw()  # redraw currently active mplwidget
 
         self.needs_redraw[1] = False
 
     # -------------------------------------------------------------------------
     def redraw(self):
         """
-        Redraw the currently visible canvas when e.g. the canvas size has changed
+        Redraw the currently visible canvas (but not the plot!) when e.g. the canvas
+        size has changed
         """
         idx = self.tab_mpl_w.currentIndex()
         self.tab_mpl_w.currentWidget().redraw()
-        # wdg = getattr(self, self.tab_mplwidget_list[idx])
         logger.debug("Redrawing tab {0}".format(idx))
-        # wdg_cur.redraw()
         self.needs_redraw[idx] = False
 #        self.mplwidget_t.redraw()
-#        self.mplwidget_f.redraw()
 
+     # -------------------------------------------------------------------------
+    def zoom_home(self):
+        """
+        Zoom to home settings
+        """
+        idx = self.tab_mpl_w.currentIndex()
+        if idx == 0:  # time plot widget
+            self.draw_time()
+        else:
+            self.draw_freq()
 
 # ------------------------------------------------------------------------------
 
 if __name__ == "__main__":
     """ Run widget standalone with `python -m pyfda.plot_widgets.plot_impz` """
     import sys
     from pyfda.libs.compat import QApplication
```

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/plot_impz_ui.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/plot_impz_ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 # (see file LICENSE in root directory for details)
 
 """
 Create the UI for the PlotImz class
 """
 from pyfda.libs.compat import (
     QCheckBox, QWidget, QComboBox, QLineEdit, QLabel, QPushButton, QPushButtonRT,
-    QIcon, QProgressBar, pyqtSignal, QSize, QHBoxLayout, QVBoxLayout)
+    QIcon, QProgressBar, pyqtSignal, QSize, QFrame,
+    QHBoxLayout, QVBoxLayout, QGridLayout)
 
 from pyfda.libs.pyfda_lib import to_html, safe_eval, pprint_log
 import pyfda.filterbroker as fb
 from pyfda.libs.pyfda_qt_lib import (
-    qcmb_box_populate, qget_cmb_box, qset_cmb_box, qtext_width,
+    qcmb_box_populate, qget_cmb_box, qset_cmb_box, qtext_width, qstyle_widget,
     QVLine, PushButton)
 from pyfda.libs.pyfda_fft_windows_lib import get_windows_dict, QFFTWinSelector
-from pyfda.pyfda_rc import params  # FMT string for QLineEdit fields, e.g. '{:.3g}'
+# FMT string for QLineEdit fields, e.g. '{:.3g}'
+from pyfda.pyfda_rc import params
 
 from pyfda.plot_widgets.plot_fft_win import Plot_FFT_win
 
 import logging
 logger = logging.getLogger(__name__)
 
 
@@ -49,15 +51,16 @@
         - qfft_win_select
         """
 
         # logger.debug("PROCESS_SIG_RX - vis: {0}\n{1}"
         #              .format(self.isVisible(), pprint_log(dict_sig)))
 
         if 'id' in dict_sig and dict_sig['id'] == id(self):
-            logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
+            logger.warning("Stopped infinite loop:\n{0}".format(
+                pprint_log(dict_sig)))
             return
 
         # --- signals coming from the FFT window widget or the FFT window selector
         if dict_sig['class'] in {'Plot_FFT_win', 'QFFTWinSelector'}:
             if 'closeEvent' in dict_sig:   # hide FFT window widget and return
                 self.hide_fft_wdg()
                 return
@@ -84,14 +87,15 @@
         self.N_user = 0
         self.N = 0
         self.N_frame_user = 0
         self.N_frame = 0
 
         # run
         self.cmb_sim_select_init = "float"
+        self.cmb_ui_select_init = "plot_stim"
 
         # time
         self.plt_time_resp = "stem"
         self.plt_time_stim = "line"
         self.plt_time_stmq = "none"
         self.plt_time_spgr = "none"
 
@@ -109,27 +113,27 @@
         self.bottom_f = -120  # initial value for log. scale
         self.param = None
 
         self.f_scale = fb.fil[0]['f_S']
         self.t_scale = fb.fil[0]['T_S']
         # list of windows that are available for FFT analysis
         win_names_list = ["Boxcar", "Rectangular", "Barthann", "Bartlett", "Blackman",
-                          "Blackmanharris", "Bohman", "Cosine", "Dolph-Chebyshev",
+                          "Blackmanharris", "Bohman", "Cosine", "Dolph-Chebyshev", "DPSS",
                           "Flattop", "General Gaussian", "Gauss", "Hamming", "Hann",
-                          "Kaiser", "Nuttall", "Parzen", "Slepian", "Triangular", "Tukey"]
+                          "Kaiser", "Nuttall", "Parzen", "Triangular", "Tukey"]
         self.cur_win_name = "Rectangular"  # set initial window type
 
         # initialize windows dict with the list above
         self.win_dict = get_windows_dict(
             win_names_list=win_names_list,
             cur_win_name=self.cur_win_name)
 
         # instantiate FFT window with default windows dict
         self.fft_widget = Plot_FFT_win(
-            self, self.win_dict, sym=False, title="pyFDA Spectral Window Viewer")
+            self.win_dict, sym=False, title="pyFDA Spectral Window Viewer")
         # hide window initially, this is modeless i.e. a non-blocking popup window
         self.fft_widget.hide()
 
         # combobox fixpoint / floating point simulation
         self.cmb_sim_select_items = [
             "<span>Simulate floating-point or fixpoint response.</span>",
             ("float", "Float", "floating point simulation"),
@@ -143,41 +147,41 @@
             ("dots*", QIcon(":/plot_style-mkr"), "markers only"),
             ("line", QIcon(":/plot_style-line"), "line"),
             ("line*", QIcon(":/plot_style-line-mkr"), "line + markers"),
             ("stem", QIcon(":/plot_style-stem"), "stems"),
             ("stem*", QIcon(":/plot_style-stem-mkr"), "stems + markers"),
             ("steps", QIcon(":/plot_style-steps"), "steps"),
             ("steps*", QIcon(":/plot_style-steps-mkr"), "steps + markers")
-            ]
+        ]
 
         self.cmb_time_spgr_items = [
             "<span>Show Spectrogram for selected signal.</span>",
             ("none", "None", ""),
             ("xn", "x[n]", "input"),
             ("xqn", "x_q[n]", "quantized input"),
             ("yn", "y[n]", "output")
-            ]
+        ]
 
         self.cmb_mode_spgr_time_items = [
             "<span>Spectrogram display mode.</span>",
             ("psd", "PSD",
              "<span>Power Spectral Density, either per bin or referred to "
              "<i>f<sub>S</sub></i></span>"),
             ("magnitude", "Mag.", "Signal magnitude"),
             ("angle", "Angle", "Phase, wrapped to &pm; &pi;"),
             ("phase", "Phase", "Phase (unwrapped)")
-            ]
+        ]
 #        self.N
 
         self.cmb_freq_display_items = [
             "<span>Select how to display the spectrum.</span>",
             ("mag", "Magnitude", "<span>Spectral magnitude</span>"),
             ("mag_phi", "Mag. / Phase", "<span>Magnitude and phase.</span>"),
             ("re_im", "Re. / Imag.", "<span>Real and imaginary part of spectrum.</span>")
-            ]
+        ]
 
         self._construct_UI()
 #        self._enable_stim_widgets()
         self.update_N(emit=False)  # also updates window function and win_dict
 #        self._update_noi()
 
     def _construct_UI(self):
@@ -195,53 +199,57 @@
 
         but_height = self.but_auto_run.sizeHint().height()
 
         self.but_run = QPushButton(self)
         self.but_run.setIcon(QIcon(":/play.svg"))
 
         self.but_run.setIconSize(QSize(but_height, but_height))
-        self.but_run.setFixedSize(QSize(2*but_height, but_height))
+        self.but_run.setFixedSize(QSize(2 * but_height, but_height))
         self.but_run.setToolTip("Run simulation")
         self.but_run.setEnabled(True)
 
         self.cmb_sim_select = QComboBox(self)
         qcmb_box_populate(self.cmb_sim_select, self.cmb_sim_select_items,
                           self.cmb_sim_select_init)
 
+        self.prg_wdg = QProgressBar(self)
+        self.prg_wdg.setToolTip("Show simulation progress")
+        self.prg_wdg.setFixedHeight(but_height)
+        self.prg_wdg.setFixedWidth(qtext_width(N_x=6))
+        self.prg_wdg.setMinimum(0)
+        self.prg_wdg.setValue(0)
+
         self.lbl_N_points = QLabel(to_html("N", frmt='bi') + " =", self)
         self.led_N_points = QLineEdit(self)
         self.led_N_points.setText(str(self.N))
         self.led_N_points.setToolTip(
             "<span>Number of data points to plot. "
             "<i>N</i> = 0 tries to choose for you.</span>")
         self.led_N_points.setMaximumWidth(qtext_width(N_x=8))
         self.lbl_N_start = QLabel(to_html("N_0", frmt='bi') + " =", self)
         self.led_N_start = QLineEdit(self)
         self.led_N_start.setText(str(self.N_start))
         self.led_N_start.setToolTip("<span>First point to plot.</span>")
         self.led_N_start.setMaximumWidth(qtext_width(N_x=8))
 
-        self.lbl_N_frame = QLabel(to_html("&Delta;N", frmt='bi') + " =", self)
+        self.lbl_N_frame = QLabel(to_html("N_Frame", frmt='bi') + " =", self)
+        self.lbl_N_frame.setVisible(False)
         self.led_N_frame = QLineEdit(self)
         self.led_N_frame.setText(str(self.N_frame))
         self.led_N_frame.setToolTip(
             "<span>Frame length; longer frames calculate faster but calculation cannot "
             "be stopped so quickly. "
-            "<i>&Delta;N</i> = 0 calculates all samples in one frame.</span>")
+            "<i>N</i><sub>Frame</sub> = 0 calculates all samples in one frame.</span>")
         self.led_N_frame.setMaximumWidth(qtext_width(N_x=8))
+        self.led_N_frame.setVisible(False)
 
-        self.prg_wdg = QProgressBar(self)
-        self.prg_wdg.setFixedHeight(but_height)
-        self.prg_wdg.setFixedWidth(qtext_width(N_x=6))
-        self.prg_wdg.setMinimum(0)
-        self.prg_wdg.setValue(0)
-
-        self.but_toggle_stim_options = PushButton(" Stimuli ", checked=True)
-        self.but_toggle_stim_options.setObjectName("but_stim_options")
-        self.but_toggle_stim_options.setToolTip("<span>Show / hide stimulus options.</span>")
+        # This frame is a placeholder that is filled with content in Plot_Impz()
+        self.frm_file_io = QFrame(self)
+        self.frm_file_io.setContentsMargins(0, 0, 0, 0)
+        self.frm_file_io.setEnabled(False)
 
         self.lbl_stim_cmplx_warn = QLabel(self)
         self.lbl_stim_cmplx_warn = QLabel(to_html("Cmplx!", frmt='b'), self)
         self.lbl_stim_cmplx_warn.setToolTip(
             '<span>Signal is complex valued; '
             'single-sided and H<sub>id</sub> spectra may be wrong.</span>')
         self.lbl_stim_cmplx_warn.setStyleSheet("background-color : yellow;"
@@ -252,40 +260,39 @@
         self.but_fft_wdg.setIconSize(QSize(but_height, but_height))
         self.but_fft_wdg.setFixedSize(QSize(int(1.5 * but_height), but_height))
         self.but_fft_wdg.setToolTip('<span>Show / hide FFT widget (select window type '
                                     ' and display its properties).</span>')
         self.but_fft_wdg.setCheckable(True)
         self.but_fft_wdg.setChecked(False)
 
-        self.qfft_win_select = QFFTWinSelector(self, self.win_dict)
+        self.qfft_win_select = QFFTWinSelector(self.win_dict)
 
         self.but_fx_scale = PushButton(" FX:Int ")
         self.but_fx_scale.setObjectName("but_fx_scale")
         self.but_fx_scale.setToolTip(
             "<span>Display data with integer (fixpoint) scale.</span>")
 
         self.but_fx_range = PushButton(" FX:Range")
         self.but_fx_range.setObjectName("but_fx_limits")
-        self.but_fx_range.setToolTip("<span>Display limits of fixpoint range.</span>")
+        self.but_fx_range.setToolTip(
+            "<span>Display limits of fixpoint range.</span>")
 
         layH_ctrl_run = QHBoxLayout()
         layH_ctrl_run.addWidget(self.but_auto_run)
         layH_ctrl_run.addWidget(self.but_run)
         layH_ctrl_run.addWidget(self.cmb_sim_select)
+        layH_ctrl_run.addWidget(self.prg_wdg)
         layH_ctrl_run.addSpacing(10)
+        layH_ctrl_run.addWidget(self.lbl_N_frame)
+        layH_ctrl_run.addWidget(self.led_N_frame)
         layH_ctrl_run.addWidget(self.lbl_N_start)
         layH_ctrl_run.addWidget(self.led_N_start)
         layH_ctrl_run.addWidget(self.lbl_N_points)
         layH_ctrl_run.addWidget(self.led_N_points)
-        layH_ctrl_run.addWidget(self.lbl_N_frame)
-        layH_ctrl_run.addWidget(self.led_N_frame)
-        layH_ctrl_run.addWidget(self.prg_wdg)
-
-        layH_ctrl_run.addSpacing(20)
-        layH_ctrl_run.addWidget(self.but_toggle_stim_options)
+        layH_ctrl_run.addWidget(self.frm_file_io)
         layH_ctrl_run.addSpacing(5)
         layH_ctrl_run.addWidget(self.lbl_stim_cmplx_warn)
         layH_ctrl_run.addSpacing(20)
         layH_ctrl_run.addWidget(self.but_fft_wdg)
         layH_ctrl_run.addWidget(self.qfft_win_select)
         layH_ctrl_run.addSpacing(20)
         layH_ctrl_run.addWidget(self.but_fx_scale)
@@ -297,182 +304,238 @@
         self.wdg_ctrl_run = QWidget(self)
         self.wdg_ctrl_run.setLayout(layH_ctrl_run)
         # --- end of run control ----------------------------------------
 
         # ----------- ---------------------------------------------------
         # Controls for time domain
         # ---------------------------------------------------------------
+        self.lbl_title_plot_time = QLabel("Plots:")
+        self.lbl_title_plot_time.setObjectName("large")
+
+        # setting up background color and border
+        # self.lbl_title_plot_time.setStyleSheet("font-size:14")
+        # self.lbl_title_plot_time.setFont(QFont('Arial', 10))
+        # self.lbl_title_plot_time.resize(200, 20)
+        # color_effect = QGraphicsColorizeEffect()
+        # color_effect.setColor(Qt.darkGreen)
+        # self.lbl_title_plot_time.setGraphicsEffect(color_effect)
+
         self.lbl_plt_time_stim = QLabel(to_html("Stim. x", frmt='bi'), self)
         self.cmb_plt_time_stim = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_time_stim, self.plot_styles_list, self.plt_time_stim)
-        self.cmb_plt_time_stim.setToolTip("<span>Plot style for stimulus.</span>")
+        self.cmb_plt_time_stim.setToolTip(
+            "<span>Plot style for stimulus.</span>")
+
+        self.lbl_plt_time_stim_interp = QLabel(
+            to_html("&nbsp;&nbsp;x(t)", frmt='bi'), self)
+        self.chk_plt_time_stim_interp = QCheckBox(self)
+        self.chk_plt_time_stim_interp.setChecked(False)
+        self.chk_plt_time_stim_interp.setObjectName("chk_plt_time_stim_interp")
+        self.chk_plt_time_stim_interp.setToolTip(
+            '<span>Plot interpolated pseudo-analog stimulus "<i>x</i>(<i>t</i>)", '
+            'valid up to approx. 0.4 <i>f<sub>S</sub></i>.</span>')
 
         self.lbl_plt_time_stmq = QLabel(to_html(
-            "&nbsp;&nbsp;Fixp. Stim. x_Q", frmt='bi'), self)
+            "&nbsp;&nbsp;FX Stim. x_Q", frmt='bi'), self)
         self.cmb_plt_time_stmq = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_time_stmq, self.plot_styles_list, self.plt_time_stmq)
         self.cmb_plt_time_stmq.setToolTip("<span>Plot style for <em>fixpoint</em> "
                                           "(quantized) stimulus.</span>")
 
-        lbl_plt_time_resp = QLabel(to_html("&nbsp;&nbsp;Resp. y", frmt='bi'), self)
+        lbl_plt_time_resp = QLabel(
+            to_html("&nbsp;&nbsp;Resp. y", frmt='bi'), self)
         self.cmb_plt_time_resp = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_time_resp, self.plot_styles_list, self.plt_time_resp)
-        self.cmb_plt_time_resp.setToolTip("<span>Plot style for response.</span>")
+        self.cmb_plt_time_resp.setToolTip(
+            "<span>Plot style for response.</span>")
 
         self.lbl_win_time = QLabel(to_html("&nbsp;&nbsp;Win", frmt='bi'), self)
         self.chk_win_time = QCheckBox(self)
         self.chk_win_time.setObjectName("chk_win_time")
         self.chk_win_time.setToolTip(
             '<span>Plot FFT windowing function.</span>')
         self.chk_win_time.setChecked(False)
 
         line1 = QVLine()
         line2 = QVLine(width=5)
 
         self.but_log_time = PushButton(" dB")
         self.but_log_time.setObjectName("but_log_time")
-        self.but_log_time.setToolTip("<span>Logarithmic scale for y-axis.</span>")
+        self.but_log_time.setToolTip(
+            "<span>Logarithmic scale for y-axis.</span>")
 
         lbl_plt_time_spgr = QLabel(to_html("Spectrogram", frmt='bi'), self)
         self.cmb_plt_time_spgr = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_time_spgr, self.cmb_time_spgr_items, self.plt_time_spgr)
-        spgr_en = self.plt_time_spgr != "none"
 
         self.cmb_mode_spgr_time = QComboBox(self)
         qcmb_box_populate(
             self.cmb_mode_spgr_time, self.cmb_mode_spgr_time_items, self.mode_spgr_time)
-        self.cmb_mode_spgr_time.setVisible(spgr_en)
 
-        self.lbl_byfs_spgr_time = QLabel(to_html("&nbsp;per f_S", frmt='b'), self)
-        self.lbl_byfs_spgr_time.setVisible(spgr_en)
+        self.lbl_byfs_spgr_time = QLabel(
+            to_html("&nbsp;per f_S", frmt='b'), self)
         self.chk_byfs_spgr_time = QCheckBox(self)
         self.chk_byfs_spgr_time.setObjectName("chk_log_spgr")
         self.chk_byfs_spgr_time.setToolTip("<span>Display spectral density "
                                            "i.e. scale by f_S</span>")
         self.chk_byfs_spgr_time.setChecked(True)
-        self.chk_byfs_spgr_time.setVisible(spgr_en)
 
         self.but_log_spgr_time = QPushButton("dB")
         self.but_log_spgr_time.setMaximumWidth(qtext_width(text=" dB"))
         self.but_log_spgr_time.setObjectName("but_log_spgr")
         self.but_log_spgr_time.setToolTip(
             "<span>Logarithmic scale for spectrogram.</span>")
         self.but_log_spgr_time.setCheckable(True)
         self.but_log_spgr_time.setChecked(True)
-        self.but_log_spgr_time.setVisible(spgr_en)
 
-        self.lbl_time_nfft_spgr = QLabel(to_html("&nbsp;N_FFT =", frmt='bi'), self)
-        self.lbl_time_nfft_spgr.setVisible(spgr_en)
+        self.lbl_time_nfft_spgr = QLabel(
+            to_html("&nbsp;N_FFT =", frmt='bi'), self)
         self.led_time_nfft_spgr = QLineEdit(self)
         self.led_time_nfft_spgr.setText(str(self.time_nfft_spgr))
         self.led_time_nfft_spgr.setToolTip("<span>Number of FFT points per "
                                            "spectrogram segment.</span>")
-        self.led_time_nfft_spgr.setVisible(spgr_en)
 
-        self.lbl_time_ovlp_spgr = QLabel(to_html("&nbsp;N_OVLP =", frmt='bi'), self)
-        self.lbl_time_ovlp_spgr.setVisible(spgr_en)
+        self.lbl_time_ovlp_spgr = QLabel(
+            to_html("&nbsp;N_OVLP =", frmt='bi'), self)
         self.led_time_ovlp_spgr = QLineEdit(self)
         self.led_time_ovlp_spgr.setText(str(self.time_ovlp_spgr))
         self.led_time_ovlp_spgr.setToolTip("<span>Number of overlap data points "
                                            "between spectrogram segments.</span>")
-        self.led_time_ovlp_spgr.setVisible(spgr_en)
 
         self.lbl_log_bottom_time = QLabel(to_html("min =", frmt='bi'), self)
         self.led_log_bottom_time = QLineEdit(self)
         self.led_log_bottom_time.setText(str(self.bottom_t))
         self.led_log_bottom_time.setMaximumWidth(qtext_width(N_x=8))
         self.led_log_bottom_time.setToolTip(
             "<span>Minimum display value for time and spectrogram plots with log. scale."
             "</span>")
         self.lbl_log_bottom_time.setVisible(
             self.but_log_time.isChecked() or
-            (spgr_en and self.but_log_spgr_time.isChecked()))
-        self.led_log_bottom_time.setVisible(self.lbl_log_bottom_time.isVisible())
+            ((self.plt_time_spgr != "none") and self.but_log_spgr_time.isChecked()))
+        self.led_log_bottom_time.setVisible(
+            self.lbl_log_bottom_time.isVisible())
 
         # self.lbl_colorbar_time = QLabel(to_html("&nbsp;Col.bar", frmt='b'), self)
         # self.lbl_colorbar_time.setVisible(spgr_en)
         # self.chk_colorbar_time = QCheckBox(self)
         # self.chk_colorbar_time.setObjectName("chk_colorbar_time")
         # self.chk_colorbar_time.setToolTip("<span>Enable colorbar</span>")
         # self.chk_colorbar_time.setChecked(True)
         # self.chk_colorbar_time.setVisible(spgr_en)
 
-        layH_ctrl_time = QHBoxLayout()
-        layH_ctrl_time.addWidget(self.lbl_plt_time_stim)
-        layH_ctrl_time.addWidget(self.cmb_plt_time_stim)
-        #
-        layH_ctrl_time.addWidget(self.lbl_plt_time_stmq)
-        layH_ctrl_time.addWidget(self.cmb_plt_time_stmq)
+        layH_ctrl_time_0 = QHBoxLayout()
+        layH_ctrl_time_0.addWidget(self.lbl_title_plot_time)
+        # layH_ctrl_time_0.addSpacing(10)
+
+        layH_ctrl_time_1 = QHBoxLayout()
+        layH_ctrl_time_1.addWidget(self.lbl_plt_time_stim)
+        layH_ctrl_time_1.addWidget(self.cmb_plt_time_stim)
+        layH_ctrl_time_1.addWidget(self.lbl_plt_time_stim_interp)
+        layH_ctrl_time_1.addWidget(self.chk_plt_time_stim_interp)
+#
+        layH_ctrl_time_1.addWidget(self.lbl_plt_time_stmq)
+        layH_ctrl_time_1.addWidget(self.cmb_plt_time_stmq)
         #
-        layH_ctrl_time.addWidget(lbl_plt_time_resp)
-        layH_ctrl_time.addWidget(self.cmb_plt_time_resp)
+        layH_ctrl_time_1.addWidget(lbl_plt_time_resp)
+        layH_ctrl_time_1.addWidget(self.cmb_plt_time_resp)
         #
-        layH_ctrl_time.addWidget(self.lbl_win_time)
-        layH_ctrl_time.addWidget(self.chk_win_time)
-        layH_ctrl_time.addSpacing(5)
-        layH_ctrl_time.addWidget(line1)
-        layH_ctrl_time.addSpacing(5)
+        layH_ctrl_time_1.addWidget(self.lbl_win_time)
+        layH_ctrl_time_1.addWidget(self.chk_win_time)
+        layH_ctrl_time_1.addSpacing(5)
+        layH_ctrl_time_1.addWidget(line1)
+        layH_ctrl_time_1.addSpacing(5)
         #
-        layH_ctrl_time.addWidget(self.lbl_log_bottom_time)
-        layH_ctrl_time.addWidget(self.led_log_bottom_time)
-        layH_ctrl_time.addWidget(self.but_log_time)
-
-        layH_ctrl_time.addSpacing(5)
-        layH_ctrl_time.addWidget(line2)
-        layH_ctrl_time.addSpacing(5)
+        layH_ctrl_time_1.addWidget(self.lbl_log_bottom_time)
+        layH_ctrl_time_1.addWidget(self.led_log_bottom_time)
+        layH_ctrl_time_1.addWidget(self.but_log_time)
+
+        layH_ctrl_time_1.addSpacing(5)
+        layH_ctrl_time_1.addWidget(line2)
+        layH_ctrl_time_1.addSpacing(5)
         #
-        layH_ctrl_time.addWidget(lbl_plt_time_spgr)
-        layH_ctrl_time.addWidget(self.cmb_plt_time_spgr)
-        layH_ctrl_time.addWidget(self.cmb_mode_spgr_time)
-        layH_ctrl_time.addWidget(self.lbl_byfs_spgr_time)
-        layH_ctrl_time.addWidget(self.chk_byfs_spgr_time)
-        layH_ctrl_time.addWidget(self.but_log_spgr_time)
-        layH_ctrl_time.addWidget(self.lbl_time_nfft_spgr)
-        layH_ctrl_time.addWidget(self.led_time_nfft_spgr)
-        layH_ctrl_time.addWidget(self.lbl_time_ovlp_spgr)
-        layH_ctrl_time.addWidget(self.led_time_ovlp_spgr)
-
-        layH_ctrl_time.addStretch(10)
+        layH_ctrl_time_1.addWidget(lbl_plt_time_spgr)
+        layH_ctrl_time_1.addWidget(self.cmb_plt_time_spgr)
+        layH_ctrl_time_1.addStretch(10)
+
+        layH_ctrl_time_spgr = QHBoxLayout()
+        layH_ctrl_time_spgr.addWidget(self.cmb_mode_spgr_time)
+        layH_ctrl_time_spgr.addWidget(self.lbl_byfs_spgr_time)
+        layH_ctrl_time_spgr.addWidget(self.chk_byfs_spgr_time)
+        layH_ctrl_time_spgr.addWidget(self.but_log_spgr_time)
+        layH_ctrl_time_spgr.addWidget(self.lbl_time_nfft_spgr)
+        layH_ctrl_time_spgr.addWidget(self.led_time_nfft_spgr)
+        layH_ctrl_time_spgr.addWidget(self.lbl_time_ovlp_spgr)
+        layH_ctrl_time_spgr.addWidget(self.led_time_ovlp_spgr)
+        layH_ctrl_time_spgr.addStretch(10)
 
         # layH_ctrl_time.setContentsMargins(*params['wdg_margins'])
+        self.wdg_ctrl_time_0 = QWidget(self)
+        self.wdg_ctrl_time_0.setLayout(layH_ctrl_time_0)
+        self.wdg_ctrl_time_0.setContentsMargins(0, 0, 0, 0)
+        self.wdg_ctrl_time_1 = QWidget(self)
+        self.wdg_ctrl_time_1.setLayout(layH_ctrl_time_1)
+        self.wdg_ctrl_time_1.setContentsMargins(0, 0, 0, 0)
+        self.wdg_ctrl_time_spgr = QWidget(self)
+        self.wdg_ctrl_time_spgr.setLayout(layH_ctrl_time_spgr)
+        self.wdg_ctrl_time_spgr.setContentsMargins(0, 0, 0, 0)
+
+        layG_ctrl_time = QGridLayout()
+        layG_ctrl_time.addWidget(self.wdg_ctrl_time_0, 0, 0, 2, 1)
+        layG_ctrl_time.addWidget(self.wdg_ctrl_time_1, 0, 1)
+        layG_ctrl_time.addWidget(self.wdg_ctrl_time_spgr, 1, 1)
+        layG_ctrl_time.setContentsMargins(0, 0, 0, 0)
+        layG_ctrl_time.setVerticalSpacing(0)
 
         self.wdg_ctrl_time = QWidget(self)
-        self.wdg_ctrl_time.setLayout(layH_ctrl_time)
+        self.wdg_ctrl_time.setLayout(layG_ctrl_time)
+        self.wdg_ctrl_time.setObjectName("transparent")
+        self.wdg_ctrl_time.setContentsMargins(0, 0, 0, 0) # (*rc.params['wdg_margins'])
+
+        self.wdg_ctrl_time_spgr.setVisible(self.plt_time_spgr != "none")
+
         # ---- end time domain ------------------
 
         # ---------------------------------------------------------------
         # Controls for frequency domain
         # ---------------------------------------------------------------
+        self.lbl_title_plot_freq = QLabel("Plots:")
+        self.lbl_title_plot_freq.setObjectName("large")
+        #
         self.lbl_plt_freq_stim = QLabel(to_html("Stimulus X", frmt='bi'), self)
         self.cmb_plt_freq_stim = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_freq_stim, self.plot_styles_list, self.plt_freq_stim)
-        self.cmb_plt_freq_stim.setToolTip("<span>Plot style for stimulus.</span>")
+        self.cmb_plt_freq_stim.setToolTip(
+            "<span>Plot style for stimulus.</span>")
 
-        self.lbl_plt_freq_stmq = QLabel(to_html("&nbsp;Fixp. Stim. X_Q", frmt='bi'), self)
+        self.lbl_plt_freq_stmq = QLabel(
+            to_html("&nbsp;Fixp. Stim. X_Q", frmt='bi'), self)
         self.cmb_plt_freq_stmq = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_freq_stmq, self.plot_styles_list, self.plt_freq_stmq)
         self.cmb_plt_freq_stmq.setToolTip(
             "<span>Plot style for <em>fixpoint</em> (quantized) stimulus.</span>")
 
-        lbl_plt_freq_resp = QLabel(to_html("&nbsp;Response Y", frmt='bi'), self)
+        lbl_plt_freq_resp = QLabel(
+            to_html("&nbsp;Response Y", frmt='bi'), self)
         self.cmb_plt_freq_resp = QComboBox(self)
         qcmb_box_populate(
             self.cmb_plt_freq_resp, self.plot_styles_list, self.plt_freq_resp)
-        self.cmb_plt_freq_resp.setToolTip("<span>Plot style for response.</span>")
+        self.cmb_plt_freq_resp.setToolTip(
+            "<span>Plot style for response.</span>")
 
         self.but_log_freq = QPushButton("dB")
         self.but_log_freq.setMaximumWidth(qtext_width(" dB"))
         self.but_log_freq.setObjectName(".but_log_freq")
-        self.but_log_freq.setToolTip("<span>Logarithmic scale for y-axis.</span>")
+        self.but_log_freq.setToolTip(
+            "<span>Logarithmic scale for y-axis.</span>")
         self.but_log_freq.setCheckable(True)
         self.but_log_freq.setChecked(True)
 
         self.lbl_log_bottom_freq = QLabel(to_html("min =", frmt='bi'), self)
         self.lbl_log_bottom_freq.setVisible(self.but_log_freq.isChecked())
         self.led_log_bottom_freq = QLineEdit(self)
         self.led_log_bottom_freq.setText(str(self.bottom_f))
@@ -495,59 +558,76 @@
                                "from the filter coefficients.</span>")
         self.but_Hf.setChecked(False)
         self.but_Hf.setCheckable(True)
 
         self.but_freq_norm_impz = QPushButtonRT(text="<b><i>E<sub>X</sub></i> = 1</b>",
                                                 margin=5)
         self.but_freq_norm_impz.setToolTip(
-            "<span>Normalize the FFT of the stimulus with <i>N<sub>FFT</sub></i> for "
-            "<i>E<sub>X</sub></i> = 1. For a dirac pulse, this yields "
-            "|<i>Y(f)</i>| = |<i>H(f)</i>|. DC and Noise need to be "
+            "<span>Normalize the FFT of an impulse stimulus with <i>N<sub>FFT</sub></i> "
+            "to an energy <i>E<sub>X</sub></i> = 1. For a dirac pulse, this yields "
+            "|<i>Y(f)</i>| = |<i>H(f)</i>|. DC, Noise and file I/O need to be "
             "turned off, window should be <b>Rectangular</b>.</span>")
         self.but_freq_norm_impz.setCheckable(True)
         self.but_freq_norm_impz.setChecked(True)
         self.but_freq_norm_impz.setObjectName("freq_norm_impz")
 
         self.but_freq_show_info = QPushButton("Info", self)
         self.but_freq_show_info.setMaximumWidth(qtext_width(" Info "))
         self.but_freq_show_info.setObjectName("but_show_info_freq")
-        self.but_freq_show_info.setToolTip("<span>Show signal power in legend.</span>")
+        self.but_freq_show_info.setToolTip(
+            "<span>Show signal power in legend.</span>")
         self.but_freq_show_info.setCheckable(True)
         self.but_freq_show_info.setChecked(False)
 
-        layH_ctrl_freq = QHBoxLayout()
-        layH_ctrl_freq.addWidget(self.lbl_plt_freq_stim)
-        layH_ctrl_freq.addWidget(self.cmb_plt_freq_stim)
+        layH_ctrl_freq_0 = QHBoxLayout()
+        layH_ctrl_freq_0.addWidget(self.lbl_title_plot_freq)
+
+        layH_ctrl_freq_1 = QHBoxLayout()
+        layH_ctrl_freq_1.addWidget(self.lbl_plt_freq_stim)
+        layH_ctrl_freq_1.addWidget(self.cmb_plt_freq_stim)
         #
-        layH_ctrl_freq.addWidget(self.lbl_plt_freq_stmq)
-        layH_ctrl_freq.addWidget(self.cmb_plt_freq_stmq)
+        layH_ctrl_freq_1.addWidget(self.lbl_plt_freq_stmq)
+        layH_ctrl_freq_1.addWidget(self.cmb_plt_freq_stmq)
         #
-        layH_ctrl_freq.addWidget(lbl_plt_freq_resp)
-        layH_ctrl_freq.addWidget(self.cmb_plt_freq_resp)
+        layH_ctrl_freq_1.addWidget(lbl_plt_freq_resp)
+        layH_ctrl_freq_1.addWidget(self.cmb_plt_freq_resp)
         #
-        layH_ctrl_freq.addSpacing(5)
-        layH_ctrl_freq.addWidget(self.but_Hf)
-        layH_ctrl_freq.addStretch(1)
+        layH_ctrl_freq_1.addSpacing(5)
+        layH_ctrl_freq_1.addWidget(self.but_Hf)
+        layH_ctrl_freq_1.addStretch(1)
         #
-        layH_ctrl_freq.addWidget(self.lbl_log_bottom_freq)
-        layH_ctrl_freq.addWidget(self.led_log_bottom_freq)
-        layH_ctrl_freq.addWidget(self.but_log_freq)
-        layH_ctrl_freq.addStretch(1)
-        layH_ctrl_freq.addWidget(self.cmb_freq_display)
-        layH_ctrl_freq.addStretch(1)
-
-        layH_ctrl_freq.addWidget(self.but_freq_norm_impz)
-        layH_ctrl_freq.addStretch(1)
-        layH_ctrl_freq.addWidget(self.but_freq_show_info)
-        layH_ctrl_freq.addStretch(10)
-
-        # layH_ctrl_freq.setContentsMargins(*params['wdg_margins'])
+        layH_ctrl_freq_1.addWidget(self.lbl_log_bottom_freq)
+        layH_ctrl_freq_1.addWidget(self.led_log_bottom_freq)
+        layH_ctrl_freq_1.addWidget(self.but_log_freq)
+        layH_ctrl_freq_1.addStretch(1)
+        layH_ctrl_freq_1.addWidget(self.cmb_freq_display)
+        layH_ctrl_freq_1.addStretch(1)
+
+        layH_ctrl_freq_1.addWidget(self.but_freq_norm_impz)
+        layH_ctrl_freq_1.addStretch(1)
+        layH_ctrl_freq_1.addWidget(self.but_freq_show_info)
+        layH_ctrl_freq_1.addStretch(10)
+        # layH_ctrl_freq_1.setContentsMargins(*params['wdg_margins'])
+
+        self.wdg_ctrl_freq_0 = QWidget(self)
+        self.wdg_ctrl_freq_0.setLayout(layH_ctrl_freq_0)
+        self.wdg_ctrl_freq_0.setContentsMargins(0, 0, 0, 0)
+        self.wdg_ctrl_freq_1 = QWidget(self)
+        self.wdg_ctrl_freq_1.setLayout(layH_ctrl_freq_1)
+        self.wdg_ctrl_freq_1.setContentsMargins(0, 0, 0, 0)
+        layG_ctrl_freq = QGridLayout()
+        layG_ctrl_freq.addWidget(self.wdg_ctrl_freq_0, 0, 0)
+        layG_ctrl_freq.addWidget(self.wdg_ctrl_freq_1, 0, 1)
+        layG_ctrl_freq.setContentsMargins(0, 0, 0, 0)
+        layG_ctrl_freq.setVerticalSpacing(0)
 
         self.wdg_ctrl_freq = QWidget(self)
-        self.wdg_ctrl_freq.setLayout(layH_ctrl_freq)
+        self.wdg_ctrl_freq.setLayout(layG_ctrl_freq)
+        self.wdg_ctrl_freq.setObjectName("transparent")
+        self.wdg_ctrl_freq.setContentsMargins(0, 0, 0, 0)  # (*rc.params['wdg_margins'])
         # ---- end Frequency Domain ------------------
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         # connect FFT widget to qfft_selector and vice versa and to and signals upstream:
         self.fft_widget.sig_tx.connect(self.process_sig_rx)
@@ -597,25 +677,26 @@
         self.N_start = safe_eval(self.led_N_start.text(), self.N_start,
                                  return_type='int', sign='poszero')
 
         # Read value for number of data points to be plotted from UI
         self.N_user = safe_eval(self.led_N_points.text(), self.N_user,
                                 return_type='int', sign='poszero')
 
-        if N_end > 0:  # total number of data points was specified, e.g. for file I/O
+        if N_end > 0:  # total number of data points was specified, e.g. from file I/O
             if N_end <= self.N_start:
                 logger.warning(
                     f"Total number of data points must be {N_end} > "
                     f"N_start = {self.N_start}, setting N_start = 0.")
                 self.N_start = 0
                 self.led_N_start.setText(str(self.N_start))  # update widget
 
             self.N_end = N_end
             # calculate number of data points to be plotted
             self.N = self.N_end - self.N_start
+            self.led_N_points.setText(str(self.N))  # update widget
         else:
             if self.N_user == 0:  # automatic calculation
                 self.N = self.calc_n_points(self.N_user)
                 self.led_N_points.setText("0")  # widget remains set to 0
             else:
                 self.N = self.N_user  # specified by user
                 self.led_N_points.setText(str(self.N))  # update widget
@@ -624,15 +705,16 @@
 
         # read number of data points per frame from UI
         self.N_frame_user = safe_eval(self.led_N_frame.text(), self.N_frame_user,
                                       return_type='int', sign='poszero')
 
         if self.N_frame_user == 0:
             self.N_frame = self.N_end  # use N_end for frame length
-            self.led_N_frame.setText("0")  # update widget with "0" as set by user
+            # update widget with "0" as set by user
+            self.led_N_frame.setText("0")
         else:
             self.N_frame = self.N_frame_user
             self.led_N_frame.setText(str(self.N_frame))  # update widget
 
         if emit:
             # use `'ui_local_changed'` as this triggers recalculation of the
             #  transient response
@@ -691,15 +773,16 @@
 
     mainw = PlotImpz_UI(None)
     layVMain = QVBoxLayout()
     layVMain.addWidget(mainw.wdg_ctrl_time)
     layVMain.addWidget(mainw.wdg_ctrl_freq)
     layVMain.addWidget(mainw.wdg_ctrl_stim)
     layVMain.addWidget(mainw.wdg_ctrl_run)
-    layVMain.setContentsMargins(*params['wdg_margins'])  # (left, top, right, bottom)
+    # (left, top, right, bottom)
+    layVMain.setContentsMargins(*params['wdg_margins'])
 
     mainw.setLayout(layVMain)
 
     app.setActiveWindow(mainw)
     mainw.show()
     sys.exit(app.exec_())
```

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/plot_phi.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/plot_phi.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,21 +50,25 @@
         #              .format(dict_sig, self.needs_calc, self.isVisible()))
 
         if dict_sig['id'] == id(self):
             logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
             return
 
         if self.isVisible():
-            if 'data_changed' in dict_sig or 'home' in dict_sig or self.needs_calc:
+            if 'data_changed' in dict_sig or self.needs_calc\
+                    or ('mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'home'):
                 self.draw()
                 self.needs_calc = False
                 self.needs_draw = False
             elif 'view_changed' in dict_sig or self.needs_draw:
                 self.update_view()
                 self.needs_draw = False
+            elif 'mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'ui_level':
+                self.frmControls.setVisible(dict_sig['value'] == 0)
+
         else:
             if 'data_changed' in dict_sig:
                 self.needs_calc = True
             elif 'view_changed' in dict_sig:
                 self.needs_draw = True
 
 # ------------------------------------------------------------------------------
@@ -108,14 +112,15 @@
         # main widget, encompassing the other widgets
         # ----------------------------------------------------------------------
         self.mplwidget = MplWidget(self)
         self.mplwidget.layVMainMpl.addWidget(self.frmControls)
         self.mplwidget.layVMainMpl.setContentsMargins(*params['mpl_margins'])
         self.mplwidget.mplToolbar.a_he.setEnabled(True)
         self.mplwidget.mplToolbar.a_he.info = "manual/plot_phi.html"
+        self.mplwidget.mplToolbar.a_ui_num_levels = 2
         self.setLayout(self.mplwidget.layVMainMpl)
 
         self.init_axes()
 
         self.draw()  # initial drawing
 
         # ----------------------------------------------------------------------
@@ -230,15 +235,14 @@
 # ------------------------------------------------------------------------------
     def redraw(self):
         """
         Redraw the canvas when e.g. the canvas size has changed
         """
         self.mplwidget.redraw()
 
-
 # ------------------------------------------------------------------------------
 if __name__ == "__main__":
     """ Run widget standalone with `python -m pyfda.plot_widgets.plot_phi` """
     import sys
     from pyfda.libs.compat import QApplication
     from pyfda import pyfda_rc as rc
```

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/plot_pz.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/plot_pz.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,24 +65,28 @@
     def process_sig_rx(self, dict_sig: dict = None) -> None:
         """
         Process signals coming from the navigation toolbar and from sig_rx
         """
         # logger.info("Processing {0} | needs_draw = {1}, visible = {2}"\
         #              .format(dict_sig, self.needs_calc, self.isVisible()))
         if self.isVisible():
-            if 'data_changed' in dict_sig or 'home' in dict_sig or self.needs_calc:
+            if 'data_changed' in dict_sig or self.needs_calc\
+                    or ('mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'home'):
                 self.draw()
                 self.needs_calc = False
                 self.needs_draw = False
             elif 'view_changed' in dict_sig or self.needs_draw:
                 self.update_view()
                 self.needs_draw = False
             elif 'ui_global_changed' in dict_sig\
                     and dict_sig['ui_global_changed'] == 'resized':
                 self.draw()
+            elif 'mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'ui_level':
+                self.frmControls.setVisible(dict_sig['value'] == 0)
+
         else:
             if 'data_changed' in dict_sig:
                 self.needs_calc = True
             elif 'view_changed' in dict_sig:
                 self.needs_draw = True
             elif 'ui_global_changed' in dict_sig\
                     and dict_sig['ui_global_changed'] == 'resized':
@@ -166,14 +170,15 @@
         # main widget, encompassing the other widgets
         # ----------------------------------------------------------------------
         self.mplwidget = MplWidget(self)
         self.mplwidget.layVMainMpl.addWidget(self.frmControls)
         self.mplwidget.layVMainMpl.setContentsMargins(*params['wdg_margins'])
         self.mplwidget.mplToolbar.a_he.setEnabled(True)
         self.mplwidget.mplToolbar.a_he.info = "manual/plot_pz.html"
+        self.mplwidget.mplToolbar.a_ui_num_levels = 2
         self.setLayout(self.mplwidget.layVMainMpl)
 
         self.init_axes()
 
         self._log_clicked()  # calculate and draw poles and zeros
 
         # ----------------------------------------------------------------------
@@ -265,25 +270,14 @@
         (re)draw P/Z plot
         """
         p_marker = params['P_Marker']
         z_marker = params['Z_Marker']
 
         zpk = fb.fil[0]['zpk']
 
-        # add antiCausals if they exist (must take reciprocal to plot)
-        if 'rpk' in fb.fil[0]:
-            zA = fb.fil[0]['zpk'][0]
-            zA = np.conj(1./zA)
-            pA = fb.fil[0]['zpk'][1]
-            pA = np.conj(1./pA)
-            zC = np.append(zpk[0], zA)
-            pC = np.append(zpk[1], pA)
-            zpk[0] = zC
-            zpk[1] = pC
-
         self.ax.clear()
 
         [z, p, k] = self.zplane(
             z=zpk[0], p=zpk[1], k=zpk[2], plt_ax=self.ax,
             plt_poles=self.but_fir_poles.isChecked() or fb.fil[0]['ft'] == 'IIR',
             mps=p_marker[0], mpc=p_marker[1], mzs=z_marker[0], mzc=z_marker[1])
```

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/plot_tab_widgets.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/plot_tab_widgets.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/plot_tau_g.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/plot_tau_g.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         self.frmControls.setLayout(layHControls)
 
         self.mplwidget = MplWidget(self)
         self.mplwidget.layVMainMpl.addWidget(self.frmControls)
         self.mplwidget.layVMainMpl.setContentsMargins(*params['mpl_margins'])
         self.mplwidget.mplToolbar.a_he.setEnabled(True)
         self.mplwidget.mplToolbar.a_he.info = "manual/plot_tau_g.html"
+        self.mplwidget.mplToolbar.a_ui_num_levels = 2
         self.setLayout(self.mplwidget.layVMainMpl)
 
         self.init_axes()
         self.draw()  # initial drawing of tau_g
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
@@ -109,19 +110,23 @@
     def process_sig_rx(self, dict_sig=None):
         """
         Process signals coming from the navigation toolbar and from sig_rx
         """
         # logger.debug("Processing {0} | needs_calc = {1}, visible = {2}"
         #              .format(dict_sig, self.needs_calc, self.isVisible()))
         if self.isVisible():
-            if 'data_changed' in dict_sig or 'home' in dict_sig or self.needs_calc:
+            if 'data_changed' in dict_sig or self.needs_calc\
+                    or ('mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'home'):
                 self.draw()
                 self.needs_calc = False
             elif 'view_changed' in dict_sig:
                 self.update_view()
+            elif 'mpl_toolbar' in dict_sig and dict_sig['mpl_toolbar'] == 'ui_level':
+                self.frmControls.setVisible(dict_sig['value'] == 0)
+
         else:
             if 'data_changed' in dict_sig or 'view_changed' in dict_sig:
                 self.needs_calc = True
 
 # ------------------------------------------------------------------------------
     def init_axes(self):
         """
```

### Comparing `pyfda-0.7.1/pyfda/plot_widgets/tran/plot_tran_stim_ui.py` & `pyfda-0.8.0a2/pyfda/plot_widgets/tran/plot_tran_stim_ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 # (see file LICENSE in root directory for details)
 
 """
 Create the UI for the Plot_Tran_Impz class
 """
 import collections
 
-from PyQt5.QtWidgets import QSizePolicy
 from pyfda.libs.compat import (
-    QWidget, QComboBox, QLineEdit, QLabel, QPushButton, QFrame,
+    QWidget, QComboBox, QLineEdit, QLabel, QPushButton,
     pyqtSignal, QEvent, Qt, QHBoxLayout, QVBoxLayout, QGridLayout)
 
 from pyfda.libs.pyfda_lib import to_html, safe_eval, pprint_log
 import pyfda.filterbroker as fb
 from pyfda.libs.pyfda_qt_lib import (
-    qcmb_box_populate, qget_cmb_box, qtext_width, QVLine)
-from pyfda.pyfda_rc import params  # FMT string for QLineEdit fields, e.g. '{:.3g}'
+    qcmb_box_populate, qget_cmb_box, qtext_width, qstyle_widget, QVLine, PushButton)
+# FMT string for QLineEdit fields, e.g. '{:.3g}'
+from pyfda.pyfda_rc import params
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 class Plot_Tran_Stim_UI(QWidget):
     """
@@ -47,19 +47,20 @@
         - qfft_win_select
         """
 
         # logger.warning("PROCESS_SIG_RX - vis: {0}\n{1}"
         #             .format(self.isVisible(), pprint_log(dict_sig)))
 
         if 'id' in dict_sig and dict_sig['id'] == id(self):
-            logger.warning("Stopped infinite loop:\n{0}".format(pprint_log(dict_sig)))
+            logger.warning("Stopped infinite loop:\n{0}".format(
+                pprint_log(dict_sig)))
             return
         elif 'view_changed' in dict_sig:
             if dict_sig['view_changed'] == 'f_S':
-                self.recalc_freqs()
+                self.normalize_freqs()
 
 # ------------------------------------------------------------------------------
     def __init__(self):
         super().__init__()
 
         """
         Intitialize the widget, consisting of:
@@ -75,24 +76,25 @@
         self.cmb_stim_periodic_item = "square"
         self.cmb_stim_modulation_item = "am"
         self.stim = "dirac"
         self.impulse_type = "dirac"
         self.sinusoid_type = "sine"
 
         self.chirp_type = "linear"
-        self.cmb_file_io_default = "off"
+        self.cmb_file_io_default = "use"
 
         self.f1 = 0.02
         self.f2 = 0.03
         self.A1 = 1.0
         self.A2 = 0.0
         self.phi1 = self.phi2 = 0
         self.T1 = self.T2 = 0
         self.TW1 = self.TW2 = 1
         self.BW1 = self.BW2 = 0.5
+        self.N1 = self.N2 = 5
         self.noi = 0.1
         self.noise = "none"
         self.mls_b = 8
         self.DC = 0.0
         self.stim_formula = "A1 * abs(sin(2 * pi * f1 * n))"
         self.stim_par1 = 0.5
 
@@ -110,97 +112,97 @@
             "gauss":   {"dc", "a1", "a2", "T1", "T2", "f1", "f2", "BW1", "BW2",
                         "norm", "noise"},
             "rect":    {"dc", "a1", "T1", "TW1", "norm", "noise"},
             "step":    {"a1", "T1", "noise"},
             "cos":     {"dc", "a1", "a2", "phi1", "phi2", "f1", "f2", "noise"},
             "sine":    {"dc", "a1", "a2", "phi1", "phi2", "f1", "f2", "noise"},
             "exp":     {"dc", "a1", "a2", "phi1", "phi2", "f1", "f2", "noise"},
-            "diric":   {"dc", "a1", "phi1", "T1", "TW1", "f1", "noise"},
+            "diric":   {"dc", "a1", "T1", "N1", "f1", "noise"},
 
             "chirp":   {"dc", "a1", "phi1", "f1", "f2", "T2", "noise"},
             "triang":  {"dc", "a1", "phi1", "f1", "noise", "bl"},
             "saw":     {"dc", "a1", "phi1", "f1", "noise", "bl"},
             "square":  {"dc", "a1", "phi1", "f1", "noise", "bl", "par1"},
             "comb":    {"dc", "a1", "phi1", "f1", "noise"},
             "am":      {"dc", "a1", "a2", "phi1", "phi2", "f1", "f2", "noise"},
             "pmfm":    {"dc", "a1", "a2", "phi1", "phi2", "f1", "f2", "noise"},
             "pwm":     {"dc", "a1", "a2", "phi1", "phi2", "f1", "f2", "noise", "bl"},
-            "formula": {"dc", "a1", "a2", "phi1", "phi2", "f1", "f2", "BW1",
-                        "BW2", "noise"}
-         })
+            "formula": {"dc", "a1", "a2", "phi1", "phi2", "f1", "f2", "N1", "N2",
+                        "T1", "T2", "BW1", "BW2", "noise"}
+        })
 
         # combobox tooltip + data / text / tooltip for stimulus category items
         self.cmb_stim_items = [
             ("<span>Stimulus category.</span>"),
             ("none", "None", "<span>Only noise and DC can be selected.</span>"),
             ("impulse", "Impulse", "<span>Different impulses</span>"),
             ("step", "Step", "<span>Calculate step response and its error.</span>"),
             ("sinusoid", "Sinusoid", "<span>Sinusoidal waveforms</span>"),
             ("chirp", "Chirp", "<span>Different frequency sweeps.</span>"),
             ("periodic", "Periodic", "<span>Periodic functions with discontinuities, "
              "either band-limited or with aliasing.</span>"),
             ("modulation", "Modulat.", "<span>Modulated waveforms.</span>"),
             ("formula", "Formula", "<span>Formula defined stimulus.</span>")
-            ]
+        ]
 
         # combobox tooltip + data / text / tooltip for file I/O usage
         self.cmb_file_io_items = [
-            ("<span>Select data from File I/O widget/span>"),
-            ("off", "Off", "<span>Don't use file I/O data.</span>"),
+            ("<span>Select data from File I/O widget</span>"),
             ("use", "Use", "<span><b>Use</b> file I/O data as stimuli.</span>"),
             ("add", "Add", "<span><b>Add</b> file I/O data to other stimuli</span>")
-            ]
+        ]
 
         # combobox tooltip + data / text / tooltip for periodic signals items
         self.cmb_stim_periodic_items = [
             "<span>Periodic functions with discontinuities.</span>",
             ("square", "Square", "<span>Square signal with duty cycle &alpha;</span>"),
             ("saw", "Saw", "Sawtooth signal"),
             ("triang", "Triang", "Triangular signal"),
             ("comb", "Comb", "Comb signal")
-            ]
+        ]
 
         # combobox tooltip + data / text / tooltip for chirp signals items
         self.cmb_stim_chirp_items = [
             "<span>Type of frequency sweep from <i>f</i><sub>1</sub> @ <i>t</i> = 0 to "
             "<i>f</i><sub>2</sub> @ t = <i>T</i><sub>2</sub>.</span>",
             ("linear", "Lin", "Linear frequency sweep"),
             ("quadratic", "Square", "Quadratic frequency sweep"),
             ("logarithmic", "Log", "Logarithmic frequency sweep"),
             ("hyperbolic", "Hyper",  "Hyperbolic frequency sweep")
-            ]
+        ]
 
         self.cmb_stim_impulse_items = [
             "<span>Different aperiodic impulse forms</span>",
             ("dirac", "Dirac",
              "<span>Discrete-time dirac impulse for simulating impulse and "
              "frequency response.</span>"),
             ("gauss", "Gauss",
              "<span>Gaussian pulse with bandpass spectrum and controllable "
              "relative -6 dB bandwidth.</span>"),
             ("sinc", "Sinc",
              "<span>Sinc pulse with rectangular baseband spectrum</span>"),
             ("rect", "Rect", "<span>Rectangular pulse with sinc-shaped spectrum</span>")
-            ]
+        ]
 
         self.cmb_stim_sinusoid_items = [
             "Sinusoidal or similar signals",
             ("sine", "Sine", "Sine signal"),
             ("cos", "Cos", "Cosine signal"),
             ("exp", "Exp", "Complex exponential"),
-            ("diric", "Sinc", "<span>Periodic Sinc (Dirichlet function)</span>")
-            ]
+            ("diric", "Diric", "<span>Periodic sinc (Dirichlet) function, "
+             "diric(x, N) = sin(Nx/2) / N*sin(x/2)</span>")
+        ]
 
         self.cmb_stim_modulation_items = [
             "Modulated signals",
             ("am", "AM", "<span>Sinusoidal amplitude modulation of a sine</span>"),
             ("pmfm", "PM / FM", "<span>Sinusoidal phase or frequency modulation "
              "of a sine</span>"),
             ("pwm", "PWM", "sinusoidal pulse width modulation")
-            ]
+        ]
 
         # data / text / tooltip for noise stimulus combobox.
         self.cmb_stim_noise_items = [
             "Type of additive noise.",
             ("none", "None", ""),
             ("gauss", "Gauss",
              "<span>Normal- or Gauss-distributed process with std. deviation &sigma;."
@@ -212,37 +214,42 @@
              "<span>Random integer sequence in the interval [0, <i>I</i>]</span>"),
             ("mls", "MLS",
              "<span>Maximum Length Sequence with amplitude <i>A</i> and maximum length "
              "2<sup><i>b</i></sup> - 1 after which the sequence is repeated.</span>"),
             ("brownian", "Brownian",
              "<span>Brownian (cumulated sum) process based on Gaussian noise with"
              " std. deviation &sigma;.</span>")
-            ]
+        ]
+
+        # Dict with objectNames as keys and tuples with normalized variables
+        # and scaling factors as values, e.g. {'led_f1': (self.f1, self.f_scale)}
+        self.dict_filtered_widgets = {
+            'led_f1': ('f1', 'f_scale'),
+            'led_f2': ('f2', 'f_scale'),
+            'led_T1': ('T1', 't_scale'),
+            'led_T2': ('T2', 't_scale'),
+            'led_TW1': ('TW1', 't_scale'),
+            'led_TW2': ('TW2', 't_scale')
+        }
 
         self._construct_UI()
         self._enable_stim_widgets()
         self._update_noi()
 
     def _construct_UI(self):
         # =====================================================================
         # Controls for stimuli
         # =====================================================================
-        self.lbl_file_io = QLabel(to_html("&nbsp;File IO", frmt='bi'))
-        self.cmb_file_io = QComboBox(self)
-        qcmb_box_populate(
-            self.cmb_file_io, self.cmb_file_io_items, self.cmb_file_io_default)
-        self.cmb_file_io.setEnabled(False)
-        layV_stim_io = QVBoxLayout()
-        layV_stim_io.setContentsMargins(0, 0, 0, 0)
-        layV_stim_io.addWidget(self.lbl_file_io)
-        layV_stim_io.addWidget(self.cmb_file_io)
-        # -------------------------------------
-        line1 = QVLine()
+
+        self.lbl_title_stim = QLabel("Stim:")
+        self.lbl_title_stim.setObjectName("large")
+        #
         self.cmbStimulus = QComboBox(self)
-        qcmb_box_populate(self.cmbStimulus, self.cmb_stim_items, self.cmb_stim_item)
+        qcmb_box_populate(self.cmbStimulus,
+                          self.cmb_stim_items, self.cmb_stim_item)
 
         self.lblStimPar1 = QLabel(to_html("&alpha; =", frmt='b'), self)
         self.ledStimPar1 = QLineEdit(self)
         self.ledStimPar1.setText("0.5")
         self.ledStimPar1.setToolTip("Duty Cycle, 0 ... 1")
         self.ledStimPar1.setObjectName("ledStimPar1")
 
@@ -255,15 +262,16 @@
         self.but_stim_bl.setMaximumWidth(qtext_width(text="BL "))
         self.but_stim_bl.setCheckable(True)
         self.but_stim_bl.setChecked(True)
         self.but_stim_bl.setObjectName("stim_bl")
 
         # -------------------------------------
         self.cmbChirpType = QComboBox(self)
-        qcmb_box_populate(self.cmbChirpType, self.cmb_stim_chirp_items, self.chirp_type)
+        qcmb_box_populate(self.cmbChirpType,
+                          self.cmb_stim_chirp_items, self.chirp_type)
 
         self.cmbImpulseType = QComboBox(self)
         qcmb_box_populate(
             self.cmbImpulseType, self.cmb_stim_impulse_items, self.impulse_type)
 
         self.cmbSinusoidType = QComboBox(self)
         qcmb_box_populate(
@@ -276,19 +284,37 @@
         self.cmbModulationType = QComboBox(self)
         qcmb_box_populate(
             self.cmbModulationType, self.cmb_stim_modulation_items,
             self.cmb_stim_modulation_item)
 
         # -------------------------------------
         self.chk_step_err = QPushButton("Error", self)
-        self.chk_step_err.setToolTip("<span>Display the step response error.</span>")
+        self.chk_step_err.setToolTip(
+            "<span>Display the step response error.</span>")
         self.chk_step_err.setMaximumWidth(qtext_width(text="Error "))
         self.chk_step_err.setCheckable(True)
         self.chk_step_err.setChecked(False)
         self.chk_step_err.setObjectName("stim_step_err")
+        #
+        self.but_file_io = PushButton("<", checkable=False)
+        self.but_file_io.setToolTip(
+            "<span>Use file length as number of data points.</span>")
+        self.lbl_file_io = QLabel(to_html("&nbsp;File IO", frmt='bi'))
+        self.cmb_file_io = QComboBox(self)
+        self.cmb_file_io.setObjectName("cmb_file_io")
+        qcmb_box_populate(
+            self.cmb_file_io, self.cmb_file_io_items, self.cmb_file_io_default)
+
+        # TODO: layH_file_io is instantiated in plot_impz, this is very hacky
+        self.layH_file_io = QHBoxLayout()
+        self.layH_file_io.addWidget(self.but_file_io)
+        self.layH_file_io.addWidget(self.lbl_file_io)
+        self.layH_file_io.addWidget(self.cmb_file_io)
+        self.layH_file_io.setContentsMargins(0, 0, 0, 0)
+        # -------------------------------------
 
         layHCmbStim = QHBoxLayout()
         layHCmbStim.addWidget(self.cmbStimulus)
         layHCmbStim.addWidget(self.cmbImpulseType)
         layHCmbStim.addWidget(self.cmbSinusoidType)
         layHCmbStim.addWidget(self.cmbChirpType)
         layHCmbStim.addWidget(self.cmbPeriodicType)
@@ -322,251 +348,299 @@
         self.ledAmp2.setToolTip(
             "Stimulus amplitude 2, complex values like 3j - 1 are allowed")
         self.ledAmp2.setObjectName("stimAmp2")
         # ----------------------------------------------
         self.lblPhi1 = QLabel(to_html("&nbsp;&phi;_1", frmt='bi') + " =", self)
         self.ledPhi1 = QLineEdit(self)
         self.ledPhi1.setText(str(self.phi1))
-        self.ledPhi1.setToolTip("Stimulus phase")
+        self.ledPhi1.setToolTip("Stimulus phase 1 in degrees")
         self.ledPhi1.setObjectName("stimPhi1")
-        self.lblPhU1 = QLabel(to_html("&deg;", frmt='b'), self)
+        self.lblPhU1 = QLabel(to_html("&deg;", frmt='i'), self)
 
         self.lblPhi2 = QLabel(to_html("&nbsp;&phi;_2", frmt='bi') + " =", self)
         self.ledPhi2 = QLineEdit(self)
         self.ledPhi2.setText(str(self.phi2))
-        self.ledPhi2.setToolTip("Stimulus phase 2")
+        self.ledPhi2.setToolTip("Stimulus phase 2 in degrees")
         self.ledPhi2.setObjectName("stimPhi2")
-        self.lblPhU2 = QLabel(to_html("&deg;", frmt='b'), self)
+        self.lblPhU2 = QLabel(to_html("&deg;", frmt='i'), self)
         # ----------------------------------------------
         self.lbl_T1 = QLabel(to_html("&nbsp;T_1", frmt='bi') + " =", self)
         self.led_T1 = QLineEdit(self)
         self.led_T1.setText(str(self.T1))
-        self.led_T1.setToolTip("Time shift")
-        self.led_T1.setObjectName("stimT1")
-        self.lbl_TU1 = QLabel(to_html("T_S", frmt='b'), self)
+        self.led_T1.setToolTip("Time shift 1")
+        self.led_T1.setObjectName("led_T1")
+        self.lbl_TU1 = QLabel(to_html("T_S", frmt='i'), self)
 
         self.lbl_T2 = QLabel(to_html("&nbsp;T_2", frmt='bi') + " =", self)
         self.led_T2 = QLineEdit(self)
         self.led_T2.setText(str(self.T2))
         self.led_T2.setToolTip("Time shift 2")
-        self.led_T2.setObjectName("stimT2")
-        self.lbl_TU2 = QLabel(to_html("T_S", frmt='b'), self)
+        self.led_T2.setObjectName("led_T2")
+        self.lbl_TU2 = QLabel(to_html("T_S", frmt='i'), self)
+
+        # ----------------------------------------------
+        self.lbl_N1 = QLabel(to_html("&nbsp;N_1", frmt='bi') + " =", self)
+        self.led_N1 = QLineEdit(self)
+        self.led_N1.setText(str(self.N1))
+        self.led_N1.setToolTip("Parameter N1")
+        self.led_N1.setObjectName("stimN1")
+
+        self.lbl_N2 = QLabel(to_html("&nbsp;N_2", frmt='bi') + " =", self)
+        self.led_N2 = QLineEdit(self)
+        self.led_N2.setText(str(self.N2))
+        self.led_N2.setToolTip("Parameter N2")
+        self.led_N2.setObjectName("stimN2")
         # ---------------------------------------------
-        self.lbl_TW1 = QLabel(to_html("&nbsp;&Delta;T_1", frmt='bi') + " =", self)
+        self.lbl_TW1 = QLabel(
+            to_html("&nbsp;&Delta;T_1", frmt='bi') + " =", self)
         self.led_TW1 = QLineEdit(self)
         self.led_TW1.setText(str(self.TW1))
         self.led_TW1.setToolTip("Time width")
-        self.led_TW1.setObjectName("stimTW1")
-        self.lbl_TWU1 = QLabel(to_html("T_S", frmt='b'), self)
+        self.led_TW1.setObjectName("led_TW1")
+        self.lbl_TWU1 = QLabel(to_html("T_S", frmt='i'), self)
 
-        self.lbl_TW2 = QLabel(to_html("&nbsp;&Delta;T_2", frmt='bi') + " =", self)
+        self.lbl_TW2 = QLabel(
+            to_html("&nbsp;&Delta;T_2", frmt='bi') + " =", self)
         self.led_TW2 = QLineEdit(self)
         self.led_TW2.setText(str(self.TW2))
         self.led_TW2.setToolTip("Time width 2")
-        self.led_TW2.setObjectName("stimTW2")
-        self.lbl_TWU2 = QLabel(to_html("T_S", frmt='b'), self)
+        self.led_TW2.setObjectName("led_TW2")
+        self.lbl_TWU2 = QLabel(to_html("T_S", frmt='i'), self)
         # ----------------------------------------------
         self.txtFreq1_f = to_html("&nbsp;f_1", frmt='bi') + " ="
         self.txtFreq1_k = to_html("&nbsp;k_1", frmt='bi') + " ="
         self.lblFreq1 = QLabel(self.txtFreq1_f, self)
-        self.ledFreq1 = QLineEdit(self)
-        self.ledFreq1.setText(str(self.f1))
-        self.ledFreq1.setToolTip("Stimulus frequency")
-        self.ledFreq1.setObjectName("stimFreq1")
+        self.led_f1 = QLineEdit(self)
+        self.led_f1.setText(str(self.f1))
+        self.led_f1.setToolTip("Stimulus frequency")
+        self.led_f1.setObjectName("led_f1")
         self.lblFreqUnit1 = QLabel(to_html("f_S", frmt='i'), self)
 
         self.txtFreq2_f = to_html("&nbsp;f_2", frmt='bi') + " ="
         self.txtFreq2_k = to_html("&nbsp;k_2", frmt='bi') + " ="
         self.lblFreq2 = QLabel(self.txtFreq2_f, self)
-        self.ledFreq2 = QLineEdit(self)
-        self.ledFreq2.setText(str(self.f2))
-        self.ledFreq2.setToolTip("Stimulus frequency 2")
-        self.ledFreq2.setObjectName("stimFreq2")
+        self.led_f2 = QLineEdit(self)
+        self.led_f2.setText(str(self.f2))
+        self.led_f2.setToolTip("Stimulus frequency 2")
+        self.led_f2.setObjectName("led_f2")
         self.lblFreqUnit2 = QLabel(to_html("f_S", frmt='i'), self)
         # ----------------------------------------------
-        self.lbl_BW1 = QLabel(to_html(self.tr("&nbsp;BW_1"), frmt='bi') + " =", self)
+        self.lbl_BW1 = QLabel(
+            to_html(self.tr("&nbsp;BW_1"), frmt='bi') + " =", self)
         self.led_BW1 = QLineEdit(self)
         self.led_BW1.setText(str(self.BW1))
         self.led_BW1.setToolTip(self.tr("Relative bandwidth"))
         self.led_BW1.setObjectName("stimBW1")
 
-        self.lbl_BW2 = QLabel(to_html(self.tr("&nbsp;BW_2"), frmt='bi') + " =", self)
+        self.lbl_BW2 = QLabel(
+            to_html(self.tr("&nbsp;BW_2"), frmt='bi') + " =", self)
         self.led_BW2 = QLineEdit(self)
         self.led_BW2.setText(str(self.BW2))
         self.led_BW2.setToolTip(self.tr("Relative bandwidth 2"))
         self.led_BW2.setObjectName("stimBW2")
         # ----------------------------------------------
         self.lblNoise = QLabel(to_html("&nbsp;Noise", frmt='bi'), self)
-        self.cmbNoise = QComboBox(self)
-        qcmb_box_populate(self.cmbNoise, self.cmb_stim_noise_items, self.noise)
+        self.cmb_stim_noise = QComboBox(self)
+        qcmb_box_populate(self.cmb_stim_noise, self.cmb_stim_noise_items, self.noise)
 
         line2 = QVLine()
         self.lblNoi = QLabel("not initialized", self)
         self.ledNoi = QLineEdit(self)
-        self.ledNoi.setMaximumWidth(self.cmbNoise.width())
+        self.ledNoi.setMaximumWidth(self.cmb_stim_noise.width())
         self.ledNoi.setText(str(self.noi))
         self.ledNoi.setToolTip("not initialized")
         self.ledNoi.setObjectName("stimNoi")
         self.lblNoi_par = QLabel("not initialized", self)
         self.ledNoi_par = QLineEdit(self)
         self.ledNoi_par.setMaximumWidth(qtext_width(N_x=4))
         layH_noi_params = QHBoxLayout()
         layH_noi_params.addWidget(self.ledNoi)
         layH_noi_params.addWidget(self.lblNoi_par)
         layH_noi_params.addWidget(self.ledNoi_par)
 
-        layGStim = QGridLayout()
-        layGStim.setContentsMargins(0, 0, 0, 0)
+        # ----------------------------------------------
+        # Widget and Layout containing formula editor
+        self.lblStimFormula = QLabel(to_html("x =", frmt='bi'), self)
+        self.ledStimFormula = QLineEdit(self)
+        self.ledStimFormula.setText(str(self.stim_formula))
+        self.ledStimFormula.setToolTip(
+            "<span>Enter formula for stimulus in numexpr syntax, using the index "
+            "<i>n</i> or the time vector <i>t</i> and the following UI settings: "
+            + to_html("A_1, A_2, phi_1, phi_2, f_1, f_2, T_1, T_2, BW_1, BW_2",
+                      frmt='i') + ".</span>")
+        self.ledStimFormula.setObjectName("stimFormula")
+
+        layH_formula_stim = QHBoxLayout()
+        layH_formula_stim.addWidget(self.lblStimFormula)
+        layH_formula_stim.addWidget(self.ledStimFormula)
+        layH_formula_stim.setContentsMargins(0, 0, 0, 0)
+        self.wdg_formula_stim = QWidget(self)
+        self.wdg_formula_stim.setLayout(layH_formula_stim)
+        self.wdg_formula_stim.setContentsMargins(0, 0, 0, 0)
+
+        # Main grid layout for all control elements
+        layG_ctrl_stim = QGridLayout()
         i = 0
-        layGStim.addWidget(line1, 0, i, 2, 1)  # fromRow, fromCol, rowSpan, colSpan
+        layG_ctrl_stim.addLayout(layHCmbStim, 0, i)
+        layG_ctrl_stim.addLayout(layHStimDC, 1, i)
         i += 1
-        layGStim.addLayout(layHCmbStim, 0, i)
-        layGStim.addLayout(layHStimDC, 1, i)
+        layG_ctrl_stim.addWidget(self.lblAmp1, 0, i)
+        layG_ctrl_stim.addWidget(self.lblAmp2, 1, i)
         i += 1
-        layGStim.addWidget(self.lblAmp1, 0, i)
-        layGStim.addWidget(self.lblAmp2, 1, i)
+        layG_ctrl_stim.addWidget(self.ledAmp1, 0, i)
+        layG_ctrl_stim.addWidget(self.ledAmp2, 1, i)
         i += 1
-        layGStim.addWidget(self.ledAmp1, 0, i)
-        layGStim.addWidget(self.ledAmp2, 1, i)
+        layG_ctrl_stim.addWidget(self.lblPhi1, 0, i)
+        layG_ctrl_stim.addWidget(self.lblPhi2, 1, i)
         i += 1
-        layGStim.addWidget(self.lblPhi1, 0, i)
-        layGStim.addWidget(self.lblPhi2, 1, i)
+        layG_ctrl_stim.addWidget(self.ledPhi1, 0, i)
+        layG_ctrl_stim.addWidget(self.ledPhi2, 1, i)
         i += 1
-        layGStim.addWidget(self.ledPhi1, 0, i)
-        layGStim.addWidget(self.ledPhi2, 1, i)
+        layG_ctrl_stim.addWidget(self.lblPhU1, 0, i)
+        layG_ctrl_stim.addWidget(self.lblPhU2, 1, i)
         i += 1
-        layGStim.addWidget(self.lblPhU1, 0, i)
-        layGStim.addWidget(self.lblPhU2, 1, i)
+        layG_ctrl_stim.addWidget(self.lbl_T1, 0, i)
+        layG_ctrl_stim.addWidget(self.lbl_T2, 1, i)
         i += 1
-        layGStim.addWidget(self.lbl_T1, 0, i)
-        layGStim.addWidget(self.lbl_T2, 1, i)
+        layG_ctrl_stim.addWidget(self.led_T1, 0, i)
+        layG_ctrl_stim.addWidget(self.led_T2, 1, i)
         i += 1
-        layGStim.addWidget(self.led_T1, 0, i)
-        layGStim.addWidget(self.led_T2, 1, i)
+        layG_ctrl_stim.addWidget(self.lbl_TU1, 0, i)
+        layG_ctrl_stim.addWidget(self.lbl_TU2, 1, i)
         i += 1
-        layGStim.addWidget(self.lbl_TU1, 0, i)
-        layGStim.addWidget(self.lbl_TU2, 1, i)
+        layG_ctrl_stim.addWidget(self.lbl_N1, 0, i)
+        layG_ctrl_stim.addWidget(self.lbl_N2, 1, i)
         i += 1
-        layGStim.addWidget(self.lbl_TW1, 0, i)
-        layGStim.addWidget(self.lbl_TW2, 1, i)
+        layG_ctrl_stim.addWidget(self.led_N1, 0, i)
+        layG_ctrl_stim.addWidget(self.led_N2, 1, i)
         i += 1
-        layGStim.addWidget(self.led_TW1, 0, i)
-        layGStim.addWidget(self.led_TW2, 1, i)
+        layG_ctrl_stim.addWidget(self.lbl_TW1, 0, i)
+        layG_ctrl_stim.addWidget(self.lbl_TW2, 1, i)
         i += 1
-        layGStim.addWidget(self.lbl_TWU1, 0, i)
-        layGStim.addWidget(self.lbl_TWU2, 1, i)
+        layG_ctrl_stim.addWidget(self.led_TW1, 0, i)
+        layG_ctrl_stim.addWidget(self.led_TW2, 1, i)
         i += 1
-        layGStim.addWidget(self.lblFreq1, 0, i)
-        layGStim.addWidget(self.lblFreq2, 1, i)
+        layG_ctrl_stim.addWidget(self.lbl_TWU1, 0, i)
+        layG_ctrl_stim.addWidget(self.lbl_TWU2, 1, i)
         i += 1
-        layGStim.addWidget(self.ledFreq1, 0, i)
-        layGStim.addWidget(self.ledFreq2, 1, i)
+        layG_ctrl_stim.addWidget(self.lblFreq1, 0, i)
+        layG_ctrl_stim.addWidget(self.lblFreq2, 1, i)
         i += 1
-        layGStim.addWidget(self.lblFreqUnit1, 0, i)
-        layGStim.addWidget(self.lblFreqUnit2, 1, i)
+        layG_ctrl_stim.addWidget(self.led_f1, 0, i)
+        layG_ctrl_stim.addWidget(self.led_f2, 1, i)
         i += 1
-        layGStim.addWidget(self.lbl_BW1, 0, i)
-        layGStim.addWidget(self.lbl_BW2, 1, i)
+        layG_ctrl_stim.addWidget(self.lblFreqUnit1, 0, i)
+        layG_ctrl_stim.addWidget(self.lblFreqUnit2, 1, i)
         i += 1
-        layGStim.addWidget(self.led_BW1, 0, i)
-        layGStim.addWidget(self.led_BW2, 1, i)
+        layG_ctrl_stim.addWidget(self.lbl_BW1, 0, i)
+        layG_ctrl_stim.addWidget(self.lbl_BW2, 1, i)
         i += 1
-        layGStim.addWidget(line2, 0, i, 2, 1)
+        layG_ctrl_stim.addWidget(self.led_BW1, 0, i)
+        layG_ctrl_stim.addWidget(self.led_BW2, 1, i)
         i += 1
-        layGStim.addWidget(self.lblNoise, 0, i)
-        layGStim.addWidget(self.lblNoi, 1, i)
+        layG_ctrl_stim.addWidget(line2, 0, i, 2, 1)
         i += 1
-        layGStim.addWidget(self.cmbNoise, 0, i)
-        layGStim.addLayout(layH_noi_params, 1, i)
-
-        self.frmGStim = QFrame(self)
-        self.frmGStim.setContentsMargins(0, 0, 0, 0)
-        self.frmGStim.setLayout(layGStim)
-
-        # ----------------------------------------------
-        self.lblStimFormula = QLabel(to_html("x =", frmt='bi'), self)
-        self.ledStimFormula = QLineEdit(self)
-        self.ledStimFormula.setText(str(self.stim_formula))
-        self.ledStimFormula.setToolTip(
-            "<span>Enter formula for stimulus in numexpr syntax.</span>")
-        self.ledStimFormula.setObjectName("stimFormula")
-
-        layH_stim_formula = QHBoxLayout()
-        layH_stim_formula.addWidget(self.lblStimFormula)
-        layH_stim_formula.addWidget(self.ledStimFormula, 10)
+        layG_ctrl_stim.addWidget(self.lblNoise, 0, i)
+        layG_ctrl_stim.addWidget(self.lblNoi, 1, i)
+        i += 1
+        layG_ctrl_stim.addWidget(self.cmb_stim_noise, 0, i)
+        layG_ctrl_stim.addLayout(layH_noi_params, 1, i)
+        i += 1
+        layG_ctrl_stim.setColumnStretch(i, 1)
+        i += 1
+        # place formula widget in row 2, stretching over i columns
+        layG_ctrl_stim.addWidget(self.wdg_formula_stim, 2, 0, 1, i)
 
         # ----------------------------------------------------------------------
         # Main Widget
         # ----------------------------------------------------------------------
-        layH_stim_par = QHBoxLayout()
-        layH_stim_par.addLayout(layV_stim_io)
-        layH_stim_par.addWidget(self.frmGStim)
-
-        layV_stim = QVBoxLayout()
-        layV_stim.addLayout(layH_stim_par)
-        layV_stim.addLayout(layH_stim_formula)
+
+        # Widget with the text block "Stim:"
+        layH_title_stim = QHBoxLayout()
+        layH_title_stim.addWidget(self.lbl_title_stim)
+        self.wdg_title_stim = QWidget(self)
+        self.wdg_title_stim.setLayout(layH_title_stim)
+        self.wdg_title_stim.setContentsMargins(0, 0, 0, 0)
+
+        # Widget containing all control elements for stimuli
+        self.wdg_ctrl_stim = QWidget(self)
+        self.wdg_ctrl_stim.setLayout(layG_ctrl_stim)
 
         layH_stim = QHBoxLayout()
-        layH_stim.addLayout(layV_stim)
-        layH_stim.addStretch(10)
+        layH_stim.addWidget(self.wdg_title_stim)
+        layH_stim.addWidget(self.wdg_ctrl_stim)
+        layH_stim.setContentsMargins(0, 0, 0, 0)
 
         self.wdg_stim = QWidget(self)
+        self.wdg_stim.setObjectName("transparent")
         self.wdg_stim.setLayout(layH_stim)
-        self.wdg_stim.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.wdg_stim.setContentsMargins(0, 0, 0, 0)
 
         # ----------------------------------------------------------------------
-        # Event Filter
+        # Initialization
         # ----------------------------------------------------------------------
-        # frequency related widgets are scaled with f_s, requiring special handling
-        self.ledFreq1.installEventFilter(self)
-        self.ledFreq2.installEventFilter(self)
-        self.led_T1.installEventFilter(self)
-        self.led_T2.installEventFilter(self)
-        self.led_TW1.installEventFilter(self)
-        self.led_TW2.installEventFilter(self)
+        self.normalize_freqs()  # set f_scale and t_scale factors
 
         # ----------------------------------------------------------------------
         # GLOBAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         self.sig_rx.connect(self.process_sig_rx)
         # ----------------------------------------------------------------------
         # LOCAL SIGNALS & SLOTs
         # ----------------------------------------------------------------------
         # --- stimulus control ---
         self.but_stim_bl.clicked.connect(self._enable_stim_widgets)
         self.chk_step_err.clicked.connect(self._enable_stim_widgets)
         self.cmbStimulus.currentIndexChanged.connect(self._enable_stim_widgets)
 
-        self.cmbNoise.currentIndexChanged.connect(self._update_noi)
+        self.cmb_stim_noise.currentIndexChanged.connect(self._update_noi)
         self.ledNoi.editingFinished.connect(self._update_noi)
         self.ledNoi_par.editingFinished.connect(self._update_noi)
         self.ledAmp1.editingFinished.connect(self._update_amp1)
         self.ledAmp2.editingFinished.connect(self._update_amp2)
         self.ledPhi1.editingFinished.connect(self._update_phi1)
         self.ledPhi2.editingFinished.connect(self._update_phi2)
         self.led_BW1.editingFinished.connect(self._update_BW1)
         self.led_BW2.editingFinished.connect(self._update_BW2)
+        self.led_N1.editingFinished.connect(self._update_N1)
+        self.led_N2.editingFinished.connect(self._update_N2)
 
         self.cmb_file_io.currentIndexChanged.connect(self._enable_stim_widgets)
-        self.cmbImpulseType.currentIndexChanged.connect(self._update_impulse_type)
-        self.cmbSinusoidType.currentIndexChanged.connect(self._update_sinusoid_type)
+        self.cmbImpulseType.currentIndexChanged.connect(
+            self._update_impulse_type)
+        self.cmbSinusoidType.currentIndexChanged.connect(
+            self._update_sinusoid_type)
         self.cmbChirpType.currentIndexChanged.connect(self._update_chirp_type)
-        self.cmbPeriodicType.currentIndexChanged.connect(self._update_periodic_type)
-        self.cmbModulationType.currentIndexChanged.connect(self._update_modulation_type)
+        self.cmbPeriodicType.currentIndexChanged.connect(
+            self._update_periodic_type)
+        self.cmbModulationType.currentIndexChanged.connect(
+            self._update_modulation_type)
 
         self.ledDC.editingFinished.connect(self._update_DC)
         self.ledStimFormula.editingFinished.connect(self._update_stim_formula)
         self.ledStimPar1.editingFinished.connect(self._update_stim_par1)
 
+        # ----------------------------------------------------------------------
+        # Event Filter
+        # ----------------------------------------------------------------------
+        # time / frequency related widgets have to be scaled with f_s, this
+        # special handling is performed in an EventFilter (hence no regular
+        # signal-slot connection).
+        self.led_f1.installEventFilter(self)
+        self.led_f2.installEventFilter(self)
+        self.led_T1.installEventFilter(self)
+        self.led_T2.installEventFilter(self)
+        self.led_TW1.installEventFilter(self)
+        self.led_TW2.installEventFilter(self)
+
 # ------------------------------------------------------------------------------
     def update_freq_units(self):
         """
-        Update labels referrring to frequency specs
+        Update labels for time / frequency related specs
         """
-
         if fb.fil[0]['freq_specs_unit'] == 'k':
             f_unit = ''
             t_unit = ''
             self.lblFreq1.setText(self.txtFreq1_k)
             self.lblFreq2.setText(self.txtFreq2_k)
         else:
             f_unit = fb.fil[0]['plt_fUnit']
@@ -583,97 +657,80 @@
         self.lblFreqUnit2.setText(to_html(f_unit, frmt=unit_frmt))
         self.lbl_TU1.setText(to_html(t_unit, frmt=unit_frmt))
         self.lbl_TU2.setText(to_html(t_unit, frmt=unit_frmt))
 
 # ------------------------------------------------------------------------------
     def eventFilter(self, source, event):
         """
-        Filter all events generated by the monitored widgets (ledFreq1 and 2 and T1 / T2).
+        Filter all events generated by the monitored frequency / time related widgets
+        led_f1 and 2, T1 / T2 and TW1 / TW2.
         Source and type of all events generated by monitored objects are passed
          to this eventFilter, evaluated and passed on to the next hierarchy level.
 
         - When a QLineEdit widget gains input focus (``QEvent.FocusIn``), display
           the stored value from filter dict with full precision
         - When a key is pressed inside the text field, set the `spec_edited` flag
           to True.
-        - When a QLineEdit widget loses input focus (``QEvent.FocusOut``), store
-          current value normalized to f_S with full precision (only if
-          ``spec_edited == True``) and display the stored value in selected format
-
-          Emit 'ui_local_changed':'stim'
-        """
-        def _reload_entry(source):
-            """ Reload text entry for active line edit field in rounded format """
-            if source.objectName() == "stimFreq1":
-                source.setText(str(params['FMT'].format(self.f1 * self.f_scale)))
-            elif source.objectName() == "stimFreq2":
-                source.setText(str(params['FMT'].format(self.f2 * self.f_scale)))
-            elif source.objectName() == "stimT1":
-                source.setText(str(params['FMT'].format(self.T1 * self.t_scale)))
-            elif source.objectName() == "stimT2":
-                source.setText(str(params['FMT'].format(self.T2 * self.t_scale)))
-            elif source.objectName() == "stimTW1":
-                source.setText(str(params['FMT'].format(self.TW1 * self.t_scale)))
-            elif source.objectName() == "stimTW2":
-                source.setText(str(params['FMT'].format(self.TW2 * self.t_scale)))
+        - When a QLineEdit widget loses input focus (``QEvent.FocusOut``) or when
+          the Return key is pressed, store current value normalized to f_S with
+          full precision and display the denormalized value in selected format
+          or full precision when `spec_edited == True`. Emit 'ui_local_changed':'stim'.
+        """
+        def _reload_entry(source, full_prec=False):
+            """
+            Reload text entry for active line edit field in denormalized format,
+            either with full precision (`full_prec == True`) or rounded.
+            """
+            try:
+                var_name, param_name = self.dict_filtered_widgets[source.objectName()]
+                var = getattr(self, var_name)
+                scale = getattr(self, param_name)
+                if full_prec:
+                    source.setText(str(var * scale))
+                else:
+                    source.setText(str(params['FMT'].format(var * scale)))
+            except KeyError:
+                logger.warning(f"Unknown objectName {source.objectName}!")
+        #------------------------------------------------------------
 
         def _store_entry(source):
             """ Store transformed frequency / time values """
             if self.spec_edited:
-                if source.objectName() == "stimFreq1":
-                    self.f1 = safe_eval(
-                       source.text(), self.f1 * self.f_scale,
-                       return_type='float') / self.f_scale
-                    source.setText(str(params['FMT'].format(self.f1 * self.f_scale)))
-
-                elif source.objectName() == "stimFreq2":
-                    self.f2 = safe_eval(
-                        source.text(), self.f2 * self.f_scale,
-                        return_type='float') / self.f_scale
-                    source.setText(str(params['FMT'].format(self.f2 * self.f_scale)))
-
-                elif source.objectName() == "stimT1":
-                    self.T1 = safe_eval(
-                        source.text(), self.T1 * self.t_scale,
-                        return_type='float') / self.t_scale
-                    source.setText(str(params['FMT'].format(self.T1 * self.t_scale)))
-
-                elif source.objectName() == "stimT2":
-                    self.T2 = safe_eval(
-                        source.text(), self.T2 * self.t_scale,
-                        return_type='float') / self.t_scale
-                    source.setText(str(params['FMT'].format(self.T2 * self.t_scale)))
-
-                elif source.objectName() == "stimTW1":
-                    self.TW1 = safe_eval(
-                        source.text(), self.TW1 * self.t_scale, sign='pos',
-                        return_type='float') / self.t_scale
-                    source.setText(str(params['FMT'].format(self.TW1 * self.t_scale)))
-
-                elif source.objectName() == "stimTW2":
-                    self.TW2 = safe_eval(
-                        source.text(), self.TW2 * self.t_scale, sign='pos',
-                        return_type='float') / self.t_scale
-                    source.setText(str(params['FMT'].format(self.TW2 * self.t_scale)))
+                try:
+                    var_name, param_name = self.dict_filtered_widgets[source.objectName()]
+                    scale = getattr(self, param_name)  # get scale value
+                    var_old = getattr(self, var_name)  # get old var value
+                    # assign var with either content of text field or fallback value:
+                    var = safe_eval(source.text(), var_old * scale,
+                                    sign='pos', return_type='float') / scale
+                    # assign evaluated text field to variable
+                    setattr(self, var_name, var)
+                    # set textfield with scaled value of `var_name`:
+                    source.setText(str(params['FMT'].format(var * scale)))
+                    # highlight lineedit field in red when normalized frequency is > 0.5
+                    if var >= 0.5 and "_f" in source.objectName():  # only test this for 'led_f1' and 'led_f2'
+                        qstyle_widget(source, 'failed')
+                    else:
+                        qstyle_widget(source, 'normal')
+                except KeyError:
+                    pass
 
                 self.spec_edited = False  # reset flag
-                self._update_scale_impz()
+                self._update_energy_scaling_impz()
                 self.emit({'ui_local_changed': 'stim'})
 
             # nothing has changed, but display frequencies in rounded format anyway
             else:
                 _reload_entry(source)
         # --------------------------------------------------------------------
-
-#        if isinstance(source, QLineEdit):
-#        if source.objectName() in {"stimFreq1","stimFreq2"}:
+        # ------ EventFilter main part ---------------------------------------
         if event.type() in {QEvent.FocusIn, QEvent.KeyPress, QEvent.FocusOut}:
             if event.type() == QEvent.FocusIn:
                 self.spec_edited = False
-                self.update_freqs()
+                _reload_entry(source, full_prec=True)
             elif event.type() == QEvent.KeyPress:
                 self.spec_edited = True  # entry has been changed
                 key = event.key()
                 if key in {Qt.Key_Return, Qt.Key_Enter}:
                     _store_entry(source)
                 elif key == Qt.Key_Escape:  # revert changes
                     self.spec_edited = False
@@ -682,102 +739,92 @@
             elif event.type() == QEvent.FocusOut:
                 _store_entry(source)
 
         # Call base class method to continue normal event processing:
         return super(Plot_Tran_Stim_UI, self).eventFilter(source, event)
 
     # -------------------------------------------------------------
-    def recalc_freqs(self):
-        """
-        Update normalized frequencies if required. This is called via signal
-        ['ui_global_changed':'f_S'] from plot_impz.process_sig_rx
+    def normalize_freqs(self):
         """
-        if fb.fil[0]['freq_locked']:
-            self.f1 *= fb.fil[0]['f_S_prev'] / fb.fil[0]['f_S']
-            self.f2 *= fb.fil[0]['f_S_prev'] / fb.fil[0]['f_S']
-            self.T1 *= fb.fil[0]['f_S'] / fb.fil[0]['f_S_prev']
-            self.T2 *= fb.fil[0]['f_S'] / fb.fil[0]['f_S_prev']
-            self.TW1 *= fb.fil[0]['f_S'] / fb.fil[0]['f_S_prev']
-            self.TW2 *= fb.fil[0]['f_S'] / fb.fil[0]['f_S_prev']
+        Update normalized frequencies and periods if required.
 
-        self._update_scale_impz()
+        `normalize_freqs()` is called when sampling frequency has been changed
+        via signal ['view_changed':'f_S'] from plot_impz.process_sig_rx
 
-        self.update_freqs()
+        Frequency and time related entries are always stored normalized w.r.t. f_S
+        which is loaded from filter dictionary and stored as  `self.f_scale`
+        (except when the frequency unit is k when `f_scale = self.N_FFT`).
 
-        self.emit({'ui_local_changed': 'f1_f2'})
+        - When the `f_S` lock button is unchecked, only the displayed
+          values for frequency entries are updated with f_S, not the normalized freqs.
 
-    # -------------------------------------------------------------
-    def update_freqs(self):
+        - When the `f_S` lock button is checked, the absolute frequency values in
+          the widget fields are kept constant, and the normalized freqs are updated.
         """
-        `update_freqs()` is called:
-
-        - when one of the stimulus frequencies has changed via eventFilter()
-        - sampling frequency has been changed via signal ['view_changed':'f_S']
-          from plot_impz.process_sig_rx -> self.recalc_freqs
 
-        The sampling frequency is loaded from filter dictionary and stored as
-        `self.f_scale` (except when the frequency unit is k when `f_scale = self.N_FFT`).
+        f_corr = 1
+        if fb.fil[0]['freq_locked'] and fb.fil[0]['freq_specs_unit'] != 'k':
+            f_corr = fb.fil[0]['f_S_prev'] / fb.fil[0]['f_S']
+            self.f1 *= f_corr
+            self.f2 *= f_corr
+            self.T1 /= f_corr
+            self.T2 /= f_corr
+            self.TW1 /= f_corr
+            self.TW2 /= f_corr
 
-        Frequency field entries are always stored normalized w.r.t. f_S in the
-        dictionary: When the `f_S` lock button is unlocked, only the displayed
-        values for frequency entries are updated with f_S, not the dictionary.
-
-        When the `f_S` lock button is pressed, the absolute frequency values in
-        the widget fields are kept constant, and the dictionary entries are updated.
-
-        """
+        self._update_energy_scaling_impz()
 
         # recalculate displayed freq spec values for (maybe) changed f_S
         if fb.fil[0]['freq_specs_unit'] == 'k':
             self.f_scale = self.N_FFT
         else:
             self.f_scale = fb.fil[0]['f_S']
         self.t_scale = fb.fil[0]['T_S']
 
-        if self.ledFreq1.hasFocus():
-            # widget has focus, show full precision
-            self.ledFreq1.setText(str(self.f1 * self.f_scale))
-
-        elif self.ledFreq2.hasFocus():
-            self.ledFreq2.setText(str(self.f2 * self.f_scale))
+        # logger.warning(f"f_S = {fb.fil[0]['f_S']}, prev = {fb.fil[0]['f_S_prev']}\n"
+        #                f"f_scale = {self.f_scale}, f_1 = {self.f1}, f_corr = {f_corr}")
 
-        elif self.led_T1.hasFocus():
-            self.led_T1.setText(str(self.T1 * self.t_scale))
-
-        elif self.led_T2.hasFocus():
-            self.led_T2.setText(str(self.T2 * self.t_scale))
-
-        elif self.led_TW1.hasFocus():
-            self.led_TW1.setText(str(self.TW1 * self.t_scale))
-
-        elif self.led_TW2.hasFocus():
-            self.led_TW2.setText(str(self.TW2 * self.t_scale))
+        # update and round the display
+        for w in self.dict_filtered_widgets:
+            var_name, param_name = self.dict_filtered_widgets[w]
+            # read value and scale of normalized frequency / time value
+            var = getattr(self, var_name)
+            scale = getattr(self, param_name)
+            # access lineedit object
+            led = getattr(self, w)
+            # logger.warning(f"{w} - {var} - {getattr(self, w).text()}")
+            # update the text with the denormalized frequency / time variable
+            led.setText(str(params['FMT'].format(var * scale)))
+            # self.led_f1.setText(str(params['FMT'].format(self.f1 * self.f_scale)))
+
+            # highlight lineedit field in red when normalized frequency is > 0.5
+            if var >= 0.5 and "_f" in w:  # only test this for 'led_f1' and 'led_f2'
+                qstyle_widget(led, 'failed')
+            else:
+                qstyle_widget(led, 'normal')
 
-        else:
-            # widgets have no focus, round the display
-            self.ledFreq1.setText(str(params['FMT'].format(self.f1 * self.f_scale)))
-            self.ledFreq2.setText(str(params['FMT'].format(self.f2 * self.f_scale)))
-            self.led_T1.setText(str(params['FMT'].format(self.T1 * self.t_scale)))
-            self.led_T2.setText(str(params['FMT'].format(self.T2 * self.t_scale)))
-            self.led_TW1.setText(str(params['FMT'].format(self.TW1 * self.t_scale)))
-            self.led_TW2.setText(str(params['FMT'].format(self.TW2 * self.t_scale)))
+        self.update_freq_units()
 
-        self.update_freq_units()  # TODO: should only be called at f_S / unit update
+        # emit a signal if normalized frequencies have changed due to an update
+        # of f_S
+        if fb.fil[0]['freq_locked'] and fb.fil[0]['freq_specs_unit'] != 'k':
+            self.emit({'ui_local_changed': 'f1_f2'})
 
     # -------------------------------------------------------------
     def _enable_stim_widgets(self):
         """ Enable / disable widgets depending on the selected stimulus """
-        use_file_io = qget_cmb_box(self.cmb_file_io) != "use"
-        self.frmGStim.setVisible(use_file_io)
 
         self.cmb_stim = qget_cmb_box(self.cmbStimulus)
+
+        self.wdg_formula_stim.setVisible(self.cmb_stim == "formula")
+
         if self.cmb_stim == "impulse":
             self.stim = qget_cmb_box(self.cmbImpulseType)
             # recalculate the energy scaling for impulse functions
-            self._update_scale_impz()
+            self._update_energy_scaling_impz()
 
         elif self.cmb_stim == "sinusoid":
             self.stim = qget_cmb_box(self.cmbSinusoidType)
         elif self.cmb_stim == "periodic":
             self.stim = qget_cmb_box(self.cmbPeriodicType)
         elif self.cmb_stim == "modulation":
             self.stim = qget_cmb_box(self.cmbModulationType)
@@ -801,41 +848,43 @@
         self.ledAmp1.setVisible("a1" in stim_wdg)
         self.lblPhi1.setVisible("phi1" in stim_wdg)
         self.ledPhi1.setVisible("phi1" in stim_wdg)
         self.lblPhU1.setVisible("phi1" in stim_wdg)
         self.lbl_T1.setVisible("T1" in stim_wdg)
         self.led_T1.setVisible("T1" in stim_wdg)
         self.lbl_TU1.setVisible("T1" in stim_wdg)
+        self.lbl_N1.setVisible("N1" in stim_wdg)
+        self.led_N1.setVisible("N1" in stim_wdg)
         self.lbl_TW1.setVisible("TW1" in stim_wdg)
         self.led_TW1.setVisible("TW1" in stim_wdg)
         self.lbl_TWU1.setVisible("TW1" in stim_wdg)
         self.lblFreq1.setVisible("f1" in stim_wdg)
-        self.ledFreq1.setVisible("f1" in stim_wdg)
+        self.led_f1.setVisible("f1" in stim_wdg)
         self.lblFreqUnit1.setVisible("f1" in stim_wdg)
         self.lbl_BW1.setVisible("BW1" in stim_wdg)
         self.led_BW1.setVisible("BW1" in stim_wdg)
 
         self.lblAmp2.setVisible("a2" in stim_wdg)
         self.ledAmp2.setVisible("a2" in stim_wdg)
         self.lblPhi2.setVisible("phi2" in stim_wdg)
         self.ledPhi2.setVisible("phi2" in stim_wdg)
         self.lblPhU2.setVisible("phi2" in stim_wdg)
         self.lbl_T2.setVisible("T2" in stim_wdg)
         self.led_T2.setVisible("T2" in stim_wdg)
         self.lbl_TU2.setVisible("T2" in stim_wdg)
+        self.lbl_N2.setVisible("N2" in stim_wdg)
+        self.led_N2.setVisible("N2" in stim_wdg)
         self.lbl_TW2.setVisible("TW2" in stim_wdg)
         self.led_TW2.setVisible("TW2" in stim_wdg)
         self.lbl_TWU2.setVisible("TW2" in stim_wdg)
         self.lblFreq2.setVisible("f2" in stim_wdg)
-        self.ledFreq2.setVisible("f2" in stim_wdg)
+        self.led_f2.setVisible("f2" in stim_wdg)
         self.lblFreqUnit2.setVisible("f2" in stim_wdg)
         self.lbl_BW2.setVisible("BW2" in stim_wdg)
         self.led_BW2.setVisible("BW2" in stim_wdg)
-        self.lblStimFormula.setVisible(self.stim == "formula" and use_file_io)
-        self.ledStimFormula.setVisible(self.stim == "formula" and use_file_io)
 
         self.cmbImpulseType.setVisible(self.cmb_stim == 'impulse')
         self.cmbSinusoidType.setVisible(self.cmb_stim == 'sinusoid')
         self.cmbChirpType.setVisible(self.cmb_stim == 'chirp')
         self.cmbPeriodicType.setVisible(self.cmb_stim == 'periodic')
         self.cmbModulationType.setVisible(self.cmb_stim == 'modulation')
 
@@ -852,34 +901,47 @@
         """ Update value for self.A2 from the QLineEditWidget"""
         self.A2 = safe_eval(self.ledAmp2.text(), self.A2, return_type='cmplx')
         self.ledAmp2.setText(str(self.A2))
         self.emit({'ui_local_changed': 'a2'})
 
     def _update_phi1(self):
         """ Update value for self.phi1 from QLineEditWidget"""
-        self.phi1 = safe_eval(self.ledPhi1.text(), self.phi1, return_type='float')
+        self.phi1 = safe_eval(self.ledPhi1.text(),
+                              self.phi1, return_type='float')
         self.ledPhi1.setText(str(self.phi1))
         self.emit({'ui_local_changed': 'phi1'})
 
+    def _update_N1(self):
+        """ Update value for self.N1 from `self.led_N1`"""
+        self.N1 = safe_eval(self.led_N1.text(), self.N1, return_type='int', sign='pos')
+        self.led_N1.setText(str(self.N1))
+        self.emit({'ui_local_changed': 'N1'})
+
+    def _update_N2(self):
+        """ Update value for self.N2 from `self.led_N2`"""
+        self.N2 = safe_eval(self.led_N2.text(), self.N2, return_type='int', sign='pos')
+        self.led_N2.setText(str(self.N2))
+        self.emit({'ui_local_changed': 'N2'})
+
     def _update_BW1(self):
         """ Update value for self.BW1 from QLineEditWidget"""
         self.BW1 = safe_eval(
             self.led_BW1.text(), self.BW1, return_type='float', sign='pos')
         self.led_BW1.setText(str(self.BW1))
-        self._update_scale_impz()
+        self._update_energy_scaling_impz()
         self.emit({'ui_local_changed': 'BW1'})
 
     def _update_BW2(self):
         """ Update value for self.BW2 from QLineEditWidget"""
         self.BW2 = safe_eval(
             self.led_BW2.text(), self.BW2, return_type='float', sign='pos')
         self.led_BW2.setText(str(self.BW2))
         self.emit({'ui_local_changed': 'BW2'})
 
-    def _update_scale_impz(self):
+    def _update_energy_scaling_impz(self):
         """
         recalculate the energy scaling for impulse functions when impulse type or
         relevant frequency / bandwidth parameter have been updated
         """
         if self.stim == "dirac":
             self.scale_impz = 1.
         elif self.stim == "sinc":
@@ -887,15 +949,16 @@
         elif self.stim == "gauss":
             self.scale_impz = self.f1 * 2 * self.BW1
         elif self.stim == "rect":
             self.scale_impz = 1. / self.TW1
 
     def _update_phi2(self):
         """ Update value for self.phi2 from the QLineEditWidget"""
-        self.phi2 = safe_eval(self.ledPhi2.text(), self.phi2, return_type='float')
+        self.phi2 = safe_eval(self.ledPhi2.text(),
+                              self.phi2, return_type='float')
         self.ledPhi2.setText(str(self.phi2))
         self.emit({'ui_local_changed': 'phi2'})
 
     def _update_chirp_type(self):
         """ Update value for self.chirp_type from data field of ComboBox"""
         self.chirp_type = qget_cmb_box(self.cmbChirpType)
         self.emit({'ui_local_changed': 'chirp_type'})
@@ -919,15 +982,15 @@
         """ Update value for self.modulation_type from from data field of ComboBox"""
         self.modulation_type = qget_cmb_box(self.cmbModulationType)
         self._enable_stim_widgets()
 
     # -------------------------------------------------------------
     def _update_noi(self):
         """ Update type + value + label for self.noi for noise"""
-        self.noise = qget_cmb_box(self.cmbNoise)
+        self.noise = qget_cmb_box(self.cmb_stim_noise)
         self.lblNoi.setVisible(self.noise != 'none')
         self.ledNoi.setVisible(self.noise != 'none')
         self.lblNoi_par.setVisible(self.noise == 'mls')
         self.ledNoi_par.setVisible(self.noise == 'mls')
         if self.noise != 'none':
             self.noi = safe_eval(self.ledNoi.text(), 0, return_type='cmplx')
             self.ledNoi.setText(str(self.noi))
@@ -996,15 +1059,16 @@
     from pyfda.libs.compat import QApplication
 
     app = QApplication(sys.argv)
 
     mainw = Plot_Tran_Stim_UI(None)
     layVMain = QVBoxLayout()
     layVMain.addWidget(mainw.wdg_stim)
-    layVMain.setContentsMargins(*params['wdg_margins'])  # (left, top, right, bottom)
+    # (left, top, right, bottom)
+    layVMain.setContentsMargins(*params['wdg_margins'])
 
     mainw.setLayout(layVMain)
 
     app.setActiveWindow(mainw)
     mainw.show()
     sys.exit(app.exec_())
```

### Comparing `pyfda-0.7.1/pyfda/pyfda.qrc` & `pyfda-0.8.0a2/pyfda/pyfda.qrc`

 * *Files 5% similar despite different names*

```diff
@@ -11,237 +11,248 @@
 000000a0: 6573 2f69 636f 6e73 2f64 6172 6b2f 6163  es/icons/dark/ac
 000000b0: 7469 6f6e 2d75 6e64 6f2e 7376 673c 2f66  tion-undo.svg</f
 000000c0: 696c 653e 0a20 2020 203c 6669 6c65 2061  ile>.    <file a
 000000d0: 6c69 6173 3d22 6272 7573 682e 7376 6722  lias="brush.svg"
 000000e0: 3e69 6d61 6765 732f 6963 6f6e 732f 6461  >images/icons/da
 000000f0: 726b 2f62 7275 7368 2e73 7667 3c2f 6669  rk/brush.svg</fi
 00000100: 6c65 3e0a 2020 2020 3c66 696c 6520 616c  le>.    <file al
-00000110: 6961 733d 2263 616d 6572 612d 736c 722e  ias="camera-slr.
-00000120: 7376 6722 3e69 6d61 6765 732f 6963 6f6e  svg">images/icon
-00000130: 732f 6461 726b 2f63 616d 6572 612d 736c  s/dark/camera-sl
-00000140: 722e 7376 673c 2f66 696c 653e 0a20 2020  r.svg</file>.   
-00000150: 203c 6669 6c65 2061 6c69 6173 3d22 6369   <file alias="ci
-00000160: 7263 6c65 2d63 6865 636b 2e73 7667 223e  rcle-check.svg">
+00000110: 6961 733d 2263 6972 636c 652d 6368 6563  ias="circle-chec
+00000120: 6b2e 7376 6722 3e69 6d61 6765 732f 6963  k.svg">images/ic
+00000130: 6f6e 732f 6461 726b 2f63 6972 636c 652d  ons/dark/circle-
+00000140: 6368 6563 6b2e 7376 673c 2f66 696c 653e  check.svg</file>
+00000150: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
+00000160: 3d22 6369 7263 6c65 2d78 2e73 7667 223e  ="circle-x.svg">
 00000170: 696d 6167 6573 2f69 636f 6e73 2f64 6172  images/icons/dar
-00000180: 6b2f 6369 7263 6c65 2d63 6865 636b 2e73  k/circle-check.s
-00000190: 7667 3c2f 6669 6c65 3e0a 2020 2020 3c66  vg</file>.    <f
-000001a0: 696c 6520 616c 6961 733d 2263 6972 636c  ile alias="circl
-000001b0: 652d 782e 7376 6722 3e69 6d61 6765 732f  e-x.svg">images/
-000001c0: 6963 6f6e 732f 6461 726b 2f63 6972 636c  icons/dark/circl
-000001d0: 652d 782e 7376 673c 2f66 696c 653e 2020  e-x.svg</file>  
-000001e0: 2020 0a20 2020 203c 6669 6c65 2061 6c69    .    <file ali
-000001f0: 6173 3d22 636c 6970 626f 6172 642e 7376  as="clipboard.sv
-00000200: 6722 3e69 6d61 6765 732f 6963 6f6e 732f  g">images/icons/
-00000210: 6461 726b 2f63 6c69 7062 6f61 7264 2e73  dark/clipboard.s
-00000220: 7667 3c2f 6669 6c65 3e0a 2020 2020 3c66  vg</file>.    <f
-00000230: 696c 6520 616c 6961 733d 2264 6f77 6e6c  ile alias="downl
-00000240: 6f61 642e 7376 6722 3e69 6d61 6765 732f  oad.svg">images/
-00000250: 6963 6f6e 732f 6461 726b 2f64 6174 612d  icons/dark/data-
-00000260: 7472 616e 7366 6572 2d64 6f77 6e6c 6f61  transfer-downloa
-00000270: 642e 7376 673c 2f66 696c 653e 0a20 2020  d.svg</file>.   
+00000180: 6b2f 6369 7263 6c65 2d78 2e73 7667 3c2f  k/circle-x.svg</
+00000190: 6669 6c65 3e20 2020 200a 2020 2020 3c66  file>    .    <f
+000001a0: 696c 6520 616c 6961 733d 2263 6c69 7062  ile alias="clipb
+000001b0: 6f61 7264 2e73 7667 223e 696d 6167 6573  oard.svg">images
+000001c0: 2f69 636f 6e73 2f64 6172 6b2f 636c 6970  /icons/dark/clip
+000001d0: 626f 6172 642e 7376 673c 2f66 696c 653e  board.svg</file>
+000001e0: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
+000001f0: 3d22 646f 776e 6c6f 6164 2e73 7667 223e  ="download.svg">
+00000200: 696d 6167 6573 2f69 636f 6e73 2f64 6172  images/icons/dar
+00000210: 6b2f 6461 7461 2d74 7261 6e73 6665 722d  k/data-transfer-
+00000220: 646f 776e 6c6f 6164 2e73 7667 3c2f 6669  download.svg</fi
+00000230: 6c65 3e0a 2020 2020 3c66 696c 6520 616c  le>.    <file al
+00000240: 6961 733d 2265 6c6c 6970 7365 735f 682e  ias="ellipses_h.
+00000250: 7376 6722 3e69 6d61 6765 732f 6963 6f6e  svg">images/icon
+00000260: 732f 6461 726b 2f65 6c6c 6970 7365 735f  s/dark/ellipses_
+00000270: 682e 7376 673c 2f66 696c 653e 0a20 2020  h.svg</file>.   
 00000280: 203c 6669 6c65 2061 6c69 6173 3d22 656c   <file alias="el
-00000290: 6c69 7073 6573 5f68 2e73 7667 223e 696d  lipses_h.svg">im
+00000290: 6c69 7073 6573 5f76 2e73 7667 223e 696d  lipses_v.svg">im
 000002a0: 6167 6573 2f69 636f 6e73 2f64 6172 6b2f  ages/icons/dark/
-000002b0: 656c 6c69 7073 6573 5f68 2e73 7667 3c2f  ellipses_h.svg</
+000002b0: 656c 6c69 7073 6573 5f76 2e73 7667 3c2f  ellipses_v.svg</
 000002c0: 6669 6c65 3e0a 2020 2020 3c66 696c 6520  file>.    <file 
-000002d0: 616c 6961 733d 2265 6c6c 6970 7365 735f  alias="ellipses_
-000002e0: 762e 7376 6722 3e69 6d61 6765 732f 6963  v.svg">images/ic
-000002f0: 6f6e 732f 6461 726b 2f65 6c6c 6970 7365  ons/dark/ellipse
-00000300: 735f 762e 7376 673c 2f66 696c 653e 0a20  s_v.svg</file>. 
-00000310: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
-00000320: 6669 6c65 2e73 7667 223e 696d 6167 6573  file.svg">images
-00000330: 2f69 636f 6e73 2f64 6172 6b2f 6669 6c65  /icons/dark/file
-00000340: 2e73 7667 3c2f 6669 6c65 3e0a 2020 2020  .svg</file>.    
-00000350: 3c66 696c 6520 616c 6961 733d 2266 6674  <file alias="fft
-00000360: 2e73 7667 223e 696d 6167 6573 2f69 636f  .svg">images/ico
-00000370: 6e73 2f66 6674 2e73 7667 3c2f 6669 6c65  ns/fft.svg</file
-00000380: 3e0a 2020 2020 3c66 696c 6520 616c 6961  >.    <file alia
-00000390: 733d 2266 726f 6d5f 636c 6970 626f 6172  s="from_clipboar
-000003a0: 642e 7376 6722 3e69 6d61 6765 732f 6963  d.svg">images/ic
-000003b0: 6f6e 732f 6461 726b 2f61 7070 6261 722e  ons/dark/appbar.
-000003c0: 6672 6f6d 5f63 6c69 7062 6f61 7264 2e73  from_clipboard.s
-000003d0: 7667 3c2f 6669 6c65 3e0a 2020 2020 3c66  vg</file>.    <f
-000003e0: 696c 6520 616c 6961 733d 2266 756c 6c73  ile alias="fulls
-000003f0: 6372 6565 6e2d 656e 7465 722e 7376 6722  creen-enter.svg"
-00000400: 3e69 6d61 6765 732f 6963 6f6e 732f 6461  >images/icons/da
-00000410: 726b 2f66 756c 6c73 6372 6565 6e2d 656e  rk/fullscreen-en
-00000420: 7465 722e 7376 673c 2f66 696c 653e 0a20  ter.svg</file>. 
-00000430: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
-00000440: 6772 6170 685f 3930 2e70 6e67 223e 696d  graph_90.png">im
-00000450: 6167 6573 2f69 636f 6e73 2f64 6172 6b2f  ages/icons/dark/
-00000460: 6772 6170 685f 3930 2e70 6e67 3c2f 6669  graph_90.png</fi
-00000470: 6c65 3e0a 2020 2020 3c66 696c 6520 616c  le>.    <file al
-00000480: 6961 733d 2267 7269 645f 6e6f 6e65 2e73  ias="grid_none.s
-00000490: 7667 223e 696d 6167 6573 2f69 636f 6e73  vg">images/icons
-000004a0: 2f67 7269 645f 6e6f 6e65 2e73 7667 3c2f  /grid_none.svg</
-000004b0: 6669 6c65 3e0a 2020 2020 3c66 696c 6520  file>.    <file 
-000004c0: 616c 6961 733d 2267 7269 645f 6669 6e65  alias="grid_fine
-000004d0: 2e73 7667 223e 696d 6167 6573 2f69 636f  .svg">images/ico
-000004e0: 6e73 2f67 7269 645f 6669 6e65 2e73 7667  ns/grid_fine.svg
-000004f0: 3c2f 6669 6c65 3e0a 2020 2020 3c66 696c  </file>.    <fil
-00000500: 6520 616c 6961 733d 2267 7269 645f 636f  e alias="grid_co
-00000510: 6172 7365 2e73 7667 223e 696d 6167 6573  arse.svg">images
-00000520: 2f69 636f 6e73 2f67 7269 645f 636f 6172  /icons/grid_coar
-00000530: 7365 2e73 7667 3c2f 6669 6c65 3e0a 2020  se.svg</file>.  
-00000540: 2020 3c66 696c 6520 616c 6961 733d 2268    <file alias="h
-00000550: 6561 7269 6e67 2e73 7667 223e 696d 6167  earing.svg">imag
-00000560: 6573 2f69 636f 6e73 2f64 6172 6b2f 6963  es/icons/dark/ic
-00000570: 5f68 6561 7269 6e67 5f34 3870 782e 7376  _hearing_48px.sv
-00000580: 673c 2f66 696c 653e 2020 0a20 2020 203c  g</file>  .    <
-00000590: 6669 6c65 2061 6c69 6173 3d22 6865 6c70  file alias="help
-000005a0: 2e73 7667 223e 696d 6167 6573 2f69 636f  .svg">images/ico
-000005b0: 6e73 2f64 6172 6b2f 6963 5f68 656c 705f  ns/dark/ic_help_
-000005c0: 6f75 746c 696e 655f 3234 7078 2e73 7667  outline_24px.svg
-000005d0: 3c2f 6669 6c65 3e0a 2020 2020 3c66 696c  </file>.    <fil
-000005e0: 6520 616c 6961 733d 2268 6f6d 652e 7376  e alias="home.sv
-000005f0: 6722 3e69 6d61 6765 732f 6963 6f6e 732f  g">images/icons/
-00000600: 6461 726b 2f68 6f6d 652e 7376 673c 2f66  dark/home.svg</f
-00000610: 696c 653e 0a20 2020 203c 6669 6c65 2061  ile>.    <file a
-00000620: 6c69 6173 3d22 6c6f 636b 2d6c 6f63 6b65  lias="lock-locke
-00000630: 642e 7376 6722 3e69 6d61 6765 732f 6963  d.svg">images/ic
-00000640: 6f6e 732f 6461 726b 2f6c 6f63 6b2d 6c6f  ons/dark/lock-lo
-00000650: 636b 6564 2e73 7667 3c2f 6669 6c65 3e0a  cked.svg</file>.
-00000660: 2020 2020 3c66 696c 6520 616c 6961 733d      <file alias=
-00000670: 226c 6f63 6b2d 756e 6c6f 636b 6564 2e73  "lock-unlocked.s
-00000680: 7667 223e 696d 6167 6573 2f69 636f 6e73  vg">images/icons
-00000690: 2f64 6172 6b2f 6c6f 636b 2d75 6e6c 6f63  /dark/lock-unloc
-000006a0: 6b65 642e 7376 673c 2f66 696c 653e 2020  ked.svg</file>  
-000006b0: 2020 0a20 2020 203c 6669 6c65 2061 6c69    .    <file ali
-000006c0: 6173 3d22 6d61 676e 6966 7969 6e67 2d67  as="magnifying-g
-000006d0: 6c61 7373 2e73 7667 223e 696d 6167 6573  lass.svg">images
-000006e0: 2f69 636f 6e73 2f64 6172 6b2f 6d61 676e  /icons/dark/magn
-000006f0: 6966 7969 6e67 2d67 6c61 7373 2e73 7667  ifying-glass.svg
-00000700: 3c2f 6669 6c65 3e0a 2020 2020 3c66 696c  </file>.    <fil
-00000710: 6520 616c 6961 733d 226d 6f76 652e 7376  e alias="move.sv
-00000720: 6722 3e69 6d61 6765 732f 6963 6f6e 732f  g">images/icons/
-00000730: 6461 726b 2f6d 6f76 652e 7376 673c 2f66  dark/move.svg</f
-00000740: 696c 653e 0a20 2020 203c 6669 6c65 2061  ile>.    <file a
-00000750: 6c69 6173 3d22 6d61 702d 6d61 726b 6572  lias="map-marker
-00000760: 2e73 7667 223e 696d 6167 6573 2f69 636f  .svg">images/ico
-00000770: 6e73 2f64 6172 6b2f 6d61 702d 6d61 726b  ns/dark/map-mark
-00000780: 6572 2e73 7667 3c2f 6669 6c65 3e0a 2020  er.svg</file>.  
-00000790: 2020 3c66 696c 6520 616c 6961 733d 2270    <file alias="p
-000007a0: 6c61 792e 7376 6722 3e69 6d61 6765 732f  lay.svg">images/
-000007b0: 6963 6f6e 732f 6461 726b 2f69 635f 706c  icons/dark/ic_pl
-000007c0: 6179 5f61 7272 6f77 5f34 3870 782e 7376  ay_arrow_48px.sv
-000007d0: 673c 2f66 696c 653e 2020 0a20 2020 203c  g</file>  .    <
-000007e0: 6669 6c65 2061 6c69 6173 3d22 7175 616e  file alias="quan
-000007f0: 7469 7a65 2e73 7667 223e 696d 6167 6573  tize.svg">images
-00000800: 2f69 636f 6e73 2f64 6172 6b2f 7175 616e  /icons/dark/quan
-00000810: 7469 7a65 2e73 7667 3c2f 6669 6c65 3e0a  tize.svg</file>.
-00000820: 2020 2020 3c66 696c 6520 616c 6961 733d      <file alias=
-00000830: 2272 6f77 5f64 656c 6574 652e 7376 6722  "row_delete.svg"
-00000840: 3e69 6d61 6765 732f 6963 6f6e 732f 6461  >images/icons/da
-00000850: 726b 2f61 7070 6261 722e 6c69 7374 2e64  rk/appbar.list.d
-00000860: 656c 6574 652e 7376 673c 2f66 696c 653e  elete.svg</file>
-00000870: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
-00000880: 3d22 726f 775f 696e 7365 7274 5f61 626f  ="row_insert_abo
-00000890: 7665 2e73 7667 223e 696d 6167 6573 2f69  ve.svg">images/i
-000008a0: 636f 6e73 2f64 6172 6b2f 6170 7062 6172  cons/dark/appbar
-000008b0: 2e6c 6973 742e 6164 642e 6162 6f76 652e  .list.add.above.
-000008c0: 7376 673c 2f66 696c 653e 0a20 2020 203c  svg</file>.    <
-000008d0: 6669 6c65 2061 6c69 6173 3d22 7361 7665  file alias="save
-000008e0: 2e73 7667 223e 696d 6167 6573 2f69 636f  .svg">images/ico
-000008f0: 6e73 2f64 6172 6b2f 6170 7062 6172 2e64  ns/dark/appbar.d
-00000900: 6973 6b2e 7376 673c 2f66 696c 653e 0a20  isk.svg</file>. 
-00000910: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
-00000920: 7365 7474 696e 6773 2e73 7667 223e 696d  settings.svg">im
-00000930: 6167 6573 2f69 636f 6e73 2f64 6172 6b2f  ages/icons/dark/
-00000940: 636f 672e 7376 673c 2f66 696c 653e 0a20  cog.svg</file>. 
-00000950: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
-00000960: 7370 6561 6b65 722e 7376 6722 3e69 6d61  speaker.svg">ima
-00000970: 6765 732f 6963 6f6e 732f 6461 726b 2f69  ges/icons/dark/i
-00000980: 635f 766f 6c75 6d65 5f75 705f 3438 7078  c_volume_up_48px
-00000990: 2e73 7667 3c2f 6669 6c65 3e0a 2020 2020  .svg</file>.    
-000009a0: 3c66 696c 6520 616c 6961 733d 2273 7065  <file alias="spe
-000009b0: 616b 6572 5f39 302e 7376 6722 3e69 6d61  aker_90.svg">ima
-000009c0: 6765 732f 6963 6f6e 732f 6461 726b 2f69  ges/icons/dark/i
-000009d0: 635f 766f 6c75 6d65 5f75 705f 3438 7078  c_volume_up_48px
-000009e0: 5f39 302e 7376 673c 2f66 696c 653e 0a20  _90.svg</file>. 
-000009f0: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
-00000a00: 736f 7274 2d61 7363 656e 6469 6e67 2e73  sort-ascending.s
-00000a10: 7667 223e 696d 6167 6573 2f69 636f 6e73  vg">images/icons
-00000a20: 2f64 6172 6b2f 736f 7274 2d61 7363 656e  /dark/sort-ascen
-00000a30: 6469 6e67 2e73 7667 3c2f 6669 6c65 3e0a  ding.svg</file>.
-00000a40: 2020 2020 3c21 2d2d 203c 6669 6c65 2061      <!-- <file a
-00000a50: 6c69 6173 3d22 7374 6f70 2e73 7667 223e  lias="stop.svg">
-00000a60: 696d 6167 6573 2f69 636f 6e73 2f64 6172  images/icons/dar
-00000a70: 6b2f 6963 5f73 746f 705f 3438 7078 2e73  k/ic_stop_48px.s
-00000a80: 7667 3c2f 6669 6c65 3e20 2d2d 3e0a 2020  vg</file> -->.  
-00000a90: 2020 3c66 696c 6520 616c 6961 733d 2273    <file alias="s
-00000aa0: 746f 702e 7376 6722 3e69 6d61 6765 732f  top.svg">images/
-00000ab0: 6963 6f6e 732f 6461 726b 2f69 635f 706c  icons/dark/ic_pl
-00000ac0: 6179 5f61 7272 6f77 5f34 3870 782e 7376  ay_arrow_48px.sv
-00000ad0: 673c 2f66 696c 653e 0a20 2020 203c 6669  g</file>.    <fi
-00000ae0: 6c65 2061 6c69 6173 3d22 746f 5f63 6c69  le alias="to_cli
-00000af0: 7062 6f61 7264 2e73 7667 223e 696d 6167  pboard.svg">imag
-00000b00: 6573 2f69 636f 6e73 2f64 6172 6b2f 6170  es/icons/dark/ap
-00000b10: 7062 6172 2e74 6f5f 636c 6970 626f 6172  pbar.to_clipboar
-00000b20: 642e 7376 673c 2f66 696c 653e 0a20 2020  d.svg</file>.   
-00000b30: 203c 6669 6c65 2061 6c69 6173 3d22 7472   <file alias="tr
-00000b40: 6173 682e 7376 6722 3e69 6d61 6765 732f  ash.svg">images/
-00000b50: 6963 6f6e 732f 6461 726b 2f74 7261 7368  icons/dark/trash
-00000b60: 2e73 7667 3c2f 6669 6c65 3e0a 2020 2020  .svg</file>.    
-00000b70: 3c66 696c 6520 616c 6961 733d 2275 706c  <file alias="upl
-00000b80: 6f61 642e 7376 6722 3e69 6d61 6765 732f  oad.svg">images/
-00000b90: 6963 6f6e 732f 6461 726b 2f64 6174 612d  icons/dark/data-
-00000ba0: 7472 616e 7366 6572 2d75 706c 6f61 642e  transfer-upload.
-00000bb0: 7376 673c 2f66 696c 653e 0a0a 2020 2020  svg</file>..    
-00000bc0: 3c66 696c 6520 616c 6961 733d 2270 6175  <file alias="pau
-00000bd0: 7365 5f77 2e73 7667 223e 696d 6167 6573  se_w.svg">images
-00000be0: 2f69 636f 6e73 2f6c 6967 6874 2f69 635f  /icons/light/ic_
-00000bf0: 7061 7573 655f 3438 7078 5f77 6869 7465  pause_48px_white
-00000c00: 2e73 7667 3c2f 6669 6c65 3e0a 2020 2020  .svg</file>.    
-00000c10: 3c66 696c 6520 616c 6961 733d 2270 6c61  <file alias="pla
-00000c20: 795f 772e 7376 6722 3e69 6d61 6765 732f  y_w.svg">images/
-00000c30: 6963 6f6e 732f 6c69 6768 742f 6963 5f70  icons/light/ic_p
-00000c40: 6c61 795f 6172 726f 775f 3438 7078 5f77  lay_arrow_48px_w
-00000c50: 6869 7465 2e73 7667 3c2f 6669 6c65 3e0a  hite.svg</file>.
-00000c60: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
-00000c70: 3d22 706c 6f74 5f73 7479 6c65 2d6e 6f6e  ="plot_style-non
-00000c80: 6522 3e69 6d61 6765 732f 6963 6f6e 732f  e">images/icons/
-00000c90: 706c 6f74 5f73 7479 6c65 2d6e 6f6e 652e  plot_style-none.
-00000ca0: 706e 673c 2f66 696c 653e 0a20 2020 203c  png</file>.    <
-00000cb0: 6669 6c65 2061 6c69 6173 3d22 706c 6f74  file alias="plot
-00000cc0: 5f73 7479 6c65 2d6d 6b72 223e 696d 6167  _style-mkr">imag
-00000cd0: 6573 2f69 636f 6e73 2f70 6c6f 745f 7374  es/icons/plot_st
-00000ce0: 796c 652d 6d6b 722e 706e 673c 2f66 696c  yle-mkr.png</fil
-00000cf0: 653e 0a20 2020 203c 6669 6c65 2061 6c69  e>.    <file ali
-00000d00: 6173 3d22 706c 6f74 5f73 7479 6c65 2d6c  as="plot_style-l
-00000d10: 696e 6522 3e69 6d61 6765 732f 6963 6f6e  ine">images/icon
-00000d20: 732f 706c 6f74 5f73 7479 6c65 2d6c 696e  s/plot_style-lin
-00000d30: 652e 706e 673c 2f66 696c 653e 0a20 2020  e.png</file>.   
-00000d40: 203c 6669 6c65 2061 6c69 6173 3d22 706c   <file alias="pl
-00000d50: 6f74 5f73 7479 6c65 2d6c 696e 652d 6d6b  ot_style-line-mk
-00000d60: 7222 3e69 6d61 6765 732f 6963 6f6e 732f  r">images/icons/
-00000d70: 706c 6f74 5f73 7479 6c65 2d6c 696e 652d  plot_style-line-
-00000d80: 6d6b 722e 706e 673c 2f66 696c 653e 0a20  mkr.png</file>. 
-00000d90: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
-00000da0: 706c 6f74 5f73 7479 6c65 2d73 7465 6d22  plot_style-stem"
-00000db0: 3e69 6d61 6765 732f 6963 6f6e 732f 706c  >images/icons/pl
-00000dc0: 6f74 5f73 7479 6c65 2d73 7465 6d2e 706e  ot_style-stem.pn
-00000dd0: 673c 2f66 696c 653e 0a20 2020 203c 6669  g</file>.    <fi
-00000de0: 6c65 2061 6c69 6173 3d22 706c 6f74 5f73  le alias="plot_s
-00000df0: 7479 6c65 2d73 7465 6d2d 6d6b 7222 3e69  tyle-stem-mkr">i
-00000e00: 6d61 6765 732f 6963 6f6e 732f 706c 6f74  mages/icons/plot
-00000e10: 5f73 7479 6c65 2d73 7465 6d2d 6d6b 722e  _style-stem-mkr.
-00000e20: 706e 673c 2f66 696c 653e 0a20 2020 203c  png</file>.    <
-00000e30: 6669 6c65 2061 6c69 6173 3d22 706c 6f74  file alias="plot
-00000e40: 5f73 7479 6c65 2d73 7465 7073 223e 696d  _style-steps">im
-00000e50: 6167 6573 2f69 636f 6e73 2f70 6c6f 745f  ages/icons/plot_
-00000e60: 7374 796c 652d 7374 6570 732e 706e 673c  style-steps.png<
-00000e70: 2f66 696c 653e 0a20 2020 203c 6669 6c65  /file>.    <file
-00000e80: 2061 6c69 6173 3d22 706c 6f74 5f73 7479   alias="plot_sty
-00000e90: 6c65 2d73 7465 7073 2d6d 6b72 223e 696d  le-steps-mkr">im
-00000ea0: 6167 6573 2f69 636f 6e73 2f70 6c6f 745f  ages/icons/plot_
-00000eb0: 7374 796c 652d 7374 6570 732d 6d6b 722e  style-steps-mkr.
-00000ec0: 706e 673c 2f66 696c 653e 0a0a 2020 2020  png</file>..    
-00000ed0: 3c66 696c 6520 616c 6961 733d 2270 7966  <file alias="pyf
-00000ee0: 6461 5f69 636f 6e2e 7376 6722 3e69 6d61  da_icon.svg">ima
-00000ef0: 6765 732f 6963 6f6e 732f 7079 6664 615f  ges/icons/pyfda_
-00000f00: 6963 6f6e 2e73 7667 3c2f 6669 6c65 3e0a  icon.svg</file>.
-00000f10: 3c2f 7172 6573 6f75 7263 653e 0a0a 0a3c  </qresource>...<
-00000f20: 2f52 4343 3e0a 0a0a 3c21 2d2d 200a 2020  /RCC>...<!-- .  
-00000f30: 2020 2051 7450 7935 3a20 7079 7263 6335     QtPy5: pyrcc5
-00000f40: 2070 7966 6461 2e71 7263 202d 6f20 7172   pyfda.qrc -o qr
-00000f50: 635f 7265 736f 7572 6365 732e 7079 0a2d  c_resources.py.-
-00000f60: 2d3e 0a0a                                ->..
+000002d0: 616c 6961 733d 2266 696c 652e 7376 6722  alias="file.svg"
+000002e0: 3e69 6d61 6765 732f 6963 6f6e 732f 6461  >images/icons/da
+000002f0: 726b 2f66 696c 652e 7376 673c 2f66 696c  rk/file.svg</fil
+00000300: 653e 0a20 2020 203c 6669 6c65 2061 6c69  e>.    <file ali
+00000310: 6173 3d22 6666 742e 7376 6722 3e69 6d61  as="fft.svg">ima
+00000320: 6765 732f 6963 6f6e 732f 6666 742e 7376  ges/icons/fft.sv
+00000330: 673c 2f66 696c 653e 0a20 2020 203c 6669  g</file>.    <fi
+00000340: 6c65 2061 6c69 6173 3d22 6672 6f6d 5f63  le alias="from_c
+00000350: 6c69 7062 6f61 7264 2e73 7667 223e 696d  lipboard.svg">im
+00000360: 6167 6573 2f69 636f 6e73 2f64 6172 6b2f  ages/icons/dark/
+00000370: 6170 7062 6172 2e66 726f 6d5f 636c 6970  appbar.from_clip
+00000380: 626f 6172 642e 7376 673c 2f66 696c 653e  board.svg</file>
+00000390: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
+000003a0: 3d22 6675 6c6c 7363 7265 656e 2d65 6e74  ="fullscreen-ent
+000003b0: 6572 2e73 7667 223e 696d 6167 6573 2f69  er.svg">images/i
+000003c0: 636f 6e73 2f64 6172 6b2f 6675 6c6c 7363  cons/dark/fullsc
+000003d0: 7265 656e 2d65 6e74 6572 2e73 7667 3c2f  reen-enter.svg</
+000003e0: 6669 6c65 3e0a 2020 2020 3c66 696c 6520  file>.    <file 
+000003f0: 616c 6961 733d 2267 7261 7068 5f39 302e  alias="graph_90.
+00000400: 7376 6722 3e69 6d61 6765 732f 6963 6f6e  svg">images/icon
+00000410: 732f 6461 726b 2f67 7261 7068 5f39 302e  s/dark/graph_90.
+00000420: 7376 673c 2f66 696c 653e 0a20 2020 203c  svg</file>.    <
+00000430: 6669 6c65 2061 6c69 6173 3d22 6772 6964  file alias="grid
+00000440: 5f6e 6f6e 652e 7376 6722 3e69 6d61 6765  _none.svg">image
+00000450: 732f 6963 6f6e 732f 6461 726b 2f67 7269  s/icons/dark/gri
+00000460: 645f 6e6f 6e65 2e73 7667 3c2f 6669 6c65  d_none.svg</file
+00000470: 3e0a 2020 2020 3c66 696c 6520 616c 6961  >.    <file alia
+00000480: 733d 2267 7269 645f 6669 6e65 2e73 7667  s="grid_fine.svg
+00000490: 223e 696d 6167 6573 2f69 636f 6e73 2f64  ">images/icons/d
+000004a0: 6172 6b2f 6772 6964 5f66 696e 652e 7376  ark/grid_fine.sv
+000004b0: 673c 2f66 696c 653e 0a20 2020 203c 6669  g</file>.    <fi
+000004c0: 6c65 2061 6c69 6173 3d22 6772 6964 5f63  le alias="grid_c
+000004d0: 6f61 7273 652e 7376 6722 3e69 6d61 6765  oarse.svg">image
+000004e0: 732f 6963 6f6e 732f 6461 726b 2f67 7269  s/icons/dark/gri
+000004f0: 645f 636f 6172 7365 2e73 7667 3c2f 6669  d_coarse.svg</fi
+00000500: 6c65 3e0a 2020 2020 203c 212d 2d20 203c  le>.     <!--  <
+00000510: 6669 6c65 2061 6c69 6173 3d22 6865 6172  file alias="hear
+00000520: 696e 672e 7376 6722 3e69 6d61 6765 732f  ing.svg">images/
+00000530: 6963 6f6e 732f 6461 726b 2f69 635f 6865  icons/dark/ic_he
+00000540: 6172 696e 675f 3438 7078 2e73 7667 3c2f  aring_48px.svg</
+00000550: 6669 6c65 3e20 202d 2d3e 0a20 2020 203c  file>  -->.    <
+00000560: 6669 6c65 2061 6c69 6173 3d22 6865 6c70  file alias="help
+00000570: 2e73 7667 223e 696d 6167 6573 2f69 636f  .svg">images/ico
+00000580: 6e73 2f64 6172 6b2f 6963 5f68 656c 705f  ns/dark/ic_help_
+00000590: 3234 7078 2e73 7667 3c2f 6669 6c65 3e0a  24px.svg</file>.
+000005a0: 2020 2020 3c66 696c 6520 616c 6961 733d      <file alias=
+000005b0: 2268 6f6d 652e 7376 6722 3e69 6d61 6765  "home.svg">image
+000005c0: 732f 6963 6f6e 732f 6461 726b 2f68 6f6d  s/icons/dark/hom
+000005d0: 652e 7376 673c 2f66 696c 653e 0a20 2020  e.svg</file>.   
+000005e0: 203c 6669 6c65 2061 6c69 6173 3d22 6c6f   <file alias="lo
+000005f0: 636b 2d6c 6f63 6b65 642e 7376 6722 3e69  ck-locked.svg">i
+00000600: 6d61 6765 732f 6963 6f6e 732f 6461 726b  mages/icons/dark
+00000610: 2f6c 6f63 6b2d 6c6f 636b 6564 2e73 7667  /lock-locked.svg
+00000620: 3c2f 6669 6c65 3e0a 2020 2020 3c66 696c  </file>.    <fil
+00000630: 6520 616c 6961 733d 226c 6f63 6b2d 756e  e alias="lock-un
+00000640: 6c6f 636b 6564 2e73 7667 223e 696d 6167  locked.svg">imag
+00000650: 6573 2f69 636f 6e73 2f64 6172 6b2f 6c6f  es/icons/dark/lo
+00000660: 636b 2d75 6e6c 6f63 6b65 642e 7376 673c  ck-unlocked.svg<
+00000670: 2f66 696c 653e 2020 2020 0a20 2020 203c  /file>    .    <
+00000680: 6669 6c65 2061 6c69 6173 3d22 6d61 676e  file alias="magn
+00000690: 6966 7969 6e67 2d67 6c61 7373 2e73 7667  ifying-glass.svg
+000006a0: 223e 696d 6167 6573 2f69 636f 6e73 2f64  ">images/icons/d
+000006b0: 6172 6b2f 6d61 676e 6966 7969 6e67 2d67  ark/magnifying-g
+000006c0: 6c61 7373 2e73 7667 3c2f 6669 6c65 3e0a  lass.svg</file>.
+000006d0: 2020 2020 3c66 696c 6520 616c 6961 733d      <file alias=
+000006e0: 226d 6f76 652e 7376 6722 3e69 6d61 6765  "move.svg">image
+000006f0: 732f 6963 6f6e 732f 6461 726b 2f6d 6f76  s/icons/dark/mov
+00000700: 652e 7376 673c 2f66 696c 653e 0a20 2020  e.svg</file>.   
+00000710: 203c 6669 6c65 2061 6c69 6173 3d22 6d61   <file alias="ma
+00000720: 702d 6d61 726b 6572 2e73 7667 223e 696d  p-marker.svg">im
+00000730: 6167 6573 2f69 636f 6e73 2f64 6172 6b2f  ages/icons/dark/
+00000740: 6d61 702d 6d61 726b 6572 2e73 7667 3c2f  map-marker.svg</
+00000750: 6669 6c65 3e0a 2020 2020 3c66 696c 6520  file>.    <file 
+00000760: 616c 6961 733d 2270 6c61 792e 7376 6722  alias="play.svg"
+00000770: 3e69 6d61 6765 732f 6963 6f6e 732f 6461  >images/icons/da
+00000780: 726b 2f69 635f 706c 6179 5f61 7272 6f77  rk/ic_play_arrow
+00000790: 5f34 3870 782e 7376 673c 2f66 696c 653e  _48px.svg</file>
+000007a0: 2020 0a20 2020 203c 6669 6c65 2061 6c69    .    <file ali
+000007b0: 6173 3d22 7175 616e 7469 7a65 2e73 7667  as="quantize.svg
+000007c0: 223e 696d 6167 6573 2f69 636f 6e73 2f64  ">images/icons/d
+000007d0: 6172 6b2f 7175 616e 7469 7a65 2e73 7667  ark/quantize.svg
+000007e0: 3c2f 6669 6c65 3e0a 2020 2020 3c66 696c  </file>.    <fil
+000007f0: 6520 616c 6961 733d 2272 6f77 5f64 656c  e alias="row_del
+00000800: 6574 652e 7376 6722 3e69 6d61 6765 732f  ete.svg">images/
+00000810: 6963 6f6e 732f 6461 726b 2f61 7070 6261  icons/dark/appba
+00000820: 722e 6c69 7374 2e64 656c 6574 652e 7376  r.list.delete.sv
+00000830: 673c 2f66 696c 653e 0a20 2020 203c 6669  g</file>.    <fi
+00000840: 6c65 2061 6c69 6173 3d22 726f 775f 696e  le alias="row_in
+00000850: 7365 7274 5f61 626f 7665 2e73 7667 223e  sert_above.svg">
+00000860: 696d 6167 6573 2f69 636f 6e73 2f64 6172  images/icons/dar
+00000870: 6b2f 6170 7062 6172 2e6c 6973 742e 6164  k/appbar.list.ad
+00000880: 642e 6162 6f76 652e 7376 673c 2f66 696c  d.above.svg</fil
+00000890: 653e 0a20 2020 203c 6669 6c65 2061 6c69  e>.    <file ali
+000008a0: 6173 3d22 7361 7665 2e73 7667 223e 696d  as="save.svg">im
+000008b0: 6167 6573 2f69 636f 6e73 2f64 6172 6b2f  ages/icons/dark/
+000008c0: 6170 7062 6172 2e64 6973 6b2e 7376 673c  appbar.disk.svg<
+000008d0: 2f66 696c 653e 0a20 2020 203c 6669 6c65  /file>.    <file
+000008e0: 2061 6c69 6173 3d22 7365 7474 696e 6773   alias="settings
+000008f0: 2e73 7667 223e 696d 6167 6573 2f69 636f  .svg">images/ico
+00000900: 6e73 2f64 6172 6b2f 636f 672e 7376 673c  ns/dark/cog.svg<
+00000910: 2f66 696c 653e 0a20 2020 203c 6669 6c65  /file>.    <file
+00000920: 2061 6c69 6173 3d22 7370 6561 6b65 722e   alias="speaker.
+00000930: 7376 6722 3e69 6d61 6765 732f 6963 6f6e  svg">images/icon
+00000940: 732f 6461 726b 2f69 635f 766f 6c75 6d65  s/dark/ic_volume
+00000950: 5f75 705f 3438 7078 2e73 7667 3c2f 6669  _up_48px.svg</fi
+00000960: 6c65 3e0a 2020 2020 3c66 696c 6520 616c  le>.    <file al
+00000970: 6961 733d 2273 7065 616b 6572 5f39 302e  ias="speaker_90.
+00000980: 7376 6722 3e69 6d61 6765 732f 6963 6f6e  svg">images/icon
+00000990: 732f 6461 726b 2f69 635f 766f 6c75 6d65  s/dark/ic_volume
+000009a0: 5f75 705f 3438 7078 5f39 302e 7376 673c  _up_48px_90.svg<
+000009b0: 2f66 696c 653e 0a20 2020 203c 6669 6c65  /file>.    <file
+000009c0: 2061 6c69 6173 3d22 736f 7274 2d61 7363   alias="sort-asc
+000009d0: 656e 6469 6e67 2e73 7667 223e 696d 6167  ending.svg">imag
+000009e0: 6573 2f69 636f 6e73 2f64 6172 6b2f 736f  es/icons/dark/so
+000009f0: 7274 2d61 7363 656e 6469 6e67 2e73 7667  rt-ascending.svg
+00000a00: 3c2f 6669 6c65 3e0a 2020 2020 3c21 2d2d  </file>.    <!--
+00000a10: 203c 6669 6c65 2061 6c69 6173 3d22 7374   <file alias="st
+00000a20: 6f70 2e73 7667 223e 696d 6167 6573 2f69  op.svg">images/i
+00000a30: 636f 6e73 2f64 6172 6b2f 6963 5f73 746f  cons/dark/ic_sto
+00000a40: 705f 3438 7078 2e73 7667 3c2f 6669 6c65  p_48px.svg</file
+00000a50: 3e20 2d2d 3e0a 2020 2020 3c66 696c 6520  > -->.    <file 
+00000a60: 616c 6961 733d 2273 746f 702e 7376 6722  alias="stop.svg"
+00000a70: 3e69 6d61 6765 732f 6963 6f6e 732f 6461  >images/icons/da
+00000a80: 726b 2f69 635f 706c 6179 5f61 7272 6f77  rk/ic_play_arrow
+00000a90: 5f34 3870 782e 7376 673c 2f66 696c 653e  _48px.svg</file>
+00000aa0: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
+00000ab0: 3d22 746f 5f63 6c69 7062 6f61 7264 2e73  ="to_clipboard.s
+00000ac0: 7667 223e 696d 6167 6573 2f69 636f 6e73  vg">images/icons
+00000ad0: 2f64 6172 6b2f 6170 7062 6172 2e74 6f5f  /dark/appbar.to_
+00000ae0: 636c 6970 626f 6172 642e 7376 673c 2f66  clipboard.svg</f
+00000af0: 696c 653e 0a20 2020 203c 6669 6c65 2061  ile>.    <file a
+00000b00: 6c69 6173 3d22 7472 6173 682e 7376 6722  lias="trash.svg"
+00000b10: 3e69 6d61 6765 732f 6963 6f6e 732f 6461  >images/icons/da
+00000b20: 726b 2f74 7261 7368 2e73 7667 3c2f 6669  rk/trash.svg</fi
+00000b30: 6c65 3e0a 2020 2020 3c66 696c 6520 616c  le>.    <file al
+00000b40: 6961 733d 2275 695f 6c65 7665 6c5f 6d69  ias="ui_level_mi
+00000b50: 6e2e 7376 6722 3e69 6d61 6765 732f 6963  n.svg">images/ic
+00000b60: 6f6e 732f 6461 726b 2f64 656e 7369 7479  ons/dark/density
+00000b70: 5f6c 6172 6765 2e73 7667 3c2f 6669 6c65  _large.svg</file
+00000b80: 3e0a 2020 2020 3c66 696c 6520 616c 6961  >.    <file alia
+00000b90: 733d 2275 695f 6c65 7665 6c5f 6d69 642e  s="ui_level_mid.
+00000ba0: 7376 6722 3e69 6d61 6765 732f 6963 6f6e  svg">images/icon
+00000bb0: 732f 6461 726b 2f64 656e 7369 7479 5f6d  s/dark/density_m
+00000bc0: 6564 6975 6d2e 7376 673c 2f66 696c 653e  edium.svg</file>
+00000bd0: 0a20 2020 203c 6669 6c65 2061 6c69 6173  .    <file alias
+00000be0: 3d22 7569 5f6c 6576 656c 5f6d 6178 2e73  ="ui_level_max.s
+00000bf0: 7667 223e 696d 6167 6573 2f69 636f 6e73  vg">images/icons
+00000c00: 2f64 6172 6b2f 6465 6e73 6974 795f 736d  /dark/density_sm
+00000c10: 616c 6c2e 7376 673c 2f66 696c 653e 0a20  all.svg</file>. 
+00000c20: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
+00000c30: 7570 6c6f 6164 2e73 7667 223e 696d 6167  upload.svg">imag
+00000c40: 6573 2f69 636f 6e73 2f64 6172 6b2f 6461  es/icons/dark/da
+00000c50: 7461 2d74 7261 6e73 6665 722d 7570 6c6f  ta-transfer-uplo
+00000c60: 6164 2e73 7667 3c2f 6669 6c65 3e0a 0a20  ad.svg</file>.. 
+00000c70: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
+00000c80: 7061 7573 655f 772e 7376 6722 3e69 6d61  pause_w.svg">ima
+00000c90: 6765 732f 6963 6f6e 732f 6c69 6768 742f  ges/icons/light/
+00000ca0: 6963 5f70 6175 7365 5f34 3870 785f 7768  ic_pause_48px_wh
+00000cb0: 6974 652e 7376 673c 2f66 696c 653e 0a20  ite.svg</file>. 
+00000cc0: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
+00000cd0: 706c 6179 5f77 2e73 7667 223e 696d 6167  play_w.svg">imag
+00000ce0: 6573 2f69 636f 6e73 2f6c 6967 6874 2f69  es/icons/light/i
+00000cf0: 635f 706c 6179 5f61 7272 6f77 5f34 3870  c_play_arrow_48p
+00000d00: 785f 7768 6974 652e 7376 673c 2f66 696c  x_white.svg</fil
+00000d10: 653e 0a0a 2020 2020 3c66 696c 6520 616c  e>..    <file al
+00000d20: 6961 733d 2270 6c6f 745f 7374 796c 652d  ias="plot_style-
+00000d30: 6e6f 6e65 223e 696d 6167 6573 2f69 636f  none">images/ico
+00000d40: 6e73 2f70 6c6f 745f 7374 796c 652d 6e6f  ns/plot_style-no
+00000d50: 6e65 2e70 6e67 3c2f 6669 6c65 3e0a 2020  ne.png</file>.  
+00000d60: 2020 3c66 696c 6520 616c 6961 733d 2270    <file alias="p
+00000d70: 6c6f 745f 7374 796c 652d 6d6b 7222 3e69  lot_style-mkr">i
+00000d80: 6d61 6765 732f 6963 6f6e 732f 706c 6f74  mages/icons/plot
+00000d90: 5f73 7479 6c65 2d6d 6b72 2e70 6e67 3c2f  _style-mkr.png</
+00000da0: 6669 6c65 3e0a 2020 2020 3c66 696c 6520  file>.    <file 
+00000db0: 616c 6961 733d 2270 6c6f 745f 7374 796c  alias="plot_styl
+00000dc0: 652d 6c69 6e65 223e 696d 6167 6573 2f69  e-line">images/i
+00000dd0: 636f 6e73 2f70 6c6f 745f 7374 796c 652d  cons/plot_style-
+00000de0: 6c69 6e65 2e70 6e67 3c2f 6669 6c65 3e0a  line.png</file>.
+00000df0: 2020 2020 3c66 696c 6520 616c 6961 733d      <file alias=
+00000e00: 2270 6c6f 745f 7374 796c 652d 6c69 6e65  "plot_style-line
+00000e10: 2d6d 6b72 223e 696d 6167 6573 2f69 636f  -mkr">images/ico
+00000e20: 6e73 2f70 6c6f 745f 7374 796c 652d 6c69  ns/plot_style-li
+00000e30: 6e65 2d6d 6b72 2e70 6e67 3c2f 6669 6c65  ne-mkr.png</file
+00000e40: 3e0a 2020 2020 3c66 696c 6520 616c 6961  >.    <file alia
+00000e50: 733d 2270 6c6f 745f 7374 796c 652d 7374  s="plot_style-st
+00000e60: 656d 223e 696d 6167 6573 2f69 636f 6e73  em">images/icons
+00000e70: 2f70 6c6f 745f 7374 796c 652d 7374 656d  /plot_style-stem
+00000e80: 2e70 6e67 3c2f 6669 6c65 3e0a 2020 2020  .png</file>.    
+00000e90: 3c66 696c 6520 616c 6961 733d 2270 6c6f  <file alias="plo
+00000ea0: 745f 7374 796c 652d 7374 656d 2d6d 6b72  t_style-stem-mkr
+00000eb0: 223e 696d 6167 6573 2f69 636f 6e73 2f70  ">images/icons/p
+00000ec0: 6c6f 745f 7374 796c 652d 7374 656d 2d6d  lot_style-stem-m
+00000ed0: 6b72 2e70 6e67 3c2f 6669 6c65 3e0a 2020  kr.png</file>.  
+00000ee0: 2020 3c66 696c 6520 616c 6961 733d 2270    <file alias="p
+00000ef0: 6c6f 745f 7374 796c 652d 7374 6570 7322  lot_style-steps"
+00000f00: 3e69 6d61 6765 732f 6963 6f6e 732f 706c  >images/icons/pl
+00000f10: 6f74 5f73 7479 6c65 2d73 7465 7073 2e70  ot_style-steps.p
+00000f20: 6e67 3c2f 6669 6c65 3e0a 2020 2020 3c66  ng</file>.    <f
+00000f30: 696c 6520 616c 6961 733d 2270 6c6f 745f  ile alias="plot_
+00000f40: 7374 796c 652d 7374 6570 732d 6d6b 7222  style-steps-mkr"
+00000f50: 3e69 6d61 6765 732f 6963 6f6e 732f 706c  >images/icons/pl
+00000f60: 6f74 5f73 7479 6c65 2d73 7465 7073 2d6d  ot_style-steps-m
+00000f70: 6b72 2e70 6e67 3c2f 6669 6c65 3e0a 0a20  kr.png</file>.. 
+00000f80: 2020 203c 6669 6c65 2061 6c69 6173 3d22     <file alias="
+00000f90: 7079 6664 615f 6963 6f6e 2e73 7667 223e  pyfda_icon.svg">
+00000fa0: 696d 6167 6573 2f69 636f 6e73 2f70 7966  images/icons/pyf
+00000fb0: 6461 5f69 636f 6e2e 7376 673c 2f66 696c  da_icon.svg</fil
+00000fc0: 653e 0a3c 2f71 7265 736f 7572 6365 3e0a  e>.</qresource>.
+00000fd0: 0a0a 3c2f 5243 433e 0a0a 0a3c 212d 2d20  ..</RCC>...<!-- 
+00000fe0: 0a20 2020 2020 5174 5079 353a 2070 7972  .     QtPy5: pyr
+00000ff0: 6363 3520 7079 6664 612e 7172 6320 2d6f  cc5 pyfda.qrc -o
+00001000: 2071 7263 5f72 6573 6f75 7263 6573 2e70   qrc_resources.p
+00001010: 790a 2d2d 3e0a 0a                        y.-->..
```

### Comparing `pyfda-0.7.1/pyfda/pyfda_rc.py` & `pyfda-0.8.0a2/pyfda/pyfda_rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,18 +41,18 @@
 # Mac only:         macintosh
 
 mpl_ms = 8  # base size for matplotlib markers
 # Various parameters for calculation and plotting
 params = {'N_FFT':  2048,   # number of FFT points for plot commands (freqz etc.)
           'FMT': '{:.3g}',  # format string for QLineEdit fields
           'CSV':  {  # format options and parameters for CSV-files and clipboard
-                  'delimiter': ',',  # default delimiter
-                  'lineterminator': CRLF,  # OS-dependend line break from pyfda_lib
+                  'delimiter': 'auto',  # default delimiter
+                  'lineterminator': CRLF,  # OS-dependent line break from pyfda_lib
                   'orientation': 'auto',  # 'auto', 'vert', 'horiz'# table orientation
-                  'header': 'off',  # 'auto', 'on', 'off'
+                  'header': 'auto',  # 'auto', 'on', 'off'
                   'cmsis' : False,  # True, False
                   'clipboard': False  # source/target is QClipboard or file
                   },
           'FMT_ba': 4,      # number of digits for coefficient table
           'FMT_pz': 5,      # number of digits for Pole/Zero table
           'P_Marker': [mpl_ms, 'r'],  # size and color for poles' marker
           'Z_Marker': [mpl_ms, 'b'],  # size and color for zeros' marker
@@ -279,17 +279,16 @@
 
     QTextEdit{background-color: white;}
 
     QTableWidget{color:black; background-color:white;}
 
     .QTabWidget::pane{background-color: #F0F0F0;} /* background of tab content */
 
-    QLineEdit{background: white;
-                border-color: darkgrey;}
-    QLineEdit:disabled{background-color:lightgrey; color:blue}
+    QLineEdit{background: white; border-color: darkgrey;}
+    QLineEdit:disabled{background-color:lightgrey; color:blue;}
 
     QPushButton{
          background-color: qlineargradient(x1: 0, y1: 0, x2: 0, y2: 1,
                         stop: 0 white, stop: 0.5 lightgray, stop: 1.0 #C2C7CB);
                     }
     QPushButton:disabled{color:darkgrey; }
 
@@ -406,17 +405,22 @@
                 * [state="changed"]{background-color: yellow}
                 /* fully transparent background using white and alpha = 0 */
                 * [state="normal"]{background-color: rgba(255, 255, 255, 0)}
                 * [state="running"]{background-color: orange; color: white;}
                 * [state="highlight"]{background-color: rgba(173, 216, 230, 25%)}
                 * [state="unused"], *[state="u"]{background-color: white; color:darkgrey}
                 /* semi-transparent red */
-                * [state="failed"]{background-color: rgba(255, 0, 0, 50%); color:black}
+                * [state="failed"]{background-color: rgba(255, 0, 0, 50%); color:black;
+                    font-weight:800;}
 
                 QWidget{font-size:10pt; font-family: Tahoma;}
+
+                #large{font-size: 12pt; font-weight: bold; }
+                #xlarge{font-size: 14pt; font-weight: black;}
+
                 /* Frame with control elements of all plot widgets */
                 #frmControls{
                     border-top: solid darkgrey;
                     border-width: 2px;
                     margin: 0;
                     padding: 0;
                     }
@@ -438,14 +442,16 @@
                     /* background-color:lime; */
                     border: solid darkgrey;
                     border-width: 1px 0 0 0;
                     padding: 0;
                     margin: 0;
                     }
 
+                QWidget#transparent{background-color:none}
+
                 /* Dynamic filter subwidget */
                 #wdg_fil{
                     /*background-color:lightblue;*/
                     border: none;
                     padding: 5px 0 0 0;
                     }
 
@@ -481,17 +487,17 @@
                     x1: 0, y1: 0, x2: 0, y2: 1,
                     stop: 0 #cccccc, stop: 0.1 green, stop: 1.0 #444444);
                     color: white;}
 
                 QPushButton:pressed {background-color:black; color:white}
 
                 QPushButton:checked{
-                    background-color:lightblue; color:black;font-weight:800;}
+                    background-color:lightblue; color:black;font-weight: bold;}
                 QPushButtonRT:checked{
-                    background-color:lightblue; color:black;font-weight:800;}
+                    background-color:lightblue; color:black;font-weight: bold;}
 
                 QLineEdit{background-color:lightblue;
                                 /* border-style: outset; */
                                 border-width: 2px;}
 
                 /* QSplitter styling adopted from
                 http://stackoverflow.com/questions/6832499/qsplitter-show-a-divider-or-a-margin-between-the-two-widgets
```

### Comparing `pyfda-0.7.1/pyfda/pyfdax.py` & `pyfda-0.8.0a2/pyfda/pyfdax.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,14 +249,19 @@
         self.popMenu.exec_(self.loggerWin.mapToGlobal(point))
 
 # =============================================================================
     def closeEvent(self, event):
         """
         reimplement QMainWindow.closeEvent() to prompt the user
         """
+        # test for a handle to another pop-up window (CSV options) and close it,
+        # otherwise pyfda cannot be terminated and freezes
+        if not dirs.csv_options_handle is None:
+            dirs.csv_options_handle.close()
+
         reply = QMessageBox.question(self, 'Message',
             "Quit pyFDA?", QMessageBox.Yes, QMessageBox.No)
 
         if reply == QMessageBox.Yes:
             # Clear clipboard before exit to avoid error message on older Qt versions
             # "QClipboard: Unable to receive an event from the clipboard manager
             # in a reasonable time
```

### Comparing `pyfda-0.7.1/pyfda/qrc_resources.py` & `pyfda-0.8.0a2/pyfda/qrc_resources.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,184 +5,84 @@
 # Created by: The Resource Compiler for PyQt5 (Qt v5.15.2)
 #
 # WARNING! All changes made in this file will be lost!
 
 from PyQt5 import QtCore
 
 qt_resource_data = b"\
-\x00\x00\x00\xcb\
+\x00\x00\x00\xe3\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\
-\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\x69\
-\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\x38\
-\x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\
-\x22\x4d\x31\x32\x20\x33\x38\x68\x38\x56\x31\x30\x68\x2d\x38\x76\
-\x32\x38\x7a\x6d\x31\x36\x2d\x32\x38\x76\x32\x38\x68\x38\x56\x31\
-\x30\x68\x2d\x38\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\x77\x68\x69\
-\x74\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\
-\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x34\x38\x76\x34\x38\x48\x30\
-\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x2f\x3e\
-\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
-\x00\x00\x09\x82\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x20\x30\x63\
+\x2d\x31\x2e\x31\x20\x30\x2d\x32\x20\x2e\x39\x2d\x32\x20\x32\x76\
+\x31\x68\x2d\x31\x76\x34\x68\x36\x76\x2d\x34\x68\x2d\x31\x76\x2d\
+\x31\x63\x30\x2d\x31\x2e\x31\x2d\x2e\x39\x2d\x32\x2d\x32\x2d\x32\
+\x7a\x6d\x30\x20\x31\x63\x2e\x35\x36\x20\x30\x20\x31\x20\x2e\x34\
+\x34\x20\x31\x20\x31\x76\x31\x68\x2d\x32\x76\x2d\x31\x63\x30\x2d\
+\x2e\x35\x36\x2e\x34\x34\x2d\x31\x20\x31\x2d\x31\x7a\x22\x20\x74\
+\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\
+\x61\x74\x65\x28\x31\x29\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\
+\x67\x3e\
+\x00\x00\x02\x7d\
+\x00\
+\x00\x0c\x4f\x78\x9c\xad\x97\x4f\x6f\x9b\x30\x18\x87\xbf\x8a\xe5\
+\x5e\xb6\x43\x08\x36\xb6\xa1\x55\x88\xb4\xf6\x30\x0e\xab\x54\xad\
+\xd2\xa4\x1d\x51\x70\xb1\x37\x02\x0c\x88\x89\xf2\xe9\xf7\x9a\x26\
+\xcd\x9f\xc2\xa1\x8d\x0f\x96\x30\xbc\xfe\x3d\xf6\xf3\x82\xa2\x2c\
+\x5a\x93\xa3\xed\xba\x28\xdb\x18\xab\xae\xab\xef\xe6\xf3\xbe\xef\
+\xbd\x3e\xf0\xaa\x26\x9f\x53\xdf\xf7\xe7\x50\x81\x6d\xc9\x5d\x5b\
+\xa7\x2b\x19\xe3\xba\x91\xad\x6c\x8c\xc4\xa8\xd7\x59\xa7\x62\x1c\
+\xad\xd7\x18\x29\xa9\x73\xd5\xed\x27\x2f\xba\x28\x66\xcd\xa6\x80\
+\x6a\x69\x64\x59\x65\x19\x46\x6d\xd7\x54\x7f\xe5\xac\xd0\xa5\xfc\
+\x53\xe9\x32\xc6\x4d\xb5\x29\x8f\xf7\xf7\x59\x34\xf2\x28\xa5\x18\
+\x1d\x20\xdf\xda\x5a\xae\xba\x9f\x69\xa7\xab\x18\x6f\x1f\x75\xf6\
+\x1b\x06\x46\x46\x36\xad\xae\x20\x84\x78\x50\x6c\xb4\xec\xef\xab\
+\x6d\x8c\x7d\xe4\xa3\xc8\x1f\x06\x5e\x2e\x32\xf9\xd2\xa2\x55\x91\
+\xb6\x70\xb6\x87\x42\xd7\x4f\x69\xa7\xbe\x03\xb5\x86\x67\xab\xfd\
+\x1c\xe9\x2c\xc6\x29\xdc\xa8\xed\x04\xae\x1f\x21\x43\xc1\x7a\x03\
+\x23\xf1\x77\x78\xbe\x5c\xcc\x0f\xc5\x70\x69\x33\x97\x8b\xfc\x10\
+\xfb\x5c\xe8\x4c\x1e\x32\xcf\xef\x62\x64\x97\xcd\x6c\x6e\x8c\x37\
+\x4d\xf1\xe5\x26\xfd\x7a\x5a\xf4\x94\xe6\x72\x98\x5b\x59\x31\x2e\
+\xab\x72\x58\x32\x3c\x5b\x55\x6b\xaf\xdd\x94\x5e\xdb\xa5\x8d\x97\
+\x35\x69\xaf\xcb\xdc\xfb\x01\xe6\x9e\x55\x5a\xcb\xd3\xdd\xd2\xdb\
+\x08\xdd\x46\x8a\x04\x46\x90\x40\xcd\x48\xb0\x7b\x0b\xb9\xb7\x7e\
+\x61\x21\x98\xb1\xa7\x18\x96\xbc\xca\x8e\xf1\x0d\x34\xf6\x52\x3d\
+\x21\x78\x88\x0c\x7c\x86\x88\xcf\x8c\x80\x12\x7b\xfa\xfc\x23\x9b\
+\x7c\xd8\xb4\x5d\xb5\x7e\xbf\x4d\x81\x68\xa8\x42\xce\x4d\xc8\x59\
+\x42\xc5\x27\x76\x69\x5f\x9c\x55\x5a\xc7\xb8\xfd\xb7\x49\x1b\x39\
+\xf2\x42\xad\x75\x27\x9b\xcb\x53\x85\xd1\xeb\xa9\x98\x1f\xa0\x90\
+\x91\x44\xf0\x5f\x42\x28\x11\x0a\x23\x42\x9e\xc0\xdd\xdd\xc7\x0f\
+\x39\xda\x09\xe6\xbe\x13\xfc\xbc\x13\x6f\x28\x20\x41\xdf\x15\x70\
+\x0c\x09\x92\xdb\xe8\x7a\x52\x08\x24\xe8\x7b\x02\xb4\x4b\x12\x73\
+\x4f\xe2\x47\xd2\xab\xf8\x7d\xe6\xf1\x43\xba\xee\x9b\xf0\x29\x0a\
+\x38\x53\xdc\x10\x9f\xab\x19\xff\xfc\xa6\x19\xde\x07\x82\x1d\x2e\
+\x20\xee\xbc\x0f\x16\x44\x38\x75\x0b\x22\x9c\x8d\x82\xb8\x6b\x10\
+\x1f\x01\x31\xd7\xea\xd8\x84\x3a\xe6\x5a\x1d\x9b\x50\xc7\x5c\xab\
+\x63\x13\xea\x84\x6b\x75\x62\x42\x9d\x70\xad\x4e\x4c\xa8\x13\xae\
+\xd5\x89\x09\x75\xa0\x0d\x41\x9f\x14\x60\x0c\x4f\x60\x76\x35\x09\
+\xbc\x41\x22\x53\x97\x24\xf0\x76\x42\x82\xd9\xd5\x24\x32\xec\xfd\
+\x3d\x89\x9f\x91\xb8\x03\x12\x9f\x20\x59\x7b\xd4\xb9\x3d\x3a\x61\
+\x8f\x3a\xb7\x37\x46\xe2\x67\x24\x57\xf6\xc6\x48\xd6\x9e\x70\x6e\
+\x4f\x4c\xd8\x13\xce\xed\x8d\x91\xf8\x19\xc9\x95\xbd\x13\x92\xfd\
+\xd5\x7e\x37\xe0\x7f\xc2\xf2\x3f\x6a\x77\xb2\xf8\
+\x00\x00\x00\x8b\
 \x3c\
-\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
-\x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\x55\x54\x46\
-\x2d\x38\x22\x3f\x3e\x0d\x0a\x3c\x21\x44\x4f\x43\x54\x59\x50\x45\
-\x20\x73\x76\x67\x20\x20\x50\x55\x42\x4c\x49\x43\x20\x27\x2d\x2f\
-\x2f\x57\x33\x43\x2f\x2f\x44\x54\x44\x20\x53\x56\x47\x20\x31\x2e\
-\x31\x2f\x2f\x45\x4e\x27\x20\x20\x27\x68\x74\x74\x70\x3a\x2f\x2f\
-\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x47\x72\x61\x70\x68\
-\x69\x63\x73\x2f\x53\x56\x47\x2f\x31\x2e\x31\x2f\x44\x54\x44\x2f\
-\x73\x76\x67\x31\x31\x2e\x64\x74\x64\x27\x3e\x0d\x0a\x3c\x73\x76\
-\x67\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\
-\x20\x66\x69\x6c\x6c\x2d\x72\x75\x6c\x65\x3d\x22\x65\x76\x65\x6e\
-\x6f\x64\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\
-\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\x72\
-\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x38\x2e\x32\x32\
-\x32\x22\x20\x70\x72\x65\x73\x65\x72\x76\x65\x41\x73\x70\x65\x63\
-\x74\x52\x61\x74\x69\x6f\x3d\x22\x78\x4d\x69\x64\x59\x4d\x69\x64\
-\x22\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\x32\x22\x20\
-\x76\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x34\x37\
-\x20\x38\x34\x37\x22\x20\x78\x6d\x6c\x3a\x73\x70\x61\x63\x65\x3d\
-\x22\x70\x72\x65\x73\x65\x72\x76\x65\x22\x20\x78\x6d\x6c\x6e\x73\
-\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\
-\x6f\x72\x67\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\x20\x78\x6d\
-\x6c\x6e\x73\x3a\x6f\x6f\x6f\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\
-\x78\x6d\x6c\x2e\x6f\x70\x65\x6e\x6f\x66\x66\x69\x63\x65\x2e\x6f\
-\x72\x67\x2f\x73\x76\x67\x2f\x65\x78\x70\x6f\x72\x74\x22\x3e\x0d\
-\x0a\x20\x3c\x64\x65\x66\x73\x20\x63\x6c\x61\x73\x73\x3d\x22\x43\
-\x6c\x69\x70\x50\x61\x74\x68\x47\x72\x6f\x75\x70\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x63\x6c\x69\x70\x50\x61\x74\x68\x20\x69\x64\x3d\x22\
-\x70\x72\x65\x73\x65\x6e\x74\x61\x74\x69\x6f\x6e\x5f\x63\x6c\x69\
-\x70\x5f\x70\x61\x74\x68\x22\x3e\x0d\x0a\x20\x20\x20\x3c\x72\x65\
-\x63\x74\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x34\x37\x22\x20\x68\
-\x65\x69\x67\x68\x74\x3d\x22\x38\x34\x37\x22\x2f\x3e\x0d\x0a\x20\
-\x20\x3c\x2f\x63\x6c\x69\x70\x50\x61\x74\x68\x3e\x0d\x0a\x20\x20\
-\x0d\x0a\x20\x3c\x2f\x64\x65\x66\x73\x3e\x0d\x0a\x20\x3c\x64\x65\
-\x66\x73\x20\x63\x6c\x61\x73\x73\x3d\x22\x54\x65\x78\x74\x53\x68\
-\x61\x70\x65\x49\x6e\x64\x65\x78\x22\x3e\x0d\x0a\x20\x20\x0d\x0a\
-\x20\x3c\x2f\x64\x65\x66\x73\x3e\x0d\x0a\x20\x3c\x64\x65\x66\x73\
-\x20\x63\x6c\x61\x73\x73\x3d\x22\x45\x6d\x62\x65\x64\x64\x65\x64\
-\x42\x75\x6c\x6c\x65\x74\x43\x68\x61\x72\x73\x22\x3e\x0d\x0a\x20\
-\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x20\x0d\x0a\x20\
-\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x20\x0d\x0a\x20\
-\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x3c\x2f\x64\x65\x66\x73\x3e\x0d\
-\x0a\x20\x0d\x0a\x20\x0d\x0a\x20\x20\x3c\x67\x20\x69\x64\x3d\x22\
-\x69\x64\x32\x22\x20\x63\x6c\x61\x73\x73\x3d\x22\x4d\x61\x73\x74\
-\x65\x72\x5f\x53\x6c\x69\x64\x65\x22\x3e\x0d\x0a\x20\x20\x20\x0d\
-\x0a\x20\x20\x20\x0d\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x0d\
-\x0a\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x53\x6c\x69\x64\
-\x65\x47\x72\x6f\x75\x70\x22\x3e\x0d\x0a\x20\x20\x0d\x0a\x20\x20\
-\x20\x3c\x67\x20\x69\x64\x3d\x22\x63\x6f\x6e\x74\x61\x69\x6e\x65\
-\x72\x2d\x69\x64\x31\x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x67\x20\
-\x69\x64\x3d\x22\x69\x64\x31\x22\x20\x63\x6c\x61\x73\x73\x3d\x22\
-\x53\x6c\x69\x64\x65\x22\x20\x63\x6c\x69\x70\x2d\x70\x61\x74\x68\
-\x3d\x22\x75\x72\x6c\x28\x23\x70\x72\x65\x73\x65\x6e\x74\x61\x74\
-\x69\x6f\x6e\x5f\x63\x6c\x69\x70\x5f\x70\x61\x74\x68\x29\x22\x3e\
-\x0d\x0a\x20\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\
-\x22\x50\x61\x67\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\
-\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\
-\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x4c\x69\
-\x6e\x65\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x33\x22\x20\x66\x69\
-\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\
-\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\x3d\
-\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x78\x3d\
-\x22\x32\x39\x34\x22\x20\x79\x3d\x22\x39\x34\x22\x20\x77\x69\x64\
-\x74\x68\x3d\x22\x31\x33\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\
-\x36\x31\x33\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x20\
-\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x6d\x33\x30\x30\x20\x31\x30\
-\x30\x76\x36\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x23\
-\x30\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\
-\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\x72\
-\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x31\x31\x22\x2f\x3e\
-\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\
-\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\
-\x43\x75\x73\x74\x6f\x6d\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x20\x20\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x34\
-\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\
-\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\
-\x22\x20\x78\x3d\x22\x32\x32\x22\x20\x79\x3d\x22\x32\x33\x22\x20\
-\x77\x69\x64\x74\x68\x3d\x22\x37\x35\x35\x22\x20\x68\x65\x69\x67\
-\x68\x74\x3d\x22\x37\x35\x34\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\
-\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x6d\x33\x39\
-\x39\x20\x37\x33\x37\x68\x2d\x33\x33\x38\x76\x2d\x36\x37\x35\x68\
-\x36\x37\x36\x76\x36\x37\x35\x68\x2d\x33\x33\x38\x7a\x22\x20\x73\
-\x74\x72\x6f\x6b\x65\x3d\x22\x23\x30\x30\x30\x22\x20\x73\x74\x72\
-\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x63\x61\x70\x3d\x22\x73\x71\x75\
-\x61\x72\x65\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\
-\x6a\x6f\x69\x6e\x3d\x22\x6d\x69\x74\x65\x72\x22\x20\x73\x74\x72\
-\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x37\x38\x22\x2f\x3e\
-\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\
-\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\
-\x50\x6f\x6c\x79\x50\x6f\x6c\x79\x67\x6f\x6e\x53\x68\x61\x70\x65\
-\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x67\x20\x69\x64\
-\x3d\x22\x69\x64\x35\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\
-\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\
-\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x77\x69\x64\x74\x68\
-\x3d\x22\x38\x34\x39\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\
-\x34\x39\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x2f\
-\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\
-\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\
-\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\
-\x2e\x4c\x69\x6e\x65\x53\x68\x61\x70\x65\x22\x20\x66\x69\x6c\x6c\
-\x3d\x22\x6e\x6f\x6e\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\
-\x20\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x36\x22\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\
-\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\
-\x20\x78\x3d\x22\x34\x39\x34\x22\x20\x79\x3d\x22\x39\x34\x22\x20\
-\x77\x69\x64\x74\x68\x3d\x22\x31\x33\x22\x20\x68\x65\x69\x67\x68\
-\x74\x3d\x22\x36\x31\x33\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x6d\x35\x30\x30\
-\x20\x31\x30\x30\x76\x36\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\
-\x3d\x22\x23\x30\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\
-\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\
-\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x31\x31\
-\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\
-\x0d\x0a\x20\x20\x20\x20\x20\x20\x0d\x0a\x20\x20\x20\x20\x20\x20\
-\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x67\x20\x69\x64\x3d\x22\
-\x69\x64\x37\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x3c\
-\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\
-\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x78\x3d\x22\x39\x34\x22\x20\
-\x79\x3d\x22\x32\x39\x34\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x36\
-\x31\x33\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x31\x33\x22\x2f\
-\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x70\x61\x74\x68\
-\x20\x64\x3d\x22\x6d\x37\x30\x30\x20\x33\x30\x30\x68\x2d\x36\x30\
-\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x23\x30\x30\x30\x22\
-\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\
-\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
-\x77\x69\x64\x74\x68\x3d\x22\x31\x31\x22\x2f\x3e\x0d\x0a\x20\x20\
-\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x0d\x0a\x20\x20\x20\x20\x20\x20\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x38\x22\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\
-\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\
-\x22\x20\x78\x3d\x22\x39\x34\x22\x20\x79\x3d\x22\x34\x39\x34\x22\
-\x20\x77\x69\x64\x74\x68\x3d\x22\x36\x31\x33\x22\x20\x68\x65\x69\
-\x67\x68\x74\x3d\x22\x31\x33\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\
-\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x6d\x37\x30\
-\x30\x20\x35\x30\x30\x68\x2d\x36\x30\x30\x22\x20\x73\x74\x72\x6f\
-\x6b\x65\x3d\x22\x23\x30\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\
-\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\
-\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\
-\x31\x31\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\
-\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x3c\
-\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\
-\x0d\x0a\x20\x3c\x2f\x67\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\
-\x0a\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x76\
+\x38\x68\x37\x76\x2d\x34\x68\x2d\x34\x76\x2d\x34\x68\x2d\x33\x7a\
+\x6d\x34\x20\x30\x76\x33\x68\x33\x6c\x2d\x33\x2d\x33\x7a\x22\x20\
+\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
 \x00\x00\x03\x4c\
 \xef\
 \xbb\xbf\x3c\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\
 \x22\x31\x2e\x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\
 \x75\x74\x66\x2d\x38\x22\x3f\x3e\x0d\x0a\x3c\x21\x44\x4f\x43\x54\
 \x59\x50\x45\x20\x73\x76\x67\x20\x50\x55\x42\x4c\x49\x43\x20\x22\
 \x2d\x2f\x2f\x57\x33\x43\x2f\x2f\x44\x54\x44\x20\x53\x56\x47\x20\
@@ -230,230 +130,43 @@
 \x35\x4c\x20\x33\x34\x2e\x35\x2c\x33\x32\x4c\x20\x32\x37\x2e\x35\
 \x2c\x33\x39\x4c\x20\x32\x32\x2e\x35\x2c\x33\x39\x4c\x20\x32\x37\
 \x2e\x35\x2c\x33\x34\x4c\x20\x31\x39\x2e\x35\x35\x2c\x33\x34\x4c\
 \x20\x31\x39\x2e\x35\x35\x2c\x33\x30\x20\x5a\x0d\x0a\x09\x20\x22\
 \x20\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\
 \x73\x6c\x61\x74\x65\x28\x2d\x31\x37\x20\x2d\x31\x37\x29\x22\x2f\
 \x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
-\x00\x00\x01\x6b\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
-\x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x01\x01\x01\x0a\x0d\
-\x0e\x14\x19\x1a\x29\x33\x36\x3c\x4c\x51\x4a\x59\x5f\x5f\x70\x75\
-\x6b\x85\x8e\x76\x94\x9e\x81\xa2\xac\x96\xb1\xba\xcb\xcd\xce\xac\
-\xd7\xe5\xad\xd8\xe6\xa1\xc9\xd6\x5a\xda\xbc\xfc\x00\x00\x00\xf6\
-\x49\x44\x41\x54\x28\xcf\xad\xd0\x4d\x0a\x41\x51\x14\x07\xf0\xbf\
-\x47\xc9\x40\xc9\x06\x88\x09\x43\x4c\x94\x42\x16\x20\x59\x81\x15\
-\x48\x86\x46\x7a\x0b\x90\xa9\x89\xa9\xba\x03\x1b\x90\x81\x29\x32\
-\xb2\x00\xf2\x7c\xd7\x95\x0d\xc8\x79\xf7\x3e\x1c\x1f\x65\xc0\x7f\
-\xf2\x5e\xbf\x7b\xba\xe7\x9c\x8b\x29\x65\x32\x98\xf2\x60\x26\xa5\
-\x99\x30\x52\x7d\xf9\x08\x99\x15\x06\x90\x7e\xb6\x12\x11\x8c\x16\
-\xb7\xad\x5d\x06\x64\xb8\x2d\x15\xc1\xc3\xcd\xd4\xe6\xbe\x30\xab\
-\x68\x33\xfa\xcc\x4a\x4e\x5d\xf7\x4b\x1d\xbf\xef\xd8\x19\x2a\x5b\
-\x3c\xfa\xee\x92\xd1\x48\x55\xcd\x17\xb8\xcf\x57\xa0\x6f\xf0\x62\
-\xef\x91\xbf\xed\x61\xa9\xc3\xdc\x7d\xdf\x18\x95\x95\xf5\xc5\xb6\
-\xc9\x3a\xfd\x50\xd7\xa3\x5e\xd2\x68\xd9\xb6\x07\x7c\x54\xb6\xd1\
-\xcd\x50\x64\x66\x39\xe6\xff\x60\x19\x66\x2b\xc7\x42\xcc\xd6\x8e\
-\x65\x99\x1d\x74\x5f\x57\x95\x99\x1e\x9e\x16\xe7\x76\x56\x16\x97\
-\xdc\x4e\x01\xfd\x66\xdc\xe4\x3c\xac\xde\xe2\xc9\x64\x13\xe8\xbe\
-\x5a\xfb\x77\x1b\x0b\xd1\x03\xbc\x42\xa5\x06\x34\x84\xc0\x08\xef\
-\xf9\xb7\x8d\xc5\x5b\xae\x6f\xd7\x4f\x6c\x5a\x3f\xe0\x76\x00\x00\
-\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-\x00\x00\x03\xf6\
-\xef\
-\xbb\xbf\x3c\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\
-\x22\x31\x2e\x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\
-\x75\x74\x66\x2d\x38\x22\x3f\x3e\x0d\x0a\x3c\x21\x44\x4f\x43\x54\
-\x59\x50\x45\x20\x73\x76\x67\x20\x50\x55\x42\x4c\x49\x43\x20\x22\
-\x2d\x2f\x2f\x57\x33\x43\x2f\x2f\x44\x54\x44\x20\x53\x56\x47\x20\
-\x31\x2e\x31\x2f\x2f\x45\x4e\x22\x20\x22\x68\x74\x74\x70\x3a\x2f\
-\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x47\x72\x61\x70\
-\x68\x69\x63\x73\x2f\x53\x56\x47\x2f\x31\x2e\x31\x2f\x44\x54\x44\
-\x2f\x73\x76\x67\x31\x31\x2e\x64\x74\x64\x22\x3e\x0d\x0a\x3c\x73\
-\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\x2f\
-\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\
-\x2f\x73\x76\x67\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x78\x6c\x69\x6e\
-\x6b\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\
-\x2e\x6f\x72\x67\x2f\x31\x39\x39\x39\x2f\x78\x6c\x69\x6e\x6b\x22\
-\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\x31\x22\x20\x62\
-\x61\x73\x65\x50\x72\x6f\x66\x69\x6c\x65\x3d\x22\x66\x75\x6c\x6c\
-\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x30\x22\x20\x68\x65\x69\
-\x67\x68\x74\x3d\x22\x33\x35\x22\x20\x76\x69\x65\x77\x42\x6f\x78\
-\x3d\x22\x30\x20\x30\x20\x34\x30\x2e\x30\x30\x20\x33\x35\x2e\x30\
-\x30\x22\x20\x65\x6e\x61\x62\x6c\x65\x2d\x62\x61\x63\x6b\x67\x72\
-\x6f\x75\x6e\x64\x3d\x22\x6e\x65\x77\x20\x30\x20\x30\x20\x34\x30\
-\x2e\x30\x30\x20\x33\x35\x2e\x30\x30\x22\x20\x78\x6d\x6c\x3a\x73\
-\x70\x61\x63\x65\x3d\x22\x70\x72\x65\x73\x65\x72\x76\x65\x22\x3e\
-\x0d\x0a\x09\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x23\
-\x30\x30\x30\x30\x30\x30\x22\x20\x66\x69\x6c\x6c\x2d\x6f\x70\x61\
-\x63\x69\x74\x79\x3d\x22\x31\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
-\x77\x69\x64\x74\x68\x3d\x22\x30\x2e\x32\x22\x20\x73\x74\x72\x6f\
-\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\
-\x6e\x64\x22\x20\x64\x3d\x22\x4d\x20\x33\x37\x2e\x39\x31\x36\x37\
-\x2c\x31\x35\x2e\x38\x33\x33\x33\x43\x20\x34\x30\x2e\x31\x30\x32\
-\x38\x2c\x31\x35\x2e\x38\x33\x33\x33\x20\x34\x32\x2e\x32\x35\x2c\
-\x31\x37\x2e\x38\x31\x33\x39\x20\x34\x32\x2e\x32\x35\x2c\x32\x30\
-\x4c\x20\x34\x32\x2c\x32\x31\x4c\x20\x35\x34\x2c\x32\x31\x4c\x20\
-\x35\x34\x2c\x35\x37\x4c\x20\x32\x32\x2c\x35\x37\x4c\x20\x32\x32\
-\x2c\x32\x31\x4c\x20\x33\x34\x2c\x32\x31\x4c\x20\x33\x33\x2e\x37\
-\x35\x2c\x32\x30\x43\x20\x33\x33\x2e\x37\x35\x2c\x31\x37\x2e\x38\
-\x31\x33\x39\x20\x33\x35\x2e\x37\x33\x30\x35\x2c\x31\x35\x2e\x38\
-\x33\x33\x33\x20\x33\x37\x2e\x39\x31\x36\x37\x2c\x31\x35\x2e\x38\
-\x33\x33\x33\x20\x5a\x20\x4d\x20\x35\x31\x2c\x32\x34\x4c\x20\x34\
-\x35\x2e\x35\x2c\x32\x34\x4c\x20\x34\x37\x2e\x35\x2c\x32\x38\x4c\
-\x20\x32\x38\x2e\x35\x2c\x32\x38\x4c\x20\x33\x30\x2e\x35\x2c\x32\
-\x34\x4c\x20\x32\x35\x2c\x32\x34\x4c\x20\x32\x35\x2c\x35\x34\x4c\
-\x20\x35\x31\x2c\x35\x34\x4c\x20\x35\x31\x2c\x32\x34\x20\x5a\x20\
-\x4d\x20\x33\x37\x2e\x39\x31\x36\x36\x2c\x31\x38\x2e\x32\x30\x38\
-\x34\x43\x20\x33\x37\x2e\x30\x34\x32\x32\x2c\x31\x38\x2e\x32\x30\
-\x38\x34\x20\x33\x36\x2c\x31\x38\x2e\x38\x37\x35\x36\x20\x33\x36\
-\x2c\x31\x39\x2e\x37\x35\x43\x20\x33\x36\x2c\x32\x30\x2e\x30\x33\
-\x38\x34\x20\x33\x36\x2e\x33\x36\x35\x33\x2c\x32\x30\x2e\x37\x36\
-\x37\x31\x20\x33\x36\x2e\x35\x2c\x32\x31\x4c\x20\x33\x39\x2e\x35\
-\x2c\x32\x31\x43\x20\x33\x39\x2e\x36\x33\x34\x37\x2c\x32\x30\x2e\
-\x37\x36\x37\x31\x20\x34\x30\x2c\x32\x30\x2e\x30\x33\x38\x34\x20\
-\x34\x30\x2c\x31\x39\x2e\x37\x35\x43\x20\x34\x30\x2c\x31\x38\x2e\
-\x38\x37\x35\x36\x20\x33\x38\x2e\x37\x39\x31\x31\x2c\x31\x38\x2e\
-\x32\x30\x38\x34\x20\x33\x37\x2e\x39\x31\x36\x36\x2c\x31\x38\x2e\
-\x32\x30\x38\x34\x20\x5a\x20\x0d\x0a\x4d\x20\x34\x33\x2e\x35\x35\
-\x2c\x34\x30\x4c\x20\x36\x31\x2e\x35\x2c\x34\x30\x4c\x20\x35\x34\
-\x2e\x35\x2c\x33\x35\x4c\x20\x36\x31\x2e\x35\x2c\x33\x35\x4c\x20\
-\x36\x38\x2e\x35\x2c\x34\x32\x4c\x20\x36\x31\x2e\x35\x2c\x34\x39\
-\x4c\x20\x35\x34\x2e\x35\x2c\x34\x39\x4c\x20\x36\x31\x2e\x35\x2c\
-\x34\x34\x4c\x20\x34\x33\x2e\x35\x35\x2c\x34\x34\x4c\x20\x34\x33\
-\x2e\x35\x35\x2c\x34\x30\x20\x5a\x22\x0d\x0a\x74\x72\x61\x6e\x73\
-\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\x61\x74\x65\x28\
-\x2d\x32\x38\x20\x2d\x31\x36\x29\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\
-\x76\x67\x3e\x0d\x0a\
-\x00\x00\x03\xf6\
-\xef\
-\xbb\xbf\x3c\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\
-\x22\x31\x2e\x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\
-\x75\x74\x66\x2d\x38\x22\x3f\x3e\x0d\x0a\x3c\x21\x44\x4f\x43\x54\
-\x59\x50\x45\x20\x73\x76\x67\x20\x50\x55\x42\x4c\x49\x43\x20\x22\
-\x2d\x2f\x2f\x57\x33\x43\x2f\x2f\x44\x54\x44\x20\x53\x56\x47\x20\
-\x31\x2e\x31\x2f\x2f\x45\x4e\x22\x20\x22\x68\x74\x74\x70\x3a\x2f\
-\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x47\x72\x61\x70\
-\x68\x69\x63\x73\x2f\x53\x56\x47\x2f\x31\x2e\x31\x2f\x44\x54\x44\
-\x2f\x73\x76\x67\x31\x31\x2e\x64\x74\x64\x22\x3e\x0d\x0a\x3c\x73\
-\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\x2f\
-\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\
-\x2f\x73\x76\x67\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x78\x6c\x69\x6e\
-\x6b\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\
-\x2e\x6f\x72\x67\x2f\x31\x39\x39\x39\x2f\x78\x6c\x69\x6e\x6b\x22\
-\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\x31\x22\x20\x62\
-\x61\x73\x65\x50\x72\x6f\x66\x69\x6c\x65\x3d\x22\x66\x75\x6c\x6c\
-\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x33\x37\x22\x20\x68\x65\x69\
-\x67\x68\x74\x3d\x22\x33\x35\x22\x20\x76\x69\x65\x77\x42\x6f\x78\
-\x3d\x22\x30\x20\x30\x20\x33\x37\x2e\x30\x30\x20\x33\x35\x2e\x30\
-\x30\x22\x20\x65\x6e\x61\x62\x6c\x65\x2d\x62\x61\x63\x6b\x67\x72\
-\x6f\x75\x6e\x64\x3d\x22\x6e\x65\x77\x20\x30\x20\x30\x20\x33\x37\
-\x2e\x30\x30\x20\x33\x35\x2e\x30\x30\x22\x20\x78\x6d\x6c\x3a\x73\
-\x70\x61\x63\x65\x3d\x22\x70\x72\x65\x73\x65\x72\x76\x65\x22\x3e\
-\x0d\x0a\x09\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x23\
-\x30\x30\x30\x30\x30\x30\x22\x20\x66\x69\x6c\x6c\x2d\x6f\x70\x61\
-\x63\x69\x74\x79\x3d\x22\x31\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
-\x77\x69\x64\x74\x68\x3d\x22\x30\x2e\x32\x22\x20\x73\x74\x72\x6f\
-\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\
-\x6e\x64\x22\x20\x64\x3d\x22\x4d\x20\x33\x37\x2e\x39\x31\x36\x37\
-\x2c\x31\x35\x2e\x38\x33\x33\x33\x43\x20\x34\x30\x2e\x31\x30\x32\
-\x38\x2c\x31\x35\x2e\x38\x33\x33\x33\x20\x34\x32\x2e\x32\x35\x2c\
-\x31\x37\x2e\x38\x31\x33\x39\x20\x34\x32\x2e\x32\x35\x2c\x32\x30\
-\x4c\x20\x34\x32\x2c\x32\x31\x4c\x20\x35\x34\x2c\x32\x31\x4c\x20\
-\x35\x34\x2c\x35\x37\x4c\x20\x32\x32\x2c\x35\x37\x4c\x20\x32\x32\
-\x2c\x32\x31\x4c\x20\x33\x34\x2c\x32\x31\x4c\x20\x33\x33\x2e\x37\
-\x35\x2c\x32\x30\x43\x20\x33\x33\x2e\x37\x35\x2c\x31\x37\x2e\x38\
-\x31\x33\x39\x20\x33\x35\x2e\x37\x33\x30\x35\x2c\x31\x35\x2e\x38\
-\x33\x33\x33\x20\x33\x37\x2e\x39\x31\x36\x37\x2c\x31\x35\x2e\x38\
-\x33\x33\x33\x20\x5a\x20\x4d\x20\x35\x31\x2c\x32\x34\x4c\x20\x34\
-\x35\x2e\x35\x2c\x32\x34\x4c\x20\x34\x37\x2e\x35\x2c\x32\x38\x4c\
-\x20\x32\x38\x2e\x35\x2c\x32\x38\x4c\x20\x33\x30\x2e\x35\x2c\x32\
-\x34\x4c\x20\x32\x35\x2c\x32\x34\x4c\x20\x32\x35\x2c\x35\x34\x4c\
-\x20\x35\x31\x2c\x35\x34\x4c\x20\x35\x31\x2c\x32\x34\x20\x5a\x20\
-\x4d\x20\x33\x37\x2e\x39\x31\x36\x36\x2c\x31\x38\x2e\x32\x30\x38\
-\x34\x43\x20\x33\x37\x2e\x30\x34\x32\x32\x2c\x31\x38\x2e\x32\x30\
-\x38\x34\x20\x33\x36\x2c\x31\x38\x2e\x38\x37\x35\x36\x20\x33\x36\
-\x2c\x31\x39\x2e\x37\x35\x43\x20\x33\x36\x2c\x32\x30\x2e\x30\x33\
-\x38\x34\x20\x33\x36\x2e\x33\x36\x35\x33\x2c\x32\x30\x2e\x37\x36\
-\x37\x31\x20\x33\x36\x2e\x35\x2c\x32\x31\x4c\x20\x33\x39\x2e\x35\
-\x2c\x32\x31\x43\x20\x33\x39\x2e\x36\x33\x34\x37\x2c\x32\x30\x2e\
-\x37\x36\x37\x31\x20\x34\x30\x2c\x32\x30\x2e\x30\x33\x38\x34\x20\
-\x34\x30\x2c\x31\x39\x2e\x37\x35\x43\x20\x34\x30\x2c\x31\x38\x2e\
-\x38\x37\x35\x36\x20\x33\x38\x2e\x37\x39\x31\x31\x2c\x31\x38\x2e\
-\x32\x30\x38\x34\x20\x33\x37\x2e\x39\x31\x36\x36\x2c\x31\x38\x2e\
-\x32\x30\x38\x34\x20\x5a\x20\x0d\x0a\x4d\x20\x31\x34\x2e\x35\x35\
-\x2c\x34\x30\x4c\x20\x33\x32\x2e\x35\x2c\x34\x30\x4c\x20\x32\x35\
-\x2e\x35\x2c\x33\x35\x4c\x20\x33\x32\x2e\x35\x2c\x33\x35\x4c\x20\
-\x33\x39\x2e\x35\x2c\x34\x32\x4c\x20\x33\x32\x2e\x35\x2c\x34\x39\
-\x4c\x20\x32\x35\x2e\x35\x2c\x34\x39\x4c\x20\x33\x32\x2e\x35\x2c\
-\x34\x34\x4c\x20\x31\x34\x2e\x35\x35\x2c\x34\x34\x4c\x20\x31\x34\
-\x2e\x35\x35\x2c\x34\x30\x20\x5a\x22\x0d\x0a\x74\x72\x61\x6e\x73\
-\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\x61\x74\x65\x28\
-\x2d\x31\x32\x20\x2d\x31\x37\x29\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\
-\x76\x67\x3e\x0d\x0a\
-\x00\x00\x01\x62\
+\x00\x00\x00\xcb\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\
 \x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\x69\
 \x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\x38\
 \x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\
-\x22\x4d\x36\x20\x31\x38\x76\x31\x32\x68\x38\x6c\x31\x30\x20\x31\
-\x30\x56\x38\x4c\x31\x34\x20\x31\x38\x48\x36\x7a\x6d\x32\x37\x20\
-\x36\x63\x30\x2d\x33\x2e\x35\x33\x2d\x32\x2e\x30\x34\x2d\x36\x2e\
-\x35\x38\x2d\x35\x2d\x38\x2e\x30\x35\x76\x31\x36\x2e\x31\x31\x63\
-\x32\x2e\x39\x36\x2d\x31\x2e\x34\x38\x20\x35\x2d\x34\x2e\x35\x33\
-\x20\x35\x2d\x38\x2e\x30\x36\x7a\x4d\x32\x38\x20\x36\x2e\x34\x36\
-\x76\x34\x2e\x31\x33\x63\x35\x2e\x37\x38\x20\x31\x2e\x37\x32\x20\
-\x31\x30\x20\x37\x2e\x30\x37\x20\x31\x30\x20\x31\x33\x2e\x34\x31\
-\x73\x2d\x34\x2e\x32\x32\x20\x31\x31\x2e\x36\x39\x2d\x31\x30\x20\
-\x31\x33\x2e\x34\x31\x76\x34\x2e\x31\x33\x63\x38\x2e\x30\x31\x2d\
-\x31\x2e\x38\x32\x20\x31\x34\x2d\x38\x2e\x39\x37\x20\x31\x34\x2d\
-\x31\x37\x2e\x35\x34\x53\x33\x36\x2e\x30\x31\x20\x38\x2e\x32\x38\
-\x20\x32\x38\x20\x36\x2e\x34\x36\x7a\x22\x2f\x3e\x0d\x0a\x20\x20\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\
-\x34\x38\x76\x34\x38\x48\x30\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\
-\x6e\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\
-\x0a\
-\x00\x00\x01\xf7\
+\x22\x4d\x31\x32\x20\x33\x38\x68\x38\x56\x31\x30\x68\x2d\x38\x76\
+\x32\x38\x7a\x6d\x31\x36\x2d\x32\x38\x76\x32\x38\x68\x38\x56\x31\
+\x30\x68\x2d\x38\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\x77\x68\x69\
+\x74\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\
+\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x34\x38\x76\x34\x38\x48\x30\
+\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x2f\x3e\
+\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
+\x00\x00\x00\xb4\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
 \x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
 \x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x34\x2e\x30\x39\
-\x20\x30\x63\x2d\x2e\x30\x35\x20\x30\x2d\x2e\x31\x2e\x30\x34\x2d\
-\x2e\x31\x33\x2e\x30\x39\x6c\x2d\x2e\x39\x34\x20\x31\x2e\x38\x31\
-\x63\x2d\x2e\x30\x32\x2e\x30\x35\x2d\x2e\x30\x37\x2e\x30\x39\x2d\
-\x2e\x31\x33\x2e\x30\x39\x68\x2d\x31\x2e\x34\x31\x63\x2d\x2e\x38\
-\x33\x20\x30\x2d\x31\x2e\x35\x2e\x36\x37\x2d\x31\x2e\x35\x20\x31\
-\x2e\x35\x76\x34\x2e\x34\x31\x63\x30\x20\x2e\x30\x35\x2e\x30\x34\
-\x2e\x30\x39\x2e\x30\x39\x2e\x30\x39\x68\x37\x2e\x38\x31\x63\x2e\
-\x30\x35\x20\x30\x20\x2e\x30\x39\x2d\x2e\x30\x34\x2e\x30\x39\x2d\
-\x2e\x30\x39\x76\x2d\x35\x2e\x38\x31\x63\x30\x2d\x2e\x30\x36\x2d\
-\x2e\x30\x34\x2d\x2e\x30\x39\x2d\x2e\x30\x39\x2d\x2e\x30\x39\x68\
-\x2d\x2e\x38\x31\x63\x2d\x2e\x30\x35\x20\x30\x2d\x2e\x31\x2d\x2e\
-\x30\x34\x2d\x2e\x31\x33\x2d\x2e\x30\x39\x6c\x2d\x2e\x39\x34\x2d\
-\x31\x2e\x38\x31\x63\x2d\x2e\x30\x33\x2d\x2e\x30\x35\x2d\x2e\x30\
-\x37\x2d\x2e\x30\x39\x2d\x2e\x31\x33\x2d\x2e\x30\x39\x68\x2d\x31\
-\x2e\x38\x31\x7a\x6d\x2d\x32\x2e\x35\x39\x20\x33\x63\x2e\x32\x38\
-\x20\x30\x20\x2e\x35\x2e\x32\x32\x2e\x35\x2e\x35\x73\x2d\x2e\x32\
-\x32\x2e\x35\x2d\x2e\x35\x2e\x35\x2d\x2e\x35\x2d\x2e\x32\x32\x2d\
-\x2e\x35\x2d\x2e\x35\x2e\x32\x32\x2d\x2e\x35\x2e\x35\x2d\x2e\x35\
-\x7a\x6d\x33\x2e\x35\x20\x30\x63\x31\x2e\x31\x20\x30\x20\x32\x20\
-\x2e\x39\x20\x32\x20\x32\x73\x2d\x2e\x39\x20\x32\x2d\x32\x20\x32\
-\x2d\x32\x2d\x2e\x39\x2d\x32\x2d\x32\x20\x2e\x39\x2d\x32\x20\x32\
-\x2d\x32\x7a\x6d\x30\x20\x31\x63\x2d\x2e\x35\x35\x20\x30\x2d\x31\
-\x20\x2e\x34\x35\x2d\x31\x20\x31\x73\x2e\x34\x35\x20\x31\x20\x31\
-\x20\x31\x20\x31\x2d\x2e\x34\x35\x20\x31\x2d\x31\x2d\x2e\x34\x35\
-\x2d\x31\x2d\x31\x2d\x31\x7a\x22\x0d\x0a\x20\x20\x2f\x3e\x0d\x0a\
-\x3c\x2f\x73\x76\x67\x3e\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x32\x20\x30\x76\
+\x36\x68\x2d\x32\x6c\x32\x2e\x35\x20\x32\x20\x32\x2e\x35\x2d\x32\
+\x68\x2d\x32\x76\x2d\x36\x68\x2d\x31\x7a\x6d\x32\x20\x30\x76\x31\
+\x68\x32\x76\x2d\x31\x68\x2d\x32\x7a\x6d\x30\x20\x32\x76\x31\x68\
+\x33\x76\x2d\x31\x68\x2d\x33\x7a\x6d\x30\x20\x32\x76\x31\x68\x34\
+\x76\x2d\x31\x68\x2d\x34\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\
+\x76\x67\x3e\
 \x00\x00\x01\xa4\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
 \x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x61\x79\x81\x21\x29\
 \x2c\x97\xbc\xc8\xc0\xc0\xc0\x41\x52\x58\x89\xac\xb7\x0c\x0f\x0f\
 \xad\xd8\xe6\xcb\xcd\xce\x2f\x3b\x3f\x55\x68\x6e\xa7\xaa\xab\x16\
@@ -475,57 +188,156 @@
 \xe6\x4b\x60\xdd\x18\x37\xef\xdc\x03\xaf\xd6\xda\xc5\x88\xc6\x7a\
 \x6a\xb9\x35\x3f\x0f\x63\x1b\xcb\xd4\xce\xad\x85\x23\x75\xd6\xfa\
 \x6a\xf5\x8e\xb1\xbd\xf0\xde\x87\xb1\x62\x1f\xad\x85\x63\x71\xb6\
 \xf7\x22\x58\x6e\x6c\x90\x84\x63\xfe\x9d\xb9\x56\x32\x09\x43\x1b\
 \x6b\x4d\x7e\x92\x67\xfe\x5f\x0e\x4d\xcd\x1e\x16\x7c\xf9\x02\x05\
 \x63\xff\xe0\x36\x9a\x0b\x5e\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
 \x42\x60\x82\
-\x00\x00\x01\xc7\
+\x00\x00\x02\xed\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x31\x30\
-\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x33\x34\x22\x20\x76\x69\
-\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x31\x30\x20\x33\x34\
-\x22\x3e\x0d\x0a\x20\x20\x3c\x21\x2d\x2d\x20\x3c\x70\x61\x74\x68\
-\x20\x64\x3d\x22\x4d\x30\x20\x30\x76\x32\x68\x32\x76\x2d\x32\x68\
-\x2d\x32\x7a\x6d\x33\x20\x30\x76\x32\x68\x32\x76\x2d\x32\x68\x2d\
-\x32\x7a\x6d\x33\x20\x30\x76\x32\x68\x32\x76\x2d\x32\x68\x2d\x32\
-\x7a\x22\x20\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\
-\x61\x6e\x73\x6c\x61\x74\x65\x28\x30\x20\x33\x29\x22\x20\x2f\x3e\
-\x20\x2d\x2d\x3e\x0d\x0a\x20\x3c\x72\x65\x63\x74\x20\x78\x3d\x22\
-\x31\x22\x20\x79\x3d\x22\x31\x22\x20\x77\x69\x64\x74\x68\x3d\x22\
-\x38\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x66\x69\
-\x6c\x6c\x3d\x22\x67\x72\x65\x79\x22\x20\x73\x74\x72\x6f\x6b\x65\
-\x3d\x22\x72\x65\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\
-\x64\x74\x68\x3d\x22\x32\x22\x20\x20\x2f\x3e\x20\x0d\x0a\x20\x3c\
-\x72\x65\x63\x74\x20\x78\x3d\x22\x31\x22\x20\x79\x3d\x22\x31\x33\
-\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\x20\x68\x65\x69\x67\
-\x68\x74\x3d\x22\x38\x22\x20\x66\x69\x6c\x6c\x3d\x22\x72\x65\x64\
-\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x67\x72\x65\x79\x22\x20\
-\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x22\
-\x20\x20\x2f\x3e\x20\x0d\x0a\x20\x3c\x72\x65\x63\x74\x20\x78\x3d\
-\x22\x31\x22\x20\x79\x3d\x22\x32\x35\x22\x20\x77\x69\x64\x74\x68\
-\x3d\x22\x38\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\
-\x66\x69\x6c\x6c\x3d\x22\x67\x72\x65\x79\x22\x20\x73\x74\x72\x6f\
-\x6b\x65\x3d\x22\x72\x65\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
-\x77\x69\x64\x74\x68\x3d\x22\x32\x22\x20\x20\x2f\x3e\x20\x0d\x0a\
-\x3c\x2f\x73\x76\x67\x3e\
+\x30\x2f\x73\x76\x67\x22\x20\x78\x6d\x6c\x3a\x73\x70\x61\x63\x65\
+\x3d\x22\x70\x72\x65\x73\x65\x72\x76\x65\x22\x20\x77\x69\x64\x74\
+\x68\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\x20\x68\x65\x69\x67\x68\
+\x74\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\x20\x66\x69\x6c\x6c\x2d\
+\x72\x75\x6c\x65\x3d\x22\x65\x76\x65\x6e\x6f\x64\x64\x22\x20\x73\
+\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\
+\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\
+\x64\x74\x68\x3d\x22\x32\x38\x2e\x32\x32\x32\x22\x20\x70\x72\x65\
+\x73\x65\x72\x76\x65\x41\x73\x70\x65\x63\x74\x52\x61\x74\x69\x6f\
+\x3d\x22\x78\x4d\x69\x64\x59\x4d\x69\x64\x22\x20\x76\x65\x72\x73\
+\x69\x6f\x6e\x3d\x22\x31\x2e\x32\x22\x20\x76\x69\x65\x77\x42\x6f\
+\x78\x3d\x22\x30\x20\x30\x20\x38\x34\x37\x20\x38\x34\x37\x22\x3e\
+\x3c\x64\x65\x66\x73\x20\x63\x6c\x61\x73\x73\x3d\x22\x43\x6c\x69\
+\x70\x50\x61\x74\x68\x47\x72\x6f\x75\x70\x22\x3e\x3c\x63\x6c\x69\
+\x70\x50\x61\x74\x68\x20\x69\x64\x3d\x22\x61\x22\x3e\x3c\x70\x61\
+\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x38\x34\x37\x76\x38\
+\x34\x37\x48\x30\x7a\x22\x2f\x3e\x3c\x2f\x63\x6c\x69\x70\x50\x61\
+\x74\x68\x3e\x3c\x2f\x64\x65\x66\x73\x3e\x3c\x67\x20\x63\x6c\x61\
+\x73\x73\x3d\x22\x53\x6c\x69\x64\x65\x47\x72\x6f\x75\x70\x22\x3e\
+\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x53\x6c\x69\x64\x65\x22\
+\x20\x63\x6c\x69\x70\x2d\x70\x61\x74\x68\x3d\x22\x75\x72\x6c\x28\
+\x23\x61\x29\x22\x3e\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x50\
+\x61\x67\x65\x22\x3e\x3c\x67\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\
+\x6e\x65\x22\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\
+\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\
+\x43\x75\x73\x74\x6f\x6d\x53\x68\x61\x70\x65\x22\x3e\x3c\x70\x61\
+\x74\x68\x20\x64\x3d\x22\x4d\x34\x36\x20\x34\x36\x68\x37\x35\x35\
+\x76\x37\x35\x34\x48\x34\x36\x7a\x22\x20\x63\x6c\x61\x73\x73\x3d\
+\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x2f\x3e\x3c\
+\x70\x61\x74\x68\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x23\x30\x30\
+\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x63\x61\
+\x70\x3d\x22\x73\x71\x75\x61\x72\x65\x22\x20\x73\x74\x72\x6f\x6b\
+\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x6d\x69\x74\x65\
+\x72\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\
+\x22\x37\x38\x22\x20\x64\x3d\x22\x4d\x34\x32\x33\x20\x37\x36\x30\
+\x48\x38\x35\x56\x38\x35\x68\x36\x37\x36\x76\x36\x37\x35\x48\x34\
+\x32\x33\x7a\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\x67\x20\x63\x6c\x61\
+\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\
+\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x50\x6f\x6c\x79\x50\x6f\x6c\
+\x79\x67\x6f\x6e\x53\x68\x61\x70\x65\x22\x3e\x3c\x70\x61\x74\x68\
+\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x64\x3d\x22\
+\x4d\x30\x20\x30\x68\x38\x34\x39\x76\x38\x34\x39\x48\x30\x7a\x22\
+\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\
+\x42\x6f\x78\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\x2f\x67\x3e\x3c\x2f\
+\x67\x3e\x3c\x2f\x67\x3e\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x01\x6b\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
+\x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x01\x01\x01\x0a\x0d\
+\x0e\x14\x19\x1a\x29\x33\x36\x3c\x4c\x51\x4a\x59\x5f\x5f\x70\x75\
+\x6b\x85\x8e\x76\x94\x9e\x81\xa2\xac\x96\xb1\xba\xcb\xcd\xce\xac\
+\xd7\xe5\xad\xd8\xe6\xa1\xc9\xd6\x5a\xda\xbc\xfc\x00\x00\x00\xf6\
+\x49\x44\x41\x54\x28\xcf\xad\xd0\x4d\x0a\x41\x51\x14\x07\xf0\xbf\
+\x47\xc9\x40\xc9\x06\x88\x09\x43\x4c\x94\x42\x16\x20\x59\x81\x15\
+\x48\x86\x46\x7a\x0b\x90\xa9\x89\xa9\xba\x03\x1b\x90\x81\x29\x32\
+\xb2\x00\xf2\x7c\xd7\x95\x0d\xc8\x79\xf7\x3e\x1c\x1f\x65\xc0\x7f\
+\xf2\x5e\xbf\x7b\xba\xe7\x9c\x8b\x29\x65\x32\x98\xf2\x60\x26\xa5\
+\x99\x30\x52\x7d\xf9\x08\x99\x15\x06\x90\x7e\xb6\x12\x11\x8c\x16\
+\xb7\xad\x5d\x06\x64\xb8\x2d\x15\xc1\xc3\xcd\xd4\xe6\xbe\x30\xab\
+\x68\x33\xfa\xcc\x4a\x4e\x5d\xf7\x4b\x1d\xbf\xef\xd8\x19\x2a\x5b\
+\x3c\xfa\xee\x92\xd1\x48\x55\xcd\x17\xb8\xcf\x57\xa0\x6f\xf0\x62\
+\xef\x91\xbf\xed\x61\xa9\xc3\xdc\x7d\xdf\x18\x95\x95\xf5\xc5\xb6\
+\xc9\x3a\xfd\x50\xd7\xa3\x5e\xd2\x68\xd9\xb6\x07\x7c\x54\xb6\xd1\
+\xcd\x50\x64\x66\x39\xe6\xff\x60\x19\x66\x2b\xc7\x42\xcc\xd6\x8e\
+\x65\x99\x1d\x74\x5f\x57\x95\x99\x1e\x9e\x16\xe7\x76\x56\x16\x97\
+\xdc\x4e\x01\xfd\x66\xdc\xe4\x3c\xac\xde\xe2\xc9\x64\x13\xe8\xbe\
+\x5a\xfb\x77\x1b\x0b\xd1\x03\xbc\x42\xa5\x06\x34\x84\xc0\x08\xef\
+\xf9\xb7\x8d\xc5\x5b\xae\x6f\xd7\x4f\x6c\x5a\x3f\xe0\x76\x00\x00\
+\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x00\xc6\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x76\
+\x34\x6c\x31\x2e\x35\x2d\x31\x2e\x35\x20\x31\x2e\x35\x20\x31\x2e\
+\x35\x20\x31\x2d\x31\x2d\x31\x2e\x35\x2d\x31\x2e\x35\x20\x31\x2e\
+\x35\x2d\x31\x2e\x35\x68\x2d\x34\x7a\x6d\x35\x20\x34\x6c\x2d\x31\
+\x20\x31\x20\x31\x2e\x35\x20\x31\x2e\x35\x2d\x31\x2e\x35\x20\x31\
+\x2e\x35\x68\x34\x76\x2d\x34\x6c\x2d\x31\x2e\x35\x20\x31\x2e\x35\
+\x2d\x31\x2e\x35\x2d\x31\x2e\x35\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\
+\x2f\x73\x76\x67\x3e\
 \x00\x00\x00\x93\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
 \x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
 \x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
 \x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x20\x30\x76\
 \x33\x68\x2d\x32\x6c\x33\x20\x33\x20\x33\x2d\x33\x68\x2d\x32\x76\
 \x2d\x33\x68\x2d\x32\x7a\x6d\x2d\x33\x20\x37\x76\x31\x68\x38\x76\
 \x2d\x31\x68\x2d\x38\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\
 \x67\x3e\
+\x00\x00\x00\xd2\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x20\x30\x63\
+\x2d\x31\x2e\x31\x20\x30\x2d\x32\x20\x2e\x39\x2d\x32\x20\x32\x68\
+\x31\x63\x30\x2d\x2e\x35\x36\x2e\x34\x34\x2d\x31\x20\x31\x2d\x31\
+\x73\x31\x20\x2e\x34\x34\x20\x31\x20\x31\x76\x32\x68\x2d\x34\x76\
+\x34\x68\x36\x76\x2d\x34\x68\x2d\x31\x76\x2d\x32\x63\x30\x2d\x31\
+\x2e\x31\x2d\x2e\x39\x2d\x32\x2d\x32\x2d\x32\x7a\x22\x20\x74\x72\
+\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\x61\
+\x74\x65\x28\x31\x29\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\
+\x3e\
+\x00\x00\x01\x62\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\
+\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\x69\
+\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\x38\
+\x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\
+\x22\x4d\x36\x20\x31\x38\x76\x31\x32\x68\x38\x6c\x31\x30\x20\x31\
+\x30\x56\x38\x4c\x31\x34\x20\x31\x38\x48\x36\x7a\x6d\x32\x37\x20\
+\x36\x63\x30\x2d\x33\x2e\x35\x33\x2d\x32\x2e\x30\x34\x2d\x36\x2e\
+\x35\x38\x2d\x35\x2d\x38\x2e\x30\x35\x76\x31\x36\x2e\x31\x31\x63\
+\x32\x2e\x39\x36\x2d\x31\x2e\x34\x38\x20\x35\x2d\x34\x2e\x35\x33\
+\x20\x35\x2d\x38\x2e\x30\x36\x7a\x4d\x32\x38\x20\x36\x2e\x34\x36\
+\x76\x34\x2e\x31\x33\x63\x35\x2e\x37\x38\x20\x31\x2e\x37\x32\x20\
+\x31\x30\x20\x37\x2e\x30\x37\x20\x31\x30\x20\x31\x33\x2e\x34\x31\
+\x73\x2d\x34\x2e\x32\x32\x20\x31\x31\x2e\x36\x39\x2d\x31\x30\x20\
+\x31\x33\x2e\x34\x31\x76\x34\x2e\x31\x33\x63\x38\x2e\x30\x31\x2d\
+\x31\x2e\x38\x32\x20\x31\x34\x2d\x38\x2e\x39\x37\x20\x31\x34\x2d\
+\x31\x37\x2e\x35\x34\x53\x33\x36\x2e\x30\x31\x20\x38\x2e\x32\x38\
+\x20\x32\x38\x20\x36\x2e\x34\x36\x7a\x22\x2f\x3e\x0d\x0a\x20\x20\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\
+\x34\x38\x76\x34\x38\x48\x30\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\
+\x6e\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\
+\x0a\
 \x00\x00\x03\x09\
 \x3c\
 \x73\x76\x67\x20\x77\x69\x64\x74\x68\x3d\x22\x33\x39\x22\x20\x68\
 \x65\x69\x67\x68\x74\x3d\x22\x33\x31\x22\x20\x78\x6d\x6c\x6e\x73\
 \x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\
 \x6f\x72\x67\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\x3e\x0d\x0a\
 \x0d\x0a\x20\x3c\x67\x3e\x0d\x0a\x20\x20\x3c\x74\x69\x74\x6c\x65\
@@ -569,31 +381,256 @@
 \x2e\x39\x39\x39\x38\x39\x39\x2c\x30\x6c\x30\x2c\x2d\x38\x6c\x2d\
 \x32\x35\x2e\x39\x39\x39\x38\x39\x39\x2c\x30\x7a\x22\x20\x73\x74\
 \x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\
 \x6f\x75\x6e\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\
 \x74\x68\x3d\x22\x30\x2e\x32\x22\x20\x66\x69\x6c\x6c\x3d\x22\x23\
 \x30\x30\x30\x30\x30\x30\x22\x2f\x3e\x0d\x0a\x20\x3c\x2f\x67\x3e\
 \x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x00\xea\
+\x00\x00\x05\x0b\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x78\x6d\x6c\x3a\x73\x70\x61\x63\x65\
+\x3d\x22\x70\x72\x65\x73\x65\x72\x76\x65\x22\x20\x77\x69\x64\x74\
+\x68\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\x20\x68\x65\x69\x67\x68\
+\x74\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\x20\x66\x69\x6c\x6c\x2d\
+\x72\x75\x6c\x65\x3d\x22\x65\x76\x65\x6e\x6f\x64\x64\x22\x20\x73\
+\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\
+\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\
+\x64\x74\x68\x3d\x22\x32\x38\x2e\x32\x32\x32\x22\x20\x70\x72\x65\
+\x73\x65\x72\x76\x65\x41\x73\x70\x65\x63\x74\x52\x61\x74\x69\x6f\
+\x3d\x22\x78\x4d\x69\x64\x59\x4d\x69\x64\x22\x20\x76\x65\x72\x73\
+\x69\x6f\x6e\x3d\x22\x31\x2e\x32\x22\x20\x76\x69\x65\x77\x42\x6f\
+\x78\x3d\x22\x30\x20\x30\x20\x38\x34\x37\x20\x38\x34\x37\x22\x3e\
+\x3c\x64\x65\x66\x73\x20\x63\x6c\x61\x73\x73\x3d\x22\x43\x6c\x69\
+\x70\x50\x61\x74\x68\x47\x72\x6f\x75\x70\x22\x3e\x3c\x63\x6c\x69\
+\x70\x50\x61\x74\x68\x20\x69\x64\x3d\x22\x61\x22\x3e\x3c\x70\x61\
+\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x38\x34\x37\x76\x38\
+\x34\x37\x48\x30\x7a\x22\x2f\x3e\x3c\x2f\x63\x6c\x69\x70\x50\x61\
+\x74\x68\x3e\x3c\x2f\x64\x65\x66\x73\x3e\x3c\x67\x20\x63\x6c\x61\
+\x73\x73\x3d\x22\x53\x6c\x69\x64\x65\x47\x72\x6f\x75\x70\x22\x3e\
+\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x53\x6c\x69\x64\x65\x22\
+\x20\x63\x6c\x69\x70\x2d\x70\x61\x74\x68\x3d\x22\x75\x72\x6c\x28\
+\x23\x61\x29\x22\x3e\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x50\
+\x61\x67\x65\x22\x3e\x3c\x67\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\
+\x6e\x65\x22\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\
+\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\
+\x4c\x69\x6e\x65\x53\x68\x61\x70\x65\x22\x3e\x3c\x70\x61\x74\x68\
+\x20\x64\x3d\x22\x4d\x32\x39\x34\x20\x39\x34\x68\x31\x33\x76\x36\
+\x31\x33\x68\x2d\x31\x33\x7a\x22\x20\x63\x6c\x61\x73\x73\x3d\x22\
+\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x2f\x3e\x3c\x70\
+\x61\x74\x68\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x23\x30\x30\x30\
+\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\
+\x31\x31\x22\x20\x64\x3d\x22\x4d\x33\x30\x30\x20\x31\x30\x30\x76\
+\x36\x30\x30\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\x67\x20\x66\x69\x6c\
+\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x63\x6c\x61\x73\x73\x3d\x22\
+\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\
+\x77\x69\x6e\x67\x2e\x43\x75\x73\x74\x6f\x6d\x53\x68\x61\x70\x65\
+\x22\x3e\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x32\x32\x20\x32\
+\x33\x68\x37\x35\x35\x76\x37\x35\x34\x48\x32\x32\x7a\x22\x20\x63\
+\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\
+\x78\x22\x2f\x3e\x3c\x70\x61\x74\x68\x20\x73\x74\x72\x6f\x6b\x65\
+\x3d\x22\x23\x30\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\
+\x69\x6e\x65\x63\x61\x70\x3d\x22\x73\x71\x75\x61\x72\x65\x22\x20\
+\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\
+\x22\x6d\x69\x74\x65\x72\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\
+\x69\x64\x74\x68\x3d\x22\x37\x38\x22\x20\x64\x3d\x22\x4d\x33\x39\
+\x39\x20\x37\x33\x37\x48\x36\x31\x56\x36\x32\x68\x36\x37\x36\x76\
+\x36\x37\x35\x48\x33\x39\x39\x7a\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\
+\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\
+\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x50\x6f\
+\x6c\x79\x50\x6f\x6c\x79\x67\x6f\x6e\x53\x68\x61\x70\x65\x22\x3e\
+\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\
+\x22\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x38\x34\x39\x76\x38\x34\
+\x39\x48\x30\x7a\x22\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\
+\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\
+\x67\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x63\x6c\
+\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\
+\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x4c\x69\x6e\x65\x53\x68\
+\x61\x70\x65\x22\x3e\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x34\
+\x39\x34\x20\x39\x34\x68\x31\x33\x76\x36\x31\x33\x68\x2d\x31\x33\
+\x7a\x22\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\
+\x6e\x67\x42\x6f\x78\x22\x2f\x3e\x3c\x70\x61\x74\x68\x20\x73\x74\
+\x72\x6f\x6b\x65\x3d\x22\x23\x30\x30\x30\x22\x20\x73\x74\x72\x6f\
+\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x31\x31\x22\x20\x64\x3d\
+\x22\x4d\x35\x30\x30\x20\x31\x30\x30\x76\x36\x30\x30\x22\x2f\x3e\
+\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x39\x34\x20\x32\x39\x34\
+\x68\x36\x31\x33\x76\x31\x33\x48\x39\x34\x7a\x22\x20\x63\x6c\x61\
+\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\
+\x2f\x3e\x3c\x70\x61\x74\x68\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\
+\x23\x30\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\
+\x74\x68\x3d\x22\x31\x31\x22\x20\x64\x3d\x22\x4d\x37\x30\x30\x20\
+\x33\x30\x30\x48\x31\x30\x30\x22\x2f\x3e\x3c\x70\x61\x74\x68\x20\
+\x64\x3d\x22\x4d\x39\x34\x20\x34\x39\x34\x68\x36\x31\x33\x76\x31\
+\x33\x48\x39\x34\x7a\x22\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\
+\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x2f\x3e\x3c\x70\x61\x74\
+\x68\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x23\x30\x30\x30\x22\x20\
+\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x31\x31\
+\x22\x20\x64\x3d\x22\x4d\x37\x30\x30\x20\x35\x30\x30\x48\x31\x30\
+\x30\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\x2f\x67\x3e\x3c\x2f\x67\x3e\
+\x3c\x2f\x67\x3e\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x01\x7d\
+\x3c\
+\x73\x76\x67\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\x32\
+\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x32\x2e\x33\x38\x6d\x6d\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x2e\x33\x38\x6d\x6d\x22\
+\x20\x76\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x32\x33\
+\x38\x20\x32\x33\x38\x22\x20\x70\x72\x65\x73\x65\x72\x76\x65\x41\
+\x73\x70\x65\x63\x74\x52\x61\x74\x69\x6f\x3d\x22\x78\x4d\x69\x64\
+\x59\x4d\x69\x64\x22\x20\x66\x69\x6c\x6c\x2d\x72\x75\x6c\x65\x3d\
+\x22\x65\x76\x65\x6e\x6f\x64\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\
+\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x38\x2e\x32\x32\x32\x22\x20\
+\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\
+\x22\x72\x6f\x75\x6e\x64\x22\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\
+\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\
+\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\x20\x3e\x0a\x0a\x3c\x70\
+\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x72\x67\x62\x28\x30\x2c\
+\x30\x2c\x30\x29\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\
+\x6e\x65\x22\x20\x64\x3d\x22\x4d\x20\x32\x32\x33\x2c\x31\x39\x38\
+\x20\x4c\x20\x31\x34\x34\x2c\x31\x31\x39\x20\x31\x37\x30\x2c\x39\
+\x32\x20\x39\x30\x2c\x31\x33\x20\x36\x34\x2c\x34\x30\x20\x31\x31\
+\x38\x2c\x39\x32\x20\x39\x31\x2c\x31\x31\x39\x20\x31\x39\x37\x2c\
+\x32\x32\x34\x20\x32\x32\x33\x2c\x31\x39\x38\x20\x32\x32\x33\x2c\
+\x31\x39\x38\x20\x5a\x20\x4d\x20\x33\x38\x2c\x31\x33\x20\x4c\x20\
+\x31\x32\x2c\x31\x33\x20\x31\x32\x2c\x32\x32\x34\x20\x33\x38\x2c\
+\x32\x32\x34\x20\x33\x38\x2c\x31\x33\x20\x33\x38\x2c\x31\x33\x20\
+\x5a\x22\x2f\x3e\x0a\x0a\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x02\xa4\
+\x3c\
+\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
+\x30\x22\x3f\x3e\x0d\x0a\x3c\x73\x76\x67\x20\x77\x69\x64\x74\x68\
+\x3d\x22\x33\x38\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x33\x35\
+\x22\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\
+\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\x2f\
+\x73\x76\x67\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x73\x76\x67\x3d\x22\
+\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\
+\x67\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\x3e\x0d\x0a\x0d\x0a\
+\x20\x3c\x67\x3e\x0d\x0a\x20\x20\x3c\x74\x69\x74\x6c\x65\x3e\x4c\
+\x61\x79\x65\x72\x20\x31\x3c\x2f\x74\x69\x74\x6c\x65\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x69\x64\x3d\x22\x73\x76\x67\x5f\
+\x31\x22\x20\x64\x3d\x22\x6d\x31\x32\x2e\x38\x38\x36\x2c\x33\x32\
+\x2e\x34\x32\x31\x36\x6c\x33\x2e\x35\x33\x35\x36\x30\x31\x2c\x2d\
+\x33\x2e\x35\x33\x35\x35\x6c\x2d\x33\x2e\x35\x33\x35\x36\x30\x31\
+\x2c\x2d\x33\x2e\x35\x33\x35\x36\x30\x33\x6c\x32\x2e\x35\x37\x38\
+\x35\x30\x31\x2c\x2d\x32\x2e\x35\x37\x38\x34\x6c\x33\x2e\x35\x33\
+\x35\x35\x2c\x33\x2e\x35\x33\x35\x35\x6c\x33\x2e\x35\x33\x35\x35\
+\x2c\x2d\x33\x2e\x35\x33\x35\x35\x6c\x32\x2e\x35\x37\x38\x34\x2c\
+\x32\x2e\x35\x37\x38\x34\x6c\x2d\x33\x2e\x35\x33\x35\x35\x2c\x33\
+\x2e\x35\x33\x35\x35\x30\x33\x6c\x33\x2e\x35\x33\x35\x35\x39\x39\
+\x2c\x33\x2e\x35\x33\x35\x35\x39\x39\x6c\x2d\x32\x2e\x35\x37\x38\
+\x34\x39\x39\x2c\x32\x2e\x35\x37\x38\x34\x6c\x2d\x33\x2e\x35\x33\
+\x35\x35\x2c\x2d\x33\x2e\x35\x33\x35\x35\x6c\x2d\x33\x2e\x35\x33\
+\x35\x35\x2c\x33\x2e\x35\x33\x35\x35\x6c\x2d\x32\x2e\x35\x37\x38\
+\x35\x30\x31\x2c\x2d\x32\x2e\x35\x37\x38\x34\x7a\x6d\x2d\x31\x32\
+\x2e\x38\x38\x36\x2c\x2d\x33\x32\x2e\x36\x37\x31\x36\x6c\x38\x2c\
+\x30\x6c\x30\x2c\x38\x6c\x2d\x38\x2c\x30\x6c\x30\x2c\x2d\x38\x7a\
+\x6d\x31\x31\x2e\x39\x39\x39\x39\x30\x31\x2c\x30\x2e\x30\x30\x30\
+\x32\x39\x39\x6c\x32\x35\x2e\x39\x39\x39\x37\x39\x38\x2c\x30\x6c\
+\x30\x2c\x38\x6c\x2d\x32\x35\x2e\x39\x39\x39\x37\x39\x38\x2c\x30\
+\x6c\x30\x2c\x2d\x38\x7a\x6d\x2d\x31\x31\x2e\x39\x39\x39\x39\x30\
+\x31\x2c\x31\x30\x2e\x39\x39\x39\x37\x30\x31\x6c\x38\x2c\x30\x6c\
+\x30\x2c\x38\x6c\x2d\x38\x2c\x30\x6c\x30\x2c\x2d\x38\x7a\x6d\x31\
+\x2c\x31\x6c\x30\x2c\x36\x6c\x36\x2c\x30\x6c\x30\x2c\x2d\x36\x6c\
+\x2d\x36\x2c\x30\x7a\x6d\x31\x2c\x31\x6c\x34\x2c\x30\x6c\x30\x2c\
+\x34\x6c\x2d\x34\x2c\x30\x6c\x30\x2c\x2d\x34\x7a\x6d\x31\x30\x2c\
+\x2d\x32\x6c\x32\x36\x2c\x30\x6c\x30\x2c\x38\x6c\x2d\x32\x36\x2c\
+\x30\x6c\x30\x2c\x2d\x38\x7a\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
+\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\
+\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x30\
+\x2e\x32\x22\x20\x66\x69\x6c\x6c\x3d\x22\x23\x30\x30\x30\x30\x30\
+\x30\x22\x2f\x3e\x0d\x0a\x20\x3c\x2f\x67\x3e\x0d\x0a\x3c\x2f\x73\
+\x76\x67\x3e\
+\x00\x00\x01\xc5\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
 \x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
 \x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
 \x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x2e\x35\x20\
-\x30\x6c\x2d\x31\x2e\x35\x20\x31\x2e\x35\x68\x31\x76\x31\x2e\x35\
-\x68\x2d\x31\x2e\x35\x76\x2d\x31\x6c\x2d\x31\x2e\x35\x20\x31\x2e\
-\x35\x20\x31\x2e\x35\x20\x31\x2e\x35\x76\x2d\x31\x68\x31\x2e\x35\
-\x76\x31\x2e\x35\x68\x2d\x31\x6c\x31\x2e\x35\x20\x31\x2e\x35\x20\
-\x31\x2e\x35\x2d\x31\x2e\x35\x68\x2d\x31\x76\x2d\x31\x2e\x35\x68\
-\x31\x2e\x35\x76\x31\x6c\x31\x2e\x35\x2d\x31\x2e\x35\x2d\x31\x2e\
-\x35\x2d\x31\x2e\x35\x76\x31\x68\x2d\x31\x2e\x35\x76\x2d\x31\x2e\
-\x35\x68\x31\x6c\x2d\x31\x2e\x35\x2d\x31\x2e\x35\x7a\x22\x20\x2f\
-\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
+\x30\x63\x2d\x31\x2e\x39\x33\x20\x30\x2d\x33\x2e\x35\x20\x31\x2e\
+\x35\x37\x2d\x33\x2e\x35\x20\x33\x2e\x35\x73\x31\x2e\x35\x37\x20\
+\x33\x2e\x35\x20\x33\x2e\x35\x20\x33\x2e\x35\x63\x2e\x35\x39\x20\
+\x30\x20\x31\x2e\x31\x37\x2d\x2e\x31\x34\x20\x31\x2e\x36\x36\x2d\
+\x2e\x34\x31\x61\x31\x20\x31\x20\x30\x20\x30\x20\x30\x20\x2e\x31\
+\x33\x2e\x31\x33\x6c\x31\x20\x31\x61\x31\x2e\x30\x32\x20\x31\x2e\
+\x30\x32\x20\x30\x20\x31\x20\x30\x20\x31\x2e\x34\x34\x2d\x31\x2e\
+\x34\x34\x6c\x2d\x31\x2d\x31\x61\x31\x20\x31\x20\x30\x20\x30\x20\
+\x30\x2d\x2e\x31\x36\x2d\x2e\x31\x33\x63\x2e\x32\x37\x2d\x2e\x34\
+\x39\x2e\x34\x34\x2d\x31\x2e\x30\x36\x2e\x34\x34\x2d\x31\x2e\x36\
+\x36\x20\x30\x2d\x31\x2e\x39\x33\x2d\x31\x2e\x35\x37\x2d\x33\x2e\
+\x35\x2d\x33\x2e\x35\x2d\x33\x2e\x35\x7a\x6d\x30\x20\x31\x63\x31\
+\x2e\x33\x39\x20\x30\x20\x32\x2e\x35\x20\x31\x2e\x31\x31\x20\x32\
+\x2e\x35\x20\x32\x2e\x35\x20\x30\x20\x2e\x36\x36\x2d\x2e\x32\x34\
+\x20\x31\x2e\x32\x37\x2d\x2e\x36\x36\x20\x31\x2e\x37\x32\x2d\x2e\
+\x30\x31\x2e\x30\x31\x2d\x2e\x30\x32\x2e\x30\x32\x2d\x2e\x30\x33\
+\x2e\x30\x33\x61\x31\x20\x31\x20\x30\x20\x30\x20\x30\x2d\x2e\x31\
+\x33\x2e\x31\x33\x63\x2d\x2e\x34\x34\x2e\x34\x2d\x31\x2e\x30\x34\
+\x2e\x36\x33\x2d\x31\x2e\x36\x39\x2e\x36\x33\x2d\x31\x2e\x33\x39\
+\x20\x30\x2d\x32\x2e\x35\x2d\x31\x2e\x31\x31\x2d\x32\x2e\x35\x2d\
+\x32\x2e\x35\x73\x31\x2e\x31\x31\x2d\x32\x2e\x35\x20\x32\x2e\x35\
+\x2d\x32\x2e\x35\x7a\x22\x0d\x0a\x20\x20\x2f\x3e\x0d\x0a\x3c\x2f\
+\x73\x76\x67\x3e\
+\x00\x00\x00\xb4\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
+\x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x30\x30\x30\x40\x40\x40\x50\x50\x50\x60\x60\x60\x60\x6f\x74\
+\x80\x80\x80\x76\x94\x9e\x81\xa2\xac\xb0\xb0\xb0\xcb\xce\xcf\xae\
+\xd8\xe6\xad\xd8\xe6\xad\xd8\xe6\x0c\x60\x27\x73\x00\x00\x00\x3f\
+\x49\x44\x41\x54\x28\xcf\x63\x38\x83\x09\x18\xce\xbd\x7b\xf7\x52\
+\x50\x50\xf2\x1d\x12\x18\x15\x23\x46\x6c\xa2\xa0\xe0\xbc\x51\x31\
+\x9c\x62\xa7\x56\xad\x5a\x2e\x28\x28\xbe\x0a\x0c\x0a\x05\x05\xab\
+\x56\xad\x62\x38\x28\x88\x01\xa8\x2e\x76\x6a\x15\x06\x00\x00\x9e\
+\xe8\xcb\xd7\xeb\xf5\xf2\x67\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
+\x42\x60\x82\
+\x00\x00\x01\x08\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x34\x20\x30\x63\
+\x2d\x32\x2e\x32\x31\x20\x30\x2d\x34\x20\x31\x2e\x37\x39\x2d\x34\
+\x20\x34\x73\x31\x2e\x37\x39\x20\x34\x20\x34\x20\x34\x20\x34\x2d\
+\x31\x2e\x37\x39\x20\x34\x2d\x34\x2d\x31\x2e\x37\x39\x2d\x34\x2d\
+\x34\x2d\x34\x7a\x6d\x2d\x31\x2e\x35\x20\x31\x2e\x37\x38\x6c\x31\
+\x2e\x35\x20\x31\x2e\x35\x20\x31\x2e\x35\x2d\x31\x2e\x35\x2e\x37\
+\x32\x2e\x37\x32\x2d\x31\x2e\x35\x20\x31\x2e\x35\x20\x31\x2e\x35\
+\x20\x31\x2e\x35\x2d\x2e\x37\x32\x2e\x37\x32\x2d\x31\x2e\x35\x2d\
+\x31\x2e\x35\x2d\x31\x2e\x35\x20\x31\x2e\x35\x2d\x2e\x37\x32\x2d\
+\x2e\x37\x32\x20\x31\x2e\x35\x2d\x31\x2e\x35\x2d\x31\x2e\x35\x2d\
+\x31\x2e\x35\x2e\x37\x32\x2d\x2e\x37\x32\x7a\x22\x20\x2f\x3e\x0d\
+\x0a\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x01\x55\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x2e\x35\x20\
+\x30\x63\x2d\x2e\x32\x38\x20\x30\x2d\x2e\x35\x2e\x32\x32\x2d\x2e\
+\x35\x2e\x35\x76\x2e\x35\x68\x2d\x2e\x37\x35\x63\x2d\x2e\x31\x34\
+\x20\x30\x2d\x2e\x32\x35\x2e\x31\x31\x2d\x2e\x32\x35\x2e\x32\x35\
+\x76\x2e\x37\x35\x68\x33\x76\x2d\x2e\x37\x35\x63\x30\x2d\x2e\x31\
+\x34\x2d\x2e\x31\x31\x2d\x2e\x32\x35\x2d\x2e\x32\x35\x2d\x2e\x32\
+\x35\x68\x2d\x2e\x37\x35\x76\x2d\x2e\x35\x63\x30\x2d\x2e\x32\x38\
+\x2d\x2e\x32\x32\x2d\x2e\x35\x2d\x2e\x35\x2d\x2e\x35\x7a\x6d\x2d\
+\x33\x2e\x32\x35\x20\x31\x63\x2d\x2e\x31\x34\x20\x30\x2d\x2e\x32\
+\x35\x2e\x31\x31\x2d\x2e\x32\x35\x2e\x32\x35\x76\x36\x2e\x35\x63\
+\x30\x20\x2e\x31\x34\x2e\x31\x31\x2e\x32\x35\x2e\x32\x35\x2e\x32\
+\x35\x68\x36\x2e\x35\x63\x2e\x31\x34\x20\x30\x20\x2e\x32\x35\x2d\
+\x2e\x31\x31\x2e\x32\x35\x2d\x2e\x32\x35\x76\x2d\x36\x2e\x35\x63\
+\x30\x2d\x2e\x31\x34\x2d\x2e\x31\x31\x2d\x2e\x32\x35\x2d\x2e\x32\
+\x35\x2d\x2e\x32\x35\x68\x2d\x2e\x37\x35\x76\x32\x68\x2d\x35\x76\
+\x2d\x32\x68\x2d\x2e\x37\x35\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\
+\x73\x76\x67\x3e\
 \x00\x00\x01\x44\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
 \x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x01\x01\x01\x0d\x10\
 \x11\x1f\x27\x2a\x37\x44\x48\x45\x55\x5b\x5b\x65\x68\x56\x6c\x73\
 \x6c\x86\x8e\x7f\x9e\xa9\xa0\xa0\xa0\x94\xb9\xc5\xcb\xce\xcf\xad\
@@ -609,156 +646,30 @@
 \x0d\x34\xb1\xd7\x40\xc7\x33\xcd\x43\x15\xdb\x04\xf2\x8f\x26\x8a\
 \x18\x8b\x01\x48\x8c\xa9\xbc\x1b\x49\x0c\x01\x60\x62\x2f\xb0\x88\
 \xbd\xc7\x22\xf6\xee\x47\x39\x38\xcc\x98\x1c\x90\xc4\x20\x61\xc6\
 \xa0\x51\x80\x22\xf6\x42\x01\x14\xa7\xa8\x62\xef\x8a\x18\x18\x54\
 \xdf\xa1\x89\xbd\x2e\x36\xdb\x87\x2e\x06\x06\x94\x89\x01\x00\x6a\
 \xae\xde\x44\xf4\xac\x37\x49\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
 \x42\x60\x82\
-\x00\x00\x00\xb4\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x32\x20\x30\x76\
-\x36\x68\x2d\x32\x6c\x32\x2e\x35\x20\x32\x20\x32\x2e\x35\x2d\x32\
-\x68\x2d\x32\x76\x2d\x36\x68\x2d\x31\x7a\x6d\x32\x20\x30\x76\x31\
-\x68\x32\x76\x2d\x31\x68\x2d\x32\x7a\x6d\x30\x20\x32\x76\x31\x68\
-\x33\x76\x2d\x31\x68\x2d\x33\x7a\x6d\x30\x20\x32\x76\x31\x68\x34\
-\x76\x2d\x31\x68\x2d\x34\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\
-\x76\x67\x3e\
-\x00\x00\x00\x8b\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x76\
-\x38\x68\x37\x76\x2d\x34\x68\x2d\x34\x76\x2d\x34\x68\x2d\x33\x7a\
-\x6d\x34\x20\x30\x76\x33\x68\x33\x6c\x2d\x33\x2d\x33\x7a\x22\x20\
-\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x03\xe9\
-\x00\
-\x00\x19\x14\x78\x9c\xcd\x98\x5d\x6f\xdb\x36\x14\x86\xef\x0b\xf4\
-\x3f\x70\xec\x45\xb6\x0b\x7d\x50\x12\x25\x37\xb0\x56\x2c\x4e\x16\
-\x14\x68\xb7\x60\x49\x37\xf4\x2a\xd0\x24\xc6\xe2\x26\x8b\xaa\x24\
-\xcb\xee\x7e\xfd\x0e\x65\x7d\x35\xb6\x1b\x53\x68\xec\x02\x51\x44\
-\x52\x47\x47\x7c\x5e\xbe\x87\x20\x3c\x7d\xb3\x5e\x24\xa8\x62\x79\
-\xc1\x45\xea\x63\xa2\x9b\x18\xb1\x34\x14\x11\x4f\xe7\x3e\xfe\x70\
-\xf7\xab\x36\xc1\x6f\x7e\x7e\xf9\x62\xfa\xc3\xe5\xef\xb3\xbb\x8f\
-\x37\x57\xa8\xa8\xe6\x08\xdd\x7c\xb8\x78\xf7\x76\x86\xce\x34\xc3\
-\xf8\xcb\x9e\x19\xc6\xe5\xdd\x25\xba\xfd\xf3\x1a\x11\x9d\x18\xc6\
-\xd5\x6f\x67\x08\x9d\xc5\x65\x99\x9d\x1b\xc6\x6a\xb5\xd2\x57\xb6\
-\x2e\xf2\xb9\x71\x9d\x07\x59\xcc\xc3\xc2\x80\x48\x43\x46\xc2\x5b\
-\x06\xa4\x23\x44\x8f\xca\xe8\x4c\x7e\x45\x26\x5f\xf1\xa8\x8c\x7d\
-\x3c\x59\x2c\x30\x8a\x19\x9f\xc7\x65\xd3\x79\xe0\x49\xa2\xe5\xcb\
-\x84\xf9\x98\x55\x2c\x15\x51\x84\x51\x51\xe6\xe2\x5f\xa6\x25\x3c\
-\x65\xff\x08\x0e\x04\xb9\x58\xa6\xfd\x78\x93\xcb\x9a\xe8\x96\x65\
-\x61\x94\xe5\xac\x60\x79\xc5\x7e\x29\x32\x16\x96\x7f\x04\x25\x17\
-\x3e\x5e\xbf\xe7\xd1\x47\xb8\xf0\x50\x06\x08\xae\x38\x5b\x5d\x88\
-\xb5\x8f\x4d\x64\xa2\x89\x59\x5f\x18\x81\x5c\xe7\x45\x16\x84\x30\
-\x89\x36\x5b\x3d\x98\x16\x3e\xde\x46\xb6\x4c\xd3\x94\x88\x4d\xc8\
-\xb9\x10\xa2\x0b\x83\x11\x5d\x64\xc0\xf1\xf0\xc0\x43\x56\x87\x43\
-\xa4\xc1\xd6\x99\xc8\x4b\x0c\x6a\xa0\x69\xc4\x1e\x0a\x14\x26\x41\
-\x01\xc9\x67\x09\xcf\x6e\x82\x32\xbe\x06\xc2\xac\x7e\x8c\xa6\x61\
-\x33\x86\x78\xd4\x4c\x27\x2d\x25\x54\x7a\x2f\x9f\xdc\x67\xf0\x68\
-\x13\x89\xa6\x39\x00\x77\xd2\x4a\x90\x4e\x5a\xe8\x18\x9b\x74\x46\
-\x9b\xaf\xee\xca\x09\x18\x72\x06\x5b\x53\xb9\x63\xeb\xf2\x36\x0e\
-\x32\xf6\x36\x8d\xd8\x1a\x3f\x11\x7d\xb5\xf8\x9b\x45\x11\x8b\x2e\
-\x96\x49\xc2\xca\x59\x1c\xe4\x45\xf7\xca\x21\x57\x9f\x76\xf3\x87\
-\xa6\xf3\x9a\x97\x47\xb0\x48\xcd\x37\xde\x07\x45\xc9\xf2\xfb\xdb\
-\x84\x47\xac\x21\xee\xfe\x4d\x8d\x79\xf3\x32\xbc\xd8\xc4\xd7\x81\
-\x03\x25\x37\x1a\x6d\xf2\x86\x02\x44\x04\x3f\xe5\x1a\x8f\x48\x93\
-\xac\xff\x26\xc1\x5f\xe4\x90\x3d\x9e\x69\x52\x69\x1f\x2f\xf3\xe4\
-\xc7\x57\xbb\x97\xe1\xa7\x36\xd1\x60\x12\x37\xc1\x9c\x75\xc3\x83\
-\xf1\x50\x2c\xf4\x62\x99\xea\x45\x19\xe4\x7a\x94\x07\x2b\xa8\x45\
-\xfd\x1d\xcc\xa8\xd6\xbc\x7f\xa3\x9f\x94\xbd\x29\x0e\x1f\xa7\x22\
-\x1d\x06\x34\xcb\xde\xe4\xbd\x90\xa5\x01\xb9\xc0\xd4\xe0\x47\xa8\
-\x8a\xd7\x13\x8c\x3e\xfb\x58\xde\x1a\x67\x10\xbb\x37\x86\x0b\x1d\
-\x63\x98\x4b\x72\x20\xf8\xde\xc2\x36\x1d\x44\x4c\xa7\x72\xa5\x8f\
-\x36\x95\xe6\xe3\x57\x66\xdf\x7b\xaa\x1e\x09\x19\x66\x6e\x16\x68\
-\xbb\xfd\x75\x45\x66\xcb\xa2\x14\x8b\xbd\x9a\x38\xe3\x34\x71\x6b\
-\x49\x2c\xaf\x93\xc4\xa3\xb4\xd7\xc4\xa3\xce\x1e\x4d\x1c\xd3\x46\
-\x9e\x43\x62\xcd\xb6\x27\x95\xe6\x7a\x34\x76\x3d\xb7\x92\x77\x39\
-\xf2\xdf\x57\x74\x0a\x83\xcc\xc7\xc5\xa7\x65\x90\xb3\x1d\xfa\x2d\
-\x38\x18\xfb\xb1\x7e\xde\xe4\x1b\xe8\xd7\x3b\x6a\xb7\x50\x9d\x92\
-\xf4\x60\xf5\x9c\xb1\x8e\xa2\xcf\xe7\xa8\xc7\xf7\x9e\xcb\x3d\x98\
-\xab\xc1\xb2\x06\x5c\xee\x10\x6c\x2f\x97\x07\x5c\x50\x2d\xb1\x76\
-\x54\x30\x4f\x15\xcc\x19\x05\x46\x9f\x09\x6c\xb7\x87\x07\xbb\xf5\
-\xb7\x70\x77\xaf\xd6\x64\x38\xfa\xc4\xee\x60\x5a\xb5\x5e\x36\x6c\
-\x03\xad\x5e\x83\xdd\x81\x98\xf4\x0b\xb9\x06\x7a\x59\xd2\x08\xd4\
-\xad\xc8\x58\xb9\x1e\xed\x3b\x03\x89\xd0\x76\xa3\x87\x7b\xad\x0e\
-\x47\xa8\x35\x02\x8e\x50\xe7\xe8\x70\xc4\x54\xa7\xa3\xa3\xe8\xe8\
-\x33\xd3\x6d\xd5\xf2\x2e\x5a\x72\x38\xad\x33\xda\xa8\xce\x89\x8c\
-\x4a\x2c\x75\x3a\x75\xa7\x3a\xa7\x72\xaa\xad\x4e\xa7\xee\x54\xe7\
-\x7b\x71\xaa\x73\x38\xad\x3b\xda\xa9\xee\xa9\x9c\x4a\xd5\xe9\xd4\
-\x9d\xea\x9e\xca\xa9\xae\x3a\x9d\xba\x53\xdd\xef\xc5\xa9\xde\xe1\
-\xb4\xb5\x43\x3f\x37\xf5\xd9\x1e\x62\xcc\x01\xef\x5e\x5a\x70\x29\
-\x82\xda\x8c\x8f\xbe\x96\x0a\x47\x9b\xda\xa1\xa3\xe8\xc0\xa5\xa7\
-\xa1\x53\x38\xdb\xd0\xd1\x74\xf4\x08\x74\x87\x38\xd5\x52\x38\xeb\
-\xb4\x4e\xb5\x46\x39\xd5\x3a\xc1\x5a\x5a\x0a\x67\x9b\xd6\xa9\xea\
-\x74\xd2\xa9\x27\xa1\x53\x38\xdb\xd0\xd1\x74\xf4\x08\x74\x07\x39\
-\x55\xe1\xac\xd3\x3a\xd5\x1d\xe5\x54\xf7\x14\x6b\xa9\x70\xb6\x69\
-\x9d\xaa\x4e\x27\x9d\x7a\x12\x3a\x85\xb3\x0d\x1d\x4d\x47\x9f\x91\
-\x6e\xcf\x0f\x09\x7d\xb3\x6b\xb5\x8d\x97\x2f\x9a\xe6\x54\xfe\xfe\
-\x0e\xf7\xff\x01\x87\x91\x73\x66\
-\x00\x00\x02\x13\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x2e\x35\x20\
-\x30\x6c\x2d\x2e\x35\x20\x31\x2e\x31\x39\x63\x2d\x2e\x31\x2e\x30\
-\x33\x2d\x2e\x31\x39\x2e\x30\x38\x2d\x2e\x32\x38\x2e\x31\x33\x6c\
-\x2d\x31\x2e\x31\x39\x2d\x2e\x35\x2d\x2e\x37\x32\x2e\x37\x32\x2e\
-\x35\x20\x31\x2e\x31\x39\x63\x2d\x2e\x30\x35\x2e\x31\x2d\x2e\x30\
-\x39\x2e\x31\x38\x2d\x2e\x31\x33\x2e\x32\x38\x6c\x2d\x31\x2e\x31\
-\x39\x2e\x35\x76\x31\x6c\x31\x2e\x31\x39\x2e\x35\x63\x2e\x30\x34\
-\x2e\x31\x2e\x30\x38\x2e\x31\x38\x2e\x31\x33\x2e\x32\x38\x6c\x2d\
-\x2e\x35\x20\x31\x2e\x31\x39\x2e\x37\x32\x2e\x37\x32\x20\x31\x2e\
-\x31\x39\x2d\x2e\x35\x63\x2e\x30\x39\x2e\x30\x34\x2e\x31\x38\x2e\
-\x30\x39\x2e\x32\x38\x2e\x31\x33\x6c\x2e\x35\x20\x31\x2e\x31\x39\
-\x68\x31\x6c\x2e\x35\x2d\x31\x2e\x31\x39\x63\x2e\x30\x39\x2d\x2e\
-\x30\x34\x2e\x31\x39\x2d\x2e\x30\x38\x2e\x32\x38\x2d\x2e\x31\x33\
-\x6c\x31\x2e\x31\x39\x2e\x35\x2e\x37\x32\x2d\x2e\x37\x32\x2d\x2e\
-\x35\x2d\x31\x2e\x31\x39\x63\x2e\x30\x34\x2d\x2e\x30\x39\x2e\x30\
-\x39\x2d\x2e\x31\x39\x2e\x31\x33\x2d\x2e\x32\x38\x6c\x31\x2e\x31\
-\x39\x2d\x2e\x35\x76\x2d\x31\x6c\x2d\x31\x2e\x31\x39\x2d\x2e\x35\
-\x63\x2d\x2e\x30\x33\x2d\x2e\x30\x39\x2d\x2e\x30\x38\x2d\x2e\x31\
-\x39\x2d\x2e\x31\x33\x2d\x2e\x32\x38\x6c\x2e\x35\x2d\x31\x2e\x31\
-\x39\x2d\x2e\x37\x32\x2d\x2e\x37\x32\x2d\x31\x2e\x31\x39\x2e\x35\
-\x63\x2d\x2e\x30\x39\x2d\x2e\x30\x34\x2d\x2e\x31\x39\x2d\x2e\x30\
-\x39\x2d\x2e\x32\x38\x2d\x2e\x31\x33\x6c\x2d\x2e\x35\x2d\x31\x2e\
-\x31\x39\x68\x2d\x31\x7a\x6d\x2e\x35\x20\x32\x2e\x35\x63\x2e\x38\
-\x33\x20\x30\x20\x31\x2e\x35\x2e\x36\x37\x20\x31\x2e\x35\x20\x31\
-\x2e\x35\x73\x2d\x2e\x36\x37\x20\x31\x2e\x35\x2d\x31\x2e\x35\x20\
-\x31\x2e\x35\x2d\x31\x2e\x35\x2d\x2e\x36\x37\x2d\x31\x2e\x35\x2d\
-\x31\x2e\x35\x2e\x36\x37\x2d\x31\x2e\x35\x20\x31\x2e\x35\x2d\x31\
-\x2e\x35\x7a\x22\x0d\x0a\x20\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\
-\x67\x3e\
-\x00\x00\x1c\x57\
+\x00\x00\x1d\x11\
 \x3c\
 \x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
 \x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\x55\x54\x46\
 \x2d\x38\x22\x3f\x3e\x0d\x0a\x3c\x21\x44\x4f\x43\x54\x59\x50\x45\
 \x20\x73\x76\x67\x20\x50\x55\x42\x4c\x49\x43\x20\x22\x2d\x2f\x2f\
 \x57\x33\x43\x2f\x2f\x44\x54\x44\x20\x53\x56\x47\x20\x31\x2e\x31\
 \x2f\x2f\x45\x4e\x22\x20\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\
 \x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x47\x72\x61\x70\x68\x69\x63\
 \x73\x2f\x53\x56\x47\x2f\x31\x2e\x31\x2f\x44\x54\x44\x2f\x73\x76\
 \x67\x31\x31\x2e\x64\x74\x64\x22\x3e\x0d\x0a\x3c\x73\x76\x67\x20\
 \x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\x32\x22\x20\x77\x69\
-\x64\x74\x68\x3d\x22\x33\x34\x2e\x30\x31\x6d\x6d\x22\x20\x68\x65\
-\x69\x67\x68\x74\x3d\x22\x33\x34\x2e\x30\x31\x6d\x6d\x22\x20\x76\
-\x69\x65\x77\x42\x6f\x78\x3d\x22\x31\x32\x37\x30\x30\x20\x31\x37\
-\x39\x30\x30\x20\x33\x34\x30\x31\x20\x33\x34\x30\x31\x22\x20\x70\
+\x64\x74\x68\x3d\x22\x33\x33\x2e\x30\x31\x6d\x6d\x22\x20\x68\x65\
+\x69\x67\x68\x74\x3d\x22\x33\x33\x2e\x30\x31\x6d\x6d\x22\x20\x76\
+\x69\x65\x77\x42\x6f\x78\x3d\x22\x31\x33\x30\x31\x33\x20\x31\x37\
+\x31\x30\x30\x20\x33\x33\x30\x31\x20\x33\x33\x30\x31\x22\x20\x70\
 \x72\x65\x73\x65\x72\x76\x65\x41\x73\x70\x65\x63\x74\x52\x61\x74\
 \x69\x6f\x3d\x22\x78\x4d\x69\x64\x59\x4d\x69\x64\x22\x20\x66\x69\
 \x6c\x6c\x2d\x72\x75\x6c\x65\x3d\x22\x65\x76\x65\x6e\x6f\x64\x64\
 \x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\
 \x32\x38\x2e\x32\x32\x32\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\
 \x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\
 \x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\
@@ -966,354 +877,369 @@
 \x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\
 \x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x43\x75\x73\
 \x74\x6f\x6d\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\
 \x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x33\x22\x3e\x0d\x0a\x20\x20\
 \x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\x3d\x22\
 \x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x73\x74\x72\
 \x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x66\x69\x6c\x6c\x3d\
-\x22\x6e\x6f\x6e\x65\x22\x20\x78\x3d\x22\x31\x32\x37\x30\x30\x22\
-\x20\x79\x3d\x22\x31\x37\x39\x30\x30\x22\x20\x77\x69\x64\x74\x68\
-\x3d\x22\x33\x34\x30\x31\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\
-\x33\x34\x30\x31\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x2f\x67\
-\x3e\x0d\x0a\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x3c\
-\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x47\x72\x6f\x75\x70\x22\x3e\
-\x0d\x0a\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\
-\x47\x72\x6f\x75\x70\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x67\
+\x22\x6e\x6f\x6e\x65\x22\x20\x78\x3d\x22\x31\x33\x30\x31\x33\x22\
+\x20\x79\x3d\x22\x31\x37\x31\x30\x30\x22\x20\x77\x69\x64\x74\x68\
+\x3d\x22\x33\x33\x30\x31\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\
+\x33\x33\x30\x31\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x70\
+\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x72\x67\x62\x28\x32\x35\
+\x35\x2c\x32\x35\x35\x2c\x32\x35\x35\x29\x22\x20\x66\x69\x6c\x6c\
+\x2d\x6f\x70\x61\x63\x69\x74\x79\x3d\x22\x30\x2e\x32\x22\x20\x73\
+\x74\x72\x6f\x6b\x65\x3d\x22\x72\x67\x62\x28\x32\x35\x35\x2c\x32\
+\x35\x35\x2c\x32\x35\x35\x29\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
+\x6f\x70\x61\x63\x69\x74\x79\x3d\x22\x30\x2e\x32\x22\x20\x64\x3d\
+\x22\x4d\x20\x31\x34\x36\x36\x33\x2c\x32\x30\x34\x30\x30\x20\x4c\
+\x20\x31\x33\x30\x31\x33\x2c\x32\x30\x34\x30\x30\x20\x31\x33\x30\
+\x31\x33\x2c\x31\x37\x31\x30\x30\x20\x31\x36\x33\x31\x33\x2c\x31\
+\x37\x31\x30\x30\x20\x31\x36\x33\x31\x33\x2c\x32\x30\x34\x30\x30\
+\x20\x31\x34\x36\x36\x33\x2c\x32\x30\x34\x30\x30\x20\x5a\x22\x2f\
+\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\
+\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\
+\x73\x3d\x22\x47\x72\x6f\x75\x70\x22\x3e\x0d\x0a\x20\x20\x20\x20\
+\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x47\x72\x6f\x75\x70\x22\
+\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\
+\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\
+\x72\x61\x77\x69\x6e\x67\x2e\x4f\x70\x65\x6e\x42\x65\x7a\x69\x65\
+\x72\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\
+\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x34\x22\x3e\x0d\x0a\x20\x20\
+\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\
+\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x73\
+\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x66\x69\x6c\
+\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x78\x3d\x22\x31\x33\x30\x37\
+\x32\x22\x20\x79\x3d\x22\x31\x37\x31\x34\x31\x22\x20\x77\x69\x64\
+\x74\x68\x3d\x22\x32\x30\x31\x22\x20\x68\x65\x69\x67\x68\x74\x3d\
+\x22\x39\x39\x36\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\
+\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\
+\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x72\x67\x62\x28\x31\x30\
+\x32\x2c\x31\x30\x32\x2c\x31\x30\x32\x29\x22\x20\x73\x74\x72\x6f\
+\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x30\x30\x22\x20\x73\
+\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\
+\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\
+\x6e\x65\x63\x61\x70\x3d\x22\x73\x71\x75\x61\x72\x65\x22\x20\x64\
+\x3d\x22\x4d\x20\x31\x33\x31\x37\x32\x2c\x31\x37\x32\x34\x31\x20\
+\x4c\x20\x31\x33\x31\x37\x32\x2c\x31\x38\x30\x33\x36\x22\x2f\x3e\
+\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\
+\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x67\
 \x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\
 \x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x4f\x70\x65\
 \x6e\x42\x65\x7a\x69\x65\x72\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x34\
+\x20\x20\x20\x20\x20\x20\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x35\
 \x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\
 \x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\
 \x42\x6f\x78\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\
 \x65\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x78\
-\x3d\x22\x31\x32\x38\x32\x32\x22\x20\x79\x3d\x22\x31\x37\x39\x39\
+\x3d\x22\x31\x34\x35\x36\x31\x22\x20\x79\x3d\x22\x31\x37\x31\x34\
 \x31\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x32\x30\x31\x22\x20\x68\
-\x65\x69\x67\x68\x74\x3d\x22\x39\x39\x37\x22\x2f\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\
-\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\
-\x72\x67\x62\x28\x31\x30\x32\x2c\x31\x30\x32\x2c\x31\x30\x32\x29\
-\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\
-\x32\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\
-\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\x72\
-\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x63\x61\x70\x3d\x22\x73\x71\x75\
-\x61\x72\x65\x22\x20\x64\x3d\x22\x4d\x20\x31\x32\x39\x32\x32\x2c\
-\x31\x38\x30\x39\x31\x20\x4c\x20\x31\x32\x39\x32\x32\x2c\x31\x38\
-\x38\x38\x36\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x2f\
-\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\
-\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\
-\x6e\x67\x2e\x4f\x70\x65\x6e\x42\x65\x7a\x69\x65\x72\x53\x68\x61\
+\x65\x69\x67\x68\x74\x3d\x22\x32\x31\x33\x35\x22\x2f\x3e\x0d\x0a\
+\x20\x20\x20\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\
+\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\
+\x22\x72\x67\x62\x28\x31\x30\x32\x2c\x31\x30\x32\x2c\x31\x30\x32\
+\x29\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\
+\x22\x32\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\
+\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\
+\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x63\x61\x70\x3d\x22\x73\x71\
+\x75\x61\x72\x65\x22\x20\x64\x3d\x22\x4d\x20\x31\x34\x36\x36\x31\
+\x2c\x31\x37\x32\x34\x32\x20\x4c\x20\x31\x34\x36\x36\x31\x2c\x31\
+\x39\x31\x37\x35\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\
+\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\
+\x20\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\
+\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\
+\x69\x6e\x67\x2e\x45\x6c\x6c\x69\x70\x73\x65\x53\x68\x61\x70\x65\
+\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x67\x20\x69\x64\x3d\
+\x22\x69\x64\x36\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\
+\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\
+\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\
+\x22\x6e\x6f\x6e\x65\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\
+\x65\x22\x20\x78\x3d\x22\x31\x33\x35\x36\x34\x22\x20\x79\x3d\x22\
+\x31\x37\x31\x36\x30\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x37\x30\
+\x36\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x31\x35\x34\x31\x22\
+\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x70\x61\x74\x68\
+\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x73\x74\x72\
+\x6f\x6b\x65\x3d\x22\x72\x67\x62\x28\x31\x30\x32\x2c\x31\x30\x32\
+\x2c\x31\x30\x32\x29\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\
+\x64\x74\x68\x3d\x22\x32\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\
+\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\
+\x22\x20\x64\x3d\x22\x4d\x20\x31\x33\x39\x31\x37\x2c\x31\x38\x36\
+\x30\x30\x20\x43\x20\x31\x33\x38\x37\x32\x2c\x31\x38\x36\x30\x30\
+\x20\x31\x33\x38\x32\x39\x2c\x31\x38\x35\x36\x39\x20\x31\x33\x37\
+\x39\x30\x2c\x31\x38\x35\x31\x30\x20\x31\x33\x37\x35\x32\x2c\x31\
+\x38\x34\x35\x31\x20\x31\x33\x37\x32\x30\x2c\x31\x38\x33\x36\x37\
+\x20\x31\x33\x36\x39\x38\x2c\x31\x38\x32\x36\x35\x20\x31\x33\x36\
+\x37\x36\x2c\x31\x38\x31\x36\x33\x20\x31\x33\x36\x36\x34\x2c\x31\
+\x38\x30\x34\x38\x20\x31\x33\x36\x36\x34\x2c\x31\x37\x39\x33\x30\
+\x20\x31\x33\x36\x36\x34\x2c\x31\x37\x38\x31\x32\x20\x31\x33\x36\
+\x37\x36\x2c\x31\x37\x36\x39\x37\x20\x31\x33\x36\x39\x38\x2c\x31\
+\x37\x35\x39\x35\x20\x31\x33\x37\x32\x30\x2c\x31\x37\x34\x39\x33\
+\x20\x31\x33\x37\x35\x32\x2c\x31\x37\x34\x30\x39\x20\x31\x33\x37\
+\x39\x30\x2c\x31\x37\x33\x35\x30\x20\x31\x33\x38\x32\x39\x2c\x31\
+\x37\x32\x39\x31\x20\x31\x33\x38\x37\x32\x2c\x31\x37\x32\x36\x30\
+\x20\x31\x33\x39\x31\x37\x2c\x31\x37\x32\x36\x30\x20\x31\x33\x39\
+\x36\x31\x2c\x31\x37\x32\x36\x30\x20\x31\x34\x30\x30\x34\x2c\x31\
+\x37\x32\x39\x31\x20\x31\x34\x30\x34\x33\x2c\x31\x37\x33\x35\x30\
+\x20\x31\x34\x30\x38\x31\x2c\x31\x37\x34\x30\x39\x20\x31\x34\x31\
+\x31\x33\x2c\x31\x37\x34\x39\x33\x20\x31\x34\x31\x33\x35\x2c\x31\
+\x37\x35\x39\x35\x20\x31\x34\x31\x35\x37\x2c\x31\x37\x36\x39\x37\
+\x20\x31\x34\x31\x36\x39\x2c\x31\x37\x38\x31\x32\x20\x31\x34\x31\
+\x36\x39\x2c\x31\x37\x39\x33\x30\x20\x31\x34\x31\x36\x39\x2c\x31\
+\x38\x30\x34\x38\x20\x31\x34\x31\x35\x37\x2c\x31\x38\x31\x36\x33\
+\x20\x31\x34\x31\x33\x35\x2c\x31\x38\x32\x36\x35\x20\x31\x34\x31\
+\x31\x33\x2c\x31\x38\x33\x36\x37\x20\x31\x34\x30\x38\x31\x2c\x31\
+\x38\x34\x35\x31\x20\x31\x34\x30\x34\x33\x2c\x31\x38\x35\x31\x30\
+\x20\x31\x34\x30\x30\x34\x2c\x31\x38\x35\x36\x39\x20\x31\x33\x39\
+\x36\x31\x2c\x31\x38\x36\x30\x30\x20\x31\x33\x39\x31\x37\x2c\x31\
+\x38\x36\x30\x30\x20\x5a\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\
+\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\
+\x0d\x0a\x20\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\
+\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\
+\x61\x77\x69\x6e\x67\x2e\x45\x6c\x6c\x69\x70\x73\x65\x53\x68\x61\
 \x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x67\x20\x69\
-\x64\x3d\x22\x69\x64\x35\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\
+\x64\x3d\x22\x69\x64\x37\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\
 \x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\
 \x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x73\x74\x72\x6f\x6b\
 \x65\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\
-\x6f\x6e\x65\x22\x20\x78\x3d\x22\x31\x34\x33\x31\x31\x22\x20\x79\
-\x3d\x22\x31\x37\x39\x39\x32\x22\x20\x77\x69\x64\x74\x68\x3d\x22\
-\x32\x30\x31\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x31\x33\
-\x34\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x70\x61\
+\x6f\x6e\x65\x22\x20\x78\x3d\x22\x31\x35\x30\x31\x33\x22\x20\x79\
+\x3d\x22\x31\x37\x31\x36\x30\x22\x20\x77\x69\x64\x74\x68\x3d\x22\
+\x37\x38\x36\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x35\x30\
+\x30\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x70\x61\
 \x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x73\
 \x74\x72\x6f\x6b\x65\x3d\x22\x72\x67\x62\x28\x31\x30\x32\x2c\x31\
 \x30\x32\x2c\x31\x30\x32\x29\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
 \x77\x69\x64\x74\x68\x3d\x22\x32\x30\x30\x22\x20\x73\x74\x72\x6f\
 \x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\
-\x6e\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x63\
-\x61\x70\x3d\x22\x73\x71\x75\x61\x72\x65\x22\x20\x64\x3d\x22\x4d\
-\x20\x31\x34\x34\x31\x31\x2c\x31\x38\x30\x39\x32\x20\x4c\x20\x31\
-\x34\x34\x31\x31\x2c\x32\x30\x30\x32\x35\x22\x2f\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\
-\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\
-\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x45\x6c\x6c\x69\x70\x73\
-\x65\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\
-\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x36\x22\x3e\x0d\x0a\x20\x20\
-\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\
-\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x73\
-\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x66\x69\x6c\
-\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x78\x3d\x22\x31\x33\x33\x31\
-\x34\x22\x20\x79\x3d\x22\x31\x38\x30\x31\x30\x22\x20\x77\x69\x64\
-\x74\x68\x3d\x22\x37\x30\x36\x22\x20\x68\x65\x69\x67\x68\x74\x3d\
-\x22\x31\x35\x34\x31\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\
-\x20\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\
-\x65\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x72\x67\x62\x28\x31\
-\x30\x32\x2c\x31\x30\x32\x2c\x31\x30\x32\x29\x22\x20\x73\x74\x72\
-\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x30\x30\x22\x20\
-\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\
-\x22\x72\x6f\x75\x6e\x64\x22\x20\x64\x3d\x22\x4d\x20\x31\x33\x36\
-\x36\x37\x2c\x31\x39\x34\x35\x30\x20\x43\x20\x31\x33\x36\x32\x32\
-\x2c\x31\x39\x34\x35\x30\x20\x31\x33\x35\x37\x39\x2c\x31\x39\x34\
-\x31\x39\x20\x31\x33\x35\x34\x30\x2c\x31\x39\x33\x36\x30\x20\x31\
-\x33\x35\x30\x32\x2c\x31\x39\x33\x30\x31\x20\x31\x33\x34\x37\x30\
-\x2c\x31\x39\x32\x31\x37\x20\x31\x33\x34\x34\x38\x2c\x31\x39\x31\
-\x31\x35\x20\x31\x33\x34\x32\x36\x2c\x31\x39\x30\x31\x33\x20\x31\
-\x33\x34\x31\x34\x2c\x31\x38\x38\x39\x38\x20\x31\x33\x34\x31\x34\
-\x2c\x31\x38\x37\x38\x30\x20\x31\x33\x34\x31\x34\x2c\x31\x38\x36\
-\x36\x32\x20\x31\x33\x34\x32\x36\x2c\x31\x38\x35\x34\x37\x20\x31\
-\x33\x34\x34\x38\x2c\x31\x38\x34\x34\x35\x20\x31\x33\x34\x37\x30\
-\x2c\x31\x38\x33\x34\x33\x20\x31\x33\x35\x30\x32\x2c\x31\x38\x32\
-\x35\x39\x20\x31\x33\x35\x34\x30\x2c\x31\x38\x32\x30\x30\x20\x31\
-\x33\x35\x37\x39\x2c\x31\x38\x31\x34\x31\x20\x31\x33\x36\x32\x32\
-\x2c\x31\x38\x31\x31\x30\x20\x31\x33\x36\x36\x37\x2c\x31\x38\x31\
-\x31\x30\x20\x31\x33\x37\x31\x31\x2c\x31\x38\x31\x31\x30\x20\x31\
-\x33\x37\x35\x34\x2c\x31\x38\x31\x34\x31\x20\x31\x33\x37\x39\x33\
-\x2c\x31\x38\x32\x30\x30\x20\x31\x33\x38\x33\x31\x2c\x31\x38\x32\
-\x35\x39\x20\x31\x33\x38\x36\x33\x2c\x31\x38\x33\x34\x33\x20\x31\
-\x33\x38\x38\x35\x2c\x31\x38\x34\x34\x35\x20\x31\x33\x39\x30\x37\
-\x2c\x31\x38\x35\x34\x37\x20\x31\x33\x39\x31\x39\x2c\x31\x38\x36\
-\x36\x32\x20\x31\x33\x39\x31\x39\x2c\x31\x38\x37\x38\x30\x20\x31\
-\x33\x39\x31\x39\x2c\x31\x38\x38\x39\x38\x20\x31\x33\x39\x30\x37\
-\x2c\x31\x39\x30\x31\x33\x20\x31\x33\x38\x38\x35\x2c\x31\x39\x31\
-\x31\x35\x20\x31\x33\x38\x36\x33\x2c\x31\x39\x32\x31\x37\x20\x31\
-\x33\x38\x33\x31\x2c\x31\x39\x33\x30\x31\x20\x31\x33\x37\x39\x33\
-\x2c\x31\x39\x33\x36\x30\x20\x31\x33\x37\x35\x34\x2c\x31\x39\x34\
-\x31\x39\x20\x31\x33\x37\x31\x31\x2c\x31\x39\x34\x35\x30\x20\x31\
-\x33\x36\x36\x37\x2c\x31\x39\x34\x35\x30\x20\x5a\x22\x2f\x3e\x0d\
-\x0a\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\
-\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x67\x20\
-\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\
-\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x45\x6c\x6c\x69\
-\x70\x73\x65\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\
-\x20\x20\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x37\x22\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\
-\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\
-\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x66\
-\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x78\x3d\x22\x31\x34\
-\x37\x36\x33\x22\x20\x79\x3d\x22\x31\x38\x30\x31\x30\x22\x20\x77\
-\x69\x64\x74\x68\x3d\x22\x37\x38\x36\x22\x20\x68\x65\x69\x67\x68\
-\x74\x3d\x22\x32\x35\x30\x30\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\
-\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x6e\
-\x6f\x6e\x65\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x72\x67\x62\
-\x28\x31\x30\x32\x2c\x31\x30\x32\x2c\x31\x30\x32\x29\x22\x20\x73\
-\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x30\x30\
-\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\
-\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x64\x3d\x22\x4d\x20\x31\
-\x35\x31\x35\x36\x2c\x32\x30\x34\x30\x39\x20\x43\x20\x31\x35\x31\
-\x30\x34\x2c\x32\x30\x34\x30\x39\x20\x31\x35\x30\x35\x34\x2c\x32\
-\x30\x33\x35\x36\x20\x31\x35\x30\x30\x39\x2c\x32\x30\x32\x35\x35\
-\x20\x31\x34\x39\x36\x35\x2c\x32\x30\x31\x35\x34\x20\x31\x34\x39\
-\x32\x38\x2c\x32\x30\x30\x30\x39\x20\x31\x34\x39\x30\x32\x2c\x31\
-\x39\x38\x33\x34\x20\x31\x34\x38\x37\x37\x2c\x31\x39\x36\x36\x30\
-\x20\x31\x34\x38\x36\x33\x2c\x31\x39\x34\x36\x31\x20\x31\x34\x38\
-\x36\x33\x2c\x31\x39\x32\x36\x30\x20\x31\x34\x38\x36\x33\x2c\x31\
-\x39\x30\x35\x38\x20\x31\x34\x38\x37\x37\x2c\x31\x38\x38\x35\x39\
-\x20\x31\x34\x39\x30\x32\x2c\x31\x38\x36\x38\x35\x20\x31\x34\x39\
-\x32\x38\x2c\x31\x38\x35\x31\x30\x20\x31\x34\x39\x36\x35\x2c\x31\
-\x38\x33\x36\x35\x20\x31\x35\x30\x30\x39\x2c\x31\x38\x32\x36\x34\
-\x20\x31\x35\x30\x35\x34\x2c\x31\x38\x31\x36\x33\x20\x31\x35\x31\
-\x30\x34\x2c\x31\x38\x31\x31\x30\x20\x31\x35\x31\x35\x36\x2c\x31\
-\x38\x31\x31\x30\x20\x31\x35\x32\x30\x37\x2c\x31\x38\x31\x31\x30\
-\x20\x31\x35\x32\x35\x37\x2c\x31\x38\x31\x36\x33\x20\x31\x35\x33\
-\x30\x32\x2c\x31\x38\x32\x36\x34\x20\x31\x35\x33\x34\x36\x2c\x31\
-\x38\x33\x36\x35\x20\x31\x35\x33\x38\x33\x2c\x31\x38\x35\x31\x30\
-\x20\x31\x35\x34\x30\x39\x2c\x31\x38\x36\x38\x35\x20\x31\x35\x34\
-\x33\x34\x2c\x31\x38\x38\x35\x39\x20\x31\x35\x34\x34\x38\x2c\x31\
-\x39\x30\x35\x38\x20\x31\x35\x34\x34\x38\x2c\x31\x39\x32\x36\x30\
-\x20\x31\x35\x34\x34\x38\x2c\x31\x39\x34\x36\x31\x20\x31\x35\x34\
-\x33\x34\x2c\x31\x39\x36\x36\x30\x20\x31\x35\x34\x30\x39\x2c\x31\
-\x39\x38\x33\x34\x20\x31\x35\x33\x38\x33\x2c\x32\x30\x30\x30\x39\
-\x20\x31\x35\x33\x34\x36\x2c\x32\x30\x31\x35\x34\x20\x31\x35\x33\
-\x30\x32\x2c\x32\x30\x32\x35\x35\x20\x31\x35\x32\x35\x37\x2c\x32\
-\x30\x33\x35\x36\x20\x31\x35\x32\x30\x37\x2c\x32\x30\x34\x30\x39\
-\x20\x31\x35\x31\x35\x36\x2c\x32\x30\x34\x30\x39\x20\x5a\x22\x2f\
-\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\
-\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\
-\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x4c\x69\
-\x6e\x65\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x38\x22\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\x73\
-\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\
-\x73\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x66\x69\
-\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x78\x3d\x22\x31\x35\x38\
-\x30\x30\x22\x20\x79\x3d\x22\x31\x37\x39\x39\x31\x22\x20\x77\x69\
-\x64\x74\x68\x3d\x22\x32\x30\x31\x22\x20\x68\x65\x69\x67\x68\x74\
-\x3d\x22\x33\x31\x37\x36\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\
-\x6e\x65\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x72\x67\x62\x28\
-\x31\x30\x32\x2c\x31\x30\x32\x2c\x31\x30\x32\x29\x22\x20\x73\x74\
-\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x30\x30\x22\
-\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\
-\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
-\x6c\x69\x6e\x65\x63\x61\x70\x3d\x22\x73\x71\x75\x61\x72\x65\x22\
-\x20\x64\x3d\x22\x4d\x20\x31\x35\x39\x30\x30\x2c\x31\x38\x30\x39\
-\x31\x20\x4c\x20\x31\x35\x39\x30\x30\x2c\x32\x31\x30\x36\x36\x22\
-\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x3c\
-\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\
+\x6e\x64\x22\x20\x64\x3d\x22\x4d\x20\x31\x35\x34\x30\x36\x2c\x31\
+\x39\x35\x35\x39\x20\x43\x20\x31\x35\x33\x35\x34\x2c\x31\x39\x35\
+\x35\x39\x20\x31\x35\x33\x30\x34\x2c\x31\x39\x35\x30\x36\x20\x31\
+\x35\x32\x35\x39\x2c\x31\x39\x34\x30\x35\x20\x31\x35\x32\x31\x35\
+\x2c\x31\x39\x33\x30\x34\x20\x31\x35\x31\x37\x38\x2c\x31\x39\x31\
+\x35\x39\x20\x31\x35\x31\x35\x32\x2c\x31\x38\x39\x38\x34\x20\x31\
+\x35\x31\x32\x37\x2c\x31\x38\x38\x31\x30\x20\x31\x35\x31\x31\x33\
+\x2c\x31\x38\x36\x31\x31\x20\x31\x35\x31\x31\x33\x2c\x31\x38\x34\
+\x31\x30\x20\x31\x35\x31\x31\x33\x2c\x31\x38\x32\x30\x38\x20\x31\
+\x35\x31\x32\x37\x2c\x31\x38\x30\x30\x39\x20\x31\x35\x31\x35\x32\
+\x2c\x31\x37\x38\x33\x35\x20\x31\x35\x31\x37\x38\x2c\x31\x37\x36\
+\x36\x30\x20\x31\x35\x32\x31\x35\x2c\x31\x37\x35\x31\x35\x20\x31\
+\x35\x32\x35\x39\x2c\x31\x37\x34\x31\x34\x20\x31\x35\x33\x30\x34\
+\x2c\x31\x37\x33\x31\x33\x20\x31\x35\x33\x35\x34\x2c\x31\x37\x32\
+\x36\x30\x20\x31\x35\x34\x30\x36\x2c\x31\x37\x32\x36\x30\x20\x31\
+\x35\x34\x35\x37\x2c\x31\x37\x32\x36\x30\x20\x31\x35\x35\x30\x37\
+\x2c\x31\x37\x33\x31\x33\x20\x31\x35\x35\x35\x32\x2c\x31\x37\x34\
+\x31\x34\x20\x31\x35\x35\x39\x36\x2c\x31\x37\x35\x31\x35\x20\x31\
+\x35\x36\x33\x33\x2c\x31\x37\x36\x36\x30\x20\x31\x35\x36\x35\x39\
+\x2c\x31\x37\x38\x33\x35\x20\x31\x35\x36\x38\x34\x2c\x31\x38\x30\
+\x30\x39\x20\x31\x35\x36\x39\x38\x2c\x31\x38\x32\x30\x38\x20\x31\
+\x35\x36\x39\x38\x2c\x31\x38\x34\x31\x30\x20\x31\x35\x36\x39\x38\
+\x2c\x31\x38\x36\x31\x31\x20\x31\x35\x36\x38\x34\x2c\x31\x38\x38\
+\x31\x30\x20\x31\x35\x36\x35\x39\x2c\x31\x38\x39\x38\x34\x20\x31\
+\x35\x36\x33\x33\x2c\x31\x39\x31\x35\x39\x20\x31\x35\x35\x39\x36\
+\x2c\x31\x39\x33\x30\x34\x20\x31\x35\x35\x35\x32\x2c\x31\x39\x34\
+\x30\x35\x20\x31\x35\x35\x30\x37\x2c\x31\x39\x35\x30\x36\x20\x31\
+\x35\x34\x35\x37\x2c\x31\x39\x35\x35\x39\x20\x31\x35\x34\x30\x36\
+\x2c\x31\x39\x35\x35\x39\x20\x5a\x22\x2f\x3e\x0d\x0a\x20\x20\x20\
+\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x2f\
+\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\
 \x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\
-\x64\x72\x61\x77\x69\x6e\x67\x2e\x4f\x70\x65\x6e\x42\x65\x7a\x69\
-\x65\x72\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x3c\x67\x20\x69\x64\x3d\x22\x69\x64\x39\x22\x3e\x0d\x0a\x20\x20\
-\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\x3d\
-\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x73\x74\
-\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x66\x69\x6c\x6c\
-\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x78\x3d\x22\x31\x32\x38\x32\x35\
-\x22\x20\x79\x3d\x22\x31\x39\x30\x32\x31\x22\x20\x77\x69\x64\x74\
-\x68\x3d\x22\x32\x39\x34\x38\x22\x20\x68\x65\x69\x67\x68\x74\x3d\
-\x22\x32\x31\x36\x34\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\
-\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\
-\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x72\x67\x62\x28\x31\x38\
-\x34\x2c\x30\x2c\x37\x31\x29\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
-\x77\x69\x64\x74\x68\x3d\x22\x31\x35\x30\x22\x20\x73\x74\x72\x6f\
-\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\
-\x6e\x64\x22\x20\x64\x3d\x22\x4d\x20\x31\x35\x36\x39\x37\x2c\x32\
-\x30\x39\x39\x33\x20\x43\x20\x31\x35\x36\x30\x32\x2c\x32\x31\x31\
-\x36\x33\x20\x31\x35\x35\x35\x39\x2c\x32\x31\x30\x39\x30\x20\x31\
-\x35\x34\x39\x35\x2c\x32\x30\x39\x36\x37\x20\x31\x35\x34\x33\x31\
-\x2c\x32\x30\x38\x34\x34\x20\x31\x35\x33\x39\x30\x2c\x32\x30\x37\
-\x32\x36\x20\x31\x35\x32\x39\x35\x2c\x32\x30\x39\x33\x38\x20\x31\
-\x35\x32\x30\x31\x2c\x32\x31\x32\x30\x30\x20\x31\x35\x31\x35\x38\
-\x2c\x32\x31\x30\x38\x38\x20\x31\x35\x30\x39\x33\x2c\x32\x30\x39\
-\x30\x32\x20\x31\x35\x30\x32\x38\x2c\x32\x30\x37\x31\x36\x20\x31\
-\x34\x39\x38\x36\x2c\x32\x30\x35\x34\x33\x20\x31\x34\x38\x39\x34\
-\x2c\x32\x30\x38\x36\x33\x20\x4c\x20\x31\x34\x38\x39\x34\x2c\x32\
-\x30\x38\x35\x35\x20\x43\x20\x31\x34\x38\x30\x31\x2c\x32\x31\x32\
-\x34\x34\x20\x31\x34\x37\x35\x38\x2c\x32\x31\x30\x38\x30\x20\x31\
-\x34\x36\x39\x32\x2c\x32\x30\x38\x31\x30\x20\x31\x34\x36\x32\x36\
-\x2c\x32\x30\x35\x33\x38\x20\x31\x34\x35\x38\x35\x2c\x32\x30\x32\
-\x39\x31\x20\x31\x34\x34\x39\x33\x2c\x32\x30\x37\x35\x35\x20\x31\
-\x34\x33\x39\x39\x2c\x32\x31\x33\x30\x37\x20\x31\x34\x33\x37\x37\
-\x2c\x32\x31\x30\x39\x33\x20\x31\x34\x32\x39\x32\x2c\x32\x30\x36\
-\x39\x35\x20\x31\x34\x32\x32\x37\x2c\x32\x30\x33\x31\x31\x20\x31\
-\x34\x31\x38\x32\x2c\x31\x39\x39\x37\x35\x20\x31\x34\x30\x39\x31\
-\x2c\x32\x30\x36\x32\x36\x20\x4c\x20\x31\x34\x30\x39\x31\x2c\x32\
-\x30\x36\x32\x33\x20\x43\x20\x31\x34\x30\x30\x30\x2c\x32\x31\x33\
-\x38\x36\x20\x31\x33\x39\x39\x39\x2c\x32\x31\x31\x36\x36\x20\x31\
-\x33\x38\x39\x32\x2c\x32\x30\x35\x34\x35\x20\x31\x33\x38\x32\x38\
-\x2c\x32\x30\x30\x32\x36\x20\x31\x33\x37\x38\x33\x2c\x31\x39\x35\
-\x35\x36\x20\x31\x33\x36\x39\x32\x2c\x32\x30\x34\x34\x30\x20\x31\
-\x33\x36\x30\x30\x2c\x32\x31\x34\x36\x38\x20\x31\x33\x35\x37\x33\
-\x2c\x32\x31\x31\x36\x36\x20\x31\x33\x34\x39\x32\x2c\x32\x30\x33\
-\x34\x32\x20\x31\x33\x34\x32\x37\x2c\x31\x39\x36\x34\x35\x20\x31\
-\x33\x33\x38\x36\x2c\x31\x39\x30\x35\x33\x20\x31\x33\x32\x39\x32\
-\x2c\x32\x30\x32\x33\x33\x20\x31\x33\x32\x30\x30\x2c\x32\x31\x34\
-\x38\x30\x20\x31\x33\x32\x30\x30\x2c\x32\x31\x32\x38\x36\x20\x31\
-\x33\x30\x39\x35\x2c\x32\x30\x31\x31\x31\x20\x31\x33\x30\x33\x35\
-\x2c\x31\x39\x32\x30\x30\x20\x31\x32\x39\x39\x34\x2c\x31\x38\x34\
-\x33\x39\x20\x31\x32\x39\x30\x30\x2c\x31\x39\x39\x37\x39\x22\x2f\
-\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\
-\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x3c\x2f\x67\x3e\x0d\
-\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x3c\x2f\x67\x3e\x0d\x0a\
-\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x01\x50\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x20\x30\x63\
-\x2d\x2e\x35\x35\x20\x30\x2d\x31\x20\x2e\x34\x35\x2d\x31\x20\x31\
-\x68\x2d\x31\x63\x2d\x2e\x35\x35\x20\x30\x2d\x31\x20\x2e\x34\x35\
-\x2d\x31\x20\x31\x68\x37\x63\x30\x2d\x2e\x35\x35\x2d\x2e\x34\x35\
-\x2d\x31\x2d\x31\x2d\x31\x68\x2d\x31\x63\x30\x2d\x2e\x35\x35\x2d\
-\x2e\x34\x35\x2d\x31\x2d\x31\x2d\x31\x68\x2d\x31\x7a\x6d\x2d\x32\
-\x20\x33\x76\x34\x2e\x38\x31\x63\x30\x20\x2e\x31\x31\x2e\x30\x38\
-\x2e\x31\x39\x2e\x31\x39\x2e\x31\x39\x68\x34\x2e\x36\x33\x63\x2e\
-\x31\x31\x20\x30\x20\x2e\x31\x39\x2d\x2e\x30\x38\x2e\x31\x39\x2d\
-\x2e\x31\x39\x76\x2d\x34\x2e\x38\x31\x68\x2d\x31\x76\x33\x2e\x35\
-\x63\x30\x20\x2e\x32\x38\x2d\x2e\x32\x32\x2e\x35\x2d\x2e\x35\x2e\
-\x35\x73\x2d\x2e\x35\x2d\x2e\x32\x32\x2d\x2e\x35\x2d\x2e\x35\x76\
-\x2d\x33\x2e\x35\x68\x2d\x31\x76\x33\x2e\x35\x63\x30\x20\x2e\x32\
-\x38\x2d\x2e\x32\x32\x2e\x35\x2d\x2e\x35\x2e\x35\x73\x2d\x2e\x35\
-\x2d\x2e\x32\x32\x2d\x2e\x35\x2d\x2e\x35\x76\x2d\x33\x2e\x35\x68\
-\x2d\x31\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x00\xb4\
+\x64\x72\x61\x77\x69\x6e\x67\x2e\x4c\x69\x6e\x65\x53\x68\x61\x70\
+\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x67\x20\x69\x64\
+\x3d\x22\x69\x64\x38\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\
+\x3c\x72\x65\x63\x74\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\
+\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x73\x74\x72\x6f\x6b\x65\
+\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\
+\x6e\x65\x22\x20\x78\x3d\x22\x31\x36\x30\x35\x30\x22\x20\x79\x3d\
+\x22\x31\x37\x31\x34\x31\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x32\
+\x30\x31\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x33\x31\x37\x36\
+\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x70\x61\x74\
+\x68\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x73\x74\
+\x72\x6f\x6b\x65\x3d\x22\x72\x67\x62\x28\x31\x30\x32\x2c\x31\x30\
+\x32\x2c\x31\x30\x32\x29\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\
+\x69\x64\x74\x68\x3d\x22\x32\x30\x30\x22\x20\x73\x74\x72\x6f\x6b\
+\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\
+\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x63\x61\
+\x70\x3d\x22\x73\x71\x75\x61\x72\x65\x22\x20\x64\x3d\x22\x4d\x20\
+\x31\x36\x31\x35\x30\x2c\x31\x37\x32\x34\x31\x20\x4c\x20\x31\x36\
+\x31\x35\x30\x2c\x32\x30\x32\x31\x36\x22\x2f\x3e\x0d\x0a\x20\x20\
+\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\
+\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\
+\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\
+\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\
+\x67\x2e\x4f\x70\x65\x6e\x42\x65\x7a\x69\x65\x72\x53\x68\x61\x70\
+\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x3c\x67\x20\x69\x64\x3d\
+\x22\x69\x64\x39\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x72\
+\x65\x63\x74\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\
+\x69\x6e\x67\x42\x6f\x78\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\
+\x6e\x6f\x6e\x65\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\
+\x22\x20\x78\x3d\x22\x31\x33\x30\x37\x35\x22\x20\x79\x3d\x22\x31\
+\x38\x31\x37\x32\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x32\x39\x34\
+\x38\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x31\x36\x34\x22\
+\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\
+\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x73\x74\x72\x6f\
+\x6b\x65\x3d\x22\x72\x67\x62\x28\x31\x38\x34\x2c\x30\x2c\x37\x31\
+\x29\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\
+\x22\x31\x35\x30\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\
+\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x64\x3d\
+\x22\x4d\x20\x31\x35\x39\x34\x37\x2c\x32\x30\x31\x34\x33\x20\x43\
+\x20\x31\x35\x38\x35\x32\x2c\x32\x30\x33\x31\x34\x20\x31\x35\x38\
+\x30\x39\x2c\x32\x30\x32\x34\x30\x20\x31\x35\x37\x34\x35\x2c\x32\
+\x30\x31\x31\x37\x20\x31\x35\x36\x38\x31\x2c\x31\x39\x39\x39\x34\
+\x20\x31\x35\x36\x34\x30\x2c\x31\x39\x38\x37\x36\x20\x31\x35\x35\
+\x34\x35\x2c\x32\x30\x30\x38\x38\x20\x31\x35\x34\x35\x31\x2c\x32\
+\x30\x33\x35\x30\x20\x31\x35\x34\x30\x38\x2c\x32\x30\x32\x33\x38\
+\x20\x31\x35\x33\x34\x33\x2c\x32\x30\x30\x35\x32\x20\x31\x35\x32\
+\x37\x38\x2c\x31\x39\x38\x36\x36\x20\x31\x35\x32\x33\x36\x2c\x31\
+\x39\x36\x39\x33\x20\x31\x35\x31\x34\x34\x2c\x32\x30\x30\x31\x34\
+\x20\x4c\x20\x31\x35\x31\x34\x34\x2c\x32\x30\x30\x30\x36\x20\x43\
+\x20\x31\x35\x30\x35\x31\x2c\x32\x30\x33\x39\x34\x20\x31\x35\x30\
+\x30\x38\x2c\x32\x30\x32\x33\x30\x20\x31\x34\x39\x34\x32\x2c\x31\
+\x39\x39\x36\x30\x20\x31\x34\x38\x37\x36\x2c\x31\x39\x36\x38\x38\
+\x20\x31\x34\x38\x33\x35\x2c\x31\x39\x34\x34\x31\x20\x31\x34\x37\
+\x34\x33\x2c\x31\x39\x39\x30\x35\x20\x31\x34\x36\x34\x39\x2c\x32\
+\x30\x34\x35\x37\x20\x31\x34\x36\x32\x37\x2c\x32\x30\x32\x34\x33\
+\x20\x31\x34\x35\x34\x32\x2c\x31\x39\x38\x34\x35\x20\x31\x34\x34\
+\x37\x37\x2c\x31\x39\x34\x36\x32\x20\x31\x34\x34\x33\x32\x2c\x31\
+\x39\x31\x32\x36\x20\x31\x34\x33\x34\x31\x2c\x31\x39\x37\x37\x36\
+\x20\x4c\x20\x31\x34\x33\x34\x31\x2c\x31\x39\x37\x37\x33\x20\x43\
+\x20\x31\x34\x32\x35\x30\x2c\x32\x30\x35\x33\x36\x20\x31\x34\x32\
+\x34\x39\x2c\x32\x30\x33\x31\x37\x20\x31\x34\x31\x34\x32\x2c\x31\
+\x39\x36\x39\x36\x20\x31\x34\x30\x37\x38\x2c\x31\x39\x31\x37\x36\
+\x20\x31\x34\x30\x33\x33\x2c\x31\x38\x37\x30\x36\x20\x31\x33\x39\
+\x34\x32\x2c\x31\x39\x35\x39\x30\x20\x31\x33\x38\x35\x30\x2c\x32\
+\x30\x36\x31\x39\x20\x31\x33\x38\x32\x33\x2c\x32\x30\x33\x31\x37\
+\x20\x31\x33\x37\x34\x32\x2c\x31\x39\x34\x39\x33\x20\x31\x33\x36\
+\x37\x37\x2c\x31\x38\x37\x39\x35\x20\x31\x33\x36\x33\x36\x2c\x31\
+\x38\x32\x30\x34\x20\x31\x33\x35\x34\x32\x2c\x31\x39\x33\x38\x33\
+\x20\x31\x33\x34\x35\x30\x2c\x32\x30\x36\x33\x30\x20\x31\x33\x34\
+\x35\x30\x2c\x32\x30\x34\x33\x37\x20\x31\x33\x33\x34\x35\x2c\x31\
+\x39\x32\x36\x31\x20\x31\x33\x32\x38\x35\x2c\x31\x38\x33\x35\x30\
+\x20\x31\x33\x32\x34\x34\x2c\x31\x37\x35\x38\x39\x20\x31\x33\x31\
+\x35\x30\x2c\x31\x39\x31\x33\x30\x22\x2f\x3e\x0d\x0a\x20\x20\x20\
+\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x2f\x67\x3e\
+\x0d\x0a\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x3c\x2f\x67\
+\x3e\x0d\x0a\x20\x3c\x2f\x67\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
+\
+\x00\x00\x01\x7f\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
-\x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x30\x30\x30\x40\x40\x40\x50\x50\x50\x60\x60\x60\x60\x6f\x74\
-\x80\x80\x80\x76\x94\x9e\x81\xa2\xac\xb0\xb0\xb0\xcb\xce\xcf\xae\
-\xd8\xe6\xad\xd8\xe6\xad\xd8\xe6\x0c\x60\x27\x73\x00\x00\x00\x3f\
-\x49\x44\x41\x54\x28\xcf\x63\x38\x83\x09\x18\xce\xbd\x7b\xf7\x52\
-\x50\x50\xf2\x1d\x12\x18\x15\x23\x46\x6c\xa2\xa0\xe0\xbc\x51\x31\
-\x9c\x62\xa7\x56\xad\x5a\x2e\x28\x28\xbe\x0a\x0c\x0a\x05\x05\xab\
-\x56\xad\x62\x38\x28\x88\x01\xa8\x2e\x76\x6a\x15\x06\x00\x00\x9e\
-\xe8\xcb\xd7\xeb\xf5\xf2\x67\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
-\x42\x60\x82\
-\x00\x00\x01\x03\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x20\x30\x63\
-\x2d\x31\x2e\x36\x36\x20\x30\x2d\x33\x20\x31\x2e\x33\x34\x2d\x33\
-\x20\x33\x20\x30\x20\x32\x20\x33\x20\x35\x20\x33\x20\x35\x73\x33\
-\x2d\x33\x20\x33\x2d\x35\x63\x30\x2d\x31\x2e\x36\x36\x2d\x31\x2e\
-\x33\x34\x2d\x33\x2d\x33\x2d\x33\x7a\x6d\x30\x20\x31\x63\x31\x2e\
-\x31\x31\x20\x30\x20\x32\x20\x2e\x39\x20\x32\x20\x32\x20\x30\x20\
-\x31\x2e\x31\x31\x2d\x2e\x38\x39\x20\x32\x2d\x32\x20\x32\x2d\x31\
-\x2e\x31\x20\x30\x2d\x32\x2d\x2e\x38\x39\x2d\x32\x2d\x32\x20\x30\
-\x2d\x31\x2e\x31\x2e\x39\x2d\x32\x20\x32\x2d\x32\x7a\x22\x20\x74\
-\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\
-\x61\x74\x65\x28\x31\x29\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\
-\x67\x3e\
-\x00\x00\x01\x08\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x34\x20\x30\x63\
-\x2d\x32\x2e\x32\x31\x20\x30\x2d\x34\x20\x31\x2e\x37\x39\x2d\x34\
-\x20\x34\x73\x31\x2e\x37\x39\x20\x34\x20\x34\x20\x34\x20\x34\x2d\
-\x31\x2e\x37\x39\x20\x34\x2d\x34\x2d\x31\x2e\x37\x39\x2d\x34\x2d\
-\x34\x2d\x34\x7a\x6d\x2d\x31\x2e\x35\x20\x31\x2e\x37\x38\x6c\x31\
-\x2e\x35\x20\x31\x2e\x35\x20\x31\x2e\x35\x2d\x31\x2e\x35\x2e\x37\
-\x32\x2e\x37\x32\x2d\x31\x2e\x35\x20\x31\x2e\x35\x20\x31\x2e\x35\
-\x20\x31\x2e\x35\x2d\x2e\x37\x32\x2e\x37\x32\x2d\x31\x2e\x35\x2d\
-\x31\x2e\x35\x2d\x31\x2e\x35\x20\x31\x2e\x35\x2d\x2e\x37\x32\x2d\
-\x2e\x37\x32\x20\x31\x2e\x35\x2d\x31\x2e\x35\x2d\x31\x2e\x35\x2d\
-\x31\x2e\x35\x2e\x37\x32\x2d\x2e\x37\x32\x7a\x22\x20\x2f\x3e\x0d\
-\x0a\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x00\xd7\
+\x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x61\x79\x81\x31\x3d\
+\x41\x97\xbd\xc9\xcb\xcd\xce\x16\x1b\x1d\x81\xa2\xac\x4b\x5e\x64\
+\xad\xd8\xe6\x0a\x0d\x0e\x40\x51\x56\x6f\x8b\x94\x56\x6c\x73\x20\
+\x28\x2b\x8c\xaf\xba\xa2\xca\xd7\x36\xf6\x87\x6c\x00\x00\x01\x0a\
+\x49\x44\x41\x54\x28\xcf\x65\xd1\xa1\x4e\x03\x41\x10\x80\xe1\x3f\
+\x4d\x1a\x72\x6d\x09\x24\x7d\x00\x2c\x8a\x20\x2b\x10\x84\x20\x96\
+\xd4\x9c\xc4\x81\x44\x12\xde\xa0\x15\xed\x94\x10\xee\x24\x0e\x64\
+\x25\xb2\x92\xa0\x2a\x2b\x71\x20\x8b\x43\x22\x99\xd9\x5e\xc2\xec\
+\xf6\xcc\x6e\xbe\xec\x7f\x97\xdb\xe1\x7c\xfb\x21\x88\xc8\xfb\x91\
+\xf8\xc7\x6c\x44\xb1\xce\x6d\x06\x1f\xb9\xbd\x42\x2f\xb7\x15\xb0\
+\x4e\xed\x51\x29\x89\xd5\xee\xcd\x7a\xa9\xfd\x98\xf9\x58\x6d\x3f\
+\xda\x55\x62\x25\xbc\xc1\x8e\xb7\x09\xec\x4e\xf5\xe0\x8d\xb3\x31\
+\x74\xab\xd2\xc7\x84\x63\x78\x96\x6b\x1f\x13\xf4\x5d\x73\x49\x62\
+\x42\x0d\x03\x49\x62\x86\xd0\xd2\xd5\xc7\x9c\xe9\x27\x74\xf5\x31\
+\xa7\x70\xa9\x6b\xb5\xfa\x8f\xb9\x80\xa5\x6d\xbe\x9a\xb8\xba\x3b\
+\x60\x58\xb7\x7f\x6d\xff\xd0\xc4\x63\xda\x84\x93\xfe\xa6\x68\x62\
+\x3d\x1f\x67\x24\x2e\xbe\xf5\xd6\xc4\xa5\xb7\x4d\xac\x37\xd2\x72\
+\x16\x63\xbd\xf4\xae\xb3\x18\xeb\x5c\xf7\x9c\xc5\x58\xe7\x7a\xe8\
+\xcd\xe2\x17\x58\x78\xb3\xb8\xa6\x10\x6f\x71\xf8\x74\x52\xb3\x7f\
+\xd0\x5b\x4a\xcc\x62\x9e\x52\x8b\xf1\x3c\x33\x8b\x17\x99\x69\x5c\
+\x48\x66\x1a\x77\xb6\xec\x9b\x4f\x91\x3f\x5e\x72\x22\x91\xd1\xe5\
+\x86\x70\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x03\xf6\
+\xef\
+\xbb\xbf\x3c\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\
+\x22\x31\x2e\x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\
+\x75\x74\x66\x2d\x38\x22\x3f\x3e\x0d\x0a\x3c\x21\x44\x4f\x43\x54\
+\x59\x50\x45\x20\x73\x76\x67\x20\x50\x55\x42\x4c\x49\x43\x20\x22\
+\x2d\x2f\x2f\x57\x33\x43\x2f\x2f\x44\x54\x44\x20\x53\x56\x47\x20\
+\x31\x2e\x31\x2f\x2f\x45\x4e\x22\x20\x22\x68\x74\x74\x70\x3a\x2f\
+\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x47\x72\x61\x70\
+\x68\x69\x63\x73\x2f\x53\x56\x47\x2f\x31\x2e\x31\x2f\x44\x54\x44\
+\x2f\x73\x76\x67\x31\x31\x2e\x64\x74\x64\x22\x3e\x0d\x0a\x3c\x73\
+\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\x2f\
+\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\
+\x2f\x73\x76\x67\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x78\x6c\x69\x6e\
+\x6b\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\
+\x2e\x6f\x72\x67\x2f\x31\x39\x39\x39\x2f\x78\x6c\x69\x6e\x6b\x22\
+\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\x31\x22\x20\x62\
+\x61\x73\x65\x50\x72\x6f\x66\x69\x6c\x65\x3d\x22\x66\x75\x6c\x6c\
+\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x30\x22\x20\x68\x65\x69\
+\x67\x68\x74\x3d\x22\x33\x35\x22\x20\x76\x69\x65\x77\x42\x6f\x78\
+\x3d\x22\x30\x20\x30\x20\x34\x30\x2e\x30\x30\x20\x33\x35\x2e\x30\
+\x30\x22\x20\x65\x6e\x61\x62\x6c\x65\x2d\x62\x61\x63\x6b\x67\x72\
+\x6f\x75\x6e\x64\x3d\x22\x6e\x65\x77\x20\x30\x20\x30\x20\x34\x30\
+\x2e\x30\x30\x20\x33\x35\x2e\x30\x30\x22\x20\x78\x6d\x6c\x3a\x73\
+\x70\x61\x63\x65\x3d\x22\x70\x72\x65\x73\x65\x72\x76\x65\x22\x3e\
+\x0d\x0a\x09\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x23\
+\x30\x30\x30\x30\x30\x30\x22\x20\x66\x69\x6c\x6c\x2d\x6f\x70\x61\
+\x63\x69\x74\x79\x3d\x22\x31\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
+\x77\x69\x64\x74\x68\x3d\x22\x30\x2e\x32\x22\x20\x73\x74\x72\x6f\
+\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\
+\x6e\x64\x22\x20\x64\x3d\x22\x4d\x20\x33\x37\x2e\x39\x31\x36\x37\
+\x2c\x31\x35\x2e\x38\x33\x33\x33\x43\x20\x34\x30\x2e\x31\x30\x32\
+\x38\x2c\x31\x35\x2e\x38\x33\x33\x33\x20\x34\x32\x2e\x32\x35\x2c\
+\x31\x37\x2e\x38\x31\x33\x39\x20\x34\x32\x2e\x32\x35\x2c\x32\x30\
+\x4c\x20\x34\x32\x2c\x32\x31\x4c\x20\x35\x34\x2c\x32\x31\x4c\x20\
+\x35\x34\x2c\x35\x37\x4c\x20\x32\x32\x2c\x35\x37\x4c\x20\x32\x32\
+\x2c\x32\x31\x4c\x20\x33\x34\x2c\x32\x31\x4c\x20\x33\x33\x2e\x37\
+\x35\x2c\x32\x30\x43\x20\x33\x33\x2e\x37\x35\x2c\x31\x37\x2e\x38\
+\x31\x33\x39\x20\x33\x35\x2e\x37\x33\x30\x35\x2c\x31\x35\x2e\x38\
+\x33\x33\x33\x20\x33\x37\x2e\x39\x31\x36\x37\x2c\x31\x35\x2e\x38\
+\x33\x33\x33\x20\x5a\x20\x4d\x20\x35\x31\x2c\x32\x34\x4c\x20\x34\
+\x35\x2e\x35\x2c\x32\x34\x4c\x20\x34\x37\x2e\x35\x2c\x32\x38\x4c\
+\x20\x32\x38\x2e\x35\x2c\x32\x38\x4c\x20\x33\x30\x2e\x35\x2c\x32\
+\x34\x4c\x20\x32\x35\x2c\x32\x34\x4c\x20\x32\x35\x2c\x35\x34\x4c\
+\x20\x35\x31\x2c\x35\x34\x4c\x20\x35\x31\x2c\x32\x34\x20\x5a\x20\
+\x4d\x20\x33\x37\x2e\x39\x31\x36\x36\x2c\x31\x38\x2e\x32\x30\x38\
+\x34\x43\x20\x33\x37\x2e\x30\x34\x32\x32\x2c\x31\x38\x2e\x32\x30\
+\x38\x34\x20\x33\x36\x2c\x31\x38\x2e\x38\x37\x35\x36\x20\x33\x36\
+\x2c\x31\x39\x2e\x37\x35\x43\x20\x33\x36\x2c\x32\x30\x2e\x30\x33\
+\x38\x34\x20\x33\x36\x2e\x33\x36\x35\x33\x2c\x32\x30\x2e\x37\x36\
+\x37\x31\x20\x33\x36\x2e\x35\x2c\x32\x31\x4c\x20\x33\x39\x2e\x35\
+\x2c\x32\x31\x43\x20\x33\x39\x2e\x36\x33\x34\x37\x2c\x32\x30\x2e\
+\x37\x36\x37\x31\x20\x34\x30\x2c\x32\x30\x2e\x30\x33\x38\x34\x20\
+\x34\x30\x2c\x31\x39\x2e\x37\x35\x43\x20\x34\x30\x2c\x31\x38\x2e\
+\x38\x37\x35\x36\x20\x33\x38\x2e\x37\x39\x31\x31\x2c\x31\x38\x2e\
+\x32\x30\x38\x34\x20\x33\x37\x2e\x39\x31\x36\x36\x2c\x31\x38\x2e\
+\x32\x30\x38\x34\x20\x5a\x20\x0d\x0a\x4d\x20\x34\x33\x2e\x35\x35\
+\x2c\x34\x30\x4c\x20\x36\x31\x2e\x35\x2c\x34\x30\x4c\x20\x35\x34\
+\x2e\x35\x2c\x33\x35\x4c\x20\x36\x31\x2e\x35\x2c\x33\x35\x4c\x20\
+\x36\x38\x2e\x35\x2c\x34\x32\x4c\x20\x36\x31\x2e\x35\x2c\x34\x39\
+\x4c\x20\x35\x34\x2e\x35\x2c\x34\x39\x4c\x20\x36\x31\x2e\x35\x2c\
+\x34\x34\x4c\x20\x34\x33\x2e\x35\x35\x2c\x34\x34\x4c\x20\x34\x33\
+\x2e\x35\x35\x2c\x34\x30\x20\x5a\x22\x0d\x0a\x74\x72\x61\x6e\x73\
+\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\x61\x74\x65\x28\
+\x2d\x32\x38\x20\x2d\x31\x36\x29\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\
+\x76\x67\x3e\x0d\x0a\
+\x00\x00\x01\x71\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x34\x20\x30\x63\
-\x2d\x32\x2e\x32\x31\x20\x30\x2d\x34\x20\x31\x2e\x37\x39\x2d\x34\
-\x20\x34\x73\x31\x2e\x37\x39\x20\x34\x20\x34\x20\x34\x20\x34\x2d\
-\x31\x2e\x37\x39\x20\x34\x2d\x34\x2d\x31\x2e\x37\x39\x2d\x34\x2d\
-\x34\x2d\x34\x7a\x6d\x32\x20\x31\x2e\x37\x38\x6c\x2e\x37\x32\x2e\
-\x37\x32\x2d\x33\x2e\x32\x32\x20\x33\x2e\x32\x32\x2d\x31\x2e\x37\
-\x32\x2d\x31\x2e\x37\x32\x2e\x37\x32\x2d\x2e\x37\x32\x20\x31\x20\
-\x31\x20\x32\x2e\x35\x2d\x32\x2e\x35\x7a\x22\x20\x2f\x3e\x0d\x0a\
-\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x01\x5d\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
-\x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x62\x7a\x82\xad\xd8\
-\xe6\x23\x2a\x2c\xaf\xb4\xb6\x4e\x4e\x4e\x89\xa3\xac\x0b\x0e\x0f\
-\xcb\xcd\xce\x92\xb7\xc3\x31\x3d\x42\x78\x8b\x91\xc0\xc0\xc0\x54\
-\x69\x70\x14\x19\x1b\x06\x08\x09\x4b\x93\x60\x3b\x00\x00\x00\xe8\
-\x49\x44\x41\x54\x28\xcf\x63\x38\xd1\xd1\x71\xc4\xa5\x03\x19\xf4\
-\x30\x34\x29\x89\x3f\x60\x7f\x3c\x49\x09\x01\x74\x18\x9a\xb4\x0a\
-\x18\x18\x18\xca\x50\xc5\x16\x00\x85\x18\xd8\x93\x90\xc5\x1a\x41\
-\xca\x18\x18\x1e\x21\x8b\xb5\x83\x85\x18\x78\x91\xc5\xce\x41\xc4\
-\x98\x91\xc5\x1c\x20\x62\x0c\x58\xc4\xf8\x26\x21\x89\xf9\x63\x51\
-\xd7\x07\x11\xe2\x42\x16\x6b\x86\x88\xfd\x46\x16\xeb\x84\xb8\xcf\
-\x08\xc5\x1f\xf9\x68\x4e\x01\x89\xa9\x3d\x60\x60\xe0\x37\x42\x15\
-\x53\xd2\x35\x78\xb0\x5a\x09\x4d\x4c\x49\x09\x39\xa4\x60\x62\x4a\
-\x74\x15\xdb\x7b\x71\x12\xba\xd8\x85\x02\x86\xe2\x49\xa8\x62\xca\
-\x1f\x40\x51\x88\x2a\x66\x00\x8e\xc2\x1c\x64\x31\xdd\x0f\xe0\x20\
-\x7a\x83\x2c\xa6\x00\x09\x4a\x1e\x64\xb1\xed\x10\x31\x6e\x64\xb1\
-\x0b\xd0\xa8\xc1\x22\xc6\x8a\x2c\x26\x00\x8d\x7e\x64\xb1\xe9\x10\
-\x31\x36\x64\x31\x65\x88\x58\x0d\xb2\x98\x26\x38\x0a\xf9\xd7\xa0\
-\xf8\x23\x1d\x24\xf6\x19\xd5\x6f\xa0\x28\x64\x5f\xa4\xc3\x70\x06\
-\x05\x6c\x08\xce\x39\x73\x06\x00\x07\x79\x83\xb6\x91\x0b\xff\x56\
-\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x32\x34\
+\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x34\x22\x20\x76\x69\
+\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x32\x34\x20\x32\x34\
+\x22\x3e\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x31\x32\x20\x32\
+\x43\x36\x2e\x34\x38\x20\x32\x20\x32\x20\x36\x2e\x34\x38\x20\x32\
+\x20\x31\x32\x73\x34\x2e\x34\x38\x20\x31\x30\x20\x31\x30\x20\x31\
+\x30\x20\x31\x30\x2d\x34\x2e\x34\x38\x20\x31\x30\x2d\x31\x30\x53\
+\x31\x37\x2e\x35\x32\x20\x32\x20\x31\x32\x20\x32\x7a\x6d\x31\x20\
+\x31\x37\x68\x2d\x32\x76\x2d\x32\x68\x32\x76\x32\x7a\x6d\x32\x2e\
+\x30\x37\x2d\x37\x2e\x37\x35\x6c\x2d\x2e\x39\x2e\x39\x32\x43\x31\
+\x33\x2e\x34\x35\x20\x31\x32\x2e\x39\x20\x31\x33\x20\x31\x33\x2e\
+\x35\x20\x31\x33\x20\x31\x35\x68\x2d\x32\x76\x2d\x2e\x35\x63\x30\
+\x2d\x31\x2e\x31\x2e\x34\x35\x2d\x32\x2e\x31\x20\x31\x2e\x31\x37\
+\x2d\x32\x2e\x38\x33\x6c\x31\x2e\x32\x34\x2d\x31\x2e\x32\x36\x63\
+\x2e\x33\x37\x2d\x2e\x33\x36\x2e\x35\x39\x2d\x2e\x38\x36\x2e\x35\
+\x39\x2d\x31\x2e\x34\x31\x20\x30\x2d\x31\x2e\x31\x2d\x2e\x39\x2d\
+\x32\x2d\x32\x2d\x32\x73\x2d\x32\x20\x2e\x39\x2d\x32\x20\x32\x48\
+\x38\x63\x30\x2d\x32\x2e\x32\x31\x20\x31\x2e\x37\x39\x2d\x34\x20\
+\x34\x2d\x34\x73\x34\x20\x31\x2e\x37\x39\x20\x34\x20\x34\x63\x30\
+\x20\x2e\x38\x38\x2d\x2e\x33\x36\x20\x31\x2e\x36\x38\x2d\x2e\x39\
+\x33\x20\x32\x2e\x32\x35\x7a\x22\x2f\x3e\x3c\x2f\x73\x76\x67\x3e\
+\
 \x00\x00\x00\xf9\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
 \x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
 \x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
@@ -1324,227 +1250,14 @@
 \x30\x2d\x31\x2e\x33\x38\x20\x31\x2e\x31\x32\x2d\x32\x2e\x35\x20\
 \x32\x2e\x35\x2d\x32\x2e\x35\x73\x32\x2e\x35\x20\x31\x2e\x31\x32\
 \x20\x32\x2e\x35\x20\x32\x2e\x35\x63\x30\x2d\x31\x2e\x39\x33\x2d\
 \x31\x2e\x35\x37\x2d\x33\x2e\x35\x2d\x33\x2e\x35\x2d\x33\x2e\x35\
 \x7a\x22\x20\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\
 \x61\x6e\x73\x6c\x61\x74\x65\x28\x30\x20\x31\x29\x22\x20\x2f\x3e\
 \x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x00\x91\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x76\
-\x31\x68\x38\x76\x2d\x31\x68\x2d\x38\x7a\x6d\x34\x20\x32\x6c\x2d\
-\x33\x20\x33\x68\x32\x76\x33\x68\x32\x76\x2d\x33\x68\x32\x6c\x2d\
-\x33\x2d\x33\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
-\
-\x00\x00\x00\xc6\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x76\
-\x34\x6c\x31\x2e\x35\x2d\x31\x2e\x35\x20\x31\x2e\x35\x20\x31\x2e\
-\x35\x20\x31\x2d\x31\x2d\x31\x2e\x35\x2d\x31\x2e\x35\x20\x31\x2e\
-\x35\x2d\x31\x2e\x35\x68\x2d\x34\x7a\x6d\x35\x20\x34\x6c\x2d\x31\
-\x20\x31\x20\x31\x2e\x35\x20\x31\x2e\x35\x2d\x31\x2e\x35\x20\x31\
-\x2e\x35\x68\x34\x76\x2d\x34\x6c\x2d\x31\x2e\x35\x20\x31\x2e\x35\
-\x2d\x31\x2e\x35\x2d\x31\x2e\x35\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\
-\x2f\x73\x76\x67\x3e\
-\x00\x00\x00\xee\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\
-\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\x69\
-\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\x38\
-\x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\
-\x22\x4d\x2d\x38\x33\x38\x2d\x32\x32\x33\x32\x48\x35\x36\x32\x76\
-\x33\x36\x30\x30\x48\x2d\x38\x33\x38\x7a\x22\x20\x66\x69\x6c\x6c\
-\x3d\x22\x6e\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\
-\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x31\x36\x20\x31\x30\x76\x32\
-\x38\x6c\x32\x32\x2d\x31\x34\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\
-\x77\x68\x69\x74\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\
-\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x34\x38\x76\x34\
-\x38\x48\x30\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\
-\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
-\x00\x00\x02\xda\
-\x3c\
-\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\
-\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\x69\
-\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\x38\
-\x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\
-\x22\x4d\x33\x34\x20\x34\x30\x63\x2d\x2e\x35\x37\x20\x30\x2d\x31\
-\x2e\x31\x33\x2d\x2e\x31\x32\x2d\x31\x2e\x35\x33\x2d\x2e\x33\x2d\
-\x31\x2e\x34\x31\x2d\x2e\x37\x35\x2d\x32\x2e\x34\x33\x2d\x31\x2e\
-\x37\x37\x2d\x33\x2e\x34\x32\x2d\x34\x2e\x37\x37\x2d\x31\x2e\x30\
-\x33\x2d\x33\x2e\x31\x31\x2d\x32\x2e\x39\x34\x2d\x34\x2e\x35\x38\
-\x2d\x34\x2e\x37\x39\x2d\x36\x2e\x30\x31\x2d\x31\x2e\x35\x38\x2d\
-\x31\x2e\x32\x32\x2d\x33\x2e\x32\x32\x2d\x32\x2e\x34\x38\x2d\x34\
-\x2e\x36\x33\x2d\x35\x2e\x30\x35\x43\x31\x38\x2e\x35\x38\x20\x32\
-\x31\x2e\x39\x35\x20\x31\x38\x20\x31\x39\x2e\x38\x36\x20\x31\x38\
-\x20\x31\x38\x63\x30\x2d\x35\x2e\x36\x31\x20\x34\x2e\x33\x39\x2d\
-\x31\x30\x20\x31\x30\x2d\x31\x30\x73\x31\x30\x20\x34\x2e\x33\x39\
-\x20\x31\x30\x20\x31\x30\x68\x34\x63\x30\x2d\x37\x2e\x38\x35\x2d\
-\x36\x2e\x31\x35\x2d\x31\x34\x2d\x31\x34\x2d\x31\x34\x73\x2d\x31\
-\x34\x20\x36\x2e\x31\x35\x2d\x31\x34\x20\x31\x34\x63\x30\x20\x32\
-\x2e\x35\x33\x2e\x37\x36\x20\x35\x2e\x33\x20\x32\x2e\x31\x33\x20\
-\x37\x2e\x38\x20\x31\x2e\x38\x32\x20\x33\x2e\x33\x31\x20\x33\x2e\
-\x39\x37\x20\x34\x2e\x39\x36\x20\x35\x2e\x37\x20\x36\x2e\x33\x20\
-\x31\x2e\x36\x32\x20\x31\x2e\x32\x35\x20\x32\x2e\x37\x39\x20\x32\
-\x2e\x31\x35\x20\x33\x2e\x34\x33\x20\x34\x2e\x30\x39\x20\x31\x2e\
-\x32\x20\x33\x2e\x36\x33\x20\x32\x2e\x37\x35\x20\x35\x2e\x36\x38\
-\x20\x35\x2e\x34\x35\x20\x37\x2e\x31\x20\x31\x2e\x30\x34\x2e\x34\
-\x37\x20\x32\x2e\x31\x34\x2e\x37\x31\x20\x33\x2e\x32\x39\x2e\x37\
-\x31\x20\x34\x2e\x34\x31\x20\x30\x20\x38\x2d\x33\x2e\x35\x39\x20\
-\x38\x2d\x38\x68\x2d\x34\x63\x30\x20\x32\x2e\x32\x31\x2d\x31\x2e\
-\x37\x39\x20\x34\x2d\x34\x20\x34\x7a\x4d\x31\x35\x2e\x32\x37\x20\
-\x35\x2e\x32\x37\x6c\x2d\x32\x2e\x38\x33\x2d\x32\x2e\x38\x33\x43\
-\x38\x2e\x34\x36\x20\x36\x2e\x34\x32\x20\x36\x20\x31\x31\x2e\x39\
-\x32\x20\x36\x20\x31\x38\x73\x32\x2e\x34\x36\x20\x31\x31\x2e\x35\
-\x38\x20\x36\x2e\x34\x34\x20\x31\x35\x2e\x35\x36\x6c\x32\x2e\x38\
-\x33\x2d\x32\x2e\x38\x33\x43\x31\x32\x2e\x30\x31\x20\x32\x37\x2e\
-\x34\x37\x20\x31\x30\x20\x32\x32\x2e\x39\x37\x20\x31\x30\x20\x31\
-\x38\x73\x32\x2e\x30\x31\x2d\x39\x2e\x34\x37\x20\x35\x2e\x32\x37\
-\x2d\x31\x32\x2e\x37\x33\x7a\x4d\x32\x33\x20\x31\x38\x63\x30\x20\
-\x32\x2e\x37\x36\x20\x32\x2e\x32\x34\x20\x35\x20\x35\x20\x35\x73\
-\x35\x2d\x32\x2e\x32\x34\x20\x35\x2d\x35\x2d\x32\x2e\x32\x34\x2d\
-\x35\x2d\x35\x2d\x35\x2d\x35\x20\x32\x2e\x32\x34\x2d\x35\x20\x35\
-\x7a\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\
-\x64\x3d\x22\x4d\x30\x20\x30\x68\x34\x38\x76\x34\x38\x48\x30\x7a\
-\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x2f\x3e\x0d\
-\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
-\x00\x00\x07\x66\
-\x3c\
-\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
-\x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\x55\x54\x46\
-\x2d\x38\x22\x20\x73\x74\x61\x6e\x64\x61\x6c\x6f\x6e\x65\x3d\x22\
-\x6e\x6f\x22\x3f\x3e\x0d\x0a\x3c\x73\x76\x67\x0d\x0a\x20\x20\x20\
-\x78\x6d\x6c\x6e\x73\x3a\x64\x63\x3d\x22\x68\x74\x74\x70\x3a\x2f\
-\x2f\x70\x75\x72\x6c\x2e\x6f\x72\x67\x2f\x64\x63\x2f\x65\x6c\x65\
-\x6d\x65\x6e\x74\x73\x2f\x31\x2e\x31\x2f\x22\x0d\x0a\x20\x20\x20\
-\x78\x6d\x6c\x6e\x73\x3a\x63\x63\x3d\x22\x68\x74\x74\x70\x3a\x2f\
-\x2f\x63\x72\x65\x61\x74\x69\x76\x65\x63\x6f\x6d\x6d\x6f\x6e\x73\
-\x2e\x6f\x72\x67\x2f\x6e\x73\x23\x22\x0d\x0a\x20\x20\x20\x78\x6d\
-\x6c\x6e\x73\x3a\x72\x64\x66\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\
-\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x31\x39\x39\x39\x2f\
-\x30\x32\x2f\x32\x32\x2d\x72\x64\x66\x2d\x73\x79\x6e\x74\x61\x78\
-\x2d\x6e\x73\x23\x22\x0d\x0a\x20\x20\x20\x78\x6d\x6c\x6e\x73\x3a\
-\x73\x76\x67\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\
-\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\
-\x0d\x0a\x20\x20\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\
-\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\
-\x30\x30\x2f\x73\x76\x67\x22\x0d\x0a\x20\x20\x20\x78\x6d\x6c\x6e\
-\x73\x3a\x73\x6f\x64\x69\x70\x6f\x64\x69\x3d\x22\x68\x74\x74\x70\
-\x3a\x2f\x2f\x73\x6f\x64\x69\x70\x6f\x64\x69\x2e\x73\x6f\x75\x72\
-\x63\x65\x66\x6f\x72\x67\x65\x2e\x6e\x65\x74\x2f\x44\x54\x44\x2f\
-\x73\x6f\x64\x69\x70\x6f\x64\x69\x2d\x30\x2e\x64\x74\x64\x22\x0d\
-\x0a\x20\x20\x20\x78\x6d\x6c\x6e\x73\x3a\x69\x6e\x6b\x73\x63\x61\
-\x70\x65\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x69\
-\x6e\x6b\x73\x63\x61\x70\x65\x2e\x6f\x72\x67\x2f\x6e\x61\x6d\x65\
-\x73\x70\x61\x63\x65\x73\x2f\x69\x6e\x6b\x73\x63\x61\x70\x65\x22\
-\x0d\x0a\x20\x20\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\x22\x0d\
-\x0a\x20\x20\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x0d\
-\x0a\x20\x20\x20\x76\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\
-\x20\x34\x38\x20\x34\x38\x22\x0d\x0a\x20\x20\x20\x76\x65\x72\x73\
-\x69\x6f\x6e\x3d\x22\x31\x2e\x31\x22\x0d\x0a\x20\x20\x20\x69\x64\
-\x3d\x22\x73\x76\x67\x36\x22\x0d\x0a\x20\x20\x20\x73\x6f\x64\x69\
-\x70\x6f\x64\x69\x3a\x64\x6f\x63\x6e\x61\x6d\x65\x3d\x22\x69\x63\
-\x5f\x76\x6f\x6c\x75\x6d\x65\x5f\x75\x70\x5f\x34\x38\x70\x78\x5f\
-\x39\x30\x2e\x73\x76\x67\x22\x0d\x0a\x20\x20\x20\x69\x6e\x6b\x73\
-\x63\x61\x70\x65\x3a\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
-\x30\x2e\x31\x20\x28\x33\x62\x63\x32\x65\x38\x31\x33\x66\x35\x2c\
-\x20\x32\x30\x32\x30\x2d\x30\x39\x2d\x30\x37\x29\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x6d\x65\x74\x61\x64\x61\x74\x61\x0d\x0a\x20\x20\x20\
-\x20\x20\x69\x64\x3d\x22\x6d\x65\x74\x61\x64\x61\x74\x61\x31\x32\
-\x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x72\x64\x66\x3a\x52\x44\x46\
-\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x63\x63\x3a\x57\x6f\x72\
-\x6b\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x20\x72\x64\x66\x3a\
-\x61\x62\x6f\x75\x74\x3d\x22\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x20\x3c\x64\x63\x3a\x66\x6f\x72\x6d\x61\x74\x3e\x69\x6d\
-\x61\x67\x65\x2f\x73\x76\x67\x2b\x78\x6d\x6c\x3c\x2f\x64\x63\x3a\
-\x66\x6f\x72\x6d\x61\x74\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\
-\x20\x3c\x64\x63\x3a\x74\x79\x70\x65\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x20\x20\x20\x20\x72\x64\x66\x3a\x72\x65\x73\x6f\x75\x72\
-\x63\x65\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x70\x75\x72\x6c\x2e\
-\x6f\x72\x67\x2f\x64\x63\x2f\x64\x63\x6d\x69\x74\x79\x70\x65\x2f\
-\x53\x74\x69\x6c\x6c\x49\x6d\x61\x67\x65\x22\x20\x2f\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x64\x63\x3a\x74\x69\x74\x6c\
-\x65\x3e\x3c\x2f\x64\x63\x3a\x74\x69\x74\x6c\x65\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x20\x3c\x2f\x63\x63\x3a\x57\x6f\x72\x6b\x3e\x0d\
-\x0a\x20\x20\x20\x20\x3c\x2f\x72\x64\x66\x3a\x52\x44\x46\x3e\x0d\
-\x0a\x20\x20\x3c\x2f\x6d\x65\x74\x61\x64\x61\x74\x61\x3e\x0d\x0a\
-\x20\x20\x3c\x64\x65\x66\x73\x0d\x0a\x20\x20\x20\x20\x20\x69\x64\
-\x3d\x22\x64\x65\x66\x73\x31\x30\x22\x20\x2f\x3e\x0d\x0a\x20\x20\
-\x3c\x73\x6f\x64\x69\x70\x6f\x64\x69\x3a\x6e\x61\x6d\x65\x64\x76\
-\x69\x65\x77\x0d\x0a\x20\x20\x20\x20\x20\x70\x61\x67\x65\x63\x6f\
-\x6c\x6f\x72\x3d\x22\x23\x66\x66\x66\x66\x66\x66\x22\x0d\x0a\x20\
-\x20\x20\x20\x20\x62\x6f\x72\x64\x65\x72\x63\x6f\x6c\x6f\x72\x3d\
-\x22\x23\x36\x36\x36\x36\x36\x36\x22\x0d\x0a\x20\x20\x20\x20\x20\
-\x62\x6f\x72\x64\x65\x72\x6f\x70\x61\x63\x69\x74\x79\x3d\x22\x31\
-\x22\x0d\x0a\x20\x20\x20\x20\x20\x6f\x62\x6a\x65\x63\x74\x74\x6f\
-\x6c\x65\x72\x61\x6e\x63\x65\x3d\x22\x31\x30\x22\x0d\x0a\x20\x20\
-\x20\x20\x20\x67\x72\x69\x64\x74\x6f\x6c\x65\x72\x61\x6e\x63\x65\
-\x3d\x22\x31\x30\x22\x0d\x0a\x20\x20\x20\x20\x20\x67\x75\x69\x64\
-\x65\x74\x6f\x6c\x65\x72\x61\x6e\x63\x65\x3d\x22\x31\x30\x22\x0d\
-\x0a\x20\x20\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x70\
-\x61\x67\x65\x6f\x70\x61\x63\x69\x74\x79\x3d\x22\x30\x22\x0d\x0a\
-\x20\x20\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x70\x61\
-\x67\x65\x73\x68\x61\x64\x6f\x77\x3d\x22\x32\x22\x0d\x0a\x20\x20\
-\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x77\x69\x6e\x64\
-\x6f\x77\x2d\x77\x69\x64\x74\x68\x3d\x22\x31\x39\x31\x31\x22\x0d\
-\x0a\x20\x20\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x77\
-\x69\x6e\x64\x6f\x77\x2d\x68\x65\x69\x67\x68\x74\x3d\x22\x31\x30\
-\x34\x30\x22\x0d\x0a\x20\x20\x20\x20\x20\x69\x64\x3d\x22\x6e\x61\
-\x6d\x65\x64\x76\x69\x65\x77\x38\x22\x0d\x0a\x20\x20\x20\x20\x20\
-\x73\x68\x6f\x77\x67\x72\x69\x64\x3d\x22\x66\x61\x6c\x73\x65\x22\
-\x0d\x0a\x20\x20\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\
-\x7a\x6f\x6f\x6d\x3d\x22\x31\x37\x2e\x31\x32\x35\x22\x0d\x0a\x20\
-\x20\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x63\x78\x3d\
-\x22\x32\x34\x22\x0d\x0a\x20\x20\x20\x20\x20\x69\x6e\x6b\x73\x63\
-\x61\x70\x65\x3a\x63\x79\x3d\x22\x32\x34\x22\x0d\x0a\x20\x20\x20\
-\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x77\x69\x6e\x64\x6f\
-\x77\x2d\x78\x3d\x22\x30\x22\x0d\x0a\x20\x20\x20\x20\x20\x69\x6e\
-\x6b\x73\x63\x61\x70\x65\x3a\x77\x69\x6e\x64\x6f\x77\x2d\x79\x3d\
-\x22\x30\x22\x0d\x0a\x20\x20\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\
-\x70\x65\x3a\x77\x69\x6e\x64\x6f\x77\x2d\x6d\x61\x78\x69\x6d\x69\
-\x7a\x65\x64\x3d\x22\x30\x22\x0d\x0a\x20\x20\x20\x20\x20\x69\x6e\
-\x6b\x73\x63\x61\x70\x65\x3a\x63\x75\x72\x72\x65\x6e\x74\x2d\x6c\
-\x61\x79\x65\x72\x3d\x22\x73\x76\x67\x36\x22\x20\x2f\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x0d\x0a\x20\x20\x20\x20\x20\x64\x3d\
-\x22\x4d\x20\x33\x30\x2c\x36\x20\x48\x20\x31\x38\x20\x76\x20\x38\
-\x20\x4c\x20\x38\x2c\x32\x34\x20\x48\x20\x34\x30\x20\x4c\x20\x33\
-\x30\x2c\x31\x34\x20\x5a\x20\x6d\x20\x2d\x36\x2c\x32\x37\x20\x63\
-\x20\x33\x2e\x35\x33\x2c\x30\x20\x36\x2e\x35\x38\x2c\x2d\x32\x2e\
-\x30\x34\x20\x38\x2e\x30\x35\x2c\x2d\x35\x20\x48\x20\x31\x35\x2e\
-\x39\x34\x20\x63\x20\x31\x2e\x34\x38\x2c\x32\x2e\x39\x36\x20\x34\
-\x2e\x35\x33\x2c\x35\x20\x38\x2e\x30\x36\x2c\x35\x20\x7a\x20\x4d\
-\x20\x34\x31\x2e\x35\x34\x2c\x32\x38\x20\x48\x20\x33\x37\x2e\x34\
-\x31\x20\x43\x20\x33\x35\x2e\x36\x39\x2c\x33\x33\x2e\x37\x38\x20\
-\x33\x30\x2e\x33\x34\x2c\x33\x38\x20\x32\x34\x2c\x33\x38\x20\x31\
-\x37\x2e\x36\x36\x2c\x33\x38\x20\x31\x32\x2e\x33\x31\x2c\x33\x33\
-\x2e\x37\x38\x20\x31\x30\x2e\x35\x39\x2c\x32\x38\x20\x48\x20\x36\
-\x2e\x34\x36\x20\x63\x20\x31\x2e\x38\x32\x2c\x38\x2e\x30\x31\x20\
-\x38\x2e\x39\x37\x2c\x31\x34\x20\x31\x37\x2e\x35\x34\x2c\x31\x34\
-\x20\x38\x2e\x35\x37\x2c\x30\x20\x31\x35\x2e\x37\x32\x2c\x2d\x35\
-\x2e\x39\x39\x20\x31\x37\x2e\x35\x34\x2c\x2d\x31\x34\x20\x7a\x22\
-\x0d\x0a\x20\x20\x20\x20\x20\x69\x64\x3d\x22\x70\x61\x74\x68\x32\
-\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x3c\x70\x61\x74\x68\x0d\x0a\x20\
-\x20\x20\x20\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x34\x38\x76\x34\
-\x38\x48\x30\x7a\x22\x0d\x0a\x20\x20\x20\x20\x20\x66\x69\x6c\x6c\
-\x3d\x22\x6e\x6f\x6e\x65\x22\x0d\x0a\x20\x20\x20\x20\x20\x69\x64\
-\x3d\x22\x70\x61\x74\x68\x34\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\
-\x76\x67\x3e\x0d\x0a\
 \x00\x00\x01\xad\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
 \x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
 \x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
@@ -1566,725 +1279,126 @@
 \x39\x2d\x2e\x35\x35\x20\x31\x2e\x38\x35\x2d\x31\x2e\x33\x34\x20\
 \x32\x2e\x33\x31\x2e\x33\x39\x2e\x32\x32\x2e\x38\x36\x2e\x33\x34\
 \x20\x31\x2e\x33\x34\x2e\x33\x34\x20\x31\x2e\x34\x37\x20\x30\x20\
 \x32\x2e\x36\x36\x2d\x31\x2e\x31\x38\x20\x32\x2e\x36\x36\x2d\x32\
 \x2e\x36\x36\x20\x30\x2d\x2e\x37\x34\x2d\x2e\x36\x31\x2d\x31\x2e\
 \x33\x34\x2d\x31\x2e\x33\x34\x2d\x31\x2e\x33\x34\x7a\x22\x0d\x0a\
 \x20\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x00\x91\
+\x00\x00\x01\xc7\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x34\x20\x30\x6c\
-\x2d\x34\x20\x33\x68\x31\x76\x34\x68\x32\x76\x2d\x32\x68\x32\x76\
-\x32\x68\x32\x76\x2d\x34\x2e\x30\x33\x6c\x31\x20\x2e\x30\x33\x2d\
-\x34\x2d\x33\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
-\
-\x00\x00\x1c\x00\
-\x3c\
-\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
-\x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\x55\x54\x46\
-\x2d\x38\x22\x20\x73\x74\x61\x6e\x64\x61\x6c\x6f\x6e\x65\x3d\x22\
-\x6e\x6f\x22\x3f\x3e\x0d\x0a\x3c\x73\x76\x67\x0d\x0a\x20\x20\x20\
-\x78\x6d\x6c\x6e\x73\x3a\x6f\x6f\x6f\x3d\x22\x68\x74\x74\x70\x3a\
-\x2f\x2f\x78\x6d\x6c\x2e\x6f\x70\x65\x6e\x6f\x66\x66\x69\x63\x65\
-\x2e\x6f\x72\x67\x2f\x73\x76\x67\x2f\x65\x78\x70\x6f\x72\x74\x22\
-\x0d\x0a\x20\x20\x20\x78\x6d\x6c\x6e\x73\x3a\x64\x63\x3d\x22\x68\
-\x74\x74\x70\x3a\x2f\x2f\x70\x75\x72\x6c\x2e\x6f\x72\x67\x2f\x64\
-\x63\x2f\x65\x6c\x65\x6d\x65\x6e\x74\x73\x2f\x31\x2e\x31\x2f\x22\
-\x0d\x0a\x20\x20\x20\x78\x6d\x6c\x6e\x73\x3a\x63\x63\x3d\x22\x68\
-\x74\x74\x70\x3a\x2f\x2f\x63\x72\x65\x61\x74\x69\x76\x65\x63\x6f\
-\x6d\x6d\x6f\x6e\x73\x2e\x6f\x72\x67\x2f\x6e\x73\x23\x22\x0d\x0a\
-\x20\x20\x20\x78\x6d\x6c\x6e\x73\x3a\x72\x64\x66\x3d\x22\x68\x74\
-\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\
-\x31\x39\x39\x39\x2f\x30\x32\x2f\x32\x32\x2d\x72\x64\x66\x2d\x73\
-\x79\x6e\x74\x61\x78\x2d\x6e\x73\x23\x22\x0d\x0a\x20\x20\x20\x78\
-\x6d\x6c\x6e\x73\x3a\x73\x76\x67\x3d\x22\x68\x74\x74\x70\x3a\x2f\
-\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\
-\x2f\x73\x76\x67\x22\x0d\x0a\x20\x20\x20\x78\x6d\x6c\x6e\x73\x3d\
-\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\
-\x72\x67\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\x0d\x0a\x20\x20\
-\x20\x78\x6d\x6c\x6e\x73\x3a\x73\x6f\x64\x69\x70\x6f\x64\x69\x3d\
-\x22\x68\x74\x74\x70\x3a\x2f\x2f\x73\x6f\x64\x69\x70\x6f\x64\x69\
-\x2e\x73\x6f\x75\x72\x63\x65\x66\x6f\x72\x67\x65\x2e\x6e\x65\x74\
-\x2f\x44\x54\x44\x2f\x73\x6f\x64\x69\x70\x6f\x64\x69\x2d\x30\x2e\
-\x64\x74\x64\x22\x0d\x0a\x20\x20\x20\x78\x6d\x6c\x6e\x73\x3a\x69\
-\x6e\x6b\x73\x63\x61\x70\x65\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\
-\x77\x77\x77\x2e\x69\x6e\x6b\x73\x63\x61\x70\x65\x2e\x6f\x72\x67\
-\x2f\x6e\x61\x6d\x65\x73\x70\x61\x63\x65\x73\x2f\x69\x6e\x6b\x73\
-\x63\x61\x70\x65\x22\x0d\x0a\x20\x20\x20\x76\x65\x72\x73\x69\x6f\
-\x6e\x3d\x22\x31\x2e\x32\x22\x0d\x0a\x20\x20\x20\x77\x69\x64\x74\
-\x68\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\x0d\x0a\x20\x20\x20\x68\
-\x65\x69\x67\x68\x74\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\x0d\x0a\
-\x20\x20\x20\x76\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\
-\x38\x34\x37\x20\x38\x34\x37\x22\x0d\x0a\x20\x20\x20\x70\x72\x65\
-\x73\x65\x72\x76\x65\x41\x73\x70\x65\x63\x74\x52\x61\x74\x69\x6f\
-\x3d\x22\x78\x4d\x69\x64\x59\x4d\x69\x64\x22\x0d\x0a\x20\x20\x20\
-\x66\x69\x6c\x6c\x2d\x72\x75\x6c\x65\x3d\x22\x65\x76\x65\x6e\x6f\
-\x64\x64\x22\x0d\x0a\x20\x20\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\
-\x69\x64\x74\x68\x3d\x22\x32\x38\x2e\x32\x32\x32\x22\x0d\x0a\x20\
-\x20\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\
-\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x0d\x0a\x20\x20\x20\x78\x6d\
-\x6c\x3a\x73\x70\x61\x63\x65\x3d\x22\x70\x72\x65\x73\x65\x72\x76\
-\x65\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x73\x76\x67\x39\x34\
-\x22\x0d\x0a\x20\x20\x20\x73\x6f\x64\x69\x70\x6f\x64\x69\x3a\x64\
-\x6f\x63\x6e\x61\x6d\x65\x3d\x22\x66\x66\x74\x5f\x32\x2e\x73\x76\
-\x67\x22\x0d\x0a\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\
-\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\x30\x2e\x31\x20\x28\
-\x33\x62\x63\x32\x65\x38\x31\x33\x66\x35\x2c\x20\x32\x30\x32\x30\
-\x2d\x30\x39\x2d\x30\x37\x29\x22\x3e\x3c\x6d\x65\x74\x61\x64\x61\
-\x74\x61\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x6d\x65\x74\x61\x64\
-\x61\x74\x61\x39\x38\x22\x3e\x3c\x72\x64\x66\x3a\x52\x44\x46\x3e\
-\x3c\x63\x63\x3a\x57\x6f\x72\x6b\x0d\x0a\x20\x20\x20\x20\x20\x20\
-\x20\x72\x64\x66\x3a\x61\x62\x6f\x75\x74\x3d\x22\x22\x3e\x3c\x64\
-\x63\x3a\x66\x6f\x72\x6d\x61\x74\x3e\x69\x6d\x61\x67\x65\x2f\x73\
-\x76\x67\x2b\x78\x6d\x6c\x3c\x2f\x64\x63\x3a\x66\x6f\x72\x6d\x61\
-\x74\x3e\x3c\x64\x63\x3a\x74\x79\x70\x65\x0d\x0a\x20\x20\x20\x20\
-\x20\x20\x20\x20\x20\x72\x64\x66\x3a\x72\x65\x73\x6f\x75\x72\x63\
-\x65\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x70\x75\x72\x6c\x2e\x6f\
-\x72\x67\x2f\x64\x63\x2f\x64\x63\x6d\x69\x74\x79\x70\x65\x2f\x53\
-\x74\x69\x6c\x6c\x49\x6d\x61\x67\x65\x22\x20\x2f\x3e\x3c\x64\x63\
-\x3a\x74\x69\x74\x6c\x65\x20\x2f\x3e\x3c\x2f\x63\x63\x3a\x57\x6f\
-\x72\x6b\x3e\x3c\x2f\x72\x64\x66\x3a\x52\x44\x46\x3e\x3c\x2f\x6d\
-\x65\x74\x61\x64\x61\x74\x61\x3e\x3c\x73\x6f\x64\x69\x70\x6f\x64\
-\x69\x3a\x6e\x61\x6d\x65\x64\x76\x69\x65\x77\x0d\x0a\x20\x20\x20\
-\x70\x61\x67\x65\x63\x6f\x6c\x6f\x72\x3d\x22\x23\x66\x66\x66\x66\
-\x66\x66\x22\x0d\x0a\x20\x20\x20\x62\x6f\x72\x64\x65\x72\x63\x6f\
-\x6c\x6f\x72\x3d\x22\x23\x36\x36\x36\x36\x36\x36\x22\x0d\x0a\x20\
-\x20\x20\x62\x6f\x72\x64\x65\x72\x6f\x70\x61\x63\x69\x74\x79\x3d\
-\x22\x31\x22\x0d\x0a\x20\x20\x20\x6f\x62\x6a\x65\x63\x74\x74\x6f\
-\x6c\x65\x72\x61\x6e\x63\x65\x3d\x22\x31\x30\x22\x0d\x0a\x20\x20\
-\x20\x67\x72\x69\x64\x74\x6f\x6c\x65\x72\x61\x6e\x63\x65\x3d\x22\
-\x31\x30\x22\x0d\x0a\x20\x20\x20\x67\x75\x69\x64\x65\x74\x6f\x6c\
-\x65\x72\x61\x6e\x63\x65\x3d\x22\x31\x30\x22\x0d\x0a\x20\x20\x20\
-\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x70\x61\x67\x65\x6f\x70\x61\
-\x63\x69\x74\x79\x3d\x22\x30\x22\x0d\x0a\x20\x20\x20\x69\x6e\x6b\
-\x73\x63\x61\x70\x65\x3a\x70\x61\x67\x65\x73\x68\x61\x64\x6f\x77\
-\x3d\x22\x32\x22\x0d\x0a\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\
-\x65\x3a\x77\x69\x6e\x64\x6f\x77\x2d\x77\x69\x64\x74\x68\x3d\x22\
-\x31\x39\x31\x38\x22\x0d\x0a\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\
-\x70\x65\x3a\x77\x69\x6e\x64\x6f\x77\x2d\x68\x65\x69\x67\x68\x74\
-\x3d\x22\x39\x39\x31\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x6e\
-\x61\x6d\x65\x64\x76\x69\x65\x77\x39\x36\x22\x0d\x0a\x20\x20\x20\
-\x73\x68\x6f\x77\x67\x72\x69\x64\x3d\x22\x66\x61\x6c\x73\x65\x22\
-\x0d\x0a\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x7a\x6f\
-\x6f\x6d\x3d\x22\x32\x35\x2e\x36\x37\x37\x33\x39\x22\x0d\x0a\x20\
-\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x63\x78\x3d\x22\x34\
-\x2e\x37\x33\x31\x37\x38\x39\x36\x22\x0d\x0a\x20\x20\x20\x69\x6e\
-\x6b\x73\x63\x61\x70\x65\x3a\x63\x79\x3d\x22\x31\x34\x2e\x34\x34\
-\x38\x35\x30\x39\x22\x0d\x0a\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\
-\x70\x65\x3a\x77\x69\x6e\x64\x6f\x77\x2d\x78\x3d\x22\x30\x22\x0d\
-\x0a\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x77\x69\x6e\
-\x64\x6f\x77\x2d\x79\x3d\x22\x30\x22\x0d\x0a\x20\x20\x20\x69\x6e\
-\x6b\x73\x63\x61\x70\x65\x3a\x77\x69\x6e\x64\x6f\x77\x2d\x6d\x61\
-\x78\x69\x6d\x69\x7a\x65\x64\x3d\x22\x30\x22\x0d\x0a\x20\x20\x20\
-\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x63\x75\x72\x72\x65\x6e\x74\
-\x2d\x6c\x61\x79\x65\x72\x3d\x22\x73\x76\x67\x39\x34\x22\x0d\x0a\
-\x20\x20\x20\x69\x6e\x6b\x73\x63\x61\x70\x65\x3a\x64\x6f\x63\x75\
-\x6d\x65\x6e\x74\x2d\x72\x6f\x74\x61\x74\x69\x6f\x6e\x3d\x22\x30\
-\x22\x20\x2f\x3e\x0d\x0a\x20\x3c\x64\x65\x66\x73\x0d\x0a\x20\x20\
-\x20\x63\x6c\x61\x73\x73\x3d\x22\x43\x6c\x69\x70\x50\x61\x74\x68\
-\x47\x72\x6f\x75\x70\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x64\
-\x65\x66\x73\x38\x22\x3e\x0d\x0a\x20\x20\x3c\x63\x6c\x69\x70\x50\
-\x61\x74\x68\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x70\x72\x65\x73\
-\x65\x6e\x74\x61\x74\x69\x6f\x6e\x5f\x63\x6c\x69\x70\x5f\x70\x61\
-\x74\x68\x22\x0d\x0a\x20\x20\x20\x63\x6c\x69\x70\x50\x61\x74\x68\
-\x55\x6e\x69\x74\x73\x3d\x22\x75\x73\x65\x72\x53\x70\x61\x63\x65\
-\x4f\x6e\x55\x73\x65\x22\x3e\x0d\x0a\x20\x20\x20\x3c\x72\x65\x63\
-\x74\x0d\x0a\x20\x20\x20\x78\x3d\x22\x30\x22\x0d\x0a\x20\x20\x20\
-\x79\x3d\x22\x30\x22\x0d\x0a\x20\x20\x20\x77\x69\x64\x74\x68\x3d\
-\x22\x38\x34\x37\x22\x0d\x0a\x20\x20\x20\x68\x65\x69\x67\x68\x74\
-\x3d\x22\x38\x34\x37\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x72\
-\x65\x63\x74\x32\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x3c\x2f\x63\x6c\
-\x69\x70\x50\x61\x74\x68\x3e\x0d\x0a\x20\x20\x3c\x63\x6c\x69\x70\
-\x50\x61\x74\x68\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x70\x72\x65\
-\x73\x65\x6e\x74\x61\x74\x69\x6f\x6e\x5f\x63\x6c\x69\x70\x5f\x70\
-\x61\x74\x68\x5f\x73\x68\x72\x69\x6e\x6b\x22\x0d\x0a\x20\x20\x20\
-\x63\x6c\x69\x70\x50\x61\x74\x68\x55\x6e\x69\x74\x73\x3d\x22\x75\
-\x73\x65\x72\x53\x70\x61\x63\x65\x4f\x6e\x55\x73\x65\x22\x3e\x0d\
-\x0a\x20\x20\x20\x3c\x72\x65\x63\x74\x0d\x0a\x20\x20\x20\x78\x3d\
-\x22\x30\x22\x0d\x0a\x20\x20\x20\x79\x3d\x22\x30\x22\x0d\x0a\x20\
-\x20\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x34\x36\x22\x0d\x0a\x20\
-\x20\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x34\x36\x22\x0d\x0a\
-\x20\x20\x20\x69\x64\x3d\x22\x72\x65\x63\x74\x35\x22\x20\x2f\x3e\
-\x0d\x0a\x20\x20\x3c\x2f\x63\x6c\x69\x70\x50\x61\x74\x68\x3e\x0d\
-\x0a\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x0d\x0a\x20\x20\x20\x0d\x0a\
-\x20\x20\x0d\x0a\x20\x20\x20\x20\x0d\x0a\x20\x20\x20\x0d\x0a\x20\
-\x20\x20\x20\x20\x0d\x0a\x20\x20\x20\x20\x0d\x0a\x20\x20\x20\x20\
-\x20\x20\x0d\x0a\x20\x20\x20\x20\x20\x20\x0d\x0a\x20\x20\x20\x20\
-\x20\x20\x0d\x0a\x20\x20\x20\x20\x20\x3c\x2f\x64\x65\x66\x73\x3e\
-\x0d\x0a\x20\x3c\x64\x65\x66\x73\x0d\x0a\x20\x20\x20\x63\x6c\x61\
-\x73\x73\x3d\x22\x54\x65\x78\x74\x53\x68\x61\x70\x65\x49\x6e\x64\
-\x65\x78\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x64\x65\x66\x73\
-\x31\x32\x22\x3e\x0d\x0a\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x6f\
-\x6f\x6f\x3a\x73\x6c\x69\x64\x65\x3d\x22\x69\x64\x31\x22\x0d\x0a\
-\x20\x20\x20\x6f\x6f\x6f\x3a\x69\x64\x2d\x6c\x69\x73\x74\x3d\x22\
-\x69\x64\x33\x20\x69\x64\x34\x20\x69\x64\x35\x20\x69\x64\x36\x20\
-\x69\x64\x37\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x67\x31\x30\
-\x22\x20\x2f\x3e\x0d\x0a\x20\x3c\x2f\x64\x65\x66\x73\x3e\x0d\x0a\
-\x20\x3c\x64\x65\x66\x73\x0d\x0a\x20\x20\x20\x63\x6c\x61\x73\x73\
-\x3d\x22\x45\x6d\x62\x65\x64\x64\x65\x64\x42\x75\x6c\x6c\x65\x74\
-\x43\x68\x61\x72\x73\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x64\
-\x65\x66\x73\x34\x34\x22\x3e\x0d\x0a\x20\x20\x3c\x67\x0d\x0a\x20\
-\x20\x20\x69\x64\x3d\x22\x62\x75\x6c\x6c\x65\x74\x2d\x63\x68\x61\
-\x72\x2d\x74\x65\x6d\x70\x6c\x61\x74\x65\x2d\x35\x37\x33\x35\x36\
-\x22\x0d\x0a\x20\x20\x20\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\
-\x22\x73\x63\x61\x6c\x65\x28\x30\x2e\x30\x30\x30\x34\x38\x38\x32\
-\x38\x31\x32\x35\x2c\x2d\x30\x2e\x30\x30\x30\x34\x38\x38\x32\x38\
-\x31\x32\x35\x29\x22\x3e\x0d\x0a\x20\x20\x20\x3c\x70\x61\x74\x68\
-\x0d\x0a\x20\x20\x20\x64\x3d\x22\x4d\x20\x35\x38\x30\x2c\x31\x31\
-\x34\x31\x20\x4c\x20\x31\x31\x36\x33\x2c\x35\x37\x31\x20\x35\x38\
-\x30\x2c\x30\x20\x2d\x34\x2c\x35\x37\x31\x20\x35\x38\x30\x2c\x31\
-\x31\x34\x31\x20\x5a\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x70\
-\x61\x74\x68\x31\x34\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x3c\x2f\x67\
-\x3e\x0d\x0a\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\
-\x62\x75\x6c\x6c\x65\x74\x2d\x63\x68\x61\x72\x2d\x74\x65\x6d\x70\
-\x6c\x61\x74\x65\x2d\x35\x37\x33\x35\x34\x22\x0d\x0a\x20\x20\x20\
-\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x73\x63\x61\x6c\x65\
-\x28\x30\x2e\x30\x30\x30\x34\x38\x38\x32\x38\x31\x32\x35\x2c\x2d\
-\x30\x2e\x30\x30\x30\x34\x38\x38\x32\x38\x31\x32\x35\x29\x22\x3e\
-\x0d\x0a\x20\x20\x20\x3c\x70\x61\x74\x68\x0d\x0a\x20\x20\x20\x64\
-\x3d\x22\x4d\x20\x38\x2c\x31\x31\x32\x38\x20\x4c\x20\x31\x31\x33\
-\x37\x2c\x31\x31\x32\x38\x20\x31\x31\x33\x37\x2c\x30\x20\x38\x2c\
-\x30\x20\x38\x2c\x31\x31\x32\x38\x20\x5a\x22\x0d\x0a\x20\x20\x20\
-\x69\x64\x3d\x22\x70\x61\x74\x68\x31\x37\x22\x20\x2f\x3e\x0d\x0a\
-\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x3c\x67\x0d\x0a\x20\x20\
-\x20\x69\x64\x3d\x22\x62\x75\x6c\x6c\x65\x74\x2d\x63\x68\x61\x72\
-\x2d\x74\x65\x6d\x70\x6c\x61\x74\x65\x2d\x31\x30\x31\x34\x36\x22\
-\x0d\x0a\x20\x20\x20\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\
-\x73\x63\x61\x6c\x65\x28\x30\x2e\x30\x30\x30\x34\x38\x38\x32\x38\
-\x31\x32\x35\x2c\x2d\x30\x2e\x30\x30\x30\x34\x38\x38\x32\x38\x31\
-\x32\x35\x29\x22\x3e\x0d\x0a\x20\x20\x20\x3c\x70\x61\x74\x68\x0d\
-\x0a\x20\x20\x20\x64\x3d\x22\x4d\x20\x31\x37\x34\x2c\x30\x20\x4c\
-\x20\x36\x30\x32\x2c\x37\x33\x39\x20\x31\x37\x34\x2c\x31\x34\x38\
-\x31\x20\x31\x34\x35\x36\x2c\x37\x33\x39\x20\x31\x37\x34\x2c\x30\
-\x20\x5a\x20\x4d\x20\x31\x33\x35\x38\x2c\x37\x33\x39\x20\x4c\x20\
-\x33\x30\x39\x2c\x31\x33\x34\x36\x20\x36\x35\x39\x2c\x37\x33\x39\
-\x20\x31\x33\x35\x38\x2c\x37\x33\x39\x20\x5a\x22\x0d\x0a\x20\x20\
-\x20\x69\x64\x3d\x22\x70\x61\x74\x68\x32\x30\x22\x20\x2f\x3e\x0d\
-\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x3c\x67\x0d\x0a\x20\
-\x20\x20\x69\x64\x3d\x22\x62\x75\x6c\x6c\x65\x74\x2d\x63\x68\x61\
-\x72\x2d\x74\x65\x6d\x70\x6c\x61\x74\x65\x2d\x31\x30\x31\x33\x32\
-\x22\x0d\x0a\x20\x20\x20\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\
-\x22\x73\x63\x61\x6c\x65\x28\x30\x2e\x30\x30\x30\x34\x38\x38\x32\
-\x38\x31\x32\x35\x2c\x2d\x30\x2e\x30\x30\x30\x34\x38\x38\x32\x38\
-\x31\x32\x35\x29\x22\x3e\x0d\x0a\x20\x20\x20\x3c\x70\x61\x74\x68\
-\x0d\x0a\x20\x20\x20\x64\x3d\x22\x4d\x20\x32\x30\x31\x35\x2c\x37\
-\x33\x39\x20\x4c\x20\x31\x32\x37\x36\x2c\x30\x20\x37\x31\x37\x2c\
-\x30\x20\x31\x32\x36\x30\x2c\x35\x34\x33\x20\x31\x37\x34\x2c\x35\
-\x34\x33\x20\x31\x37\x34\x2c\x39\x33\x36\x20\x31\x32\x36\x30\x2c\
-\x39\x33\x36\x20\x37\x31\x37\x2c\x31\x34\x38\x31\x20\x31\x32\x37\
-\x34\x2c\x31\x34\x38\x31\x20\x32\x30\x31\x35\x2c\x37\x33\x39\x20\
-\x5a\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x70\x61\x74\x68\x32\
-\x33\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\
-\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x62\x75\x6c\x6c\
-\x65\x74\x2d\x63\x68\x61\x72\x2d\x74\x65\x6d\x70\x6c\x61\x74\x65\
-\x2d\x31\x30\x30\x30\x37\x22\x0d\x0a\x20\x20\x20\x74\x72\x61\x6e\
-\x73\x66\x6f\x72\x6d\x3d\x22\x73\x63\x61\x6c\x65\x28\x30\x2e\x30\
-\x30\x30\x34\x38\x38\x32\x38\x31\x32\x35\x2c\x2d\x30\x2e\x30\x30\
-\x30\x34\x38\x38\x32\x38\x31\x32\x35\x29\x22\x3e\x0d\x0a\x20\x20\
-\x20\x3c\x70\x61\x74\x68\x0d\x0a\x20\x20\x20\x64\x3d\x22\x4d\x20\
-\x30\x2c\x2d\x32\x20\x43\x20\x2d\x37\x2c\x31\x34\x20\x2d\x31\x36\
-\x2c\x32\x37\x20\x2d\x32\x35\x2c\x33\x37\x20\x4c\x20\x33\x35\x36\
-\x2c\x35\x36\x37\x20\x43\x20\x32\x36\x32\x2c\x38\x32\x33\x20\x32\
-\x31\x35\x2c\x39\x35\x32\x20\x32\x31\x35\x2c\x39\x35\x34\x20\x32\
-\x31\x35\x2c\x39\x37\x39\x20\x32\x32\x38\x2c\x39\x39\x32\x20\x32\
-\x35\x35\x2c\x39\x39\x32\x20\x32\x36\x34\x2c\x39\x39\x32\x20\x32\
-\x37\x36\x2c\x39\x39\x30\x20\x32\x38\x39\x2c\x39\x38\x37\x20\x33\
-\x31\x30\x2c\x39\x39\x31\x20\x33\x33\x31\x2c\x39\x39\x39\x20\x33\
-\x35\x34\x2c\x31\x30\x31\x32\x20\x4c\x20\x33\x38\x31\x2c\x39\x39\
-\x39\x20\x34\x39\x32\x2c\x37\x34\x38\x20\x37\x37\x32\x2c\x31\x30\
-\x34\x39\x20\x38\x33\x36\x2c\x31\x30\x32\x34\x20\x38\x36\x30\x2c\
-\x31\x30\x34\x39\x20\x43\x20\x38\x38\x31\x2c\x31\x30\x33\x39\x20\
-\x39\x30\x31\x2c\x31\x30\x32\x35\x20\x39\x32\x32\x2c\x31\x30\x30\
-\x36\x20\x38\x38\x36\x2c\x39\x33\x37\x20\x38\x33\x35\x2c\x38\x36\
-\x33\x20\x37\x37\x30\x2c\x37\x38\x34\x20\x37\x36\x39\x2c\x37\x38\
-\x33\x20\x37\x31\x30\x2c\x37\x31\x36\x20\x35\x39\x34\x2c\x35\x38\
-\x34\x20\x4c\x20\x37\x37\x34\x2c\x32\x32\x33\x20\x43\x20\x37\x37\
-\x34\x2c\x31\x39\x36\x20\x37\x35\x33\x2c\x31\x36\x38\x20\x37\x31\
-\x31\x2c\x31\x33\x39\x20\x4c\x20\x37\x32\x37\x2c\x31\x31\x39\x20\
-\x43\x20\x37\x31\x37\x2c\x39\x30\x20\x36\x39\x39\x2c\x37\x36\x20\
-\x36\x37\x32\x2c\x37\x36\x20\x36\x34\x31\x2c\x37\x36\x20\x35\x37\
-\x30\x2c\x31\x37\x38\x20\x34\x35\x37\x2c\x33\x38\x31\x20\x4c\x20\
-\x31\x36\x34\x2c\x2d\x37\x36\x20\x43\x20\x31\x34\x32\x2c\x2d\x31\
-\x31\x30\x20\x31\x31\x31\x2c\x2d\x31\x32\x37\x20\x37\x32\x2c\x2d\
-\x31\x32\x37\x20\x33\x30\x2c\x2d\x31\x32\x37\x20\x39\x2c\x2d\x31\
-\x31\x30\x20\x38\x2c\x2d\x37\x36\x20\x31\x2c\x2d\x36\x37\x20\x2d\
-\x32\x2c\x2d\x35\x32\x20\x2d\x32\x2c\x2d\x33\x32\x20\x2d\x32\x2c\
-\x2d\x32\x33\x20\x2d\x31\x2c\x2d\x31\x33\x20\x30\x2c\x2d\x32\x20\
-\x5a\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x70\x61\x74\x68\x32\
-\x36\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\
-\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x62\x75\x6c\x6c\
-\x65\x74\x2d\x63\x68\x61\x72\x2d\x74\x65\x6d\x70\x6c\x61\x74\x65\
-\x2d\x31\x30\x30\x30\x34\x22\x0d\x0a\x20\x20\x20\x74\x72\x61\x6e\
-\x73\x66\x6f\x72\x6d\x3d\x22\x73\x63\x61\x6c\x65\x28\x30\x2e\x30\
-\x30\x30\x34\x38\x38\x32\x38\x31\x32\x35\x2c\x2d\x30\x2e\x30\x30\
-\x30\x34\x38\x38\x32\x38\x31\x32\x35\x29\x22\x3e\x0d\x0a\x20\x20\
-\x20\x3c\x70\x61\x74\x68\x0d\x0a\x20\x20\x20\x64\x3d\x22\x4d\x20\
-\x32\x38\x35\x2c\x2d\x33\x33\x20\x43\x20\x31\x38\x32\x2c\x2d\x33\
-\x33\x20\x31\x31\x31\x2c\x33\x30\x20\x37\x34\x2c\x31\x35\x36\x20\
-\x35\x32\x2c\x32\x32\x38\x20\x34\x31\x2c\x33\x33\x33\x20\x34\x31\
-\x2c\x34\x37\x31\x20\x34\x31\x2c\x35\x34\x39\x20\x35\x35\x2c\x36\
-\x31\x36\x20\x38\x32\x2c\x36\x37\x32\x20\x31\x31\x36\x2c\x37\x34\
-\x33\x20\x31\x36\x39\x2c\x37\x37\x38\x20\x32\x34\x30\x2c\x37\x37\
-\x38\x20\x32\x39\x33\x2c\x37\x37\x38\x20\x33\x32\x38\x2c\x37\x34\
-\x37\x20\x33\x34\x36\x2c\x36\x38\x34\x20\x4c\x20\x33\x36\x39\x2c\
-\x35\x30\x38\x20\x43\x20\x33\x37\x37\x2c\x34\x34\x34\x20\x33\x39\
-\x37\x2c\x34\x31\x31\x20\x34\x32\x38\x2c\x34\x31\x30\x20\x4c\x20\
-\x31\x31\x36\x33\x2c\x31\x31\x31\x36\x20\x43\x20\x31\x31\x37\x34\
-\x2c\x31\x31\x32\x37\x20\x31\x31\x39\x36\x2c\x31\x31\x33\x33\x20\
-\x31\x32\x32\x39\x2c\x31\x31\x33\x33\x20\x31\x32\x37\x31\x2c\x31\
-\x31\x33\x33\x20\x31\x32\x39\x32\x2c\x31\x31\x31\x38\x20\x31\x32\
-\x39\x32\x2c\x31\x30\x38\x37\x20\x4c\x20\x31\x32\x39\x32\x2c\x39\
-\x36\x35\x20\x43\x20\x31\x32\x39\x32\x2c\x39\x32\x39\x20\x31\x32\
-\x38\x32\x2c\x39\x30\x31\x20\x31\x32\x36\x32\x2c\x38\x38\x31\x20\
-\x4c\x20\x34\x34\x32\x2c\x34\x37\x20\x43\x20\x33\x39\x30\x2c\x2d\
-\x36\x20\x33\x33\x38\x2c\x2d\x33\x33\x20\x32\x38\x35\x2c\x2d\x33\
-\x33\x20\x5a\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x70\x61\x74\
-\x68\x32\x39\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\
-\x0a\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x62\x75\
-\x6c\x6c\x65\x74\x2d\x63\x68\x61\x72\x2d\x74\x65\x6d\x70\x6c\x61\
-\x74\x65\x2d\x39\x36\x37\x39\x22\x0d\x0a\x20\x20\x20\x74\x72\x61\
-\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x73\x63\x61\x6c\x65\x28\x30\x2e\
-\x30\x30\x30\x34\x38\x38\x32\x38\x31\x32\x35\x2c\x2d\x30\x2e\x30\
-\x30\x30\x34\x38\x38\x32\x38\x31\x32\x35\x29\x22\x3e\x0d\x0a\x20\
-\x20\x20\x3c\x70\x61\x74\x68\x0d\x0a\x20\x20\x20\x64\x3d\x22\x4d\
-\x20\x38\x31\x33\x2c\x30\x20\x43\x20\x36\x33\x32\x2c\x30\x20\x34\
-\x38\x39\x2c\x35\x34\x20\x33\x38\x33\x2c\x31\x36\x31\x20\x32\x37\
-\x36\x2c\x32\x36\x38\x20\x32\x32\x33\x2c\x34\x31\x31\x20\x32\x32\
-\x33\x2c\x35\x39\x32\x20\x32\x32\x33\x2c\x37\x37\x33\x20\x32\x37\
-\x36\x2c\x39\x31\x36\x20\x33\x38\x33\x2c\x31\x30\x32\x33\x20\x34\
-\x38\x39\x2c\x31\x31\x33\x30\x20\x36\x33\x32\x2c\x31\x31\x38\x34\
-\x20\x38\x31\x33\x2c\x31\x31\x38\x34\x20\x39\x39\x32\x2c\x31\x31\
-\x38\x34\x20\x31\x31\x33\x36\x2c\x31\x31\x33\x30\x20\x31\x32\x34\
-\x35\x2c\x31\x30\x32\x33\x20\x31\x33\x35\x33\x2c\x39\x31\x36\x20\
-\x31\x34\x30\x37\x2c\x37\x37\x32\x20\x31\x34\x30\x37\x2c\x35\x39\
-\x32\x20\x31\x34\x30\x37\x2c\x34\x31\x32\x20\x31\x33\x35\x33\x2c\
-\x32\x36\x38\x20\x31\x32\x34\x35\x2c\x31\x36\x31\x20\x31\x31\x33\
-\x36\x2c\x35\x34\x20\x39\x39\x32\x2c\x30\x20\x38\x31\x33\x2c\x30\
-\x20\x5a\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x70\x61\x74\x68\
-\x33\x32\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\
-\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x62\x75\x6c\
-\x6c\x65\x74\x2d\x63\x68\x61\x72\x2d\x74\x65\x6d\x70\x6c\x61\x74\
-\x65\x2d\x38\x32\x32\x36\x22\x0d\x0a\x20\x20\x20\x74\x72\x61\x6e\
-\x73\x66\x6f\x72\x6d\x3d\x22\x73\x63\x61\x6c\x65\x28\x30\x2e\x30\
-\x30\x30\x34\x38\x38\x32\x38\x31\x32\x35\x2c\x2d\x30\x2e\x30\x30\
-\x30\x34\x38\x38\x32\x38\x31\x32\x35\x29\x22\x3e\x0d\x0a\x20\x20\
-\x20\x3c\x70\x61\x74\x68\x0d\x0a\x20\x20\x20\x64\x3d\x22\x4d\x20\
-\x33\x34\x36\x2c\x34\x35\x37\x20\x43\x20\x32\x37\x33\x2c\x34\x35\
-\x37\x20\x32\x30\x39\x2c\x34\x38\x33\x20\x31\x35\x35\x2c\x35\x33\
-\x35\x20\x31\x30\x31\x2c\x35\x38\x36\x20\x37\x34\x2c\x36\x34\x39\
-\x20\x37\x34\x2c\x37\x32\x33\x20\x37\x34\x2c\x37\x39\x36\x20\x31\
-\x30\x31\x2c\x38\x35\x39\x20\x31\x35\x35\x2c\x39\x31\x31\x20\x32\
-\x30\x39\x2c\x39\x36\x33\x20\x32\x37\x33\x2c\x39\x38\x39\x20\x33\
-\x34\x36\x2c\x39\x38\x39\x20\x34\x31\x39\x2c\x39\x38\x39\x20\x34\
-\x38\x30\x2c\x39\x36\x33\x20\x35\x33\x31\x2c\x39\x31\x30\x20\x35\
-\x38\x32\x2c\x38\x35\x39\x20\x36\x30\x38\x2c\x37\x39\x36\x20\x36\
-\x30\x38\x2c\x37\x32\x33\x20\x36\x30\x38\x2c\x36\x34\x38\x20\x35\
-\x38\x33\x2c\x35\x38\x36\x20\x35\x33\x32\x2c\x35\x33\x35\x20\x34\
-\x38\x32\x2c\x34\x38\x33\x20\x34\x32\x30\x2c\x34\x35\x37\x20\x33\
-\x34\x36\x2c\x34\x35\x37\x20\x5a\x22\x0d\x0a\x20\x20\x20\x69\x64\
-\x3d\x22\x70\x61\x74\x68\x33\x35\x22\x20\x2f\x3e\x0d\x0a\x20\x20\
-\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\
-\x64\x3d\x22\x62\x75\x6c\x6c\x65\x74\x2d\x63\x68\x61\x72\x2d\x74\
-\x65\x6d\x70\x6c\x61\x74\x65\x2d\x38\x32\x31\x31\x22\x0d\x0a\x20\
-\x20\x20\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x73\x63\x61\
-\x6c\x65\x28\x30\x2e\x30\x30\x30\x34\x38\x38\x32\x38\x31\x32\x35\
-\x2c\x2d\x30\x2e\x30\x30\x30\x34\x38\x38\x32\x38\x31\x32\x35\x29\
-\x22\x3e\x0d\x0a\x20\x20\x20\x3c\x70\x61\x74\x68\x0d\x0a\x20\x20\
-\x20\x64\x3d\x22\x4d\x20\x2d\x34\x2c\x34\x35\x39\x20\x4c\x20\x31\
-\x31\x33\x35\x2c\x34\x35\x39\x20\x31\x31\x33\x35\x2c\x36\x30\x36\
-\x20\x2d\x34\x2c\x36\x30\x36\x20\x2d\x34\x2c\x34\x35\x39\x20\x5a\
-\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x70\x61\x74\x68\x33\x38\
-\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\
-\x3c\x67\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x62\x75\x6c\x6c\x65\
-\x74\x2d\x63\x68\x61\x72\x2d\x74\x65\x6d\x70\x6c\x61\x74\x65\x2d\
-\x36\x31\x35\x34\x38\x22\x0d\x0a\x20\x20\x20\x74\x72\x61\x6e\x73\
-\x66\x6f\x72\x6d\x3d\x22\x73\x63\x61\x6c\x65\x28\x30\x2e\x30\x30\
-\x30\x34\x38\x38\x32\x38\x31\x32\x35\x2c\x2d\x30\x2e\x30\x30\x30\
-\x34\x38\x38\x32\x38\x31\x32\x35\x29\x22\x3e\x0d\x0a\x20\x20\x20\
-\x3c\x70\x61\x74\x68\x0d\x0a\x20\x20\x20\x64\x3d\x22\x4d\x20\x31\
-\x37\x33\x2c\x37\x34\x30\x20\x43\x20\x31\x37\x33\x2c\x39\x30\x33\
-\x20\x32\x33\x31\x2c\x31\x30\x34\x33\x20\x33\x34\x36\x2c\x31\x31\
-\x35\x39\x20\x34\x36\x32\x2c\x31\x32\x37\x34\x20\x36\x30\x31\x2c\
-\x31\x33\x33\x32\x20\x37\x36\x35\x2c\x31\x33\x33\x32\x20\x39\x32\
-\x38\x2c\x31\x33\x33\x32\x20\x31\x30\x36\x37\x2c\x31\x32\x37\x34\
-\x20\x31\x31\x38\x33\x2c\x31\x31\x35\x39\x20\x31\x32\x39\x39\x2c\
-\x31\x30\x34\x33\x20\x31\x33\x35\x37\x2c\x39\x30\x33\x20\x31\x33\
-\x35\x37\x2c\x37\x34\x30\x20\x31\x33\x35\x37\x2c\x35\x37\x37\x20\
-\x31\x32\x39\x39\x2c\x34\x33\x37\x20\x31\x31\x38\x33\x2c\x33\x32\
-\x32\x20\x31\x30\x36\x37\x2c\x32\x30\x36\x20\x39\x32\x38\x2c\x31\
-\x34\x38\x20\x37\x36\x35\x2c\x31\x34\x38\x20\x36\x30\x31\x2c\x31\
-\x34\x38\x20\x34\x36\x32\x2c\x32\x30\x36\x20\x33\x34\x36\x2c\x33\
-\x32\x32\x20\x32\x33\x31\x2c\x34\x33\x37\x20\x31\x37\x33\x2c\x35\
-\x37\x37\x20\x31\x37\x33\x2c\x37\x34\x30\x20\x5a\x22\x0d\x0a\x20\
-\x20\x20\x69\x64\x3d\x22\x70\x61\x74\x68\x34\x31\x22\x20\x2f\x3e\
-\x0d\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x3c\x2f\x64\x65\x66\
-\x73\x3e\x0d\x0a\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\
-\x67\x34\x39\x22\x3e\x0d\x0a\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\
-\x69\x64\x3d\x22\x69\x64\x32\x22\x0d\x0a\x20\x20\x20\x63\x6c\x61\
-\x73\x73\x3d\x22\x4d\x61\x73\x74\x65\x72\x5f\x53\x6c\x69\x64\x65\
-\x22\x3e\x0d\x0a\x20\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\x64\
-\x3d\x22\x62\x67\x2d\x69\x64\x32\x22\x0d\x0a\x20\x20\x20\x63\x6c\
-\x61\x73\x73\x3d\x22\x42\x61\x63\x6b\x67\x72\x6f\x75\x6e\x64\x22\
-\x20\x2f\x3e\x0d\x0a\x20\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\
-\x64\x3d\x22\x62\x6f\x2d\x69\x64\x32\x22\x0d\x0a\x20\x20\x20\x63\
-\x6c\x61\x73\x73\x3d\x22\x42\x61\x63\x6b\x67\x72\x6f\x75\x6e\x64\
-\x4f\x62\x6a\x65\x63\x74\x73\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x3c\
-\x2f\x67\x3e\x0d\x0a\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x3c\x67\x0d\
-\x0a\x20\x20\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\
-\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\
-\x50\x6f\x6c\x79\x50\x6f\x6c\x79\x67\x6f\x6e\x53\x68\x61\x70\x65\
-\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x67\x36\x31\x22\x3e\x0d\
-\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\
-\x64\x3d\x22\x69\x64\x34\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\
-\x20\x20\x3c\x72\x65\x63\x74\x0d\x0a\x20\x20\x20\x63\x6c\x61\x73\
-\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x0d\
-\x0a\x20\x20\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\
-\x22\x0d\x0a\x20\x20\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\
-\x22\x0d\x0a\x20\x20\x20\x78\x3d\x22\x30\x22\x0d\x0a\x20\x20\x20\
-\x79\x3d\x22\x30\x22\x0d\x0a\x20\x20\x20\x77\x69\x64\x74\x68\x3d\
-\x22\x38\x34\x39\x22\x0d\x0a\x20\x20\x20\x68\x65\x69\x67\x68\x74\
-\x3d\x22\x38\x34\x39\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x72\
-\x65\x63\x74\x35\x38\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x2f\
-\x67\x3e\x3c\x67\x0d\x0a\x20\x20\x20\x63\x6c\x61\x73\x73\x3d\x22\
-\x47\x72\x6f\x75\x70\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x67\
-\x38\x34\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x67\x0d\
-\x0a\x20\x20\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\
-\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\
-\x50\x6f\x6c\x79\x50\x6f\x6c\x79\x67\x6f\x6e\x53\x68\x61\x70\x65\
-\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x67\x36\x38\x22\x3e\x0d\
-\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\
-\x69\x64\x3d\x22\x69\x64\x35\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x0d\x0a\x20\x20\x20\x63\x6c\
-\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\
-\x22\x0d\x0a\x20\x20\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\
-\x6e\x65\x22\x0d\x0a\x20\x20\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\
-\x6e\x65\x22\x0d\x0a\x20\x20\x20\x78\x3d\x22\x31\x33\x37\x22\x0d\
-\x0a\x20\x20\x20\x79\x3d\x22\x31\x38\x37\x22\x0d\x0a\x20\x20\x20\
-\x77\x69\x64\x74\x68\x3d\x22\x31\x36\x31\x22\x0d\x0a\x20\x20\x20\
-\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x37\x22\x0d\x0a\x20\x20\
-\x20\x69\x64\x3d\x22\x72\x65\x63\x74\x36\x33\x22\x20\x2f\x3e\x0d\
-\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x0d\
-\x0a\x20\x20\x20\x66\x69\x6c\x6c\x3d\x22\x23\x30\x30\x30\x30\x30\
-\x30\x22\x0d\x0a\x20\x20\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x6e\
-\x6f\x6e\x65\x22\x0d\x0a\x20\x20\x20\x64\x3d\x22\x4d\x20\x31\x33\
-\x37\x2c\x36\x37\x33\x20\x56\x20\x31\x38\x37\x20\x68\x20\x31\x35\
-\x39\x20\x76\x20\x39\x32\x20\x48\x20\x31\x39\x31\x20\x76\x20\x31\
-\x31\x38\x20\x68\x20\x39\x39\x20\x76\x20\x39\x31\x20\x68\x20\x2d\
-\x39\x39\x20\x76\x20\x31\x38\x35\x20\x7a\x22\x0d\x0a\x20\x20\x20\
-\x69\x64\x3d\x22\x70\x61\x74\x68\x36\x35\x22\x20\x2f\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\
-\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x63\x6c\x61\x73\x73\x3d\x22\
-\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\
-\x77\x69\x6e\x67\x2e\x50\x6f\x6c\x79\x50\x6f\x6c\x79\x67\x6f\x6e\
-\x53\x68\x61\x70\x65\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x67\
-\x37\x35\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x67\
-\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x69\x64\x36\x22\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x0d\x0a\
-\x20\x20\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\
-\x6e\x67\x42\x6f\x78\x22\x0d\x0a\x20\x20\x20\x73\x74\x72\x6f\x6b\
-\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x0d\x0a\x20\x20\x20\x66\x69\x6c\
-\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x0d\x0a\x20\x20\x20\x78\x3d\x22\
-\x33\x33\x37\x22\x0d\x0a\x20\x20\x20\x79\x3d\x22\x31\x38\x37\x22\
-\x0d\x0a\x20\x20\x20\x77\x69\x64\x74\x68\x3d\x22\x31\x36\x32\x22\
-\x0d\x0a\x20\x20\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x37\
-\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x72\x65\x63\x74\x37\x30\
-\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x20\x3c\
-\x70\x61\x74\x68\x0d\x0a\x20\x20\x20\x66\x69\x6c\x6c\x3d\x22\x23\
-\x30\x30\x30\x30\x30\x30\x22\x0d\x0a\x20\x20\x20\x73\x74\x72\x6f\
-\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x0d\x0a\x20\x20\x20\x64\x3d\
-\x22\x4d\x20\x33\x33\x38\x2c\x36\x37\x33\x20\x56\x20\x31\x38\x37\
-\x20\x68\x20\x31\x35\x39\x20\x76\x20\x39\x32\x20\x48\x20\x33\x39\
-\x32\x20\x76\x20\x31\x31\x38\x20\x68\x20\x39\x39\x20\x76\x20\x39\
-\x31\x20\x68\x20\x2d\x39\x39\x20\x76\x20\x31\x38\x35\x20\x7a\x22\
-\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x70\x61\x74\x68\x37\x32\x22\
-\x20\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\
-\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x63\x6c\
-\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\
-\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x50\x6f\x6c\x79\x50\x6f\
-\x6c\x79\x67\x6f\x6e\x53\x68\x61\x70\x65\x22\x0d\x0a\x20\x20\x20\
-\x69\x64\x3d\x22\x67\x38\x32\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x20\x3c\x67\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x69\x64\
-\x37\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x72\
-\x65\x63\x74\x0d\x0a\x20\x20\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\
-\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x0d\x0a\x20\x20\x20\
-\x73\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x0d\x0a\x20\
-\x20\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x0d\x0a\x20\
-\x20\x20\x78\x3d\x22\x35\x32\x34\x22\x0d\x0a\x20\x20\x20\x79\x3d\
-\x22\x31\x38\x37\x22\x0d\x0a\x20\x20\x20\x77\x69\x64\x74\x68\x3d\
-\x22\x31\x38\x37\x22\x0d\x0a\x20\x20\x20\x68\x65\x69\x67\x68\x74\
-\x3d\x22\x34\x38\x37\x22\x0d\x0a\x20\x20\x20\x69\x64\x3d\x22\x72\
-\x65\x63\x74\x37\x37\x22\x20\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x0d\x0a\x20\x20\x20\x66\x69\
-\x6c\x6c\x3d\x22\x23\x30\x30\x30\x30\x30\x30\x22\x0d\x0a\x20\x20\
-\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x6e\x6f\x6e\x65\x22\x0d\x0a\
-\x20\x20\x20\x64\x3d\x22\x4d\x20\x35\x39\x30\x2c\x36\x37\x33\x20\
-\x56\x20\x32\x37\x39\x20\x68\x20\x2d\x36\x36\x20\x76\x20\x2d\x39\
-\x32\x20\x68\x20\x31\x38\x35\x20\x76\x20\x39\x32\x20\x68\x20\x2d\
-\x36\x36\x20\x76\x20\x33\x39\x34\x20\x7a\x22\x0d\x0a\x20\x20\x20\
-\x69\x64\x3d\x22\x70\x61\x74\x68\x37\x39\x22\x20\x2f\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\
-\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x3c\x2f\x67\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
-\x00\x00\x01\xc5\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x31\x30\
+\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x33\x34\x22\x20\x76\x69\
+\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x31\x30\x20\x33\x34\
+\x22\x3e\x0d\x0a\x20\x20\x3c\x21\x2d\x2d\x20\x3c\x70\x61\x74\x68\
+\x20\x64\x3d\x22\x4d\x30\x20\x30\x76\x32\x68\x32\x76\x2d\x32\x68\
+\x2d\x32\x7a\x6d\x33\x20\x30\x76\x32\x68\x32\x76\x2d\x32\x68\x2d\
+\x32\x7a\x6d\x33\x20\x30\x76\x32\x68\x32\x76\x2d\x32\x68\x2d\x32\
+\x7a\x22\x20\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\
+\x61\x6e\x73\x6c\x61\x74\x65\x28\x30\x20\x33\x29\x22\x20\x2f\x3e\
+\x20\x2d\x2d\x3e\x0d\x0a\x20\x3c\x72\x65\x63\x74\x20\x78\x3d\x22\
+\x31\x22\x20\x79\x3d\x22\x31\x22\x20\x77\x69\x64\x74\x68\x3d\x22\
+\x38\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x66\x69\
+\x6c\x6c\x3d\x22\x67\x72\x65\x79\x22\x20\x73\x74\x72\x6f\x6b\x65\
+\x3d\x22\x72\x65\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\
+\x64\x74\x68\x3d\x22\x32\x22\x20\x20\x2f\x3e\x20\x0d\x0a\x20\x3c\
+\x72\x65\x63\x74\x20\x78\x3d\x22\x31\x22\x20\x79\x3d\x22\x31\x33\
+\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\x20\x68\x65\x69\x67\
+\x68\x74\x3d\x22\x38\x22\x20\x66\x69\x6c\x6c\x3d\x22\x72\x65\x64\
+\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x67\x72\x65\x79\x22\x20\
+\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x22\
+\x20\x20\x2f\x3e\x20\x0d\x0a\x20\x3c\x72\x65\x63\x74\x20\x78\x3d\
+\x22\x31\x22\x20\x79\x3d\x22\x32\x35\x22\x20\x77\x69\x64\x74\x68\
+\x3d\x22\x38\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\
+\x66\x69\x6c\x6c\x3d\x22\x67\x72\x65\x79\x22\x20\x73\x74\x72\x6f\
+\x6b\x65\x3d\x22\x72\x65\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
+\x77\x69\x64\x74\x68\x3d\x22\x32\x22\x20\x20\x2f\x3e\x20\x0d\x0a\
+\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x01\x91\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x2e\x35\x20\
-\x30\x63\x2d\x31\x2e\x39\x33\x20\x30\x2d\x33\x2e\x35\x20\x31\x2e\
-\x35\x37\x2d\x33\x2e\x35\x20\x33\x2e\x35\x73\x31\x2e\x35\x37\x20\
-\x33\x2e\x35\x20\x33\x2e\x35\x20\x33\x2e\x35\x63\x2e\x35\x39\x20\
-\x30\x20\x31\x2e\x31\x37\x2d\x2e\x31\x34\x20\x31\x2e\x36\x36\x2d\
-\x2e\x34\x31\x61\x31\x20\x31\x20\x30\x20\x30\x20\x30\x20\x2e\x31\
-\x33\x2e\x31\x33\x6c\x31\x20\x31\x61\x31\x2e\x30\x32\x20\x31\x2e\
-\x30\x32\x20\x30\x20\x31\x20\x30\x20\x31\x2e\x34\x34\x2d\x31\x2e\
-\x34\x34\x6c\x2d\x31\x2d\x31\x61\x31\x20\x31\x20\x30\x20\x30\x20\
-\x30\x2d\x2e\x31\x36\x2d\x2e\x31\x33\x63\x2e\x32\x37\x2d\x2e\x34\
-\x39\x2e\x34\x34\x2d\x31\x2e\x30\x36\x2e\x34\x34\x2d\x31\x2e\x36\
-\x36\x20\x30\x2d\x31\x2e\x39\x33\x2d\x31\x2e\x35\x37\x2d\x33\x2e\
-\x35\x2d\x33\x2e\x35\x2d\x33\x2e\x35\x7a\x6d\x30\x20\x31\x63\x31\
-\x2e\x33\x39\x20\x30\x20\x32\x2e\x35\x20\x31\x2e\x31\x31\x20\x32\
-\x2e\x35\x20\x32\x2e\x35\x20\x30\x20\x2e\x36\x36\x2d\x2e\x32\x34\
-\x20\x31\x2e\x32\x37\x2d\x2e\x36\x36\x20\x31\x2e\x37\x32\x2d\x2e\
-\x30\x31\x2e\x30\x31\x2d\x2e\x30\x32\x2e\x30\x32\x2d\x2e\x30\x33\
-\x2e\x30\x33\x61\x31\x20\x31\x20\x30\x20\x30\x20\x30\x2d\x2e\x31\
-\x33\x2e\x31\x33\x63\x2d\x2e\x34\x34\x2e\x34\x2d\x31\x2e\x30\x34\
-\x2e\x36\x33\x2d\x31\x2e\x36\x39\x2e\x36\x33\x2d\x31\x2e\x33\x39\
-\x20\x30\x2d\x32\x2e\x35\x2d\x31\x2e\x31\x31\x2d\x32\x2e\x35\x2d\
-\x32\x2e\x35\x73\x31\x2e\x31\x31\x2d\x32\x2e\x35\x20\x32\x2e\x35\
-\x2d\x32\x2e\x35\x7a\x22\x0d\x0a\x20\x20\x2f\x3e\x0d\x0a\x3c\x2f\
-\x73\x76\x67\x3e\
-\x00\x00\x00\xe3\
+\x30\x2f\x73\x76\x67\x22\x20\x20\x77\x69\x64\x74\x68\x3d\x22\x34\
+\x38\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\
+\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\
+\x38\x22\x3e\x0d\x0a\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x20\
+\x33\x30\x2c\x36\x20\x48\x20\x31\x38\x20\x76\x20\x38\x20\x4c\x20\
+\x38\x2c\x32\x34\x20\x48\x20\x34\x30\x20\x4c\x20\x33\x30\x2c\x31\
+\x34\x20\x5a\x20\x6d\x20\x2d\x36\x2c\x32\x37\x20\x63\x20\x33\x2e\
+\x35\x33\x2c\x30\x20\x36\x2e\x35\x38\x2c\x2d\x32\x2e\x30\x34\x20\
+\x38\x2e\x30\x35\x2c\x2d\x35\x20\x48\x20\x31\x35\x2e\x39\x34\x20\
+\x63\x20\x31\x2e\x34\x38\x2c\x32\x2e\x39\x36\x20\x34\x2e\x35\x33\
+\x2c\x35\x20\x38\x2e\x30\x36\x2c\x35\x20\x7a\x20\x4d\x20\x34\x31\
+\x2e\x35\x34\x2c\x32\x38\x20\x48\x20\x33\x37\x2e\x34\x31\x20\x43\
+\x20\x33\x35\x2e\x36\x39\x2c\x33\x33\x2e\x37\x38\x20\x33\x30\x2e\
+\x33\x34\x2c\x33\x38\x20\x32\x34\x2c\x33\x38\x20\x31\x37\x2e\x36\
+\x36\x2c\x33\x38\x20\x31\x32\x2e\x33\x31\x2c\x33\x33\x2e\x37\x38\
+\x20\x31\x30\x2e\x35\x39\x2c\x32\x38\x20\x48\x20\x36\x2e\x34\x36\
+\x20\x63\x20\x31\x2e\x38\x32\x2c\x38\x2e\x30\x31\x20\x38\x2e\x39\
+\x37\x2c\x31\x34\x20\x31\x37\x2e\x35\x34\x2c\x31\x34\x20\x38\x2e\
+\x35\x37\x2c\x30\x20\x31\x35\x2e\x37\x32\x2c\x2d\x35\x2e\x39\x39\
+\x20\x31\x37\x2e\x35\x34\x2c\x2d\x31\x34\x20\x7a\x22\x20\x2f\x3e\
+\x0d\x0a\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\
+\x34\x38\x76\x34\x38\x48\x30\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\
+\x6e\x6f\x6e\x65\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
+\
+\x00\x00\x00\xee\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x20\x30\x63\
-\x2d\x31\x2e\x31\x20\x30\x2d\x32\x20\x2e\x39\x2d\x32\x20\x32\x76\
-\x31\x68\x2d\x31\x76\x34\x68\x36\x76\x2d\x34\x68\x2d\x31\x76\x2d\
-\x31\x63\x30\x2d\x31\x2e\x31\x2d\x2e\x39\x2d\x32\x2d\x32\x2d\x32\
-\x7a\x6d\x30\x20\x31\x63\x2e\x35\x36\x20\x30\x20\x31\x20\x2e\x34\
-\x34\x20\x31\x20\x31\x76\x31\x68\x2d\x32\x76\x2d\x31\x63\x30\x2d\
-\x2e\x35\x36\x2e\x34\x34\x2d\x31\x20\x31\x2d\x31\x7a\x22\x20\x74\
-\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\
-\x61\x74\x65\x28\x31\x29\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\
-\x67\x3e\
-\x00\x00\x08\x41\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x64\x00\x00\x00\x64\x08\x06\x00\x00\x00\x70\xe2\x95\x54\
-\x00\x00\x08\x08\x49\x44\x41\x54\x78\xda\xed\x9d\x69\x48\x5c\x57\
-\x14\xc7\xeb\x8e\x51\xd4\xb1\x6e\x51\xd1\x6a\x1b\x6c\x94\x8a\x20\
-\x01\xeb\xbe\xe2\x16\xab\x36\x2e\xc1\xda\x60\x5a\x12\xdb\x1a\x49\
-\x49\xfc\xd8\x8f\xf9\x68\x4b\x8a\x35\x89\x2d\x49\xa5\x31\x52\x8d\
-\x8d\x1a\x5b\x5b\x71\xb7\x4b\x84\x22\x88\x41\x1b\x69\xa2\x51\xd4\
-\xba\xc5\x0d\xad\xb8\x77\xfe\x85\x0b\x22\x51\xdf\x8c\xef\xbe\x77\
-\xdf\x9b\xfb\x87\x30\x93\xc4\x79\xce\x9b\xdf\x9c\x7b\xef\x39\xf7\
-\xdc\x73\x4c\x77\x76\x76\x5e\xe1\x62\x47\xa6\xfc\x23\x60\x10\x48\
-\x41\x41\x41\xe9\x8d\x1b\x37\x3e\x11\xfa\xa2\x5b\xb7\x6e\x7d\x94\
-\x9f\x9f\x5f\x46\xe3\x0d\x3d\x7e\xfc\xf8\xad\xc2\xc2\xc2\x92\xda\
-\xda\xda\x74\x8d\x46\x33\xcf\x2d\x44\x80\xb4\xc3\x9c\x11\x8d\x37\
-\xf3\xe4\xc9\x93\x37\x23\x23\x23\x3b\xe6\xe6\xe6\xec\xc3\xc2\xc2\
-\x7e\xd5\x2a\xcc\xd0\xa0\x30\x03\x04\x30\xc2\xc3\xc3\xbb\x00\x03\
-\x7f\xef\xef\xef\xf7\x03\x94\x8e\x8e\x8e\x48\x07\x07\x87\x59\x0e\
-\xe4\x00\x6d\x6f\x6f\x1b\x8b\xf9\x26\x9e\x3e\x7d\xfa\x06\x60\xcc\
-\xcc\xcc\x38\xee\xfe\x77\x40\x09\x0d\x0d\xfd\x4d\xab\x50\x43\x81\
-\x22\xbb\x85\x3c\x7f\xfe\xfc\x35\x58\xc2\x5e\x18\x44\x83\x83\x83\
-\x3e\x80\xd2\xd9\xd9\x19\xe1\xec\xec\x3c\xc5\x81\x50\x04\x42\x60\
-\x4c\x4e\x4e\xba\x1c\xf4\x73\x80\x12\x1c\x1c\xfc\x87\x56\xc1\x6a\
-\x87\x22\x1b\x90\xb1\xb1\x31\x77\xc0\xc0\xa3\x90\x9f\x1f\x1a\x1a\
-\xf2\x06\x94\xae\xae\xae\x70\x37\x37\xb7\x71\x0e\x44\x44\x20\xb0\
-\x08\x5d\x60\xec\x86\x12\x12\x12\xf2\xbb\x56\x21\x6a\x85\x22\xf9\
-\xa4\x4e\x60\x60\xb8\xd2\xe7\xf5\x23\x23\x23\x9e\x80\x82\x39\xc5\
-\xd3\xd3\x73\x84\x03\x39\x82\x85\x60\xe2\x06\x0c\xac\xaa\x8e\xf2\
-\xa6\x09\x14\x0c\x5f\xde\xde\xde\x43\x1c\x88\x1e\x40\xe0\x5f\x60\
-\x69\x7b\x54\x18\x44\xe3\xe3\xe3\x6e\x64\xa2\x57\x13\x14\x49\x80\
-\x2c\x2e\x2e\xda\xc2\x03\x87\xf3\x27\xe6\x9b\x9f\x9a\x9a\x72\x06\
-\x14\x0c\x5f\x3e\x3e\x3e\x83\xaa\x01\x62\x64\x64\xb4\x43\x13\x08\
-\x42\x20\x88\x51\xd1\xb8\x01\x40\x81\xe5\xc1\xa3\x3f\x79\xf2\xe4\
-\x5f\xaa\x00\xa2\xeb\x07\xac\xeb\xa4\x7e\xfa\xf4\xe9\x1f\xeb\xea\
-\xea\xd2\x32\x32\x32\x6a\x36\x37\x37\x45\x8f\x30\x4f\x4f\x4f\x3b\
-\x11\x28\x7e\x7e\x7e\xfd\x7c\xc8\x12\xa0\xd4\xd4\xd4\xfa\x87\x0f\
-\x1f\xbe\x83\xc7\x8d\x8d\x0d\x33\xb1\x6f\x64\x76\x76\xd6\x81\x04\
-\x24\x95\x0c\x45\xd2\x55\x56\x62\x62\xe2\xcf\x5a\x25\x26\x27\x27\
-\xff\xb4\xb6\xb6\x66\x21\xf6\xcd\xcc\xcf\xcf\x6b\x00\xa5\xad\xad\
-\x2d\x3a\x20\x20\xa0\x97\x03\x11\xa0\x98\x98\x98\xd6\xe6\xe6\xe6\
-\xb8\xf8\xf8\xf8\xa6\xd5\xd5\x55\x4b\x1a\x50\x22\x22\x22\x3a\x31\
-\xd1\x2b\x11\x8a\x2c\x9e\x3a\xf9\x16\xc7\xc6\xc6\xb6\xac\xac\xac\
-\x58\x89\x7d\x53\x4b\x4b\x4b\x36\x80\xd2\xd2\xd2\x12\x7b\xea\xd4\
-\xa9\x3f\xb9\xa7\x2e\x40\x41\x41\x41\xdd\xf8\x16\x03\xca\xc2\xc2\
-\x82\x1d\x0d\x28\xd1\xd1\xd1\x6d\x00\xaf\x24\x28\xb2\x46\x7b\x03\
-\x03\x03\x7b\x10\x97\xc2\x0a\xe9\xc5\x8b\x17\xaf\x8a\x7d\x73\xcb\
-\xcb\xcb\xd6\x80\xd2\xd4\xd4\x14\x0f\x7f\x85\x03\x11\x20\x5f\x5f\
-\xdf\x81\x47\x8f\x1e\xbd\x8d\x3d\x0f\x2c\x5f\x69\x40\x81\x15\x62\
-\xf8\x52\x02\x14\x26\xb6\x70\x4f\x9c\x38\xf1\x77\x77\x77\x77\x10\
-\xa0\x4c\x4c\x4c\xb8\x8a\x7d\x93\x58\x3c\x00\x4a\x63\x63\x63\x12\
-\x22\x06\x1c\x88\x00\x79\x79\x79\x0d\xc3\x52\x30\xe1\x8f\x8e\x8e\
-\x7a\xd0\x80\x92\x90\x90\xf0\x8b\x56\x09\x2c\x43\x61\x62\x4f\x9d\
-\xc8\xc3\xc3\x63\x94\x0c\x5f\xc3\xc3\xc3\x5e\x62\x5f\x1f\xbe\x0f\
-\xa0\x34\x34\x34\xa4\xc4\xc5\xc5\x35\x73\x0b\x11\x20\x57\x57\xd7\
-\x09\x0c\x5f\x51\x51\x51\xed\x03\x03\x03\xbe\x34\xa0\xc0\x31\x45\
-\xde\x17\x1e\x39\x10\x01\x72\x72\x72\x9a\xc6\xea\x0b\xbe\x44\x5f\
-\x5f\x9f\xbf\xd8\xd7\x47\xe8\x26\x2d\x2d\xad\x0e\xf1\x35\xd6\xa0\
-\x30\x09\x04\xb2\xb3\xb3\x5b\x40\x5c\x0a\xcb\xd6\x9e\x9e\x9e\x40\
-\xb1\xaf\x8f\x20\x27\xa0\x54\x57\x57\x67\xa5\xa7\xa7\xd7\x72\x20\
-\x02\x64\x63\x63\xb3\x44\x9c\x47\x0c\x63\x34\xa0\x64\x66\x66\xde\
-\xd7\x2a\x93\x15\x28\x4c\x4d\xea\x2f\x93\x95\x95\xd5\x0a\xbc\x6d\
-\xc4\xbe\x60\x31\x62\x5f\x7f\x6b\x6b\xcb\x04\x50\x2a\x2a\x2a\x72\
-\xcf\x9e\x3d\xfb\x3d\xb7\x10\x01\xb2\xb4\xb4\x5c\x45\x40\x12\xe3\
-\x7d\x6b\x6b\x6b\x0c\x0d\x28\x39\x39\x39\x95\x78\x2e\x37\x14\x45\
-\x00\x81\x2c\x2c\x2c\xd6\x10\xba\xc7\xb7\xb9\xbe\xbe\x3e\x55\xec\
-\xeb\xe3\x9e\x00\x65\x7d\x7d\xdd\xfc\xdc\xb9\x73\xdf\x71\x20\x02\
-\x64\x66\x66\xb6\xf1\xe0\xc1\x83\x77\xf1\x2d\xc6\xb8\x4f\x03\x4a\
-\x5e\x5e\x5e\x39\x9e\xcb\x05\x45\x51\x40\x20\x63\x63\xe3\xed\xaa\
-\xaa\xaa\x6c\x73\x73\xf3\xf5\x7b\xf7\xee\xbd\x47\x0b\x0a\xfc\x95\
-\x0b\x17\x2e\x7c\xc3\x27\x75\x01\x42\x52\xc6\xdd\xbb\x77\xdf\xc7\
-\x30\x76\xe7\xce\x9d\x0f\x68\x40\xb9\x78\xf1\xe2\xd7\x78\x2e\x35\
-\x14\xc5\x59\xc8\x6e\x28\xb7\x6f\xdf\xfe\x10\x50\x6e\xde\xbc\xf9\
-\x31\x8d\xdf\x01\x28\xb0\x94\x4b\x97\x2e\x7d\xc5\x81\x08\x14\x8e\
-\xe2\x01\xca\xf5\xeb\xd7\x3f\xa5\x71\x7d\x1c\xaf\xc3\xa3\x54\x50\
-\xf4\xca\xcb\x62\x4d\x57\xaf\x5e\xfd\xbc\xbc\xbc\x3c\x8f\xc6\xce\
-\x23\x54\x5c\x5c\x5c\x74\xfe\xfc\xf9\x6f\xe1\x13\x49\x02\x84\x76\
-\x5e\x16\x4d\x91\x63\x0d\xb4\x60\x1c\x3f\x7e\xfc\x9f\xf6\xf6\xf6\
-\x28\x29\x60\x28\x76\x52\xdf\x0b\x43\xdf\x4c\xfa\xc3\x64\x6f\x6f\
-\x3f\x87\xd0\x0d\xf6\x6a\xf8\x1c\x72\x88\x8e\x7a\xac\xe1\x30\xd9\
-\xda\xda\x2e\xc2\x32\xb0\x9b\xc9\x57\x59\x32\xc3\xb0\xb6\xb6\x5e\
-\x46\x88\xc6\xdf\xdf\xbf\x8f\x3b\x86\x02\x61\x88\x75\xac\x61\xaf\
-\x8e\x1d\x3b\xf6\x2f\xe2\x66\xc8\x88\xe1\x9e\xba\xcc\x30\xe0\xfd\
-\x23\x5e\x86\x9c\x31\xb9\xbe\x70\x8a\x01\x42\x1b\x86\xa9\xa9\xe9\
-\x26\xb6\x75\x91\x23\x26\xe7\x70\xac\x88\x55\x16\x6d\x18\x26\x26\
-\x26\x5b\x08\x56\x26\x25\x25\x35\xca\xbd\x58\x61\xde\x42\x68\xc3\
-\x80\x53\x8c\x20\x25\xb6\x73\x59\x58\xca\x33\x0d\x84\x36\x0c\xa8\
-\xac\xac\x2c\x3f\x3b\x3b\xbb\x8a\x15\x47\x97\x59\x20\x62\x9d\xd8\
-\x3d\x48\x25\x25\x25\x85\x72\x84\xd8\x0f\x05\x42\xfb\x8c\xa1\x3e\
-\x12\xf3\xc4\xee\xcb\x54\x54\x54\x54\x2c\x65\x14\x57\x27\x20\x2c\
-\xc6\xb2\xae\x5c\xb9\xf2\x05\xd9\x93\xa0\xa1\x9a\x9a\x9a\x8c\xcb\
-\x97\x2f\x7f\xe9\xee\xee\x3e\xc6\x1c\x10\x16\x87\x2c\x32\x94\xa0\
-\x72\x1d\x8d\xdf\x47\x0a\xdf\x20\x93\x85\x25\x28\x4c\x4f\xea\x80\
-\x82\xbd\x0e\x6c\xa9\x1a\x0a\x14\xe6\x97\xbd\x24\xd9\xc0\x50\xa0\
-\x28\xc2\x53\x07\x14\x84\x35\x90\xa6\xa3\x76\x28\x8a\xd9\x0f\x21\
-\x09\x6c\x6a\x87\xa2\xa8\xe0\x22\x81\x92\x9b\x9b\x5b\x81\x6c\x43\
-\x35\x42\x51\x5c\xf8\x1d\x50\x30\xd1\x23\x83\x51\x8d\x50\x14\xb9\
-\x41\x85\x4c\x75\x04\x03\xb3\xb2\xb2\xaa\x69\xd4\x4e\x91\x13\x8a\
-\x62\xb7\x70\x01\x05\x07\x6e\x10\x14\x54\x13\x14\x45\x27\x39\x20\
-\x1b\x5e\x6d\x50\x14\x9f\x28\x47\xa0\xc0\x62\x68\x54\x19\x22\x50\
-\x70\x18\xd5\xc5\xc5\x65\x92\x03\x11\x08\x45\xab\x64\x3c\xd2\x84\
-\x02\x4b\xa1\x0d\x45\x15\x40\x20\x1c\x73\xa6\x09\x05\x91\x67\x29\
-\xa0\xa8\x06\xc8\x6e\x28\x29\x29\x29\x0d\x34\xea\x71\x49\x01\x45\
-\xd1\x93\xfa\x7e\x50\x50\xad\x01\x05\x02\x94\x08\x45\x55\x16\x42\
-\x84\xd2\x19\x80\x82\xa4\x05\x1a\x45\xd2\x68\x42\x51\x25\x10\x02\
-\x05\x15\x80\x70\xa4\x5a\x49\x50\x54\x0b\x04\x42\x39\x26\xa5\x41\
-\x51\x35\x90\xdd\x50\x70\xce\x1d\xb5\xb3\x58\x87\xa2\xba\x49\x7d\
-\x3f\x28\x28\x3e\x80\x32\x1d\xac\x43\x51\xbd\x85\x10\xa1\xee\x22\
-\x29\xbc\x89\x7a\x8c\xac\x42\x31\x18\x20\x04\x0a\x0e\xe0\xa0\xca\
-\x10\xab\x50\x0c\x0a\x08\x84\x5a\xbe\x52\x40\x41\xd7\x06\x47\x47\
-\xc7\x19\x0e\x44\x07\x28\x98\x53\x50\x78\x99\x06\x14\x24\xfa\xa1\
-\xbf\x89\xae\x50\x0c\x62\x52\xdf\x0f\x0a\x86\x16\x7c\x9b\x69\x40\
-\x21\x7d\x19\x75\x85\x62\x90\x16\x42\x84\xa2\xfd\x80\x02\x27\x12\
-\xc5\xfc\x59\x80\x62\xd0\x40\x08\x14\x34\xae\x44\xe1\x4d\x16\xa0\
-\x18\x3c\x10\x08\xdd\x79\x58\x81\xc2\x81\xec\x81\x82\xd5\x17\xba\
-\xf6\xc8\x05\xc5\x60\x27\xf5\xfd\xa0\x60\xb9\x0a\xcf\x5e\x2e\x28\
-\xdc\x42\xf6\x08\x1d\xdf\x00\x05\x1f\x1c\x3a\xc1\x49\x0d\x85\x03\
-\xd9\x07\x0a\xea\x06\xa3\x57\xa2\xd4\x50\x38\x90\x7d\x84\x2e\xa2\
-\x72\x40\xe1\x40\x04\x40\xc1\x44\x8f\xee\xa2\x52\x40\xe1\x40\x74\
-\xb0\x14\x29\xa0\x30\x7b\xe8\x93\x25\xa1\x33\x35\xb1\x94\x67\xcf\
-\x9e\xbd\x4e\x03\x0a\x80\x9c\x39\x73\xe6\x07\xc5\x17\x30\x93\x1a\
-\x0a\x96\xc4\x68\x23\x2e\xd6\x75\x61\x0c\xa8\x86\x07\x18\x7c\xc8\
-\xd2\x51\xce\xce\xce\x53\xc4\x4f\x11\x03\x0a\x60\x54\x56\x56\xe6\
-\xec\xae\xa6\xcd\x81\xe8\x09\x05\xc3\xd7\xe0\xe0\xa0\x8f\xbe\xd7\
-\x41\x7d\x95\x97\xd5\x9b\xe7\x40\xf4\x84\x42\x62\x5f\xfa\x40\x41\
-\xe5\xa1\xfd\xda\x64\xf0\xd0\x89\x9e\x72\x70\x70\x98\x05\x14\x84\
-\xee\xfb\xfb\xfb\xfd\x74\x81\x71\x50\x23\x19\x6e\x21\x47\x84\x42\
-\x36\xb9\x84\x40\x41\xed\xfa\xc3\x5a\x2d\x71\x20\x47\x94\x46\xa3\
-\x99\x17\x02\x05\x30\x90\x08\x7e\x58\x33\x32\x0e\x44\x44\x28\xd8\
-\xa3\xef\xed\xed\x0d\xd8\xfb\xff\x38\xa4\x2a\xb4\x33\x1c\x07\x22\
-\x22\x14\x92\xcd\xb2\x1b\x0a\x9a\xd1\xe8\xd2\xd0\x92\x4f\xea\x22\
-\x8a\xf4\xcc\x22\x50\x00\x43\xd7\x96\xaf\xdc\x42\x28\x41\xc1\x41\
-\xd4\x6b\xd7\xae\x7d\xa6\x6b\xff\xdd\xff\x81\x94\x96\x96\x16\xe0\
-\x0f\xff\x38\xc5\x83\x82\xb4\x55\x7d\x5e\xfb\x1f\x03\x08\xc4\xcc\
-\x05\x66\x4b\x88\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-\
-\x00\x00\x00\xd2\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\
+\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\x69\
+\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\x38\
+\x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\
+\x22\x4d\x2d\x38\x33\x38\x2d\x32\x32\x33\x32\x48\x35\x36\x32\x76\
+\x33\x36\x30\x30\x48\x2d\x38\x33\x38\x7a\x22\x20\x66\x69\x6c\x6c\
+\x3d\x22\x6e\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\
+\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x31\x36\x20\x31\x30\x76\x32\
+\x38\x6c\x32\x32\x2d\x31\x34\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\
+\x77\x68\x69\x74\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\
+\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x34\x38\x76\x34\
+\x38\x48\x30\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\
+\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
+\x00\x00\x00\x91\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
 \x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
 \x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x20\x30\x63\
-\x2d\x31\x2e\x31\x20\x30\x2d\x32\x20\x2e\x39\x2d\x32\x20\x32\x68\
-\x31\x63\x30\x2d\x2e\x35\x36\x2e\x34\x34\x2d\x31\x20\x31\x2d\x31\
-\x73\x31\x20\x2e\x34\x34\x20\x31\x20\x31\x76\x32\x68\x2d\x34\x76\
-\x34\x68\x36\x76\x2d\x34\x68\x2d\x31\x76\x2d\x32\x63\x30\x2d\x31\
-\x2e\x31\x2d\x2e\x39\x2d\x32\x2d\x32\x2d\x32\x7a\x22\x20\x74\x72\
-\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\x61\
-\x74\x65\x28\x31\x29\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\
-\x3e\
-\x00\x00\x01\x58\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x34\x20\x30\x6c\
+\x2d\x34\x20\x33\x68\x31\x76\x34\x68\x32\x76\x2d\x32\x68\x32\x76\
+\x32\x68\x32\x76\x2d\x34\x2e\x30\x33\x6c\x31\x20\x2e\x30\x33\x2d\
+\x34\x2d\x33\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
+\
+\x00\x00\x01\x60\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x32\x34\
-\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x34\x22\x20\x76\x69\
-\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x32\x34\x20\x32\x34\
-\x22\x3e\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x31\x31\x20\x31\
-\x38\x68\x32\x76\x2d\x32\x68\x2d\x32\x76\x32\x7a\x6d\x31\x2d\x31\
-\x36\x43\x36\x2e\x34\x38\x20\x32\x20\x32\x20\x36\x2e\x34\x38\x20\
-\x32\x20\x31\x32\x73\x34\x2e\x34\x38\x20\x31\x30\x20\x31\x30\x20\
-\x31\x30\x20\x31\x30\x2d\x34\x2e\x34\x38\x20\x31\x30\x2d\x31\x30\
-\x53\x31\x37\x2e\x35\x32\x20\x32\x20\x31\x32\x20\x32\x7a\x6d\x30\
-\x20\x31\x38\x63\x2d\x34\x2e\x34\x31\x20\x30\x2d\x38\x2d\x33\x2e\
-\x35\x39\x2d\x38\x2d\x38\x73\x33\x2e\x35\x39\x2d\x38\x20\x38\x2d\
-\x38\x20\x38\x20\x33\x2e\x35\x39\x20\x38\x20\x38\x2d\x33\x2e\x35\
-\x39\x20\x38\x2d\x38\x20\x38\x7a\x6d\x30\x2d\x31\x34\x63\x2d\x32\
-\x2e\x32\x31\x20\x30\x2d\x34\x20\x31\x2e\x37\x39\x2d\x34\x20\x34\
-\x68\x32\x63\x30\x2d\x31\x2e\x31\x2e\x39\x2d\x32\x20\x32\x2d\x32\
-\x73\x32\x20\x2e\x39\x20\x32\x20\x32\x63\x30\x20\x32\x2d\x33\x20\
-\x31\x2e\x37\x35\x2d\x33\x20\x35\x68\x32\x63\x30\x2d\x32\x2e\x32\
-\x35\x20\x33\x2d\x32\x2e\x35\x20\x33\x2d\x35\x20\x30\x2d\x32\x2e\
-\x32\x31\x2d\x31\x2e\x37\x39\x2d\x34\x2d\x34\x2d\x34\x7a\x22\x2f\
-\x3e\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x01\x7f\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
-\x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x61\x79\x81\x31\x3d\
-\x41\x97\xbd\xc9\xcb\xcd\xce\x16\x1b\x1d\x81\xa2\xac\x4b\x5e\x64\
-\xad\xd8\xe6\x0a\x0d\x0e\x40\x51\x56\x6f\x8b\x94\x56\x6c\x73\x20\
-\x28\x2b\x8c\xaf\xba\xa2\xca\xd7\x36\xf6\x87\x6c\x00\x00\x01\x0a\
-\x49\x44\x41\x54\x28\xcf\x65\xd1\xa1\x4e\x03\x41\x10\x80\xe1\x3f\
-\x4d\x1a\x72\x6d\x09\x24\x7d\x00\x2c\x8a\x20\x2b\x10\x84\x20\x96\
-\xd4\x9c\xc4\x81\x44\x12\xde\xa0\x15\xed\x94\x10\xee\x24\x0e\x64\
-\x25\xb2\x92\xa0\x2a\x2b\x71\x20\x8b\x43\x22\x99\xd9\x5e\xc2\xec\
-\xf6\xcc\x6e\xbe\xec\x7f\x97\xdb\xe1\x7c\xfb\x21\x88\xc8\xfb\x91\
-\xf8\xc7\x6c\x44\xb1\xce\x6d\x06\x1f\xb9\xbd\x42\x2f\xb7\x15\xb0\
-\x4e\xed\x51\x29\x89\xd5\xee\xcd\x7a\xa9\xfd\x98\xf9\x58\x6d\x3f\
-\xda\x55\x62\x25\xbc\xc1\x8e\xb7\x09\xec\x4e\xf5\xe0\x8d\xb3\x31\
-\x74\xab\xd2\xc7\x84\x63\x78\x96\x6b\x1f\x13\xf4\x5d\x73\x49\x62\
-\x42\x0d\x03\x49\x62\x86\xd0\xd2\xd5\xc7\x9c\xe9\x27\x74\xf5\x31\
-\xa7\x70\xa9\x6b\xb5\xfa\x8f\xb9\x80\xa5\x6d\xbe\x9a\xb8\xba\x3b\
-\x60\x58\xb7\x7f\x6d\xff\xd0\xc4\x63\xda\x84\x93\xfe\xa6\x68\x62\
-\x3d\x1f\x67\x24\x2e\xbe\xf5\xd6\xc4\xa5\xb7\x4d\xac\x37\xd2\x72\
-\x16\x63\xbd\xf4\xae\xb3\x18\xeb\x5c\xf7\x9c\xc5\x58\xe7\x7a\xe8\
-\xcd\xe2\x17\x58\x78\xb3\xb8\xa6\x10\x6f\x71\xf8\x74\x52\xb3\x7f\
-\xd0\x5b\x4a\xcc\x62\x9e\x52\x8b\xf1\x3c\x33\x8b\x17\x99\x69\x5c\
-\x48\x66\x1a\x77\xb6\xec\x9b\x4f\x91\x3f\x5e\x72\x22\x91\xd1\xe5\
-\x86\x70\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x30\x2f\x73\x76\x67\x22\x20\x65\x6e\x61\x62\x6c\x65\x2d\x62\x61\
+\x63\x6b\x67\x72\x6f\x75\x6e\x64\x3d\x22\x6e\x65\x77\x20\x30\x20\
+\x30\x20\x32\x34\x20\x32\x34\x22\x20\x68\x65\x69\x67\x68\x74\x3d\
+\x22\x32\x34\x22\x20\x76\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\
+\x30\x20\x32\x34\x20\x32\x34\x22\x20\x77\x69\x64\x74\x68\x3d\x22\
+\x32\x34\x22\x3e\x3c\x67\x3e\x3c\x72\x65\x63\x74\x20\x66\x69\x6c\
+\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x68\x65\x69\x67\x68\x74\x3d\
+\x22\x32\x34\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x32\x34\x22\x2f\
+\x3e\x3c\x2f\x67\x3e\x3c\x67\x3e\x3c\x67\x3e\x3c\x72\x65\x63\x74\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x22\x20\x77\x69\x64\x74\
+\x68\x3d\x22\x31\x38\x22\x20\x78\x3d\x22\x33\x22\x20\x79\x3d\x22\
+\x32\x22\x2f\x3e\x3c\x72\x65\x63\x74\x20\x68\x65\x69\x67\x68\x74\
+\x3d\x22\x32\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x31\x38\x22\x20\
+\x78\x3d\x22\x33\x22\x20\x79\x3d\x22\x32\x30\x22\x2f\x3e\x3c\x72\
+\x65\x63\x74\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x22\x20\x77\
+\x69\x64\x74\x68\x3d\x22\x31\x38\x22\x20\x78\x3d\x22\x33\x22\x20\
+\x79\x3d\x22\x31\x34\x22\x2f\x3e\x3c\x72\x65\x63\x74\x20\x68\x65\
+\x69\x67\x68\x74\x3d\x22\x32\x22\x20\x77\x69\x64\x74\x68\x3d\x22\
+\x31\x38\x22\x20\x78\x3d\x22\x33\x22\x20\x79\x3d\x22\x38\x22\x2f\
+\x3e\x3c\x2f\x67\x3e\x3c\x2f\x67\x3e\x3c\x2f\x73\x76\x67\x3e\
 \x00\x00\x00\xcb\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
 \x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x00\x00\x00\x20\x20\
 \x20\x30\x30\x30\x40\x40\x40\x44\x51\x55\x60\x60\x60\x70\x70\x70\
 \x65\x7a\x81\x90\x90\x90\x82\xa2\xad\x98\xb1\xb9\xc9\xcb\xcc\xae\
@@ -2292,14 +1406,202 @@
 \x49\x44\x41\x54\x28\xcf\x63\x38\x83\x09\x18\x0e\x0a\x0a\xae\x7b\
 \x87\x0a\x86\x82\x58\xd7\x2a\x30\xd8\x87\x2c\x06\x05\xa2\x58\xc4\
 \x04\xf7\x61\x11\x5b\x87\x4f\xec\x28\x16\xb1\x73\xbb\x20\xb6\x36\
 \x22\x8b\x41\x19\x0b\x07\x4e\x0c\x16\x16\xc8\x62\xb0\xb0\xc0\x22\
 \x26\x88\x57\x6c\x23\x16\xb1\xa7\x58\xc4\xde\x21\xc2\x02\x21\x86\
 \x30\x77\x30\x89\x01\x00\x56\x2a\xff\x13\x4e\x4a\xdd\x86\x00\x00\
 \x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x00\xea\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x2e\x35\x20\
+\x30\x6c\x2d\x31\x2e\x35\x20\x31\x2e\x35\x68\x31\x76\x31\x2e\x35\
+\x68\x2d\x31\x2e\x35\x76\x2d\x31\x6c\x2d\x31\x2e\x35\x20\x31\x2e\
+\x35\x20\x31\x2e\x35\x20\x31\x2e\x35\x76\x2d\x31\x68\x31\x2e\x35\
+\x76\x31\x2e\x35\x68\x2d\x31\x6c\x31\x2e\x35\x20\x31\x2e\x35\x20\
+\x31\x2e\x35\x2d\x31\x2e\x35\x68\x2d\x31\x76\x2d\x31\x2e\x35\x68\
+\x31\x2e\x35\x76\x31\x6c\x31\x2e\x35\x2d\x31\x2e\x35\x2d\x31\x2e\
+\x35\x2d\x31\x2e\x35\x76\x31\x68\x2d\x31\x2e\x35\x76\x2d\x31\x2e\
+\x35\x68\x31\x6c\x2d\x31\x2e\x35\x2d\x31\x2e\x35\x7a\x22\x20\x2f\
+\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x01\x5d\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x26\x00\x00\x00\x26\x04\x03\x00\x00\x00\x5a\x13\xf4\x9d\
+\x00\x00\x00\x30\x50\x4c\x54\x45\x00\x00\x00\x62\x7a\x82\xad\xd8\
+\xe6\x23\x2a\x2c\xaf\xb4\xb6\x4e\x4e\x4e\x89\xa3\xac\x0b\x0e\x0f\
+\xcb\xcd\xce\x92\xb7\xc3\x31\x3d\x42\x78\x8b\x91\xc0\xc0\xc0\x54\
+\x69\x70\x14\x19\x1b\x06\x08\x09\x4b\x93\x60\x3b\x00\x00\x00\xe8\
+\x49\x44\x41\x54\x28\xcf\x63\x38\xd1\xd1\x71\xc4\xa5\x03\x19\xf4\
+\x30\x34\x29\x89\x3f\x60\x7f\x3c\x49\x09\x01\x74\x18\x9a\xb4\x0a\
+\x18\x18\x18\xca\x50\xc5\x16\x00\x85\x18\xd8\x93\x90\xc5\x1a\x41\
+\xca\x18\x18\x1e\x21\x8b\xb5\x83\x85\x18\x78\x91\xc5\xce\x41\xc4\
+\x98\x91\xc5\x1c\x20\x62\x0c\x58\xc4\xf8\x26\x21\x89\xf9\x63\x51\
+\xd7\x07\x11\xe2\x42\x16\x6b\x86\x88\xfd\x46\x16\xeb\x84\xb8\xcf\
+\x08\xc5\x1f\xf9\x68\x4e\x01\x89\xa9\x3d\x60\x60\xe0\x37\x42\x15\
+\x53\xd2\x35\x78\xb0\x5a\x09\x4d\x4c\x49\x09\x39\xa4\x60\x62\x4a\
+\x74\x15\xdb\x7b\x71\x12\xba\xd8\x85\x02\x86\xe2\x49\xa8\x62\xca\
+\x1f\x40\x51\x88\x2a\x66\x00\x8e\xc2\x1c\x64\x31\xdd\x0f\xe0\x20\
+\x7a\x83\x2c\xa6\x00\x09\x4a\x1e\x64\xb1\xed\x10\x31\x6e\x64\xb1\
+\x0b\xd0\xa8\xc1\x22\xc6\x8a\x2c\x26\x00\x8d\x7e\x64\xb1\xe9\x10\
+\x31\x36\x64\x31\x65\x88\x58\x0d\xb2\x98\x26\x38\x0a\xf9\xd7\xa0\
+\xf8\x23\x1d\x24\xf6\x19\xd5\x6f\xa0\x28\x64\x5f\xa4\xc3\x70\x06\
+\x05\x6c\x08\xce\x39\x73\x06\x00\x07\x79\x83\xb6\x91\x0b\xff\x56\
+\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x01\xe7\
+\x3c\
+\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
+\x30\x22\x3f\x3e\x0d\x0a\x3c\x73\x76\x67\x20\x77\x69\x64\x74\x68\
+\x3d\x22\x33\x36\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x33\x36\
+\x22\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\
+\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\x2f\
+\x73\x76\x67\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x73\x76\x67\x3d\x22\
+\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\
+\x67\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\x3e\x0d\x0a\x0d\x0a\
+\x20\x3c\x67\x3e\x0d\x0a\x20\x20\x3c\x74\x69\x74\x6c\x65\x3e\x4c\
+\x61\x79\x65\x72\x20\x31\x3c\x2f\x74\x69\x74\x6c\x65\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x69\x64\x3d\x22\x73\x76\x67\x5f\
+\x31\x22\x20\x64\x3d\x22\x6d\x2d\x30\x2e\x30\x30\x30\x32\x36\x31\
+\x2c\x2d\x30\x2e\x30\x30\x30\x32\x36\x31\x6c\x33\x30\x2e\x32\x35\
+\x30\x30\x30\x32\x2c\x30\x6c\x35\x2e\x37\x35\x2c\x35\x2e\x37\x35\
+\x6c\x30\x2c\x33\x30\x2e\x32\x35\x30\x30\x30\x32\x6c\x2d\x33\x36\
+\x2e\x30\x30\x30\x30\x30\x32\x2c\x30\x6c\x30\x2c\x2d\x33\x36\x2e\
+\x30\x30\x30\x30\x30\x32\x7a\x6d\x33\x32\x2e\x30\x30\x30\x30\x30\
+\x32\x2c\x37\x2e\x32\x35\x6c\x2d\x33\x2e\x32\x35\x2c\x2d\x33\x2e\
+\x32\x35\x6c\x2d\x30\x2e\x37\x35\x2c\x30\x6c\x30\x2c\x31\x33\x2e\
+\x30\x30\x30\x30\x30\x32\x6c\x2d\x32\x30\x2e\x30\x30\x30\x30\x30\
+\x32\x2c\x30\x6c\x30\x2c\x2d\x31\x33\x2e\x30\x30\x30\x30\x30\x32\
+\x6c\x2d\x34\x2c\x30\x6c\x30\x2c\x32\x38\x2e\x30\x30\x30\x30\x30\
+\x32\x6c\x32\x38\x2e\x30\x30\x30\x30\x30\x32\x2c\x30\x6c\x30\x2c\
+\x2d\x32\x34\x2e\x37\x35\x30\x30\x30\x32\x7a\x6d\x2d\x31\x33\x2c\
+\x2d\x33\x2e\x32\x35\x6c\x30\x2c\x31\x30\x6c\x35\x2c\x30\x6c\x30\
+\x2c\x2d\x31\x30\x6c\x2d\x35\x2c\x30\x7a\x22\x20\x73\x74\x72\x6f\
+\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\
+\x6e\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\
+\x3d\x22\x30\x2e\x32\x22\x20\x66\x69\x6c\x6c\x3d\x22\x23\x30\x30\
+\x30\x30\x30\x30\x22\x2f\x3e\x0d\x0a\x20\x3c\x2f\x67\x3e\x0d\x0a\
+\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x02\x13\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x2e\x35\x20\
+\x30\x6c\x2d\x2e\x35\x20\x31\x2e\x31\x39\x63\x2d\x2e\x31\x2e\x30\
+\x33\x2d\x2e\x31\x39\x2e\x30\x38\x2d\x2e\x32\x38\x2e\x31\x33\x6c\
+\x2d\x31\x2e\x31\x39\x2d\x2e\x35\x2d\x2e\x37\x32\x2e\x37\x32\x2e\
+\x35\x20\x31\x2e\x31\x39\x63\x2d\x2e\x30\x35\x2e\x31\x2d\x2e\x30\
+\x39\x2e\x31\x38\x2d\x2e\x31\x33\x2e\x32\x38\x6c\x2d\x31\x2e\x31\
+\x39\x2e\x35\x76\x31\x6c\x31\x2e\x31\x39\x2e\x35\x63\x2e\x30\x34\
+\x2e\x31\x2e\x30\x38\x2e\x31\x38\x2e\x31\x33\x2e\x32\x38\x6c\x2d\
+\x2e\x35\x20\x31\x2e\x31\x39\x2e\x37\x32\x2e\x37\x32\x20\x31\x2e\
+\x31\x39\x2d\x2e\x35\x63\x2e\x30\x39\x2e\x30\x34\x2e\x31\x38\x2e\
+\x30\x39\x2e\x32\x38\x2e\x31\x33\x6c\x2e\x35\x20\x31\x2e\x31\x39\
+\x68\x31\x6c\x2e\x35\x2d\x31\x2e\x31\x39\x63\x2e\x30\x39\x2d\x2e\
+\x30\x34\x2e\x31\x39\x2d\x2e\x30\x38\x2e\x32\x38\x2d\x2e\x31\x33\
+\x6c\x31\x2e\x31\x39\x2e\x35\x2e\x37\x32\x2d\x2e\x37\x32\x2d\x2e\
+\x35\x2d\x31\x2e\x31\x39\x63\x2e\x30\x34\x2d\x2e\x30\x39\x2e\x30\
+\x39\x2d\x2e\x31\x39\x2e\x31\x33\x2d\x2e\x32\x38\x6c\x31\x2e\x31\
+\x39\x2d\x2e\x35\x76\x2d\x31\x6c\x2d\x31\x2e\x31\x39\x2d\x2e\x35\
+\x63\x2d\x2e\x30\x33\x2d\x2e\x30\x39\x2d\x2e\x30\x38\x2d\x2e\x31\
+\x39\x2d\x2e\x31\x33\x2d\x2e\x32\x38\x6c\x2e\x35\x2d\x31\x2e\x31\
+\x39\x2d\x2e\x37\x32\x2d\x2e\x37\x32\x2d\x31\x2e\x31\x39\x2e\x35\
+\x63\x2d\x2e\x30\x39\x2d\x2e\x30\x34\x2d\x2e\x31\x39\x2d\x2e\x30\
+\x39\x2d\x2e\x32\x38\x2d\x2e\x31\x33\x6c\x2d\x2e\x35\x2d\x31\x2e\
+\x31\x39\x68\x2d\x31\x7a\x6d\x2e\x35\x20\x32\x2e\x35\x63\x2e\x38\
+\x33\x20\x30\x20\x31\x2e\x35\x2e\x36\x37\x20\x31\x2e\x35\x20\x31\
+\x2e\x35\x73\x2d\x2e\x36\x37\x20\x31\x2e\x35\x2d\x31\x2e\x35\x20\
+\x31\x2e\x35\x2d\x31\x2e\x35\x2d\x2e\x36\x37\x2d\x31\x2e\x35\x2d\
+\x31\x2e\x35\x2e\x36\x37\x2d\x31\x2e\x35\x20\x31\x2e\x35\x2d\x31\
+\x2e\x35\x7a\x22\x0d\x0a\x20\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\
+\x67\x3e\
+\x00\x00\x00\x91\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x76\
+\x31\x68\x38\x76\x2d\x31\x68\x2d\x38\x7a\x6d\x34\x20\x32\x6c\x2d\
+\x33\x20\x33\x68\x32\x76\x33\x68\x32\x76\x2d\x33\x68\x32\x6c\x2d\
+\x33\x2d\x33\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
+\
+\x00\x00\x03\xf6\
+\xef\
+\xbb\xbf\x3c\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\
+\x22\x31\x2e\x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\
+\x75\x74\x66\x2d\x38\x22\x3f\x3e\x0d\x0a\x3c\x21\x44\x4f\x43\x54\
+\x59\x50\x45\x20\x73\x76\x67\x20\x50\x55\x42\x4c\x49\x43\x20\x22\
+\x2d\x2f\x2f\x57\x33\x43\x2f\x2f\x44\x54\x44\x20\x53\x56\x47\x20\
+\x31\x2e\x31\x2f\x2f\x45\x4e\x22\x20\x22\x68\x74\x74\x70\x3a\x2f\
+\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x47\x72\x61\x70\
+\x68\x69\x63\x73\x2f\x53\x56\x47\x2f\x31\x2e\x31\x2f\x44\x54\x44\
+\x2f\x73\x76\x67\x31\x31\x2e\x64\x74\x64\x22\x3e\x0d\x0a\x3c\x73\
+\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\x2f\
+\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\
+\x2f\x73\x76\x67\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x78\x6c\x69\x6e\
+\x6b\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\
+\x2e\x6f\x72\x67\x2f\x31\x39\x39\x39\x2f\x78\x6c\x69\x6e\x6b\x22\
+\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\x31\x22\x20\x62\
+\x61\x73\x65\x50\x72\x6f\x66\x69\x6c\x65\x3d\x22\x66\x75\x6c\x6c\
+\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x33\x37\x22\x20\x68\x65\x69\
+\x67\x68\x74\x3d\x22\x33\x35\x22\x20\x76\x69\x65\x77\x42\x6f\x78\
+\x3d\x22\x30\x20\x30\x20\x33\x37\x2e\x30\x30\x20\x33\x35\x2e\x30\
+\x30\x22\x20\x65\x6e\x61\x62\x6c\x65\x2d\x62\x61\x63\x6b\x67\x72\
+\x6f\x75\x6e\x64\x3d\x22\x6e\x65\x77\x20\x30\x20\x30\x20\x33\x37\
+\x2e\x30\x30\x20\x33\x35\x2e\x30\x30\x22\x20\x78\x6d\x6c\x3a\x73\
+\x70\x61\x63\x65\x3d\x22\x70\x72\x65\x73\x65\x72\x76\x65\x22\x3e\
+\x0d\x0a\x09\x3c\x70\x61\x74\x68\x20\x66\x69\x6c\x6c\x3d\x22\x23\
+\x30\x30\x30\x30\x30\x30\x22\x20\x66\x69\x6c\x6c\x2d\x6f\x70\x61\
+\x63\x69\x74\x79\x3d\x22\x31\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
+\x77\x69\x64\x74\x68\x3d\x22\x30\x2e\x32\x22\x20\x73\x74\x72\x6f\
+\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\
+\x6e\x64\x22\x20\x64\x3d\x22\x4d\x20\x33\x37\x2e\x39\x31\x36\x37\
+\x2c\x31\x35\x2e\x38\x33\x33\x33\x43\x20\x34\x30\x2e\x31\x30\x32\
+\x38\x2c\x31\x35\x2e\x38\x33\x33\x33\x20\x34\x32\x2e\x32\x35\x2c\
+\x31\x37\x2e\x38\x31\x33\x39\x20\x34\x32\x2e\x32\x35\x2c\x32\x30\
+\x4c\x20\x34\x32\x2c\x32\x31\x4c\x20\x35\x34\x2c\x32\x31\x4c\x20\
+\x35\x34\x2c\x35\x37\x4c\x20\x32\x32\x2c\x35\x37\x4c\x20\x32\x32\
+\x2c\x32\x31\x4c\x20\x33\x34\x2c\x32\x31\x4c\x20\x33\x33\x2e\x37\
+\x35\x2c\x32\x30\x43\x20\x33\x33\x2e\x37\x35\x2c\x31\x37\x2e\x38\
+\x31\x33\x39\x20\x33\x35\x2e\x37\x33\x30\x35\x2c\x31\x35\x2e\x38\
+\x33\x33\x33\x20\x33\x37\x2e\x39\x31\x36\x37\x2c\x31\x35\x2e\x38\
+\x33\x33\x33\x20\x5a\x20\x4d\x20\x35\x31\x2c\x32\x34\x4c\x20\x34\
+\x35\x2e\x35\x2c\x32\x34\x4c\x20\x34\x37\x2e\x35\x2c\x32\x38\x4c\
+\x20\x32\x38\x2e\x35\x2c\x32\x38\x4c\x20\x33\x30\x2e\x35\x2c\x32\
+\x34\x4c\x20\x32\x35\x2c\x32\x34\x4c\x20\x32\x35\x2c\x35\x34\x4c\
+\x20\x35\x31\x2c\x35\x34\x4c\x20\x35\x31\x2c\x32\x34\x20\x5a\x20\
+\x4d\x20\x33\x37\x2e\x39\x31\x36\x36\x2c\x31\x38\x2e\x32\x30\x38\
+\x34\x43\x20\x33\x37\x2e\x30\x34\x32\x32\x2c\x31\x38\x2e\x32\x30\
+\x38\x34\x20\x33\x36\x2c\x31\x38\x2e\x38\x37\x35\x36\x20\x33\x36\
+\x2c\x31\x39\x2e\x37\x35\x43\x20\x33\x36\x2c\x32\x30\x2e\x30\x33\
+\x38\x34\x20\x33\x36\x2e\x33\x36\x35\x33\x2c\x32\x30\x2e\x37\x36\
+\x37\x31\x20\x33\x36\x2e\x35\x2c\x32\x31\x4c\x20\x33\x39\x2e\x35\
+\x2c\x32\x31\x43\x20\x33\x39\x2e\x36\x33\x34\x37\x2c\x32\x30\x2e\
+\x37\x36\x37\x31\x20\x34\x30\x2c\x32\x30\x2e\x30\x33\x38\x34\x20\
+\x34\x30\x2c\x31\x39\x2e\x37\x35\x43\x20\x34\x30\x2c\x31\x38\x2e\
+\x38\x37\x35\x36\x20\x33\x38\x2e\x37\x39\x31\x31\x2c\x31\x38\x2e\
+\x32\x30\x38\x34\x20\x33\x37\x2e\x39\x31\x36\x36\x2c\x31\x38\x2e\
+\x32\x30\x38\x34\x20\x5a\x20\x0d\x0a\x4d\x20\x31\x34\x2e\x35\x35\
+\x2c\x34\x30\x4c\x20\x33\x32\x2e\x35\x2c\x34\x30\x4c\x20\x32\x35\
+\x2e\x35\x2c\x33\x35\x4c\x20\x33\x32\x2e\x35\x2c\x33\x35\x4c\x20\
+\x33\x39\x2e\x35\x2c\x34\x32\x4c\x20\x33\x32\x2e\x35\x2c\x34\x39\
+\x4c\x20\x32\x35\x2e\x35\x2c\x34\x39\x4c\x20\x33\x32\x2e\x35\x2c\
+\x34\x34\x4c\x20\x31\x34\x2e\x35\x35\x2c\x34\x34\x4c\x20\x31\x34\
+\x2e\x35\x35\x2c\x34\x30\x20\x5a\x22\x0d\x0a\x74\x72\x61\x6e\x73\
+\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\x61\x74\x65\x28\
+\x2d\x31\x32\x20\x2d\x31\x37\x29\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\
+\x76\x67\x3e\x0d\x0a\
 \x00\x00\x01\x65\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x33\x34\
 \x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x31\x30\x22\x20\x76\x69\
 \x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x33\x34\x20\x31\x30\
@@ -2317,128 +1619,78 @@
 \x2f\x3e\x0d\x0a\x20\x3c\x72\x65\x63\x74\x20\x78\x3d\x22\x32\x35\
 \x22\x20\x79\x3d\x22\x31\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\
 \x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x66\x69\x6c\
 \x6c\x3d\x22\x67\x72\x65\x79\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\
 \x22\x72\x65\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\
 \x74\x68\x3d\x22\x32\x22\x20\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\
 \x67\x3e\x0d\x0a\
-\x00\x00\x00\xe1\
+\x00\x00\x01\x37\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\
-\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\x69\
-\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\x38\
-\x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\
-\x22\x4d\x2d\x38\x33\x38\x2d\x32\x32\x33\x32\x48\x35\x36\x32\x76\
-\x33\x36\x30\x30\x48\x2d\x38\x33\x38\x7a\x22\x20\x66\x69\x6c\x6c\
-\x3d\x22\x6e\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\
-\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x31\x36\x20\x31\x30\x76\x32\
-\x38\x6c\x32\x32\x2d\x31\x34\x7a\x22\x2f\x3e\x0d\x0a\x20\x20\x20\
-\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x34\
-\x38\x76\x34\x38\x48\x30\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\
-\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
-\
-\x00\x00\x00\x85\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x26\x00\x00\x00\x26\x08\x06\x00\x00\x00\xa8\x3d\xe9\xae\
-\x00\x00\x00\x4c\x49\x44\x41\x54\x78\xda\xed\xce\xb1\x0d\x80\x20\
-\x10\x00\x40\x0a\x16\x70\x12\x12\xe6\xb7\x74\x13\x7a\xb4\x24\x9f\
-\x68\x58\xe3\x63\xee\x26\xb8\x1a\xef\x77\x3c\x2b\x5a\x49\xa6\xde\
-\x2b\xfa\x35\xe6\x99\x2e\x56\x92\x12\x13\x13\x13\x13\x13\x13\x13\
-\x13\x13\x13\x13\x13\x13\x13\x13\x13\x13\x13\x13\xfb\x41\x6c\x03\
-\x7d\x7d\x0d\x14\x97\xb2\x1c\x95\x00\x00\x00\x00\x49\x45\x4e\x44\
-\xae\x42\x60\x82\
-\x00\x00\x05\x3d\
+\x30\x2f\x73\x76\x67\x22\x20\x65\x6e\x61\x62\x6c\x65\x2d\x62\x61\
+\x63\x6b\x67\x72\x6f\x75\x6e\x64\x3d\x22\x6e\x65\x77\x20\x30\x20\
+\x30\x20\x32\x34\x20\x32\x34\x22\x20\x68\x65\x69\x67\x68\x74\x3d\
+\x22\x32\x34\x22\x20\x76\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\
+\x30\x20\x32\x34\x20\x32\x34\x22\x20\x77\x69\x64\x74\x68\x3d\x22\
+\x32\x34\x22\x3e\x3c\x67\x3e\x3c\x72\x65\x63\x74\x20\x66\x69\x6c\
+\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x68\x65\x69\x67\x68\x74\x3d\
+\x22\x32\x34\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x32\x34\x22\x2f\
+\x3e\x3c\x2f\x67\x3e\x3c\x67\x3e\x3c\x67\x3e\x3c\x72\x65\x63\x74\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x22\x20\x77\x69\x64\x74\
+\x68\x3d\x22\x31\x38\x22\x20\x78\x3d\x22\x33\x22\x20\x79\x3d\x22\
+\x33\x22\x2f\x3e\x3c\x72\x65\x63\x74\x20\x68\x65\x69\x67\x68\x74\
+\x3d\x22\x32\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x31\x38\x22\x20\
+\x78\x3d\x22\x33\x22\x20\x79\x3d\x22\x31\x39\x22\x2f\x3e\x3c\x72\
+\x65\x63\x74\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x22\x20\x77\
+\x69\x64\x74\x68\x3d\x22\x31\x38\x22\x20\x78\x3d\x22\x33\x22\x20\
+\x79\x3d\x22\x31\x31\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\x2f\x67\x3e\
+\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x01\x03\
 \x3c\
-\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
-\x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\x55\x54\x46\
-\x2d\x38\x22\x3f\x3e\x0d\x0a\x3c\x21\x44\x4f\x43\x54\x59\x50\x45\
-\x20\x73\x76\x67\x20\x20\x50\x55\x42\x4c\x49\x43\x20\x27\x2d\x2f\
-\x2f\x57\x33\x43\x2f\x2f\x44\x54\x44\x20\x53\x56\x47\x20\x31\x2e\
-\x31\x2f\x2f\x45\x4e\x27\x20\x20\x27\x68\x74\x74\x70\x3a\x2f\x2f\
-\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x47\x72\x61\x70\x68\
-\x69\x63\x73\x2f\x53\x56\x47\x2f\x31\x2e\x31\x2f\x44\x54\x44\x2f\
-\x73\x76\x67\x31\x31\x2e\x64\x74\x64\x27\x3e\x0d\x0a\x3c\x73\x76\
-\x67\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x2e\x34\x37\x6d\x6d\x22\
-\x20\x66\x69\x6c\x6c\x2d\x72\x75\x6c\x65\x3d\x22\x65\x76\x65\x6e\
-\x6f\x64\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\
-\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x73\x74\x72\
-\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x38\x2e\x32\x32\
-\x32\x22\x20\x70\x72\x65\x73\x65\x72\x76\x65\x41\x73\x70\x65\x63\
-\x74\x52\x61\x74\x69\x6f\x3d\x22\x78\x4d\x69\x64\x59\x4d\x69\x64\
-\x22\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\x32\x22\x20\
-\x76\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x34\x37\
-\x20\x38\x34\x37\x22\x20\x78\x6d\x6c\x3a\x73\x70\x61\x63\x65\x3d\
-\x22\x70\x72\x65\x73\x65\x72\x76\x65\x22\x20\x78\x6d\x6c\x6e\x73\
-\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\
-\x6f\x72\x67\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\x20\x78\x6d\
-\x6c\x6e\x73\x3a\x6f\x6f\x6f\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\
-\x78\x6d\x6c\x2e\x6f\x70\x65\x6e\x6f\x66\x66\x69\x63\x65\x2e\x6f\
-\x72\x67\x2f\x73\x76\x67\x2f\x65\x78\x70\x6f\x72\x74\x22\x3e\x0d\
-\x0a\x20\x3c\x64\x65\x66\x73\x20\x63\x6c\x61\x73\x73\x3d\x22\x43\
-\x6c\x69\x70\x50\x61\x74\x68\x47\x72\x6f\x75\x70\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x63\x6c\x69\x70\x50\x61\x74\x68\x20\x69\x64\x3d\x22\
-\x61\x22\x3e\x0d\x0a\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x77\x69\
-\x64\x74\x68\x3d\x22\x38\x34\x37\x22\x20\x68\x65\x69\x67\x68\x74\
-\x3d\x22\x38\x34\x37\x22\x2f\x3e\x0d\x0a\x20\x20\x3c\x2f\x63\x6c\
-\x69\x70\x50\x61\x74\x68\x3e\x0d\x0a\x20\x20\x0d\x0a\x20\x3c\x2f\
-\x64\x65\x66\x73\x3e\x0d\x0a\x20\x3c\x64\x65\x66\x73\x20\x63\x6c\
-\x61\x73\x73\x3d\x22\x54\x65\x78\x74\x53\x68\x61\x70\x65\x49\x6e\
-\x64\x65\x78\x22\x3e\x0d\x0a\x20\x20\x0d\x0a\x20\x3c\x2f\x64\x65\
-\x66\x73\x3e\x0d\x0a\x20\x3c\x64\x65\x66\x73\x20\x63\x6c\x61\x73\
-\x73\x3d\x22\x45\x6d\x62\x65\x64\x64\x65\x64\x42\x75\x6c\x6c\x65\
-\x74\x43\x68\x61\x72\x73\x22\x3e\x0d\x0a\x20\x20\x0d\x0a\x20\x20\
-\x0d\x0a\x20\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x20\
-\x0d\x0a\x20\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x20\
-\x0d\x0a\x20\x3c\x2f\x64\x65\x66\x73\x3e\x0d\x0a\x20\x0d\x0a\x20\
-\x0d\x0a\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x4d\x61\
-\x73\x74\x65\x72\x5f\x53\x6c\x69\x64\x65\x22\x3e\x0d\x0a\x20\x20\
-\x20\x0d\x0a\x20\x20\x20\x0d\x0a\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\
-\x20\x0d\x0a\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x53\x6c\
-\x69\x64\x65\x47\x72\x6f\x75\x70\x22\x3e\x0d\x0a\x20\x20\x0d\x0a\
-\x20\x20\x20\x0d\x0a\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\
-\x73\x3d\x22\x53\x6c\x69\x64\x65\x22\x20\x63\x6c\x69\x70\x2d\x70\
-\x61\x74\x68\x3d\x22\x75\x72\x6c\x28\x23\x61\x29\x22\x3e\x0d\x0a\
-\x20\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x50\
-\x61\x67\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x67\x20\
-\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\
-\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x43\x75\x73\x74\
-\x6f\x6d\x53\x68\x61\x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\
-\x20\x20\x3c\x67\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\
-\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\
-\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\
-\x42\x6f\x78\x22\x20\x78\x3d\x22\x34\x36\x22\x20\x79\x3d\x22\x34\
-\x36\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x37\x35\x35\x22\x20\x68\
-\x65\x69\x67\x68\x74\x3d\x22\x37\x35\x34\x22\x2f\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\
-\x6d\x34\x32\x33\x20\x37\x36\x30\x68\x2d\x33\x33\x38\x76\x2d\x36\
-\x37\x35\x68\x36\x37\x36\x76\x36\x37\x35\x68\x2d\x33\x33\x38\x7a\
-\x22\x20\x73\x74\x72\x6f\x6b\x65\x3d\x22\x23\x30\x30\x30\x22\x20\
-\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x63\x61\x70\x3d\x22\
-\x73\x71\x75\x61\x72\x65\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\
-\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x6d\x69\x74\x65\x72\x22\x20\
-\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x37\x38\
-\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\
-\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\
-\x20\x20\x20\x20\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\
-\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\
-\x6e\x67\x2e\x50\x6f\x6c\x79\x50\x6f\x6c\x79\x67\x6f\x6e\x53\x68\
-\x61\x70\x65\x22\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\x20\x0d\x0a\
-\x20\x20\x20\x20\x20\x20\x20\x20\x3c\x72\x65\x63\x74\x20\x63\x6c\
-\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\
-\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x34\x39\x22\x20\x68\x65\
-\x69\x67\x68\x74\x3d\x22\x38\x34\x39\x22\x20\x66\x69\x6c\x6c\x3d\
-\x22\x6e\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x20\x20\
-\x20\x0d\x0a\x20\x20\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\
-\x20\x20\x20\x20\x3c\x2f\x67\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x2f\
-\x67\x3e\x0d\x0a\x20\x20\x20\x0d\x0a\x20\x20\x0d\x0a\x20\x3c\x2f\
-\x67\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x20\x30\x63\
+\x2d\x31\x2e\x36\x36\x20\x30\x2d\x33\x20\x31\x2e\x33\x34\x2d\x33\
+\x20\x33\x20\x30\x20\x32\x20\x33\x20\x35\x20\x33\x20\x35\x73\x33\
+\x2d\x33\x20\x33\x2d\x35\x63\x30\x2d\x31\x2e\x36\x36\x2d\x31\x2e\
+\x33\x34\x2d\x33\x2d\x33\x2d\x33\x7a\x6d\x30\x20\x31\x63\x31\x2e\
+\x31\x31\x20\x30\x20\x32\x20\x2e\x39\x20\x32\x20\x32\x20\x30\x20\
+\x31\x2e\x31\x31\x2d\x2e\x38\x39\x20\x32\x2d\x32\x20\x32\x2d\x31\
+\x2e\x31\x20\x30\x2d\x32\x2d\x2e\x38\x39\x2d\x32\x2d\x32\x20\x30\
+\x2d\x31\x2e\x31\x2e\x39\x2d\x32\x20\x32\x2d\x32\x7a\x22\x20\x74\
+\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\x61\x6e\x73\x6c\
+\x61\x74\x65\x28\x31\x29\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\
+\x67\x3e\
+\x00\x00\x01\x50\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x20\x30\x63\
+\x2d\x2e\x35\x35\x20\x30\x2d\x31\x20\x2e\x34\x35\x2d\x31\x20\x31\
+\x68\x2d\x31\x63\x2d\x2e\x35\x35\x20\x30\x2d\x31\x20\x2e\x34\x35\
+\x2d\x31\x20\x31\x68\x37\x63\x30\x2d\x2e\x35\x35\x2d\x2e\x34\x35\
+\x2d\x31\x2d\x31\x2d\x31\x68\x2d\x31\x63\x30\x2d\x2e\x35\x35\x2d\
+\x2e\x34\x35\x2d\x31\x2d\x31\x2d\x31\x68\x2d\x31\x7a\x6d\x2d\x32\
+\x20\x33\x76\x34\x2e\x38\x31\x63\x30\x20\x2e\x31\x31\x2e\x30\x38\
+\x2e\x31\x39\x2e\x31\x39\x2e\x31\x39\x68\x34\x2e\x36\x33\x63\x2e\
+\x31\x31\x20\x30\x20\x2e\x31\x39\x2d\x2e\x30\x38\x2e\x31\x39\x2d\
+\x2e\x31\x39\x76\x2d\x34\x2e\x38\x31\x68\x2d\x31\x76\x33\x2e\x35\
+\x63\x30\x20\x2e\x32\x38\x2d\x2e\x32\x32\x2e\x35\x2d\x2e\x35\x2e\
+\x35\x73\x2d\x2e\x35\x2d\x2e\x32\x32\x2d\x2e\x35\x2d\x2e\x35\x76\
+\x2d\x33\x2e\x35\x68\x2d\x31\x76\x33\x2e\x35\x63\x30\x20\x2e\x32\
+\x38\x2d\x2e\x32\x32\x2e\x35\x2d\x2e\x35\x2e\x35\x73\x2d\x2e\x35\
+\x2d\x2e\x32\x32\x2d\x2e\x35\x2d\x2e\x35\x76\x2d\x33\x2e\x35\x68\
+\x2d\x31\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
 \x00\x00\x00\xf9\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
 \x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
 \x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
@@ -2449,116 +1701,42 @@
 \x2e\x35\x73\x32\x2e\x35\x20\x31\x2e\x31\x32\x20\x32\x2e\x35\x20\
 \x32\x2e\x35\x76\x2e\x35\x68\x2d\x31\x6c\x32\x20\x32\x20\x32\x2d\
 \x32\x68\x2d\x31\x76\x2d\x2e\x35\x63\x30\x2d\x31\x2e\x39\x33\x2d\
 \x31\x2e\x35\x37\x2d\x33\x2e\x35\x2d\x33\x2e\x35\x2d\x33\x2e\x35\
 \x7a\x22\x20\x74\x72\x61\x6e\x73\x66\x6f\x72\x6d\x3d\x22\x74\x72\
 \x61\x6e\x73\x6c\x61\x74\x65\x28\x30\x20\x31\x29\x22\x20\x2f\x3e\
 \x0d\x0a\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x02\xa4\
-\x3c\
-\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
-\x30\x22\x3f\x3e\x0d\x0a\x3c\x73\x76\x67\x20\x77\x69\x64\x74\x68\
-\x3d\x22\x33\x38\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x33\x35\
-\x22\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\
-\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\x2f\
-\x73\x76\x67\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x73\x76\x67\x3d\x22\
-\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\
-\x67\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\x3e\x0d\x0a\x0d\x0a\
-\x20\x3c\x67\x3e\x0d\x0a\x20\x20\x3c\x74\x69\x74\x6c\x65\x3e\x4c\
-\x61\x79\x65\x72\x20\x31\x3c\x2f\x74\x69\x74\x6c\x65\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x69\x64\x3d\x22\x73\x76\x67\x5f\
-\x31\x22\x20\x64\x3d\x22\x6d\x31\x32\x2e\x38\x38\x36\x2c\x33\x32\
-\x2e\x34\x32\x31\x36\x6c\x33\x2e\x35\x33\x35\x36\x30\x31\x2c\x2d\
-\x33\x2e\x35\x33\x35\x35\x6c\x2d\x33\x2e\x35\x33\x35\x36\x30\x31\
-\x2c\x2d\x33\x2e\x35\x33\x35\x36\x30\x33\x6c\x32\x2e\x35\x37\x38\
-\x35\x30\x31\x2c\x2d\x32\x2e\x35\x37\x38\x34\x6c\x33\x2e\x35\x33\
-\x35\x35\x2c\x33\x2e\x35\x33\x35\x35\x6c\x33\x2e\x35\x33\x35\x35\
-\x2c\x2d\x33\x2e\x35\x33\x35\x35\x6c\x32\x2e\x35\x37\x38\x34\x2c\
-\x32\x2e\x35\x37\x38\x34\x6c\x2d\x33\x2e\x35\x33\x35\x35\x2c\x33\
-\x2e\x35\x33\x35\x35\x30\x33\x6c\x33\x2e\x35\x33\x35\x35\x39\x39\
-\x2c\x33\x2e\x35\x33\x35\x35\x39\x39\x6c\x2d\x32\x2e\x35\x37\x38\
-\x34\x39\x39\x2c\x32\x2e\x35\x37\x38\x34\x6c\x2d\x33\x2e\x35\x33\
-\x35\x35\x2c\x2d\x33\x2e\x35\x33\x35\x35\x6c\x2d\x33\x2e\x35\x33\
-\x35\x35\x2c\x33\x2e\x35\x33\x35\x35\x6c\x2d\x32\x2e\x35\x37\x38\
-\x35\x30\x31\x2c\x2d\x32\x2e\x35\x37\x38\x34\x7a\x6d\x2d\x31\x32\
-\x2e\x38\x38\x36\x2c\x2d\x33\x32\x2e\x36\x37\x31\x36\x6c\x38\x2c\
-\x30\x6c\x30\x2c\x38\x6c\x2d\x38\x2c\x30\x6c\x30\x2c\x2d\x38\x7a\
-\x6d\x31\x31\x2e\x39\x39\x39\x39\x30\x31\x2c\x30\x2e\x30\x30\x30\
-\x32\x39\x39\x6c\x32\x35\x2e\x39\x39\x39\x37\x39\x38\x2c\x30\x6c\
-\x30\x2c\x38\x6c\x2d\x32\x35\x2e\x39\x39\x39\x37\x39\x38\x2c\x30\
-\x6c\x30\x2c\x2d\x38\x7a\x6d\x2d\x31\x31\x2e\x39\x39\x39\x39\x30\
-\x31\x2c\x31\x30\x2e\x39\x39\x39\x37\x30\x31\x6c\x38\x2c\x30\x6c\
-\x30\x2c\x38\x6c\x2d\x38\x2c\x30\x6c\x30\x2c\x2d\x38\x7a\x6d\x31\
-\x2c\x31\x6c\x30\x2c\x36\x6c\x36\x2c\x30\x6c\x30\x2c\x2d\x36\x6c\
-\x2d\x36\x2c\x30\x7a\x6d\x31\x2c\x31\x6c\x34\x2c\x30\x6c\x30\x2c\
-\x34\x6c\x2d\x34\x2c\x30\x6c\x30\x2c\x2d\x34\x7a\x6d\x31\x30\x2c\
-\x2d\x32\x6c\x32\x36\x2c\x30\x6c\x30\x2c\x38\x6c\x2d\x32\x36\x2c\
-\x30\x6c\x30\x2c\x2d\x38\x7a\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\
-\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\
-\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x30\
-\x2e\x32\x22\x20\x66\x69\x6c\x6c\x3d\x22\x23\x30\x30\x30\x30\x30\
-\x30\x22\x2f\x3e\x0d\x0a\x20\x3c\x2f\x67\x3e\x0d\x0a\x3c\x2f\x73\
-\x76\x67\x3e\
-\x00\x00\x01\xe7\
-\x3c\
-\x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
-\x30\x22\x3f\x3e\x0d\x0a\x3c\x73\x76\x67\x20\x77\x69\x64\x74\x68\
-\x3d\x22\x33\x36\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x33\x36\
-\x22\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\
-\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\x30\x2f\
-\x73\x76\x67\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x73\x76\x67\x3d\x22\
-\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\
-\x67\x2f\x32\x30\x30\x30\x2f\x73\x76\x67\x22\x3e\x0d\x0a\x0d\x0a\
-\x20\x3c\x67\x3e\x0d\x0a\x20\x20\x3c\x74\x69\x74\x6c\x65\x3e\x4c\
-\x61\x79\x65\x72\x20\x31\x3c\x2f\x74\x69\x74\x6c\x65\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x69\x64\x3d\x22\x73\x76\x67\x5f\
-\x31\x22\x20\x64\x3d\x22\x6d\x2d\x30\x2e\x30\x30\x30\x32\x36\x31\
-\x2c\x2d\x30\x2e\x30\x30\x30\x32\x36\x31\x6c\x33\x30\x2e\x32\x35\
-\x30\x30\x30\x32\x2c\x30\x6c\x35\x2e\x37\x35\x2c\x35\x2e\x37\x35\
-\x6c\x30\x2c\x33\x30\x2e\x32\x35\x30\x30\x30\x32\x6c\x2d\x33\x36\
-\x2e\x30\x30\x30\x30\x30\x32\x2c\x30\x6c\x30\x2c\x2d\x33\x36\x2e\
-\x30\x30\x30\x30\x30\x32\x7a\x6d\x33\x32\x2e\x30\x30\x30\x30\x30\
-\x32\x2c\x37\x2e\x32\x35\x6c\x2d\x33\x2e\x32\x35\x2c\x2d\x33\x2e\
-\x32\x35\x6c\x2d\x30\x2e\x37\x35\x2c\x30\x6c\x30\x2c\x31\x33\x2e\
-\x30\x30\x30\x30\x30\x32\x6c\x2d\x32\x30\x2e\x30\x30\x30\x30\x30\
-\x32\x2c\x30\x6c\x30\x2c\x2d\x31\x33\x2e\x30\x30\x30\x30\x30\x32\
-\x6c\x2d\x34\x2c\x30\x6c\x30\x2c\x32\x38\x2e\x30\x30\x30\x30\x30\
-\x32\x6c\x32\x38\x2e\x30\x30\x30\x30\x30\x32\x2c\x30\x6c\x30\x2c\
-\x2d\x32\x34\x2e\x37\x35\x30\x30\x30\x32\x7a\x6d\x2d\x31\x33\x2c\
-\x2d\x33\x2e\x32\x35\x6c\x30\x2c\x31\x30\x6c\x35\x2c\x30\x6c\x30\
-\x2c\x2d\x31\x30\x6c\x2d\x35\x2c\x30\x7a\x22\x20\x73\x74\x72\x6f\
-\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\x69\x6e\x3d\x22\x72\x6f\x75\
-\x6e\x64\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\
-\x3d\x22\x30\x2e\x32\x22\x20\x66\x69\x6c\x6c\x3d\x22\x23\x30\x30\
-\x30\x30\x30\x30\x22\x2f\x3e\x0d\x0a\x20\x3c\x2f\x67\x3e\x0d\x0a\
-\x3c\x2f\x73\x76\x67\x3e\
-\x00\x00\x01\x55\
+\x00\x00\x00\x85\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x26\x00\x00\x00\x26\x08\x06\x00\x00\x00\xa8\x3d\xe9\xae\
+\x00\x00\x00\x4c\x49\x44\x41\x54\x78\xda\xed\xce\xb1\x0d\x80\x20\
+\x10\x00\x40\x0a\x16\x70\x12\x12\xe6\xb7\x74\x13\x7a\xb4\x24\x9f\
+\x68\x58\xe3\x63\xee\x26\xb8\x1a\xef\x77\x3c\x2b\x5a\x49\xa6\xde\
+\x2b\xfa\x35\xe6\x99\x2e\x56\x92\x12\x13\x13\x13\x13\x13\x13\x13\
+\x13\x13\x13\x13\x13\x13\x13\x13\x13\x13\x13\x13\xfb\x41\x6c\x03\
+\x7d\x7d\x0d\x14\x97\xb2\x1c\x95\x00\x00\x00\x00\x49\x45\x4e\x44\
+\xae\x42\x60\x82\
+\x00\x00\x00\xe1\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
-\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
-\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
-\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
-\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x2e\x35\x20\
-\x30\x63\x2d\x2e\x32\x38\x20\x30\x2d\x2e\x35\x2e\x32\x32\x2d\x2e\
-\x35\x2e\x35\x76\x2e\x35\x68\x2d\x2e\x37\x35\x63\x2d\x2e\x31\x34\
-\x20\x30\x2d\x2e\x32\x35\x2e\x31\x31\x2d\x2e\x32\x35\x2e\x32\x35\
-\x76\x2e\x37\x35\x68\x33\x76\x2d\x2e\x37\x35\x63\x30\x2d\x2e\x31\
-\x34\x2d\x2e\x31\x31\x2d\x2e\x32\x35\x2d\x2e\x32\x35\x2d\x2e\x32\
-\x35\x68\x2d\x2e\x37\x35\x76\x2d\x2e\x35\x63\x30\x2d\x2e\x32\x38\
-\x2d\x2e\x32\x32\x2d\x2e\x35\x2d\x2e\x35\x2d\x2e\x35\x7a\x6d\x2d\
-\x33\x2e\x32\x35\x20\x31\x63\x2d\x2e\x31\x34\x20\x30\x2d\x2e\x32\
-\x35\x2e\x31\x31\x2d\x2e\x32\x35\x2e\x32\x35\x76\x36\x2e\x35\x63\
-\x30\x20\x2e\x31\x34\x2e\x31\x31\x2e\x32\x35\x2e\x32\x35\x2e\x32\
-\x35\x68\x36\x2e\x35\x63\x2e\x31\x34\x20\x30\x20\x2e\x32\x35\x2d\
-\x2e\x31\x31\x2e\x32\x35\x2d\x2e\x32\x35\x76\x2d\x36\x2e\x35\x63\
-\x30\x2d\x2e\x31\x34\x2d\x2e\x31\x31\x2d\x2e\x32\x35\x2d\x2e\x32\
-\x35\x2d\x2e\x32\x35\x68\x2d\x2e\x37\x35\x76\x32\x68\x2d\x35\x76\
-\x2d\x32\x68\x2d\x2e\x37\x35\x7a\x22\x20\x2f\x3e\x0d\x0a\x3c\x2f\
-\x73\x76\x67\x3e\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\
+\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\x69\
+\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\x38\
+\x22\x3e\x0d\x0a\x20\x20\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\
+\x22\x4d\x2d\x38\x33\x38\x2d\x32\x32\x33\x32\x48\x35\x36\x32\x76\
+\x33\x36\x30\x30\x48\x2d\x38\x33\x38\x7a\x22\x20\x66\x69\x6c\x6c\
+\x3d\x22\x6e\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\
+\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x31\x36\x20\x31\x30\x76\x32\
+\x38\x6c\x32\x32\x2d\x31\x34\x7a\x22\x2f\x3e\x0d\x0a\x20\x20\x20\
+\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x34\
+\x38\x76\x34\x38\x48\x30\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\
+\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
+\
 \x00\x00\x00\xe1\
 \x3c\
 \x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
 \x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
 \x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x34\x38\
 \x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x34\x38\x22\x20\x76\x69\
 \x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x34\x38\x20\x34\x38\
@@ -2568,385 +1746,484 @@
 \x3d\x22\x6e\x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x20\x20\x20\x20\x3c\
 \x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x31\x36\x20\x31\x30\x76\x32\
 \x38\x6c\x32\x32\x2d\x31\x34\x7a\x22\x2f\x3e\x0d\x0a\x20\x20\x20\
 \x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x34\
 \x38\x76\x34\x38\x48\x30\x7a\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\
 \x6f\x6e\x65\x22\x2f\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
 \
+\x00\x00\x01\x0d\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x65\x6e\x61\x62\x6c\x65\x2d\x62\x61\
+\x63\x6b\x67\x72\x6f\x75\x6e\x64\x3d\x22\x6e\x65\x77\x20\x30\x20\
+\x30\x20\x32\x34\x20\x32\x34\x22\x20\x68\x65\x69\x67\x68\x74\x3d\
+\x22\x32\x34\x22\x20\x76\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\
+\x30\x20\x32\x34\x20\x32\x34\x22\x20\x77\x69\x64\x74\x68\x3d\x22\
+\x32\x34\x22\x3e\x3c\x67\x3e\x3c\x72\x65\x63\x74\x20\x66\x69\x6c\
+\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x68\x65\x69\x67\x68\x74\x3d\
+\x22\x32\x34\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x32\x34\x22\x2f\
+\x3e\x3c\x2f\x67\x3e\x3c\x67\x3e\x3c\x67\x3e\x3c\x72\x65\x63\x74\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x32\x22\x20\x77\x69\x64\x74\
+\x68\x3d\x22\x31\x38\x22\x20\x78\x3d\x22\x33\x22\x20\x79\x3d\x22\
+\x33\x22\x2f\x3e\x3c\x72\x65\x63\x74\x20\x68\x65\x69\x67\x68\x74\
+\x3d\x22\x32\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x31\x38\x22\x20\
+\x78\x3d\x22\x33\x22\x20\x79\x3d\x22\x31\x39\x22\x2f\x3e\x3c\x2f\
+\x67\x3e\x3c\x2f\x67\x3e\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x03\x6a\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\
+\x31\x2e\x32\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x2e\x34\x37\
+\x6d\x6d\x22\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x2e\x34\x37\
+\x6d\x6d\x22\x20\x76\x69\x65\x77\x42\x6f\x78\x3d\x22\x30\x20\x30\
+\x20\x38\x34\x37\x20\x38\x34\x37\x22\x20\x70\x72\x65\x73\x65\x72\
+\x76\x65\x41\x73\x70\x65\x63\x74\x52\x61\x74\x69\x6f\x3d\x22\x78\
+\x4d\x69\x64\x59\x4d\x69\x64\x22\x20\x66\x69\x6c\x6c\x2d\x72\x75\
+\x6c\x65\x3d\x22\x65\x76\x65\x6e\x6f\x64\x64\x22\x20\x73\x74\x72\
+\x6f\x6b\x65\x2d\x77\x69\x64\x74\x68\x3d\x22\x32\x38\x2e\x32\x32\
+\x32\x22\x20\x73\x74\x72\x6f\x6b\x65\x2d\x6c\x69\x6e\x65\x6a\x6f\
+\x69\x6e\x3d\x22\x72\x6f\x75\x6e\x64\x22\x20\x78\x6d\x6c\x3a\x73\
+\x70\x61\x63\x65\x3d\x22\x70\x72\x65\x73\x65\x72\x76\x65\x22\x3e\
+\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\
+\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x50\
+\x6f\x6c\x79\x50\x6f\x6c\x79\x67\x6f\x6e\x53\x68\x61\x70\x65\x22\
+\x3e\x3c\x70\x61\x74\x68\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\
+\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x66\x69\x6c\x6c\x3d\
+\x22\x6e\x6f\x6e\x65\x22\x20\x64\x3d\x22\x4d\x30\x20\x30\x68\x38\
+\x34\x39\x76\x38\x34\x39\x48\x30\x7a\x22\x2f\x3e\x3c\x2f\x67\x3e\
+\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x47\x72\x6f\x75\x70\x22\
+\x3e\x3c\x67\x20\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\
+\x75\x6e\x2e\x73\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\
+\x50\x6f\x6c\x79\x50\x6f\x6c\x79\x67\x6f\x6e\x53\x68\x61\x70\x65\
+\x22\x3e\x3c\x70\x61\x74\x68\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\
+\x6f\x75\x6e\x64\x69\x6e\x67\x42\x6f\x78\x22\x20\x66\x69\x6c\x6c\
+\x3d\x22\x6e\x6f\x6e\x65\x22\x20\x64\x3d\x22\x4d\x31\x33\x37\x20\
+\x31\x38\x37\x68\x31\x36\x31\x76\x34\x38\x37\x48\x31\x33\x37\x7a\
+\x22\x2f\x3e\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x31\x33\x37\
+\x20\x36\x37\x33\x56\x31\x38\x37\x68\x31\x35\x39\x76\x39\x32\x48\
+\x31\x39\x31\x76\x31\x31\x38\x68\x39\x39\x76\x39\x31\x68\x2d\x39\
+\x39\x76\x31\x38\x35\x7a\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\x67\x20\
+\x63\x6c\x61\x73\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\
+\x74\x61\x72\x2e\x64\x72\x61\x77\x69\x6e\x67\x2e\x50\x6f\x6c\x79\
+\x50\x6f\x6c\x79\x67\x6f\x6e\x53\x68\x61\x70\x65\x22\x3e\x3c\x70\
+\x61\x74\x68\x20\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\
+\x69\x6e\x67\x42\x6f\x78\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\
+\x6e\x65\x22\x20\x64\x3d\x22\x4d\x33\x33\x37\x20\x31\x38\x37\x68\
+\x31\x36\x32\x76\x34\x38\x37\x48\x33\x33\x37\x7a\x22\x2f\x3e\x3c\
+\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x33\x33\x38\x20\x36\x37\x33\
+\x56\x31\x38\x37\x68\x31\x35\x39\x76\x39\x32\x48\x33\x39\x32\x76\
+\x31\x31\x38\x68\x39\x39\x76\x39\x31\x68\x2d\x39\x39\x76\x31\x38\
+\x35\x7a\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\x67\x20\x63\x6c\x61\x73\
+\x73\x3d\x22\x63\x6f\x6d\x2e\x73\x75\x6e\x2e\x73\x74\x61\x72\x2e\
+\x64\x72\x61\x77\x69\x6e\x67\x2e\x50\x6f\x6c\x79\x50\x6f\x6c\x79\
+\x67\x6f\x6e\x53\x68\x61\x70\x65\x22\x3e\x3c\x70\x61\x74\x68\x20\
+\x63\x6c\x61\x73\x73\x3d\x22\x42\x6f\x75\x6e\x64\x69\x6e\x67\x42\
+\x6f\x78\x22\x20\x66\x69\x6c\x6c\x3d\x22\x6e\x6f\x6e\x65\x22\x20\
+\x64\x3d\x22\x4d\x35\x32\x34\x20\x31\x38\x37\x68\x31\x38\x37\x76\
+\x34\x38\x37\x48\x35\x32\x34\x7a\x22\x2f\x3e\x3c\x70\x61\x74\x68\
+\x20\x64\x3d\x22\x4d\x35\x39\x30\x20\x36\x37\x33\x56\x32\x37\x39\
+\x68\x2d\x36\x36\x76\x2d\x39\x32\x68\x31\x38\x35\x76\x39\x32\x68\
+\x2d\x36\x36\x76\x33\x39\x34\x7a\x22\x2f\x3e\x3c\x2f\x67\x3e\x3c\
+\x2f\x67\x3e\x3c\x2f\x73\x76\x67\x3e\
+\x00\x00\x00\xd7\
+\x3c\
+\x73\x76\x67\x20\x78\x6d\x6c\x6e\x73\x3d\x22\x68\x74\x74\x70\x3a\
+\x2f\x2f\x77\x77\x77\x2e\x77\x33\x2e\x6f\x72\x67\x2f\x32\x30\x30\
+\x30\x2f\x73\x76\x67\x22\x20\x77\x69\x64\x74\x68\x3d\x22\x38\x22\
+\x20\x68\x65\x69\x67\x68\x74\x3d\x22\x38\x22\x20\x76\x69\x65\x77\
+\x42\x6f\x78\x3d\x22\x30\x20\x30\x20\x38\x20\x38\x22\x3e\x0d\x0a\
+\x20\x20\x3c\x70\x61\x74\x68\x20\x64\x3d\x22\x4d\x34\x20\x30\x63\
+\x2d\x32\x2e\x32\x31\x20\x30\x2d\x34\x20\x31\x2e\x37\x39\x2d\x34\
+\x20\x34\x73\x31\x2e\x37\x39\x20\x34\x20\x34\x20\x34\x20\x34\x2d\
+\x31\x2e\x37\x39\x20\x34\x2d\x34\x2d\x31\x2e\x37\x39\x2d\x34\x2d\
+\x34\x2d\x34\x7a\x6d\x32\x20\x31\x2e\x37\x38\x6c\x2e\x37\x32\x2e\
+\x37\x32\x2d\x33\x2e\x32\x32\x20\x33\x2e\x32\x32\x2d\x31\x2e\x37\
+\x32\x2d\x31\x2e\x37\x32\x2e\x37\x32\x2d\x2e\x37\x32\x20\x31\x20\
+\x31\x20\x32\x2e\x35\x2d\x32\x2e\x35\x7a\x22\x20\x2f\x3e\x0d\x0a\
+\x3c\x2f\x73\x76\x67\x3e\
 "
 
 qt_resource_name = b"\
-\x00\x0b\
-\x0b\x87\x43\xe7\
-\x00\x70\
-\x00\x61\x00\x75\x00\x73\x00\x65\x00\x5f\x00\x77\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x0f\
-\x06\xde\xab\xe7\
+\x02\x7e\xfc\x67\
+\x00\x6c\
+\x00\x6f\x00\x63\x00\x6b\x00\x2d\x00\x6c\x00\x6f\x00\x63\x00\x6b\x00\x65\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0d\
+\x05\x5b\x10\xe7\
 \x00\x67\
-\x00\x72\x00\x69\x00\x64\x00\x5f\x00\x63\x00\x6f\x00\x61\x00\x72\x00\x73\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x72\x00\x69\x00\x64\x00\x5f\x00\x66\x00\x69\x00\x6e\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x08\
+\x00\x28\x57\x67\
+\x00\x66\
+\x00\x69\x00\x6c\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x0c\
 \x0e\x13\x51\xa7\
 \x00\x71\
 \x00\x75\x00\x61\x00\x6e\x00\x74\x00\x69\x00\x7a\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x13\
-\x01\xe2\xd4\x62\
+\x00\x0b\
+\x0b\x87\x43\xe7\
 \x00\x70\
-\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x73\x00\x74\x00\x65\x00\x6d\x00\x2d\x00\x6d\
-\x00\x6b\x00\x72\
+\x00\x61\x00\x75\x00\x73\x00\x65\x00\x5f\x00\x77\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x12\
-\x07\x82\x05\x27\
-\x00\x66\
-\x00\x72\x00\x6f\x00\x6d\x00\x5f\x00\x63\x00\x6c\x00\x69\x00\x70\x00\x62\x00\x6f\x00\x61\x00\x72\x00\x64\x00\x2e\x00\x73\x00\x76\
-\x00\x67\
-\x00\x10\
-\x0c\xf9\x5d\x07\
-\x00\x74\
-\x00\x6f\x00\x5f\x00\x63\x00\x6c\x00\x69\x00\x70\x00\x62\x00\x6f\x00\x61\x00\x72\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0b\
-\x01\x31\x8d\xc7\
+\x03\xe3\x0f\x47\
 \x00\x73\
-\x00\x70\x00\x65\x00\x61\x00\x6b\x00\x65\x00\x72\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0e\
-\x0a\x4c\x78\x27\
-\x00\x63\
-\x00\x61\x00\x6d\x00\x65\x00\x72\x00\x61\x00\x2d\x00\x73\x00\x6c\x00\x72\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x6f\x00\x72\x00\x74\x00\x2d\x00\x61\x00\x73\x00\x63\x00\x65\x00\x6e\x00\x64\x00\x69\x00\x6e\x00\x67\x00\x2e\x00\x73\x00\x76\
+\x00\x67\
 \x00\x13\
 \x07\x1a\xa5\x62\
 \x00\x70\
 \x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x6c\x00\x69\x00\x6e\x00\x65\x00\x2d\x00\x6d\
 \x00\x6b\x00\x72\
-\x00\x0e\
-\x0f\x3b\xb2\x47\
-\x00\x65\
-\x00\x6c\x00\x6c\x00\x69\x00\x70\x00\x73\x00\x65\x00\x73\x00\x5f\x00\x68\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0d\
+\x0b\x5b\x17\xc7\
+\x00\x67\
+\x00\x72\x00\x69\x00\x64\x00\x5f\x00\x6e\x00\x6f\x00\x6e\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x13\
+\x01\xe2\xd4\x62\
+\x00\x70\
+\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x73\x00\x74\x00\x65\x00\x6d\x00\x2d\x00\x6d\
+\x00\x6b\x00\x72\
+\x00\x14\
+\x0d\x09\x76\xa7\
+\x00\x66\
+\x00\x75\x00\x6c\x00\x6c\x00\x73\x00\x63\x00\x72\x00\x65\x00\x65\x00\x6e\x00\x2d\x00\x65\x00\x6e\x00\x74\x00\x65\x00\x72\x00\x2e\
+\x00\x73\x00\x76\x00\x67\
 \x00\x0c\
 \x08\x1a\x90\xa7\
 \x00\x64\
 \x00\x6f\x00\x77\x00\x6e\x00\x6c\x00\x6f\x00\x61\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x11\
+\x09\x70\x56\x07\
+\x00\x6c\
+\x00\x6f\x00\x63\x00\x6b\x00\x2d\x00\x75\x00\x6e\x00\x6c\x00\x6f\x00\x63\x00\x6b\x00\x65\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
+\
+\x00\x0b\
+\x01\x31\x8d\xc7\
+\x00\x73\
+\x00\x70\x00\x65\x00\x61\x00\x6b\x00\x65\x00\x72\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x14\
 \x04\xac\xdf\x27\
 \x00\x72\
 \x00\x6f\x00\x77\x00\x5f\x00\x69\x00\x6e\x00\x73\x00\x65\x00\x72\x00\x74\x00\x5f\x00\x61\x00\x62\x00\x6f\x00\x76\x00\x65\x00\x2e\
 \x00\x73\x00\x76\x00\x67\
-\x00\x08\
-\x06\xc8\x54\x47\
-\x00\x6d\
-\x00\x6f\x00\x76\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x14\
-\x09\x9f\x48\x02\
-\x00\x70\
-\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x73\x00\x74\x00\x65\x00\x70\x00\x73\x00\x2d\
-\x00\x6d\x00\x6b\x00\x72\
-\x00\x12\
-\x03\xe3\x0f\x47\
-\x00\x73\
-\x00\x6f\x00\x72\x00\x74\x00\x2d\x00\x61\x00\x73\x00\x63\x00\x65\x00\x6e\x00\x64\x00\x69\x00\x6e\x00\x67\x00\x2e\x00\x73\x00\x76\
-\x00\x67\
-\x00\x08\
-\x00\x28\x57\x67\
-\x00\x66\
-\x00\x69\x00\x6c\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0d\
-\x05\x5b\x10\xe7\
+\x00\x0f\
+\x06\xde\xab\xe7\
 \x00\x67\
-\x00\x72\x00\x69\x00\x64\x00\x5f\x00\x66\x00\x69\x00\x6e\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x72\x00\x69\x00\x64\x00\x5f\x00\x63\x00\x6f\x00\x61\x00\x72\x00\x73\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x0c\
-\x0b\xdf\x2c\xc7\
-\x00\x73\
-\x00\x65\x00\x74\x00\x74\x00\x69\x00\x6e\x00\x67\x00\x73\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x0f\x12\x57\x07\
+\x00\x67\
+\x00\x72\x00\x61\x00\x70\x00\x68\x00\x5f\x00\x39\x00\x30\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x0e\
-\x09\xf5\xac\xc7\
-\x00\x70\
-\x00\x79\x00\x66\x00\x64\x00\x61\x00\x5f\x00\x69\x00\x63\x00\x6f\x00\x6e\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x09\
-\x08\x9b\xad\xc7\
-\x00\x74\
-\x00\x72\x00\x61\x00\x73\x00\x68\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x01\x0f\x14\xc7\
+\x00\x72\
+\x00\x6f\x00\x77\x00\x5f\x00\x64\x00\x65\x00\x6c\x00\x65\x00\x74\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x14\
+\x0f\xa5\xe0\xc7\
+\x00\x6d\
+\x00\x61\x00\x67\x00\x6e\x00\x69\x00\x66\x00\x79\x00\x69\x00\x6e\x00\x67\x00\x2d\x00\x67\x00\x6c\x00\x61\x00\x73\x00\x73\x00\x2e\
+\x00\x73\x00\x76\x00\x67\
 \x00\x0f\
 \x0f\x48\x21\xfd\
 \x00\x70\
 \x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x73\x00\x74\x00\x65\x00\x6d\
-\x00\x0e\
-\x01\xad\x37\x07\
-\x00\x6d\
-\x00\x61\x00\x70\x00\x2d\x00\x6d\x00\x61\x00\x72\x00\x6b\x00\x65\x00\x72\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x0c\
 \x0d\x0a\x4e\x87\
 \x00\x63\
 \x00\x69\x00\x72\x00\x63\x00\x6c\x00\x65\x00\x2d\x00\x78\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x10\
-\x0f\xc8\xab\x27\
+\x00\x0d\
+\x0c\xe7\x89\xc7\
 \x00\x63\
-\x00\x69\x00\x72\x00\x63\x00\x6c\x00\x65\x00\x2d\x00\x63\x00\x68\x00\x65\x00\x63\x00\x6b\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x6c\x00\x69\x00\x70\x00\x62\x00\x6f\x00\x61\x00\x72\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x14\
+\x09\x9f\x48\x02\
+\x00\x70\
+\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x73\x00\x74\x00\x65\x00\x70\x00\x73\x00\x2d\
+\x00\x6d\x00\x6b\x00\x72\
 \x00\x0e\
-\x0a\xf5\x0c\x82\
+\x09\xf5\xac\xc7\
 \x00\x70\
-\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x6d\x00\x6b\x00\x72\
+\x00\x79\x00\x66\x00\x64\x00\x61\x00\x5f\x00\x69\x00\x63\x00\x6f\x00\x6e\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0f\
+\x0f\x50\xa7\x05\
+\x00\x70\
+\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x6c\x00\x69\x00\x6e\x00\x65\
+\x00\x12\
+\x07\x82\x05\x27\
+\x00\x66\
+\x00\x72\x00\x6f\x00\x6d\x00\x5f\x00\x63\x00\x6c\x00\x69\x00\x70\x00\x62\x00\x6f\x00\x61\x00\x72\x00\x64\x00\x2e\x00\x73\x00\x76\
+\x00\x67\
+\x00\x08\
+\x0c\x33\x57\x07\
+\x00\x68\
+\x00\x65\x00\x6c\x00\x70\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x0f\
 \x02\xbf\xe2\xe7\
 \x00\x61\
 \x00\x63\x00\x74\x00\x69\x00\x6f\x00\x6e\x00\x2d\x00\x75\x00\x6e\x00\x64\x00\x6f\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0a\
-\x05\x78\xd4\xa7\
-\x00\x75\
-\x00\x70\x00\x6c\x00\x6f\x00\x61\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x14\
-\x0d\x09\x76\xa7\
-\x00\x66\
-\x00\x75\x00\x6c\x00\x6c\x00\x73\x00\x63\x00\x72\x00\x65\x00\x65\x00\x6e\x00\x2d\x00\x65\x00\x6e\x00\x74\x00\x65\x00\x72\x00\x2e\
-\x00\x73\x00\x76\x00\x67\
-\x00\x0a\
-\x0f\x68\xbf\xc7\
-\x00\x70\
-\x00\x6c\x00\x61\x00\x79\x00\x5f\x00\x77\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0b\
-\x00\x97\x2b\xe7\
-\x00\x68\
-\x00\x65\x00\x61\x00\x72\x00\x69\x00\x6e\x00\x67\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0e\
-\x0f\xb3\x7c\x47\
-\x00\x73\
-\x00\x70\x00\x65\x00\x61\x00\x6b\x00\x65\x00\x72\x00\x5f\x00\x39\x00\x30\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x09\
 \x0c\x9b\x89\xe7\
 \x00\x62\
 \x00\x72\x00\x75\x00\x73\x00\x68\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0e\
+\x0f\x3b\xb2\x47\
+\x00\x65\
+\x00\x6c\x00\x6c\x00\x69\x00\x70\x00\x73\x00\x65\x00\x73\x00\x5f\x00\x68\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0e\
+\x0f\xb3\x7c\x47\
+\x00\x73\
+\x00\x70\x00\x65\x00\x61\x00\x6b\x00\x65\x00\x72\x00\x5f\x00\x39\x00\x30\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0a\
+\x0f\x68\xbf\xc7\
+\x00\x70\
+\x00\x6c\x00\x61\x00\x79\x00\x5f\x00\x77\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x08\
 \x06\x38\x57\x27\
 \x00\x68\
 \x00\x6f\x00\x6d\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x07\
-\x0c\xd7\x5a\x07\
-\x00\x66\
-\x00\x66\x00\x74\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x14\
-\x0f\xa5\xe0\xc7\
-\x00\x6d\
-\x00\x61\x00\x67\x00\x6e\x00\x69\x00\x66\x00\x79\x00\x69\x00\x6e\x00\x67\x00\x2d\x00\x67\x00\x6c\x00\x61\x00\x73\x00\x73\x00\x2e\
-\x00\x73\x00\x76\x00\x67\
-\x00\x0f\
-\x02\x7e\xfc\x67\
-\x00\x6c\
-\x00\x6f\x00\x63\x00\x6b\x00\x2d\x00\x6c\x00\x6f\x00\x63\x00\x6b\x00\x65\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0c\
-\x0f\x12\x5a\x87\
-\x00\x67\
-\x00\x72\x00\x61\x00\x70\x00\x68\x00\x5f\x00\x39\x00\x30\x00\x2e\x00\x70\x00\x6e\x00\x67\
-\x00\x11\
-\x09\x70\x56\x07\
-\x00\x6c\
-\x00\x6f\x00\x63\x00\x6b\x00\x2d\x00\x75\x00\x6e\x00\x6c\x00\x6f\x00\x63\x00\x6b\x00\x65\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
-\
-\x00\x08\
-\x0c\x33\x57\x07\
-\x00\x68\
-\x00\x65\x00\x6c\x00\x70\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0f\
-\x0f\x50\xa7\x05\
-\x00\x70\
-\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x6c\x00\x69\x00\x6e\x00\x65\
+\x00\x10\
+\x06\x03\x5b\x87\
+\x00\x75\
+\x00\x69\x00\x5f\x00\x6c\x00\x65\x00\x76\x00\x65\x00\x6c\x00\x5f\x00\x6d\x00\x61\x00\x78\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x10\
 \x04\x82\x19\x93\
 \x00\x70\
 \x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x73\x00\x74\x00\x65\x00\x70\x00\x73\
+\x00\x08\
+\x06\xc8\x54\x47\
+\x00\x6d\
+\x00\x6f\x00\x76\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0e\
+\x0a\xf5\x0c\x82\
+\x00\x70\
+\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x6d\x00\x6b\x00\x72\
+\x00\x08\
+\x08\xc8\x55\xe7\
+\x00\x73\
+\x00\x61\x00\x76\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0c\
+\x0b\xdf\x2c\xc7\
+\x00\x73\
+\x00\x65\x00\x74\x00\x74\x00\x69\x00\x6e\x00\x67\x00\x73\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0a\
+\x05\x78\xd4\xa7\
+\x00\x75\
+\x00\x70\x00\x6c\x00\x6f\x00\x61\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x10\
+\x0c\xf9\x5d\x07\
+\x00\x74\
+\x00\x6f\x00\x5f\x00\x63\x00\x6c\x00\x69\x00\x70\x00\x62\x00\x6f\x00\x61\x00\x72\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x0e\
 \x0f\x09\xb2\x47\
 \x00\x65\
 \x00\x6c\x00\x6c\x00\x69\x00\x70\x00\x73\x00\x65\x00\x73\x00\x5f\x00\x76\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x08\
-\x0b\x63\x55\x87\
-\x00\x73\
-\x00\x74\x00\x6f\x00\x70\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0f\
-\x0f\x50\xe1\x05\
-\x00\x70\
-\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x6e\x00\x6f\x00\x6e\x00\x65\
-\x00\x0d\
-\x0b\x5b\x17\xc7\
-\x00\x67\
-\x00\x72\x00\x69\x00\x64\x00\x5f\x00\x6e\x00\x6f\x00\x6e\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x10\
+\x06\x7f\x5b\x87\
+\x00\x75\
+\x00\x69\x00\x5f\x00\x6c\x00\x65\x00\x76\x00\x65\x00\x6c\x00\x5f\x00\x6d\x00\x69\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0e\
+\x01\xad\x37\x07\
+\x00\x6d\
+\x00\x61\x00\x70\x00\x2d\x00\x6d\x00\x61\x00\x72\x00\x6b\x00\x65\x00\x72\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x09\
+\x08\x9b\xad\xc7\
+\x00\x74\
+\x00\x72\x00\x61\x00\x73\x00\x68\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x0f\
 \x0d\xbf\xed\x67\
 \x00\x61\
 \x00\x63\x00\x74\x00\x69\x00\x6f\x00\x6e\x00\x2d\x00\x72\x00\x65\x00\x64\x00\x6f\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0e\
-\x01\x0f\x14\xc7\
-\x00\x72\
-\x00\x6f\x00\x77\x00\x5f\x00\x64\x00\x65\x00\x6c\x00\x65\x00\x74\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x08\
-\x08\xc8\x55\xe7\
-\x00\x73\
-\x00\x61\x00\x76\x00\x65\x00\x2e\x00\x73\x00\x76\x00\x67\
-\x00\x0d\
-\x0c\xe7\x89\xc7\
-\x00\x63\
-\x00\x6c\x00\x69\x00\x70\x00\x62\x00\x6f\x00\x61\x00\x72\x00\x64\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x0f\
+\x0f\x50\xe1\x05\
+\x00\x70\
+\x00\x6c\x00\x6f\x00\x74\x00\x5f\x00\x73\x00\x74\x00\x79\x00\x6c\x00\x65\x00\x2d\x00\x6e\x00\x6f\x00\x6e\x00\x65\
 \x00\x08\
 \x02\x8c\x54\x27\
 \x00\x70\
 \x00\x6c\x00\x61\x00\x79\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x08\
+\x0b\x63\x55\x87\
+\x00\x73\
+\x00\x74\x00\x6f\x00\x70\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x10\
+\x06\x89\x5b\x87\
+\x00\x75\
+\x00\x69\x00\x5f\x00\x6c\x00\x65\x00\x76\x00\x65\x00\x6c\x00\x5f\x00\x6d\x00\x69\x00\x6e\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x07\
+\x0c\xd7\x5a\x07\
+\x00\x66\
+\x00\x66\x00\x74\x00\x2e\x00\x73\x00\x76\x00\x67\
+\x00\x10\
+\x0f\xc8\xab\x27\
+\x00\x63\
+\x00\x69\x00\x72\x00\x63\x00\x6c\x00\x65\x00\x2d\x00\x63\x00\x68\x00\x65\x00\x63\x00\x6b\x00\x2e\x00\x73\x00\x76\x00\x67\
 "
 
 qt_resource_struct_v1 = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x32\x00\x00\x00\x01\
-\x00\x00\x02\x20\x00\x00\x00\x00\x00\x01\x00\x00\x24\x6e\
-\x00\x00\x03\xe0\x00\x00\x00\x00\x00\x01\x00\x00\x51\x05\
-\x00\x00\x05\xf8\x00\x00\x00\x00\x00\x01\x00\x00\x92\x25\
-\x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x17\x08\
-\x00\x00\x02\xd2\x00\x00\x00\x00\x00\x01\x00\x00\x49\x68\
-\x00\x00\x00\x5e\x00\x00\x00\x00\x00\x01\x00\x00\x0d\xa5\
-\x00\x00\x04\x8e\x00\x00\x00\x00\x00\x01\x00\x00\x7b\x60\
-\x00\x00\x06\x50\x00\x00\x00\x00\x00\x01\x00\x00\x98\x11\
-\x00\x00\x03\x5a\x00\x00\x00\x00\x00\x01\x00\x00\x4d\xb7\
-\x00\x00\x01\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x23\xb6\
-\x00\x00\x05\x32\x00\x00\x00\x00\x00\x01\x00\x00\x88\x41\
-\x00\x00\x01\x84\x00\x00\x00\x00\x00\x01\x00\x00\x1e\x73\
-\x00\x00\x02\x36\x00\x01\x00\x00\x00\x01\x00\x00\x24\xfd\
-\x00\x00\x03\x7e\x00\x00\x00\x00\x00\x01\x00\x00\x4e\xb4\
-\x00\x00\x04\x36\x00\x00\x00\x00\x00\x01\x00\x00\x5c\xfe\
-\x00\x00\x01\xb2\x00\x00\x00\x00\x00\x01\x00\x00\x21\x80\
-\x00\x00\x00\x1c\x00\x00\x00\x00\x00\x01\x00\x00\x00\xcf\
-\x00\x00\x01\x18\x00\x00\x00\x00\x00\x01\x00\x00\x1a\x69\
-\x00\x00\x00\x8a\x00\x00\x00\x00\x00\x01\x00\x00\x0f\x14\
-\x00\x00\x01\x66\x00\x00\x00\x00\x00\x01\x00\x00\x1d\xdc\
-\x00\x00\x02\x96\x00\x00\x00\x00\x00\x01\x00\x00\x47\x5c\
-\x00\x00\x06\x1a\x00\x00\x00\x00\x00\x01\x00\x00\x94\xcd\
-\x00\x00\x04\xd0\x00\x00\x00\x00\x00\x01\x00\x00\x84\x8c\
-\x00\x00\x01\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x22\x6e\
-\x00\x00\x02\x74\x00\x00\x00\x00\x00\x01\x00\x00\x2b\x01\
-\x00\x00\x00\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x18\x6e\
-\x00\x00\x03\x38\x00\x00\x00\x00\x00\x01\x00\x00\x4c\x56\
-\x00\x00\x05\xb4\x00\x00\x00\x00\x00\x01\x00\x00\x8b\xe7\
-\x00\x00\x05\x7a\x00\x00\x00\x00\x00\x01\x00\x00\x8a\x79\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x33\x00\x00\x00\x01\
+\x00\x00\x00\x44\x00\x00\x00\x00\x00\x01\x00\x00\x03\x68\
+\x00\x00\x02\x36\x00\x00\x00\x00\x00\x01\x00\x00\x1c\x10\
+\x00\x00\x01\xaa\x00\x00\x00\x00\x00\x01\x00\x00\x11\x0d\
+\x00\x00\x05\x8c\x00\x00\x00\x00\x00\x01\x00\x00\x60\x39\
+\x00\x00\x01\x0a\x00\x00\x00\x00\x00\x01\x00\x00\x0d\x67\
 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x02\x56\x00\x00\x00\x00\x00\x01\x00\x00\x28\xea\
-\x00\x00\x04\xf8\x00\x00\x00\x00\x00\x01\x00\x00\x85\x62\
-\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x5b\x4d\
-\x00\x00\x04\x4c\x00\x00\x00\x00\x00\x01\x00\x00\x5d\x93\
-\x00\x00\x06\x30\x00\x00\x00\x00\x00\x01\x00\x00\x96\xb8\
-\x00\x00\x00\xb4\x00\x00\x00\x00\x00\x01\x00\x00\x13\x0e\
-\x00\x00\x03\x98\x00\x00\x00\x00\x00\x01\x00\x00\x4f\x49\
-\x00\x00\x02\xf4\x00\x00\x00\x00\x00\x01\x00\x00\x4a\x6f\
-\x00\x00\x05\xd4\x00\x00\x00\x00\x00\x01\x00\x00\x91\x28\
-\x00\x00\x00\x40\x00\x00\x00\x00\x00\x01\x00\x00\x0a\x55\
-\x00\x00\x05\x58\x00\x00\x00\x00\x00\x01\x00\x00\x89\x10\
-\x00\x00\x04\xb2\x00\x00\x00\x00\x00\x01\x00\x00\x7c\x47\
-\x00\x00\x01\x44\x00\x00\x00\x00\x00\x01\x00\x00\x1c\x11\
-\x00\x00\x02\xae\x00\x00\x00\x00\x00\x01\x00\x00\x48\xb0\
-\x00\x00\x05\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x86\xbe\
-\x00\x00\x05\x90\x00\x00\x00\x00\x00\x01\x00\x00\x8b\x5e\
-\x00\x00\x03\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x50\x13\
-\x00\x00\x04\x60\x00\x00\x00\x00\x00\x01\x00\x00\x79\x97\
-\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00\x53\xe3\
-\x00\x00\x03\x12\x00\x00\x00\x00\x00\x01\x00\x00\x4b\x7b\
+\x00\x00\x06\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x64\x1a\
+\x00\x00\x03\x9c\x00\x00\x00\x00\x00\x01\x00\x00\x48\xed\
+\x00\x00\x00\x94\x00\x00\x00\x00\x00\x01\x00\x00\x08\x16\
+\x00\x00\x04\x72\x00\x00\x00\x00\x00\x01\x00\x00\x51\xe6\
+\x00\x00\x01\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x12\x73\
+\x00\x00\x00\x24\x00\x01\x00\x00\x00\x01\x00\x00\x00\xe7\
+\x00\x00\x05\x04\x00\x00\x00\x00\x00\x01\x00\x00\x59\x06\
+\x00\x00\x04\x4c\x00\x00\x00\x00\x00\x01\x00\x00\x50\x82\
+\x00\x00\x04\x36\x00\x00\x00\x00\x00\x01\x00\x00\x4f\xed\
+\x00\x00\x05\x66\x00\x00\x00\x00\x00\x01\x00\x00\x5e\xfe\
+\x00\x00\x06\x3a\x00\x00\x00\x00\x00\x01\x00\x00\x65\xe4\
+\x00\x00\x04\x98\x00\x00\x00\x00\x00\x01\x00\x00\x52\xb5\
+\x00\x00\x01\xf4\x00\x00\x00\x00\x00\x01\x00\x00\x15\x80\
+\x00\x00\x00\xbe\x00\x00\x00\x00\x00\x01\x00\x00\x08\xce\
+\x00\x00\x03\x5c\x00\x00\x00\x00\x00\x01\x00\x00\x43\x7e\
+\x00\x00\x01\x64\x00\x00\x00\x00\x00\x01\x00\x00\x0f\xa0\
+\x00\x00\x05\xae\x00\x00\x00\x00\x00\x01\x00\x00\x61\x40\
+\x00\x00\x04\xd0\x00\x00\x00\x00\x00\x01\x00\x00\x55\x04\
+\x00\x00\x01\x82\x00\x00\x00\x00\x00\x01\x00\x00\x10\x37\
+\x00\x00\x02\xe8\x00\x00\x00\x00\x00\x01\x00\x00\x23\x9e\
+\x00\x00\x03\x16\x00\x00\x00\x00\x00\x01\x00\x00\x24\xe6\
+\x00\x00\x04\xae\x00\x00\x00\x00\x00\x01\x00\x00\x53\xa3\
+\x00\x00\x00\xea\x00\x00\x00\x00\x00\x01\x00\x00\x0a\x76\
+\x00\x00\x06\x24\x00\x00\x00\x00\x00\x01\x00\x00\x64\xff\
+\x00\x00\x00\x78\x00\x00\x00\x00\x00\x01\x00\x00\x07\x47\
+\x00\x00\x04\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x56\xef\
+\x00\x00\x03\x86\x00\x00\x00\x00\x00\x01\x00\x00\x47\x78\
+\x00\x00\x03\xc0\x00\x00\x00\x00\x00\x01\x00\x00\x49\xea\
+\x00\x00\x06\x60\x00\x00\x00\x00\x00\x01\x00\x00\x66\xf5\
+\x00\x00\x02\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x22\x45\
+\x00\x00\x05\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x59\x9b\
+\x00\x00\x01\x36\x00\x00\x00\x00\x00\x01\x00\x00\x0e\xd6\
+\x00\x00\x02\xaa\x00\x00\x00\x00\x00\x01\x00\x00\x21\x39\
+\x00\x00\x05\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x62\x94\
+\x00\x00\x00\x5a\x00\x00\x00\x00\x00\x01\x00\x00\x03\xf7\
+\x00\x00\x05\x44\x00\x00\x00\x00\x00\x01\x00\x00\x5d\x95\
+\x00\x00\x02\x18\x00\x00\x00\x00\x00\x01\x00\x00\x1a\x8f\
+\x00\x00\x03\xd8\x00\x00\x00\x00\x00\x01\x00\x00\x4b\x9b\
+\x00\x00\x02\x86\x00\x00\x00\x00\x00\x01\x00\x00\x20\x81\
+\x00\x00\x03\x38\x00\x00\x00\x00\x00\x01\x00\x00\x41\xfb\
+\x00\x00\x05\xea\x00\x00\x00\x00\x00\x01\x00\x00\x63\x91\
+\x00\x00\x04\x1c\x00\x00\x00\x00\x00\x01\x00\x00\x4e\xfb\
+\x00\x00\x02\x58\x00\x00\x00\x00\x00\x01\x00\x00\x1e\xb8\
+\x00\x00\x03\xfa\x00\x00\x00\x00\x00\x01\x00\x00\x4d\x66\
+\x00\x00\x06\x74\x00\x00\x00\x00\x00\x01\x00\x00\x6a\x63\
 "
 
 qt_resource_struct_v2 = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x32\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x33\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x02\x20\x00\x00\x00\x00\x00\x01\x00\x00\x24\x6e\
-\x00\x00\x01\x70\x78\x2f\x94\x65\
-\x00\x00\x03\xe0\x00\x00\x00\x00\x00\x01\x00\x00\x51\x05\
-\x00\x00\x01\x7b\x3b\x98\x74\x68\
-\x00\x00\x05\xf8\x00\x00\x00\x00\x00\x01\x00\x00\x92\x25\
-\x00\x00\x01\x70\x78\x2f\x94\x61\
-\x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x17\x08\
-\x00\x00\x01\x7b\x3b\x98\x74\x73\
-\x00\x00\x02\xd2\x00\x00\x00\x00\x00\x01\x00\x00\x49\x68\
-\x00\x00\x01\x74\x90\x51\x29\x78\
-\x00\x00\x00\x5e\x00\x00\x00\x00\x00\x01\x00\x00\x0d\xa5\
-\x00\x00\x01\x7d\x1f\x10\x16\xee\
-\x00\x00\x04\x8e\x00\x00\x00\x00\x00\x01\x00\x00\x7b\x60\
-\x00\x00\x01\x70\x78\x2f\x94\x67\
-\x00\x00\x06\x50\x00\x00\x00\x00\x00\x01\x00\x00\x98\x11\
-\x00\x00\x01\x7b\x3b\x98\x74\x70\
-\x00\x00\x03\x5a\x00\x00\x00\x00\x00\x01\x00\x00\x4d\xb7\
-\x00\x00\x01\x70\x78\x2f\x94\x5f\
-\x00\x00\x01\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x23\xb6\
-\x00\x00\x01\x76\x44\x5b\x3c\x44\
-\x00\x00\x05\x32\x00\x00\x00\x00\x00\x01\x00\x00\x88\x41\
-\x00\x00\x01\x7d\x1f\x10\x16\xef\
-\x00\x00\x01\x84\x00\x00\x00\x00\x00\x01\x00\x00\x1e\x73\
-\x00\x00\x01\x70\x78\x2f\x94\x60\
-\x00\x00\x02\x36\x00\x01\x00\x00\x00\x01\x00\x00\x24\xfd\
-\x00\x00\x01\x75\xd7\x50\x16\x9e\
-\x00\x00\x03\x7e\x00\x00\x00\x00\x00\x01\x00\x00\x4e\xb4\
-\x00\x00\x01\x70\x78\x2f\x94\x64\
-\x00\x00\x04\x36\x00\x00\x00\x00\x00\x01\x00\x00\x5c\xfe\
-\x00\x00\x01\x70\x78\x2f\x94\x67\
-\x00\x00\x01\xb2\x00\x00\x00\x00\x00\x01\x00\x00\x21\x80\
-\x00\x00\x01\x70\x78\x2f\x94\x68\
-\x00\x00\x00\x1c\x00\x00\x00\x00\x00\x01\x00\x00\x00\xcf\
-\x00\x00\x01\x75\xd7\x50\x16\x9e\
-\x00\x00\x01\x18\x00\x00\x00\x00\x00\x01\x00\x00\x1a\x69\
-\x00\x00\x01\x7d\x1f\x10\x16\xee\
-\x00\x00\x00\x8a\x00\x00\x00\x00\x00\x01\x00\x00\x0f\x14\
-\x00\x00\x01\x70\x78\x2f\x94\x60\
-\x00\x00\x01\x66\x00\x00\x00\x00\x00\x01\x00\x00\x1d\xdc\
-\x00\x00\x01\x70\x78\x2f\x94\x64\
-\x00\x00\x02\x96\x00\x00\x00\x00\x00\x01\x00\x00\x47\x5c\
-\x00\x00\x01\x70\x78\x2f\x94\x69\
-\x00\x00\x06\x1a\x00\x00\x00\x00\x00\x01\x00\x00\x94\xcd\
-\x00\x00\x01\x70\x78\x2f\x94\x5f\
-\x00\x00\x04\xd0\x00\x00\x00\x00\x00\x01\x00\x00\x84\x8c\
-\x00\x00\x01\x70\x78\x2f\x94\x67\
-\x00\x00\x01\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x22\x6e\
-\x00\x00\x01\x7d\x1f\x10\x16\xef\
-\x00\x00\x02\x74\x00\x00\x00\x00\x00\x01\x00\x00\x2b\x01\
-\x00\x00\x01\x7d\x1f\x10\x16\xf0\
-\x00\x00\x00\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x18\x6e\
-\x00\x00\x01\x70\x78\x2f\x94\x62\
-\x00\x00\x03\x38\x00\x00\x00\x00\x00\x01\x00\x00\x4c\x56\
-\x00\x00\x01\x7d\x1f\x10\x16\xee\
-\x00\x00\x05\xb4\x00\x00\x00\x00\x00\x01\x00\x00\x8b\xe7\
-\x00\x00\x01\x75\xd7\x50\x16\x9e\
-\x00\x00\x05\x7a\x00\x00\x00\x00\x00\x01\x00\x00\x8a\x79\
-\x00\x00\x01\x7b\x3b\x98\x74\x70\
+\x00\x00\x00\x44\x00\x00\x00\x00\x00\x01\x00\x00\x03\x68\
+\x00\x00\x01\x85\xa6\x6c\xb8\xda\
+\x00\x00\x02\x36\x00\x00\x00\x00\x00\x01\x00\x00\x1c\x10\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd8\
+\x00\x00\x01\xaa\x00\x00\x00\x00\x00\x01\x00\x00\x11\x0d\
+\x00\x00\x01\x85\xa6\x6c\xb8\xde\
+\x00\x00\x05\x8c\x00\x00\x00\x00\x00\x01\x00\x00\x60\x39\
+\x00\x00\x01\x85\xa6\x6c\xb8\xde\
+\x00\x00\x01\x0a\x00\x00\x00\x00\x00\x01\x00\x00\x0d\x67\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe3\
 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x7d\x1f\x10\x16\xed\
-\x00\x00\x02\x56\x00\x00\x00\x00\x00\x01\x00\x00\x28\xea\
-\x00\x00\x01\x70\x78\x2f\x94\x63\
-\x00\x00\x04\xf8\x00\x00\x00\x00\x00\x01\x00\x00\x85\x62\
-\x00\x00\x01\x7b\x3b\x98\x74\x6f\
-\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x5b\x4d\
-\x00\x00\x01\x70\x78\x2f\x94\x61\
-\x00\x00\x04\x4c\x00\x00\x00\x00\x00\x01\x00\x00\x5d\x93\
-\x00\x00\x01\x7b\x3b\x98\x74\x79\
-\x00\x00\x06\x30\x00\x00\x00\x00\x00\x01\x00\x00\x96\xb8\
-\x00\x00\x01\x70\x78\x2f\x94\x63\
-\x00\x00\x00\xb4\x00\x00\x00\x00\x00\x01\x00\x00\x13\x0e\
-\x00\x00\x01\x70\x78\x2f\x94\x61\
-\x00\x00\x03\x98\x00\x00\x00\x00\x00\x01\x00\x00\x4f\x49\
-\x00\x00\x01\x70\x78\x2f\x94\x66\
-\x00\x00\x02\xf4\x00\x00\x00\x00\x00\x01\x00\x00\x4a\x6f\
-\x00\x00\x01\x70\x78\x2f\x94\x63\
-\x00\x00\x05\xd4\x00\x00\x00\x00\x00\x01\x00\x00\x91\x28\
-\x00\x00\x01\x70\x78\x2f\x94\x5f\
-\x00\x00\x00\x40\x00\x00\x00\x00\x00\x01\x00\x00\x0a\x55\
-\x00\x00\x01\x70\x78\x2f\x94\x69\
-\x00\x00\x05\x58\x00\x00\x00\x00\x00\x01\x00\x00\x89\x10\
-\x00\x00\x01\x7b\x3b\x98\x74\x64\
-\x00\x00\x04\xb2\x00\x00\x00\x00\x00\x01\x00\x00\x7c\x47\
-\x00\x00\x01\x7b\x3b\x98\x74\x66\
-\x00\x00\x01\x44\x00\x00\x00\x00\x00\x01\x00\x00\x1c\x11\
-\x00\x00\x01\x70\x78\x2f\x94\x65\
-\x00\x00\x02\xae\x00\x00\x00\x00\x00\x01\x00\x00\x48\xb0\
-\x00\x00\x01\x7d\x1f\x10\x16\xef\
-\x00\x00\x05\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x86\xbe\
-\x00\x00\x01\x7d\x1f\x10\x16\xee\
-\x00\x00\x05\x90\x00\x00\x00\x00\x00\x01\x00\x00\x8b\x5e\
-\x00\x00\x01\x78\x02\x9b\xa6\xe9\
-\x00\x00\x03\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x50\x13\
-\x00\x00\x01\x7d\x1f\x10\x16\xed\
-\x00\x00\x04\x60\x00\x00\x00\x00\x00\x01\x00\x00\x79\x97\
-\x00\x00\x01\x70\x78\x2f\x94\x68\
-\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00\x53\xe3\
-\x00\x00\x01\x7b\x3b\x98\x74\x73\
-\x00\x00\x03\x12\x00\x00\x00\x00\x00\x01\x00\x00\x4b\x7b\
-\x00\x00\x01\x70\x78\x2f\x94\x62\
+\x00\x00\x01\x85\xa6\x6c\xb8\xde\
+\x00\x00\x06\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x64\x1a\
+\x00\x00\x01\x85\xa6\x6c\xb8\xdd\
+\x00\x00\x03\x9c\x00\x00\x00\x00\x00\x01\x00\x00\x48\xed\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd7\
+\x00\x00\x00\x94\x00\x00\x00\x00\x00\x01\x00\x00\x08\x16\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe0\
+\x00\x00\x04\x72\x00\x00\x00\x00\x00\x01\x00\x00\x51\xe6\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe4\
+\x00\x00\x01\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x12\x73\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd8\
+\x00\x00\x00\x24\x00\x01\x00\x00\x00\x01\x00\x00\x00\xe7\
+\x00\x00\x01\x86\xa2\xe1\x75\x10\
+\x00\x00\x05\x04\x00\x00\x00\x00\x00\x01\x00\x00\x59\x06\
+\x00\x00\x01\x85\xa6\x6c\xb8\xda\
+\x00\x00\x04\x4c\x00\x00\x00\x00\x00\x01\x00\x00\x50\x82\
+\x00\x00\x01\x85\x89\xd1\xeb\x50\
+\x00\x00\x04\x36\x00\x00\x00\x00\x00\x01\x00\x00\x4f\xed\
+\x00\x00\x01\x85\xa6\x6c\xb8\xdc\
+\x00\x00\x05\x66\x00\x00\x00\x00\x00\x01\x00\x00\x5e\xfe\
+\x00\x00\x01\x85\x89\xd1\xeb\x50\
+\x00\x00\x06\x3a\x00\x00\x00\x00\x00\x01\x00\x00\x65\xe4\
+\x00\x00\x01\x85\x89\xd1\xeb\x50\
+\x00\x00\x04\x98\x00\x00\x00\x00\x00\x01\x00\x00\x52\xb5\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe0\
+\x00\x00\x01\xf4\x00\x00\x00\x00\x00\x01\x00\x00\x15\x80\
+\x00\x00\x01\x86\xa2\xe1\x75\x10\
+\x00\x00\x00\xbe\x00\x00\x00\x00\x00\x01\x00\x00\x08\xce\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe3\
+\x00\x00\x03\x5c\x00\x00\x00\x00\x00\x01\x00\x00\x43\x7e\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd8\
+\x00\x00\x01\x64\x00\x00\x00\x00\x00\x01\x00\x00\x0f\xa0\
+\x00\x00\x01\x85\xa6\x6c\xb8\xda\
+\x00\x00\x05\xae\x00\x00\x00\x00\x00\x01\x00\x00\x61\x40\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe0\
+\x00\x00\x04\xd0\x00\x00\x00\x00\x00\x01\x00\x00\x55\x04\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd8\
+\x00\x00\x01\x82\x00\x00\x00\x00\x00\x01\x00\x00\x10\x37\
+\x00\x00\x01\x85\xa6\x6c\xb8\xde\
+\x00\x00\x02\xe8\x00\x00\x00\x00\x00\x01\x00\x00\x23\x9e\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe4\
+\x00\x00\x03\x16\x00\x00\x00\x00\x00\x01\x00\x00\x24\xe6\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe4\
+\x00\x00\x04\xae\x00\x00\x00\x00\x00\x01\x00\x00\x53\xa3\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe3\
+\x00\x00\x00\xea\x00\x00\x00\x00\x00\x01\x00\x00\x0a\x76\
+\x00\x00\x01\x86\xa2\xe1\x75\x10\
+\x00\x00\x06\x24\x00\x00\x00\x00\x00\x01\x00\x00\x64\xff\
+\x00\x00\x01\x85\xa6\x6c\xb8\xdd\
+\x00\x00\x00\x78\x00\x00\x00\x00\x00\x01\x00\x00\x07\x47\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe2\
+\x00\x00\x04\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x56\xef\
+\x00\x00\x01\x85\xa6\x6c\xb8\xda\
+\x00\x00\x03\x86\x00\x00\x00\x00\x00\x01\x00\x00\x47\x78\
+\x00\x00\x01\x56\xe8\x21\x2a\xd8\
+\x00\x00\x03\xc0\x00\x00\x00\x00\x00\x01\x00\x00\x49\xea\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd9\
+\x00\x00\x06\x60\x00\x00\x00\x00\x00\x01\x00\x00\x66\xf5\
+\x00\x00\x01\x86\xa2\xde\x50\xe1\
+\x00\x00\x02\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x22\x45\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd9\
+\x00\x00\x05\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x59\x9b\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd8\
+\x00\x00\x01\x36\x00\x00\x00\x00\x00\x01\x00\x00\x0e\xd6\
+\x00\x00\x01\x85\xa6\x6c\xb8\xda\
+\x00\x00\x02\xaa\x00\x00\x00\x00\x00\x01\x00\x00\x21\x39\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd9\
+\x00\x00\x05\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x62\x94\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd7\
+\x00\x00\x00\x5a\x00\x00\x00\x00\x00\x01\x00\x00\x03\xf7\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe0\
+\x00\x00\x05\x44\x00\x00\x00\x00\x00\x01\x00\x00\x5d\x95\
+\x00\x00\x01\x85\xa6\x6c\xb8\xda\
+\x00\x00\x02\x18\x00\x00\x00\x00\x00\x01\x00\x00\x1a\x8f\
+\x00\x00\x01\x86\xa7\x9d\x25\x5e\
+\x00\x00\x03\xd8\x00\x00\x00\x00\x00\x01\x00\x00\x4b\x9b\
+\x00\x00\x01\x85\xa6\x6c\xb8\xda\
+\x00\x00\x02\x86\x00\x00\x00\x00\x00\x01\x00\x00\x20\x81\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe3\
+\x00\x00\x03\x38\x00\x00\x00\x00\x00\x01\x00\x00\x41\xfb\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe3\
+\x00\x00\x05\xea\x00\x00\x00\x00\x00\x01\x00\x00\x63\x91\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe3\
+\x00\x00\x04\x1c\x00\x00\x00\x00\x00\x01\x00\x00\x4e\xfb\
+\x00\x00\x01\x85\xa6\x6c\xb8\xe3\
+\x00\x00\x02\x58\x00\x00\x00\x00\x00\x01\x00\x00\x1e\xb8\
+\x00\x00\x01\x85\xa6\x6c\xb8\xde\
+\x00\x00\x03\xfa\x00\x00\x00\x00\x00\x01\x00\x00\x4d\x66\
+\x00\x00\x01\x86\xa7\x65\xdc\x82\
+\x00\x00\x06\x74\x00\x00\x00\x00\x00\x01\x00\x00\x6a\x63\
+\x00\x00\x01\x85\xa6\x6c\xb8\xd9\
 "
 
 qt_version = [int(v) for v in QtCore.qVersion().split('.')]
 if qt_version < [5, 8, 0]:
     rcc_version = 1
     qt_resource_struct = qt_resource_struct_v1
 else:
```

### Comparing `pyfda-0.7.1/pyfda/widget_templates/filter_widgets/my_filter_widget.py` & `pyfda-0.8.0a2/pyfda/widget_templates/filter_widgets/my_filter_widget.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/widget_templates/input_widgets/my_input_widget.py` & `pyfda-0.8.0a2/pyfda/widget_templates/input_widgets/my_input_widget.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda/widget_templates/plot_widgets/myplot.py` & `pyfda-0.8.0a2/pyfda/widget_templates/plot_widgets/myplot.py`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/pyfda.egg-info/PKG-INFO` & `pyfda-0.8.0a2/pyfda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfda
-Version: 0.7.1
+Version: 0.8.0a2
 Summary: Design and analyse discrete time DSP filters with a user-friendly GUI tool. Fixpoint filters in time and frequency domain, too.
 Home-page: https://github.com/chipmuenk/pyFDA
 Author: Christian Muenker
 Author-email: mail07@chipmuenk.de
 License: MIT
 Keywords: digital,discrete time,filter design,IIR,FIR,GUI
 Platform: any
```

### Comparing `pyfda-0.7.1/pyfda.egg-info/SOURCES.txt` & `pyfda-0.8.0a2/pyfda.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 LICENSE_GPLv3.md
 MANIFEST.in
 README.md
 README_PYPI.md
 pyfdax.spec
 requirements.txt
 setup.py
-bak/iir_df1_test.py
-bak/delay/fx_delay.py
-docs/source/conf.py
-docs/source/_static/ideas/mpl_pyqt4_widget.py
-docs/source/_static/ideas/plotTest.py
 pyfda/__init__.py
 pyfda/filter_factory.py
 pyfda/filterbroker.py
 pyfda/license_info.md
 pyfda/module_versions.md
 pyfda/pyfda.qrc
 pyfda/pyfda_rc.py
@@ -51,20 +46,14 @@
 pyfda/fixpoint_widgets/fir_df/fir_df.png
 pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp.py
 pyfda/fixpoint_widgets/fir_df/fir_df_pyfixp_ui.py
 pyfda/fixpoint_widgets/iir_df1/iir_df1.png
 pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp.py
 pyfda/fixpoint_widgets/iir_df1/iir_df1_pyfixp_ui.py
 pyfda/images/icons/fft.svg
-pyfda/images/icons/graph.svg
-pyfda/images/icons/grid_coarse.svg
-pyfda/images/icons/grid_fine.svg
-pyfda/images/icons/grid_man.svg
-pyfda/images/icons/grid_none.svg
-pyfda/images/icons/help.svg
 pyfda/images/icons/plot_style-line-mkr.png
 pyfda/images/icons/plot_style-line.png
 pyfda/images/icons/plot_style-mkr.png
 pyfda/images/icons/plot_style-none.png
 pyfda/images/icons/plot_style-stem-mkr.png
 pyfda/images/icons/plot_style-stem.png
 pyfda/images/icons/plot_style-steps-mkr.png
@@ -81,71 +70,79 @@
 pyfda/images/icons/dark/action-redo.svg
 pyfda/images/icons/dark/action-undo.svg
 pyfda/images/icons/dark/appbar.disk.svg
 pyfda/images/icons/dark/appbar.from_clipboard.svg
 pyfda/images/icons/dark/appbar.list.add.above.svg
 pyfda/images/icons/dark/appbar.list.delete.svg
 pyfda/images/icons/dark/appbar.to_clipboard.svg
-pyfda/images/icons/dark/audio_90.odg
 pyfda/images/icons/dark/brush.svg
-pyfda/images/icons/dark/camera-slr.svg
 pyfda/images/icons/dark/circle-check.svg
 pyfda/images/icons/dark/circle-x.svg
 pyfda/images/icons/dark/clipboard.svg
 pyfda/images/icons/dark/cog.svg
 pyfda/images/icons/dark/data-transfer-download.svg
 pyfda/images/icons/dark/data-transfer-upload.svg
+pyfda/images/icons/dark/density_large.svg
+pyfda/images/icons/dark/density_medium.svg
+pyfda/images/icons/dark/density_small.svg
 pyfda/images/icons/dark/ellipses_h.svg
 pyfda/images/icons/dark/ellipses_v.svg
 pyfda/images/icons/dark/file.svg
 pyfda/images/icons/dark/fullscreen-enter.svg
-pyfda/images/icons/dark/graph.svg
-pyfda/images/icons/dark/graph_90.odg
-pyfda/images/icons/dark/graph_90.png
-pyfda/images/icons/dark/grid-four-up.svg
-pyfda/images/icons/dark/grid-three-up.svg
-pyfda/images/icons/dark/grid-two-up.svg
+pyfda/images/icons/dark/graph_90.svg
+pyfda/images/icons/dark/grid_coarse.svg
+pyfda/images/icons/dark/grid_fine.svg
+pyfda/images/icons/dark/grid_none.svg
 pyfda/images/icons/dark/home.svg
-pyfda/images/icons/dark/ic_fiber_manual_record_48px.svg
-pyfda/images/icons/dark/ic_forward_10_48px.svg
-pyfda/images/icons/dark/ic_hearing_48px.svg
-pyfda/images/icons/dark/ic_help_48px.svg
-pyfda/images/icons/dark/ic_help_outline_24px.svg
-pyfda/images/icons/dark/ic_mic_48px.svg
+pyfda/images/icons/dark/ic_help_24px.svg
 pyfda/images/icons/dark/ic_pause_48px.svg
 pyfda/images/icons/dark/ic_play_arrow_48px.svg
-pyfda/images/icons/dark/ic_skip_next_48px.svg
 pyfda/images/icons/dark/ic_stop_48px.svg
-pyfda/images/icons/dark/ic_volume_mute_48px.svg
 pyfda/images/icons/dark/ic_volume_up_48px.svg
 pyfda/images/icons/dark/ic_volume_up_48px_90.svg
 pyfda/images/icons/dark/lock-locked.svg
 pyfda/images/icons/dark/lock-unlocked.svg
 pyfda/images/icons/dark/magnifying-glass.svg
 pyfda/images/icons/dark/map-marker.svg
-pyfda/images/icons/dark/media-pause-4x.png
-pyfda/images/icons/dark/media-play-4x.png
-pyfda/images/icons/dark/media-record-4x.png
-pyfda/images/icons/dark/media-skip-backward-4x.png
-pyfda/images/icons/dark/media-skip-forward-4x.png
-pyfda/images/icons/dark/media-step-backward-4x.png
-pyfda/images/icons/dark/media-step-forward-4x.png
-pyfda/images/icons/dark/media-stop-4x.png
 pyfda/images/icons/dark/move.svg
 pyfda/images/icons/dark/quantize.svg
-pyfda/images/icons/dark/question-mark.svg
 pyfda/images/icons/dark/sort-ascending.svg
 pyfda/images/icons/dark/trash.svg
-pyfda/images/icons/light/appbar.base.select_grey.svg
-pyfda/images/icons/light/appbar.list.add.above_grey.svg
 pyfda/images/icons/light/ic_pause_48px_white.svg
 pyfda/images/icons/light/ic_play_arrow_48px_white.svg
-pyfda/images/unused/audio.svg
-pyfda/images/unused/audio_90.png
-pyfda/images/unused/audio_90.svg
+pyfda/images/unused/appbar.base.select_grey.svg
+pyfda/images/unused/appbar.list.add.above_grey.svg
+pyfda/images/unused/camera-slr.svg
+pyfda/images/unused/graph.svg
+pyfda/images/unused/graph_90.odg
+pyfda/images/unused/graph_90.png
+pyfda/images/unused/grid-four-up.svg
+pyfda/images/unused/grid-three-up.svg
+pyfda/images/unused/grid-two-up.svg
+pyfda/images/unused/ic_volume_mute_48px.svg
+pyfda/images/unused/question-mark.svg
+pyfda/images/unused/square_outlined.svg
+pyfda/images/unused/table_chart_outlined.svg
+pyfda/images/unused/table_outlined.svg
+pyfda/images/unused/audio/audio.svg
+pyfda/images/unused/audio/audio_90.odg
+pyfda/images/unused/audio/audio_90.png
+pyfda/images/unused/audio/audio_90.svg
+pyfda/images/unused/audio/ic_fiber_manual_record_48px.svg
+pyfda/images/unused/audio/ic_forward_10_48px.svg
+pyfda/images/unused/audio/ic_mic_48px.svg
+pyfda/images/unused/audio/ic_skip_next_48px.svg
+pyfda/images/unused/audio/media-pause-4x.png
+pyfda/images/unused/audio/media-play-4x.png
+pyfda/images/unused/audio/media-record-4x.png
+pyfda/images/unused/audio/media-skip-backward-4x.png
+pyfda/images/unused/audio/media-skip-forward-4x.png
+pyfda/images/unused/audio/media-step-backward-4x.png
+pyfda/images/unused/audio/media-step-forward-4x.png
+pyfda/images/unused/audio/media-stop-4x.png
 pyfda/input_widgets/__init__.py
 pyfda/input_widgets/amplitude_specs.py
 pyfda/input_widgets/freq_specs.py
 pyfda/input_widgets/freq_units.py
 pyfda/input_widgets/input_coeffs.py
 pyfda/input_widgets/input_coeffs_ui.py
 pyfda/input_widgets/input_fixpoint_specs.py
@@ -184,27 +181,15 @@
 pyfda/plot_widgets/plot_tab_widgets.py
 pyfda/plot_widgets/plot_tau_g.py
 pyfda/plot_widgets/tran/__init__.py
 pyfda/plot_widgets/tran/plot_tran_stim.py
 pyfda/plot_widgets/tran/plot_tran_stim_ui.py
 pyfda/plot_widgets/tran/tran_io.py
 pyfda/plot_widgets/tran/tran_io_ui.py
-pyfda/tests/__init__.py
-pyfda/tests/test_dummy.py
-pyfda/tests/test_fir_df.py
-pyfda/tests/test_fixpoint_helpers.py
-pyfda/tests/test_pyfda_fix_lib.py
-pyfda/tests/test_uniqueroots.py
-pyfda/tests/test_uniqueroots_time.py
-pyfda/tests/widgets/__init__.py
-pyfda/tests/widgets/input_widgets/__init__.py
-pyfda/tests/widgets/input_widgets/test_input_coeffs.py
-pyfda/tests/widgets/plot_widgets/__init__.py
 pyfda/widget_templates/__init__.py
 pyfda/widget_templates/filter_widgets/__init__.py
 pyfda/widget_templates/filter_widgets/my_filter_widget.py
 pyfda/widget_templates/fixpoint_widgets/__init__.py
 pyfda/widget_templates/input_widgets/__init__.py
 pyfda/widget_templates/input_widgets/my_input_widget.py
 pyfda/widget_templates/plot_widgets/__init__.py
-pyfda/widget_templates/plot_widgets/myplot.py
-recipe/pyfdax.spec_bak.py
+pyfda/widget_templates/plot_widgets/myplot.py
```

### Comparing `pyfda-0.7.1/pyfdax.spec` & `pyfda-0.8.0a2/pyfdax.spec`

 * *Files identical despite different names*

### Comparing `pyfda-0.7.1/setup.py` & `pyfda-0.8.0a2/setup.py`

 * *Files identical despite different names*

