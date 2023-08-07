# Comparing `tmp/pyplotbrookings-0.2.tar.gz` & `tmp/pyplotbrookings-0.2.1.tar.gz`

## Comparing `pyplotbrookings-0.2.tar` & `pyplotbrookings-0.2.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/examples/.DS_Store
--rw-r--r--   0        0        0   282940 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/examples/Examples.ipynb
--rw-r--r--   0        0        0   870265 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/examples/Palettes.ipynb
--rw-r--r--   0        0        0   556797 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/examples/.ipynb_checkpoints/Examples-checkpoint.ipynb
--rw-r--r--   0        0        0    40685 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/figures/Figure1A.png
--rw-r--r--   0        0        0    94387 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/figures/Figure2.png
--rw-r--r--   0        0        0    32720 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/figures/Figure3.png
--rw-r--r--   0        0        0   105552 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/figures/cmaps1.png
--rw-r--r--   0        0        0    73751 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/figures/cmaps2.png
--rw-r--r--   0        0        0    26595 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/figures/cmaps3.png
--rw-r--r--   0        0        0    30774 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/figures/logo.png
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/.DS_Store
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/__init__.py
--rw-r--r--   0        0        0    20954 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/pyplotbrookings.py
--rw-r--r--   0        0        0   931903 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/.ipynb_checkpoints/Examples-checkpoint.ipynb
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/readme.html
--rw-r--r--   0        0        0    20100 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Black Condensed/Helvetica Black Condensed.otf
--rw-r--r--   0        0        0    20184 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Black Condensed Oblique/Helvetica Black Condensed Oblique.otf
--rw-r--r--   0        0        0    20004 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Condensed/Helvetica Bold Condensed.otf
--rw-r--r--   0        0        0    20108 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Condensed Oblique/Helvetica Bold Condensed Oblique.otf
--rw-r--r--   0        0        0    30648 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Italic/Helvetica Bold Italic.ttf
--rw-r--r--   0        0        0    17520 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Narrow Oblique/Helvetica Bold Narrow Oblique.otf
--rw-r--r--   0        0        0    49200 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica BoldOblique/Helvetica BoldOblique.ttf
--rw-r--r--   0        0        0    24324 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold/Helvetica CE Bold.otf
--rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Condensed/Helvetica CE Bold Condensed.otf
--rw-r--r--   0        0        0    22004 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Condensed Oblique/Helvetica CE Bold Condensed Oblique.otf
--rw-r--r--   0        0        0    24464 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Narrow/Helvetica CE Bold Narrow.otf
--rw-r--r--   0        0        0    24580 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Narrow Oblique/Helvetica CE Bold Narrow Oblique.otf
--rw-r--r--   0        0        0    24488 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Oblique/Helvetica CE Bold Oblique.otf
--rw-r--r--   0        0        0    20688 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Condensed Oblique/Helvetica CE Condensed Oblique.otf
--rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Medium/Helvetica CE Medium.otf
--rw-r--r--   0        0        0    20632 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Medium Condensed/Helvetica CE Medium Condensed.otf
--rw-r--r--   0        0        0    24348 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Narrow/Helvetica CE Narrow.otf
--rw-r--r--   0        0        0    24444 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Narrow Oblique/Helvetica CE Narrow Oblique.otf
--rw-r--r--   0        0        0    24348 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Oblique/Helvetica CE Oblique.otf
--rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Condensed Oblique/Helvetica Condensed Oblique.otf
--rw-r--r--   0        0        0    18800 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Light Condensed/Helvetica Light Condensed.otf
--rw-r--r--   0        0        0    18880 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Light Condensed Oblique/Helvetica Light Condensed Oblique.otf
--rw-r--r--   0        0        0    18908 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Medium Condensed/Helvetica Medium Condensed.otf
--rw-r--r--   0        0        0    50280 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Roman/Helvetica Roman.ttf
--rw-r--r--   0        0        0    50884 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica RomanItalic/Helvetica RomanItalic.ttf
--rw-r--r--   0        0        0    16748 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Ultra Compressed/Helvetica Ultra Compressed.otf
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/b_logo.png
--rw-r--r--   0        0        0    21136 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/bc.png
--rw-r--r--   0        0        0    12097 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/bi.png
--rw-r--r--   0        0        0    17913 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/brookings.png
--rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/cc.png
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/ccf.png
--rw-r--r--   0        0        0   101943 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/ceaps.png
--rw-r--r--   0        0        0    26494 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/cepm.png
--rw-r--r--   0        0        0    56387 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/chp.png
--rw-r--r--   0        0        0   107876 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/cmep.png
--rw-r--r--   0        0        0   107158 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/crm.png
--rw-r--r--   0        0        0    22586 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/csd.png
--rw-r--r--   0        0        0    93053 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/cti.png
--rw-r--r--   0        0        0    20197 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/cue.png
--rw-r--r--   0        0        0    96557 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/cuse.png
--rw-r--r--   0        0        0    14692 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/es.png
--rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/fp.png
--rw-r--r--   0        0        0    21605 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/global.png
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/gs.png
--rw-r--r--   0        0        0    47345 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/hc.png
--rw-r--r--   0        0        0    20101 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/metro.png
--rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/src/pyplotbrookings/logos/thp.png
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/LICENSE
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/pyproject.toml
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 pyplotbrookings-0.2/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/examples/.DS_Store
+-rw-r--r--   0        0        0   282940 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/examples/Examples.ipynb
+-rw-r--r--   0        0        0   870265 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/examples/Palettes.ipynb
+-rw-r--r--   0        0        0   556797 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/examples/.ipynb_checkpoints/Examples-checkpoint.ipynb
+-rw-r--r--   0        0        0    40685 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/figures/Figure1A.png
+-rw-r--r--   0        0        0    94387 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/figures/Figure2.png
+-rw-r--r--   0        0        0    32720 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/figures/Figure3.png
+-rw-r--r--   0        0        0   105552 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/figures/cmaps1.png
+-rw-r--r--   0        0        0    73751 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/figures/cmaps2.png
+-rw-r--r--   0        0        0    26595 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/figures/cmaps3.png
+-rw-r--r--   0        0        0    30774 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/figures/logo.png
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/.DS_Store
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/__init__.py
+-rw-r--r--   0        0        0    21210 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/pyplotbrookings.py
+-rw-r--r--   0        0        0   931903 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/.ipynb_checkpoints/Examples-checkpoint.ipynb
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/readme.html
+-rw-r--r--   0        0        0    20100 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Black Condensed/Helvetica Black Condensed.otf
+-rw-r--r--   0        0        0    20184 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Black Condensed Oblique/Helvetica Black Condensed Oblique.otf
+-rw-r--r--   0        0        0    20004 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Condensed/Helvetica Bold Condensed.otf
+-rw-r--r--   0        0        0    20108 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Condensed Oblique/Helvetica Bold Condensed Oblique.otf
+-rw-r--r--   0        0        0    30648 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Italic/Helvetica Bold Italic.ttf
+-rw-r--r--   0        0        0    17520 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Narrow Oblique/Helvetica Bold Narrow Oblique.otf
+-rw-r--r--   0        0        0    49200 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica BoldOblique/Helvetica BoldOblique.ttf
+-rw-r--r--   0        0        0    24324 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold/Helvetica CE Bold.otf
+-rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Condensed/Helvetica CE Bold Condensed.otf
+-rw-r--r--   0        0        0    22004 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Condensed Oblique/Helvetica CE Bold Condensed Oblique.otf
+-rw-r--r--   0        0        0    24464 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Narrow/Helvetica CE Bold Narrow.otf
+-rw-r--r--   0        0        0    24580 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Narrow Oblique/Helvetica CE Bold Narrow Oblique.otf
+-rw-r--r--   0        0        0    24488 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Oblique/Helvetica CE Bold Oblique.otf
+-rw-r--r--   0        0        0    20688 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Condensed Oblique/Helvetica CE Condensed Oblique.otf
+-rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Medium/Helvetica CE Medium.otf
+-rw-r--r--   0        0        0    20632 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Medium Condensed/Helvetica CE Medium Condensed.otf
+-rw-r--r--   0        0        0    24348 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Narrow/Helvetica CE Narrow.otf
+-rw-r--r--   0        0        0    24444 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Narrow Oblique/Helvetica CE Narrow Oblique.otf
+-rw-r--r--   0        0        0    24348 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Oblique/Helvetica CE Oblique.otf
+-rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Condensed Oblique/Helvetica Condensed Oblique.otf
+-rw-r--r--   0        0        0    18800 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Light Condensed/Helvetica Light Condensed.otf
+-rw-r--r--   0        0        0    18880 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Light Condensed Oblique/Helvetica Light Condensed Oblique.otf
+-rw-r--r--   0        0        0    18908 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Medium Condensed/Helvetica Medium Condensed.otf
+-rw-r--r--   0        0        0    50280 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Roman/Helvetica Roman.ttf
+-rw-r--r--   0        0        0    50884 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica RomanItalic/Helvetica RomanItalic.ttf
+-rw-r--r--   0        0        0    16748 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Ultra Compressed/Helvetica Ultra Compressed.otf
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/b_logo.png
+-rw-r--r--   0        0        0    21136 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/bc.png
+-rw-r--r--   0        0        0    12097 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/bi.png
+-rw-r--r--   0        0        0    17913 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/brookings.png
+-rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cc.png
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/ccf.png
+-rw-r--r--   0        0        0   101943 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/ceaps.png
+-rw-r--r--   0        0        0    26494 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cepm.png
+-rw-r--r--   0        0        0    56387 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/chp.png
+-rw-r--r--   0        0        0   107876 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cmep.png
+-rw-r--r--   0        0        0   107158 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/crm.png
+-rw-r--r--   0        0        0    22586 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/csd.png
+-rw-r--r--   0        0        0    93053 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cti.png
+-rw-r--r--   0        0        0    20197 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cue.png
+-rw-r--r--   0        0        0    96557 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cuse.png
+-rw-r--r--   0        0        0    14692 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/es.png
+-rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/fp.png
+-rw-r--r--   0        0        0    21605 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/global.png
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/gs.png
+-rw-r--r--   0        0        0    47345 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/hc.png
+-rw-r--r--   0        0        0    20101 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/metro.png
+-rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/src/pyplotbrookings/logos/thp.png
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7887 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 pyplotbrookings-0.2.1/PKG-INFO
```

### Comparing `pyplotbrookings-0.2/examples/.DS_Store` & `pyplotbrookings-0.2.1/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/examples/Examples.ipynb` & `pyplotbrookings-0.2.1/examples/Examples.ipynb`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/examples/Palettes.ipynb` & `pyplotbrookings-0.2.1/examples/Palettes.ipynb`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/examples/.ipynb_checkpoints/Examples-checkpoint.ipynb` & `pyplotbrookings-0.2.1/examples/.ipynb_checkpoints/Examples-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/figures/Figure1A.png` & `pyplotbrookings-0.2.1/figures/Figure1A.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/figures/Figure2.png` & `pyplotbrookings-0.2.1/figures/Figure2.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/figures/Figure3.png` & `pyplotbrookings-0.2.1/figures/Figure3.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/figures/cmaps1.png` & `pyplotbrookings-0.2.1/figures/cmaps1.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/figures/cmaps2.png` & `pyplotbrookings-0.2.1/figures/cmaps2.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/figures/cmaps3.png` & `pyplotbrookings-0.2.1/figures/cmaps3.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/figures/logo.png` & `pyplotbrookings-0.2.1/figures/logo.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/.DS_Store` & `pyplotbrookings-0.2.1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/.DS_Store` & `pyplotbrookings-0.2.1/src/pyplotbrookings/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/pyplotbrookings.py` & `pyplotbrookings-0.2.1/src/pyplotbrookings/pyplotbrookings.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,46 +45,51 @@
         'orange': ('#663205', '#994B08', '#B85B0A', '#EF6A00', '#FF851A', '#FF9E1B', '#FFB24D', '#FEC87F', '#FBD9A5'),
         'red': ('#660507', '#A00D11', '#CD1A1C', '#E22827', '#ED3A35', '#F75C57', '#F98B83', '#FCB0AA', '#FDD7D4'),
         'magenta': ('#510831', '#8D1655', '#A82168', '#BF317B', '#D2468E', '#E160A2', '#EC81B7', '#F5A8CF', '#FAD4E7'),
         'purple': ('#3E2C72', '#533C91', '#6A50AD', '#7C60BF', '#8E72D0', '#9C82D9', '#B59DEA', '#D0BEF5', '#E9E0FC'),
         'gray': ('#191919', '#404040', '#666666', '#757575', '#949494', '#B1B3B3', '#CCCCCC', '#E6E6E6', '#F2F2F2'),
     }
 
-def set_theme(font_size=12, line_width=1.4, web=False, font_family='Helvetica'):
+def set_theme(font_size=12, line_width=1.4, font_family='Helvetica', 
+              background_color='transparent'):
     '''
     Sets matplotlib default style parameters to be consistent with
     the Brookings style. 
 
     font_size (float): A number specifying the base font size of all 
         default plots
 
     line_width (float): A number specifying the default thickness of all
         lines in plots
-
-    web (bool): If the plot is for a website figure (the background color for 
-        the website is an off white requiring a different color)
-
+        
     font_family (str): The font family for figures (either Helvetica or Roboto)
+
+    background_color (str): The background color of the plot, specified as
+        a named color string (e.g., 'white') or hexcode (e.g., '#FFFFFF').
+        Defaults to a transparent plot background.
     '''
     # Reset matplotlib style parameters to the defaults
     mpl.rcdefaults()
-    # Setting the background color
-    background_color = '#FAFAFA' if web else '#FFFFFF'
+    
+    # Should the background plot be transparent
+    transparent = (background_color == 'transparent')
+    background_color = 'white' if transparent else background_color
 
     # Setting up Helvetica font
     cwd = os.path.join(os.path.dirname(__file__), 'fonts')
     font_files = font_manager.findSystemFonts(fontpaths=cwd, fontext="ttf")
 
     for font_file in font_files:
         font_manager.fontManager.addfont(font_file)
 
     # Dictionary of style features to set
     style_dict = {
         'axes.axisbelow': True,  # Place gride lines behind the plot
         'axes.facecolor': background_color,
+        'figure.facecolor': background_color,
 
         'axes.grid': True,
         'axes.grid.axis': 'y',
         'axes.labelsize': 0.833*font_size,
         'axes.labelweight': 'bold',
         'axes.linewidth': line_width,
         'axes.spines.left': False,
@@ -108,20 +113,23 @@
         'grid.color': '#CCCCCC',
         'grid.linestyle': (0, (1, 4)),
 
         'legend.loc': 'upper center',
         'legend.frameon': False,  # Remove legend border
         'legend.handlelength': 0.75,  # Shorten size of legend key
         'legend.borderaxespad': -1,  # Place legend outside the figure
+        'legend.fontsize': 0.833*font_size,
 
         'patch.linewidth': 0,
 
         'ytick.left': False,
         'ytick.labelsize': 0.833*font_size,
         'xtick.labelsize': 0.833*font_size,
+        
+        'savefig.transparent': transparent,
     }
     # Apply all styles
     for key, value in style_dict.items():
         mpl.rcParams[key] = value
 
 
 def get_palette(name, list_supported=False):
@@ -246,21 +254,22 @@
 
     if tag:
         y = get_coords('top')
         right = get_coords('right') - x
         # Adding the tag in a seprate subplot 
         # Figure annotations can be finicky so a new subplot is easiest way to add them   
         ax = plt.gcf().add_axes([x, y, right, 0.01], zorder=1)
-        ax.set_ylim(0.9, 1.25)
-        # Line at the top of th figure
-        ax.annotate('', xytext=(0, 1.25), xy=(1, 1.25), 
-                    arrowprops = dict(arrowstyle="-", linewidth=0.5, color='#666666'))
-        # Adding the tag annotation
-        text = ax.annotate(tag + '   ', (0, 1), fontsize=0.75*font_size, weight="light", color='#666666')
-        text.set_bbox(dict(facecolor='white'))
+        
+        
+        ax.set_ylim(0.9, 1.5)
+        # Adding the tag and line at the top of the figure
+        ax.annotate(tag + '   ', xytext=(0, 1.25), xy=(1, 1.5), 
+                    fontsize=0.75*font_size, weight="light", color='#666666',
+                    arrowprops=dict(arrowstyle="-", linewidth=0.5, color='#666666'))
+        
         # Turning off axis so only text is displayed
         ax.axis('off')
 
 
 def add_notes(*args, v_pad=-5, h_pad=0, text_pad=0):
     '''
     Adds footnotes to the current figure.
@@ -412,15 +421,15 @@
     colors = get_palette(name)
 
     # Reverse colors if needed
     if reverse:
         colors = colors[::-1]
 
     # Return a color map over the list of colors
-    return matplotlib.colors.LinearSegmentedColormap.from_list("", colors, **kargs)
+    return mpl.colors.LinearSegmentedColormap.from_list("", colors, **kargs)
 
 
 def set_palette(name, ax=None, reverse=False):
     '''
     Sets the a color palette cycler for the current axis
 
     name (str): Name of the Brookings color palette
@@ -491,15 +500,15 @@
     # Reshape the data into a 2D image
     data = np.arange(2*cols).reshape(2, cols)
     
     # Append white "squares" to the end of the color map 
     palette_extended = np.append(palette, np.repeat('#FFFFFF', len(palette) % 2))
     
     # Create a color map
-    cmap = matplotlib.colors.LinearSegmentedColormap.from_list("", palette_extended)
+    cmap = mpl.colors.LinearSegmentedColormap.from_list("", palette_extended)
     # Plot the image
     plt.imshow(data, cmap=cmap)
     
     # Counter for the order of the colors
     k = 0
     for i in range(data.shape[0]):
         for j in range(data.shape[1]):
```

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/.ipynb_checkpoints/Examples-checkpoint.ipynb` & `pyplotbrookings-0.2.1/src/pyplotbrookings/.ipynb_checkpoints/Examples-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/readme.html` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/readme.html`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Black Condensed/Helvetica Black Condensed.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Black Condensed/Helvetica Black Condensed.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Black Condensed Oblique/Helvetica Black Condensed Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Black Condensed Oblique/Helvetica Black Condensed Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Condensed/Helvetica Bold Condensed.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Condensed/Helvetica Bold Condensed.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Condensed Oblique/Helvetica Bold Condensed Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Condensed Oblique/Helvetica Bold Condensed Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Italic/Helvetica Bold Italic.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Italic/Helvetica Bold Italic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Narrow Oblique/Helvetica Bold Narrow Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Bold Narrow Oblique/Helvetica Bold Narrow Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica BoldOblique/Helvetica BoldOblique.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica BoldOblique/Helvetica BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold/Helvetica CE Bold.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold/Helvetica CE Bold.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Condensed/Helvetica CE Bold Condensed.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Condensed/Helvetica CE Bold Condensed.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Condensed Oblique/Helvetica CE Bold Condensed Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Condensed Oblique/Helvetica CE Bold Condensed Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Narrow/Helvetica CE Bold Narrow.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Narrow/Helvetica CE Bold Narrow.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Narrow Oblique/Helvetica CE Bold Narrow Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Narrow Oblique/Helvetica CE Bold Narrow Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Oblique/Helvetica CE Bold Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Bold Oblique/Helvetica CE Bold Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Condensed Oblique/Helvetica CE Condensed Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Condensed Oblique/Helvetica CE Condensed Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Medium/Helvetica CE Medium.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Medium/Helvetica CE Medium.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Medium Condensed/Helvetica CE Medium Condensed.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Medium Condensed/Helvetica CE Medium Condensed.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Narrow/Helvetica CE Narrow.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Narrow/Helvetica CE Narrow.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Narrow Oblique/Helvetica CE Narrow Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Narrow Oblique/Helvetica CE Narrow Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Oblique/Helvetica CE Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica CE Oblique/Helvetica CE Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Condensed Oblique/Helvetica Condensed Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Condensed Oblique/Helvetica Condensed Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Light Condensed/Helvetica Light Condensed.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Light Condensed/Helvetica Light Condensed.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Light Condensed Oblique/Helvetica Light Condensed Oblique.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Light Condensed Oblique/Helvetica Light Condensed Oblique.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Medium Condensed/Helvetica Medium Condensed.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Medium Condensed/Helvetica Medium Condensed.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Roman/Helvetica Roman.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Roman/Helvetica Roman.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica RomanItalic/Helvetica RomanItalic.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica RomanItalic/Helvetica RomanItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Helvetica/Helvetica Ultra Compressed/Helvetica Ultra Compressed.otf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Helvetica/Helvetica Ultra Compressed/Helvetica Ultra Compressed.otf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/LICENSE.txt` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Black.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-BlackItalic.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Bold.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-BoldItalic.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Italic.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Light.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-LightItalic.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Medium.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-MediumItalic.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Regular.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-Thin.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/fonts/Roboto/Roboto-ThinItalic.ttf` & `pyplotbrookings-0.2.1/src/pyplotbrookings/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/b_logo.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/b_logo.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/bc.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/bc.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/bi.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/bi.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/brookings.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/brookings.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/cc.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cc.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/ccf.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/ccf.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/ceaps.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/ceaps.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/cepm.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cepm.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/chp.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/chp.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/cmep.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cmep.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/crm.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/crm.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/csd.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/csd.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/cti.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cti.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/cue.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cue.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/cuse.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/cuse.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/es.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/es.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/fp.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/fp.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/global.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/global.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/gs.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/gs.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/hc.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/hc.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/metro.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/metro.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/src/pyplotbrookings/logos/thp.png` & `pyplotbrookings-0.2.1/src/pyplotbrookings/logos/thp.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/LICENSE` & `pyplotbrookings-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.2/README.md` & `pyplotbrookings-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 -   `figure()` creates a `matplotlib` figure in one of the standard 
     Brookings sizes.
 
 -   `save()` saves a figure in the Brookings advised dpi values depending
      on content type.
 
 ## Updates
-### Whats New?!
+### What's New?!
 - Plotting has been updated to be consistent with the new [Brand Guidelines](https://brookingsinstitution.sharepoint.com/sites/IBCommunications/SiteAssets/Forms/AllItems.aspx?id=%2Fsites%2FIBCommunications%2FSiteAssets%2FSitePages%2FCrea%2FVisual%2DIdentity%2DGuidelines%2D2023%5F07%5F07%2Epdf&parent=%2Fsites%2FIBCommunications%2FSiteAssets%2FSitePages%2FCrea).
 - New palettes, a color picker, and palette maker have been added!
     - Many palettes have been removed or renamed. If an older palette is critical all hope is not lost, just add it back in with `ppb.make_palette()`.
 -  New fonts and titles (Roboto is out, Helvetica is in!). Roboto is still included in this distribution if needed.
 -  As always please reach out if you find bugs or styling inconsistencies. Thank you so much!
 
 ## Contact
```

### Comparing `pyplotbrookings-0.2/pyproject.toml` & `pyplotbrookings-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyplotbrookings"
-version = "0.2"
+version = "0.2.1"
 authors = [
   { name="Adam Sedlak", email="asedlak@brookings.edu" },
 ]
 description = "A plotting package for the Brookings Institution"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyplotbrookings-0.2/PKG-INFO` & `pyplotbrookings-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotbrookings
-Version: 0.2
+Version: 0.2.1
 Summary: A plotting package for the Brookings Institution
 Project-URL: Homepage, https://github.com/Adam-Sedlak-Brookings/pyplotbrookings
 Author-email: Adam Sedlak <asedlak@brookings.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -73,15 +73,15 @@
 -   `figure()` creates a `matplotlib` figure in one of the standard 
     Brookings sizes.
 
 -   `save()` saves a figure in the Brookings advised dpi values depending
      on content type.
 
 ## Updates
-### Whats New?!
+### What's New?!
 - Plotting has been updated to be consistent with the new [Brand Guidelines](https://brookingsinstitution.sharepoint.com/sites/IBCommunications/SiteAssets/Forms/AllItems.aspx?id=%2Fsites%2FIBCommunications%2FSiteAssets%2FSitePages%2FCrea%2FVisual%2DIdentity%2DGuidelines%2D2023%5F07%5F07%2Epdf&parent=%2Fsites%2FIBCommunications%2FSiteAssets%2FSitePages%2FCrea).
 - New palettes, a color picker, and palette maker have been added!
     - Many palettes have been removed or renamed. If an older palette is critical all hope is not lost, just add it back in with `ppb.make_palette()`.
 -  New fonts and titles (Roboto is out, Helvetica is in!). Roboto is still included in this distribution if needed.
 -  As always please reach out if you find bugs or styling inconsistencies. Thank you so much!
 
 ## Contact
```

