# Comparing `tmp/ivy-robot-1.1.8.tar.gz` & `tmp/ivy-robot-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivy-robot-1.1.8.tar", last modified: Wed Dec  1 08:49:17 2021, max compression
+gzip compressed data, was "ivy-robot-1.1.9.tar", last modified: Wed Dec  1 16:23:42 2021, max compression
```

## Comparing `ivy-robot-1.1.8.tar` & `ivy-robot-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:49:17.085058 ivy-robot-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 08:49:01.000000 ivy-robot-1.1.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 08:49:01.000000 ivy-robot-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12042 2021-12-01 08:49:17.085058 ivy-robot-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    24552 2021-12-01 08:49:01.000000 ivy-robot-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:49:17.081058 ivy-robot-1.1.8/ivy_robot/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-12-01 08:49:01.000000 ivy-robot-1.1.8/ivy_robot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13746 2021-12-01 08:49:01.000000 ivy-robot-1.1.8/ivy_robot/manipulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2021-12-01 08:49:01.000000 ivy-robot-1.1.8/ivy_robot/planning.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-12-01 08:49:01.000000 ivy-robot-1.1.8/ivy_robot/rigid_mobile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:49:17.085058 ivy-robot-1.1.8/ivy_robot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12042 2021-12-01 08:49:17.000000 ivy-robot-1.1.8/ivy_robot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      315 2021-12-01 08:49:17.000000 ivy-robot-1.1.8/ivy_robot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 08:49:17.000000 ivy-robot-1.1.8/ivy_robot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-01 08:49:17.000000 ivy-robot-1.1.8/ivy_robot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-01 08:49:17.000000 ivy-robot-1.1.8/ivy_robot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-01 08:49:01.000000 ivy-robot-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 08:49:17.085058 ivy-robot-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-12-01 08:49:01.000000 ivy-robot-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:42.752520 ivy-robot-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 16:23:26.000000 ivy-robot-1.1.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 16:23:26.000000 ivy-robot-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    13261 2021-12-01 16:23:42.752520 ivy-robot-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    24437 2021-12-01 16:23:26.000000 ivy-robot-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:42.752520 ivy-robot-1.1.9/ivy_robot/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-12-01 16:23:26.000000 ivy-robot-1.1.9/ivy_robot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13746 2021-12-01 16:23:26.000000 ivy-robot-1.1.9/ivy_robot/manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3489 2021-12-01 16:23:26.000000 ivy-robot-1.1.9/ivy_robot/planning.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-12-01 16:23:26.000000 ivy-robot-1.1.9/ivy_robot/rigid_mobile.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:42.752520 ivy-robot-1.1.9/ivy_robot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13261 2021-12-01 16:23:42.000000 ivy-robot-1.1.9/ivy_robot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2021-12-01 16:23:42.000000 ivy-robot-1.1.9/ivy_robot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 16:23:42.000000 ivy-robot-1.1.9/ivy_robot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-01 16:23:42.000000 ivy-robot-1.1.9/ivy_robot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-01 16:23:42.000000 ivy-robot-1.1.9/ivy_robot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-01 16:23:26.000000 ivy-robot-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 16:23:42.752520 ivy-robot-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4116 2021-12-01 16:23:26.000000 ivy-robot-1.1.9/setup.py
```

### Comparing `ivy-robot-1.1.8/LICENCE` & `ivy-robot-1.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `ivy-robot-1.1.8/PKG-INFO` & `ivy-robot-1.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: ivy-robot
-Version: 1.1.8
+Version: 1.1.9
 Summary: Functions and classes for gradient-based robot motion planning, written in Ivy.
 Home-page: https://ivy-dl.org/robot
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/robot/
 Project-URL: Source, https://github.com/ivy-dl/robot
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **Functions and classes for gradient-based robot motion planning, written in Ivy.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 Contents
 --------
 
 * `Overview`_
 * `Run Through`_
 * `Interactive Demos`_
 * `Get Involed`_
@@ -47,14 +51,17 @@
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
 
 
 
 
 
 
 
@@ -151,15 +158,16 @@
     anchor_xy_positions = anchor_poses[..., 0:2]
 
     # num_samples x 2
     interpolated_xy_positions = interpolated_poses[..., 0:2]
 
 The interpolated xy positions and anchor positions from the path are shown below in the x-y plane.
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/interpolated_drone_poses.png?raw=true
+   :width: 100%
 
 **Rigid Mobile Class**
 
 We now introduce the ``RigidMobile`` robot class,
 which can be used to represent rigid jointless robots which are able to move freely.
 In this case, we consider the case of a drone executing 6DOF motion in a scene.
 
@@ -225,15 +233,16 @@
     # num_samples x num_body_points x 3
     interpolated_body_points = drone.sample_body(interpolated_matrices)
 
 The sampled drone body xy positions during motion are shown below in the x-y plane.
 By tracing the body points for each of the four corners of the drone,
 we can see how the drone performs the 180 degree self-rotation about the z-axis during the motion.
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/sampled_drone_body_positions.png?raw=true
+   :width: 100%
 
 **Manipulator Class**
 
 We now introduce the robot Manipulator class,
 which can be used to represent arbitrary robot manipulators.
 In this case, we consider the case of very simple 2-link manipulator,
 which is constrained to move in the x-y plane.
@@ -279,15 +288,16 @@
     # interpolated joint angles
 
     # num_anchors x 2
     interpolated_joint_angles = ivy_robot.sample_spline_path(anchor_points, anchor_joint_angles, query_points)
 
 The interpolated joint angles are presented below.
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/interpolated_manipulator_joint_angles.png?raw=true
+   :width: 100%
 
 In a similar fashion to how the drone body was sampled in the previous example,
 we next use these interpolated joint angles to sample the link positions for the manipulator.
 
 .. code-block:: python
 
     # sample links
@@ -296,15 +306,16 @@
     anchor_link_points = manipulator.sample_links(anchor_joint_angles, samples_per_metre=5)
 
     # num_anchors x num_link_points x 3
     interpolated_link_points = manipulator.sample_links(interpolated_joint_angles, samples_per_metre=5)
 
 we show the sampled link positions during the course of the forward reaching motion in the x-y plane below.
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/sampled_manipulator_links.png?raw=true
+   :width: 100%
 
 Interactive Demos
 -----------------
 
 The main benefit of the library is not simply the ability to sample paths, but to optimize these paths using gradients.
 For exmaple, the body or link sample positions can be used to query the signed distance function (SDF) of a 3D scene in batch.
 Then, assuming the spline anchor points to be free variables,
@@ -318,22 +329,28 @@
 **RigidMobile Planning**
 
 The first demo uses the ``RigidMobile`` class to optimzie the motion of a drone to a target pose,
 making use of functions ``ivy_robot.sample_spline_path`` and ``ivy_robot.RigidMobile.sample_body``.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_robot/demo_a.png?raw=true
+   :width: 100%
+
 **Manipulator Planning**
 
 The second demo uses the ``MicoManipulator`` class, derived from ``Manipulator``,
 to optimzie the motion of a mico robot manipulator to a set of target joint angles,
 making use of functions ``ivy_robot.sample_spline_path`` and ``ivy_robot.Manipulator.sample_links``.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_robot/demo_b.png?raw=true
+   :width: 100%
+
 Get Involed
 -----------
 
 We hope the functions in this library are useful to a wide range of machine learning developers.
 However, there are many more areas of gradient-based motion planning and broader robotics
 which could be covered by this library.
```

### Comparing `ivy-robot-1.1.8/README.rst` & `ivy-robot-1.1.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/logos/logo.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 .. raw:: html
 
     <br/>
     <a href="https://pypi.org/project/ivy-robot">
         <img style="float: left; padding-right: 4px; padding-bottom: 4px;" src="https://badge.fury.io/py/ivy-robot.svg">
     </a>
@@ -280,19 +277,16 @@
     anchor_xy_positions = anchor_poses[..., 0:2]
 
     # num_samples x 2
     interpolated_xy_positions = interpolated_poses[..., 0:2]
 
 The interpolated xy positions and anchor positions from the path are shown below in the x-y plane.
 
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/images/interpolated_drone_poses.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/interpolated_drone_poses.png?raw=true
+   :width: 100%
 
 **Rigid Mobile Class**
 
 We now introduce the ``RigidMobile`` robot class,
 which can be used to represent rigid jointless robots which are able to move freely.
 In this case, we consider the case of a drone executing 6DOF motion in a scene.
 
@@ -358,19 +352,16 @@
     # num_samples x num_body_points x 3
     interpolated_body_points = drone.sample_body(interpolated_matrices)
 
 The sampled drone body xy positions during motion are shown below in the x-y plane.
 By tracing the body points for each of the four corners of the drone,
 we can see how the drone performs the 180 degree self-rotation about the z-axis during the motion.
 
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/images/sampled_drone_body_positions.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/sampled_drone_body_positions.png?raw=true
+   :width: 100%
 
 **Manipulator Class**
 
 We now introduce the robot Manipulator class,
 which can be used to represent arbitrary robot manipulators.
 In this case, we consider the case of very simple 2-link manipulator,
 which is constrained to move in the x-y plane.
@@ -416,19 +407,16 @@
     # interpolated joint angles
 
     # num_anchors x 2
     interpolated_joint_angles = ivy_robot.sample_spline_path(anchor_points, anchor_joint_angles, query_points)
 
 The interpolated joint angles are presented below.
 
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/images/interpolated_manipulator_joint_angles.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/interpolated_manipulator_joint_angles.png?raw=true
+   :width: 100%
 
 In a similar fashion to how the drone body was sampled in the previous example,
 we next use these interpolated joint angles to sample the link positions for the manipulator.
 
 .. code-block:: python
 
     # sample links
@@ -437,19 +425,16 @@
     anchor_link_points = manipulator.sample_links(anchor_joint_angles, samples_per_metre=5)
 
     # num_anchors x num_link_points x 3
     interpolated_link_points = manipulator.sample_links(interpolated_joint_angles, samples_per_metre=5)
 
 we show the sampled link positions during the course of the forward reaching motion in the x-y plane below.
 
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/images/sampled_manipulator_links.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/sampled_manipulator_links.png?raw=true
+   :width: 100%
 
 Interactive Demos
 -----------------
 
 The main benefit of the library is not simply the ability to sample paths, but to optimize these paths using gradients.
 For exmaple, the body or link sample positions can be used to query the signed distance function (SDF) of a 3D scene in batch.
 Then, assuming the spline anchor points to be free variables,
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-.. raw:: html
-                     [docs/partial_source/logos/logo.png]
-.. raw:: html
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/
+logos/logo.png?raw=true :width: 100% .. raw:: html
 [https://badge.fury.io/py/ivy-robot.svg] [https://img.shields.io/github/
 workflow/status/ivy-dl/robot/docs?label=docs] [https://img.shields.io/github/
 workflow/status/ivy-dl/robot/nightly-tests?label=tests] [https://
 img.shields.io/discord/
 799879767196958751?color=blue&label=%20&logo=discord&logoColor=white]
 **Functions and classes for gradient-based robot motion planning, written in
 Ivy.** .. raw:: html
@@ -133,26 +132,26 @@
 anchor_points = ivy.expand_dims(ivy.linspace(0., 1., num_anchors), -1) #
 num_samples x 1 query_points = ivy.expand_dims(ivy.linspace(0., 1.,
 num_samples), -1) # interpolated spline poses # num_samples x 6
 interpolated_poses = ivy_robot.sample_spline_path(anchor_points, anchor_poses,
 query_points) # xy motion # num_samples x 2 anchor_xy_positions = anchor_poses
 [..., 0:2] # num_samples x 2 interpolated_xy_positions = interpolated_poses
 [..., 0:2] The interpolated xy positions and anchor positions from the path are
-shown below in the x-y plane. .. raw:: html
-           [docs/partial_source/images/interpolated_drone_poses.png]
-**Rigid Mobile Class** We now introduce the ``RigidMobile`` robot class, which
-can be used to represent rigid jointless robots which are able to move freely.
-In this case, we consider the case of a drone executing 6DOF motion in a scene.
-The body of the drone is specified by a number of relative body points. In this
-case, we represent the drone with 5 points: one in the centre, and one in each
-of the four corners. We assume the same target position in the x-y plane as
-before, but this time with a self-rotation of 180 degrees about the z-axis. ..
-code-block:: python # drone relative body points rel_body_points = ivy.array([
-[0., 0., 0.], [-0.1, -0.1, 0.], [-0.1, 0.1, 0.], [0.1, -0.1, 0.], [0.1, 0.1,
-0.]]) # create drone as ivy rigid mobile robot drone = RigidMobile
+shown below in the x-y plane. .. image:: https://github.com/ivy-dl/robot/blob/
+master/docs/partial_source/images/interpolated_drone_poses.png?raw=true :width:
+100% **Rigid Mobile Class** We now introduce the ``RigidMobile`` robot class,
+which can be used to represent rigid jointless robots which are able to move
+freely. In this case, we consider the case of a drone executing 6DOF motion in
+a scene. The body of the drone is specified by a number of relative body
+points. In this case, we represent the drone with 5 points: one in the centre,
+and one in each of the four corners. We assume the same target position in the
+x-y plane as before, but this time with a self-rotation of 180 degrees about
+the z-axis. .. code-block:: python # drone relative body points rel_body_points
+= ivy.array([[0., 0., 0.], [-0.1, -0.1, 0.], [-0.1, 0.1, 0.], [0.1, -0.1, 0.],
+[0.1, 0.1, 0.]]) # create drone as ivy rigid mobile robot drone = RigidMobile
 (rel_body_points) # rotatin vectors # 1 x 3 start_rot_vec = ivy.array([[0., 0.,
 0.]]) target_rot_vec = ivy.array([[0., 0., np.pi]]) # 1 x 3 anchor1_rot_vec =
 ivy.array([[0., 0., np.pi/4]]) anchor2_rot_vec = ivy.array([[0., 0., 2*np.pi/
 4]]) anchor3_rot_vec = ivy.array([[0., 0., 3*np.pi/4]]) # as 6DOF poses # 1 x 6
 start_pose = ivy.concatenate((start_xy, constant_z, start_rot_vec), -1)
 anchor1_pose = ivy.concatenate((anchor1_xy, constant_z, anchor1_rot_vec), -1)
 anchor2_pose = ivy.concatenate((anchor2_xy, constant_z, anchor2_rot_vec), -1)
@@ -166,64 +165,66 @@
 x 3 x 4 interpolated_matrices = ivy_mech.rot_vec_pose_to_mat_pose
 (interpolated_poses) # sample drone body # num_anchors x num_body_points x 3
 anchor_body_points = drone.sample_body(anchor_matrices) # num_samples x
 num_body_points x 3 interpolated_body_points = drone.sample_body
 (interpolated_matrices) The sampled drone body xy positions during motion are
 shown below in the x-y plane. By tracing the body points for each of the four
 corners of the drone, we can see how the drone performs the 180 degree self-
-rotation about the z-axis during the motion. .. raw:: html
-         [docs/partial_source/images/sampled_drone_body_positions.png]
-**Manipulator Class** We now introduce the robot Manipulator class, which can
-be used to represent arbitrary robot manipulators. In this case, we consider
-the case of very simple 2-link manipulator, which is constrained to move in the
-x-y plane. The manipulator is specified by the DenavitâHartenberg parameters,
-as outlined in the newly derived class below. We assume a manipulator with two
-0.5m links, where a configuration with both joints angles at 0 degrees
-represents a upright link configuration. We specify a new set of target joint
-angles which corresponds with a forward reaching motion in the positive x
-direction. .. code-block:: python class SimpleManipulator(Manipulator): def
-__init__(self, base_inv_ext_mat=None): a_s = ivy.array([0.5, 0.5]) d_s =
-ivy.array([0., 0.]) alpha_s = ivy.array([0., 0.]) dh_joint_scales = ivy.ones(
-(2,)) dh_joint_offsets = ivy.array([-np.pi/2, 0.]) super().__init__(a_s, d_s,
-alpha_s, dh_joint_scales, dh_joint_offsets, base_inv_ext_mat) # create
-manipulator as ivy manipulator manipulator = SimpleManipulator() # joint angles
-# 1 x 2 start_joint_angles = ivy.array([[0., 0.]]) target_joint_angles =
-ivy.array([[-np.pi/4, -np.pi/4]]) # 1 x 2 anchor1_joint_angles = -ivy.array([
-[0.2, 0.6]])*np.pi/4 anchor2_joint_angles = -ivy.array([[0.5, 0.5]])*np.pi/
+rotation about the z-axis during the motion. .. image:: https://github.com/ivy-
+dl/robot/blob/master/docs/partial_source/images/
+sampled_drone_body_positions.png?raw=true :width: 100% **Manipulator Class** We
+now introduce the robot Manipulator class, which can be used to represent
+arbitrary robot manipulators. In this case, we consider the case of very simple
+2-link manipulator, which is constrained to move in the x-y plane. The
+manipulator is specified by the DenavitâHartenberg parameters, as outlined in
+the newly derived class below. We assume a manipulator with two 0.5m links,
+where a configuration with both joints angles at 0 degrees represents a upright
+link configuration. We specify a new set of target joint angles which
+corresponds with a forward reaching motion in the positive x direction. ..
+code-block:: python class SimpleManipulator(Manipulator): def __init__(self,
+base_inv_ext_mat=None): a_s = ivy.array([0.5, 0.5]) d_s = ivy.array([0., 0.])
+alpha_s = ivy.array([0., 0.]) dh_joint_scales = ivy.ones((2,)) dh_joint_offsets
+= ivy.array([-np.pi/2, 0.]) super().__init__(a_s, d_s, alpha_s,
+dh_joint_scales, dh_joint_offsets, base_inv_ext_mat) # create manipulator as
+ivy manipulator manipulator = SimpleManipulator() # joint angles # 1 x 2
+start_joint_angles = ivy.array([[0., 0.]]) target_joint_angles = ivy.array([[-
+np.pi/4, -np.pi/4]]) # 1 x 2 anchor1_joint_angles = -ivy.array([[0.2,
+0.6]])*np.pi/4 anchor2_joint_angles = -ivy.array([[0.5, 0.5]])*np.pi/
 4 anchor3_joint_angles = -ivy.array([[0.8, 0.4]])*np.pi/4 # num_anchors x 2
 anchor_joint_angles = ivy.concatenate( (start_joint_angles,
 anchor1_joint_angles, anchor2_joint_angles, anchor3_joint_angles,
 target_joint_angles), 0) # interpolated joint angles # num_anchors x 2
 interpolated_joint_angles = ivy_robot.sample_spline_path(anchor_points,
 anchor_joint_angles, query_points) The interpolated joint angles are presented
-below. .. raw:: html
-    [docs/partial_source/images/interpolated_manipulator_joint_angles.png]
-In a similar fashion to how the drone body was sampled in the previous example,
-we next use these interpolated joint angles to sample the link positions for
-the manipulator. .. code-block:: python # sample links # num_anchors x
-num_link_points x 3 anchor_link_points = manipulator.sample_links
+below. .. image:: https://github.com/ivy-dl/robot/blob/master/docs/
+partial_source/images/interpolated_manipulator_joint_angles.png?raw=true :
+width: 100% In a similar fashion to how the drone body was sampled in the
+previous example, we next use these interpolated joint angles to sample the
+link positions for the manipulator. .. code-block:: python # sample links #
+num_anchors x num_link_points x 3 anchor_link_points = manipulator.sample_links
 (anchor_joint_angles, samples_per_metre=5) # num_anchors x num_link_points x 3
 interpolated_link_points = manipulator.sample_links(interpolated_joint_angles,
 samples_per_metre=5) we show the sampled link positions during the course of
-the forward reaching motion in the x-y plane below. .. raw:: html
-          [docs/partial_source/images/sampled_manipulator_links.png]
-Interactive Demos ----------------- The main benefit of the library is not
-simply the ability to sample paths, but to optimize these paths using
-gradients. For exmaple, the body or link sample positions can be used to query
-the signed distance function (SDF) of a 3D scene in batch. Then, assuming the
-spline anchor points to be free variables, the gradients of the mean sampled
-SDF and a path length metric can be computed with respect to the anchor points.
-The anhcor points can then be incrementally updated using gradient descent on
-this loss function. We provide two further demo scripts which outline this
-gradient-based path optimization in a 3D scene. Rather than presenting the code
-here, we show visualizations of the demos. The scripts for these demos can be
-found in the interactive_ demos folder. **RigidMobile Planning** The first demo
-uses the ``RigidMobile`` class to optimzie the motion of a drone to a target
-pose, making use of functions ``ivy_robot.sample_spline_path`` and
-``ivy_robot.RigidMobile.sample_body``. .. raw:: html
+the forward reaching motion in the x-y plane below. .. image:: https://
+github.com/ivy-dl/robot/blob/master/docs/partial_source/images/
+sampled_manipulator_links.png?raw=true :width: 100% Interactive Demos ---------
+-------- The main benefit of the library is not simply the ability to sample
+paths, but to optimize these paths using gradients. For exmaple, the body or
+link sample positions can be used to query the signed distance function (SDF)
+of a 3D scene in batch. Then, assuming the spline anchor points to be free
+variables, the gradients of the mean sampled SDF and a path length metric can
+be computed with respect to the anchor points. The anhcor points can then be
+incrementally updated using gradient descent on this loss function. We provide
+two further demo scripts which outline this gradient-based path optimization in
+a 3D scene. Rather than presenting the code here, we show visualizations of the
+demos. The scripts for these demos can be found in the interactive_ demos
+folder. **RigidMobile Planning** The first demo uses the ``RigidMobile`` class
+to optimzie the motion of a drone to a target pose, making use of functions
+``ivy_robot.sample_spline_path`` and ``ivy_robot.RigidMobile.sample_body``. ..
+raw:: html
 [https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/
                         ivy_robot/demo_a.gif?raw=true]
 **Manipulator Planning** The second demo uses the ``MicoManipulator`` class,
 derived from ``Manipulator``, to optimzie the motion of a mico robot
 manipulator to a set of target joint angles, making use of functions
 ``ivy_robot.sample_spline_path`` and ``ivy_robot.Manipulator.sample_links``. ..
 raw:: html
```

### Comparing `ivy-robot-1.1.8/ivy_robot/manipulator.py` & `ivy-robot-1.1.9/ivy_robot/manipulator.py`

 * *Files identical despite different names*

### Comparing `ivy-robot-1.1.8/ivy_robot/planning.py` & `ivy-robot-1.1.9/ivy_robot/planning.py`

 * *Files identical despite different names*

### Comparing `ivy-robot-1.1.8/ivy_robot/rigid_mobile.py` & `ivy-robot-1.1.9/ivy_robot/rigid_mobile.py`

 * *Files identical despite different names*

### Comparing `ivy-robot-1.1.8/ivy_robot.egg-info/PKG-INFO` & `ivy-robot-1.1.9/ivy_robot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: ivy-robot
-Version: 1.1.8
+Version: 1.1.9
 Summary: Functions and classes for gradient-based robot motion planning, written in Ivy.
 Home-page: https://ivy-dl.org/robot
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/robot/
 Project-URL: Source, https://github.com/ivy-dl/robot
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **Functions and classes for gradient-based robot motion planning, written in Ivy.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 Contents
 --------
 
 * `Overview`_
 * `Run Through`_
 * `Interactive Demos`_
 * `Get Involed`_
@@ -47,14 +51,17 @@
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
 
 
 
 
 
 
 
@@ -151,15 +158,16 @@
     anchor_xy_positions = anchor_poses[..., 0:2]
 
     # num_samples x 2
     interpolated_xy_positions = interpolated_poses[..., 0:2]
 
 The interpolated xy positions and anchor positions from the path are shown below in the x-y plane.
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/interpolated_drone_poses.png?raw=true
+   :width: 100%
 
 **Rigid Mobile Class**
 
 We now introduce the ``RigidMobile`` robot class,
 which can be used to represent rigid jointless robots which are able to move freely.
 In this case, we consider the case of a drone executing 6DOF motion in a scene.
 
@@ -225,15 +233,16 @@
     # num_samples x num_body_points x 3
     interpolated_body_points = drone.sample_body(interpolated_matrices)
 
 The sampled drone body xy positions during motion are shown below in the x-y plane.
 By tracing the body points for each of the four corners of the drone,
 we can see how the drone performs the 180 degree self-rotation about the z-axis during the motion.
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/sampled_drone_body_positions.png?raw=true
+   :width: 100%
 
 **Manipulator Class**
 
 We now introduce the robot Manipulator class,
 which can be used to represent arbitrary robot manipulators.
 In this case, we consider the case of very simple 2-link manipulator,
 which is constrained to move in the x-y plane.
@@ -279,15 +288,16 @@
     # interpolated joint angles
 
     # num_anchors x 2
     interpolated_joint_angles = ivy_robot.sample_spline_path(anchor_points, anchor_joint_angles, query_points)
 
 The interpolated joint angles are presented below.
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/interpolated_manipulator_joint_angles.png?raw=true
+   :width: 100%
 
 In a similar fashion to how the drone body was sampled in the previous example,
 we next use these interpolated joint angles to sample the link positions for the manipulator.
 
 .. code-block:: python
 
     # sample links
@@ -296,15 +306,16 @@
     anchor_link_points = manipulator.sample_links(anchor_joint_angles, samples_per_metre=5)
 
     # num_anchors x num_link_points x 3
     interpolated_link_points = manipulator.sample_links(interpolated_joint_angles, samples_per_metre=5)
 
 we show the sampled link positions during the course of the forward reaching motion in the x-y plane below.
 
-
+.. image:: https://github.com/ivy-dl/robot/blob/master/docs/partial_source/images/sampled_manipulator_links.png?raw=true
+   :width: 100%
 
 Interactive Demos
 -----------------
 
 The main benefit of the library is not simply the ability to sample paths, but to optimize these paths using gradients.
 For exmaple, the body or link sample positions can be used to query the signed distance function (SDF) of a 3D scene in batch.
 Then, assuming the spline anchor points to be free variables,
@@ -318,22 +329,28 @@
 **RigidMobile Planning**
 
 The first demo uses the ``RigidMobile`` class to optimzie the motion of a drone to a target pose,
 making use of functions ``ivy_robot.sample_spline_path`` and ``ivy_robot.RigidMobile.sample_body``.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_robot/demo_a.png?raw=true
+   :width: 100%
+
 **Manipulator Planning**
 
 The second demo uses the ``MicoManipulator`` class, derived from ``Manipulator``,
 to optimzie the motion of a mico robot manipulator to a set of target joint angles,
 making use of functions ``ivy_robot.sample_spline_path`` and ``ivy_robot.Manipulator.sample_links``.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_robot/demo_b.png?raw=true
+   :width: 100%
+
 Get Involed
 -----------
 
 We hope the functions in this library are useful to a wide range of machine learning developers.
 However, there are many more areas of gradient-based motion planning and broader robotics
 which could be covered by this library.
```

