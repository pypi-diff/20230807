# Comparing `tmp/idem_vmware_alb-0.3.0.tar.gz` & `tmp/idem_vmware_alb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem_vmware_alb-0.3.0.tar", last modified: Mon Jul 17 17:38:52 2023, max compression
+gzip compressed data, was "idem_vmware_alb-0.4.0.tar", last modified: Mon Aug  7 14:01:32 2023, max compression
```

## Comparing `idem_vmware_alb-0.3.0.tar` & `idem_vmware_alb-0.4.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3289 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2236 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/acct/nsx_alb/
--rw-r--r--   0 root         (0) root         (0)     1149 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/acct/nsx_alb/basic_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/cloudspec/customize/
--rw-r--r--   0 root         (0) root         (0)      694 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/cloudspec/customize/nsx_alb.py
--rw-r--r--   0 root         (0) root         (0)     1319 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/
--rw-r--r--   0 root         (0) root         (0)    28941 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/applicationpersistenceprofile.py
--rw-r--r--   0 root         (0) root         (0)   653506 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/applicationprofile.py
--rw-r--r--   0 root         (0) root         (0)   256843 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/cloud.py
--rw-r--r--   0 root         (0) root         (0)   115841 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/healthmonitor.py
--rw-r--r--   0 root         (0) root         (0)    50174 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/networkprofile.py
--rw-r--r--   0 root         (0) root         (0)   147756 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/pool.py
--rw-r--r--   0 root         (0) root         (0)   335167 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/serviceenginegroup.py
--rw-r--r--   0 root         (0) root         (0)    32044 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/sslprofile.py
--rw-r--r--   0 root         (0) root         (0)   455650 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/virtualservice.py
--rw-r--r--   0 root         (0) root         (0)    74157 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/vsvip.py
--rw-r--r--   0 root         (0) root         (0)      283 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/
--rw-r--r--   0 root         (0) root         (0)    20940 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/applicationpersistenceprofile.py
--rw-r--r--   0 root         (0) root         (0)   332037 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/applicationprofile.py
--rw-r--r--   0 root         (0) root         (0)   134347 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/cloud.py
--rw-r--r--   0 root         (0) root         (0)    63671 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/healthmonitor.py
--rw-r--r--   0 root         (0) root         (0)    30893 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/networkprofile.py
--rw-r--r--   0 root         (0) root         (0)    84673 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/pool.py
--rw-r--r--   0 root         (0) root         (0)   185809 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/serviceenginegroup.py
--rw-r--r--   0 root         (0) root         (0)    21142 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/sslprofile.py
--rw-r--r--   0 root         (0) root         (0)   236548 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/virtualservice.py
--rw-r--r--   0 root         (0) root         (0)    42893 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/vsvip.py
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.196908 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/
--rw-r--r--   0 root         (0) root         (0)     3890 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/session.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 17:38:51.000000 idem_vmware_alb-0.3.0/idem_vmware_alb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 17:38:52.200908 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3289 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1623 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-17 17:38:52.000000 idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 17:38:52.204908 idem_vmware_alb-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3007 2023-07-17 17:38:37.000000 idem_vmware_alb-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.514613 idem_vmware_alb-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-08-07 14:01:32.514613 idem_vmware_alb-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb/acct/nsx_alb/
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/acct/nsx_alb/basic_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb/cloudspec/customize/
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/cloudspec/customize/nsx_alb.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.514613 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/
+-rw-r--r--   0 root         (0) root         (0)    28967 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/application_persistence_profile.py
+-rw-r--r--   0 root         (0) root         (0)   653519 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/application_profile.py
+-rw-r--r--   0 root         (0) root         (0)   256843 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/cloud.py
+-rw-r--r--   0 root         (0) root         (0)   115854 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/health_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    50187 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/network_profile.py
+-rw-r--r--   0 root         (0) root         (0)   147756 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/pool.py
+-rw-r--r--   0 root         (0) root         (0)   335193 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/service_engine_group.py
+-rw-r--r--   0 root         (0) root         (0)    32057 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/ssl_profile.py
+-rw-r--r--   0 root         (0) root         (0)   455663 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/virtual_service.py
+-rw-r--r--   0 root         (0) root         (0)    74170 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/vs_vip.py
+-rw-r--r--   0 root         (0) root         (0)      283 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.514613 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.514613 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/
+-rw-r--r--   0 root         (0) root         (0)    20984 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/application_persistence_profile.py
+-rw-r--r--   0 root         (0) root         (0)   332119 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/application_profile.py
+-rw-r--r--   0 root         (0) root         (0)   134347 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/cloud.py
+-rw-r--r--   0 root         (0) root         (0)    63693 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/health_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    30975 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/network_profile.py
+-rw-r--r--   0 root         (0) root         (0)    84673 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/pool.py
+-rw-r--r--   0 root         (0) root         (0)   185913 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/service_engine_group.py
+-rw-r--r--   0 root         (0) root         (0)    21210 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/ssl_profile.py
+-rw-r--r--   0 root         (0) root         (0)   236705 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/virtual_service.py
+-rw-r--r--   0 root         (0) root         (0)    42915 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/vs_vip.py
+-rw-r--r--   0 root         (0) root         (0)      131 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.514613 idem_vmware_alb-0.4.0/idem_vmware_alb/tool/nsx_alb/
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/tool/nsx_alb/session.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/tool/nsx_alb/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/tool/nsx_alb/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-07 14:01:31.000000 idem_vmware_alb-0.4.0/idem_vmware_alb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:01:32.510613 idem_vmware_alb-0.4.0/idem_vmware_alb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-08-07 14:01:32.000000 idem_vmware_alb-0.4.0/idem_vmware_alb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-08-07 14:01:32.000000 idem_vmware_alb-0.4.0/idem_vmware_alb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 14:01:32.000000 idem_vmware_alb-0.4.0/idem_vmware_alb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-08-07 14:01:32.000000 idem_vmware_alb-0.4.0/idem_vmware_alb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-07 14:01:32.000000 idem_vmware_alb-0.4.0/idem_vmware_alb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-07 14:01:32.514613 idem_vmware_alb-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-08-07 14:01:17.000000 idem_vmware_alb-0.4.0/setup.py
```

### Comparing `idem_vmware_alb-0.3.0/LICENSE` & `idem_vmware_alb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/PKG-INFO` & `idem_vmware_alb-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem_vmware_alb
-Version: 0.3.0
+Version: 0.4.0
 Summary: VMware ALB Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-vmware-alb
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-vmware-alb
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-vmware-alb/-/issues
```

### Comparing `idem_vmware_alb-0.3.0/README.rst` & `idem_vmware_alb-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/acct/nsx_alb/basic_auth.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/acct/nsx_alb/basic_auth.py`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/conf.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/conf.py`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/applicationpersistenceprofile.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/application_persistence_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: nsx_alb.alb.applicationpersistenceprofile.get
+                - path: nsx_alb.alb.application_persistence_profile.get
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationpersistenceprofile.get
+            idem exec nsx_alb.alb.application_persistence_profile.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
     get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
@@ -130,29 +130,29 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: nsx_alb.alb.applicationpersistenceprofile.list
+                - path: nsx_alb.alb.application_persistence_profile.list
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationpersistenceprofile.list
+            idem exec nsx_alb.alb.application_persistence_profile.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.applicationpersistenceprofile
+            $ idem describe nsx_alb.alb.application_persistence_profile
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     list = await hub.tool.nsx_alb.session.request(
         ctx,
@@ -278,22 +278,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.applicationpersistenceprofile.present:
+              nsx_alb.alb.application_persistence_profile.present:
                 - persistence_type: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationpersistenceprofile.create persistence_type=value
+            idem exec nsx_alb.alb.application_persistence_profile.create persistence_type=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -330,15 +330,15 @@
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created nsx_alb.alb.applicationpersistenceprofile '{name}'",
+        f"Created nsx_alb.alb.application_persistence_profile '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -447,22 +447,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.applicationpersistenceprofile.present:
+              nsx_alb.alb.application_persistence_profile.present:
                 - persistence_type: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationpersistenceprofile.update persistence_type=value
+            idem exec nsx_alb.alb.application_persistence_profile.update persistence_type=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -508,15 +508,15 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated nsx_alb.alb.applicationpersistenceprofile '{name}'",
+            f"Updated nsx_alb.alb.application_persistence_profile '{name}'",
         )
 
     return result
 
 
 async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
@@ -532,22 +532,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.applicationpersistenceprofile.absent:
+              nsx_alb.alb.application_persistence_profile.absent:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationpersistenceprofile.delete
+            idem exec nsx_alb.alb.application_persistence_profile.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/applicationprofile.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/application_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: nsx_alb.alb.applicationprofile.get
+                - path: nsx_alb.alb.application_profile.get
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationprofile.get
+            idem exec nsx_alb.alb.application_profile.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
     get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
@@ -136,29 +136,29 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: nsx_alb.alb.applicationprofile.list
+                - path: nsx_alb.alb.application_profile.list
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationprofile.list
+            idem exec nsx_alb.alb.application_profile.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.applicationprofile
+            $ idem describe nsx_alb.alb.application_profile
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     list = await hub.tool.nsx_alb.session.request(
         ctx,
@@ -3212,22 +3212,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.applicationprofile.present:
+              nsx_alb.alb.application_profile.present:
                 - type: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationprofile.create type=value
+            idem exec nsx_alb.alb.application_profile.create type=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -3270,15 +3270,15 @@
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created nsx_alb.alb.applicationprofile '{name}'",
+        f"Created nsx_alb.alb.application_profile '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -6315,22 +6315,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.applicationprofile.present:
+              nsx_alb.alb.application_profile.present:
                 - type: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationprofile.update type=value
+            idem exec nsx_alb.alb.application_profile.update type=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -6380,15 +6380,15 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated nsx_alb.alb.applicationprofile '{name}'",
+            f"Updated nsx_alb.alb.application_profile '{name}'",
         )
 
     return result
 
 
 async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
@@ -6404,22 +6404,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.applicationprofile.absent:
+              nsx_alb.alb.application_profile.absent:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.applicationprofile.delete
+            idem exec nsx_alb.alb.application_profile.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/cloud.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/cloud.py`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/healthmonitor.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/health_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: nsx_alb.alb.healthmonitor.get
+                - path: nsx_alb.alb.health_monitor.get
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.healthmonitor.get
+            idem exec nsx_alb.alb.health_monitor.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
     get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
@@ -152,29 +152,29 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: nsx_alb.alb.healthmonitor.list
+                - path: nsx_alb.alb.health_monitor.list
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.healthmonitor.list
+            idem exec nsx_alb.alb.health_monitor.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.healthmonitor
+            $ idem describe nsx_alb.alb.health_monitor
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     list = await hub.tool.nsx_alb.session.request(
         ctx,
@@ -708,22 +708,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.healthmonitor.present:
+              nsx_alb.alb.health_monitor.present:
                 - type: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.healthmonitor.create type=value
+            idem exec nsx_alb.alb.health_monitor.create type=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -782,15 +782,15 @@
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created nsx_alb.alb.healthmonitor '{name}'",
+        f"Created nsx_alb.alb.health_monitor '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -1307,22 +1307,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.healthmonitor.present:
+              nsx_alb.alb.health_monitor.present:
                 - type: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.healthmonitor.update type=value
+            idem exec nsx_alb.alb.health_monitor.update type=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -1388,15 +1388,15 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated nsx_alb.alb.healthmonitor '{name}'",
+            f"Updated nsx_alb.alb.health_monitor '{name}'",
         )
 
     return result
 
 
 async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
@@ -1412,22 +1412,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.healthmonitor.absent:
+              nsx_alb.alb.health_monitor.absent:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.healthmonitor.delete
+            idem exec nsx_alb.alb.health_monitor.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/networkprofile.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/network_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: nsx_alb.alb.networkprofile.get
+                - path: nsx_alb.alb.network_profile.get
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.networkprofile.get
+            idem exec nsx_alb.alb.network_profile.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
     get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
@@ -125,29 +125,29 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: nsx_alb.alb.networkprofile.list
+                - path: nsx_alb.alb.network_profile.list
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.networkprofile.list
+            idem exec nsx_alb.alb.network_profile.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.networkprofile
+            $ idem describe nsx_alb.alb.network_profile
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     list = await hub.tool.nsx_alb.session.request(
         ctx,
@@ -372,22 +372,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.networkprofile.present:
+              nsx_alb.alb.network_profile.present:
                 - profile: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.networkprofile.create profile=value
+            idem exec nsx_alb.alb.network_profile.create profile=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -419,15 +419,15 @@
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created nsx_alb.alb.networkprofile '{name}'",
+        f"Created nsx_alb.alb.network_profile '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -635,22 +635,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.networkprofile.present:
+              nsx_alb.alb.network_profile.present:
                 - profile: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.networkprofile.update profile=value
+            idem exec nsx_alb.alb.network_profile.update profile=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -689,15 +689,15 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated nsx_alb.alb.networkprofile '{name}'",
+            f"Updated nsx_alb.alb.network_profile '{name}'",
         )
 
     return result
 
 
 async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
@@ -713,22 +713,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.networkprofile.absent:
+              nsx_alb.alb.network_profile.absent:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.networkprofile.delete
+            idem exec nsx_alb.alb.network_profile.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/pool.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/pool.py`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/serviceenginegroup.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/service_engine_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,23 +38,23 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: nsx_alb.alb.serviceenginegroup.get
+                - path: nsx_alb.alb.service_engine_group.get
                 - kwargs:
                   resource_id: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.serviceenginegroup.get resource_id=value
+            idem exec nsx_alb.alb.service_engine_group.get resource_id=value
     """
 
     result = dict(comment=[], ret=None, result=True)
 
     get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
@@ -428,29 +428,29 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: nsx_alb.alb.serviceenginegroup.list
+                - path: nsx_alb.alb.service_engine_group.list
                 - kwargs:
                   resource_id: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.serviceenginegroup.list resource_id= value
+            idem exec nsx_alb.alb.service_engine_group.list resource_id= value
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.serviceenginegroup
+            $ idem describe nsx_alb.alb.service_engine_group
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     list = await hub.tool.nsx_alb.session.request(
         ctx,
@@ -1547,22 +1547,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.serviceenginegroup.present:
+              nsx_alb.alb.service_engine_group.present:
                 - name: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.serviceenginegroup.create name=value
+            idem exec nsx_alb.alb.service_engine_group.create name=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -1870,15 +1870,15 @@
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created nsx_alb.alb.serviceenginegroup '{name}'",
+        f"Created nsx_alb.alb.service_engine_group '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -2948,22 +2948,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.serviceenginegroup.present:
+              nsx_alb.alb.service_engine_group.present:
                 - name: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.serviceenginegroup.update name=value
+            idem exec nsx_alb.alb.service_engine_group.update name=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -3278,15 +3278,15 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated nsx_alb.alb.serviceenginegroup '{name}'",
+            f"Updated nsx_alb.alb.service_engine_group '{name}'",
         )
 
     return result
 
 
 async def delete(hub, ctx, name: str = None, resource_id: str = None) -> Dict[str, Any]:
     r"""
@@ -3304,22 +3304,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.serviceenginegroup.absent:
+              nsx_alb.alb.service_engine_group.absent:
                 - resource_id: value
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.serviceenginegroup.delete resource_id=value
+            idem exec nsx_alb.alb.service_engine_group.delete resource_id=value
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/sslprofile.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/ssl_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: nsx_alb.alb.sslprofile.get
+                - path: nsx_alb.alb.ssl_profile.get
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.sslprofile.get
+            idem exec nsx_alb.alb.ssl_profile.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
     get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
@@ -139,29 +139,29 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: nsx_alb.alb.sslprofile.list
+                - path: nsx_alb.alb.ssl_profile.list
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.sslprofile.list
+            idem exec nsx_alb.alb.ssl_profile.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.sslprofile
+            $ idem describe nsx_alb.alb.ssl_profile
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     list = await hub.tool.nsx_alb.session.request(
         ctx,
@@ -267,22 +267,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.sslprofile.present:
+              nsx_alb.alb.ssl_profile.present:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.sslprofile.create
+            idem exec nsx_alb.alb.ssl_profile.create
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -328,15 +328,15 @@
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created nsx_alb.alb.sslprofile '{name}'",
+        f"Created nsx_alb.alb.ssl_profile '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -425,22 +425,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.sslprofile.present:
+              nsx_alb.alb.ssl_profile.present:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.sslprofile.update
+            idem exec nsx_alb.alb.ssl_profile.update
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -493,15 +493,15 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated nsx_alb.alb.sslprofile '{name}'",
+            f"Updated nsx_alb.alb.ssl_profile '{name}'",
         )
 
     return result
 
 
 async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
@@ -517,22 +517,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.sslprofile.absent:
+              nsx_alb.alb.ssl_profile.absent:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.sslprofile.delete
+            idem exec nsx_alb.alb.ssl_profile.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/virtualservice.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/virtual_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: nsx_alb.alb.virtualservice.get
+                - path: nsx_alb.alb.virtual_service.get
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.virtualservice.get
+            idem exec nsx_alb.alb.virtual_service.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
     get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
@@ -216,29 +216,29 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: nsx_alb.alb.virtualservice.list
+                - path: nsx_alb.alb.virtual_service.list
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.virtualservice.list
+            idem exec nsx_alb.alb.virtual_service.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.virtualservice
+            $ idem describe nsx_alb.alb.virtual_service
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     list = await hub.tool.nsx_alb.session.request(
         ctx,
@@ -2612,22 +2612,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.virtualservice.present:
+              nsx_alb.alb.virtual_service.present:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.virtualservice.create
+            idem exec nsx_alb.alb.virtual_service.create
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -2745,15 +2745,15 @@
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created nsx_alb.alb.virtualservice '{name}'",
+        f"Created nsx_alb.alb.virtual_service '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -5110,22 +5110,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.virtualservice.present:
+              nsx_alb.alb.virtual_service.present:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.virtualservice.update
+            idem exec nsx_alb.alb.virtual_service.update
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -5250,15 +5250,15 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated nsx_alb.alb.virtualservice '{name}'",
+            f"Updated nsx_alb.alb.virtual_service '{name}'",
         )
 
     return result
 
 
 async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
@@ -5274,22 +5274,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.virtualservice.absent:
+              nsx_alb.alb.virtual_service.absent:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.virtualservice.delete
+            idem exec nsx_alb.alb.virtual_service.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/exec/nsx_alb/alb/vsvip.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/exec/nsx_alb/alb/vs_vip.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
-                - path: nsx_alb.alb.vsvip.get
+                - path: nsx_alb.alb.vs_vip.get
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.vsvip.get
+            idem exec nsx_alb.alb.vs_vip.get
     """
 
     result = dict(comment=[], ret=None, result=True)
 
     get = await hub.tool.nsx_alb.session.request(
         ctx,
         method="get",
@@ -139,29 +139,29 @@
 
         Unmanaged Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
-                - path: nsx_alb.alb.vsvip.list
+                - path: nsx_alb.alb.vs_vip.list
                 - kwargs:
 
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.vsvip.list
+            idem exec nsx_alb.alb.vs_vip.list
 
         Describe call from the CLI:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.vsvip
+            $ idem describe nsx_alb.alb.vs_vip
 
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     list = await hub.tool.nsx_alb.session.request(
         ctx,
@@ -573,22 +573,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.vsvip.present:
+              nsx_alb.alb.vs_vip.present:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.vsvip.create
+            idem exec nsx_alb.alb.vs_vip.create
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -629,15 +629,15 @@
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(
-        f"Created nsx_alb.alb.vsvip '{name}'",
+        f"Created nsx_alb.alb.vs_vip '{name}'",
     )
 
     result["ret"] = create["ret"]
 
     result["ret"]["resource_id"] = create["ret"]["uuid"]
     return result
 
@@ -1032,22 +1032,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.vsvip.present:
+              nsx_alb.alb.vs_vip.present:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.vsvip.update
+            idem exec nsx_alb.alb.vs_vip.update
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
@@ -1095,15 +1095,15 @@
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["resource_id"] = update["ret"]["uuid"]
         result["comment"].append(
-            f"Updated nsx_alb.alb.vsvip '{name}'",
+            f"Updated nsx_alb.alb.vs_vip '{name}'",
         )
 
     return result
 
 
 async def delete(hub, ctx, resource_id: str, name: str = None) -> Dict[str, Any]:
     r"""
@@ -1119,22 +1119,22 @@
     Examples:
 
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.vsvip.absent:
+              nsx_alb.alb.vs_vip.absent:
                 -
 
         Exec call from the CLI:
 
         .. code-block:: bash
 
-            idem exec nsx_alb.alb.vsvip.delete
+            idem exec nsx_alb.alb.vs_vip.delete
     """
 
     result = dict(comment=[], ret=[], result=True)
 
     delete = await hub.tool.nsx_alb.session.request(
         ctx,
         method="delete",
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/applicationpersistenceprofile.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/application_persistence_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.applicationpersistenceprofile.present:
+              nsx_alb.alb.application_persistence_profile.present:
                 - persistence_type: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
@@ -140,40 +140,40 @@
                 tenant_ref_acct = ctx.acct.get("tenant_ref")
                 desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
 
             if k == "cloud_ref" and v is not None:
                 cloud_ref_acct = ctx.acct.get("cloud_ref")
                 desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
 
-    before = await hub.exec.nsx_alb.alb.applicationpersistenceprofile.get(
+    before = await hub.exec.nsx_alb.alb.application_persistence_profile.get(
         ctx,
         name=name,
     )
     if before["ret"]:
         result["old_state"] = before.ret
         resource_id = before["ret"]["resource_id"]
     else:
         resource_id = None
 
     if resource_id:
-        before = await hub.exec.nsx_alb.alb.applicationpersistenceprofile.get(
+        before = await hub.exec.nsx_alb.alb.application_persistence_profile.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
         result["comment"].append(
-            f"'nsx_alb.alb.applicationpersistenceprofile:{name}' already exists"
+            f"'nsx_alb.alb.application_persistence_profile:{name}' already exists"
         )
 
         # If there are changes in desired state from existing state
         if desired_state:
             desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
                 ctx, data=desired_state
             )
@@ -194,20 +194,20 @@
             if ctx.test:
                 result[
                     "new_state"
                 ] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
                 result["comment"] = (
-                    f"Would update nsx_alb.alb.applicationpersistenceprofile '{name}'",
+                    f"Would update nsx_alb.alb.application_persistence_profile '{name}'",
                 )
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.nsx_alb.alb.applicationpersistenceprofile.update(
+                update_ret = await hub.exec.nsx_alb.alb.application_persistence_profile.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "app_cookie_persistence_profile": app_cookie_persistence_profile,
                         "configpb_attributes": configpb_attributes,
                         "description": description,
@@ -221,29 +221,29 @@
                         "tenant_ref": tenant_ref,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
                     result["comment"].append(
-                        f"Updated 'nsx_alb.alb.applicationpersistenceprofile:{name}'"
+                        f"Updated 'nsx_alb.alb.application_persistence_profile:{name}'"
                     )
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result["new_state"] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
             result["comment"] = (
-                f"Would create nsx_alb.alb.applicationpersistenceprofile {name}",
+                f"Would create nsx_alb.alb.application_persistence_profile {name}",
             )
             return result
         else:
-            create_ret = await hub.exec.nsx_alb.alb.applicationpersistenceprofile.create(
+            create_ret = await hub.exec.nsx_alb.alb.application_persistence_profile.create(
                 ctx,
                 name=name,
                 **{
                     "app_cookie_persistence_profile": app_cookie_persistence_profile,
                     "configpb_attributes": configpb_attributes,
                     "description": description,
                     "hdr_persistence_profile": hdr_persistence_profile,
@@ -256,29 +256,29 @@
                     "tenant_ref": tenant_ref,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
                 result["comment"].append(
-                    f"Created 'nsx_alb.alb.applicationpersistenceprofile:{name}'"
+                    f"Created 'nsx_alb.alb.application_persistence_profile:{name}'"
                 )
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.nsx_alb.alb.applicationpersistenceprofile.get(
+    after = await hub.exec.nsx_alb.alb.application_persistence_profile.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -299,61 +299,61 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.applicationpersistenceprofile.absent:
+              nsx_alb.alb.application_persistence_profile.absent:
                 - resource_id : value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
         result["comment"].append(
-            f"'nsx_alb.alb.applicationpersistenceprofile:{name}' already absent"
+            f"'nsx_alb.alb.application_persistence_profile:{name}' already absent"
         )
         return result
 
-    before = await hub.exec.nsx_alb.alb.applicationpersistenceprofile.get(
+    before = await hub.exec.nsx_alb.alb.application_persistence_profile.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
             result[
                 "comment"
-            ] = f"Would delete nsx_alb.alb.applicationpersistenceprofile:{name}"
+            ] = f"Would delete nsx_alb.alb.application_persistence_profile:{name}"
             return result
 
-        delete_ret = await hub.exec.nsx_alb.alb.applicationpersistenceprofile.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.application_persistence_profile.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
             result["comment"].append(
-                f"Deleted 'nsx_alb.alb.applicationpersistenceprofile:{name}'"
+                f"Deleted 'nsx_alb.alb.application_persistence_profile:{name}'"
             )
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
         result["comment"].append(
-            f"'nsx_alb.alb.applicationpersistenceprofile:{name}' already absent"
+            f"'nsx_alb.alb.application_persistence_profile:{name}' already absent"
         )
         return result
 
     result["old_state"] = before.ret
     return result
 
 
@@ -378,30 +378,30 @@
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.applicationpersistenceprofile
+            $ idem describe nsx_alb.alb.application_persistence_profile
     """
 
     result = {}
 
-    ret = await hub.exec.nsx_alb.alb.applicationpersistenceprofile.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.application_persistence_profile.list(ctx)
 
     if not ret or not ret["result"]:
         hub.log.debug(
-            f"Could not describe nsx_alb.alb.applicationpersistenceprofile {ret['comment']}"
+            f"Could not describe nsx_alb.alb.application_persistence_profile {ret['comment']}"
         )
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "nsx_alb.alb.applicationpersistenceprofile.present": [
+            "nsx_alb.alb.application_persistence_profile.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/applicationprofile.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/application_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -3044,15 +3044,15 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.applicationprofile.present:
+              nsx_alb.alb.application_profile.present:
                 - type: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
@@ -3067,40 +3067,40 @@
                 tenant_ref_acct = ctx.acct.get("tenant_ref")
                 desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
 
             if k == "cloud_ref" and v is not None:
                 cloud_ref_acct = ctx.acct.get("cloud_ref")
                 desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
 
-    before = await hub.exec.nsx_alb.alb.applicationprofile.get(
+    before = await hub.exec.nsx_alb.alb.application_profile.get(
         ctx,
         name=name,
     )
     if before["ret"]:
         result["old_state"] = before.ret
         resource_id = before["ret"]["resource_id"]
     else:
         resource_id = None
 
     if resource_id:
-        before = await hub.exec.nsx_alb.alb.applicationprofile.get(
+        before = await hub.exec.nsx_alb.alb.application_profile.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
         result["comment"].append(
-            f"'nsx_alb.alb.applicationprofile:{name}' already exists"
+            f"'nsx_alb.alb.application_profile:{name}' already exists"
         )
 
         # If there are changes in desired state from existing state
         if desired_state:
             desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
                 ctx, data=desired_state
             )
@@ -3121,20 +3121,20 @@
             if ctx.test:
                 result[
                     "new_state"
                 ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
                 result["comment"] = (
-                    f"Would update nsx_alb.alb.applicationprofile '{name}'",
+                    f"Would update nsx_alb.alb.application_profile '{name}'",
                 )
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.nsx_alb.alb.applicationprofile.update(
+                update_ret = await hub.exec.nsx_alb.alb.application_profile.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "app_service_type": app_service_type,
                         "cloud_config_cksum": cloud_config_cksum,
                         "configpb_attributes": configpb_attributes,
@@ -3154,29 +3154,31 @@
                         "type": type,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
                     result["comment"].append(
-                        f"Updated 'nsx_alb.alb.applicationprofile:{name}'"
+                        f"Updated 'nsx_alb.alb.application_profile:{name}'"
                     )
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result[
                 "new_state"
             ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create nsx_alb.alb.applicationprofile {name}",)
+            result["comment"] = (
+                f"Would create nsx_alb.alb.application_profile {name}",
+            )
             return result
         else:
-            create_ret = await hub.exec.nsx_alb.alb.applicationprofile.create(
+            create_ret = await hub.exec.nsx_alb.alb.application_profile.create(
                 ctx,
                 name=name,
                 **{
                     "app_service_type": app_service_type,
                     "cloud_config_cksum": cloud_config_cksum,
                     "configpb_attributes": configpb_attributes,
                     "created_by": created_by,
@@ -3195,29 +3197,29 @@
                     "type": type,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
                 result["comment"].append(
-                    f"Created 'nsx_alb.alb.applicationprofile:{name}'"
+                    f"Created 'nsx_alb.alb.application_profile:{name}'"
                 )
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.nsx_alb.alb.applicationprofile.get(
+    after = await hub.exec.nsx_alb.alb.application_profile.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -3236,57 +3238,59 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.applicationprofile.absent:
+              nsx_alb.alb.application_profile.absent:
                 -
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
         result["comment"].append(
-            f"'nsx_alb.alb.applicationprofile:{name}' already absent"
+            f"'nsx_alb.alb.application_profile:{name}' already absent"
         )
         return result
 
-    before = await hub.exec.nsx_alb.alb.applicationprofile.get(
+    before = await hub.exec.nsx_alb.alb.application_profile.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete nsx_alb.alb.applicationprofile:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.application_profile:{name}"
             return result
 
-        delete_ret = await hub.exec.nsx_alb.alb.applicationprofile.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.application_profile.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'nsx_alb.alb.applicationprofile:{name}'")
+            result["comment"].append(
+                f"Deleted 'nsx_alb.alb.application_profile:{name}'"
+            )
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
         result["comment"].append(
-            f"'nsx_alb.alb.applicationprofile:{name}' already absent"
+            f"'nsx_alb.alb.application_profile:{name}' already absent"
         )
         return result
 
     result["old_state"] = before.ret
     return result
 
 
@@ -3304,30 +3308,30 @@
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.applicationprofile
+            $ idem describe nsx_alb.alb.application_profile
     """
 
     result = {}
 
-    ret = await hub.exec.nsx_alb.alb.applicationprofile.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.application_profile.list(ctx)
 
     if not ret or not ret["result"]:
         hub.log.debug(
-            f"Could not describe nsx_alb.alb.applicationprofile {ret['comment']}"
+            f"Could not describe nsx_alb.alb.application_profile {ret['comment']}"
         )
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "nsx_alb.alb.applicationprofile.present": [
+            "nsx_alb.alb.application_profile.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/cloud.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/cloud.py`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/healthmonitor.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/health_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,15 +524,15 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.healthmonitor.present:
+              nsx_alb.alb.health_monitor.present:
                 - type: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
@@ -546,39 +546,39 @@
             if k == "tenant_ref" and v is not None:
                 tenant_ref_acct = ctx.acct.get("tenant_ref")
                 desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
             if k == "cloud_ref" and v is not None:
                 cloud_ref_acct = ctx.acct.get("cloud_ref")
                 desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
 
-    before = await hub.exec.nsx_alb.alb.healthmonitor.get(
+    before = await hub.exec.nsx_alb.alb.health_monitor.get(
         ctx,
         name=name,
     )
     if before["ret"]:
         result["old_state"] = before.ret
         resource_id = before["ret"]["resource_id"]
     else:
         resource_id = None
 
     if resource_id:
-        before = await hub.exec.nsx_alb.alb.healthmonitor.get(
+        before = await hub.exec.nsx_alb.alb.health_monitor.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'nsx_alb.alb.healthmonitor:{name}' already exists")
+        result["comment"].append(f"'nsx_alb.alb.health_monitor:{name}' already exists")
 
         # If there are changes in desired state from existing state
         if desired_state:
             desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
                 ctx, data=desired_state
             )
         if desired_state:
@@ -598,20 +598,20 @@
             if ctx.test:
                 result[
                     "new_state"
                 ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
                 result["comment"] = (
-                    f"Would update nsx_alb.alb.healthmonitor '{name}'",
+                    f"Would update nsx_alb.alb.health_monitor '{name}'",
                 )
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.nsx_alb.alb.healthmonitor.update(
+                update_ret = await hub.exec.nsx_alb.alb.health_monitor.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "allow_duplicate_monitors": allow_duplicate_monitors,
                         "authentication": authentication,
                         "configpb_attributes": configpb_attributes,
@@ -647,29 +647,29 @@
                         "udp_monitor": udp_monitor,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
                     result["comment"].append(
-                        f"Updated 'nsx_alb.alb.healthmonitor:{name}'"
+                        f"Updated 'nsx_alb.alb.health_monitor:{name}'"
                     )
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result[
                 "new_state"
             ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create nsx_alb.alb.healthmonitor {name}",)
+            result["comment"] = (f"Would create nsx_alb.alb.health_monitor {name}",)
             return result
         else:
-            create_ret = await hub.exec.nsx_alb.alb.healthmonitor.create(
+            create_ret = await hub.exec.nsx_alb.alb.health_monitor.create(
                 ctx,
                 name=name,
                 **{
                     "allow_duplicate_monitors": allow_duplicate_monitors,
                     "authentication": authentication,
                     "configpb_attributes": configpb_attributes,
                     "description": description,
@@ -703,28 +703,28 @@
                     "type": type,
                     "udp_monitor": udp_monitor,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created 'nsx_alb.alb.healthmonitor:{name}'")
+                result["comment"].append(f"Created 'nsx_alb.alb.health_monitor:{name}'")
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.nsx_alb.alb.healthmonitor.get(
+    after = await hub.exec.nsx_alb.alb.health_monitor.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -743,54 +743,54 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.healthmonitor.absent:
+              nsx_alb.alb.health_monitor.absent:
                 -
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
-        result["comment"].append(f"'nsx_alb.alb.healthmonitor:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.health_monitor:{name}' already absent")
         return result
 
-    before = await hub.exec.nsx_alb.alb.healthmonitor.get(
+    before = await hub.exec.nsx_alb.alb.health_monitor.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete nsx_alb.alb.healthmonitor:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.health_monitor:{name}"
             return result
 
-        delete_ret = await hub.exec.nsx_alb.alb.healthmonitor.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.health_monitor.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'nsx_alb.alb.healthmonitor:{name}'")
+            result["comment"].append(f"Deleted 'nsx_alb.alb.health_monitor:{name}'")
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'nsx_alb.alb.healthmonitor:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.health_monitor:{name}' already absent")
         return result
 
     result["old_state"] = before.ret
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
@@ -807,28 +807,28 @@
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.healthmonitor
+            $ idem describe nsx_alb.alb.health_monitor
     """
 
     result = {}
 
-    ret = await hub.exec.nsx_alb.alb.healthmonitor.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.health_monitor.list(ctx)
 
     if not ret or not ret["result"]:
-        hub.log.debug(f"Could not describe nsx_alb.alb.healthmonitor {ret['comment']}")
+        hub.log.debug(f"Could not describe nsx_alb.alb.health_monitor {ret['comment']}")
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "nsx_alb.alb.healthmonitor.present": [
+            "nsx_alb.alb.health_monitor.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/networkprofile.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/network_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.networkprofile.present:
+              nsx_alb.alb.network_profile.present:
                 - profile: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
@@ -239,39 +239,39 @@
                 tenant_ref_acct = ctx.acct.get("tenant_ref")
                 desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
 
             if k == "cloud_ref" and v is not None:
                 cloud_ref_acct = ctx.acct.get("cloud_ref")
                 desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
 
-    before = await hub.exec.nsx_alb.alb.networkprofile.get(
+    before = await hub.exec.nsx_alb.alb.network_profile.get(
         ctx,
         name=name,
     )
     if before["ret"]:
         result["old_state"] = before.ret
         resource_id = before["ret"]["resource_id"]
     else:
         resource_id = None
 
     if resource_id:
-        before = await hub.exec.nsx_alb.alb.networkprofile.get(
+        before = await hub.exec.nsx_alb.alb.network_profile.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'nsx_alb.alb.networkprofile:{name}' already exists")
+        result["comment"].append(f"'nsx_alb.alb.network_profile:{name}' already exists")
 
         # If there are changes in desired state from existing state
         if desired_state:
             desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
                 ctx, data=desired_state
             )
         if desired_state:
@@ -291,20 +291,20 @@
             if ctx.test:
                 result[
                     "new_state"
                 ] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
                 result["comment"] = (
-                    f"Would update nsx_alb.alb.networkprofile '{name}'",
+                    f"Would update nsx_alb.alb.network_profile '{name}'",
                 )
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.nsx_alb.alb.networkprofile.update(
+                update_ret = await hub.exec.nsx_alb.alb.network_profile.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "configpb_attributes": configpb_attributes,
                         "connection_mirror": connection_mirror,
                         "description": description,
@@ -313,55 +313,57 @@
                         "tenant_ref": tenant_ref,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
                     result["comment"].append(
-                        f"Updated 'nsx_alb.alb.networkprofile:{name}'"
+                        f"Updated 'nsx_alb.alb.network_profile:{name}'"
                     )
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result["new_state"] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create nsx_alb.alb.networkprofile {name}",)
+            result["comment"] = (f"Would create nsx_alb.alb.network_profile {name}",)
             return result
         else:
-            create_ret = await hub.exec.nsx_alb.alb.networkprofile.create(
+            create_ret = await hub.exec.nsx_alb.alb.network_profile.create(
                 ctx,
                 name=name,
                 **{
                     "configpb_attributes": configpb_attributes,
                     "connection_mirror": connection_mirror,
                     "description": description,
                     "markers": markers,
                     "profile": profile,
                     "tenant_ref": tenant_ref,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created 'nsx_alb.alb.networkprofile:{name}'")
+                result["comment"].append(
+                    f"Created 'nsx_alb.alb.network_profile:{name}'"
+                )
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.nsx_alb.alb.networkprofile.get(
+    after = await hub.exec.nsx_alb.alb.network_profile.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -382,54 +384,54 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.networkprofile.absent:
+              nsx_alb.alb.network_profile.absent:
                 - resource_id: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
-        result["comment"].append(f"'nsx_alb.alb.networkprofile:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.network_profile:{name}' already absent")
         return result
 
-    before = await hub.exec.nsx_alb.alb.networkprofile.get(
+    before = await hub.exec.nsx_alb.alb.network_profile.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete nsx_alb.alb.networkprofile:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.network_profile:{name}"
             return result
 
-        delete_ret = await hub.exec.nsx_alb.alb.networkprofile.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.network_profile.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'nsx_alb.alb.networkprofile:{name}'")
+            result["comment"].append(f"Deleted 'nsx_alb.alb.network_profile:{name}'")
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'nsx_alb.alb.networkprofile:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.network_profile:{name}' already absent")
         return result
 
     result["old_state"] = before.ret
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
@@ -453,28 +455,30 @@
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.networkprofile
+            $ idem describe nsx_alb.alb.network_profile
     """
 
     result = {}
 
-    ret = await hub.exec.nsx_alb.alb.networkprofile.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.network_profile.list(ctx)
 
     if not ret or not ret["result"]:
-        hub.log.debug(f"Could not describe nsx_alb.alb.networkprofile {ret['comment']}")
+        hub.log.debug(
+            f"Could not describe nsx_alb.alb.network_profile {ret['comment']}"
+        )
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "nsx_alb.alb.networkprofile.present": [
+            "nsx_alb.alb.network_profile.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/pool.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/pool.py`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/serviceenginegroup.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/service_engine_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1075,15 +1075,15 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.serviceenginegroup.present:
+              nsx_alb.alb.service_engine_group.present:
                 - name: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
@@ -1098,40 +1098,40 @@
                 tenant_ref_acct = ctx.acct.get("tenant_ref")
                 desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
 
             if k == "cloud_ref" and v is not None:
                 cloud_ref_acct = ctx.acct.get("cloud_ref")
                 desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
 
-    before = await hub.exec.nsx_alb.alb.serviceenginegroup.get(
+    before = await hub.exec.nsx_alb.alb.service_engine_group.get(
         ctx,
         name=name,
     )
     if before["ret"]:
         result["old_state"] = before.ret
         resource_id = before["ret"]["resource_id"]
     else:
         resource_id = None
 
     if resource_id:
-        before = await hub.exec.nsx_alb.alb.serviceenginegroup.get(
+        before = await hub.exec.nsx_alb.alb.service_engine_group.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
         result["comment"].append(
-            f"'nsx_alb.alb.serviceenginegroup:{name}' already exists"
+            f"'nsx_alb.alb.service_engine_group:{name}' already exists"
         )
 
         # If there are changes in desired state from existing state
         if desired_state:
             desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
                 ctx, data=desired_state
             )
@@ -1152,20 +1152,20 @@
             if ctx.test:
                 result[
                     "new_state"
                 ] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
                 result["comment"] = (
-                    f"Would update nsx_alb.alb.serviceenginegroup '{name}'",
+                    f"Would update nsx_alb.alb.service_engine_group '{name}'",
                 )
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.nsx_alb.alb.serviceenginegroup.update(
+                update_ret = await hub.exec.nsx_alb.alb.service_engine_group.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "accelerated_networking": accelerated_networking,
                         "active_standby": active_standby,
                         "aggressive_failure_detection": aggressive_failure_detection,
@@ -1448,27 +1448,29 @@
                         "waf_mempool_size": waf_mempool_size,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
                     result["comment"].append(
-                        f"Updated 'nsx_alb.alb.serviceenginegroup:{name}'"
+                        f"Updated 'nsx_alb.alb.service_engine_group:{name}'"
                     )
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result["new_state"] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create nsx_alb.alb.serviceenginegroup {name}",)
+            result["comment"] = (
+                f"Would create nsx_alb.alb.service_engine_group {name}",
+            )
             return result
         else:
-            create_ret = await hub.exec.nsx_alb.alb.serviceenginegroup.create(
+            create_ret = await hub.exec.nsx_alb.alb.service_engine_group.create(
                 ctx,
                 name=name,
                 **{
                     "accelerated_networking": accelerated_networking,
                     "active_standby": active_standby,
                     "aggressive_failure_detection": aggressive_failure_detection,
                     "algo": algo,
@@ -1750,29 +1752,29 @@
                     "waf_mempool_size": waf_mempool_size,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
                 result["comment"].append(
-                    f"Created 'nsx_alb.alb.serviceenginegroup:{name}'"
+                    f"Created 'nsx_alb.alb.service_engine_group:{name}'"
                 )
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.nsx_alb.alb.serviceenginegroup.get(
+    after = await hub.exec.nsx_alb.alb.service_engine_group.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -1794,57 +1796,59 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.serviceenginegroup.absent:
+              nsx_alb.alb.service_engine_group.absent:
                 - resource_id: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
         result["comment"].append(
-            f"'nsx_alb.alb.serviceenginegroup:{name}' already absent"
+            f"'nsx_alb.alb.service_engine_group:{name}' already absent"
         )
         return result
 
-    before = await hub.exec.nsx_alb.alb.serviceenginegroup.get(
+    before = await hub.exec.nsx_alb.alb.service_engine_group.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete nsx_alb.alb.serviceenginegroup:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.service_engine_group:{name}"
             return result
 
-        delete_ret = await hub.exec.nsx_alb.alb.serviceenginegroup.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.service_engine_group.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'nsx_alb.alb.serviceenginegroup:{name}'")
+            result["comment"].append(
+                f"Deleted 'nsx_alb.alb.service_engine_group:{name}'"
+            )
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
         result["comment"].append(
-            f"'nsx_alb.alb.serviceenginegroup:{name}' already absent"
+            f"'nsx_alb.alb.service_engine_group:{name}' already absent"
         )
         return result
 
     result["old_state"] = before.ret
     return result
 
 
@@ -1869,30 +1873,30 @@
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.serviceenginegroup
+            $ idem describe nsx_alb.alb.service_engine_group
     """
 
     result = {}
 
-    ret = await hub.exec.nsx_alb.alb.serviceenginegroup.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.service_engine_group.list(ctx)
 
     if not ret or not ret["result"]:
         hub.log.debug(
-            f"Could not describe nsx_alb.alb.serviceenginegroup {ret['comment']}"
+            f"Could not describe nsx_alb.alb.service_engine_group {ret['comment']}"
         )
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "nsx_alb.alb.serviceenginegroup.present": [
+            "nsx_alb.alb.service_engine_group.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/sslprofile.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/ssl_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.sslprofile.present:
+              nsx_alb.alb.ssl_profile.present:
                 - name: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
@@ -119,39 +119,39 @@
                 tenant_ref_acct = ctx.acct.get("tenant_ref")
                 desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
 
             if k == "cloud_ref" and v is not None:
                 cloud_ref_acct = ctx.acct.get("cloud_ref")
                 desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
 
-    before = await hub.exec.nsx_alb.alb.sslprofile.get(
+    before = await hub.exec.nsx_alb.alb.ssl_profile.get(
         ctx,
         name=name,
     )
     if before["ret"]:
         result["old_state"] = before.ret
         resource_id = before["ret"]["resource_id"]
     else:
         resource_id = None
 
     if resource_id:
-        before = await hub.exec.nsx_alb.alb.sslprofile.get(
+        before = await hub.exec.nsx_alb.alb.ssl_profile.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'nsx_alb.alb.sslprofile:{name}' already exists")
+        result["comment"].append(f"'nsx_alb.alb.ssl_profile:{name}' already exists")
 
         # If there are changes in desired state from existing state
         if desired_state:
             desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
                 ctx, data=desired_state
             )
         if desired_state:
@@ -170,19 +170,19 @@
         if bool(changes.get("new")):
             if ctx.test:
                 result[
                     "new_state"
                 ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
-                result["comment"] = (f"Would update nsx_alb.alb.sslprofile '{name}'",)
+                result["comment"] = (f"Would update nsx_alb.alb.ssl_profile '{name}'",)
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.nsx_alb.alb.sslprofile.update(
+                update_ret = await hub.exec.nsx_alb.alb.ssl_profile.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "accepted_ciphers": accepted_ciphers,
                         "accepted_versions": accepted_versions,
                         "cipher_enums": cipher_enums,
@@ -204,28 +204,30 @@
                         "tenant_ref": tenant_ref,
                         "type": type,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
-                    result["comment"].append(f"Updated 'nsx_alb.alb.sslprofile:{name}'")
+                    result["comment"].append(
+                        f"Updated 'nsx_alb.alb.ssl_profile:{name}'"
+                    )
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result[
                 "new_state"
             ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create nsx_alb.alb.sslprofile {name}",)
+            result["comment"] = (f"Would create nsx_alb.alb.ssl_profile {name}",)
             return result
         else:
-            create_ret = await hub.exec.nsx_alb.alb.sslprofile.create(
+            create_ret = await hub.exec.nsx_alb.alb.ssl_profile.create(
                 ctx,
                 name=name,
                 **{
                     "accepted_ciphers": accepted_ciphers,
                     "accepted_versions": accepted_versions,
                     "cipher_enums": cipher_enums,
                     "ciphersuites": ciphersuites,
@@ -246,28 +248,28 @@
                     "tenant_ref": tenant_ref,
                     "type": type,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created 'nsx_alb.alb.sslprofile:{name}'")
+                result["comment"].append(f"Created 'nsx_alb.alb.ssl_profile:{name}'")
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.nsx_alb.alb.sslprofile.get(
+    after = await hub.exec.nsx_alb.alb.ssl_profile.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -286,54 +288,54 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.sslprofile.absent:
+              nsx_alb.alb.ssl_profile.absent:
                 -
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
-        result["comment"].append(f"'nsx_alb.alb.sslprofile:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.ssl_profile:{name}' already absent")
         return result
 
-    before = await hub.exec.nsx_alb.alb.sslprofile.get(
+    before = await hub.exec.nsx_alb.alb.ssl_profile.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete nsx_alb.alb.sslprofile:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.ssl_profile:{name}"
             return result
 
-        delete_ret = await hub.exec.nsx_alb.alb.sslprofile.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.ssl_profile.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'nsx_alb.alb.sslprofile:{name}'")
+            result["comment"].append(f"Deleted 'nsx_alb.alb.ssl_profile:{name}'")
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'nsx_alb.alb.sslprofile:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.ssl_profile:{name}' already absent")
         return result
 
     result["old_state"] = before.ret
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
@@ -350,28 +352,28 @@
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.sslprofile
+            $ idem describe nsx_alb.alb.ssl_profile
     """
 
     result = {}
 
-    ret = await hub.exec.nsx_alb.alb.sslprofile.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.ssl_profile.list(ctx)
 
     if not ret or not ret["result"]:
-        hub.log.debug(f"Could not describe nsx_alb.alb.sslprofile {ret['comment']}")
+        hub.log.debug(f"Could not describe nsx_alb.alb.ssl_profile {ret['comment']}")
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "nsx_alb.alb.sslprofile.present": [
+            "nsx_alb.alb.ssl_profile.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/virtualservice.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/virtual_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2364,15 +2364,15 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.virtualservice.present:
+              nsx_alb.alb.virtual_service.present:
                 - name: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
@@ -2388,39 +2388,42 @@
                 tenant_ref_acct = ctx.acct.get("tenant_ref")
                 desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
 
             if k == "cloud_ref" and v is not None:
                 cloud_ref_acct = ctx.acct.get("cloud_ref")
                 desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
 
-    before = await hub.exec.nsx_alb.alb.virtualservice.get(
+    before = await hub.exec.nsx_alb.alb.virtual_service.get(
         ctx,
         name=name,
     )
     if before["ret"]:
         result["old_state"] = before.ret
         resource_id = before["ret"]["resource_id"]
     else:
         resource_id = None
 
+    for count in range(0, len(vip)):
+        vip[count]["vip_id"] = count
+
     if resource_id:
-        before = await hub.exec.nsx_alb.alb.virtualservice.get(
+        before = await hub.exec.nsx_alb.alb.virtual_service.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'nsx_alb.alb.virtualservice:{name}' already exists")
+        result["comment"].append(f"'nsx_alb.alb.virtual_service:{name}' already exists")
 
         # If there are changes in desired state from existing state
         if desired_state:
             desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
                 ctx, data=desired_state
             )
         if desired_state:
@@ -2440,20 +2443,20 @@
             if ctx.test:
                 result[
                     "new_state"
                 ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
                 result["comment"] = (
-                    f"Would update nsx_alb.alb.virtualservice '{name}'",
+                    f"Would update nsx_alb.alb.virtual_service '{name}'",
                 )
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.nsx_alb.alb.virtualservice.update(
+                update_ret = await hub.exec.nsx_alb.alb.virtual_service.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "active_standby_se_tag": active_standby_se_tag,
                         "advertise_down_vs": advertise_down_vs,
                         "allow_invalid_client_cert": allow_invalid_client_cert,
@@ -2548,29 +2551,29 @@
                         "weight": weight,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
                     result["comment"].append(
-                        f"Updated 'nsx_alb.alb.virtualservice:{name}'"
+                        f"Updated 'nsx_alb.alb.virtual_service:{name}'"
                     )
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result[
                 "new_state"
             ] = hub.tool.nsx_alb.alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create nsx_alb.alb.virtualservice {name}",)
+            result["comment"] = (f"Would create nsx_alb.alb.virtual_service {name}",)
             return result
         else:
-            create_ret = await hub.exec.nsx_alb.alb.virtualservice.create(
+            create_ret = await hub.exec.nsx_alb.alb.virtual_service.create(
                 ctx,
                 name=name,
                 **{
                     "active_standby_se_tag": active_standby_se_tag,
                     "advertise_down_vs": advertise_down_vs,
                     "allow_invalid_client_cert": allow_invalid_client_cert,
                     "analytics_policy": analytics_policy,
@@ -2663,28 +2666,30 @@
                     "waf_policy_ref": waf_policy_ref,
                     "weight": weight,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created 'nsx_alb.alb.virtualservice:{name}'")
+                result["comment"].append(
+                    f"Created 'nsx_alb.alb.virtual_service:{name}'"
+                )
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.nsx_alb.alb.virtualservice.get(
+    after = await hub.exec.nsx_alb.alb.virtual_service.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -2703,54 +2708,54 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.virtualservice.absent:
+              nsx_alb.alb.virtual_service.absent:
                 - resource_id: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
-        result["comment"].append(f"'nsx_alb.alb.virtualservice:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.virtual_service:{name}' already absent")
         return result
 
-    before = await hub.exec.nsx_alb.alb.virtualservice.get(
+    before = await hub.exec.nsx_alb.alb.virtual_service.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete nsx_alb.alb.virtualservice:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.virtual_service:{name}"
             return result
 
-        delete_ret = await hub.exec.nsx_alb.alb.virtualservice.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.virtual_service.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'nsx_alb.alb.virtualservice:{name}'")
+            result["comment"].append(f"Deleted 'nsx_alb.alb.virtual_service:{name}'")
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'nsx_alb.alb.virtualservice:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.virtual_service:{name}' already absent")
         return result
 
     result["old_state"] = before.ret
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
@@ -2770,28 +2775,30 @@
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.virtualservice
+            $ idem describe nsx_alb.alb.virtual_service
     """
 
     result = {}
 
-    ret = await hub.exec.nsx_alb.alb.virtualservice.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.virtual_service.list(ctx)
 
     if not ret or not ret["result"]:
-        hub.log.debug(f"Could not describe nsx_alb.alb.virtualservice {ret['comment']}")
+        hub.log.debug(
+            f"Could not describe nsx_alb.alb.virtual_service {ret['comment']}"
+        )
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "nsx_alb.alb.virtualservice.present": [
+            "nsx_alb.alb.virtual_service.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/states/nsx_alb/alb/vsvip.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/states/nsx_alb/alb/vs_vip.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_present:
-              nsx_alb.alb.vsvip.present:
+              nsx_alb.alb.vs_vip.present:
                 - x_avi_version: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
@@ -426,39 +426,39 @@
                 tenant_ref_acct = ctx.acct.get("tenant_ref")
                 desired_state.update({k: "/api/tenant/?name=" + tenant_ref_acct})
 
             if k == "cloud_ref" and v is not None:
                 cloud_ref_acct = ctx.acct.get("cloud_ref")
                 desired_state.update({k: "/api/cloud/?name=" + cloud_ref_acct})
 
-    before = await hub.exec.nsx_alb.alb.vsvip.get(
+    before = await hub.exec.nsx_alb.alb.vs_vip.get(
         ctx,
         name=name,
     )
     if before["ret"]:
         result["old_state"] = before.ret
         resource_id = before["ret"]["resource_id"]
     else:
         resource_id = None
 
     if resource_id:
-        before = await hub.exec.nsx_alb.alb.vsvip.get(
+        before = await hub.exec.nsx_alb.alb.vs_vip.get(
             ctx,
             name=name,
             resource_id=resource_id,
         )
 
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'nsx_alb.alb.vsvip:{name}' already exists")
+        result["comment"].append(f"'nsx_alb.alb.vs_vip:{name}' already exists")
 
         # If there are changes in desired state from existing state
         if desired_state:
             desired_state = await hub.tool.nsx_alb.utils.get_appended_prefix(
                 ctx, data=desired_state
             )
         if desired_state:
@@ -477,19 +477,19 @@
         if bool(changes.get("new")):
             if ctx.test:
                 result[
                     "new_state"
                 ] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                     enforced_state={}, desired_state=desired_state
                 )
-                result["comment"] = (f"Would update nsx_alb.alb.vsvip '{name}'",)
+                result["comment"] = (f"Would update nsx_alb.alb.vs_vip '{name}'",)
                 return result
             else:
                 # Update the resource
-                update_ret = await hub.exec.nsx_alb.alb.vsvip.update(
+                update_ret = await hub.exec.nsx_alb.alb.vs_vip.update(
                     ctx,
                     name=name,
                     resource_id=resource_id,
                     **{
                         "bgp_local_preference": bgp_local_preference,
                         "bgp_num_as_path_prepend": bgp_num_as_path_prepend,
                         "bgp_peer_labels": bgp_peer_labels,
@@ -506,26 +506,26 @@
                         "vrf_context_ref": vrf_context_ref,
                         "vsvip_cloud_config_cksum": vsvip_cloud_config_cksum,
                     },
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
-                    result["comment"].append(f"Updated 'nsx_alb.alb.vsvip:{name}'")
+                    result["comment"].append(f"Updated 'nsx_alb.alb.vs_vip:{name}'")
                 else:
                     result["comment"].append(update_ret["comment"])
     else:
         if ctx.test:
             result["new_state"] = hub.tool.nsx_alb.test_state_utils.generate_test_state(
                 enforced_state={}, desired_state=desired_state
             )
-            result["comment"] = (f"Would create nsx_alb.alb.vsvip {name}",)
+            result["comment"] = (f"Would create nsx_alb.alb.vs_vip {name}",)
             return result
         else:
-            create_ret = await hub.exec.nsx_alb.alb.vsvip.create(
+            create_ret = await hub.exec.nsx_alb.alb.vs_vip.create(
                 ctx,
                 name=name,
                 **{
                     "bgp_local_preference": bgp_local_preference,
                     "bgp_num_as_path_prepend": bgp_num_as_path_prepend,
                     "bgp_peer_labels": bgp_peer_labels,
                     "cloud_ref": cloud_ref,
@@ -541,28 +541,28 @@
                     "vrf_context_ref": vrf_context_ref,
                     "vsvip_cloud_config_cksum": vsvip_cloud_config_cksum,
                 },
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
-                result["comment"].append(f"Created 'nsx_alb.alb.vsvip:{name}'")
+                result["comment"].append(f"Created 'nsx_alb.alb.vs_vip:{name}'")
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
                 result["new_state"] = dict(name=name, resource_id=resource_id)
             else:
                 result["comment"].append(create_ret["comment"])
 
     if not result["result"]:
         # If there is any failure in create/update, it should reconcile.
         # The type of data is less important here to use default reconciliation
         # If there are no changes for 3 runs with rerun_data, then it will come out of execution
         result["rerun_data"] = dict(name=name, resource_id=resource_id)
 
-    after = await hub.exec.nsx_alb.alb.vsvip.get(
+    after = await hub.exec.nsx_alb.alb.vs_vip.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
     result["new_state"] = after.ret
     return result
 
@@ -584,54 +584,54 @@
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             resource_is_absent:
-              nsx_alb.alb.vsvip.absent:
+              nsx_alb.alb.vs_vip.absent:
                 - resource_id: value
     """
 
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
     if not resource_id:
-        result["comment"].append(f"'nsx_alb.alb.vsvip:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.vs_vip:{name}' already absent")
         return result
 
-    before = await hub.exec.nsx_alb.alb.vsvip.get(
+    before = await hub.exec.nsx_alb.alb.vs_vip.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
         if ctx.test:
-            result["comment"] = f"Would delete nsx_alb.alb.vsvip:{name}"
+            result["comment"] = f"Would delete nsx_alb.alb.vs_vip:{name}"
             return result
 
-        delete_ret = await hub.exec.nsx_alb.alb.vsvip.delete(
+        delete_ret = await hub.exec.nsx_alb.alb.vs_vip.delete(
             ctx,
             name=name,
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
-            result["comment"].append(f"Deleted 'nsx_alb.alb.vsvip:{name}'")
+            result["comment"].append(f"Deleted 'nsx_alb.alb.vs_vip:{name}'")
         else:
             # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
-        result["comment"].append(f"'nsx_alb.alb.vsvip:{name}' already absent")
+        result["comment"].append(f"'nsx_alb.alb.vs_vip:{name}' already absent")
         return result
 
     result["old_state"] = before.ret
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
@@ -655,28 +655,28 @@
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: bash
 
-            $ idem describe nsx_alb.alb.vsvip
+            $ idem describe nsx_alb.alb.vs_vip
     """
 
     result = {}
 
-    ret = await hub.exec.nsx_alb.alb.vsvip.list(ctx)
+    ret = await hub.exec.nsx_alb.alb.vs_vip.list(ctx)
 
     if not ret or not ret["result"]:
-        hub.log.debug(f"Could not describe nsx_alb.alb.vsvip {ret['comment']}")
+        hub.log.debug(f"Could not describe nsx_alb.alb.vs_vip {ret['comment']}")
         return result
 
     for resource in ret["ret"]:
 
         resource_id = resource.get("resource_id")
         result[resource_id] = {
-            "nsx_alb.alb.vsvip.present": [
+            "nsx_alb.alb.vs_vip.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/session.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/tool/nsx_alb/session.py`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb/tool/nsx_alb/test_state_utils.py` & `idem_vmware_alb-0.4.0/idem_vmware_alb/tool/nsx_alb/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/PKG-INFO` & `idem_vmware_alb-0.4.0/idem_vmware_alb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-vmware-alb
-Version: 0.3.0
+Version: 0.4.0
 Summary: VMware ALB Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-vmware-alb
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-vmware-alb
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-vmware-alb/-/issues
```

### Comparing `idem_vmware_alb-0.3.0/idem_vmware_alb.egg-info/SOURCES.txt` & `idem_vmware_alb-0.4.0/idem_vmware_alb.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 idem_vmware_alb.egg-info/SOURCES.txt
 idem_vmware_alb.egg-info/dependency_links.txt
 idem_vmware_alb.egg-info/requires.txt
 idem_vmware_alb.egg-info/top_level.txt
 idem_vmware_alb/acct/nsx_alb/basic_auth.py
 idem_vmware_alb/cloudspec/customize/nsx_alb.py
 idem_vmware_alb/exec/nsx_alb/init.py
-idem_vmware_alb/exec/nsx_alb/alb/applicationpersistenceprofile.py
-idem_vmware_alb/exec/nsx_alb/alb/applicationprofile.py
+idem_vmware_alb/exec/nsx_alb/alb/application_persistence_profile.py
+idem_vmware_alb/exec/nsx_alb/alb/application_profile.py
 idem_vmware_alb/exec/nsx_alb/alb/cloud.py
-idem_vmware_alb/exec/nsx_alb/alb/healthmonitor.py
-idem_vmware_alb/exec/nsx_alb/alb/networkprofile.py
+idem_vmware_alb/exec/nsx_alb/alb/health_monitor.py
+idem_vmware_alb/exec/nsx_alb/alb/network_profile.py
 idem_vmware_alb/exec/nsx_alb/alb/pool.py
-idem_vmware_alb/exec/nsx_alb/alb/serviceenginegroup.py
-idem_vmware_alb/exec/nsx_alb/alb/sslprofile.py
-idem_vmware_alb/exec/nsx_alb/alb/virtualservice.py
-idem_vmware_alb/exec/nsx_alb/alb/vsvip.py
+idem_vmware_alb/exec/nsx_alb/alb/service_engine_group.py
+idem_vmware_alb/exec/nsx_alb/alb/ssl_profile.py
+idem_vmware_alb/exec/nsx_alb/alb/virtual_service.py
+idem_vmware_alb/exec/nsx_alb/alb/vs_vip.py
 idem_vmware_alb/states/nsx_alb/init.py
-idem_vmware_alb/states/nsx_alb/alb/applicationpersistenceprofile.py
-idem_vmware_alb/states/nsx_alb/alb/applicationprofile.py
+idem_vmware_alb/states/nsx_alb/alb/application_persistence_profile.py
+idem_vmware_alb/states/nsx_alb/alb/application_profile.py
 idem_vmware_alb/states/nsx_alb/alb/cloud.py
-idem_vmware_alb/states/nsx_alb/alb/healthmonitor.py
-idem_vmware_alb/states/nsx_alb/alb/networkprofile.py
+idem_vmware_alb/states/nsx_alb/alb/health_monitor.py
+idem_vmware_alb/states/nsx_alb/alb/network_profile.py
 idem_vmware_alb/states/nsx_alb/alb/pool.py
-idem_vmware_alb/states/nsx_alb/alb/serviceenginegroup.py
-idem_vmware_alb/states/nsx_alb/alb/sslprofile.py
-idem_vmware_alb/states/nsx_alb/alb/virtualservice.py
-idem_vmware_alb/states/nsx_alb/alb/vsvip.py
+idem_vmware_alb/states/nsx_alb/alb/service_engine_group.py
+idem_vmware_alb/states/nsx_alb/alb/ssl_profile.py
+idem_vmware_alb/states/nsx_alb/alb/virtual_service.py
+idem_vmware_alb/states/nsx_alb/alb/vs_vip.py
 idem_vmware_alb/tool/nsx_alb/session.py
 idem_vmware_alb/tool/nsx_alb/test_state_utils.py
 idem_vmware_alb/tool/nsx_alb/utils.py
```

### Comparing `idem_vmware_alb-0.3.0/setup.py` & `idem_vmware_alb-0.4.0/setup.py`

 * *Files identical despite different names*

