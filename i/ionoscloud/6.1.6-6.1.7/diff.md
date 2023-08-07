# Comparing `tmp/ionoscloud-6.1.6.tar.gz` & `tmp/ionoscloud-6.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionoscloud-6.1.6.tar", last modified: Thu May 25 15:59:12 2023, max compression
+gzip compressed data, was "ionoscloud-6.1.7.tar", last modified: Mon Aug  7 10:14:57 2023, max compression
```

## Comparing `ionoscloud-6.1.6.tar` & `ionoscloud-6.1.7.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:59:12.755700 ionoscloud-6.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-05-25 13:54:45.000000 ionoscloud-6.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    67140 2023-05-25 15:59:12.755700 ionoscloud-6.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66298 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:59:12.735700 ionoscloud-6.1.6/ionoscloud/
--rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:59:12.739700 ionoscloud-6.1.6/ionoscloud/api/
--rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/__api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   214360 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/application_load_balancers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    64006 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/backup_units_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/contract_resources_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    59505 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/data_centers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    75244 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/firewall_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    70578 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/flow_logs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45940 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/images_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57205 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/ip_blocks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   160838 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/kubernetes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   273991 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/labels_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    95950 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/lans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   108586 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/load_balancers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28903 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/locations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   198835 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/nat_gateways_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/network_interfaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/network_load_balancers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45784 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/private_cross_connects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36951 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/requests_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   241017 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/servers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46438 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    59171 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/target_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   226405 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/user_management_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    56921 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/user_s3_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    86491 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api/volumes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34764 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:59:12.755700 ionoscloud-6.1.6/ionoscloud/models/
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_forwarding_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_forwarding_rule_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_forwarding_rule_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_http_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_http_rule_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/application_load_balancers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/attached_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/backup_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/backup_unit_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/backup_unit_sso.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/backup_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/balanced_nics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/cdroms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/connectable_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/contract_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/cpu_architecture_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/data_center_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/datacenter_element_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/datacenter_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    18284 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/firewallrule_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/flow_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/flow_log_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/flow_log_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/group_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/group_members.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/group_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/group_share.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/group_share_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/group_shares.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/group_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/image_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/ip_block_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/ip_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/ip_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/ip_failover.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_auto_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_for_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_for_put.py
--rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_properties_for_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_properties_for_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_for_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_for_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_lan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_lan_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)    23285 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    22471 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_properties_for_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_properties_for_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/kubernetes_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/label_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/label_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/label_resource_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/label_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/lan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/lan_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/lan_nics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/lan_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/lan_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/lan_properties_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/lans.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/loadbalancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/loadbalancer_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/loadbalancer_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/location_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_lan_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nat_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_target_health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/network_load_balancers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nic_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nic_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nic_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/nics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/no_state_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/pagination_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/private_cross_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/private_cross_connect_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/private_cross_connects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/remote_console_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/request_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/request_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/request_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/request_status_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/request_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/resource_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    30562 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/resource_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/resource_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/resource_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/resources_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/s3_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/s3_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/s3_key_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/s3_key_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/s3_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/s3_object_storage_sso.py
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/server_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/server_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/snapshot_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/target_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/target_group_health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/target_group_http_health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/target_group_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/target_group_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/target_group_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/target_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/target_port_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/template_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/user_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/user_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/user_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/user_properties_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/user_properties_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/user_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/users_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/volume_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-05-25 13:55:09.000000 ionoscloud-6.1.6/ionoscloud/models/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/ionoscloud/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:59:12.735700 ionoscloud-6.1.6/ionoscloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    67140 2023-05-25 15:59:12.000000 ionoscloud-6.1.6/ionoscloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-05-25 15:59:12.000000 ionoscloud-6.1.6/ionoscloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:59:12.000000 ionoscloud-6.1.6/ionoscloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 15:59:12.000000 ionoscloud-6.1.6/ionoscloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 15:59:12.000000 ionoscloud-6.1.6/ionoscloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 15:59:12.755700 ionoscloud-6.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-25 13:55:10.000000 ionoscloud-6.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:14:57.419974 ionoscloud-6.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-08-07 10:13:53.000000 ionoscloud-6.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    67140 2023-08-07 10:14:57.419974 ionoscloud-6.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66298 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:14:57.379974 ionoscloud-6.1.7/ionoscloud/
+-rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:14:57.387974 ionoscloud-6.1.7/ionoscloud/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/__api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214360 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/application_load_balancers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64006 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/backup_units_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/contract_resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59505 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/data_centers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75244 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/firewall_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70578 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/flow_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45940 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/images_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57205 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/ip_blocks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160838 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/kubernetes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   273991 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/labels_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95950 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/lans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108586 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/load_balancers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28903 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/locations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198835 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/nat_gateways_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/network_interfaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/network_load_balancers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45784 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/private_cross_connects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36951 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241017 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/servers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46438 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59171 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/target_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226405 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/user_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56921 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/user_s3_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86491 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api/volumes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34932 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:14:57.419974 ionoscloud-6.1.7/ionoscloud/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_forwarding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_forwarding_rule_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_forwarding_rule_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_http_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_http_rule_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/application_load_balancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/attached_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/backup_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/backup_unit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/backup_unit_sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/backup_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/balanced_nics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/cdroms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/connectable_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/contract_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/cpu_architecture_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/data_center_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/datacenter_element_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/datacenter_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18284 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/firewallrule_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/flow_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/flow_log_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/flow_log_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/group_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/group_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/group_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/group_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/group_share_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/group_shares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/group_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/image_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/ip_block_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/ip_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/ip_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/ip_failover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_auto_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_for_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_for_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_properties_for_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_properties_for_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_for_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_for_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_lan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_lan_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23285 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22471 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_properties_for_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_properties_for_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/kubernetes_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/label_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/label_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/label_resource_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/label_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/lan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/lan_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/lan_nics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/lan_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/lan_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-07 10:14:15.000000 ionoscloud-6.1.7/ionoscloud/models/lan_properties_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/lans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/loadbalancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/loadbalancer_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/loadbalancer_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/location_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_lan_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nat_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_target_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/network_load_balancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nic_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nic_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nic_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/nics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/no_state_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/pagination_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/private_cross_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/private_cross_connect_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/private_cross_connects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/remote_console_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/request_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/request_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/request_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/request_status_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/resource_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30562 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/resource_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/resource_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/resource_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/resources_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/s3_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/s3_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/s3_key_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/s3_key_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/s3_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/s3_object_storage_sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/server_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/server_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/snapshot_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/target_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/target_group_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/target_group_http_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/target_group_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/target_group_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/target_group_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/target_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/target_port_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/template_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/user_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/user_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/user_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/user_properties_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/user_properties_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/user_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/users_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/volume_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-08-07 10:14:16.000000 ionoscloud-6.1.7/ionoscloud/models/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/ionoscloud/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:14:57.379974 ionoscloud-6.1.7/ionoscloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    67140 2023-08-07 10:14:57.000000 ionoscloud-6.1.7/ionoscloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-08-07 10:14:57.000000 ionoscloud-6.1.7/ionoscloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:14:57.000000 ionoscloud-6.1.7/ionoscloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 10:14:57.000000 ionoscloud-6.1.7/ionoscloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 10:14:57.000000 ionoscloud-6.1.7/ionoscloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 10:14:57.419974 ionoscloud-6.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-07 10:14:17.000000 ionoscloud-6.1.7/setup.py
```

### Comparing `ionoscloud-6.1.6/LICENSE` & `ionoscloud-6.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/PKG-INFO` & `ionoscloud-6.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionoscloud
-Version: 6.1.6
+Version: 6.1.7
 Summary: Python SDK for the Ionos Cloud API
 Home-page: https://github.com/ionos-cloud/ionos-cloud-sdk-python
 Author: Ionos Cloud
 Author-email: sdk@cloud.ionos.com
 Keywords: OpenAPI,OpenAPI-Generator,CLOUD API
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
```

### Comparing `ionoscloud-6.1.6/README.md` & `ionoscloud-6.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/__init__.py` & `ionoscloud-6.1.7/ionoscloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 6.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "6.1.6"
+__version__ = "6.1.7"
 
 # import apis into sdk package
 from ionoscloud.api.application_load_balancers_api import ApplicationLoadBalancersApi
 from ionoscloud.api.backup_units_api import BackupUnitsApi
 from ionoscloud.api.contract_resources_api import ContractResourcesApi
 from ionoscloud.api.data_centers_api import DataCentersApi
 from ionoscloud.api.firewall_rules_api import FirewallRulesApi
```

### Comparing `ionoscloud-6.1.6/ionoscloud/api/__api.py` & `ionoscloud-6.1.7/ionoscloud/api/__api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/__init__.py` & `ionoscloud-6.1.7/ionoscloud/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/application_load_balancers_api.py` & `ionoscloud-6.1.7/ionoscloud/api/application_load_balancers_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/backup_units_api.py` & `ionoscloud-6.1.7/ionoscloud/api/backup_units_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/contract_resources_api.py` & `ionoscloud-6.1.7/ionoscloud/api/contract_resources_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/data_centers_api.py` & `ionoscloud-6.1.7/ionoscloud/api/data_centers_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/firewall_rules_api.py` & `ionoscloud-6.1.7/ionoscloud/api/firewall_rules_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/flow_logs_api.py` & `ionoscloud-6.1.7/ionoscloud/api/flow_logs_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/images_api.py` & `ionoscloud-6.1.7/ionoscloud/api/images_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/ip_blocks_api.py` & `ionoscloud-6.1.7/ionoscloud/api/ip_blocks_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/kubernetes_api.py` & `ionoscloud-6.1.7/ionoscloud/api/kubernetes_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/labels_api.py` & `ionoscloud-6.1.7/ionoscloud/api/labels_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/lans_api.py` & `ionoscloud-6.1.7/ionoscloud/api/lans_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/load_balancers_api.py` & `ionoscloud-6.1.7/ionoscloud/api/load_balancers_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/locations_api.py` & `ionoscloud-6.1.7/ionoscloud/api/locations_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/nat_gateways_api.py` & `ionoscloud-6.1.7/ionoscloud/api/nat_gateways_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/network_interfaces_api.py` & `ionoscloud-6.1.7/ionoscloud/api/network_interfaces_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/network_load_balancers_api.py` & `ionoscloud-6.1.7/ionoscloud/api/network_load_balancers_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/private_cross_connects_api.py` & `ionoscloud-6.1.7/ionoscloud/api/private_cross_connects_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/requests_api.py` & `ionoscloud-6.1.7/ionoscloud/api/requests_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/servers_api.py` & `ionoscloud-6.1.7/ionoscloud/api/servers_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/snapshots_api.py` & `ionoscloud-6.1.7/ionoscloud/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/target_groups_api.py` & `ionoscloud-6.1.7/ionoscloud/api/target_groups_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/templates_api.py` & `ionoscloud-6.1.7/ionoscloud/api/templates_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/user_management_api.py` & `ionoscloud-6.1.7/ionoscloud/api/user_management_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/user_s3_keys_api.py` & `ionoscloud-6.1.7/ionoscloud/api/user_s3_keys_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api/volumes_api.py` & `ionoscloud-6.1.7/ionoscloud/api/volumes_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/api_client.py` & `ionoscloud-6.1.7/ionoscloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'ionos-cloud-sdk-python/6.1.6'
+        self.user_agent = 'ionos-cloud-sdk-python/6.1.7'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -856,18 +856,21 @@
             check_response = fn_check(resp)
 
             if check_response:
                 break
 
             current_time = time.time()
             if timeout and current_time > timeout:
-                raise ApiTimeout(
-                    message='Timed out waiting for request {0}.'.format(resp['requestId']),
-                    request_id=resp['requestId']
-                )
+                if type(resp) == dict and resp.get('requestId'):
+                    raise ApiTimeout(
+                        message='Timed out waiting for request {0}.'.format(resp['requestId']),
+                        request_id=resp['requestId'],
+                    )
+                else:
+                    raise ApiTimeout(message='Timeout reached')
 
             if current_time > next_increase:
                 wait_period *= 2
                 next_increase = time.time() + wait_period * scaleup
                 scaleup *= 2
 
             logger.info("Sleeping for %i seconds...", wait_period)
```

### Comparing `ionoscloud-6.1.6/ionoscloud/configuration.py` & `ionoscloud-6.1.7/ionoscloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 6.0\n"\
-               "SDK Package Version: 6.1.6".\
+               "SDK Package Version: 6.1.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ionoscloud-6.1.6/ionoscloud/exceptions.py` & `ionoscloud-6.1.7/ionoscloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/__init__.py` & `ionoscloud-6.1.7/ionoscloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_forwarding_rule.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_forwarding_rule_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_forwarding_rule_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_forwarding_rule_put.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_forwarding_rule_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_forwarding_rules.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_http_rule.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_http_rule.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_http_rule_condition.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_http_rule_condition.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancer_put.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancer_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/application_load_balancers.py` & `ionoscloud-6.1.7/ionoscloud/models/application_load_balancers.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/attached_volumes.py` & `ionoscloud-6.1.7/ionoscloud/models/attached_volumes.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/backup_unit.py` & `ionoscloud-6.1.7/ionoscloud/models/backup_unit.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/backup_unit_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/backup_unit_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/backup_unit_sso.py` & `ionoscloud-6.1.7/ionoscloud/models/backup_unit_sso.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/backup_units.py` & `ionoscloud-6.1.7/ionoscloud/models/backup_units.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/balanced_nics.py` & `ionoscloud-6.1.7/ionoscloud/models/balanced_nics.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/cdroms.py` & `ionoscloud-6.1.7/ionoscloud/models/cdroms.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/connectable_datacenter.py` & `ionoscloud-6.1.7/ionoscloud/models/connectable_datacenter.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/contract.py` & `ionoscloud-6.1.7/ionoscloud/models/contract.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/contract_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/contract_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/contracts.py` & `ionoscloud-6.1.7/ionoscloud/models/contracts.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/cpu_architecture_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/cpu_architecture_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/data_center_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/data_center_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/datacenter.py` & `ionoscloud-6.1.7/ionoscloud/models/datacenter.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/datacenter_element_metadata.py` & `ionoscloud-6.1.7/ionoscloud/models/datacenter_element_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/datacenter_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/datacenter_properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
         'cpu_architecture': 'list[CpuArchitectureProperties]',
 
         'description': 'str',
 
         'features': 'list[str]',
 
+        'ipv6_cidr_block': 'str',
+
         'location': 'str',
 
         'name': 'str',
 
         'sec_auth_protection': 'bool',
 
         'version': 'int',
@@ -53,44 +55,48 @@
 
         'cpu_architecture': 'cpuArchitecture',
 
         'description': 'description',
 
         'features': 'features',
 
+        'ipv6_cidr_block': 'ipv6CidrBlock',
+
         'location': 'location',
 
         'name': 'name',
 
         'sec_auth_protection': 'secAuthProtection',
 
         'version': 'version',
     }
 
-    def __init__(self, cpu_architecture=None, description=None, features=None, location=None, name=None, sec_auth_protection=None, version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, cpu_architecture=None, description=None, features=None, ipv6_cidr_block=None, location=None, name=None, sec_auth_protection=None, version=None, local_vars_configuration=None):  # noqa: E501
         """DatacenterProperties - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._cpu_architecture = None
         self._description = None
         self._features = None
+        self._ipv6_cidr_block = None
         self._location = None
         self._name = None
         self._sec_auth_protection = None
         self._version = None
         self.discriminator = None
 
         if cpu_architecture is not None:
             self.cpu_architecture = cpu_architecture
         if description is not None:
             self.description = description
         if features is not None:
             self.features = features
+        self.ipv6_cidr_block = ipv6_cidr_block
         self.location = location
         if name is not None:
             self.name = name
         if sec_auth_protection is not None:
             self.sec_auth_protection = sec_auth_protection
         if version is not None:
             self.version = version
@@ -162,14 +168,37 @@
         :param features: The features of this DatacenterProperties.  # noqa: E501
         :type features: list[str]
         """
 
         self._features = features
 
     @property
+    def ipv6_cidr_block(self):
+        """Gets the ipv6_cidr_block of this DatacenterProperties.  # noqa: E501
+
+        [The IPv6 feature is in beta phase and not ready for production usage.] This value is either 'null' or contains an automatically-assigned /56 IPv6 CIDR block if IPv6 is enabled on this virtual data center. It can neither be changed nor removed.  # noqa: E501
+
+        :return: The ipv6_cidr_block of this DatacenterProperties.  # noqa: E501
+        :rtype: str
+        """
+        return self._ipv6_cidr_block
+
+    @ipv6_cidr_block.setter
+    def ipv6_cidr_block(self, ipv6_cidr_block):
+        """Sets the ipv6_cidr_block of this DatacenterProperties.
+
+        [The IPv6 feature is in beta phase and not ready for production usage.] This value is either 'null' or contains an automatically-assigned /56 IPv6 CIDR block if IPv6 is enabled on this virtual data center. It can neither be changed nor removed.  # noqa: E501
+
+        :param ipv6_cidr_block: The ipv6_cidr_block of this DatacenterProperties.  # noqa: E501
+        :type ipv6_cidr_block: str
+        """
+
+        self._ipv6_cidr_block = ipv6_cidr_block
+
+    @property
     def location(self):
         """Gets the location of this DatacenterProperties.  # noqa: E501
 
         The physical location where the datacenter will be created. This will be where all of your servers live. Property cannot be modified after datacenter creation (disallowed in update requests).  # noqa: E501
 
         :return: The location of this DatacenterProperties.  # noqa: E501
         :rtype: str
```

### Comparing `ionoscloud-6.1.6/ionoscloud/models/datacenters.py` & `ionoscloud-6.1.7/ionoscloud/models/datacenters.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/error.py` & `ionoscloud-6.1.7/ionoscloud/models/error.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/error_message.py` & `ionoscloud-6.1.7/ionoscloud/models/error_message.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/firewall_rule.py` & `ionoscloud-6.1.7/ionoscloud/models/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/firewall_rules.py` & `ionoscloud-6.1.7/ionoscloud/models/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/firewallrule_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/firewallrule_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/flow_log.py` & `ionoscloud-6.1.7/ionoscloud/models/flow_log.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/flow_log_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/flow_log_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/flow_log_put.py` & `ionoscloud-6.1.7/ionoscloud/models/flow_log_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/flow_logs.py` & `ionoscloud-6.1.7/ionoscloud/models/flow_logs.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/group.py` & `ionoscloud-6.1.7/ionoscloud/models/group.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/group_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/group_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/group_members.py` & `ionoscloud-6.1.7/ionoscloud/models/group_members.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/group_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/group_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/group_share.py` & `ionoscloud-6.1.7/ionoscloud/models/group_share.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/group_share_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/group_share_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/group_shares.py` & `ionoscloud-6.1.7/ionoscloud/models/group_shares.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/group_users.py` & `ionoscloud-6.1.7/ionoscloud/models/group_users.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/groups.py` & `ionoscloud-6.1.7/ionoscloud/models/groups.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/image.py` & `ionoscloud-6.1.7/ionoscloud/models/image.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/image_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/image_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/images.py` & `ionoscloud-6.1.7/ionoscloud/models/images.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/info.py` & `ionoscloud-6.1.7/ionoscloud/models/info.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/ip_block.py` & `ionoscloud-6.1.7/ionoscloud/models/ip_block.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/ip_block_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/ip_block_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/ip_blocks.py` & `ionoscloud-6.1.7/ionoscloud/models/ip_blocks.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/ip_consumer.py` & `ionoscloud-6.1.7/ionoscloud/models/ip_consumer.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/ip_failover.py` & `ionoscloud-6.1.7/ionoscloud/models/ip_failover.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_auto_scaling.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_auto_scaling.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_for_post.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_for_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_for_put.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_for_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_properties_for_post.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_properties_for_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_cluster_properties_for_put.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_cluster_properties_for_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_clusters.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_clusters.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_maintenance_window.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_maintenance_window.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_metadata.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_for_post.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_for_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_for_put.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_for_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_lan.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_lan.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_lan_routes.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_lan_routes.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_properties_for_post.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_properties_for_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pool_properties_for_put.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pool_properties_for_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_pools.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_pools.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_node_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_node_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/kubernetes_nodes.py` & `ionoscloud-6.1.7/ionoscloud/models/kubernetes_nodes.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/label.py` & `ionoscloud-6.1.7/ionoscloud/models/label.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/label_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/label_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/label_resource.py` & `ionoscloud-6.1.7/ionoscloud/models/label_resource.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/label_resource_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/label_resource_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/label_resources.py` & `ionoscloud-6.1.7/ionoscloud/models/label_resources.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/labels.py` & `ionoscloud-6.1.7/ionoscloud/models/labels.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/lan.py` & `ionoscloud-6.1.7/ionoscloud/models/lan.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/lan_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/lan_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/lan_nics.py` & `ionoscloud-6.1.7/ionoscloud/models/lan_nics.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/lan_post.py` & `ionoscloud-6.1.7/ionoscloud/models/lan_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/lan_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/volume.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class LanProperties(object):
+class Volume(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,147 +30,174 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'ip_failover': 'list[IPFailover]',
+        'href': 'str',
 
-        'name': 'str',
+        'id': 'str',
 
-        'pcc': 'str',
+        'metadata': 'DatacenterElementMetadata',
 
-        'public': 'bool',
+        'properties': 'VolumeProperties',
+
+        'type': 'Type',
     }
 
     attribute_map = {
 
-        'ip_failover': 'ipFailover',
+        'href': 'href',
+
+        'id': 'id',
 
-        'name': 'name',
+        'metadata': 'metadata',
 
-        'pcc': 'pcc',
+        'properties': 'properties',
 
-        'public': 'public',
+        'type': 'type',
     }
 
-    def __init__(self, ip_failover=None, name=None, pcc=None, public=None, local_vars_configuration=None):  # noqa: E501
-        """LanProperties - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, href=None, id=None, metadata=None, properties=None, type=None, local_vars_configuration=None):  # noqa: E501
+        """Volume - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._ip_failover = None
-        self._name = None
-        self._pcc = None
-        self._public = None
+        self._href = None
+        self._id = None
+        self._metadata = None
+        self._properties = None
+        self._type = None
         self.discriminator = None
 
-        if ip_failover is not None:
-            self.ip_failover = ip_failover
-        if name is not None:
-            self.name = name
-        if pcc is not None:
-            self.pcc = pcc
-        if public is not None:
-            self.public = public
+        if href is not None:
+            self.href = href
+        if id is not None:
+            self.id = id
+        if metadata is not None:
+            self.metadata = metadata
+        self.properties = properties
+        if type is not None:
+            self.type = type
 
 
     @property
-    def ip_failover(self):
-        """Gets the ip_failover of this LanProperties.  # noqa: E501
+    def href(self):
+        """Gets the href of this Volume.  # noqa: E501
 
-        IP failover configurations for lan  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
-        :return: The ip_failover of this LanProperties.  # noqa: E501
-        :rtype: list[IPFailover]
+        :return: The href of this Volume.  # noqa: E501
+        :rtype: str
         """
-        return self._ip_failover
+        return self._href
 
-    @ip_failover.setter
-    def ip_failover(self, ip_failover):
-        """Sets the ip_failover of this LanProperties.
+    @href.setter
+    def href(self, href):
+        """Sets the href of this Volume.
 
-        IP failover configurations for lan  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
-        :param ip_failover: The ip_failover of this LanProperties.  # noqa: E501
-        :type ip_failover: list[IPFailover]
+        :param href: The href of this Volume.  # noqa: E501
+        :type href: str
         """
 
-        self._ip_failover = ip_failover
+        self._href = href
 
     @property
-    def name(self):
-        """Gets the name of this LanProperties.  # noqa: E501
+    def id(self):
+        """Gets the id of this Volume.  # noqa: E501
 
-        The name of the  resource.  # noqa: E501
+        The resource's unique identifier.  # noqa: E501
 
-        :return: The name of this LanProperties.  # noqa: E501
+        :return: The id of this Volume.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._id
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this LanProperties.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this Volume.
 
-        The name of the  resource.  # noqa: E501
+        The resource's unique identifier.  # noqa: E501
 
-        :param name: The name of this LanProperties.  # noqa: E501
-        :type name: str
+        :param id: The id of this Volume.  # noqa: E501
+        :type id: str
         """
 
-        self._name = name
+        self._id = id
 
     @property
-    def pcc(self):
-        """Gets the pcc of this LanProperties.  # noqa: E501
+    def metadata(self):
+        """Gets the metadata of this Volume.  # noqa: E501
 
-        The unique identifier of the private Cross-Connect the LAN is connected to, if any.  # noqa: E501
 
-        :return: The pcc of this LanProperties.  # noqa: E501
-        :rtype: str
+        :return: The metadata of this Volume.  # noqa: E501
+        :rtype: DatacenterElementMetadata
+        """
+        return self._metadata
+
+    @metadata.setter
+    def metadata(self, metadata):
+        """Sets the metadata of this Volume.
+
+
+        :param metadata: The metadata of this Volume.  # noqa: E501
+        :type metadata: DatacenterElementMetadata
+        """
+
+        self._metadata = metadata
+
+    @property
+    def properties(self):
+        """Gets the properties of this Volume.  # noqa: E501
+
+
+        :return: The properties of this Volume.  # noqa: E501
+        :rtype: VolumeProperties
         """
-        return self._pcc
+        return self._properties
 
-    @pcc.setter
-    def pcc(self, pcc):
-        """Sets the pcc of this LanProperties.
+    @properties.setter
+    def properties(self, properties):
+        """Sets the properties of this Volume.
 
-        The unique identifier of the private Cross-Connect the LAN is connected to, if any.  # noqa: E501
 
-        :param pcc: The pcc of this LanProperties.  # noqa: E501
-        :type pcc: str
+        :param properties: The properties of this Volume.  # noqa: E501
+        :type properties: VolumeProperties
         """
+        if self.local_vars_configuration.client_side_validation and properties is None:  # noqa: E501
+            raise ValueError("Invalid value for `properties`, must not be `None`")  # noqa: E501
 
-        self._pcc = pcc
+        self._properties = properties
 
     @property
-    def public(self):
-        """Gets the public of this LanProperties.  # noqa: E501
+    def type(self):
+        """Gets the type of this Volume.  # noqa: E501
 
-        This LAN faces the public Internet.  # noqa: E501
+        The type of object that has been created.  # noqa: E501
 
-        :return: The public of this LanProperties.  # noqa: E501
-        :rtype: bool
+        :return: The type of this Volume.  # noqa: E501
+        :rtype: Type
         """
-        return self._public
+        return self._type
 
-    @public.setter
-    def public(self, public):
-        """Sets the public of this LanProperties.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this Volume.
 
-        This LAN faces the public Internet.  # noqa: E501
+        The type of object that has been created.  # noqa: E501
 
-        :param public: The public of this LanProperties.  # noqa: E501
-        :type public: bool
+        :param type: The type of this Volume.  # noqa: E501
+        :type type: Type
         """
 
-        self._public = public
+        self._type = type
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -197,18 +224,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LanProperties):
+        if not isinstance(other, Volume):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LanProperties):
+        if not isinstance(other, Volume):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.6/ionoscloud/models/lan_properties_post.py` & `ionoscloud-6.1.7/ionoscloud/models/nics.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class LanPropertiesPost(object):
+class Nics(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,147 +30,235 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'ip_failover': 'list[IPFailover]',
+        'links': 'PaginationLinks',
 
-        'name': 'str',
+        'href': 'str',
 
-        'pcc': 'str',
+        'id': 'str',
 
-        'public': 'bool',
+        'items': 'list[Nic]',
+
+        'limit': 'float',
+
+        'offset': 'float',
+
+        'type': 'Type',
     }
 
     attribute_map = {
 
-        'ip_failover': 'ipFailover',
+        'links': '_links',
+
+        'href': 'href',
+
+        'id': 'id',
 
-        'name': 'name',
+        'items': 'items',
 
-        'pcc': 'pcc',
+        'limit': 'limit',
 
-        'public': 'public',
+        'offset': 'offset',
+
+        'type': 'type',
     }
 
-    def __init__(self, ip_failover=None, name=None, pcc=None, public=None, local_vars_configuration=None):  # noqa: E501
-        """LanPropertiesPost - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, links=None, href=None, id=None, items=None, limit=None, offset=None, type=None, local_vars_configuration=None):  # noqa: E501
+        """Nics - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._ip_failover = None
-        self._name = None
-        self._pcc = None
-        self._public = None
+        self._links = None
+        self._href = None
+        self._id = None
+        self._items = None
+        self._limit = None
+        self._offset = None
+        self._type = None
         self.discriminator = None
 
-        if ip_failover is not None:
-            self.ip_failover = ip_failover
-        if name is not None:
-            self.name = name
-        if pcc is not None:
-            self.pcc = pcc
-        if public is not None:
-            self.public = public
+        if links is not None:
+            self.links = links
+        if href is not None:
+            self.href = href
+        if id is not None:
+            self.id = id
+        if items is not None:
+            self.items = items
+        if limit is not None:
+            self.limit = limit
+        if offset is not None:
+            self.offset = offset
+        if type is not None:
+            self.type = type
 
 
     @property
-    def ip_failover(self):
-        """Gets the ip_failover of this LanPropertiesPost.  # noqa: E501
+    def links(self):
+        """Gets the links of this Nics.  # noqa: E501
 
-        IP failover configurations for lan  # noqa: E501
 
-        :return: The ip_failover of this LanPropertiesPost.  # noqa: E501
-        :rtype: list[IPFailover]
+        :return: The links of this Nics.  # noqa: E501
+        :rtype: PaginationLinks
         """
-        return self._ip_failover
+        return self._links
 
-    @ip_failover.setter
-    def ip_failover(self, ip_failover):
-        """Sets the ip_failover of this LanPropertiesPost.
+    @links.setter
+    def links(self, links):
+        """Sets the links of this Nics.
 
-        IP failover configurations for lan  # noqa: E501
 
-        :param ip_failover: The ip_failover of this LanPropertiesPost.  # noqa: E501
-        :type ip_failover: list[IPFailover]
+        :param links: The links of this Nics.  # noqa: E501
+        :type links: PaginationLinks
         """
 
-        self._ip_failover = ip_failover
+        self._links = links
 
     @property
-    def name(self):
-        """Gets the name of this LanPropertiesPost.  # noqa: E501
+    def href(self):
+        """Gets the href of this Nics.  # noqa: E501
 
-        The name of the  resource.  # noqa: E501
+        URL to the object representation (absolute path).  # noqa: E501
 
-        :return: The name of this LanPropertiesPost.  # noqa: E501
+        :return: The href of this Nics.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._href
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this LanPropertiesPost.
+    @href.setter
+    def href(self, href):
+        """Sets the href of this Nics.
 
-        The name of the  resource.  # noqa: E501
+        URL to the object representation (absolute path).  # noqa: E501
 
-        :param name: The name of this LanPropertiesPost.  # noqa: E501
-        :type name: str
+        :param href: The href of this Nics.  # noqa: E501
+        :type href: str
         """
 
-        self._name = name
+        self._href = href
 
     @property
-    def pcc(self):
-        """Gets the pcc of this LanPropertiesPost.  # noqa: E501
+    def id(self):
+        """Gets the id of this Nics.  # noqa: E501
 
-        The unique identifier of the private Cross-Connect the LAN is connected to, if any.  # noqa: E501
+        The resource's unique identifier.  # noqa: E501
 
-        :return: The pcc of this LanPropertiesPost.  # noqa: E501
+        :return: The id of this Nics.  # noqa: E501
         :rtype: str
         """
-        return self._pcc
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this Nics.
+
+        The resource's unique identifier.  # noqa: E501
+
+        :param id: The id of this Nics.  # noqa: E501
+        :type id: str
+        """
+
+        self._id = id
+
+    @property
+    def items(self):
+        """Gets the items of this Nics.  # noqa: E501
+
+        Array of items in the collection.  # noqa: E501
+
+        :return: The items of this Nics.  # noqa: E501
+        :rtype: list[Nic]
+        """
+        return self._items
+
+    @items.setter
+    def items(self, items):
+        """Sets the items of this Nics.
+
+        Array of items in the collection.  # noqa: E501
+
+        :param items: The items of this Nics.  # noqa: E501
+        :type items: list[Nic]
+        """
+
+        self._items = items
+
+    @property
+    def limit(self):
+        """Gets the limit of this Nics.  # noqa: E501
+
+        The limit (if specified in the request).  # noqa: E501
+
+        :return: The limit of this Nics.  # noqa: E501
+        :rtype: float
+        """
+        return self._limit
+
+    @limit.setter
+    def limit(self, limit):
+        """Sets the limit of this Nics.
+
+        The limit (if specified in the request).  # noqa: E501
+
+        :param limit: The limit of this Nics.  # noqa: E501
+        :type limit: float
+        """
+
+        self._limit = limit
+
+    @property
+    def offset(self):
+        """Gets the offset of this Nics.  # noqa: E501
+
+        The offset (if specified in the request).  # noqa: E501
+
+        :return: The offset of this Nics.  # noqa: E501
+        :rtype: float
+        """
+        return self._offset
 
-    @pcc.setter
-    def pcc(self, pcc):
-        """Sets the pcc of this LanPropertiesPost.
+    @offset.setter
+    def offset(self, offset):
+        """Sets the offset of this Nics.
 
-        The unique identifier of the private Cross-Connect the LAN is connected to, if any.  # noqa: E501
+        The offset (if specified in the request).  # noqa: E501
 
-        :param pcc: The pcc of this LanPropertiesPost.  # noqa: E501
-        :type pcc: str
+        :param offset: The offset of this Nics.  # noqa: E501
+        :type offset: float
         """
 
-        self._pcc = pcc
+        self._offset = offset
 
     @property
-    def public(self):
-        """Gets the public of this LanPropertiesPost.  # noqa: E501
+    def type(self):
+        """Gets the type of this Nics.  # noqa: E501
 
-        This LAN faces the public Internet.  # noqa: E501
+        The type of object that has been created.  # noqa: E501
 
-        :return: The public of this LanPropertiesPost.  # noqa: E501
-        :rtype: bool
+        :return: The type of this Nics.  # noqa: E501
+        :rtype: Type
         """
-        return self._public
+        return self._type
 
-    @public.setter
-    def public(self, public):
-        """Sets the public of this LanPropertiesPost.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this Nics.
 
-        This LAN faces the public Internet.  # noqa: E501
+        The type of object that has been created.  # noqa: E501
 
-        :param public: The public of this LanPropertiesPost.  # noqa: E501
-        :type public: bool
+        :param type: The type of this Nics.  # noqa: E501
+        :type type: Type
         """
 
-        self._public = public
+        self._type = type
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -197,18 +285,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LanPropertiesPost):
+        if not isinstance(other, Nics):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LanPropertiesPost):
+        if not isinstance(other, Nics):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.6/ionoscloud/models/lans.py` & `ionoscloud-6.1.7/ionoscloud/models/lans.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/loadbalancer.py` & `ionoscloud-6.1.7/ionoscloud/models/loadbalancer.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/loadbalancer_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/loadbalancer_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/loadbalancer_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/loadbalancer_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/loadbalancers.py` & `ionoscloud-6.1.7/ionoscloud/models/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/location.py` & `ionoscloud-6.1.7/ionoscloud/models/location.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/location_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/location_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/locations.py` & `ionoscloud-6.1.7/ionoscloud/models/locations.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_lan_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_lan_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_put.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule_protocol.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule_protocol.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule_put.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rule_type.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rule_type.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateway_rules.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateway_rules.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nat_gateways.py` & `ionoscloud-6.1.7/ionoscloud/models/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_health_check.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_health_check.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_put.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_target.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_target.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rule_target_health_check.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rule_target_health_check.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_forwarding_rules.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancer_put.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancer_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/network_load_balancers.py` & `ionoscloud-6.1.7/ionoscloud/models/network_load_balancers.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nic.py` & `ionoscloud-6.1.7/ionoscloud/models/nic.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nic_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/nic_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nic_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/server_properties.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class NicProperties(object):
+class ServerProperties(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,303 +30,335 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'device_number': 'int',
+        'availability_zone': 'str',
 
-        'dhcp': 'bool',
+        'boot_cdrom': 'ResourceReference',
 
-        'firewall_active': 'bool',
+        'boot_volume': 'ResourceReference',
 
-        'firewall_type': 'str',
+        'cores': 'int',
 
-        'ips': 'list[str]',
+        'cpu_family': 'str',
 
-        'lan': 'int',
+        'name': 'str',
 
-        'mac': 'str',
+        'ram': 'int',
 
-        'name': 'str',
+        'template_uuid': 'str',
+
+        'type': 'str',
 
-        'pci_slot': 'int',
+        'vm_state': 'str',
     }
 
     attribute_map = {
 
-        'device_number': 'deviceNumber',
+        'availability_zone': 'availabilityZone',
 
-        'dhcp': 'dhcp',
+        'boot_cdrom': 'bootCdrom',
 
-        'firewall_active': 'firewallActive',
+        'boot_volume': 'bootVolume',
 
-        'firewall_type': 'firewallType',
+        'cores': 'cores',
 
-        'ips': 'ips',
+        'cpu_family': 'cpuFamily',
 
-        'lan': 'lan',
+        'name': 'name',
 
-        'mac': 'mac',
+        'ram': 'ram',
 
-        'name': 'name',
+        'template_uuid': 'templateUuid',
+
+        'type': 'type',
 
-        'pci_slot': 'pciSlot',
+        'vm_state': 'vmState',
     }
 
-    def __init__(self, device_number=None, dhcp=True, firewall_active=None, firewall_type=None, ips=None, lan=None, mac=None, name=None, pci_slot=None, local_vars_configuration=None):  # noqa: E501
-        """NicProperties - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, availability_zone=None, boot_cdrom=None, boot_volume=None, cores=None, cpu_family=None, name=None, ram=None, template_uuid=None, type=None, vm_state=None, local_vars_configuration=None):  # noqa: E501
+        """ServerProperties - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._device_number = None
-        self._dhcp = None
-        self._firewall_active = None
-        self._firewall_type = None
-        self._ips = None
-        self._lan = None
-        self._mac = None
+        self._availability_zone = None
+        self._boot_cdrom = None
+        self._boot_volume = None
+        self._cores = None
+        self._cpu_family = None
         self._name = None
-        self._pci_slot = None
+        self._ram = None
+        self._template_uuid = None
+        self._type = None
+        self._vm_state = None
         self.discriminator = None
 
-        if device_number is not None:
-            self.device_number = device_number
-        if dhcp is not None:
-            self.dhcp = dhcp
-        if firewall_active is not None:
-            self.firewall_active = firewall_active
-        if firewall_type is not None:
-            self.firewall_type = firewall_type
-        self.ips = ips
-        self.lan = lan
-        if mac is not None:
-            self.mac = mac
+        if availability_zone is not None:
+            self.availability_zone = availability_zone
+        if boot_cdrom is not None:
+            self.boot_cdrom = boot_cdrom
+        if boot_volume is not None:
+            self.boot_volume = boot_volume
+        if cores is not None:
+            self.cores = cores
+        if cpu_family is not None:
+            self.cpu_family = cpu_family
         if name is not None:
             self.name = name
-        if pci_slot is not None:
-            self.pci_slot = pci_slot
+        if ram is not None:
+            self.ram = ram
+        if template_uuid is not None:
+            self.template_uuid = template_uuid
+        if type is not None:
+            self.type = type
+        if vm_state is not None:
+            self.vm_state = vm_state
 
 
     @property
-    def device_number(self):
-        """Gets the device_number of this NicProperties.  # noqa: E501
+    def availability_zone(self):
+        """Gets the availability_zone of this ServerProperties.  # noqa: E501
 
-        The Logical Unit Number (LUN) of the storage volume. Null if this NIC was created using Cloud API and no DCD changes were performed on the Datacenter.  # noqa: E501
+        The availability zone in which the server should be provisioned.  # noqa: E501
 
-        :return: The device_number of this NicProperties.  # noqa: E501
-        :rtype: int
+        :return: The availability_zone of this ServerProperties.  # noqa: E501
+        :rtype: str
+        """
+        return self._availability_zone
+
+    @availability_zone.setter
+    def availability_zone(self, availability_zone):
+        """Sets the availability_zone of this ServerProperties.
+
+        The availability zone in which the server should be provisioned.  # noqa: E501
+
+        :param availability_zone: The availability_zone of this ServerProperties.  # noqa: E501
+        :type availability_zone: str
         """
-        return self._device_number
+        allowed_values = ["AUTO", "ZONE_1", "ZONE_2"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and availability_zone not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `availability_zone` ({0}), must be one of {1}"  # noqa: E501
+                .format(availability_zone, allowed_values)
+            )
 
-    @device_number.setter
-    def device_number(self, device_number):
-        """Sets the device_number of this NicProperties.
+        self._availability_zone = availability_zone
+
+    @property
+    def boot_cdrom(self):
+        """Gets the boot_cdrom of this ServerProperties.  # noqa: E501
 
-        The Logical Unit Number (LUN) of the storage volume. Null if this NIC was created using Cloud API and no DCD changes were performed on the Datacenter.  # noqa: E501
 
-        :param device_number: The device_number of this NicProperties.  # noqa: E501
-        :type device_number: int
+        :return: The boot_cdrom of this ServerProperties.  # noqa: E501
+        :rtype: ResourceReference
         """
+        return self._boot_cdrom
+
+    @boot_cdrom.setter
+    def boot_cdrom(self, boot_cdrom):
+        """Sets the boot_cdrom of this ServerProperties.
 
-        self._device_number = device_number
+
+        :param boot_cdrom: The boot_cdrom of this ServerProperties.  # noqa: E501
+        :type boot_cdrom: ResourceReference
+        """
+
+        self._boot_cdrom = boot_cdrom
 
     @property
-    def dhcp(self):
-        """Gets the dhcp of this NicProperties.  # noqa: E501
+    def boot_volume(self):
+        """Gets the boot_volume of this ServerProperties.  # noqa: E501
 
-        Indicates if the NIC will reserve an IP using DHCP.  # noqa: E501
 
-        :return: The dhcp of this NicProperties.  # noqa: E501
-        :rtype: bool
+        :return: The boot_volume of this ServerProperties.  # noqa: E501
+        :rtype: ResourceReference
         """
-        return self._dhcp
+        return self._boot_volume
 
-    @dhcp.setter
-    def dhcp(self, dhcp):
-        """Sets the dhcp of this NicProperties.
+    @boot_volume.setter
+    def boot_volume(self, boot_volume):
+        """Sets the boot_volume of this ServerProperties.
 
-        Indicates if the NIC will reserve an IP using DHCP.  # noqa: E501
 
-        :param dhcp: The dhcp of this NicProperties.  # noqa: E501
-        :type dhcp: bool
+        :param boot_volume: The boot_volume of this ServerProperties.  # noqa: E501
+        :type boot_volume: ResourceReference
         """
 
-        self._dhcp = dhcp
+        self._boot_volume = boot_volume
 
     @property
-    def firewall_active(self):
-        """Gets the firewall_active of this NicProperties.  # noqa: E501
+    def cores(self):
+        """Gets the cores of this ServerProperties.  # noqa: E501
 
-        Activate or deactivate the firewall. By default, an active firewall without any defined rules will block all incoming network traffic except for the firewall rules that explicitly allows certain protocols, IP addresses and ports.  # noqa: E501
+        The total number of cores for the enterprise server.  # noqa: E501
 
-        :return: The firewall_active of this NicProperties.  # noqa: E501
-        :rtype: bool
+        :return: The cores of this ServerProperties.  # noqa: E501
+        :rtype: int
         """
-        return self._firewall_active
+        return self._cores
 
-    @firewall_active.setter
-    def firewall_active(self, firewall_active):
-        """Sets the firewall_active of this NicProperties.
+    @cores.setter
+    def cores(self, cores):
+        """Sets the cores of this ServerProperties.
 
-        Activate or deactivate the firewall. By default, an active firewall without any defined rules will block all incoming network traffic except for the firewall rules that explicitly allows certain protocols, IP addresses and ports.  # noqa: E501
+        The total number of cores for the enterprise server.  # noqa: E501
 
-        :param firewall_active: The firewall_active of this NicProperties.  # noqa: E501
-        :type firewall_active: bool
+        :param cores: The cores of this ServerProperties.  # noqa: E501
+        :type cores: int
         """
 
-        self._firewall_active = firewall_active
+        self._cores = cores
 
     @property
-    def firewall_type(self):
-        """Gets the firewall_type of this NicProperties.  # noqa: E501
+    def cpu_family(self):
+        """Gets the cpu_family of this ServerProperties.  # noqa: E501
 
-        The type of firewall rules that will be allowed on the NIC. If not specified, the default INGRESS value is used.  # noqa: E501
+        CPU architecture on which server gets provisioned; not all CPU architectures are available in all datacenter regions; available CPU architectures can be retrieved from the datacenter resource; must not be provided for CUBE servers.  # noqa: E501
 
-        :return: The firewall_type of this NicProperties.  # noqa: E501
+        :return: The cpu_family of this ServerProperties.  # noqa: E501
         :rtype: str
         """
-        return self._firewall_type
+        return self._cpu_family
 
-    @firewall_type.setter
-    def firewall_type(self, firewall_type):
-        """Sets the firewall_type of this NicProperties.
+    @cpu_family.setter
+    def cpu_family(self, cpu_family):
+        """Sets the cpu_family of this ServerProperties.
 
-        The type of firewall rules that will be allowed on the NIC. If not specified, the default INGRESS value is used.  # noqa: E501
+        CPU architecture on which server gets provisioned; not all CPU architectures are available in all datacenter regions; available CPU architectures can be retrieved from the datacenter resource; must not be provided for CUBE servers.  # noqa: E501
 
-        :param firewall_type: The firewall_type of this NicProperties.  # noqa: E501
-        :type firewall_type: str
+        :param cpu_family: The cpu_family of this ServerProperties.  # noqa: E501
+        :type cpu_family: str
         """
-        allowed_values = ["INGRESS", "EGRESS", "BIDIRECTIONAL"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and firewall_type not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `firewall_type` ({0}), must be one of {1}"  # noqa: E501
-                .format(firewall_type, allowed_values)
-            )
 
-        self._firewall_type = firewall_type
+        self._cpu_family = cpu_family
 
     @property
-    def ips(self):
-        """Gets the ips of this NicProperties.  # noqa: E501
+    def name(self):
+        """Gets the name of this ServerProperties.  # noqa: E501
 
-        Collection of IP addresses, assigned to the NIC. Explicitly assigned public IPs need to come from reserved IP blocks. Passing value null or empty array will assign an IP address automatically.  # noqa: E501
+        The name of the  resource.  # noqa: E501
 
-        :return: The ips of this NicProperties.  # noqa: E501
-        :rtype: list[str]
+        :return: The name of this ServerProperties.  # noqa: E501
+        :rtype: str
         """
-        return self._ips
+        return self._name
 
-    @ips.setter
-    def ips(self, ips):
-        """Sets the ips of this NicProperties.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this ServerProperties.
 
-        Collection of IP addresses, assigned to the NIC. Explicitly assigned public IPs need to come from reserved IP blocks. Passing value null or empty array will assign an IP address automatically.  # noqa: E501
+        The name of the  resource.  # noqa: E501
 
-        :param ips: The ips of this NicProperties.  # noqa: E501
-        :type ips: list[str]
+        :param name: The name of this ServerProperties.  # noqa: E501
+        :type name: str
         """
 
-        self._ips = ips
+        self._name = name
 
     @property
-    def lan(self):
-        """Gets the lan of this NicProperties.  # noqa: E501
+    def ram(self):
+        """Gets the ram of this ServerProperties.  # noqa: E501
 
-        The LAN ID the NIC will be on. If the LAN ID does not exist, it will be implicitly created.  # noqa: E501
+        The memory size for the enterprise server in MB, such as 2048. Size must be specified in multiples of 256 MB with a minimum of 256 MB; however, if you set ramHotPlug to TRUE then you must use a minimum of 1024 MB. If you set the RAM size more than 240GB, then ramHotPlug will be set to FALSE and can not be set to TRUE unless RAM size not set to less than 240GB.  # noqa: E501
 
-        :return: The lan of this NicProperties.  # noqa: E501
+        :return: The ram of this ServerProperties.  # noqa: E501
         :rtype: int
         """
-        return self._lan
+        return self._ram
 
-    @lan.setter
-    def lan(self, lan):
-        """Sets the lan of this NicProperties.
+    @ram.setter
+    def ram(self, ram):
+        """Sets the ram of this ServerProperties.
 
-        The LAN ID the NIC will be on. If the LAN ID does not exist, it will be implicitly created.  # noqa: E501
+        The memory size for the enterprise server in MB, such as 2048. Size must be specified in multiples of 256 MB with a minimum of 256 MB; however, if you set ramHotPlug to TRUE then you must use a minimum of 1024 MB. If you set the RAM size more than 240GB, then ramHotPlug will be set to FALSE and can not be set to TRUE unless RAM size not set to less than 240GB.  # noqa: E501
 
-        :param lan: The lan of this NicProperties.  # noqa: E501
-        :type lan: int
+        :param ram: The ram of this ServerProperties.  # noqa: E501
+        :type ram: int
         """
-        if self.local_vars_configuration.client_side_validation and lan is None:  # noqa: E501
-            raise ValueError("Invalid value for `lan`, must not be `None`")  # noqa: E501
 
-        self._lan = lan
+        self._ram = ram
 
     @property
-    def mac(self):
-        """Gets the mac of this NicProperties.  # noqa: E501
+    def template_uuid(self):
+        """Gets the template_uuid of this ServerProperties.  # noqa: E501
 
-        The MAC address of the NIC.  # noqa: E501
+        The ID of the template for creating a CUBE server; the available templates for CUBE servers can be found on the templates resource.  # noqa: E501
 
-        :return: The mac of this NicProperties.  # noqa: E501
+        :return: The template_uuid of this ServerProperties.  # noqa: E501
         :rtype: str
         """
-        return self._mac
+        return self._template_uuid
 
-    @mac.setter
-    def mac(self, mac):
-        """Sets the mac of this NicProperties.
+    @template_uuid.setter
+    def template_uuid(self, template_uuid):
+        """Sets the template_uuid of this ServerProperties.
 
-        The MAC address of the NIC.  # noqa: E501
+        The ID of the template for creating a CUBE server; the available templates for CUBE servers can be found on the templates resource.  # noqa: E501
 
-        :param mac: The mac of this NicProperties.  # noqa: E501
-        :type mac: str
+        :param template_uuid: The template_uuid of this ServerProperties.  # noqa: E501
+        :type template_uuid: str
         """
 
-        self._mac = mac
+        self._template_uuid = template_uuid
 
     @property
-    def name(self):
-        """Gets the name of this NicProperties.  # noqa: E501
+    def type(self):
+        """Gets the type of this ServerProperties.  # noqa: E501
 
-        The name of the  resource.  # noqa: E501
+        Server type: CUBE or ENTERPRISE.  # noqa: E501
 
-        :return: The name of this NicProperties.  # noqa: E501
+        :return: The type of this ServerProperties.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._type
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this NicProperties.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this ServerProperties.
 
-        The name of the  resource.  # noqa: E501
+        Server type: CUBE or ENTERPRISE.  # noqa: E501
 
-        :param name: The name of this NicProperties.  # noqa: E501
-        :type name: str
+        :param type: The type of this ServerProperties.  # noqa: E501
+        :type type: str
         """
 
-        self._name = name
+        self._type = type
 
     @property
-    def pci_slot(self):
-        """Gets the pci_slot of this NicProperties.  # noqa: E501
+    def vm_state(self):
+        """Gets the vm_state of this ServerProperties.  # noqa: E501
 
-        The PCI slot number for the NIC.  # noqa: E501
+        Status of the virtual machine.  # noqa: E501
 
-        :return: The pci_slot of this NicProperties.  # noqa: E501
-        :rtype: int
+        :return: The vm_state of this ServerProperties.  # noqa: E501
+        :rtype: str
         """
-        return self._pci_slot
+        return self._vm_state
 
-    @pci_slot.setter
-    def pci_slot(self, pci_slot):
-        """Sets the pci_slot of this NicProperties.
+    @vm_state.setter
+    def vm_state(self, vm_state):
+        """Sets the vm_state of this ServerProperties.
 
-        The PCI slot number for the NIC.  # noqa: E501
+        Status of the virtual machine.  # noqa: E501
 
-        :param pci_slot: The pci_slot of this NicProperties.  # noqa: E501
-        :type pci_slot: int
+        :param vm_state: The vm_state of this ServerProperties.  # noqa: E501
+        :type vm_state: str
         """
+        allowed_values = ["NOSTATE", "RUNNING", "BLOCKED", "PAUSED", "SHUTDOWN", "SHUTOFF", "CRASHED", "SUSPENDED"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and vm_state not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `vm_state` ({0}), must be one of {1}"  # noqa: E501
+                .format(vm_state, allowed_values)
+            )
 
-        self._pci_slot = pci_slot
+        self._vm_state = vm_state
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -353,18 +385,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NicProperties):
+        if not isinstance(other, ServerProperties):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, NicProperties):
+        if not isinstance(other, ServerProperties):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nic_put.py` & `ionoscloud-6.1.7/ionoscloud/models/nic_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/nics.py` & `ionoscloud-6.1.7/ionoscloud/models/servers.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class Nics(object):
+class Servers(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -36,15 +36,15 @@
 
         'links': 'PaginationLinks',
 
         'href': 'str',
 
         'id': 'str',
 
-        'items': 'list[Nic]',
+        'items': 'list[Server]',
 
         'limit': 'float',
 
         'offset': 'float',
 
         'type': 'Type',
     }
@@ -63,15 +63,15 @@
 
         'offset': 'offset',
 
         'type': 'type',
     }
 
     def __init__(self, links=None, href=None, id=None, items=None, limit=None, offset=None, type=None, local_vars_configuration=None):  # noqa: E501
-        """Nics - a model defined in OpenAPI"""  # noqa: E501
+        """Servers - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._links = None
         self._href = None
         self._id = None
@@ -95,166 +95,166 @@
             self.offset = offset
         if type is not None:
             self.type = type
 
 
     @property
     def links(self):
-        """Gets the links of this Nics.  # noqa: E501
+        """Gets the links of this Servers.  # noqa: E501
 
 
-        :return: The links of this Nics.  # noqa: E501
+        :return: The links of this Servers.  # noqa: E501
         :rtype: PaginationLinks
         """
         return self._links
 
     @links.setter
     def links(self, links):
-        """Sets the links of this Nics.
+        """Sets the links of this Servers.
 
 
-        :param links: The links of this Nics.  # noqa: E501
+        :param links: The links of this Servers.  # noqa: E501
         :type links: PaginationLinks
         """
 
         self._links = links
 
     @property
     def href(self):
-        """Gets the href of this Nics.  # noqa: E501
+        """Gets the href of this Servers.  # noqa: E501
 
         URL to the object representation (absolute path).  # noqa: E501
 
-        :return: The href of this Nics.  # noqa: E501
+        :return: The href of this Servers.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
-        """Sets the href of this Nics.
+        """Sets the href of this Servers.
 
         URL to the object representation (absolute path).  # noqa: E501
 
-        :param href: The href of this Nics.  # noqa: E501
+        :param href: The href of this Servers.  # noqa: E501
         :type href: str
         """
 
         self._href = href
 
     @property
     def id(self):
-        """Gets the id of this Nics.  # noqa: E501
+        """Gets the id of this Servers.  # noqa: E501
 
         The resource's unique identifier.  # noqa: E501
 
-        :return: The id of this Nics.  # noqa: E501
+        :return: The id of this Servers.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this Nics.
+        """Sets the id of this Servers.
 
         The resource's unique identifier.  # noqa: E501
 
-        :param id: The id of this Nics.  # noqa: E501
+        :param id: The id of this Servers.  # noqa: E501
         :type id: str
         """
 
         self._id = id
 
     @property
     def items(self):
-        """Gets the items of this Nics.  # noqa: E501
+        """Gets the items of this Servers.  # noqa: E501
 
         Array of items in the collection.  # noqa: E501
 
-        :return: The items of this Nics.  # noqa: E501
-        :rtype: list[Nic]
+        :return: The items of this Servers.  # noqa: E501
+        :rtype: list[Server]
         """
         return self._items
 
     @items.setter
     def items(self, items):
-        """Sets the items of this Nics.
+        """Sets the items of this Servers.
 
         Array of items in the collection.  # noqa: E501
 
-        :param items: The items of this Nics.  # noqa: E501
-        :type items: list[Nic]
+        :param items: The items of this Servers.  # noqa: E501
+        :type items: list[Server]
         """
 
         self._items = items
 
     @property
     def limit(self):
-        """Gets the limit of this Nics.  # noqa: E501
+        """Gets the limit of this Servers.  # noqa: E501
 
         The limit (if specified in the request).  # noqa: E501
 
-        :return: The limit of this Nics.  # noqa: E501
+        :return: The limit of this Servers.  # noqa: E501
         :rtype: float
         """
         return self._limit
 
     @limit.setter
     def limit(self, limit):
-        """Sets the limit of this Nics.
+        """Sets the limit of this Servers.
 
         The limit (if specified in the request).  # noqa: E501
 
-        :param limit: The limit of this Nics.  # noqa: E501
+        :param limit: The limit of this Servers.  # noqa: E501
         :type limit: float
         """
 
         self._limit = limit
 
     @property
     def offset(self):
-        """Gets the offset of this Nics.  # noqa: E501
+        """Gets the offset of this Servers.  # noqa: E501
 
         The offset (if specified in the request).  # noqa: E501
 
-        :return: The offset of this Nics.  # noqa: E501
+        :return: The offset of this Servers.  # noqa: E501
         :rtype: float
         """
         return self._offset
 
     @offset.setter
     def offset(self, offset):
-        """Sets the offset of this Nics.
+        """Sets the offset of this Servers.
 
         The offset (if specified in the request).  # noqa: E501
 
-        :param offset: The offset of this Nics.  # noqa: E501
+        :param offset: The offset of this Servers.  # noqa: E501
         :type offset: float
         """
 
         self._offset = offset
 
     @property
     def type(self):
-        """Gets the type of this Nics.  # noqa: E501
+        """Gets the type of this Servers.  # noqa: E501
 
         The type of object that has been created.  # noqa: E501
 
-        :return: The type of this Nics.  # noqa: E501
+        :return: The type of this Servers.  # noqa: E501
         :rtype: Type
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this Nics.
+        """Sets the type of this Servers.
 
         The type of object that has been created.  # noqa: E501
 
-        :param type: The type of this Nics.  # noqa: E501
+        :param type: The type of this Servers.  # noqa: E501
         :type type: Type
         """
 
         self._type = type
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -285,18 +285,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Nics):
+        if not isinstance(other, Servers):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Nics):
+        if not isinstance(other, Servers):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.6/ionoscloud/models/no_state_meta_data.py` & `ionoscloud-6.1.7/ionoscloud/models/no_state_meta_data.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/pagination_links.py` & `ionoscloud-6.1.7/ionoscloud/models/pagination_links.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/peer.py` & `ionoscloud-6.1.7/ionoscloud/models/peer.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/private_cross_connect.py` & `ionoscloud-6.1.7/ionoscloud/models/private_cross_connect.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/private_cross_connect_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/private_cross_connect_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/private_cross_connects.py` & `ionoscloud-6.1.7/ionoscloud/models/private_cross_connects.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/remote_console_url.py` & `ionoscloud-6.1.7/ionoscloud/models/remote_console_url.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/request.py` & `ionoscloud-6.1.7/ionoscloud/models/request.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/request_metadata.py` & `ionoscloud-6.1.7/ionoscloud/models/request_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/request_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/request_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/request_status.py` & `ionoscloud-6.1.7/ionoscloud/models/request_status.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/request_status_metadata.py` & `ionoscloud-6.1.7/ionoscloud/models/request_status_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/request_target.py` & `ionoscloud-6.1.7/ionoscloud/models/request_target.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/requests.py` & `ionoscloud-6.1.7/ionoscloud/models/requests.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/resource.py` & `ionoscloud-6.1.7/ionoscloud/models/resource.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/resource_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/resource_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/resource_groups.py` & `ionoscloud-6.1.7/ionoscloud/models/resource_groups.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/resource_limits.py` & `ionoscloud-6.1.7/ionoscloud/models/resource_limits.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/resource_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/resource_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/resource_reference.py` & `ionoscloud-6.1.7/ionoscloud/models/resource_reference.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/resources.py` & `ionoscloud-6.1.7/ionoscloud/models/resources.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/resources_users.py` & `ionoscloud-6.1.7/ionoscloud/models/resources_users.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/s3_bucket.py` & `ionoscloud-6.1.7/ionoscloud/models/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/s3_key.py` & `ionoscloud-6.1.7/ionoscloud/models/s3_key.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/s3_key_metadata.py` & `ionoscloud-6.1.7/ionoscloud/models/s3_key_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/s3_key_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/s3_key_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/s3_keys.py` & `ionoscloud-6.1.7/ionoscloud/models/s3_keys.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/s3_object_storage_sso.py` & `ionoscloud-6.1.7/ionoscloud/models/s3_object_storage_sso.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/server.py` & `ionoscloud-6.1.7/ionoscloud/models/server.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/server_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/server_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/server_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/target_group_properties.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class ServerProperties(object):
+class TargetGroupProperties(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,335 +30,218 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'availability_zone': 'str',
+        'algorithm': 'str',
 
-        'boot_cdrom': 'ResourceReference',
+        'health_check': 'TargetGroupHealthCheck',
 
-        'boot_volume': 'ResourceReference',
-
-        'cores': 'int',
-
-        'cpu_family': 'str',
+        'http_health_check': 'TargetGroupHttpHealthCheck',
 
         'name': 'str',
 
-        'ram': 'int',
-
-        'template_uuid': 'str',
-
-        'type': 'str',
+        'protocol': 'str',
 
-        'vm_state': 'str',
+        'targets': 'list[TargetGroupTarget]',
     }
 
     attribute_map = {
 
-        'availability_zone': 'availabilityZone',
+        'algorithm': 'algorithm',
 
-        'boot_cdrom': 'bootCdrom',
+        'health_check': 'healthCheck',
 
-        'boot_volume': 'bootVolume',
-
-        'cores': 'cores',
-
-        'cpu_family': 'cpuFamily',
+        'http_health_check': 'httpHealthCheck',
 
         'name': 'name',
 
-        'ram': 'ram',
-
-        'template_uuid': 'templateUuid',
+        'protocol': 'protocol',
 
-        'type': 'type',
-
-        'vm_state': 'vmState',
+        'targets': 'targets',
     }
 
-    def __init__(self, availability_zone=None, boot_cdrom=None, boot_volume=None, cores=None, cpu_family=None, name=None, ram=None, template_uuid=None, type=None, vm_state=None, local_vars_configuration=None):  # noqa: E501
-        """ServerProperties - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, algorithm=None, health_check=None, http_health_check=None, name=None, protocol=None, targets=None, local_vars_configuration=None):  # noqa: E501
+        """TargetGroupProperties - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._availability_zone = None
-        self._boot_cdrom = None
-        self._boot_volume = None
-        self._cores = None
-        self._cpu_family = None
+        self._algorithm = None
+        self._health_check = None
+        self._http_health_check = None
         self._name = None
-        self._ram = None
-        self._template_uuid = None
-        self._type = None
-        self._vm_state = None
+        self._protocol = None
+        self._targets = None
         self.discriminator = None
 
-        if availability_zone is not None:
-            self.availability_zone = availability_zone
-        if boot_cdrom is not None:
-            self.boot_cdrom = boot_cdrom
-        if boot_volume is not None:
-            self.boot_volume = boot_volume
-        if cores is not None:
-            self.cores = cores
-        if cpu_family is not None:
-            self.cpu_family = cpu_family
-        if name is not None:
-            self.name = name
-        if ram is not None:
-            self.ram = ram
-        if template_uuid is not None:
-            self.template_uuid = template_uuid
-        if type is not None:
-            self.type = type
-        if vm_state is not None:
-            self.vm_state = vm_state
+        self.algorithm = algorithm
+        if health_check is not None:
+            self.health_check = health_check
+        if http_health_check is not None:
+            self.http_health_check = http_health_check
+        self.name = name
+        self.protocol = protocol
+        if targets is not None:
+            self.targets = targets
 
 
     @property
-    def availability_zone(self):
-        """Gets the availability_zone of this ServerProperties.  # noqa: E501
+    def algorithm(self):
+        """Gets the algorithm of this TargetGroupProperties.  # noqa: E501
 
-        The availability zone in which the server should be provisioned.  # noqa: E501
+        The balancing algorithm. A balancing algorithm consists of predefined rules with the logic that a load balancer uses to distribute network traffic between servers.  - **Round Robin**: Targets are served alternately according to their weighting.  - **Least Connection**: The target with the least active connection is served.  - **Random**: The targets are served based on a consistent pseudorandom algorithm.  - **Source IP**: It is ensured that the same client IP address reaches the same target.  # noqa: E501
 
-        :return: The availability_zone of this ServerProperties.  # noqa: E501
+        :return: The algorithm of this TargetGroupProperties.  # noqa: E501
         :rtype: str
         """
-        return self._availability_zone
+        return self._algorithm
 
-    @availability_zone.setter
-    def availability_zone(self, availability_zone):
-        """Sets the availability_zone of this ServerProperties.
+    @algorithm.setter
+    def algorithm(self, algorithm):
+        """Sets the algorithm of this TargetGroupProperties.
 
-        The availability zone in which the server should be provisioned.  # noqa: E501
+        The balancing algorithm. A balancing algorithm consists of predefined rules with the logic that a load balancer uses to distribute network traffic between servers.  - **Round Robin**: Targets are served alternately according to their weighting.  - **Least Connection**: The target with the least active connection is served.  - **Random**: The targets are served based on a consistent pseudorandom algorithm.  - **Source IP**: It is ensured that the same client IP address reaches the same target.  # noqa: E501
 
-        :param availability_zone: The availability_zone of this ServerProperties.  # noqa: E501
-        :type availability_zone: str
+        :param algorithm: The algorithm of this TargetGroupProperties.  # noqa: E501
+        :type algorithm: str
         """
-        allowed_values = ["AUTO", "ZONE_1", "ZONE_2"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and availability_zone not in allowed_values:  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and algorithm is None:  # noqa: E501
+            raise ValueError("Invalid value for `algorithm`, must not be `None`")  # noqa: E501
+        allowed_values = ["ROUND_ROBIN", "LEAST_CONNECTION", "RANDOM", "SOURCE_IP"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and algorithm not in allowed_values:  # noqa: E501
             raise ValueError(
-                "Invalid value for `availability_zone` ({0}), must be one of {1}"  # noqa: E501
-                .format(availability_zone, allowed_values)
+                "Invalid value for `algorithm` ({0}), must be one of {1}"  # noqa: E501
+                .format(algorithm, allowed_values)
             )
 
-        self._availability_zone = availability_zone
-
-    @property
-    def boot_cdrom(self):
-        """Gets the boot_cdrom of this ServerProperties.  # noqa: E501
-
-
-        :return: The boot_cdrom of this ServerProperties.  # noqa: E501
-        :rtype: ResourceReference
-        """
-        return self._boot_cdrom
-
-    @boot_cdrom.setter
-    def boot_cdrom(self, boot_cdrom):
-        """Sets the boot_cdrom of this ServerProperties.
-
-
-        :param boot_cdrom: The boot_cdrom of this ServerProperties.  # noqa: E501
-        :type boot_cdrom: ResourceReference
-        """
-
-        self._boot_cdrom = boot_cdrom
+        self._algorithm = algorithm
 
     @property
-    def boot_volume(self):
-        """Gets the boot_volume of this ServerProperties.  # noqa: E501
+    def health_check(self):
+        """Gets the health_check of this TargetGroupProperties.  # noqa: E501
 
 
-        :return: The boot_volume of this ServerProperties.  # noqa: E501
-        :rtype: ResourceReference
+        :return: The health_check of this TargetGroupProperties.  # noqa: E501
+        :rtype: TargetGroupHealthCheck
         """
-        return self._boot_volume
+        return self._health_check
 
-    @boot_volume.setter
-    def boot_volume(self, boot_volume):
-        """Sets the boot_volume of this ServerProperties.
+    @health_check.setter
+    def health_check(self, health_check):
+        """Sets the health_check of this TargetGroupProperties.
 
 
-        :param boot_volume: The boot_volume of this ServerProperties.  # noqa: E501
-        :type boot_volume: ResourceReference
+        :param health_check: The health_check of this TargetGroupProperties.  # noqa: E501
+        :type health_check: TargetGroupHealthCheck
         """
 
-        self._boot_volume = boot_volume
+        self._health_check = health_check
 
     @property
-    def cores(self):
-        """Gets the cores of this ServerProperties.  # noqa: E501
+    def http_health_check(self):
+        """Gets the http_health_check of this TargetGroupProperties.  # noqa: E501
 
-        The total number of cores for the enterprise server.  # noqa: E501
 
-        :return: The cores of this ServerProperties.  # noqa: E501
-        :rtype: int
+        :return: The http_health_check of this TargetGroupProperties.  # noqa: E501
+        :rtype: TargetGroupHttpHealthCheck
         """
-        return self._cores
+        return self._http_health_check
 
-    @cores.setter
-    def cores(self, cores):
-        """Sets the cores of this ServerProperties.
+    @http_health_check.setter
+    def http_health_check(self, http_health_check):
+        """Sets the http_health_check of this TargetGroupProperties.
 
-        The total number of cores for the enterprise server.  # noqa: E501
 
-        :param cores: The cores of this ServerProperties.  # noqa: E501
-        :type cores: int
+        :param http_health_check: The http_health_check of this TargetGroupProperties.  # noqa: E501
+        :type http_health_check: TargetGroupHttpHealthCheck
         """
 
-        self._cores = cores
-
-    @property
-    def cpu_family(self):
-        """Gets the cpu_family of this ServerProperties.  # noqa: E501
-
-        CPU architecture on which server gets provisioned; not all CPU architectures are available in all datacenter regions; available CPU architectures can be retrieved from the datacenter resource; must not be provided for CUBE servers.  # noqa: E501
-
-        :return: The cpu_family of this ServerProperties.  # noqa: E501
-        :rtype: str
-        """
-        return self._cpu_family
-
-    @cpu_family.setter
-    def cpu_family(self, cpu_family):
-        """Sets the cpu_family of this ServerProperties.
-
-        CPU architecture on which server gets provisioned; not all CPU architectures are available in all datacenter regions; available CPU architectures can be retrieved from the datacenter resource; must not be provided for CUBE servers.  # noqa: E501
-
-        :param cpu_family: The cpu_family of this ServerProperties.  # noqa: E501
-        :type cpu_family: str
-        """
-
-        self._cpu_family = cpu_family
+        self._http_health_check = http_health_check
 
     @property
     def name(self):
-        """Gets the name of this ServerProperties.  # noqa: E501
+        """Gets the name of this TargetGroupProperties.  # noqa: E501
 
-        The name of the  resource.  # noqa: E501
+        The target group name.  # noqa: E501
 
-        :return: The name of this ServerProperties.  # noqa: E501
+        :return: The name of this TargetGroupProperties.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this ServerProperties.
+        """Sets the name of this TargetGroupProperties.
 
-        The name of the  resource.  # noqa: E501
+        The target group name.  # noqa: E501
 
-        :param name: The name of this ServerProperties.  # noqa: E501
+        :param name: The name of this TargetGroupProperties.  # noqa: E501
         :type name: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def ram(self):
-        """Gets the ram of this ServerProperties.  # noqa: E501
-
-        The memory size for the enterprise server in MB, such as 2048. Size must be specified in multiples of 256 MB with a minimum of 256 MB; however, if you set ramHotPlug to TRUE then you must use a minimum of 1024 MB. If you set the RAM size more than 240GB, then ramHotPlug will be set to FALSE and can not be set to TRUE unless RAM size not set to less than 240GB.  # noqa: E501
-
-        :return: The ram of this ServerProperties.  # noqa: E501
-        :rtype: int
-        """
-        return self._ram
-
-    @ram.setter
-    def ram(self, ram):
-        """Sets the ram of this ServerProperties.
-
-        The memory size for the enterprise server in MB, such as 2048. Size must be specified in multiples of 256 MB with a minimum of 256 MB; however, if you set ramHotPlug to TRUE then you must use a minimum of 1024 MB. If you set the RAM size more than 240GB, then ramHotPlug will be set to FALSE and can not be set to TRUE unless RAM size not set to less than 240GB.  # noqa: E501
-
-        :param ram: The ram of this ServerProperties.  # noqa: E501
-        :type ram: int
-        """
-
-        self._ram = ram
-
-    @property
-    def template_uuid(self):
-        """Gets the template_uuid of this ServerProperties.  # noqa: E501
+    def protocol(self):
+        """Gets the protocol of this TargetGroupProperties.  # noqa: E501
 
-        The ID of the template for creating a CUBE server; the available templates for CUBE servers can be found on the templates resource.  # noqa: E501
+        The forwarding protocol. Only the value 'HTTP' is allowed.  # noqa: E501
 
-        :return: The template_uuid of this ServerProperties.  # noqa: E501
+        :return: The protocol of this TargetGroupProperties.  # noqa: E501
         :rtype: str
         """
-        return self._template_uuid
+        return self._protocol
 
-    @template_uuid.setter
-    def template_uuid(self, template_uuid):
-        """Sets the template_uuid of this ServerProperties.
+    @protocol.setter
+    def protocol(self, protocol):
+        """Sets the protocol of this TargetGroupProperties.
 
-        The ID of the template for creating a CUBE server; the available templates for CUBE servers can be found on the templates resource.  # noqa: E501
+        The forwarding protocol. Only the value 'HTTP' is allowed.  # noqa: E501
 
-        :param template_uuid: The template_uuid of this ServerProperties.  # noqa: E501
-        :type template_uuid: str
-        """
-
-        self._template_uuid = template_uuid
-
-    @property
-    def type(self):
-        """Gets the type of this ServerProperties.  # noqa: E501
-
-        Server type: CUBE or ENTERPRISE.  # noqa: E501
-
-        :return: The type of this ServerProperties.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this ServerProperties.
-
-        Server type: CUBE or ENTERPRISE.  # noqa: E501
-
-        :param type: The type of this ServerProperties.  # noqa: E501
-        :type type: str
+        :param protocol: The protocol of this TargetGroupProperties.  # noqa: E501
+        :type protocol: str
         """
+        if self.local_vars_configuration.client_side_validation and protocol is None:  # noqa: E501
+            raise ValueError("Invalid value for `protocol`, must not be `None`")  # noqa: E501
+        allowed_values = ["HTTP"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and protocol not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `protocol` ({0}), must be one of {1}"  # noqa: E501
+                .format(protocol, allowed_values)
+            )
 
-        self._type = type
+        self._protocol = protocol
 
     @property
-    def vm_state(self):
-        """Gets the vm_state of this ServerProperties.  # noqa: E501
+    def targets(self):
+        """Gets the targets of this TargetGroupProperties.  # noqa: E501
 
-        Status of the virtual machine.  # noqa: E501
+        Array of items in the collection.  # noqa: E501
 
-        :return: The vm_state of this ServerProperties.  # noqa: E501
-        :rtype: str
+        :return: The targets of this TargetGroupProperties.  # noqa: E501
+        :rtype: list[TargetGroupTarget]
         """
-        return self._vm_state
+        return self._targets
 
-    @vm_state.setter
-    def vm_state(self, vm_state):
-        """Sets the vm_state of this ServerProperties.
+    @targets.setter
+    def targets(self, targets):
+        """Sets the targets of this TargetGroupProperties.
 
-        Status of the virtual machine.  # noqa: E501
+        Array of items in the collection.  # noqa: E501
 
-        :param vm_state: The vm_state of this ServerProperties.  # noqa: E501
-        :type vm_state: str
+        :param targets: The targets of this TargetGroupProperties.  # noqa: E501
+        :type targets: list[TargetGroupTarget]
         """
-        allowed_values = ["NOSTATE", "RUNNING", "BLOCKED", "PAUSED", "SHUTDOWN", "SHUTOFF", "CRASHED", "SUSPENDED"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and vm_state not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `vm_state` ({0}), must be one of {1}"  # noqa: E501
-                .format(vm_state, allowed_values)
-            )
 
-        self._vm_state = vm_state
+        self._targets = targets
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -385,18 +268,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ServerProperties):
+        if not isinstance(other, TargetGroupProperties):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ServerProperties):
+        if not isinstance(other, TargetGroupProperties):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.6/ionoscloud/models/snapshot.py` & `ionoscloud-6.1.7/ionoscloud/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/snapshot_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/snapshot_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/snapshots.py` & `ionoscloud-6.1.7/ionoscloud/models/snapshots.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/target_group.py` & `ionoscloud-6.1.7/ionoscloud/models/target_group.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/target_group_health_check.py` & `ionoscloud-6.1.7/ionoscloud/models/target_group_health_check.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/target_group_http_health_check.py` & `ionoscloud-6.1.7/ionoscloud/models/target_group_http_health_check.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/target_group_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/target_group_target.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class TargetGroupProperties(object):
+class TargetGroupTarget(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,218 +30,180 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'algorithm': 'str',
+        'health_check_enabled': 'bool',
 
-        'health_check': 'TargetGroupHealthCheck',
+        'ip': 'str',
 
-        'http_health_check': 'TargetGroupHttpHealthCheck',
+        'maintenance_enabled': 'bool',
 
-        'name': 'str',
+        'port': 'int',
 
-        'protocol': 'str',
-
-        'targets': 'list[TargetGroupTarget]',
+        'weight': 'int',
     }
 
     attribute_map = {
 
-        'algorithm': 'algorithm',
-
-        'health_check': 'healthCheck',
+        'health_check_enabled': 'healthCheckEnabled',
 
-        'http_health_check': 'httpHealthCheck',
+        'ip': 'ip',
 
-        'name': 'name',
+        'maintenance_enabled': 'maintenanceEnabled',
 
-        'protocol': 'protocol',
+        'port': 'port',
 
-        'targets': 'targets',
+        'weight': 'weight',
     }
 
-    def __init__(self, algorithm=None, health_check=None, http_health_check=None, name=None, protocol=None, targets=None, local_vars_configuration=None):  # noqa: E501
-        """TargetGroupProperties - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, health_check_enabled=None, ip=None, maintenance_enabled=None, port=None, weight=None, local_vars_configuration=None):  # noqa: E501
+        """TargetGroupTarget - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._algorithm = None
-        self._health_check = None
-        self._http_health_check = None
-        self._name = None
-        self._protocol = None
-        self._targets = None
+        self._health_check_enabled = None
+        self._ip = None
+        self._maintenance_enabled = None
+        self._port = None
+        self._weight = None
         self.discriminator = None
 
-        self.algorithm = algorithm
-        if health_check is not None:
-            self.health_check = health_check
-        if http_health_check is not None:
-            self.http_health_check = http_health_check
-        self.name = name
-        self.protocol = protocol
-        if targets is not None:
-            self.targets = targets
-
-
-    @property
-    def algorithm(self):
-        """Gets the algorithm of this TargetGroupProperties.  # noqa: E501
-
-        The balancing algorithm. A balancing algorithm consists of predefined rules with the logic that a load balancer uses to distribute network traffic between servers.  - **Round Robin**: Targets are served alternately according to their weighting.  - **Least Connection**: The target with the least active connection is served.  - **Random**: The targets are served based on a consistent pseudorandom algorithm.  - **Source IP**: It is ensured that the same client IP address reaches the same target.  # noqa: E501
-
-        :return: The algorithm of this TargetGroupProperties.  # noqa: E501
-        :rtype: str
-        """
-        return self._algorithm
-
-    @algorithm.setter
-    def algorithm(self, algorithm):
-        """Sets the algorithm of this TargetGroupProperties.
-
-        The balancing algorithm. A balancing algorithm consists of predefined rules with the logic that a load balancer uses to distribute network traffic between servers.  - **Round Robin**: Targets are served alternately according to their weighting.  - **Least Connection**: The target with the least active connection is served.  - **Random**: The targets are served based on a consistent pseudorandom algorithm.  - **Source IP**: It is ensured that the same client IP address reaches the same target.  # noqa: E501
-
-        :param algorithm: The algorithm of this TargetGroupProperties.  # noqa: E501
-        :type algorithm: str
-        """
-        if self.local_vars_configuration.client_side_validation and algorithm is None:  # noqa: E501
-            raise ValueError("Invalid value for `algorithm`, must not be `None`")  # noqa: E501
-        allowed_values = ["ROUND_ROBIN", "LEAST_CONNECTION", "RANDOM", "SOURCE_IP"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and algorithm not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `algorithm` ({0}), must be one of {1}"  # noqa: E501
-                .format(algorithm, allowed_values)
-            )
+        if health_check_enabled is not None:
+            self.health_check_enabled = health_check_enabled
+        self.ip = ip
+        if maintenance_enabled is not None:
+            self.maintenance_enabled = maintenance_enabled
+        self.port = port
+        self.weight = weight
 
-        self._algorithm = algorithm
 
     @property
-    def health_check(self):
-        """Gets the health_check of this TargetGroupProperties.  # noqa: E501
+    def health_check_enabled(self):
+        """Gets the health_check_enabled of this TargetGroupTarget.  # noqa: E501
 
+        When the health check is enabled, the target is available only when it accepts regular TCP or HTTP connection attempts for state checking. The state check consists of one connection attempt with the target's address and port. The default value is 'TRUE'.  # noqa: E501
 
-        :return: The health_check of this TargetGroupProperties.  # noqa: E501
-        :rtype: TargetGroupHealthCheck
+        :return: The health_check_enabled of this TargetGroupTarget.  # noqa: E501
+        :rtype: bool
         """
-        return self._health_check
+        return self._health_check_enabled
 
-    @health_check.setter
-    def health_check(self, health_check):
-        """Sets the health_check of this TargetGroupProperties.
+    @health_check_enabled.setter
+    def health_check_enabled(self, health_check_enabled):
+        """Sets the health_check_enabled of this TargetGroupTarget.
 
+        When the health check is enabled, the target is available only when it accepts regular TCP or HTTP connection attempts for state checking. The state check consists of one connection attempt with the target's address and port. The default value is 'TRUE'.  # noqa: E501
 
-        :param health_check: The health_check of this TargetGroupProperties.  # noqa: E501
-        :type health_check: TargetGroupHealthCheck
+        :param health_check_enabled: The health_check_enabled of this TargetGroupTarget.  # noqa: E501
+        :type health_check_enabled: bool
         """
 
-        self._health_check = health_check
+        self._health_check_enabled = health_check_enabled
 
     @property
-    def http_health_check(self):
-        """Gets the http_health_check of this TargetGroupProperties.  # noqa: E501
+    def ip(self):
+        """Gets the ip of this TargetGroupTarget.  # noqa: E501
 
+        The IP address of the balanced target.  # noqa: E501
 
-        :return: The http_health_check of this TargetGroupProperties.  # noqa: E501
-        :rtype: TargetGroupHttpHealthCheck
+        :return: The ip of this TargetGroupTarget.  # noqa: E501
+        :rtype: str
         """
-        return self._http_health_check
+        return self._ip
 
-    @http_health_check.setter
-    def http_health_check(self, http_health_check):
-        """Sets the http_health_check of this TargetGroupProperties.
+    @ip.setter
+    def ip(self, ip):
+        """Sets the ip of this TargetGroupTarget.
 
+        The IP address of the balanced target.  # noqa: E501
 
-        :param http_health_check: The http_health_check of this TargetGroupProperties.  # noqa: E501
-        :type http_health_check: TargetGroupHttpHealthCheck
+        :param ip: The ip of this TargetGroupTarget.  # noqa: E501
+        :type ip: str
         """
+        if self.local_vars_configuration.client_side_validation and ip is None:  # noqa: E501
+            raise ValueError("Invalid value for `ip`, must not be `None`")  # noqa: E501
 
-        self._http_health_check = http_health_check
+        self._ip = ip
 
     @property
-    def name(self):
-        """Gets the name of this TargetGroupProperties.  # noqa: E501
+    def maintenance_enabled(self):
+        """Gets the maintenance_enabled of this TargetGroupTarget.  # noqa: E501
 
-        The target group name.  # noqa: E501
+        When the maintenance mode is enabled, the target is prevented from receiving traffic; the default value is 'FALSE'.  # noqa: E501
 
-        :return: The name of this TargetGroupProperties.  # noqa: E501
-        :rtype: str
+        :return: The maintenance_enabled of this TargetGroupTarget.  # noqa: E501
+        :rtype: bool
         """
-        return self._name
+        return self._maintenance_enabled
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this TargetGroupProperties.
+    @maintenance_enabled.setter
+    def maintenance_enabled(self, maintenance_enabled):
+        """Sets the maintenance_enabled of this TargetGroupTarget.
 
-        The target group name.  # noqa: E501
+        When the maintenance mode is enabled, the target is prevented from receiving traffic; the default value is 'FALSE'.  # noqa: E501
 
-        :param name: The name of this TargetGroupProperties.  # noqa: E501
-        :type name: str
+        :param maintenance_enabled: The maintenance_enabled of this TargetGroupTarget.  # noqa: E501
+        :type maintenance_enabled: bool
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._maintenance_enabled = maintenance_enabled
 
     @property
-    def protocol(self):
-        """Gets the protocol of this TargetGroupProperties.  # noqa: E501
+    def port(self):
+        """Gets the port of this TargetGroupTarget.  # noqa: E501
 
-        The forwarding protocol. Only the value 'HTTP' is allowed.  # noqa: E501
+        The port of the balanced target service; the valid range is 1 to 65535.  # noqa: E501
 
-        :return: The protocol of this TargetGroupProperties.  # noqa: E501
-        :rtype: str
+        :return: The port of this TargetGroupTarget.  # noqa: E501
+        :rtype: int
         """
-        return self._protocol
+        return self._port
 
-    @protocol.setter
-    def protocol(self, protocol):
-        """Sets the protocol of this TargetGroupProperties.
+    @port.setter
+    def port(self, port):
+        """Sets the port of this TargetGroupTarget.
 
-        The forwarding protocol. Only the value 'HTTP' is allowed.  # noqa: E501
+        The port of the balanced target service; the valid range is 1 to 65535.  # noqa: E501
 
-        :param protocol: The protocol of this TargetGroupProperties.  # noqa: E501
-        :type protocol: str
+        :param port: The port of this TargetGroupTarget.  # noqa: E501
+        :type port: int
         """
-        if self.local_vars_configuration.client_side_validation and protocol is None:  # noqa: E501
-            raise ValueError("Invalid value for `protocol`, must not be `None`")  # noqa: E501
-        allowed_values = ["HTTP"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and protocol not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `protocol` ({0}), must be one of {1}"  # noqa: E501
-                .format(protocol, allowed_values)
-            )
+        if self.local_vars_configuration.client_side_validation and port is None:  # noqa: E501
+            raise ValueError("Invalid value for `port`, must not be `None`")  # noqa: E501
 
-        self._protocol = protocol
+        self._port = port
 
     @property
-    def targets(self):
-        """Gets the targets of this TargetGroupProperties.  # noqa: E501
+    def weight(self):
+        """Gets the weight of this TargetGroupTarget.  # noqa: E501
 
-        Array of items in the collection.  # noqa: E501
+        The traffic is distributed proportionally to target weight, which is the ratio of the total weight of all targets. A target with higher weight receives a larger share of traffic. The valid range is from 0 to 256; the default value is '1'. Targets with a weight of '0' do not participate in load balancing but still accept persistent connections. We recommend using values in the middle range to leave room for later adjustments.  # noqa: E501
 
-        :return: The targets of this TargetGroupProperties.  # noqa: E501
-        :rtype: list[TargetGroupTarget]
+        :return: The weight of this TargetGroupTarget.  # noqa: E501
+        :rtype: int
         """
-        return self._targets
+        return self._weight
 
-    @targets.setter
-    def targets(self, targets):
-        """Sets the targets of this TargetGroupProperties.
+    @weight.setter
+    def weight(self, weight):
+        """Sets the weight of this TargetGroupTarget.
 
-        Array of items in the collection.  # noqa: E501
+        The traffic is distributed proportionally to target weight, which is the ratio of the total weight of all targets. A target with higher weight receives a larger share of traffic. The valid range is from 0 to 256; the default value is '1'. Targets with a weight of '0' do not participate in load balancing but still accept persistent connections. We recommend using values in the middle range to leave room for later adjustments.  # noqa: E501
 
-        :param targets: The targets of this TargetGroupProperties.  # noqa: E501
-        :type targets: list[TargetGroupTarget]
+        :param weight: The weight of this TargetGroupTarget.  # noqa: E501
+        :type weight: int
         """
+        if self.local_vars_configuration.client_side_validation and weight is None:  # noqa: E501
+            raise ValueError("Invalid value for `weight`, must not be `None`")  # noqa: E501
 
-        self._targets = targets
+        self._weight = weight
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -268,18 +230,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TargetGroupProperties):
+        if not isinstance(other, TargetGroupTarget):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TargetGroupProperties):
+        if not isinstance(other, TargetGroupTarget):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.6/ionoscloud/models/target_group_put.py` & `ionoscloud-6.1.7/ionoscloud/models/target_group_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/target_group_target.py` & `ionoscloud-6.1.7/ionoscloud/models/lan_properties.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class TargetGroupTarget(object):
+class LanProperties(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,180 +30,176 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'health_check_enabled': 'bool',
+        'ip_failover': 'list[IPFailover]',
 
-        'ip': 'str',
+        'ipv6_cidr_block': 'str',
 
-        'maintenance_enabled': 'bool',
+        'name': 'str',
 
-        'port': 'int',
+        'pcc': 'str',
 
-        'weight': 'int',
+        'public': 'bool',
     }
 
     attribute_map = {
 
-        'health_check_enabled': 'healthCheckEnabled',
+        'ip_failover': 'ipFailover',
 
-        'ip': 'ip',
+        'ipv6_cidr_block': 'ipv6CidrBlock',
 
-        'maintenance_enabled': 'maintenanceEnabled',
+        'name': 'name',
 
-        'port': 'port',
+        'pcc': 'pcc',
 
-        'weight': 'weight',
+        'public': 'public',
     }
 
-    def __init__(self, health_check_enabled=None, ip=None, maintenance_enabled=None, port=None, weight=None, local_vars_configuration=None):  # noqa: E501
-        """TargetGroupTarget - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, ip_failover=None, ipv6_cidr_block=None, name=None, pcc=None, public=None, local_vars_configuration=None):  # noqa: E501
+        """LanProperties - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._health_check_enabled = None
-        self._ip = None
-        self._maintenance_enabled = None
-        self._port = None
-        self._weight = None
+        self._ip_failover = None
+        self._ipv6_cidr_block = None
+        self._name = None
+        self._pcc = None
+        self._public = None
         self.discriminator = None
 
-        if health_check_enabled is not None:
-            self.health_check_enabled = health_check_enabled
-        self.ip = ip
-        if maintenance_enabled is not None:
-            self.maintenance_enabled = maintenance_enabled
-        self.port = port
-        self.weight = weight
+        if ip_failover is not None:
+            self.ip_failover = ip_failover
+        self.ipv6_cidr_block = ipv6_cidr_block
+        if name is not None:
+            self.name = name
+        if pcc is not None:
+            self.pcc = pcc
+        if public is not None:
+            self.public = public
 
 
     @property
-    def health_check_enabled(self):
-        """Gets the health_check_enabled of this TargetGroupTarget.  # noqa: E501
+    def ip_failover(self):
+        """Gets the ip_failover of this LanProperties.  # noqa: E501
 
-        When the health check is enabled, the target is available only when it accepts regular TCP or HTTP connection attempts for state checking. The state check consists of one connection attempt with the target's address and port. The default value is 'TRUE'.  # noqa: E501
+        IP failover configurations for lan  # noqa: E501
 
-        :return: The health_check_enabled of this TargetGroupTarget.  # noqa: E501
-        :rtype: bool
+        :return: The ip_failover of this LanProperties.  # noqa: E501
+        :rtype: list[IPFailover]
         """
-        return self._health_check_enabled
+        return self._ip_failover
 
-    @health_check_enabled.setter
-    def health_check_enabled(self, health_check_enabled):
-        """Sets the health_check_enabled of this TargetGroupTarget.
+    @ip_failover.setter
+    def ip_failover(self, ip_failover):
+        """Sets the ip_failover of this LanProperties.
 
-        When the health check is enabled, the target is available only when it accepts regular TCP or HTTP connection attempts for state checking. The state check consists of one connection attempt with the target's address and port. The default value is 'TRUE'.  # noqa: E501
+        IP failover configurations for lan  # noqa: E501
 
-        :param health_check_enabled: The health_check_enabled of this TargetGroupTarget.  # noqa: E501
-        :type health_check_enabled: bool
+        :param ip_failover: The ip_failover of this LanProperties.  # noqa: E501
+        :type ip_failover: list[IPFailover]
         """
 
-        self._health_check_enabled = health_check_enabled
+        self._ip_failover = ip_failover
 
     @property
-    def ip(self):
-        """Gets the ip of this TargetGroupTarget.  # noqa: E501
+    def ipv6_cidr_block(self):
+        """Gets the ipv6_cidr_block of this LanProperties.  # noqa: E501
 
-        The IP address of the balanced target.  # noqa: E501
+        [The IPv6 feature is in beta phase and not ready for production usage.] For a GET request, this value is either 'null' or contains the LAN's /64 IPv6 CIDR block if this LAN is IPv6 enabled. For POST/PUT/PATCH requests, 'AUTO' will result in enabling this LAN for IPv6 and automatically assign a /64 IPv6 CIDR block to this LAN and /80 IPv6 CIDR blocks to the NICs and one /128 IPv6 address to each connected NIC. If you choose the IPv6 CIDR block for the LAN on your own, then you must provide a /64 block, which is inside the IPv6 CIDR block of the virtual datacenter and unique inside all LANs from this virtual datacenter. If you enable IPv6 on a LAN with NICs, those NICs will get a /80 IPv6 CIDR block and one IPv6 address assigned to each automatically, unless you specify them explicitly on the LAN and on the NICs. A virtual data center is limited to a maximum of 256 IPv6-enabled LANs.  # noqa: E501
 
-        :return: The ip of this TargetGroupTarget.  # noqa: E501
+        :return: The ipv6_cidr_block of this LanProperties.  # noqa: E501
         :rtype: str
         """
-        return self._ip
+        return self._ipv6_cidr_block
 
-    @ip.setter
-    def ip(self, ip):
-        """Sets the ip of this TargetGroupTarget.
+    @ipv6_cidr_block.setter
+    def ipv6_cidr_block(self, ipv6_cidr_block):
+        """Sets the ipv6_cidr_block of this LanProperties.
 
-        The IP address of the balanced target.  # noqa: E501
+        [The IPv6 feature is in beta phase and not ready for production usage.] For a GET request, this value is either 'null' or contains the LAN's /64 IPv6 CIDR block if this LAN is IPv6 enabled. For POST/PUT/PATCH requests, 'AUTO' will result in enabling this LAN for IPv6 and automatically assign a /64 IPv6 CIDR block to this LAN and /80 IPv6 CIDR blocks to the NICs and one /128 IPv6 address to each connected NIC. If you choose the IPv6 CIDR block for the LAN on your own, then you must provide a /64 block, which is inside the IPv6 CIDR block of the virtual datacenter and unique inside all LANs from this virtual datacenter. If you enable IPv6 on a LAN with NICs, those NICs will get a /80 IPv6 CIDR block and one IPv6 address assigned to each automatically, unless you specify them explicitly on the LAN and on the NICs. A virtual data center is limited to a maximum of 256 IPv6-enabled LANs.  # noqa: E501
 
-        :param ip: The ip of this TargetGroupTarget.  # noqa: E501
-        :type ip: str
+        :param ipv6_cidr_block: The ipv6_cidr_block of this LanProperties.  # noqa: E501
+        :type ipv6_cidr_block: str
         """
-        if self.local_vars_configuration.client_side_validation and ip is None:  # noqa: E501
-            raise ValueError("Invalid value for `ip`, must not be `None`")  # noqa: E501
 
-        self._ip = ip
+        self._ipv6_cidr_block = ipv6_cidr_block
 
     @property
-    def maintenance_enabled(self):
-        """Gets the maintenance_enabled of this TargetGroupTarget.  # noqa: E501
+    def name(self):
+        """Gets the name of this LanProperties.  # noqa: E501
 
-        When the maintenance mode is enabled, the target is prevented from receiving traffic; the default value is 'FALSE'.  # noqa: E501
+        The name of the  resource.  # noqa: E501
 
-        :return: The maintenance_enabled of this TargetGroupTarget.  # noqa: E501
-        :rtype: bool
+        :return: The name of this LanProperties.  # noqa: E501
+        :rtype: str
         """
-        return self._maintenance_enabled
+        return self._name
 
-    @maintenance_enabled.setter
-    def maintenance_enabled(self, maintenance_enabled):
-        """Sets the maintenance_enabled of this TargetGroupTarget.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this LanProperties.
 
-        When the maintenance mode is enabled, the target is prevented from receiving traffic; the default value is 'FALSE'.  # noqa: E501
+        The name of the  resource.  # noqa: E501
 
-        :param maintenance_enabled: The maintenance_enabled of this TargetGroupTarget.  # noqa: E501
-        :type maintenance_enabled: bool
+        :param name: The name of this LanProperties.  # noqa: E501
+        :type name: str
         """
 
-        self._maintenance_enabled = maintenance_enabled
+        self._name = name
 
     @property
-    def port(self):
-        """Gets the port of this TargetGroupTarget.  # noqa: E501
+    def pcc(self):
+        """Gets the pcc of this LanProperties.  # noqa: E501
 
-        The port of the balanced target service; the valid range is 1 to 65535.  # noqa: E501
+        The unique identifier of the private Cross-Connect the LAN is connected to, if any.  # noqa: E501
 
-        :return: The port of this TargetGroupTarget.  # noqa: E501
-        :rtype: int
+        :return: The pcc of this LanProperties.  # noqa: E501
+        :rtype: str
         """
-        return self._port
+        return self._pcc
 
-    @port.setter
-    def port(self, port):
-        """Sets the port of this TargetGroupTarget.
+    @pcc.setter
+    def pcc(self, pcc):
+        """Sets the pcc of this LanProperties.
 
-        The port of the balanced target service; the valid range is 1 to 65535.  # noqa: E501
+        The unique identifier of the private Cross-Connect the LAN is connected to, if any.  # noqa: E501
 
-        :param port: The port of this TargetGroupTarget.  # noqa: E501
-        :type port: int
+        :param pcc: The pcc of this LanProperties.  # noqa: E501
+        :type pcc: str
         """
-        if self.local_vars_configuration.client_side_validation and port is None:  # noqa: E501
-            raise ValueError("Invalid value for `port`, must not be `None`")  # noqa: E501
 
-        self._port = port
+        self._pcc = pcc
 
     @property
-    def weight(self):
-        """Gets the weight of this TargetGroupTarget.  # noqa: E501
+    def public(self):
+        """Gets the public of this LanProperties.  # noqa: E501
 
-        The traffic is distributed proportionally to target weight, which is the ratio of the total weight of all targets. A target with higher weight receives a larger share of traffic. The valid range is from 0 to 256; the default value is '1'. Targets with a weight of '0' do not participate in load balancing but still accept persistent connections. We recommend using values in the middle range to leave room for later adjustments.  # noqa: E501
+        This LAN faces the public Internet.  # noqa: E501
 
-        :return: The weight of this TargetGroupTarget.  # noqa: E501
-        :rtype: int
+        :return: The public of this LanProperties.  # noqa: E501
+        :rtype: bool
         """
-        return self._weight
+        return self._public
 
-    @weight.setter
-    def weight(self, weight):
-        """Sets the weight of this TargetGroupTarget.
+    @public.setter
+    def public(self, public):
+        """Sets the public of this LanProperties.
 
-        The traffic is distributed proportionally to target weight, which is the ratio of the total weight of all targets. A target with higher weight receives a larger share of traffic. The valid range is from 0 to 256; the default value is '1'. Targets with a weight of '0' do not participate in load balancing but still accept persistent connections. We recommend using values in the middle range to leave room for later adjustments.  # noqa: E501
+        This LAN faces the public Internet.  # noqa: E501
 
-        :param weight: The weight of this TargetGroupTarget.  # noqa: E501
-        :type weight: int
+        :param public: The public of this LanProperties.  # noqa: E501
+        :type public: bool
         """
-        if self.local_vars_configuration.client_side_validation and weight is None:  # noqa: E501
-            raise ValueError("Invalid value for `weight`, must not be `None`")  # noqa: E501
 
-        self._weight = weight
+        self._public = public
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -230,18 +226,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TargetGroupTarget):
+        if not isinstance(other, LanProperties):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TargetGroupTarget):
+        if not isinstance(other, LanProperties):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.6/ionoscloud/models/target_groups.py` & `ionoscloud-6.1.7/ionoscloud/models/target_groups.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/target_port_range.py` & `ionoscloud-6.1.7/ionoscloud/models/target_port_range.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/template.py` & `ionoscloud-6.1.7/ionoscloud/models/template.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/template_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/template_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/templates.py` & `ionoscloud-6.1.7/ionoscloud/models/templates.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/token.py` & `ionoscloud-6.1.7/ionoscloud/models/token.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/type.py` & `ionoscloud-6.1.7/ionoscloud/models/type.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/user.py` & `ionoscloud-6.1.7/ionoscloud/models/user.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/user_metadata.py` & `ionoscloud-6.1.7/ionoscloud/models/user_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/user_post.py` & `ionoscloud-6.1.7/ionoscloud/models/user_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/user_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/user_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/user_properties_post.py` & `ionoscloud-6.1.7/ionoscloud/models/user_properties_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/user_properties_put.py` & `ionoscloud-6.1.7/ionoscloud/models/user_properties_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/user_put.py` & `ionoscloud-6.1.7/ionoscloud/models/user_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/users.py` & `ionoscloud-6.1.7/ionoscloud/models/users.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/users_entities.py` & `ionoscloud-6.1.7/ionoscloud/models/users_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/models/volume.py` & `ionoscloud-6.1.7/ionoscloud/models/volumes.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class Volume(object):
+class Volumes(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,170 +30,231 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
+        'links': 'PaginationLinks',
+
         'href': 'str',
 
         'id': 'str',
 
-        'metadata': 'DatacenterElementMetadata',
+        'items': 'list[Volume]',
+
+        'limit': 'float',
 
-        'properties': 'VolumeProperties',
+        'offset': 'float',
 
         'type': 'Type',
     }
 
     attribute_map = {
 
+        'links': '_links',
+
         'href': 'href',
 
         'id': 'id',
 
-        'metadata': 'metadata',
+        'items': 'items',
 
-        'properties': 'properties',
+        'limit': 'limit',
+
+        'offset': 'offset',
 
         'type': 'type',
     }
 
-    def __init__(self, href=None, id=None, metadata=None, properties=None, type=None, local_vars_configuration=None):  # noqa: E501
-        """Volume - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, links=None, href=None, id=None, items=None, limit=None, offset=None, type=None, local_vars_configuration=None):  # noqa: E501
+        """Volumes - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._links = None
         self._href = None
         self._id = None
-        self._metadata = None
-        self._properties = None
+        self._items = None
+        self._limit = None
+        self._offset = None
         self._type = None
         self.discriminator = None
 
+        if links is not None:
+            self.links = links
         if href is not None:
             self.href = href
         if id is not None:
             self.id = id
-        if metadata is not None:
-            self.metadata = metadata
-        self.properties = properties
+        if items is not None:
+            self.items = items
+        if limit is not None:
+            self.limit = limit
+        if offset is not None:
+            self.offset = offset
         if type is not None:
             self.type = type
 
 
     @property
+    def links(self):
+        """Gets the links of this Volumes.  # noqa: E501
+
+
+        :return: The links of this Volumes.  # noqa: E501
+        :rtype: PaginationLinks
+        """
+        return self._links
+
+    @links.setter
+    def links(self, links):
+        """Sets the links of this Volumes.
+
+
+        :param links: The links of this Volumes.  # noqa: E501
+        :type links: PaginationLinks
+        """
+
+        self._links = links
+
+    @property
     def href(self):
-        """Gets the href of this Volume.  # noqa: E501
+        """Gets the href of this Volumes.  # noqa: E501
 
-        The URL to the object representation (absolute path).  # noqa: E501
+        URL to the object representation (absolute path).  # noqa: E501
 
-        :return: The href of this Volume.  # noqa: E501
+        :return: The href of this Volumes.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
-        """Sets the href of this Volume.
+        """Sets the href of this Volumes.
 
-        The URL to the object representation (absolute path).  # noqa: E501
+        URL to the object representation (absolute path).  # noqa: E501
 
-        :param href: The href of this Volume.  # noqa: E501
+        :param href: The href of this Volumes.  # noqa: E501
         :type href: str
         """
 
         self._href = href
 
     @property
     def id(self):
-        """Gets the id of this Volume.  # noqa: E501
+        """Gets the id of this Volumes.  # noqa: E501
 
         The resource's unique identifier.  # noqa: E501
 
-        :return: The id of this Volume.  # noqa: E501
+        :return: The id of this Volumes.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this Volume.
+        """Sets the id of this Volumes.
 
         The resource's unique identifier.  # noqa: E501
 
-        :param id: The id of this Volume.  # noqa: E501
+        :param id: The id of this Volumes.  # noqa: E501
         :type id: str
         """
 
         self._id = id
 
     @property
-    def metadata(self):
-        """Gets the metadata of this Volume.  # noqa: E501
+    def items(self):
+        """Gets the items of this Volumes.  # noqa: E501
+
+        Array of items in the collection.  # noqa: E501
+
+        :return: The items of this Volumes.  # noqa: E501
+        :rtype: list[Volume]
+        """
+        return self._items
+
+    @items.setter
+    def items(self, items):
+        """Sets the items of this Volumes.
+
+        Array of items in the collection.  # noqa: E501
+
+        :param items: The items of this Volumes.  # noqa: E501
+        :type items: list[Volume]
+        """
+
+        self._items = items
+
+    @property
+    def limit(self):
+        """Gets the limit of this Volumes.  # noqa: E501
 
+        The limit (if specified in the request).  # noqa: E501
 
-        :return: The metadata of this Volume.  # noqa: E501
-        :rtype: DatacenterElementMetadata
+        :return: The limit of this Volumes.  # noqa: E501
+        :rtype: float
         """
-        return self._metadata
+        return self._limit
 
-    @metadata.setter
-    def metadata(self, metadata):
-        """Sets the metadata of this Volume.
+    @limit.setter
+    def limit(self, limit):
+        """Sets the limit of this Volumes.
 
+        The limit (if specified in the request).  # noqa: E501
 
-        :param metadata: The metadata of this Volume.  # noqa: E501
-        :type metadata: DatacenterElementMetadata
+        :param limit: The limit of this Volumes.  # noqa: E501
+        :type limit: float
         """
 
-        self._metadata = metadata
+        self._limit = limit
 
     @property
-    def properties(self):
-        """Gets the properties of this Volume.  # noqa: E501
+    def offset(self):
+        """Gets the offset of this Volumes.  # noqa: E501
 
+        The offset (if specified in the request).  # noqa: E501
 
-        :return: The properties of this Volume.  # noqa: E501
-        :rtype: VolumeProperties
+        :return: The offset of this Volumes.  # noqa: E501
+        :rtype: float
         """
-        return self._properties
+        return self._offset
 
-    @properties.setter
-    def properties(self, properties):
-        """Sets the properties of this Volume.
+    @offset.setter
+    def offset(self, offset):
+        """Sets the offset of this Volumes.
 
+        The offset (if specified in the request).  # noqa: E501
 
-        :param properties: The properties of this Volume.  # noqa: E501
-        :type properties: VolumeProperties
+        :param offset: The offset of this Volumes.  # noqa: E501
+        :type offset: float
         """
-        if self.local_vars_configuration.client_side_validation and properties is None:  # noqa: E501
-            raise ValueError("Invalid value for `properties`, must not be `None`")  # noqa: E501
 
-        self._properties = properties
+        self._offset = offset
 
     @property
     def type(self):
-        """Gets the type of this Volume.  # noqa: E501
+        """Gets the type of this Volumes.  # noqa: E501
 
         The type of object that has been created.  # noqa: E501
 
-        :return: The type of this Volume.  # noqa: E501
+        :return: The type of this Volumes.  # noqa: E501
         :rtype: Type
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this Volume.
+        """Sets the type of this Volumes.
 
         The type of object that has been created.  # noqa: E501
 
-        :param type: The type of this Volume.  # noqa: E501
+        :param type: The type of this Volumes.  # noqa: E501
         :type type: Type
         """
 
         self._type = type
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -224,18 +285,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Volume):
+        if not isinstance(other, Volumes):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Volume):
+        if not isinstance(other, Volumes):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.6/ionoscloud/models/volume_properties.py` & `ionoscloud-6.1.7/ionoscloud/models/volume_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud/rest.py` & `ionoscloud-6.1.7/ionoscloud/rest.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/ionoscloud.egg-info/PKG-INFO` & `ionoscloud-6.1.7/ionoscloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionoscloud
-Version: 6.1.6
+Version: 6.1.7
 Summary: Python SDK for the Ionos Cloud API
 Home-page: https://github.com/ionos-cloud/ionos-cloud-sdk-python
 Author: Ionos Cloud
 Author-email: sdk@cloud.ionos.com
 Keywords: OpenAPI,OpenAPI-Generator,CLOUD API
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
```

### Comparing `ionoscloud-6.1.6/ionoscloud.egg-info/SOURCES.txt` & `ionoscloud-6.1.7/ionoscloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.6/setup.py` & `ionoscloud-6.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from setuptools import setup  # noqa: H301
 import os
 import codecs
 
 NAME = "ionoscloud"
-VERSION = "6.1.6"
+VERSION = "6.1.7"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

