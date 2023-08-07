# Comparing `tmp/ivy-vision-1.1.8.tar.gz` & `tmp/ivy-vision-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivy-vision-1.1.8.tar", last modified: Wed Dec  1 08:48:31 2021, max compression
+gzip compressed data, was "ivy-vision-1.1.9.tar", last modified: Wed Dec  1 16:23:29 2021, max compression
```

## Comparing `ivy-vision-1.1.8.tar` & `ivy-vision-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:31.667477 ivy-vision-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13038 2021-12-01 08:48:31.667477 ivy-vision-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    25856 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:31.663477 ivy-vision-1.1.8/ivy_vision/
--rw-r--r--   0 runner    (1001) docker     (121)      636 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8837 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)    15640 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/implicit.py
--rw-r--r--   0 runner    (1001) docker     (121)     9442 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)    21618 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/optical_flow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/padding.py
--rw-r--r--   0 runner    (1001) docker     (121)     4731 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/projective_geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)    13874 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/quantization.py
--rw-r--r--   0 runner    (1001) docker     (121)     3937 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/sdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    51733 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/single_view_geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     4043 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (121)    19056 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/two_view_geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     7389 2021-12-01 08:48:17.000000 ivy-vision-1.1.8/ivy_vision/voxel_grids.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:31.667477 ivy-vision-1.1.8/ivy_vision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13038 2021-12-01 08:48:31.000000 ivy-vision-1.1.8/ivy_vision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      560 2021-12-01 08:48:31.000000 ivy-vision-1.1.8/ivy_vision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 08:48:31.000000 ivy-vision-1.1.8/ivy_vision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-01 08:48:31.000000 ivy-vision-1.1.8/ivy_vision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-01 08:48:31.000000 ivy-vision-1.1.8/ivy_vision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-01 08:48:18.000000 ivy-vision-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 08:48:31.667477 ivy-vision-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2216 2021-12-01 08:48:18.000000 ivy-vision-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:29.719638 ivy-vision-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    14480 2021-12-01 16:23:29.719638 ivy-vision-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    25719 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:29.719638 ivy-vision-1.1.9/ivy_vision/
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8837 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15640 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9442 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21618 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/optical_flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/padding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4731 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/projective_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13874 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3937 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/sdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51733 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/single_view_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4043 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19056 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/two_view_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7389 2021-12-01 16:23:12.000000 ivy-vision-1.1.9/ivy_vision/voxel_grids.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:29.719638 ivy-vision-1.1.9/ivy_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14480 2021-12-01 16:23:29.000000 ivy-vision-1.1.9/ivy_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2021-12-01 16:23:29.000000 ivy-vision-1.1.9/ivy_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 16:23:29.000000 ivy-vision-1.1.9/ivy_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-01 16:23:29.000000 ivy-vision-1.1.9/ivy_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-01 16:23:29.000000 ivy-vision-1.1.9/ivy_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-01 16:23:13.000000 ivy-vision-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 16:23:29.719638 ivy-vision-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4132 2021-12-01 16:23:13.000000 ivy-vision-1.1.9/setup.py
```

### Comparing `ivy-vision-1.1.8/LICENSE` & `ivy-vision-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/PKG-INFO` & `ivy-vision-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: ivy-vision
-Version: 1.1.8
+Version: 1.1.9
 Summary: 3D Vision functions with end-to-end support for machine learning developers, written in Ivy.
 Home-page: https://ivy-dl.org/vision
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/vision/
 Project-URL: Source, https://github.com/ivy-dl/vision
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **3D Vision functions with end-to-end support for machine learning developers, written in Ivy.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 Contents
 --------
 
 * `Overview`_
 * `Run Through`_
 * `Interactive Demos`_
 * `Get Involed`_
@@ -48,14 +52,17 @@
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
 
 
 
 
 
 
 
@@ -127,16 +134,16 @@
         cam1_inv_ext_mat, intrinsics)
     cam2_geom = ivy_vision.inv_ext_mat_and_intrinsics_to_cam_geometry_object(
         cam2_inv_ext_mat, intrinsics)
     cam_geoms = [cam1_geom, cam2_geom]
 
 The geometries used in this quick start demo are based upon the scene presented below.
 
-
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/scene.png?raw=true
+   :width: 100%
 
 The code sample below demonstrates all of the attributes contained within the Ivy camera geometry class.
 
 .. code-block:: python
 
     for cam_geom in cam_geoms:
 
@@ -181,15 +188,16 @@
     # h x w x 3
     u_pix_coords = ivy_vision.create_uniform_pixel_coords_image(img_dims)
     ds_pixel_coords1 = u_pix_coords * depth1
     ds_pixel_coords2 = u_pix_coords * depth2
 
 The rgb and depth images are presented below.
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/rgb_and_depth.png?raw=true
+   :width: 100%
 
 **Optical Flow and Depth Triangulation**
 
 Now that we have two cameras, their geometries, and their images fully defined,
 we can start to apply some of the more interesting vision functions.
 We start with some optical flow and depth triangulation functions.
 
@@ -206,15 +214,16 @@
     flow1to2 = ivy_vision.flow_from_depth_and_cam_mats(ds_pixel_coords1, cam1to2_full_mat)
 
     # depth again
     depth1_from_flow = ivy_vision.depth_from_flow_and_cam_mats(flow1to2, full_mats)
 
 Visualizations of these images are given below.
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/flow_and_depth.png?raw=true
+   :width: 100%
 
 **Inverse and Forward Warping**
 
 Most of the vision functions, including the flow and depth functions above,
 make use of image projections,
 whereby an image of depth-scaled homogeneous pixel-coordinates is transformed into
 cartesian co-ordinates relative to the acquiring camera, the world, another camera,
@@ -252,15 +261,16 @@
     # inverse warp rendering with mask
     color2_warp_to_f1_masked = ivy.where(depth_validity, color2_warp_to_f1, ivy.zeros_like(color2_warp_to_f1))
 
 Again, visualizations of these images are given below.
 The images represent intermediate steps for the inverse warping of color from frame 2 to frame 1,
 which is shown in the bottom right corner.
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/inverse_warped.png?raw=true
+   :width: 100%
 
 For forward warping, we instead assume depth to be known in the source frame.
 A common approach is to construct a mesh, and then perform rasterization of the mesh.
 
 The ivy method ``ivy_vision.render_pixel_coords`` instead takes a simpler approach,
 by determining the pixel projections into the target frame,
 quantizing these to integer pixel co-ordinates,
@@ -293,15 +303,16 @@
         ivy.reshape(ds_pixel_coords1_proj, (-1, 2)), img_dims, ivy.reshape(features_to_render, (-1, 4)),
         ivy.zeros_like(features_to_render), with_db=False if ivy.get_framework() == 'mxnet' else True)
 
 Again, visualizations of these images are given below.
 The images show the forward warping of both depth and color from frame 2 to frame 1,
 which are shown with and without depth buffers in the right-hand and central columns respectively.
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/forward_warped.png?raw=true
+   :width: 100%
 
 Interactive Demos
 -----------------
 
 In addition to the examples above, we provide two further demo scripts,
 which are more visual and interactive, and are each built around a particular function.
 
@@ -312,32 +323,41 @@
 
 The first demo uses method ``ivy_vision.render_implicit_features_and_depth``
 to train a Neural Radiance Field (NeRF) model to encode a lego digger. The NeRF model can then be queried at new camera
 poses to render new images from poses unseen during training.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_vision/nerf_demo.png?raw=true
+   :width: 100%
+
 **Co-ordinates to Voxel Grid**
 
 The second demo captures depth and color images from a set of cameras,
 converts the depth to world-centric co-ordinartes,
 and uses the method ``ivy_vision.coords_to_voxel_grid`` to
 voxelize the depth and color values into a grid, as shown below:
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_vision/voxel_grid_demo.png?raw=true
+   :width: 100%
+
 **Point Rendering**
 
 The final demo again captures depth and color images from a set of cameras,
 but this time uses the method ``ivy_vision.quantize_to_image`` to
 dynamically forward warp and point render the images into a new target frame, as shown below.
 The acquiring cameras all remain static, while the target frame for point rendering moves freely.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_vision/point_render_demo.png?raw=true
+   :width: 100%
+
 Get Involed
 -----------
 
 We hope the functions in this library are useful to a wide range of machine learning developers.
 However, there are many more areas of 3D vision which could be covered by this library.
 
 If there are any particular vision functions you feel are missing,
```

### Comparing `ivy-vision-1.1.8/README.rst` & `ivy-vision-1.1.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/logos/logo.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 .. raw:: html
 
     <br/>
     <a href="https://pypi.org/project/ivy-vision">
         <img style="float: left; padding-right: 4px; padding-bottom: 4px;" src="https://badge.fury.io/py/ivy-vision.svg">
     </a>
@@ -256,20 +253,16 @@
         cam1_inv_ext_mat, intrinsics)
     cam2_geom = ivy_vision.inv_ext_mat_and_intrinsics_to_cam_geometry_object(
         cam2_inv_ext_mat, intrinsics)
     cam_geoms = [cam1_geom, cam2_geom]
 
 The geometries used in this quick start demo are based upon the scene presented below.
 
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/images/scene.png'>
-    </p>
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/scene.png?raw=true
+   :width: 100%
 
 The code sample below demonstrates all of the attributes contained within the Ivy camera geometry class.
 
 .. code-block:: python
 
     for cam_geom in cam_geoms:
 
@@ -314,19 +307,16 @@
     # h x w x 3
     u_pix_coords = ivy_vision.create_uniform_pixel_coords_image(img_dims)
     ds_pixel_coords1 = u_pix_coords * depth1
     ds_pixel_coords2 = u_pix_coords * depth2
 
 The rgb and depth images are presented below.
 
-.. raw:: html
-
-    <p align="center">
-        <img width="100%" style="display: block;" src='docs/partial_source/images/rgb_and_depth.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/rgb_and_depth.png?raw=true
+   :width: 100%
 
 **Optical Flow and Depth Triangulation**
 
 Now that we have two cameras, their geometries, and their images fully defined,
 we can start to apply some of the more interesting vision functions.
 We start with some optical flow and depth triangulation functions.
 
@@ -343,19 +333,16 @@
     flow1to2 = ivy_vision.flow_from_depth_and_cam_mats(ds_pixel_coords1, cam1to2_full_mat)
 
     # depth again
     depth1_from_flow = ivy_vision.depth_from_flow_and_cam_mats(flow1to2, full_mats)
 
 Visualizations of these images are given below.
 
-.. raw:: html
-
-    <p align="center">
-        <img width="100%" style="display: block;" src='docs/partial_source/images/flow_and_depth.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/flow_and_depth.png?raw=true
+   :width: 100%
 
 **Inverse and Forward Warping**
 
 Most of the vision functions, including the flow and depth functions above,
 make use of image projections,
 whereby an image of depth-scaled homogeneous pixel-coordinates is transformed into
 cartesian co-ordinates relative to the acquiring camera, the world, another camera,
@@ -393,19 +380,16 @@
     # inverse warp rendering with mask
     color2_warp_to_f1_masked = ivy.where(depth_validity, color2_warp_to_f1, ivy.zeros_like(color2_warp_to_f1))
 
 Again, visualizations of these images are given below.
 The images represent intermediate steps for the inverse warping of color from frame 2 to frame 1,
 which is shown in the bottom right corner.
 
-.. raw:: html
-
-    <p align="center">
-        <img width="100%" style="display: block;" src='docs/partial_source/images/inverse_warped.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/inverse_warped.png?raw=true
+   :width: 100%
 
 For forward warping, we instead assume depth to be known in the source frame.
 A common approach is to construct a mesh, and then perform rasterization of the mesh.
 
 The ivy method ``ivy_vision.render_pixel_coords`` instead takes a simpler approach,
 by determining the pixel projections into the target frame,
 quantizing these to integer pixel co-ordinates,
@@ -438,19 +422,16 @@
         ivy.reshape(ds_pixel_coords1_proj, (-1, 2)), img_dims, ivy.reshape(features_to_render, (-1, 4)),
         ivy.zeros_like(features_to_render), with_db=False if ivy.get_framework() == 'mxnet' else True)
 
 Again, visualizations of these images are given below.
 The images show the forward warping of both depth and color from frame 2 to frame 1,
 which are shown with and without depth buffers in the right-hand and central columns respectively.
 
-.. raw:: html
-
-    <p align="center">
-        <img width="100%" style="display: block;" src='docs/partial_source/images/forward_warped.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/forward_warped.png?raw=true
+   :width: 100%
 
 Interactive Demos
 -----------------
 
 In addition to the examples above, we provide two further demo scripts,
 which are more visual and interactive, and are each built around a particular function.
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-.. raw:: html
-                     [docs/partial_source/logos/logo.png]
-.. raw:: html
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/
+logos/logo.png?raw=true :width: 100% .. raw:: html
 [https://badge.fury.io/py/ivy-vision.svg] [https://img.shields.io/github/
 workflow/status/ivy-dl/vision/docs?label=docs] [https://img.shields.io/github/
 workflow/status/ivy-dl/vision/nightly-tests?label=tests] [https://
 img.shields.io/discord/
 799879767196958751?color=blue&label=%20&logo=discord&logoColor=white]
 **3D Vision functions with end-to-end support for machine learning developers,
 written in Ivy.** .. raw:: html
@@ -127,19 +126,20 @@
 (data_dir + '/cam1_inv_ext_mat.npy'), 'float32') cam2_inv_ext_mat = ivy.array
 (np.load(data_dir + '/cam2_inv_ext_mat.npy'), 'float32') # full geometry # ivy
 cam geometry container cam1_geom =
 ivy_vision.inv_ext_mat_and_intrinsics_to_cam_geometry_object( cam1_inv_ext_mat,
 intrinsics) cam2_geom =
 ivy_vision.inv_ext_mat_and_intrinsics_to_cam_geometry_object( cam2_inv_ext_mat,
 intrinsics) cam_geoms = [cam1_geom, cam2_geom] The geometries used in this
-quick start demo are based upon the scene presented below. .. raw:: html
-                    [docs/partial_source/images/scene.png]
-The code sample below demonstrates all of the attributes contained within the
-Ivy camera geometry class. .. code-block:: python for cam_geom in cam_geoms:
-assert cam_geom.intrinsics.focal_lengths.shape == (2,) assert
+quick start demo are based upon the scene presented below. .. image:: https://
+github.com/ivy-dl/vision/blob/master/docs/partial_source/images/
+scene.png?raw=true :width: 100% The code sample below demonstrates all of the
+attributes contained within the Ivy camera geometry class. .. code-block::
+python for cam_geom in cam_geoms: assert
+cam_geom.intrinsics.focal_lengths.shape == (2,) assert
 cam_geom.intrinsics.persp_angles.shape == (2,) assert
 cam_geom.intrinsics.pp_offsets.shape == (2,) assert
 cam_geom.intrinsics.calib_mats.shape == (3, 3) assert
 cam_geom.intrinsics.inv_calib_mats.shape == (3, 3) assert
 cam_geom.extrinsics.cam_centers.shape == (3, 1) assert
 cam_geom.extrinsics.Rs.shape == (3, 3) assert cam_geom.extrinsics.inv_Rs.shape
 == (3, 3) assert cam_geom.extrinsics.ext_mats_homo.shape == (4, 4) assert
@@ -155,92 +155,92 @@
 rgb2.png').astype(np.float32) / 255) # h x w x 1 depth1 = ivy.array(np.reshape
 (np.frombuffer(cv2.imread( data_dir + '/depth1.png', -1).tobytes(),
 np.float32), img_dims + [1])) depth2 = ivy.array(np.reshape(np.frombuffer
 (cv2.imread( data_dir + '/depth2.png', -1).tobytes(), np.float32), img_dims +
 [1])) # depth scaled pixel coords # h x w x 3 u_pix_coords =
 ivy_vision.create_uniform_pixel_coords_image(img_dims) ds_pixel_coords1 =
 u_pix_coords * depth1 ds_pixel_coords2 = u_pix_coords * depth2 The rgb and
-depth images are presented below. .. raw:: html
-                [docs/partial_source/images/rgb_and_depth.png]
+depth images are presented below. .. image:: https://github.com/ivy-dl/vision/
+blob/master/docs/partial_source/images/rgb_and_depth.png?raw=true :width: 100%
 **Optical Flow and Depth Triangulation** Now that we have two cameras, their
 geometries, and their images fully defined, we can start to apply some of the
 more interesting vision functions. We start with some optical flow and depth
 triangulation functions. .. code-block:: python # required mat formats
 cam1to2_full_mat_homo = ivy.matmul(cam2_geom.full_mats_homo,
 cam1_geom.inv_full_mats_homo) cam1to2_full_mat = cam1to2_full_mat_homo[..., 0:
 3, :] full_mats_homo = ivy.concatenate((ivy.expand_dims
 (cam1_geom.full_mats_homo, 0), ivy.expand_dims(cam2_geom.full_mats_homo, 0)),
 0) full_mats = full_mats_homo[..., 0:3, :] # flow flow1to2 =
 ivy_vision.flow_from_depth_and_cam_mats(ds_pixel_coords1, cam1to2_full_mat) #
 depth again depth1_from_flow = ivy_vision.depth_from_flow_and_cam_mats
-(flow1to2, full_mats) Visualizations of these images are given below. .. raw::
-html
-                [docs/partial_source/images/flow_and_depth.png]
-**Inverse and Forward Warping** Most of the vision functions, including the
-flow and depth functions above, make use of image projections, whereby an image
-of depth-scaled homogeneous pixel-coordinates is transformed into cartesian co-
-ordinates relative to the acquiring camera, the world, another camera, or
-transformed directly to pixel co-ordinates in another camera frame. These
-projections also allow warping of the color values from one camera to another.
-For inverse warping, we assume depth to be known for the target frame. We can
-then determine the pixel projections into the source frame, and bilinearly
-interpolate these color values at the pixel projections, to infer the color
-image in the target frame. Treating frame 1 as our target frame, we can use the
-previously calculated optical flow from frame 1 to 2, in order to inverse warp
-the color data from frame 2 to frame 1, as shown below. .. code-block:: python
-# inverse warp rendering warp = u_pix_coords[..., 0:2] + flow1to2
-color2_warp_to_f1 = ivy.bilinear_resample(color2, warp) # projected depth
-scaled pixel coords 2 ds_pixel_coords1_wrt_f2 =
-ivy_vision.ds_pixel_to_ds_pixel_coords(ds_pixel_coords1, cam1to2_full_mat) #
-projected depth 2 depth1_wrt_f2 = ds_pixel_coords1_wrt_f2[..., -1:] # inverse
-warp depth depth2_warp_to_f1 = ivy.bilinear_resample(depth2, warp) # depth
-validity depth_validity = ivy.abs(depth1_wrt_f2 - depth2_warp_to_f1) < 0.01 #
-inverse warp rendering with mask color2_warp_to_f1_masked = ivy.where
-(depth_validity, color2_warp_to_f1, ivy.zeros_like(color2_warp_to_f1)) Again,
-visualizations of these images are given below. The images represent
-intermediate steps for the inverse warping of color from frame 2 to frame 1,
-which is shown in the bottom right corner. .. raw:: html
-                [docs/partial_source/images/inverse_warped.png]
-For forward warping, we instead assume depth to be known in the source frame. A
-common approach is to construct a mesh, and then perform rasterization of the
-mesh. The ivy method ``ivy_vision.render_pixel_coords`` instead takes a simpler
-approach, by determining the pixel projections into the target frame,
-quantizing these to integer pixel co-ordinates, and scattering the
-corresponding color values directly into these integer pixel co-ordinates. This
-process in general leads to holes and duplicates in the resultant image, but
-when compared to inverse warping, it has the beneft that the target frame does
-not need to correspond to a real camera with known depth. Only the target
-camera geometry is required, which can be for any hypothetical camera. We now
-consider the case of forward warping the color data from camera frame 2 to
-camera frame 1, and again render the new color image in target frame 1. ..
-code-block:: python # forward warp rendering ds_pixel_coords1_proj =
-ivy_vision.ds_pixel_to_ds_pixel_coords( ds_pixel_coords2, ivy.inv
-(cam1to2_full_mat_homo)[..., 0:3, :]) depth1_proj = ds_pixel_coords1_proj[...,
--1:] ds_pixel_coords1_proj = ds_pixel_coords1_proj[..., 0:2] / depth1_proj
-features_to_render = ivy.concatenate((depth1_proj, color2), -1) # without depth
-buffer f1_forward_warp_no_db, _, _ = ivy_vision.quantize_to_image( ivy.reshape
-(ds_pixel_coords1_proj, (-1, 2)), img_dims, ivy.reshape(features_to_render, (-
-1, 4)), ivy.zeros_like(features_to_render), with_db=False) # with depth buffer
-f1_forward_warp_w_db, _, _ = ivy_vision.quantize_to_image( ivy.reshape
-(ds_pixel_coords1_proj, (-1, 2)), img_dims, ivy.reshape(features_to_render, (-
-1, 4)), ivy.zeros_like(features_to_render), with_db=False if ivy.get_framework
-() == 'mxnet' else True) Again, visualizations of these images are given below.
-The images show the forward warping of both depth and color from frame 2 to
-frame 1, which are shown with and without depth buffers in the right-hand and
-central columns respectively. .. raw:: html
-                [docs/partial_source/images/forward_warped.png]
-Interactive Demos ----------------- In addition to the examples above, we
-provide two further demo scripts, which are more visual and interactive, and
-are each built around a particular function. Rather than presenting the code
-here, we show visualizations of the demos. The scripts for these demos can be
-found in the interactive_ demos folder. **Neural Rendering** The first demo
-uses method ``ivy_vision.render_implicit_features_and_depth`` to train a Neural
-Radiance Field (NeRF) model to encode a lego digger. The NeRF model can then be
-queried at new camera poses to render new images from poses unseen during
-training. .. raw:: html
+(flow1to2, full_mats) Visualizations of these images are given below. ..
+image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/
+images/flow_and_depth.png?raw=true :width: 100% **Inverse and Forward Warping**
+Most of the vision functions, including the flow and depth functions above,
+make use of image projections, whereby an image of depth-scaled homogeneous
+pixel-coordinates is transformed into cartesian co-ordinates relative to the
+acquiring camera, the world, another camera, or transformed directly to pixel
+co-ordinates in another camera frame. These projections also allow warping of
+the color values from one camera to another. For inverse warping, we assume
+depth to be known for the target frame. We can then determine the pixel
+projections into the source frame, and bilinearly interpolate these color
+values at the pixel projections, to infer the color image in the target frame.
+Treating frame 1 as our target frame, we can use the previously calculated
+optical flow from frame 1 to 2, in order to inverse warp the color data from
+frame 2 to frame 1, as shown below. .. code-block:: python # inverse warp
+rendering warp = u_pix_coords[..., 0:2] + flow1to2 color2_warp_to_f1 =
+ivy.bilinear_resample(color2, warp) # projected depth scaled pixel coords 2
+ds_pixel_coords1_wrt_f2 = ivy_vision.ds_pixel_to_ds_pixel_coords
+(ds_pixel_coords1, cam1to2_full_mat) # projected depth 2 depth1_wrt_f2 =
+ds_pixel_coords1_wrt_f2[..., -1:] # inverse warp depth depth2_warp_to_f1 =
+ivy.bilinear_resample(depth2, warp) # depth validity depth_validity = ivy.abs
+(depth1_wrt_f2 - depth2_warp_to_f1) < 0.01 # inverse warp rendering with mask
+color2_warp_to_f1_masked = ivy.where(depth_validity, color2_warp_to_f1,
+ivy.zeros_like(color2_warp_to_f1)) Again, visualizations of these images are
+given below. The images represent intermediate steps for the inverse warping of
+color from frame 2 to frame 1, which is shown in the bottom right corner. ..
+image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/
+images/inverse_warped.png?raw=true :width: 100% For forward warping, we instead
+assume depth to be known in the source frame. A common approach is to construct
+a mesh, and then perform rasterization of the mesh. The ivy method
+``ivy_vision.render_pixel_coords`` instead takes a simpler approach, by
+determining the pixel projections into the target frame, quantizing these to
+integer pixel co-ordinates, and scattering the corresponding color values
+directly into these integer pixel co-ordinates. This process in general leads
+to holes and duplicates in the resultant image, but when compared to inverse
+warping, it has the beneft that the target frame does not need to correspond to
+a real camera with known depth. Only the target camera geometry is required,
+which can be for any hypothetical camera. We now consider the case of forward
+warping the color data from camera frame 2 to camera frame 1, and again render
+the new color image in target frame 1. .. code-block:: python # forward warp
+rendering ds_pixel_coords1_proj = ivy_vision.ds_pixel_to_ds_pixel_coords
+( ds_pixel_coords2, ivy.inv(cam1to2_full_mat_homo)[..., 0:3, :]) depth1_proj =
+ds_pixel_coords1_proj[..., -1:] ds_pixel_coords1_proj = ds_pixel_coords1_proj
+[..., 0:2] / depth1_proj features_to_render = ivy.concatenate((depth1_proj,
+color2), -1) # without depth buffer f1_forward_warp_no_db, _, _ =
+ivy_vision.quantize_to_image( ivy.reshape(ds_pixel_coords1_proj, (-1, 2)),
+img_dims, ivy.reshape(features_to_render, (-1, 4)), ivy.zeros_like
+(features_to_render), with_db=False) # with depth buffer f1_forward_warp_w_db,
+_, _ = ivy_vision.quantize_to_image( ivy.reshape(ds_pixel_coords1_proj, (-1,
+2)), img_dims, ivy.reshape(features_to_render, (-1, 4)), ivy.zeros_like
+(features_to_render), with_db=False if ivy.get_framework() == 'mxnet' else
+True) Again, visualizations of these images are given below. The images show
+the forward warping of both depth and color from frame 2 to frame 1, which are
+shown with and without depth buffers in the right-hand and central columns
+respectively. .. image:: https://github.com/ivy-dl/vision/blob/master/docs/
+partial_source/images/forward_warped.png?raw=true :width: 100% Interactive
+Demos ----------------- In addition to the examples above, we provide two
+further demo scripts, which are more visual and interactive, and are each built
+around a particular function. Rather than presenting the code here, we show
+visualizations of the demos. The scripts for these demos can be found in the
+interactive_ demos folder. **Neural Rendering** The first demo uses method
+``ivy_vision.render_implicit_features_and_depth`` to train a Neural Radiance
+Field (NeRF) model to encode a lego digger. The NeRF model can then be queried
+at new camera poses to render new images from poses unseen during training. ..
+raw:: html
 [https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/
                       ivy_vision/nerf_demo.gif?raw=true]
 **Co-ordinates to Voxel Grid** The second demo captures depth and color images
 from a set of cameras, converts the depth to world-centric co-ordinartes, and
 uses the method ``ivy_vision.coords_to_voxel_grid`` to voxelize the depth and
 color values into a grid, as shown below: .. raw:: html
 [https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/
```

### Comparing `ivy-vision-1.1.8/ivy_vision/__init__.py` & `ivy-vision-1.1.9/ivy_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/containers.py` & `ivy-vision-1.1.9/ivy_vision/containers.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/implicit.py` & `ivy-vision-1.1.9/ivy_vision/implicit.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/mesh.py` & `ivy-vision-1.1.9/ivy_vision/mesh.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/optical_flow.py` & `ivy-vision-1.1.9/ivy_vision/optical_flow.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/padding.py` & `ivy-vision-1.1.9/ivy_vision/padding.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/projective_geometry.py` & `ivy-vision-1.1.9/ivy_vision/projective_geometry.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/quantization.py` & `ivy-vision-1.1.9/ivy_vision/quantization.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/sdf.py` & `ivy-vision-1.1.9/ivy_vision/sdf.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/single_view_geometry.py` & `ivy-vision-1.1.9/ivy_vision/single_view_geometry.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/smoothing.py` & `ivy-vision-1.1.9/ivy_vision/smoothing.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/two_view_geometry.py` & `ivy-vision-1.1.9/ivy_vision/two_view_geometry.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision/voxel_grids.py` & `ivy-vision-1.1.9/ivy_vision/voxel_grids.py`

 * *Files identical despite different names*

### Comparing `ivy-vision-1.1.8/ivy_vision.egg-info/PKG-INFO` & `ivy-vision-1.1.9/ivy_vision.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: ivy-vision
-Version: 1.1.8
+Version: 1.1.9
 Summary: 3D Vision functions with end-to-end support for machine learning developers, written in Ivy.
 Home-page: https://ivy-dl.org/vision
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/vision/
 Project-URL: Source, https://github.com/ivy-dl/vision
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **3D Vision functions with end-to-end support for machine learning developers, written in Ivy.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 Contents
 --------
 
 * `Overview`_
 * `Run Through`_
 * `Interactive Demos`_
 * `Get Involed`_
@@ -48,14 +52,17 @@
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
 
 
 
 
 
 
 
@@ -127,16 +134,16 @@
         cam1_inv_ext_mat, intrinsics)
     cam2_geom = ivy_vision.inv_ext_mat_and_intrinsics_to_cam_geometry_object(
         cam2_inv_ext_mat, intrinsics)
     cam_geoms = [cam1_geom, cam2_geom]
 
 The geometries used in this quick start demo are based upon the scene presented below.
 
-
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/scene.png?raw=true
+   :width: 100%
 
 The code sample below demonstrates all of the attributes contained within the Ivy camera geometry class.
 
 .. code-block:: python
 
     for cam_geom in cam_geoms:
 
@@ -181,15 +188,16 @@
     # h x w x 3
     u_pix_coords = ivy_vision.create_uniform_pixel_coords_image(img_dims)
     ds_pixel_coords1 = u_pix_coords * depth1
     ds_pixel_coords2 = u_pix_coords * depth2
 
 The rgb and depth images are presented below.
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/rgb_and_depth.png?raw=true
+   :width: 100%
 
 **Optical Flow and Depth Triangulation**
 
 Now that we have two cameras, their geometries, and their images fully defined,
 we can start to apply some of the more interesting vision functions.
 We start with some optical flow and depth triangulation functions.
 
@@ -206,15 +214,16 @@
     flow1to2 = ivy_vision.flow_from_depth_and_cam_mats(ds_pixel_coords1, cam1to2_full_mat)
 
     # depth again
     depth1_from_flow = ivy_vision.depth_from_flow_and_cam_mats(flow1to2, full_mats)
 
 Visualizations of these images are given below.
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/flow_and_depth.png?raw=true
+   :width: 100%
 
 **Inverse and Forward Warping**
 
 Most of the vision functions, including the flow and depth functions above,
 make use of image projections,
 whereby an image of depth-scaled homogeneous pixel-coordinates is transformed into
 cartesian co-ordinates relative to the acquiring camera, the world, another camera,
@@ -252,15 +261,16 @@
     # inverse warp rendering with mask
     color2_warp_to_f1_masked = ivy.where(depth_validity, color2_warp_to_f1, ivy.zeros_like(color2_warp_to_f1))
 
 Again, visualizations of these images are given below.
 The images represent intermediate steps for the inverse warping of color from frame 2 to frame 1,
 which is shown in the bottom right corner.
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/inverse_warped.png?raw=true
+   :width: 100%
 
 For forward warping, we instead assume depth to be known in the source frame.
 A common approach is to construct a mesh, and then perform rasterization of the mesh.
 
 The ivy method ``ivy_vision.render_pixel_coords`` instead takes a simpler approach,
 by determining the pixel projections into the target frame,
 quantizing these to integer pixel co-ordinates,
@@ -293,15 +303,16 @@
         ivy.reshape(ds_pixel_coords1_proj, (-1, 2)), img_dims, ivy.reshape(features_to_render, (-1, 4)),
         ivy.zeros_like(features_to_render), with_db=False if ivy.get_framework() == 'mxnet' else True)
 
 Again, visualizations of these images are given below.
 The images show the forward warping of both depth and color from frame 2 to frame 1,
 which are shown with and without depth buffers in the right-hand and central columns respectively.
 
-
+.. image:: https://github.com/ivy-dl/vision/blob/master/docs/partial_source/images/forward_warped.png?raw=true
+   :width: 100%
 
 Interactive Demos
 -----------------
 
 In addition to the examples above, we provide two further demo scripts,
 which are more visual and interactive, and are each built around a particular function.
 
@@ -312,32 +323,41 @@
 
 The first demo uses method ``ivy_vision.render_implicit_features_and_depth``
 to train a Neural Radiance Field (NeRF) model to encode a lego digger. The NeRF model can then be queried at new camera
 poses to render new images from poses unseen during training.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_vision/nerf_demo.png?raw=true
+   :width: 100%
+
 **Co-ordinates to Voxel Grid**
 
 The second demo captures depth and color images from a set of cameras,
 converts the depth to world-centric co-ordinartes,
 and uses the method ``ivy_vision.coords_to_voxel_grid`` to
 voxelize the depth and color values into a grid, as shown below:
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_vision/voxel_grid_demo.png?raw=true
+   :width: 100%
+
 **Point Rendering**
 
 The final demo again captures depth and color images from a set of cameras,
 but this time uses the method ``ivy_vision.quantize_to_image`` to
 dynamically forward warp and point render the images into a new target frame, as shown below.
 The acquiring cameras all remain static, while the target frame for point rendering moves freely.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_vision/point_render_demo.png?raw=true
+   :width: 100%
+
 Get Involed
 -----------
 
 We hope the functions in this library are useful to a wide range of machine learning developers.
 However, there are many more areas of 3D vision which could be covered by this library.
 
 If there are any particular vision functions you feel are missing,
```

### Comparing `ivy-vision-1.1.8/ivy_vision.egg-info/SOURCES.txt` & `ivy-vision-1.1.9/ivy_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

