# Comparing `tmp/phidata-2.0.0.dev8.tar.gz` & `tmp/phidata-2.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-2.0.0.dev8.tar", last modified: Mon Jul 24 17:46:49 2023, max compression
+gzip compressed data, was "phidata-2.0.0.dev9.tar", last modified: Tue Jul 25 10:18:41 2023, max compression
```

## Comparing `phidata-2.0.0.dev8.tar` & `phidata-2.0.0.dev9.tar`

### file list

```diff
@@ -1,755 +1,759 @@
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.702121 phidata-2.0.0.dev8/
--rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev8/LICENSE
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-24 17:46:49.701968 phidata-2.0.0.dev8/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev8/README.md
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.568589 phidata-2.0.0.dev8/phi/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.569746 phidata-2.0.0.dev8/phi/api/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/api/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1543 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/client.py
--rw-r--r--   0 zu         (501) staff       (20)      815 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/routes.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.570393 phidata-2.0.0.dev8/phi/api/schemas/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/schemas/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      131 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/schemas/response.py
--rw-r--r--   0 zu         (501) staff       (20)      490 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/schemas/user.py
--rw-r--r--   0 zu         (501) staff       (20)      442 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/schemas/workspace.py
--rw-r--r--   0 zu         (501) staff       (20)     3514 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/user.py
--rw-r--r--   0 zu         (501) staff       (20)     5735 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/workspace.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.570752 phidata-2.0.0.dev8/phi/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1310 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/api_client.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.571662 phidata-2.0.0.dev8/phi/aws/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    26919 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)      171 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/context.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.572136 phidata-2.0.0.dev8/phi/aws/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      766 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/fastapi/fastapi.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.572533 phidata-2.0.0.dev8/phi/aws/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2862 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/jupyter/jupyter.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.572932 phidata-2.0.0.dev8/phi/aws/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)       81 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      649 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.573447 phidata-2.0.0.dev8/phi/aws/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)       90 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      735 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/streamlit/streamlit.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.574754 phidata-2.0.0.dev8/phi/aws/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.575136 phidata-2.0.0.dev8/phi/aws/resource/acm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/acm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10489 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/acm/certificate.py
--rw-r--r--   0 zu         (501) staff       (20)     8725 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.575410 phidata-2.0.0.dev8/phi/aws/resource/cloudformation/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10247 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.576393 phidata-2.0.0.dev8/phi/aws/resource/ec2/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ec2/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21177 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ec2/security_group.py
--rw-r--r--   0 zu         (501) staff       (20)     2427 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ec2/subnet.py
--rw-r--r--   0 zu         (501) staff       (20)    11791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ec2/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.577742 phidata-2.0.0.dev8/phi/aws/resource/ecs/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6316 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    11368 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/container.py
--rw-r--r--   0 zu         (501) staff       (20)    19592 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/service.py
--rw-r--r--   0 zu         (501) staff       (20)    21760 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/task_definition.py
--rw-r--r--   0 zu         (501) staff       (20)     3385 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.579195 phidata-2.0.0.dev8/phi/aws/resource/eks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7252 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/addon.py
--rw-r--r--   0 zu         (501) staff       (20)    29689 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    13244 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 zu         (501) staff       (20)    24791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 zu         (501) staff       (20)    23405 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/node_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.579737 phidata-2.0.0.dev8/phi/aws/resource/elasticache/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elasticache/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    15451 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elasticache/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     5922 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.580480 phidata-2.0.0.dev8/phi/aws/resource/elb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10268 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elb/listener.py
--rw-r--r--   0 zu         (501) staff       (20)     7618 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elb/load_balancer.py
--rw-r--r--   0 zu         (501) staff       (20)     9507 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elb/target_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.580800 phidata-2.0.0.dev8/phi/aws/resource/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12578 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/emr/cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.581129 phidata-2.0.0.dev8/phi/aws/resource/glue/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12558 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/glue/crawler.py
--rw-r--r--   0 zu         (501) staff       (20)    23734 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.581655 phidata-2.0.0.dev8/phi/aws/resource/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7481 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/iam/policy.py
--rw-r--r--   0 zu         (501) staff       (20)     9714 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/iam/role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.582497 phidata-2.0.0.dev8/phi/aws/resource/rds/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/rds/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    35097 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/rds/db_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    34346 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/rds/db_instance.py
--rw-r--r--   0 zu         (501) staff       (20)     7611 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/rds/db_subnet_group.py
--rw-r--r--   0 zu         (501) staff       (20)      290 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/reference.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.582786 phidata-2.0.0.dev8/phi/aws/resource/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6400 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/s3/bucket.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.583363 phidata-2.0.0.dev8/phi/aws/resource/secret/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/secret/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11028 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/secret/manager.py
--rw-r--r--   0 zu         (501) staff       (20)      999 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/secret/reader.py
--rw-r--r--   0 zu         (501) staff       (20)     3475 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     5037 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.584639 phidata-2.0.0.dev8/phi/cli/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/cli/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3659 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/auth_server.py
--rw-r--r--   0 zu         (501) staff       (20)    13299 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/config.py
--rw-r--r--   0 zu         (501) staff       (20)     2907 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/console.py
--rw-r--r--   0 zu         (501) staff       (20)      804 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/credentials.py
--rw-r--r--   0 zu         (501) staff       (20)    20376 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/entrypoint.py
--rw-r--r--   0 zu         (501) staff       (20)    15872 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/operator.py
--rw-r--r--   0 zu         (501) staff       (20)     2045 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/cli/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.584973 phidata-2.0.0.dev8/phi/cli/ws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/cli/ws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27460 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/ws/ws_cli.py
--rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-24 15:34:09.000000 phidata-2.0.0.dev8/phi/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.585317 phidata-2.0.0.dev8/phi/docker/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1150 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/api_client.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.585841 phidata-2.0.0.dev8/phi/docker/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    14659 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/context.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.586135 phidata-2.0.0.dev8/phi/docker/app/django/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/django/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      917 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/django/django.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.586592 phidata-2.0.0.dev8/phi/docker/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      932 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/fastapi/fastapi.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.586909 phidata-2.0.0.dev8/phi/docker/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3275 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/jupyter/jupyter.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.587694 phidata-2.0.0.dev8/phi/docker/app/postgres/
--rw-r--r--   0 zu         (501) staff       (20)      148 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/postgres/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      232 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/postgres/pgvector.py
--rw-r--r--   0 zu         (501) staff       (20)     4732 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/docker/app/postgres/postgres.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.588213 phidata-2.0.0.dev8/phi/docker/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      731 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.588620 phidata-2.0.0.dev8/phi/docker/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)       93 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      901 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/streamlit/streamlit.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.590233 phidata-2.0.0.dev8/phi/docker/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4871 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)    15125 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/container.py
--rw-r--r--   0 zu         (501) staff       (20)    21704 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)    14791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/image.py
--rw-r--r--   0 zu         (501) staff       (20)     5126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/network.py
--rw-r--r--   0 zu         (501) staff       (20)     1130 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     4785 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.590679 phidata-2.0.0.dev8/phi/document/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/document/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      809 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/document/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.591544 phidata-2.0.0.dev8/phi/document/reader/
--rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/document/reader/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2149 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/document/reader/base.py
--rw-r--r--   0 zu         (501) staff       (20)     2074 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/document/reader/pdf.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.592252 phidata-2.0.0.dev8/phi/embedder/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/embedder/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      466 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/embedder/base.py
--rw-r--r--   0 zu         (501) staff       (20)      976 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/embedder/openai.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.592615 phidata-2.0.0.dev8/phi/infra/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.593500 phidata-2.0.0.dev8/phi/infra/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    13633 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)      522 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/app/context.py
--rw-r--r--   0 zu         (501) staff       (20)     1778 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/infra/app/db_app.py
--rw-r--r--   0 zu         (501) staff       (20)      126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/enums.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.594062 phidata-2.0.0.dev8/phi/infra/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6896 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)     1679 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.594259 phidata-2.0.0.dev8/phi/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/k8s/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.594910 phidata-2.0.0.dev8/phi/llm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/llm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      362 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/llm/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.595742 phidata-2.0.0.dev8/phi/llm/conversation/
--rw-r--r--   0 zu         (501) staff       (20)       85 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/conversation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11437 2023-07-24 16:43:22.000000 phidata-2.0.0.dev8/phi/llm/conversation/conversation.py
--rw-r--r--   0 zu         (501) staff       (20)     1293 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/conversation/schemas.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.596225 phidata-2.0.0.dev8/phi/llm/history/
--rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/history/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1636 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/history/base.py
--rw-r--r--   0 zu         (501) staff       (20)     1027 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/history/simple.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.596752 phidata-2.0.0.dev8/phi/llm/knowledge/
--rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/knowledge/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      714 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/knowledge/base.py
--rw-r--r--   0 zu         (501) staff       (20)     2382 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/knowledge/pdf.py
--rw-r--r--   0 zu         (501) staff       (20)     1169 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/llm/openai.py
--rw-r--r--   0 zu         (501) staff       (20)     1030 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/schemas.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.597469 phidata-2.0.0.dev8/phi/llm/storage/
--rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-23 16:37:22.000000 phidata-2.0.0.dev8/phi/llm/storage/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      670 2023-07-24 17:38:59.000000 phidata-2.0.0.dev8/phi/llm/storage/base.py
--rw-r--r--   0 zu         (501) staff       (20)     7930 2023-07-24 17:39:14.000000 phidata-2.0.0.dev8/phi/llm/storage/postgres.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.597792 phidata-2.0.0.dev8/phi/table/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/table/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.598101 phidata-2.0.0.dev8/phi/table/sql/
--rw-r--r--   0 zu         (501) staff       (20)       41 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/table/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      403 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/table/sql/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.600727 phidata-2.0.0.dev8/phi/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/common.py
--rw-r--r--   0 zu         (501) staff       (20)     1342 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/defaults.py
--rw-r--r--   0 zu         (501) staff       (20)      120 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/dttm.py
--rw-r--r--   0 zu         (501) staff       (20)     1020 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/filesystem.py
--rw-r--r--   0 zu         (501) staff       (20)     1640 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/git.py
--rw-r--r--   0 zu         (501) staff       (20)      889 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/json_io.py
--rw-r--r--   0 zu         (501) staff       (20)      665 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/load_env.py
--rw-r--r--   0 zu         (501) staff       (20)     1009 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/log.py
--rw-r--r--   0 zu         (501) staff       (20)     1010 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/pickle.py
--rw-r--r--   0 zu         (501) staff       (20)      724 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/py_io.py
--rw-r--r--   0 zu         (501) staff       (20)      589 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/pyproject.py
--rw-r--r--   0 zu         (501) staff       (20)      962 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/resource_filter.py
--rw-r--r--   0 zu         (501) staff       (20)      829 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/yaml_io.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.601152 phidata-2.0.0.dev8/phi/vectordb/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/vectordb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      700 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/vectordb/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.601712 phidata-2.0.0.dev8/phi/vectordb/pgvector/
--rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/vectordb/pgvector/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5592 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/vectordb/pgvector/pgvector.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.603105 phidata-2.0.0.dev8/phi/workspace/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/workspace/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10069 2023-07-24 15:35:53.000000 phidata-2.0.0.dev8/phi/workspace/config.py
--rw-r--r--   0 zu         (501) staff       (20)      321 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/workspace/enums.py
--rw-r--r--   0 zu         (501) staff       (20)     1914 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/workspace/helpers.py
--rw-r--r--   0 zu         (501) staff       (20)    25401 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/workspace/operator.py
--rw-r--r--   0 zu         (501) staff       (20)     9063 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/workspace/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.603761 phidata-2.0.0.dev8/phidata/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.605162 phidata-2.0.0.dev8/phidata/airflow/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/airflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      140 2022-10-01 00:05:40.000000 phidata-2.0.0.dev8/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.605592 phidata-2.0.0.dev8/phidata/airflow/operators/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/airflow/operators/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      584 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.608629 phidata-2.0.0.dev8/phidata/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-10-28 00:34:05.000000 phidata-2.0.0.dev8/phidata/app/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.611500 phidata-2.0.0.dev8/phidata/app/airflow/
--rw-r--r--   0 zu         (501) staff       (20)      385 2022-11-02 02:52:41.000000 phidata-2.0.0.dev8/phidata/app/airflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)   100927 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 zu         (501) staff       (20)    30469 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 zu         (501) staff       (20)    30508 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 zu         (501) staff       (20)    30505 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 zu         (501) staff       (20)    30515 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 zu         (501) staff       (20)    30710 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.612136 phidata-2.0.0.dev8/phidata/app/alertmanager/
--rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47889 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.613269 phidata-2.0.0.dev8/phidata/app/amundsen/
--rw-r--r--   0 zu         (501) staff       (20)      398 2023-03-11 17:40:59.000000 phidata-2.0.0.dev8/phidata/app/amundsen/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    48031 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/amundsen/frontend.py
--rw-r--r--   0 zu         (501) staff       (20)    48032 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/amundsen/metadata.py
--rw-r--r--   0 zu         (501) staff       (20)    47944 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/amundsen/search.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.613912 phidata-2.0.0.dev8/phidata/app/assistant/
--rw-r--r--   0 zu         (501) staff       (20)      139 2023-01-15 00:33:10.000000 phidata-2.0.0.dev8/phidata/app/assistant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49912 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/assistant/assistant.py
--rw-r--r--   0 zu         (501) staff       (20)    30166 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/aws_app.py
--rw-r--r--   0 zu         (501) staff       (20)    17164 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/base_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.614417 phidata-2.0.0.dev8/phidata/app/cadvisor/
--rw-r--r--   0 zu         (501) staff       (20)      118 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49678 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.615130 phidata-2.0.0.dev8/phidata/app/databox/
--rw-r--r--   0 zu         (501) staff       (20)      157 2023-01-15 00:32:07.000000 phidata-2.0.0.dev8/phidata/app/databox/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    86151 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/databox/databox.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.616101 phidata-2.0.0.dev8/phidata/app/db/
--rw-r--r--   0 zu         (501) staff       (20)       52 2022-03-29 16:28:05.000000 phidata-2.0.0.dev8/phidata/app/db/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3187 2023-01-05 15:43:33.000000 phidata-2.0.0.dev8/phidata/app/db/base_db.py
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-04 16:30:27.000000 phidata-2.0.0.dev8/phidata/app/db/db_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.616735 phidata-2.0.0.dev8/phidata/app/django/
--rw-r--r--   0 zu         (501) staff       (20)      105 2023-05-18 09:49:43.000000 phidata-2.0.0.dev8/phidata/app/django/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27483 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/django/django_app.py
--rw-r--r--   0 zu         (501) staff       (20)    30070 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/django/django_backup.py
--rw-r--r--   0 zu         (501) staff       (20)    17172 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/docker_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.617307 phidata-2.0.0.dev8/phidata/app/elastic/
--rw-r--r--   0 zu         (501) staff       (20)       71 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/app/elastic/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3723 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.617797 phidata-2.0.0.dev8/phidata/app/elasticsearch/
--rw-r--r--   0 zu         (501) staff       (20)      138 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    48675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.618559 phidata-2.0.0.dev8/phidata/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)      175 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    20266 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/fastapi/fastapi_server.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.619193 phidata-2.0.0.dev8/phidata/app/grafana/
--rw-r--r--   0 zu         (501) staff       (20)      114 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/grafana/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49781 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/grafana/grafana.py
--rw-r--r--   0 zu         (501) staff       (20)      822 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.620485 phidata-2.0.0.dev8/phidata/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)      273 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27093 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/jupyter/jupyter.py
--rw-r--r--   0 zu         (501) staff       (20)    46942 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 zu         (501) staff       (20)    93432 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.621349 phidata-2.0.0.dev8/phidata/app/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-05-24 02:25:43.000000 phidata-2.0.0.dev8/phidata/app/k8s/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3930 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/k8s/app.py
--rw-r--r--   0 zu         (501) staff       (20)     1766 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/k8s/dir.py
--rw-r--r--   0 zu         (501) staff       (20)     6550 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/k8s/url.py
--rw-r--r--   0 zu         (501) staff       (20)    37830 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/k8s_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.621746 phidata-2.0.0.dev8/phidata/app/mysql/
--rw-r--r--   0 zu         (501) staff       (20)      151 2023-05-03 15:21:14.000000 phidata-2.0.0.dev8/phidata/app/mysql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49110 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.622277 phidata-2.0.0.dev8/phidata/app/neo4j/
--rw-r--r--   0 zu         (501) staff       (20)      106 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/neo4j/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47856 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.622806 phidata-2.0.0.dev8/phidata/app/nodeexporter/
--rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47898 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 zu         (501) staff       (20)    38495 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/phidata_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.623512 phidata-2.0.0.dev8/phidata/app/postgres/
--rw-r--r--   0 zu         (501) staff       (20)      166 2023-01-15 00:33:00.000000 phidata-2.0.0.dev8/phidata/app/postgres/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    53156 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.624101 phidata-2.0.0.dev8/phidata/app/prometheus/
--rw-r--r--   0 zu         (501) staff       (20)      126 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/prometheus/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49051 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.624710 phidata-2.0.0.dev8/phidata/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12372 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.625411 phidata-2.0.0.dev8/phidata/app/redis/
--rw-r--r--   0 zu         (501) staff       (20)      144 2023-01-15 00:32:35.000000 phidata-2.0.0.dev8/phidata/app/redis/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/redis/redis.py
--rw-r--r--   0 zu         (501) staff       (20)    53296 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/redis/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.626559 phidata-2.0.0.dev8/phidata/app/server/
--rw-r--r--   0 zu         (501) staff       (20)      207 2023-05-18 09:49:43.000000 phidata-2.0.0.dev8/phidata/app/server/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    18424 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/server/api_server.py
--rw-r--r--   0 zu         (501) staff       (20)    58714 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/server/server_base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.628175 phidata-2.0.0.dev8/phidata/app/spark/
--rw-r--r--   0 zu         (501) staff       (20)      193 2023-02-07 16:41:27.000000 phidata-2.0.0.dev8/phidata/app/spark/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49424 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/spark/spark_base.py
--rw-r--r--   0 zu         (501) staff       (20)    17222 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/spark/spark_driver.py
--rw-r--r--   0 zu         (501) staff       (20)    17332 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.628677 phidata-2.0.0.dev8/phidata/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)      174 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    20207 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/app/streamlit/streamlit_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.630543 phidata-2.0.0.dev8/phidata/app/superset/
--rw-r--r--   0 zu         (501) staff       (20)      411 2022-11-02 02:52:41.000000 phidata-2.0.0.dev8/phidata/app/superset/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    71570 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_base.py
--rw-r--r--   0 zu         (501) staff       (20)    22925 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_init.py
--rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_worker.py
--rw-r--r--   0 zu         (501) staff       (20)    22917 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.631848 phidata-2.0.0.dev8/phidata/app/traefik/
--rw-r--r--   0 zu         (501) staff       (20)      173 2023-01-15 00:32:52.000000 phidata-2.0.0.dev8/phidata/app/traefik/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)   115905 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/traefik/crds.py
--rw-r--r--   0 zu         (501) staff       (20)    48190 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 zu         (501) staff       (20)    44972 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/traefik/router.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.632276 phidata-2.0.0.dev8/phidata/asset/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/asset/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.632691 phidata-2.0.0.dev8/phidata/asset/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/asset/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3210 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 zu         (501) staff       (20)    24787 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/asset/data_asset.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.633444 phidata-2.0.0.dev8/phidata/asset/local/
--rw-r--r--   0 zu         (501) staff       (20)       71 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/asset/local/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    14564 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/asset/local/file.py
--rw-r--r--   0 zu         (501) staff       (20)      574 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.635438 phidata-2.0.0.dev8/phidata/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1835 2023-03-13 15:21:09.000000 phidata-2.0.0.dev8/phidata/aws/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)      487 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/aws/args.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.635932 phidata-2.0.0.dev8/phidata/aws/athena/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8186 2023-03-13 15:21:09.000000 phidata-2.0.0.dev8/phidata/aws/athena/query.py
--rw-r--r--   0 zu         (501) staff       (20)     3168 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/aws/config.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.636200 phidata-2.0.0.dev8/phidata/aws/create/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/create/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.636690 phidata-2.0.0.dev8/phidata/aws/create/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3233 2023-03-13 15:21:09.000000 phidata-2.0.0.dev8/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 zu         (501) staff       (20)     2472 2023-03-13 15:21:09.000000 phidata-2.0.0.dev8/phidata/aws/create/iam/role.py
--rw-r--r--   0 zu         (501) staff       (20)    23058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/driver.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.637235 phidata-2.0.0.dev8/phidata/aws/enums/
--rw-r--r--   0 zu         (501) staff       (20)       62 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/enums/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1083 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/enums/manager_status.py
--rw-r--r--   0 zu         (501) staff       (20)      304 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8588 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.638248 phidata-2.0.0.dev8/phidata/aws/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.638597 phidata-2.0.0.dev8/phidata/aws/resource/acm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.638987 phidata-2.0.0.dev8/phidata/aws/resource/athena/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/athena/query.py
--rw-r--r--   0 zu         (501) staff       (20)     9127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.639299 phidata-2.0.0.dev8/phidata/aws/resource/cloudformation/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.640026 phidata-2.0.0.dev8/phidata/aws/resource/ec2/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21341 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ec2/security_group.py
--rw-r--r--   0 zu         (501) staff       (20)     2563 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 zu         (501) staff       (20)    11801 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.641388 phidata-2.0.0.dev8/phidata/aws/resource/ecs/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6140 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    26253 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 zu         (501) staff       (20)    19630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 zu         (501) staff       (20)    22397 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 zu         (501) staff       (20)     3614 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.642970 phidata-2.0.0.dev8/phidata/aws/resource/eks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 zu         (501) staff       (20)    30104 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    13731 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 zu         (501) staff       (20)    23785 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 zu         (501) staff       (20)    23742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.643617 phidata-2.0.0.dev8/phidata/aws/resource/elasticache/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    15823 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     6305 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.644526 phidata-2.0.0.dev8/phidata/aws/resource/elb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-07 15:40:41.000000 phidata-2.0.0.dev8/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10727 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 zu         (501) staff       (20)     7994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 zu         (501) staff       (20)     9834 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.644930 phidata-2.0.0.dev8/phidata/aws/resource/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12806 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.645429 phidata-2.0.0.dev8/phidata/aws/resource/glue/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12850 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 zu         (501) staff       (20)     3418 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/aws/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.648124 phidata-2.0.0.dev8/phidata/aws/resource/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     9958 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/iam/group.py
--rw-r--r--   0 zu         (501) staff       (20)     7653 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 zu         (501) staff       (20)     9828 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.648999 phidata-2.0.0.dev8/phidata/aws/resource/rds/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    36056 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    35380 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 zu         (501) staff       (20)     7990 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.649286 phidata-2.0.0.dev8/phidata/aws/resource/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6472 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.649780 phidata-2.0.0.dev8/phidata/aws/resource/secret/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11398 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 zu         (501) staff       (20)     1007 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/aws/resource/secret/reader.py
--rw-r--r--   0 zu         (501) staff       (20)     3604 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     9688 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/utils.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.650903 phidata-2.0.0.dev8/phidata/aws/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21797 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 zu         (501) staff       (20)    24100 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/s3/dataset.py
--rw-r--r--   0 zu         (501) staff       (20)    14394 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 zu         (501) staff       (20)     7409 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/s3/object.py
--rw-r--r--   0 zu         (501) staff       (20)    22470 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/worker.py
--rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.651552 phidata-2.0.0.dev8/phidata/checks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/checks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2790 2023-01-31 22:57:08.000000 phidata-2.0.0.dev8/phidata/checks/check.py
--rw-r--r--   0 zu         (501) staff       (20)      754 2023-02-03 21:54:28.000000 phidata-2.0.0.dev8/phidata/checks/not_empty.py
--rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev8/phidata/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.652345 phidata-2.0.0.dev8/phidata/decorators/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/decorators/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      582 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/decorators/timer.py
--rw-r--r--   0 zu         (501) staff       (20)     1110 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/decorators/validate_env.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.654310 phidata-2.0.0.dev8/phidata/docker/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1728 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     1645 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/args.py
--rw-r--r--   0 zu         (501) staff       (20)     4482 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/config.py
--rw-r--r--   0 zu         (501) staff       (20)     1166 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/enums.py
--rw-r--r--   0 zu         (501) staff       (20)      322 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8899 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.656302 phidata-2.0.0.dev8/phidata/docker/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3804 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)    16440 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/container.py
--rw-r--r--   0 zu         (501) staff       (20)      932 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/docker/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)    14773 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/image.py
--rw-r--r--   0 zu         (501) staff       (20)     5226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/resource/network.py
--rw-r--r--   0 zu         (501) staff       (20)     1165 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)    10737 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/utils.py
--rw-r--r--   0 zu         (501) staff       (20)     4961 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/resource/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.656610 phidata-2.0.0.dev8/phidata/docker/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3584 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/utils/container.py
--rw-r--r--   0 zu         (501) staff       (20)    24179 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.657799 phidata-2.0.0.dev8/phidata/exceptions/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-22 20:24:07.000000 phidata-2.0.0.dev8/phidata/exceptions/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)       47 2022-05-24 18:09:11.000000 phidata-2.0.0.dev8/phidata/exceptions/app.py
--rw-r--r--   0 zu         (501) staff       (20)       39 2022-04-22 20:24:07.000000 phidata-2.0.0.dev8/phidata/exceptions/task.py
--rw-r--r--   0 zu         (501) staff       (20)       43 2022-04-25 21:05:27.000000 phidata-2.0.0.dev8/phidata/exceptions/workflow.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.659315 phidata-2.0.0.dev8/phidata/infra/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/infra/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      341 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/infra/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     2466 2023-01-25 22:40:46.000000 phidata-2.0.0.dev8/phidata/infra/args.py
--rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/infra/config.py
--rw-r--r--   0 zu         (501) staff       (20)    12048 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/infra/resource.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.661159 phidata-2.0.0.dev8/phidata/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     1986 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/k8s/args.py
--rw-r--r--   0 zu         (501) staff       (20)     7871 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/config.py
--rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.662123 phidata-2.0.0.dev8/phidata/k8s/create/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.662408 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.662887 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3418 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 zu         (501) staff       (20)     2430 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.663113 phidata-2.0.0.dev8/phidata/k8s/create/apps/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.663297 phidata-2.0.0.dev8/phidata/k8s/create/apps/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5429 2023-01-24 16:40:47.000000 phidata-2.0.0.dev8/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.663833 phidata-2.0.0.dev8/phidata/k8s/create/common/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      357 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/common/labels.py
--rw-r--r--   0 zu         (501) staff       (20)     1553 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.663982 phidata-2.0.0.dev8/phidata/k8s/create/core/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.665953 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1395 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 zu         (501) staff       (20)     5490 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 zu         (501) staff       (20)     1515 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 zu         (501) staff       (20)     6695 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 zu         (501) staff       (20)     2005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 zu         (501) staff       (20)     1555 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 zu         (501) staff       (20)     4200 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 zu         (501) staff       (20)     2030 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 zu         (501) staff       (20)     4516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.666225 phidata-2.0.0.dev8/phidata/k8s/create/crb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2115 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 zu         (501) staff       (20)    19062 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/group.py
--rw-r--r--   0 zu         (501) staff       (20)     5795 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.666521 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.666741 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:37.000000 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2069 2023-01-31 02:29:01.000000 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.667083 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.667508 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1754 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 zu         (501) staff       (20)     1503 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.667689 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.667917 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.670111 phidata-2.0.0.dev8/phidata/k8s/enums/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/api_group.py
--rw-r--r--   0 zu         (501) staff       (20)      542 2023-01-31 02:03:51.000000 phidata-2.0.0.dev8/phidata/k8s/enums/api_version.py
--rw-r--r--   0 zu         (501) staff       (20)      162 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 zu         (501) staff       (20)      762 2023-01-31 02:04:08.000000 phidata-2.0.0.dev8/phidata/k8s/enums/kind.py
--rw-r--r--   0 zu         (501) staff       (20)     1085 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 zu         (501) staff       (20)      127 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/protocol.py
--rw-r--r--   0 zu         (501) staff       (20)      753 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/pv.py
--rw-r--r--   0 zu         (501) staff       (20)      153 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 zu         (501) staff       (20)      171 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/service_type.py
--rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 zu         (501) staff       (20)      377 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 zu         (501) staff       (20)      419 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8596 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.671386 phidata-2.0.0.dev8/phidata/k8s/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.671562 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.671976 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8592 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.672308 phidata-2.0.0.dev8/phidata/k8s/resource/apps/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.672922 phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10211 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 zu         (501) staff       (20)     1958 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.673134 phidata-2.0.0.dev8/phidata/k8s/resource/core/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.677517 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6602 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 zu         (501) staff       (20)    18530 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 zu         (501) staff       (20)      822 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 zu         (501) staff       (20)     6635 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 zu         (501) staff       (20)     3863 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 zu         (501) staff       (20)     1614 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 zu         (501) staff       (20)    12419 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 zu         (501) staff       (20)     8107 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 zu         (501) staff       (20)     2693 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 zu         (501) staff       (20)     7468 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 zu         (501) staff       (20)      901 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 zu         (501) staff       (20)     1244 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 zu         (501) staff       (20)     6196 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 zu         (501) staff       (20)    18982 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 zu         (501) staff       (20)     8657 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 zu         (501) staff       (20)     2313 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 zu         (501) staff       (20)     4086 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 zu         (501) staff       (20)     4788 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 zu         (501) staff       (20)      890 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 zu         (501) staff       (20)    13397 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 zu         (501) staff       (20)    12690 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/k8s/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)     4475 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.678983 phidata-2.0.0.dev8/phidata/k8s/resource/meta/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.679471 phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1058 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 zu         (501) staff       (20)     2739 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.679679 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:16.000000 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.679988 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:42.000000 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10026 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.680248 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.680940 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 zu         (501) staff       (20)     6675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.681175 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.681540 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7198 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 zu         (501) staff       (20)     3415 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)    10127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.682023 phidata-2.0.0.dev8/phidata/k8s/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1864 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/utils/pod.py
--rw-r--r--   0 zu         (501) staff       (20)    43059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.682200 phidata-2.0.0.dev8/phidata/llm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/llm/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.683655 phidata-2.0.0.dev8/phidata/llm/duckdb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4403 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/agent.py
--rw-r--r--   0 zu         (501) staff       (20)     3896 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/chain.py
--rw-r--r--   0 zu         (501) staff       (20)      920 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/connection.py
--rw-r--r--   0 zu         (501) staff       (20)     1194 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/loader.py
--rw-r--r--   0 zu         (501) staff       (20)     2177 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/query.py
--rw-r--r--   0 zu         (501) staff       (20)     1063 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.684330 phidata-2.0.0.dev8/phidata/product/
--rw-r--r--   0 zu         (501) staff       (20)       70 2022-03-13 21:20:10.000000 phidata-2.0.0.dev8/phidata/product/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    29505 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/product/data_product.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.684671 phidata-2.0.0.dev8/phidata/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      445 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/resource/reference.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.684908 phidata-2.0.0.dev8/phidata/table/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/table/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.685547 phidata-2.0.0.dev8/phidata/table/local/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/table/local/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4616 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/local/csv.py
--rw-r--r--   0 zu         (501) staff       (20)    23516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/local/local_table.py
--rw-r--r--   0 zu         (501) staff       (20)     4624 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/local/parquet.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.686201 phidata-2.0.0.dev8/phidata/table/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/table/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4673 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/s3/csv.py
--rw-r--r--   0 zu         (501) staff       (20)     4668 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/s3/parquet.py
--rw-r--r--   0 zu         (501) staff       (20)    23064 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.686832 phidata-2.0.0.dev8/phidata/table/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/table/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1752 2023-04-07 15:40:41.000000 phidata-2.0.0.dev8/phidata/table/sql/postgres.py
--rw-r--r--   0 zu         (501) staff       (20)    35497 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.688477 phidata-2.0.0.dev8/phidata/task/
--rw-r--r--   0 zu         (501) staff       (20)       79 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/task/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.688755 phidata-2.0.0.dev8/phidata/task/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/aws/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.689298 phidata-2.0.0.dev8/phidata/task/aws/athena/
--rw-r--r--   0 zu         (501) staff       (20)       81 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2210 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.689843 phidata-2.0.0.dev8/phidata/task/aws/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.690405 phidata-2.0.0.dev8/phidata/task/aws/glue/
--rw-r--r--   0 zu         (501) staff       (20)      100 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2038 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 zu         (501) staff       (20)     1381 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/decorator.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.690618 phidata-2.0.0.dev8/phidata/task/dev/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/dev/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.690740 phidata-2.0.0.dev8/phidata/task/download/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/download/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.690976 phidata-2.0.0.dev8/phidata/task/download/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/download/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2114 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.691866 phidata-2.0.0.dev8/phidata/task/download/url/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/download/url/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4775 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/task/download/url/to_file.py
--rw-r--r--   0 zu         (501) staff       (20)     3681 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/task/download/url/to_s3.py
--rw-r--r--   0 zu         (501) staff       (20)     8180 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692021 phidata-2.0.0.dev8/phidata/task/plot/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/plot/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692263 phidata-2.0.0.dev8/phidata/task/plot/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2541 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/plot/sql/query.py
--rw-r--r--   0 zu         (501) staff       (20)    12300 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/task/python_task.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692537 phidata-2.0.0.dev8/phidata/task/run/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/run/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692725 phidata-2.0.0.dev8/phidata/task/run/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/run/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4126 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/task/run/sql/query.py
--rw-r--r--   0 zu         (501) staff       (20)     7636 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/task/task.py
--rw-r--r--   0 zu         (501) staff       (20)     1041 2022-04-25 21:05:27.000000 phidata-2.0.0.dev8/phidata/task/task_relatives.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692995 phidata-2.0.0.dev8/phidata/task/upload/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/upload/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.693332 phidata-2.0.0.dev8/phidata/task/upload/file/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/upload/file/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2039 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 zu         (501) staff       (20)     4721 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.694457 phidata-2.0.0.dev8/phidata/types/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/types/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1023 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/types/airflow.py
--rw-r--r--   0 zu         (501) staff       (20)     2063 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/types/context.py
--rw-r--r--   0 zu         (501) staff       (20)      705 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/types/phidata_runtime.py
--rw-r--r--   0 zu         (501) staff       (20)      101 2022-04-22 20:24:07.000000 phidata-2.0.0.dev8/phidata/types/run_status.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.699386 phidata-2.0.0.dev8/phidata/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4779 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/cli_console.py
--rw-r--r--   0 zu         (501) staff       (20)     2044 2023-01-31 02:10:08.000000 phidata-2.0.0.dev8/phidata/utils/common.py
--rw-r--r--   0 zu         (501) staff       (20)     1037 2022-11-28 16:47:00.000000 phidata-2.0.0.dev8/phidata/utils/compare.py
--rw-r--r--   0 zu         (501) staff       (20)     2146 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/utils/context.py
--rw-r--r--   0 zu         (501) staff       (20)     1113 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/dttm.py
--rw-r--r--   0 zu         (501) staff       (20)      786 2022-06-12 23:07:23.000000 phidata-2.0.0.dev8/phidata/utils/enums.py
--rw-r--r--   0 zu         (501) staff       (20)     1595 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/env_file.py
--rw-r--r--   0 zu         (501) staff       (20)     1430 2022-07-31 02:48:39.000000 phidata-2.0.0.dev8/phidata/utils/env_var.py
--rw-r--r--   0 zu         (501) staff       (20)      661 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/utils/filesystem.py
--rw-r--r--   0 zu         (501) staff       (20)      742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/get_python_objects_from_module.py
--rw-r--r--   0 zu         (501) staff       (20)      893 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/utils/json_io.py
--rw-r--r--   0 zu         (501) staff       (20)     1257 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/utils/k8s.py
--rw-r--r--   0 zu         (501) staff       (20)     1459 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/log.py
--rw-r--r--   0 zu         (501) staff       (20)      707 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/utils/print_table.py
--rw-r--r--   0 zu         (501) staff       (20)      994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/workspace_path.py
--rw-r--r--   0 zu         (501) staff       (20)      833 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/utils/yaml_io.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.700552 phidata-2.0.0.dev8/phidata/workflow/
--rw-r--r--   0 zu         (501) staff       (20)      109 2022-04-15 05:02:36.000000 phidata-2.0.0.dev8/phidata/workflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1855 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/workflow/decorator.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.700854 phidata-2.0.0.dev8/phidata/workflow/dev/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/workflow/dev/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    42342 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/workflow/workflow.py
--rw-r--r--   0 zu         (501) staff       (20)     1105 2022-04-25 21:05:27.000000 phidata-2.0.0.dev8/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.701374 phidata-2.0.0.dev8/phidata/workspace/
--rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/workspace/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11316 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/workspace/config.py
--rw-r--r--   0 zu         (501) staff       (20)     8781 2023-07-06 09:54:23.000000 phidata-2.0.0.dev8/phidata/workspace/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.604904 phidata-2.0.0.dev8/phidata.egg-info/
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)    18804 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/entry_points.txt
--rw-r--r--   0 zu         (501) staff       (20)      181 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/requires.txt
--rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/top_level.txt
--rw-r--r--   0 zu         (501) staff       (20)     1676 2023-07-24 17:42:03.000000 phidata-2.0.0.dev8/pyproject.toml
--rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-24 17:46:49.702166 phidata-2.0.0.dev8/setup.cfg
--rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev8/setup.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.701653 phidata-2.0.0.dev8/tests/
--rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev8/tests/test_placeholder.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.436544 phidata-2.0.0.dev9/
+-rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev9/LICENSE
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-25 10:18:41.436352 phidata-2.0.0.dev9/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev9/README.md
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.341147 phidata-2.0.0.dev9/phi/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.342440 phidata-2.0.0.dev9/phi/api/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/api/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1543 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/api/client.py
+-rw-r--r--   0 zu         (501) staff       (20)      815 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/api/routes.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.343161 phidata-2.0.0.dev9/phi/api/schemas/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/api/schemas/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      131 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/api/schemas/response.py
+-rw-r--r--   0 zu         (501) staff       (20)      490 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/api/schemas/user.py
+-rw-r--r--   0 zu         (501) staff       (20)      442 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/api/schemas/workspace.py
+-rw-r--r--   0 zu         (501) staff       (20)     3514 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/api/user.py
+-rw-r--r--   0 zu         (501) staff       (20)     5735 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/api/workspace.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.343409 phidata-2.0.0.dev9/phi/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1310 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/api_client.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.344156 phidata-2.0.0.dev9/phi/aws/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    26919 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      171 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/context.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.344611 phidata-2.0.0.dev9/phi/aws/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      766 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/fastapi/fastapi.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.345060 phidata-2.0.0.dev9/phi/aws/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2862 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/jupyter/jupyter.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.345490 phidata-2.0.0.dev9/phi/aws/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)       81 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      649 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.345941 phidata-2.0.0.dev9/phi/aws/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)       90 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      735 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/app/streamlit/streamlit.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.347487 phidata-2.0.0.dev9/phi/aws/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.347884 phidata-2.0.0.dev9/phi/aws/resource/acm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/acm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10489 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/acm/certificate.py
+-rw-r--r--   0 zu         (501) staff       (20)     8725 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.348176 phidata-2.0.0.dev9/phi/aws/resource/cloudformation/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10247 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.349328 phidata-2.0.0.dev9/phi/aws/resource/ec2/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ec2/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21177 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ec2/security_group.py
+-rw-r--r--   0 zu         (501) staff       (20)     2427 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ec2/subnet.py
+-rw-r--r--   0 zu         (501) staff       (20)    11791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ec2/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.350887 phidata-2.0.0.dev9/phi/aws/resource/ecs/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ecs/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6316 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ecs/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    11368 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ecs/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    19592 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ecs/service.py
+-rw-r--r--   0 zu         (501) staff       (20)    21760 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 zu         (501) staff       (20)     3385 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/ecs/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.352465 phidata-2.0.0.dev9/phi/aws/resource/eks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/eks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7252 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/eks/addon.py
+-rw-r--r--   0 zu         (501) staff       (20)    29689 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/eks/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    13244 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 zu         (501) staff       (20)    24791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 zu         (501) staff       (20)    23405 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/eks/node_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.353033 phidata-2.0.0.dev9/phi/aws/resource/elasticache/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    15451 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     5922 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.353984 phidata-2.0.0.dev9/phi/aws/resource/elb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/elb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10268 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/elb/listener.py
+-rw-r--r--   0 zu         (501) staff       (20)     7618 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 zu         (501) staff       (20)     9507 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/elb/target_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.354315 phidata-2.0.0.dev9/phi/aws/resource/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12578 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/emr/cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.354665 phidata-2.0.0.dev9/phi/aws/resource/glue/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12558 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/glue/crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)    23734 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.355198 phidata-2.0.0.dev9/phi/aws/resource/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7481 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/iam/policy.py
+-rw-r--r--   0 zu         (501) staff       (20)     9714 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/iam/role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.356220 phidata-2.0.0.dev9/phi/aws/resource/rds/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/rds/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    35097 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    34346 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/rds/db_instance.py
+-rw-r--r--   0 zu         (501) staff       (20)     7611 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/rds/db_subnet_group.py
+-rw-r--r--   0 zu         (501) staff       (20)      290 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/reference.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.356541 phidata-2.0.0.dev9/phi/aws/resource/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6400 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/s3/bucket.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.357063 phidata-2.0.0.dev9/phi/aws/resource/secret/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/secret/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11028 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/secret/manager.py
+-rw-r--r--   0 zu         (501) staff       (20)      999 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/secret/reader.py
+-rw-r--r--   0 zu         (501) staff       (20)     3475 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/aws/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     5037 2023-07-18 13:44:43.000000 phidata-2.0.0.dev9/phi/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.358458 phidata-2.0.0.dev9/phi/cli/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/cli/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3659 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/cli/auth_server.py
+-rw-r--r--   0 zu         (501) staff       (20)    13299 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/cli/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     2907 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/cli/console.py
+-rw-r--r--   0 zu         (501) staff       (20)      804 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/cli/credentials.py
+-rw-r--r--   0 zu         (501) staff       (20)    20376 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/cli/entrypoint.py
+-rw-r--r--   0 zu         (501) staff       (20)    15872 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/cli/operator.py
+-rw-r--r--   0 zu         (501) staff       (20)     2045 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/cli/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.358818 phidata-2.0.0.dev9/phi/cli/ws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/cli/ws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27460 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/cli/ws/ws_cli.py
+-rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-24 15:34:09.000000 phidata-2.0.0.dev9/phi/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.359121 phidata-2.0.0.dev9/phi/docker/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1150 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/api_client.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.359689 phidata-2.0.0.dev9/phi/docker/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    14659 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/context.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.360015 phidata-2.0.0.dev9/phi/docker/app/django/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/django/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      917 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/django/django.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.360343 phidata-2.0.0.dev9/phi/docker/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      932 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/fastapi/fastapi.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.360628 phidata-2.0.0.dev9/phi/docker/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3275 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/jupyter/jupyter.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.361258 phidata-2.0.0.dev9/phi/docker/app/postgres/
+-rw-r--r--   0 zu         (501) staff       (20)      148 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/postgres/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      232 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/postgres/pgvector.py
+-rw-r--r--   0 zu         (501) staff       (20)     4732 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/docker/app/postgres/postgres.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.361825 phidata-2.0.0.dev9/phi/docker/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      731 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.362241 phidata-2.0.0.dev9/phi/docker/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)       93 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      901 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/app/streamlit/streamlit.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.364035 phidata-2.0.0.dev9/phi/docker/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4871 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)    15125 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/resource/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    21704 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)    14791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/resource/image.py
+-rw-r--r--   0 zu         (501) staff       (20)     5126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/resource/network.py
+-rw-r--r--   0 zu         (501) staff       (20)     1130 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     4785 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/docker/resource/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.364454 phidata-2.0.0.dev9/phi/document/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/document/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      809 2023-07-18 13:44:43.000000 phidata-2.0.0.dev9/phi/document/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.366578 phidata-2.0.0.dev9/phi/document/reader/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/document/reader/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2149 2023-07-18 13:44:43.000000 phidata-2.0.0.dev9/phi/document/reader/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     1442 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/document/reader/json.py
+-rw-r--r--   0 zu         (501) staff       (20)     2108 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/document/reader/pdf.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.367268 phidata-2.0.0.dev9/phi/embedder/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/embedder/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      466 2023-07-18 13:44:43.000000 phidata-2.0.0.dev9/phi/embedder/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      976 2023-07-18 13:44:43.000000 phidata-2.0.0.dev9/phi/embedder/openai.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.367580 phidata-2.0.0.dev9/phi/infra/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/infra/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.368422 phidata-2.0.0.dev9/phi/infra/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/infra/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    13633 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/infra/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      522 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/infra/app/context.py
+-rw-r--r--   0 zu         (501) staff       (20)     1778 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/infra/app/db_app.py
+-rw-r--r--   0 zu         (501) staff       (20)      126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/infra/enums.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.369178 phidata-2.0.0.dev9/phi/infra/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/infra/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6896 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/infra/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     1679 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/infra/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.369455 phidata-2.0.0.dev9/phi/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/k8s/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.370131 phidata-2.0.0.dev9/phi/llm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/llm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      362 2023-07-18 13:44:43.000000 phidata-2.0.0.dev9/phi/llm/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.370799 phidata-2.0.0.dev9/phi/llm/conversation/
+-rw-r--r--   0 zu         (501) staff       (20)       85 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/llm/conversation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11850 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/llm/conversation/conversation.py
+-rw-r--r--   0 zu         (501) staff       (20)     1293 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/llm/conversation/schemas.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.371412 phidata-2.0.0.dev9/phi/llm/history/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/llm/history/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1636 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/llm/history/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     1027 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/llm/history/simple.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.372370 phidata-2.0.0.dev9/phi/llm/knowledge/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/llm/knowledge/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2158 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/llm/knowledge/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      642 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/llm/knowledge/combined.py
+-rw-r--r--   0 zu         (501) staff       (20)      581 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/llm/knowledge/document.py
+-rw-r--r--   0 zu         (501) staff       (20)     1011 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/llm/knowledge/json.py
+-rw-r--r--   0 zu         (501) staff       (20)      991 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/llm/knowledge/pdf.py
+-rw-r--r--   0 zu         (501) staff       (20)     1169 2023-07-18 13:44:43.000000 phidata-2.0.0.dev9/phi/llm/openai.py
+-rw-r--r--   0 zu         (501) staff       (20)     1030 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/llm/schemas.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.373150 phidata-2.0.0.dev9/phi/llm/storage/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-23 16:37:22.000000 phidata-2.0.0.dev9/phi/llm/storage/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      670 2023-07-24 17:38:59.000000 phidata-2.0.0.dev9/phi/llm/storage/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     7930 2023-07-24 17:39:14.000000 phidata-2.0.0.dev9/phi/llm/storage/postgres.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.373416 phidata-2.0.0.dev9/phi/table/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/table/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.373698 phidata-2.0.0.dev9/phi/table/sql/
+-rw-r--r--   0 zu         (501) staff       (20)       41 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/table/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      403 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/table/sql/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.376081 phidata-2.0.0.dev9/phi/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/common.py
+-rw-r--r--   0 zu         (501) staff       (20)     1342 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/defaults.py
+-rw-r--r--   0 zu         (501) staff       (20)      120 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/dttm.py
+-rw-r--r--   0 zu         (501) staff       (20)     1020 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/filesystem.py
+-rw-r--r--   0 zu         (501) staff       (20)     1640 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/git.py
+-rw-r--r--   0 zu         (501) staff       (20)      889 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/json_io.py
+-rw-r--r--   0 zu         (501) staff       (20)      665 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/load_env.py
+-rw-r--r--   0 zu         (501) staff       (20)     1009 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/log.py
+-rw-r--r--   0 zu         (501) staff       (20)     1010 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/pickle.py
+-rw-r--r--   0 zu         (501) staff       (20)      724 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/py_io.py
+-rw-r--r--   0 zu         (501) staff       (20)      589 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/pyproject.py
+-rw-r--r--   0 zu         (501) staff       (20)      962 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/resource_filter.py
+-rw-r--r--   0 zu         (501) staff       (20)      829 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/utils/yaml_io.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.376447 phidata-2.0.0.dev9/phi/vectordb/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:44:43.000000 phidata-2.0.0.dev9/phi/vectordb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      705 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/vectordb/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.376826 phidata-2.0.0.dev9/phi/vectordb/pgvector/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-18 13:44:43.000000 phidata-2.0.0.dev9/phi/vectordb/pgvector/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5652 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/phi/vectordb/pgvector/pgvector.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.377964 phidata-2.0.0.dev9/phi/workspace/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/workspace/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10069 2023-07-24 15:35:53.000000 phidata-2.0.0.dev9/phi/workspace/config.py
+-rw-r--r--   0 zu         (501) staff       (20)      321 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/workspace/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)     1914 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/workspace/helpers.py
+-rw-r--r--   0 zu         (501) staff       (20)    25401 2023-07-24 14:21:57.000000 phidata-2.0.0.dev9/phi/workspace/operator.py
+-rw-r--r--   0 zu         (501) staff       (20)     9063 2023-07-18 13:43:48.000000 phidata-2.0.0.dev9/phi/workspace/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.378411 phidata-2.0.0.dev9/phidata/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev9/phidata/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.379406 phidata-2.0.0.dev9/phidata/airflow/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/airflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      140 2022-10-01 00:05:40.000000 phidata-2.0.0.dev9/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.379652 phidata-2.0.0.dev9/phidata/airflow/operators/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      584 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.381099 phidata-2.0.0.dev9/phidata/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-10-28 00:34:05.000000 phidata-2.0.0.dev9/phidata/app/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.382398 phidata-2.0.0.dev9/phidata/app/airflow/
+-rw-r--r--   0 zu         (501) staff       (20)      385 2022-11-02 02:52:41.000000 phidata-2.0.0.dev9/phidata/app/airflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)   100927 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    30469 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 zu         (501) staff       (20)    30508 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 zu         (501) staff       (20)    30505 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 zu         (501) staff       (20)    30515 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 zu         (501) staff       (20)    30710 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.382861 phidata-2.0.0.dev9/phidata/app/alertmanager/
+-rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev9/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47889 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.383649 phidata-2.0.0.dev9/phidata/app/amundsen/
+-rw-r--r--   0 zu         (501) staff       (20)      398 2023-03-11 17:40:59.000000 phidata-2.0.0.dev9/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    48031 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 zu         (501) staff       (20)    48032 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 zu         (501) staff       (20)    47944 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/amundsen/search.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.383969 phidata-2.0.0.dev9/phidata/app/assistant/
+-rw-r--r--   0 zu         (501) staff       (20)      139 2023-01-15 00:33:10.000000 phidata-2.0.0.dev9/phidata/app/assistant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49912 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/assistant/assistant.py
+-rw-r--r--   0 zu         (501) staff       (20)    30166 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/aws_app.py
+-rw-r--r--   0 zu         (501) staff       (20)    17164 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/base_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.384301 phidata-2.0.0.dev9/phidata/app/cadvisor/
+-rw-r--r--   0 zu         (501) staff       (20)      118 2023-03-11 17:22:33.000000 phidata-2.0.0.dev9/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49678 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.384611 phidata-2.0.0.dev9/phidata/app/databox/
+-rw-r--r--   0 zu         (501) staff       (20)      157 2023-01-15 00:32:07.000000 phidata-2.0.0.dev9/phidata/app/databox/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    86151 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/databox/databox.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.385010 phidata-2.0.0.dev9/phidata/app/db/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2022-03-29 16:28:05.000000 phidata-2.0.0.dev9/phidata/app/db/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3187 2023-01-05 15:43:33.000000 phidata-2.0.0.dev9/phidata/app/db/base_db.py
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-04 16:30:27.000000 phidata-2.0.0.dev9/phidata/app/db/db_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.385336 phidata-2.0.0.dev9/phidata/app/django/
+-rw-r--r--   0 zu         (501) staff       (20)      105 2023-05-18 09:49:43.000000 phidata-2.0.0.dev9/phidata/app/django/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27483 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/django/django_app.py
+-rw-r--r--   0 zu         (501) staff       (20)    30070 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/django/django_backup.py
+-rw-r--r--   0 zu         (501) staff       (20)    17172 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/docker_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.385615 phidata-2.0.0.dev9/phidata/app/elastic/
+-rw-r--r--   0 zu         (501) staff       (20)       71 2022-02-28 02:08:34.000000 phidata-2.0.0.dev9/phidata/app/elastic/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3723 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.385879 phidata-2.0.0.dev9/phidata/app/elasticsearch/
+-rw-r--r--   0 zu         (501) staff       (20)      138 2023-03-11 17:22:33.000000 phidata-2.0.0.dev9/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    48675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.386148 phidata-2.0.0.dev9/phidata/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)      175 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    20266 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/fastapi/fastapi_server.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.386433 phidata-2.0.0.dev9/phidata/app/grafana/
+-rw-r--r--   0 zu         (501) staff       (20)      114 2023-03-11 17:22:33.000000 phidata-2.0.0.dev9/phidata/app/grafana/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49781 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/grafana/grafana.py
+-rw-r--r--   0 zu         (501) staff       (20)      822 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.387299 phidata-2.0.0.dev9/phidata/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)      273 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27093 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/jupyter/jupyter.py
+-rw-r--r--   0 zu         (501) staff       (20)    46942 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 zu         (501) staff       (20)    93432 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.387807 phidata-2.0.0.dev9/phidata/app/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-05-24 02:25:43.000000 phidata-2.0.0.dev9/phidata/app/k8s/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3930 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/k8s/app.py
+-rw-r--r--   0 zu         (501) staff       (20)     1766 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/k8s/dir.py
+-rw-r--r--   0 zu         (501) staff       (20)     6550 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/k8s/url.py
+-rw-r--r--   0 zu         (501) staff       (20)    37830 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/k8s_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.388094 phidata-2.0.0.dev9/phidata/app/mysql/
+-rw-r--r--   0 zu         (501) staff       (20)      151 2023-05-03 15:21:14.000000 phidata-2.0.0.dev9/phidata/app/mysql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49110 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.388355 phidata-2.0.0.dev9/phidata/app/neo4j/
+-rw-r--r--   0 zu         (501) staff       (20)      106 2023-03-11 17:22:33.000000 phidata-2.0.0.dev9/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47856 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.388607 phidata-2.0.0.dev9/phidata/app/nodeexporter/
+-rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev9/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47898 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 zu         (501) staff       (20)    38495 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/phidata_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.388910 phidata-2.0.0.dev9/phidata/app/postgres/
+-rw-r--r--   0 zu         (501) staff       (20)      166 2023-01-15 00:33:00.000000 phidata-2.0.0.dev9/phidata/app/postgres/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    53156 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.389240 phidata-2.0.0.dev9/phidata/app/prometheus/
+-rw-r--r--   0 zu         (501) staff       (20)      126 2023-03-11 17:22:33.000000 phidata-2.0.0.dev9/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49051 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.389519 phidata-2.0.0.dev9/phidata/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12372 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.389902 phidata-2.0.0.dev9/phidata/app/redis/
+-rw-r--r--   0 zu         (501) staff       (20)      144 2023-01-15 00:32:35.000000 phidata-2.0.0.dev9/phidata/app/redis/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/redis/redis.py
+-rw-r--r--   0 zu         (501) staff       (20)    53296 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/redis/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.390303 phidata-2.0.0.dev9/phidata/app/server/
+-rw-r--r--   0 zu         (501) staff       (20)      207 2023-05-18 09:49:43.000000 phidata-2.0.0.dev9/phidata/app/server/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    18424 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/server/api_server.py
+-rw-r--r--   0 zu         (501) staff       (20)    58714 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/server/server_base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.390949 phidata-2.0.0.dev9/phidata/app/spark/
+-rw-r--r--   0 zu         (501) staff       (20)      193 2023-02-07 16:41:27.000000 phidata-2.0.0.dev9/phidata/app/spark/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49424 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/spark/spark_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    17222 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 zu         (501) staff       (20)    17332 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.391189 phidata-2.0.0.dev9/phidata/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)      174 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    20207 2023-06-20 14:11:22.000000 phidata-2.0.0.dev9/phidata/app/streamlit/streamlit_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.391950 phidata-2.0.0.dev9/phidata/app/superset/
+-rw-r--r--   0 zu         (501) staff       (20)      411 2022-11-02 02:52:41.000000 phidata-2.0.0.dev9/phidata/app/superset/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    71570 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/superset/superset_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    22925 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/superset/superset_init.py
+-rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 zu         (501) staff       (20)    22917 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.392492 phidata-2.0.0.dev9/phidata/app/traefik/
+-rw-r--r--   0 zu         (501) staff       (20)      173 2023-01-15 00:32:52.000000 phidata-2.0.0.dev9/phidata/app/traefik/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)   115905 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/traefik/crds.py
+-rw-r--r--   0 zu         (501) staff       (20)    48190 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 zu         (501) staff       (20)    44972 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/app/traefik/router.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.392713 phidata-2.0.0.dev9/phidata/asset/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/asset/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.393437 phidata-2.0.0.dev9/phidata/asset/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/asset/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3210 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 zu         (501) staff       (20)    24787 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/asset/data_asset.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.393905 phidata-2.0.0.dev9/phidata/asset/local/
+-rw-r--r--   0 zu         (501) staff       (20)       71 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/asset/local/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    14564 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/asset/local/file.py
+-rw-r--r--   0 zu         (501) staff       (20)      574 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.394824 phidata-2.0.0.dev9/phidata/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1835 2023-03-13 15:21:09.000000 phidata-2.0.0.dev9/phidata/aws/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)      487 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/aws/args.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.395039 phidata-2.0.0.dev9/phidata/aws/athena/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8186 2023-03-13 15:21:09.000000 phidata-2.0.0.dev9/phidata/aws/athena/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     3168 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/aws/config.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.395154 phidata-2.0.0.dev9/phidata/aws/create/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/create/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.395436 phidata-2.0.0.dev9/phidata/aws/create/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3233 2023-03-13 15:21:09.000000 phidata-2.0.0.dev9/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 zu         (501) staff       (20)     2472 2023-03-13 15:21:09.000000 phidata-2.0.0.dev9/phidata/aws/create/iam/role.py
+-rw-r--r--   0 zu         (501) staff       (20)    23058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/driver.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.395686 phidata-2.0.0.dev9/phidata/aws/enums/
+-rw-r--r--   0 zu         (501) staff       (20)       62 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/enums/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1083 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 zu         (501) staff       (20)      304 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8588 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.396263 phidata-2.0.0.dev9/phidata/aws/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.396496 phidata-2.0.0.dev9/phidata/aws/resource/acm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.396730 phidata-2.0.0.dev9/phidata/aws/resource/athena/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     9127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.396967 phidata-2.0.0.dev9/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.397501 phidata-2.0.0.dev9/phidata/aws/resource/ec2/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21341 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/ec2/security_group.py
+-rw-r--r--   0 zu         (501) staff       (20)     2563 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 zu         (501) staff       (20)    11801 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.398642 phidata-2.0.0.dev9/phidata/aws/resource/ecs/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6140 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    26253 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    19630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 zu         (501) staff       (20)    22397 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 zu         (501) staff       (20)     3614 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.400887 phidata-2.0.0.dev9/phidata/aws/resource/eks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 zu         (501) staff       (20)    30104 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    13731 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 zu         (501) staff       (20)    23785 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 zu         (501) staff       (20)    23742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.401504 phidata-2.0.0.dev9/phidata/aws/resource/elasticache/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    15823 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     6305 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.402924 phidata-2.0.0.dev9/phidata/aws/resource/elb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-07 15:40:41.000000 phidata-2.0.0.dev9/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10727 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 zu         (501) staff       (20)     7994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 zu         (501) staff       (20)     9834 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.403600 phidata-2.0.0.dev9/phidata/aws/resource/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12806 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.403946 phidata-2.0.0.dev9/phidata/aws/resource/glue/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12850 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)     3418 2023-06-20 14:11:22.000000 phidata-2.0.0.dev9/phidata/aws/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.404518 phidata-2.0.0.dev9/phidata/aws/resource/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     9958 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     7653 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 zu         (501) staff       (20)     9828 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.405082 phidata-2.0.0.dev9/phidata/aws/resource/rds/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    36056 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    35380 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 zu         (501) staff       (20)     7990 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.405313 phidata-2.0.0.dev9/phidata/aws/resource/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6472 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.405736 phidata-2.0.0.dev9/phidata/aws/resource/secret/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11398 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 zu         (501) staff       (20)     1007 2023-06-20 14:11:22.000000 phidata-2.0.0.dev9/phidata/aws/resource/secret/reader.py
+-rw-r--r--   0 zu         (501) staff       (20)     3604 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     9688 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/resource/utils.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.406461 phidata-2.0.0.dev9/phidata/aws/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/aws/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21797 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 zu         (501) staff       (20)    24100 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/s3/dataset.py
+-rw-r--r--   0 zu         (501) staff       (20)    14394 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 zu         (501) staff       (20)     7409 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/s3/object.py
+-rw-r--r--   0 zu         (501) staff       (20)    22470 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/aws/worker.py
+-rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.406905 phidata-2.0.0.dev9/phidata/checks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/checks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2790 2023-01-31 22:57:08.000000 phidata-2.0.0.dev9/phidata/checks/check.py
+-rw-r--r--   0 zu         (501) staff       (20)      754 2023-02-03 21:54:28.000000 phidata-2.0.0.dev9/phidata/checks/not_empty.py
+-rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev9/phidata/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.407379 phidata-2.0.0.dev9/phidata/decorators/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev9/phidata/decorators/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      582 2022-02-28 02:08:34.000000 phidata-2.0.0.dev9/phidata/decorators/timer.py
+-rw-r--r--   0 zu         (501) staff       (20)     1110 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/decorators/validate_env.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.408789 phidata-2.0.0.dev9/phidata/docker/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/docker/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1728 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     1645 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/args.py
+-rw-r--r--   0 zu         (501) staff       (20)     4482 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     1166 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/docker/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)      322 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/docker/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8899 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.410094 phidata-2.0.0.dev9/phidata/docker/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/docker/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3804 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)    16440 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/resource/container.py
+-rw-r--r--   0 zu         (501) staff       (20)      932 2023-06-20 14:11:22.000000 phidata-2.0.0.dev9/phidata/docker/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)    14773 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/resource/image.py
+-rw-r--r--   0 zu         (501) staff       (20)     5226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/docker/resource/network.py
+-rw-r--r--   0 zu         (501) staff       (20)     1165 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)    10737 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/resource/utils.py
+-rw-r--r--   0 zu         (501) staff       (20)     4961 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/docker/resource/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.410295 phidata-2.0.0.dev9/phidata/docker/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/docker/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3584 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/utils/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    24179 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/docker/worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.410720 phidata-2.0.0.dev9/phidata/exceptions/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-22 20:24:07.000000 phidata-2.0.0.dev9/phidata/exceptions/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)       47 2022-05-24 18:09:11.000000 phidata-2.0.0.dev9/phidata/exceptions/app.py
+-rw-r--r--   0 zu         (501) staff       (20)       39 2022-04-22 20:24:07.000000 phidata-2.0.0.dev9/phidata/exceptions/task.py
+-rw-r--r--   0 zu         (501) staff       (20)       43 2022-04-25 21:05:27.000000 phidata-2.0.0.dev9/phidata/exceptions/workflow.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.411255 phidata-2.0.0.dev9/phidata/infra/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev9/phidata/infra/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      341 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/infra/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     2466 2023-01-25 22:40:46.000000 phidata-2.0.0.dev9/phidata/infra/args.py
+-rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/infra/config.py
+-rw-r--r--   0 zu         (501) staff       (20)    12048 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/infra/resource.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.412168 phidata-2.0.0.dev9/phidata/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     1986 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/k8s/args.py
+-rw-r--r--   0 zu         (501) staff       (20)     7871 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/config.py
+-rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.412531 phidata-2.0.0.dev9/phidata/k8s/create/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.412643 phidata-2.0.0.dev9/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.412931 phidata-2.0.0.dev9/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3418 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 zu         (501) staff       (20)     2430 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.413037 phidata-2.0.0.dev9/phidata/k8s/create/apps/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.413216 phidata-2.0.0.dev9/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5429 2023-01-24 16:40:47.000000 phidata-2.0.0.dev9/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.413540 phidata-2.0.0.dev9/phidata/k8s/create/common/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      357 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 zu         (501) staff       (20)     1553 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.413651 phidata-2.0.0.dev9/phidata/k8s/create/core/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.414694 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1395 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 zu         (501) staff       (20)     5490 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 zu         (501) staff       (20)     1515 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 zu         (501) staff       (20)     6695 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 zu         (501) staff       (20)     2005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 zu         (501) staff       (20)     1555 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 zu         (501) staff       (20)     4200 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 zu         (501) staff       (20)     2030 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 zu         (501) staff       (20)     4516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.414885 phidata-2.0.0.dev9/phidata/k8s/create/crb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2115 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 zu         (501) staff       (20)    19062 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     5795 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.414991 phidata-2.0.0.dev9/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.415162 phidata-2.0.0.dev9/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:37.000000 phidata-2.0.0.dev9/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2069 2023-01-31 02:29:01.000000 phidata-2.0.0.dev9/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.415272 phidata-2.0.0.dev9/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.415571 phidata-2.0.0.dev9/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1754 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 zu         (501) staff       (20)     1503 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.415700 phidata-2.0.0.dev9/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.415885 phidata-2.0.0.dev9/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.417209 phidata-2.0.0.dev9/phidata/k8s/enums/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 zu         (501) staff       (20)      542 2023-01-31 02:03:51.000000 phidata-2.0.0.dev9/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 zu         (501) staff       (20)      162 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 zu         (501) staff       (20)      762 2023-01-31 02:04:08.000000 phidata-2.0.0.dev9/phidata/k8s/enums/kind.py
+-rw-r--r--   0 zu         (501) staff       (20)     1085 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 zu         (501) staff       (20)      127 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 zu         (501) staff       (20)      753 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/pv.py
+-rw-r--r--   0 zu         (501) staff       (20)      153 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 zu         (501) staff       (20)      171 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 zu         (501) staff       (20)      377 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 zu         (501) staff       (20)      419 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8596 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.417887 phidata-2.0.0.dev9/phidata/k8s/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.417996 phidata-2.0.0.dev9/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.418401 phidata-2.0.0.dev9/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8592 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.418565 phidata-2.0.0.dev9/phidata/k8s/resource/apps/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.418980 phidata-2.0.0.dev9/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10211 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 zu         (501) staff       (20)     1958 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.419286 phidata-2.0.0.dev9/phidata/k8s/resource/core/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.423099 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6602 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 zu         (501) staff       (20)    18530 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 zu         (501) staff       (20)      822 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 zu         (501) staff       (20)     6635 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 zu         (501) staff       (20)     3863 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 zu         (501) staff       (20)     1614 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 zu         (501) staff       (20)    12419 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 zu         (501) staff       (20)     8107 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 zu         (501) staff       (20)     2693 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 zu         (501) staff       (20)     7468 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 zu         (501) staff       (20)      901 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 zu         (501) staff       (20)     1244 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 zu         (501) staff       (20)     6196 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 zu         (501) staff       (20)    18982 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 zu         (501) staff       (20)     8657 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 zu         (501) staff       (20)     2313 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 zu         (501) staff       (20)     4086 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 zu         (501) staff       (20)     4788 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 zu         (501) staff       (20)      890 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 zu         (501) staff       (20)    13397 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 zu         (501) staff       (20)    12690 2023-06-20 14:11:22.000000 phidata-2.0.0.dev9/phidata/k8s/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     4475 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.423242 phidata-2.0.0.dev9/phidata/k8s/resource/meta/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.423602 phidata-2.0.0.dev9/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1058 2023-04-09 17:01:38.000000 phidata-2.0.0.dev9/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 zu         (501) staff       (20)     2739 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.423750 phidata-2.0.0.dev9/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:16.000000 phidata-2.0.0.dev9/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.423936 phidata-2.0.0.dev9/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:42.000000 phidata-2.0.0.dev9/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10026 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.424047 phidata-2.0.0.dev9/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.424368 phidata-2.0.0.dev9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 zu         (501) staff       (20)     6675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.424478 phidata-2.0.0.dev9/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.424645 phidata-2.0.0.dev9/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7198 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 zu         (501) staff       (20)     3415 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)    10127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.424842 phidata-2.0.0.dev9/phidata/k8s/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1864 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/utils/pod.py
+-rw-r--r--   0 zu         (501) staff       (20)    43059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/k8s/worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.424947 phidata-2.0.0.dev9/phidata/llm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev9/phidata/llm/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.425634 phidata-2.0.0.dev9/phidata/llm/duckdb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev9/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4403 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 zu         (501) staff       (20)     3896 2023-04-09 17:01:38.000000 phidata-2.0.0.dev9/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 zu         (501) staff       (20)      920 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 zu         (501) staff       (20)     1194 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 zu         (501) staff       (20)     2177 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/llm/duckdb/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     1063 2023-04-09 17:01:38.000000 phidata-2.0.0.dev9/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.425851 phidata-2.0.0.dev9/phidata/product/
+-rw-r--r--   0 zu         (501) staff       (20)       70 2022-03-13 21:20:10.000000 phidata-2.0.0.dev9/phidata/product/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    29505 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/product/data_product.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.426058 phidata-2.0.0.dev9/phidata/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      445 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/resource/reference.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.426168 phidata-2.0.0.dev9/phidata/table/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/table/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.426569 phidata-2.0.0.dev9/phidata/table/local/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/table/local/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4616 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/table/local/csv.py
+-rw-r--r--   0 zu         (501) staff       (20)    23516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/table/local/local_table.py
+-rw-r--r--   0 zu         (501) staff       (20)     4624 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/table/local/parquet.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.426967 phidata-2.0.0.dev9/phidata/table/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/table/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4673 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/table/s3/csv.py
+-rw-r--r--   0 zu         (501) staff       (20)     4668 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/table/s3/parquet.py
+-rw-r--r--   0 zu         (501) staff       (20)    23064 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.427290 phidata-2.0.0.dev9/phidata/table/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/table/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1752 2023-04-07 15:40:41.000000 phidata-2.0.0.dev9/phidata/table/sql/postgres.py
+-rw-r--r--   0 zu         (501) staff       (20)    35497 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.427858 phidata-2.0.0.dev9/phidata/task/
+-rw-r--r--   0 zu         (501) staff       (20)       79 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/task/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.427963 phidata-2.0.0.dev9/phidata/task/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/aws/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.428161 phidata-2.0.0.dev9/phidata/task/aws/athena/
+-rw-r--r--   0 zu         (501) staff       (20)       81 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2210 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.428457 phidata-2.0.0.dev9/phidata/task/aws/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.428671 phidata-2.0.0.dev9/phidata/task/aws/glue/
+-rw-r--r--   0 zu         (501) staff       (20)      100 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2038 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)     1381 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/decorator.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.428777 phidata-2.0.0.dev9/phidata/task/dev/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/dev/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.428865 phidata-2.0.0.dev9/phidata/task/download/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/download/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.429029 phidata-2.0.0.dev9/phidata/task/download/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2114 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.429430 phidata-2.0.0.dev9/phidata/task/download/url/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/download/url/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4775 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/task/download/url/to_file.py
+-rw-r--r--   0 zu         (501) staff       (20)     3681 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 zu         (501) staff       (20)     8180 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.429537 phidata-2.0.0.dev9/phidata/task/plot/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/plot/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.430305 phidata-2.0.0.dev9/phidata/task/plot/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2541 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/task/plot/sql/query.py
+-rw-r--r--   0 zu         (501) staff       (20)    12300 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/task/python_task.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.430526 phidata-2.0.0.dev9/phidata/task/run/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/run/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.430811 phidata-2.0.0.dev9/phidata/task/run/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4126 2023-04-09 17:01:38.000000 phidata-2.0.0.dev9/phidata/task/run/sql/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     7636 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/task/task.py
+-rw-r--r--   0 zu         (501) staff       (20)     1041 2022-04-25 21:05:27.000000 phidata-2.0.0.dev9/phidata/task/task_relatives.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.430998 phidata-2.0.0.dev9/phidata/task/upload/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/upload/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.431396 phidata-2.0.0.dev9/phidata/task/upload/file/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2039 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 zu         (501) staff       (20)     4721 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.431962 phidata-2.0.0.dev9/phidata/types/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev9/phidata/types/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1023 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/types/airflow.py
+-rw-r--r--   0 zu         (501) staff       (20)     2063 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/types/context.py
+-rw-r--r--   0 zu         (501) staff       (20)      705 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/types/phidata_runtime.py
+-rw-r--r--   0 zu         (501) staff       (20)      101 2022-04-22 20:24:07.000000 phidata-2.0.0.dev9/phidata/types/run_status.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.434810 phidata-2.0.0.dev9/phidata/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev9/phidata/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4779 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/utils/cli_console.py
+-rw-r--r--   0 zu         (501) staff       (20)     2044 2023-01-31 02:10:08.000000 phidata-2.0.0.dev9/phidata/utils/common.py
+-rw-r--r--   0 zu         (501) staff       (20)     1037 2022-11-28 16:47:00.000000 phidata-2.0.0.dev9/phidata/utils/compare.py
+-rw-r--r--   0 zu         (501) staff       (20)     2146 2023-03-13 15:21:10.000000 phidata-2.0.0.dev9/phidata/utils/context.py
+-rw-r--r--   0 zu         (501) staff       (20)     1113 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/utils/dttm.py
+-rw-r--r--   0 zu         (501) staff       (20)      786 2022-06-12 23:07:23.000000 phidata-2.0.0.dev9/phidata/utils/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)     1595 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/utils/env_file.py
+-rw-r--r--   0 zu         (501) staff       (20)     1430 2022-07-31 02:48:39.000000 phidata-2.0.0.dev9/phidata/utils/env_var.py
+-rw-r--r--   0 zu         (501) staff       (20)      661 2022-02-28 02:08:34.000000 phidata-2.0.0.dev9/phidata/utils/filesystem.py
+-rw-r--r--   0 zu         (501) staff       (20)      742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/utils/get_python_objects_from_module.py
+-rw-r--r--   0 zu         (501) staff       (20)      893 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/utils/json_io.py
+-rw-r--r--   0 zu         (501) staff       (20)     1257 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/utils/k8s.py
+-rw-r--r--   0 zu         (501) staff       (20)     1459 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/utils/log.py
+-rw-r--r--   0 zu         (501) staff       (20)      707 2023-01-14 19:22:32.000000 phidata-2.0.0.dev9/phidata/utils/print_table.py
+-rw-r--r--   0 zu         (501) staff       (20)      994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/utils/workspace_path.py
+-rw-r--r--   0 zu         (501) staff       (20)      833 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/utils/yaml_io.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.435417 phidata-2.0.0.dev9/phidata/workflow/
+-rw-r--r--   0 zu         (501) staff       (20)      109 2022-04-15 05:02:36.000000 phidata-2.0.0.dev9/phidata/workflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1855 2022-04-18 19:05:50.000000 phidata-2.0.0.dev9/phidata/workflow/decorator.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.435565 phidata-2.0.0.dev9/phidata/workflow/dev/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev9/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    42342 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/workflow/workflow.py
+-rw-r--r--   0 zu         (501) staff       (20)     1105 2022-04-25 21:05:27.000000 phidata-2.0.0.dev9/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.435929 phidata-2.0.0.dev9/phidata/workspace/
+-rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev9/phidata/workspace/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11316 2023-07-07 23:39:27.000000 phidata-2.0.0.dev9/phidata/workspace/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     8781 2023-07-06 09:54:23.000000 phidata-2.0.0.dev9/phidata/workspace/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.379185 phidata-2.0.0.dev9/phidata.egg-info/
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-25 10:18:41.000000 phidata-2.0.0.dev9/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)    18918 2023-07-25 10:18:41.000000 phidata-2.0.0.dev9/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-25 10:18:41.000000 phidata-2.0.0.dev9/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-25 10:18:41.000000 phidata-2.0.0.dev9/phidata.egg-info/entry_points.txt
+-rw-r--r--   0 zu         (501) staff       (20)      181 2023-07-25 10:18:41.000000 phidata-2.0.0.dev9/phidata.egg-info/requires.txt
+-rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-25 10:18:41.000000 phidata-2.0.0.dev9/phidata.egg-info/top_level.txt
+-rw-r--r--   0 zu         (501) staff       (20)     1676 2023-07-25 10:18:31.000000 phidata-2.0.0.dev9/pyproject.toml
+-rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-25 10:18:41.436598 phidata-2.0.0.dev9/setup.cfg
+-rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev9/setup.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-25 10:18:41.436085 phidata-2.0.0.dev9/tests/
+-rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev9/tests/test_placeholder.py
```

### Comparing `phidata-2.0.0.dev8/LICENSE` & `phidata-2.0.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/PKG-INFO` & `phidata-2.0.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev8
+Version: 2.0.0.dev9
 Summary: A toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev8 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev9 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev8/README.md` & `phidata-2.0.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/api/client.py` & `phidata-2.0.0.dev9/phi/api/client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/api/routes.py` & `phidata-2.0.0.dev9/phi/api/routes.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/api/user.py` & `phidata-2.0.0.dev9/phi/api/user.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/api/workspace.py` & `phidata-2.0.0.dev9/phi/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/api_client.py` & `phidata-2.0.0.dev9/phi/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/app/base.py` & `phidata-2.0.0.dev9/phi/aws/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/app/fastapi/fastapi.py` & `phidata-2.0.0.dev9/phi/aws/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/app/jupyter/jupyter.py` & `phidata-2.0.0.dev9/phi/aws/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/app/qdrant/qdrant.py` & `phidata-2.0.0.dev9/phi/aws/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/app/streamlit/streamlit.py` & `phidata-2.0.0.dev9/phi/aws/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/acm/certificate.py` & `phidata-2.0.0.dev9/phi/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/base.py` & `phidata-2.0.0.dev9/phi/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/cloudformation/stack.py` & `phidata-2.0.0.dev9/phi/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/ec2/security_group.py` & `phidata-2.0.0.dev9/phi/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/ec2/subnet.py` & `phidata-2.0.0.dev9/phi/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/ec2/volume.py` & `phidata-2.0.0.dev9/phi/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/ecs/cluster.py` & `phidata-2.0.0.dev9/phi/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/ecs/container.py` & `phidata-2.0.0.dev9/phi/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/ecs/service.py` & `phidata-2.0.0.dev9/phi/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/ecs/task_definition.py` & `phidata-2.0.0.dev9/phi/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/ecs/volume.py` & `phidata-2.0.0.dev9/phi/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/eks/addon.py` & `phidata-2.0.0.dev9/phi/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/eks/cluster.py` & `phidata-2.0.0.dev9/phi/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/eks/fargate_profile.py` & `phidata-2.0.0.dev9/phi/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/eks/kubeconfig.py` & `phidata-2.0.0.dev9/phi/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/eks/node_group.py` & `phidata-2.0.0.dev9/phi/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/elasticache/cluster.py` & `phidata-2.0.0.dev9/phi/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/elasticache/subnet_group.py` & `phidata-2.0.0.dev9/phi/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/elb/listener.py` & `phidata-2.0.0.dev9/phi/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/elb/load_balancer.py` & `phidata-2.0.0.dev9/phi/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/elb/target_group.py` & `phidata-2.0.0.dev9/phi/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/emr/cluster.py` & `phidata-2.0.0.dev9/phi/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/glue/crawler.py` & `phidata-2.0.0.dev9/phi/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/group.py` & `phidata-2.0.0.dev9/phi/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/iam/policy.py` & `phidata-2.0.0.dev9/phi/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/iam/role.py` & `phidata-2.0.0.dev9/phi/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/rds/db_cluster.py` & `phidata-2.0.0.dev9/phi/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/rds/db_instance.py` & `phidata-2.0.0.dev9/phi/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/rds/db_subnet_group.py` & `phidata-2.0.0.dev9/phi/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/s3/bucket.py` & `phidata-2.0.0.dev9/phi/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/secret/manager.py` & `phidata-2.0.0.dev9/phi/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/secret/reader.py` & `phidata-2.0.0.dev9/phi/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/aws/resource/types.py` & `phidata-2.0.0.dev9/phi/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/base.py` & `phidata-2.0.0.dev9/phi/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/cli/auth_server.py` & `phidata-2.0.0.dev9/phi/cli/auth_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/cli/config.py` & `phidata-2.0.0.dev9/phi/cli/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/cli/console.py` & `phidata-2.0.0.dev9/phi/cli/console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/cli/credentials.py` & `phidata-2.0.0.dev9/phi/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/cli/entrypoint.py` & `phidata-2.0.0.dev9/phi/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/cli/operator.py` & `phidata-2.0.0.dev9/phi/cli/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/cli/settings.py` & `phidata-2.0.0.dev9/phi/cli/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/cli/ws/ws_cli.py` & `phidata-2.0.0.dev9/phi/cli/ws/ws_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/constants.py` & `phidata-2.0.0.dev9/phi/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/api_client.py` & `phidata-2.0.0.dev9/phi/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/app/base.py` & `phidata-2.0.0.dev9/phi/docker/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/app/django/django.py` & `phidata-2.0.0.dev9/phi/docker/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/app/fastapi/fastapi.py` & `phidata-2.0.0.dev9/phi/docker/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/app/jupyter/jupyter.py` & `phidata-2.0.0.dev9/phi/docker/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/app/postgres/postgres.py` & `phidata-2.0.0.dev9/phi/docker/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/app/qdrant/qdrant.py` & `phidata-2.0.0.dev9/phi/docker/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/app/streamlit/streamlit.py` & `phidata-2.0.0.dev9/phi/docker/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/resource/base.py` & `phidata-2.0.0.dev9/phi/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/resource/container.py` & `phidata-2.0.0.dev9/phi/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/resource/group.py` & `phidata-2.0.0.dev9/phi/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/resource/image.py` & `phidata-2.0.0.dev9/phi/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/resource/network.py` & `phidata-2.0.0.dev9/phi/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/resource/types.py` & `phidata-2.0.0.dev9/phi/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/docker/resource/volume.py` & `phidata-2.0.0.dev9/phi/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/document/base.py` & `phidata-2.0.0.dev9/phi/document/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/document/reader/base.py` & `phidata-2.0.0.dev9/phi/document/reader/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/document/reader/pdf.py` & `phidata-2.0.0.dev9/phi/document/reader/pdf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 from pathlib import Path
-from typing import List, Optional
+from typing import List
 
 from phi.document.base import Document
 from phi.document.reader.base import Reader
 from phi.utils.log import logger
 
 
 class PDFReader(Reader):
     """Reader for PDF files"""
 
     def read(self, path: Path) -> List[Document]:
         if not path:
             raise ValueError("No path provided")
 
         if not path.exists():
-            raise FileNotFoundError(f"Could not find PDF: {path}")
+            raise FileNotFoundError(f"Could not find file: {path}")
 
         try:
             from pypdf import PdfReader as DocumentReader  # noqa: F401
         except ImportError:
             raise ImportError("`pypdf` not installed")
 
         try:
             logger.info(f"Reading: {path}")
-            doc_reader = DocumentReader(path)
             doc_name = path.name.split(".")[0]
+            doc_reader = DocumentReader(path)
+
             documents = [
                 Document(
                     name=doc_name,
-                    meta_data={"page": page_number + 1},
+                    meta_data={"page": page_number},
                     content=page.extract_text(),
                 )
-                for page_number, page in enumerate(doc_reader.pages)
+                for page_number, page in enumerate(doc_reader.pages, start=1)
             ]
             if self.chunk:
                 chunked_documents = []
                 for document in documents:
                     chunked_documents.extend(self.chunk_document(document))
                 return chunked_documents
             return documents
         except Exception:
             raise
 
 
-def read_pdfs_from_dir(dir: Path) -> List[Document]:
-    """Read data from a PDF and return a list of Documents"""
-
-    logger.info(f"Reading PDFs in: {dir}")
-    pdfs_to_read: List[Path] = []
-    for pdf in dir.glob("*.pdf"):
-        pdfs_to_read.append(pdf)
-    logger.info(f"Found {len(pdfs_to_read)} PDFs to read")
-
-    reader = PDFReader()
-    parsed_pdfs: List[Document] = []
-    for pdf in pdfs_to_read:
-        # Parse the PDF document
-        documents: Optional[List[Document]] = reader.read(path=pdf)
-        if documents is not None:
-            # Add the parsed documents to the list
-            parsed_pdfs.extend(documents)
-        logger.info(f"Parsed: {str(pdf)}")
-
-    return parsed_pdfs
+# def read_pdfs_from_dir(dir: Path) -> List[Document]:
+#     """Read data from a PDF and return a list of Documents"""
+#
+#     logger.info(f"Reading PDFs in: {dir}")
+#     pdfs_to_read: List[Path] = []
+#     for pdf in dir.glob("*.pdf"):
+#         pdfs_to_read.append(pdf)
+#     logger.info(f"Found {len(pdfs_to_read)} PDFs to read")
+#
+#     reader = PDFReader()
+#     parsed_pdfs: List[Document] = []
+#     for pdf in pdfs_to_read:
+#         # Parse the PDF document
+#         documents: Optional[List[Document]] = reader.read(path=pdf)
+#         if documents is not None:
+#             # Add the parsed documents to the list
+#             parsed_pdfs.extend(documents)
+#         logger.info(f"Parsed: {str(pdf)}")
+#
+#     return parsed_pdfs
```

### Comparing `phidata-2.0.0.dev8/phi/embedder/openai.py` & `phidata-2.0.0.dev9/phi/embedder/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/infra/app/base.py` & `phidata-2.0.0.dev9/phi/infra/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/infra/app/context.py` & `phidata-2.0.0.dev9/phi/infra/app/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/infra/app/db_app.py` & `phidata-2.0.0.dev9/phi/infra/app/db_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/infra/resource/base.py` & `phidata-2.0.0.dev9/phi/infra/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/infra/resource/group.py` & `phidata-2.0.0.dev9/phi/infra/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/llm/conversation/conversation.py` & `phidata-2.0.0.dev9/phi/llm/conversation/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Any, Optional, Dict, Iterator
+from typing import List, Any, Optional, Dict, Iterator, Callable
 
 from pydantic import BaseModel, ConfigDict, field_validator
 
 from phi.document import Document
 from phi.llm.base import LLM
 from phi.llm.schemas import Message, References
 from phi.llm.conversation.schemas import ConversationRow
@@ -24,14 +24,15 @@
     # Monitor conversations on phidata.com
     monitoring: bool = False
 
     # LLM settings
     llm: LLM = OpenAIChat()
     llm_name: Optional[str] = None
     system_prompt: Optional[str] = None
+    user_prompt_function: Optional[Callable[[str, Optional[str], Optional[str]], str]] = None
 
     # User settings
     user_id: str = "anonymous"
     user_persona: Optional[str] = None
     user_data: Optional[Dict[str, Any]] = None
 
     # Usage data
@@ -176,79 +177,89 @@
         return relevant_info
 
     def get_user_prompt(
         self, question: str, references: Optional[str] = None, chat_history: Optional[str] = None
     ) -> str:
         """Build the user prompt given a question, references and chat_history"""
 
-        _user_prompt = "Your task is to answer the following question "
+        if self.user_prompt_function is not None:
+            _generated_user_prompt = self.user_prompt_function(question, references, chat_history)
+            if _generated_user_prompt is not None:
+                return _generated_user_prompt
+
+        _user_prompt = "Your task is to answer the following question"
         if self.user_persona:
-            _user_prompt += f"for a '{self.user_persona}' "
-        _user_prompt += "using the following information:\n"
+            _user_prompt += f" for a '{self.user_persona}'"
         # Add question to the prompt
-        _user_prompt += f"\nQuestion: {question}\n"
+        _user_prompt += f":\nQuestion: {question}\n"
 
         # Add relevant_information to prompt
         if references:
             _user_prompt += f"""
-                You can use the following references if they help you answer the question.
-                If you use the information from the references, please cite them as a bulleted list at the end.
-                START OF REFERENCES
+                You can use the following information if it helps you answer the question.
+                START OF INFORMATION
                 ```
                 {references}
                 ```
-                END OF REFERENCES
+                END OF INFORMATION
                 """
 
         # Add chat history to prompt
         if chat_history:
             _user_prompt += f"""
                 You can use the following chat history if it helps you answer the question.
                 START OF CHAT HISTORY
                 ```
                 {chat_history}
                 ```
                 END OF CHAT HISTORY
                 """
 
-        _user_prompt += "\nRemember, your task is to answer the following question using the provided information:\n"
-        _user_prompt += f"Question: {question}\n"
+        _user_prompt += "\nRemember, your task is to answer the following question:"
+        _user_prompt += f"\nQuestion: {question}"
+        _user_prompt += "\nAnswer: "
 
         # Return the user prompt after removing newlines and indenting
         return "\n".join([line.strip() for line in _user_prompt.split("\n")])
 
     def review(self, question: str) -> Iterator[str]:
         logger.debug(f"Reviewing: {question}")
 
-        # Build the system prompt
+        # -*- Build the system prompt
         system_prompt = self.get_system_prompt()
 
-        # Build the user prompt
+        # -*- Build the user prompt
         references = self.get_references(question=question)
         chat_history = self.history.get_formatted_history() if self.add_history_to_prompt else None
         user_prompt = self.get_user_prompt(question=question, references=references, chat_history=chat_history)
 
-        # Create messages for the LLM
+        # -*- Build messages to send to the LLM
+        # Create system message
         system_message = Message(role="system", content=system_prompt)
+        # Create user message
         user_message = Message(role="user", content=user_prompt)
-        messages: List[Message] = [system_message, user_message]
+        # Create message list
+        messages: List[Message] = [system_message]
+        if self.add_history_to_messages:
+            messages += self.history.chat_history
+        messages += [user_message]
 
         # Add messages to the history
-        # Add the system prompt to the history - only added if this is the first message to the LLM
+        # Add the system prompt to the history - added only if this is the first message to the LLM
         self.history.add_system_prompt(message=system_message)
         # Add user question to the history - this is added to the chat history
         self.history.add_user_question(message=Message(role="user", content=question))
         # Add user prompt to the history - this is added to the llm history
         self.history.add_user_prompt(message=user_message)
         # Add references to the history
         if references:
             self.history.add_references(references=References(question=question, references=references))
 
         # Log messages
-        for message in self.history.chat_history:
+        for message in self.history.llm_history:
             logger.debug(f"{message.role}: {message.content}")
 
         # Generate response
         response = ""
         response_tokens = 0
         for delta in self.llm.streaming_response(messages=[m.model_dump(exclude_none=True) for m in messages]):
             response += delta
@@ -287,9 +298,9 @@
     def end(self) -> None:
         """End the conversation"""
         if self.storage is not None:
             if self.id is not None:
                 self.storage.end_conversation(conversation_id=self.id, user_id=self.user_id)
 
     def monitor(self):
-        logger.debug("Monitoring request")
+        logger.debug("Sending monitoring request")
         pass
```

### Comparing `phidata-2.0.0.dev8/phi/llm/conversation/schemas.py` & `phidata-2.0.0.dev9/phi/llm/conversation/schemas.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/llm/history/base.py` & `phidata-2.0.0.dev9/phi/llm/history/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/llm/history/simple.py` & `phidata-2.0.0.dev9/phi/llm/history/simple.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/llm/knowledge/pdf.py` & `phidata-2.0.0.dev9/phi/llm/knowledge/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from pathlib import Path
-from typing import Union, List, Optional, Iterator
+from typing import List, Optional, Iterator
+
+from pydantic import BaseModel, ConfigDict
 
 from phi.document import Document
-from phi.document.reader.pdf import PDFReader
-from phi.llm.knowledge.base import LLMKnowledgeBase
+from phi.document.reader.base import Reader
 from phi.vectordb import VectorDb
 from phi.utils.log import logger
 
 
-class PDFKnowledgeBase(LLMKnowledgeBase):
-    path: Union[str, Path]
-    reader: PDFReader = PDFReader()
+class LLMKnowledgeBase(BaseModel):
+    """Base class for LLM knowledge base"""
+
+    # Reader to read the documents
+    reader: Optional[Reader] = None
+    # Vector db to store the knowledge base
     vector_db: Optional[VectorDb] = None
+    # Number of relevant documents to return on search
     relevant_documents: int = 5
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     @property
     def document_lists(self) -> Iterator[List[Document]]:
-        """Iterate over PDFs and return a list of document in each PDF
-        Returns:
-            Iterator[List[Document]]: Iterator over List of documents in each PDF
+        """Iterator that yields lists of documents in the knowledge base
+        Each object yielded by the iterator is a list of documents.
         """
+        raise NotImplementedError
 
-        pdf_dir_path: Path = Path(self.path) if isinstance(self.path, str) else self.path
+    def search(self, query: str, relevant_documents: Optional[int] = None) -> List[Document]:
+        """Returns relevant documents matching the query"""
 
-        if pdf_dir_path.exists() and pdf_dir_path.is_dir():
-            for _pdf in pdf_dir_path.glob("*.pdf"):
-                yield self.reader.read(path=_pdf)
-        elif pdf_dir_path.exists() and pdf_dir_path.is_file() and pdf_dir_path.suffix == ".pdf":
-            yield self.reader.read(path=pdf_dir_path)
-
-    def search(self, query: str, num_documents: Optional[int] = None) -> List[Document]:
-        """Return all relevant documents matching the query"""
         if self.vector_db is None:
             logger.warning("No vector db provided")
             return []
 
-        _num_documents = num_documents or self.relevant_documents
+        _num_documents = relevant_documents or self.relevant_documents
         logger.debug(f"Getting {_num_documents} relevant documents for query: {query}")
-        return self.vector_db.search(query=query, num_documents=_num_documents)
+        return self.vector_db.search(query=query, relevant_documents=_num_documents)
 
     def load(self, recreate: bool = False) -> None:
         """Load the knowledge base to vector db"""
+
         if self.vector_db is None:
             logger.warning("No vector db provided")
             return
 
         if recreate:
-            logger.debug("Recreating collection")
+            logger.debug("Deleting collection")
             self.vector_db.delete()
 
         logger.debug("Creating collection")
         self.vector_db.create()
 
         logger.info("Loading knowledge base")
         num_documents = 0
```

### Comparing `phidata-2.0.0.dev8/phi/llm/openai.py` & `phidata-2.0.0.dev9/phi/llm/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/llm/schemas.py` & `phidata-2.0.0.dev9/phi/llm/schemas.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/llm/storage/base.py` & `phidata-2.0.0.dev9/phi/llm/storage/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/llm/storage/postgres.py` & `phidata-2.0.0.dev9/phi/llm/storage/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/common.py` & `phidata-2.0.0.dev9/phi/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/defaults.py` & `phidata-2.0.0.dev9/phi/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/filesystem.py` & `phidata-2.0.0.dev9/phi/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/git.py` & `phidata-2.0.0.dev9/phi/utils/git.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/json_io.py` & `phidata-2.0.0.dev9/phi/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/load_env.py` & `phidata-2.0.0.dev9/phi/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/log.py` & `phidata-2.0.0.dev9/phi/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/pickle.py` & `phidata-2.0.0.dev9/phi/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/py_io.py` & `phidata-2.0.0.dev9/phi/utils/py_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/pyproject.py` & `phidata-2.0.0.dev9/phi/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/resource_filter.py` & `phidata-2.0.0.dev9/phi/utils/resource_filter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/utils/yaml_io.py` & `phidata-2.0.0.dev9/phi/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/vectordb/base.py` & `phidata-2.0.0.dev9/phi/vectordb/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,9 +20,9 @@
         raise NotImplementedError
 
     # @abstractmethod
     # def upsert(self, documents: List[Document]) -> None:
     #     raise NotImplementedError
 
     @abstractmethod
-    def search(self, query: str, num_documents: int = 5) -> List[Document]:
+    def search(self, query: str, relevant_documents: int = 5) -> List[Document]:
         raise NotImplementedError
```

### Comparing `phidata-2.0.0.dev8/phi/vectordb/pgvector/pgvector.py` & `phidata-2.0.0.dev9/phi/vectordb/pgvector/pgvector.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                         content=document.content,
                         embedding=document.embedding,
                         usage=document.usage,
                     )
                     sess.execute(stmt)
                     logger.debug(f"Inserted document: {document.name} ({document.meta_data})")
 
-    def search(self, query: str, num_documents: int = 5) -> List[Document]:
+    def search(self, query: str, relevant_documents: int = 5) -> List[Document]:
         from sqlalchemy.sql.expression import select
 
         query_embedding = self.embedder.get_embedding(query)
         if query_embedding is None:
             logger.error(f"Error getting embedding for Query: {query}")
             return []
 
@@ -118,15 +118,19 @@
             self.table.c.name,
             self.table.c.meta_data,
             self.table.c.content,
             self.table.c.embedding,
             self.table.c.usage,
         ]
 
-        stmt = select(*columns).order_by(self.table.c.embedding.max_inner_product(query_embedding)).limit(num_documents)
+        stmt = (
+            select(*columns)
+            .order_by(self.table.c.embedding.max_inner_product(query_embedding))
+            .limit(relevant_documents)
+        )
         logger.debug(f"Query: {stmt}")
 
         # Get neighbors
         with self.Session() as sess:
             with sess.begin():
                 neighbors = sess.execute(stmt).fetchall() or []
```

### Comparing `phidata-2.0.0.dev8/phi/workspace/config.py` & `phidata-2.0.0.dev9/phi/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/workspace/helpers.py` & `phidata-2.0.0.dev9/phi/workspace/helpers.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/workspace/operator.py` & `phidata-2.0.0.dev9/phi/workspace/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phi/workspace/settings.py` & `phidata-2.0.0.dev9/phi/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/airflow/operators/empty.py` & `phidata-2.0.0.dev9/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/airflow/airflow_base.py` & `phidata-2.0.0.dev9/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/airflow/airflow_flower.py` & `phidata-2.0.0.dev9/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/airflow/airflow_manager.py` & `phidata-2.0.0.dev9/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/airflow/airflow_scheduler.py` & `phidata-2.0.0.dev9/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/airflow/airflow_webserver.py` & `phidata-2.0.0.dev9/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/airflow/airflow_worker.py` & `phidata-2.0.0.dev9/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/alertmanager/alertmanager.py` & `phidata-2.0.0.dev9/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/amundsen/frontend.py` & `phidata-2.0.0.dev9/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/amundsen/metadata.py` & `phidata-2.0.0.dev9/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/amundsen/search.py` & `phidata-2.0.0.dev9/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/assistant/assistant.py` & `phidata-2.0.0.dev9/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/aws_app.py` & `phidata-2.0.0.dev9/phidata/app/aws_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/base_app.py` & `phidata-2.0.0.dev9/phidata/app/base_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/cadvisor/cadvisor.py` & `phidata-2.0.0.dev9/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/databox/databox.py` & `phidata-2.0.0.dev9/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/db/base_db.py` & `phidata-2.0.0.dev9/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/django/django_app.py` & `phidata-2.0.0.dev9/phidata/app/django/django_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/django/django_backup.py` & `phidata-2.0.0.dev9/phidata/app/django/django_backup.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/docker_app.py` & `phidata-2.0.0.dev9/phidata/app/docker_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/elastic/elastic_app.py` & `phidata-2.0.0.dev9/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/elasticsearch/elasticsearch.py` & `phidata-2.0.0.dev9/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/fastapi/fastapi_server.py` & `phidata-2.0.0.dev9/phidata/app/fastapi/fastapi_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/grafana/grafana.py` & `phidata-2.0.0.dev9/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/group.py` & `phidata-2.0.0.dev9/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/jupyter/jupyter.py` & `phidata-2.0.0.dev9/phidata/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/jupyter/jupyter_hub.py` & `phidata-2.0.0.dev9/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/jupyter/jupyter_lab.py` & `phidata-2.0.0.dev9/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/k8s/app.py` & `phidata-2.0.0.dev9/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/k8s/dir.py` & `phidata-2.0.0.dev9/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/k8s/url.py` & `phidata-2.0.0.dev9/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/k8s_app.py` & `phidata-2.0.0.dev9/phidata/app/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/mysql/mysql_db.py` & `phidata-2.0.0.dev9/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/neo4j/neo4j.py` & `phidata-2.0.0.dev9/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/nodeexporter/nodeexporter.py` & `phidata-2.0.0.dev9/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/phidata_app.py` & `phidata-2.0.0.dev9/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/postgres/postgres_db.py` & `phidata-2.0.0.dev9/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/prometheus/prometheus.py` & `phidata-2.0.0.dev9/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/qdrant/qdrant.py` & `phidata-2.0.0.dev9/phidata/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/redis/redis.py` & `phidata-2.0.0.dev9/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/redis/stack.py` & `phidata-2.0.0.dev9/phidata/app/redis/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/server/api_server.py` & `phidata-2.0.0.dev9/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/server/server_base.py` & `phidata-2.0.0.dev9/phidata/app/server/server_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/spark/spark_base.py` & `phidata-2.0.0.dev9/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/spark/spark_driver.py` & `phidata-2.0.0.dev9/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/spark/spark_worker.py` & `phidata-2.0.0.dev9/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/streamlit/streamlit_app.py` & `phidata-2.0.0.dev9/phidata/app/streamlit/streamlit_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/superset/superset_base.py` & `phidata-2.0.0.dev9/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/superset/superset_init.py` & `phidata-2.0.0.dev9/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/superset/superset_webserver.py` & `phidata-2.0.0.dev9/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/superset/superset_worker.py` & `phidata-2.0.0.dev9/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/superset/superset_worker_beat.py` & `phidata-2.0.0.dev9/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/traefik/crds.py` & `phidata-2.0.0.dev9/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/traefik/ingress_route.py` & `phidata-2.0.0.dev9/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/app/traefik/router.py` & `phidata-2.0.0.dev9/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/asset/aws/aws_asset.py` & `phidata-2.0.0.dev9/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/asset/data_asset.py` & `phidata-2.0.0.dev9/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/asset/local/file.py` & `phidata-2.0.0.dev9/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/asset/local/local_asset.py` & `phidata-2.0.0.dev9/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/api_client.py` & `phidata-2.0.0.dev9/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/athena/query.py` & `phidata-2.0.0.dev9/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/config.py` & `phidata-2.0.0.dev9/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/create/iam/eks_admin_role.py` & `phidata-2.0.0.dev9/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/create/iam/role.py` & `phidata-2.0.0.dev9/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/driver.py` & `phidata-2.0.0.dev9/phidata/aws/driver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/enums/manager_status.py` & `phidata-2.0.0.dev9/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/manager.py` & `phidata-2.0.0.dev9/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/acm/certificate.py` & `phidata-2.0.0.dev9/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/athena/query.py` & `phidata-2.0.0.dev9/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/base.py` & `phidata-2.0.0.dev9/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/cloudformation/stack.py` & `phidata-2.0.0.dev9/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/ec2/security_group.py` & `phidata-2.0.0.dev9/phidata/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/ec2/subnet.py` & `phidata-2.0.0.dev9/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/ec2/volume.py` & `phidata-2.0.0.dev9/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/ecs/cluster.py` & `phidata-2.0.0.dev9/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/ecs/container.py` & `phidata-2.0.0.dev9/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/ecs/service.py` & `phidata-2.0.0.dev9/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/ecs/task_definition.py` & `phidata-2.0.0.dev9/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/ecs/volume.py` & `phidata-2.0.0.dev9/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/eks/addon.py` & `phidata-2.0.0.dev9/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/eks/cluster.py` & `phidata-2.0.0.dev9/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/eks/fargate_profile.py` & `phidata-2.0.0.dev9/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/eks/kubeconfig.py` & `phidata-2.0.0.dev9/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/eks/node_group.py` & `phidata-2.0.0.dev9/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/elasticache/cluster.py` & `phidata-2.0.0.dev9/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-2.0.0.dev9/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/elb/listener.py` & `phidata-2.0.0.dev9/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/elb/load_balancer.py` & `phidata-2.0.0.dev9/phidata/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/elb/target_group.py` & `phidata-2.0.0.dev9/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/emr/cluster.py` & `phidata-2.0.0.dev9/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/glue/crawler.py` & `phidata-2.0.0.dev9/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/group.py` & `phidata-2.0.0.dev9/phidata/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/iam/group.py` & `phidata-2.0.0.dev9/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/iam/policy.py` & `phidata-2.0.0.dev9/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/iam/role.py` & `phidata-2.0.0.dev9/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/rds/db_cluster.py` & `phidata-2.0.0.dev9/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/rds/db_instance.py` & `phidata-2.0.0.dev9/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-2.0.0.dev9/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/s3/bucket.py` & `phidata-2.0.0.dev9/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/secret/manager.py` & `phidata-2.0.0.dev9/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/secret/reader.py` & `phidata-2.0.0.dev9/phidata/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/types.py` & `phidata-2.0.0.dev9/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/resource/utils.py` & `phidata-2.0.0.dev9/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/s3/csv_dataset.py` & `phidata-2.0.0.dev9/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/s3/dataset.py` & `phidata-2.0.0.dev9/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/s3/dataset_base.py` & `phidata-2.0.0.dev9/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/s3/object.py` & `phidata-2.0.0.dev9/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/aws/worker.py` & `phidata-2.0.0.dev9/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/base.py` & `phidata-2.0.0.dev9/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/checks/check.py` & `phidata-2.0.0.dev9/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/checks/not_empty.py` & `phidata-2.0.0.dev9/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/constants.py` & `phidata-2.0.0.dev9/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/decorators/timer.py` & `phidata-2.0.0.dev9/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/decorators/validate_env.py` & `phidata-2.0.0.dev9/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/api_client.py` & `phidata-2.0.0.dev9/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/args.py` & `phidata-2.0.0.dev9/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/config.py` & `phidata-2.0.0.dev9/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/enums.py` & `phidata-2.0.0.dev9/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/manager.py` & `phidata-2.0.0.dev9/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/resource/base.py` & `phidata-2.0.0.dev9/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/resource/container.py` & `phidata-2.0.0.dev9/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/resource/group.py` & `phidata-2.0.0.dev9/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/resource/image.py` & `phidata-2.0.0.dev9/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/resource/network.py` & `phidata-2.0.0.dev9/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/resource/types.py` & `phidata-2.0.0.dev9/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/resource/utils.py` & `phidata-2.0.0.dev9/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/resource/volume.py` & `phidata-2.0.0.dev9/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/utils/container.py` & `phidata-2.0.0.dev9/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/docker/worker.py` & `phidata-2.0.0.dev9/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/infra/args.py` & `phidata-2.0.0.dev9/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/infra/config.py` & `phidata-2.0.0.dev9/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/infra/resource.py` & `phidata-2.0.0.dev9/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/api_client.py` & `phidata-2.0.0.dev9/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/args.py` & `phidata-2.0.0.dev9/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/config.py` & `phidata-2.0.0.dev9/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.0.0.dev9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.0.0.dev9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/apps/v1/deployment.py` & `phidata-2.0.0.dev9/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/common/port.py` & `phidata-2.0.0.dev9/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/config_map.py` & `phidata-2.0.0.dev9/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/container.py` & `phidata-2.0.0.dev9/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/namespace.py` & `phidata-2.0.0.dev9/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-2.0.0.dev9/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-2.0.0.dev9/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/secret.py` & `phidata-2.0.0.dev9/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/service.py` & `phidata-2.0.0.dev9/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/service_account.py` & `phidata-2.0.0.dev9/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/volume.py` & `phidata-2.0.0.dev9/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-2.0.0.dev9/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/group.py` & `phidata-2.0.0.dev9/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/kubeconfig.py` & `phidata-2.0.0.dev9/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-2.0.0.dev9/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.0.0.dev9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.0.0.dev9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-2.0.0.dev9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/enums/api_version.py` & `phidata-2.0.0.dev9/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/enums/kind.py` & `phidata-2.0.0.dev9/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/enums/manager_status.py` & `phidata-2.0.0.dev9/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/enums/pv.py` & `phidata-2.0.0.dev9/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/manager.py` & `phidata-2.0.0.dev9/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/base.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/config_map.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/container.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/namespace.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/secret.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/service.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/service_account.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/toleration.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/group.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/kubeconfig.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/types.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/resource/utils.py` & `phidata-2.0.0.dev9/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/utils/pod.py` & `phidata-2.0.0.dev9/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/k8s/worker.py` & `phidata-2.0.0.dev9/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/llm/duckdb/agent.py` & `phidata-2.0.0.dev9/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/llm/duckdb/chain.py` & `phidata-2.0.0.dev9/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/llm/duckdb/connection.py` & `phidata-2.0.0.dev9/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/llm/duckdb/loader.py` & `phidata-2.0.0.dev9/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/llm/duckdb/query.py` & `phidata-2.0.0.dev9/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/llm/duckdb/tool.py` & `phidata-2.0.0.dev9/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/product/data_product.py` & `phidata-2.0.0.dev9/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/table/local/csv.py` & `phidata-2.0.0.dev9/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/table/local/local_table.py` & `phidata-2.0.0.dev9/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/table/local/parquet.py` & `phidata-2.0.0.dev9/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/table/s3/csv.py` & `phidata-2.0.0.dev9/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/table/s3/parquet.py` & `phidata-2.0.0.dev9/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/table/s3/s3_table.py` & `phidata-2.0.0.dev9/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/table/sql/postgres.py` & `phidata-2.0.0.dev9/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/table/sql/sql_table.py` & `phidata-2.0.0.dev9/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/aws/athena/run_query.py` & `phidata-2.0.0.dev9/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/aws/emr/create_cluster.py` & `phidata-2.0.0.dev9/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/aws/emr/delete_cluster.py` & `phidata-2.0.0.dev9/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/aws/glue/start_crawler.py` & `phidata-2.0.0.dev9/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/decorator.py` & `phidata-2.0.0.dev9/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/download/s3/to_file.py` & `phidata-2.0.0.dev9/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/download/url/to_file.py` & `phidata-2.0.0.dev9/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/download/url/to_s3.py` & `phidata-2.0.0.dev9/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/download/url/to_sql.py` & `phidata-2.0.0.dev9/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/plot/sql/query.py` & `phidata-2.0.0.dev9/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/python_task.py` & `phidata-2.0.0.dev9/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/run/sql/query.py` & `phidata-2.0.0.dev9/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/task.py` & `phidata-2.0.0.dev9/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/task_relatives.py` & `phidata-2.0.0.dev9/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/upload/file/to_s3.py` & `phidata-2.0.0.dev9/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/task/upload/file/to_sql.py` & `phidata-2.0.0.dev9/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/types/airflow.py` & `phidata-2.0.0.dev9/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/types/context.py` & `phidata-2.0.0.dev9/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/types/phidata_runtime.py` & `phidata-2.0.0.dev9/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/cli_console.py` & `phidata-2.0.0.dev9/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/common.py` & `phidata-2.0.0.dev9/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/compare.py` & `phidata-2.0.0.dev9/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/context.py` & `phidata-2.0.0.dev9/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/dttm.py` & `phidata-2.0.0.dev9/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/enums.py` & `phidata-2.0.0.dev9/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/env_file.py` & `phidata-2.0.0.dev9/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/env_var.py` & `phidata-2.0.0.dev9/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/filesystem.py` & `phidata-2.0.0.dev9/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/get_python_objects_from_module.py` & `phidata-2.0.0.dev9/phidata/utils/get_python_objects_from_module.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/json_io.py` & `phidata-2.0.0.dev9/phidata/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/k8s.py` & `phidata-2.0.0.dev9/phidata/utils/k8s.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/log.py` & `phidata-2.0.0.dev9/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/print_table.py` & `phidata-2.0.0.dev9/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/workspace_path.py` & `phidata-2.0.0.dev9/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/utils/yaml_io.py` & `phidata-2.0.0.dev9/phidata/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/workflow/decorator.py` & `phidata-2.0.0.dev9/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/workflow/workflow.py` & `phidata-2.0.0.dev9/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/workflow/workflow_relatives.py` & `phidata-2.0.0.dev9/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/workspace/config.py` & `phidata-2.0.0.dev9/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata/workspace/settings.py` & `phidata-2.0.0.dev9/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev8/phidata.egg-info/PKG-INFO` & `phidata-2.0.0.dev9/phidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev8
+Version: 2.0.0.dev9
 Summary: A toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev8 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev9 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev8/phidata.egg-info/SOURCES.txt` & `phidata-2.0.0.dev9/phidata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 phi/docker/resource/network.py
 phi/docker/resource/types.py
 phi/docker/resource/volume.py
 phi/document/__init__.py
 phi/document/base.py
 phi/document/reader/__init__.py
 phi/document/reader/base.py
+phi/document/reader/json.py
 phi/document/reader/pdf.py
 phi/embedder/__init__.py
 phi/embedder/base.py
 phi/embedder/openai.py
 phi/infra/__init__.py
 phi/infra/enums.py
 phi/infra/app/__init__.py
@@ -137,14 +138,17 @@
 phi/llm/conversation/conversation.py
 phi/llm/conversation/schemas.py
 phi/llm/history/__init__.py
 phi/llm/history/base.py
 phi/llm/history/simple.py
 phi/llm/knowledge/__init__.py
 phi/llm/knowledge/base.py
+phi/llm/knowledge/combined.py
+phi/llm/knowledge/document.py
+phi/llm/knowledge/json.py
 phi/llm/knowledge/pdf.py
 phi/llm/storage/__init__.py
 phi/llm/storage/base.py
 phi/llm/storage/postgres.py
 phi/table/__init__.py
 phi/table/sql/__init__.py
 phi/table/sql/base.py
```

### Comparing `phidata-2.0.0.dev8/pyproject.toml` & `phidata-2.0.0.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phidata"
-version = "2.0.0.dev8"
+version = "2.0.0.dev9"
 description = "A toolkit for building applications using OSS"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
```

