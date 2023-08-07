# Comparing `tmp/deltares-coastalhazardstoolkit-0.2.1.tar.gz` & `tmp/deltares-coastalhazardstoolkit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltares-coastalhazardstoolkit-0.2.1.tar", last modified: Fri Aug  4 19:06:18 2023, max compression
+gzip compressed data, was "deltares-coastalhazardstoolkit-0.2.2.tar", last modified: Mon Aug  7 19:40:21 2023, max compression
```

## Comparing `deltares-coastalhazardstoolkit-0.2.1.tar` & `deltares-coastalhazardstoolkit-0.2.2.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.879370 deltares-coastalhazardstoolkit-0.2.1/
--rw-rw-rw-   0        0        0    35823 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      376 2023-08-04 19:06:18.879370 deltares-coastalhazardstoolkit-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      923 2023-08-04 19:06:03.000000 deltares-coastalhazardstoolkit-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-04 19:06:18.879370 deltares-coastalhazardstoolkit-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.793242 deltares-coastalhazardstoolkit-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.795243 deltares-coastalhazardstoolkit-0.2.1/src/cht/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.801738 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/__init__.py
--rw-rw-rw-   0        0        0    26958 2023-06-09 14:37:46.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/bathymetry_database.py
--rw-rw-rw-   0        0        0    26344 2023-01-03 18:41:58.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/tiling.py
--rw-rw-rw-   0        0        0      803 2022-11-09 17:01:21.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/tiling_example.py
--rw-rw-rw-   0        0        0     1324 2023-01-03 19:45:23.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/tiling_example_gebco22.py
--rw-rw-rw-   0        0        0     1645 2023-06-05 18:25:14.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.803067 deltares-coastalhazardstoolkit-0.2.1/src/cht/beware/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/beware/__init__.py
--rw-rw-rw-   0        0        0    38019 2023-06-06 20:06:44.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/beware/beware.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.804348 deltares-coastalhazardstoolkit-0.2.1/src/cht/delft3dfm/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/delft3dfm/__init__.py
--rw-rw-rw-   0        0        0    45459 2023-02-18 18:54:56.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/delft3dfm/delft3dfm.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.812360 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-02-16 02:20:58.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/bathymetry.py
--rw-rw-rw-   0        0        0    17214 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/boundary_conditions.py
--rw-rw-rw-   0        0        0    18023 2023-06-09 15:38:31.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/grid.py
--rw-rw-rw-   0        0        0    31446 2023-06-07 17:46:39.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave.py
--rw-rw-rw-   0        0        0     4763 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave_builder.py
--rw-rw-rw-   0        0        0     6804 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave_domain.py
--rw-rw-rw-   0        0        0     5288 2023-05-15 15:51:19.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/input.py
--rw-rw-rw-   0        0        0     5454 2023-02-16 02:34:58.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/mask.py
--rw-rw-rw-   0        0        0     7393 2023-05-19 15:46:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/observation_points.py
--rw-rw-rw-   0        0        0     4004 2023-05-22 15:09:37.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/to_xugrid.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.820358 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/__init__.py
--rw-rw-rw-   0        0        0    11578 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_analysis.py
--rw-rw-rw-   0        0        0    26632 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_tc_forecast.py
--rw-rw-rw-   0        0        0    23025 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_tc_hindcast.py
--rw-rw-rw-   0        0        0     4688 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_tc_ufl_d01.py
--rw-rw-rw-   0        0        0    12331 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50.py
--rw-rw-rw-   0        0        0     9220 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_02.py
--rw-rw-rw-   0        0        0    14130 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_03.py
--rw-rw-rw-   0        0        0    15644 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_04.py
--rw-rw-rw-   0        0        0     6399 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_forecast_0p25.py
--rw-rw-rw-   0        0        0     4146 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_forecast_0p25_02.py
--rw-rw-rw-   0        0        0    58037 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/meteo.py
--rw-rw-rw-   0        0        0     2074 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/test_coamps.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.827229 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/__init__.py
--rw-rw-rw-   0        0        0     9328 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/deltares_ini.py
--rw-rw-rw-   0        0        0     3138 2023-06-06 20:06:44.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/fileops.py
--rw-rw-rw-   0        0        0     4434 2023-02-16 02:05:36.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/geometry.py
--rw-rw-rw-   0        0        0     2901 2023-02-12 05:38:17.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/misc_tools.py
--rw-rw-rw-   0        0        0     4440 2023-06-07 20:21:34.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/pli_file.py
--rw-rw-rw-   0        0        0     3833 2023-08-04 18:05:53.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/prob_maps.py
--rw-rw-rw-   0        0        0     6472 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/sftp.py
--rw-rw-rw-   0        0        0     9845 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/tekal.py
--rw-rw-rw-   0        0        0     5317 2023-05-17 17:18:05.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/xmlkit.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.828706 deltares-coastalhazardstoolkit-0.2.1/src/cht/model_builder/
--rw-rw-rw-   0        0        0    22934 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/model_builder/model_builder.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.830942 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/__init__.py
--rw-rw-rw-   0        0        0     7791 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nest1.py
--rw-rw-rw-   0        0        0    33815 2023-07-28 19:48:45.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nest2.py
--rw-rw-rw-   0        0        0    37037 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nesting.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.834309 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/
--rw-rw-rw-   0        0        0       92 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/__init__.py
--rw-rw-rw-   0        0        0      993 2023-05-17 17:26:56.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/_ndbc.py
--rw-rw-rw-   0        0        0     1127 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/_noaa_coops.py
--rw-rw-rw-   0        0        0     1181 2023-05-17 17:33:01.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/observation_stations.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.837309 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/__init__.py
--rw-rw-rw-   0        0        0      590 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/deshoal.py
--rw-rw-rw-   0        0        0     1238 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/disper.py
--rw-rw-rw-   0        0        0     7860 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/vo21.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.841538 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/__init__.py
--rw-rw-rw-   0        0        0    66271 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/quadtree.py
--rw-rw-rw-   0        0        0    11167 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/regulargrid.py
--rw-rw-rw-   0        0        0    46392 2023-07-25 20:52:10.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/sfincs.py
--rw-rw-rw-   0        0        0    12920 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/sfincs_builder.py
--rw-rw-rw-   0        0        0    48185 2023-01-05 19:25:34.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/subgrid.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.851369 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/
--rw-rw-rw-   0        0        0       92 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/__init__.py
--rw-rw-rw-   0        0        0    12996 2023-06-14 15:50:17.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/boundary_conditions.py
--rw-rw-rw-   0        0        0    46524 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/grid.py
--rw-rw-rw-   0        0        0     8587 2023-06-07 20:03:21.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/input.py
--rw-rw-rw-   0        0        0    22639 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/mask.py
--rw-rw-rw-   0        0        0     3308 2023-05-27 14:29:58.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/observation_points.py
--rw-rw-rw-   0        0        0    78823 2023-06-01 20:37:42.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/quadtree_grid.py
--rw-rw-rw-   0        0        0    25105 2023-06-02 21:09:28.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/quadtree_grid_snapwave.py
--rw-rw-rw-   0        0        0    18022 2023-05-25 16:37:22.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/regular_grid.py
--rw-rw-rw-   0        0        0    46298 2023-06-14 14:43:07.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/sfincs.py
--rw-rw-rw-   0        0        0    11719 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/sfincs_builder.py
--rw-rw-rw-   0        0        0    20663 2023-06-08 11:04:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/snapwave.py
--rw-rw-rw-   0        0        0    46524 2023-06-14 15:18:38.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/subgrid.py
--rw-rw-rw-   0        0        0     1707 2023-06-07 20:14:52.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/wave_makers.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.852369 deltares-coastalhazardstoolkit-0.2.1/src/cht/snapwave/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/snapwave/__init__.py
--rw-rw-rw-   0        0        0    24908 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/snapwave/mesh.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.859369 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/__init__.py
--rw-rw-rw-   0        0        0     7255 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/astro.py
--rw-rw-rw-   0        0        0     7524 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/constituent.py
--rw-rw-rw-   0        0        0     3542 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/fes2014.py
--rw-rw-rw-   0        0        0     4860 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/nodal_corrections.py
--rw-rw-rw-   0        0        0     1479 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/predict.py
--rw-rw-rw-   0        0        0      687 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/test_tide_database.py
--rw-rw-rw-   0        0        0    15388 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide.py
--rw-rw-rw-   0        0        0     3365 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide_model.py
--rw-rw-rw-   0        0        0      965 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide_predict.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.860370 deltares-coastalhazardstoolkit-0.2.1/src/cht/tiling/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tiling/__init__.py
--rw-rw-rw-   0        0        0    32567 2023-06-06 20:06:44.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tiling/tiling.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.864370 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/
--rw-rw-rw-   0        0        0    10203 2023-05-17 12:40:56.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/cyclone_track_database.py
--rw-rw-rw-   0        0        0     2406 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/test_meteo.py
--rw-rw-rw-   0        0        0      480 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/test_track.py
--rw-rw-rw-   0        0        0     1517 2023-01-25 14:41:34.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/testje.py
--rw-rw-rw-   0        0        0     1091 2023-01-25 14:41:34.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/testje_forecasting.py
--rw-rw-rw-   0        0        0   102706 2023-07-29 20:44:35.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/tropical_cyclone.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.866370 deltares-coastalhazardstoolkit-0.2.1/src/cht/watersheds/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/watersheds/__init__.py
--rw-rw-rw-   0        0        0     7923 2022-11-10 16:13:06.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/watersheds/watersheds.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.867370 deltares-coastalhazardstoolkit-0.2.1/src/cht/xbeach/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/xbeach/__init__.py
--rw-rw-rw-   0        0        0    28049 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.1/src/cht/xbeach/xbeach.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:06:18.878377 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/
--rw-rw-rw-   0        0        0      376 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3455 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-04 19:06:18.000000 deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.890704 deltares-coastalhazardstoolkit-0.2.2/
+-rw-rw-rw-   0        0        0    35823 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      376 2023-08-07 19:40:21.890187 deltares-coastalhazardstoolkit-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2023-08-07 19:39:11.000000 deltares-coastalhazardstoolkit-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 19:40:21.890704 deltares-coastalhazardstoolkit-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.393722 deltares-coastalhazardstoolkit-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.399526 deltares-coastalhazardstoolkit-0.2.2/src/cht/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.423492 deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/__init__.py
+-rw-rw-rw-   0        0        0    26958 2023-06-09 14:37:46.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/bathymetry_database.py
+-rw-rw-rw-   0        0        0    26344 2023-01-03 18:41:58.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/tiling.py
+-rw-rw-rw-   0        0        0      803 2022-11-09 17:01:21.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/tiling_example.py
+-rw-rw-rw-   0        0        0     1324 2023-01-03 19:45:23.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/tiling_example_gebco22.py
+-rw-rw-rw-   0        0        0     1645 2023-06-05 18:25:14.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.426492 deltares-coastalhazardstoolkit-0.2.2/src/cht/beware/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/beware/__init__.py
+-rw-rw-rw-   0        0        0    38019 2023-06-06 20:06:44.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/beware/beware.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.428483 deltares-coastalhazardstoolkit-0.2.2/src/cht/delft3dfm/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/delft3dfm/__init__.py
+-rw-rw-rw-   0        0        0    45459 2023-02-18 18:54:56.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/delft3dfm/delft3dfm.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.473759 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-02-16 02:20:58.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/bathymetry.py
+-rw-rw-rw-   0        0        0    17214 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/boundary_conditions.py
+-rw-rw-rw-   0        0        0    18023 2023-06-09 15:38:31.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/grid.py
+-rw-rw-rw-   0        0        0    31446 2023-06-07 17:46:39.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/hurrywave.py
+-rw-rw-rw-   0        0        0     4763 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/hurrywave_builder.py
+-rw-rw-rw-   0        0        0     6804 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/hurrywave_domain.py
+-rw-rw-rw-   0        0        0     5288 2023-05-15 15:51:19.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/input.py
+-rw-rw-rw-   0        0        0     5454 2023-02-16 02:34:58.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/mask.py
+-rw-rw-rw-   0        0        0     7393 2023-05-19 15:46:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/observation_points.py
+-rw-rw-rw-   0        0        0     4004 2023-05-22 15:09:37.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/to_xugrid.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.544226 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/__init__.py
+-rw-rw-rw-   0        0        0    11578 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/coamps_analysis.py
+-rw-rw-rw-   0        0        0    26632 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/coamps_tc_forecast.py
+-rw-rw-rw-   0        0        0    23025 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/coamps_tc_hindcast.py
+-rw-rw-rw-   0        0        0     4688 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/coamps_tc_ufl_d01.py
+-rw-rw-rw-   0        0        0    12331 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_anl_0p50.py
+-rw-rw-rw-   0        0        0     9220 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_anl_0p50_02.py
+-rw-rw-rw-   0        0        0    14130 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_anl_0p50_03.py
+-rw-rw-rw-   0        0        0    15644 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_anl_0p50_04.py
+-rw-rw-rw-   0        0        0     6399 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_forecast_0p25.py
+-rw-rw-rw-   0        0        0     4146 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_forecast_0p25_02.py
+-rw-rw-rw-   0        0        0    58037 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/meteo.py
+-rw-rw-rw-   0        0        0     2074 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/test_coamps.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.583465 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/__init__.py
+-rw-rw-rw-   0        0        0      828 2023-08-07 16:59:17.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/argo.py
+-rw-rw-rw-   0        0        0     9328 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/deltares_ini.py
+-rw-rw-rw-   0        0        0     3138 2023-06-06 20:06:44.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/fileops.py
+-rw-rw-rw-   0        0        0     4434 2023-02-16 02:05:36.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/geometry.py
+-rw-rw-rw-   0        0        0     2901 2023-02-12 05:38:17.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/misc_tools.py
+-rw-rw-rw-   0        0        0     4440 2023-06-07 20:21:34.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/pli_file.py
+-rw-rw-rw-   0        0        0     3833 2023-08-04 18:05:53.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/prob_maps.py
+-rw-rw-rw-   0        0        0     6472 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/sftp.py
+-rw-rw-rw-   0        0        0     9845 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/tekal.py
+-rw-rw-rw-   0        0        0     5317 2023-05-17 17:18:05.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/xmlkit.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.592464 deltares-coastalhazardstoolkit-0.2.2/src/cht/model_builder/
+-rw-rw-rw-   0        0        0    22934 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/model_builder/model_builder.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.596464 deltares-coastalhazardstoolkit-0.2.2/src/cht/nesting/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/nesting/__init__.py
+-rw-rw-rw-   0        0        0     7791 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/nesting/nest1.py
+-rw-rw-rw-   0        0        0    33815 2023-07-28 19:48:45.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/nesting/nest2.py
+-rw-rw-rw-   0        0        0    37037 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/nesting/nesting.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.639357 deltares-coastalhazardstoolkit-0.2.2/src/cht/observation_stations/
+-rw-rw-rw-   0        0        0       92 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/observation_stations/__init__.py
+-rw-rw-rw-   0        0        0      993 2023-05-17 17:26:56.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/observation_stations/_ndbc.py
+-rw-rw-rw-   0        0        0     1127 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/observation_stations/_noaa_coops.py
+-rw-rw-rw-   0        0        0     1181 2023-05-17 17:33:01.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/observation_stations/observation_stations.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.661882 deltares-coastalhazardstoolkit-0.2.2/src/cht/physics/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/physics/__init__.py
+-rw-rw-rw-   0        0        0      590 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/physics/deshoal.py
+-rw-rw-rw-   0        0        0     1238 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/physics/disper.py
+-rw-rw-rw-   0        0        0     7860 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/physics/vo21.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.704580 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/__init__.py
+-rw-rw-rw-   0        0        0    66271 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/quadtree.py
+-rw-rw-rw-   0        0        0    11167 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/regulargrid.py
+-rw-rw-rw-   0        0        0    46392 2023-07-25 20:52:10.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/sfincs.py
+-rw-rw-rw-   0        0        0    12920 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/sfincs_builder.py
+-rw-rw-rw-   0        0        0    48185 2023-01-05 19:25:34.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/subgrid.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.791790 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/
+-rw-rw-rw-   0        0        0       92 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/__init__.py
+-rw-rw-rw-   0        0        0    12996 2023-06-14 15:50:17.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/boundary_conditions.py
+-rw-rw-rw-   0        0        0    46524 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/grid.py
+-rw-rw-rw-   0        0        0     8587 2023-06-07 20:03:21.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/input.py
+-rw-rw-rw-   0        0        0    22639 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/mask.py
+-rw-rw-rw-   0        0        0     3308 2023-05-27 14:29:58.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/observation_points.py
+-rw-rw-rw-   0        0        0    78823 2023-06-01 20:37:42.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/quadtree_grid.py
+-rw-rw-rw-   0        0        0    25105 2023-06-02 21:09:28.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/quadtree_grid_snapwave.py
+-rw-rw-rw-   0        0        0    18022 2023-05-25 16:37:22.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/regular_grid.py
+-rw-rw-rw-   0        0        0    46298 2023-06-14 14:43:07.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/sfincs.py
+-rw-rw-rw-   0        0        0    11719 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/sfincs_builder.py
+-rw-rw-rw-   0        0        0    20663 2023-06-08 11:04:18.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/snapwave.py
+-rw-rw-rw-   0        0        0    46524 2023-06-14 15:18:38.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/subgrid.py
+-rw-rw-rw-   0        0        0     1707 2023-06-07 20:14:52.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/wave_makers.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.797793 deltares-coastalhazardstoolkit-0.2.2/src/cht/snapwave/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/snapwave/__init__.py
+-rw-rw-rw-   0        0        0    24908 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/snapwave/mesh.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.826809 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/__init__.py
+-rw-rw-rw-   0        0        0     7255 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/astro.py
+-rw-rw-rw-   0        0        0     7524 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/constituent.py
+-rw-rw-rw-   0        0        0     3542 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/fes2014.py
+-rw-rw-rw-   0        0        0     4860 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/nodal_corrections.py
+-rw-rw-rw-   0        0        0     1479 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/predict.py
+-rw-rw-rw-   0        0        0      687 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/test_tide_database.py
+-rw-rw-rw-   0        0        0    15388 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/tide.py
+-rw-rw-rw-   0        0        0     3365 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/tide_model.py
+-rw-rw-rw-   0        0        0      965 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/tide_predict.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.828801 deltares-coastalhazardstoolkit-0.2.2/src/cht/tiling/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tiling/__init__.py
+-rw-rw-rw-   0        0        0    32567 2023-06-06 20:06:44.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tiling/tiling.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.865877 deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/
+-rw-rw-rw-   0        0        0    10203 2023-05-17 12:40:56.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/cyclone_track_database.py
+-rw-rw-rw-   0        0        0     2406 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/test_meteo.py
+-rw-rw-rw-   0        0        0      480 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/test_track.py
+-rw-rw-rw-   0        0        0     1517 2023-01-25 14:41:34.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/testje.py
+-rw-rw-rw-   0        0        0     1091 2023-01-25 14:41:34.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/testje_forecasting.py
+-rw-rw-rw-   0        0        0   102706 2023-07-29 20:44:35.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/tropical_cyclone.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.871992 deltares-coastalhazardstoolkit-0.2.2/src/cht/watersheds/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/watersheds/__init__.py
+-rw-rw-rw-   0        0        0     7923 2022-11-10 16:13:06.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/watersheds/watersheds.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.873005 deltares-coastalhazardstoolkit-0.2.2/src/cht/xbeach/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/xbeach/__init__.py
+-rw-rw-rw-   0        0        0    28049 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.2/src/cht/xbeach/xbeach.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:40:21.888902 deltares-coastalhazardstoolkit-0.2.2/src/deltares_coastalhazardstoolkit.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-08-07 19:40:21.000000 deltares-coastalhazardstoolkit-0.2.2/src/deltares_coastalhazardstoolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3476 2023-08-07 19:40:21.000000 deltares-coastalhazardstoolkit-0.2.2/src/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 19:40:21.000000 deltares-coastalhazardstoolkit-0.2.2/src/deltares_coastalhazardstoolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      172 2023-08-07 19:40:21.000000 deltares-coastalhazardstoolkit-0.2.2/src/deltares_coastalhazardstoolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 19:40:21.000000 deltares-coastalhazardstoolkit-0.2.2/src/deltares_coastalhazardstoolkit.egg-info/top_level.txt
```

### Comparing `deltares-coastalhazardstoolkit-0.2.1/LICENSE` & `deltares-coastalhazardstoolkit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/pyproject.toml` & `deltares-coastalhazardstoolkit-0.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.2.1"
+version = "0.2.2"
 name = "deltares-coastalhazardstoolkit"
 authors = [
     {name = "Maarten van Ormondt", email = "maarten.vanormondt@deltares-usa.us"},
     {name = "Roel de Goede", email = "roel.degoede@deltares.nl"},
     {name = "Kees Nederhoff", email = "kees.nederhoff@deltares-usa.us"},
     {name = "Tim Leijnse", email = "tim.leijnse@deltares.nl"},
     {name = "Panos Athanasiou", email = "panos.athanasiou@deltares.nl"},
@@ -30,9 +30,10 @@
     "noaa-coops",
     "metpy",
     "siphon",
     "netCDF4",
     "mat73",
     "tabulate",
     "pyyaml",
-    "toml"
+    "toml",
+	"hera"
 ]
```

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/bathymetry_database.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/bathymetry_database.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/tiling.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/tiling.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/tiling_example.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/tiling_example.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/tiling_example_gebco22.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/tiling_example_gebco22.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/bathymetry/utils.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/bathymetry/utils.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/beware/beware.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/beware/beware.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/delft3dfm/delft3dfm.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/delft3dfm/delft3dfm.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/bathymetry.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/bathymetry.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/boundary_conditions.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/grid.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/grid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/hurrywave.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave_builder.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/hurrywave_builder.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/hurrywave_domain.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/hurrywave_domain.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/input.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/input.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/mask.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/mask.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/observation_points.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/observation_points.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/hurrywave/to_xugrid.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/hurrywave/to_xugrid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_analysis.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/coamps_analysis.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_tc_forecast.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/coamps_tc_forecast.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_tc_hindcast.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/coamps_tc_hindcast.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/coamps_tc_ufl_d01.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/coamps_tc_ufl_d01.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_anl_0p50.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_02.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_anl_0p50_02.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_03.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_anl_0p50_03.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_anl_0p50_04.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_anl_0p50_04.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_forecast_0p25.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_forecast_0p25.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/gfs_forecast_0p25_02.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/gfs_forecast_0p25_02.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/meteo.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/meteo.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/meteo/test_coamps.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/meteo/test_coamps.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/deltares_ini.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/deltares_ini.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/fileops.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/fileops.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/geometry.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/geometry.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/misc_tools.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/misc_tools.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/pli_file.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/pli_file.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/prob_maps.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/prob_maps.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/sftp.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/sftp.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/tekal.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/tekal.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/misc/xmlkit.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/misc/xmlkit.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/model_builder/model_builder.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/model_builder/model_builder.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nest1.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/nesting/nest1.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nest2.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/nesting/nest2.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/nesting/nesting.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/nesting/nesting.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/_ndbc.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/observation_stations/_ndbc.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/_noaa_coops.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/observation_stations/_noaa_coops.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/observation_stations/observation_stations.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/observation_stations/observation_stations.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/deshoal.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/physics/deshoal.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/disper.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/physics/disper.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/physics/vo21.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/physics/vo21.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/quadtree.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/quadtree.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/regulargrid.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/regulargrid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/sfincs.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/sfincs.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/sfincs_builder.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/sfincs_builder.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs/subgrid.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs/subgrid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/boundary_conditions.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/grid.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/grid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/input.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/input.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/mask.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/mask.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/observation_points.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/observation_points.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/quadtree_grid.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/quadtree_grid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/quadtree_grid_snapwave.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/quadtree_grid_snapwave.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/regular_grid.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/regular_grid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/sfincs.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/sfincs.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/sfincs_builder.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/sfincs_builder.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/snapwave.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/snapwave.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/subgrid.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/subgrid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/sfincs2/wave_makers.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/sfincs2/wave_makers.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/snapwave/mesh.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/snapwave/mesh.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/astro.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/astro.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/constituent.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/constituent.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/fes2014.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/fes2014.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/nodal_corrections.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/nodal_corrections.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/predict.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/predict.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/test_tide_database.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/test_tide_database.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/tide.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide_model.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/tide_model.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tide/tide_predict.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tide/tide_predict.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tiling/tiling.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tiling/tiling.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/cyclone_track_database.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/cyclone_track_database.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/test_meteo.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/test_meteo.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/testje.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/testje.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/testje_forecasting.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/testje_forecasting.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/tropical_cyclone/tropical_cyclone.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/tropical_cyclone/tropical_cyclone.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/watersheds/watersheds.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/watersheds/watersheds.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/cht/xbeach/xbeach.py` & `deltares-coastalhazardstoolkit-0.2.2/src/cht/xbeach/xbeach.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.1/src/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt` & `deltares-coastalhazardstoolkit-0.2.2/src/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/cht/meteo/gfs_anl_0p50_03.py
 src/cht/meteo/gfs_anl_0p50_04.py
 src/cht/meteo/gfs_forecast_0p25.py
 src/cht/meteo/gfs_forecast_0p25_02.py
 src/cht/meteo/meteo.py
 src/cht/meteo/test_coamps.py
 src/cht/misc/__init__.py
+src/cht/misc/argo.py
 src/cht/misc/deltares_ini.py
 src/cht/misc/fileops.py
 src/cht/misc/geometry.py
 src/cht/misc/misc_tools.py
 src/cht/misc/pli_file.py
 src/cht/misc/prob_maps.py
 src/cht/misc/sftp.py
```

