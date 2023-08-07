# Comparing `tmp/tud_sumo-1.2.2.tar.gz` & `tmp/tud_sumo-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tud_sumo-1.2.2.tar", last modified: Tue Jul 18 15:50:00 2023, max compression
+gzip compressed data, was "tud_sumo-1.3.0.tar", last modified: Mon Aug  7 15:05:18 2023, max compression
```

## Comparing `tud_sumo-1.2.2.tar` & `tud_sumo-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-18 15:50:00.232788 tud_sumo-1.2.2/
--rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.2.2/.gitattributes
--rw-r--r--   0 callumevans (50765939) 1653728465       78 2023-05-26 14:50:47.000000 tud_sumo-1.2.2/.gitignore
--rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.2.2/LICENSE
--rw-r--r--   0 callumevans (50765939) 1653728465     4694 2023-07-18 15:50:00.232642 tud_sumo-1.2.2/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465     3087 2023-07-18 15:47:28.000000 tud_sumo-1.2.2/README.md
--rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-07-18 15:47:40.000000 tud_sumo-1.2.2/pyproject.toml
--rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-07-18 15:50:00.232833 tud_sumo-1.2.2/setup.cfg
--rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.2.2/setup.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-18 15:50:00.231576 tud_sumo-1.2.2/tud_sumo/
--rw-r--r--   0 callumevans (50765939) 1653728465    19186 2023-07-18 15:44:58.000000 tud_sumo-1.2.2/tud_sumo/tud_sumo.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-18 15:50:00.232460 tud_sumo-1.2.2/tud_sumo.egg-info/
--rw-r--r--   0 callumevans (50765939) 1653728465     4694 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/requires.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-08-07 15:05:18.742495 tud_sumo-1.3.0/
+-rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.3.0/.gitattributes
+-rw-r--r--   0 callumevans (50765939) 1653728465       78 2023-05-26 14:50:47.000000 tud_sumo-1.3.0/.gitignore
+-rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.3.0/LICENSE
+-rw-r--r--   0 callumevans (50765939) 1653728465     6333 2023-08-07 15:05:18.742367 tud_sumo-1.3.0/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465     4726 2023-08-07 15:02:25.000000 tud_sumo-1.3.0/README.md
+-rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-08-07 15:02:42.000000 tud_sumo-1.3.0/pyproject.toml
+-rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-08-07 15:05:18.742537 tud_sumo-1.3.0/setup.cfg
+-rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.3.0/setup.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-08-07 15:05:18.741461 tud_sumo-1.3.0/tud_sumo/
+-rw-r--r--   0 callumevans (50765939) 1653728465    13074 2023-08-07 14:37:14.000000 tud_sumo-1.3.0/tud_sumo/plot.py
+-rw-r--r--   0 callumevans (50765939) 1653728465    29537 2023-08-07 14:35:48.000000 tud_sumo-1.3.0/tud_sumo/tud_sumo.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-08-07 15:05:18.742190 tud_sumo-1.3.0/tud_sumo.egg-info/
+-rw-r--r--   0 callumevans (50765939) 1653728465     6333 2023-08-07 15:05:18.000000 tud_sumo-1.3.0/tud_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      264 2023-08-07 15:05:18.000000 tud_sumo-1.3.0/tud_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-08-07 15:05:18.000000 tud_sumo-1.3.0/tud_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-08-07 15:05:18.000000 tud_sumo-1.3.0/tud_sumo.egg-info/requires.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-08-07 15:05:18.000000 tud_sumo-1.3.0/tud_sumo.egg-info/top_level.txt
```

### Comparing `tud_sumo-1.2.2/LICENSE` & `tud_sumo-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tud_sumo-1.2.2/README.md` & `tud_sumo-1.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -4,46 +4,51 @@
 
 ## Requirements 
 
 Required packages are: `tqdm`, `matplotlib` and `traci`.
 
 ## Updates
 
-This is version '1.2.2', with the changelog:
-  - Added `sim.get_vehicle_route()`
-  - Added `flatten` option to `sim.get_last_step_vehicles()`
+This is version '1.3.0'. The changelog is:
+  - Added Junction tracking
+  - Added Plotter objects
+  - Added better SUMO vType handling
+  - `sim_data` is automatically appended and stored in the `Simulation` object, instead of using `prev_data`
+  - Removed default junctions
 
 Check changes and previous versions through the project's [GitHub repository](https://github.com/calluume/tud_sumo).
 
-## Usage examples
+## Simulation Class
 
 ```python    
 from tud_sumo import tud_sumo
 
-sim = tud_sumo.Simulation()
+sim = tud_sumo.Simulation(all_vtypes=list_of_vehicle_types)
 sim.start("files/scenario.sumocfg", gui=True)
 ```
 
 The phase dictionary is a dictionary containing the phases and times. `math.inf` will set a light permanently, and `'-'` will keep that movement on the same setting as the previous phase. `sim.set_phases()` will then start these settings within the simulation on the next time step. If no phase dictionary is given, the simulation will use the default SUMO logic.
 
 ```python
 phase_dictionary = {'junctionID': {'phases': [ 'ggrryy', 'rryygg', 'yyggrr', 'rrrr--' ], # Phase light settings
                                    'times':  [ 10.12345, 10.12345, 10.12345, math.inf ]}} # Phase durations
 
 sim.set_phases(phase_dictionary)
 ```
 
-Use `sim.step_through()` to run through the simulation, collecting and aggregating the simulation data. This will return a dictionary containing all data collected, which can be used again as `prev_data` if continuing the simulation, meaning all data is appended and aggregated correctly throughout the whole runtime. This will contain all detector and vehicle information, although detectors and vehicle types can be specified using `detector_list` and `vTypes` respectively. To improve performance, set `sim.get_individual_vehicles = False` to not collect all individual vehicles' data at each time step when not needed.
+Use `sim.step_through()` to run through the simulation, collecting and aggregating the simulation data. This will return a dictionary containing all aggregated data collected. This will contain all detector and vehicle information, although detectors and vehicle types can be specified using `detector_list` and `vTypes` respectively. Data from calls to `sim.step_through()` is automatically aggregated and appended together, although to collect data independent from other runs, set `append_data` to false. Note, this will reset the data stored in the `Simulation` object.
 
-The `example_data.json` file shows the output of the `step_through` function.
+To improve performance, set `sim.get_individual_vehicles = False` to not collect all individual vehicles' data at each time step when not needed.
+
+The `example_data.json` file shows the output of the `step_through` function, which can also be saved as a JSON file using `sim.save_data()`.
 
 ```python
-sim_data = sim.step_through(end_step=1000)                    # Run simulation until step 1000
-sim_data = sim.step_through(n_steps=1000, prev_data=sim_data) # Run simulation for 1000 steps
-sim_data = sim.step_through(sim_dur=1000, prev_data=sim_data) # Run simulation for 1000s
+sim_data = sim.step_through(end_step=1000) # Run simulation until step 1000
+sim_data = sim.step_through(n_steps=1000)  # Run simulation for 1000 steps
+sim_data = sim.step_through(sim_dur=1000)  # Run simulation for 1000s
 ```
 
 Use `sim.get_vehicle_data()` and `sim.get_all_vehicle_data()` to get individual/all vehicles' data during the simulation. `sim.get_last_step_vehicles()` can also be used to get the list of vehicle IDs of those that passed over specified (or all) detectors.
 
 ```python
 bike = sim.get_vehicle_data('bike1')
 all_cars = sim.get_all_vehicle_data(types=['cars'])
@@ -53,8 +58,39 @@
 Use `sim.is_running()` to test if the simulation has ended and run until it has, according to the simulation end time in the SUMO config file. This will call `sim.end()`, but this can also be done manually at any other point.
 
 ```python
 while sim.is_running():
     sim_data = sim.step_through(prev_data=sim_data)
 
 sim.end()
-```
+
+sim.save_data("simulation_data.json")
+```
+
+## Junction Class
+
+It is now possible to track specific junctions and collect vehicle and traffic light data using the `Junction` class. This is started using the `sim.start_junc_tracking()` function. By default, all junctions with traffic lights are tracked, although a list of junction IDs can be given.
+
+The traffic light status at a junction is automatically tracked when one is present, but to track traffic flow, use a `junc_params` dictionary to define inflow and outflow detectors. The type of vehicles being tracked can also be specified using `"flow_vtypes"` in the dictionary.
+
+```python
+junc_params = {'junc_id': {
+                "inflow_detectors":  ["in_1", "in_2"],
+                "outflow_detectors": ["out_1", "out_2"],
+                "flow_vtypes":       ["cars", "bikes"]}}
+sim.start_junc_tracking(junc_params)
+```
+
+## Plotter Class
+
+The `Plotter` class is used to visualise the simulation data. Initialise the `Plotter` object with either the current `Simulation` object, `sim_data` dictionary or the filepath to a previously saved `sim_data` file.
+
+```python
+plotter = Plotter(sim)
+
+plotter.plot_vehicle_data("vehicle")
+
+plotter.plot_junc_flows('J0')
+plotter.plot_tl_colours('J0')
+```
+
+Both `plotter.plot_junc_flows()` and `plotter.plot_tl_colours()` both require junction tracking during the simulation.
```

### Comparing `tud_sumo-1.2.2/pyproject.toml` & `tud_sumo-1.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tud_sumo"
-version = "1.2.2"
+version = "1.3.0"
 description = "TU Delft SUMO wrapper"
 readme = "README.md"
 authors = [{ name = "Callum Evans", email = "c.evans@tudelft.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

