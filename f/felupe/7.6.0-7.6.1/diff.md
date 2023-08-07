# Comparing `tmp/felupe-7.6.0.tar.gz` & `tmp/felupe-7.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-7.6.0.tar", last modified: Sat Aug  5 22:04:16 2023, max compression
+gzip compressed data, was "felupe-7.6.1.tar", last modified: Mon Aug  7 10:27:25 2023, max compression
```

## Comparing `felupe-7.6.0.tar` & `felupe-7.6.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.355532 felupe-7.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-08-05 22:04:07.000000 felupe-7.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50402 2023-08-05 22:04:16.355532 felupe-7.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-08-05 22:04:07.000000 felupe-7.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-05 22:04:07.000000 felupe-7.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 22:04:16.355532 felupe-7.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.339532 felupe-7.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.343532 felupe-7.6.0/src/felupe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.343532 felupe-7.6.0/src/felupe/_assembly/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_assembly/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23227 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_assembly/_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_assembly/_integral.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_assembly/_weak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.343532 felupe-7.6.0/src/felupe/_basis/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_basis/_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.343532 felupe-7.6.0/src/felupe/_field/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_field/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_field/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_field/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_field/_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_field/_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/_field/_planestrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.347532 felupe-7.6.0/src/felupe/constitution/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/_models_hyperelasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/_models_hyperelasticity_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/_models_linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/_models_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/_user_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/_user_materials_hyperelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/constitution/_user_materials_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.347532 felupe-7.6.0/src/felupe/dof/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/dof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/dof/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/dof/_loadcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/dof/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.347532 felupe-7.6.0/src/felupe/element/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/element/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/element/_hexahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/element/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/element/_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/element/_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/element/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/element/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.347532 felupe-7.6.0/src/felupe/math/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/math/_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/math/_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/math/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/math/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.351532 felupe-7.6.0/src/felupe/mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_pointload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_solidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_solidbody_gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_solidbody_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_solidbody_pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mechanics/_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.351532 felupe-7.6.0/src/felupe/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_discrete_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_dual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_line_rectangle_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/mesh/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.351532 felupe-7.6.0/src/felupe/quadrature/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/quadrature/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/quadrature/_gausslegendre.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/quadrature/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/quadrature/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.351532 felupe-7.6.0/src/felupe/region/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/region/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/region/_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/region/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.351532 felupe-7.6.0/src/felupe/solve/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/solve/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.351532 felupe-7.6.0/src/felupe/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/tools/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/tools/_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/tools/_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/tools/_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/tools/_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/tools/_save.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-05 22:04:07.000000 felupe-7.6.0/src/felupe/tools/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.343532 felupe-7.6.0/src/felupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50402 2023-08-05 22:04:16.000000 felupe-7.6.0/src/felupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-08-05 22:04:16.000000 felupe-7.6.0/src/felupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 22:04:16.000000 felupe-7.6.0/src/felupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-05 22:04:16.000000 felupe-7.6.0/src/felupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 22:04:16.000000 felupe-7.6.0/src/felupe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:16.355532 felupe-7.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_bilinearform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_constitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_dof.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_planestrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-08-05 22:04:07.000000 felupe-7.6.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.762699 felupe-7.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-08-07 10:27:16.000000 felupe-7.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50402 2023-08-07 10:27:25.758698 felupe-7.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-08-07 10:27:16.000000 felupe-7.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-07 10:27:16.000000 felupe-7.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:27:25.762699 felupe-7.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.742698 felupe-7.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.746698 felupe-7.6.1/src/felupe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.746698 felupe-7.6.1/src/felupe/_assembly/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_assembly/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23227 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_assembly/_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_assembly/_integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_assembly/_weak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.746698 felupe-7.6.1/src/felupe/_basis/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_basis/_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.750698 felupe-7.6.1/src/felupe/_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_field/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_field/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_field/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_field/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_field/_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/_field/_planestrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.750698 felupe-7.6.1/src/felupe/constitution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/_models_hyperelasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/_models_hyperelasticity_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/_models_linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/_models_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/_user_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/_user_materials_hyperelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/constitution/_user_materials_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.750698 felupe-7.6.1/src/felupe/dof/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/dof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/dof/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/dof/_loadcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/dof/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.750698 felupe-7.6.1/src/felupe/element/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/element/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/element/_hexahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/element/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/element/_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/element/_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/element/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/element/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.750698 felupe-7.6.1/src/felupe/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/math/_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/math/_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/math/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/math/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.754698 felupe-7.6.1/src/felupe/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_pointload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_solidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_solidbody_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_solidbody_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_solidbody_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mechanics/_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.754698 felupe-7.6.1/src/felupe/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_discrete_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_line_rectangle_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/mesh/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.754698 felupe-7.6.1/src/felupe/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/quadrature/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/quadrature/_gausslegendre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/quadrature/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/quadrature/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.754698 felupe-7.6.1/src/felupe/region/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/region/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/region/_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/region/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.758698 felupe-7.6.1/src/felupe/solve/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/solve/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.758698 felupe-7.6.1/src/felupe/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/tools/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/tools/_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/tools/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/tools/_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/tools/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/tools/_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-07 10:27:16.000000 felupe-7.6.1/src/felupe/tools/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.746698 felupe-7.6.1/src/felupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50402 2023-08-07 10:27:25.000000 felupe-7.6.1/src/felupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-08-07 10:27:25.000000 felupe-7.6.1/src/felupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:27:25.000000 felupe-7.6.1/src/felupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 10:27:25.000000 felupe-7.6.1/src/felupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 10:27:25.000000 felupe-7.6.1/src/felupe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:27:25.758698 felupe-7.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_bilinearform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_constitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_dof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_planestrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-08-07 10:27:16.000000 felupe-7.6.1/tests/test_tools.py
```

### Comparing `felupe-7.6.0/LICENSE` & `felupe-7.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/PKG-INFO` & `felupe-7.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.6.0
+Version: 7.6.1
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `felupe-7.6.0/README.md` & `felupe-7.6.1/README.md`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/pyproject.toml` & `felupe-7.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/__init__.py` & `felupe-7.6.1/src/felupe/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_assembly/_axi.py` & `felupe-7.6.1/src/felupe/_assembly/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_assembly/_form.py` & `felupe-7.6.1/src/felupe/_assembly/_form.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_assembly/_integral.py` & `felupe-7.6.1/src/felupe/_assembly/_integral.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_assembly/_weak.py` & `felupe-7.6.1/src/felupe/_assembly/_weak.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_basis/_basis.py` & `felupe-7.6.1/src/felupe/_basis/_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_field/_axi.py` & `felupe-7.6.1/src/felupe/_field/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_field/_base.py` & `felupe-7.6.1/src/felupe/_field/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_field/_container.py` & `felupe-7.6.1/src/felupe/_field/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_field/_fields.py` & `felupe-7.6.1/src/felupe/_field/_fields.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_field/_indices.py` & `felupe-7.6.1/src/felupe/_field/_indices.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/_field/_planestrain.py` & `felupe-7.6.1/src/felupe/_field/_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/__init__.py` & `felupe-7.6.1/src/felupe/constitution/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/_kinematics.py` & `felupe-7.6.1/src/felupe/constitution/_kinematics.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/_mixed.py` & `felupe-7.6.1/src/felupe/constitution/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/_models_hyperelasticity.py` & `felupe-7.6.1/src/felupe/constitution/_models_hyperelasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/_models_hyperelasticity_ad.py` & `felupe-7.6.1/src/felupe/constitution/_models_hyperelasticity_ad.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/_models_linear_elasticity.py` & `felupe-7.6.1/src/felupe/constitution/_models_linear_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/_models_pseudo_elasticity.py` & `felupe-7.6.1/src/felupe/constitution/_models_pseudo_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/_user_materials.py` & `felupe-7.6.1/src/felupe/constitution/_user_materials.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/_user_materials_hyperelastic.py` & `felupe-7.6.1/src/felupe/constitution/_user_materials_hyperelastic.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/constitution/_user_materials_models.py` & `felupe-7.6.1/src/felupe/constitution/_user_materials_models.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/dof/_boundary.py` & `felupe-7.6.1/src/felupe/dof/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/dof/_loadcase.py` & `felupe-7.6.1/src/felupe/dof/_loadcase.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/dof/_tools.py` & `felupe-7.6.1/src/felupe/dof/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/element/__init__.py` & `felupe-7.6.1/src/felupe/element/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/element/_base.py` & `felupe-7.6.1/src/felupe/element/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/element/_hexahedron.py` & `felupe-7.6.1/src/felupe/element/_hexahedron.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/element/_lagrange.py` & `felupe-7.6.1/src/felupe/element/_lagrange.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/element/_line.py` & `felupe-7.6.1/src/felupe/element/_line.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/element/_quad.py` & `felupe-7.6.1/src/felupe/element/_quad.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/element/_tetra.py` & `felupe-7.6.1/src/felupe/element/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/element/_triangle.py` & `felupe-7.6.1/src/felupe/element/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/math/__init__.py` & `felupe-7.6.1/src/felupe/math/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/math/_field.py` & `felupe-7.6.1/src/felupe/math/_field.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/math/_math.py` & `felupe-7.6.1/src/felupe/math/_math.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/math/_spatial.py` & `felupe-7.6.1/src/felupe/math/_spatial.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/math/_tensor.py` & `felupe-7.6.1/src/felupe/math/_tensor.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/__init__.py` & `felupe-7.6.1/src/felupe/mechanics/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_curve.py` & `felupe-7.6.1/src/felupe/mechanics/_curve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_helpers.py` & `felupe-7.6.1/src/felupe/mechanics/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_job.py` & `felupe-7.6.1/src/felupe/mechanics/_job.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_multipoint.py` & `felupe-7.6.1/src/felupe/mechanics/_multipoint.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_pointload.py` & `felupe-7.6.1/src/felupe/mechanics/_pointload.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_solidbody.py` & `felupe-7.6.1/src/felupe/mechanics/_solidbody.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_solidbody_gravity.py` & `felupe-7.6.1/src/felupe/mechanics/_solidbody_gravity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_solidbody_incompressible.py` & `felupe-7.6.1/src/felupe/mechanics/_solidbody_incompressible.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_solidbody_pressure.py` & `felupe-7.6.1/src/felupe/mechanics/_solidbody_pressure.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mechanics/_step.py` & `felupe-7.6.1/src/felupe/mechanics/_step.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/__init__.py` & `felupe-7.6.1/src/felupe/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_container.py` & `felupe-7.6.1/src/felupe/mesh/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_convert.py` & `felupe-7.6.1/src/felupe/mesh/_convert.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_discrete_geometry.py` & `felupe-7.6.1/src/felupe/mesh/_discrete_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_dual.py` & `felupe-7.6.1/src/felupe/mesh/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_geometry.py` & `felupe-7.6.1/src/felupe/mesh/_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_helpers.py` & `felupe-7.6.1/src/felupe/mesh/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_line_rectangle_cube.py` & `felupe-7.6.1/src/felupe/mesh/_line_rectangle_cube.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_mesh.py` & `felupe-7.6.1/src/felupe/mesh/_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_read.py` & `felupe-7.6.1/src/felupe/mesh/_read.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/mesh/_tools.py` & `felupe-7.6.1/src/felupe/mesh/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/quadrature/_base.py` & `felupe-7.6.1/src/felupe/quadrature/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/quadrature/_gausslegendre.py` & `felupe-7.6.1/src/felupe/quadrature/_gausslegendre.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/quadrature/_tetra.py` & `felupe-7.6.1/src/felupe/quadrature/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/quadrature/_triangle.py` & `felupe-7.6.1/src/felupe/quadrature/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/region/__init__.py` & `felupe-7.6.1/src/felupe/region/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/region/_boundary.py` & `felupe-7.6.1/src/felupe/region/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/region/_region.py` & `felupe-7.6.1/src/felupe/region/_region.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/region/_templates.py` & `felupe-7.6.1/src/felupe/region/_templates.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/solve/_solve.py` & `felupe-7.6.1/src/felupe/solve/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/tools/__init__.py` & `felupe-7.6.1/src/felupe/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/tools/_misc.py` & `felupe-7.6.1/src/felupe/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/tools/_newton.py` & `felupe-7.6.1/src/felupe/tools/_newton.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/tools/_plot.py` & `felupe-7.6.1/src/felupe/tools/_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
+import os
+
 import numpy as np
 
 from ..math import eigvalsh, tovoigt
 from ..mechanics._job import (
     deformation_gradient,
     displacement,
     log_strain,
@@ -108,14 +110,20 @@
         """
 
         import pyvista as pv
 
         if theme is not None:
             pv.set_plot_theme(theme)
 
+        # try to start a virtual framebuffer on linux
+        # requires ``sudo apt-get install xvfb``
+        if notebook:
+            if os.name == "posix":
+                pv.start_xvfb()
+
         if plotter is None:
             plotter = pv.Plotter(off_screen=off_screen, notebook=notebook)
 
         if scalar_bar_args is None:
             scalar_bar_args = {}
 
         if name is not None:
```

### Comparing `felupe-7.6.0/src/felupe/tools/_post.py` & `felupe-7.6.1/src/felupe/tools/_post.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/tools/_project.py` & `felupe-7.6.1/src/felupe/tools/_project.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/tools/_save.py` & `felupe-7.6.1/src/felupe/tools/_save.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe/tools/_solve.py` & `felupe-7.6.1/src/felupe/tools/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/src/felupe.egg-info/PKG-INFO` & `felupe-7.6.1/src/felupe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.6.0
+Version: 7.6.1
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `felupe-7.6.0/src/felupe.egg-info/SOURCES.txt` & `felupe-7.6.1/src/felupe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_basis.py` & `felupe-7.6.1/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_bilinearform.py` & `felupe-7.6.1/tests/test_bilinearform.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_composite.py` & `felupe-7.6.1/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_constitution.py` & `felupe-7.6.1/tests/test_constitution.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_dof.py` & `felupe-7.6.1/tests/test_dof.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_element.py` & `felupe-7.6.1/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_field.py` & `felupe-7.6.1/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_form.py` & `felupe-7.6.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_job.py` & `felupe-7.6.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_math.py` & `felupe-7.6.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_mechanics.py` & `felupe-7.6.1/tests/test_mechanics.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_mesh.py` & `felupe-7.6.1/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_mpc.py` & `felupe-7.6.1/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_planestrain.py` & `felupe-7.6.1/tests/test_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_plot.py` & `felupe-7.6.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_quadrature.py` & `felupe-7.6.1/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_readme.py` & `felupe-7.6.1/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_region.py` & `felupe-7.6.1/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_solve.py` & `felupe-7.6.1/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.6.0/tests/test_tools.py` & `felupe-7.6.1/tests/test_tools.py`

 * *Files identical despite different names*

