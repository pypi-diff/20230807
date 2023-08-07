# Comparing `tmp/onqlave-python-0.1.1.tar.gz` & `tmp/onqlave-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onqlave-python-0.1.1.tar", last modified: Fri Aug  4 07:16:17 2023, max compression
+gzip compressed data, was "onqlave-python-0.1.2.tar", last modified: Mon Aug  7 02:28:49 2023, max compression
```

## Comparing `onqlave-python-0.1.1.tar` & `onqlave-python-0.1.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.284382 onqlave-python-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-08-04 07:16:17.284382 onqlave-python-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.272381 onqlave-python-0.1.1/onqlave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.272381 onqlave-python-0.1.1/onqlave/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/connection/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.276381 onqlave-python-0.1.1/onqlave/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.276381 onqlave-python-0.1.1/onqlave/contracts/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/contracts/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/contracts/requests/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.276381 onqlave-python-0.1.1/onqlave/contracts/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/contracts/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/contracts/responses/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.276381 onqlave-python-0.1.1/onqlave/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/credentials/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.276381 onqlave-python-0.1.1/onqlave/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/encryption/encrypted_stream_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/encryption/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/encryption/plain_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.276381 onqlave-python-0.1.1/onqlave/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/errors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.276381 onqlave-python-0.1.1/onqlave/keymanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.276381 onqlave-python-0.1.1/onqlave/keymanager/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/factories/aes_gcm_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/factories/xchacha20_poly1305_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/id_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/key_manager_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.276381 onqlave-python-0.1.1/onqlave/keymanager/keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/keys/aes_gcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/keys/xchacha_20_poly_1350.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.280382 onqlave-python-0.1.1/onqlave/keymanager/onqlave_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/onqlave_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/onqlave_types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.280382 onqlave-python-0.1.1/onqlave/keymanager/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/operations/aes_128_gcm_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/operations/aes_256_gcm_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.280382 onqlave-python-0.1.1/onqlave/keymanager/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/primitives/aes_gcm_aead.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/keymanager/random_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.280382 onqlave-python-0.1.1/onqlave/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.280382 onqlave-python-0.1.1/onqlave/messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/messages/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.280382 onqlave-python-0.1.1/onqlave/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-04 07:15:59.000000 onqlave-python-0.1.1/onqlave/utils/hasher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:16:17.280382 onqlave-python-0.1.1/onqlave_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-08-04 07:16:17.000000 onqlave-python-0.1.1/onqlave_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-04 07:16:17.000000 onqlave-python-0.1.1/onqlave_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 07:16:17.000000 onqlave-python-0.1.1/onqlave_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-04 07:16:17.000000 onqlave-python-0.1.1/onqlave_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 07:16:17.000000 onqlave-python-0.1.1/onqlave_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 07:16:17.284382 onqlave-python-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-04 07:16:16.000000 onqlave-python-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.316144 onqlave-python-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-08-07 02:28:49.316144 onqlave-python-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.308144 onqlave-python-0.1.2/onqlave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.308144 onqlave-python-0.1.2/onqlave/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/connection/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.308144 onqlave-python-0.1.2/onqlave/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.308144 onqlave-python-0.1.2/onqlave/contracts/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/contracts/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/contracts/requests/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.308144 onqlave-python-0.1.2/onqlave/contracts/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/contracts/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/contracts/responses/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.308144 onqlave-python-0.1.2/onqlave/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/credentials/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.308144 onqlave-python-0.1.2/onqlave/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/encryption/encrypted_stream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/encryption/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/encryption/plain_stream_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.308144 onqlave-python-0.1.2/onqlave/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/errors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.308144 onqlave-python-0.1.2/onqlave/keymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.312144 onqlave-python-0.1.2/onqlave/keymanager/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/factories/aes_gcm_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/factories/xchacha20_poly1305_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/id_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/key_manager_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.312144 onqlave-python-0.1.2/onqlave/keymanager/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/keys/aes_gcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/keys/xchacha_20_poly_1350.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.312144 onqlave-python-0.1.2/onqlave/keymanager/onqlave_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/onqlave_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/onqlave_types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.312144 onqlave-python-0.1.2/onqlave/keymanager/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/operations/aes_128_gcm_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/operations/aes_256_gcm_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/operations/xchacha20_poly1305_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.312144 onqlave-python-0.1.2/onqlave/keymanager/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/primitives/aes_gcm_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/keymanager/random_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.312144 onqlave-python-0.1.2/onqlave/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.312144 onqlave-python-0.1.2/onqlave/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/messages/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.312144 onqlave-python-0.1.2/onqlave/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-07 02:28:31.000000 onqlave-python-0.1.2/onqlave/utils/hasher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:28:49.316144 onqlave-python-0.1.2/onqlave_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-08-07 02:28:49.000000 onqlave-python-0.1.2/onqlave_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-07 02:28:49.000000 onqlave-python-0.1.2/onqlave_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 02:28:49.000000 onqlave-python-0.1.2/onqlave_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-07 02:28:49.000000 onqlave-python-0.1.2/onqlave_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 02:28:49.000000 onqlave-python-0.1.2/onqlave_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 02:28:49.316144 onqlave-python-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-07 02:28:48.000000 onqlave-python-0.1.2/setup.py
```

### Comparing `onqlave-python-0.1.1/LICENSE` & `onqlave-python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/PKG-INFO` & `onqlave-python-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: This Python SDK is designed to help developers easily integrate Onqlave Encryption As A Service into their python backend.
 Home-page: https://github.com/onqlavelabs/onqlave-python/
 Download-URL: https://pypi.org/project/onqlave-python/#history
 Author: Onqlave Pty
 Author-email: product@onqlave.com
 Maintainer: DC
 Maintainer-email: dc@onqlave.com
@@ -27,16 +27,15 @@
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This Python SDK is designed to help developers easily integrate Onqlave `Encryption As A Service` into their python backend.
 
 [![CI](https://img.shields.io/static/v1?label=CI&message=passing&color=green?style=plastic&logo=github)](https://github.com/onqlavelabs/onqlave-python/actions)
-[![GitHub release](https://img.shields.io/github/v/release/onqlavelabs/onqlave-go.svg)](https://github.com/onqlavelabs/onqlave-python/releases)
-[![License](https://img.shields.io/github/license/onqlavelabs/onqlave-python)](https://github.com/onqlavelabs/onqlave-python/blob/main/LICENSE)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 # Table of Contents
 
 - [Description](#description)
 - [Table of Contents](#table-of-contents)
 	- [Features](#features)
```

### Comparing `onqlave-python-0.1.1/README.md` & `onqlave-python-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 This Python SDK is designed to help developers easily integrate Onqlave `Encryption As A Service` into their python backend.
 
 [![CI](https://img.shields.io/static/v1?label=CI&message=passing&color=green?style=plastic&logo=github)](https://github.com/onqlavelabs/onqlave-python/actions)
-[![GitHub release](https://img.shields.io/github/v/release/onqlavelabs/onqlave-go.svg)](https://github.com/onqlavelabs/onqlave-python/releases)
-[![License](https://img.shields.io/github/license/onqlavelabs/onqlave-python)](https://github.com/onqlavelabs/onqlave-python/blob/main/LICENSE)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 # Table of Contents
 
 - [Description](#description)
 - [Table of Contents](#table-of-contents)
 	- [Features](#features)
```

### Comparing `onqlave-python-0.1.1/onqlave/connection/client.py` & `onqlave-python-0.1.2/onqlave/connection/client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/connection/connection.py` & `onqlave-python-0.1.2/onqlave/connection/connection.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/contracts/requests/requests.py` & `onqlave-python-0.1.2/onqlave/contracts/requests/requests.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/contracts/responses/responses.py` & `onqlave-python-0.1.2/onqlave/contracts/responses/responses.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/credentials/credentials.py` & `onqlave-python-0.1.2/onqlave/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/encryption/encrypted_stream_processor.py` & `onqlave-python-0.1.2/onqlave/encryption/encrypted_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/encryption/encryption.py` & `onqlave-python-0.1.2/onqlave/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/encryption/options.py` & `onqlave-python-0.1.2/onqlave/encryption/options.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/encryption/plain_stream_processor.py` & `onqlave-python-0.1.2/onqlave/encryption/plain_stream_processor.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/errors/errors.py` & `onqlave-python-0.1.2/onqlave/errors/errors.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/factories/aes_gcm_factory.py` & `onqlave-python-0.1.2/onqlave/keymanager/factories/aes_gcm_factory.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py` & `onqlave-python-0.1.2/onqlave/keymanager/factories/rsa_ssa_pkcs1_sha_factory.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/factories/xchacha20_poly1305_factory.py` & `onqlave-python-0.1.2/onqlave/keymanager/factories/xchacha20_poly1305_factory.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/id_service.py` & `onqlave-python-0.1.2/onqlave/keymanager/id_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/key_manager_client.py` & `onqlave-python-0.1.2/onqlave/keymanager/key_manager_client.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/keys/aes_gcm.py` & `onqlave-python-0.1.2/onqlave/keymanager/keys/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/keys/xchacha_20_poly_1350.py` & `onqlave-python-0.1.2/onqlave/keymanager/keys/xchacha_20_poly_1350.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/onqlave_types/types.py` & `onqlave-python-0.1.2/onqlave/keymanager/onqlave_types/types.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/operations/aes_128_gcm_operation.py` & `onqlave-python-0.1.2/onqlave/keymanager/operations/aes_128_gcm_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/operations/aes_256_gcm_operation.py` & `onqlave-python-0.1.2/onqlave/keymanager/operations/aes_256_gcm_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py` & `onqlave-python-0.1.2/onqlave/keymanager/operations/rsa_ssa_pkcs1_sha_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/operations/xchacha20_poly1305_operation.py` & `onqlave-python-0.1.2/onqlave/keymanager/operations/xchacha20_poly1305_operation.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/primitives/aes_gcm_aead.py` & `onqlave-python-0.1.2/onqlave/keymanager/primitives/aes_gcm_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py` & `onqlave-python-0.1.2/onqlave/keymanager/primitives/rsa_ssa_pkcs1_sha.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py` & `onqlave-python-0.1.2/onqlave/keymanager/primitives/xchacha20_poly1305_aead.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/keymanager/random_service.py` & `onqlave-python-0.1.2/onqlave/keymanager/random_service.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/messages/messages.py` & `onqlave-python-0.1.2/onqlave/messages/messages.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave/utils/hasher.py` & `onqlave-python-0.1.2/onqlave/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave_python.egg-info/PKG-INFO` & `onqlave-python-0.1.2/onqlave_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onqlave-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: This Python SDK is designed to help developers easily integrate Onqlave Encryption As A Service into their python backend.
 Home-page: https://github.com/onqlavelabs/onqlave-python/
 Download-URL: https://pypi.org/project/onqlave-python/#history
 Author: Onqlave Pty
 Author-email: product@onqlave.com
 Maintainer: DC
 Maintainer-email: dc@onqlave.com
@@ -27,16 +27,15 @@
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This Python SDK is designed to help developers easily integrate Onqlave `Encryption As A Service` into their python backend.
 
 [![CI](https://img.shields.io/static/v1?label=CI&message=passing&color=green?style=plastic&logo=github)](https://github.com/onqlavelabs/onqlave-python/actions)
-[![GitHub release](https://img.shields.io/github/v/release/onqlavelabs/onqlave-go.svg)](https://github.com/onqlavelabs/onqlave-python/releases)
-[![License](https://img.shields.io/github/license/onqlavelabs/onqlave-python)](https://github.com/onqlavelabs/onqlave-python/blob/main/LICENSE)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 # Table of Contents
 
 - [Description](#description)
 - [Table of Contents](#table-of-contents)
 	- [Features](#features)
```

### Comparing `onqlave-python-0.1.1/onqlave_python.egg-info/SOURCES.txt` & `onqlave-python-0.1.2/onqlave_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/onqlave_python.egg-info/requires.txt` & `onqlave-python-0.1.2/onqlave_python.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `onqlave-python-0.1.1/setup.py` & `onqlave-python-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 package_name = 'onqlave-python'
 download_url = format('https://pypi.org/project/%s/#history' % package_name)
 
 setup(
     name=package_name,
-    version='0.1.1',
+    version='0.1.2',
     author='Onqlave Pty',
     author_email='product@onqlave.com',
     maintainer='DC',
     maintainer_email='dc@onqlave.com',
     description='This Python SDK is designed to help developers easily integrate Onqlave Encryption As A Service into their python backend.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

