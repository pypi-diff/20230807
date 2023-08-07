# Comparing `tmp/wbpUFO-0.2.2.tar.gz` & `tmp/wbpUFO-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpUFO-0.2.2.tar", last modified: Wed Jul 19 14:25:21 2023, max compression
+gzip compressed data, was "wbpUFO-0.2.3.tar", last modified: Mon Aug  7 16:04:47 2023, max compression
```

## Comparing `wbpUFO-0.2.2.tar` & `wbpUFO-0.2.3.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.379218 wbpUFO-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.355219 wbpUFO-0.2.2/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.357219 wbpUFO-0.2.2/Lib/wbpUFO/
--rw-rw-rw-   0 root         (0) root         (0)    10601 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.360219 wbpUFO-0.2.2/Lib/wbpUFO/control/
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/dialogItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/dialogItemPickerUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/findGlyphListCtrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.361219 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 14:25:20.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24105 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/canvas.py
--rw-rw-rw-   0 root         (0) root         (0)    20703 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.361219 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8393 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3460 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/font.py
--rw-rw-rw-   0 root         (0) root         (0)    28062 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py
--rw-rw-rw-   0 root         (0) root         (0)     5602 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/editPanel.py
--rw-rw-rw-   0 root         (0) root         (0)    21609 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/menu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.364219 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py
--rw-rw-rw-   0 root         (0) root         (0)    13199 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2079 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py
--rw-rw-rw-   0 root         (0) root         (0)     2953 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py
--rw-rw-rw-   0 root         (0) root         (0)    16709 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py
--rw-rw-rw-   0 root         (0) root         (0)     3421 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py
--rw-rw-rw-   0 root         (0) root         (0)     7101 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py
--rw-rw-rw-   0 root         (0) root         (0)     5302 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py
--rw-rw-rw-   0 root         (0) root         (0)     1691 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2756 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py
--rw-rw-rw-   0 root         (0) root         (0)     4094 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphGridStatusPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     5122 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/kerningViewCanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/kerningViewPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     5038 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/libControl.py
--rw-rw-rw-   0 root         (0) root         (0)     2798 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/panelItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     5686 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/panelItemPickerUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.368219 wbpUFO-0.2.2/Lib/wbpUFO/dialog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 14:25:20.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1292 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/anchorDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4887 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/anchorDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3351 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/assignLayerDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     6012 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/assignLayerDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/componentDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4425 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/componentDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/deleteGlyphsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     6084 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/findGlyphDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5036 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/findGlyphDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/guidelineDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5816 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/guidelineDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/layerDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2511 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/layerDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/newFontDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/newFontDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/newGlyphDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/newGlyphDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     8386 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/renameGlyphDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     9608 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/renameGlyphDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     5367 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/revertFontDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     7261 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/revertFontDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/selectFontsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     1967 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/selectFontsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    19544 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.370219 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/
--rw-rw-rw-   0 root         (0) root         (0)     3040 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1773 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/anchor.py
--rw-rw-rw-   0 root         (0) root         (0)     4404 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/base.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListCtrl.py
--rw-rw-rw-   0 root         (0) root         (0)    13260 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListDialog.py
--rw-rw-rw-   0 root         (0) root         (0)    12967 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     4328 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2070 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/guideline.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     7342 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/metric.py
--rw-rw-rw-   0 root         (0) root         (0)     1685 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     5157 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/parameter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.370219 wbpUFO-0.2.2/Lib/wbpUFO/panel/
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/panel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16132 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewCanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewPanel.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.371219 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5259 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/command.py
--rw-rw-rw-   0 root         (0) root         (0)     4790 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/editTool.py
--rw-rw-rw-   0 root         (0) root         (0)     4521 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/glyphLock.py
--rw-rw-rw-   0 root         (0) root         (0)     7625 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/glyphShow.py
--rw-rw-rw-   0 root         (0) root         (0)    12968 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     4501 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/markColor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.372218 wbpUFO-0.2.2/Lib/wbpUFO/view/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.379218 wbpUFO-0.2.2/Lib/wbpUFO/view/font/
--rw-rw-rw-   0 root         (0) root         (0)     5480 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19462 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/feature.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoBase.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCaret.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCaretUI.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoClassification.py
--rw-rw-rw-   0 root         (0) root         (0)     4073 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoClassificationUI.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCodepage.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCodepageUI.py
--rw-rw-rw-   0 root         (0) root         (0)     8952 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoControl.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEmbedding.py
--rw-rw-rw-   0 root         (0) root         (0)     3938 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEncoding.py
--rw-rw-rw-   0 root         (0) root         (0)     4188 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEncodingUI.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHinting.py
--rw-rw-rw-   0 root         (0) root         (0)     1910 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingPS.py
--rw-rw-rw-   0 root         (0) root         (0)    10731 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py
--rw-rw-rw-   0 root         (0) root         (0)     6830 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingUI.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoIdentification.py
--rw-rw-rw-   0 root         (0) root         (0)     6714 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLegal.py
--rw-rw-rw-   0 root         (0) root         (0)     6955 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLegalUI.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLine.py
--rw-rw-rw-   0 root         (0) root         (0)     4862 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLineUI.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoMetric.py
--rw-rw-rw-   0 root         (0) root         (0)    13226 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoMetricUI.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoName.py
--rw-rw-rw-   0 root         (0) root         (0)    13730 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNameUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNote.py
--rw-rw-rw-   0 root         (0) root         (0)     1740 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNoteUI.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoSuperSubscript.py
--rw-rw-rw-   0 root         (0) root         (0)     7207 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoUnicode.py
--rw-rw-rw-   0 root         (0) root         (0)     2453 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoValidator.py
--rw-rw-rw-   0 root         (0) root         (0)    42129 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/glyphGrid.py
--rw-rw-rw-   0 root         (0) root         (0)    13747 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/groupsStatusPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3244 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/hintPSlistCtrl.py
--rw-rw-rw-   0 root         (0) root         (0)     7302 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/hintPSpanel.py
--rw-rw-rw-   0 root         (0) root         (0)    16330 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/info.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/kerning.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/kerningStatusPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     4342 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/stemPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     4950 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/zonePanelUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.379218 wbpUFO-0.2.2/Lib/wbpUFO/view/fontinfo/
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/fontinfo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/glyph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.358219 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2211 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5825 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2211 2023-07-19 14:25:21.379218 wbpUFO-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2221 2023-07-19 14:25:21.380218 wbpUFO-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-19 14:25:20.000000 wbpUFO-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.954537 wbpUFO-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.924537 wbpUFO-0.2.3/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.927537 wbpUFO-0.2.3/Lib/wbpUFO/
+-rw-rw-rw-   0 root         (0) root         (0)    10601 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.930537 wbpUFO-0.2.3/Lib/wbpUFO/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/dialogItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/dialogItemPickerUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/findGlyphListCtrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.931537 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24105 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/canvas.py
+-rw-rw-rw-   0 root         (0) root         (0)    20703 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.932537 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/drawing/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/drawing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8393 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/drawing/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3460 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/drawing/font.py
+-rw-rw-rw-   0 root         (0) root         (0)    28062 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5602 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/editPanel.py
+-rw-rw-rw-   0 root         (0) root         (0)    21769 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/menu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.935537 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py
+-rw-rw-rw-   0 root         (0) root         (0)    13199 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py
+-rw-rw-rw-   0 root         (0) root         (0)     2953 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py
+-rw-rw-rw-   0 root         (0) root         (0)    17019 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py
+-rw-rw-rw-   0 root         (0) root         (0)     7101 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py
+-rw-rw-rw-   0 root         (0) root         (0)     5302 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2756 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py
+-rw-rw-rw-   0 root         (0) root         (0)     4094 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/glyphGridStatusPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     5122 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/kerningViewCanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/kerningViewPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     5038 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/libControl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/panelItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5686 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/control/panelItemPickerUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.941537 wbpUFO-0.2.3/Lib/wbpUFO/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/anchorDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4887 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/anchorDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3351 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/assignLayerDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     6012 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/assignLayerDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/componentDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4425 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/componentDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/deleteGlyphsDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     6084 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/findGlyphDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5036 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/findGlyphDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/guidelineDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5816 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/guidelineDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/layerDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2511 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/layerDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/newFontDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/newFontDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/newGlyphDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/newGlyphDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     8386 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/renameGlyphDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     9608 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/renameGlyphDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     5367 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/revertFontDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     7261 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/revertFontDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/selectFontsDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/dialog/selectFontsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    19544 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.943537 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/
+-rw-rw-rw-   0 root         (0) root         (0)     3040 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/anchor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/commandListCtrl.py
+-rw-rw-rw-   0 root         (0) root         (0)    13260 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/commandListDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    12967 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/commandListDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     4328 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/guideline.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7342 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/metric.py
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5157 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/parameter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.944537 wbpUFO-0.2.3/Lib/wbpUFO/panel/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/panel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16132 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/panel/glyphViewCanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/panel/glyphViewPanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/panel/glyphViewPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.946537 wbpUFO-0.2.3/Lib/wbpUFO/toolbar/
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/toolbar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5259 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/toolbar/command.py
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/toolbar/editTool.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/toolbar/glyphLock.py
+-rw-rw-rw-   0 root         (0) root         (0)     7625 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/toolbar/glyphShow.py
+-rw-rw-rw-   0 root         (0) root         (0)    12968 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/toolbar/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4501 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/toolbar/markColor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.946537 wbpUFO-0.2.3/Lib/wbpUFO/view/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.954537 wbpUFO-0.2.3/Lib/wbpUFO/view/font/
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19462 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/feature.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoCaret.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoCaretUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoClassification.py
+-rw-rw-rw-   0 root         (0) root         (0)     4073 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoClassificationUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoCodepage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoCodepageUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     8952 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoControl.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoEmbedding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoEncoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoEncodingUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoHinting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoHintingPS.py
+-rw-rw-rw-   0 root         (0) root         (0)    10731 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     6830 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoHintingUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoIdentification.py
+-rw-rw-rw-   0 root         (0) root         (0)     6714 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoLegal.py
+-rw-rw-rw-   0 root         (0) root         (0)     6955 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoLegalUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoLine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4862 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoLineUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoMetric.py
+-rw-rw-rw-   0 root         (0) root         (0)    13226 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoMetricUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoName.py
+-rw-rw-rw-   0 root         (0) root         (0)    13730 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoNameUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoNote.py
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoNoteUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoSuperSubscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     7207 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoUnicode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2453 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoValidator.py
+-rw-rw-rw-   0 root         (0) root         (0)    42129 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/glyphGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    13747 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/groupsStatusPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/hintPSlistCtrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     7302 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/hintPSpanel.py
+-rw-rw-rw-   0 root         (0) root         (0)    16330 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/kerning.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/kerningStatusPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4342 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/stemPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4950 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/font/zonePanelUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.954537 wbpUFO-0.2.3/Lib/wbpUFO/view/fontinfo/
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/fontinfo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/Lib/wbpUFO/view/glyph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:04:47.928537 wbpUFO-0.2.3/Lib/wbpUFO.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-08-07 16:04:47.000000 wbpUFO-0.2.3/Lib/wbpUFO.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5825 2023-08-07 16:04:47.000000 wbpUFO-0.2.3/Lib/wbpUFO.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 16:04:47.000000 wbpUFO-0.2.3/Lib/wbpUFO.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-07 16:04:47.000000 wbpUFO-0.2.3/Lib/wbpUFO.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-07 16:04:47.000000 wbpUFO-0.2.3/Lib/wbpUFO.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-07 16:04:47.000000 wbpUFO-0.2.3/Lib/wbpUFO.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-08-07 16:04:47.955536 wbpUFO-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2023-08-07 16:04:47.955536 wbpUFO-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-08-07 16:04:46.000000 wbpUFO-0.2.3/setup.py
```

### Comparing `wbpUFO-0.2.2/LICENSE` & `wbpUFO-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/__init__.py` & `wbpUFO-0.2.3/Lib/wbpUFO/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from .toolbar.markColor import GlyphMarkToolbar
 from .view.font import UfoFontView
 from .view.glyph import UfoGlyphView
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 
 def getApp() -> App:
     """
     The currently running Workbench application.
     """
     return wx.GetApp()
```

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/config.py` & `wbpUFO-0.2.3/Lib/wbpUFO/config.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/__init__.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/dialogItemPicker.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/dialogItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/dialogItemPickerUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/dialogItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/findGlyphListCtrl.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/findGlyphListCtrl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/canvas.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/canvas.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/cursor.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/cursor.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/base.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/drawing/base.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/font.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/drawing/font.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/editPanel.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/editPanel.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/menu.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 import os
 
 import wx
 from booleanOperations import BooleanOperationManager as Boolean
 
 from wbBase.scripting import MacroMenu
-from wbDefcon import Anchor, Component, Point, Guideline, Glyph
+from wbDefcon import Anchor, Component, Point, Guideline, Glyph, Font
 from wbDefcon.pens import ContourHit
 
 from ...dialog.anchorDialog import AnchorDialog
 from ...dialog.componentDialog import ComponentDialog
 from ...dialog.findGlyphDialog import FindGlyphDialog
 from ...dialog.guidelineDialog import GuidelineDialog
 from ...glyphCommand.commandListDialog import CommandListDialog
@@ -261,15 +261,15 @@
         #     item.SetFont(wx.GetApp().TopWindow.Font)
 
     @property
     def app(self):
         return wx.GetApp()
 
     @property
-    def glyph(self):
+    def glyph(self) -> Glyph:
         planeStack = self.canvas.getActiveDrawingPlaneStack()
         if isinstance(planeStack, LayerPlanes):
             return planeStack.glyph
         else:
             return self.canvas.glyph
 
     @property
@@ -370,27 +370,27 @@
 
     # Components --------------------
 
     def on_editComponent(self, event):
         self.subject.font[self.subject.baseGlyph].show()
 
     def on_componentProperties(self, event):
-        component = self.subject
+        component:Component = self.subject
         componentDialog = ComponentDialog(self.canvas, component)
         if componentDialog.ShowModal() == wx.ID_OK:
             component.baseGlyph = componentDialog.baseGlyph
             component.offset = componentDialog.offset
             component.scale = componentDialog.scale
         componentDialog.Destroy()
 
     def on_setComponentIndex(self, event):
         font = self.font
-        if font:
+        if isinstance(font, Font):
             font.holdNotifications()
-        glyph = self.glyph
+        glyph:Glyph = self.glyph
         glyph.disableNotifications()
         glyph.undoManager.saveState()
         pointedComponent = self.subject
         pointedComponentIndex = glyph.componentIndex(pointedComponent)
         with wx.SingleChoiceDialog(
             self.Parent,
             "Select new Component Index",
@@ -401,15 +401,15 @@
             if dialog.ShowModal() == wx.ID_OK:
                 newComponentIndex = dialog.Selection
                 if newComponentIndex != pointedComponentIndex:
                     glyph.removeComponent(pointedComponent)
                     glyph.insertComponent(newComponentIndex, pointedComponent)
         glyph.enableNotifications()
         glyph.postNotification("Glyph.ComponentsChanged")
-        if font:
+        if isinstance(font, Font):
             font.releaseHeldNotifications()
 
 
     def on_decomposeComponent(self, event):
         self.glyph.decomposeComponent(self.subject)
 
     def on_deleteComponent(self, event):
@@ -444,15 +444,15 @@
 
     def on_reverseAllContours(self, event):
         for contour in self.glyph:
             contour.reverse()
 
     def on_setContourIndex(self, event):
         font = self.font
-        if font:
+        if isinstance(font, Font):
             font.holdNotifications()
         glyph = self.glyph
         glyph.disableNotifications()
         glyph.undoManager.saveState()
         pointedContour = None
         if isinstance(self.subject, ContourHit):
             pointedContour = self.subject.contour
@@ -472,16 +472,17 @@
             ) as dialog:
                 dialog.Selection = pointedContourIndex
                 if dialog.ShowModal() == wx.ID_OK:
                     newContourIndex = dialog.Selection
                     if newContourIndex != pointedContourIndex:
                         glyph.removeContour(pointedContour)
                         glyph.insertContour(newContourIndex, pointedContour)
-        glyph.enableNotifications()
-        glyph.postNotification("Glyph.ContoursChanged")
+                        glyph.dirty = True
+                        glyph.enableNotifications()
+                        glyph.postNotification("Glyph.ContoursChanged")
         if font:
             font.releaseHeldNotifications()
 
     def on_substractContour(self, event):
         font = self.font
         if font:
             font.holdNotifications()
```

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/__init__.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/base.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/base.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,16 @@
     def on_LEFT_DOWN(self, event):
         super().on_LEFT_DOWN(event)
         glyph = self.glyph
         if self.subject is None:
             self.state = RUBBERBANDING
         elif glyph is not None:
             glyph.undoManager.saveState()
-            glyph.disableNotifications()
+            # glyph.disableNotifications()
+            glyph.holdNotifications()
             self.state = WORKING
         event.Skip()
 
     def on_LEFT_UP(self, event):
         log.debug("on_LEFT_UP: %r", self.state)
         glyph = self.glyph
         if glyph is not None:
@@ -155,46 +156,51 @@
                 )
                 glyph.font.selectRect(
                     (x0, y0, x1, y1),
                     addToSelection=event.ShiftDown(),
                     selectGuidelines=not stack["GlyphGuide"].locked,
                 )
             elif self.state == WORKING:
-                try:
-                    glyph.enableNotifications()
-                except KeyError:
-                    pass
+                # try:
+                #     glyph.enableNotifications()
+                # except KeyError:
+                #     pass
                 if not self.subject.selected:
                     if not event.ShiftDown():
                         self.unselectAll()
                     self.subject.selected = True
                     if (
                         isinstance(self.subject, Point)
                         and self.subject.segmentType is not None
                     ):
                         for contour in glyph:
                             if self.subject in contour.onCurvePoints:
                                 contour.updateSelection()
                 self.postNotifications()
+            if glyph.dispatcher.areNotificationsHeld(glyph):
+                glyph.releaseHeldNotifications()
         super().on_LEFT_UP(event)
 
     def on_RIGHT_DOWN(self, event):
         if self.state == WORKING and not self.subject.selected:
             # right click while left is down on unselected objets
             glyph = self.glyph
             if isinstance(self.subject, Anchor):
                 glyph.removeAnchor(self.subject)
+                self.anchorsChanged = True
             elif isinstance(self.subject, Component):
                 glyph.removeComponent(self.subject)
                 self.componentsChanged = True
             elif isinstance(self.subject, Guideline):
                 if self.subject.glyph is None:
                     glyph.font.removeGuideline(self.subject)
+                    self.fontGuidelinesChanged = True
                 else:
                     glyph.removeGuideline(self.subject)
+                    self.glyphGuidelinesChanged = True
             elif isinstance(self.subject, Point):
                 point = self.subject
                 for contour in glyph:
                     if point in contour:
                         segmentIndex = contour.segmentIndex(point)
                         if segmentIndex >= 0:
                             glyph.enableNotifications()
```

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphGridStatusPanelUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/glyphGridStatusPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/kerningViewCanvas.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/kerningViewCanvas.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/kerningViewPanelUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/kerningViewPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/libControl.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/libControl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/panelItemPicker.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/panelItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/control/panelItemPickerUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/control/panelItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/anchorDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/anchorDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/anchorDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/anchorDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/assignLayerDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/assignLayerDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/assignLayerDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/assignLayerDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/componentDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/componentDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/componentDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/componentDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/deleteGlyphsDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/deleteGlyphsDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/findGlyphDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/findGlyphDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/findGlyphDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/findGlyphDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/guidelineDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/guidelineDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/guidelineDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/guidelineDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/layerDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/layerDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/layerDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/layerDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/newFontDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/newFontDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/newGlyphDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/newGlyphDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/newGlyphDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/newGlyphDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/renameGlyphDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/renameGlyphDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/renameGlyphDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/renameGlyphDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/revertFontDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/revertFontDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/revertFontDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/revertFontDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/selectFontsDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/selectFontsDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/dialog/selectFontsDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/dialog/selectFontsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/document.py` & `wbpUFO-0.2.3/Lib/wbpUFO/document.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/__init__.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/anchor.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/anchor.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/base.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/base.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListCtrl.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/commandListCtrl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListDialog.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/commandListDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListDialogUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/commandListDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/composite.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/composite.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/contour.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/contour.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/guideline.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/guideline.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/layer.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/layer.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/metric.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/metric.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/misc.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/misc.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/parameter.py` & `wbpUFO-0.2.3/Lib/wbpUFO/glyphCommand/parameter.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewCanvas.py` & `wbpUFO-0.2.3/Lib/wbpUFO/panel/glyphViewCanvas.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewPanel.py` & `wbpUFO-0.2.3/Lib/wbpUFO/panel/glyphViewPanel.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewPanelUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/panel/glyphViewPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/template.py` & `wbpUFO-0.2.3/Lib/wbpUFO/template.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/__init__.py` & `wbpUFO-0.2.3/Lib/wbpUFO/toolbar/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/command.py` & `wbpUFO-0.2.3/Lib/wbpUFO/toolbar/command.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/editTool.py` & `wbpUFO-0.2.3/Lib/wbpUFO/toolbar/editTool.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/glyphLock.py` & `wbpUFO-0.2.3/Lib/wbpUFO/toolbar/glyphLock.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/glyphShow.py` & `wbpUFO-0.2.3/Lib/wbpUFO/toolbar/glyphShow.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/layer.py` & `wbpUFO-0.2.3/Lib/wbpUFO/toolbar/layer.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/markColor.py` & `wbpUFO-0.2.3/Lib/wbpUFO/toolbar/markColor.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/__init__.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/feature.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/feature.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoBase.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoBase.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCaretUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoCaretUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoClassificationUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoClassificationUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCodepageUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoCodepageUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoControl.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoControl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEncodingUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoEncodingUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingPS.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoHintingPS.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoHintingUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLegalUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoLegalUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLineUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoLineUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoMetricUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoMetricUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNameUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoNameUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNoteUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoNoteUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoValidator.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/fontInfoValidator.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/glyphGrid.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/glyphGrid.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/groups.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/groups.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/groupsStatusPanelUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/groupsStatusPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/hintPSlistCtrl.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/hintPSlistCtrl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/hintPSpanel.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/hintPSpanel.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/info.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/info.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/kerning.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/kerning.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/kerningStatusPanelUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/kerningStatusPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/stemPanelUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/stemPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/font/zonePanelUI.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/font/zonePanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/fontinfo/__init__.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/fontinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO/view/glyph.py` & `wbpUFO-0.2.3/Lib/wbpUFO/view/glyph.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO.egg-info/PKG-INFO` & `wbpUFO-0.2.3/Lib/wbpUFO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpUFO
-Version: 0.2.2
+Version: 0.2.3
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUFO
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUFO/-/issues
```

### Comparing `wbpUFO-0.2.2/Lib/wbpUFO.egg-info/SOURCES.txt` & `wbpUFO-0.2.3/Lib/wbpUFO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/PKG-INFO` & `wbpUFO-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpUFO
-Version: 0.2.2
+Version: 0.2.3
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUFO
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUFO/-/issues
```

### Comparing `wbpUFO-0.2.2/README.md` & `wbpUFO-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.2/setup.cfg` & `wbpUFO-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.2
+current_version = 0.2.3
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
```

