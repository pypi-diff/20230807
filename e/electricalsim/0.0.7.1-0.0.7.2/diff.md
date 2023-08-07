# Comparing `tmp/electricalsim-0.0.7.1.tar.gz` & `tmp/electricalsim-0.0.7.2.tar.gz`

## Comparing `electricalsim-0.0.7.1.tar` & `electricalsim-0.0.7.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    18645 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/README.md
--rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/10_PF4.png
--rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/11_PF_tooltips.png
--rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/12_App_settings.png
--rw-r--r--   0        0        0    50389 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/13_Disabling_nodes.png
--rw-r--r--   0        0        0   114751 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/14_Context_menu.png
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/15_Extension_manager.png
--rw-r--r--   0        0        0   124772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/1_Main_Window.png
--rw-r--r--   0        0        0   122916 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/1_Main_Window_dark.png
--rw-r--r--   0        0        0   149680 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/2_Dialogs.png
--rw-r--r--   0        0        0    25172 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/3_Widgets.png
--rw-r--r--   0        0        0   134645 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/4_Pandapower_DataFrames.png
--rw-r--r--   0        0        0    16870 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/5_Connections_angle_b.png
--rw-r--r--   0        0        0    21425 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/5_Connections_curved_b.png
--rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/5_Connections_straight_b.png
--rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/6_Line_and_transformer_nodes.png
--rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/7_PF1.png
--rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/8_PF2.png
--rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/9_PF3.png
--rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/img/app_icon.png
--rw-r--r--   0        0        0    22462 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/Electrical_Grid_Simulator.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/__init__.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/config.ini
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/egs_create_shortcut.py
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/egs_run.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/version.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/electricalsim.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/modules.xml
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/workspace.xml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/extensions/extension_classes.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/hotkeys/hotkey_functions.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/hotkeys/hotkeys.json
--rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.ico
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.png
--rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.svg
--rw-r--r--   0        0        0    30015 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/auxiliary.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/calculations.py
--rw-r--r--   0        0        0   213066 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/electricalGraph.py
--rw-r--r--   0        0        0    81561 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/main_components.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/lib/table_widget.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/about_dialog.ui
--rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/aload_dialog.ui
--rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/asgen_dialog.ui
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/bus_dialog.ui
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_bus_switch.ui
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_generator_type.ui
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_line_type.ui
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_load_type.ui
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/choose_transformer_type.ui
--rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/dcline_dialog.ui
--rw-r--r--   0        0        0   138693 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/dialogs.py
--rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/ext_grid_dialog.ui
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/extension.ui
--rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/gen_dialog.ui
--rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/impedance_dialog.ui
--rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/line_dialog.ui
--rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/load_dialog.ui
--rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/main_window.ui
--rw-r--r--   0        0        0    12741 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/main_window_backup.ui
--rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/motor_dialog.ui
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/network_settings_dialog.ui
--rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/pf_settings_widget.ui
--rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/power_flow_dialog.ui
--rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/settings_dialog.ui
--rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/sgen_dialog.ui
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/shunt_dialog.ui
--rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/stdline_dialog.ui
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/stdtransformer3w_dialog.ui
--rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/stdtransformer_dialog.ui
--rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/storage_dialog.ui
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/switch_dialog.ui
--rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/transformer3w_dialog.ui
--rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/transformer_dialog.ui
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/ward_dialog.ui
--rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/src/electricalsim/ui/xward_dialog.ui
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/LICENSE
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/README_PyPI.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 electricalsim-0.0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    18645 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/README.md
+-rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/10_PF4.png
+-rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/11_PF_tooltips.png
+-rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/12_App_settings.png
+-rw-r--r--   0        0        0    50389 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/13_Disabling_nodes.png
+-rw-r--r--   0        0        0   114751 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/14_Context_menu.png
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/15_Extension_manager.png
+-rw-r--r--   0        0        0   124772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/1_Main_Window.png
+-rw-r--r--   0        0        0   122916 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/1_Main_Window_dark.png
+-rw-r--r--   0        0        0   149680 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/2_Dialogs.png
+-rw-r--r--   0        0        0    25172 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/3_Widgets.png
+-rw-r--r--   0        0        0   134645 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/4_Pandapower_DataFrames.png
+-rw-r--r--   0        0        0    16870 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/5_Connections_angle_b.png
+-rw-r--r--   0        0        0    21425 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/5_Connections_curved_b.png
+-rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/5_Connections_straight_b.png
+-rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/6_Line_and_transformer_nodes.png
+-rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/7_PF1.png
+-rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/8_PF2.png
+-rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/9_PF3.png
+-rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/img/app_icon.png
+-rw-r--r--   0        0        0    22462 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/Electrical_Grid_Simulator.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/__init__.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/config.ini
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/egs_create_shortcut.py
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/egs_run.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/version.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/.idea/electricalsim.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/.idea/modules.xml
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/.idea/workspace.xml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/extensions/extension_classes.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/hotkeys/hotkey_functions.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/hotkeys/hotkeys.json
+-rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/icons/app_icon.ico
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/icons/app_icon.png
+-rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/icons/app_icon.svg
+-rw-r--r--   0        0        0    30015 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/lib/auxiliary.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/lib/calculations.py
+-rw-r--r--   0        0        0   222733 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/lib/electricalGraph.py
+-rw-r--r--   0        0        0    82025 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/lib/main_components.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/lib/table_widget.py
+-rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/about_dialog.ui
+-rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/aload_dialog.ui
+-rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/asgen_dialog.ui
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/bus_dialog.ui
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/choose_bus_switch.ui
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/choose_generator_type.ui
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/choose_line_type.ui
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/choose_load_type.ui
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/choose_transformer_type.ui
+-rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/dcline_dialog.ui
+-rw-r--r--   0        0        0   138693 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/dialogs.py
+-rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/ext_grid_dialog.ui
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/extension.ui
+-rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/gen_dialog.ui
+-rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/impedance_dialog.ui
+-rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/line_dialog.ui
+-rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/load_dialog.ui
+-rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/main_window.ui
+-rw-r--r--   0        0        0    12741 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/main_window_backup.ui
+-rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/motor_dialog.ui
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/network_settings_dialog.ui
+-rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/pf_settings_widget.ui
+-rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/power_flow_dialog.ui
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/settings_dialog.ui
+-rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/sgen_dialog.ui
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/shunt_dialog.ui
+-rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/stdline_dialog.ui
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/stdtransformer3w_dialog.ui
+-rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/stdtransformer_dialog.ui
+-rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/storage_dialog.ui
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/switch_dialog.ui
+-rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/transformer3w_dialog.ui
+-rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/transformer_dialog.ui
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/ward_dialog.ui
+-rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/src/electricalsim/ui/xward_dialog.ui
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/LICENSE
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/README_PyPI.md
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6751 2020-02-02 00:00:00.000000 electricalsim-0.0.7.2/PKG-INFO
```

### Comparing `electricalsim-0.0.7.1/README.md` & `electricalsim-0.0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/10_PF4.png` & `electricalsim-0.0.7.2/img/10_PF4.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/11_PF_tooltips.png` & `electricalsim-0.0.7.2/img/11_PF_tooltips.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/12_App_settings.png` & `electricalsim-0.0.7.2/img/12_App_settings.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/13_Disabling_nodes.png` & `electricalsim-0.0.7.2/img/13_Disabling_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/14_Context_menu.png` & `electricalsim-0.0.7.2/img/14_Context_menu.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/15_Extension_manager.png` & `electricalsim-0.0.7.2/img/15_Extension_manager.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/1_Main_Window.png` & `electricalsim-0.0.7.2/img/1_Main_Window.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/1_Main_Window_dark.png` & `electricalsim-0.0.7.2/img/1_Main_Window_dark.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/2_Dialogs.png` & `electricalsim-0.0.7.2/img/2_Dialogs.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/3_Widgets.png` & `electricalsim-0.0.7.2/img/3_Widgets.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/4_Pandapower_DataFrames.png` & `electricalsim-0.0.7.2/img/4_Pandapower_DataFrames.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/5_Connections_angle_b.png` & `electricalsim-0.0.7.2/img/5_Connections_angle_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/5_Connections_curved_b.png` & `electricalsim-0.0.7.2/img/5_Connections_curved_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/5_Connections_straight_b.png` & `electricalsim-0.0.7.2/img/5_Connections_straight_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/6_Line_and_transformer_nodes.png` & `electricalsim-0.0.7.2/img/6_Line_and_transformer_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/7_PF1.png` & `electricalsim-0.0.7.2/img/7_PF1.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/8_PF2.png` & `electricalsim-0.0.7.2/img/8_PF2.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/9_PF3.png` & `electricalsim-0.0.7.2/img/9_PF3.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/Logo_CIESE_2021 y UTN_Sta_Fe.png` & `electricalsim-0.0.7.2/img/Logo_CIESE_2021 y UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/img/app_icon.png` & `electricalsim-0.0.7.2/img/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/Electrical_Grid_Simulator.py` & `electricalsim-0.0.7.2/src/electricalsim/Electrical_Grid_Simulator.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/config.ini` & `electricalsim-0.0.7.2/src/electricalsim/config.ini`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/egs_create_shortcut.py` & `electricalsim-0.0.7.2/src/electricalsim/egs_create_shortcut.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/.idea/workspace.xml` & `electricalsim-0.0.7.2/src/electricalsim/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml` & `electricalsim-0.0.7.2/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/extensions/extension_classes.py` & `electricalsim-0.0.7.2/src/electricalsim/extensions/extension_classes.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/hotkeys/hotkey_functions.py` & `electricalsim-0.0.7.2/src/electricalsim/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/hotkeys/hotkeys.json` & `electricalsim-0.0.7.2/src/electricalsim/hotkeys/hotkeys.json`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png` & `electricalsim-0.0.7.2/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.ico` & `electricalsim-0.0.7.2/src/electricalsim/icons/app_icon.ico`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.png` & `electricalsim-0.0.7.2/src/electricalsim/icons/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/icons/app_icon.svg` & `electricalsim-0.0.7.2/src/electricalsim/icons/app_icon.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/lib/auxiliary.py` & `electricalsim-0.0.7.2/src/electricalsim/lib/auxiliary.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/lib/electricalGraph.py` & `electricalsim-0.0.7.2/src/electricalsim/lib/electricalGraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,30 @@
         self.extensions_dict = kwargs.get('extensions_dict', dict())
 
         # When something in the graph changed:
         self.property_changed.connect(self.session_change_warning)
         self.message_unsaved = StatusMessageUnsaved()
         self.main_window.statusbar.addWidget(self.message_unsaved)
         self.message_unsaved.hide()
+        self.set_main_window_title()
+
+    def set_main_window_title(self, file_name=None):
+        """
+        Change the main window title.
+
+        Args:
+            file_name: File name (for saved .egs files)
+
+        Returns: None
+
+        """
+        if file_name is None:
+            self.main_window.setWindowTitle('Electrical Grid Simulation - Unsaved file')
+        else:
+            self.main_window.setWindowTitle(f'Electrical Grid Simulation - {file_name}')
 
     def _on_connection_changed(self, disconnected, connected):
         """
         REPLACED ORIGINAL METHOD IR ORDER TO AVOID UNDO/REDO COMMANDS AFTER CONNECTING OR
         DISCONNECTING PORTS.
 
         called when a pipe connection has been changed in the viewer.
@@ -233,14 +249,16 @@
         serial = self._serialize(nodes)
         new_nodes = self._deserialize2(serial)
         offset = 50
         for n in new_nodes:
             x, y = n.pos()
             n.set_pos(x + offset, y + offset)
             n.set_property('selected', True)
+            if n.get_property('layout_vert') is True:
+                n.set_layout_direction(1)
 
         # self._undo_stack.endMacro()
         return new_nodes
 
     def _deserialize2(self, data, relative_pos=False, pos=None):
         """
         ALTERNATIVE TO _deserialize2 METHOD WITHOUT push_undo
@@ -254,17 +272,17 @@
             pos (tuple or list): custom x, y position.
 
         Returns:
             list[NodeGraphQt.Nodes]: list of node instances.
         """
         # update node graph properties.
         for attr_name, attr_value in data.get('graph', {}).items():
-            if attr_name == 'layout_direction':
-                self.set_layout_direction(attr_value)
-            elif attr_name == 'acyclic':
+            # if attr_name == 'layout_direction':
+            #     self.set_layout_direction(attr_value)
+            if attr_name == 'acyclic':
                 self.set_acyclic(attr_value)
             elif attr_name == 'pipe_collision':
                 self.set_pipe_collision(attr_value)
             elif attr_name == 'pipe_slicing':
                 self.set_pipe_slicing(attr_value)
             elif attr_name == 'pipe_style':
                 self.set_pipe_style(attr_value)
@@ -453,14 +471,16 @@
             with open(full_file_path, 'wb') as file:
                 data = {'graph_dict': self.serialize_session(),
                         'pandapower_net': pp.to_json(self.net, None)}
                 pickle.dump(data, file)
 
             self.saved_file_path = full_file_path
             self.message_unsaved.hide()
+            _, file_name = os.path.split(full_file_path)
+            self.set_main_window_title(file_name[:-4])
         else:
             simulate_ESC_key()
 
     def open_session(self):
         """
         Open session from a file and overwrite the current one (graph and pandapower network).
         """
@@ -518,14 +538,19 @@
             if self.main_window.toolBox.currentIndex()==1:
                 self.page_changed_on_toolbox(index=1)
                 
             
 
         simulate_ESC_key()
 
+        self.update_widgets_properties()
+
+        _, file_name = os.path.split(full_file_path)
+        self.set_main_window_title(file_name[:-4])
+
     def new_session(self):
         """
         Clear the session (graph and pandapower network) and creates a new one.
         """
         title = 'Warning: Current session will be lost'
         text_content = """A new session will clear the current one, and data will be\
                         lost if it was not saved. Do you want to continue anyway?"""
@@ -544,14 +569,16 @@
                                            sn_mva=float(settings['sn_mva']))
         self.saved_file_path = None
         self.message_unsaved.hide()
         
         if self.main_window.toolBox.currentIndex()==1:
             self.page_changed_on_toolbox(index=1)
 
+        self.set_main_window_title()
+
     def edit_settings(self):
         """
         Show the dialog to edit settings.
         """
         # show_WIP(self.main_window)
         dataframe_line_stds = pp.available_std_types(self.net, 'line')
         dataframe_trafo_stds = pp.available_std_types(self.net, 'trafo')
@@ -723,15 +750,15 @@
                 stds = pp.available_std_types(self.net, element='trafo3w')
 
             for name, value in settings.items():
                 if name in ('tap_side', 'vector_group', 'std_type'):
                     node.set_property(name, value, push_undo=False)
                 elif name in ('tap_neutral', 'tap_max', 'tap_min', 'tap_pos', 'parallel'):
                     node.set_property(name, int(value), push_undo=False)
-                elif name in ('tap_phase_shifter', 'oltc', 'tap_at_star_point') and value=='True':
+                elif name in ('tap_phase_shifter', 'oltc', '') and value=='True':
                     node.set_property(name, True, push_undo=False)
                 elif name in ('tap_phase_shifter', 'oltc', 'tap_at_star_point') and value=='False':
                     node.set_property(name, False, push_undo=False)
                 else:
                     node.set_property(name, float(value), push_undo=False)
 
                 if name=='tap_min':
@@ -2616,14 +2643,15 @@
             node.set_property('si0_hv_partial', dialog.si0_hv_partial.value(), push_undo=False)
             node.set_property('xn_ohm', dialog.xn_ohm.value(), push_undo=False)
             oltc = True if dialog.oltc.isChecked() else False
             node.set_property('oltc', oltc, push_undo=False)
 
             node.tap_pos_widget.get_custom_widget().setMinimum(int(dialog.tap_min.value()))
             node.tap_pos_widget.get_custom_widget().setMaximum(int(dialog.tap_max.value()))
+            node.tap_pos_widget.get_custom_widget().setValue(int(dialog.tap_pos.value()))
 
             transformer_index = node.get_property('transformer_index')
             if transformer_index is not None and node.connected_to_network():
                 for name in node.electrical_properties:
                     if name in ('tap_pos', 'tap_max', 'tap_min', 'tap_neutral', 'parallel'):  # int
                         self.net.trafo.loc[transformer_index, name] = int(node.get_property(name))
                     elif name in ('tap_side', 'vector_group'):  # str
@@ -2732,15 +2760,15 @@
         dialog.tap_step_percent.setValue(node.get_property('tap_step_percent'))
         dialog.tap_step_degree.setValue(node.get_property('tap_step_degree'))
         dialog.tap_pos.setValue(node.get_property('tap_pos'))
         dialog.tap_pos_display.setText(str(node.get_property('tap_pos')))
         dialog.tap_pos.setMinimum(node.get_property('tap_min'))
         dialog.tap_pos.setMaximum(node.get_property('tap_max'))
 
-        dialog.tap_at_star_point.setChecked(node.get_property('tap_at_star_point'))
+        dialog.tap_at_star_point.setChecked(True if node.get_property('tap_at_star_point')=='True' else False)
 
         vector_group = node.get_property('vector_group')
         all_vector_groups = ('Ddd', 'Ddy', 'Dyd', 'Dyy', 'Ydd', 'Ydy', 'Yyd',
                              'Yyy', 'YNyd', 'YNdy', 'Yynd', 'Ydyn', 'YNynd',
                              'YNdyn', 'YNdd', 'YNyy')
         dialog.vector_group.setCurrentIndex(all_vector_groups.index(vector_group))
         dialog.max_loading_percent.setValue(node.get_property('max_loading_percent'))
@@ -2820,15 +2848,15 @@
         dialog.setWindowIcon(QtGui.QIcon(icon_path))
         dialog.max_loading_percent.setValue(node.get_property('max_loading_percent'))
         dialog.tap_pos.setValue(node.get_property('tap_pos'))
         dialog.tap_pos_display.setText(str(node.get_property('tap_pos')))
         dialog.tap_pos.setMinimum(table.at[selected_std, 'tap_min'])
         dialog.tap_pos.setMaximum(table.at[selected_std, 'tap_max'])
         
-        dialog.tap_at_star_point.setChecked(node.get_property('tap_at_star_point'))
+        dialog.tap_at_star_point.setChecked(True if node.get_property('tap_at_star_point')=='True' else False)
 
         if dialog.exec():
             node.set_property('max_loading_percent', dialog.max_loading_percent.value(), push_undo=False)
             node.set_property('std_type', dialog.std_type.currentText(), push_undo=False)
             node.set_property('tap_pos', dialog.tap_pos.value(), push_undo=False)
 
             tap_at_star_point = 'True' if dialog.tap_at_star_point.isChecked() else 'False'
@@ -3979,7 +4007,146 @@
         selector.clear()
         if self.extensions_dict:
             selector.addItems(sorted(self.extensions_dict.keys()))
             btn.setEnabled(True)
         else:
             selector.addItem('<No extensions available>')
             btn.setEnabled(False)
+
+    def update_widgets_properties(self):
+        """
+        Update the state of widgets inside the nodes when opening a session.
+
+        Returns: None
+
+        """
+        dcline_nodes = self.get_nodes_by_type('DCLineNode.DCLineNode')
+        for node in dcline_nodes:
+            node.p_mw_widget.get_custom_widget().setMaximum(node.get_property('max_p_mw'))
+            line_index = node.get_property('line_index')
+            if line_index is not None:
+                try:
+                    node.p_mw_widget.get_custom_widget().setValue(self.net.dcline.loc[line_index, 'p_mw'])
+                except KeyError:
+                    node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
+
+        trafo_nodes = self.get_nodes_by_type('TrafoNode.TrafoNode')
+        for node in trafo_nodes:
+            node.tap_pos_widget.get_custom_widget().setMinimum(node.get_property('tap_min'))
+            node.tap_pos_widget.get_custom_widget().setMaximum(node.get_property('tap_max'))
+            # node.tap_pos_widget.get_custom_widget().setValue(node.get_property('tap_pos'))
+            transformer_index = node.get_property('transformer_index')
+            if transformer_index is not None:
+                try:
+                    node.tap_pos_widget.get_custom_widget().setValue(self.net.trafo.loc[transformer_index, 'tap_pos'])
+                except KeyError:
+                    node.tap_pos_widget.get_custom_widget().setValue(node.get_property('tap_pos'))
+
+        std_trafo_nodes = self.get_nodes_by_type('StdTrafoNode.StdTrafoNode')
+        for node in std_trafo_nodes:
+            node.tap_pos_widget.get_custom_widget().setMinimum(node.get_property('tap_min'))
+            node.tap_pos_widget.get_custom_widget().setMaximum(node.get_property('tap_max'))
+            # node.tap_pos_widget.get_custom_widget().setValue(node.get_property('tap_pos'))
+            transformer_index = node.get_property('transformer_index')
+            if transformer_index is not None:
+                try:
+                    node.tap_pos_widget.get_custom_widget().setValue(self.net.trafo.loc[transformer_index, 'tap_pos'])
+                except KeyError:
+                    node.tap_pos_widget.get_custom_widget().setValue(node.get_property('tap_pos'))
+
+        trafo3w_nodes = self.get_nodes_by_type('Trafo3wNode.Trafo3wNode')
+        for node in trafo3w_nodes:
+            node.tap_pos_widget.get_custom_widget().setMinimum(node.get_property('tap_min'))
+            node.tap_pos_widget.get_custom_widget().setMaximum(node.get_property('tap_max'))
+            # node.tap_pos_widget.get_custom_widget().setValue(node.get_property('tap_pos'))
+            transformer_index = node.get_property('transformer_index')
+            if transformer_index is not None:
+                try:
+                    node.tap_pos_widget.get_custom_widget().setValue(self.net.trafo3w.loc[transformer_index, 'tap_pos'])
+                except KeyError:
+                    node.tap_pos_widget.get_custom_widget().setValue(node.get_property('tap_pos'))
+
+        std_trafo3w_nodes = self.get_nodes_by_type('StdTrafo3wNode.StdTrafo3wNode')
+        for node in std_trafo3w_nodes:
+            node.tap_pos_widget.get_custom_widget().setMinimum(node.get_property('tap_min'))
+            node.tap_pos_widget.get_custom_widget().setMaximum(node.get_property('tap_max'))
+            # node.tap_pos_widget.get_custom_widget().setValue(node.get_property('tap_pos'))
+            transformer_index = node.get_property('transformer_index')
+            if transformer_index is not None:
+                try:
+                    node.tap_pos_widget.get_custom_widget().setValue(self.net.trafo3w.loc[transformer_index, 'tap_pos'])
+                except KeyError:
+                    node.tap_pos_widget.get_custom_widget().setValue(node.get_property('tap_pos'))
+
+        gen_nodes = self.get_nodes_by_type('GenNode.GenNode')
+        for node in gen_nodes:
+            node.p_mw_widget.get_custom_widget().setMinimum(node.get_property('min_p_mw'))
+            node.p_mw_widget.get_custom_widget().setMaximum(node.get_property('max_p_mw'))
+            node.vm_pu_widget.get_custom_widget().setMinimum(node.get_property('min_vm_pu'))
+            node.vm_pu_widget.get_custom_widget().setMaximum(node.get_property('max_vm_pu'))
+
+            gen_index = node.get_property('gen_index')
+            if gen_index is not None:
+                try:
+                    node.p_mw_widget.get_custom_widget().setValue(self.net.gen.loc[gen_index, 'p_mw'])
+                    node.vm_pu_widget.get_custom_widget().setValue(self.net.gen.loc[gen_index, 'vm_pu'])
+                except KeyError:
+                    node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
+                    node.vm_pu_widget.get_custom_widget().setValue(node.get_property('vm_pu'))
+
+        sgen_nodes = self.get_nodes_by_type('SGenNode.SGenNode')
+        for node in sgen_nodes:
+            node.p_mw_widget.get_custom_widget().setMinimum(node.get_property('min_p_mw'))
+            node.p_mw_widget.get_custom_widget().setMaximum(node.get_property('max_p_mw'))
+            # node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
+            node.q_mvar_widget.get_custom_widget().setMinimum(node.get_property('min_q_mvar'))
+            node.q_mvar_widget.get_custom_widget().setMaximum(node.get_property('max_q_mvar'))
+            # node.q_mvar_widget.get_custom_widget().setValue(node.get_property('q_mvar'))
+
+            gen_index = node.get_property('gen_index')
+            if gen_index is not None:
+                try:
+                    node.p_mw_widget.get_custom_widget().setValue(self.net.sgen.loc[gen_index, 'p_mw'])
+                    node.q_mvar_widget.get_custom_widget().setValue(self.net.sgen.loc[gen_index, 'q_mvar'])
+                except KeyError:
+                    node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
+                    node.q_mvar_widget.get_custom_widget().setValue(node.get_property('q_mvar'))
+
+        # ext_grid_nodes = self.get_nodes_by_type('ExtGridNode.ExtGridNode')
+        # for node in ext_grid_nodes:
+        #     node.vm_pu_widget.get_custom_widget().setValue(node.get_property('vm_pu'))
+
+        load_nodes = self.get_nodes_by_type('LoadNode.LoadNode')
+        for node in load_nodes:
+            node.p_mw_widget.get_custom_widget().setMinimum(node.get_property('min_p_mw'))
+            node.p_mw_widget.get_custom_widget().setMaximum(node.get_property('max_p_mw'))
+            # node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
+            node.q_mvar_widget.get_custom_widget().setMinimum(node.get_property('min_q_mvar'))
+            node.q_mvar_widget.get_custom_widget().setMaximum(node.get_property('max_q_mvar'))
+            # node.q_mvar_widget.get_custom_widget().setValue(node.get_property('q_mvar'))
+
+            load_index = node.get_property('load_index')
+            if load_index is not None:
+                try:
+                    node.p_mw_widget.get_custom_widget().setValue(self.net.load.loc[load_index, 'p_mw'])
+                    node.q_mvar_widget.get_custom_widget().setValue(self.net.load.loc[load_index, 'q_mvar'])
+                except KeyError:
+                    node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
+                    node.q_mvar_widget.get_custom_widget().setValue(node.get_property('q_mvar'))
+
+        shunt_nodes = self.get_nodes_by_type('ShuntNode.ShuntNode')
+        for node in shunt_nodes:
+            # node.p_mw_widget.get_custom_widget().setMinimum(node.get_property('min_p_mw'))
+            # node.p_mw_widget.get_custom_widget().setMaximum(node.get_property('max_p_mw'))
+            # node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
+            # node.q_mvar_widget.get_custom_widget().setMinimum(node.get_property('min_q_mvar'))
+            # node.q_mvar_widget.get_custom_widget().setMaximum(node.get_property('max_q_mvar'))
+            # node.q_mvar_widget.get_custom_widget().setValue(node.get_property('q_mvar'))
+
+            shunt_index = node.get_property('shunt_index')
+            if shunt_index is not None:
+                try:
+                    node.p_mw_widget.get_custom_widget().setValue(self.net.shunt.loc[shunt_index, 'p_mw'])
+                    node.q_mvar_widget.get_custom_widget().setValue(self.net.shunt.loc[shunt_index, 'q_mvar'])
+                except KeyError:
+                    node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
+                    node.q_mvar_widget.get_custom_widget().setValue(node.get_property('q_mvar'))
```

### Comparing `electricalsim-0.0.7.1/src/electricalsim/lib/main_components.py` & `electricalsim-0.0.7.2/src/electricalsim/lib/main_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,14 +604,21 @@
         
     def update_tap_pos(self, value):
         """
         Updates 'tap_pos' property when changing the tap position widget from the node.
         
         Updates the 'tap_pos' parameter on the pandapower network too.
         """
+        # tap_max = self.get_property('tap_max')
+        # if tap_max is not None:
+        #     self.tap_pos_widget.get_custom_widget().setMaximum(tap_max)
+        # tap_min = self.get_property('tap_min')
+        # if tap_min is not None:
+        #     self.tap_pos_widget.get_custom_widget().setMinimum(tap_min)
+
         self.set_property('tap_pos', value, push_undo=False)
         
         transformer_index = self.get_property('transformer_index')
         if transformer_index is not None and self.connected_to_network():
             self.graph.net.trafo.loc[transformer_index, 'tap_pos'] = int(value)
             
     def connected_to_network(self):
@@ -885,14 +892,17 @@
         # add custom widget to node with "node.view" as the parent.
         self.p_mw_widget = QSpinBoxWrapper(self.view, widget_type=QtWidgets.QDoubleSpinBox())
         self.p_mw_widget.set_name('p_mw')
         self.p_mw_widget.set_label('Pg (MW)')
         
         self.p_mw_widget.get_custom_widget().valueChanged.connect(self.update_p_mw)
         self.p_mw_widget.get_custom_widget().setDecimals(5)
+        # max_p = self.get_property('max_p_mw')
+        # if max_p is not None:
+        #     self.p_mw_widget.get_custom_widget().setMaximum(max_p)
         self.add_custom_widget(self.p_mw_widget, tab=None)  # Adds the 'p_mw' property.
         
         # add custom widget to node with "node.view" as the parent.
         self.scaling_widget = QSpinBoxWrapper(self.view, widget_type=QtWidgets.QDoubleSpinBox())
         self.scaling_widget.set_name('scaling')
         self.scaling_widget.set_label('Scaling Pg')
         self.scaling_widget.get_custom_widget().valueChanged.connect(self.update_scaling)
```

### Comparing `electricalsim-0.0.7.1/src/electricalsim/lib/table_widget.py` & `electricalsim-0.0.7.2/src/electricalsim/lib/table_widget.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/about_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/aload_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/aload_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/asgen_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/asgen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/bus_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/bus_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/choose_bus_switch.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/choose_bus_switch.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/choose_generator_type.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/choose_generator_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/choose_line_type.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/choose_line_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/choose_load_type.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/choose_load_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/choose_transformer_type.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/choose_transformer_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/dcline_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/dcline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/dialogs.py` & `electricalsim-0.0.7.2/src/electricalsim/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/ext_grid_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/ext_grid_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/extension.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/extension.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/gen_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/gen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/impedance_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/impedance_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/line_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/line_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/load_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/load_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/main_window.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/main_window_backup.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/main_window_backup.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/motor_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/motor_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/network_settings_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/network_settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/pf_settings_widget.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/pf_settings_widget.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/power_flow_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/power_flow_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/settings_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/sgen_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/sgen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/shunt_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/shunt_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/stdline_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/stdline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/stdtransformer3w_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/stdtransformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/stdtransformer_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/stdtransformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/storage_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/storage_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/switch_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/switch_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/transformer3w_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/transformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/transformer_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/transformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/ward_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/ward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/src/electricalsim/ui/xward_dialog.ui` & `electricalsim-0.0.7.2/src/electricalsim/ui/xward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/LICENSE` & `electricalsim-0.0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/README_PyPI.md` & `electricalsim-0.0.7.2/README_PyPI.md`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.7.1/pyproject.toml` & `electricalsim-0.0.7.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "electricalsim"
-version = "0.0.7.1"
+version = "0.0.7.2"
 author = "Dr. Ing. Ariel S. Loyarte"
 authors = [
   { name="Dr. Ing. Ariel S. Loyarte", email="aloyarte@frsf.utn.edu.ar" },
 ]
 description = "Graphical user interface for simulating electrical networks based on the pandapower library"
 readme = "README_PyPI.md"
 requires-python = ">=3.8"
@@ -22,15 +22,15 @@
   "pynput>=1.7.6",
   "lightsim2grid>=0.7.1",
   "matplotlib>=3.6.0",
   "platformdirs>=3.0.0",
   "qtpy>=2.3.0",
   "pyshortcuts>=1.8.3",
   "importlib_metadata>=4.11.3",
-  "NodeGraphQt>=0.6.1",
+  "NodeGraphQt>=0.6.16",
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 keywords = ["electrical networks", "simulation", "energy", "power systems"]
```

### Comparing `electricalsim-0.0.7.1/PKG-INFO` & `electricalsim-0.0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electricalsim
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: Graphical user interface for simulating electrical networks based on the pandapower library
 Project-URL: Homepage, https://github.com/aloytag/electrical-grid-simulator
 Project-URL: Bug Tracker, https://github.com/aloytag/electrical-grid-simulator/issues
 Project-URL: Repository, https://github.com/aloytag/electrical-grid-simulator
 Author-email: "Dr. Ing. Ariel S. Loyarte" <aloyarte@frsf.utn.edu.ar>
 License: MIT
 License-File: LICENSE
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: importlib-metadata>=4.11.3
 Requires-Dist: lightsim2grid>=0.7.1
 Requires-Dist: matplotlib>=3.6.0
-Requires-Dist: nodegraphqt>=0.6.1
+Requires-Dist: nodegraphqt>=0.6.16
 Requires-Dist: numba>=0.56.4
 Requires-Dist: pandapower>=2.13.1
 Requires-Dist: platformdirs>=3.0.0
 Requires-Dist: pynput>=1.7.6
 Requires-Dist: pyqtdarktheme>=2.1.0
 Requires-Dist: pyshortcuts>=1.8.3
 Requires-Dist: pyside2>=5.15
```

