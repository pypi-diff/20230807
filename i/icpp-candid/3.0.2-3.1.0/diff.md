# Comparing `tmp/icpp-candid-3.0.2.tar.gz` & `tmp/icpp-candid-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icpp-candid-3.0.2.tar", last modified: Tue Aug  1 19:20:40 2023, max compression
+gzip compressed data, was "icpp-candid-3.1.0.tar", last modified: Mon Aug  7 18:06:09 2023, max compression
```

## Comparing `icpp-candid-3.0.2.tar` & `icpp-candid-3.1.0.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.176572 icpp-candid-3.0.2/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1066 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/LICENSE
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2940 2023-08-01 19:20:40.176572 icpp-candid-3.0.2/PKG-INFO
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2185 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/README.md
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      453 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/pyproject.toml
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       38 2023-08-01 19:20:40.176572 icpp-candid-3.0.2/setup.cfg
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9863 2023-07-17 01:01:37.000000 icpp-candid-3.0.2/setup.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.136572 icpp-candid-3.0.2/src/
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.140572 icpp-candid-3.0.2/src/icpp_candid/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      652 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/__init__.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.168572 icpp-candid-3.0.2/src/icpp_candid/candid/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      381 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_args.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      362 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_args.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1699 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_assert.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      613 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_assert.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    14245 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_deserialize.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1071 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_deserialize.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7115 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_opcode.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2856 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_opcode.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4243 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_serialize.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      989 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_serialize.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3546 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2290 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_all_includes.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1820 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_base.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1955 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_base.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2062 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_bool.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      869 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_bool.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1163 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_empty.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      663 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_empty.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2232 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_float32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      900 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_float32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2239 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_float64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      907 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_float64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1979 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      904 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2031 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2031 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2031 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2004 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      883 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2001 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      910 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2023 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2023 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2023 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1996 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      890 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      816 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_null.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      559 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_null.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1861 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_base.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      445 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_base.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2743 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_bool.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      871 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_bool.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2763 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_float32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      896 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_float32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2769 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_float64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      903 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_float64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2751 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      907 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2744 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2743 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      900 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2743 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2719 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      885 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2757 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      914 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2749 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2749 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2749 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2725 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      892 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3030 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_principal.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      952 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_principal.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3019 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_text.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      920 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_text.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9802 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_principal.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2032 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_principal.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    11268 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_record.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1330 2023-07-20 02:32:24.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_record.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1059 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_reserved.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      677 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_reserved.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2660 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_table.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      618 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_table.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2832 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_text.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      971 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_text.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    13313 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_variant.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1720 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_variant.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1861 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_base.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      445 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_base.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2552 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_bool.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      745 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_bool.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2525 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_float32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      770 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_float32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2532 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_float64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      777 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_float64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2493 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      781 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      772 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      772 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      772 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2516 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      759 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      788 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2555 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      779 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2555 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      779 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2555 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      779 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2530 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      766 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2738 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_principal.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      824 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_principal.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2791 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_text.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      795 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_text.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    20524 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/vec_bytes.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5038 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/candid/vec_bytes.h
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.168572 icpp-candid-3.0.2/src/icpp_candid/hooks/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3481 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/hooks/icpp_hooks.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1192 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/hooks/icpp_hooks.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)       98 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/py.typed
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.136572 icpp-candid-3.0.2/src/icpp_candid/vendors/
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.172572 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1155 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/LICENSE
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3933 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1366 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1342 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3090 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_hex.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3143 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1336 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1381 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3070 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3201 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_url.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1805 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.172572 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/data/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    12087 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/data/access.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2352 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.172572 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7994 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/base32.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5692 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/base64.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    11905 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/codec.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1606 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/config.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4545 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/hex.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    19664 2023-07-16 22:17:57.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3009 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/hex_lower.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2994 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/hex_upper.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3283 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/parse_error.hpp
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.176572 icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      861 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/LICENSE
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    31026 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/crc32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1736 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/crc32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1758 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/readme.md
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    15133 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/sha256.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1968 2023-07-10 11:15:35.000000 icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/sha256.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      322 2023-08-01 19:18:23.000000 icpp-candid-3.0.2/src/icpp_candid/version.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-01 19:20:40.140572 icpp-candid-3.0.2/src/icpp_candid.egg-info/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2940 2023-08-01 19:20:40.000000 icpp-candid-3.0.2/src/icpp_candid.egg-info/PKG-INFO
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     7629 2023-08-01 19:20:40.000000 icpp-candid-3.0.2/src/icpp_candid.egg-info/SOURCES.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        1 2023-08-01 19:20:40.000000 icpp-candid-3.0.2/src/icpp_candid.egg-info/dependency_links.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       45 2023-08-01 19:20:40.000000 icpp-candid-3.0.2/src/icpp_candid.egg-info/requires.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       12 2023-08-01 19:20:40.000000 icpp-candid-3.0.2/src/icpp_candid.egg-info/top_level.txt
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.060775 icpp-candid-3.1.0/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1066 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/LICENSE
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2940 2023-08-07 18:06:09.060775 icpp-candid-3.1.0/PKG-INFO
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2185 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/README.md
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      453 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/pyproject.toml
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       38 2023-08-07 18:06:09.060775 icpp-candid-3.1.0/setup.cfg
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9863 2023-07-17 01:01:37.000000 icpp-candid-3.1.0/setup.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.020775 icpp-candid-3.1.0/src/
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.020775 icpp-candid-3.1.0/src/icpp_candid/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      652 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/__init__.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.052775 icpp-candid-3.1.0/src/icpp_candid/candid/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      381 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_args.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      362 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_args.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1699 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_assert.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      613 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_assert.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    14245 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_deserialize.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1071 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_deserialize.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7115 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_opcode.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2856 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_opcode.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4243 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_serialize.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1052 2023-08-02 16:17:53.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_serialize.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3546 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2290 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_all_includes.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1820 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_base.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1955 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_base.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2062 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_bool.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      869 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_bool.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1163 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_empty.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      663 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_empty.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2232 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_float32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      900 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_float32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2239 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_float64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      907 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_float64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1979 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      904 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2031 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2031 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2031 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2004 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      883 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2001 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      910 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2023 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2023 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2023 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1996 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      890 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      816 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_null.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      559 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_null.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1861 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_base.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      445 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_base.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2743 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_bool.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      871 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_bool.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2763 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_float32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      896 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_float32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2769 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_float64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      903 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_float64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2751 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      907 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2744 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2743 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      900 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2743 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2719 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      885 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2757 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      914 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2749 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2749 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2749 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2725 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      892 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3030 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_principal.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      952 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_principal.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3019 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_text.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      920 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_text.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9802 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_principal.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2032 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_principal.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    11268 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_record.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1330 2023-07-20 02:32:24.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_record.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1059 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_reserved.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      677 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_reserved.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2660 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_table.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      618 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_table.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2832 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_text.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      971 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_text.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    13313 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_variant.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1720 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_variant.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1861 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_base.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      445 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_base.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2552 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_bool.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      745 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_bool.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2525 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_float32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      770 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_float32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2532 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_float64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      777 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_float64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2493 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      781 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      772 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      772 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      772 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2516 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      759 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      788 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2555 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      779 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2555 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      779 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2555 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      779 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2530 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      766 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2738 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_principal.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      824 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_principal.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2791 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_text.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      795 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_text.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    20716 2023-08-02 16:31:59.000000 icpp-candid-3.1.0/src/icpp_candid/candid/vec_bytes.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5061 2023-08-02 16:17:53.000000 icpp-candid-3.1.0/src/icpp_candid/candid/vec_bytes.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.052775 icpp-candid-3.1.0/src/icpp_candid/hooks/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3481 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/hooks/icpp_hooks.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1192 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/hooks/icpp_hooks.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)       98 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/py.typed
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.020775 icpp-candid-3.1.0/src/icpp_candid/vendors/
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.056775 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1155 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/LICENSE
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3933 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1366 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1342 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3090 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_hex.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3143 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1336 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1381 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3070 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3201 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_url.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1805 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.056775 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/data/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    12087 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/data/access.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2352 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.060775 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7994 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/base32.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5692 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/base64.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    11905 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/codec.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1606 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/config.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4545 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/hex.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    19664 2023-07-16 22:17:57.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3009 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/hex_lower.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2994 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/hex_upper.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3283 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/parse_error.hpp
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.060775 icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      861 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/LICENSE
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    31026 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/crc32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1736 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/crc32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1758 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/readme.md
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    15133 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/sha256.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1968 2023-07-10 11:15:35.000000 icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/sha256.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      322 2023-08-07 18:03:35.000000 icpp-candid-3.1.0/src/icpp_candid/version.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-08-07 18:06:09.024775 icpp-candid-3.1.0/src/icpp_candid.egg-info/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2940 2023-08-07 18:06:09.000000 icpp-candid-3.1.0/src/icpp_candid.egg-info/PKG-INFO
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     7629 2023-08-07 18:06:09.000000 icpp-candid-3.1.0/src/icpp_candid.egg-info/SOURCES.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        1 2023-08-07 18:06:09.000000 icpp-candid-3.1.0/src/icpp_candid.egg-info/dependency_links.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       45 2023-08-07 18:06:09.000000 icpp-candid-3.1.0/src/icpp_candid.egg-info/requires.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       12 2023-08-07 18:06:09.000000 icpp-candid-3.1.0/src/icpp_candid.egg-info/top_level.txt
```

### Comparing `icpp-candid-3.0.2/LICENSE` & `icpp-candid-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/PKG-INFO` & `icpp-candid-3.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-candid
-Version: 3.0.2
+Version: 3.1.0
 Summary: C++ Candid Library
 Home-page: https://docs.icpp.world/
 Author: icppWorld
 Author-email: icpp@icpp.world
 License: MIT
 Keywords: C++ Candid Library,Internet Computer,C++,Candid,blockchain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `icpp-candid-3.0.2/README.md` & `icpp-candid-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/setup.py` & `icpp-candid-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/__init__.py` & `icpp-candid-3.1.0/src/icpp_candid/__init__.py`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_assert.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_assert.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_assert.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_assert.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_deserialize.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_deserialize.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_deserialize.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_deserialize.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_opcode.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_opcode.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_opcode.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_opcode.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_serialize.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_serialize.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_serialize.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_serialize.h`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,16 @@
   CandidArgs get_A() { return m_A; }
   VecBytes get_B() { return m_B; }
   __uint128_t get_num_typetables() { return m_num_typetables; }
 
   int assert_candid(const std::string &candid_expected,
                     const bool &assert_value);
 
+  std::string as_hex_string() { return m_B.as_hex_string(); }
+
 private:
   void serialize();
 
   // The argument list to be serialized
   CandidArgs m_A;
 
   // The serialized byte stream
```

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_all_includes.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_all_includes.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_base.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_base.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_base.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_base.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_bool.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_bool.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_bool.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_bool.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_empty.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_empty.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_empty.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_empty.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_float32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_float32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_float32.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_float32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_float64.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_float64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_float64.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_float64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int16.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int16.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int32.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int64.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int64.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int8.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_int8.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_int8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat16.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat16.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat32.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat64.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat64.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat8.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_nat8.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_nat8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_null.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_null.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_null.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_null.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_base.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_base.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_bool.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_bool.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_bool.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_bool.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_float32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_float32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_float32.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_float32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_float64.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_float64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_float64.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_float64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int16.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int16.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int32.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int64.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int64.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int8.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_int8.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_int8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat16.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat16.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat32.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat64.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat64.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat8.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_nat8.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_nat8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_principal.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_principal.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_principal.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_principal.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_text.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_text.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_opt_text.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_opt_text.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_principal.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_principal.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_principal.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_principal.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_record.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_record.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_record.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_record.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_reserved.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_reserved.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_reserved.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_reserved.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_table.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_table.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_table.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_table.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_text.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_text.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_text.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_text.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_variant.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_variant.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_variant.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_variant.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_base.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_base.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_bool.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_bool.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_bool.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_bool.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_float32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_float32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_float32.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_float32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_float64.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_float64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_float64.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_float64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int16.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int16.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int32.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int64.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int64.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int8.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_int8.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_int8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat16.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat16.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat32.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat64.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat64.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat8.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_nat8.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_nat8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_principal.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_principal.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_principal.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_principal.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_text.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_text.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/candid_type_vec_text.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/candid_type_vec_text.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/vec_bytes.cpp` & `icpp-candid-3.1.0/src/icpp_candid/candid/vec_bytes.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 //  Wrapper around a std::vector<std::byte>
 
 #include "vec_bytes.h"
 
 #include <cassert>
-#include <cstring>
 #include <cstdint>
+#include <cstring>
 
 #include <algorithm>
 #include <bit>
 #include <string>
 
 #include <limits.h>
 #include <limits>
@@ -307,14 +307,23 @@
   s.append(byte_to_char(m_vec[2]));
   s.append(byte_to_char(m_vec[3]));
   if (s != "DIDL") {
     ICPP_HOOKS::trap("ERROR: Message does not start with DIDL");
   }
 }
 
+// Returns the bytes of the vec as a hex string
+std::string VecBytes::as_hex_string() {
+  std::string s_hex;
+  for (std::byte b : m_vec) {
+    s_hex.append(byte_to_hex(b, ""));
+  }
+  return s_hex;
+}
+
 // Prints the bytes of the vec in hex, dec & bits
 void VecBytes::debug_print() {
   ICPP_HOOKS::debug_print("  hex, decimal, char");
 
   std::string s_hex;
   for (std::byte b : m_vec) {
     std::string s;
@@ -564,15 +573,15 @@
 void VecBytes::trap(const std::string &msg) { ICPP_HOOKS::trap(msg); }
 
 // -----------------------------------------------------------------------------
 // template definitions with Explicit Template Instantiations
 // Doing it this way avoids the COMDAT warnings & multiple definitions errors
 
 template <typename T>
-  requires MyFixedWidthInts<T>
+requires MyFixedWidthInts<T>
 void VecBytes::append_int_fixed_width(const T &v) {
   uint8_t *bytes{nullptr};
   if (is_little_endian()) bytes = (uint8_t *)&v;
   else
     // Probably best to do a memcpy and then a byteswap
     trap(
         "ERROR: append_int_fixed_width not yet implemented on big endian architecture");
@@ -588,15 +597,15 @@
 template void VecBytes::append_int_fixed_width<uint16_t>(const uint16_t &v);
 template void VecBytes::append_int_fixed_width<uint32_t>(const uint32_t &v);
 template void VecBytes::append_int_fixed_width<uint64_t>(const uint64_t &v);
 // clang-format on
 
 // --
 template <typename T>
-  requires MyFloats<T>
+requires MyFloats<T>
 void VecBytes::append_float_ieee754(const T &v) {
   if (is_float_ieee754()) {
     // https://github.com/dfinity/candid/blob/master/spec/Candid.md#floating-point-numbers
     // Floating-point values are represented in IEEE 754 binary format and are
     // supported in single precision (32 bit) and double precision (64 bit).
     // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
     // M(z : float<N>) = f<N>(z)
@@ -612,15 +621,15 @@
 // clang-format off
 template void VecBytes::append_float_ieee754<float>  (const float &v);
 template void VecBytes::append_float_ieee754<double> (const double &v);
 // clang-format on
 
 // --
 template <typename T>
-  requires MyFixedWidthInts<T>
+requires MyFixedWidthInts<T>
 bool VecBytes::parse_int_fixed_width(__uint128_t &offset, T &v,
                                      std::string &parse_error) {
   __uint128_t len = m_vec.size() - offset;
 
   uint8_t *buf = &m_vec_uint8_t[offset];
   uint8_t *buf_end = &m_vec_uint8_t[offset + len];
 
@@ -641,15 +650,15 @@
 template bool VecBytes::parse_int_fixed_width<uint16_t>(__uint128_t &offset, uint16_t &v, std::string &parse_error);
 template bool VecBytes::parse_int_fixed_width<uint32_t>(__uint128_t &offset, uint32_t &v, std::string &parse_error);
 template bool VecBytes::parse_int_fixed_width<uint64_t>(__uint128_t &offset, uint64_t &v, std::string &parse_error);
 // clang-format on
 
 // --
 template <typename T>
-  requires MyFloats<T>
+requires MyFloats<T>
 bool VecBytes::parse_float_ieee754(__uint128_t &offset, T &v,
                                    std::string &parse_error) {
   if (is_float_ieee754()) {
     // https://github.com/dfinity/candid/blob/master/spec/Candid.md#floating-point-numbers
     // Floating-point values are represented in IEEE 754 binary format and are
     // supported in single precision (32 bit) and double precision (64 bit).
     // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
```

### Comparing `icpp-candid-3.0.2/src/icpp_candid/candid/vec_bytes.h` & `icpp-candid-3.1.0/src/icpp_candid/candid/vec_bytes.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 //  Wrapper around a std::vector<std::byte>
 
 #pragma once
 
-#include <cstring>
 #include <cstdint>
+#include <cstring>
 
 #include <string>
 #include <vector>
 
 template <typename T>
 concept MyFixedWidthInts =
     std::is_same_v<T, uint8_t> || std::is_same_v<T, uint16_t> ||
@@ -76,19 +76,19 @@
   template <class T> void append_sleb128(T) = delete;
 
   void append_uleb128(const bool &v);
   void append_uleb128(const __uint128_t &v);
   template <class T> void append_uleb128(T) = delete;
 
   template <typename T>
-    requires MyFixedWidthInts<T>
+  requires MyFixedWidthInts<T>
   void append_int_fixed_width(const T &v);
 
   template <typename T>
-    requires MyFloats<T>
+  requires MyFloats<T>
   void append_float_ieee754(const T &v);
 
   // parse methods
   void trap_if_vec_does_not_start_with_DIDL();
 
   bool parse_uleb128(__uint128_t &offset, __uint128_t &v, __uint128_t &numbytes,
                      std::string &parse_error);
@@ -99,34 +99,35 @@
   bool parse_sleb128(__uint128_t &offset, __int128_t &v, __uint128_t &numbytes,
                      std::string &parse_error);
   template <class T>
   bool parse_sleb128(__uint128_t &, T, __uint128_t &numbytes,
                      std::string &parse_error) = delete;
 
   template <typename T>
-    requires MyFixedWidthInts<T>
+  requires MyFixedWidthInts<T>
   bool parse_int_fixed_width(__uint128_t &offset, T &v,
                              std::string &parse_error);
 
   template <typename T>
-    requires MyFloats<T>
+  requires MyFloats<T>
   bool parse_float_ieee754(__uint128_t &offset, T &v, std::string &parse_error);
 
   bool parse_bytes(__uint128_t &offset, std::vector<std::byte> &v,
                    __uint128_t &n, __uint128_t &numbytes,
                    std::string &parse_error);
   bool parse_bytes(__uint128_t &offset, std::vector<uint8_t> &v, __uint128_t &n,
                    __uint128_t &numbytes, std::string &parse_error);
 
   // store methods
   void store(const uint8_t *bytes, const uint32_t num_bytes);
   void store_hex_string(const std::string candid_in);
   void store_hex_tokens(std::vector<std::string> hex_tokens);
 
   // helper methods
+  std::string as_hex_string();
   void debug_print();
   const std::vector<std::byte> &vec() const { return m_vec; };
   const std::vector<uint8_t> &vec_uint8_t() const { return m_vec_uint8_t; };
   int size() const { return m_vec.size(); }
   void clear();
   bool is_little_endian();
   bool is_big_endian();
```

### Comparing `icpp-candid-3.0.2/src/icpp_candid/hooks/icpp_hooks.cpp` & `icpp-candid-3.1.0/src/icpp_candid/hooks/icpp_hooks.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/hooks/icpp_hooks.h` & `icpp-candid-3.1.0/src/icpp_candid/hooks/icpp_hooks.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/LICENSE` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_hex.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_hex.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_url.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_url.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/data/access.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/data/access.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/base32.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/base32.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/base64.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/base64.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/codec.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/codec.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/config.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/config.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/hex.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/hex.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/hex_lower.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/hex_lower.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/hex_upper.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/hex_upper.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/cppcodec/parse_error.hpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/cppcodec/parse_error.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/LICENSE` & `icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/crc32.cpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/crc32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/crc32.h` & `icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/crc32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/readme.md` & `icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/readme.md`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/sha256.cpp` & `icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/sha256.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid/vendors/hash-library/sha256.h` & `icpp-candid-3.1.0/src/icpp_candid/vendors/hash-library/sha256.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.0.2/src/icpp_candid.egg-info/PKG-INFO` & `icpp-candid-3.1.0/src/icpp_candid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-candid
-Version: 3.0.2
+Version: 3.1.0
 Summary: C++ Candid Library
 Home-page: https://docs.icpp.world/
 Author: icppWorld
 Author-email: icpp@icpp.world
 License: MIT
 Keywords: C++ Candid Library,Internet Computer,C++,Candid,blockchain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `icpp-candid-3.0.2/src/icpp_candid.egg-info/SOURCES.txt` & `icpp-candid-3.1.0/src/icpp_candid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

