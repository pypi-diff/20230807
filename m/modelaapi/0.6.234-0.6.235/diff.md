# Comparing `tmp/modelaapi-0.6.234.tar.gz` & `tmp/modelaapi-0.6.235.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.234.tar", last modified: Thu Aug  3 18:08:34 2023, max compression
+gzip compressed data, was "modelaapi-0.6.235.tar", last modified: Mon Aug  7 20:49:10 2023, max compression
```

## Comparing `modelaapi-0.6.234.tar` & `modelaapi-0.6.235.tar`

### file list

```diff
@@ -1,581 +1,581 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.234/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.234/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.234/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.234/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.234/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.234/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-03 18:08:34.927729 modelaapi-0.6.234/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.234/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6763 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24765 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    41839 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    52674 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    91844 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    22799 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35286 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    40354 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.895729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18422 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    55370 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    97138 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8164 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4594 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4881 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3133 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12730 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4263 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.899729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23069 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11572 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7286 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    20675 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    61254 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    64734 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)   104658 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4969 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4644 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5326 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5395 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4276 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.903729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11708 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7194 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    20179 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5885 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    66312 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3961 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5613 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4141 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2012 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.887729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.887729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)     2035 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1010 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     3056 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.907729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18392 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19563 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17943 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4516 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4951 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13520 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2363 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.887729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)    11990 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6559 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    23986 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4035 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.911729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1956 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1204 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4282 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3917 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4820 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1294 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5788 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6533 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5338 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.915729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3883 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4364 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4597 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3815 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4459 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6909 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6597 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.919729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3580 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12936 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4784 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3696 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-08-03 17:26:18.000000 modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      310 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/annotations_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2272 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/http_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/apps/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21422 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/apps/v1/generated_pb2.pyi
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   150106 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6650 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.923729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      579 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23310 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1267 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      135 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      577 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/apps/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/apps/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/core/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/api/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/apis/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/apis/meta/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/pkg/util/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.891729 modelaapi-0.6.234/k8s/io/rbac/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/k8s/io/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-03 17:26:18.000000 modelaapi-0.6.234/k8s/io/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.234/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-08-03 18:08:33.000000 modelaapi-0.6.234/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-03 18:08:34.927729 modelaapi-0.6.234/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    24585 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.234/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-08-03 18:08:34.000000 modelaapi-0.6.234/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.234/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-08-03 18:08:34.931729 modelaapi-0.6.234/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5473 2023-07-21 18:09:27.000000 modelaapi-0.6.234/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.235/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.235/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.235/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.235/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.235/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.235/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-07 20:49:10.540722 modelaapi-0.6.235/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.235/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6763 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24765 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    41839 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    52674 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    91844 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    22799 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35286 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    40354 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18422 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    55414 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    97242 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8164 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4594 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4881 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3133 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12730 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4263 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.508722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23069 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11572 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7286 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20675 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    61368 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    64910 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)   104658 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4969 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4644 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5326 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5395 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.512722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4276 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11708 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7194 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20179 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5885 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    66312 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3961 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5613 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4141 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2012 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.496722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpc/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.496722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpc/health/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpc/health/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2035 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1010 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3056 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.516722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18392 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19563 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17943 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4516 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4951 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13520 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2363 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.496722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclassrun/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclassrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11990 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6559 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23986 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.520722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4035 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1956 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1204 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4282 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3917 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4820 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1294 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5788 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6533 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.524722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5338 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3883 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4364 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4597 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3815 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4459 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6909 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.528722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6597 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3580 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12936 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4784 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3696 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-08-07 20:39:33.000000 modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-08-07 20:39:33.000000 modelaapi-0.6.235/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      310 2023-08-07 20:39:33.000000 modelaapi-0.6.235/google/api/annotations_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-08-07 20:39:33.000000 modelaapi-0.6.235/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2272 2023-08-07 20:39:33.000000 modelaapi-0.6.235/google/api/http_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/api/apps/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21422 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/api/apps/v1/generated_pb2.pyi
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   150106 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/api/core/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.532722 modelaapi-0.6.235/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6650 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/api/rbac/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      579 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23310 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1267 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      135 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      577 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.235/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.500722 modelaapi-0.6.235/k8s/io/apps/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/apps/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.500722 modelaapi-0.6.235/k8s/io/core/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.500722 modelaapi-0.6.235/k8s/io/pkg/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.500722 modelaapi-0.6.235/k8s/io/pkg/api/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.500722 modelaapi-0.6.235/k8s/io/pkg/apis/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.500722 modelaapi-0.6.235/k8s/io/pkg/apis/meta/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.500722 modelaapi-0.6.235/k8s/io/pkg/util/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.504722 modelaapi-0.6.235/k8s/io/rbac/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/k8s/io/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:39:33.000000 modelaapi-0.6.235/k8s/io/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.235/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.235/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.235/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.235/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.235/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-08-07 20:49:02.000000 modelaapi-0.6.235/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:49:10.536722 modelaapi-0.6.235/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-07 20:49:10.000000 modelaapi-0.6.235/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24585 2023-08-07 20:49:10.000000 modelaapi-0.6.235/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-08-07 20:49:10.000000 modelaapi-0.6.235/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-08-07 20:49:10.000000 modelaapi-0.6.235/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.235/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-08-07 20:49:10.000000 modelaapi-0.6.235/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-08-07 20:49:10.000000 modelaapi-0.6.235/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.235/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-08-07 20:49:10.540722 modelaapi-0.6.235/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5473 2023-07-21 18:09:27.000000 modelaapi-0.6.235/setup.py
```

### Comparing `modelaapi-0.6.234/CONTRIBUTING.rst` & `modelaapi-0.6.235/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/LICENSE.txt` & `modelaapi-0.6.235/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/Makefile` & `modelaapi-0.6.235/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/PKG-INFO` & `modelaapi-0.6.235/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.234
+Version: 0.6.235
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.234
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.235
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.234
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.235
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.234/README.md` & `modelaapi-0.6.235/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.235/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi` & `modelaapi-0.6.235/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\xab\x01\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\"O\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1c\n\x14modelsWithNoProgress\x18\x03 \x01(\x05\"\xfb\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12g\n\rbaseEstimator\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xcc\x02\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\x02 \x03(\t\x12\x12\n\nimputation\x18\x03 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x04 \x01(\t\x12\x0f\n\x07scaling\x18\x05 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x06 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x07 \x01(\t\x12\x17\n\x0foutlierHandling\x18\x08 \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\t \x01(\t\x12X\n\x04text\x18\n \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12\x0c\n\x04\x64rop\x18\x0b \x01(\x08\"\x94\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"e\n\x15GarbageCollectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12!\n\x19keepBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xaa\x04\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x11\x65xplainerLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x66\n\x17trainShapValuesLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x65\n\x16testShapValuesLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xd6\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xe7\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18predictionScheduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18monitoringScheduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12h\n\x14reportScheduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x87\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"]\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\talgorithm\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\xe6\x0b\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x11\n\tstudyName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x0f\n\x07subtask\x18\x07 \x01(\t\x12Y\n\tobjective\x18\x08 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0c\n\x04test\x18\r \x01(\x08\x12\r\n\x05\x61\x62ort\x18\x0e \x01(\x08\x12\x0f\n\x07package\x18\x0f \x01(\x08\x12\x0e\n\x06report\x18\x10 \x01(\x08\x12\r\n\x05pause\x18\x11 \x01(\x08\x12\x0f\n\x07profile\x18\x12 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x14 \x01(\x08\x12\x10\n\x08unitTest\x18\x15 \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\x16 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x17 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x18 \x01(\t\x12]\n\x0b\x66orecasting\x18\x19 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x1a \x01(\x03\x12\x15\n\restimatorType\x18\x1b \x01(\t\x12\x12\n\nmodelClass\x18\x1c \x01(\t\x12\x0f\n\x07trialID\x18\x1d \x01(\x05\x12T\n\x08\x61pproval\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x1f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18  \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18! \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12_\n\x0cnotification\x18$ \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xf2\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0fvalidationScore\x18\x08 \x01(\x01\x12\x15\n\rtrainingScore\x18\t \x01(\x01\x12\x11\n\ttestScore\x18\n \x01(\x01\x12X\n\nvalidation\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05phase\x18\x12 \x01(\t\x12\x12\n\nreportName\x18\x13 \x01(\t\x12]\n\x0ereportLocation\x18\x14 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x63\n\x14trainWeightsLocation\x18\x15 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testWeightsLocation\x18\x16 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13\x66ullWeightsLocation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19trainLabelEncoderLocation\x18\x18 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x1b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19misclassificationLocation\x18\x1c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\x10\x66orecastLocation\x18\x1d \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fpackageLocation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12g\n\x12impurityImportance\x18\x1f \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18  \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12X\n\x07runtime\x18! \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18# \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18$ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18% \x01(\x03\x12\x14\n\x0ctrainingRows\x18& \x01(\x05\x12\x13\n\x0btestingRows\x18\' \x01(\x05\x12\x16\n\x0evalidationRows\x18( \x01(\x05\x12\x16\n\x0e\x66\x61ilureMessage\x18* \x01(\t\x12\x10\n\x08progress\x18+ \x01(\x05\x12\x13\n\x0b\x64\x61tasetName\x18, \x01(\t\x12\x16\n\x0e\x64\x61taSourceName\x18- \x01(\t\x12X\n\x07serving\x18/ \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12\x13\n\x0btarFileHash\x18\x30 \x01(\t\x12^\n\x10trainingDataHash\x18\x31 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18\x32 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18\x33 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18\x34 \x01(\t\x12K\n\x04logs\x18\x35 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x36 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x37 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x38 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x39 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18: \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18; \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18< \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18= \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18> \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18? \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestResults\x18@ \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestResults\x18\x41 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18\x42 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12[\n\x05usage\x18\x44 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x45 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"=\n\x10OutlierModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe9\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nreportType\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\x06 \x01(\t\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x08 \x01(\x03\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\n \x03(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x0b \x01(\t\x12\x16\n\x0emodelClassName\x18\x0c \x01(\t\x12\x19\n\x11modelClassRunName\x18\r \x01(\t\"\xb3\x04\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xde\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x10\n\x08maxScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\r \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x62\n\x12secondaryObjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04goal\x18\x0f \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xd2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\x7f\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x19\n\x11predictorEndpoint\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61shboardEndpoint\x18\x05 \x01(\t\x12\x0c\n\x04role\x18\x06 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xc9\x0e\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x05 \x01(\t\x12\x0f\n\x07subtask\x18\x06 \x01(\t\x12l\n\x12\x66\x65\x61tureEngineering\x18\x07 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12i\n\x10imbalanceHandler\x18\x08 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\x0b \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x62\n\x10\x66orecastTemplate\x18\r \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x0f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0coutlierModel\x18\x10 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.OutlierModelSpec\x12\r\n\x05\x61\x62ort\x18\x11 \x01(\x08\x12\x0e\n\x06report\x18\x12 \x01(\x08\x12\r\n\x05pause\x18\x13 \x01(\x08\x12\x0f\n\x07profile\x18\x14 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x15 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x16 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x17 \x01(\t\x12\r\n\x05owner\x18\x18 \x01(\t\x12\x10\n\x08template\x18\x19 \x01(\x08\x12_\n\x0cnotification\x18\x1a \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12[\n\x02gc\x18\x1b \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x14\n\x0cmodelVersion\x18\x1c \x01(\t\x12\x0f\n\x07timeout\x18\x1d \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18\x1f \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18  \x01(\t\x12\x19\n\x11modelClassRunName\x18! \x01(\t\x12V\n\x07serving\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xa4\x0f\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x03 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x04 \x01(\x01\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12]\n\x0ereportLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nreportName\x18\x07 \x01(\t\x12\r\n\x05phase\x18\x08 \x01(\t\x12\x1a\n\x12observedGeneration\x18\t \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11optimizerLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x15 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x16 \x01(\t\x12K\n\x04logs\x18\x17 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\\\n\x08\x62\x61seline\x18\x18 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1d \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18\x1e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12]\n\x02gc\x18\x1f \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12\x43\n\nconditions\x18  \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\xe2\x04\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x0f\n\x07timeout\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\xab\x01\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\"O\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1c\n\x14modelsWithNoProgress\x18\x03 \x01(\x05\"\xfb\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12g\n\rbaseEstimator\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xde\x02\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61taType\x18\x02 \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12\x0c\n\x04\x64rop\x18\x0c \x01(\x08\"\x94\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"e\n\x15GarbageCollectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12!\n\x19keepBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xaa\x04\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x11\x65xplainerLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x66\n\x17trainShapValuesLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x65\n\x16testShapValuesLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xd6\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xe7\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18predictionScheduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18monitoringScheduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12h\n\x14reportScheduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x87\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"]\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\talgorithm\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\xe6\x0b\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x11\n\tstudyName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x0f\n\x07subtask\x18\x07 \x01(\t\x12Y\n\tobjective\x18\x08 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0c\n\x04test\x18\r \x01(\x08\x12\r\n\x05\x61\x62ort\x18\x0e \x01(\x08\x12\x0f\n\x07package\x18\x0f \x01(\x08\x12\x0e\n\x06report\x18\x10 \x01(\x08\x12\r\n\x05pause\x18\x11 \x01(\x08\x12\x0f\n\x07profile\x18\x12 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x14 \x01(\x08\x12\x10\n\x08unitTest\x18\x15 \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\x16 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x17 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x18 \x01(\t\x12]\n\x0b\x66orecasting\x18\x19 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x1a \x01(\x03\x12\x15\n\restimatorType\x18\x1b \x01(\t\x12\x12\n\nmodelClass\x18\x1c \x01(\t\x12\x0f\n\x07trialID\x18\x1d \x01(\x05\x12T\n\x08\x61pproval\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x1f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18  \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18! \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12_\n\x0cnotification\x18$ \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xf2\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0fvalidationScore\x18\x08 \x01(\x01\x12\x15\n\rtrainingScore\x18\t \x01(\x01\x12\x11\n\ttestScore\x18\n \x01(\x01\x12X\n\nvalidation\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05phase\x18\x12 \x01(\t\x12\x12\n\nreportName\x18\x13 \x01(\t\x12]\n\x0ereportLocation\x18\x14 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x63\n\x14trainWeightsLocation\x18\x15 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testWeightsLocation\x18\x16 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13\x66ullWeightsLocation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19trainLabelEncoderLocation\x18\x18 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x1b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19misclassificationLocation\x18\x1c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\x10\x66orecastLocation\x18\x1d \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fpackageLocation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12g\n\x12impurityImportance\x18\x1f \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18  \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12X\n\x07runtime\x18! \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18# \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18$ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18% \x01(\x03\x12\x14\n\x0ctrainingRows\x18& \x01(\x05\x12\x13\n\x0btestingRows\x18\' \x01(\x05\x12\x16\n\x0evalidationRows\x18( \x01(\x05\x12\x16\n\x0e\x66\x61ilureMessage\x18* \x01(\t\x12\x10\n\x08progress\x18+ \x01(\x05\x12\x13\n\x0b\x64\x61tasetName\x18, \x01(\t\x12\x16\n\x0e\x64\x61taSourceName\x18- \x01(\t\x12X\n\x07serving\x18/ \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12\x13\n\x0btarFileHash\x18\x30 \x01(\t\x12^\n\x10trainingDataHash\x18\x31 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18\x32 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18\x33 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18\x34 \x01(\t\x12K\n\x04logs\x18\x35 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x36 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x37 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x38 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x39 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18: \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18; \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18< \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18= \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18> \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18? \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestResults\x18@ \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestResults\x18\x41 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18\x42 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12[\n\x05usage\x18\x44 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x45 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"=\n\x10OutlierModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe9\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nreportType\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\x06 \x01(\t\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x08 \x01(\x03\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\n \x03(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x0b \x01(\t\x12\x16\n\x0emodelClassName\x18\x0c \x01(\t\x12\x19\n\x11modelClassRunName\x18\r \x01(\t\"\xb3\x04\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xde\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x10\n\x08maxScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\r \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x62\n\x12secondaryObjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04goal\x18\x0f \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xd2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\x7f\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x19\n\x11predictorEndpoint\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61shboardEndpoint\x18\x05 \x01(\t\x12\x0c\n\x04role\x18\x06 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xc9\x0e\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x05 \x01(\t\x12\x0f\n\x07subtask\x18\x06 \x01(\t\x12l\n\x12\x66\x65\x61tureEngineering\x18\x07 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12i\n\x10imbalanceHandler\x18\x08 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\x0b \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x62\n\x10\x66orecastTemplate\x18\r \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x0f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0coutlierModel\x18\x10 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.OutlierModelSpec\x12\r\n\x05\x61\x62ort\x18\x11 \x01(\x08\x12\x0e\n\x06report\x18\x12 \x01(\x08\x12\r\n\x05pause\x18\x13 \x01(\x08\x12\x0f\n\x07profile\x18\x14 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x15 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x16 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x17 \x01(\t\x12\r\n\x05owner\x18\x18 \x01(\t\x12\x10\n\x08template\x18\x19 \x01(\x08\x12_\n\x0cnotification\x18\x1a \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12[\n\x02gc\x18\x1b \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x14\n\x0cmodelVersion\x18\x1c \x01(\t\x12\x0f\n\x07timeout\x18\x1d \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18\x1f \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18  \x01(\t\x12\x19\n\x11modelClassRunName\x18! \x01(\t\x12V\n\x07serving\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xa4\x0f\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x03 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x04 \x01(\x01\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12]\n\x0ereportLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nreportName\x18\x07 \x01(\t\x12\r\n\x05phase\x18\x08 \x01(\t\x12\x1a\n\x12observedGeneration\x18\t \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11optimizerLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x15 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x16 \x01(\t\x12K\n\x04logs\x18\x17 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\\\n\x08\x62\x61seline\x18\x18 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1d \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18\x1e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12]\n\x02gc\x18\x1f \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12\x43\n\nconditions\x18  \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\xe2\x04\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x0f\n\x07timeout\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1'
@@ -68,149 +68,149 @@
   _ENTITYREF._serialized_start=2597
   _ENTITYREF._serialized_end=2639
   _EVALMETRICS._serialized_start=2642
   _EVALMETRICS._serialized_end=2779
   _EVALPERIOD._serialized_start=2782
   _EVALPERIOD._serialized_end=3006
   _FEATUREENGINEERINGPIPELINE._serialized_start=3009
-  _FEATUREENGINEERINGPIPELINE._serialized_end=3341
-  _FEATUREENGINEERINGSPEC._serialized_start=3344
-  _FEATUREENGINEERINGSPEC._serialized_end=3492
-  _FEATUREIMPORTANCE._serialized_start=3494
-  _FEATUREIMPORTANCE._serialized_end=3550
-  _FEATUREINFO._serialized_start=3552
-  _FEATUREINFO._serialized_end=3610
-  _FEATUREPAIR._serialized_start=3612
-  _FEATUREPAIR._serialized_end=3647
-  _FEATURESELECTIONSPEC._serialized_start=3650
-  _FEATURESELECTIONSPEC._serialized_end=3863
-  _FORECASTERSPEC._serialized_start=3866
-  _FORECASTERSPEC._serialized_end=4882
-  _GARBAGECOLLECTIONSPEC._serialized_start=4884
-  _GARBAGECOLLECTIONSPEC._serialized_end=4985
-  _GARBAGECOLLECTIONSTATUS._serialized_start=4988
-  _GARBAGECOLLECTIONSTATUS._serialized_end=5130
-  _GENERATEDCOLUMNSPEC._serialized_start=5132
-  _GENERATEDCOLUMNSPEC._serialized_end=5234
-  _GROUPSPLITLOCATIONSSPEC._serialized_start=5236
-  _GROUPSPLITLOCATIONSSPEC._serialized_end=5322
-  _HYPERPARAMETERVALUE._serialized_start=5324
-  _HYPERPARAMETERVALUE._serialized_end=5374
-  _HYPERBANDOPTIONS._serialized_start=5376
-  _HYPERBANDOPTIONS._serialized_end=5487
-  _IMAGEPIPELINESPEC._serialized_start=5489
-  _IMAGEPIPELINESPEC._serialized_end=5528
-  _IMBALANCEHANDLINGSPEC._serialized_start=5530
-  _IMBALANCEHANDLINGSPEC._serialized_end=5589
-  _INTERPRETABILITYSPEC._serialized_start=5592
-  _INTERPRETABILITYSPEC._serialized_end=5874
-  _INTERPRETABILITYSTATUS._serialized_start=5877
-  _INTERPRETABILITYSTATUS._serialized_end=6431
-  _MEDIANPRUNEROPTIONS._serialized_start=6433
-  _MEDIANPRUNEROPTIONS._serialized_end=6540
-  _MODEL._serialized_start=6543
-  _MODEL._serialized_end=6788
-  _MODELCLASS._serialized_start=6791
-  _MODELCLASS._serialized_end=7051
-  _MODELCLASSDATASPEC._serialized_start=7054
-  _MODELCLASSDATASPEC._serialized_end=7643
-  _MODELCLASSLIST._serialized_start=7646
-  _MODELCLASSLIST._serialized_end=7813
-  _MODELCLASSRUN._serialized_start=7816
-  _MODELCLASSRUN._serialized_end=8085
-  _MODELCLASSRUNLIST._serialized_start=8088
-  _MODELCLASSRUNLIST._serialized_end=8261
-  _MODELCLASSRUNSPEC._serialized_start=8264
-  _MODELCLASSRUNSPEC._serialized_end=8470
-  _MODELCLASSRUNSTATUS._serialized_start=8473
-  _MODELCLASSRUNSTATUS._serialized_end=9071
-  _MODELCLASSSERVINGSPEC._serialized_start=9074
-  _MODELCLASSSERVINGSPEC._serialized_end=9415
-  _MODELCLASSSPEC._serialized_start=9418
-  _MODELCLASSSPEC._serialized_end=10259
-  _MODELCLASSSTATUS._serialized_start=10262
-  _MODELCLASSSTATUS._serialized_end=11389
-  _MODELCLASSTRAININGSPEC._serialized_start=11392
-  _MODELCLASSTRAININGSPEC._serialized_end=12039
-  _MODELGROUPBYSTATUS._serialized_start=12042
-  _MODELGROUPBYSTATUS._serialized_end=12221
-  _MODELLIST._serialized_start=12224
-  _MODELLIST._serialized_end=12381
-  _MODELRESULT._serialized_start=12383
-  _MODELRESULT._serialized_end=12476
-  _MODELSPEC._serialized_start=12479
-  _MODELSPEC._serialized_end=13989
-  _MODELSTAGESTATUS._serialized_start=13992
-  _MODELSTAGESTATUS._serialized_end=14267
-  _MODELSTATUS._serialized_start=14270
-  _MODELSTATUS._serialized_end=18736
-  _MODELTESTSUITE._serialized_start=18739
-  _MODELTESTSUITE._serialized_end=18962
-  _NNLAYERPARAMETER._serialized_start=18964
-  _NNLAYERPARAMETER._serialized_end=19011
-  _OUTLIERMODELSPEC._serialized_start=19013
-  _OUTLIERMODELSPEC._serialized_end=19074
-  _PARTITIONMODELLOCATIONSSPEC._serialized_start=19077
-  _PARTITIONMODELLOCATIONSSPEC._serialized_end=19281
-  _PERCENTILEPRUNEROPTIONS._serialized_start=19284
-  _PERCENTILEPRUNEROPTIONS._serialized_end=19416
-  _PRUNERSPEC._serialized_start=19419
-  _PRUNERSPEC._serialized_end=19950
-  _REGRESSIONFORECASTERSPEC._serialized_start=19953
-  _REGRESSIONFORECASTERSPEC._serialized_end=20161
-  _REPORT._serialized_start=20164
-  _REPORT._serialized_end=20412
-  _REPORTGROUPBYSTATUS._serialized_start=20415
-  _REPORTGROUPBYSTATUS._serialized_end=20553
-  _REPORTLIST._serialized_start=20556
-  _REPORTLIST._serialized_end=20715
-  _REPORTSPEC._serialized_start=20718
-  _REPORTSPEC._serialized_end=21207
-  _REPORTSTATUS._serialized_start=21210
-  _REPORTSTATUS._serialized_end=21773
-  _RUNTIMESTATUS._serialized_start=21776
-  _RUNTIMESTATUS._serialized_end=21998
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=21945
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=21998
-  _SEARCHSPEC._serialized_start=22001
-  _SEARCHSPEC._serialized_end=22644
-  _SEASONALITYPERIODSPEC._serialized_start=22646
-  _SEASONALITYPERIODSPEC._serialized_end=22722
-  _SEASONALITYSPEC._serialized_start=22725
-  _SEASONALITYSPEC._serialized_end=23244
-  _SERVINGENVIRONMENT._serialized_start=23247
-  _SERVINGENVIRONMENT._serialized_end=23686
-  _SERVINGSPEC._serialized_start=23689
-  _SERVINGSPEC._serialized_end=24155
-  _SERVINGSTATUS._serialized_start=24157
-  _SERVINGSTATUS._serialized_end=24284
-  _STUDY._serialized_start=24287
-  _STUDY._serialized_end=24532
-  _STUDYLIST._serialized_start=24535
-  _STUDYLIST._serialized_end=24692
-  _STUDYPHASESTATUS._serialized_start=24695
-  _STUDYPHASESTATUS._serialized_end=25003
-  _STUDYSCHEDULESPEC._serialized_start=25005
-  _STUDYSCHEDULESPEC._serialized_end=25102
-  _STUDYSPEC._serialized_start=25105
-  _STUDYSPEC._serialized_end=26970
-  _STUDYSTATUS._serialized_start=26973
-  _STUDYSTATUS._serialized_end=28929
-  _SUCCESSIVEHALVINGOPTIONS._serialized_start=28931
-  _SUCCESSIVEHALVINGOPTIONS._serialized_end=29058
-  _SUCCESSIVEHALVINGSPEC._serialized_start=29060
-  _SUCCESSIVEHALVINGSPEC._serialized_end=29164
-  _TEXTPIPELINESPEC._serialized_start=29167
-  _TEXTPIPELINESPEC._serialized_end=29340
-  _THRESHOLDPRUNEROPTIONS._serialized_start=29342
-  _THRESHOLDPRUNEROPTIONS._serialized_end=29440
-  _TIMESERIESEVENT._serialized_start=29443
-  _TIMESERIESEVENT._serialized_end=29581
-  _TRAININGSPEC._serialized_start=29584
-  _TRAININGSPEC._serialized_end=30194
-  _UNIVARIATEFORECASTSTATUS._serialized_start=30197
-  _UNIVARIATEFORECASTSTATUS._serialized_end=30417
-  _VIDEOPIPELINESPEC._serialized_start=30419
-  _VIDEOPIPELINESPEC._serialized_end=30458
-  _WINDOWSPEC._serialized_start=30460
-  _WINDOWSPEC._serialized_end=30521
+  _FEATUREENGINEERINGPIPELINE._serialized_end=3359
+  _FEATUREENGINEERINGSPEC._serialized_start=3362
+  _FEATUREENGINEERINGSPEC._serialized_end=3510
+  _FEATUREIMPORTANCE._serialized_start=3512
+  _FEATUREIMPORTANCE._serialized_end=3568
+  _FEATUREINFO._serialized_start=3570
+  _FEATUREINFO._serialized_end=3628
+  _FEATUREPAIR._serialized_start=3630
+  _FEATUREPAIR._serialized_end=3665
+  _FEATURESELECTIONSPEC._serialized_start=3668
+  _FEATURESELECTIONSPEC._serialized_end=3881
+  _FORECASTERSPEC._serialized_start=3884
+  _FORECASTERSPEC._serialized_end=4900
+  _GARBAGECOLLECTIONSPEC._serialized_start=4902
+  _GARBAGECOLLECTIONSPEC._serialized_end=5003
+  _GARBAGECOLLECTIONSTATUS._serialized_start=5006
+  _GARBAGECOLLECTIONSTATUS._serialized_end=5148
+  _GENERATEDCOLUMNSPEC._serialized_start=5150
+  _GENERATEDCOLUMNSPEC._serialized_end=5252
+  _GROUPSPLITLOCATIONSSPEC._serialized_start=5254
+  _GROUPSPLITLOCATIONSSPEC._serialized_end=5340
+  _HYPERPARAMETERVALUE._serialized_start=5342
+  _HYPERPARAMETERVALUE._serialized_end=5392
+  _HYPERBANDOPTIONS._serialized_start=5394
+  _HYPERBANDOPTIONS._serialized_end=5505
+  _IMAGEPIPELINESPEC._serialized_start=5507
+  _IMAGEPIPELINESPEC._serialized_end=5546
+  _IMBALANCEHANDLINGSPEC._serialized_start=5548
+  _IMBALANCEHANDLINGSPEC._serialized_end=5607
+  _INTERPRETABILITYSPEC._serialized_start=5610
+  _INTERPRETABILITYSPEC._serialized_end=5892
+  _INTERPRETABILITYSTATUS._serialized_start=5895
+  _INTERPRETABILITYSTATUS._serialized_end=6449
+  _MEDIANPRUNEROPTIONS._serialized_start=6451
+  _MEDIANPRUNEROPTIONS._serialized_end=6558
+  _MODEL._serialized_start=6561
+  _MODEL._serialized_end=6806
+  _MODELCLASS._serialized_start=6809
+  _MODELCLASS._serialized_end=7069
+  _MODELCLASSDATASPEC._serialized_start=7072
+  _MODELCLASSDATASPEC._serialized_end=7661
+  _MODELCLASSLIST._serialized_start=7664
+  _MODELCLASSLIST._serialized_end=7831
+  _MODELCLASSRUN._serialized_start=7834
+  _MODELCLASSRUN._serialized_end=8103
+  _MODELCLASSRUNLIST._serialized_start=8106
+  _MODELCLASSRUNLIST._serialized_end=8279
+  _MODELCLASSRUNSPEC._serialized_start=8282
+  _MODELCLASSRUNSPEC._serialized_end=8488
+  _MODELCLASSRUNSTATUS._serialized_start=8491
+  _MODELCLASSRUNSTATUS._serialized_end=9089
+  _MODELCLASSSERVINGSPEC._serialized_start=9092
+  _MODELCLASSSERVINGSPEC._serialized_end=9433
+  _MODELCLASSSPEC._serialized_start=9436
+  _MODELCLASSSPEC._serialized_end=10277
+  _MODELCLASSSTATUS._serialized_start=10280
+  _MODELCLASSSTATUS._serialized_end=11407
+  _MODELCLASSTRAININGSPEC._serialized_start=11410
+  _MODELCLASSTRAININGSPEC._serialized_end=12057
+  _MODELGROUPBYSTATUS._serialized_start=12060
+  _MODELGROUPBYSTATUS._serialized_end=12239
+  _MODELLIST._serialized_start=12242
+  _MODELLIST._serialized_end=12399
+  _MODELRESULT._serialized_start=12401
+  _MODELRESULT._serialized_end=12494
+  _MODELSPEC._serialized_start=12497
+  _MODELSPEC._serialized_end=14007
+  _MODELSTAGESTATUS._serialized_start=14010
+  _MODELSTAGESTATUS._serialized_end=14285
+  _MODELSTATUS._serialized_start=14288
+  _MODELSTATUS._serialized_end=18754
+  _MODELTESTSUITE._serialized_start=18757
+  _MODELTESTSUITE._serialized_end=18980
+  _NNLAYERPARAMETER._serialized_start=18982
+  _NNLAYERPARAMETER._serialized_end=19029
+  _OUTLIERMODELSPEC._serialized_start=19031
+  _OUTLIERMODELSPEC._serialized_end=19092
+  _PARTITIONMODELLOCATIONSSPEC._serialized_start=19095
+  _PARTITIONMODELLOCATIONSSPEC._serialized_end=19299
+  _PERCENTILEPRUNEROPTIONS._serialized_start=19302
+  _PERCENTILEPRUNEROPTIONS._serialized_end=19434
+  _PRUNERSPEC._serialized_start=19437
+  _PRUNERSPEC._serialized_end=19968
+  _REGRESSIONFORECASTERSPEC._serialized_start=19971
+  _REGRESSIONFORECASTERSPEC._serialized_end=20179
+  _REPORT._serialized_start=20182
+  _REPORT._serialized_end=20430
+  _REPORTGROUPBYSTATUS._serialized_start=20433
+  _REPORTGROUPBYSTATUS._serialized_end=20571
+  _REPORTLIST._serialized_start=20574
+  _REPORTLIST._serialized_end=20733
+  _REPORTSPEC._serialized_start=20736
+  _REPORTSPEC._serialized_end=21225
+  _REPORTSTATUS._serialized_start=21228
+  _REPORTSTATUS._serialized_end=21791
+  _RUNTIMESTATUS._serialized_start=21794
+  _RUNTIMESTATUS._serialized_end=22016
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=21963
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=22016
+  _SEARCHSPEC._serialized_start=22019
+  _SEARCHSPEC._serialized_end=22662
+  _SEASONALITYPERIODSPEC._serialized_start=22664
+  _SEASONALITYPERIODSPEC._serialized_end=22740
+  _SEASONALITYSPEC._serialized_start=22743
+  _SEASONALITYSPEC._serialized_end=23262
+  _SERVINGENVIRONMENT._serialized_start=23265
+  _SERVINGENVIRONMENT._serialized_end=23704
+  _SERVINGSPEC._serialized_start=23707
+  _SERVINGSPEC._serialized_end=24173
+  _SERVINGSTATUS._serialized_start=24175
+  _SERVINGSTATUS._serialized_end=24302
+  _STUDY._serialized_start=24305
+  _STUDY._serialized_end=24550
+  _STUDYLIST._serialized_start=24553
+  _STUDYLIST._serialized_end=24710
+  _STUDYPHASESTATUS._serialized_start=24713
+  _STUDYPHASESTATUS._serialized_end=25021
+  _STUDYSCHEDULESPEC._serialized_start=25023
+  _STUDYSCHEDULESPEC._serialized_end=25120
+  _STUDYSPEC._serialized_start=25123
+  _STUDYSPEC._serialized_end=26988
+  _STUDYSTATUS._serialized_start=26991
+  _STUDYSTATUS._serialized_end=28947
+  _SUCCESSIVEHALVINGOPTIONS._serialized_start=28949
+  _SUCCESSIVEHALVINGOPTIONS._serialized_end=29076
+  _SUCCESSIVEHALVINGSPEC._serialized_start=29078
+  _SUCCESSIVEHALVINGSPEC._serialized_end=29182
+  _TEXTPIPELINESPEC._serialized_start=29185
+  _TEXTPIPELINESPEC._serialized_end=29358
+  _THRESHOLDPRUNEROPTIONS._serialized_start=29360
+  _THRESHOLDPRUNEROPTIONS._serialized_end=29458
+  _TIMESERIESEVENT._serialized_start=29461
+  _TIMESERIESEVENT._serialized_end=29599
+  _TRAININGSPEC._serialized_start=29602
+  _TRAININGSPEC._serialized_end=30212
+  _UNIVARIATEFORECASTSTATUS._serialized_start=30215
+  _UNIVARIATEFORECASTSTATUS._serialized_end=30435
+  _VIDEOPIPELINESPEC._serialized_start=30437
+  _VIDEOPIPELINESPEC._serialized_end=30476
+  _WINDOWSPEC._serialized_start=30478
+  _WINDOWSPEC._serialized_end=30539
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -242,38 +242,40 @@
     cvPeriodsBetweenSplits: int
     cvUseMostRecentSplits: bool
     periodsBetweenTrainTest: int
     testHorizon: int
     def __init__(self, testHorizon: _Optional[int] = ..., periodsBetweenTrainTest: _Optional[int] = ..., cvPeriodsBetweenSplits: _Optional[int] = ..., cvExpandingWindows: bool = ..., cvHorizon: _Optional[int] = ..., cvMinTrainPeriods: _Optional[int] = ..., cvMaxSplits: _Optional[int] = ..., cvUseMostRecentSplits: bool = ...) -> None: ...
 
 class FeatureEngineeringPipeline(_message.Message):
-    __slots__ = ["datetimeTransformation", "discretisation", "drop", "encoding", "features", "imputation", "name", "outlierHandling", "scaling", "text", "variableTransformation"]
+    __slots__ = ["dataType", "datetimeTransformation", "discretisation", "drop", "encoding", "features", "imputation", "name", "outlierHandling", "scaling", "text", "variableTransformation"]
+    DATATYPE_FIELD_NUMBER: _ClassVar[int]
     DATETIMETRANSFORMATION_FIELD_NUMBER: _ClassVar[int]
     DISCRETISATION_FIELD_NUMBER: _ClassVar[int]
     DROP_FIELD_NUMBER: _ClassVar[int]
     ENCODING_FIELD_NUMBER: _ClassVar[int]
     FEATURES_FIELD_NUMBER: _ClassVar[int]
     IMPUTATION_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     OUTLIERHANDLING_FIELD_NUMBER: _ClassVar[int]
     SCALING_FIELD_NUMBER: _ClassVar[int]
     TEXT_FIELD_NUMBER: _ClassVar[int]
     VARIABLETRANSFORMATION_FIELD_NUMBER: _ClassVar[int]
+    dataType: str
     datetimeTransformation: str
     discretisation: str
     drop: bool
     encoding: str
     features: _containers.RepeatedScalarFieldContainer[str]
     imputation: str
     name: str
     outlierHandling: str
     scaling: str
     text: TextPipelineSpec
     variableTransformation: str
-    def __init__(self, name: _Optional[str] = ..., features: _Optional[_Iterable[str]] = ..., imputation: _Optional[str] = ..., encoding: _Optional[str] = ..., scaling: _Optional[str] = ..., discretisation: _Optional[str] = ..., variableTransformation: _Optional[str] = ..., outlierHandling: _Optional[str] = ..., datetimeTransformation: _Optional[str] = ..., text: _Optional[_Union[TextPipelineSpec, _Mapping]] = ..., drop: bool = ...) -> None: ...
+    def __init__(self, name: _Optional[str] = ..., dataType: _Optional[str] = ..., features: _Optional[_Iterable[str]] = ..., imputation: _Optional[str] = ..., encoding: _Optional[str] = ..., scaling: _Optional[str] = ..., discretisation: _Optional[str] = ..., variableTransformation: _Optional[str] = ..., outlierHandling: _Optional[str] = ..., datetimeTransformation: _Optional[str] = ..., text: _Optional[_Union[TextPipelineSpec, _Mapping]] = ..., drop: bool = ...) -> None: ...
 
 class FeatureEngineeringSpec(_message.Message):
     __slots__ = ["imbalance", "pipelines"]
     IMBALANCE_FIELD_NUMBER: _ClassVar[int]
     PIPELINES_FIELD_NUMBER: _ClassVar[int]
     imbalance: str
     pipelines: _containers.RepeatedCompositeFieldContainer[FeatureEngineeringPipeline]
```

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_inference_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_common_dot_v1_dot_common__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xa2\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa8\x03\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xf4\x03\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xae\x03\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xfd\x03\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xf6\x07\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x06 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\t \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\n \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xc8\x03\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe6\x04\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"~\n\x1c\x44sCreateModelProfileResponse\x12^\n\x0fprofileLocation\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x83\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xe7\x04\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"~\n\x1c\x44sCreateStudyProfileResponse\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe8\x06\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\n \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xd2\x03\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12U\n\x06target\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0c\n\x04rows\x18\x06 \x01(\x05\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xcf\x05\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12^\n\x0ftrainingDataset\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12]\n\x0etestingDataset\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"\xc3\x03\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x14\n\x0ctrainingHash\x18\x04 \x01(\t\x12\x13\n\x0btestingHash\x18\x05 \x01(\t\x12\x16\n\x0evalidationHash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\x12\\\n\rtrainLocation\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12[\n\x0ctestLocation\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x61\n\x12validationLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x80\x03\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\r\n\x05rungs\x18\x05 \x01(\x05\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\xea\x02\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x86\x04\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xd7\x08\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xc3\x01\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Q\n\x07reports\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xc1\x03\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12P\n\x06report\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe4\x04\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xc2\x04\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x07 \x01(\x05\x12\x11\n\tdefaultHP\x18\x08 \x01(\x08\x12\x11\n\talgorithm\x18\t \x01(\t\x12V\n\nalgorithms\x18\n \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xeb\x02\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xc9\x03\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xe0\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xae\x04\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x10\n\x08\x61lgnames\x18\x07 \x03(\t\x12\x0b\n\x03\x61ll\x18\x08 \x01(\x08\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb5\x04\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x95\x04\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\xb9\x01\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\x16\n\x14\x44sStudyEndedResponse\"\x92\x02\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"r\n\x17SaveOptimizerDBResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x8d\x02\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x14\n\x12\x44sSnapshotResponse\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xca\x03\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelClass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelClassRun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x08\x65ntities\x18\x04 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\x05 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"r\n\x17GenTrainingDataResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xa5\x04\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xf1\x04\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xb6\x04\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xfb\x02\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf0?\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xa2\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa8\x03\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xf4\x03\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xae\x03\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xfd\x03\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xf6\x07\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x06 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\t \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\n \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xc8\x03\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe6\x04\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"~\n\x1c\x44sCreateModelProfileResponse\x12^\n\x0fprofileLocation\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x83\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xe7\x04\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"~\n\x1c\x44sCreateStudyProfileResponse\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe8\x06\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\n \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xd2\x03\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12U\n\x06target\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0c\n\x04rows\x18\x06 \x01(\x05\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xcf\x05\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12^\n\x0ftrainingDataset\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12]\n\x0etestingDataset\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"\xc3\x03\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x14\n\x0ctrainingHash\x18\x04 \x01(\t\x12\x13\n\x0btestingHash\x18\x05 \x01(\t\x12\x16\n\x0evalidationHash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\x12\\\n\rtrainLocation\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12[\n\x0ctestLocation\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x61\n\x12validationLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x80\x03\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\r\n\x05rungs\x18\x05 \x01(\x05\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\xea\x02\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x86\x04\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xd7\x08\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xc3\x01\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Q\n\x07reports\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xc1\x03\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12P\n\x06report\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe4\x04\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xc2\x04\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x07 \x01(\x05\x12\x11\n\tdefaultHP\x18\x08 \x01(\x08\x12\x11\n\talgorithm\x18\t \x01(\t\x12V\n\nalgorithms\x18\n \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xeb\x02\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xc9\x03\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xe0\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xae\x04\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x10\n\x08\x61lgnames\x18\x07 \x03(\t\x12\x0b\n\x03\x61ll\x18\x08 \x01(\x08\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb5\x04\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x95\x04\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\xb9\x01\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\x16\n\x14\x44sStudyEndedResponse\"\x92\x02\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"r\n\x17SaveOptimizerDBResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xe6\x02\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"\x14\n\x12\x44sSnapshotResponse\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xca\x03\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelClass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelClassRun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x08\x65ntities\x18\x04 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\x05 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"r\n\x17GenTrainingDataResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xa5\x04\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xf1\x04\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xb6\x04\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xfb\x02\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf0?\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.data.v1.data_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z.github.com/metaprov/modelaapi/services/data/v1'
@@ -223,57 +223,57 @@
   _DSGETTABLESRESPONSE._serialized_start=20600
   _DSGETTABLESRESPONSE._serialized_end=20637
   _DSEXECUTESQLREQUEST._serialized_start=20639
   _DSEXECUTESQLREQUEST._serialized_end=20760
   _DSEXECUTESQLRESPONSE._serialized_start=20762
   _DSEXECUTESQLRESPONSE._serialized_end=20864
   _DSSNAPSHOTREQUEST._serialized_start=20867
-  _DSSNAPSHOTREQUEST._serialized_end=21136
-  _DSSNAPSHOTRESPONSE._serialized_start=21138
-  _DSSNAPSHOTRESPONSE._serialized_end=21158
-  _ASKMODELRESPONSE._serialized_start=21160
-  _ASKMODELRESPONSE._serialized_end=21258
-  _GENTRAININGDATAREQUEST._serialized_start=21261
-  _GENTRAININGDATAREQUEST._serialized_end=21719
-  _GENTRAININGDATARESPONSE._serialized_start=21721
-  _GENTRAININGDATARESPONSE._serialized_end=21835
-  _SYNCONLINESTOREREQUEST._serialized_start=21838
-  _SYNCONLINESTOREREQUEST._serialized_end=22713
+  _DSSNAPSHOTREQUEST._serialized_end=21225
+  _DSSNAPSHOTRESPONSE._serialized_start=21227
+  _DSSNAPSHOTRESPONSE._serialized_end=21247
+  _ASKMODELRESPONSE._serialized_start=21249
+  _ASKMODELRESPONSE._serialized_end=21347
+  _GENTRAININGDATAREQUEST._serialized_start=21350
+  _GENTRAININGDATAREQUEST._serialized_end=21808
+  _GENTRAININGDATARESPONSE._serialized_start=21810
+  _GENTRAININGDATARESPONSE._serialized_end=21924
+  _SYNCONLINESTOREREQUEST._serialized_start=21927
+  _SYNCONLINESTOREREQUEST._serialized_end=22802
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_start=4342
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_end=4394
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_start=4396
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_end=4443
-  _SYNCONLINESTORERESPONSE._serialized_start=22715
-  _SYNCONLINESTORERESPONSE._serialized_end=22740
-  _GENONLINESTOREDATASETREQUEST._serialized_start=22743
-  _GENONLINESTOREDATASETREQUEST._serialized_end=23636
+  _SYNCONLINESTORERESPONSE._serialized_start=22804
+  _SYNCONLINESTORERESPONSE._serialized_end=22829
+  _GENONLINESTOREDATASETREQUEST._serialized_start=22832
+  _GENONLINESTOREDATASETREQUEST._serialized_end=23725
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_start=4342
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_end=4394
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_start=4396
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_end=4443
-  _GENONLINESTOREDATASETRESPONSE._serialized_start=23638
-  _GENONLINESTOREDATASETRESPONSE._serialized_end=23758
-  _BATCHPREDICTREQUEST._serialized_start=23761
-  _BATCHPREDICTREQUEST._serialized_end=24798
+  _GENONLINESTOREDATASETRESPONSE._serialized_start=23727
+  _GENONLINESTOREDATASETRESPONSE._serialized_end=23847
+  _BATCHPREDICTREQUEST._serialized_start=23850
+  _BATCHPREDICTREQUEST._serialized_end=24887
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_start=4342
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_end=4394
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_start=4396
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_end=4443
-  _BATCHPREDICTRESPONSE._serialized_start=24800
-  _BATCHPREDICTRESPONSE._serialized_end=24836
-  _SAVEDATASETREQUEST._serialized_start=24839
-  _SAVEDATASETREQUEST._serialized_end=25388
-  _SAVEMODELREQUEST._serialized_start=25391
-  _SAVEMODELREQUEST._serialized_end=26016
-  _SAVEPREDICTIONREQUEST._serialized_start=26019
-  _SAVEPREDICTIONREQUEST._serialized_end=26585
-  _SAVEPREDICTORREQUEST._serialized_start=26588
-  _SAVEPREDICTORREQUEST._serialized_end=26967
-  _CREATEMETRICSSTOREREQUEST._serialized_start=26970
-  _CREATEMETRICSSTOREREQUEST._serialized_end=27102
-  _CREATEMETRICSSTORERESPONSE._serialized_start=27104
-  _CREATEMETRICSSTORERESPONSE._serialized_end=27132
-  _SAVERESPONSE._serialized_start=27134
-  _SAVERESPONSE._serialized_end=27162
-  _DATASERVICE._serialized_start=27165
-  _DATASERVICE._serialized_end=35341
+  _BATCHPREDICTRESPONSE._serialized_start=24889
+  _BATCHPREDICTRESPONSE._serialized_end=24925
+  _SAVEDATASETREQUEST._serialized_start=24928
+  _SAVEDATASETREQUEST._serialized_end=25477
+  _SAVEMODELREQUEST._serialized_start=25480
+  _SAVEMODELREQUEST._serialized_end=26105
+  _SAVEPREDICTIONREQUEST._serialized_start=26108
+  _SAVEPREDICTIONREQUEST._serialized_end=26674
+  _SAVEPREDICTORREQUEST._serialized_start=26677
+  _SAVEPREDICTORREQUEST._serialized_end=27056
+  _CREATEMETRICSSTOREREQUEST._serialized_start=27059
+  _CREATEMETRICSSTOREREQUEST._serialized_end=27191
+  _CREATEMETRICSSTORERESPONSE._serialized_start=27193
+  _CREATEMETRICSSTORERESPONSE._serialized_end=27221
+  _SAVERESPONSE._serialized_start=27223
+  _SAVERESPONSE._serialized_end=27251
+  _DATASERVICE._serialized_start=27254
+  _DATASERVICE._serialized_end=35430
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -672,22 +672,24 @@
     def __init__(self) -> None: ...
 
 class DsShutdownResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class DsSnapshotRequest(_message.Message):
-    __slots__ = ["dataset", "datasource", "product"]
+    __slots__ = ["dataset", "datasource", "product", "snapshot"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    SNAPSHOT_FIELD_NUMBER: _ClassVar[int]
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     product: _generated_pb2.DataProduct
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ...) -> None: ...
+    snapshot: _generated_pb2.DatasetSnapshot
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., snapshot: _Optional[_Union[_generated_pb2.DatasetSnapshot, _Mapping]] = ...) -> None: ...
 
 class DsSnapshotResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class DsSplitDatasetRequest(_message.Message):
     __slots__ = ["bucket", "dataset", "datasource", "product", "snapshot", "study", "testingDataset", "trainingDataset"]
```

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.6.235/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/google/api/annotations_pb2.py` & `modelaapi-0.6.235/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/google/api/http_pb2.py` & `modelaapi-0.6.235/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/google/api/http_pb2.pyi` & `modelaapi-0.6.235/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.235/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/api/apps/v1/generated_pb2.pyi` & `modelaapi-0.6.235/k8s/io/api/apps/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.235/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/api/core/v1/generated_pb2.pyi` & `modelaapi-0.6.235/k8s/io/api/core/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.235/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/api/rbac/v1/generated_pb2.pyi` & `modelaapi-0.6.235/k8s/io/api/rbac/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.235/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi` & `modelaapi-0.6.235/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi` & `modelaapi-0.6.235/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi` & `modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.235/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.235/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi` & `modelaapi-0.6.235/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/modelaapi/consts.py` & `modelaapi-0.6.235/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/modelaapi/custom_transformers.py` & `modelaapi-0.6.235/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/modelaapi/graykite_model.py` & `modelaapi-0.6.235/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/modelaapi/ts.py` & `modelaapi-0.6.235/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/modelaapi/version.py` & `modelaapi-0.6.235/modelaapi/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 234,
+    "micro": 235,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.234/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.235/modelaapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.234
+Version: 0.6.235
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.234
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.235
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.234
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.235
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.234/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.235/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/setup.cfg` & `modelaapi-0.6.235/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.234/setup.py` & `modelaapi-0.6.235/setup.py`

 * *Files identical despite different names*

