# Comparing `tmp/mercuryclient-1.8.1.tar.gz` & `tmp/mercuryclient-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mercuryclient-1.8.1.tar", last modified: Wed Jan 11 08:54:04 2023, max compression
+gzip compressed data, was "dist/mercuryclient-1.9.0.tar", last modified: Thu Feb 23 06:03:52 2023, max compression
```

## Comparing `mercuryclient-1.8.1.tar` & `mercuryclient-1.9.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/
--rw-r--r--   0 root         (0) root         (0)     3789 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2631 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3992 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/api.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/http_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      871 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/bank_account_verify.py
--rw-rw-rw-   0 root         (0) root         (0)     2115 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/bank_statement.py
--rw-rw-rw-   0 root         (0) root         (0)    13887 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/bbps.py
--rw-rw-rw-   0 root         (0) root         (0)     4284 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/cibil.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/experian.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/gst_verificaion.py
--rw-rw-rw-   0 root         (0) root         (0)     4385 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/highmark.py
--rw-rw-rw-   0 root         (0) root         (0)     2816 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/id_verification.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/insurance.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/okyc_verification.py
--rw-rw-rw-   0 root         (0) root         (0)     5245 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/recharge.py
--rw-rw-rw-   0 root         (0) root         (0)     2888 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/sms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2977 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_bank_account_verify.py
--rw-rw-rw-   0 root         (0) root         (0)     5268 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_bank_statement.py
--rw-rw-rw-   0 root         (0) root         (0)    23724 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_bbps.py
--rw-rw-rw-   0 root         (0) root         (0)     6724 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_cibil.py
--rw-rw-rw-   0 root         (0) root         (0)     6815 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_experian.py
--rw-rw-rw-   0 root         (0) root         (0)     3471 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_gst_verification.py
--rw-rw-rw-   0 root         (0) root         (0)     7646 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_highmark.py
--rw-rw-rw-   0 root         (0) root         (0)     5706 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_id_verification.py
--rw-rw-rw-   0 root         (0) root         (0)     6883 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_insurance.py
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_okyc_verification.py
--rw-rw-rw-   0 root         (0) root         (0)     1960 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_recharge.py
--rw-rw-rw-   0 root         (0) root         (0)     4585 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_sms.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/tests/test_webhooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2206 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/mixins/webhooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/types/bank_account_verify/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/bank_account_verify/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/bank_account_verify/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/types/bbps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/bbps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/bbps/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     2228 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/bbps/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/types/cibil/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/cibil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5744 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/cibil/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     2293 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/cibil/request.py
--rw-rw-rw-   0 root         (0) root         (0)     1206 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/types/experian/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/experian/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/experian/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     3729 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/experian/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/types/highmark/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/highmark/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5672 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/highmark/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     3388 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/highmark/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/types/id_verification/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/id_verification/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/id_verification/enums.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/id_verification/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/types/insurance/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/insurance/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/insurance/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     2383 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/insurance/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient/types/okyc_verification/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/okyc_verification/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/okyc_verification/enums.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/mercuryclient/types/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3789 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2557 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       85 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/mercuryclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-11 08:54:04.000000 mercuryclient-1.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-01-11 08:53:49.000000 mercuryclient-1.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4042 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/api.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/http_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/bank_account_verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/bank_statement.py
+-rw-rw-rw-   0 root         (0) root         (0)    13887 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/bbps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4284 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/cibil.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/experian.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/gst_verificaion.py
+-rw-rw-rw-   0 root         (0) root         (0)     4385 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/highmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2816 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/id_verification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/insurance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/okyc_verification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/rc_verification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5245 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/recharge.py
+-rw-rw-rw-   0 root         (0) root         (0)     2888 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/sms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_bank_account_verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     5268 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_bank_statement.py
+-rw-rw-rw-   0 root         (0) root         (0)    23724 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_bbps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6724 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_cibil.py
+-rw-rw-rw-   0 root         (0) root         (0)     6815 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_experian.py
+-rw-rw-rw-   0 root         (0) root         (0)     3471 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_gst_verification.py
+-rw-rw-rw-   0 root         (0) root         (0)     7646 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_highmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     5706 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_id_verification.py
+-rw-rw-rw-   0 root         (0) root         (0)     6883 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_insurance.py
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_okyc_verification.py
+-rw-rw-rw-   0 root         (0) root         (0)     3561 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_rc_vrification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_recharge.py
+-rw-rw-rw-   0 root         (0) root         (0)     4585 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_sms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/tests/test_webhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2206 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/mixins/webhooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/types/bank_account_verify/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/bank_account_verify/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/bank_account_verify/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/types/bbps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/bbps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/bbps/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/bbps/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/types/cibil/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/cibil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5744 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/cibil/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/cibil/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/types/experian/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/experian/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/experian/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     3729 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/experian/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/types/highmark/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/highmark/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5672 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/highmark/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/highmark/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/types/id_verification/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/id_verification/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/id_verification/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/id_verification/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/types/insurance/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/insurance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/insurance/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2383 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/insurance/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient/types/okyc_verification/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/okyc_verification/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/okyc_verification/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/mercuryclient/types/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       85 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/mercuryclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 06:03:52.000000 mercuryclient-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-02-23 06:03:36.000000 mercuryclient-1.9.0/setup.py
```

### Comparing `mercuryclient-1.8.1/PKG-INFO` & `mercuryclient-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercuryclient
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python SDK for Mercury service
 Home-page: https://bitbucket.org/esthenos/mercury
 Author: Esthenos Technologies Private Limited
 Author-email: dinu@esthenos.com
 License: Proprietary License
 Description: ===========
         Mercury SDK
@@ -65,14 +65,15 @@
            - get_complaint_status
            - get_bbpsid
         - verify_bank_account
         - verify_gstin
         - get_verify_gst_result
         - generate_okyc_otp
         - verify_okyc_otp
+        - fetch_rc_details
         
         Types:
         ------
         For complex requests like CIBIL, Experian or Highmark, you can construct the request
         JSON using the provided pydantic models. The types are available at *mercury.types.<request_type>.request*.
         
         Example using models for generating Highmark Request::
```

### Comparing `mercuryclient-1.8.1/README.rst` & `mercuryclient-1.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
    - get_complaint_status
    - get_bbpsid
 - verify_bank_account
 - verify_gstin
 - get_verify_gst_result
 - generate_okyc_otp
 - verify_okyc_otp
+- fetch_rc_details
 
 Types:
 ------
 For complex requests like CIBIL, Experian or Highmark, you can construct the request
 JSON using the provided pydantic models. The types are available at *mercury.types.<request_type>.request*.
 
 Example using models for generating Highmark Request::
```

### Comparing `mercuryclient-1.8.1/mercuryclient/api.py` & `mercuryclient-1.9.0/mercuryclient/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     WebhookMixin,
     InsuranceMixin,
     RechargeMixin,
     BbpsMixin,
     AccountVerifyMixin,
     GstVerifyMixin,
     OkycVerificationMixin,
+    RcVerificationMixin,
 )
 
 
 class MercuryApi(
     AuthMixin,
     BankStatementMixin,
     CibilMixin,
@@ -33,14 +34,15 @@
     WebhookMixin,
     InsuranceMixin,
     RechargeMixin,
     BbpsMixin,
     AccountVerifyMixin,
     GstVerifyMixin,
     OkycVerificationMixin,
+    RcVerificationMixin,
 ):
     """
     Mercury client to connect to the mercury service
 
     """
 
     def __init__(self, conn_params=None):
```

### Comparing `mercuryclient-1.8.1/mercuryclient/http_utils.py` & `mercuryclient-1.9.0/mercuryclient/http_utils.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/__init__.py` & `mercuryclient-1.9.0/mercuryclient/mixins/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .id_verification import IDVerificationMixin
 from .mail import MailMixin
 from .recharge import RechargeMixin
 from .sms import SMSMixin
 from .webhooks import WebhookMixin
 from .insurance import InsuranceMixin
 from .okyc_verification import OkycVerificationMixin
+from .rc_verification import RcVerificationMixin
 
 __all__ = [
     AuthMixin,
     BankStatementMixin,
     CibilMixin,
     ExperianMixin,
     HighmarkMixin,
@@ -26,8 +27,9 @@
     WebhookMixin,
     InsuranceMixin,
     RechargeMixin,
     BbpsMixin,
     AccountVerifyMixin,
     GstVerifyMixin,
     OkycVerificationMixin,
+    RcVerificationMixin,
 ]
```

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/auth.py` & `mercuryclient-1.9.0/mercuryclient/mixins/auth.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/bank_account_verify.py` & `mercuryclient-1.9.0/mercuryclient/mixins/bank_account_verify.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/bank_statement.py` & `mercuryclient-1.9.0/mercuryclient/mixins/bank_statement.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/bbps.py` & `mercuryclient-1.9.0/mercuryclient/mixins/bbps.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/cibil.py` & `mercuryclient-1.9.0/mercuryclient/mixins/cibil.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/experian.py` & `mercuryclient-1.9.0/mercuryclient/mixins/experian.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/gst_verificaion.py` & `mercuryclient-1.9.0/mercuryclient/mixins/gst_verificaion.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/highmark.py` & `mercuryclient-1.9.0/mercuryclient/mixins/highmark.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/id_verification.py` & `mercuryclient-1.9.0/mercuryclient/mixins/id_verification.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/insurance.py` & `mercuryclient-1.9.0/mercuryclient/mixins/insurance.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/mail.py` & `mercuryclient-1.9.0/mercuryclient/mixins/mail.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/okyc_verification.py` & `mercuryclient-1.9.0/mercuryclient/mixins/okyc_verification.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/recharge.py` & `mercuryclient-1.9.0/mercuryclient/mixins/recharge.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/sms.py` & `mercuryclient-1.9.0/mercuryclient/mixins/sms.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_auth.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_bank_account_verify.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_bank_account_verify.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_bank_statement.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_bank_statement.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_bbps.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_bbps.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_cibil.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_cibil.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_experian.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_experian.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_gst_verification.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_gst_verification.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_highmark.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_highmark.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_id_verification.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_id_verification.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_insurance.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_insurance.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_okyc_verification.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_okyc_verification.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_recharge.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_recharge.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_sms.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_sms.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/tests/test_webhooks.py` & `mercuryclient-1.9.0/mercuryclient/mixins/tests/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/mixins/webhooks.py` & `mercuryclient-1.9.0/mercuryclient/mixins/webhooks.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/types/bbps/request.py` & `mercuryclient-1.9.0/mercuryclient/types/bbps/request.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/types/cibil/enums.py` & `mercuryclient-1.9.0/mercuryclient/types/cibil/enums.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/types/cibil/request.py` & `mercuryclient-1.9.0/mercuryclient/types/cibil/request.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/types/common.py` & `mercuryclient-1.9.0/mercuryclient/types/common.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/types/experian/enums.py` & `mercuryclient-1.9.0/mercuryclient/types/experian/enums.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/types/experian/request.py` & `mercuryclient-1.9.0/mercuryclient/types/experian/request.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/types/highmark/enums.py` & `mercuryclient-1.9.0/mercuryclient/types/highmark/enums.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/types/highmark/request.py` & `mercuryclient-1.9.0/mercuryclient/types/highmark/request.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient/types/insurance/request.py` & `mercuryclient-1.9.0/mercuryclient/types/insurance/request.py`

 * *Files identical despite different names*

### Comparing `mercuryclient-1.8.1/mercuryclient.egg-info/PKG-INFO` & `mercuryclient-1.9.0/mercuryclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercuryclient
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python SDK for Mercury service
 Home-page: https://bitbucket.org/esthenos/mercury
 Author: Esthenos Technologies Private Limited
 Author-email: dinu@esthenos.com
 License: Proprietary License
 Description: ===========
         Mercury SDK
@@ -65,14 +65,15 @@
            - get_complaint_status
            - get_bbpsid
         - verify_bank_account
         - verify_gstin
         - get_verify_gst_result
         - generate_okyc_otp
         - verify_okyc_otp
+        - fetch_rc_details
         
         Types:
         ------
         For complex requests like CIBIL, Experian or Highmark, you can construct the request
         JSON using the provided pydantic models. The types are available at *mercury.types.<request_type>.request*.
         
         Example using models for generating Highmark Request::
```

### Comparing `mercuryclient-1.8.1/mercuryclient.egg-info/SOURCES.txt` & `mercuryclient-1.9.0/mercuryclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 mercuryclient/mixins/experian.py
 mercuryclient/mixins/gst_verificaion.py
 mercuryclient/mixins/highmark.py
 mercuryclient/mixins/id_verification.py
 mercuryclient/mixins/insurance.py
 mercuryclient/mixins/mail.py
 mercuryclient/mixins/okyc_verification.py
+mercuryclient/mixins/rc_verification.py
 mercuryclient/mixins/recharge.py
 mercuryclient/mixins/sms.py
 mercuryclient/mixins/webhooks.py
 mercuryclient/mixins/tests/__init__.py
 mercuryclient/mixins/tests/test_auth.py
 mercuryclient/mixins/tests/test_bank_account_verify.py
 mercuryclient/mixins/tests/test_bank_statement.py
@@ -33,14 +34,15 @@
 mercuryclient/mixins/tests/test_cibil.py
 mercuryclient/mixins/tests/test_experian.py
 mercuryclient/mixins/tests/test_gst_verification.py
 mercuryclient/mixins/tests/test_highmark.py
 mercuryclient/mixins/tests/test_id_verification.py
 mercuryclient/mixins/tests/test_insurance.py
 mercuryclient/mixins/tests/test_okyc_verification.py
+mercuryclient/mixins/tests/test_rc_vrification.py
 mercuryclient/mixins/tests/test_recharge.py
 mercuryclient/mixins/tests/test_sms.py
 mercuryclient/mixins/tests/test_webhooks.py
 mercuryclient/types/__init__.py
 mercuryclient/types/common.py
 mercuryclient/types/validators.py
 mercuryclient/types/bank_account_verify/__init__.py
```

### Comparing `mercuryclient-1.8.1/setup.py` & `mercuryclient-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 requirements = ["requests >=2.25.0,<3", "PyJWT >=1.7.0,<2", "pydantic >=1.7.0,<2"]
 dev_requirements = ["pre-commit", "wheel", "twine"]
 
 setup(
     name="mercuryclient",
-    version="1.8.1",
+    version="1.9.0",
     description="Python SDK for Mercury service",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://bitbucket.org/esthenos/mercury",
     author="Esthenos Technologies Private Limited",
     author_email="dinu@esthenos.com",
     license="Proprietary License",
```

