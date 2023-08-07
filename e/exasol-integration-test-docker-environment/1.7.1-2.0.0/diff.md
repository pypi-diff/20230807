# Comparing `tmp/exasol_integration_test_docker_environment-1.7.1.tar.gz` & `tmp/exasol_integration_test_docker_environment-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_integration_test_docker_environment-1.7.1.tar", max compression
+gzip compressed data, was "exasol_integration_test_docker_environment-2.0.0.tar", max compression
```

## Comparing `exasol_integration_test_docker_environment-1.7.1.tar` & `exasol_integration_test_docker_environment-2.0.0.tar`

### file list

```diff
@@ -1,239 +1,203 @@
--rw-r--r--   0        0        0     1063 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/LICENSE
--rw-r--r--   0        0        0      737 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/README.rst
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/__init__.py
--rw-r--r--   0        0        0       51 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/abstract_method_exception.py
--rw-r--r--   0        0        0      370 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/certificate_resources/container/Dockerfile
--rw-r--r--   0        0        0     1254 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh
--rwxr-xr-x   0        0        0      570 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/__init__.py
--rw-r--r--   0        0        0      524 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/cli.py
--rw-r--r--   0        0        0       86 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/commands/__init__.py
--rw-r--r--   0        0        0      744 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/commands/health.py
--rw-r--r--   0        0        0     5391 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/__init__.py
--rw-r--r--   0        0        0     1655 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/build_options.py
--rw-r--r--   0        0        0     3106 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py
--rw-r--r--   0        0        0      376 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/push_options.py
--rw-r--r--   0        0        0     1660 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/system_options.py
--rw-r--r--   0        0        0     3634 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/test_environment_options.py
--rw-r--r--   0        0        0     1871 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/termination_handler.py
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.0/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.1/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.10/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.11/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.12/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.163156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.13/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.14/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.15/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.16/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.17/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.18/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.19/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.2/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.20/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.3/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.4/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.6/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.7/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.8/init_db.sh
--rw-r--r--   0        0        0     6440 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.9/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.0/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.1/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.10/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.11/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.12/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.13/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.14/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.15/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.16/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.17/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.2/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.3/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.4/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.5/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.6/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.7/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.8/init_db.sh
--rw-r--r--   0        0        0     7182 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.1.9/init_db.sh
--rw-r--r--   0        0        0     8025 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/8.17.0/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/8.17.0/init_db.sh
--rw-r--r--   0        0        0     8167 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/8.18.1/EXAConf
--rwxr-xr-x   0        0        0      318 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/8.18.1/init_db.sh
--rw-r--r--   0        0        0     2576 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/doctor.py
--rw-r--r--   0        0        0      165 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/__init__.py
--rw-r--r--   0        0        0      544 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/__init__.py
--rw-r--r--   0        0        0     1268 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/api_errors.py
--rw-r--r--   0        0        0     3459 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/build_test_container.py
--rw-r--r--   0        0        0    11905 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/common.py
--rw-r--r--   0        0        0     1328 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/health.py
--rw-r--r--   0        0        0     3567 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/push_test_container.py
--rw-r--r--   0        0        0     6881 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py
--rw-r--r--   0        0        0     7357 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/__init__.py
--rw-r--r--   0        0        0      110 2023-06-19 13:39:19.167156 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/abstract_task_future.py
--rw-r--r--   0        0        0    16982 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/base_task.py
--rw-r--r--   0        0        0     4654 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py
--rw-r--r--   0        0        0      459 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/docker_base_task.py
--rw-r--r--   0        0        0      340 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/docker_parameter.py
--rw-r--r--   0        0        0     1516 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/flavor_task.py
--rw-r--r--   0        0        0      325 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/frozendict_to_dict.py
--rw-r--r--   0        0        0     1007 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/info.py
--rw-r--r--   0        0        0     1165 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py
--rw-r--r--   0        0        0      737 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py
--rw-r--r--   0        0        0     3405 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py
--rw-r--r--   0        0        0      495 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/pickle_target.py
--rw-r--r--   0        0        0     3741 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/ssh_access.py
--rw-r--r--   0        0        0     1261 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/still_running_logger.py
--rw-r--r--   0        0        0     3362 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py
--rw-r--r--   0        0        0     1775 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/task_dependency.py
--rw-r--r--   0        0        0     1055 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py
--rw-r--r--   0        0        0      173 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/task_state.py
--rw-r--r--   0        0        0     4619 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py
--rw-r--r--   0        0        0      282 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/wrong_task_state_exception.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/config/__init__.py
--rw-r--r--   0        0        0      675 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/config/build_config.py
--rw-r--r--   0        0        0     1297 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/config/docker_config.py
--rw-r--r--   0        0        0      440 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/config/log_config.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/__init__.py
--rw-r--r--   0        0        0      656 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/container_info.py
--rw-r--r--   0        0        0      810 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/database_credentials.py
--rw-r--r--   0        0        0      507 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/database_info.py
--rw-r--r--   0        0        0      330 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/docker_network_info.py
--rw-r--r--   0        0        0      508 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/docker_volume_info.py
--rw-r--r--   0        0        0      840 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/environment_info.py
--rw-r--r--   0        0        0       91 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/environment_type.py
--rw-r--r--   0        0        0     1773 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py
--rw-r--r--   0        0        0     1010 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/container/__init__.py
--rw-r--r--   0        0        0      492 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/container/utils.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/__init__.py
--rw-r--r--   0        0        0     2778 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/__init__.py
--rw-r--r--   0        0        0     6144 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py
--rw-r--r--   0        0        0    11405 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py
--rw-r--r--   0        0        0     2977 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py
--rw-r--r--   0        0        0     5074 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py
--rw-r--r--   0        0        0      724 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py
--rw-r--r--   0        0        0     1024 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py
--rw-r--r--   0        0        0     2916 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/__init__.py
--rw-r--r--   0        0        0     3306 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py
--rw-r--r--   0        0        0     3697 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py
--rw-r--r--   0        0        0     2323 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py
--rw-r--r--   0        0        0     1734 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py
--rw-r--r--   0        0        0      659 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py
--rw-r--r--   0        0        0     1846 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py
--rw-r--r--   0        0        0    11297 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py
--rw-r--r--   0        0        0     2224 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py
--rw-r--r--   0        0        0      861 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py
--rw-r--r--   0        0        0     4017 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/image_info.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/__init__.py
--rw-r--r--   0        0        0     2683 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py
--rw-r--r--   0        0        0     1334 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py
--rw-r--r--   0        0        0      160 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/docker_push_parameter.py
--rw-r--r--   0        0        0     2107 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py
--rw-r--r--   0        0        0      800 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py
--rw-r--r--   0        0        0      426 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/required_task_info.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/save/__init__.py
--rw-r--r--   0        0        0     3106 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py
--rw-r--r--   0        0        0     1335 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py
--rw-r--r--   0        0        0      815 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py
--rw-r--r--   0        0        0     1998 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py
--rw-r--r--   0        0        0      371 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/utils.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/networks/__init__.py
--rw-r--r--   0        0        0      478 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/networks/utils.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/volumes/__init__.py
--rw-r--r--   0        0        0      473 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/volumes/utils.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/logging/__init__.py
--rw-r--r--   0        0        0     1111 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py
--rw-r--r--   0        0        0     1587 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py
--rw-r--r--   0        0        0      911 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/__init__.py
--rw-r--r--   0        0        0    13026 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py
--rw-r--r--   0        0        0     3571 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/__init__.py
--rw-r--r--   0        0        0     3485 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py
--rw-r--r--   0        0        0     6359 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/__init__.py
--rw-r--r--   0        0        0      283 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/bucketfs_sync_checker.py
--rw-r--r--   0        0        0     2274 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py
--rw-r--r--   0        0        0     1243 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py
--rw-r--r--   0        0        0     2560 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py
--rw-r--r--   0        0        0      443 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/time_based_bucketfs_sync_waiter.py
--rw-r--r--   0        0        0     8069 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/__init__.py
--rw-r--r--   0        0        0     2186 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py
--rw-r--r--   0        0        0     3021 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py
--rw-r--r--   0        0        0     1128 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py
--rw-r--r--   0        0        0     6010 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py
--rw-r--r--   0        0        0     1737 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/db_version.py
--rw-r--r--   0        0        0     1787 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/__init__.py
--rw-r--r--   0        0        0     1445 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py
--rw-r--r--   0        0        0     1364 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py
--rw-r--r--   0        0        0      831 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py
--rw-r--r--   0        0        0      894 2023-06-19 13:39:19.171157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py
--rw-r--r--   0        0        0      771 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/test_container_parameter.py
--rw-r--r--   0        0        0     4769 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py
--rw-r--r--   0        0        0     5045 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py
--rw-r--r--   0        0        0    10576 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py
--rw-r--r--   0        0        0    15736 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py
--rw-r--r--   0        0        0     2628 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py
--rw-r--r--   0        0        0     4888 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py
--rw-r--r--   0        0        0     2905 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/utils/__init__.py
--rw-r--r--   0        0        0     3362 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/utils/resource_directory.py
--rwxr-xr-x   0        0        0      347 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/main.py
--rw-r--r--   0        0        0      774 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/templates/luigi_log.conf
--rw-r--r--   0        0        0        0 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/__init__.py
--rw-r--r--   0        0        0     2445 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/api_consistency_utils.py
--rw-r--r--   0        0        0     4408 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/api_test_environment.py
--rw-r--r--   0        0        0     2691 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/docker_registry.py
--rw-r--r--   0        0        0     1407 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py
--rw-r--r--   0        0        0     8911 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py
--rw-r--r--   0        0        0      559 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/luigi_utils.py
--rw-r--r--   0        0        0      824 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/spawned_test_environments.py
--rw-r--r--   0        0        0     1988 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/utils.py
--rw-r--r--   0        0        0      331 2023-06-19 13:39:19.175157 exasol_integration_test_docker_environment-1.7.1/ext/01_nodoc
--rw-r--r--   0        0        0     1796 2023-06-19 13:39:19.179157 exasol_integration_test_docker_environment-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     6147 2023-06-19 13:39:19.179157 exasol_integration_test_docker_environment-1.7.1/pytest_itde/__init__.py
--rw-r--r--   0        0        0     3335 2023-06-19 13:39:19.179157 exasol_integration_test_docker_environment-1.7.1/pytest_itde/config.py
--rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 exasol_integration_test_docker_environment-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/LICENSE
+-rw-r--r--   0        0        0      737 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/README.rst
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/__init__.py
+-rw-r--r--   0        0        0       51 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/abstract_method_exception.py
+-rw-r--r--   0        0        0      370 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/certificate_resources/container/Dockerfile
+-rw-r--r--   0        0        0     1254 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh
+-rwxr-xr-x   0        0        0      570 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/__init__.py
+-rw-r--r--   0        0        0      524 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/cli.py
+-rw-r--r--   0        0        0       86 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/commands/__init__.py
+-rw-r--r--   0        0        0      744 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/commands/health.py
+-rw-r--r--   0        0        0     5679 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/__init__.py
+-rw-r--r--   0        0        0     1655 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/build_options.py
+-rw-r--r--   0        0        0     3106 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py
+-rw-r--r--   0        0        0      376 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/push_options.py
+-rw-r--r--   0        0        0     1660 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/system_options.py
+-rw-r--r--   0        0        0     3970 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py
+-rw-r--r--   0        0        0     1871 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/termination_handler.py
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.062673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/init_db.sh
+-rw-r--r--   0        0        0     7180 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/init_db.sh
+-rw-r--r--   0        0        0     8163 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/8.17.0/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/8.17.0/init_db.sh
+-rw-r--r--   0        0        0     8163 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/8.18.1/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/8.18.1/init_db.sh
+-rw-r--r--   0        0        0     2576 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/doctor.py
+-rw-r--r--   0        0        0      165 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/__init__.py
+-rw-r--r--   0        0        0      544 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/__init__.py
+-rw-r--r--   0        0        0     1268 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/api_errors.py
+-rw-r--r--   0        0        0     3459 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py
+-rw-r--r--   0        0        0    11905 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/common.py
+-rw-r--r--   0        0        0     1328 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/health.py
+-rw-r--r--   0        0        0     3567 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py
+-rw-r--r--   0        0        0     6929 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py
+-rw-r--r--   0        0        0     7403 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/__init__.py
+-rw-r--r--   0        0        0      110 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/abstract_task_future.py
+-rw-r--r--   0        0        0    16982 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/base_task.py
+-rw-r--r--   0        0        0     4689 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/db_os_executor.py
+-rw-r--r--   0        0        0     4654 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py
+-rw-r--r--   0        0        0      459 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/docker_base_task.py
+-rw-r--r--   0        0        0      340 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/docker_parameter.py
+-rw-r--r--   0        0        0     1516 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py
+-rw-r--r--   0        0        0      325 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/frozendict_to_dict.py
+-rw-r--r--   0        0        0     1007 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/info.py
+-rw-r--r--   0        0        0     1165 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py
+-rw-r--r--   0        0        0      737 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py
+-rw-r--r--   0        0        0     3445 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py
+-rw-r--r--   0        0        0      495 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/pickle_target.py
+-rw-r--r--   0        0        0     3741 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/ssh_access.py
+-rw-r--r--   0        0        0     1261 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py
+-rw-r--r--   0        0        0     3362 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py
+-rw-r--r--   0        0        0     1775 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py
+-rw-r--r--   0        0        0     1055 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py
+-rw-r--r--   0        0        0      173 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/task_state.py
+-rw-r--r--   0        0        0     4619 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py
+-rw-r--r--   0        0        0      282 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/wrong_task_state_exception.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/config/__init__.py
+-rw-r--r--   0        0        0      675 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/config/build_config.py
+-rw-r--r--   0        0        0     1297 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/config/docker_config.py
+-rw-r--r--   0        0        0      440 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/config/log_config.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/__init__.py
+-rw-r--r--   0        0        0      656 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/container_info.py
+-rw-r--r--   0        0        0      810 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py
+-rw-r--r--   0        0        0      819 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/database_info.py
+-rw-r--r--   0        0        0      330 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/docker_network_info.py
+-rw-r--r--   0        0        0      508 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/docker_volume_info.py
+-rw-r--r--   0        0        0      840 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/environment_info.py
+-rw-r--r--   0        0        0       91 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/environment_type.py
+-rw-r--r--   0        0        0      221 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/ssh_info.py
+-rw-r--r--   0        0        0     1773 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py
+-rw-r--r--   0        0        0     1010 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/container/__init__.py
+-rw-r--r--   0        0        0      704 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/container/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/__init__.py
+-rw-r--r--   0        0        0     2778 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/__init__.py
+-rw-r--r--   0        0        0     6144 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py
+-rw-r--r--   0        0        0    11405 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py
+-rw-r--r--   0        0        0     2977 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py
+-rw-r--r--   0        0        0     5074 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py
+-rw-r--r--   0        0        0      724 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py
+-rw-r--r--   0        0        0     1024 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py
+-rw-r--r--   0        0        0     2916 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/__init__.py
+-rw-r--r--   0        0        0     3306 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py
+-rw-r--r--   0        0        0     3697 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py
+-rw-r--r--   0        0        0     2323 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py
+-rw-r--r--   0        0        0     1734 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py
+-rw-r--r--   0        0        0      659 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py
+-rw-r--r--   0        0        0     1846 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py
+-rw-r--r--   0        0        0    11297 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py
+-rw-r--r--   0        0        0     2224 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py
+-rw-r--r--   0        0        0      861 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py
+-rw-r--r--   0        0        0     4017 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/__init__.py
+-rw-r--r--   0        0        0     2683 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py
+-rw-r--r--   0        0        0     1334 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py
+-rw-r--r--   0        0        0      160 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_push_parameter.py
+-rw-r--r--   0        0        0     2107 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py
+-rw-r--r--   0        0        0      800 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py
+-rw-r--r--   0        0        0      426 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/required_task_info.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/save/__init__.py
+-rw-r--r--   0        0        0     3106 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py
+-rw-r--r--   0        0        0     1335 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py
+-rw-r--r--   0        0        0      815 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py
+-rw-r--r--   0        0        0     1998 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py
+-rw-r--r--   0        0        0      371 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/networks/__init__.py
+-rw-r--r--   0        0        0      478 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/networks/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/volumes/__init__.py
+-rw-r--r--   0        0        0      473 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/volumes/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/logging/__init__.py
+-rw-r--r--   0        0        0     1111 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py
+-rw-r--r--   0        0        0     1587 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py
+-rw-r--r--   0        0        0      911 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/__init__.py
+-rw-r--r--   0        0        0    10046 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py
+-rw-r--r--   0        0        0     3571 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/__init__.py
+-rw-r--r--   0        0        0     3485 2023-08-07 08:29:36.066673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py
+-rw-r--r--   0        0        0     6315 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/__init__.py
+-rw-r--r--   0        0        0      283 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/bucketfs_sync_checker.py
+-rw-r--r--   0        0        0     2426 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py
+-rw-r--r--   0        0        0     1352 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py
+-rw-r--r--   0        0        0     2567 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py
+-rw-r--r--   0        0        0      443 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/time_based_bucketfs_sync_waiter.py
+-rw-r--r--   0        0        0     8643 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/__init__.py
+-rw-r--r--   0        0        0     2421 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py
+-rw-r--r--   0        0        0     3693 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py
+-rw-r--r--   0        0        0     1128 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py
+-rw-r--r--   0        0        0     6067 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py
+-rw-r--r--   0        0        0     1737 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py
+-rw-r--r--   0        0        0     1787 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/__init__.py
+-rw-r--r--   0        0        0     1517 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py
+-rw-r--r--   0        0        0     1349 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py
+-rw-r--r--   0        0        0      831 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py
+-rw-r--r--   0        0        0      894 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py
+-rw-r--r--   0        0        0      771 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/test_container_parameter.py
+-rw-r--r--   0        0        0     1928 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/ports.py
+-rw-r--r--   0        0        0     4769 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py
+-rw-r--r--   0        0        0     5149 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py
+-rw-r--r--   0        0        0     2338 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/shell_variables.py
+-rw-r--r--   0        0        0    10576 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py
+-rw-r--r--   0        0        0    18205 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py
+-rw-r--r--   0        0        0     2628 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py
+-rw-r--r--   0        0        0     5378 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py
+-rw-r--r--   0        0        0     2905 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/utils/__init__.py
+-rw-r--r--   0        0        0     3362 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py
+-rwxr-xr-x   0        0        0      347 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/main.py
+-rw-r--r--   0        0        0      774 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/templates/luigi_log.conf
+-rw-r--r--   0        0        0        0 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/__init__.py
+-rw-r--r--   0        0        0     2445 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py
+-rw-r--r--   0        0        0     3904 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/api_test_environment.py
+-rw-r--r--   0        0        0     2704 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/docker_registry.py
+-rw-r--r--   0        0        0     1455 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py
+-rw-r--r--   0        0        0     8951 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py
+-rw-r--r--   0        0        0      559 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/luigi_utils.py
+-rw-r--r--   0        0        0      824 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py
+-rw-r--r--   0        0        0     1113 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/utils.py
+-rw-r--r--   0        0        0      331 2023-08-07 08:29:36.070673 exasol_integration_test_docker_environment-2.0.0/ext/01_nodoc
+-rw-r--r--   0        0        0     1796 2023-08-07 08:29:36.074673 exasol_integration_test_docker_environment-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6922 2023-08-07 08:29:36.074673 exasol_integration_test_docker_environment-2.0.0/pytest_itde/__init__.py
+-rw-r--r--   0        0        0     3402 2023-08-07 08:29:36.074673 exasol_integration_test_docker_environment-2.0.0/pytest_itde/config.py
+-rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 exasol_integration_test_docker_environment-2.0.0/PKG-INFO
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/LICENSE` & `exasol_integration_test_docker_environment-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/README.rst` & `exasol_integration_test_docker_environment-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/commands/health.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/commands/health.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,21 @@
     "--bucketfs-port-forward",
     type=int,
     default=None,
     show_default=True,
     help="Host port to which the BucketFS port gets forwarded",
 )
 @click.option(
+    "--ssh-port-forward",
+    type=int,
+    default=None,
+    show_default=True,
+    help="Host port to which the SSH port gets forwarded. If not specified then ITDE selects a random free port.",
+)
+@click.option(
     "--db-mem-size",
     type=str,
     default="2 GiB",
     show_default=True,
     help="The main memory used by the database. Format <number> <unit>, e.g. 1 GiB. The minimum size is 1 GB, below that the database will not start.",
 )
 @click.option(
@@ -79,14 +86,15 @@
 @add_options([tempory_base_directory_option])
 @add_options(system_options)
 @add_options(luigi_logging_options)
 def spawn_test_environment(
         environment_name: str,
         database_port_forward: Optional[int],
         bucketfs_port_forward: Optional[int],
+        ssh_port_forward: Optional[int],
         db_mem_size: str,
         db_disk_size: str,
         nameserver: Tuple[str, ...],
         docker_runtime: Optional[str],
         docker_db_image_version: str,
         docker_db_image_name: str,
         db_os_access: Optional[str],
@@ -113,14 +121,15 @@
     """
     with TerminationHandler():
         try:
             api.spawn_test_environment(
                 environment_name,
                 database_port_forward,
                 bucketfs_port_forward,
+                ssh_port_forward,
                 db_mem_size,
                 db_disk_size,
                 nameserver,
                 docker_runtime,
                 docker_db_image_version,
                 docker_db_image_name,
                 db_os_access,
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/build_options.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/build_options.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/system_options.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/system_options.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/options/test_environment_options.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import click
 from exasol_integration_test_docker_environment \
     .lib.test_environment.parameter \
     .docker_db_test_environment_parameter \
     import DbOsAccess
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.ports import Ports
 
 test_environment_options = [
     click.option('--environment-type', type=click.Choice(['docker_db', 'external_db']), default="""docker_db""",
                  show_default=True,
                  help="""Environment type for tests."""),
     click.option('--max_start_attempts', type=int, default=2,
                  show_default=True,
@@ -34,18 +36,22 @@
     click.option('--additional-db-parameter', '-p', type=str, multiple=True,
                  help="""Additional database parameter which will be injected to EXAConf. Value should have format '-param=value'.""")
 ]
 
 external_db_options = [
     click.option('--external-exasol-db-host', type=str,
                  help="""Host name or IP of external Exasol DB, needs to be set if --environment-type=external_db"""),
-    click.option('--external-exasol-db-port', type=int, default=8563,
+    click.option('--external-exasol-db-port', type=int,
+                 default=Ports.external.database,
                  help="""Database port of external Exasol DB, needs to be set if --environment-type=external_db"""),
-    click.option('--external-exasol-bucketfs-port', type=int, default=6583,
+    click.option('--external-exasol-bucketfs-port', type=int,
+                 default=Ports.external.bucketfs,
                  help="""Bucketfs port of external Exasol DB, needs to be set if --environment-type=external_db"""),
+    click.option('--external-exasol-ssh-port', type=int,
+                 help="""SSH port of external Exasol DB, needs to be set if --environment-type=external_db"""),
     click.option('--external-exasol-db-user', type=str,
                  help="""User for external Exasol DB, needs to be set if --environment-type=external_db"""),
     click.option('--external-exasol-db-password', type=str,
                  help="""Database Password for external Exasol DB"""),
     click.option('--external-exasol-bucketfs-write-password', type=str,
                  help="""BucketFS write Password for external Exasol DB"""),
     click.option('--external-exasol-xmlrpc-host', type=str,
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/cli/termination_handler.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/cli/termination_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 [Global]
     Revision = 14
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
     LicenseFile = /exa/etc/license.xml
     CoredPort = 10001
-    SSHPort = 22
+    SSHPort = {{ ssh_port }}
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = VFdOQ2ZVZExoRGZqb21ZVzpWWVR0d0NXYVh6am9TckhmeGdnQ3pwU2pFSktOTXlqUHNMclhQU0drWHdld2xDZndXeFFORU1rVnNFSGN4c2Jp
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
     ConfVersion = {{ db_version }}
     OSVersion = {{ db_version }}
     REVersion = {{ db_version }}
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
     [[exadbadm]]
@@ -57,39 +69,40 @@
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
         AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
         AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = 02F4E2AF9C294CABA0A119A89AC60B44EC95D19C
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,39 +113,42 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
 # An EXASOL database
 [DB : DB1]
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
+    EnableAuditing = True
+    BuiltinScriptLanguageName = ScriptLanguages-release-standard-exasol-7.1.0-1.1.0
+    AutoStart = True
     # Additional db parameters
     {% if additional_db_parameters %}
     Params = {{ additional_db_parameters }}
     {% endif %}
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
@@ -148,30 +164,32 @@
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = c3RxWjRxWUFpZUFQblEyc0p2djZUM0VZamVZa1M0bUs=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
+        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/ScriptLanguages/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -180,7 +198,11 @@
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = jdbc-adapter
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = cloud_data_remote_volume
+    RemoteLogRotationPrefix = Logs
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/8.18.1/EXAConf`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,124 @@
 [Global]
-    Revision = 14
+    Revision = 17
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
-    LicenseFile = /exa/etc/license.xml
-    CoredPort = 10001
-    SSHPort = 22
+    LicenseFile = /exa/etc/license.exasol_license
+    CoredPort = 325
+    SSHPort = {{ ssh_port }}
+    IssueTracker = Jira
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = bVNQU0lRT0dhQWhmck5kZDpjU3RwUUJsZkxxalhKTUVpbkVXVHBNd1ZRQlpkenpzTlF5VllxeGNBd3ZPY1JRQUZhQ3VZWGdDcXZLR0p3SWd4
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
-    ConfVersion = {{ db_version }}
-    OSVersion = {{ db_version }}
-    REVersion = {{ db_version }}
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
+    # The meta package name, which was installed by C4 to run this system.
+    MetaPackage = none
+    ConfVersion = 8.29.2
+    OSVersion = 8.29.2
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
+    # Cored only accepts incomming messages from privileged ports (port number less than 1024).
+    CoredUsePrivilegedPorts = True
+    # Cored only accepts incomming messages from its own subnet.
+    CoredAllowOnlySameSubnet = True
+    # Which subnets Cored will allow messages from. Each subnet must be sepparated by a comma.
+    # A subnet is either an IPv4 or IPv6 address in CIDR notation.
+    CoredSubnets =
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
+    [[exaadm]]
+        ID = 499
     [[exadbadm]]
-        ID = 1001
+        ID = 498
     [[exastoradm]]
-        ID = 1002
+        ID = 497
     [[exabfsadm]]
-        ID = 1003
-    [[exaadm]]
-        ID = 1004
+        ID = 496
+    [[exasaasadm]]
+        ID = 495
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
-        AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AdditionalGroups = exausers, exaadm, exadbadm, exastoradm, exabfsadm, exasaasadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
-        AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
+        AdditionalGroups = exaadm, exadbadm, exastoradm, exabfsadm, exasaasadm
+    [[exasaasusr]]
+        ID = 499
+        Group = exausers
+        LoginEnabled = False
+        AdditionalGroups = exasaasadm,
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = F0EA64D47F374A00B0530772981C559EE1C59086
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,78 +129,94 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
+# RemoteLogging : None/None
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = None
+    RemoteLogRotationPrefix = None
+
 # An EXASOL database
 [DB : DB1]
+    # Unique id of this database.
+    ID = aCbUZhU3R8eEc0UIDS7wQw
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
-    # Additional db parameters
+    EnableAuditing = True
+    BuiltinScriptLanguageName = slc-6.0.0-c4-5-standard-EXASOL-8.0.0/ScriptLanguages-standard-EXASOL-8.0.0-slc-v6.0.0-PB5EHDLN
+    AutoStart = True
     {% if additional_db_parameters %}
-    Params = {{ additional_db_parameters }}
+    Params = -sandboxCHROOT=/opt/exasol/cos-8.29.2/sbin/nsexec_chroot {{ additional_db_parameters }}
+    {% else %}
+    Params = -sandboxCHROOT=/opt/exasol/cos-8.29.2/sbin/nsexec_chroot
     {% endif %}
+
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
         BucketFS = bfsdefault
         # Bucket that contains the JDBC driver
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/jdbc
+        # Additional URLs used to search for JDBC drivers, like: bucketfs://bfs2/bucket3/jdbcdir or file:///exa/etc/jdbc_drivers.
+        AdditionalURLs =
     # Oracle driver configuration
     [[Oracle]]
         # BucketFS that contains the JDBC drivers
         BucketFS = bfsdefault
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = bDRYa3pCNXRwaW9OR3k2NjJ2TGpyQ3YweXZEOVUyanQ=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -179,8 +224,8 @@
 
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
-        Name = jdbc-adapter
+        Name = jdbc-adapter
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/docker_db_config/8.17.0/EXAConf`

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,124 @@
 [Global]
-    Revision = 14
+    Revision = 17
     Checksum = COMMIT
     ClusterName = cl4
     Platform = Docker
-    LicenseFile = /exa/etc/license.xml
-    CoredPort = 10001
-    SSHPort = 22
+    LicenseFile = /exa/etc/license.exasol_license
+    CoredPort = 325
+    SSHPort = {{ ssh_port }}
+    IssueTracker = Jira
     XMLRPCPort = 443
-    AuthenticationToken = WG9JQkZYb0R5T1pIcWZPWTpyUHFsR3V6QUFkV1FQbHZmdm91cXJDYmNQTFl4eE1vRlZ6VnhxamdxYnpxUGRkZEhtR2NJaVVGbEpsb2NnbnRZ
+    WebUIBackendPort = 4444
+    WebUIDomain = exacluster.local
+    EnableLoadBalancer = False
+    AuthenticationToken = bVNQU0lRT0dhQWhmck5kZDpjU3RwUUJsZkxxalhKTUVpbkVXVHBNd1ZRQlpkenpzTlF5VllxeGNBd3ZPY1JRQUZhQ3VZWGdDcXZLR0p3SWd4
     # List of networks for this cluster: 'private' is mandatory, 'public' is optional.
     Networks = private
     # Comma-separated list of nameservers for this cluster.
-    NameServers = {{ name_servers }} 
+    NameServers = {{ name_servers }}
+    # Path to c4 unix domain socket, used for deployments of new clusters and nodes.
+    C4Socket = /var/run/c4_socket
     Timezone = Europe/Berlin
+    LicenseRAWMEMWarnThreshold = 80
     # Nr. of hugepages ('0' = disabled, 'host' = manually configured on the host, 'auto' = set automatically based on DB config)
     Hugepages = 0
-    ConfVersion = {{ db_version }}
-    OSVersion = {{ db_version }}
-    REVersion = {{ db_version }}
+    StorageConnectionThreads = 16
+    StorageMaxConnections = 1024
+    # The meta package name, which was installed by C4 to run this system.
+    MetaPackage = none
+    ConfVersion = 8.28.0
+    OSVersion = 8.28.0
     DBVersion = {{ db_version }}
-    ImageVersion = {{ image_version }}
+    ImageVersion = {{ db_version }}
+    # Cored only accepts incomming messages from privileged ports (port number less than 1024).
+    CoredUsePrivilegedPorts = True
+    # Cored only accepts incomming messages from its own subnet.
+    CoredAllowOnlySameSubnet = True
+    # Which subnets Cored will allow messages from. Each subnet must be sepparated by a comma.
+    # A subnet is either an IPv4 or IPv6 address in CIDR notation.
+    CoredSubnets =
 
 # SSL options
 [SSL]
     # The SSL certificate, private key and CA for all EXASOL services
     Cert = {{ certificate_dir }}/cert.crt
     CertKey = {{ certificate_dir }}/cert.key
     CertAuth = {{ certificate_dir }}/rootCA.crt
+    # Options to verify certificates: none, optional, required
+    CertVerify = none
+    # Domain name in the certifcate
+    CertDomainName =
 
 # Docker related options
 [Docker]
     # The directory that contains all data related to this docker cluster
     # (except for mapped devices)
     RootDir = /exa/etc
     # The EXASOL docker image used for all containers of this cluster
     Image = exasol/docker-db:latest
     # The type of storage devices for this cluster: 'block' or 'file'
     DeviceType = file
     # Comma-separated list of volumes to be mounted in all containers (e. g. '/mnt/my_data:/exa/my_data:rw' )
     # These user-defined volumes are mounted additionally to the internal ones (like the node root volume)
-    AdditionalVolumes = 
+    AdditionalVolumes =
 
 [Groups]
     [[root]]
         ID = 0
     [[exausers]]
         ID = 500
+    [[exaadm]]
+        ID = 499
     [[exadbadm]]
-        ID = 1001
+        ID = 498
     [[exastoradm]]
-        ID = 1002
+        ID = 497
     [[exabfsadm]]
-        ID = 1003
-    [[exaadm]]
-        ID = 1004
+        ID = 496
+    [[exasaasadm]]
+        ID = 495
 
 [Users]
     [[root]]
         ID = 0
         Group = root
         LoginEnabled = True
-        AdditionalGroups = exausers, exadbadm, exastoradm, exabfsadm, exaadm
+        AdditionalGroups = exausers, exaadm, exadbadm, exastoradm, exabfsadm, exasaasadm
+        AuthorizedKeys = {{ authorized_keys }}
     [[exadefusr]]
         ID = 500
         Group = exausers
         LoginEnabled = False
-        AdditionalGroups = exadbadm, exastoradm, exabfsadm, exaadm
+        AdditionalGroups = exaadm, exadbadm, exastoradm, exabfsadm, exasaasadm
+    [[exasaasusr]]
+        ID = 499
+        Group = exausers
+        LoginEnabled = False
+        AdditionalGroups = exasaasadm,
 
 [Node : 11]
-    PrivateNet = {{private_network}}
-    PublicNet = 
+    PrivateNet = {{ private_network }}
+    PublicNet =
     Name = n11
-    UUID = A5F8F92113A34BA4B0A48D5397423BBA5CF95161
+    # Affinity decides how this node is used in the cluster. i.e, the possibility to become master
+    Affinity = 11
+    UUID = F0EA64D47F374A00B0530772981C559EE1C59086
     DockerVolume = n11
-    # Ports to be exposed (container : host)
-    ExposedPorts = 8888:8899, 6583:6594
     [[Disk : disk1]]
         Component = exastorage
         Devices = dev.1
         Mapping = dev.1:/exa/data/storage
 
 # Global EXAStorage options
 [EXAStorage]
     # Enable or disable background recovery / data restoration (does not affect on-demand recovery)
     BgRecEnabled = True
     # Max. throughput for background recovery / data restoration (in MiB/s)
-    BgRecLimit = 
+    BgRecLimit =
     # Space usage threshold (in percent, per node) for sending a warning
     SpaceWarnThreshold = 90
 
 # An EXAStorage volume
 [EXAVolume : DataVolume1]
     # Type of volume: 'data' | 'archive'
     Type = data
@@ -100,78 +129,94 @@
     Disk = disk1
     # Comma-separated list of node IDs for this volume (put dedicated redundancy nodes at the end, if any)
     Nodes = 11
     # OPTIONAL: Nr. of master nodes for this volume. Remaining nodes will be used for redundancy only.
     NumMasterNodes = 1
     # Desired redundancy for this volume
     Redundancy = 1
+    BlockSize = 4 KiB
+    StripeSize = 256 KiB
     # User and group IDs that own this volume (e. g. '1000:1005')
     Owner = 500 : 500
     Permissions = rwx
-    BlockSize = 4 KiB
-    StripeSize = 256 KiB
     # OPTIONAL: shared volumes can be opened (for writing) by multiple clients simultaneously
     Shared = True
     # OPTIONAL: I/O priority (0 = highest, 20 = lowest)
     Priority = 10
 
+# RemoteLogging : None/None
+[Logging]
+    LogRotationTypes = local,
+    RemoteLogRotationVolume = None
+    RemoteLogRotationPrefix = None
+
 # An EXASOL database
 [DB : DB1]
+    # Unique id of this database.
+    ID = aCbUZhU3R8eEc0UIDS7wQw
     # Version nr. of this database.
-    Version = {{db_version}}
+    Version = {{ db_version }}
     # Memory size over all nodes (e. g. '1 TiB').
     MemSize = {{ mem_size }}
-    Port = 8888
+    Port = {{ db_port }}
     # User and group IDs that own this database (e. g. '1000:1005').
     Owner = 500 : 500
     # Comma-separated list of node IDs for this DB (put reserve nodes at the end, if any).
     Nodes = 11
     # Nr. of initially active nodes for this DB. The remaining nodes will be reserve nodes.
     NumActiveNodes = 1
     # Name of the data volume to be used by this database.
     DataVolume = DataVolume1
-    # Additional db parameters
+    EnableAuditing = True
+    BuiltinScriptLanguageName = slc-6.0.0-c4-5-standard-EXASOL-8.0.0/ScriptLanguages-standard-EXASOL-8.0.0-slc-v6.0.0-PB5EHDLN
+    AutoStart = True
     {% if additional_db_parameters %}
-    Params = {{ additional_db_parameters }}
+    Params = -sandboxCHROOT=/opt/exasol/cos-8.28.0/sbin/nsexec_chroot {{ additional_db_parameters }}
+    {% else %}
+    Params = -sandboxCHROOT=/opt/exasol/cos-8.28.0/sbin/nsexec_chroot
     {% endif %}
+
     # JDBC driver configuration
     [[JDBC]]
         # BucketFS that contains the JDBC driver
         BucketFS = bfsdefault
         # Bucket that contains the JDBC driver
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/jdbc
+        # Additional URLs used to search for JDBC drivers, like: bucketfs://bfs2/bucket3/jdbcdir or file:///exa/etc/jdbc_drivers.
+        AdditionalURLs =
     # Oracle driver configuration
     [[Oracle]]
         # BucketFS that contains the JDBC drivers
         BucketFS = bfsdefault
         # Bucket that contains the JDBC drivers
         Bucket = default
         # Directory within the bucket that contains the drivers
         Dir = drivers/oracle
 
 # The default BucketFS (auto-generated)
 [BucketFS : bfsdefault]
-    Owner = 500:500
+    Owner = 500 : 500
     # HTTP port number (0 = disabled)
-    HttpPort = 6583
+    HttpPort = {{ bucketfs_port }}
     # HTTPS port number (0 = disabled)
     HttpsPort = 0
-    SyncKey = OGhvcmxrTnluTlFrZTV3RVBTWG5Idlc4bkVMQUNxcWs=
+    SyncKey = bDRYa3pCNXRwaW9OR3k2NjJ2TGpyQ3YweXZEOVUyanQ=
     SyncPeriod = 30000
+    mode = rsync
+    bucketvolume = None
     # The default bucket (auto-generated)
     [[Bucket : default]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
         Name = default
-        AdditionalFiles = EXAClusterOS:/usr/opt/EXASuite-7/EXAClusterOS-{{db_version}}/var/clients/packages/ScriptLanguages-*, EXASolution-{{db_version}}:/usr/opt/EXASuite-7/EXASolution-{{db_version}}/bin/udf/*
 
     [[Bucket : myudfs]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
@@ -179,8 +224,8 @@
 
     [[Bucket : jdbc_adapter]]
         # ReadPasswd is "read" (without quotes)
         ReadPasswd = cmVhZAo=
         # WritePasswd is "write" (without quotes)
         WritePasswd = d3JpdGU=
         Public = True
-        Name = jdbc-adapter
+        Name = jdbc-adapter
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/doctor.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/doctor.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/__init__.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/api_errors.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/api_errors.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/build_test_container.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/common.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/common.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/health.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/health.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/push_test_container.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 
 @cli_function
 def spawn_test_environment(
         environment_name: str,
         database_port_forward: Optional[int] = None,
         bucketfs_port_forward: Optional[int] = None,
+        ssh_port_forward: Optional[int] = None,
         db_mem_size: str = "2 GiB",
         db_disk_size: str = "2 GiB",
         nameserver: Tuple[str, ...] = tuple(),
         docker_runtime: Optional[str] = None,
         docker_db_image_version: str = LATEST_DB_VERSION,
         docker_db_image_name: str = "exasol/docker-db",
         db_os_access: Optional[str] = "DOCKER_EXEC",
@@ -64,14 +65,17 @@
     This function spawns a test environment with a docker-db container and a connected test-container.
     The test-container is reachable by the database for output redirects of UDFs.
     The function returns an environment_info object, describing the environment, and a cleanup-method, which
     can be used to stop the environment.
     raises: TaskRuntimeError if spawning the test environment fails
 
     """
+    def str_or_none(x: any) -> str:
+        return str(x) if x is not None else None
+
     parsed_db_mem_size = humanfriendly.parse_size(db_mem_size)
     if parsed_db_mem_size < humanfriendly.parse_size("1 GiB"):
         raise ArgumentConstraintError("db_mem_size", "needs to be at least 1 GiB")
     parsed_db_disk_size = humanfriendly.parse_size(db_disk_size)
     if parsed_db_disk_size < humanfriendly.parse_size("100 MiB"):
         raise ArgumentConstraintError("db_disk_size", "needs to be at least 100 MiB")
     set_build_config(False,
@@ -84,18 +88,17 @@
                      None)
     set_docker_repository_config(source_docker_password, source_docker_repository_name, source_docker_username,
                                  source_docker_tag_prefix, "source")
     set_docker_repository_config(target_docker_password, target_docker_repository_name, target_docker_username,
                                  target_docker_tag_prefix, "target")
     task_creator = lambda: generate_root_task(task_class=SpawnTestEnvironmentWithDockerDB,
                                               environment_name=environment_name,
-                                              database_port_forward=str(
-                                                  database_port_forward) if database_port_forward is not None else None,
-                                              bucketfs_port_forward=str(
-                                                  bucketfs_port_forward) if bucketfs_port_forward is not None else None,
+                                              database_port_forward=str_or_none(database_port_forward),
+                                              bucketfs_port_forward=str_or_none(bucketfs_port_forward),
+                                              ssh_port_forward=str_or_none(ssh_port_forward),
                                               mem_size=db_mem_size,
                                               disk_size=db_disk_size,
                                               nameservers=nameserver,
                                               docker_runtime=docker_runtime,
                                               docker_db_image_version=docker_db_image_version,
                                               docker_db_image_name=docker_db_image_name,
                                               db_os_access=DbOsAccess[db_os_access],
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from exasol_integration_test_docker_environment.lib.docker.networks.utils import remove_docker_networks
 from exasol_integration_test_docker_environment.lib.test_environment.spawn_test_environment_with_docker_db import \
     SpawnTestEnvironmentWithDockerDB
 from exasol_integration_test_docker_environment \
     .lib.test_environment.parameter \
     .docker_db_test_environment_parameter import DbOsAccess
 
-
 def _cleanup(environment_info: EnvironmentInfo) -> None:
     if environment_info.test_container_info is None:
         remove_docker_container([environment_info.database_info.container_info.container_name])
     else:
         remove_docker_container([environment_info.test_container_info.container_name,
                                  environment_info.database_info.container_info.container_name])
     remove_docker_volumes([environment_info.database_info.container_info.volume_name])
@@ -34,14 +33,15 @@
 
 @no_cli_function
 def spawn_test_environment_with_test_container(
         environment_name: str,
         test_container_content: TestContainerContentDescription,
         database_port_forward: Optional[int] = None,
         bucketfs_port_forward: Optional[int] = None,
+        ssh_port_forward: Optional[int] = None,
         db_mem_size: str = "2 GiB",
         db_disk_size: str = "2 GiB",
         nameserver: Tuple[str, ...] = tuple(),
         docker_runtime: Optional[str] = None,
         docker_db_image_version: str = LATEST_DB_VERSION,
         docker_db_image_name: str = "exasol/docker-db",
         db_os_access: str = "DOCKER_EXEC",
@@ -67,14 +67,16 @@
     This function spawns a test environment with a docker-db container and a connected test-container.
     The test-container is reachable by the database for output redirects of UDFs.
     The function returns an environment_info object, describing the environment, and a cleanup-method, which
     can be used to stop the environment.
     raises: TaskRuntimeError if spawning the test environment fails
 
     """
+    def str_or_none(x: any) -> str:
+        return str(x) if x is not None else None
     parsed_db_mem_size = humanfriendly.parse_size(db_mem_size)
     if parsed_db_mem_size < humanfriendly.parse_size("1 GiB"):
         raise ArgumentConstraintError("db_mem_size", "needs to be at least 1 GiB")
     parsed_db_disk_size = humanfriendly.parse_size(db_disk_size)
     if parsed_db_disk_size < humanfriendly.parse_size("100 MiB"):
         raise ArgumentConstraintError("db_disk_size", "needs to be at least 100 MiB")
     set_build_config(False,
@@ -87,18 +89,17 @@
                      None)
     set_docker_repository_config(source_docker_password, source_docker_repository_name, source_docker_username,
                                  source_docker_tag_prefix, "source")
     set_docker_repository_config(target_docker_password, target_docker_repository_name, target_docker_username,
                                  target_docker_tag_prefix, "target")
     task_creator = lambda: generate_root_task(task_class=SpawnTestEnvironmentWithDockerDB,
                                               environment_name=environment_name,
-                                              database_port_forward=str(
-                                                  database_port_forward) if database_port_forward is not None else None,
-                                              bucketfs_port_forward=str(
-                                                  bucketfs_port_forward) if bucketfs_port_forward is not None else None,
+                                              database_port_forward=str_or_none(database_port_forward),
+                                              bucketfs_port_forward=str_or_none(bucketfs_port_forward),
+                                              ssh_port_forward=str_or_none(ssh_port_forward),
                                               mem_size=db_mem_size,
                                               disk_size=db_disk_size,
                                               nameservers=nameserver,
                                               docker_runtime=docker_runtime,
                                               docker_db_image_version=docker_db_image_version,
                                               docker_db_image_name=docker_db_image_name,
                                               db_os_access=DbOsAccess[db_os_access],
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/base_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/flavor_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/info.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/info.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,22 @@
 
 def get_log_path(job_id: str) -> Path:
     """
     Retrieve the log-file path. Default path is $output_path/jobs/logs/main.log, but can be overwritten by
     the environment variable LOG_ENV_VARIABLE_NAME.
     """
     main_log_path = Path(build_config().output_directory) / "jobs" / job_id / "logs"
-    main_log_path.mkdir(parents=True, exist_ok=True)
     def_log_path = main_log_path / "main.log"
     env_log_path = os.getenv(LOG_ENV_VARIABLE_NAME)
     if env_log_path is not None:
         log_path = Path(env_log_path)
     else:
         log_path = def_log_path
+    log_path_dir = Path(log_path).parent
+    log_path_dir.mkdir(parents=True, exist_ok=True)
     return log_path
 
 
 @contextlib.contextmanager
 def restore_logger(logger_creator: Callable[[], logging.Logger]):
     before_logger = logger_creator()
     logger_info = {
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/ssh_access.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/ssh_access.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/still_running_logger.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/task_dependency.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/config/build_config.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/config/build_config.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/config/docker_config.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/config/docker_config.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/container_info.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/container_info.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/database_credentials.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/environment_info.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/environment_info.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/__init__.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/image_info.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,30 +108,31 @@
                 "bind": CERTIFICATES_MOUNT_PATH,
                 "mode": "rw"
             }
         }
 
         with self._get_docker_client() as docker_client:
             try:
-                test_container = \
-                    docker_client.containers.create(
-                        image=certificate_container_image_info.get_target_complete_name(),
-                        name="certificate_resources",
-                        network_mode=None,
-                        command="sleep infinity",
-                        detach=True,
-                        volumes=volumes,
-                        labels={"test_environment_name": self.environment_name,
-                                "container_type": "certificate_resources"},
-                        runtime=self.docker_runtime
-                    )
-                test_container.start()
+                container = docker_client.containers.create(
+                    image=certificate_container_image_info.get_target_complete_name(),
+                    name="certificate_resources",
+                    network_mode=None,
+                    command="sleep infinity",
+                    detach=True,
+                    volumes=volumes,
+                    labels={
+                        "test_environment_name": self.environment_name,
+                        "container_type": "certificate_resources",
+                    },
+                    runtime=self.docker_runtime
+                )
+                container.start()
                 self.logger.info("Creating certificates...")
                 cmd = f"bash /scripts/create_certificates.sh " \
                       f"{self._construct_complete_host_name} {CERTIFICATES_MOUNT_PATH}"
-                exit_code, output = test_container.exec_run(cmd)
+                exit_code, output = container.exec_run(cmd)
                 self.logger.info(output.decode('utf-8'))
                 if exit_code != 0:
                     raise RuntimeError(f"Error creating certificates:'{output.decode('utf-8')}'")
             finally:
-                test_container.stop()
-                test_container.remove()
+                container.stop()
+                container.remove()
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import time
 from datetime import datetime
 
 from docker.models.containers import Container
 
-from exasol_integration_test_docker_environment.lib.test_environment.database_setup.bucketfs_sync_checker import \
-    BucketFSSyncChecker
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.database_setup.bucketfs_sync_checker \
+    import BucketFSSyncChecker
+from exasol_integration_test_docker_environment \
+    .lib.base.db_os_executor import DbOsExecutor
 
 
 class DockerDBLogBasedBucketFSSyncChecker(BucketFSSyncChecker):
 
     def __init__(self, logger,
                  database_container: Container,
                  pattern_to_wait_for: str,
                  log_file_to_check: str,
-                 bucketfs_write_password: str):
+                 bucketfs_write_password: str,
+                 executor: DbOsExecutor):
         self.logger = logger
         self.pattern_to_wait_for = pattern_to_wait_for
         self.log_file_to_check = log_file_to_check
         self.database_container = database_container
         self.bucketfs_write_password = bucketfs_write_password
+        self.executor = executor
 
     def prepare_upload(self):
         self.start_exit_code, self.start_output = self.find_pattern_in_logfile()
 
     def wait_for_bucketfs_sync(self):
         self.logger.info("wait for upload of file")
 
@@ -41,16 +46,15 @@
     def found_new_log_line(self, exit_code, start_exit_code,
                            start_output, output):
         return exit_code == 0 and start_exit_code == 0 and len(start_output) < len(output)
 
     def find_pattern_in_logfile(self):
         cmd = f"""grep '{self.pattern_to_wait_for}' {self.log_file_to_check}"""
         bash_cmd = f"""bash -c "{cmd}" """
-        exit_code, output = \
-            self.database_container.exec_run(bash_cmd)
+        exit_code, output = self.executor.exec(bash_cmd)
         return exit_code, output
 
     def output_happened_after_start_time(self, output, start_time):
         time_str_from_output = " ".join(output.decode("utf-8").split(" ")[1:3])
         time_from_output = datetime.strptime(time_str_from_output, "%y%m%d %H:%M:%S")
         happened_after = time_from_output > start_time
         return happened_after
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         username = self.db_user
         password = self.db_password
         data_path_within_test_container = self.get_data_path_within_test_container()
         data_file_within_data_path = self.get_data_file_within_data_path()
         with self._get_docker_client() as docker_client:
             test_container = docker_client.containers.get(self._test_container_info.container_name)
             cmd = f"cd {data_path_within_test_container}; " \
-                  f"$EXAPLUS -c '{self._database_info.host}:{self._database_info.db_port}' " \
+                  f"$EXAPLUS -c '{self._database_info.host}:{self._database_info.ports.database}' " \
                   f"-x -u '{username}' -p '{password}' -f {data_file_within_data_path} " \
                   f"-jdbcparam 'validateservercertificate=0'"
 
             bash_cmd = f"""bash -c "{cmd}" """
             exit_code, output = test_container.exec_run(cmd=bash_cmd)
         self.write_logs(output.decode("utf-8"))
         if exit_code != 0:
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,27 @@
 
 # TODO add timeout, because sometimes the upload stucks
 from exasol_integration_test_docker_environment.abstract_method_exception import AbstractMethodException
 from exasol_integration_test_docker_environment.lib.base.docker_base_task import DockerBaseTask
 from exasol_integration_test_docker_environment.lib.base.json_pickle_parameter import JsonPickleParameter
 from exasol_integration_test_docker_environment.lib.base.still_running_logger import StillRunningLogger, \
     StillRunningLoggerThread
-from exasol_integration_test_docker_environment.lib.data.environment_info import EnvironmentInfo
-from exasol_integration_test_docker_environment.lib.test_environment.database_setup.docker_db_log_based_bucket_sync_checker import \
-    DockerDBLogBasedBucketFSSyncChecker
-from exasol_integration_test_docker_environment.lib.test_environment.database_setup.time_based_bucketfs_sync_waiter import \
-    TimeBasedBucketFSSyncWaiter
+from exasol_integration_test_docker_environment.lib.data.environment_info \
+    import EnvironmentInfo
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.database_setup.docker_db_log_based_bucket_sync_checker \
+    import DockerDBLogBasedBucketFSSyncChecker
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.database_setup.time_based_bucketfs_sync_waiter \
+    import TimeBasedBucketFSSyncWaiter
+from exasol_integration_test_docker_environment \
+    .lib.base.db_os_executor import (
+        DbOsExecutor,
+        DbOsExecFactory,
+    )
 
 
 @dataclasses.dataclass
 class UploadResult:
     upload_target: str
     reused: bool
 
@@ -31,14 +39,15 @@
 class UploadFileToBucketFS(DockerBaseTask):
     environment_name = luigi.Parameter()
     test_environment_info = JsonPickleParameter(
         EnvironmentInfo, significant=False)  # type: EnvironmentInfo
     reuse_uploaded = luigi.BoolParameter(False, significant=False)
     bucketfs_write_password = luigi.Parameter(
         significant=False, visibility=luigi.parameter.ParameterVisibility.HIDDEN)
+    executor_factory=JsonPickleParameter(DbOsExecFactory, significant=False)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._database_info = self.test_environment_info.database_info
 
     def run_task(self):
         file_to_upload = self.get_file_to_upload()
@@ -50,64 +59,89 @@
         with self._get_docker_client() as docker_client:
             if self._database_info.container_info is not None:
                 database_container = docker_client.containers.get(
                     self._database_info.container_info.container_name)
             else:
                 database_container = None
             if not self.should_be_reused(upload_target):
-                self.upload_and_wait(database_container,
-                                     file_to_upload,
-                                     upload_target,
-                                     log_file,
-                                     pattern_to_wait_for,
-                                     sync_time_estimation)
-                self.return_object(UploadResult(
-                    upload_target=upload_target,
-                    reused=False
-                ))
+                with self.executor_factory.executor() as executor:
+                    executor.prepare()
+                    self.upload_and_wait(
+                        database_container,
+                        file_to_upload,
+                        upload_target,
+                        log_file,
+                        pattern_to_wait_for,
+                        sync_time_estimation,
+                        db_os_executor=executor,
+                    )
+                    self.return_object(UploadResult(
+                        upload_target=upload_target,
+                        reused=False
+                    ))
             else:
                 self.logger.warning("Reusing uploaded target %s instead of file %s",
                                     upload_target, file_to_upload)
                 self.write_logs("Reusing")
                 self.return_object(UploadResult(
                     upload_target=upload_target,
                     reused=True
                 ))
 
-    def upload_and_wait(self, database_container,
-                        file_to_upload: str, upload_target: str,
-                        log_file: str, pattern_to_wait_for: str,
-                        sync_time_estimation: int):
-        still_running_logger = StillRunningLogger(self.logger,
-                                                  "file upload of %s to %s"
-                                                  % (file_to_upload, upload_target))
+    def upload_and_wait(
+            self,
+            database_container,
+            file_to_upload: str,
+            upload_target: str,
+            log_file: str,
+            pattern_to_wait_for: str,
+            sync_time_estimation: int,
+            db_os_executor: DbOsExecutor,
+    ):
+        still_running_logger = StillRunningLogger(
+            self.logger,
+            f"file upload of {file_to_upload} to {upload_target}",
+        )
         thread = StillRunningLoggerThread(still_running_logger)
         thread.start()
-        sync_checker = self.get_sync_checker(database_container, sync_time_estimation,
-                                             log_file, pattern_to_wait_for)
+        sync_checker = self.get_sync_checker(
+            database_container,
+            sync_time_estimation,
+            log_file,
+            pattern_to_wait_for,
+            db_os_executor=db_os_executor,
+        )
         sync_checker.prepare_upload()
         try:
-            output = self.upload_file(file_to_upload=file_to_upload, upload_target=upload_target)
+            output = self.upload_file(
+                file_to_upload=file_to_upload,
+                upload_target=upload_target,
+            )
             sync_checker.wait_for_bucketfs_sync()
             self.write_logs(output)
         finally:
             thread.stop()
             thread.join()
 
-    def get_sync_checker(self, database_container: Container,
-                         sync_time_estimation: int,
-                         log_file: str,
-                         pattern_to_wait_for: str):
+    def get_sync_checker(
+            self,
+            database_container: Container,
+            sync_time_estimation: int,
+            log_file: str,
+            pattern_to_wait_for: str,
+            db_os_executor: DbOsExecutor,
+    ):
         if database_container is not None:
             return DockerDBLogBasedBucketFSSyncChecker(
                 database_container=database_container,
                 log_file_to_check=log_file,
                 pattern_to_wait_for=pattern_to_wait_for,
                 logger=self.logger,
-                bucketfs_write_password=str(self.bucketfs_write_password)
+                bucketfs_write_password=str(self.bucketfs_write_password),
+                executor=db_os_executor,
             )
         else:
             return TimeBasedBucketFSSyncWaiter(sync_time_estimation)
 
     def should_be_reused(self, upload_target: str):
         return self.reuse_uploaded and self.exist_file_in_bucketfs(upload_target)
 
@@ -130,35 +164,35 @@
                 bucket_file_path=path_in_bucket)
             return file_in_bucket in files
         except FileNotFoundError as ex:
             return False
 
     def generate_bucket_config(self, bucket_name: str) -> BucketConfig:
         connection_config = BucketFSConnectionConfig(
-            host=self._database_info.host, port=int(self._database_info.bucketfs_port),
+            host=self._database_info.host, port=int(self._database_info.ports.bucketfs),
             user="w", pwd=str(self.bucketfs_write_password),
             is_https=False)
         bucketfs_config = BucketFSConfig(
             connection_config=connection_config,
             bucketfs_name="bfsdefault")
         bucket_config = BucketConfig(
             bucket_name=bucket_name,
             bucketfs_config=bucketfs_config)
         return bucket_config
 
     def upload_file(self, file_to_upload: str, upload_target: str):
         self.logger.info("upload file %s to %s",
                          file_to_upload, upload_target)
         bucket_name, path_in_bucket, file_in_bucket = self.split_upload_target(upload_target)
-
         bucket_config = self.generate_bucket_config(bucket_name)
         upload.upload_file_to_bucketfs(
             bucket_config=bucket_config,
             bucket_file_path=f"{path_in_bucket}/{file_in_bucket}",
-            local_file_path=Path(file_to_upload))
+            local_file_path=Path(file_to_upload)
+        )
         return f"File '{file_to_upload}' to '{upload_target}'"
 
     def write_logs(self, output):
         log_file = Path(self.get_log_path(), "log")
         with log_file.open("w") as file:
             file.write(output)
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,27 +23,31 @@
         self.error_message = None
 
     def stop(self):
         self.logger.info("Stop ContainerLogThread")
         self.finish = True
 
     def run(self):
-        with ContainerLogHandler(self.log_file, self.logger, self.description) as log_handler:
-            still_running_logger = StillRunningLogger(
-                self.logger, self.description)
-            while not self.finish:
-                self.current_timestamp = math.floor(time.time())
-                log = self.container.logs(since=self.previous_timestamp, until=self.current_timestamp)
-                if len(log) != 0:
-                    still_running_logger.log()
-                    log_handler.handle_log_lines(log)
-                log_line = log.decode("utf-8").lower()
-                if ("error" in log_line and not "sshd was not started" in log_line) \
-                        or "exception" in log_line \
-                        or ("returned with state 1" in log_line 
-                                and not "(membership) returned with state 1" in log_line): # exclude webui not found in 7.0.0 
-                    self.logger.info("ContainerLogHandler error message, %s", log_line)
-                    self.error_message = log_line
-                    self.finish = True
-                self.previous_timestamp = self.current_timestamp
-                self.complete_log = log_handler.get_complete_log().copy()
-                time.sleep(1)
+        try:
+            with ContainerLogHandler(self.log_file, self.logger, self.description) as log_handler:
+                still_running_logger = StillRunningLogger(
+                    self.logger, self.description)
+                while not self.finish:
+                    self.current_timestamp = math.floor(time.time())
+                    log = self.container.logs(since=self.previous_timestamp, until=self.current_timestamp)
+                    if len(log) != 0:
+                        still_running_logger.log()
+                        log_handler.handle_log_lines(log)
+                    log_line = log.decode("utf-8").lower()
+                    if ("error" in log_line and not "sshd was not started" in log_line) \
+                            or "exception" in log_line \
+                            or ("returned with state 1" in log_line
+                                    and not "(membership) returned with state 1" in log_line): # exclude webui not found in 7.0.0
+                        self.logger.info("ContainerLogHandler error message, %s", log_line)
+                        self.error_message = log_line
+                        self.finish = True
+                    self.previous_timestamp = self.current_timestamp
+                    self.complete_log = log_handler.get_complete_log().copy()
+                    time.sleep(1)
+        except Exception as e:
+            self.finish = True
+            self.logger.exception("Caught exception in DBContainerLogThread.run.")
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 import time
+from logging import Logger
 from pathlib import PurePath
 from threading import Thread
 
 from docker.models.containers import Container
 
 from exasol_integration_test_docker_environment.lib.data.database_credentials import DatabaseCredentials
 from exasol_integration_test_docker_environment.lib.data.database_info import DatabaseInfo
 from exasol_integration_test_docker_environment.lib.test_environment.database_setup.find_exaplus_in_db_container import \
     find_exaplus
+from exasol_integration_test_docker_environment.lib.base.db_os_executor import \
+    DbOsExecFactory
 
 
 class IsDatabaseReadyThread(Thread):
-
     def __init__(self,
-                 logger,
+                 logger: Logger,
                  database_info: DatabaseInfo,
                  database_container: Container,
                  database_credentials: DatabaseCredentials,
-                 docker_db_image_version: str):
+                 docker_db_image_version: str,
+                 executor_factory: DbOsExecFactory):
         super().__init__()
         self.logger = logger
         self.database_credentials = database_credentials
         self._database_info = database_info
         self._db_container = database_container
         self.finish = False
         self.is_ready = False
         self.output_db_connection = None
         self.output_bucketfs_connection = None
         self.docker_db_image_version = docker_db_image_version
+        self.executor_factory = executor_factory
 
     def stop(self):
         self.logger.info("Stop IsDatabaseReadyThread")
         self.finish = True
 
     def run(self):
-        db_connection_command = ""
-        bucket_fs_connection_command = ""
         try:
-            exaplus_path = find_exaplus(self._db_container)
-            db_connection_command = self.create_db_connection_command(exaplus_path)
-            bucket_fs_connection_command = self.create_bucketfs_connection_command()
-        except RuntimeError as e:
-            self.logger.error(e)
+            with self.executor_factory.executor() as executor:
+                db_connection_command = ""
+                bucket_fs_connection_command = ""
+                try:
+                    executor.prepare()
+                    exaplus_path = find_exaplus(self._db_container, executor)
+                    db_connection_command = self.create_db_connection_command(exaplus_path)
+                    bucket_fs_connection_command = self.create_bucketfs_connection_command()
+                except RuntimeError as e:
+                    self.logger.exception("Caught exception while searching for exaplus.")
+                    self.finish = True
+                while not self.finish:
+                    (exit_code_db_connection, self.output_db_connection) = \
+                        executor.exec(db_connection_command)
+                    (exit_code_bucketfs_connection, self.output_bucketfs_connection) = \
+                        executor.exec(bucket_fs_connection_command)
+                    if exit_code_db_connection == 0 and exit_code_bucketfs_connection == 0:
+                        self.finish = True
+                        self.is_ready = True
+                    time.sleep(1)
+        except Exception as e:
             self.finish = True
-        while not self.finish:
-            (exit_code_db_connection, self.output_db_connection) = \
-                self._db_container.exec_run(cmd=db_connection_command)
-            (exit_code_bucketfs_connection, self.output_bucketfs_connection) = \
-                self._db_container.exec_run(cmd=bucket_fs_connection_command)
-            if exit_code_db_connection == 0 and exit_code_bucketfs_connection == 0:
-                self.finish = True
-                self.is_ready = True
-            time.sleep(1)
+            self.logger.exception("Caught exception in IsDatabaseReadyThread.run.")
 
     def create_db_connection_command(self, exaplus_path: PurePath):
         username = self.database_credentials.db_user
         password = self.database_credentials.db_password
-        connection_options = f"""-c 'localhost:{self._database_info.db_port}' -u '{username}' -p '{password}'"""
+        connection_options = f"""-c 'localhost:{self._database_info.ports.database}' -u '{username}' -p '{password}'"""
 
-        cmd = f"""{exaplus_path} {connection_options}  -sql 'select 1;' -jdbcparam 'validateservercertificate=0'"""
+        cmd = f"""{exaplus_path} {connection_options} -sql 'select 1;' -jdbcparam 'validateservercertificate=0'"""
         bash_cmd = f"""bash -c "{cmd}" """
         return bash_cmd
 
     def create_bucketfs_connection_command(self):
         username = "w"
         password = self.database_credentials.bucketfs_write_password
-        cmd = f"""curl --silent --show-error --fail '{username}:{password}@localhost:{self._database_info.bucketfs_port}'"""
+        cmd = f"""curl --silent --show-error --fail '{username}:{password}@localhost:{self._database_info.ports.bucketfs}'"""
         bash_cmd = f"""bash -c "{cmd}" """
         return bash_cmd
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,25 @@
 from exasol_integration_test_docker_environment.lib.base.json_pickle_parameter import JsonPickleParameter
 from exasol_integration_test_docker_environment.lib.data.database_credentials import DatabaseCredentialsParameter
 from exasol_integration_test_docker_environment.lib.data.database_info import DatabaseInfo
 from exasol_integration_test_docker_environment.lib.test_environment.database_waiters.db_container_log_thread import \
     DBContainerLogThread
 from exasol_integration_test_docker_environment.lib.test_environment.database_waiters.is_database_ready_thread import \
     IsDatabaseReadyThread
+from exasol_integration_test_docker_environment.lib.base.db_os_executor import \
+    DbOsExecFactory
 
 
 class WaitForTestDockerDatabase(DockerBaseTask, DatabaseCredentialsParameter):
     environment_name = luigi.Parameter()
     database_info = JsonPickleParameter(DatabaseInfo, significant=False)  # type: DatabaseInfo
     db_startup_timeout_in_seconds = luigi.IntParameter(10 * 60, significant=False)
     attempt = luigi.IntParameter(1)
     docker_db_image_version = luigi.Parameter()
+    executor_factory = JsonPickleParameter(DbOsExecFactory, significant=False)
 
     def run_task(self):
         with self._get_docker_client() as docker_client:
             db_container_name = self.database_info.container_info.container_name
             db_container = docker_client.containers.get(db_container_name)
             is_database_ready = \
                 self.wait_for_database_startup(db_container)
@@ -45,19 +48,22 @@
     def start_wait_threads(self, db_container: Container):
         startup_log_file = self.get_log_path().joinpath("startup.log")
         container_log_thread = DBContainerLogThread(db_container,
                                                     self.logger,
                                                     startup_log_file,
                                                     "Database Startup %s" % db_container.name)
         container_log_thread.start()
-        is_database_ready_thread = IsDatabaseReadyThread(self.logger,
-                                                         self.database_info,
-                                                         db_container,
-                                                         self.get_database_credentials(),
-                                                         self.docker_db_image_version)
+        is_database_ready_thread = IsDatabaseReadyThread(
+            self.logger,
+            self.database_info,
+            db_container,
+            self.get_database_credentials(),
+            self.docker_db_image_version,
+            self.executor_factory,
+        )
         is_database_ready_thread.start()
         return container_log_thread, is_database_ready_thread
 
     def join_threads(self, container_log_thread: DBContainerLogThread,
                      is_database_ready_thread: IsDatabaseReadyThread):
         container_log_thread.stop()
         is_database_ready_thread.stop()
@@ -95,15 +101,15 @@
                                is_database_ready_thread: IsDatabaseReadyThread, reason):
         container_log = '\n'.join(container_log_thread.complete_log)
         log_information = f"""
 ========== IsDatabaseReadyThread output db connection: ============
 {is_database_ready_thread.output_db_connection}
 ========== IsDatabaseReadyThread output bucketfs connection: ============
 {is_database_ready_thread.output_bucketfs_connection}
-========== Container-Log: ============ 
+========== Container-Log: ============
 {container_log}
 """
         self.logger.warning(
             'Database startup failed for following reason "%s", here some debug information \n%s',
             reason, log_information)
 
     def timeout_occured(self, start_time):
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/db_version.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,10 +23,11 @@
     docker_db_image_version = luigi.OptionalParameter(None)
     reuse_database = luigi.BoolParameter(False, significant=False)
     db_os_access = luigi.EnumParameter(DbOsAccess.DOCKER_EXEC, enum=DbOsAccess, significant=False)
     no_database_cleanup_after_success = luigi.BoolParameter(False, significant=False)
     no_database_cleanup_after_failure = luigi.BoolParameter(False, significant=False)
     database_port_forward = luigi.OptionalParameter(None, significant=False)
     bucketfs_port_forward = luigi.OptionalParameter(None, significant=False)
+    ssh_port_forward = luigi.OptionalParameter(None, significant=False)
     mem_size = luigi.OptionalParameter("2 GiB", significant=False)
     disk_size = luigi.OptionalParameter("2 GiB", significant=False)
     nameservers = luigi.ListParameter([], significant=False)
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/parameter/test_container_parameter.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/test_container_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 import luigi
 
 from exasol_integration_test_docker_environment.lib.base.dependency_logger_base_task import DependencyLoggerBaseTask
 from exasol_integration_test_docker_environment.lib.base.json_pickle_parameter import JsonPickleParameter
 from exasol_integration_test_docker_environment.lib.data.database_credentials import DatabaseCredentialsParameter
 from exasol_integration_test_docker_environment.lib.data.database_info import DatabaseInfo
 from exasol_integration_test_docker_environment.lib.data.docker_network_info import DockerNetworkInfo
-from exasol_integration_test_docker_environment.lib.test_environment.parameter.external_test_environment_parameter import \
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.parameter.external_test_environment_parameter import \
     ExternalDatabaseXMLRPCParameter, ExternalDatabaseHostParameter
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.ports import Ports
 
 
 class SetupExternalDatabaseHost(DependencyLoggerBaseTask,
                                 ExternalDatabaseXMLRPCParameter,
                                 ExternalDatabaseHostParameter,
                                 DatabaseCredentialsParameter):
     environment_name = luigi.Parameter()
@@ -24,18 +27,20 @@
 
     def run_task(self):
         database_host = self.external_exasol_db_host
         if self.external_exasol_db_host == "localhost" or \
                 self.external_exasol_db_host == "127.0.01":
             database_host = self.network_info.gateway
         self.setup_database()
-        database_info = DatabaseInfo(host=database_host,
-                                     db_port=self.external_exasol_db_port,
-                                     bucketfs_port=self.external_exasol_bucketfs_port,
-                                     reused=False)
+        ports = Ports(
+            database=self.external_exasol_db_port,
+            bucketfs=self.external_exasol_bucketfs_port,
+            ssh=self.external_exasol_ssh_port,
+        )
+        database_info = DatabaseInfo(host=database_host, ports=ports, reused=False)
         self.return_object(database_info)
 
     def setup_database(self):
         if self.external_exasol_xmlrpc_host is not None:
             # TODO add option to use unverified ssl
             cluster = self.get_xml_rpc_object()
             self.start_database(cluster)
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,85 @@
 import math
-from typing import Tuple
+from typing import Optional, Tuple
 
 import docker
 import humanfriendly
 import luigi
 import netaddr
 import pkg_resources
 from docker.models.containers import Container
 from docker.models.volumes import Volume
+from docker.client import DockerClient
 from jinja2 import Template
 
 from exasol_integration_test_docker_environment.lib import PACKAGE_NAME
 from exasol_integration_test_docker_environment.lib.base.docker_base_task import DockerBaseTask
 from exasol_integration_test_docker_environment.lib.base.json_pickle_parameter import JsonPickleParameter
 from exasol_integration_test_docker_environment.lib.base.still_running_logger import StillRunningLogger
 from exasol_integration_test_docker_environment.lib.data.container_info import ContainerInfo
 from exasol_integration_test_docker_environment.lib.data.database_info import DatabaseInfo
 from exasol_integration_test_docker_environment.lib.data.docker_network_info import DockerNetworkInfo
 from exasol_integration_test_docker_environment.lib.docker.images.create.utils.pull_log_handler import PullLogHandler
 from exasol_integration_test_docker_environment.lib.docker.images.image_info import ImageInfo
 from exasol_integration_test_docker_environment.lib.test_environment.db_version import DbVersion
+from exasol_integration_test_docker_environment.lib.data.ssh_info import SshInfo
+from exasol_integration_test_docker_environment.lib.test_environment.ports import (
+    find_free_ports,
+    Ports,
+)
 from exasol_integration_test_docker_environment.lib.test_environment.docker_container_copy import DockerContainerCopy
 from exasol_integration_test_docker_environment.lib \
     .test_environment.parameter \
     .docker_db_test_environment_parameter import (
         DbOsAccess,
         DockerDBTestEnvironmentParameter,
 )
 from exasol_integration_test_docker_environment.lib.base.ssh_access import (
     SshKeyCache,
     SshKey,
 )
 
 
-BUCKETFS_PORT = "6583"
-DB_PORT = "8888"
 CERTIFICATES_MOUNT_DIR = "/certificates"
 CERTIFICATES_DEFAULT_DIR = "/exa/etc/ssl/"
 
 
+def int_or_none(value: str) -> Optional[int]:
+    return None if value is None else int(value)
+
+
 class SpawnTestDockerDatabase(DockerBaseTask, DockerDBTestEnvironmentParameter):
     environment_name = luigi.Parameter()  # type: str
     db_container_name = luigi.Parameter()  # type: str
     attempt = luigi.IntParameter(1)  # type: int
     network_info = JsonPickleParameter(DockerNetworkInfo, significant=False)  # type: DockerNetworkInfo
     ip_address_index_in_subnet = luigi.IntParameter(significant=False)  # type: int
     docker_runtime = luigi.OptionalParameter(None, significant=False)  # type: str
     certificate_volume_name = luigi.OptionalParameter(None, significant=False)
     additional_db_parameter = luigi.ListParameter()
+    ssh_user = luigi.Parameter("root")
+    ssh_key_file = luigi.OptionalParameter(None, significant=False)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if self.ip_address_index_in_subnet < 0:
             raise Exception(
                 "ip_address_index_in_subnet needs to be greater than 0 got %s"
                 % self.ip_address_index_in_subnet)
 
         self.db_version = DbVersion.from_db_version_str(self.docker_db_image_version)
         self.docker_db_config_resource_name = f"docker_db_config/{self.db_version}"
+        self.internal_ports = Ports.default_ports
+        if self.ssh_port_forward is None:
+            self.ssh_port_forward = str(find_free_ports(1)[0])
+        self.forwarded_ports = Ports(
+            database=int_or_none(self.database_port_forward),
+            bucketfs=int_or_none(self.bucketfs_port_forward),
+            ssh=int_or_none(self.ssh_port_forward),
+        )
 
     def run_task(self):
         subnet = netaddr.IPNetwork(self.network_info.subnet)
         db_ip_address = str(subnet[2 + self.ip_address_index_in_subnet])
         db_private_network = "{ip}/{prefix}".format(ip=db_ip_address, prefix=subnet.prefixlen)
         database_info = None
         if self.network_info.reused:
@@ -70,93 +88,131 @@
             database_info = self._create_database_container(db_ip_address, db_private_network)
         self.return_object(database_info)
 
     def _try_to_reuse_database(self, db_ip_address: str) -> DatabaseInfo:
         self.logger.info("Try to reuse database container %s",
                          self.db_container_name)
         database_info = None
+        ssh_key = self._get_ssh_key()
         try:
             database_info = self._create_database_info(db_ip_address=db_ip_address, reused=True)
         except Exception as e:
             self.logger.warning("Tried to reuse database container %s, but got Exeception %s. "
                                 "Fallback to create new database.", self.db_container_name, e)
         return database_info
 
+    def _get_ssh_key(self) -> SshKey:
+        if self.ssh_key_file:
+            return SshKey.read_from(self.ssh_key_file)
+        self.ssh_key_file = SshKeyCache().private_key
+        return SshKey.from_cache()
+
     def _handle_output(self, output_generator, image_info: ImageInfo):
         log_file_path = self.get_log_path().joinpath("pull_docker_db_image.log")
         with PullLogHandler(log_file_path, self.logger, image_info) as log_handler:
             still_running_logger = StillRunningLogger(
                 self.logger, "pull image %s" % image_info.get_source_complete_name())
             for log_line in output_generator:
                 still_running_logger.log()
                 log_handler.handle_log_lines(log_line)
 
-    def _enable_ssh_access(self, container: Container):
-        sshkey = SshKey.from_cache()
-        copy = DockerContainerCopy(container)
-        content = sshkey.public_key_as_string("itde-ssh-access")
-        copy.add_string_to_file(".ssh/authorized_keys", content)
-        copy.copy("/root/")
+    def _get_network_aliases(self):
+        network_aliases = ["exasol_test_database", "exasol-test-database", self.db_container_name]
+        return network_aliases
+
+    def _connect_docker_network(
+            self,
+            docker_client: DockerClient,
+            container: Container,
+            ip_address: str,
+    ):
+        network = docker_client.networks.get(self.network_info.network_name)
+        aliases = self._get_network_aliases()
+        network.connect(container, ipv4_address=ip_address, aliases=aliases)
+
+    def _port_mapping(self, internal_ports, forwarded_ports):
+        result = {}
+        for name, internal in internal_ports.__dict__.items():
+            forward = forwarded_ports.__getattribute__(name)
+            if forward:
+                result[f"{internal}/tcp"] = ('0.0.0.0', forward)
+        return result
 
     def _create_database_container(self, db_ip_address: str, db_private_network: str):
+        def get_authorized_keys(ssh_key) -> str:
+            """
+            Multiple authorized_keys can be comma-separated.
+            """
+            if self.db_os_access != DbOsAccess.SSH:
+                return ""
+            return ssh_key.public_key_as_string("itde-ssh-access")
+
+        def enable_ssh_access(container: Container, authorized_keys: str):
+            copy = DockerContainerCopy(container)
+            copy.add_string_to_file(".ssh/authorized_keys", authorized_keys)
+            copy.copy("/root/")
+
         self.logger.info("Starting database container %s", self.db_container_name)
+        ssh_key = self._get_ssh_key()
+        authorized_keys = get_authorized_keys(ssh_key)
         with self._get_docker_client() as docker_client:
             try:
                 docker_client.containers.get(self.db_container_name).remove(force=True, v=True)
             except:
                 pass
             docker_db_image_info = self._pull_docker_db_images_if_necessary()
-            db_volume = self._prepare_db_volume(docker_client, db_private_network, docker_db_image_info)
-            ports = {}
-            if self.database_port_forward is not None:
-                ports[f"{DB_PORT}/tcp"] = ('0.0.0.0', int(self.database_port_forward))
-            if self.bucketfs_port_forward is not None:
-                ports[f"{BUCKETFS_PORT}/tcp"] = ('0.0.0.0', int(self.bucketfs_port_forward))
+            db_volume = self._prepare_db_volume(
+                docker_client,
+                db_private_network,
+                authorized_keys,
+                docker_db_image_info,
+            )
+            port_mapping = self._port_mapping(self.internal_ports, self.forwarded_ports)
             volumes = {db_volume.name: {"bind": "/exa", "mode": "rw"}}
             if self.certificate_volume_name is not None:
                 volumes[self.certificate_volume_name] = {"bind": CERTIFICATES_MOUNT_DIR, "mode": "ro"}
             db_container = \
                 docker_client.containers.create(
                     image="%s" % (docker_db_image_info.get_source_complete_name()),
                     name=self.db_container_name,
                     detach=True,
                     privileged=True,
                     volumes=volumes,
                     network_mode=None,
-                    ports=ports,
+                    ports=port_mapping,
                     runtime=self.docker_runtime
                 )
-            if self.db_os_access == DbOsAccess.SSH:
-                self._enable_ssh_access(db_container)
-            docker_network = docker_client.networks.get(self.network_info.network_name)
-            network_aliases = self._get_network_aliases()
-            docker_network.connect(db_container, ipv4_address=db_ip_address, aliases=network_aliases)
+            enable_ssh_access(db_container, authorized_keys)
+            self._connect_docker_network(docker_client, db_container, db_ip_address)
             db_container.start()
             database_info = self._create_database_info(db_ip_address=db_ip_address, reused=False)
             return database_info
 
-    def _get_network_aliases(self):
-        network_aliases = ["exasol_test_database", "exasol-test-database", self.db_container_name]
-        return network_aliases
-
     def _create_database_info(self, db_ip_address: str, reused: bool) -> DatabaseInfo:
         with self._get_docker_client() as docker_client:
             db_container = docker_client.containers.get(self.db_container_name)
             if db_container.status != "running":
                 raise Exception(f"Container {self.db_container_name} not running")
             network_aliases = self._get_network_aliases()
-            container_info = \
-                ContainerInfo(container_name=self.db_container_name,
-                              ip_address=db_ip_address,
-                              network_aliases=network_aliases,
-                              network_info=self.network_info,
-                              volume_name=self._get_db_volume_name())
-            database_info = \
-                DatabaseInfo(host=db_ip_address, db_port=DB_PORT, bucketfs_port=BUCKETFS_PORT,
-                             reused=reused, container_info=container_info)
+            container_info = ContainerInfo(
+                container_name=self.db_container_name,
+                ip_address=db_ip_address,
+                network_aliases=network_aliases,
+                network_info=self.network_info,
+                volume_name=self._get_db_volume_name(),
+            )
+            ssh_info = SshInfo(self.ssh_user, self.ssh_key_file)
+            database_info = DatabaseInfo(
+                host=db_ip_address,
+                ports=self.internal_ports,
+                reused=reused,
+                container_info=container_info,
+                ssh_info=ssh_info,
+                forwarded_ports=self.forwarded_ports,
+            )
             return database_info
 
     def _pull_docker_db_images_if_necessary(self):
         image_name = "exasol/docker-db"
         docker_db_image_info = ImageInfo(
             target_repository_name=image_name,
             source_repository_name=image_name,
@@ -173,24 +229,29 @@
                 output_generator = docker_client.api.pull(
                     docker_db_image_info.source_repository_name,
                     tag=docker_db_image_info.source_tag,
                     stream=True)
                 self._handle_output(output_generator, docker_db_image_info)
         return docker_db_image_info
 
-    def _prepare_db_volume(self, docker_client, db_private_network: str,
-                           docker_db_image_info: ImageInfo) -> Volume:
+    def _prepare_db_volume(
+            self,
+            docker_client,
+            db_private_network: str,
+            authorized_keys: str,
+            docker_db_image_info: ImageInfo
+    ) -> Volume:
         volume, container = self._prepare_volume(
             docker_client,
             self._get_db_volume_name(),
             self._get_db_volume_preparation_container_name(),
             remove_old_instances=True,
         )
         try:
-            self._upload_init_db_files(container, db_private_network)
+            self._upload_init_db_files(container, db_private_network, authorized_keys)
             self._execute_init_db(volume, container)
             return volume
         finally:
             container.remove(force=True)
 
     def _get_db_volume_preparation_container_name(self):
         return f"""{self.db_container_name}_preparation"""
@@ -239,41 +300,57 @@
                 labels={
                     "test_environment_name": self.environment_name,
                     "container_type": "db_volume_preparation_container",
                 }
         )
         return volume, container
 
-    def _upload_init_db_files(self, container: Container, db_private_network: str):
+    def _upload_init_db_files(
+            self,
+            container: Container,
+            db_private_network: str,
+            authorized_keys: str,
+    ):
         copy = DockerContainerCopy(container)
         init_db_script_str = pkg_resources.resource_string(
             PACKAGE_NAME,
             f"{self.docker_db_config_resource_name}/init_db.sh") # type: bytes
 
         copy.add_string_to_file("init_db.sh", init_db_script_str.decode("utf-8"))
-        self._add_exa_conf(copy, db_private_network)
+        self._add_exa_conf(copy, db_private_network, authorized_keys)
         copy.copy("/")
 
-    def _add_exa_conf(self, copy: DockerContainerCopy,
-                      db_private_network: str):
+    def _add_exa_conf(
+            self,
+            copy: DockerContainerCopy,
+            db_private_network: str,
+            authorized_keys: str,
+    ):
+        """
+        Multiple authorized_keys can be comma-separated.
+        """
         certificate_dir = CERTIFICATES_MOUNT_DIR if self.certificate_volume_name is not None \
                             else CERTIFICATES_DEFAULT_DIR
         template_str = pkg_resources.resource_string(
             PACKAGE_NAME,
             f"{self.docker_db_config_resource_name}/EXAConf") # type: bytes
         template = Template(template_str.decode("utf-8"))
         additional_db_parameter_str = " ".join(self.additional_db_parameter)
         rendered_template = template.render(private_network=db_private_network,
                                             db_version=str(self.db_version),
+                                            db_port=self.internal_ports.database,
+                                            ssh_port=self.internal_ports.ssh,
+                                            bucketfs_port=self.internal_ports.bucketfs,
                                             image_version=self.docker_db_image_version,
                                             mem_size=self.mem_size,
                                             disk_size=self.disk_size,
                                             name_servers=",".join(self.nameservers),
                                             certificate_dir=certificate_dir,
-                                            additional_db_parameters=additional_db_parameter_str)
+                                            additional_db_parameters=additional_db_parameter_str,
+                                            authorized_keys=authorized_keys)
         copy.add_string_to_file("EXAConf", rendered_template)
 
     def _execute_init_db(self, db_volume: Volume, preparation_container: Container):
         disk_size_in_bytes = humanfriendly.parse_size(self.disk_size)
         min_overhead_in_gigabyte = 2  # Exasol needs at least a 2 GB larger device than the configured disk size
         overhead_factor = max(0.01, (
                 min_overhead_in_gigabyte * 1024 * 1024 * 1024) / disk_size_in_bytes)  # and in general 1% larger
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 from typing import Optional
 
 from exasol_integration_test_docker_environment.lib.data.container_info import ContainerInfo
 from exasol_integration_test_docker_environment.lib.data.database_info import DatabaseInfo
 from exasol_integration_test_docker_environment.lib.data.docker_network_info import DockerNetworkInfo
 from exasol_integration_test_docker_environment.lib.data.docker_volume_info import DockerVolumeInfo
 from exasol_integration_test_docker_environment.lib.data.environment_type import EnvironmentType
-from exasol_integration_test_docker_environment.lib.test_environment.abstract_spawn_test_environment import \
-    AbstractSpawnTestEnvironment
-from exasol_integration_test_docker_environment.lib.test_environment.create_certificates.create_ssl_certificates_task import \
-    CreateSSLCertificatesTask
-from exasol_integration_test_docker_environment.lib.test_environment.database_waiters.wait_for_test_docker_database import \
-    WaitForTestDockerDatabase
-from exasol_integration_test_docker_environment.lib.test_environment.db_version import \
-    db_version_supports_custom_certificates
-from exasol_integration_test_docker_environment.lib.test_environment.parameter.docker_db_test_environment_parameter import \
-    DockerDBTestEnvironmentParameter
-from exasol_integration_test_docker_environment.lib.test_environment.prepare_network_for_test_environment import \
-    PrepareDockerNetworkForTestEnvironment
-from exasol_integration_test_docker_environment.lib.test_environment.spawn_test_database import SpawnTestDockerDatabase
-
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.abstract_spawn_test_environment \
+    import AbstractSpawnTestEnvironment
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.create_certificates.create_ssl_certificates_task \
+    import CreateSSLCertificatesTask
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.database_waiters.wait_for_test_docker_database \
+    import WaitForTestDockerDatabase
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.db_version \
+    import db_version_supports_custom_certificates
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.parameter.docker_db_test_environment_parameter \
+    import DockerDBTestEnvironmentParameter
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.prepare_network_for_test_environment \
+    import PrepareDockerNetworkForTestEnvironment
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.spawn_test_database \
+    import SpawnTestDockerDatabase
+from exasol_integration_test_docker_environment \
+    .lib.base.db_os_executor import (
+        DockerClientFactory,
+        DbOsExecFactory,
+        SshExecFactory,
+        DockerExecFactory,
+    )
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.parameter.docker_db_test_environment_parameter \
+    import DbOsAccess
 
 class SpawnTestEnvironmentWithDockerDB(
     AbstractSpawnTestEnvironment,
     DockerDBTestEnvironmentParameter):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -31,59 +48,63 @@
 
     def get_environment_type(self):
         return EnvironmentType.docker_db
 
     def create_ssl_certificates(self):
         if not db_version_supports_custom_certificates(self.docker_db_image_version):
             raise ValueError("Minimal supported Database with custom certificates is '7.0.6'")
-        return \
-            self.create_child_task_with_common_params(
-                CreateSSLCertificatesTask,
-                environment_name=self.environment_name,
-                db_container_name=self.db_container_name,
-                network_name=self.network_name,
-                docker_runtime=self.docker_runtime,
-                volume_name=self.certificate_volume_name,
-                reuse=self.reuse_database or self.reuse_test_container,
-                no_cleanup_after_success=self.no_database_cleanup_after_success or self.no_test_container_cleanup_after_success,
-                no_cleanup_after_failure=self.no_database_cleanup_after_failure or self.no_test_container_cleanup_after_failure,
-            )
+        return self.create_child_task_with_common_params(
+            CreateSSLCertificatesTask,
+            environment_name=self.environment_name,
+            db_container_name=self.db_container_name,
+            network_name=self.network_name,
+            docker_runtime=self.docker_runtime,
+            volume_name=self.certificate_volume_name,
+            reuse=self.reuse_database or self.reuse_test_container,
+            no_cleanup_after_success=self.no_database_cleanup_after_success or self.no_test_container_cleanup_after_success,
+            no_cleanup_after_failure=self.no_database_cleanup_after_failure or self.no_test_container_cleanup_after_failure,
+        )
 
     def create_network_task(self, attempt: int):
-        return \
-            self.create_child_task_with_common_params(
-                PrepareDockerNetworkForTestEnvironment,
-                test_container_name=self.test_container_name,
-                network_name=self.network_name,
-                db_container_name=self.db_container_name,
-                reuse=self.reuse_database or self.reuse_test_container,
-                no_cleanup_after_success=self.no_database_cleanup_after_success or self.no_test_container_cleanup_after_success,
-                no_cleanup_after_failure=self.no_database_cleanup_after_failure or self.no_test_container_cleanup_after_failure,
-                attempt=attempt
-            )
-
-    def create_spawn_database_task(self,
-                                   network_info: DockerNetworkInfo,
-                                   certificate_volume_info: Optional[DockerVolumeInfo],
-                                   attempt: int):
-        certificate_volume_name = certificate_volume_info.volume_name if certificate_volume_info is not None else None
-
-        return \
-            self.create_child_task_with_common_params(
-                SpawnTestDockerDatabase,
-                db_container_name=self.db_container_name,
-                network_info=network_info,
-                certificate_volume_name=certificate_volume_name,
-                ip_address_index_in_subnet=0,
-                attempt=attempt,
-                additional_db_parameter=self.additional_db_parameter
-            )
-
-    def create_wait_for_database_task(self,
-                                      attempt: int,
-                                      database_info: DatabaseInfo):
-        return \
-            self.create_child_task_with_common_params(
-                WaitForTestDockerDatabase,
-                database_info=database_info,
-                attempt=attempt,
-                docker_db_image_version=self.docker_db_image_version)
+        return self.create_child_task_with_common_params(
+            PrepareDockerNetworkForTestEnvironment,
+            test_container_name=self.test_container_name,
+            network_name=self.network_name,
+            db_container_name=self.db_container_name,
+            reuse=self.reuse_database or self.reuse_test_container,
+            no_cleanup_after_success=self.no_database_cleanup_after_success or self.no_test_container_cleanup_after_success,
+            no_cleanup_after_failure=self.no_database_cleanup_after_failure or self.no_test_container_cleanup_after_failure,
+            attempt=attempt,
+        )
+
+    def _executor_factory(self, database_info: DatabaseInfo) -> DbOsExecFactory:
+        if self.db_os_access == DbOsAccess.SSH:
+            return SshExecFactory.from_database_info(database_info)
+        client_factory = DockerClientFactory(timeout=100000)
+        return DockerExecFactory(self.db_container_name, client_factory)
+
+    def create_spawn_database_task(
+            self,
+            network_info: DockerNetworkInfo,
+            certificate_volume_info: Optional[DockerVolumeInfo],
+            attempt: int,
+    ):
+        def volume_name(info):
+            return None if info is None else info.volume_name
+        return self.create_child_task_with_common_params(
+            SpawnTestDockerDatabase,
+            db_container_name=self.db_container_name,
+            network_info=network_info,
+            certificate_volume_name=volume_name(certificate_volume_info),
+            ip_address_index_in_subnet=0,
+            attempt=attempt,
+            additional_db_parameter=self.additional_db_parameter
+        )
+
+    def create_wait_for_database_task(self, attempt: int, database_info: DatabaseInfo):
+        return self.create_child_task_with_common_params(
+            WaitForTestDockerDatabase,
+            database_info=database_info,
+            attempt=attempt,
+            docker_db_image_version=self.docker_db_image_version,
+            executor_factory=self._executor_factory(database_info)
+        )
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/lib/utils/resource_directory.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/templates/luigi_log.conf` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/templates/luigi_log.conf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/api_consistency_utils.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/api_test_environment.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/api_test_environment.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     .testing.exaslct_docker_test_environment import \
     ExaslctDockerTestEnvironment
 from exasol_integration_test_docker_environment \
     .testing.exaslct_test_environment import (
         get_class,
         get_test_flavor,
 )
-from exasol_integration_test_docker_environment.testing.utils import find_free_ports
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.ports import Ports
 
 
 class ApiTestEnvironment:
 
     def __init__(self, test_object, name=None):
         self.test_object = test_object
         self.test_class = get_class(test_object)
@@ -42,50 +43,59 @@
 
     def close(self):
         try:
             shutil.rmtree(self.temp_dir)
         except Exception as e:
             print(e, file=stderr)
 
-    def _get_default_test_environment(self, name: str, database_port: int, bucketfs_port: int):
+    def _get_default_test_environment(self, name: str, ports: Ports):
         return ExaslctDockerTestEnvironment(
             name=self.name + "_" + name,
             database_host="localhost",
             db_username="sys",
             db_password="exasol",
             bucketfs_username="w",
             bucketfs_password="write",
-            database_port=database_port,
-            bucketfs_port=bucketfs_port)
+            ports=ports,
+        )
 
-    def spawn_docker_test_environment_with_test_container(self, name: str,
-                                                          test_container_content: TestContainerContentDescription,
-                                                          additional_parameter: Dict[str, Any] = None) \
-            -> ExaslctDockerTestEnvironment:
+    def spawn_docker_test_environment_with_test_container(
+            self,
+            name: str,
+            test_container_content: TestContainerContentDescription,
+            additional_parameter: Dict[str, Any] = None,
+    ) -> ExaslctDockerTestEnvironment:
         if additional_parameter is None:
             additional_parameter = dict()
-        database_port, bucketfs_port = find_free_ports(2)
-        on_host_parameter = self._get_default_test_environment(name, database_port, bucketfs_port)
+        ports = Ports.random_free()
+        on_host_parameter = self._get_default_test_environment(name, ports)
         docker_db_image_version = on_host_parameter.docker_db_image_version
         on_host_parameter.environment_info, on_host_parameter.clean_up = \
-            spawn_test_environment_with_test_container(environment_name=on_host_parameter.name,
-                                                       database_port_forward=on_host_parameter.database_port,
-                                                       bucketfs_port_forward=on_host_parameter.bucketfs_port,
-                                                       docker_db_image_version=docker_db_image_version,
-                                                       test_container_content=test_container_content,
-                                                       **additional_parameter)
+            spawn_test_environment_with_test_container(
+                environment_name=on_host_parameter.name,
+                database_port_forward=ports.database,
+                bucketfs_port_forward=ports.bucketfs,
+                ssh_port_forward=ports.ssh,
+                docker_db_image_version=docker_db_image_version,
+                test_container_content=test_container_content,
+                **additional_parameter,
+            )
         return on_host_parameter
 
-    def spawn_docker_test_environment(self, name: str,
-                                      additional_parameter: Dict[str, Any] = None) \
-            -> ExaslctDockerTestEnvironment:
+    def spawn_docker_test_environment(
+            self,
+            name: str,
+            additional_parameter: Dict[str, Any] = None,
+    ) -> ExaslctDockerTestEnvironment:
         if additional_parameter is None:
             additional_parameter = dict()
-        database_port, bucketfs_port = find_free_ports(2)
-        on_host_parameter = self._get_default_test_environment(name, database_port, bucketfs_port)
-        on_host_parameter.environment_info, on_host_parameter.clean_up = \
-            spawn_test_environment(environment_name=on_host_parameter.name,
-                                   database_port_forward=on_host_parameter.database_port,
-                                   bucketfs_port_forward=on_host_parameter.bucketfs_port,
-                                   docker_db_image_version=on_host_parameter.docker_db_image_version,
-                                   **additional_parameter)
-        return on_host_parameter
+        ports = Ports.random_free()
+        on_host = self._get_default_test_environment(name, ports)
+        on_host.environment_info, on_host.clean_up = spawn_test_environment(
+            environment_name=on_host.name,
+            database_port_forward=on_host.ports.database,
+            bucketfs_port_forward=on_host.ports.bucketfs,
+            ssh_port_forward=on_host.ports.ssh,
+            docker_db_image_version=on_host.docker_db_image_version,
+            **additional_parameter,
+        )
+        return on_host
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/docker_registry.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/docker_registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import time
 
 import requests
 
 from exasol_integration_test_docker_environment.lib.docker import ContextDockerClient
 from exasol_integration_test_docker_environment.lib.docker.container.utils import remove_docker_container
-from exasol_integration_test_docker_environment.testing.utils import find_free_ports
+from exasol_integration_test_docker_environment.lib.test_environment.ports import find_free_ports
 
 
 def default_docker_repository_name(env_name: str) -> str:
     return f"exaslct_test/{env_name.lower()}"
 
 
 class LocalDockerRegistry:
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import subprocess
 from typing import Optional
 
-from exasol_integration_test_docker_environment.cli.options.test_environment_options import LATEST_DB_VERSION
-from exasol_integration_test_docker_environment.lib.data.environment_info import EnvironmentInfo
-from exasol_integration_test_docker_environment.testing.utils import check_db_version_from_env
+from exasol_integration_test_docker_environment \
+    .cli.options.test_environment_options import LATEST_DB_VERSION
+from exasol_integration_test_docker_environment \
+    .lib.data.environment_info import EnvironmentInfo
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.ports import Ports
+from exasol_integration_test_docker_environment \
+    .testing.utils import check_db_version_from_env
 
 
 class ExaslctDockerTestEnvironment:
     def __init__(self, name: str, database_host: str,
                  db_username: str, db_password: str,
-                 bucketfs_username: str, bucketfs_password: str,
-                 database_port: int, bucketfs_port: int,
+                 bucketfs_username: str,
+                 bucketfs_password: str,
+                 ports: Ports,
                  environment_info: Optional[EnvironmentInfo] = None,
                  completed_process: Optional[subprocess.CompletedProcess] = None):
         self.db_password = db_password
         self.db_username = db_username
-        self.database_port = database_port
-        self.bucketfs_port = bucketfs_port
+        self.ports = ports
         self.bucketfs_username = bucketfs_username
         self.bucketfs_password = bucketfs_password
         self.database_host = database_host
         self.name = name
         self.environment_info = environment_info
         self.completed_process = completed_process
         self.clean_up = None
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from exasol_integration_test_docker_environment.lib.docker import ContextDockerClient
 from exasol_integration_test_docker_environment.lib.docker.container.utils import remove_docker_container
 from exasol_integration_test_docker_environment.lib.docker.volumes.utils import remove_docker_volumes
 from exasol_integration_test_docker_environment.testing.docker_registry import default_docker_repository_name
 from exasol_integration_test_docker_environment.testing.exaslct_docker_test_environment import \
     ExaslctDockerTestEnvironment
 from exasol_integration_test_docker_environment.testing.spawned_test_environments import SpawnedTestEnvironments
-from exasol_integration_test_docker_environment.testing.utils import find_free_ports, check_db_version_from_env
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.ports import Ports
+from exasol_integration_test_docker_environment.testing.utils import check_db_version_from_env
 
 
 def _cleanup(env_name: str):
     remove_docker_container([f"test_container_{env_name}",
                              f"db_container_{env_name}"])
     remove_docker_volumes([f"db_container_{env_name}_volume"])
 
@@ -126,58 +128,60 @@
         try:
             shutil.rmtree(self.temp_dir)
         except Exception as e:
             print(e, file=stderr)
 
     def spawn_docker_test_environments(self, name: str, additional_parameter: List[str] = None) \
             -> SpawnedTestEnvironments:
-        database_port, bucketfs_port = find_free_ports(2)
+        ports = Ports.random_free()
         on_host_parameter = ExaslctDockerTestEnvironment(
             name=self.name + "_" + name,
             database_host="localhost",
             db_username="sys",
             db_password="exasol",
             bucketfs_username="w",
             bucketfs_password="write",
-            database_port=database_port,
-            bucketfs_port=bucketfs_port)
+            ports=ports,
+        )
 
         arguments = [
             f"--environment-name {on_host_parameter.name}",
-            f"--database-port-forward {on_host_parameter.database_port}",
-            f"--bucketfs-port-forward {on_host_parameter.bucketfs_port}",
+            f"--database-port-forward {on_host_parameter.ports.database}",
+            f"--bucketfs-port-forward {on_host_parameter.ports.bucketfs}",
+            f"--ssh-port-forward {on_host_parameter.ports.ssh}",
         ]
         db_version = check_db_version_from_env()
         if db_version:
             arguments.append(f'--docker-db-image-version "{db_version}"')
         if additional_parameter:
             arguments += additional_parameter
         arguments = " ".join(arguments)
 
         command = f"{self.executable} spawn-test-environment {arguments}"
         completed_process = self.run_command(command, use_flavor_path=False, use_docker_repository=False,
                                              capture_output=True)
         on_host_parameter.completed_process = completed_process
-        environment_info_json_path = Path(self.temp_dir,
-                                          f"cache/environments/{on_host_parameter.name}/environment_info.json")
+        environment_info_json_path = Path(
+            self.temp_dir,
+            f"cache/environments/{on_host_parameter.name}/environment_info.json",
+        )
         if environment_info_json_path.exists():
             with environment_info_json_path.open() as f:
                 environment_info = EnvironmentInfo.from_json(f.read())
                 on_host_parameter.environment_info = environment_info
         on_host_parameter.clean_up = functools.partial(_cleanup, on_host_parameter.name)
         if "RUN_SLC_TESTS_WITHIN_CONTAINER" in os.environ:
             slc_test_run_parameter = ExaslctDockerTestEnvironment(
                 name=on_host_parameter.name,
                 database_host="localhost",
                 db_username=on_host_parameter.db_username,
                 db_password=on_host_parameter.db_password,
                 bucketfs_username=on_host_parameter.bucketfs_username,
                 bucketfs_password=on_host_parameter.bucketfs_password,
-                database_port=8888,
-                bucketfs_port=6583,
+                ports=Ports.default_ports,
                 environment_info=on_host_parameter.completed_process,
                 completed_process=on_host_parameter.completed_process
             )
 
             with ContextDockerClient() as docker_client:
                 db_container = docker_client.containers.get(f"db_container_{slc_test_run_parameter.name}")
                 cloudbuild_network = docker_client.networks.get("cloudbuild")
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/luigi_utils.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/luigi_utils.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/exasol_integration_test_docker_environment/testing/spawned_test_environments.py` & `exasol_integration_test_docker_environment-2.0.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.7.1/pyproject.toml` & `exasol_integration_test_docker_environment-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "exasol-integration-test-docker-environment"
 packages = [
     { include = "exasol_integration_test_docker_environment" },
     { include = "pytest_itde" }
 ]
-version = "1.7.1"
+version = "2.0.0"
 description = "Integration Test Docker Environment for Exasol"
 
 license = "MIT"
 
 authors = [
     "Torsten Kilias <torsten.kilias@exasol.com>"
 ]
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/pytest_itde/__init__.py` & `exasol_integration_test_docker_environment-2.0.0/pytest_itde/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import os
 from typing import Tuple
 
 import pyexasol
 import pytest
 
 from pytest_itde import config
+from exasol_integration_test_docker_environment.lib.test_environment.ports import Ports
 
 EXASOL = config.OptionGroup(
     prefix="exasol",
     options=(
         {
             "name": "host",
             "type": str,
             "default": "localhost",
             "help_text": "Host to connect to",
         },
         {
             "name": "port",
             "type": int,
-            "default": 8888,
+            "default": Ports.forward.database,
             "help_text": "Port on which the exasol db is listening",
         },
         {
             "name": "username",
             "type": str,
             "default": "SYS",
             "help_text": "Username used to authenticate against the exasol db",
@@ -38,15 +39,15 @@
 
 BUCKETFS = config.OptionGroup(
     prefix="bucketfs",
     options=(
         {
             "name": "url",
             "type": str,
-            "default": "http://127.0.0.1:6666",
+            "default": f"http://127.0.0.1:{Ports.forward.bucketfs}",
             "help_text": "Base url used to connect to the bucketfs service",
         },
         {
             "name": "username",
             "type": str,
             "default": "w",
             "help_text": "Username used to authenticate against the bucketfs service",
@@ -56,14 +57,25 @@
             "type": str,
             "default": "write",
             "help_text": "Password used to authenticate against the bucketfs service",
         },
     ),
 )
 
+SSH = config.OptionGroup(
+    prefix="ssh",
+    options=(
+        {
+            "name": "port",
+            "type": int,
+            "default": Ports.forward.ssh,
+            "help_text": "Port on which external processes can access the database via SSH protocol",
+        },
+    ),
+)
 
 def TestSchemas(value) -> Tuple[str]:
     """
     Parses a test schema spec string.
 
     Args:
         value: spec string for the test schemas.
@@ -112,14 +124,22 @@
     """Returns the configuration settings of the bucketfs for this session."""
     cli_arguments = request.config.option
     kwargs = BUCKETFS.kwargs(os.environ, cli_arguments)
     return config.BucketFs(**kwargs)
 
 
 @pytest.fixture(scope="session")
+def ssh_config(request) -> config.Ssh:
+    """Returns the configuration settings for SSH access in this session."""
+    cli_arguments = request.config.option
+    kwargs = SSH.kwargs(os.environ, cli_arguments)
+    return config.Ssh(**kwargs)
+
+
+@pytest.fixture(scope="session")
 def itde_config(request) -> config.Itde:
     """Returns the configuration settings of the ITDE for this session."""
     cli_arguments = request.config.option
     kwargs = ITDE.kwargs(os.environ, cli_arguments)
     return config.Itde(**kwargs)
 
 
@@ -145,40 +165,41 @@
     yield factory
 
     for connection in connections:
         connection.close()
 
 
 @pytest.fixture(scope="session")
-def _bootstrap_db(itde_config, exasol_config, bucketfs_config):
+def _bootstrap_db(itde_config, exasol_config, bucketfs_config, ssh_config):
     """Bootstraps the database should not be used from outside the itde plugin."""
 
     def nop():
         pass
 
-    def start_db(name, itde, exasol, bucketfs):
+    def start_db(name, itde, exasol, bucketfs, ssh_access):
         from urllib.parse import urlparse
 
         from exasol_integration_test_docker_environment.lib import api
 
         bucketfs_url = urlparse(bucketfs.url)
         _, cleanup_function = api.spawn_test_environment(
             environment_name=name,
             database_port_forward=exasol.port,
             bucketfs_port_forward=bucketfs_url.port,
+            ssh_port_forward=ssh_access.port,
             db_mem_size="4GB",
             docker_db_image_version=itde.db_version,
         )
         return cleanup_function
 
     db_name = "pytest_exasol_db"
     bootstrap_db = itde_config.db_version != "external"
 
     start = (
-        lambda: start_db(db_name, itde_config, exasol_config, bucketfs_config)
+        lambda: start_db(db_name, itde_config, exasol_config, bucketfs_config, ssh_config)
         if bootstrap_db
         else lambda: nop
     )
     stop = start()
     yield
     stop()
 
@@ -207,15 +228,15 @@
     )
 
     for schema in itde_config.schemas:
         connection.execute(f"DROP SCHEMA IF EXISTS {schema} CASCADE;")
         connection.commit()
 
 
-OPTION_GROUPS = (EXASOL, BUCKETFS, ITDE)
+OPTION_GROUPS = (EXASOL, BUCKETFS, ITDE, SSH)
 
 
 def _add_option_group(parser, group):
     parser_group = parser.getgroup(group.prefix)
     for option in group.options:
         parser_group.addoption(
             option.cli,
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/pytest_itde/config.py` & `exasol_integration_test_docker_environment-2.0.0/pytest_itde/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,14 +118,21 @@
 
     url: str
     username: str
     password: str
 
 
 @dataclass
+class Ssh:
+    """SSH configuration"""
+
+    port: int
+
+
+@dataclass
 class Itde:
     """Itde configuration settings"""
 
     db_version: str
     schemas: List[str]
```

### Comparing `exasol_integration_test_docker_environment-1.7.1/PKG-INFO` & `exasol_integration_test_docker_environment-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exasol-integration-test-docker-environment
-Version: 1.7.1
+Version: 2.0.0
 Summary: Integration Test Docker Environment for Exasol
 Home-page: https://github.com/exasol/integration-test-docker-environment
 License: MIT
 Keywords: exasol,docker,testing
 Author: Torsten Kilias
 Author-email: torsten.kilias@exasol.com
 Requires-Python: >=3.8,<4
```

