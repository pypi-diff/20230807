# Comparing `tmp/safe2pay-0.0.5.tar.gz` & `tmp/safe2pay-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe2pay-0.0.5.tar", last modified: Fri Aug  4 01:12:22 2023, max compression
+gzip compressed data, was "safe2pay-0.0.6.tar", last modified: Mon Aug  7 01:40:10 2023, max compression
```

## Comparing `safe2pay-0.0.5.tar` & `safe2pay-0.0.6.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-04 01:12:22.315184 safe2pay-0.0.5/
--rw-r--r--   0 elainecro   (501) staff       (20)     1070 2023-07-25 01:59:11.000000 safe2pay-0.0.5/LICENSE
--rw-r--r--   0 elainecro   (501) staff       (20)      120 2023-07-04 17:18:28.000000 safe2pay-0.0.5/MANIFEST.in
--rw-r--r--   0 elainecro   (501) staff       (20)    25597 2023-08-04 01:12:22.315355 safe2pay-0.0.5/PKG-INFO
--rw-r--r--   0 elainecro   (501) staff       (20)    24684 2023-07-25 02:38:58.000000 safe2pay-0.0.5/README.md
--rw-r--r--   0 elainecro   (501) staff       (20)      113 2023-08-02 03:12:44.000000 safe2pay-0.0.5/requirements.txt
-drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-04 01:12:22.296248 safe2pay-0.0.5/safe2pay/
--rw-r--r--   0 elainecro   (501) staff       (20)       89 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/__init__.py
-drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-04 01:12:22.313698 safe2pay-0.0.5/safe2pay/entities/
--rw-r--r--   0 elainecro   (501) staff       (20)     2043 2023-07-19 04:42:10.000000 safe2pay-0.0.5/safe2pay/entities/__init__.py
--rw-r--r--   0 elainecro   (501) staff       (20)      465 2023-07-14 14:33:03.000000 safe2pay-0.0.5/safe2pay/entities/accountresponse.py
--rw-r--r--   0 elainecro   (501) staff       (20)      275 2023-07-15 03:21:20.000000 safe2pay-0.0.5/safe2pay/entities/accounttype.py
--rw-r--r--   0 elainecro   (501) staff       (20)      563 2023-07-19 02:50:03.000000 safe2pay-0.0.5/safe2pay/entities/address.py
--rw-r--r--   0 elainecro   (501) staff       (20)     1231 2023-07-15 02:48:28.000000 safe2pay-0.0.5/safe2pay/entities/anticipation.py
--rw-r--r--   0 elainecro   (501) staff       (20)      267 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/bank.py
--rw-r--r--   0 elainecro   (501) staff       (20)      658 2023-07-15 02:21:38.000000 safe2pay-0.0.5/safe2pay/entities/bankdata.py
--rw-r--r--   0 elainecro   (501) staff       (20)     1193 2023-07-14 14:17:51.000000 safe2pay-0.0.5/safe2pay/entities/bankslip.py
--rw-r--r--   0 elainecro   (501) staff       (20)      322 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/bankslip_response.py
--rw-r--r--   0 elainecro   (501) staff       (20)      652 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/boleto.py
--rw-r--r--   0 elainecro   (501) staff       (20)      928 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/carnet.py
--rw-r--r--   0 elainecro   (501) staff       (20)     1190 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/carnetasync.py
--rw-r--r--   0 elainecro   (501) staff       (20)     1253 2023-07-19 04:44:43.000000 safe2pay-0.0.5/safe2pay/entities/chargeback.py
--rw-r--r--   0 elainecro   (501) staff       (20)     1640 2023-07-15 02:30:06.000000 safe2pay-0.0.5/safe2pay/entities/checkingaccount.py
--rw-r--r--   0 elainecro   (501) staff       (20)      244 2023-07-19 02:45:45.000000 safe2pay-0.0.5/safe2pay/entities/city.py
--rw-r--r--   0 elainecro   (501) staff       (20)     1282 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/creditcard.py
--rw-r--r--   0 elainecro   (501) staff       (20)      403 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/customer.py
--rw-r--r--   0 elainecro   (501) staff       (20)      746 2023-07-15 02:00:55.000000 safe2pay-0.0.5/safe2pay/entities/deposit.py
--rw-r--r--   0 elainecro   (501) staff       (20)      245 2023-07-15 02:47:48.000000 safe2pay-0.0.5/safe2pay/entities/effectiveness.py
--rw-r--r--   0 elainecro   (501) staff       (20)      243 2023-07-15 01:51:52.000000 safe2pay-0.0.5/safe2pay/entities/extract.py
--rw-r--r--   0 elainecro   (501) staff       (20)      427 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/installments.py
--rw-r--r--   0 elainecro   (501) staff       (20)      673 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/installmentvalue.py
--rw-r--r--   0 elainecro   (501) staff       (20)      361 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/integration.py
-drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-04 01:12:22.314355 safe2pay-0.0.5/safe2pay/entities/lib/
--rw-r--r--   0 elainecro   (501) staff       (20)       69 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/lib/__init__.py
--rw-r--r--   0 elainecro   (501) staff       (20)     7831 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/lib/datatype.py
--rw-r--r--   0 elainecro   (501) staff       (20)     9687 2023-07-19 04:52:48.000000 safe2pay-0.0.5/safe2pay/entities/lib/entity.py
--rw-r--r--   0 elainecro   (501) staff       (20)     2479 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/marketplace.py
--rw-r--r--   0 elainecro   (501) staff       (20)      487 2023-07-15 02:10:52.000000 safe2pay-0.0.5/safe2pay/entities/marketplacelistresponse.py
--rw-r--r--   0 elainecro   (501) staff       (20)      249 2023-07-15 02:06:48.000000 safe2pay-0.0.5/safe2pay/entities/marketplaceobjects.py
--rw-r--r--   0 elainecro   (501) staff       (20)      430 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/merchantaccount.py
--rw-r--r--   0 elainecro   (501) staff       (20)      774 2023-07-15 02:22:55.000000 safe2pay-0.0.5/safe2pay/entities/merchantbankdata.py
--rw-r--r--   0 elainecro   (501) staff       (20)      600 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/merchantpayment.py
--rw-r--r--   0 elainecro   (501) staff       (20)      410 2023-07-19 03:25:58.000000 safe2pay-0.0.5/safe2pay/entities/merchantpayment_response.py
--rw-r--r--   0 elainecro   (501) staff       (20)      360 2023-07-14 13:33:59.000000 safe2pay-0.0.5/safe2pay/entities/merchantsplit.py
--rw-r--r--   0 elainecro   (501) staff       (20)      275 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/merchanttype.py
--rw-r--r--   0 elainecro   (501) staff       (20)     3207 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/payment.py
--rw-r--r--   0 elainecro   (501) staff       (20)     1266 2023-07-19 04:52:40.000000 safe2pay-0.0.5/safe2pay/entities/paymentmethod.py
--rw-r--r--   0 elainecro   (501) staff       (20)     2339 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/paymentobject.py
--rw-r--r--   0 elainecro   (501) staff       (20)      506 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/paymentoption.py
--rw-r--r--   0 elainecro   (501) staff       (20)      585 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/pix.py
--rw-r--r--   0 elainecro   (501) staff       (20)     3169 2023-08-04 01:11:53.000000 safe2pay-0.0.5/safe2pay/entities/plan.py
--rw-r--r--   0 elainecro   (501) staff       (20)      460 2023-07-19 04:02:02.000000 safe2pay-0.0.5/safe2pay/entities/plandataresponse.py
--rw-r--r--   0 elainecro   (501) staff       (20)      313 2023-07-19 03:49:14.000000 safe2pay-0.0.5/safe2pay/entities/planresponse.py
--rw-r--r--   0 elainecro   (501) staff       (20)     3100 2023-07-19 04:36:17.000000 safe2pay-0.0.5/safe2pay/entities/plansubscription.py
--rw-r--r--   0 elainecro   (501) staff       (20)      363 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/product.py
--rw-r--r--   0 elainecro   (501) staff       (20)     4649 2023-07-19 03:26:28.000000 safe2pay-0.0.5/safe2pay/entities/responsedetail.py
--rw-r--r--   0 elainecro   (501) staff       (20)      319 2023-07-14 14:35:40.000000 safe2pay-0.0.5/safe2pay/entities/responsedetail_account.py
--rw-r--r--   0 elainecro   (501) staff       (20)     3581 2023-07-14 14:11:12.000000 safe2pay-0.0.5/safe2pay/entities/singlesale.py
--rw-r--r--   0 elainecro   (501) staff       (20)      427 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/split.py
--rw-r--r--   0 elainecro   (501) staff       (20)      728 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/staticpix.py
--rw-r--r--   0 elainecro   (501) staff       (20)      305 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/tax.py
--rw-r--r--   0 elainecro   (501) staff       (20)     1117 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/token.py
--rw-r--r--   0 elainecro   (501) staff       (20)     4724 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/entities/transaction.py
--rw-r--r--   0 elainecro   (501) staff       (20)      457 2023-07-14 13:55:29.000000 safe2pay-0.0.5/safe2pay/entities/transaction_response.py
--rw-r--r--   0 elainecro   (501) staff       (20)      419 2023-07-14 13:58:44.000000 safe2pay-0.0.5/safe2pay/entities/transactionlistresponse.py
--rw-r--r--   0 elainecro   (501) staff       (20)      783 2023-07-15 03:27:53.000000 safe2pay-0.0.5/safe2pay/entities/transfer.py
--rw-r--r--   0 elainecro   (501) staff       (20)     2469 2023-07-16 17:06:58.000000 safe2pay-0.0.5/safe2pay/entities/transferregister.py
-drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-04 01:12:22.315026 safe2pay-0.0.5/safe2pay/utils/
--rw-r--r--   0 elainecro   (501) staff       (20)       23 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/utils/__init__.py
--rw-r--r--   0 elainecro   (501) staff       (20)      240 2023-07-13 03:09:51.000000 safe2pay-0.0.5/safe2pay/utils/constants.py
--rw-r--r--   0 elainecro   (501) staff       (20)     4807 2023-08-04 01:02:20.000000 safe2pay-0.0.5/safe2pay/utils/safe2pay.py
-drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-04 01:12:22.297393 safe2pay-0.0.5/safe2pay.egg-info/
--rw-r--r--   0 elainecro   (501) staff       (20)    25597 2023-08-04 01:12:22.000000 safe2pay-0.0.5/safe2pay.egg-info/PKG-INFO
--rw-r--r--   0 elainecro   (501) staff       (20)     2238 2023-08-04 01:12:22.000000 safe2pay-0.0.5/safe2pay.egg-info/SOURCES.txt
--rw-r--r--   0 elainecro   (501) staff       (20)        1 2023-08-04 01:12:22.000000 safe2pay-0.0.5/safe2pay.egg-info/dependency_links.txt
--rw-r--r--   0 elainecro   (501) staff       (20)      114 2023-08-04 01:12:22.000000 safe2pay-0.0.5/safe2pay.egg-info/requires.txt
--rw-r--r--   0 elainecro   (501) staff       (20)        9 2023-08-04 01:12:22.000000 safe2pay-0.0.5/safe2pay.egg-info/top_level.txt
--rw-r--r--   0 elainecro   (501) staff       (20)      102 2023-08-04 01:12:22.315699 safe2pay-0.0.5/setup.cfg
--rw-r--r--   0 elainecro   (501) staff       (20)     1227 2023-08-04 01:11:59.000000 safe2pay-0.0.5/setup.py
+drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-07 01:40:10.784607 safe2pay-0.0.6/
+-rw-r--r--   0 elainecro   (501) staff       (20)     1070 2023-07-25 01:59:11.000000 safe2pay-0.0.6/LICENSE
+-rw-r--r--   0 elainecro   (501) staff       (20)      120 2023-07-04 17:18:28.000000 safe2pay-0.0.6/MANIFEST.in
+-rw-r--r--   0 elainecro   (501) staff       (20)    25597 2023-08-07 01:40:10.784738 safe2pay-0.0.6/PKG-INFO
+-rw-r--r--   0 elainecro   (501) staff       (20)    24684 2023-07-25 02:38:58.000000 safe2pay-0.0.6/README.md
+-rw-r--r--   0 elainecro   (501) staff       (20)      113 2023-08-02 03:12:44.000000 safe2pay-0.0.6/requirements.txt
+drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-07 01:40:10.750098 safe2pay-0.0.6/safe2pay/
+-rw-r--r--   0 elainecro   (501) staff       (20)       89 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/__init__.py
+drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-07 01:40:10.768986 safe2pay-0.0.6/safe2pay/entities/
+-rw-r--r--   0 elainecro   (501) staff       (20)     2043 2023-07-19 04:42:10.000000 safe2pay-0.0.6/safe2pay/entities/__init__.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      465 2023-07-14 14:33:03.000000 safe2pay-0.0.6/safe2pay/entities/accountresponse.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      275 2023-07-15 03:21:20.000000 safe2pay-0.0.6/safe2pay/entities/accounttype.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      563 2023-07-19 02:50:03.000000 safe2pay-0.0.6/safe2pay/entities/address.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     1231 2023-07-15 02:48:28.000000 safe2pay-0.0.6/safe2pay/entities/anticipation.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      267 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/bank.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      658 2023-07-15 02:21:38.000000 safe2pay-0.0.6/safe2pay/entities/bankdata.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     1193 2023-07-14 14:17:51.000000 safe2pay-0.0.6/safe2pay/entities/bankslip.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      322 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/bankslip_response.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      652 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/boleto.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      928 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/carnet.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     1190 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/carnetasync.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     1253 2023-07-19 04:44:43.000000 safe2pay-0.0.6/safe2pay/entities/chargeback.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     1640 2023-07-15 02:30:06.000000 safe2pay-0.0.6/safe2pay/entities/checkingaccount.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      244 2023-07-19 02:45:45.000000 safe2pay-0.0.6/safe2pay/entities/city.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     1282 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/creditcard.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      403 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/customer.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      746 2023-07-15 02:00:55.000000 safe2pay-0.0.6/safe2pay/entities/deposit.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      245 2023-07-15 02:47:48.000000 safe2pay-0.0.6/safe2pay/entities/effectiveness.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      260 2023-08-07 01:35:14.000000 safe2pay-0.0.6/safe2pay/entities/erroresponse.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      243 2023-07-15 01:51:52.000000 safe2pay-0.0.6/safe2pay/entities/extract.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      427 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/installments.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      673 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/installmentvalue.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      361 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/integration.py
+drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-07 01:40:10.783050 safe2pay-0.0.6/safe2pay/entities/lib/
+-rw-r--r--   0 elainecro   (501) staff       (20)       69 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/lib/__init__.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     7831 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/lib/datatype.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     9687 2023-07-19 04:52:48.000000 safe2pay-0.0.6/safe2pay/entities/lib/entity.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     2479 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/marketplace.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      487 2023-07-15 02:10:52.000000 safe2pay-0.0.6/safe2pay/entities/marketplacelistresponse.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      249 2023-07-15 02:06:48.000000 safe2pay-0.0.6/safe2pay/entities/marketplaceobjects.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      430 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/merchantaccount.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      774 2023-07-15 02:22:55.000000 safe2pay-0.0.6/safe2pay/entities/merchantbankdata.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      600 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/merchantpayment.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      410 2023-07-19 03:25:58.000000 safe2pay-0.0.6/safe2pay/entities/merchantpayment_response.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      360 2023-07-14 13:33:59.000000 safe2pay-0.0.6/safe2pay/entities/merchantsplit.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      275 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/merchanttype.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     3207 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/payment.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     1266 2023-07-19 04:52:40.000000 safe2pay-0.0.6/safe2pay/entities/paymentmethod.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     2339 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/paymentobject.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      506 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/paymentoption.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      585 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/pix.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     3169 2023-08-07 01:35:33.000000 safe2pay-0.0.6/safe2pay/entities/plan.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      460 2023-07-19 04:02:02.000000 safe2pay-0.0.6/safe2pay/entities/plandataresponse.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      409 2023-08-07 01:34:29.000000 safe2pay-0.0.6/safe2pay/entities/planresponse.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     3100 2023-07-19 04:36:17.000000 safe2pay-0.0.6/safe2pay/entities/plansubscription.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      363 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/product.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     4649 2023-07-19 03:26:28.000000 safe2pay-0.0.6/safe2pay/entities/responsedetail.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      319 2023-07-14 14:35:40.000000 safe2pay-0.0.6/safe2pay/entities/responsedetail_account.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     3581 2023-07-14 14:11:12.000000 safe2pay-0.0.6/safe2pay/entities/singlesale.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      427 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/split.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      728 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/staticpix.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      305 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/tax.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     1117 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/token.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     4724 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/entities/transaction.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      457 2023-07-14 13:55:29.000000 safe2pay-0.0.6/safe2pay/entities/transaction_response.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      419 2023-07-14 13:58:44.000000 safe2pay-0.0.6/safe2pay/entities/transactionlistresponse.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      783 2023-07-15 03:27:53.000000 safe2pay-0.0.6/safe2pay/entities/transfer.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     2469 2023-07-16 17:06:58.000000 safe2pay-0.0.6/safe2pay/entities/transferregister.py
+drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-07 01:40:10.783817 safe2pay-0.0.6/safe2pay/utils/
+-rw-r--r--   0 elainecro   (501) staff       (20)       23 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/utils/__init__.py
+-rw-r--r--   0 elainecro   (501) staff       (20)      240 2023-07-13 03:09:51.000000 safe2pay-0.0.6/safe2pay/utils/constants.py
+-rw-r--r--   0 elainecro   (501) staff       (20)     4911 2023-08-07 01:35:38.000000 safe2pay-0.0.6/safe2pay/utils/safe2pay.py
+drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-07 01:40:10.750871 safe2pay-0.0.6/safe2pay.egg-info/
+-rw-r--r--   0 elainecro   (501) staff       (20)    25597 2023-08-07 01:40:10.000000 safe2pay-0.0.6/safe2pay.egg-info/PKG-INFO
+-rw-r--r--   0 elainecro   (501) staff       (20)     2286 2023-08-07 01:40:10.000000 safe2pay-0.0.6/safe2pay.egg-info/SOURCES.txt
+-rw-r--r--   0 elainecro   (501) staff       (20)        1 2023-08-07 01:40:10.000000 safe2pay-0.0.6/safe2pay.egg-info/dependency_links.txt
+-rw-r--r--   0 elainecro   (501) staff       (20)      114 2023-08-07 01:40:10.000000 safe2pay-0.0.6/safe2pay.egg-info/requires.txt
+-rw-r--r--   0 elainecro   (501) staff       (20)        9 2023-08-07 01:40:10.000000 safe2pay-0.0.6/safe2pay.egg-info/top_level.txt
+-rw-r--r--   0 elainecro   (501) staff       (20)      102 2023-08-07 01:40:10.785036 safe2pay-0.0.6/setup.cfg
+-rw-r--r--   0 elainecro   (501) staff       (20)     1227 2023-08-07 01:40:08.000000 safe2pay-0.0.6/setup.py
+drwxr-xr-x   0 elainecro   (501) staff       (20)        0 2023-08-07 01:40:10.784271 safe2pay-0.0.6/test/
+-rw-r--r--   0 elainecro   (501) staff       (20)       89 2023-08-05 00:29:16.000000 safe2pay-0.0.6/test/teste.py
```

### Comparing `safe2pay-0.0.5/LICENSE` & `safe2pay-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/PKG-INFO` & `safe2pay-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe2pay
-Version: 0.0.5
+Version: 0.0.6
 Summary: SDK Python3 para Integração com Safe2Pay
 Home-page: https://github.com/robertons/safe2pay
 Author: Roberto Neves
 Author-email: robertonsilva@gmail.com
 License: MIT
 Keywords: safe2pay,pagamento,cartão de crédito,boleto,pix,pagamentos,transações,payment,payments,credit-card
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `safe2pay-0.0.5/README.md` & `safe2pay-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/__init__.py` & `safe2pay-0.0.6/safe2pay/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/address.py` & `safe2pay-0.0.6/safe2pay/entities/address.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/anticipation.py` & `safe2pay-0.0.6/safe2pay/entities/anticipation.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/bankdata.py` & `safe2pay-0.0.6/safe2pay/entities/bankdata.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/bankslip.py` & `safe2pay-0.0.6/safe2pay/entities/bankslip.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/boleto.py` & `safe2pay-0.0.6/safe2pay/entities/boleto.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/carnet.py` & `safe2pay-0.0.6/safe2pay/entities/carnet.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/carnetasync.py` & `safe2pay-0.0.6/safe2pay/entities/carnetasync.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/chargeback.py` & `safe2pay-0.0.6/safe2pay/entities/chargeback.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/checkingaccount.py` & `safe2pay-0.0.6/safe2pay/entities/checkingaccount.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/creditcard.py` & `safe2pay-0.0.6/safe2pay/entities/creditcard.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/deposit.py` & `safe2pay-0.0.6/safe2pay/entities/deposit.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/installmentvalue.py` & `safe2pay-0.0.6/safe2pay/entities/installmentvalue.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/lib/datatype.py` & `safe2pay-0.0.6/safe2pay/entities/lib/datatype.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/lib/entity.py` & `safe2pay-0.0.6/safe2pay/entities/lib/entity.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/marketplace.py` & `safe2pay-0.0.6/safe2pay/entities/marketplace.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/merchantbankdata.py` & `safe2pay-0.0.6/safe2pay/entities/merchantbankdata.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/merchantpayment.py` & `safe2pay-0.0.6/safe2pay/entities/merchantpayment.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/payment.py` & `safe2pay-0.0.6/safe2pay/entities/payment.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/paymentmethod.py` & `safe2pay-0.0.6/safe2pay/entities/paymentmethod.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/paymentobject.py` & `safe2pay-0.0.6/safe2pay/entities/paymentobject.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/pix.py` & `safe2pay-0.0.6/safe2pay/entities/pix.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/plan.py` & `safe2pay-0.0.6/safe2pay/entities/plan.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/plansubscription.py` & `safe2pay-0.0.6/safe2pay/entities/plansubscription.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/responsedetail.py` & `safe2pay-0.0.6/safe2pay/entities/responsedetail.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/singlesale.py` & `safe2pay-0.0.6/safe2pay/entities/singlesale.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/staticpix.py` & `safe2pay-0.0.6/safe2pay/entities/staticpix.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/token.py` & `safe2pay-0.0.6/safe2pay/entities/token.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/transaction.py` & `safe2pay-0.0.6/safe2pay/entities/transaction.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/transfer.py` & `safe2pay-0.0.6/safe2pay/entities/transfer.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/entities/transferregister.py` & `safe2pay-0.0.6/safe2pay/entities/transferregister.py`

 * *Files identical despite different names*

### Comparing `safe2pay-0.0.5/safe2pay/utils/safe2pay.py` & `safe2pay-0.0.6/safe2pay/utils/safe2pay.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,27 +119,30 @@
             return response.text
     elif response.status_code > 204:
         status_code = response.status_code
         try:
             response_json = response.json()
             response_json['date'] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             response_json['status'] = status_code
+            return response.json()
         except Exception as e:
+            print("Exceçao: ", e)
             response_json = {
                 "date": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                 "status": status_code,
                 "message": "Unexpected Error",
                 "errors": [
                     {
                         "message": str(e),
                         "errorCode": "0"
                     }
                 ]
             }
-        raise Safe2PayException("Safe2Pay Request Error", response_json)
+            return response.text
+        #raise Safe2PayException("Safe2Pay Request Error", response_json)
 
 def DecimalToCents(value) -> int:
     return int(value*100)
 
 def CentsToDecimal(value) -> Decimal:
     return Decimal(Decimal(value)/Decimal(100))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `safe2pay-0.0.5/safe2pay.egg-info/PKG-INFO` & `safe2pay-0.0.6/safe2pay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe2pay
-Version: 0.0.5
+Version: 0.0.6
 Summary: SDK Python3 para Integração com Safe2Pay
 Home-page: https://github.com/robertons/safe2pay
 Author: Roberto Neves
 Author-email: robertonsilva@gmail.com
 License: MIT
 Keywords: safe2pay,pagamento,cartão de crédito,boleto,pix,pagamentos,transações,payment,payments,credit-card
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `safe2pay-0.0.5/safe2pay.egg-info/SOURCES.txt` & `safe2pay-0.0.6/safe2pay.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 safe2pay/entities/chargeback.py
 safe2pay/entities/checkingaccount.py
 safe2pay/entities/city.py
 safe2pay/entities/creditcard.py
 safe2pay/entities/customer.py
 safe2pay/entities/deposit.py
 safe2pay/entities/effectiveness.py
+safe2pay/entities/erroresponse.py
 safe2pay/entities/extract.py
 safe2pay/entities/installments.py
 safe2pay/entities/installmentvalue.py
 safe2pay/entities/integration.py
 safe2pay/entities/marketplace.py
 safe2pay/entities/marketplacelistresponse.py
 safe2pay/entities/marketplaceobjects.py
@@ -65,8 +66,9 @@
 safe2pay/entities/transfer.py
 safe2pay/entities/transferregister.py
 safe2pay/entities/lib/__init__.py
 safe2pay/entities/lib/datatype.py
 safe2pay/entities/lib/entity.py
 safe2pay/utils/__init__.py
 safe2pay/utils/constants.py
-safe2pay/utils/safe2pay.py
+safe2pay/utils/safe2pay.py
+test/teste.py
```

### Comparing `safe2pay-0.0.5/setup.py` & `safe2pay-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 readme = open('README.md').read()
 
 with open('requirements.txt') as reqs:
     requirements = reqs.read().split()
 
 setuptools.setup(
     name='safe2pay',
-    version='0.0.5',
+    version='0.0.6',
     description='SDK Python3 para Integração com Safe2Pay',
     author='Roberto Neves',
     author_email='robertonsilva@gmail.com',
     url='https://github.com/robertons/safe2pay',
     packages=setuptools.find_packages(),
     install_requires=requirements,
     long_description=readme,
```

