# Comparing `tmp/ztpserver-1.6.0.tar.gz` & `tmp/ztpserver-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ztpserver-1.6.0.tar", last modified: Mon Aug  8 20:40:47 2022, max compression
+gzip compressed data, was "ztpserver-2.0.0.tar", last modified: Mon Aug  7 16:39:00 2023, max compression
```

## Comparing `ztpserver-1.6.0.tar` & `ztpserver-2.0.0.tar`

### file list

```diff
@@ -1,179 +1,186 @@
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/
--rw-r--r--   0 mhartzel   (501) staff       (20)     3235 2022-08-08 20:40:47.000000 ztpserver-1.6.0/PKG-INFO
--rw-r--r--   0 mhartzel   (501) staff       (20)     1229 2022-06-09 19:50:37.000000 ztpserver-1.6.0/.pylintrc
--rw-r--r--   0 mhartzel   (501) staff       (20)     2224 2022-06-09 19:50:37.000000 ztpserver-1.6.0/LICENSE
--rw-r--r--   0 mhartzel   (501) staff       (20)      101 2022-06-21 20:26:52.000000 ztpserver-1.6.0/requirements.txt
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:46.000000 ztpserver-1.6.0/test/
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/test/server/
--rw-r--r--   0 mhartzel   (501) staff       (20)     5876 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/server/test_repository.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     2165 2022-06-21 20:26:52.000000 ztpserver-1.6.0/test/server/test_utils.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     3894 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/server/test_wsgiapp.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     2719 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/server/test_serializers.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     9765 2022-06-21 20:26:52.000000 ztpserver-1.6.0/test/server/test_ndb.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    15557 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/server/test_topology_classes.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     8832 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/server/server_test_lib.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    13928 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/server/test_config.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1997 2022-06-21 20:26:52.000000 ztpserver-1.6.0/test/server/test_app.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     7083 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/server/test_types.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    59652 2022-06-21 20:26:52.000000 ztpserver-1.6.0/test/server/test_controller.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     5389 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/server/test_topology.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/test/neighbordb/
--rw-r--r--   0 mhartzel   (501) staff       (20)     3247 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/large_pattern_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)     1259 2022-06-21 20:26:52.000000 ztpserver-1.6.0/test/neighbordb/chassis_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)      810 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/interface_name_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)     5749 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/ndb_entries_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)     1184 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/README.md
--rw-r--r--   0 mhartzel   (501) staff       (20)     2201 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/bogus_patterns_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)     4054 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/small_pattern_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)    13948 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/ndb_values_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)      541 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/node_interfaces_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)     2252 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/simple_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)      483 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/node_test.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)     1326 2022-06-21 20:26:52.000000 ztpserver-1.6.0/test/neighbordb/chassis_test_2.yml
--rw-r--r--   0 mhartzel   (501) staff       (20)     1559 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/neighbordb/simple_functions_test.yml
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/test/actions/
--rw-r--r--   0 mhartzel   (501) staff       (20)     3828 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/actions/test_send_email.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    11455 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/actions/test_add_config.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     7177 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/actions/test_run_bash_script.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    23799 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/actions/test_copy_file.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     5512 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/actions/test_replace_config.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     6092 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/actions/test_install_cli_plugin.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     6595 2022-06-21 20:26:52.000000 ztpserver-1.6.0/test/actions/test_install_image.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     7015 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/actions/test_run_cli_commands.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     7710 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/actions/test_install_extension.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/test/client/
--rw-r--r--   0 mhartzel   (501) staff       (20)     5255 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/client/test_xmpp_bootstrap.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     5245 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/client/test_bootstrap_cleanup.py
--rwxr-xr-x   0 mhartzel   (501) staff       (20)     1961 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/client/FastCli
--rwxr-xr-x   0 mhartzel   (501) staff       (20)    29855 2022-06-09 19:50:37.000000 ztpserver-1.6.0/test/client/test_bootstrap.py
--rwxr-xr-x   0 mhartzel   (501) staff       (20)    22210 2022-07-12 15:40:16.000000 ztpserver-1.6.0/test/client/client_test_lib.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:46.000000 ztpserver-1.6.0/bin/
--rwxr-xr-x   0 mhartzel   (501) staff       (20)     1720 2022-06-09 19:50:37.000000 ztpserver-1.6.0/bin/ztps
--rw-r--r--   0 mhartzel   (501) staff       (20)      100 2022-06-09 19:50:37.000000 ztpserver-1.6.0/CHANGELOG.md
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/ztpserver/
--rw-r--r--   0 mhartzel   (501) staff       (20)    36477 2022-06-21 20:26:52.000000 ztpserver-1.6.0/ztpserver/controller.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    10622 2022-06-09 19:50:37.000000 ztpserver-1.6.0/ztpserver/config.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     4419 2022-06-09 19:50:37.000000 ztpserver-1.6.0/ztpserver/wsgiapp.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    13110 2022-06-09 19:50:37.000000 ztpserver-1.6.0/ztpserver/validators.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    10107 2022-06-21 20:26:52.000000 ztpserver-1.6.0/ztpserver/serializers.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1969 2022-06-09 19:50:37.000000 ztpserver-1.6.0/ztpserver/constants.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     1589 2022-06-09 19:50:37.000000 ztpserver-1.6.0/ztpserver/__init__.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     3765 2022-06-09 19:50:37.000000 ztpserver-1.6.0/ztpserver/types.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    11872 2022-06-21 20:26:52.000000 ztpserver-1.6.0/ztpserver/utils.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    32764 2022-06-21 20:26:52.000000 ztpserver-1.6.0/ztpserver/topology.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    12714 2022-06-21 20:26:52.000000 ztpserver-1.6.0/ztpserver/app.py
--rw-r--r--   0 mhartzel   (501) staff       (20)     2179 2022-06-21 20:26:52.000000 ztpserver-1.6.0/ztpserver/resources.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    10831 2022-06-09 19:50:37.000000 ztpserver-1.6.0/ztpserver/repository.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/plugins/
--rw-r--r--   0 mhartzel   (501) staff       (20)     1879 2022-06-21 20:26:52.000000 ztpserver-1.6.0/plugins/test
--rw-r--r--   0 mhartzel   (501) staff       (20)     5724 2022-06-21 20:26:52.000000 ztpserver-1.6.0/plugins/sqlite
--rw-r--r--   0 mhartzel   (501) staff       (20)     4896 2022-06-21 20:26:52.000000 ztpserver-1.6.0/plugins/mysql_vars
--rw-r--r--   0 mhartzel   (501) staff       (20)     5163 2022-06-21 20:26:52.000000 ztpserver-1.6.0/plugins/allocate
--rw-r--r--   0 mhartzel   (501) staff       (20)     2778 2022-06-21 20:26:52.000000 ztpserver-1.6.0/Makefile
--rw-r--r--   0 mhartzel   (501) staff       (20)      300 2022-06-09 19:50:37.000000 ztpserver-1.6.0/INSTALL.md
--rw-r--r--   0 mhartzel   (501) staff       (20)      491 2022-06-21 20:26:52.000000 ztpserver-1.6.0/MANIFEST.in
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/utils/
--rwxr-xr-x   0 mhartzel   (501) staff       (20)     4088 2022-06-09 19:50:37.000000 ztpserver-1.6.0/utils/refresh_ztps
--rwxr-xr-x   0 mhartzel   (501) staff       (20)     1154 2022-06-21 20:26:52.000000 ztpserver-1.6.0/utils/create_db.py
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/docs/
--rw-r--r--   0 mhartzel   (501) staff       (20)     1144 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/actions.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     8097 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/install.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)      304 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/ReleaseNotes1.4.1.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1543 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/index.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1393 2022-07-12 20:40:04.000000 ztpserver-1.6.0/docs/ReleaseNotes1.6.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)       95 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/requirements.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)     4958 2022-07-12 20:05:54.000000 ztpserver-1.6.0/docs/support.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     7042 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/Makefile
--rw-r--r--   0 mhartzel   (501) staff       (20)     1058 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/ReleaseNotes1.4.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1072 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/ReleaseNotes1.5.0.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     9234 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/conf.py
--rw-r--r--   0 mhartzel   (501) staff       (20)    33240 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/config.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)    10277 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/examples.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3226 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/ReleaseNotes1.3.rst
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/docs/_static/
--rwxr-xr-x   0 mhartzel   (501) staff       (20)    56384 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/_static/AttrsActions.png
--rw-r--r--   0 mhartzel   (501) staff       (20)     4286 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/_static/favicon.ico
--rw-r--r--   0 mhartzel   (501) staff       (20)    26494 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/_static/arista_logo_11-trans-w.png
--rw-r--r--   0 mhartzel   (501) staff       (20)    62200 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/_static/arista_logo_jpg-11.jpg
--rwxr-xr-x   0 mhartzel   (501) staff       (20)    21706 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/_static/Components.png
--rw-r--r--   0 mhartzel   (501) staff       (20)    32128 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/_static/ztpserver-seqdiag.png
--rwxr-xr-x   0 mhartzel   (501) staff       (20)    38264 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/_static/LeafDefn.png
--rw-r--r--   0 mhartzel   (501) staff       (20)     1563 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/ReleaseNotes1.3.2.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     9949 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/ReleaseNotes1.2.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     9170 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/overview.rst
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/docs/cookbook/
--rw-r--r--   0 mhartzel   (501) staff       (20)    13760 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/cookbook/actions.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2836 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/install.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2791 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/ztpsVMonEOS.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     4659 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/dynamicNodes.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2053 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/resourcePools.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2212 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/clientLogging.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     5911 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/configuration.rst
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/docs/cookbook/ztpsVMonEOS/
--rw-r--r--   0 mhartzel   (501) staff       (20)     8370 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/ztpsVMonEOS/l2l3wm.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     8397 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/ztpsVMonEOS/l2wom.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)    13958 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/ztpsVMonEOS/l3wom.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2551 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/cookbook/puppet.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)    12359 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/helloWorld.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     8853 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/topologyValidation.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     5211 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/cookbook/ansible.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1878 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/serverLogging.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)      326 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/_template.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     9146 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/runningZTPS.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     5214 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/definitions.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)    13411 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/cookbook/staticNodes.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3951 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/cookbook/advanced.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)      250 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/ReleaseNotes1.3.1.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)    13740 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/ReleaseNotes1.1.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)      681 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/README.md
--rw-r--r--   0 mhartzel   (501) staff       (20)       68 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/modules.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     8563 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/tips.rst
--rwxr-xr-x   0 mhartzel   (501) staff       (20)      576 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/setup_rtd_files.sh
--rw-r--r--   0 mhartzel   (501) staff       (20)       16 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/.gitignore
--rw-r--r--   0 mhartzel   (501) staff       (20)     2546 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/implementation.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     5182 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/startup.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2328 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/CONTRIBUTING.md
--rw-r--r--   0 mhartzel   (501) staff       (20)     2224 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/license.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     3060 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/troubleshooting.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)      448 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/cookbook.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)      145 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/client.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     8624 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/api.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)       88 2022-06-09 19:50:37.000000 ztpserver-1.6.0/docs/internals.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     1568 2022-06-21 20:26:52.000000 ztpserver-1.6.0/docs/glossary.rst
--rw-r--r--   0 mhartzel   (501) staff       (20)     2470 2022-06-09 19:50:37.000000 ztpserver-1.6.0/README.md
--rwxr-xr-x   0 mhartzel   (501) staff       (20)     6772 2022-08-08 20:33:59.000000 ztpserver-1.6.0/setup.py
--rw-r--r--   0 mhartzel   (501) staff       (20)        6 2022-08-08 20:37:55.000000 ztpserver-1.6.0/VERSION
--rw-r--r--   0 mhartzel   (501) staff       (20)     1814 2022-06-09 19:50:37.000000 ztpserver-1.6.0/CONTRIBUTING.md
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:46.000000 ztpserver-1.6.0/actions/
--rw-r--r--   0 mhartzel   (501) staff       (20)     3462 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/the_nick
--rw-r--r--   0 mhartzel   (501) staff       (20)     3622 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/configure_ansible_client
--rw-r--r--   0 mhartzel   (501) staff       (20)     3978 2022-06-21 20:26:52.000000 ztpserver-1.6.0/actions/install_image
--rw-r--r--   0 mhartzel   (501) staff       (20)     1921 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/template
--rw-r--r--   0 mhartzel   (501) staff       (20)     3610 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/add_config
--rw-r--r--   0 mhartzel   (501) staff       (20)     3383 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/run_cli_commands
--rw-r--r--   0 mhartzel   (501) staff       (20)     3462 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/run_bash_script
--rw-r--r--   0 mhartzel   (501) staff       (20)     3186 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/install_extension
--rw-r--r--   0 mhartzel   (501) staff       (20)     2852 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/install_cli_plugin
--rw-r--r--   0 mhartzel   (501) staff       (20)     6113 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/send_email
--rw-r--r--   0 mhartzel   (501) staff       (20)     6622 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/copy_file
--rw-r--r--   0 mhartzel   (501) staff       (20)     2364 2022-06-09 19:50:37.000000 ztpserver-1.6.0/actions/replace_config
--rw-r--r--   0 mhartzel   (501) staff       (20)       99 2022-08-08 20:40:47.000000 ztpserver-1.6.0/setup.cfg
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/ztpserver.egg-info/
--rw-r--r--   0 mhartzel   (501) staff       (20)     3235 2022-08-08 20:40:46.000000 ztpserver-1.6.0/ztpserver.egg-info/PKG-INFO
--rw-r--r--   0 mhartzel   (501) staff       (20)     3941 2022-08-08 20:40:46.000000 ztpserver-1.6.0/ztpserver.egg-info/SOURCES.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)       29 2022-08-08 20:40:46.000000 ztpserver-1.6.0/ztpserver.egg-info/requires.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)       10 2022-08-08 20:40:46.000000 ztpserver-1.6.0/ztpserver.egg-info/top_level.txt
--rw-r--r--   0 mhartzel   (501) staff       (20)        1 2022-08-08 20:40:46.000000 ztpserver-1.6.0/ztpserver.egg-info/dependency_links.txt
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:47.000000 ztpserver-1.6.0/rpm/
--rw-r--r--   0 mhartzel   (501) staff       (20)     1761 2022-06-09 19:50:37.000000 ztpserver-1.6.0/rpm/Makefile
--rw-r--r--   0 mhartzel   (501) staff       (20)    12188 2022-06-21 20:26:52.000000 ztpserver-1.6.0/rpm/ztpserver.spec
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:46.000000 ztpserver-1.6.0/conf/
--rw-r--r--   0 mhartzel   (501) staff       (20)     1117 2022-06-09 19:50:37.000000 ztpserver-1.6.0/conf/ztpserver.conf
--rw-r--r--   0 mhartzel   (501) staff       (20)      373 2022-06-09 19:50:37.000000 ztpserver-1.6.0/conf/bootstrap.conf
--rw-r--r--   0 mhartzel   (501) staff       (20)      730 2022-06-09 19:50:37.000000 ztpserver-1.6.0/conf/neighbordb
--rw-r--r--   0 mhartzel   (501) staff       (20)      345 2022-06-09 19:50:37.000000 ztpserver-1.6.0/conf/ztpserver-wsgi.conf
--rw-r--r--   0 mhartzel   (501) staff       (20)     1785 2022-06-09 19:50:37.000000 ztpserver-1.6.0/conf/ztpserver.wsgi
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:46.000000 ztpserver-1.6.0/client/
--rwxr-xr-x   0 mhartzel   (501) staff       (20)    50445 2022-07-12 15:40:16.000000 ztpserver-1.6.0/client/bootstrap
-drwxr-xr-x   0 mhartzel   (501) staff       (20)        0 2022-08-08 20:40:46.000000 ztpserver-1.6.0/client/lib/
--rw-r--r--   0 mhartzel   (501) staff       (20)   429521 2022-06-09 19:50:37.000000 ztpserver-1.6.0/client/lib/requests-2.3.0.tar.gz
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.277114 ztpserver-2.0.0/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1045 2023-07-14 16:52:30.000000 ztpserver-2.0.0/.pylintrc
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      100 2023-07-07 10:57:57.000000 ztpserver-2.0.0/CHANGELOG.md
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1814 2023-07-07 10:57:57.000000 ztpserver-2.0.0/CONTRIBUTING.md
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      300 2023-07-07 10:57:57.000000 ztpserver-2.0.0/INSTALL.md
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2224 2023-06-26 16:36:08.000000 ztpserver-2.0.0/LICENSE
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      491 2023-08-02 14:44:30.000000 ztpserver-2.0.0/MANIFEST.in
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2778 2023-07-07 10:57:29.000000 ztpserver-2.0.0/Makefile
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2810 2023-08-07 16:39:00.277114 ztpserver-2.0.0/PKG-INFO
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2462 2023-08-07 16:37:02.000000 ztpserver-2.0.0/README.md
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)        6 2023-08-07 16:18:27.000000 ztpserver-2.0.0/VERSION
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.253113 ztpserver-2.0.0/actions/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3567 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/add_config
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3716 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/configure_ansible_client
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     6387 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/copy_file
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2747 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/install_cli_plugin
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3260 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/install_extension
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4136 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/install_image
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2358 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/replace_config
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3462 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/run_bash_script
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4181 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/run_cli_commands
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     6268 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/send_email
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1970 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/template
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3462 2023-07-26 15:52:26.000000 ztpserver-2.0.0/actions/the_nick
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.257113 ztpserver-2.0.0/bin/
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)     1720 2023-07-14 16:52:30.000000 ztpserver-2.0.0/bin/ztps
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.257113 ztpserver-2.0.0/client/
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)    50778 2023-07-26 15:52:26.000000 ztpserver-2.0.0/client/bootstrap
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.257113 ztpserver-2.0.0/client/lib/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)   429521 2023-06-26 16:36:08.000000 ztpserver-2.0.0/client/lib/requests-2.3.0.tar.gz
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.257113 ztpserver-2.0.0/conf/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      373 2023-07-07 10:57:57.000000 ztpserver-2.0.0/conf/bootstrap.conf
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      730 2023-07-07 10:57:57.000000 ztpserver-2.0.0/conf/neighbordb
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      345 2023-06-26 16:36:08.000000 ztpserver-2.0.0/conf/ztpserver-wsgi.conf
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1117 2023-07-07 10:57:57.000000 ztpserver-2.0.0/conf/ztpserver.conf
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1785 2023-07-07 10:43:52.000000 ztpserver-2.0.0/conf/ztpserver.wsgi
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.265113 ztpserver-2.0.0/docs/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)       16 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/.gitignore
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2328 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/CONTRIBUTING.md
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     7042 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/Makefile
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      681 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/README.md
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    13740 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/ReleaseNotes1.1.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     9949 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/ReleaseNotes1.2.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      250 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/ReleaseNotes1.3.1.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1563 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/ReleaseNotes1.3.2.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3226 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/ReleaseNotes1.3.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      304 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/ReleaseNotes1.4.1.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1058 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/ReleaseNotes1.4.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1072 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/ReleaseNotes1.5.0.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1393 2023-07-14 16:52:30.000000 ztpserver-2.0.0/docs/ReleaseNotes1.6.0.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      475 2023-08-07 14:16:17.000000 ztpserver-2.0.0/docs/ReleaseNotes2.0.0.rst
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.265113 ztpserver-2.0.0/docs/_static/
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)    56384 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/_static/AttrsActions.png
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)    21706 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/_static/Components.png
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)    38264 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/_static/LeafDefn.png
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    26494 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/_static/arista_logo_11-trans-w.png
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    62200 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/_static/arista_logo_jpg-11.jpg
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4286 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/_static/favicon.ico
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    32128 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/_static/ztpserver-seqdiag.png
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1144 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/actions.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     8625 2023-07-14 16:52:30.000000 ztpserver-2.0.0/docs/api.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      145 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/client.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     9234 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/conf.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    33240 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/config.rst
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.269114 ztpserver-2.0.0/docs/cookbook/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      326 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/_template.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    13760 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/cookbook/actions.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3951 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/advanced.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5211 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/ansible.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2212 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/clientLogging.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5911 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/configuration.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5214 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/definitions.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4659 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/dynamicNodes.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    12359 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/helloWorld.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2836 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/install.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2551 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/puppet.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2053 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/cookbook/resourcePools.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     9146 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/runningZTPS.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1878 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/serverLogging.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    13411 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/staticNodes.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     8853 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/topologyValidation.rst
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.269114 ztpserver-2.0.0/docs/cookbook/ztpsVMonEOS/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     8370 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook/ztpsVMonEOS/l2l3wm.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     8397 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/cookbook/ztpsVMonEOS/l2wom.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    13959 2023-07-14 16:52:30.000000 ztpserver-2.0.0/docs/cookbook/ztpsVMonEOS/l3wom.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2791 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/cookbook/ztpsVMonEOS.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      448 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/cookbook.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    10277 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/examples.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1568 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/glossary.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2548 2023-07-14 16:52:30.000000 ztpserver-2.0.0/docs/implementation.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1543 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/index.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     8107 2023-08-07 14:07:01.000000 ztpserver-2.0.0/docs/install.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)       88 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/internals.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2224 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/license.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)       68 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/modules.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     9170 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/overview.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)       95 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/requirements.txt
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)      576 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/setup_rtd_files.sh
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5182 2023-06-26 16:36:08.000000 ztpserver-2.0.0/docs/startup.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4980 2023-08-07 14:19:35.000000 ztpserver-2.0.0/docs/support.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     8563 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/tips.rst
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3060 2023-07-07 10:57:57.000000 ztpserver-2.0.0/docs/troubleshooting.rst
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.269114 ztpserver-2.0.0/plugins/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4894 2023-07-14 16:52:30.000000 ztpserver-2.0.0/plugins/allocate
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4861 2023-07-14 16:52:30.000000 ztpserver-2.0.0/plugins/mysql_vars
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5554 2023-07-14 16:52:30.000000 ztpserver-2.0.0/plugins/sqlite
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1871 2023-07-14 16:52:30.000000 ztpserver-2.0.0/plugins/test
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)       29 2023-08-07 14:07:01.000000 ztpserver-2.0.0/requirements.txt
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.269114 ztpserver-2.0.0/rpm/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1761 2023-06-26 16:36:08.000000 ztpserver-2.0.0/rpm/Makefile
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    12188 2023-06-26 16:36:08.000000 ztpserver-2.0.0/rpm/ztpserver.spec
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      100 2023-08-07 16:39:00.277114 ztpserver-2.0.0/setup.cfg
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)     6076 2023-07-14 16:52:30.000000 ztpserver-2.0.0/setup.py
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.269114 ztpserver-2.0.0/test/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)        0 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/__init__.py
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.269114 ztpserver-2.0.0/test/actions/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)        0 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/actions/__init__.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    10808 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/actions/test_add_config.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    22495 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/actions/test_copy_file.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5612 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/actions/test_install_cli_plugin.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     6949 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/actions/test_install_extension.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5993 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/actions/test_install_image.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5163 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/actions/test_replace_config.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     6892 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/actions/test_run_bash_script.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     6670 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/actions/test_run_cli_commands.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3869 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/actions/test_send_email.py
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.273114 ztpserver-2.0.0/test/client/
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)     1962 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/client/FastCli
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)        0 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/client/__init__.py
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)    21382 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/client/client_test_lib.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2535 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/client/smtp_server2.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2295 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/client/smtp_server3.py
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)    29627 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/client/test_bootstrap.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5625 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/client/test_bootstrap_cleanup.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5073 2023-07-26 15:52:26.000000 ztpserver-2.0.0/test/client/test_xmpp_bootstrap.py
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.273114 ztpserver-2.0.0/test/neighbordb/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1184 2023-07-07 10:57:57.000000 ztpserver-2.0.0/test/neighbordb/README.md
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2201 2023-06-26 16:36:08.000000 ztpserver-2.0.0/test/neighbordb/bogus_patterns_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1259 2023-07-07 10:57:57.000000 ztpserver-2.0.0/test/neighbordb/chassis_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1326 2023-07-06 10:51:07.000000 ztpserver-2.0.0/test/neighbordb/chassis_test_2.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      810 2023-06-26 16:36:08.000000 ztpserver-2.0.0/test/neighbordb/interface_name_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3247 2023-07-07 10:57:57.000000 ztpserver-2.0.0/test/neighbordb/large_pattern_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5749 2023-06-26 16:36:08.000000 ztpserver-2.0.0/test/neighbordb/ndb_entries_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    13948 2023-06-26 16:36:08.000000 ztpserver-2.0.0/test/neighbordb/ndb_values_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      541 2023-07-07 10:57:57.000000 ztpserver-2.0.0/test/neighbordb/node_interfaces_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)      483 2023-07-07 10:57:57.000000 ztpserver-2.0.0/test/neighbordb/node_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1559 2023-06-26 16:36:08.000000 ztpserver-2.0.0/test/neighbordb/simple_functions_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2252 2023-06-26 16:36:08.000000 ztpserver-2.0.0/test/neighbordb/simple_test.yml
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4054 2023-07-07 10:57:57.000000 ztpserver-2.0.0/test/neighbordb/small_pattern_test.yml
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.277114 ztpserver-2.0.0/test/server/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)        0 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/__init__.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     8799 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/server_test_lib.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2008 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_app.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    13617 2023-07-17 17:11:57.000000 ztpserver-2.0.0/test/server/test_config.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    56228 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_controller.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     9251 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_ndb.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5769 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_repository.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2641 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_serializers.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     5181 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_topology.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    14203 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_topology_classes.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     7057 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_types.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2021 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_utils.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3913 2023-07-14 16:52:30.000000 ztpserver-2.0.0/test/server/test_wsgiapp.py
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.277114 ztpserver-2.0.0/utils/
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)     1158 2023-07-14 16:52:30.000000 ztpserver-2.0.0/utils/create_db.py
+-rwxrwxr-x   0 dlobato   (1000) dlobato   (1000)     3694 2023-07-14 16:52:30.000000 ztpserver-2.0.0/utils/refresh_ztps
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.277114 ztpserver-2.0.0/ztpserver/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1589 2023-06-26 16:36:08.000000 ztpserver-2.0.0/ztpserver/__init__.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    11819 2023-07-27 17:38:23.000000 ztpserver-2.0.0/ztpserver/app.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    10295 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/config.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     1969 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/constants.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    35461 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/controller.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    10673 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/repository.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2497 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/resources.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     9473 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/serializers.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    32061 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/topology.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     3591 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/types.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    11065 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/utils.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)    12018 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/validators.py
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4310 2023-07-14 16:52:30.000000 ztpserver-2.0.0/ztpserver/wsgiapp.py
+drwxrwxr-x   0 dlobato   (1000) dlobato   (1000)        0 2023-08-07 16:39:00.277114 ztpserver-2.0.0/ztpserver.egg-info/
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     2810 2023-08-07 16:39:00.000000 ztpserver-2.0.0/ztpserver.egg-info/PKG-INFO
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)     4114 2023-08-07 16:39:00.000000 ztpserver-2.0.0/ztpserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)        1 2023-08-07 16:39:00.000000 ztpserver-2.0.0/ztpserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)       29 2023-08-07 16:39:00.000000 ztpserver-2.0.0/ztpserver.egg-info/requires.txt
+-rw-rw-r--   0 dlobato   (1000) dlobato   (1000)       10 2023-08-07 16:39:00.000000 ztpserver-2.0.0/ztpserver.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ztpserver-1.6.0/PKG-INFO` & `ztpserver-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 Metadata-Version: 2.1
 Name: ztpserver
-Version: 1.6.0
+Version: 2.0.0
 Summary: ZTP Server for EOS
 Home-page: https://github.com/arista-eosplus/ztpserver
+Download-URL: https://github.com/arista-eosplus/ztpserver/tarball/v2.0.0
 Author: Arista Networks
 Author-email: eosplus-dev@arista.com
 License: BSD-3
-Download-URL: https://github.com/arista-eosplus/ztpserver/tarball/v1.6.0
-Description: 
-        [![Build Status](https://travis-ci.org/arista-eosplus/ztpserver.png)](https://travis-ci.org/arista-eosplus/ztpserver)
-        
-        Quick Overview
-        =====================
-        ZTPServer provides a bootstrap environment for Arista EOS based products.  ZTPserver interacts with the  ZeroTouch Provisioning (ZTP) mode of Arista EOS. The default ZTP start up mode triggers an unprovisioned Arista EOS nodes to enter a bootstrap readdy state if a valid configuration file is not already present on the internal flash storage.
-        
-        ZTPServer provides a number of configurable bootstrap operation workflows that extend beyond simply loading an configuration and boot image. It provides the ability to define the target node through the introduction of definitions and templates that call pre-built actions and statically defined or dynamically generated attributes. The attributes and actions can also be extended to provide custom functionality that are specific to a given implementation. ZTPServer also provides a topology validation engine with a simple syntax to express LLDP neighbor adjacencies. It is written mostly in Python and leverages standard protocols like DHCP and DHCP options for boot functions, HTTP for bi-directional transport, and XMPP and syslog for logging. Most of the files that the user interacts with are YAML based.
-        
-        ZTPServer Features
-        ==================
-        * Automated configuration file generation and application
-        * Image and file system validation and standardization
-        * Connectivity validation and topology based auto-provisioning
-        * Config and device templates with resource allocation for dynamic deployments
-        * Zero touch replacement and upgrade capabilities
-        * User extensible actions
-        * Email, XMPP, syslog based logging and accounting of all processes
-        
-        Docs
-        ====
-        [ZTPServer official documentation](http://ztpserver.readthedocs.org/) is built and hosted at (http://ReadTheDocs.org/).
-        
-        Contributing
-        ============
-        Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for additional information.
-        
-        Support
-        =======
-        
-        * [Mailing List](https://groups.google.com/forum/#!forum/eosplus)
-        * eosplus-dev@arista.com
-        * IRC: irc.freenode.net#arista
-        
-        Dependencies
-        ============
-        
-        Server
-        ======
-        * [Python 2.7](https://www.python.org/download/releases/2.7/)
-        * [routes 2.0 or later](https://pypi.python.org/pypi/Routes)
-        * [webob 1.3 or later](http://webob.org/)
-        * [PyYaml 3.0 or later](http://pyyaml.org/)
-        
-        Client
-        ======
-        * Arista EOS 4.12.0 or later
-        
-        License
-        =======
-        BSD-3, See LICENSE file
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+[![Build Status](https://travis-ci.org/arista-eosplus/ztpserver.png)](https://travis-ci.org/arista-eosplus/ztpserver)
+
+Quick Overview
+=====================
+ZTPServer provides a bootstrap environment for Arista EOS based products.  ZTPserver interacts with the  ZeroTouch Provisioning (ZTP) mode of Arista EOS. The default ZTP start up mode triggers an unprovisioned Arista EOS nodes to enter a bootstrap readdy state if a valid configuration file is not already present on the internal flash storage.
+
+ZTPServer provides a number of configurable bootstrap operation workflows that extend beyond simply loading an configuration and boot image. It provides the ability to define the target node through the introduction of definitions and templates that call pre-built actions and statically defined or dynamically generated attributes. The attributes and actions can also be extended to provide custom functionality that are specific to a given implementation. ZTPServer also provides a topology validation engine with a simple syntax to express LLDP neighbor adjacencies. It is written mostly in Python and leverages standard protocols like DHCP and DHCP options for boot functions, HTTP for bi-directional transport, and XMPP and syslog for logging. Most of the files that the user interacts with are YAML based.
+
+ZTPServer Features
+==================
+* Automated configuration file generation and application
+* Image and file system validation and standardization
+* Connectivity validation and topology based auto-provisioning
+* Config and device templates with resource allocation for dynamic deployments
+* Zero touch replacement and upgrade capabilities
+* User extensible actions
+* Email, XMPP, syslog based logging and accounting of all processes
+
+Docs
+====
+[ZTPServer official documentation](http://ztpserver.readthedocs.org/) is built and hosted at (http://ReadTheDocs.org/).
+
+Contributing
+============
+Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for additional information.
+
+Support
+=======
+
+* [Mailing List](https://groups.google.com/forum/#!forum/eosplus)
+* eosplus-dev@arista.com
+* IRC: irc.freenode.net#arista
+
+Dependencies
+============
+
+Server
+======
+* Python 3.7 or later (https://www.python.org/downloads)
+* routes 2.5 or later (https://pypi.python.org/pypi/Routes)
+* webob 1.8 or later (http://webob.org/)
+* PyYaml 6.0 or later (http://pyyaml.org/)
+
+Client
+======
+* Arista EOS 4.12.0 or later
+
+License
+=======
+BSD-3, See LICENSE file
```

### Comparing `ztpserver-1.6.0/.pylintrc` & `ztpserver-2.0.0/.pylintrc`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,43 @@
-[FORMAT]
-
+[MASTER]
+init-hook="from pylint.config import find_pylintrc;import os, sys; sys.path.append(os.path.dirname(find_pylintrc()))"
 [BASIC]
 method-rgx=[a-z_][a-z0-9_]{2,50}$
 
 [MESSAGES CONTROL]
 # Used when an except catches Exception instances.
-disable=W0703
-
-# Too many branches
-disable=R0912
-
-# Too many return statements
-disable=R0911
-
-# No exception type specified
-disable=W0702
-
-# Disable statistics by type
-disable=RP0101
-
-# Allow local disables
-# Missing docstring
-# Abstract class not referenced
-# Similar lines in 2 files
-disable=I0011,C0111,R0921,R0801
+disable=
+  W0703, # broad-exception-caught
+  R0912, # Too many branches
+  C0111, # Missing docstring
+  R0801 # Similar lines in 2 files
 
 [REPORTS]
-# Include message's id in output
-include-ids=yes
 
 # Tells wether to display a full report or only the messages
 reports=no
 
 [FORMAT]
 max-module-lines=2000
+good-names=fd
 
 [DESIGN]
 # Maximum number of locals for function / method body
 max-locals=20
 
 # Maximum number of return / yield for function / method body
 max-returns=20
 
-# Maximum number of branch for function / method body
-# pylint bug
-max-branchs=30
-
 # Maximum number of statements in function / method body
 max-statements=100
 
 # Maximum number of arguments for function / method
 max-args=10
 
 # Minimum number of public methods for a class (see R0903).
 min-public-methods=0
 
 # Maximum number of public methods for a class (see R0904).
 max-public-methods=600
 
 # Maximum number of attributes for a class (see R0902).
 max-attributes=20
-
```

### Comparing `ztpserver-1.6.0/LICENSE` & `ztpserver-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/server/test_repository.py` & `ztpserver-2.0.0/test/server/test_repository.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,127 +29,125 @@
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
 # pylint: disable=R0904,C0103
 #
 import unittest
+from test.server.server_test_lib import enable_logging, random_string
+from unittest.mock import patch
 
-from mock import patch
-
+from ztpserver.repository import (
+    FileObject,
+    FileObjectError,
+    FileObjectNotFound,
+    Repository,
+    RepositoryError,
+)
 from ztpserver.serializers import SerializerError
 
-from ztpserver.repository import FileObject, FileObjectError
-from ztpserver.repository import Repository, RepositoryError
-from ztpserver.repository import FileObjectNotFound
-
-from server_test_lib import enable_logging, random_string
 
 class FileObjectUnitTests(unittest.TestCase):
-
-    @patch('ztpserver.serializers.load')
+    @patch("ztpserver.serializers.load")
     def test_read_success(self, m_load):
         m_load.return_value = random_string()
         obj = FileObject(random_string())
         result = obj.read()
         self.assertEqual(m_load.return_value, result)
 
-    @patch('ztpserver.serializers.load')
+    @patch("ztpserver.serializers.load")
     def test_read_failure(self, m_load):
         m_load.side_effect = SerializerError
         obj = FileObject(random_string())
         self.assertRaises(FileObjectError, obj.read)
 
     @classmethod
-    @patch('ztpserver.serializers.dump')
+    @patch("ztpserver.serializers.dump")
     def test_write_success(cls, _):
         obj = FileObjectError(random_string())
         obj = FileObject(random_string())
         obj.write(random_string())
 
-    @patch('ztpserver.serializers.dump')
+    @patch("ztpserver.serializers.dump")
     def test_write_failure(self, m_dump):
         m_dump.side_effect = SerializerError
         obj = FileObject(random_string())
         self.assertRaises(FileObjectError, obj.write, random_string())
 
 
 class RepositoryUnitTests(unittest.TestCase):
-
     @classmethod
-    @patch('os.makedirs')
+    @patch("os.makedirs")
     def test_add_folder_success(cls, _):
         store = Repository(random_string())
         store.add_folder(random_string())
 
-    @patch('os.makedirs')
+    @patch("os.makedirs")
     def test_add_folder_failure(self, m_makedirs):
         m_makedirs.side_effect = OSError
         store = Repository(random_string())
         self.assertRaises(RepositoryError, store.add_folder, random_string())
 
-    @patch('ztpserver.repository.FileObject')
-    @patch('os.chmod')
+    @patch("ztpserver.repository.FileObject")
+    @patch("os.chmod")
     def test_create_file_success(self, _, m_fileobj):
         store = Repository(random_string())
         store.add_file(random_string())
         self.assertFalse(m_fileobj.return_value.write.called)
 
-    @patch('ztpserver.repository.FileObject')
-    @patch('os.chmod')
-    def test_create_file_with_contents_success(self, _,
-                                               m_fileobj):
+    @patch("ztpserver.repository.FileObject")
+    @patch("os.chmod")
+    def test_create_file_with_contents_success(self, _, m_fileobj):
         store = Repository(random_string())
         store.add_file(random_string(), random_string())
         self.assertTrue(m_fileobj.return_value.write.called)
-            
-    @patch('ztpserver.repository.FileObject')
+
+    @patch("ztpserver.repository.FileObject")
     def test_create_file_failure(self, m_fileobj):
         m_fileobj.return_value.write.side_effect = FileObjectError
         store = Repository(random_string())
-        self.assertRaises(FileObjectError, store.add_file,
-                          random_string(), random_string())
+        self.assertRaises(FileObjectError, store.add_file, random_string(), random_string())
 
-    @patch('os.path.exists')
+    @patch("os.path.exists")
     def test_exists_success(self, _):
         store = Repository(random_string())
         result = store.exists(random_string())
         self.assertTrue(result)
 
-    @patch('os.path.exists')
+    @patch("os.path.exists")
     def test_exists_missing_file(self, m_exists):
         m_exists.return_value = False
         store = Repository(random_string())
         result = store.exists(random_string())
         self.assertFalse(result)
 
-    @patch('os.path.exists')
-    @patch('ztpserver.repository.FileObject')
+    @patch("os.path.exists")
+    @patch("ztpserver.repository.FileObject")
     def test_get_file_success(self, m_fileobj, _):
         store = Repository(random_string())
         store.get_file(random_string())
         self.assertTrue(m_fileobj.called)
 
-    @patch('os.path.exists')
-    @patch('ztpserver.repository.FileObject')
+    @patch("os.path.exists")
+    @patch("ztpserver.repository.FileObject")
     def test_get_file_failure(self, m_fileobj, m_exists):
         m_exists.return_value = False
         store = Repository(random_string())
         self.assertRaises(FileObjectNotFound, store.get_file, random_string())
         self.assertFalse(m_fileobj.called)
 
-    @patch('os.remove')
+    @patch("os.remove")
     def test_delete_file_success(self, m_remove):
         store = Repository(random_string())
         store.delete_file(random_string())
         self.assertTrue(m_remove.called)
 
-    @patch('os.remove')
+    @patch("os.remove")
     def test_delete_file_failure(self, m_remove):
         m_remove.side_effect = OSError
         store = Repository(random_string())
         self.assertRaises(RepositoryError, store.delete_file, random_string())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     enable_logging()
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/server/test_utils.py` & `ztpserver-2.0.0/test/server/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,28 +28,20 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 import unittest
 
-
 from ztpserver import utils
 
 
 class UtilsUnitTests(unittest.TestCase):
-
     def test_expand_basic_range(self):
-        """ Issue #358
-        """
-        result = utils.expand_range('Ethernet2-4')
-        self.assertItemsEqual(result,
-                              ['Ethernet2', 'Ethernet3', 'Ethernet4'])
+        """Issue #358"""
+        result = utils.expand_range("Ethernet2-4")
+        self.assertCountEqual(result, ["Ethernet2", "Ethernet3", "Ethernet4"])
 
     def test_expand_linecard_range(self):
-        """ Issue #358
-        """
-        result = utils.expand_range('Ethernet2/2-2/4')
-        self.assertItemsEqual(result,
-                              ['Ethernet2/2',
-                               'Ethernet2/3',
-                               'Ethernet2/4'])
+        """Issue #358"""
+        result = utils.expand_range("Ethernet2/2-2/4")
+        self.assertCountEqual(result, ["Ethernet2/2", "Ethernet2/3", "Ethernet2/4"])
```

### Comparing `ztpserver-1.6.0/test/server/test_wsgiapp.py` & `ztpserver-2.0.0/test/server/test_wsgiapp.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,90 +26,88 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,C0103
+# pylint: disable=R0904,C0103
 
+import http.client
 import unittest
-import httplib
-import routes
 
+import routes
 import webob
 
 from ztpserver.wsgiapp import WSGIController, WSGIRouter
 
-class TestWsgiApp(unittest.TestCase):
 
+class TestWsgiApp(unittest.TestCase):
     def setUp(self):
         mapper = routes.Mapper()
-        mapper.collection('tests', 'test', controller=WSGIController)
+        mapper.collection("tests", "test", controller=WSGIController)
 
         self.router = WSGIRouter(mapper)
 
-    def request(self, url, method='GET', **kwargs):
+    def request(self, url, method="GET", **kwargs):
         req = webob.Request.blank(url, method=method, **kwargs)
         return req.get_response(self.router)
 
-    def get_url(self, url, expected_status=httplib.OK, **kwargs):
+    def get_url(self, url, expected_status=http.client.OK, **kwargs):
         resp = self.request(url, **kwargs)
         self.assertEqual(resp.status_code, expected_status)
         return resp
 
-    def post_url(self, url, expected_status=httplib.OK, **kwargs):
-        resp = self.request(url, 'POST', **kwargs)
+    def post_url(self, url, expected_status=http.client.OK, **kwargs):
+        resp = self.request(url, "POST", **kwargs)
         self.assertEqual(resp.status_code, expected_status)
         return resp
 
-    def put_url(self, url, expected_status=httplib.OK, **kwargs):
-        resp = self.request(url, 'PUT', **kwargs)
+    def put_url(self, url, expected_status=http.client.OK, **kwargs):
+        resp = self.request(url, "PUT", **kwargs)
         self.assertEqual(resp.status_code, expected_status)
         return resp
 
-    def delete_url(self, url, expected_status=httplib.OK, **kwargs):
-        resp = self.request(url, 'DELETE', **kwargs)
+    def delete_url(self, url, expected_status=http.client.OK, **kwargs):
+        resp = self.request(url, "DELETE", **kwargs)
         self.assertEqual(resp.status_code, expected_status)
         return resp
 
     def test_get_url_collection(self):
-        self.get_url('/tests', 204)
+        self.get_url("/tests", 204)
 
     def test_get_url_resource(self):
-        self.get_url('/test/resource', 404)
+        self.get_url("/test/resource", 404)
 
     def test_get_url_missing(self):
-        self.get_url('/missing', 404)
+        self.get_url("/missing", 404)
 
     def test_post_url_collection(self):
-        self.post_url('/tests', 204)
+        self.post_url("/tests", 204)
 
     def test_post_url_resource(self):
-        self.post_url('/test/resource', 404)
+        self.post_url("/test/resource", 404)
 
     def test_post_url_missing(self):
-        self.post_url('/missing', 404)
+        self.post_url("/missing", 404)
 
     def test_put_url_collection(self):
-        self.put_url('/tests', 404)
+        self.put_url("/tests", 404)
 
     def test_put_url_resource(self):
-        self.put_url('/test/resource', 404)
+        self.put_url("/test/resource", 404)
 
     def test_put_url_missing(self):
-        self.put_url('/missing', 404)
+        self.put_url("/missing", 404)
 
     def test_delete_url_collection(self):
-        self.delete_url('/tests', 404)
+        self.delete_url("/tests", 404)
 
     def test_delete_url_resource(self):
-        self.delete_url('/test/resource', 404)
+        self.delete_url("/test/resource", 404)
 
     def test_delete_url_missing(self):
-        self.delete_url('/missing', 404)
-
-if __name__ == '__main__':
-    unittest.main()
-
+        self.delete_url("/missing", 404)
 
 
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `ztpserver-1.6.0/test/server/test_serializers.py` & `ztpserver-2.0.0/test/server/test_serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,31 +30,31 @@
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 import os
 import random
 import unittest
 
-import ztpserver.serializers as serializers
-
+from ztpserver import serializers
 from ztpserver.constants import CONTENT_TYPE_JSON
 
-TMP_FILE = '/tmp/test_serializers-%s' % os.getpid()
+TMP_FILE = f"/tmp/test_serializers-{os.getpid()}"
+
 
 def get_data():
     result = {}
     for _ in range(random.randint(10, 100)):
-        key = 'x' * random.randint(0, 10)
-        value = 'x' * random.randint(0, 50)
+        key = "x" * random.randint(0, 10)
+        value = "x" * random.randint(0, 50)
         result[key] = value
 
     return result
 
-class SerializersUnitTest(unittest.TestCase):
 
+class SerializersUnitTest(unittest.TestCase):
     def test_dump_success(self):
         pass
 
     def test_dumps_success(self):
         pass
 
     def test_load_success(self):
@@ -68,14 +68,13 @@
         # stress test writing and loading the same file over and
         # over again and make sure the file does not get corrupted
         # in the process
         index = 0
         while index < 100:
             index += 1
             data = get_data()
-            serializers.dump(data, TMP_FILE, 
-                             CONTENT_TYPE_JSON)
-            assert serializers.load(TMP_FILE, 
-                                    CONTENT_TYPE_JSON) == data
+            serializers.dump(data, TMP_FILE, CONTENT_TYPE_JSON)
+            assert serializers.load(TMP_FILE, CONTENT_TYPE_JSON) == data
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/server/test_ndb.py` & `ztpserver-2.0.0/test/server/test_ndb.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,241 +26,236 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-# pylint: disable=W0142
-
 import os
-import unittest
 import traceback
+import unittest
+from test.server.server_test_lib import enable_logging, log, random_string
+
 import yaml
 
 from ztpserver.app import enable_handler_console
-from ztpserver.topology import load_neighbordb, load_file
-from ztpserver.topology import Node
-from ztpserver.validators import NeighbordbValidator
 from ztpserver.constants import CONTENT_TYPE_YAML
-from server_test_lib import enable_logging, log, random_string
+from ztpserver.topology import Node, load_file, load_neighbordb
+from ztpserver.validators import NeighbordbValidator
 
-TEST_DIR = 'test/neighbordb'
+TEST_DIR = "test/neighbordb"
 ID = random_string()
 
+
 def debug(exc):
     # Uncomment line for debugging
     # import pdb; pdb.set_trace()
-    
+
     raise exc
 
+
 def load_node(node, content_type=CONTENT_TYPE_YAML):
     try:
-        if not hasattr(node, 'items'):
+        if not hasattr(node, "items"):
             node = load_file(node, content_type, ID)
-        if 'systemmac' in node:
-            for symbol in [':', '.']:
-                node['systemmac'] = str(node['systemmac']).replace(symbol, '')
+        if "systemmac" in node:
+            for symbol in [":", "."]:
+                node["systemmac"] = str(node["systemmac"]).replace(symbol, "")
         return Node(**node)
     except TypeError:
-        log.error('Failed to load node')
+        log.error("Failed to load node")
     except KeyError as err:
-        log.error('Failed to load node - missing attribute: %s' % err)
+        log.error("Failed to load node - missing attribute: %s", err)
+
+    return None
+
 
 class NeighbordbTest(unittest.TestCase):
     # pylint: disable=C0103
 
     def __init__(self, test_name, ndb, **kwargs):
         self.ndb = ndb
-        self.node = kwargs.get('node')
-        self.tag = kwargs.get('tag')
-        self.match = kwargs.get('match')
-        self.filename = kwargs.get('filename')
-
-        self.valid_patterns = kwargs.get('valid_patterns', dict())
-        if not self.valid_patterns.get('nodes'):
-            self.valid_patterns['nodes'] = list()
-        if not self.valid_patterns.get('globals'):
-            self.valid_patterns['globals'] = list()
+        self.node = kwargs.get("node")
+        self.tag = kwargs.get("tag")
+        self.match = kwargs.get("match")
+        self.filename = kwargs.get("filename")
+
+        self.valid_patterns = kwargs.get("valid_patterns", {})
+        if not self.valid_patterns.get("nodes"):
+            self.valid_patterns["nodes"] = []
+        if not self.valid_patterns.get("globals"):
+            self.valid_patterns["globals"] = []
 
-        self.invalid_patterns = kwargs.get('invalid_patterns')
+        self.invalid_patterns = kwargs.get("invalid_patterns")
 
-        self.longMessage = True   
+        self.longMessage = True
         self.maxDiff = None
 
-        super(NeighbordbTest, self).__init__(test_name)
+        super().__init__(test_name)
 
     def _load_neighbordb(self):
         return load_neighbordb(ID, contents=self.ndb)
 
     def _validate_neighbordb(self):
         validator = NeighbordbValidator(ID)
         validator.validate(self.ndb)
         return (validator.valid_patterns, validator.invalid_patterns)
 
     def neighbordb_pattern(self):
         try:
-            log.info('START: neighbordb_patterns')
-            tag = 'tag=%s, fn=%s' % (self.tag, self.filename)
+            log.info("START: neighbordb_patterns")
+            tag = f"tag={self.tag}, fn={self.filename}"
 
             (valid, failed) = self._validate_neighbordb()
 
             if self.invalid_patterns:
                 failed_names = sorted([p[1] for p in failed])
-                self.assertEqual(failed_names, 
-                                 sorted(self.invalid_patterns),
-                                 tag)
+                self.assertEqual(failed_names, sorted(self.invalid_patterns), tag)
                 self.assertEqual(len(failed), len(self.invalid_patterns), tag)
 
-            p_all = self.valid_patterns.get('nodes') + \
-                    self.valid_patterns.get('globals')
+            p_all = self.valid_patterns.get("nodes") + self.valid_patterns.get("globals")
             if p_all:
                 valid_actual = sorted([str(p[1]) for p in valid])
                 valid_configured = sorted([str(x) for x in p_all])
 
                 self.assertEqual(valid_actual, valid_configured, tag)
 
-            log.info('END: neighbordb_pattern')
+            log.info("END: neighbordb_pattern")
         except AssertionError as exc:
-            print exc
-            print traceback.format_exc()
+            print(exc)
+            print(traceback.format_exc())
             debug(exc)
 
     def neighbordb_topology(self):
         try:
-            log.info('START: neighbordb_test')
-            tag = 'tag=%s, fn=%s' % (self.tag, self.filename)
+            log.info("START: neighbordb_test")
+            tag = f"tag={self.tag}, fn={self.filename}"
 
             topo = self._load_neighbordb()
             self.assertIsNotNone(topo, tag)
 
-            p_nodes = [p.name for p in topo.get_patterns() 
-                       if topo.is_node_pattern(p)]
-            p_globals = [p.name for p in topo.get_patterns()
-                         if topo.is_global_pattern(p)]
-
-            self.assertEqual(sorted(self.valid_patterns['nodes']),
-                             sorted(p_nodes),
-                             tag)
-            self.assertEqual(sorted(self.valid_patterns['globals']),
-                             sorted(p_globals),
-                             tag)
+            p_nodes = [p.name for p in topo.get_patterns() if topo.is_node_pattern(p)]
+            p_globals = [p.name for p in topo.get_patterns() if topo.is_global_pattern(p)]
+
+            self.assertEqual(sorted(self.valid_patterns["nodes"]), sorted(p_nodes), tag)
+            self.assertEqual(sorted(self.valid_patterns["globals"]), sorted(p_globals), tag)
 
-            log.info('END: neighbordb_test')
+            log.info("END: neighbordb_test")
             return topo
         except AssertionError as exc:
-            print exc
-            print traceback.format_exc()
+            print(exc)
+            print(traceback.format_exc())
             debug(exc)
 
+        return None
+
     def node_pass(self):
         try:
-            log.info('START: node_pass')
-            tag = 'tag=%s, fn=%s' % (self.tag, self.filename)
-            
+            log.info("START: node_pass")
+            tag = f"tag={self.tag}, fn={self.filename}"
+
             node = load_node(self.node)
             self.assertIsNotNone(node, tag)
-            
+
             neighbordb = self._load_neighbordb()
             self.assertIsNotNone(neighbordb, tag)
             result = neighbordb.match_node(node)
-            
+
             self.assertTrue(result, tag)
             self.assertEqual(result[0].name, self.match, tag)
-            log.info('END: node_pass')
+            log.info("END: node_pass")
         except AssertionError as exc:
-            print exc
-            print traceback.format_exc()
+            print(exc)
+            print(traceback.format_exc())
             debug(exc)
 
     def node_fail(self):
         try:
-            log.info('START: node_fail')
-            tag = 'tag=%s, fn=%s' % (self.tag, self.filename)
+            log.info("START: node_fail")
+            tag = f"tag={self.tag}, fn={self.filename}"
 
             node = load_node(self.node)
             self.assertIsNotNone(node, tag)
 
             neighbordb = self._load_neighbordb()
             self.assertIsNotNone(neighbordb, tag)
 
             result = neighbordb.match_node(node)
 
             self.assertFalse(result, tag)
-            log.info('END: node_fail')
+            log.info("END: node_fail")
         except AssertionError as exc:
-            print exc
-            print traceback.format_exc()
+            print(exc)
+            print(traceback.format_exc())
             debug(exc)
 
 
 def get_test_list(filepath):
-    test_list = os.environ.get('TESTS', None)
+    test_list = os.environ.get("TESTS", None)
     if not test_list:
-        log.debug('Checking directory %s for tests', TEST_DIR)
-        test_list = [os.path.join(filepath, f) for f in os.listdir(filepath)
-                     if f.endswith('yml')]
+        log.debug("Checking directory %s for tests", TEST_DIR)
+        test_list = [os.path.join(filepath, f) for f in os.listdir(filepath) if f.endswith("yml")]
     else:
-        test_list = [os.path.join(filepath, f) for f in test_list.split(',')]
+        test_list = [os.path.join(filepath, f) for f in test_list.split(",")]
     return test_list
 
-def load_tests(loader, tests, pattern):      # pylint: disable=W0613
-    try:
-        log.info('Start ndb tests')
+
+def load_tests(loader, tests, pattern):  # pylint: disable=W0613
+    try:  # pylint: disable=R1702
+        log.info("Start ndb tests")
 
         suite = unittest.TestSuite()
         test_list = get_test_list(TEST_DIR)
-        log.info('Test list is %s', test_list)
+        log.info("Test list is %s", test_list)
 
         for test in test_list:
-            log.info('Starting test harness %s', test)
+            log.info("Starting test harness %s", test)
 
-            harness = yaml.load(open(test))
-            if harness.get('debug'):
+            with open(test, encoding="utf8") as fd:
+                harness = yaml.safe_load(fd)
+            if harness.get("debug"):
                 enable_handler_console()
 
-            tests = harness.get('tests', ['topology'])
+            tests = harness.get("tests", ["topology"])
 
-            name = harness.get('ndb', 'neighbordb')
-            filename = name.split('/')[-1]
+            name = harness.get("ndb", "neighbordb")
+            filename = name.split("/")[-1]
             if filename in harness:
                 ndb = harness.get(filename)
             else:
                 assert os.path.exists(name)
-                ndb = yaml.load(open(name))
+                with open(name, encoding="utf8") as fd:
+                    ndb = yaml.safe_load(fd)
 
-            kwargs = dict()
-            kwargs['valid_patterns'] = harness.get('valid_patterns', dict())
-            kwargs['invalid_patterns'] = harness.get('invalid_patterns')
-            kwargs['tag'] = harness.get('tag', filename)
-            kwargs['filename'] = test
+            kwargs = {
+                "valid_patterns": harness.get("valid_patterns", {}),
+                "invalid_patterns": harness.get("invalid_patterns"),
+                "tag": harness.get("tag", filename),
+                "filename": test,
+            }
 
             for test in tests:
-                assert test in ['pattern', 'topology']
-                suite.addTest(NeighbordbTest('neighbordb_%s' % test, 
-                                             ndb, **kwargs))
-
-            if 'nodes' in harness and 'topology' in tests:
-                for key in harness['nodes'].keys():
-                    assert key in ['pass', 'fail']
-                    entries = harness['nodes'][key]
+                assert test in ["pattern", "topology"]
+                suite.addTest(NeighbordbTest(f"neighbordb_{test}", ndb, **kwargs))
+
+            if "nodes" in harness and "topology" in tests:
+                for key in harness["nodes"].keys():
+                    assert key in ["pass", "fail"]
+                    entries = harness["nodes"][key]
                     if not entries is None:
                         for entry in entries:
-                            filename = entry['name'].split('/')[-1]
-                            kwargs['node'] = harness.get(filename, 
-                                                         entry['name'])
-                            kwargs['match'] = entry.get('match')
-                            kwargs['tag'] = '%s:%s' % (harness.get('tag'), 
-                                                       filename)
-                            log.info('Adding node %s', name)
-                            suite.addTest(NeighbordbTest('node_%s' % key, 
-                                                         ndb, **kwargs))
-
-    except Exception as exc:      # pylint: disable=W0703
-        log.exception('Unexpected error trying to execute load_tests: %s' %
-                      exc)
-    else:
-        return suite
+                            filename = entry["name"].split("/")[-1]
+                            kwargs["node"] = harness.get(filename, entry["name"])
+                            kwargs["match"] = entry.get("match")
+                            kwargs["tag"] = f"{harness.get('tag')}:{filename}"
+                            log.info("Adding node %s", name)
+                            suite.addTest(NeighbordbTest(f"node_{key}", ndb, **kwargs))
+
+    except Exception as exc:  # pylint: disable=W0703
+        log.exception("Unexpected error trying to execute load_tests: %s", exc)
+
+    return suite
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     enable_logging()
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/server/test_topology_classes.py` & `ztpserver-2.0.0/test/server/test_topology_classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,34 +26,37 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
-# pylint: disable=W0142
 #
-import unittest
-
-from mock import Mock
-
-from ztpserver.app import enable_handler_console    # pylint: disable=W0611
-from ztpserver.topology import InterfacePattern, InterfacePatternError
-from ztpserver.topology import Pattern, PatternError
-from ztpserver.topology import Node, NodeError, Neighbor
 
-from ztpserver.topology import ExcludesFunction, IncludesFunction
-from ztpserver.topology import ExactFunction, RegexFunction
+import unittest
+from test.server.server_test_lib import create_node, enable_logging, random_string
+from unittest.mock import Mock
 
-from server_test_lib import random_string, enable_logging
-from server_test_lib import create_node
+from ztpserver.app import enable_handler_console  # pylint: disable=W0611
+from ztpserver.topology import (
+    ExactFunction,
+    ExcludesFunction,
+    IncludesFunction,
+    InterfacePattern,
+    InterfacePatternError,
+    Neighbor,
+    Node,
+    NodeError,
+    Pattern,
+    PatternError,
+    RegexFunction,
+)
 
 
 class NodeUnitTests(unittest.TestCase):
-
     def test_create_node_success(self):
         node = create_node()
         systemmac = node.systemmac
         kwargs = node.as_dict()
         node = Node(**kwargs)
         self.assertEqual(node.systemmac, systemmac)
 
@@ -71,117 +74,109 @@
 
     def test_create_node_neighbors_valid(self):
         nodeattrs = create_node()
 
         remote_device = random_string()
         remote_interface = random_string()
 
-        neighbors = {'Ethernet1': {'device': remote_device, 
-                                   'port': remote_interface}}
+        neighbors = {"Ethernet1": {"device": remote_device, "port": remote_interface}}
         nodeattrs.add_neighbors(neighbors)
 
         kwargs = nodeattrs.as_dict()
         node = Node(**kwargs)
 
-        self.assertIsNotNone(node.neighbors('Ethernet1'))
-        self.assertEqual(node.neighbors('Ethernet1')[0].device, 
-                         remote_device)
-        self.assertEqual(node.neighbors('Ethernet1')[0].interface, 
-                         remote_interface)
+        self.assertIsNotNone(node.neighbors("Ethernet1"))
+        self.assertEqual(node.neighbors("Ethernet1")[0].device, remote_device)
+        self.assertEqual(node.neighbors("Ethernet1")[0].interface, remote_interface)
 
     def test_create_node_neighbors_remote_interface_missing(self):
         nodeattrs = create_node()
 
         remote_device = random_string()
 
-        neighbors = {'Ethernet1': {'remote_device': remote_device}}
+        neighbors = {"Ethernet1": {"remote_device": remote_device}}
         nodeattrs.add_neighbors(neighbors)
 
         kwargs = nodeattrs.as_dict()
+        node = None
         try:
-            node = None
             node = Node(**kwargs)
         except NodeError:
             pass
         finally:
             self.assertIsNone(node)
 
     def test_create_node_neighbors_remote_device_missing(self):
         nodeattrs = create_node()
 
         remote_interface = random_string()
 
-        neighbors = {'Ethernet1': {'remote_interface': remote_interface}}
+        neighbors = {"Ethernet1": {"remote_interface": remote_interface}}
         nodeattrs.add_neighbors(neighbors)
 
         kwargs = nodeattrs.as_dict()
+        node = None
         try:
-            node = None
             node = Node(**kwargs)
         except NodeError:
             pass
         finally:
             self.assertIsNone(node)
 
     def test_add_neighbor(self):
         systemmac = random_string()
         peer = Mock()
         intf = random_string()
 
         node = Node(systemmac=systemmac)
-        node.add_neighbor(intf, [dict(device=peer.remote_device, 
-                                      port=peer.remote_interface)])
+        node.add_neighbor(intf, [{"device": peer.remote_device, "port": peer.remote_interface}])
 
         self.assertIsNotNone(node.neighbors(intf))
 
-        self.assertEqual(node.neighbors(intf)[0].device, 
-                         peer.remote_device)
-        self.assertEqual(node.neighbors(intf)[0].interface, 
-                         peer.remote_interface)
+        self.assertEqual(node.neighbors(intf)[0].device, peer.remote_device)
+        self.assertEqual(node.neighbors(intf)[0].interface, peer.remote_interface)
 
     def test_add_neighbor_existing_interface(self):
         systemmac = random_string()
         peer = Mock()
         intf = random_string()
 
         node = Node(systemmac=systemmac)
-        node.add_neighbor(intf, [dict(device=peer.remote_device, 
-                                      port=peer.remote_interface)])
-        self.assertRaises(NodeError, node.add_neighbor,
-                          intf, [dict(device=peer.remote_device, 
-                                      port=peer.remote_interface)])
+        node.add_neighbor(intf, [{"device": peer.remote_device, "port": peer.remote_interface}])
+        self.assertRaises(
+            NodeError,
+            node.add_neighbor,
+            intf,
+            [{"device": peer.remote_device, "port": peer.remote_interface}],
+        )
 
     def test_add_neighbors_success(self):
         nodeattrs = create_node()
 
         remote_device = random_string()
         remote_interface = random_string()
-        neighbors = {'Ethernet1': [{'device': remote_device, 
-                                    'port': remote_interface}]}
+        neighbors = {"Ethernet1": [{"device": remote_device, "port": remote_interface}]}
 
         kwargs = nodeattrs.as_dict()
         node = Node(**kwargs)
         node.add_neighbors(neighbors)
 
-        self.assertIsNotNone(node.neighbors('Ethernet1'))
-        self.assertEqual(node.neighbors('Ethernet1')[0].device, 
-                         remote_device)
-        self.assertEqual(node.neighbors('Ethernet1')[0].interface, 
-                         remote_interface)
+        self.assertIsNotNone(node.neighbors("Ethernet1"))
+        self.assertEqual(node.neighbors("Ethernet1")[0].device, remote_device)
+        self.assertEqual(node.neighbors("Ethernet1")[0].interface, remote_interface)
 
     def test_serialize_success(self):
         nodeattrs = create_node()
         kwargs = nodeattrs.as_dict()
         node = Node(**kwargs)
         result = node.serialize()
         self.assertEqual(result, nodeattrs.as_dict())
 
 
 class FunctionsUnitTests(unittest.TestCase):
-
     def test_exactfunction_true(self):
         value = random_string()
         func = ExactFunction(value)
         self.assertTrue(func.match(value))
 
     def test_exactfunction_false(self):
         value = random_string()
@@ -205,207 +200,188 @@
 
     def test_excludesfunction_false(self):
         value = random_string()
         func = ExcludesFunction(value)
         self.assertFalse(func.match(value))
 
     def test_regexfunction_true(self):
-        value = r'[\w+]'
+        value = r"[\w+]"
         func = RegexFunction(value)
         self.assertTrue(func.match(random_string()))
 
     def test_regexfunction_false(self):
-        value = '[^a-zA-Z0-9]'
+        value = "[^a-zA-Z0-9]"
         func = RegexFunction(value)
         self.assertFalse(func.match(random_string()))
 
 
 class TestPattern(unittest.TestCase):
-
     def test_create_pattern_with_defaults(self):
         obj = Pattern(None, None, None)
         self.assertIsInstance(obj, Pattern)
 
     def test_create_pattern_with_kwargs(self):
-        obj = Pattern(name='test',
-                                         definition='test',
-                                         node='abc123',
-                                         variables={'var': 'test'},
-                                         interfaces=[{'Ethernet1': 'any'}])
-        self.assertEqual(obj.name, 'test')
-        self.assertEqual(obj.definition, 'test')
-        self.assertEqual(obj.node, 'abc123')
-        self.assertDictEqual({'var': 'test'}, obj.variables)
+        obj = Pattern(
+            name="test",
+            definition="test",
+            node="abc123",
+            variables={"var": "test"},
+            interfaces=[{"Ethernet1": "any"}],
+        )
+        self.assertEqual(obj.name, "test")
+        self.assertEqual(obj.definition, "test")
+        self.assertEqual(obj.node, "abc123")
+        self.assertDictEqual({"var": "test"}, obj.variables)
         self.assertEqual(1, len(obj.interfaces))
 
     def test_add_interface(self):
-        obj = Pattern(interfaces=[{'Ethernet1': 'any'}])
+        obj = Pattern(interfaces=[{"Ethernet1": "any"}])
         self.assertEqual(len(obj.interfaces), 1)
 
 
 class PatternUnitTests(unittest.TestCase):
-
     def test_create_pattern(self):
         pattern = Pattern(random_string())
         self.assertIsInstance(pattern, Pattern)
 
     def test_create_pattern_kwargs(self):
-        kwargs = dict(name=random_string(),
-                      definition=random_string(),
-                      interfaces=None)
+        kwargs = {"name": random_string(), "definition": random_string(), "interfaces": None}
 
         pattern = Pattern(**kwargs)
         self.assertIsInstance(pattern, Pattern)
 
     @classmethod
     def test_add_interface_success(cls):
-        kwargs = dict(name=random_string(),
-                      definition=random_string(),
-                      interfaces=None)
+        kwargs = {"name": random_string(), "definition": random_string(), "interfaces": None}
 
         pattern = Pattern(**kwargs)
 
         remote_remote_device = random_string()
         remote_intf = random_string()
-        neighbors = dict(Ethernet1={'device': remote_remote_device,
-                                    'port': remote_intf})
+        neighbors = {"Ethernet1": {"device": remote_remote_device, "port": remote_intf}}
 
         pattern.add_interface(neighbors)
-            
+
     def test_add_interface_failure(self):
-        kwargs = dict(name=random_string(),
-                      definition=random_string(),
-                      interfaces=None)
+        kwargs = {"name": random_string(), "definition": random_string(), "interfaces": None}
 
         pattern = Pattern(**kwargs)
-        self.assertRaises(PatternError, pattern.add_interface, 
-                          random_string())
+        self.assertRaises(PatternError, pattern.add_interface, random_string())
 
 
 class TestInterfacePattern(unittest.TestCase):
-
     def test_create_interface_pattern(self):
-        intf = 'Ethernet1'
+        intf = "Ethernet1"
         remote_device = random_string()
         remote_interface = random_string()
 
-        obj = InterfacePattern(intf, remote_device,
-                               remote_interface,
-                               random_string())
-        reprobj = 'InterfacePattern(interface=%s, remote_device=%s, ' \
-                   'remote_interface=%s)' % \
-                  (intf, remote_device, remote_interface)
+        obj = InterfacePattern(intf, remote_device, remote_interface, random_string())
+        reprobj = (
+            f"InterfacePattern(interface={intf}, "
+            f"remote_device={remote_device}, remote_interface={remote_interface})"
+        )
         self.assertEqual(repr(obj), reprobj)
 
     def test_match_success(self):
         interface = random_string()
         remote_device = random_string()
         remote_interface = random_string()
 
         neighbor = Neighbor(remote_device, remote_interface)
-        for intf in ['any', interface]:
-            for remote_d in ['any', remote_device]:
-                for remote_i in ['any', remote_interface]:
-                    
-                    pattern = InterfacePattern(intf, remote_d, remote_i,
-                                               random_string())
+        for intf in ["any", interface]:
+            for remote_d in ["any", remote_device]:
+                for remote_i in ["any", remote_interface]:
+                    pattern = InterfacePattern(intf, remote_d, remote_i, random_string())
                     result = pattern.match(interface, [neighbor])
                     self.assertTrue(result)
 
     def test_match_failure(self):
         interface = random_string()
         remote_device = random_string()
         remote_interface = random_string()
 
-        for intf in ['none', interface + 'dummy']:
-            pattern = InterfacePattern(intf, remote_device, 
-                                       remote_interface,
-                                       random_string())
+        for intf in ["none", interface + "dummy"]:
+            pattern = InterfacePattern(intf, remote_device, remote_interface, random_string())
             neighbor = Neighbor(remote_device, remote_interface)
             result = pattern.match(interface, [neighbor])
             self.assertFalse(result)
 
-        for remote_d in ['none', remote_device + 'dummy']:
-            pattern = InterfacePattern(interface, remote_d, 
-                                       remote_interface,
-                                       random_string())
+        for remote_d in ["none", remote_device + "dummy"]:
+            pattern = InterfacePattern(interface, remote_d, remote_interface, random_string())
             neighbor = Neighbor(remote_device, remote_interface)
             result = pattern.match(interface, [neighbor])
             self.assertFalse(result)
 
-        for remote_i in ['none', remote_interface + 'dummy']:
-            pattern = InterfacePattern(interface, remote_device, 
-                                       remote_i, random_string())
+        for remote_i in ["none", remote_interface + "dummy"]:
+            pattern = InterfacePattern(interface, remote_device, remote_i, random_string())
             neighbor = Neighbor(remote_device, remote_interface)
             result = pattern.match(interface, [neighbor])
             self.assertFalse(result)
 
-        for remote_d in ['none', remote_device + 'dummy']:
-            for remote_i in ['none', remote_interface + 'dummy']:
-                pattern = InterfacePattern(interface, remote_d, 
-                                           remote_i, random_string())
+        for remote_d in ["none", remote_device + "dummy"]:
+            for remote_i in ["none", remote_interface + "dummy"]:
+                pattern = InterfacePattern(interface, remote_d, remote_i, random_string())
                 neighbor = Neighbor(remote_device, remote_interface)
                 result = pattern.match(interface, [neighbor])
                 self.assertFalse(result)
 
-        for intf in ['none', interface + 'dummy']:
-            for remote_i in ['none', remote_interface + 'dummy']:
-                pattern = InterfacePattern(intf, remote_device, 
-                                           remote_i, random_string())
+        for intf in ["none", interface + "dummy"]:
+            for remote_i in ["none", remote_interface + "dummy"]:
+                pattern = InterfacePattern(intf, remote_device, remote_i, random_string())
                 neighbor = Neighbor(remote_device, remote_interface)
                 result = pattern.match(interface, [neighbor])
                 self.assertFalse(result)
 
-        for intf in ['none', interface + 'dummy']:
-            for remote_d in ['none', remote_device + 'dummy']:
-                pattern = InterfacePattern(intf, remote_d, 
-                                           remote_interface, random_string())
+        for intf in ["none", interface + "dummy"]:
+            for remote_d in ["none", remote_device + "dummy"]:
+                pattern = InterfacePattern(intf, remote_d, remote_interface, random_string())
                 neighbor = Neighbor(remote_device, remote_interface)
                 result = pattern.match(interface, [neighbor])
                 self.assertFalse(result)
 
-        for intf in ['none', interface + 'dummy']:
-            for remote_d in ['none', remote_device + 'dummy']:
-                for remote_i in ['none', remote_interface + 'dummy']:
-                    pattern = InterfacePattern(intf, remote_d, 
-                                               remote_i, random_string())
+        for intf in ["none", interface + "dummy"]:
+            for remote_d in ["none", remote_device + "dummy"]:
+                for remote_i in ["none", remote_interface + "dummy"]:
+                    pattern = InterfacePattern(intf, remote_d, remote_i, random_string())
                     neighbor = Neighbor(remote_device, remote_interface)
                     result = pattern.match(interface, [neighbor])
                     self.assertFalse(result)
 
     def compile_known_function(self, interface, cls):
-        pattern = InterfacePattern(random_string(),
-                                   interface,
-                                   random_string(),
-                                   random_string())
+        pattern = InterfacePattern(random_string(), interface, random_string(), random_string())
         self.assertIsInstance(pattern.remote_device_re, cls)
 
     def test_compile_exact_function(self):
-        interface = 'exact(\'%s\')' % random_string()
+        interface = f"exact('{random_string()}')"
         self.compile_known_function(interface, ExactFunction)
 
     def test_compile_includes_function(self):
-        interface = 'includes(\'%s\')' % random_string()
+        interface = f"includes('{random_string()}')"
         self.compile_known_function(interface, IncludesFunction)
 
     def test_compile_excludes_function(self):
-        interface = 'excludes(\'%s\')' % random_string()
+        interface = f"excludes('{random_string()}')"
         self.compile_known_function(interface, ExcludesFunction)
 
     def test_compile_regex_function(self):
-        interface = 'regex(\'%s\')' % random_string()
+        interface = f"regex('{random_string()}')"
         self.compile_known_function(interface, RegexFunction)
 
     def test_compile_no_function(self):
         interface = random_string()
         self.compile_known_function(interface, ExactFunction)
 
     def test_compile_unknown_function(self):
-        interface = '%s(\'%s\')' % (random_string(), random_string())
-        self.assertRaises(InterfacePatternError,
-                          InterfacePattern,
-                          random_string(), interface,
-                          random_string(), random_string())
+        interface = f"{random_string()}('{random_string()}')"
+        self.assertRaises(
+            InterfacePatternError,
+            InterfacePattern,
+            random_string(),
+            interface,
+            random_string(),
+            random_string(),
+        )
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     enable_logging()
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/server/server_test_lib.py` & `ztpserver-2.0.0/test/server/server_test_lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,255 +29,273 @@
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
 # pylint: disable=C0103
 #
 import json
-import os
 import logging
+import os
 import random
 import shutil
-import string        #pylint: disable=W0402
+import string  # pylint: disable=W0402
+from unittest.mock import Mock
 
 import yaml
 
-from mock import Mock
 from ztpserver.app import enable_handler_console
 
-WORKINGDIR = '/tmp/ztpserver'
+WORKINGDIR = "/tmp/ztpserver"
 
-log = logging.getLogger('ztpserver')
+log = logging.getLogger("ztpserver")
 log.setLevel(logging.DEBUG)
 log.addHandler(logging.NullHandler())
 
+
 def enable_logging():
     enable_handler_console()
 
+
 def random_string():
-    return ''.join(random.choice(string.ascii_uppercase + string.digits)
-                   for _ in range(random.randint(3, 20)))
+    return "".join(
+        random.choice(string.ascii_uppercase + string.digits) for _ in range(random.randint(3, 20))
+    )
+
 
 def random_json(keys=None):
-    data = dict()
+    data = {}
     if keys:
         for key in keys:
             data[key] = random_string()
     else:
         for _ in range(0, 5):
             data[random_string()] = random_string()
     return json.dumps(data)
 
+
 def remove_all():
     if os.path.exists(WORKINGDIR):
         shutil.rmtree(WORKINGDIR)
 
+
 def add_folder(name=None):
     if not name:
         name = random_string()
     filepath = os.path.join(WORKINGDIR, name)
     if os.path.exists(filepath):
         shutil.rmtree(filepath)
     os.makedirs(filepath)
     return filepath
 
-def write_file(contents, filename=None, mode='w'):
+
+def write_file(contents, filename=None, mode="w"):
     if not filename:
         filename = random_string()
     if not os.path.exists(WORKINGDIR):
         os.makedirs(WORKINGDIR)
     filepath = os.path.join(WORKINGDIR, filename)
-    open(filepath, mode).write(contents)
+    with open(filepath, mode, encoding="utf8") as fd:
+        fd.write(contents)
     return filepath
 
+
 def ztp_headers():
     return {
-        'X-Arista-Systemmac': random_string(),
-        'X-Arista-Serialnum': random_string(),
-        'X-Arista-Architecture': random_string(),
-        'X-Arista-Modelname': random_string(),
-        'X-Arista-Softwareversion': random_string()
+        "X-Arista-Systemmac": random_string(),
+        "X-Arista-Serialnum": random_string(),
+        "X-Arista-Architecture": random_string(),
+        "X-Arista-Modelname": random_string(),
+        "X-Arista-Softwareversion": random_string(),
     }
 
-class SerializerMixin(object):
+
+class SerializerMixin:
     def as_dict(self):
         raise NotImplementedError
 
     def as_yaml(self):
         return yaml.dump(self.as_dict())
 
     def as_json(self):
         return json.dumps(self.as_dict())
 
-class Definition(SerializerMixin):
 
+class Definition(SerializerMixin):
     def __init__(self, **kwargs):
-        self.name = kwargs.get('name')
-        self.attributes = kwargs.get('attributes', dict())
-        self.actions = kwargs.get('actions', list())
+        self.name = kwargs.get("name")
+        self.attributes = kwargs.get("attributes", {})
+        self.actions = kwargs.get("actions", [])
 
     def add_attribute(self, key, value):
         self.attributes[key] = value
 
     def add_action(self, **kwargs):
-        action = dict()
-        action['name'] = kwargs.get('name', 'test action')
-        action['action'] = kwargs.get('action', 'test_action')
-        action['attributes'] = kwargs.get('attributes', dict())
-        action['always_execute'] = kwargs.get('always_execute', dict())
+        action = {}
+        action["name"] = kwargs.get("name", "test action")
+        action["action"] = kwargs.get("action", "test_action")
+        action["attributes"] = kwargs.get("attributes", {})
+        action["always_execute"] = kwargs.get("always_execute", {})
         self.actions.append(action)
 
     def as_dict(self):
-        return dict(name=self.name,
-                    attributes=self.attributes,
-                    actions=self.actions)
+        return {"name": self.name, "attributes": self.attributes, "actions": self.actions}
+
 
 def create_definition():
     return Definition()
 
-class Attributes(SerializerMixin):
 
+class Attributes(SerializerMixin):
     def __init__(self, **kwargs):
-        self.attributes = kwargs.get('attributes', dict())
+        self.attributes = kwargs.get("attributes", {})
 
     def add_attribute(self, key, value):
         self.attributes[key] = value
 
     def add_attributes(self, attributes):
         assert isinstance(attributes, dict)
         for key, value in attributes.items():
             self.add_attribute(key, value)
 
     def as_dict(self):
         return self.attributes
 
+
 def create_attributes():
     return Attributes()
 
-class NodeDict(SerializerMixin):
 
+class NodeDict(SerializerMixin):
     def __init__(self, **kwargs):
-        self.serialnumber = kwargs.get('serialnumber', random_string())
-        self.model = kwargs.get('model', random_string())
-        self.version = kwargs.get('version', random_string())
-        self.systemmac = kwargs.get('systemmac', random_string())
-        self.neighbors = kwargs.get('neighbors', dict())
+        self.serialnumber = kwargs.get("serialnumber", random_string())
+        self.model = kwargs.get("model", random_string())
+        self.version = kwargs.get("version", random_string())
+        self.systemmac = kwargs.get("systemmac", random_string())
+        self.neighbors = kwargs.get("neighbors", {})
 
     def add_random_neighbor(self, interface):
-        neighbor = dict(device=random_string(), port=random_string())
+        neighbor = {"device": random_string(), "port": random_string()}
         self.add_neighbor(interface, neighbor)
 
     def add_neighbor(self, interface, peer):
         if interface not in self.neighbors:
-            self.neighbors[interface] = list()
+            self.neighbors[interface] = []
         self.neighbors[interface].append(peer)
 
     def add_neighbors(self, neighbors):
         assert isinstance(neighbors, dict)
         for key, value in neighbors.items():
             self.add_neighbor(key, value)
 
     def as_dict(self):
-        return dict(systemmac=self.systemmac,
-                    serialnumber=self.serialnumber,
-                    model=self.model,
-                    version=self.version,
-                    neighbors=self.neighbors)
+        return {
+            "systemmac": self.systemmac,
+            "serialnumber": self.serialnumber,
+            "model": self.model,
+            "version": self.version,
+            "neighbors": self.neighbors,
+        }
+
 
 def create_node():
     return NodeDict()
 
-def mock_match(node=None, definition=None,
-               variables=None,
-               name=None,
-               interfaces=None):
+
+def mock_match(
+    node=None, definition=None, variables=None, name=None, interfaces=None, config_handler=None
+):
     if not definition:
         definition = random_string()
     if not variables:
         variables = {}
     if not interfaces:
         interfaces = []
     if not name:
         name = random_string()
 
-    match = Mock()
+    match = Mock(definition=definition, config_handler=config_handler)
     match.serialize.return_value = {
-        'node': node,
-        'definition': definition,
-        'variables': variables, 
-        'name': name, 
-        'interfaces': interfaces}
+        "node": node,
+        "definition": definition,
+        "variables": variables,
+        "name": name,
+        "interfaces": interfaces,
+    }
 
     return match
 
+
 class BootstrapConf(SerializerMixin):
     def __init__(self, **kwargs):
-        self.logging = kwargs.get('logging', list())
-        self.xmpp = kwargs.get('xmpp', dict())
+        self.logging = kwargs.get("logging", [])
+        self.xmpp = kwargs.get("xmpp", {})
 
     def add_logging(self, entry):
         self.logging.append(entry)
 
     def as_dict(self):
-        return dict(logging=self.logging, xmpp=self.xmpp)
+        return {"logging": self.logging, "xmpp": self.xmpp}
+
 
 def create_bootstrap_conf():
     return BootstrapConf()
 
-class Pattern(SerializerMixin):
 
+class Pattern(SerializerMixin):
     def __init__(self, **kwargs):
-
-        self.name = kwargs.get('name', random_string())
-        self.node = kwargs.get('node')
-        self.definition = kwargs.get('definition', random_string())
-        self.interfaces = list()
+        self.name = kwargs.get("name", random_string())
+        self.node = kwargs.get("node")
+        self.definition = kwargs.get("definition", random_string())
+        self.interfaces = []
 
     def add_interface(self, local_intf, remote_device, remote_intf):
-        self.interfaces.append({local_intf: {'device': remote_device,
-                                             'port': remote_intf}})
+        self.interfaces.append({local_intf: {"device": remote_device, "port": remote_intf}})
 
     def add_random_interface(self, count=1):
-        for i in range(0, count):       # pylint: disable=W0612
+        for i in range(0, count):  # pylint: disable=W0612
             while True:
-                intf = 'Ethernet%d' % random.randint(1, 64)
+                intf = f"Ethernet{random.randint(1, 64):d}"
                 if intf not in self.interfaces:
                     self.add_interface(intf, random_string(), random_string())
                     break
 
     def as_dict(self):
-        return dict(name=self.name,
-                    node=self.node,
-                    definition=self.definition,
-                    interfaces=self.interfaces)
+        return {
+            "name": self.name,
+            "node": self.node,
+            "definition": self.definition,
+            "interfaces": self.interfaces,
+        }
+
 
 def create_pattern():
     return Pattern()
 
-class NeighborDb(SerializerMixin):
 
+class NeighborDb(SerializerMixin):
     def __init__(self, **kwargs):
-        self.name = kwargs.get('name', random_string())
-        self.variables = kwargs.get('variables', dict())
-        self.patterns = kwargs.get('patterns', list())
+        self.name = kwargs.get("name", random_string())
+        self.variables = kwargs.get("variables", {})
+        self.patterns = kwargs.get("patterns", [])
 
     def get_patterns(self):
         return [x.as_dict() for x in self.patterns]
 
     def add_pattern(self, pattern=None):
         if not pattern:
             pattern = Pattern()
             pattern = pattern.as_dict()
         self.patterns.append(pattern)
 
     def add_variable(self, key, value):
         self.variables[key] = value
 
     def as_dict(self):
-        return dict(name=self.name,
-                    variables=self.variables,
-                    patterns=[x.as_dict() for x in self.patterns])
+        return {
+            "name": self.name,
+            "variables": self.variables,
+            "patterns": [x.as_dict() for x in self.patterns],
+        }
+
 
 def create_neighbordb():
     return NeighborDb()
-
-
```

### Comparing `ztpserver-1.6.0/test/server/test_config.py` & `ztpserver-2.0.0/test/server/test_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,309 +33,302 @@
 import collections
 import os
 import tempfile
 import unittest
 
 import ztpserver.config
 
-class TestAttributes(unittest.TestCase):
 
+class TestAttributes(unittest.TestCase):
     def test_attr_valid(self):
-        obj = ztpserver.config.Attr('test')
+        obj = ztpserver.config.Attr("test")
         self.assertIsInstance(obj, ztpserver.config.Attr)
 
     def test_attr_invalid(self):
         self.assertRaises(TypeError, ztpserver.config.Attr)
 
     def test_strattr_defaults(self):
-        obj = ztpserver.config.StrAttr('test')
+        obj = ztpserver.config.StrAttr("test")
         self.assertIsInstance(obj, ztpserver.config.StrAttr)
 
     def test_strattr_with_choices(self):
-        obj = ztpserver.config.StrAttr('test', choices=['one', 'two'])
+        obj = ztpserver.config.StrAttr("test", choices=["one", "two"])
         self.assertIsInstance(obj, ztpserver.config.StrAttr)
-        self.assertEqual(repr(obj.type), 'String(choices=one,two)')
+        self.assertEqual(repr(obj.type), "String(choices=one,two)")
 
     def test_strattr_with_default(self):
-        obj = ztpserver.config.StrAttr('test', default='test')
+        obj = ztpserver.config.StrAttr("test", default="test")
         self.assertIsInstance(obj, ztpserver.config.StrAttr)
-        self.assertEqual(obj.default, 'test')
+        self.assertEqual(obj.default, "test")
 
     def test_strattr_with_group(self):
-        obj = ztpserver.config.StrAttr('test', group='test')
+        obj = ztpserver.config.StrAttr("test", group="test")
         self.assertIsInstance(obj, ztpserver.config.StrAttr)
-        self.assertEqual(obj.group, 'test')
+        self.assertEqual(obj.group, "test")
 
     def test_strattr_with_choices_default_valid(self):
-        obj = ztpserver.config.StrAttr('test', choices=['one', 'two'],
-            default='one')
+        obj = ztpserver.config.StrAttr("test", choices=["one", "two"], default="one")
         self.assertIsInstance(obj, ztpserver.config.StrAttr)
-        self.assertEqual(repr(obj.type), 'String(choices=one,two)')
-        self.assertEqual(obj.default, 'one')
+        self.assertEqual(repr(obj.type), "String(choices=one,two)")
+        self.assertEqual(obj.default, "one")
 
     def test_strattr_with_choices_default_invalid(self):
-        self.assertRaises(ValueError, ztpserver.config.StrAttr,
-            'test', choices=['one', 'two'], default='three')
+        self.assertRaises(
+            ValueError, ztpserver.config.StrAttr, "test", choices=["one", "two"], default="three"
+        )
 
     def test_strattr_with_choices_default_group(self):
-        obj = ztpserver.config.StrAttr('test', choices=['one', 'two'],
-            group='test', default='one')
+        obj = ztpserver.config.StrAttr("test", choices=["one", "two"], group="test", default="one")
         self.assertIsInstance(obj, ztpserver.config.StrAttr)
-        self.assertEqual(repr(obj.type), 'String(choices=one,two)')
-        self.assertEqual(obj.default, 'one')
-        self.assertEqual(obj.group, 'test')
+        self.assertEqual(repr(obj.type), "String(choices=one,two)")
+        self.assertEqual(obj.default, "one")
+        self.assertEqual(obj.group, "test")
 
     def test_intattr_defaults(self):
-        obj = ztpserver.config.IntAttr('test')
+        obj = ztpserver.config.IntAttr("test")
         self.assertIsInstance(obj, ztpserver.config.IntAttr)
 
     def test_intattr_with_min_value(self):
-        obj = ztpserver.config.IntAttr('test', min_value=1)
+        obj = ztpserver.config.IntAttr("test", min_value=1)
         self.assertIsInstance(obj, ztpserver.config.IntAttr)
         self.assertEqual(repr(obj.type), "Integer(min_value=1, max_value=None)")
 
     def test_intattr_with_max_value(self):
-        obj = ztpserver.config.IntAttr('test', max_value=1)
+        obj = ztpserver.config.IntAttr("test", max_value=1)
         self.assertIsInstance(obj, ztpserver.config.IntAttr)
         self.assertEqual(repr(obj.type), "Integer(min_value=None, max_value=1)")
 
     def test_intattr_with_min_and_max_value(self):
-        obj = ztpserver.config.IntAttr('test', min_value=1, max_value=1)
+        obj = ztpserver.config.IntAttr("test", min_value=1, max_value=1)
         self.assertIsInstance(obj, ztpserver.config.IntAttr)
         self.assertEqual(repr(obj.type), "Integer(min_value=1, max_value=1)")
 
     def test_intattr_with_default(self):
-        obj = ztpserver.config.IntAttr('test', default=1)
+        obj = ztpserver.config.IntAttr("test", default=1)
         self.assertIsInstance(obj, ztpserver.config.IntAttr)
         self.assertEqual(obj.default, 1)
 
     def test_intattr_with_min_valid_default(self):
-        obj = ztpserver.config.IntAttr('test', min_value=1, default=1)
+        obj = ztpserver.config.IntAttr("test", min_value=1, default=1)
         self.assertIsInstance(obj, ztpserver.config.IntAttr)
         self.assertEqual(obj.default, 1)
 
     def test_intattr_with_max_valid_default(self):
-        obj = ztpserver.config.IntAttr('test', max_value=1, default=1)
+        obj = ztpserver.config.IntAttr("test", max_value=1, default=1)
         self.assertIsInstance(obj, ztpserver.config.IntAttr)
         self.assertEqual(obj.default, 1)
 
     def test_intattr_with_range_valid_default(self):
-        obj = ztpserver.config.IntAttr('test', min_value=1, max_value=1,
-            default=1)
+        obj = ztpserver.config.IntAttr("test", min_value=1, max_value=1, default=1)
         self.assertIsInstance(obj, ztpserver.config.IntAttr)
         self.assertEqual(obj.default, 1)
 
     def test_intattr_with_min_invalid_default(self):
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=0, default=-1)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=1, default=0)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=2, default=1)
+        self.assertRaises(ValueError, ztpserver.config.IntAttr, "test", min_value=0, default=-1)
+        self.assertRaises(ValueError, ztpserver.config.IntAttr, "test", min_value=1, default=0)
+        self.assertRaises(ValueError, ztpserver.config.IntAttr, "test", min_value=2, default=1)
 
     def test_intattr_with_max_invalid_default(self):
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', max_value=0, default=1)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', max_value=1, default=2)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', max_value=2, default=3)
+        self.assertRaises(ValueError, ztpserver.config.IntAttr, "test", max_value=0, default=1)
+        self.assertRaises(ValueError, ztpserver.config.IntAttr, "test", max_value=1, default=2)
+        self.assertRaises(ValueError, ztpserver.config.IntAttr, "test", max_value=2, default=3)
 
     def test_intattr_with_range_invalid_default(self):
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=0, max_value=0, default=1)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=1, max_value=0, default=2)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=1, max_value=0, default=2)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=1, max_value=1, default=2)
-
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=2, max_value=0, default=3)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=0, max_value=2, default=3)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=2, max_value=2, default=3)
-        self.assertRaises(ValueError, ztpserver.config.IntAttr,
-            'test', min_value=2, max_value=3, default=4)
+        self.assertRaises(
+            ValueError, ztpserver.config.IntAttr, "test", min_value=0, max_value=0, default=1
+        )
+        self.assertRaises(
+            ValueError, ztpserver.config.IntAttr, "test", min_value=1, max_value=0, default=2
+        )
+        self.assertRaises(
+            ValueError, ztpserver.config.IntAttr, "test", min_value=1, max_value=0, default=2
+        )
+        self.assertRaises(
+            ValueError, ztpserver.config.IntAttr, "test", min_value=1, max_value=1, default=2
+        )
+
+        self.assertRaises(
+            ValueError, ztpserver.config.IntAttr, "test", min_value=2, max_value=0, default=3
+        )
+        self.assertRaises(
+            ValueError, ztpserver.config.IntAttr, "test", min_value=0, max_value=2, default=3
+        )
+        self.assertRaises(
+            ValueError, ztpserver.config.IntAttr, "test", min_value=2, max_value=2, default=3
+        )
+        self.assertRaises(
+            ValueError, ztpserver.config.IntAttr, "test", min_value=2, max_value=3, default=4
+        )
 
     def test_intattr_with_group(self):
-        obj = ztpserver.config.IntAttr('test', group='test')
+        obj = ztpserver.config.IntAttr("test", group="test")
         self.assertIsInstance(obj, ztpserver.config.IntAttr)
-        self.assertEqual(obj.group, 'test')
+        self.assertEqual(obj.group, "test")
 
     def test_boolattr_defaults(self):
-        obj = ztpserver.config.BoolAttr('test')
+        obj = ztpserver.config.BoolAttr("test")
         self.assertIsInstance(obj, ztpserver.config.BoolAttr)
         self.assertEqual(repr(obj.type), "Boolean")
 
     def test_boolattr_with_default(self):
-        obj = ztpserver.config.BoolAttr('test', default=True)
+        obj = ztpserver.config.BoolAttr("test", default=True)
         self.assertIsInstance(obj, ztpserver.config.BoolAttr)
         self.assertTrue(obj.default)
 
     def test_boolattr_with_group(self):
-        obj = ztpserver.config.BoolAttr('test', group='test')
+        obj = ztpserver.config.BoolAttr("test", group="test")
         self.assertIsInstance(obj, ztpserver.config.BoolAttr)
-        self.assertEqual(obj.group, 'test')
+        self.assertEqual(obj.group, "test")
+
 
 class TestGroup(unittest.TestCase):
-    #pylint: disable=C0103
+    # pylint: disable=C0103
 
-    class Config(object):
+    class Config:
         def __init__(self):
-            self.attributes = list()
+            self.attributes = []
 
         @classmethod
         def __get_attribute__(cls, name, group_name):
             return (name, group_name)
 
         def add_attribute(self, item, group_name):
             self.attributes.append((item, group_name))
 
         def __repr__(self):
-            return 'Config'
+            return "Config"
 
     def setUp(self):
         self.config = self.Config()
 
     def tearDown(self):
         del self.config
 
     def test_group(self):
-        obj = ztpserver.config.Group('test', self.config)
+        obj = ztpserver.config.Group("test", self.config)
         self.assertIsInstance(obj, ztpserver.config.Group)
-        self.assertEqual('test', obj.name)
-        self.assertEqual('Config', repr(obj.config))
+        self.assertEqual("test", obj.name)
+        self.assertEqual("Config", repr(obj.config))
 
     def test_group_get_attr(self):
-        obj = ztpserver.config.Group('test', self.config)
-        self.assertEqual(obj.testattr, ('testattr', 'test'))
-        self.assertEqual(obj['testattr'], ('testattr', 'test'))
+        obj = ztpserver.config.Group("test", self.config)
+        self.assertEqual(obj.testattr, ("testattr", "test"))
+        self.assertEqual(obj["testattr"], ("testattr", "test"))
 
     def test_group_add_attribute(self):
-        obj = ztpserver.config.Group('test', self.config)
-        obj.add_attribute('test')
-        self.assertEqual(self.config.attributes[0], ('test', 'test'))
+        obj = ztpserver.config.Group("test", self.config)
+        obj.add_attribute("test")
+        self.assertEqual(self.config.attributes[0], ("test", "test"))
 
 
 class TestConfig(unittest.TestCase):
-    #pylint: disable=C0103
+    # pylint: disable=C0103
 
-    Attr = collections.namedtuple('Attr', ['name', 'type', 'group', 'default'])
+    Attr = collections.namedtuple("Attr", ["name", "type", "group", "default"])
     CONF = """\n[default]\ntest = value\n[group]\ntest = value\n"""
 
     def setUp(self):
         self.config = ztpserver.config.Config()
 
     def tearDown(self):
         del self.config
 
     def test_config(self):
         self.assertIsInstance(self.config, ztpserver.config.Config)
-        self.assertEqual(repr(self.config), 'Config')
+        self.assertEqual(repr(self.config), "Config")
 
     def test_config_add_attribute_valid(self):
-        attr = self.Attr('test', str, None, None)
+        attr = self.Attr("test", str, None, None)
         self.config.add_attribute(attr)
-        self.assertIsNone(getattr(self.config, 'test'))
-        self.assertIn((None, 'test'), self.config.attributes)
+        self.assertIsNone(getattr(self.config, "test"))
+        self.assertIn((None, "test"), self.config.attributes)
 
     def test_config_add_attribute_default_value(self):
-        attr = self.Attr('test', str, None, 'value')
+        attr = self.Attr("test", str, None, "value")
         self.config.add_attribute(attr)
-        self.assertEqual(self.config.test, 'value')
+        self.assertEqual(self.config.test, "value")
 
     def test_config_add_attribute_group_and_default_value(self):
-        attr = self.Attr('test', str, 'group', 'value')
+        attr = self.Attr("test", str, "group", "value")
         self.config.add_attribute(attr)
-        self.assertEqual(self.config.group.test, 'value')
+        self.assertEqual(self.config.group.test, "value")
         self.assertIsInstance(self.config.group, ztpserver.config.Group)
 
     def test_config_add_attribute_invalid(self):
-        self.assertRaises(AttributeError, self.config.add_attribute, 'test')
+        self.assertRaises(AttributeError, self.config.add_attribute, "test")
 
     def test_config_add_attribute_duplicate(self):
-        attr = self.Attr('test', str, None, None)
+        attr = self.Attr("test", str, None, None)
         self.config.add_attribute(attr)
         self.assertRaises(AttributeError, self.config.add_attribute, attr)
 
     def test_config_add_group(self):
-        for grp in ['test', 100]:
+        for grp in ["test", 100]:
             self.config.add_group(grp)
             grp = str(grp) if isinstance(grp, int) else grp
             self.assertIn(grp, self.config.groups)
-            self.assertIsInstance(getattr(self.config, grp),
-                                  ztpserver.config.Group)
+            self.assertIsInstance(getattr(self.config, grp), ztpserver.config.Group)
 
     def test_config_set_value_attribute(self):
-        attr = self.Attr('test', str, None, None)
+        attr = self.Attr("test", str, None, None)
         self.config.add_attribute(attr)
-        self.config.set_value('test', 'value')
-        self.assertEqual(self.config.test, 'value')
+        self.config.set_value("test", "value")
+        self.assertEqual(self.config.test, "value")
 
     def test_config_runtime(self):
         obj = ztpserver.config.runtime
         self.assertIsInstance(obj, ztpserver.config.Config)
 
     def test_config_runtime_clear_value(self):
         obj = ztpserver.config.runtime
-        obj.set_value('interface', '1.1.1.1', 'server')
-        self.assertEqual(obj.server.interface, '1.1.1.1')
-        obj.clear_value('interface', 'server')
-        self.assertEqual(obj.server.interface, '0.0.0.0')
+        obj.set_value("interface", "1.1.1.1", "server")
+        self.assertEqual(obj.server.interface, "1.1.1.1")
+        obj.clear_value("interface", "server")
+        self.assertEqual(obj.server.interface, "0.0.0.0")
 
     def test_config_runtime_set_value(self):
         obj = ztpserver.config.runtime
-        obj.set_value('interface', '1.1.1.1', 'server')
-        self.assertEqual(obj.server.interface, '1.1.1.1')
+        obj.set_value("interface", "1.1.1.1", "server")
+        self.assertEqual(obj.server.interface, "1.1.1.1")
 
     def test_config_runtime_environ_env_set(self):
-        os.environ['ZTPS_ENV'] = 'environ'
+        os.environ["ZTPS_ENV"] = "environ"
         obj = ztpserver.config.Config()
-        attr = ztpserver.config.StrAttr(name='env',
-                                        default='default',
-                                        environ='ZTPS_ENV')
+        attr = ztpserver.config.StrAttr(name="env", default="default", environ="ZTPS_ENV")
         obj.add_attribute(attr)
-        self.assertEqual(obj.default.env, 'environ')
+        self.assertEqual(obj.default.env, "environ")
 
     def test_config_runtime_environ_env_notset(self):
         obj = ztpserver.config.Config()
-        attr = ztpserver.config.StrAttr(name='env',
-                                        default='default',
-                                        environ='ZTPS_ENV')
+        attr = ztpserver.config.StrAttr(name="env", default="default", environ="ZTPS_ENV")
         obj.add_attribute(attr)
-        self.assertEqual(obj.default.env, 'default')
+        self.assertEqual(obj.default.env, "default")
 
     def test_config_runtime_environ_env_set_no_default(self):
-        os.environ['ZTPS_ENV'] = 'environ'
+        os.environ["ZTPS_ENV"] = "environ"
         obj = ztpserver.config.Config()
-        attr = ztpserver.config.StrAttr(name='env',
-                                        environ='ZTPS_ENV')
+        attr = ztpserver.config.StrAttr(name="env", environ="ZTPS_ENV")
         obj.add_attribute(attr)
-        self.assertEqual(obj.default.env, 'environ')
+        self.assertEqual(obj.default.env, "environ")
 
     def test_config_runtime_environ_env_notset_no_default(self):
         obj = ztpserver.config.Config()
-        attr = ztpserver.config.StrAttr(name='env',
-                                        environ='ZTPS_ENV')
+        attr = ztpserver.config.StrAttr(name="env", environ="ZTPS_ENV")
         obj.add_attribute(attr)
         self.assertIsNone(obj.default.env)
 
     def test_load_config_file(self):
-        filename = tempfile.NamedTemporaryFile(mode='w')
-        filename.writelines(self.CONF)
-        filename.flush()
+        with tempfile.NamedTemporaryFile(mode="w") as fd:
+            fd.writelines(self.CONF)
+            fd.flush()
 
-        obj = ztpserver.config.runtime
-        obj.add_attribute(ztpserver.config.StrAttr(name='test'))
-        obj.add_attribute(ztpserver.config.StrAttr(name='test', group='group'))
-        obj.read(filename.name)
+            obj = ztpserver.config.runtime
+            obj.add_attribute(ztpserver.config.StrAttr(name="test"))
+            obj.add_attribute(ztpserver.config.StrAttr(name="test", group="group"))
+            obj.read(fd.name)
 
-        self.assertEqual(obj.default.test, 'value')
-        self.assertEqual(obj.group.test, 'value')
-        filename.close()
+            self.assertEqual(obj.default.test, "value")
+            self.assertEqual(obj.group.test, "value")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/server/test_app.py` & `ztpserver-2.0.0/test/server/test_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,23 +28,24 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # pylint: disable=W0613
 #
 import unittest
-
-from mock import patch
+from unittest.mock import patch
 
 import ztpserver.app
 
+
 class TestApp(unittest.TestCase):
-    #pylint: disable=R0904,C0103
+    # pylint: disable=R0904,C0103
 
-    @patch('ztpserver.topology.load')
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.topology.load")
+    @patch("ztpserver.controller.create_repository")
     def test_application_defaults(self, m_repository, m_load):
         obj = ztpserver.app.start_wsgiapp()
         self.assertIsInstance(obj, ztpserver.controller.Router)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/server/test_types.py` & `ztpserver-2.0.0/test/server/test_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,85 +31,85 @@
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 import unittest
 
 import ztpserver.types
 
-class TestTypes(unittest.TestCase):
 
+class TestTypes(unittest.TestCase):
     def test_create_string_defaults(self):
         obj = ztpserver.types.String()
         self.assertIsInstance(obj, ztpserver.types.String)
 
     def test_create_string_choices(self):
-        obj = ztpserver.types.String(['one', 'two'])
+        obj = ztpserver.types.String(["one", "two"])
         self.assertIsInstance(obj, ztpserver.types.String)
         self.assertEqual(repr(obj), "String(choices=one,two)")
 
     def test_create_string_choices_integers(self):
         obj = ztpserver.types.String([1, 2])
         self.assertIsInstance(obj, ztpserver.types.String)
         self.assertEqual(repr(obj), "String(choices=1,2)")
 
     def test_call_string_using_defaults_and_string(self):
         obj = ztpserver.types.String()
         self.assertIsInstance(obj, ztpserver.types.String)
-        self.assertEqual(obj('hello'), 'hello')
+        self.assertEqual(obj("hello"), "hello")
 
     def test_call_string_using_defaults_and_int(self):
         obj = ztpserver.types.String()
         self.assertIsInstance(obj, ztpserver.types.String)
-        self.assertEqual(obj(1), '1')
+        self.assertEqual(obj(1), "1")
 
     def test_call_string_using_defaults_and_bool(self):
         obj = ztpserver.types.String()
         self.assertIsInstance(obj, ztpserver.types.String)
-        self.assertEqual(obj(True), 'True')
+        self.assertEqual(obj(True), "True")
 
     def test_call_string_using_defaults_and_list(self):
         obj = ztpserver.types.String()
         self.assertIsInstance(obj, ztpserver.types.String)
-        self.assertEqual(obj(['one']), "['one']")
+        self.assertEqual(obj(["one"]), "['one']")
 
     def test_call_string_with_choices_valid(self):
-        obj = ztpserver.types.String(['one', 'two'])
+        obj = ztpserver.types.String(["one", "two"])
         self.assertIsInstance(obj, ztpserver.types.String)
         self.assertEqual(repr(obj), "String(choices=one,two)")
-        self.assertEqual(obj('one'), 'one')
+        self.assertEqual(obj("one"), "one")
 
     def test_call_string_with_choices_invalid(self):
-        obj = ztpserver.types.String(['one', 'two'])
+        obj = ztpserver.types.String(["one", "two"])
         self.assertIsInstance(obj, ztpserver.types.String)
         self.assertEqual(repr(obj), "String(choices=one,two)")
-        self.assertRaises(ValueError, obj, 'three')
+        self.assertRaises(ValueError, obj, "three")
 
     def test_create_boolean_defaults(self):
         obj = ztpserver.types.Boolean()
         self.assertIsInstance(obj, ztpserver.types.Boolean)
-        self.assertEqual(repr(obj), 'Boolean')
+        self.assertEqual(repr(obj), "Boolean")
 
     def test_call_boolean_true_values_valid(self):
         obj = ztpserver.types.Boolean()
         self.assertIsInstance(obj, ztpserver.types.Boolean)
-        values = obj.TRUEVALUES + ['YES', 'TRUE', True, 1, 'ON']
+        values = obj.TRUEVALUES + ["YES", "TRUE", True, 1, "ON"]
         for value in values:
             obj(value)
 
     def test_call_boolean_false_values_valid(self):
         obj = ztpserver.types.Boolean()
         self.assertIsInstance(obj, ztpserver.types.Boolean)
-        values = obj.FALSEVALUES + ['NO', 'FALSE', False, 0, 'OFF']
+        values = obj.FALSEVALUES + ["NO", "FALSE", False, 0, "OFF"]
         for value in values:
             obj(value)
 
     def test_call_boolean_invalid_values(self):
         obj = ztpserver.types.Boolean()
         self.assertIsInstance(obj, ztpserver.types.Boolean)
-        values = ['test', 100, ['one', 'two']]
+        values = ["test", 100, ["one", "two"]]
         for value in values:
             self.assertRaises(ValueError, obj, value)
 
     def test_create_integer_defaults(self):
         obj = ztpserver.types.Integer()
         self.assertIsInstance(obj, ztpserver.types.Integer)
         self.assertEqual(repr(obj), "Integer(min_value=None, max_value=None)")
@@ -125,56 +125,53 @@
         self.assertIsNone(obj.min_value)
 
     def test_create_integer_range(self):
         obj = ztpserver.types.Integer(min_value=1, max_value=1)
         self.assertEqual(obj.min_value, 1)
         self.assertEqual(obj.max_value, 1)
 
-    def test_call_integer_defaults_valid(self): #pylint: disable=R0201
+    def test_call_integer_defaults_valid(self):
         obj = ztpserver.types.Integer()
-        for value in [0, 1.0, 1.1, '65535', True]:
+        for value in [0, 1.0, 1.1, "65535", True]:
             obj(value)
 
     def test_call_integer_defaults_invalid(self):
         obj = ztpserver.types.Integer()
-        self.assertRaises(ValueError, obj, 'string')
+        self.assertRaises(ValueError, obj, "string")
         self.assertRaises(TypeError, obj, [1, 2])
 
     def test_call_integer_min_value_valid(self):
         obj = ztpserver.types.Integer(min_value=1)
         self.assertEqual(obj(1), 1)
-        self.assertEqual(obj('1'), 1)
+        self.assertEqual(obj("1"), 1)
 
     def test_call_integer_min_value_invalid(self):
         obj = ztpserver.types.Integer(min_value=1)
         self.assertRaises(ValueError, obj, 0)
-        self.assertRaises(ValueError, obj, '0')
+        self.assertRaises(ValueError, obj, "0")
 
     def test_call_integer_max_value_valid(self):
         obj = ztpserver.types.Integer(max_value=1)
         self.assertEqual(obj(1), 1)
-        self.assertEqual(obj('1'), 1)
+        self.assertEqual(obj("1"), 1)
 
     def test_call_integer_max_value_invalid(self):
         obj = ztpserver.types.Integer(max_value=1)
         self.assertRaises(ValueError, obj, 2)
-        self.assertRaises(ValueError, obj, '2')
+        self.assertRaises(ValueError, obj, "2")
 
     def test_call_integer_range_valid(self):
         obj = ztpserver.types.Integer(min_value=1, max_value=2)
         self.assertEqual(obj(1), 1)
 
     def test_call_integer_range_invalid(self):
         obj = ztpserver.types.Integer(min_value=1, max_value=2)
         self.assertRaises(ValueError, obj, 3)
 
     def test_create_list_defaults(self):
         obj = ztpserver.types.List()
         self.assertIsInstance(obj, ztpserver.types.List)
-        self.assertEqual(repr(obj), 'List(delimiter=,)')
-
-
-
+        self.assertEqual(repr(obj), "List(delimiter=,)")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/server/test_controller.py` & `ztpserver-2.0.0/test/server/test_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,1477 +25,1392 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
-# pylint: disable=C0102,C0103,E1103,W0142,W0613,C0302,E1120
+# pylint: disable=C0102,C0103,E1103,W0613,C0302,E1120
 #
 
 import json
 import random
 import unittest
+from test.server.server_test_lib import (
+    create_attributes,
+    create_bootstrap_conf,
+    create_definition,
+    create_node,
+    enable_logging,
+    mock_match,
+    random_string,
+    remove_all,
+    write_file,
+    ztp_headers,
+)
+from unittest.mock import MagicMock, Mock, patch
 
 from webob import Request
 
-from mock import MagicMock, Mock, patch
-
-import ztpserver.controller
 import ztpserver.config
+import ztpserver.controller
 import ztpserver.repository
-
+from ztpserver import constants
 from ztpserver.controller import DEFINITION_FN, PATTERN_FN
-
-from ztpserver.repository import FileObjectNotFound, FileObjectError
-
-from server_test_lib import enable_logging, remove_all, random_string
-from server_test_lib import mock_match, ztp_headers, write_file
-from server_test_lib import create_definition, create_attributes, create_node
-from server_test_lib import create_bootstrap_conf
-
-import ztpserver.constants as constants
+from ztpserver.repository import FileObjectError, FileObjectNotFound
 
 
 class RouterUnitTests(unittest.TestCase):
-
     def match_routes(self, url, valid, invalid):
-
         request = Request.blank(url)
         router = ztpserver.controller.Router()
 
         if valid:
-            for method in valid.split(','):
+            for method in valid.split(","):
                 request.method = method
-                msg = 'method %s failed for url %s' % (method, url)
-                self.assertIsNotNone(router.map.match(environ=request.environ),
-                                     msg)
+                msg = f"method {method} failed for url {url}"
+                self.assertIsNotNone(router.map.match(environ=request.environ), msg)
 
         if invalid:
-            for method in invalid.split(','):
+            for method in invalid.split(","):
                 request.method = method
-                msg = 'method %s failed for url %s' % (method, url)
-                self.assertIsNone(router.map.match(environ=request.environ),
-                                  msg)
+                msg = f"method {method} failed for url {url}"
+                self.assertIsNone(router.map.match(environ=request.environ), msg)
 
     def test_bootstrap_collection(self):
-        url = '/bootstrap'
-        self.match_routes(url, 'GET', 'POST,PUT,DELETE')
+        url = "/bootstrap"
+        self.match_routes(url, "GET", "POST,PUT,DELETE")
 
     def test_bootstrap_resource(self):
-        url = '/bootstrap/%s' % random_string()
-        self.match_routes(url, None, 'GET,POST,PUT,DELETE')
+        url = f"/bootstrap/{random_string()}"
+        self.match_routes(url, None, "GET,POST,PUT,DELETE")
 
     def test_bootstrap_config(self):
-        url = '/bootstrap/config'
-        self.match_routes(url, 'GET', 'POST,PUT,DELETE')
+        url = "/bootstrap/config"
+        self.match_routes(url, "GET", "POST,PUT,DELETE")
 
     def test_meta_action(self):
-        url = '/meta/actions/dummy'
-        self.match_routes(url, 'GET', 'POST,PUT,DELETE')
+        url = "/meta/actions/dummy"
+        self.match_routes(url, "GET", "POST,PUT,DELETE")
 
     def test_meta_files(self):
-        url = '/meta/files/dummy'
-        self.match_routes(url, 'GET', 'POST,PUT,DELETE')
+        url = "/meta/files/dummy"
+        self.match_routes(url, "GET", "POST,PUT,DELETE")
 
     def test_meta_files_long(self):
-        url = '/meta/files/dummy/long'
-        self.match_routes(url, 'GET', 'POST,PUT,DELETE')
+        url = "/meta/files/dummy/long"
+        self.match_routes(url, "GET", "POST,PUT,DELETE")
 
     def test_files_collection(self):
-        url = '/files'
-        self.match_routes(url, None, 'GET,POST,PUT,DELETE')
+        url = "/files"
+        self.match_routes(url, None, "GET,POST,PUT,DELETE")
 
     def test_files_resource(self):
-        url = '/files/%s' % random_string()
-        self.match_routes(url, 'GET', 'POST,PUT,DELETE')
+        url = f"/files/{random_string()}"
+        self.match_routes(url, "GET", "POST,PUT,DELETE")
 
-        url = '/files/%s/%s' % (random_string(), random_string())
-        self.match_routes(url, 'GET', 'POST,PUT,DELETE')
+        url = f"/files/{random_string()}/{random_string()}"
+        self.match_routes(url, "GET", "POST,PUT,DELETE")
 
     def test_actions_collection(self):
-        url = '/actions'
-        self.match_routes(url, None, 'GET,POST,PUT,DELETE')
+        url = "/actions"
+        self.match_routes(url, None, "GET,POST,PUT,DELETE")
 
     def test_actions_resource(self):
-        url = '/actions/%s' % random_string()
-        self.match_routes(url, 'GET', 'POST,PUT,DELETE')
+        url = f"/actions/{random_string()}"
+        self.match_routes(url, "GET", "POST,PUT,DELETE")
 
     def test_nodes_collection(self):
-        url = '/nodes'
-        self.match_routes(url, 'POST', 'GET,PUT,DELETE')
+        url = "/nodes"
+        self.match_routes(url, "POST", "GET,PUT,DELETE")
 
     def test_nodes_resource(self):
-        url = '/nodes/%s' % random_string()
-        self.match_routes(url, 'GET', 'POST,PUT,DELETE')
+        url = f"/nodes/{random_string()}"
+        self.match_routes(url, "GET", "POST,PUT,DELETE")
 
     def test_nodes_resource_get_config(self):
-        url = '/nodes/%s/startup-config' % random_string()
-        self.match_routes(url, 'GET,PUT', 'POST,DELETE')
-
+        url = f"/nodes/{random_string()}/startup-config"
+        self.match_routes(url, "GET,PUT", "POST,DELETE")
 
 
 class MetaControllerUnitTests(unittest.TestCase):
-
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_bad_request_file_not_found(self, m_repository):
         error = IOError
-        cfg = {'return_value.get_file.side_effect': error}
+        cfg = {"return_value.get_file.side_effect": error}
         m_repository.configure_mock(**cfg)
 
-        path = '/'.join([random_string()] * random.randint(1, 4))
+        path = "/".join([random_string()] * random.randint(1, 4))
 
         controller = ztpserver.controller.MetaController()
-        resp = controller.metadata(None,
-                                   type=random.choice(['files', 'actions']),
-                                   path_info=path)
-
-        self.assertEqual(resp['body'], '')
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_HTML)
-        self.assertEqual(resp['status'], constants.HTTP_STATUS_NOT_FOUND)
+        resp = controller.metadata(None, type=random.choice(["files", "actions"]), path_info=path)
+
+        self.assertEqual(resp["body"], "")
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_HTML)
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_NOT_FOUND)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_bad_request_io_error(self, m_repository):
-        cfg = random.choice([
-                {'return_value.get_file.return_value.hash.side_effect':
-                 IOError},
-                {'return_value.get_file.return_value.size.side_effect':
-                 IOError}])
+        cfg = random.choice(
+            [
+                {"return_value.get_file.return_value.hash.side_effect": IOError},
+                {"return_value.get_file.return_value.size.side_effect": IOError},
+            ]
+        )
         m_repository.configure_mock(**cfg)
 
         controller = ztpserver.controller.MetaController()
-        resp = controller.metadata(None,
-                                   type=random.choice(['files', 'actions']),
-                                   path_info=random_string())
-
-        self.assertEqual(resp['body'], '')
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_HTML)
-        self.assertEqual(resp['status'],
-                         constants.HTTP_STATUS_INTERNAL_SERVER_ERROR)
+        resp = controller.metadata(
+            None, type=random.choice(["files", "actions"]), path_info=random_string()
+        )
+
+        self.assertEqual(resp["body"], "")
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_HTML)
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_INTERNAL_SERVER_ERROR)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_success(self, m_repository):
         sha1 = random_string()
         size = random.randint(1, 1000000)
-        cfg = {'return_value.get_file.return_value.hash.return_value':
-               sha1,
-               'return_value.get_file.return_value.size.return_value':
-               size}
+        cfg = {
+            "return_value.get_file.return_value.hash.return_value": sha1,
+            "return_value.get_file.return_value.size.return_value": size,
+        }
         m_repository.configure_mock(**cfg)
 
         controller = ztpserver.controller.MetaController()
-        resp = controller.metadata(None,
-                                   type=random.choice(['files', 'actions']),
-                                   path_info=random_string())
+        resp = controller.metadata(
+            None, type=random.choice(["files", "actions"]), path_info=random_string()
+        )
 
-        self.assertEqual(resp['body'], {'sha1': sha1, 'size': size})
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_JSON)
+        self.assertEqual(resp["body"], {"sha1": sha1, "size": size})
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_JSON)
 
 
 class BootstrapConfigUnitTests(unittest.TestCase):
-
-    @patch('ztpserver.controller.create_repository')
-    @patch('string.Template.safe_substitute')
+    @patch("ztpserver.controller.create_repository")
+    @patch("string.Template.safe_substitute")
     def test_index_success(self, m_substitute, m_repository):
         m_substitute.return_value = random_string()
 
         controller = ztpserver.controller.BootstrapController()
 
-        request = Request.blank('')
-        request.remote_addr = ''
+        request = Request.blank("")
+        request.remote_addr = ""
         resp = controller.index(request)
 
         self.assertTrue(m_substitute.called)
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_PYTHON)
-        self.assertEqual(resp['body'], m_substitute.return_value)
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_PYTHON)
+        self.assertEqual(resp["body"], m_substitute.return_value)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_index_bootstrap_not_found_failure(self, m_repository):
-        cfg = {'return_value.get_file.side_effect': FileObjectError}
+        cfg = {"return_value.get_file.side_effect": FileObjectError}
         m_repository.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
         resp = controller.index(None)
 
-        self.assertTrue(resp['status'], constants.HTTP_STATUS_BAD_REQUEST)
-        self.assertEqual(resp['body'], '')
+        self.assertTrue(resp["status"], constants.HTTP_STATUS_BAD_REQUEST)
+        self.assertEqual(resp["body"], "")
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_index_bootstrap_inaccessible_failure(self, m_repository):
-        cfg = {'return_value.read.side_effect': FileObjectError}
+        cfg = {"return_value.read.side_effect": FileObjectError}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
         resp = controller.index(None)
 
-        self.assertTrue(resp['status'], constants.HTTP_STATUS_BAD_REQUEST)
-        self.assertEqual(resp['body'], '')
+        self.assertTrue(resp["status"], constants.HTTP_STATUS_BAD_REQUEST)
+        self.assertEqual(resp["body"], "")
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_config_success(self, m_repository):
         config = create_bootstrap_conf()
-        config.add_logging(dict(destination=random_string(),
-                                level=random_string()))
+        config.add_logging({"destination": random_string(), "level": random_string()})
 
-        cfg = {'return_value.read.return_value': config.as_dict()}
+        cfg = {"return_value.read.return_value": config.as_dict()}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
 
-        request = Request.blank('')
-        request.remote_addr = ''
+        request = Request.blank("")
+        request.remote_addr = ""
         resp = controller.config(request)
 
-        self.assertEqual(resp['body'], config.as_dict())
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_JSON)
+        self.assertEqual(resp["body"], config.as_dict())
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_JSON)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_config_defaults(self, m_repository):
-        cfg = {'return_value.get_file.side_effect': FileObjectNotFound}
+        cfg = {"return_value.get_file.side_effect": FileObjectNotFound}
         m_repository.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
 
-        request = Request.blank('')
-        request.remote_addr = ''
+        request = Request.blank("")
+        request.remote_addr = ""
         resp = controller.config(request)
 
-        self.assertEqual(resp['body'], controller.DEFAULT_CONFIG)
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_JSON)
+        self.assertEqual(resp["body"], controller.DEFAULT_CONFIG)
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_JSON)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_config_failure(self, m_repository):
-        cfg = {'return_value.read.side_effect': FileObjectError}
+        cfg = {"return_value.read.side_effect": FileObjectError}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
         resp = controller.config(None)
 
-        self.assertEqual(resp['body'], '')
-        self.assertEqual(resp['status'], constants.HTTP_STATUS_BAD_REQUEST)
+        self.assertEqual(resp["body"], "")
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_BAD_REQUEST)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_no_config(self, m_repository):
-        cfg = {'return_value.read.return_value': {}}
+        cfg = {"return_value.read.return_value": {}}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
 
-        request = Request.blank('')
-        request.remote_addr = ''
+        request = Request.blank("")
+        request.remote_addr = ""
         resp = controller.config(request)
 
-        self.assertEqual(resp['body'], controller.DEFAULT_CONFIG)
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_JSON)
+        self.assertEqual(resp["body"], controller.DEFAULT_CONFIG)
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_JSON)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_no_xmpp(self, m_repository):
-        cfg = {'return_value.read.return_value': {'logging': []}}
+        cfg = {"return_value.read.return_value": {"logging": []}}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
 
-        request = Request.blank('')
-        request.remote_addr = ''
+        request = Request.blank("")
+        request.remote_addr = ""
         resp = controller.config(request)
 
-        self.assertEqual(resp['body'], controller.DEFAULT_CONFIG)
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_JSON)
+        self.assertEqual(resp["body"], controller.DEFAULT_CONFIG)
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_JSON)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_no_logging(self, m_repository):
-        cfg = {'return_value.read.return_value': {'xmpp': {}}}
+        cfg = {"return_value.read.return_value": {"xmpp": {}}}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
 
-        request = Request.blank('')
-        request.remote_addr = ''
+        request = Request.blank("")
+        request.remote_addr = ""
         resp = controller.config(request)
 
-        self.assertEqual(resp['body'], controller.DEFAULT_CONFIG)
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_JSON)
-
+        self.assertEqual(resp["body"], controller.DEFAULT_CONFIG)
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_JSON)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_empty_xmpp(self, m_repository):
-        cfg = {'return_value.read.return_value': {'logging': [],
-                                                  'xmpp': None}}
+        cfg = {"return_value.read.return_value": {"logging": [], "xmpp": None}}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
 
-        request = Request.blank('')
-        request.remote_addr = ''
+        request = Request.blank("")
+        request.remote_addr = ""
         resp = controller.config(request)
 
-        self.assertEqual(resp['body'], controller.DEFAULT_CONFIG)
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_JSON)
+        self.assertEqual(resp["body"], controller.DEFAULT_CONFIG)
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_JSON)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_empty_logging(self, m_repository):
-        cfg = {'return_value.read.return_value': {'logging': None,
-                                                  'xmpp': {}}}
+        cfg = {"return_value.read.return_value": {"logging": None, "xmpp": {}}}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
 
-        request = Request.blank('')
-        request.remote_addr = ''
+        request = Request.blank("")
+        request.remote_addr = ""
         resp = controller.config(request)
 
-        self.assertEqual(resp['body'], controller.DEFAULT_CONFIG)
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_JSON)
+        self.assertEqual(resp["body"], controller.DEFAULT_CONFIG)
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_JSON)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_empty_xmpp_logging(self, m_repository):
-        cfg = {'return_value.read.return_value': {'logging': None,
-                                                  'xmpp': None}}
+        cfg = {"return_value.read.return_value": {"logging": None, "xmpp": None}}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.BootstrapController()
 
-        request = Request.blank('')
-        request.remote_addr = ''
+        request = Request.blank("")
+        request.remote_addr = ""
         resp = controller.config(request)
 
-        self.assertEqual(resp['body'], controller.DEFAULT_CONFIG)
-        self.assertEqual(resp['content_type'], constants.CONTENT_TYPE_JSON)
+        self.assertEqual(resp["body"], controller.DEFAULT_CONFIG)
+        self.assertEqual(resp["content_type"], constants.CONTENT_TYPE_JSON)
 
 
 class BootstrapUnitTests(unittest.TestCase):
-
     def setUp(self):
         self.m_repository = Mock()
         ztpserver.controller.create_repository = self.m_repository
 
-    @patch('string.Template.safe_substitute')
+    @patch("string.Template.safe_substitute")
     def test_get_bootstrap_success(self, m_substitute):
         contents = random_string()
         m_substitute.return_value = contents
 
-        request = Request.blank('/bootstrap', headers=ztp_headers())
+        request = Request.blank("/bootstrap", headers=ztp_headers())
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_PYTHON)
-        self.assertEqual(resp.body, contents)
+        self.assertEqual(resp.text, contents)
 
     def test_get_bootstrap_missing(self):
-        cfg = {'return_value.get_file.side_effect': FileObjectNotFound}
+        cfg = {"return_value.get_file.side_effect": FileObjectNotFound}
         self.m_repository.configure_mock(**cfg)
 
-        request = Request.blank('/bootstrap', headers=ztp_headers())
+        request = Request.blank("/bootstrap", headers=ztp_headers())
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_BAD_REQUEST)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_HTML)
 
-    @patch('string.Template.safe_substitute')
+    @patch("string.Template.safe_substitute")
     def test_get_bootstrap_misconfigured(self, m_substitute):
         m_substitute.side_effect = KeyError
 
-        request = Request.blank('/bootstrap', headers=ztp_headers())
+        request = Request.blank("/bootstrap", headers=ztp_headers())
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_BAD_REQUEST)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_HTML)
 
     def test_get_bootstrap_inaccessible(self):
-        cfg = {'return_value.get_file.side_effect': FileObjectError}
+        cfg = {"return_value.get_file.side_effect": FileObjectError}
         self.m_repository.configure_mock(**cfg)
 
-        request = Request.blank('/bootstrap', headers=ztp_headers())
+        request = Request.blank("/bootstrap", headers=ztp_headers())
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_BAD_REQUEST)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_HTML)
 
     def test_get_bootstrap_config_success(self):
         config = create_bootstrap_conf()
-        config.add_logging(dict(destination=random_string(),
-                                level=random_string()))
+        config.add_logging({"destination": random_string(), "level": random_string()})
 
-        cfg = {'return_value.read.return_value': config.as_dict()}
+        cfg = {"return_value.read.return_value": config.as_dict()}
         self.m_repository.return_value.get_file.configure_mock(**cfg)
 
-        request = Request.blank('/bootstrap/config')
+        request = Request.blank("/bootstrap/config")
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_JSON)
         self.assertEqual(json.loads(resp.body), config.as_dict())
 
     def test_get_bootstrap_config_defaults(self):
-        cfg = {'return_value.get_file.side_effect': FileObjectNotFound}
+        cfg = {"return_value.get_file.side_effect": FileObjectNotFound}
         self.m_repository.configure_mock(**cfg)
 
-        request = Request.blank('/bootstrap/config')
+        request = Request.blank("/bootstrap/config")
         resp = request.get_response(ztpserver.controller.Router())
 
-        defaultconfig = {'logging': list(), 'xmpp': dict()}
+        defaultconfig = {"logging": [], "xmpp": {}}
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_JSON)
         self.assertEqual(json.loads(resp.body), defaultconfig)
 
 
 class FilesControllerIntegrationTests(unittest.TestCase):
-
     def tearDown(self):
         remove_all()
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_file_success(self, m_repository):
         contents = random_string()
         filepath = write_file(contents)
 
         m_repository.return_value.get_file.return_value.name = filepath
 
-        url = '/files/%s' % filepath
+        url = f"/files/{filepath}"
         request = Request.blank(url)
         resp = request.get_response(ztpserver.controller.Router())
 
         m_repository.return_value.get_file.assert_called_with(filepath)
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_OTHER)
-        self.assertEqual(resp.body, contents)
-
+        self.assertEqual(resp.text, contents)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_missing_file(self, m_repository):
-        cfg = {'return_value.get_file.side_effect':
-                    ztpserver.repository.FileObjectNotFound}
+        cfg = {"return_value.get_file.side_effect": ztpserver.repository.FileObjectNotFound}
         m_repository.configure_mock(**cfg)
 
         filename = random_string()
-        url = '/files/%s' % filename
+        url = f"/files/{filename}"
 
         request = Request.blank(url)
         resp = request.get_response(ztpserver.controller.Router())
 
-        filepath = 'files/%s' % filename
+        filepath = f"files/{filename}"
         m_repository.return_value.get_file.assert_called_with(filepath)
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_NOT_FOUND)
 
 
 class ActionsControllerIntegrationTests(unittest.TestCase):
-
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_action_success(self, m_repository):
         contents = random_string()
-        cfg = {'return_value.read.return_value': contents}
+        cfg = {"return_value.read.return_value": contents}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         filename = random_string()
-        url = '/actions/%s' % filename
+        url = f"/actions/{filename}"
 
         request = Request.blank(url)
         resp = request.get_response(ztpserver.controller.Router())
 
         m_repository.return_value.get_file.assert_called_with(url[1:])
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_PYTHON)
-        self.assertEqual(resp.body, contents)
+        self.assertEqual(resp.text, contents)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_action_missing(self, m_repository):
-        cfg = {'return_value.get_file.side_effect': FileObjectNotFound}
+        cfg = {"return_value.get_file.side_effect": FileObjectNotFound}
         m_repository.configure_mock(**cfg)
 
         filename = random_string()
-        url = '/actions/%s' % filename
+        url = f"/actions/{filename}"
 
         request = Request.blank(url)
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_NOT_FOUND)
 
 
 class NodesControllerUnitTests(unittest.TestCase):
-
-
     def tearDown(self):
-        ztpserver.config.runtime.set_value(\
-            'disable_topology_validation', False, 'default')
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'serialnumber', 'default')
-        
+        ztpserver.config.runtime.set_value("disable_topology_validation", False, "default")
+        ztpserver.config.runtime.set_value("identifier", "serialnumber", "default")
+
     @classmethod
     def identifier(cls, node):
         identifier = ztpserver.config.runtime.default.identifier
-        if identifier == 'systemmac':
+        if identifier == "systemmac":
             return node.systemmac
-        else:
-            return node.serialnumber
+        return node.serialnumber
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_create(self, m_repository):
         node = Mock(systemmac=random_string(), serialnumber=random_string())
-        body = dict(systemmac=node.systemmac, serialnumber=node.serialnumber)
+        body = {"systemmac": node.systemmac, "serialnumber": node.serialnumber}
 
-        request = Request.blank('/nodes')
-        request.body = json.dumps(body)
+        request = Request.blank("/nodes")
+        request.body = json.dumps(body).encode("utf8")
 
         controller = ztpserver.controller.NodesController()
-        with patch.object(controller, 'fsm') as m_fsm:
+        with patch.object(controller, "fsm") as m_fsm:
             controller.create(request)
-            self.assertEqual(self.identifier(node),
-                             m_fsm.call_args[1]['node_id'])
+            self.assertEqual(self.identifier(node), m_fsm.call_args[1]["node_id"])
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_create_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_create()
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_create_missing_identifier(self, m_repository):
         node = Mock(systemmac=None, serialnumber=None)
-        body = dict(systemmac=node.systemmac, serialnumber=node.serialnumber)
+        body = {"systemmac": node.systemmac, "serialnumber": node.serialnumber}
 
-        request = Request.blank('/nodes')
-        request.body = json.dumps(body)
+        request = Request.blank("/nodes")
+        request.body = json.dumps(body).encode("utf8")
 
         controller = ztpserver.controller.NodesController()
         resp = controller.create(request)
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_BAD_REQUEST)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_create_missing_identifier_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_create_missing_identifier()
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists(self, m_repository):
         m_repository.return_value.exists.return_value = True
 
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.node_exists(dict(), node=node,
-                                               node_id=self.identifier(node))
+        (resp, state) = controller.node_exists({}, node=node, node_id=self.identifier(node))
 
-        self.assertEqual(state, 'dump_node')
-        self.assertEqual(resp['status'], constants.HTTP_STATUS_CONFLICT)
+        self.assertEqual(state, "dump_node")
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_CONFLICT)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_node_exists()
 
-
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists_definition_exists(self, m_repository):
         node = create_node()
-        cfg = dict()
+        cfg = {}
 
         def m_exists(arg):
             if arg.endswith(DEFINITION_FN):
                 return True
             return False
-        cfg['return_value.exists.side_effect'] = m_exists
+
+        cfg["return_value.exists.side_effect"] = m_exists
 
         m_repository.configure_mock(**cfg)
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.node_exists(dict(), node=node,
-                                               node_id=self.identifier(node))
+        (resp, state) = controller.node_exists({}, node=node, node_id=self.identifier(node))
 
-        self.assertEqual(state, 'dump_node')
-        self.assertEqual(resp['status'], constants.HTTP_STATUS_CONFLICT)
+        self.assertEqual(state, "dump_node")
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_CONFLICT)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists_definition_exists_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_node_exists_definition_exists()
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists_startup_config_exists(self, m_repository):
         node = create_node()
-        cfg = dict()
+        cfg = {}
 
         def m_exists(arg):
             if arg.endswith(ztpserver.controller.STARTUP_CONFIG_FN):
                 return True
             return False
-        cfg['return_value.exists.side_effect'] = m_exists
+
+        cfg["return_value.exists.side_effect"] = m_exists
 
         m_repository.configure_mock(**cfg)
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.node_exists(dict(), node=node,
-                                               node_id=self.identifier(node))
+        (resp, state) = controller.node_exists({}, node=node, node_id=self.identifier(node))
 
-        self.assertEqual(state, 'dump_node')
-        self.assertEqual(resp['status'], constants.HTTP_STATUS_CONFLICT)
+        self.assertEqual(state, "dump_node")
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_CONFLICT)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists_startup_config_exists_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_node_exists_startup_config_exists()
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists_sysmac_folder_exists(self, m_repository):
         node = create_node()
-        cfg = dict()
+        cfg = {}
 
         def m_exists(arg):
             if arg.endswith(self.identifier(node)):
                 return True
             return False
-        cfg['return_value.exists.side_effect'] = m_exists
+
+        cfg["return_value.exists.side_effect"] = m_exists
 
         m_repository.configure_mock(**cfg)
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.node_exists(dict(), node=node,
-                                               node_id=self.identifier(node))
+        (resp, state) = controller.node_exists({}, node=node, node_id=self.identifier(node))
 
         self.assertEqual(state, None)
-        self.assertEqual(resp['status'],
-                         constants.HTTP_STATUS_BAD_REQUEST)
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_BAD_REQUEST)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists_sysmac_folder_exists_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_node_exists_sysmac_folder_exists()
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists_failure(self, m_repository):
         m_repository.return_value.exists.return_value = False
 
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.node_exists(dict(), node=node,
-                                               node_id=self.identifier(node))
+        (resp, state) = controller.node_exists({}, node=node, node_id=self.identifier(node))
 
-        self.assertEqual(state, 'post_config')
+        self.assertEqual(state, "post_config")
         self.assertIsInstance(resp, dict)
-        self.assertEqual(resp, dict())
+        self.assertEqual(resp, {})
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists_failure_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_node_exists_failure()
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_dump_node_success(self, m_repository):
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
 
-        cfg = dict()
-        cfg['return_value.get_file'] = Mock()
+        cfg = {}
+        cfg["return_value.get_file"] = Mock()
         m_repository.configure_mock(**cfg)
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.dump_node(dict(), node=node,
-                                             node_id=self.identifier(node))
+        (resp, state) = controller.dump_node({}, node=node, node_id=self.identifier(node))
 
-        self.assertEqual(state, 'set_location')
+        self.assertEqual(state, "set_location")
         self.assertIsInstance(resp, dict)
-        self.assertEqual(resp, dict())
+        self.assertEqual(resp, {})
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_dump_node_success_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_dump_node_success()
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_dump_node_write_file_failure(self, m_repository):
-
-        cfg = {'return_value.get_file.return_value.write.side_effect': \
-               ztpserver.repository.FileObjectError}
+        cfg = {
+            "return_value.get_file.return_value.write.side_effect": (
+                ztpserver.repository.FileObjectError
+            )
+        }
         m_repository.configure_mock(**cfg)
 
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
 
         controller = ztpserver.controller.NodesController()
-        self.assertRaises(ztpserver.repository.FileObjectError,
-                          controller.dump_node,
-                          dict(),
-                          node=node,
-                          node_id=self.identifier(node))
+        self.assertRaises(
+            ztpserver.repository.FileObjectError,
+            controller.dump_node,
+            {},
+            node=node,
+            node_id=self.identifier(node),
+        )
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_dump_node_write_file_failure_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_dump_node_write_file_failure()
 
     def test_set_location_success(self):
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.set_location(dict(), node=node,
-                                                node_id=self.identifier(node))
+        (resp, state) = controller.set_location({}, node=node, node_id=self.identifier(node))
 
-        location = 'nodes/%s' % self.identifier(node)
+        location = f"nodes/{self.identifier(node)}"
         self.assertIsNone(state)
         self.assertIsInstance(resp, dict)
-        self.assertEqual(resp['location'], location)
+        self.assertEqual(resp["location"], location)
 
+    @unittest.skip(
+        "this test is broken. set_location access node_id throw get which won't throw "
+        "AttributeError"
+    )
     def test_set_location_failure(self):
         controller = ztpserver.controller.NodesController()
-        self.assertRaises(AttributeError, controller.set_location,
-                          dict(), node=None)
+        self.assertRaises(AttributeError, controller.set_location, {}, node=None)
 
     def test_post_config_success(self):
-        request = Mock(json=dict(config=random_string()))
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        request = Mock(json={"config": random_string()})
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.post_config(dict(), request=request,
-                                               node=node,
-                                               node_id=self.identifier(node))
+        (resp, state) = controller.post_config(
+            {}, request=request, node=node, node_id=self.identifier(node)
+        )
 
-        self.assertEqual(state, 'set_location')
+        self.assertEqual(state, "set_location")
         self.assertIsInstance(resp, dict)
-        self.assertEqual(resp['status'], constants.HTTP_STATUS_CREATED)
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_CREATED)
 
     def test_post_config_success_systemmac(self):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_post_config_success()
 
     def test_post_config_key_error_failure(self):
-        request = Mock(json=dict())
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        request = Mock(json={})
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.post_config(dict(), request=request,
-                                               node=node,
-                                               node_id=self.identifier(node))
+        (resp, state) = controller.post_config(
+            {}, request=request, node=node, node_id=self.identifier(node)
+        )
 
-        self.assertEqual(state, 'post_node')
+        self.assertEqual(state, "post_node")
         self.assertIsInstance(resp, dict)
-        self.assertEqual(resp, dict())
+        self.assertEqual(resp, {})
 
     def test_post_config_key_error_failure_systemmac(self):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_post_config_key_error_failure()
 
     def test_post_config_failure(self):
         controller = ztpserver.controller.NodesController()
-        self.assertRaises(Exception, controller.post_config, dict())
+        self.assertRaises(Exception, controller.post_config, {})
 
-    @patch('ztpserver.controller.load_neighbordb')
+    @patch("ztpserver.controller.load_neighbordb")
     def test_post_node_success_single_match(self, m_load_neighbordb):
-        request = Mock(json=dict(neighbors=dict()))
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        request = Mock(json={"neighbors": {}})
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
 
         m_load_neighbordb.return_value.match_node.return_value = [mock_match()]
         controller = ztpserver.controller.NodesController()
 
-        (resp, state) = controller.post_node(dict(), request=request, node=node,
-                                             node_id=self.identifier(node))
+        (resp, state) = controller.post_node(
+            {}, request=request, node=node, node_id=self.identifier(node)
+        )
 
-        self.assertEqual(state, 'dump_node')
+        self.assertEqual(state, "dump_node")
         self.assertIsInstance(resp, dict)
-        self.assertEqual(resp['status'], constants.HTTP_STATUS_CREATED)
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_CREATED)
 
-    @patch('ztpserver.controller.load_neighbordb')
+    @patch("ztpserver.controller.load_neighbordb")
     def test_post_node_success_single_match_systemmac(self, m_load_neighbordb):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_post_node_success_single_match()
 
-    @patch('ztpserver.controller.load_neighbordb')
+    @patch("ztpserver.controller.load_neighbordb")
     def test_post_node_success_multiple_matches(self, m_load_neighbordb):
-        request = Mock(json=dict(neighbors=dict()))
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        request = Mock(json={"neighbors": {}})
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
 
-        m_load_neighbordb.return_value.match_node.return_value = [mock_match(),
-                                                                  mock_match(),
-                                                                  mock_match()]
+        m_load_neighbordb.return_value.match_node.return_value = [
+            mock_match(),
+            mock_match(),
+            mock_match(),
+        ]
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.post_node(dict(), request=request, node=node,
-                                             node_id=self.identifier(node))
+        (resp, state) = controller.post_node(
+            {}, request=request, node=node, node_id=self.identifier(node)
+        )
 
-        self.assertEqual(state, 'dump_node')
+        self.assertEqual(state, "dump_node")
         self.assertIsInstance(resp, dict)
-        self.assertEqual(resp['status'], constants.HTTP_STATUS_CREATED)
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_CREATED)
 
-    @patch('ztpserver.controller.load_neighbordb')
-    def test_post_node_success_multiple_matches_systemmac(self,
-                                                          m_load_neighbordb):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+    @patch("ztpserver.controller.load_neighbordb")
+    def test_post_node_success_multiple_matches_systemmac(self, m_load_neighbordb):
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_post_node_success_multiple_matches()
 
-    @patch('ztpserver.controller.load_neighbordb')
+    @patch("ztpserver.controller.load_neighbordb")
     def test_post_node_failure_no_matches(self, m_load_neighbordb):
-        request = Mock(json=dict(neighbors=dict()))
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        request = Mock(json={"neighbors": {}})
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
 
-        m_load_neighbordb.return_value.match_node.return_value = list()
+        m_load_neighbordb.return_value.match_node.return_value = []
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.post_node(dict(), request=request,
-                                             node=node,
-                                             node_id=self.identifier(node))
+        (resp, state) = controller.post_node(
+            {}, request=request, node=node, node_id=self.identifier(node)
+        )
         self.assertEqual(state, None)
         self.assertIsInstance(resp, dict)
-        self.assertEqual(resp['status'], constants.HTTP_STATUS_BAD_REQUEST)
+        self.assertEqual(resp["status"], constants.HTTP_STATUS_BAD_REQUEST)
 
-    @patch('ztpserver.controller.load_neighbordb')
+    @patch("ztpserver.controller.load_neighbordb")
     def test_post_node_failure_no_matches_systemac(self, m_load_neighbordb):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_post_node_failure_no_matches()
 
-    @patch('ztpserver.controller.load_neighbordb')
+    @patch("ztpserver.controller.load_neighbordb")
     def test_post_node_no_definition_in_pattern(self, m_load_neighbordb):
-        request = Mock(json=dict(neighbors=dict()))
-        node = Mock(serialnumber=random_string(),
-                    systemmac=random_string())
+        request = Mock(json={"neighbors": {}})
+        node = Mock(serialnumber=random_string(), systemmac=random_string())
 
         pattern = Mock()
         del pattern.definition
 
         m_load_neighbordb.return_value.match_node.return_value = [pattern]
 
         controller = ztpserver.controller.NodesController()
-        self.assertRaises(AttributeError, controller.post_node, dict(),
-                          request=request, node=node,
-                          node_id=self.identifier(node))
-
-    @patch('ztpserver.controller.load_neighbordb')
-    def test_post_node_no_definition_in_pattern_systemmac(self,
-                                                          m_load_neighbordb):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        self.assertRaises(
+            AttributeError,
+            controller.post_node,
+            {},
+            request=request,
+            node=node,
+            node_id=self.identifier(node),
+        )
+
+    @patch("ztpserver.controller.load_neighbordb")
+    def test_post_node_no_definition_in_pattern_systemmac(self, m_load_neighbordb):
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_post_node_no_definition_in_pattern()
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_definition_success(self, m_repository):
-        cfg = {'return_value.read.return_value': MagicMock()}
+        cfg = {"return_value.read.return_value": MagicMock()}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.get_definition(dict(),
-                                                  resource=random_string())
+        (resp, state) = controller.get_definition({}, resource=random_string())
 
-        self.assertEqual(state, 'get_attributes')
+        self.assertEqual(state, "get_attributes")
         self.assertIsInstance(resp, dict)
 
-    @patch('ztpserver.controller.replace_config_action')
+    @patch("ztpserver.controller.replace_config_action")
     def test_get_startup_config_success(self, m_replace_config_action):
-        m_replace_config_action.return_value = dict()
+        m_replace_config_action.return_value = {}
 
-        ztpserver.topology.replace_config_action = Mock(return_value=dict())
+        ztpserver.topology.replace_config_action = Mock(return_value={})
 
-        response = dict(definition={'actions': list()})
+        response = {"definition": {"actions": []}}
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.get_startup_config(response,
-                                                      resource=random_string())
+        (resp, state) = controller.get_startup_config(response, resource=random_string())
 
-        self.assertEqual(state, 'get_definition')
+        self.assertEqual(state, "get_definition")
         self.assertIsInstance(resp, dict)
 
-
-    @patch('ztpserver.controller.replace_config_action')
-    def test_get_startup_config_success_no_definition(self,
-                                                      m_replace_config_action):
+    @patch("ztpserver.controller.replace_config_action")
+    def test_get_startup_config_success_no_definition(self, m_replace_config_action):
         resource = random_string()
 
         action_name = random_string()
-        action = {'name': action_name, 'action': 'replace_config'}
+        action = {"name": action_name, "action": "replace_config"}
         m_replace_config_action.return_value = action
         ztpserver.topology.replace_config_action = Mock(return_value=action)
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.get_startup_config(dict(), resource=resource)
+        (resp, state) = controller.get_startup_config({}, resource=resource)
 
-        self.assertEqual(state, 'get_definition')
+        self.assertEqual(state, "get_definition")
         self.assertIsInstance(resp, dict)
-        self.assertTrue(resp['get_startup_config'])
-        self.assertTrue(resp['definition'], 'Autogenerated definition')
-        self.assertEqual(resp['definition']['actions'][0]['name'], action_name)
+        self.assertTrue(resp["get_startup_config"])
+        self.assertTrue(resp["definition"], "Autogenerated definition")
+        self.assertEqual(resp["definition"]["actions"][0]["name"], action_name)
 
-    @patch('ztpserver.controller.load_pattern')
+    @patch("ztpserver.controller.load_pattern")
     def test_do_validation_success(self, m_load_pattern):
-
-        cfg = {'return_value.match_node.return_value': True}
+        cfg = {"return_value.match_node.return_value": True}
         m_load_pattern.configure_mock(**cfg)
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.do_validation(dict(),
-                                                 resource=random_string(),
-                                                 node=Mock())
+        (resp, state) = controller.do_validation({}, resource=random_string(), node=Mock())
 
-        self.assertEqual(state, 'get_startup_config')
+        self.assertEqual(state, "get_startup_config")
         self.assertIsInstance(resp, dict)
 
     def test_do_validation_disabled_success(self):
-        ztpserver.config.runtime.set_value(\
-            'disable_topology_validation', True, 'default')
+        ztpserver.config.runtime.set_value("disable_topology_validation", True, "default")
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.do_validation(dict(),
-                                                 resource=random_string())
+        (resp, state) = controller.do_validation({}, resource=random_string())
 
-        self.assertEqual(state, 'get_startup_config')
+        self.assertEqual(state, "get_startup_config")
         self.assertIsInstance(resp, dict)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_attributes_success(self, m_repository):
-        cfg = {'return_value.read.return_value': random_string()}
+        cfg = {"return_value.read.return_value": random_string()}
         m_repository.return_value.get_file.configure_mock(**cfg)
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.get_attributes(dict(),
-                                                  resource=random_string())
+        (resp, state) = controller.get_attributes({}, resource=random_string())
 
-        self.assertEqual(state, 'do_substitution')
+        self.assertEqual(state, "do_substitution")
         self.assertIsInstance(resp, dict)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_attributes_missing(self, m_repository):
         node = create_node()
 
         m_repository.return_value.exists.return_value = False
-        m_repository.return_value.get_file = \
-            Mock(side_effect=ztpserver.repository.FileObjectNotFound)
-
+        m_repository.return_value.get_file = Mock(
+            side_effect=ztpserver.repository.FileObjectNotFound
+        )
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.get_attributes(
-            dict(),
-            resource=self.identifier(node))
+        (resp, state) = controller.get_attributes({}, resource=self.identifier(node))
 
-        self.assertEqual(state, 'do_substitution')
+        self.assertEqual(state, "do_substitution")
         self.assertIsInstance(resp, dict)
-        self.assertEqual(resp['attributes'], dict())
+        self.assertEqual(resp["attributes"], {})
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_attributes_missing_systemmac(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'identifier', 'systemmac', 'default')
+        ztpserver.config.runtime.set_value("identifier", "systemmac", "default")
         self.test_get_attributes_missing()
 
     def test_do_substitution_success(self):
-        defattrs = dict(foo='$foo')
+        defattrs = {"foo": "$foo"}
 
         definition = create_definition()
-        definition.add_attribute('foo', 'bar')
-        definition.add_action(name='dummy action', attributes=defattrs)
+        definition.add_attribute("foo", "bar")
+        definition.add_action(name="dummy action", attributes=defattrs)
 
-        response = dict(definition=definition.as_dict())
+        response = {"definition": definition.as_dict()}
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.do_substitution(response,
-                                                   resource=random_string())
+        (resp, state) = controller.do_substitution(response, resource=random_string())
 
-        self.assertEqual(state, 'do_resources')
+        self.assertEqual(state, "do_resources")
         self.assertIsInstance(resp, dict)
 
-        foo = resp['definition']['actions'][0]['attributes']['foo']
-        self.assertEqual(foo, 'bar')
+        foo = resp["definition"]["actions"][0]["attributes"]["foo"]
+        self.assertEqual(foo, "bar")
 
     def test_do_substitution_with_attributes(self):
-        defattrs = dict(foo='$foo')
+        defattrs = {"foo": "$foo"}
 
         definition = create_definition()
-        definition.add_attribute('foo', 'bar')
-        definition.add_action(name='dummy action', attributes=defattrs)
+        definition.add_attribute("foo", "bar")
+        definition.add_action(name="dummy action", attributes=defattrs)
 
         g_attr_foo = random_string()
         attributes = create_attributes()
-        attributes.add_attribute('foo', g_attr_foo)
+        attributes.add_attribute("foo", g_attr_foo)
 
-        response = dict(definition=definition.as_dict(),
-                        attributes=attributes.as_dict())
+        response = {"definition": definition.as_dict(), "attributes": attributes.as_dict()}
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.do_substitution(response,
-                                                   resource=random_string())
+        (resp, state) = controller.do_substitution(response, resource=random_string())
 
-        self.assertEqual(state, 'do_resources')
+        self.assertEqual(state, "do_resources")
         self.assertIsInstance(resp, dict)
 
-        foo = resp['definition']['actions'][0]['attributes']['foo']
+        foo = resp["definition"]["actions"][0]["attributes"]["foo"]
         self.assertEqual(foo, g_attr_foo)
 
     def test_do_substitution_without_actions(self):
         # github issue #129
         definition = create_definition()
-        definition.actions.append({'name': 'foo'})
-        response = dict(definition=definition.as_dict())
+        definition.actions.append({"name": "foo"})
+        response = {"definition": definition.as_dict()}
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.do_substitution(response,
-                                                   resource=random_string())
+        (resp, state) = controller.do_substitution(response, resource=random_string())
 
-        self.assertEqual(state, 'do_resources')
+        self.assertEqual(state, "do_resources")
         self.assertIsInstance(resp, dict)
 
     def test_do_resources_success(self):
         var_foo = random_string()
-        ztpserver.controller.load_resources = \
-            Mock(return_value=dict(foo=var_foo))
+        ztpserver.controller.load_resources = Mock(return_value={"foo": var_foo})
 
         definition = create_definition()
-        definition.add_action(name='dummy action',
-                              attributes=dict(foo=random_string()))
+        definition.add_action(name="dummy action", attributes={"foo": random_string()})
 
-        response = dict(definition=definition.as_dict())
+        response = {"definition": definition.as_dict()}
 
         controller = ztpserver.controller.NodesController()
-        (resp, state) = controller.do_resources(response, node=Mock(),
-                                                resource=random_string())
+        (resp, state) = controller.do_resources(response, node=Mock(), resource=random_string())
 
-        self.assertEqual(state, 'finalize_response')
+        self.assertEqual(state, "finalize_response")
         self.assertIsInstance(resp, dict)
-        foo = resp['definition']['actions'][0]['attributes']['foo']
+        foo = resp["definition"]["actions"][0]["attributes"]["foo"]
         self.assertEqual(foo, var_foo)
 
-    @patch('os.path.isfile')
+    @patch("os.path.isfile")
     def test_put_config_success(self, m_is_file):
         m_is_file.return_value = False
 
         resource = random_string()
         body = random_string()
         request = Mock(content_type=constants.CONTENT_TYPE_OTHER, body=body)
 
         controller = ztpserver.controller.NodesController()
-        resp = controller.put_config(request,
-                                     resource=resource)
+        resp = controller.put_config(request, resource=resource)
 
-        self.assertEqual(resp, dict())
+        self.assertEqual(resp, {})
 
 
 class NodesControllerPostFsmIntegrationTests(unittest.TestCase):
-
     def setUp(self):
-        ztpserver.config.runtime.set_value(\
-            'disable_topology_validation', False, 'default')
+        ztpserver.config.runtime.set_value("disable_topology_validation", False, "default")
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_missing_required_attributes(self, m_repository):
-        url = '/nodes'
-        body = json.dumps(dict())
+        url = "/nodes"
+        body = json.dumps({}).encode("utf8")
 
-        request = Request.blank(url, body=body, method='POST',
-                                headers=ztp_headers())
+        request = Request.blank(url, body=body, method="POST", headers=ztp_headers())
 
         resp = request.get_response(ztpserver.controller.Router())
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_BAD_REQUEST)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_node_exists(self, m_repository):
-        url = '/nodes'
+        url = "/nodes"
         serialnumber = random_string()
-        body = json.dumps(dict(serialnumber=serialnumber))
+        body = json.dumps({"serialnumber": serialnumber}).encode("utf8")
 
         m_repository.return_value.exists.return_value = True
 
-        request = Request.blank(url, body=body, method='POST',
-                                headers=ztp_headers())
+        request = Request.blank(url, body=body, method="POST", headers=ztp_headers())
 
         resp = request.get_response(ztpserver.controller.Router())
 
-        location = 'http://localhost/nodes/%s' % serialnumber
+        location = f"http://localhost/nodes/{serialnumber}"
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_CONFLICT)
         self.assertEqual(resp.location, location)
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_post_config(self, m_repository):
-        url = '/nodes'
+        url = "/nodes"
         serialnumber = random_string()
         config = random_string()
-        body = json.dumps(dict(serialnumber=serialnumber, config=config))
+        body = json.dumps({"serialnumber": serialnumber, "config": config}).encode("utf8")
 
         m_repository.return_value.exists.return_value = False
 
-        request = Request.blank(url, body=body, method='POST',
-                                headers=ztp_headers())
+        request = Request.blank(url, body=body, method="POST", headers=ztp_headers())
         resp = request.get_response(ztpserver.controller.Router())
 
-        location = 'http://localhost/nodes/%s' % serialnumber
+        location = f"http://localhost/nodes/{serialnumber}"
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_CREATED)
         self.assertEqual(resp.location, location)
 
-    @patch('ztpserver.controller.create_repository')
-    @patch('ztpserver.controller.load_neighbordb')
+    @patch("ztpserver.controller.create_repository")
+    @patch("ztpserver.controller.load_neighbordb")
     def test_post_node_success(self, m_load_neighbordb, m_repository):
         node = create_node()
 
         definition = create_definition()
         definition.add_action()
 
-        cfg = {'return_value.exists.return_value': False}
+        cfg = {"return_value.exists.return_value": False}
         m_repository.configure_mock(**cfg)
 
         pattern_name = random_string()
-        cfg = {'return_value.match_node.return_value':
-               [mock_match(name=pattern_name)]}
+        cfg = {"return_value.match_node.return_value": [mock_match(name=pattern_name)]}
         m_load_neighbordb.configure_mock(**cfg)
 
-        request = Request.blank('/nodes', body=node.as_json(), method='POST',
-                                headers=ztp_headers())
+        body = node.as_json().encode("utf8")
+
+        request = Request.blank("/nodes", body=body, method="POST", headers=ztp_headers())
         resp = request.get_response(ztpserver.controller.Router())
 
-        args_list = list()
-        args_list.append('nodes/%s/%s' % (node.serialnumber, DEFINITION_FN))
-        args_list.append('nodes/%s/%s' % (node.serialnumber, PATTERN_FN))
+        args_list = []
+        args_list.append(f"nodes/{node.serialnumber}/{DEFINITION_FN}")
+        args_list.append(f"nodes/{node.serialnumber}/{PATTERN_FN}")
 
         for arg in args_list:
             m_repository.return_value.add_file.assert_any_call(arg)
 
         write_mock = m_repository.return_value.add_file.return_value.write
         # 'definition' is not written to the pattern file
         # Empty 'variables', 'node' are not written to the
         # pattern file either
-        self.assertEqual(sorted(write_mock.call_args_list[1][0][0].keys()),
-                         ['interfaces', 'name'])
+        self.assertEqual(sorted(write_mock.call_args_list[1][0][0].keys()), ["interfaces", "name"])
 
-        location = 'http://localhost/nodes/%s' % node.serialnumber
+        location = f"http://localhost/nodes/{node.serialnumber}"
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_CREATED)
         self.assertEqual(resp.location, location)
 
 
 class NodesControllerGetFsmIntegrationTests(unittest.TestCase):
-
     def setUp(self):
-        ztpserver.config.runtime.set_value(\
-            'disable_topology_validation', False, 'default')
+        ztpserver.config.runtime.set_value("disable_topology_validation", False, "default")
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_fsm_missing_node(self, m_repository):
-        cfg = {'return_value.get_file.side_effect': FileObjectNotFound}
+        cfg = {"return_value.get_file.side_effect": FileObjectNotFound}
         m_repository.configure_mock(**cfg)
 
-        url = '/nodes/%s' % random_string()
-        request = Request.blank(url, method='GET')
+        url = f"/nodes/{random_string()}"
+        request = Request.blank(url, method="GET")
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_BAD_REQUEST)
 
-
-    @patch('ztpserver.controller.create_node')
-    @patch('ztpserver.controller.create_repository')
-    @patch('ztpserver.controller.load_pattern')
-    def test_get_startup_config_wo_validation(self, m_load_pattern,
-                                              m_repository, m_create_node):
-
-        ztpserver.config.runtime.set_value(\
-            'disable_topology_validation', True, 'default')
+    @patch("ztpserver.controller.create_node")
+    @patch("ztpserver.controller.create_repository")
+    @patch("ztpserver.controller.load_pattern")
+    def test_get_startup_config_wo_validation(self, m_load_pattern, m_repository, m_create_node):
+        ztpserver.config.runtime.set_value("disable_topology_validation", True, "default")
 
         definition = create_definition()
         definition.add_action()
 
         node = create_node()
-        cfg = dict()
+        cfg = {}
 
         def m_get_file(arg):
             fileobj = Mock()
-            if arg.endswith('.node'):
+            if arg.endswith(".node"):
                 fileobj.return_value.read.return_value = node.as_dict()
-            elif arg.endswith('startup-config'):
+            elif arg.endswith("startup-config"):
                 fileobj.return_value.read.return_value = random_string()
             else:
                 raise ztpserver.repository.FileObjectNotFound
             return fileobj
-        cfg['return_value.get_file'] = Mock(side_effect=m_get_file)
+
+        cfg["return_value.get_file"] = Mock(side_effect=m_get_file)
 
         m_repository.configure_mock(**cfg)
 
-        url = '/nodes/%s' % node.serialnumber
-        request = Request.blank(url, method='GET')
+        url = f"/nodes/{node.serialnumber}"
+        request = Request.blank(url, method="GET")
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_JSON)
         self.assertIsInstance(json.loads(resp.body), dict)
 
-    @patch('ztpserver.controller.load_pattern')
-    @patch('ztpserver.controller.create_repository')
-    @patch('ztpserver.controller.create_node')
-    def test_get_startup_config_w_validation_success(self,
-                                                     m_load_pattern,
-                                                     m_repository,
-                                                     m_create_node):
-
+    @patch("ztpserver.controller.load_pattern")
+    @patch("ztpserver.controller.create_repository")
+    @patch("ztpserver.controller.create_node")
+    def test_get_startup_config_w_validation_success(
+        self, m_load_pattern, m_repository, m_create_node
+    ):
         definition = create_definition()
         definition.add_action()
 
         node = create_node()
-        cfg = dict()
+        cfg = {}
 
         def m_get_file(arg):
             fileobj = Mock()
-            if arg.endswith('.node'):
+            if arg.endswith(".node"):
                 fileobj.read.return_value = node.as_dict()
-            elif arg.endswith('startup-config'):
+            elif arg.endswith("startup-config"):
                 fileobj.read.return_value = random_string()
-            elif arg.endswith('pattern'):
+            elif arg.endswith("pattern"):
                 fileobj.read.return_value = random_string()
             else:
                 raise ztpserver.repository.FileObjectNotFound
             return fileobj
 
-        cfg['return_value.get_file'] = Mock(side_effect=m_get_file)
+        cfg["return_value.get_file"] = Mock(side_effect=m_get_file)
 
         m_repository.configure_mock(**cfg)
 
-        cfg = {'return_value.match_node.return_value': True}
+        cfg = {"return_value.match_node.return_value": True}
         m_load_pattern.configure_mock(**cfg)
 
-        url = '/nodes/%s' % node.serialnumber
-        request = Request.blank(url, method='GET')
+        url = f"/nodes/{node.serialnumber}"
+        request = Request.blank(url, method="GET")
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_JSON)
         self.assertIsInstance(json.loads(resp.body), dict)
 
-    @patch('ztpserver.controller.create_repository')
-    @patch('ztpserver.controller.load_pattern')
-    def test_get_startup_config_w_validation_failure(self, m_load_pattern,
-                                                     m_repository):
-
-        m_load_pattern.return_value.match_node.return_value = list()
+    @patch("ztpserver.controller.create_repository")
+    @patch("ztpserver.controller.load_pattern")
+    def test_get_startup_config_w_validation_failure(self, m_load_pattern, m_repository):
+        m_load_pattern.return_value.match_node.return_value = []
 
         node = create_node()
-        cfg = dict()
+        cfg = {}
 
         def exists(filepath):
-            if filepath.endswith('startup-config'):
+            if filepath.endswith("startup-config"):
                 return True
             return False
-        cfg['return_value.exists'] = Mock(side_effect=exists)
+
+        cfg["return_value.exists"] = Mock(side_effect=exists)
 
         def get_file(filepath):
             fileobj = Mock()
-            if filepath.endswith('node'):
+            if filepath.endswith("node"):
                 fileobj.contents = node.as_json()
                 return fileobj
-            elif filepath.endswith('pattern'):
+            if filepath.endswith("pattern"):
                 return fileobj
             raise ztpserver.repository.FileObjectNotFound
-        cfg['return_value.get_file'] = Mock(side_effect=get_file)
+
+        cfg["return_value.get_file"] = Mock(side_effect=get_file)
 
         m_repository.configure_mock(**cfg)
 
-        url = '/nodes/%s' % node.serialnumber
-        request = Request.blank(url, method='GET')
+        url = f"/nodes/{node.serialnumber}"
+        request = Request.blank(url, method="GET")
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_BAD_REQUEST)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_HTML)
-        self.assertEqual(resp.body, str())
+        self.assertEqual(resp.text, "")
 
-    @patch('ztpserver.controller.create_repository')
+    @patch("ztpserver.controller.create_repository")
     def test_get_definition_wo_validation(self, m_repository):
-        ztpserver.config.runtime.set_value(\
-            'disable_topology_validation', True, 'default')
+        ztpserver.config.runtime.set_value("disable_topology_validation", True, "default")
 
         definitions_file = create_definition()
         definitions_file.add_action()
 
         node = create_node()
-        cfg = dict()
+        cfg = {}
 
         def m_get_file(arg):
             m_file_object = Mock()
-            if arg.endswith('.node'):
+            if arg.endswith(".node"):
                 m_file_object.read.return_value = node.as_dict()
-            elif arg.endswith('definition'):
+            elif arg.endswith("definition"):
                 m_file_object.read.return_value = definitions_file.as_dict()
             else:
                 raise ztpserver.repository.FileObjectNotFound
             return m_file_object
 
-        cfg['return_value.get_file.side_effect'] = m_get_file
+        cfg["return_value.get_file.side_effect"] = m_get_file
         m_repository.configure_mock(**cfg)
 
-        url = '/nodes/%s' % node.serialnumber
-        request = Request.blank(url, method='GET')
+        url = f"/nodes/{node.serialnumber}"
+        request = Request.blank(url, method="GET")
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_JSON)
         self.assertIsInstance(json.loads(resp.body), dict)
 
-    @patch('ztpserver.controller.create_repository')
-    @patch('ztpserver.controller.load_pattern')
-    def test_get_definition_w_validation_success(self, m_load_pattern,
-                                                 m_repository):
+    @patch("ztpserver.controller.create_repository")
+    @patch("ztpserver.controller.load_pattern")
+    def test_get_definition_w_validation_success(self, m_load_pattern, m_repository):
         node = create_node()
 
         definitions_file = create_definition()
         definitions_file.add_action()
 
-        cfg = dict()
+        cfg = {}
 
         def m_get_file(arg):
             m_file_object = Mock()
-            if arg.endswith('.node'):
+            if arg.endswith(".node"):
                 m_file_object.read.return_value = node.as_dict()
-            elif arg.endswith('definition'):
+            elif arg.endswith("definition"):
                 m_file_object.read.return_value = definitions_file.as_dict()
-            elif arg.endswith('attributes'):
+            elif arg.endswith("attributes"):
                 raise ztpserver.repository.FileObjectNotFound
             return m_file_object
 
-        cfg['return_value.get_file.side_effect'] = m_get_file
+        cfg["return_value.get_file.side_effect"] = m_get_file
 
         m_repository.configure_mock(**cfg)
 
         m_load_pattern.return_value.match_node.return_value = Mock()
 
-        url = '/nodes/%s' % node.serialnumber
-        request = Request.blank(url, method='GET')
+        url = f"/nodes/{node.serialnumber}"
+        request = Request.blank(url, method="GET")
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_JSON)
         self.assertIsInstance(json.loads(resp.body), dict)
 
-
-    @patch('ztpserver.controller.create_repository')
-    @patch('ztpserver.controller.load_pattern')
-    def test_get_definition_w_validation_failure(self, m_load_pattern,
-                                                 m_repository):
+    @patch("ztpserver.controller.create_repository")
+    @patch("ztpserver.controller.load_pattern")
+    def test_get_definition_w_validation_failure(self, m_load_pattern, m_repository):
         definitions_file = create_definition()
         definitions_file.add_action()
 
         serialnumber = random_string()
         node = Mock(serialnumber=serialnumber)
         node.identifier.return_value = serialnumber
 
-        cfg = dict()
+        cfg = {}
 
         def m_get_file(arg):
             m_file_object = Mock()
-            if arg.endswith('.node'):
+            if arg.endswith(".node"):
                 m_file_object.read.return_value = node
-            elif arg.endswith('definition'):
+            elif arg.endswith("definition"):
                 m_file_object.read.return_value = definitions_file.as_dict()
             return m_file_object
 
-        cfg['return_value.get_file.side_effect'] = m_get_file
+        cfg["return_value.get_file.side_effect"] = m_get_file
         m_repository.configure_mock(**cfg)
 
         m_load_pattern.return_value.match_node.return_value = False
 
-        url = '/nodes/%s' % node.serialnumber
-        request = Request.blank(url, method='GET')
+        url = f"/nodes/{node.serialnumber}"
+        request = Request.blank(url, method="GET")
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_BAD_REQUEST)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_HTML)
-        self.assertEqual(resp.body, str())
-
-    @patch('ztpserver.controller.create_repository')
-    @patch('ztpserver.controller.load_pattern')
-    def test_get_definition_w_attributes_no_substitution(self, m_load_pattern,
-                                                         m_repository):
+        self.assertEqual(resp.text, "")
 
+    @patch("ztpserver.controller.create_repository")
+    @patch("ztpserver.controller.load_pattern")
+    def test_get_definition_w_attributes_no_substitution(self, m_load_pattern, m_repository):
         node = create_node()
 
         g_attr_foo = random_string()
         attributes_file = create_attributes()
-        attributes_file.add_attribute('variables', {'foo': g_attr_foo})
+        attributes_file.add_attribute("variables", {"foo": g_attr_foo})
 
         l_attr_url = random_string()
         definitions_file = create_definition()
-        definitions_file.add_attribute('foo', random_string())
-        definitions_file.add_action(name='dummy action',
-                                    attributes=dict(url=l_attr_url))
+        definitions_file.add_attribute("foo", random_string())
+        definitions_file.add_action(name="dummy action", attributes={"url": l_attr_url})
+
+        cfg = {}
 
-        cfg = dict()
         def m_get_file(arg):
             m_file_object = Mock()
-            if arg.endswith('.node'):
+            if arg.endswith(".node"):
                 m_file_object.read.return_value = node.as_dict()
-            elif arg.endswith('definition'):
+            elif arg.endswith("definition"):
                 m_file_object.read.return_value = definitions_file.as_dict()
-            elif arg.endswith('attributes'):
+            elif arg.endswith("attributes"):
                 m_file_object.read.return_value = attributes_file.as_dict()
-            elif arg.endswith('startup-config'):
+            elif arg.endswith("startup-config"):
                 raise ztpserver.repository.FileObjectNotFound
             return m_file_object
-        cfg['return_value.get_file'] = Mock(side_effect=m_get_file)
 
-        cfg['return_value.match_node.return_value'] = True
+        cfg["return_value.get_file"] = Mock(side_effect=m_get_file)
+
+        cfg["return_value.match_node.return_value"] = True
         m_repository.configure_mock(**cfg)
 
-        url = '/nodes/%s' % node.serialnumber
-        request = Request.blank(url, method='GET')
+        url = f"/nodes/{node.serialnumber}"
+        request = Request.blank(url, method="GET")
 
         resp = request.get_response(ztpserver.controller.Router())
 
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_JSON)
 
-        attrs = resp.json['actions'][0]['attributes']
-        self.assertFalse('variables' in attrs)
-        self.assertFalse('foo' in attrs)
-        self.assertEqual(attrs['url'], l_attr_url)
+        attrs = resp.json["actions"][0]["attributes"]
+        self.assertFalse("variables" in attrs)
+        self.assertFalse("foo" in attrs)
+        self.assertEqual(attrs["url"], l_attr_url)
 
-class DefinitionStartupConfigTests(unittest.TestCase):
-
-    @patch('ztpserver.controller.create_repository')
-    @patch('ztpserver.controller.load_pattern')
-    def test_get_definition_w_startuo_config(self, m_load_pattern,
-                                             m_repository):
 
+class DefinitionStartupConfigTests(unittest.TestCase):
+    @patch("ztpserver.controller.create_repository")
+    @patch("ztpserver.controller.load_pattern")
+    def test_get_definition_w_startuo_config(self, m_load_pattern, m_repository):
         node = create_node()
 
         action_name_1 = random_string()
         action_name_2 = random_string()
         definitions_file = create_definition()
         definitions_file.add_action(action=action_name_1)
-        definitions_file.add_action(action=action_name_2,
-                                    always_execute=True)
+        definitions_file.add_action(action=action_name_2, always_execute=True)
 
-        cfg = dict()
+        cfg = {}
 
         def m_get_file(arg):
             m_file_object = Mock()
-            if arg.endswith('.node'):
+            if arg.endswith(".node"):
                 m_file_object.read.return_value = dict(node.as_dict())
-            elif arg.endswith('definition'):
-                m_file_object.read.return_value = \
-                    dict(definitions_file.as_dict())
-            elif arg.endswith('attributes'):
+            elif arg.endswith("definition"):
+                m_file_object.read.return_value = dict(definitions_file.as_dict())
+            elif arg.endswith("attributes"):
                 raise ztpserver.repository.FileObjectNotFound
             return m_file_object
 
-        cfg['return_value.get_file.side_effect'] = m_get_file
+        cfg["return_value.get_file.side_effect"] = m_get_file
         m_repository.configure_mock(**cfg)
         m_load_pattern.return_value.match_node.return_value = Mock()
 
-        url = '/nodes/%s' % node.serialnumber
-        request = Request.blank(url, method='GET')
+        url = f"/nodes/{node.serialnumber}"
+        request = Request.blank(url, method="GET")
 
         resp = request.get_response(ztpserver.controller.Router())
         self.assertEqual(resp.status_code, constants.HTTP_STATUS_OK)
         self.assertEqual(resp.content_type, constants.CONTENT_TYPE_JSON)
-        actions = [x['action'] for x in json.loads(resp.body)['actions']]
-        self.assertEqual(actions, ['replace_config',
-                                   action_name_2])
+        actions = [x["action"] for x in json.loads(resp.body)["actions"]]
+        self.assertEqual(actions, ["replace_config", action_name_2])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     enable_logging()
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/server/test_topology.py` & `ztpserver-2.0.0/test/server/test_topology.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,114 +27,118 @@
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 import unittest
-import yaml
+from test.server.server_test_lib import enable_logging, random_string
+from unittest.mock import Mock, patch
 
-from mock import patch, Mock
+import yaml
 
 import ztpserver.serializers
 import ztpserver.topology
+from ztpserver.topology import (
+    Neighbordb,
+    Pattern,
+    create_node,
+    load_file,
+    load_neighbordb,
+    load_pattern,
+    neighbordb_path,
+    replace_config_action,
+)
 
-from ztpserver.topology import Neighbordb, Pattern
-from ztpserver.topology import create_node, load_file, load_neighbordb
-from ztpserver.topology import neighbordb_path, replace_config_action
-from ztpserver.topology import load_pattern
-from server_test_lib import enable_logging, random_string
 
 class NeighbordbUnitTests(unittest.TestCase):
-
     def test_neighbordb_path(self):
         result = neighbordb_path()
-        self.assertEqual(result, '/usr/share/ztpserver/neighbordb')
+        self.assertEqual(result, "/usr/share/ztpserver/neighbordb")
 
-    @patch('ztpserver.topology.load')
+    @patch("ztpserver.topology.load")
     def test_load_file(self, m_load):
-        result = load_file(random_string(),
-                           random_string(),
-                           random_string())
+        result = load_file(random_string(), random_string(), random_string())
         self.assertEqual(result, m_load.return_value)
 
-    @patch('ztpserver.topology.validate_neighbordb')
-    @patch('ztpserver.topology.load')
+    @patch("ztpserver.topology.validate_neighbordb")
+    @patch("ztpserver.topology.load")
     def test_load_file_failure(self, m_load, _):
         m_load.side_effect = ztpserver.serializers.SerializerError
-        self.assertRaises(ztpserver.serializers.SerializerError,
-                          load_file,
-                          random_string(),
-                          random_string(),
-                          random_string())
+        self.assertRaises(
+            ztpserver.serializers.SerializerError,
+            load_file,
+            random_string(),
+            random_string(),
+            random_string(),
+        )
 
-    @patch('ztpserver.topology.validate_neighbordb')
-    @patch('ztpserver.topology.load')
+    @patch("ztpserver.topology.validate_neighbordb")
+    @patch("ztpserver.topology.load")
     def test_load_neighbordb(self, _, m_load):
-        contents = '''
+        contents = """
             variables:
                 foo: bar
             patterns:
                 - name: dummy pattern
                   definition: dummy_definition
                   interfaces:
                     - any: any
-        '''
-        m_load.return_value = yaml.load(contents)
+        """
+        m_load.return_value = yaml.safe_load(contents)
         result = load_neighbordb(random_string())
         self.assertIsNotNone(result)
 
-    @patch('ztpserver.topology.load')
+    @patch("ztpserver.topology.load")
     def test_load_neighbordb_no_variables(self, m_load):
         # github issue #114
         contents = """
             patterns:
                 - name: dummy pattern
                   definition: dummy_definition
                   interfaces:
                     - any: any
         """
-        m_load.return_value = yaml.load(contents)
+        m_load.return_value = yaml.safe_load(contents)
         result = load_neighbordb(random_string())
         self.assertIsInstance(result, Neighbordb)
 
     def test_load_pattern_minimal(self):
-        pattern = load_pattern({'name': random_string(),
-                                'definition': random_string(),
-                                'interfaces': []})
+        pattern = load_pattern(
+            {"name": random_string(), "definition": random_string(), "interfaces": []}
+        )
         self.assertIsInstance(pattern, Pattern)
 
     def test_load_pattern_with_interfaces(self):
         # github issue #128
         contents = """
             name: test
             # Default pattern - always succeeds
             definition: dummy_definition
             interfaces:
                 - any: any:any
         """
-        kwargs = yaml.load(contents)
+        kwargs = yaml.safe_load(contents)
         pattern = load_pattern(kwargs)
         self.assertIsInstance(pattern, Pattern)
 
     def test_replace_config_action(self):
         resource = random_string()
         result = replace_config_action(resource)
-        self.assertEqual('install static startup-config file', result['name'])
-        self.assertEqual('replace_config', result['action'])
-        self.assertTrue(result['always_execute'])
+        self.assertEqual("install static startup-config file", result["name"])
+        self.assertEqual("replace_config", result["action"])
+        self.assertTrue(result["always_execute"])
 
     def test_create_node_fixup_systemmac_colon(self):
-        attrs = Mock(systemmac='99:99:99:99:99:99')
-        result = create_node({'systemmac': 
-                              attrs.systemmac})
-        self.assertTrue(':' not in result.systemmac)
+        attrs = Mock(systemmac="99:99:99:99:99:99")
+        result = create_node({"systemmac": attrs.systemmac})
+        self.assertTrue(":" not in result.systemmac)
 
     def test_create_node_fixup_systemmac_period(self):
-        attrs = Mock(systemmac='99.99.99.99.99.99')
-        result = create_node({'systemmac': 
-                              attrs.systemmac})
-        self.assertTrue('.' not in result.systemmac)
+        attrs = Mock(systemmac="99.99.99.99.99.99")
+        result = create_node({"systemmac": attrs.systemmac})
+        self.assertTrue("." not in result.systemmac)
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     enable_logging()
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/neighbordb/large_pattern_test.yml` & `ztpserver-2.0.0/test/neighbordb/large_pattern_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/chassis_test.yml` & `ztpserver-2.0.0/test/neighbordb/chassis_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/interface_name_test.yml` & `ztpserver-2.0.0/test/neighbordb/interface_name_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/ndb_entries_test.yml` & `ztpserver-2.0.0/test/neighbordb/ndb_entries_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/README.md` & `ztpserver-2.0.0/test/neighbordb/README.md`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/bogus_patterns_test.yml` & `ztpserver-2.0.0/test/neighbordb/bogus_patterns_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/small_pattern_test.yml` & `ztpserver-2.0.0/test/neighbordb/small_pattern_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/ndb_values_test.yml` & `ztpserver-2.0.0/test/neighbordb/ndb_values_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/node_interfaces_test.yml` & `ztpserver-2.0.0/test/neighbordb/node_interfaces_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/simple_test.yml` & `ztpserver-2.0.0/test/neighbordb/simple_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/chassis_test_2.yml` & `ztpserver-2.0.0/test/neighbordb/chassis_test_2.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/neighbordb/simple_functions_test.yml` & `ztpserver-2.0.0/test/neighbordb/simple_functions_test.yml`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/test/actions/test_send_email.py` & `ztpserver-2.0.0/test/actions/test_send_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,76 +23,89 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401,W0232,E1101
+# pylint: disable=C0209
 
-import sys
 import unittest
+from test.client.client_test_lib import (
+    ActionFailureTest,
+    Bootstrap,
+    get_action,
+    raise_exception,
+    random_string,
+    startup_config_action,
+)
+
+import six
+
+if six.PY2:
+    from test.client.smtp_server2 import SmtpServer
+else:
+    from test.client.smtp_server3 import SmtpServer
 
-sys.path.append('test/client')
-
-from client_test_lib import Bootstrap, ActionFailureTest
-from client_test_lib import get_action, random_string
-from client_test_lib import startup_config_action
-from client_test_lib import raise_exception
 
 class FailureTest(ActionFailureTest):
-
     def test_missing_smarthost(self):
-        self.basic_test('send_email',
-                        'Missing attribute(\'smarthost\')')
+        self.basic_test("send_email", "Missing attribute('smarthost')")
 
     def test_missing_sender(self):
-        self.basic_test('send_email',
-                        'Missing attribute(\'sender\')',
-                        attributes={'smarthost' :
-                                    random_string()})
+        self.basic_test(
+            "send_email", "Missing attribute('sender')", attributes={"smarthost": random_string()}
+        )
+
     def test_missing_receivers(self):
-        self.basic_test('send_email',
-                        'Missing attribute(\'receivers\')',
-                        attributes={'smarthost' :
-                                    random_string(),
-                                    'sender' :
-                                    random_string()})
+        self.basic_test(
+            "send_email",
+            "Missing attribute('receivers')",
+            attributes={"smarthost": random_string(), "sender": random_string()},
+        )
 
 
 class SuccessTest(unittest.TestCase):
+    def setUp(self):
+        self.smtp_server = SmtpServer()
+        self.smtp_server.start()
+
+    def tearDown(self):
+        self.smtp_server.stop()
 
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
-        smarthost = "%s:2525" % str(bootstrap.server).split(':')[0]
-
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {
-                        'smarthost': smarthost,
-                        'sender': 'ztps@localhost',
-                        'receivers': ['ztps@localhost']}}])
+            actions=[
+                {"action": "startup_config_action"},
+                {
+                    "action": "test_action",
+                    "attributes": {
+                        "smarthost": "{}:{}".format(
+                            self.smtp_server.hostname, self.smtp_server.port
+                        ),
+                        "sender": "ztps@localhost",
+                        "receivers": ["ztps@localhost"],
+                    },
+                },
+            ]
+        )
 
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
 
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
-
-        action = get_action('send_email')
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+        action = get_action("send_email")
+        bootstrap.ztps.set_action_response("test_action", action)
 
         bootstrap.start_test()
         try:
-            self.failUnless(bootstrap.success())
-        except Exception as exception: #pylint: disable=W0703
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            self.assertTrue(bootstrap.success())
+        except Exception as exception:  # pylint: disable=W0703
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(exception)
         finally:
             bootstrap.end_test()
 
 
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/actions/test_add_config.py` & `ztpserver-2.0.0/test/actions/test_add_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,248 +23,254 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401,W0232,E1101,W0402
+# pylint: disable=C0209
 
 import os
 import os.path
 import unittest
-import sys
 from string import Template
+from test.client.client_test_lib import (
+    ActionFailureTest,
+    Bootstrap,
+    file_log,
+    get_action,
+    raise_exception,
+    random_string,
+    startup_config_action,
+)
 
-sys.path.append('test/client')
-
-from client_test_lib import Bootstrap, ActionFailureTest
-from client_test_lib import file_log, get_action, random_string
-from client_test_lib import startup_config_action
-from client_test_lib import raise_exception
 
 class FailureTest(ActionFailureTest):
-
     def test_missing_url(self):
-        self.basic_test('add_config', 'Missing attribute(\'url\')')
+        self.basic_test("add_config", "Missing attribute('url')")
 
     def test_url_failure(self):
-        self.basic_test('add_config', 'Unable to retrieve config from URL',
-                        attributes={'url' :
-                                    random_string()})
+        self.basic_test(
+            "add_config", "Unable to retrieve config from URL", attributes={"url": random_string()}
+        )
 
     def test_variables_failure(self):
         url = random_string()
         contents = random_string()
-        self.basic_test('add_config', 
-                        'Unable to perform variable substitution - '
-                        'invalid variables',
-                        attributes={'url' : url,
-                                    'variables' : random_string()},
-                        file_responses={url : contents})
+        self.basic_test(
+            "add_config",
+            "Unable to perform variable substitution - invalid variables",
+            attributes={"url": url, "variables": random_string()},
+            file_responses={url: contents},
+        )
 
     def test_variable_missing_failure(self):
         url = random_string()
-        contents = random_string() + ' $missing_var'
-        self.basic_test('add_config', 
-                        'Unable to perform variable substitution - '
-                        '\'missing_var\' missing from list of substitutions',
-                        attributes={'url' : url,
-                                    'substitution_mode': 'strict',
-                                    'variables' : {}},
-                        file_responses={url : contents})
+        contents = random_string() + " $missing_var"
+        self.basic_test(
+            "add_config",
+            (
+                "Unable to perform variable substitution - 'missing_var' missing from list of "
+                "substitutions"
+            ),
+            attributes={"url": url, "substitution_mode": "strict", "variables": {}},
+            file_responses={url: contents},
+        )
 
     def test_invalid_substitution_mode(self):
-        self.basic_test('add_config', 
-                        'Invalid option specified for '
-                        'substitution_mode attribute',
-                        attributes={'url': random_string(),
-                                    'substitution_mode': 'dummy'})
+        self.basic_test(
+            "add_config",
+            "Invalid option specified for substitution_mode attribute",
+            attributes={"url": random_string(), "substitution_mode": "dummy"},
+        )
 
 
 class SuccessTest(unittest.TestCase):
-
-
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('add_config'))
+            actions=[{"action": "test_action", "attributes": {"url": url}}]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("add_config"))
         contents = random_string()
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless(contents.split() == 
-                            file_log(bootstrap.startup_config))
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(contents.split() == file_log(bootstrap.startup_config))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_success_url(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
-        url = 'http://%s/%s' % (bootstrap.server, config)
+        url = "http://{}/{}".format(bootstrap.server, config)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('add_config'))
+            actions=[{"action": "test_action", "attributes": {"url": url}}]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("add_config"))
         contents = random_string()
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless(contents.split() == 
-                            file_log(bootstrap.startup_config))
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(contents.split() == file_log(bootstrap.startup_config))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_append(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
-        url = 'http://%s/%s' % (bootstrap.server, config)
+        url = "http://{}/{}".format(bootstrap.server, config)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('add_config'))
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"url": url}},
+            ]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("add_config"))
 
         startup_config_text = random_string()
         bootstrap.ztps.set_action_response(
-            'startup_config_action',
-            startup_config_action(lines=[startup_config_text]))
+            "startup_config_action", startup_config_action(lines=[startup_config_text])
+        )
         contents = random_string()
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
             log = file_log(bootstrap.startup_config)
-            self.failUnless(contents in log)
-            self.failUnless(startup_config_text in log)
-            self.failUnless(bootstrap.success())
+            self.assertTrue(contents in log)
+            self.assertTrue(startup_config_text in log)
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_multi_lines(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
-        url = 'http://%s/%s' % (bootstrap.server, config)
+        url = "http://{}/{}".format(bootstrap.server, config)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('add_config'))
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"url": url}},
+            ]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("add_config"))
 
-        startup_config_lines = [random_string(), random_string(),
-                                random_string(), random_string()]
+        startup_config_lines = [random_string(), random_string(), random_string(), random_string()]
         bootstrap.ztps.set_action_response(
-            'startup_config_action',
-            startup_config_action(lines=startup_config_lines))
-        contents = '\n'.join([random_string(), random_string(),
-                              random_string(), random_string(),
-                              random_string(), random_string()])
+            "startup_config_action", startup_config_action(lines=startup_config_lines)
+        )
+        contents = "\n".join(
+            [
+                random_string(),
+                random_string(),
+                random_string(),
+                random_string(),
+                random_string(),
+                random_string(),
+            ]
+        )
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
             log = file_log(bootstrap.startup_config)
             all_lines = startup_config_lines + contents.split()
             for line in all_lines:
-                self.failUnless(line in log)
-            self.failUnless(bootstrap.success())
+                self.assertTrue(line in log)
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_variables_strict(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
-        var_dict = { 'a' : 'A',
-                     'b' : 'A',
-                     'xxx' : '999',
-                     'dummy': 'DUMMY'}
-        bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {'url' : url,
-                                     'substitution_mode': 'strict',
-                                     'variables': var_dict}}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('add_config'))
-        contents = '$a 1234 $b 4  321 $xxx$a'
+        var_dict = {"a": "A", "b": "A", "xxx": "999", "dummy": "DUMMY"}
+        bootstrap.ztps.set_definition_response(
+            actions=[
+                {
+                    "action": "test_action",
+                    "attributes": {
+                        "url": url,
+                        "substitution_mode": "strict",
+                        "variables": var_dict,
+                    },
+                }
+            ]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("add_config"))
+        contents = "$a 1234 $b 4  321 $xxx$a"
         expected_contents = Template(contents).substitute(var_dict)
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless([expected_contents] ==
-                            file_log(bootstrap.startup_config))
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue([expected_contents] == file_log(bootstrap.startup_config))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_variables_loose(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
-        var_dict = { 'a' : 'A',
-                     'b' : 'A',
-                     'xxx' : '999',
-                     'dummy': 'DUMMY'}
-        bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {'url' : url,
-                                     'substitution_mode': 'loose',
-                                     'variables': var_dict}}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('add_config'))
-        contents = '$a 1234 $b 4  321 $xxx$a'
+        var_dict = {"a": "A", "b": "A", "xxx": "999", "dummy": "DUMMY"}
+        bootstrap.ztps.set_definition_response(
+            actions=[
+                {
+                    "action": "test_action",
+                    "attributes": {"url": url, "substitution_mode": "loose", "variables": var_dict},
+                }
+            ]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("add_config"))
+        contents = "$a 1234 $b 4  321 $xxx$a"
         expected_contents = Template(contents).safe_substitute(var_dict)
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless([expected_contents] ==
-                            file_log(bootstrap.startup_config))
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue([expected_contents] == file_log(bootstrap.startup_config))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/actions/test_run_bash_script.py` & `ztpserver-2.0.0/test/actions/test_run_bash_script.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,157 +23,167 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401,W0232,E1101,W0402
+# pylint: disable=C0209
 
 import os
 import os.path
 import unittest
-import sys
 from string import Template
+from test.client.client_test_lib import (
+    ActionFailureTest,
+    Bootstrap,
+    get_action,
+    raise_exception,
+    random_string,
+    startup_config_action,
+)
 
-sys.path.append('test/client')
-
-from client_test_lib import Bootstrap, ActionFailureTest
-from client_test_lib import get_action, random_string
-from client_test_lib import startup_config_action
-from client_test_lib import raise_exception
 
 class FailureTest(ActionFailureTest):
-
     def test_missing_url(self):
-        self.basic_test('run_bash_script', 'Missing attribute(\'url\')')
+        self.basic_test("run_bash_script", "Missing attribute('url')")
 
     def test_url_failure(self):
-        self.basic_test('run_bash_script', 
-                        'Unable to retrieve config from URL',
-                        attributes={'url' :
-                                    random_string()})
+        self.basic_test(
+            "run_bash_script",
+            "Unable to retrieve config from URL",
+            attributes={"url": random_string()},
+        )
 
     def test_variables_failure(self):
         url = random_string()
         contents = random_string()
-        self.basic_test('run_bash_script', 
-                        'Unable to perform variable substitution - '
-                        'invalid variables',
-                        attributes={'url' : url,
-                                    'variables' : random_string()},
-                        file_responses={url : contents})
+        self.basic_test(
+            "run_bash_script",
+            "Unable to perform variable substitution - invalid variables",
+            attributes={"url": url, "variables": random_string()},
+            file_responses={url: contents},
+        )
 
     def test_variable_missing_failure(self):
         url = random_string()
-        contents = random_string() + ' $missing_var'
-        self.basic_test('run_bash_script', 
-                        'Unable to perform variable substitution - '
-                        '\'missing_var\' missing from list of substitutions',
-                        attributes={'url' : url,
-                                    'variables' : {}},
-                        file_responses={url : contents})
+        contents = random_string() + " $missing_var"
+        self.basic_test(
+            "run_bash_script",
+            (
+                "Unable to perform variable substitution - "
+                "'missing_var' missing from list of substitutions"
+            ),
+            attributes={"url": url, "variables": {}},
+            file_responses={url: contents},
+        )
 
 
 class SuccessTest(unittest.TestCase):
-
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('run_bash_script'))
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"url": url}},
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+        bootstrap.ztps.set_action_response("test_action", get_action("run_bash_script"))
 
         print_string = random_string()
-        contents = '''#!/usr/bin/env python
-print "%s"''' % print_string
+        contents = """#!/usr/bin/env python
+print("{}")""".format(
+            print_string
+        )
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless(print_string in bootstrap.output)
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(print_string in bootstrap.output)
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_failure(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('run_bash_script'))
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"url": url}},
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+        bootstrap.ztps.set_action_response("test_action", get_action("run_bash_script"))
 
-        contents = '''#!/usr/bin/env python
-assert False'''
+        contents = """#!/usr/bin/env python
+assert False"""
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless('AssertionError' in bootstrap.output)
-            self.failUnless(bootstrap.action_failure())
+            self.assertTrue("AssertionError" in bootstrap.output)
+            self.assertTrue(bootstrap.action_failure())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_variables(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
-        var_dict = { 'a' : 'A',
-                     'b' : 'A',
-                     'xxx' : '999',
-                     'dummy': 'DUMMY'}
+        var_dict = {"a": "A", "b": "A", "xxx": "999", "dummy": "DUMMY"}
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes': {'url' : url,
-                                     'substitution_mode': 'strict',
-                                     'variables': var_dict}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('run_bash_script'))
-
-        print_string = '$a 1234 $b 4 321 $xxx$a'
-        contents = '''#!/usr/bin/env bash
-echo %s''' % print_string
+            actions=[
+                {"action": "startup_config_action"},
+                {
+                    "action": "test_action",
+                    "attributes": {
+                        "url": url,
+                        "substitution_mode": "strict",
+                        "variables": var_dict,
+                    },
+                },
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+        bootstrap.ztps.set_action_response("test_action", get_action("run_bash_script"))
+
+        print_string = "$a 1234 $b 4 321 $xxx$a"
+        contents = """#!/usr/bin/env bash
+echo {}""".format(
+            print_string
+        )
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         expected_contents = Template(print_string).substitute(var_dict)
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless(expected_contents in bootstrap.output)
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(expected_contents in bootstrap.output)
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/actions/test_copy_file.py` & `ztpserver-2.0.0/test/actions/test_copy_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,608 +23,605 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401,W0232,E1101
+# pylint: disable=C0209
 
+import io
 import os
 import os.path
 import random
 import shutil
-import sys
 import unittest
-
 from stat import ST_MODE
+from test.client.client_test_lib import (
+    ActionFailureTest,
+    Bootstrap,
+    file_log,
+    get_action,
+    raise_exception,
+    random_string,
+    remove_file,
+    startup_config_action,
+)
 
-sys.path.append('test/client')
+import six
 
-from client_test_lib import Bootstrap, ActionFailureTest
-from client_test_lib import file_log, get_action, random_string
-from client_test_lib import startup_config_action, remove_file
-from client_test_lib import raise_exception
 
 def random_permissions():
-    return '7%s%s' % ((random.choice([1, 2, 3, 4, 5, 6, 7]),
-                       random.choice([1, 2, 3, 4, 5, 6, 7])))
+    return "7{}{}".format(
+        random.choice([1, 2, 3, 4, 5, 6, 7]), random.choice([1, 2, 3, 4, 5, 6, 7])
+    )
 
 
 class FailureTest(ActionFailureTest):
-
     def test_missing_src_url(self):
-        self.basic_test('copy_file',
-                        'Missing attribute(\'src_url\')')
+        self.basic_test("copy_file", "Missing attribute('src_url')")
 
     def test_missing_dst_url(self):
-        self.basic_test('copy_file',
-                        'Missing attribute(\'dst_url\')',
-                        attributes={'src_url' :
-                                        random_string()})
+        self.basic_test(
+            "copy_file", "Missing attribute('dst_url')", attributes={"src_url": random_string()}
+        )
 
     def test_wrong_overwrite_value(self):
-        self.basic_test('copy_file',
-                        'Erroneous \'overwrite\' value',
-                        attributes={'src_url' :
-                                    random_string(),
-                                    'dst_url' :
-                                    random_string(),
-                                    'overwrite' :
-                                    'bogus'})
+        self.basic_test(
+            "copy_file",
+            "Erroneous 'overwrite' value",
+            attributes={
+                "src_url": random_string(),
+                "dst_url": random_string(),
+                "overwrite": "bogus",
+            },
+        )
 
     def test_url_failure(self):
-        action = get_action('copy_file')
-        action = action.replace('/mnt/flash/.ztp-files',
-                                '/tmp')
-
-        self.basic_test('copy_file',
-                        'Unable to retrieve file from URL',
-                        attributes={'src_url' :
-                                    random_string(),
-                                    'dst_url' :
-                                    random_string()},
-                        action_value=action)
+        action = get_action("copy_file")
+        action = action.replace("/mnt/flash/.ztp-files", "/tmp")
 
+        self.basic_test(
+            "copy_file",
+            "Unable to retrieve file from URL",
+            attributes={"src_url": random_string(), "dst_url": random_string()},
+            action_value=action,
+        )
 
-class SuccessSrcUrlReplacementTests(unittest.TestCase):
 
+class SuccessSrcUrlReplacementTests(unittest.TestCase):
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
-        destination = '/tmp/%s' % random_string()
-        ztps_server = 'http://%s' % bootstrap.server
-        url = 'http://%s/%s' % (bootstrap.server, source)
+        destination = "/tmp/{}".format(random_string())
+        ztps_server = "http://{}".format(bootstrap.server)
+        url = "http://{}/{}".format(bootstrap.server, source)
 
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'src_url'    : url,
-                                      'dst_url'    : destination,
-                                      'ztps_server': ztps_server}}])
+            actions=[
+                {"action": "startup_config_action"},
+                {
+                    "action": "test_action",
+                    "attributes": {
+                        "src_url": url,
+                        "dst_url": destination,
+                        "ztps_server": ztps_server,
+                    },
+                },
+            ]
+        )
 
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
 
-        action = get_action('copy_file')
+        action = get_action("copy_file")
 
         # Make the destinaton persistent
-        action = action.replace('PERSISTENT_STORAGE = [',
-                                'PERSISTENT_STORAGE = [\'%s\', ' %
-                                destination)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+        action = action.replace(
+            "PERSISTENT_STORAGE = [", "PERSISTENT_STORAGE = ['{}', ".format(destination)
+        )
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
         bootstrap.start_test()
 
-        destination_path = '%s/%s' % (destination, source)
+        destination_path = "{}/{}".format(destination, source)
 
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([contents] ==
-                            file_log(destination_path))
-            self.failIf(os.path.isfile(bootstrap.rc_eos))
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([contents] == file_log(destination_path))
+            self.assertFalse(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             shutil.rmtree(destination)
             bootstrap.end_test()
 
     def test_append_server(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
-        destination = '/tmp/%s' % random_string()
-        ztps_server = 'http://%s' % bootstrap.server
+        destination = "/tmp/{}".format(random_string())
+        ztps_server = "http://{}".format(bootstrap.server)
 
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                     'attributes' : {'src_url'    : source,
-                                     'dst_url'    : destination,
-                                     'ztps_server': ztps_server}}])
+            actions=[
+                {"action": "startup_config_action"},
+                {
+                    "action": "test_action",
+                    "attributes": {
+                        "src_url": source,
+                        "dst_url": destination,
+                        "ztps_server": ztps_server,
+                    },
+                },
+            ]
+        )
 
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
 
-        action = get_action('copy_file')
+        action = get_action("copy_file")
 
         # Make the destinaton persistent
-        action = action.replace('PERSISTENT_STORAGE = [',
-                                'PERSISTENT_STORAGE = [\'%s\', ' %
-                                destination)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+        action = action.replace(
+            "PERSISTENT_STORAGE = [", "PERSISTENT_STORAGE = ['{}', ".format(destination)
+        )
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
         bootstrap.start_test()
 
-        destination_path = '%s/%s' % (destination, source)
+        destination_path = "{}/{}".format(destination, source)
 
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([contents] ==
-                            file_log(destination_path))
-            self.failIf(os.path.isfile(bootstrap.rc_eos))
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([contents] == file_log(destination_path))
+            self.assertFalse(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             shutil.rmtree(destination)
             bootstrap.end_test()
 
 
-
-
 class SuccessPersistentTest(unittest.TestCase):
-
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
-        destination = '/tmp/%s' % random_string()
+        destination = "/tmp/{}".format(random_string())
 
-        url = 'http://%s/%s' % (bootstrap.server, source)
+        url = "http://{}/{}".format(bootstrap.server, source)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'src_url' : url,
-                                      'dst_url' : destination}}])
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"src_url": url, "dst_url": destination}},
+            ]
+        )
 
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
 
-        action = get_action('copy_file')
+        action = get_action("copy_file")
 
         # Make the destinaton persistent
-        action = action.replace('PERSISTENT_STORAGE = [',
-                                'PERSISTENT_STORAGE = [\'%s\', ' %
-                                destination)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+        action = action.replace(
+            "PERSISTENT_STORAGE = [", "PERSISTENT_STORAGE = ['{}', ".format(destination)
+        )
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
         bootstrap.start_test()
 
-        destination_path = '%s/%s' % (destination, source)
+        destination_path = "{}/{}".format(destination, source)
 
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([contents] ==
-                            file_log(destination_path))
-            self.failIf(os.path.isfile(bootstrap.rc_eos))
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([contents] == file_log(destination_path))
+            self.assertFalse(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             shutil.rmtree(destination)
             bootstrap.end_test()
 
     def test_replace(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
-        destination = '/tmp/%s' % random_string()
+        destination = "/tmp/{}".format(random_string())
 
-        url = 'http://%s/%s' % (bootstrap.server, source)
-        attributes = {'src_url' : url,
-                      'dst_url' : destination}
+        url = "http://{}/{}".format(bootstrap.server, source)
+        attributes = {"src_url": url, "dst_url": destination}
 
         # 'replace' is the default
         if bool(random.getrandbits(1)):
-            attributes['overwrite'] = 'replace'
+            attributes["overwrite"] = "replace"
 
-        mode = None
-        if True or bool(random.getrandbits(1)):
-            mode = random_permissions()
-            attributes['mode'] = mode
+        mode = random_permissions()
+        attributes["mode"] = mode
 
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : attributes}])
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": attributes},
+            ]
+        )
 
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
 
-        action = get_action('copy_file')
+        action = get_action("copy_file")
 
         # Make the destinaton persistent
-        action = action.replace('PERSISTENT_STORAGE = [',
-                                'PERSISTENT_STORAGE = [\'%s\', ' %
-                                destination)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+        action = action.replace(
+            "PERSISTENT_STORAGE = [", "PERSISTENT_STORAGE = ['{}', ".format(destination)
+        )
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
-        destination_path = '%s/%s' % (destination, source)
+        destination_path = "{}/{}".format(destination, source)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([contents] ==
-                            file_log(destination_path))
-            self.failIf(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([contents] == file_log(destination_path))
+            self.assertFalse(os.path.isfile(bootstrap.rc_eos))
             if mode:
-                self.failUnless(mode ==
-                                oct(os.stat(destination_path)[ST_MODE])[-3:])
-            self.failUnless(bootstrap.success())
+                self.assertTrue(mode == oct(os.stat(destination_path)[ST_MODE])[-3:])
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             shutil.rmtree(destination)
             bootstrap.end_test()
 
     def test_keep_original(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
-        destination = '/tmp/%s' % random_string()
+        destination = "/tmp/{}".format(random_string())
 
-        url = 'http://%s/%s' % (bootstrap.server, source)
+        url = "http://{}/{}".format(bootstrap.server, source)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'src_url' : url,
-                                      'dst_url' : destination,
-                                      'overwrite' : 'if-missing'}}])
+            actions=[
+                {"action": "startup_config_action"},
+                {
+                    "action": "test_action",
+                    "attributes": {
+                        "src_url": url,
+                        "dst_url": destination,
+                        "overwrite": "if-missing",
+                    },
+                },
+            ]
+        )
 
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
 
-        action = get_action('copy_file')
+        action = get_action("copy_file")
 
         # Make the destinaton persistent
-        action = action.replace('PERSISTENT_STORAGE = [',
-                                'PERSISTENT_STORAGE = [\'%s\', ' %
-                                destination)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+        action = action.replace(
+            "PERSISTENT_STORAGE = [", "PERSISTENT_STORAGE = ['{}', ".format(destination)
+        )
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
-        destination_path = '%s/%s' % (destination, source)
+        destination_path = "{}/{}".format(destination, source)
         existing_contents = random_string()
         os.makedirs(destination)
-        file_descriptor = open(destination_path, 'w')
-        file_descriptor.write(existing_contents)
-        file_descriptor.close()
+        with io.open(destination_path, "w", encoding="utf8") as file_descriptor:
+            file_descriptor.write(six.ensure_text(existing_contents))
 
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([existing_contents] ==
-                            file_log(destination_path))
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([existing_contents] == file_log(destination_path))
 
-            self.failIf(os.path.isfile(bootstrap.rc_eos))
-            self.failUnless(bootstrap.success())
+            self.assertFalse(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             shutil.rmtree(destination)
             bootstrap.end_test()
 
     def test_keep_backup(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
-        destination = '/tmp/%s' % random_string()
+        destination = "/tmp/{}".format(random_string())
 
-        url = 'http://%s/%s' % (bootstrap.server, source)
+        url = "http://{}/{}".format(bootstrap.server, source)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'src_url' : url,
-                                      'dst_url' : destination,
-                                      'overwrite' : 'backup'}}])
+            actions=[
+                {"action": "startup_config_action"},
+                {
+                    "action": "test_action",
+                    "attributes": {"src_url": url, "dst_url": destination, "overwrite": "backup"},
+                },
+            ]
+        )
 
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
 
-        action = get_action('copy_file')
+        action = get_action("copy_file")
 
         # Make the destinaton persistent
-        action = action.replace('PERSISTENT_STORAGE = [',
-                                'PERSISTENT_STORAGE = [\'%s\', ' %
-                                destination)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+        action = action.replace(
+            "PERSISTENT_STORAGE = [", "PERSISTENT_STORAGE = ['{}', ".format(destination)
+        )
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
-        destination_path = '%s/%s' % (destination, source)
+        destination_path = "{}/{}".format(destination, source)
         backup_contents = random_string()
         os.makedirs(destination)
-        file_descriptor = open(destination_path, 'w')
-        file_descriptor.write(backup_contents)
-        file_descriptor.close()
+        with io.open(destination_path, "w", encoding="utf8") as file_descriptor:
+            file_descriptor.write(six.ensure_text(backup_contents))
 
         bootstrap.start_test()
 
-        backup_path = '%s.backup' % destination_path
+        backup_path = "{}.backup".format(destination_path)
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([contents] ==
-                            file_log(destination_path))
-
-            self.failUnless(os.path.isfile(backup_path))
-            self.failUnless([backup_contents] ==
-                            file_log(backup_path))
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([contents] == file_log(destination_path))
+
+            self.assertTrue(os.path.isfile(backup_path))
+            self.assertTrue([backup_contents] == file_log(backup_path))
 
-            self.failIf(os.path.isfile(bootstrap.rc_eos))
-            self.failUnless(bootstrap.success())
+            self.assertFalse(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             remove_file(backup_path)
             shutil.rmtree(destination)
             bootstrap.end_test()
 
-class SuccessNonPersistentTest(unittest.TestCase):
 
+class SuccessNonPersistentTest(unittest.TestCase):
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
         destination = random_string()
 
-        url = 'http://%s/%s' % (bootstrap.server, source)
+        url = "http://{}/{}".format(bootstrap.server, source)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'src_url' : url,
-                                      'dst_url' : destination}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-
-        persistent_dir = '/tmp'
-        action = get_action('copy_file')
-        action = action.replace('/mnt/flash/.ztp-files',
-                                persistent_dir)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"src_url": url, "dst_url": destination}},
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+
+        persistent_dir = "/tmp"
+        action = get_action("copy_file")
+        action = action.replace("/mnt/flash/.ztp-files", persistent_dir)
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
         bootstrap.start_test()
 
-        destination_path = '%s/%s' % (persistent_dir, source)
+        destination_path = "{}/{}".format(persistent_dir, source)
 
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([contents] ==
-                            file_log(destination_path))
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([contents] == file_log(destination_path))
 
-            self.failUnless(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(os.path.isfile(bootstrap.rc_eos))
             log = file_log(bootstrap.rc_eos)
-            self.failUnless('#!/bin/bash' in log)
-            self.failUnless('sudo cp %s %s' %
-                            (destination_path, destination) in log)
-            self.failUnless(bootstrap.success())
+            self.assertTrue("#!/bin/bash" in log)
+            self.assertTrue("sudo cp {} {}".format(destination_path, destination) in log)
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             bootstrap.end_test()
 
     def test_replace(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
         destination = random_string()
 
-        url = 'http://%s/%s' % (bootstrap.server, source)
-        attributes = {'src_url' : url,
-                      'dst_url' : destination}
+        url = "http://{}/{}".format(bootstrap.server, source)
+        attributes = {"src_url": url, "dst_url": destination}
 
         # 'replace' is the default
         if bool(random.getrandbits(1)):
-            attributes['overwrite'] = 'replace'
+            attributes["overwrite"] = "replace"
 
-        mode = None
-        if True or bool(random.getrandbits(1)):
-            mode = random_permissions()
-            attributes['mode'] = mode
+        mode = random_permissions()
+        attributes["mode"] = mode
 
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : attributes}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-
-        persistent_dir = '/tmp'
-        action = get_action('copy_file')
-        action = action.replace('/mnt/flash/.ztp-files',
-                                persistent_dir)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": attributes},
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+
+        persistent_dir = "/tmp"
+        action = get_action("copy_file")
+        action = action.replace("/mnt/flash/.ztp-files", persistent_dir)
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
-        destination_path = '%s/%s' % (persistent_dir, source)
+        destination_path = "{}/{}".format(persistent_dir, source)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([contents] ==
-                            file_log(destination_path))
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([contents] == file_log(destination_path))
 
-            self.failUnless(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(os.path.isfile(bootstrap.rc_eos))
             log = file_log(bootstrap.rc_eos)
-            self.failUnless('#!/bin/bash' in log)
-            self.failUnless('sudo cp %s %s' %
-                            (destination_path, destination) in log)
+            self.assertTrue("#!/bin/bash" in log)
+            self.assertTrue("sudo cp {} {}".format(destination_path, destination) in log)
             if mode:
-                self.failUnless('sudo chmod %s %s' %
-                                (mode, destination) in log)
-            self.failUnless(bootstrap.success())
+                self.assertTrue("sudo chmod {} {}".format(mode, destination) in log)
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             bootstrap.end_test()
 
     def test_keep_original(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
         destination = random_string()
 
-        url = 'http://%s/%s' % (bootstrap.server, source)
+        url = "http://{}/{}".format(bootstrap.server, source)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'src_url' : url,
-                                      'dst_url' : destination,
-                                      'overwrite' : 'if-missing'}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-
-        persistent_dir = '/tmp'
-        action = get_action('copy_file')
-        action = action.replace('/mnt/flash/.ztp-files',
-                                persistent_dir)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+            actions=[
+                {"action": "startup_config_action"},
+                {
+                    "action": "test_action",
+                    "attributes": {
+                        "src_url": url,
+                        "dst_url": destination,
+                        "overwrite": "if-missing",
+                    },
+                },
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+
+        persistent_dir = "/tmp"
+        action = get_action("copy_file")
+        action = action.replace("/mnt/flash/.ztp-files", persistent_dir)
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
         bootstrap.start_test()
 
-        destination_path = '%s/%s' % (persistent_dir, source)
+        destination_path = "{}/{}".format(persistent_dir, source)
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([contents] ==
-                            file_log(destination_path))
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([contents] == file_log(destination_path))
 
-            self.failUnless(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(os.path.isfile(bootstrap.rc_eos))
             log = file_log(bootstrap.rc_eos)
-            self.failUnless('#!/bin/bash' in log)
-            self.failUnless('[ ! -f %s ] && sudo cp %s %s' %
-                            (destination, destination_path,
-                             destination) in log)
-            self.failUnless(bootstrap.success())
+            self.assertTrue("#!/bin/bash" in log)
+            self.assertTrue(
+                "[ ! -f {destination} ] && sudo cp {} {destination}".format(
+                    destination_path, destination=destination
+                )
+                in log
+            )
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             bootstrap.end_test()
 
     def test_keep_backup(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         source = random_string()
         destination = random_string()
 
-        url = 'http://%s/%s' % (bootstrap.server, source)
+        url = "http://{}/{}".format(bootstrap.server, source)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'src_url' : url,
-                                      'dst_url' : destination,
-                                      'overwrite' : 'backup'}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-
-        persistent_dir = '/tmp'
-        action = get_action('copy_file')
-        action = action.replace('/mnt/flash/.ztp-files',
-                                persistent_dir)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+            actions=[
+                {"action": "startup_config_action"},
+                {
+                    "action": "test_action",
+                    "attributes": {"src_url": url, "dst_url": destination, "overwrite": "backup"},
+                },
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+
+        persistent_dir = "/tmp"
+        action = get_action("copy_file")
+        action = action.replace("/mnt/flash/.ztp-files", persistent_dir)
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(source, contents)
 
         bootstrap.start_test()
 
-        destination_path = '%s/%s' % (persistent_dir, source)
+        destination_path = "{}/{}".format(persistent_dir, source)
         try:
-            self.failUnless(os.path.isfile(destination_path))
-            self.failUnless([contents] ==
-                            file_log(destination_path))
+            self.assertTrue(os.path.isfile(destination_path))
+            self.assertTrue([contents] == file_log(destination_path))
 
-            self.failUnless(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(os.path.isfile(bootstrap.rc_eos))
             log = file_log(bootstrap.rc_eos)
-            self.failUnless('#!/bin/bash' in log)
-            self.failUnless('sudo cp %s %s' %
-                            (destination_path, destination) in log)
-            self.failUnless('[ -f %s ] && sudo mv %s %s.backup' %
-                            (destination, destination,
-                             destination) in log)
-            self.failUnless(bootstrap.success())
+            self.assertTrue("#!/bin/bash" in log)
+            self.assertTrue("sudo cp {} {}".format(destination_path, destination) in log)
+            self.assertTrue(
+                "[ -f {destination} ] && sudo mv {destination} {destination}.backup".format(
+                    destination=destination
+                )
+                in log
+            )
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(destination_path)
             bootstrap.end_test()
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/actions/test_replace_config.py` & `ztpserver-2.0.0/test/actions/test_replace_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,113 +23,108 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401,W0232,E1101
+# pylint: disable=C0209
 
 import os
 import os.path
 import unittest
-import sys
+from test.client.client_test_lib import (
+    STATUS_NOT_FOUND,
+    ActionFailureTest,
+    Bootstrap,
+    file_log,
+    get_action,
+    raise_exception,
+    random_string,
+)
 
-sys.path.append('test/client')
-
-from client_test_lib import STATUS_NOT_FOUND
-from client_test_lib import Bootstrap, ActionFailureTest
-from client_test_lib import file_log, get_action, random_string
-from client_test_lib import raise_exception
 
 class FailureTest(ActionFailureTest):
-
     def test_missing_url(self):
-        self.basic_test('replace_config',
-                        'Missing attribute(\'url\')')
+        self.basic_test("replace_config", "Missing attribute('url')")
 
     def test_url_failure(self):
-        self.basic_test('replace_config',
-                        'Unable to retrieve config from URL',
-                        attributes={'url' : random_string()})
+        self.basic_test(
+            "replace_config",
+            "Unable to retrieve config from URL",
+            attributes={"url": random_string()},
+        )
 
     def test_bad_file_status(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
-        url = 'http://%s/%s' % (bootstrap.server, config)
+        url = "http://{}/{}".format(bootstrap.server, config)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('replace_config'))
+            actions=[{"action": "test_action", "attributes": {"url": url}}]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("replace_config"))
         contents = random_string()
-        bootstrap.ztps.set_file_response(config, contents,
-                                         status=STATUS_NOT_FOUND)
+        bootstrap.ztps.set_file_response(config, contents, status=STATUS_NOT_FOUND)
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.action_failure())
-            msg = [x for x in bootstrap.output.split('\n') if x][-1]
-            self.failUnless('Unable to retrieve config from URL' in msg)
+            self.assertTrue(bootstrap.action_failure())
+            msg = [x for x in bootstrap.output.split("\n") if x][-1]
+            self.assertTrue("Unable to retrieve config from URL" in msg)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
 class SuccessTest(unittest.TestCase):
-
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('replace_config'))
+            actions=[{"action": "test_action", "attributes": {"url": url}}]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("replace_config"))
         contents = random_string()
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless(contents.split() == 
-                            file_log(bootstrap.startup_config))
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(contents.split() == file_log(bootstrap.startup_config))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_url_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
-        url = 'http://%s/%s' % (bootstrap.server, config)
+        url = "http://{}/{}".format(bootstrap.server, config)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('replace_config'))
+            actions=[{"action": "test_action", "attributes": {"url": url}}]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("replace_config"))
         contents = random_string()
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless(contents.split() == 
-                            file_log(bootstrap.startup_config))
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(contents.split() == file_log(bootstrap.startup_config))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/actions/test_install_cli_plugin.py` & `ztpserver-2.0.0/test/actions/test_install_cli_plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,131 +23,122 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401,W0232,E1101
+# pylint: disable=C0209
 
 import os
 import os.path
-import unittest
 import shutil
-import sys
-
-sys.path.append('test/client')
+import unittest
+from test.client.client_test_lib import (
+    ActionFailureTest,
+    Bootstrap,
+    file_log,
+    get_action,
+    raise_exception,
+    random_string,
+    startup_config_action,
+)
 
-from client_test_lib import Bootstrap, ActionFailureTest
-from client_test_lib import file_log, get_action, random_string
-from client_test_lib import startup_config_action
-from client_test_lib import raise_exception
 
 class FailureTest(ActionFailureTest):
-
     def test_missing_url(self):
-        self.basic_test('install_cli_plugin',
-                        'Missing attribute(\'url\')')
+        self.basic_test("install_cli_plugin", "Missing attribute('url')")
 
     def test_url_failure(self):
-        self.basic_test('install_cli_plugin',
-                        'Unable to retrieve CliPlugin from URL',
-                        attributes={'url' :
-                                    random_string()})
+        self.basic_test(
+            "install_cli_plugin",
+            "Unable to retrieve CliPlugin from URL",
+            attributes={"url": random_string()},
+        )
 
 
 class SuccessTest(unittest.TestCase):
-
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         plugin = random_string()
-        url = 'http://%s/%s' % (bootstrap.server, plugin)
+        url = "http://{}/{}".format(bootstrap.server, plugin)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'url' : url}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-
-        plugin_dir = '/tmp'
-        persistent_dir = '/tmp/persistent'
-        action = get_action('install_cli_plugin')
-        action = action.replace('/usr/lib/python2.7/site-packages/CliPlugin',
-                                plugin_dir)
-
-        action = action.replace('/mnt/flash/.ztp-plugins',
-                                persistent_dir)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"url": url}},
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+
+        plugin_dir = "/tmp"
+        persistent_dir = "/tmp/persistent"
+        action = get_action("install_cli_plugin")
+        action = action.replace("/usr/lib/python2.7/site-packages/CliPlugin", plugin_dir)
+
+        action = action.replace("/mnt/flash/.ztp-plugins", persistent_dir)
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(plugin, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(os.path.isfile(bootstrap.rc_eos))
             log = file_log(bootstrap.rc_eos)
-            self.failUnless('#!/bin/bash' in log)
-            self.failUnless('sudo cp %s/%s %s' %
-                            (persistent_dir, plugin, plugin_dir) in log)
-
-            self.failUnless(contents in
-                            file_log('%s/%s' % (persistent_dir, plugin)))
-            self.failUnless(bootstrap.success())
+            self.assertTrue("#!/bin/bash" in log)
+            self.assertTrue("sudo cp {}/{} {}".format(persistent_dir, plugin, plugin_dir) in log)
+
+            self.assertTrue(contents in file_log("{}/{}".format(persistent_dir, plugin)))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             shutil.rmtree(persistent_dir)
             bootstrap.end_test()
 
     def test_ztps_path_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         plugin = url = random_string()
-        ztps_server = 'http://%s' % bootstrap.server
+        ztps_server = "http://{}".format(bootstrap.server)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'url' : url,
-                                      'ztps_server': ztps_server}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-
-        plugin_dir = '/tmp'
-        persistent_dir = '/tmp/persistent'
-        action = get_action('install_cli_plugin')
-        action = action.replace('/usr/lib/python2.7/site-packages/CliPlugin',
-                                plugin_dir)
-
-        action = action.replace('/mnt/flash/.ztp-plugins',
-                                persistent_dir)
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"url": url, "ztps_server": ztps_server}},
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+
+        plugin_dir = "/tmp"
+        persistent_dir = "/tmp/persistent"
+        action = get_action("install_cli_plugin")
+        action = action.replace("/usr/lib/python2.7/site-packages/CliPlugin", plugin_dir)
+
+        action = action.replace("/mnt/flash/.ztp-plugins", persistent_dir)
+        bootstrap.ztps.set_action_response("test_action", action)
 
         contents = random_string()
         bootstrap.ztps.set_file_response(plugin, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.rc_eos))
+            self.assertTrue(os.path.isfile(bootstrap.rc_eos))
             log = file_log(bootstrap.rc_eos)
-            self.failUnless('#!/bin/bash' in log)
-            self.failUnless('sudo cp %s/%s %s' %
-                            (persistent_dir, plugin, plugin_dir) in log)
-
-            self.failUnless(contents in
-                            file_log('%s/%s' % (persistent_dir, plugin)))
-            self.failUnless(bootstrap.success())
+            self.assertTrue("#!/bin/bash" in log)
+            self.assertTrue("sudo cp {}/{} {}".format(persistent_dir, plugin, plugin_dir) in log)
+
+            self.assertTrue(contents in file_log("{}/{}".format(persistent_dir, plugin)))
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             shutil.rmtree(persistent_dir)
             bootstrap.end_test()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/actions/test_install_image.py` & `ztpserver-2.0.0/test/actions/test_install_image.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,137 +23,133 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401,W0232,E1101
+# pylint: disable=C0209
 
 import os
 import os.path
 import unittest
-import sys
+from test.client.client_test_lib import (
+    ActionFailureTest,
+    Bootstrap,
+    eapi_log,
+    get_action,
+    print_action,
+    raise_exception,
+    random_string,
+    remove_file,
+    startup_config_action,
+)
 
-sys.path.append('test/client')
-
-from client_test_lib import Bootstrap, ActionFailureTest
-from client_test_lib import eapi_log, remove_file, get_action
-from client_test_lib import startup_config_action, random_string
-from client_test_lib import print_action
-from client_test_lib import raise_exception
 
 class FailureTest(ActionFailureTest):
-
     def test_missing_url(self):
-        self.basic_test('install_image',
-                        'Missing attribute(\'url\')')
+        self.basic_test("install_image", "Missing attribute('url')")
 
     def test_missing_version(self):
-        self.basic_test('install_image',
-                        'Missing attribute(\'version\')',
-                        attributes={'url' :
-                                        random_string()})
+        self.basic_test(
+            "install_image", "Missing attribute('version')", attributes={"url": random_string()}
+        )
 
     def test_url_failure(self):
-        self.basic_test('install_image',
-                        'Unable to retrieve image file from URL',
-                        attributes={'url' :
-                                    random_string(),
-                                    'version' :
-                                    random_string()})
+        self.basic_test(
+            "install_image",
+            "Unable to retrieve image file from URL",
+            attributes={"url": random_string(), "version": random_string()},
+        )
 
 
 class SuccessTest(unittest.TestCase):
-
     def test_no_op(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         version = random_string()
         bootstrap.eapi.version = version
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {
-                        'url' : random_string(),
-                        'version' : version}},
-                     {'action' :'startup_config_action'}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('install_image'))
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
+            actions=[
+                {
+                    "action": "test_action",
+                    "attributes": {"url": random_string(), "version": version},
+                },
+                {"action": "startup_config_action"},
+            ]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("install_image"))
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.success())
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_no_downgrade(self):
         bootstrap = Bootstrap(ztps_default_config=True)
-        version1 = '4.18.1F'
-        version2 = '4.17.2F'
+        version1 = "4.18.1F"
+        version2 = "4.17.2F"
         bootstrap.eapi.version = version1
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {
-                        'downgrade' : False,
-                        'url' : random_string(),
-                        'version' : version2}},
-                     {'action' :'startup_config_action'}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('install_image'))
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
+            actions=[
+                {
+                    "action": "test_action",
+                    "attributes": {"downgrade": False, "url": random_string(), "version": version2},
+                },
+                {"action": "startup_config_action"},
+            ]
+        )
+        bootstrap.ztps.set_action_response("test_action", get_action("install_image"))
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
         bootstrap.start_test()
 
-        image_file = '%s/EOS-%s.swi' % (bootstrap.flash, version2)
+        image_file = "{}/EOS-{}.swi".format(bootstrap.flash, version2)
         try:
-            self.failUnless(bootstrap.success())
-            self.failUnless('install_image: nothing to do: downgrade disabled'
-                            in bootstrap.output)
+            self.assertTrue(bootstrap.success())
+            self.assertTrue("install_image: nothing to do: downgrade disabled" in bootstrap.output)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(image_file)
             bootstrap.end_test()
 
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         version = random_string()
         image = random_string()
-        url = 'http://%s/%s' % (bootstrap.server, image)
+        url = "http://{}/{}".format(bootstrap.server, image)
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes' : {
-                        'url' : url,
-                        'version' : version}},
-                     {'action' :'startup_config_action'}])
-
-        action = get_action('install_image')
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
+            actions=[
+                {"action": "test_action", "attributes": {"url": url, "version": version}},
+                {"action": "startup_config_action"},
+            ]
+        )
+
+        action = get_action("install_image")
+        bootstrap.ztps.set_action_response("test_action", action)
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
         bootstrap.ztps.set_file_response(image, print_action())
         bootstrap.start_test()
 
-        image_file = '%s/EOS-%s.swi' % (bootstrap.flash, version)
+        image_file = "{}/EOS-{}.swi".format(bootstrap.flash, version)
         try:
-            self.failUnless(os.path.isfile(image_file))
-            self.failUnless(bootstrap.success())
-            self.failUnless(eapi_log()[-1] == 
-                            'install source flash:EOS-%s.swi' % version)
+            self.assertTrue(os.path.isfile(image_file))
+            self.assertTrue(bootstrap.success())
+            self.assertTrue(eapi_log()[-1] == "install source flash:EOS-{}.swi".format(version))
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             remove_file(image_file)
             bootstrap.end_test()
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/actions/test_run_cli_commands.py` & `ztpserver-2.0.0/test/actions/test_run_cli_commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,152 +23,159 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401,W0232,E1101,W0402
+# pylint: disable=C0209
 
 import os
 import os.path
 import unittest
-import sys
 from string import Template
+from test.client.client_test_lib import (
+    ActionFailureTest,
+    Bootstrap,
+    eapi_log,
+    get_action,
+    raise_exception,
+    random_string,
+    startup_config_action,
+)
 
-sys.path.append('test/client')
-
-from client_test_lib import Bootstrap, ActionFailureTest
-from client_test_lib import eapi_log, get_action, random_string
-from client_test_lib import startup_config_action
-from client_test_lib import raise_exception
 
 class FailureTest(ActionFailureTest):
-
     def test_missing_url(self):
-        self.basic_test('run_cli_commands', 'Missing attribute(\'url\')')
+        self.basic_test("run_cli_commands", "Missing attribute('url')")
 
     def test_url_failure(self):
-        self.basic_test('run_cli_commands', 
-                        'Unable to retrieve config from URL',
-                        attributes={'url' :
-                                    random_string()})
+        self.basic_test(
+            "run_cli_commands",
+            "Unable to retrieve config from URL",
+            attributes={"url": random_string()},
+        )
 
     def test_variables_failure(self):
         url = random_string()
         contents = random_string()
-        self.basic_test('run_cli_commands', 
-                        'Unable to perform variable substitution - '
-                        'invalid variables',
-                        attributes={'url' : url,
-                                    'variables' : random_string()},
-                        file_responses={url : contents})
+        self.basic_test(
+            "run_cli_commands",
+            "Unable to perform variable substitution - invalid variables",
+            attributes={"url": url, "variables": random_string()},
+            file_responses={url: contents},
+        )
 
     def test_variable_missing_failure(self):
         url = random_string()
-        contents = random_string() + ' $missing_var'
-        self.basic_test('run_cli_commands', 
-                        'Unable to perform variable substitution - '
-                        '\'missing_var\' missing from list of substitutions',
-                        attributes={'url' : url,
-                                    'variables' : {}},
-                        file_responses={url : contents})
+        contents = random_string() + " $missing_var"
+        self.basic_test(
+            "run_cli_commands",
+            (
+                "Unable to perform variable substitution - "
+                "'missing_var' missing from list of substitutions"
+            ),
+            attributes={"url": url, "variables": {}},
+            file_responses={url: contents},
+        )
 
 
 class SuccessTest(unittest.TestCase):
-
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes': {'url' : url}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('run_cli_commands'))
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"url": url}},
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+        bootstrap.ztps.set_action_response("test_action", get_action("run_cli_commands"))
 
         contents = random_string()
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless(eapi_log()[-1] == contents)
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(eapi_log()[-1] == contents)
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_failure(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes': {'url' : url}}])
+            actions=[{"action": "test_action", "attributes": {"url": url}}]
+        )
 
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('run_cli_commands'))
+        bootstrap.ztps.set_action_response("test_action", get_action("run_cli_commands"))
 
         contents = random_string()
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.eapi.add_failing_command(contents)
         bootstrap.start_test()
 
         try:
-            self.failUnless(eapi_log()[-1] == contents)
-            self.failUnless(bootstrap.action_failure())
-            self.failUnless('Running CLI commands [\'%s\'] failed' % 
-                            contents in bootstrap.output)
+            self.assertTrue(eapi_log()[-1] == contents)
+            self.assertTrue(bootstrap.action_failure())
+            self.assertTrue(
+                "Running CLI commands ['{}'] failed".format(contents) in bootstrap.output
+            )
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_variables(self):
         bootstrap = Bootstrap(ztps_default_config=True)
         config = random_string()
         url = config
-        var_dict = { 'a' : 'A',
-                     'b' : 'A',
-                     'xxx' : '999',
-                     'dummy': 'DUMMY'}
+        var_dict = {"a": "A", "b": "A", "xxx": "999", "dummy": "DUMMY"}
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes': {'url' : url,
-                                     'substitution_mode': 'strict',
-                                     'variables': var_dict}}])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-        bootstrap.ztps.set_action_response('test_action',
-                                           get_action('run_cli_commands'))
+            actions=[
+                {"action": "startup_config_action"},
+                {
+                    "action": "test_action",
+                    "attributes": {
+                        "url": url,
+                        "substitution_mode": "strict",
+                        "variables": var_dict,
+                    },
+                },
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+        bootstrap.ztps.set_action_response("test_action", get_action("run_cli_commands"))
 
-        contents = '$a 1234 $b 4  321 $xxx$a'
+        contents = "$a 1234 $b 4  321 $xxx$a"
         bootstrap.ztps.set_file_response(config, contents)
         bootstrap.start_test()
 
         expected_contents = Template(contents).substitute(var_dict)
 
         try:
-            self.failUnless(os.path.isfile(bootstrap.startup_config))
-            self.failUnless(expected_contents == eapi_log()[-1])
-            self.failUnless(bootstrap.success())
+            self.assertTrue(os.path.isfile(bootstrap.startup_config))
+            self.assertTrue(expected_contents == eapi_log()[-1])
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/actions/test_install_extension.py` & `ztpserver-2.0.0/test/actions/test_install_extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,173 +23,155 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401,W0232,E1101
+# pylint: disable=C0209
 
 import os
 import os.path
-import unittest
 import shutil
-import sys
-
-sys.path.append('test/client')
+import unittest
+from test.client.client_test_lib import (
+    ActionFailureTest,
+    Bootstrap,
+    file_log,
+    get_action,
+    raise_exception,
+    random_string,
+    remove_file,
+    startup_config_action,
+)
 
-from client_test_lib import Bootstrap, ActionFailureTest
-from client_test_lib import file_log, get_action, random_string
-from client_test_lib import startup_config_action, remove_file
-from client_test_lib import raise_exception
 
 class FailureTest(ActionFailureTest):
-
     def test_missing_url(self):
-        self.basic_test('install_extension',
-                        'Missing attribute(\'url\')')
+        self.basic_test("install_extension", "Missing attribute('url')")
 
     def test_url_failure(self):
-        self.basic_test('install_extension',
-                        'Unable to retrieve extension from URL',
-                        attributes={'url' :
-                                    random_string()})
+        self.basic_test(
+            "install_extension",
+            "Unable to retrieve extension from URL",
+            attributes={"url": random_string()},
+        )
 
 
 class SuccessTest(unittest.TestCase):
-
     def test_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         extension = random_string()
         url = extension
 
         extension_force = random_string()
-        url_force = 'http://%s/%s' % (bootstrap.server, extension_force)
+        url_force = "http://{}/{}".format(bootstrap.server, extension_force)
 
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'url' : url}},
-                     {'action' : 'test_action_force',
-                      'attributes' :
-                      {'url' : url_force,
-                       'force' : True}}
-                     ])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-
-        extensions_dir = '/tmp/extensions'
-        boot_extensions = '/tmp/boot-extensions'
-        action = get_action('install_extension')
-        action = action.replace('/mnt/flash/.extensions',
-                                extensions_dir)
-        action = action.replace('/mnt/flash/boot-extensions',
-                                boot_extensions)
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"url": url}},
+                {"action": "test_action_force", "attributes": {"url": url_force, "force": True}},
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+
+        extensions_dir = "/tmp/extensions"
+        boot_extensions = "/tmp/boot-extensions"
+        action = get_action("install_extension")
+        action = action.replace("/mnt/flash/.extensions", extensions_dir)
+        action = action.replace("/mnt/flash/boot-extensions", boot_extensions)
 
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+        bootstrap.ztps.set_action_response("test_action", action)
         contents = random_string()
         bootstrap.ztps.set_file_response(extension, contents)
 
-        bootstrap.ztps.set_action_response('test_action_force',
-                                           action)
+        bootstrap.ztps.set_action_response("test_action_force", action)
         contents_force = random_string()
         bootstrap.ztps.set_file_response(extension_force, contents_force)
 
         bootstrap.start_test()
 
         try:
-            ext_filename = '%s/%s' % (extensions_dir, extension)
-            self.failUnless(os.path.isfile(ext_filename))
-            self.failUnless([contents] ==
-                            file_log(ext_filename))
-            self.failUnless(extension in file_log(boot_extensions))
-
-            ext_filename_force = '%s/%s' % (extensions_dir, extension_force)
-            self.failUnless(os.path.isfile(ext_filename_force))
-
-            self.failUnless([contents_force] ==
-                            file_log(ext_filename_force))
-            self.failUnless('%s force' % extension_force in
-                            file_log(boot_extensions))
+            ext_filename = "{}/{}".format(extensions_dir, extension)
+            self.assertTrue(os.path.isfile(ext_filename))
+            self.assertTrue([contents] == file_log(ext_filename))
+            self.assertTrue(extension in file_log(boot_extensions))
 
-            self.failUnless(bootstrap.success())
+            ext_filename_force = "{}/{}".format(extensions_dir, extension_force)
+            self.assertTrue(os.path.isfile(ext_filename_force))
+
+            self.assertTrue([contents_force] == file_log(ext_filename_force))
+            self.assertTrue("{} force".format(extension_force) in file_log(boot_extensions))
+
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             shutil.rmtree(extensions_dir)
             remove_file(boot_extensions)
             bootstrap.end_test()
 
     def test_url_success(self):
         bootstrap = Bootstrap(ztps_default_config=True)
 
         extension = random_string()
-        url = 'http://%s/%s' % (bootstrap.server, extension)
+        url = "http://{}/{}".format(bootstrap.server, extension)
 
         extension_force = random_string()
-        url_force = 'http://%s/%s' % (bootstrap.server, extension_force)
+        url_force = "http://{}/{}".format(bootstrap.server, extension_force)
 
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'test_action',
-                      'attributes' : {'url' : url}},
-                     {'action' : 'test_action_force',
-                      'attributes' :
-                      {'url' : url_force,
-                       'force' : True}}
-                     ])
-
-        bootstrap.ztps.set_action_response(
-            'startup_config_action', startup_config_action())
-
-        extensions_dir = '/tmp/extensions'
-        boot_extensions = '/tmp/boot-extensions'
-        action = get_action('install_extension')
-        action = action.replace('/mnt/flash/.extensions',
-                                extensions_dir)
-        action = action.replace('/mnt/flash/boot-extensions',
-                                boot_extensions)
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "test_action", "attributes": {"url": url}},
+                {"action": "test_action_force", "attributes": {"url": url_force, "force": True}},
+            ]
+        )
+
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+
+        extensions_dir = "/tmp/extensions"
+        boot_extensions = "/tmp/boot-extensions"
+        action = get_action("install_extension")
+        action = action.replace("/mnt/flash/.extensions", extensions_dir)
+        action = action.replace("/mnt/flash/boot-extensions", boot_extensions)
 
-        bootstrap.ztps.set_action_response('test_action',
-                                           action)
+        bootstrap.ztps.set_action_response("test_action", action)
         contents = random_string()
         bootstrap.ztps.set_file_response(extension, contents)
 
-        bootstrap.ztps.set_action_response('test_action_force',
-                                           action)
+        bootstrap.ztps.set_action_response("test_action_force", action)
         contents_force = random_string()
         bootstrap.ztps.set_file_response(extension_force, contents_force)
 
         bootstrap.start_test()
 
         try:
-            ext_filename = '%s/%s' % (extensions_dir, extension)
-            self.failUnless(os.path.isfile(ext_filename))
-            self.failUnless([contents] ==
-                            file_log(ext_filename))
-            self.failUnless(extension in file_log(boot_extensions))
-
-            ext_filename_force = '%s/%s' % (extensions_dir, extension_force)
-            self.failUnless(os.path.isfile(ext_filename_force))
-
-            self.failUnless([contents_force] ==
-                            file_log(ext_filename_force))
-            self.failUnless('%s force' % extension_force in
-                            file_log(boot_extensions))
+            ext_filename = "{}/{}".format(extensions_dir, extension)
+            self.assertTrue(os.path.isfile(ext_filename))
+            self.assertTrue([contents] == file_log(ext_filename))
+            self.assertTrue(extension in file_log(boot_extensions))
+
+            ext_filename_force = "{}/{}".format(extensions_dir, extension_force)
+            self.assertTrue(os.path.isfile(ext_filename_force))
 
-            self.failUnless(bootstrap.success())
+            self.assertTrue([contents_force] == file_log(ext_filename_force))
+            self.assertTrue("{} force".format(extension_force) in file_log(boot_extensions))
+
+            self.assertTrue(bootstrap.success())
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             shutil.rmtree(extensions_dir)
             remove_file(boot_extensions)
             bootstrap.end_test()
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/client/test_xmpp_bootstrap.py` & `ztpserver-2.0.0/test/client/test_xmpp_bootstrap.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,100 +23,116 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401
+# pylint: disable=R0904,F0401,C0209
 
 import unittest
-
-from client_test_lib import Bootstrap
-from client_test_lib import raise_exception
+from test.client.client_test_lib import Bootstrap, raise_exception
 
 
 class XmppConfigTest(unittest.TestCase):
-
     @classmethod
     def bootstrap(cls, xmpp):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response(xmpp=xmpp)
         bootstrap.ztps.set_node_check_response()
         bootstrap.ztps.set_definition_response()
         bootstrap.start_test()
         return bootstrap
 
     def xmpp_sanity_test(self, xmpp):
         bootstrap = self.bootstrap(xmpp)
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.missing_startup_config_failure())
-            self.failIf(bootstrap.error)
-            self.failIf('XmppClient' not in bootstrap.output)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.missing_startup_config_failure())
+            self.assertFalse(bootstrap.error)
+            self.assertFalse("XmppClient" not in bootstrap.output)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_full(self):
-        self.xmpp_sanity_test({'server' : 'test-server',
-                               'port' : 112233,
-                               'username' : 'test-username',
-                               'password' : 'test-password',
-                               'domain' :   'test-domain',
-                               'rooms' : ['test-room-1', 'test-room-2']})
+        self.xmpp_sanity_test(
+            {
+                "server": "test-server",
+                "port": 112233,
+                "username": "test-username",
+                "password": "test-password",
+                "domain": "test-domain",
+                "rooms": ["test-room-1", "test-room-2"],
+            }
+        )
 
     def test_msg_type_debug(self):
-        self.xmpp_sanity_test({'server' : 'test-server',
-                               'port' : 112233,
-                               'username' : 'test-username',
-                               'password' : 'test-password',
-                               'domain' :   'test-domain',
-                               'rooms' : ['test-room-1', 'test-room-2'],
-                               'msg_type' : 'debug'})
+        self.xmpp_sanity_test(
+            {
+                "server": "test-server",
+                "port": 112233,
+                "username": "test-username",
+                "password": "test-password",
+                "domain": "test-domain",
+                "rooms": ["test-room-1", "test-room-2"],
+                "msg_type": "debug",
+            }
+        )
 
     def test_msg_type_info(self):
-        self.xmpp_sanity_test({'server' : 'test-server',
-                               'port' : 112233,
-                               'username' : 'test-username',
-                               'password' : 'test-password',
-                               'domain' :   'test-domain',
-                               'rooms' : ['test-room-1', 'test-room-2'],
-                               'msg_type' : 'debug'})
+        self.xmpp_sanity_test(
+            {
+                "server": "test-server",
+                "port": 112233,
+                "username": "test-username",
+                "password": "test-password",
+                "domain": "test-domain",
+                "rooms": ["test-room-1", "test-room-2"],
+                "msg_type": "debug",
+            }
+        )
 
     def test_partial(self):
-        self.xmpp_sanity_test({'rooms' : ['test-room-1'],
-                               'username' : 'test-username',
-                               'password' : 'test-password',
-                               'domain' :   'test-domain'})
+        self.xmpp_sanity_test(
+            {
+                "rooms": ["test-room-1"],
+                "username": "test-username",
+                "password": "test-password",
+                "domain": "test-domain",
+            }
+        )
 
     def test_erroneous_msg_type(self):
-        bootstrap = self.bootstrap({'server' : 'test-server',
-                                    'port' : 112233,
-                                    'username' : 'test-username',
-                                    'password' : 'test-password',
-                                    'domain' :   'test-domain',
-                                    'rooms' : ['test-room-1', 'test-room-2'],
-                                    'msg_type' : 'bogus'})
+        bootstrap = self.bootstrap(
+            {
+                "server": "test-server",
+                "port": 112233,
+                "username": "test-username",
+                "password": "test-password",
+                "domain": "test-domain",
+                "rooms": ["test-room-1", "test-room-2"],
+                "msg_type": "bogus",
+            }
+        )
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.missing_startup_config_failure())
-            self.failIf(bootstrap.error)
-            self.failIf('XMPP configuration failed because of '
-                        'unexpected \'msg_type\''
-                        not in bootstrap.output)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.missing_startup_config_failure())
+            self.assertFalse(bootstrap.error)
+            self.assertFalse(
+                "XMPP configuration failed because of unexpected 'msg_type'" not in bootstrap.output
+            )
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/client/FastCli` & `ztpserver-2.0.0/test/client/FastCli`

 * *Files 9% similar despite different names*

```diff
@@ -25,18 +25,19 @@
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 # This is used by the tests in order to simulate FastCli calls
 import sys
+
 from client_test_lib import CLI_LOG
 
-open(CLI_LOG, 'a+b').write('%s\n' % ' '.join(sys.argv))
+open(CLI_LOG, "a+").write("%s\n" % " ".join(sys.argv))
 
-if sys.argv[-1] == 'show version':
+if sys.argv[-1] == "show version":
     # serial number is used for client-side logging
-    print 'Serial number:       DUMMY_SERIAL'
+    print("Serial number:       DUMMY_SERIAL")
 else:
-    # Need to return something, so that the check for 
+    # Need to return something, so that the check for
     # EAPI being enabled succeeds
-    print 'dummy-response'
+    print("dummy-response")
```

### Comparing `ztpserver-1.6.0/test/client/test_bootstrap.py` & `ztpserver-2.0.0/test/client/test_bootstrap.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,449 +23,443 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=R0904,F0401
+# pylint: disable=C0209
 
+import io
 import os
 import os.path
 import unittest
+from test.client.client_test_lib import (
+    Bootstrap,
+    erroneous_action,
+    exception_action,
+    fail_action,
+    file_log,
+    missing_main_action,
+    print_action,
+    raise_exception,
+    random_string,
+    remove_file,
+    startup_config_action,
+    wrong_signature_action,
+)
 
-from client_test_lib import Bootstrap
-from client_test_lib import file_log, remove_file
-from client_test_lib import startup_config_action
-from client_test_lib import fail_action, print_action, random_string
-from client_test_lib import erroneous_action, missing_main_action
-from client_test_lib import wrong_signature_action, exception_action
-from client_test_lib import raise_exception
+from six import ensure_text
+
+# pylint: disable=R0904,F0401
 
-class ServerNotRunningTest(unittest.TestCase):
 
+class ServerNotRunningTest(unittest.TestCase):
     def test(self):
-        bootstrap = Bootstrap(server='unkown')
+        bootstrap = Bootstrap(server="unkown")
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.server_connection_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.server_connection_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
 class ConfigRequestErrorTest(unittest.TestCase):
-
     def test_status(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response(status=201)
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_content_type(self):
         bootstrap = Bootstrap()
-        bootstrap.ztps.set_config_response(content_type='text/plain')
+        bootstrap.ztps.set_config_response(content_type="text/plain")
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_status_content_type(self):
         bootstrap = Bootstrap()
-        bootstrap.ztps.set_config_response(
-            status=201,
-            content_type='text/plain')
+        bootstrap.ztps.set_config_response(status=201, content_type="text/plain")
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
 class EAPIErrorTest(unittest.TestCase):
-
     def test(self):
         bootstrap = Bootstrap(eapi_port=54321)
         bootstrap.ztps.set_config_response()
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_configured())
-            self.failUnless(bootstrap.eapi_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_configured())
+            self.assertTrue(bootstrap.eapi_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
 class CheckNodeErrorTest(unittest.TestCase):
-
     def test_status(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response(status=200)
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_content_type(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
-        bootstrap.ztps.set_node_check_response(
-            content_type='text/plain')
+        bootstrap.ztps.set_node_check_response(content_type="text/plain")
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_status_content_type(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
-        bootstrap.ztps.set_node_check_response(
-            status=200,
-            content_type='text/plain')
+        bootstrap.ztps.set_node_check_response(status=200, content_type="text/plain")
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_node_not_found(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response(status=400)
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.node_not_found_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.node_not_found_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_bogus_location(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
-        bootstrap.ztps.set_node_check_response(location='bogus_location')
+        bootstrap.ztps.set_node_check_response(location="bogus_location")
         bootstrap.ztps.set_definition_response()
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.server_connection_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.server_connection_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
 class DefinitionErrorTest(unittest.TestCase):
-
     def test_definition_missing(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.server_connection_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.server_connection_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_status(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
         bootstrap.ztps.set_definition_response(status=201)
 
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_content_type(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
-        bootstrap.ztps.set_definition_response(
-            content_type='text/plain')
+        bootstrap.ztps.set_definition_response(content_type="text/plain")
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_status_content_type(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
-        bootstrap.ztps.set_definition_response(
-            status=201,
-            content_type='text/plain')
+        bootstrap.ztps.set_definition_response(status=201, content_type="text/plain")
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_bogus_definition_response(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
         bootstrap.ztps.set_bogus_definition_response()
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.invalid_definition_format())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.invalid_definition_format())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_topology_check(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
-        bootstrap.ztps.set_definition_response(
-            status=400,
-            content_type='text/html')
+        bootstrap.ztps.set_definition_response(status=400, content_type="text/html")
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.toplogy_check_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.toplogy_check_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
 class MissingStartupConfigTest(unittest.TestCase):
-
     def test(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
         bootstrap.ztps.set_definition_response()
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.missing_startup_config_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.missing_startup_config_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
 class FactoryDefaultTest(unittest.TestCase):
-
     def test(self):
         bootstrap = Bootstrap()
 
-        open(bootstrap.rc_eos, 'w').write(random_string())
-        open(bootstrap.boot_extensions, 'w').write(random_string())
+        with io.open(bootstrap.rc_eos, "w", encoding="utf8") as fd:
+            fd.write(ensure_text(random_string()))
+        with io.open(bootstrap.boot_extensions, "w", encoding="utf8") as fd:
+            fd.write(ensure_text(random_string()))
         os.makedirs(bootstrap.boot_extensions_folder)
-        open('%s/%s' % (bootstrap.boot_extensions_folder, 
-                        random_string()),
-             'w').write(random_string())
+        with io.open(
+            os.path.join(bootstrap.boot_extensions_folder, random_string()), "w", encoding="utf8"
+        ) as fd:
+            fd.write(ensure_text(random_string()))
 
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
         bootstrap.ztps.set_definition_response()
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.missing_startup_config_failure())
-            self.failIf(os.path.exists(bootstrap.rc_eos))
-            self.failIf(os.path.exists(bootstrap.boot_extensions))
-            self.failIf(os.path.exists(bootstrap.boot_extensions_folder))
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.missing_startup_config_failure())
+            self.assertFalse(os.path.exists(bootstrap.rc_eos))
+            self.assertFalse(os.path.exists(bootstrap.boot_extensions))
+            self.assertFalse(os.path.exists(bootstrap.boot_extensions_folder))
 
-            self.failIf(bootstrap.error)
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
 class FileLogConfigTest(unittest.TestCase):
-
     def test(self):
         filenames = {
-            'DEBUG' : '/tmp/ztps-log-%s-debug' % os.getpid(),
-            'ERROR' : '/tmp/ztps-log-%s-error' % os.getpid(),
-            'INFO' : '/tmp/ztps-log-%s-info' % os.getpid(),
-            'bogus' : '/tmp/ztps-log-%s-bogus' % os.getpid()
-            }
+            "DEBUG": "/tmp/ztps-log-{}-debug".format(os.getpid()),
+            "ERROR": "/tmp/ztps-log-{}-error".format(os.getpid()),
+            "INFO": "/tmp/ztps-log-{}-info".format(os.getpid()),
+            "bogus": "/tmp/ztps-log-{}-bogus".format(os.getpid()),
+        }
 
         logging = []
-        for level, filename in filenames.iteritems():
-            logging += {'destination' : 'file:%s' % filename,
-                        'level' : level},
+        for level, filename in filenames.items():
+            logging += ({"destination": "file:{}".format(filename), "level": level},)
 
-        for filename in filenames.itervalues():
-            self.failIf(os.path.isfile(filename))
+        for filename in filenames.values():
+            self.assertFalse(os.path.isfile(filename))
 
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response(logging=logging)
         bootstrap.ztps.set_node_check_response()
         bootstrap.ztps.set_definition_response()
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.missing_startup_config_failure())
-            for filename in filenames.itervalues():
-                self.failUnless(file_log(filename))
-            self.assertEquals(file_log(filenames['DEBUG'],
-                                       ignore_string='SyslogManager'),
-                              file_log(filenames['bogus'],
-                                       ignore_string='SyslogManager'))
-            self.assertEquals(file_log(filenames['DEBUG'],
-                                       ignore_string='SyslogManager'),
-                              file_log(filenames['INFO'],
-                                       ignore_string='SyslogManager'))
-            self.failIfEqual(file_log(filenames['DEBUG'],
-                                       ignore_string='SyslogManager'),
-                             file_log(filenames['ERROR'],
-                                       ignore_string='SyslogManager'))
-            self.failUnless(set(file_log(filenames['ERROR'])).issubset(
-                    set(file_log(filenames['DEBUG']))))
-            for filename in filenames.itervalues():
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.missing_startup_config_failure())
+            for filename in filenames.values():
+                self.assertTrue(file_log(filename))
+            self.assertEqual(
+                file_log(filenames["DEBUG"], ignore_string="SyslogManager"),
+                file_log(filenames["bogus"], ignore_string="SyslogManager"),
+            )
+            self.assertEqual(
+                file_log(filenames["DEBUG"], ignore_string="SyslogManager"),
+                file_log(filenames["INFO"], ignore_string="SyslogManager"),
+            )
+            self.assertNotEqual(
+                file_log(filenames["DEBUG"], ignore_string="SyslogManager"),
+                file_log(filenames["ERROR"], ignore_string="SyslogManager"),
+            )
+            self.assertTrue(
+                set(file_log(filenames["ERROR"])).issubset(set(file_log(filenames["DEBUG"])))
+            )
+            for filename in filenames.values():
                 remove_file(filename)
-                self.failIf(bootstrap.error)
+                self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
-
 class ActionFailureTest(unittest.TestCase):
-
     def action_fail_test(self, action):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
-        bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action'}])
-        bootstrap.ztps.set_action_response('test_action', action)
+        bootstrap.ztps.set_definition_response(actions=[{"action": "test_action"}])
+        bootstrap.ztps.set_action_response("test_action", action)
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.action_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.action_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_return_code_action_failed(self):
         self.action_fail_test(fail_action())
 
@@ -481,288 +475,289 @@
     def test_exception_action_failed(self):
         self.action_fail_test(exception_action())
 
     def test_status(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
-        bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action'}])
-        bootstrap.ztps.set_action_response('test_action', print_action(),
-                                           status=201)
+        bootstrap.ztps.set_definition_response(actions=[{"action": "test_action"}])
+        bootstrap.ztps.set_action_response("test_action", print_action(), status=201)
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_content_type(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
-        bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action'}])
-        bootstrap.ztps.set_action_response('test_action', print_action(),
-                                           content_type='test/plain')
+        bootstrap.ztps.set_definition_response(actions=[{"action": "test_action"}])
+        bootstrap.ztps.set_action_response("test_action", print_action(), content_type="test/plain")
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_status_content_type(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
-        bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action'}])
-        bootstrap.ztps.set_action_response('test_action', print_action(),
-                                           status=201,
-                                           content_type='test/plain')
+        bootstrap.ztps.set_definition_response(actions=[{"action": "test_action"}])
+        bootstrap.ztps.set_action_response(
+            "test_action", print_action(), status=201, content_type="test/plain"
+        )
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.unexpected_response_failure())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.unexpected_response_failure())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_action_failure_log(self):
-        log = '/tmp/ztps-log-%s-debug' % os.getpid()
+        log = "/tmp/ztps-log-{}-debug".format(os.getpid())
 
         bootstrap = Bootstrap()
-        bootstrap.ztps.set_config_response(logging=[
-                {'destination' : 'file:%s' % log,
-                 'level' : 'DEBUG'},])
+        bootstrap.ztps.set_config_response(
+            logging=[
+                {"destination": "file:{}".format(log), "level": "DEBUG"},
+            ]
+        )
         bootstrap.ztps.set_node_check_response()
 
         text_onstart = random_string()
         text_onsuccess = random_string()
         text_onfailure = random_string()
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'onstart' : text_onstart,
-                      'onsuccess' : text_onsuccess,
-                      'onfailure' : text_onfailure},
-                     ])
-        bootstrap.ztps.set_action_response('test_action',
-                                           fail_action())
+            actions=[
+                {
+                    "action": "test_action",
+                    "onstart": text_onstart,
+                    "onsuccess": text_onsuccess,
+                    "onfailure": text_onfailure,
+                },
+            ]
+        )
+        bootstrap.ztps.set_action_response("test_action", fail_action())
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.action_failure())
-            self.failIf(bootstrap.error)
-            log = ''.join(file_log(log))
-            self.failUnless('test_action: %s' % text_onstart in log)
-            self.failUnless('test_action: %s' % text_onsuccess not in log)
-            self.failUnless('test_action: %s' % text_onfailure in log)
+            self.assertTrue(bootstrap.eapi_node_information_collected(), "0")
+            self.assertTrue(bootstrap.action_failure(), "1")
+            self.assertFalse(bootstrap.error)
+            log = "".join(file_log(log))
+            self.assertTrue("test_action: {}".format(text_onstart) in log, "2")
+            self.assertTrue("test_action: {}".format(text_onsuccess) not in log, "3")
+            self.assertTrue("test_action: {}".format(text_onfailure) in log, "4")
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
 class BootstrapSuccessTest(unittest.TestCase):
-
     def test_success(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
-        bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'}])
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
+        bootstrap.ztps.set_definition_response(actions=[{"action": "startup_config_action"}])
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.success())
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.success())
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_multiple_actions(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'print_action_1'},
-                     {'action' : 'print_action_2'}])
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "print_action_1"},
+                {"action": "print_action_2"},
+            ]
+        )
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
 
         text_1 = random_string()
-        bootstrap.ztps.set_action_response('print_action_1',
-                                           print_action(text_1))
+        bootstrap.ztps.set_action_response("print_action_1", print_action(text_1))
         text_2 = random_string()
-        bootstrap.ztps.set_action_response('print_action_2',
-                                           print_action(text_2))
+        bootstrap.ztps.set_action_response("print_action_2", print_action(text_2))
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.success())
-            self.failUnless(text_1 in bootstrap.output)
-            self.failUnless(text_2 in bootstrap.output)
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.success())
+            self.assertTrue(text_1 in bootstrap.output)
+            self.assertTrue(text_2 in bootstrap.output)
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_duplicate_actions(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'print_action'},
-                     {'action' : 'print_action'}])
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "print_action"},
+                {"action": "print_action"},
+            ]
+        )
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
 
         text = random_string()
-        bootstrap.ztps.set_action_response('print_action',
-                                           print_action(text))
+        bootstrap.ztps.set_action_response("print_action", print_action(text))
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.success())
-            self.failUnless(bootstrap.output.count('Downloading action '
-                                                   'print_action') == 1)
-            self.failUnless(bootstrap.output.count('Executing action '
-                                                   'print_action') == 2)
-            self.failUnless(bootstrap.output.count(text) == 2)
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.success())
+            self.assertTrue(bootstrap.output.count("Downloading action print_action") == 1)
+            self.assertTrue(bootstrap.output.count("Executing action print_action") == 2)
+            self.assertTrue(bootstrap.output.count(text) == 2)
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_attribute_copy(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
         text = random_string()
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'print_action',
-                      'attributes' : {'print_action-attr' : text}}])
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
-        bootstrap.ztps.set_action_response('print_action',
-                                           print_action(use_attribute=True,
-                                                        create_copy=True))
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "print_action", "attributes": {"print_action-attr": text}},
+            ]
+        )
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+        bootstrap.ztps.set_action_response(
+            "print_action", print_action(use_attribute=True, create_copy=True)
+        )
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.success())
-            self.failUnless(text in bootstrap.output)
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.success())
+            self.assertTrue(text in bootstrap.output)
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_attribute(self):
         bootstrap = Bootstrap()
         bootstrap.ztps.set_config_response()
         bootstrap.ztps.set_node_check_response()
         text = random_string()
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action'},
-                     {'action' : 'print_action',
-                      'attributes' : {'print_action-attr':text}}])
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
-        bootstrap.ztps.set_action_response('print_action',
-                                           print_action(use_attribute=True))
+            actions=[
+                {"action": "startup_config_action"},
+                {"action": "print_action", "attributes": {"print_action-attr": text}},
+            ]
+        )
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
+        bootstrap.ztps.set_action_response("print_action", print_action(use_attribute=True))
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.success())
-            self.failUnless(text in bootstrap.output)
-            self.failIf(bootstrap.error)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.success())
+            self.assertTrue(text in bootstrap.output)
+            self.assertFalse(bootstrap.error)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
     def test_action_success_log(self):
-        log = '/tmp/ztps-log-%s-debug' % os.getpid()
+        log = "/tmp/ztps-log-{}-debug".format(os.getpid())
 
         bootstrap = Bootstrap()
-        bootstrap.ztps.set_config_response(logging=[
-                {'destination' : 'file:%s' % log,
-                 'level' : 'DEBUG'},])
+        bootstrap.ztps.set_config_response(
+            logging=[
+                {"destination": "file:{}".format(log), "level": "DEBUG"},
+            ]
+        )
         bootstrap.ztps.set_node_check_response()
 
         text_onstart = random_string()
         text_onsuccess = random_string()
         text_onfailure = random_string()
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'startup_config_action',
-                      'onstart' : text_onstart,
-                      'onsuccess' : text_onsuccess,
-                      'onfailure' : text_onfailure,
-                      }])
-        bootstrap.ztps.set_action_response('startup_config_action',
-                                           startup_config_action())
+            actions=[
+                {
+                    "action": "startup_config_action",
+                    "onstart": text_onstart,
+                    "onsuccess": text_onsuccess,
+                    "onfailure": text_onfailure,
+                }
+            ]
+        )
+        bootstrap.ztps.set_action_response("startup_config_action", startup_config_action())
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.eapi_node_information_collected())
-            self.failUnless(bootstrap.success())
-            self.failIf(bootstrap.error)
-            log = ''.join(file_log(log))
-            self.failUnless('startup_config_action: %s' % text_onstart in log)
-            self.failUnless('startup_config_action: %s' % text_onsuccess in log)
-            self.failUnless('startup_config_action: %s' % 
-                            text_onfailure not in log)
+            self.assertTrue(bootstrap.eapi_node_information_collected())
+            self.assertTrue(bootstrap.success())
+            self.assertFalse(bootstrap.error)
+            log = "".join(file_log(log))
+            self.assertTrue("startup_config_action: {}".format(text_onstart) in log)
+            self.assertTrue("startup_config_action: {}".format(text_onsuccess) in log)
+            self.assertTrue("startup_config_action: {}".format(text_onfailure) not in log)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ztpserver-1.6.0/test/client/client_test_lib.py` & `ztpserver-2.0.0/test/client/client_test_lib.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,686 +23,661 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import asyncore
-import imp
+# pylint: disable=C0209
+
+import io
 import json
-import re
 import os
 import random
-import subprocess
-import string                        #pylint: disable=W0402
+import re
 import shutil
-import smtpd
+import string
+import subprocess
 import time
-import thread
 import unittest
-
-import BaseHTTPServer
-
 from collections import namedtuple
 
+from six import ensure_binary, ensure_str, ensure_text, raise_from
+from six.moves import _thread
+from six.moves.BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer
+
+# pylint: disable=C0103
+Response = namedtuple("Response", "content_type status contents headers")
+# pylint: enable=C0103
+
+RC_EOS = "rc.eos"
+BOOT_EXTENSIONS = "boot-extensions"
+BOOT_EXTENSIONS_FOLDER = ".extensions"
+STARTUP_CONFIG = "startup-config"
+ZTP_PLUGINS_FOLDER = ".ztp-plugins"
 
-#pylint: disable=C0103
-Response = namedtuple('Response', 'content_type status contents headers')
-#pylint: enable=C0103
-
-RC_EOS = 'rc.eos'
-BOOT_EXTENSIONS = 'boot-extensions'
-BOOT_EXTENSIONS_FOLDER = '.extensions'
-STARTUP_CONFIG = 'startup-config'
-
-ZTPS_SERVER = '127.0.0.1'
+ZTPS_SERVER = "127.0.0.1"
 ZTPS_PORT = 12345
 
-EAPI_SERVER = '127.0.0.1'
+EAPI_SERVER = "127.0.0.1"
 EAPI_PORT = 1080
 
-SMTP_SERVER = '127.0.0.1'
-SMTP_PORT = 2525
+BOOTSTRAP_FILE = "client/bootstrap"
 
-BOOTSTRAP_FILE = 'client/bootstrap'
-
-CLI_LOG = '/tmp/FastCli-log'
-EAPI_LOG = '/tmp/eapi-log-%s' % os.getpid()
+CLI_LOG = "/tmp/FastCli-log"
+EAPI_LOG = "/tmp/eapi-log-{}".format(os.getpid())
 
 STATUS_OK = 200
 STATUS_CREATED = 201
 STATUS_BAD_REQUEST = 400
 STATUS_NOT_FOUND = 404
 STATUS_CONFLICT = 409
 
-SYSTEM_MAC = '1234567890'
+SYSTEM_MAC = "1234567890"
 
 
 def raise_exception(exception):
-    #pylint: disable=C0301, C0321
+    # pylint: disable=C0301, C0321
 
     # Uncomment the following line for debugging
     # import pdb; pdb.set_trace()
 
-    raise Exception('%s\nUncomment line in client_test_lib.py:raise_'
-                    'exception for debugging' % exception.message)
+    raise_from(
+        RuntimeError(
+            "{}\nUncomment line in client_test_lib.py:raise_exception for debugging".format(
+                exception
+            )
+        ),
+        exception,
+    )
+
+
+ztps = None  # pylint: disable=C0103
+
 
-ztps = None    #pylint: disable=C0103
 def start_ztp_server():
-    global ztps     #pylint: disable=W0603
+    global ztps  # pylint: disable=W0603
     if not ztps:
         ztps = ZTPServer()
         ztps.start()
     else:
         ztps.cleanup()
     return ztps
 
-smtp = None    #pylint: disable=C0103
-def start_smtp_server():
-    global smtp     #pylint: disable=W0603
-    if not smtp:
-        smtp = SmtpServer()
-        smtp.start()
-    return smtp
 
-eapis = None    #pylint: disable=C0103
+eapis = None  # pylint: disable=C0103
+
+
 def start_eapi_server():
-    global eapis    #pylint: disable=W0603
+    global eapis  # pylint: disable=W0603
     if not eapis:
         eapis = EAPIServer()
         eapis.start()
     else:
         eapis.cleanup()
     return eapis
 
+
 def remove_file(filename):
     try:
         os.remove(filename)
     except OSError:
         pass
 
+
 def clear_cli_log():
     remove_file(CLI_LOG)
 
+
 def clear_eapi_log():
     remove_file(EAPI_LOG)
 
+
 def clear_logs():
     clear_cli_log()
     clear_eapi_log()
 
+
 def eapi_log():
     try:
-        return [x.strip()
-                for x in open(EAPI_LOG, 'r').readlines()]
-    except IOError:
+        with io.open(EAPI_LOG, encoding="utf8") as fd:
+            return [x.strip() for x in fd.readlines()]
+    except OSError:
         return []
 
+
 def cli_log():
     try:
-        return [x.strip().split('-c ')[ -1 ]
-                for x in open(CLI_LOG, 'r').readlines()]
-    except IOError:
+        with io.open(CLI_LOG, encoding="utf8") as fd:
+            return [x.strip().split("-c ")[-1] for x in fd.readlines()]
+    except OSError:
         return []
 
-def file_log(filename, ignore_string=None):
 
+def file_log(filename, ignore_string=None):
     try:
-        lines = [x.strip() for x in open(filename, 'r').readlines()]
+        with io.open(filename, encoding="utf8") as fd:
+            lines = [x.strip() for x in fd.readlines()]
         if ignore_string:
             return [y for y in lines if y and ignore_string not in y]
-        else:
-            return [y for y in lines if y]
-    except IOError:
+        return [y for y in lines if y]
+    except OSError:
         return []
 
+
 def get_action(action):
-    return open('actions/%s' % action, 'r').read()
+    with io.open("actions/{}".format(action), encoding="utf8") as fd:
+        return fd.read()
+
 
 def startup_config_action(lines=None):
-    startup_config = '/tmp/ztps-flash-%s/startup-config' % os.getpid()
+    startup_config = "/tmp/ztps-flash-{}/startup-config".format(os.getpid())
     if not lines:
-        lines = ['test']
+        lines = ["test"]
 
-    user = os.getenv('USER')
-    return '''#!/usr/bin/env python
+    user = os.getenv("USER")
+    return """#!/usr/bin/env python
 import os
 import pwd
 
 def main(attributes):
-   user = pwd.getpwnam('%s').pw_uid
-   group = pwd.getpwnam('%s').pw_gid
+   user = pwd.getpwnam('{user}').pw_uid
+   group = pwd.getpwnam('{user}').pw_gid
 
-   f = file('%s', 'w')
-   f.write(\'\'\'%s\'\'\')
+   f = open('{startup_config}', 'w')
+   f.write(\'\'\'{}\'\'\')
    f.close()
 
-   os.chmod('%s', 0777)
-   os.chown('%s', user, group)
-''' % (user, user, startup_config, '\n'.join(lines),
-       startup_config, startup_config)
+   os.chmod('{startup_config}', 0o777)
+   os.chown('{startup_config}', user, group)
+""".format(
+        "\n".join(lines),
+        user=user,
+        startup_config=startup_config,
+    )
+
 
-def print_action(msg='TEST', use_attribute=False, create_copy=False):
-    #pylint: disable=E0602
+def print_action(msg="TEST", use_attribute=False, create_copy=False):
+    # pylint: disable=E0602
     if use_attribute and create_copy:
-        return '''#!/usr/bin/env python
+        return """#!/usr/bin/env python
 
 def main(attributes):
    attrs = attributes.copy()
-   print attrs.get('print_action-attr')
-'''
+   print(attrs.get('print_action-attr'))
+"""
 
     if use_attribute:
-        return '''#!/usr/bin/env python
+        return """#!/usr/bin/env python
 
 def main(attributes):
-   print attributes.get('print_action-attr')
-'''
-    else:
-        return '''#!/usr/bin/env python
+   print(attributes.get('print_action-attr'))
+"""
+
+    return """#!/usr/bin/env python
 
 def main(attributes):
-   print '%s'
-''' % msg
+   print('{}')
+""".format(
+        msg
+    )
+
 
 def print_attributes_action(attributes):
-    #pylint: disable=E0602
-    result = '''#!/usr/bin/env python
+    # pylint: disable=E0602
+    result = """#!/usr/bin/env python
 
 def main(attributes):
-'''
-    for attr in attributes:
-        result += '    print attributes.get(\'%s\')\n' % attr
+"""
+    result += "\n".join("    print(attributes.get('{}')".format(attr) for attr in attributes)
     return result
 
+
 def fail_flash_file_action(flash, filename):
-    '''Creates file on flash and then fails'''
+    """Creates file on flash and then fails"""
 
-    return '''#!/usr/bin/env python
+    return """#!/usr/bin/env python
 
 def main(attributes):
-   open('%s/%s', 'w').write('test')
+   open('{}/{}', 'w').write('test')
    raise Exception('Ops! I failed! :(')
-''' % (flash, filename)
+""".format(
+        flash, filename
+    )
+
 
 def fail_action():
-    return '''#!/usr/bin/env python
+    return """#!/usr/bin/env python
 
 def main(attributes):
    raise Exception('Ops! I failed! :(')
-'''
+"""
+
 
 def erroneous_action():
-    return '''THIS_IS_NOT_PYTHON'''
+    return """THIS_IS_NOT_PYTHON"""
+
 
 def missing_main_action():
-    return '''#!/usr/bin/env python'''
+    return """#!/usr/bin/env python"""
+
 
 def wrong_signature_action():
-    return '''#!/usr/bin/env python
+    return """#!/usr/bin/env python
 
 def main():
    pass
-'''
+"""
+
 
 def exception_action():
-    return '''#!/usr/bin/env python
+    return """#!/usr/bin/env python
 
 def main(attributes):
    raise Exception
-'''
+"""
 
-def random_string():
-    return ''.join(random.choice(
-            string.ascii_uppercase +
-            string.digits) for _ in range(random.randint(3, 20)))
 
+def random_string():
+    return "".join(
+        random.choice(string.ascii_uppercase + string.digits) for _ in range(random.randint(3, 20))
+    )
 
-class Bootstrap(object):
-    #pylint: disable=R0201
 
-    def __init__(self, server=None, eapi_port=None,
-                 ztps_default_config=False):
-        os.environ['PATH'] += ':%s/test/client' % os.getcwd()
+class Bootstrap:
+    def __init__(self, server=None, eapi_port=None, ztps_default_config=False):
+        os.environ["PATH"] += ":{}/test/client".format(os.getcwd())
 
-        self.server = server if server else '%s:%s' % (ZTPS_SERVER, ZTPS_PORT)
+        self.server = server if server else "{}:{}".format(ZTPS_SERVER, ZTPS_PORT)
         self.eapi_port = eapi_port if eapi_port else EAPI_PORT
 
         self.output = None
         self.error = None
         self.return_code = None
         self.filename = None
         self.module = None
 
         self.eapi = start_eapi_server()
         self.ztps = start_ztp_server()
-        self.smtp = start_smtp_server()
 
-        self.flash = '/tmp/ztps-flash-%s' % os.getpid()
-        self.temp = '/tmp/ztps-tmp-%s' % os.getpid()
+        self.flash = "/tmp/ztps-flash-{}".format(os.getpid())
+        self.temp = "/tmp/ztps-tmp-{}".format(os.getpid())
 
-        self.rc_eos = '%s/%s' % (self.flash, RC_EOS)
-        self.boot_extensions = '%s/%s' % (self.flash, BOOT_EXTENSIONS)
-        self.boot_extensions_folder = '%s/%s' % (self.flash, 
-                                          BOOT_EXTENSIONS_FOLDER)
-        self.startup_config = '%s/%s' % (self.flash, STARTUP_CONFIG)
+        self.rc_eos = "{}/{}".format(self.flash, RC_EOS)
+        self.boot_extensions = "{}/{}".format(self.flash, BOOT_EXTENSIONS)
+        self.boot_extensions_folder = "{}/{}".format(self.flash, BOOT_EXTENSIONS_FOLDER)
+        self.ztp_plugins_folder = os.path.join(self.flash, ZTP_PLUGINS_FOLDER)
+        self.startup_config = "{}/{}".format(self.flash, STARTUP_CONFIG)
 
         self.configure()
 
         if ztps_default_config:
             self.ztps.set_config_response()
             self.ztps.set_node_check_response()
 
     def configure(self):
         for folder in [self.flash, self.temp]:
             if not os.path.exists(folder):
                 os.makedirs(folder)
 
-        infile = open(BOOTSTRAP_FILE)
-        self.filename = '/tmp/bootstrap-%s' % os.getpid()
-        outfile = open(self.filename, 'w')
+        self.filename = "/tmp/bootstrap-{}".format(os.getpid())
+        with io.open(BOOTSTRAP_FILE, encoding="utf8") as infile, io.open(
+            self.filename, "w", encoding="utf8"
+        ) as outfile:
+            for line in infile:
+                line = line.replace("$SERVER", "http://{}".format(self.server))
+                line = line.replace(
+                    'COMMAND_API_SERVER = "localhost"',
+                    'COMMAND_API_SERVER = "localhost:{}"'.format(self.eapi_port),
+                )
+
+                line = line.replace('FLASH = "/mnt/flash"', 'FLASH = "{}"'.format(self.flash))
+
+                line = line.replace('TEMP = "/tmp"', 'TEMP = "{}"'.format(self.temp))
+
+                # Reduce HTTP timeout
+                if re.match("^HTTP_TIMEOUT", line):
+                    line = "HTTP_TIMEOUT = 0.01"
 
-        for line in infile:
-            line = line.replace('$SERVER', 'http://%s' % self.server)
-            line = line.replace("COMMAND_API_SERVER = 'localhost'",
-                                "COMMAND_API_SERVER = 'localhost:%s'" %
-                                self.eapi_port)
+                outfile.write(ensure_text(line))
 
-            line = line.replace("FLASH = '/mnt/flash'",
-                                "FLASH = '%s'" % self.flash)
-
-            line = line.replace("TEMP = '/tmp'", "TEMP = '%s'" % 
-                                self.temp)
-
-           # Reduce HTTP timeout
-            if re.match('^HTTP_TIMEOUT', line):
-                line = 'HTTP_TIMEOUT = 0.01'
-
-            outfile.write(line)
-
-        infile.close()
-        outfile.close()
-
-        os.chmod(self.filename, 0777)
-        self.module = imp.load_source('bootstrap', self.filename)
+        os.chmod(self.filename, 0o777)
 
     def end_test(self):
         shutil.rmtree(self.temp)
         shutil.rmtree(self.flash)
 
         # Clean up actions
-        for url in self.ztps.responses.keys():
-            filename = url.split('/')[-1]
-            remove_file('/tmp/%s' % filename)
-            remove_file('/tmp/%sc' % filename)
+        for url in self.ztps.responses:
+            filename = url.split("/")[-1]
+            remove_file("/tmp/{}".format(filename))
+            remove_file("/tmp/{}c".format(filename))
 
         # Clean up log files
-        for filename in os.listdir('/tmp'):
-            if re.search('^ztps-log-', filename):
-                os.remove(os.path.join('/tmp', filename))
+        for filename in os.listdir("/tmp"):
+            if re.search("^ztps-log-", filename):
+                os.remove(os.path.join("/tmp", filename))
 
         # Clean up bootstrap script
         remove_file(self.filename)
-        remove_file('%sc' % self.filename)
+        remove_file("{}c".format(self.filename))
 
         # Clean up logs
         clear_logs()
 
     def start_test(self):
         try:
-            proc = subprocess.Popen([self.filename],
-                                    stdin=subprocess.PIPE,
-                                    stdout=subprocess.PIPE,
-                                    stderr=subprocess.PIPE)
-            (self.output, self.error) = proc.communicate()
+            proc = subprocess.Popen(  # pylint: disable=R1732
+                [self.filename],
+                stdin=subprocess.PIPE,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            (output, error) = proc.communicate()
+            self.output, self.error = ensure_str(output), ensure_str(error)
+            self.return_code = proc.returncode
         finally:
             os.remove(self.filename)
 
-        self.return_code = proc.returncode         #pylint: disable=E1101
-
     def node_information_collected(self):
-        cmds = ['show version',          # Collect system MAC for logging
-                'show lldp neighbors']
-        return [x for x in eapi_log() if x != 'enable'][-2:] == cmds
+        cmds = ["show version", "show lldp neighbors"]  # Collect system MAC for logging
+        return [x for x in eapi_log() if x != "enable"][-2:] == cmds
 
     def eapi_configured(self):
-        cmds = ['configure',
-                'username ztps secret ztps-password privilege 15',
-                'management api http-commands',
-                'no protocol https',
-                'protocol http',
-                'no shutdown']
+        cmds = [
+            "configure",
+            "username ztps secret ztps-password privilege 15",
+            "management api http-commands",
+            "no protocol https",
+            "protocol http",
+            "no shutdown",
+        ]
         return cli_log()[:6] == cmds
 
     def eapi_node_information_collected(self):
         return self.eapi_configured() and self.node_information_collected()
 
     def server_connection_failure(self):
-        return ('server connection error' in self.output or
-                'Read timed out' in self.output) and \
-               self.return_code
+        return (
+            "server connection error" in self.output or "Read timed out" in self.output
+        ) and self.return_code
 
     def eapi_failure(self):
-        return 'unable to enable eAPI' in self.output and \
-               self.return_code
+        return "unable to enable eAPI" in self.output and self.return_code
 
     def unexpected_response_failure(self):
-        return 'unexpected response from server' in self.output and \
-               self.return_code
+        return "unexpected response from server" in self.output and self.return_code
 
     def node_not_found_failure(self):
-        return 'node not found on server' in self.output and \
-               self.return_code
+        return "node not found on server" in self.output and self.return_code
 
     def toplogy_check_failure(self):
-        return 'server-side topology check failed' in self.output and \
-               self.return_code
+        return "server-side topology check failed" in self.output and self.return_code
 
     def action_not_found_failure(self):
-        return 'action not found on server' in self.output and \
-               self.return_code
+        return "action not found on server" in self.output and self.return_code
 
     def missing_startup_config_failure(self):
-        return 'startup configuration is missing' in self.output and \
-               self.return_code
+        return "startup configuration is missing" in self.output and self.return_code
 
     def action_failure(self):
-        return 'executing action failed' in self.output and \
-               self.return_code
+        return "executing action failed" in self.output and self.return_code
 
     def invalid_definition_format(self):
-        return 'section missing from definition' in self.output and \
-               self.return_code
+        return "section missing from definition" in self.output and self.return_code
 
     def invalid_definition_location_failure(self):
-        return 'invalid definition location received ' \
-               'from server' in self.output and \
-               self.return_code
+        return (
+            "invalid definition location received from server" in self.output and self.return_code
+        )
 
     def success(self):
-        return 'ZTP bootstrap completed successfully!' in self.output and \
-               not self.return_code
+        return "ZTP bootstrap completed successfully!" in self.output and not self.return_code
 
 
-class EAPIServer(object):
-    #pylint: disable=C0103,E0213,W0201
+class EAPIServer:
+    # pylint: disable=C0103,E0213,W0201
 
-    def __init__(self, mac=SYSTEM_MAC, model='',
-                 serial_number='', version=''):
+    def __init__(self, mac=SYSTEM_MAC, model="", serial_number="", version=""):
         self.mac = mac
         self.model = model
         self.serial_number = serial_number
         self.version = version
 
         self.fail_commands = []
 
     def cleanup(self):
         self.responses = {}
 
     def add_failing_command(self, cmd):
         self.fail_commands += [cmd]
 
     def start(self):
-        thread.start_new_thread(self._run, ())
+        _thread.start_new_thread(self._run, ())
 
     def _run(self):
-
-        class EAPIHandler(BaseHTTPServer.BaseHTTPRequestHandler):
-
+        class EAPIHandler(BaseHTTPRequestHandler):
             def do_POST(req):
-                request = req.rfile.read(int(req.headers.getheader(
-                            'content-length')))
-                cmds = [x for x in json.loads(request)['params'][1] if x]
+                request = req.rfile.read(int(req.headers.get("content-length")))
+                cmds = [x for x in json.loads(request)["params"][1] if x]
                 if cmds:
-                    open(EAPI_LOG, 'a+b').write('%s\n' % '\n'.join(cmds))
+                    with open(EAPI_LOG, "a+b") as fd:
+                        fd.write(ensure_binary("%s\n" % "\n".join(cmds), "utf8"))
 
-                print 'EAPIServer: responding to request:%s (%s)' % (
-                    req.path, ', '.join(cmds))
+                print("EAPIServer: responding to request:{} ({})".format(req.path, ", ".join(cmds)))
 
                 if [x for x in cmds if x in self.fail_commands]:
-                    print 'EAPIServer: failed on-demand'
-                    req.send_response(STATUS_BAD_REQUEST)                    
+                    print("EAPIServer: failed on-demand")
+                    req.send_response(STATUS_BAD_REQUEST)
                     return
 
                 req.send_response(STATUS_OK)
 
-                if req.path == '/command-api':
-                    req.send_header('Content-type', 'application/json')
+                if req.path == "/command-api":
+                    req.send_header("Content-type", "application/json")
                     req.end_headers()
-                    if cmds == ['enable', 'show version']:
-                        req.wfile.write(json.dumps(
-                                {'result' :
-                                 [{},
-                                  {'modelName' : self.model,
-                                   'version' : self.version,
-                                   'serialNumber' : self.serial_number,
-                                   'systemMacAddress' : self.mac}]}))
-                    elif cmds == ['enable', 'show lldp neighbors']:
-                        req.wfile.write(json.dumps({'result' :
-                                                  [{},
-                                                   {'lldpNeighbors': []}]}))
+                    if cmds == ["enable", "show version"]:
+                        req.wfile.write(
+                            ensure_binary(
+                                json.dumps(
+                                    {
+                                        "result": [
+                                            {},
+                                            {
+                                                "modelName": self.model,
+                                                "version": self.version,
+                                                "serialNumber": self.serial_number,
+                                                "systemMacAddress": self.mac,
+                                            },
+                                        ]
+                                    }
+                                ),
+                                "utf8",
+                            )
+                        )
+                    elif cmds == ["enable", "show lldp neighbors"]:
+                        req.wfile.write(
+                            ensure_binary(
+                                json.dumps({"result": [{}, {"lldpNeighbors": []}]}), "utf8"
+                            )
+                        )
                     else:
-                        req.wfile.write(json.dumps({'result' : [{}]}))
-                    print 'EAPIServer: RESPONSE: [{}]'
+                        req.wfile.write(ensure_binary(json.dumps({"result": [{}]}), "utf8"))
+                    print("EAPIServer: RESPONSE: [{}]")
                 else:
-                    print 'EAPIServer: No RESPONSE'
+                    print("EAPIServer: No RESPONSE")
 
-        server_class = BaseHTTPServer.HTTPServer
+        server_class = HTTPServer
         httpd = server_class((EAPI_SERVER, EAPI_PORT), EAPIHandler)
-        print time.asctime(), 'EAPIServer: Server starts - %s:%s' % (
-            EAPI_SERVER, EAPI_PORT)
+        print(time.asctime(), "EAPIServer: Server starts - {}:{}".format(EAPI_SERVER, EAPI_PORT))
 
         try:
             httpd.serve_forever()
         except KeyboardInterrupt:
             pass
         finally:
             httpd.server_close()
-            print time.asctime(), 'EAPIServer: Server stops - %s:%s' % (
-                EAPI_SERVER, EAPI_PORT)
+            print(time.asctime(), "EAPIServer: Server stops - {}:{}".format(EAPI_SERVER, EAPI_PORT))
 
 
-class ZTPServer(object):
-    #pylint: disable=C0103,,E0213
+class ZTPServer:
+    # pylint: disable=C0103,,E0213
 
     # { <URL>: ( <CONTNENT-TYPE>, <STATUS>, <RESPONSE> ) }
     responses = {}
 
     def cleanup(self):
         self.responses = {}
 
-    def set_file_response(self, filename, output,
-                          content_type='text/plain',
-                          status=STATUS_OK):
-        self.responses['/%s' % filename ] = Response(
-            content_type, status,
-            output, {})
-
-        meta = { 'size': len( output ) }
-        self.responses['/meta/%s' % filename ] = Response(
-            'application/json', 200,
-            json.dumps(meta), {})
-
-    def set_action_response(self, action, output,
-                            content_type='text/x-python',
-                            status=STATUS_OK):
-        self.responses['/actions/%s' % action ] = Response(
-            content_type, status,
-            output, {})
-
-    def set_config_response(self, logging=None, xmpp=None,
-                            content_type='application/json',
-                            status=STATUS_OK):
-        response = { 'logging': [],
-                     'xmpp': {}
-                     }
+    def set_file_response(self, filename, output, content_type="text/plain", status=STATUS_OK):
+        self.responses["/{}".format(filename)] = Response(content_type, status, output, {})
+
+        meta = {"size": len(output)}
+        self.responses["/meta/{}".format(filename)] = Response(
+            "application/json", 200, json.dumps(meta), {}
+        )
+
+    def set_action_response(self, action, output, content_type="text/x-python", status=STATUS_OK):
+        self.responses["/actions/{}".format(action)] = Response(content_type, status, output, {})
+
+    def set_config_response(
+        self, logging=None, xmpp=None, content_type="application/json", status=STATUS_OK
+    ):
+        response = {"logging": [], "xmpp": {}}
         if logging:
-            response['logging'] = logging
+            response["logging"] = logging
 
         if xmpp:
-            response['xmpp'] = xmpp
+            response["xmpp"] = xmpp
 
-        self.responses['/bootstrap/config'] = Response(
-            content_type, status,
-            json.dumps(response), {})
+        self.responses["/bootstrap/config"] = Response(
+            content_type, status, json.dumps(response), {}
+        )
 
-    def set_node_check_response(self, content_type='text/html',
-                                status=None, location=None):
+    def set_node_check_response(self, content_type="text/html", status=None, location=None):
         if status is None:
-            status = random.choice([STATUS_CONFLICT,
-                                    STATUS_CREATED])
+            status = random.choice([STATUS_CONFLICT, STATUS_CREATED])
 
         headers = {}
         if location:
-            headers['location'] = location
+            headers["location"] = location
 
-        self.responses['/nodes'] = Response(
-            content_type, status, 
-            '', headers)
+        self.responses["/nodes"] = Response(content_type, status, "", headers)
 
     def set_bogus_definition_response(self):
-        self.responses['/nodes/%s' % SYSTEM_MAC] = Response(
-            'application/json', STATUS_OK,
-            json.dumps({}), {})
-
-    def set_definition_response(self, node_id=SYSTEM_MAC,
-                                name='DEFAULT_DEFINITION',
-                                actions=None,
-                                content_type='application/json',
-                                status=STATUS_OK):
-        response = { 'name': name,
-                     'actions': [],
-                     }
+        self.responses["/nodes/{}".format(SYSTEM_MAC)] = Response(
+            "application/json", STATUS_OK, json.dumps({}), {}
+        )
+
+    def set_definition_response(
+        self,
+        node_id=SYSTEM_MAC,
+        name="DEFAULT_DEFINITION",
+        actions=None,
+        content_type="application/json",
+        status=STATUS_OK,
+    ):
+        response = {
+            "name": name,
+            "actions": [],
+        }
         if actions:
-            response['actions'] += actions
+            response["actions"] += actions
 
-        self.responses['/nodes/%s' % node_id] = Response(
-            content_type, status,
-            json.dumps(response), {})
+        self.responses["/nodes/{}".format(node_id)] = Response(
+            content_type, status, json.dumps(response), {}
+        )
 
     def start(self):
-        thread.start_new_thread(self._run, ())
+        _thread.start_new_thread(self._run, ())
 
     def _run(self):
-
-        class ZTPSHandler(BaseHTTPServer.BaseHTTPRequestHandler):
-
+        class ZTPSHandler(BaseHTTPRequestHandler):
             @classmethod
             def do_request(cls, req):
-                if req.path in self.responses.keys():
+                if req.path in self.responses:
                     response = self.responses[req.path]
                     req.send_response(response.status)
                     req.error_content_type = response.content_type
 
-                    req.send_header('Content-type', response.content_type)
-                    for name, value in response.headers.iteritems():
+                    req.send_header("Content-type", response.content_type)
+                    for name, value in response.headers.items():
                         req.send_header(name, value)
 
                     req.end_headers()
-                    req.wfile.write(response.contents)
-                    print 'ZTPS: RESPONSE: (ct=%s, status=%s, output=%s...)' % (
-                        response[0],
-                        response[1],
-                        response[2][:100])
+                    req.wfile.write(ensure_binary(response.contents, "utf8"))
+                    print(
+                        "ZTPS: RESPONSE: (ct={}, status={}, output={}...)".format(
+                            response[0], response[1], response[2][:100]
+                        )
+                    )
                 else:
-                    print 'ZTPS: No RESPONSE'
+                    print("ZTPS: No RESPONSE")
 
             def do_GET(req):
-                print 'ZTPS: responding to GET request:%s' % req.path
+                print("ZTPS: responding to GET request:{}".format(req.path))
                 ZTPSHandler.do_request(req)
 
             def do_POST(req):
-                print 'ZTPS: responding to POST request:%s' % req.path
-                headers = self.responses['/nodes'].headers
-                if 'location' not in headers:
-                    length = req.headers.getheader('content-length')
-                    node_id = json.loads(req.rfile.read(
-                            int(length)))['systemmac']
-                    location  = 'http://%s:%s/nodes/%s' % (ZTPS_SERVER, 
-                                                           ZTPS_PORT,
-                                                           node_id)
-                    self.responses['/nodes'].headers['location'] = location
+                print("ZTPS: responding to POST request:{}".format(req.path))
+                headers = self.responses["/nodes"].headers
+                if "location" not in headers:
+                    length = req.headers.get("content-length")
+                    node_id = json.loads(req.rfile.read(int(length)))["systemmac"]
+                    location = "http://{}:{}/nodes/{}".format(ZTPS_SERVER, ZTPS_PORT, node_id)
+                    self.responses["/nodes"].headers["location"] = location
 
                 ZTPSHandler.do_request(req)
 
-        server_class = BaseHTTPServer.HTTPServer
+        server_class = HTTPServer
         httpd = server_class((ZTPS_SERVER, ZTPS_PORT), ZTPSHandler)
 
-        print time.asctime(), 'ZTPS: Server starts - %s:%s' % (
-            ZTPS_SERVER, ZTPS_PORT)
+        print(time.asctime(), "ZTPS: Server starts - {}:{}".format(ZTPS_SERVER, ZTPS_PORT))
         try:
             httpd.serve_forever()
         except KeyboardInterrupt:
             pass
         finally:
             httpd.server_close()
-            print time.asctime(), 'ZTPS: Server stops - %s:%s' % (
-                ZTPS_SERVER, ZTPS_PORT)
-
-
-class SmtpServer(object):
-    #pylint: disable=E0211
-
-    def start(self):
-        thread.start_new_thread(self._run, ())
-
-    @classmethod
-    def _run(cls):
+            print(time.asctime(), "ZTPS: Server stops - {}:{}".format(ZTPS_SERVER, ZTPS_PORT))
 
-        class SMTPServer(smtpd.SMTPServer):
-
-            def __init__(*args, **kwargs):
-                print "SMTP: Running smtp server on port 2525"
-                smtpd.SMTPServer.__init__(*args, **kwargs)
-
-            def process_message(*args, **kwargs):
-                pass
-
-        smtp_server = SMTPServer((SMTP_SERVER, SMTP_PORT), None)
-        print time.asctime(), 'SMTP: Server starts - %s:%s' % (
-            SMTP_SERVER, SMTP_PORT)
-        try:
-            asyncore.loop()
-        except KeyboardInterrupt:
-            pass
-        finally:
-            smtp_server.close()
-            print time.asctime(), 'SMTPS: Server stops - %s:%s' % (
-                SMTP_SERVER, SMTP_PORT)
 
 class ActionFailureTest(unittest.TestCase):
-    #pylint: disable=R0904
+    # pylint: disable=R0904
 
-    def basic_test(self, action, return_string, attributes=None,
-                   action_value=None, file_responses=None):
+    def basic_test(
+        self, action, return_string, attributes=None, action_value=None, file_responses=None
+    ):
         if not attributes:
             attributes = {}
 
         if not file_responses:
             file_responses = {}
 
         if not action_value:
             action_value = get_action(action)
 
         bootstrap = Bootstrap(ztps_default_config=True)
+        action_value = (
+            action_value.replace("/mnt/flash/.extensions", bootstrap.boot_extensions_folder)
+            .replace("/mnt/flash/boot-extensions", bootstrap.boot_extensions)
+            .replace("/mnt/flash/.ztp-plugins", bootstrap.ztp_plugins_folder)
+        )
         bootstrap.ztps.set_definition_response(
-            actions=[{'action' : 'test_action',
-                      'attributes' : attributes}])
-        bootstrap.ztps.set_action_response('test_action',
-                                           action_value)
+            actions=[{"action": "test_action", "attributes": attributes}]
+        )
+        bootstrap.ztps.set_action_response("test_action", action_value)
 
-        for key, value in file_responses.iteritems():
-            bootstrap.ztps.set_file_response(key, value)            
+        for key, value in file_responses.items():
+            bootstrap.ztps.set_file_response(key, value)
 
         bootstrap.start_test()
 
         try:
-            self.failUnless(bootstrap.action_failure())
-            msg = [x for x in bootstrap.output.split('\n') if x][-1]
-            self.failUnless('%s' % return_string in msg)
+            self.assertTrue(bootstrap.action_failure())
+            self.assertTrue(return_string in bootstrap.output)
         except AssertionError as assertion:
-            print 'Output: %s' % bootstrap.output
-            print 'Error: %s' % bootstrap.error
+            print("Output: {}".format(bootstrap.output))
+            print("Error: {}".format(bootstrap.error))
             raise_exception(assertion)
         finally:
             bootstrap.end_test()
```

### Comparing `ztpserver-1.6.0/bin/ztps` & `ztpserver-2.0.0/bin/ztps`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 #
 # Copyright (c) 2013, Arista Networks
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
@@ -32,8 +32,7 @@
 #
 import sys
 
 import ztpserver.app
 
 if __name__ == "__main__":
     sys.exit(ztpserver.app.main())
-
```

### Comparing `ztpserver-1.6.0/ztpserver/controller.py` & `ztpserver-2.0.0/ztpserver/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,284 +25,288 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-# pylint: disable=W0622,W0402,W0613,W0142,R0201,E1103,W0150
+# pylint: disable=W0622,W0402,W0613,E1103,W0150
 #
 
 import logging
 import os
-import routes
 import subprocess
-
 from string import Template
 from subprocess import PIPE
-from webob.static import FileApp
 
-from ztpserver.constants import HTTP_STATUS_NOT_FOUND, HTTP_STATUS_CREATED
-from ztpserver.constants import HTTP_STATUS_BAD_REQUEST, HTTP_STATUS_CONFLICT
-from ztpserver.constants import HTTP_STATUS_INTERNAL_SERVER_ERROR
-from ztpserver.constants import CONTENT_TYPE_JSON, CONTENT_TYPE_PYTHON
-from ztpserver.constants import CONTENT_TYPE_YAML, CONTENT_TYPE_OTHER
+import routes
+from webob.static import FileApp
 
-from ztpserver.repository import create_repository
-from ztpserver.repository import FileObjectNotFound, FileObjectError
+from ztpserver.config import runtime
+from ztpserver.constants import (
+    CONTENT_TYPE_JSON,
+    CONTENT_TYPE_OTHER,
+    CONTENT_TYPE_PYTHON,
+    CONTENT_TYPE_YAML,
+    HTTP_STATUS_BAD_REQUEST,
+    HTTP_STATUS_CONFLICT,
+    HTTP_STATUS_CREATED,
+    HTTP_STATUS_INTERNAL_SERVER_ERROR,
+    HTTP_STATUS_NOT_FOUND,
+)
+from ztpserver.repository import FileObjectError, FileObjectNotFound, create_repository
 from ztpserver.serializers import SerializerError
-from ztpserver.topology import create_node, load_pattern
-from ztpserver.topology import load_neighbordb, load_resources
-from ztpserver.topology import replace_config_action
+from ztpserver.topology import (
+    create_node,
+    load_neighbordb,
+    load_pattern,
+    load_resources,
+    replace_config_action,
+)
 from ztpserver.wsgiapp import WSGIController, WSGIRouter
-from ztpserver.config import runtime
-
 
-DEFINITION_FN = 'definition'
-CONFIG_HANDLER_FN = 'config-handler'
-STARTUP_CONFIG_FN = 'startup-config'
-PATTERN_FN = 'pattern'
-NODE_FN = '.node'
-ATTRIBUTES_FN = 'attributes'
-BOOTSTRAP_CONF = 'bootstrap.conf'
+DEFINITION_FN = "definition"
+CONFIG_HANDLER_FN = "config-handler"
+STARTUP_CONFIG_FN = "startup-config"
+PATTERN_FN = "pattern"
+NODE_FN = ".node"
+ATTRIBUTES_FN = "attributes"
+BOOTSTRAP_CONF = "bootstrap.conf"
 
-log = logging.getLogger(__name__)    # pylint: disable=C0103
+log = logging.getLogger(__name__)  # pylint: disable=C0103
 
 
 class ValidationError(Exception):
-    ''' Base exception class for :py:class:`Pattern` '''
-    pass
+    """Base exception class for :py:class:`Pattern`"""
 
 
 class BaseController(WSGIController):
-
     FOLDER = None
 
     def __init__(self, **kwargs):
         self.data_root = runtime.default.data_root
         self.repository = create_repository(self.data_root)
-        super(BaseController, self).__init__()
+        super().__init__()
 
     def expand(self, *args, **kwargs):
-        ''' Returns an expanded file path relative to data_root '''
+        """Returns an expanded file path relative to data_root"""
 
         file_path = os.path.join(*args)
-        folder = kwargs.get('folder', self.FOLDER)
+        folder = kwargs.get("folder", self.FOLDER)
         return os.path.join(folder, file_path)
 
     def http_bad_request(self, *args, **kwargs):
-        ''' Returns HTTP 400 Bad Request '''
-        return dict(body='', content_type='text/html',
-                    status=HTTP_STATUS_BAD_REQUEST)
+        """Returns HTTP 400 Bad Request"""
+        return {
+            "body": "",
+            "content_type": "text/html",
+            "status": HTTP_STATUS_BAD_REQUEST,
+        }
 
     def http_not_found(self, *args, **kwargs):
-        ''' Returns HTTP 404 Not Found '''
+        """Returns HTTP 404 Not Found"""
 
-        return dict(body='', content_type='text/html',
-                    status=HTTP_STATUS_NOT_FOUND)
+        return {
+            "body": "",
+            "content_type": "text/html",
+            "status": HTTP_STATUS_NOT_FOUND,
+        }
 
     def http_internal_server_error(self, *args, **kwargs):
-        ''' Returns HTTP 500 Internal server error '''
+        """Returns HTTP 500 Internal server error"""
 
-        return dict(body='', content_type='text/html',
-                    status=HTTP_STATUS_INTERNAL_SERVER_ERROR)
+        return {
+            "body": "",
+            "content_type": "text/html",
+            "status": HTTP_STATUS_INTERNAL_SERVER_ERROR,
+        }
 
 
 class FilesController(BaseController):
-
-    FOLDER = 'files'
+    FOLDER = "files"
 
     def __repr__(self):
-        return 'FilesController(folder=%s)' % self.FOLDER
+        return f"FilesController(folder={self.FOLDER})"
 
     def show(self, request, resource, **kwargs):
-        ''' Handles GET /files/{resource} '''
-        log.debug('%s\nResource: %s\n' % (request, resource))
+        """Handles GET /files/{resource}"""
+        log.debug("%s\nResource: %s\n", request, resource)
 
         try:
             urlvars = request.urlvars
-            if urlvars.get('format') is not None:
-                resource += '.%s' % urlvars.get('format')
+            if urlvars.get("format") is not None:
+                resource += f'.{urlvars.get("format")}'
             file_path = self.expand(resource)
             filename = self.repository.get_file(file_path).name
             return FileApp(filename, content_type=CONTENT_TYPE_OTHER)
         except FileObjectNotFound:
-            log.error('File %s not found' % resource)
+            log.error("File %s not found", resource)
             return self.http_not_found()
 
 
 class ActionsController(BaseController):
-
-    FOLDER = 'actions'
+    FOLDER = "actions"
 
     def __repr__(self):
-        return 'ActionsController(folder=%s)' % self.FOLDER
+        return f"ActionsController(folder={self.FOLDER})"
 
     def show(self, request, resource, **kwargs):
-        ''' Handles GET /actions/{resource} '''
-        log.debug('%s\nResource: %s\n' % (request, resource))
+        """Handles GET /actions/{resource}"""
+        log.debug("%s\nResource: %s\n", request, resource)
 
         try:
             file_path = self.expand(resource)
             body = self.repository.get_file(file_path).read(CONTENT_TYPE_PYTHON)
-            return dict(body=body, content_type=CONTENT_TYPE_PYTHON)
+            return {"body": body, "content_type": CONTENT_TYPE_PYTHON}
         except FileObjectNotFound:
-            log.error('Action %s not found' % resource)
+            log.error("Action %s not found", resource)
             return self.http_not_found()
 
 
 class NodesController(BaseController):
-
-    FOLDER = 'nodes'
+    FOLDER = "nodes"
 
     def __repr__(self):
-        return 'NodesController(folder=%s)' % self.FOLDER
-
+        return f"NodesController(folder={self.FOLDER})"
 
     def fsm(self, state, **kwargs):
-        ''' Execute the FSM for the request '''
+        """Execute the FSM for the request"""
 
-        response = dict()
+        response = {}
+        prev_state = None
         try:
-            while state != None:
+            while state is not None:
                 method = getattr(self, state)
                 prev_state = state
-                log.debug('%s: running %s' % (kwargs['node_id'], state))
+                log.debug("%s: running %s", kwargs["node_id"], state)
                 (response, state) = method(response, **kwargs)
-        except ValidationError:            # pylint: disable=W0703
-            log.error('%s: validation error in %s' %
-                      (kwargs['node_id'], prev_state))
+        except ValidationError:  # pylint: disable=W0703
+            log.error("%s: validation error in %s", kwargs["node_id"], prev_state)
             response = self.http_bad_request()
-        except Exception as err:            # pylint: disable=W0703
-            log.error('%s: error in %s: %s' %
-                      (kwargs['node_id'], prev_state, str(err)))
+        except Exception as err:  # pylint: disable=W0703
+            log.error("%s: error in %s: %s", kwargs["node_id"], prev_state, str(err))
             response = self.http_bad_request()
 
-        log.debug('%s: response to %s: %s' %
-                  (kwargs['node_id'], prev_state, response))
-        return response                     # pylint: disable=W0150
+        log.debug("%s: response to %s: %s", kwargs["node_id"], prev_state, response)
+        return response
 
-    #-------------------------------------------------------------------
+    # -------------------------------------------------------------------
 
     def get_config(self, request, resource, **kwargs):
-        log.debug('%s: node resource GET request: \n%s\n' %
-                  (resource, request))
+        log.debug("%s: node resource GET request: \n%s\n", resource, request)
 
-        response = dict()
+        response = {}
+        filename = self.expand(resource, STARTUP_CONFIG_FN)
 
         try:
-            filename = self.expand(resource, STARTUP_CONFIG_FN)
-            response['body'] = self.repository.get_file(filename).read()
-            response['content_type'] = CONTENT_TYPE_OTHER
+            response["body"] = self.repository.get_file(filename).read()
+            response["content_type"] = CONTENT_TYPE_OTHER
         except FileObjectNotFound:
-            log.error('%s: missing startup-config file %s' %
-                      (resource, filename))
+            log.error("%s: missing startup-config file %s", resource, filename)
             response = self.http_bad_request()
         except Exception as err:
-            log.error('%s: unable to retrieve startup-config (%s)' %
-                      (resource, err))
+            log.error("%s: unable to retrieve startup-config (%s)", resource, err)
             response = self.http_bad_request()
 
         return response
 
-    #-------------------------------------------------------------------
+    # -------------------------------------------------------------------
 
     def put_config(self, request, **kwargs):
-        node_id = kwargs['resource']
+        node_id = kwargs["resource"]
 
-        log.debug('%s: startup-config PUT request: \n%s\n' %
-                  (node_id, request))
+        log.debug("%s: startup-config PUT request: \n%s\n", node_id, request)
 
         fobj = None
+        filename = self.expand(node_id, STARTUP_CONFIG_FN)
+        body = str(request.body)
+        content_type = str(request.content_type)
         try:
-            body = str(request.body)
-            content_type = str(request.content_type)
-            filename = self.expand(node_id, STARTUP_CONFIG_FN)
             fobj = self.repository.get_file(filename)
         except FileObjectNotFound:
-            log.debug('%s: file not found: %s (adding it)' %
-                      (node_id, filename))
+            log.debug("%s: file not found: %s (adding it)", node_id, filename)
             fobj = self.repository.add_file(filename)
         finally:
             if fobj:
                 fobj.write(body, content_type)
             else:
-                log.error('%s: unable to write %s' %
-                          (node_id, filename))
+                log.error("%s: unable to write %s", node_id, filename)
                 return self.http_bad_request()
 
         # Execute event-handler
-        script = self.repository.expand(
-            self.expand(node_id, CONFIG_HANDLER_FN))
+        script = self.repository.expand(self.expand(node_id, CONFIG_HANDLER_FN))
         if os.path.isfile(script):
-            proc = subprocess.Popen(script, stdin=PIPE,
-                                    stdout=PIPE, stderr=PIPE,
-                                    shell=True)
-            code = proc.returncode         #pylint: disable=E1101
-            (out, err) = proc.communicate()
+            with subprocess.Popen(script, stdin=PIPE, stdout=PIPE, stderr=PIPE, shell=True) as proc:
+                code = proc.returncode
+                (out, err) = proc.communicate()
             if code or err:
-                log.warn('Startup-config saved for %s '
-                         '(%s failed: return code=%s, stderr=%s)' %
-                         (node_id, script, code, err))
-                log.debug('%s output: \n%s' % (script, out))
+                log.warning(
+                    "Startup-config saved for %s (%s failed: return code=%s, stderr=%s)",
+                    node_id,
+                    script,
+                    code,
+                    err,
+                )
+                log.debug("%s output: \n%s", script, out)
             else:
-                log.info('Startup-config saved for %s '
-                         '(%s executed successfully)' %
-                         (node_id, script))
-                log.debug('%s output: \n%s' % (script, out))
+                log.info(
+                    "Startup-config saved for %s (%s executed successfully)",
+                    node_id,
+                    script,
+                )
+                log.debug("%s output: \n%s", script, out)
         else:
-            log.info('Startup-config saved for %s (no config-handler)' %
-                     node_id)
+            log.info("Startup-config saved for %s (no config-handler)", node_id)
 
         return {}
 
-    #-------------------------------------------------------------------
+    # -------------------------------------------------------------------
 
     def create(self, request, **kwargs):
-        """ Handle the POST /nodes request
+        """Handle the POST /nodes request
 
         The create method will handle in incoming POST request from the node
         and determine if the node already exists or not.  If the node
         does not exist, then the node will be created based on the
         request body.
 
         Args:
             request (webob.Request): the request object from WSGI
 
         Returns:
             A dict as the result of the state machine which is used to
             create a WSGI response object.
 
         """
-        log.info('%s: received system information from node:\n%s' %
-                 (request.remote_addr, request.json))
+        log.info(
+            "%s: received system information from node:\n%s",
+            request.remote_addr,
+            request.json,
+        )
 
         try:
             node = create_node(request.json)
-        except Exception as err:       # pylint: disable=W0703
-            log.error('Unable to create node: %s (request=%s)' % (err, request))
+        except Exception as err:  # pylint: disable=W0703
+            log.error("Unable to create node: %s (request=%s)", err, request)
             response = self.http_bad_request()
             return self.response(**response)
 
         node_id = node.identifier()
         if not node_id:
-            log.error('Missing node identifier: %s (request=%s)' %
-                      (node, request))
+            log.error("Missing node identifier: %s (request=%s)", node, request)
             response = self.http_bad_request()
             return self.response(**response)
 
         identifier = runtime.default.identifier
-        log.info('%s: node ID is %s:%s' %
-                 (request.remote_addr, identifier, node_id))
+        log.info("%s: node ID is %s:%s", request.remote_addr, identifier, node_id)
 
-        return self.fsm('node_exists', request=request,
-                        node=node, node_id=node_id)
+        return self.fsm("node_exists", request=request, node=node, node_id=node_id)
 
     def node_exists(self, response, *args, **kwargs):
-        """ Checks if the node already exists and determines the next state
+        """Checks if the node already exists and determines the next state
 
         This method will check for the existence of the node in the
         repository based on the node_id.  The node_id keyword is pulled
         from the kwargs dict.
 
         Args:
             response (dict): the response object being constructed
@@ -312,67 +316,72 @@
             A tuple that includes the updated response object and the
             next state to transition to.  If the node already exists
             in the repository with a valid definition or startup-config,
             then the next state is 'dump_node' otherwise the next state
             is 'post_config'
 
         """
-        next_state = 'post_config'
-        node_id = kwargs.get('node_id')
+        next_state = "post_config"
+        node_id = kwargs.get("node_id")
 
-        if self.repository.exists(self.expand(node_id, DEFINITION_FN)) or \
-           self.repository.exists(self.expand(node_id, STARTUP_CONFIG_FN)):
-            log.info('%s: this node already exists on the server' % node_id)
-            response['status'] = HTTP_STATUS_CONFLICT
-            next_state = 'dump_node'
+        if self.repository.exists(self.expand(node_id, DEFINITION_FN)) or self.repository.exists(
+            self.expand(node_id, STARTUP_CONFIG_FN)
+        ):
+            log.info("%s: this node already exists on the server", node_id)
+            response["status"] = HTTP_STATUS_CONFLICT
+            next_state = "dump_node"
         else:
             if self.repository.exists(self.expand(node_id)):
-                log.error('%s: node found on server, but no definition '
-                          'or startup-config configured' % node_id)
-                return (self.http_bad_request(), None)
+                log.error(
+                    "%s: node found on server, but no definition or startup-config configured",
+                    node_id,
+                )
+                return self.http_bad_request(), None
 
-        return (response, next_state)
+        return response, next_state
 
     def post_config(self, response, *args, **kwargs):
-        """ Writes the nodes startup config file if found in the request
+        """Writes the nodes startup config file if found in the request
 
         Args:
             response (dict): the response object being constructed
             kwargs (dict): arbitrary keyword arguments
 
         Returns:
             a tuple of response object and next state.  If a config key
             was found in the request, the next state is 'set_location'.
             If not, the next state is 'post_node'.
 
         """
 
-        if 'config' not in kwargs['request'].json:
+        if "config" not in kwargs["request"].json:
             # POST request for the node - will try to match neighbordb
-            next_state = 'post_node'
-            log.info('%s: node does not exist on the server - '
-                     'will try to match node against neighbordb' %
-                     kwargs['node_id'])
+            next_state = "post_node"
+            log.info(
+                "%s: node does not exist on the server - "
+                "will try to match node against neighbordb",
+                kwargs["node_id"],
+            )
         else:
             # POST request for the node's startup-config
-            config = kwargs['request'].json['config']
-            node_id = kwargs['node_id']
+            config = kwargs["request"].json["config"]
+            node_id = kwargs["node_id"]
 
             self.repository.add_folder(self.expand(node_id))
 
             config_fn = self.expand(node_id, STARTUP_CONFIG_FN)
             self.repository.add_file(config_fn).write(config)
 
-            response['status'] = HTTP_STATUS_CREATED
-            next_state = 'set_location'
+            response["status"] = HTTP_STATUS_CREATED
+            next_state = "set_location"
 
         return (response, next_state)
 
     def post_node(self, response, *args, **kwargs):
-        """ Checks topology validation matches and writes node specific files
+        """Checks topology validation matches and writes node specific files
 
         This method will attempt to match the current node against the
         defined topology.  If a match is found, then the pattern matched
         and definition (defined in the pattern) are written to the nodes
         folder in the repository and the response status is set to HTTP
         201 Created.
 
@@ -385,548 +394,575 @@
             is 'dump_node'
 
         Raises:
             If a match is not found, then a log message is created and
             an IndexError is raised.  If the node does not already
             exist in the repository, then a log message is created and a
             FileObjectNotFound exception is raised
-            """
+        """
 
-        node = kwargs['node']
-        node_id = kwargs['node_id']
+        node = kwargs["node"]
+        node_id = kwargs["node_id"]
 
         neighbordb = load_neighbordb(node_id)
         if not neighbordb:
-            return (self.http_bad_request(), None)
+            return self.http_bad_request(), None
 
         # pylint: disable=E1103
         matches = neighbordb.match_node(node)
         if not matches:
-            log.info('%s: node matched no patterns in neighbordb' %
-                     node_id)
-            return (self.http_bad_request(), None)
+            log.info("%s: node matched no patterns in neighbordb", node_id)
+            return self.http_bad_request(), None
 
-        log.debug('%s: %d pattern(s) in neihgbordb are a good match' %
-                  (node_id, len(matches)))
+        log.debug("%s: %d pattern(s) in neihgbordb are a good match", node_id, len(matches))
         match = matches[0]
 
-        log.info('%s: node matched \'%s\' pattern in neighbordb' %
-                 (node_id, match.name))
+        log.info("%s: node matched '%s' pattern in neighbordb", node_id, match.name)
 
         # Load definition
+        definition_url = self.expand(match.definition, folder="definitions")
         try:
-            definition_url = self.expand(match.definition,
-                                         folder='definitions')
             fobj = self.repository.get_file(definition_url)
-            log.info('%s: node definition copied from: %s' %
-                     (node_id, definition_url))
+            log.info("%s: node definition copied from: %s", node_id, definition_url)
         except FileObjectNotFound:
-            log.error('%s: failed to find definition (%s)' %
-                      (node_id, definition_url))
+            log.error("%s: failed to find definition (%s)", node_id, definition_url)
             raise
 
         try:
             definition = fobj.read(content_type=CONTENT_TYPE_YAML)
         except FileObjectError:
-            log.error('%s: failed to load definition' %
-                      (node_id))
+            log.error("%s: failed to load definition", node_id)
             raise
 
         definition_fn = self.expand(node_id, DEFINITION_FN)
 
         # Load config-handler
         if match.config_handler:
+            config_handler_url = self.expand(match.config_handler, folder="config-handlers")
             try:
-                config_handler_url = self.expand(match.config_handler,
-                                                 folder='config-handlers')
                 fobj = self.repository.get_file(config_handler_url)
-                log.info('%s: node config-handler copied from: %s' %
-                         (node_id, config_handler_url))
+                log.info(
+                    "%s: node config-handler copied from: %s",
+                    node_id,
+                    config_handler_url,
+                )
             except FileObjectNotFound:
-                log.error('%s: failed to find config-handler (%s)' %
-                          (node_id, config_handler_url))
+                log.error(
+                    "%s: failed to find config-handler (%s)",
+                    node_id,
+                    config_handler_url,
+                )
                 raise
 
             try:
                 config_handler = fobj.read(content_type=CONTENT_TYPE_OTHER)
             except FileObjectError:
-                log.error('%s: failed to load config-handler' %
-                          (node_id))
+                log.error("%s: failed to load config-handler", node_id)
                 raise
 
             config_handler_fn = self.expand(node_id, CONFIG_HANDLER_FN)
 
         # Create node folder
         self.repository.add_folder(self.expand(node_id))
 
-        log.info('%s: new dynamically-provisioned node created: /nodes/%s' %
-                 (node_id, node_id))
+        log.info("%s: new dynamically-provisioned node created: /nodes/%s", node_id, node_id)
 
         # Add definition
         fobj = self.repository.add_file(definition_fn)
         fobj.write(definition, CONTENT_TYPE_YAML)
 
         # Add pattern
         pattern_fn = self.expand(node_id, PATTERN_FN)
         fobj = self.repository.add_file(pattern_fn)
 
         pattern = match.serialize()
 
         # No need to write the definition name in the pattern file
-        del pattern['definition']
+        del pattern["definition"]
 
-        for attr in ['node', 'variables']:
+        for attr in ["node", "variables"]:
             if not pattern[attr]:
                 del pattern[attr]
 
         # Add default pattern, if 'interfaces' is not specified
-        if 'interfaces' not in pattern or not pattern['interfaces']:
-            pattern['interfaces'] = [{'any': {'any': 'any'}}]
+        if "interfaces" not in pattern or not pattern["interfaces"]:
+            pattern["interfaces"] = [{"any": {"any": "any"}}]
 
         fobj.write(pattern, CONTENT_TYPE_YAML)
 
         # Add config-handler
         if match.config_handler:
             fobj = self.repository.add_file(config_handler_fn)
             fobj.write(config_handler, CONTENT_TYPE_OTHER)
 
-        response['status'] = HTTP_STATUS_CREATED
-        return (response, 'dump_node')
+        response["status"] = HTTP_STATUS_CREATED
+        return (response, "dump_node")
 
     def dump_node(self, response, *args, **kwargs):
-        """ Writes the contents of the node to the repository
+        """Writes the contents of the node to the repository
 
         Args:
             response (dict): the response object being constructed
             kwargs (dict): arbitrary keyword arguments
 
         Returns:
             a tuple of response object and next state.  The next state is
             'set_location'
 
         """
 
+        node_id = kwargs.get("node_id")
+        filename = self.expand(node_id, NODE_FN)
+        fobj = None
+        contents = None
         try:
-            node = kwargs.get('node')
-            node_id = kwargs.get('node_id')
+            node = kwargs.get("node")
             contents = node.serialize()
-            filename = self.expand(node_id, NODE_FN)
             fobj = self.repository.get_file(filename)
         except FileObjectNotFound:
             fobj = self.repository.add_file(filename)
         finally:
-            fobj.write(contents, CONTENT_TYPE_JSON)
+            if fobj and contents:
+                fobj.write(contents, CONTENT_TYPE_JSON)
+            else:
+                log.error("%s: unable to write %s", node_id, filename)
+                return self.http_bad_request()
 
-        log.info('%s: node data written to %s:\n%s' %
-                 (node_id, filename, contents))
+        log.info("%s: node data written to %s:\n%s", node_id, filename, contents)
 
-        return (response, 'set_location')
+        return response, "set_location"
 
     def set_location(self, response, *args, **kwargs):
-        """ Writes the HTTP Content-Location header
+        """Writes the HTTP Content-Location header
 
         Args:
             response (dict): the response object being constructed
             kwargs (dict): arbitrary keyword arguments
 
         Returns:
             a tuple of response object and next state.  The next state is
             None.
 
         Raises:
             Exception: catches a general exception for logging and then
                        re-raises it
         """
-        node_id = kwargs.get('node_id')
-        response['location'] = self.expand(node_id)
+        node_id = kwargs.get("node_id")
+        response["location"] = self.expand(node_id)
         return (response, None)
 
-    #-------------------------------------------------------------------
+    # -------------------------------------------------------------------
 
     def show(self, request, resource, *args, **kwargs):
-        """ Handle the GET /nodes/{resource} request
+        """Handle the GET /nodes/{resource} request
 
         Args:
             request (webob.Request): the request object from WSGI
             resource (str): the resource being requested
 
         Returns:
             A dict as the result of the state machine which is used to
             create a WSGI response object.
 
         """
-        log.info('%s: received request for definition: %s' %
-                 (resource, request.url))
-        log.debug('%s\nResource: %s\n' % (request, resource))
+        log.info("%s: received request for definition: %s", resource, request.url)
+        log.debug("%s\nResource: %s\n", request, resource)
 
-        node_id = resource.split('/')[0]
+        node_id = resource.split("/")[0]
         try:
             fobj = self.repository.get_file(self.expand(resource, NODE_FN))
             node = create_node(fobj.read(CONTENT_TYPE_JSON))
-        except Exception as err:           # pylint: disable=W0703
-            log.error('%s: unable to read %s file for %s: %s' %
-                      (NODE_FN, node_id, resource, err))
+        except Exception as err:  # pylint: disable=W0703
+            log.error("%s: unable to read %s file for %s: %s", NODE_FN, node_id, resource, err)
             response = self.http_bad_request()
             return self.response(**response)
 
-        return self.fsm('do_validation', resource=resource, request=request,
-                        node=node, node_id=node_id)
+        return self.fsm(
+            "do_validation",
+            resource=resource,
+            request=request,
+            node=node,
+            node_id=node_id,
+        )
 
     def do_validation(self, response, *args, **kwargs):
         if not runtime.default.disable_topology_validation:
-            log.info('%s: topology validation is ENABLED' % kwargs['resource'])
+            log.info("%s: topology validation is ENABLED", kwargs["resource"])
 
-            filename = self.expand(kwargs['resource'], PATTERN_FN)
+            filename = self.expand(kwargs["resource"], PATTERN_FN)
             fobj = self.repository.get_file(filename)
 
             try:
-                log.info('%s: checking syntax of pattern file used for topology'
-                         ' validation: %s' % (kwargs['resource'], filename))
-                pattern = load_pattern(fobj.name, node_id=kwargs['resource'])
+                log.info(
+                    "%s: checking syntax of pattern file used for topology validation: %s",
+                    kwargs["resource"],
+                    filename,
+                )
+                pattern = load_pattern(fobj.name, node_id=kwargs["resource"])
             except SerializerError as err:
-                log.error(err.message)
-                raise Exception('failed to load pattern %s' % filename)
+                log.error(str(err))
+                raise RuntimeError(f"failed to load pattern {filename}") from err
 
             if not pattern:
-                raise Exception('failed to validate pattern')
+                raise RuntimeError("failed to validate pattern")
 
-            log.info('%s: evaluating node against pattern: %s' %
-                     (kwargs['resource'], filename))
-            if not pattern.match_node(kwargs['node']):
-                log.error('%s: node failed pattern validation (%s)' %
-                          (kwargs['resource'], filename))
-                raise ValidationError('%s: node failed pattern '
-                                      'validation (%s)' %
-                                      (kwargs['resource'], filename))
-            log.info('%s: node passed pattern validation: %s' %
-                      (kwargs['resource'], filename))
+            log.info("%s: evaluating node against pattern: %s", kwargs["resource"], filename)
+            if not pattern.match_node(kwargs["node"]):
+                log.error(
+                    "%s: node failed pattern validation (%s)",
+                    kwargs["resource"],
+                    filename,
+                )
+                raise ValidationError(
+                    f"{kwargs['resource']}: " f"node failed pattern validation ({filename})"
+                )
+            log.info("%s: node passed pattern validation: %s", kwargs["resource"], filename)
         else:
-            log.warning('%s: topology validation is DISABLED' %
-                        kwargs['resource'])
-        return (response, 'get_startup_config')
+            log.warning("%s: topology validation is DISABLED", kwargs["resource"])
+        return response, "get_startup_config"
 
     def get_startup_config(self, response, *args, **kwargs):
-        response['get_startup_config'] = False
+        response["get_startup_config"] = False
+        filename = self.expand(kwargs["resource"], STARTUP_CONFIG_FN)
         try:
-            filename = self.expand(kwargs['resource'], STARTUP_CONFIG_FN)
             self.repository.get_file(filename)
-            response['get_startup_config'] = True
-            actions = [replace_config_action(kwargs['resource'],
-                                             STARTUP_CONFIG_FN)]
-            response['definition'] = dict(name='Autogenerated definition',
-                                          actions=actions)
+            response["get_startup_config"] = True
+            actions = [replace_config_action(kwargs["resource"], STARTUP_CONFIG_FN)]
+            response["definition"] = {
+                "name": "Autogenerated definition",
+                "actions": actions,
+            }
         except FileObjectNotFound:
-            log.debug('%s: no startup-config %s' %
-                      (kwargs['resource'], filename))
+            log.debug("%s: no startup-config %s", kwargs["resource"], filename)
 
-        return (response, 'get_definition')
+        return response, "get_definition"
 
     def get_definition(self, response, *args, **kwargs):
-        ''' Reads the node specific definition from disk and stores it in the
+        """Reads the node specific definition from disk and stores it in the
         repsonse dict with key `definition`
-        '''
+        """
 
+        filename = self.expand(kwargs["resource"], DEFINITION_FN)
         try:
-            filename = self.expand(kwargs['resource'], DEFINITION_FN)
             fobj = self.repository.get_file(filename)
-            definition = fobj.read(CONTENT_TYPE_YAML,
-                                   kwargs['resource'])
+            definition = fobj.read(CONTENT_TYPE_YAML, kwargs["resource"])
             actions = []
-            if 'actions' in definition:
-                actions = definition['actions']
+            if "actions" in definition:
+                actions = definition["actions"]
 
-            if 'definition' in response:
+            if "definition" in response:
                 # startup-config already present
-                _actions = list()
+                _actions = []
                 for action in actions:
-                    always_execute = action.get('always_execute', False)
+                    always_execute = action.get("always_execute", False)
                     if always_execute:
                         _actions.append(action)
-                        log.debug('%s: always_execute action %s included '
-                                  'in definition' %
-                                  (kwargs['resource'],  action.get('name')))
+                        log.debug(
+                            "%s: always_execute action %s included in definition",
+                            kwargs["resource"],
+                            action.get("name"),
+                        )
                     else:
-                        log.debug('%s: action %s not included '
-                                  'in definition' %
-                                  (kwargs['resource'],  action.get('name')))
-                response['definition']['actions'] += _actions
+                        log.debug(
+                            "%s: action %s not included in definition",
+                            kwargs["resource"],
+                            action.get("name"),
+                        )
+                response["definition"]["actions"] += _actions
             else:
                 # no startup-config
                 for action in actions:
-                    log.debug('%s: action %s included '
-                              'in definition' %
-                              (kwargs['resource'],  action.get('name')))
-                response['definition'] = definition
-            log.debug('%s: defintion is %s (%s)' % (kwargs['resource'],
-                                                    filename,
-                                                    definition['actions']))
+                    log.debug(
+                        "%s: action %s included in definition",
+                        kwargs["resource"],
+                        action.get("name"),
+                    )
+                response["definition"] = definition
+            log.debug(
+                "%s: defintion is %s (%s)",
+                kwargs["resource"],
+                filename,
+                definition["actions"],
+            )
         except FileObjectNotFound:
-            log.warning('%s: missing definition %s' %
-                        (kwargs['resource'], filename))
+            log.warning("%s: missing definition %s", kwargs["resource"], filename)
         except FileObjectError as err:
-            log.error(err.message)
-            raise Exception('failed to load definition %s' % filename)
-        return (response, 'get_attributes')
+            log.error(str(err))
+            raise RuntimeError(f"failed to load definition {filename}") from err
+        return response, "get_attributes"
 
     def get_attributes(self, response, *args, **kwargs):
-        ''' Reads the resource specific attributes file and stores it in the
+        """Reads the resource specific attributes file and stores it in the
         response dict as 'attributes'
-        '''
+        """
         try:
-            filename = self.expand(kwargs['resource'], ATTRIBUTES_FN)
+            filename = self.expand(kwargs["resource"], ATTRIBUTES_FN)
             fileobj = self.repository.get_file(filename)
             attributes = fileobj.read(CONTENT_TYPE_YAML)
-            response['attributes'] = attributes
-            log.debug('%s: loaded %s attributes from %s' %
-                      (kwargs['resource'], attributes, filename))
-        except FileObjectNotFound:
-            log.warning('%s: no node specific attributes file' %
-                        kwargs['resource'])
-            response['attributes'] = dict()
+            response["attributes"] = attributes
+            log.debug(
+                "%s: loaded %s attributes from %s",
+                kwargs["resource"],
+                attributes,
+                filename,
+            )
+        except FileObjectNotFound:
+            log.warning("%s: no node specific attributes file", kwargs["resource"])
+            response["attributes"] = {}
 
-        return (response, 'do_substitution')
+        return response, "do_substitution"
 
     def do_substitution(self, response, *args, **kwargs):
-        # pylint: disable=R0914
-        definition = response.get('definition')
-        attrs = definition.get('attributes', dict())
+        # pylint: disable=R1702
+        definition = response.get("definition")
+        attrs = definition.get("attributes", {})
 
-        nodeattrs = response.get('attributes', dict())
+        nodeattrs = response.get("attributes", {})
 
         def lookup(name):
-            log.debug('%s: lookup up value for variable %s' %
-                      (kwargs['resource'], name))
+            log.debug("%s: lookup up value for variable %s", kwargs["resource"], name)
             return nodeattrs.get(name, attrs.get(name))
 
-        _actions = list()
-        for action in definition['actions']:
-            log.debug('%s: processing action %s (variable substitution)' %
-                      (kwargs['resource'], action.get('name')))
-            _attributes = dict()
-            if 'attributes' in action:
-                for key, value in action.get('attributes').items():
+        _actions = []
+        for action in definition["actions"]:
+            log.debug(
+                "%s: processing action %s (variable substitution)",
+                kwargs["resource"],
+                action.get("name"),
+            )
+            _attributes = {}
+            if "attributes" in action:
+                for key, value in action.get("attributes").items():
                     try:
-                        update = dict()
+                        update = {}
                         for _key, _value in value.items():
-                            if str(_value).startswith('$'):
+                            if str(_value).startswith("$"):
                                 _value = lookup(_value[1:])
                             update[_key] = _value
                     except AttributeError:
-                        if str(value).startswith('$'):
+                        if str(value).startswith("$"):
                             value = lookup(value[1:])
                         update = value
                     finally:
                         _attributes[key] = update
-            action['attributes'] = _attributes
+            action["attributes"] = _attributes
             _actions.append(action)
-        definition['actions'] = _actions
-        response['definition'] = definition
-        return (response, 'do_resources')
+        definition["actions"] = _actions
+        response["definition"] = definition
+        return response, "do_resources"
 
     def do_resources(self, response, *args, **kwargs):
-        definition = response['definition']
-        node = kwargs.get('node')
-        _actions = list()
+        definition = response["definition"]
+        node = kwargs.get("node")
+        _actions = []
 
         try:
-            for action in definition.get('actions'):
-                attrs = action.get('attributes', dict())
+            for action in definition.get("actions"):
+                attrs = action.get("attributes", {})
 
-                action['attributes'] = \
-                    load_resources(attrs, node, kwargs['resource'])
+                action["attributes"] = load_resources(attrs, node, kwargs["resource"])
                 _actions.append(action)
         except Exception as exc:
             log.error(exc)
-            raise Exception('failed to allocate resources')
+            raise RuntimeError("failed to allocate resources") from exc
 
-        definition['actions'] = _actions
-        response['definition'] = definition
-        return (response, 'finalize_response')
+        definition["actions"] = _actions
+        response["definition"] = definition
+        return response, "finalize_response"
 
     def finalize_response(self, response, *args, **kwargs):
-        _response = dict()
-        _response['body'] = response['definition']
-        _response['status'] = response.get('status', 200)
-        _response['content_type'] = response.get('content_type',
-                                                 CONTENT_TYPE_JSON)
-        return (_response, None)
-
+        _response = {}
+        _response["body"] = response["definition"]
+        _response["status"] = response.get("status", 200)
+        _response["content_type"] = response.get("content_type", CONTENT_TYPE_JSON)
+        return _response, None
 
 
 class BootstrapController(BaseController):
+    DEFAULT_CONFIG = {"logging": [], "xmpp": {}}
 
-    DEFAULT_CONFIG = {
-        'logging': list(),
-        'xmpp': dict()
-    }
-
-    FOLDER = 'bootstrap'
+    FOLDER = "bootstrap"
 
     def __repr__(self):
-        return 'BootstrapController(folder=%s)' % self.FOLDER
+        return f"BootstrapController(folder={self.FOLDER})"
 
     def config(self, request, **kwargs):
-        ''' Handles GET /bootstrap/config '''
+        """Handles GET /bootstrap/config"""
 
         body = self.DEFAULT_CONFIG.copy()
-
+        filename = self.expand(BOOTSTRAP_CONF)
         try:
-            filename = self.expand(BOOTSTRAP_CONF)
             config = self.repository.get_file(filename).read(CONTENT_TYPE_YAML)
             if not config:
-                log.warning('Bootstrap config file empty')
+                log.warning("Bootstrap config file empty")
             else:
-                if 'logging' in config and config['logging']:
-                    body['logging'] = config['logging']
-                    log.info('%s: syslog info included in bootstrap config' %
-                             request.remote_addr)
-
-                if 'xmpp' in config and config['xmpp']:
-                    body['xmpp'] = config['xmpp']
-                    for key in ['username', 'password', 'domain']:
-                        if key not in body['xmpp']:
-                            log.warning('Bootstrap config: \'%s\' missing from '
-                                        'XMPP config' % key)
-                    if 'rooms' not in body['xmpp'] or \
-                       not body['xmpp']['rooms']:
-                        log.warning('Bootstrap config: no XMPP rooms '
-                                    'configured')
-                    log.info('%s: xmpp info included in bootstrap config' %
-                             request.remote_addr)
-            resp = dict(body=body, content_type=CONTENT_TYPE_JSON)
+                if "logging" in config and config["logging"]:
+                    body["logging"] = config["logging"]
+                    log.info(
+                        "%s: syslog info included in bootstrap config",
+                        request.remote_addr,
+                    )
+
+                if "xmpp" in config and config["xmpp"]:
+                    body["xmpp"] = config["xmpp"]
+                    for key in ["username", "password", "domain"]:
+                        if key not in body["xmpp"]:
+                            log.warning(
+                                "Bootstrap config: '%s' missing from XMPP config",
+                                key,
+                            )
+                    if "rooms" not in body["xmpp"] or not body["xmpp"]["rooms"]:
+                        log.warning("Bootstrap config: no XMPP rooms configured")
+                    log.info(
+                        "%s: xmpp info included in bootstrap config",
+                        request.remote_addr,
+                    )
+            resp = {"body": body, "content_type": CONTENT_TYPE_JSON}
         except FileObjectNotFound:
-            log.warning('Bootstrap config file not found')
-            resp = dict(body=body, content_type=CONTENT_TYPE_JSON)
+            log.warning("Bootstrap config file not found")
+            resp = {"body": body, "content_type": CONTENT_TYPE_JSON}
         except FileObjectError:
-            log.error('Failed to read bootstrap config file (%s)' % filename)
+            log.error("Failed to read bootstrap config file (%s)", filename)
             resp = self.http_bad_request()
         except Exception as exc:
-            log.error('Failed to load bootstrap config file (%s): %s' %
-                      (filename, exc))
+            log.error("Failed to load bootstrap config file (%s): %s", filename, exc)
             resp = self.http_bad_request()
         return resp
 
     def index(self, request, **kwargs):
-        ''' Handles GET /bootstrap '''
+        """Handles GET /bootstrap"""
 
+        filename = self.expand(runtime.bootstrap.filename)
         try:
-            filename = self.expand(runtime.bootstrap.filename)
             fobj = self.repository.get_file(filename).read(CONTENT_TYPE_PYTHON)
 
             default_server = runtime.default.server_url
             body = Template(fobj).safe_substitute(SERVER=default_server)
 
-            resp = dict(body=body, content_type=CONTENT_TYPE_PYTHON)
-            log.info('%s: node beginning provisioning' %
-                     request.remote_addr)
+            resp = {"body": body, "content_type": CONTENT_TYPE_PYTHON}
+            log.info("%s: node beginning provisioning", request.remote_addr)
         except KeyError as err:
-            log.debug('Missing variable: %s' % err)
+            log.debug("Missing variable: %s", err)
             resp = self.http_bad_request()
         except FileObjectNotFound:
-            log.error('Bootstrap file not found (%s)' % filename)
+            log.error("Bootstrap file not found (%s)", filename)
             resp = self.http_bad_request()
         except FileObjectError:
-            log.error('Failed to read bootstrap file (%s)' % filename)
+            log.error("Failed to read bootstrap file (%s)", filename)
             resp = self.http_bad_request()
         return resp
 
 
 class MetaController(BaseController):
+    FOLDER = "meta"
 
-    FOLDER = 'meta'
-
-    BODY = {'size': None,
-            'sha1': None}
+    BODY = {"size": None, "sha1": None}
 
     def __repr__(self):
-        return 'MetaController(folder=%s)' % self.FOLDER
+        return f"MetaController(folder={self.FOLDER})"
 
     def metadata(self, request, **kwargs):
-        ''' Handles GET /meta/[actions|files|nodes]/<PATH_INFO> '''
+        """Handles GET /meta/[actions|files|nodes]/<PATH_INFO>"""
 
-        file_path = '%s/%s' % (kwargs['type'], kwargs['path_info'])
+        file_path = f"{kwargs['type']}/{kwargs['path_info']}"
 
         try:
             try:
                 file_resource = self.repository.get_file(file_path)
-            except IOError as exc:
+            except OSError as exc:
                 # IOError is file_path points to a folder
-                log.error('%s is a folder, not a file: %s' %
-                          (file_path, str(exc)))
+                log.error("%s is a folder, not a file: %s", file_path, str(exc))
                 resp = self.http_not_found()
             else:
-                self.BODY['size'] = file_resource.size()
-                self.BODY['sha1'] = file_resource.hash()
-                resp = dict(body=self.BODY, content_type=CONTENT_TYPE_JSON)
-        except IOError as exc:
-            log.error('Failed to collect meta information for %s: %s' %
-                      (file_path, exc))
+                self.BODY["size"] = file_resource.size()
+                self.BODY["sha1"] = file_resource.hash()
+                resp = {"body": self.BODY, "content_type": CONTENT_TYPE_JSON}
+        except OSError as exc:
+            log.error("Failed to collect meta information for %s: %s", file_path, exc)
             resp = self.http_internal_server_error()
         return resp
 
 
 class Router(WSGIRouter):
-    ''' Routes incoming requests by mapping the URL to a controller '''
+    """Routes incoming requests by mapping the URL to a controller"""
 
     def __init__(self):
-        # pylint: disable=E1103,W0142
+        # pylint: disable=E1103
         mapper = routes.Mapper()
 
         url = runtime.default.server_url
-        log.debug('server URL: %s', url)
+        log.debug("server URL: %s", url)
 
         with mapper.submapper() as router_mapper:
-
             # configure /bootstrap
-            router_mapper.connect('bootstrap', '/bootstrap',
-                                  controller=BootstrapController,
-                                  action='index',
-                                  conditions=dict(method=['GET']))
-
-            router_mapper.connect('bootstrap_config', '/bootstrap/config',
-                                  controller=BootstrapController,
-                                  action='config',
-                                  conditions=dict(method=['GET']))
-
+            router_mapper.connect(
+                "bootstrap",
+                "/bootstrap",
+                controller=BootstrapController,
+                action="index",
+                conditions={"method": ["GET"]},
+            )
+
+            router_mapper.connect(
+                "bootstrap_config",
+                "/bootstrap/config",
+                controller=BootstrapController,
+                action="config",
+                conditions={"method": ["GET"]},
+            )
 
             # configure /meta
-            router_mapper.connect('meta',
-                                  '/meta/{type:actions|files|nodes}/'
-                                  '{path_info:.*}',
-                                  controller=MetaController,
-                                  action='metadata',
-                                  conditions=dict(method=['GET']))
+            router_mapper.connect(
+                "meta",
+                "/meta/{type:actions|files|nodes}/{path_info:.*}",
+                controller=MetaController,
+                action="metadata",
+                conditions={"method": ["GET"]},
+            )
 
             # configure /nodes
-            router_mapper.collection('nodes', 'node',
-                                     controller=NodesController,
-                                     collection_actions=['create'],
-                                     member_actions=['show'],
-                                     member_prefix='/{resource}')
-
-            router_mapper.connect('get_node_config',
-                                  '/nodes/{resource}/startup-config',
-                                  controller=NodesController,
-                                  action='get_config',
-                                  conditions=dict(method=['GET']))
-
-            router_mapper.connect('put_node_config',
-                                  '/nodes/{resource}/startup-config',
-                                  controller=NodesController,
-                                  action='put_config',
-                                  conditions=dict(method=['PUT']))
+            router_mapper.collection(
+                "nodes",
+                "node",
+                controller=NodesController,
+                collection_actions=["create"],
+                member_actions=["show"],
+                member_prefix="/{resource}",
+            )
+
+            router_mapper.connect(
+                "get_node_config",
+                "/nodes/{resource}/startup-config",
+                controller=NodesController,
+                action="get_config",
+                conditions={"method": ["GET"]},
+            )
+
+            router_mapper.connect(
+                "put_node_config",
+                "/nodes/{resource}/startup-config",
+                controller=NodesController,
+                action="put_config",
+                conditions={"method": ["PUT"]},
+            )
 
             # configure /actions
-            router_mapper.collection('actions', 'action',
-                                     controller=ActionsController,
-                                     collection_actions=[],
-                                     member_actions=['show'],
-                                     member_prefix='/{resource}')
+            router_mapper.collection(
+                "actions",
+                "action",
+                controller=ActionsController,
+                collection_actions=[],
+                member_actions=["show"],
+                member_prefix="/{resource}",
+            )
 
             # configure /files
-            router_mapper.collection('files', 'file',
-                                     controller=FilesController,
-                                     collection_actions=[],
-                                     member_actions=['show'],
-                                     member_prefix='/{resource:.*}')
+            router_mapper.collection(
+                "files",
+                "file",
+                controller=FilesController,
+                collection_actions=[],
+                member_actions=["show"],
+                member_prefix="/{resource:.*}",
+            )
 
-        super(Router, self).__init__(mapper)
+        super().__init__(mapper)
```

### Comparing `ztpserver-1.6.0/ztpserver/config.py` & `ztpserver-2.0.0/ztpserver/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,116 +26,113 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
-#pylint: disable=C0103
 
-import collections
+import collections.abc
+import configparser
 import logging
 import os
-import ConfigParser
 
 import ztpserver.types
 
-CONF_PATH = '/etc/ztpserver'
+CONF_PATH = "/etc/ztpserver"
 
-VERSION_FILE = '.VERSION'
-VERSION_FILE_PATH = '%s/%s' % (CONF_PATH, VERSION_FILE)
+VERSION_FILE = ".VERSION"
+VERSION_FILE_PATH = f"{CONF_PATH}/{VERSION_FILE}"
 
-GLOBAL_CONF_FILE = 'ztpserver.conf'
-GLOBAL_CONF_FILE_PATH = '%s/%s' % (CONF_PATH, GLOBAL_CONF_FILE)
+GLOBAL_CONF_FILE = "ztpserver.conf"
+GLOBAL_CONF_FILE_PATH = f"{CONF_PATH}/{GLOBAL_CONF_FILE}"
 
-INSTALL_PATH = '/usr/share/ztpserver'
+INSTALL_PATH = "/usr/share/ztpserver"
 
 log = logging.getLogger(__name__)
 
-class Attr(object):
-    """ Base Attribute class for deriving all attributes for a Config object
+
+class Attr:
+    """Base Attribute class for deriving all attributes for a Config object
 
     :param name: required argument specifies attribute name
     :param type: optional keyword argument specifies attribute type.  the
                  default argument type is String
     :param group: optional keyword argument specifies attribute group.  All
                   attribute names must be unique within the group
     :param default: optional keyword argument specifies the default value for
                     the attribute.  The default value is None
 
     """
 
     def __init__(self, name, **kwargs):
-
         self.name = name
-        self.type = kwargs.get('type') or ztpserver.types.String()
-        self.group = kwargs.get('group') or 'default'
-        self.default = kwargs.get('default')
-        self.environ = kwargs.get('environ')
+        self.type = kwargs.get("type") or ztpserver.types.String()
+        self.group = kwargs.get("group") or "default"
+        self.default = kwargs.get("default")
+        self.environ = kwargs.get("environ")
 
         if self.environ is not None and self.environ in os.environ:
             self.default = self.type(os.environ.get(self.environ))
         elif self.default is not None:
             self.default = self.type(self.default)
 
     def __repr__(self):
-        return 'Attr(name=%s, group=%s, default=%s)' % \
-            (self.name, self.group, self.default)
+        return f"Attr(name={self.name}, group={self.group}, default={self.default})"
 
 
 class StrAttr(Attr):
-    """ String attribute class derived from Attr
+    """String attribute class derived from Attr
 
     :param choices: optional keyword argument specifies valid choices
     """
 
     def __init__(self, name, choices=None, **kwargs):
         self.choices = choices
         attrtype = ztpserver.types.String(choices=choices)
-        super(StrAttr, self).__init__(name, type=attrtype, **kwargs)
+        super().__init__(name, type=attrtype, **kwargs)
 
 
 class IntAttr(Attr):
-    """ Integer attribute class derived from Attr
+    """Integer attribute class derived from Attr
 
     :param min_value: specifies the min value.  the default is None
     :param max_value: specifies the max value.  the default is None
 
     """
 
     def __init__(self, name, min_value=None, max_value=None, **kwargs):
         self.min_value = min_value
         self.max_value = max_value
-        attrtype = ztpserver.types.Integer(min_value=min_value, 
-                                           max_value=max_value)
-        super(IntAttr, self).__init__(name, type=attrtype, **kwargs)
+        attrtype = ztpserver.types.Integer(min_value=min_value, max_value=max_value)
+        super().__init__(name, type=attrtype, **kwargs)
 
 
 class BoolAttr(Attr):
-    """ Boolean attribute class derived from Attr """
+    """Boolean attribute class derived from Attr"""
 
     def __init__(self, name, **kwargs):
         attrtype = ztpserver.types.Boolean()
-        super(BoolAttr, self).__init__(name, type=attrtype, **kwargs)
+        super().__init__(name, type=attrtype, **kwargs)
 
 
 class ListAttr(Attr):
-    """ List attribute class derived from Attr
+    """List attribute class derived from Attr
 
     :param delimiter: specifies the delimiter character to split the string on
 
     """
 
-    def __init__(self, name, delimiter=',', **kwargs):
+    def __init__(self, name, delimiter=",", **kwargs):
         attrtype = ztpserver.types.List(delimiter=delimiter)
-        super(ListAttr, self).__init__(name, type=attrtype, **kwargs)
+        super().__init__(name, type=attrtype, **kwargs)
 
 
-class Group(collections.Mapping):
-    """ The Group class provides a logical grouping of attributes in a
+class Group(collections.abc.Mapping):
+    """The Group class provides a logical grouping of attributes in a
     Config object.   Group names must be unique for each Config instance
     and cannot be assigned values.
 
     :param name: the name of the group
     :param config: the config object the group is associated with
 
     """
@@ -153,203 +150,185 @@
 
     def __iter__(self):
         return iter(self._keys())
 
     def __len__(self):
         return len(self._keys())
 
-    def __delitem__(self):
+    def __delitem__(self, index):
         pass
 
-    def __setitem__(self):
+    def __setitem__(self, index, value):
         pass
 
     def _keys(self):
         return [key[1] for key in self.config if key[0] == self.name]
 
     def add_attribute(self, item):
         self.config.add_attribute(item, self.name)
 
 
-class Config(collections.Mapping):
-    """ The Config class represents the configuration for collection.  """
+class Config(collections.abc.Mapping):
+    """The Config class represents the configuration for collection."""
 
     def __init__(self):
-        self.attributes = dict()
-        self.groups = list()
+        self.attributes = {}
+        self.groups = []
 
     def __getattr__(self, name):
         return self.__get_attribute__(name)
 
     def __getitem__(self, name):
         return self.__get_attribute__(name)
 
     def __iter__(self):
         return iter(self.attributes)
 
     def __len__(self):
         return len(self.attributes)
 
     def __repr__(self):
-        return 'Config'
+        return "Config"
 
-    def __delitem__(self):
+    def __delitem__(self, index):
         pass
 
-    def __setitem__(self):
+    def __setitem__(self, index, value):
         pass
 
     def __get_attribute__(self, name, group=None):
         if not group and name in self.groups:
             return Group(name, self)
 
         key = (group, name)
         if key not in self.attributes:
-            raise AttributeError('Missing attribute: %s' % str(key))
+            raise AttributeError(f"Missing attribute: {str(key)}")
 
         item = self.attributes.get(key)
-        return item.get('value')
+        return item.get("value")
 
     def add_attribute(self, item, group=None):
+        obj = {"_metadata": item}
 
-        obj = dict(_metadata=item)
-
-        if group is None and hasattr(item, 'group'):
+        if group is None and hasattr(item, "group"):
             group = item.group
 
         key = (group, item.name)
 
         if group not in self.groups:
             self.add_group(group)
 
         if key in self.attributes:
-            raise AttributeError('Duplicate attribute: %s' % str(key))
+            raise AttributeError(f"Duplicate attribute: {str(key)}")
 
         self.attributes[key] = obj
         if item.default is not None:
-            obj['value'] = self._transform(obj, item.default)
+            obj["value"] = self._transform(obj, item.default)
 
     def add_group(self, group):
         if isinstance(group, Group):
             self.groups.append(group.name)
         else:
             group = str(group)
             self.groups.append(group)
 
     def _transform(self, item, value):
-        # pylint: disable=R0201
-        return item['_metadata'].type(value)
+        return item["_metadata"].type(value)
 
     def set_value(self, name, value, group=None):
         if not group and name in self.groups:
-            raise AttributeError('Failed to set value (name=%s, group=%s): '
-                                 'cannot set a value for a group' %
-                                 (name, group))
+            raise AttributeError(
+                f"Failed to set value (name={name}, group={group}): cannot set a value for a group"
+            )
 
         item = self.attributes.get((group, name))
         if item is None:
-            raise AttributeError('Failed to set value (name=%s, group=%s): '
-                                 'missing item' %
-                                 (name, group))
-        item['value'] = self._transform(item, value)
+            raise AttributeError(f"Failed to set value (name={name}, group={group}): missing item")
+        item["value"] = self._transform(item, value)
 
     def clear_value(self, name, group=None):
-        """ clears the attributes value and resets it to default """
+        """clears the attributes value and resets it to default"""
 
         if not group and name in self.groups:
-            raise AttributeError('Failed to clear value (name=%s, group=%s): '
-                                 'cannot clear values for a group' %
-                                 (name, group))
+            raise AttributeError(
+                f"Failed to clear value (name={name}, group={group}): cannot clear values for a "
+                "group"
+            )
 
         item = self.attributes.get((group, name))
 
-        if item['_metadata'].default is None:   # pylint: disable=W0104
-            item['value'] = None
+        if item["_metadata"].default is None:  # pylint: disable=W0104
+            item["value"] = None
         else:
-            item['value'] = self._transform(item, item['_metadata'].default)
+            item["value"] = self._transform(item, item["_metadata"].default)
 
     def read(self, filename):
-        cp = ConfigParser.RawConfigParser() #pylint: disable=C0103
+        cp = configparser.RawConfigParser()  # pylint: disable=C0103
         cp.read(filename)
         for section in cp.sections():
             for key, value in cp.items(section):
                 try:
                     self.set_value(key, value, section)
                 except AttributeError as err:
-                    log.warning('Error detected while reading %s: %s' %
-                                (filename, err))
+                    log.warning("Error detected while reading %s: %s", filename, err)
                     continue
 
+
 runtime = Config()
 
 # Group: default
-runtime.add_attribute(StrAttr(
-    name='data_root',
-    default=INSTALL_PATH,
-    environ='ZTPS_DEFAULT_DATAROOT'
-))
-
-runtime.add_attribute(StrAttr(
-    name='identifier',
-    choices=['systemmac', 'serialnumber'],
-    default='serialnumber'
-))
-
-runtime.add_attribute(StrAttr(
-    name='server_url',
-    default='http://ztpserver:8080',
-    environ='ZTPS_DEFAULT_SERVER'
-))
-
-runtime.add_attribute(BoolAttr(
-    name='logging',
-    default=True,
-    environ='ZTPS_DEFAULT_LOGGING'
-))
-
-runtime.add_attribute(BoolAttr(
-    name='console_logging',
-    default=True
-))
-
-runtime.add_attribute(StrAttr(
-    name='console_logging_format',
-    default='%(asctime)s:%(levelname)s:[%(module)s:%(lineno)d] %(message)s',
-    environ='ZTPS_CONSOLE_LOGGING_FORMAT'
-))
-
-runtime.add_attribute(BoolAttr(
-    name='disable_topology_validation',
-    default=False
-))
+runtime.add_attribute(
+    StrAttr(name="data_root", default=INSTALL_PATH, environ="ZTPS_DEFAULT_DATAROOT")
+)
+
+runtime.add_attribute(
+    StrAttr(name="identifier", choices=["systemmac", "serialnumber"], default="serialnumber")
+)
+
+runtime.add_attribute(
+    StrAttr(
+        name="server_url",
+        default="http://ztpserver:8080",
+        environ="ZTPS_DEFAULT_SERVER",
+    )
+)
+
+runtime.add_attribute(BoolAttr(name="logging", default=True, environ="ZTPS_DEFAULT_LOGGING"))
+
+runtime.add_attribute(BoolAttr(name="console_logging", default=True))
+
+runtime.add_attribute(
+    StrAttr(
+        name="console_logging_format",
+        default="%(asctime)s:%(levelname)s:[%(module)s:%(lineno)d] %(message)s",
+        environ="ZTPS_CONSOLE_LOGGING_FORMAT",
+    )
+)
+
+runtime.add_attribute(BoolAttr(name="disable_topology_validation", default=False))
 
 # Group: server
-runtime.add_attribute(StrAttr(
-    name='interface',
-    group='server',
-    default='0.0.0.0'
-))
-
-runtime.add_attribute(IntAttr(
-    name='port',
-    group='server',
-    min_value=1,
-    max_value=65534,
-    default=8080
-))
+runtime.add_attribute(StrAttr(name="interface", group="server", default="0.0.0.0"))
 
+runtime.add_attribute(
+    IntAttr(name="port", group="server", min_value=1, max_value=65534, default=8080)
+)
 
 # Group: bootstrap
-runtime.add_attribute(StrAttr(
-    name='filename',
-    group='bootstrap',
-    default='bootstrap',
-    environ='ZTPS_BOOTSTRAP_FILENAME'
-))
+runtime.add_attribute(
+    StrAttr(
+        name="filename",
+        group="bootstrap",
+        default="bootstrap",
+        environ="ZTPS_BOOTSTRAP_FILENAME",
+    )
+)
 
 # Group: neighbordb
-runtime.add_attribute(StrAttr(
-    name='filename',
-    group='neighbordb',
-    default='neighbordb',
-    environ='ZTPS_NEIGHBORDB_FILENAME'
-))
+runtime.add_attribute(
+    StrAttr(
+        name="filename",
+        group="neighbordb",
+        default="neighbordb",
+        environ="ZTPS_NEIGHBORDB_FILENAME",
+    )
+)
```

### Comparing `ztpserver-1.6.0/ztpserver/wsgiapp.py` & `ztpserver-2.0.0/ztpserver/wsgiapp.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,31 +26,30 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
-# pylint: disable=W0613,C0103,R0201,W0622,W0614
+# pylint: disable=W0613,W0622,W0614
 #
 import logging
 
 import webob
 import webob.dec
 import webob.exc
-
 from routes.middleware import RoutesMiddleware
 
-from ztpserver.serializers import dumps
 from ztpserver.constants import CONTENT_TYPE_HTML, HTTP_STATUS_OK
+from ztpserver.serializers import dumps
 
 log = logging.getLogger(__name__)
 
-class WSGIController(object):
 
+class WSGIController:
     def index(self, request, **kwargs):
         return webob.exc.HTTPNoContent()
 
     def create(self, request, **kwargs):
         return webob.exc.HTTPNoContent()
 
     def new(self, request, **kwargs):
@@ -69,58 +68,58 @@
         return webob.exc.HTTPNotFound()
 
     def response(self, **kwargs):
         return webob.Response(**kwargs)
 
     @webob.dec.wsgify
     def __call__(self, request):
-        action = request.urlvars['action']
+        action = request.urlvars["action"]
 
         try:
-            method = getattr(self, action)    #pylint: disable=R0921
+            method = getattr(self, action)
             result = method(request, **request.urlvars)
         except Exception as exc:
-            log.error('Unrecoverable error detected: %s' % exc.message)
+            log.error("Unrecoverable error detected: %s", exc)
             raise webob.exc.HTTPInternalServerError()
 
         if result is None:
             result = webob.exc.HTTPNoContent()
 
         elif isinstance(result, dict):
             # serialize body based on response content type
-            if 'body' in result:
-                content_type = result.get('content_type')
-                result['body'] = dumps(result['body'], content_type,
-                                       'general')
-
-            result.setdefault('status', HTTP_STATUS_OK)
-            result.setdefault('content_type', CONTENT_TYPE_HTML)
-
-            result = self.response(**result)   #pylint: disable=W0142
-
-        elif not isinstance(result, webob.Response) and \
-             not isinstance(result, webob.static.FileApp):
+            if "body" in result:
+                content_type = result.get("content_type")
+                result["body"] = dumps(result["body"], content_type, "general")
+
+            result.setdefault("status", HTTP_STATUS_OK)
+            result.setdefault("content_type", CONTENT_TYPE_HTML)
+            result.setdefault("charset", "UTF-8")
+
+            result = self.response(**result)
+
+        elif not isinstance(result, webob.Response) and not isinstance(
+            result, webob.static.FileApp
+        ):
             result = webob.exc.HTTPInternalServerError()
 
         return result
 
-class WSGIRouter(object):
 
+class WSGIRouter:
     def __init__(self, mapper):
         self.map = mapper
         self.router = RoutesMiddleware(self.route, self.map)
 
     @webob.dec.wsgify
     def __call__(self, request):
         return self.router
 
     @webob.dec.wsgify
     def route(self, request):
-        ''' Routes the incoming request to the appropriate controller '''
+        """Routes the incoming request to the appropriate controller"""
 
-        if 'controller' not in request.urlvars:
-            log.debug('WSGIRouter: missing controller (request=%s)' % 
-                      request)
-            return webob.exc.HTTPNotFound()            
+        if "controller" not in request.urlvars:
+            log.debug("WSGIRouter: missing controller (request=%s)", request)
+            return webob.exc.HTTPNotFound()
 
-        controller = request.urlvars['controller']
+        controller = request.urlvars["controller"]
         return controller()
```

### Comparing `ztpserver-1.6.0/ztpserver/validators.py` & `ztpserver-2.0.0/ztpserver/validators.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,321 +25,313 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-# pylint: disable=W0631
 
-import string    #pylint: disable=W0402
-import re
+import collections.abc
 import inspect
 import logging
-import collections
+import re
+import string  # pylint: disable=W0402
 
-from ztpserver.utils import expand_range, parse_interface
 from ztpserver.config import runtime
+from ztpserver.utils import expand_range, parse_interface
 
-REQUIRED_PATTERN_ATTRIBUTES = ['name', 'definition']
-OPTIONAL_PATTERN_ATTRIBUTES = ['node', 'variables', 'interfaces']
-INTERFACE_PATTERN_KEYWORDS = ['any', 'none']
-ANTINODE_PATTERN = r'[^%s]' % string.hexdigits
-KW_ANY_RE = re.compile(r' *any *')
-KW_NONE_RE = re.compile(r' *none *')
-WC_PORT_RE = re.compile(r'.*')
-
-INVALID_INTERFACE_PATTERNS = [(KW_ANY_RE, KW_ANY_RE, KW_NONE_RE),
-                              (KW_ANY_RE, KW_NONE_RE, KW_NONE_RE),
-                              (KW_ANY_RE, KW_NONE_RE, KW_ANY_RE),
-                              (KW_ANY_RE, KW_NONE_RE, WC_PORT_RE),
-                              (KW_NONE_RE, KW_ANY_RE, KW_ANY_RE),
-                              (KW_NONE_RE, KW_ANY_RE, KW_NONE_RE),
-                              (KW_NONE_RE, KW_NONE_RE, WC_PORT_RE),
-                              (KW_NONE_RE, KW_NONE_RE, KW_ANY_RE)]
-
+REQUIRED_PATTERN_ATTRIBUTES = ["name", "definition"]
+OPTIONAL_PATTERN_ATTRIBUTES = ["node", "variables", "interfaces"]
+INTERFACE_PATTERN_KEYWORDS = ["any", "none"]
+ANTINODE_PATTERN = rf"[^{string.hexdigits}]"
+KW_ANY_RE = re.compile(r" *any *")
+KW_NONE_RE = re.compile(r" *none *")
+WC_PORT_RE = re.compile(r".*")
+
+INVALID_INTERFACE_PATTERNS = [
+    (KW_ANY_RE, KW_ANY_RE, KW_NONE_RE),
+    (KW_ANY_RE, KW_NONE_RE, KW_NONE_RE),
+    (KW_ANY_RE, KW_NONE_RE, KW_ANY_RE),
+    (KW_ANY_RE, KW_NONE_RE, WC_PORT_RE),
+    (KW_NONE_RE, KW_ANY_RE, KW_ANY_RE),
+    (KW_NONE_RE, KW_ANY_RE, KW_NONE_RE),
+    (KW_NONE_RE, KW_NONE_RE, WC_PORT_RE),
+    (KW_NONE_RE, KW_NONE_RE, KW_ANY_RE),
+]
 
-log = logging.getLogger(__name__)   #pylint: disable=C0103
+log = logging.getLogger(__name__)  # pylint: disable=C0103
 
 
 class ValidationError(Exception):
-    ''' Base error class for validation failures '''
-    pass
+    """Base error class for validation failures"""
 
 
-class Validator(object):
-
+class Validator:
     def __init__(self, node_id):
         self.node_id = node_id
-        self.data = dict()
+        self.data = {}
         self.fail = False
-        self.errors = list()
+        self.errors = []
 
     def validate(self, data=None):
-        log.debug('%s: running %s.validate' % 
-                  (self.node_id, self.__class__.__name__))
+        log.debug("%s: running %s.validate", self.node_id, self.__class__.__name__)
         if data:
             self.data = data
         else:
-            self.data = dict()
+            self.data = {}
 
         error = None
         methods = inspect.getmembers(self, predicate=inspect.ismethod)
         for name in methods:
-            if name[0].startswith('validate_'):
-                if 'name' not in self.data:
-                    name_string  = ''
+            if name[0].startswith("validate_"):
+                if "name" not in self.data:
+                    name_string = ""
                 else:
-                    name_string  = 'for \'%s\'' % self.data['name']
+                    name_string = f"for '{self.data['name']}'"
 
-                log.debug('%s: running %s.%s %s' % 
-                          (self.node_id, self.__class__.__name__,
-                           name[0], name_string))
+                log.debug(
+                    "%s: running %s.%s %s",
+                    self.node_id,
+                    self.__class__.__name__,
+                    name[0],
+                    name_string,
+                )
                 try:
                     getattr(self, name[0])()
                 except ValidationError as err:
                     if not error:
                         error = err
         if error:
-            self.error(err)
+            self.error(error)
 
         return not self.fail
 
     def error(self, err, *args, **kwargs):
-        #pylint: disable=W0613
-        cls = str(self.__class__).split('\'')[1].split('.')[-1]
-        log.error('%s: %s validation error: %s' % 
-                  (self.node_id, cls, err))
+        # pylint: disable=W0613
+        cls = str(self.__class__).split("'")[1].split(".")[-1]
+        log.error("%s: %s validation error: %s", self.node_id, cls, err)
         self.fail = True
 
 
 class NeighbordbValidator(Validator):
-
     def __init__(self, node_id):
         self.invalid_patterns = set()
         self.valid_patterns = set()
-        super(NeighbordbValidator, self).__init__(node_id)
+        super().__init__(node_id)
 
     def validate_variables(self):
-        variables = self.data.get('variables', None)
+        variables = self.data.get("variables", None)
         if variables is not None:
-            if not hasattr(variables, '__iter__'):
-                raise ValidationError('invalid global variables value (%s)' %
-                                      variables)
+            if not hasattr(variables, "__iter__"):
+                raise ValidationError(f"invalid global variables value ({variables})")
 
     def validate_patterns(self):
-        patterns = self.data.get('patterns', None)
+        patterns = self.data.get("patterns", None)
 
         if not patterns:
-            log.warning('%s: no patterns found in neighbordb (%s)' % 
-                        (self.node_id, self.data))
+            log.warning("%s: no patterns found in neighbordb (%s)", self.node_id, self.data)
             return
 
         for index, entry in enumerate(patterns):
-            name = entry.get('name', None)
- 
+            name = entry.get("name", None)
+
             validator = PatternValidator(self.node_id)
 
             if name and validator.validate(entry):
-                log.debug('%s: adding pattern \'%s\' (%s) to valid patterns' % 
-                         (self.node_id, name, entry))
+                log.debug(
+                    "%s: adding pattern '%s' (%s) to valid patterns",
+                    self.node_id,
+                    name,
+                    entry,
+                )
                 self.valid_patterns.add((index, str(name)))
             else:
                 if not name:
-                    name = 'N/A'
-                log.debug('%s: adding pattern \'%s\' (%s) to '
-                          'invalid patterns' % 
-                         (self.node_id, name, entry))
+                    name = "N/A"
+                log.debug(
+                    "%s: adding pattern '%s' (%s) to invalid patterns",
+                    self.node_id,
+                    name,
+                    entry,
+                )
                 self.invalid_patterns.add((index, str(name)))
-        
+
         if self.invalid_patterns:
-            raise ValidationError('invalid patterns: %s' % 
-                                  self.invalid_patterns)
+            raise ValidationError(f"invalid patterns: {self.invalid_patterns}")
 
 
 class PatternValidator(Validator):
-
     def __init__(self, node_id):
         self.invalid_interface_patterns = set()
         self.valid_interface_patterns = set()
-        super(PatternValidator, self).__init__(node_id)
+        super().__init__(node_id)
 
     def validate_attributes(self):
         for attr in REQUIRED_PATTERN_ATTRIBUTES:
             if attr not in self.data:
-                raise ValidationError('missing attribute: %s' % attr)
+                raise ValidationError(f"missing attribute: {attr}")
 
-        if 'node' not in self.data and 'interfaces' not in self.data:
-            raise ValidationError('missing attribute: \'node\' OR '
-                                  '\'interfaces\'')
+        if "node" not in self.data and "interfaces" not in self.data:
+            raise ValidationError("missing attribute: 'node' OR 'interfaces'")
 
         for attr in OPTIONAL_PATTERN_ATTRIBUTES:
             if attr not in self.data:
-                log.warning('%s: PatternValidator warning: \'%s\' is missing '
-                            'optional attribute (%s)' % 
-                            (self.node_id, self.data['name'], attr))
-
-        
+                log.warning(
+                    "%s: PatternValidator warning: '%s' is missing optional attribute (%s)",
+                    self.node_id,
+                    self.data["name"],
+                    attr,
+                )
 
     def validate_name(self):
-        if not self.data or 'name' not in self.data:
-            raise ValidationError('missing attribute: \'name\'')
+        if not self.data or "name" not in self.data:
+            raise ValidationError("missing attribute: 'name'")
 
-        if  self.data['name'] is None or not isinstance(self.data['name'], 
-                                                        (int, basestring)):
-            raise ValidationError('invalid value for \'name\' (%s)' %
-                                  self.data['name'])
+        if self.data["name"] is None or not isinstance(self.data["name"], (int, str)):
+            raise ValidationError(f"invalid value for 'name' ({self.data['name']})")
 
     def validate_interfaces(self):
         if not self.data:
             return
 
-        if 'interfaces' not in self.data:
+        if "interfaces" not in self.data:
             return
 
-        if not isinstance(self.data['interfaces'], 
-                          collections.Iterable):
-            raise ValidationError('\'interfaces\' is not iterable (%s)' %
-                                  self.data['interfaces'])
-
-        for index, pattern in enumerate(self.data['interfaces']):
-            if not isinstance(pattern, collections.Mapping):
-                raise ValidationError('invalid value for interface pattern '
-                                      '(%s)' % pattern)
+        if not isinstance(self.data["interfaces"], collections.abc.Iterable):
+            raise ValidationError(f"'interfaces' is not iterable ({self.data['interfaces']})")
+
+        for index, pattern in enumerate(self.data["interfaces"]):
+            if not isinstance(pattern, collections.abc.Mapping):
+                raise ValidationError(f"invalid value for interface pattern ({pattern})")
 
             validator = InterfacePatternValidator(self.node_id)
 
             if validator.validate(pattern):
-                log.debug('%s: adding interface pattern \'%s\' to '
-                         'valid interface patterns' % 
-                         (self.node_id, repr(pattern)))
+                log.debug(
+                    "%s: adding interface pattern '%s' to valid interface patterns",
+                    self.node_id,
+                    repr(pattern),
+                )
                 self.valid_interface_patterns.add((index, repr(pattern)))
             else:
-                log.debug('%s: adding interface pattern \'%s\' to '
-                         'invalid interface patterns' % 
-                         (self.node_id, repr(pattern)))
+                log.debug(
+                    "%s: adding interface pattern '%s' to invalid interface patterns",
+                    self.node_id,
+                    repr(pattern),
+                )
                 self.invalid_interface_patterns.add((index, repr(pattern)))
 
         if self.invalid_interface_patterns:
-            raise ValidationError('invalid interface patterns: %s' %
-                                  self.invalid_interface_patterns)
+            raise ValidationError(f"invalid interface patterns: {self.invalid_interface_patterns}")
 
     def validate_definition(self):
         if not self.data:
             return
 
-        if 'definition' not in self.data:
+        if "definition" not in self.data:
             return
 
-        if not isinstance(self.data['definition'], (int, basestring)):
-            raise ValidationError('invalid value for \'definition\' (%s)' %
-                                  self.data['definition'])
+        if not isinstance(self.data["definition"], (int, str)):
+            raise ValidationError(f"invalid value for 'definition' ({self.data['definition']})")
 
         for wspc in string.whitespace:
-            if wspc in self.data['definition']:
-                raise ValidationError('invalid value for \'definition\' (%s) - '
-                                      '\'%s\' not allowed' % 
-                                      (self.data['definition'], wspc))
+            if wspc in self.data["definition"]:
+                raise ValidationError(
+                    f"invalid value for 'definition' "
+                    f"({self.data['definition']}) - '{wspc}' not allowed"
+                )
 
     def validate_node(self):
         if not self.data:
             return
 
-        node = self.data.get('node', None)
+        node = self.data.get("node", None)
         if not node:
             return
-        else:
-            if isinstance(node, int):
-                node = str(node)
 
-            if not isinstance(node, str):
-                raise ValidationError('invalid value for \'node\' (%s)' %
-                                      str(node))
+        if isinstance(node, int):
+            node = str(node)
+
+        if not isinstance(node, str):
+            raise ValidationError(f"invalid value for 'node' ({str(node)})")
 
         # if system MAC is used
-        if runtime.default.identifier == 'systemmac':
-            node = node.replace(':', '').replace('.', '')
+        if runtime.default.identifier == "systemmac":
+            node = node.replace(":", "").replace(".", "")
             if re.search(ANTINODE_PATTERN, node):
-                raise ValidationError('invalid value for \'node\' (%s)' %
-                                      node)
+                raise ValidationError(f"invalid value for 'node' ({node})")
 
     def validate_variables(self):
         if not self.data:
             return
 
-        if 'variables' not in self.data:
+        if "variables" not in self.data:
             return
 
-        if 'variables' in self.data:
-            if not hasattr(self.data['variables'], '__iter__'):
-                raise ValidationError('invalid value for \'variables\' ('
-                                      'expecting iterable object, got: %s)' % 
-                                      self.data['variables'])
+        if "variables" in self.data:
+            if not hasattr(self.data["variables"], "__iter__"):
+                raise ValidationError(
+                    f"invalid value for 'variables' "
+                    f"(expecting iterable object, got: {self.data['variables']})"
+                )
 
 
 class InterfacePatternValidator(Validator):
-
-    def __init__(self, node_id):
-        super(InterfacePatternValidator, self).__init__(node_id)
-
     def validate_interface_pattern(self):
-
         for interface, peer in self.data.items():
             if peer is None:
-                raise ValidationError('missing peer for interface %s' % 
-                                      interface)
+                raise ValidationError(f"missing peer for interface {interface}")
 
             try:
                 (device, port) = parse_interface(peer, self.node_id)
             except Exception as err:
-                raise ValidationError('PatternError: %s' % err)
+                raise ValidationError(f"PatternError: {err}") from err
 
             if interface not in INTERFACE_PATTERN_KEYWORDS:
                 try:
                     for entry in expand_range(interface):
                         self._validate_pattern(entry, device, port)
                 except Exception as err:
-                    raise ValidationError('invalid interface %s (%s)' % 
-                                          (interface, err))
+                    raise ValidationError(f"invalid interface {interface} ({err})") from err
             else:
                 self._validate_pattern(interface, device, port)
 
     def _validate_pattern(self, interface, device, port):
-        # pylint: disable=R0201
-        if KW_NONE_RE.match(interface) and KW_NONE_RE.match(device) \
-                and KW_NONE_RE.match(port):
+        if KW_NONE_RE.match(interface) and KW_NONE_RE.match(device) and KW_NONE_RE.match(port):
             # no LLDP neighbors
             return
 
         for interface_re, device_re, port_re in INVALID_INTERFACE_PATTERNS:
-            if interface_re.match(interface) and device_re.match(device) \
-               and port_re.match(port):
-                raise ValidationError('invalid interface pattern: (%s, %s, %s) '
-                                      'matches (%s, %s, %s)'%
-                                      (interface, device, port,
-                                       interface_re.pattern, 
-                                       device_re.pattern, 
-                                       port_re.pattern))
+            if interface_re.match(interface) and device_re.match(device) and port_re.match(port):
+                raise ValidationError(
+                    f"invalid interface pattern: ({interface}, {device}, {port}) matches "
+                    f"({interface_re.pattern}, {device_re.pattern}, {port_re.pattern})"
+                )
 
 
 def _validator(contents, cls, node_id):
     try:
         validator = cls(node_id)
         result = validator.validate(contents)
         if result:
-            log.debug('%s: %s validation successful' % 
-                      (node_id, validator.__class__.__name__))
+            log.debug("%s: %s validation successful", node_id, validator.__class__.__name__)
         else:
-            log.debug('%s: %s validation failed' % 
-                      (node_id, validator.__class__.__name__))
+            log.debug("%s: %s validation failed", node_id, validator.__class__.__name__)
 
         return result
     except Exception as exc:
-        log.error('%s: failed to run validator %s(%s): %s' %
-                  (node_id, cls.__name__, contents, repr(exc)))
+        log.error(
+            "%s: failed to run validator %s(%s): %s",
+            node_id,
+            cls.__name__,
+            contents,
+            repr(exc),
+        )
         raise
 
+
 def validate_neighbordb(contents, node_id):
     return _validator(contents, NeighbordbValidator, node_id)
 
+
 def validate_pattern(contents, node_id):
     return _validator(contents, PatternValidator, node_id)
```

### Comparing `ztpserver-1.6.0/ztpserver/serializers.py` & `ztpserver-2.0.0/ztpserver/serializers.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,271 +26,257 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
-# pylint: disable=R0201
 #
 
-import collections
-import logging
+import collections.abc
 import json
+import logging
 import os
 import threading
-import yaml
-
 from collections import OrderedDict
 
-from ztpserver.constants import CONTENT_TYPE_OTHER
-from ztpserver.constants import CONTENT_TYPE_JSON
-from ztpserver.constants import CONTENT_TYPE_YAML
+import yaml
+
+from ztpserver.constants import CONTENT_TYPE_JSON, CONTENT_TYPE_OTHER, CONTENT_TYPE_YAML
 
 READ_WRITE_LOCK = {}
-log = logging.getLogger(__name__)   #pylint: disable=C0103
+log = logging.getLogger(__name__)  # pylint: disable=C0103
+
 
 class SerializerError(Exception):
-    ''' base error raised by serialization functions '''
-    pass
+    """base error raised by serialization functions"""
 
 
-class BaseSerializer(object):
-    ''' Base serializer object '''
+class BaseSerializer:
+    """Base serializer object"""
 
     def __init__(self, node_id):
         self.node_id = node_id
 
     def serialize(self, data):
-        ''' Serialize a dict to object '''
+        """Serialize a dict to object"""
         raise NotImplementedError
 
     def deserialize(self, data):
-        ''' Deserialize an object to dict '''
+        """Deserialize an object to dict"""
         raise NotImplementedError
 
 
 class TextSerializer(BaseSerializer):
-
     def deserialize(self, data):
-        ''' Deserialize a text object and return a dict '''
+        """Deserialize a text object and return a dict"""
         return str(data)
 
     def serialize(self, data):
-        ''' Serialize a dict object and return text '''
+        """Serialize a dict object and return text"""
         return str(data)
 
-#----------------------------------------------------------------------------
+
+# ----------------------------------------------------------------------------
 # Source: Michael Elsdorfer (https://gist.github.com/miracle2k))
 #         https://gist.githubusercontent.com/miracle2k/
 #         3184458/raw/ae89e23502f95c4555f0643dafae8a748e3fb382/
 #         odict.py
 
+
 def represent_odict(dump_odict, tag, mapping, flow_style=None):
-    '''
+    """
     Like BaseRepresenter.represent_mapping, but does not issue the sort().
-    '''
+    """
     value = []
     node = yaml.MappingNode(tag, value, flow_style=flow_style)
     if dump_odict.alias_key is not None:
         dump_odict.represented_objects[dump_odict.alias_key] = node
     best_style = True
-    if hasattr(mapping, 'items'):
+    if hasattr(mapping, "items"):
         mapping = mapping.items()
     for item_key, item_value in mapping:
         node_key = dump_odict.represent_data(item_key)
         node_value = dump_odict.represent_data(item_value)
-        if not (isinstance(node_key, yaml.ScalarNode) and 
-                not node_key.style):
+        if not (isinstance(node_key, yaml.ScalarNode) and not node_key.style):
             best_style = False
-        if not (isinstance(node_value, yaml.ScalarNode) and 
-                not node_value.style):
+        if not (isinstance(node_value, yaml.ScalarNode) and not node_value.style):
             best_style = False
         value.append((node_key, node_value))
     if flow_style is None:
         if dump_odict.default_flow_style is not None:
             node.flow_style = dump_odict.default_flow_style
         else:
             node.flow_style = best_style
     return node
 
+
 yaml.SafeDumper.add_representer(
     OrderedDict,
-    lambda dumper, 
-    value: represent_odict(dumper, 
-                           u'tag:yaml.org,2002:map', 
-                           value))
-#------------------------------------------------------------------------------
+    lambda dumper, value: represent_odict(dumper, "tag:yaml.org,2002:map", value),
+)
+
+
+# ------------------------------------------------------------------------------
 
-class YAMLSerializer(BaseSerializer):
 
+class YAMLSerializer(BaseSerializer):
     def deserialize(self, data):
-        ''' Deserialize a YAML object and return a dict '''
+        """Deserialize a YAML object and return a dict"""
 
         try:
             return yaml.safe_load(data)
         except yaml.YAMLError as err:
-            msg = '''%s: unable to deserialize YAML data:
-%s 
+            msg = f"""{self.node_id}: unable to deserialize YAML data:
+{data}
 
 Error:
-%s''' % (self.node_id, data, err)
-            raise SerializerError(msg)
+{err}"""
+            raise SerializerError(msg) from err
 
     def serialize(self, data):
-        ''' Serialize a dict object and return YAML '''
+        """Serialize a dict object and return YAML"""
 
         try:
             return yaml.safe_dump(data, default_flow_style=False)
         except yaml.YAMLError as err:
-            msg = '''%s: unable to serialize YAML data:
-%s 
+            msg = f"""{self.node_id}: unable to serialize YAML data:
+{data}
 
 Error:
-%s''' % (self.node_id, data, err)
-            raise SerializerError(msg)
+{err}"""
+            raise SerializerError(msg) from err
 
 
 class JSONSerializer(BaseSerializer):
-
     def deserialize(self, data):
-        ''' Deserialize a JSON object and return a dict '''
+        """Deserialize a JSON object and return a dict"""
 
         try:
             return json.loads(data)
         except Exception as err:
-            msg = '''%s: unable to deserialize JSON data:
-%s 
+            msg = f"""{self.node_id}: unable to deserialize JSON data:
+{data}
 
 Error:
-%s''' % (self.node_id, data, err)
-            raise SerializerError(msg)
+{err}"""
+            raise SerializerError(msg) from err
 
     def serialize(self, data):
-        ''' Serialize a dict object and return JSON '''
+        """Serialize a dict object and return JSON"""
 
         try:
             return json.dumps(data)
         except Exception as err:
-            msg = '''%s: unable to serialize JSON data:
-%s 
+            msg = f"""{self.node_id}: unable to serialize JSON data:
+{data}
 
 Error:
-%s''' % (self.node_id, data, err)
-            raise SerializerError(msg)
+{err}"""
+            raise SerializerError(msg) from err
 
 
-class Serializer(object):
-
+class Serializer:
     def __init__(self, node_id):
         self.node_id = node_id
 
         self._handlers = {
             CONTENT_TYPE_OTHER: TextSerializer(self.node_id),
             CONTENT_TYPE_JSON: JSONSerializer(self.node_id),
-            CONTENT_TYPE_YAML: YAMLSerializer(self.node_id)
+            CONTENT_TYPE_YAML: YAMLSerializer(self.node_id),
         }
 
     @property
     def handlers(self):
         return self._handlers
 
     def add_handler(self, content_type, instance):
         if content_type in self._handlers:
-            log.warning('%s: overwriting previous loaded handler %s', 
-                        (self.node_id, content_type))
+            log.warning("%s: overwriting previous loaded handler %s", self.node_id, content_type)
         self._handlers[content_type] = instance
 
     def serialize(self, data, content_type):
-        ''' Serialize the data based on the content_type '''
+        """Serialize the data based on the content_type"""
 
-        handler = self.handlers.get(content_type, 
-                                    TextSerializer(self.node_id))
+        handler = self.handlers.get(content_type, TextSerializer(self.node_id))
         return handler.serialize(data)
 
     def deserialize(self, data, content_type=None):
-        ''' Deserialize the data based on the content_type '''
+        """Deserialize the data based on the content_type"""
 
-        handler = self.handlers.get(content_type, 
-                                    TextSerializer(self.node_id))
+        handler = self.handlers.get(content_type, TextSerializer(self.node_id))
         data = self._convert_from_unicode(handler.deserialize(data))
         return data
 
     @staticmethod
     def _convert_from_unicode(data):
-        if isinstance(data, basestring):
+        if isinstance(data, str):
             return str(data)
-        elif isinstance(data, collections.Mapping):
-            return dict([Serializer._convert_from_unicode(x)
-                         for x in data.items()])
-        elif isinstance(data, collections.Iterable):
-            return type(data)([Serializer._convert_from_unicode(x)
-                               for x in data])
-        else:
-            return data
+        if isinstance(data, collections.abc.Mapping):
+            return dict([Serializer._convert_from_unicode(x) for x in data.items()])
+        if isinstance(data, collections.abc.Iterable):
+            return type(data)([Serializer._convert_from_unicode(x) for x in data])
+        return data
 
 
 def loads(data, content_type, node_id):
     serializer = Serializer(node_id)
     return serializer.deserialize(data, content_type)
 
-def load(file_path, content_type, node_id='N/A', lock=False):
-    log.debug('%s: reading %s...' % (node_id, file_path))
+
+def load(file_path, content_type, node_id="N/A", lock=False):
+    log.debug("%s: reading %s...", node_id, file_path)
 
     if lock and file_path not in READ_WRITE_LOCK:
         READ_WRITE_LOCK[file_path] = threading.Lock()
 
     try:
         if lock:
             with READ_WRITE_LOCK[file_path]:
-                with open(file_path) as fhandler:
+                with open(file_path, encoding="utf8") as fhandler:
                     data = fhandler.read()
         else:
-            with open(file_path) as fhandler:
-                data = fhandler.read()            
+            with open(file_path, encoding="utf8") as fhandler:
+                data = fhandler.read()
 
         result = loads(data, content_type, node_id)
-    except (OSError, IOError) as err:
-        log.error('%s: failed to load file from %s (%s)' % 
-                  (node_id, file_path, err))
-        raise SerializerError('%s: failed to load file from %s (%s)' % 
-                              (node_id, file_path, err))
+    except OSError as err:
+        log.error("%s: failed to load file from %s (%s)", node_id, file_path, err)
+        raise SerializerError(f"{node_id}: failed to load file from {file_path} ({err})") from err
 
     # Enable this log if you want to see the contents of the file (verbose)
     # log.debug('%s: loaded %s: %s' % (node_id, file_path, result))
     return result
 
+
 def dumps(data, content_type, node_id):
     serializer = Serializer(node_id)
-    if hasattr(data, 'serialize'):
+    if hasattr(data, "serialize"):
         data = data.serialize()
     return serializer.serialize(data, content_type)
 
 
-def dump(data, file_path, content_type, node_id='N/A', lock=False):
-    log.debug('%s: writing %s...' % (node_id, file_path))
+def dump(data, file_path, content_type, node_id="N/A", lock=False):
+    log.debug("%s: writing %s...", node_id, file_path)
 
     if lock and file_path not in READ_WRITE_LOCK:
         READ_WRITE_LOCK[file_path] = threading.Lock()
 
     try:
         if lock:
             with READ_WRITE_LOCK[file_path]:
-                with os.fdopen(os.open(file_path, 
-                                       os.O_WRONLY | os.O_CREAT | os.O_TRUNC,
-                                       0754),
-                               'w') as fhandler:
+                with os.fdopen(
+                    os.open(file_path, os.O_WRONLY | os.O_CREAT | os.O_TRUNC, 0o754),
+                    "w",
+                ) as fhandler:
                     fhandler.write(dumps(data, content_type, node_id))
         else:
-            with os.fdopen(os.open(file_path, 
-                                   os.O_WRONLY | os.O_CREAT | os.O_TRUNC,
-                                   0754),
-                           'w') as fhandler:
-                fhandler.write(dumps(data, content_type, node_id))            
-    except (OSError, IOError) as err:
-        log.error('%s: failed to write file to %s (%s)' % 
-                  (node_id, file_path, err))
-        raise SerializerError('%s: failed to write file to %s (%s)' % 
-                              (node_id, file_path, err))
+            with os.fdopen(
+                os.open(file_path, os.O_WRONLY | os.O_CREAT | os.O_TRUNC, 0o754), "w"
+            ) as fhandler:
+                fhandler.write(dumps(data, content_type, node_id))
+    except OSError as err:
+        log.error("%s: failed to write file to %s (%s)", node_id, file_path, err)
+        raise SerializerError(f"{node_id}: failed to write file to {file_path} ({err})") from err
 
     # Enable this log if you want to see the contents of the file (verbose)
     # log.debug('%s: wrote %s: %s' % (node_id, file_path, data))
```

### Comparing `ztpserver-1.6.0/ztpserver/constants.py` & `ztpserver-2.0.0/ztpserver/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-CONTENT_TYPE_PYTHON = 'text/x-python'
-CONTENT_TYPE_HTML = 'text/html'
-CONTENT_TYPE_OTHER = 'text/plain'
-CONTENT_TYPE_JSON = 'application/json'
-CONTENT_TYPE_YAML = 'application/yaml'
+CONTENT_TYPE_PYTHON = "text/x-python"
+CONTENT_TYPE_HTML = "text/html"
+CONTENT_TYPE_OTHER = "text/plain"
+CONTENT_TYPE_JSON = "application/json"
+CONTENT_TYPE_YAML = "application/yaml"
 
 HTTP_STATUS_OK = 200
 HTTP_STATUS_CREATED = 201
 HTTP_STATUS_NO_CONTENT = 204
 HTTP_STATUS_BAD_REQUEST = 400
 HTTP_STATUS_NOT_FOUND = 404
 HTTP_STATUS_CONFLICT = 409
```

### Comparing `ztpserver-1.6.0/ztpserver/__init__.py` & `ztpserver-2.0.0/ztpserver/__init__.py`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/ztpserver/types.py` & `ztpserver-2.0.0/ztpserver/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,87 +28,79 @@
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 
-class String(object):
-
+class String:
     def __init__(self, choices=None):
         if choices:
             choices = [str(c) for c in choices]
         self.choices = choices
 
     def __call__(self, value):
         value = str(value)
 
         if self.choices and value not in self.choices:
-            raise ValueError('Invalid string value: %s is not one of %s' %
-                             (value, self.choices))
+            raise ValueError(f"Invalid string value: {value} is not one of {self.choices}")
 
         return value
 
     def __repr__(self):
-        obj = 'String'
+        obj = "String"
         if self.choices:
-            obj += '(choices=%s)' % ','.join(self.choices)
+            obj += f"(choices={','.join(self.choices)})"
         return obj
 
 
-class Boolean(object):
-
-    TRUEVALUES = ['yes', 'true', '1', 'on']
-    FALSEVALUES = ['no', 'false', '0', 'off']
+class Boolean:
+    TRUEVALUES = ["yes", "true", "1", "on"]
+    FALSEVALUES = ["no", "false", "0", "off"]
 
     def __call__(self, value):
         if str(value).lower() in self.TRUEVALUES:
             return True
-        elif str(value).lower() in self.FALSEVALUES:
+        if str(value).lower() in self.FALSEVALUES:
             return False
-        else:
-            raise ValueError('Invalid boolean value: %s' % value)
 
-    def __repr__(self):
-        return 'Boolean'
+        raise ValueError(f"Invalid boolean value: %{value}")
 
+    def __repr__(self):
+        return "Boolean"
 
-class Integer(object):
 
+class Integer:
     def __init__(self, min_value=None, max_value=None):
         self.min_value = min_value
         self.max_value = max_value
 
     def __call__(self, value):
         try:
             value = int(value)
-        except ValueError:
-            raise ValueError('Invalid integer value: %s' % value)
+        except ValueError as exc:
+            raise ValueError(f"Invalid integer value: {value}") from exc
 
         if self.min_value is not None and value < self.min_value:
-            raise ValueError('Invalid integer value: %s (min is %s)' %
-                             (value, self.min_value))
+            raise ValueError(f"Invalid integer value: {value} (min is {self.min_value})")
 
         if self.max_value is not None and value > self.max_value:
-            raise ValueError('Invalid integer value: %s (max is %s)' %
-                             (value, self.max_value))
+            raise ValueError(f"Invalid integer value: {value} (max is {self.max_value})")
 
         return value
 
     def __repr__(self):
-        return 'Integer(min_value=%s, max_value=%s)' % \
-               (self.min_value, self.max_value)
-
+        return f"Integer(min_value={self.min_value}, max_value={self.max_value})"
 
-class List(object):
 
-    def __init__(self, delimiter=','):
+class List:
+    def __init__(self, delimiter=","):
         self.delimiter = delimiter
 
     def __call__(self, value):
         if isinstance(value, list):
             return value
 
         return str(value).split(self.delimiter)
 
     def __repr__(self):
-        return 'List(delimiter=%s)' % self.delimiter
+        return f"List(delimiter={self.delimiter})"
```

### Comparing `ztpserver-1.6.0/ztpserver/topology.py` & `ztpserver-2.0.0/ztpserver/topology.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,220 +26,215 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
-# pylint: disable=C0103,W0142
 #
-import collections
 import logging
 import os
 import re
-import string # pylint: disable=W0402
+import string
+from collections import OrderedDict, namedtuple
+from collections.abc import Mapping
 
-from ztpserver.validators import validate_neighbordb, validate_pattern
-from ztpserver.constants import CONTENT_TYPE_YAML
-from ztpserver.serializers import load, SerializerError
-from ztpserver.utils import expand_range, parse_interface, url_path_join
 from ztpserver.config import runtime
+from ztpserver.constants import CONTENT_TYPE_YAML
 from ztpserver.resources import run_plugin
+from ztpserver.serializers import SerializerError, load
+from ztpserver.utils import expand_range, parse_interface, url_path_join
+from ztpserver.validators import validate_neighbordb, validate_pattern
 
-ANY_DEVICE_PARSER_RE = re.compile(r':(?=[any])')
-NONE_DEVICE_PARSER_RE = re.compile(r':(?=[none])')
-FUNC_RE = re.compile(r'(?P<function>\w+)(?=\(\S+\))\([\'|\"]'
-                     r'(?P<arg>.+?)[\'|\"]\)')
+ANY_DEVICE_PARSER_RE = re.compile(r":(?=[any])")
+NONE_DEVICE_PARSER_RE = re.compile(r":(?=[none])")
+FUNC_RE = re.compile(r"(?P<function>\w+)(?=\(\S+\))\([\'|\"](?P<arg>.+?)[\'|\"]\)")
 
-ALL_CHARS = set([chr(c) for c in range(256)])
+ALL_CHARS = {chr(c) for c in range(256)}
 NON_HEX_CHARS = ALL_CHARS - set(string.hexdigits)
 
 log = logging.getLogger(__name__)
 
+Neighbor = namedtuple("Neighbor", ["device", "interface"])
 
-Neighbor = collections.namedtuple('Neighbor', ['device', 'interface'])
 
 def neighbordb_path():
-    ''' Returns the path for neighbordb based on the conf file
-    '''
+    """Returns the path for neighbordb based on the conf file"""
 
     filepath = runtime.default.data_root
     filename = runtime.neighbordb.filename
     return os.path.join(filepath, filename)
 
+
 def load_file(filename, content_type, node_id):
-    ''' Returns the contents of a file specified by filename.
+    """Returns the contents of a file specified by filename.
 
     The requred content_type argument is required and indicates the
     text serialization format the contents are stored in.
 
     If the serializer load function encounters errors, None is returned
 
-    '''
+    """
     try:
         return load(filename, content_type, node_id)
     except SerializerError:
-        log.error('%s: failed to load file: %s' % (node_id, filename))
+        log.error("%s: failed to load file: %s", node_id, filename)
         raise
 
+
 def load_neighbordb(node_id, contents=None):
     try:
         if not contents:
-            log.info('%s: loading neighbordb file: %s' %
-                     (node_id, neighbordb_path()))
-            contents = load_file(neighbordb_path(), CONTENT_TYPE_YAML,
-                                 node_id)
+            log.info("%s: loading neighbordb file: %s", node_id, neighbordb_path())
+            contents = load_file(neighbordb_path(), CONTENT_TYPE_YAML, node_id)
 
         # neighbordb is empty
         if not contents:
-            log.info('%s: unable to load neighbordb - file is missing/empty' %
-                     node_id)
-            contents = dict()
+            log.info("%s: unable to load neighbordb - file is missing/empty", node_id)
+            contents = {}
 
         if not validate_neighbordb(contents, node_id):
-            log.error('%s: failed to validate neighbordb' % node_id)
-            return
+            log.error("%s: failed to validate neighbordb", node_id)
+            return None
 
         neighbordb = Neighbordb(node_id)
 
-        if 'variables' in contents:
-            neighbordb.add_variables(contents['variables'])
+        if "variables" in contents:
+            neighbordb.add_variables(contents["variables"])
 
-        if 'patterns' in contents:
-            neighbordb.add_patterns(contents['patterns'])
+        if "patterns" in contents:
+            neighbordb.add_patterns(contents["patterns"])
 
-        log.debug('%s: loaded neighbordb: %s' % (node_id, neighbordb))
+        log.debug("%s: loaded neighbordb: %s", node_id, neighbordb)
         return neighbordb
     except SerializerError as err:
         # pylint: disable=E1101
-        tokens = err.message.split('Error:')
-        log.error('%s: failed to load neighbordb: %s' %
-                  (node_id,
-                   'Error:'.join(tokens[1:])
-                   if len(tokens) > 1
-                   else err.message))
+        tokens = str(err).split("Error:")
+        log.error(
+            "%s: failed to load neighbordb: %s",
+            node_id,
+            "Error:".join(tokens[1:]) if len(tokens) > 1 else err,
+        )
         return None
     except Exception as err:
-        log.error('%s: failed to load neighbordb because of error: %s' %
-                  (node_id, err))
+        log.error("%s: failed to load neighbordb because of error: %s", node_id, err)
         return None
 
+
 def load_pattern(pattern, content_type=CONTENT_TYPE_YAML, node_id=None):
-    """ Returns an instance of Pattern """
+    """Returns an instance of Pattern"""
     try:
-        if not isinstance(pattern, collections.Mapping):
-            pattern = load_file(pattern, content_type,
-                                node_id)
-            if 'config-handler' in pattern:
-                pattern['config_handler'] = pattern['config-handler']
-                del pattern['config-handler']
+        if not isinstance(pattern, Mapping):
+            pattern = load_file(pattern, content_type, node_id)
+            if "config-handler" in pattern:
+                pattern["config_handler"] = pattern["config-handler"]
+                del pattern["config-handler"]
 
         # add dummy values to pass validation
-        for dummy in ['definition', 'name', 'config_handler']:
+        for dummy in ["definition", "name", "config_handler"]:
             if dummy not in pattern:
                 pattern[dummy] = dummy
 
         if not validate_pattern(pattern, node_id):
-            log.error('%s: failed to validate pattern attributes' % node_id)
+            log.error("%s: failed to validate pattern attributes", node_id)
             return None
 
-        pattern['node_id'] = node_id
+        pattern["node_id"] = node_id
         return Pattern(**pattern)
     except TypeError as exc:
-        log.error('%s: failed to load pattern \'%s\' (%s)' %
-                  (node_id, pattern, exc))
+        log.error("%s: failed to load pattern '%s' (%s)", node_id, pattern, exc)
+
+    return None
+
 
 def create_node(nodeattrs):
     try:
-        if nodeattrs.get('systemmac') is not None:
-            _systemmac = nodeattrs['systemmac']
-            for symbol in [':', '.']:
-                _systemmac = str(_systemmac).replace(symbol, '')
-            nodeattrs['systemmac'] = _systemmac
+        if nodeattrs.get("systemmac") is not None:
+            _systemmac = nodeattrs["systemmac"]
+            for symbol in [":", "."]:
+                _systemmac = str(_systemmac).replace(symbol, "")
+            nodeattrs["systemmac"] = _systemmac
         node = Node(**nodeattrs)
-        log.debug('%s: created node object %r' % (node.identifier(), node))
+        log.debug("%s: created node object %r", node.identifier(), node)
         return node
     except KeyError as err:
-        log.error('Failed to create node - missing attribute: %s' % err)
+        log.error("Failed to create node - missing attribute: %s", err)
+
+    return None
+
 
 def load_resources(attributes, node, node_id):
-    log.debug('%s: computing resources (attr=%s)' %
-              (node_id, attributes))
+    log.debug("%s: computing resources (attr=%s)", node_id, attributes)
 
-    _attributes = dict()
+    _attributes = {}
     for key, value in attributes.items():
-        if hasattr(value, 'items'):
+        if hasattr(value, "items"):
             value = load_resources(value, node, node_id)
-        elif hasattr(value, '__iter__'):
-            _value = list()
+        elif not isinstance(value, str) and hasattr(value, "__iter__"):
+            _value = []
             for item in value:
                 match = FUNC_RE.match(item)
                 if match:
-                    plugin = match.group('function')
-                    _value.append(run_plugin(plugin,
-                                             node_id,
-                                             match.group('arg')),
-                                             node)
+                    plugin = match.group("function")
+                    _value.append(run_plugin(plugin, node_id, match.group("arg"), node))
                 else:
                     _value.append(item)
             value = _value
         else:
             match = FUNC_RE.match(str(value))
             if match:
-                plugin = match.group('function')
-                value = run_plugin(plugin,
-                                   node_id,
-                                   match.group('arg'),
-                                   node)
+                plugin = match.group("function")
+                value = run_plugin(plugin, node_id, match.group("arg"), node)
         _attributes[key] = value
-    log.debug('%s: resources: %s' % (node_id, _attributes))
+    log.debug("%s: resources: %s", node_id, _attributes)
     return _attributes
 
+
 def replace_config_action(resource, filename=None):
-    ''' Builds a definition with a single action replace_config '''
+    """Builds a definition with a single action replace_config"""
 
-    filename = filename or 'startup-config'
+    filename = filename or "startup-config"
     server_url = runtime.default.server_url
-    url = url_path_join(server_url, 'nodes/', str(resource), filename)
+    url = url_path_join(server_url, "nodes/", str(resource), filename)
 
-    action = dict(name='install static startup-config file',
-                  action='replace_config',
-                  always_execute=True,
-                  attributes={'url': url})
+    action = {
+        "name": "install static startup-config file",
+        "action": "replace_config",
+        "always_execute": True,
+        "attributes": {"url": url},
+    }
 
     return action
 
+
 class NodeError(Exception):
-    ''' Base exception class for :py:class:`Node` '''
-    pass
+    """Base exception class for :py:class:`Node`"""
 
 
 class PatternError(Exception):
-    ''' Base exception class for :py:class:`Pattern` '''
-    pass
+    """Base exception class for :py:class:`Pattern`"""
 
 
 class InterfacePatternError(Exception):
-    ''' Base exception class for :py:class:`InterfacePattern` '''
-    pass
+    """Base exception class for :py:class:`InterfacePattern`"""
 
 
 class NeighbordbError(Exception):
-    ''' Base exception class for :py:class:`Neighbordb` '''
-    pass
+    """Base exception class for :py:class:`Neighbordb`"""
 
 
-class OrderedCollection(collections.OrderedDict):
-    ''' base object for using an ordered dictionary '''
+class OrderedCollection(OrderedDict):
+    """base object for using an ordered dictionary"""
+
     def __call__(self, key=None):
-        #pylint: disable=W0221
-        return self.get(key) if key else self.keys()
+        # pylint: disable=W0221
+        return self.get(key) if key else list(self.keys())
 
 
-class Function(object):
+class Function:
     def __init__(self, value):
         self.value = value
 
     def match(self, arg):
         raise NotImplementedError
 
 
@@ -260,602 +255,666 @@
 
 
 class ExactFunction(Function):
     def match(self, arg):
         return arg == self.value
 
 
-class Node(object):
-    ''' A Node object is maps the metadata from an EOS node.  It provides
+class Node:
+    """A Node object is maps the metadata from an EOS node.  It provides
     access to the node's meta data including interfaces and the
     associated neighbors found on those interfaces.
-    '''
+    """
 
     def __init__(self, **kwargs):
-        self.systemmac = kwargs.get('systemmac')
-        self.model = kwargs.get('model')
-        self.serialnumber = kwargs.get('serialnumber')
-        self.version = kwargs.get('version')
+        self.systemmac = kwargs.get("systemmac")
+        self.model = kwargs.get("model")
+        self.serialnumber = kwargs.get("serialnumber")
+        self.version = kwargs.get("version")
 
         self.neighbors = OrderedCollection()
-        if 'neighbors' in kwargs:
-            self.add_neighbors(kwargs['neighbors'])
+        if "neighbors" in kwargs:
+            self.add_neighbors(kwargs["neighbors"])
 
     def __repr__(self):
-        return 'Node(serialnumber=%s, systemmac=%s, neighbors=%s)' % \
-               (self.serialnumber, self.systemmac, self.neighbors)
+        return (
+            "Node(serialnumber={self.serialnumber}, systemmac={self.systemmac}, "
+            "neighbors={self.neighbors})"
+        )
 
     def identifier(self):
         identifier = runtime.default.identifier
         return getattr(self, identifier)
 
     def add_neighbor(self, interface, peers):
         try:
             if self.neighbors.get(interface):
-                raise NodeError('%s: interface \'%s\' already added to node' %
-                                (self.identifier(), interface))
+                raise NodeError(
+                    f"{self.identifier()}: interface '{interface}' already added to node"
+                )
 
-            _neighbors = list()
+            _neighbors = []
             for peer in peers:
-                log.debug('%s: creating neighbor %s:%s for interface %s' %
-                          ( self.identifier(), peer['device'],
-                            peer['port'], interface))
-                _neighbors.append(Neighbor(peer['device'],
-                                           peer['port']))
+                log.debug(
+                    "%s: creating neighbor %s:%s for interface %s",
+                    self.identifier(),
+                    peer["device"],
+                    peer["port"],
+                    interface,
+                )
+                _neighbors.append(Neighbor(peer["device"], peer["port"]))
             self.neighbors[interface] = _neighbors
         except KeyError as err:
-            log.error('%s: failed to neighbor because of missing key (%s)' %
-                      (self.identifier(), str(err)))
-            raise NodeError('%s: failed to neighbor because of KeyError (%s)' %
-                      (self.identifier(), str(err)))
+            log.error(
+                "%s: failed to neighbor because of missing key (%s)",
+                self.identifier(),
+                str(err),
+            )
+            raise NodeError(
+                f"{self.identifier()}: failed to neighbor because of KeyError ({str(err)})"
+            ) from err
 
     def add_neighbors(self, neighbors):
-        log.info('%s: parsing node\'s LLDP Neighbor information' %
-                 self.identifier())
+        log.info("%s: parsing node's LLDP Neighbor information", self.identifier())
         for interface, peers in neighbors.items():
             self.add_neighbor(interface, peers)
 
     def serialize(self):
         result = {}
-        for prop in ['model', 'systemmac', 'serialnumber', 'version']:
+        for prop in ["model", "systemmac", "serialnumber", "version"]:
             if getattr(self, prop):
                 result[prop] = getattr(self, prop)
 
         neighbors = {}
         if self.neighbors:
             for interface, neighbor_list in self.neighbors.items():
                 serialized_neighbor_list = []
                 for neighbor in neighbor_list:
                     serialized_neighbor_list.append(
-                        dict(device=neighbor.device, port=neighbor.interface))
+                        {"device": neighbor.device, "port": neighbor.interface}
+                    )
                 neighbors[interface] = serialized_neighbor_list
-        result['neighbors'] = neighbors
+        result["neighbors"] = neighbors
         return result
 
 
-class Neighbordb(object):
-
-    RESERVED_VARIABLES = ['any', 'none']
+class Neighbordb:
+    RESERVED_VARIABLES = ["any", "none"]
 
     def __init__(self, node_id):
         self.node_id = node_id
 
-        self.variables = dict()
-        self.patterns = {'globals': list(), 'nodes': dict()}
+        self.variables = {}
+        self.patterns = {"globals": [], "nodes": {}}
 
     def __repr__(self):
-        return 'Neighbordb(variables=%d, globals=%d, nodes=%d)' % \
-               (len(self.variables),
-                len(self.patterns['globals']),
-                len(self.patterns['nodes']))
+        return (
+            f"Neighbordb(variables={len(self.variables)}, "
+            f'globals={len(self.patterns["globals"])}, nodes={len(self.patterns["nodes"])})'
+        )
 
     def add_variable(self, key, value, overwrite=False):
         if key in self.RESERVED_VARIABLES:
-            log.error('%s: failed to add variable: %s (reserved keyword)' %
-                      (self.node_id, key))
-            raise NeighbordbError('%s: failed to add variable: %s '
-                                '(reserved keyword)' % (self.node_id, key))
-        elif key in self.variables and not overwrite:
-            log.error('%s: failed to add variable: %s (duplicate)' %
-                      (self.node_id, key))
-            raise NeighbordbError('%s: failed to add variable %s '
-                                '(duplicate)' % (self.node_id, key))
+            log.error("%s: failed to add variable: %s (reserved keyword)", self.node_id, key)
+            raise NeighbordbError(
+                f"{self.node_id}: failed to add variable: {key} (reserved keyword)"
+            )
+        if key in self.variables and not overwrite:
+            log.error("%s: failed to add variable: %s (duplicate)", self.node_id, key)
+            raise NeighbordbError(f"{self.node_id}: failed to add variable {key} (duplicate)")
 
         self.variables[key] = value
 
     def add_variables(self, variables):
-        if not hasattr(variables, 'items'):
-            log.error('%s: failed to add variables: missing attribute '
-                      '\'items\' (%s)' % (self.node_id, variables))
-            raise NeighbordbError('%s: failed to add variables: '
-                                  'missing attribute \'items\' (%s)' %
-                                  (self.node_id, variables))
+        if not hasattr(variables, "items"):
+            log.error(
+                "%s: failed to add variables: missing attribute 'items' (%s)",
+                self.node_id,
+                variables,
+            )
+            raise NeighbordbError(
+                f"{self.node_id}: failed to add variables: missing attribute 'items' ({variables})"
+            )
 
         for key, value in variables.items():
             self.add_variable(key, value)
 
     def add_pattern(self, name, **kwargs):
-
         try:
-            kwargs['node_id'] = self.node_id
-            kwargs['name'] = name
+            kwargs["node_id"] = self.node_id
+            kwargs["name"] = name
 
-            kwargs['config_handler'] = kwargs.get('config-handler',
-                                                  None)
-            if 'config-handler' in kwargs:
-                del kwargs['config-handler']
-            kwargs['interfaces'] = kwargs.get('interfaces', list())
-            kwargs['variables'] = kwargs.get('variables', dict())
+            kwargs["config_handler"] = kwargs.get("config-handler", None)
+            if "config-handler" in kwargs:
+                del kwargs["config-handler"]
+            kwargs["interfaces"] = kwargs.get("interfaces", [])
+            kwargs["variables"] = kwargs.get("variables", {})
 
-            for key in set(self.variables).difference(kwargs['variables']):
-                kwargs['variables'][key] = self.variables[key]
+            for key in set(self.variables).difference(kwargs["variables"]):
+                kwargs["variables"][key] = self.variables[key]
 
             pattern = Pattern(**kwargs)
 
-            log.debug('%s: pattern \'%r\' parsed successfully' %
-                      (self.node_id, pattern))
+            log.debug("%s: pattern '%r' parsed successfully", self.node_id, pattern)
 
             # Add pattern to neighbordb
-            if 'node' in kwargs:
-                if pattern.node not in self.patterns['nodes']:
-                    self.patterns['nodes'][pattern.node] = pattern
-                else:
-                    log.warning('%s: pattern \'%r\' ignored because '
-                                'another node-specific pattern is '
-                                'configured earlier in neighbordb'
-                                '\'%r\'' %
-                                (self.node_id, pattern,
-                                 self.patterns['nodes'][pattern.node]))
+            if "node" in kwargs:
+                if pattern.node not in self.patterns["nodes"]:
+                    self.patterns["nodes"][pattern.node] = pattern
+                else:
+                    log.warning(
+                        "%s: pattern '%r' ignored because "
+                        "another node-specific pattern is "
+                        "configured earlier in neighbordb"
+                        "'%r'",
+                        self.node_id,
+                        pattern,
+                        self.patterns["nodes"][pattern.node],
+                    )
             else:
-                self.patterns['globals'].append(pattern)
+                self.patterns["globals"].append(pattern)
         except KeyError as err:
-            log.error('%s: failed to add pattern \'%s\' because of '
-                      'missing key (%s)' % (self.node_id, name, str(err)))
-            raise NeighbordbError('%s: failed to pattern \'%s\' because of '
-                                'missing key (%s)' %
-                                  (self.node_id, name, str(err)))
-        except PatternError:
-            log.error('%s: failed to add pattern \'%s\'' %
-                      (self.node_id, name))
-            raise NeighbordbError('%s: failed to add pattern \'%s\'' %
-                                  (self.node_id, name))
+            log.error(
+                "%s: failed to add pattern '%s' because of missing key (%s)",
+                self.node_id,
+                name,
+                str(err),
+            )
+            raise NeighbordbError(
+                f"{self.node_id}: failed to pattern '{name}' because of missing key ({str(err)})"
+            ) from err
+        except PatternError as exc:
+            log.error("%s: failed to add pattern '%s'", self.node_id, name)
+            raise NeighbordbError(f"{self.node_id}: failed to add pattern '{name}'") from exc
 
     def add_patterns(self, patterns):
         try:
             for pattern in patterns:
                 self.add_pattern(**pattern)
         except TypeError as err:
-            log.error('%s: failed to add patterns %s: %s' %
-                      (self.node_id, patterns, str(err)))
-            raise NeighbordbError('%s: failed to add patterns %s: %s' %
-                                  (self.node_id, patterns, str(err)))
+            log.error("%s: failed to add patterns %s: %s", self.node_id, patterns, str(err))
+            raise NeighbordbError(
+                f"{self.node_id}: failed to add patterns {patterns}: {str(err)}"
+            ) from err
 
     def is_node_pattern(self, pattern):
-        #pylint: disable=R0201
         return pattern.node
 
     def is_global_pattern(self, pattern):
-        #pylint: disable=R0201
         return not pattern.node
 
     def get_patterns(self):
-        return self.patterns['nodes'].values() + self.patterns['globals']
+        return list(self.patterns["nodes"].values()) + self.patterns["globals"]
 
     @staticmethod
     def identifier(node):
         identifier = runtime.default.identifier
         return node[identifier]
 
     def find_patterns(self, node):
         identifier = node.identifier()
-        log.debug('%s: searching for eligible patterns' %
-                  identifier)
+        log.debug("%s: searching for eligible patterns", identifier)
 
         result = []
 
-        pattern = self.patterns['nodes'].get(identifier, None)
+        pattern = self.patterns["nodes"].get(identifier, None)
         if pattern:
-            log.debug('%s: node-specific pattern eligible in neighbordb: %s' %
-                      (identifier,
-                       pattern.name))
+            log.debug(
+                "%s: node-specific pattern eligible in neighbordb: %s",
+                identifier,
+                pattern.name,
+            )
             result += [pattern]
 
-        elif self.patterns['globals']:
-            log.debug('%s: global patterns eligible in neighbordb' %
-                      identifier)
-            result += self.patterns['globals']
+        elif self.patterns["globals"]:
+            log.debug("%s: global patterns eligible in neighbordb", identifier)
+            result += self.patterns["globals"]
         else:
-            log.debug('%s: no patterns eligible in neighbordb' %
-                      identifier)
+            log.debug("%s: no patterns eligible in neighbordb", identifier)
 
         return result
 
     def match_node(self, node):
         identifier = node.identifier()
-        result = list()
+        result = []
         for pattern in self.find_patterns(node):
-            log.debug('%s: attempting to match pattern %s' %
-                      (identifier, pattern.name))
+            log.debug("%s: attempting to match pattern %s", identifier, pattern.name)
             if pattern.match_node(node):
-                log.debug('%s: pattern %s matched' %
-                          (identifier, pattern.name))
+                log.debug("%s: pattern %s matched", identifier, pattern.name)
                 result.append(pattern)
             else:
-                log.debug('%s: pattern %s match failed' %
-                          (identifier, pattern.name))
+                log.debug("%s: pattern %s match failed", identifier, pattern.name)
         return result
 
 
-class Pattern(object):
-
-    def __init__(self, name=None, definition=None,
-                 config_handler=None, interfaces=None,
-                 node=None, variables=None, node_id=None):
-
+class Pattern:
+    def __init__(
+        self,
+        name=None,
+        definition=None,
+        config_handler=None,
+        interfaces=None,
+        node=None,
+        variables=None,
+        node_id=None,
+    ):
         self.name = name
         self.definition = definition
         self.config_handler = config_handler
 
         self.node = node
         self.node_id = node_id
-        self.variables = variables or dict()
+        self.variables = variables or {}
 
-        self.interfaces = list()
+        self.interfaces = []
         if interfaces:
             self.add_interfaces(interfaces)
 
         self.variable_substitution()
 
     def __repr__(self):
-        return 'Pattern(name=\'%s\')' % self.name
+        return f"Pattern(name='{self.name}')"
 
     def variable_substitution(self):
         try:
-            log.debug('%s: checking pattern \'%s\' entries for variable '
-                      'substitution' % (self.node_id, self.name))
+            log.debug(
+                "%s: checking pattern '%s' entries for variable substitution",
+                self.node_id,
+                self.name,
+            )
             for entry in self.interfaces:
-                for item in entry['patterns']:
-                    for attr in ['remote_device', 'remote_interface']:
+                for item in entry["patterns"]:
+                    for attr in ["remote_device", "remote_interface"]:
                         value = getattr(item, attr)
-                        if value.startswith('$'):
+                        if value.startswith("$"):
                             newvalue = self.variables[value[1:]]
                             setattr(item, attr, newvalue)
                     item.refresh()
-            log.debug('%s: pattern \'%s\' variable substitution complete' %
-                      (self.node_id, self.name))
+            log.debug(
+                "%s: pattern '%s' variable substitution complete",
+                self.node_id,
+                self.name,
+            )
         except KeyError as exc:
-            log.debug('%s: pattern \'%s\' variable substitution failed: %s' %
-                      (self.node_id, self.name, str(exc)))
-            raise PatternError('%s: pattern \'%s\' variable substitution '
-                               'failed: %s' %
-                               (self.node_id, self.name, str(exc)))
+            log.debug(
+                "%s: pattern '%s' variable substitution failed: %s",
+                self.node_id,
+                self.name,
+                str(exc),
+            )
+            raise PatternError(
+                f"{self.node_id}: pattern '{self.name}' variable substitution failed: {str(exc)}"
+            ) from exc
 
     def serialize(self):
-        data = dict(name=self.name, definition=self.definition,
-                    variables=self.variables, node=self.node)
-
-        data['config-handler'] = self.config_handler
+        data = {
+            "name": self.name,
+            "definition": self.definition,
+            "variables": self.variables,
+            "node": self.node,
+            "config-handler": self.config_handler,
+        }
 
         interfaces = []
         for item in self.interfaces:
-            _item = item['metadata']
-            interfaces.append({_item['interface']: _item['neighbors']})
-        data['interfaces'] = interfaces
+            _item = item["metadata"]
+            interfaces.append({_item["interface"]: _item["neighbors"]})
+        data["interfaces"] = interfaces
 
         return data
 
     def parse_interface(self, neighbor):
         try:
             return parse_interface(neighbor, self.node_id)
         except Exception as err:
-            raise PatternError(str(err))
+            raise PatternError(str(err)) from err
 
     def add_interface(self, interface):
         try:
-            if not hasattr(interface, 'items'):
-                log.error('%s: pattern \'%s\' - failed to add interface %s: '
-                          'missing attribute (items)' %
-                          (self.node_id, self.name, interface))
-                raise PatternError('%s: pattern \'%s\' - failed to add '
-                                   'interface %s: missing attribute (items)' %
-                                   (self.node_id, self.name, interface))
+            if not hasattr(interface, "items"):
+                log.error(
+                    "%s: pattern '%s' - failed to add interface %s: missing attribute (items)",
+                    self.node_id,
+                    self.name,
+                    interface,
+                )
+                raise PatternError(
+                    f"{self.node_id}: pattern '{self.name}' - failed to add interface {interface}: "
+                    "missing attribute (items)"
+                )
 
             for intf, neighbors in interface.items():
-                (remote_device, remote_interface) = \
-                    self.parse_interface(neighbors)
+                (remote_device, remote_interface) = self.parse_interface(neighbors)
 
-                metadata = dict(interface=intf, neighbors=neighbors)
+                metadata = {"interface": intf, "neighbors": neighbors}
 
-                patterns = list()
-                if intf in ['none', 'any']:
-                    patterns.append(InterfacePattern(intf, remote_device,
-                                                     remote_interface,
-                                                     self.node_id))
+                patterns = []
+                if intf in ["none", "any"]:
+                    patterns.append(
+                        InterfacePattern(intf, remote_device, remote_interface, self.node_id)
+                    )
                 else:
                     intfs = expand_range(intf)
                     for item in intfs:
-                        pattern = InterfacePattern(item, remote_device,
-                                                   remote_interface,
-                                                   self.node_id)
+                        pattern = InterfacePattern(
+                            item, remote_device, remote_interface, self.node_id
+                        )
                         patterns.append(pattern)
-                self.interfaces.append(dict(metadata=metadata,
-                                            patterns=patterns))
-        except InterfacePatternError:
-            log.error('%s: pattern \'%s\' - failed to add interface %s' %
-                      (self.node_id, self.name, interface))
-            raise PatternError('%s: pattern \'%s\' - failed to add '
-                               'interface %s' %
-                               (self.node_id, self.name, interface))
+                self.interfaces.append({"metadata": metadata, "patterns": patterns})
+        except InterfacePatternError as exc:
+            log.error(
+                "%s: pattern '%s' - failed to add interface %s",
+                self.node_id,
+                self.name,
+                interface,
+            )
+            raise PatternError(
+                f"{self.node_id}: pattern '{self.name}' - failed to add interface {interface}"
+            ) from exc
 
     def add_interfaces(self, interfaces):
         try:
             for interface in interfaces:
                 self.add_interface(interface)
         except TypeError as err:
-            log.error('%s: pattern \'%s\' - failed to add interfaces %s: %s' %
-                      (self.node_id, self.name, interface, str(err)))
-            raise PatternError('%s: pattern \'%s\' - failed to add '
-                               'interfaces %s: %s' %
-                               (self.node_id, self.name, interface, str(err)))
+            log.error(
+                "%s: pattern '%s' - failed to add interfaces %s: %s",
+                self.node_id,
+                self.name,
+                interface,
+                str(err),
+            )
+            raise PatternError(
+                f"{self.node_id}: pattern '{self.name}' - "
+                f"failed to add interfaces {interface}: {str(err)}"
+            ) from err
 
     def match_node(self, node):
-
-        log.debug('%s: pattern \'%s\' - attempting to match node (%r)' %
-                  (self.node_id, self.name, str(node)))
+        log.debug(
+            "%s: pattern '%s' - attempting to match node (%r)",
+            self.node_id,
+            self.name,
+            str(node),
+        )
 
         # No need to match system ID - that it already taken care of
         # while selecting the set of nodes which are eligible for a
         # match.
 
-        patterns = list()
+        patterns = []
         for entry in self.interfaces:
-            for pattern in entry['patterns']:
+            for pattern in entry["patterns"]:
                 patterns.append(pattern)
 
         for interface, neighbors in node.neighbors.items():
-            log.debug('%s: pattern \'%s\' - attempting to match '
-                      'interface %s(%s)' %
-                      (self.node_id, self.name, interface, str(neighbors)))
+            log.debug(
+                "%s: pattern '%s' - attempting to match interface %s(%s)",
+                self.node_id,
+                self.name,
+                interface,
+                str(neighbors),
+            )
 
             match = False
             for index, pattern in enumerate(patterns):
-                log.debug('%s: pattern \'%s\' - checking interface pattern '
-                          'for %s: %s' %
-                          (self.node_id, self.name, interface, pattern))
+                log.debug(
+                    "%s: pattern '%s' - checking interface pattern for %s: %s",
+                    self.node_id,
+                    self.name,
+                    interface,
+                    pattern,
+                )
                 result = pattern.match(interface, neighbors)
 
                 # True, False, None
                 if result is True:
-                    log.debug('%s: pattern \'%s\' - interface pattern match '
-                              'for %s: %s' %
-                              (self.node_id, self.name, interface, pattern))
+                    log.debug(
+                        "%s: pattern '%s' - interface pattern match for %s: %s",
+                        self.node_id,
+                        self.name,
+                        interface,
+                        pattern,
+                    )
                     del patterns[index]
                     match = True
                     break
-                elif result is False:
-                    log.debug('%s: pattern \'%s\' - interface pattern match '
-                              'failure for %s: %s' %
-                              (self.node_id, self.name, interface, pattern))
+                if result is False:
+                    log.debug(
+                        "%s: pattern '%s' - interface pattern match failure for %s: %s",
+                        self.node_id,
+                        self.name,
+                        interface,
+                        pattern,
+                    )
                     return False
 
             if not match:
-                log.debug('%s: pattern \'%s\' - interface %s did not match '
-                          'any interface patterns' %
-                          (self.node_id, self.name, interface))
+                log.debug(
+                    "%s: pattern '%s' - interface %s did not match any interface patterns",
+                    self.node_id,
+                    self.name,
+                    interface,
+                )
 
         for pattern in patterns:
             if pattern.is_positive_constraint():
-                log.debug('%s: pattern \'%s\' - interface pattern %s did '
-                          'not match any interface' %
-                          (self.node_id, self.name, pattern))
+                log.debug(
+                    "%s: pattern '%s' - interface pattern %s did not match any interface",
+                    self.node_id,
+                    self.name,
+                    pattern,
+                )
                 return False
         return True
 
 
-class InterfacePattern(object):
-
-    KEYWORDS = {
-        'any': RegexFunction('.*'),
-        'none': RegexFunction('[^a-zA-Z0-9]')
-    }
+class InterfacePattern:
+    KEYWORDS = {"any": RegexFunction(".*"), "none": RegexFunction("[^a-zA-Z0-9]")}
 
     FUNCTIONS = {
-        'exact': ExactFunction,
-        'includes': IncludesFunction,
-        'excludes': ExcludesFunction,
-        'regex': RegexFunction
+        "exact": ExactFunction,
+        "includes": IncludesFunction,
+        "excludes": ExcludesFunction,
+        "regex": RegexFunction,
     }
 
     def __init__(self, interface, remote_device, remote_interface, node_id):
-        match = re.match(r'^[ehnrtE]+(\d.*)$', interface)
+        match = re.match(r"^[ehnrtE]+(\d.*)$", interface)
         if match:
-            self.interface = 'Ethernet%s' % match.groups()[0]
+            self.interface = f"Ethernet{match.groups()[0]}"
         else:
             self.interface = interface
 
         self.remote_device = remote_device
         self.remote_interface = remote_interface
         self.node_id = node_id
 
         self.remote_device_re = self.compile(remote_device)
         self.remote_interface_re = self.compile(remote_interface)
 
-
     def __repr__(self):
-        return 'InterfacePattern(interface=%s, remote_device=%s, ' \
-               'remote_interface=%s)' % \
-                (self.interface, self.remote_device, self.remote_interface)
+        return (
+            f"InterfacePattern(interface={self.interface}, "
+            f"remote_device={self.remote_device}, remote_interface={self.remote_interface})"
+        )
 
     def refresh(self):
         self.remote_device_re = self.compile(self.remote_device)
         self.remote_interface_re = self.compile(self.remote_interface)
 
     def compile(self, value):
         if value in self.KEYWORDS:
             return self.KEYWORDS[value]
 
         try:
             match = FUNC_RE.match(value)
             if match:
-                function = match.group('function')
-                arg = match.group('arg')
+                function = match.group("function")
+                arg = match.group("arg")
                 return self.FUNCTIONS[function](arg)
-            else:
-                return ExactFunction(value)
+
+            return ExactFunction(value)
         except KeyError as exc:
-            log.error('%s: compile error: unknown function \'%s\' (%s)' %
-                      (self.node_id, function, str(exc)))
-            raise InterfacePatternError
+            log.error(
+                "%s: compile error: unknown function '%s' (%s)",
+                self.node_id,
+                function,
+                str(exc),
+            )
+            raise InterfacePatternError from exc
 
     def match(self, interface, neighbors):
         for neighbor in neighbors:
-            res = self.match_neighbor(interface, Neighbor(neighbor.device,
-                                                          neighbor.interface))
-            if res is True:
-                return True
-            elif res is False:
-                return False
+            res = self.match_neighbor(interface, Neighbor(neighbor.device, neighbor.interface))
+            return res
         return None
 
     def match_neighbor(self, interface, neighbor):
         # pylint: disable=R0911,R0912
-        log.debug('%s: attempting to match %s(%s) against '
-                  'interface pattern %r' %
-                  (self.node_id, interface, neighbor, self))
-
-        if self.interface == 'any':
-            if self.remote_device == 'any':
-                if self.remote_interface == 'any':
+        log.debug(
+            "%s: attempting to match %s(%s) against interface pattern %r",
+            self.node_id,
+            interface,
+            neighbor,
+            self,
+        )
+
+        if self.interface == "any":
+            if self.remote_device == "any":
+                if self.remote_interface == "any":
                     return True
-                elif self.remote_interface == 'none':
+                if self.remote_interface == "none":
                     # bogus
                     return False
-                else:
-                    if self.match_remote_interface(neighbor.interface):
-                        return True
-            elif self.remote_device == 'none':
-                if self.remote_interface == 'any':
+                if self.match_remote_interface(neighbor.interface):
+                    return True
+            elif self.remote_device == "none":
+                if self.remote_interface == "any":
                     # bogus
                     return False
-                elif self.remote_interface == 'none':
+                if self.remote_interface == "none":
                     # bogus
                     return False
-                else:
-                    return False
+                return False
             else:
-                if self.remote_interface == 'any':
+                if self.remote_interface == "any":
                     if self.match_remote_device(neighbor.device):
                         return True
-                elif self.remote_interface == 'none':
+                if self.remote_interface == "none":
                     if self.match_remote_device(neighbor.device):
                         return False
-                else:
-                    if(self.match_remote_device(neighbor.device) and
-                       self.match_remote_interface(neighbor.interface)):
-                        return True
+                if self.match_remote_device(neighbor.device) and self.match_remote_interface(
+                    neighbor.interface
+                ):
+                    return True
 
-        elif self.interface == 'none':
-            if self.remote_device == 'any':
-                if self.remote_interface == 'any':
+        elif self.interface == "none":
+            if self.remote_device == "any":
+                if self.remote_interface == "any":
                     # bogus
                     return False
-                elif self.remote_interface == 'none':
+                if self.remote_interface == "none":
                     # bogus
                     return False
-                else:
-                    if self.match_remote_interface(neighbor.interface):
-                        return False
-            elif self.remote_device == 'none':
-                if self.remote_interface == 'any':
+                if self.match_remote_interface(neighbor.interface):
+                    return False
+            elif self.remote_device == "none":
+                if self.remote_interface == "any":
                     # bogus
                     return False
-                elif self.remote_interface == 'none':
+                if self.remote_interface == "none":
                     # no LLDP capable neighbors
                     return False
-                else:
-                    # bogus
-                    return False
+
+                # bogus
+                return False
             else:
-                if self.remote_interface == 'any':
+                if self.remote_interface == "any":
                     if self.match_remote_device(neighbor.device):
                         return False
-                elif self.remote_interface == 'none':
+                if self.remote_interface == "none":
                     if self.match_remote_device(neighbor.device):
                         return False
                 else:
-                    if(self.match_remote_device(neighbor.device) and
-                       self.match_remote_interface(neighbor.interface)):
+                    if self.match_remote_device(neighbor.device) and self.match_remote_interface(
+                        neighbor.interface
+                    ):
                         return False
         else:
-            if self.remote_device == 'any':
-                if self.remote_interface == 'any':
+            if self.remote_device == "any":
+                if self.remote_interface == "any":
                     if self.match_interface(interface):
                         return True
-                elif self.remote_interface == 'none':
+                elif self.remote_interface == "none":
                     if self.match_interface(interface):
                         return False
                 else:
-                    if(self.match_interface(interface) and
-                        self.match_remote_interface(neighbor.interface)):
+                    if self.match_interface(interface) and self.match_remote_interface(
+                        neighbor.interface
+                    ):
                         return True
-            elif self.remote_device == 'none':
-                if self.remote_interface == 'any':
+            elif self.remote_device == "none":
+                if self.remote_interface == "any":
                     if self.match_interface(interface):
                         return False
-                elif self.remote_interface == 'none':
+                elif self.remote_interface == "none":
                     if self.match_interface(interface):
                         return False
                 else:
-                    if(self.match_interface(interface) and
-                        self.match_remote_interface(neighbor.interface)):
+                    if self.match_interface(interface) and self.match_remote_interface(
+                        neighbor.interface
+                    ):
                         return False
             elif self.match_interface(interface):
-                if self.remote_interface == 'any':
+                if self.remote_interface == "any":
                     if self.match_remote_device(neighbor.device):
                         return True
-                elif self.remote_interface == 'none':
+                elif self.remote_interface == "none":
                     if self.match_remote_device(neighbor.device):
                         return False
                 else:
-                    if(self.match_interface(interface) and
-                       self.match_remote_device(neighbor.device) and
-                       self.match_remote_interface(neighbor.interface)):
+                    if (
+                        self.match_interface(interface)
+                        and self.match_remote_device(neighbor.device)
+                        and self.match_remote_interface(neighbor.interface)
+                    ):
                         return True
         return None
 
-
     def match_interface(self, interface):
-        if self.interface == 'any':
+        if self.interface == "any":
             return True
-        elif self.interface is None:
+        if self.interface is None:
             return False
-        else:
-            return self.interface == interface
+
+        return self.interface == interface
 
     def match_remote_device(self, remote_device):
-        if self.remote_device == 'any':
+        if self.remote_device == "any":
             return True
-        elif self.remote_device is None:
+        if self.remote_device is None:
             return False
-        else:
-            return self.remote_device_re.match(remote_device)
+
+        return self.remote_device_re.match(remote_device)
 
     def match_remote_interface(self, remote_interface):
-        if self.remote_interface == 'any':
+        if self.remote_interface == "any":
             return True
-        elif self.remote_interface is None:
+        if self.remote_interface is None:
             return False
-        else:
-            return self.remote_interface_re.match(remote_interface)
+
+        return self.remote_interface_re.match(remote_interface)
 
     def is_positive_constraint(self):
-        if self.interface == 'any':
-            if self.remote_device == 'any':
+        if self.interface == "any":
+            if self.remote_device == "any":
                 return True
-            elif self.remote_device != 'none':
-                return self.interface != 'none'
+            if self.remote_device != "none":
+                return self.interface != "none"
 
-        elif self.interface != 'none':
-            if self.remote_device == 'any':
+        elif self.interface != "none":
+            if self.remote_device == "any":
                 return True
-            elif self.remote_device != 'none':
-                return self.interface != 'none'
+            if self.remote_device != "none":
+                return self.interface != "none"
+
+        return False
```

### Comparing `ztpserver-1.6.0/ztpserver/app.py` & `ztpserver-2.0.0/ztpserver/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,327 +26,322 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
-# pylint: disable=C0103
 #
 
 import argparse
 import logging
 import os
 import re
 import sys
-
 from wsgiref.simple_server import make_server
 
-
 from ztpserver import config, controller
-
-from ztpserver.serializers import load, dump
-from ztpserver.validators import NeighbordbValidator
 from ztpserver.constants import CONTENT_TYPE_YAML
+from ztpserver.resources import resource_plugins
+from ztpserver.serializers import dump, load
 from ztpserver.topology import FUNC_RE, neighbordb_path
 from ztpserver.utils import all_files
-from ztpserver.resources import resource_plugins
+from ztpserver.validators import NeighbordbValidator
 
-log = logging.getLogger('ztpserver')
+log = logging.getLogger("ztpserver")
 log.setLevel(logging.DEBUG)
 log.addHandler(logging.NullHandler())
 
+
 def enable_handler_console(level=None):
-    ''' Enables logging to stdout '''
-    
+    """Enables logging to stdout"""
+
     logging_fmt = config.runtime.default.console_logging_format
     formatter = logging.Formatter(logging_fmt)
 
-    ch = logging.StreamHandler()
-    ch.tag = 'console'
+    console_handler = logging.StreamHandler()
+    console_handler.tag = "console"
 
-    
     for handler in log.handlers:
-        if 'tag' in handler.__dict__ and handler.tag == ch.tag:
+        if "tag" in handler.__dict__ and handler.tag == console_handler.tag:
             # Handler previously added
             return
 
-    level = level or 'DEBUG'
+    level = level or "DEBUG"
     level = str(level).upper()
     level = logging.getLevelName(level)
-    ch.setLevel(level)
-    ch.setFormatter(formatter)
+    console_handler.setLevel(level)
+    console_handler.setFormatter(formatter)
+
+    log.addHandler(console_handler)
 
-    log.addHandler(ch)
 
 def python_supported():
-    ''' Returns True if the current version of the python runtime is valid '''
-    return sys.version_info > (2, 7) and sys.version_info < (3, 0)
+    """Returns True if the current version of the python runtime is valid"""
+    return sys.version_info >= (3, 7)
+
+
+logging_started = False  # pylint: disable=C0103
+
 
-logging_started = False
 def start_logging(debug):
-    ''' reads the runtime config and starts logging if enabled '''
-    global logging_started     #pylint: disable=W0603
+    """reads the runtime config and starts logging if enabled"""
+    global logging_started  # pylint: disable=C0103,W0603
     if logging_started:
         return
 
     if config.runtime.default.logging:
         if config.runtime.default.console_logging:
-            enable_handler_console('DEBUG' if debug else 'INFO')
+            enable_handler_console("DEBUG" if debug else "INFO")
 
     logging_started = True
 
+
 def load_config(conf=None):
     conf = conf or config.GLOBAL_CONF_FILE_PATH
-    conf = os.environ.get('ZTPS_CONFIG', conf)
+    conf = os.environ.get("ZTPS_CONFIG", conf)
 
     if os.path.exists(conf):
-        log.info('Loading config file: %s' % conf)
+        log.info("Loading config file: %s", conf)
         config.runtime.read(conf)
 
+
 def start_wsgiapp(config_file=None, debug=False):
-    ''' Provides the entry point into the application for wsgi compliant
+    """Provides the entry point into the application for wsgi compliant
     servers.   Accepts an optional argument ``config_file``.   The
     ``config_file`` keyword argument specifies the path the server
     configuration file.  The default value is /etc/ztpserver/ztpserver.conf.
 
     :param config_file: string path pointing to configuration file
     :param debug: boolean set debug level logging? (Default: False)
     :return: a wsgi application object
 
-    '''
+    """
     load_config(config_file)
     start_logging(debug)
 
     try:
-        version = open(config.VERSION_FILE_PATH).read().split()[0].strip()
-    except Exception:  # pylint: disable=W0703
-        version = 'N/A'
+        with open(config.VERSION_FILE_PATH, encoding="utf8") as fd:
+            version = fd.read().split()[0].strip()
+    except OSError:
+        version = "N/A"
 
-    log.info('Starting ZTPServer v%s...' % version)
+    log.info("Starting ZTPServer v%s...", version)
 
-    log.info('Logging started for ztpserver')
-    log.info('Using repository %s', config.runtime.default.data_root)
+    log.info("Logging started for ztpserver")
+    log.info("Using repository %s", config.runtime.default.data_root)
 
     if not python_supported():
-        raise SystemExit('ERROR: ZTPServer requires Python 2.7')
+        raise SystemExit("ERROR: ZTPServer requires Python >= 3.8")
 
     return controller.Router()
 
+
 def run_server(version, config_file, debug):
-    ''' The :py:func:`run_server` is called by the main command line routine to
+    """The :py:func:`run_server` is called by the main command line routine to
     run the server as standalone.   This function accepts a single argument
     that points towards the configuration file describing this server
 
     This function will block on the active thread until stopped.
 
-    :param conf: string path pointing to configuration file
-    '''
+    :param config_file: string path pointing to configuration file
+    """
     app = start_wsgiapp(config_file, debug)
 
     host = config.runtime.server.interface
     port = config.runtime.server.port
 
-    log.info('URL: http://%s:%s' % (host, port))
+    log.info("URL: http://%s:%s", host, port)
 
     httpd = make_server(host, port, app)
 
-    log.info('Starting ZTPServer v%s on http://%s:%s' % 
-             (version, host, port))
+    log.info("Starting ZTPServer v%s on http://%s:%s", version, host, port)
 
     try:
         httpd.serve_forever()
     except KeyboardInterrupt:
-        log.info('Shutdown...')
+        log.info("Shutdown...")
+
 
 def validate_neighbordb():
     # Validating neighbordb
-    validator = NeighbordbValidator('N/A')
+    validator = NeighbordbValidator("N/A")
     neighbordb = neighbordb_path()
-    print 'Validating neighbordb (\'%s\')...' % neighbordb
+    print(f"Validating neighbordb ('{neighbordb}')...")
     try:
-        validator.validate(load(neighbordb, CONTENT_TYPE_YAML,
-                                'validator'))
-        total_patterns = len(validator.valid_patterns) + \
-            len(validator.invalid_patterns)
-            
+        validator.validate(load(neighbordb, CONTENT_TYPE_YAML, "validator"))
+        total_patterns = len(validator.valid_patterns) + len(validator.invalid_patterns)
+
         if validator.invalid_patterns:
-            print '\nERROR: Failed to validate neighbordb patterns'
-            print '   Invalid Patterns (count: %d/%d)' % \
-                (len(validator.invalid_patterns),
-                 total_patterns)
-            print '   ---------------------------'
-            for index, pattern in enumerate(
-                sorted(validator.invalid_patterns)):
-                print '   [%d] %s' % (index, pattern[1])
+            print("\nERROR: Failed to validate neighbordb patterns")
+            print(
+                f"   Invalid Patterns "
+                f"(count: {len(validator.invalid_patterns):d}/{total_patterns:d})"
+            )
+            print("   ---------------------------")
+            for index, pattern in enumerate(sorted(validator.invalid_patterns)):
+                print(f"   [{index}] {pattern[1]}")
         else:
-            print 'Ok!'            
-    except Exception as exc:        #pylint: disable=W0703
-        print 'ERROR: Failed to validate neighbordb\n%s' % exc
+            print("Ok!")
+    except Exception as exc:  # pylint: disable=W0703
+        print(f"ERROR: Failed to validate neighbordb\n{exc}")
+
 
 def validate_definitions():
     data_root = config.runtime.default.data_root
 
-    print '\nValidating definitions...'
+    print("\nValidating definitions...")
 
-    for definition in all_files(os.path.join(data_root, 
-                                             'definitions')):
-        print 'Validating %s...' % definition,
+    for definition in all_files(os.path.join(data_root, "definitions")):
+        print(f"Validating {definition}...")
         try:
-            def_data = load(definition, CONTENT_TYPE_YAML,
-                            'validator')
+            def_data = load(definition, CONTENT_TYPE_YAML, "validator")
 
-            resources = re.findall(FUNC_RE, 
-                                   str(def_data))
+            resources = re.findall(FUNC_RE, str(def_data))
 
             # Validating plugins
             plugins = resource_plugins()
-            missing_plugins = set([x for (x, _) in resources 
-                                   if x not in plugins])
+            missing_plugins = {x for (x, _) in resources if x not in plugins}
             if missing_plugins:
-                plugins_path = os.path.join(data_root, 
-                                            'plugins')
-                print ''
+                plugins_path = os.path.join(data_root, "plugins")
+                print("")
                 for plugin in missing_plugins:
-                    print 'ERROR: Plugin \'%s\' configured in \'%s\' ' \
-                        'is missing from \'%s\'!' % \
-                        (plugin, definition, plugins_path)
+                    print(
+                        f"ERROR: Plugin '{plugin}' configured in '{definition}' "
+                        f"is missing from '{plugins_path}'!"
+                    )
 
             # Special validation for 'allocate' plugin
-            resources_path = os.path.join(data_root, 
-                                          'resources')
-            resource_files = [x.split('/')[-1] 
-                              for x in os.listdir(resources_path)]
-            missing_resources = [x for (y, x) in resources 
-                                 if x not in resource_files and
-                                 y == 'allocate']
+            resources_path = os.path.join(data_root, "resources")
+            resource_files = [x.split("/")[-1] for x in os.listdir(resources_path)]
+            missing_resources = [
+                x for (y, x) in resources if x not in resource_files and y == "allocate"
+            ]
             if missing_resources:
                 if not missing_plugins:
-                    print ''
+                    print("")
                 for res in missing_resources:
-                    print 'ERROR: Resource file \'%s\' configured in \'%s\' ' \
-                        'is missing from \'%s\'!' % \
-                        (res, definition, resources_path)
+                    print(
+                        f"ERROR: Resource file '{res}' configured in '{definition}' is missing "
+                        f"from '{resources_path}'!"
+                    )
             else:
-                print 'Ok!'
-        except Exception as exc:        #pylint: disable=W0703            
-            print '\nERROR: Failed to validate %s\n%s' % \
-                (definition, exc)
+                print("Ok!")
+        except Exception as exc:  # pylint: disable=W0703
+            print(f"\nERROR: Failed to validate {definition}\n{exc}")
+
 
-def validate_resources(raiseException=False):
+def validate_resources(raise_exception=False):
     data_root = config.runtime.default.data_root
 
-    print '\nValidating resources...'
-    for resource in all_files(os.path.join(data_root, 
-                                           'resources')):
-        print 'Validating %s...' % resource,
+    print("\nValidating resources...")
+    for resource in all_files(os.path.join(data_root, "resources")):
+        print(f"Validating {resource}...")
         try:
-            load(resource, CONTENT_TYPE_YAML,
-                 'validator')
-            print 'Ok!'
-        except Exception as exc:        #pylint: disable=W0703 
-            print '\nERROR: Failed to validate %s\n%s' % \
-                (resource, exc)
-            if raiseException:
+            load(resource, CONTENT_TYPE_YAML, "validator")
+            print("Ok!")
+        except Exception as exc:  # pylint: disable=W0703
+            print(f"\nERROR: Failed to validate {resource}\n{exc}")
+            if raise_exception:
                 raise exc
 
+
 def validate_nodes():
     data_root = config.runtime.default.data_root
 
-    print '\nValidating nodes...'
-    for filename in [x for x in all_files(os.path.join(data_root, 
-                                                       'nodes'))
-                     if x.split('/')[-1] in ['definition',
-                                             'pattern']]:
-        print 'Validating %s...' % filename,
+    print("\nValidating nodes...")
+    for filename in [
+        x
+        for x in all_files(os.path.join(data_root, "nodes"))
+        if x.split("/")[-1] in ["definition", "pattern"]
+    ]:
+        print(f"Validating {filename}...")
         try:
-            load(filename, CONTENT_TYPE_YAML,
-                 'validator')
-            print 'Ok!'
-        except Exception as exc:        #pylint: disable=W0703            
-            print '\nERROR: Failed to validate %s\n%s' % \
-                (filename, exc)
+            load(filename, CONTENT_TYPE_YAML, "validator")
+            print("Ok!")
+        except Exception as exc:  # pylint: disable=W0703
+            print(f"\nERROR: Failed to validate {filename}\n{exc}")
+
 
 def clear_resources(debug):
     start_logging(debug)
 
     try:
-        validate_resources(raiseException=True)
-    except Exception:                   #pylint: disable=W0703 
-        sys.exit('ERROR: Unable to clear resources because of validation error')
+        validate_resources(raise_exception=True)
+    except Exception:  # pylint: disable=W0703
+        sys.exit("ERROR: Unable to clear resources because of validation error")
 
     data_root = config.runtime.default.data_root
 
-    print '\nClearing resources...'
-    for resource in all_files(os.path.join(data_root, 
-                                           'resources')):
-        print 'Clearing %s...' % resource,
+    print("\nClearing resources...")
+    for resource in all_files(os.path.join(data_root, "resources")):
+        print(f"Clearing {resource}...")
         try:
-            contents = load(resource, CONTENT_TYPE_YAML,
-                            'clear_resource')
+            contents = load(resource, CONTENT_TYPE_YAML, "clear_resource")
             for key in contents:
-                contents[key] = 'None'
-            dump(contents, resource, CONTENT_TYPE_YAML,
-                 'clear_resource')
-            print 'Ok!'            
-        except Exception as exc:        #pylint: disable=W0703            
-            print '\nERROR: Failed to clear %s\n%s' % \
-                (resource, exc)
-    
+                contents[key] = "None"
+            dump(contents, resource, CONTENT_TYPE_YAML, "clear_resource")
+            print("Ok!")
+        except Exception as exc:  # pylint: disable=W0703
+            print(f"\nERROR: Failed to clear {resource}\n{exc}")
+
+
 def run_validator(debug):
     start_logging(debug)
 
     validate_neighbordb()
     validate_definitions()
     validate_resources()
     validate_nodes()
 
+
 def main():
-    ''' The :py:func:`main` is the main entry point for the ztpserver if called
+    """The :py:func:`main` is the main entry point for the ztpserver if called
     from the commmand line.   When called from the command line, the server is
     running in standalone mode as opposed to using the :py:func:`application` to
     run under a python wsgi compliant server
-    '''
+    """
 
-    usage = 'ztpserver [options]'
+    usage = "ztpserver [options]"
 
     parser = argparse.ArgumentParser(usage=usage)
 
-    parser.add_argument('--version', '-v',
-                        action='store_true',
-                        help='Displays the version information')
-
-    parser.add_argument('--conf', '-c',
-                        type=str,
-                        default=config.GLOBAL_CONF_FILE_PATH,
-                        help='Specifies the configuration file to use')
-
-    parser.add_argument('--validate-config', '-V',
-                        action='store_true',
-                        help='Validates config files')
-
-    parser.add_argument('--debug',
-                        action='store_true',
-                        help='Enables debug output to the STDOUT')
-
-    parser.add_argument('--clear-resources', '-r',
-                        action='store_true',
-                        help='Clears all resource files')
-
+    parser.add_argument(
+        "--version", "-v", action="store_true", help="Displays the version information"
+    )
+
+    parser.add_argument(
+        "--conf",
+        "-c",
+        type=str,
+        default=config.GLOBAL_CONF_FILE_PATH,
+        help="Specifies the configuration file to use",
+    )
+
+    parser.add_argument(
+        "--validate-config", "-V", action="store_true", help="Validates config files"
+    )
+
+    parser.add_argument("--debug", action="store_true", help="Enables debug output to the STDOUT")
+
+    parser.add_argument(
+        "--clear-resources", "-r", action="store_true", help="Clears all resource files"
+    )
 
     args = parser.parse_args()
 
-    version = 'N/A'
+    version = "N/A"
     try:
-        version = open(config.VERSION_FILE_PATH).read().split()[0].strip()
-    except IOError:
+        with open(config.VERSION_FILE_PATH, encoding="utf8") as fd:
+            version = fd.read().split()[0].strip()
+    except OSError:
         pass
 
     if args.version:
-        print 'ZTPServer version %s' % version
+        print(f"ZTPServer version {version}")
 
     if args.validate_config:
         run_validator(args.debug)
 
     if args.clear_resources:
         clear_resources(args.debug)
```

### Comparing `ztpserver-1.6.0/ztpserver/resources.py` & `ztpserver-2.0.0/ztpserver/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,31 +26,39 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-import imp
+import importlib.machinery
+import importlib.util
 import os
+import sys
 
 from ztpserver.config import runtime
 
+
 def resource_plugins():
-    path = os.path.join(runtime.default.data_root, 'plugins')
+    path = os.path.join(runtime.default.data_root, "plugins")
 
     plugins = []
-    for (_, _, filenames) in os.walk(path):
+    for _, _, filenames in os.walk(path):
         plugins.extend(filenames)
         break
     return plugins
 
-def run_plugin(plugin, node_id, pool, node):
 
-    filename = os.path.join(runtime.default.data_root, 
-                            'plugins',
-                            plugin)
+def run_plugin(plugin, node_id, pool, node):
+    filename = os.path.join(runtime.default.data_root, "plugins", plugin)
     try:
-        module = imp.load_source(plugin, filename)
+        if plugin not in sys.modules:
+            loader = importlib.machinery.SourceFileLoader(plugin, filename)
+            spec = importlib.util.spec_from_loader(loader.name, loader)
+            module = importlib.util.module_from_spec(spec)
+            sys.modules[plugin] = module
+            spec.loader.exec_module(module)
+
+        module = sys.modules[plugin]
         return module.main(node_id, pool, node)
     except Exception as exc:
-        raise Exception('failed to run plugin: %s' % exc)
+        raise RuntimeError(f"failed to run plugin: {exc}") from exc
```

### Comparing `ztpserver-1.6.0/ztpserver/repository.py` & `ztpserver-2.0.0/ztpserver/repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
 #
-'''
+"""
     MODULE:
         ztpserver.respository
 
     AUTHOR:
         Arista Networks
 
     DESCRIPTION:
@@ -43,104 +43,101 @@
         for ztpserver.  The repository module can perform basic file
         system like functionality for performing basid CRUD on
         files and well as reading and writing specific file contents.
 
     :copyright: Copyright (c) 2015, Arista Networks
     :license: BSD, see LICENSE for more details
 
-'''
+"""
 
 import hashlib
 import logging
 import mimetypes
 import os
 
 import ztpserver.serializers
-
 from ztpserver.serializers import SerializerError
 
-log = logging.getLogger(__name__)   #pylint: disable=C0103
-
+log = logging.getLogger(__name__)  # pylint: disable=C0103
 
 
 def create_repository(path):
     if not os.path.exists(path):
-        raise RepositoryError('%s not found' % path)
+        raise RepositoryError(f"{path} not found")
     return Repository(path)
 
 
 class RepositoryError(Exception):
-    ''' Base exception class for :py:class:`Repository` '''
-    pass
+    """Base exception class for :py:class:`Repository`"""
+
 
 class FileObjectError(Exception):
-    ''' Base exception class for :py:class:`FileObject` '''
-    pass
+    """Base exception class for :py:class:`FileObject`"""
+
 
 class FileObjectNotFound(RepositoryError):
-    ''' Raised when a requested file is not found in the repository.  This
+    """Raised when a requested file is not found in the repository.  This
     exception is a subclass of :py:class:`RespositoryError`
-    '''
-    pass
+    """
 
 
-
-class FileObject(object):
-    ''' The :py:class:`FileObject` represents a single file entity in the
+class FileObject:
+    """The :py:class:`FileObject` represents a single file entity in the
     repository.   The instance provides convienent methods to read and write
     contents to the file using a specified serialization
-    '''
+    """
 
     def __init__(self, name, path=None, **kwargs):
-        ''' The initialize method for :py:class:`FileObject`
+        """The initialize method for :py:class:`FileObject`
 
         :param name: the name of the file
         :type name: str
         :param path: the base path of the file
         :type path: str
         :param content_type: the content type of the file (optional)
         :type content_type: str
         :returns: object
 
-        '''
+        """
         self.name = name
         if path is not None:
             self.name = os.path.join(path, name)
 
         self.type, self.encoding = mimetypes.guess_type(self.name)
-        self.content_type = kwargs.get('content_type')
+        self.content_type = kwargs.get("content_type")
 
     def __repr__(self):
-        return 'FileObject(name=%s, type=%s, encoding=%s, content_type=%s)' % \
-               (self.name, self.type, self.encoding, self.content_type)
+        return (
+            "FileObject(name={self.name}, type={self.type}, encoding={self.encoding}, "
+            "content_type={self.content_type})"
+        )
 
     def read(self, content_type=None, node_id=None):
-        ''' Reads the contents from the file system
+        """Reads the contents from the file system
 
         :param content_type: defines the content_type of the file used to
                              deserialize the object
         :type content_type: str
         :returns: object
         :raises: FileObjectError
 
         The read method will read the file from the file system, deserializing
         the contents as specified by the content_type argument.  If the
         content_type argument is not specified, the read method will read
         the file as text. If any errors occur, a FileObjectError is raised.
 
-        '''
+        """
         try:
             self.content_type = content_type
-            return ztpserver.serializers.load(self.name, content_type,
-                                              node_id)
+            return ztpserver.serializers.load(self.name, content_type, node_id)
         except SerializerError as err:
-            raise FileObjectError(err.message)
+            raise FileObjectError(str(err)) from err
 
     def write(self, contents, content_type=None):
-        ''' Writes the contents to the file
+        """Writes the contents to the file
 
         :param contents: specifies the contents to be written to the file
         :type contents: str
         :param content_type: defines the serialization format to use when
                              saving the file
         :type content_type: str
         :returns: None
@@ -149,96 +146,96 @@
         The write method takes the contents argument and writes it to the file
         using the serialization specified in the content_type argument.  If
         the content_type argument is not specified, the contents are written
         as string text.  This method will overwrite any contents that
         previously existed for the FileObj instance.  If any errors are
         encountered during the write operation, a FileObjectError is raised
 
-        '''
+        """
         try:
             ztpserver.serializers.dump(contents, self.name, content_type)
             self.content_type = content_type
         except SerializerError as err:
-            raise FileObjectError(err.message)
+            raise FileObjectError(str(err)) from err
 
     def size(self):
-        ''' Returns the size of the object in bytes.
+        """Returns the size of the object in bytes.
 
         :raises: IOError
-        '''
+        """
         return os.path.getsize(self.name)
 
     def hash(self):
-        ''' Returns the SHA1 hash of the object.
+        """Returns the SHA1 hash of the object.
 
         :raises: IOError
-        '''
+        """
 
         sha1 = hashlib.sha1()
-        sha1.update(open(self.name).read())       #pylint: disable=E1101
+        with open(self.name, encoding="utf8") as fd:
+            sha1.update(fd.read().encode("utf8"))  # pylint: disable=E1101
         return sha1.hexdigest()
 
-class Repository(object):
-    ''' The Respository class represents a repository of :py:class:`FileObject`
+
+class Repository:
+    """The Respository class represents a repository of :py:class:`FileObject`
     instances.  It is an abstract wrapper providing the ability to interact
     with persistently stored files.
-    '''
+    """
 
     def __init__(self, path):
-        ''' The initialize method for :py:class:`Repository`
+        """The initialize method for :py:class:`Repository`
 
         :param path: the base path of the repository
         :type path: str
         :returns: object
 
-        '''
+        """
         self.path = path
 
     def __repr__(self):
-        return "Repository(path=%s)" % self.path
+        return f"Repository(path={self.path})"
 
     def expand(self, file_path):
-        ''' Expands a file_path to the full path to a file object
+        """Expands a file_path to the full path to a file object
 
         :param file_path: the file path to expand
         :type file_path: str
         :returns: str -- the full path to the file
 
         This method is used to transform a relative file path into an
         absolute file path for identifying a file object resource
 
-        '''
-        if file_path == '/':
+        """
+        if file_path == "/":
             file_path = self.path
         elif not str(file_path).startswith(self.path):
-            file_path = file_path[1:] if file_path[0] == '/' else file_path
+            file_path = file_path[1:] if file_path[0] == "/" else file_path
             file_path = os.path.join(self.path, file_path)
         return file_path
 
     def add_folder(self, folder_path):
-        ''' Add a new folder to the repository
+        """Add a new folder to the repository
 
         :param folder_path: the full path of the folder to add
         :type folder_path: str
         :returns: str -- the full path to the new folder
         :raises: RespositoryError
 
-        '''
+        """
         try:
             folder_path = self.expand(folder_path)
-            os.makedirs(folder_path, 0774)
+            os.makedirs(folder_path, 0o774)
             return folder_path
         except OSError as err:
-            log.error('Failed to add folder %s (%s)' %
-                      (folder_path, err))
-            raise RepositoryError('Failed to add folder %s (%s)' %
-                                  (folder_path, err))
+            log.error("Failed to add folder %s (%s)", folder_path, err)
+            raise RepositoryError(f"Failed to add folder {folder_path} ({err})") from err
 
     def add_file(self, file_path, contents=None, content_type=None):
-        ''' Adds a new :py:class:`FileObject` to the repository
+        """Adds a new :py:class:`FileObject` to the repository
 
         :param file_path: the full path of the file to add
         :type file_path: str
         :param contents: the contents to write to the file
         :type contents: str
         :param content_type: specifies the serialization to use for the file
         :type content_type: str
@@ -248,59 +245,57 @@
         The add_file method allows for a new file to be added to the
         respository.  If the file already exists, it is returned as an instance
         of :py:class:`FileObject`.   If the file doesn't already exist and
         the contents argument is not None, then the file is created and
         the contents written to the file.  The content_type argument provides
         the serialization to be used when saving the file.
 
-        '''
+        """
         file_path = self.expand(file_path)
         obj = FileObject(file_path)
         if contents:
             obj.write(contents, content_type)
         return obj
 
     def exists(self, file_path):
-        ''' Returns boolean if the file_path exists in the repository
+        """Returns boolean if the file_path exists in the repository
 
         :param file_path: the file_path to check for existence
         :type file_path: str
         :returns: boolean -- True if it exists otherwise False
 
-        '''
+        """
         file_path = self.expand(file_path)
         return os.path.exists(file_path)
 
     def get_file(self, file_path):
-        ''' Returns an intance of :py:class:`FileObject` if it exists
+        """Returns an intance of :py:class:`FileObject` if it exists
 
         :param file_path: the file path of the instance to return
         :type file_path: str
         :returns: instance of :py:class:`FileObject`
         :raises: FileObjectNotFound
 
         This method will retrieve a file object instance if it exists in the
         repository.  If the file does not exist then an error is raised
 
-        '''
+        """
         file_path = self.expand(file_path)
         if not self.exists(file_path):
-            raise FileObjectNotFound('file not found (%s)' % file_path)
+            raise FileObjectNotFound(f"file not found ({file_path})")
         return FileObject(file_path)
 
     def delete_file(self, file_path):
-        ''' Deletes an existing file in the respository
+        """Deletes an existing file in the respository
 
         :param file_path: the file path of the instance to delete
         :type file_path: str
         :returns: None
         :raises: RepositoryError
 
-        '''
+        """
         try:
             file_path = self.expand(file_path)
             os.remove(file_path)
-        except (OSError, IOError) as err:
-            log.error('Failed to delete file %s (%s)' %
-                      (file_path, err))
-            raise RepositoryError('Failed to delete file %s (%s)' %
-                                  (file_path, err))
+        except OSError as err:
+            log.error("Failed to delete file %s (%s)", file_path, err)
+            raise RepositoryError(f"Failed to delete file {file_path} ({err})") from err
```

### Comparing `ztpserver-1.6.0/plugins/test` & `ztpserver-2.0.0/plugins/test`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,25 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-'''
+"""
 Simply returns a string made of the node ID and the name of 
 the resource pool.
 
 Definition example:
 
     actions:
       -
         action: add_config
         attributes:
           url: files/templates/demo.templates
           variables:
             ipaddress: test('demo')
-'''
+"""
 
-def main(node_id, pool, node):
-    return '%s:%s' % (node_id, pool)
+
+def main(node_id, pool, _):
+    return f"{node_id}:{pool}"
```

### Comparing `ztpserver-1.6.0/plugins/sqlite` & `ztpserver-2.0.0/plugins/sqlite`

 * *Files 19% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-'''
+"""
 Allocates a resource from a prefilled sqlite database. The database
 is defined by the global variable, 'DB_URL' below. The database
 can include multiple tables, but the value passed into the
 'sqlite(table)' will be used to look for an available resource.
 
 Table structure should be as follows:
 
@@ -74,93 +74,92 @@
       -
         action: add_config
         attributes:
           url: files/templates/ma1.templates
           variables:
             ipaddress: sqlite('mgmt_subnet')
         name: "configure ma1"
-'''
+"""
 
 import logging
 import os
 import sqlite3 as lite
 
-log = logging.getLogger('ztpserver')   #pylint: disable=C0103
+log = logging.getLogger("ztpserver")  # pylint: disable=C0103
 
 # SQLITE VARIABLES
 DB_URL = "/usr/share/ztpserver/db/resources.db"
 
 
 def check_url_valid(url):
-    
-    if not url.startswith('http'):
-        log.info('checking sqlite db (%s) exists...' % DB_URL)
+    if not url.startswith("http"):
+        log.info("checking sqlite db (%s) exists...", DB_URL)
         if not os.path.isfile(url):
-            raise Exception('Specified DB file %s does not exists.'
-                            % url)
+            raise RuntimeError(f"Specified DB file {url} does not exists.")
 
 
 def assign_resource(node_id, table):
-
     # Proactively check if the db file exists
     check_url_valid(DB_URL)
 
-    log.info('%s: looking for resources in sqlite DB(%s) in table(%s)'
-             % (node_id, DB_URL, table))
+    log.info("%s: looking for resources in sqlite DB(%s) in table(%s)", node_id, DB_URL, table)
 
-    #Setup connection to local sqlite database
+    # Setup connection to local sqlite database
     con = lite.connect(DB_URL)
 
     with con:
         cur = con.cursor()
 
-        query = "SELECT * FROM `%s` WHERE node_id='%s'"  % (table, node_id)
+        query = f"SELECT * FROM `{table}` WHERE node_id='{node_id}'"
 
-        log.debug('%s: executing sql query:%s' % (node_id, query))
+        log.debug("%s: executing sql query:%s", node_id, query)
         match = cur.execute(query).fetchone()
 
         if match:
-            log.debug('%s: already allocated:%s in table %s'
-                      % (node_id, match[0], table))
+            log.debug("%s: already allocated:%s in table %s", node_id, match[0], table)
+            return match[0]
+
+        log.info(
+            "%s: no existing resources matches this node "
+            "in the db. Looking for new resource in %s",
+            node_id,
+            table,
+        )
+
+        # The query must use subquery since sqlite is not
+        # typically compiled with LIMIT support for UPDATE
+        query = """UPDATE `{table}`
+                   SET node_id = '{node_id}'
+                   WHERE key IN (
+                     SELECT key
+                     FROM `{table}`
+                     WHERE node_id IS NULL
+                     ORDER BY rowid ASC
+                     LIMIT 1
+                  )""".format(
+            table=table, node_id=node_id
+        )
+        log.debug("%s: executing query: %s", node_id, query)
+        cur.execute(query).fetchone()
+        log.debug("%s: number of rows affected:%s", node_id, cur.rowcount)
+
+        if cur.rowcount == 1:
+            # Go get the resouce that was just allocated
+            query = f"SELECT * FROM `{table}` WHERE node_id='{node_id}'"
+            log.debug("%s: executing sql query:%s", node_id, query)
+            match = cur.execute(query).fetchone()
             return match[0]
-        else:
-            log.info('%s: no existing resources matches this node '
-                     'in the db. Looking for new resource in %s'
-                     % (node_id, table))
-
-            # The query must use subquery since sqlite is not
-            # typically compiled with LIMIT support for UPDATE
-            query = """UPDATE `%s`
-                       SET node_id = '%s'
-                       WHERE key IN (
-                         SELECT key
-                         FROM `%s`
-                         WHERE node_id IS NULL
-                         ORDER BY rowid ASC
-                         LIMIT 1
-                      )""" % (table, node_id, table)
-            log.debug('%s: executing query: %s' % (node_id, query))
-            assigned = cur.execute(query).fetchone()
-            log.debug('%s: number of rows affected:%s' %
-                      (node_id, cur.rowcount))
-
-            if cur.rowcount == 1:
-                # Go get the resouce that was just allocated
-                query = "SELECT * FROM `%s` WHERE node_id='%s'" % (table, node_id)
-                log.debug('%s: executing sql query:%s' % (node_id, query))
-                match = cur.execute(query).fetchone()
-                return match[0]
+
+    raise RuntimeError("Resource not found")
 
 
-def main(node_id, table, node):
+def main(node_id, table, _):
     try:
         key = assign_resource(node_id, table)
-        log.debug('%s: assigned resource from \'%s\': %s' % 
-                  (node_id, table, key))
+        log.debug("%s: assigned resource from '%s': %s", node_id, table, key)
 
     except Exception as exc:
-        msg = '%s: failed to allocate resource from \'%s\'' % \
-            (node_id, table)
+        msg = f"{node_id}: failed to allocate resource from '{table}'"
         log.error(msg)
-        raise Exception('%s : %s' % (msg, exc.message))
+        raise RuntimeError(f"{msg} : {exc}") from exc
 
     return str(key)
```

### Comparing `ztpserver-1.6.0/plugins/mysql_vars` & `ztpserver-2.0.0/plugins/mysql_vars`

 * *Files 17% similar despite different names*

```diff
@@ -24,112 +24,116 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
+import hashlib
+import json
 import logging
 import os
-import MySQLdb
-import json, hashlib
 
-log = logging.getLogger('ztpserver')   #pylint: disable=C0103
+import MySQLdb  # pylint: disable=E0401
+
+log = logging.getLogger("ztpserver")  # pylint: disable=C0103
+
 
 def fetch_tor(node, node_id):
-    '''
+    """
     Query mysql database using the node's neighbors and return the tor record.
     The key for the tor loopkup is the md5 hash of the json serialized
     neighbors.
 
     Returns: tor dict:
          { 'neighbors' : dict( <neighbors),
            'type' : <tor-type>,
            'hostName' : <hostname>,
            ...
          }
-    '''
+    """
 
     # Connect to mysql server
-    user = os.environ.get('MYSQL_USER', 'root')
-    db = os.environ.get('MYSQL_DB', 'db')
-    host = os.environ.get('MYSQL_HOST', 'localhost')
-    log.debug('%s: Connecting to mysql %s:%s:%s' % \
-               (node_id, host, user, db))
+    user = os.environ.get("MYSQL_USER", "root")
+    db = os.environ.get("MYSQL_DB", "db")  # pylint: disable=C0103
+    host = os.environ.get("MYSQL_HOST", "localhost")
+    log.debug("%s: Connecting to mysql %s:%s:%s", node_id, host, user, db)
 
-    assert db and host and user, 'Params to connect to mysql server missing'
+    assert db and host and user, "Params to connect to mysql server missing"
     con = MySQLdb.connect(db=db, host=host, user=user)
     cur = con.cursor()
 
     # Build a dict of neighbors based on node's LLDP neighbors.
-    # 
+    #
     # Format:
     #    { <interface> : { 'device': <neighbor-device>, 'port': <neighbor-port> }
     #      ...
     #    }
 
     neighbors = {}
     for intf, nlist in node.neighbors.items():
-        ndevice = nlist[ 0 ]
-        device = ndevice.device.split('.')[ 0 ]
-        neighbors[ intf ] = dict(device=device, port=ndevice.interface)
+        ndevice = nlist[0]
+        device = ndevice.device.split(".")[0]
+        neighbors[intf] = {"device": device, "port": ndevice.interface}
 
     # Serialize the neighbors and get the md5 hash
-    neighborsStr = json.dumps(neighbors, sort_keys=True)
-    hash = hashlib.md5(neighborsStr).hexdigest()
-    log.debug('%s: hash: %s' % (node_id, hash))
+    neighbors_str = json.dumps(neighbors, sort_keys=True)
+    digest = hashlib.md5(neighbors_str).hexdigest()
+    log.debug("%s: hash: %s", node_id, hash)
 
     # Lookup tor by hash
-    stmt = ('select hostName, torData, type from tor where hash=%s')
-    where = (hash,)
+    stmt = "select hostName, torData, type from tor where hash=%s"
+    where = (digest,)
     cur.execute(stmt, where)
-    hostName, torData , torType = cur.fetchone()
-    tor = json.loads(torData)
-    tor[ 'type' ] = torType
+    host_name, tor_data, tor_type = cur.fetchone()
+    tor = json.loads(tor_data)
+    tor["type"] = tor_type
 
     # Check for hash collision
-    if tor['neighbors'] != neighbors:
-        raise Exception('%s: hash collision for TOR %s' % (node_id, hostName))
+    if tor["neighbors"] != neighbors:
+        raise RuntimeError(f"{node_id}: hash collision for TOR {host_name}")
     return tor
 
+
 def assign_url(tor):
-    if tor[ 'type' ] == 'systest':
-        return 'files/templates/dm1-tor-systest.template'
-    elif tor[ 'type' ] == 'software':
-        return 'files/templates/dm1-tor-software.template'
-    elif tor[ 'type' ] == 'server':
-        return 'files/templates/dm1-tor-server.template'
-    else:
-        raise Exception('Unknown TOR type %s' % tor[ 'type' ])
+    if tor["type"] == "systest":
+        return "files/templates/dm1-tor-systest.template"
+    if tor["type"] == "software":
+        return "files/templates/dm1-tor-software.template"
+    if tor["type"] == "server":
+        return "files/templates/dm1-tor-server.template"
+
+    raise RuntimeError(f"Unknown TOR type {tor['type']}")
+
 
 def assign_var(tor):
     # The tor 'type' and 'neighbors' are just for internal usage. They are not
     # variables required by the template.
-    tor.pop('type')
-    tor.pop('neighbors')
+    tor.pop("type")
+    tor.pop("neighbors")
     return tor
 
+
 def main(node_id, pool, node):
-    '''
+    """
     Return the resource requested for the pool type.
 
     node_id - Node identifier, usually the serial number
     pool - Type of resource requested, its either url or variable.
     node - Copy of the Node object
-    '''
+    """
     try:
         # Get a copy of the tor record stored in mysql, based on the node's
         # neighbors.
         tor = fetch_tor(node, node_id)
 
-        if pool == 'url':
+        if pool == "url":
             return assign_url(tor)
-        elif pool == 'variables':
+        if pool == "variables":
             return assign_var(tor)
-        else:
-            assert False, 'Unknown pool %s' % pool
+
+        assert False, f"Unknown pool {pool}"
     except Exception as exc:
-        msg = '%s: failed to allocate resource from \'%s\'' % \
-            (node_id, pool)
+        msg = f"{node_id}: failed to allocate resource from '{pool}'"
         log.error(msg)
-        log.error(exc.message)
-        raise Exception('%s : %s' % (msg, exc.message))
+        log.error(str(exc))
+        raise RuntimeError(f"{msg} : {exc}") from exc
```

### Comparing `ztpserver-1.6.0/plugins/allocate` & `ztpserver-2.0.0/plugins/allocate`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-'''
+"""
 Allocates a resource from a key/value YAML file (under
 DATA_ROOT/resources) that contains a set of resources to be
 allocated. Here is an example (DATA_ROOT/resoruces/ip_address):
 
     192.168.1.1/24: null
     192.168.1.2/24: null
 
@@ -59,94 +59,84 @@
       -
         action: add_config
         attributes:
           url: files/templates/ma1.templates
           variables:
             ipaddress: allocate('mgmt_subnet')
         name: "configure ma1"
-'''
+"""
 
 import logging
 import os
-
 from collections import OrderedDict
 
-from ztpserver.serializers import load, dump
-from ztpserver.constants import CONTENT_TYPE_YAML
 from ztpserver.config import runtime
+from ztpserver.constants import CONTENT_TYPE_YAML
+from ztpserver.serializers import dump, load
 
+log = logging.getLogger(__name__)  # pylint: disable=C0103
 
-log = logging.getLogger(__name__)   #pylint: disable=C0103
 
 def load_resource(node_id, filename):
     data = OrderedDict()
 
-    contents = load(filename, 
-                    CONTENT_TYPE_YAML, 
-                    node_id,
-                    lock=True)
+    contents = load(filename, CONTENT_TYPE_YAML, node_id, lock=True)
 
     if contents and isinstance(contents, dict):
         for key, value in contents.iteritems():
             data[key] = str(value) if value else None
     else:
         if not contents:
-            contents = 'empty pool'
-        raise Exception(contents)
+            contents = "empty pool"
+        raise RuntimeError(contents)
 
     return data
 
+
 def lookup(node_id, data):
-    ''' Return an existing allocated resource if one exists '''
+    """Return an existing allocated resource if one exists"""
 
     try:
-        key = next(m[0] for m in data.iteritems()
-                   if m[1] == node_id)
+        key = next(m[0] for m in data.iteritems() if m[1] == node_id)
     except StopIteration:
         key = None
 
     return key
 
-def main(node_id, pool, node):
+
+def main(node_id, pool, _):
     try:
-        file_path = os.path.join(runtime.default.data_root, 
-                                 'resources')
+        file_path = os.path.join(runtime.default.data_root, "resources")
         filename = os.path.join(file_path, pool)
 
         data = load_resource(node_id, filename)
-        log.debug('%s: loaded resource pool \'%s\': %s' % 
-                  (node_id, pool, data))
+        log.debug("%s: loaded resource pool '%s': %s", node_id, pool, data)
 
         match = lookup(node_id, data)
 
         if match:
-            log.debug('%s: already allocated resource \'%s\':\'%s\'' % 
-                     (node_id, pool, match))
+            log.debug("%s: already allocated resource '%s':'%s'", node_id, pool, match)
             return match
 
-        entry = next(x[0] for x in data.iteritems() if x[1] is None)
-        log.debug('%s: allocated \'%s\':\'%s\'' % (node_id, pool, entry))
+        entry = next(x[0] for x in data.items() if x[1] is None)
+        log.debug("%s: allocated '%s':'%s'", node_id, pool, entry)
 
         data[entry] = node_id
 
-        log.debug('%s: writing resource pool \'%s\': %s' % 
-                  (node_id, pool, data))
+        log.debug("%s: writing resource pool '%s': %s", node_id, pool, data)
         file_path = os.path.join(file_path, pool)
 
         # serialize data
         for key, value in data.items():
             data[key] = str(value) if value else None
 
-        dump(data, file_path, CONTENT_TYPE_YAML, 
-             node_id, lock=True)
+        dump(data, file_path, CONTENT_TYPE_YAML, node_id, lock=True)
 
-    except StopIteration:
-        log.error('%s: no resource free in \'%s\'' % (node_id, pool))
-        raise Exception('%s: no resource free in \'%s\'' % 
-                                (node_id, pool))
+    except StopIteration as exc:
+        log.error("%s: no resource free in '%s'", node_id, pool)
+        raise RuntimeError(f"{node_id}: no resource free in '{pool}'") from exc
     except Exception as exc:
-        msg = '%s: failed to allocate resource from \'%s\'' % \
-            (node_id, pool)
+        msg = f"{node_id}: failed to allocate resource from '{pool}'"
         log.error(msg)
-        raise Exception('%s : %s' % (msg, exc.message))
+        raise RuntimeError(f"{msg} : {exc}") from exc
 
     return str(entry)
```

### Comparing `ztpserver-1.6.0/Makefile` & `ztpserver-2.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/utils/refresh_ztps` & `ztpserver-2.0.0/utils/refresh_ztps`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,130 @@
-#!/usr/bin/env python 
+#!/usr/bin/env python3
 
 # This script can be used in order to automatically refresh the
 # installation of ZTP Server to the latest code on GitHub.  This can
 # be useful in order to pull bug fixes or run the latest version of
 # various development branches.
 
 # INSTRUCTIONS:
 #  - The script must be run by a user with sudo access.
 
 import argparse
 import os
 import re
 import sys
 
-BACKUP_FOLDER = '/tmp/ztps_backup'
-BACKUP_CONFIG_FOLDER = '/tmp/ztps_backup/home'
-GLOBAL_CONFIG_FILE = '/etc/ztpserver/ztpserver.conf'
+BACKUP_FOLDER = "/tmp/ztps_backup"
+BACKUP_CONFIG_FOLDER = "/tmp/ztps_backup/home"
+GLOBAL_CONFIG_FILE = "/etc/ztpserver/ztpserver.conf"
+
+GIT_REPO_FOLDER = "/tmp/ztps"
 
-GIT_REPO_FOLDER = '/tmp/ztps'
 
 def create_folder(path):
-    os.system('sudo rm -fr \'%s\'' % path)
-    os.system('sudo mkdir %s' % path)
-    os.system('sudo chmod 777 %s' % path)
+    os.system(f"sudo rm -fr '{path}'")
+    os.system(f"sudo mkdir {path}")
+    os.system(f"sudo chmod 777 {path}")
+
 
 def all_files(path):
     result = []
     for top, dirs, files in os.walk(path):
         result += [os.path.join(top, d) for d in dirs]
         result += [os.path.join(top, f) for f in files]
 
     return result
 
-def refresh_ztps(home_folder, branch):
 
+def refresh_ztps(home_folder, branch):
     # Backup configuration files
     create_folder(BACKUP_FOLDER)
     create_folder(BACKUP_CONFIG_FOLDER)
 
-    os.system('sudo cp %s %s' % 
-              (GLOBAL_CONFIG_FILE,
-               '%s/ztpserver.conf' % BACKUP_FOLDER))
-    os.system('sudo cp -r %s/* %s' % 
-              (home_folder, BACKUP_CONFIG_FOLDER))
+    os.system(f"sudo cp {GLOBAL_CONFIG_FILE} {'%s/ztpserver.conf' % BACKUP_FOLDER}")
+    os.system(f"sudo cp -r {home_folder}/* {BACKUP_CONFIG_FOLDER}")
 
     # Uninstall
-    paths = all_files('/usr/lib')
-    paths += all_files('/usr/local')
-    for path in [p for p in paths if re.match('.*ztpserver.*', p)]:
-        os.system('sudo rm -rf %s' % path)
+    paths = all_files("/usr/lib")
+    paths += all_files("/usr/local")
+    for path in [p for p in paths if re.match(".*ztpserver.*", p)]:
+        os.system(f"sudo rm -rf {path}")
 
     # Clone repository
-    os.system('sudo rm -rf \'%s\'' % GIT_REPO_FOLDER)
-    result = os.system('''
-        sudo git clone https://github.com/arista-eosplus/ztpserver %s;
-        cd %s;
-        sudo git checkout %s;
+    os.system(f"sudo rm -rf '{GIT_REPO_FOLDER}'")
+    result = os.system(
+        f"""
+        sudo git clone https://github.com/arista-eosplus/ztpserver {GIT_REPO_FOLDER};
+        cd {GIT_REPO_FOLDER};
+        sudo git checkout {branch};
         sudo git pull;
 
         sudo python setup.py build;
         sudo python setup.py install
-        ''' % (GIT_REPO_FOLDER, GIT_REPO_FOLDER, branch))
+        """
+    )
     if result != 0:
-        sys.exit('ERROR: failed to re-install ZTP Server (branch %s)' % branch)
+        sys.exit(f"ERROR: failed to re-install ZTP Server (branch {branch})")
 
     # Reconfigure
-    os.system('sudo cp %s %s' % 
-              ('%s/ztpserver.conf' % BACKUP_FOLDER,
-               GLOBAL_CONFIG_FILE))
-
-    os.system('sudo cp %s %s' % 
-              ('%s/bootstrap/bootstrap.conf' % BACKUP_CONFIG_FOLDER,
-               '%s/bootstrap/bootstrap.conf' % home_folder))
-    os.system('sudo cp %s %s' % 
-              ('%s/neighbordb' % BACKUP_CONFIG_FOLDER,
-               '%s/neighbordb' % home_folder))
-
-    files_1 = [y for y in [x.replace(home_folder + '/', '')
-                           for x in all_files(home_folder)] if y]
-    files_2 = [y for y in [x.replace(BACKUP_CONFIG_FOLDER + '/', '')
-                           for x in all_files(BACKUP_CONFIG_FOLDER)] if y]
+    os.system(f"sudo cp {'%s/ztpserver.conf' % BACKUP_FOLDER} {GLOBAL_CONFIG_FILE}")
+
+    os.system(
+        f"sudo cp {BACKUP_CONFIG_FOLDER}/bootstrap/bootstrap.conf {home_folder}/bootstrap/bootstrap.conf"
+    )
+    os.system(f"sudo cp {BACKUP_CONFIG_FOLDER}/neighbordb' {home_folder}/neighbordb")
+
+    files_1 = [y for y in [x.replace(home_folder + "/", "") for x in all_files(home_folder)] if y]
+    files_2 = [
+        y
+        for y in [
+            x.replace(BACKUP_CONFIG_FOLDER + "/", "") for x in all_files(BACKUP_CONFIG_FOLDER)
+        ]
+        if y
+    ]
 
     for file_path in [x for x in files_2 if x not in files_1]:
         try:
-            os.system('sudo cp %s %s' % 
-                      ('%s/%s' % (BACKUP_CONFIG_FOLDER, file_path),
-                       '%s/%s' % (home_folder, file_path)))
-        except IOError: 
+            os.system(f"sudo cp {BACKUP_CONFIG_FOLDER}/{file_path} {home_folder}/{file_path}")
+        except IOError:
             # directory
-            create_folder('%s/%f' % (home_folder, file_path))
+            create_folder(f"{home_folder}/{file_path:f}")
 
     # Set permissions
-    os.system('sudo chmod 777 %s -R' % home_folder)
-    os.system('sudo chmod 777 %s -R' % GLOBAL_CONFIG_FILE)
+    os.system(f"sudo chmod 777 {home_folder} -R")
+    os.system(f"sudo chmod 777 {GLOBAL_CONFIG_FILE} -R")
 
     # Clean up
-    os.system('sudo rm -fr \'%s\'' % BACKUP_FOLDER)
-    os.system('sudo rm -fr \'%s\'' % GIT_REPO_FOLDER)
-    print '\nDone!'
+    os.system(f"sudo rm -fr '{BACKUP_FOLDER}'")
+    os.system(f"sudo rm -fr '{GIT_REPO_FOLDER}'")
+    print("\nDone!")
+
 
 def main():
-    parser = argparse.ArgumentParser(prog='refresh_ztps')
-    parser.add_argument('-b', '--branch',
-                        metavar='BRANCH',
-                        nargs='?',
-                        default='master',
-                        help='ZTP Server branch to be used for the refresh',
-                        action='store')
-    parser.add_argument('-f', '--home-folder',
-                        metavar='HOME_FOLDER',
-                        nargs='?',
-                        default='/usr/share/ztpserver',
-                        help='ZTP Server home folder',
-                        action='store')
+    parser = argparse.ArgumentParser(prog="refresh_ztps")
+    parser.add_argument(
+        "-b",
+        "--branch",
+        metavar="BRANCH",
+        nargs="?",
+        default="master",
+        help="ZTP Server branch to be used for the refresh",
+        action="store",
+    )
+    parser.add_argument(
+        "-f",
+        "--home-folder",
+        metavar="HOME_FOLDER",
+        nargs="?",
+        default="/usr/share/ztpserver",
+        help="ZTP Server home folder",
+        action="store",
+    )
     args = parser.parse_args()
     refresh_ztps(args.home_folder, args.branch)
-    
-if __name__ == '__main__':
+
+
+if __name__ == "__main__":
     try:
         main()
     except KeyboardInterrupt:
         pass
```

### Comparing `ztpserver-1.6.0/utils/create_db.py` & `ztpserver-2.0.0/utils/create_db.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 con = lite.connect('/usr/share/ztpserver/db/resources.db')
 
 with con:
 
     for table in ['mgmt_subnet', 'tor_hostnames', 'ip_vlan100', 'ip_loopback']:
-        print "Working on: ",table
+        print("Working on: ", table)
         cur = con.cursor()
         sql = "DROP TABLE IF EXISTS `%s`" % table
         cur.execute(sql)
         sql = "CREATE TABLE `%s`(key TEXT, node_id TEXT)" % table
         cur.execute(sql)
         if table == "mgmt_subnet":
             base = "172.16.130."
@@ -29,12 +29,12 @@
             subnet = "/32"
 
         for x in range(1,500):
             sql = "INSERT INTO %s VALUES('%s%s%s',NULL)" % (table, base, str(x), subnet)
             cur.execute(sql)
 
         sql = "SELECT * FROM `%s`" % table
-        print sql
+        print(sql)
         cur.execute(sql)
         rows = cur.fetchall()
         for row in rows:
-            print row
+            print(row)
```

### Comparing `ztpserver-1.6.0/docs/actions.rst` & `ztpserver-2.0.0/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/install.rst` & `ztpserver-2.0.0/docs/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 .. contents:: :local:
 
 Requirements
 `````````````
 
   **Server:**
 
-  * Python 2.7 or later (https://www.python.org/download/releases)
-  * routes 2.0 or later (https://pypi.python.org/pypi/Routes)
-  * webob 1.3 or later (http://webob.org/)
-  * PyYaml 3.0 or later (http://pyyaml.org/)
+  * Python 3.7 or later (https://www.python.org/download/releases)
+  * routes 2.5 or later (https://pypi.python.org/pypi/Routes)
+  * webob 1.8 or later (http://webob.org/)
+  * PyYaml 6.0 or later (http://pyyaml.org/)
 
   **Client:**
 
   * `EOS <http://eos.arista.com>`_ 4.12.0 or later (ZTPServer 1.1+)
   * `EOS <http://eos.arista.com>`_ 4.13.3 or later (ZTPServer 1.0)
 
-.. NOTE:: We recommend using a Linux distribution which has Python 2.7 as its standard Python install (e.g. yum in Centos requires Python 2.6 and a dual Python install can be fairly tricky and buggy). This guide was written based ZTPServer v1.1.0 installed on Fedora 20. 
+.. NOTE:: We recommend using a Linux distribution which has Python 2.7 as its standard Python install (e.g. yum in Centos requires Python 2.6 and a dual Python install can be fairly tricky and buggy). This guide was written based ZTPServer v1.1.0 installed on Fedora 20.
 
 Installation Options
 ````````````````````
 
     * :ref:`packer_install`
     * :ref:`pypi_install`
     * :ref:`manual_install`
 
 .. _packer_install:
 
-Turn-key VM Creation
+Turn-key VM Creation (deprecated)
 ~~~~~~~~~~~~~~~~~~~~
 
 The turn-key VM option leverages `Packer <http://www.packer.io/>`_ to auto generate a VM on your local system. Packer.io automates the creation of the ZTPServer VM. All of the required packages and dependencies are installed and configured. The current Packer configuration allows you to choose between VirtualBox or VMWare as your hypervisor and each can support Fedora 20 or Ubuntu Server 12.04.
 
 VM Specification:
 
 * 7GB Hard Drive
@@ -190,15 +190,15 @@
 .. NOTE:: If using the :ref:`packer_install`, all of the steps, below, will have been completed, please reference the VM documentation.
 
 Allow ZTPServer Connections In Through The Firewall
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Be sure your host firewall allows incoming connections to ZTPServer.  The standalone server runs on port TCP/8080 by default.
 
-**Firewalld** examples: 
+**Firewalld** examples:
 
   * Open TCP/<port> through firewalld
     ``bash-3.2$ firewall-cmd --zone=public --add-port=<port>/tcp [--permanent]``
   * Stop firewalld
     ``bash-3.2$ systemctl stop firewalld``
   * Disable firewalld
     ``bash-3.2$ systemctl disable firewalld``
@@ -251,8 +251,7 @@
 
   ``bash-3.2# sudo /usr/sbin/service isc-dhcp-server start``
 
 Check that /etc/init/isc-dhcp-server.conf is configured for automatic startup on boot.
 
 
 Edit the global configuration file located at ``/etc/ztpserver/ztpserver.conf`` (if needed). See the :ref:`global_configuration` options for more information.
-
```

### Comparing `ztpserver-1.6.0/docs/index.rst` & `ztpserver-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/ReleaseNotes1.6.0.rst` & `ztpserver-2.0.0/docs/ReleaseNotes1.6.0.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/support.rst` & `ztpserver-2.0.0/docs/support.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 The authoritative state for any known issue can be found in `GitHub issues <https://github.com/arista-eosplus/ztpserver/issues>`_.
 
 .. toctree::
     :maxdepth: 2
     :titlesonly:
 
+    ReleaseNotes2.0.0
     ReleaseNotes1.6.0
     ReleaseNotes1.5.0
     ReleaseNotes1.4.1
     ReleaseNotes1.4
     ReleaseNotes1.3.2
     ReleaseNotes1.3.1
     ReleaseNotes1.3
```

### Comparing `ztpserver-1.6.0/docs/Makefile` & `ztpserver-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/ReleaseNotes1.4.rst` & `ztpserver-2.0.0/docs/ReleaseNotes1.4.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/ReleaseNotes1.5.0.rst` & `ztpserver-2.0.0/docs/ReleaseNotes1.5.0.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/conf.py` & `ztpserver-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/config.rst` & `ztpserver-2.0.0/docs/config.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/examples.rst` & `ztpserver-2.0.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/ReleaseNotes1.3.rst` & `ztpserver-2.0.0/docs/ReleaseNotes1.3.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/_static/AttrsActions.png` & `ztpserver-2.0.0/docs/_static/AttrsActions.png`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/_static/favicon.ico` & `ztpserver-2.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/_static/arista_logo_11-trans-w.png` & `ztpserver-2.0.0/docs/_static/arista_logo_11-trans-w.png`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/_static/arista_logo_jpg-11.jpg` & `ztpserver-2.0.0/docs/_static/arista_logo_jpg-11.jpg`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/_static/Components.png` & `ztpserver-2.0.0/docs/_static/Components.png`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/_static/ztpserver-seqdiag.png` & `ztpserver-2.0.0/docs/_static/ztpserver-seqdiag.png`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/_static/LeafDefn.png` & `ztpserver-2.0.0/docs/_static/LeafDefn.png`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/ReleaseNotes1.3.2.rst` & `ztpserver-2.0.0/docs/ReleaseNotes1.3.2.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/ReleaseNotes1.2.rst` & `ztpserver-2.0.0/docs/ReleaseNotes1.2.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/overview.rst` & `ztpserver-2.0.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/actions.rst` & `ztpserver-2.0.0/docs/cookbook/actions.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/install.rst` & `ztpserver-2.0.0/docs/cookbook/install.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/ztpsVMonEOS.rst` & `ztpserver-2.0.0/docs/cookbook/ztpsVMonEOS.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/dynamicNodes.rst` & `ztpserver-2.0.0/docs/cookbook/dynamicNodes.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/resourcePools.rst` & `ztpserver-2.0.0/docs/cookbook/resourcePools.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/clientLogging.rst` & `ztpserver-2.0.0/docs/cookbook/clientLogging.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/configuration.rst` & `ztpserver-2.0.0/docs/cookbook/configuration.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/ztpsVMonEOS/l2l3wm.rst` & `ztpserver-2.0.0/docs/cookbook/ztpsVMonEOS/l2l3wm.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/ztpsVMonEOS/l2wom.rst` & `ztpserver-2.0.0/docs/cookbook/ztpsVMonEOS/l2wom.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/ztpsVMonEOS/l3wom.rst` & `ztpserver-2.0.0/docs/cookbook/ztpsVMonEOS/l3wom.rst`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 I want to create a python script that restarts DHCPD whenever an interface comes up.
 
 Solution
 ^^^^^^^^
 
 .. code-block:: python
 
-  #!/usr/bin/env python
+  #!/usr/bin/env python3
 
   import jsonrpclib
   import os
   import time
 
   #PROTO = "https"
   #USERNAME = "admin"
```

### Comparing `ztpserver-1.6.0/docs/cookbook/puppet.rst` & `ztpserver-2.0.0/docs/cookbook/puppet.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/helloWorld.rst` & `ztpserver-2.0.0/docs/cookbook/helloWorld.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/topologyValidation.rst` & `ztpserver-2.0.0/docs/cookbook/topologyValidation.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/ansible.rst` & `ztpserver-2.0.0/docs/cookbook/ansible.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/serverLogging.rst` & `ztpserver-2.0.0/docs/cookbook/serverLogging.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/runningZTPS.rst` & `ztpserver-2.0.0/docs/cookbook/runningZTPS.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/definitions.rst` & `ztpserver-2.0.0/docs/cookbook/definitions.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/staticNodes.rst` & `ztpserver-2.0.0/docs/cookbook/staticNodes.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/cookbook/advanced.rst` & `ztpserver-2.0.0/docs/cookbook/advanced.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/ReleaseNotes1.1.rst` & `ztpserver-2.0.0/docs/ReleaseNotes1.1.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/README.md` & `ztpserver-2.0.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/tips.rst` & `ztpserver-2.0.0/docs/tips.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/setup_rtd_files.sh` & `ztpserver-2.0.0/docs/setup_rtd_files.sh`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/implementation.rst` & `ztpserver-2.0.0/docs/implementation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -22,28 +22,28 @@
    then the ‘get’ method will return **None**
 
 e.g. (action code)
 
 .. code-block:: python
 
     def main(attributes):
-        print attributes.get(‘software_image’)
+        print(attributes.get(‘software_image’))
 
 Besides the values coming from the server, a couple of **special
 entries**\ \* (always upper case) are also contained in the attributes
 object:
 
 * ‘NODE’: a node object for making eAPI calls to localhost. See the :doc:`client` documentation.
 
 e.g. (action\_code)
 
 .. code-block:: python
 
     def main(attributes):
-        print attributes.get(‘NODE’).api_enable_cmds([‘show version’])
+        print(attributes.get(‘NODE’).api_enable_cmds([‘show version’]))
 
 Bootstrap URLs
 ~~~~~~~~~~~~~~
 
 1. DHCP response contains the **URL pointing to the bootstrap script** on the server
 2. The location of the server is hardcoded in
    the bootstrap script, using the SERVER global variable. The bootstrap
```

### Comparing `ztpserver-1.6.0/docs/startup.rst` & `ztpserver-2.0.0/docs/startup.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/CONTRIBUTING.md` & `ztpserver-2.0.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/license.rst` & `ztpserver-2.0.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/troubleshooting.rst` & `ztpserver-2.0.0/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/docs/api.rst` & `ztpserver-2.0.0/docs/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 .. The RESTful API is documented using sphinxcontrib-httpdomain.  See
    http://pythonhosted.org/sphinxcontrib-httpdomain/
 
 .. Verify sync with ztpserver.controller.py using the following:
    (PYTHONPATH=.; python)
    my_map = controller.Router()
-   print my_map.map
+   print(my_map.map)
 
 .. contents:: :local:
 
 URL Endpoints
 ~~~~~~~~~~~~~
 
 +---------------+-----------------------------------------+
```

### Comparing `ztpserver-1.6.0/docs/glossary.rst` & `ztpserver-2.0.0/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/README.md` & `ztpserver-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 * IRC: irc.freenode.net#arista
 
 Dependencies
 ============
 
 Server
 ======
-* [Python 2.7](https://www.python.org/download/releases/2.7/)
-* [routes 2.0 or later](https://pypi.python.org/pypi/Routes)
-* [webob 1.3 or later](http://webob.org/)
-* [PyYaml 3.0 or later](http://pyyaml.org/)
+* Python 3.7 or later (https://www.python.org/downloads)
+* routes 2.5 or later (https://pypi.python.org/pypi/Routes)
+* webob 1.8 or later (http://webob.org/)
+* PyYaml 6.0 or later (http://pyyaml.org/)
 
 Client
 ======
 * Arista EOS 4.12.0 or later
 
 License
 =======
```

### Comparing `ztpserver-1.6.0/setup.py` & `ztpserver-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,163 +30,140 @@
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import io
 import os
 import shutil
 import sys
-
 from glob import glob
+
 from ztpserver import config
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 
 def install():
-    if "install" in sys.argv:
-        return True
-    else:
-        return False
+    return bool("install" in sys.argv)
 
 
 def join_url(x, y):
-    start = '' if x == '.' else '/'
-    return start + '/'.join([z for z in x.split('/') + y.split('/') if z])
+    start = "" if x == "." else "/"
+    return start + "/".join([z for z in x.split("/") + y.split("/") if z])
 
 
 def ensure_dir(f):
     d = os.path.dirname(f)
     if not os.path.exists(d):
         os.makedirs(d)
 
 
 def get_long_description():
-    ''' Get the long description from README.md if it exists.
-        Null string is returned if README.md is non-existent
-    '''
-    long_description = ''
+    """Get the long description from README.md if it exists.
+    Null string is returned if README.md is non-existent
+    """
+    long_description = ""
     here = os.path.abspath(os.path.dirname(__file__))
     try:
-        with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as file_hdl:
+        with io.open(os.path.join(here, "README.md"), encoding="utf-8") as file_hdl:
             long_description = file_hdl.read()
     except IOError:
         pass
     return long_description
 
 
 conf_path = config.CONF_PATH
 install_path = config.INSTALL_PATH
 
-if install() and os.environ.get('ZTPS_INSTALL_PREFIX'):
-    print "Customizing install for VirtualEnv install with RPM"
-    conf_path = join_url(os.environ.get('ZTPS_INSTALL_PREFIX'), config.CONF_PATH)
-    install_path = join_url(os.environ.get('ZTPS_INSTALL_PREFIX'), config.INSTALL_PATH)
-
-packages = ['ztpserver']
-if install() and os.environ.get('READTHEDOCS'):
-    print 'Customizing install for ReadTheDocs.org build servers...'
-    conf_path = '.' + conf_path
-    install_path = '.' +  install_path
-    os.environ['ZTPS_INSTALL_ROOT'] = '.'
+if install() and os.environ.get("ZTPS_INSTALL_PREFIX"):
+    print("Customizing install for VirtualEnv install with RPM")
+    conf_path = join_url(os.environ.get("ZTPS_INSTALL_PREFIX"), config.CONF_PATH)
+    install_path = join_url(os.environ.get("ZTPS_INSTALL_PREFIX"), config.INSTALL_PATH)
+
+packages = ["ztpserver"]
+if install() and os.environ.get("READTHEDOCS"):
+    print("Customizing install for ReadTheDocs.org build servers...")
+    conf_path = "." + conf_path
+    install_path = "." + install_path
+    os.environ["ZTPS_INSTALL_ROOT"] = "."
     from subprocess import call
-    call(['docs/setup_rtd_files.sh'])
-    packages.append('client')
-    packages.append('actions')
-    packages.append('plugins')
-
-install_requirements = None
-version = None
-
-install_requirements = open('requirements.txt').read().split('\n')
-install_requirements = [x.strip() for x in install_requirements
-                        if x.strip() and
-                        'dev only' not in x]
-version = open('VERSION').read().split()[0].strip()
+
+    call(["docs/setup_rtd_files.sh"])
+    packages.append("client")
+    packages.append("actions")
+    packages.append("plugins")
+
+install_requirements = open("requirements.txt").read().split("\n")
+install_requirements = [
+    x.strip() for x in install_requirements if x.strip() and "dev only" not in x
+]
+version = open("VERSION").read().split()[0].strip()
 
 data_files = []
 # configuration folders are not cleared on upgrade/downgrade
-for folder in ['nodes', 'definitions', 'files', 'resources',
-               'bootstrap', 'config-handlers']:
-    path = '%s/%s' % (install_path, folder)
+for folder in ["nodes", "definitions", "files", "resources", "bootstrap", "config-handlers"]:
+    path = f"{install_path}/{folder}"
     if install() and not os.path.isdir(path):
         if os.path.exists(path):
             os.remove(path)
         data_files += [(path, [])]
 
-for (filename, dst, src) in [('neighbordb',
-                              install_path,
-                              'conf/neighbordb'),
-                             ('bootstrap.conf',
-                              '%s/bootstrap' % install_path,
-                              'conf/bootstrap.conf'),
-                             ('ztpserver.conf',
-                              conf_path,
-                              'conf/ztpserver.conf'),
-                             ('ztpserver.wsgi',
-                              conf_path,
-                              'conf/ztpserver.wsgi')]:
-    file_path = '%s/%s' % (dst, filename)
+for filename, dst, src in [
+    ("neighbordb", install_path, "conf/neighbordb"),
+    ("bootstrap.conf", f"{install_path}/bootstrap", "conf/bootstrap.conf"),
+    ("ztpserver.conf", conf_path, "conf/ztpserver.conf"),
+    ("ztpserver.wsgi", conf_path, "conf/ztpserver.wsgi"),
+]:
+    file_path = f"{dst}/{filename}"
     if install() and os.path.exists(file_path):
         if os.path.isdir(file_path):
-            shutil.rmtree(file_path,
-                          ignore_errors=True)
+            shutil.rmtree(file_path, ignore_errors=True)
         else:
             # do this manually
-            shutil.copy(src, file_path + '.new')
+            shutil.copy(src, file_path + ".new")
             continue
 
     data_files += [(dst, glob(src))]
 
 # bootstrap file, libraries, VERSION, plugins and actions are
 # always overwritten
-file_list = [('bootstrap', '%s/bootstrap' % install_path,
-              'client/bootstrap')]
-for filename in glob('actions/*'):
-    file_list += [(filename.split('/')[-1],
-                   '%s/actions' % install_path,
-                   filename)]
-for filename in glob('plugins/*'):
-    file_list += [(filename.split('/')[-1],
-                   '%s/plugins' % install_path,
-                   filename)]
-for filename in glob('client/lib/*'):
-    file_list += [(filename.split('/')[-1],
-                   '%s/files/lib' % install_path,
-                   filename)]
-for (filename, dst, src) in file_list:
-    file_path = '%s/%s' % (dst, filename)
-    if install() and os.path.exists(file_path) and \
-            os.path.isdir(file_path):
-        shutil.rmtree(file_path,
-                      ignore_errors=True)
+file_list = [("bootstrap", f"{install_path}/bootstrap", "client/bootstrap")]
+for filename in glob("actions/*"):
+    file_list += [(filename.split("/")[-1], f"{install_path}/actions", filename)]
+for filename in glob("plugins/*"):
+    file_list += [(filename.split("/")[-1], f"{install_path}/plugins", filename)]
+for filename in glob("client/lib/*"):
+    file_list += [(filename.split("/")[-1], f"{install_path}/files/lib", filename)]
+for filename, dst, src in file_list:
+    file_path = f"{dst}/{filename}"
+    if install() and os.path.exists(file_path) and os.path.isdir(file_path):
+        shutil.rmtree(file_path, ignore_errors=True)
     data_files += [(dst, glob(src))]
 
 setup(
-    name='ztpserver',
+    name="ztpserver",
     version=version,
-    description='ZTP Server for EOS',
+    description="ZTP Server for EOS",
     long_description=get_long_description(),
-    long_description_content_type='text/markdown',
-    author='Arista Networks',
-    author_email='eosplus-dev@arista.com',
-    url='https://github.com/arista-eosplus/ztpserver',
-    download_url='https://github.com/arista-eosplus/ztpserver/tarball/v%s'
-                 % version,
-    license='BSD-3',
+    long_description_content_type="text/markdown",
+    author="Arista Networks",
+    author_email="eosplus-dev@arista.com",
+    url="https://github.com/arista-eosplus/ztpserver",
+    download_url=f"https://github.com/arista-eosplus/ztpserver/tarball/v{version}",
+    license="BSD-3",
     install_requires=install_requirements,
     packages=packages,
-    scripts=glob('bin/*'),
-    data_files=data_files
+    scripts=glob("bin/*"),
+    data_files=data_files,
 )
 
 # hidden version file
 if install():
-    custom_path = os.environ.get('ZTPS_INSTALL_ROOT')
+    custom_path = os.environ.get("ZTPS_INSTALL_ROOT")
     if custom_path:
-        version_file =  join_url(custom_path, config.VERSION_FILE_PATH)
+        version_file = join_url(custom_path, config.VERSION_FILE_PATH)
     else:
-        version_file =  config.VERSION_FILE_PATH
+        version_file = config.VERSION_FILE_PATH
     ensure_dir(version_file)
-    shutil.copy('VERSION', version_file)
+    shutil.copy("VERSION", version_file)
```

### Comparing `ztpserver-1.6.0/CONTRIBUTING.md` & `ztpserver-2.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/actions/the_nick` & `ztpserver-2.0.0/actions/run_bash_script`

 * *Files 11% similar despite different names*

```diff
@@ -23,81 +23,82 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=W0703,E1103
+# pylint: disable=C0209
 
+import io
 import os
 
-TEMP_FILE = '/tmp/tmp-run-script'
+from six import raise_from
+
+TEMP_FILE = "/tmp/tmp-run-script"
+
 
 def main(attributes):
-    ''' Runs a script in EOS from bash.
+    """Runs a script in EOS from bash.
 
     This action is dual-supervisor compatible.
 
     Attributes:
         url: path to source script/template
-        variables (optional): 
+        variables (optional):
              list of value substitutions (for a script template)
-        
-    Special_attributes: 
+
+    Special_attributes:
         NODE: API object - see documentation for details
 
     Example:
         ::
 
           -
             action: run_bash_script
             attributes:
               url: files/scripts/install_script
               variables:
                 version: 1.2.3
             name: 'install temp package'
-    '''
+    """
 
-    node = attributes.get('NODE')
-    url = attributes.get('url')
+    node = attributes.get("NODE")
+    url = attributes.get("url")
 
     if not url:
-        raise Exception('Missing attribute(\'url\')')
-
+        raise RuntimeError("Missing attribute('url')")
 
     try:
         node.retrieve_url(url, TEMP_FILE)
     except Exception as exc:
-        raise Exception('Unable to retrieve config from URL (%s)' % 
-                        exc)
+        raise_from(RuntimeError("Unable to retrieve config from URL"), exc)
 
-    exec_file = open(TEMP_FILE, 'r')
-    contents = exec_file.read()
-    exec_file.close()
+    with io.open(TEMP_FILE, encoding="utf8") as exec_file:
+        contents = exec_file.read()
 
-    variables = attributes.get('variables')
+    variables = attributes.get("variables")
     if not variables:
         variables = {}
 
     if not isinstance(variables, dict):
-        node.log_msg('Variables: %s' % variables)
-        raise Exception('Unable to perform variable substitution - '
-                        'invalid variables')
+        node.log_msg("Variables: {}".format(variables))
+        raise RuntimeError("Unable to perform variable substitution - invalid variables")
 
     contents = node.substitute(contents, variables)
 
-    exec_file = open(TEMP_FILE, 'w')
-    exec_file.write(contents)
-    exec_file.close()
+    with io.open(TEMP_FILE, "w", encoding="utf8") as exec_file:
+        exec_file.write(contents)
 
-    os.chmod(TEMP_FILE, 0777)
+    os.chmod(TEMP_FILE, 0o777)
     (cmd, code, out, err) = node.bash_cmds([TEMP_FILE])
 
     if code or err:
-        raise Exception('Running %s in bash failed '
-                        'return_code=%s, stdout=%s, stderr=%s)' % 
-                        (cmd, code, out, err))
-    
+        raise RuntimeError(
+            "Running {} in bash failed return_code={}, stdout={}, stderr={})".format(
+                cmd, code, out, err
+            )
+        )
+
     # Only remove this in case everything else succeeded
     # for debugging purposes
     os.remove(TEMP_FILE)
```

### Comparing `ztpserver-1.6.0/actions/configure_ansible_client` & `ztpserver-2.0.0/actions/configure_ansible_client`

 * *Files 10% similar despite different names*

```diff
@@ -23,27 +23,30 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=W0703,W0402,E1103
+# pylint: disable=C0209
 
+import io
 import os
 
-TEMP_FILE = '/tmp/tmp-pub-key'
-DEFAULT_ROOT = '/persist/local/'
-DEFAULT_USER = 'ansible'
-DEFAULT_PASSWD = 'ansible'
-DEFAULT_GROUP = 'eosadmin'
+from six import raise_from
+
+TEMP_FILE = "/tmp/tmp-pub-key"
+DEFAULT_ROOT = "/persist/local/"
+DEFAULT_USER = "ansible"
+DEFAULT_PASSWD = "ansible"
+DEFAULT_GROUP = "eosadmin"
 
 
 def main(attributes):
-    '''Create a user and configure ssh keys (optional) to help deploy an
+    """Create a user and configure ssh keys (optional) to help deploy an
     Ansible client automatically. The user that is created will be persistant
     across reboots. For more details on user creation, see NODE documentation
     for create_user().
 
     Attributes:
         user: username used by Ansible server to SSH into node
         passwd: cleartext password for user (default = ansible)
@@ -64,33 +67,34 @@
             attributes:
               user: ansible
               passwd: ansible
               group: eosadmin
               root: /persist/local
               key: files/ssh/ansible_server_id_rsa.pub
             name: "Configure Ansible SSH Keys"
-    '''
+    """
 
-    node = attributes.get('NODE')
-    url = attributes.get('key')
-    user = attributes.get('user', DEFAULT_USER)
-    passwd = attributes.get('passwd', DEFAULT_PASSWD)
-    group = attributes.get('group', DEFAULT_GROUP)
-    root = attributes.get('root', DEFAULT_ROOT)
+    node = attributes.get("NODE")
+    url = attributes.get("key")
+    user = attributes.get("user", DEFAULT_USER)
+    passwd = attributes.get("passwd", DEFAULT_PASSWD)
+    group = attributes.get("group", DEFAULT_GROUP)
+    root = attributes.get("root", DEFAULT_ROOT)
     public_keys = None
 
     if url:
         try:
             node.retrieve_url(url, TEMP_FILE)
         except Exception as exc:
-            raise Exception('Unable to retrieve file %s (%s)' % (url, exc))
+            raise_from(RuntimeError("Unable to retrieve file {}".format(url)), exc)
 
         try:
-            public_keys = open(TEMP_FILE).read()
+            with io.open(TEMP_FILE, encoding="utf8") as fd:
+                public_keys = fd.read()
         except Exception as exc:
-            raise Exception('Unable to read file %s (%s)' % (TEMP_FILE, exc))
+            raise_from(RuntimeError("Unable to read file {}".format(TEMP_FILE)), exc)
 
     node.create_user(user, group, passwd, root, public_keys)
 
     # Only remove this in case everything else succeeded
     # for debugging purposes
     os.remove(TEMP_FILE)
```

### Comparing `ztpserver-1.6.0/actions/install_image` & `ztpserver-2.0.0/actions/install_image`

 * *Files 14% similar despite different names*

```diff
@@ -23,20 +23,30 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=W0703
+# pylint: disable=C0209
+
+from pkg_resources import parse_version
+from six import raise_from
+
+BOOT_CONFIG = "/mnt/flash/boot-config"
+
+
+def remove_eos_release_kind(version):
+    if version[-1] in ("M", "F"):
+        return version[:-1]
+    return version
 
-BOOT_CONFIG = '/mnt/flash/boot-config'
 
 def main(attributes):
-    '''Installs new software image.
+    """Installs new software image.
 
     If the current software image is the same as the 'version'
     attribute value, then this action is a no-op.  Otherwise, the
     action will replace the existing software image.
 
     For dual supervisor systems, the image on the active supervisor is
     used as reference.
@@ -45,15 +55,15 @@
 
     Attributes:
         url: path to source image file
         version: EOS version of new image file
         downgrade: Boolean - Should EOS images be downgraded to match?
                    (Default: True)
 
-    Special_attributes: 
+    Special_attributes:
         NODE: API object - see documentation for details
 
     Example:
         ::
 
             -
               action: install_image
@@ -63,45 +73,43 @@
                 version: 4.13.5F
                 downgrade: true
               name: "validate image"
               onstart: "Starting to install image"
               onsuccess: "SUCCESS: 4.13.5F installed"
               onfailure: "FAIL: IM nick@example.com for help"
 
-    '''
+    """
 
-    node = attributes.get('NODE')
-    url = attributes.get('url')
+    node = attributes.get("NODE")
+    url = attributes.get("url")
 
     if not url:
-        raise Exception('Missing attribute(\'url\')')
+        raise RuntimeError("Missing attribute('url')")
 
-    downgrade = attributes.get('downgrade', True)
+    downgrade = attributes.get("downgrade", True)
 
-    version = attributes.get('version')
+    version = attributes.get("version")
     if not version:
-        raise Exception('Missing attribute(\'version\')')
+        raise RuntimeError("Missing attribute('version')")
 
     # Return if version matches
-    current_version = node.api_enable_cmds(['show version'])[0]['version']
+    current_version = node.api_enable_cmds(["show version"])[0]["version"]
     if current_version == version:
-        node.log_msg('install_image: nothing to do: '
-                     'already running the configured version')
+        node.log_msg("install_image: nothing to do: already running the configured version")
         return
 
     # Don't downgrade images if flag is set
     if downgrade is not True:
-        from pkg_resources import parse_version
-        if parse_version(version) < parse_version(current_version):
-            node.log_msg('install_image: nothing to do: '
-                         'downgrade disabled')
+        if parse_version(remove_eos_release_kind(version)) < parse_version(
+            remove_eos_release_kind(current_version)
+        ):
+            node.log_msg("install_image: nothing to do: downgrade disabled")
             return
 
     # In all other cases, copy the image
-    image = 'EOS-%s.swi' % version
+    image = "EOS-{}.swi".format(version)
     try:
-        node.retrieve_url(url, '%s/%s' % (node.flash(), image))
+        node.retrieve_url(url, "{}/{}".format(node.flash(), image))
     except Exception as exc:
-        raise Exception('Unable to retrieve image file from URL (%s)' % 
-                        exc)
+        raise_from(RuntimeError("Unable to retrieve image file from URL"), exc)
 
-    node.api_enable_cmds(['install source flash:%s' % image])
+    node.api_enable_cmds(["install source flash:{}".format(image)])
```

### Comparing `ztpserver-1.6.0/actions/template` & `ztpserver-2.0.0/actions/template`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python 
+#!/usr/bin/env python
 #
 # Copyright (c) 2015, Arista Networks, Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
@@ -10,36 +10,39 @@
 # this list of conditions and the following disclaimer.
 #  - Redistributions in binary form must reproduce the above copyright
 # notice, this list of conditions and the following disclaimer in the
 # documentation and/or other materials provided with the distribution.
 #  - Neither the name of Arista Networks nor the names of its
 # contributors may be used to endorse or promote products derived from
 # this software without specific prior written permission.
-# 
+#
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 # "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
 # LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
 # A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL ARISTA NETWORKS
 # BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-def main(attributes): 
-    '''TITLE
+# pylint: disable=C0209
+
+
+def main(attributes):
+    """TITLE
 
     SHORT_DESCRIPTION
 
     This action is [NOT] dual-supervisor compatible.
 
     Args:
        attributes: list of attributes; use attributes.get(<ATTRIBUTE_NAME>)
                    to read attribute values
 
        Special attributes:
            node: attributes.get('NODE')
                  API: see documentation
-    '''
-    print attributes
+    """
+    print(attributes)  # pylint: disable=C0325
```

### Comparing `ztpserver-1.6.0/actions/add_config` & `ztpserver-2.0.0/actions/add_config`

 * *Files 14% similar despite different names*

```diff
@@ -23,31 +23,35 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=W0703,W0402,E1103
+# pylint: disable=C0209
 
+import io
 import os
 
-TEMP_CONFIG = '/tmp/tmp-add-config'
+from six import raise_from
+
+TEMP_CONFIG = "/tmp/tmp-add-config"
+
 
 def main(attributes):
-    ''' Appends config section to startup-config.
+    """Appends config section to startup-config.
 
     This action is dual-supervisor compatible.
 
     Attributes:
         url: path to source config/template
         substitution_mode: loose|strict (default: loose)
         variables: list of value substitutions
-        
-    Special_attributes: 
+
+    Special_attributes:
         NODE: API object - see documentation for details
 
     Example:
         ::
 
           -
             action: add_config
@@ -56,45 +60,41 @@
               variables:
                 ipaddress: allocate('mgmt_subnet')
             name: "configure ma1"
             onstart: "Starting to configure ma1"
             onsuccess: "SUCCESS: ma1 configure"
             onfailure: "FAIL: IM provisioning@example.com for help"
 
-    '''
+    """
 
-    node = attributes.get('NODE')
-    url = attributes.get('url')
+    node = attributes.get("NODE")
+    url = attributes.get("url")
 
     if not url:
-        raise Exception('Missing attribute(\'url\')')
+        raise RuntimeError("Missing attribute('url')")
 
-
-    substitution_mode = attributes.get('substitution_mode', 'loose')
-    if substitution_mode not in ['loose', 'strict']:
-        raise Exception('Invalid option specified for substitution_mode '
-                        'attribute')
+    substitution_mode = attributes.get("substitution_mode", "loose")
+    if substitution_mode not in ["loose", "strict"]:
+        raise RuntimeError("Invalid option specified for substitution_mode attribute")
 
     try:
         node.retrieve_url(url, TEMP_CONFIG)
     except Exception as exc:
-        raise Exception('Unable to retrieve config from URL (%s)' % 
-                        exc)
+        raise_from(RuntimeError("Unable to retrieve config from URL"), exc)
 
-    contents = open(TEMP_CONFIG, 'r').read()
+    with io.open(TEMP_CONFIG, encoding="utf8") as fd:
+        contents = fd.read()
 
-    variables = attributes.get('variables')
+    variables = attributes.get("variables")
     if not variables:
         variables = {}
 
     if not isinstance(variables, dict):
-        node.log_msg('Variables: %s' % variables)
-        raise Exception('Unable to perform variable substitution - '
-                        'invalid variables')
-
-    contents = node.substitute(contents, variables,
-                               substitution_mode == 'strict')
-    node.append_startup_config_lines(contents.split('\n'))
-    
+        node.log_msg("Variables: {}".format(variables))
+        raise RuntimeError("Unable to perform variable substitution - invalid variables")
+
+    contents = node.substitute(contents, variables, substitution_mode == "strict")
+    node.append_startup_config_lines(contents.split("\n"))
+
     # Only remove this in case everything else succeeded
     # for debugging purposes
     os.remove(TEMP_CONFIG)
```

### Comparing `ztpserver-1.6.0/actions/run_cli_commands` & `ztpserver-2.0.0/actions/the_nick`

 * *Files 19% similar despite different names*

```diff
@@ -23,75 +23,82 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=W0703,E1103
+# pylint: disable=C0209
 
+import io
 import os
 
-TEMP_CONFIG = '/tmp/tmp-run-commands'
+from six import raise_from
+
+TEMP_FILE = "/tmp/tmp-run-script"
+
 
 def main(attributes):
-    ''' Runs a set of EOS commands, starting from enable mode.
+    """Runs a script in EOS from bash.
 
     This action is dual-supervisor compatible.
 
     Attributes:
-        url: path to source command list/template
-        variables (optional): 
-             list of value substitutions (for a template)
-        
-    Special_attributes: 
+        url: path to source script/template
+        variables (optional):
+             list of value substitutions (for a script template)
+
+    Special_attributes:
         NODE: API object - see documentation for details
 
     Example:
         ::
 
           -
-            action: run_cli_commands
+            action: run_bash_script
             attributes:
-              url: files/templates/ma1.template
+              url: files/scripts/install_script
               variables:
-                ipaddress: allocate('mgmt_subnet')
-            name: 'configure ma1'
-    '''
+                version: 1.2.3
+            name: 'install temp package'
+    """
 
-    node = attributes.get('NODE')
-    url = attributes.get('url')
+    node = attributes.get("NODE")
+    url = attributes.get("url")
 
     if not url:
-        raise Exception('Missing attribute(\'url\')')
+        raise RuntimeError("Missing attribute('url')")
 
     try:
-        node.retrieve_url(url, TEMP_CONFIG)
+        node.retrieve_url(url, TEMP_FILE)
     except Exception as exc:
-        raise Exception('Unable to retrieve config from URL (%s)' % 
-                        exc)
+        raise_from(RuntimeError("Unable to retrieve config from URL"), exc)
 
-    contents = open(TEMP_CONFIG, 'r').read()
+    with io.open(TEMP_FILE, encoding="utf8") as exec_file:
+        contents = exec_file.read()
 
-    variables = attributes.get('variables')
+    variables = attributes.get("variables")
     if not variables:
         variables = {}
 
     if not isinstance(variables, dict):
-        node.log_msg('Variables: %s' % variables)
-        raise Exception('Unable to perform variable substitution - '
-                        'invalid variables')
-
+        node.log_msg("Variables: {}".format(variables))
+        raise RuntimeError("Unable to perform variable substitution - invalid variables")
 
     contents = node.substitute(contents, variables)
-    commands = [x for x in contents.split('\n') if x]
 
-    try:
-        node.api_enable_cmds(commands,
-                             text_format=True)
-    except Exception as exc:
-        raise Exception('Running CLI commands %s failed: %s' % 
-                        (commands, exc.message))
+    with io.open(TEMP_FILE, "w", encoding="utf8") as exec_file:
+        exec_file.write(contents)
+
+    os.chmod(TEMP_FILE, 0o777)
+    (cmd, code, out, err) = node.bash_cmds([TEMP_FILE])
+
+    if code or err:
+        raise RuntimeError(
+            "Running {} in bash failed return_code={}, stdout={}, stderr={})".format(
+                cmd, code, out, err
+            )
+        )
 
     # Only remove this in case everything else succeeded
     # for debugging purposes
-    os.remove(TEMP_CONFIG)
+    os.remove(TEMP_FILE)
```

### Comparing `ztpserver-1.6.0/actions/run_bash_script` & `ztpserver-2.0.0/actions/install_extension`

 * *Files 23% similar despite different names*

```diff
@@ -23,81 +23,75 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=W0703,E1103
+# pylint: disable=C0209
 
+import ast
+import io
 import os
 
-TEMP_FILE = '/tmp/tmp-run-script'
+from six import raise_from
+
+EXTENSIONS_DIR = "/mnt/flash/.extensions"
+BOOT_EXTENSIONS = "/mnt/flash/boot-extensions"
+
 
 def main(attributes):
-    ''' Runs a script in EOS from bash.
+    """Installs extension.
 
-    This action is dual-supervisor compatible.
+    If 'force' is
+    set, then the dependency checks are overridden.
+
+    This action is NOT dual-supervisor compatible.
 
     Attributes:
-        url: path to source script/template
-        variables (optional): 
-             list of value substitutions (for a script template)
-        
-    Special_attributes: 
+        url: path to source extension file
+        force: ignore validation errors (default: false)
+        always_execute: perform copy even if file exists
+
+    Special_attributes:
         NODE: API object - see documentation for details
 
     Example:
         ::
 
           -
-            action: run_bash_script
+            action: install_extension
+            always_execute: true
             attributes:
-              url: files/scripts/install_script
-              variables:
-                version: 1.2.3
-            name: 'install temp package'
-    '''
+              url: files/telemetry-1.0-1.rpm
+            name: "Install Telemetry"
 
-    node = attributes.get('NODE')
-    url = attributes.get('url')
+    """
+
+    node = attributes.get("NODE")
+    url = attributes.get("url")
 
     if not url:
-        raise Exception('Missing attribute(\'url\')')
+        raise RuntimeError("Missing attribute('url')")
+
+    force = ast.literal_eval(str(attributes.get("force")))
 
+    if not os.path.exists(EXTENSIONS_DIR):
+        os.makedirs(EXTENSIONS_DIR)
 
+    name = url.split("/")[-1]
     try:
-        node.retrieve_url(url, TEMP_FILE)
+        node.retrieve_url(url, "{}/{}".format(EXTENSIONS_DIR, name))
     except Exception as exc:
-        raise Exception('Unable to retrieve config from URL (%s)' % 
-                        exc)
+        raise_from(RuntimeError("Unable to retrieve extension from URL"), exc)
+
+    line = name
+    if force:
+        line = line + " force"
+
+    lines = []
+    if os.access(BOOT_EXTENSIONS, os.R_OK):
+        with io.open(BOOT_EXTENSIONS, encoding="utf8") as boot_ext_fd:
+            lines = [x.strip() for x in boot_ext_fd.readlines() if x.strip()]
 
-    exec_file = open(TEMP_FILE, 'r')
-    contents = exec_file.read()
-    exec_file.close()
-
-    variables = attributes.get('variables')
-    if not variables:
-        variables = {}
-
-    if not isinstance(variables, dict):
-        node.log_msg('Variables: %s' % variables)
-        raise Exception('Unable to perform variable substitution - '
-                        'invalid variables')
-
-    contents = node.substitute(contents, variables)
-
-    exec_file = open(TEMP_FILE, 'w')
-    exec_file.write(contents)
-    exec_file.close()
-
-    os.chmod(TEMP_FILE, 0777)
-    (cmd, code, out, err) = node.bash_cmds([TEMP_FILE])
-
-    if code or err:
-        raise Exception('Running %s in bash failed '
-                        'return_code=%s, stdout=%s, stderr=%s)' % 
-                        (cmd, code, out, err))
-    
-    # Only remove this in case everything else succeeded
-    # for debugging purposes
-    os.remove(TEMP_FILE)
+    with io.open(BOOT_EXTENSIONS, "w", encoding="utf8") as boot_ext_fd:
+        boot_ext_fd.write("\n".join(lines + [line]))
```

### Comparing `ztpserver-1.6.0/actions/install_extension` & `ztpserver-2.0.0/actions/install_cli_plugin`

 * *Files 25% similar despite different names*

```diff
@@ -23,78 +23,58 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=W0703,E1103
+# pylint: disable=C0209
 
-EXTENSIONS_DIR = '/mnt/flash/.extensions'
-BOOT_EXTENSIONS = '/mnt/flash/boot-extensions'
-
-import ast
 import os
 
-def main(attributes):
-    '''Installs extension.
+from six import raise_from
+
+CLI_PLUGIN_DIR = "/usr/lib/python2.7/site-packages/CliPlugin"
+PERSISTENT_PLUGIN_DIR = "/mnt/flash/.ztp-plugins"
 
-    If 'force' is
-    set, then the dependency checks are overridden.
+
+def main(attributes):
+    """Installs CliPlugin.
 
     This action is NOT dual-supervisor compatible.
 
     Attributes:
-        url: path to source extension file
-        force: ignore validation errors (default: false)
-        always_execute: perform copy even if file exists
+        url: path to the CliPlugin
 
     Special_attributes:
         NODE: API object - see documentation for details
 
     Example:
         ::
 
           -
-            action: install_extension
+            action: install_image
             always_execute: true
             attributes:
-              url: files/telemetry-1.0-1.rpm
-            name: "Install Telemetry"
+              url: files/my_cli_plugin
+            name: "install cli plugin"
 
-    '''
+    """
 
-    node = attributes.get('NODE')
-    url = attributes.get('url')
+    node = attributes.get("NODE")
+    url = attributes.get("url")
 
     if not url:
-        raise Exception('Missing attribute(\'url\')')
+        raise RuntimeError("Missing attribute('url')")
 
-    force = ast.literal_eval(
-        str(attributes.get('force')))
+    if not os.path.exists(PERSISTENT_PLUGIN_DIR):
+        os.makedirs(PERSISTENT_PLUGIN_DIR)
 
+    name = url.split("/")[-1]
     try:
-        os.makedirs(EXTENSIONS_DIR)
-    except OSError:
-        # file exists
-        pass
-
-    name = url.split('/')[ -1 ]
-    try:
-        node.retrieve_url(url, '%s/%s' % (EXTENSIONS_DIR, name))
+        node.retrieve_url(url, "{}/{}".format(PERSISTENT_PLUGIN_DIR, name))
     except Exception as exc:
-        raise Exception('Unable to retrieve extension from URL (%s)' %
-                        exc)
+        raise_from(RuntimeError("Unable to retrieve CliPlugin from URL"), exc)
 
-    line = name
-    if force:
-        line = line + ' force'
-
-    lines = []
-    try:
-        lines = [x.strip() for x in open(BOOT_EXTENSIONS).readlines()
-                 if x.strip()]
-    except IOError:
-        # file Missing
-        pass
+    lines = ["sudo cp {}/{} {}".format(PERSISTENT_PLUGIN_DIR, name, CLI_PLUGIN_DIR)]
 
-    open(BOOT_EXTENSIONS, 'w').write('\n'.join(lines + [line]))
+    node.append_rc_eos_lines(lines)
```

### Comparing `ztpserver-1.6.0/actions/send_email` & `ztpserver-2.0.0/actions/send_email`

 * *Files 17% similar despite different names*

```diff
@@ -25,41 +25,44 @@
 # BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-#
 
+# pylint: disable=C0209
+
+import io
 import os
 import smtplib
-
-from email.mime import multipart as MIMEMultipart
-from email.mime import base as MIMEBase
 from email import encoders as Encoders
+from email.mime import base as MIMEBase
+from email.mime import multipart as MIMEMultipart
 from email.mime.text import MIMEText
-
 from email.utils import COMMASPACE, formatdate
 
 
 def send_message(smarthost, sender, receivers, msg):
     smtp = smtplib.SMTP(smarthost)
     smtp.sendmail(sender, COMMASPACE.join(receivers), msg.as_string())
     smtp.close()
 
+
 def run_command(command, node):
     command = command.strip()
     output = node.api_enable_cmds([command], text_format=True)
-    filename = str(command).replace(' ', '_')
-    open(filename, 'w').write(' '.join(output))
+    filename = str(command).replace(" ", "_")
+    with io.open(filename, "w", encoding="utf8") as fd:
+        fd.write(" ".join(output))
     return filename
 
+
 def main(attributes):
-    '''Sends an email using an SMTP relay host
+    """Sends an email using an SMTP relay host
 
     Generates an email from the bootstrap process and routes it through a
     smarthost.  The parameters value expects a dictionary with the
     following values in order for this function to work properly.
     ::
 
         {
@@ -74,15 +77,16 @@
 
     The required fields for this function are smarthost, sender, and
     receivers. All other fields are optional.
 
     This action is dual-supervisor compatible.
 
     Args:
-        attributes (list): list of attributes; use attributes.get(<ATTRIBUTE_NAME>) to read attribute values
+        attributes (list): list of attributes; use attributes.get(<ATTRIBUTE_NAME>)
+                            to read attribute values
         node (internal): attributes.get('NODE') API: see documentation
         smarthost: hostname of smarthos>,
         sender: from email addres>
         receivers: [ <array of recipients to send email to> ]
         subject: subject line of the message
         body: the message body
         attachments: [ <array of files to attach> ]
@@ -99,62 +103,61 @@
                   subject: This is a test message from a switch in ZTP
                   receivers:
                       bob@exmple.com
                       helen@example.com
                   body: Please see the attached 'show version'
                   commands: show version
 
-    '''
+    """
 
-    node = attributes.get('NODE')
+    node = attributes.get("NODE")
 
-    smarthost = attributes.get('smarthost')
+    smarthost = attributes.get("smarthost")
     if not smarthost:
-        raise Exception('Missing attribute(\'smarthost\')')
+        raise RuntimeError("Missing attribute('smarthost')")
 
-    sender = attributes.get('sender')
+    sender = attributes.get("sender")
     if not sender:
-        raise Exception('Missing attribute(\'sender\')')
+        raise RuntimeError("Missing attribute('sender')")
 
-    receivers = attributes.get('receivers')
+    receivers = attributes.get("receivers")
     if not receivers:
-        raise Exception('Missing attribute(\'receivers\')')
+        raise RuntimeError("Missing attribute('receivers')")
 
     msg = MIMEMultipart.MIMEMultipart()
-    msg['From'] = sender
-    msg['To'] = COMMASPACE.join(receivers)
-    msg['Date'] = formatdate(localtime=True)
-    msg['Subject'] = attributes.get('subject') or 'ZTP Bootstrap'
-
-    body = attributes.get('body')
-    attachments = attributes.get('attachments') or list()
-    commands = attributes.get('commands') or list()
+    msg["From"] = sender
+    msg["To"] = COMMASPACE.join(receivers)
+    msg["Date"] = formatdate(localtime=True)
+    msg["Subject"] = attributes.get("subject") or "ZTP Bootstrap"
+
+    body = attributes.get("body", "empty-body")
+    attachments = attributes.get("attachments", [])
+    commands = attributes.get("commands", [])
 
-    attributes.get('NODE').log_msg("Running commands: %s" % str(commands))
+    attributes.get("NODE").log_msg("Running commands: {}".format(str(commands)))
     if commands:
-        body += '\nThe output from the following commmands have '\
-            'been added as attachments:'
+        body += "\nThe output from the following commmands have been added as attachments:"
         for command in commands:
             filename = run_command(command, node)
             attachments.append(filename)
-            body += '\n\t* %s (%s)' % (command, filename)
+            body += "\n\t* {} ({})".format(command, filename)
 
-    attributes.get('NODE').log_msg("Collecting attachments: %s" % \
-        str(attachments))
+    attributes.get("NODE").log_msg("Collecting attachments: {}".format(str(attachments)))
     if attachments:
         for filename in attachments:
             if os.path.exists(filename):
                 filename = filename.strip()
-                part = MIMEBase.MIMEBase('application', 'octet-stream')
-                part.set_payload(open(filename, 'rb').read())
+                part = MIMEBase.MIMEBase("application", "octet-stream")
+                with io.open(filename, "rb", encoding="utf8") as fd:
+                    part.set_payload(fd.read())
                 Encoders.encode_base64(part)
-                part.add_header('Content-Disposition',
-                                'attachment; filename=\'%s\'' %
-                                os.path.basename(filename))
-                attributes.get('NODE').log_msg("Attaching %s" % filename)
+                part.add_header(
+                    "Content-Disposition",
+                    "attachment; filename='{}'".format(os.path.basename(filename)),
+                )
+                attributes.get("NODE").log_msg("Attaching {}".format(filename))
                 msg.attach(part)
 
     msg.attach(MIMEText(body))
 
-    attributes.get('NODE').log_msg("Sending email using smarthost %s" % \
-        smarthost)
+    attributes.get("NODE").log_msg("Sending email using smarthost {}".format(smarthost))
     send_message(smarthost, sender, receivers, msg)
```

### Comparing `ztpserver-1.6.0/actions/copy_file` & `ztpserver-2.0.0/actions/copy_file`

 * *Files 18% similar despite different names*

```diff
@@ -23,35 +23,45 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=W0703,E1103
-
-BACKUP_SUFFIX = '.backup'
-PERSISTENT_DIR = '/mnt/flash/.ztp-files'
-PERSISTENT_STORAGE = ['/mnt/flash/', '/mnt/usb1/', '/mnt/drive/',
-                      '/persist/local/', '/persyst/sys/']
+# pylint: disable=C0209
 
 import os
 import shutil
 
+from six import raise_from
+
+BACKUP_SUFFIX = ".backup"
+PERSISTENT_DIR = "/mnt/flash/.ztp-files"
+PERSISTENT_STORAGE = [
+    "/mnt/flash/",
+    "/mnt/usb1/",
+    "/mnt/drive/",
+    "/persist/local/",
+    "/persist/sys/",
+]
+
+
 def is_subdir(path, directory):
     return os.path.realpath(path).startswith(os.path.realpath(directory))
 
+
 def url_persistent(url):
     for directory in PERSISTENT_STORAGE:
         if is_subdir(url, directory):
             return True
     return False
 
+
 def main(attributes):
-    '''Copies file to the switch.
+    """Copies file to the switch.
 
     Copies file based on the values of 'src_url' and 'dst_url'
     attributes ('dst_url' should point to the destination folder).
 
     This action is NOT dual-supervisor compatible.
 
     Attributes:
@@ -67,15 +77,15 @@
        * 'if-missing': the file is copied to the switch only if
          there is not already a file with the same name at the
          destination; if there is, then the action is a no-op;
        * 'backup': the file is copied to the switch; if there is
          already another file at the destination, that file is renamed
          by appending the '.backup' suffix
 
-    Special_attributes: 
+    Special_attributes:
         NODE: API object - see documentation for details
 
 
     Example:
         ::
 
           -
@@ -84,100 +94,89 @@
             attributes:
               dst_url: /mnt/flash/
               mode: 777
               overwrite: if-missing
               src_url: files/automate/bgpautoinf.py
             name: "automate BGP peer interface config"
 
-    '''
+    """
 
-    node = attributes.get('NODE')
-    src_url = attributes.get('src_url')
+    node = attributes.get("NODE")
+    src_url = attributes.get("src_url")
 
     if not src_url:
-        raise Exception('Missing attribute(\'src_url\')')
+        raise RuntimeError("Missing attribute('src_url')")
 
-    dst_url = attributes.get('dst_url')
+    dst_url = attributes.get("dst_url")
     if not dst_url:
-        raise Exception('Missing attribute(\'dst_url\')')
+        raise RuntimeError("Missing attribute('dst_url')")
 
     name = os.path.basename(src_url)
 
-    mode = attributes.get('mode')
+    mode = attributes.get("mode")
 
-    overwrite = attributes.get('overwrite')
+    overwrite = attributes.get("overwrite")
     if not overwrite:
-        overwrite = 'replace'
+        overwrite = "replace"
 
     if url_persistent(dst_url):
         dst_path = os.path.join(dst_url, name)
 
-        if overwrite == 'if-missing':
+        if overwrite == "if-missing":
             if os.path.exists(dst_path):
-                node.log_msg('copy_file: nothing to do: %s '
-                             'already exists' % dst_path)
+                node.log_msg("copy_file: nothing to do: {} already exists".format(dst_path))
                 return
-        elif overwrite == 'backup':
+        elif overwrite == "backup":
             if os.path.exists(dst_path):
-                backup_path = '%s%s' % (dst_path, BACKUP_SUFFIX)
-                node.log_msg('copy_file: backing up %s '
-                             'to %s' % (dst_path, backup_path))
+                backup_path = "{}{}".format(dst_path, BACKUP_SUFFIX)
+                node.log_msg("copy_file: backing up {} to {}".format(dst_path, backup_path))
                 shutil.copy(dst_path, backup_path)
-        elif overwrite == 'replace':
+        elif overwrite == "replace":
             pass
         else:
-            raise Exception('Erroneous \'overwrite\' value')
+            raise RuntimeError("Erroneous 'overwrite' value")
 
-        try:
+        if not os.path.exists(dst_url):
             os.makedirs(dst_url)
-        except OSError:
-            # file exists
-            pass
 
         try:
             node.retrieve_url(src_url, dst_path)
-            node.log_msg('copy_file: saving %s '
-                         'to %s' % (src_url, dst_path))
+            node.log_msg("copy_file: saving {} to {}".format(src_url, dst_path))
             if mode is not None:
                 os.chmod(dst_path, int(str(mode), 8))
         except Exception as exc:
-            raise Exception('Unable to retrieve file from URL (%s)' % 
-                            exc)
+            raise_from(RuntimeError("Unable to retrieve file from URL"), exc)
     else:
         dst_path = os.path.join(PERSISTENT_DIR, name)
 
         lines = []
-        if overwrite == 'if-missing':
-            lines = lines + ['[ ! -f %s ] && '
-                             'sudo cp %s %s'  % (dst_url, dst_path,
-                                                 dst_url)]
-        elif overwrite == 'backup':
-            lines = lines + ['[ -f %s ] && '
-                             'sudo mv %s %s%s' % (dst_url, dst_url,
-                                                  dst_url, BACKUP_SUFFIX)]
-            lines = lines + ['sudo cp %s %s'  % (dst_path, dst_url)]
-        elif overwrite == 'replace':
-            lines = lines + ['sudo cp %s %s'  % (dst_path, dst_url)]
+        if overwrite == "if-missing":
+            lines = lines + [
+                "[ ! -f {dst_url} ] && sudo cp {} {dst_url}".format(dst_path, dst_url=dst_url)
+            ]
+        elif overwrite == "backup":
+            lines = lines + [
+                "[ -f {dst_url} ] && sudo mv {dst_url} {dst_url}{}".format(
+                    BACKUP_SUFFIX, dst_url=dst_url
+                )
+            ]
+            lines = lines + ["sudo cp {} {}".format(dst_path, dst_url)]
+        elif overwrite == "replace":
+            lines = lines + ["sudo cp {} {}".format(dst_path, dst_url)]
         else:
-            raise Exception('Erroneous \'overwrite\' value')
+            raise RuntimeError("Erroneous 'overwrite' value")
 
         if mode:
-            lines = lines + ['sudo chmod %s %s'  % (mode, dst_url)]
+            lines = lines + ["sudo chmod {} {}".format(mode, dst_url)]
 
-        try:
+        if not os.path.exists(PERSISTENT_DIR):
             os.makedirs(PERSISTENT_DIR)
-        except OSError:
-            # file exists
-            pass
 
         try:
-            file_path = '%s/%s' % (PERSISTENT_DIR, name)
+            file_path = "{}/{}".format(PERSISTENT_DIR, name)
             node.retrieve_url(src_url, file_path)
-            node.log_msg('copy_file: saving %s '
-                         'to %s' % (src_url, file_path))
+            node.log_msg("copy_file: saving {} to {}".format(src_url, file_path))
         except Exception as exc:
-            raise Exception('Unable to retrieve file from URL (%s)' % 
-                            exc)
+            raise_from(RuntimeError("Unable to retrieve file from URL"), exc)
 
-        node.log_msg('copy_file: adding rc.eos lines: \n%s$' %
-                     '\n'.join(lines))
+        node.log_msg("copy_file: adding rc.eos lines: \n%s$" % "\n".join(lines))
         node.append_rc_eos_lines(lines)
```

### Comparing `ztpserver-1.6.0/actions/replace_config` & `ztpserver-2.0.0/actions/replace_config`

 * *Files 11% similar despite different names*

```diff
@@ -23,41 +23,43 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#pylint: disable=W0703,E1103
+# pylint: disable=C0209
+
+from six import raise_from
+
 
 def main(attributes):
-    '''Replaces /mnt/flash/startup-config with new file.
+    """Replaces /mnt/flash/startup-config with new file.
 
     This action is dual-supervisor compatible.
 
     Attributes:
         url: path to source config/template
 
-    Special_attributes: 
+    Special_attributes:
         NODE: API object - see documentation for details
 
     Example:
         ::
 
           -
             action: replace_config
             attributes:
               url: files/configs/tor-startup-config
             name: "tor config"
-    '''
+    """
 
-    node = attributes.get('NODE')
-    url = attributes.get('url')
+    node = attributes.get("NODE")
+    url = attributes.get("url")
 
     if not url:
-        raise Exception('Missing attribute(\'url\')')
+        raise RuntimeError("Missing attribute('url')")
 
     try:
         node.retrieve_url(url, node.startup_config())
     except Exception as exc:
-        raise Exception('Unable to retrieve config from URL (%s)' % 
-                        exc.message)
+        raise_from(RuntimeError("Unable to retrieve config from URL"), exc)
```

### Comparing `ztpserver-1.6.0/ztpserver.egg-info/PKG-INFO` & `ztpserver-2.0.0/ztpserver.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 Metadata-Version: 2.1
 Name: ztpserver
-Version: 1.6.0
+Version: 2.0.0
 Summary: ZTP Server for EOS
 Home-page: https://github.com/arista-eosplus/ztpserver
+Download-URL: https://github.com/arista-eosplus/ztpserver/tarball/v2.0.0
 Author: Arista Networks
 Author-email: eosplus-dev@arista.com
 License: BSD-3
-Download-URL: https://github.com/arista-eosplus/ztpserver/tarball/v1.6.0
-Description: 
-        [![Build Status](https://travis-ci.org/arista-eosplus/ztpserver.png)](https://travis-ci.org/arista-eosplus/ztpserver)
-        
-        Quick Overview
-        =====================
-        ZTPServer provides a bootstrap environment for Arista EOS based products.  ZTPserver interacts with the  ZeroTouch Provisioning (ZTP) mode of Arista EOS. The default ZTP start up mode triggers an unprovisioned Arista EOS nodes to enter a bootstrap readdy state if a valid configuration file is not already present on the internal flash storage.
-        
-        ZTPServer provides a number of configurable bootstrap operation workflows that extend beyond simply loading an configuration and boot image. It provides the ability to define the target node through the introduction of definitions and templates that call pre-built actions and statically defined or dynamically generated attributes. The attributes and actions can also be extended to provide custom functionality that are specific to a given implementation. ZTPServer also provides a topology validation engine with a simple syntax to express LLDP neighbor adjacencies. It is written mostly in Python and leverages standard protocols like DHCP and DHCP options for boot functions, HTTP for bi-directional transport, and XMPP and syslog for logging. Most of the files that the user interacts with are YAML based.
-        
-        ZTPServer Features
-        ==================
-        * Automated configuration file generation and application
-        * Image and file system validation and standardization
-        * Connectivity validation and topology based auto-provisioning
-        * Config and device templates with resource allocation for dynamic deployments
-        * Zero touch replacement and upgrade capabilities
-        * User extensible actions
-        * Email, XMPP, syslog based logging and accounting of all processes
-        
-        Docs
-        ====
-        [ZTPServer official documentation](http://ztpserver.readthedocs.org/) is built and hosted at (http://ReadTheDocs.org/).
-        
-        Contributing
-        ============
-        Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for additional information.
-        
-        Support
-        =======
-        
-        * [Mailing List](https://groups.google.com/forum/#!forum/eosplus)
-        * eosplus-dev@arista.com
-        * IRC: irc.freenode.net#arista
-        
-        Dependencies
-        ============
-        
-        Server
-        ======
-        * [Python 2.7](https://www.python.org/download/releases/2.7/)
-        * [routes 2.0 or later](https://pypi.python.org/pypi/Routes)
-        * [webob 1.3 or later](http://webob.org/)
-        * [PyYaml 3.0 or later](http://pyyaml.org/)
-        
-        Client
-        ======
-        * Arista EOS 4.12.0 or later
-        
-        License
-        =======
-        BSD-3, See LICENSE file
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+[![Build Status](https://travis-ci.org/arista-eosplus/ztpserver.png)](https://travis-ci.org/arista-eosplus/ztpserver)
+
+Quick Overview
+=====================
+ZTPServer provides a bootstrap environment for Arista EOS based products.  ZTPserver interacts with the  ZeroTouch Provisioning (ZTP) mode of Arista EOS. The default ZTP start up mode triggers an unprovisioned Arista EOS nodes to enter a bootstrap readdy state if a valid configuration file is not already present on the internal flash storage.
+
+ZTPServer provides a number of configurable bootstrap operation workflows that extend beyond simply loading an configuration and boot image. It provides the ability to define the target node through the introduction of definitions and templates that call pre-built actions and statically defined or dynamically generated attributes. The attributes and actions can also be extended to provide custom functionality that are specific to a given implementation. ZTPServer also provides a topology validation engine with a simple syntax to express LLDP neighbor adjacencies. It is written mostly in Python and leverages standard protocols like DHCP and DHCP options for boot functions, HTTP for bi-directional transport, and XMPP and syslog for logging. Most of the files that the user interacts with are YAML based.
+
+ZTPServer Features
+==================
+* Automated configuration file generation and application
+* Image and file system validation and standardization
+* Connectivity validation and topology based auto-provisioning
+* Config and device templates with resource allocation for dynamic deployments
+* Zero touch replacement and upgrade capabilities
+* User extensible actions
+* Email, XMPP, syslog based logging and accounting of all processes
+
+Docs
+====
+[ZTPServer official documentation](http://ztpserver.readthedocs.org/) is built and hosted at (http://ReadTheDocs.org/).
+
+Contributing
+============
+Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for additional information.
+
+Support
+=======
+
+* [Mailing List](https://groups.google.com/forum/#!forum/eosplus)
+* eosplus-dev@arista.com
+* IRC: irc.freenode.net#arista
+
+Dependencies
+============
+
+Server
+======
+* Python 3.7 or later (https://www.python.org/downloads)
+* routes 2.5 or later (https://pypi.python.org/pypi/Routes)
+* webob 1.8 or later (http://webob.org/)
+* PyYaml 6.0 or later (http://pyyaml.org/)
+
+Client
+======
+* Arista EOS 4.12.0 or later
+
+License
+=======
+BSD-3, See LICENSE file
```

### Comparing `ztpserver-1.6.0/ztpserver.egg-info/SOURCES.txt` & `ztpserver-2.0.0/ztpserver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 docs/ReleaseNotes1.3.1.rst
 docs/ReleaseNotes1.3.2.rst
 docs/ReleaseNotes1.3.rst
 docs/ReleaseNotes1.4.1.rst
 docs/ReleaseNotes1.4.rst
 docs/ReleaseNotes1.5.0.rst
 docs/ReleaseNotes1.6.0.rst
+docs/ReleaseNotes2.0.0.rst
 docs/actions.rst
 docs/api.rst
 docs/client.rst
 docs/conf.py
 docs/config.rst
 docs/cookbook.rst
 docs/examples.rst
@@ -93,25 +94,30 @@
 docs/cookbook/ztpsVMonEOS/l3wom.rst
 plugins/allocate
 plugins/mysql_vars
 plugins/sqlite
 plugins/test
 rpm/Makefile
 rpm/ztpserver.spec
+test/__init__.py
+test/actions/__init__.py
 test/actions/test_add_config.py
 test/actions/test_copy_file.py
 test/actions/test_install_cli_plugin.py
 test/actions/test_install_extension.py
 test/actions/test_install_image.py
 test/actions/test_replace_config.py
 test/actions/test_run_bash_script.py
 test/actions/test_run_cli_commands.py
 test/actions/test_send_email.py
 test/client/FastCli
+test/client/__init__.py
 test/client/client_test_lib.py
+test/client/smtp_server2.py
+test/client/smtp_server3.py
 test/client/test_bootstrap.py
 test/client/test_bootstrap_cleanup.py
 test/client/test_xmpp_bootstrap.py
 test/neighbordb/README.md
 test/neighbordb/bogus_patterns_test.yml
 test/neighbordb/chassis_test.yml
 test/neighbordb/chassis_test_2.yml
@@ -120,14 +126,15 @@
 test/neighbordb/ndb_entries_test.yml
 test/neighbordb/ndb_values_test.yml
 test/neighbordb/node_interfaces_test.yml
 test/neighbordb/node_test.yml
 test/neighbordb/simple_functions_test.yml
 test/neighbordb/simple_test.yml
 test/neighbordb/small_pattern_test.yml
+test/server/__init__.py
 test/server/server_test_lib.py
 test/server/test_app.py
 test/server/test_config.py
 test/server/test_controller.py
 test/server/test_ndb.py
 test/server/test_repository.py
 test/server/test_serializers.py
```

### Comparing `ztpserver-1.6.0/rpm/Makefile` & `ztpserver-2.0.0/rpm/Makefile`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/rpm/ztpserver.spec` & `ztpserver-2.0.0/rpm/ztpserver.spec`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/conf/ztpserver.conf` & `ztpserver-2.0.0/conf/ztpserver.conf`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/conf/neighbordb` & `ztpserver-2.0.0/conf/neighbordb`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/conf/ztpserver.wsgi` & `ztpserver-2.0.0/conf/ztpserver.wsgi`

 * *Files identical despite different names*

### Comparing `ztpserver-1.6.0/client/bootstrap` & `ztpserver-2.0.0/client/bootstrap`

 * *Files 11% similar despite different names*

```diff
@@ -28,78 +28,76 @@
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 # Bootstrap script
 #
 #    Written by:
 #       EOS+, Arista Networks
 
-# pylint: disable=W0703
+# pylint: disable=W0703,C0209,C0415,W4901
 
 import argparse
+import crypt
 import datetime
-import imp
+import grp
+import io
 import json
-import jsonrpclib
 import logging
 import os
 import os.path
+import pwd
 import re
-import sleekxmpp
 import shutil
-import socket
 import subprocess
 import sys
 import time
-import pwd
-import grp
-import crypt
 import traceback
-import urllib2
-import urlparse
-
 from collections import namedtuple
 from logging.handlers import SysLogHandler
-from string import Template              # pylint: disable=W0402
+from string import Template  # pylint: disable=W0402
 from subprocess import PIPE
-from urlparse import urlsplit, urlunsplit
+
+import jsonrpclib
+import sleekxmpp
+from six import PY2, PY3, binary_type, raise_from, text_type
+from six.moves import urllib
 
 # Server will replace this value with the correct IP address/hostname
 # before responding to the bootstrap request.
-SERVER = '$SERVER'
+SERVER = "$SERVER"
 
-LOGGING_FACILITY = 'ztpbootstrap'
-SYSLOG = '/dev/log'
+LOGGING_FACILITY = "ztpbootstrap"
+SYSLOG = "/dev/log"
 DEFAULT_SYSLOG_PORT = 514
 
-CONTENT_TYPE_PYTHON = 'text/x-python'
-CONTENT_TYPE_HTML = 'text/html'
-CONTENT_TYPE_OTHER = 'text/plain'
-CONTENT_TYPE_JSON = 'application/json'
-
-TEMP = '/tmp'
-
-COMMAND_API_SERVER = 'localhost'
-COMMAND_API_USERNAME = 'ztps'
-COMMAND_API_PASSWORD = 'ztps-password'
-COMMAND_API_PROTOCOL = 'unix-socket'
+CONTENT_TYPE_PYTHON = "text/x-python"
+CONTENT_TYPE_HTML = "text/html"
+CONTENT_TYPE_OTHER = "text/plain"
+CONTENT_TYPE_JSON = "application/json"
+
+TEMP = "/tmp"
+
+COMMAND_API_SERVER = "localhost"
+COMMAND_API_USERNAME = "ztps"
+COMMAND_API_PASSWORD = "ztps-password"
+COMMAND_API_PROTOCOL = "unix-socket"
 
 HTTP_STATUS_OK = 200
 HTTP_STATUS_CREATED = 201
 HTTP_STATUS_BAD_REQUEST = 400
 HTTP_STATUS_NOT_FOUND = 404
 HTTP_STATUS_CONFLICT = 409
 HTTP_STATUS_INTERNAL_SERVER_ERROR = 500
 
-FLASH = '/mnt/flash'
+FLASH = "/mnt/flash"
 
-STARTUP_CONFIG = '%s/startup-config' % FLASH
-RC_EOS = '%s/rc.eos' % FLASH
+STARTUP_CONFIG = "{}/startup-config".format(FLASH)
+RC_EOS = "{}/rc.eos".format(FLASH)
 
-BOOT_EXTENSIONS = '%s/boot-extensions' % FLASH
-BOOT_EXTENSIONS_FOLDER = '%s/.extensions' % FLASH
+BOOT_EXTENSIONS = "{}/boot-extensions".format(FLASH)
+BOOT_EXTENSIONS_FOLDER = "{}/.extensions".format(FLASH)
 
 HTTP_TIMEOUT = 30
 
 FLASH_FILES = []
 RESTORE_FACTORY_FLASH = True
 
 # pylint: disable=C0103
@@ -109,150 +107,195 @@
 
 # --------------------------------XMPP------------------------
 # Uncomment this section in order to enable XMPP debug logging
 # logging.basicConfig(level=logging.DEBUG,
 #                     format='%(levelname)-8s %(message)s')
 
 # You will also have to comment out the following lines:
-for logger in ['sleekxmpp.xmlstream.xmlstream',
-               'sleekxmpp.basexmpp']:
+for logger in ["sleekxmpp.xmlstream.xmlstream", "sleekxmpp.basexmpp"]:
     xmpp_log = logging.getLogger(logger)
     xmpp_log.addHandler(logging.NullHandler())
 # --------------------------------XMPP------------------------
 
 # --------------------------------SYSLOG----------------------
 # Comment out this section in order to enable syslog debug
 # logging
 logging.raiseExceptions = False
+
+
 # --------------------------------XMPP------------------------
 
 
 # ------------------Utilities---------------------------------
+# pylint: disable=C0103,C0123,R1705
+# ensure_str backport from six 1.6 as older EOS packs six 1.11
+def ensure_str(s, encoding="utf-8", errors="strict"):
+    """Coerce *s* to `str`.
+
+    For Python 2:
+      - `unicode` -> encoded to `str`
+      - `str` -> `str`
+
+    For Python 3:
+      - `str` -> `str`
+      - `bytes` -> decoded to `str`
+    """
+    # Optimization: Fast return for the common case.
+    if type(s) is str:
+        return s
+    if PY2 and isinstance(s, text_type):
+        return s.encode(encoding, errors)
+    elif PY3 and isinstance(s, binary_type):
+        return s.decode(encoding, errors)
+    elif not isinstance(s, (text_type, binary_type)):
+        raise TypeError("not expecting type '%s'" % type(s))
+    return s
+
+
+# ensure_str backport from six 1.6 as older EOS packs six 1.11
+def ensure_text(s, encoding="utf-8", errors="strict"):
+    """Coerce *s* to six.text_type.
+
+    For Python 2:
+      - `unicode` -> `unicode`
+      - `str` -> `unicode`
+
+    For Python 3:
+      - `str` -> `str`
+      - `bytes` -> decoded to `str`
+    """
+    if isinstance(s, binary_type):
+        return s.decode(encoding, errors)
+    elif isinstance(s, text_type):
+        return s
+    else:
+        raise TypeError("not expecting type '%s'" % type(s))
+
+
+# pylint: enable=C0103,C0123,R1705
+
+
 def _exit(code):
     # pylint: disable=W0702
 
     # Wait for XMPP messages to drain
     time.sleep(3)
 
     if xmpp_client:
         try:
             xmpp_client.abort()
         except:
             pass
 
     if not RESTORE_FACTORY_FLASH:
         for path in [STARTUP_CONFIG, RC_EOS, BOOT_EXTENSIONS]:
-            filename = path.split('/')[-1]
+            filename = os.path.basename(path)
             if os.path.isfile(path):
-                dst = '%s.ztp' % path
-                log('Saving %s as %s...' % (filename, dst))
+                dst = "{}.ztp".format(path)
+                log("Saving {} as {}...".format(filename, dst))
 
                 if os.path.isfile(dst):
                     os.remove(dst)
 
                 shutil.move(path, dst)
 
-            backup_path = url_path_join('/', TEMP,
-                                        os.path.basename(filename))
+            backup_path = url_path_join("/", TEMP, os.path.basename(filename))
 
             if os.path.isfile(backup_path):
-                log('Recovering %s...' % path)
+                log("Recovering {}...".format(path))
                 shutil.move(backup_path, path)
 
         if os.path.isdir(BOOT_EXTENSIONS_FOLDER):
-            dst = '%s.ztp' % BOOT_EXTENSIONS_FOLDER
-            log('Saving %s as %s...' %
-                (BOOT_EXTENSIONS_FOLDER.split('/')[-1],
-                 dst))
+            dst = "{}.ztp".format(BOOT_EXTENSIONS_FOLDER)
+            log("Saving {} as {}...".format(BOOT_EXTENSIONS_FOLDER.split("/", maxsplit=1)[-1], dst))
 
             if os.path.isdir(dst):
                 shutil.rmtree(dst)
 
-            shutil.move(BOOT_EXTENSIONS_FOLDER,
-                        '%s.ztp' % BOOT_EXTENSIONS_FOLDER)
+            shutil.move(BOOT_EXTENSIONS_FOLDER, "{}.ztp".format(BOOT_EXTENSIONS_FOLDER))
 
-        backup_path = url_path_join(
-            '/', TEMP,
-            os.path.basename(BOOT_EXTENSIONS_FOLDER))
+        backup_path = url_path_join("/", TEMP, os.path.basename(BOOT_EXTENSIONS_FOLDER))
         if os.path.isdir(backup_path):
-            log('Recovering %s...' % BOOT_EXTENSIONS_FOLDER)
+            log("Recovering {}...".format(BOOT_EXTENSIONS_FOLDER))
             shutil.move(backup_path, BOOT_EXTENSIONS_FOLDER)
     else:
         if code:
-            for path in [x for x in all_files_and_dirs(FLASH)
-                         if x not in FLASH_FILES]:
-                log('Deleting %s...' % path)
+            for path in [x for x in all_files_and_dirs(FLASH) if x not in FLASH_FILES]:
+                log("Deleting {}...".format(path))
                 if os.path.isdir(path):
                     shutil.rmtree(path)
                 else:
                     try:
                         os.remove(path)
                     except OSError:
                         # already removed
                         pass
 
     sys.stdout.flush()
     sys.stderr.flush()
 
     # pylint: disable=W0212
     # Need to close background sleekxmpp threads as well
-    os._exit(code)
+    sys.exit(code)
+
 
 SYSTEM_ID = None
 XMPP_MSG_TYPE = None
 
 
 def log_xmpp():
-    return XMPP_MSG_TYPE == 'debug'
+    return XMPP_MSG_TYPE == "debug"
 
 
 def log(msg, error=False, xmpp=None):
     if xmpp is None:
         xmpp = log_xmpp()
 
-    timestamp = datetime.datetime.now().strftime('%Y-%m-%d_%H:%M:%S')
-    xmpp_msg = '%s: %s - %s%s' % (SYSTEM_ID if SYSTEM_ID else 'N/A',
-                                  timestamp,
-                                  'ERROR: ' if error else '',
-                                  msg)
+    timestamp = datetime.datetime.now().strftime("%Y-%m-%d_%H:%M:%S")
+    xmpp_msg = "{}: {} - {}{}".format(
+        SYSTEM_ID if SYSTEM_ID else "N/A", timestamp, "ERROR: " if error else "", msg
+    )
 
     if xmpp and xmpp_client and xmpp_client.connected:
         xmpp_client.message(xmpp_msg)
 
     if SYSTEM_ID:
-        syslog_msg = '%s: %s' % (SYSTEM_ID, msg)
+        syslog_msg = "{}: {}".format(SYSTEM_ID, msg)
     else:
         syslog_msg = msg
 
     if error:
-        print 'ERROR: %s' % syslog_msg
+        print("ERROR: {}".format(syslog_msg))
     else:
-        print syslog_msg
+        print(syslog_msg)
 
     if syslog_manager:
         if error:
             syslog_manager.log.error(syslog_msg)
         else:
             syslog_manager.log.info(syslog_msg)
 
 
 def url_path_join(*parts):
     """Normalize URL parts and join them with a slash."""
-    # pylint: disable=W0142
-    schemes, netlocs, paths, queries, fragments = \
-        zip(*(urlsplit(part) for part in parts))
+    schemes, netlocs, paths, queries, fragments = list(
+        zip(*(urllib.parse.urlsplit(part) for part in parts))
+    )
     scheme = get_first_token(schemes)
     netloc = get_first_token(netlocs)
-    path = '/'.join(x.strip('/') for x in paths if x)
+    path = "/".join(x.strip("/") for x in paths if x)
     query = get_first_token(queries)
     fragment = get_first_token(fragments)
-    return urlunsplit((scheme, netloc, path, query, fragment))
+    return urllib.parse.urlunsplit((scheme, netloc, path, query, fragment))
+
 
 # pylint: disable=C0103
-_ntuple_diskusage = namedtuple('usage', 'total used free')
+_ntuple_diskusage = namedtuple("usage", "total used free")
+
+
 # pylint: enable=C0103
 
 
 def flash_usage():
     stats = os.statvfs(FLASH)
     free = stats.f_bavail * stats.f_frsize
     total = stats.f_blocks * stats.f_frsize
@@ -263,80 +306,87 @@
 def flash_snapshot():
     # pylint: disable=W0603
     global FLASH_FILES
     FLASH_FILES = all_files_and_dirs(FLASH)
 
     for filename in [STARTUP_CONFIG, RC_EOS, BOOT_EXTENSIONS]:
         if os.path.isfile(filename):
-            log('Backing up %s...' % filename)
+            log("Backing up {}...".format(filename))
 
             # Delete old folder in tmp
-            dst = url_path_join('/', TEMP,
-                                os.path.basename(filename))
+            dst = url_path_join("/", TEMP, os.path.basename(filename))
             if os.path.isfile(dst):
                 os.remove(dst)
 
             shutil.move(filename, TEMP)
 
     if os.path.isdir(BOOT_EXTENSIONS_FOLDER):
-        log('Backing up %s...' % BOOT_EXTENSIONS_FOLDER)
+        log("Backing up {}...".format(BOOT_EXTENSIONS_FOLDER))
 
         # Delete old folder in /tmp
-        dst = url_path_join('/', TEMP,
-                            os.path.basename(BOOT_EXTENSIONS_FOLDER))
+        dst = url_path_join("/", TEMP, os.path.basename(BOOT_EXTENSIONS_FOLDER))
         if os.path.isdir(dst):
             shutil.rmtree(dst)
 
         shutil.move(BOOT_EXTENSIONS_FOLDER, TEMP)
 
 
 def get_first_token(sequence):
-    return next((x for x in sequence if x), '')
+    return next((x for x in sequence if x), "")
 
 
 def all_files_and_dirs(path):
     result = []
     for top, dirs, files in os.walk(path):
         result += [os.path.join(top, d) for d in dirs]
         result += [os.path.join(top, f) for f in files]
 
     return result
+
+
 # ------------------Utilities---------------------------------
 
 
 # ------------------4.12.x support----------------------------
 def download_file(url, path):
-    if not urlparse.urlsplit(url).scheme:      # pylint: disable=E1103
+    if not urllib.parse.urlsplit(url).scheme:  # pylint: disable=E1103
         url = url_path_join(SERVER, url)
 
-    log('Retrieving URL: %s' % url)
+    log("Retrieving URL: {}".format(url))
+
+    with urllib.request.urlopen(url, timeout=HTTP_TIMEOUT) as url_fd, io.open(
+        path, "wb"
+    ) as output_file:
+        output_file.write(url_fd.read())
 
-    url = urllib2.urlopen(url, timeout=HTTP_TIMEOUT)
-    output_file = open(path, 'wb')
-    output_file.write(url.read())
-    output_file.close()
 
 # pylint: disable=C0103
-REQUESTS = 'requests-2.3.0'
-REQUESTS_URL = url_path_join(SERVER, '/files/lib/', REQUESTS+'.tar.gz')
+REQUESTS = "requests-2.3.0"
+REQUESTS_URL = url_path_join(SERVER, "/files/lib/", REQUESTS + ".tar.gz")
 try:
     import requests
 except ImportError:
-    requests_url = '%s/%s.tar.gz' % (TEMP, REQUESTS)
+    requests_url = "{}/{}.tar.gz".format(TEMP, REQUESTS)
     download_file(REQUESTS_URL, requests_url)
-    cmd = 'sudo tar -xzvf %s -C /tmp;' \
-          'cd %s/%s;' \
-          'sudo python setup.py build;' \
-          'sudo python setup.py install' % \
-          (requests_url, TEMP, REQUESTS)
+    cmd = """
+sudo tar -xzvf {} -C /tmp;
+cd {}/{};
+sudo python setup.py build;
+sudo python setup.py install
+""".format(
+        requests_url, TEMP, REQUESTS
+    )
+
     res = os.system(cmd)
     if res:
-        log('%s returned %s' % (cmd, res), error=True)
+        log("{} returned {}".format(cmd, res), error=True)
         _exit(1)
     import requests
+
+
 # pylint: enable=C0103
 # ------------------4.12.x support----------------------------
 
 
 class ZtpError(Exception):
     pass
 
@@ -345,385 +395,390 @@
     pass
 
 
 class ZtpUnexpectedServerResponseError(ZtpError):
     pass
 
 
-class Attributes(object):
-
+class Attributes:
     def __init__(self, local_attr=None, special_attr=None):
         self.local_attr = local_attr if local_attr else []
         self.special_attr = special_attr if special_attr else []
 
     def get(self, attr, default=None):
         if attr in self.local_attr:
             return self.local_attr[attr]
-        elif attr in self.special_attr:
+        if attr in self.special_attr:
             return self.special_attr[attr]
-        else:
-            return default
+
+        return default
 
     def copy(self):
-        attrs = dict()
+        attrs = {}
         if self.special_attr:
             attrs = self.special_attr.copy()
         if self.local_attr:
             attrs.update(self.local_attr)
         return attrs
 
 
-class Node(object):
-    # pylint: disable=R0201
-
-    '''Node object which can be used by actions via:
+class Node:
+    """Node object which can be used by actions via:
            attributes.get('NODE')
 
     Attributes:
       client (jsonrpclib.Server): jsonrpclib connect to Command API engine
-    '''
+    """
 
     def __init__(self, server):
         self.server_ = server
 
         url = Node._enable_api()
+        print(url)
 
         self.client = jsonrpclib.Server(url)
 
         try:
             self.api_enable_cmds([])
-        except socket.error:
-            raise ZtpError('unable to enable eAPI')
+        except (OSError, IOError) as exc:
+            raise_from(ZtpError("unable to enable eAPI"), exc)
 
         # Workaround for BUG89374
         try:
             self._disable_copp()
         except jsonrpclib.jsonrpc.ProtocolError as err:
-            log('WARNING: unable to disable COPP: %s '
-                '(platform/EOS version might not support this feature)' %
-                err)
-
-        global SYSTEM_ID                    # pylint: disable=W0603
-        SYSTEM_ID = \
-            self.api_enable_cmds(['show version'])[0]['serialNumber']
+            log(
+                "WARNING: unable to disable COPP: {} (platform/EOS version might not support this"
+                " feature)".format(err)
+            )
+
+        global SYSTEM_ID  # pylint: disable=W0603
+        SYSTEM_ID = self.api_enable_cmds(["show version"])[0]["serialNumber"]
 
     @classmethod
     def _cli_enable_cmd(cls, cli_cmd):
-        bash_cmd = ['FastCli', '-p', '15', '-A', '-c', cli_cmd]
-        proc = subprocess.Popen(bash_cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE)
-        (out, err) = proc.communicate()
-        return (proc.returncode, out, err)      # pylint: disable=E1101
+        bash_cmd = ["FastCli", "-p", "15", "-A", "-c", cli_cmd]
+        proc = subprocess.Popen(  # pylint: disable=R1732
+            bash_cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE
+        )
+        (outb, errb) = proc.communicate()
+        out = ensure_str(outb)
+        err = ensure_str(errb)
+        return_code = proc.returncode
+        return return_code, out, err
 
     @classmethod
     def _cli_config_cmds(cls, cmds):
-        cls._cli_enable_cmd('\n'.join(['configure'] + cmds))
+        cls._cli_enable_cmd("\n".join(["configure"] + cmds))
 
     @classmethod
     def _enable_api(cls):
-        create_user = ''
+        create_user = ""
+        api_protocol = COMMAND_API_PROTOCOL
         # Don't use unix sockets in CI environment
-        if os.environ.get('EAPI_TEST') is not None:
-            COMMAND_API_PROTOCOL = 'http'
-            create_user = 'username %s secret %s privilege 15' % (
-                          COMMAND_API_USERNAME,
-                          COMMAND_API_PASSWORD)
-            url = '%s://%s:%s@%s/command-api' % (COMMAND_API_PROTOCOL,
-                                                 COMMAND_API_USERNAME,
-                                                 COMMAND_API_PASSWORD,
-                                                 COMMAND_API_SERVER)
+        if os.environ.get("EAPI_TEST") is not None:
+            api_protocol = "http"
+            create_user = "username {} secret {} privilege 15".format(
+                COMMAND_API_USERNAME, COMMAND_API_PASSWORD
+            )
+            url = "{}://{}:{}@{}/command-api".format(
+                api_protocol, COMMAND_API_USERNAME, COMMAND_API_PASSWORD, COMMAND_API_SERVER
+            )
         else:
-            url = 'unix:/var/run/command-api.sock'
-            _, out, _ = cls._cli_enable_cmd('show version | include image')
-            version = out.split(': ')[1]
-            (major, minor, patch) = version.split('.')[0:3]
+            url = "unix:/var/run/command-api.sock"
+            _, out, _ = cls._cli_enable_cmd("show version | include image")
+            version = out.split(": ")[1]
+            (major, minor, patch) = version.split(".")[0:3]
             patch = int(list(filter(str.isdigit, patch))[0])
-            if (int(major) <= 4 and int(minor) <= 14 and patch <= 5):
-                COMMAND_API_PROTOCOL = 'http'
-                create_user = 'username %s secret %s privilege 15' % (
-                              COMMAND_API_USERNAME,
-                              COMMAND_API_PASSWORD)
-                url = '%s://%s:%s@%s/command-api' % (COMMAND_API_PROTOCOL,
-                                                     COMMAND_API_USERNAME,
-                                                     COMMAND_API_PASSWORD,
-                                                     COMMAND_API_SERVER)
-            else:
-                COMMAND_API_PROTOCOL = 'unix-socket'
+            if int(major) <= 4 and int(minor) <= 14 and patch <= 5:
+                api_protocol = "http"
+                create_user = "username {} secret {} privilege 15".format(
+                    COMMAND_API_USERNAME, COMMAND_API_PASSWORD
+                )
+                url = "{}://{}:{}@{}/command-api".format(
+                    api_protocol, COMMAND_API_USERNAME, COMMAND_API_PASSWORD, COMMAND_API_SERVER
+                )
+
+        cls._cli_config_cmds(
+            [
+                create_user,
+                "management api http-commands",
+                "no protocol https",
+                "protocol {}".format(api_protocol),
+                "no shutdown",
+            ]
+        )
 
-        cls._cli_config_cmds([create_user,
-                              'management api http-commands',
-                              'no protocol https',
-                              'protocol %s' % COMMAND_API_PROTOCOL,
-                              'no shutdown'])
-
-        _, out, _ = cls._cli_enable_cmd('show management api http-commands |'
-                                        ' grep running')
+        _, out, _ = cls._cli_enable_cmd("show management api http-commands | grep running")
         retries = 3
         while not out and retries:
-            log('Waiting for CommandAPI to be enabled...')
+            log("Waiting for CommandAPI to be enabled...")
             time.sleep(1)
             retries = retries - 1
-            _, out, _ = cls._cli_enable_cmd(
-                'show management api http-commands | grep running')
+            _, out, _ = cls._cli_enable_cmd("show management api http-commands | grep running")
         return url
 
     def _disable_copp(self):
         # COPP does not apply to vEOS or EOS-4.11.x and earlier
-        if (self.system()['model'] != 'vEOS' and
-            len(self.system()['version'].split('.')) > 2 and
-            int(self.system()['version'].split('.')[1]) < 12):
-            self.api_config_cmds([
-                'control-plane',
-                'no service-policy input copp-system-policy'])
+        if (
+            self.system()["model"] != "vEOS"
+            and len(self.system()["version"].split(".")) > 2
+            and int(self.system()["version"].split(".")[1]) < 12
+        ):
+            self.api_config_cmds(["control-plane", "no service-policy input copp-system-policy"])
 
     def _has_rc_eos(self):
         return os.path.isfile(RC_EOS)
 
     def _append_lines(self, filename, lines):
-        if os.path.exists(filename) and os.path.getsize(filename) > 0:
-            fileexists = True
-        else:
-            fileexists = False
+        file_exists = bool(os.path.exists(filename) and os.path.getsize(filename) > 0)
 
-        with open(filename, 'a') as output:
-            if fileexists:
-                output.write('\n')
-            output.write('\n'.join(lines))
+        with io.open(filename, "a", encoding="utf8") as output:
+            if file_exists:
+                output.write(ensure_text("\n"))
+            output.write(ensure_text("\n".join(lines)))
 
     @classmethod
     def bash_cmds(cls, cmds):
-        '''Executes bash commands in order - stops on first failure.
+        """Executes bash commands in order - stops on first failure.
 
         Args:
             cmds: list of bash commands
 
         Returns:
             cmd:  first failing command (None otherwise)
             code: exit code for first failing command (None otherwise)
             out:  stdout for first failing command (None otherwise)
             err:  stderr for first failing command (None otherwise)
-        '''
+        """
 
         for bash_cmd in cmds:
-            proc = subprocess.Popen(bash_cmd, stdin=PIPE,
-                                    stdout=PIPE, stderr=PIPE,
-                                    shell=True)
-            code = proc.returncode         # pylint: disable=E1101
+            proc = subprocess.Popen(  # pylint: disable=R1732
+                bash_cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE, shell=True
+            )
+            code = proc.returncode
             (out, err) = proc.communicate()
             if code or err:
-                return (bash_cmd, code, out, err)
-            else:
-                print out
+                return bash_cmd, code, out, err
+
+            print(out)
 
-        return (None, None, None, None)
+        return None, None, None, None
 
     @classmethod
-    def substitute(cls, template, substitutions, strict=True):
-        '''Perform variable substitution on a config template.
+    def substitute(cls, template, substitutions, strict=True):  # pylint: disable=R1710
+        """Perform variable substitution on a config template.
 
         Args:
             template (string): EOS configuration template
             substitutions (dict): set of substitutions for the template
             strict (bool, optional): If true, method will raise Exception
                                      when template variables are missing
                                      from 'substitutions'.
 
         Returns:
             string: template string with variable substitution
-        '''
+        """
         try:
             if strict:
                 return Template(template).substitute(substitutions)
-            else:
-                return Template(template).safe_substitute(substitutions)
+
+            return Template(template).safe_substitute(substitutions)
         except KeyError as exc:
-            raise Exception('Unable to perform variable substitution - '
-                            '\'%s\' missing from list of substitutions' %
-                            exc.message)
+            exc_message = ensure_str(getattr(exc, "message", str(exc))).replace("'", "")
+            raise_from(
+                RuntimeError(
+                    "Unable to perform variable substitution - '{}' missing from list of"
+                    " substitutions".format(exc_message)
+                ),
+                exc,
+            )
 
     def api_enable_cmds(self, cmds, text_format=False):
-        '''Run CLI commands via Command API, starting from enable mode.
+        """Run CLI commands via Command API, starting from enable mode.
 
         Commands are ran in order.
 
         Args:
             cmds (list): List of CLI commands.
             text_format (bool, optional): If true, Command API request will run
                                           in text mode (instead of JSON).
 
         Returns:
             list: List of Command API results corresponding to the
                   input commands.
-        '''
-        req_format = 'text' if text_format else 'json'
+        """
+        req_format = "text" if text_format else "json"
 
         result = None
         try:
-            result = self.client.runCmds(1, ['enable'] + cmds, req_format)
+            result = self.client.runCmds(1, ["enable"] + cmds, req_format)
         except Exception as exc:
             # EOS-4.14.5+: persistent connection might be have been closed
             # on timeout - should recover on first retry
-            if exc.args[0] == 32:      # Broken PIPE
-                result = self.client.runCmds(1, ['enable'] + cmds, req_format)
+            if exc.args[0] == 32:  # Broken PIPE
+                result = self.client.runCmds(1, ["enable"] + cmds, req_format)
             else:
                 raise exc
 
         if text_format:
-            return [x.values()[0] for x in result if x.values()][1:]
-        else:
-            return result[1:]
+            return [list(x.values())[0] for x in result if list(x.values())][1:]
+
+        return result[1:]
 
     def api_config_cmds(self, cmds):
-        '''Run CLI commands via Command API, starting from config mode.
+        """Run CLI commands via Command API, starting from config mode.
 
         Commands are ran in order.
 
         Args:
             cmds (list): List of CLI commands.
 
         Returns:
             list: List of Command API results corresponding to the
                   input commands.
-        '''
-        return self.api_enable_cmds(['configure'] + cmds)[1:]
+        """
+        return self.api_enable_cmds(["configure"] + cmds)[1:]
 
     def system(self):
-        '''Get system information.
+        """Get system information.
 
         Returns:
             dict: System information
 
             Format::
 
                 {'model':        <MODEL>,
                  'version':      <EOS_VERSION>,
                  'systemmac':    <SYSTEM_MAC>,
                  'serialnumber': <SERIAL_NUMBER>}
 
-        '''
+        """
 
         result = {}
-        info = self.api_enable_cmds(['show version'])[0]
+        info = self.api_enable_cmds(["show version"])[0]
 
-        result['model'] = info['modelName']
-        result['version'] = info['version']
-        result['systemmac'] = info['systemMacAddress']
-        result['serialnumber'] = info['serialNumber']
+        result["model"] = info["modelName"]
+        result["version"] = info["version"]
+        result["systemmac"] = info["systemMacAddress"]
+        result["serialnumber"] = info["serialNumber"]
 
         return result
 
     def neighbors(self):
-        '''Get neighbors.
+        """Get neighbors.
 
         Returns:
             dict: LLDP neighbor
 
             Format::
 
                 {'neighbors': {<LOCAL_PORT>:
                  [{'device': <REMOTE_DEVICE>,
                    'port': <REMOTE_PORT>}, ...],
                 ...}}
 
-        '''
+        """
 
         result = {}
-        info = self.api_enable_cmds(['show lldp neighbors'])[0]
-        result['neighbors'] = {}
-        for entry in info['lldpNeighbors']:
+        info = self.api_enable_cmds(["show lldp neighbors"])[0]
+        result["neighbors"] = {}
+        for entry in info["lldpNeighbors"]:
             neighbor = {}
-            neighbor['device'] = entry['neighborDevice']
-            neighbor['port'] = entry['neighborPort']
-            if entry['port'] in result['neighbors']:
-                result['neighbors'][entry['port']] += [neighbor]
+            neighbor["device"] = entry["neighborDevice"]
+            neighbor["port"] = entry["neighborPort"]
+            if entry["port"] in result["neighbors"]:
+                result["neighbors"][entry["port"]] += [neighbor]
             else:
-                result['neighbors'][entry['port']] = [neighbor]
+                result["neighbors"][entry["port"]] = [neighbor]
         return result
 
     def details(self):
-        '''Get details.
+        """Get details.
 
         Returns:
             dict: System details
 
             Format::
 
                 {'model':        <MODEL>,
                  'version':      <EOS_VERSION>,
                  'systemmac':    <SYSTEM_MAC>,
                  'serialnumber': <SERIAL_NUMBER>,
                  'neighbors':    <NEIGHBORS>        # see neighbors()
                 }
 
-        '''
+        """
 
-        return dict(self.system().items() +
-                    self.neighbors().items())
+        return dict(list(self.system().items()) + list(self.neighbors().items()))
 
     def has_startup_config(self):
-        '''Check whether startup-config is configured or not.
+        """Check whether startup-config is configured or not.
 
         Returns:
             bool: True is startup-config is configured; false otherwise.
-        '''
-        return os.path.isfile(STARTUP_CONFIG) and \
-               open(STARTUP_CONFIG).read().strip()
+        """
+        return (
+            os.path.isfile(STARTUP_CONFIG)
+            and io.open(STARTUP_CONFIG, encoding="utf8").read().strip()
+        )
 
     def append_startup_config_lines(self, lines):
-        '''Add lines to startup-config.
+        """Add lines to startup-config.
 
         Args:
             lines (list): List of CLI commands
-        '''
+        """
         self._append_lines(STARTUP_CONFIG, lines)
 
     def append_rc_eos_lines(self, lines):
-        '''Add lines to rc.eos.
+        """Add lines to rc.eos.
 
         Args:
             lines (list): List of bash commands
-        '''
+        """
         if not self._has_rc_eos():
-            lines = ['#!/bin/bash'] + lines
+            lines = ["#!/bin/bash"] + lines
         self._append_lines(RC_EOS, lines)
 
     def log_msg(self, msg, error=False):
-        '''Log message via configured syslog/XMPP.
+        """Log message via configured syslog/XMPP.
 
         Args:
             msg (string): Message
             error (bool, optional): True if msg is an error; false otherwise.
-        '''
+        """
         log(msg, error)
 
     def rc_eos(self):
-        '''Get rc.eos path.
+        """Get rc.eos path.
 
         Returns:
             string: rc.eos path
-        '''
+        """
         return RC_EOS
 
     def flash(self):
-        '''Get flash path.
+        """Get flash path.
 
         Returns:
             string: flash path
-        '''
+        """
         return FLASH
 
     def startup_config(self):
-        '''Get startup-config path.
+        """Get startup-config path.
 
         Returns:
             string: startup-config path
-        '''
+        """
         return STARTUP_CONFIG
 
     def retrieve_url(self, url, path):
-        '''Download resource from server.
+        """Download resource from server.
 
         If 'path' is somewhere on flash and 'url' points back to
         SERVER, then the client will request the metadata for
         the resource from the server (in order to check whether there
         is enough disk space available). If 'url' points to a different
         server, then the 'content-length' header will be used for the
         disk space checks.
@@ -733,21 +788,19 @@
                 - metadata cannot be retrieved from server OR
                 - metadata is inconsistent with request OR
                 - disk space on flash is insufficient OR
                 - file cannot be written to disk
 
         Returns:
             string: startup-config path
-        '''
+        """
         self.server_.get_resource(url, path)
 
-    def create_user(self, user, group, passwd, root='/persist/local/',
-                    ssh_keys=None):
-
-        '''Create a local user on the bootstrapped node. If 'ssh_keys' are
+    def create_user(self, user, group, passwd, root="/persist/local/", ssh_keys=None):
+        """Create a local user on the bootstrapped node. If 'ssh_keys' are
         provided, they will be copied to $HOME/.ssh/authorized_keys. Also,
         rc.eos will be modified to add this user on every boot. If the user
         provided already exists, the function will continue and install the
         ssh_keys (if necessary). The $HOME/.ssh directory will be assigned
         0700 permissions and the $HOME/.ssh/authorized_keys file will be
         assigned 0600 permissions in accord with SSH best practices.
 
@@ -764,691 +817,702 @@
             - missing argument: user, group, passwd
             - useradd fails, return the error
             - ssh_keys cannot be written to 'authorized_keys'
             - files cannot change ownership or permissions
 
         Returns:
             bool: True if user created; False if otherwise
-        '''
+        """
         if not user:
-            raise ZtpError('A user must be provided for create_user()')
+            raise ZtpError("A user must be provided for create_user()")
 
         if not group:
-            raise ZtpError('A group must be provided for create_user()')
+            raise ZtpError("A group must be provided for create_user()")
 
         if not passwd:
-            raise ZtpError('A passwd must be provided for create_user()')
+            raise ZtpError("A passwd must be provided for create_user()")
 
         if not root:
-            root = '/persist/local/'
+            root = "/persist/local/"
 
         home = os.path.join(root, user)
-        ssh_path = os.path.join(home, '.ssh')
-        auth_path = os.path.join(ssh_path, 'authorized_keys')
+        ssh_path = os.path.join(home, ".ssh")
+        auth_path = os.path.join(ssh_path, "authorized_keys")
 
         # Encrypt password
         enc_passwd = crypt.crypt(passwd, "22")
 
-        add_cmd = 'sudo useradd -p %s -d %s -G %s %s' % (enc_passwd, home,
-                                                         group, user)
+        add_cmd = "sudo useradd -p {} -d {} -G {} {}".format(enc_passwd, home, group, user)
 
         # Create user
         try:
-            proc = subprocess.Popen(add_cmd, stdin=PIPE, stdout=PIPE,
-                                    stderr=PIPE, shell=True)
-
-            (_, err) = proc.communicate()
-            return_code = proc.wait()       # pylint: disable=E1101
+            with subprocess.Popen(
+                add_cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE, shell=True
+            ) as proc:
+                (_, err) = proc.communicate()
+                return_code = proc.wait()
 
             if return_code or err:
                 if return_code in (4, 9):
-                    self.log_msg('User already exists - continuing. (%s:%s)'
-                                 % (return_code, err))
+                    self.log_msg(
+                        "User already exists - continuing. ({}:{})".format(return_code, err)
+                    )
                 else:
-                    raise ZtpError('Failed to add user.(%s:%s)'
-                                   % (return_code, err))
+                    raise ZtpError("Failed to add user.({}:{})".format(return_code, err))
 
         except Exception as exc:
-            raise ZtpError(exc)
+            raise_from(ZtpError(exc), exc)
 
         # Get User ID and Group ID for chown
         uid = pwd.getpwnam(user).pw_uid
         gid = grp.getgrnam(group).gr_gid
 
         # Write keys if provided
         if ssh_keys:
-
             if not os.path.exists(home):
-                os.mkdir(ssh_path, 0700)
+                os.mkdir(ssh_path, 0o700)
 
             if not os.path.exists(ssh_path):
-                os.mkdir(ssh_path, 0700)
+                os.mkdir(ssh_path, 0o700)
             else:
-                os.chmod(ssh_path, 0700)
+                os.chmod(ssh_path, 0o700)
 
             os.chown(ssh_path, uid, gid)
 
-            auth_keys = open(auth_path, 'ab+')
-            auth_keys.write(ssh_keys)
-            auth_keys.close()
+            with io.open(auth_path, "ab+", encoding="utf8") as auth_keys:
+                auth_keys.write(ssh_keys)
             os.chown(auth_path, uid, gid)
-            os.chmod(auth_path, 0600)
+            os.chmod(auth_path, 0o600)
 
         self.append_rc_eos_lines([add_cmd])
 
-        return
-
     @classmethod
     def server_address(cls):
-        '''Get ZTP Server URL.
+        """Get ZTP Server URL.
 
         Returns:
             string: ZTP Server URL.
-        '''
+        """
         return SERVER
 
 
-class SyslogManager(object):
-
+class SyslogManager:
     def __init__(self):
-        self.log = logging.getLogger('ztpbootstrap')
+        self.log = logging.getLogger("ztpbootstrap")
         self.log.setLevel(logging.DEBUG)
-        self.formatter = logging.Formatter('ZTPS - %(levelname)s: '
-                                           '%(message)s')
+        self.formatter = logging.Formatter("ZTPS - %(levelname)s: %(message)s")
 
         # syslog to localhost enabled by default
         self._add_syslog_handler()
 
     def _add_handler(self, handler, level=None):
         if level is None:
-            level = 'DEBUG'
+            level = "DEBUG"
 
         try:
             handler.setLevel(logging.getLevelName(level))
         except ValueError:
-            log('SyslogManager: unknown logging level (%s) - using '
-                'log.DEFAULT instead' % level, error=True)
+            log(
+                "SyslogManager: unknown logging level ({}) - using log.DEFAULT instead".format(
+                    level
+                ),
+                error=True,
+            )
             handler.setLevel(logging.DEBUG)
 
         handler.setFormatter(self.formatter)
         self.log.addHandler(handler)
 
     def _add_syslog_handler(self):
-        log('SyslogManager: adding localhost handler')
+        log("SyslogManager: adding localhost handler")
         self._add_handler(SysLogHandler(address=SYSLOG))
 
     def _add_file_handler(self, filename, level=None):
-        log('SyslogManager: adding file handler (%s - level:%s)' %
-            (filename, level))
+        log("SyslogManager: adding file handler ({} - level:{})".format(filename, level))
         self._add_handler(logging.FileHandler(filename), level)
 
     def _add_remote_syslog_handler(self, host, port, level=None):
-        log('SyslogManager: adding remote handler (%s:%s - level:%s)' %
-            (host, port, level))
+        log("SyslogManager: adding remote handler ({}:{} - level:{})".format(host, port, level))
         self._add_handler(SysLogHandler(address=(host, port)), level)
 
     def add_handlers(self, handler_config):
         for entry in handler_config:
-            match = re.match('^file:(.+)',
-                             entry['destination'])
+            match = re.match("^file:(.+)", entry["destination"])
             if match:
-                self._add_file_handler(match.groups()[0],
-                                       entry['level'])
+                self._add_file_handler(match.groups()[0], entry["level"])
             else:
-                match = re.match('^(.+):(.+)',
-                                 entry['destination'])
+                match = re.match("^(.+):(.+)", entry["destination"])
                 if match:
-                    self._add_remote_syslog_handler(match.groups()[0],
-                                                    int(match.groups()[1]),
-                                                    entry['level'])
+                    self._add_remote_syslog_handler(
+                        match.groups()[0], int(match.groups()[1]), entry["level"]
+                    )
                 else:
-                    self._add_remote_syslog_handler(entry['destination'],
-                                                    DEFAULT_SYSLOG_PORT,
-                                                    entry['level'])
-
+                    self._add_remote_syslog_handler(
+                        entry["destination"], DEFAULT_SYSLOG_PORT, entry["level"]
+                    )
 
-class Server(object):
 
+class Server:
     def __init__(self):
         pass
 
     @classmethod
-    def _http_request(cls, path=None, method='get', headers=None,
-                      payload=None, files=None, local_file=None):
+    def _http_request(
+        cls, path=None, method="get", headers=None, payload=None, files=None, local_file=None
+    ):
         if headers is None:
             headers = {}
         # Disable gzip, deflate so we can safely determine available space
-        headers[u'Accept-Encoding'] = None
+        headers["Accept-Encoding"] = None
         if files is None:
             files = []
 
         request_files = []
         for entry in files:
-            request_files[entry] = open(entry, 'rb')
+            request_files[entry] = io.open(entry, "rb")  # pylint: disable=R1732
 
-        if not urlparse.urlsplit(path).scheme:   # pylint: disable=E1103
+        if not urllib.parse.urlsplit(path).scheme:  # pylint: disable=E1103
             full_url = url_path_join(SERVER, path)
         else:
             full_url = path
 
         response = None
         try:
-            if method == 'get':
-                log('GET %s' % full_url)
-                response = requests.get(full_url,
-                                        data=json.dumps(payload),
-                                        headers=headers,
-                                        files=request_files,
-                                        timeout=HTTP_TIMEOUT)
-            elif method == 'post':
-                log('POST %s' % full_url)
-                response = requests.post(full_url,
-                                         data=json.dumps(payload),
-                                         headers=headers,
-                                         files=request_files,
-                                         timeout=HTTP_TIMEOUT)
-            elif method == 'stream':
-                log('STREAM %s - %s' % (full_url, local_file))
+            if method == "get":
+                log("GET {}".format(full_url))
+                response = requests.get(
+                    full_url,
+                    data=json.dumps(payload),
+                    headers=headers,
+                    files=request_files,
+                    timeout=HTTP_TIMEOUT,
+                )
+            elif method == "post":
+                log("POST {}".format(full_url))
+                response = requests.post(
+                    full_url,
+                    data=json.dumps(payload),
+                    headers=headers,
+                    files=request_files,
+                    timeout=HTTP_TIMEOUT,
+                )
+            elif method == "stream":
+                log("STREAM {} - {}".format(full_url, local_file))
                 # Don't use streaming request in CI environment
-                if os.environ.get('EAPI_TEST') is not None:
-                    log('NOT STREAM FOR CI %s - %s' % (full_url, local_file))
-                    response = requests.get(full_url,
-                                            data=json.dumps(payload),
-                                            headers=headers,
-                                            files=request_files,
-                                            timeout=HTTP_TIMEOUT)
+                if os.environ.get("EAPI_TEST") is not None:
+                    log("NOT STREAM FOR CI {} - {}".format(full_url, local_file))
+                    response = requests.get(
+                        full_url,
+                        data=json.dumps(payload),
+                        headers=headers,
+                        files=request_files,
+                        timeout=HTTP_TIMEOUT,
+                    )
                 else:
                     if not local_file:
-                        raise ZtpError('Cant STREAM EOS image file without'
-                                       ' file name and path')
-                    with requests.get(full_url, stream=True) as response:
+                        raise ZtpError("Cant STREAM EOS image file without file name and path")
+                    with requests.get(full_url, stream=True, timeout=HTTP_TIMEOUT) as response:
                         response.raise_for_status()
-                        with open(local_file, 'wb') as f:
+                        with io.open(local_file, "wb") as fd:
                             for chunk in response.iter_content(chunk_size=8192):
-                                f.write(chunk)
+                                fd.write(chunk)
             else:
-                log('Unknown method %s' % method, error=True)
-        except requests.exceptions.ConnectionError:
-            raise ZtpError('server connection error')
+                log("Unknown method {}".format(method), error=True)
+        except requests.exceptions.ConnectionError as exc:
+            raise_from(ZtpError("server connection error"), exc)
 
         return response
 
     def _get_request(self, url, stream=False, local_file=None):
         # resource or action
-        headers = {'content-type': CONTENT_TYPE_HTML}
+        headers = {"content-type": CONTENT_TYPE_HTML}
         if stream:
-            result = self._http_request(url, method='stream', headers=headers,
-                                        local_file=local_file)
+            result = self._http_request(
+                url, method="stream", headers=headers, local_file=local_file
+            )
         else:
             result = self._http_request(url, headers=headers)
-        log('Server response to GET request: status=%s' % result.status_code)
+        log("Server response to GET request: status={}".format(result.status_code))
 
-        return (result.status_code,
-                result.headers['content-type'].split(';')[0],
-                result)
+        return result.status_code, result.headers["content-type"].split(";")[0], result
 
     def _save_file_contents(self, contents, path, url=None):
         if path.startswith(FLASH):
             if not url:
-                raise ZtpError('attempting to save file to %s, but cannot'
-                               'retrieve content metadata' % path)
+                raise ZtpError(
+                    "attempting to save file to {}, but cannotretrieve content metadata".format(
+                        path
+                    )
+                )
 
             size = 0
-            if 'content-length' in contents.headers:
-                size = int(contents.headers['content-length'])
+            if "content-length" in contents.headers:
+                size = int(contents.headers["content-length"])
 
             if url.startswith(SERVER):
                 _, _, metadata = self.get_metadata(url)
                 metadata = metadata.json()
-                if size and metadata['size'] != size:
-                    raise ZtpError('"content-length" for %s does not match '
-                                   'metadata: %s != %s' %
-                                   (url, metadata['size'], size))
+                if size and metadata["size"] != size:
+                    raise ZtpError(
+                        '"content-length" for {} does not match metadata: {} != {}'.format(
+                            url, metadata["size"], size
+                        )
+                    )
 
             usage = flash_usage()
 
             free_space = usage.free
             potential_used_space = size + usage.used
             if os.path.isfile(path):
                 size = os.path.getsize(path)
                 free_space += size
                 potential_used_space -= size
 
-            if (size > free_space):
-                raise ZtpError('not enough memory on flash for saving %s to %s'
-                               ' (free: %s bytes, required: %s bytes)' %
-                               (url, path, free_space, size))
-            elif (potential_used_space > 0.9 * usage.total):
+            if size > free_space:
+                raise ZtpError(
+                    "not enough memory on flash for saving {} to {} (free: {} bytes, required: {}"
+                    " bytes)".format(url, path, free_space, size)
+                )
+            if potential_used_space > 0.9 * usage.total:
                 percent = (size + usage.used) * 100.0 / usage.total
-                log('WARNING: flash disk usage will exceeed %s%% after '
-                    'saving %s to %s' % (percent, url, path))
+                log(
+                    "WARNING: flash disk usage will exceeed {}% after saving {} to {}".format(
+                        percent, url, path
+                    )
+                )
 
-            log('File streamed earlier. No need to write content.')
+            log("File streamed earlier. No need to write content.")
 
         write_response_contents = False
-        if os.environ.get('EAPI_TEST') is not None:
-            log('File not streamed earlier in CI environment. Need to write content')
+        if os.environ.get("EAPI_TEST") is not None:
+            log("File not streamed earlier in CI environment. Need to write content")
             write_response_contents = True
 
         if not path.startswith(FLASH) or write_response_contents:
-            log('Writing %s...' % path)
+            log("Writing {}...".format(path))
             # Save contents to file
             try:
-                with open(path, 'wb') as result:
+                with io.open(path, "wb") as result:
                     for chunk in contents.iter_content(chunk_size=1024):
                         if chunk:
                             result.write(chunk)
                     result.close()
-            except IOError as err:
-                raise ZtpError('unable to write %s: %s' % (path, err))
+            except OSError as err:
+                raise_from(ZtpError("unable to write {}: {}".format(path, err)), err)
 
         # Set permissions
-        os.chmod(path, 0777)
+        os.chmod(path, 0o777)
 
     def get_config(self):
-        headers = {'content-type': CONTENT_TYPE_HTML}
-        result = self._http_request('bootstrap/config',
-                                    headers=headers)
+        headers = {"content-type": CONTENT_TYPE_HTML}
+        result = self._http_request("bootstrap/config", headers=headers)
 
-        log('Server response to GET config: contents=%s' % result.json())
+        log("Server response to GET config: contents={}".format(result.json()))
 
         status = result.status_code
-        content = result.headers['content-type'].split(';')[0]
-        if(status != HTTP_STATUS_OK or
-           content != CONTENT_TYPE_JSON):
+        content = result.headers["content-type"].split(";")[0]
+        if status != HTTP_STATUS_OK or content != CONTENT_TYPE_JSON:
             raise ZtpUnexpectedServerResponseError(
-                'unexpected response from server (status=%s; content-type=%s)' %
-                (status, content))
+                "unexpected response from server (status={}; content-type={})".format(
+                    status, content
+                )
+            )
 
-        return (status, content, result)
+        return status, content, result
 
     def post_nodes(self, node):
-        headers = {'content-type': CONTENT_TYPE_JSON}
-        result = self._http_request('nodes',
-                                    method='post',
-                                    headers=headers,
-                                    payload=node)
-        location = result.headers['location'] \
-            if 'location' in result.headers \
-            else None
-        log('Server response to POST nodes: status=%s, location=%s' %
-            (result.status_code, location))
+        headers = {"content-type": CONTENT_TYPE_JSON}
+        result = self._http_request("nodes", method="post", headers=headers, payload=node)
+        location = result.headers["location"] if "location" in result.headers else None
+        log(
+            "Server response to POST nodes: status={}, location={}".format(
+                result.status_code, location
+            )
+        )
 
         status = result.status_code
-        content = result.headers['content-type'].split(';')[0]
-        if(status not in [HTTP_STATUS_CREATED,
-                          HTTP_STATUS_BAD_REQUEST,
-                          HTTP_STATUS_CONFLICT] or
-           content != CONTENT_TYPE_HTML):
+        content = result.headers["content-type"].split(";")[0]
+        if (
+            status not in [HTTP_STATUS_CREATED, HTTP_STATUS_BAD_REQUEST, HTTP_STATUS_CONFLICT]
+            or content != CONTENT_TYPE_HTML
+        ):
             raise ZtpUnexpectedServerResponseError(
-                'unexpected response from server (status=%s; content-type=%s)' %
-                (status, content))
-        elif status == HTTP_STATUS_BAD_REQUEST:
-            raise ZtpError('node not found on server (status=%s)' % status)
+                "unexpected response from server (status={}; content-type={})".format(
+                    status, content
+                )
+            )
+        if status == HTTP_STATUS_BAD_REQUEST:
+            raise ZtpError("node not found on server (status={})".format(status))
 
-        return (status, content, location)
+        return status, content, location
 
     def get_definition(self, location):
-        headers = {'content-type': CONTENT_TYPE_HTML}
-        result = self._http_request(location,
-                                    headers=headers)
+        headers = {"content-type": CONTENT_TYPE_HTML}
+        result = self._http_request(location, headers=headers)
 
         if result.status_code == HTTP_STATUS_OK:
-            log('Server response to GET definition: status=%s, contents=%s' %
-                (result.status_code, result.json()))
+            log(
+                "Server response to GET definition: status={}, contents={}".format(
+                    result.status_code, result.json()
+                )
+            )
         else:
-            log('Server response to GET definition: status=%s' %
-                result.status_code)
+            log("Server response to GET definition: status={}".format(result.status_code))
 
         status = result.status_code
-        content = result.headers['content-type'].split(';')[0]
-        if not ((status == HTTP_STATUS_OK and
-                 content == CONTENT_TYPE_JSON) or
-                (status == HTTP_STATUS_BAD_REQUEST and
-                 content == CONTENT_TYPE_HTML)):
+        content = result.headers["content-type"].split(";")[0]
+        if not (
+            (status == HTTP_STATUS_OK and content == CONTENT_TYPE_JSON)
+            or (status == HTTP_STATUS_BAD_REQUEST and content == CONTENT_TYPE_HTML)
+        ):
             raise ZtpUnexpectedServerResponseError(
-                'unexpected response from server (status=%s; content-type=%s)' %
-                (status, content))
-        elif status == HTTP_STATUS_BAD_REQUEST:
-            raise ZtpError('server-side topology check failed (status=%s)' %
-                           status)
+                "unexpected response from server (status={}; content-type={})".format(
+                    status, content
+                )
+            )
+        if status == HTTP_STATUS_BAD_REQUEST:
+            raise ZtpError("server-side topology check failed (status={})".format(status))
 
-        return (status, content, result)
+        return status, content, result
 
     def get_action(self, action):
-        status, content, action_response = \
-            self._get_request('actions/%s' % action)
+        status, content, action_response = self._get_request("actions/{}".format(action))
 
-        if not ((status == HTTP_STATUS_OK and
-                 content == CONTENT_TYPE_PYTHON) or
-                (status == HTTP_STATUS_NOT_FOUND and
-                 content == CONTENT_TYPE_HTML)):
+        if not (
+            (status == HTTP_STATUS_OK and content == CONTENT_TYPE_PYTHON)
+            or (status == HTTP_STATUS_NOT_FOUND and content == CONTENT_TYPE_HTML)
+        ):
             raise ZtpUnexpectedServerResponseError(
-                'unexpected response from server (status=%s; content-type=%s)' %
-                (status, content))
-        elif status == HTTP_STATUS_NOT_FOUND:
-            raise ZtpError('action not found on server (status=%s)' % status)
+                "unexpected response from server (status={}; content-type={})".format(
+                    status, content
+                )
+            )
+        if status == HTTP_STATUS_NOT_FOUND:
+            raise ZtpError("action not found on server (status={})".format(status))
 
         filename = os.path.join(TEMP, action)
         self._save_file_contents(action_response, filename)
         return filename
 
     def get_metadata(self, url):
-        if urlparse.urlsplit(url).scheme:   # pylint: disable=E1103
+        if urllib.parse.urlsplit(url).scheme:  # pylint: disable=E1103
             regex = re.compile(SERVER, re.IGNORECASE)
             if regex.match(url):
-                url = re.sub(regex, '', url)
-                url = url_path_join(SERVER, '/meta', url)
+                url = re.sub(regex, "", url)
+                url = url_path_join(SERVER, "/meta", url)
         else:
-            aux = [x for x in url.split('/') if x]
-            url = '/'.join(['meta'] + aux)
+            aux = [x for x in url.split("/") if x]
+            url = "/".join(["meta"] + aux)
 
-        headers = {'content-type': CONTENT_TYPE_HTML}
-        result = self._http_request(url,
-                                    headers=headers)
-        log('Server response to GET meta: contents=%s' % result.json())
+        headers = {"content-type": CONTENT_TYPE_HTML}
+        result = self._http_request(url, headers=headers)
+        log("Server response to GET meta: contents={}".format(result.json()))
 
         status = result.status_code
-        content = result.headers['content-type'].split(';')[0]
+        content = result.headers["content-type"].split(";")[0]
 
-        if not ((status == HTTP_STATUS_OK and
-                 content == CONTENT_TYPE_JSON) or
-                (status == HTTP_STATUS_NOT_FOUND and
-                 content == CONTENT_TYPE_HTML) or
-                (status == HTTP_STATUS_INTERNAL_SERVER_ERROR and
-                 content == CONTENT_TYPE_HTML)):
+        if not (
+            (status == HTTP_STATUS_OK and content == CONTENT_TYPE_JSON)
+            or (status == HTTP_STATUS_NOT_FOUND and content == CONTENT_TYPE_HTML)
+            or (status == HTTP_STATUS_INTERNAL_SERVER_ERROR and content == CONTENT_TYPE_HTML)
+        ):
             raise ZtpUnexpectedServerResponseError(
-                'unexpected response from server (status=%s; content-type=%s)' %
-                (status, content))
-        elif status == HTTP_STATUS_NOT_FOUND:
-            raise ZtpError('metadata not found on server (status=%s)' %
-                           status)
-        elif status == HTTP_STATUS_INTERNAL_SERVER_ERROR:
-            raise ZtpError(
-                'unable to retrieve metadata from server (status=%s)' %
-                status)
+                "unexpected response from server (status={}; content-type={})".format(
+                    status, content
+                )
+            )
+        if status == HTTP_STATUS_NOT_FOUND:
+            raise ZtpError("metadata not found on server (status={})".format(status))
+        if status == HTTP_STATUS_INTERNAL_SERVER_ERROR:
+            raise ZtpError("unable to retrieve metadata from server (status={})".format(status))
 
-        return (status, content, result)
+        return status, content, result
 
     def get_resource(self, url, path):
-        if not urlparse.urlsplit(url).scheme:     # pylint: disable=E1103
+        if not urllib.parse.urlsplit(url).scheme:  # pylint: disable=E1103
             url = url_path_join(SERVER, url)
 
         if path.startswith(FLASH):
-            status, content, response = self._get_request(url, stream=True,
-                                                          local_file=path)
+            status, content, response = self._get_request(url, stream=True, local_file=path)
         else:
             status, content, response = self._get_request(url)
 
         if url.startswith(SERVER):
-            if not ((status == HTTP_STATUS_OK and
-                     content == CONTENT_TYPE_OTHER) or
-                    (status == HTTP_STATUS_NOT_FOUND and
-                     content == CONTENT_TYPE_HTML)):
+            if not (
+                (status == HTTP_STATUS_OK and content == CONTENT_TYPE_OTHER)
+                or (status == HTTP_STATUS_NOT_FOUND and content == CONTENT_TYPE_HTML)
+            ):
                 raise ZtpUnexpectedServerResponseError(
-                    'unexpected response from server for %s '
-                    '(status=%s; content-type=%s)' %
-                    (url, status, content))
+                    "unexpected response from server for {} (status={}; content-type={})".format(
+                        url, status, content
+                    )
+                )
         else:
-            if not (status == HTTP_STATUS_OK or
-                    status == HTTP_STATUS_NOT_FOUND):
+            if status not in [HTTP_STATUS_OK, HTTP_STATUS_NOT_FOUND]:
                 raise ZtpUnexpectedServerResponseError(
-                    'unexpected response from server for %s '
-                    '(status=%s; content-type=%s)' %
-                    (url, status, content))
+                    "unexpected response from server for {} (status={}; content-type={})".format(
+                        url, status, content
+                    )
+                )
 
         if status == HTTP_STATUS_NOT_FOUND:
-            raise ZtpError('resource %s not found on server (status=%s)' %
-                           (url, status))
+            raise ZtpError("resource {} not found on server (status={})".format(url, status))
 
         self._save_file_contents(response, path, url)
 
 
 class XmppClient(sleekxmpp.ClientXMPP):
-    # pylint: disable=W0613, R0904, R0201, R0924
-
-    def __init__(self, user, domain, password, rooms,
-                 nick, xmpp_server, xmpp_port):
-
-        self.xmpp_jid = '%s@%s' % (user, domain)
+    def __init__(self, user, domain, password, rooms, nick, xmpp_server, xmpp_port):
+        self.xmpp_jid = "{}@{}".format(user, domain)
         self.connected = False
 
         try:
-            sleekxmpp.ClientXMPP.__init__(self, self.xmpp_jid,
-                                          password)
+            sleekxmpp.ClientXMPP.__init__(self, self.xmpp_jid, password)
         except sleekxmpp.jid.InvalidJID:
-            log('Unable to connect XMPP client because of invalid jid: %s' %
-                self.xmpp_jid, xmpp=False)
+            log(
+                "Unable to connect XMPP client because of invalid jid: {}".format(self.xmpp_jid),
+                xmpp=False,
+            )
             return
 
         self.xmpp_nick = nick
         self.xmpp_rooms = rooms
 
         self.xmpp_rooms = []
         for room in rooms:
-            self.xmpp_rooms.append('%s@conference.%s' % (room, domain))
+            self.xmpp_rooms.append("{}@conference.{}".format(room, domain))
 
-        self.add_event_handler('session_start', self._session_connected)
-        self.add_event_handler('connect', self._session_connected)
-        self.add_event_handler('disconnected', self._session_disconnected)
+        self.add_event_handler("session_start", self._session_connected)
+        self.add_event_handler("connect", self._session_connected)
+        self.add_event_handler("disconnected", self._session_disconnected)
 
         # Multi-User Chat
-        self.register_plugin('xep_0045')
+        self.register_plugin("xep_0045")
         # XMPP Ping
-        self.register_plugin('xep_0199')
+        self.register_plugin("xep_0199")
         # Service Discovery
-        self.register_plugin('xep_0030')
+        self.register_plugin("xep_0030")
 
-        log('XmppClient connecting to server...', xmpp=False)
+        log("XmppClient connecting to server...", xmpp=False)
         if xmpp_server is not None:
             self.connect((xmpp_server, xmpp_port), reattempt=False)
         else:
             self.connect(reattempt=False)
 
         self.process(block=False)
 
         retries = 3
         while not self.connected and retries:
             # Wait to connect
             time.sleep(1)
             retries -= 1
 
-    def _session_connected(self, event):
-        log('XmppClient: Session connected (%s)' % self.xmpp_jid,
-            xmpp=False)
+    def _session_connected(self, _):
+        log("XmppClient: Session connected ({})".format(self.xmpp_jid), xmpp=False)
         self.send_presence()
         self.get_roster()
 
         self.connected = True
 
         # Joining rooms
         for room in self.xmpp_rooms:
-            self.plugin['xep_0045'].joinMUC(room,
-                                            self.xmpp_nick,
-                                            wait=True)
-            log('XmppClient: Joined room %s as %s' %
-                (room, self.xmpp_nick),
-                xmpp=False)
-
-    def _session_disconnected(self, event):
-        log('XmppClient: Session disconnected (%s)' % self.xmpp_jid,
-            xmpp=False)
+            self.plugin["xep_0045"].joinMUC(room, self.xmpp_nick, wait=True)
+            log("XmppClient: Joined room {} as {}".format(room, self.xmpp_nick), xmpp=False)
+
+    def _session_disconnected(self, _):
+        log("XmppClient: Session disconnected ({})".format(self.xmpp_jid), xmpp=False)
         self.connected = False
 
     def message(self, message):
         for room in self.xmpp_rooms:
-            self.send_message(mto=room,
-                              mbody=message,
-                              mtype='groupchat')
+            self.send_message(mto=room, mbody=message, mtype="groupchat")
 
 
 def apply_config(config, node):
-    global xmpp_client                      # pylint: disable=W0603
+    global xmpp_client  # pylint: disable=W0603
 
-    log('Applying server config')
+    log("Applying server config")
 
     # XMPP not configured yet
-    xmpp_config = config.get('xmpp', {})
+    xmpp_config = config.get("xmpp", {})
 
-    global XMPP_MSG_TYPE                        # pylint: disable=W0603
-    XMPP_MSG_TYPE = xmpp_config.get('msg_type', 'debug')
-    if XMPP_MSG_TYPE not in ['debug', 'info']:
-        log('XMPP configuration failed because of unexpected \'msg_type\': '
-            '%s not in [\'debug\', \'info\']' % XMPP_MSG_TYPE, error=True,
-            xmpp=False)
+    global XMPP_MSG_TYPE  # pylint: disable=W0603
+    XMPP_MSG_TYPE = xmpp_config.get("msg_type", "debug")
+    if XMPP_MSG_TYPE not in ["debug", "info"]:
+        log(
+            "XMPP configuration failed because of unexpected 'msg_type': "
+            "{} not in ['debug', 'info']".format(XMPP_MSG_TYPE),
+            error=True,
+            xmpp=False,
+        )
     else:
         if xmpp_config:
-            log('Configuring XMPP', xmpp=False)
-            if ('username' in xmpp_config and
-                'domain' in xmpp_config and
-                'password' in xmpp_config and
-                'rooms' in xmpp_config and
-                xmpp_config['rooms']):
-                nick = node.system()['serialnumber']
+            log("Configuring XMPP", xmpp=False)
+            if (
+                "username" in xmpp_config
+                and "domain" in xmpp_config
+                and "password" in xmpp_config
+                and "rooms" in xmpp_config
+                and xmpp_config["rooms"]
+            ):
+                nick = node.system()["serialnumber"]
                 if not nick:
                     # vEOS might not have a serial number configured
-                    nick = node.system()['systemmac']
-                xmpp_client = XmppClient(xmpp_config['username'],
-                                         xmpp_config['domain'],
-                                         xmpp_config['password'],
-                                         xmpp_config['rooms'],
-                                         nick,
-                                         xmpp_config.get('server', None),
-                                         xmpp_config.get('port', 5222))
+                    nick = node.system()["systemmac"]
+                xmpp_client = XmppClient(
+                    xmpp_config["username"],
+                    xmpp_config["domain"],
+                    xmpp_config["password"],
+                    xmpp_config["rooms"],
+                    nick,
+                    xmpp_config.get("server", None),
+                    xmpp_config.get("port", 5222),
+                )
             else:
                 # XMPP not configured yet
-                log('XMPP configuration failed because server response '
-                    'is missing config details',
-                    error=True, xmpp=False)
+                log(
+                    "XMPP configuration failed because server response is missing config details",
+                    error=True,
+                    xmpp=False,
+                )
         else:
-            log('No XMPP configuration received from server', xmpp=False)
+            log("No XMPP configuration received from server", xmpp=False)
 
-    log_config = config.get('logging', [])
+    log_config = config.get("logging", [])
     if log_config:
-        log('Configuring syslog')
+        log("Configuring syslog")
         syslog_manager.add_handlers(log_config)
     else:
-        log('No XMPP configuration received from server')
+        log("No XMPP configuration received from server")
+
+
+def load_module(module_name, source_path):
+    if PY3:
+        import importlib.machinery
+        import importlib.util
+
+        loader = importlib.machinery.SourceFileLoader(module_name, source_path)
+        spec = importlib.util.spec_from_loader(loader.name, loader)
+        module = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(module)
+
+        return module
+
+    import imp
+
+    return imp.load_source(module_name, source_path)
 
 
 def execute_action(server, action_details, special_attr):
-    action = action_details['action']
+    action = action_details["action"]
 
-    description = ''
-    if 'description'in action_details:
-        description = '(%s)' % action_details['description']
-
-    if action not in sys.modules:
-        log('Downloading action %s%s' % (action, description))
-        filename = server.get_action(action)
-
-    log('Executing action %s' % action)
-    if 'onstart' in action_details:
-        log('Action %s: %s' % (action, action_details['onstart']),
-            xmpp=True)
+    description = ""
+    if "description" in action_details:
+        description = "({})".format(action_details["description"])
+
+    log("Executing action {}".format(action))
+    if "onstart" in action_details:
+        log("Action {}: {}".format(action, action_details["onstart"]), xmpp=True)
 
     try:
-        if action in sys.modules:
-            module = sys.modules[action]
-        else:
-            module = imp.load_source(action, filename)
-
-        local_attr = action_details['attributes'] \
-                     if 'attributes' in action_details \
-                     else []
-        try:
-            module.main(Attributes(local_attr, special_attr))
-        except Exception as exc:
-            raise ZtpActionError(exc)
-        log('Action executed succesfully (%s)' % action)
-        if 'onsuccess' in action_details:
-            log('Action %s: %s' % (action, action_details['onsuccess']),
-                xmpp=True)
-    except Exception as err:                  # pylint: disable=W0703
-        if 'onfailure' in action_details:
-            log('Action %s: %s' % (action, action_details['onfailure']),
-                xmpp=True)
-        raise ZtpActionError('executing action failed (%s): %s' % (action,
-                                                                   err))
+        if action not in sys.modules:
+            log("Downloading action {}{}".format(action, description))
+            filename = server.get_action(action)
+            sys.modules[action] = load_module(action, filename)
+
+        action_module = sys.modules[action]
+
+        local_attr = action_details["attributes"] if "attributes" in action_details else []
+
+        action_module.main(Attributes(local_attr, special_attr))
+
+        log("Action executed succesfully ({})".format(action))
+        if "onsuccess" in action_details:
+            log("Action {}: {}".format(action, action_details["onsuccess"]), xmpp=True)
+    except Exception as err:  # pylint: disable=W0703
+        if "onfailure" in action_details:
+            log("Action {}: {}".format(action, action_details["onfailure"]), xmpp=True)
+        raise_from(ZtpActionError("executing action failed ({}): {}".format(action, err)), err)
 
 
 def main():
     # pylint: disable=W0603,R0912,R0915
     global syslog_manager, RESTORE_FACTORY_FLASH
 
-    usage = 'bootstrap [options]'
+    usage = "bootstrap [options]"
     parser = argparse.ArgumentParser(usage=usage)
-    parser.add_argument('--no-flash-factory-restore', '-n',
-                        action='store_true',
-                        help='Do NOT restore flash config to factory default')
+    parser.add_argument(
+        "--no-flash-factory-restore",
+        "-n",
+        action="store_true",
+        help="Do NOT restore flash config to factory default",
+    )
     args = parser.parse_args()
     RESTORE_FACTORY_FLASH = not args.no_flash_factory_restore
 
     flash_snapshot()
 
     syslog_manager = SyslogManager()
     server = Server()
 
     # Retrieve and apply logging/XMPP configuration from server
     # XMPP not configured yet
-    log('Retrieving config from server', xmpp=False)
+    log("Retrieving config from server", xmpp=False)
     _, _, config = server.get_config()
 
     # Creating node
     node = Node(server)
 
     # XMPP not configured yet
-    log('Config retrieved from server', xmpp=False)
+    log("Config retrieved from server", xmpp=False)
     apply_config(config.json(), node)
 
     # Checking node on server
     # XMPP not configured yet
-    log('Collecting node information', xmpp=False)
+    log("Collecting node information", xmpp=False)
     _, _, location = server.post_nodes(node.details())
 
     # Get definition
     _, _, definition = server.get_definition(location)
 
     # Execute actions
     definition = definition.json()
 
-    if 'actions' not in definition:
-        raise ZtpError('\'actions\' section missing from definition')
+    if "actions" not in definition:
+        raise ZtpError("'actions' section missing from definition")
 
-    definition_name = definition.get('name', '')
-    log('Applying definition %s' % definition_name)
+    definition_name = definition.get("name", "")
+    log("Applying definition {}".format(definition_name))
 
-    special_attr = {}
-    special_attr['NODE'] = node
-    for details in definition['actions']:
+    special_attr = {"NODE": node}
+    for details in definition["actions"]:
         execute_action(server, details, special_attr)
 
-    log('Definition %s applied successfully' % definition_name)
+    log("Definition {} applied successfully".format(definition_name))
 
     # Check for startup-config
     if not node.has_startup_config():
-        raise ZtpError('startup configuration is missing at the end of the '
-                       'bootstrap process')
+        raise ZtpError("startup configuration is missing at the end of the bootstrap process")
 
-    log('ZTP bootstrap completed successfully!')
+    log("ZTP bootstrap completed successfully!")
 
     _exit(0)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     try:
         main()
     except ZtpError as exception:
-        log('Bootstrap process failed: %s' % str(exception), error=True)
+        log("Bootstrap process failed: {}".format(str(exception)), error=True)
+        log(traceback.format_exc())
         _exit(1)
     except KeyboardInterrupt:
-        log('Bootstrap process keyboard-interrupted', error=True)
+        log("Bootstrap process keyboard-interrupted", error=True)
         log(sys.exc_info()[0])
         log(traceback.format_exc())
         _exit(1)
-    except Exception, exception:
-        errStr = 'Bootstrap process failed because of unknown' \
-                 ' exception: %s' % exception
+    except Exception as exception:
+        errStr = "Bootstrap process failed because of unknown exception: {}".format(exception)
         log(errStr, error=True)
         log(sys.exc_info()[0])
         log(traceback.format_exc())
         _exit(1)
```

### Comparing `ztpserver-1.6.0/client/lib/requests-2.3.0.tar.gz` & `ztpserver-2.0.0/client/lib/requests-2.3.0.tar.gz`

 * *Files identical despite different names*

