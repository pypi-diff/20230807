# Comparing `tmp/microstructpy-1.5.6.tar.gz` & `tmp/microstructpy-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microstructpy-1.5.6.tar", last modified: Fri Sep  2 05:57:59 2022, max compression
+gzip compressed data, was "microstructpy-1.5.7.tar", last modified: Mon Aug  7 01:52:05 2023, max compression
```

## Comparing `microstructpy-1.5.6.tar` & `microstructpy-1.5.7.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.732161 microstructpy-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-02 05:57:48.000000 microstructpy-1.5.6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-02 05:57:48.000000 microstructpy-1.5.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8643 2022-09-02 05:57:48.000000 microstructpy-1.5.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-09-02 05:57:48.000000 microstructpy-1.5.6/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-09-02 05:57:48.000000 microstructpy-1.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7693 2022-09-02 05:57:59.732161 microstructpy-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6567 2022-09-02 05:57:48.000000 microstructpy-1.5.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.704160 microstructpy-1.5.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.704160 microstructpy-1.5.6/docs/publications/
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/publications/cmame2020.bib
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/publications/swx2020.bib
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.708160 microstructpy-1.5.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.708160 microstructpy-1.5.6/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.712161 microstructpy-1.5.6/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (121)   166269 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)   220912 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    20992 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_114x114.png
--rw-r--r--   0 runner    (1001) docker     (121)    22769 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_120x120.png
--rw-r--r--   0 runner    (1001) docker     (121)    24740 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_128x128.png
--rw-r--r--   0 runner    (1001) docker     (121)    29954 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)    41275 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_180x180.png
--rw-r--r--   0 runner    (1001) docker     (121)    40240 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_192x192.png
--rw-r--r--   0 runner    (1001) docker     (121)    41511 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_196x196.png
--rw-r--r--   0 runner    (1001) docker     (121)    50396 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_228x228.png
--rw-r--r--   0 runner    (1001) docker     (121)     3480 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)     7623 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_57x57.png
--rw-r--r--   0 runner    (1001) docker     (121)    11158 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_72x72.png
--rw-r--r--   0 runner    (1001) docker     (121)    12266 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_76x76.png
--rw-r--r--   0 runner    (1001) docker     (121)    16209 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/logo_96x96.png
--rw-r--r--   0 runner    (1001) docker     (121)   201850 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/pad_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)   249032 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/pad_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    49494 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_static/logo/social.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.712161 microstructpy-1.5.6/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     3790 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.712161 microstructpy-1.5.6/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/cli.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.716161 microstructpy-1.5.6/docs/source/api/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/box.rst
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/circle.rst
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/cube.rst
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/ellipse.rst
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/ellipsoid.rst
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/factory.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/n_box.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/n_sphere.rst
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/rectangle.rst
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/sphere.rst
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/geometry/square.rst
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.716161 microstructpy-1.5.6/docs/source/api/meshing/
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/meshing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/meshing/polymesh.rst
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/meshing/rastermesh.rst
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/meshing/trimesh.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.716161 microstructpy-1.5.6/docs/source/api/seeding/
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/seeding/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/seeding/seed.rst
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/seeding/seedlist.rst
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/api/verification.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/changelog.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.716161 microstructpy-1.5.6/docs/source/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     8000 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/cli/domain.rst
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/cli/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)    18169 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/cli/material.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14248 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/cli/settings.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8281 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/docutils.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.716161 microstructpy-1.5.6/docs/source/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.720161 microstructpy-1.5.6/docs/source/examples/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     3133 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/cli/basalt.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/cli/colormap.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/cli/elliptical_grains.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/cli/minimal.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/cli/two_phase_3d.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4179 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.720161 microstructpy-1.5.6/docs/source/examples/intro/
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/intro/intro_1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/intro/intro_2.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/intro/intro_3.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/intro/intro_4.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/intro/intro_5.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/intro/intro_6.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.720161 microstructpy-1.5.6/docs/source/examples/package/
--rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/package/foam.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/package/from_image.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/package/grain_neighborhoods.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/package/logo.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3290 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/package/mesh_process.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/package/standard_voronoi.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/examples/package/uniform_seeding.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7011 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/file_formats.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8687 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/package_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.720161 microstructpy-1.5.6/docs/source/sphinx_gallery/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/sphinx_gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.720161 microstructpy-1.5.6/docs/source/sphinx_gallery/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/sphinx_gallery/geometry/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/sphinx_gallery/geometry/plot_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/sphinx_gallery/geometry/plot_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/sphinx_gallery/plot_demos.py
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-09-02 05:57:48.000000 microstructpy-1.5.6/docs/source/welcome.rst
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-09-02 05:57:48.000000 microstructpy-1.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-09-02 05:57:59.732161 microstructpy-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2972 2022-09-02 05:57:48.000000 microstructpy-1.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.700160 microstructpy-1.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.724161 microstructpy-1.5.6/src/microstructpy/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5532 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    45567 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.728161 microstructpy-1.5.6/src/microstructpy/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    12266 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/aluminum_micro.png
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/aphanitic_cdf.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4233 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/basalt_circle.xml
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/colormap.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/docs_banner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/elliptical_grains.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/foam.py
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/from_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3277 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/grain_neighborhoods.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/intro_1_basic.xml
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/intro_2_quality.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/intro_3_size_shape.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/intro_4_oriented.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/intro_5_plotting.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/intro_6_culmination.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5550 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/logo.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/minimal.xml
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/minimal_paired.xml
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/olivine_cdf.csv
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/standard_voronoi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/two_phase_3D.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/examples/uniform_seeding.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.728161 microstructpy-1.5.6/src/microstructpy/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/geometry/box.py
--rw-r--r--   0 runner    (1001) docker     (121)     6590 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/geometry/circle.py
--rw-r--r--   0 runner    (1001) docker     (121)    25014 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/geometry/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (121)    33330 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/geometry/ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (121)     7545 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/geometry/n_box.py
--rw-r--r--   0 runner    (1001) docker     (121)    10468 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/geometry/n_sphere.py
--rw-r--r--   0 runner    (1001) docker     (121)    18345 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/geometry/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (121)     6971 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/geometry/sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.728161 microstructpy-1.5.6/src/microstructpy/meshing/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/meshing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    52817 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/meshing/polymesh.py
--rw-r--r--   0 runner    (1001) docker     (121)    80831 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/meshing/trimesh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.728161 microstructpy-1.5.6/src/microstructpy/seeding/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/seeding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13882 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/seeding/seed.py
--rw-r--r--   0 runner    (1001) docker     (121)    49028 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/seeding/seedlist.py
--rw-r--r--   0 runner    (1001) docker     (121)    41458 2022-09-02 05:57:48.000000 microstructpy-1.5.6/src/microstructpy/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.732161 microstructpy-1.5.6/src/microstructpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5251 2022-09-02 05:57:59.000000 microstructpy-1.5.6/src/microstructpy.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.728161 microstructpy-1.5.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.728161 microstructpy-1.5.6/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tests/cli/test_includes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.732161 microstructpy-1.5.6/tests/cli/test_includes_files/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.732161 microstructpy-1.5.6/tests/cli/test_includes_files/different_dir/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tests/cli/test_includes_files/different_dir/input.xml
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tests/cli/test_includes_files/expected_input.xml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tests/cli/test_includes_files/fine_grained.xml
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tests/cli/test_includes_files/input.xml
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tests/cli/test_includes_files/materials.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.732161 microstructpy-1.5.6/tests/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tests/geometry/test_n_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 05:57:59.732161 microstructpy-1.5.6/tests/meshing/
--rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tests/meshing/test_polymesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-09-02 05:57:48.000000 microstructpy-1.5.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-07 01:51:55.000000 microstructpy-1.5.7/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-07 01:51:55.000000 microstructpy-1.5.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-08-07 01:51:55.000000 microstructpy-1.5.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-07 01:51:55.000000 microstructpy-1.5.7/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-07 01:51:55.000000 microstructpy-1.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-08-07 01:52:05.114379 microstructpy-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-08-07 01:51:55.000000 microstructpy-1.5.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.098379 microstructpy-1.5.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.098379 microstructpy-1.5.7/docs/publications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/publications/cmame2020.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/publications/swx2020.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.098379 microstructpy-1.5.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.098379 microstructpy-1.5.7/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.102379 microstructpy-1.5.7/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   166269 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   220912 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_114x114.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22769 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24740 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29954 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41275 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_180x180.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40240 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_196x196.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50396 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_228x228.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_57x57.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_72x72.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_76x76.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/logo_96x96.png
+-rw-r--r--   0 runner    (1001) docker     (123)   201850 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/pad_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   249032 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/pad_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    49494 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_static/logo/social.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.102379 microstructpy-1.5.7/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.102379 microstructpy-1.5.7/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/cli.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.102379 microstructpy-1.5.7/docs/source/api/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/box.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/circle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/cube.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/ellipse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/ellipsoid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/n_box.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/n_sphere.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/rectangle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/sphere.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/geometry/square.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.102379 microstructpy-1.5.7/docs/source/api/meshing/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/meshing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/meshing/polymesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/meshing/rastermesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/meshing/trimesh.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.106379 microstructpy-1.5.7/docs/source/api/seeding/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/seeding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/seeding/seed.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/seeding/seedlist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/api/verification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/changelog.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.106379 microstructpy-1.5.7/docs/source/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/cli/domain.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/cli/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/cli/material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/cli/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/docutils.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.106379 microstructpy-1.5.7/docs/source/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.106379 microstructpy-1.5.7/docs/source/examples/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/cli/basalt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/cli/colormap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/cli/elliptical_grains.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/cli/minimal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/cli/two_phase_3d.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.106379 microstructpy-1.5.7/docs/source/examples/intro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/intro/intro_1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/intro/intro_2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/intro/intro_3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/intro/intro_4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/intro/intro_5.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/intro/intro_6.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.106379 microstructpy-1.5.7/docs/source/examples/package/
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/package/foam.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/package/from_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/package/grain_neighborhoods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/package/logo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/package/mesh_process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/package/standard_voronoi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/examples/package/uniform_seeding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/file_formats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/package_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.106379 microstructpy-1.5.7/docs/source/sphinx_gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/sphinx_gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.106379 microstructpy-1.5.7/docs/source/sphinx_gallery/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/sphinx_gallery/geometry/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/sphinx_gallery/geometry/plot_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/sphinx_gallery/geometry/plot_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/sphinx_gallery/plot_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-08-07 01:51:55.000000 microstructpy-1.5.7/docs/source/welcome.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-07 01:51:55.000000 microstructpy-1.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-07 01:52:05.118379 microstructpy-1.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-07 01:51:55.000000 microstructpy-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.094379 microstructpy-1.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.106379 microstructpy-1.5.7/src/microstructpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45747 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.110379 microstructpy-1.5.7/src/microstructpy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/aluminum_micro.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/aphanitic_cdf.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/basalt_circle.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/colormap.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/docs_banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/elliptical_grains.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/foam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/from_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/grain_neighborhoods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/intro_1_basic.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/intro_2_quality.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/intro_3_size_shape.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/intro_4_oriented.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/intro_5_plotting.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/intro_6_culmination.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/minimal.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/minimal_paired.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/olivine_cdf.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/standard_voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/two_phase_3D.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/examples/uniform_seeding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/src/microstructpy/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/geometry/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/geometry/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25014 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/geometry/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33340 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/geometry/ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/geometry/n_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/geometry/n_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/geometry/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/geometry/sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/src/microstructpy/meshing/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/meshing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52869 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/meshing/polymesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80857 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/meshing/trimesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/src/microstructpy/seeding/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/seeding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13882 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/seeding/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/seeding/seedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41458 2023-08-07 01:51:55.000000 microstructpy-1.5.7/src/microstructpy/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/src/microstructpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-08-07 01:52:05.000000 microstructpy-1.5.7/src/microstructpy.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tests/cli/test_includes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/tests/cli/test_includes_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/tests/cli/test_includes_files/different_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tests/cli/test_includes_files/different_dir/input.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tests/cli/test_includes_files/expected_input.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tests/cli/test_includes_files/fine_grained.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tests/cli/test_includes_files/input.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tests/cli/test_includes_files/materials.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/tests/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tests/geometry/test_n_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:52:05.114379 microstructpy-1.5.7/tests/meshing/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tests/meshing/test_polymesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-07 01:51:55.000000 microstructpy-1.5.7/tox.ini
```

### Comparing `microstructpy-1.5.6/CHANGELOG.rst` & `microstructpy-1.5.7/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
+`1.5.7`_ - 2023-08-06
+--------------------------
+Fixed
+'''''''
+- Errors associated with using keyword arguments in ``plt.gca()`` deprecated in matplotlib 3.4.
+- 3D plots now use matplotlib standard for setting equal aspect ratios.
+
+
 `1.5.6`_ - 2022-09-01
 --------------------------
 Fixed
 '''''''
 - Bug in RasterMesh VTK writer.
 
 `1.5.5`_ - 2022-08-31
@@ -288,15 +296,16 @@
 '''''
 - Project added to GitHub.
 
 
 
 .. LINKS
 
-.. _`Unreleased`: https://github.com/kip-hart/MicroStructPy/compare/v1.5.6...HEAD
+.. _`Unreleased`: https://github.com/kip-hart/MicroStructPy/compare/v1.5.7...HEAD
+.. _`1.5.7`: https://github.com/kip-hart/MicroStructPy/compare/v1.5.6...v1.5.7
 .. _`1.5.6`: https://github.com/kip-hart/MicroStructPy/compare/v1.5.5...v1.5.6
 .. _`1.5.5`: https://github.com/kip-hart/MicroStructPy/compare/v1.5.4...v1.5.5
 .. _`1.5.4`: https://github.com/kip-hart/MicroStructPy/compare/v1.5.3...v1.5.4
 .. _`1.5.3`: https://github.com/kip-hart/MicroStructPy/compare/v1.5.2...v1.5.3
 .. _`1.5.2`: https://github.com/kip-hart/MicroStructPy/compare/v1.5.1...v1.5.2
 .. _`1.5.1`: https://github.com/kip-hart/MicroStructPy/compare/v1.5.0...v1.5.1
 .. _`1.5.0`: https://github.com/kip-hart/MicroStructPy/compare/v1.4.10...v1.5.0
```

### Comparing `microstructpy-1.5.6/LICENSE.rst` & `microstructpy-1.5.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/MANIFEST.in` & `microstructpy-1.5.7/MANIFEST.in`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 graft tests
 
 include .azure-pipelines.yml
 include .bumpversion.cfg
 include .coveragerc
 include .editorconfig
 include .pyup.yml
-include .readthedocs.yml
+include .readthedocs.yaml
 
 include CHANGELOG.rst
 include LICENSE.rst
 include README.rst
 
 include tox.ini
 include requirements.txt
```

### Comparing `microstructpy-1.5.6/PKG-INFO` & `microstructpy-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microstructpy
-Version: 1.5.6
+Version: 1.5.7
 Summary: Microstructure modeling, mesh generation, analysis, and visualization.
 Home-page: https://github.com/kip-hart/MicroStructPy
 Author: Kenneth (Kip) Hart
 Author-email: kiphart91@gmail.com
 License: MIT License
 Project-URL: Documentation, https://docs.microstructpy.org
 Keywords: microstructure,micromechanics,finite element,FEM,FEA,mesh,polycrystal,tessellation,Laguerre tessellation,multi-sphere
```

### Comparing `microstructpy-1.5.6/README.rst` & `microstructpy-1.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/publications/cmame2020.bib` & `microstructpy-1.5.7/docs/publications/cmame2020.bib`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/publications/swx2020.bib` & `microstructpy-1.5.7/docs/publications/swx2020.bib`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/favicon.ico` & `microstructpy-1.5.7/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo.svg` & `microstructpy-1.5.7/docs/source/_static/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_114x114.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_114x114.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_120x120.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_120x120.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_128x128.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_128x128.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_144x144.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_144x144.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_180x180.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_180x180.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_192x192.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_192x192.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_196x196.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_196x196.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_228x228.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_228x228.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_32x32.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_32x32.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_57x57.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_57x57.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_72x72.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_72x72.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_76x76.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_76x76.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/logo_96x96.png` & `microstructpy-1.5.7/docs/source/_static/logo/logo_96x96.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/pad_logo.png` & `microstructpy-1.5.7/docs/source/_static/logo/pad_logo.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/pad_logo.svg` & `microstructpy-1.5.7/docs/source/_static/logo/pad_logo.svg`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_static/logo/social.png` & `microstructpy-1.5.7/docs/source/_static/logo/social.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/_templates/layout.html` & `microstructpy-1.5.7/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/api/geometry/index.rst` & `microstructpy-1.5.7/docs/source/api/geometry/index.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/cli/domain.rst` & `microstructpy-1.5.7/docs/source/cli/domain.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/cli/introduction.rst` & `microstructpy-1.5.7/docs/source/cli/introduction.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/cli/material.rst` & `microstructpy-1.5.7/docs/source/cli/material.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/cli/settings.rst` & `microstructpy-1.5.7/docs/source/cli/settings.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/conf.py` & `microstructpy-1.5.7/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
 import os
 import sys
 sys.path.insert(0, os.path.abspath('../../src/'))
-sys.path.insert(0, os.path.abspath('../../src/MicroStructPy/'))
-
+sys.path.insert(0, os.path.abspath('../../src/microstructpy/'))
 import sphinx_gallery
-
 import microstructpy
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'MicroStructPy'
-copyright = '2019-2022, Georgia Tech Research Corporation'
+copyright = '2019-2023, Georgia Tech Research Corporation'
 author = 'Kenneth Hart'
 
 # The short X.Y version
 version = ''.join(microstructpy.__version__.split('.')[:2])
 # The full version, including alpha/beta/rc tags
 release = microstructpy.__version__
 
@@ -134,15 +132,15 @@
 # documentation.
 #
 html_theme_options = {
     'logo': 'logo/pad_logo.svg',
     'logo_name': True,
     'sidebar_width': '230px',
     'description': 'Microstructure modeling, mesh generation, analysis, and visualization.',
-    'analytics_id': 'UA-147258715-1',
+    'analytics_id': 'G-TK7PBETHC0',
     'code_font_size': '12.5px',
 }
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 html_title = 'MicroStructPy'
```

### Comparing `microstructpy-1.5.6/docs/source/examples/cli/basalt.rst` & `microstructpy-1.5.7/docs/source/examples/cli/basalt.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/cli/colormap.rst` & `microstructpy-1.5.7/docs/source/examples/cli/colormap.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/cli/elliptical_grains.rst` & `microstructpy-1.5.7/docs/source/examples/cli/elliptical_grains.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/cli/minimal.rst` & `microstructpy-1.5.7/docs/source/examples/cli/minimal.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/cli/two_phase_3d.rst` & `microstructpy-1.5.7/docs/source/examples/cli/two_phase_3d.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/index.rst` & `microstructpy-1.5.7/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/intro/intro_1.rst` & `microstructpy-1.5.7/docs/source/examples/intro/intro_1.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/intro/intro_2.rst` & `microstructpy-1.5.7/docs/source/examples/intro/intro_2.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/intro/intro_3.rst` & `microstructpy-1.5.7/docs/source/examples/intro/intro_3.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/intro/intro_4.rst` & `microstructpy-1.5.7/docs/source/examples/intro/intro_4.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/intro/intro_5.rst` & `microstructpy-1.5.7/docs/source/examples/intro/intro_5.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/intro/intro_6.rst` & `microstructpy-1.5.7/docs/source/examples/intro/intro_6.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/package/foam.rst` & `microstructpy-1.5.7/docs/source/examples/package/foam.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/package/from_image.rst` & `microstructpy-1.5.7/docs/source/examples/package/from_image.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/package/grain_neighborhoods.rst` & `microstructpy-1.5.7/docs/source/examples/package/grain_neighborhoods.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/package/logo.rst` & `microstructpy-1.5.7/docs/source/examples/package/logo.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/package/mesh_process.rst` & `microstructpy-1.5.7/docs/source/examples/package/mesh_process.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/package/standard_voronoi.rst` & `microstructpy-1.5.7/docs/source/examples/package/standard_voronoi.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/examples/package/uniform_seeding.rst` & `microstructpy-1.5.7/docs/source/examples/package/uniform_seeding.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/file_formats.rst` & `microstructpy-1.5.7/docs/source/file_formats.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/getting_started.rst` & `microstructpy-1.5.7/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/package_guide.rst` & `microstructpy-1.5.7/docs/source/package_guide.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/sphinx_gallery/geometry/plot_ellipse.py` & `microstructpy-1.5.7/docs/source/sphinx_gallery/geometry/plot_ellipse.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 
 
 def breakdown():
     a = 3
     b = 1
     x1 = 0.7
 
-    plt.figure(figsize=(14, 6))
+    fig = plt.figure(figsize=(14, 6))
     ellipse = msp.geometry.Ellipse(a=a, b=b)
     approx = ellipse.approximate(x1)
     ellipse.plot(edgecolor='k', facecolor='none', lw=3)
     t = np.linspace(0, 2 * np.pi)
     for x, y, r in approx:
         plt.plot(x + r * np.cos(t), y + r * np.sin(t), 'b')
     
     xticks = np.unique(np.concatenate((approx[:, 0], (-a, a))))
     plt.xticks(xticks)
     plt.yticks(np.unique(np.concatenate((approx[:, 1], (-b, b)))))
     plt.gca().set_xticklabels([str(round(float(label), 1)) for label in xticks])
     plt.axis('scaled')
     plt.grid(True, linestyle=':')
+    plt.tight_layout()
 
 
 if __name__ == '__main__':
-    plt.rc('savefig', dpi=300, bbox='tight', pad_inches=0)
+    plt.rc('savefig', dpi=300, pad_inches=0)
     main()
```

### Comparing `microstructpy-1.5.6/docs/source/sphinx_gallery/geometry/plot_rectangle.py` & `microstructpy-1.5.7/docs/source/sphinx_gallery/geometry/plot_rectangle.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def breakdown(length, width, x1, figsize):
     r = msp.geometry.Rectangle(length=length, width=width)
     approx = r.approximate(x1=x1)
 
     # Plot rectangle
-    plt.figure(figsize=figsize)
+    fig = plt.figure(figsize=figsize)
     r.plot(edgecolor='k', facecolor='none', lw=3)
 
     # Plot breakdown
     t = np.linspace(0, 2 * np.pi)
     xp = np.cos(t)
     yp = np.sin(t)
     for x, y, radius in approx:
@@ -34,12 +34,13 @@
     xtick = np.unique([circ[0] for circ in approx])
     ytick = np.unique([circ[1] for circ in approx])
     plt.xticks(xtick)
     plt.yticks(ytick)
 
     plt.axis('scaled')
     plt.grid(True, linestyle=':')
+    plt.tight_layout()
 
 
 if __name__ == '__main__':
-    plt.rc('savefig', dpi=300, bbox='tight', pad_inches=0)
+    plt.rc('savefig', dpi=300, pad_inches=0)
     main()
```

### Comparing `microstructpy-1.5.6/docs/source/sphinx_gallery/plot_demos.py` & `microstructpy-1.5.7/docs/source/sphinx_gallery/plot_demos.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 
         ax.set_axis_off()
         ax.get_xaxis().set_visible(False)
         ax.get_yaxis().set_visible(False)
 
     sub_fname = 'welcome_examples.png'
     sub_filename = os.path.join(example_dir, sub_fname)
-    plt.savefig(sub_filename, pad_inches=0, bbox_inches='tight', dpi=200)
+    plt.tight_layout()
+    plt.savefig(sub_filename, pad_inches=0, dpi=200)
     plt.close('all')
 
 
 def seed_poly_tri(filepath):
     basenames = ['seeds.png', 'polymesh.png', 'trimesh.png']
     ex_path = os.path.join(example_dir, filepath)
     fig, axes = plt.subplots(1, 3, figsize=(20, 10))
@@ -88,15 +89,16 @@
 
         ax.set_axis_off()
         ax.get_xaxis().set_visible(False)
         ax.get_yaxis().set_visible(False)
     
     sub_fname = 'joined.png'
     sub_filename = os.path.join(ex_path, sub_fname)
-    plt.savefig(sub_filename, pad_inches=0, bbox_inches='tight', dpi=300)
+    plt.tight_layout()
+    plt.savefig(sub_filename, pad_inches=0, dpi=300)
     plt.close('all')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `microstructpy-1.5.6/docs/source/troubleshooting.rst` & `microstructpy-1.5.7/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/docs/source/welcome.rst` & `microstructpy-1.5.7/docs/source/welcome.rst`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/setup.py` & `microstructpy-1.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         'Laguerre tessellation',
         'multi-sphere'
     ],
     install_requires=[
         'aabbtree>=2.5.0',
         'pybind11',  # must come before meshpy for successful install
         'lsq-ellipse',
-        'matplotlib>=3.3.0',
+        'matplotlib>=3.4.0',
         'meshpy>=2018.2.1',
         'numpy>=1.13.0',
         'pygmsh>=7.0.2',
         'pyquaternion',
         'pyvoro-mmalahe',  # install issue with pyvoro
         'scipy',
         'xmltodict'
```

### Comparing `microstructpy-1.5.6/src/microstructpy/_misc.py` & `microstructpy-1.5.7/src/microstructpy/_misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,22 +152,15 @@
 
     # return results
     spheres = np.hstack((posc, rc.reshape(-1, 1)))
     return np.squeeze(spheres)
 
 
 def axisEqual3D(ax):
-    '''From stackoverflow: https://stackoverflow.com/a/19248731'''
-    extents = np.array([getattr(ax, 'get_{}lim'.format(d))() for d in 'xyz'])
-    sz = extents[:, 1] - extents[:, 0]
-    centers = np.mean(extents, axis=1)
-    maxsize = max(abs(sz))
-    r = maxsize/2
-    for ctr, dim in zip(centers, 'xyz'):
-        getattr(ax, 'set_{}lim'.format(dim))(ctr - r, ctr + r)
+    ax.set_aspect('equal')
 
 
 def ax_objects(ax):
     n = 0
     for att in ['collections', 'images', 'lines', 'patches', 'texts']:
         n += len(getattr(ax, att))
     return n
```

### Comparing `microstructpy-1.5.6/src/microstructpy/cli.py` & `microstructpy-1.5.7/src/microstructpy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -699,26 +699,26 @@
     seed_colors = _seed_colors(seeds, phases, color_by, colormap)
     n_dim = seeds[0].geometry.n_dim
 
     # Set up axes
     plt.clf()
     plt.close('all')
     fig = plt.figure()
-    ax = fig.gca(projection={2: None, 3: Axes3D.name}[n_dim], label='seeds')
+    ax = fig.add_subplot(projection={2: None, 3: Axes3D.name}[n_dim], label='seeds')
 
     if not plot_axes:
         if n_dim == 2:
             ax.set_axis_off()
             ax.get_xaxis().set_visible(False)
             ax.get_yaxis().set_visible(False)
         else:
             ax._axis3don = False
 
     # Plot seeds
-    edge_kwargs.setdefault('edgecolors', {2: 'k', 3: 'none'}[n_dim])
+    edge_kwargs.setdefault('edgecolors', {2: 'k', 3: None}[n_dim])
     if given_names and color_by == 'material':
         seeds.plot(material=phase_names, facecolors=seed_colors, loc=4,
                    **edge_kwargs)
     else:
         seeds.plot(facecolors=seed_colors, **edge_kwargs)
 
     # Crop to Domain
@@ -733,16 +733,17 @@
         plt.gca().set_zlim(d_lims[2])
 
         _misc.axisEqual3D(plt.gca())
 
     # Save plot
     for fname in plot_files:
         if n_dim == 3:
-            fig.subplots_adjust(**_misc.plt_3d_adj)
-            plt.savefig(fname, bbox_inches='tight', pad_inches=0.15)
+            _misc.axisEqual3D(ax)
+            plt.subplots_adjust(left=0, bottom=.05, right=1, top=1, wspace=0, hspace=0)
+            plt.savefig(fname)
         else:
             plt.savefig(fname, bbox_inches='tight', pad_inches=0)
 
     plt.close('all')
 
 
 def _seed_colors(seeds, phases, color_by='material', colormap='viridis'):
@@ -819,15 +820,15 @@
         phase_colors.append(color)
         phase_names.append(name)
 
     # Set up axes
     plt.clf()
     plt.close('all')
     fig = plt.figure()
-    ax = fig.gca(projection={2: None, 3: Axes3D.name}[n_dim], label='poly')
+    ax = fig.add_subplot(projection={2: None, 3: Axes3D.name}[n_dim], label='poly')
 
     if not plot_axes:
         if n_dim == 2:
             ax.set_axis_off()
             ax.get_xaxis().set_visible(False)
             ax.get_yaxis().set_visible(False)
         else:
@@ -858,17 +859,19 @@
                        **edge_kwargs)
         else:
             pmesh.plot(facecolors=fcs, index_by='seed', **edge_kwargs)
 
     # save plot
     for fname in plot_files:
         if n_dim == 3:
-            fig.subplots_adjust(**_misc.plt_3d_adj)
-            plt.savefig(fname, bbox_inches='tight', pad_inches=0.15)
+            _misc.axisEqual3D(ax)
+            plt.subplots_adjust(left=0, bottom=.05, right=1, top=1, wspace=0, hspace=0)
+            plt.savefig(fname)
         else:
+            plt.tight_layout()
             plt.savefig(fname, bbox_inches='tight', pad_inches=0)
     plt.close('all')
 
 
 def _poly_colors(pmesh, phases, color_by, colormap, n_dim):
     if n_dim == 2:
         if color_by == 'material':
@@ -953,15 +956,15 @@
         if 'name' in phase:
             given_names = True
 
     # Set up axes
     plt.clf()
     plt.close('all')
     fig = plt.figure()
-    ax = fig.gca(projection={2: None, 3: Axes3D.name}[n_dim], label='tri')
+    ax = fig.add_subplot(projection={2: None, 3: Axes3D.name}[n_dim], label='tri')
 
     if not plot_axes:
         if n_dim == 2:
             ax.set_axis_off()
             ax.get_xaxis().set_visible(False)
             ax.get_yaxis().set_visible(False)
         else:
@@ -1034,17 +1037,19 @@
     else:
         fcs = {2: seed_colors, 3: facet_colors}[n_dim]
         tmesh.plot(facecolors=fcs, index_by='attribute', **edge_kwargs)
 
     # save plot
     for fname in plot_files:
         if n_dim == 3:
-            fig.subplots_adjust(**_misc.plt_3d_adj)
-            plt.savefig(fname, bbox_inches='tight', pad_inches=0.15)
+            _misc.axisEqual3D(ax)
+            plt.subplots_adjust(left=0, bottom=.05, right=1, top=1, wspace=0, hspace=0)
+            plt.savefig(fname)
         else:
+            plt.tight_layout()
             plt.savefig(fname, bbox_inches='tight', pad_inches=0)
 
     plt.close('all')
 
 
 def _f_plottable(n_pair, vis, invis):
     if set(n_pair) <= vis or set(n_pair) <= invis:
```

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/aluminum_micro.png` & `microstructpy-1.5.7/src/microstructpy/examples/aluminum_micro.png`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/aphanitic_cdf.csv` & `microstructpy-1.5.7/src/microstructpy/examples/aphanitic_cdf.csv`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/basalt_circle.xml` & `microstructpy-1.5.7/src/microstructpy/examples/basalt_circle.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/colormap.xml` & `microstructpy-1.5.7/src/microstructpy/examples/colormap.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/docs_banner.py` & `microstructpy-1.5.7/src/microstructpy/examples/docs_banner.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                                               max_edge_length=0.2,
                                               max_volume=0.4)
 
     # Create Figure
     k = 0.12
     len_x = 3 * domain.length + 4 * off
     len_y = domain.width + 2 * off
-    plt.figure(figsize=(k * len_x, k * len_y))
+    fig = plt.figure(figsize=(k * len_x, k * len_y))
 
     # Plot Seeds
     seed_colors = [phases[s.phase]['color'] for s in seeds]
     seeds.plot(color=seed_colors, alpha=0.8, edgecolor='k', linewidth=0.3)
     domain.plot(facecolor='none', edgecolor='k', linewidth=0.3)
 
     # Plot Polygonal Mesh
@@ -119,16 +119,16 @@
 
     ylim[0] -= off
     ylim[1] += off
 
     plt.axis(list(xlim) + list(ylim))
 
     fname = os.path.join(dirname, 'banner.png')
-    plt.savefig(fname, bbox='tight', pad_inches=0)
-    plt.savefig(fname.replace('.png', '.pdf'), bbox='tight', pad_inches=0)
+    plt.savefig(fname, bbox_inches='tight', pad_inches=0)
+    plt.savefig(fname.replace('.png', '.pdf'), bbox_inches='tight', pad_inches=0)
 
 
 def ordered_kps(pairs):
     t_pairs = [tuple(p) for p in pairs]
     kps = list(t_pairs.pop())
     while t_pairs:
         for i, pair in enumerate(t_pairs):
```

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/elliptical_grains.xml` & `microstructpy-1.5.7/src/microstructpy/examples/elliptical_grains.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/foam.py` & `microstructpy-1.5.7/src/microstructpy/examples/foam.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/from_image.py` & `microstructpy-1.5.7/src/microstructpy/examples/from_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             k_facets += 1
 
             if i + 1 < m:
                 facet_top[i + 1, j] = fnum_bottom
         else:
             fnum_bottom = facet_bottom[i, j]
 
-        # region
+        # update region
         region = (fnum_top, fnum_left, fnum_bottom, fnum_right)
         regions[k_regions] = region
         region_phases[k_regions] = bin_nums[i, j]
         k_regions += 1
 
 
 pmesh = msp.meshing.PolyMesh(pts, facets, regions,
```

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/grain_neighborhoods.py` & `microstructpy-1.5.7/src/microstructpy/examples/grain_neighborhoods.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/intro_1_basic.xml` & `microstructpy-1.5.7/src/microstructpy/examples/intro_1_basic.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/intro_2_quality.xml` & `microstructpy-1.5.7/src/microstructpy/examples/intro_2_quality.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/intro_3_size_shape.xml` & `microstructpy-1.5.7/src/microstructpy/examples/intro_3_size_shape.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/intro_4_oriented.xml` & `microstructpy-1.5.7/src/microstructpy/examples/intro_4_oriented.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/intro_5_plotting.xml` & `microstructpy-1.5.7/src/microstructpy/examples/intro_5_plotting.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/intro_6_culmination.xml` & `microstructpy-1.5.7/src/microstructpy/examples/intro_6_culmination.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/logo.py` & `microstructpy-1.5.7/src/microstructpy/examples/logo.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
                    horizontalalignment='center',
                    verticalalignment='center')
     ax_social.text(1, 0.23, 'Microstructure Mesh Generation in Python',
                    fontsize=10,
                    horizontalalignment='center',
                    verticalalignment='center')
     plt.draw()
-    plt.savefig(social_filename, bbox_inches='tight')
+    plt.savefig(social_filename, bbox_inches='tight', pad_inches=0)
     plt.close('all')
 
 
 if __name__ == '__main__':
     n_seeds = 14
     size_rng = 4
     pos_rng = 7
```

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/olivine_cdf.csv` & `microstructpy-1.5.7/src/microstructpy/examples/olivine_cdf.csv`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/standard_voronoi.py` & `microstructpy-1.5.7/src/microstructpy/examples/standard_voronoi.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/two_phase_3D.xml` & `microstructpy-1.5.7/src/microstructpy/examples/two_phase_3D.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/examples/uniform_seeding.py` & `microstructpy-1.5.7/src/microstructpy/examples/uniform_seeding.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/geometry/__init__.py` & `microstructpy-1.5.7/src/microstructpy/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/geometry/box.py` & `microstructpy-1.5.7/src/microstructpy/geometry/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,18 +90,18 @@
         :class:`mpl_toolkits.mplot3d.art3d.Poly3DCollection` to the current
         axes. The keyword arguments are passed through to the Poly3DCollection.
 
         Args:
             **kwargs (dict): Keyword arguments for Poly3DCollection.
 
         """  # NOQA: E501
-        if len(plt.gcf().axes) == 0:
-            ax = plt.axes(projection=Axes3D.name)
-        else:
+        if plt.gcf().axes:
             ax = plt.gca()
+        else:
+            ax = plt.gcf().add_subplot(projection=Axes3D.name)
 
         xlim, ylim, zlim = self.limits
 
         inds = [(0, 0), (0, 1), (1, 1), (1, 0)]
 
         # x faces
         f1 = np.array([(xlim[0], ylim[i], zlim[j]) for i, j in inds])
```

### Comparing `microstructpy-1.5.6/src/microstructpy/geometry/circle.py` & `microstructpy-1.5.7/src/microstructpy/geometry/circle.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/geometry/ellipse.py` & `microstructpy-1.5.7/src/microstructpy/geometry/ellipse.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/geometry/ellipsoid.py` & `microstructpy-1.5.7/src/microstructpy/geometry/ellipsoid.py`

 * *Files 0% similar despite different names*

```diff
@@ -714,26 +714,26 @@
 
     # ----------------------------------------------------------------------- #
     # Plot Function                                                           #
     # ----------------------------------------------------------------------- #
     def plot(self, **kwargs):
         """Plot the ellipsoid.
 
-        This function uses the :meth:`mpl_toolkits.mplot3d.Axes3D.plot_surface`
+        This function uses the :meth:`mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface`
         method to add an ellipsoid to the current axes. The keyword arguments
         are passes through to the plot_surface function.
 
         Args:
             **kwargs (dict): Keyword arguments for matplotlib.
 
         """  # NOQA: E501
-        if len(plt.gcf().axes) == 0:
-            ax = plt.axes(projection=Axes3D.name)
-        else:
+        if plt.gcf().axes:
             ax = plt.gca()
+        else:
+            ax = plt.gcf().add_subplot(projection=Axes3D.name)
 
         u = np.linspace(0, 2 * np.pi, 11)
         cv = np.linspace(-1, 1, 12)
         uu, cvv = np.meshgrid(u, cv)
         svv = np.sin(np.arccos(cvv))
         grid_shape = uu.shape
```

### Comparing `microstructpy-1.5.6/src/microstructpy/geometry/n_box.py` & `microstructpy-1.5.7/src/microstructpy/geometry/n_box.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/geometry/n_sphere.py` & `microstructpy-1.5.7/src/microstructpy/geometry/n_sphere.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/geometry/rectangle.py` & `microstructpy-1.5.7/src/microstructpy/geometry/rectangle.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/geometry/sphere.py` & `microstructpy-1.5.7/src/microstructpy/geometry/sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,26 +148,26 @@
 
     # ----------------------------------------------------------------------- #
     # Plot Function                                                           #
     # ----------------------------------------------------------------------- #
     def plot(self, **kwargs):
         """Plot the sphere.
 
-        This function uses the :meth:`mpl_toolkits.mplot3d.Axes3D.plot_surface`
+        This function uses the :meth:`mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface`
         method to add the sphere to the current axes. The keyword arguments
         are passed through to plot_surface.
 
         Args:
             **kwargs (dict): Keyword arguments for plot_surface.
 
         """  # NOQA: E501
-        if len(plt.gcf().axes) == 0:
-            ax = plt.axes(projection=Axes3D.name)
-        else:
+        if plt.gcf().axes:
             ax = plt.gca()
+        else:
+            ax = plt.add_subplot(projection=Axes3D.name)
 
         u = np.linspace(0, 2 * np.pi, 11)
         cv = np.linspace(-1, 1, 12)
         uu, cvv = np.meshgrid(u, cv)
         svv = np.sin(np.arccos(cvv))
 
         xc, yc, zc = self.center
```

### Comparing `microstructpy-1.5.6/src/microstructpy/meshing/polymesh.py` & `microstructpy-1.5.7/src/microstructpy/meshing/polymesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -848,18 +848,18 @@
                 if 'material' is specified. This argument is passed directly
                 through to :func:`matplotlib.pyplot.legend`. Defaults to 0,
                 which is 'best' in matplotlib.
             **kwargs: Keyword arguments for matplotlib.
 
         """
         n_dim = len(self.points[0])
-        if n_dim == 2:
+        if n_dim == 2 or plt.gca().axes:
             ax = plt.gca()
         else:
-            ax = plt.gcf().gca(projection=Axes3D.name)
+            ax = plt.gcf().add_subplot(projection=Axes3D.name)
         n_obj = _misc.ax_objects(ax)
         if n_obj > 0:
             xlim = ax.get_xlim()
             ylim = ax.get_ylim()
         else:
             xlim = [float('inf'), -float('inf')]
             ylim = [float('inf'), -float('inf')]
@@ -989,18 +989,18 @@
                     v = value[ind]
                     f_values.append(v)
                 f_kwargs[key] = f_values
             else:
                 f_kwargs[key] = value
 
         n_dim = len(self.points[0])
-        if n_dim == 2:
+        if n_dim == 2 or plt.gcf().axes:
             ax = plt.gca()
         else:
-            ax = plt.gcf().gca(projection=Axes3D.name)
+            ax = plt.gcf().add_subplot(projection=Axes3D.name)
         n_obj = _misc.ax_objects(ax)
         if n_obj > 0:
             xlim = ax.get_xlim()
             ylim = ax.get_ylim()
         else:
             xlim = [float('inf'), -float('inf')]
             ylim = [float('inf'), -float('inf')]
```

### Comparing `microstructpy-1.5.6/src/microstructpy/meshing/trimesh.py` & `microstructpy-1.5.7/src/microstructpy/meshing/trimesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -562,18 +562,18 @@
                 if 'material' is specified. This argument is passed directly
                 through to :func:`matplotlib.pyplot.legend`. Defaults to 0,
                 which is 'best' in matplotlib.
             **kwargs: Keyword arguments that are passed through to matplotlib.
 
         """
         n_dim = len(self.points[0])
-        if n_dim == 2:
+        if n_dim == 2 or plt.gcf().axes:
             ax = plt.gca()
         else:
-            ax = plt.gcf().gca(projection=Axes3D.name)
+            ax = plt.gcf().add_subplot(projection=Axes3D.name)
         n_obj = _misc.ax_objects(ax)
         if n_obj > 0:
             xlim = ax.get_xlim()
             ylim = ax.get_ylim()
         else:
             xlim = [float('inf'), -float('inf')]
             ylim = [float('inf'), -float('inf')]
```

### Comparing `microstructpy-1.5.6/src/microstructpy/seeding/seed.py` & `microstructpy-1.5.7/src/microstructpy/seeding/seed.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy/seeding/seedlist.py` & `microstructpy-1.5.7/src/microstructpy/seeding/seedlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,18 +446,18 @@
                         seed_args[seed_num][key] = val[seed_num]
                     elif index_by == 'material' and len(val) > phase_num:
                         seed_args[seed_num][key] = val[phase_num]
                 else:
                     seed_args[seed_num][key] = val
 
         n = self[0].geometry.n_dim
-        if n == 2:
+        if n == 2 or plt.gcf().axes:
             ax = plt.gca()
         else:
-            ax = plt.gcf().gca(projection=Axes3D.name)
+            ax = plt.gcf().add_subplot(projection=Axes3D.name)
         n_obj = _misc.ax_objects(ax)
         if n_obj > 0:
             xlim = ax.get_xlim()
             ylim = ax.get_ylim()
         else:
             xlim = [float('inf'), -float('inf')]
             ylim = [float('inf'), -float('inf')]
```

### Comparing `microstructpy-1.5.6/src/microstructpy/verification.py` & `microstructpy-1.5.7/src/microstructpy/verification.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/src/microstructpy.egg-info/SOURCES.txt` & `microstructpy-1.5.7/src/microstructpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .coveragerc
-.readthedocs.yml
+.readthedocs.yaml
 CHANGELOG.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
```

### Comparing `microstructpy-1.5.6/tests/cli/test_includes_files/expected_input.xml` & `microstructpy-1.5.7/tests/cli/test_includes_files/expected_input.xml`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/tests/meshing/test_polymesh.py` & `microstructpy-1.5.7/tests/meshing/test_polymesh.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/tests/test_misc.py` & `microstructpy-1.5.7/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `microstructpy-1.5.6/tox.ini` & `microstructpy-1.5.7/tox.ini`

 * *Files identical despite different names*

