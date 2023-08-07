# Comparing `tmp/threemystic_cloud_data_client-0.1.70.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.71.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.70.tar` & `threemystic_cloud_data_client-0.1.71.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0    20103 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/clouddb.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/elastisearch.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/function.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
--rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
--rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    25671 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/clouddb.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    13576 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/hatch.toml
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/pyproject.toml
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.70/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0    21191 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/clouddb.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/elastisearch.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/function.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
+-rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
+-rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    25671 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/clouddb.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    13576 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/hatch.toml
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/pyproject.toml
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.71/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,16 +10,9 @@
        "--elastisearch,--es": {
         "default": None, 
         "const": "elastisearch",
         "dest": "data_action",
         "help": "Data Action: This pulls Elasticsearch data from aws",
         "action": 'store_const' # could look into append_const
       },
-       "--elasticache,--ec": {
-        "default": None, 
-        "const": "elasticache",
-        "dest": "data_action",
-        "help": "Data Action: This pulls Elasticache data from aws",
-        "action": 'store_const' # could look into append_const
-      },
     }
```

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The AWS database Action. This will pull the AWS rds"""
 from threemystic_cloud_data_client.cloud_providers.aws.client.actions.base_class.base import cloud_data_client_aws_client_action_base as base
 import asyncio
 from decimal import Decimal, ROUND_HALF_UP
+from random import randint
 
 class cloud_data_client_aws_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="budget",
       logger_name= "cloud_data_client_aws_client_action_budget",
       *args, **kwargs)
@@ -82,84 +83,115 @@
       return "USAGE_QUANTITY"
     
     if self.get_common().helper_type().string().set_case(string_value= cost_metric, case= "lower") == "normalizedusageamount":
       return "NORMALIZED_USAGE_AMOUNT"
     
     return cost_metric
 
-
+  def __process_get_cost_data_process_forcast_process_day(self, cost_metric, year_data, data_dt, fiscal_start, fiscal_end, raw_data_cost, currency, total_key, *args, **kwargs):
+    by_month_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m", dt= data_dt)
+    day_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m%d", dt= data_dt)
+
+    if year_data.get(by_month_key) is None:
+      year_data[by_month_key] = self.__init_costdata_month(data_dt= data_dt)
+    
+    if year_data[by_month_key]["days"].get(day_key) is None:
+      year_data[by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= currency)
+    
+    raw_row_data_cost = raw_data_cost
+    row_data_cost = raw_data_cost
+    
+    if year_data[by_month_key]["days"][day_key]["currency"] != year_data[by_month_key]["days"][day_key]["origional_currency"]:
+      row_data_cost = self.get_common().helper_currency().convert(
+        ammount= row_data_cost,
+        currency_from= currency,
+        currency_to= year_data[by_month_key]["days"][day_key]["currency"],
+        conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
+          dt_string= self.get_common().helper_type().datetime().datetime_as_string(
+            dt= data_dt,
+            dt_format= "%Y%m01"
+          ),
+          dt_format= "%Y%m%d"
+        )).date()
+      )
+
+    year_data[by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
+    year_data[by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
+    year_data[by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
+    
+    if data_dt >= fiscal_start and data_dt <= fiscal_end:
+      year_data[by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
+  
   async def __process_get_cost_data_process_forcast(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, cost_metrics, *args, **kwargs):
     
     adjusted_enddated = (start_date
                  + self.get_common().helper_type().datetime().time_delta(months= 4, dt= start_date))
     for cost_metric in cost_metrics:
       
-      while start_date < end_date:
-        adjusted_enddated = (start_date + self.get_common().helper_type().datetime().time_delta(months= 4, dt= start_date))
-        
-        
-        results_by_time_forcast = self.get_cloud_client().general_boto_call_array(
-          boto_call=lambda: client.get_cost_forecast(
-            TimePeriod={
-              'Start': start_date.strftime("%Y-%m-%d"),
-              'End': (end_date if end_date < adjusted_enddated else adjusted_enddated).strftime("%Y-%m-%d"),
-            },
-            Granularity='DAILY',
-            Metric=self.__convert_costmetric_forecast_metric(cost_metric= cost_metric),
-            Filter={
-              "Dimensions":{
-                "Key":"LINKED_ACCOUNT",
-                "Values":[self.get_cloud_client().get_account_id(account= account)]
-              }
-            },
-          ),
-          boto_params= None,
-          boto_nextkey = None,
-          boto_key= None
-        )
-        
-        start_date += self.get_common().helper_type().datetime().time_delta(months= 4, dt= start_date)
-        total_key = "forcast_total"
-        currency = results_by_time_forcast["Total"]["Unit"]
+      adjusted_enddated = (start_date + self.get_common().helper_type().datetime().time_delta(months= 4, dt= start_date))
+      adjusted_enddated = self.get_common().helper_type().datetime().datetime_from_string(adjusted_enddated.strftime("%Y-01-%d"), dt_format="%Y-%m-%d")
+      if end_date < adjusted_enddated:
+       adjusted_enddated =  end_date
       
+      results_by_time_forcast = self.get_cloud_client().general_boto_call_array(
+        boto_call=lambda: client.get_cost_forecast(
+          TimePeriod={
+            'Start': start_date.strftime("%Y-%m-%d"),
+            'End': adjusted_enddated.strftime("%Y-%m-%d"),
+          },
+          Granularity='DAILY',
+          Metric=self.__convert_costmetric_forecast_metric(cost_metric= cost_metric),
+          Filter={
+            "Dimensions":{
+              "Key":"LINKED_ACCOUNT",
+              "Values":[self.get_cloud_client().get_account_id(account= account)]
+            }
+          },
+        ),
+        boto_params= None,
+        boto_nextkey = None,
+        boto_key= None
+      )
       
-        year_data[cost_metric] = {}
-        for cost_data in results_by_time_forcast["ForecastResultsByTime"]:
-          data_dt = self.get_common().helper_type().datetime().datetime_from_string(dt_string= str(cost_data["TimePeriod"]["Start"]), dt_format= "%Y-%m-%d")
-          by_month_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m", dt= data_dt)
-
-          day_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m%d", dt= data_dt)
-          if year_data.get(by_month_key) is None:
-            year_data[cost_metric][by_month_key] = self.__init_costdata_month(data_dt= data_dt)
-          
-          if year_data[cost_metric][by_month_key]["days"].get(day_key) is None:
-            year_data[cost_metric][by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= currency)
-          
-          raw_row_data_cost = (cost_data["MeanValue"])
-          row_data_cost = (cost_data["MeanValue"])
-          
-          if year_data[cost_metric][by_month_key]["days"][day_key]["currency"] != year_data[cost_metric][by_month_key]["days"][day_key]["origional_currency"]:
-            row_data_cost = self.get_common().helper_currency().convert(
-              ammount= row_data_cost,
-              currency_from= currency,
-              currency_to= year_data[cost_metric][by_month_key]["days"][day_key]["currency"],
-              conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
-                dt_string= self.get_common().helper_type().datetime().datetime_as_string(
-                  dt= data_dt,
-                  dt_format= "%Y%m01"
-                ),
-                dt_format= "%Y%m%d"
-              )).date()
-            )
-
-          year_data[cost_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
-          year_data[cost_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
-          year_data[cost_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
-          if data_dt >= fiscal_start and data_dt <= fiscal_end:
-            year_data[cost_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
+      total_key = "forcast_total"
+      currency = results_by_time_forcast["Total"]["Unit"]
+    
+    
+      year_data[cost_metric] = {}
+      for cost_data in results_by_time_forcast["ForecastResultsByTime"]:
+        data_dt = self.get_common().helper_type().datetime().datetime_from_string(dt_string= str(cost_data["TimePeriod"]["Start"]), dt_format= "%Y-%m-%d")
+
+        self.__process_get_cost_data_process_forcast_process_day(
+          cost_metric= cost_metric,
+          year_data= year_data[cost_metric],
+          data_dt= data_dt,
+          fiscal_start= fiscal_start,
+          fiscal_end= fiscal_end,
+          raw_data_cost = (cost_data["MeanValue"]),
+          currency= currency,
+          total_key= total_key
+        )
+
+      while data_dt < end_date:
+        data_dt += (self.get_common().helper_type().datetime().time_delta(days= 1, dt= data_dt))
+        by_month_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m", dt= data_dt)
+        day_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m%d", dt= data_dt)
+        cost_data = year_data[cost_metric][by_month_key]["days"][day_key]
+
+        self.__process_get_cost_data_process_forcast_process_day(
+          cost_metric= cost_metric,
+          year_data= year_data[cost_metric],
+          data_dt= data_dt,
+          fiscal_start= fiscal_start,
+          fiscal_end= fiscal_end,
+          raw_data_cost = (cost_data[total_key] * (1 + (randint(0,20)/Decimal(100)))),
+          currency= (cost_data["currency"]),
+          total_key= total_key
+        )
+
 
   def get_total_cost_data(self, cost_data, cost_metric, *args, **kwargs):
     if cost_data["Total"].get(cost_metric) is not None:
       if cost_data["Total"][cost_metric].get("Amount") is not None:
         return Decimal(cost_data["Total"][cost_metric]["Amount"])
     
     return Decimal(0)
```

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/clouddb.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/clouddb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/elastisearch.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/elastisearch.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/function.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/function.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/clouddb.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/clouddb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.71/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/.gitignore` & `threemystic_cloud_data_client-0.1.71/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/LICENSE` & `threemystic_cloud_data_client-0.1.71/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/README.md` & `threemystic_cloud_data_client-0.1.71/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/hatch.toml` & `threemystic_cloud_data_client-0.1.71/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/pyproject.toml` & `threemystic_cloud_data_client-0.1.71/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.70/PKG-INFO` & `threemystic_cloud_data_client-0.1.71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.70
+Version: 0.1.71
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

