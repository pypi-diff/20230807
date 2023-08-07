# Comparing `tmp/hsds-0.7.0b11.tar.gz` & `tmp/hsds-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsds-0.7.0b11.tar", last modified: Mon Jan 24 22:26:24 2022, max compression
+gzip compressed data, was "hsds-0.8.0.tar", last modified: Mon Aug  7 16:32:06 2023, max compression
```

## Comparing `hsds-0.7.0b11.tar` & `hsds-0.8.0.tar`

### file list

```diff
@@ -1,316 +1,74 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.502730 hsds-0.7.0b11/
--rw-r--r--   0 john       (501) staff       (20)       69 2021-10-30 20:01:45.000000 hsds-0.7.0b11/.gitignore
--rw-r--r--   0 john       (501) staff       (20)      824 2021-10-30 20:01:45.000000 hsds-0.7.0b11/.travis.yml
--rwxr-xr-x   0 john       (501) staff       (20)     1237 2022-01-13 05:14:23.000000 hsds-0.7.0b11/Dockerfile
--rw-r--r--   0 john       (501) staff       (20)      676 2022-01-13 05:14:23.000000 hsds-0.7.0b11/Dockerfile.lambda
--rw-r--r--   0 john       (501) staff       (20)    11880 2021-10-30 20:01:45.000000 hsds-0.7.0b11/LICENSE
--rw-r--r--   0 john       (501) staff       (20)      690 2022-01-24 22:26:24.502194 hsds-0.7.0b11/PKG-INFO
--rwxr-xr-x   0 john       (501) staff       (20)     6075 2022-01-13 05:14:23.000000 hsds-0.7.0b11/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.263824 hsds-0.7.0b11/admin/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.283938 hsds-0.7.0b11/admin/aws/
--rwxr-xr-x   0 john       (501) staff       (20)     1855 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/aws/config.py
--rw-r--r--   0 john       (501) staff       (20)      850 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/aws/create_dynamodb_usrs.sh
--rw-r--r--   0 john       (501) staff       (20)     2814 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/aws/create_instance.py
--rwxr-xr-x   0 john       (501) staff       (20)     2922 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/aws/get_s3json.py
--rw-r--r--   0 john       (501) staff       (20)      877 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/aws/list_instances.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.291517 hsds-0.7.0b11/admin/config/
--rwxr-xr-x   0 john       (501) staff       (20)     6210 2022-01-20 04:45:13.000000 hsds-0.7.0b11/admin/config/config.yml
--rw-r--r--   0 john       (501) staff       (20)     1130 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/config/dump_config.py
--rw-r--r--   0 john       (501) staff       (20)      138 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/config/groups.default
--rw-r--r--   0 john       (501) staff       (20)      547 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/config/passwd.default
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.293712 hsds-0.7.0b11/admin/dcos/
--rwxr-xr-x   0 john       (501) staff       (20)     1356 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/dcos/dcos_dn.json
--rw-r--r--   0 john       (501) staff       (20)     1465 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/dcos/dcos_headnode.json
--rwxr-xr-x   0 john       (501) staff       (20)     1453 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/dcos/dcos_sn.json
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.297948 hsds-0.7.0b11/admin/docker/
--rw-r--r--   0 john       (501) staff       (20)     1685 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/docker/docker-compose-internal-lb.yml
--rw-r--r--   0 john       (501) staff       (20)     2145 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/docker/docker-compose.aws.yml
--rw-r--r--   0 john       (501) staff       (20)     1677 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/docker/docker-compose.azure.yml
--rw-r--r--   0 john       (501) staff       (20)     2169 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/docker/docker-compose.openio.yml
--rw-r--r--   0 john       (501) staff       (20)     1543 2022-01-05 01:04:22.000000 hsds-0.7.0b11/admin/docker/docker-compose.posix.yml
--rw-r--r--   0 john       (501) staff       (20)     2223 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/docker/docker-compose.yml
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.299948 hsds-0.7.0b11/admin/ecs/
--rw-r--r--   0 john       (501) staff       (20)     4246 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/ecs/README.md
--rwxr-xr-x   0 john       (501) staff       (20)     1317 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/ecs/buildecr.sh
--rwxr-xr-x   0 john       (501) staff       (20)     7529 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/ecs/runecs.sh
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.308347 hsds-0.7.0b11/admin/kubernetes/
--rw-r--r--   0 john       (501) staff       (20)     2356 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_deployment.yml
--rw-r--r--   0 john       (501) staff       (20)     2415 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_deployment_aws.yml
--rw-r--r--   0 john       (501) staff       (20)     6511 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_deployment_aws_singleton.yml
--rw-r--r--   0 john       (501) staff       (20)     2466 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_deployment_azure.yml
--rw-r--r--   0 john       (501) staff       (20)     1594 2021-11-05 00:03:31.000000 hsds-0.7.0b11/admin/kubernetes/k8s_deployment_posix.yml
--rwxr-xr-x   0 john       (501) staff       (20)      111 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_make_configmap.sh
--rwxr-xr-x   0 john       (501) staff       (20)     1373 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_make_secrets.sh
--rw-r--r--   0 john       (501) staff       (20)      405 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_rbac.yml
--rw-r--r--   0 john       (501) staff       (20)      152 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_service.yml
--rw-r--r--   0 john       (501) staff       (20)      665 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_service_lb.yml
--rw-r--r--   0 john       (501) staff       (20)      186 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/kubernetes/k8s_service_lb_azure.yml
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.312941 hsds-0.7.0b11/admin/systemd/
--rw-r--r--   0 john       (501) staff       (20)     1020 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/systemd/README.rst
--rw-r--r--   0 john       (501) staff       (20)      266 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/systemd/hsds_dn.service
--rw-r--r--   0 john       (501) staff       (20)      270 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/systemd/hsds_head.service
--rw-r--r--   0 john       (501) staff       (20)      266 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/systemd/hsds_sn.service
--rwxr-xr-x   0 john       (501) staff       (20)     1160 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/systemd/run.sh
--rwxr-xr-x   0 john       (501) staff       (20)       38 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/systemd/run_dn.sh
--rwxr-xr-x   0 john       (501) staff       (20)       42 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/systemd/run_head.sh
--rwxr-xr-x   0 john       (501) staff       (20)       38 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/systemd/run_sn.sh
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.313879 hsds-0.7.0b11/admin/tools/
--rwxr-xr-x   0 john       (501) staff       (20)     5914 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/tools/get_s3_stats.py
--rwxr-xr-x   0 john       (501) staff       (20)      437 2021-10-30 20:01:45.000000 hsds-0.7.0b11/admin/tools/run_cadvisor.sh
--rwxr-xr-x   0 john       (501) staff       (20)      857 2021-10-30 20:01:45.000000 hsds-0.7.0b11/build.sh
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.323122 hsds-0.7.0b11/docs/
--rw-r--r--   0 john       (501) staff       (20)     9744 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/authorization.md
--rw-r--r--   0 john       (501) staff       (20)     5785 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/aws_lambda_setup.md
--rw-r--r--   0 john       (501) staff       (20)     5611 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/azure_ad_setup.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.265771 hsds-0.7.0b11/docs/design/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.323645 hsds-0.7.0b11/docs/design/azure/
--rw-r--r--   0 john       (501) staff       (20)    10281 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/azure/azure.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.333637 hsds-0.7.0b11/docs/design/direct_access/
--rw-r--r--   0 john       (501) staff       (20)   201364 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/direct_access/diagram1.png
--rw-r--r--   0 john       (501) staff       (20)    52141 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/direct_access/diagrams.pptx
--rw-r--r--   0 john       (501) staff       (20)     9979 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/direct_access/direct_access.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.342383 hsds-0.7.0b11/docs/design/hsds_arch/
--rw-r--r--   0 john       (501) staff       (20)   131527 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/hsds_arch/authentication.png
--rw-r--r--   0 john       (501) staff       (20)    28003 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/hsds_arch/cluster_state.png
--rw-r--r--   0 john       (501) staff       (20)    36108 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/hsds_arch/dataset_selection.png
--rw-r--r--   0 john       (501) staff       (20)   103035 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/hsds_arch/dn_diagram.png
--rw-r--r--   0 john       (501) staff       (20)    24077 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/hsds_arch/hsds_arch.md
--rw-r--r--   0 john       (501) staff       (20)    24783 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/hsds_arch/hsds_arch.rst
--rw-r--r--   0 john       (501) staff       (20)    34885 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/hsds_arch/sn_diagram.png
--rw-r--r--   0 john       (501) staff       (20)   124150 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/hsds_arch/sys_diagram.png
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.345113 hsds-0.7.0b11/docs/design/kubernetes/
--rw-r--r--   0 john       (501) staff       (20)     7622 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/kubernetes/hsds_kubernetes.md
--rw-r--r--   0 john       (501) staff       (20)   274861 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/kubernetes/state_diagram.png
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.348457 hsds-0.7.0b11/docs/design/obj_store_schema/
--rw-r--r--   0 john       (501) staff       (20)    36487 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/obj_store_schema/obj_store_schema.rst
--rw-r--r--   0 john       (501) staff       (20)    35326 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/obj_store_schema/obj_store_schema_v2.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.349242 hsds-0.7.0b11/docs/design/operators/
--rw-r--r--   0 john       (501) staff       (20)     5450 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/operators/operators.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.350678 hsds-0.7.0b11/docs/design/query/
--rw-r--r--   0 john       (501) staff       (20)     4677 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/query/chunk_summary.md
--rw-r--r--   0 john       (501) staff       (20)     5972 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/query/md_query.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.351524 hsds-0.7.0b11/docs/design/rbac/
--rw-r--r--   0 john       (501) staff       (20)     4738 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/rbac/RBAC.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.352279 hsds-0.7.0b11/docs/design/single_object/
--rw-r--r--   0 john       (501) staff       (20)     6110 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/design/single_object/SingleObject.md
--rw-r--r--   0 john       (501) staff       (20)     3512 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/docker_install_aws.md
--rw-r--r--   0 john       (501) staff       (20)     5556 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/docker_install_azure.md
--rw-r--r--   0 john       (501) staff       (20)     2590 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/docker_install_dcos.md
--rw-r--r--   0 john       (501) staff       (20)     3082 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/docker_install_openio.md
--rw-r--r--   0 john       (501) staff       (20)     3456 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/docker_install_posix.md
--rw-r--r--   0 john       (501) staff       (20)     4287 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/frontdoor_install_azure.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.358508 hsds-0.7.0b11/docs/img/
--rw-r--r--   0 john       (501) staff       (20)   143834 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/img/Front_door1.jpg
--rw-r--r--   0 john       (501) staff       (20)   129892 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/img/Front_door2.jpg
--rw-r--r--   0 john       (501) staff       (20)   121360 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/img/Front_door3.jpg
--rw-r--r--   0 john       (501) staff       (20)   173532 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/img/Front_door4.jpg
--rw-r--r--   0 john       (501) staff       (20)     3935 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/keycloak_setup.md
--rw-r--r--   0 john       (501) staff       (20)     8894 2022-01-23 19:52:01.000000 hsds-0.7.0b11/docs/kubernetes_install_aws.md
--rw-r--r--   0 john       (501) staff       (20)    11499 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/kubernetes_install_azure.md
--rw-r--r--   0 john       (501) staff       (20)     4039 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/post_install.md
--rw-r--r--   0 john       (501) staff       (20)      734 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/setup_docker.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.382703 hsds-0.7.0b11/docs/usecases/
--rw-r--r--   0 john       (501) staff       (20)   116510 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/1d-1.png
--rw-r--r--   0 john       (501) staff       (20)   121866 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/1d-mny.png
--rw-r--r--   0 john       (501) staff       (20)   113538 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/2d-1.png
--rw-r--r--   0 john       (501) staff       (20)   118223 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/2d-2.png
--rw-r--r--   0 john       (501) staff       (20)    97100 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/3d-1.png
--rw-r--r--   0 john       (501) staff       (20)   114710 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/3d-2.png
--rw-r--r--   0 john       (501) staff       (20)      539 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/Makefile
--rw-r--r--   0 john       (501) staff       (20)     2736 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/extract_one_dimensional_subset.rst
--rw-r--r--   0 john       (501) staff       (20)     2795 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/extract_several_one_dimensional_subsets.rst
--rw-r--r--   0 john       (501) staff       (20)     3393 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/extract_subsets_with_shared_common_dimensions.rst
--rw-r--r--   0 john       (501) staff       (20)     3018 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/extract_three_dimensional_subset.rst
--rw-r--r--   0 john       (501) staff       (20)     2956 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/extract_two_dimensional_subset.rst
--rw-r--r--   0 john       (501) staff       (20)     4453 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/into.rst
--rw-r--r--   0 john       (501) staff       (20)   115228 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/layout.png
--rw-r--r--   0 john       (501) staff       (20)   337539 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/layoutmulti.png
--rw-r--r--   0 john       (501) staff       (20)   316676 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/layoutmultisub.png
--rw-r--r--   0 john       (501) staff       (20)     2087 2021-10-30 20:01:45.000000 hsds-0.7.0b11/docs/usecases/view_end-point_metadata.rst
--rwxr-xr-x   0 john       (501) staff       (20)      730 2021-10-30 20:01:45.000000 hsds-0.7.0b11/entrypoint.sh
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.406821 hsds-0.7.0b11/hsds/
--rw-r--r--   0 john       (501) staff       (20)        0 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     9454 2022-01-20 07:31:19.000000 hsds-0.7.0b11/hsds/app.py
--rwxr-xr-x   0 john       (501) staff       (20)    21211 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/async_lib.py
--rwxr-xr-x   0 john       (501) staff       (20)     8859 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/attr_dn.py
--rwxr-xr-x   0 john       (501) staff       (20)    26102 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/attr_sn.py
--rw-r--r--   0 john       (501) staff       (20)    24974 2022-01-14 21:44:44.000000 hsds-0.7.0b11/hsds/basenode.py
--rw-r--r--   0 john       (501) staff       (20)    19680 2022-01-13 05:14:23.000000 hsds-0.7.0b11/hsds/chunk_dn.py
--rwxr-xr-x   0 john       (501) staff       (20)    74186 2022-01-05 01:29:42.000000 hsds-0.7.0b11/hsds/chunk_sn.py
--rwxr-xr-x   0 john       (501) staff       (20)     6819 2022-01-20 07:13:54.000000 hsds-0.7.0b11/hsds/config.py
--rwxr-xr-x   0 john       (501) staff       (20)     5538 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/ctype_dn.py
--rwxr-xr-x   0 john       (501) staff       (20)    10341 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/ctype_sn.py
--rw-r--r--   0 john       (501) staff       (20)    14726 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/datanode.py
--rw-r--r--   0 john       (501) staff       (20)    36326 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/datanode_lib.py
--rwxr-xr-x   0 john       (501) staff       (20)     7187 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/domain_dn.py
--rwxr-xr-x   0 john       (501) staff       (20)    63055 2022-01-13 04:23:22.000000 hsds-0.7.0b11/hsds/domain_sn.py
--rwxr-xr-x   0 john       (501) staff       (20)     9395 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/dset_dn.py
--rwxr-xr-x   0 john       (501) staff       (20)    45051 2022-01-05 21:59:14.000000 hsds-0.7.0b11/hsds/dset_sn.py
--rwxr-xr-x   0 john       (501) staff       (20)     9694 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/group_dn.py
--rwxr-xr-x   0 john       (501) staff       (20)    10257 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/group_sn.py
--rwxr-xr-x   0 john       (501) staff       (20)    15805 2021-11-05 03:51:06.000000 hsds-0.7.0b11/hsds/headnode.py
--rw-r--r--   0 john       (501) staff       (20)    10885 2022-01-20 07:23:19.000000 hsds-0.7.0b11/hsds/hsds_app.py
--rw-r--r--   0 john       (501) staff       (20)     4934 2021-11-05 17:05:25.000000 hsds-0.7.0b11/hsds/hsds_logger.py
--rwxr-xr-x   0 john       (501) staff       (20)     8805 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/link_dn.py
--rwxr-xr-x   0 john       (501) staff       (20)    12960 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/link_sn.py
--rw-r--r--   0 john       (501) staff       (20)    11355 2021-11-05 03:51:17.000000 hsds-0.7.0b11/hsds/rangeget_proxy.py
--rwxr-xr-x   0 john       (501) staff       (20)    10236 2021-11-05 16:54:47.000000 hsds-0.7.0b11/hsds/servicenode.py
--rw-r--r--   0 john       (501) staff       (20)    11768 2021-12-15 01:21:40.000000 hsds-0.7.0b11/hsds/servicenode_lib.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.435040 hsds-0.7.0b11/hsds/util/
--rw-r--r--   0 john       (501) staff       (20)      884 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/__init__.py
--rw-r--r--   0 john       (501) staff       (20)    16483 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/arrayUtil.py
--rwxr-xr-x   0 john       (501) staff       (20)     2220 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/attrUtil.py
--rwxr-xr-x   0 john       (501) staff       (20)    24379 2022-01-07 01:11:06.000000 hsds-0.7.0b11/hsds/util/authUtil.py
--rw-r--r--   0 john       (501) staff       (20)     7013 2021-11-29 18:22:36.000000 hsds-0.7.0b11/hsds/util/awsLambdaClient.py
--rw-r--r--   0 john       (501) staff       (20)    23669 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/azureBlobClient.py
--rw-r--r--   0 john       (501) staff       (20)     7864 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/boolparser.py
--rw-r--r--   0 john       (501) staff       (20)    36503 2021-12-15 01:21:40.000000 hsds-0.7.0b11/hsds/util/chunkUtil.py
--rw-r--r--   0 john       (501) staff       (20)     8497 2022-01-13 04:23:06.000000 hsds-0.7.0b11/hsds/util/domainUtil.py
--rw-r--r--   0 john       (501) staff       (20)    23568 2022-01-05 22:07:21.000000 hsds-0.7.0b11/hsds/util/dsetUtil.py
--rw-r--r--   0 john       (501) staff       (20)    14517 2021-11-11 18:55:46.000000 hsds-0.7.0b11/hsds/util/fileClient.py
--rw-r--r--   0 john       (501) staff       (20)    28525 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/hdf5dtype.py
--rw-r--r--   0 john       (501) staff       (20)    16718 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/httpUtil.py
--rw-r--r--   0 john       (501) staff       (20)    15884 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/idUtil.py
--rw-r--r--   0 john       (501) staff       (20)     7935 2021-11-29 18:22:36.000000 hsds-0.7.0b11/hsds/util/jwtUtil.py
--rw-r--r--   0 john       (501) staff       (20)     8140 2022-01-13 05:14:23.000000 hsds-0.7.0b11/hsds/util/k8sClient.py
--rw-r--r--   0 john       (501) staff       (20)     1303 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/linkUtil.py
--rw-r--r--   0 john       (501) staff       (20)    13782 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/lruCache.py
--rw-r--r--   0 john       (501) staff       (20)     4548 2021-11-29 18:22:36.000000 hsds-0.7.0b11/hsds/util/query_marathon.py
--rw-r--r--   0 john       (501) staff       (20)    25485 2021-11-29 18:22:36.000000 hsds-0.7.0b11/hsds/util/s3Client.py
--rw-r--r--   0 john       (501) staff       (20)    15324 2022-01-05 21:57:53.000000 hsds-0.7.0b11/hsds/util/storUtil.py
--rwxr-xr-x   0 john       (501) staff       (20)     2264 2021-10-30 20:01:45.000000 hsds-0.7.0b11/hsds/util/timeUtil.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.409304 hsds-0.7.0b11/hsds.egg-info/
--rw-r--r--   0 john       (501) staff       (20)      690 2022-01-24 22:26:23.000000 hsds-0.7.0b11/hsds.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)     7440 2022-01-24 22:26:23.000000 hsds-0.7.0b11/hsds.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2022-01-24 22:26:23.000000 hsds-0.7.0b11/hsds.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)      192 2022-01-24 22:26:23.000000 hsds-0.7.0b11/hsds.egg-info/entry_points.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2021-10-30 20:03:45.000000 hsds-0.7.0b11/hsds.egg-info/not-zip-safe
--rw-r--r--   0 john       (501) staff       (20)      168 2022-01-24 22:26:23.000000 hsds-0.7.0b11/hsds.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        5 2022-01-24 22:26:23.000000 hsds-0.7.0b11/hsds.egg-info/top_level.txt
--rwxr-xr-x   0 john       (501) staff       (20)       49 2021-10-30 20:01:45.000000 hsds-0.7.0b11/lambda_build.sh
--rwxr-xr-x   0 john       (501) staff       (20)     8124 2022-01-14 21:39:19.000000 hsds-0.7.0b11/lambda_function.py
--rw-r--r--   0 john       (501) staff       (20)      429 2021-10-30 20:01:45.000000 hsds-0.7.0b11/local.env
--rw-r--r--   0 john       (501) staff       (20)    18543 2021-10-30 20:01:45.000000 hsds-0.7.0b11/nginx.tmpl
--rwxr-xr-x   0 john       (501) staff       (20)      553 2021-10-30 20:01:45.000000 hsds-0.7.0b11/pyflakes.sh
--rwxr-xr-x   0 john       (501) staff       (20)     1448 2021-10-30 20:01:45.000000 hsds-0.7.0b11/run_client.sh
--rwxr-xr-x   0 john       (501) staff       (20)     1003 2021-10-30 20:01:45.000000 hsds-0.7.0b11/run_openio.sh
--rwxr-xr-x   0 john       (501) staff       (20)     7195 2022-01-20 07:29:13.000000 hsds-0.7.0b11/runall.sh
--rw-r--r--   0 john       (501) staff       (20)       38 2022-01-24 22:26:24.502880 hsds-0.7.0b11/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)     1711 2022-01-24 22:14:48.000000 hsds-0.7.0b11/setup.py
--rwxr-xr-x   0 john       (501) staff       (20)      114 2021-10-30 20:01:45.000000 hsds-0.7.0b11/stopall.sh
--rwxr-xr-x   0 john       (501) staff       (20)     2389 2021-10-30 20:01:45.000000 hsds-0.7.0b11/testall.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.268893 hsds-0.7.0b11/tests/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.453317 hsds-0.7.0b11/tests/integ/
--rw-r--r--   0 john       (501) staff       (20)    14518 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/acl_test.py
--rw-r--r--   0 john       (501) staff       (20)    54739 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/attr_test.py
--rwxr-xr-x   0 john       (501) staff       (20)     1927 2022-01-13 05:14:23.000000 hsds-0.7.0b11/tests/integ/config.py
--rwxr-xr-x   0 john       (501) staff       (20)    87171 2022-01-05 22:12:42.000000 hsds-0.7.0b11/tests/integ/dataset_test.py
--rwxr-xr-x   0 john       (501) staff       (20)    15941 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/datatype_test.py
--rwxr-xr-x   0 john       (501) staff       (20)    54290 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/domain_test.py
--rwxr-xr-x   0 john       (501) staff       (20)    17846 2021-11-28 22:03:23.000000 hsds-0.7.0b11/tests/integ/group_test.py
--rw-r--r--   0 john       (501) staff       (20)     5293 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/headtest.py
--rw-r--r--   0 john       (501) staff       (20)     7935 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/helper.py
--rwxr-xr-x   0 john       (501) staff       (20)    21788 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/link_test.py
--rwxr-xr-x   0 john       (501) staff       (20)    43058 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/pointsel_test.py
--rw-r--r--   0 john       (501) staff       (20)    19741 2021-12-15 01:21:40.000000 hsds-0.7.0b11/tests/integ/query_test.py
--rwxr-xr-x   0 john       (501) staff       (20)     4667 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/rangeget_test.py
--rw-r--r--   0 john       (501) staff       (20)     4110 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/reqsize.py
--rw-r--r--   0 john       (501) staff       (20)     3011 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/sample-shuffle-data.json
--rwxr-xr-x   0 john       (501) staff       (20)     5133 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/setup_test.py
--rw-r--r--   0 john       (501) staff       (20)     7137 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/snp500.json
--rw-r--r--   0 john       (501) staff       (20)      647 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/tall.json
--rwxr-xr-x   0 john       (501) staff       (20)     3552 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/uptest.py
--rwxr-xr-x   0 john       (501) staff       (20)   123638 2022-01-13 05:14:23.000000 hsds-0.7.0b11/tests/integ/value_test.py
--rwxr-xr-x   0 john       (501) staff       (20)    19441 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/integ/vlen_test.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.454888 hsds-0.7.0b11/tests/lambda/
--rw-r--r--   0 john       (501) staff       (20)      580 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/lambda/config.yml
--rw-r--r--   0 john       (501) staff       (20)     1472 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/lambda/lambdaTest.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.267525 hsds-0.7.0b11/tests/load/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.461572 hsds-0.7.0b11/tests/load/kubeptwrite/
--rw-r--r--   0 john       (501) staff       (20)      216 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/Dockerfile
--rw-r--r--   0 john       (501) staff       (20)     2471 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/README.md
--rwxr-xr-x   0 john       (501) staff       (20)       44 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/build.sh
--rwxr-xr-x   0 john       (501) staff       (20)     3260 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/config.py
--rwxr-xr-x   0 john       (501) staff       (20)       55 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/entrypoint.sh
--rwxr-xr-x   0 john       (501) staff       (20)       54 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/getpods.sh
--rwxr-xr-x   0 john       (501) staff       (20)       36 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/killjob.sh
--rw-r--r--   0 john       (501) staff       (20)     4330 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/rand_write.py
--rwxr-xr-x   0 john       (501) staff       (20)      495 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/run.sh
--rw-r--r--   0 john       (501) staff       (20)     1301 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/run.yaml
--rwxr-xr-x   0 john       (501) staff       (20)       27 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/runjob.sh
--rw-r--r--   0 john       (501) staff       (20)     2503 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/setup.py
--rwxr-xr-x   0 john       (501) staff       (20)       39 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubeptwrite/viewjob.sh
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.468203 hsds-0.7.0b11/tests/load/kubewrite/
--rw-r--r--   0 john       (501) staff       (20)      217 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/Dockerfile
--rw-r--r--   0 john       (501) staff       (20)     2467 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/README.md
--rwxr-xr-x   0 john       (501) staff       (20)       42 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/build.sh
--rwxr-xr-x   0 john       (501) staff       (20)     3260 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/config.py
--rwxr-xr-x   0 john       (501) staff       (20)       56 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/entrypoint.sh
--rwxr-xr-x   0 john       (501) staff       (20)       52 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/getpods.sh
--rwxr-xr-x   0 john       (501) staff       (20)       34 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/killjob.sh
--rwxr-xr-x   0 john       (501) staff       (20)      493 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/run.sh
--rw-r--r--   0 john       (501) staff       (20)     1284 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/run.yaml
--rwxr-xr-x   0 john       (501) staff       (20)       27 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/runjob.sh
--rw-r--r--   0 john       (501) staff       (20)     2369 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/setup.py
--rwxr-xr-x   0 john       (501) staff       (20)       37 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/viewjob.sh
--rw-r--r--   0 john       (501) staff       (20)     4522 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/load/kubewrite/write_slice.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.268588 hsds-0.7.0b11/tests/perf/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.470157 hsds-0.7.0b11/tests/perf/append/
--rw-r--r--   0 john       (501) staff       (20)     3721 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/append/append_1d.py
--rw-r--r--   0 john       (501) staff       (20)    10068 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/append/append_1d_async.py
--rw-r--r--   0 john       (501) staff       (20)     2705 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/append/config.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.474737 hsds-0.7.0b11/tests/perf/async_http/
--rw-r--r--   0 john       (501) staff       (20)      482 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/async_http/README.md
--rw-r--r--   0 john       (501) staff       (20)     1247 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/async_http/async_batch_client.py
--rw-r--r--   0 john       (501) staff       (20)     1237 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/async_http/async_client.py
--rwxr-xr-x   0 john       (501) staff       (20)     1494 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/async_http/config.py
--rw-r--r--   0 john       (501) staff       (20)     1119 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/async_http/hello_srv.py
--rw-r--r--   0 john       (501) staff       (20)   261303 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/async_http/html_text.html
--rw-r--r--   0 john       (501) staff       (20)      289 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/async_http/sync_client.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.478131 hsds-0.7.0b11/tests/perf/mkgroups/
--rwxr-xr-x   0 john       (501) staff       (20)     1587 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/mkgroups/config.py
--rw-r--r--   0 john       (501) staff       (20)     3520 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/mkgroups/helper.py
--rw-r--r--   0 john       (501) staff       (20)     1700 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/mkgroups/hsds_logger.py
--rw-r--r--   0 john       (501) staff       (20)     8378 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/mkgroups/mkgroups.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.479777 hsds-0.7.0b11/tests/perf/nsrdb/
--rw-r--r--   0 john       (501) staff       (20)     2705 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/nsrdb/config.py
--rw-r--r--   0 john       (501) staff       (20)     9712 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/nsrdb/nsrdb_async.py
--rw-r--r--   0 john       (501) staff       (20)     2861 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/nsrdb/nsrdb_test.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.481952 hsds-0.7.0b11/tests/perf/socket/
--rw-r--r--   0 john       (501) staff       (20)     2197 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/socket/client.py
--rwxr-xr-x   0 john       (501) staff       (20)     1891 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/socket/config.py
--rw-r--r--   0 john       (501) staff       (20)     1166 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/socket/readme.md
--rw-r--r--   0 john       (501) staff       (20)     1805 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/socket/server.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.482531 hsds-0.7.0b11/tests/perf/wtk/
--rw-r--r--   0 john       (501) staff       (20)     3122 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/perf/wtk/wtk_test.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.491392 hsds-0.7.0b11/tests/unit/
--rw-r--r--   0 john       (501) staff       (20)    21223 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/unit/arrayUtilTest.py
--rwxr-xr-x   0 john       (501) staff       (20)     3761 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/unit/boolParserTest.py
--rwxr-xr-x   0 john       (501) staff       (20)    60680 2021-12-15 01:21:40.000000 hsds-0.7.0b11/tests/unit/chunkUtilTest.py
--rw-r--r--   0 john       (501) staff       (20)      164 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/unit/config.yml
--rwxr-xr-x   0 john       (501) staff       (20)     4815 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/unit/domainUtilTest.py
--rwxr-xr-x   0 john       (501) staff       (20)    12285 2021-12-15 01:21:40.000000 hsds-0.7.0b11/tests/unit/dsetUtilTest.py
--rwxr-xr-x   0 john       (501) staff       (20)    26968 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/unit/hdf5dtypeTest.py
--rwxr-xr-x   0 john       (501) staff       (20)     6997 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/unit/idUtilTest.py
--rwxr-xr-x   0 john       (501) staff       (20)    10609 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/unit/lruCacheTest.py
--rwxr-xr-x   0 john       (501) staff       (20)     2412 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/unit/shuffleTest.py
--rwxr-xr-x   0 john       (501) staff       (20)     9888 2021-11-29 18:22:36.000000 hsds-0.7.0b11/tests/unit/storUtilTest.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.494772 hsds-0.7.0b11/tests/util/
--rw-r--r--   0 john       (501) staff       (20)     2080 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/util/create_group_dn.py
--rw-r--r--   0 john       (501) staff       (20)     1701 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/util/delete_obj_dn.py
--rw-r--r--   0 john       (501) staff       (20)     1695 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/util/get_obj_dn.py
--rw-r--r--   0 john       (501) staff       (20)     2455 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/util/get_obj_sn.py
--rw-r--r--   0 john       (501) staff       (20)     2037 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/util/put_domain_dn.py
--rw-r--r--   0 john       (501) staff       (20)     2146 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tests/util/put_domain_sn.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-01-24 22:26:24.501242 hsds-0.7.0b11/tools/
--rwxr-xr-x   0 john       (501) staff       (20)     4504 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tools/bucket_check.py
--rwxr-xr-x   0 john       (501) staff       (20)     5153 2021-11-29 18:22:36.000000 hsds-0.7.0b11/tools/bucket_scan.py
--rwxr-xr-x   0 john       (501) staff       (20)     6812 2021-11-29 18:22:36.000000 hsds-0.7.0b11/tools/create_toplevel_domain_json.py
--rwxr-xr-x   0 john       (501) staff       (20)     2466 2021-11-29 18:22:36.000000 hsds-0.7.0b11/tools/delete_bucket.py
--rwxr-xr-x   0 john       (501) staff       (20)     2789 2021-11-29 18:22:36.000000 hsds-0.7.0b11/tools/get_s3json.py
--rw-r--r--   0 john       (501) staff       (20)     3346 2021-11-05 21:34:12.000000 hsds-0.7.0b11/tools/lambda_log_filter.py
--rwxr-xr-x   0 john       (501) staff       (20)     7423 2021-11-29 18:22:36.000000 hsds-0.7.0b11/tools/link_mod.py
--rwxr-xr-x   0 john       (501) staff       (20)     3591 2021-11-29 18:22:36.000000 hsds-0.7.0b11/tools/list_objects.py
--rwxr-xr-x   0 john       (501) staff       (20)     2318 2021-11-29 18:22:36.000000 hsds-0.7.0b11/tools/root_delete.py
--rwxr-xr-x   0 john       (501) staff       (20)     4305 2021-11-29 18:22:36.000000 hsds-0.7.0b11/tools/root_scan.py
--rw-r--r--   0 john       (501) staff       (20)      773 2021-10-30 20:01:45.000000 hsds-0.7.0b11/tools/status_check.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-07 16:32:06.480292 hsds-0.8.0/
+-rw-rw-r--   0 john      (1000) john      (1000)    11880 2023-07-12 12:33:17.000000 hsds-0.8.0/LICENSE
+-rw-rw-r--   0 john      (1000) john      (1000)       31 2023-07-12 12:33:17.000000 hsds-0.8.0/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)      670 2023-08-07 16:32:06.480292 hsds-0.8.0/PKG-INFO
+-rwxrwxr-x   0 john      (1000) john      (1000)     8675 2023-07-12 12:33:17.000000 hsds-0.8.0/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-07 16:32:06.476292 hsds-0.8.0/admin/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-12 12:33:17.000000 hsds-0.8.0/admin/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-07 16:32:06.476292 hsds-0.8.0/admin/config/
+-rwxrwxr-x   0 john      (1000) john      (1000)     7285 2023-07-12 12:33:17.000000 hsds-0.8.0/admin/config/config.yml
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-07 16:32:06.480292 hsds-0.8.0/hsds/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10917 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/app.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    21786 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/async_lib.py
+-rwxrwxr-x   0 john      (1000) john      (1000)     9784 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/attr_dn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    26688 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/attr_sn.py
+-rw-rw-r--   0 john      (1000) john      (1000)    24927 2023-08-07 16:21:32.000000 hsds-0.8.0/hsds/basenode.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    31410 2023-08-07 16:21:32.000000 hsds-0.8.0/hsds/chunk_crawl.py
+-rw-rw-r--   0 john      (1000) john      (1000)    25760 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/chunk_dn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    66647 2023-08-07 16:21:32.000000 hsds-0.8.0/hsds/chunk_sn.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7284 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/chunklocator.py
+-rwxrwxr-x   0 john      (1000) john      (1000)     6496 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/config.py
+-rwxrwxr-x   0 john      (1000) john      (1000)     5640 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/ctype_dn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    10640 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/ctype_sn.py
+-rw-rw-r--   0 john      (1000) john      (1000)    17217 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/datanode.py
+-rw-rw-r--   0 john      (1000) john      (1000)    51624 2023-08-07 16:21:32.000000 hsds-0.8.0/hsds/datanode_lib.py
+-rwxrwxr-x   0 john      (1000) john      (1000)     7185 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/domain_dn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    67088 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/domain_sn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)     9487 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/dset_dn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    44636 2023-08-07 16:21:32.000000 hsds-0.8.0/hsds/dset_sn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    10017 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/group_dn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    10746 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/group_sn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    15924 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/headnode.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14167 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/hsds_app.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4958 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/hsds_logger.py
+-rwxrwxr-x   0 john      (1000) john      (1000)     9800 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/link_dn.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    13200 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/link_sn.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1557 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/node_runner.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    10834 2023-07-27 09:29:53.000000 hsds-0.8.0/hsds/servicenode.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16864 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/servicenode_lib.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-07 16:32:06.480292 hsds-0.8.0/hsds/util/
+-rw-rw-r--   0 john      (1000) john      (1000)      884 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    20861 2023-08-07 16:21:32.000000 hsds-0.8.0/hsds/util/arrayUtil.py
+-rwxrwxr-x   0 john      (1000) john      (1000)     2210 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/attrUtil.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    24347 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/authUtil.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6966 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/awsLambdaClient.py
+-rw-rw-r--   0 john      (1000) john      (1000)    24176 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/azureBlobClient.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9732 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/boolparser.py
+-rw-rw-r--   0 john      (1000) john      (1000)    37717 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/chunkUtil.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8605 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/domainUtil.py
+-rw-rw-r--   0 john      (1000) john      (1000)    31676 2023-08-07 16:21:32.000000 hsds-0.8.0/hsds/util/dsetUtil.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15931 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/fileClient.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3915 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/globparser.py
+-rw-rw-r--   0 john      (1000) john      (1000)    28574 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/hdf5dtype.py
+-rw-rw-r--   0 john      (1000) john      (1000)    22520 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/httpUtil.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16144 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/idUtil.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7967 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/jwtUtil.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8654 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/k8sClient.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1558 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/linkUtil.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14196 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/lruCache.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4546 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/query_marathon.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3730 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/rangegetUtil.py
+-rw-rw-r--   0 john      (1000) john      (1000)    26417 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/s3Client.py
+-rw-rw-r--   0 john      (1000) john      (1000)    17643 2023-08-07 16:21:32.000000 hsds-0.8.0/hsds/util/storUtil.py
+-rwxrwxr-x   0 john      (1000) john      (1000)     2270 2023-07-12 12:33:17.000000 hsds-0.8.0/hsds/util/timeUtil.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-07 16:32:06.480292 hsds-0.8.0/hsds.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)      670 2023-08-07 16:32:06.000000 hsds-0.8.0/hsds.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     1358 2023-08-07 16:32:06.000000 hsds-0.8.0/hsds.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-08-07 16:32:06.000000 hsds-0.8.0/hsds.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      268 2023-08-07 16:32:06.000000 hsds-0.8.0/hsds.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-07-16 20:06:23.000000 hsds-0.8.0/hsds.egg-info/not-zip-safe
+-rw-rw-r--   0 john      (1000) john      (1000)      178 2023-08-07 16:32:06.000000 hsds-0.8.0/hsds.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       11 2023-08-07 16:32:06.000000 hsds-0.8.0/hsds.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      143 2023-08-07 16:32:06.480292 hsds-0.8.0/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     2225 2023-08-07 16:21:32.000000 hsds-0.8.0/setup.py
```

### Comparing `hsds-0.7.0b11/LICENSE` & `hsds-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hsds-0.7.0b11/PKG-INFO` & `hsds-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: hsds
-Version: 0.7.0b11
+Version: 0.8.0
 Summary: HDF REST API
 Home-page: http://github.com/HDFGroup/hsds
 Author: John Readey
 Author-email: jreadey@hdfgrouup.org
 License: Apache
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: azure
+License-File: LICENSE
```

### Comparing `hsds-0.7.0b11/admin/config/config.yml` & `hsds-0.8.0/admin/config/config.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,99 @@
 # HSDS configuration
-allow_noauth: true  # enable unauthenticated requests
+allow_noauth: true # enable unauthenticated requests
 auth_expiration: -1 # set an expiration for credential caching
 default_public: False # new domains are publically readable by default
-aws_access_key_id: xxx  # Replace with access key for account or use aws_iam_role
-aws_secret_access_key: xxx   # Replace with secret key for account
-aws_iam_role: hsds_role  # For EC2 using IAM roles
+aws_access_key_id: xxx # Replace with access key for account or use aws_iam_role
+aws_secret_access_key: xxx # Replace with secret key for account
+aws_iam_role: hsds_role # For EC2 using IAM roles
 aws_region: us-east-1
 hsds_endpoint: http://hsds.hdf.test # used for hateos links in response
-aws_s3_gateway: null   # use endpoint for the region HSDS is running in, e.g. 'https://s3.amazonaws.com' for us-east-1
+aws_s3_gateway: null # use endpoint for the region HSDS is running in, e.g. 'https://s3.amazonaws.com' for us-east-1
+aws_s3_no_sign_request: false # do not use credentials for S3 requests, equivalent of --no-sign-request for AWS CLI
 aws_dynamodb_gateway: null # use for dynamodb endpint, e.g. 'https://dynamodb.us-east-1.amazonaws.com',
 aws_dynamodb_users_table: null # set to table name if dynamodb is used to store usernames and passwords
 azure_connection_string: null # use for connecting to Azure blob storage
-azure_resource_id: null  # resource id for use with Azure Active Directory
-azure_storage_account: null  # storage account to use on Azure
-azure_resource_group: null  # Azure resource group the container (BUCKET_NAME) belongs to
-root_dir: null   # base directory to use for Posix storage
-password_salt: null  # salt value if dynamically generated passwords are used
-bucket_name: hsdstest  # set to use a default bucket, otherwise bucket param is needed for all requests
-head_port: 5100     # port to use for head node
-head_ram: 512m  # memory for head container
-dn_port: 6101  # Start dn ports at 6101
-dn_ram: 3g     # memory for DN container (per container)
-sn_port: 5101   # Start sn ports at 5101
-sn_ram: 1g     # memory for SN container
-rangeget_port: 6900  # singleton proxy at port 6900
-rangeget_ram: 2g  # memory for RANGEGET container 
-target_sn_count: 0  # desired number of SN containers
+azure_resource_id: null # resource id for use with Azure Active Directory
+azure_storage_account: null # storage account to use on Azure
+azure_resource_group: null # Azure resource group the container (BUCKET_NAME) belongs to
+root_dir: null # base directory to use for Posix storage
+password_salt: null # salt value to generate password based on username.  Not recommended for public deployments
+bucket_name: hsdstest # set to use a default bucket, otherwise bucket param is needed for all requests
+head_port: 5100 # port to use for head node
+head_ram: 512m # memory for head container
+dn_port: 6101 # Start dn ports at 6101
+dn_ram: 3g # memory for DN container (per container)
+sn_port: 5101 # Start sn ports at 5101
+sn_ram: 3g # memory for SN container
+target_sn_count: 0 # desired number of SN containers
 target_dn_count: 0 # desire number of DN containers
-log_level: INFO    # log level.  One of ERROR, WARNING, INFO, DEBUG 
+log_level: INFO    # log level.  One of ERROR, WARNING, INFO, DEBUG
 log_timestamps: false # emit timestamp with log messages
-log_prefix: null   # Prefix text to append to log entries
-max_tcp_connections: 100   # max number of inflight tcp connections
-head_sleep_time: 10  # max sleep time between health checks for head node
+log_prefix: null # Prefix text to append to log entries
+max_tcp_connections: 100 # max number of inflight tcp connections
+head_sleep_time: 10 # max sleep time between health checks for head node
 node_sleep_time: 10 # max sleep time between health checks for SN/DN nodes
-async_sleep_time: 10  # max sleep time between async task runs
-s3_sync_interval: 1  # time to wait to write object data to S3 (in sec)
-s3_sync_task_timeout: 10  # time to cancel write task if no response
-store_read_timeout: 1  # time to cancel storage read request if no response
-store_read_sleep_interval: 0.1  # time to sleep between checking on read request
-max_pending_write_requests: 20  # maxium number of inflight write requests
-flush_sleep_interval: 1  # time to wait between checking on dirty objects
-max_chunks_per_request: 1000  # maximum number of chunks to be serviced by one request
-min_chunk_size: 1m  # 1 MB
+async_sleep_time: 10 # max sleep time between async task runs
+s3_sync_interval: 1 # time to wait between s3_sync checks (in sec)
+s3_age_time: 1 # time to wait since last update to write an object to S3
+s3_sync_task_timeout: 10 # time to cancel write task if no response
+store_read_timeout: 1 # time to cancel storage read request if no response
+store_read_sleep_interval: 0.1 # time to sleep between checking on read request
+max_pending_write_requests: 20 # maxium number of inflight write requests
+flush_sleep_interval: 1 # time to wait between checking on dirty objects
+min_chunk_size: 1m # 1 MB
 max_chunk_size: 4m # 4 MB
-max_request_size: 100m  # 100 MB - should be no smaller than client_max_body_size in nginx tmpl
+max_request_size: 100m # 100 MB - should be no smaller than client_max_body_size in nginx tmpl (if using nginx)
 max_chunks_per_folder: 0 # max number of chunks per s3 folder. 0 for unlimiited
-max_task_count: 100  # maximum number of concurrent tasks before server will return 503 error
-aio_max_pool_connections: 64  # number of connections to keep in conection pool for aiobotocore requests
-metadata_mem_cache_size: 128m  # 128 MB - metadata cache size per DN node
-metadata_mem_cache_expire: 3600  # expire cache items after one hour
-chunk_mem_cache_size: 128m  # 128 MB - chunk cache size per DN node
-chunk_mem_cache_expire: 3600  # expire cache items after one hour
-data_cache_size: 128m  # cache for rangegets
-data_cache_max_req_size: 128k  # max size for rangeget fetches
-data_cache_expire_time: 3600  # expire cache items after one hour
-data_cache_page_size: 4m  # page size for range get cache, set to zero to disable proxy
-data_cache_max_concurrent_read: 16  # maximum number of inflight storage read requests
-timeout: 30     # http timeout - 30 sec
-password_file: /config/passwd.txt  # filepath to a text file of username/passwords. set to '' for no-auth access
-groups_file: /config/groups.txt     # filepath to text file defining user groups
-server_name: Highly Scalable Data Service (HSDS)  # this gets returned in the about request
+max_task_count: 100 # maximum number of concurrent tasks before server will return 503 error
+max_tasks_per_node_per_request: 16 # maximum number of inflight tasks to to each node per request
+aio_max_pool_connections: 64 # number of connections to keep in conection pool for aiobotocore requests
+client_pool_count: 10 # pool count for SessionClient
+metadata_mem_cache_size: 128m # 128 MB - metadata cache size per DN node
+metadata_mem_cache_expire: 3600 # expire cache items after one hour
+chunk_mem_cache_size: 128m # 128 MB - chunk cache size per DN node
+chunk_mem_cache_expire: 3600 # expire cache items after one hour
+timeout: 30 # http timeout - 30 sec
+password_file: /config/passwd.txt # filepath to a text file of username/passwords. set to '' for no-auth access
+groups_file: /config/groups.txt # filepath to text file defining user groups
+server_name: Highly Scalable Data Service (HSDS) # this gets returned in the about request
 greeting: Welcome to HSDS!
 about: HSDS is a webservice for HDF data
-top_level_domains: []  # list of possible top-level domains, example: ["/home", "/shared"], if empty all top-level folders in default bucket will be returned
-cors_domain: "*"     # domains allowed for CORS
-admin_user: admin  # user with admin privileges
-admin_group: null  # enable admin privileges for any user in this group
-openid_provider: azure  # OpenID authentication provider
+top_level_domains: [] # list of possible top-level domains, example: ["/home", "/shared"], if empty all top-level folders in default bucket will be returned
+cors_domain: "*" # domains allowed for CORS
+admin_user: admin # user with admin privileges
+admin_group: null # enable admin privileges for any user in this group
+openid_provider: azure # OpenID authentication provider
 openid_url: null # OpenID connect endpoint if provider is not azure or google
 openid_audience: null # OpenID audience. This is synonymous with azure_resource_id for azure
-openid_claims: unique_name,appid,roles   # Comma seperated list of claims to resolve to usernames.
-chaos_die: 0           # if > 0, have nodes randomly die after n seconds (for testing)
-standalone_app: false   # True when run as a single application
-blosc_nthreads: 2  # number of threads to use for blosc compression.  Set to 0 to have blosc auto-determine thread count
-http_compression: false  # Use HTTP compression 
-k8s_app_label: hsds  # The app label for k8s deployments
+openid_claims: unique_name,appid,roles # Comma seperated list of claims to resolve to usernames.
+chaos_die: 0 # if > 0, have nodes randomly die after n seconds (for testing)
+standalone_app: false # True when run as a single application
+blosc_nthreads: 2 # number of threads to use for blosc compression.  Set to 0 to have blosc auto-determine thread count
+http_compression: false # Use HTTP compression
+http_max_url_length: 512 # Limit http request url + params to be less than this
+http_streaming: true  # enable HTTP streaming 
+k8s_dn_label_selector: app=hsds # Selector for getting data node pods from a k8s deployment (https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors)
 k8s_namespace: null # Specifies if a the client should be limited to a specific namespace. Useful for some RBAC configurations.
 restart_policy: on-failure # Docker restart policy
-domain_req_max_objects_limit: 500  # maximum number of objects to return in GET domain request with use_cache
+domain_req_max_objects_limit: 500 # maximum number of objects to return in GET domain request with use_cache
+# the following two values with give backoff times of approx: 0.2, 0.4, 0.8, 1.6, 3.2, 6.4, 12.8
+dn_max_retries: 7 # number of time to retry DN requests
+dn_retry_backoff_exp: 0.1 # backoff factor for retries
+xss_protection: "1; mode=block"  # Include in response headers if set
+allow_any_bucket_read: true  # enable reads to buckets other than default bucket
+allow_any_bucket_write: true # enable writes to buckets other than default bucket
 # DEPRECATED - the remaining config values are not used in currently but kept for backward compatibility with older container images
-aws_lambda_chunkread_function: null  # name of aws lambda function for chunk reading
-aws_lambda_threshold: 4   # number of chunks per node per request to reach before using lambda
-aws_lambda_max_invoke: 1000  # max number of lambda functions to invoke simultaneously
+aws_lambda_chunkread_function: null # name of aws lambda function for chunk reading
+aws_lambda_threshold: 4 # number of chunks per node per request to reach before using lambda
+aws_lambda_max_invoke: 1000 # max number of lambda functions to invoke simultaneously
 aws_lambda_gateway: null # use lambda endpoint for region HSDS is running in
-write_zero_chunks: False # write chunk to storage even when it's all zeros (or in general equial to the fill value)
+k8s_app_label: null # The app label for k8s deployments (use k8s_dn_label_selector instead)
+write_zero_chunks: False # write chunk to storage even when it's all zeros (or in general equal to the fill value)
+max_chunks_per_request: 1000 # maximum number of chunks to be serviced by one request
+rangeget_port: 6900 # singleton proxy at port 6900
+rangeget_ram: 2g # memory for RANGEGET container
+data_cache_size: 128m # cache for rangegets
+data_cache_max_req_size: 128k # max size for rangeget fetches
+data_cache_expire_time: 3600 # expire cache items after one hour
+data_cache_page_size: 4m # page size for range get cache, set to zero to disable proxy
+data_cache_max_concurrent_read: 16 # maximum number of inflight storage read requests
```

### Comparing `hsds-0.7.0b11/hsds/app.py` & `hsds-0.8.0/hsds/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,36 +14,42 @@
 import json
 import sys
 import logging
 import time
 import uuid
 
 from .hsds_app import HsdsApp
- 
+
 _HELP_USAGE = "Starts hsds a REST-based service for HDF5 data."
 
 _HELP_EPILOG = """Examples:
 
-- with openio/sds data storage:
+- with minio data storage:
 
   hsds --s3-gateway http://localhost:6007 --access-key-id demo:demo
       --secret-access-key DEMO_PASS --password-file ./admin/config/passwd.txt
       --bucket-name hsds.test
 
 - with a POSIX-based storage for 'hsds.test' sub-folder in the './data'
   folder:
 
   hsds --bucket-dir ./data/hsds.test
 """
 
+# maximum number of characters if socket directory is given
+# Exceeding this can cause errors - see: https://github.com/HDFGroup/hsds/issues/129
+# Underlying issue is reported here: https://bugs.python.org/issue32958
+MAX_SOCKET_DIR_PATH_LEN = 63
+
 
 class UserConfig:
     """
     User Config state
     """
+
     def __init__(self, config_file=None, **kwargs):
         self._cfg = {}
         if config_file:
             self._config_file = config_file
         elif os.path.isfile(".hscfg"):
             self._config_file = ".hscfg"
         else:
@@ -53,58 +59,63 @@
             line_number = 0
             with open(self._config_file) as f:
                 for line in f:
                     line_number += 1
                     s = line.strip()
                     if not s:
                         continue
-                    if s[0] == '#':
+                    if s[0] == "#":
                         # comment line
                         continue
-                    index = line.find('=')
+                    index = line.find("=")
                     if index <= 0:
-                        print("config file: {} line: {} is not valid".format(self._config_file, line_number))
+                        print(
+                            "config file: {} line: {} is not valid".format(
+                                self._config_file, line_number
+                            )
+                        )
                         continue
                     k = line[:index].strip()
-                    v = line[(index+1):].strip()
+                    nlen = index + 1
+                    v = line[nlen:].strip()
                     if v and v.upper() != "NONE":
                         self._cfg[k] = v
         # override any config values with environment variable if found
         for k in self._cfg.keys():
             if k.upper() in os.environ:
                 self._cfg[k] = os.environ[k.upper()]
 
         # finally update any values that are passed in to the constructor
         for k in kwargs.keys():
             self._cfg[k.upper()] = kwargs[k]
 
     def __getitem__(self, name):
-        """ Get a config item  """
+        """Get a config item"""
 
         # Load a variable from environment. It would have only been loaded in
         # __init__ if it was also specified in the config file.
         env_name = name.upper()
         if name not in self._cfg and env_name in os.environ:
             self._cfg[name] = os.environ[env_name]
 
         return self._cfg[name]
 
     def __setitem__(self, name, obj):
-        """ set config item """
+        """set config item"""
         self._cfg[name] = obj
 
     def __delitem__(self, name):
-        """ Delete option. """
+        """Delete option."""
         del self._cfg[name]
 
     def __len__(self):
         return len(self._cfg)
 
     def __iter__(self):
-        """ Iterate over config names """
+        """Iterate over config names"""
         keys = self._cfg.keys()
         for key in keys:
             yield key
 
     def __contains__(self, name):
         return name in self._cfg or name.upper() in os.environ
 
@@ -121,56 +132,98 @@
             return default
 
 
 def main():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawTextHelpFormatter,
         usage=_HELP_USAGE,
-        epilog=_HELP_EPILOG)
+        epilog=_HELP_EPILOG,
+    )
 
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument(
-        '--root_dir', type=str, dest='root_dir',
-        help='Directory where to store the object store data')
+        "--root_dir",
+        type=str,
+        dest="root_dir",
+        help="Directory where to store the object store data",
+    )
     group.add_argument(
-        '--bucket_name', nargs=1, type=str, dest='bucket_name',
-        help='Name of the bucket to use (e.g., "hsds.test").')
-    parser.add_argument('--host', default='localhost',
-                        type=str, dest='host',
-                        help="host address for service node")
-    parser.add_argument('--hs_username', type=str,  dest='hs_username',
-                        help="username to be added to list of valid users",
-                        default='')
-    parser.add_argument('--hs_password', type=str,  dest='hs_password',
-                        help="password for hs_username", default='')
-    parser.add_argument('--password_file', type=str, dest='password_file',
-                        help="location of hsds password file",  default='')
-
-    parser.add_argument('--logfile', default='',
-                        type=str, dest='logfile',
-                        help="filename for logout (default stdout).")
-    parser.add_argument('--loglevel', default='',
-                        type=str, dest='loglevel',
-                        help="log verbosity: DEBUG, WARNING, INFO, OR ERROR")
-    parser.add_argument('-p', '--port', default=0,
-                        type=int, dest='port',
-                        help='Service node port')
-    parser.add_argument('--count', default=1, type=int,
-                        dest='dn_count',
-                        help='Number of dn sub-processes to create.')
-    parser.add_argument('--socket_dir', default='',
-                        type=str, dest='socket_dir',
-                        help="directory for socket endpoint")
-    parser.add_argument("--config_dir", default='',
-                        type=str, dest="config_dir",
-                        help="directory for config data")
+        "--bucket_name",
+        nargs=1,
+        type=str,
+        dest="bucket_name",
+        help='Name of the bucket to use (e.g., "hsds.test").',
+    )
+    parser.add_argument(
+        "--host", default="", type=str, dest="host", help="host name for url"
+    )
+    parser.add_argument(
+        "--hs_username",
+        type=str,
+        dest="hs_username",
+        help="username to be added to list of valid users",
+        default="",
+    )
+    parser.add_argument(
+        "--hs_password",
+        type=str,
+        dest="hs_password",
+        help="password for hs_username",
+        default="",
+    )
+    parser.add_argument(
+        "--password_file",
+        type=str,
+        dest="password_file",
+        help="location of hsds password file",
+        default="",
+    )
+
+    parser.add_argument(
+        "--logfile",
+        default="",
+        type=str,
+        dest="logfile",
+        help="filename for logout (default stdout).",
+    )
+    parser.add_argument(
+        "--loglevel",
+        default="",
+        type=str,
+        dest="loglevel",
+        help="log verbosity: DEBUG, WARNING, INFO, OR ERROR",
+    )
+    parser.add_argument(
+        "-p", "--port", default=0, type=int, dest="port", help="Service node port"
+    )
+    parser.add_argument(
+        "--count",
+        default=1,
+        type=int,
+        dest="dn_count",
+        help="Number of dn sub-processes to create.",
+    )
+    parser.add_argument(
+        "--socket_dir",
+        default="",
+        type=str,
+        dest="socket_dir",
+        help="directory for socket endpoint",
+    )
+    parser.add_argument(
+        "--config_dir",
+        default="",
+        type=str,
+        dest="config_dir",
+        help="directory for config data",
+    )
 
-    args, extra_args = parser.parse_known_args()
+    args = parser.parse_args()
 
-    kwargs = {} # options to pass to hsdsapp
+    kwargs = {}  # options to pass to hsdsapp
 
     # setup logging
     if args.loglevel:
         log_level_cfg = args.loglevel
         kwargs["log_level"] = args.loglevel
     elif "LOG_LEVEL" in os.environ:
         log_level_cfg = os.environ["LOG_LEVEL"]
@@ -214,52 +267,80 @@
         kwargs["password"] = password
 
     if args.password_file:
         if not os.path.isfile(args.password_file):
             sys.exit(f"password file: {args.password_file} not found")
         kwargs["password_file"] = args.password_file
 
-    # choose a tmp directory for socket if one is not provided
-    if args.socket_dir:
-        socket_dir = args.socket_dir
+    if args.host:
+        # use TCP connect
+        kwargs["host"] = args.host
+        # sn_port only relevant for TCP connections
+        if args.port:
+            kwargs["sn_port"] = args.port
+        else:
+            kwargs["sn_port"] = 5101  # TBD - use config
     else:
-        tmp_dir = "/tmp"  # TBD: will this work on windows?
-        rand_name = uuid.uuid4().hex[:8]
-        socket_dir = f"{tmp_dir}/hs{rand_name}/"
-    kwargs["socket_dir"] = socket_dir
+        # choose a tmp directory for socket if one is not provided
+        if args.socket_dir:
+            socket_dir = os.path.abspath(args.socket_dir)
+            if not os.path.isdir(socket_dir):
+                raise FileNotFoundError(f"directory: {socket_dir} not found")
+        else:
+            if "TMP" in os.environ:
+                # This should be set at least on Windows
+                tmp_dir = os.environ["TMP"]
+                print("set tmp_dir:", tmp_dir)
+            else:
+                tmp_dir = "/tmp"
+            if not os.path.isdir(tmp_dir):
+                raise FileNotFoundError(f"directory {tmp_dir} not found")
+            rand_name = uuid.uuid4().hex[:8]
+            socket_dir = os.path.join(tmp_dir, f"hs{rand_name}")
+            print("using socket dir:", socket_dir)
+            if len(socket_dir) > MAX_SOCKET_DIR_PATH_LEN:
+                raise ValueError(
+                    f"length of socket_dir must be less than: {MAX_SOCKET_DIR_PATH_LEN}"
+                )
+            os.mkdir(socket_dir)
+        kwargs["socket_dir"] = socket_dir
 
     if args.logfile:
-        if os.path.isabs(args.logfile):
-            logfile = args.logfile
-        else:
-            # use filename in the socket directory
-            logfile = os.path.join(socket_dir, args.logfile)
+        logfile = os.path.abspath(args.logfile)
+    elif args.host:
+        logfile = os.path.abspath("hs.log")
     else:
-        logfile = None
-    if logfile:
-        kwargs["logfile"] = logfile
+        socket_dir = os.path.abspath(args.socket_dir)
+        logfile = os.path.join(socket_dir, "hs.log")
+    print("logfile:", logfile)
+    kwargs["logfile"] = logfile
+
+    if args.root_dir:
+        kwargs["root_dir"] = args.root_dir
+
     config_dir = None
     if args.config_dir:
         if not os.path.isdir(args.config_dir):
             print(f"config_dir: {args.config_dir} not found")
         else:
             config_dir = args.config_dir
     if config_dir:
         kwargs["config_dir"] = config_dir
+
     if args.dn_count:
         kwargs["dn_count"] = args.dn_count
 
     app = HsdsApp(**kwargs)
     app.run()
 
     waiting_on_ready = True
 
     while True:
         try:
-            time.sleep(1)   
+            time.sleep(1)
             app.check_processes()
         except KeyboardInterrupt:
             print("got keyboard interrupt")
             break
         except Exception as e:
             print(f"got exception: {e}")
             break
@@ -267,9 +348,7 @@
             waiting_on_ready = False
             print("")
             print("READY! use endpoint:", app.endpoint)
             print("")
 
     print("shutting down server")
     app.stop()
-    
-
```

### Comparing `hsds-0.7.0b11/hsds/async_lib.py` & `hsds-0.8.0/hsds/async_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from aiohttp.web_exceptions import HTTPNotFound, HTTPInternalServerError
 from aiohttp.web_exceptions import HTTPForbidden
 from .util.idUtil import isValidUuid, isSchema2Id, getS3Key, isS3ObjKey
 from .util.idUtil import getObjId, isValidChunkId, getCollectionForId
 from .util.chunkUtil import getDatasetId, getNumChunks, ChunkIterator
 from .util.hdf5dtype import getItemSize, createDataType
 from .util.arrayUtil import getShapeDims, getNumElements, bytesToArray
-from .util.dsetUtil import getHyperslabSelection, getFilterOps
+from .util.dsetUtil import getHyperslabSelection, getFilterOps, getChunkDims
+from .util.dsetUtil import getDatasetLayoutClass, getDatasetCreationPropertyLayout
 
 from .util.storUtil import getStorKeys, putStorJSONObj, getStorJSONObj
 from .util.storUtil import deleteStorObj, getStorBytes, isStorObj
 from . import hsds_logger as log
 from . import config
 
 # List all keys under given root and optionally update info.json
@@ -47,126 +48,128 @@
         msg = f"HTTPInternalServerError error for {s3_key} bucket:{bucket}"
         log.warn(msg)
         return None
     return dset_json
 
 
 async def updateDatasetInfo(app, dset_id, dataset_info, bucket=None):
-    # get dataset metadata and deteermine number logical)_bytes,
+    # get dataset metadata and determine number logical_bytes,
     # linked_bytes, and num_linked_chunks
 
     dset_json = await getDatasetJson(app, dset_id, bucket=bucket)
     msg = f"updateDatasetInfo - id: {dset_id} dataset_info: {dataset_info}"
     log.debug(msg)
     if "shape" not in dset_json:
         msg = f"updateDatasetInfo - no shape dataset_json for {dset_id} "
         msg += "- skipping"
         log.debug(msg)
-        return   # null dataspace
+        return  # null dataspace
     shape_json = dset_json["shape"]
-    if "class" in shape_json and shape_json["class"] == 'H5S_NULL':
+    if "class" in shape_json and shape_json["class"] == "H5S_NULL":
         log.debug(f"updatedDatasetInfo - null space for {dset_id} - skipping")
         return
     if "type" not in dset_json:
         msg = "updateDatasetInfo - expected to find type in dataset_json for "
         msg += f"{dset_id}"
         log.warn(msg)
         return
     type_json = dset_json["type"]
     item_size = getItemSize(type_json)
     if "layout" not in dset_json:
         msg = "updateDatasetInfo - expected to find layout in dataset_json "
         msg += f"for {dset_id}"
         log.warn(msg)
         return
-    layout = dset_json["layout"]
+    layout = getDatasetCreationPropertyLayout(dset_json)
     msg = f"updateDatasetInfo - shape: {shape_json} type: {type_json} "
     msg += f"item size: {item_size} layout: {layout}"
     log.info(msg)
 
     dims = getShapeDims(shape_json)  # returns None for HS_NULL dsets
 
     if dims is None:
         return  # null dataspace
 
-    if item_size == 'H5T_VARIABLE':
+    if item_size == "H5T_VARIABLE":
         # arbitrary lgoical size for vaariable, so just set to allocated size
-        logical_bytes = dataset_info['allocated_bytes']
+        logical_bytes = dataset_info["allocated_bytes"]
     else:
         num_elements = getNumElements(dims)
         logical_bytes = num_elements * item_size
     dataset_info["logical_bytes"] = logical_bytes
-    log.debug(f"dims: {dims}")
+    log.debug(f"updateDatasetInfo - dims: {dims}")
     rank = len(dims)
-    layout_class = layout["class"]
+    layout_class = getDatasetLayoutClass(dset_json)
     msg = f"updateDatasetInfo - {dset_id} has layout_class: {layout_class}"
     log.debug(msg)
     selection = getHyperslabSelection(dims)  # select entire datashape
     linked_bytes = 0
     num_linked_chunks = 0
 
-    if layout_class == 'H5D_CONTIGUOUS_REF':
+    if layout_class == "H5D_CONTIGUOUS_REF":
         # In H5D_CONTIGUOUS_REF a non-compressed part of the HDF5 is divided
         # into equal size chunks, so we can just compute link bytes and num
         # chunks based on the size of the coniguous dataset
-        layout_dims = layout["dims"]
+        layout_dims = getChunkDims(dset_json)
         num_chunks = getNumChunks(selection, layout_dims)
         chunk_size = item_size
         for dim in layout_dims:
             chunk_size *= dim
         msg = "updateDatasetInfo, H5D_CONTIGUOUS_REF, num_chunks: "
         msg += f"{num_chunks} chunk_size: {chunk_size}"
         log.debug(msg)
         linked_bytes = chunk_size * num_chunks
         num_linked_chunks = num_chunks
-    elif layout_class == 'H5D_CHUNKED_REF':
+    elif layout_class == "H5D_CHUNKED_REF":
+        if "chunks" not in layout:
+            log.error("Expected to find 'chunks' key in H5D_CHUNKED_REF layout")
+            return
         chunks = layout["chunks"]
         # chunks is a dict with tuples (offset, size)
         for chunk_id in chunks:
             chunk_info = chunks[chunk_id]
             linked_bytes += chunk_info[1]
         num_linked_chunks = len(chunks)
-    elif layout_class == 'H5D_CHUNKED_REF_INDIRECT':
+    elif layout_class == "H5D_CHUNKED_REF_INDIRECT":
         log.debug("chunk ref indirect")
         if "chunk_table" not in layout:
             msg = "Expected to find chunk_table in dataset layout for "
             msg += f"{dset_id}"
-            log.error()
+            log.error(msg)
             return
         chunktable_id = layout["chunk_table"]
         # get  state for dataset from DN.
         kwargs = {"bucket": bucket}
         chunktable_json = await getDatasetJson(app, chunktable_id, **kwargs)
         log.debug(f"chunktable_json: {chunktable_json}")
         chunktable_dims = getShapeDims(chunktable_json["shape"])
         if len(chunktable_dims) != rank:
             msg = "Expected rank of chunktable to be same as the dataset "
             msg += f"for {dset_id}"
             log.warn(msg)
             return
-        chunktable_layout = chunktable_json["layout"]
+        chunktable_layout = getDatasetCreationPropertyLayout(chunktable_json)
         log.debug(f"chunktable_layout: {chunktable_layout}")
         if not isinstance(chunktable_layout, dict):
             log.warn(f"unexpected chunktable_layout: {chunktable_id}")
             return
         if "class" not in chunktable_layout:
             log.warn(f"expected class in chunktable_layout: {chunktable_id}")
             return
-        if chunktable_layout["class"] != 'H5D_CHUNKED':
+        if chunktable_layout["class"] != "H5D_CHUNKED":
             log.warn("expected chunktable layout class to be chunked")
             return
         if "dims" not in chunktable_layout:
             log.warn("expected chunktable layout to have dims key")
             return
         dims = chunktable_layout["dims"]
         chunktable_type_json = chunktable_json["type"]
         chunktable_item_size = getItemSize(chunktable_type_json)
         chunktable_dt = createDataType(chunktable_type_json)
-        chunktable_filter_ops = \
-            getFilterOps(app, chunktable_json, chunktable_item_size)
+        chunktable_filter_ops = getFilterOps(app, chunktable_json, chunktable_item_size)
 
         # read chunktable one chunk at a time - this can be slow if there
         # are a lot of chunks, but this is only used by the async bucket
         # scan task
         sel = getHyperslabSelection(chunktable_dims)
         it = ChunkIterator(chunktable_id, sel, dims)
         msg = f"updateDatasetInfo - iterating over chunks in {chunktable_id}"
@@ -177,29 +180,26 @@
                 chunktable_chunk_id = it.next()
                 msg = "updateDatasetInfo - gotchunktable chunk id: "
                 msg += f"{chunktable_chunk_id}"
                 log.debug(msg)
                 s3key = getS3Key(chunktable_chunk_id)
                 # read the chunk
                 try:
-                    is_stor_obj = await isStorObj(app,
-                                                  s3key,
-                                                  bucket=bucket)
+                    is_stor_obj = await isStorObj(app, s3key, bucket=bucket)
                 except HTTPInternalServerError as hse:
                     msg = "updateDatasetInfo - got error checking for key: "
                     msg += f"{s3key}: {hse}"
                     log.warning(msg)
                     continue
                 if not is_stor_obj:
                     msg = "updateDatasetInfo - no chunk found for chunktable "
                     msg += f"id: {chunktable_chunk_id}"
                     log.debug(msg)
                 else:
-                    kwargs = {"filter_ops": chunktable_filter_ops,
-                              "bucket": bucket}
+                    kwargs = {"filter_ops": chunktable_filter_ops, "bucket": bucket}
                     try:
                         chunk_bytes = await getStorBytes(app, s3key, **kwargs)
                     except HTTPInternalServerError as hse:
                         msg = "updateDatasetInfo - got error reading "
                         msg += f"chunktable for key: {s3key}: {hse}"
                         log.warning(msg)
                         continue
@@ -227,15 +227,15 @@
                             msg += f"{chunktable_chunk_id}: {e}"
                             log.error(msg)
             except StopIteration:
                 break
         msg = "updateDatasetInfo - done with chunktable iteration "
         msg += f"for {chunktable_id}"
         log.debug(msg)
-    elif layout_class == 'H5D_CHUNKED':
+    elif layout_class == "H5D_CHUNKED":
         msg = "updateDatasetInfo - no linked bytes/chunks for "
         msg += "H5D_CHUNKED layout"
         log.debug(msg)
     else:
         log.error(f"unexpected chunk layout: {layout_class}")
 
     msg = f"updateDatasetInfo - {dset_id} setting linked_bytes to "
@@ -353,15 +353,15 @@
     if not bucket:
         raise ValueError(f"no bucket defined for scan of {rootid}")
 
     root_key = getS3Key(rootid)
 
     if not root_key.endswith("/.group.json"):
         raise ValueError("unexpected root key")
-    root_prefix = root_key[:-(len(".group.json"))]
+    root_prefix = root_key[: -(len(".group.json"))]
 
     log.debug(f"scanRoot - using prefix: {root_prefix}")
 
     results = {}
     results["lastModified"] = 0
     results["num_groups"] = 0
     results["num_datatypes"] = 0
@@ -375,16 +375,20 @@
     results["checksums"] = {}  # map of objid to checksums
     results["bucket"] = bucket
     results["scan_start"] = time.time()
 
     app["scanRoot_results"] = results
     app["scanRoot_keyset"] = set()
 
-    kwargs = {"prefix": root_prefix, "include_stats": True,
-              "bucket": bucket, "callback": scanRootCallback}
+    kwargs = {
+        "prefix": root_prefix,
+        "include_stats": True,
+        "bucket": bucket,
+        "callback": scanRootCallback,
+    }
     await getStorKeys(app, **kwargs)
     num_objects = results["num_groups"]
     num_objects += results["num_datatypes"]
     num_objects += len(results["datasets"])
     num_objects += results["num_chunks"]
     log.info(f"scanRoot - got {num_objects} keys for rootid: {rootid}")
 
@@ -407,15 +411,15 @@
         msg = f"skipping domain checksum calculation - {len(checksums)} found "
         msg += f"but {num_objects} hdf objects"
         log.warn(msg)
     else:
         # create a numpy array to store checksums
         msg = f"creating numpy checksum array for {num_objects} checksums"
         log.debug(msg)
-        checksum_arr = np.zeros((num_objects,), dtype='S16')
+        checksum_arr = np.zeros((num_objects,), dtype="S16")
         objids = list(checksums.keys())
         objids.sort()
         for i in range(num_objects):
             objid = objids[i]
             checksum_arr[i] = checksums[objid]
         log.debug("numpy array created")
         hash_object = hashlib.md5(checksum_arr.tobytes())
@@ -443,62 +447,70 @@
     if not isinstance(s3keys, list):
         log.error("expected list result for objDeleteCallback")
         raise ValueError("unexpected callback format")
 
     if "objDelete_prefix" not in app or not app["objDelete_prefix"]:
         log.error("Unexpected objDeleteCallback")
         raise ValueError("Invalid objDeleteCallback")
+    if "objDelete_bucket" not in app:
+        log.error("Expecte to find objDelete_bucket key for objDeleteCallback")
+        raise ValueError("Invalid objDeleteCallback")
 
     prefix = app["objDelete_prefix"]
+    bucket = app["objDelete_bucket"]
     prefix_len = len(prefix)
     for s3key in s3keys:
         if not s3key.startswith(prefix):
             log.error(f"Unexpected key {s3key} for prefix: {prefix}")
             raise ValueError("invalid s3key for objDeleteCallback")
         full_key = prefix + s3key[prefix_len:]
         log.info(f"removeKeys - objDeleteCallback deleting key: {full_key}")
-        await deleteStorObj(app, full_key)
+        await deleteStorObj(app, full_key, bucket=bucket)
 
     log.info("objDeleteCallback complete")
 
 
-async def removeKeys(app, objid):
-    """ delete all keys for given root or dataset id"""
+async def removeKeys(app, objid, bucket=None):
+    """delete all keys for given root or dataset id"""
     # iterate through all s3 keys under the given root or dataset id
     #  and delete them
     #
     # Note: not re-entrant!  Only one removeKeys an be run at a time
     # per app.
-    log.debug(f"removeKeys: {objid}")
+    log.info(f"removeKeys: {objid}, bucket: {bucket}")
     if not isSchema2Id(objid):
         log.warn("ignoring non-schema2 id")
         raise KeyError("Invalid key")
     s3key = getS3Key(objid)
     log.debug(f"removeKeys - got s3key: {s3key}")
     expected_suffixes = (".dataset.json", ".group.json")
     s3prefix = None
 
     for suffix in expected_suffixes:
         if s3key.endswith(suffix):
-            s3prefix = s3key[:-len(suffix)]
+            s3prefix = s3key[: -len(suffix)]
     if not s3prefix:
         log.error("removeKeys - unexpected s3key for delete_set")
         raise KeyError("unexpected key suffix")
     msg = f"removeKeys - delete for {objid} searching for s3prefix: {s3prefix}"
     log.info(msg)
     if app["objDelete_prefix"]:
         msg = "removeKeys - objDelete_prefix is already set - improper use of "
         msg += "non-reentrant call?"
         log.error(msg)
         # just continue and reset
     app["objDelete_prefix"] = s3prefix
+    app["objDelete_bucket"] = bucket
     try:
-        kwargs = {"prefix": s3prefix,
-                  "include_stats": False,
-                  "callback": objDeleteCallback}
+        kwargs = {
+            "prefix": s3prefix,
+            "include_stats": False,
+            "bucket": bucket,
+            "callback": objDeleteCallback,
+        }
         await getStorKeys(app, **kwargs)
     except ClientError as ce:
         log.error(f"removeKeys - getS3Keys faiiled: {ce}")
     except HTTPNotFound:
         msg = "removeKeys - HTTPNotFound error for getStorKeys with prefix: "
         msg += f"{s3prefix}"
         log.warn(msg)
@@ -509,7 +521,8 @@
     except Exception as e:
         msg = "removeKeys - Unexpected Exception for getStorKeys with "
         msg += f"prefix: {s3prefix}: {e}"
         log.error(msg)
 
     # reset the prefix
     app["objDelete_prefix"] = None
+    app["objDelete_bucket"] = None
```

### Comparing `hsds-0.7.0b11/hsds/attr_dn.py` & `hsds-0.8.0/hsds/attr_dn.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,26 @@
 from aiohttp.web import json_response
 
 from .util.attrUtil import validateAttributeName
 from .datanode_lib import get_obj_id, get_metadata_obj, save_metadata_obj
 from . import hsds_logger as log
 
 
-def index(a, x):
-    """ Locate the leftmost value exactly equal to x
-    """
-    i = bisect_left(a, x)
-    if i != len(a) and a[i] == x:
-        return i
+def _index(items, marker, create_order=False):
+    """Locate the leftmost value exactly equal to x"""
+    if create_order:
+        # list is not ordered, juse search linearly
+        for i in range(len(items)):
+            if items[i] == marker:
+                return i
+    else:
+        i = bisect_left(items, marker)
+        if i != len(items) and items[i] == marker:
+            return i
+    # not found
     return -1
 
 
 async def GET_Attributes(request):
     """ Return JSON for attribute collection
     """
     log.request(request)
@@ -42,14 +48,18 @@
 
     obj_id = get_obj_id(request)
     if "bucket" in params:
         bucket = params["bucket"]
     else:
         bucket = None
 
+    create_order = False
+    if "CreateOrder" in params and params["CreateOrder"]:
+        create_order = True
+
     include_data = False
     if "IncludeData" in params and params["IncludeData"]:
         include_data = True
 
     limit = None
     if "Limit" in params:
         try:
@@ -59,46 +69,62 @@
             msg = "Bad Request: Expected int type for limit"
             log.error(msg)  # should be validated by SN
             raise HTTPInternalServerError()
 
     marker = None
     if "Marker" in params:
         marker = params["Marker"]
-        log.info("GET_Links - using Marker: {}".format(marker))
+        log.info(f"GET_Links - using Marker: {marker}")
 
     obj_json = await get_metadata_obj(app, obj_id, bucket=bucket)
 
-    log.debug("GET attributes obj_id: {} got json".format(obj_id))
+    log.debug(f"GET attributes obj_id: {obj_id} got json")
     if "attributes" not in obj_json:
-        msg = "unexpected data for obj id: {}".format(obj_id)
+        msg = f"unexpected data for obj id: {obj_id}"
         msg.error(msg)
         raise HTTPInternalServerError()
 
     # return a list of attributes based on sorted dictionary keys
     attr_dict = obj_json["attributes"]
-    attr_names = list(attr_dict.keys())
-    attr_names.sort()  # sort by key
-    # TBD: provide an option to sort by create date
+
+    titles = []
+    if create_order:
+        order_dict = {}
+        for title in attr_dict:
+            item = attr_dict[title]
+            if "created" not in item:
+                log.warning(f"expected to find 'created' key in attr item {title}")
+                continue
+            order_dict[title] = item["created"]
+        log.debug(f"order_dict: {order_dict}")
+        # now sort by created
+        for k in sorted(order_dict.items(), key=lambda item: item[1]):
+            titles.append(k[0])
+        log.debug(f"attrs by create order: {titles}")
+    else:
+        titles = list(attr_dict.keys())
+        titles.sort()  # sort by key
+        log.debug(f"attrs by lexographic order: {titles}")
 
     start_index = 0
     if marker is not None:
-        start_index = index(attr_names, marker) + 1
+        start_index = _index(titles, marker, create_order=create_order) + 1
         if start_index == 0:
             # marker not found, return 404
-            msg = "attribute marker: {}, not found".format(marker)
+            msg = f"attribute marker: {marker}, not found"
             log.warn(msg)
             raise HTTPNotFound()
 
-    end_index = len(attr_names)
+    end_index = len(titles)
     if limit is not None and (end_index - start_index) > limit:
         end_index = start_index + limit
 
     attr_list = []
     for i in range(start_index, end_index):
-        attr_name = attr_names[i]
+        attr_name = titles[i]
         src_attr = attr_dict[attr_name]
         des_attr = {}
         des_attr["created"] = src_attr["created"]
         des_attr["type"] = src_attr["type"]
         des_attr["shape"] = src_attr["shape"]
         des_attr["name"] = attr_name
         if include_data:
```

### Comparing `hsds-0.7.0b11/hsds/attr_sn.py` & `hsds-0.8.0/hsds/attr_sn.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 # attribute methods for SN
 #
 
 import numpy as np
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPInternalServerError
 from aiohttp.web import StreamResponse
+from json import JSONDecodeError
 
 from .util.httpUtil import http_get, http_put, http_delete, getHref
 from .util.httpUtil import getAcceptType, jsonResponse
 from .util.idUtil import isValidUuid, getDataNodeUrl
 from .util.authUtil import getUserPasswordFromRequest, validateUserPassword
 from .util.domainUtil import getDomainFromRequest, isValidDomain
 from .util.domainUtil import getBucketForDomain, verifyRoot
@@ -37,46 +38,49 @@
     """HTTP method to return JSON for attribute collection"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
     # returns datasets|groups|datatypes
     collection = getRequestCollectionName(request)
 
-    obj_id = request.match_info.get('id')
+    obj_id = request.match_info.get("id")
     if not obj_id:
         msg = "Missing object id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     if not isValidUuid(obj_id, obj_class=collection):
-        msg = "Invalid obj id: {}".format(obj_id)
+        msg = f"Invalid obj id: {obj_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     include_data = False
     ignore_nan = False
     if "IncludeData" in params and params["IncludeData"]:
         include_data = True
         if "ignore_nan" in params and params["ignore_nan"]:
             ignore_nan = True
+    create_order = False
+    if "CreateOrder" in params and params["CreateOrder"]:
+        create_order = True
 
     limit = None
     if "Limit" in params:
         try:
             limit = int(params["Limit"])
         except ValueError:
             msg = "Bad Request: Expected int type for limit"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
     marker = None
     if "Marker" in params:
         marker = params["Marker"]
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
@@ -85,24 +89,26 @@
     bucket = getBucketForDomain(domain)
 
     # TBD - verify that the obj_id belongs to the given domain
     await validateAction(app, domain, obj_id, username, "read")
 
     req = getDataNodeUrl(app, obj_id)
 
-    req += '/' + collection + '/' + obj_id + "/attributes"
+    req += "/" + collection + "/" + obj_id + "/attributes"
     params = {}
     if limit is not None:
         params["Limit"] = str(limit)
     if marker is not None:
         params["Marker"] = marker
     if include_data:
-        params["IncludeData"] = '1'
+        params["IncludeData"] = 1
     if bucket:
         params["bucket"] = bucket
+    if create_order:
+        params["CreateOrder"] = 1
 
     log.debug(f"get attributes: {req}")
     dn_json = await http_get(app, req, params=params)
     log.debug(f"got attributes json from dn for obj_id: {obj_id}")
     attributes = dn_json["attributes"]
 
     # mixin hrefs
@@ -111,47 +117,47 @@
         attr_href = f"/{collection}/{obj_id}/attributes/{attr_name}"
         attribute["href"] = getHref(request, attr_href)
 
     resp_json = {}
     resp_json["attributes"] = attributes
 
     hrefs = []
-    obj_uri = '/' + collection + '/' + obj_id
-    href = getHref(request, obj_uri + '/attributes')
-    hrefs.append({'rel': 'self', 'href': href})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
-    hrefs.append({'rel': 'owner', 'href': getHref(request, obj_uri)})
+    obj_uri = "/" + collection + "/" + obj_id
+    href = getHref(request, obj_uri + "/attributes")
+    hrefs.append({"rel": "self", "href": href})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
+    hrefs.append({"rel": "owner", "href": getHref(request, obj_uri)})
     resp_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, resp_json, ignore_nan=ignore_nan)
     log.response(request, resp=resp)
     return resp
 
 
 async def GET_Attribute(request):
     """HTTP method to return JSON for an attribute"""
     log.request(request)
     app = request.app
     # returns datasets|groups|datatypes
     collection = getRequestCollectionName(request)
 
-    obj_id = request.match_info.get('id')
+    obj_id = request.match_info.get("id")
     if not obj_id:
         msg = "Missing object id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(obj_id, obj_class=collection):
         msg = f"Invalid object id: {obj_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    attr_name = request.match_info.get('name')
+    attr_name = request.match_info.get("name")
     validateAttributeName(attr_name)
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
@@ -183,56 +189,61 @@
     if "value" in dn_json:
         resp_json["value"] = dn_json["value"]
     resp_json["created"] = dn_json["created"]
     # attributes don't get modified, so use created timestamp as lastModified
     resp_json["lastModified"] = dn_json["created"]
 
     hrefs = []
-    obj_uri = '/' + collection + '/' + obj_id
-    attr_uri = obj_uri + '/attributes/' + attr_name
-    hrefs.append({'rel': 'self', 'href': getHref(request, attr_uri)})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
-    hrefs.append({'rel': 'owner', 'href': getHref(request, obj_uri)})
+    obj_uri = "/" + collection + "/" + obj_id
+    attr_uri = obj_uri + "/attributes/" + attr_name
+    hrefs.append({"rel": "self", "href": getHref(request, attr_uri)})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
+    hrefs.append({"rel": "owner", "href": getHref(request, obj_uri)})
     resp_json["hrefs"] = hrefs
     resp = await jsonResponse(request, resp_json, ignore_nan=ignore_nan)
     log.response(request, resp=resp)
     return resp
 
 
 async def PUT_Attribute(request):
     """HTTP method to create a new attribute"""
     log.request(request)
     app = request.app
     # returns datasets|groups|datatypes
     collection = getRequestCollectionName(request)
 
-    obj_id = request.match_info.get('id')
+    obj_id = request.match_info.get("id")
     if not obj_id:
         msg = "Missing object id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(obj_id, obj_class=collection):
         msg = f"Invalid object id: {obj_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    attr_name = request.match_info.get('name')
+    attr_name = request.match_info.get("name")
     log.debug(f"Attribute name: [{attr_name}]")
     validateAttributeName(attr_name)
 
     log.info(f"PUT Attribute id: {obj_id} name: {attr_name}")
     username, pswd = getUserPasswordFromRequest(request)
     # write actions need auth
     await validateUserPassword(app, username, pswd)
 
     if not request.has_body:
         msg = "PUT Attribute with no body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
-    body = await request.json()
+    try:
+        body = await request.json()
+    except JSONDecodeError:
+        msg = "Unable to load JSON body"
+        log.warn(msg)
+        raise HTTPBadRequest(reason=msg)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     bucket = getBucketForDomain(domain)
@@ -327,33 +338,39 @@
                 log.warn(msg)
                 raise HTTPBadRequest(reason=msg)
         else:
             # no class, interpet shape value as dimensions and
             # use H5S_SIMPLE as class
             if isinstance(shape_body, list) and len(shape_body) == 0:
                 shape_json["class"] = "H5S_SCALAR"
-                dims = [1, ]
+                dims = [
+                    1,
+                ]
             else:
                 shape_json["class"] = "H5S_SIMPLE"
                 dims = getShapeDims(shape_body)
                 shape_json["dims"] = dims
     else:
         shape_json["class"] = "H5S_SCALAR"
-        dims = [1, ]
+        dims = [
+            1,
+        ]
 
     if "value" in body:
         if dims is None:
             msg = "Bad Request: data can not be included with H5S_NULL space"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         value = body["value"]
         # validate that the value agrees with type/shape
         arr_dtype = createDataType(datatype)  # np datatype
         if len(dims) == 0:
-            np_dims = [1, ]
+            np_dims = [
+                1,
+            ]
         else:
             np_dims = dims
         log.debug(f"attribute dims: {np_dims}")
         log.debug(f"attribute value: {value}")
         try:
             arr = jsonToArray(np_dims, arr_dtype, value)
         except ValueError:
@@ -362,15 +379,15 @@
             raise HTTPBadRequest(reason=msg)
         log.info(f"Got: {arr.size} array elements")
     else:
         value = None
 
     # ready to add attribute now
     req = getDataNodeUrl(app, obj_id)
-    req += '/' + collection + '/' + obj_id + "/attributes/" + attr_name
+    req += "/" + collection + "/" + obj_id + "/attributes/" + attr_name
     log.info("PUT Attribute: " + req)
 
     attr_json = {}
     attr_json["type"] = datatype
     attr_json["shape"] = shape_json
     if value is not None:
         attr_json["value"] = value
@@ -392,24 +409,24 @@
 async def DELETE_Attribute(request):
     """HTTP method to delete a attribute resource"""
     log.request(request)
     app = request.app
     # returns datasets|groups|datatypes
     collection = getRequestCollectionName(request)
 
-    obj_id = request.match_info.get('id')
+    obj_id = request.match_info.get("id")
     if not obj_id:
         msg = "Missing object id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(obj_id, obj_class=collection):
         msg = f"Invalid object id: {obj_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    attr_name = request.match_info.get('name')
+    attr_name = request.match_info.get("name")
     log.debug(f"Attribute name: [{attr_name}]")
     validateAttributeName(attr_name)
 
     username, pswd = getUserPasswordFromRequest(request)
     await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
@@ -423,15 +440,15 @@
     domain_json = await getDomainJson(app, domain)
     verifyRoot(domain_json)
 
     # TBD - verify that the obj_id belongs to the given domain
     await validateAction(app, domain, obj_id, username, "delete")
 
     req = getDataNodeUrl(app, obj_id)
-    req += '/' + collection + '/' + obj_id + "/attributes/" + attr_name
+    req += "/" + collection + "/" + obj_id + "/attributes/" + attr_name
     log.info("PUT Attribute: " + req)
     params = {}
     if bucket:
         params["bucket"] = bucket
     rsp_json = await http_delete(app, req, params=params)
 
     log.info(f"PUT Attribute resp: {rsp_json}")
@@ -447,28 +464,28 @@
     """HTTP method to return an attribute value"""
     log.request(request)
     app = request.app
     log.info("GET_AttributeValue")
     # returns datasets|groups|datatypes
     collection = getRequestCollectionName(request)
 
-    obj_id = request.match_info.get('id')
+    obj_id = request.match_info.get("id")
     if not obj_id:
         msg = "Missing object id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(obj_id, obj_class=collection):
         msg = f"Invalid object id: {obj_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    attr_name = request.match_info.get('name')
+    attr_name = request.match_info.get("name")
     validateAttributeName(attr_name)
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain value: {domain}"
@@ -486,36 +503,36 @@
     params = request.rel_url.query
     if "ignore_nan" in params and params["ignore_nan"]:
         ignore_nan = True
     else:
         ignore_nan = False
 
     req = getDataNodeUrl(app, obj_id)
-    req += '/' + collection + '/' + obj_id + "/attributes/" + attr_name
+    req += "/" + collection + "/" + obj_id + "/attributes/" + attr_name
     log.debug("get Attribute: " + req)
     params = {}
     if bucket:
         params["bucket"] = bucket
     dn_json = await http_get(app, req, params=params)
     log.debug("got attributes json from dn for obj_id: " + str(dn_json))
 
     attr_shape = dn_json["shape"]
     log.debug(f"attribute shape: {attr_shape}")
-    if attr_shape["class"] == 'H5S_NULL':
+    if attr_shape["class"] == "H5S_NULL":
         msg = "Null space attributes can not be read"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     accept_type = getAcceptType(request)
-    response_type = accept_type    # will adjust later if binary not possible
+    response_type = accept_type  # will adjust later if binary not possible
     type_json = dn_json["type"]
     shape_json = dn_json["shape"]
     item_size = getItemSize(type_json)
 
-    if item_size == 'H5T_VARIABLE' and accept_type != "json":
+    if item_size == "H5T_VARIABLE" and accept_type != "json":
         msg = "Client requested binary, but only JSON is supported for "
         msg += "variable length data types"
         log.info(msg)
         response_type = "json"
 
     if response_type == "binary":
         arr_dtype = createDataType(type_json)  # np datatype
@@ -536,61 +553,61 @@
         # write response
         try:
             resp = StreamResponse()
             resp.content_type = "application/octet-stream"
             resp.content_length = len(output_data)
             # allow CORS
             if cors_domain:
-                resp.headers['Access-Control-Allow-Origin'] = cors_domain
+                resp.headers["Access-Control-Allow-Origin"] = cors_domain
                 cors_methods = "GET, POST, DELETE, PUT, OPTIONS"
-                resp.headers['Access-Control-Allow-Methods'] = cors_methods
+                resp.headers["Access-Control-Allow-Methods"] = cors_methods
                 cors_headers = "Content-Type, api_key, Authorization"
-                resp.headers['Access-Control-Allow-Headers'] = cors_headers
+                resp.headers["Access-Control-Allow-Headers"] = cors_headers
             await resp.prepare(request)
             await resp.write(output_data)
         except Exception as e:
             log.error(f"Got exception: {e}")
             raise HTTPInternalServerError()
         finally:
             await resp.write_eof()
 
     else:
         resp_json = {}
         if "value" in dn_json:
             resp_json["value"] = dn_json["value"]
 
         hrefs = []
-        obj_uri = '/' + collection + '/' + obj_id
-        attr_uri = obj_uri + '/attributes/' + attr_name
-        hrefs.append({'rel': 'self', 'href': getHref(request, attr_uri)})
-        hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
-        hrefs.append({'rel': 'owner', 'href': getHref(request, obj_uri)})
+        obj_uri = "/" + collection + "/" + obj_id
+        attr_uri = obj_uri + "/attributes/" + attr_name
+        hrefs.append({"rel": "self", "href": getHref(request, attr_uri)})
+        hrefs.append({"rel": "home", "href": getHref(request, "/")})
+        hrefs.append({"rel": "owner", "href": getHref(request, obj_uri)})
         resp_json["hrefs"] = hrefs
         resp = await jsonResponse(request, resp_json, ignore_nan=ignore_nan)
         log.response(request, resp=resp)
     return resp
 
 
 async def PUT_AttributeValue(request):
     """HTTP method to update an attributes data"""
     log.request(request)
     log.info("PUT_AttributeValue")
     app = request.app
     # returns datasets|groups|datatypes
     collection = getRequestCollectionName(request)
-    obj_id = request.match_info.get('id')
+    obj_id = request.match_info.get("id")
     if not obj_id:
         msg = "Missing object id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(obj_id, obj_class=collection):
         msg = f"Invalid object id: {obj_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    attr_name = request.match_info.get('name')
+    attr_name = request.match_info.get("name")
     log.debug(f"Attribute name: [{attr_name}]")
     validateAttributeName(attr_name)
 
     log.info(f"PUT Attribute Value id: {obj_id} name: {attr_name}")
     username, pswd = getUserPasswordFromRequest(request)
     # write actions need auth
     await validateUserPassword(app, username, pswd)
@@ -611,25 +628,25 @@
     domain_json = await getDomainJson(app, domain)
     verifyRoot(domain_json)
 
     # TBD - verify that the obj_id belongs to the given domain
     await validateAction(app, domain, obj_id, username, "update")
 
     req = getDataNodeUrl(app, obj_id)
-    req += '/' + collection + '/' + obj_id + "/attributes/" + attr_name
+    req += "/" + collection + "/" + obj_id + "/attributes/" + attr_name
     log.debug("get Attribute: " + req)
     params = {}
     if bucket:
         params["bucket"] = bucket
     dn_json = await http_get(app, req, params=params)
     log.debug("got attributes json from dn for obj_id: " + str(obj_id))
     log.debug(f"got dn_json: {dn_json}")
 
     attr_shape = dn_json["shape"]
-    if attr_shape["class"] == 'H5S_NULL':
+    if attr_shape["class"] == "H5S_NULL":
         msg = "Null space attributes can not be updated"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     np_shape = getShapeDims(attr_shape)
     type_json = dn_json["type"]
     np_dtype = createDataType(type_json)  # np datatype
@@ -649,15 +666,15 @@
         else:
             log.debug("PUT AttribueValue - request type is json")
 
     binary_data = None
     if request_type == "binary":
         item_size = getItemSize(type_json)
 
-        if item_size == 'H5T_VARIABLE':
+        if item_size == "H5T_VARIABLE":
             msg = "Only JSON is supported for variable length data types"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         # read binary data
         binary_data = await request.read()
         if len(binary_data) != request.content_length:
             msg = f"Read {len(binary_data)} bytes, expecting: "
@@ -665,26 +682,31 @@
             log.error(msg)
             raise HTTPInternalServerError()
 
     arr = None  # np array to hold request data
 
     if binary_data:
         npoints = getNumElements(np_shape)
-        if npoints*item_size != len(binary_data):
+        if npoints * item_size != len(binary_data):
             msg = f"Expected: {npoints*item_size} bytes, "
             msg += f"but got {len(binary_data)}"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         arr = np.fromstring(binary_data, dtype=np_dtype)
         arr = arr.reshape(np_shape)  # conform to selection shape
         # convert to JSON for transmission to DN
         data = arr.tolist()
         value = bytesArrayToList(data)
     else:
-        body = await request.json()
+        try:
+            body = await request.json()
+        except JSONDecodeError:
+            msg = "Unable to load JSON body"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
 
         if "value" not in body:
             msg = "PUT attribute value with no value in body"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         value = body["value"]
 
@@ -700,15 +722,15 @@
     # ready to add attribute now
     attr_json = {}
     attr_json["type"] = type_json
     attr_json["shape"] = attr_shape
     attr_json["value"] = value
 
     req = getDataNodeUrl(app, obj_id)
-    req += '/' + collection + '/' + obj_id + "/attributes/" + attr_name
+    req += "/" + collection + "/" + obj_id + "/attributes/" + attr_name
     log.info(f"PUT Attribute Value: {req}")
 
     dn_json["value"] = value
     params = {}
     params = {"replace": 1}  # let the DN know we can overwrite the attribute
     if bucket:
         params["bucket"] = bucket
```

### Comparing `hsds-0.7.0b11/hsds/basenode.py` & `hsds-0.8.0/hsds/basenode.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,26 +20,24 @@
 import random
 import psutil
 
 from aiohttp.web import Application
 from aiohttp.web_exceptions import HTTPNotFound, HTTPGone
 from aiohttp.web_exceptions import HTTPInternalServerError
 from aiohttp.web_exceptions import HTTPServiceUnavailable
-from aiohttp.client_exceptions import ClientError
-from asyncio import CancelledError
 
 from . import config
 from .util.httpUtil import http_get, http_post, jsonResponse
 from .util.idUtil import createNodeId, getNodeNumber, getNodeCount
 from .util.authUtil import getUserPasswordFromRequest, validateUserPassword
 from .util.authUtil import isAdminUser
-from .util.k8sClient import getPodIps
+from .util.k8sClient import getDnLabelSelector, getPodIps
 from . import hsds_logger as log
 
-HSDS_VERSION = "0.7.0beta"
+HSDS_VERSION = "0.8.0"
 
 
 def getVersion():
     return HSDS_VERSION
 
 
 def getHeadUrl(app):
@@ -97,154 +95,155 @@
         return None
     except Exception as e:
         log.warn(f"uncaught exception in get_info: {e}")
 
     return rsp_json
 
 
-async def oio_update_dn_info(app):
-    """ talk to conscience to get DN info """
-    oio_proxy = app["oio_proxy"]
-    if "HOST_IP" not in os.environ:
-        log.error("expected to find HOST_IP env variable")
-        return
-
-    node_ip = os.environ["HOST_IP"]
-    node_type = app["node_type"]
-    if node_type not in ("sn", "dn"):
-        log.error("unexpected node type")
-        return
-    service_name = "hdf" + node_type
-    req = oio_proxy + "/v3.0/OPENIO/conscience/register"
-
-    body = {
-        "addr": node_ip + ":" + str(app["node_port"]),
-        "tags": {"stat.cpu": 100, "tag.up": True},
-        "type": service_name
-    }
-    log.debug(f"conscience register: body: {body}")
-    try:
-        await http_post(app, req, data=body)
-    except ClientError as client_exception:
-        msg = "got ClientError registering with oio_proxy: "
-        msg += f"{client_exception} and body {body}"
-        log.error(msg)
-        return
-    except CancelledError as cancelled_exception:
-        msg = "got CancelledError registering with oio_proxy: "
-        msg += f"{cancelled_exception} and body {body}"
-        log.error(msg)
-        return
-    log.info("oio registration successful")
-
-    # get list of DN containers
-    req = oio_proxy + "/v3.0/OPENIO/conscience/list?type=hdfdn"
-    try:
-        dn_node_list = await http_get(app, req)
-    except ClientError as client_exception:
-        msg = "got ClientError listing dn nodes with oio_proxy: "
-        msg += f"{client_exception}"
-        log.error(msg)
-        return
-    except CancelledError as cancelled_exception:
-        msg = "got CancelledError listing dn nodes with oio_proxy: "
-        msg += f"{cancelled_exception}"
-        log.error(msg)
-        return
-    except BaseException as error:
-        log.error(f"A BaseException occurred: {error}")
-        return
-    log.info(f"got {len(dn_node_list)} conscience list items")
-    # create map keyed by dn addr
-    dn_urls = []
-    for dn_node in dn_node_list:
-        log.debug(f"checking dn conscience list item: {dn_node}")
-        if "addr" not in dn_node:
-            log.warn(f"conscience list item with no addr: {dn_node}")
-            continue
-        addr = dn_node["addr"]
-        if "score" not in dn_node:
-            log.warn(f'conscience list item with no score key: {dn_node}')
+async def k8s_get_dn_info(app, dn_urls=None):
+    # call info on each dn container and return map of info json key'd by dn_url
+    log.debug("k8s_get_dn_info")
+    info_map = {}
+    if dn_urls is None:
+        dn_urls = app["dn_urls"]
+    for dn_url in dn_urls:
+        req = dn_url + "/info"
+        log.debug(f"k8s_get_dn_urls - about to call: {req}")
+        # TBD - running these requests in a batch would be a bit faster
+        try:
+            rsp_json = await http_get(app, req)
+            if "node" not in rsp_json:
+                log.error("k8s_get_dn_urls - Unexpected response from info (no node key)")
+                continue
+            node_json = rsp_json["node"]
+            if "id" not in node_json:
+                log.error("k8s_get_dn_urls - Unexpected response from info (no node/id key)")
+                continue
+        except HTTPServiceUnavailable:
+            log.warn("k8s_get_dn_urls - 503 error from /info request")
             continue
-        if dn_node["score"] <= 0:
-            log.debug(f"zero score - skipping conscience list addr: {addr}")
+        except Exception as e:
+            log.error(f"k8s_get_dn_urls - Exception: {e} from /info request")
             continue
-        log.debug(f"oio_get_dn_urls - adding address: {addr}")
-        dn_urls.append("http://" + addr)
-
-    app["dn_urls"] = dn_urls
-
-    log.info(f"done with oio_update_dn_info, got: {len(dn_urls)} dn urls")
+        info_map[dn_url] = node_json
+        log.debug(f"adding {dn_url} to dn info map: {node_json}")
+    log.debug(f"k8s_get_dn_info, returning {len(info_map)} items")
+    return info_map
 
 
 async def k8s_update_dn_info(app):
-    """ update dn urls by querying k8s api.
-        Call each url to determine node_ids
+    """update dn urls by querying k8s api.
+    Call each url to determine node_ids
     """
     log.info("k8s_update_dn_info")
-    k8s_app_label = config.get("k8s_app_label")
-    # put import here to avoid k8s package dependency unless required
-    pod_ips = await getPodIps(k8s_app_label)
+    k8s_dn_label_selector = getDnLabelSelector(config)
+    pod_ips = await getPodIps(k8s_dn_label_selector)
     if not pod_ips:
         log.error("Expected to find at least one hsds pod")
         return
     pod_ips.sort()  # for assigning node numbers
     log.debug(f"got pod_ips: {pod_ips}")
+
     dn_port = config.get("dn_port")
     dn_urls = []
     for pod_ip in pod_ips:
         dn_urls.append(f"http://{pod_ip}:{dn_port}")
-    # call info on each dn container and get node ids
-    dn_ids = []
-    for dn_url in dn_urls:
-        req = dn_url + "/info"
-        log.debug(f"about to call: {req}")
-        try:
-            rsp_json = await http_get(app, req)
-            if "node" not in rsp_json:
-                log.error("Unexepected response from info (no node key)")
-                continue
-            node_json = rsp_json["node"]
-            if "id" not in node_json:
-                log.error("Unexpected response from info (no node/id key)")
-                continue
-            dn_ids.append(node_json["id"])
-        except HTTPServiceUnavailable:
-            log.warn("503 error from /info request")
-        except Exception as e:
-            log.error(f"Exception: {e} from /info request")
-    log.info(f"node_info check dn_ids: {dn_ids}")
 
-    # save to global
-    app["dn_urls"] = dn_urls
-    app["dn_ids"] = dn_ids
+    old_count = len(app["dn_urls"])
+    new_count = len(dn_urls)
+
+    if old_count != new_count:
+        log.info(f"pod count changed from {old_count} to {new_count}, fetch dn_ids")
+        scale_update = True
+    elif app["dn_urls"] != dn_urls:
+        log.info(f"pod ips have changed: {dn_urls}, fetch dn_ids")
+        scale_update = True
+    else:
+        scale_update = False
+
+    log.debug(f"scale_update: {scale_update}")
+    if scale_update:
+        # save to global
+        app["dn_urls"] = dn_urls
+        log.info(f"k8s_update_dn_info - dn_urls: {dn_urls}")
+        log.debug("scale_update is True, calling k8s_get_dn_info")
+        info_map = await k8s_get_dn_info(app, dn_urls=dn_urls)
+        dn_ids = []
+        dn_node_numbers = []
+        min_node_count = len(dn_urls)
+        max_node_count = len(dn_urls)
+        for dn_url in dn_urls:
+            if dn_url in info_map:
+                item = info_map[dn_url]
+                if "id" in item:
+                    dn_ids.append(item["id"])
+                if "node_number" in item:
+                    dn_node_numbers.append(item["node_number"])
+                if "node_count" in item:
+                    node_count = item["node_count"]
+                else:
+                    node_count = 0
+                if node_count < min_node_count:
+                    min_node_count = node_count
+                elif node_count > max_node_count:
+                    max_node_count = node_count
+
+        log.debug(f"scale update - min_node_count: {min_node_count}")
+        log.debug(f"scale update - max_node_couunt: {max_node_count}")
+        log.debug(f"scale_update - dn_node_numbers: {dn_node_numbers}")
+        log.debug(f"scale update - dn_ids: {dn_ids}")
+        # signal ready state by setting app["dn_ids"] only if:
+        #  1) node_count == len(dn_urls) for all dn's
+        #  2) dn_ids set for all nodes
+        #  3) dn node number are consecutive
+
+        consecutive = True
+        dn_node_numbers.sort()
+        for i in range(len(dn_node_numbers)):
+            if dn_node_numbers[i] != i:
+                consecutive = False
+                break
+
+        # save ids
+        log.info(f"scaling - updating dn_ids to: {dn_ids}")
+        app["dn_ids"] = dn_ids
+
+        if len(dn_ids) != new_count:
+            log.warn(f"scaling - got {len(dn_ids)} dn_ids expected {new_count}")
+        elif len(dn_node_numbers) != len(dn_urls):
+            log.warn(f"scaling - got {len(dn_node_numbers)} node numbers, expected {new_count}")
+        elif not consecutive:
+            log.warn(f"scaling - node_numbers not consecutive - got: {dn_node_numbers}")
+        else:
+            log.info("scaling - node numbers complete")
 
 
 async def docker_update_dn_info(app):
-    """ update list of dn_urls by making request to head node """
+    """update list of dn_urls by making request to head node"""
     head_url = getHeadUrl(app)
     if not head_url:
         log.warn("head_url is not set, can not register yet")
         return
     req_reg = head_url + "/register"
     log.info(f"register: {req_reg}")
 
-    body = {"id": app["id"],
-            "port": app["node_port"],
-            "node_type": app["node_type"]}
+    body = {"id": app["id"], "port": app["node_port"], "node_type": app["node_type"]}
+    rsp_json = None
 
     try:
         log.info(f"register req: {req_reg} body: {body}")
         rsp_json = await http_post(app, req_reg, data=body)
     except HTTPInternalServerError:
         log.error("HEAD node seems to be down.")
-        return []
+        app["dn_urls"] = []
+        app["dn_ids"] = []
     except OSError:
         log.error("failed to register")
-        return []
+        app["dn_urls"] = []
+        app["dn_ids"] = []
 
     if rsp_json is not None:
         log.info(f"register response: {rsp_json}")
         app["dn_urls"] = rsp_json["dn_urls"]
         app["dn_ids"] = rsp_json["dn_ids"]
 
 
@@ -253,106 +252,121 @@
     dn_ids = app["dn_ids"]
     for dn_id in dn_ids:
         id_set.add(dn_id)
     return id_set
 
 
 async def update_dn_info(app):
-    """ update http urls and ids for each dn node """
+    """update http urls and ids for each dn node"""
 
     if "is_standalone" in app:
         # nothing to do in standalone mode
         return
 
     id_set_pre = get_dn_id_set(app)
 
-    if "oio_proxy" in app:
-        #  Using OpenIO consicience daemons
-        await oio_update_dn_info(app)
-    elif "is_k8s" in app and not getHeadUrl(app):
+    if "is_k8s" in app and not getHeadUrl(app):
         await k8s_update_dn_info(app)
     else:
         # docker or kubernetes running with head container
         await docker_update_dn_info(app)
 
     # do a log if there has been a change in the dn nodes
     id_set_post = get_dn_id_set(app)
+    log.debug(f"update_dn_info - id_set_post: {id_set_post}")
     if id_set_pre != id_set_post:
         gone_ids = id_set_pre.difference(id_set_post)
         if gone_ids:
             msg = f"update_dn_info - dn_nodes: {gone_ids} "
             msg += "are no longer active"
             log.info(msg)
         new_ids = id_set_post.difference(id_set_pre)
         if new_ids:
             log.info(f"update_dn_info - dn_nodes: {new_ids} are now active")
 
 
-def updateReadyState(app):
-    """ update node state (and node_number and node_count) based on number
-        of dn_urls available
+def updateReadyState(app, old_dn_urls=None):
+    """update node state (and node_number and node_count) based on number
+    of dn_urls available
     """
     if "is_standalone" in app:
         # dn_urls don't change in standalone mode, so just return
         log.debug("skip updateReadyState for standalone app")
         return
     dn_urls = app["dn_urls"]
-    log.debug(f"updateReadyState for dn_urls: {dn_urls}")
-    if len(dn_urls) == 0:
-        if app["node_type"] == "dn":
-            log.error("no dn_urls returned from dn node!")
-        if app["node_state"] != "INITIALIZING":
-            msg = f"setting node_state from {app['node_state']} to "
-            msg += "INITIALIZING since there are no dn nodes"
-            log.info(msg)
-            app["node_state"] = "INITIALIZING"
-    elif app["node_type"] == "dn":
+    dn_ids = app["dn_ids"]
+    log.debug(f"updateReadyState - for old_dn_urls: {old_dn_urls}")
+    log.debug(f"updateReadyState - for new dn_urls: {dn_urls}")
+    log.debug(f"updateReadyState - dn_ids: {dn_ids}")
+
+    is_ready = True
+    if len(dn_urls) == 0 or len(dn_urls) != len(dn_ids):
+        if len(dn_urls) > 0:
+            log.warning(f"not all dn_ids found, got: {dn_ids}")
+        is_ready = False
+
+    if app["node_type"] == "dn":
+        # dn node
+        old_number = app["node_number"]
         node_number = getNodeNumber(app)
-        if app["node_number"] != node_number:
-            old_number = app["node_number"]
-            msg = f"node_number has changed - old value was {old_number} "
-            msg += f"new number is {node_number}"
+        if old_number != node_number:
+            msg = f"node_number was {old_number}, setting to: {node_number}"
             log.info(msg)
             meta_cache = app["meta_cache"]
             chunk_cache = app["chunk_cache"]
             dirty_cache_count = meta_cache.dirtyCount + chunk_cache.dirtyCount
             if dirty_cache_count > 0:
                 # set the node state to waiting till the chunk cache have
                 # been flushed
-                msg = f"Waiting on {dirty_cache_count} cache items to be "
-                msg += "flushed"
+                msg = f"updateReadyState - waiting on {dirty_cache_count} "
+                msg += "cache items to be flushed"
                 log.info(msg)
-                if app["node_state"] == "READY":
-                    log.info("Setting node_state to WAITING (was READY)")
-                    app["node_state"] = "WAITING"
+                is_ready = False
             else:
                 # flush remaining items from cache
                 meta_cache.clearCache()
                 chunk_cache.clearCache()
-                msg = f"setting node_number to: {node_number}, node_state "
-                msg += "to READY"
+                msg = f"scaling - setting node_number to: {node_number} (old value: {old_number}"
                 log.info(msg)
                 app["node_number"] = node_number
-                app["node_state"] = "READY"
     else:
-        # sn node with at least one dn node
-        old_count = getNodeCount(app)
+        # sn node
+        if old_dn_urls:
+            old_count = len(old_dn_urls)
+        else:
+            old_count = 0
         new_count = len(dn_urls)
         if old_count != new_count:
-            msg = f"number of dn nodes has changed from {old_count} "
+            msg = f"scaling - number of dn nodes has changed from {old_count} "
             msg += f"to {new_count}"
             log.info(msg)
-        if app["node_state"] != "READY":
-            log.info(f"setting node_state from {app['node_state']} to READY")
+
+    # finally, change state if indicated
+    node_state = app["node_state"]
+    if node_state == "READY":
+        if not is_ready:
+            log.info("setting node_state from READY to WAITING")
+            app["node_state"] = "WAITING"
+    elif node_state == "WAITING":
+        if is_ready:
+            log.info("setting node_state from WAITING to READY")
             app["node_state"] = "READY"
+    elif node_state == "INITIALIZING":
+        if is_ready:
+            log.info("setting node_state from INITIALIZING to READY")
+    elif node_state == "TERMINATING":
+        if is_ready:
+            log.warn("got is_ready for node in TERMINATING state")
+    else:
+        log.error(f"unexpected node_state: {node_state}")
 
 
 def _activeTaskCount():
     count = 0
-    for task in asyncio.Task.all_tasks():
+    for task in asyncio.all_tasks():
         if not task.done():
             count += 1
     return count
 
 
 async def doHealthCheck(app, chaos_die=0):
     node_state = app["node_state"]
@@ -360,28 +374,29 @@
         if random.randint(0, chaos_die) == 0:
             log.error("chaos die - suicide!")
             sys.exit(1)
         else:
             log.info("chaos die - still alive")
     log.info(f"healthCheck - node_state: {node_state}")
     if node_state != "TERMINATING":
-        await update_dn_info(app)
-        updateReadyState(app)
+        old_dn_urls = app["dn_urls"]
+        await update_dn_info(app)  # may update app["dn_urls"]
+        updateReadyState(app, old_dn_urls=old_dn_urls)
 
     svmem = psutil.virtual_memory()
-    num_tasks = len(asyncio.Task.all_tasks())
+    num_tasks = len(asyncio.all_tasks())
     msg = f"health check vm: {svmem.percent} num tasks: {num_tasks} "
     msg += f"active tasks: {_activeTaskCount()}"
     log.debug(msg)
 
 
 async def healthCheck(app):
-    """ Periodic method that either registers with headnode (if state in
-        INITIALIZING) or calls headnode to verify vitals about this node
-        (otherwise)
+    """Periodic method that either registers with headnode (if state in
+    INITIALIZING) or calls headnode to verify vitals about this node
+    (otherwise)
     """
 
     # let the server event loop startup before starting the health check
     await asyncio.sleep(1)
     log.info("health check start")
     sleep_secs = config.get("node_sleep_time")
     chaos_die = config.get("chaos_die")
@@ -394,39 +409,25 @@
         except Exception as e:
             msg = f"Unexpected {e.__class__.__name__} exception in "
             msg += f"doHealthCheck: {e}"
             log.error(msg)
         await asyncio.sleep(sleep_secs)
 
 
-async def preStop(request):
-    """ HTTP Method used by K8s to signal the container is shutting down
-    """
-
-    log.request(request)
-    app = request.app
-    app["node_state"] = "TERMINATING"
-    log.warn("preStop request setting node_state to TERMINATING")
-
-    resp = await jsonResponse(request, {})
-    log.response(request, resp=resp)
-    return resp
-
-
 async def about(request):
-    """ HTTP Method to return general info about the service """
+    """HTTP Method to return general info about the service"""
     log.request(request)
 
     app = request.app
     (username, pswd) = getUserPasswordFromRequest(request)
     if username:
         await validateUserPassword(app, username, pswd)
     answer = {}
-    answer['start_time'] = app["start_time"]
-    answer['state'] = app['node_state']
+    answer["start_time"] = app["start_time"]
+    answer["state"] = app["node_state"]
     answer["hsds_version"] = getVersion()
     answer["name"] = config.get("server_name")
     answer["greeting"] = config.get("greeting")
     answer["about"] = config.get("about")
     answer["node_count"] = getNodeCount(app)
     answer["dn_urls"] = app["dn_urls"]
     answer["dn_ids"] = app["dn_ids"]
@@ -447,21 +448,21 @@
 async def info(request):
     """HTTP Method to return node state to caller"""
     log.request(request)
     app = request.app
     answer = {}
     # copy relevant entries from state dictionary to response
     node = {}
-    node['id'] = app['id']
-    node['type'] = app['node_type']
-    node['start_time'] = app["start_time"]
-    node['state'] = app['node_state']
-    if app['node_type'] == 'dn':
-        node['node_number'] = app['node_number']
-    node['node_count'] = getNodeCount(app)
+    node["id"] = app["id"]
+    node["type"] = app["node_type"]
+    node["start_time"] = app["start_time"]
+    node["state"] = app["node_state"]
+    if app["node_type"] == "dn":
+        node["node_number"] = app["node_number"]
+    node["node_count"] = getNodeCount(app)
 
     answer["node"] = node
     # psutil info
     # see: http://pythonhosted.org/psutil/ for description of different fields
     cpu = {}
     cpu["percent"] = psutil.cpu_percent()
     cpu["cores"] = psutil.cpu_count()
@@ -493,15 +494,15 @@
     sswap = psutil.swap_memory()
     mem_stats["swap_total"] = sswap.total
     mem_stats["swap_used"] = sswap.used
     mem_stats["swap_free"] = sswap.free
     mem_stats["percent"] = sswap.percent
     answer["memory"] = mem_stats
     disk_stats = {}
-    sdiskusage = psutil.disk_usage('/')
+    sdiskusage = psutil.disk_usage("/")
     disk_stats["total"] = sdiskusage.total
     disk_stats["used"] = sdiskusage.used
     disk_stats["free"] = sdiskusage.free
     disk_stats["percent"] = sdiskusage.percent
     answer["disk"] = disk_stats
     answer["log_stats"] = log.log_count
     answer["req_count"] = log.req_count
@@ -537,33 +538,33 @@
         dc_stats["mem_target"] = dc.memTarget
     answer["domain_cache_stats"] = dc_stats
 
     resp = await jsonResponse(request, answer)
     log.response(request, resp=resp)
     return resp
 
+
 def baseInit(node_type):
     """Intitialize application and return app object"""
 
     # setup log config
     log_level = config.get("log_level")
     prefix = config.get("log_prefix")
     log_timestamps = config.get("log_timestamps", default=False)
     log.setLogConfig(log_level, prefix=prefix, timestamps=log_timestamps)
-     
 
     # create the app object
     log.info("Application baseInit")
     app = Application()
 
     app["node_state"] = "INITIALIZING"
     app["node_number"] = -1
     app["node_type"] = node_type
     app["start_time"] = int(time.time())  # seconds after epoch
-    app['register_time'] = 0
+    app["register_time"] = 0
     app["max_task_count"] = config.get("max_task_count")
 
     is_standalone = config.getCmdLineArg("standalone")
 
     if is_standalone:
         log.info("running in standalone mode")
         app["is_standalone"] = True
@@ -596,21 +597,23 @@
 
     bucket_name = config.get("bucket_name")
     if bucket_name:
         log.info(f"using bucket: {bucket_name}")
     else:
         log.info("no default bucket defined")
     app["bucket_name"] = bucket_name
+    app["allow_any_bucket_read"] = config.get("allow_any_bucket_read", default=True)
+    app["allow_any_bucket_write"] = config.get("allow_any_bucket_write", default=True)
     app["dn_urls"] = []
     app["dn_ids"] = []  # node ids for each dn_url
-     
+
     if is_standalone:
-        dn_urls_arg = config.getCmdLineArg("dn_urls")  
+        dn_urls_arg = config.getCmdLineArg("dn_urls")
         if dn_urls_arg:
-            dn_urls = dn_urls_arg.split(',')
+            dn_urls = dn_urls_arg.split(",")
             dn_urls.sort()
             dn_ids = []
             for i in range(len(dn_urls)):
                 dn_url = dn_urls[i]
                 if not dn_url.startswith("http"):
                     log.warn(f"Unexpected dn_url value: {dn_url}, type: {type(dn_url)}")
                 dn_id = createNodeId("dn", node_number=i)
@@ -621,54 +624,44 @@
                 log.error(msg)
                 raise ValueError(msg)
             dn_urls = []
             dn_ids = []
 
         app["dn_urls"] = dn_urls
         app["dn_ids"] = dn_ids
-        rangeget_url = config.getCmdLineArg("rangeget_url")
-        if rangeget_url:
-            log.debug(f"store rangeget_url: {rangeget_url}")
-            app["rangeget_url"] = rangeget_url
-        
+
         # check to see if we are running in a DCOS cluster
+    elif "IS_DOCKER" in os.environ:
+        log.info("running in docker")
+        app["is_docker"] = True
     elif "MARATHON_APP_ID" in os.environ:
         msg = "Found MARATHON_APP_ID environment variable, "
         msg += "setting is_dcos to True"
         log.info(msg)
         app["is_dcos"] = True
-    elif "OIO_PROXY" in os.environ:
-        app["oio_proxy"] = os.environ["OIO_PROXY"]
-        # will set node_ip at registration time
-    else:
-        # check to see if we are running in a k8s cluster
-        if "KUBERNETES_SERVICE_HOST" in os.environ:
-            log.info("running in kubernetes")
-            app["is_k8s"] = True
-        else:
-            # check to see if we are running in a docker container
-            proc_file = "/proc/self/cgroup"
-            if os.path.isfile(proc_file):
-                with open(proc_file) as f:
-                    first_line = f.readline()
-                    if first_line:
-                        fields = first_line.split(':')
-                        if len(fields) >= 3:
-                            field = fields[2]
-                            if field.startswith("/docker/"):
-                                log.info("running in docker")
-                                app["is_docker"] = True
+    elif "KUBERNETES_SERVICE_HOST" in os.environ:
+        # indicates we are running in a k8s cluster
+        log.info("running in kubernetes")
+        app["is_k8s"] = True
+    else:
+        # check the root inode - high values indicate
+        # we are running in a container
+        if os.path.isdir("/"):
+            stat = os.stat("/")
+            if stat and stat.st_ino > 10:
+                log.info("running in docker based on inode number")
+                app["is_docker"] = True
 
     if "is_dcos" in app:
         if "PORT0" not in os.environ:
             msg = "Expected PORT0 environment variable for DCOS"
             log.error(msg)
             node_port = config.get(node_type + "_port")
         else:
-            node_port = os.environ['PORT0']
+            node_port = os.environ["PORT0"]
     else:
         node_port = config.get(node_type + "_port")
         log.info(f"using node port: {node_port}")
         app["node_port"] = node_port
 
     try:
         aws_iam_role = config.get("aws_iam_role")
@@ -693,21 +686,19 @@
         log.info("aws_access_key_id not set")
     try:
         aws_region = config.get("aws_region")
         log.info(f"aws_region set to: {aws_region}")
     except KeyError:
         log.info("aws_region not set")
 
-    app.router.add_get('/info', info)
-    app.router.add_get('/about', about)
+    app.router.add_get("/info", info)
+    app.router.add_get("/about", about)
 
     if is_standalone:
         # can go straight to ready state
-        msg = "setting cluster_state to inital state of READY for standalone"
+        msg = "setting node_state to inital state of READY for standalone"
         log.info(msg)
-        app["cluster_state"] = "READY"
-        app['node_state'] = "READY"
+        app["node_state"] = "READY"
     else:
-        app["custer_state"] = "WAITING"
-
+        app["node_state"] = "WAITING"
 
     return app
```

### Comparing `hsds-0.7.0b11/hsds/chunk_dn.py` & `hsds-0.8.0/hsds/util/httpUtil.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,596 +3,675 @@
 # All rights reserved.                                                       #
 #                                                                            #
 # This file is part of HSDS (HDF5 Scalable Data Service), Libraries and      #
 # Utilities.  The full HSDS copyright notice, including                      #
 # terms governing use, modification, and redistribution, is contained in     #
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
-# request a copy from help@hdfgroup.org.                                     #
+# request a copy from  help@hdfgroup.org.                                     #
 ##############################################################################
 #
-# value operations
-# handles regauests to read/write chunk data
-#
+# httpUtil:
+# http-related helper functions
 #
+from asyncio import CancelledError
+import os
+import socket
 import numpy as np
-from aiohttp.web_exceptions import HTTPBadRequest, HTTPInternalServerError
-from aiohttp.web_exceptions import HTTPNotFound
-from aiohttp.web import json_response, StreamResponse
-
-from .util.httpUtil import request_read
-from .util.arrayUtil import bytesToArray, arrayToBytes
-from .util.idUtil import getS3Key, validateInPartition, isValidUuid
-from .util.storUtil import isStorObj, deleteStorObj
-from .util.hdf5dtype import createDataType
-from .util.dsetUtil import getSelectionList, getChunkLayout
-from .util.dsetUtil import getSelectionShape
-from .util.chunkUtil import getChunkIndex, getDatasetId, chunkQuery
-from .util.chunkUtil import chunkWriteSelection, chunkReadSelection
-from .util.chunkUtil import chunkWritePoints, chunkReadPoints
-from .datanode_lib import get_metadata_obj, get_chunk, save_chunk
-
-from . import hsds_logger as log
-from . import config
+from aiohttp.web import json_response
+import simplejson
+from aiohttp import ClientSession, UnixConnector, TCPConnector
+from aiohttp.web_exceptions import HTTPForbidden, HTTPNotFound, HTTPConflict
+from aiohttp.web_exceptions import HTTPGone, HTTPInternalServerError
+from aiohttp.web_exceptions import HTTPRequestEntityTooLarge
+from aiohttp.web_exceptions import HTTPServiceUnavailable, HTTPBadRequest
+from aiohttp.client_exceptions import ClientError
+from hsds.util.idUtil import isValidUuid
+
+from .. import hsds_logger as log
+from .. import config
+
+
+def isOK(http_response):
+    """return True for successful http_status codes"""
+    if http_response < 300:
+        return True
+    return False
+
+
+def getUrl(host, port):
+    """return url for host and port"""
+    return f"http://{host}:{port}"
+
+
+def getPortFromUrl(url):
+    """Get Port number for given url"""
+    if not url:
+        raise ValueError("url undefined")
+    if url.startswith("http://"):
+        default_port = 80
+    elif url.startswith("https://"):
+        default_port = 443
+    elif url.startswith("http+unix://"):
+        # unix domain socket
+        return None
+    else:
+        raise ValueError(f"Invalid Url: {url}")
+
+    start = url.find("//")
+    port = None
+    dns = url[start:]
+    index = dns.find(":")
+    port_str = ""
+    if index > 0:
+        for i in range(index + 1, len(dns)):
+            ch = dns[i]
+            if ch.isdigit():
+                port_str += ch
+            else:
+                break
+    if port_str:
+        port = int(port_str)
+    else:
+        port = default_port
+
+    return port
+
+
+def isUnixDomainUrl(url):
+    # return True if url is a Unix Socket domain
+    # e.g. http://unix:%2Ftmp%2Fdn_1.sock/about -> True
+    #      http://localhost:80 -> False
+    if not url:
+        raise ValueError("url undefined")
+    if not url.startswith("http"):
+        raise ValueError(f"invalid url, no http: {url}")
+    if url.startswith("http+unix:"):
+        if not url.startswith("http+unix://"):
+            raise ValueError(f"invalid socket url: {url}")
+        return True
+    else:
+        return False
+
+
+def getSocketPath(url):
+    # return socket path part of the url
+    # E.g. for "http+unix://%2Ftmp%2Fdn_1.sock/about" return "/tmp/dn_1.sock"
+    if not isUnixDomainUrl(url):
+        return None
+    # url must start with http+unix://:
+    skip = len("http+unix://")
+    chars = []
+    # TBD - replace with proper url-decode
+    for i in range(len(url)):
+        if skip:
+            skip -= 1
+        elif url[i] == "/":
+            break
+        elif url[i] == "%" and url[i + 1] == "2" and url[i + 2] == "F":
+            chars.append("/")
+            skip = 2
+        else:
+            chars.append(url[i])
+    return "".join(chars)
 
 
-async def PUT_Chunk(request):
+def bindToSocket(url):
     """
-    Update the requested chunk/selection
+    Bind to socket specified by http+unix url
     """
-    log.request(request)
-    app = request.app
-    params = request.rel_url.query
-    query = None
-    query_update = None
-    limit = 0
-    bucket = None
-    input_arr = None
-
-    if "query" in params:
-        query = params["query"]
-        log.info(f"PUT_Chunk query: {query}")
-    if "Limit" in params:
-        limit = int(params["Limit"])
-    chunk_id = request.match_info.get('id')
-    if not chunk_id:
-        msg = "Missing chunk id"
-        log.error(msg)
-        raise HTTPBadRequest(reason=msg)
-    if not isValidUuid(chunk_id, "Chunk"):
-        msg = f"Invalid chunk id: {chunk_id}"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
-
-    if not request.has_body:
-        msg = "PUT Value with no body"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
-    if "bucket" in params:
-        bucket = params["bucket"]
-        log.debug(f"PUT_Chunk using bucket: {bucket}")
-    
-    if not bucket:
-        msg = "PUT_Chunk - bucket is None"
-        log.warn(msg)
-        raise HTTPInternalServerError(reason=msg)
+    if not isUnixDomainUrl(url):
+        raise ValueError(f"Invalid url for bindToSocket: {url}")
+    # use a unix domain socket path
+    path = getSocketPath(url)
+    log.debug(f"got socketpath: {path}")
+    # first, make sure the socket does not already exist
+    try:
+        os.unlink(path)
+    except OSError:
+        if os.path.exists(path):
+            raise
+    s = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
+    s.bind(path)
+    return s
+
+
+def get_http_std_url(url):
+    # replace socket path (if exists) with 127.0.0.1
+    if not isUnixDomainUrl(url):
+        return url
+    index = url.find(".sock")
+    n = index + 5
+    url = "http://127.0.0.1" + url[n:]
+    return url
+
+
+def get_base_url(url):
+    """return protocal+dns+port part of url.
+    Returns just url if a non-standard protocol is given."""
+    n = len(url)
+    for protocol in ("http://", "https://", "http+unix://"):
+        if url.startswith(protocol):
+            start = len(protocol)
+            n = url.find("/", start)
+            if n < 0:
+                n = len(url)
+            break
+    s = url[:n]
+    return s
+
+
+def get_http_client(app, url=None, cache_client=True):
+    """get http client"""
+    log.debug(f"get_http_client, url: {url}")
+    if url is None or not isUnixDomainUrl(url):
+        socket_path = None
+    else:
+        socket_path = getSocketPath(url)
+        log.debug(f"socket_path: {socket_path}")
+
+    if cache_client:
+        if "client" in app and not socket_path:
+            return app["client"]
+        if socket_path:
+            if "socket_clients" not in app:
+                app["socket_clients"] = {}
+            socket_clients = app["socket_clients"]
+            if socket_path in socket_clients:
+                return socket_clients[socket_path]
+
+    # first time call, create client interface
+    # use shared client so that all client requests
+    #   will share the same connection pool
+
+    if socket_path:
+        log.info(f"Initiating UnixConnector with path: {socket_path}")
+        client = ClientSession(connector=UnixConnector(path=socket_path))
+        if cache_client:
+            socket_clients[socket_path] = client
+        log.info(f"Socket Ready: {socket_path}")
+    else:
+        max_tcp_connections = int(config.get("max_tcp_connections"))
+        msg = f"Initiating TCPConnector for {url} with limit "
+        msg += f"{max_tcp_connections} connections"
+        log.info(msg)
+        kwargs = {"limit_per_host": max_tcp_connections}
+        # not yet supported in this aiohttp version
+        # read_buf_size = config.get("read_buf_size", default=10*1024*1024)
+        # log.debug(f"setting read_buf_size to: {read_buf_size}")
+        # kwargs['read_bufsize'] = read_buf_size
+        client = ClientSession(connector=TCPConnector(**kwargs))
+        if cache_client:
+            app["client"] = client
 
-    if query:
-        chunk_init = False  # don't initalize new chunks on query update
-    else:
-        chunk_init = True
+    # return client instance
+    return client
 
+
+async def release_http_client(app):
+    """
+    Release any http clients
+    """
+    log.info("releasing http clients")
+    if "client" in app:
+        client = app["client"]
+        await client.close()
+        del app["client"]
+    if "socket_clients" in app:
+        socket_clients = app["socket_clients"]
+        for socket_path in socket_clients:
+            client = socket_clients[socket_path]
+            await client.close()
+        app["socket_clients"] = {}
+
+
+async def request_read(request, count=None) -> bytes:
+    """
+    Replacement for aiohttp Request.read using our max request limit
+    Read request body if present.
+
+    Returns bytes object with full request content,
+       or next count bytes if count is set
+    """
+    log.debug(f"request_read - count: {count}")
+    body = bytearray()
+    max_request_size = int(config.get("max_request_size"))
+    while True:
+        if count is not None:
+            chunk = await request._payload.readexactly(count)
+            count -= len(chunk)
+        else:
+            chunk = await request._payload.readany()
+        body.extend(chunk)
+        body_size = len(body)
+        if body_size >= max_request_size:
+            raise HTTPRequestEntityTooLarge(
+                max_size=max_request_size, actual_size=body_size
+            )
+        if not chunk:
+            break
+        if count is not None and count <= 0:
+            break
+    return bytes(body)
+
+
+async def http_get(app, url, params=None, client=None):
+    """
+    Helper function  - async HTTP GET
+    """
+    log.info(f"http_get('{url}')")
+    if client is None:
+        client = get_http_client(app, url=url)
+    url = get_http_std_url(url)
+    status_code = None
+    timeout = config.get("timeout")
+    # TBD: use read_bufsize parameter to optimize read for large responses
     try:
-        validateInPartition(app, chunk_id)
-    except KeyError:
-        msg = f"invalid partition for obj id: {chunk_id}"
-        log.error(msg)
+        async with client.get(url, params=params, timeout=timeout) as rsp:
+            log.info(f"http_get status: {rsp.status} for req: {url}")
+            status_code = rsp.status
+            if rsp.status == 200:
+                # 200, so read the response
+                if isBinaryResponse(rsp):
+                    # return binary data
+                    retval = await rsp.read()  # read response as bytes
+                else:
+                    retval = await rsp.json()
+            elif status_code == 400:
+                log.info(f"BadRequest to {url}")
+                raise HTTPBadRequest()
+            elif status_code == 403:
+                log.info(f"Forbiden to access {url}")
+                raise HTTPForbidden()
+            elif status_code == 404:
+                log.info(f"Object: {url} not found")
+                raise HTTPNotFound()
+            elif status_code == 410:
+                log.info(f"Object: {url} removed")
+                raise HTTPGone()
+            elif status_code == 503:
+                log.warn(f"503 error for http_get_Json {url}")
+                raise HTTPServiceUnavailable()
+            else:
+                log.error(f"request to {url} failed with code: {status_code}")
+                raise HTTPInternalServerError()
+
+    except ClientError as ce:
+        log.warn(f"ClientError: {ce}")
+        raise HTTPInternalServerError()
+    except CancelledError as cle:
+        log.warn(f"CancelledError for http_get({url}): {cle}")
         raise HTTPInternalServerError()
 
-    if "dset" in params:
-        msg = "Unexpected param dset in PUT request"
-        log.error(msg)
-        raise HTTPBadRequest(reason=msg)
+    return retval
 
-    log.debug(f"PUT_Chunk - id: {chunk_id}")
 
-    dset_id = getDatasetId(chunk_id)
+async def http_post(app, url, data=None, params=None, client=None):
+    """
+    Helper function  - async HTTP POST
+    """
+    log.info(f"http_post('{url}', {len(data)} bytes)")
+    if client is None:
+        client = get_http_client(app, url=url)
+    url = get_http_std_url(url)
+    if isinstance(data, bytes):
+        log.debug("setting http_post for binary")
+        kwargs = {"data": data}
+    else:
+        kwargs = {"json": data}
+    timeout = config.get("timeout")
+    if timeout:
+        kwargs["timeout"] = timeout
+    if params:
+        kwargs["params"] = params
 
-    dset_json = await get_metadata_obj(app, dset_id, bucket=bucket)
+    try:
+        async with client.post(url, **kwargs) as rsp:
+            log.info(f"http_post status: {rsp.status}")
+            if rsp.status == 200:
+                pass  # ok
+            elif rsp.status == 201:
+                pass  # also ok
+            elif rsp.status == 204:  # no data
+                return None
+            elif rsp.status == 400:
+                msg = f"POST  request HTTPBadRequest error for url: {url}"
+                log.info(msg)
+                raise HTTPBadRequest()
+            elif rsp.status == 404:
+                msg = f"POST  request HTTPNotFound error for url: {url}"
+                log.info(msg)
+                raise HTTPNotFound()
+            elif rsp.status == 410:
+                log.info(f"POST  request HTTPGone error for url: {url}")
+                raise HTTPGone()
+            elif rsp.status == 503:
+                log.warn(f"503 error for http_get_Json {url}")
+                raise HTTPServiceUnavailable()
+            else:
+                msg = f"POST request error for url: {url} status: {rsp.status}"
+                log.warn(msg)
+                raise HTTPInternalServerError()
+            if isBinaryResponse(rsp):
+                # return binary data
+                retval = await (rsp.read())
+                log.debug(f"http_post({url}) returning {len(retval)} bytes")
+            else:
+                retval = await rsp.json()
+                log.debug(f"http_post({url}) response: {retval}")
+
+    except ClientError as ce:
+        log.warn(f"ClientError for http_post({url}): {ce} ")
+        raise HTTPInternalServerError()
+    except CancelledError as cle:
+        log.warn(f"CancelledError for http_post({url}): {cle}")
+        raise HTTPInternalServerError()
 
-    # TBD - does this work with linked datasets?
-    dims = getChunkLayout(dset_json)
-    log.debug(f"got dims: {dims}")
-    rank = len(dims)
+    return retval
 
-    type_json = dset_json["type"]
-    dt = createDataType(type_json)
-    log.debug(f"dtype: {dt}")
-    itemsize = 'H5T_VARIABLE'
-    if "size" in type_json:
-        itemsize = type_json["size"]
 
-    # get chunk selection from query params
-    if "select" in params:
-        select = params["select"]
-    else:
-        select = None # put for entire dataspace
+async def http_put(app, url, data=None, params=None, client=None):
+    """
+    Helper function  - async HTTP PUT
+    """
+    log.info(f"http_put('{url}')")
+    if client is None:
+        client = get_http_client(app, url=url)
+    url = get_http_std_url(url)
+    if isinstance(data, bytes):
+        log.debug("setting http_put for binary")
+        kwargs = {"data": data}
+    else:
+        log.debug("setting http_put for json")
+        kwargs = {"json": data}
+
+    rsp_json = None
+    if params is not None:
+        kwargs["params"] = params
+    timeout = config.get("timeout")
+    if timeout:
+        kwargs["timeout"] = timeout
+
     try:
-        selection = getSelectionList(select, dims)
-    except ValueError as ve:
-        log.error(f"ValueError for select: {select}: {ve}")
+        async with client.put(url, **kwargs) as rsp:
+            log.info(f"http_put status: {rsp.status}")
+            if rsp.status in (200, 201):
+                pass  # expected
+            elif rsp.status == 404:
+                # can come up for replace ops
+                log.info(f"HTTPNotFound for: {url}")
+            elif rsp.status == 409:
+                log.info(f"HTTPConflict for: {url}")
+                raise HTTPConflict()
+            elif rsp.status == 503:
+                log.warn(f"503 error for http_put url: {url}")
+                raise HTTPServiceUnavailable()
+            else:
+                msg = f"PUT request error for url: {url} status: {rsp.status}"
+                log.error(msg)
+                raise HTTPInternalServerError()
+            if isBinaryResponse(rsp):
+                # return binary data
+                retval = await rsp.read()  # read response as bytes
+                log.debug(f"http_put({url}): return {len(retval)} bytes")
+            else:
+                retval = await rsp.json()
+                log.debug(f"http_put({url}) response: {rsp_json}")
+    except ClientError as ce:
+        log.warn(f"ClientError for http_put({url}): {ce} ")
         raise HTTPInternalServerError()
-    log.debug(f"got selection: {selection}")
+    except CancelledError as cle:
+        log.warn(f"CancelledError for http_put({url}): {cle}")
+        raise HTTPInternalServerError()
+    return retval
 
-    mshape = getSelectionShape(selection)
-    log.debug(f"mshape: {mshape}")
-    num_elements = 1
-    for extent in mshape:
-        num_elements *= extent
-    kwargs = {"bucket": bucket, "chunk_init": chunk_init}
-    chunk_arr = await get_chunk(app, chunk_id, dset_json, **kwargs)
-    is_dirty = False
-    if chunk_arr is None:
-        if chunk_init:
-            log.error("failed to create numpy array")
-            raise HTTPInternalServerError()
-        else:
-            log.warn(f"chunk {chunk_id} not found")
-            raise HTTPNotFound()
 
-    if query:
-        if not dt.fields:
-            log.error("expected compound dtype for PUT query")
-            raise HTTPInternalServerError()
-        if rank != 1:
-            log.error("expected one-dimensional array for PUT query")
-            raise HTTPInternalServerError()
-        query_update = await request.json()
-        log.debug(f"query_update: {query_update}")
-        # TBD - send back binary response to SN node
-        try:
-            kwargs = {"chunk_id": chunk_id,
-                      "chunk_layout": dims,
-                      "chunk_arr": chunk_arr,
-                      "slices": selection,
-                      "query": query,
-                      "query_update": query_update,
-                      "limit": limit,
-                      "return_json": True}
-            resp = chunkQuery(**kwargs)
-        except TypeError as te:
-            log.warn(f"chunkQuery - TypeError: {te}")
-            raise HTTPBadRequest()
-        except ValueError as ve:
-            log.warn(f"chunkQuery - ValueError: {ve}")
-            raise HTTPBadRequest()
-        if query_update and resp is not None:
-            is_dirty = True
-    else:
-        # regular chunk update
-
-        # check that the content_length is what we expect
-        if itemsize != 'H5T_VARIABLE':
-            log.debug(f"expect content_length: {num_elements*itemsize}")
-        log.debug(f"actual content_length: {request.content_length}")
-
-        expected = num_elements*itemsize
-        actual = request.content_length
-        if itemsize != 'H5T_VARIABLE' and expected != actual:
-            msg = f"Expected content_length of: {expected}, but got: {actual}"
-            log.error(msg)
-            raise HTTPBadRequest(reason=msg)
+async def http_delete(app, url, data=None, params=None, client=None):
+    """
+    Helper function  - async HTTP DELETE
+    """
+    # TBD - do we really need a data param?
+    log.info(f"http_delete('{url}')")
+    if client is None:
+        client = get_http_client(app, url=url)
+    url = get_http_std_url(url)
+
+    rsp_json = None
+    kwargs = {}
+    timeout = config.get("timeout")
+    if timeout:
+        kwargs["timeout"] = timeout
+    if params:
+        kwargs["params"] = params
+    if data:
+        params["json"] = data
 
-        # create a numpy array for incoming data
-        input_bytes = await request_read(request)
-        # TBD - will it cause problems when failures are raised before
-        #    reading data?
-        if len(input_bytes) != actual:
-            msg = f"Read {len(input_bytes)} bytes, expecting: {actual}"
-            log.error(msg)
-            raise HTTPInternalServerError()
-
-        input_arr = bytesToArray(input_bytes, dt, mshape)
-        kwargs = {"chunk_arr": chunk_arr,
-                  "slices": selection,
-                  "data": input_arr}
-        is_dirty = chunkWriteSelection(**kwargs)
-
-        # chunk update successful
-        resp = {}
-    if is_dirty or config.get("write_zero_chunks", default=False):
-        save_chunk(app, chunk_id, dset_json, bucket=bucket)
-        status_code = 201
-    else:
-        status_code = 200
-
-    resp = json_response(resp, status=status_code)
-    log.response(request, resp=resp)
-    return resp
-
-
-async def GET_Chunk(request):
-    """
-    Return data from requested chunk and selection
-    """
-    log.request(request)
-
-    bucket = None
-    s3path = None
-    s3offset = None
-    s3size = None
-    query = None
-    limit = 0
+    try:
+        async with client.delete(url, **kwargs) as rsp:
+            log.info(f"http_delete status: {rsp.status}")
+            if rsp.status == 200:
+                pass  # expected
+            elif rsp.status == 404:
+                log.info(f"NotFound response for DELETE for url: {url}")
+            elif rsp.status == 503:
+                log.warn(f"503 error for http_delete {url}")
+                raise HTTPServiceUnavailable()
+            else:
+                msg = f"DELETE request error for url: {url} "
+                msg += f"status: {rsp.status}"
+                log.error(msg)
+                raise HTTPInternalServerError()
+
+            # rsp_json = await rsp.json()
+            # log.debug(f"http_delete({url}) response: {rsp_json}")
+    except ClientError as ce:
+        log.warn(f"ClientError for http_delete({url}): {ce} ")
+        raise HTTPInternalServerError()
+    except CancelledError as cle:
+        log.warn(f"CancelledError for http_delete({url}): {cle}")
+        raise HTTPInternalServerError()
+    except ConnectionResetError as cre:
+        log.warn(f"ConnectionResetError for http_delete({url}): {cre}")
+        raise HTTPInternalServerError()
 
-    app = request.app
-    params = request.rel_url.query
+    return rsp_json
 
-    chunk_id = request.match_info.get('id')
-    if not chunk_id:
-        msg = "Missing chunk id"
-        log.error(msg)
-        raise HTTPBadRequest(reason=msg)
-    if not isValidUuid(chunk_id, "Chunk"):
-        msg = f"Invalid chunk id: {chunk_id}"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
+
+async def jsonResponse(resp, data, status=200, ignore_nan=False, body_only=False):
+    """
+    Helper function, create a response object using the provided
+    JSON data
+    """
+    # tbd - remove resp parameter - not used
 
     try:
-        validateInPartition(app, chunk_id)
-    except KeyError:
-        msg = f"invalid partition for obj id: {chunk_id}"
-        log.error(msg)
-        raise HTTPInternalServerError()
-    log.debug(f"request params: {params.keys()}")
-
-    if "s3path" in params:
-        s3path = params["s3path"]
-        log.debug(f"GET_Chunk - using URI: {s3path}")
-    if "bucket" in params:
-        bucket = params["bucket"]
-    if not bucket:
-        msg = "GET_Chunk - bucket is None"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
-
-    log.debug(f"GET_Chunk - using bucket: {bucket}")
-        
-    if "s3offset" in params:
-        try:
-            s3offset = int(params["s3offset"])
-        except ValueError:
-            log.error(f"invalid s3offset params: {params['s3offset']}")
-            raise HTTPBadRequest()
-    if "s3size" in params:
-        try:
-            s3size = int(params["s3size"])
-        except ValueError:
-            log.error(f"invalid s3size params: {params['s3sieze']}")
-            raise HTTPBadRequest()
-
-    if "query" in params:
-        query = params["query"]
-        log.debug(f"got query: {query}")
-    if "Limit" in params:
-        limit = int(params["Limit"])
-
-    dset_id = getDatasetId(chunk_id)
-
-    dset_json = await get_metadata_obj(app, dset_id, bucket=bucket)
-    dims = getChunkLayout(dset_json)
-    log.debug(f"GET_Chunk - got dims: {dims}")
-
-    # get chunk selection from query params
-    if "select" in params:
-        select = params["select"]
-    else:
-        select = None # get slices for entire datashape
-    log.debug(f"using select string: {select}")
-    try:
-        selection = getSelectionList(select, dims)
+        text = simplejson.dumps(data, ignore_nan=ignore_nan, allow_nan=True)
     except ValueError as ve:
-        log.error(f"ValueError for select: {select}: {ve}")
+        # this exception started to get raised around 04/12/2023
+        # "out of range float values" when nan is eturned and ignore_nan is False
+        # some change in numpy behaviour?
+        log.warn(f"got exception {ve} trying to do json dump of: {data}")
         raise HTTPInternalServerError()
-    log.debug(f"GET_Chunk - got selection: {selection}")
+    if body_only:
+        return text
+    else:
+        server_name = config.get("server_name")
+        xss_protection = config.get("xss_protection", default="1; mode=block")
+        headers = {"Server": server_name}
+        if xss_protection:
+            headers["X-XSS-Protection"] = xss_protection
+        return json_response(text=text, headers=headers, status=status)
 
-    kwargs = {"chunk_init": False}
-    if s3path:
-        kwargs["s3path"] = s3path
-        kwargs["s3offset"] = s3offset
-        kwargs["s3size"] = s3size   
-    else:
-        kwargs["bucket"] = bucket 
-    chunk_arr = await get_chunk(app, chunk_id, dset_json, **kwargs)
-    if chunk_arr is None:
-        msg = f"chunk {chunk_id} not found"
-        log.warn(msg)
-        raise HTTPNotFound()
-
-    if query:
-        # run given query
-        try:
-            kwargs = {"chunk_id": chunk_id,
-                      "chunk_layout": dims,
-                      "chunk_arr": chunk_arr,
-                      "slices": selection,
-                      "query": query,
-                      "limit": limit,
-                      "return_json": True}
-            read_resp = chunkQuery(**kwargs)
-        except TypeError as te:
-            log.warn(f"chunkQuery - TypeError: {te}")
-            raise HTTPBadRequest()
-        except ValueError as ve:
-            log.warn(f"chunkQuery - ValueError: {ve}")
-            raise HTTPBadRequest()
-    else:
-        # read selected data from chunk
-        output_arr = chunkReadSelection(chunk_arr, slices=selection)
-        read_resp = arrayToBytes(output_arr)
-
-    # write response
-    if isinstance(read_resp, bytes):
-
-        try:
-            resp = StreamResponse()
-            resp.headers['Content-Type'] = "application/octet-stream"
-            resp.content_length = len(read_resp)
-            await resp.prepare(request)
-            await resp.write(read_resp)
-        except Exception as e:
-            log.error(f"Exception during binary data write: {e}")
-            raise HTTPInternalServerError()
-        finally:
-            await resp.write_eof()
-    else:
-        # JSON response
-        resp = json_response(read_resp)
-
-    return resp
 
+def respJsonAssemble(obj_json, params, id):
+    """
+    Populate response fields based on object type
+    """
+    log.debug("enter assemble")
 
-async def POST_Chunk(request):
+    if isValidUuid(id, "dataset"):
+        log.debug("assemble dataset")
+        resp_json = {}
+        resp_json["id"] = obj_json["id"]
+        resp_json["root"] = obj_json["root"]
+        resp_json["shape"] = obj_json["shape"]
+        resp_json["type"] = obj_json["type"]
+        if "creationProperties" in obj_json:
+            if "ignore_nan" in params and params["ignore_nan"]:
+                # convert fillValue to "nan" if it is a np.nan
+                s = obj_json["creationProperties"]
+                d = {}
+                for k in s:
+                    v = s[k]
+                    if k == "fillValue" and isinstance(v, float) and np.isnan(v):
+                        d[k] = "nan"
+                    else:
+                        d[k] = v
+                resp_json["creationProperties"] = d
+            else:
+                # just return the dset_json creation props as is
+                resp_json["creationProperties"] = obj_json["creationProperties"]
+        else:
+            resp_json["creationProperties"] = {}
+
+        if "layout" in obj_json:
+            resp_json["layout"] = obj_json["layout"]
+        resp_json["attributeCount"] = obj_json["attributeCount"]
+        resp_json["created"] = obj_json["created"]
+        resp_json["lastModified"] = obj_json["lastModified"]
+        if "include_attrs" in params and params["include_attrs"]:
+            resp_json["attributes"] = obj_json["attributes"]
+        return resp_json
+    elif isValidUuid(id, "group"):
+        log.debug("assemble group")
+        return obj_json
+    elif isValidUuid(id, "type"):
+        log.debug("assemble type")
+        return obj_json
+    elif isValidUuid(id, "chunk"):
+        log.debug("assemble chunk")
+        return obj_json
+    else:
+        return obj_json
+
+
+def getHeader(uri):
     """
-    Return data from requested chunk and point selection
+    Determine domain header based on id
     """
-    log.request(request)
-    app = request.app
-    params = request.rel_url.query
+    if isValidUuid(uri, "group"):
+        return "/groups/"
+    elif isValidUuid(uri, "dataset"):
+        return "/datasets/"
+    elif isValidUuid(uri, "type"):
+        return "/datatypes/"
+    else:
+        log.error("Couldn't determine proper header for type")
+        raise HTTPInternalServerError()
 
-    put_points = False
-    num_points = 0
-    if "count" not in params:
-        log.warn("expected count param")
-        raise HTTPBadRequest()
-    if "count" in params:
-        num_points = int(params["count"])
-
-    if "action" in params and params["action"] == "put":
-        log.info(f"POST Chunk put points - num_points: {num_points}")
-        put_points = True
-    else:
-        log.info(f"POST Chunk get points - num_points: {num_points}")
-
-    if "bucket" not in params:
-        msg = "POST_Chunk - expected bucket param"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
-
-    bucket = params["bucket"]
-
-    s3path = None
-    s3offset = 0
-    s3size = 0
-    if "s3path" in params:
-        if put_points:
-            log.error("s3path can not be used with put points POST request")
-            raise HTTPBadRequest()
-        s3path = params["s3path"]
-        log.debug(f"POST_Chunk - using s3path: {s3path}")
-     
-    if "s3offset" in params:
-        try:
-            s3offset = int(params["s3offset"])
-        except ValueError:
-            log.error(f"invalid s3offset params: {params['s3offset']}")
-            raise HTTPBadRequest()
-    if "s3size" in params:
-        try:
-            s3size = int(params["s3size"])
-        except ValueError:
-            log.error(f"invalid s3size params: {params['s3size']}")
-            raise HTTPBadRequest()
-
-    chunk_id = request.match_info.get('id')
-    if not chunk_id:
-        msg = "Missing chunk id"
-        log.error(msg)
-        raise HTTPBadRequest(reason=msg)
-    log.info(f"POST chunk_id: {chunk_id}")
-    chunk_index = getChunkIndex(chunk_id)
-    log.debug(f"chunk_index: {chunk_index}")
-
-    if not isValidUuid(chunk_id, "Chunk"):
-        msg = f"Invalid chunk id: {chunk_id}"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
 
-    try:
-        validateInPartition(app, chunk_id)
-    except KeyError:
-        msg = f"invalid partition for obj id: {chunk_id}"
-        log.error(msg)
-        raise HTTPInternalServerError()
-
-    log.debug(f"request params: {list(params.keys())}")
-    if "dset" in params:
-        msg = "Unexpected dset in POST request"
-        log.error(msg)
-        raise HTTPBadRequest(reason=msg)
-
-    if not request.has_body:
-        msg = "POST Value with no body"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
+def getObjectClass(uri):
+    """
+    Determine object based on id
+    """
+    if isValidUuid(uri, "group"):
+        return "group"
+    elif isValidUuid(uri, "dataset"):
+        return "dataset"
+    elif isValidUuid(uri, "type"):
+        return "datatype"
+    else:
+        log.error("Couldn't determine proper object class for id")
+        raise HTTPInternalServerError()
 
-    content_type = "application/octet-stream"
-    if "Content-Type" in request.headers:
-        # client should use "application/octet-stream" for binary transfer
-        content_type = request.headers["Content-Type"]
-    if content_type != "application/octet-stream":
-        msg = f"Unexpected content_type: {content_type}"
-        log.error(msg)
-        raise HTTPBadRequest(reason=msg)
-
-    dset_id = getDatasetId(chunk_id)
-
-    dset_json = await get_metadata_obj(app, dset_id, bucket=bucket)
-    dims = getChunkLayout(dset_json)
-    rank = len(dims)
-
-    type_json = dset_json["type"]
-    dset_dtype = createDataType(type_json)
-
-    # create a numpy array for incoming points
-    input_bytes = await request_read(request)
-    actual = request.content_length
-    if len(input_bytes) != actual:
-        msg = f"Read {len(input_bytes)} bytes, expecting: {actual}"
-        log.error(msg)
-        raise HTTPInternalServerError()
-
-    if rank == 1:
-        coord_type_str = "uint64"
-    else:
-        coord_type_str = f"({rank},)uint64"
-
-    if put_points:
-        # create a numpy array with the following type:
-        #       (coord1, coord2, ...) | dset_dtype
-        type_fields = [("coord", np.dtype(coord_type_str)),
-                       ("value", dset_dtype)]
-        point_dt = np.dtype(type_fields)
-        point_shape = (num_points,)
-        chunk_init = True
-    else:
-        point_dt = np.dtype('uint64')
-        point_shape = (num_points, rank)
-        chunk_init = False
-
-    point_arr = bytesToArray(input_bytes, point_dt, point_shape)
-
-    kwargs = {"chunk_init": chunk_init}
-    if s3path:
-        kwargs["s3path"] = s3path
-        kwargs["s3offset"] = s3offset
-        kwargs["s3size"] = s3size
-    else:
-        kwargs["bucket"] = bucket
-              
-    chunk_arr = await get_chunk(app, chunk_id, dset_json, **kwargs)
-    if chunk_arr is None:
-        log.warn(f"chunk {chunk_id} not found")
-        raise HTTPNotFound()
-
-    if put_points:
-        # writing point data
-        try:
-            kwargs = {"chunk_id": chunk_id,
-                      "chunk_layout": dims,
-                      "chunk_arr": chunk_arr,
-                      "point_arr": point_arr}
-            chunkWritePoints(**kwargs)
-        except ValueError as ve:
-            log.warn(f"got value error from chunkWritePoints: {ve}")
-            raise HTTPBadRequest()
-        # write empty response
-        resp = json_response({})
-        # lazily write chunk to storage
-        save_chunk(app, chunk_id, dset_json, bucket=bucket)
-    else:
-        # read points
-        try:
-            kwargs = {"chunk_id": chunk_id,
-                      "chunk_layout": dims,
-                      "chunk_arr": chunk_arr,
-                      "point_arr": point_arr}
-            output_arr = chunkReadPoints(**kwargs)
-        except ValueError as ve:
-            log.warn(f"got value error from chunkReadPoints: {ve}")
-            raise HTTPBadRequest()
-        output_data = arrayToBytes(output_arr)
-        # write response
-        try:
-            resp = StreamResponse()
-            resp.headers['Content-Type'] = "application/octet-stream"
-            resp.content_length = len(output_data)
-            await resp.prepare(request)
-            await resp.write(output_data)
-        except Exception as e:
-            log.error(f"Exception during binary data write: {e}")
-            raise HTTPInternalServerError()
-        finally:
-            await resp.write_eof()
-
-    return resp
-
-
-async def DELETE_Chunk(request):
-    """HTTP DELETE method for /chunks/
-    Note: clients (i.e. SN nodes) don't directly delete chunks.
-       This method should only be called by the AN node.
+
+def getHref(request, uri, query=None, domain=None):
+    """
+    Convenience method to compute href links
     """
-    log.request(request)
-    app = request.app
     params = request.rel_url.query
-    chunk_id = request.match_info.get('id')
-    if not chunk_id:
-        msg = "Missing chunk id"
-        log.error(msg)
-        raise HTTPBadRequest(reason=msg)
-    log.info(f"DELETE chunk: {chunk_id}")
-
-    if not isValidUuid(chunk_id, "Chunk"):
-        msg = f"Invalid chunk id: {chunk_id}"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
-    if "bucket" in params:
-        bucket = params["bucket"]
-    
-    if not bucket:
-        msg = "DELETE_Chunk - bucket param not set"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
+    href = config.get("hsds_endpoint")
+    if not href:
+        href = request.scheme + "://127.0.0.1"
+    href += uri
+    delimiter = "?"
+    if domain:
+        href += "?domain=" + domain
+        delimiter = "&"
+    elif "domain" in params:
+        href += "?domain=" + params["domain"]
+        delimiter = "&"
+    elif "host" in params:
+        href += "?host=" + params["host"]
+        delimiter = "&"
+
+    if query is not None:
+        if type(query) is str:
+            href += delimiter + query
+        else:
+            # list or tuple
+            for item in query:
+                href += delimiter + item
+                delimiter = "&"
+    return href
 
 
-    try:
-        validateInPartition(app, chunk_id)
-    except KeyError:
-        msg = f"invalid partition for obj id: {chunk_id}"
-        log.error(msg)
-        raise HTTPInternalServerError()
-
-    chunk_cache = app['chunk_cache']
-    s3key = getS3Key(chunk_id)
-    log.debug(f"DELETE_Chunk s3_key: {s3key}")
-
-    if chunk_id in chunk_cache:
-        del chunk_cache[chunk_id]
-
-    filter_map = app["filter_map"]
-    dset_id = getDatasetId(chunk_id)
-    if dset_id in filter_map:
-        # The only reason chunks are ever deleted is if the dataset is being
-        # deleted, so it should be safe to remove this entry now
-        log.info(f"Removing filter_map entry for {dset_id}")
-        del filter_map[dset_id]
+def getAcceptType(request):
+    """
+    Get requested content type.  Returns either "binary" if the accept
+    header is octet stream, otherwise json.
+    Currently does not support q fields.
+    """
+    accept_type = "json"  # default to JSON
+    if "accept" in request.headers:
+        accept = request.headers["accept"]
+        # treat everything as json unless octet-stream is given
+        if accept != "application/octet-stream":
+            msg = f"Ignoring accept value: {accept}"
+            log.debug(msg)
+        else:
+            accept_type = "binary"
+    return accept_type
+
+
+def isAWSLambda(request):
+    """
+    Return true if this is a lambda request
+    """
+    is_lambda = False
+    if "User-Agent" in request.headers:
+        if request.headers["User-Agent"] == "AWSLambda":
+            is_lambda = True
+    return is_lambda
+
 
-    if await isStorObj(app, s3key, bucket=bucket):
-        await deleteStorObj(app, s3key, bucket=bucket)
+def getContentType(request):
+    """
+    Get the content type from request headers.
+    Default to json if not specified
+    """
+    if "Content-Type" in request.headers:
+        # client should use "application/octet-stream" for binary transfer
+        content_type = request.headers["Content-Type"]
+        if content_type == "application/octet-stream":
+            request_type = "binary"
+        elif content_type == "application/json":
+            request_type = "json"
+        else:
+            msg = f"Unknown content_type: {content_type}"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
     else:
-        msg = f"delete_metadata_obj - key {s3key} not found (never written)?"
-        log.info(msg)
+        request_type = "json"
+    return request_type
+
 
-    resp_json = {}
-    resp = json_response(resp_json)
-    log.response(request, resp=resp)
-    return resp
+def isBinaryResponse(rsp):
+    """
+    Return True if response is binary data
+    """
+    is_binary = False
+    if "Content-Type" in rsp.headers:
+        content_type = rsp.headers["Content-Type"]
+        if content_type == "application/octet-stream":
+            is_binary = True
+    return is_binary
```

### Comparing `hsds-0.7.0b11/hsds/chunk_sn.py` & `hsds-0.8.0/hsds/chunk_sn.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,936 +7,419 @@
 # terms governing use, modification, and redistribution, is contained in     #
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # value operations
-# handles dataset /value requests
+# handles dataset /value requests for service node
 #
-import asyncio
-from multiprocessing import shared_memory
-from asyncio import CancelledError
+
 import base64
+import math
 import numpy as np
-from aiohttp.web_exceptions import HTTPBadRequest, HTTPNotFound
+from json import JSONDecodeError
+from asyncio import IncompleteReadError
+from aiohttp.web_exceptions import HTTPException, HTTPBadRequest
 from aiohttp.web_exceptions import HTTPRequestEntityTooLarge
 from aiohttp.web_exceptions import HTTPConflict, HTTPInternalServerError
-from aiohttp.web_exceptions import HTTPServiceUnavailable
-from aiohttp.client_exceptions import ClientError
 from aiohttp.web import StreamResponse
 
-from .util.httpUtil import getHref, getAcceptType, http_get, http_put
-from .util.httpUtil import http_post, request_read, jsonResponse
-from .util.idUtil import isValidUuid, getDataNodeUrl, getNodeCount
+from .util.httpUtil import getHref, getAcceptType, getContentType, http_put
+from .util.httpUtil import request_read, jsonResponse, isAWSLambda
+from .util.idUtil import isValidUuid, getDataNodeUrl
 from .util.domainUtil import getDomainFromRequest, isValidDomain
 from .util.domainUtil import getBucketForDomain
 from .util.hdf5dtype import getItemSize, createDataType
-from .util.dsetUtil import getSelectionList, setSliceQueryParam  
-from .util.dsetUtil import getFillValue, isExtensible
+from .util.dsetUtil import getSelectionList, isNullSpace, getDatasetLayoutClass
+from .util.dsetUtil import getFillValue, isExtensible, getSelectionPagination
 from .util.dsetUtil import getSelectionShape, getDsetMaxDims, getChunkLayout
+from .util.dsetUtil import getDatasetCreationPropertyLayout
 from .util.chunkUtil import getNumChunks, getChunkIds, getChunkId
 from .util.chunkUtil import getChunkIndex, getChunkSuffix
 from .util.chunkUtil import getChunkCoverage, getDataCoverage
-from .util.chunkUtil import getChunkIdForPartition
+from .util.chunkUtil import getQueryDtype, get_chunktable_dims
 from .util.arrayUtil import bytesArrayToList, jsonToArray, getShapeDims
 from .util.arrayUtil import getNumElements, arrayToBytes, bytesToArray
 from .util.arrayUtil import squeezeArray
 from .util.authUtil import getUserPasswordFromRequest, validateUserPassword
+from .util.boolparser import BooleanParser
 from .servicenode_lib import getObjectJson, validateAction
+from .chunk_crawl import ChunkCrawler
 from . import config
 from . import hsds_logger as log
 
-CHUNK_REF_LAYOUTS = ('H5D_CONTIGUOUS_REF',
-                     'H5D_CHUNKED_REF',
-                     'H5D_CHUNKED_REF_INDIRECT')
+CHUNK_REF_LAYOUTS = (
+    "H5D_CONTIGUOUS_REF",
+    "H5D_CHUNKED_REF",
+    "H5D_CHUNKED_REF_INDIRECT",
+)
 
-EXPECTED_CONTENT_TYPES = ("application/json", "application/octet-stream")
+VARIABLE_AVG_ITEM_SIZE = 512  # guess at avg variable type length
 
 
-def _isNonStrict(params):
-    """
-    Check nonstrict parameter.
+def get_hrefs(request, dset_json):
     """
-    retval = False
-    if "nonstrict" in params:
-        v = params["nonstrict"]
-        if isinstance(v, str):
-            if v.startswith("T") or v.startswith("t"):
-                retval = True   # True, true, T, t
-            else:
-                try:
-                    n = int(v)
-                    if n != 0:
-                        retval = True
-                except ValueError:
-                    log.warn(f"unexpected nonstrict param value: {v}")
-        else:
-            if v:
-                retval = True
-    return retval
-
-
-async def write_chunk_hyperslab(app, chunk_id, dset_json, slices, arr,
-                                bucket=None):
-    """ write the chunk selection to the DN
-    chunk_id: id of chunk to write to
-    chunk_sel: chunk-relative selection to write to
-    np_arr: numpy array of data to be written
+    Convience function to set up hrefs for GET
     """
-
-    if not bucket:
-        bucket = config.get("bucket_name")
-
-    msg = f"write_chunk_hyperslab, chunk_id:{chunk_id}, slices:{slices}, "
-    msg += f"bucket: {bucket}"
-    log.info(msg)
-    if "layout" not in dset_json:
-        log.error(f"No layout found in dset_json: {dset_json}")
-        raise HTTPInternalServerError()
-    partition_chunk_id = getChunkIdForPartition(chunk_id, dset_json)
-    if partition_chunk_id != chunk_id:
-        log.debug(f"using partition_chunk_id: {partition_chunk_id}")
-        chunk_id = partition_chunk_id  # replace the chunk_id
-
-    if "type" not in dset_json:
-        log.error(f"No type found in dset_json: {dset_json}")
-        raise HTTPInternalServerError()
-
-    layout = getChunkLayout(dset_json)
-    chunk_sel = getChunkCoverage(chunk_id, slices, layout)
-    log.debug(f"chunk_sel: {chunk_sel}")
-    data_sel = getDataCoverage(chunk_id, slices, layout)
-    log.debug(f"data_sel: {data_sel}")
-    log.debug(f"arr.shape: {arr.shape}")
-    arr_chunk = arr[data_sel]
-    req = getDataNodeUrl(app, chunk_id)
-    req += "/chunks/" + chunk_id
-
-    log.debug(f"PUT chunk req: {req}")
-    data = arrayToBytes(arr_chunk)
-    # pass itemsize, type, dimensions, and selection as query params
-    params = {}
-    setSliceQueryParam(params, chunk_sel)
-    if bucket:
-        params["bucket"] = bucket
-
-    try:
-        json_rsp = await http_put(app, req, data=data, params=params)
-        msg = f"got rsp: {json_rsp} for put binary request: {req}, "
-        msg += f"{len(data)} bytes"
-        log.debug(msg)
-    except ClientError as ce:
-        log.error(f"Error for http_put({req}): {ce} ")
-        raise HTTPInternalServerError()
-    except CancelledError as cle:
-        log.warn(f"CancelledError for http_put({req}): {cle}")
+    hrefs = []
+    dset_id = dset_json["id"]
+    dset_uri = f"/datasets/{dset_id}"
+    self_uri = f"{dset_uri}/value"
+    hrefs.append({"rel": "self", "href": getHref(request, self_uri)})
+    root_uri = "/groups/" + dset_json["root"]
+    hrefs.append({"rel": "root", "href": getHref(request, root_uri)})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
+    hrefs.append({"rel": "owner", "href": getHref(request, dset_uri)})
+    return hrefs
 
 
-async def read_chunk_hyperslab(app, chunk_id, dset_json, slices, np_arr,
-                               chunk_map=None, bucket=None):
-    """ read the chunk selection from the DN
-    chunk_id: id of chunk to write to
-    chunk_sel: chunk-relative selection to read from
-    np_arr: numpy array to store read bytes
-    chunk_map: map of chunk_id to chunk_offset and chunk_size
-        chunk_offset: location of chunk with the s3 object
-        chunk_size: size of chunk within the s3 object (or 0 if the
-           entire object)
-    bucket: s3 bucket to read from
+async def get_slices(app, select, dset_json, bucket=None):
+    """Get desired slices from selection query param string or json value.
+    If select is none or empty, slices for entire datashape will be
+    returned.
+    Refretch dims if the dataset is extensible
     """
-    if not bucket:
-        bucket = config.get("bucket_name")
-
-    msg = f"read_chunk_hyperslab, chunk_id: {chunk_id}, slices: {slices}, "
-    msg += f"bucket: {bucket}"
-    log.info(msg)
-    if chunk_map and chunk_id not in chunk_map:
-        log.warn(f"expected to find {chunk_id} in chunk_map")
 
-    partition_chunk_id = getChunkIdForPartition(chunk_id, dset_json)
-    if partition_chunk_id != chunk_id:
-        log.debug(f"using partition_chunk_id: {partition_chunk_id}")
-        chunk_id = partition_chunk_id  # replace the chunk_id
-
-    if "type" not in dset_json:
-        log.error(f"No type found in dset_json: {dset_json}")
-        raise HTTPInternalServerError()
-
-    layout = getChunkLayout(dset_json)
+    dset_id = dset_json["id"]
+    datashape = dset_json["shape"]
+    if datashape["class"] == "H5S_NULL":
+        msg = "Null space datasets can not be used as target for GET value"
+        log.warn(msg)
+        raise HTTPBadRequest(reason=msg)
 
-    chunk_sel = getChunkCoverage(chunk_id, slices, layout)
-    log.debug(f"read_chunk_hyperslab - chunk_sel: {chunk_sel}")
-    data_sel = getDataCoverage(chunk_id, slices, layout)
-    log.debug(f"read_chunk_hyperslab - data_sel: {data_sel}")
-
-    # pass dset json and selection as query params
-    params = {}
-
-    fill_value = getFillValue(dset_json)
-
-    chunk_shape = getSelectionShape(chunk_sel)
-    log.debug(f"chunk_shape: {chunk_shape}")
-    dt = np_arr.dtype
-
-    def defaultChunk():
-        # no data, return zero array
-        if fill_value:
-            chunk_arr = np.empty(chunk_shape, dtype=dt, order='C')
-            chunk_arr[...] = fill_value
-        else:
-            chunk_arr = np.zeros(chunk_shape, dtype=dt, order='C')
-        return chunk_arr
+    dims = getShapeDims(datashape)  # throws 400 for HS_NULL dsets
+    maxdims = getDsetMaxDims(dset_json)
 
-    chunk_arr = None
-    array_data = None
-    setSliceQueryParam(params, chunk_sel)
-    if chunk_map:
-        if chunk_id not in chunk_map:
-            msg = f"{chunk_id} not found in chunk_map, returning default arr"
-            log.debug(msg)
-            chunk_arr = defaultChunk()
-        else:
-            chunk_info = chunk_map[chunk_id]
-            params["s3path"] = chunk_info["s3path"]
-            params["s3offset"] = chunk_info["s3offset"]
-            params["s3size"] = chunk_info["s3size"]
-            log.debug(f"using chunk_map entry for {chunk_id}: {chunk_info}")
-    
-    # bucket will be used to get dset json even when s3path is used for 
-    # the chunk data
-    params["bucket"] = bucket
-
-    if chunk_arr is None:
-
-        req = getDataNodeUrl(app, chunk_id)
-        req += "/chunks/" + chunk_id
-        log.debug("GET chunk req: " + req)
-        try:
-            array_data = await http_get(app, req, params=params)
-            log.debug(f"http_get {req}, read {len(array_data)} bytes")
-        except HTTPNotFound:
-            if "s3path" in params:
-                s3path = params["s3path"]
-                # external HDF5 file, should exist
-                log.warn(f"s3path: {s3path} for S3 range get not found")
-                raise
-            # no data, return zero array
-            chunk_arr = defaultChunk()
-        except ClientError as ce:
-            log.error(f"Error for http_get({req}): {ce} ")
-            raise HTTPInternalServerError()
-        except CancelledError as cle:
-            log.warn(f"CancelledError for http_get({req}): {cle}")
-            return
+    # refetch the dims if the dataset is extensible and request or hasn't
+    # provided an explicit region
+    if isExtensible(dims, maxdims) and (select is None or not select):
+        kwargs = {"bucket": bucket, "refresh": True}
+        dset_json = await getObjectJson(app, dset_id, **kwargs)
+        dims = getShapeDims(dset_json["shape"])
 
-    if array_data is None:
-        log.debug(f"No data returned for chunk: {chunk_id}")
-    else:
-        log.debug(f"got data for chunk: {chunk_id}")
-        # convert binary data to numpy array
+    slices = None  # selection for read
+    if isExtensible and select:
         try:
-            chunk_arr = bytesToArray(array_data, dt, chunk_shape)
-        except ValueError as ve:
-            log.warn(f"bytesToArray ValueError: {ve}")
-            raise HTTPBadRequest()
-        nelements_read = getNumElements(chunk_arr.shape)
-        nelements_expected = getNumElements(chunk_shape)
-        if nelements_read != nelements_expected:
-            msg = f"Expected {nelements_expected} points, "
-            msg += f"but got: {nelements_read}"
-            log.error(msg)
-            raise HTTPInternalServerError()
-        chunk_arr = chunk_arr.reshape(chunk_shape)
-
-    log.info(f"chunk_arr shape: {chunk_arr.shape}")
-    log.info(f"data_sel: {data_sel}")
-    log.info(f"np_arr shape: {np_arr.shape}")
-
-    np_arr[data_sel] = chunk_arr
-
-
-async def read_point_sel(app, chunk_id, dset_json, point_list, point_index,
-                         np_arr, chunk_map=None, bucket=None):
-    """
-    Read point selection
-    --
-    app: application object
-    chunk_id: id of chunk to read from
-    dset_json: dset JSON
-    point_list: array of points to read
-    point_index: index of arr element to update for a given point
-    arr: numpy array to store read bytes
-    """
-
-    if not bucket:
-        bucket = config.get("bucket_name")
-
-    msg = f"read_point_sel, chunk_id: {chunk_id}, bucket: {bucket}"
-    log.info(msg)
-
-    partition_chunk_id = getChunkIdForPartition(chunk_id, dset_json)
-    if partition_chunk_id != chunk_id:
-        log.debug(f"using partition_chunk_id: {partition_chunk_id}")
-        chunk_id = partition_chunk_id  # replace the chunk_id
-
-    point_dt = np.dtype('u8')  # use unsigned long for point index
-
-    if "type" not in dset_json:
-        log.error(f"No type found in dset_json: {dset_json}")
-        raise HTTPInternalServerError()
-
-    num_points = len(point_list)
-    log.debug(f"read_point_sel: {num_points}")
-    np_arr_points = np.asarray(point_list, dtype=point_dt)
-    post_data = np_arr_points.tobytes()
-
-    # set action as query params
-    params = {}
-    params["action"] = "get"
-    params["count"] = num_points
-
-    fill_value = getFillValue(dset_json)
-
-    np_arr_rsp = None
-    dt = np_arr.dtype
-
-    def defaultArray():
-        # no data, return zero array
-        if fill_value:
-            arr = np.empty((num_points,), dtype=dt)
-            arr[...] = fill_value
-        else:
-            arr = np.zeros((num_points,), dtype=dt)
-        return arr
+            slices = getSelectionList(select, dims)
+        except ValueError:
+            # exception might be due to us having stale version of dims,
+            # so use refresh
+            kwargs = {"bucket": bucket, "refresh": True}
+            dset_json = await getObjectJson(app, dset_id, **kwargs)
+            dims = getShapeDims(dset_json["shape"])
+            slices = None  # retry below
 
-    np_arr_rsp = None
-    if chunk_map:
-        if chunk_id not in chunk_map:
-            msg = f"{chunk_id} not found in chunk_map, returning default arr"
-            log.debug(msg)
-            np_arr_rsp = defaultArray()
-        else:
-            chunk_info = chunk_map[chunk_id]
-            params["s3path"] = chunk_info["s3path"]
-            params["s3offset"] = chunk_info["s3offset"]
-            params["s3size"] = chunk_info["s3size"]
-   
-    # bucket will be used to get dset json even when s3path is used for 
-    # the chunk data
-    params["bucket"] = bucket
-
-    if np_arr_rsp is None:
-
-        # make request to DN node
-        req = getDataNodeUrl(app, chunk_id)
-        req += "/chunks/" + chunk_id
-        log.debug(f"GET chunk req: {req}")
+    if slices is None:
         try:
-            kwargs = {"params": params, "data": post_data}
-            rsp_data = await http_post(app, req, **kwargs)
-            msg = f"got rsp for http_post({req}): {len(rsp_data)} bytes"
-            log.debug(msg)
-            np_arr_rsp = bytesToArray(rsp_data, dt, (num_points,))
-        except HTTPNotFound:
-            if "s3path" in params:
-                s3path = params["s3path"]
-                # external HDF5 file, should exist
-                log.warn(f"s3path: {s3path} for S3 range get found")
-                raise
-            # no data, return zero array
-            np_arr_rsp = defaultArray()
-
-    npoints_read = len(np_arr_rsp)
-    log.info(f"got {npoints_read} points response")
-    log.debug(f"np_arr {np_arr}")
-    log.debug(f"np_arr_rsp: {np_arr_rsp}")
+            slices = getSelectionList(select, dims)
+        except ValueError:
+            msg = f"Invalid selection: {select} on dims: {dims} "
+            msg += f"for dataset: {dset_id}"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
+    return slices
 
-    if npoints_read != num_points:
-        msg = f"Expected {num_points} points, but got: {npoints_read}"
-        log.error(msg)
-        raise HTTPInternalServerError()
 
-    # Fill in the return array based on passed in index values
-    for i in range(num_points):
-        index = point_index[i]
-        np_arr[index] = np_arr_rsp[i]
+def use_http_streaming(request, rank):
+    """ return boolean indicating whether http streaming should be used """
+    if rank == 0:
+        return False
+    if isAWSLambda(request):
+        return False
+    if not config.get("http_streaming", default=True):
+        return False
+    return True
 
 
-async def write_point_sel(app, chunk_id, dset_json, point_list, point_data,
-                          bucket=None):
-    """
-    Write point selection
-    --
-      app: application object
-      chunk_id: id of chunk to write to
-      dset_json: dset JSON
-      point_list: array of points to write
-      point_data: index of arr element to update for a given point
+async def getChunkLocations(app, dset_id, dset_json, chunkinfo_map, chunk_ids, bucket=None):
     """
-
-    if not bucket:
-        bucket = config.get("bucket_name")
-
-    msg = f"write_point_sel, chunk_id: {chunk_id}, points: {point_list}, "
-    msg += f"data: {point_data}"
-    log.info(msg)
-    if "type" not in dset_json:
-        log.error(f"No type found in dset_json: {dset_json}")
-        raise HTTPInternalServerError()
-
-    datashape = dset_json["shape"]
-    dims = getShapeDims(datashape)
-    rank = len(dims)
-    type_json = dset_json["type"]
-    dset_dtype = createDataType(type_json)  # np datatype
-
-    partition_chunk_id = getChunkIdForPartition(chunk_id, dset_json)
-    if partition_chunk_id != chunk_id:
-        log.debug(f"using partition_chunk_id: {partition_chunk_id}")
-        chunk_id = partition_chunk_id  # replace the chunk_id
-
-    req = getDataNodeUrl(app, chunk_id)
-    req += "/chunks/" + chunk_id
-    log.debug("POST chunk req: " + req)
-
-    num_points = len(point_list)
-    log.debug(f"write_point_sel - {num_points}")
-
-    # create a numpy array with point_data
-    data_arr = jsonToArray((num_points,), dset_dtype, point_data)
-
-    # create a numpy array with the following type:
-    #   (coord1, coord2, ...) | dset_dtype
-    if rank == 1:
-        coord_type_str = "uint64"
-    else:
-        coord_type_str = f"({rank},)uint64"
-    type_fields = [("coord", np.dtype(coord_type_str)), ("value", dset_dtype)]
-    comp_type = np.dtype(type_fields)
-    np_arr = np.zeros((num_points, ), dtype=comp_type)
-
-    # Zip together coordinate and point_data to one numpy array
-    for i in range(num_points):
-        if rank == 1:
-            elem = (point_list[i], data_arr[i])
-        else:
-            elem = (tuple(point_list[i]), data_arr[i])
-        np_arr[i] = elem
-
-    # TBD - support VLEN data
-    post_data = np_arr.tobytes()
-
-    # pass dset_json as query params
-    params = {}
-    params["action"] = "put"
-    params["count"] = num_points
-    params["bucket"] = bucket
-
-    json_rsp = await http_post(app, req, params=params, data=post_data)
-    log.debug(f"post to {req} returned {json_rsp}")
-
-
-async def read_chunk_query(app, chunk_id, dset_json, slices, query, limit,
-                           rsp_dict, chunk_map=None, bucket=None):
-    """ read the chunk selection from the DN
-    chunk_id: id of chunk to write to
-    chunk_sel: chunk-relative selection to read from
-    np_arr: numpy array to store read bytes
+    Get info for chunk locations (for reference layouts)
     """
-    msg = f"read_chunk_query, chunk_id: {chunk_id}, slices: {slices}, "
-    msg += f"query: {query}"
-    log.info(msg)
-    chunk_rsp = None
-
-    partition_chunk_id = getChunkIdForPartition(chunk_id, dset_json)
-    if partition_chunk_id != chunk_id:
-        log.debug(f"using partition_chunk_id: {partition_chunk_id}")
-        chunk_id = partition_chunk_id  # replace the chunk_id
+    layout_class = getDatasetLayoutClass(dset_json)
 
-    layout = getChunkLayout(dset_json)
-    chunk_sel = getChunkCoverage(chunk_id, slices, layout)
-
-    # pass query as param
-    params = {}
-    params["query"] = query
-    if limit > 0:
-        params["Limit"] = limit
-    if chunk_map:
-        if chunk_id not in chunk_map:
-            # no data, don't return any results
-            chunk_rsp = {"index": [], "value": []}
-        else:
-            chunk_info = chunk_map[chunk_id]
-            params["s3path"] = chunk_info["s3path"]
-            params["s3offset"] = chunk_info["s3offset"]
-            params["s3size"] = chunk_info["s3size"]
-  
-    # bucket will be used to get dset json even when s3path is used for 
-    # the chunk data
-    params["bucket"] = bucket
-
-    chunk_shape = getSelectionShape(chunk_sel)
-    log.debug(f"chunk_shape: {chunk_shape}")
-    setSliceQueryParam(params, chunk_sel)
- 
-    req = getDataNodeUrl(app, chunk_id)
-    req += "/chunks/" + chunk_id
-    log.debug("GET chunk req: " + req)
-    try:
-        chunk_rsp = await http_get(app, req, params=params)
-    except HTTPNotFound:
-        # no data, don't return any results
-        chunk_rsp = {"index": [], "value": []}
-
-    rsp_dict[chunk_id] = chunk_rsp
-
-
-async def getPointData(app, dset_id, dset_json, points, bucket=None):
-    """
-    Return list of elements from a dataset
-    """
-    loop = asyncio.get_event_loop()
-    num_points = len(points)
-    log.info(f"getPointData {dset_id} for {num_points} points bucket: {bucket}")
-    log.debug(f"points: {points}")
-    if not bucket:
-        msg = "Expected bucket param for getPointData"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
+    if layout_class not in CHUNK_REF_LAYOUTS:
+        msg = f"skip getChunkLocations for layout class: {layout_class}"
+        log.debug(msg)
+        return
 
-    chunk_dict = {}  # chunk ids to list of points in chunk
-    datashape = dset_json["shape"]
-    if datashape["class"] in ('H5S_NULL', 'H5S_SCALAR'):
-        msg = "H5S_NULL, H5S_SCALAR shape classes can not be used with "
-        msg += "point selection"
+    chunk_dims = None
+    if "layout" in dset_json:
+        dset_layout = dset_json["layout"]
+        log.debug(f"dset_json layout: {dset_layout}")
+        if "dims" in dset_layout:
+            chunk_dims = dset_layout["dims"]
+    if chunk_dims is None:
+        msg = "no chunk dimensions set in dataset layout"
         log.error(msg)
         raise HTTPInternalServerError()
-    dims = getShapeDims(datashape)
-    rank = len(dims)
-    type_json = dset_json["type"]
-    dset_dtype = createDataType(type_json)  # np datatype
-    layout = dset_json["layout"]
-    chunk_dims = layout["dims"]  # TBD: What if this is not defined?
-    log.debug(f"chunk_dims: {chunk_dims}")
-
-    for pt_indx in range(num_points):
-        point = points[pt_indx]
-        log.debug(f"point: {point}")
-        if rank == 1:
-            if point < 0 or point >= dims[0]:
-                msg = f"POST Value point: {point} is not within the bounds "
-                msg += "of the dataset"
-                log.warn(msg)
-                raise HTTPBadRequest(reason=msg)
-        else:
-            if len(point) != rank:
-                msg = "POST Value point value did not match dataset rank"
-                log.warn(msg)
-                raise HTTPBadRequest(reason=msg)
-            for i in range(rank):
-                if point[i] < 0 or point[i] >= dims[i]:
-                    msg = f"POST Value point: {point} is not within the "
-                    msg += "bounds of the dataset"
-                    log.warn(msg)
-                    raise HTTPBadRequest(reason=msg)
-        chunk_id = getChunkId(dset_id, point, chunk_dims)
-        log.debug(f"got chunk_id: {chunk_id}")
-        if chunk_id not in chunk_dict:
-            point_list = [point, ]
-            point_index = [pt_indx, ]
-            chunk_entry = {"points": point_list, "indices": point_index}
-            chunk_dict[chunk_id] = chunk_entry
-        else:
-            item = chunk_dict[chunk_id]
-            point_list = item["points"]
-            point_list.append(point)
-            point_index = item["indices"]
-            point_index.append(pt_indx)
-
-    num_chunks = len(chunk_dict)
-    log.debug(f"getPointData - num_chunks: {num_chunks}")
-    max_chunks = config.get("max_chunks_per_request")
-    if max_chunks > 0 and num_chunks > max_chunks:
-        msg = f"Point selection request too large, num_chunks: {num_chunks} "
-        msg == f"max_chunks: {max_chunks}"
-        log.warn(msg)
-        raise HTTPRequestEntityTooLarge(num_chunks, max_chunks)
-
-    # Get information about where chunks are located
-    #   Will be None except for H5D_CHUNKED_REF_INDIRECT type
-    chunk_map = await getChunkInfoMap(app, dset_id, dset_json,
-                                      list(chunk_dict), bucket=bucket)
-    log.debug(f"chunkinfo_map: {chunk_map}")
-
-    # create array to hold response data
-    arr_rsp = np.zeros((num_points,), dtype=dset_dtype)
-    tasks = []
-    for chunk_id in chunk_dict.keys():
-        item = chunk_dict[chunk_id]
-        point_list = item["points"]
-        point_index = item["indices"]
-        task = asyncio.ensure_future(read_point_sel(app,
-                                                    chunk_id,
-                                                    dset_json,
-                                                    point_list,
-                                                    point_index,
-                                                    arr_rsp,
-                                                    chunk_map=chunk_map,
-                                                    bucket=bucket))
-        tasks.append(task)
-    await asyncio.gather(*tasks, loop=loop)
-
-    log.debug(f"arr shape: {arr_rsp.shape}")
-    return arr_rsp
-
-
-async def getChunkInfoMap(app, dset_id, dset_json, chunk_ids, bucket=None):
-    """
-    Get info for chunk locations (for reference layouts)
-    """
-    layout = dset_json["layout"]
-    if layout["class"] not in CHUNK_REF_LAYOUTS:
-        msg = f"skip getChunkInfoMap for layout class: { layout['class'] }"
-        log.debug(msg)
-        return None
 
     datashape = dset_json["shape"]
     datatype = dset_json["type"]
-    if datashape["class"] == 'H5S_NULL':
+    if isNullSpace(dset_json):
         log.error("H5S_NULL shape class used with reference chunk layout")
         raise HTTPInternalServerError()
     dims = getShapeDims(datashape)
     rank = len(dims)
-    msg = f"getChunkInfoMap for dset: {dset_id} bucket: {bucket} "
-    msg += f"rank: {rank} num chunk_ids: {len(chunk_ids)}"
+    # chunk_ids = list(chunkinfo_map.keys())
+    # chunk_ids.sort()
+    num_chunks = len(chunk_ids)
+    msg = f"getChunkLocations for dset: {dset_id} bucket: {bucket} "
+    msg += f"rank: {rank} num chunk_ids: {num_chunks}"
     log.info(msg)
-    log.debug(f"getChunkInfoMap layout: {layout}")
-    chunkinfo_map = {}
+    log.debug(f"getChunkLocations layout: {layout_class}")
 
-    if layout["class"] == 'H5D_CONTIGUOUS_REF':
+    def getChunkItem(chunkid):
+        if chunk_id in chunkinfo_map:
+            chunk_item = chunkinfo_map[chunk_id]
+        else:
+            chunk_item = {}
+            chunkinfo_map[chunk_id] = chunk_item
+        return chunk_item
+
+    if layout_class == "H5D_CONTIGUOUS_REF":
+        layout = getDatasetCreationPropertyLayout(dset_json)
+        log.debug(f"cpl layout: {layout}")
         s3path = layout["file_uri"]
         s3size = layout["size"]
         if s3size == 0:
-            msg = "getChunkInfoMap - H5D_CONTIGUOUS_REF layout size 0, "
+            msg = "getChunkLocations - H5D_CONTIGUOUS_REF layout size 0, "
             msg += "no allocation"
             log.info(msg)
-            return None
-        chunk_dims = layout["dims"]
+            return
         item_size = getItemSize(datatype)
         chunk_size = item_size
         for dim in chunk_dims:
             chunk_size *= dim
         log.debug(f"using chunk_size: {chunk_size} for H5D_CONTIGUOUS_REF")
 
         for chunk_id in chunk_ids:
-            log.debug(f"getChunkInfoMap - getting data for chunk: {chunk_id}")
+            log.debug(f"getChunkLocations - getting data for chunk: {chunk_id}")
+            chunk_item = getChunkItem(chunk_id)
             chunk_index = getChunkIndex(chunk_id)
             if len(chunk_index) != rank:
                 log.error("Unexpected chunk_index")
                 raise HTTPInternalServerError()
             extent = item_size
             if "offset" not in layout:
-                msg = "getChunkInfoMap - expected to find offset in chunk "
+                msg = "getChunkLocations - expected to find offset in chunk "
                 msg += "layout for H5D_CONTIGUOUS_REF"
                 log.error(msg)
                 continue
             s3offset = layout["offset"]
             if not isinstance(s3offset, int):
-                msg = "getChunkInfoMap - expected offset to be an int but "
+                msg = "getChunkLocations - expected offset to be an int but "
                 msg += f"got: {s3offset}"
                 log.error(msg)
                 continue
-            log.debug(f"getChunkInfoMap s3offset: {s3offset}")
+            log.debug(f"getChunkLocations s3offset: {s3offset}")
             for i in range(rank):
                 dim = rank - i - 1
                 index = chunk_index[dim]
                 s3offset += index * chunk_dims[dim] * extent
                 extent *= dims[dim]
             msg = f"setting chunk_info_map to s3offset: {s3offset} "
             msg == f"s3size: {s3size} for chunk_id: {chunk_id}"
             log.debug(msg)
             if s3offset > layout["offset"] + layout["size"]:
                 msg = f"range get of s3offset: {s3offset} s3size: {s3size} "
                 msg += "extends beyond end of contiguous dataset for "
                 msg += f"chunk_id: {chunk_id}"
                 log.warn(msg)
-            chunkinfo_map[chunk_id] = {"s3path": s3path,
-                                       "s3offset": s3offset,
-                                       "s3size": chunk_size}
-    elif layout["class"] == 'H5D_CHUNKED_REF':
+            chunk_item["s3path"] = s3path
+            chunk_item["s3offset"] = s3offset
+            chunk_item["s3size"] = chunk_size
+    elif layout_class == "H5D_CHUNKED_REF":
+        layout = getDatasetCreationPropertyLayout(dset_json)
+        log.debug(f"cpl layout: {layout}")
         s3path = layout["file_uri"]
         chunks = layout["chunks"]
 
         for chunk_id in chunk_ids:
+            chunk_item = getChunkItem(chunk_id)
             s3offset = 0
             s3size = 0
             chunk_key = getChunkSuffix(chunk_id)
             if chunk_key in chunks:
                 item = chunks[chunk_key]
                 s3offset = item[0]
                 s3size = item[1]
-            chunkinfo_map[chunk_id] = {"s3path": s3path,
-                                       "s3offset": s3offset,
-                                       "s3size": s3size}
-    elif layout["class"] == 'H5D_CHUNKED_REF_INDIRECT':
+            chunk_item["s3path"] = s3path
+            chunk_item["s3offset"] = s3offset
+            chunk_item["s3size"] = s3size
+
+    elif layout_class == "H5D_CHUNKED_REF_INDIRECT":
+        layout = getDatasetCreationPropertyLayout(dset_json)
+        log.debug(f"cpl layout: {layout}")
         if "chunk_table" not in layout:
             log.error("Expected to find chunk_table in dataset layout")
             raise HTTPInternalServerError()
         chunktable_id = layout["chunk_table"]
         # get  state for dataset from DN.
         kwargs = {"bucket": bucket, "refresh": False}
         chunktable_json = await getObjectJson(app, chunktable_id, **kwargs)
-        log.debug(f"chunktable_json: {chunktable_json}")
+        # log.debug(f"chunktable_json: {chunktable_json}")
         chunktable_dims = getShapeDims(chunktable_json["shape"])
-        # TBD: verify chunktable type
+        chunktable_layout = chunktable_json["layout"]
+        if chunktable_layout.get("class") == "H5D_CHUNKED_REF_INDIRECT":
+            # We don't support recursive chunked_ref_indirect classes
+            msg = "chunktable layout: H5D_CHUNKED_REF_INDIRECT is invalid"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
 
         if len(chunktable_dims) != rank:
             msg = "Rank of chunktable should be same as the dataset"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
 
         # convert the list of chunk_ids into a set of points to query in
         # the chunk table
-        num_pts = len(chunk_ids)
+        log.debug(f"datashape: {dims}")
+        log.debug(f"chunk_dims: {chunk_dims}")
+        log.debug(f"chunktable_dims: {chunktable_dims}")
+        default_chunktable_dims = get_chunktable_dims(dims, chunk_dims)
+        log.debug(f"default_chunktable_dims: {default_chunktable_dims}")
+        table_factors = []
+        if "hyper_dims" in layout:
+            hyper_dims = layout["hyper_dims"]
+        else:
+            # assume 1 to 1 matching
+            hyper_dims = chunk_dims
+        ref_num_chunks = num_chunks
+        for dim in range(rank):
+            if chunk_dims[dim] % hyper_dims[dim] != 0:
+                msg = f"expected hyper_dims [{hyper_dims[dim]}] to be a factor"
+                msg += f" of {chunk_dims[dim]}"
+                log.warn(msg)
+                raise HTTPBadRequest(reason=msg)
+            factor = chunk_dims[dim] // hyper_dims[dim]
+            table_factors.append(factor)
+            ref_num_chunks *= factor
+        log.debug(f"table_factors: {table_factors}")
+        log.debug(f"ref_num_chunks: {ref_num_chunks}")
+        log.debug(f"hyper_dims: {hyper_dims}")
+
         if rank == 1:
-            arr_points = np.zeros((num_pts,), dtype=np.dtype('u8'))
+            arr_points = np.zeros((ref_num_chunks,), dtype=np.dtype("u8"))
+            table_factor = table_factors[0]
+            for i in range(num_chunks):
+                chunk_id = chunk_ids[i]
+                log.debug(f"chunk_id: {chunk_id}")
+                chunk_index = getChunkIndex(chunk_id)
+                chunk_index = chunk_index[0]
+                log.debug(f"chunk_index: {chunk_index}")
+                for j in range(table_factor):
+                    index = chunk_index * table_factor + j
+                    arr_index = i * table_factor + j
+                    arr_points[arr_index] = index
         else:
-            arr_points = np.zeros((num_pts, rank), dtype=np.dtype('u8'))
-        for i in range(len(chunk_ids)):
-            chunk_id = chunk_ids[i]
-            log.debug(f"chunk_id for chunktable: {chunk_id}")
-            indx = getChunkIndex(chunk_id)
-            log.debug(f"get chunk indx: {indx}")
-            if rank == 1:
-                log.debug(f"convert: {indx[0]} to {indx}")
-                indx = indx[0]
-            arr_points[i] = indx
-        msg = f"got chunktable points: {arr_points}, calling getPointData"
+            if ref_num_chunks != num_chunks:
+                msg = "hyperchunks not supported for multidimensional datasets"
+                log.warn(msg)
+                raise HTTPBadRequest(msg=msg)
+            arr_points = np.zeros((num_chunks, rank), dtype=np.dtype("u8"))
+            for i in range(num_chunks):
+                chunk_id = chunk_ids[i]
+                log.debug(f"chunk_id for chunktable: {chunk_id}")
+                indx = getChunkIndex(chunk_id)
+                log.debug(f"get chunk indx: {indx}")
+                arr_points[i] = indx
+
+        msg = f"got chunktable points: {arr_points}, calling getSelectionData"
         log.debug(msg)
-        point_data = await getPointData(app,
-                                        chunktable_id,
-                                        chunktable_json,
-                                        arr_points,
-                                        bucket=bucket)
+        # this call won't lead to a circular loop of calls since we've checked
+        # that the chunktable layout is not H5D_CHUNKED_REF_INDIRECT
+        kwargs = {"points": arr_points, "bucket": bucket}
+        point_data = await getSelectionData(app, chunktable_id, chunktable_json, **kwargs)
+
         log.debug(f"got chunktable data: {point_data}")
         if "file_uri" in layout:
             s3_layout_path = layout["file_uri"]
+            log.debug(f"got s3_layout_path: {s3_layout_path}")
         else:
             s3_layout_path = None
 
-        for i in range(len(chunk_ids)):
+        for i in range(num_chunks):
             chunk_id = chunk_ids[i]
+            chunk_item = getChunkItem(chunk_id)
             item = point_data[i]
-            log.debug(f"got item: {item}")
-            s3offset = int(item[0])
-            s3size = int(item[1])
             if s3_layout_path is None:
                 if len(item) < 3:
                     msg = "expected chunk table to have three fields"
                     log.warn(msg)
                     raise HTTPBadRequest(reason=msg)
                 e = item[2]
                 if e:
-                    s3path = e.decode('utf-8')
+                    s3path = e.decode("utf-8")
                     log.debug(f"got s3path: {s3path}")
             else:
                 s3path = s3_layout_path
+            chunk_item["s3path"] = s3path
+
+            if ref_num_chunks == num_chunks:
+                item = point_data[i]
+                s3offset = int(item[0])
+                s3size = int(item[1])
+                chunk_item["s3offset"] = s3offset
+                chunk_item["s3size"] = s3size
+            else:
+                factor = ref_num_chunks // num_chunks
+                s3offsets = []
+                s3sizes = []
+                for j in range(factor):
+                    item = point_data[i * factor + j]
+                    s3offset = int(item[0])
+                    s3offsets.append(s3offset)
+                    s3size = int(item[1])
+                    s3sizes.append(s3size)
+                chunk_item["s3offset"] = s3offsets
+                chunk_item["s3size"] = s3sizes
+                chunk_item["hyper_dims"] = hyper_dims
 
-            chunkinfo_map[chunk_id] = {"s3path": s3path,
-                                       "s3offset": s3offset,
-                                       "s3size": s3size}
     else:
         log.error(f"Unexpected chunk layout: {layout['class']}")
         raise HTTPInternalServerError()
 
     log.debug(f"returning chunkinfo_map: {chunkinfo_map}")
     return chunkinfo_map
 
 
-async def write_chunk_query(app, chunk_id, dset_json, slices, query,
-                            query_update, limit, bucket=None):
-    """ update the chunk selection from the DN based on query string
-    chunk_id: id of chunk to write to
-    chunk_sel: chunk-relative selection to read from
-    np_arr: numpy array to store read bytes
-    """
-    # TBD = see if this code can be merged with the read_chunk_query function
-    msg = f"write_chunk_query, chunk_id: {chunk_id}, slices: {slices}, "
-    msg += f"query: {query}, query_udpate: {query_update}"
-    log.info(msg)
-    partition_chunk_id = getChunkIdForPartition(chunk_id, dset_json)
-    if partition_chunk_id != chunk_id:
-        log.debug(f"using partition_chunk_id: {partition_chunk_id}")
-        chunk_id = partition_chunk_id  # replace the chunk_id
-
-    req = getDataNodeUrl(app, chunk_id)
-    req += "/chunks/" + chunk_id
-    log.debug("PUT chunk req: " + req)
-
-    layout = getChunkLayout(dset_json)
-    chunk_sel = getChunkCoverage(chunk_id, slices, layout)
-
-    # pass query as param
-    params = {}
-    params["query"] = query
-    if limit > 0:
-        params["Limit"] = limit
-    if bucket:
-        params["bucket"] = bucket
-
-    chunk_shape = getSelectionShape(chunk_sel)
-    log.debug(f"chunk_shape: {chunk_shape}")
-    setSliceQueryParam(params, chunk_sel)
-    try:
-        dn_rsp = await http_put(app, req, data=query_update, params=params)
-    except HTTPNotFound:
-        # no data, don't return any results
-        dn_rsp = {"index": [], "value": []}
-
-    return dn_rsp
-
-
-async def doPutQuery(request, query_update, dset_json):
-    """
-    Helper function for PUT queries
-    """
-    app = request.app
-    params = request.rel_url.query
-    if not isinstance(query_update, dict):
-        msg = "Expected dict type for PUT query body, but "
-        msg += f"got: {type(query_update)}"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
-    query = params["query"]
-    domain = getDomainFromRequest(request)
-    bucket = getBucketForDomain(domain)
-     
-    datashape = dset_json["shape"]
-    dims = getShapeDims(datashape)
-    num_rows = dims[0]
-    log.debug(f"doPutQuery - num_rows: {num_rows}")
-
-    type_json = dset_json["type"]
-    log.debug(f"doPutQuery - type json: {type_json}")
-
-    if type_json["class"] != 'H5T_COMPOUND':
-        msg = "Expected compound type for PUT query operation"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
-
-    fields = type_json["fields"]
-    field_names = set()
-    for field in fields:
-        field_names.add(field['name'])
-    for key in query_update:
-        if key not in field_names:
-            msg = f"Unknown fieldname: {key} in update body"
-            log.warn(msg)
-            raise HTTPBadRequest(reason=msg)
-
-    limit = 0
-    if "Limit" in params:
-        try:
-            limit = int(params["Limit"])
-        except ValueError:
-            msg = "Invalid Limit query param"
-            log.warn(msg)
-            raise HTTPBadRequest(reason=msg)
-
-    if "select" in params:
-        select = params["select"]
-    else:
-        select = None
-    try:
-        slices = getSelectionList(select, dims)
-    except ValueError as ve:
-        msg = str(ve)
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
-     
-
-    msg = f"doPutQuery - got dim_slice: {slices[0]}"
-    log.info(msg)
-
+def get_chunk_selections(chunk_map, chunk_ids, slices, dset_json):
+    """Update chunk_map with chunk and data selections for the
+    given set of slices
+    """
+    log.debug(f"get_chunk_selections - chunk_ids: {chunk_ids}")
+    if not slices:
+        log.debug("no slices set, returning")
+        return  # nothing to do
+    log.debug(f"slices: {slices}")
     layout = getChunkLayout(dset_json)
+    for chunk_id in chunk_ids:
+        if chunk_id in chunk_map:
+            item = chunk_map[chunk_id]
+        else:
+            item = {}
+            chunk_map[chunk_id] = item
 
-    num_chunks = getNumChunks(slices, layout)
-    log.debug(f"doPutQuery - num_chunks: {num_chunks}")
-    max_chunks = int(config.get('max_chunks_per_request'))
-    if num_chunks > max_chunks:
-        log.warn(f"doPutQuery - too many chunks: {num_chunks}, {max_chunks}")
-        raise HTTPRequestEntityTooLarge(num_chunks, max_chunks)
-
-    dset_id = dset_json["id"]
-
-    try:
-        chunk_ids = getChunkIds(dset_id, slices, layout)
-    except ValueError:
-        log.warn("doPutQuery - getChunkIds failed")
-        raise HTTPInternalServerError()
-    log.debug(f"doPutQuery - chunk_ids: {chunk_ids}")
-
-    node_count = getNodeCount(app)
-    if node_count == 0:
-        log.warn("PutQuery request with no active dn nodes")
-        raise HTTPServiceUnavailable()
-    resp_index = []
-    resp_value = []
-    chunk_index = 0
-    num_chunks = len(chunk_ids)
-    count = 0
-
-    while chunk_index < num_chunks:
-        next_chunks = []
-        for i in range(node_count):
-            next_chunks.append(chunk_ids[chunk_index])
-            chunk_index += 1
-            if chunk_index >= num_chunks:
-                break
-        log.debug(f"doPutQuery - next chunk ids: {next_chunks}")
-        # run query on DN nodes
-        # do write_chunks sequentially do avoid exceeding the limit value
-        for chunk_id in next_chunks:
-            dn_rsp = await write_chunk_query(app,
-                                             chunk_id,
-                                             dset_json,
-                                             slices,
-                                             query,
-                                             query_update,
-                                             limit,
-                                             bucket=bucket)
-            log.debug(f"write_chunk_query: {dn_rsp}")
-            num_hits = len(dn_rsp["index"])
-            count += num_hits
-            msg = f"doPutQuery - got {num_hits} for chunk_id: {chunk_id}, "
-            msg += f"total: {count}"
-            log.debug(msg)
-            resp_index.extend(dn_rsp["index"])
-            resp_value.extend(dn_rsp["value"])
-            if limit > 0 and count >= limit:
-                log.debug(f"doPutQuery - reached limit: {limit}")
-                break
-        if limit > 0 and count >= limit:
-            # break out of outer loop
-            break
-
-    resp_json = {"index": resp_index, "value": resp_value}
-    resp_json["hrefs"] = get_hrefs(request, dset_json)
-    log.debug(f"doPutQuery - done returning {count} values")
-    return resp_json
+        chunk_sel = getChunkCoverage(chunk_id, slices, layout)
+        log.debug(
+            f"get_chunk_selections - chunk_id: {chunk_id}, chunk_sel: {chunk_sel}"
+        )
+        item["chunk_sel"] = chunk_sel
+        data_sel = getDataCoverage(chunk_id, slices, layout)
+        log.debug(f"get_chunk_selections - data_sel: {data_sel}")
+        item["data_sel"] = data_sel
 
 
 async def PUT_Value(request):
     """
     Handler for PUT /<dset_uuid>/value request
     """
     log.request(request)
     app = request.app
-    loop = asyncio.get_event_loop()
     bucket = None
     body = None
     query = None
     json_data = None
     params = request.rel_url.query
     append_rows = None  # this is a append update or not
     append_dim = 0
@@ -956,23 +439,23 @@
         try:
             append_dim = int(params["append_dim"])
         except ValueError:
             msg = "invalid append_dim"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         log.info(f"append_dim: {append_dim}")
-   
+
     if "query" in params:
         if "append" in params:
             msg = "Query string can not be used with append parameter"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         query = params["query"]
 
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
     if not dset_id:
         msg = "Missing dataset id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(dset_id, "Dataset"):
         msg = f"Invalid dataset id: {dset_id}"
         log.warn(msg)
@@ -984,35 +467,30 @@
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     bucket = getBucketForDomain(domain)
 
-    request_type = "json"
-    if "Content-Type" in request.headers:
-        # client should use "application/octet-stream" for binary transfer
-        content_type = request.headers["Content-Type"]
-        if content_type not in EXPECTED_CONTENT_TYPES:
-            msg = f"Unknown content_type: {content_type}"
-            log.warn(msg)
-            raise HTTPBadRequest(reason=msg)
-        if content_type == "application/octet-stream":
-            log.debug("PUT value - request_type is binary")
-            request_type = "binary"
-        else:
-            log.debug("PUT value - request type is json")
+    request_type = getContentType(request)
+
+    log.debug(f"PUT value - request_type is {request_type}")
 
     if not request.has_body:
         msg = "PUT Value with no body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     if request_type == "json":
-        body = await request.json()
+        try:
+            body = await request.json()
+        except JSONDecodeError:
+            msg = "Unable to load JSON body"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
         if "append" in body and body["append"]:
             try:
                 append_rows = int(body["append"])
             except ValueError:
                 msg = "invalid append value in body"
                 log.warn(msg)
                 raise HTTPBadRequest(reason=msg)
@@ -1034,15 +512,15 @@
             log.info(f"append_dim: {append_dim}")
 
     # get state for dataset from DN.
     dset_json = await getObjectJson(app, dset_id, bucket=bucket, refresh=False)
 
     layout = None
     datashape = dset_json["shape"]
-    if datashape["class"] == 'H5S_NULL':
+    if datashape["class"] == "H5S_NULL":
         msg = "Null space datasets can not be used as target for PUT value"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     dims = getShapeDims(datashape)
     maxdims = getDsetMaxDims(dset_json)
     rank = len(dims)
@@ -1051,44 +529,137 @@
         msg = "Query string is not supported for multidimensional arrays"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     layout = getChunkLayout(dset_json)
 
     type_json = dset_json["type"]
+    dset_dtype = createDataType(type_json)
     item_size = getItemSize(type_json)
-    log.debug(f"item size: {item_size}")
-
-    if query and request_type != "json":
-        msg = "Only JSON is supported for query updates"
-        log.warn(msg)
-        raise HTTPBadRequest(reason=msg)
-
-    await validateAction(app, domain, dset_id, username, "update")
+    max_request_size = int(config.get("max_request_size"))
 
     if query:
         # divert here if we are doing a put query
-        put_query_rsp = await doPutQuery(request, body, dset_json)
-        resp = await jsonResponse(request, put_query_rsp)
+        # returns array data like a GET query request
+        log.debug(f"got query: {query}")
+        try:
+            parser = BooleanParser(query)
+        except Exception:
+            msg = f"query: {query} is not valid"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
+
+        field_names = set(dset_dtype.names)
+        variables = parser.getVariables()
+        for variable in variables:
+            if variable not in field_names:
+                msg = f"query variable {variable} not valid"
+                log.warn(msg)
+                raise HTTPBadRequest(reason=msg)
+
+        select = params.get("select")
+        slices = await get_slices(app, select, dset_json, bucket=bucket)
+        if "Limit" in params:
+            try:
+                limit = int(params["Limit"])
+            except ValueError:
+                msg = "Limit param must be positive int"
+                log.warning(msg)
+                raise HTTPBadRequest(reason=msg)
+        else:
+            limit = 0
+
+        arr_rsp = await getSelectionData(
+            app,
+            dset_id,
+            dset_json,
+            slices,
+            query=query,
+            bucket=bucket,
+            limit=limit,
+            query_update=body,
+            method=request.method,
+        )
+
+        log.debug(f"arr shape: {arr_rsp.shape}")
+        response_type = getAcceptType(request)
+
+        if response_type == "binary":
+            output_data = arr_rsp.tobytes()
+            msg = f"PUT_Value query - returning {len(output_data)} bytes binary data"
+            log.debug(msg)
+
+            # write response
+            try:
+                resp = StreamResponse()
+                if config.get("http_compression"):
+                    log.debug("enabling http_compression")
+                    resp.enable_compression()
+                resp.headers["Content-Type"] = "application/octet-stream"
+                resp.content_length = len(output_data)
+                await resp.prepare(request)
+                await resp.write(output_data)
+                await resp.write_eof()
+            except Exception as e:
+                log.error(f"Exception during binary data write: {e}")
+        else:
+            log.debug("PUT Value query - returning JSON data")
+            rsp_json = {}
+            data = arr_rsp.tolist()
+            log.debug(f"got rsp data {len(data)} points")
+            json_query_data = bytesArrayToList(data)
+            rsp_json["value"] = json_query_data
+            rsp_json["hrefs"] = get_hrefs(request, dset_json)
+            resp = await jsonResponse(request, rsp_json)
+        log.response(request, resp=resp)
         return resp
 
+    # Resume regular PUT_Value processing without query update
     dset_dtype = createDataType(type_json)  # np datatype
     binary_data = None
-    np_shape = None  # expected shape of input data
     points = None  # used for point selection writes
     np_shape = []  # shape of incoming data
-    slices = []    # selection area to write to
+    slices = []  # selection area to write to
+
+    if item_size == 'H5T_VARIABLE' or not use_http_streaming(request, rank):
+        http_streaming = False
+    else:
+        http_streaming = True
+
+    # body could also contain a point selection specifier
+    if body and "points" in body:
+        if append_rows:
+            msg = "points not valid with append update"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
+
+        json_points = body["points"]
+        num_points = len(json_points)
+        if rank == 1:
+            point_shape = (num_points,)
+            log.info(f"rank 1: point_shape: {point_shape}")
+        else:
+            point_shape = (num_points, rank)
+            log.info(f"rank >1: point_shape: {point_shape}")
+        try:
+            # use uint64 so we can address large array extents
+            dt = np.dtype(np.uint64)
+            points = jsonToArray(point_shape, dt, json_points)
+        except ValueError:
+            msg = "Bad Request: point list not valid for dataset shape"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
 
     if append_rows:
         # shape must be extensible
         if not isExtensible(dims, maxdims):
             msg = "Dataset shape must be extensible for packet updates"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-        if append_dim < 0 or append_dim > rank-1:
+        if append_dim < 0 or append_dim > rank - 1:
             msg = "invalid append_dim"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         maxdims = getDsetMaxDims(dset_json)
         if maxdims[append_dim] != 0:
             if dims[append_dim] + append_rows > maxdims[append_dim]:
                 log.warn("unable to append to dataspace")
@@ -1097,172 +668,140 @@
     # refetch the dims if the dataset is extensible
     if isExtensible(dims, maxdims):
         kwargs = {"bucket": bucket, "refresh": True}
         dset_json = await getObjectJson(app, dset_id, **kwargs)
         dims = getShapeDims(dset_json["shape"])
 
     if request_type == "json":
-        body_json = body
-    else:
-        body_json = None
-
-    if request_type == "json":
         if "value" in body:
             json_data = body["value"]
+
         elif "value_base64" in body:
             base64_data = body["value_base64"]
             base64_data = base64_data.encode("ascii")
             binary_data = base64.b64decode(base64_data)
         else:
             msg = "PUT value has no value or value_base64 key in body"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-
-        # body could also contain a point selection specifier
-        if "points" in body:
-            if append_rows:
-                msg = "points not valid with packet update"
-                log.warn(msg)
-                raise HTTPBadRequest(reason=msg)
-
-            json_points = body["points"]
-            num_points = len(json_points)
-            if rank == 1:
-                point_shape = (num_points,)
-                log.info(f"rank 1: point_shape: {point_shape}")
-            else:
-                point_shape = (num_points, rank)
-                log.info(f"rank >1: point_shape: {point_shape}")
-            try:
-                # use uint64 so we can address large array extents
-                dt = np.dtype(np.uint64)
-                points = jsonToArray(point_shape, dt, json_points)
-            except ValueError:
-                msg = "Bad Request: point list not valid for dataset shape"
-                log.warn(msg)
-                raise HTTPBadRequest(reason=msg)
     else:
-        # read binary data
+        # read binary data from request
         log.info(f"request content_length: {request.content_length}")
-        max_request_size = int(config.get("max_request_size"))
+
         if isinstance(request.content_length, int):
             if request.content_length >= max_request_size:
-                msg = f"Request size too large: {request.content_length} "
-                msg += f"max: {max_request_size}"
-                log.warn(msg)
-                raise HTTPRequestEntityTooLarge(request.content_length,
-                                                max_request_size)
+                if http_streaming:
+                    # just do an info log that we'll be paginating over a large request
+                    msg = f"will paginate over large request with {request.content_length} bytes"
+                    log.info(msg)
+                else:
+                    msg = f"Request size {request.content_length} too large "
+                    msg += f"for variable length data, max: {max_request_size}"
+                    log.warn(msg)
+                    raise HTTPRequestEntityTooLarge(max_request_size, request.content_length)
 
-        try:
-            binary_data = await request_read(request)
-        except HTTPRequestEntityTooLarge as tle:
-            msg = "Got HTTPRequestEntityTooLarge exception during "
-            msg += f"binary read: {tle})"
-            log.warn(msg)
-            raise  # re-throw
+        if not http_streaming:
+            # read the request data now
+            # TBD: support streaming for variable length types
+            try:
+                binary_data = await request_read(request)
+            except HTTPRequestEntityTooLarge as tle:
+                msg = "Got HTTPRequestEntityTooLarge exception during "
+                msg += f"binary read: {tle})"
+                log.warn(msg)
+                raise  # re-throw
 
-        if len(binary_data) != request.content_length:
-            msg = f"Read {len(binary_data)} bytes, expecting: "
-            msg += f"{request.content_length}"
-            log.error(msg)
-            raise HTTPBadRequest(reason=msg)
+            if len(binary_data) != request.content_length:
+                msg = f"Read {len(binary_data)} bytes, expecting: "
+                msg += f"{request.content_length}"
+                log.error(msg)
+                raise HTTPBadRequest(reason=msg)
 
     if append_rows:
         for i in range(rank):
             if i == append_dim:
                 np_shape.append(append_rows)
                 # this will be adjusted once the dataspace is extended
                 slices.append(slice(0, append_rows, 1))
             else:
                 if dims[i] == 0:
                     dims[i] = 1  # need a non-zero extent for all dimensionas
                 np_shape.append(dims[i])
                 slices.append(slice(0, dims[i], 1))
+        log.debug(f"np_shape based on append_rows: {np_shape}")
         np_shape = tuple(np_shape)
 
     elif points is None:
-        if body_json and "start" in body_json and "stop" in body_json:
-            try:
-                slices = getSelectionList(body_json, dims)
-            except ValueError as ve:
-                msg = str(ve)
-                log.warn(msg)
-                raise HTTPBadRequest(reason=msg)
+        if body and "start" in body and "stop" in body:
+            slices = await get_slices(app, body, dset_json, bucket=bucket)
         else:
-            if "select" in params:
-                select = params["select"]
-            else:
-                select = None  # will get slices for entire datashape
-            try:
-                slices = getSelectionList(select, dims)
-            except ValueError as ve:
-                msg = str(ve)
-                log.warn(msg)
-                raise HTTPBadRequest(reason=msg)
+            select = params.get("select")
+            slices = await get_slices(app, select, dset_json, bucket=bucket)
 
         # The selection parameters will determine expected put value shape
         log.debug(f"PUT Value selection: {slices}")
         # not point selection, get hyperslab selection shape
         np_shape = getSelectionShape(slices)
-        num_elements = getNumElements(np_shape)
     else:
         # point update
         np_shape = (num_points,)
-        num_elements = num_points
-    log.debug(f"selection shape: {np_shape}")
 
+    log.debug(f"selection shape: {np_shape}")
     num_elements = getNumElements(np_shape)
     log.debug(f"selection num elements: {num_elements}")
     if num_elements <= 0:
         msg = "Selection is empty"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     arr = None  # np array to hold request data
     if binary_data and isinstance(item_size, int):
         # binary, fixed item_size
-        if num_elements*item_size != len(binary_data):
+        if num_elements * item_size != len(binary_data):
             msg = f"Expected: {num_elements*item_size} bytes, "
-            msg += f"but got: {len(binary_data)}"
+            msg += f"but got: {len(binary_data)}, "
+            msg += f"num_elements: {num_elements}, item_size: {item_size}"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
+        if num_elements * item_size > max_request_size:
+            msg = f"read {num_elements*item_size} bytes, greater than {max_request_size}"
+            log.warn(msg)
         arr = np.fromstring(binary_data, dtype=dset_dtype)
         try:
             arr = arr.reshape(np_shape)  # conform to selection shape
         except ValueError:
             msg = "Bad Request: binary input data doesn't match selection"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         msg = f"PUT value - numpy array shape: {arr.shape} dtype: {arr.dtype}"
         log.debug(msg)
-    elif binary_data and item_size == 'H5T_VARIABLE':
+    elif binary_data and item_size == "H5T_VARIABLE":
         # binary variable length data
         try:
             arr = bytesToArray(binary_data, dset_dtype, np_shape)
         except ValueError as ve:
             log.warn(f"bytesToArray value error: {ve}")
             raise HTTPBadRequest()
-        log.debug(f"got vlen arr: {arr}")
-    else:
-        #
-        # data is json
-        #
+    elif request_type == "json":
+        # get array from json input
         try:
             msg = "input data doesn't match selection"
             arr = jsonToArray(np_shape, dset_dtype, json_data)
         except ValueError:
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         except TypeError:
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         except IndexError:
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         log.debug(f"got json arr: {arr.shape}")
+    else:
+        log.debug("will using streaming for request data")
 
     if append_rows:
         # extend the shape of the dataset
         req = getDataNodeUrl(app, dset_id) + "/datasets/" + dset_id + "/shape"
         body = {"extend": append_rows, "extend_dim": append_dim}
         params = {}
         if bucket:
@@ -1282,19 +821,19 @@
         # selection should be in the format [:,n:m,:].
         # extract n and m and use it to update the slice for the
         # appending dimension
         if not selection.startswith("[") or not selection.endswith("]"):
             log.error("Unexpected selection in PUT shape response")
             raise HTTPInternalServerError()
         selection = selection[1:-1]  # strip off brackets
-        parts = selection.split(',')
+        parts = selection.split(",")
         for part in parts:
             if part == ":":
                 continue
-            bounds = part.split(':')
+            bounds = part.split(":")
             if len(bounds) != 2:
                 log.error("Unexpected selection in PUT shape response")
                 raise HTTPInternalServerError()
             lb = ub = 0
             try:
                 lb = int(bounds[0])
                 ub = int(bounds[1])
@@ -1302,73 +841,100 @@
                 log.error("Unexpected selection in PUT shape response")
                 raise HTTPInternalServerError()
             log.info(f"lb: {lb} ub: {ub}")
             # update the slices to indicate where to place the data
             slices[append_dim] = slice(lb, ub, 1)
 
     slices = tuple(slices)  # no more edits to slices
-
+    crawler_status = None  # will be set below
     if points is None:
-        # for hyperslab selection, verify the input shape matches the
-        # selection
-        np_index = 0
-        for dim in range(len(arr.shape)):
-            data_extent = arr.shape[dim]
-            selection_extent = 1
-            if np_index < len(np_shape):
-                selection_extent = np_shape[np_index]
-            if selection_extent == data_extent:
-                np_index += 1
-                continue  # good
-            if data_extent == 1:
-                continue  # skip singleton selection
-            if selection_extent == 1:
-                np_index += 1
-                continue  # skip singleton selection
-
-            # selection/data mismatch!
-            msg = "data shape doesn't match selection shape"
-            msg += "--data shape: " + str(arr.shape)
-            msg += "--selection shape: " + str(np_shape)
-            log.warn(msg)
-            raise HTTPBadRequest(reason=msg)
-
-        num_chunks = getNumChunks(slices, layout)
-        log.debug(f"num_chunks: {num_chunks}")
-        max_chunks = int(config.get('max_chunks_per_request'))
-        if num_chunks > max_chunks:
-            log.warn(f"PUT value too many chunks: {num_chunks}, {max_chunks}")
-            raise HTTPRequestEntityTooLarge(num_chunks, max_chunks)
+        if arr is not None:
+            # make a one page list to handle the write in one chunk crawler run
+            # (larger write request should user binary streaming)
+            pages = (slices,)
+            log.debug(f"non-streaming data, setting page list to: {slices}")
+        else:
+            pages = getSelectionPagination(slices, dims, item_size, max_request_size)
+            log.debug(f"getSelectionPagination returned: {len(pages)} pages")
+        bytes_streamed = 0
+        max_chunks = int(config.get("max_chunks_per_request", default=1000))
+
+        for page_number in range(len(pages)):
+            page = pages[page_number]
+            msg = f"streaming request data for page: {page_number+1} of {len(pages)}, "
+            msg += f"selection: {page}"
+            log.info(msg)
+            num_chunks = getNumChunks(page, layout)
+            log.debug(f"num_chunks: {num_chunks}")
+            if num_chunks > max_chunks:
+                log.warn(
+                    f"PUT value chunk count: {num_chunks} exceeds max_chunks: {max_chunks}"
+                )
+            select_shape = getSelectionShape(page)
+            log.debug(f"got select_shape: {select_shape} for page: {page}")
+            num_bytes = math.prod(select_shape) * item_size
+            if arr is None or page_number > 0:
+                log.debug(
+                    f"page: {page_number} reading {num_bytes} from request stream"
+                )
+                # read page of data from input stream
+                try:
+                    page_bytes = await request_read(request, count=num_bytes)
+                except HTTPRequestEntityTooLarge as tle:
+                    msg = "Got HTTPRequestEntityTooLarge exception during "
+                    msg += f"binary read: {tle})"
+                    log.warn(msg)
+                    raise  # re-throw
+                except IncompleteReadError as ire:
+                    msg = "Got asyncio.IncompleteReadError during binary "
+                    msg += f"read: {ire}"
+                    log.warn(msg)
+                    raise HTTPBadRequest(reason=msg)
+                log.debug(f"read {len(page_bytes)} for page: {page_number+1}")
+                bytes_streamed += len(page_bytes)
+                try:
+                    arr = bytesToArray(page_bytes, dset_dtype, select_shape)
+                except ValueError as ve:
+                    msg = f"bytesToArray value error for page: {page_number+1}: {ve}"
+                    log.warn(msg)
+                    raise HTTPBadRequest(reason=msg)
+                if len(select_shape) == 2:
+                    log.debug(f"arr test value[0,0]: {arr[0,0]}")
 
-        try:
-            chunk_ids = getChunkIds(dset_id, slices, layout)
-        except ValueError:
-            log.warn("getChunkIds failed")
-            raise HTTPInternalServerError()
-        log.debug(f"chunk_ids: {chunk_ids}")
+            try:
+                chunk_ids = getChunkIds(dset_id, page, layout)
+            except ValueError:
+                log.warn("getChunkIds failed")
+                raise HTTPInternalServerError()
+            log.debug(f"chunk_ids: {chunk_ids}")
+            if len(chunk_ids) > max_chunks:
+                log.warn(
+                    f"got {len(chunk_ids)} for page: {page_number+1}.  max_chunks: {max_chunks} "
+                )
+
+            crawler = ChunkCrawler(
+                app,
+                chunk_ids,
+                dset_json=dset_json,
+                bucket=bucket,
+                slices=page,
+                arr=arr,
+                action="write_chunk_hyperslab",
+            )
+            await crawler.crawl()
+
+            crawler_status = crawler.get_status()
+
+            if crawler_status not in (200, 201):
+                log.warn(
+                    f"crawler failed for page: {page_number+1} with status: {crawler_status}"
+                )
+            else:
+                log.info("crawler write_chunk_hyperslab successful")
 
-        tasks = []
-        node_count = getNodeCount(app)
-        if node_count == 0:
-            log.warn("write_chunk_hyperslab request with no active dn nodes")
-            raise HTTPServiceUnavailable()
-        task_batch_size = node_count * 10
-        for chunk_id in chunk_ids:
-            task = asyncio.ensure_future(write_chunk_hyperslab(app,
-                                                               chunk_id,
-                                                               dset_json,
-                                                               slices,
-                                                               arr,
-                                                               bucket=bucket))
-            tasks.append(task)
-            if len(tasks) == task_batch_size:
-                await asyncio.gather(*tasks, loop=loop)
-                tasks = []
-        if tasks:
-            await asyncio.gather(*tasks, loop=loop)
     else:
         #
         # Do point PUT
         #
         log.debug(f"num_points: {num_points}")
 
         chunk_dict = {}  # chunk ids to list of points in chunk
@@ -1398,578 +964,813 @@
                         msg += "bounds of the dataset"
                         log.warn(msg)
                         raise HTTPBadRequest(reason=msg)
             chunk_id = getChunkId(dset_id, point, layout)
             # get the pt_indx element from the input data
             value = arr[pt_indx]
             if chunk_id not in chunk_dict:
-                point_list = [point, ]
-                point_data = [value, ]
-                chunk_dict[chunk_id] = {"points": point_list,
-                                        "values": point_data}
+                point_list = [
+                    point,
+                ]
+                point_data = [
+                    value,
+                ]
+                chunk_dict[chunk_id] = {"indices": point_list, "points": point_data}
             else:
                 item = chunk_dict[chunk_id]
-                point_list = item["points"]
+                point_list = item["indices"]
                 point_list.append(point)
-                point_data = item["values"]
+                point_data = item["points"]
                 point_data.append(value)
 
         num_chunks = len(chunk_dict)
         log.debug(f"num_chunks: {num_chunks}")
-        max_chunks = int(config.get('max_chunks_per_request'))
+        max_chunks = int(config.get("max_chunks_per_request", default=1000))
         if num_chunks > max_chunks:
-            msg = "PUT value request too large"
+            msg = f"PUT value request with more than {max_chunks} chunks"
             log.warn(msg)
-            raise HTTPRequestEntityTooLarge(num_chunks, max_chunks)
-        tasks = []
-        for chunk_id in chunk_dict.keys():
-            item = chunk_dict[chunk_id]
-            point_list = item["points"]
-            point_data = item["values"]
-            task = asyncio.ensure_future(write_point_sel(app,
-                                                         chunk_id,
-                                                         dset_json,
-                                                         point_list,
-                                                         point_data,
-                                                         bucket=bucket))
-            tasks.append(task)
-        await asyncio.gather(*tasks, loop=loop)
+
+        chunk_ids = list(chunk_dict.keys())
+        chunk_ids.sort()
+
+        crawler = ChunkCrawler(
+            app,
+            chunk_ids,
+            dset_json=dset_json,
+            bucket=bucket,
+            points=chunk_dict,
+            action="write_point_sel",
+        )
+        await crawler.crawl()
+
+        crawler_status = crawler.get_status()
+
+    if crawler_status == 400:
+        log.info(f"doWriteSelection raising BadRequest error:  {crawler_status}")
+        raise HTTPBadRequest()
+    if crawler_status not in (200, 201):
+        log.info(
+            f"doWriteSelection raising HTTPInternalServerError for status:  {crawler_status}"
+        )
+        raise HTTPInternalServerError()
+
+    # write successful
 
     resp_json = {}
     resp = await jsonResponse(request, resp_json)
     return resp
 
 
-def get_hrefs(request, dset_json):
-    """
-    Convience function to set up hrefs for GET
-    """
-    hrefs = []
-    dset_id = dset_json["id"]
-    dset_uri = f"/datasets/{dset_id}"
-    self_uri = f"{dset_uri}/value"
-    hrefs.append({'rel': 'self', 'href': getHref(request, self_uri)})
-    root_uri = '/groups/' + dset_json["root"]
-    hrefs.append({'rel': 'root', 'href': getHref(request, root_uri)})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
-    hrefs.append({'rel': 'owner', 'href': getHref(request, dset_uri)})
-    return hrefs
-
-
 async def GET_Value(request):
     """
     Handler for GET /<dset_uuid>/value request
     """
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
     if not dset_id:
         msg = "Missing dataset id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(dset_id, "Dataset"):
         msg = f"Invalid dataset id: {dset_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     bucket = getBucketForDomain(domain)
 
     # get state for dataset from DN.
     dset_json = await getObjectJson(app, dset_id, bucket=bucket)
+    type_json = dset_json["type"]
+    dset_dtype = createDataType(type_json)
 
-    datashape = dset_json["shape"]
-    if datashape["class"] == 'H5S_NULL':
+    if isNullSpace(dset_json):
         msg = "Null space datasets can not be used as target for GET value"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
-    dims = getShapeDims(datashape)  # throws 400 for HS_NULL dsets
-    maxdims = getDsetMaxDims(dset_json)
+    datashape = dset_json["shape"]
+    dims = getShapeDims(datashape)
+    log.debug(f"dset shape: {dims}")
     rank = len(dims)
+
     layout = getChunkLayout(dset_json)
     log.debug(f"chunk layout: {layout}")
-    if "shm_name" in params and params["shm_name"]:
-        shm_name = params["shm_name"]
-    else:
-        shm_name = None
 
     await validateAction(app, domain, dset_id, username, "read")
 
-    # refetch the dims if the dataset is extensible and requestor hasn't
-    # provided an explicit region
-    if isExtensible(dims, maxdims) and "select" not in params:
-        kwargs = {"bucket": bucket, "refresh": True}
-        dset_json = await getObjectJson(app, dset_id, **kwargs)
-        dims = getShapeDims(dset_json["shape"])
-
-    slices = None  # selection for read
+    # Get query parameter for selection
+    select = params.get("select")
+    if select:
+        log.debug(f"select query param: {select}")
+    slices = await get_slices(app, select, dset_json, bucket=bucket)
+    log.debug(f"GET Value selection: {slices}")
 
-    # Get query parameter for selection 
-    if "select" in params:
-        select = params["select"]
-    else:
-        select = None
-    if isExtensible and select:
+    limit = 0
+    if "Limit" in params:
         try:
-            slices = getSelectionList(select, dims)
+            limit = int(params["Limit"])
+            log.debug(f"limit: {limit}")
         except ValueError:
-            # exception might be due to us having stale version of dims,
-            # so use refresh
-            kwargs = {"bucket": bucket, "refresh": True}
-            dset_json = await getObjectJson(app, dset_id, **kwargs)
-            dims = getShapeDims(dset_json["shape"])
-            slices = None  # retry below
+            msg = "Invalid Limit query param"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
 
-    if slices is None:
+    if "ignore_nan" in params and params["ignore_nan"]:
+        ignore_nan = True
+    else:
+        ignore_nan = False
+    log.debug(f"ignore nan: {ignore_nan}")
+
+    query = params.get("query")
+    if query:
+        log.debug(f"got query: {query}")
         try:
-            slices = getSelectionList(select, dims)
-        except ValueError as ve:
-            msg = str(ve)
+            parser = BooleanParser(query)
+        except Exception:
+            msg = f"query: {query} is not valid"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
 
-    log.debug(f"GET Value selection: {slices}")
+        field_names = set(dset_dtype.names)
+        variables = parser.getVariables()
+        for variable in variables:
+            if variable not in field_names:
+                msg = f"query variable {variable} not valid"
+                log.warn(msg)
+                raise HTTPBadRequest(reason=msg)
 
-    np_shape = getSelectionShape(slices)
-    log.debug("selection shape:" + str(np_shape))
+    response_type = getAcceptType(request)
 
-    npoints = getNumElements(np_shape)
-    log.debug(f"selection num elements: {npoints}")
+    if response_type == "binary" and use_http_streaming(request, rank):
+        stream_pagination = True
+        log.debug("use stream_pagination")
+    else:
+        stream_pagination = False
+        log.debug("no stream_pagination")
 
-    num_chunks = getNumChunks(slices, layout)
-    log.debug(f"num_chunks: {num_chunks}")
+    # for non query requests with non-variable types we can fetch
+    # the expected response bytes length now
+    item_size = getItemSize(type_json)
+    log.debug(f"item size: {item_size}")
 
-    max_chunks = int(config.get('max_chunks_per_request'))
-    if num_chunks > max_chunks:
+    # get the shape of the response array
+    np_shape = getSelectionShape(slices)
+    log.debug(f"selection shape: {np_shape}")
+
+    # check that the array size is reasonable
+    request_size = math.prod(np_shape)
+    if item_size == "H5T_VARIABLE":
+        request_size *= VARIABLE_AVG_ITEM_SIZE  # random guess of avg item_size
+    else:
+        request_size *= item_size
+    log.debug(f"request_size: {request_size}")
+    max_request_size = int(config.get("max_request_size"))
+    if isAWSLambda(request):
+        # reduce max size to account for hex_encoding and other JSON content
+        max_request_size -= 1000
+        max_request_size /= 2
+    if request_size >= max_request_size and not stream_pagination:
         msg = "GET value request too large"
         log.warn(msg)
-        raise HTTPRequestEntityTooLarge(num_chunks, max_chunks)
-
-    chunk_ids = getChunkIds(dset_id, slices, layout)
-    # Get information about where chunks are located
-    #   Will be None except for H5D_CHUNKED_REF_INDIRECT type
-    chunkinfo = await getChunkInfoMap(app,
-                                      dset_id,
-                                      dset_json,
-                                      chunk_ids,
-                                      bucket=bucket)
-    log.debug(f"chunkinfo_map: {chunkinfo}")
-
-    if request.method == "OPTIONS":
-        # skip doing any big data load for options request
-        resp = await jsonResponse(request,  None)
-    elif "query" in params:
-        if rank > 1:
-            msg = "Query string is not supported for multidimensional arrays"
-            log.warn(msg)
-            raise HTTPBadRequest(reason=msg)
-        try:
-            resp = await doQueryRead(request,
-                                     chunk_ids,
-                                     dset_json,
-                                     slices,
-                                     bucket=bucket)
-        except CancelledError as ce:
-            log.warn(f"Cancelled error on query read: {ce}")
-            # TBD: what do return if client cancels
-            resp = await jsonResponse(request, None)
+        raise HTTPRequestEntityTooLarge(max_request_size, request_size)
+    if item_size != "H5T_VARIABLE" and not query:
+        # this is the exact number of bytes to be returned
+        content_length = request_size
     else:
-        try:
-            resp = await doHyperSlabRead(request,
-                                         chunk_ids,
-                                         dset_json,
-                                         slices,
-                                         chunk_map=chunkinfo,
-                                         bucket=bucket,
-                                         shm_name=shm_name)
-        except CancelledError as ce:
-            log.warn(f"Cancelled error on hyperslab read: {ce}")
-            # TBD: what do return if client cancels
-            resp = await jsonResponse(request, None)
-    log.response(request, resp=resp)
-    return resp
+        content_length = None
 
+    resp_json = {"status": 200}  # will over-write if there's a problem
+    # write response
+    try:
+        resp = StreamResponse()
+        if config.get("http_compression"):
+            log.debug("enabling http_compression")
+            resp.enable_compression()
+        if response_type == "binary":
+            resp.headers["Content-Type"] = "application/octet-stream"
+            if content_length is None:
+                log.debug("content_length could not be determined")
+            else:
+                resp.content_length = content_length
+        else:
+            resp.headers["Content-Type"] = "application/json"
+        log.debug("prepare request")
+        await resp.prepare(request)
+        arr = None  # will be set based on returned data
+
+        if stream_pagination:
+            # example
+            # get binary data a page at a time and write back to response
+            if item_size == "H5T_VARIABLE":
+                page_item_size = VARIABLE_AVG_ITEM_SIZE  # random guess of avg item_size
+            else:
+                page_item_size = item_size
+            pages = getSelectionPagination(
+                slices, dims, page_item_size, max_request_size
+            )
+            log.debug(f"getSelectionPagination returned: {len(pages)} pages")
+            bytes_streamed = 0
+            try:
+                for page_number in range(len(pages)):
+                    page = pages[page_number]
+                    msg = f"streaming response data for page: {page_number+1} "
+                    msg += f"of {len(pages)}, selection: {page}"
+                    log.info(msg)
+
+                    arr = await getSelectionData(
+                        app,
+                        dset_id,
+                        dset_json,
+                        page,
+                        query=query,
+                        bucket=bucket,
+                        limit=limit,
+                        method=request.method,
+                    )
+
+                    if arr is None or math.prod(arr.shape) == 0:
+                        log.warn(f"no data returend for streaming page: {page_number}")
+                        continue
+
+                    log.debug("preparing binary response")
+                    output_data = arrayToBytes(arr)
+                    log.debug(f"got {len(output_data)} bytes for resp")
+                    bytes_streamed += len(output_data)
+                    log.debug("write request")
+                    await resp.write(output_data)
+
+                    if query and limit > 0:
+                        query_rows = arr.shape[0]
+                        log.debug(
+                            f"streaming page {page_number} returned {query_rows} rows"
+                        )
+                        limit -= query_rows
+                        if limit <= 0:
+                            log.debug("skipping remaining pages, query limit reached")
+                            break
+
+            except HTTPException as he:
+                # close the response stream
+                log.error(f"got {type(he)} exception doing getSelectionData: {he}")
+                resp_json["status"] = he.status_code
+                # can't raise a HTTPException here since write is in progress
+                #
+            finally:
+                msg = f"streaming data for {len(pages)} pages complete, "
+                msg += f"{bytes_streamed} bytes written"
+                log.info(msg)
 
-async def doQueryRead(request, chunk_ids, dset_json, slices, bucket=None):
-    """ query read utility function """
-    app = request.app
-    params = request.rel_url.query
-    query = params["query"]
-    log.info(f"Query request: {query}")
-    loop = asyncio.get_event_loop()
-
-    dset_id = dset_json["id"]
-    type_json = dset_json["type"]
-    item_size = getItemSize(type_json)
+                await resp.write_eof()
+                return resp
 
-    log.debug(f"item size: {item_size}")
+        #
+        # non-paginated response
+        #
 
-    limit = 0
-    if "Limit" in params:
         try:
-            limit = int(params["Limit"])
-        except ValueError:
-            msg = "Invalid Limit query param"
-            log.warn(msg)
-            raise HTTPBadRequest(reason=msg)
+            arr = await getSelectionData(
+                app,
+                dset_id,
+                dset_json,
+                slices,
+                query=query,
+                bucket=bucket,
+                limit=limit,
+                method=request.method,
+            )
+        except HTTPException as he:
+            # close the response stream
+            log.error(f"got {type(he)} exception doing getSelectionData: {he}")
+            resp_json["status"] = he.status_code
+            # can't raise a HTTPException here since write is in progress
+
+        if arr is None:
+            # no array (OPTION request?)  Return empty json response
+            log.warn("got None response from getSelectionData")
+
+        elif not isinstance(arr, np.ndarray):
+            msg = f"GET_Value - Expected ndarray but got: {type(arr)}"
+            resp_json["status"] = 500
+        elif response_type == "binary":
+            if resp_json["status"] != 200:
+                # write json with status_code
+                # resp_json = resp_json.encode('utf-8')
+                # await resp.write(resp_json)
+                log.warn(f"GET Value - got error status: {resp_json['status']}")
+            else:
+                log.debug("preparing binary response")
+                output_data = arrayToBytes(arr)
+                log.debug(f"got {len(output_data)} bytes for resp")
+                log.debug("write request")
+                await resp.write(output_data)
+        else:
+            # return json
+            log.debug("GET Value - returning JSON data")
+            params = request.rel_url.query
+            if "reduce_dim" in params and params["reduce_dim"]:
+                arr = squeezeArray(arr)
+
+            data = arr.tolist()
+            json_data = bytesArrayToList(data)
+
+            datashape = dset_json["shape"]
+
+            if datashape["class"] == "H5S_SCALAR":
+                # convert array response to value
+                resp_json["value"] = json_data[0]
+            else:
+                resp_json["value"] = json_data
+            resp_json["hrefs"] = get_hrefs(request, dset_json)
+            resp_body = await jsonResponse(
+                resp, resp_json, ignore_nan=ignore_nan, body_only=True
+            )
+            log.debug(f"jsonResponse returned: {resp_body}")
+            resp_body = resp_body.encode("utf-8")
+            await resp.write(resp_body)
+        await resp.write_eof()
+    except Exception as e:
+        log.error(f"{type(e)} Exception during data write: {e}")
+        import traceback
+
+        tb = traceback.format_exc()
+        print("traceback:", tb)
+        raise HTTPInternalServerError()
 
-    tasks = []
-    node_count = getNodeCount(app)
-    if node_count == 0:
-        log.warn("query read request with no active dn nodes")
-        raise HTTPServiceUnavailable()
-    chunk_index = 0
-    resp_index = []
-    resp_value = []
-    num_chunks = len(chunk_ids)
-    log.info(f"doQueryRead with {num_chunks} chunks")
-    # Get information about where chunks are located
-    #   Will be None except for H5D_CHUNKED_REF_INDIRECT type
-    chunk_map = await getChunkInfoMap(app,
-                                      dset_id,
-                                      dset_json,
-                                      chunk_ids,
-                                      bucket=bucket)
-    log.debug(f"chunkinfo_map: {chunk_map}")
-
-    while chunk_index < num_chunks:
-        next_chunks = chunk_ids[chunk_index:]
-        chunk_index = num_chunks
-        
-        log.debug(f"doQueryRead - next batch of chunk ids: {next_chunks}")
-        
-        dn_rsp = {}  # dictionary keyed by chunk_id
-        kwargs = {"chunk_map": chunk_map,
-                  "bucket": bucket}
-
-        for chunk_id in next_chunks:
-
-            task = asyncio.ensure_future(read_chunk_query(app,
-                                                          chunk_id,
-                                                          dset_json,
-                                                          slices,
-                                                          query,
-                                                          limit,
-                                                          dn_rsp,
-                                                          **kwargs))
-            tasks.append(task)
-        await asyncio.gather(*tasks, loop=loop)
-
-        for chunk_id in next_chunks:
-            chunk_rsp = dn_rsp[chunk_id]
-            resp_index.extend(chunk_rsp["index"])
-            resp_value.extend(chunk_rsp["value"])
-        # trim response if we're over limit
-        if limit > 0 and len(resp_index) > limit:
-            resp_index = resp_index[0:limit]
-            resp_value = resp_index[0:limit]
-            break  # don't need any more DN queries
-    resp_json = {"index": resp_index, "value": resp_value}
-    resp_json["hrefs"] = get_hrefs(request, dset_json)
-    resp = await jsonResponse(request, resp_json)
     return resp
 
 
-async def doHyperSlabRead(request, chunk_ids, dset_json, slices,
-                          chunk_map=None, bucket=None, shm_name=None):
-    """ hyperslab read utility function """
-    app = request.app
-    loop = asyncio.get_event_loop()
-    log.info(f"doHyperSlabRead - number of chunk_ids: {len(chunk_ids)}")
-    log.debug(f"doHyperSlabRead - chunk_ids: {chunk_ids}")
-    log.debug("headers...")
-    for k in request.headers:
-        v = request.headers[k]
-        log.debug(f"   {k}: {v}")
+async def doReadSelection(
+    app,
+    chunk_ids,
+    dset_json,
+    slices=None,
+    points=None,
+    query=None,
+    query_update=None,
+    chunk_map=None,
+    bucket=None,
+    limit=0,
+):
+    """read selection utility function"""
+    log.info(f"doReadSelection - number of chunk_ids: {len(chunk_ids)}")
+    log.debug(f"doReadSelection - chunk_ids: {chunk_ids}")
 
-    accept_type = getAcceptType(request)
-    
     type_json = dset_json["type"]
     item_size = getItemSize(type_json)
     log.debug(f"item size: {item_size}")
     dset_dtype = createDataType(type_json)  # np datatype
+    if query is None:
+        query_dtype = None
+    else:
+        log.debug(f"query: {query} limit: {limit}")
+        query_dtype = getQueryDtype(dset_dtype)
 
     # create array to hold response data
-    np_shape = getSelectionShape(slices)
-    log.debug(f"selection shape: {np_shape}")
+    arr = None
 
-    # check that the array size is reasonable
-    request_size = np.prod(np_shape)
-    if item_size == 'H5T_VARIABLE':
-        request_size *= 512  # random guess of avg item_size
+    if points is not None:
+        # point selection
+        np_shape = [
+            len(points),
+        ]
+    elif query is not None:
+        # return shape will be determined by number of matches
+        np_shape = None
+    elif slices is not None:
+        log.debug(f"get np_shape for slices: {slices}")
+        np_shape = getSelectionShape(slices)
     else:
-        request_size *= item_size
-    log.debug(f"request_size: {request_size}")
-    max_request_size = int(config.get("max_request_size"))
-    if request_size >= max_request_size:
-        msg = "GET value request too large"
-        log.warn(msg)
-        raise HTTPRequestEntityTooLarge(request_size, max_request_size)
+        log.error("doReadSelection - expected points or slices to be set")
+        raise HTTPInternalServerError()
+    log.debug(f"selection shape: {np_shape}")
 
-    response_type = accept_type  # use JSON or binary per accept value
-    
-    arr = np.zeros(np_shape, dtype=dset_dtype, order='C')
-    tasks = []
-    kwargs = {"chunk_map": chunk_map,
-              "bucket": bucket}
+    if np_shape is not None:
+        # check that the array size is reasonable
+        request_size = math.prod(np_shape)
+        if item_size == "H5T_VARIABLE":
+            request_size *= 512  # random guess of avg item_size
+        else:
+            request_size *= item_size
+            log.debug(f"request_size: {request_size}")
+        max_request_size = int(config.get("max_request_size"))
+        if request_size >= max_request_size:
+            msg = f"Attempting to fetch {request_size} bytes (greater than "
+            msg += f"{max_request_size} limit"
+            log.error(msg)
+            raise HTTPBadRequest(reason=msg)
 
-    for chunk_id in chunk_ids:
-        task = asyncio.ensure_future(read_chunk_hyperslab(app,
-                                                          chunk_id,
-                                                          dset_json,
-                                                          slices,
-                                                          arr,
-                                                          **kwargs))
-        tasks.append(task)
-    await asyncio.gather(*tasks, loop=loop)
+        arr = np.zeros(np_shape, dtype=dset_dtype, order="C")
+        fill_value = getFillValue(dset_json)
+        if fill_value is not None:
+            arr[...] = fill_value
 
-    log.info(f"read_chunk_hyperslab gather complete, arr shape: {arr.shape}")
+    crawler = ChunkCrawler(
+        app,
+        chunk_ids,
+        dset_json=dset_json,
+        chunk_map=chunk_map,
+        bucket=bucket,
+        slices=slices,
+        query=query,
+        query_update=query_update,
+        limit=limit,
+        arr=arr,
+        action="read_chunk_hyperslab",
+    )
+    await crawler.crawl()
+
+    crawler_status = crawler.get_status()
+
+    log.info(f"doReadSelection complete - status:  {crawler_status}")
+    if crawler_status == 400:
+        log.info(f"doReadSelection raising BadRequest error:  {crawler_status}")
+        raise HTTPBadRequest()
+    if crawler_status not in (200, 201):
+        log.info(
+            f"doReadSelection raising HTTPInternalServerError for status:  {crawler_status}"
+        )
+        raise HTTPInternalServerError()
 
-    if shm_name:
-        log.debug(f"attaching to shared memory block: {shm_name}")
-        try:
-            shm = shared_memory.SharedMemory(name=shm_name)
-        except FileNotFoundError:
-            msg = f"no shared memory block with name: {shm_name} found"
-            log.warning(msg)
-            raise HTTPBadRequest(reason=msg)
-        except OSError as oe:
-            msg = f"Unexpected OSError: {oe.errno} attaching to shared memory block"
-            log.error(msg)
-            raise HTTPInternalServerError()
-        buffer = arrayToBytes(arr)
-        num_bytes = len(buffer)
-        if shm.size < num_bytes:
-            msg = f"unable to copy {num_bytes} to shared memory block of size: {shm.size}"
-            log.warning(msg)
-            raise HTTPRequestEntityTooLarge(num_bytes, shm.size)
-
-        # copy array data
-        shm.buf[:num_bytes] = buffer[:]
-        log.debug(f"copied {num_bytes} array data to shared memory name: {shm_name}")
-
-        # close shared memory block
-        # Note - since we are not calling shm.unlink (expecting the 
-        # client to do that), it's likely the resource tracker will complain on
-        # app exit.  This should be fixed in Python 3.9.  See: 
-        # https://bugs.python.org/issue39959
-        shm.close()
-
-        log.debug("GET Value - returning JSON data with shared memory buffer")
-        resp_json = {"shm_name": shm.name, "num_bytes": num_bytes}
-        resp_json["hrefs"] = get_hrefs(request, dset_json)
-        resp = await jsonResponse(request, resp_json)
-        return resp
-        
-    if response_type == "binary":
-        log.debug("preparing binary response")
-        output_data = arrayToBytes(arr)
-        log.debug(f"got {len(output_data)} bytes for resp")
+    if query is not None:
+        # combine chunk responses and return
+        if limit > 0 and crawler._hits > limit:
+            nrows = limit
+        else:
+            nrows = crawler._hits
+        arr = np.empty((nrows,), dtype=query_dtype)
+        start = 0
+        for chunkid in chunk_ids:
+            if chunkid not in chunk_map:
+                continue
+            chunk_item = chunk_map[chunkid]
+            if "query_rsp" not in chunk_item:
+                continue
+            query_rsp = chunk_item["query_rsp"]
+            if len(query_rsp) == 0:
+                continue
+            stop = start + len(query_rsp)
+            if stop > nrows:
+                rsp_stop = len(query_rsp) - (stop - nrows)
+                arr[start:] = query_rsp[0:rsp_stop]
+            else:
+                arr[start:stop] = query_rsp[:]
+            start = stop
+            if start >= nrows:
+                log.debug(f"got {nrows} rows for query, quitting")
+                break
+    return arr
 
-        # write response
-        try:
-            resp = StreamResponse()
-            if config.get("http_compression"):
-                log.debug("enabling http_compression")
-                resp.enable_compression()
-            resp.headers['Content-Type'] = "application/octet-stream"
-            resp.content_length = len(output_data)
-
-            log.debug("prepare request")
-            await resp.prepare(request)
-            log.debug("write request")
-            await resp.write(output_data)
-            log.debug("write_eof")
-            await resp.write_eof()
-        except Exception as e:
-            log.error(f"{type(e)} Exception during binary data write: {e}")
 
+async def getSelectionData(
+    app,
+    dset_id,
+    dset_json,
+    slices=None,
+    points=None,
+    query=None,
+    query_update=None,
+    bucket=None,
+    limit=0,
+    method="GET",
+):
+    """Read selected slices and return numpy array"""
+    log.debug("getSelectionData")
+    if slices is None and points is None:
+        log.error("getSelectionData - expected either slices or points to be set")
+        raise HTTPInternalServerError()
+
+    layout = getChunkLayout(dset_json)
+
+    chunkinfo = {}
+
+    if slices is not None:
+        num_chunks = getNumChunks(slices, layout)
+        log.debug(f"num_chunks: {num_chunks}")
+
+        max_chunks = int(config.get("max_chunks_per_request", default=1000))
+        if num_chunks > max_chunks:
+            msg = f"num_chunks over {max_chunks} limit, but will attempt to fetch with crawler"
+            log.warn(msg)
+
+        chunk_ids = getChunkIds(dset_id, slices, layout)
     else:
-        log.debug("GET Value - returning JSON data")
-        params = request.rel_url.query
-        if "reduce_dim" in params and params["reduce_dim"]:
-            arr = squeezeArray(arr)
-        resp_json = {}
-        data = arr.tolist()
-        params = request.rel_url.query
-        if "ignore_nan" in params and params["ignore_nan"]:
-            ignore_nan = True
-        else:
-            ignore_nan = False
+        # points - already checked it is not None
+        num_points = len(points)
+        chunk_ids = []
+        for pt_indx in range(num_points):
+            point = points[pt_indx]
+            chunk_id = getChunkId(dset_id, point, layout)
+            if chunk_id in chunkinfo:
+                chunk_entry = chunkinfo[chunk_id]
+            else:
+                chunk_entry = {}
+                chunkinfo[chunk_id] = chunk_entry
+                chunk_ids.append(chunk_id)
+            if "points" in chunk_entry:
+                point_list = chunk_entry["points"]
+            else:
+                point_list = []
+                chunk_entry["points"] = point_list
+            if "indices" in chunk_entry:
+                point_index = chunk_entry["indices"]
+            else:
+                point_index = []
+                chunk_entry["indices"] = point_index
 
-        json_data = bytesArrayToList(data)
-        datashape = dset_json["shape"]
+            point_list.append(point)
+            point_index.append(pt_indx)
 
-        if datashape["class"] == 'H5S_SCALAR':
-            # convert array response to value
-            resp_json["value"] = json_data[0]
-        else:
-            resp_json["value"] = json_data
-        resp_json["hrefs"] = get_hrefs(request, dset_json)
-        resp = await jsonResponse(request, resp_json, ignore_nan=ignore_nan)
-    return resp
+    # Get information about where chunks are located
+    #   Will be None except for H5D_CHUNKED_REF_INDIRECT type
+    await getChunkLocations(app, dset_id, dset_json, chunkinfo, chunk_ids, bucket=bucket)
+
+    if slices is None:
+        slices = await get_slices(app, None, dset_json, bucket=bucket)
+
+    if points is None:
+        # get chunk selections for hyperslab select
+        get_chunk_selections(chunkinfo, chunk_ids, slices, dset_json)
+
+    log.debug(f"chunkinfo_map: {chunkinfo}")
+
+    if method == "OPTIONS":
+        # skip doing any big data load for options request
+        return None
+
+    arr = await doReadSelection(
+        app,
+        chunk_ids,
+        dset_json,
+        slices=slices,
+        points=points,
+        query=query,
+        query_update=query_update,
+        limit=limit,
+        chunk_map=chunkinfo,
+        bucket=bucket,
+    )
+
+    return arr
 
 
 async def POST_Value(request):
     """
-    Handler for POST /<dset_uuid>/value request - point selection
+    Handler for POST /<dset_uuid>/value request - point selection or hyperslab read
     """
     log.request(request)
 
     app = request.app
     body = None
 
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
     if not dset_id:
         msg = "Missing dataset id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(dset_id, "Dataset"):
         msg = f"Invalid dataset id: {dset_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
-    log.info(f"POST_VALUE, id: {dset_id}")
+    log.info(f"POST_Value, dataset id: {dset_id}")
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     bucket = getBucketForDomain(domain)
 
     accept_type = getAcceptType(request)
     response_type = accept_type  # will adjust later if binary not possible
 
-    request_type = "json"
-    if "Content-Type" in request.headers:
-        # client should use "application/octet-stream" for binary transfer
-        content_type = request.headers["Content-Type"]
-        if content_type not in EXPECTED_CONTENT_TYPES:
-            msg = f"Unknown content_type: {content_type}"
-            log.warn(msg)
-            raise HTTPBadRequest(reason=msg)
-        if content_type == "application/octet-stream":
-            log.debug("POST value - request_type is binary")
-            request_type = "binary"
-        else:
-            log.debug("POST value - request type is json")
+    params = request.rel_url.query
+    if "ignore_nan" in params and params["ignore_nan"]:
+        ignore_nan = True
+    else:
+        ignore_nan = False
+
+    request_type = getContentType(request)
+    log.debug(f"POST value - request_type is {request_type}")
 
     if not request.has_body:
         msg = "POST Value with no body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     # get  state for dataset from DN.
     dset_json = await getObjectJson(app, dset_id, bucket=bucket)
 
     datashape = dset_json["shape"]
-    if datashape["class"] == 'H5S_NULL':
+    if datashape["class"] == "H5S_NULL":
         msg = "POST value not supported for datasets with NULL shape"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    if datashape["class"] == 'H5S_SCALAR':
+    if datashape["class"] == "H5S_SCALAR":
         msg = "POST value not supported for datasets with SCALAR shape"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     dims = getShapeDims(datashape)
     rank = len(dims)
 
     type_json = dset_json["type"]
     item_size = getItemSize(type_json)
     log.debug(f"item size: {item_size}")
 
     await validateAction(app, domain, dset_id, username, "read")
 
     # read body data
-    num_points = None
-    point_dt = np.dtype('u8')  # use unsigned long for point index
+    slices = None  # this will be set for hyperslab selection
+    points = None  # this will be set for point selection
+    point_dt = np.dtype("u8")  # use unsigned long for point index
     if request_type == "json":
-        body = await request.json()
-        if "points" not in body:
-            msg = "Expected points key in request body"
+        try:
+            body = await request.json()
+        except JSONDecodeError:
+            msg = "Unable to load JSON body"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-        points = body["points"]
-        if not isinstance(points, list):
-            msg = "POST Value expected list of points"
+        if "points" in body:
+            points_list = body["points"]
+            if not isinstance(points_list, list):
+                msg = "POST Value expected list of points"
+                log.warn(msg)
+                raise HTTPBadRequest(reason=msg)
+            points = np.asarray(points_list, dtype=point_dt)
+            log.debug(f"get {len(points)} points from json request")
+        elif "select" in body:
+            select = body["select"]
+            log.debug(f"select: {select}")
+            slices = await get_slices(app, select, dset_json, bucket=bucket)
+            log.debug(f"got slices: {slices}")
+        else:
+            msg = "Expected points or select key in request body"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-        num_points = len(points)
-
     else:
         # read binary data
         binary_data = await request_read(request)
         if len(binary_data) != request.content_length:
             msg = f"Read {len(binary_data)} bytes, expecting: "
             msg += f"{request.content_length}"
-            log.error(msg)
-            raise HTTPInternalServerError()
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
         if request.content_length % point_dt.itemsize != 0:
             msg = f"Content length: {request.content_length} not "
             msg += f"divisible by element size: {item_size}"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         num_points = request.content_length // point_dt.itemsize
-        log.debug(f"got {num_points} num_points")
         points = np.fromstring(binary_data, dtype=point_dt)
+        # reshape the data based on the rank (num_points x rank)
         if rank > 1:
-            if num_points % rank != 0:
-                msg = "Number of points is not consistent with dataset rank"
+            if len(points) % rank != 0:
+                msg = "Number of point values is not consistent with dataset rank"
                 log.warn(msg)
                 raise HTTPBadRequest(reason=msg)
-            num_points //= rank
+            num_points = len(points) // rank
             # conform to point index shape
             points = points.reshape((num_points, rank))
 
-    kwargs = {"bucket": bucket}
-    arr_rsp = await getPointData(app, dset_id, dset_json, points, **kwargs)
+    if points is not None:
+        log.debug(f"got {len(points)} num_points")
 
-    log.debug(f"arr shape: {arr_rsp.shape}")
+    # get expected content_length
+    item_size = getItemSize(type_json)
+    log.debug(f"item size: {item_size}")
 
-    if response_type == "binary":
-        output_data = arr_rsp.tobytes()
-        msg = f"POST Value - returning {len(output_data)} bytes binary data"
-        log.debug(msg)
+    # get the shape of the response array
+    if slices:
+        # hyperslab post
+        np_shape = getSelectionShape(slices)
+    else:
+        # point selection
+        np_shape = [
+            len(points),
+        ]
 
-        # write response
-        try:
-            resp = StreamResponse()
-            if config.get("http_compression"):
-                log.debug("enabling http_compression")
-                resp.enable_compression()
-            resp.headers['Content-Type'] = "application/octet-stream"
-            resp.content_length = len(output_data)
-            await resp.prepare(request)
-            await resp.write(output_data)
-            await resp.write_eof()
-        except Exception as e:
-            log.error(f"Exception during binary data write: {e}")
+    log.debug(f"selection shape: {np_shape}")
+
+    # check that the array size is reasonable
+    request_size = np.prod(np_shape)
+    if item_size == "H5T_VARIABLE":
+        request_size *= 512  # random guess of avg item_size
+    else:
+        request_size *= item_size
+    log.debug(f"request_size: {request_size}")
+    max_request_size = int(config.get("max_request_size"))
+    if request_size >= max_request_size:
+        msg = "POST value request too large"
+        log.warn(msg)
+        raise HTTPRequestEntityTooLarge(max_request_size, request_size)
+    if item_size != "H5T_VARIABLE":
+        # this is the exact number of bytes to be returned
+        content_length = request_size
     else:
-        log.debug("POST Value - returning JSON data")
-        rsp_json = {}
-        data = arr_rsp.tolist()
-        log.debug(f"got rsp data {len(data)} points")
-        json_data = bytesArrayToList(data)
-        rsp_json["value"] = json_data
-        resp = await jsonResponse(request, rsp_json)
+        # don't put content_length in response headers
+        content_length = None
+
+    if points is not None:
+        # validate content of points input array
+        for i in range(len(points)):
+            point = points[i]
+            if rank == 1:
+                if point < 0 or point >= dims[0]:
+                    msg = f"POST Value point: {point} is not within the bounds "
+                    msg += "of the dataset"
+                    log.warn(msg)
+                    raise HTTPBadRequest(reason=msg)
+            else:
+                if len(point) != rank:
+                    msg = "POST Value point value did not match dataset rank"
+                    log.warn(msg)
+                    raise HTTPBadRequest(reason=msg)
+                for i in range(rank):
+                    if point[i] < 0 or point[i] >= dims[i]:
+                        msg = f"POST Value point: {point} is not within the "
+                        msg += "bounds of the dataset"
+                        log.warn(msg)
+                        raise HTTPBadRequest(reason=msg)
+
+    # write response
+    resp = StreamResponse()
+    try:
+        if config.get("http_compression"):
+            log.debug("enabling http_compression")
+            resp.enable_compression()
+        if response_type == "binary":
+            resp.headers["Content-Type"] = "application/octet-stream"
+            if content_length is None:
+                log.debug("content_length could not be determined")
+            else:
+                resp.content_length = content_length
+        else:
+            resp.headers["Content-Type"] = "application/json"
+        log.debug("prepare request...")
+        await resp.prepare(request)
+
+        kwargs = {"bucket": bucket}
+        if slices is not None:
+            kwargs["slices"] = slices
+        if points is not None:
+            kwargs["points"] = points
+        log.debug(f"getSelectionData kwargs: {kwargs}")
+
+        arr_rsp = await getSelectionData(app, dset_id, dset_json, **kwargs)
+        if not isinstance(arr_rsp, np.ndarray):
+            msg = f"POST_Value - Expected ndarray but got: {type(arr_rsp)}"
+            log.error(msg)
+            raise ValueError(msg)
+
+        log.debug(f"arr shape: {arr_rsp.shape}")
+        if response_type == "binary":
+            log.debug("preparing binary response")
+            output_data = arr_rsp.tobytes()
+            msg = f"POST Value - returning {len(output_data)} bytes binary data"
+            log.debug(msg)
+            await resp.write(output_data)
+        else:
+            log.debug("POST Value - returning JSON data")
+            resp_json = {}
+            data = arr_rsp.tolist()
+            log.debug(f"got rsp data {len(data)} points")
+            json_data = bytesArrayToList(data)
+            resp_json["value"] = json_data
+            resp_json["hrefs"] = get_hrefs(request, dset_json)
+            resp_body = await jsonResponse(
+                resp, resp_json, ignore_nan=ignore_nan, body_only=True
+            )
+            log.debug(f"jsonResponse returned: {resp_body}")
+            resp_body = resp_body.encode("utf-8")
+            await resp.write(resp_body)
+    except Exception as e:
+        log.error(f"{type(e)} Exception during response write")
+        import traceback
+
+        tb = traceback.format_exc()
+        print("traceback:", tb)
+
+    # finalize response
+    await resp.write_eof()
+
     log.response(request, resp=resp)
     return resp
```

### Comparing `hsds-0.7.0b11/hsds/config.py` & `hsds-0.8.0/hsds/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 import os
 import sys
 import yaml
+from pkg_resources import resource_filename
 
 cfg = {}
 
 
 def eprint(*args, **kwargs):
     print(*args, file=sys.stderr, **kwargs)
 
@@ -23,84 +24,78 @@
 def debug(*args, **kwargs):
     # can't use log.debug since that calls back to cfg
     if "LOG_LEVEL" in os.environ and os.environ["LOG_LEVEL"] == "DEBUG":
         print("DEBUG>", *args, **kwargs)
 
 
 def _has_unit(cfgval):
-    """ return True if val has unit char at end of string,
-        otherwise return False
+    """return True if val has unit char at end of string,
+    otherwise return False
     """
     if isinstance(cfgval, str):
-        if len(cfgval) > 1 and cfgval[-1] in ('g', 'm', 'k'):
+        if len(cfgval) > 1 and cfgval[-1] in ("g", "m", "k"):
             if cfgval[:-1].isdigit():
                 return True
     return False
 
 
 def getCmdLineArg(x):
     # return value of command-line option
     # use "--x=val" to set option 'x' to 'val'
     # use "--x" for boolean flags
-    option = '--'+x+'='
+    option = "--" + x + "="
     for i in range(1, len(sys.argv)):
         arg = sys.argv[i]
-        if arg == '--'+x:
+        if arg == "--" + x:
             # boolean flag
             debug(f"got cmd line flag for {x}")
             return True
         elif arg.startswith(option):
             # found an override
-            override = arg[len(option):]  # return text after option string
+            nlen = len(option)
+            override = arg[nlen:]  # return text after option string
             debug(f"got cmd line override for {x}")
             return override
     return None
 
 
 def _load_cfg():
     # load config yaml
     yml_file = None
     config_dirs = []
     # check if there is a command line option for config directory
     config_dir = getCmdLineArg("config-dir")
     # check cmdLineArg with underline
     if not config_dir:
         config_dir = getCmdLineArg("config_dir")
-    
+
     if config_dir:
         config_dirs.append(config_dir)
     if not config_dirs and "CONFIG_DIR" in os.environ:
         config_dirs.append(os.environ["CONFIG_DIR"])
         debug(f"got environment override for config-dir: {config_dirs[0]}")
     if not config_dirs:
         debug("set default location for config dirs")
         config_dirs = ["./", "/config", "/etc/hsds/"]  # default locations
     for config_dir in config_dirs:
         file_name = os.path.join(config_dir, "config.yml")
         debug("checking config path:", file_name)
         if os.path.isfile(file_name):
             yml_file = file_name
             break
-        file_name = os.path.join(config_dir, "config.yaml") # Check for alt extension
+        # Check for alt extension
+        file_name = os.path.join(config_dir, "config.yaml")
         debug("checking config path:", file_name)
         if os.path.isfile(file_name):
             yml_file = file_name
             break
     if not yml_file:
         # use yaml file embedded in package
-        # TBD: is there a more elegant way to get the directory
-        # where config.yml gets placed in the setup data_files list?
-        package_dir = os.path.dirname(__file__)
-        while package_dir != '/':
-            s = os.path.join(package_dir, "config/config.yml")
-            if os.path.isfile(s):
-                yml_file = s
-                break
-            package_dir = os.path.dirname(package_dir)
-            
+        yml_file = resource_filename("admin", "config/config.yml")
+
         if not yml_file:
             raise FileNotFoundError("unable to load config.yml")
     debug(f"_load_cfg with '{yml_file}'")
     try:
         with open(yml_file, "r") as f:
             yml_config = yaml.safe_load(f)
     except yaml.scanner.ScannerError as se:
@@ -155,30 +150,30 @@
                     # raise KeyError(msg)
             cfgval = override  # replace the yml value
 
         if _has_unit(cfgval):
             # convert values like 512m to corresponding integer
             u = cfgval[-1]
             n = int(cfgval[:-1])
-            if u == 'k':
+            if u == "k":
                 cfgval = n * 1024
-            elif u == 'm':
-                cfgval = n * 1024*1024
-            elif u == 'g':
-                cfgval = n * 1024*1024*1024
+            elif u == "m":
+                cfgval = n * 1024 * 1024
+            elif u == "g":
+                cfgval = n * 1024 * 1024 * 1024
             else:
                 raise ValueError("Unexpected unit char")
         cfg[x] = cfgval
 
 
 def get(x, default=None):
-    """ get x if found in config
-        otherwise return default
+    """get x if found in config
+    otherwise return default
     """
     if not cfg:
         _load_cfg()
     if x not in cfg:
         if default is not None:
             cfg[x] = default
         else:
-            raise KeyError(f"config value {x} not found")
+            return None
     return cfg[x]
```

### Comparing `hsds-0.7.0b11/hsds/ctype_dn.py` & `hsds-0.8.0/hsds/ctype_dn.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # data node of hsds cluster
 #
+
 import time
 
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPNotFound
 from aiohttp.web_exceptions import HTTPInternalServerError
 from aiohttp.web import json_response
 
 from .util.idUtil import isValidUuid, validateUuid
 from .datanode_lib import get_obj_id, get_metadata_obj, save_metadata_obj
 from .datanode_lib import delete_metadata_obj, check_metadata_obj
 from . import hsds_logger as log
 
 
 async def GET_Datatype(request):
-    """HTTP GET method to return JSON for /groups/
-    """
+    """HTTP GET method to return JSON for /groups/"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
     ctype_id = get_obj_id(request)
 
     if not isValidUuid(ctype_id, obj_class="type"):
         log.error(f"Unexpected type_id: {ctype_id}")
@@ -55,15 +55,15 @@
 
     resp = json_response(resp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def POST_Datatype(request):
-    """ Handler for POST /datatypes"""
+    """Handler for POST /datatypes"""
     log.info("Post_Datatype")
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
     if not request.has_body:
         msg = "POST_Datatype with no body"
@@ -110,20 +110,22 @@
     type_json = body["type"]
 
     # ok - all set, create committed type obj
     now = time.time()
 
     log.info(f"POST_datatype, typejson: {type_json}")
 
-    ctype_json = {"id": ctype_id,
-                  "root": root_id,
-                  "created": now,
-                  "lastModified": now,
-                  "type": type_json,
-                  "attributes": {}}
+    ctype_json = {
+        "id": ctype_id,
+        "root": root_id,
+        "created": now,
+        "lastModified": now,
+        "type": type_json,
+        "attributes": {},
+    }
 
     kwargs = {"bucket": bucket, "notify": True, "flush": True}
     await save_metadata_obj(app, ctype_id, ctype_json, **kwargs)
 
     resp_json = {}
     resp_json["id"] = ctype_id
     resp_json["root"] = root_id
@@ -133,27 +135,31 @@
     resp = json_response(resp_json, status=201)
 
     log.response(request, resp=resp)
     return resp
 
 
 async def DELETE_Datatype(request):
-    """HTTP DELETE method for datatype
-    """
+    """HTTP DELETE method for datatype"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
     ctype_id = get_obj_id(request)
     log.info(f"DELETE ctype: {ctype_id}")
 
     if "bucket" in params:
         bucket = params["bucket"]
     else:
-        bucket = None
+        bucket = app["bucket_name"]
+
+    if not bucket:
+        msg = "DELETE_Datatype - bucket not set"
+        log.error(msg)
+        raise HTTPBadRequest(reason=msg)
 
     # verify the id  exist
     obj_found = await check_metadata_obj(app, ctype_id)
     if not obj_found:
         log.warn(f"Delete on non-existent obj: {ctype_id}")
         raise HTTPNotFound
```

### Comparing `hsds-0.7.0b11/hsds/ctype_sn.py` & `hsds-0.8.0/hsds/ctype_sn.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 ##############################################################################
 #
 # service node of hsds cluster
 # handles datatypes requests
 #
 
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPGone
-
-from .util.httpUtil import http_post, http_put, http_delete, getHref
+from json import JSONDecodeError
+from .util.httpUtil import http_post, http_put, http_delete, getHref, respJsonAssemble
 from .util.httpUtil import jsonResponse
 from .util.idUtil import isValidUuid, getDataNodeUrl, createObjId
 from .util.authUtil import getUserPasswordFromRequest, aclCheck
 from .util.authUtil import validateUserPassword
-from .util.domainUtil import getDomainFromRequest, isValidDomain
+from .util.domainUtil import getDomainFromRequest, getPathForDomain, isValidDomain
 from .util.domainUtil import getBucketForDomain, verifyRoot
 from .util.hdf5dtype import validateTypeItem, getBaseTypeJson
 from .servicenode_lib import getDomainJson, getObjectJson, validateAction
 from .servicenode_lib import getObjectIdByPath, getPathForObjectId
 from . import hsds_logger as log
 
 
@@ -34,15 +34,15 @@
     log.request(request)
     app = request.app
     params = request.rel_url.query
     include_attrs = False
 
     h5path = None
     getAlias = False
-    ctype_id = request.match_info.get('id')
+    ctype_id = request.match_info.get("id")
     if not ctype_id and "h5path" not in params:
         msg = "Missing type id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if "include_attrs" in params and params["include_attrs"]:
         include_attrs = True
 
@@ -64,22 +64,22 @@
                 raise HTTPBadRequest(reason=msg)
         if "h5path" not in params:
             msg = "Expecting either ctype id or h5path url param"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
 
         h5path = params["h5path"]
-        if h5path[0] != '/' and group_id is None:
+        if h5path[0] != "/" and group_id is None:
             msg = "h5paths must be absolute"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         log.info(f"GET_Datatype, h5path: {h5path}")
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
@@ -90,50 +90,50 @@
     if h5path:
         domain_json = await getDomainJson(app, domain)
         verifyRoot(domain_json)
 
         if group_id is None:
             group_id = domain_json["root"]
         # throws 404 if not found
-        kwargs = {"bucket": bucket}
-        ctype_id = await getObjectIdByPath(app, group_id, h5path, **kwargs)
+        kwargs = {"bucket": bucket, "domain": domain}
+        ctype_id, domain, _ = await getObjectIdByPath(app, group_id, h5path, **kwargs)
         if not isValidUuid(ctype_id, "Datatype"):
             msg = f"No datatype exist with the path: {h5path}"
             log.warn(msg)
             raise HTTPGone()
         log.info(f"got ctype_id: {ctype_id} from h5path: {h5path}")
 
     await validateAction(app, domain, ctype_id, username, "read")
 
     # get authoritative state for ctype from DN
     #   (even if it's in the meta_cache)
-    kwargs = {"bucket": bucket,
-              "refresh": True,
-              "include_attrs": include_attrs}
+    kwargs = {"bucket": bucket, "refresh": True, "include_attrs": include_attrs}
+
     type_json = await getObjectJson(app, ctype_id, **kwargs)
-    type_json["domain"] = domain
+    type_json = respJsonAssemble(type_json, params, ctype_id)
+    type_json["domain"] = getPathForDomain(domain)
 
     if getAlias:
         root_id = type_json["root"]
         alias = []
-        idpath_map = {root_id: '/'}
+        idpath_map = {root_id: "/"}
         kwargs = {"bucket": bucket, "tgt_id": ctype_id}
         h5path = await getPathForObjectId(app, root_id, idpath_map, **kwargs)
         if h5path:
             alias.append(h5path)
         type_json["alias"] = alias
 
     hrefs = []
-    ctype_uri = '/datatypes/'+ctype_id
-    hrefs.append({'rel': 'self', 'href': getHref(request, ctype_uri)})
-    root_uri = '/groups/' + type_json["root"]
-    hrefs.append({'rel': 'root', 'href': getHref(request, root_uri)})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
-    href = getHref(request, ctype_uri+'/attributes')
-    hrefs.append({'rel': 'attributes', 'href': href})
+    ctype_uri = "/datatypes/" + ctype_id
+    hrefs.append({"rel": "self", "href": getHref(request, ctype_uri)})
+    root_uri = "/groups/" + type_json["root"]
+    hrefs.append({"rel": "root", "href": getHref(request, root_uri)})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
+    href = getHref(request, ctype_uri + "/attributes")
+    hrefs.append({"rel": "attributes", "href": href})
     type_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, type_json)
     log.response(request, resp=resp)
     return resp
 
 
@@ -147,15 +147,20 @@
     await validateUserPassword(app, username, pswd)
 
     if not request.has_body:
         msg = "POST Datatype with no body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
-    body = await request.json()
+    try:
+        body = await request.json()
+    except JSONDecodeError:
+        msg = "Unable to load JSON body"
+        log.warn(msg)
+        raise HTTPBadRequest(reason=msg)
     if "type" not in body:
         msg = "POST Datatype has no type key in body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     datatype = body["type"]
     if isinstance(datatype, str):
         try:
@@ -239,17 +244,17 @@
     return resp
 
 
 async def DELETE_Datatype(request):
     """HTTP method to delete a committed type resource"""
     log.request(request)
     app = request.app
-    meta_cache = app['meta_cache']
+    meta_cache = app["meta_cache"]
 
-    ctype_id = request.match_info.get('id')
+    ctype_id = request.match_info.get("id")
     if not ctype_id:
         msg = "Missing committed type id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(ctype_id, "Type"):
         msg = f"Invalid committed type id: {ctype_id}"
         log.warn(msg)
```

### Comparing `hsds-0.7.0b11/hsds/datanode.py` & `hsds-0.8.0/hsds/datanode.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # data node of hsds cluster
 #
+
 import asyncio
 import time
+import traceback
 from aiohttp.web import run_app
 
 from . import config
 from .util.lruCache import LruCache
 from .util.idUtil import isValidUuid, isSchema2Id, getCollectionForId
 from .util.idUtil import isRootObjId
 from .util.httpUtil import isUnixDomainUrl, bindToSocket, getPortFromUrl
-from .util.httpUtil import release_http_client
-from . util.storUtil import setBloscThreads, getBloscThreads
-from .basenode import healthCheck, baseInit, preStop
-# from .util.httpUtil import release_http_client
+from .util.httpUtil import jsonResponse, release_http_client
+from .util.storUtil import setBloscThreads, getBloscThreads
+from .basenode import healthCheck, baseInit
 from . import hsds_logger as log
 from .domain_dn import GET_Domain, PUT_Domain, DELETE_Domain, PUT_ACL
 from .group_dn import GET_Group, POST_Group, DELETE_Group, PUT_Group
 from .group_dn import POST_Root
 from .link_dn import GET_Links, GET_Link, PUT_Link, DELETE_Link
 from .attr_dn import GET_Attributes, GET_Attribute, PUT_Attribute
 from .attr_dn import DELETE_Attribute
@@ -40,72 +41,64 @@
 from .async_lib import scanRoot, removeKeys
 from aiohttp.web_exceptions import HTTPNotFound, HTTPInternalServerError
 from aiohttp.web_exceptions import HTTPForbidden, HTTPBadRequest
 
 
 async def init():
     """Intitialize application and return app object"""
-    app = baseInit('dn')
+    app = baseInit("dn")
 
     #
     # call app.router.add_get() here to add node-specific routes
     #
-    app.router.add_route('GET', '/domains', GET_Domain)
-    app.router.add_route('PUT', '/domains', PUT_Domain)
-    app.router.add_route('DELETE', '/domains', DELETE_Domain)
-    app.router.add_route('PUT', '/acls/{username}', PUT_ACL)
-    app.router.add_route('GET', '/groups/{id}', GET_Group)
-    app.router.add_route('DELETE', '/groups/{id}', DELETE_Group)
-    app.router.add_route('PUT', '/groups/{id}', PUT_Group)
-    app.router.add_route('POST', '/groups', POST_Group)
-    app.router.add_route('GET', '/groups/{id}/links', GET_Links)
-    app.router.add_route('GET', '/groups/{id}/links/{title}', GET_Link)
-    app.router.add_route('DELETE', '/groups/{id}/links/{title}', DELETE_Link)
-    app.router.add_route('PUT', '/groups/{id}/links/{title}', PUT_Link)
-    app.router.add_route('GET', '/groups/{id}/attributes', GET_Attributes)
-    app.router.add_route('GET', '/groups/{id}/attributes/{name}',
-                         GET_Attribute)
-    app.router.add_route('DELETE', '/groups/{id}/attributes/{name}',
-                         DELETE_Attribute)
-    app.router.add_route('PUT', '/groups/{id}/attributes/{name}',
-                         PUT_Attribute)
-    app.router.add_route('GET', '/datatypes/{id}', GET_Datatype)
-    app.router.add_route('DELETE', '/datatypes/{id}', DELETE_Datatype)
-    app.router.add_route('POST', '/datatypes', POST_Datatype)
-    app.router.add_route('GET', '/datatypes/{id}/attributes', GET_Attributes)
-    app.router.add_route('GET', '/datatypes/{id}/attributes/{name}',
-                         GET_Attribute)
-    app.router.add_route('DELETE', '/datatypes/{id}/attributes/{name}',
-                         DELETE_Attribute)
-    app.router.add_route('PUT', '/datatypes/{id}/attributes/{name}',
-                         PUT_Attribute)
-    app.router.add_route('GET', '/datasets/{id}', GET_Dataset)
-    app.router.add_route('DELETE', '/datasets/{id}', DELETE_Dataset)
-    app.router.add_route('POST', '/datasets', POST_Dataset)
-    app.router.add_route('PUT', '/datasets/{id}/shape', PUT_DatasetShape)
-    app.router.add_route('GET', '/datasets/{id}/attributes', GET_Attributes)
-    app.router.add_route('GET', '/datasets/{id}/attributes/{name}',
-                         GET_Attribute)
-    app.router.add_route('DELETE', '/datasets/{id}/attributes/{name}',
-                         DELETE_Attribute)
-    app.router.add_route('PUT', '/datasets/{id}/attributes/{name}',
-                         PUT_Attribute)
-    app.router.add_route('PUT', '/chunks/{id}', PUT_Chunk)
-    app.router.add_route('GET', '/chunks/{id}', GET_Chunk)
-    app.router.add_route('POST', '/chunks/{id}', POST_Chunk)
-    app.router.add_route('DELETE', '/chunks/{id}', DELETE_Chunk)
-    app.router.add_route("POST", '/roots/{id}', POST_Root)
-    app.router.add_route("DELETE", '/prestop', preStop)
+    app.router.add_route("GET", "/domains", GET_Domain)
+    app.router.add_route("PUT", "/domains", PUT_Domain)
+    app.router.add_route("DELETE", "/domains", DELETE_Domain)
+    app.router.add_route("PUT", "/acls/{username}", PUT_ACL)
+    app.router.add_route("GET", "/groups/{id}", GET_Group)
+    app.router.add_route("DELETE", "/groups/{id}", DELETE_Group)
+    app.router.add_route("PUT", "/groups/{id}", PUT_Group)
+    app.router.add_route("POST", "/groups", POST_Group)
+    app.router.add_route("GET", "/groups/{id}/links", GET_Links)
+    app.router.add_route("GET", "/groups/{id}/links/{title}", GET_Link)
+    app.router.add_route("DELETE", "/groups/{id}/links/{title}", DELETE_Link)
+    app.router.add_route("PUT", "/groups/{id}/links/{title}", PUT_Link)
+    app.router.add_route("GET", "/groups/{id}/attributes", GET_Attributes)
+    app.router.add_route("GET", "/groups/{id}/attributes/{name}", GET_Attribute)
+    app.router.add_route("DELETE", "/groups/{id}/attributes/{name}", DELETE_Attribute)
+    app.router.add_route("PUT", "/groups/{id}/attributes/{name}", PUT_Attribute)
+    app.router.add_route("GET", "/datatypes/{id}", GET_Datatype)
+    app.router.add_route("DELETE", "/datatypes/{id}", DELETE_Datatype)
+    app.router.add_route("POST", "/datatypes", POST_Datatype)
+    app.router.add_route("GET", "/datatypes/{id}/attributes", GET_Attributes)
+    app.router.add_route("GET", "/datatypes/{id}/attributes/{name}", GET_Attribute)
+    app.router.add_route(
+        "DELETE", "/datatypes/{id}/attributes/{name}", DELETE_Attribute
+    )
+    app.router.add_route("PUT", "/datatypes/{id}/attributes/{name}", PUT_Attribute)
+    app.router.add_route("GET", "/datasets/{id}", GET_Dataset)
+    app.router.add_route("DELETE", "/datasets/{id}", DELETE_Dataset)
+    app.router.add_route("POST", "/datasets", POST_Dataset)
+    app.router.add_route("PUT", "/datasets/{id}/shape", PUT_DatasetShape)
+    app.router.add_route("GET", "/datasets/{id}/attributes", GET_Attributes)
+    app.router.add_route("GET", "/datasets/{id}/attributes/{name}", GET_Attribute)
+    app.router.add_route("DELETE", "/datasets/{id}/attributes/{name}", DELETE_Attribute)
+    app.router.add_route("PUT", "/datasets/{id}/attributes/{name}", PUT_Attribute)
+    app.router.add_route("PUT", "/chunks/{id}", PUT_Chunk)
+    app.router.add_route("GET", "/chunks/{id}", GET_Chunk)
+    app.router.add_route("POST", "/chunks/{id}", POST_Chunk)
+    app.router.add_route("DELETE", "/chunks/{id}", DELETE_Chunk)
+    app.router.add_route("POST", "/roots/{id}", POST_Root)
+    app.router.add_route("DELETE", "/prestop", preStop)
 
     return app
 
 
 async def bucketScan(app):
-    """ Scan v2 keys and update .info.json
-    """
+    """Scan v2 keys and update .info.json"""
     log.info("bucketScan start")
 
     async_sleep_time = int(config.get("async_sleep_time"))
     scan_wait_time = async_sleep_time * 6  # default to ~1min
     log.info("scan_wait_time: {}".format(scan_wait_time))
 
     # update/initialize root object before starting node updates
@@ -153,66 +146,86 @@
                 msg = f"bucketScan - HTTPForbidden error scanning {root_id}: "
                 msg += f"{fe}"
                 log.warn(msg)
             except HTTPBadRequest as bre:
                 msg = f"bucketScan - HTTPBadRequest error scanning {root_id}: "
                 msg += f"{bre}"
                 log.error(msg)
+                tb = traceback.format_exc()
+                print("traceback:", tb)
             except HTTPInternalServerError as ise:
                 msg = "bucketScan - HTTPInternalServer error scanning "
                 msg += f"{root_id}: {ise}"
-                log.error()
+                log.error(msg)
+                tb = traceback.format_exc()
+                print("traceback:", tb)
             except Exception as e:
                 msg = "bucketScan - Unexpected exception scanning "
                 msg += f"{root_id}: {e}"
                 log.error(msg)
+                tb = traceback.format_exc()
+                print("traceback:", tb)
 
         log.info(f"bucketScan - sleep: {async_sleep_time}")
         await asyncio.sleep(async_sleep_time)
 
     # shouldn't ever get here
     log.error("bucketScan terminating unexpectedly")
 
 
+def get_gc_count(app):
+    """Return number of items in gc queue"""
+    count = 0
+    gc_buckets = app["gc_buckets"]
+    for bucket in gc_buckets:
+        log.debug(f"gc_count - getting count for bucket: {bucket}")
+        gc_ids = gc_buckets[bucket]
+        count += len(gc_ids)
+    return count
+
+
 async def bucketGC(app):
-    """ remove objects from db for any deleted root groups or datasets
-    """
-    log.info("bucketGC start")
+    """remove objects from db for any deleted root groups or datasets"""
     async_sleep_time = int(config.get("async_sleep_time"))
-    log.info("async_sleep_time: {}".format(async_sleep_time))
+    log.info(f"bucketGC start - async_sleep_time: {async_sleep_time}")
 
     # update/initialize root object before starting GC
 
     while True:
-        if app["node_state"] != "READY":
+        if app["node_state"] not in ("READY", "TERMINATING"):
             log.info("bucketGC - waiting for Node state to be READY")
             await asyncio.sleep(async_sleep_time)
             continue  # wait for READY state
 
-        gc_ids = app["gc_ids"]
-        while len(gc_ids) > 0:
-            obj_id = gc_ids.pop()
-            log.info(f"got gc id: {obj_id}")
-            if not isValidUuid(obj_id):
-                log.error(f"bucketGC - got unexpected gc id: {obj_id}")
-                continue
-            if not isSchema2Id(obj_id):
-                log.warn(f"bucketGC - ignoring v1 id: {obj_id}")
-                continue
-            if getCollectionForId(obj_id) == "groups":
-                if not isRootObjId(obj_id):
-                    log.error(f"bucketGC - unexpected non-root id: {obj_id}")
+        gc_buckets = app["gc_buckets"]
+        for bucket in gc_buckets:
+            log.debug(f"bucketGC - getting keys for bucket: {bucket}")
+            gc_ids = gc_buckets[bucket]
+            while len(gc_ids) > 0:
+                obj_id = gc_ids.pop()
+                log.info(f"got gc id: {obj_id}")
+                if not isValidUuid(obj_id):
+                    log.error(f"bucketGC - got unexpected gc id: {bucket}/{obj_id}")
                     continue
-                log.info(f"bucketGC - delete root objs: {obj_id}")
-                await removeKeys(app, obj_id)
-            elif getCollectionForId(obj_id) == "datasets":
-                log.info(f"bucketGC - delete dataset: {obj_id}")
-                await removeKeys(app, obj_id)
-            else:
-                log.error(f"bucketGC - unexpected obj_id class: {obj_id}")
+                if not isSchema2Id(obj_id):
+                    log.warn(f"bucketGC - ignoring v1 id: {bucket}/{obj_id}")
+                    continue
+                if getCollectionForId(obj_id) == "groups":
+                    if not isRootObjId(obj_id):
+                        log.error(
+                            f"bucketGC - unexpected non-root id: {bucket}/{obj_id}"
+                        )
+                        continue
+                    log.info(f"bucketGC - delete root objs: {bucket}/{obj_id}")
+                    await removeKeys(app, obj_id, bucket=bucket)
+                elif getCollectionForId(obj_id) == "datasets":
+                    log.info(f"bucketGC - delete dataset: {bucket}/{obj_id}")
+                    await removeKeys(app, obj_id, bucket=bucket)
+                else:
+                    log.error(f"bucketGC - unexpected obj_id class: {bucket}/{obj_id}")
 
         log.info(f"bucketGC - sleep: {async_sleep_time}")
         await asyncio.sleep(async_sleep_time)
 
     # shouldn't ever get here
     log.error("bucketGC terminating unexpectedly")
 
@@ -229,19 +242,14 @@
 
         # run root scan
         loop.create_task(bucketScan(app))
 
         # run root/dataset GC
         loop.create_task(bucketGC(app))
 
-async def on_shutdown(app):
-    """ Release any held resources """
-    log.info("on_shutdown")
-    await release_http_client(app)
-
 
 def create_app():
     """Create datanode aiohttp application
 
     :param loop: The asyncio loop to use for the application
     :rtype: aiohttp.web.Application
     """
@@ -266,64 +274,127 @@
         # let Blosc select thread count based on processor type
         blosc_nthreads = getBloscThreads()
         log.debug(f"Using default blosc nthreads: {blosc_nthreads}")
 
     # create the app object
     loop = asyncio.get_event_loop()
     app = loop.run_until_complete(init())
-    kwargs = {"mem_target": metadata_mem_cache_size,
-              "name": "MetaCache",
-              "expire_time": metadata_mem_cache_expire}
-    app['meta_cache'] = LruCache(**kwargs)
-    kwargs = {"mem_target": chunk_mem_cache_size,
-              "name": "ChunkCache",
-              "expire_time": chunk_mem_cache_expire}
-    app['chunk_cache'] = LruCache(**kwargs)
-    app['deleted_ids'] = set()
+    kwargs = {
+        "mem_target": metadata_mem_cache_size,
+        "name": "MetaCache",
+        "expire_time": metadata_mem_cache_expire,
+    }
+    app["meta_cache"] = LruCache(**kwargs)
+    kwargs = {
+        "mem_target": chunk_mem_cache_size,
+        "name": "ChunkCache",
+        "expire_time": chunk_mem_cache_expire,
+    }
+    app["chunk_cache"] = LruCache(**kwargs)
+    app["deleted_ids"] = set()
     # map of objids to timestamp and bucket of which they were last updated
-    app['dirty_ids'] = {}
+    app["dirty_ids"] = {}
     # map of dataset ids to deflate levels (if compressed)
-    app['filter_map'] = {}
+    app["filter_map"] = {}
     # map of objid to timestamp for in-flight read requests
-    app['pending_s3_read'] = {}
+    app["pending_s3_read"] = {}
     # map of objid to timestamp for in-flight write requests
-    app['pending_s3_write'] = {}
+    app["pending_s3_write"] = {}
     # map of objid to asyncio Task objects for writes
-    app['pending_s3_write_tasks'] = {}
+    app["pending_s3_write_tasks"] = {}
     # map of root_id to bucket name used for notify root of changes in domain
-    app['root_notify_ids'] = {}
+    app["root_notify_ids"] = {}
     # map of root_id to bucket name for pending root scans
-    app['root_scan_ids'] = {}
+    app["root_scan_ids"] = {}
     # set of root or dataset ids for deletion
-    app['gc_ids'] = set()
-    app['objDelete_prefix'] = None  # used by async_lib removeKeys
+    app["gc_buckets"] = {}
+    app["objDelete_prefix"] = None  # used by async_lib removeKeys
 
     # TODO - there's nothing to prevent the deflate_map from getting
     # ever larger
     # (though it is only one int per dataset id)
     # add a timestamp and remove at a certain time?
     # delete entire map whenver the synch queue is empty?
 
     # run background tasks
     app.on_startup.append(start_background_tasks)
+    # set method to run when app is being terminated
     app.on_shutdown.append(on_shutdown)
 
     return app
 
 
+async def on_shutdown(app):
+    """Release any held resources"""
+    log.info("on_shutdown - setting node_state to TERMINATING")
+    app["node_state"] = "TERMINATING"
+    s3_sync_interval = config.get("s3_sync_interval")
+    sleep_interval = float(s3_sync_interval) / 4.0
+    pending_s3_write_tasks = app["pending_s3_write_tasks"]
+
+    # wait for s3sync queue to drain
+    while True:
+        pending_write_count = len(pending_s3_write_tasks)
+        if pending_write_count == 0:
+            log.debug("on_shutdown - no pending write tasks")
+            break
+        msg = f"on_shutdown - waiting on {pending_write_count} write tasks "
+        msg += f"sleeping for {sleep_interval:.2f}"
+        log.warning(msg)
+        await asyncio.sleep(sleep_interval)
+
+    # wait on gc tasks to complete
+    while True:
+        gc_count = get_gc_count(app)
+        if gc_count == 0:
+            log.debug("on_shutdown - no gc items")
+            break
+        msg = f"on_shutdown - waiting on {gc_count} gc tasks "
+        msg += f"sleeping for {sleep_interval:.2f}"
+        log.warning(msg)
+        await asyncio.sleep(sleep_interval)
+
+    # finally release any http_clients
+    await release_http_client(app)
+
+    log.info("on_shutdown - done")
+
+
+async def preStop(request):
+    """HTTP Method used by K8s to signal the container is shutting down"""
+
+    log.request(request)
+    app = request.app
+
+    shutdown_start = time.time()
+    log.warn(f"preStop request calling on_shutdown at {shutdown_start:.2f}")
+    await on_shutdown(app)
+    shutdown_elapse_time = time.time() - shutdown_start
+    msg = f"shutdown took: {shutdown_elapse_time:.2f} seconds"
+    if shutdown_elapse_time > 2.0:
+        # 2.0 is the default grace period for kubernetes
+        log.warn(msg)
+    else:
+        log.info(msg)
+    resp = await jsonResponse(request, {})
+    log.response(request, resp=resp)
+    return resp
+
+
 #
 # Main
 #
 
+
 def main():
     log.info("Data node initializing")
     app = create_app()
 
     # run app using either socket or tcp
-    
+
     if app["dn_urls"] and app["node_number"] >= 0:
         dn_urls = app["dn_urls"]
         node_number = app["node_number"]
         if node_number >= len(dn_urls):
             msg = f"Invalid node_number: {node_number} "
             msg += f"must be less than {len(dn_urls)}"
             msg += f" dn_urls: {dn_urls}"
@@ -357,9 +428,9 @@
         # Use TCP connection
         log.info(f"run_app on port: {dn_port}")
         run_app(app, port=dn_port)
 
     log.info("datanode exiting")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `hsds-0.7.0b11/hsds/datanode_lib.py` & `hsds-0.8.0/hsds/datanode_lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,53 +6,60 @@
 # Utilities.  The full HSDS copyright notice, including                      #
 # terms governing use, modification, and redistribution, is contained in     #
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
-# data node of hsds cluster
+# utility methods for datanode handlers
 #
+
 import asyncio
+import json
 import time
 import numpy as np
 from aiohttp.web_exceptions import HTTPGone, HTTPInternalServerError
 from aiohttp.web_exceptions import HTTPNotFound, HTTPForbidden
 from aiohttp.web_exceptions import HTTPServiceUnavailable, HTTPBadRequest
 from .util.idUtil import validateInPartition, getS3Key, isValidUuid
 from .util.idUtil import isValidChunkId, getDataNodeUrl, isSchema2Id
 from .util.idUtil import getRootObjId, isRootObjId
 from .util.storUtil import getStorJSONObj, putStorJSONObj, putStorBytes
 from .util.storUtil import getStorBytes, isStorObj, deleteStorObj
-from .util.storUtil import getBucketFromStorURI, getKeyFromStorURI
+from .util.storUtil import getBucketFromStorURI, getKeyFromStorURI, getURIFromKey
 from .util.domainUtil import isValidDomain, getBucketForDomain
 from .util.attrUtil import getRequestCollectionName
 from .util.httpUtil import http_post
 from .util.dsetUtil import getChunkLayout, getFilterOps, getFillValue
-from .util.chunkUtil import getDatasetId
-from .util.arrayUtil import arrayToBytes, bytesToArray
+from .util.dsetUtil import getChunkInitializer, getSliceQueryParam
+from .util.chunkUtil import getDatasetId, getChunkSelection, getChunkIndex
+from .util.arrayUtil import arrayToBytes, bytesToArray, getShapeDims, jsonToArray
 from .util.hdf5dtype import createDataType, getItemSize
+from .util.rangegetUtil import ChunkLocation, chunkMunge
 
 from . import config
 from . import hsds_logger as log
 
+# supported initializer commands
+INITIALIZER_CMDS = ["chunklocator", "arange"]
+
 
 def get_obj_id(request, body=None):
-    """ Get object id from request
-        Raise HTTPException on errors.
+    """Get object id from request
+    Raise HTTPException on errors.
     """
     obj_id = None
     collection = None
     app = request.app
     if body and "id" in body:
         obj_id = body["id"]
     else:
         # returns datasets|groups|datatypes
         collection = getRequestCollectionName(request)
-        obj_id = request.match_info.get('id')
+        obj_id = request.match_info.get("id")
 
     if not obj_id:
         msg = "Missing object id"
         log.error(msg)
         raise HTTPInternalServerError()
 
     if not isValidUuid(obj_id, obj_class=collection):
@@ -66,73 +73,74 @@
         log.error(f"Object {obj_id} not in partition")
         raise HTTPInternalServerError()
 
     return obj_id
 
 
 async def notify_root(app, root_id, bucket=None):
-    """ flag to write to S3
-    """
+    """flag to write to S3"""
 
-    log.info(f"notify_root: {root_id}")
+    log.info(f"notify_root: {root_id}, bucket={bucket}")
     if not isValidUuid(root_id) or not isSchema2Id(root_id):
         log.error(f"unexpected call to notify with invalid id: {root_id}")
         return
+    if not bucket:
+        log.error("notify_root - bucket not set")
+        return
     notify_req = getDataNodeUrl(app, root_id) + "/roots/" + root_id
     log.info(f"Notify: {notify_req} [{bucket}]")
     params = {}
     if bucket:
         params["bucket"] = bucket
     await http_post(app, notify_req, data={}, params=params)
 
 
 async def check_metadata_obj(app, obj_id, bucket=None):
-    """ Return False is obj does not exist
-    """
+    """Return False is obj does not exist"""
     if isValidDomain(obj_id):
         bucket = getBucketForDomain(obj_id)
 
     try:
         validateInPartition(app, obj_id)
     except KeyError:
         log.error(f"Object {obj_id} not in partition")
         raise HTTPInternalServerError()
 
-    deleted_ids = app['deleted_ids']
+    deleted_ids = app["deleted_ids"]
     if obj_id in deleted_ids:
         msg = f"{obj_id} has been deleted"
         log.info(msg)
         return False
 
-    meta_cache = app['meta_cache']
+    meta_cache = app["meta_cache"]
     if obj_id in meta_cache:
         found = True
     else:
         # Not in chache, check s3 obj exists
         s3_key = getS3Key(obj_id)
         log.debug(f"check_metadata_obj({s3_key})")
         # does key exist?
         found = await isStorObj(app, s3_key, bucket=bucket)
     return found
 
 
 async def write_s3_obj(app, obj_id, bucket=None):
-    """ writes the given object to s3 """
+    """writes the given object to s3"""
     s3key = getS3Key(obj_id)
     msg = f"write_s3_obj for obj_id: {obj_id} / s3_key: {s3key}  "
     msg += f"bucket: {bucket}"
     log.info(msg)
     pending_s3_write = app["pending_s3_write"]
     pending_s3_write_tasks = app["pending_s3_write_tasks"]
     dirty_ids = app["dirty_ids"]
-    chunk_cache = app['chunk_cache']
-    meta_cache = app['meta_cache']
-    filter_map = app['filter_map']
+    chunk_cache = app["chunk_cache"]
+    meta_cache = app["meta_cache"]
+    filter_map = app["filter_map"]
     notify_objs = app["root_notify_ids"]
-    deleted_ids = app['deleted_ids']
+    deleted_ids = app["deleted_ids"]
     success = False
 
     if isValidDomain(obj_id):
         domain_bucket = getBucketForDomain(obj_id)
         if bucket and bucket != domain_bucket:
             msg = f"expected bucket for domain: {obj_id} to match what was "
             msg += "passed to write_s3_obj"
@@ -308,42 +316,44 @@
     # calculate time to do the write
     elapsed_time = time.time() - now
     log.info(f"s3 write for {obj_id} took {elapsed_time:.3f}s")
     return obj_id
 
 
 async def get_metadata_obj(app, obj_id, bucket=None):
-    """ Get object from metadata cache (if present).
-        Otherwise fetch from S3 and add to cache
+    """Get object from metadata cache (if present).
+    Otherwise fetch from S3 and add to cache
     """
     log.info(f"get_metadata_obj: {obj_id} bucket: {bucket}")
     if isValidDomain(obj_id):
         domain_bucket = getBucketForDomain(obj_id)
         if bucket and domain_bucket and bucket != domain_bucket:
-            msg = f"get_metadata_obj for domain: {obj_id} but bucket param was: {bucket}"
+            msg = (
+                f"get_metadata_obj for domain: {obj_id} but bucket param was: {bucket}"
+            )
             log.error(msg)
             raise HTTPInternalServerError()
         if not bucket:
             bucket = domain_bucket
 
     if not bucket:
         log.warn("get_metadata_obj - bucket is None")
 
     # don't call validateInPartition since this is used to pull in
     # immutable data from other nodes
 
-    deleted_ids = app['deleted_ids']
+    deleted_ids = app["deleted_ids"]
     # don't raise 410 for domains since a domain might have been
     # re-created outside the server
     if obj_id in deleted_ids and not isValidDomain(obj_id):
         msg = f"{obj_id} has been deleted"
         log.warn(msg)
         raise HTTPGone()
 
-    meta_cache = app['meta_cache']
+    meta_cache = app["meta_cache"]
     obj_json = None
     if obj_id in meta_cache:
         log.debug(f"{obj_id} found in meta cache")
         obj_json = meta_cache[obj_id]
     else:
         s3_key = getS3Key(obj_id)
         pending_s3_read = app["pending_s3_read"]
@@ -351,15 +361,17 @@
             # already a read in progress, wait for it to complete
             read_start_time = pending_s3_read[obj_id]
             msg = f"s3 read request for {s3_key} was "
             msg += f"requested at: {read_start_time}"
             log.info(msg)
             store_read_timeout = float(config.get("store_read_timeout", default=2.0))
             log.debug(f"store_read_timeout: {store_read_timeout}")
-            store_read_sleep_interval = float(config.get("store_read_sleep_interval", default=0.1))
+            store_read_sleep_interval = float(
+                config.get("store_read_sleep_interval", default=0.1)
+            )
             while time.time() - read_start_time < store_read_timeout:
                 log.debug(f"waiting for pending s3 read {s3_key}, sleeping")
                 await asyncio.sleep(store_read_sleep_interval)  # sleep for sub-second?
                 if obj_id in meta_cache:
                     log.info(f"object {obj_id} has arrived!")
                     obj_json = meta_cache[obj_id]
                     break
@@ -373,16 +385,19 @@
             log.debug(f"getS3JSONObj({obj_id}, bucket={bucket})")
             if obj_id not in pending_s3_read:
                 pending_s3_read[obj_id] = time.time()
             # read S3 object as JSON
             try:
                 obj_json = await getStorJSONObj(app, s3_key, bucket=bucket)
                 # read complete - remove from pending map
-                elapsed_time = time.time() - pending_s3_read[obj_id]
-                log.info(f"s3 read for {obj_id} took {elapsed_time}")
+                if obj_id in pending_s3_read:
+                    elapsed_time = time.time() - pending_s3_read[obj_id]
+                    log.info(f"s3 read for {obj_id} took {elapsed_time}")
+                else:
+                    log.warn(f"s3 read complete but pending object: {obj_id} not found")
                 meta_cache[obj_id] = obj_json  # add to cache
             except HTTPNotFound:
                 msg = f"HTTPNotFound for {obj_id} bucket:{bucket} "
                 msg += f"s3key: {s3_key}"
                 log.warn(msg)
                 if obj_id in deleted_ids and isValidDomain(obj_id):
                     raise HTTPGone()
@@ -400,17 +415,18 @@
             finally:
                 if obj_id in pending_s3_read:
                     del pending_s3_read[obj_id]
 
     return obj_json
 
 
-async def save_metadata_obj(app, obj_id, obj_json,
-                            bucket=None, notify=False, flush=False):
-    """ Persist the given object """
+async def save_metadata_obj(
+    app, obj_id, obj_json, bucket=None, notify=False, flush=False
+):
+    """Persist the given object"""
     msg = f"save_metadata_obj {obj_id} bucket={bucket} notify={notify} "
     msg += f"flush={flush}"
     log.info(msg)
     if notify and not flush:
         log.error("notify not valid when flush is false")
         raise HTTPInternalServerError()
 
@@ -425,26 +441,26 @@
         raise HTTPInternalServerError()
 
     if isValidChunkId(obj_id):
         log.warn(f"save_metadata_obj {obj_id} not supported for chunks")
         raise HTTPBadRequest()
 
     dirty_ids = app["dirty_ids"]
-    deleted_ids = app['deleted_ids']
+    deleted_ids = app["deleted_ids"]
     if obj_id in deleted_ids:
         if isValidUuid(obj_id):
             # domain objects may be re-created, but shouldn't see repeats of
             # deleted uuids
             log.warn(f"{obj_id} has been deleted")
             raise HTTPInternalServerError()
         elif obj_id in deleted_ids:
             deleted_ids.remove(obj_id)  # un-gone the domain id
 
     # update meta cache
-    meta_cache = app['meta_cache']
+    meta_cache = app["meta_cache"]
     log.debug(f"save: {obj_id} to cache")
     meta_cache[obj_id] = obj_json
 
     meta_cache.setDirty(obj_id)
     now = time.time()
     log.debug(f"setting dirty_ids[{obj_id}] = ({now}, {bucket})")
     if isValidUuid(obj_id) and not bucket:
@@ -473,30 +489,36 @@
         if notify:
             log.debug(f"save_metadata_obj - sending notify for {obj_id}")
             if isValidUuid(obj_id) and isSchema2Id(obj_id):
                 root_id = getRootObjId(obj_id)
                 await notify_root(app, root_id, bucket=bucket)
 
 
-async def delete_metadata_obj(app, obj_id, notify=True,
-                              root_id=None, bucket=None):
-    """ Delete the given object """
-    meta_cache = app['meta_cache']
+async def delete_metadata_obj(app, obj_id, notify=True, root_id=None, bucket=None):
+    """Delete the given object"""
+    meta_cache = app["meta_cache"]
     dirty_ids = app["dirty_ids"]
     log.info(f"delete_meta_data_obj: {obj_id} notify: {notify}")
     if isValidDomain(obj_id):
         bucket = getBucketForDomain(obj_id)
+        log.debug(f"delete_meta_data_obj: using bucket: {bucket}")
+
+    if not bucket:
+        log.error("delete_metadata_obj - bucket not set")
+        raise HTTPInternalServerError()
+
+    log.info(f"delete_meta_obj - using bucket:{bucket}")
 
     try:
         validateInPartition(app, obj_id)
     except KeyError:
         log.error(f"obj: {obj_id} not in partition")
         raise HTTPInternalServerError()
 
-    deleted_ids = app['deleted_ids']
+    deleted_ids = app["deleted_ids"]
     if obj_id in deleted_ids:
         log.warn(f"{obj_id} has already been deleted")
     else:
         log.debug(f"adding {obj_id} to deleted ids")
         deleted_ids.add(obj_id)
 
     if obj_id in meta_cache:
@@ -515,91 +537,473 @@
     else:
         msg = f"delete_metadata_obj - key {s3key} not found (never written)?"
         log.info(msg)
 
     if isValidUuid(obj_id) and isSchema2Id(obj_id):
         if isRootObjId(obj_id):
             # add to gc ids so sub-objects will be deleted
-            gc_ids = app["gc_ids"]
-            log.info(f"adding root id: {obj_id} for GC cleanup")
+            gc_buckets = app["gc_buckets"]
+            if bucket not in gc_buckets:
+                gc_buckets[bucket] = set()
+            gc_ids = gc_buckets[bucket]
+            log.info(f"adding root id: {bucket}/{obj_id} for GC cleanup")
             gc_ids.add(obj_id)
         elif notify:
             root_id = getRootObjId(obj_id)
             await notify_root(app, root_id, bucket=bucket)
         # no notify for domain deletes since the root group is being deleted
 
     log.debug(f"delete_metadata_obj for {obj_id} done")
 
 
-async def get_chunk(app, chunk_id, dset_json, bucket=None, s3path=None,
-                    s3offset=0, s3size=0, chunk_init=False):
+def arange_chunk_init(
+    app,
+    initializer,
+    chunk_id=None,
+    dset_json=None,
+):
+    """ run arange chunk initializer """
+    log.debug(f"arange_chunk_init, chunk_id: {chunk_id}")
+    if app is None:
+        log.warn("arange_chunk_init - app not set")
+    datashape = dset_json["shape"]
+    dims = getShapeDims(datashape)
+    log.debug(f"dataset shape: {dims}")
+
+    if len(dims) != 1:
+        msg = "arange initializer can only be used with 1-dimensional datasets"
+        log.warn(msg)
+        raise None
+    type_json = dset_json["type"]
+    dt = createDataType(type_json)
+    if len(dt) > 1:
+        msg = "arange initializer can't be used with compound types"
+        log.warn(msg)
+        raise None
+    type_class = type_json.get("class")
+    if type_class not in ("H5T_INTEGER", "H5T_FLOAT"):
+        msg = "arange initializer: unsupported type class: {type_class}"
+        log.warn(msg)
+        raise None
+
+    try:
+        chunk_layout = getChunkLayout(dset_json)
+    except HTTPInternalServerError:
+        msg = "non-chunked dataset"
+        log.warning(msg)
+        raise None
+
+    chunk_index = getChunkIndex(chunk_id)
+    msg = f"arange_chunk_init - chunk_index: {chunk_index}, chunk_layout: {chunk_layout}"
+    log.debug(msg)
+
+    if len(chunk_index) != 1:
+        msg = "expected chunk_index to be one-element list, but got: {chunk_index}"
+        log.error(msg)
+        raise HTTPInternalServerError()
+
+    chunk_index = chunk_index[0]
+    chunk_length = chunk_layout[0]
+
+    start = 0.0
+    step = 1.0
+
+    # adjust based on chunk initializer args
+    for i in range(1, len(initializer)):
+        arg = initializer[i]
+        parts = arg.split("=")
+        if len(parts) != 2:
+            log.warn(f"ignoring argument: {arg}")
+        if parts[0] == "--start":
+            start = float(parts[1])
+        elif parts[0] == "--step":
+            step = float(parts[1])
+        else:
+            log.warn(f"unexpected initializer arg: {arg}")
+
+    log.debug(f"arange_chunk_init - get arguments start: {start}, step: {step}")
+
+    # adjust start and stop to be chunk relative
+    start += chunk_index * chunk_length * step
+
+    if type_class == "H5T_INTEGER":
+        # convert arguments to ints
+        start = int(start)
+        step = int(step)
+
+    # compute stop based on start, step, and chunk length
+    stop = start + chunk_length * step
+
+    log.debug(f"arange_chunk_init - start: {start}, step: {step} stop: {stop}")
+
+    # finally - create the array
+    arr = np.arange(start, stop, step, dtype=dt)
+
+    return arr
+
+
+async def run_chunk_initializer(
+    app,
+    chunk_id,
+    initializer,
+    dset_json=None,
+    bucket=None
+):
+    """ initialize chunk using given initializer function """
+    log.info(f"run_chunk_initializer - chunk_id: {chunk_id} init: {initializer}")
+
+    if len(initializer) == 0:
+        log.warn("expected cmd args, but found none")
+        return None
+
+    if not dset_json:
+        log.error("run_chunk_initializer - dset_json arg not set")
+        raise HTTPInternalServerError()
+
+    if bucket is None:
+        bucket = app.get_bucket()
+    filepath = None
+
+    init_app = initializer[0]
+    if init_app not in INITIALIZER_CMDS:
+        log.warn(f"initializer cmd is not supported: {init_app}")
+        return None
+
+    # some specific initializers can be run in process
+    # if so, just do it now
+    kwargs = {"chunk_id": chunk_id, "dset_json": dset_json}
+    if init_app == "arange":
+        # can just initialize chunk directly
+        chunk_arr = None
+        try:
+            chunk_arr = arange_chunk_init(app, initializer, **kwargs)
+        except ValueError as ve:
+            log.error(f"arange chunk initializer raised value error: {ve}")
+        return chunk_arr
+
+    # example initializer args:
+    # 'hsds-chunklocator', '--h5path=/dset', '--filepath=/data/myfile.h5' '--bucket=hdf5.sample'
+    cmd_args = None
+    for arg in initializer:
+        if cmd_args is None:
+            # app name, add "hsds-" prefix for disambiguation
+            cmd_args = [f"hsds-{arg}"]
+        if arg.startswith("--filepath="):
+            npos = arg.find("=") + 1
+            filepath = arg[npos:]
+            continue
+        elif arg.startswith("--bucket="):
+            npos = arg.find("=") + 1
+            bucket = arg[npos:]
+            bucket
+        else:
+            # options other than filepath and bucket, just pass through
+            cmd_args.append(arg)
+
+    if filepath:
+        # convert to uri and add to arg list
+        log.info(f"bucket: {bucket} filepath: {filepath}")
+        fileuri = getURIFromKey(app, bucket=bucket, key=filepath)
+        log.info(f"using fileuri: {fileuri}")
+        cmd_args.append(f"--fileuri={fileuri}")
+
+    # add select option based on chunk_id
+    datashape = dset_json["shape"]
+    dims = getShapeDims(datashape)
+    log.debug(f"dataset shape: {dims}")
+    # get the chunk layout for this dataset
+    layout = getChunkLayout(dset_json)
+    log.debug(f"chunk layout: {layout}")
+
+    rank = len(dims)
+    slices = []
+    for dim in range(rank):
+        slices.append(slice(0, dims[dim], 1))
+    slices = tuple(slices)
+    chunk_selection = getChunkSelection(chunk_id, slices, layout)
+    log.debug(f"got chunk_selection: {chunk_selection}")
+    select = getSliceQueryParam(chunk_selection)
+    select_arg = f"--select={select}"
+    log.debug(f"got select arg: {select_arg}")
+    cmd_args.append(select_arg)
+
+    # set the log prefix so we can filter that out from the output
+    prefix = "chunkinit_"
+    cmd_args.append(f"--log_prefix={prefix}")
+
+    # stitch together the cmd_args to a string
+    cmd = ""
+    for cmd_arg in cmd_args:
+        cmd += f"{cmd_arg} "
+
+    log.info(f"running subprocessing cmd: {cmd}")
+
+    proc = await asyncio.create_subprocess_shell(
+        cmd,
+        stderr=asyncio.subprocess.PIPE,
+        stdout=asyncio.subprocess.PIPE
+    )
+
+    stdout, stderr = await proc.communicate()
+
+    log.info(f"{init_app} exited with {proc.returncode}")
+
+    if stderr:
+        log.warn(f'[stderr]\n{stderr.decode()}')
+    if proc.returncode != 0:
+        log.warn(f"{cmd_args[0]} returned error code; {proc.returncode}")
+        return None
+
+    if not stdout:
+        log.warn(f"no output from chunk_initializer: {init_app}")
+        return None
+
+    type_json = dset_json["type"]
+    dt = createDataType(type_json)
+
+    lines = stdout.split(b"\n")
+    log.debug(f"got {len(lines)} lines of output")
+    data = ""
+    for line in lines:
+        line = line.decode().strip()
+        if not line:
+            continue
+        if line.startswith(prefix):
+            # dump out the log line
+            print(line)
+        elif line.find(">") != -1:
+            # ignore other lines with debug output
+            pass
+        else:
+            log.debug(line)
+            data += line
+
+    if data is None:
+        log.warn("no data returned")
+        return None
+
+    log.debug(f"got {len(data)} data elements")
+
+    # read into json array
+    try:
+        json_data = json.loads(data)
+    except json.JSONDecodeError as jde:
+        log.warn(f"unable to parse return data from chunk_initializer: {jde}")
+        return None
+
+    # initializer chunk array
+    chunk_arr = np.zeros(dims, dtype=dt, order="C")
+
+    # fill in array using the text we got back
+    # will raise ValueError if the shape doesn't work out right
+
+    chunk_arr = jsonToArray(dims, dt, json_data)
+
+    log.info(f"chunk initializer: {init_app} was successful")
+    return chunk_arr
+
+
+async def get_chunk_bytes(
+        app,
+        s3key,
+        filter_ops=None,
+        bucket=None,
+        offset=0,
+        length=0,
+        item_size=0,
+        chunk_id=None,
+        chunk_dims=None,
+        hyper_dims=None
+):
+    """ For regular chunk reads, just call getStorBytes.
+        """
+    msg = f"get_chunk_bytes({chunk_id}, bucket={bucket}, offset={offset}, length={length}, "
+    msg += f"item_size={item_size}, chunk_dims={chunk_dims}, hyper_dims={hyper_dims}"
+    log.debug(msg)
+
+    if not isinstance(offset, list):
+        # regular store read
+        kwargs = {
+            "filter_ops": filter_ops,
+            "offset": offset,
+            "length": length,
+            "bucket": bucket
+        }
+
+        chunk_bytes = await getStorBytes(app, s3key, **kwargs)
+        return chunk_bytes
+
+    # intelligent range get request
+    log.debug("intelligent range get")
+
+    if hyper_dims is None:
+        log.error("get_chunk_bytes - expected hyper_dims parameter to be set")
+        raise HTTPInternalServerError()
+
+    rank = len(chunk_dims)
+    if rank != 1:
+        msg = "get_chunk_bytes - only one-dimensional datasets are supported currently "
+        msg += "for intelligent range gets"
+        log.error(msg)
+        raise HTTPInternalServerError()
+
+    num_chunks = len(offset)
+    log.debug(f"get_chunk_bytes - num_chunks: {num_chunks}")
+    if len(length) != num_chunks:
+        log.error("get_chunk_bytes - expecting length and num_chunks to have same value")
+        raise HTTPInternalServerError()
+
+    # create a buffer for the hsds chunk and arrange h5 chunks within it
+    chunk_size = np.prod(chunk_dims) * item_size
+    # number of bytes in the hd5 chunk
+    # hyper_dims = [4000,]  # test
+    h5_size = np.prod(hyper_dims) * item_size
+    log.debug(f"h5 chunk size: {h5_size}")
+    chunk_bytes = bytearray(chunk_size)
+    if num_chunks > chunk_size // h5_size:
+        # shouldn't have more than this many hyperchunks
+        msg = f"get_chunk_bytes - got more than expected hyperchunks: {num_chunks}"
+        log.error(msg)
+        raise HTTPInternalServerError()
+
+    # create a list of the chunk to be fetched
+    chunk_list = []
+    for i in range(num_chunks):
+        if length[i] == 0:
+            # ignore empty range get requests
+            continue
+        chunk_list.append(ChunkLocation(i, offset[i], length[i]))
+
+    if len(chunk_list) == 0:
+        # nothing to fetch, return zero-initialized array
+        return chunk_bytes
+
+    # munge adjacent chunks to reduce the number of storage
+    # requests needed
+    chunk_list = chunkMunge(chunk_list, max_gap=1024)
+
+    log.info(f"get_chunk_butes - stor get requests reduced from {num_chunks} to {len(chunk_list)}")
+
+    # gather all the individual h5 chunk reads into a list of tasks
+    tasks = []
+
+    for chunk_item in chunk_list:
+        if not isinstance(chunk_item, list):
+            # convert to a one-element list
+            chunk_locations = [chunk_item, ]
+        else:
+            chunk_locations = chunk_item
+
+        log.debug(f"getStorBytes processing chunk_locations {chunk_locations}")
+        # get the byte range we'll read from storage
+        item_offset = chunk_locations[0].offset
+        item_length = chunk_locations[-1].offset + chunk_locations[-1].length - item_offset
+
+        kwargs = {
+            "filter_ops": filter_ops,
+            "offset": item_offset,
+            "length": item_length,
+            "chunk_locations": chunk_locations,
+            "bucket": bucket,
+            "chunk_bytes": chunk_bytes,
+            "h5_size": h5_size,
+        }
+        msg = f"get_chunk_bytes - {len(chunk_locations)} h5 chunks,  "
+        msg += f"offset: {item_offset}, length: {item_length}"
+        log.debug(msg)
+        tasks.append(getStorBytes(app, s3key, **kwargs))
+
+    log.debug(f"running asyncio.gather on {len(tasks)} tasks")
+    results = await asyncio.gather(*tasks)
+    log.debug(f"asyncio.gather got {len(results)} results")
+    if len(results) != len(chunk_list):
+        msg = "getStorBytes - unexpected number of gather results, "
+        msg += f"expected: {len(chunk_list)}, got: {len(results)}"
+        log.error(msg)
+        raise HTTPInternalServerError()
+
+    log.debug("get_chunk_bytes done")
+    return chunk_bytes
+
+
+async def get_chunk(
+    app,
+    chunk_id,
+    dset_json,
+    bucket=None,
+    s3path=None,
+    s3offset=0,
+    s3size=0,
+    hyper_dims=None,
+    chunk_init=False,
+):
     """
     Utility method for GET_Chunk, PUT_Chunk, and POST_CHunk
-    Get a numpy array for the chunk (possibly initizaling a new chunk
+    Get a numpy array for the chunk (possibly initializing a new chunk
     if requested)
     """
     # if the chunk cache has too many dirty items, wait till items
     # get flushed to S3
-    MAX_WAIT_TIME = 10.0  # TBD - make this a config
-    chunk_cache = app['chunk_cache']
+    log.debug(f"get_chunk - chunk_id: {chunk_id} bucket: {bucket} chunk_init: {chunk_init}")
+    if s3path:
+        log.debug(f"   s3path: {s3path} s3offset: {s3offset} s3size: {s3size}")
+    if hyper_dims is not None:
+        log.debug(f"   hyper_dims: {hyper_dims}")
+    chunk_cache = app["chunk_cache"]
     if chunk_init and s3offset > 0:
-        msg = f"unable to initiale chunk {chunk_id} for reference layouts "
+        msg = f"unable to initialize chunk {chunk_id} for reference layouts "
         log.error(msg)
         raise HTTPInternalServerError()
 
     # validate arguments
     if s3path:
-        if s3size == 0:
-            msg = f"Unexpected get_chunk parameter - s3path: {s3path} with size 0"
-            log.error(msg)
-            raise HTTPInternalServerError()
         if bucket:
             msg = "get_chunk - bucket arg should not be used with s3path"
             log.error(msg)
             raise HTTPInternalServerError()
         log.debug(f"get_chunk - chunk_id: {chunk_id} s3path: {s3path}")
-        
+
     else:
         if not bucket:
             msg = "get_chunk - bucket not set"
             log.error(msg)
             raise HTTPInternalServerError()
         log.debug(f"get_chunk - chunk_id: {chunk_id} bucket: {bucket}")
 
-    if "oio_proxy" in app or "is_k8s" in app:
-        # TBD - rangeget proxy not supported on k8s yet
-        use_proxy = False
-    else:
-        use_proxy = True
-    msg = f"getChunk cache utilization: {chunk_cache.cacheUtilizationPercent}"
-    msg += f" per, dirty_count: {chunk_cache.dirtyCount}, "
+    msg = f"getChunk cache utilization: {chunk_cache.cacheUtilizationPercent}%, "
+    msg += f"dirty_count: {chunk_cache.dirtyCount}, "
     msg += f"mem_dirty: {chunk_cache.memDirty}"
     log.debug(msg)
 
     chunk_arr = None
     dims = getChunkLayout(dset_json)
     type_json = dset_json["type"]
     item_size = getItemSize(type_json)
-    layout = dset_json["layout"]
-    layout_class = None
-    if "class" in layout:
-        layout_class = layout["class"]
+    layout_json = dset_json["layout"]
+    log.debug(f"dset_json: {dset_json}")
+    layout_class = layout_json.get("class")
+    chunk_dims = getChunkLayout(dset_json)
 
     dt = createDataType(type_json)
     # note - officially we should follow the order in which the filters are
     # defined in the filter_list,
     # but since we currently have just deflate and shuffle we will always
     # apply deflate then shuffle on read, and shuffle then deflate on write
     # also note - get deflate and shuffle will update the deflate and
     # shuffle map so that the s3sync will do the right thing
     filter_ops = getFilterOps(app, dset_json, item_size)
 
     if s3path:
-        bucket = getBucketFromStorURI(s3path)
-        s3key = getKeyFromStorURI(s3path)
+        try:
+            bucket = getBucketFromStorURI(s3path)
+            s3key = getKeyFromStorURI(s3path)
+        except ValueError as ve:
+            log.error(f"Invalid URI path: {s3path} exception: {ve}")
+            raise
+            # raise HTTPInternalServerError()
         msg = f"Using s3path bucket: {bucket} and  s3key: {s3key} "
         msg += f"offset: {s3offset} length: {s3size}"
         log.debug(msg)
     else:
         s3key = getS3Key(chunk_id)
         log.debug(f"getChunk chunkid: {chunk_id} bucket: {bucket}")
     if chunk_id in chunk_cache:
@@ -613,62 +1017,70 @@
             # already a read in progress, wait for it to complete
             read_start_time = pending_s3_read[chunk_id]
             msg = f"s3 read request for {chunk_id} was requested at: "
             msg += f"{read_start_time}"
             log.info(msg)
             store_read_timeout = float(config.get("store_read_timeout", default=2.0))
             log.debug(f"store_read_timeout: {store_read_timeout}")
-            store_read_sleep_interval = float(config.get("store_read_sleep_interval", default=0.1))
+            store_read_sleep_interval = float(
+                config.get("store_read_sleep_interval", default=0.1)
+            )
 
             while time.time() - read_start_time < store_read_timeout:
                 log.debug("waiting for pending s3 read, sleeping")
-                await asyncio.sleep(store_read_sleep_interval) 
+                await asyncio.sleep(store_read_sleep_interval)
                 if chunk_id in chunk_cache:
                     log.info(f"Chunk {chunk_id} has arrived!")
                     chunk_arr = chunk_cache[chunk_id]
                     break
             if chunk_arr is None:
                 msg = f"s3 read for chunk {chunk_id} timed-out, "
                 msg += "initiaiting a new read"
                 log.warn(msg)
 
         if chunk_arr is None:
             if chunk_id not in pending_s3_read:
                 pending_s3_read[chunk_id] = time.time()
-                log.debug(f"Reading chunk {chunk_id} from S3")
 
             try:
-                kwargs = {"filter_ops": filter_ops,
-                          "offset": s3offset,
-                          "length": s3size,
-                          "bucket": bucket,
-                          "use_proxy": use_proxy}
-                chunk_bytes = await getStorBytes(app, s3key, **kwargs)
+                kwargs = {
+                    "chunk_id": chunk_id,
+                    "filter_ops": filter_ops,
+                    "offset": s3offset,
+                    "length": s3size,
+                    "item_size": item_size,
+                    "chunk_dims": chunk_dims,
+                    "hyper_dims": hyper_dims,
+                    "bucket": bucket,
+                }
+
+                chunk_bytes = await get_chunk_bytes(app, s3key, **kwargs)
+
                 if chunk_id in pending_s3_read:
                     # read complete - remove from pending map
                     elapsed_time = time.time() - pending_s3_read[chunk_id]
                     log.info(f"s3 read for {chunk_id} took {elapsed_time}")
                 else:
                     msg = f"expected to find {chunk_id} in "
                     msg += "pending_s3_read map"
                     log.warn(msg)
                 if chunk_bytes is None:
                     msg = f"read {chunk_id} bucket: {bucket} returned None"
                     raise ValueError(msg)
-                if layout_class == 'H5D_CONTIGUOUS_REF':
+                if layout_class == "H5D_CONTIGUOUS_REF":
                     if len(chunk_bytes) < s3size:
                         # we may get less than expected bytes if this chunk
                         # is close to the end of the file
                         # expand to expected number of bytes
                         msg = "extending returned bytearray for "
                         msg += "H5D_CONTIGUOUS layout from "
                         msg += f"{len(chunk_bytes)} to {s3size}"
                         log.info(msg)
                         tmp_buffer = bytearray(s3size)
-                        tmp_buffer[:len(chunk_bytes)] = chunk_bytes
+                        tmp_buffer[: len(chunk_bytes)] = chunk_bytes
                         chunk_bytes = bytes(tmp_buffer)
                 chunk_arr = bytesToArray(chunk_bytes, dt, dims)
                 log.debug(f"chunk size: {chunk_arr.size}")
             except HTTPNotFound:
                 if not chunk_init:
                     log.info(f"chunk not found for id: {chunk_id}")
                     raise  # not found return 404
@@ -676,86 +1088,103 @@
                 log.error(f"Unable to retrieve chunk array: {ve}")
                 raise HTTPInternalServerError()
             finally:
                 # exception or not, no longer pending
                 if chunk_id in pending_s3_read:
                     del pending_s3_read[chunk_id]
 
+        if chunk_arr is not None:
+            # check that there's room in the cache before adding it
+            if chunk_id in chunk_cache or chunk_cache.memFree >= chunk_arr.size:
+                chunk_cache[chunk_id] = chunk_arr  # store in cache
+            else:
+                # no room in the cache, just skip caching
+                msg = "getChunk, cache utilization: "
+                msg += f"{chunk_cache.cacheUtilizationPercent}, "
+                msg += "skip cache for chunk_id {chunk_id}"
+                log.warn(msg)
+
         if chunk_arr is None and chunk_init:
             log.debug(f"Initializing chunk {chunk_id}")
-            fill_value = getFillValue(dset_json)
-            if fill_value:
-                # need to convert list to tuples for numpy broadcast
-                if isinstance(fill_value, list):
-                    fill_value = tuple(fill_value)
-                chunk_arr = np.empty(dims, dtype=dt, order='C')
-                chunk_arr[...] = fill_value
-            else:
-                chunk_arr = np.zeros(dims, dtype=dt, order='C')
+            initializer = getChunkInitializer(dset_json)
+            if initializer:
+                log.info(f"initializing chunk:{chunk_id} with initializer: {initializer}")
+                kwargs = {}
+                kwargs["dset_json"] = dset_json
+                kwargs["bucket"] = bucket
+                # TBD - add selection for this chunk
+                chunk_arr = await run_chunk_initializer(app, chunk_id, initializer, **kwargs)
+                if chunk_arr is None:
+                    msg = f"chunk initializer {initializer} for {chunk_id} returned None"
+                    log.warn(msg)
+
+            if chunk_arr is None:
+                # normal fill value based init or initializer failed
+                fill_value = getFillValue(dset_json)
+                if fill_value:
+                    # need to convert list to tuples for numpy broadcast
+                    if isinstance(fill_value, list):
+                        fill_value = tuple(fill_value)
+                    chunk_arr = np.empty(dims, dtype=dt, order="C")
+                    chunk_arr[...] = fill_value
+                else:
+                    chunk_arr = np.zeros(dims, dtype=dt, order="C")
         else:
             log.debug(f"Chunk {chunk_id} not found")
 
-        if chunk_arr is not None:
-            # check that there's room in the cache before adding it
-            if chunk_cache.memTarget - chunk_cache.memDirty < chunk_arr.size:
-                # no room in the cache, wait till space is freed by
-                # the s3sync task
-                wait_start = time.time()
-                free_space = 0
-                while free_space < chunk_arr.size:
-                    msg = "getChunk, cache utilization: "
-                    msg += f"{chunk_cache.cacheUtilizationPercent}, "
-                    msg += "sleeping till items are flushed"
-                    log.warn(msg)
-                    if time.time() - wait_start > MAX_WAIT_TIME:
-                        msg = f"unable to save chunk {chunk_id} to "
-                        msg += "cache returning 503 error"
-                        log.warn(msg)
-                        raise HTTPServiceUnavailable()
-                    await asyncio.sleep(1)
-                    free_space = chunk_cache.memTarget - chunk_cache.memDirty
-
-            chunk_cache[chunk_id] = chunk_arr  # store in cache
     return chunk_arr
 
 
-def save_chunk(app, chunk_id, dset_json, bucket=None):
-    """ Persist the given chunk """
+def save_chunk(app, chunk_id, dset_json, chunk_arr, bucket=None):
+    """Persist the given chunk"""
     log.info(f"save_chunk {chunk_id} bucket={bucket}")
 
     try:
         validateInPartition(app, chunk_id)
     except KeyError:
         log.error(f"Chunk {chunk_id} not in partition")
         raise HTTPInternalServerError()
 
-    item_size = getItemSize(dset_json['type'])
+    item_size = getItemSize(dset_json["type"])
+    # will store filter options into app['filter_map']
+    getFilterOps(app, dset_json, item_size)
 
     chunk_cache = app["chunk_cache"]
-    chunk_cache.setDirty(chunk_id)
-    log.info(f"chunk cache dirty count: {chunk_cache.dirtyCount}")
+    if chunk_id not in chunk_cache:
+        # check that we have enough room to store the chunk
+        # TBD: there could be issues with the free space calculation
+        # not working precisely with variable types
+        log.debug(f"chunk_cache free space: {chunk_cache.memFree}")
+        if chunk_cache.memFree < chunk_arr.size:
+            msg = f"unable to save chunk: {chunk_id}, "
+            msg += f"chunk_cache free space: {chunk_cache.memFree}, "
+            msg += f"chunk_size:{chunk_arr.size}"
+            log.warn(msg)
+            raise HTTPServiceUnavailable()
 
-    # will store filter options into app['filter_map']
-    getFilterOps(app, dset_json, item_size)
+    chunk_cache[chunk_id] = chunk_arr
+    chunk_cache.setDirty(chunk_id)
+    log.debug(f"chunk cache dirty count: {chunk_cache.dirtyCount}")
 
     # async write to S3
     dirty_ids = app["dirty_ids"]
     now = time.time()
     dirty_ids[chunk_id] = (now, bucket)
 
 
-async def s3sync(app):
-    """ Periodic method that writes dirty objects in
-        the metadata cache to S3
+async def s3sync(app, s3_age_time=0):
+    """Periodic method that writes dirty objects in
+    the metadata cache to S3
     """
     max_pending_write_requests = config.get("max_pending_write_requests")
     dirty_ids = app["dirty_ids"]
     pending_s3_write = app["pending_s3_write"]
     pending_s3_write_tasks = app["pending_s3_write_tasks"]
     s3_sync_task_timeout = config.get("s3_sync_task_timeout")
+
     dirty_count = len(dirty_ids)
     if not dirty_count:
         log.info("s3sync nothing to update")
         return 0
     msg = f"s3sync update - dirtyid count: {dirty_count}, "
     msg += f"active write tasks: {len(pending_s3_write_tasks)}/"
     msg += f"{max_pending_write_requests}"
@@ -768,14 +1197,16 @@
 
     def callback(future):
         try:
             obj_id = future.result()  # returns a objid
             log.info(f"write_s3_obj callback result: {obj_id}")
         except HTTPInternalServerError as hse:
             log.error(f"write_s3_obj callback got 500: {hse}")
+        except HTTPNotFound as nfe:
+            log.error(f"write_s3_obj callback got 404: {nfe}")
         except Exception as e:
             msg = f"write_s3_obj callback unexpected exception {type(e)}: {e}"
             log.error(msg)
 
     update_count = 0
     s3sync_start = time.time()
 
@@ -791,15 +1222,15 @@
         time_since_dirty = s3sync_start - item[0]
         if time_since_dirty < 0.0:
             msg = "s3sync: expected time since dirty to be positive, "
             msg += f"but was {time_since_dirty}"
             log.warn(msg)
         bucket = item[1]
         if not bucket:
-            if "bucket_name" in app and app["bucket_name"]:
+            if app["bucket_name"]:
                 bucket = app["bucket_name"]
             else:
                 msg = f"can not determine bucket for s3sync obj_id: {obj_id}"
                 log.error(msg)
                 continue
         s3key = getS3Key(obj_id)
         msg = f"s3sync - dirty id: {obj_id}, s3key: {s3key} bucket: {bucket}"
@@ -827,15 +1258,15 @@
                 log.debug(f"s3sync - key {obj_id} has a pending write")
                 if obj_id not in pending_s3_write_tasks:
                     msg = f"s3sync - no pending task for {obj_id} in "
                     msg += "pending_s3_write_tasks"
                     log.info(msg)
                 create_task = False
 
-        elif time_since_dirty < 1.0:
+        elif time_since_dirty < s3_age_time:
             msg = f"s3sync - obj {obj_id} last written {time_since_dirty:.3f} "
             msg += "seconds ago, waiting to age"
             log.debug(msg)
             create_task = False
         else:
             msg = f"s3sync - obj {obj_id} last written {time_since_dirty:.3f} "
             msg += "seconds ago, creating write task"
@@ -858,44 +1289,75 @@
         # create a set since we are not allowed to change
         root_ids = set()
         for root_id in notify_ids:
             root_ids.add(root_id)
 
         for root_id in root_ids:
             bucket = notify_ids[root_id]
-            await notify_root(app, root_id, bucket=bucket)
-            del notify_ids[root_id]
+            try:
+                await notify_root(app, root_id, bucket=bucket)
+                del notify_ids[root_id]
+            except HTTPServiceUnavailable:
+                # this can happen if we go into a WAITING state
+                log.warning(
+                    f"got HTTPServiceUnavailable exception try to notify root_id: {root_id}"
+                )
         log.info("root notify complete")
 
     # return number of objects written
     return update_count
 
 
 async def s3syncCheck(app):
     s3_sync_interval = config.get("s3_sync_interval")
+    s3_age_time = config.get("s3_age_time", default=1)
+    last_update = time.time()
+    if app["node_state"] != "TERMINATING":
+        s3_dirty_age_to_write = config.get("s3_dirty_age_to_write", default=20)
+        log.debug(f"s3sync - s3_dirty_age_to_write is {s3_dirty_age_to_write}")
+    else:
+        log.info("s3sync - node is terminating, using s3_dirty_age_to_write of 0")
+        s3_dirty_age_to_write = 0
 
     while True:
-        if app["node_state"] != "READY":
-            log.info("s3sync - clusterstate is not ready, sleeping")
+        node_state = app["node_state"]
+        if node_state == "INITIALIZING":
+            log.info("s3sync - nodestate is INITIALIZING, sleeping")
             await asyncio.sleep(s3_sync_interval)
             continue
+        elif node_state == "TERMINATING":
+            s3_age_time = 0
+            log.debug("s3sync - nodestate is TERMINATING, set s3_age_time to 0")
         else:
-            log.debug(f"s3sync - clusterstate is {app['node_state']}")
+            log.debug(
+                f"s3sync - nodestate is {node_state}, using s3_age_time of: {s3_age_time}"
+            )
 
-        update_count = await s3sync(app)
-        if update_count:
-            log.info(f"s3syncCheck {update_count} objects updated")
+        update_count = 0
+        try:
+            update_count = await s3sync(app, s3_age_time=s3_age_time)
+            if update_count:
+                log.info(f"s3syncCheck {update_count} objects updated")
+        except Exception as e:
+            # catch any exception so don't prematurely end the s3sync task
+            log.warn(f"s3syncCheck - got {type(e)} exception: {e}")
 
         pending_s3_write_tasks = app["pending_s3_write_tasks"]
-        log.debug(f"pending_write_tasks: {pending_s3_write_tasks}")
+        log.debug(f"pending_write_tasks count: {len(pending_s3_write_tasks)}")
         dirty_ids = app["dirty_ids"]
         log.debug(f"dirty_ids: {dirty_ids}")
 
         if update_count > 0:
             log.debug("s3syncCheck short sleep")
+            last_update = time.time()
             # give other tasks a chance to run
             await asyncio.sleep(0)
         else:
+            last_update_delta = time.time() - last_update
+            if last_update_delta > s3_sync_interval:
+                sleep_time = s3_sync_interval
+            else:
+                sleep_time = last_update_delta
             msg = "s3syncCheck no objects to write, "
-            msg += f"sleeping for {s3_sync_interval}"
+            msg += f"sleeping for {sleep_time:.2f}"
             log.info(msg)
-            await asyncio.sleep(s3_sync_interval)
+            await asyncio.sleep(sleep_time)
```

### Comparing `hsds-0.7.0b11/hsds/domain_dn.py` & `hsds-0.8.0/hsds/domain_dn.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # data node of hsds cluster
 #
+
 import time
 from aiohttp.web_exceptions import HTTPConflict, HTTPInternalServerError
 from aiohttp.web import json_response
 
 from .util.authUtil import getAclKeys
 from .util.domainUtil import isValidDomain, getBucketForDomain
 from .util.idUtil import validateInPartition
 from .datanode_lib import get_metadata_obj, save_metadata_obj
 from .datanode_lib import delete_metadata_obj, check_metadata_obj
 from . import hsds_logger as log
 
 
 def get_domain(request, body=None):
-    """ Extract domain and validate """
+    """Extract domain and validate"""
     app = request.app
     params = request.rel_url.query
 
     domain = None
     if "domain" in params:
         domain = params["domain"]
         log.debug(f"got domain param: {domain}")
@@ -50,16 +51,15 @@
     except KeyError:
         log.error(f"Domain {domain} not in partition")
         raise HTTPInternalServerError()
     return domain
 
 
 async def GET_Domain(request):
-    """HTTP GET method to return JSON for /domains/
-    """
+    """HTTP GET method to return JSON for /domains/"""
     log.request(request)
     app = request.app
 
     domain = get_domain(request)
     log.debug(f"get domain: {domain}")
     bucket = getBucketForDomain(domain)
     if not bucket:
@@ -71,16 +71,15 @@
 
     resp = json_response(domain_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def PUT_Domain(request):
-    """HTTP PUT method to create a domain
-    """
+    """HTTP PUT method to create a domain"""
     log.request(request)
     app = request.app
 
     if not request.has_body:
         msg = "Expected body in put domain"
         log.error(msg)
         raise HTTPInternalServerError()
@@ -142,16 +141,15 @@
 
     resp = json_response(domain_json, status=201)
     log.response(request, resp=resp)
     return resp
 
 
 async def DELETE_Domain(request):
-    """HTTP DELETE method to delete a domain
-    """
+    """HTTP DELETE method to delete a domain"""
     log.request(request)
     app = request.app
     domain = get_domain(request)
     bucket = getBucketForDomain(domain)
 
     log.info(f"delete domain: {domain}")
 
@@ -161,28 +159,28 @@
         raise HTTPInternalServerError()
     log.debug(f"using bucket: {bucket}")
 
     domain_json = await get_metadata_obj(app, domain)
     if domain_json:
         log.debug("got domain json")
     # delete domain
-    await delete_metadata_obj(app, domain, notify=True)
+    await delete_metadata_obj(app, domain, notify=True, bucket=bucket)
 
     json_rsp = {"domain": domain}
 
     resp = json_response(json_rsp)
     log.response(request, resp=resp)
     return resp
 
 
 async def PUT_ACL(request):
-    """ Handler creating/update an ACL"""
+    """Handler creating/update an ACL"""
     log.request(request)
     app = request.app
-    acl_username = request.match_info.get('username')
+    acl_username = request.match_info.get("username")
 
     if not request.has_body:
         msg = "Expected body in delete domain"
         log.error(msg)
         raise HTTPInternalServerError()
     body_json = await request.json()
```

### Comparing `hsds-0.7.0b11/hsds/domain_sn.py` & `hsds-0.8.0/hsds/domain_sn.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,65 +8,72 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # service node of hsds cluster
 #
+
 from asyncio import CancelledError
 import asyncio
 import json
 import os.path as op
-import re
 import time
 
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPForbidden, HTTPNotFound
 from aiohttp.web_exceptions import HTTPGone, HTTPInternalServerError
 from aiohttp.web_exceptions import HTTPConflict, HTTPServiceUnavailable
 from aiohttp import ClientResponseError
 from aiohttp.client_exceptions import ClientError
 from aiohttp.web import json_response
 from requests.sessions import merge_setting
 
-from .util.httpUtil import http_post, http_put, http_get, http_delete, getHref
+from .util.httpUtil import getObjectClass, http_post, http_put, http_get, http_delete
+from .util.httpUtil import getHref, respJsonAssemble
 from .util.httpUtil import jsonResponse
 from .util.idUtil import getDataNodeUrl, createObjId, getCollectionForId
 from .util.idUtil import isValidUuid, isSchema2Id, getNodeCount
 from .util.authUtil import getUserPasswordFromRequest, aclCheck, isAdminUser
 from .util.authUtil import validateUserPassword, getAclKeys
 from .util.domainUtil import getParentDomain, getDomainFromRequest
 from .util.domainUtil import isValidDomain, getBucketForDomain
 from .util.domainUtil import getPathForDomain
 from .util.storUtil import getStorKeys, getCompressors
 from .util.boolparser import BooleanParser
+from .util.globparser import globmatch
 from .servicenode_lib import getDomainJson, getObjectJson, getObjectIdByPath
-from .servicenode_lib import getRootInfo
+from .servicenode_lib import getRootInfo, checkBucketAccess
 from .basenode import getVersion
 from . import hsds_logger as log
 from . import config
 
 
 class DomainCrawler:
-
-    def __init__(self, app, root_id, bucket=None, include_attrs=True,
-                 max_tasks=40, max_objects_limit=0):
+    def __init__(
+        self,
+        app,
+        root_id,
+        bucket=None,
+        include_attrs=True,
+        max_tasks=40,
+        max_objects_limit=0,
+    ):
         log.info(f"DomainCrawler.__init__  root_id: {root_id}")
         self._app = app
         self._max_objects_limit = max_objects_limit
         self._include_attrs = include_attrs
         self._max_tasks = max_tasks
         self._q = asyncio.Queue()
         self._obj_dict = {}
         self.seen_ids = set()
         self._q.put_nowait(root_id)
         self._bucket = bucket
 
     async def crawl(self):
-        workers = [asyncio.Task(self.work())
-                   for _ in range(self._max_tasks)]
+        workers = [asyncio.Task(self.work()) for _ in range(self._max_tasks)]
         # When all work is done, exit.
         msg = "DomainCrawler - await queue.join - "
         msg += f"count: {len(self._obj_dict)}"
         log.info(msg)
         await self._q.join()
         msg = "DomainCrawler - join complete - "
         msg += f"count: {len(self._obj_dict)}"
@@ -80,17 +87,19 @@
         while True:
             obj_id = await self._q.get()
             await self.fetch(obj_id)
             self._q.task_done()
 
     async def fetch(self, obj_id):
         log.debug(f"DomainCrawler - fetch for obj_id: {obj_id}")
-        kwargs = {"include_links": True,
-                  "include_attrs": self._include_attrs,
-                  "bucket": self._bucket}
+        kwargs = {
+            "include_links": True,
+            "include_attrs": self._include_attrs,
+            "bucket": self._bucket,
+        }
         obj_json = await getObjectJson(self._app, obj_id, **kwargs)
         log.debug(f"DomainCrawler - got json for {obj_id}")
 
         # including links, so don't need link count
         if "link_count" in obj_json:
             del obj_json["link_count"]
         self._obj_dict[obj_id] = obj_json
@@ -108,30 +117,37 @@
                 num_objects = len(self._obj_dict)
                 if self._max_objects_limit > 0:
                     if num_objects >= self._max_objects_limit:
                         msg = "DomainCrawler reached limit of "
                         msg += f"{self._max_objects_limit}"
                         log.info(msg)
                         break
-                if link_obj["class"] != 'H5L_TYPE_HARD':
+                if link_obj["class"] != "H5L_TYPE_HARD":
                     continue
                 link_id = link_obj["id"]
                 if link_id not in self._obj_dict:
                     # haven't seen this object yet, get obj json
                     log.debug(f"DomainCrawler - adding link_id: {link_id}")
                     self._obj_dict[link_id] = {}  # placeholder for obj id
                     self._q.put_nowait(link_id)
         msg = f"DomainCrawler - fetch complete obj_id: {obj_id}, "
         msg += f"{len(self._obj_dict)} objects found"
         log.debug(msg)
 
 
 class FolderCrawler:
-    def __init__(self, app, domains, bucket=None, get_root=False,
-                 verbose=False, max_tasks_per_node=100):
+    def __init__(
+        self,
+        app,
+        domains,
+        bucket=None,
+        get_root=False,
+        verbose=False,
+        max_tasks_per_node=100,
+    ):
         log.info(f"FolderCrawler.__init__  {len(domains)} domain names")
         self._app = app
         self._get_root = get_root
         self._verbose = verbose
         self._q = asyncio.Queue()
         self._domain_dict = {}
         self._group_dict = {}
@@ -141,16 +157,15 @@
         max_tasks = max_tasks_per_node * getNodeCount(app)
         if len(domains) > max_tasks:
             self._max_tasks = max_tasks
         else:
             self._max_tasks = len(domains)
 
     async def crawl(self):
-        workers = [asyncio.Task(self.work())
-                   for _ in range(self._max_tasks)]
+        workers = [asyncio.Task(self.work()) for _ in range(self._max_tasks)]
         # When all work is done, exit.
         msg = f"FolderCrawler max_tasks {self._max_tasks} = await queue.join "
         msg += f"- count: {len(self._domain_dict)}"
         log.info(msg)
         await self._q.join()
         folder_count = len(self._domain_dict)
         msg = f"FolderCrawler - join complete - count: {folder_count}"
@@ -179,39 +194,39 @@
         try:
             kwargs = {"reload": True}
             domain_json = await getDomainJson(self._app, domain_key, **kwargs)
             msg = f"FolderCrawler - {domain} got domain_json: {domain_json}"
             log.debug(msg)
             if domain_json:
                 kwargs = {"verbose": self._verbose, "bucket": self._bucket}
-                domain_rsp = await get_domain_response(self._app,
-                                                       domain_json,
-                                                       **kwargs)
-                if "limits" in domain_rsp:
-                    # don't return limits for multi-domain responses
-                    del domain_rsp["limits"]
-                if "version" in domain_rsp:
-                    del domain_rsp["version"]
+                domain_rsp = await get_domain_response(self._app, domain_json, **kwargs)
+                for k in ("limits", "version", "compressors"):
+                    if k in domain_rsp:
+                        # don't return given key for multi-domain responses
+                        del domain_rsp[k]
                 msg = f"FolderCrawler - {domain} get domain_rsp: {domain_rsp}"
                 log.debug(msg)
                 # mixin domain name
                 self._domain_dict[domain] = domain_rsp
                 if self._get_root and "root" in domain_json:
                     root_id = domain_json["root"]
                     log.debug(f"fetching root json for {root_id}")
-                    root_json = await getObjectJson(self._app, root_id,
-                                                    include_links=False,
-                                                    include_attrs=True,
-                                                    bucket=self._bucket)
+                    root_json = await getObjectJson(
+                        self._app,
+                        root_id,
+                        include_links=False,
+                        include_attrs=True,
+                        bucket=self._bucket,
+                    )
                     log.debug(f"got root_json: {root_json}")
                     self._group_dict[root_id] = root_json
             else:
                 log.warn(f"FolderCrawler - no domain found for {domain}")
         except HTTPNotFound:
-            # One of the dmains not found, but continue through the list
+            # One of the domains not found, but continue through the list
             log.warn(f"fetch result - not found error for: {domain}")
         except HTTPGone:
             log.warn(f"fetch result - domain: {domain} has been deleted")
         except HTTPInternalServerError:
             log.error(f"fetch result - internal error fetching: {domain}")
         except HTTPForbidden:
             log.warn(f"fetch result - access not allowed for: {domain}")
@@ -223,42 +238,41 @@
         except Exception as e:
             msg = f"fetch result - unexpected exception for domain {domain}: "
             msg += f"exception of type {type(e)}, {e}"
             log.error(msg)
 
 
 async def get_collections(app, root_id, bucket=None):
-    """ Return the object ids for given root.
-    """
+    """Return the object ids for given root."""
 
     log.info(f"get_collections for {root_id}")
     groups = {}
     datasets = {}
     datatypes = {}
     lookup_ids = set()
     lookup_ids.add(root_id)
     params = {"bucket": bucket}
 
     while lookup_ids:
         grp_id = lookup_ids.pop()
         req = getDataNodeUrl(app, grp_id)
-        req += '/groups/' + grp_id + "/links"
+        req += "/groups/" + grp_id + "/links"
         log.debug("collection get LINKS: " + req)
         try:
             # throws 404 if doesn't exist
             links_json = await http_get(app, req, params=params)
         except HTTPNotFound:
             log.warn(f"get_collection, group {grp_id} not found")
             continue
 
         log.debug(f"got links json from dn for group_id: {grp_id}")
         links = links_json["links"]
         log.debug(f"get_collection: got links: {links}")
         for link in links:
-            if link["class"] != 'H5L_TYPE_HARD':
+            if link["class"] != "H5L_TYPE_HARD":
                 continue
             link_id = link["id"]
             obj_type = getCollectionForId(link_id)
             if obj_type == "groups":
                 if link_id in groups:
                     continue  # been here before
                 groups[link_id] = {}
@@ -281,41 +295,42 @@
     result["groups"] = groups
     result["datasets"] = datasets
     result["datatypes"] = datatypes
     return result
 
 
 async def getDomainObjects(app, root_id, include_attrs=False, bucket=None):
-    """ Iterate through all objects in heirarchy and add to obj_dict
-        keyed by obj id
+    """Iterate through all objects in heirarchy and add to obj_dict
+    keyed by obj id
     """
 
     log.info(f"getDomainObjects for root: {root_id}")
-    max_objects_limit = int(config.get("domain_req_max_objects_limit",
-                                       default=500))
+    max_objects_limit = int(config.get("domain_req_max_objects_limit", default=500))
 
-    kwargs = {"include_attrs": include_attrs,
-              "bucket": bucket,
-              "max_objects_limit": max_objects_limit}
+    kwargs = {
+        "include_attrs": include_attrs,
+        "bucket": bucket,
+        "max_objects_limit": max_objects_limit,
+    }
     crawler = DomainCrawler(app, root_id, **kwargs)
     await crawler.crawl()
     if len(crawler._obj_dict) >= max_objects_limit:
         msg = "getDomainObjects - too many objects:  "
         msg += f"{len(crawler._obj_dict)}, returning None"
-        log.info()
+        log.info(msg)
         return None
     else:
         msg = f"getDomainObjects returning: {len(crawler._obj_dict)} objects"
         log.info(msg)
         return crawler._obj_dict
 
 
 def getIdList(objs, marker=None, limit=None):
-    """ takes a map of ids to objs and returns ordered list
-        of ids, optionally reduced by marker and limit """
+    """takes a map of ids to objs and returns ordered list
+    of ids, optionally reduced by marker and limit"""
 
     ids = []
     for k in objs:
         ids.append(k)
     ids.sort()
     if not marker and not limit:
         return ids  # just return ids
@@ -328,23 +343,23 @@
         ret_ids.append(id)
         if limit and len(ret_ids) == limit:
             break
     return ret_ids
 
 
 def getLimits():
-    """ return limits the client may need """
+    """return limits the client may need"""
     limits = {}
     limits["min_chunk_size"] = int(config.get("min_chunk_size"))
     limits["max_chunk_size"] = int(config.get("max_chunk_size"))
     limits["max_request_size"] = int(config.get("max_request_size"))
-    cfg_val = int(config.get("max_chunks_per_request"))
-    limits["max_chunks_per_request"] = cfg_val
+
     return limits
 
+
 async def get_domain_response(app, domain_json, bucket=None, verbose=False):
     rsp_json = {}
     if "root" in domain_json:
         rsp_json["root"] = domain_json["root"]
         rsp_json["class"] = "domain"
     else:
         rsp_json["class"] = "folder"
@@ -421,37 +436,39 @@
     rsp_json["compressors"] = getCompressors()
     rsp_json["version"] = getVersion()
     rsp_json["lastModified"] = lastModified
     return rsp_json
 
 
 async def get_domains(request):
-    """ This method is called by GET_Domains and GET_Domain """
+    """This method is called by GET_Domains and GET_Domain"""
     app = request.app
     params = request.rel_url.query
 
     #  DomainCrawler will expect this to be larger than zero
     node_count = getNodeCount(app)
     if node_count == 0:
         log.warn("get_domains called with no active DN nodes")
         raise HTTPServiceUnavailable()
 
-    # if there is no domain passed in, get a list of top level domains
-    if "domain" not in request.rel_url.query:
-        prefix = '/'
-    else:
-        prefix = request.rel_url.query["domain"]
+    # allow domain with / to indicate a folder
+    prefix = None
+    try:
+        prefix = getDomainFromRequest(request, validate=False, allow_dns=False)
+    except ValueError:
+        pass  # igore
+    if not prefix:
+        # if there is no domain passed in, get a list of top level domains
+        prefix = "/"
 
     if "pattern" not in request.rel_url.query:
         pattern = None
-        regex = None
     else:
         pattern = request.rel_url.query["pattern"]
-        log.info(f"get_domains - using regex pattern: {pattern}")
-        regex = re.compile(pattern)
+        log.info(f"get_domains - using glob pattern: {pattern}")
 
     if "query" not in request.rel_url.query:
         query = None
     else:
         query = request.rel_url.query["query"]
         log.info(f"get_domains - using query: {query}")
 
@@ -460,15 +477,15 @@
     if k in request.rel_url.query and request.rel_url.query[k]:
         verbose = True
     else:
         verbose = False
 
     log.info(f"get_domains for: {prefix} verbose: {verbose}")
 
-    if not prefix.startswith('/'):
+    if not prefix.startswith("/"):
         msg = "Prefix must start with '/'"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     limit = None
     if "Limit" in request.rel_url.query:
         try:
@@ -502,40 +519,54 @@
 
     # list the S3 keys for this prefix
     domainNames = []
     if prefix == "/" and config.get("top_level_domains"):
         domainNames = config.get("top_level_domains")
         if isinstance(domainNames, str):
             # split multiple domains by comma char
-            domainNames = domainNames.split(',')
+            domainNames = domainNames.split(",")
     else:
         s3prefix = prefix[1:]
         log.debug(f"get_domains - listing S3 keys for {s3prefix}")
-        kwargs = {"include_stats": False,
-                  "prefix": s3prefix,
-                  "deliminator": '/',
-                  "bucket": bucket}
+        kwargs = {
+            "include_stats": False,
+            "prefix": s3prefix,
+            "deliminator": "/",
+            "bucket": bucket,
+        }
         s3keys = await getStorKeys(app, **kwargs)
         log.debug(f"get_domains - getS3Keys returned: {len(s3keys)} keys")
 
         for s3key in s3keys:
-            if s3key[-1] != '/':
+            if s3key[-1] != "/":
                 log.debug(f"get_domains - ignoring key: {s3key}")
                 continue
-            if len(s3key) > 1 and s3key[-2] == '/':
+            if len(s3key) > 1 and s3key[-2] == "/":
                 # trim off double slash
                 s3key = s3key[:-1]
             log.debug(f"get_domains - got s3key: {s3key}")
             domain = "/" + s3key[:-1]
-            if regex:
+            if pattern:
                 # do a pattern match on the basename
                 basename = op.basename(domain)
-                if not regex.match(basename):
+                log.debug(
+                    f"get_domains: checking {basename} against pattern: {pattern}"
+                )
+                try:
+                    got_match = globmatch(basename, pattern)
+                except ValueError as ve:
+                    log.warn(
+                        f"get_domains, invalid query pattern {pattern}, ValueError: {ve}"
+                    )
+                    raise HTTPBadRequest(reason="invalid query pattern")
+                if got_match:
+                    log.debug("get_domains - got_match")
+                else:
                     msg = f"get_domains - {basename} did not match "
-                    msg += f"regex: {pattern}"
+                    msg += f"pattern: {pattern}"
                     log.debug(msg)
                     continue
 
             if marker:
                 msg = f"get_domains - compare marker {marker} and {domain}"
                 log.debug(msg)
                 if marker == domain:
@@ -561,15 +592,15 @@
     await crawler.crawl()
 
     if query:
         log.info(f"get_domains - proccessing query: {query}")
         try:
             parser = BooleanParser(query)
         except IndexError as ie:
-            log.warn(f"get_domains - domaing query syntax error: {ie}")
+            log.warn(f"get_domains - domain query syntax error: {ie}")
             raise HTTPBadRequest(reason="Invalid query expression")
         attr_names = parser.getVariables()
         log.info(f"get_domains - query variables: {attr_names}")
         # remove any domains from dict for which the attribute query is false
         domain_keys = list(crawler._domain_dict.keys())
         log.debug(f"get_domains - querying through {len(domain_keys)}")
 
@@ -595,24 +626,24 @@
                     log.debug(f"{attr_name} not found")
                     del crawler._domain_dict[domain]
                     continue
                 attr_json = attributes[attr_name]
                 log.debug(f"{attr_name}: {attr_json}")
                 attr_type = attr_json["type"]
                 attr_type_class = attr_type["class"]
-                primative_types = ('H5T_INTEGER', 'H5T_FLOAT', 'H5T_STRING')
+                primative_types = ("H5T_INTEGER", "H5T_FLOAT", "H5T_STRING")
                 if attr_type_class not in primative_types:
                     msg = "unable to query non-primitive attribute class: "
                     msg += f"{attr_type_class}"
                     log.debug(msg)
                     del crawler._domain_dict[domain]
                     continue
                 attr_shape = attr_json["shape"]
                 attr_shape_class = attr_shape["class"]
-                if attr_shape_class == 'H5S_SCALAR':
+                if attr_shape_class == "H5S_SCALAR":
                     variable_dict[attr_name] = attr_json["value"]
                 else:
                     msg = "get_domains - unable to query non-scalar "
                     msg += "attributes"
                     log.debug(msg)
                     del crawler._domain_dict[domain]
                     continue
@@ -649,15 +680,15 @@
 
 async def GET_Domains(request):
     """HTTP method to return JSON for child domains of given domain"""
     log.request(request)
     app = request.app
 
     (username, pswd) = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domains = await get_domains(request)
 
     rsp_json = {"domains": domains}
@@ -669,16 +700,33 @@
 
 async def GET_Domain(request):
     """HTTP method to return JSON for given domain"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
+    parent_id = None
+    include_links = False
+    include_attrs = False
+    follow_soft_links = False
+    follow_external_links = False
+
+    if "parent_id" in params and params["parent_id"]:
+        parent_id = params["parent_id"]
+    if "include_links" in params and params["include_links"]:
+        include_links = True
+    if "include_attrs" in params and params["include_attrs"]:
+        include_attrs = True
+    if "follow_soft_links" in params and params["follow_soft_links"]:
+        follow_soft_links = True
+    if "follow_external_links" in params and params["follow_external_links"]:
+        follow_external_links = True
+
     (username, pswd) = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = None
     try:
         domain = getDomainFromRequest(request)
@@ -690,14 +738,16 @@
     log.debug(f"GET_Domain domain: {domain} bucket: {bucket}")
 
     if not bucket and not config.get("bucket_name"):
         # no bucket defined, raise 400
         msg = "Bucket not provided"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
+    if bucket:
+        checkBucketAccess(app, bucket)
 
     verbose = False
     if "verbose" in params and params["verbose"]:
         verbose = True
 
     if not domain:
         log.info("no domain passed in, returning all top-level domains")
@@ -713,41 +763,83 @@
 
     domain_json = await getDomainJson(app, domain, reload=True)
 
     if domain_json is None:
         log.warn(f"domain: {domain} not found")
         raise HTTPNotFound()
 
-    if 'owner' not in domain_json:
+    if "owner" not in domain_json:
         log.error("No owner key found in domain")
         raise HTTPInternalServerError()
 
-    if 'acls' not in domain_json:
+    if "acls" not in domain_json:
         log.error("No acls key found in domain")
         raise HTTPInternalServerError()
 
     log.debug(f"got domain_json: {domain_json}")
     # validate that the requesting user has permission to read this domain
     # aclCheck throws exception if not authorized
     aclCheck(app, domain_json, "read", username)
 
     if "h5path" in params:
         # if h5path is passed in, return object info for that path
         #   (if exists)
         h5path = params["h5path"]
-        root_id = domain_json["root"]
+
+        # select which object to perform path search under
+        root_id = parent_id if parent_id else domain_json["root"]
+
         # getObjectIdByPath throws 404 if not found
-        obj_id = await getObjectIdByPath(app, root_id, h5path, bucket=bucket)
+        obj_id, domain, _ = await getObjectIdByPath(
+            app, root_id, h5path, bucket=bucket, domain=domain,
+            follow_soft_links=follow_soft_links,
+            follow_external_links=follow_external_links)
         log.info(f"get obj_id: {obj_id} from h5path: {h5path}")
         # get authoritative state for object from DN (even if
         # it's in the meta_cache).
-        kwargs = {"refresh": True, "bucket": bucket}
+        kwargs = {"refresh": True, "bucket": bucket,
+                  "include_attrs": include_attrs, "include_links": include_links}
+
         obj_json = await getObjectJson(app, obj_id, **kwargs)
-        obj_json["domain"] = domain
-        # Not bothering with hrefs for h5path lookups...
+
+        obj_json = respJsonAssemble(obj_json, params, obj_id)
+
+        obj_json["domain"] = getPathForDomain(domain)
+
+        # client may not know class of object retrieved via path
+        obj_json["class"] = getObjectClass(obj_id)
+
+        hrefs = []
+        hrefs.append({"rel": "self", "href": getHref(request, "/")})
+        if "root" in domain_json:
+            root_uuid = domain_json["root"]
+            href = getHref(request, "/datasets")
+            hrefs.append({"rel": "database", "href": href})
+            href = getHref(request, "/groups")
+            hrefs.append({"rel": "groupbase", "href": href})
+            href = getHref(request, "/datatypes")
+            hrefs.append({"rel": "typebase", "href": href})
+            href = getHref(request, "/groups/" + root_uuid)
+            hrefs.append({"rel": "root", "href": href})
+            href = getHref(request, "/")
+            hrefs.append({"rel": "home", "href": href})
+
+        hrefs.append({"rel": "acls", "href": getHref(request, "/acls")})
+        parent_domain = getParentDomain(domain)
+        if not parent_domain or getPathForDomain(parent_domain) == "/":
+            is_toplevel = True
+        else:
+            is_toplevel = False
+        log.debug(f"href parent domain: {parent_domain}")
+        if not is_toplevel:
+            href = getHref(request, "/", domain=parent_domain)
+            hrefs.append({"rel": "parent", "href": href})
+
+        obj_json["hrefs"] = hrefs
+
         resp = await jsonResponse(request, obj_json)
         log.response(request, resp=resp)
         return resp
 
     # return just the keys as per the REST API
     kwargs = {"verbose": verbose, "bucket": bucket}
     rsp_json = await get_domain_response(app, domain_json, **kwargs)
@@ -764,49 +856,49 @@
             rsp_json["domain_objs"] = domain_objs
 
     # include dn_ids if requested
     if "getdnids" in params and params["getdnids"]:
         rsp_json["dn_ids"] = app["dn_ids"]
 
     hrefs = []
-    hrefs.append({'rel': 'self', 'href': getHref(request, '/')})
+    hrefs.append({"rel": "self", "href": getHref(request, "/")})
     if "root" in domain_json:
         root_uuid = domain_json["root"]
-        href = getHref(request, '/datasets')
-        hrefs.append({'rel': 'database', 'href': href})
-        href = getHref(request, '/groups')
-        hrefs.append({'rel': 'groupbase', 'href': href})
-        href = getHref(request, '/datatypes')
-        hrefs.append({'rel': 'typebase', 'href': href})
-        href = getHref(request, '/groups/' + root_uuid)
-        hrefs.append({'rel': 'root', 'href': href})
+        href = getHref(request, "/datasets")
+        hrefs.append({"rel": "database", "href": href})
+        href = getHref(request, "/groups")
+        hrefs.append({"rel": "groupbase", "href": href})
+        href = getHref(request, "/datatypes")
+        hrefs.append({"rel": "typebase", "href": href})
+        href = getHref(request, "/groups/" + root_uuid)
+        hrefs.append({"rel": "root", "href": href})
 
-    hrefs.append({'rel': 'acls', 'href': getHref(request, '/acls')})
+    hrefs.append({"rel": "acls", "href": getHref(request, "/acls")})
     parent_domain = getParentDomain(domain)
-    if not parent_domain or getPathForDomain(parent_domain) == '/':
+    if not parent_domain or getPathForDomain(parent_domain) == "/":
         is_toplevel = True
     else:
         is_toplevel = False
     log.debug(f"href parent domain: {parent_domain}")
     if not is_toplevel:
-        href = getHref(request, '/', domain=parent_domain)
-        hrefs.append({'rel': 'parent', 'href': href})
+        href = getHref(request, "/", domain=parent_domain)
+        hrefs.append({"rel": "parent", "href": href})
 
     rsp_json["hrefs"] = hrefs
     # mixin limits, version
     domain_json["limits"] = getLimits()
     domain_json["compressors"] = getCompressors()
     domain_json["version"] = getVersion()
     resp = await jsonResponse(request, rsp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def doFlush(app, root_id, bucket=None):
-    """ return wnen all DN nodes have wrote any pending changes to S3"""
+    """return wnen all DN nodes have wrote any pending changes to S3"""
     log.info(f"doFlush {root_id}")
     params = {"flush": 1}
     if bucket:
         params["bucket"] = bucket
     dn_urls = app["dn_urls"]
     dn_ids = []
     log.debug(f"doFlush - dn_urls: {dn_urls}")
@@ -861,41 +953,52 @@
     params = request.rel_url.query
     log.debug(f"PUT_domain params: {dict(params)}")
     # verify username, password
     username, pswd = getUserPasswordFromRequest(request)
     await validateUserPassword(app, username, pswd)
 
     # inital perms for owner and default
-    owner_perm = {'create': True,
-                  'read': True,
-                  'update': True,
-                  'delete': True,
-                  'readACL': True,
-                  'updateACL': True}
-    default_perm = {'create': False,
-                    'read': True,
-                    'update': False,
-                    'delete': False,
-                    'readACL': False,
-                    'updateACL': False}
+    owner_perm = {
+        "create": True,
+        "read": True,
+        "update": True,
+        "delete": True,
+        "readACL": True,
+        "updateACL": True,
+    }
+    default_perm = {
+        "create": False,
+        "read": True,
+        "update": False,
+        "delete": False,
+        "readACL": False,
+        "updateACL": False,
+    }
 
     try:
         domain = getDomainFromRequest(request)
     except ValueError:
         msg = "Invalid domain"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     bucket = getBucketForDomain(domain)
 
     log.info(f"PUT domain: {domain}, bucket: {bucket}")
+    if bucket:
+        checkBucketAccess(app, bucket, action="write")
 
     body = None
     if request.has_body:
-        body = await request.json()
+        try:
+            body = await request.json()
+        except json.JSONDecodeError:
+            msg = "Unable to load JSON body"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
         log.debug(f"PUT domain with body: {body}")
 
     if "getdnids" in params and params["getdnids"]:
         getdnids = True
     elif body and "getdnids" in body and body["getdnids"]:
         getdnids = True
     else:
@@ -914,19 +1017,19 @@
         domain_json = await getDomainJson(app, domain, reload=True)
         log.debug(f"got domain_json: {domain_json}")
 
         if domain_json is None:
             log.warn(f"domain: {domain} not found")
             raise HTTPNotFound()
 
-        if 'owner' not in domain_json:
+        if "owner" not in domain_json:
             log.error("No owner key found in domain")
             raise HTTPInternalServerError()
 
-        if 'acls' not in domain_json:
+        if "acls" not in domain_json:
             log.error("No acls key found in domain")
             raise HTTPInternalServerError()
         # throws exception if not allowed
         aclCheck(app, domain_json, "update", username)
         rsp_json = None
         if "root" in domain_json:
             # nothing to to do for folder objects
@@ -1011,15 +1114,15 @@
     if owner != username and not isAdminUser(app, username):
         log.warn("Only admin users are allowed to set owner for new domains")
         raise HTTPForbidden()
 
     parent_domain = getParentDomain(domain)
     log.debug(f"Parent domain: [{parent_domain}]")
 
-    if not parent_domain or getPathForDomain(parent_domain) == '/':
+    if not parent_domain or getPathForDomain(parent_domain) == "/":
         is_toplevel = True
     else:
         is_toplevel = False
 
     if is_toplevel and not is_folder:
         msg = "Only folder domains can be created at the top-level"
         log.warn(msg)
@@ -1074,25 +1177,29 @@
     if not is_folder and not linked_json:
         # create a root group for the new domain
         root_id = createObjId("roots")
         log.debug(f"new root group id: {root_id}")
         group_json = {"id": root_id, "root": root_id, "domain": domain}
         log.debug(f"create group for domain, body: {group_json}")
 
+        if body and "group" in body:
+            group_body = body["group"]
+            if "creationProperties" in group_body:
+                cpl = group_body["creationProperties"]
+                log.debug(f"adding creationProperties to post group request: {cpl}")
+                group_json["creationProperties"] = cpl
+
         # create root group
         req = getDataNodeUrl(app, root_id) + "/groups"
         post_params = {}
         bucket = getBucketForDomain(domain)
         if bucket:
             post_params["bucket"] = bucket
         try:
-            group_json = await http_post(app,
-                                         req,
-                                         data=group_json,
-                                         params=post_params)
+            group_json = await http_post(app, req, data=group_json, params=post_params)
         except ClientResponseError as ce:
             msg = "Error creating root group for domain -- " + str(ce)
             log.error(msg)
             raise HTTPInternalServerError()
     else:
         log.debug("no root group, creating folder")
 
@@ -1169,15 +1276,20 @@
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
     meta_only = False  # if True, just delete the meta cache value
     keep_root = False
     if request.has_body:
-        body = await request.json()
+        try:
+            body = await request.json()
+        except json.JSONDecodeError:
+            msg = "Unable to load JSON body"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
         if "meta_only" in body:
             meta_only = body["meta_only"]
         if "keep_root" in body:
             keep_root = body["keep_root"]
     else:
         if "meta_only" in params:
             meta_only = params["meta_only"]
@@ -1186,37 +1298,40 @@
 
     domain = None
     try:
         domain = getDomainFromRequest(request)
     except ValueError:
         log.warn(f"Invalid domain: {domain}")
         raise HTTPBadRequest(reason="Invalid domain name")
-    bucket = getBucketForDomain(domain)
-    log.debug(f"GET_Domain domain: {domain}")
+    log.debug(f"DELETE_Domain domain: {domain}")
 
     if not domain:
         msg = "No domain given"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
+    bucket = getBucketForDomain(domain)
+    if bucket:
+        checkBucketAccess(app, bucket, action="delete")
+
     log.info(f"meta_only domain delete: {meta_only}")
     if meta_only:
         # remove from domain cache if present
         domain_cache = app["domain_cache"]
         if domain in domain_cache:
             log.info(f"deleting {domain} from domain_cache")
             del domain_cache[domain]
         resp = await jsonResponse(request, {})
         return resp
 
     username, pswd = getUserPasswordFromRequest(request)
     await validateUserPassword(app, username, pswd)
 
     parent_domain = getParentDomain(domain)
-    if not parent_domain or getPathForDomain(parent_domain) == '/':
+    if not parent_domain or getPathForDomain(parent_domain) == "/":
         is_toplevel = True
     else:
         is_toplevel = False
 
     if is_toplevel and not isAdminUser(app, username):
         msg = "Deletion of top-level domains is only supported by admin users"
         log.warn(msg)
@@ -1236,21 +1351,24 @@
             raise HTTPInternalServerError()
 
     # throws exception if not allowed
     aclCheck(app, domain_json, "delete", username)
 
     # check for sub-objects if this is a folder
     if "root" not in domain_json:
-        index = domain.find('/')
-        s3prefix = domain[(index+1):] + '/'
+        index = domain.find("/")
+        nlen = index + 1
+        s3prefix = domain[nlen:] + "/"
         log.info(f"checking s3key with prefix: {s3prefix} in bucket: {bucket}")
-        kwargs = {"include_stats": False,
-                  "prefix": s3prefix,
-                  "deliminator": '/',
-                  "bucket": bucket}
+        kwargs = {
+            "include_stats": False,
+            "prefix": s3prefix,
+            "deliminator": "/",
+            "bucket": bucket,
+        }
         s3keys = await getStorKeys(app, **kwargs)
         for s3key in s3keys:
             if s3key.endswith("/"):
                 log.warn(f"attempt to delete folder {domain} with sub-items")
                 log.debug(f"got prefix: {s3keys[0]}")
                 raise HTTPConflict(reason="folder has sub-items")
 
@@ -1263,14 +1381,17 @@
 
     if "root" in domain_json and not keep_root:
         # delete the root group
 
         root_id = domain_json["root"]
         req = getDataNodeUrl(app, root_id)
         req += "/groups/" + root_id
+        params = {}
+        if bucket:
+            params["bucket"] = bucket
         await http_delete(app, req, params=params)
 
     # remove from domain cache if present
     domain_cache = app["domain_cache"]
     if domain in domain_cache:
         del domain_cache[domain]
 
@@ -1280,33 +1401,38 @@
 
 
 async def GET_ACL(request):
     """HTTP method to return JSON for given domain/ACL"""
     log.request(request)
     app = request.app
 
-    acl_username = request.match_info.get('username')
+    acl_username = request.match_info.get("username")
     if not acl_username:
         msg = "Missing username for ACL"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     (username, pswd) = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     try:
         domain = getDomainFromRequest(request)
     except ValueError:
         msg = "Invalid domain"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
+    bucket = getBucketForDomain(domain)
+
+    if bucket:
+        checkBucketAccess(app, bucket)
+
     # use reload to get authoritative domain json
     try:
         domain_json = await getDomainJson(app, domain, reload=True)
     except ClientResponseError as ce:
         if ce.code in (404, 410):
             msg = "domain not found"
             log.warn(msg)
@@ -1321,19 +1447,19 @@
         # allow read access for a users on ACL, or default
         # throws exception if not authorized
         aclCheck(app, domain_json, "read", username)
     else:
         # throws exception if not authorized
         aclCheck(app, domain_json, "readACL", username)
 
-    if 'owner' not in domain_json:
+    if "owner" not in domain_json:
         log.warn("No owner key found in domain")
         raise HTTPInternalServerError()
 
-    if 'acls' not in domain_json:
+    if "acls" not in domain_json:
         log.warn("No acls key found in domain")
         raise HTTPInternalServerError()
 
     acls = domain_json["acls"]
 
     log.debug(f"got domain_json: {domain_json}")
 
@@ -1348,58 +1474,61 @@
         acl_rsp[k] = acl[k]
     acl_rsp["userName"] = acl_username
 
     # return just the keys as per the REST API
     rsp_json = {}
     rsp_json["acl"] = acl_rsp
     hrefs = []
-    hrefs.append({'rel': 'self', 'href': getHref(request, '/acls')})
+    hrefs.append({"rel": "self", "href": getHref(request, "/acls")})
     if "root" in domain_json:
-        href = getHref(request, '/groups/' + domain_json["root"])
-        hrefs.append({'rel': 'root', 'href': href})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
-    hrefs.append({'rel': 'owner', 'href': getHref(request, '/')})
+        href = getHref(request, "/groups/" + domain_json["root"])
+        hrefs.append({"rel": "root", "href": href})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
+    hrefs.append({"rel": "owner", "href": getHref(request, "/")})
     rsp_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, rsp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def GET_ACLs(request):
     """HTTP method to return JSON for domain/ACLs"""
     log.request(request)
     app = request.app
 
     (username, pswd) = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     try:
         domain = getDomainFromRequest(request)
     except ValueError:
         msg = "Invalid domain"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
+    bucket = getBucketForDomain(domain)
+    if bucket:
+        checkBucketAccess(app, bucket)
+
     # use reload to get authoritative domain json
     try:
         domain_json = await getDomainJson(app, domain, reload=True)
     except ClientResponseError:
         log.warn("domain not found")
-        log.warn(msg)
         raise HTTPNotFound()
 
-    if 'owner' not in domain_json:
+    if "owner" not in domain_json:
         log.error("No owner key found in domain")
         raise HTTPInternalServerError()
 
-    if 'acls' not in domain_json:
+    if "acls" not in domain_json:
         log.error("No acls key found in domain")
         raise HTTPInternalServerError()
 
     acls = domain_json["acls"]
 
     log.debug(f"got domain_json: {domain_json}")
     # validate that the requesting user has permission to read this domain
@@ -1417,47 +1546,53 @@
             entry[k] = acl[k]
         acl_list.append(entry)
     # return just the keys as per the REST API
     rsp_json = {}
     rsp_json["acls"] = acl_list
 
     hrefs = []
-    hrefs.append({'rel': 'self', 'href': getHref(request, '/acls')})
+    hrefs.append({"rel": "self", "href": getHref(request, "/acls")})
     if "root" in domain_json:
-        href = getHref(request, '/groups/' + domain_json["root"])
-        hrefs.append({'rel': 'root', 'href': href})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
-    hrefs.append({'rel': 'owner', 'href': getHref(request, '/')})
+        href = getHref(request, "/groups/" + domain_json["root"])
+        hrefs.append({"rel": "root", "href": href})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
+    hrefs.append({"rel": "owner", "href": getHref(request, "/")})
     rsp_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, rsp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def PUT_ACL(request):
     """HTTP method to add a new ACL for a domain"""
     log.request(request)
     app = request.app
 
-    acl_username = request.match_info.get('username')
+    acl_username = request.match_info.get("username")
     if not acl_username:
         msg = "Missing username for ACL"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     (username, pswd) = getUserPasswordFromRequest(request)
     await validateUserPassword(app, username, pswd)
 
     if not request.has_body:
         msg = "PUT ACL with no body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
-    body = await request.json()
+    try:
+        body = await request.json()
+    except json.JSONDecodeError:
+        msg = "Unable to load JSON body"
+        log.warn(msg)
+        raise HTTPBadRequest(reason=msg)
+
     acl_keys = getAclKeys()
 
     for k in body.keys():
         if k not in acl_keys:
             msg = f"Unexpected key in request body: {k}"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
@@ -1469,14 +1604,18 @@
     try:
         domain = getDomainFromRequest(request)
     except ValueError:
         msg = "Invalid domain"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
+    bucket = getBucketForDomain(domain)
+    if bucket:
+        checkBucketAccess(app, bucket, action="write")
+
     # don't use app["domain_cache"]  if a direct domain request is made
     # as opposed to an implicit request as with other operations, query
     # the domain from the authoritative source (the dn node)
     req = getDataNodeUrl(app, domain)
     req += "/acls/" + acl_username
     log.info(f"sending dn req: {req}")
     body["domain"] = domain
@@ -1493,29 +1632,31 @@
 async def GET_Datasets(request):
     """HTTP method to return dataset collection for given domain"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
     (username, pswd) = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     try:
         domain = getDomainFromRequest(request)
     except ValueError:
         msg = "Invalid domain"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     bucket = getBucketForDomain(domain)
     if not bucket:
         bucket = config.get("bucket_name")
+    else:
+        checkBucketAccess(app, bucket)
 
     # verify the domain
     try:
         domain_json = await getDomainJson(app, domain)
     except ClientResponseError as ce:
         if ce.code == 404:
             msg = f"Domain: {domain} not found"
@@ -1524,23 +1665,20 @@
         elif ce.code == 410:
             msg = f"Domain: {domain} removed"
             log.warn(msg)
             raise HTTPGone()
         else:
             log.error(f"Unexpected error: {ce.code}")
             raise HTTPInternalServerError()
-        msg = "domain not found"
-        log.warn(msg)
-        raise HTTPNotFound()
 
-    if 'owner' not in domain_json:
+    if "owner" not in domain_json:
         log.error("No owner key found in domain")
         raise HTTPInternalServerError()
 
-    if 'acls' not in domain_json:
+    if "acls" not in domain_json:
         log.error("No acls key found in domain")
         raise HTTPInternalServerError()
 
     log.debug(f"got domain_json: {domain_json}")
     # validate that the requesting user has permission to read this domain
     # aclCheck throws exception if not authorized
     aclCheck(app, domain_json, "read", username)
@@ -1564,20 +1702,20 @@
         objs = collections["datasets"]
         obj_ids = getIdList(objs, marker=marker, limit=limit)
 
     log.debug(f"returning obj_ids: {obj_ids}")
 
     # create hrefs
     hrefs = []
-    hrefs.append({'rel': 'self', 'href': getHref(request, '/datasets')})
+    hrefs.append({"rel": "self", "href": getHref(request, "/datasets")})
     if "root" in domain_json:
         root_uuid = domain_json["root"]
-        href = getHref(request, '/groups/' + root_uuid)
-        hrefs.append({'rel': 'root', 'href': href})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
+        href = getHref(request, "/groups/" + root_uuid)
+        hrefs.append({"rel": "root", "href": href})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
 
     # return obj ids and hrefs
     rsp_json = {}
     rsp_json["datasets"] = obj_ids
     rsp_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, rsp_json)
@@ -1588,47 +1726,49 @@
 async def GET_Groups(request):
     """HTTP method to return groups collection for given domain"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
     (username, pswd) = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     try:
         domain = getDomainFromRequest(request)
     except ValueError:
         msg = "Invalid domain"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     bucket = getBucketForDomain(domain)
     if not bucket:
         bucket = config.get("bucket_name")
+    else:
+        checkBucketAccess(app, bucket)
 
     # use reload to get authoritative domain json
     try:
         domain_json = await getDomainJson(app, domain, reload=True)
     except ClientResponseError as ce:
         if ce.code == 404:
             msg = "domain not found"
             log.warn(msg)
             raise HTTPNotFound()
         else:
             log.error(f"Unexpected error: {ce.code}")
             raise HTTPInternalServerError()
 
-    if 'owner' not in domain_json:
+    if "owner" not in domain_json:
         log.error("No owner key found in domain")
         raise HTTPInternalServerError()
 
-    if 'acls' not in domain_json:
+    if "acls" not in domain_json:
         log.error("No acls key found in domain")
         raise HTTPInternalServerError()
 
     log.debug(f"got domain_json: {domain_json}")
     # validate that the requesting user has permission to read this domain
     # aclCheck throws exception if not authorized
     aclCheck(app, domain_json, "read", username)
@@ -1651,20 +1791,20 @@
         # get the groups collection list
         collections = await get_collections(app, domain_json["root"], bucket=bucket)
         objs = collections["groups"]
         obj_ids = getIdList(objs, marker=marker, limit=limit)
 
     # create hrefs
     hrefs = []
-    hrefs.append({'rel': 'self', 'href': getHref(request, '/groups')})
+    hrefs.append({"rel": "self", "href": getHref(request, "/groups")})
     if "root" in domain_json:
         root_uuid = domain_json["root"]
-        href = getHref(request, '/groups/' + root_uuid)
-        hrefs.append({'rel': 'root', 'href': href})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
+        href = getHref(request, "/groups/" + root_uuid)
+        hrefs.append({"rel": "root", "href": href})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
 
     # return obj ids and hrefs
     rsp_json = {}
     rsp_json["groups"] = obj_ids
     rsp_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, rsp_json)
@@ -1675,47 +1815,49 @@
 async def GET_Datatypes(request):
     """HTTP method to return datatype collection for given domain"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
     (username, pswd) = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     try:
         domain = getDomainFromRequest(request)
     except ValueError:
         msg = "Invalid domain"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     bucket = getBucketForDomain(domain)
     if not bucket:
         bucket = config.get("bucket_name")
+    else:
+        checkBucketAccess(app, bucket)
 
     # use reload to get authoritative domain json
     try:
         domain_json = await getDomainJson(app, domain, reload=True)
     except ClientResponseError as ce:
         if ce.code in (404, 410):
             msg = "domain not found"
             log.warn(msg)
             raise HTTPNotFound()
         else:
             log.error(f"Unexpected Error: {ce.code})")
             raise HTTPInternalServerError()
 
-    if 'owner' not in domain_json:
+    if "owner" not in domain_json:
         log.error("No owner key found in domain")
         raise HTTPInternalServerError()
 
-    if 'acls' not in domain_json:
+    if "acls" not in domain_json:
         log.error("No acls key found in domain")
         raise HTTPInternalServerError()
 
     log.debug(f"got domain_json: {domain_json}")
     # validate that the requesting user has permission to read this domain
     # aclCheck throws exception if not authorized
     aclCheck(app, domain_json, "read", username)
@@ -1738,20 +1880,20 @@
         # get the groups collection list
         collections = await get_collections(app, domain_json["root"], bucket=bucket)
         objs = collections["datatypes"]
         obj_ids = getIdList(objs, marker=marker, limit=limit)
 
     # create hrefs
     hrefs = []
-    hrefs.append({'rel': 'self', 'href': getHref(request, '/datatypes')})
+    hrefs.append({"rel": "self", "href": getHref(request, "/datatypes")})
     if "root" in domain_json:
         root_uuid = domain_json["root"]
-        href = getHref(request, '/groups/' + root_uuid)
-        hrefs.append({'rel': 'root', 'href': href})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
+        href = getHref(request, "/groups/" + root_uuid)
+        hrefs.append({"rel": "root", "href": href})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
 
     # return obj ids and hrefs
     rsp_json = {}
     rsp_json["datatypes"] = obj_ids
     rsp_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, rsp_json)
```

### Comparing `hsds-0.7.0b11/hsds/dset_dn.py` & `hsds-0.8.0/hsds/dset_dn.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # data node of hsds cluster
 #
+
 import time
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPNotFound, HTTPConflict
 from aiohttp.web_exceptions import HTTPInternalServerError
 from aiohttp.web import json_response
 
 
 from .util.idUtil import isValidUuid, validateUuid
 from .datanode_lib import get_obj_id, check_metadata_obj, get_metadata_obj
 from .datanode_lib import save_metadata_obj, delete_metadata_obj
 from . import hsds_logger as log
 
 
 async def GET_Dataset(request):
-    """HTTP GET method to return JSON for /groups/
-    """
+    """HTTP GET method to return JSON for /groups/"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
     dset_id = get_obj_id(request)
 
     if not isValidUuid(dset_id, obj_class="dataset"):
-        log.error("Unexpected type_id: {}".format(dset_id))
+        log.error(f"Unexpected dataset_id: {dset_id}")
         raise HTTPInternalServerError()
     if "bucket" in params:
         bucket = params["bucket"]
     else:
         bucket = None
 
     dset_json = await get_metadata_obj(app, dset_id, bucket=bucket)
@@ -59,15 +59,15 @@
 
     resp = json_response(resp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def POST_Dataset(request):
-    """ Handler for POST /datasets"""
+    """Handler for POST /datasets"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
     if not request.has_body:
         msg = "POST_Dataset with no body"
         log.error(msg)
@@ -121,21 +121,23 @@
         layout = body["layout"]  # client specified chunk layout
 
     # ok - all set, create committed type obj
     now = int(time.time())
 
     log.debug(f"POST_dataset typejson: {type_json}, shapejson: {shape_json}")
 
-    dset_json = {"id": dset_id,
-                 "root": root_id,
-                 "created": now,
-                 "lastModified": now,
-                 "type": type_json,
-                 "shape": shape_json,
-                 "attributes": {}}
+    dset_json = {
+        "id": dset_id,
+        "root": root_id,
+        "created": now,
+        "lastModified": now,
+        "type": type_json,
+        "shape": shape_json,
+        "attributes": {},
+    }
 
     if "creationProperties" in body:
         dset_json["creationProperties"] = body["creationProperties"]
     if layout is not None:
         dset_json["layout"] = layout
 
     kwargs = {"bucket": bucket, "notify": True, "flush": True}
@@ -152,30 +154,34 @@
 
     resp = json_response(resp_json, status=201)
     log.response(request, resp=resp)
     return resp
 
 
 async def DELETE_Dataset(request):
-    """HTTP DELETE method for dataset
-    """
+    """HTTP DELETE method for dataset"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
     log.info(f"DELETE dataset: {dset_id}")
 
     if not isValidUuid(dset_id, obj_class="dataset"):
         log.error(f"Unexpected dataset id: {dset_id}")
         raise HTTPInternalServerError()
 
     if "bucket" in params:
         bucket = params["bucket"]
     else:
-        bucket = None
+        bucket = app["bucket_name"]
+
+    if not bucket:
+        msg = "DELETE_Dataset - bucket not set"
+        log.error(msg)
+        raise HTTPBadRequest(reason=msg)
 
     # verify the id  exist
     obj_found = await check_metadata_obj(app, dset_id, bucket=bucket)
     if not obj_found:
         raise HTTPNotFound()
 
     log.debug(f"deleting dataset: {dset_id}")
@@ -193,15 +199,15 @@
 
 
 async def PUT_DatasetShape(request):
     """HTTP method to update dataset's shape"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
 
     if not isValidUuid(dset_id, obj_class="dataset"):
         log.error("Unexpected type_id: {}".format(dset_id))
         raise HTTPInternalServerError()
 
     body = await request.json()
```

### Comparing `hsds-0.7.0b11/hsds/dset_sn.py` & `hsds-0.8.0/hsds/dset_sn.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,40 +9,41 @@
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # service node of hsds cluster
 # handles dataset requests
 #
+
 import math
 import numpy as np
+from json import JSONDecodeError
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPNotFound, HTTPConflict
 
-from .util.httpUtil import http_post, http_put, http_delete, getHref
+from .util.httpUtil import http_post, http_put, http_delete, getHref, respJsonAssemble
 from .util.httpUtil import jsonResponse
 from .util.idUtil import isValidUuid, getDataNodeUrl, createObjId, isSchema2Id
 from .util.dsetUtil import getPreviewQuery, getFilterItem
 from .util.arrayUtil import getNumElements, getShapeDims
 from .util.chunkUtil import getChunkSize, guessChunk, expandChunk, shrinkChunk
 from .util.chunkUtil import getContiguousLayout
 from .util.authUtil import getUserPasswordFromRequest, aclCheck
 from .util.authUtil import validateUserPassword
-from .util.domainUtil import getDomainFromRequest, isValidDomain
-from .util.domainUtil import getBucketForDomain, getPathForDomain, verifyRoot
+from .util.domainUtil import getDomainFromRequest, getPathForDomain, isValidDomain
+from .util.domainUtil import getBucketForDomain, verifyRoot
 from .util.storUtil import getFilters
 from .util.hdf5dtype import validateTypeItem, createDataType, getBaseTypeJson
 from .util.hdf5dtype import getItemSize
 from .servicenode_lib import getDomainJson, getObjectJson, getPathForObjectId
 from .servicenode_lib import getObjectIdByPath, validateAction, getRootInfo
 from . import config
 from . import hsds_logger as log
 
 
-async def validateChunkLayout(app, shape_json, item_size, layout,
-                              bucket=None):
+async def validateChunkLayout(app, shape_json, item_size, layout, bucket=None):
     """
     Use chunk layout given in the creationPropertiesList (if defined and
     layout is valid).
     Return chunk_layout_json
     """
 
     rank = 0
@@ -59,15 +60,17 @@
     if "dims" in layout:
         chunk_dims = layout["dims"]
 
     if chunk_dims:
         # validate that the chunk_dims are valid and correlates with the
         # dataset shape
         if isinstance(chunk_dims, int):
-            chunk_dims = [chunk_dims, ]  # promote to array
+            chunk_dims = [
+                chunk_dims,
+            ]  # promote to array
         if len(chunk_dims) != rank:
             msg = "Layout rank does not match shape rank"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         for i in range(rank):
             dim_extent = space_dims[i]
             chunk_extent = chunk_dims[i]
@@ -95,18 +98,18 @@
     if "class" not in layout:
         msg = "class key not found in layout for creation property list"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     layout_class = layout["class"]
 
-    if layout_class == 'H5D_CONTIGUOUS_REF':
+    if layout_class == "H5D_CONTIGUOUS_REF":
         # reference to a dataset in a traditional HDF5 files with
         # contigious storage
-        if item_size == 'H5T_VARIABLE':
+        if item_size == "H5T_VARIABLE":
             # can't be used with variable types..
             msg = "Datsets with variable types cannot be used with "
             msg += "reference layouts"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         if "file_uri" not in layout:
             # needed for H5D_CONTIGUOUS_REF
@@ -128,18 +131,18 @@
             raise HTTPBadRequest(reason=msg)
         if "dims" in layout:
             # used defined chunk layout not allowed for H5D_CONTIGUOUS_REF
             msg = "'dims' key can not be provided for "
             msg += "H5D_CONTIGUOUS_REF layout"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-    elif layout_class == 'H5D_CHUNKED_REF':
+    elif layout_class == "H5D_CHUNKED_REF":
         # reference to a dataset in a traditional HDF5 files with
         # chunked storage
-        if item_size == 'H5T_VARIABLE':
+        if item_size == "H5T_VARIABLE":
             # can't be used with variable types..
             msg = "Datsets with variable types cannot be used with "
             msg += "reference layouts"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         if "file_uri" not in layout:
             # needed for H5D_CHUNKED_REF
@@ -154,18 +157,18 @@
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         if "chunks" not in layout:
             msg = "'chunks' key must be provided for "
             msg += "H5D_CHUNKED_REF layout"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-    elif layout_class == 'H5D_CHUNKED_REF_INDIRECT':
+    elif layout_class == "H5D_CHUNKED_REF_INDIRECT":
         # reference to a dataset in a traditional HDF5 files with chunked
         # storage using an auxillary dataset
-        if item_size == 'H5T_VARIABLE':
+        if item_size == "H5T_VARIABLE":
             # can't be used with variable types..
             msg = "Datsets with variable types cannot be used with "
             msg += "reference layouts"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         if "dims" not in layout:
             # needed for H5D_CHUNKED_REF_INDIRECT
@@ -181,51 +184,62 @@
         chunktable_id = layout["chunk_table"]
         if not isValidUuid(chunktable_id, "Dataset"):
             msg = f"Invalid chunk table id: {chunktable_id}"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         # verify the chunk table exists and is of reasonable shape
         try:
-            chunktable_json = await getObjectJson(app,
-                                                  chunktable_id,
-                                                  bucket=bucket,
-                                                  refresh=False)
+            chunktable_json = await getObjectJson(
+                app, chunktable_id, bucket=bucket, refresh=False
+            )
         except HTTPNotFound:
             msg = f"chunk table id: {chunktable_id} not found"
             log.warn(msg)
             raise
         chunktable_shape = chunktable_json["shape"]
-        if chunktable_shape["class"] == 'H5S_NULL':
+        if chunktable_shape["class"] == "H5S_NULL":
             msg = "Null space datasets can not be used as chunk tables"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
 
         chunktable_dims = getShapeDims(chunktable_shape)
         if len(chunktable_dims) != len(space_dims):
             msg = "Chunk table rank must be same as dataspace rank"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-    elif layout_class == 'H5D_CHUNKED':
+    elif layout_class == "H5D_CHUNKED":
         if "dims" not in layout:
             msg = "dims key not found in layout for creation property list"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-        if shape_json["class"] != 'H5S_SIMPLE':
+        if shape_json["class"] != "H5S_SIMPLE":
             msg = "Bad Request: chunked layout not valid with shape class: "
             msg += f"{shape_json['class']}"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
+    elif layout_class == "H5D_CONTIGUOUS":
+        if "dims" in layout:
+            msg = "dims key found in layout for creation property list "
+            msg += "for H5D_CONTIGUOUS storage class"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
+    elif layout_class == "H5D_COMPACT":
+        if "dims" in layout:
+            msg = "dims key found in layout for creation property list "
+            msg += "for H5D_COMPACT storage class"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
     else:
         msg = f"Unexpected layout: {layout_class}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
 
 async def getDatasetDetails(app, dset_id, root_id, bucket=None):
-    """ Get extra information about the given dataset """
+    """Get extra information about the given dataset"""
     # Gather additional info on the domain
     log.debug(f"getDatasetDetails {dset_id}")
 
     if not isSchema2Id(root_id):
         msg = f"no dataset details not available for schema v1 id: {root_id}"
         msg += "returning null result"
         log.info(msg)
@@ -250,19 +264,20 @@
 
 
 async def GET_Dataset(request):
     """HTTP method to return JSON description of a dataset"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
+
     include_attrs = False
 
     h5path = None
     getAlias = False
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
     if not dset_id and "h5path" not in params:
         msg = "Missing dataset id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if "include_attrs" in params and params["include_attrs"]:
         include_attrs = True
 
@@ -284,22 +299,22 @@
                 raise HTTPBadRequest(reason=msg)
         if "h5path" not in params:
             msg = "Expecting either ctype id or h5path url param"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
 
         h5path = params["h5path"]
-        if not group_id and h5path[0] != '/':
+        if not group_id and h5path[0] != "/":
             msg = "h5paths must be absolute"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         log.info(f"GET_Dataset, h5path: {h5path}")
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
@@ -313,145 +328,112 @@
 
     if h5path:
         if group_id is None:
             domain_json = await getDomainJson(app, domain)
             verifyRoot(domain_json)
             group_id = domain_json["root"]
         # throws 404 if not found
-        kwargs = {"bucket": bucket}
-        dset_id = await getObjectIdByPath(app, group_id, h5path, **kwargs)
+        kwargs = {"bucket": bucket, "domain": domain}
+        dset_id, domain, _ = await getObjectIdByPath(app, group_id, h5path, **kwargs)
         if not isValidUuid(dset_id, "Dataset"):
             msg = f"No dataset exist with the path: {h5path}"
             log.warn(msg)
             raise HTTPNotFound()
         log.info(f"get dataset_id: {dset_id} from h5path: {h5path}")
 
     # get authoritative state for dataset from DN (even if it's
     # in the meta_cache).
-    dset_json = await getObjectJson(app,
-                                    dset_id,
-                                    refresh=True,
-                                    include_attrs=include_attrs,
-                                    bucket=bucket)
+    dset_json = await getObjectJson(
+        app, dset_id, refresh=True, include_attrs=include_attrs, bucket=bucket
+    )
 
     # check that we have permissions to read the object
     await validateAction(app, domain, dset_id, username, "read")
 
-    resp_json = {}
-    resp_json["id"] = dset_json["id"]
-    resp_json["root"] = dset_json["root"]
-    resp_json["shape"] = dset_json["shape"]
-    resp_json["type"] = dset_json["type"]
-    if "creationProperties" in dset_json:
-        if "ignore_nan" in params and params["ignore_nan"]:
-            # convert fillValue to "nan" if it is a np.nan
-            s = dset_json["creationProperties"]
-            d = {}
-            for k in s:
-                v = s[k]
-                if k == "fillValue" and isinstance(v, float) and np.isnan(v):
-                    d[k] = "nan"
-                else:
-                    d[k] = v
-            resp_json["creationProperties"] = d
-        else:
-            # just return the dset_json creation props as is
-            resp_json["creationProperties"] = dset_json["creationProperties"]
-    else:
-        resp_json["creationProperties"] = {}
+    dset_json = respJsonAssemble(dset_json, params, dset_id)
 
-    if "layout" in dset_json:
-        resp_json["layout"] = dset_json["layout"]
-    resp_json["attributeCount"] = dset_json["attributeCount"]
-    resp_json["created"] = dset_json["created"]
-    resp_json["lastModified"] = dset_json["lastModified"]
-    resp_json["domain"] = getPathForDomain(domain)
+    dset_json["domain"] = getPathForDomain(domain)
 
     if getAlias:
         root_id = dset_json["root"]
         alias = []
-        idpath_map = {root_id: '/'}
-        h5path = await getPathForObjectId(app,
-                                          root_id,
-                                          idpath_map,
-                                          tgt_id=dset_id,
-                                          bucket=bucket)
+        idpath_map = {root_id: "/"}
+        h5path = await getPathForObjectId(
+            app, root_id, idpath_map, tgt_id=dset_id, bucket=bucket
+        )
         if h5path:
             alias.append(h5path)
-        resp_json["alias"] = alias
-    if include_attrs:
-        resp_json["attributes"] = dset_json["attributes"]
+        dset_json["alias"] = alias
 
     hrefs = []
-    dset_uri = '/datasets/'+dset_id
-    hrefs.append({'rel': 'self', 'href': getHref(request, dset_uri)})
-    root_uri = '/groups/' + dset_json["root"]
-    hrefs.append({'rel': 'root', 'href': getHref(request, root_uri)})
-    hrefs.append({'rel': 'home', 'href': getHref(request, '/')})
-    href = getHref(request, dset_uri+'/attributes')
-    hrefs.append({'rel': 'attributes', 'href': href})
+    dset_uri = "/datasets/" + dset_id
+    hrefs.append({"rel": "self", "href": getHref(request, dset_uri)})
+    root_uri = "/groups/" + dset_json["root"]
+    hrefs.append({"rel": "root", "href": getHref(request, root_uri)})
+    hrefs.append({"rel": "home", "href": getHref(request, "/")})
+    href = getHref(request, dset_uri + "/attributes")
+    hrefs.append({"rel": "attributes", "href": href})
 
     # provide a value link if the dataset is relatively small,
     # otherwise create a preview link that shows a limited number of
     # data values
     dset_shape = dset_json["shape"]
-    if dset_shape["class"] != 'H5S_NULL':
+    if dset_shape["class"] != "H5S_NULL":
         count = 1
-        if dset_shape["class"] == 'H5S_SIMPLE':
+        if dset_shape["class"] == "H5S_SIMPLE":
             dims = dset_shape["dims"]
             count = getNumElements(dims)
         if count <= 100:
             # small number of values, provide link to entire dataset
-            href = getHref(request, dset_uri + '/value')
-            hrefs.append({'rel': 'data', 'href': href})
+            href = getHref(request, dset_uri + "/value")
+            hrefs.append({"rel": "data", "href": href})
         else:
             # large number of values, create preview link
             previewQuery = getPreviewQuery(dset_shape["dims"])
             kwargs = {"query": previewQuery}
-            href = getHref(request, dset_uri + '/value', **kwargs)
-            hrefs.append({'rel': 'preview', 'href': href})
+            href = getHref(request, dset_uri + "/value", **kwargs)
+            hrefs.append({"rel": "preview", "href": href})
 
-    resp_json["hrefs"] = hrefs
+    dset_json["hrefs"] = hrefs
 
     if verbose:
         # get allocated size and num_chunks for the dataset if available
-        dset_detail = await getDatasetDetails(app,
-                                              dset_id,
-                                              dset_json["root"],
-                                              bucket=bucket)
+        dset_detail = await getDatasetDetails(
+            app, dset_id, dset_json["root"], bucket=bucket
+        )
         if dset_detail is not None:
             if "num_chunks" in dset_detail:
-                resp_json["num_chunks"] = dset_detail["num_chunks"]
+                dset_json["num_chunks"] = dset_detail["num_chunks"]
             if "allocated_bytes" in dset_detail:
-                resp_json["allocated_size"] = dset_detail["allocated_bytes"]
+                dset_json["allocated_size"] = dset_detail["allocated_bytes"]
             if "lastModified" in dset_detail:
-                resp_json["lastModified"] = dset_detail["lastModified"]
+                dset_json["lastModified"] = dset_detail["lastModified"]
 
-    resp = await jsonResponse(request, resp_json)
+    resp = await jsonResponse(request, dset_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def GET_DatasetType(request):
     """HTTP method to return JSON for dataset's type"""
     log.request(request)
     app = request.app
 
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
     if not dset_id:
         msg = "Missing dataset id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(dset_id, "Dataset"):
         msg = f"Invalid dataset id: {dset_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
@@ -462,21 +444,21 @@
     # get authoritative state for group from DN (even if it's in
     # the meta_cache).
     dset_json = await getObjectJson(app, dset_id, refresh=True, bucket=bucket)
 
     await validateAction(app, domain, dset_id, username, "read")
 
     hrefs = []
-    dset_uri = '/datasets/'+dset_id
+    dset_uri = "/datasets/" + dset_id
     self_uri = dset_uri + "/type"
-    hrefs.append({'rel': 'self', 'href': getHref(request, self_uri)})
-    dset_uri = '/datasets/'+dset_id
-    hrefs.append({'rel': 'owner', 'href': getHref(request, dset_uri)})
-    root_uri = '/groups/' + dset_json["root"]
-    hrefs.append({'rel': 'root', 'href': getHref(request, root_uri)})
+    hrefs.append({"rel": "self", "href": getHref(request, self_uri)})
+    dset_uri = "/datasets/" + dset_id
+    hrefs.append({"rel": "owner", "href": getHref(request, dset_uri)})
+    root_uri = "/groups/" + dset_json["root"]
+    hrefs.append({"rel": "root", "href": getHref(request, root_uri)})
 
     resp_json = {}
     resp_json["type"] = dset_json["type"]
     resp_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, resp_json)
     log.response(request, resp=resp)
@@ -484,26 +466,26 @@
 
 
 async def GET_DatasetShape(request):
     """HTTP method to return JSON for dataset's shape"""
     log.request(request)
     app = request.app
 
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
     if not dset_id:
         msg = "Missing dataset id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(dset_id, "Dataset"):
         msg = f"Invalid dataset id: {dset_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
@@ -514,21 +496,21 @@
     # get authoritative state for dataset from DN (even if it's in
     # the meta_cache).
     dset_json = await getObjectJson(app, dset_id, refresh=True, bucket=bucket)
 
     await validateAction(app, domain, dset_id, username, "read")
 
     hrefs = []
-    dset_uri = '/datasets/'+dset_id
+    dset_uri = "/datasets/" + dset_id
     self_uri = dset_uri + "/shape"
-    hrefs.append({'rel': 'self', 'href': getHref(request, self_uri)})
-    dset_uri = '/datasets/'+dset_id
-    hrefs.append({'rel': 'owner', 'href': getHref(request, dset_uri)})
-    root_uri = '/groups/' + dset_json["root"]
-    hrefs.append({'rel': 'root', 'href': getHref(request, root_uri)})
+    hrefs.append({"rel": "self", "href": getHref(request, self_uri)})
+    dset_uri = "/datasets/" + dset_id
+    hrefs.append({"rel": "owner", "href": getHref(request, dset_uri)})
+    root_uri = "/groups/" + dset_json["root"]
+    hrefs.append({"rel": "root", "href": getHref(request, root_uri)})
 
     resp_json = {}
     resp_json["shape"] = dset_json["shape"]
     resp_json["hrefs"] = hrefs
     resp_json["created"] = dset_json["created"]
     resp_json["lastModified"] = dset_json["lastModified"]
 
@@ -541,15 +523,15 @@
     """HTTP method to update dataset's shape"""
     log.request(request)
     app = request.app
     shape_update = None
     extend = 0
     extend_dim = 0
 
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
     if not dset_id:
         msg = "Missing dataset id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(dset_id, "Dataset"):
         msg = f"Invalid dataset id: {dset_id}"
         log.warn(msg)
@@ -560,25 +542,33 @@
 
     # validate request
     if not request.has_body:
         msg = "PUT shape with no body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
-    data = await request.json()
+    try:
+        data = await request.json()
+    except JSONDecodeError:
+        msg = "Unable to load JSON body"
+        log.warn(msg)
+        raise HTTPBadRequest(reason=msg)
+
     if "shape" not in data and "extend" not in data:
         msg = "PUT shape has no shape or extend key in body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     if "shape" in data:
         shape_update = data["shape"]
         if isinstance(shape_update, int):
             # convert to a list
-            shape_update = [shape_update, ]
+            shape_update = [
+                shape_update,
+            ]
         log.debug(f"shape_update: {shape_update}")
 
     if "extend" in data:
         try:
             extend = int(data["extend"])
         except ValueError:
             msg = "extend value must be integer"
@@ -683,15 +673,20 @@
     await validateUserPassword(app, username, pswd)
 
     if not request.has_body:
         msg = "POST Datasets with no body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
-    body = await request.json()
+    try:
+        body = await request.json()
+    except JSONDecodeError:
+        msg = "Unable to load JSON body"
+        log.warn(msg)
+        raise HTTPBadRequest(reason=msg)
 
     # get domain, check authorization
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
@@ -764,15 +759,17 @@
 
     if "shape" not in body:
         shape_json["class"] = "H5S_SCALAR"
     else:
         shape = body["shape"]
         if isinstance(shape, int):
             shape_json["class"] = "H5S_SIMPLE"
-            dims = [shape, ]
+            dims = [
+                shape,
+            ]
             shape_json["dims"] = dims
             rank = 1
         elif isinstance(shape, str):
             # only valid string value is H5S_NULL
             if shape != "H5S_NULL":
                 msg = "POST Datset with invalid shape value"
                 log.warn(msg)
@@ -854,79 +851,90 @@
                 msg = "Bad Request: maxdims extent can't be smaller "
                 msg += "than shape extent"
                 log.warn(msg)
                 raise HTTPBadRequest(reason=msg)
             else:
                 shape_json["maxdims"].append(maxextent)
 
-    layout = None
+    layout_props = None
     min_chunk_size = int(config.get("min_chunk_size"))
     max_chunk_size = int(config.get("max_chunk_size"))
-    if 'creationProperties' in body:
+    if "creationProperties" in body:
         creationProperties = body["creationProperties"]
-        if 'layout' in creationProperties:
-            layout = creationProperties["layout"]
+        log.debug(f"got creationProperties: {creationProperties}")
+        if "layout" in creationProperties:
+            layout_props = creationProperties["layout"]
+            await validateChunkLayout(app, shape_json, item_size, layout_props, bucket=bucket)
+    else:
+        creationProperties = {}
+
+    if layout_props:
+        if layout_props["class"] in ("H5D_COMPACT", "H5D_CONTIGUOUS"):
+            # treat compact and contiguous as chunked
+            layout_class = "H5D_CHUNKED"
+        else:
+            layout_class = layout_props["class"]
 
-            await validateChunkLayout(app,
-                                      shape_json,
-                                      item_size,
-                                      layout,
-                                      bucket=bucket)
+    elif shape_json["class"] != "H5S_NULL":
+        layout_class = "H5D_CHUNKED"
+    else:
+        layout_class = None
 
-    if layout is None and shape_json["class"] != "H5S_NULL":
-        # default to chunked layout
+    if layout_class:
+        # initialize to H5D_CHUNKED
         layout = {"class": "H5D_CHUNKED"}
+    else:
+        # null space - no layout
+        layout = None
 
-    if layout:
-        layout_class = layout["class"]
+    if layout_props and "dims" in layout_props:
+        chunk_dims = layout_props["dims"]
     else:
-        layout_class = None
+        chunk_dims = None
 
-    if layout_class == 'H5D_CONTIGUOUS_REF':
+    if layout_class == "H5D_CONTIGUOUS_REF":
         kwargs = {"chunk_min": min_chunk_size, "chunk_max": max_chunk_size}
         chunk_dims = getContiguousLayout(shape_json, item_size, **kwargs)
         layout["dims"] = chunk_dims
         log.debug(f"autoContiguous layout: {layout}")
 
-    if layout_class == 'H5D_CHUNKED' and "dims" not in layout:
+    if layout_class == "H5D_CHUNKED" and chunk_dims is None:
         # do autochunking
         chunk_dims = guessChunk(shape_json, item_size)
-        layout["dims"] = chunk_dims
-        log.debug(f"initial autochunk layout: {layout}")
+        log.debug(f"initial autochunk layout: {chunk_dims}")
 
-    if layout_class == 'H5D_CHUNKED':
-        chunk_dims = layout["dims"]
+    if layout_class == "H5D_CHUNKED":
         chunk_size = getChunkSize(chunk_dims, item_size)
 
         msg = f"chunk_size: {chunk_size}, min: {min_chunk_size}, "
         msg += f"max: {max_chunk_size}"
         log.debug(msg)
         # adjust the chunk shape if chunk size is too small or too big
         adjusted_chunk_dims = None
         if chunk_size < min_chunk_size:
             msg = f"chunk size: {chunk_size} less than min size: "
             msg += f"{min_chunk_size}, expanding"
             log.debug(msg)
-            kwargs = {"chunk_min": min_chunk_size,
-                      "layout_class": layout_class}
-            adjusted_chunk_dims = expandChunk(chunk_dims,
-                                              item_size,
-                                              shape_json,
-                                              **kwargs)
+            kwargs = {"chunk_min": min_chunk_size, "layout_class": layout_class}
+            adjusted_chunk_dims = expandChunk(
+                chunk_dims, item_size, shape_json, **kwargs
+            )
         elif chunk_size > max_chunk_size:
             msg = f"chunk size: {chunk_size} greater than max size: "
             msg += f"{max_chunk_size}, shrinking"
             log.debug(msg)
             kwargs = {"chunk_max": max_chunk_size}
             adjusted_chunk_dims = shrinkChunk(chunk_dims, item_size, **kwargs)
         if adjusted_chunk_dims:
             msg = f"requested chunk_dimensions: {chunk_dims} modified "
             msg += f"dimensions: {adjusted_chunk_dims}"
             log.debug(msg)
             layout["dims"] = adjusted_chunk_dims
+        else:
+            layout["dims"] = chunk_dims  # don't need to adjust chunk size
 
         # set partition_count if needed:
         max_chunks_per_folder = int(config.get("max_chunks_per_folder"))
         set_partition = False
         if max_chunks_per_folder > 0:
             if "dims" in shape_json and "dims" in layout:
                 set_partition = True
@@ -953,34 +961,33 @@
                 if max_dims:
                     max_dim = max_dims[i]
                     if max_dim == 0:
                         # don't really know what the ultimate extent
                         # could be, but assume 10^6 for total number of
                         # elements and square-shaped array...
                         MAX_ELEMENT_GUESS = 10.0 ** 6
-                        exp = 1/unlimited_count
+                        exp = 1 / unlimited_count
                         max_dim = int(math.pow(MAX_ELEMENT_GUESS, exp))
                 else:
                     max_dim = shape_dims[i]
-                num_chunks *= math.ceil(max_dim/chunk_dims[i])
+                num_chunks *= math.ceil(max_dim / chunk_dims[i])
 
             if num_chunks > max_chunks_per_folder:
-                partition_count = math.ceil(num_chunks/max_chunks_per_folder)
+                partition_count = math.ceil(num_chunks / max_chunks_per_folder)
                 msg = f"set partition count to: {partition_count}, "
                 msg += f"num_chunks: {num_chunks}"
                 log.info(msg)
                 layout["partition_count"] = partition_count
             else:
                 msg = "do not need chunk partitions, num_chunks: "
                 msg += f"{num_chunks} max_chunks_per_folder: "
                 msg += f"{max_chunks_per_folder}"
                 log.info(msg)
 
-    if layout_class in ('H5D_CHUNKED_REF', 'H5D_CHUNKED_REF_INDIRECT'):
-        chunk_dims = layout["dims"]
+    if layout_class in ("H5D_CHUNKED_REF", "H5D_CHUNKED_REF_INDIRECT"):
         chunk_size = getChunkSize(chunk_dims, item_size)
 
         msg = f"chunk_size: {chunk_size}, min: {min_chunk_size}, "
         msg += f"max: {max_chunk_size}"
         log.debug(msg)
         # nothing to do about inefficencly small chunks, but large chunks
         # can be subdivided
@@ -988,14 +995,15 @@
             msg = f"chunk size: {chunk_size} less than min size: "
             msg += f"{min_chunk_size} for {layout_class} dataset"
             log.warn(msg)
         elif chunk_size > max_chunk_size:
             msg = f"chunk size: {chunk_size} greater than max size: "
             msg += f"{max_chunk_size}, for {layout_class} dataset"
             log.warn(msg)
+        layout["dims"] = chunk_dims
 
     link_id = None
     link_title = None
     if "link" in body:
         link_body = body["link"]
         if "id" in link_body:
             link_id = link_body["id"]
@@ -1006,28 +1014,29 @@
             # verify that the referenced id exists and is in this domain
             # and that the requestor has permissions to create a link
             await validateAction(app, domain, link_id, username, "create")
 
     dset_id = createObjId("datasets", rootid=root_id)
     log.info(f"new  dataset id: {dset_id}")
 
-    dataset_json = {"id": dset_id,
-                    "root": root_id,
-                    "type": datatype,
-                    "shape": shape_json}
+    dataset_json = {
+        "id": dset_id,
+        "root": root_id,
+        "type": datatype,
+        "shape": shape_json,
+    }
 
-    if "creationProperties" in body:
+    if creationProperties:
         # TBD - validate all creationProperties
-        creationProperties = body["creationProperties"]
         if "fillValue" in creationProperties:
             # validate fill value compatible with type
             dt = createDataType(datatype)
             fill_value = creationProperties["fillValue"]
             is_nan = False
-            if dt.kind == 'f':
+            if dt.kind == "f":
                 if isinstance(fill_value, str) and fill_value == "nan":
                     is_nan = True
 
             if is_nan:
                 # use np.nan as fill value
                 # TBD: this needs to be fixed up for compound types
                 log.debug("converting 'nan' to np.nan for fillValue")
@@ -1062,40 +1071,40 @@
             for filter in f_in:
                 if isinstance(filter, int) or isinstance(filter, str):
                     item = getFilterItem(filter)
                     if not item:
                         msg = f"filter {filter} not recognized"
                         log.warn(msg)
                         raise HTTPBadRequest(reason=msg)
-                    
-                    if item['name'] not in supported_filters:
+
+                    if item["name"] not in supported_filters:
                         msg = f"filter {filter} is not supported"
                         log.warn(msg)
                         raise HTTPBadRequest(reason=msg)
                     f_out.append(item)
                 elif isinstance(filter, dict):
                     if "class" not in filter:
                         msg = "expected 'class' key for filter property"
                         log.warn(msg)
                         raise HTTPBadRequest(reason=msg)
-                    if filter['class'] != 'H5Z_FILTER_USER':
-                        item = getFilterItem(filter['class'])
-                    elif 'id' in filter:
-                        item = getFilterItem(filter['id'])
-                    elif 'name' in filter:
-                        item = getFilterItem(filter['name'])
+                    if filter["class"] != "H5Z_FILTER_USER":
+                        item = getFilterItem(filter["class"])
+                    elif "id" in filter:
+                        item = getFilterItem(filter["id"])
+                    elif "name" in filter:
+                        item = getFilterItem(filter["name"])
                     else:
                         item = None
                     if not item:
                         msg = f"filter {filter['class']} not recognized"
                         log.warn(msg)
                         raise HTTPBadRequest(reason=msg)
-                    if 'id' not in filter:
-                        filter['id'] = item['id']
-                    elif item['id'] != filter['id']:
+                    if "id" not in filter:
+                        filter["id"] = item["id"]
+                    elif item["id"] != filter["id"]:
                         msg = f"Expected {filter['class']} to have id: "
                         msg += f"{item['id']} but got {filter['id']}"
                         log.warn(msg)
                         raise HTTPBadRequest(reason=msg)
                     if "name" not in filter:
                         filter["name"] = item["name"]
                     if filter["name"] not in supported_filters:
@@ -1108,14 +1117,15 @@
                     msg = f"Unexpected type for filter: {filter}"
                     log.warn(msg)
                     raise HTTPBadRequest(reason=msg)
             # replace filters with our starndardized list
             log.debug(f"setting filters to: {f_out}")
             creationProperties["filters"] = f_out
 
+        log.debug(f"set dataset json creationPropries: {creationProperties}")
         dataset_json["creationProperties"] = creationProperties
 
     if layout is not None:
         dataset_json["layout"] = layout
 
     log.debug(f"create dataset: {dataset_json}")
     req = getDataNodeUrl(app, dset_id) + "/datasets"
@@ -1143,17 +1153,17 @@
     return resp
 
 
 async def DELETE_Dataset(request):
     """HTTP method to delete a dataset resource"""
     log.request(request)
     app = request.app
-    meta_cache = app['meta_cache']
+    meta_cache = app["meta_cache"]
 
-    dset_id = request.match_info.get('id')
+    dset_id = request.match_info.get("id")
     if not dset_id:
         msg = "Missing dataset id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(dset_id, "Dataset"):
         msg = f"Invalid dataset id: {dset_id}"
         log.warn(msg)
```

### Comparing `hsds-0.7.0b11/hsds/group_dn.py` & `hsds-0.8.0/hsds/group_dn.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # data node of hsds cluster
 #
+
 import time
 import asyncio
 
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPInternalServerError
 from aiohttp.web_exceptions import HTTPNotFound, HTTPServiceUnavailable
 from aiohttp.web import json_response
 
@@ -23,16 +24,15 @@
 from .datanode_lib import get_obj_id, check_metadata_obj, get_metadata_obj
 from .datanode_lib import save_metadata_obj, delete_metadata_obj
 from . import hsds_logger as log
 from . import config
 
 
 async def GET_Group(request):
-    """HTTP GET method to return JSON for /groups/
-    """
+    """HTTP GET method to return JSON for /groups/"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
     group_id = get_obj_id(request)
     if "bucket" in params:
         bucket = params["bucket"]
     else:
@@ -53,22 +53,24 @@
     resp_json["linkCount"] = len(group_json["links"])
     resp_json["attributeCount"] = len(group_json["attributes"])
 
     if "include_links" in params and params["include_links"]:
         resp_json["links"] = group_json["links"]
     if "include_attrs" in params and params["include_attrs"]:
         resp_json["attributes"] = group_json["attributes"]
+    if "creationProperties" in group_json:
+        resp_json["creationProperties"] = group_json["creationProperties"]
 
     resp = json_response(resp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def POST_Group(request):
-    """ Handler for POST /groups"""
+    """Handler for POST /groups"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
     if not request.has_body:
         msg = "POST_Group with no body"
         log.warn(msg)
@@ -105,20 +107,25 @@
         msg = "Invalid root_id: " + root_id
         log.error(msg)
         raise HTTPInternalServerError()
 
     # ok - all set, create group obj
     now = time.time()
 
-    group_json = {"id": group_id,
-                  "root": root_id,
-                  "created": now,
-                  "lastModified": now,
-                  "links": {},
-                  "attributes": {}}
+    group_json = {
+        "id": group_id,
+        "root": root_id,
+        "created": now,
+        "lastModified": now,
+        "links": {},
+        "attributes": {},
+    }
+
+    if "creationProperties" in body:
+        group_json["creationProperties"] = body["creationProperties"]
 
     kwargs = {"bucket": bucket, "notify": True, "flush": True}
     await save_metadata_obj(app, group_id, group_json, **kwargs)
 
     # formulate response
     resp_json = {}
     resp_json["id"] = group_id
@@ -130,25 +137,25 @@
 
     resp = json_response(resp_json, status=201)
     log.response(request, resp=resp)
     return resp
 
 
 async def PUT_Group(request):
-    """ Handler for PUT /groups
-        Used to flush all objects under a root group to S3
+    """Handler for PUT /groups
+    Used to flush all objects under a root group to S3
     """
 
     flush_time_out = config.get("s3_sync_interval") * 2
     flush_sleep_interval = config.get("flush_sleep_interval")
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
-    root_id = request.match_info.get('id')
+    root_id = request.match_info.get("id")
     if "bucket" in params:
         bucket = params["bucket"]
     else:
         bucket = None
     log.info(f"PUT group (flush): {root_id}  bucket: {bucket}")
     # don't really need bucket param since the dirty ids know which bucket
     # they should write too
@@ -204,47 +211,51 @@
     if len(flush_set) > 0:
         msg = f"flushop - {len(flush_set)} items not updated after "
         msg += f"{flush_time_out} seconds"
         log.warn(msg)
         log.debug(f"flush set: {flush_set}")
         raise HTTPServiceUnavailable()
 
-    rsp_json = {"id": app['id']}  # return the node id
+    rsp_json = {"id": app["id"]}  # return the node id
     log.debug(f"flush returning: {rsp_json}")
     resp = json_response(rsp_json, status=200)
     log.response(request, resp=resp)
     return resp
 
 
 async def DELETE_Group(request):
-    """HTTP DELETE method for /groups/
-    """
+    """HTTP DELETE method for /groups/"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
     group_id = get_obj_id(request)
 
     if not isValidUuid(group_id, obj_class="group"):
         log.error(f"Unexpected group_id: {group_id}")
         raise HTTPInternalServerError()
 
     if "bucket" in params:
         bucket = params["bucket"]
     else:
-        bucket = None
+        bucket = app["bucket_name"]
+
+    if not bucket:
+        msg = "DELETE_Group - bucket not set"
+        log.error(msg)
+        raise HTTPBadRequest(reason=msg)
 
     log.info(f"DELETE group: {group_id} bucket: {bucket}")
 
     # verify the id exist
     obj_found = await check_metadata_obj(app, group_id, bucket=bucket)
     if not obj_found:
         log.debug(f"delete called on non-exsistet obj: {group_id}")
         raise HTTPNotFound()
 
-    log.debug("deleting group: {}".format(group_id))
+    log.debug(f"deleting group: {group_id}, bucket:{bucket}")
 
     if "Notify" in params and not params["Notify"]:
         notify = False
     else:
         notify = True
 
     await delete_metadata_obj(app, group_id, bucket=bucket, notify=notify)
@@ -253,19 +264,18 @@
 
     resp = json_response(resp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def POST_Root(request):
-    """ Notify root that content in the domain has been modified.
-    """
+    """Notify root that content in the domain has been modified."""
     log.request(request)
     app = request.app
-    root_id = request.match_info.get('id')
+    root_id = request.match_info.get("id")
     if not root_id:
         log.error("missing id in request")
         raise HTTPInternalServerError()
     if not isSchema2Id(root_id):
         log.error(f"expected schema2 id but got: {root_id}")
         raise HTTPInternalServerError()
     if not isRootObjId(root_id):
```

### Comparing `hsds-0.7.0b11/hsds/group_sn.py` & `hsds-0.8.0/hsds/group_sn.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # group handler for service node of hsds cluster
 #
 
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPForbidden, HTTPNotFound
+from json import JSONDecodeError
 
 from .util.httpUtil import http_post, http_put, http_delete, getHref
 from .util.httpUtil import jsonResponse
 from .util.idUtil import isValidUuid, getDataNodeUrl, createObjId
 from .util.authUtil import getUserPasswordFromRequest, aclCheck
 from .util.authUtil import validateUserPassword
 from .util.domainUtil import getDomainFromRequest, isValidDomain
@@ -33,15 +34,17 @@
     app = request.app
     params = request.rel_url.query
 
     h5path = None
     getAlias = False
     include_links = False
     include_attrs = False
-    group_id = request.match_info.get('id')
+
+    group_id = request.match_info.get("id")
+
     if not group_id and "h5path" not in params:
         # no id, or path provided, so bad request
         msg = "Missing group id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if group_id:
         log.info(f"GET_Group, id: {group_id}")
@@ -51,96 +54,101 @@
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         if "getalias" in params:
             if params["getalias"]:
                 getAlias = True
     if "h5path" in params:
         h5path = params["h5path"]
-        if not group_id and h5path[0] != '/':
+        if not group_id and h5path[0] != "/":
             msg = "h5paths must be absolute if no parent id is provided"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         log.info(f"GET_Group, h5path: {h5path}")
     if "include_links" in params and params["include_links"]:
         include_links = True
     if "include_attrs" in params and params["include_attrs"]:
         include_attrs = True
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     bucket = getBucketForDomain(domain)
 
-    if h5path and h5path[0] == '/':
+    if h5path and h5path[0] == "/":
         # ignore the request path id (if given) and start
         # from root group for absolute paths
 
         domain_json = await getDomainJson(app, domain)
         verifyRoot(domain_json)
         group_id = domain_json["root"]
 
     if h5path:
         # throws 404 if not found
-        kwargs = {"bucket": bucket}
-        group_id = await getObjectIdByPath(app, group_id, h5path, **kwargs)
+        kwargs = {"bucket": bucket, "domain": domain}
+        group_id, domain, obj_json = await getObjectIdByPath(app, group_id, h5path, **kwargs)
+
         if not isValidUuid(group_id, "Group"):
             msg = f"No group exist with the path: {h5path}"
             log.warn(msg)
             raise HTTPNotFound()
-        log.info(f"get group_id: {group_id} from h5path: {h5path}")
+        log.info(f"get group_id: {group_id} from h5path: {h5path} in the domain: {domain}")
 
     # verify authorization to read the group
     await validateAction(app, domain, group_id, username, "read")
 
     # get authoritative state for group from DN (even if it's in the
     # meta_cache).
-    kwargs = {"refresh": True,
-              "include_links": include_links,
-              "include_attrs": include_attrs,
-              "bucket": bucket}
+    kwargs = {
+        "refresh": True,
+        "include_links": include_links,
+        "include_attrs": include_attrs,
+        "bucket": bucket,
+    }
+
     group_json = await getObjectJson(app, group_id, **kwargs)
     log.debug(f"domain from request: {domain}")
+
     group_json["domain"] = getPathForDomain(domain)
     if bucket:
         group_json["bucket"] = bucket
 
     if getAlias:
         root_id = group_json["root"]
         alias = []
         if group_id == root_id:
-            alias.append('/')
+            alias.append("/")
         else:
-            id_map = {root_id: '/'}
+            id_map = {root_id: "/"}
             kwargs = {"bucket": bucket, "tgt_id": group_id}
             h5path = await getPathForObjectId(app, root_id, id_map, **kwargs)
             if h5path:
                 alias.append(h5path)
         group_json["alias"] = alias
 
     hrefs = []
-    group_uri = '/groups/'+group_id
+    group_uri = "/groups/" + group_id
     href = getHref(request, group_uri)
-    hrefs.append({'rel': 'self', 'href': href})
-    href = getHref(request, group_uri+'/links')
-    hrefs.append({'rel': 'links', 'href': href})
-    root_uri = '/groups/' + group_json["root"]
+    hrefs.append({"rel": "self", "href": href})
+    href = getHref(request, group_uri + "/links")
+    hrefs.append({"rel": "links", "href": href})
+    root_uri = "/groups/" + group_json["root"]
     href = getHref(request, root_uri)
-    hrefs.append({'rel': 'root', 'href': href})
-    href = getHref(request, '/')
-    hrefs.append({'rel': 'home', 'href': href})
-    href = getHref(request, group_uri+'/attributes')
-    hrefs.append({'rel': 'attributes', 'href': href})
+    hrefs.append({"rel": "root", "href": href})
+    href = getHref(request, "/")
+    hrefs.append({"rel": "home", "href": href})
+    href = getHref(request, group_uri + "/attributes")
+    hrefs.append({"rel": "attributes", "href": href})
     group_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, group_json)
     log.response(request, resp=resp)
     return resp
 
 
@@ -165,16 +173,25 @@
     # throws exception if not allowed
     aclCheck(app, domain_json, "create", username)
 
     verifyRoot(domain_json)
 
     link_id = None
     link_title = None
+    creation_props = None
+
     if request.has_body:
-        body = await request.json()
+
+        try:
+            body = await request.json()
+        except JSONDecodeError:
+            msg = "Unable to load JSON body"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
+
         log.info(f"POST Group body: {body}")
         if body:
             if "link" in body:
                 link_body = body["link"]
                 log.debug(f"link_body: {link_body}")
                 if "id" in link_body:
                     link_id = link_body["id"]
@@ -183,24 +200,28 @@
                 if link_id and link_title:
                     log.debug(f"link id: {link_id}")
                     # verify that the referenced id exists and is in this
                     # domainand that the requestor has permissions to create
                     # a link
                     act = "create"
                     await validateAction(app, domain, link_id, username, act)
-            if not link_id or not link_title:
-                log.warn(f"POST Group body with no link: {body}")
+                if not link_id or not link_title:
+                    log.warn(f"POST Group body with no link: {body}")
+            if "creationProperties" in body:
+                creation_props = body["creationProperties"]
 
     # get again in case cache was invalidated
     domain_json = await getDomainJson(app, domain)
 
     root_id = domain_json["root"]
     group_id = createObjId("groups", rootid=root_id)
     log.info(f"new  group id: {group_id}")
     group_json = {"id": group_id, "root": root_id}
+    if creation_props:
+        group_json["creationProperties"] = creation_props
     log.debug(f"create group, body: {group_json}")
     req = getDataNodeUrl(app, group_id) + "/groups"
     params = {}
     if bucket:
         params["bucket"] = bucket
 
     group_json = await http_post(app, req, data=group_json, params=params)
@@ -223,17 +244,17 @@
     return resp
 
 
 async def DELETE_Group(request):
     """HTTP method to delete a group resource"""
     log.request(request)
     app = request.app
-    meta_cache = app['meta_cache']
+    meta_cache = app["meta_cache"]
 
-    group_id = request.match_info.get('id')
+    group_id = request.match_info.get("id")
     if not group_id:
         msg = "Missing group id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(group_id, "Group"):
         msg = f"Invalid group id: {group_id}"
         log.warn(msg)
```

### Comparing `hsds-0.7.0b11/hsds/headnode.py` & `hsds-0.8.0/hsds/headnode.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,44 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # Head node of hsds cluster
 #
+
 import asyncio
 import os
 import time
 
 from aiohttp.web import Application, StreamResponse, run_app, json_response
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPInternalServerError
 
 from . import config
 from .util.timeUtil import unixTimeToUTC, elapsedTime
 from .util.idUtil import createNodeId
 from . import hsds_logger as log
 from .util import query_marathon as marathonClient
 
-NODE_STAT_KEYS = ("cpu", "diskio", "memory", "log_stats", "disk", "netio",
-                  "req_count", "s3_stats", "azure_stats", "chunk_cache_stats")
+NODE_STAT_KEYS = (
+    "cpu",
+    "diskio",
+    "memory",
+    "log_stats",
+    "disk",
+    "netio",
+    "req_count",
+    "s3_stats",
+    "azure_stats",
+    "chunk_cache_stats",
+)
 
 
 class Node:
-    def __init__(self, node_id=None,
-                 node_type=None, node_host=None, node_port=None):
+    def __init__(self, node_id=None, node_type=None, node_host=None, node_port=None):
         self._id = node_id
         self._type = node_type
         self._host = node_host
         self._port = node_port
         now = time.time()
         self._create_time = now
         self._last_poll = now
@@ -116,15 +126,15 @@
         return False
 
     log.debug("cluster is ready")
     return True
 
 
 def removeNode(app, host=None, port=None):
-    dead_node_ids = app['dead_node_ids']
+    dead_node_ids = app["dead_node_ids"]
     nodes = app["nodes"]
     remove_id = None
     for node_id in nodes:
         node = nodes[node_id]
         if node.port == port and node.host == host:
             remove_id = node_id
             break  # only expecting one at most
@@ -134,73 +144,73 @@
 
 
 async def info(request):
     """HTTP Method to return node state to caller"""
     log.request(request)
     app = request.app
     resp = StreamResponse()
-    resp.headers['Content-Type'] = 'application/json'
+    resp.headers["Content-Type"] = "application/json"
     if await isClusterReady(app):
-        cluster_state = 'READY'
+        cluster_state = "READY"
     else:
-        cluster_state = 'WAITING'
+        cluster_state = "WAITING"
     answer = {}
     # copy relevant entries from state dictionary to response
-    answer['id'] = request.app['id']
-    answer['start_time'] = unixTimeToUTC(app['start_time'])
-    answer['last_health_check'] = unixTimeToUTC(app['last_health_check'])
-    answer['up_time'] = elapsedTime(app['start_time'])
-    answer['cluster_state'] = cluster_state
-    answer['bucket_name'] = app['bucket_name']
-    answer['target_sn_count'] = await getTargetNodeCount(app, "sn")
-    answer['active_sn_count'] = getActiveNodeCount(app, "sn")
-    answer['target_dn_count'] = await getTargetNodeCount(app, "dn")
-    answer['active_dn_count'] = getActiveNodeCount(app, "dn")
+    answer["id"] = request.app["id"]
+    answer["start_time"] = unixTimeToUTC(app["start_time"])
+    answer["last_health_check"] = unixTimeToUTC(app["last_health_check"])
+    answer["up_time"] = elapsedTime(app["start_time"])
+    answer["cluster_state"] = cluster_state
+    answer["bucket_name"] = app["bucket_name"]
+    answer["target_sn_count"] = await getTargetNodeCount(app, "sn")
+    answer["active_sn_count"] = getActiveNodeCount(app, "sn")
+    answer["target_dn_count"] = await getTargetNodeCount(app, "dn")
+    answer["active_dn_count"] = getActiveNodeCount(app, "dn")
 
     resp = json_response(answer)
     log.response(request, resp=resp)
     return resp
 
 
 async def register(request):
-    """ HTTP method for nodes to register with head node"""
+    """HTTP method for nodes to register with head node"""
     app = request.app
     if not request.has_body:
         msg = "register missing body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     body = await request.json()
     log.info(f"register request body: {body}")
     node_host = None
     node_port = None
     node_type = None
     node_id = None
-    if 'id' not in body:
+    if "id" not in body:
         msg = "Missing 'id'"
         log.response(request, code=400, message=msg)
         raise HTTPBadRequest(reason=msg)
-    node_id = body['id']
-    if 'node_type' not in body:
+    node_id = body["id"]
+    if "node_type" not in body:
         msg = "missing key 'node_type'"
         log.response(request, code=400, message=msg)
         raise HTTPBadRequest(reason=msg)
-    node_type = body['node_type']
-    if node_type not in ('sn', 'dn'):
+    node_type = body["node_type"]
+    if node_type not in ("sn", "dn"):
         msg = f"invalid node_type: {node_type}"
         log.response(request, code=400, message=msg)
         raise HTTPBadRequest(reason=msg)
-    if 'port' not in body:
+    if "port" not in body:
         msg = "missing key 'port'"
         log.response(request, code=400, message=msg)
         raise HTTPBadRequest(reason=msg)
-    node_port = body['port']
+    node_port = body["port"]
 
-    if 'ip' not in body:
+    if "ip" not in body:
         log.debug("register - get ip/port from request.transport")
-        peername = request.transport.get_extra_info('peername')
+        peername = request.transport.get_extra_info("peername")
         if peername is None:
             msg = "Can not determine caller IP"
             log.error(msg)
             raise HTTPBadRequest(reason=msg)
         if peername[0] is None or peername[0] in ("::1", "127.0.0.1"):
             node_host = "localhost"
         else:
@@ -208,16 +218,16 @@
     else:
         # Specify the ip is useful in docker / DCOS situations, where in
         # certain situations a docker private network IP might be used
         node_host = body["ip"]
 
     log.info(f"register host: {node_host}, port: {node_port}")
 
-    nodes = app['nodes']
-    dead_node_ids = app['dead_node_ids']
+    nodes = app["nodes"]
+    dead_node_ids = app["dead_node_ids"]
 
     if node_id in nodes:
         # already registered?
         node = nodes[node_id]
         if node_type != node.type:
             msg = f"Unexpected node_type {node_type} (expected: {node.type}) "
             msg += f"for node_id: {node_id}"
@@ -235,22 +245,26 @@
             raise HTTPBadRequest(reason=msg)
         node.poll_update()  # note that the node has checked in
     elif node_id in dead_node_ids:
         log.error(f"unexpected register request from node id: {node_id}")
         raise HTTPInternalServerError()
     else:
         log.info(f"Node {node_id} is unknown, new node coming online.")
-        node = Node(node_id=node_id, node_type=node_type,
-                    node_host=node_host, node_port=node_port)
+        node = Node(
+            node_id=node_id,
+            node_type=node_type,
+            node_host=node_host,
+            node_port=node_port,
+        )
         # delete any existing node with the same port
         removeNode(app, host=node_host, port=node_port)
         nodes[node_id] = node
 
     resp = StreamResponse()
-    resp.headers['Content-Type'] = 'application/json'
+    resp.headers["Content-Type"] = "application/json"
     answer = {}
 
     if await isClusterReady(app):
         answer["cluster_state"] = "READY"
     else:
         answer["cluster_state"] = "WAITING"
     sn_urls = []
@@ -293,63 +307,63 @@
     log.response(request, resp=resp)
     return resp
 
 
 async def nodestate(request):
     """HTTP method to return information about registered nodes"""
     log.request(request)
-    node_id = request.match_info.get('node_id', '*')
-    node_type = request.match_info.get('node_type', '*')
+    node_id = request.match_info.get("node_id", "*")
+    node_type = request.match_info.get("node_type", "*")
 
     log.info(f"nodestate/{node_type}/{node_id}")
 
     app = request.app
     resp = StreamResponse()
-    resp.headers['Content-Type'] = 'application/json'
+    resp.headers["Content-Type"] = "application/json"
     nodes = app["nodes"]
 
-    if node_id == '*':
+    if node_id == "*":
         info_list = []
         for node_id in nodes:
             node = nodes[node_id]
             if node.type == node_type or node_type == "*":
                 info_list.append(node.get_info())
         answer = {"nodes": info_list}
         log.debug(f"returning nodestate for {len(nodes)} nodes")
     elif node_id in nodes:
         node = nodes[node_id]
         answer = {}
         answer["node"] = node.get_info()
     if await isClusterReady(app):
-        cluster_state = 'READY'
+        cluster_state = "READY"
     else:
-        cluster_state = 'WAITING'
+        cluster_state = "WAITING"
     answer["cluster_state"] = cluster_state
     resp = json_response(answer)
     log.response(request, resp=resp)
     return resp
 
 
 async def nodeinfo(request):
     """HTTP method to return node stats (cpu usage, request count, errors,
-        etc.) about registed nodes
+    etc.) about registed nodes
     """
     log.request(request)
     node_stat_keys = NODE_STAT_KEYS
-    stat_key = request.match_info.get('statkey', '*')
-    if stat_key != '*':
+    stat_key = request.match_info.get("statkey", "*")
+    if stat_key != "*":
         if stat_key not in node_stat_keys:
             msg = f"nodeinfo - invalid key: {stat_key}"
             log.warn(msg)
             raise HTTPBadRequest(msg)
         node_stat_keys = (stat_key,)
 
     app = request.app
     resp = StreamResponse()
-    resp.headers['Content-Type'] = 'application/json'
+    resp.headers["Content-Type"] = "application/json"
 
     dn_count = 0
     sn_count = 0
 
     answer = {}
     nodes = app["nodes"]
 
@@ -375,33 +389,37 @@
             else:
                 node_number = dn_count
                 dn_count += 1
             stats_field = node.stats[stat_key]
             for k in stats_field:
                 if k not in stats:
                     stats[k] = {}
-                    stats[k]["sn"] = [0, ] * sn_count
-                    stats[k]["dn"] = [0, ] * dn_count
+                    stats[k]["sn"] = [
+                        0,
+                    ] * sn_count
+                    stats[k]["dn"] = [
+                        0,
+                    ] * dn_count
                 stats[k][node.type][node_number] = stats_field[k]
         answer[stat_key] = stats
 
     resp = json_response(answer)
     log.response(request, resp=resp)
     return resp
 
 
 async def getTargetNodeCount(app, node_type):
 
     if node_type == "dn":
-        key = 'target_sn_count'
+        key = "target_sn_count"
     elif node_type == "sn":
         key = "target_sn_count"
     else:
         raise KeyError()
-    if 'key' not in app:
+    if "key" not in app:
         if "is_dcos" in app:
             marathon = marathonClient.MarathonClient(app)
             if node_type == "dn":
                 app[key] = int(await marathon.getDNInstances())
             else:
                 app[key] = int(await marathon.getDNInstances())
         else:
@@ -418,21 +436,21 @@
             continue
         if node.is_healthy:
             count += 1
     return count
 
 
 async def init():
-    """Intitialize application and return app object """
+    """Intitialize application and return app object"""
 
     # setup log config
     log_level = config.get("log_level")
     prefix = config.get("log_prefix")
     log_timestamps = config.get("log_timestamps", default=False)
-    log.setLogConfig(log_level, prefix=prefix, timestamps=log_timestamps)     
+    log.setLogConfig(log_level, prefix=prefix, timestamps=log_timestamps)
 
     app = Application()
 
     # set a bunch of global state
     app["id"] = createNodeId("head")
 
     bucket_name = config.get("bucket_name")
@@ -456,44 +474,43 @@
         log.info("not setting is_dcos")
 
     app["nodes"] = nodes
     app["dead_node_ids"] = set()
     app["start_time"] = int(time.time())  # seconds after epoch
     app["last_health_check"] = 0
     app["max_task_count"] = config.get("max_task_count")
-    app.router.add_get('/', info)
-    app.router.add_get('/nodestate', nodestate)
-    app.router.add_get('/nodestate/{nodetype}', nodestate)
-    app.router.add_get('/nodestate/{nodetype}/{nodenumber}', nodestate)
-    app.router.add_get('/nodeinfo', nodeinfo)
-    app.router.add_get('/nodeinfo/{statkey}', nodeinfo)
-    app.router.add_get('/info', info)
-    app.router.add_post('/register', register)
+    app.router.add_get("/", info)
+    app.router.add_get("/nodestate", nodestate)
+    app.router.add_get("/nodestate/{nodetype}", nodestate)
+    app.router.add_get("/nodestate/{nodetype}/{nodenumber}", nodestate)
+    app.router.add_get("/nodeinfo", nodeinfo)
+    app.router.add_get("/nodeinfo/{statkey}", nodeinfo)
+    app.router.add_get("/info", info)
+    app.router.add_post("/register", register)
 
     return app
 
 
 def create_app():
-    """Create servicenode aiohttp application
-    """
+    """Create servicenode aiohttp application"""
     log.info("Head node initializing")
     loop = asyncio.get_event_loop()
     app = loop.run_until_complete(init())
     return app
 
 
 def main():
     """
-       Main - entry point for headnode
+    Main - entry point for headnode
     """
     app = create_app()
 
     # create a client Session here so that all client requests
     #   will share the same connection pool
 
     head_port = config.get("head_port")
     log.info(f"Starting service on port: {head_port}")
     run_app(app, port=int(head_port))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `hsds-0.7.0b11/hsds/hsds_app.py` & `hsds-0.8.0/hsds/hsds_app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,128 +1,186 @@
 import os
 import sys
-import signal
+from pathlib import Path
+import site
 import subprocess
 import time
-import uuid
 import queue
 import threading
 import logging
+from shutil import which
 
 
 def _enqueue_output(out, queue, loglevel):
-    for line in iter(out.readline, b''):
-        # filter lines by loglevel
-        words = line.split()
-        put_line = True
-
-        if loglevel != logging.DEBUG:
-            if len(words) >= 2:
-                # format should be "node_name log_level> msg"
-                level = words[1][:-1]
-                if loglevel == logging.INFO:
-                    if level == "DEBUG":
-                        put_line = False
-                elif loglevel == logging.WARN or loglevel == logging.WARNING:
-                    if not level.startswith("WARN") and level != "ERROR":
-                        put_line = False
-                elif loglevel == logging.ERROR:
-                    if level != "ERROR":
-                        put_line = False
-        put_line = True
-        if put_line:
-            queue.put(line)
-    logging.debug("enqueu_output close()")
-    out.close()
+    try:
+        for line in iter(out.readline, b""):
+            # filter lines by loglevel
+            words = line.split()
+            put_line = True
+
+            if loglevel != logging.DEBUG:
+                if len(words) >= 2:
+                    # format should be "node_name log_level> msg"
+                    level = words[1][:-1]
+                    if loglevel == logging.INFO:
+                        if level == "DEBUG":
+                            put_line = False
+                    elif loglevel == logging.WARN or loglevel == logging.WARNING:
+                        if not level.startswith("WARN") and level != "ERROR":
+                            put_line = False
+                    elif loglevel == logging.ERROR:
+                        if level != "ERROR":
+                            put_line = False
+            put_line = True
+            if put_line:
+                queue.put(line)
+        logging.debug("_enqueue_output close()")
+        out.close()
+    except ValueError as ve:
+        logging.warn(f"_enqueue_output - ValueError (handle closed?): {ve}")
+    except Exception as e:
+        logging.error(f"_enqueue_output - Unexpected exception {type(e)}: {e}")
+
+
+def get_cmd_dir():
+    """Return directory where hsds console shortcuts are."""
+    hsds_shortcut = "hsds-servicenode"
+
+    user_bin_dir = os.path.join(site.getuserbase(), "bin")
+    if os.path.isdir(user_bin_dir):
+        logging.debug(f"userbase bin_dir: {user_bin_dir}")
+        if os.path.isfile(os.path.join(user_bin_dir, hsds_shortcut)):
+            logging.info(f"using cmd_dir: {user_bin_dir}")
+            return user_bin_dir
+
+    logging.debug(f"looking for {hsds_shortcut} in PATH env var folders")
+    cmd = which(hsds_shortcut, mode=os.F_OK | os.R_OK)
+    if cmd is not None:
+        cmd_dir = os.path.dirname(cmd)
+        logging.info(f"using cmd_dir: {cmd_dir}")
+        return cmd_dir
+
+    sys_bin_dir = os.path.join(sys.exec_prefix, "bin")
+    if os.path.isdir(sys_bin_dir):
+        logging.debug(f"sys bin_dir: {sys_bin_dir}")
+        if os.path.isfile(os.path.join(sys_bin_dir, hsds_shortcut)):
+            logging.info(f"using cmd_dir: {sys_bin_dir}")
+            return sys_bin_dir
+
+    # fall back to just use __file__.parent
+    bin_dir = Path(__file__).parent
+    logging.info(f"no userbase or syspath found - using: {bin_dir}")
+    return bin_dir
 
 
 class HsdsApp:
     """
     Class to initiate and manage sub-process HSDS service
     """
 
-    def __init__(self, username=None, 
-                password=None, password_file=None, logger=None, 
-                log_level=None, dn_count=1, logfile=None, 
-                socket_dir=None, config_dir=None, readonly=False):
+    def __init__(
+        self,
+        username=None,
+        password=None,
+        password_file=None,
+        logger=None,
+        log_level=None,
+        dn_count=1,
+        logfile=None,
+        root_dir=None,
+        socket_dir=None,
+        host=None,
+        sn_port=None,
+        config_dir=None,
+        readonly=False,
+        islambda=False,
+    ):
         """
         Initializer for class
         """
 
-        """
-        # Using tempdir is causing a unicode exception
-        # See: https://bugs.python.org/issue32958
-        self._tempdir = tempfile.TemporaryDirectory()
-        tmp_dir = self._tempdir.name
-        """
-        # create a random dirname if one is not supplied
-        if socket_dir:
-            if socket_dir[-1] != '/':
-                socket_dir += '/'
-        else:
-            tmp_dir = "/tmp"  # TBD: will this work on windows?
-            rand_name = uuid.uuid4().hex[:8]
-            socket_dir = f"{tmp_dir}/hs{rand_name}/"  # TBD: use temp dir
         self._dn_urls = []
         self._socket_paths = []
-        self._processes = []
+        self._processes = {}
         self._queues = []
         self._threads = []
         self._dn_count = dn_count
         self._username = username
         self._password = password
         self._password_file = password_file
         self._logfile = logfile
         self._loglevel = log_level
         self._readonly = readonly
+        self._islambda = islambda
         self._ready = False
         self._config_dir = config_dir
+        self._cmd_dir = get_cmd_dir()
 
         if logger is None:
             self.log = logging
         else:
             self.log = logger
 
-        if not os.path.isdir(socket_dir):
+        # create a random dirname if one is not supplied
+        if not socket_dir and not host:
+            raise ValueError("socket_dir or host needs to be set")
+        if host and not sn_port:
+            raise ValueError("sn_port not set")
+
+        if socket_dir is not None and not os.path.isdir(socket_dir):
             os.mkdir(socket_dir)
 
-        self.log.debug(f"HsdsApp init - Using socketdir: {socket_dir}")
+        if root_dir:
+            if not os.path.isdir(root_dir):
+                raise FileNotFoundError(f"storage directory: '{root_dir}' not found")
+            self._root_dir = os.path.abspath(root_dir)
+        else:
+            self._root_dir = None
 
         # url-encode any slashed in the socket dir
-        socket_url = ""
-        for ch in socket_dir:
-            if ch == '/':
-                socket_url += "%2F"
-            else:
-                socket_url += ch
+        if socket_dir:
+            if not socket_dir.endswith(os.path.sep):
+                socket_dir += os.path.sep
+            self.log.debug(f"HsdsApp init - Using socketdir: {socket_dir}")
+            socket_url = ""
+            for ch in socket_dir:
+                if ch == "/" or ch == "\\":
+                    socket_url += "%2F"
+                else:
+                    socket_url += ch
+            sn_url = f"http+unix://{socket_url}sn_1.sock"
 
-        for i in range(dn_count):
-            socket_name = f"dn_{(i+1)}.sock"
-            dn_url = f"http+unix://{socket_url}{socket_name}"
-            self._dn_urls.append(dn_url)
-            self._socket_paths.append(f"{socket_dir}{socket_name}")
+            for i in range(dn_count):
+                socket_name = f"dn_{(i+1)}.sock"
+                dn_url = f"http+unix://{socket_url}{socket_name}"
+                self._dn_urls.append(dn_url)
+                self._socket_paths.append(f"{socket_dir}{socket_name}")
+            self._socket_paths.append(f"{socket_dir}sn_1.sock")
+        else:
+            # setup TCP/IP endpoints
+            sn_url = f"http://{host}:{sn_port}"
+            dn_port = 6101  # TBD: pull this from config
+            for i in range(dn_count):
+                dn_url = f"http://{host}:{dn_port+i}"
+                self._dn_urls.append(dn_url)
 
         # sort the ports so that node_number can be determined based on dn_url
         self._dn_urls.sort()
-        self._endpoint = f"http+unix://{socket_url}sn_1.sock"
-        self._socket_paths.append(f"{socket_dir}sn_1.sock")
-        self._rangeget_url = f"http+unix://{socket_url}rangeget.sock"
-        self._socket_paths.append(f"{socket_dir}rangeget.sock")
+        self._endpoint = sn_url
 
     @property
     def endpoint(self):
         return self._endpoint
 
     @property
     def ready(self):
         return self._ready
 
     def print_process_output(self):
-        """ print any queue output from sub-processes
-        """
+        """print any queue output from sub-processes"""
         if self._logfile:
             f = open(self._logfile, "a")
         else:
             f = sys.stdout
 
         while True:
             got_output = False
@@ -142,109 +200,131 @@
                 break  # all queues empty for now
         if self._logfile:
             f.close()
 
     def check_processes(self):
         # self.log.debug("check processes")
         self.print_process_output()
-        for p in self._processes:
+        for pname in self._processes:
+            p = self._processes[pname]
             if p.poll() is not None:
                 result = p.communicate()
-                msg = f"process {p.args[0]} ended, result: {result}"
+                msg = f"process {pname} ended, result: {result}"
                 self.log.warn(msg)
                 # TBD - restart failed process
 
     def run(self):
-        """ startup hsds processes
-        """
+        """startup hsds processes"""
         if self._processes:
             # just check process state and restart if necessary
             self.check_processes()
             return
 
         dn_urls_arg = ""
         for dn_url in self._dn_urls:
             if dn_urls_arg:
-                dn_urls_arg += ','
+                dn_urls_arg += ","
             dn_urls_arg += dn_url
 
-        pout = subprocess.PIPE   # will pipe to parent
-        # create processes for count dn nodes, sn node, and rangeget node
-        count = self._dn_count + 2  # plus 2 for rangeget proxy and sn
+        pout = subprocess.PIPE  # will pipe to parent
+        # create processes for count dn nodes and sn nodes
+        count = self._dn_count + 1  # plus 1 for sn
         # set PYTHONUNBUFFERED so we can get any output immediately
         os.environ["PYTHONUNBUFFERED"] = "1"
         # TODO: don't modify parent process env, use os.environ.copy(), set, and popen(env=)
 
-        common_args = ["--standalone", ]
+        common_args = [
+            "--standalone",
+        ]
         common_args.append(f"--dn_urls={dn_urls_arg}")
-        common_args.append(f"--rangeget_url={self._rangeget_url}")
         common_args.append(f"--hsds_endpoint={self._endpoint}")
+        if self._islambda:
+            # base boto packages installed in AWS image conflicting with aiobotocore
+            # see: https://github.com/aio-libs/aiobotocore/issues/862
+            # This command line argument will tell the sub-processes to remove
+            # sitepackage libs from their path before importing aiobotocore
+            common_args.append("--removesitepackages")
         # common_args.append("--server_name=Direct Connect (HSDS)")
-        common_args.append("--use_socket")
+        if len(self._socket_paths) > 0:
+            common_args.append("--use_socket")
         if self._readonly:
             common_args.append("--readonly")
         if self._config_dir:
-            common_args.append(f"--config-dir={self._config_dir}")
+            common_args.append(f"--config_dir={self._config_dir}")
+        if self._root_dir:
+            common_args.append(f"--root_dir={self._root_dir}")
         if self._loglevel:
             common_args.append(f"--log_level={self._loglevel}")
 
         py_exe = sys.executable
-        cmd_dir = os.path.join(sys.exec_prefix, "bin")
+        cmd_path = os.path.join(self._cmd_dir, "hsds-node")
+        if not os.path.isfile(cmd_path):
+            # search corresponding location for windows installs
+            cmd_path = os.path.join(sys.exec_prefix, "Scripts")
+            cmd_path = os.path.join(cmd_path, "hsds-node-script.py")
+            if not os.path.isfile(cmd_path):
+                raise FileNotFoundError("can't find hsds-node executable")
+
         for i in range(count):
             if i == 0:
                 # args for service node
-                pargs = [py_exe,
-                         os.path.join(cmd_dir, "hsds-servicenode"),
-                         "--log_prefix=sn "]
+                pname = "sn"
+                pargs = [py_exe, cmd_path, "--node_type=sn", "--log_prefix=sn "]
                 if self._username:
                     pargs.append(f"--hs_username={self._username}")
                 if self._password:
                     pargs.append(f"--hs_password={self._password}")
                 if self._password_file:
                     pargs.append(f"--password_file={self._password_file}")
                 else:
                     pargs.append("--password_file=")
 
                 pargs.append(f"--sn_url={self._endpoint}")
                 pargs.append("--logfile=sn1.log")
-            elif i == 1:
-                # args for rangeget node
-                pargs = [py_exe,
-                         os.path.join(cmd_dir, "hsds-rangeget"),
-                         "--log_prefix=rg "]
             else:
-                node_number = i - 2  # start with 0
-                pargs = [py_exe,
-                         os.path.join(cmd_dir, "hsds-datanode"),
-                         f"--log_prefix=dn{node_number+1} "]
+                node_number = i - 1  # start with 0
+                pname = f"dn{node_number}"
+                pargs = [
+                    py_exe,
+                    cmd_path,
+                    "--node_type=dn",
+                    f"--log_prefix=dn{node_number+1} ",
+                ]
                 pargs.append(f"--dn_urls={dn_urls_arg}")
                 pargs.append(f"--node_number={node_number}")
             # logging.info(f"starting {pargs[0]}")
             pargs.extend(common_args)
-            p = subprocess.Popen(pargs, bufsize=1, universal_newlines=True, shell=False, stdout=pout)
-            self._processes.append(p)
+            p = subprocess.Popen(
+                pargs, bufsize=1, universal_newlines=True, shell=False, stdout=pout
+            )
+            self._processes[pname] = p
             # setup queue so we can check on process output without blocking
             q = queue.Queue()
             loglevel = self.log.root.level
             t = threading.Thread(target=_enqueue_output, args=(p.stdout, q, loglevel))
             self._queues.append(q)
             t.daemon = True  # thread dies with the program
             t.start()
             self._threads.append(t)
 
         # wait to sockets are initialized
         start_ts = time.time()
-        SLEEP_TIME = 0.1  # time to sleep between checking on socket connection
+        SLEEP_TIME = 1  # time to sleep between checking on socket connection
         MAX_INIT_TIME = 10.0  # max time to wait for socket to be initialized
 
         while True:
             ready = 0
-            for socket_path in self._socket_paths:
-                if os.path.exists(socket_path):
-                    ready += 1
+            if len(self._socket_paths) > 0:
+                for socket_path in self._socket_paths:
+                    if os.path.exists(socket_path):
+                        ready += 1
+            else:
+                if time.time() > start_ts + 5:
+                    # TBD - put a real ready check here
+                    ready = count
             if ready == count:
                 self.log.info("all processes ready!")
                 break
             else:
                 self.log.debug(f"{ready}/{count} ready")
                 self.log.debug(f"sleeping for {SLEEP_TIME}")
                 time.sleep(SLEEP_TIME)
@@ -253,50 +333,59 @@
                     self.log.error(msg)
                     raise IOError(msg)
 
         self.log.info(f"Ready after: {(time.time()-start_ts):4.2f} s")
         self._ready = True
 
     def stop(self):
-        """ terminate hsds processes
-        """
+        """terminate hsds processes"""
         if not self._processes:
             return
+
         now = time.time()
         logging.info(f"hsds app stop at {now}")
-        for p in self._processes:
-            logging.info(f"sending SIGINT to {p.args[0]}")
-            p.send_signal(signal.SIGINT)
+
+        for pname in self._processes:
+            p = self._processes[pname]
+            logging.info(f"terminating sub-process: {pname}")
+            p.terminate()
+
         # wait for sub-proccesses to exit
         SLEEP_TIME = 0.1  # time to sleep between checking on process state
         MAX_WAIT_TIME = 10.0  # max time to wait for sub-process to terminate
         start_ts = time.time()
         while True:
-            is_alive = False
-            for p in self._processes:
+            is_alive_cnt = 0
+            for pname in self._processes:
+                p = self._processes[pname]
                 if p.poll() is None:
-                    is_alive = True
-            if is_alive:
-                logging.debug(f"still alive, sleep {SLEEP_TIME}")
+                    self.log.debug(f"process {pname} still alive")
+                    is_alive_cnt += 1
+                else:
+                    self.log.debug(f"process {pname} has exited")
+
+            if is_alive_cnt > 0:
+                logging.debug(f"stop - {is_alive_cnt} processes still alive, sleep {SLEEP_TIME}")
                 time.sleep(SLEEP_TIME)
             else:
                 logging.debug("all subprocesses exited")
                 break
             if time.time() > start_ts + MAX_WAIT_TIME:
                 msg = f"failed to terminate after {MAX_WAIT_TIME} seconds"
                 self.log.error(msg)
                 break
 
         # kill any reluctant to die processes
-        for p in self._processes:
+        for pname in self._processes:
+            p = self._processes[pname]
             if p.poll():
-                logging.info(f"terminating {p.args[0]}")
+                logging.info(f"terminating process {pname}")
                 p.terminate()
-        self._processes = []
+        self._processes = {}  # reset
         for t in self._threads:
             del t
         self._threads = []
 
     def __del__(self):
-        """ cleanup class resources """
+        """cleanup class resources"""
         self.stop()
         # self._tempdir.cleanup()
```

### Comparing `hsds-0.7.0b11/hsds/hsds_logger.py` & `hsds-0.8.0/hsds/hsds_logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # Simple looger for hsds
 #
+
 import asyncio
 import time
 from aiohttp.web_exceptions import HTTPServiceUnavailable
 from .util.domainUtil import getDomainFromRequest
 
 # Levels copied from python logging module
 DEBUG = 10
@@ -24,115 +25,129 @@
 ERROR = 40
 
 req_count = {"GET": 0, "POST": 0, "PUT": 0, "DELETE": 0, "num_tasks": 0}
 log_count = {"DEBUG": 0, "INFO": 0, "WARN": 0, "ERROR": 0}
 # the following defaults will be adjusted by the app
 config = {"log_level": DEBUG, "prefix": "", "timestamps": False}
 
+
 def _getLevelName(level):
     if level == DEBUG:
         name = "DEBUG"
     elif level == INFO:
         name = "INFO"
     elif level == WARNING:
         name = "WARN"
     elif level == ERROR:
         name = "ERROR"
     else:
         name = "????"
     return name
 
+
 def setLogConfig(level, prefix=None, timestamps=None):
     if level == "DEBUG":
         config["log_level"] = DEBUG
     elif level == "INFO":
         config["log_level"] = INFO
     elif level == "WARNING":
         config["log_level"] = WARNING
     elif level == "WARN":
         config["log_level"] = WARNING
     elif level == "ERROR":
         config["log_level"] = ERROR
     else:
         raise ValueError(f"unexpected log_level: {level}")
+    # print(f"setLogConfig - level={level}")
     if prefix is not None:
         config["prefix"] = prefix
     if timestamps is not None:
         config["timestamps"] = timestamps
-    
-        
+
+
 def _activeTaskCount():
     count = 0
     for task in asyncio.all_tasks():
         if not task.done():
             count += 1
     return count
 
+
 def _timestamp():
 
     if config["timestamps"]:
         now = time.time()
         ts = f"{now:.3f} "
     else:
         ts = ""
-    
+
     return ts
 
+
 def _logMsg(level, msg):
     if config["log_level"] > level:
         return  # ignore
 
     ts = _timestamp()
 
     prefix = config["prefix"]
 
     level_name = _getLevelName(level)
 
     print(f"{prefix}{ts}{level_name}> {msg}")
 
     log_count[level_name] += 1
-        
 
 
 def debug(msg):
     _logMsg(DEBUG, msg)
-    
+
+
 def info(msg):
     _logMsg(INFO, msg)
-     
+
+
 def warn(msg):
-    _logMsg(WARNING,  msg)
-     
+    _logMsg(WARNING, msg)
+
+
 def warning(msg):
     _logMsg(WARNING, msg)
-     
+
+
 def error(msg):
     _logMsg(ERROR, msg)
-     
+
 
 def request(req):
     app = req.app
     domain = getDomainFromRequest(req, validate=False)
     prefix = config["prefix"]
     ts = _timestamp()
 
     msg = f"{prefix}{ts}REQ> {req.method}: {req.path}"
     if domain:
         msg += f" [{domain}]"
     print(msg)
- 
-    INFO_METHODS = ("/about", "/register", "/info", "/nodeinfo",
-                    "/nodestate", "/register")
+
+    INFO_METHODS = (
+        "/about",
+        "/register",
+        "/info",
+        "/nodeinfo",
+        "/nodestate",
+        "/register",
+    )
     if req.path in INFO_METHODS:
         # always service these state requests regardles of node state and
         # task load
         return
     node_state = app["node_state"] if "node_state" in app else None
     if node_state != "READY":
-        warning(f"returnåing 503 - node_state: {node_state}")
+        warning(f"returning 503 - node_state: {node_state}")
         raise HTTPServiceUnavailable()
     if req.method in ("GET", "POST", "PUT", "DELETE"):
         req_count[req.method] += 1
     num_tasks = len(asyncio.all_tasks())
     active_tasks = _activeTaskCount()
     req_count["num_tasks"] = num_tasks
     if config["log_level"] == DEBUG:
@@ -158,14 +173,14 @@
     if code > 399:
         if code < 500:
             level = WARNING
         else:
             level = ERROR
 
     log_level = config["log_level"]
-    
+
     if log_level <= level:
         prefix = config["prefix"]
         ts = _timestamp()
-        
+
         s = "{}{} RSP> <{}> ({}): {}"
         print(s.format(prefix, ts, code, message, req.path))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hsds-0.7.0b11/hsds/link_dn.py` & `hsds-0.8.0/hsds/link_dn.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,49 +8,59 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # data node of hsds cluster
 #
+
 import time
 from copy import copy
 from bisect import bisect_left
 
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPNotFound, HTTPConflict
 from aiohttp.web_exceptions import HTTPInternalServerError
 from aiohttp.web import json_response
 
 from .util.idUtil import isValidUuid
 from .util.linkUtil import validateLinkName
 from .datanode_lib import get_obj_id, get_metadata_obj, save_metadata_obj
 from . import hsds_logger as log
 
 
-def _index(a, x):
-    """ Locate the leftmost value exactly equal to x
-    """
-    i = bisect_left(a, x)
-    if i != len(a) and a[i] == x:
-        return i
+def _index(items, marker, create_order=False):
+    """Locate the leftmost value exactly equal to x"""
+    if create_order:
+        # list is not ordered, juse search linearly
+        for i in range(len(items)):
+            if items[i] == marker:
+                return i
+    else:
+        i = bisect_left(items, marker)
+        if i != len(items) and items[i] == marker:
+            return i
+    # not found
     return -1
 
 
 async def GET_Links(request):
-    """HTTP GET method to return JSON for a link collection
-    """
+    """HTTP GET method to return JSON for a link collection"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
     group_id = get_obj_id(request)
     log.info(f"GET links: {group_id}")
     if not isValidUuid(group_id, obj_class="group"):
         log.error(f"Unexpected group_id: {group_id}")
         raise HTTPInternalServerError()
 
+    create_order = False
+    if "CreateOrder" in params and params["CreateOrder"]:
+        create_order = True
+
     limit = None
     if "Limit" in params:
         try:
             limit = int(params["Limit"])
             log.info(f"GET_Links - using Limit: {limit}")
         except ValueError:
             msg = "Bad Request: Expected int type for limit"
@@ -60,73 +70,89 @@
     if "Marker" in params:
         marker = params["Marker"]
         log.info(f"GET_Links - using Marker: {marker}")
 
     bucket = None
     if "bucket" in params:
         bucket = params["bucket"]
-    
+
     if not bucket:
         msg = "GET_Links - no bucket param"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     group_json = await get_metadata_obj(app, group_id, bucket=bucket)
 
     log.info(f"for id: {group_id} got group json: {group_json}")
     if "links" not in group_json:
         msg.error(f"unexpected group data for id: {group_id}")
         raise HTTPInternalServerError()
 
     # return a list of links based on sorted dictionary keys
     link_dict = group_json["links"]
-    titles = list(link_dict.keys())
-    titles.sort()  # sort by key
-    # TBD: provide an option to sort by create date
+
+    titles = []
+    if create_order:
+        order_dict = {}
+        for title in link_dict:
+            item = link_dict[title]
+            if "created" not in item:
+                log.warning(f"expected to find 'created' key in link item {title}")
+                continue
+            order_dict[title] = item["created"]
+        log.debug(f"order_dict: {order_dict}")
+        # now sort by created
+        for k in sorted(order_dict.items(), key=lambda item: item[1]):
+            titles.append(k[0])
+        log.debug(f"links by create order: {titles}")
+    else:
+        titles = list(link_dict.keys())
+        titles.sort()  # sort by key
+        log.debug(f"links by lexographic order: {titles}")
 
     start_index = 0
     if marker is not None:
-        start_index = _index(titles, marker) + 1
+        start_index = _index(titles, marker, create_order=create_order) + 1
         if start_index == 0:
             # marker not found, return 404
             msg = f"Link marker: {marker}, not found"
             log.warn(msg)
             raise HTTPNotFound()
 
     end_index = len(titles)
     if limit is not None and (end_index - start_index) > limit:
         end_index = start_index + limit
 
     link_list = []
     for i in range(start_index, end_index):
         title = titles[i]
         link = copy(link_dict[title])
+        log.debug(f"link list[{i}: {link}")
         link["title"] = title
         link_list.append(link)
 
     resp_json = {"links": link_list}
     resp = json_response(resp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def GET_Link(request):
-    """HTTP GET method to return JSON for a link
-    """
+    """HTTP GET method to return JSON for a link"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
     group_id = get_obj_id(request)
     log.info(f"GET link: {group_id}")
 
     if not isValidUuid(group_id, obj_class="group"):
         log.error(f"Unexpected group_id: {group_id}")
         raise HTTPInternalServerError()
 
-    link_title = request.match_info.get('title')
+    link_title = request.match_info.get("title")
 
     validateLinkName(link_title)
 
     bucket = None
     if "bucket" in params:
         bucket = params["bucket"]
     if not bucket:
@@ -149,25 +175,25 @@
 
     resp = json_response(link_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def PUT_Link(request):
-    """ Handler creating a new link"""
+    """Handler creating a new link"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
     group_id = get_obj_id(request)
     log.info(f"PUT link: {group_id}")
     if not isValidUuid(group_id, obj_class="group"):
         log.error(f"Unexpected group_id: {group_id}")
         raise HTTPInternalServerError()
 
-    link_title = request.match_info.get('title')
+    link_title = request.match_info.get("title")
     validateLinkName(link_title)
 
     log.info(f"link_title: {link_title}")
 
     if not request.has_body:
         msg = "PUT Link with no body"
         log.warn(msg)
@@ -193,15 +219,15 @@
 
     if "bucket" in params:
         bucket = params["bucket"]
     elif "bucket" in body:
         bucket = params["bucket"]
     else:
         bucket = None
-    
+
     if not bucket:
         msg = "GET_Links - no bucket param"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     group_json = await get_metadata_obj(app, group_id, bucket=bucket)
     if "links" not in group_json:
@@ -230,28 +256,27 @@
 
     resp = json_response(resp_json, status=201)
     log.response(request, resp=resp)
     return resp
 
 
 async def DELETE_Link(request):
-    """HTTP DELETE method for group links
-    """
+    """HTTP DELETE method for group links"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
     group_id = get_obj_id(request)
     log.info(f"DELETE link: {group_id}")
 
     if not isValidUuid(group_id, obj_class="group"):
         msg = f"Unexpected group_id: {group_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
-    link_title = request.match_info.get('title')
+    link_title = request.match_info.get("title")
     validateLinkName(link_title)
 
     if "bucket" in params:
         bucket = params["bucket"]
     else:
         bucket = None
     if not bucket:
@@ -277,12 +302,12 @@
     now = time.time()
     group_json["lastModified"] = now
 
     # write back to S3
     await save_metadata_obj(app, group_id, group_json, bucket=bucket)
 
     hrefs = []  # TBD
-    resp_json = {"href":  hrefs}
+    resp_json = {"href": hrefs}
 
     resp = json_response(resp_json)
     log.response(request, resp=resp)
     return resp
```

### Comparing `hsds-0.7.0b11/hsds/link_sn.py` & `hsds-0.8.0/hsds/link_sn.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,56 +10,62 @@
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # service node of hsds cluster
 #
 
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPConflict
+from json import JSONDecodeError
 
 from .util.httpUtil import http_get, http_put, http_delete, getHref
 from .util.httpUtil import jsonResponse
 from .util.idUtil import isValidUuid, getDataNodeUrl, getCollectionForId
-from .util.authUtil import getUserPasswordFromRequest,   validateUserPassword
+from .util.authUtil import getUserPasswordFromRequest, validateUserPassword
 from .util.domainUtil import getDomainFromRequest, isValidDomain
 from .util.domainUtil import getBucketForDomain
 from .util.linkUtil import validateLinkName
 from .servicenode_lib import validateAction, getObjectJson
 from . import config
 from . import hsds_logger as log
 
 
 async def GET_Links(request):
     """HTTP method to return JSON for link collection"""
     log.request(request)
     app = request.app
     params = request.rel_url.query
 
-    group_id = request.match_info.get('id')
+    group_id = request.match_info.get("id")
+
     if not group_id:
         msg = "Missing group id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(group_id, obj_class="Group"):
         msg = f"Invalid group id: {group_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     limit = None
+    create_order = False
+    if "CreateOrder" in params and params["CreateOrder"]:
+        create_order = True
+
     if "Limit" in params:
         try:
             limit = int(params["Limit"])
         except ValueError:
             msg = "Bad Request: Expected int type for limit"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
     marker = None
     if "Marker" in params:
         marker = params["Marker"]
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"domain: {domain}"
@@ -69,75 +75,74 @@
     if not bucket:
         bucket = config.get("bucket_name")
 
     await validateAction(app, domain, group_id, username, "read")
 
     req = getDataNodeUrl(app, group_id)
     req += "/groups/" + group_id + "/links"
-    query_sep = '?'
-    if limit is not None:
-        req += query_sep + "Limit=" + str(limit)
-        query_sep = '&'
-    if marker is not None:
-        req += query_sep + "Marker=" + marker
 
-    log.debug("get LINKS: " + req)
     params = {}
+    if create_order:
+        params["CreateOrder"] = 1
+    if limit is not None:
+        params["Limit"] = str(limit)
+    if marker is not None:
+        params["Marker"] = marker
     if bucket:
         params["bucket"] = bucket
     links_json = await http_get(app, req, params=params)
     log.debug(f"got links json from dn for group_id: {group_id}")
     links = links_json["links"]
 
     # mix in collection key, target and hrefs
     for link in links:
         if link["class"] == "H5L_TYPE_HARD":
             collection_name = getCollectionForId(link["id"])
             link["collection"] = collection_name
-            target_uri = '/' + collection_name + '/' + link["id"]
+            target_uri = "/" + collection_name + "/" + link["id"]
             link["target"] = getHref(request, target_uri)
-        link_uri = '/groups/' + group_id + '/links/' + link['title']
+        link_uri = "/groups/" + group_id + "/links/" + link["title"]
         link["href"] = getHref(request, link_uri)
 
     resp_json = {}
     resp_json["links"] = links
     hrefs = []
-    group_uri = '/groups/'+group_id
-    href = getHref(request, group_uri+'/links')
-    hrefs.append({'rel': 'self', 'href': href})
-    href = getHref(request, '/')
-    hrefs.append({'rel': 'home', 'href': href})
+    group_uri = "/groups/" + group_id
+    href = getHref(request, group_uri + "/links")
+    hrefs.append({"rel": "self", "href": href})
+    href = getHref(request, "/")
+    hrefs.append({"rel": "home", "href": href})
     href = getHref(request, group_uri)
-    hrefs.append({'rel': 'owner', 'href': href})
+    hrefs.append({"rel": "owner", "href": href})
     resp_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, resp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def GET_Link(request):
     """HTTP method to return JSON for a group link"""
     log.request(request)
     app = request.app
 
-    group_id = request.match_info.get('id')
+    group_id = request.match_info.get("id")
     if not group_id:
         msg = "Missing group id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(group_id, obj_class="Group"):
         msg = f"Invalid group id: {group_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    link_title = request.match_info.get('title')
+    link_title = request.match_info.get("title")
     validateLinkName(link_title)
 
     username, pswd = getUserPasswordFromRequest(request)
-    if username is None and app['allow_noauth']:
+    if username is None and app["allow_noauth"]:
         username = "default"
     else:
         await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
@@ -174,61 +179,66 @@
     resp_json = {}
     resp_json["link"] = resp_link
     resp_json["created"] = link_json["created"]
     # links don't get modified, so use created timestamp as lastModified
     resp_json["lastModified"] = link_json["created"]
 
     hrefs = []
-    group_uri = '/groups/'+group_id
+    group_uri = "/groups/" + group_id
     href = getHref(request, f"{group_uri}/links/{link_title}")
-    hrefs.append({'rel': 'self', 'href': href})
-    href = getHref(request, '/')
-    hrefs.append({'rel': 'home', 'href': href})
+    hrefs.append({"rel": "self", "href": href})
+    href = getHref(request, "/")
+    hrefs.append({"rel": "home", "href": href})
     href = getHref(request, group_uri)
-    hrefs.append({'rel': 'owner', 'href': href})
+    hrefs.append({"rel": "owner", "href": href})
     if link_json["class"] == "H5L_TYPE_HARD":
-        target = '/' + resp_link["collection"] + '/' + resp_link["id"]
+        target = "/" + resp_link["collection"] + "/" + resp_link["id"]
         href = getHref(request, target)
-        hrefs.append({'rel': 'target', 'href': href})
+        hrefs.append({"rel": "target", "href": href})
 
     resp_json["hrefs"] = hrefs
 
     resp = await jsonResponse(request, resp_json)
     log.response(request, resp=resp)
     return resp
 
 
 async def PUT_Link(request):
     """HTTP method to create a new link"""
     log.request(request)
     app = request.app
 
-    group_id = request.match_info.get('id')
+    group_id = request.match_info.get("id")
     if not group_id:
         msg = "Missing group id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(group_id, obj_class="Group"):
         msg = f"Invalid group id: {group_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    link_title = request.match_info.get('title')
+    link_title = request.match_info.get("title")
     log.info(f"PUT Link_title: [{link_title}]")
     validateLinkName(link_title)
 
     username, pswd = getUserPasswordFromRequest(request)
     # write actions need auth
     await validateUserPassword(app, username, pswd)
 
     if not request.has_body:
         msg = "PUT Link with no body"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
-    body = await request.json()
+    try:
+        body = await request.json()
+    except JSONDecodeError:
+        msg = "Unable to load JSON body"
+        log.warn(msg)
+        raise HTTPBadRequest(reason=msg)
 
     link_json = {}
     if "id" in body:
         if not isValidUuid(body["id"]):
             msg = "PUT Link with invalid id in body"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
@@ -253,14 +263,15 @@
     if not isValidDomain(domain):
         msg = f"Invalid domain: {domain}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     bucket = getBucketForDomain(domain)
     if not bucket:
         bucket = config.get("bucket_name")
+
     await validateAction(app, domain, group_id, username, "create")
 
     # for hard links, verify that the referenced id exists and is in
     # this domain
     if "id" in body:
         ref_id = body["id"]
         ref_json = await getObjectJson(app, ref_id, bucket=bucket)
@@ -317,39 +328,39 @@
 
 
 async def DELETE_Link(request):
     """HTTP method to delete a link"""
     log.request(request)
     app = request.app
 
-    group_id = request.match_info.get('id')
+    group_id = request.match_info.get("id")
     if not group_id:
         msg = "Missing group id"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     if not isValidUuid(group_id, obj_class="Group"):
         msg = f"Invalid group id: {group_id}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    link_title = request.match_info.get('title')
+    link_title = request.match_info.get("title")
     validateLinkName(link_title)
 
     username, pswd = getUserPasswordFromRequest(request)
     await validateUserPassword(app, username, pswd)
 
     domain = getDomainFromRequest(request)
     if not isValidDomain(domain):
         msg = f"domain: {domain}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     bucket = getBucketForDomain(domain)
     if not bucket:
         bucket = config.get("bucket_name")
-        
+
     await validateAction(app, domain, group_id, username, "delete")
 
     req = getDataNodeUrl(app, group_id)
     req += "/groups/" + group_id + "/links/" + link_title
     params = {}
     if bucket:
         params["bucket"] = bucket
```

### Comparing `hsds-0.7.0b11/hsds/servicenode.py` & `hsds-0.8.0/hsds/servicenode.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # service node of hsds cluster
 #
+
 import asyncio
-from collections import deque
+import time
 from aiohttp.web import run_app
 import aiohttp_cors
 from .util.lruCache import LruCache
 from .util.httpUtil import isUnixDomainUrl, bindToSocket, getPortFromUrl
-from .util.httpUtil import release_http_client
+from .util.httpUtil import release_http_client, jsonResponse
 
 from . import config
-from .basenode import healthCheck,  baseInit
+from .basenode import healthCheck, baseInit
 from . import hsds_logger as log
 from .util.authUtil import initUserDB, initGroupDB, setPassword
 from .domain_sn import GET_Domain, PUT_Domain, DELETE_Domain, GET_Domains
 from .domain_sn import GET_Datasets, GET_Groups, GET_Datatypes
 from .domain_sn import GET_ACL, GET_ACLs, PUT_ACL
 from .group_sn import GET_Group, POST_Group, DELETE_Group
 from .link_sn import GET_Links, GET_Link, PUT_Link, DELETE_Link
@@ -35,168 +36,193 @@
 from .dset_sn import GET_Dataset, POST_Dataset, DELETE_Dataset
 from .dset_sn import GET_DatasetShape, PUT_DatasetShape, GET_DatasetType
 from .chunk_sn import PUT_Value, GET_Value, POST_Value
 
 
 async def init():
     """Intitialize application and return app object"""
-    app = baseInit('sn')
+    app = baseInit("sn")
 
     # call app.router.add_get() here to add node-specific routes
     #
-    path = '/'
-    app.router.add_route('GET', path, GET_Domain)
-    app.router.add_route('DELETE', path, DELETE_Domain)
-    app.router.add_route('PUT', path, PUT_Domain)
-    path = '/domains'
-    app.router.add_route('GET', path, GET_Domains)
-    path = '/acls/{username}'
-    app.router.add_route('GET', path, GET_ACL)
-    app.router.add_route('PUT', path, PUT_ACL)
-    path = '/acls'
-    app.router.add_route('GET', path, GET_ACLs)
-    path = '/groups/'
-    app.router.add_route('GET', path, GET_Group)
-    path = '/groups'
-    app.router.add_route('GET', path, GET_Groups)
-    app.router.add_route('POST', path, POST_Group)
-    path = '/groups/{id}'
-    app.router.add_route('GET', path, GET_Group)
-    app.router.add_route('DELETE', path, DELETE_Group)
-    path = '/groups/{id}/links'
-    app.router.add_route('GET', path, GET_Links)
-    path = '/groups/{id}/links/{title}'
-    app.router.add_route('GET', path, GET_Link)
-    app.router.add_route('DELETE', path, DELETE_Link)
-    app.router.add_route('PUT', path, PUT_Link)
-    path = '/groups/{id}/attributes'
-    app.router.add_route('GET', path, GET_Attributes)
-    path = '/groups/{id}/attributes/{name}'
-    app.router.add_route('GET', path, GET_Attribute)
-    app.router.add_route('DELETE', path, DELETE_Attribute)
-    app.router.add_route('PUT', path, PUT_Attribute)
-    path = '/groups/{id}/attributes/{name}/value'
-    app.router.add_route('GET', path, GET_AttributeValue)
-    app.router.add_route('PUT', path, PUT_AttributeValue)
-    path = '/groups/{id}/acls/{username}'
-    app.router.add_route('GET', path, GET_ACL)
-    app.router.add_route('PUT', path, PUT_ACL)
-    path = '/groups/{id}/acls'
-    app.router.add_route('GET', path, GET_ACLs)
-    path = '/datatypes'
-    app.router.add_route('GET', path, GET_Datatypes)
-    app.router.add_route('POST', path, POST_Datatype)
-    path = '/datatypes/'
-    app.router.add_route('GET', path, GET_Datatype)
-    path = '/datatypes/{id}'
-    app.router.add_route('GET', path, GET_Datatype)
-    app.router.add_route('DELETE', path, DELETE_Datatype)
-    path = '/datatypes/{id}/attributes'
-    app.router.add_route('GET', path, GET_Attributes)
-    path = '/datatypes/{id}/attributes/{name}'
-    app.router.add_route('GET', path, GET_Attribute)
-    app.router.add_route('DELETE', path, DELETE_Attribute)
-    app.router.add_route('PUT', path, PUT_Attribute)
-    path = '/datatypes/{id}/attributes/{name}/value'
-    app.router.add_route('GET', path, GET_AttributeValue)
-    app.router.add_route('PUT', path, PUT_AttributeValue)
-    path = '/datatypes/{id}/acls/{username}'
-    app.router.add_route('GET', path, GET_ACL)
-    app.router.add_route('PUT', path, PUT_ACL)
-    path = '/datatypes/{id}/acls'
-    app.router.add_route('GET', path, GET_ACLs)
-    path = '/datasets/{id}'
-    app.router.add_route('GET', path, GET_Dataset)
-    app.router.add_route('DELETE', path, DELETE_Dataset)
-    path = '/datasets/'
-    app.router.add_route('GET', path, GET_Dataset)
-    path = '/datasets'
-    app.router.add_route('GET', path, GET_Datasets)
-    app.router.add_route('POST', path, POST_Dataset)
-    path = '/datasets/{id}/shape'
-    app.router.add_route('GET', path, GET_DatasetShape)
-    app.router.add_route('PUT', path, PUT_DatasetShape)
-    path = '/datasets/{id}/type'
-    app.router.add_route('GET', path, GET_DatasetType)
-    path = '/datasets/{id}/attributes'
-    app.router.add_route('GET', path, GET_Attributes)
-    path = '/datasets/{id}/attributes/{name}'
-    app.router.add_route('GET', path, GET_Attribute)
-    app.router.add_route('DELETE', path, DELETE_Attribute)
-    app.router.add_route('PUT', path, PUT_Attribute)
-    path = '/datasets/{id}/attributes/{name}/value'
-    app.router.add_route('GET', path, GET_AttributeValue)
-    app.router.add_route('PUT', path, PUT_AttributeValue)
-    path = '/datasets/{id}/value'
-    app.router.add_route('PUT', path, PUT_Value)
-    app.router.add_route('GET', path, GET_Value)
-    app.router.add_route('POST', path, POST_Value)
-    path = '/datasets/{id}/acls/{username}'
-    app.router.add_route('GET', path, GET_ACL)
-    app.router.add_route('PUT', path, PUT_ACL)
-    path = '/datasets/{id}/acls'
-    app.router.add_route('GET', path, GET_ACLs)
+    path = "/"
+    app.router.add_route("GET", path, GET_Domain)
+    app.router.add_route("DELETE", path, DELETE_Domain)
+    app.router.add_route("PUT", path, PUT_Domain)
+    path = "/domains"
+    app.router.add_route("GET", path, GET_Domains)
+    path = "/acls/{username}"
+    app.router.add_route("GET", path, GET_ACL)
+    app.router.add_route("PUT", path, PUT_ACL)
+    path = "/acls"
+    app.router.add_route("GET", path, GET_ACLs)
+    path = "/groups/"
+    app.router.add_route("GET", path, GET_Group)
+    path = "/groups"
+    app.router.add_route("GET", path, GET_Groups)
+    app.router.add_route("POST", path, POST_Group)
+    path = "/groups/{id}"
+    app.router.add_route("GET", path, GET_Group)
+    app.router.add_route("DELETE", path, DELETE_Group)
+    path = "/groups/{id}/links"
+    app.router.add_route("GET", path, GET_Links)
+    path = "/groups/{id}/links/{title}"
+    app.router.add_route("GET", path, GET_Link)
+    app.router.add_route("DELETE", path, DELETE_Link)
+    app.router.add_route("PUT", path, PUT_Link)
+    path = "/groups/{id}/attributes"
+    app.router.add_route("GET", path, GET_Attributes)
+    path = "/groups/{id}/attributes/{name}"
+    app.router.add_route("GET", path, GET_Attribute)
+    app.router.add_route("DELETE", path, DELETE_Attribute)
+    app.router.add_route("PUT", path, PUT_Attribute)
+    path = "/groups/{id}/attributes/{name}/value"
+    app.router.add_route("GET", path, GET_AttributeValue)
+    app.router.add_route("PUT", path, PUT_AttributeValue)
+    path = "/groups/{id}/acls/{username}"
+    app.router.add_route("GET", path, GET_ACL)
+    app.router.add_route("PUT", path, PUT_ACL)
+    path = "/groups/{id}/acls"
+    app.router.add_route("GET", path, GET_ACLs)
+    path = "/datatypes"
+    app.router.add_route("GET", path, GET_Datatypes)
+    app.router.add_route("POST", path, POST_Datatype)
+    path = "/datatypes/"
+    app.router.add_route("GET", path, GET_Datatype)
+    path = "/datatypes/{id}"
+    app.router.add_route("GET", path, GET_Datatype)
+    app.router.add_route("DELETE", path, DELETE_Datatype)
+    path = "/datatypes/{id}/attributes"
+    app.router.add_route("GET", path, GET_Attributes)
+    path = "/datatypes/{id}/attributes/{name}"
+    app.router.add_route("GET", path, GET_Attribute)
+    app.router.add_route("DELETE", path, DELETE_Attribute)
+    app.router.add_route("PUT", path, PUT_Attribute)
+    path = "/datatypes/{id}/attributes/{name}/value"
+    app.router.add_route("GET", path, GET_AttributeValue)
+    app.router.add_route("PUT", path, PUT_AttributeValue)
+    path = "/datatypes/{id}/acls/{username}"
+    app.router.add_route("GET", path, GET_ACL)
+    app.router.add_route("PUT", path, PUT_ACL)
+    path = "/datatypes/{id}/acls"
+    app.router.add_route("GET", path, GET_ACLs)
+    path = "/datasets/{id}"
+    app.router.add_route("GET", path, GET_Dataset)
+    app.router.add_route("DELETE", path, DELETE_Dataset)
+    path = "/datasets/"
+    app.router.add_route("GET", path, GET_Dataset)
+    path = "/datasets"
+    app.router.add_route("GET", path, GET_Datasets)
+    app.router.add_route("POST", path, POST_Dataset)
+    path = "/datasets/{id}/shape"
+    app.router.add_route("GET", path, GET_DatasetShape)
+    app.router.add_route("PUT", path, PUT_DatasetShape)
+    path = "/datasets/{id}/type"
+    app.router.add_route("GET", path, GET_DatasetType)
+    path = "/datasets/{id}/attributes"
+    app.router.add_route("GET", path, GET_Attributes)
+    path = "/datasets/{id}/attributes/{name}"
+    app.router.add_route("GET", path, GET_Attribute)
+    app.router.add_route("DELETE", path, DELETE_Attribute)
+    app.router.add_route("PUT", path, PUT_Attribute)
+    path = "/datasets/{id}/attributes/{name}/value"
+    app.router.add_route("GET", path, GET_AttributeValue)
+    app.router.add_route("PUT", path, PUT_AttributeValue)
+    path = "/datasets/{id}/value"
+    app.router.add_route("PUT", path, PUT_Value)
+    app.router.add_route("GET", path, GET_Value)
+    app.router.add_route("POST", path, POST_Value)
+    path = "/datasets/{id}/acls/{username}"
+    app.router.add_route("GET", path, GET_ACL)
+    app.router.add_route("PUT", path, PUT_ACL)
+    path = "/datasets/{id}/acls"
+    app.router.add_route("GET", path, GET_ACLs)
 
     # Add CORS to all routes
     cors_domain = config.get("cors_domain")
     if cors_domain:
-        kwargs = {"allow_credentials": True,
-                  "expose_headers": "*",
-                  "allow_headers": "*",
-                  "allow_methods": ["POST", "PUT", "GET", "DELETE"]}
+        kwargs = {
+            "allow_credentials": True,
+            "expose_headers": "*",
+            "allow_headers": "*",
+            "allow_methods": ["POST", "PUT", "GET", "DELETE"],
+        }
         cors_defaults = {cors_domain: aiohttp_cors.ResourceOptions(**kwargs)}
         cors = aiohttp_cors.setup(app, defaults=cors_defaults)
         for route in list(app.router.routes()):
-            log.info(f"CORS add route: {route}")
             cors.add(route)
 
     return app
 
 
 async def start_background_tasks(app):
     if "is_standalone" in app:
-       return  # don't need health check
+        return  # don't need health check
     loop = asyncio.get_event_loop()
     loop.create_task(healthCheck(app))
 
+
 async def on_shutdown(app):
-    """ Release any held resources """
+    """Release any held resources"""
     log.info("on_shutdown")
+    # finally release any http_clients
     await release_http_client(app)
 
+    log.info("on_shutdown - done")
+
+
+async def preStop(request):
+    """HTTP Method used by K8s to signal the container is shutting down"""
+
+    log.request(request)
+    app = request.app
+
+    shutdown_start = time.time()
+    log.warn(f"preStop request calling on_shutdown at {shutdown_start:.2f}")
+    await on_shutdown(app)
+    shutdown_elapse_time = time.time() - shutdown_start
+    msg = f"shutdown took: {shutdown_elapse_time:.2f} seconds"
+    if shutdown_elapse_time > 2.0:
+        # 2.0 is the default grace period for kubernetes
+        log.warn(msg)
+    else:
+        log.info(msg)
+    resp = await jsonResponse(request, {})
+    log.response(request, resp=resp)
+    return resp
+
+
 def create_app():
-    """Create servicenode aiohttp application
-    """
+    """Create servicenode aiohttp application"""
     log.info("service node initializing")
 
     loop = asyncio.get_event_loop()
     app = loop.run_until_complete(init())
 
     metadata_mem_cache_size = int(config.get("metadata_mem_cache_size"))
     msg = f"Using metadata memory cache size of: {metadata_mem_cache_size}"
     log.info(msg)
     kwargs = {"mem_target": metadata_mem_cache_size}
     kwargs["name"] = "MetaCache"
     app["meta_cache"] = LruCache(**kwargs)
     kwargs["name"] = "DomainCache"
-    app['domain_cache'] = LruCache(**kwargs)
-    app["shm_blocks"] =  deque()  # store (timestamp, shm_name) tuples
+    app["domain_cache"] = LruCache(**kwargs)
 
     if config.get("allow_noauth"):
         allow_noauth = config.get("allow_noauth")
         if isinstance(allow_noauth, str):
             if allow_noauth in ("0", "F", "False"):
                 allow_noauth = False
             else:
                 allow_noauth = True
         log.info(f"allow_noauth = {allow_noauth}")
-        app['allow_noauth'] = allow_noauth
+        app["allow_noauth"] = allow_noauth
     else:
         log.info("allow_noauth = False")
-        app['allow_noauth'] = False
+        app["allow_noauth"] = False
 
     initUserDB(app)
     initGroupDB(app)
 
     # typically these are null
     hs_username = config.getCmdLineArg("hs_username")
     hs_password = config.getCmdLineArg("hs_password")
@@ -211,15 +237,15 @@
     app.on_shutdown.append(on_shutdown)
 
     return app
 
 
 def main():
     """
-      Main - entry point for service node
+    Main - entry point for service node
     """
     log.info("Service node initializing")
     app = create_app()
 
     # run app using either socket or tcp
     sn_url = config.getCmdLineArg("sn_url")
     if sn_url:
@@ -249,13 +275,13 @@
             log.error(f"got exception: {e}")
         log.info("run_app done")
         # close socket?
     else:
         # Use TCP connection
         log.info(f"run_app on port: {sn_port}")
         run_app(app, port=sn_port)
-    
+
     log.info("Service node exiting")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `hsds-0.7.0b11/hsds/servicenode_lib.py` & `hsds-0.8.0/hsds/servicenode_lib.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,35 +6,36 @@
 # Utilities.  The full HSDS copyright notice, including                      #
 # terms governing use, modification, and redistribution, is contained in     #
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
-# service node of hsds cluster
+# utility methods for service node handlers
 #
-import os.path as op
-from aiohttp.web_exceptions import HTTPBadRequest, HTTPForbidden, HTTPNotFound
-from aiohttp.web_exceptions import HTTPInternalServerError
+
+from aiohttp.web_exceptions import HTTPBadRequest, HTTPForbidden
+from aiohttp.web_exceptions import HTTPNotFound, HTTPInternalServerError
 from aiohttp.client_exceptions import ClientOSError
 
 from .util.authUtil import getAclKeys
 from .util.idUtil import getDataNodeUrl, getCollectionForId, isSchema2Id
 from .util.idUtil import getS3Key
+from .util.linkUtil import h5Join
 from .util.storUtil import getStorJSONObj, isStorObj
 from .util.authUtil import aclCheck
 from .util.httpUtil import http_get
 from .util.domainUtil import getBucketForDomain, verifyRoot
 
 from . import hsds_logger as log
 
 
 async def getDomainJson(app, domain, reload=False):
-    """ Return domain JSON from cache or fetch from DN if not found
-        Note: only call from sn!
+    """Return domain JSON from cache or fetch from DN if not found
+    Note: only call from sn!
     """
     # TBD - default reload to True because some h5pyd tests fail due to
     # cached values being picked up (test case deletes/re-creates domain)
     # It would be desirable to use default of False to avoid extra
     # round-trips to DN node
     log.info(f"getDomainJson({domain}, reload={reload})")
     if app["node_type"] != "sn":
@@ -54,49 +55,70 @@
     req += "/domains"
     params = {"domain": domain}
 
     log.debug(f"sending dn req: {req} params: {params}")
 
     domain_json = await http_get(app, req, params=params)
 
-    if 'owner' not in domain_json:
+    if "owner" not in domain_json:
         log.warn("No owner key found in domain")
         raise HTTPInternalServerError()
 
-    if 'acls' not in domain_json:
+    if "acls" not in domain_json:
         log.warn("No acls key found in domain")
         raise HTTPInternalServerError()
 
     domain_cache[domain] = domain_json  # add to cache
     return domain_json
 
 
+def checkBucketAccess(app, bucket, action="read"):
+    """ if the given bucket is not the default bucket, check
+    that non-default bucket access is enabled.
+    Throw 403 error if not allowed """
+    if bucket and bucket != app["bucket_name"]:
+        # check that we are allowed to access non-default buckets
+        if action == "read":
+            if not app["allow_any_bucket_read"]:
+                log.warn(f"read access to non-default bucket: {bucket} not enabled")
+                raise HTTPForbidden()
+        else:
+            # write acction
+            if not app["allow_any_bucket_write"]:
+                log.warn(f"write access to non-default bucket: {bucket} not enabled")
+                raise HTTPForbidden()
+
+
 async def validateAction(app, domain, obj_id, username, action):
-    """ check that the given object belongs in the domain and that the
-        requested action (create, read, update, delete, readACL, udpateACL)
-        is permitted for the requesting user.
+    """check that the given object belongs in the domain and that the
+    requested action (create, read, update, delete, readACL, udpateACL)
+    is permitted for the requesting user.
     """
-    meta_cache = app['meta_cache']
+    meta_cache = app["meta_cache"]
     msg = f"validateAction(domain={domain}, obj_id={obj_id}, "
     msg += f"username={username}, action={action})"
     log.info(msg)
+    bucket = getBucketForDomain(domain)
+    if bucket:
+        checkBucketAccess(app, bucket, action=action)
+
     # get domain JSON
     domain_json = await getDomainJson(app, domain)
     verifyRoot(domain_json)
 
     obj_json = None
     if obj_id in meta_cache:
         log.debug(f"validateAction - found {obj_id} in meta_cache")
         obj_json = meta_cache[obj_id]
     else:
         # fetch from DN
         log.debug(f"validateAction - fetch {obj_id}")
         collection = getCollectionForId(obj_id)
         req = getDataNodeUrl(app, obj_id)
-        req += '/' + collection + '/' + obj_id
+        req += "/" + collection + "/" + obj_id
         bucket = getBucketForDomain(domain)
         params = {}
         if bucket:
             params["bucket"] = bucket
         obj_json = await http_get(app, req, params=params)
         meta_cache[obj_id] = obj_json
 
@@ -128,26 +150,28 @@
         # just in case the ACL was recently updated, refetch the domain
         reload = True
     if reload:
         domain_json = await getDomainJson(app, domain, reload=True)
         aclCheck(app, domain_json, action, username)
 
 
-async def getObjectJson(app, obj_id, bucket=None, refresh=False,
-                        include_links=False, include_attrs=False):
-    """ Return top-level json (i.e. excluding attributes or links by default)
-        for a given obj_id.
-        If refresh is False, any data present in the meta_cache will be
-        returned.  If not the DN will be queried, and any resultant data
-        added to the meta_cache.
-        Note: meta_cache values may be stale, but use of immutable data
-          (e.g. type of a dataset) is always valid
+async def getObjectJson(
+    app, obj_id, bucket=None, refresh=False, include_links=False, include_attrs=False
+):
+    """Return top-level json (i.e. excluding attributes or links by default)
+    for a given obj_id.
+    If refresh is False, any data present in the meta_cache will be
+    returned.  If not the DN will be queried, and any resultant data
+    added to the meta_cache.
+    Note: meta_cache values may be stale, but use of immutable data
+      (e.g. type of a dataset) is always valid
     """
-    meta_cache = app['meta_cache']
+    meta_cache = app["meta_cache"]
     obj_json = None
+
     if include_links or include_attrs:
         # links and attributes are subject to change, so always refresh
         refresh = True
     log.info(f"getObjectJson {obj_id}")
     if obj_id in meta_cache and not refresh:
         log.debug(f"found {obj_id} in meta_cache")
         obj_json = meta_cache[obj_id]
@@ -166,73 +190,191 @@
             raise HTTPInternalServerError()
         except ClientOSError as coe:
             log.error(f"Got ClientOSError: {coe}")
             raise HTTPInternalServerError()
     else:
         req = getDataNodeUrl(app, obj_id)
         collection = getCollectionForId(obj_id)
+
         params = {}
         if include_links:
             params["include_links"] = 1
         if include_attrs:
             params["include_attrs"] = 1
         if bucket:
             params["bucket"] = bucket
-        req += '/' + collection + '/' + obj_id
+        req += "/" + collection + "/" + obj_id
 
         # throws 404 if doesn't exist
         obj_json = await http_get(app, req, params=params)
         meta_cache[obj_id] = obj_json
     if obj_json is None:
-        msg = f"Object: {obj_id} not found"
+        msg = f"Object: {obj_id} not found, req: {req}, params: {params}"
         log.warn(msg)
         raise HTTPNotFound()
+
     return obj_json
 
 
-async def getObjectIdByPath(app, obj_id, h5path, bucket=None, refresh=False):
-    """ Find the object at the provided h5path location.
+async def getObjectIdByPath(app, obj_id, h5path, bucket=None, refresh=False, domain=None,
+                            follow_soft_links=False, follow_external_links=False):
+    """Find the object at the provided h5path location.
     If not found raise 404 error.
+    Returns a tuple of the object's id, the domain it is under,
+    and the json for the link to the object.
     """
-    msg = f"getObjectIdByPath obj_id: {obj_id} h5path: {h5path} "
+
+    msg = f"getObjectIdByPath obj_id: {obj_id} h5path: {h5path} in domain: {domain} "
     msg += f"refresh: {refresh}"
     log.info(msg)
+
+    if getCollectionForId(obj_id) != "groups":
+        # not a group, so won't have links
+        msg = f"h5path: {h5path} not found"
+        msg += f"getCollectionForId({obj_id}) returned {getCollectionForId(obj_id)}"
+        log.warn(msg)
+        raise HTTPNotFound()
+
     if h5path.startswith("./"):
         h5path = h5path[2:]  # treat as relative path
-    links = h5path.split('/')
+
+    links = h5path.split("/")
+    link_json = None
+
+    if h5path == "/":
+        log.debug("Root group requested by path")
+        ext_domain_json = await getDomainJson(app, domain)
+        return ext_domain_json["root"], domain, None
+
+    if h5path == ".":
+        log.debug("Group requested self by path")
+        return obj_id, domain, None
+
     for link in links:
         if not link:
             continue  # skip empty link
-        log.debug(f"getObjectIdByPath for objid: {obj_id} got link: {link}")
-        if getCollectionForId(obj_id) != "groups":
-            # not a group, so won't have links
-            msg = f"h5path: {h5path} not found"
-            log.warn(msg)
-            raise HTTPNotFound()
+
         req = getDataNodeUrl(app, obj_id)
         req += "/groups/" + obj_id + "/links/" + link
         log.debug("get LINK: " + req)
         params = {}
         if bucket:
             params["bucket"] = bucket
         link_json = await http_get(app, req, params=params)
-        log.debug("got link_json: " + str(link_json))
-        if link_json["class"] != 'H5L_TYPE_HARD':
-            # don't follow soft/external links
-            msg = f"h5path: {h5path} not found"
-            log.warn(msg)
+
+        if link_json["class"] == "H5L_TYPE_EXTERNAL":
+            if not follow_external_links:
+                msg = "Query found unexpected external link"
+                log.warn(msg)
+                raise HTTPBadRequest()
+
+            # find domain object is stored under
+            domain = link_json["h5domain"]
+
+            if bucket:
+                domain = bucket + domain
+
+            ext_domain_json = await getDomainJson(app, domain)
+
+            verifyRoot(ext_domain_json)
+
+            msg = f"external domain response = {ext_domain_json}"
+            log.debug(msg)
+
+            if link_json["h5path"][0] == '/':
+                msg = "External link by absolute path"
+                log.debug(msg)
+                obj_id, domain, link_json = await getObjectIdByPath(
+                    app, ext_domain_json["root"], link_json["h5path"],
+                    bucket=bucket, refresh=refresh, domain=domain,
+                    follow_soft_links=follow_soft_links,
+                    follow_external_links=follow_external_links)
+            else:
+                msg = "Cannot follow external link by relative path"
+                log.warn(msg)
+                raise HTTPInternalServerError()
+
+        elif link_json["class"] == "H5L_TYPE_SOFT":
+            if not follow_soft_links:
+                msg = "Query found unexpected soft link"
+                log.warn(msg)
+                raise HTTPBadRequest()
+
+            path_from_link = link_json["h5path"]
+
+            if path_from_link[0] != "/":
+                # If relative path, keep parent object the same
+                obj_id, domain, link_json = await getObjectIdByPath(
+                    app, obj_id, path_from_link, bucket=bucket,
+                    refresh=refresh, domain=domain,
+                    follow_soft_links=follow_soft_links,
+                    follow_external_links=follow_external_links)
+            else:
+                if not domain:
+                    msg = "Soft link with absolute path used with no domain given"
+                    log.warn(msg)
+                    raise HTTPInternalServerError()
+
+                # If absolute path, replace parent object with root group
+                domain_json = await getDomainJson(app, domain)
+                verifyRoot(domain_json)
+
+                obj_id, domain, link_json = await getObjectIdByPath(
+                    app, domain_json["root"], path_from_link,
+                    bucket=bucket, refresh=refresh, domain=domain,
+                    follow_soft_links=follow_soft_links,
+                    follow_external_links=follow_external_links)
+
+        elif link_json["class"] == "H5L_TYPE_HARD":
+            obj_id = link_json["id"]
+
+        else:
+            log.warn("Link has invalid type!")
             raise HTTPInternalServerError()
-        obj_id = link_json["id"]
-    # if we get here, we've traveresed the entire path and found the object
-    return obj_id
+
+    # If object at the end of the path was a symbolic link, search again under that link
+    if link_json and (link_json["class"] != "H5L_TYPE_HARD"):
+        log.debug("Recursing under symbolic link")
+        parent_id = None
+
+        if link_json["class"] == "H5L_TYPE_SOFT":
+
+            if link_json["h5path"][0] == '/':
+                domain_json = await getDomainJson(app, domain)
+                parent_id = domain_json["root"]
+            else:
+                parent_id = obj_id
+
+        elif link_json["class"] == "H5L_TYPE_EXTERNAL":
+            domain = link_json["h5domain"]
+
+            ext_domain_json = await getDomainJson(app, domain)
+            verifyRoot(ext_domain_json)
+
+            msg = f"external domain response = {ext_domain_json}"
+            log.debug(msg)
+
+            parent_id = ext_domain_json["root"]
+
+            if link_json["h5path"][0] != '/':
+                msg = "External link by relative path is unsupported"
+                log.warn(msg)
+                raise HTTPInternalServerError()
+
+        obj_id, domain, link_json = await getObjectIdByPath(
+            app, parent_id, link_json["h5path"],
+            bucket=bucket, refresh=refresh, domain=domain,
+            follow_soft_links=follow_soft_links,
+            follow_external_links=follow_external_links)
+
+    return obj_id, domain, link_json
 
 
-async def getPathForObjectId(app, parent_id, idpath_map, tgt_id=None,
-                             bucket=None):
-    """ Search the object starting with the given parent_id.
+async def getPathForObjectId(app, parent_id, idpath_map, tgt_id=None, bucket=None):
+    """Search the object starting with the given parent_id.
     idpath should be a dict with at minimum the key: parent_id: <parent_path>.
     If tgt_id is not None, returns first path that matches the tgt_id or
     None if not found.
     If Tgt_id is None, returns the idpath_map.
     """
 
     if not parent_id:
@@ -267,42 +409,42 @@
             continue  # ignore everything except hard links
         link_id = link["id"]
         if link_id in idpath_map:
             continue  # this node has already been visited
         title = link["title"]
         if tgt_id is not None and link_id == tgt_id:
             # found it!
-            h5path = op.join(parent_path, title)
+            h5path = h5Join(parent_path, title)
             break
-        idpath_map[link_id] = op.join(parent_path, title)
+        idpath_map[link_id] = h5Join(parent_path, title)
         if getCollectionForId(link_id) != "groups":
             continue
         # recursive call
         kwargs = {"tgt_id": tgt_id, "bucket": bucket}
         h5path = await getPathForObjectId(app, link_id, idpath_map, **kwargs)
         if tgt_id is not None and h5path:
             break
 
     return h5path
 
 
 async def getRootInfo(app, root_id, bucket=None):
-    """ Get extra information the root collection. """
+    """Get extra information the root collection."""
     # Gather additional info on the domain
     log.debug(f"getRootInfo {root_id}")
 
     if not isSchema2Id(root_id):
         msg = f"no dataset details not available for schema v1 id: {root_id} "
         msg += "returning null results"
         log.info(msg)
         return None
 
     s3_key = getS3Key(root_id)
 
-    parts = s3_key.split('/')
+    parts = s3_key.split("/")
     # dset_key is in the format  db/<root>/d/<dset>/.dataset.json
     # get the key for the root info object as: db/<root>/.info.json
     if len(parts) != 3:
         log.error(f"Unexpected s3key format: {s3_key}")
         return None
 
     info_key = f"db/{parts[1]}/.info.json"
```

### Comparing `hsds-0.7.0b11/hsds/util/__init__.py` & `hsds-0.8.0/hsds/util/__init__.py`

 * *Files identical despite different names*

### Comparing `hsds-0.7.0b11/hsds/util/arrayUtil.py` & `hsds-0.8.0/hsds/util/arrayUtil.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Utilities.  The full HSDS copyright notice, including                      #
 # terms governing use, modification, and redistribution, is contained in     #
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 
+import math
 import numpy as np
 
 MAX_VLEN_ELEMENT = 1000000  # restrict largest vlen element to one million
 
 """
 Convert list that may contain bytes type elements to list of string elements
 
@@ -56,17 +57,17 @@
 Example. [[1,2],[3,4]] -> ((1,2),(3,4))
 """
 
 
 def toTuple(rank, data):
     if type(data) in (list, tuple):
         if rank > 0:
-            return list(toTuple(rank-1, x) for x in data)
+            return list(toTuple(rank - 1, x) for x in data)
         else:
-            return tuple(toTuple(rank-1, x) for x in data)
+            return tuple(toTuple(rank - 1, x) for x in data)
     else:
         return data
 
 
 """
 Get size in bytes of a numpy array.
 """
@@ -102,30 +103,34 @@
   None for null dataspaces
 """
 
 
 def getShapeDims(shape):
     dims = None
     if isinstance(shape, int):
-        dims = [shape, ]
+        dims = [
+            shape,
+        ]
     elif isinstance(shape, list) or isinstance(shape, tuple):
         dims = shape  # can use as is
     elif isinstance(shape, str):
         # only valid string value is H5S_NULL
-        if shape != 'H5S_NULL':
+        if shape != "H5S_NULL":
             raise ValueError("Invalid value for shape")
         dims = None
     elif isinstance(shape, dict):
         if "class" not in shape:
             raise ValueError("'class' key not found in shape")
-        if shape["class"] == 'H5S_NULL':
+        if shape["class"] == "H5S_NULL":
             dims = None
-        elif shape["class"] == 'H5S_SCALAR':
-            dims = [1, ]
-        elif shape["class"] == 'H5S_SIMPLE':
+        elif shape["class"] == "H5S_SCALAR":
+            dims = [
+                1,
+            ]
+        elif shape["class"] == "H5S_SIMPLE":
             if "dims" not in shape:
                 raise ValueError("'dims' key expected for shape")
             dims = shape["dims"]
         else:
             raise ValueError("Unknown shape class: {}".format(shape["class"]))
     else:
         raise ValueError("Unexpected shape class: {}".format(type(shape)))
@@ -139,15 +144,15 @@
 
 
 def jsonToArray(data_shape, data_dtype, data_json):
     # utility function to initialize vlen array
     def fillVlenArray(rank, data, arr, index):
         for i in range(len(data)):
             if rank > 1:
-                index = fillVlenArray(rank-1, data[i], arr, index)
+                index = fillVlenArray(rank - 1, data[i], arr, index)
             else:
                 arr[index] = data[i]
                 index += 1
         return index
 
     # need some special conversion for compound types --
     # each element must be a tuple, but the JSON decoder
@@ -161,15 +166,17 @@
         converted_data = []
         if npoints == 1 and len(data_json) == len(data_dtype):
             converted_data.append(toTuple(0, data_json))
         else:
             converted_data = toTuple(np_shape_rank, data_json)
         data_json = converted_data
     else:
-        data_json = [data_json, ]  # listify
+        data_json = [
+            data_json,
+        ]  # listify
 
     if isVlen(data_dtype):
         arr = np.zeros((npoints,), dtype=data_dtype)
         fillVlenArray(np_shape_rank, data_json, arr, 0)
     else:
         try:
             arr = np.array(data_json, dtype=data_dtype)
@@ -177,15 +184,15 @@
             msg = "Unable to encode data"
             raise ValueError(msg) from ude
     # raise an exception of the array shape doesn't match the selection shape
     # allow if the array is a scalar and the selection shape is one element,
     # numpy is ok with this
     if arr.size != npoints:
         msg = "Input data doesn't match selection number of elements"
-        msg += " Expected {}, but received: {}".format(npoints, arr.size)
+        msg += f" Expected {npoints}, but received: {arr.size}"
         raise ValueError(msg)
     if arr.shape != data_shape:
         arr = arr.reshape(data_shape)  # reshape to match selection
 
     return arr
 
 
@@ -230,18 +237,18 @@
             if e == 0:
                 count = 4  # non-initialized element
             else:
                 raise ValueError("Unexpected value: {}".format(e))
         elif isinstance(e, bytes):
             count = len(e) + 4
         elif isinstance(e, str):
-            count = len(e.encode('utf-8')) + 4
+            count = len(e.encode("utf-8")) + 4
         elif isinstance(e, np.ndarray):
-            nElements = np.prod(e.shape)
-            if e.dtype.kind != 'O':
+            nElements = math.prod(e.shape)
+            if e.dtype.kind != "O":
                 count = e.dtype.itemsize * nElements
             else:
                 arr1d = e.reshape((nElements,))
                 count = 0
                 for item in arr1d:
                     count += getElementSize(item, dt)
             count += 4  # byte count
@@ -260,16 +267,16 @@
 """
 Get number of bytes needed to store given numpy array as a bytestream
 """
 
 
 def getByteArraySize(arr):
     if not isVlen(arr.dtype):
-        return arr.itemsize * np.prod(arr.shape)
-    nElements = np.prod(arr.shape)
+        return arr.itemsize * math.prod(arr.shape)
+    nElements = math.prod(arr.shape)
     # reshape to 1d for easier iteration
     arr1d = arr.reshape((nElements,))
     dt = arr1d.dtype
     count = 0
     for e in arr1d:
         count += getElementSize(e, dt)
     return count
@@ -280,15 +287,15 @@
 """
 
 
 def copyBuffer(src, des, offset):
     # print(f"copyBuffer - src: {src} offset: {offset}")
     # TBD: just do: des[offset:] = src[:]  ?
     for i in range(len(src)):
-        des[i+offset] = src[i]
+        des[i + offset] = src[i]
 
     # print("returning:", offset + len(src))
     return offset + len(src)
 
 
 """
 Copy element to bytearray
@@ -320,38 +327,38 @@
         # variable length element
         vlen = dt.metadata["vlen"]
         # print("copyBuffer vlen:", vlen)
         if isinstance(e, int):
             # print("copyBuffer int")
             if e == 0:
                 # write 4-byte integer 0 to buffer
-                offset = copyBuffer(b'\x00\x00\x00\x00', buffer, offset)
+                offset = copyBuffer(b"\x00\x00\x00\x00", buffer, offset)
             else:
                 raise ValueError("Unexpected value: {}".format(e))
         elif isinstance(e, bytes):
             # print("copyBuffer bytes")
             count = np.int32(len(e))
             if count > MAX_VLEN_ELEMENT:
                 raise ValueError("vlen element too large")
             offset = copyBuffer(count.tobytes(), buffer, offset)
             offset = copyBuffer(e, buffer, offset)
         elif isinstance(e, str):
             # print("copyBuffer, str")
-            text = e.encode('utf-8')
+            text = e.encode("utf-8")
             count = np.int32(len(text))
             if count > MAX_VLEN_ELEMENT:
                 raise ValueError("vlen element too large")
             offset = copyBuffer(count.tobytes(), buffer, offset)
             offset = copyBuffer(text, buffer, offset)
 
         elif isinstance(e, np.ndarray):
-            nElements = np.prod(e.shape)
+            nElements = math.prod(e.shape)
             # print("copyBuffer ndarray, nElements:", nElements)
 
-            if e.dtype.kind != 'O':
+            if e.dtype.kind != "O":
                 count = np.int32(e.dtype.itemsize * nElements)
                 # print("copyBuffeer got vlen count:", count)
                 # print("copyBuffer e:", e)
                 if count > MAX_VLEN_ELEMENT:
                     raise ValueError("vlen element too large")
                 offset = copyBuffer(count.tobytes(), buffer, offset)
                 # print("copyBuffer write new count, offset:", offset)
@@ -380,18 +387,20 @@
 
 """
 Get the count value from persisted vlen array
 """
 
 
 def getElementCount(buffer, offset):
-    count_bytes = bytes(buffer[offset:(offset+4)])
+    n = offset
+    m = offset + 4
+    count_bytes = bytes(buffer[n:m])
 
     try:
-        count = int(np.frombuffer(count_bytes, dtype="<i4"))
+        count = int(np.frombuffer(count_bytes, dtype="<i4")[0])
     except TypeError as e:
         msg = f"Unexpected error reading count value for varlen element: {e}"
         raise TypeError(msg)
     if count < 0:
         # shouldn't be negative
         raise ValueError(f"Unexpected count value for varlen element: {count}")
     if count > MAX_VLEN_ELEMENT:
@@ -411,38 +420,42 @@
     if len(dt) > 1:
         e = arr[index]
         for name in dt.names:
             field_dt = dt[name]
             offset = readElement(buffer, offset, e, name, field_dt)
     elif not dt.metadata or "vlen" not in dt.metadata:
         count = dt.itemsize
-        e_buffer = buffer[offset:(offset+count)]
+        n = offset
+        m = offset + count
+        e_buffer = buffer[n:m]
         offset += count
         try:
             e = np.frombuffer(bytes(e_buffer), dtype=dt)
             arr[index] = e[0]
         except ValueError:
             print(f"ERROR: ValueError setting {e_buffer} and dtype: {dt}")
             raise
     else:
         # variable length element
         vlen = dt.metadata["vlen"]
         e = arr[index]
 
         if isinstance(e, np.ndarray):
-            nelements = np.prod(dt.shape)
+            nelements = math.prod(dt.shape)
             e.reshape((nelements,))
             for i in range(nelements):
                 offset = readElement(buffer, offset, e, i, dt)
             e.reshape(dt.shape)
         else:
             count = getElementCount(buffer, offset)
             offset += 4
+            n = offset
+            m = offset + count
             if count > 0:
-                e_buffer = buffer[offset:(offset+count)]
+                e_buffer = buffer[n:m]
                 offset += count
 
                 if vlen is bytes:
                     arr[index] = bytes(e_buffer)
                 elif vlen is str:
                     s = e_buffer.decode("utf-8")
                     arr[index] = s
@@ -466,15 +479,15 @@
     if not isVlen(arr.dtype):
         # can just return normal numpy bytestream
         return arr.tobytes()
 
     nSize = getByteArraySize(arr)
     buffer = bytearray(nSize)
     offset = 0
-    nElements = np.prod(arr.shape)
+    nElements = math.prod(arr.shape)
     arr1d = arr.reshape((nElements,))
     for e in arr1d:
         # print("arrayToBytes:", e)
         offset = copyElement(e, arr1d.dtype, buffer, offset)
     return bytes(buffer)
 
 
@@ -496,15 +509,15 @@
             offset = readElement(data, offset, arr, index, dt)
     arr = arr.reshape(shape)
     # check that we can update the array if needed
     # Note: this seems to have been required starting with numpuy v 1.17
     # Setting the flag directly is not recommended.
     # cf: https://github.com/numpy/numpy/issues/9440
 
-    if not arr.flags['WRITEABLE']:
+    if not arr.flags["WRITEABLE"]:
         arr_copy = arr.copy()
         arr = arr_copy
 
     return arr
 
 
 """
@@ -524,7 +537,139 @@
     for extent in data.shape:
         if extent == 1:
             can_reduce = True
         break
     if can_reduce:
         data = data.squeeze()
     return data
+
+
+class IndexIterator(object):
+    """
+    Class to iterate through list of chunks of a given dataset
+    """
+
+    def __init__(self, shape, sel=None):
+        self._shape = shape
+        self._rank = len(self._shape)
+        self._stop = False
+
+        if self._rank < 1:
+            raise ValueError("IndexIterator can not be used on arrays of zero rank")
+
+        if sel is None:
+            # select over entire dataset
+            slices = []
+            for dim in range(self._rank):
+                slices.append(slice(0, self._shape[dim]))
+            self._sel = tuple(slices)
+        else:
+            if isinstance(sel, slice):
+                self._sel = (sel,)
+            else:
+                self._sel = sel
+        if len(self._sel) != self._rank:
+            raise ValueError("Invalid selection - selection region must have same rank as shape")
+        self._index = []
+        for dim in range(self._rank):
+            s = self._sel[dim]
+            if s.start < 0 or s.stop > self._shape[dim] or s.stop <= s.start:
+                raise ValueError(
+                    "Invalid selection - selection region must be within dataset space"
+                )
+            self._index.append(s.start)
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self._stop:
+            raise StopIteration()
+        # bump up the last index and carry forward if we run outside the selection
+        dim = self._rank - 1
+        ret_index = self._index.copy()
+        while True:
+            s = self._sel[dim]
+            if s.step:
+                step = s.step
+            else:
+                step = 1
+            self._index[dim] += step
+
+            if self._index[dim] < s.stop:
+                # we still have room to extend along this dimensions
+                break
+
+            # reset to the start and continue iterating with higher dimension
+            self._index[dim] = s.start
+            dim -= 1
+            if dim < 0:
+                # ran past last index, stop iteration on next run
+                self._stop = True
+
+        return tuple(ret_index)
+
+
+# compare two numpy arrays.
+# return true if the same (exclusive of null vs. empty array)
+# false otherwise
+# TBD: this is slow for multi-megabyte vlen arrays, needs to be optimized
+
+
+def ndarray_compare(arr1, arr2):
+    if not isinstance(arr1, np.ndarray) and not isinstance(arr2, np.ndarray):
+        if not isinstance(arr1, np.void) and not isinstance(arr2, np.void):
+            return arr1 == arr2
+        if isinstance(arr1, np.void) and not isinstance(arr2, np.void):
+            if arr1.size == 0 and not arr2:
+                return True
+            else:
+                return False
+        if not isinstance(arr1, np.void) and isinstance(arr2, np.void):
+            if not arr1 and arr2.size == 0:
+                return True
+            else:
+                return False
+        # both np.voids
+        if arr1.size != arr2.size:
+            return False
+
+        if len(arr1) != len(arr2):
+            return False
+
+        for i in range(len(arr1)):
+            if not ndarray_compare(arr1[i], arr2[i]):
+                return False
+        return True
+
+    if isinstance(arr1, np.ndarray) and not isinstance(arr2, np.ndarray):
+        # same only if arr1 is empty and arr2 is 0
+        if arr1.size == 0 and not arr2:
+            return True
+        else:
+            return False
+    if not isinstance(arr1, np.ndarray) and isinstance(arr2, np.ndarray):
+        # same only if arr1 is empty and arr2 size is 0
+        if not arr1 and arr2.size == 0:
+            return True
+        else:
+            return False
+
+    # two ndarrays...
+    if arr1.shape != arr2.shape:
+        return False
+    if arr2.dtype != arr2.dtype:
+        return False
+
+    if isVlen(arr1.dtype):
+        # need to compare element by element
+
+        nElements = np.prod(arr1.shape)
+        arr1 = arr1.reshape((nElements,))
+        arr2 = arr2.reshape((nElements,))
+        for i in range(nElements):
+            if not ndarray_compare(arr1[i], arr2[i]):
+                return False
+        return True
+    else:
+        # can just us np array_compare
+        return np.array_equal(arr1, arr2)
```

### Comparing `hsds-0.7.0b11/hsds/util/attrUtil.py` & `hsds-0.8.0/hsds/util/attrUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,44 +15,44 @@
 
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPInternalServerError
 
 from .. import hsds_logger as log
 
 
 def getRequestCollectionName(request):
-    """ request is in the form:
+    """request is in the form:
         /(datasets|groups|datatypes)/<id>/attributes(/<name>),
     return: "datasets" | "groups" | "types"
     """
     uri = request.path
 
-    npos = uri.find('/')
+    npos = uri.find("/")
     if npos < 0:
         msg = "bad request uri"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    uri = uri[(npos+1):]
-    npos = uri.find('/')  # second '/'
+    npos += 1
+    uri = uri[npos:]
+    npos = uri.find("/")  # second '/'
     col_name = uri[:npos]
 
-    log.debug('got collection name: [' + col_name + ']')
-    if col_name not in ('datasets', 'groups', 'datatypes'):
-        msg = "Error: collection name unexpected: {}".format(col_name)
+    log.debug(f"got collection name: [{col_name}]")
+    if col_name not in ("datasets", "groups", "datatypes"):
+        msg = f"Error: collection name unexpected: {col_name}"
         log.error(msg)
         # shouldn't get routed here in this case
         raise HTTPInternalServerError()
 
     return col_name
 
 
 def validateAttributeName(name):
-    """ verify that the attribute name is valid
-    """
+    """verify that the attribute name is valid"""
     if not isinstance(name, str):
         msg = f"attribute name must be a string, but got: {type(name)}"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    if name.find('/') > -1:
+    if name.find("/") > -1:
         msg = "attribute names cannot contain slashes"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
     # TBD - add any other restrictions
```

### Comparing `hsds-0.7.0b11/hsds/util/authUtil.py` & `hsds-0.8.0/hsds/util/authUtil.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 GROUP_PREFIX = "g:"
 
 # keys used for each ACL
 ACL_KEYS = ("create", "read", "update", "delete", "readACL", "updateACL")
 
 
 def getDynamoDBClient(app):
-    """ Return dynamodb handle
-    """
+    """Return dynamodb handle"""
     if "session" not in app:
         session = get_session()
         app["session"] = session
     else:
         session = app["session"]
 
     if "dynamodb" in app:
@@ -59,107 +58,111 @@
     aws_secret_access_key = None
     aws_access_key_id = None
     aws_session_token = None
     aws_iam_role = config.get("aws_iam_role")
     log.info(f"using iam role: {aws_iam_role}")
     aws_secret_access_key = config.get("aws_secret_access_key")
     aws_access_key_id = config.get("aws_access_key_id")
-    if not aws_secret_access_key or aws_secret_access_key == 'xxx':
+    if not aws_secret_access_key or aws_secret_access_key == "xxx":
         log.info("aws secret access key not set")
         aws_secret_access_key = None
-    if not aws_access_key_id or aws_access_key_id == 'xxx':
+    if not aws_access_key_id or aws_access_key_id == "xxx":
         log.info("aws access key id not set")
         aws_access_key_id = None
 
     if aws_iam_role and not aws_secret_access_key:
         # TODO - refactor with similar code in s3Util
         log.info("getted EC2 IAM role credentials")
         # Use EC2 IAM role to get credentials
         # See: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/
         #    iam-roles-for-amazon-ec2.html?icmpid=docs_ec2_console
         req = "http://169.254.169.254/"
         req += f"latest/meta-data/iam/security-credentials/{aws_iam_role}"
         curl_cmd = ["curl", req]
-        p = subprocess.run(curl_cmd, stdout=subprocess.PIPE,
-                           stderr=subprocess.PIPE)
+        p = subprocess.run(curl_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         if p.returncode != 0:
             msg = f"Error getting IAM role credentials: {p.stderr}"
             log.error(msg)
         else:
             stdout = p.stdout.decode("utf-8")
             try:
                 cred = json.loads(stdout)
                 aws_secret_access_key = cred["SecretAccessKey"]
                 aws_access_key_id = cred["AccessKeyId"]
-                log.info(f"Got ACCESS_KEY_ID: {aws_access_key_id} \
-                    from EC2 metadata")
+                log.info(
+                    f"Got ACCESS_KEY_ID: {aws_access_key_id} \
+                    from EC2 metadata"
+                )
                 aws_session_token = cred["Token"]
                 log.info("Got Expiration of: {}".format(cred["Expiration"]))
                 # trim off 'Z' and add 'UTC'
                 expiration_str = cred["Expiration"][:-1] + "UTC"
                 # save the expiration
                 fmt = "%Y-%m-%dT%H:%M:%S%Z"
-                app["token_expiration"] = \
-                    datetime.datetime.strptime(expiration_str, fmt)
+                app["token_expiration"] = datetime.datetime.strptime(
+                    expiration_str, fmt
+                )
             except json.JSONDecodeError:
                 msg = f"Unexpected error decoding EC2 meta-data response: \
 {stdout}"
                 log.error(msg)
             except KeyError:
                 msg = f"Missing expected key from EC2 meta-data response: \
 {stdout}"
                 log.error(msg)
 
-    dynamodb_gateway = config.get('aws_dynamodb_gateway')
+    dynamodb_gateway = config.get("aws_dynamodb_gateway")
     if not dynamodb_gateway:
         msg = "Invalid aws dynamodb gateway"
         log.error(msg)
         raise ValueError(msg)
     use_ssl = False
     if dynamodb_gateway.startswith("https"):
         use_ssl = True
-    kwargs = {"region_name": aws_region,
-              "aws_secret_access_key": aws_secret_access_key,
-              "aws_access_key_id": aws_access_key_id,
-              "aws_session_token": aws_session_token,
-              "endpoint_url": dynamodb_gateway,
-              "use_ssl": use_ssl}
+    kwargs = {
+        "region_name": aws_region,
+        "aws_secret_access_key": aws_secret_access_key,
+        "aws_access_key_id": aws_access_key_id,
+        "aws_session_token": aws_session_token,
+        "endpoint_url": dynamodb_gateway,
+        "use_ssl": use_ssl,
+    }
 
-    dynamodb = session.create_client('dynamodb',  **kwargs)
+    dynamodb = session.create_client("dynamodb", **kwargs)
     # save so same client can be returned in subsiquent calls
-    app['dynamodb'] = dynamodb
+    app["dynamodb"] = dynamodb
 
     return dynamodb
 
 
 def releaseDynamoDBClient(app):
-    """ release the client collection to dynamoDB
-     (Used for cleanup on application exit)
+    """release the client collection to dynamoDB
+    (Used for cleanup on application exit)
     """
-    if 'dynamodb' in app:
-        client = app['dynamodb']
+    if "dynamodb" in app:
+        client = app["dynamodb"]
         client.close()
-        del app['dynamodb']
+        del app["dynamodb"]
 
 
 def loadPasswordFile(password_file):
     log.info(f"using password file: {password_file}")
     line_num = 0
     user_db = {}
     try:
         with open(password_file) as f:
             for line in f:
                 line_num += 1
                 s = line.strip()
                 if not s:
                     continue
-                if s[0] == '#':
+                if s[0] == "#":
                     # comment line
                     continue
-                fields = s.split(':')
+                fields = s.split(":")
                 if len(fields) < 2:
                     msg = f"line: {line_num} of {password_file} is not valid"
                     log.warn(msg)
                     continue
                 username = fields[0]
                 passwd = fields[1]
                 if len(username) < 3 or len(passwd) < 3:
@@ -187,16 +190,15 @@
     """
     log.info("initUserDB")
     if "user_db" in app:
         msg = "user_db already initilized"
         log.warn(msg)
         return
 
-    if config.get("aws_dynamodb_gateway") and \
-            config.get("aws_dynamodb_users_table"):
+    if config.get("aws_dynamodb_gateway") and config.get("aws_dynamodb_users_table"):
         # user entries will be obtained dynamicaly
         log.info("Getting DynamoDB client")
         # get client here so any errors will be seen right away
         getDynamoDBClient(app)
         user_db = {}
     elif config.get("password_salt"):
         # use salt key to verify passwords
@@ -266,45 +268,44 @@
         # look up name in dynamodb table
         dynamodb = getDynamoDBClient(app)
         table_name = config.get("aws_dynamodb_users_table")
         msg = f"looking for user: {username} in DynamoDB table: {table_name}"
         log.info(msg)
         try:
             response = await dynamodb.get_item(
-                TableName=table_name,
-                Key={'username': {'S': username}}
+                TableName=table_name, Key={"username": {"S": username}}
             )
         except ClientError as e:
-            msg = e.response['Error']['Message']
+            msg = e.response["Error"]["Message"]
             log.error(f"Unable to read dyanamodb table: {msg}")
             raise HTTPInternalServerError()  # 500
         if "Item" not in response:
             log.info(f"user: {username} not found")
             raise HTTPUnauthorized()  # 401
-        item = response['Item']
+        item = response["Item"]
         if "password" not in item:
             log.error("Expected to find password key in DynamoDB table")
             raise HTTPInternalServerError()  # 500
         password_item = item["password"]
-        if 'S' not in password_item:
+        if "S" not in password_item:
             log.error("Expected to find 'S' key for password item")
             raise HTTPInternalServerError()  # 500
         log.debug(f"password: {password_item}")
-        if password_item['S'] != password:
+        if password_item["S"] != password:
             log.warn(f"user password is not valid for user: {username}")
             raise HTTPUnauthorized()  # 401
         # add user/password to user_db map
         setPassword(app, username, password)
 
 
 def validatePasswordSHA512(app, username, password):
     if getPassword(app, username) is None:
         log.info(f"SHA512 check for username: {username}")
         salt = config.get("password_salt")
-        hash_str = username.encode('utf-8') + salt.encode('utf-8')
+        hash_str = username.encode("utf-8") + salt.encode("utf-8")
         hex_hash = hashlib.sha512(hash_str).hexdigest()
         if hex_hash[:32] != password:
             msg = "user password is not valid (didn't equal sha512 hash) for "
             msg += f"user: {username}"
             log.warn(msg)
             raise HTTPUnauthorized()  # 401
         setPassword(app, username, password)
@@ -316,18 +317,18 @@
         throws exception if not valid
     Note: make this async since we'll eventually need some sort of http
         request to validate user/passwords
     """
     log.debug(f"validateUserPassword username: {username}")
 
     if not username:
-        log.info('validateUserPassword - null user')
+        log.info("validateUserPassword - null user")
         raise HTTPUnauthorized()
     if not password:
-        log.info('isPasswordValid - null password')
+        log.info("isPasswordValid - null password")
         raise HTTPUnauthorized()
 
     log.debug(f"looking up username: {username}")
     if "user_db" not in app:
         msg = "user_db not intialized"
         log.error(msg)
         raise HTTPInternalServerError()  # 500
@@ -344,15 +345,15 @@
         elif config.get("password_salt"):
             validatePasswordSHA512(app, username, password)
         else:
             log.warn(f"user: {username} not found")
             raise HTTPUnauthorized()  # 401
         user_data = getPassword(app, username)
 
-    if user_data['pwd'] == password:
+    if user_data["pwd"] == password:
         log.debug("user password validated")
     else:
         log.info(f"user password is not valid for user: {username}")
         raise HTTPUnauthorized()  # 401
 
 
 def _checkTokenCache(app, token):
@@ -377,15 +378,15 @@
         if "pwd" not in user:
             msg = "expected to find key: 'pwd' in user data "
             msg += f"for user: {username}"
             log.warn(msg)
             continue
         if "pwd" not in user or user["pwd"] != token:
             continue
-        pwd = user['pwd']
+        pwd = user["pwd"]
 
         if time.time() < exp:
             # still valid!
             if pwd == token:
                 log.info(f"returning user: {username} from bearer cache")
                 user_id = username
         else:
@@ -413,25 +414,25 @@
         with open(group_file) as f:
             for line in f:
                 line_number += 1
                 s = line.strip()
                 if not s:
                     continue
                 log.debug(f"group[{line_number}]: {s}")
-                if s[0] == '#':
+                if s[0] == "#":
                     # comment line
                     continue
-                fields = s.split(':')
+                fields = s.split(":")
                 if len(fields) < 2:
                     msg = f"line: {line_number} is not valid"
                     log.warn(msg)
                     continue
                 group_name = fields[0]
                 users = fields[1]
-                user_names = users.split(' ')
+                user_names = users.split(" ")
                 log.debug(f"group: {group_name} users: {user_names}")
 
                 if group_name in group_db:
                     msg = f"line: {line_number} of {group_file} "
                     msg += f"group name: {group_name} is repeated"
                     log.warn(msg)
                 else:
@@ -483,90 +484,90 @@
             users.add(group_name)
     app["user_group_db"] = user_group_db
 
     log.info(f"group_db initialized: {len(group_user_db)} groups")
 
 
 def getUserPasswordFromRequest(request):
-    """ Return user defined in Auth header (if any)
-    """
+    """Return user defined in Auth header (if any)"""
     user = None
     pswd = None
     app = request.app
-    if 'Authorization' not in request.headers:
-        log.debug("no Authorization in header")
+    if "Authorization" not in request.headers:
+        # log.debug("no Authorization in header")
         return None, None
-    scheme, _, token = request.headers.get('Authorization', '').partition(' ')
+    scheme, _, token = request.headers.get("Authorization", "").partition(" ")
     if not scheme or not token:
-        log.info("Invalid Authorization header")
+        # log.info("Invalid Authorization header")
         raise HTTPBadRequest(reason="Invalid Authorization header")
 
-    if scheme.lower() == 'basic':
-        log.debug("using basic authorization")
+    if scheme.lower() == "basic":
+        # log.debug("using basic authorization")
         # HTTP Basic Auth
         try:
-            token = token.encode('utf-8')  # convert to bytes
+            token = token.encode("utf-8")  # convert to bytes
             token_decoded = base64.decodebytes(token)
         except binascii.Error:
             msg = "Malformed authorization header"
-            log.warn(msg)
+            # log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-        if token_decoded.index(b':') < 0:
+        if token_decoded.index(b":") < 0:
             msg = "Malformed authorization header (No ':' character)"
-            log.warn(msg)
+            # log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-        user, _, pswd = token_decoded.partition(b':')
+        user, _, pswd = token_decoded.partition(b":")
         if not user or not pswd:
             msg = "Malformed authorization header, user/password not found"
-            log.warn(msg)
+            # log.warn(msg)
             raise HTTPBadRequest(reason=msg)
-        user = user.decode('utf-8')   # convert bytes to string
-        pswd = pswd.decode('utf-8')   # convert bytes to string
+        user = user.decode("utf-8")  # convert bytes to string
+        pswd = pswd.decode("utf-8")  # convert bytes to string
 
-    elif scheme.lower() == 'bearer':
+    elif scheme.lower() == "bearer":
         # OpenID Auth.
-        log.debug(f"Got OpenID bearer token: {token}")
+        # log.debug("Got OpenID bearer token")
         user_group_db = app["user_group_db"]
 
         # see if we've already validated this token
         user = _checkTokenCache(app, token)
         if user:
             # set password to token value
             pswd = token
         else:
             # put import here to avoid jwt package dependency unless required
             from .jwtUtil import verifyBearerToken
+
             user, exp, roles = verifyBearerToken(app, token)
             if exp:
                 msg = f"decoded bearer token for user: {user}, expired: {exp}"
-                log.info(msg)
+                # log.info(msg)
                 setPassword(app, user, token, scheme="bearer", exp=exp)
             else:
                 msg = f"decoded bearer token for user: {user}, no expiration"
-                log.info(msg)
+                # log.info(msg)
                 setPassword(app, user, token, scheme="bearer")
             if user:
                 pswd = token
             if roles:
                 if user not in user_group_db:
                     user_group_db[user] = set()
                 user_group = user_group_db[user]
                 for role in roles:
                     user_group.add(role)
 
     else:
         msg = f"Unsupported Authorization header scheme: {scheme}"
-        log.warn(msg)
+        # log.warn(msg)
         raise HTTPBadRequest(reason=msg)
 
     return user, pswd
 
 
 def isAdminUser(app, username):
-    """ Return true if user is an admin """
+    """Return true if user is an admin"""
     if not username:
         return False
     if username == config.get("admin_user"):
         return True
     admin_group = config.get("admin_group")
     if not admin_group:
         return False
@@ -638,16 +639,15 @@
                 raise HTTPBadRequest(reason=msg)
             acl_value = acl[acl_key]
             if acl_value not in (True, False):
                 msg = f"Invalid ACL value: {acl_value}"
 
 
 def aclOpForRequest(request):
-    """ return default ACL action for request method
-    """
+    """return default ACL action for request method"""
     req_action = None
     if request.method == "GET":
         req_action = "read"
     elif request.method == "PUT":
         req_action = "create"
     elif request.method == "POST":
         req_action = "create"
```

### Comparing `hsds-0.7.0b11/hsds/util/awsLambdaClient.py` & `hsds-0.8.0/hsds/util/awsLambdaClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,48 +39,47 @@
     except KeyError:
         pass
     try:
         aws_region = config.get("aws_region")
     except KeyError:
         pass
     try:
-        max_pool_connections = config.get('aio_max_pool_connections')
+        max_pool_connections = config.get("aio_max_pool_connections")
     except KeyError:
         pass
     log.info(f"Lambda client init - aws_region {aws_region}")
 
-    lambda_gateway = config.get('aws_lambda_gateway')
+    lambda_gateway = config.get("aws_lambda_gateway")
     if not lambda_gateway:
         msg = "Invalid aws lambda gateway"
         log.error(msg)
         raise ValueError(msg)
     log.info(f"Using AWS Lambda Gateway: {lambda_gateway}")
 
     use_ssl = False
     if lambda_gateway.startswith("https"):
         use_ssl = True
 
-    if not aws_secret_access_key or aws_secret_access_key == 'xxx':
+    if not aws_secret_access_key or aws_secret_access_key == "xxx":
         log.info("aws secret access key not set")
         aws_secret_access_key = None
-    if not aws_access_key_id or aws_access_key_id == 'xxx':
+    if not aws_access_key_id or aws_access_key_id == "xxx":
         log.info("aws access key id not set")
         aws_access_key_id = None
 
     if aws_iam_role and not aws_secret_access_key:
         log.info(f"using iam role: {aws_iam_role}")
         log.info("getting EC2 IAM role credentials")
         # Use EC2 IAM role to get credentials
         # See: "https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ \
         # iam-roles-for-amazon-ec2.html?icmpid=docs_ec2_console
         req = "http://169.254.169.254/"
         req += f"latest/meta-data/iam/security-credentials/{aws_iam_role}"
         curl_cmd = ["curl", req]
-        p = subprocess.run(curl_cmd, stdout=subprocess.PIPE,
-                           stderr=subprocess.PIPE)
+        p = subprocess.run(curl_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         if p.returncode != 0:
             msg = f"Error getting IAM role credentials: {p.stderr}"
             log.error(msg)
         else:
             stdout = p.stdout.decode("utf-8")
             try:
                 cred = json.loads(stdout)
@@ -89,34 +88,37 @@
                 aws_cred_expiration = cred["Expiration"]
                 aws_session_token = cred["Token"]
                 log.info(f"Got Expiration of: {aws_cred_expiration}")
                 # trim off 'Z' and add 'UTC'
                 expiration_str = aws_cred_expiration[:-1] + "UTC"
                 # save the expiration
                 app["lambda_token_expiration"] = datetime.datetime.strptime(
-                        expiration_str, "%Y-%m-%dT%H:%M:%S%Z")
+                    expiration_str, "%Y-%m-%dT%H:%M:%S%Z"
+                )
             except json.JSONDecodeError:
                 msg = "Unexpected error decoding EC2 meta-data response"
                 log.error(msg)
             except KeyError:
                 msg = "Missing expected key from EC2 meta-data response"
                 log.error(msg)
     aws_region = config.get("aws_region")
     if not aws_region:
         aws_region = "us-east-1"
 
-    max_pool_connections = config.get('aio_max_pool_connections')
+    max_pool_connections = config.get("aio_max_pool_connections")
     aio_config = AioConfig(max_pool_connections=max_pool_connections)
-    kwargs = {"region_name": aws_region,
-              "aws_secret_access_key": aws_secret_access_key,
-              "aws_access_key_id": aws_access_key_id,
-              "aws_session_token": aws_session_token,
-              "use_ssl": use_ssl,
-              "config": aio_config}
-    lambda_client = session.create_client('lambda', **kwargs)
+    kwargs = {
+        "region_name": aws_region,
+        "aws_secret_access_key": aws_secret_access_key,
+        "aws_access_key_id": aws_access_key_id,
+        "aws_session_token": aws_session_token,
+        "use_ssl": use_ssl,
+        "config": aio_config,
+    }
+    lambda_client = session.create_client("lambda", **kwargs)
 
     # TBD - we are getting errors if we try to reuse lambda client
     # app["lambda"] = lambda_client
     return lambda_client
 
 
 """
@@ -136,16 +138,15 @@
 
         self.session = app["session"]
 
         if "lambda_stats" not in app:
             app["lambda_stats"] = {}
         lambda_stats = app["lambda_stats"]
         if self.lambdaFunction not in lambda_stats:
-            lambda_stats[self.lambdaFunction] = \
-                {"cnt": 0, "inflight": 0, "failed": 0}
+            lambda_stats[self.lambdaFunction] = {"cnt": 0, "inflight": 0, "failed": 0}
         self.funcStats = lambda_stats[self.lambdaFunction]
 
     async def __aenter__(self):
         start_time = time.time()
         payload = json.dumps(self.params)
         msg = f"invoking lambda function {self.lambdaFunction} "
         msg += "with payload: {self.params} start: {start_time}"
```

### Comparing `hsds-0.7.0b11/hsds/util/azureBlobClient.py` & `hsds-0.8.0/hsds/util/azureBlobClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from aiohttp.web_exceptions import HTTPNotFound, HTTPForbidden
 from aiohttp.web_exceptions import HTTPInternalServerError, HTTPBadRequest
 from .. import config
 
 CALLBACK_MAX_COUNT = 1000  # compatible with S3 batch size
 
 
-class AzureBlobClient():
+class AzureBlobClient:
     """
-     Utility class for reading and storing data to AzureStorage Blobs
+    Utility class for reading and storing data to AzureStorage Blobs
     """
 
     def __init__(self, app):
 
         self._app = app
 
         if "azureBlobClient" in app:
@@ -40,54 +40,68 @@
                 return
 
         # first time setup of Azure client or limited time token has expired
 
         # TBD - what do do about region?
         log.info("AzureBlobClient init")
 
-        azure_connection_string = config.get('azure_connection_string')
+        azure_connection_string = config.get("azure_connection_string")
         if not azure_connection_string:
             msg = "No connection string specified"
             log.error(msg)
             raise ValueError(msg)
-        log.info(f"Using azure_connection_string: {azure_connection_string}")
+        log.info(f"Using azure_connection_string: {'*'*len(azure_connection_string)}")
 
-        self._client = BlobServiceClient.from_connection_string(
-            azure_connection_string)
+        self._client = BlobServiceClient.from_connection_string(azure_connection_string)
 
         # save so same client can be returned in subsequent calls
-        app['azureBlobClient'] = self._client
+        app["azureBlobClient"] = self._client
 
     def _azure_stats_increment(self, counter, inc=1):
-        """ Incremenet the indicated connter
-        """
+        """Incremenet the indicated connter"""
         if "azure_stats" not in self._app:
             # setup stats
             azure_stats = {}
             azure_stats["get_count"] = 0
             azure_stats["put_count"] = 0
             azure_stats["delete_count"] = 0
             azure_stats["list_count"] = 0
             azure_stats["error_count"] = 0
             azure_stats["bytes_in"] = 0
             azure_stats["bytes_out"] = 0
             self._app["azure_stats"] = azure_stats
-        azure_stats = self._app['azure_stats']
+        azure_stats = self._app["azure_stats"]
         if counter not in azure_stats:
             log.error(f"unexpected counter for azure_stats: {counter}")
             return
         if inc < 1:
             log.error(f"unexpected inc for azure_stats: {inc}")
             return
 
         azure_stats[counter] += inc
 
+    def getURIFromKey(self, key, bucket=None):
+        """ return Azure specific URI for given key and bucket """
+        if not bucket:
+            log.error("getURIFromKey, bucket not set")
+            raise HTTPInternalServerError()
+        if not key:
+            log.error("getURIFromKey, key not set")
+            raise HTTPInternalServerError()
+        if key[0] == "/":
+            key = key[1:]
+
+        # TBD - do the proper azure specific uri
+
+        uri = f"{bucket}/{key}"
+        return uri
+
     async def get_object(self, key, bucket=None, offset=0, length=-1):
-        """ Return data for object at given key.
-           If Range is set, return the given byte range.
+        """Return data for object at given key.
+        If Range is set, return the given byte range.
         """
         if not bucket:
             log.error("get_object - bucket not set")
             raise HTTPInternalServerError()
 
         if length > 0:
             msg = f"storage range request -- offset: {offset} length: {length}"
@@ -138,37 +152,35 @@
                 msg += f"get_object {key}: {e}"
                 log.error(msg)
                 raise HTTPInternalServerError()
 
         return data
 
     async def put_object(self, key, data, bucket=None):
-        """ Write data to given key.
-            Returns client specific dict on success
+        """Write data to given key.
+        Returns client specific dict on success
         """
         if not bucket:
             log.error("put_object - bucket not set")
             raise HTTPInternalServerError()
 
         start_time = time.time()
         msg = f"azureBlobClient.put_object({bucket}/{key} start: {start_time}"
         log.debug(msg)
         try:
             kwargs = {"container": bucket, "blob": key}
             async with self._client.get_blob_client(**kwargs) as blob_client:
-                kwargs = {"blob_type": 'BlockBlob', "overwrite": True}
+                kwargs = {"blob_type": "BlockBlob", "overwrite": True}
                 blob_rsp = await blob_client.upload_blob(data, **kwargs)
 
             finish_time = time.time()
             ETag = blob_rsp["etag"]
             lastModified = int(blob_rsp["last_modified"].timestamp())
             data_size = len(data)
-            rsp = {"ETag": ETag,
-                   "size": data_size,
-                   "LastModified": lastModified}
+            rsp = {"ETag": ETag, "size": data_size, "LastModified": lastModified}
             log.debug(f"put_object {key} returning: {rsp}")
             msg = f"azureBlobClient.put_object({key} bucket={bucket}) "
             msg += f"start={start_time:.4f} finish={finish_time:.4f} "
             msg += "elapsed={finish_time-start_time:.4f} "
             msg += f"bytes={len(data)}"
             log.info(msg)
 
@@ -201,27 +213,25 @@
 
         if data and len(data) > 0:
             self._azure_stats_increment("bytes_out", inc=len(data))
         log.debug(f"azureBlobClient.put_object {key} complete, rsp: {rsp}")
         return rsp
 
     async def delete_object(self, key, bucket=None):
-        """ Deletes the object at the given key
-        """
+        """Deletes the object at the given key"""
         if not bucket:
             log.error("delete_object - bucket not set")
             raise HTTPInternalServerError()
 
         start_time = time.time()
         msg = f"azureBlobClient.delete_object({bucket}/{key} "
         msg += f"start: {start_time}"
         log.debug(msg)
         try:
-            async with self._client.get_container_client(container=bucket) as \
-                                                              client:
+            async with self._client.get_container_client(container=bucket) as client:
                 await client.delete_blob(blob=key)
             finish_time = time.time()
             msg = f"azureBlobClient.delete_object({key} bucket={bucket}) "
             msg += f"start={start_time:.4f} finish={finish_time:.4f} "
             msg += f"elapsed={finish_time-start_time:.4f}"
             log.info(msg)
 
@@ -251,16 +261,15 @@
             else:
                 msg = "azureBlobClient.Unexpected exception for "
                 msg += f"put_object {key}: {e}"
                 log.error(msg)
                 raise HTTPInternalServerError()
 
     async def is_object(self, key, bucket=None):
-        """ Return true if the given object exists
-        """
+        """Return true if the given object exists"""
         if not bucket:
             log.error("is_object - bucket not set")
             raise HTTPInternalServerError()
         start_time = time.time()
         found = False
         try:
             kwargs = {"container": bucket, "blob": key}
@@ -303,16 +312,15 @@
         msg += f"start={start_time:.4f} finish={finish_time:.4f} "
         msg += f"elapsed={finish_time-start_time:.4f}"
         log.info(msg)
 
         return found
 
     async def get_key_stats(self, key, bucket=None):
-        """ Get ETag, size, and last modified time for given objecct
-        """
+        """Get ETag, size, and last modified time for given objecct"""
         start_time = time.time()
         key_stats = {}
         try:
             kwargs = {"container": bucket, "blob": key}
             async with self._client.get_blob_client(**kwargs) as blob_client:
                 blob_props = await blob_client.get_blob_properties()
             finish_time = time.time()
@@ -359,42 +367,51 @@
         msg = f"azureBlobClient.get_key_stats({key} bucket={bucket}) "
         msg += f"start={start_time:.4f} finish={finish_time:.4f} "
         msg += f"elapsed={finish_time-start_time:.4f}"
         log.info(msg)
 
         return key_stats
 
-    async def walk_blobs(self, client, prefix="", suffix="",
-                         include_stats=False, deliminator='/', callback=None):
+    async def walk_blobs(
+        self,
+        client,
+        prefix="",
+        suffix="",
+        include_stats=False,
+        deliminator="/",
+        callback=None,
+    ):
         continuation_token = None
         count = 0
         while True:
-            kwargs = {"name_starts_with": prefix, "delimiter": deliminator,
-                      "results_per_page": CALLBACK_MAX_COUNT}
-            keyList = client.walk_blobs(**kwargs).\
-                by_page(continuation_token)
+            kwargs = {
+                "name_starts_with": prefix,
+                "delimiter": deliminator,
+                "results_per_page": CALLBACK_MAX_COUNT,
+            }
+            keyList = client.walk_blobs(**kwargs).by_page(continuation_token)
             key_names = {} if include_stats else []
             async for key in await keyList.__anext__():
                 key_name = key["name"]
                 log.debug(f"walk_blobs got: {key_name}")
                 if include_stats:
                     ETag = key["etag"]
                     lastModified = int(key["last_modified"].timestamp())
                     data_size = key["size"]
                     key_tags = {
                         "ETag": ETag,
                         "Size": data_size,
-                        "LastModified": lastModified
-                        }
+                        "LastModified": lastModified,
+                    }
                     key_names[key_name] = key_tags
                 else:
                     if suffix and not key_name.endswith(suffix):
                         log.debug(f"skip name that doesn't end with {suffix}")
                         continue
-                    if deliminator and key_name[-1] != '/':
+                    if deliminator and key_name[-1] != "/":
                         log.debug("skip name thaat doesn't end in '/'")
                         # only return folders
                         continue
                     if len(key_names) >= CALLBACK_MAX_COUNT:
                         break
                     key_names.append(key_name)
                     count += 1
@@ -415,52 +432,58 @@
         log.info(f"walk_blob_hierarchy, returning {count} items")
         if not callback and count != len(key_names):
             msg = f"expected {count} keys in return list "
             msg += f"but got {len(key_names)}"
             log.warning(msg)
         return key_names
 
-    async def walk_blob_hierarchy(self, client, prefix="",
-                                  include_stats=False, callback=None):
+    async def walk_blob_hierarchy(
+        self, client, prefix="", include_stats=False, callback=None
+    ):
         log.info(f"walk_blob_hierarchy, prefix: {prefix}")
 
         key_names = None
 
         async def do_callback(callback, keynames):
             if iscoroutinefunction(callback):
                 await callback(self._app, key_names)
             else:
                 callback(self._app, key_names)
 
         key_names = key_names = {} if include_stats else []
         count = 0
         async for item in client.walk_blobs(name_starts_with=prefix):
-            short_name = item.name[len(prefix):]
+            nlen = len(prefix)
+            short_name = item.name[nlen:]
             if isinstance(item, BlobPrefix):
                 log.debug(f"walk_blob_hierarchy - BlobPrefix: {short_name}")
-                kwargs = {"prefix": item.name,
-                          "include_stats": include_stats,
-                          "callback": callback}
+                kwargs = {
+                    "prefix": item.name,
+                    "include_stats": include_stats,
+                    "callback": callback,
+                }
                 key_names = await self.walk_blob_hierarchy(client, **kwargs)
             else:
                 kwargs = {"nme_starts_with": item.name}
                 async for item in client.list_blobs(**kwargs):
-                    key_name = item['name']
+                    key_name = item["name"]
                     log.debug(f"walk_blob_hierarchy - got name: {key_name}")
                     if include_stats:
                         ETag = item["etag"]
                         lastModified = int(item["last_modified"].timestamp())
                         data_size = item["size"]
-                        key_tags = {"ETag": ETag,
-                                    "Size": data_size,
-                                    "LastModified": lastModified}
+                        key_tags = {
+                            "ETag": ETag,
+                            "Size": data_size,
+                            "LastModified": lastModified,
+                        }
                         key_names[key_name] = key_tags
                     else:
                         # just add the blob name to the list
-                        key_names.append(item['name'])
+                        key_names.append(item["name"])
                     count += 1
                     if callback and len(key_names) >= CALLBACK_MAX_COUNT:
                         msg = "walk_blob_hierarchy, invoking callback "
                         msg += f"with {len(key_names)} items"
                         log.debug(msg)
                         await do_callback(callback, key_names)
                         key_names = key_names = {} if include_stats else []
@@ -475,42 +498,50 @@
         if not callback and count != len(key_names):
             msg = f"expected {count} keys in return list "
             msg += f"but got {len(key_names)}"
             log.warning(msg)
 
         return key_names
 
-    async def list_keys(self, prefix='', deliminator='', suffix='',
-                        include_stats=False, callback=None,
-                        bucket=None, limit=None):
-        """ return keys matching the arguments
-        """
+    async def list_keys(
+        self,
+        prefix="",
+        deliminator="",
+        suffix="",
+        include_stats=False,
+        callback=None,
+        bucket=None,
+        limit=None,
+    ):
+        """return keys matching the arguments"""
         if not bucket:
             log.error("list_keys - bucket not set")
             raise HTTPInternalServerError()
         msg = f"list_keys('{prefix}','{deliminator}','{suffix}', "
         msg += f"include_stats={include_stats}, callback "
         msg += f"{'set' if callback is not None else 'not set'}"
         log.info(msg)
-        if deliminator and deliminator != '/':
+        if deliminator and deliminator != "/":
             msg = "Only '/' is supported as deliminator"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         key_names = None
 
-        if prefix == '':
+        if prefix == "":
             prefix = None  # azure sdk expects None for no prefix
 
         try:
             kwargs = {"container": bucket}
             async with self._client.get_container_client(**kwargs) as client:
-                kwargs = {"prefix": prefix,
-                          "deliminator": deliminator,
-                          "include_stats": include_stats,
-                          "callback": callback}
+                kwargs = {
+                    "prefix": prefix,
+                    "deliminator": deliminator,
+                    "include_stats": include_stats,
+                    "callback": callback,
+                }
                 key_names = await self.walk_blobs(client, **kwargs)
                 # key_names = await self.walk_blob_hierarchy(client, **kwargs)
         except CancelledError as cle:
             self._azure_stats_increment("error_count")
             msg = f"azureBlobClient.CancelledError for list_keys: {cle}"
             log.error(msg)
             raise HTTPInternalServerError()
@@ -546,15 +577,15 @@
                     del key_names[k]
             else:
                 key_names = key_names[:limit]
 
         return key_names
 
     async def releaseClient(self):
-        """ release the client collection to Azure Blob Storage
-           (Used for cleanup on application exit)
+        """release the client collection to Azure Blob Storage
+        (Used for cleanup on application exit)
         """
         log.info("release AzureBlobClient")
-        if 'azureBlobClient' in self._app:
-            client = self._app['azureBlobClient']
+        if "azureBlobClient" in self._app:
+            client = self._app["azureBlobClient"]
             await client.close()
-            del self._app['azureBlobClient']
+            del self._app["azureBlobClient"]
```

### Comparing `hsds-0.7.0b11/hsds/util/boolparser.py` & `hsds-0.8.0/hsds/util/boolparser.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   p = BooleanParser('<expression text>')
   p.evaluate(variable_dict) # variable_dict is a dictionary providing values
                             # for variables that appear in <expression text>
 """
 
 
 class TokenType:
-    NUM, STR, VAR, GT, GTE, LT, LTE, EQ, NEQ, LP, RP, AND, OR = range(13)
+    NUM, STR, BYTE, VAR, GT, GTE, LT, LTE, EQ, NEQ, LP, RP, AND, OR = range(14)
 
 
 class TreeNode:
     tokenType = None
     value = None
     left = None
     right = None
@@ -33,70 +33,82 @@
     i = 0
 
     def __init__(self, exp):
         self.expression = exp
 
     def next(self):
         self.i += 1
-        return self.tokens[self.i-1]
+        return self.tokens[self.i - 1]
 
     def peek(self):
         return self.tokens[self.i]
 
     def hasNext(self):
         return self.i < len(self.tokens)
 
     def nextTokenType(self):
         return self.tokenTypes[self.i]
 
     def nextTokenTypeIsOperator(self):
         t = self.tokenTypes[self.i]
-        return t == TokenType.GT or t == TokenType.GTE \
-            or t == TokenType.LT or t == TokenType.LTE \
-            or t == TokenType.EQ or t == TokenType.NEQ
+        return t in (
+            TokenType.GT,
+            TokenType.GTE,
+            TokenType.LT,
+            TokenType.LTE,
+            TokenType.EQ,
+            TokenType.NEQ,
+        )
 
     def tokenize(self):
         import re
-        reg = re.compile(r'(\bAND\b|\bOR\b|!=|==|<=|>=|<|>|\(|\))')
+
+        reg = re.compile(r"(\bAND\b|\bOR\b|!=|==|<=|>=|<|>|\(|\)|\&|\|)")
         SINGLE_QUOTE = "'"
         DOUBLE_QUOTE = '"'
         self.tokens = reg.split(self.expression)
-        self.tokens = [t.strip() for t in self.tokens if t.strip() != '']
+        self.tokens = [t.strip() for t in self.tokens if t.strip() != ""]
 
         self.tokenTypes = []
         for i in range(len(self.tokens)):
             t = self.tokens[i]
-            if t == 'AND':
+            if t in ("AND", "&"):
                 self.tokenTypes.append(TokenType.AND)
-            elif t == 'OR':
+            elif t in ("OR", "|"):
                 self.tokenTypes.append(TokenType.OR)
-            elif t == '(':
+            elif t == "(":
                 self.tokenTypes.append(TokenType.LP)
-            elif t == ')':
+            elif t == ")":
                 self.tokenTypes.append(TokenType.RP)
-            elif t == '<':
+            elif t == "<":
                 self.tokenTypes.append(TokenType.LT)
-            elif t == '<=':
+            elif t == "<=":
                 self.tokenTypes.append(TokenType.LTE)
-            elif t == '>':
+            elif t == ">":
                 self.tokenTypes.append(TokenType.GT)
-            elif t == '>=':
+            elif t == ">=":
                 self.tokenTypes.append(TokenType.GTE)
-            elif t == '==':
+            elif t == "==":
                 self.tokenTypes.append(TokenType.EQ)
-            elif t == '!=':
+            elif t == "!=":
                 self.tokenTypes.append(TokenType.NEQ)
             else:
                 # number of string or variable
                 if t[0] == SINGLE_QUOTE and t[-1] == SINGLE_QUOTE:
                     self.tokenTypes.append(TokenType.STR)
                     self.tokens[i] = t[1:-1]  # strip quotes
                 elif t[0] == DOUBLE_QUOTE and t[-1] == DOUBLE_QUOTE:
                     self.tokenTypes.append(TokenType.STR)
                     self.tokens[i] = t[1:-1]  # strip quotes
+                elif len(t) > 3 and all(
+                    (t[0] == "b", t[1] == SINGLE_QUOTE, t[-1] == SINGLE_QUOTE)
+                ):
+                    # binary string
+                    self.tokenTypes.append(TokenType.BYTE)
+                    self.tokens[i] = t[2:-1]  # strip quotes and 'b'
                 else:
                     try:
                         float(t)
                         self.tokenTypes.append(TokenType.NUM)
                     except Exception:
                         self.tokenTypes.append(TokenType.VAR)
 
@@ -123,90 +135,90 @@
         self.root = self.parseExpression()
 
     def getVariables(self):
         return self.tokenizer.getVariables()
 
     def parseExpression(self):
         andTerm1 = self.parseAndTerm()
-        while self.tokenizer.hasNext() and \
-                self.tokenizer.nextTokenType() == TokenType.OR:
+        while (
+            self.tokenizer.hasNext() and self.tokenizer.nextTokenType() == TokenType.OR
+        ):
             self.tokenizer.next()
             andTermX = self.parseAndTerm()
             andTerm = TreeNode(TokenType.OR)
             andTerm.left = andTerm1
             andTerm.right = andTermX
             andTerm1 = andTerm
         return andTerm1
 
     def parseAndTerm(self):
         condition1 = self.parseCondition()
-        while self.tokenizer.hasNext() and \
-                self.tokenizer.nextTokenType() == TokenType.AND:
+        while (
+            self.tokenizer.hasNext() and self.tokenizer.nextTokenType() == TokenType.AND
+        ):
             self.tokenizer.next()
             conditionX = self.parseCondition()
             condition = TreeNode(TokenType.AND)
             condition.left = condition1
             condition.right = conditionX
             condition1 = condition
         return condition1
 
     def parseCondition(self):
-        if self.tokenizer.hasNext() and \
-               self.tokenizer.nextTokenType() == TokenType.LP:
+        if self.tokenizer.hasNext() and self.tokenizer.nextTokenType() == TokenType.LP:
             self.tokenizer.next()
             expression = self.parseExpression()
-            if self.tokenizer.hasNext() and \
-                    self.tokenizer.nextTokenType() == TokenType.RP:
+            next_token = None
+            if self.tokenizer.hasNext():
+                next_token = self.tokenizer.nextTokenType()
+            if next_token == TokenType.RP:
                 self.tokenizer.next()
                 return expression
             else:
                 msg = "Closing ) expected, but got " + self.tokenizer.next()
                 raise Exception(msg)
 
         terminal1 = self.parseTerminal()
-        if self.tokenizer.hasNext() and \
-                self.tokenizer.nextTokenTypeIsOperator():
+        if self.tokenizer.hasNext() and self.tokenizer.nextTokenTypeIsOperator():
             condition = TreeNode(self.tokenizer.nextTokenType())
             self.tokenizer.next()
             terminal2 = self.parseTerminal()
             condition.left = terminal1
             condition.right = terminal2
             return condition
         else:
-            msg = 'Operator expected, but got ' + self.tokenizer.next()
+            msg = "Operator expected, but got " + self.tokenizer.next()
             raise Exception(msg)
 
     def parseTerminal(self):
         if self.tokenizer.hasNext():
             tokenType = self.tokenizer.nextTokenType()
             if tokenType == TokenType.NUM:
                 n = TreeNode(tokenType)
                 n.value = float(self.tokenizer.next())
                 return n
-            elif tokenType == TokenType.STR or tokenType == TokenType.VAR:
+            elif tokenType in (TokenType.STR, TokenType.BYTE, TokenType.VAR):
                 n = TreeNode(tokenType)
                 n.value = self.tokenizer.next()
                 return n
             else:
-                msg = 'NUM, STR, or VAR expected, but got '
+                msg = "NUM, STR, or VAR expected, but got "
                 msg += self.tokenizer.next()
                 raise Exception(msg)
         else:
-            msg = 'NUM, STR, or VAR expected, but got ' + self.tokenizer.next()
+            msg = "NUM, STR, or VAR expected, but got " + self.tokenizer.next()
             raise Exception(msg)
 
     def evaluate(self, variable_dict):
         return self.evaluateRecursive(self.root, variable_dict)
 
     def evaluateRecursive(self, treeNode, variable_dict):
-        if treeNode.tokenType == TokenType.NUM:
-            return treeNode.value
-        if treeNode.tokenType == TokenType.STR:
-            # strip off outer quotes for evaluation
+        if treeNode.tokenType in (TokenType.NUM, TokenType.STR, TokenType.BYTE):
             return treeNode.value
+
         if treeNode.tokenType == TokenType.VAR:
             return variable_dict.get(treeNode.value)
 
         left = self.evaluateRecursive(treeNode.left, variable_dict)
         right = self.evaluateRecursive(treeNode.right, variable_dict)
 
         if treeNode.tokenType == TokenType.GT:
@@ -222,8 +234,48 @@
         elif treeNode.tokenType == TokenType.NEQ:
             return left != right
         elif treeNode.tokenType == TokenType.AND:
             return left and right
         elif treeNode.tokenType == TokenType.OR:
             return left or right
         else:
-            raise Exception('Unexpected type ' + str(treeNode.tokenType))
+            raise Exception("Unexpected type " + str(treeNode.tokenType))
+
+    def getEvalRecursive(self, treeNode):
+        if treeNode.tokenType == TokenType.NUM:
+            return treeNode.value
+        if treeNode.tokenType == TokenType.STR:
+            # add quotes for evaluation
+            return f"'{treeNode.value}'"
+        if treeNode.tokenType == TokenType.BYTE:
+            return f"b'{treeNode.value}'"
+        if treeNode.tokenType == TokenType.VAR:
+            return treeNode.value
+
+        left = self.getEvalRecursive(treeNode.left)
+        if isinstance(left, str) and " " in left:
+            left = f"({left})"
+        right = self.getEvalRecursive(treeNode.right)
+        if isinstance(right, str) and " " in right:
+            right = f"({right})"
+
+        if treeNode.tokenType == TokenType.GT:
+            return f"{left} > {right}"
+        elif treeNode.tokenType == TokenType.GTE:
+            return f"{left} >= {right}"
+        elif treeNode.tokenType == TokenType.LT:
+            return f"{left} < {right}"
+        elif treeNode.tokenType == TokenType.LTE:
+            return f"{left} <= {right}"
+        elif treeNode.tokenType == TokenType.EQ:
+            return f"{left} == {right}"
+        elif treeNode.tokenType == TokenType.NEQ:
+            return f"{left} != {right}"
+        elif treeNode.tokenType == TokenType.AND:
+            return f"{left} & {right}"
+        elif treeNode.tokenType == TokenType.OR:
+            return f"{left} | {right}"
+        else:
+            raise Exception("Unexpected type " + str(treeNode.tokenType))
+
+    def getEvalStr(self):
+        return self.getEvalRecursive(self.root)
```

### Comparing `hsds-0.7.0b11/hsds/util/chunkUtil.py` & `hsds-0.8.0/hsds/util/chunkUtil.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from .. import hsds_logger as log
+from .arrayUtil import ndarray_compare
 
-CHUNK_BASE = 16*1024     # Multiplier by which chunks are adjusted
-CHUNK_MIN = 512*1024     # Soft lower limit (512k)
-CHUNK_MAX = 2048*1024    # Hard upper limit (2M)
+CHUNK_BASE = 16 * 1024  # Multiplier by which chunks are adjusted
+CHUNK_MIN = 512 * 1024  # Soft lower limit (512k)
+CHUNK_MAX = 2048 * 1024  # Hard upper limit (2M)
 DEFAULT_TYPE_SIZE = 128  # Type size case when it is variable
 PRIMES = [29, 31, 37, 41, 43, 47, 53, 59, 61, 67]  # for chunk partitioning
 
 
 """
 Convert list that may contain bytes type elements to list of string elements
 
@@ -42,58 +43,58 @@
     else:
         out = data
 
     return out
 
 
 def getChunkSize(layout, type_size):
-    """ Return chunk size given layout.
+    """Return chunk size given layout.
     i.e. just the product of the values in the list.
     """
-    if type_size == 'H5T_VARIABLE':
+    if type_size == "H5T_VARIABLE":
         type_size = DEFAULT_TYPE_SIZE
 
     chunk_size = type_size
     for n in layout:
         if n <= 0:
             raise ValueError("Invalid chunk layout")
         chunk_size *= n
     return chunk_size
 
 
 def get_dset_size(shape_json, typesize):
-    """ Return the size of the dataspace.  For
-        any unlimited dimensions, assume a value of 1.
-        (so the return size will be the absolute minimum)
+    """Return the size of the dataspace.  For
+    any unlimited dimensions, assume a value of 1.
+    (so the return size will be the absolute minimum)
     """
-    if shape_json is None or shape_json["class"] == 'H5S_NULL':
+    if shape_json is None or shape_json["class"] == "H5S_NULL":
         return None
-    if shape_json["class"] == 'H5S_SCALAR':
+    if shape_json["class"] == "H5S_SCALAR":
         return typesize  # just return size for one item
-    if typesize == 'H5T_VARIABLE':
+    if typesize == "H5T_VARIABLE":
         typesize = DEFAULT_TYPE_SIZE  # just take a guess at the item size
     dset_size = typesize
     shape = shape_json["dims"]
     rank = len(shape)
 
     for n in range(rank):
         if shape[n] == 0:
             # extendable extent with value of 0
             continue  # assume this is one
         dset_size *= shape[n]
     return dset_size
 
 
-def expandChunk(layout, typesize, shape_json,
-                chunk_min=CHUNK_MIN, layout_class='H5D_CHUNKED'):
-    """ Extend the chunk shape until it is above the MIN target.
-    """
-    if shape_json is None or shape_json["class"] == 'H5S_NULL':
+def expandChunk(
+    layout, typesize, shape_json, chunk_min=CHUNK_MIN, layout_class="H5D_CHUNKED"
+):
+    """Extend the chunk shape until it is above the MIN target."""
+    if shape_json is None or shape_json["class"] == "H5S_NULL":
         return None
-    if shape_json["class"] == 'H5S_SCALAR':
+    if shape_json["class"] == "H5S_SCALAR":
         return (1,)  # just enough to store one item
 
     layout = list(layout)
     dims = shape_json["dims"]
     rank = len(dims)
     extendable_dims = 0  # number of dimensions that are extenable
     maxdims = None
@@ -156,18 +157,16 @@
         elif chunk_size > chunk_min:
             break  # we're good
         else:
             pass  # do another round
     return tuple(layout)
 
 
-def shrinkChunk(layout, typesize,
-                chunk_max=CHUNK_MAX, layout_class='H5D_CHUNKED'):
-    """ Shrink the chunk shape until it is less than the MAX target.
-    """
+def shrinkChunk(layout, typesize, chunk_max=CHUNK_MAX, layout_class="H5D_CHUNKED"):
+    """Shrink the chunk shape until it is less than the MAX target."""
     layout = list(layout)
     chunk_size = getChunkSize(layout, typesize)
     if chunk_size <= chunk_max:
         return tuple(layout)  # good already
     rank = len(layout)
 
     while chunk_size > chunk_max:
@@ -185,72 +184,75 @@
         if chunk_size >= old_chunk_size:
             # reality check to see if we'll ever break out of the while loop
             log.warning("Unexpected error in shrink_chunk")
             break
         elif chunk_size <= chunk_max:
             break  # we're good
         else:
-            pass   # do another round
+            pass  # do another round
     return tuple(layout)
 
 
 def guessChunk(shape_json, typesize):
-    """ Guess an appropriate chunk layout for a dataset, given its shape and
+    """Guess an appropriate chunk layout for a dataset, given its shape and
     the size of each element in bytes.  Will allocate chunks only as large
     as MAX_SIZE.  Chunks are generally close to some power-of-2 fraction of
     each axis, slightly favoring bigger values for the last index.
 
     Undocumented and subject to change without warning.
     """
-    if shape_json is None or shape_json["class"] == 'H5S_NULL':
+    if shape_json is None or shape_json["class"] == "H5S_NULL":
         return None
-    if shape_json["class"] == 'H5S_SCALAR':
+    if shape_json["class"] == "H5S_SCALAR":
         return (1,)  # just enough to store one item
 
     if "maxdims" in shape_json:
         shape = shape_json["maxdims"]
     else:
         shape = shape_json["dims"]
 
-    if typesize == 'H5T_VARIABLE':
+    if typesize == "H5T_VARIABLE":
         typesize = 128  # just take a guess at the item size
 
     # For unlimited dimensions we have to guess. use 1024
     shape = tuple((x if x != 0 else 1024) for i, x in enumerate(shape))
 
     return shape
 
 
-def getContiguousLayout(shape_json, item_size,
-                        chunk_min=1000*1000, chunk_max=4*1000*1000):
+def getContiguousLayout(
+    shape_json, item_size, chunk_min=1000 * 1000, chunk_max=4 * 1000 * 1000
+):
     """
     create a chunklayout for datasets use continguous storage.
     """
     if not isinstance(item_size, int):
         msg = "ContiguousLayout can only be used with fixed-length types"
         raise ValueError(msg)
     if chunk_max < chunk_min:
         raise ValueError("chunk_max cannot be less than chunk_min")
-    if shape_json is None or shape_json["class"] == 'H5S_NULL':
+    if shape_json is None or shape_json["class"] == "H5S_NULL":
         return None
-    if shape_json["class"] == 'H5S_SCALAR':
+    if shape_json["class"] == "H5S_SCALAR":
         return (1,)  # just enough to store one item
     dims = shape_json["dims"]
     rank = len(dims)
     if rank == 0:
         raise ValueError("rank must be positive for Contiguous Layout")
     for dim in dims:
         if dim < 0:
             raise ValueError("extents must be positive for Contiguous Layout")
         if dim == 0:
             # datashape with no elements, just return dims as layout
             return dims
 
     nsize = item_size
-    layout = [1, ] * rank
+    layout = [
+        1,
+    ] * rank
 
     for i in range(rank):
         dim = rank - i - 1
         extent = dims[dim]
         if extent * nsize < chunk_max:
             # just use the full extent as layout
             layout[dim] = extent
@@ -268,23 +270,23 @@
 
 
 def frac(x, d):
     """
     Utility func -- Works like fractional div, but returns ceiling
     rather than floor
     """
-    return (x + (d-1)) // d
+    return (x + (d - 1)) // d
 
 
 def slice_stop(s):
-    """ Return the end of slice, accounting that for steps > 1, this may not
-        be the slice stop value.
+    """Return the end of slice, accounting that for steps > 1, this may not
+    be the slice stop value.
     """
     if s.step > 1:
-        num_points = frac((s.stop-s.start), s.step)
+        num_points = frac((s.stop - s.start), s.step)
         w = num_points * s.step - (s.step - 1)
     else:
         w = s.stop - s.start  # selection width (>0)
     return s.start + w
 
 
 def getNumChunks(selection, layout):
@@ -293,29 +295,29 @@
     If selection is provided (a list of slices), return the number
     of chunks that intersect with the selection.
     """
 
     # do a quick check that we don't have a null selection space'
     # TBD: this needs to be revise to do the right think with stride > 1
     for s in selection:
-        if isinstance(s,slice):
+        if isinstance(s, slice):
             if s.stop <= s.start:
                 log.debug("null selection")
                 return 0
         else:
             # coordinate list
             if len(s) == 0:
                 return 0
     num_chunks = 1
     for i in range(len(selection)):
         s = selection[i]
-        c = layout[i]   # chunk size
+        c = layout[i]  # chunk size
         if isinstance(s, slice):
             if s.step > 1:
-                num_points = frac((s.stop-s.start), s.step)
+                num_points = frac((s.stop - s.start), s.step)
                 w = num_points * s.step - (s.step - 1)
             else:
                 w = s.stop - s.start  # selection width (>0)
 
             lc = frac(s.start, c) * c
 
             if s.start + w <= lc:
@@ -343,84 +345,83 @@
                     last_chunk = this_chunk
 
         num_chunks *= count
     return num_chunks
 
 
 def getChunkId(dset_id, point, layout):
-    """ get chunkid for given point in the dataset
-    """
+    """get chunkid for given point in the dataset"""
 
-    chunk_id = "c-" + dset_id[2:] + '_'
+    chunk_id = "c-" + dset_id[2:] + "_"
     rank = len(layout)
 
     for dim in range(rank):
         coord = None
         if rank == 1:
             coord = point  # integer for 1d dataset
         else:
             coord = point[dim]
         c = layout[dim]
         chunk_index = int(coord) // c
         chunk_id += str(chunk_index)
         if dim + 1 < rank:
-            chunk_id += '_'  # seperate dimensions with underscores
+            chunk_id += "_"  # seperate dimensions with underscores
 
     return chunk_id
 
 
 def getDatasetId(chunk_id):
-    """ Get dataset id given a chunk id
-    """
-    n = chunk_id.find('-') + 1
+    """Get dataset id given a chunk id"""
+    n = chunk_id.find("-") + 1
     if n <= 0:
         raise ValueError("Unexpected chunk id")
-    obj_uuid = chunk_id[n:(36+n)]
+    m = n + 36
+    obj_uuid = chunk_id[n:m]
     dset_id = "d-" + obj_uuid
     return dset_id
 
 
 def getChunkIndex(chunk_id):
-    """ given a chunk_id (e.g.: c-12345678-1234-1234-1234-1234567890ab_6_4)
+    """given a chunk_id (e.g.: c-12345678-1234-1234-1234-1234567890ab_6_4)
     return the coordinates of the chunk. In this case (6,4)
     """
     # go to the first underscore
-    n = chunk_id.find('_') + 1
+    n = chunk_id.find("_") + 1
     if n == 0:
-        raise ValueError("Invalid chunk_id: {}".format(chunk_id))
+        raise ValueError(f"Invalid chunk_id: {chunk_id}")
     suffix = chunk_id[n:]
 
     index = []
-    parts = suffix.split('_')
+    parts = suffix.split("_")
     for part in parts:
         index.append(int(part))
 
     return index
 
 
 def getChunkPartition(chunk_id):
-    """ return partition (if any) for the given chunk id.
+    """return partition (if any) for the given chunk id.
     Parition is encoded in digits after the initial 'c' character.
     E.g. for:  c56-12345678-1234-1234-1234-1234567890ab_6_4, the
     partition would be 56.
     For c-12345678-1234-1234-1234-1234567890ab_6_4, the
     partition would be None.
     """
-    if not chunk_id or chunk_id[0] != 'c':
+    if not chunk_id or chunk_id[0] != "c":
         raise ValueError("unexpected chunk id")
-    n = chunk_id.find('-')  # go to first underscore
+    n = chunk_id.find("-")  # go to first underscore
     if n == 1:
         return None  # no partition
     partition = int(chunk_id[1:n])
     return partition
 
 
 def getPartitionKey(chunk_id, partition_count):
-    """ mixin the the partition specifier based on dataset shape and
-        partition_count
+    """mixin the the partition specifier based on dataset shape and
+    partition_count
     """
     if not partition_count or partition_count < 2:
         return chunk_id  # no partition key needed
 
     chunk_index = getChunkIndex(chunk_id)
     rank = len(chunk_index)
 
@@ -428,131 +429,127 @@
     for dim in range(rank):
         prime_factor = PRIMES[dim % len(PRIMES)]
         partition_index += chunk_index[dim] * prime_factor
 
     partition_index %= partition_count
     n = chunk_id.find("-")  # get the part after the first hyphen
     s = chunk_id[n:]
-    chunk_id = 'c' + str(partition_index) + s
+    chunk_id = "c" + str(partition_index) + s
     return chunk_id
 
 
 def getChunkIdForPartition(chunk_id, dset_json):
-    """ Return the partition specific chunk id for given chunk
-    """
+    """Return the partition specific chunk id for given chunk"""
     if "layout" not in dset_json:
         msg = "No layout found in dset_json"
         log.error(msg)
         raise KeyError(msg)
     layout_json = dset_json["layout"]
     if "partition_count" in layout_json:
         partition_count = layout_json["partition_count"]
         partition = getChunkPartition(chunk_id)
         if partition is None:
             # mix in the partition key
             chunk_id = getPartitionKey(chunk_id, partition_count)
     return chunk_id
 
 
-def getChunkIds(dset_id, selection, layout, dim=0,
-                prefix=None, chunk_ids=None):
-    """ Get the all the chunk ids for chunks that lie in the
+def getChunkIds(dset_id, selection, layout, dim=0, prefix=None, chunk_ids=None):
+    """Get the all the chunk ids for chunks that lie in the
     selection of the
     given dataset.
     """
     num_chunks = getNumChunks(selection, layout)
     if num_chunks == 0:
         return []  # empty list
     if prefix is None:
         # construct a prefix using "c-" with the uuid of the dset_id
         if not dset_id.startswith("d-"):
             msg = f"Bad Request: invalid dset id: {dset_id}"
             log.warning(msg)
             raise ValueError(msg)
-        prefix = "c-" + dset_id[2:] + '_'
+        prefix = "c-" + dset_id[2:] + "_"
     rank = len(selection)
     if chunk_ids is None:
         chunk_ids = []
-    #log.debug(f"getChunkIds - selection: {selection}")
+    # log.debug(f"getChunkIds - selection: {selection}")
     s = selection[dim]
     c = layout[dim]
-    #log.debug(f"getChunkIds - layout: {layout}")
+    # log.debug(f"getChunkIds - layout: {layout}")
 
     if isinstance(s, slice) and s.step > c:
         # chunks may not be contiguous,  skip along the selection and add
         # whatever chunks we land in
         for i in range(s.start, s.stop, s.step):
             chunk_index = i // c
             chunk_id = prefix + str(chunk_index)
             if dim + 1 == rank:
                 # we've gone through all the dimensions, add this id
                 # to the list
                 chunk_ids.append(chunk_id)
             else:
-                chunk_id += '_'  # seperator between dimensions
+                chunk_id += "_"  # seperator between dimensions
                 # recursive call
-                getChunkIds(dset_id, selection, layout, dim+1,
-                            chunk_id, chunk_ids)
+                getChunkIds(dset_id, selection, layout, dim + 1, chunk_id, chunk_ids)
     elif isinstance(s, slice):
         # get a contiguous set of chunks along the selection
         if s.step > 1:
-            num_points = frac((s.stop-s.start), s.step)
+            num_points = frac((s.stop - s.start), s.step)
             w = num_points * s.step - (s.step - 1)
         else:
             w = s.stop - s.start  # selection width (>0)
 
         chunk_index_start = s.start // c
         chunk_index_end = frac((s.start + w), c)
 
         for i in range(chunk_index_start, chunk_index_end):
             chunk_id = prefix + str(i)
             if dim + 1 == rank:
                 # we've gone through all the dimensions,
                 # add this id to the list
                 chunk_ids.append(chunk_id)
             else:
-                chunk_id += '_'  # seperator between dimensions
+                chunk_id += "_"  # seperator between dimensions
                 # recursive call
-                getChunkIds(dset_id, selection, layout, dim+1,
-                            chunk_id, chunk_ids)
+                getChunkIds(dset_id, selection, layout, dim + 1, chunk_id, chunk_ids)
     else:
         # coordinate list
         last_chunk_index = None
         for coord in s:
             chunk_index = coord // c
             if chunk_index != last_chunk_index:
                 chunk_id = prefix + str(chunk_index)
                 if dim + 1 == rank:
                     # add the chunk id
                     chunk_ids.append(chunk_id)
                 else:
-                    chunk_id += '_' # dimension seperator
-                    getChunkIds(dset_id, selection, layout, dim+1,
-                                 chunk_id, chunk_ids)
+                    chunk_id += "_"  # dimension seperator
+                    getChunkIds(
+                        dset_id, selection, layout, dim + 1, chunk_id, chunk_ids
+                    )
                 last_chunk_index = chunk_index
 
-
     # got the complete list, return it!
     return chunk_ids
 
 
 def getChunkSuffix(chunk_id):
-    """ given a chunk_id (e.g.: c-12345678-1234-1234-1234-1234567890ab_6_4)
+    """given a chunk_id (e.g.: c-12345678-1234-1234-1234-1234567890ab_6_4)
     return the coordinates as a string. In this case 6_4
     """
     # go to the first underscore
-    n = chunk_id.find('_') + 1
+    n = chunk_id.find("_") + 1
     if n == 0:
-        raise ValueError("Invalid chunk_id: {}".format(chunk_id))
+        raise ValueError(f"Invalid chunk_id: {chunk_id}")
     suffix = chunk_id[n:]
     return suffix
 
 
 def getChunkCoordinate(chunk_id, layout):
-    """ given a chunk_id (e.g.: c-12345678-1234-1234-1234-1234567890ab_6_4)
+    """given a chunk_id (e.g.: c-12345678-1234-1234-1234-1234567890ab_6_4)
     and a layout (e.g. (10,10))
     return the coordinates of the chunk in dataset space. In this case (60,40)
     """
     coord = getChunkIndex(chunk_id)
     for i in range(len(layout)):
         coord[i] *= layout[i]
 
@@ -560,15 +557,15 @@
 
 
 def getChunkSelection(chunk_id, slices, layout):
     """
     Return the intersection of the chunk with the given slices
     selection of the array.
     """
-    #print("getChunkSelection - chunk_id:", chunk_id, "slices:", slices)
+    # print("getChunkSelection - chunk_id:", chunk_id, "slices:", slices)
     chunk_index = getChunkIndex(chunk_id)
     rank = len(layout)
     sel = []
     for dim in range(rank):
         s = slices[dim]
         c = layout[dim]
         n = chunk_index[dim] * c
@@ -588,15 +585,15 @@
                 start = s.start
             step = s.step
             cs = slice(start, stop, step)
             stop = slice_stop(cs)
             sel.append(slice(start, stop, step))
         else:
             # coord list
-            coords = [] 
+            coords = []
             for j in s:
                 if j >= n and j < n + c:
                     coords.append(j)
             sel.append(coords)
 
     return sel
 
@@ -637,26 +634,25 @@
                 elif j - offset >= w:
                     msg = "Unexpected chunk selection"
                     log.error(msg)
                     raise ValueError(msg)
                 coord.append(j - offset)
             sel.append(tuple(coord))
 
-
     return sel
 
 
 def getDataCoverage(chunk_id, slices, layout):
     """
     Get data-relative selection of the given chunk and selection.
     """
     chunk_sel = getChunkSelection(chunk_id, slices, layout)
     rank = len(layout)
     sel = []
-    #print(f'getDataCoverage - chunk_id: {chunk_id} slices: {slices} layout: {layout}')
+    # print(f'getDataCoverage - chunk_id: {chunk_id} slices: {slices} layout: {layout}')
     for dim in range(rank):
         c = chunk_sel[dim]
         s = slices[dim]
         if isinstance(s, slice):
             if c.step != s.step:
                 msg = "expecting step for chunk selection to be the "
                 msg += "same as data selection"
@@ -677,15 +673,15 @@
             start = 0
             for i in range(len(s)):
                 if s[i] >= c[0]:
                     break
                 start += 1
             stop = start + len(c)
             step = 1
-            sel.append(slice(start,stop,step))
+            sel.append(slice(start, stop, step))
 
     return tuple(sel)
 
 
 def getChunkRelativePoint(chunkCoord, point):
     """
     Get chunk-relative coordinate of the given point
@@ -699,25 +695,48 @@
         if chunkCoord[i] > point[i]:
             msg = "unexpected point index"
             raise IndexError(msg)
         tr[i] = point[i] - chunkCoord[i]
     return tr
 
 
+def get_chunktable_dims(shape_dims, chunk_dims):
+    """
+    Get the cannoncial size of the chunktable for a
+    given dataset and chunk shape"""
+    rank = len(shape_dims)
+    table_dims = []
+    for dim in range(rank):
+        dset_extent = shape_dims[dim]
+        chunk_extent = chunk_dims[dim]
+
+        if dset_extent > 0 and chunk_extent > 0:
+            # get integer ceil of dset and chunk extents
+            table_extent = -(dset_extent // -chunk_extent)
+        else:
+            table_extent = 0
+        table_dims.append(table_extent)
+    table_dims = tuple(table_dims)
+    return table_dims
+
+
 class ChunkIterator:
     """
     Class to iterate through list of chunks given dset_id, selection,
     and layout.
     """
+
     def __init__(self, dset_id, selection, layout):
         self._prefix = "c-" + dset_id[2:]
         self._layout = layout
         self._selection = selection
         self._rank = len(selection)
-        self._chunk_index = [0, ] * self._rank
+        self._chunk_index = [
+            0,
+        ] * self._rank
         for i in range(self._rank):
             s = selection[i]
             c = layout[i]
             self._chunk_index[i] = s.start // c
 
     def __iter__(self):
         return self
@@ -725,15 +744,15 @@
     def next(self):
         if self._chunk_index[0] * self._layout[0] >= self._selection[0].stop:
             # ran past the last chunk, end iteration
             raise StopIteration()
         chunk_id = self._prefix
         # init to minimum chunk index for each dimension
         for i in range(self._rank):
-            chunk_id += '_'
+            chunk_id += "_"
             chunk_id += str(self._chunk_index[i])
         # bump up the last index and carry forward if we run outside
         # the selection
         dim = self._rank - 1
         while dim >= 0:
             c = self._layout[dim]
             s = self._selection[dim]
@@ -781,56 +800,64 @@
     return output_arr
 
 
 def chunkWriteSelection(chunk_arr=None, slices=None, data=None):
     """
     Write data for requested chunk and selection
     """
-    log.info("chunkWriteSelection")
     dims = chunk_arr.shape
 
     rank = len(dims)
 
     if rank == 0:
         msg = "No dimension passed to chunkReadSelection"
+        log.error(msg)
         raise ValueError(msg)
     if len(slices) != rank:
         msg = "Selection rank does not match dataset rank"
+        log.error(msg)
         raise ValueError(msg)
     if len(data.shape) != rank:
         msg = "Input arr does not match dataset rank"
+        log.error(msg)
         raise ValueError(msg)
 
     updated = False
     # check if the new data modifies the array or not
-    if not np.array_equal(chunk_arr[slices], data):
-        # update chunk array
-        chunk_arr[slices] = data
-        updated = True
+    # TBD - is this worth the cost of comparing two arrays element by element?
+    try:
+        if not ndarray_compare(chunk_arr[slices], data):
+            # if not np.array_equal(chunk_arr[slices], data):
+            # update chunk array
+            chunk_arr[slices] = data
+            updated = True
+    except ValueError as ve:
+        msg = f"array_equal ValueError, chunk_arr[{slices}]: {chunk_arr[slices]} "
+        msg += f"data: {data}, data type: {type(data)} ve: {ve}"
+        log.error(msg)
+        raise
+
     return updated
 
 
-def chunkReadPoints(chunk_id=None, chunk_layout=None, chunk_arr=None,
-                    point_arr=None):
+def chunkReadPoints(chunk_id=None, chunk_layout=None, chunk_arr=None, point_arr=None):
     """
     Read points from given chunk
     """
     log.debug(f"chunkReadPoints - chunk_id: {chunk_id}")
 
     dims = chunk_arr.shape
-    log.debug(f"got dims: {dims}")
     chunk_coord = getChunkCoordinate(chunk_id, dims)
     log.debug(f"chunk_coord: {chunk_coord}")
     rank = len(dims)
     if rank == 0:
         msg = "No dimension passed to chunk read points"
         raise ValueError(msg)
 
     dset_dtype = chunk_arr.dtype
-    log.debug(f"dset dtype: {dset_dtype}")
 
     # verify chunk_layout
     if len(chunk_layout) != rank:
         msg = "chunk layout doesn't match rank"
         raise ValueError(msg)
 
     # verify points array dtype
@@ -858,16 +885,15 @@
         point = point_arr[i, :]
         tr_point = getChunkRelativePoint(chunk_coord, point)
         val = chunk_arr[tuple(tr_point)]
         output_arr[i] = val
     return output_arr
 
 
-def chunkWritePoints(chunk_id=None, chunk_layout=None, chunk_arr=None,
-                     point_arr=None):
+def chunkWritePoints(chunk_id=None, chunk_layout=None, chunk_arr=None, point_arr=None):
     """
     Write points to given chunk
     """
     # writing point data
     log.debug(f"chunkWritePoints - chunk_id: {chunk_id}")
     dims = chunk_arr.shape
 
@@ -925,42 +951,42 @@
             coord = elem[0]  # index to update
             for dim in range(rank):
                 # adjust to chunk relative
                 coord[dim] = int(coord[dim]) - chunk_coord[dim]
             coord = tuple(coord)  # need to convert to a tuple
         log.debug(f"relative coordinate: {coord}")
 
-        val = elem[1]   # value
+        val = elem[1]  # value
         chunk_arr[coord] = val  # update the point
 
 
 def _getEvalStr(query, arr_name, field_names):
     """
     _getEvalStr: Get eval string for given query
     Gets Eval string to use with numpy where method.
     """
     i = 0
     eval_str = ""
     var_name = None
     end_quote_char = None
     var_count = 0
     paren_count = 0
-    black_list = ("import", )  # field names that are not allowed
+    black_list = ("import",)  # field names that are not allowed
     for item in black_list:
         if item in field_names:
             msg = "invalid field name"
             log.warn("Bad query: " + msg)
             raise ValueError(msg)
     while i < len(query):
         ch = query[i]
-        if (i+1) < len(query):
-            ch_next = query[i+1]
+        if (i + 1) < len(query):
+            ch_next = query[i + 1]
         else:
             ch_next = None
-        if var_name and not ch.isalnum() and not ch == '_':
+        if var_name and not ch.isalnum() and not ch == "_":
             # end of variable
             if var_name not in field_names:
                 # invalid
                 msg = f"query variable: {var_name}"
                 log.debug(f"field_names: {field_names}")
                 log.warn("Bad query: " + msg)
                 raise ValueError(msg)
@@ -972,35 +998,35 @@
             if ch == end_quote_char:
                 # end of literal
                 end_quote_char = None
             eval_str += ch
         elif ch in ("'", '"'):
             end_quote_char = ch
             eval_str += ch
-        elif ch.isalpha() or ch == '_':
-            if ch == 'b' and ch_next in ("'", '"'):
-                eval_str += 'b'  # start of a byte string literal
+        elif ch.isalpha() or ch == "_":
+            if ch == "b" and ch_next in ("'", '"'):
+                eval_str += "b"  # start of a byte string literal
             elif var_name is None:
-                var_name = ch   # start of a variable
+                var_name = ch  # start of a variable
             else:
                 var_name += ch
-        elif ch == '(' and end_quote_char is None:
+        elif ch == "(" and end_quote_char is None:
             paren_count += 1
             eval_str += ch
-        elif ch == ')' and end_quote_char is None:
+        elif ch == ")" and end_quote_char is None:
             paren_count -= 1
             if paren_count < 0:
                 msg = "Mismatched paren"
                 log.warn("Bad query: " + msg)
                 raise ValueError(msg)
             eval_str += ch
         else:
             # just add to eval_str
             eval_str += ch
-        i = i+1
+        i = i + 1
     if end_quote_char:
         msg = "no matching quote character"
         log.warn("Bad Query: " + msg)
         raise ValueError(msg)
     if var_count == 0:
         msg = "No field value"
         log.warn("Bad query: " + msg)
@@ -1009,121 +1035,151 @@
         msg = "Mismatched paren"
         log.warn("Bad query: " + msg)
         raise ValueError(msg)
     log.debug(f"eval_str: {eval_str}")
     return eval_str
 
 
-def chunkQuery(chunk_id=None, chunk_layout=None, chunk_arr=None, slices=None,
-               query=None, query_update=None, limit=0, return_json=False):
+def getQueryDtype(dt):
+    """make a dtype for query response"""
+    field_names = dt.names
+    #  make up a index field name that doesn't conflict with existing names
+    index_name = "index"
+    for i in range(len(field_names)):
+        if index_name in field_names:
+            index_name = "_" + index_name
+        else:
+            break
+
+    dt_fields = [
+        (index_name, "uint64"),
+    ]
+    for i in range(len(dt)):
+        dt_fields.append((dt.names[i], dt[i]))
+    query_dt = np.dtype(dt_fields)
+
+    return query_dt
+
+
+def chunkQuery(
+    chunk_id=None,
+    chunk_layout=None,
+    chunk_arr=None,
+    slices=None,
+    query=None,
+    query_update=None,
+    limit=0,
+):
     """
     Run query on chunk and selection
     """
-    log.debug(f"chunkQuery - chunk_id: {chunk_id}")
+    log.debug(
+        f"chunkQuery - chunk_id: {chunk_id} query: {query} slices: {slices}, limit: {limit}"
+    )
 
     if not isinstance(chunk_arr, np.ndarray):
         raise TypeError("unexpected array type")
 
-    if limit and not isinstance(limit, int):
-        raise TypeError("unexpected limit")
-
     dims = chunk_arr.shape
 
     rank = len(dims)
 
-    dset_dtype = chunk_arr.dtype
-    log.debug(f"dtype: {dset_dtype}")
-    log.debug(f"selection: {slices}")
-    log.debug(f"query: {query}")
+    dset_dt = chunk_arr.dtype
 
     if rank != 1:
         msg = "Query operations only supported on one-dimensional datasets"
         log.error(msg)
         raise ValueError(msg)
+
     if not slices:
-        slices = [slice(0, dims[0], 1), ]
+        slices = [
+            slice(0, dims[0], 1),
+        ]
+    log.debug(f"chunkQuery slices: {slices}")
     if len(slices) != rank:
         msg = "Selection rank does not match shape rank"
         log.error(msg)
         raise ValueError(msg)
     slices = tuple(slices)
 
     chunk_coord = getChunkCoordinate(chunk_id, chunk_layout)
 
-    values = []
-    indices = []
     # do query selection
-    field_names = list(dset_dtype.fields.keys())
+    field_names = dset_dt.names
 
     if query_update:
-        replace_mask = [None, ] * len(field_names)
+        replace_mask = [
+            None,
+        ] * len(field_names)
         for i in range(len(field_names)):
             field_name = field_names[i]
             if field_name in query_update:
                 replace_mask[i] = query_update[field_name]
         log.debug(f"chunkQuery - replace_mask: {replace_mask}")
-        if replace_mask == [None, ] * len(field_names):
+        replace_fields = [
+            None,
+        ] * len(field_names)
+        if replace_mask == replace_fields:
             msg = "chunkQuery - no fields found in query_update"
             raise ValueError(msg)
     else:
         replace_mask = None
 
     x = chunk_arr[slices]
-    # log.debug(f"chunkQuery - x: {x}")
     eval_str = _getEvalStr(query, "x", field_names)
-    log.debug(f"chunkQuery - eval_str: {eval_str}, {x.shape[0]} rows ")
-    where_result = np.where(eval(eval_str))
-    log.debug(f"chunkQuery - where_result: {where_result}")
-    where_result_index = where_result[0]
-    log.debug(f"chunkQuery - where_result index: {where_result_index}")
-    log.debug(f"chunkQuery - boolean selection: {x[where_result_index]}")
-    s = slices[0]
-    count = 0
-    for index in where_result_index:
-        # log.debug(f"chunkQuery - index: {index}")
-        value = x[index].copy()
-        if replace_mask:
-            # log.debug(f"chunkQuery - original value: {value}")
-            for i in range(len(field_names)):
-                if replace_mask[i] is not None:
-                    value[i] = replace_mask[i]
-            # log.debug(f"chunkQuery - modified value: {value}")
-            try:
-                chunk_arr[index] = value
-            except ValueError as ve:
-                log.error(f"Numpy Value updating array: {ve}")
-                raise
-
-        # log.debug(f"chunkQuery - got value: {value}")
-        # adjust for selection
-        indices.append(int(index) * s.step + s.start + chunk_coord[0])
-        values.append(value)
-        count += 1
-        if limit > 0 and count >= limit:
-            log.debug("query update - got limit items")
-            break
+    where_indices = np.where(eval(eval_str))
+    if not isinstance(where_indices, tuple):
+        log.warn(f"expected where_indices of tuple but got: {type(where_indices)}")
+        return None
+    if len(where_indices) == 0:
+        log.warn("chunkQuery - got empty tuple where result")
+        return None
 
-    if return_json:
-        # return JSON list
-        result = {}
-        result["index"] = indices
-        result["value"] = _bytesArrayToList(values)
-        # log.debug(f"chunkQuery returning {result}")
+    where_indices = where_indices[0]
+    if not isinstance(where_indices, np.ndarray):
+        log.warn(f"expected where_indices of ndarray but got: {type(where_indices)}")
+        return None
+    nrows = where_indices.shape[0]
+    log.debug(f"chunkQuery - {nrows} found")
 
-    else:
-        # return the results as a numpy array
-        if rank == 1:
-            coord_type_str = "uint64"
-        else:
-            coord_type_str = f"({rank},)uint64"
-        result_dtype = np.dtype([
-            ("coord", np.dtype(coord_type_str)),
-            ("value", dset_dtype)])
-        result = np.zeros((count,), dtype=result_dtype)
-        for i in range(count):
-            e = result[i]
-            e[0] = indices[i]
-            e[1] = values[i]
-            result[i] = e
+    if limit > 0 and nrows > limit:
+        # truncate to limit rows
+        log.debug(f"limiting  response to {limit} rows")
+        where_indices = where_indices[:limit]
+        nrows = limit
+
+    where_result = x[where_indices].copy()
+
+    if replace_mask and nrows > 0:
+        log.debug(f"apply replace_mask: {replace_mask}")
+        for i in range(len(field_names)):
+            field = field_names[i]
+            if replace_mask[i] is not None:
+                where_result[field] = replace_mask[i]
+        # update source array
+        for i in range(nrows):
+            index = where_indices[i]
+            row = where_result[i]
+            chunk_arr[index] = row
+
+    # adjust the index to correspond with the dataset
+    s = slices[0]
+    start = s.start + chunk_coord[0]
+    if start > 0:
+        # can just increment every value by same amount
+        where_indices += start
+    if s.step and s.step > 1:
+        for i in range(nrows):
+            where_indices[i] = where_indices[i] + (s.step - 1) * i
+
+    dt_rsp = getQueryDtype(dset_dt)
+    # construct response array
+    rsp_arr = np.zeros((nrows,), dtype=dt_rsp)
+    for field in field_names:
+        rsp_arr[field] = where_result[field]
+    index_name = dt_rsp.names[0]
+    rsp_arr[index_name] = where_indices
+    log.debug(f"chunkQuery returning {len(rsp_arr)} rows")
+    for i in range(len(rsp_arr)):
+        log.debug(f"   {i}: {rsp_arr[i]}")
 
-    log.debug(f"chunkQuery returning: {count} rows")
-    return result
+    return rsp_arr
```

### Comparing `hsds-0.7.0b11/hsds/util/domainUtil.py` & `hsds-0.8.0/hsds/util/domainUtil.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 
 import os.path as op
 from aiohttp.web_exceptions import HTTPBadRequest
+
 #
 # Domain utilities
 #
 
 DOMAIN_SUFFIX = "/.domain.json"  # key suffix used to hold domain info
 
 
 def isIPAddress(s):
     """Return True if the string looks like an IP address:
-        n.n.n.n where n is between 0 and 255 """
+    n.n.n.n where n is between 0 and 255"""
     if not s:
         return False
     # see if there is a port specifier
-    if s.find(':') > 0:
+    if s.find(":") > 0:
         return True
 
-    if s == 'localhost':
+    if s == "localhost":
         return True  # special case for loopback dns_path
 
-    parts = s.split('.')
+    parts = s.split(".")
 
     if len(parts) != 4:
         return False
     for part in parts:
-        if part == ':':
+        if part == ":":
             # skip past a possible port specifier
             break
         try:
             n = int(part)
             if n < 0 or n > 255:
                 return False
         except ValueError:
@@ -55,15 +56,15 @@
     """
     if domain.endswith(DOMAIN_SUFFIX):
         n = len(DOMAIN_SUFFIX) - 1
         domain = domain[:-n]
 
     bucket = getBucketForDomain(domain)
     domain_path = getPathForDomain(domain)
-    if len(domain_path) > 1 and domain_path[-1] == '/':
+    if len(domain_path) > 1 and domain_path[-1] == "/":
         domain_path = domain_path[:-1]
     dirname = op.dirname(domain_path)
     if bucket:
         parent = bucket + dirname
     else:
         parent = dirname
 
@@ -73,32 +74,39 @@
 
 
 def validateHostDomain(id):
     if not isinstance(id, str):
         raise ValueError("Expected string type")
     if len(id) < 3:
         raise ValueError("Host Domain name is too short")
-    if len(id) == 38 and id[5] == '-' and id[7] == '-' and id[16] == '-' and \
-            id[21] == '-' and id[26] == '-':
+    if len(id) == 38 and all(
+        (
+            id[5] == "-",
+            id[7] == "-",
+            id[16] == "-",
+            id[21] == "-",
+            id[26] == "-",
+        )
+    ):
         raise ValueError("Host Domain name not allowed")
     if len(id) == 14 and id.endswith("-headnode"):
         raise ValueError("Host Domain name not allowed")
-    if id.startswith('.'):
+    if id.startswith("."):
         raise ValueError("Host Domain cannot start with dot")
-    if id.endswith('.'):
+    if id.endswith("."):
         raise ValueError("Host Domain cannot end with dot")
-    if id.startswith('-'):
+    if id.startswith("-"):
         raise ValueError("Host Domain cannot start with hyphen")
-    if id.endswith('-'):
+    if id.endswith("-"):
         raise ValueError("Host Domain cannot end with hyphen")
-    if id.find('..') > 0:
+    if id.find("..") > 0:
         raise ValueError("Host Domain cannot contain consecutive dots")
     if isIPAddress(id):
         raise ValueError("Host Domain looks like IP address")
-    if id.find('/') >= 0:
+    if id.find("/") >= 0:
         raise ValueError("Host Domain cannot contain slash")
     if id.find(".") == -1:
         raise ValueError("Host domain must have a dot")
 
 
 def isValidHostDomain(id):
     try:
@@ -109,17 +117,17 @@
 
 
 def validateDomain(id):
     if not isinstance(id, str):
         raise ValueError("Expected string type")
     if len(id) < 3:
         raise ValueError("Domain name too short")
-    if id.find('/') == -1:
+    if id.find("/") == -1:
         raise ValueError("Domain names should include a '/'")
-    if id[-1] == '/':
+    if id[-1] == "/":
         raise ValueError("Slash at end not allowed")
 
 
 def isValidDomain(id):
     try:
         validateDomain(id)
         return True
@@ -128,20 +136,20 @@
 
 
 def validateDomainPath(path):
     if not isinstance(path, str):
         raise ValueError("Expected string type")
     if len(path) < 1:
         raise ValueError("Domain path too short")
-    if path == '/':
+    if path == "/":
         return  # default buckete, root folder
-    if path[:-1].find('/') == -1:
+    if path[:-1].find("/") == -1:
         msg = "Domain path should have at least one '/' before trailing slash"
         raise ValueError(msg)
-    if path[-1] != '/':
+    if path[-1] != "/":
         raise ValueError("Domain path must end with '/'")
 
 
 def isValidDomainPath(path):
     try:
         validateDomainPath(path)
         return True
@@ -152,64 +160,64 @@
 def validateDomainKey(domain_key):
     if not domain_key.endswith(DOMAIN_SUFFIX):
         raise ValueError("Invalid domain key")
 
 
 def getDomainForHost(host_value):
     # Convert domain paths to S3 keys
-    npos = host_value.rfind(':')
+    npos = host_value.rfind(":")
     if npos > 0:
         host = host_value[:npos]
     else:
         host = host_value
 
     if len(host) < 3:
         # by equivalence to internet top-level domains, .org, .com, etc
-        raise ValueError('domain name is not valid')
+        raise ValueError("domain name is not valid")
 
-    if host[0] == '.' or host[-1] == '.':
+    if host[0] == "." or host[-1] == ".":
         # can't have a first or last dot'
-        raise ValueError('domain name is not valid')
+        raise ValueError("domain name is not valid")
 
-    dns_path = host.split('.')
+    dns_path = host.split(".")
     dns_path.reverse()  # flip to filesystem ordering
-    domain = '/'
+    domain = "/"
     for field in dns_path:
         if len(field) == 0:
             # consecutive dots are not allowed
-            raise ValueError('domain name is not valid')
+            raise ValueError("domain name is not valid")
         domain += field
-        domain += '/'
+        domain += "/"
 
     domain = domain[:-1]  # remove trailing slash
 
     return domain
 
 
-def getDomainFromRequest(request, validate=True):
+def getDomainFromRequest(request, validate=True, allow_dns=True):
     # print("gotDomainFromRequest:", request, "validate=", validate)
     app = request.app
     domain = None
     bucket = None
     params = request.rel_url.query
     if "domain" in params:
         domain = params["domain"]
     else:
-        if 'host' in params:
-            domain = params['host']
+        if "host" in params and allow_dns:
+            domain = params["host"]
         elif "X-Hdf-domain" in request.headers:
-            domain = request.headers['X-Hdf-domain']
-        elif "X-Forwarded-Host" in request.headers:
+            domain = request.headers["X-Hdf-domain"]
+        elif "X-Forwarded-Host" in request.headers and allow_dns:
             domain = request.headers["X-Forwarded-Host"]
-        else:
+        elif allow_dns:
             domain = request.host
     if not domain:
         raise ValueError("no domain")
 
-    if domain[0] != '/':
+    if domain[0] != "/":
         # DNS style hostname
         if validate:
             validateHostDomain(domain)  # throw ValueError if invalid
             domain = getDomainForHost(domain)  # convert to s3 path
         else:
             try:
                 validateHostDomain(domain)
@@ -226,52 +234,52 @@
     elif "bucket_name" in request.app and request.app["bucket_name"]:
         # prefix the domain with the bucket name
         bucket = app["bucket_name"]
     else:
         pass  # no bucket specified
 
     if bucket and validate:
-        if bucket.find('/') >= 0:
+        if bucket.find("/") >= 0:
             raise ValueError(f"bucket name: {bucket} is not valid")
-        if domain[0] == '/':
+        if domain[0] == "/":
             domain = bucket + domain
 
     return domain
 
 
 def getPathForDomain(domain):
     """
     Return the non-bucket part of the domain
     """
     if not domain:
         return None
-    index = domain.find('/')
+    index = domain.find("/")
     if index < 1:
         return domain  # no bucket
     return domain[(index):]
 
 
 def getBucketForDomain(domain):
-    """ get the bucket for the domain or None
-        if no bucket is given
+    """get the bucket for the domain or None
+    if no bucket is given
     """
     if not domain:
         return None
-    if domain[0] == '/':
+    if domain[0] == "/":
         # no bucket specified
         return None
-    index = domain.find('/')
+    index = domain.find("/")
     if index < 0:
         # invalid domain?
         return None
     return domain[:index]
 
 
 def verifyRoot(domain_json):
-    """ Throw bad request if we are expecting a domain,
-      but got a folder instead
+    """Throw bad request if we are expecting a domain,
+    but got a folder instead
     """
     if "root" not in domain_json:
         msg = "Expected root key for domain"
         # can't use hsds logger, since it would create a circular dependency
         print("WARN> " + msg)
         raise HTTPBadRequest(reason=msg)
```

### Comparing `hsds-0.7.0b11/hsds/util/dsetUtil.py` & `hsds-0.8.0/hsds/util/dsetUtil.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # terms governing use, modification, and redistribution, is contained in     #
 # the file COPYING, which can be found at the root of the source code        #
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 
 from aiohttp.web_exceptions import HTTPBadRequest, HTTPInternalServerError
+import math
 
 from .. import hsds_logger as log
 
 """
 Filters that are known to HSDS.
 Format is:
   FILTER_CODE, FILTER_ID, Name
@@ -23,57 +24,57 @@
   and H5Z_FILTER_SCALEOFFSET, are not currently supported.
 
   Non-supported filters metadata will be stored, but are
   not (currently) used for compression/decompression.
 """
 
 FILTER_DEFS = (
-    ('H5Z_FILTER_NONE', 0, "none"),
-    ('H5Z_FILTER_DEFLATE', 1, "gzip"),  # aka as "zlib" for blosc
-    ('H5Z_FILTER_SHUFFLE', 2, "shuffle"),
-    ('H5Z_FILTER_FLETCHER32', 3, "fletcher32"),
-    ('H5Z_FILTER_SZIP', 4, "szip"),
-    ('H5Z_FILTER_NBIT', 5, "nbit"),
-    ('H5Z_FILTER_SCALEOFFSET', 6, "scaleoffet"),
-    ('H5Z_FILTER_LZF', 32000, "lzf"),
-    ('H5Z_FILTER_BLOSC', 32001, "blosclz"),
-    ('H5Z_FILTER_SNAPPY', 32003, "snappy"),
-    ('H5Z_FILTER_LZ4', 32004, "lz4"),
-    ('H5Z_FILTER_LZ4HC', 32005, "lz4hc"),
-    ('H5Z_FILTER_ZSTD', 32015, "zstd")
+    ("H5Z_FILTER_NONE", 0, "none"),
+    ("H5Z_FILTER_DEFLATE", 1, "gzip"),  # aka as "zlib" for blosc
+    ("H5Z_FILTER_SHUFFLE", 2, "shuffle"),
+    ("H5Z_FILTER_FLETCHER32", 3, "fletcher32"),
+    ("H5Z_FILTER_SZIP", 4, "szip"),
+    ("H5Z_FILTER_NBIT", 5, "nbit"),
+    ("H5Z_FILTER_SCALEOFFSET", 6, "scaleoffet"),
+    ("H5Z_FILTER_LZF", 32000, "lzf"),
+    ("H5Z_FILTER_BLOSC", 32001, "blosclz"),
+    ("H5Z_FILTER_SNAPPY", 32003, "snappy"),
+    ("H5Z_FILTER_LZ4", 32004, "lz4"),
+    ("H5Z_FILTER_LZ4HC", 32005, "lz4hc"),
+    ("H5Z_FILTER_ZSTD", 32015, "zstd"),
 )
 
 COMPRESSION_FILTER_IDS = (
-    'H5Z_FILTER_DEFLATE',
-    'H5Z_FILTER_SZIP',
-    'H5Z_FILTER_SCALEOFFSET',
-    'H5Z_FILTER_LZF',
-    'H5Z_FILTER_BLOSC',
-    'H5Z_FILTER_SNAPPY',
-    'H5Z_FILTER_LZ4',
-    'H5Z_FILTER_LZ4HC',
-    'H5Z_FILTER_ZSTD'
+    "H5Z_FILTER_DEFLATE",
+    "H5Z_FILTER_SZIP",
+    "H5Z_FILTER_SCALEOFFSET",
+    "H5Z_FILTER_LZF",
+    "H5Z_FILTER_BLOSC",
+    "H5Z_FILTER_SNAPPY",
+    "H5Z_FILTER_LZ4",
+    "H5Z_FILTER_LZ4HC",
+    "H5Z_FILTER_ZSTD",
 )
 
 COMPRESSION_FILTER_NAMES = (
-    'gzip',
-    'szip',
-    'lzf',
-    'blosclz',
-    'snappy',
-    'lz4',
-    'lz4hc',
-    'zstd'
+    "gzip",
+    "szip",
+    "lzf",
+    "blosclz",
+    "snappy",
+    "lz4",
+    "lz4hc",
+    "zstd",
 )
 
 CHUNK_LAYOUT_CLASSES = (
-    'H5D_CHUNKED',
-    'H5D_CHUNKED_REF',
-    'H5D_CHUNKED_REF_INDIRECT',
-    'H5D_CONTIGUOUS_REF'
+    "H5D_CHUNKED",
+    "H5D_CHUNKED_REF",
+    "H5D_CHUNKED_REF_INDIRECT",
+    "H5D_CONTIGUOUS_REF",
 )
 
 
 def getFilterItem(key):
     """
     Return filter code, id, and name, based on an id, a name or a code.
     """
@@ -83,102 +84,131 @@
         for i in range(3):
             if key == item[i]:
                 return {"class": item[0], "id": item[1], "name": item[2]}
     return None  # not found
 
 
 def getFilters(dset_json):
-    """ Return list of filters, or empty list """
+    """Return list of filters, or empty list"""
     if "creationProperties" not in dset_json:
         return []
     creationProperties = dset_json["creationProperties"]
     if "filters" not in creationProperties:
         return []
     filters = creationProperties["filters"]
     return filters
 
 
 def getCompressionFilter(dset_json):
-    """ Return compression filter from filters, or None """
+    """Return compression filter from filters, or None"""
     filters = getFilters(dset_json)
     for filter in filters:
-        if 'class' not in filter:
+        if "class" not in filter:
             msg = f"filter option: {filter} with no class key"
             log.warn(msg)
             continue
         filter_class = filter["class"]
         if filter_class in COMPRESSION_FILTER_IDS:
             return filter
-        if filter_class == 'H5Z_FILTER_USER' and 'name' in filter and \
-                filter['name'] in COMPRESSION_FILTER_NAMES:
+        if all(
+            (
+                filter_class == "H5Z_FILTER_USER",
+                "name" in filter,
+                filter["name"] in COMPRESSION_FILTER_NAMES,
+            )
+        ):
             return filter
     return None
 
 
 def getShuffleFilter(dset_json):
-    """ Return shuffle filter, or None """
+    """Return shuffle filter, or None"""
     filters = getFilters(dset_json)
     for filter in filters:
         try:
             if filter["class"] == "H5Z_FILTER_SHUFFLE":
                 log.debug(f"Shuffle filter is used: {filter}")
                 return filter
         except KeyError:
             log.warn(f"filter option: {filter} with no class key")
             continue
     log.debug("Shuffle filter not used")
     return None
 
 
 def getFilterOps(app, dset_json, item_size):
-    """ Get list of filter operations to be used for this dataset """
-    filter_map = app['filter_map']
-    dset_id = dset_json['id']
+    """Get list of filter operations to be used for this dataset"""
+    filter_map = app["filter_map"]
+    dset_id = dset_json["id"]
     if dset_id in filter_map:
         log.debug(f"returning filter from filter_map {filter_map[dset_id]}")
         return filter_map[dset_id]
 
     compressionFilter = getCompressionFilter(dset_json)
     log.debug(f"got compressionFilter: {compressionFilter}")
 
     filter_ops = {}
 
     shuffleFilter = getShuffleFilter(dset_json)
     if shuffleFilter:
         filter_ops["use_shuffle"] = True
 
     if compressionFilter:
-        if compressionFilter["class"] == 'H5Z_FILTER_DEFLATE':
-            filter_ops["compressor"] = 'zlib'  # blosc compressor
+        if compressionFilter["class"] == "H5Z_FILTER_DEFLATE":
+            filter_ops["compressor"] = "zlib"  # blosc compressor
             if shuffleFilter:
                 filter_ops["use_shuffle"] = True
             else:
                 # for HDF5-style compression, use shuffle only if it turned on
-                filter_ops['use_shuffle'] = False
+                filter_ops["use_shuffle"] = False
         else:
             if "name" in compressionFilter:
                 filter_ops["compressor"] = compressionFilter["name"]
             else:
-                filter_ops["compressor"] = 'lz4'  # default to lz4
+                filter_ops["compressor"] = "lz4"  # default to lz4
         if "level" not in compressionFilter:
-            filter_ops['level'] = 5  # medium level
+            filter_ops["level"] = 5  # medium level
         else:
-            filter_ops['level'] = int(compressionFilter["level"])
+            filter_ops["level"] = int(compressionFilter["level"])
 
     if filter_ops:
-        filter_ops['item_size'] = item_size
-        if item_size == 'H5T_VARIABLE':
-            filter_ops['use_shuffle'] = False
+        filter_ops["item_size"] = item_size
+        if item_size == "H5T_VARIABLE":
+            filter_ops["use_shuffle"] = False
         log.debug(f"save filter ops: {filter_ops} for {dset_id}")
         filter_map[dset_id] = filter_ops  # save
         return filter_ops
     else:
         return None
 
 
+def getDsetRank(dset_json):
+    """Get rank returning 0 for sclar or NULL datashapes"""
+    datashape = dset_json["shape"]
+    if datashape["class"] == "H5S_NULL":
+        return 0
+    if datashape["class"] == "H5S_SCALAR":
+        return 0
+    if "dims" not in datashape:
+        log.warn(f"expected to find dims key in shape_json: {datashape}")
+        return 0
+    dims = datashape["dims"]
+    rank = len(dims)
+    return rank
+
+
+def isNullSpace(dset_json):
+    """Return true if this dataset is a null dataspace"""
+    datashape = dset_json["shape"]
+    if datashape["class"] == "H5S_NULL":
+        return True
+    else:
+        return False
+
+
 def getHyperslabSelection(dsetshape, start=None, stop=None, step=None):
     """
     Get slices given lists of start, stop, step values
 
     TBD: for step>1, adjust the slice to not extend beyond last
         data point returned
     """
@@ -245,32 +275,36 @@
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         slices.append(s)
     return tuple(slices)
 
 
 def getSelectionShape(selection):
-    """ Return the shape of the given selection.
-      Examples (selection -> returned shape):
-      [(3,7,1)] -> [4]
-      [(3, 7, 3)] -> [1]
-      [(44, 52, 1), (48,52,1)] -> [8, 4]
-      [[1,2,7]] ->
+    """Return the shape of the given selection.
+    Examples (selection -> returned shape):
+    [(3,7,1)] -> [4]
+    [(3, 7, 3)] -> [1]
+    [(44, 52, 1), (48,52,1)] -> [8, 4]
+    [[1,2,7]] ->
     """
     shape = []
     rank = len(selection)
     for i in range(rank):
         s = selection[i]
-        if isinstance(s,slice):
+        if isinstance(s, slice):
             extent = 0
+            if s.step and s.step > 1:
+                step = s.step
+            else:
+                step = 1
             if s.stop > s.start:
                 extent = s.stop - s.start
-            if s.step > 1 and extent > 0:
-                extent = (extent // s.step)
-            if (s.stop - s.start) % s.step != 0:
+            if step > 1 and extent > 0:
+                extent = extent // step
+            if (s.stop - s.start) % step != 0:
                 extent += 1
         else:
             # coordinate list
             extent = len(s)
         shape.append(extent)
     return shape
 
@@ -303,205 +337,348 @@
                 val = params[query_name]
 
     if val and default is not None and isinstance(default, int):
         # convert to int Type
         try:
             val = int(val)
         except ValueError:
-            msg = "Invalid request parameter: {}".format(query_name)
+            msg = f"Invalid request parameter: {query_name}"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
     if val is None:
         if default is not None:
             val = default
         else:
-            msg = "Request parameter is missing: {}".format(query_name)
+            msg = f"Request parameter is missing: {query_name}"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
     return val
 
+
 def _getSelectionStringFromRequestBody(body):
-    """ Join start, stop, and (optionally) stop keys 
-         to create an equivalent selection string """
+    """Join start, stop, and (optionally) stop keys
+    to create an equivalent selection string"""
     if "start" not in body:
         raise KeyError("no start key")
     start_val = body["start"]
     if not isinstance(start_val, (list, tuple)):
-        start_val =  [start_val,]
+        start_val = [
+            start_val,
+        ]
     rank = len(start_val)
     if "stop" not in body:
         raise KeyError("no stop key")
     stop_val = body["stop"]
     if not isinstance(stop_val, (list, tuple)):
-        stop_val = [stop_val,]
+        stop_val = [
+            stop_val,
+        ]
     if len(stop_val) != rank:
         raise ValueError("start and stop values have different ranks")
     if "step" in body:
         step_val = body["step"]
         if not isinstance(step_val, (list, tuple)):
-            step_val = [step_val,]
+            step_val = [
+                step_val,
+            ]
         if len(step_val) != rank:
-            raise ValueError("step values have differnt rank from start and stop selections")
+            raise ValueError(
+                "step values have differnt rank from start and stop selections"
+            )
     else:
         step_val = None
     selection = []
-    selection.append('[')
+    selection.append("[")
     for i in range(rank):
         dim_sel = f"{start_val[i]}:{stop_val[i]}"
         if step_val:
             dim_sel += f":{step_val[i]}"
         selection.append(dim_sel)
-        if i+1 < rank:
-            selection.append(',')
-    selection.append(']')
+        if i + 1 < rank:
+            selection.append(",")
+    selection.append("]")
     return "".join(selection)
 
+
 def _getSelectElements(select):
-    """ helper method - return array of queries for each 
-       dimension """
-    select = select[1:-1] # strip brackets
+    """helper method - return array of queries for each
+    dimension"""
+    if isinstance(select, list) or isinstance(select, tuple):
+        return select  # already listified
+    select = select[1:-1]  # strip brackets
     query_array = []
     dim_query = []
     coord_list = False
     for ch in select:
         if ch.isspace():
             # ignore
             pass
-        elif ch == ',':
+        elif ch == ",":
             if coord_list:
                 dim_query.append(ch)
             else:
                 if len(dim_query) == 0:
                     # empty dimension
                     raise ValueError("invalid query")
                 query_array.append("".join(dim_query))
-                dim_query = [] # reset
-        elif ch == '[':
+                dim_query = []  # reset
+        elif ch == "[":
             if coord_list:
                 # can't have nested coordinates
                 raise ValueError("invalid query")
             coord_list = True
             dim_query.append(ch)
-        elif ch == ']':
+        elif ch == "]":
             if not coord_list:
                 # close bracket with no open
                 raise ValueError("invalid query")
             dim_query.append(ch)
             coord_list = False
-        elif ch == ':':
+        elif ch == ":":
             if coord_list:
                 # range not allowed in coord list
                 raise ValueError("invalid query")
             dim_query.append(ch)
         else:
             dim_query.append(ch)
     if not dim_query:
-        #empty dimension
+        # empty dimension
         raise ValueError("invalid query")
     query_array.append("".join(dim_query))
-    
+
     return query_array
 
 
 def getSelectionList(select, dims):
-    """ Return tuple of slices and/or coordinate list for the given selection """
+    """Return tuple of slices and/or coordinate list for the given selection"""
     select_list = []
 
+    if isinstance(select, dict):
+        select = _getSelectionStringFromRequestBody(select)
+
     if select is None or len(select) == 0:
-        """ Return set of slices covering data space"""
+        """Return set of slices covering data space"""
         slices = []
         for extent in dims:
             s = slice(0, extent, 1)
             slices.append(s)
         return tuple(slices)
 
-    if isinstance(select, dict):
-        select = _getSelectionStringFromRequestBody(select)
-        
     # convert selection to list by dimension
     elements = _getSelectElements(select)
     rank = len(elements)
     if len(dims) != rank:
         raise ValueError("invalid rank for selection")
     for dim in range(rank):
         extent = dims[dim]
         element = elements[dim]
-        if element.startswith('['):
+        is_list = isinstance(element, list)
+        is_str = isinstance(element, str)
+        if is_list or (is_str and element.startswith("[")):
             # list of coordinates
-            fields = element[1:-1].split(',')
+            if is_str:
+                fields = element[1:-1].split(",")
+            else:
+                fields = element
             coords = []
             last_coord = None
             for field in fields:
                 try:
                     coord = int(field)
                 except ValueError:
                     raise ValueError(f"Invalid coordinate for dim {dim}")
                 if coord < 0 or coord >= extent:
-                    raise ValueError(f"out of range coordinate for dim {dim}, {coord} not in range: 0-{extent-1} ")
-                if last_coord != None and coord <= last_coord:
+                    msg = f"out of range coordinate for dim {dim}, {coord} "
+                    msg += f"not in range: 0-{extent-1}"
+                    raise ValueError(msg)
+                if last_coord is not None and coord <= last_coord:
                     raise ValueError("coordinates must be increasing")
                 last_coord = coord
                 coords.append(coord)
             select_list.append(coords)
         elif element == ":":
             s = slice(0, extent, 1)
             select_list.append(s)
-        elif element.find(':') >= 0:
-            fields = element.split(':')
-            if len(fields) not in (2,3):
+        elif is_str and element.find(":") >= 0:
+            fields = element.split(":")
+            if len(fields) not in (2, 3):
                 raise ValueError(f"Invalid selection format for dim {dim}")
             if len(fields[0]) == 0:
                 start = 0
             else:
                 try:
                     start = int(fields[0])
                 except ValueError:
                     raise ValueError(f"Invalid selection - start value for dim {dim}")
                 if start < 0 or start >= extent:
-                    raise ValueError(f"Invalid selection - start value out of range for dim {dim}")
+                    raise ValueError(
+                        f"Invalid selection - start value out of range for dim {dim}"
+                    )
             if len(fields[1]) == 0:
                 stop = extent
             else:
                 try:
                     stop = int(fields[1])
                 except ValueError:
                     raise ValueError(f"Invalid selection - stop value for dim {dim}")
                 if stop < 0 or stop > extent or stop <= start:
-                    raise ValueError(f"Invalid selection - stop value out of range for dim {dim}")
+                    raise ValueError(
+                        f"Invalid selection - stop value out of range for dim {dim}"
+                    )
             if len(fields) == 3:
                 # get step value
                 if len(fields[2]) == 0:
                     step = 1
                 else:
                     try:
                         step = int(fields[2])
                     except ValueError:
-                        raise ValueError(f"Invalid selection - step value for dim {dim}")
+                        raise ValueError(
+                            f"Invalid selection - step value for dim {dim}"
+                        )
                     if step <= 0:
-                        raise ValueError(f"Invalid selection - step value out of range for dim {dim}")
+                        raise ValueError(
+                            f"Invalid selection - step value out of range for dim {dim}"
+                        )
             else:
                 step = 1
             s = slice(start, stop, step)
             select_list.append(s)
         else:
             # expect single coordinate value
             try:
                 index = int(element)
             except ValueError:
                 raise ValueError(f"Invalid selection - index value for dim {dim}")
             if index < 0 or index >= extent:
-                raise ValueError(f"Invalid selection - index value out of range for dim {dim}")
-            
-            s = slice(index, index+1, 1)
+                raise ValueError(
+                    f"Invalid selection - index value out of range for dim {dim}"
+                )
+
+            s = slice(index, index + 1, 1)
             select_list.append(s)
     # end dimension loop
-    return tuple(select_list) 
+    return tuple(select_list)
 
 
-def setSliceQueryParam(params, sel):
+def getSelectionPagination(select, dims, itemsize, max_request_size):
+    """
+    Paginate a select tupe into multiple selects where each
+        select requires less than max_request_size bytes"""
+    msg = f"getSelectionPagination - select: {select}, dims: {dims}, "
+    msg += f"itemsize: {itemsize}, max_request_size: {max_request_size}"
+    log.debug(msg)
+    select_shape = getSelectionShape(select)
+    log.debug(f"getSelectionPagination - select_shape: {select_shape}")
+    select_size = math.prod(select_shape) * itemsize
+    log.debug(f"getSelectionPagination - select_size: {select_size}")
+    if select_size <= max_request_size:
+        # No need to paginate, just return select as as a one item tuple
+        log.debug("getSelectionPagination - not needed")
+        return (select,)
+
+    # get pagination dimension - first dimension with > 1 extent
+    rank = len(dims)
+    paginate_dim = None
+    paginate_extent = None
+    for i in range(rank):
+        s = select[i]
+        if isinstance(s, slice):
+            paginate_extent = 0
+            if s.step and s.stop > 1:
+                step = s.step
+            else:
+                step = 1
+            if s.stop > s.start:
+                paginate_extent = s.stop - s.start
+        else:
+            # coordinate list
+            paginate_extent = len(s)
+        if paginate_extent > 1:
+            paginate_dim = i
+            break
+    if paginate_dim is None:
+        msg = "unable to determine pagination dimension"
+        log.warn(msg)
+        raise ValueError(msg)
+    log.debug(f"getSelectionPagination - using pagination dimension: {paginate_dim}")
+
+    # get the approx bytes per page by doing fractional dev with ceil
+    page_count = select_size // max_request_size
+    page_count += 1  # round up by one
+    log.debug(f"getSelectionPagination - page_count: {page_count}")
+    page_size = select_size // page_count
+    log.debug(f"getSelectionPagination - page_size: {page_size}")
+
+    s = select[paginate_dim]
+    # log.debug(f"pagination dim: {paginate_dim} select: {s} paginate_extent: {paginate_extent}")
+    # page_extent = -(-max_request_size // page_size)
+    # log.debug(f"getSelectionPagination - page_extent: {page_extent}")
+    # page_count = -(-paginate_extent // page_extent)
+    if paginate_extent < page_count:
+        msg = f"select pagination unable to paginate select dim: {paginate_dim} "
+        msg += f"into {page_count} pages"
+        log.warn(msg)
+        raise ValueError(msg)
+    page_extent = paginate_extent // page_count
+    if page_extent < 1:
+        page_extent = 1
+    log.debug(f"getSelectionPagination - page_extent: {page_extent}")
+    paginate_slices = []
+    if isinstance(s, slice):
+        start = s.start
+        if s.step and s.stop > 1:
+            step = s.step
+        else:
+            step = 1
+
+        while start < s.stop:
+            stop = start + page_extent
+            if stop % step != 0:
+                # adjust to fall on step boundry
+                log.debug(f"pre-step adjust stop: {stop}")
+                stop += step - (stop % step)
+                log.debug(f"post-step adjust stop: {stop}")
+            if stop > s.stop:
+                stop = s.stop
+            paginate_slices.append(slice(start, stop, step))
+            start = stop
+    else:
+        # coordinate list
+        start = 0  # first index
+        while start < len(s):
+            stop = start + page_extent
+            if stop > len(s):
+                stop = len(s)
+            log.debug(f"page_coord s[{start}:{stop}]")
+            page_coord = s[start:stop]
+            log.debug(f"page coords: {page_coord}")
+            paginate_slices.append(tuple(page_coord))
+            start = stop
+    # adjust page count to number to actual pagination
+    page_count = len(paginate_slices)
+
+    log.debug(f"got {page_count} paginate_slices")
+    # return paginated selection list using paginate_slices for pagination
+    # dimension, original selection for each other dimension
+    pagination = []
+    for page in range(page_count):
+        s = []
+        for i in range(rank):
+            if i == paginate_dim:
+                s.append(paginate_slices[page])
+            else:
+                s.append(select[i])
+        pagination.append(tuple(s))
+    pagination = tuple(pagination)
+    # log.debug(f"returning pagination: {pagination}")
+    return pagination
+
+
+def getSliceQueryParam(sel):
     """
     Helper method - set query parameter for given shape + selection
 
     Query arg should be in the form: [<dim1>, <dim2>, ... , <dimn>]
         brackets are optional for one dimensional arrays.
          Each dimension, valid formats are:
             single integer: n
@@ -512,33 +689,35 @@
     rank = len(sel)
     if rank > 0:
         sel_param = "["
         for i in range(rank):
             s = sel[i]
             if isinstance(s, slice):
                 sel_param += str(s.start)
-                sel_param += ':'
+                sel_param += ":"
                 sel_param += str(s.stop)
                 if s.step > 1:
-                    sel_param += ':'
+                    sel_param += ":"
                     sel_param += str(s.step)
             else:
                 # coord selection
-                sel_param += '['
+                sel_param += "["
                 count = len(s)
                 for j in range(count):
                     sel_param += str(s[j])
                     if j < count - 1:
-                        sel_param += ','
-                sel_param += ']'
+                        sel_param += ","
+                sel_param += "]"
             if i < rank - 1:
-                sel_param += ','
-        sel_param += ']'
-        log.debug(f"select query param: {sel_param}")
-        params["select"] = sel_param
+                sel_param += ","
+        sel_param += "]"
+        # log.debug(f"select query param: {sel_param}")
+        if len(sel_param) > 500:
+            log.warning(f"select param is {len(sel_param)} characters long")
+        return sel_param
 
 
 def setChunkDimQueryParam(params, dims):
     """
     Helper method - set chunk dim param
     Send the chunk dimensions as a query param
     Query arg should be in the form: [<dim1>, <dim2>, ... , <dimn>]
@@ -551,15 +730,15 @@
     # pass dimensions, and selection as query params
     rank = len(dims)
     if rank > 0:
         dim_param = "["
         for i in range(rank):
             extent = dims[i]
             dim_param += str(extent)
-        dim_param += ']'
+        dim_param += "]"
         log.debug("dim query param: {}".format(dim_param))
         params["dim"] = dim_param
 
 
 def getDsetMaxDims(dset_json):
     """
     Get maxdims from a given shape.  Return [1,] for Scalar datasets
@@ -567,74 +746,94 @@
     Use with H5S_NULL datasets will throw a 400 error.
     """
     if "shape" not in dset_json:
         log.error("No shape found in dset_json")
         raise HTTPInternalServerError()
     shape_json = dset_json["shape"]
     maxdims = None
-    if shape_json['class'] == 'H5S_NULL':
+    if shape_json["class"] == "H5S_NULL":
         msg = "Expected shape class other than H5S_NULL"
         log.warn(msg)
         raise HTTPBadRequest(reason=msg)
-    elif shape_json['class'] == 'H5S_SCALAR':
-        maxdims = [1, ]
-    elif shape_json['class'] == 'H5S_SIMPLE':
+    elif shape_json["class"] == "H5S_SCALAR":
+        maxdims = [
+            1,
+        ]
+    elif shape_json["class"] == "H5S_SIMPLE":
         if "maxdims" in shape_json:
             maxdims = shape_json["maxdims"]
     else:
-        log.error("Unexpected shape class: {}".format(shape_json['class']))
+        log.error("Unexpected shape class: {}".format(shape_json["class"]))
         raise HTTPInternalServerError()
     return maxdims
 
 
 def getChunkLayout(dset_json):
-    """ Get chunk layout.  Throw 500 if used with non-H5D_CHUNKED layout
-    """
+    """Get chunk layout.  Throw 500 if used with non-H5D_CHUNKED layout"""
     if "layout" not in dset_json:
         log.error("No layout found in dset_json")
         raise HTTPInternalServerError()
     layout_json = dset_json["layout"]
-    if layout_json["class"] not in CHUNK_LAYOUT_CLASSES:
-        log.error("Unexpected shape layout: {}".format(layout_json["class"]))
+    if "class" not in layout_json:
+        log.error(f"Expected class key for layout: {layout_json}")
+        raise HTTPInternalServerError()
+    layout_class = layout_json["class"]
+    if layout_class not in CHUNK_LAYOUT_CLASSES:
+        log.error(f"Unexpected shape layout: {layout_class}")
+        raise HTTPInternalServerError()
+    if "dims" not in layout_json:
+        log.error(f"Expected dims key in layout: {layout_json}")
         raise HTTPInternalServerError()
     layout = layout_json["dims"]
     return layout
 
 
+def getChunkInitializer(dset_json):
+    """ get initializer application and arguments if set """
+    initializer = None
+    log.debug(f"getChunkInitializer({dset_json})")
+    if "creationProperties" in dset_json:
+        cprops = dset_json["creationProperties"]
+        log.debug(f"get creationProperties: {cprops}")
+        if "initializer" in cprops:
+            initializer = cprops["initializer"]
+    return initializer
+
+
 def getPreviewQuery(dims):
     """
     Helper method - return query options for a "reasonable" size
         data preview selection. Return None if the dataset is small
         enough that a preview is not needed.
     """
     select = "select=["
     rank = len(dims)
 
-    ncols = dims[rank-1]
+    ncols = dims[rank - 1]
     if rank > 1:
-        nrows = dims[rank-2]
+        nrows = dims[rank - 2]
     else:
         nrows = 1
 
     # use some rough heuristics to define the selection
     # aim to return no more than 100 elements
     if ncols > 100:
         ncols = 100
     if nrows > 100:
         nrows = 100
-    if nrows*ncols > 100:
+    if nrows * ncols > 100:
         if nrows > ncols:
             nrows = 100 // ncols
         else:
             ncols = 100 // nrows
 
     for i in range(rank):
-        if i == rank-1:
+        if i == rank - 1:
             select += "0:" + str(ncols)
-        elif i == rank-2:
+        elif i == rank - 2:
             select += "0:" + str(nrows) + ","
         else:
             select += "0:1,"
     select += "]"
     return select
 
 
@@ -654,49 +853,97 @@
 
 def isExtensible(dims, maxdims):
     """
     Determine if the dataset can be extended
     """
     if maxdims is None or len(dims) == 0:
         return False
-    log.debug("isExtensible - dims: {} maxdims: {}".format(dims, maxdims))
+    log.debug(f"isExtensible - dims: {dims} maxdims: {maxdims}")
     rank = len(dims)
     if len(maxdims) != rank:
         raise ValueError("rank of maxdims does not match dataset")
     for n in range(rank):
         # TBD - shouldn't have H5S_UNLIMITED in any new files.
         # Remove check once this is confirmed
-        if maxdims[n] in (0, 'H5S_UNLIMITED') or maxdims[n] > dims[n]:
+        if maxdims[n] in (0, "H5S_UNLIMITED") or maxdims[n] > dims[n]:
             return True
     return False
 
 
+def getDatasetCreationPropertyLayout(dset_json):
+    """ return layout json from creation property list """
+    cpl = None
+    if "creationProperties" in dset_json:
+        cp = dset_json["creationProperties"]
+        if "layout" in cp:
+            cpl = cp["layout"]
+    if not cpl and "layout" in dset_json:
+        # fallback to dset_json layout
+        cpl = dset_json["layout"]
+    if cpl is None:
+        log.warn(f"no layout found for {dset_json}")
+    return cpl
+
+
+def getDatasetLayoutClass(dset_json):
+    """ return layout class """
+    chunk_layout = None
+    cp_layout = getDatasetCreationPropertyLayout(dset_json)
+    # check creation properties first
+    if cp_layout:
+        if "class" in cp_layout:
+            chunk_layout = cp_layout["class"]
+    # otherwise, get class prop from layout
+    if chunk_layout is None and "layout" in dset_json:
+        layout = dset_json["layout"]
+        if "class" in layout:
+            chunk_layout = layout["class"]
+    return chunk_layout
+
+
+def getChunkDims(dset_json):
+    """ get chunk shape for given dset_json """
+    cpl = getDatasetCreationPropertyLayout(dset_json)
+    if cpl and "dims" in cpl:
+        return cpl["dims"]
+    # otherwise, check the 'layout' key
+    if 'layout' in dset_json:
+        layout = dset_json["layout"]
+        if "dims" in layout:
+            return layout["dims"]
+    return None  # not found
+
+
 class ItemIterator:
     """
     Class to iterator through items in a selection
     """
 
     def __init__(self, selection):
         self._selection = selection
         self._rank = len(selection)
-        self._index = [0, ] * self._rank
+        self._index = [
+            0,
+        ] * self._rank
         for i in range(self._rank):
             s = self._selection[i]
             self._index[i] = s.start
 
     def __iter__(self):
         return self
 
     def next(self):
         if self._index[0] >= self._selection[0].stop:
             # ran past last item, end iteration
             raise StopIteration()
         dim = self._rank - 1
 
-        index = [0, ] * self._rank
+        index = [
+            0,
+        ] * self._rank
         for i in range(self._rank):
             index[i] = self._index[i]
         while dim >= 0:
             s = self._selection[dim]
             self._index[dim] += s.step
             if self._index[dim] < s.stop:
                 if self._rank == 1:
```

### Comparing `hsds-0.7.0b11/hsds/util/fileClient.py` & `hsds-0.8.0/hsds/util/fileClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,66 @@
 import asyncio
 import hashlib
-import os.path as pp
 from os import mkdir, rmdir, listdir, stat, remove, walk
+import os.path as pp
 from asyncio import CancelledError
 from inspect import iscoroutinefunction
 import time
 import aiofiles
 from aiohttp.web_exceptions import HTTPNotFound, HTTPInternalServerError
 from aiohttp.web_exceptions import HTTPBadRequest
 from .. import hsds_logger as log
 from .. import config
 
 
-class FileClient():
+class FileClient:
     """
-     Utility class for reading and storing data to local files
-     using aiofiles package
+    Utility class for reading and storing data to local files
+    using aiofiles package
     """
 
     def __init__(self, app):
         self._app = app
-        self._root_dir = config.get("root_dir")
-        if not self._root_dir:
+        root_dir = config.get("root_dir")
+        if not root_dir:
             log.error("FileClient init: root_dir config not set")
             raise HTTPInternalServerError()
-        if not pp.isdir(self._root_dir):
+        if not pp.isdir(root_dir):
             log.error("FileClient init: root folder does not exist")
             raise HTTPInternalServerError()
-        if not pp.isabs(self._root_dir):
+        if not pp.isabs(root_dir):
             log.error("FileClient init: root dir most have absolute path")
             raise HTTPInternalServerError()
+        self._root_dir = pp.normpath(root_dir)
 
     def _validateBucket(self, bucket):
-        if not bucket or pp.isabs(bucket) or pp.dirname(bucket):
-            msg = "invalid bucket name"
+        if not bucket:
+            msg = "bucket not set"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
+        if bucket.find("\\") != -1:
+            msg = f"bucket: {bucket} contains invalid character, backslash"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
+        if bucket.find("/") != -1:
+            msg = f"bucket: {bucket} contains invalid character, slash"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
 
     def _validateKey(self, key):
-        if not key or pp.isabs(key):
-            msg = "invalid key name"
+        if not key:
+            msg = "key not set"
+            log.warn(msg)
+            raise HTTPBadRequest(reason=msg)
+        if key.startswith("/") or key.startswith("\\"):
+            msg = f"invalid key: {key}, cannot start with slash"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
 
-    def _getFilePath(self, bucket, key=''):
+    def _getFilePath(self, bucket, key=""):
         filepath = pp.join(self._root_dir, bucket, key)
         return pp.normpath(filepath)
 
     def _getFileStats(self, filepath, data=None):
         log.debug(f"_getFileStats({filepath})")
         if data is not None:
             if not isinstance(data, bytes):
@@ -60,66 +73,80 @@
                 ETag = hash_object.hexdigest()
         else:
             msg = "getFileStats - data is None, so ETag will not be computed"
             log.debug(msg)
             ETag = ""
         try:
             file_stats = stat(filepath)
-            key_stats = {"ETag": ETag,
-                         "Size": file_stats.st_size,
-                         "LastModified": file_stats.st_mtime}
+            key_stats = {
+                "ETag": ETag,
+                "Size": file_stats.st_size,
+                "LastModified": file_stats.st_mtime,
+            }
             log.info(f"_getFileStats({filepath}) returning: {key_stats}")
         except FileNotFoundError:
             raise HTTPNotFound()
         return key_stats
 
     def _file_stats_increment(self, counter, inc=1):
-        """ Incremenet the indicated connter
-        """
+        """Incremenet the indicated connter"""
         if "file_stats" not in self._app:
             # setup stats
             file_stats = {}
             file_stats["get_count"] = 0
             file_stats["put_count"] = 0
             file_stats["delete_count"] = 0
             file_stats["list_count"] = 0
             file_stats["error_count"] = 0
             file_stats["bytes_in"] = 0
             file_stats["bytes_out"] = 0
             self._app["file_stats"] = file_stats
-        file_stats = self._app['file_stats']
+        file_stats = self._app["file_stats"]
         if counter not in file_stats:
             log.error(f"unexpected counter for file_stats: {counter}")
             return
         if inc < 1:
             log.error(f"unexpected inc for file_stats: {inc}")
             return
 
-        file_stats[counter] += inc
+    def getURIFromKey(self, key, bucket=None):
+        """ return filesystem specific URI for given key and bucket """
+        if not bucket:
+            log.error("getURIFromKey, bucket not set")
+            raise HTTPInternalServerError()
+        if not key:
+            log.error("getURIFromKey, key not set")
+            raise HTTPInternalServerError()
+        if key[0] == "/":
+            key = key[1:]
+
+        uri = self._getFilePath(key=key, bucket=bucket)
+
+        return uri
 
     async def get_object(self, key, bucket=None, offset=0, length=-1):
-        """ Return data for object at given key.
-           If Range is set, return the given byte range.
+        """Return data for object at given key.
+        If Range is set, return the given byte range.
         """
         self._validateBucket(bucket)
         self._validateKey(key)
 
         if length > 0:
             range = f"bytes={offset}-{offset+length-1}"
             log.info(f"storage range request: {range}")
 
         filepath = self._getFilePath(bucket, key)
         log.info(f"get_object - filepath: {filepath}")
 
         start_time = time.time()
-        log.debug(f"fileClient.get_object({bucket}/{key} start: {start_time}")
+        log.debug(f"fileClient.get_object({filepath} start: {start_time}")
         loop = asyncio.get_event_loop()
 
         try:
-            async with aiofiles.open(filepath, loop=loop, mode='rb') as f:
+            async with aiofiles.open(filepath, loop=loop, mode="rb") as f:
                 if offset:
                     await f.seek(offset)
                 if length > 0:
                     data = await f.read(length)
                 else:
                     data = await f.read()
             finish_time = time.time()
@@ -145,16 +172,16 @@
             self._file_stats_increment("error_count")
             msg = f"Unexpected Exception {type(e)} get get_object {key}: {e}"
             log.error(msg)
             raise HTTPInternalServerError()
         return data
 
     async def put_object(self, key, data, bucket=None):
-        """ Write data to given key.
-            Returns client specific dict on success
+        """Write data to given key.
+        Returns client specific dict on success
         """
         self._validateBucket(bucket)
         self._validateKey(key)
 
         dirpath = self._getFilePath(bucket)
         if not pp.isdir(dirpath):
             msg = "fileClient.put_object - bucket at path: "
@@ -181,15 +208,15 @@
 
                     if not pp.isdir(dirpath):
                         log.debug(f"mkdir({dirpath})")
                         mkdir(dirpath)
                     else:
                         log.debug(f"isdir {dirpath} found")
             log.debug(f"open({filepath}, 'wb')")
-            async with aiofiles.open(filepath, loop=loop, mode='wb') as f:
+            async with aiofiles.open(filepath, loop=loop, mode="wb") as f:
                 await f.write(data)
             finish_time = time.time()
             msg = f"fileClient.put_object({key} bucket={bucket}) "
             msg += f"start={start_time:.4f} finish={finish_time:.4f} "
             msg += f"elapsed={finish_time-start_time:.4f} bytes={len(data)}"
             log.info(msg)
             write_rsp = self._getFileStats(filepath, data=data)
@@ -210,20 +237,19 @@
             log.error(msg)
             raise HTTPInternalServerError()
 
         if data and len(data) > 0:
             self._file_stats_increment("bytes_out", inc=len(data))
             msg = f"fileClient.put_object {key} complete, "
             msg += f"write_rsp: {write_rsp}"
-        log.debug(msg)
+            log.debug(msg)
         return write_rsp
 
     async def delete_object(self, key, bucket=None):
-        """ Deletes the object at the given key
-        """
+        """Deletes the object at the given key"""
         self._validateBucket(bucket)
         self._validateKey(key)
         filepath = self._getFilePath(bucket, key)
 
         start_time = time.time()
         msg = f"fileClient.delete_object({bucket}/{key} start: {start_time}"
         log.debug(msg)
@@ -273,34 +299,43 @@
             log.warn(f"get_key_stats - key: {key} not found")
             raise HTTPNotFound()
         filepath = self._getFilePath(bucket, key)
         key_stats = self._getFileStats(filepath)
 
         return key_stats
 
-    async def list_keys(self, prefix='', deliminator='', suffix='',
-                        include_stats=False, callback=None, bucket=None,
-                        limit=None):
-        """ return keys matching the arguments
-        """
+    async def list_keys(
+        self,
+        prefix="",
+        deliminator="",
+        suffix="",
+        include_stats=False,
+        callback=None,
+        bucket=None,
+        limit=None,
+    ):
+        """return keys matching the arguments"""
         self._validateBucket(bucket)
-        if deliminator and deliminator != '/':
+        if deliminator and deliminator != "/":
             msg = "Only '/' is supported as deliminator"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
 
         msg = f"list_keys('{prefix}','{deliminator}','{suffix}' "
         msg += f"include_stats={include_stats}, bucket={bucket}, "
         msg += f"callback {'set' if callback is not None else 'not set'}"
         log.info(msg)
 
+        filesep = pp.normpath("/")  # '/' on linux, '\\' on windows
+
         await asyncio.sleep(0)  # for async compat
         basedir = pp.join(self._root_dir, bucket)
         if prefix:
             basedir = pp.join(basedir, prefix)
+        basedir = pp.normpath(basedir)
         log.debug(f"fileClient listKeys for directory: {basedir}")
 
         if not pp.isdir(basedir):
             msg = f"listkeys - {basedir} not found"
             log.warn(msg)
             raise HTTPNotFound()
 
@@ -310,69 +345,78 @@
         for root, dirs, filelist in walk(basedir):
             if deliminator:
                 dirs.sort()
                 for dirname in dirs:
                     if suffix and not dirname.endswith(suffix):
                         continue
                     log.debug(f"got dirname: {dirname}")
-                    filename = pp.join(root[len(basedir):], dirname)
-                    filename += '/'
+                    nlen = len(basedir)
+                    filename = f"{root[nlen:]}{dirname}{filesep}"
                     files.append(filename)
                     if limit and len(files) >= limit:
                         break
                 break  # don't recurse into subdirs
 
             else:
                 filelist.sort()
                 for filename in filelist:
                     if suffix and not filename.endswith(suffix):
                         continue
-                    filepath = pp.join(root[len(basedir):], filename)
+                    nlen = len(basedir)
+                    filepath = pp.join(root[nlen:], filename)
                     files.append(filepath)
                     if limit and len(files) >= limit:
                         break
 
         # use a dictionary to hold return values if stats are needed
         key_names = {} if include_stats else []
         count = 0
         for filename in files:
-            if filename.startswith('/'):
+            if filename.startswith(filesep):
                 filename = filename[1:]
             log.debug(f"filename: {filename}, basedir: {basedir}")
             if suffix and not filename.endswith(suffix):
                 continue
             if include_stats:
                 filepath = pp.join(basedir, filename)
                 with open(filepath, "rb") as f:
                     data = f.read()
                     msg = f"list_keys: read file: {filepath}, "
                     msg += f"{len(data)} bytes, for getFileStats"
                     log.debug(msg)
                     key_stats = self._getFileStats(filepath, data=data)
                 key_name = pp.join(prefix, filename)
+                # replace any windows-style sep with linux
+                key_name = key_name.replace("\\", "/")
                 key_names[key_name] = key_stats
             else:
-                key_names.append(pp.join(prefix, filename))
+                key_name = pp.join(prefix, filename)
+                # replace any windows-style sep with linux
+                key_name = key_name.replace("\\", "/")
+                key_names.append(key_name)
+
             if limit and len(key_names) == limit:
                 break
         count += len(key_names)
         if callback:
             if iscoroutinefunction(callback):
                 await callback(self._app, key_names)
             else:
                 callback(self._app, key_names)
             key_names = {} if include_stats else []  # reset
 
         log.info(f"listKeys done, got {count} keys")
+        for key in key_names:
+            log.debug(key)
         if not callback and count != len(key_names):
             msg = f"expected {count} keys in return list but "
             msg == f"got {len(key_names)}"
             log.warning(msg)
 
         return key_names
 
     async def releaseClient(self):
-        """ release the client collection
-           (Used for cleanup on application exit)
+        """release the client collection
+        (Used for cleanup on application exit)
         """
         await asyncio.sleep(0)  # for async compat
         log.info("release fileClient")
```

### Comparing `hsds-0.7.0b11/hsds/util/hdf5dtype.py` & `hsds-0.8.0/hsds/util/hdf5dtype.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,78 +10,86 @@
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 
 import weakref
 import numpy as np
 
 
-class Reference():
+class Reference:
     """
-        Represents an HDF5 object reference
+    Represents an HDF5 object reference
     """
+
     @property
     def id(self):
-        """ Low-level identifier appropriate for this object """
+        """Low-level identifier appropriate for this object"""
         return self._id
 
     @property
     def objref(self):
-        """ Weak reference to object """
+        """Weak reference to object"""
         return self._objref  # return weak ref to ref'd object
 
     def __init__(self, bind):
-        """ Create a new reference by binding to
-              a group/dataset/committed type
+        """Create a new reference by binding to
+        a group/dataset/committed type
         """
         self._id = bind._id
         self._objref = weakref.ref(bind)
 
     def __repr__(self):
         return "<HDF5 object reference>"
 
     def tolist(self):
         if type(self._id.id) is not str:
             raise TypeError("Expected string id")
-        if self._id.objtype_code == 'd':
-            return [("datasets/" + self._id.id), ]
-        elif self._id.objtype_code == 'g':
-            return [("groups/" + self._id.id), ]
-        elif self._id.objtype_code == 't':
-            return [("datatypes/" + self._id.id), ]
+        if self._id.objtype_code == "d":
+            return [
+                ("datasets/" + self._id.id),
+            ]
+        elif self._id.objtype_code == "g":
+            return [
+                ("groups/" + self._id.id),
+            ]
+        elif self._id.objtype_code == "t":
+            return [
+                ("datatypes/" + self._id.id),
+            ]
         else:
             raise TypeError("Unexpected id type")
 
 
-class RegionReference():
+class RegionReference:
     """
-        Represents an HDF5 region reference
+    Represents an HDF5 region reference
     """
+
     @property
     def id(self):
-        """ Low-level identifier appropriate for this object """
+        """Low-level identifier appropriate for this object"""
         return self._id
 
     @property
     def objref(self):
-        """ Weak reference to object """
+        """Weak reference to object"""
         return self._objref  # return weak ref to ref'd object
 
     def __init__(self, bind):
-        """ Create a new reference by binding to
-              a group/dataset/committed type
+        """Create a new reference by binding to
+        a group/dataset/committed type
         """
         self._id = bind._id
         self._objref = weakref.ref(bind)
 
     def __repr__(self):
         return "<HDF5 region reference>"
 
 
 def special_dtype(**kwds):
-    """ Create a new h5py "special" type.  Only one keyword may be given.
+    """Create a new h5py "special" type.  Only one keyword may be given.
 
     Legal keywords are:
 
     vlen = basetype
         Base type for HDF5 variable-length datatype. This can be Python
         str type or instance of np.dtype.
         Example: special_dtype( vlen=str )
@@ -89,56 +97,56 @@
     enum = (basetype, values_dict)
         Create a NumPy representation of an HDF5 enumerated type.  Provide
         a 2-tuple containing an (integer) base dtype and a dict mapping
         string names to integer values.
 
     ref = Reference | RegionReference
         Create a NumPy representation of an HDF5 object or region reference
-        type.    """
+        type."""
 
     if len(kwds) != 1:
         raise TypeError("Exactly one keyword may be provided")
 
     name, val = kwds.popitem()
 
-    if name == 'vlen':
+    if name == "vlen":
 
-        return np.dtype('O', metadata={'vlen': val})
+        return np.dtype("O", metadata={"vlen": val})
 
-    if name == 'enum':
+    if name == "enum":
 
         try:
             dt, enum_vals = val
         except TypeError:
             msg = "Enums must be created from a 2-tuple "
             msg += "(basetype, values_dict)"
             raise TypeError(msg)
 
         dt = np.dtype(dt)
         if dt.kind not in "iu":
             raise TypeError("Only integer types can be used as enums")
 
-        return np.dtype(dt, metadata={'enum': enum_vals})
+        return np.dtype(dt, metadata={"enum": enum_vals})
 
-    if name == 'ref':
+    if name == "ref":
         dt = None
         if val is Reference:
-            dt = np.dtype('S48', metadata={'ref': Reference})
+            dt = np.dtype("S48", metadata={"ref": Reference})
         elif val is RegionReference:
-            dt = np.dtype('S48', metadata={'ref': RegionReference})
+            dt = np.dtype("S48", metadata={"ref": RegionReference})
         else:
             raise ValueError("Ref class must be Reference or RegionReference")
 
         return dt
 
     raise TypeError(f'Unknown special type "{name}"')
 
 
 def check_dtype(**kwds):
-    """ Check a dtype for h5py special type "hint" information.  Only one
+    """Check a dtype for h5py special type "hint" information.  Only one
     keyword may be given.
 
     vlen = dtype
         If the dtype represents an HDF5 vlen, returns the Python base class.
         Currently only builting string vlens (str) are supported.  Returns
         None if the dtype does not represent an HDF5 vlen.
 
@@ -154,15 +162,15 @@
     """
 
     if len(kwds) != 1:
         raise TypeError("Exactly one keyword may be provided")
 
     name, dt = kwds.popitem()
 
-    if name not in ('vlen', 'enum', 'ref'):
+    if name not in ("vlen", "enum", "ref"):
         raise TypeError('Unknown special type "%s"' % name)
 
     try:
         return dt.metadata[name]
     except TypeError:
         return None
     except KeyError:
@@ -170,75 +178,75 @@
 
 
 def getTypeResponse(typeItem):
     """
     Convert the given type item  to a predefined type string for
         predefined integer and floating point types ("H5T_STD_I64LE", et. al).
         For compound types, recursively iterate through the typeItem and do
-        same conversion for fields of the compound type.  """
+        same conversion for fields of the compound type."""
     response = None
-    if 'uuid' in typeItem:
+    if "uuid" in typeItem:
         # committed type, just return uuid
-        response = 'datatypes/' + typeItem['uuid']
-    elif typeItem['class'] in ('H5T_INTEGER', 'H5T_FLOAT'):
+        response = "datatypes/" + typeItem["uuid"]
+    elif typeItem["class"] in ("H5T_INTEGER", "H5T_FLOAT"):
         # just return the class and base for pre-defined types
         response = {}
-        response['class'] = typeItem['class']
-        response['base'] = typeItem['base']
-    elif typeItem['class'] == 'H5T_OPAQUE':
+        response["class"] = typeItem["class"]
+        response["base"] = typeItem["base"]
+    elif typeItem["class"] == "H5T_OPAQUE":
         response = {}
-        response['class'] = 'H5T_OPAQUE'
-        response['size'] = typeItem['size']
-    elif typeItem['class'] == 'H5T_REFERENCE':
+        response["class"] = "H5T_OPAQUE"
+        response["size"] = typeItem["size"]
+    elif typeItem["class"] == "H5T_REFERENCE":
         response = {}
-        response['class'] = 'H5T_REFERENCE'
-        response['base'] = typeItem['base']
-    elif typeItem['class'] == 'H5T_COMPOUND':
+        response["class"] = "H5T_REFERENCE"
+        response["base"] = typeItem["base"]
+    elif typeItem["class"] == "H5T_COMPOUND":
         response = {}
-        response['class'] = 'H5T_COMPOUND'
+        response["class"] = "H5T_COMPOUND"
         fieldList = []
-        for field in typeItem['fields']:
+        for field in typeItem["fields"]:
             fieldItem = {}
-            fieldItem['name'] = field['name']
-            fieldItem['type'] = getTypeResponse(field['type'])  # recurse call
+            fieldItem["name"] = field["name"]
+            fieldItem["type"] = getTypeResponse(field["type"])  # recurse call
             fieldList.append(fieldItem)
-        response['fields'] = fieldList
+        response["fields"] = fieldList
     else:
-        response = {}   # otherwise, return full type
+        response = {}  # otherwise, return full type
         for k in typeItem.keys():
-            if k == 'base':
+            if k == "base":
                 if isinstance(typeItem[k], dict):
                     response[k] = getTypeResponse(typeItem[k])  # recurse call
                 else:
                     response[k] = typeItem[k]  # predefined type
-            elif k not in ('size', 'base_size'):
+            elif k not in ("size", "base_size"):
                 response[k] = typeItem[k]
     return response
 
 
 def getTypeItem(dt, metadata=None):
     """
     Return type info.
           For primitive types, return string with typename
           For compound types return array of dictionary items
     """
     predefined_int_types = {
-        'int8':    'H5T_STD_I8',
-        'uint8':   'H5T_STD_U8',
-        'int16':   'H5T_STD_I16',
-        'uint16':  'H5T_STD_U16',
-        'int32':   'H5T_STD_I32',
-        'uint32':  'H5T_STD_U32',
-        'int64':   'H5T_STD_I64',
-        'uint64':  'H5T_STD_U64'
+        "int8": "H5T_STD_I8",
+        "uint8": "H5T_STD_U8",
+        "int16": "H5T_STD_I16",
+        "uint16": "H5T_STD_U16",
+        "int32": "H5T_STD_I32",
+        "uint32": "H5T_STD_U32",
+        "int64": "H5T_STD_I64",
+        "uint64": "H5T_STD_U64",
     }
     predefined_float_types = {
-        'float16': 'H5T_IEEE_F16',
-        'float32': 'H5T_IEEE_F32',
-        'float64': 'H5T_IEEE_F64'
+        "float16": "H5T_IEEE_F16",
+        "float32": "H5T_IEEE_F32",
+        "float64": "H5T_IEEE_F64",
     }
     # print(">getTypeItem:", dt.str)
     if not metadata and dt.metadata:
         metadata = dt.metadata
     # if metadata:
     #    print(">  metadata:", metadata)
     # if dt.shape:
@@ -246,159 +254,156 @@
     # if len(dt) > 1:
     #    print(">  len:", len(dt))
 
     type_info = {}
     if len(dt) > 1:
         # compound type
         names = dt.names
-        type_info['class'] = 'H5T_COMPOUND'
+        type_info["class"] = "H5T_COMPOUND"
         fields = []
         for name in names:
-            field = {'name': name}
-            field['type'] = getTypeItem(dt[name])
+            field = {"name": name}
+            field["type"] = getTypeItem(dt[name])
             fields.append(field)
-            type_info['fields'] = fields
+            type_info["fields"] = fields
     elif dt.shape:
         # array type
         if dt.base == dt:
             raise TypeError("Expected base type to be different than parent")
         # array type
-        type_info['dims'] = dt.shape
-        type_info['class'] = 'H5T_ARRAY'
+        type_info["dims"] = dt.shape
+        type_info["class"] = "H5T_ARRAY"
         # print(">  array type, metadata:", metadata)
-        type_info['base'] = getTypeItem(dt.base, metadata=metadata)
-    elif dt.kind == 'O':
+        type_info["base"] = getTypeItem(dt.base, metadata=metadata)
+    elif dt.kind == "O":
         # vlen string or data
         #
         # check for h5py variable length extension
 
         if metadata and "vlen" in metadata:
             vlen_check = metadata["vlen"]
             if vlen_check is not None and not isinstance(vlen_check, np.dtype):
                 vlen_check = np.dtype(vlen_check)
 
         if metadata and "ref" in metadata:
             ref_check = metadata["ref"]
         else:
             ref_check = check_dtype(ref=dt.base)
         if vlen_check == bytes:
-            type_info['class'] = 'H5T_STRING'
-            type_info['length'] = 'H5T_VARIABLE'
-            type_info['charSet'] = 'H5T_CSET_ASCII'
-            type_info['strPad'] = 'H5T_STR_NULLTERM'
+            type_info["class"] = "H5T_STRING"
+            type_info["length"] = "H5T_VARIABLE"
+            type_info["charSet"] = "H5T_CSET_ASCII"
+            type_info["strPad"] = "H5T_STR_NULLTERM"
         elif vlen_check == str:
-            type_info['class'] = 'H5T_STRING'
-            type_info['length'] = 'H5T_VARIABLE'
-            type_info['charSet'] = 'H5T_CSET_UTF8'
-            type_info['strPad'] = 'H5T_STR_NULLTERM'
+            type_info["class"] = "H5T_STRING"
+            type_info["length"] = "H5T_VARIABLE"
+            type_info["charSet"] = "H5T_CSET_UTF8"
+            type_info["strPad"] = "H5T_STR_NULLTERM"
         elif isinstance(vlen_check, np.dtype):
             # vlen data
-            type_info['class'] = 'H5T_VLEN'
-            type_info['size'] = 'H5T_VARIABLE'
-            type_info['base'] = getTypeItem(vlen_check)
+            type_info["class"] = "H5T_VLEN"
+            type_info["size"] = "H5T_VARIABLE"
+            type_info["base"] = getTypeItem(vlen_check)
         elif vlen_check is not None:
             #  unknown vlen type
             raise TypeError("Unknown h5py vlen type: " + str(vlen_check))
         elif ref_check is not None:
             # a reference type
-            type_info['class'] = 'H5T_REFERENCE'
+            type_info["class"] = "H5T_REFERENCE"
 
             if ref_check is Reference:
-                type_info['base'] = 'H5T_STD_REF_OBJ'  # objref
+                type_info["base"] = "H5T_STD_REF_OBJ"  # objref
             elif ref_check is RegionReference:
-                type_info['base'] = 'H5T_STD_REF_DSETREG'  # region ref
+                type_info["base"] = "H5T_STD_REF_DSETREG"  # region ref
             else:
                 raise TypeError("unexpected reference type")
         else:
             raise TypeError("unknown object type")
-    elif dt.kind == 'V':
+    elif dt.kind == "V":
         # void type
-        type_info['class'] = 'H5T_OPAQUE'
-        type_info['size'] = dt.itemsize
-        type_info['tag'] = ''  # todo - determine tag
-    elif dt.base.kind == 'S':
+        type_info["class"] = "H5T_OPAQUE"
+        type_info["size"] = dt.itemsize
+        type_info["tag"] = ""  # todo - determine tag
+    elif dt.base.kind == "S":
         # check for object reference
         ref_check = check_dtype(ref=dt.base)
         if ref_check is not None:
             # a reference type
-            type_info['class'] = 'H5T_REFERENCE'
+            type_info["class"] = "H5T_REFERENCE"
 
             if ref_check is Reference:
-                type_info['base'] = 'H5T_STD_REF_OBJ'  # objref
+                type_info["base"] = "H5T_STD_REF_OBJ"  # objref
             elif ref_check is RegionReference:
-                type_info['base'] = 'H5T_STD_REF_DSETREG'  # region ref
+                type_info["base"] = "H5T_STD_REF_DSETREG"  # region ref
             else:
                 raise TypeError("unexpected reference type")
         else:
             # Fixed length string type
-            type_info['class'] = 'H5T_STRING'
-        type_info['charSet'] = 'H5T_CSET_ASCII'
-        type_info['length'] = dt.itemsize
-        type_info['strPad'] = 'H5T_STR_NULLPAD'
-    elif dt.base.kind == 'U':
+            type_info["class"] = "H5T_STRING"
+        type_info["charSet"] = "H5T_CSET_ASCII"
+        type_info["length"] = dt.itemsize
+        type_info["strPad"] = "H5T_STR_NULLPAD"
+    elif dt.base.kind == "U":
         # Fixed length unicode type
         raise TypeError("Fixed length unicode type is not supported")
 
-    elif dt.kind == 'b':
+    elif dt.kind == "b":
         # boolean type - h5py stores as enum
         # assume LE unless the numpy byteorder is '>'
-        byteorder = 'LE'
-        if dt.base.byteorder == '>':
-            byteorder = 'BE'
+        byteorder = "LE"
+        if dt.base.byteorder == ">":
+            byteorder = "BE"
         # this mapping is an h5py convention for boolean support
-        mapping = {
-            "FALSE": 0,
-            "TRUE": 1
-        }
-        type_info['class'] = 'H5T_ENUM'
-        type_info['mapping'] = mapping
+        mapping = {"FALSE": 0, "TRUE": 1}
+        type_info["class"] = "H5T_ENUM"
+        type_info["mapping"] = mapping
         base_info = {"class": "H5T_INTEGER"}
-        base_info['base'] = "H5T_STD_I8" + byteorder
+        base_info["base"] = "H5T_STD_I8" + byteorder
         type_info["base"] = base_info
-    elif dt.kind == 'f':
+    elif dt.kind == "f":
         # floating point type
-        type_info['class'] = 'H5T_FLOAT'
-        byteorder = 'LE'
-        if dt.byteorder == '>':
-            byteorder = 'BE'
+        type_info["class"] = "H5T_FLOAT"
+        byteorder = "LE"
+        if dt.byteorder == ">":
+            byteorder = "BE"
         if dt.name in predefined_float_types:
             # maps to one of the HDF5 predefined types
             float_type = predefined_float_types[dt.base.name]
-            type_info['base'] = float_type + byteorder
+            type_info["base"] = float_type + byteorder
         else:
             raise TypeError("Unexpected floating point type: " + dt.name)
-    elif dt.kind == 'i' or dt.kind == 'u':
+    elif dt.kind == "i" or dt.kind == "u":
         # integer type
 
         # assume LE unless the numpy byteorder is '>'
-        byteorder = 'LE'
-        if dt.base.byteorder == '>':
-            byteorder = 'BE'
+        byteorder = "LE"
+        if dt.base.byteorder == ">":
+            byteorder = "BE"
 
         # numpy integer type - but check to see if this is the hypy
         # enum extension
         if metadata and "enum" in metadata:
             # yes, this is an enum!
             mapping = metadata["enum"]
-            type_info['class'] = 'H5T_ENUM'
-            type_info['mapping'] = mapping
+            type_info["class"] = "H5T_ENUM"
+            type_info["mapping"] = mapping
             if dt.name not in predefined_int_types:
                 raise TypeError("Unexpected integer type: " + dt.name)
             # maps to one of the HDF5 predefined types
             base_info = {"class": "H5T_INTEGER"}
-            base_info['base'] = predefined_int_types[dt.name] + byteorder
+            base_info["base"] = predefined_int_types[dt.name] + byteorder
             type_info["base"] = base_info
         else:
-            type_info['class'] = 'H5T_INTEGER'
+            type_info["class"] = "H5T_INTEGER"
             base_name = dt.name
 
             if dt.name not in predefined_int_types:
                 raise TypeError("Unexpected integer type: " + dt.name)
 
-            type_info['base'] = predefined_int_types[base_name] + byteorder
+            type_info["base"] = predefined_int_types[base_name] + byteorder
 
     else:
         # unexpected kind
         raise TypeError(f"unexpected dtype kind: {dt.kind}")
 
     return type_info
 
@@ -409,138 +414,141 @@
         For variable length types (e.g. variable length strings),
         return the string "H5T_VARIABLE"
     """
     # handle the case where we are passed a primitive type first
     if isinstance(typeItem, str) or isinstance(typeItem, bytes):
         for type_prefix in ("H5T_STD_I", "H5T_STD_U", "H5T_IEEE_F"):
             if typeItem.startswith(type_prefix):
-                num_bits = typeItem[len(type_prefix):]
-                if num_bits[-2:] in ('LE', 'BE'):
+                nlen = len(type_prefix)
+                num_bits = typeItem[nlen:]
+                if num_bits[-2:] in ("LE", "BE"):
                     num_bits = num_bits[:-2]
                 try:
                     return int(num_bits) // 8
                 except ValueError:
                     raise TypeError("Invalid Type")
         # none of the expect primative types mathched
         raise TypeError("Invalid Type")
     if not isinstance(typeItem, dict):
         raise TypeError("invalid type")
 
     item_size = 0
-    if 'class' not in typeItem:
+    if "class" not in typeItem:
         raise KeyError("'class' not provided")
-    typeClass = typeItem['class']
+    typeClass = typeItem["class"]
 
-    if typeClass == 'H5T_INTEGER':
-        if 'base' not in typeItem:
+    if typeClass == "H5T_INTEGER":
+        if "base" not in typeItem:
             raise KeyError("'base' not provided")
-        item_size = getItemSize(typeItem['base'])
+        item_size = getItemSize(typeItem["base"])
 
-    elif typeClass == 'H5T_FLOAT':
-        if 'base' not in typeItem:
+    elif typeClass == "H5T_FLOAT":
+        if "base" not in typeItem:
             raise KeyError("'base' not provided")
-        item_size = getItemSize(typeItem['base'])
+        item_size = getItemSize(typeItem["base"])
 
-    elif typeClass == 'H5T_STRING':
-        if 'length' not in typeItem:
+    elif typeClass == "H5T_STRING":
+        if "length" not in typeItem:
             raise KeyError("'length' not provided")
         item_size = typeItem["length"]
 
-    elif typeClass == 'H5T_VLEN':
+    elif typeClass == "H5T_VLEN":
         item_size = "H5T_VARIABLE"
-    elif typeClass == 'H5T_OPAQUE':
-        if 'size' not in typeItem:
+    elif typeClass == "H5T_OPAQUE":
+        if "size" not in typeItem:
             raise KeyError("'size' not provided")
-        item_size = int(typeItem['size'])
+        item_size = int(typeItem["size"])
 
-    elif typeClass == 'H5T_ARRAY':
-        if 'dims' not in typeItem:
+    elif typeClass == "H5T_ARRAY":
+        if "dims" not in typeItem:
             raise KeyError("'dims' must be provided for array types")
-        if 'base' not in typeItem:
+        if "base" not in typeItem:
             raise KeyError("'base' not provided")
-        item_size = getItemSize(typeItem['base'])
+        item_size = getItemSize(typeItem["base"])
 
-    elif typeClass == 'H5T_ENUM':
-        if 'base' not in typeItem:
+    elif typeClass == "H5T_ENUM":
+        if "base" not in typeItem:
             raise KeyError("'base' must be provided for enum types")
-        item_size = getItemSize(typeItem['base'])
+        item_size = getItemSize(typeItem["base"])
 
-    elif typeClass == 'H5T_REFERENCE':
-        if 'length' in typeItem:
-            item_size = typeItem['length']
-        elif 'base' in typeItem and typeItem['base'] == 'H5T_STD_REF_OBJ':
+    elif typeClass == "H5T_REFERENCE":
+        if "length" in typeItem:
+            item_size = typeItem["length"]
+        elif "base" in typeItem and typeItem["base"] == "H5T_STD_REF_OBJ":
             # obj ref values are in the form: "groups/<id>" or
             # "datasets/<id>" or "datatypes/<id>"
             item_size = 48
         else:
             raise KeyError("Unable to determine item size for reference type")
-    elif typeClass == 'H5T_COMPOUND':
-        if 'fields' not in typeItem:
+    elif typeClass == "H5T_COMPOUND":
+        if "fields" not in typeItem:
             raise KeyError("'fields' not provided for compound type")
-        fields = typeItem['fields']
+        fields = typeItem["fields"]
         if not isinstance(fields, list):
             raise TypeError("Type Error: expected list type for 'fields'")
         if not fields:
             raise KeyError("no 'field' elements provided")
         # add up the size of each sub-field
         for field in fields:
             if not isinstance(field, dict):
                 raise TypeError("Expected dictionary type for field")
-            if 'type' not in field:
+            if "type" not in field:
                 raise KeyError("'type' missing from field")
-            subtype_size = getItemSize(field['type'])  # recursive call
+            subtype_size = getItemSize(field["type"])  # recursive call
             if subtype_size == "H5T_VARIABLE":
                 item_size = "H5T_VARIABLE"
                 break  # don't need to look at the rest
 
             item_size += subtype_size
     else:
         raise TypeError("Invalid type class")
 
     # calculate array type
-    if 'dims' in typeItem and isinstance(item_size, int):
-        dims = typeItem['dims']
+    if "dims" in typeItem and isinstance(item_size, int):
+        dims = typeItem["dims"]
         for dim in dims:
             item_size *= dim
 
     return item_size
 
 
 def getNumpyTypename(hdf5TypeName, typeClass=None):
     predefined_int_types = {
-          'H5T_STD_I8':  'i1',
-          'H5T_STD_U8':  'u1',
-          'H5T_STD_I16': 'i2',
-          'H5T_STD_U16': 'u2',
-          'H5T_STD_I32': 'i4',
-          'H5T_STD_U32': 'u4',
-          'H5T_STD_I64': 'i8',
-          'H5T_STD_U64': 'u8'
+        "H5T_STD_I8": "i1",
+        "H5T_STD_U8": "u1",
+        "H5T_STD_I16": "i2",
+        "H5T_STD_U16": "u2",
+        "H5T_STD_I32": "i4",
+        "H5T_STD_U32": "u4",
+        "H5T_STD_I64": "i8",
+        "H5T_STD_U64": "u8",
     }
     predefined_float_types = {
-          'H5T_IEEE_F16': 'f2',
-          'H5T_IEEE_F32': 'f4',
-          'H5T_IEEE_F64': 'f8'
+        "H5T_IEEE_F16": "f2",
+        "H5T_IEEE_F32": "f4",
+        "H5T_IEEE_F64": "f8",
     }
 
     if len(hdf5TypeName) < 3:
         raise Exception("Type Error: invalid typename: ")
-    endian = '<'  # default endian
+    endian = "<"  # default endian
     key = hdf5TypeName
-    if hdf5TypeName.endswith('LE'):
+    if hdf5TypeName.endswith("LE"):
         key = hdf5TypeName[:-2]
-    elif hdf5TypeName.endswith('BE'):
+    elif hdf5TypeName.endswith("BE"):
         key = hdf5TypeName[:-2]
-        endian = '>'
+        endian = ">"
 
-    if key in predefined_int_types and (typeClass is None or
-                                        typeClass == 'H5T_INTEGER'):
+    if key in predefined_int_types and (
+        typeClass is None or typeClass == "H5T_INTEGER"
+    ):
         return endian + predefined_int_types[key]
-    if key in predefined_float_types and (typeClass is None or
-                                          typeClass == 'H5T_FLOAT'):
+    if key in predefined_float_types and (
+        typeClass is None or typeClass == "H5T_FLOAT"
+    ):
         return endian + predefined_float_types[key]
     raise TypeError("Type Error: invalid type")
 
 
 def createBaseDataType(typeItem):
     dtRet = None
     if type(typeItem) == str:
@@ -548,140 +556,148 @@
         dtName = getNumpyTypename(typeItem)
         dtRet = np.dtype(dtName)
         return dtRet  # return predefined type
 
     if not isinstance(typeItem, dict):
         raise TypeError("Type Error: invalid type")
 
-    if 'class' not in typeItem:
+    if "class" not in typeItem:
         raise KeyError("'class' not provided")
-    typeClass = typeItem['class']
+    typeClass = typeItem["class"]
 
-    dims = ''
-    if 'dims' in typeItem:
-        if typeClass != 'H5T_ARRAY':
+    dims = ""
+    if "dims" in typeItem:
+        if typeClass != "H5T_ARRAY":
             raise TypeError("'dims' only supported for integer types")
 
         dims = None
-        if isinstance(typeItem['dims'], int):
-            dims = (typeItem['dims'])  # make into a tuple
-        elif not isinstance(typeItem['dims'], list) and \
-                not isinstance(typeItem['dims'], tuple):
+        if isinstance(typeItem["dims"], int):
+            dims = typeItem["dims"]  # make into a tuple
+        elif not isinstance(typeItem["dims"], list) and not isinstance(
+            typeItem["dims"], tuple
+        ):
             raise TypeError("expected list or integer for dims")
         else:
-            dims = typeItem['dims']
+            dims = typeItem["dims"]
         dims = str(tuple(dims))
 
-    if typeClass == 'H5T_INTEGER':
-        if 'base' not in typeItem:
+    if typeClass == "H5T_INTEGER":
+        if "base" not in typeItem:
             raise KeyError("'base' not provided")
-        baseType = getNumpyTypename(typeItem['base'], typeClass='H5T_INTEGER')
+        baseType = getNumpyTypename(typeItem["base"], typeClass="H5T_INTEGER")
         dtRet = np.dtype(dims + baseType)
-    elif typeClass == 'H5T_FLOAT':
-        if 'base' not in typeItem:
+    elif typeClass == "H5T_FLOAT":
+        if "base" not in typeItem:
             raise KeyError("'base' not provided")
-        baseType = getNumpyTypename(typeItem['base'], typeClass='H5T_FLOAT')
+        baseType = getNumpyTypename(typeItem["base"], typeClass="H5T_FLOAT")
         dtRet = np.dtype(dims + baseType)
-    elif typeClass == 'H5T_STRING':
-        if 'length' not in typeItem:
+    elif typeClass == "H5T_STRING":
+        if "length" not in typeItem:
             raise KeyError("'length' not provided")
-        if 'charSet' not in typeItem:
+        if "charSet" not in typeItem:
             raise KeyError("'charSet' not provided")
 
-        if typeItem['length'] == 'H5T_VARIABLE':
+        if typeItem["length"] == "H5T_VARIABLE":
             if dims:
                 msg = "ArrayType is not supported for variable len types"
                 raise TypeError(msg)
-            if typeItem['charSet'] == 'H5T_CSET_ASCII':
+            if typeItem["charSet"] == "H5T_CSET_ASCII":
                 dtRet = special_dtype(vlen=bytes)
-            elif typeItem['charSet'] == 'H5T_CSET_UTF8':
+            elif typeItem["charSet"] == "H5T_CSET_UTF8":
                 dtRet = special_dtype(vlen=str)
             else:
                 raise TypeError("unexpected 'charSet' value")
         else:
-            nStrSize = typeItem['length']
+            nStrSize = typeItem["length"]
             if not isinstance(nStrSize, int):
                 raise TypeError("expecting integer value for 'length'")
             type_code = None
-            if typeItem['charSet'] == 'H5T_CSET_ASCII':
-                type_code = 'S'
-            elif typeItem['charSet'] == 'H5T_CSET_UTF8':
+            if typeItem["charSet"] == "H5T_CSET_ASCII":
+                type_code = "S"
+            elif typeItem["charSet"] == "H5T_CSET_UTF8":
                 msg = "fixed-width unicode strings are not supported"
                 raise TypeError(msg)
             else:
                 raise TypeError("unexpected 'charSet' value")
             # a fixed size string
             dtRet = np.dtype(dims + type_code + str(nStrSize))
-    elif typeClass == 'H5T_VLEN':
+    elif typeClass == "H5T_VLEN":
         if dims:
             msg = "ArrayType is not supported for variable len types"
             raise TypeError(msg)
-        if 'base' not in typeItem:
+        if "base" not in typeItem:
             raise KeyError("'base' not provided")
-        baseType = createBaseDataType(typeItem['base'])
+        baseType = createBaseDataType(typeItem["base"])
         dtRet = special_dtype(vlen=np.dtype(baseType))
-    elif typeClass == 'H5T_OPAQUE':
+    elif typeClass == "H5T_OPAQUE":
         if dims:
             msg = "Opaque Type is not supported for variable len types"
             raise TypeError(msg)
-        if 'size' not in typeItem:
+        if "size" not in typeItem:
             raise KeyError("'size' not provided")
-        nSize = int(typeItem['size'])
+        nSize = int(typeItem["size"])
         if nSize <= 0:
             raise TypeError("'size' must be non-negative")
-        dtRet = np.dtype('V' + str(nSize))
-    elif typeClass == 'H5T_ARRAY':
+        dtRet = np.dtype("V" + str(nSize))
+    elif typeClass == "H5T_ARRAY":
         if not dims:
             raise KeyError("'dims' must be provided for array types")
-        if 'base' not in typeItem:
+        if "base" not in typeItem:
             raise KeyError("'base' not provided")
-        arrayBaseType = typeItem['base']
+        arrayBaseType = typeItem["base"]
         if isinstance(arrayBaseType, dict):
             if "class" not in arrayBaseType:
                 raise KeyError("'class' not provided for array base type")
-            type_classes = ('H5T_INTEGER', 'H5T_FLOAT', 'H5T_STRING')
+            type_classes = ("H5T_INTEGER", "H5T_FLOAT", "H5T_STRING")
             if arrayBaseType["class"] not in type_classes:
                 msg = "Array Type base type must be integer, float, or string"
                 raise TypeError(msg)
         baseType = createDataType(arrayBaseType)
         metadata = None
         if baseType.metadata:
             metadata = dict(baseType.metadata)
-            dtRet = np.dtype(dims+baseType.str, metadata=metadata)
+            dtRet = np.dtype(dims + baseType.str, metadata=metadata)
         else:
-            dtRet = np.dtype(dims+baseType.str)
+            dtRet = np.dtype(dims + baseType.str)
         return dtRet  # return predefined type
-    elif typeClass == 'H5T_REFERENCE':
-        if 'base' not in typeItem:
+    elif typeClass == "H5T_REFERENCE":
+        if "base" not in typeItem:
             raise KeyError("'base' not provided")
-        if typeItem['base'] == 'H5T_STD_REF_OBJ':
+        if typeItem["base"] == "H5T_STD_REF_OBJ":
             dtRet = special_dtype(ref=Reference)
-        elif typeItem['base'] == 'H5T_STD_REF_DSETREG':
+        elif typeItem["base"] == "H5T_STD_REF_DSETREG":
             dtRet = special_dtype(ref=RegionReference)
         else:
             raise TypeError("Invalid base type for reference type")
 
-    elif typeClass == 'H5T_ENUM':
-        if 'base' not in typeItem:
+    elif typeClass == "H5T_ENUM":
+        if "base" not in typeItem:
             raise KeyError("Expected 'base' to be provided for enum type")
         base_json = typeItem["base"]
-        if 'class' not in base_json:
+        if "class" not in base_json:
             raise KeyError("Expected class field in base type")
-        if base_json['class'] != 'H5T_INTEGER':
+        if base_json["class"] != "H5T_INTEGER":
             msg = "Only integer base types can be used with enum type"
             raise TypeError(msg)
-        if 'mapping' not in typeItem:
+        if "mapping" not in typeItem:
             raise KeyError("'mapping' not provided for enum type")
         mapping = typeItem["mapping"]
         if len(mapping) == 0:
             raise KeyError("empty enum map")
 
         dt = createBaseDataType(base_json)
-        if dt.kind == 'i' and dt.name == 'int8' and len(mapping) == 2 and \
-                'TRUE' in mapping and 'FALSE' in mapping:
+        if all(
+            (
+                dt.kind == "i",
+                dt.name == "int8",
+                len(mapping) == 2,
+                "TRUE" in mapping,
+                "FALSE" in mapping,
+            )
+        ):
             # convert to numpy boolean type
             dtRet = np.dtype("bool")
         else:
             # not a boolean enum, use h5py special dtype
             dtRet = special_dtype(enum=(dt, mapping))
 
     else:
@@ -700,48 +716,48 @@
         dtName = getNumpyTypename(typeItem)
         dtRet = np.dtype(dtName)
         return dtRet  # return predefined type
 
     if type(typeItem) != dict:
         raise TypeError("invalid type")
 
-    if 'class' not in typeItem:
+    if "class" not in typeItem:
         raise KeyError("'class' not provided")
-    typeClass = typeItem['class']
+    typeClass = typeItem["class"]
 
-    if typeClass == 'H5T_COMPOUND':
-        if 'fields' not in typeItem:
+    if typeClass == "H5T_COMPOUND":
+        if "fields" not in typeItem:
             raise KeyError("'fields' not provided for compound type")
-        fields = typeItem['fields']
+        fields = typeItem["fields"]
         if type(fields) is not list:
             raise TypeError("Type Error: expected list type for 'fields'")
         if not fields:
             raise KeyError("no 'field' elements provided")
         subtypes = []
         for field in fields:
 
             if type(field) != dict:
                 raise TypeError("Expected dictionary type for field")
-            if 'name' not in field:
+            if "name" not in field:
                 raise KeyError("'name' missing from field")
-            if 'type' not in field:
+            if "type" not in field:
                 raise KeyError("'type' missing from field")
-            field_name = field['name']
+            field_name = field["name"]
             if not isinstance(field_name, str):
                 raise TypeError("field names must be strings")
             # verify the field name is ascii
             try:
-                field_name.encode('ascii')
+                field_name.encode("ascii")
             except UnicodeEncodeError:
                 raise TypeError("non-ascii field name not allowed")
 
-            dt = createDataType(field['type'])  # recursive call
+            dt = createDataType(field["type"])  # recursive call
             if dt is None:
                 raise Exception("unexpected error")
-            subtypes.append((field['name'], dt))  # append tuple
+            subtypes.append((field["name"], dt))  # append tuple
 
         dtRet = np.dtype(subtypes)
     else:
         dtRet = createBaseDataType(typeItem)  # create non-compound dt
     return dtRet
 
 
@@ -755,32 +771,33 @@
 
 
 def getBaseTypeJson(type_name):
     """
     Return JSON representation of a predefined type string
     """
     predefined_int_types = (
-          'H5T_STD_I8',
-          'H5T_STD_U8',
-          'H5T_STD_I16',
-          'H5T_STD_U16',
-          'H5T_STD_I32',
-          'H5T_STD_U32',
-          'H5T_STD_I64',
-          'H5T_STD_U64'
-    )
-    predefined_float_types = (
-          'H5T_IEEE_F16',
-          'H5T_IEEE_F32',
-          'H5T_IEEE_F64'
+        "H5T_STD_I8",
+        "H5T_STD_U8",
+        "H5T_STD_I16",
+        "H5T_STD_U16",
+        "H5T_STD_I32",
+        "H5T_STD_U32",
+        "H5T_STD_I64",
+        "H5T_STD_U64",
     )
+    predefined_float_types = ("H5T_IEEE_F16", "H5T_IEEE_F32", "H5T_IEEE_F64")
     type_json = {}
     # predefined typenames start with 'H5T' and end with "LE" or "BE"
-    if type_name.startswith("H5T_") and type_name[-1] == 'E' and \
-            type_name[-2] in ('L', 'B'):
+    if all(
+        (
+            type_name.startswith("H5T_"),
+            type_name[-1] == "E",
+            type_name[-2] in ("L", "B"),
+        )
+    ):
         # trime of the "BE/"LE"
         type_prefix = type_name[:-2]
         if type_prefix in predefined_int_types:
             type_json["class"] = "H5T_INTEGER"
             type_json["base"] = type_name
         elif type_prefix in predefined_float_types:
             type_json["class"] = "H5T_FLOAT"
```

### Comparing `hsds-0.7.0b11/hsds/util/idUtil.py` & `hsds-0.8.0/hsds/util/idUtil.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,194 +9,196 @@
 # distribution tree.  If you do not have access to this file, you may        #
 # request a copy from help@hdfgroup.org.                                     #
 ##############################################################################
 #
 # idUtil:
 # id (uuid) related functions
 #
+
 import os.path
 import hashlib
 import uuid
 from aiohttp.web_exceptions import HTTPServiceUnavailable
 from .. import hsds_logger as log
 
 
 def getIdHash(id):
-    """  Return md5 prefix based on id value"""
-    m = hashlib.new('md5')
-    m.update(id.encode('utf8'))
+    """Return md5 prefix based on id value"""
+    m = hashlib.new("md5")
+    m.update(id.encode("utf8"))
     hexdigest = m.hexdigest()
     return hexdigest[:5]
 
 
 def isSchema2Id(id):
-    """ return true if this is a v2 id """
+    """return true if this is a v2 id"""
     # v1 ids are in the standard UUID format: 8-4-4-4-12
     # v2 ids are in the non-standard: 8-8-4-6-6
-    parts = id.split('-')
+    parts = id.split("-")
     if len(parts) != 6:
         raise ValueError(f"Unexpected id formation for uuid: {id}")
     if len(parts[2]) == 8:
         return True
     else:
         return False
 
 
 def getIdHexChars(id):
-    """ get the hex chars of the given id """
-    if id[0] == 'c':
+    """get the hex chars of the given id"""
+    if id[0] == "c":
         # don't include chunk index
-        index = id.index('_')
-        parts = id[0:index].split('-')
+        index = id.index("_")
+        parts = id[0:index].split("-")
     else:
-        parts = id.split('-')
+        parts = id.split("-")
     if len(parts) != 6:
         raise ValueError(f"Unexpected id format for uuid: {id}")
     return "".join(parts[1:])
 
 
 def hexRot(ch):
-    """ rotate hex character by 8 """
-    return format((int(ch, base=16) + 8) % 16, 'x')
+    """rotate hex character by 8"""
+    return format((int(ch, base=16) + 8) % 16, "x")
 
 
 def isRootObjId(id):
-    """ returns true if this is a root id (only for v2 schema) """
+    """returns true if this is a root id (only for v2 schema)"""
     if not isSchema2Id(id):
         raise ValueError("isRootObjId can only be used with v2 ids")
     validateUuid(id)  # will throw ValueError exception if not a objid
-    if id[0] != 'g':
+    if id[0] != "g":
         return False  # not a group
     token = getIdHexChars(id)
     # root ids will have last 16 chars rotated version of the first 16
     is_root = True
     for i in range(16):
-        if token[i] != hexRot(token[i+16]):
+        if token[i] != hexRot(token[i + 16]):
             is_root = False
             break
     return is_root
 
 
 def getRootObjId(id):
-    """ returns root id for this objid if this is a root id
+    """returns root id for this objid if this is a root id
     (only for v2 schema)
     """
     if isRootObjId(id):
         return id  # this is the root id
     token = list(getIdHexChars(id))
     # root ids will have last 16 chars rotated version of the first 16
     for i in range(16):
-        token[i+16] = hexRot(token[i])
+        token[i + 16] = hexRot(token[i])
     token = "".join(token)
-    root_id = 'g-' + token[0:8] + '-' + token[8:16] + '-' + token[16:20]
-    root_id += '-' + token[20:26] + '-' + token[26:32]
+    root_id = "g-" + token[0:8] + "-" + token[8:16] + "-" + token[16:20]
+    root_id += "-" + token[20:26] + "-" + token[26:32]
 
     return root_id
 
 
 def createObjId(obj_type, rootid=None):
-    if obj_type not in ('groups', 'datasets', 'datatypes', 'chunks', "roots"):
+    if obj_type not in ("groups", "datasets", "datatypes", "chunks", "roots"):
         raise ValueError("unexpected obj_type")
 
     prefix = None
-    if obj_type == 'datatypes':
-        prefix = 't'  # don't collide with datasets
+    if obj_type == "datatypes":
+        prefix = "t"  # don't collide with datasets
     elif obj_type == "roots":
-        prefix = 'g'  # root obj is a group
+        prefix = "g"  # root obj is a group
     else:
         prefix = obj_type[0]
     if not rootid and obj_type != "roots":
         # v1 schema - folder
-        objid = prefix + '-' + str(uuid.uuid1())
+        objid = prefix + "-" + str(uuid.uuid1())
     elif rootid and not isSchema2Id(rootid):
         # v1 schema - domain
-        objid = prefix + '-' + str(uuid.uuid1())
+        objid = prefix + "-" + str(uuid.uuid1())
     else:
         # schema v2
         salt = uuid.uuid4().hex
         # take a hash to randomize the uuid
         token = list(hashlib.sha256(salt.encode()).hexdigest())
 
         if rootid:
             # replace first 16 chars of token with first 16 chars of rootid
             root_hex = getIdHexChars(rootid)
             token[0:16] = root_hex[0:16]
         else:
             # obj_type == "roots"
             # use only 16 chars, but make it look a 32 char id
             for i in range(16):
-                token[16+i] = hexRot(token[i])
+                token[16 + i] = hexRot(token[i])
         # format as a string
         token = "".join(token)
-        objid = prefix + '-' + token[0:8] + '-' + token[8:16] + '-'
-        objid += token[16:20] + '-' + token[20:26] + '-' + token[26:32]
+        objid = prefix + "-" + token[0:8] + "-" + token[8:16] + "-"
+        objid += token[16:20] + "-" + token[20:26] + "-" + token[26:32]
 
     return objid
 
 
 def getS3Key(id):
-    """ Return s3 key for given id.
+    """Return s3 key for given id.
 
     For schema v1:
         A md5 prefix is added to the front of the returned key to better
         distribute S3 objects.
     For schema v2:
         The id is converted to the pattern: "db/{rootid[0:16]}" for rootids and
         "db/id[0:16]/{prefix}/id[16-32]" for other ids
         Chunk ids have the chunk index added after the slash:
         "db/id[0:16]/d/id[16:32]/x_y_z
 
     For domain id's return a key with the .domain suffix and no
     preceeding slash
     """
-    if id.find('/') > 0:
+    if id.find("/") > 0:
         # a domain id
         domain_suffix = ".domain.json"
-        index = id.find('/') + 1
+        index = id.find("/") + 1
         key = id[index:]
         if not key.endswith(domain_suffix):
-            if key[-1] != '/':
-                key += '/'
+            if key[-1] != "/":
+                key += "/"
             key += domain_suffix
     else:
         if isSchema2Id(id):
             # schema v2 id
             hexid = getIdHexChars(id)
             prefix = id[0]  # one of g, d, t, c
-            if prefix not in ('g', 'd', 't', 'c'):
+            if prefix not in ("g", "d", "t", "c"):
                 raise ValueError(f"Unexpected id: {id}")
 
             if isRootObjId(id):
                 key = f"db/{hexid[0:8]}-{hexid[8:16]}"
             else:
                 partition = ""
-                if prefix == 'c':
+                if prefix == "c":
                     # use 'g' so that chunks will show up under their dataset
-                    s3col = 'd'
-                    n = id.find('-')
+                    s3col = "d"
+                    n = id.find("-")
                     if n > 1:
                         # extract the partition index if present
-                        partition = 'p' + id[1:n]
+                        partition = "p" + id[1:n]
                 else:
                     s3col = prefix
                 key = f"db/{hexid[0:8]}-{hexid[8:16]}/{s3col}/{hexid[16:20]}"
                 key += f"-{hexid[20:26]}-{hexid[26:32]}"
-            if prefix == 'c':
+            if prefix == "c":
                 if partition:
-                    key += '/'
+                    key += "/"
                     key += partition
                 # add the chunk coordinate
-                index = id.index('_')  # will raise ValueError if not found
-                coord = id[index+1:]
-                key += '/'
+                index = id.index("_")  # will raise ValueError if not found
+                n = index + 1
+                coord = id[n:]
+                key += "/"
                 key += coord
-            elif prefix == 'g':
+            elif prefix == "g":
                 # add key suffix for group
                 key += "/.group.json"
-            elif prefix == 'd':
+            elif prefix == "d":
                 # add key suffix for dataset
                 key += "/.dataset.json"
             else:
                 # add key suffix for datatype
                 key += "/.datatype.json"
         else:
             # v1 id
@@ -204,81 +206,88 @@
             idhash = getIdHash(id)
             key = f"{idhash}-{id}"
 
     return key
 
 
 def getObjId(s3key):
-    """ Return object id given valid s3key """
-    if len(s3key) >= 44 and s3key[0:5].isalnum() and s3key[5] == '-' and \
-            s3key[6] in ('g', 'd', 'c', 't'):
+    """Return object id given valid s3key"""
+    if all(
+        (
+            len(s3key) >= 44 and s3key[0:5].isalnum(),
+            len(s3key) >= 44 and s3key[5] == "-",
+            len(s3key) >= 44 and s3key[6] in ("g", "d", "c", "t"),
+        )
+    ):
         # v1 obj keys
         objid = s3key[6:]
     elif s3key.endswith("/.domain.json"):
-        objid = '/' + s3key[:-(len("/.domain.json"))]
+        objid = "/" + s3key[: -(len("/.domain.json"))]
     elif s3key.startswith("db/"):
         # schema v2 object key
-        parts = s3key.split('/')
+        parts = s3key.split("/")
         chunk_coord = ""  # used only for chunk ids
-        partition = ""    # likewise
+        partition = ""  # likewise
         token = []
         for ch in parts[1]:
-            if ch != '-':
+            if ch != "-":
                 token.append(ch)
 
         if len(parts) == 3:
             # root id
             # last part should be ".group.json"
             if parts[2] != ".group.json":
                 raise ValueError(f"unexpected S3Key: {s3key}")
             # add 16 more chars using rotated version of first 16
             for i in range(16):
                 token.append(hexRot(token[i]))
-            prefix = 'g'
+            prefix = "g"
         elif len(parts) == 5:
             # group, dataset, or datatype or chunk
             for ch in parts[3]:
-                if ch != '-':
+                if ch != "-":
                     token.append(ch)
 
-            if parts[2] == 'g' and parts[4] == ".group.json":
-                prefix = 'g'  # group json
-            elif parts[2] == 't' and parts[4] == ".datatype.json":
-                prefix = 't'  # datatype json
-            elif parts[2] == 'd':
+            if parts[2] == "g" and parts[4] == ".group.json":
+                prefix = "g"  # group json
+            elif parts[2] == "t" and parts[4] == ".datatype.json":
+                prefix = "t"  # datatype json
+            elif parts[2] == "d":
                 if parts[4] == ".dataset.json":
-                    prefix = 'd'  # dataset json
+                    prefix = "d"  # dataset json
                 else:
                     # chunk object
-                    prefix = 'c'
+                    prefix = "c"
                     chunk_coord = "_" + parts[4]
             else:
                 raise ValueError(f"unexpected S3Key: {s3key}")
         elif len(parts) == 6:
             # chunk key with partitioning
             for ch in parts[3]:
-                if ch != '-':
+                if ch != "-":
                     token.append(ch)
-            if parts[2][0] != 'd':
+            if parts[2][0] != "d":
                 raise ValueError(f"unexpected S3Key: {s3key}")
-            prefix = 'c'
+            prefix = "c"
             partition = parts[4]
-            if partition[0] != 'p':
+            if partition[0] != "p":
                 raise ValueError(f"unexpected S3Key: {s3key}")
             partition = partition[1:]  # strip off the p
             chunk_coord = "_" + parts[5]
         else:
             raise ValueError(f"unexpected S3Key: {s3key}")
 
         token = "".join(token)
-        objid = prefix + partition + '-' + token[0:8] + '-' + token[8:16]
-        objid += '-' + token[16:20] + '-' + token[20:26] + '-'
+        objid = prefix + partition + "-" + token[0:8] + "-" + token[8:16]
+        objid += "-" + token[16:20] + "-" + token[20:26] + "-"
         objid += token[26:32] + chunk_coord
     else:
-        raise ValueError(f"unexpected S3Key: {s3key}")
+        msg = f"unexpected S3Key: {s3key}"
+        log.warn(msg)
+        raise ValueError(msg)
     return objid
 
 
 def isS3ObjKey(s3key):
     valid = False
     try:
         objid = getObjId(s3key)
@@ -288,44 +297,47 @@
         pass  # ignore
     except ValueError:
         pass  # ignore
     return valid
 
 
 def createNodeId(prefix, node_number=None):
-    """ Create a random id used to identify nodes"""
+    """Create a random id used to identify nodes"""
     node_id = ""  # nothing too bad happens if this doesn't get set
     if node_number is not None:
         # just make an id based on the node_number
         hash_key = f"{node_number+1:03d}"
     else:
         # use the container id if we are running inside docker
         hash_key = getIdHash(str(uuid.uuid1()))
         proc_file = "/proc/self/cgroup"
         if os.path.isfile(proc_file):
             with open(proc_file) as f:
                 first_line = f.readline()
                 if first_line:
-                    fields = first_line.split(':')
+                    fields = first_line.split(":")
                     if len(fields) >= 3:
                         field = fields[2]
                         if field.startswith("/docker/"):
                             docker_len = len("/docker/")
+
                             if len(field) > docker_len + 12:
-                                node_id = field[docker_len:(docker_len+12)]
+                                n = docker_len
+                                m = n + 12
+                                node_id = field[n:m]
 
     if node_id:
         key = f"{prefix}-{node_id}-{hash_key}"
     else:
         key = f"{prefix}-{hash_key}"
     return key
 
 
 def getCollectionForId(obj_id):
-    """ return groups/datasets/datatypes based on id """
+    """return groups/datasets/datatypes based on id"""
     if not isinstance(obj_id, str):
         raise ValueError("invalid object id")
     collection = None
     if obj_id.startswith("g-"):
         collection = "groups"
     elif obj_id.startswith("d-"):
         collection = "datasets"
@@ -338,45 +350,46 @@
 
 def validateUuid(id, obj_class=None):
     if not isinstance(id, str):
         raise ValueError("Expected string type")
     if len(id) < 38:
         # id should be prefix (e.g. "g-") and uuid value
         raise ValueError("Unexpected id length")
-    if id[0] not in ('g', 'd', 't', 'c'):
+    if id[0] not in ("g", "d", "t", "c"):
         raise ValueError("Unexpected prefix")
-    if id[0] != 'c' and id[1] != '-':
+    if id[0] != "c" and id[1] != "-":
         # chunk ids may have a partition index following the c
         raise ValueError("Unexpected prefix")
     if obj_class is not None:
         obj_class = obj_class.lower()
         prefix = obj_class[0]
         if obj_class.startswith("datatype"):
-            prefix = 't'
+            prefix = "t"
         if id[0] != prefix:
-            raise ValueError("Unexpected prefix for class: " + obj_class)
-    if id[0] == 'c':
+            raise ValueError(f"Unexpected prefix for class: {obj_class}")
+    if id[0] == "c":
         # trim the type char and any partition id
-        n = id.find('-')
+        n = id.find("-")
         if n == -1:
             raise ValueError("Invalid chunk id")
 
         # trim the chunk index for chunk ids
-        m = id.find('_')
+        m = id.find("_")
         if m == -1:
             raise ValueError("Invalid chunk id")
-        id = "c-" + id[(n+1):m]
+        n += 1
+        id = "c-" + id[n:m]
     if len(id) != 38:
         # id should be 36 now
         raise ValueError("Unexpected id length")
 
     for ch in id:
         if ch.isalnum():
             continue
-        if ch == '-':
+        if ch == "-":
             continue
         raise ValueError(f"Unexpected character in uuid: {ch}")
 
 
 def isValidUuid(id, obj_class=None):
     try:
         validateUuid(id, obj_class)
@@ -384,76 +397,76 @@
     except ValueError:
         return False
 
 
 def isValidChunkId(id):
     if not isValidUuid(id):
         return False
-    if id[0] != 'c':
+    if id[0] != "c":
         return False
     return True
 
 
 def getClassForObjId(id):
-    """ return domains/chunks/groups/datasets/datatypes based on id """
+    """return domains/chunks/groups/datasets/datatypes based on id"""
     if not isinstance(id, str):
         raise ValueError("Expected string type")
     if len(id) == 0:
         raise ValueError("Empty string")
-    if id[0] == '/':
+    if id[0] == "/":
         return "domains"
     if isValidChunkId(id):
         return "chunks"
     else:
         return getCollectionForId(id)
 
 
 def isObjId(id):
-    """ return true if uuid or domain """
+    """return true if uuid or domain"""
     if not isinstance(id, str) or len(id) == 0:
         return False
-    if id.find('/') > 0:
+    if id.find("/") > 0:
         # domain id is any string in the form <bucket_name>/<domain_path>
         return True
     return isValidUuid(id)
 
 
 def getUuidFromId(id):
-    """ strip off the type prefix ('g-' or 'd-', or 't-')
-    and return the uuid part """
+    """strip off the type prefix ('g-' or 'd-', or 't-')
+    and return the uuid part"""
     return id[2:]
 
 
 def getObjPartition(id, count):
-    """ Get the id of the dn node that should be handling the given obj id
-    """
+    """Get the id of the dn node that should be handling the given obj id"""
     hash_code = getIdHash(id)
     hash_value = int(hash_code, 16)
     number = hash_value % count
     return number
 
 
 def getNodeNumber(app):
     if app["node_type"] == "sn":
         log.error("node number if only for DN nodes")
         raise ValueError()
 
     dn_ids = app["dn_ids"]
-    # log.debug(f"getNodeNumber(from dn_ids: {dn_ids}")
+    log.debug(f"getNodeNumber(from dn_ids: {dn_ids})")
     for i in range(len(dn_ids)):
         dn_id = dn_ids[i]
         if dn_id == app["id"]:
-            # log.debug(f"returning nodeNumber: {i}")
+            log.debug(f"returning nodeNumber: {i}")
             return i
     log.error("getNodeNumber, no matching id")
     return -1
 
 
 def getNodeCount(app):
     dn_urls = app["dn_urls"]
+    log.debug(f"getNodeCount for dn_urls: {dn_urls}")
     dn_node_count = len(dn_urls)
     return dn_node_count
 
 
 def validateInPartition(app, obj_id):
     node_number = getNodeNumber(app)
     node_count = getNodeCount(app)
@@ -466,15 +479,15 @@
         msg = f"wrong node for 'id':{obj_id}, expected node {node_number} "
         msg += f"got {partition_number}"
         log.error(msg)
         raise KeyError(msg)
 
 
 def getDataNodeUrl(app, obj_id):
-    """ Return host/port for datanode for given obj_id.
+    """Return host/port for datanode for given obj_id.
     Throw exception if service is not ready"""
     dn_urls = app["dn_urls"]
     dn_node_count = getNodeCount(app)
     node_state = app["node_state"]
     if node_state != "READY" or dn_node_count <= 0:
         msg = "Service not ready"
         log.warn(msg)
```

### Comparing `hsds-0.7.0b11/hsds/util/jwtUtil.py` & `hsds-0.8.0/hsds/util/jwtUtil.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,59 +20,59 @@
 from cryptography.x509 import load_pem_x509_certificate
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicNumbers
 
 from .. import hsds_logger as log
 from .. import config
 
-MSONLINE_OPENID_URL = \
+MSONLINE_OPENID_URL = (
     "https://login.microsoftonline.com/common/.well-known/openid-configuration"
-GOOGLE_OPENID_URL = \
-    "https://accounts.google.com/.well-known/openid-configuration"
+)
+GOOGLE_OPENID_URL = "https://accounts.google.com/.well-known/openid-configuration"
 
 
 def verifyBearerToken(app, token):
     # Contact OpenID provider to validate bearer token.
     # if valid, return username, exp, and roles
     username = None
-    provider = config.get('openid_provider')
+    provider = config.get("openid_provider")
 
     if not provider:
         log.warn("no OpenID provider configured")
         raise HTTPUnauthorized()
     # Resolve provider into an OpenID configuration.
     log.debug(f"Using OpenID provider: {provider}")
-    if provider.lower() == 'azure':
+    if provider.lower() == "azure":
         openid_url = MSONLINE_OPENID_URL
-    elif provider.lower() == 'google':
+    elif provider.lower() == "google":
         openid_url = GOOGLE_OPENID_URL
     else:
-        openid_url = config.get('openid_url')
+        openid_url = config.get("openid_url")
         if not openid_url:
             msg = f"OpenID provider: {provider} requires 'openid_url' "
             msg += "config to be set"
             log.warn(msg)
             raise HTTPUnauthorized()
 
-    audience = config.get('openid_audience')
-    claims = config.get('openid_claims').split(',')
+    audience = config.get("openid_audience")
+    claims = config.get("openid_claims").split(",")
 
     # Maintain Azure defaults for compatibility.
     if not audience:
-        audience = config.get('azure_resource_id')
+        audience = config.get("azure_resource_id")
 
     # If we still don't have a provider and audience, abort.
     if not openid_url or not audience or not claims:
-        log.warn('Bearer authorization, but no OpenID configuration.')
+        log.warn("Bearer authorization, but no OpenID configuration.")
         raise HTTPUnauthorized()
 
     log.debug(f"Bearer authorization, using provider: {provider}")
     log.debug(f"Bearer authorization, using audience: {audience}")
     log.debug(f"Bearer authorization, using claims: {claims}")
-    if provider not in ('azure', 'google'):
+    if provider not in ("azure", "google"):
         log.debug(f"Bearer authorization, using openid_url: {openid_url}")
 
     log.debug(f"token: {token}")
 
     try:
         token_header = jwt.get_unverified_header(token)
     except DecodeError as de:
@@ -103,43 +103,45 @@
         elif res.status_code == 403:
             raise HTTPForbidden()
         elif res.status_code == 503:
             raise HTTPServiceUnavailable()
         else:
             raise HTTPInternalServerError()
 
-    jwk_uri = res.json()['jwks_uri']
+    jwk_uri = res.json()["jwks_uri"]
 
     # TBD: cache responses by uri
     res = requests.get(jwk_uri)
     jwk_keys = res.json()
     x5c = None
     rsa = {}
     log.info("_verifyBearerToken")
 
     # Iterate JWK keys and extract matching x5c chain
-    for key in jwk_keys['keys']:
-        if key['kid'] == token_header['kid']:
-            if 'x5c' in key:
-                x5c = key['x5c']
-            elif 'e' in key and 'n' in key:
-                for field in ['e', 'n']:
+    for key in jwk_keys["keys"]:
+        if key["kid"] == token_header["kid"]:
+            if "x5c" in key:
+                x5c = key["x5c"]
+            elif "e" in key and "n" in key:
+                for field in ["e", "n"]:
                     val = key[field]
-                    val = val + '='*((4 - len(val) % 4) % 4)
-                    val = base64.urlsafe_b64decode(val.encode('utf-8'))
-                    rsa[field] = int.from_bytes(val, 'big')
+                    val = val + "=" * ((4 - len(val) % 4) % 4)
+                    val = base64.urlsafe_b64decode(val.encode("utf-8"))
+                    rsa[field] = int.from_bytes(val, "big")
 
     # Use the X5C chain to load a public key.
     if x5c:
         log.debug("using x5c public key")
-        cert = ''.join([
-            '-----BEGIN CERTIFICATE-----\n',
-            x5c[0],
-            '\n-----END CERTIFICATE-----\n',
-            ])
+        cert = "".join(
+            [
+                "-----BEGIN CERTIFICATE-----\n",
+                x5c[0],
+                "\n-----END CERTIFICATE-----\n",
+            ]
+        )
         x509 = load_pem_x509_certificate(cert.encode(), default_backend())
         public_key = x509.public_key()
         """
         public_key_bytes = public_key.public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.SubjectPublicKeyInfo)
         log.debug(f"got public key: {public_key_bytes.decode('utf-8')}")
@@ -157,15 +159,15 @@
 
     # log.debug(f"bearer token - public_key: {public_key}")
 
     try:
         jwt_decode = jwt.decode(
             token,
             public_key,
-            algorithms='RS256',
+            algorithms="RS256",
             audience=audience,
         )
     except InvalidAudienceError:
         log.warn(f"OpenID InvalidAudienceError with {audience}")
         raise HTTPUnauthorized()
     except InvalidSignatureError:
         log.warn("OpenID InvalidSignatureError")
```

### Comparing `hsds-0.7.0b11/hsds/util/k8sClient.py` & `hsds-0.8.0/hsds/util/k8sClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,102 +24,108 @@
 from .. import hsds_logger as log
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 APISERVER = "https://kubernetes.default.svc"
 SERVICEACCOUNT = "/var/run/secrets/kubernetes.io/serviceaccount"
 
+
 def _k8sGetNamespace():
-    """ Return namespace of current pod """
+    """Return namespace of current pod"""
     namespace = None
     try:
-        with open(SERVICEACCOUNT+"/namespace") as f:
+        with open(SERVICEACCOUNT + "/namespace") as f:
             s = f.read()
             if s:
                 namespace = s.strip()
     except FileNotFoundError:
         pass
-    
+
     if not namespace:
         log.error("Unable to read namespace - not running in Kubernetes?")
         raise ValueError("Kubernetes namespace could not be determined")
     log.debug(f"k8s namespace: [{namespace}]")
     return namespace
 
+
 def _k8sGetBearerToken():
-    """ Return kubernetes bearer token """
+    """Return kubernetes bearer token"""
     token = None
     try:
-        with open(SERVICEACCOUNT+"/token") as f:
+        with open(SERVICEACCOUNT + "/token") as f:
             s = f.read()
             if s:
                 token = s.strip()
     except FileNotFoundError:
         pass
-    
+
     if not token:
         log.error("Unable to read token - not running in Kubernetes?")
         raise ValueError("Could not get Kubernetes auth token")
 
     return "Bearer " + token
 
+
 def getIPKeys(metadata):
     KEY_PATH = ("fieldsV1", "f:status", "f:podIPs")
     pod_ips = []
     if not isinstance(metadata, dict):
         log.warn(f"getIPKeys - expected list but got: {type(metadata)}")
         return pod_ips
     if "managedFields" not in metadata:
         log.warn(f"getIPKeys - expected managedFields key but got: {metadata.keys()}")
         return pod_ips
     managedFields = metadata["managedFields"]
     if not isinstance(managedFields, list):
         log.warn(f"expected managedFields to be list but got: {type(managedFields)}")
         return pod_ips
-    #log.debug(f"mangagedFields - {len(managedFields)} items")
+    # log.debug(f"mangagedFields - {len(managedFields)} items")
     for item in managedFields:
         if not isinstance(item, dict):
             log.warn(f"ignoring item type {type(item)}: {item}")
             continue
         for key in KEY_PATH:
-            #log.debug(f"using key: {key}")
+            # log.debug(f"using key: {key}")
             if key not in item:
                 # key not found, move on to next managedField
-                msg = f"getIPKeys - looking for {key} key but not present"
-                log.debug(msg)
+                # msg = f"getIPKeys - looking for {key} key but not present"
+                # log.debug(msg)
                 break
             item = item[key]
-            #log.debug(f"got obj type: {type(item)}")
-            #log.debug(f"item: {item}")
+            # log.debug(f"got obj type: {type(item)}")
+            # log.debug(f"item: {item}")
             if not isinstance(item, dict):
                 log.warn("not a dict")
                 break
         # item should be a dict that looks like:
         # {'.': {}, 'k:{"ip":"192.168.17.20"}': {'.': {}, 'f:ip': {}}}
         # ip is burried in the key that starts with "k:"
         if not isinstance(item, dict):
             log.warn(f"expected podIPs to be dict but got: {type(item)}")
             continue
         for k in item:
-            #log.debug(f"got podIPs key: {k}")
+            # log.debug(f"got podIPs key: {k}")
             if k.startswith('k:{"ip":"'):
                 n = len('k:{"ip":"')
                 s = k[n:]
                 m = s.find('"')
                 if m < 0:
                     log.warn(f"unexpected key: {k}")
                     continue
                 ip = s[:m]
+                if ip.find("::") >= 0:
+                    log.debug(f"non-valid ip value: {ip}, skip")
+                    continue
                 log.debug(f"found pod ip: {ip}")
                 pod_ips.append(ip)
     log.debug(f"getIPKeys  done: returning {pod_ips}")
     return pod_ips
 
 
-def _k8sGetPodIPs(pod_json, k8s_app_label):
+def _k8sGetPodIPs(pod_json):
     if not isinstance(pod_json, dict):
         msg = f"_k8sGetPodIPs - unexpected type: {type(pod_json)}"
         log.error(msg)
         raise TypeError(msg)
     if "items" not in pod_json:
         msg = "_k98sGetPodIPS - no items key"
         log.error(msg)
@@ -129,52 +135,49 @@
 
     for item in items:
         if "metadata" not in item:
             msg = "_k8sGetPodIPs - expected to find metadata key"
             log.warn(msg)
             continue
         metadata = item["metadata"]
-        #log.debug(f"pod metadata: {metadata}")
-        if "labels" not in metadata:
-            msg = "_k8sGetPodIPs - expected to labels key in metadata"
-            log.warn(msg)
-            continue
-        labels = metadata["labels"]
-        if "app" not in labels:
-            msg = "_k8sGetPodIPs - no app label"
-            log.debug(msg)
-            continue
-        app_label = labels["app"]
-        if app_label != k8s_app_label:
-            msg = f"_k8sGetPodIPs - app_label: {app_label} not equal to: "
-            msg += f"{k8s_app_label}, skipping"
-            log.debug(msg)
+        # import json
+        # log.debug(f"pod metadata: {json.dumps(metadata)}")
+        if "name" not in metadata:
+            log.warn("_k8sGetPodIPs - metadata item with no name key")
+            continue
+        pod_name = metadata["name"]
+        log.debug(f"_k8sGetPodIPs - processing metadata for pod: {pod_name}")
+        if "deletionTimestamp" in metadata and metadata["deletionTimestamp"]:
+            log.info(f"_k8sGetPodIPs - pod {pod_name} is terminating, ignoring")
             continue
+        ip_keys = getIPKeys(metadata)
+        log.debug(f"_k8sGetPodIPs - pod {pod_name} adding ip keys: {ip_keys}")
         ipKeys.extend(getIPKeys(metadata))
     return ipKeys
 
 
-async def _k8sListPod():
-    """ Make http request to k8s to get info on all pods in 
-      the current namespace.  Return json dictionary """
+async def _k8sListPod(k8s_label_selector):
+    """Make http request to k8s to get info on all pods in
+    the current namespace.  Return json dictionary"""
     namespace = _k8sGetNamespace()
-    cafile = SERVICEACCOUNT+"/ca.crt"
+    cafile = SERVICEACCOUNT + "/ca.crt"
     ssl_ctx = ssl.create_default_context(cafile=cafile)
     token = _k8sGetBearerToken()
     headers = {"Authorization": token}
+    params = {"labelSelector": k8s_label_selector}
     conn = aiohttp.TCPConnector(ssl_context=ssl_ctx)
     pod_json = None
     # TBD - save session for re-use
 
     status_code = None
     url = f"{APISERVER}/api/v1/namespaces/{namespace}/pods"
     async with aiohttp.ClientSession(connector=conn) as session:
         # TBD: use read_bufsize parameter to optimize read for large responses
         try:
-            async with session.get(url, headers=headers) as rsp:
+            async with session.get(url, headers=headers, params=params) as rsp:
                 log.info(f"http_get status for k8s pods: {rsp.status} for req: {url}")
                 status_code = rsp.status
                 if rsp.status == 200:
                     # 200, so read the response
                     pod_json = await rsp.json()
                     # log.debug(f"got podlist resonse: {pod_json}")
                 elif status_code == 400:
@@ -199,19 +202,27 @@
         except CancelledError as cle:
             log.error(f"CancelledError for http_get({url}): {cle}")
             raise HTTPInternalServerError()
 
     return pod_json
 
 
-async def getPodIps(k8s_app_label):
-    log.debug(f"getPodIps({k8s_app_label})")
-    pod_json = await _k8sListPod()
-    pod_ips = _k8sGetPodIPs(pod_json, k8s_app_label)
+def getDnLabelSelector(config):
+    selector = config.get("k8s_dn_label_selector")
+    if selector:
+        return selector
+
+    # Fallback to old k8s_app_label config for backward compatibility:
+    app_label = config.get("k8s_app_label")
+    if app_label:
+        return f"app={app_label}"
+
+    return None
+
+
+async def getPodIps(k8s_label_selector):
+    log.debug(f"getPodIps({k8s_label_selector})")
+    pod_json = await _k8sListPod(k8s_label_selector)
+    pod_ips = _k8sGetPodIPs(pod_json)
     log.info(f"gotPodIps: {pod_ips}")
 
-    return pod_ips   
-    
- 
-    
-    
- 
+    return pod_ips
```

### Comparing `hsds-0.7.0b11/hsds/util/lruCache.py` & `hsds-0.8.0/hsds/util/lruCache.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,39 +12,38 @@
 import numpy
 import time
 
 from .. import hsds_logger as log
 
 
 def getArraySize(arr):
-    """ Return size in bytes of numpy array """
+    """Return size in bytes of numpy array"""
     nbytes = arr.dtype.itemsize
     for n in arr.shape:
         nbytes *= n
     return nbytes
 
 
 class Node(object):
-    def __init__(self, id, data,
-                 mem_size=1024, isdirty=False, prev=None, next=None):
+    def __init__(self, id, data, mem_size=1024, isdirty=False, prev=None, next=None):
         self._id = id
         self._data = data
         self._mem_size = mem_size
         self._isdirty = isdirty
         self._prev = prev
         self._next = next
         self._last_access = time.time()
 
 
 class LruCache(object):
-    """ LRU cache for Numpy arrays that are read/written from S3
-        If name is "ChunkCache", chunk items are assumed by be ndarrays
+    """LRU cache for Numpy arrays that are read/written from S3
+    If name is "ChunkCache", chunk items are assumed by be ndarrays
     """
-    def __init__(self, mem_target=32*1024*1024,
-                 name="LruCache", expire_time=None):
+
+    def __init__(self, mem_target=32 * 1024 * 1024, name="LruCache", expire_time=None):
         self._hash = {}
         self._lru_head = None
         self._lru_tail = None
         self._mem_size = 0
         self._dirty_size = 0
         self._mem_target = mem_target
         self._expire_time = expire_time
@@ -96,15 +95,15 @@
             if self._lru_tail != node:
                 raise KeyError("unexpected error")
             self._lru_tail = prev
         self._lru_head = node
         return node
 
     def _hasKey(self, key, ignore_expire=False):
-        """ check if key is present node  """
+        """check if key is present node"""
         if key not in self._hash:
             return False
         if ignore_expire:
             return True
         node = self._hash[key]
         now = time.time()
         if self._expire_time:
@@ -117,40 +116,42 @@
             else:
                 return True
         else:
             return True
 
     def __delitem__(self, key):
         node = self._delNode(key)  # remove from LRU
-        del self._hash[key]        # remove from hash
+        del self._hash[key]  # remove from hash
         # remove from LRU list
 
         self._mem_size -= node._mem_size
         if key in self._dirty_set:
             log.warning(f"LRU {self._name} removing dirty node: {key}")
             self._dirty_set.remove(key)
             self._dirty_size -= node._mem_size
+            if self._dirty_size < 0:
+                self._dirty_size = 0
 
     def __len__(self):
-        """ Number of nodes in the cache """
+        """Number of nodes in the cache"""
         return len(self._hash)
 
     def __iter__(self):
-        """ Iterate over node ids """
+        """Iterate over node ids"""
         node = self._lru_head
         while node is not None:
             yield node._id
             node = node._next
 
     def __contains__(self, key):
-        """ Test if key is in the cache """
+        """Test if key is in the cache"""
         return self._hasKey(key)
 
     def __getitem__(self, key):
-        """ Return numpy array from cache """
+        """Return numpy array from cache"""
         # doing a getitem has the side effect of moving this node
         # up in the LRU list
         if not self._hasKey(key):
             raise KeyError(key)
         node = self._moveToFront(key)
         return node._data
 
@@ -177,16 +178,17 @@
             self._mem_size += mem_delta
             node._data = data
             node._mem_size = mem_size
             self._moveToFront(key)
             if node._isdirty:
                 self._dirty_size += mem_delta
             node._last_access = time.time()
-            msg = f"LRU {self._name} updated node: {key} "
-            msg += f"[was {old_size} bytes now {node._mem_size} bytes]"
+            msg = f"LRU {self._name} updated node: {key}, "
+            msg += f"was {old_size} bytes now {node._mem_size} bytes, "
+            msg += f"dirty_size: {self._dirty_size}"
             log.debug(msg)
         else:
             node = Node(key, data, mem_size=mem_size)
             if self._lru_head is None:
                 self._lru_head = self._lru_tail = node
             else:
                 # newer items go to the front
@@ -199,15 +201,15 @@
             self._hash[key] = node
             self._mem_size += node._mem_size
             msg = f"LRU {self._name} adding {node._mem_size} to cache, "
             msg += f"mem_size is now: {self._mem_size}"
             log.debug(msg)
             if node._isdirty:
                 self._dirty_size += node._mem_size
-                msg = f"LRU {self._name} dirty size is now: {self._dirty_size}"
+                msg = f"LRU {self._name} dirty_size is now: {self._dirty_size}"
                 log.debug(msg)
 
             msg = f"LRU {self._name} added new node: {key} "
             msg += f"[{node._mem_size} bytes]"
             log.debug(msg)
 
         if self._mem_size > self._mem_target:
@@ -255,18 +257,19 @@
                 msg = f"LRU {self._name} found dirty node during clear: "
                 msg += f"{node._id}"
                 log.error(msg)
                 raise ValueError("Unable to clear cache")
             log.debug(f"LRU {self._name} removing node: {node._id}")
             self.__delitem__(node._id)
             node = next_node
+        self._dirty_size = 0
         # done clearCache
 
     def consistencyCheck(self):
-        """ verify that the data structure is self-consistent """
+        """verify that the data structure is self-consistent"""
         id_list = []
         dirty_count = 0
         mem_usage = 0
         dirty_usage = 0
         # walk the LRU list
         node = self._lru_head
         node_type = None
@@ -312,51 +315,53 @@
             node = node._prev
         if reverse_count != len(id_list):
             msg = "elements in reverse list do not equal forward list"
             raise ValueError(msg)
         # done - consistencyCheck
 
     def setDirty(self, key):
-        """ setting dirty flag has the side effect of moving this node
-        up in the LRU list """
+        """setting dirty flag has the side effect of moving this node
+        up in the LRU list"""
         log.debug(f"LRU {self._name} set dirty node id: {key}")
 
         node = self._moveToFront(key)
         if not node._isdirty:
             self._dirty_size += node._mem_size
+            log.debug(f"LRU {self._name} - update dirty_size to: {self._dirty_size}")
         node._isdirty = True
 
         self._dirty_set.add(key)
 
     def clearDirty(self, key):
-        """ clear the dirty flag """
+        """clear the dirty flag"""
         # clearing dirty flag has the side effect of moving this node
         # up in the LRU list
         # also, may trigger a memory cleanup
 
         log.debug(f"LRU {self._name} clear dirty node: {key}")
         node = self._moveToFront(key)
         if node._isdirty:
             self._dirty_size -= node._mem_size
+        log.debug(f"LRU {self._name} dirty_size: {self._dirty_size}")
         node._isdirty = False
 
         if key in self._dirty_set:
             self._dirty_set.remove(key)
             if self._mem_size > self._mem_target:
                 # maybe we can free up some memory now
                 self._reduceCache()
 
     def isDirty(self, key):
-        """ return dirty flag """
+        """return dirty flag"""
         # don't adjust LRU position
         return key in self._dirty_set
 
     def dump_lru(self):
-        """ Return LRU list as a string
-            (for debugging)
+        """Return LRU list as a string
+        (for debugging)
         """
         node = self._lru_head
         s = "->"
         while node:
             s += node._id
             node = node._next
             if node:
@@ -369,24 +374,31 @@
             if node:
                 s += ","
         s += "\n"
         return s
 
     @property
     def cacheUtilizationPercent(self):
-        return int((self._mem_size/self._mem_target)*100.0)
+        return int((self._mem_size / self._mem_target) * 100.0)
 
     @property
     def dirtyCount(self):
         return len(self._dirty_set)
 
     @property
     def memUsed(self):
         return self._mem_size
 
     @property
+    def memFree(self):
+        memFree = self._mem_target - self._dirty_size
+        if memFree < 0:
+            memFree = 0
+        return memFree
+
+    @property
     def memTarget(self):
         return self._mem_target
 
     @property
     def memDirty(self):
         return self._dirty_size
```

### Comparing `hsds-0.7.0b11/hsds/util/query_marathon.py` & `hsds-0.8.0/hsds/util/query_marathon.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 # This is a utility to interrogate a Marathon HSDS configuration
 # See http://mesosphere.github.io/marathon/api-console/index.html
 
 
 class MarathonClient:
     """
-     Utility class for access the parts of DCOS Marathon configurations we
-     need to coordinate the HSDS nodes
+    Utility class for access the parts of DCOS Marathon configurations we
+    need to coordinate the HSDS nodes
     """
 
     def __init__(self, app):
         if "session" not in app:
             session = get_session()
             app["session"] = session
```

### Comparing `hsds-0.7.0b11/hsds/util/s3Client.py` & `hsds-0.8.0/hsds/util/s3Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 import subprocess
 import datetime
 import json
 import time
 from aiobotocore.config import AioConfig
 from aiobotocore.session import get_session
 from botocore.exceptions import ClientError
+from botocore import UNSIGNED
 from aiohttp.web_exceptions import HTTPNotFound, HTTPInternalServerError
 from aiohttp.web_exceptions import HTTPForbidden, HTTPBadRequest
 from .. import hsds_logger as log
 from .. import config
 
 
-class S3Client():
+class S3Client:
     """
-     Utility class for reading and storing data to AWS S3
+    Utility class for reading and storing data to AWS S3
     """
 
     def __init__(self, app):
         if "session" not in app:
             session = get_session()
             app["session"] = session
         else:
@@ -60,14 +61,16 @@
         self._aws_iam_role = None
         self._aws_secret_access_key = None
         self._aws_access_key_id = None
         max_pool_connections = 64
         self._aws_session_token = None
         self._aws_role_arn = None
         self._aws_session_token = None
+        self._aws_no_sign_request = False
+        signature_version = None
 
         try:
             self._aws_iam_role = config.get("aws_iam_role")
         except KeyError:
             pass
 
         try:
@@ -79,51 +82,58 @@
         except KeyError:
             pass
         try:
             self._aws_region = config.get("aws_region")
         except KeyError:
             pass
         try:
-            max_pool_connections = config.get('aio_max_pool_connections')
+            max_pool_connections = config.get("aio_max_pool_connections")
         except KeyError:
             pass
         self._aws_role_arn = None
         if "AWS_ROLE_ARN" in os.environ:
             # Assume IAM roles for EKS is being used.  See:
             # https://aws.amazon.com/blogs/opensource/\
             # introducing-fine-grained-iam-roles-service-accounts/
-            self._aws_role_arn = os.environ['AWS_ROLE_ARN']
+            self._aws_role_arn = os.environ["AWS_ROLE_ARN"]
             log.info(f"AWS_ROLE_ARN set to: {self._aws_role_arn}")
             if "AWS_WEB_IDENTITY_TOKEN_FILE" in os.environ:
-                token_file = os.environ['AWS_WEB_IDENTITY_TOKEN_FILE']
+                token_file = os.environ["AWS_WEB_IDENTITY_TOKEN_FILE"]
                 log.debug(f"AWS_WEB_IDENTITY_TOKEN_FILE is: {token_file}")
         if "AWS_SESSION_TOKEN" in os.environ:
-            self._aws_session_token = os.environ['AWS_SESSION_TOKEN']
+            self._aws_session_token = os.environ["AWS_SESSION_TOKEN"]
             log.debug(f"got AWS_SESSION_TOKEN: {self._aws_session_token}")
 
-        self._aio_config = AioConfig(max_pool_connections=max_pool_connections)
+        try:
+            self._aws_no_sign_request = config.get("aws_s3_no_sign_request", False)
+            if self._aws_no_sign_request:
+                signature_version = UNSIGNED
+        except KeyError:
+            pass
+
+        self._aio_config = AioConfig(max_pool_connections=max_pool_connections,
+                                     signature_version=signature_version)
 
         log.debug(f"S3Client init - aws_region {self._aws_region}")
 
-        self._s3_gateway = config.get('aws_s3_gateway')
+        self._s3_gateway = config.get("aws_s3_gateway")
         if not self._s3_gateway:
             msg = "Invalid aws s3 gateway"
             log.error(msg)
             raise ValueError(msg)
         log.debug(f"Using S3Gateway: {self._s3_gateway}")
 
         self._use_ssl = False
         if self._s3_gateway.startswith("https"):
             self._use_ssl = True
 
-        if not self._aws_secret_access_key or \
-                self._aws_secret_access_key == 'xxx':
+        if not self._aws_secret_access_key or self._aws_secret_access_key == "xxx":
             log.debug("aws secret access key not set")
             self._aws_secret_access_key = None
-        if not self._aws_access_key_id or self._aws_access_key_id == 'xxx':
+        if not self._aws_access_key_id or self._aws_access_key_id == "xxx":
             log.debug("aws access key id not set")
             self._aws_access_key_id = None
         else:
             log.debug(f"using aws key id: {self._aws_access_key_id}")
         self._renewToken()
 
     def _get_client_kwargs(self):
@@ -134,19 +144,23 @@
         kwargs["aws_session_token"] = self._aws_session_token
         kwargs["endpoint_url"] = self._s3_gateway
         kwargs["use_ssl"] = self._use_ssl
         kwargs["config"] = self._aio_config
         return kwargs
 
     def _renewToken(self):
-        """ if using an aws_iam_role, fetch credentials if our token is about
-          to expire, otherwise just return
+        """if using an aws_iam_role, fetch credentials if our token is about
+        to expire, otherwise just return
         """
         app = self._app
 
+        if self._aws_no_sign_request:
+            # no need to get a token
+            return
+
         if not self._aws_iam_role:
             # need this to get a token
             return
         if self._aws_role_arn:
             # this is set for running in EKS, shouldn't need a token
             return
 
@@ -174,15 +188,15 @@
             msg = f"get S3 access token using iam role: {self._aws_iam_role}"
             log.info(msg)
             # Use EC2 IAM role to get credentials
             # See: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/\
             # iam-roles-for-amazon-ec2.html?icmpid=docs_ec2_console
             url = "http://169.254.169.254/latest/meta-data/iam/"
             url += f"security-credentials/{self._aws_iam_role}"
-            curl_cmd = ["curl", url]
+            curl_cmd = ["curl", "--no-progress-meter", url]
             kwargs = {"stdout": subprocess.PIPE, "stderr": subprocess.PIPE}
             p = subprocess.run(curl_cmd, **kwargs)
             if p.returncode != 0:
                 msg = f"Error getting IAM role credentials: {p.stderr}"
                 log.error(msg)
             else:
                 stdout = p.stdout.decode("utf-8")
@@ -207,76 +221,88 @@
                     log.error(msg)
                 except KeyError:
                     msg = "Missing expected key from EC2 meta-data "
                     msg += f"response: {stdout}"
                     log.error(msg)
 
     def _s3_stats_increment(self, counter, inc=1):
-        """ Incremenet the indicated connter
-        """
+        """Incremenet the indicated connter"""
         if "s3_stats" not in self._app:
             # setup stats
             s3_stats = {}
             s3_stats["get_count"] = 0
             s3_stats["put_count"] = 0
             s3_stats["delete_count"] = 0
             s3_stats["list_count"] = 0
             s3_stats["error_count"] = 0
             s3_stats["bytes_in"] = 0
             s3_stats["bytes_out"] = 0
             self._app["s3_stats"] = s3_stats
-        s3_stats = self._app['s3_stats']
+        s3_stats = self._app["s3_stats"]
         if counter not in s3_stats:
             log.error(f"unexpected counter for s3_stats: {counter}")
             return
         if inc < 1:
             log.error(f"unexpected inc for s3_stats: {inc}")
             return
 
         s3_stats[counter] += inc
 
+    def getURIFromKey(self, key, bucket=None):
+        """ return S3 specific URI for given key and bucket """
+        if not bucket:
+            log.error("getURIFromKey, bucket not set")
+            raise HTTPInternalServerError()
+        if not key:
+            log.error("getURIFromKey, key not set")
+            raise HTTPInternalServerError()
+        if key[0] == "/":
+            key = key[1:]
+
+        uri = f"s3://{bucket}/{key}"
+        return uri
+
     async def get_object(self, key, bucket=None, offset=0, length=-1):
-        """ Return data for object at given key.
-           If Range is set, return the given byte range.
+        """Return data for object at given key.
+        If Range is set, return the given byte range.
         """
 
         range = ""
         if length > 0:
             range = f"bytes={offset}-{offset+length-1}"
             log.info(f"storage range request: {range}")
 
         if not bucket:
             log.error("get_object - bucket not set")
             raise HTTPInternalServerError()
-        log.debug(f"bucket: {bucket} type: {type(bucket)}")
 
         start_time = time.time()
         log.debug(f"s3Client.get_object({bucket}/{key}) start: {start_time}")
         session = self._app["session"]
         self._renewToken()
         kwargs = self._get_client_kwargs()
-        async with session.create_client('s3', **kwargs) as _client:
+        async with session.create_client("s3", **kwargs) as _client:
             try:
                 kwargs = {"Bucket": bucket, "Key": key}
                 if range:
                     kwargs["Range"] = range
                 resp = await _client.get_object(**kwargs)
-                data = await resp['Body'].read()
+                data = await resp["Body"].read()
                 finish_time = time.time()
                 if offset > 0:
                     range_key = f"{key}[{offset}:{offset+length}]"
                 else:
                     range_key = key
                 msg = f"s3Client.get_object({range_key} bucket={bucket}) "
                 msg += f"start={start_time:.4f} finish={finish_time:.4f} "
                 msg += f"elapsed={finish_time-start_time:.4f} "
                 msg += f"bytes={len(data)}"
                 log.info(msg)
 
-                resp['Body'].close()
+                resp["Body"].close()
             except ClientError as ce:
                 # key does not exist?
                 # check for not found status
                 response_code = ce.response["Error"]["Code"]
                 if response_code in ("NoSuchKey", "404", 404):
                     msg = f"s3_key: {bucket}/{key} not found "
                     log.info(msg)
@@ -304,39 +330,41 @@
                 self._s3_stats_increment("error_count")
                 msg = f"Unexpected Exception {type(e)} get s3 obj {bucket}/{key}: {e}"
                 log.error(msg)
                 raise HTTPInternalServerError()
         return data
 
     async def put_object(self, key, data, bucket=None):
-        """ Write data to given key.
-            Returns client specific dict on success
+        """Write data to given key.
+        Returns client specific dict on success
         """
         if not bucket:
             log.error("put_object - bucket not set")
             raise HTTPInternalServerError()
 
         start_time = time.time()
         log.debug(f"s3Client.put_object({bucket}/{key} start: {start_time}")
         session = self._app["session"]
         self._renewToken()
         kwargs = self._get_client_kwargs()
-        async with session.create_client('s3', **kwargs) as _client:
+        async with session.create_client("s3", **kwargs) as _client:
             try:
                 kwargs = {"Bucket": bucket, "Key": key, "Body": data}
                 rsp = await _client.put_object(**kwargs)
                 finish_time = time.time()
                 msg = f"s3Client.put_object({key} bucket={bucket}) "
                 msg += f"start={start_time:.4f} finish={finish_time:.4f} "
                 msg += f"elapsed={finish_time-start_time:.4f} "
                 msg += f"bytes={len(data)}"
                 log.info(msg)
-                s3_rsp = {"etag": rsp["ETag"],
-                          "size": len(data),
-                          "lastModified": int(finish_time)}
+                s3_rsp = {
+                    "etag": rsp["ETag"],
+                    "size": len(data),
+                    "lastModified": int(finish_time),
+                }
             except ClientError as ce:
                 response_code = ce.response["Error"]["Code"]
                 if response_code == "NoSuchBucket":
                     msg = f"s3_bucket: {bucket} not found"
                     log.warn(msg)
                     raise HTTPNotFound()
                 else:
@@ -357,26 +385,25 @@
                 raise HTTPInternalServerError()
         if data and len(data) > 0:
             self._s3_stats_increment("bytes_out", inc=len(data))
         log.debug(f"s3Client.put_object {key} complete, s3_rsp: {s3_rsp}")
         return s3_rsp
 
     async def delete_object(self, key, bucket=None):
-        """ Deletes the object at the given key
-        """
+        """Deletes the object at the given key"""
         if not bucket:
             log.error("delete_object - bucket not set")
             raise HTTPInternalServerError()
 
         start_time = time.time()
         log.debug(f"s3Client.delete_object({bucket}/{key} start: {start_time}")
         session = self._app["session"]
         self._renewToken()
         kwargs = self._get_client_kwargs()
-        async with session.create_client('s3', **kwargs) as _client:
+        async with session.create_client("s3", **kwargs) as _client:
             try:
                 await _client.delete_object(Bucket=bucket, Key=key)
                 finish_time = time.time()
                 msg = f"s3Client.delete_object({key} bucket={bucket}) "
                 msg += f"start={start_time:.4f} finish={finish_time:.4f} "
                 msg += f"elapsed={finish_time-start_time:.4f}"
                 log.info(msg)
@@ -401,25 +428,24 @@
                 self._s3_stats_increment("error_count")
                 msg = f"Unexpected Exception {type(e)} deleting s3 obj "
                 msg += f"{key}: {e}"
                 log.error(msg)
                 raise HTTPInternalServerError()
 
     async def is_object(self, key, bucket=None):
-        """ Return true if the given object exists
-        """
+        """Return true if the given object exists"""
         if not bucket:
             log.error("is_object - bucket not set")
             raise HTTPInternalServerError()
         start_time = time.time()
         found = False
         session = self._app["session"]
         self._renewToken()
         kwargs = self._get_client_kwargs()
-        async with session.create_client('s3', **kwargs) as _client:
+        async with session.create_client("s3", **kwargs) as _client:
             try:
                 head_data = await _client.head_object(Bucket=bucket, Key=key)
                 finish_time = time.time()
                 found = True
                 log.info(f"head: {head_data}")
             except ClientError:
                 # key does not exist?
@@ -441,21 +467,20 @@
         msg += f"start={start_time:.4f} finish={finish_time:.4f} "
         msg += f"elapsed={finish_time-start_time:.4f}"
         log.info(msg)
 
         return found
 
     async def get_key_stats(self, key, bucket=None):
-        """ Get ETag, size, and last modified time for given object
-        """
+        """Get ETag, size, and last modified time for given object"""
         start_time = time.time()
         session = self._app["session"]
         self._renewToken()
         kwargs = self._get_client_kwargs()
-        async with session.create_client('s3', **kwargs) as _client:
+        async with session.create_client("s3", **kwargs) as _client:
             try:
                 head_data = await _client.head_object(Bucket=bucket, Key=key)
                 finish_time = time.time()
                 log.info(f"head: {head_data}")
             except ClientError:
                 # key does not exist?
                 msg = f"s3Client.get_key_stats: Key: {key} not found"
@@ -485,42 +510,42 @@
         last_modified_dt = head_data["LastModified"]
         if not isinstance(last_modified_dt, datetime.datetime):
             msg = "S3Client.get_key_stats, expected datetime object "
             msg += "in head data"
             log.error(msg)
             raise HTTPInternalServerError()
         key_stats = {}
-        key_stats["Size"] = head_data['ContentLength']
+        key_stats["Size"] = head_data["ContentLength"]
         key_stats["ETag"] = head_data["ETag"]
         LastModified = datetime.datetime.timestamp(last_modified_dt)
         key_stats["LastModified"] = LastModified
         msg = f"s3Client.get_key_stats({key} bucket={bucket}) "
         msg += f"start={start_time:.4f} finish={finish_time:.4f} "
         msg += f"elapsed={finish_time-start_time:.4f}"
         log.info(msg)
 
         return key_stats
 
     def _getPageItems(self, response, items, include_stats=False):
-        """ internl method for list pagination """
+        """internl method for list pagination"""
         log.info("getPageItems")
 
-        if 'CommonPrefixes' in response:
+        if "CommonPrefixes" in response:
             log.debug("got CommonPrefixes in s3 response")
             common = response["CommonPrefixes"]
             for item in common:
-                if 'Prefix' in item:
+                if "Prefix" in item:
                     log.debug(f"got s3 prefix: {item['Prefix']}")
                     items.append(item["Prefix"])
 
-        elif 'Contents' in response:
+        elif "Contents" in response:
             log.debug("got Contents in s3 response")
-            contents = response['Contents']
+            contents = response["Contents"]
             for item in contents:
-                key_name = item['Key']
+                key_name = item["Key"]
                 if include_stats:
                     stats = {}
                     if item["ETag"]:
                         stats["ETag"] = item["ETag"]
                     else:
                         log.warn(f"No ETag for key: {key_name}")
                     if "Size" in item:
@@ -533,44 +558,53 @@
                     else:
                         log.warn(f"No LastModified for key: {key_name}")
                     log.debug(f"key: {key_name} stats: {stats}")
                     items[key_name] = stats
                 else:
                     items.append(key_name)
 
-    async def list_keys(self, prefix='', deliminator='', suffix='',
-                        include_stats=False, callback=None, bucket=None,
-                        limit=None):
-        """ return keys matching the arguments
-        """
+    async def list_keys(
+        self,
+        prefix="",
+        deliminator="",
+        suffix="",
+        include_stats=False,
+        callback=None,
+        bucket=None,
+        limit=None,
+    ):
+        """return keys matching the arguments"""
         if not bucket:
             log.error("list_keys - bucket not set")
             raise HTTPInternalServerError()
         msg = f"list_keys('{prefix}','{deliminator}','{suffix}', "
         msg += f"include_stats={include_stats}, "
         msg += f"callback {'set' if callback is not None else 'not set'}"
         log.info(msg)
-        if deliminator and deliminator != '/':
+        if deliminator and deliminator != "/":
             msg = "Only '/' is supported as deliminator"
             log.warn(msg)
             raise HTTPBadRequest(reason=msg)
         session = self._app["session"]
         self._renewToken()
         kwargs = self._get_client_kwargs()
-        async with session.create_client('s3', **kwargs) as _client:
-            paginator = _client.get_paginator('list_objects')
+        async with session.create_client("s3", **kwargs) as _client:
+            paginator = _client.get_paginator("list_objects")
 
             # use a dictionary to hold return values if stats are needed
             key_names = {} if include_stats else []
             count = 0
 
             try:
                 async for page in paginator.paginate(
-                         PaginationConfig={'PageSize': 1000}, Bucket=bucket,
-                         Prefix=prefix, Delimiter=deliminator):
+                    PaginationConfig={"PageSize": 1000},
+                    Bucket=bucket,
+                    Prefix=prefix,
+                    Delimiter=deliminator,
+                ):
                     assert not asyncio.iscoroutine(page)
                     kwargs = {"include_stats": include_stats}
                     self._getPageItems(page, key_names, **kwargs)
                     count += len(key_names)
                     if callback:
                         if iscoroutinefunction(callback):
                             await callback(self._app, key_names)
@@ -592,12 +626,12 @@
             msg = f"expected {count} keys in return list "
             msg += f"but got {len(key_names)}"
             log.warning(msg)
 
         return key_names
 
     async def releaseClient(self):
-        """ release the client collection to s3
-           (Used for cleanup on application exit)
+        """release the client collection to s3
+        (Used for cleanup on application exit)
         """
         log.info("release S3Client")
         await asyncio.sleep(0)  # nothing to do
```

### Comparing `hsds-0.7.0b11/hsds/util/storUtil.py` & `hsds-0.8.0/hsds/util/storUtil.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,61 +22,71 @@
 from aiohttp.client_exceptions import ClientError
 from asyncio import CancelledError
 
 
 from .. import hsds_logger as log
 from .httpUtil import http_get
 from .s3Client import S3Client
+
 try:
     from .azureBlobClient import AzureBlobClient
 except ImportError:
+
     def AzureBlobClient(app):
         log.error("Unable to import AzureBlobClient")
         return None
+
+
 try:
     from .fileClient import FileClient
 except ImportError:
+
     def FileClient(app):
         log.error("ImportError for FileClient")
         return None
+
+
 from .. import config
 
 
 def getCompressors():
-    """ return available compressors """
+    """return available compressors"""
     compressors = codecs.blosc.list_compressors()
     # replace zlib with the equivalent gzip since that is the h5py name
     if "gzip" not in compressors and "zlib" in compressors:
         for i in range(len(compressors)):
             if compressors[i] == "zlib":
                 compressors[i] = "gzip"
                 break
 
     # add deflate as a synonym for gzip
     if "gzip" in compressors:
         compressors.append("deflate")
 
     return compressors
 
+
 def getFilters(include_compressors=True):
-    """ return list of other supported filters """
-    filters = ["shuffle",]
+    """return list of other supported filters"""
+    filters = [
+        "shuffle",
+    ]
     if include_compressors:
         filters.extend(getCompressors())
     return filters
 
 
 def setBloscThreads(nthreads):
-    """ Set the number of threads blosc will use for compression """
+    """Set the number of threads blosc will use for compression"""
     codecs.blosc.set_nthreads(nthreads)
 
 
 def getBloscThreads():
-    """ Get the number of blosc threads to be used for compression """
-    nthreads = codecs.blosc_get_nthreads()
+    """Get the number of blosc threads to be used for compression"""
+    nthreads = codecs.blosc.get_nthreads()
 
     return nthreads
 
 
 def _shuffle(element_size, chunk):
     shuffler = codecs.Shuffle(element_size)
     arr = shuffler.encode(chunk)
@@ -86,16 +96,15 @@
 def _unshuffle(element_size, chunk):
     shuffler = codecs.Shuffle(element_size)
     arr = shuffler.decode(chunk)
     return arr.tobytes()
 
 
 def _getStorageClient(app):
-    """ get storage client s3 or azure blob
-    """
+    """get storage client s3 or azure blob"""
 
     if "storage_client" in app:
         return app["storage_client"]
 
     if config.get("aws_s3_gateway"):
         log.debug("_getStorageClient getting S3Client")
         client = S3Client(app)
@@ -107,81 +116,93 @@
         client = FileClient(app)
     # save client so we don't neeed to recreate each time
     app["storage_client"] = client
     return client
 
 
 def getStorageDriverName(app):
-    """ Return name of storage driver that is being used
-    """
+    """Return name of storage driver that is being used"""
     if config.get("aws_s3_gateway"):
         driver = "S3Client"
     elif config.get("azure_connection_string"):
         driver = "AzureBlobClient"
     else:
         driver = "FileClient"
     return driver
 
 
 async def releaseStorageClient(app):
-    """ release the client storage connection
-     (Used for cleanup on application exit)
+    """release the client storage connection
+    (Used for cleanup on application exit)
     """
     client = _getStorageClient(app)
     await client.releaseClient()
 
     if "storage_client" in app:
         del app["storage_client"]
 
+
 def _getURIParts(uri):
-    """ return tuple of (bucket, path) for given URI """
+    """return tuple of (bucket, path) for given URI"""
     if uri.startswith("s3://"):
         uri = uri[5:]
-    if uri.startswith('/'):
+    if uri.startswith("/"):
         raise ValueError("invalid uri")
-    n = uri.find('/')
+    n = uri.find("/")
     if n < 0:
         raise ValueError("invalid uri")
     fields = (uri[:n], uri[n:])
     return fields
 
+
 def getBucketFromStorURI(uri):
-    """ Return a bucket name given a storage URI 
-        Examples:
-          s3://mybucket/folder/object.json  -> mybucket
-          mybucket/folder/object.json  -> mybucket
-          mybucket -> ValueError  # no slash
-          /mybucket/folder/object.json -> ValueError # not expecting abs path
+    """Return a bucket name given a storage URI
+    Examples:
+      s3://mybucket/folder/object.json  -> mybucket
+      mybucket/folder/object.json  -> mybucket
+      mybucket -> ValueError  # no slash
+      /mybucket/folder/object.json -> ValueError # not expecting abs path
     """
     fields = _getURIParts(uri)
     bucket = fields[0]
     if not bucket:
         raise ValueError("invalid uri")
     return bucket
 
+
 def getKeyFromStorURI(uri):
-    """ Return a key (path within a bucket) given a storage URI 
-        Examples:
-          s3://mybucket/folder/object.json  -> mybucket
-          mybucket/folder/object.json  -> mybucket
-          mybucket -> ValueError  # no slash
-          /mybucket/folder/object.json -> ValueError # not expecting abs path
+    """Return a key (path within a bucket) given a storage URI
+    Examples:
+      s3://mybucket/folder/object.json  -> mybucket
+      mybucket/folder/object.json  -> mybucket
+      mybucket -> ValueError  # no slash
+      /mybucket/folder/object.json -> ValueError # not expecting abs path
     """
     fields = _getURIParts(uri)
     path = fields[1]
     if not path:
         raise ValueError("invalid uri")
     return path
 
 
+def getURIFromKey(app, bucket=None, key=None):
+    """ return URI for given bucket and key """
+    client = _getStorageClient(app)
+    if not bucket:
+        bucket = app["bucket_name"]
+    if key[0] == "/":
+        key = key[1:]  # no leading slash
+    uri = client.getURIFromKey(key, bucket=bucket)
+    return uri
+
+
 async def rangegetProxy(app, bucket=None, key=None, offset=0, length=0):
-    """ fetch bytes from rangeget proxy
-    """
+    """fetch bytes from rangeget proxy"""
     if "rangeget_url" in app:
-        req = app["rangeget_url"] + '/'
+        req = app["rangeget_url"] + "/"
     else:
         rangeget_port = config.get("rangeget_port")
         if "is_docker" in app:
             rangeget_host = "rangeget"
         else:
             rangeget_host = "127.0.0.1"
         req = f"http://{rangeget_host}:{rangeget_port}/"
@@ -207,121 +228,74 @@
         return None
 
     if len(data) != length:
         msg = f"expected {length} bytes for rangeget {bucket}{key}, "
         msg += f"but got: {len(data)}"
         log.warn(msg)
     return data
-    
 
 
 async def getStorJSONObj(app, key, bucket=None):
-    """ Get object identified by key and read as JSON
-    """
+    """Get object identified by key and read as JSON"""
 
     client = _getStorageClient(app)
     if not bucket:
-        bucket = app['bucket_name']
-    if key[0] == '/':
+        bucket = app["bucket_name"]
+    if key[0] == "/":
         key = key[1:]  # no leading slash
     log.info(f"getStorJSONObj({bucket})/{key}")
 
     data = await client.get_object(key, bucket=bucket)
 
     try:
-        json_dict = json.loads(data.decode('utf8'))
+        json_dict = json.loads(data.decode("utf8"))
     except UnicodeDecodeError:
         log.error(f"Error loading JSON at key: {key}")
         raise HTTPInternalServerError()
 
     msg = f"storage key {key} returned json object "
     msg += f"with {len(json_dict)} keys"
     log.debug(msg)
     return json_dict
 
 
-async def getStorBytes(app, key, filter_ops=None, offset=0,
-                       length=-1, bucket=None, use_proxy=False):
-    """ Get object identified by key and read as bytes
-    """
-
-    client = _getStorageClient(app)
-    if not bucket:
-        bucket = app['bucket_name']
-    if key[0] == '/':
-        key = key[1:]  # no leading slash
-    if offset is None:
-        offset = 0
-    if length is None:
-        length = 0
-    msg = f"getStorBytes({bucket}/{key}, offset={offset}, length: {length})"
-    log.info(msg)
-
-    default_req_size = 128 * 1024 * 1024  # 128KB
-    data_cache_max_req_size = int(config.get("data_cache_max_req_size", default=default_req_size))
-
-    shuffle = 0
-    compressor = None
-    if filter_ops:
-        log.debug(f"getStorBytes for {key} with filter_ops: {filter_ops}")
-        if "use_shuffle" in filter_ops and filter_ops['use_shuffle']:
-            shuffle = filter_ops['item_size']
-            log.debug("using shuffle filter")
-        if "compressor" in filter_ops:
-            compressor = filter_ops["compressor"]
-            log.debug(f"using compressor: {compressor}")
-
-    kwargs = {"bucket": bucket, "key": key,
-              "offset": offset, "length": length}
-    if offset > 0 and use_proxy and length < data_cache_max_req_size:
-        # use rangeget proxy
-        data = await rangegetProxy(app, **kwargs)
-    else:
-        data = await client.get_object(**kwargs)
-    if data is None or len(data) == 0:
-        log.info(f"no data found for {key}")
-        return data
-
-    log.info(f"read: {len(data)} bytes for key: {key}")
-    if length > 0 and len(data) != length:
-        log.warn(f"requested {length} bytes but got {len(data)} bytes")
+def _uncompress(data, compressor=None, shuffle=0):
+    """ Uncompress the provided data using compessor and/or shuffle """
     if compressor:
-
         # compressed chunk data...
 
         # first check if this was compressed with blosc
         # returns typesize, isshuffle, and memcopied
         blosc_metainfo = codecs.blosc.cbuffer_metainfo(data)
         if blosc_metainfo[0] > 0:
-            log.info(f"blosc compressed data for {key}")
+            log.info(f"blosc compressed data for {len(data)} bytes")
             try:
                 blosc = codecs.Blosc()
                 udata = blosc.decode(data)
                 log.info(f"uncompressed to {len(udata)} bytes")
                 data = udata
                 shuffle = 0  # blosc will unshuffle the bytes for us
             except Exception as e:
-                msg = f"got exception: {e} using blosc decompression for {key}"
+                msg = f"got exception: {e} using blosc decompression"
                 log.error(msg)
                 raise HTTPInternalServerError()
         elif compressor == "zlib":
             # data may have been compressed without blosc,
             # try using zlib directly
-            log.info(f"using zlib to decompress {key}")
+            log.info(f"using zlib to decompress {len(data)} bytes")
             try:
                 udata = zlib.decompress(data)
                 log.info(f"uncompressed to {len(udata)} bytes")
                 data = udata
             except zlib.error as zlib_error:
                 log.info(f"zlib_err: {zlib_error}")
-                log.error(f"unable to uncompress obj: {key}")
+                log.error("unable to uncompress data with zlib")
                 raise HTTPInternalServerError()
         else:
             msg = f"don't know how to decompress data in {compressor} "
-            msg += f"format for {key}"
             log.error(msg)
             raise HTTPInternalServerError()
 
     if shuffle > 0:
         log.debug(f"shuffle is {shuffle}")
         start_time = time.time()
         unshuffled = _unshuffle(shuffle, data)
@@ -332,30 +306,117 @@
         elapsed = finish_time - start_time
         msg = f"unshuffled {len(data)} bytes, {(elapsed):.2f} elapsed"
         log.debug(msg)
 
     return data
 
 
+async def getStorBytes(app,
+                       key,
+                       filter_ops=None,
+                       offset=0,
+                       length=-1,
+                       chunk_locations=None,
+                       chunk_bytes=None,
+                       h5_size=None,
+                       bucket=None,
+                       ):
+    """Get object identified by key and read as bytes"""
+
+    client = _getStorageClient(app)
+    if not bucket:
+        bucket = app["bucket_name"]
+    if key[0] == "/":
+        key = key[1:]  # no leading slash
+    if offset is None:
+        offset = 0
+    if length is None:
+        length = 0
+    msg = f"getStorBytes({bucket}/{key}, offset={offset}, length: {length})"
+    log.info(msg)
+
+    shuffle = 0
+    compressor = None
+    if filter_ops:
+        log.debug(f"getStorBytes for {key} with filter_ops: {filter_ops}")
+        if "use_shuffle" in filter_ops and filter_ops["use_shuffle"]:
+            shuffle = filter_ops["item_size"]
+            log.debug("using shuffle filter")
+        if "compressor" in filter_ops:
+            compressor = filter_ops["compressor"]
+            log.debug(f"using compressor: {compressor}")
+
+    kwargs = {"bucket": bucket, "key": key, "offset": offset, "length": length}
+
+    data = await client.get_object(**kwargs)
+    if data is None or len(data) == 0:
+        log.info(f"no data found for {key}")
+        return data
+
+    log.info(f"read: {len(data)} bytes for key: {key}")
+    if length > 0 and len(data) != length:
+        log.warn(f"requested {length} bytes but got {len(data)} bytes")
+
+    if chunk_locations:
+        log.debug(f"getStorBytes - got {len(chunk_locations)} chunk locations")
+        # uncompress chunks within the fetched data and store to
+        # chunk bytes
+        if not h5_size:
+            log.error("getStorBytes - h5_size not set")
+            raise HTTPInternalServerError()
+        if not chunk_bytes:
+            log.error("getStorBytes - chunk_bytes not set")
+            raise HTTPInternalServerError()
+        if len(chunk_locations) * h5_size < len(chunk_bytes):
+            log.error(f"getStorBytes - invalid chunk_bytes length: {len(chunk_bytes)}")
+        for chunk_location in chunk_locations:
+            log.debug(f"getStoreBytes - processing chunk_location: {chunk_location}")
+            n = chunk_location.offset - offset
+            if n < 0:
+                log.warn(f"getStorBytes - unexpected offset for chunk_location: {chunk_location}")
+                continue
+            m = n + chunk_location.length
+            log.debug(f"getStorBytes - extracting chunk from data[{n}:{m}]")
+            h5_bytes = data[n:m]
+            h5_bytes = _uncompress(h5_bytes, compressor=compressor, shuffle=shuffle)
+            if len(h5_bytes) != h5_size:
+                msg = f"expected chunk index: {chunk_location.index} to have size: "
+                msg += f"{h5_size} but got: {len(h5_bytes)}"
+                log.warning(msg)
+                continue
+            # slot into the hsds chunk
+            hs_offset = chunk_location.index * h5_size
+            if hs_offset + h5_size > len(chunk_bytes):
+                msg = f"expected chunk index: {chunk_location.index} to have offset: "
+                msg += f"less than {len(chunk_bytes) - h5_size} but got: {hs_offset}"
+                log.warning(msg)
+                continue
+            chunk_bytes[hs_offset:(hs_offset + h5_size)] = h5_bytes
+        # chunk_bytes got updated, so just return None
+        return None
+    else:
+        data = _uncompress(data, compressor=compressor, shuffle=shuffle)
+        return data
+
+
 async def putStorBytes(app, key, data, filter_ops=None, bucket=None):
-    """ Store byte string as S3 object with given key
-    """
+    """Store byte string as S3 object with given key"""
 
     client = _getStorageClient(app)
     if not bucket:
-        bucket = app['bucket_name']
-    if key[0] == '/':
+        bucket = app["bucket_name"]
+    if key[0] == "/":
         key = key[1:]  # no leading slash
     shuffle = -1  # auto-shuffle
     clevel = 5
     cname = None  # compressor name
     if filter_ops:
         if "compressor" in filter_ops:
             cname = filter_ops["compressor"]
-        if "use_shuffle" in filter_ops and not filter_ops['use_shuffle']:
+        if "use_shuffle" in filter_ops and not filter_ops["use_shuffle"]:
             shuffle = 0  # client indicates to turn off shuffling
         if "level" in filter_ops:
             clevel = filter_ops["level"]
     msg = f"putStorBytes({bucket}/{key}), {len(data)} bytes shuffle: {shuffle}"
     msg += f" compressor: {cname} level: {clevel}"
     log.info(msg)
 
@@ -374,104 +435,110 @@
 
     rsp = await client.put_object(key, data, bucket=bucket)
 
     return rsp
 
 
 async def putStorJSONObj(app, key, json_obj, bucket=None):
-    """ Store JSON data as storage object with given key
-    """
+    """Store JSON data as storage object with given key"""
 
     client = _getStorageClient(app)
     if not bucket:
-        bucket = app['bucket_name']
-    if key[0] == '/':
+        bucket = app["bucket_name"]
+    if key[0] == "/":
         key = key[1:]  # no leading slash
     log.info(f"putS3JSONObj({bucket}/{key})")
     data = json.dumps(json_obj)
-    data = data.encode('utf8')
+    data = data.encode("utf8")
 
     rsp = await client.put_object(key, data, bucket=bucket)
 
     return rsp
 
 
 async def deleteStorObj(app, key, bucket=None):
-    """ Delete storage object identfied by given key
-    """
+    """Delete storage object identfied by given key"""
 
     client = _getStorageClient(app)
     if not bucket:
-        bucket = app['bucket_name']
-    if key[0] == '/':
+        bucket = app["bucket_name"]
+    if key[0] == "/":
         key = key[1:]  # no leading slash
     log.info(f"deleteStorObj({key})")
 
     await client.delete_object(key, bucket=bucket)
 
     log.debug("deleteStorObj complete")
 
 
 async def getStorObjStats(app, key, bucket=None):
-    """ Return etag, size, and last modified time for given object
-    """
+    """Return etag, size, and last modified time for given object"""
     # TBD - will need to be refactored to handle azure responses
 
     client = _getStorageClient(app)
     if not bucket:
-        bucket = app['bucket_name']
+        bucket = app["bucket_name"]
     stats = {}
 
-    if key[0] == '/':
+    if key[0] == "/":
         # key = key[1:]  # no leading slash
         msg = f"key with leading slash: {key}"
         log.error(msg)
         raise KeyError(msg)
 
     log.info(f"getStorObjStats({key}, bucket={bucket})")
 
     stats = await client.get_key_stats(key, bucket=bucket)
 
     return stats
 
 
 async def isStorObj(app, key, bucket=None):
-    """ Test if the given key maps to S3 object
-    """
+    """Test if the given key maps to S3 object"""
     found = False
     client = _getStorageClient(app)
     if not bucket:
-        bucket = app['bucket_name']
+        bucket = app["bucket_name"]
     else:
         log.debug(f"using bucket: [{bucket}]")
     log.debug(f"isStorObj {bucket}/{key}")
 
     found = await client.is_object(bucket=bucket, key=key)
 
     log.debug(f"isStorObj {key} returning {found}")
     return found
 
 
-async def getStorKeys(app, prefix='', deliminator='', suffix='',
-                      include_stats=False, callback=None, bucket=None,
-                      limit=None):
+async def getStorKeys(
+    app,
+    prefix="",
+    deliminator="",
+    suffix="",
+    include_stats=False,
+    callback=None,
+    bucket=None,
+    limit=None,
+):
     # return keys matching the arguments
     client = _getStorageClient(app)
     if not bucket:
-        bucket = app['bucket_name']
+        bucket = app["bucket_name"]
     msg = f"getStorKeys('{prefix}','{deliminator}','{suffix}', "
     msg += f"include_stats={include_stats}"
     log.info(msg)
     kwargs = {}
     kwargs["prefix"] = prefix
     kwargs["deliminator"] = deliminator
     kwargs["suffix"] = suffix
     kwargs["include_stats"] = include_stats
     kwargs["callback"] = callback
     kwargs["bucket"] = bucket
     kwargs["limit"] = limit
 
     key_names = await client.list_keys(**kwargs)
 
-    log.info(f"getStorKeys done, got {len(key_names)} keys")
+    msg = f"getStorKeys done for prefix: {prefix}"
+    if not callback:
+        msg += f", got {len(key_names)} keys"
+    log.info(msg)
 
     return key_names
```

### Comparing `hsds-0.7.0b11/hsds/util/timeUtil.py` & `hsds-0.8.0/hsds/util/timeUtil.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,31 +22,31 @@
     utc = pytz.utc
     dtTime = datetime.fromtimestamp(timestamp, utc)
     iso_str = dtTime.isoformat()
     # isoformat returns a string like this:
     # '2014-10-30T04:25:21+00:00'
     # strip off the '+00:00' and replace
     # with 'Z' (both are ISO-8601 compatible)
-    npos = iso_str.rfind('+')
-    iso_z = iso_str[:npos] + 'Z'
+    npos = iso_str.rfind("+")
+    iso_z = iso_str[:npos] + "Z"
     return iso_z
 
 
 def elapsedTime(timestamp):
     """Get Elapsed time from given timestamp"""
     delta = int(time.time()) - timestamp
     if delta < 0:
         return "Invalid timestamp!"
-    day_length = 24*60*60
+    day_length = 24 * 60 * 60
     days = 0
-    hour_length = 60*60
+    hour_length = 60 * 60
     hours = 0
     minute_length = 60
     minutes = 0
-    ret_str = ''
+    ret_str = ""
 
     if delta > day_length:
         days = delta // day_length
         delta = delta % day_length
         ret_str += "{} days ".format(days)
     if delta > hour_length or days > 0:
         hours = delta // hour_length
```

### Comparing `hsds-0.7.0b11/hsds.egg-info/PKG-INFO` & `hsds-0.8.0/hsds.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: hsds
-Version: 0.7.0b11
+Version: 0.8.0
 Summary: HDF REST API
 Home-page: http://github.com/HDFGroup/hsds
 Author: John Readey
 Author-email: jreadey@hdfgrouup.org
 License: Apache
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: azure
+License-File: LICENSE
```

