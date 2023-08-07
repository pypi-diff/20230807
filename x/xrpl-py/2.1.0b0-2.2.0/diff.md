# Comparing `tmp/xrpl_py-2.1.0b0.tar.gz` & `tmp/xrpl_py-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrpl_py-2.1.0b0.tar", max compression
+gzip compressed data, was "xrpl_py-2.2.0.tar", max compression
```

## Comparing `xrpl_py-2.1.0b0.tar` & `xrpl_py-2.2.0.tar`

### file list

```diff
@@ -1,241 +1,223 @@
--rw-r--r--   0        0        0      740 2022-08-01 03:07:06.902817 xrpl_py-2.1.0b0/LICENSE
--rw-r--r--   0        0        0    16001 2023-07-10 17:12:46.149667 xrpl_py-2.1.0b0/README.md
--rw-r--r--   0        0        0     2229 2023-07-10 17:42:47.452415 xrpl_py-2.1.0b0/pyproject.toml
--rw-r--r--   0        0        0      348 2022-08-01 03:07:06.915966 xrpl_py-2.1.0b0/xrpl/__init__.py
--rw-r--r--   0        0        0      393 2023-07-10 17:12:46.163012 xrpl_py-2.1.0b0/xrpl/account/__init__.py
--rw-r--r--   0        0        0     3376 2023-07-10 17:12:46.163184 xrpl_py-2.1.0b0/xrpl/account/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.916219 xrpl_py-2.1.0b0/xrpl/account/py.typed
--rw-r--r--   0        0        0      776 2023-07-10 17:12:46.163338 xrpl_py-2.1.0b0/xrpl/account/transaction_history.py
--rw-r--r--   0        0        0      189 2022-08-01 03:07:06.916458 xrpl_py-2.1.0b0/xrpl/asyncio/__init__.py
--rw-r--r--   0        0        0      415 2023-07-10 17:12:46.163581 xrpl_py-2.1.0b0/xrpl/asyncio/account/__init__.py
--rw-r--r--   0        0        0     4245 2023-07-10 17:12:46.163782 xrpl_py-2.1.0b0/xrpl/asyncio/account/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.916659 xrpl_py-2.1.0b0/xrpl/asyncio/account/py.typed
--rw-r--r--   0        0        0     1170 2023-07-10 17:12:46.163955 xrpl_py-2.1.0b0/xrpl/asyncio/account/transaction_history.py
--rw-r--r--   0        0        0      705 2022-08-01 03:07:06.916816 xrpl_py-2.1.0b0/xrpl/asyncio/clients/__init__.py
--rw-r--r--   0        0        0      692 2023-01-09 23:03:27.485595 xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_client.py
--rw-r--r--   0        0        0      315 2022-08-01 03:07:06.916941 xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_json_rpc_client.py
--rw-r--r--   0        0        0     7149 2023-05-23 16:51:49.263971 xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_websocket_client.py
--rw-r--r--   0        0        0     1189 2023-07-10 17:12:46.164105 xrpl_py-2.1.0b0/xrpl/asyncio/clients/client.py
--rw-r--r--   0        0        0     1083 2022-08-01 03:07:06.917148 xrpl_py-2.1.0b0/xrpl/asyncio/clients/exceptions.py
--rw-r--r--   0        0        0     1612 2023-01-09 23:03:27.486437 xrpl_py-2.1.0b0/xrpl/asyncio/clients/json_rpc_base.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917264 xrpl_py-2.1.0b0/xrpl/asyncio/clients/py.typed
--rw-r--r--   0        0        0     3341 2022-08-01 03:07:06.917343 xrpl_py-2.1.0b0/xrpl/asyncio/clients/utils.py
--rw-r--r--   0        0        0     8173 2023-05-23 16:51:49.264461 xrpl_py-2.1.0b0/xrpl/asyncio/clients/websocket_base.py
--rw-r--r--   0        0        0      328 2022-08-01 03:07:06.917510 xrpl_py-2.1.0b0/xrpl/asyncio/ledger/__init__.py
--rw-r--r--   0        0        0     3443 2023-01-09 23:03:27.487487 xrpl_py-2.1.0b0/xrpl/asyncio/ledger/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917612 xrpl_py-2.1.0b0/xrpl/asyncio/ledger/py.typed
--rw-r--r--   0        0        0     2353 2022-08-01 03:07:06.917676 xrpl_py-2.1.0b0/xrpl/asyncio/ledger/utils.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917699 xrpl_py-2.1.0b0/xrpl/asyncio/py.typed
--rw-r--r--   0        0        0      569 2023-07-10 17:12:46.164296 xrpl_py-2.1.0b0/xrpl/asyncio/transaction/__init__.py
--rw-r--r--   0        0        0    17903 2023-07-10 17:12:46.164855 xrpl_py-2.1.0b0/xrpl/asyncio/transaction/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917997 xrpl_py-2.1.0b0/xrpl/asyncio/transaction/py.typed
--rw-r--r--   0        0        0     8210 2023-07-10 17:12:46.165121 xrpl_py-2.1.0b0/xrpl/asyncio/transaction/reliable_submission.py
--rw-r--r--   0        0        0      219 2022-08-01 03:07:06.918169 xrpl_py-2.1.0b0/xrpl/asyncio/wallet/__init__.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.918193 xrpl_py-2.1.0b0/xrpl/asyncio/wallet/py.typed
--rw-r--r--   0        0        0     6614 2023-07-10 17:12:46.165310 xrpl_py-2.1.0b0/xrpl/asyncio/wallet/wallet_generation.py
--rw-r--r--   0        0        0      656 2022-08-01 03:07:06.918352 xrpl_py-2.1.0b0/xrpl/clients/__init__.py
--rw-r--r--   0        0        0      295 2022-08-01 03:07:06.918414 xrpl_py-2.1.0b0/xrpl/clients/json_rpc_client.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.918443 xrpl_py-2.1.0b0/xrpl/clients/py.typed
--rw-r--r--   0        0        0      705 2023-01-09 23:03:27.488832 xrpl_py-2.1.0b0/xrpl/clients/sync_client.py
--rw-r--r--   0        0        0     8893 2023-05-23 16:51:49.266224 xrpl_py-2.1.0b0/xrpl/clients/websocket_client.py
--rw-r--r--   0        0        0     1414 2022-08-01 03:07:06.918722 xrpl_py-2.1.0b0/xrpl/constants.py
--rw-r--r--   0        0        0      171 2022-08-01 03:07:06.918808 xrpl_py-2.1.0b0/xrpl/core/__init__.py
--rw-r--r--   0        0        0     1131 2023-07-10 17:12:46.165519 xrpl_py-2.1.0b0/xrpl/core/addresscodec/__init__.py
--rw-r--r--   0        0        0     7175 2022-08-01 03:07:06.918953 xrpl_py-2.1.0b0/xrpl/core/addresscodec/codec.py
--rw-r--r--   0        0        0      194 2022-08-01 03:07:06.919006 xrpl_py-2.1.0b0/xrpl/core/addresscodec/exceptions.py
--rw-r--r--   0        0        0     5735 2023-07-10 17:12:46.165893 xrpl_py-2.1.0b0/xrpl/core/addresscodec/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.919094 xrpl_py-2.1.0b0/xrpl/core/addresscodec/py.typed
--rw-r--r--   0        0        0      235 2022-08-01 03:07:06.919150 xrpl_py-2.1.0b0/xrpl/core/addresscodec/utils.py
--rw-r--r--   0        0        0      488 2022-08-01 03:07:06.919229 xrpl_py-2.1.0b0/xrpl/core/binarycodec/__init__.py
--rw-r--r--   0        0        0      296 2022-08-01 03:07:06.919308 xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/__init__.py
--rw-r--r--   0        0        0     9076 2022-08-01 03:07:06.919401 xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py
--rw-r--r--   0        0        0     4650 2022-08-01 03:07:06.919480 xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py
--rw-r--r--   0        0        0     1025 2022-08-01 03:07:06.919564 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/__init__.py
--rw-r--r--   0        0        0    56327 2023-07-10 16:48:55.570924 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.json
--rw-r--r--   0        0        0     8431 2022-08-01 03:07:06.919791 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.py
--rw-r--r--   0        0        0     2060 2023-07-10 16:48:55.571160 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_header.py
--rw-r--r--   0        0        0     1192 2022-08-01 03:07:06.919903 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_info.py
--rw-r--r--   0        0        0     1931 2022-08-01 03:07:06.919964 xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_instance.py
--rw-r--r--   0        0        0      191 2022-08-01 03:07:06.920016 xrpl_py-2.1.0b0/xrpl/core/binarycodec/exceptions.py
--rw-r--r--   0        0        0     3942 2022-08-01 03:07:06.920077 xrpl_py-2.1.0b0/xrpl/core/binarycodec/field_id_codec.py
--rw-r--r--   0        0        0     3898 2023-07-10 16:48:55.571442 xrpl_py-2.1.0b0/xrpl/core/binarycodec/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.920169 xrpl_py-2.1.0b0/xrpl/core/binarycodec/py.typed
--rw-r--r--   0        0        0     1407 2023-07-10 16:48:55.571638 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/__init__.py
--rw-r--r--   0        0        0     2956 2022-08-01 03:07:06.920334 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/account_id.py
--rw-r--r--   0        0        0    11513 2023-05-23 16:51:49.266730 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/amount.py
--rw-r--r--   0        0        0     1950 2022-08-01 03:07:06.920520 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/blob.py
--rw-r--r--   0        0        0     4347 2022-08-01 03:07:06.920602 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/currency.py
--rw-r--r--   0        0        0     2640 2022-08-01 03:07:06.920654 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash.py
--rw-r--r--   0        0        0     1494 2023-02-15 23:24:27.094208 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash128.py
--rw-r--r--   0        0        0      571 2022-08-01 03:07:06.920764 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash160.py
--rw-r--r--   0        0        0      572 2022-08-01 03:07:06.920890 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash256.py
--rw-r--r--   0        0        0     3325 2023-07-10 16:48:55.572074 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/issue.py
--rw-r--r--   0        0        0     3335 2023-07-10 16:48:55.572315 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/issued_currency.py
--rw-r--r--   0        0        0     9067 2022-08-01 03:07:06.921018 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/path_set.py
--rw-r--r--   0        0        0     2493 2022-08-01 03:07:06.921099 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/serialized_type.py
--rw-r--r--   0        0        0     3301 2022-08-01 03:07:06.921166 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_array.py
--rw-r--r--   0        0        0     8392 2023-05-23 16:51:49.267029 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_object.py
--rw-r--r--   0        0        0     3383 2022-08-01 03:07:06.921335 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint.py
--rw-r--r--   0        0        0     2063 2022-08-01 03:07:06.921397 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint16.py
--rw-r--r--   0        0        0     2283 2022-08-01 03:07:06.921488 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint32.py
--rw-r--r--   0        0        0     2854 2022-08-01 03:07:06.921562 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint64.py
--rw-r--r--   0        0        0     1994 2022-08-01 03:07:06.921617 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint8.py
--rw-r--r--   0        0        0     2905 2022-08-01 03:07:06.921683 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/vector256.py
--rw-r--r--   0        0        0     3407 2023-07-10 16:48:55.572418 xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/xchain_bridge.py
--rw-r--r--   0        0        0      447 2023-01-09 23:03:27.489834 xrpl_py-2.1.0b0/xrpl/core/keypairs/__init__.py
--rw-r--r--   0        0        0     1275 2022-08-01 03:07:06.921836 xrpl_py-2.1.0b0/xrpl/core/keypairs/crypto_implementation.py
--rw-r--r--   0        0        0     3662 2023-07-10 17:12:46.166050 xrpl_py-2.1.0b0/xrpl/core/keypairs/ed25519.py
--rw-r--r--   0        0        0      182 2022-08-01 03:07:06.921991 xrpl_py-2.1.0b0/xrpl/core/keypairs/exceptions.py
--rw-r--r--   0        0        0      893 2023-01-09 23:03:27.490087 xrpl_py-2.1.0b0/xrpl/core/keypairs/helpers.py
--rw-r--r--   0        0        0     4881 2023-07-10 17:12:46.166195 xrpl_py-2.1.0b0/xrpl/core/keypairs/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922143 xrpl_py-2.1.0b0/xrpl/core/keypairs/py.typed
--rw-r--r--   0        0        0     7480 2022-08-01 03:07:06.922211 xrpl_py-2.1.0b0/xrpl/core/keypairs/secp256k1.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922235 xrpl_py-2.1.0b0/xrpl/core/py.typed
--rw-r--r--   0        0        0      314 2022-08-01 03:07:06.922326 xrpl_py-2.1.0b0/xrpl/ledger/__init__.py
--rw-r--r--   0        0        0     2283 2022-08-01 03:07:06.922387 xrpl_py-2.1.0b0/xrpl/ledger/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922410 xrpl_py-2.1.0b0/xrpl/ledger/py.typed
--rw-r--r--   0        0        0      997 2023-07-10 16:48:55.573510 xrpl_py-2.1.0b0/xrpl/models/__init__.py
--rw-r--r--   0        0        0      497 2022-08-01 03:07:06.922581 xrpl_py-2.1.0b0/xrpl/models/amounts/__init__.py
--rw-r--r--   0        0        0     1377 2022-08-01 03:07:06.922638 xrpl_py-2.1.0b0/xrpl/models/amounts/amount.py
--rw-r--r--   0        0        0     1349 2022-09-14 22:10:28.650164 xrpl_py-2.1.0b0/xrpl/models/amounts/issued_currency_amount.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922737 xrpl_py-2.1.0b0/xrpl/models/amounts/py.typed
--rw-r--r--   0        0        0     2319 2023-07-10 16:48:55.573804 xrpl_py-2.1.0b0/xrpl/models/auth_account.py
--rw-r--r--   0        0        0    11037 2023-07-10 16:48:55.574109 xrpl_py-2.1.0b0/xrpl/models/base_model.py
--rw-r--r--   0        0        0      371 2023-02-23 18:51:59.114959 xrpl_py-2.1.0b0/xrpl/models/currencies/__init__.py
--rw-r--r--   0        0        0      319 2022-11-17 15:10:10.681283 xrpl_py-2.1.0b0/xrpl/models/currencies/currency.py
--rw-r--r--   0        0        0     2237 2022-08-01 03:07:06.923061 xrpl_py-2.1.0b0/xrpl/models/currencies/issued_currency.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.923083 xrpl_py-2.1.0b0/xrpl/models/currencies/py.typed
--rw-r--r--   0        0        0     2918 2023-07-10 17:12:46.166342 xrpl_py-2.1.0b0/xrpl/models/currencies/xrp.py
--rw-r--r--   0        0        0      171 2022-08-01 03:07:06.923203 xrpl_py-2.1.0b0/xrpl/models/exceptions.py
--rw-r--r--   0        0        0     4661 2023-07-10 17:12:46.166725 xrpl_py-2.1.0b0/xrpl/models/flags.py
--rw-r--r--   0        0        0     2462 2023-01-09 23:03:27.490815 xrpl_py-2.1.0b0/xrpl/models/nested_model.py
--rw-r--r--   0        0        0     2088 2022-09-15 01:11:48.323392 xrpl_py-2.1.0b0/xrpl/models/path.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.923353 xrpl_py-2.1.0b0/xrpl/models/py.typed
--rw-r--r--   0        0        0     3740 2023-07-10 16:48:55.575204 xrpl_py-2.1.0b0/xrpl/models/requests/__init__.py
--rw-r--r--   0        0        0     1549 2023-07-10 17:12:46.166921 xrpl_py-2.1.0b0/xrpl/models/requests/account_channels.py
--rw-r--r--   0        0        0     1134 2023-07-10 17:12:46.167126 xrpl_py-2.1.0b0/xrpl/models/requests/account_currencies.py
--rw-r--r--   0        0        0     1088 2023-07-10 17:12:46.167293 xrpl_py-2.1.0b0/xrpl/models/requests/account_info.py
--rw-r--r--   0        0        0     1323 2023-07-10 17:12:46.167456 xrpl_py-2.1.0b0/xrpl/models/requests/account_lines.py
--rw-r--r--   0        0        0     1216 2023-07-10 17:12:46.167656 xrpl_py-2.1.0b0/xrpl/models/requests/account_nfts.py
--rw-r--r--   0        0        0     1894 2023-07-10 17:12:46.168085 xrpl_py-2.1.0b0/xrpl/models/requests/account_objects.py
--rw-r--r--   0        0        0     1161 2023-07-10 17:12:46.168281 xrpl_py-2.1.0b0/xrpl/models/requests/account_offers.py
--rw-r--r--   0        0        0     1207 2023-07-10 17:12:46.168502 xrpl_py-2.1.0b0/xrpl/models/requests/account_tx.py
--rw-r--r--   0        0        0     1017 2023-07-10 16:48:55.577338 xrpl_py-2.1.0b0/xrpl/models/requests/amm_info.py
--rw-r--r--   0        0        0     1024 2023-07-10 17:12:46.168659 xrpl_py-2.1.0b0/xrpl/models/requests/book_offers.py
--rw-r--r--   0        0        0     3048 2023-07-10 16:48:55.577739 xrpl_py-2.1.0b0/xrpl/models/requests/channel_authorize.py
--rw-r--r--   0        0        0     1158 2023-07-10 16:48:55.578010 xrpl_py-2.1.0b0/xrpl/models/requests/channel_verify.py
--rw-r--r--   0        0        0     1145 2023-07-10 17:12:46.168920 xrpl_py-2.1.0b0/xrpl/models/requests/deposit_authorized.py
--rw-r--r--   0        0        0      775 2022-08-01 03:07:06.924306 xrpl_py-2.1.0b0/xrpl/models/requests/fee.py
--rw-r--r--   0        0        0     1076 2023-07-10 17:12:46.169151 xrpl_py-2.1.0b0/xrpl/models/requests/gateway_balances.py
--rw-r--r--   0        0        0     3068 2022-08-01 03:07:06.924450 xrpl_py-2.1.0b0/xrpl/models/requests/generic_request.py
--rw-r--r--   0        0        0      887 2023-07-10 17:12:46.169383 xrpl_py-2.1.0b0/xrpl/models/requests/ledger.py
--rw-r--r--   0        0        0      944 2022-08-01 03:07:06.924563 xrpl_py-2.1.0b0/xrpl/models/requests/ledger_closed.py
--rw-r--r--   0        0        0      726 2022-08-01 03:07:06.924621 xrpl_py-2.1.0b0/xrpl/models/requests/ledger_current.py
--rw-r--r--   0        0        0     1190 2023-07-10 17:12:46.169752 xrpl_py-2.1.0b0/xrpl/models/requests/ledger_data.py
--rw-r--r--   0        0        0     6160 2023-07-10 17:12:46.170014 xrpl_py-2.1.0b0/xrpl/models/requests/ledger_entry.py
--rw-r--r--   0        0        0      853 2022-08-01 03:07:06.924810 xrpl_py-2.1.0b0/xrpl/models/requests/manifest.py
--rw-r--r--   0        0        0      809 2023-07-10 17:12:46.170217 xrpl_py-2.1.0b0/xrpl/models/requests/nft_buy_offers.py
--rw-r--r--   0        0        0     1184 2023-07-10 17:12:46.170408 xrpl_py-2.1.0b0/xrpl/models/requests/nft_history.py
--rw-r--r--   0        0        0      772 2023-07-10 17:12:46.170596 xrpl_py-2.1.0b0/xrpl/models/requests/nft_info.py
--rw-r--r--   0        0        0      816 2023-07-10 17:12:46.170821 xrpl_py-2.1.0b0/xrpl/models/requests/nft_sell_offers.py
--rw-r--r--   0        0        0     1446 2023-07-10 17:12:46.171216 xrpl_py-2.1.0b0/xrpl/models/requests/no_ripple_check.py
--rw-r--r--   0        0        0     4347 2022-08-01 03:07:06.925088 xrpl_py-2.1.0b0/xrpl/models/requests/path_find.py
--rw-r--r--   0        0        0      547 2022-08-01 03:07:06.925142 xrpl_py-2.1.0b0/xrpl/models/requests/ping.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.925165 xrpl_py-2.1.0b0/xrpl/models/requests/py.typed
--rw-r--r--   0        0        0      579 2022-08-01 03:07:06.925223 xrpl_py-2.1.0b0/xrpl/models/requests/random.py
--rw-r--r--   0        0        0     6279 2023-07-10 17:12:46.171586 xrpl_py-2.1.0b0/xrpl/models/requests/request.py
--rw-r--r--   0        0        0     2280 2023-07-10 17:12:46.171767 xrpl_py-2.1.0b0/xrpl/models/requests/ripple_path_find.py
--rw-r--r--   0        0        0      618 2022-08-01 03:07:06.925432 xrpl_py-2.1.0b0/xrpl/models/requests/server_info.py
--rw-r--r--   0        0        0     1194 2022-08-01 03:07:06.925493 xrpl_py-2.1.0b0/xrpl/models/requests/server_state.py
--rw-r--r--   0        0        0     4034 2022-08-01 03:07:06.925582 xrpl_py-2.1.0b0/xrpl/models/requests/sign.py
--rw-r--r--   0        0        0     5062 2022-08-01 03:07:06.925632 xrpl_py-2.1.0b0/xrpl/models/requests/sign_and_submit.py
--rw-r--r--   0        0        0     3274 2022-08-01 03:07:06.925686 xrpl_py-2.1.0b0/xrpl/models/requests/sign_for.py
--rw-r--r--   0        0        0     3758 2022-08-01 03:07:06.925767 xrpl_py-2.1.0b0/xrpl/models/requests/submit.py
--rw-r--r--   0        0        0     2478 2022-08-01 03:07:06.925860 xrpl_py-2.1.0b0/xrpl/models/requests/submit_multisigned.py
--rw-r--r--   0        0        0     2842 2022-08-01 03:07:06.925936 xrpl_py-2.1.0b0/xrpl/models/requests/submit_only.py
--rw-r--r--   0        0        0     2103 2022-08-01 03:07:06.926016 xrpl_py-2.1.0b0/xrpl/models/requests/subscribe.py
--rw-r--r--   0        0        0     1200 2023-07-10 17:12:46.171975 xrpl_py-2.1.0b0/xrpl/models/requests/transaction_entry.py
--rw-r--r--   0        0        0      817 2022-08-01 03:07:06.926139 xrpl_py-2.1.0b0/xrpl/models/requests/tx.py
--rw-r--r--   0        0        0     1595 2022-08-01 03:07:06.926195 xrpl_py-2.1.0b0/xrpl/models/requests/unsubscribe.py
--rw-r--r--   0        0        0      251 2022-08-01 03:07:06.926255 xrpl_py-2.1.0b0/xrpl/models/required.py
--rw-r--r--   0        0        0     3617 2022-08-01 03:07:06.926326 xrpl_py-2.1.0b0/xrpl/models/response.py
--rw-r--r--   0        0        0     5016 2023-07-10 17:12:46.172406 xrpl_py-2.1.0b0/xrpl/models/transactions/__init__.py
--rw-r--r--   0        0        0     1333 2022-08-01 03:07:06.926509 xrpl_py-2.1.0b0/xrpl/models/transactions/account_delete.py
--rw-r--r--   0        0        0     9705 2023-07-10 17:12:46.172625 xrpl_py-2.1.0b0/xrpl/models/transactions/account_set.py
--rw-r--r--   0        0        0     2644 2023-07-10 16:48:55.581988 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_bid.py
--rw-r--r--   0        0        0     2135 2023-07-10 16:48:55.582269 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_create.py
--rw-r--r--   0        0        0     3164 2023-07-10 16:48:55.582630 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_deposit.py
--rw-r--r--   0        0        0     1984 2023-07-10 16:48:55.582934 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_vote.py
--rw-r--r--   0        0        0     3286 2023-07-10 16:48:55.583236 xrpl_py-2.1.0b0/xrpl/models/transactions/amm_withdraw.py
--rw-r--r--   0        0        0     1101 2022-08-01 03:07:06.926693 xrpl_py-2.1.0b0/xrpl/models/transactions/check_cancel.py
--rw-r--r--   0        0        0     1993 2022-08-01 03:07:06.926771 xrpl_py-2.1.0b0/xrpl/models/transactions/check_cash.py
--rw-r--r--   0        0        0     1934 2022-08-01 03:07:06.926860 xrpl_py-2.1.0b0/xrpl/models/transactions/check_create.py
--rw-r--r--   0        0        0     1598 2022-08-01 03:07:06.926937 xrpl_py-2.1.0b0/xrpl/models/transactions/deposit_preauth.py
--rw-r--r--   0        0        0     1072 2023-07-10 16:48:55.583461 xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_cancel.py
--rw-r--r--   0        0        0     2751 2023-07-10 16:48:55.583638 xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_create.py
--rw-r--r--   0        0        0     2114 2022-08-01 03:07:06.927180 xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_finish.py
--rw-r--r--   0        0        0     3163 2023-05-23 16:51:49.269564 xrpl_py-2.1.0b0/xrpl/models/transactions/metadata.py
--rw-r--r--   0        0        0     4537 2022-08-01 03:07:06.927331 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_accept_offer.py
--rw-r--r--   0        0        0     1769 2022-08-01 03:07:06.927408 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_burn.py
--rw-r--r--   0        0        0     2015 2022-08-01 03:07:06.927486 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_cancel_offer.py
--rw-r--r--   0        0        0     4324 2022-08-01 03:07:06.927560 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_create_offer.py
--rw-r--r--   0        0        0     4762 2022-08-09 19:51:34.686117 xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_mint.py
--rw-r--r--   0        0        0     1045 2022-08-01 03:07:06.927715 xrpl_py-2.1.0b0/xrpl/models/transactions/offer_cancel.py
--rw-r--r--   0        0        0     3866 2022-08-01 03:07:06.927795 xrpl_py-2.1.0b0/xrpl/models/transactions/offer_create.py
--rw-r--r--   0        0        0     5861 2022-08-01 03:07:06.927880 xrpl_py-2.1.0b0/xrpl/models/transactions/payment.py
--rw-r--r--   0        0        0     4227 2023-07-10 16:48:55.583810 xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_claim.py
--rw-r--r--   0        0        0     2569 2023-07-10 16:48:55.583967 xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_create.py
--rw-r--r--   0        0        0     1660 2023-07-10 16:48:55.584128 xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_fund.py
--rw-r--r--   0        0        0      575 2022-08-01 03:07:06.928228 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py
--rw-r--r--   0        0        0     3651 2022-08-01 03:07:06.928326 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py
--rw-r--r--   0        0        0     1366 2022-08-01 03:07:06.928402 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py
--rw-r--r--   0        0        0     1874 2022-08-01 03:07:06.928467 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py
--rw-r--r--   0        0        0     2262 2022-08-01 03:07:06.928526 xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.928554 xrpl_py-2.1.0b0/xrpl/models/transactions/py.typed
--rw-r--r--   0        0        0      959 2022-08-01 03:07:06.928643 xrpl_py-2.1.0b0/xrpl/models/transactions/set_regular_key.py
--rw-r--r--   0        0        0     5113 2023-06-07 18:37:48.861498 xrpl_py-2.1.0b0/xrpl/models/transactions/signer_list_set.py
--rw-r--r--   0        0        0      959 2022-08-01 03:07:06.928817 xrpl_py-2.1.0b0/xrpl/models/transactions/ticket_create.py
--rw-r--r--   0        0        0    15955 2023-07-10 17:12:46.173127 xrpl_py-2.1.0b0/xrpl/models/transactions/transaction.py
--rw-r--r--   0        0        0     2425 2022-08-01 03:07:06.929079 xrpl_py-2.1.0b0/xrpl/models/transactions/trust_set.py
--rw-r--r--   0        0        0      275 2022-08-01 03:07:06.929186 xrpl_py-2.1.0b0/xrpl/models/transactions/types/__init__.py
--rw-r--r--   0        0        0      287 2022-08-01 03:07:06.929265 xrpl_py-2.1.0b0/xrpl/models/transactions/types/pseudo_transaction_type.py
--rw-r--r--   0        0        0     1631 2023-07-10 16:48:55.584619 xrpl_py-2.1.0b0/xrpl/models/transactions/types/transaction_type.py
--rw-r--r--   0        0        0     2236 2023-07-10 16:48:55.584718 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_account_create_commit.py
--rw-r--r--   0        0        0     3283 2023-07-10 16:48:55.584824 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_add_account_create_attestation.py
--rw-r--r--   0        0        0     3011 2023-07-10 16:48:55.584928 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_add_claim_attestation.py
--rw-r--r--   0        0        0     2690 2023-07-10 16:48:55.585019 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_claim.py
--rw-r--r--   0        0        0     2235 2023-07-10 16:48:55.585114 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_commit.py
--rw-r--r--   0        0        0     3225 2023-07-10 16:48:55.585229 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_create_bridge.py
--rw-r--r--   0        0        0     2169 2023-07-10 16:48:55.585329 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_create_claim_id.py
--rw-r--r--   0        0        0     3388 2023-07-10 16:48:55.585409 xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_modify_bridge.py
--rw-r--r--   0        0        0      749 2022-08-01 03:07:06.929418 xrpl_py-2.1.0b0/xrpl/models/types.py
--rw-r--r--   0        0        0     2196 2023-05-23 16:51:49.272002 xrpl_py-2.1.0b0/xrpl/models/utils.py
--rw-r--r--   0        0        0     1097 2023-07-10 16:48:55.585500 xrpl_py-2.1.0b0/xrpl/models/xchain_bridge.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.929533 xrpl_py-2.1.0b0/xrpl/py.typed
--rw-r--r--   0        0        0      645 2023-07-10 17:12:46.173358 xrpl_py-2.1.0b0/xrpl/transaction/__init__.py
--rw-r--r--   0        0        0     3614 2023-07-10 17:12:46.173633 xrpl_py-2.1.0b0/xrpl/transaction/main.py
--rw-r--r--   0        0        0     1216 2023-07-10 17:12:46.173829 xrpl_py-2.1.0b0/xrpl/transaction/multisign.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.929779 xrpl_py-2.1.0b0/xrpl/transaction/py.typed
--rw-r--r--   0        0        0     2092 2023-07-10 17:12:46.174053 xrpl_py-2.1.0b0/xrpl/transaction/reliable_submission.py
--rw-r--r--   0        0        0      839 2023-05-23 16:51:49.273697 xrpl_py-2.1.0b0/xrpl/utils/__init__.py
--rw-r--r--   0        0        0     4220 2023-05-23 16:51:49.273844 xrpl_py-2.1.0b0/xrpl/utils/get_nftoken_id.py
--rw-r--r--   0        0        0     3412 2022-08-01 03:07:06.930042 xrpl_py-2.1.0b0/xrpl/utils/parse_nftoken_id.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.930069 xrpl_py-2.1.0b0/xrpl/utils/py.typed
--rw-r--r--   0        0        0      788 2022-08-01 03:07:06.930218 xrpl_py-2.1.0b0/xrpl/utils/str_conversions.py
--rw-r--r--   0        0        0     4202 2022-08-01 03:07:06.930296 xrpl_py-2.1.0b0/xrpl/utils/time_conversions.py
--rw-r--r--   0        0        0      350 2022-08-01 03:07:06.930405 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/__init__.py
--rw-r--r--   0        0        0     1717 2022-08-01 03:07:06.930477 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_balance_changes.py
--rw-r--r--   0        0        0     1446 2022-08-01 03:07:06.930538 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_final_balances.py
--rw-r--r--   0        0        0      641 2022-08-01 03:07:06.930603 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_order_book_changes.py
--rw-r--r--   0        0        0      627 2022-08-01 03:07:06.930692 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/__init__.py
--rw-r--r--   0        0        0     5218 2022-08-01 03:07:06.930789 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/balance_parser.py
--rw-r--r--   0        0        0     2518 2023-01-09 23:03:27.494325 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/nodes.py
--rw-r--r--   0        0        0     6191 2022-08-01 03:07:06.930936 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py
--rw-r--r--   0        0        0     1192 2022-08-01 03:07:06.931006 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/parser.py
--rw-r--r--   0        0        0     1404 2023-01-09 23:03:27.494567 xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/types.py
--rw-r--r--   0        0        0     3476 2022-08-01 03:07:06.931171 xrpl_py-2.1.0b0/xrpl/utils/xrp_conversions.py
--rw-r--r--   0        0        0      269 2022-08-01 03:07:06.931262 xrpl_py-2.1.0b0/xrpl/wallet/__init__.py
--rw-r--r--   0        0        0     9439 2023-07-10 17:12:46.174332 xrpl_py-2.1.0b0/xrpl/wallet/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.931385 xrpl_py-2.1.0b0/xrpl/wallet/py.typed
--rw-r--r--   0        0        0     1639 2023-07-10 17:12:46.174580 xrpl_py-2.1.0b0/xrpl/wallet/wallet_generation.py
--rw-r--r--   0        0        0    17291 1970-01-01 00:00:00.000000 xrpl_py-2.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0      740 2023-03-27 21:33:33.181289 xrpl_py-2.2.0/LICENSE
+-rw-r--r--   0        0        0    16775 2023-07-14 21:45:44.277760 xrpl_py-2.2.0/README.md
+-rw-r--r--   0        0        0     2227 2023-08-07 21:41:49.147712 xrpl_py-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-03-27 21:33:33.208293 xrpl_py-2.2.0/xrpl/__init__.py
+-rw-r--r--   0        0        0      393 2023-07-05 18:29:25.258425 xrpl_py-2.2.0/xrpl/account/__init__.py
+-rw-r--r--   0        0        0     3376 2023-07-05 18:29:25.259003 xrpl_py-2.2.0/xrpl/account/main.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.208607 xrpl_py-2.2.0/xrpl/account/py.typed
+-rw-r--r--   0        0        0      776 2023-07-05 18:29:25.259418 xrpl_py-2.2.0/xrpl/account/transaction_history.py
+-rw-r--r--   0        0        0      189 2023-03-27 21:33:33.208996 xrpl_py-2.2.0/xrpl/asyncio/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-05 18:29:25.259832 xrpl_py-2.2.0/xrpl/asyncio/account/__init__.py
+-rw-r--r--   0        0        0     4245 2023-07-05 18:29:25.260231 xrpl_py-2.2.0/xrpl/asyncio/account/main.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.209363 xrpl_py-2.2.0/xrpl/asyncio/account/py.typed
+-rw-r--r--   0        0        0     1170 2023-07-05 18:29:25.260699 xrpl_py-2.2.0/xrpl/asyncio/account/transaction_history.py
+-rw-r--r--   0        0        0      705 2023-03-27 21:33:33.209657 xrpl_py-2.2.0/xrpl/asyncio/clients/__init__.py
+-rw-r--r--   0        0        0      692 2023-03-27 21:33:33.209787 xrpl_py-2.2.0/xrpl/asyncio/clients/async_client.py
+-rw-r--r--   0        0        0      315 2023-03-27 21:33:33.209890 xrpl_py-2.2.0/xrpl/asyncio/clients/async_json_rpc_client.py
+-rw-r--r--   0        0        0     7149 2023-05-24 00:47:49.625976 xrpl_py-2.2.0/xrpl/asyncio/clients/async_websocket_client.py
+-rw-r--r--   0        0        0     1189 2023-06-28 21:24:17.291182 xrpl_py-2.2.0/xrpl/asyncio/clients/client.py
+-rw-r--r--   0        0        0     1083 2023-03-27 21:33:33.210270 xrpl_py-2.2.0/xrpl/asyncio/clients/exceptions.py
+-rw-r--r--   0        0        0     1612 2023-03-27 21:33:33.210375 xrpl_py-2.2.0/xrpl/asyncio/clients/json_rpc_base.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.210427 xrpl_py-2.2.0/xrpl/asyncio/clients/py.typed
+-rw-r--r--   0        0        0     3341 2023-03-27 21:33:33.210572 xrpl_py-2.2.0/xrpl/asyncio/clients/utils.py
+-rw-r--r--   0        0        0     8173 2023-05-24 00:47:49.626225 xrpl_py-2.2.0/xrpl/asyncio/clients/websocket_base.py
+-rw-r--r--   0        0        0      328 2023-03-27 21:33:33.210867 xrpl_py-2.2.0/xrpl/asyncio/ledger/__init__.py
+-rw-r--r--   0        0        0     3443 2023-03-27 21:33:33.210988 xrpl_py-2.2.0/xrpl/asyncio/ledger/main.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.211039 xrpl_py-2.2.0/xrpl/asyncio/ledger/py.typed
+-rw-r--r--   0        0        0     2353 2023-03-27 21:33:33.211142 xrpl_py-2.2.0/xrpl/asyncio/ledger/utils.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.211201 xrpl_py-2.2.0/xrpl/asyncio/py.typed
+-rw-r--r--   0        0        0      569 2023-07-05 18:29:25.261267 xrpl_py-2.2.0/xrpl/asyncio/transaction/__init__.py
+-rw-r--r--   0        0        0    17821 2023-07-05 18:29:25.261786 xrpl_py-2.2.0/xrpl/asyncio/transaction/main.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.211640 xrpl_py-2.2.0/xrpl/asyncio/transaction/py.typed
+-rw-r--r--   0        0        0     8210 2023-07-05 18:29:25.262451 xrpl_py-2.2.0/xrpl/asyncio/transaction/reliable_submission.py
+-rw-r--r--   0        0        0      219 2023-03-27 21:33:33.211934 xrpl_py-2.2.0/xrpl/asyncio/wallet/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.211983 xrpl_py-2.2.0/xrpl/asyncio/wallet/py.typed
+-rw-r--r--   0        0        0     6614 2023-07-05 18:29:25.262915 xrpl_py-2.2.0/xrpl/asyncio/wallet/wallet_generation.py
+-rw-r--r--   0        0        0      656 2023-03-27 21:33:33.212260 xrpl_py-2.2.0/xrpl/clients/__init__.py
+-rw-r--r--   0        0        0      295 2023-03-27 21:33:33.212375 xrpl_py-2.2.0/xrpl/clients/json_rpc_client.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.212453 xrpl_py-2.2.0/xrpl/clients/py.typed
+-rw-r--r--   0        0        0      705 2023-03-27 21:33:33.212612 xrpl_py-2.2.0/xrpl/clients/sync_client.py
+-rw-r--r--   0        0        0     8893 2023-05-24 00:47:49.627983 xrpl_py-2.2.0/xrpl/clients/websocket_client.py
+-rw-r--r--   0        0        0     1414 2023-03-27 21:33:33.212831 xrpl_py-2.2.0/xrpl/constants.py
+-rw-r--r--   0        0        0      171 2023-03-27 21:33:33.213024 xrpl_py-2.2.0/xrpl/core/__init__.py
+-rw-r--r--   0        0        0     1131 2023-07-05 18:29:25.263144 xrpl_py-2.2.0/xrpl/core/addresscodec/__init__.py
+-rw-r--r--   0        0        0     7175 2023-03-27 21:33:33.213364 xrpl_py-2.2.0/xrpl/core/addresscodec/codec.py
+-rw-r--r--   0        0        0      194 2023-03-27 21:33:33.213467 xrpl_py-2.2.0/xrpl/core/addresscodec/exceptions.py
+-rw-r--r--   0        0        0     5735 2023-07-05 18:29:25.263420 xrpl_py-2.2.0/xrpl/core/addresscodec/main.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.213616 xrpl_py-2.2.0/xrpl/core/addresscodec/py.typed
+-rw-r--r--   0        0        0      235 2023-03-27 21:33:33.213716 xrpl_py-2.2.0/xrpl/core/addresscodec/utils.py
+-rw-r--r--   0        0        0      488 2023-03-27 21:33:33.213863 xrpl_py-2.2.0/xrpl/core/binarycodec/__init__.py
+-rw-r--r--   0        0        0      296 2023-03-27 21:33:33.214024 xrpl_py-2.2.0/xrpl/core/binarycodec/binary_wrappers/__init__.py
+-rw-r--r--   0        0        0     9076 2023-03-27 21:33:33.214177 xrpl_py-2.2.0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py
+-rw-r--r--   0        0        0     4650 2023-03-27 21:33:33.214314 xrpl_py-2.2.0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py
+-rw-r--r--   0        0        0     1025 2023-03-27 21:33:33.214520 xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/__init__.py
+-rw-r--r--   0        0        0    45289 2023-08-07 21:24:31.153224 xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/definitions.json
+-rw-r--r--   0        0        0     8431 2023-03-27 21:33:33.214831 xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/definitions.py
+-rw-r--r--   0        0        0     1870 2023-06-13 17:18:50.605201 xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/field_header.py
+-rw-r--r--   0        0        0     1192 2023-03-27 21:33:33.215066 xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/field_info.py
+-rw-r--r--   0        0        0     1931 2023-03-27 21:33:33.215188 xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/field_instance.py
+-rw-r--r--   0        0        0      191 2023-03-27 21:33:33.215272 xrpl_py-2.2.0/xrpl/core/binarycodec/exceptions.py
+-rw-r--r--   0        0        0     3942 2023-03-27 21:33:33.215363 xrpl_py-2.2.0/xrpl/core/binarycodec/field_id_codec.py
+-rw-r--r--   0        0        0     3708 2023-06-13 17:18:50.605488 xrpl_py-2.2.0/xrpl/core/binarycodec/main.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.215490 xrpl_py-2.2.0/xrpl/core/binarycodec/py.typed
+-rw-r--r--   0        0        0     1255 2023-06-13 17:18:50.605779 xrpl_py-2.2.0/xrpl/core/binarycodec/types/__init__.py
+-rw-r--r--   0        0        0     2956 2023-03-27 21:33:33.215738 xrpl_py-2.2.0/xrpl/core/binarycodec/types/account_id.py
+-rw-r--r--   0        0        0    11513 2023-05-24 00:47:49.628328 xrpl_py-2.2.0/xrpl/core/binarycodec/types/amount.py
+-rw-r--r--   0        0        0     1950 2023-03-27 21:33:33.215995 xrpl_py-2.2.0/xrpl/core/binarycodec/types/blob.py
+-rw-r--r--   0        0        0     4347 2023-03-27 21:33:33.216127 xrpl_py-2.2.0/xrpl/core/binarycodec/types/currency.py
+-rw-r--r--   0        0        0     2640 2023-03-27 21:33:33.216255 xrpl_py-2.2.0/xrpl/core/binarycodec/types/hash.py
+-rw-r--r--   0        0        0     1494 2023-05-24 00:47:49.628558 xrpl_py-2.2.0/xrpl/core/binarycodec/types/hash128.py
+-rw-r--r--   0        0        0      571 2023-03-27 21:33:33.216531 xrpl_py-2.2.0/xrpl/core/binarycodec/types/hash160.py
+-rw-r--r--   0        0        0      572 2023-03-27 21:33:33.216629 xrpl_py-2.2.0/xrpl/core/binarycodec/types/hash256.py
+-rw-r--r--   0        0        0     9067 2023-03-27 21:33:33.216726 xrpl_py-2.2.0/xrpl/core/binarycodec/types/path_set.py
+-rw-r--r--   0        0        0     2493 2023-03-27 21:33:33.216814 xrpl_py-2.2.0/xrpl/core/binarycodec/types/serialized_type.py
+-rw-r--r--   0        0        0     3301 2023-03-27 21:33:33.216902 xrpl_py-2.2.0/xrpl/core/binarycodec/types/st_array.py
+-rw-r--r--   0        0        0     8392 2023-05-24 00:47:49.628841 xrpl_py-2.2.0/xrpl/core/binarycodec/types/st_object.py
+-rw-r--r--   0        0        0     3383 2023-03-27 21:33:33.217092 xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint.py
+-rw-r--r--   0        0        0     2063 2023-03-27 21:33:33.217191 xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint16.py
+-rw-r--r--   0        0        0     2283 2023-03-27 21:33:33.217268 xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint32.py
+-rw-r--r--   0        0        0     2854 2023-03-27 21:33:33.217357 xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint64.py
+-rw-r--r--   0        0        0     1994 2023-03-27 21:33:33.217433 xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint8.py
+-rw-r--r--   0        0        0     2905 2023-03-27 21:33:33.217534 xrpl_py-2.2.0/xrpl/core/binarycodec/types/vector256.py
+-rw-r--r--   0        0        0      447 2023-03-27 21:33:33.217683 xrpl_py-2.2.0/xrpl/core/keypairs/__init__.py
+-rw-r--r--   0        0        0     1275 2023-03-27 21:33:33.217784 xrpl_py-2.2.0/xrpl/core/keypairs/crypto_implementation.py
+-rw-r--r--   0        0        0     3662 2023-07-05 18:29:25.263845 xrpl_py-2.2.0/xrpl/core/keypairs/ed25519.py
+-rw-r--r--   0        0        0      182 2023-03-27 21:33:33.218030 xrpl_py-2.2.0/xrpl/core/keypairs/exceptions.py
+-rw-r--r--   0        0        0      893 2023-03-27 21:33:33.218146 xrpl_py-2.2.0/xrpl/core/keypairs/helpers.py
+-rw-r--r--   0        0        0     4881 2023-07-05 18:29:25.264355 xrpl_py-2.2.0/xrpl/core/keypairs/main.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.218330 xrpl_py-2.2.0/xrpl/core/keypairs/py.typed
+-rw-r--r--   0        0        0     7480 2023-03-27 21:33:33.218476 xrpl_py-2.2.0/xrpl/core/keypairs/secp256k1.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.218546 xrpl_py-2.2.0/xrpl/core/py.typed
+-rw-r--r--   0        0        0      314 2023-03-27 21:33:33.218727 xrpl_py-2.2.0/xrpl/ledger/__init__.py
+-rw-r--r--   0        0        0     2283 2023-03-27 21:33:33.218825 xrpl_py-2.2.0/xrpl/ledger/main.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.218878 xrpl_py-2.2.0/xrpl/ledger/py.typed
+-rw-r--r--   0        0        0      858 2023-06-13 17:18:50.606769 xrpl_py-2.2.0/xrpl/models/__init__.py
+-rw-r--r--   0        0        0      497 2023-03-27 21:33:33.219179 xrpl_py-2.2.0/xrpl/models/amounts/__init__.py
+-rw-r--r--   0        0        0     1377 2023-03-27 21:33:33.219264 xrpl_py-2.2.0/xrpl/models/amounts/amount.py
+-rw-r--r--   0        0        0     1349 2023-03-27 21:33:33.219368 xrpl_py-2.2.0/xrpl/models/amounts/issued_currency_amount.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.219418 xrpl_py-2.2.0/xrpl/models/amounts/py.typed
+-rw-r--r--   0        0        0    10682 2023-06-13 17:18:50.607347 xrpl_py-2.2.0/xrpl/models/base_model.py
+-rw-r--r--   0        0        0      371 2023-03-27 21:33:33.219720 xrpl_py-2.2.0/xrpl/models/currencies/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-20 18:04:32.828627 xrpl_py-2.2.0/xrpl/models/currencies/currency.py
+-rw-r--r--   0        0        0     2237 2023-03-27 21:33:33.219871 xrpl_py-2.2.0/xrpl/models/currencies/issued_currency.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.219913 xrpl_py-2.2.0/xrpl/models/currencies/py.typed
+-rw-r--r--   0        0        0     2716 2023-07-05 18:29:25.264811 xrpl_py-2.2.0/xrpl/models/currencies/xrp.py
+-rw-r--r--   0        0        0      171 2023-03-27 21:33:33.220096 xrpl_py-2.2.0/xrpl/models/exceptions.py
+-rw-r--r--   0        0        0     4126 2023-07-05 18:29:25.265065 xrpl_py-2.2.0/xrpl/models/flags.py
+-rw-r--r--   0        0        0     2462 2023-03-27 21:33:33.220298 xrpl_py-2.2.0/xrpl/models/nested_model.py
+-rw-r--r--   0        0        0     2088 2023-03-27 21:33:33.220387 xrpl_py-2.2.0/xrpl/models/path.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.220444 xrpl_py-2.2.0/xrpl/models/py.typed
+-rw-r--r--   0        0        0     3607 2023-06-13 17:18:50.607886 xrpl_py-2.2.0/xrpl/models/requests/__init__.py
+-rw-r--r--   0        0        0     1549 2023-06-28 21:24:17.296026 xrpl_py-2.2.0/xrpl/models/requests/account_channels.py
+-rw-r--r--   0        0        0     1134 2023-06-28 21:24:17.296337 xrpl_py-2.2.0/xrpl/models/requests/account_currencies.py
+-rw-r--r--   0        0        0     1088 2023-06-28 21:24:17.296558 xrpl_py-2.2.0/xrpl/models/requests/account_info.py
+-rw-r--r--   0        0        0     1323 2023-06-28 21:24:17.296815 xrpl_py-2.2.0/xrpl/models/requests/account_lines.py
+-rw-r--r--   0        0        0     1216 2023-06-28 21:24:17.297206 xrpl_py-2.2.0/xrpl/models/requests/account_nfts.py
+-rw-r--r--   0        0        0     1738 2023-06-28 21:24:17.297455 xrpl_py-2.2.0/xrpl/models/requests/account_objects.py
+-rw-r--r--   0        0        0     1161 2023-06-28 21:24:17.297683 xrpl_py-2.2.0/xrpl/models/requests/account_offers.py
+-rw-r--r--   0        0        0     1207 2023-06-28 21:24:17.297912 xrpl_py-2.2.0/xrpl/models/requests/account_tx.py
+-rw-r--r--   0        0        0     1024 2023-06-28 21:24:17.298185 xrpl_py-2.2.0/xrpl/models/requests/book_offers.py
+-rw-r--r--   0        0        0     3020 2023-06-13 17:18:50.608358 xrpl_py-2.2.0/xrpl/models/requests/channel_authorize.py
+-rw-r--r--   0        0        0     1130 2023-06-13 17:18:50.608584 xrpl_py-2.2.0/xrpl/models/requests/channel_verify.py
+-rw-r--r--   0        0        0     1145 2023-06-28 21:24:17.298415 xrpl_py-2.2.0/xrpl/models/requests/deposit_authorized.py
+-rw-r--r--   0        0        0      775 2023-03-27 21:33:33.222125 xrpl_py-2.2.0/xrpl/models/requests/fee.py
+-rw-r--r--   0        0        0     1076 2023-06-28 21:24:17.298642 xrpl_py-2.2.0/xrpl/models/requests/gateway_balances.py
+-rw-r--r--   0        0        0     3068 2023-03-27 21:33:33.222393 xrpl_py-2.2.0/xrpl/models/requests/generic_request.py
+-rw-r--r--   0        0        0      887 2023-06-28 21:24:17.298934 xrpl_py-2.2.0/xrpl/models/requests/ledger.py
+-rw-r--r--   0        0        0      944 2023-03-27 21:33:33.222656 xrpl_py-2.2.0/xrpl/models/requests/ledger_closed.py
+-rw-r--r--   0        0        0      726 2023-03-27 21:33:33.222760 xrpl_py-2.2.0/xrpl/models/requests/ledger_current.py
+-rw-r--r--   0        0        0     1190 2023-06-28 21:24:17.299176 xrpl_py-2.2.0/xrpl/models/requests/ledger_data.py
+-rw-r--r--   0        0        0     5171 2023-06-28 21:24:17.299427 xrpl_py-2.2.0/xrpl/models/requests/ledger_entry.py
+-rw-r--r--   0        0        0      853 2023-03-27 21:33:33.223038 xrpl_py-2.2.0/xrpl/models/requests/manifest.py
+-rw-r--r--   0        0        0      809 2023-06-28 21:24:17.299678 xrpl_py-2.2.0/xrpl/models/requests/nft_buy_offers.py
+-rw-r--r--   0        0        0     1184 2023-06-28 21:24:17.299933 xrpl_py-2.2.0/xrpl/models/requests/nft_history.py
+-rw-r--r--   0        0        0      772 2023-06-28 21:24:17.300172 xrpl_py-2.2.0/xrpl/models/requests/nft_info.py
+-rw-r--r--   0        0        0      816 2023-06-28 21:24:17.300459 xrpl_py-2.2.0/xrpl/models/requests/nft_sell_offers.py
+-rw-r--r--   0        0        0     1446 2023-06-28 21:24:17.300713 xrpl_py-2.2.0/xrpl/models/requests/no_ripple_check.py
+-rw-r--r--   0        0        0     4347 2023-03-27 21:33:33.223485 xrpl_py-2.2.0/xrpl/models/requests/path_find.py
+-rw-r--r--   0        0        0      547 2023-03-27 21:33:33.223601 xrpl_py-2.2.0/xrpl/models/requests/ping.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.223670 xrpl_py-2.2.0/xrpl/models/requests/py.typed
+-rw-r--r--   0        0        0      579 2023-03-27 21:33:33.223830 xrpl_py-2.2.0/xrpl/models/requests/random.py
+-rw-r--r--   0        0        0     6234 2023-06-28 21:24:17.300971 xrpl_py-2.2.0/xrpl/models/requests/request.py
+-rw-r--r--   0        0        0     2280 2023-06-28 21:24:17.301222 xrpl_py-2.2.0/xrpl/models/requests/ripple_path_find.py
+-rw-r--r--   0        0        0      618 2023-03-27 21:33:33.224173 xrpl_py-2.2.0/xrpl/models/requests/server_info.py
+-rw-r--r--   0        0        0     1194 2023-03-27 21:33:33.224272 xrpl_py-2.2.0/xrpl/models/requests/server_state.py
+-rw-r--r--   0        0        0     4034 2023-03-27 21:33:33.224362 xrpl_py-2.2.0/xrpl/models/requests/sign.py
+-rw-r--r--   0        0        0     5062 2023-03-27 21:33:33.224471 xrpl_py-2.2.0/xrpl/models/requests/sign_and_submit.py
+-rw-r--r--   0        0        0     3274 2023-03-27 21:33:33.224567 xrpl_py-2.2.0/xrpl/models/requests/sign_for.py
+-rw-r--r--   0        0        0     3758 2023-03-27 21:33:33.224651 xrpl_py-2.2.0/xrpl/models/requests/submit.py
+-rw-r--r--   0        0        0     2478 2023-03-27 21:33:33.224732 xrpl_py-2.2.0/xrpl/models/requests/submit_multisigned.py
+-rw-r--r--   0        0        0     2842 2023-03-27 21:33:33.224803 xrpl_py-2.2.0/xrpl/models/requests/submit_only.py
+-rw-r--r--   0        0        0     2103 2023-03-27 21:33:33.224904 xrpl_py-2.2.0/xrpl/models/requests/subscribe.py
+-rw-r--r--   0        0        0     1200 2023-06-28 21:24:17.301450 xrpl_py-2.2.0/xrpl/models/requests/transaction_entry.py
+-rw-r--r--   0        0        0      817 2023-03-27 21:33:33.225166 xrpl_py-2.2.0/xrpl/models/requests/tx.py
+-rw-r--r--   0        0        0     1595 2023-03-27 21:33:33.225289 xrpl_py-2.2.0/xrpl/models/requests/unsubscribe.py
+-rw-r--r--   0        0        0      251 2023-03-27 21:33:33.225598 xrpl_py-2.2.0/xrpl/models/required.py
+-rw-r--r--   0        0        0     3617 2023-03-27 21:33:33.225707 xrpl_py-2.2.0/xrpl/models/response.py
+-rw-r--r--   0        0        0     3412 2023-08-07 21:24:31.153749 xrpl_py-2.2.0/xrpl/models/transactions/__init__.py
+-rw-r--r--   0        0        0     1333 2023-03-27 21:33:33.225958 xrpl_py-2.2.0/xrpl/models/transactions/account_delete.py
+-rw-r--r--   0        0        0     9787 2023-08-07 21:24:31.154236 xrpl_py-2.2.0/xrpl/models/transactions/account_set.py
+-rw-r--r--   0        0        0     1101 2023-03-27 21:33:33.226157 xrpl_py-2.2.0/xrpl/models/transactions/check_cancel.py
+-rw-r--r--   0        0        0     1993 2023-03-27 21:33:33.226245 xrpl_py-2.2.0/xrpl/models/transactions/check_cash.py
+-rw-r--r--   0        0        0     1934 2023-03-27 21:33:33.226387 xrpl_py-2.2.0/xrpl/models/transactions/check_create.py
+-rw-r--r--   0        0        0     1383 2023-08-07 21:24:31.154490 xrpl_py-2.2.0/xrpl/models/transactions/clawback.py
+-rw-r--r--   0        0        0     1598 2023-03-27 21:33:33.226509 xrpl_py-2.2.0/xrpl/models/transactions/deposit_preauth.py
+-rw-r--r--   0        0        0     1069 2023-06-13 17:18:50.609915 xrpl_py-2.2.0/xrpl/models/transactions/escrow_cancel.py
+-rw-r--r--   0        0        0     2617 2023-06-13 17:18:50.610202 xrpl_py-2.2.0/xrpl/models/transactions/escrow_create.py
+-rw-r--r--   0        0        0     2114 2023-03-27 21:33:33.226807 xrpl_py-2.2.0/xrpl/models/transactions/escrow_finish.py
+-rw-r--r--   0        0        0     3163 2023-05-24 00:47:49.631283 xrpl_py-2.2.0/xrpl/models/transactions/metadata.py
+-rw-r--r--   0        0        0     4537 2023-03-27 21:33:33.226988 xrpl_py-2.2.0/xrpl/models/transactions/nftoken_accept_offer.py
+-rw-r--r--   0        0        0     1769 2023-03-27 21:33:33.227079 xrpl_py-2.2.0/xrpl/models/transactions/nftoken_burn.py
+-rw-r--r--   0        0        0     2015 2023-03-27 21:33:33.227174 xrpl_py-2.2.0/xrpl/models/transactions/nftoken_cancel_offer.py
+-rw-r--r--   0        0        0     4324 2023-03-27 21:33:33.227282 xrpl_py-2.2.0/xrpl/models/transactions/nftoken_create_offer.py
+-rw-r--r--   0        0        0     4762 2023-03-27 21:33:33.227403 xrpl_py-2.2.0/xrpl/models/transactions/nftoken_mint.py
+-rw-r--r--   0        0        0     1045 2023-03-27 21:33:33.227515 xrpl_py-2.2.0/xrpl/models/transactions/offer_cancel.py
+-rw-r--r--   0        0        0     3866 2023-03-27 21:33:33.227812 xrpl_py-2.2.0/xrpl/models/transactions/offer_create.py
+-rw-r--r--   0        0        0     5861 2023-03-27 21:33:33.227972 xrpl_py-2.2.0/xrpl/models/transactions/payment.py
+-rw-r--r--   0        0        0     3917 2023-06-13 17:18:50.610472 xrpl_py-2.2.0/xrpl/models/transactions/payment_channel_claim.py
+-rw-r--r--   0        0        0     2367 2023-06-13 17:18:50.610721 xrpl_py-2.2.0/xrpl/models/transactions/payment_channel_create.py
+-rw-r--r--   0        0        0     1614 2023-06-13 17:18:50.610980 xrpl_py-2.2.0/xrpl/models/transactions/payment_channel_fund.py
+-rw-r--r--   0        0        0      575 2023-03-27 21:33:33.228483 xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/__init__.py
+-rw-r--r--   0        0        0     3651 2023-03-27 21:33:33.228597 xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py
+-rw-r--r--   0        0        0     1366 2023-03-27 21:33:33.228692 xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py
+-rw-r--r--   0        0        0     1874 2023-03-27 21:33:33.228789 xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/set_fee.py
+-rw-r--r--   0        0        0     2262 2023-03-27 21:33:33.228920 xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/unl_modify.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.228990 xrpl_py-2.2.0/xrpl/models/transactions/py.typed
+-rw-r--r--   0        0        0      959 2023-03-27 21:33:33.229144 xrpl_py-2.2.0/xrpl/models/transactions/set_regular_key.py
+-rw-r--r--   0        0        0     5113 2023-06-01 20:44:07.712202 xrpl_py-2.2.0/xrpl/models/transactions/signer_list_set.py
+-rw-r--r--   0        0        0      959 2023-03-27 21:33:33.229383 xrpl_py-2.2.0/xrpl/models/transactions/ticket_create.py
+-rw-r--r--   0        0        0    15851 2023-06-28 21:24:17.302588 xrpl_py-2.2.0/xrpl/models/transactions/transaction.py
+-rw-r--r--   0        0        0     2425 2023-03-27 21:33:33.229646 xrpl_py-2.2.0/xrpl/models/transactions/trust_set.py
+-rw-r--r--   0        0        0      275 2023-03-27 21:33:33.229800 xrpl_py-2.2.0/xrpl/models/transactions/types/__init__.py
+-rw-r--r--   0        0        0      287 2023-03-27 21:33:33.229903 xrpl_py-2.2.0/xrpl/models/transactions/types/pseudo_transaction_type.py
+-rw-r--r--   0        0        0     1095 2023-08-07 21:24:31.154804 xrpl_py-2.2.0/xrpl/models/transactions/types/transaction_type.py
+-rw-r--r--   0        0        0      749 2023-03-27 21:33:33.230152 xrpl_py-2.2.0/xrpl/models/types.py
+-rw-r--r--   0        0        0     2196 2023-05-24 00:47:49.631890 xrpl_py-2.2.0/xrpl/models/utils.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.230311 xrpl_py-2.2.0/xrpl/py.typed
+-rw-r--r--   0        0        0      645 2023-07-05 18:29:25.266122 xrpl_py-2.2.0/xrpl/transaction/__init__.py
+-rw-r--r--   0        0        0     3614 2023-07-05 18:29:25.266841 xrpl_py-2.2.0/xrpl/transaction/main.py
+-rw-r--r--   0        0        0     1216 2023-06-28 21:24:17.303445 xrpl_py-2.2.0/xrpl/transaction/multisign.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.230897 xrpl_py-2.2.0/xrpl/transaction/py.typed
+-rw-r--r--   0        0        0     2092 2023-07-05 18:29:25.267498 xrpl_py-2.2.0/xrpl/transaction/reliable_submission.py
+-rw-r--r--   0        0        0      839 2023-05-24 00:47:49.633295 xrpl_py-2.2.0/xrpl/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2023-05-24 00:47:49.633438 xrpl_py-2.2.0/xrpl/utils/get_nftoken_id.py
+-rw-r--r--   0        0        0     3412 2023-03-27 21:33:33.231476 xrpl_py-2.2.0/xrpl/utils/parse_nftoken_id.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.231524 xrpl_py-2.2.0/xrpl/utils/py.typed
+-rw-r--r--   0        0        0      788 2023-03-27 21:33:33.231728 xrpl_py-2.2.0/xrpl/utils/str_conversions.py
+-rw-r--r--   0        0        0     4202 2023-03-27 21:33:33.231821 xrpl_py-2.2.0/xrpl/utils/time_conversions.py
+-rw-r--r--   0        0        0      350 2023-03-27 21:33:33.231975 xrpl_py-2.2.0/xrpl/utils/txn_parser/__init__.py
+-rw-r--r--   0        0        0     1717 2023-03-27 21:33:33.232058 xrpl_py-2.2.0/xrpl/utils/txn_parser/get_balance_changes.py
+-rw-r--r--   0        0        0     1446 2023-03-27 21:33:33.232179 xrpl_py-2.2.0/xrpl/utils/txn_parser/get_final_balances.py
+-rw-r--r--   0        0        0      641 2023-06-20 18:02:15.682794 xrpl_py-2.2.0/xrpl/utils/txn_parser/get_order_book_changes.py
+-rw-r--r--   0        0        0      627 2023-03-27 21:33:33.232493 xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/__init__.py
+-rw-r--r--   0        0        0     5218 2023-03-27 21:33:33.232602 xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/balance_parser.py
+-rw-r--r--   0        0        0     2518 2023-03-27 21:33:33.232692 xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/nodes.py
+-rw-r--r--   0        0        0     6191 2023-03-27 21:33:33.232824 xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/order_book_parser.py
+-rw-r--r--   0        0        0     1192 2023-06-23 20:25:14.082758 xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/parser.py
+-rw-r--r--   0        0        0     1404 2023-03-27 21:33:33.233075 xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/types.py
+-rw-r--r--   0        0        0     3476 2023-06-23 20:12:58.674281 xrpl_py-2.2.0/xrpl/utils/xrp_conversions.py
+-rw-r--r--   0        0        0      269 2023-03-27 21:33:33.233321 xrpl_py-2.2.0/xrpl/wallet/__init__.py
+-rw-r--r--   0        0        0     9439 2023-07-10 21:05:14.575844 xrpl_py-2.2.0/xrpl/wallet/main.py
+-rw-r--r--   0        0        0        0 2023-03-27 21:33:33.233455 xrpl_py-2.2.0/xrpl/wallet/py.typed
+-rw-r--r--   0        0        0     1639 2023-06-28 21:24:17.304334 xrpl_py-2.2.0/xrpl/wallet/wallet_generation.py
+-rw-r--r--   0        0        0    18063 1970-01-01 00:00:00.000000 xrpl_py-2.2.0/PKG-INFO
```

### Comparing `xrpl_py-2.1.0b0/LICENSE` & `xrpl_py-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/README.md` & `xrpl_py-2.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 [![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)
 
 # xrpl-py
 
-A pure Python implementation for interacting with the XRP Ledger, the `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing, by providing native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.
+A pure Python implementation for interacting with the [XRP Ledger](https://xrpl.org/). 
 
+The `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing. It also provides native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.
 
+As an example, this is how you would use this library to send a payment on testnet:
 
 ```py
-# create a network client
+from xrpl.account import get_balance
 from xrpl.clients import JsonRpcClient
+from xrpl.models import Payment, Tx
+from xrpl.transaction import submit_and_wait
+from xrpl.wallet import generate_faucet_wallet
+
+# Create a client to connect to the test network
 client = JsonRpcClient("https://s.altnet.rippletest.net:51234")
 
-# create a wallet on the testnet
-from xrpl.wallet import generate_faucet_wallet
-test_wallet = generate_faucet_wallet(client)
-print(test_wallet)
-public_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56
-private_key: -HIDDEN-
-address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
-
-# look up account info
-from xrpl.models import AccountInfo
-acct_info = AccountInfo(
-    account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
-    ledger_index="current",
-    queue=True,
-    strict=True,
+# Create two wallets to send money between on the test network
+wallet1 = generate_faucet_wallet(client, debug=True)
+wallet2 = generate_faucet_wallet(client, debug=True)
+
+# Both balances should be zero since nothing has been sent yet
+print("Balances of wallets before Payment tx")
+print(get_balance(wallet1.address, client))
+print(get_balance(wallet2.address, client))
+
+# Create a Payment transaction from wallet1 to wallet2
+payment_tx = Payment(
+    account=wallet1.address,
+    amount="1000",
+    destination=wallet2.address,
 )
-response = client.request(acct_info)
-result = response.result
-import json
-print(json.dumps(result["account_data"], indent=4, sort_keys=True))
-# {
-#     "Account": "rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
-#     "Balance": "1000000000",
-#     "Flags": 0,
-#     "LedgerEntryType": "AccountRoot",
-#     "OwnerCount": 0,
-#     "PreviousTxnID": "73CD4A37537A992270AAC8472F6681F44E400CBDE04EC8983C34B519F56AB107",
-#     "PreviousTxnLgrSeq": 16233962,
-#     "Sequence": 16233962,
-#     "index": "FD66EC588B52712DCE74831DCB08B24157DC3198C29A0116AA64D310A58512D7"
-# }
+
+# Submit the payment to the network and wait to see a response
+#   Behind the scenes, this fills in fields which can be looked up automatically like the fee.
+#   It also signs the transaction with wallet1 to prove you own the account you're paying from.
+payment_response = submit_and_wait(payment_tx, client, wallet1)
+print("Transaction was submitted")
+
+# Create a "Tx" request to look up the transaction on the ledger
+tx_response = client.request(Tx(transaction=payment_response.result["hash"]))
+
+# Check whether the transaction was actually validated on ledger
+print("Validated:", tx_response.result["validated"])
+
+# Check balances after 1000 drops (.001 XRP) was sent from wallet1 to wallet2
+print("Balances of wallets after Payment tx:")
+print(get_balance(wallet1.address, client))
+print(get_balance(wallet2.address, client))
 ```
 
 [![Downloads](https://pepy.tech/badge/xrpl-py/month)](https://pepy.tech/project/xrpl-py/month)
 [![Contributors](https://img.shields.io/github/contributors/xpring-eng/xrpl-py.svg)](https://github.com/xpring-eng/xrpl-py/graphs/contributors)
 
 ## Installation and supported versions
 
@@ -316,14 +324,17 @@
         is_test_network=True,
     )
 )
 print(testnet_xaddress)
 # T7QDemmxnuN7a52A62nx2fxGPWcRahLCf3qaswfrsNW9Lps
 ```
 
+## Migrating
+
+If you're currently using `xrpl-py` version 1, you can use [this guide to migrate to v2](https://xrpl.org/blog/2023/xrpl-py-2.0-release.html).
 
 ## Contributing
 
 If you want to contribute to this project, see [CONTRIBUTING.md].
 
 ### Mailing Lists
```

### Comparing `xrpl_py-2.1.0b0/pyproject.toml` & `xrpl_py-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xrpl-py"
-version = "2.1.0b0"
+version = "2.2.0"
 description = "A complete Python library for interacting with the XRP ledger"
 readme = "README.md"
 repository = "https://github.com/XRPLF/xrpl-py"
 authors = [
   "Mayukha Vadari <mvadari@ripple.com>",
   "Greg Weisbrod <gweisbrod@ripple.com>",
   "Amie Corso <acorso@ripple.com>",
```

### Comparing `xrpl_py-2.1.0b0/xrpl/account/main.py` & `xrpl_py-2.2.0/xrpl/account/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/account/transaction_history.py` & `xrpl_py-2.2.0/xrpl/account/transaction_history.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/account/main.py` & `xrpl_py-2.2.0/xrpl/asyncio/account/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/account/transaction_history.py` & `xrpl_py-2.2.0/xrpl/asyncio/account/transaction_history.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/clients/__init__.py` & `xrpl_py-2.2.0/xrpl/asyncio/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_client.py` & `xrpl_py-2.2.0/xrpl/asyncio/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/clients/async_websocket_client.py` & `xrpl_py-2.2.0/xrpl/asyncio/clients/async_websocket_client.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/clients/client.py` & `xrpl_py-2.2.0/xrpl/asyncio/clients/client.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/clients/exceptions.py` & `xrpl_py-2.2.0/xrpl/asyncio/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/clients/json_rpc_base.py` & `xrpl_py-2.2.0/xrpl/asyncio/clients/json_rpc_base.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/clients/utils.py` & `xrpl_py-2.2.0/xrpl/asyncio/clients/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/clients/websocket_base.py` & `xrpl_py-2.2.0/xrpl/asyncio/clients/websocket_base.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/ledger/main.py` & `xrpl_py-2.2.0/xrpl/asyncio/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/ledger/utils.py` & `xrpl_py-2.2.0/xrpl/asyncio/ledger/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/transaction/__init__.py` & `xrpl_py-2.2.0/xrpl/asyncio/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/transaction/main.py` & `xrpl_py-2.2.0/xrpl/asyncio/transaction/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # accurate NetworkID field in every transaction to that chain to prevent replay attacks.
 # Mainnet and testnet are exceptions.
 # More context: https://github.com/XRPLF/rippled/pull/4370
 _RESTRICTED_NETWORKS = 1024
 _REQUIRED_NETWORKID_VERSION = "1.11.0"
 _HOOKS_TESTNET_ID = 21338
 # TODO: make this dynamic based on the current ledger fee
-_OWNER_RESERVE_FEE: Final[int] = int(xrp_to_drops(2))
+_ACCOUNT_DELETE_FEE: Final[int] = int(xrp_to_drops(2))
 
 
 async def sign_and_submit(
     transaction: Transaction,
     client: Client,
     wallet: Wallet,
     autofill: bool = True,
@@ -463,28 +463,25 @@
         escrow_finish = cast(EscrowFinish, transaction)
         if escrow_finish.fulfillment is not None:
             fulfillment_bytes = escrow_finish.fulfillment.encode("ascii")
             # 10 drops × (33 + (Fulfillment size in bytes / 16))
             base_fee = math.ceil(net_fee * (33 + (len(fulfillment_bytes) / 16)))
 
     # AccountDelete Transaction
-    if (
-        transaction.transaction_type == TransactionType.ACCOUNT_DELETE
-        or transaction.transaction_type == TransactionType.AMM_CREATE
-    ):
+    if transaction.transaction_type == TransactionType.ACCOUNT_DELETE:
         if client is None:
-            base_fee = _OWNER_RESERVE_FEE
+            base_fee = _ACCOUNT_DELETE_FEE
         else:
-            base_fee = await _fetch_owner_reserve_fee(client)
+            base_fee = await _fetch_account_delete_fee(client)
 
     # Multi-signed Transaction
     # 10 drops × (1 + Number of Signatures Provided)
     if signers_count is not None and signers_count > 0:
         base_fee += net_fee * (1 + signers_count)
     # Round Up base_fee and return it as a String
     return str(math.ceil(base_fee))
 
 
-async def _fetch_owner_reserve_fee(client: Client) -> int:
+async def _fetch_account_delete_fee(client: Client) -> int:
     server_state = await client._request_impl(ServerState())
     fee = server_state.result["state"]["validated_ledger"]["reserve_inc"]
     return int(fee)
```

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/transaction/reliable_submission.py` & `xrpl_py-2.2.0/xrpl/asyncio/transaction/reliable_submission.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/asyncio/wallet/wallet_generation.py` & `xrpl_py-2.2.0/xrpl/asyncio/wallet/wallet_generation.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/clients/__init__.py` & `xrpl_py-2.2.0/xrpl/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/clients/sync_client.py` & `xrpl_py-2.2.0/xrpl/clients/sync_client.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/clients/websocket_client.py` & `xrpl_py-2.2.0/xrpl/clients/websocket_client.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/constants.py` & `xrpl_py-2.2.0/xrpl/constants.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/addresscodec/__init__.py` & `xrpl_py-2.2.0/xrpl/core/addresscodec/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/addresscodec/codec.py` & `xrpl_py-2.2.0/xrpl/core/addresscodec/codec.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/addresscodec/main.py` & `xrpl_py-2.2.0/xrpl/core/addresscodec/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/__init__.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.json` & `xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/definitions.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9092113694512495%*

 * *Differences: {"'FIELDS'": '{delete: [260, 259, 258, 257, 256, 250, 240, 239, 238, 237, 236, 235, 234, 212, 211, '*

 * *             '210, 209, 208, 202, 201, 200, 199, 198, 197, 162, 161, 160, 159, 158, 157, 156, 155, '*

 * *             '154, 153, 152, 147, 146, 145, 117, 98, 97, 96, 78, 77, 76, 75, 24, 23, 18]}',*

 * * "'LEDGER_ENTRY_TYPES'": "{delete: ['Bridge', 'XChainClaimID', 'XChainCreateAccountClaimID', "*

 * *                         "'AMM']}",*

 * * "'TRANSACTION_RESULTS'": "{delete: ['temBAD_AMM_TOKENS', 'temEQUAL_DOOR_ACCOUNTS', "*

 * *  […]*

```diff
@@ -177,24 +177,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 18,
                 "type": "UInt8"
             }
         ],
         [
-            "WasLockingChainSend",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 19,
-                "type": "UInt8"
-            }
-        ],
-        [
             "LedgerEntryType",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "UInt16"
@@ -227,34 +217,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 4,
                 "type": "UInt16"
             }
         ],
         [
-            "TradingFee",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 5,
-                "type": "UInt16"
-            }
-        ],
-        [
-            "DiscountedFee",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 6,
-                "type": "UInt16"
-            }
-        ],
-        [
             "Version",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "UInt16"
@@ -747,54 +717,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 46,
                 "type": "UInt32"
             }
         ],
         [
-            "LockCount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 47,
-                "type": "UInt32"
-            }
-        ],
-        [
-            "VoteWeight",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 48,
-                "type": "UInt32"
-            }
-        ],
-        [
-            "FirstNFTokenSequence",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 50,
-                "type": "UInt32"
-            }
-        ],
-        [
-            "LockCount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 49,
-                "type": "UInt32"
-            }
-        ],
-        [
             "IndexNext",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "UInt64"
@@ -957,44 +887,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 19,
                 "type": "UInt64"
             }
         ],
         [
-            "XChainClaimID",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 20,
-                "type": "UInt64"
-            }
-        ],
-        [
-            "XChainAccountCreateCount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 21,
-                "type": "UInt64"
-            }
-        ],
-        [
-            "XChainAccountClaimCount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 22,
-                "type": "UInt64"
-            }
-        ],
-        [
             "EmailHash",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "Hash128"
@@ -1167,24 +1067,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 13,
                 "type": "Hash256"
             }
         ],
         [
-            "AMMID",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 14,
-                "type": "Hash256"
-            }
-        ],
-        [
             "BookDirectory",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "Hash256"
@@ -1447,44 +1337,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 10,
                 "type": "Amount"
             }
         ],
         [
-            "Amount2",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 11,
-                "type": "Amount"
-            }
-        ],
-        [
-            "BidMin",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 12,
-                "type": "Amount"
-            }
-        ],
-        [
-            "BidMax",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 13,
-                "type": "Amount"
-            }
-        ],
-        [
             "MinimumOffer",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "Amount"
@@ -1517,124 +1377,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 19,
                 "type": "Amount"
             }
         ],
         [
-            "LockedBalance",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 21,
-                "type": "Amount"
-            }
-        ],
-        [
-            "BaseFeeDrops",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 22,
-                "type": "Amount"
-            }
-        ],
-        [
-            "ReserveBaseDrops",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 23,
-                "type": "Amount"
-            }
-        ],
-        [
-            "ReserveIncrementDrops",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 24,
-                "type": "Amount"
-            }
-        ],
-        [
-            "LPTokenOut",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 25,
-                "type": "Amount"
-            }
-        ],
-        [
-            "LPTokenIn",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 26,
-                "type": "Amount"
-            }
-        ],
-        [
-            "EPrice",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 27,
-                "type": "Amount"
-            }
-        ],
-        [
-            "Price",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 28,
-                "type": "Amount"
-            }
-        ],
-        [
-            "SignatureReward",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 29,
-                "type": "Amount"
-            }
-        ],
-        [
-            "MinAccountCreateAmount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 30,
-                "type": "Amount"
-            }
-        ],
-        [
-            "LPTokenBalance",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 31,
-                "type": "Amount"
-            }
-        ],
-        [
             "PublicKey",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 1,
                 "type": "Blob"
@@ -1967,74 +1717,14 @@
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 16,
                 "type": "AccountID"
             }
         ],
         [
-            "OtherChainSource",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 18,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "OtherChainDestination",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 19,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "AttestationSignerAccount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 20,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "AttestationRewardAccount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 21,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "LockingChainDoor",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 22,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "IssuingChainDoor",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 23,
-                "type": "AccountID"
-            }
-        ],
-        [
             "Indexes",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 1,
                 "type": "Vector256"
@@ -2077,64 +1767,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "PathSet"
             }
         ],
         [
-            "LockingChainIssue",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 1,
-                "type": "Issue"
-            }
-        ],
-        [
-            "IssuingChainIssue",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 2,
-                "type": "Issue"
-            }
-        ],
-        [
-            "Asset",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 3,
-                "type": "Issue"
-            }
-        ],
-        [
-            "Asset2",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 4,
-                "type": "Issue"
-            }
-        ],
-        [
-            "XChainBridge",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 1,
-                "type": "XChainBridge"
-            }
-        ],
-        [
             "TransactionMetaData",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 2,
                 "type": "STObject"
@@ -2337,84 +1977,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 24,
                 "type": "STObject"
             }
         ],
         [
-            "VoteEntry",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 25,
-                "type": "STObject"
-            }
-        ],
-        [
-            "AuctionSlot",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 26,
-                "type": "STObject"
-            }
-        ],
-        [
-            "AuthAccount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 27,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainClaimProofSig",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 32,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainCreateAccountProofSig",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 33,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainClaimAttestationBatchElement",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 34,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainCreateAccountAttestationBatchElement",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 35,
-                "type": "STObject"
-            }
-        ],
-        [
             "Signers",
             {
                 "isSerialized": true,
                 "isSigningField": false,
                 "isVLEncoded": false,
                 "nth": 3,
                 "type": "STArray"
@@ -2497,24 +2067,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 11,
                 "type": "STArray"
             }
         ],
         [
-            "VoteSlots",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 12,
-                "type": "STArray"
-            }
-        ],
-        [
             "Majorities",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "STArray"
@@ -2555,72 +2115,20 @@
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 20,
                 "type": "STArray"
             }
-        ],
-        [
-            "XChainClaimAttestationBatch",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 21,
-                "type": "STArray"
-            }
-        ],
-        [
-            "XChainCreateAccountAttestationBatch",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 22,
-                "type": "STArray"
-            }
-        ],
-        [
-            "XChainClaimAttestations",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 23,
-                "type": "STArray"
-            }
-        ],
-        [
-            "XChainCreateAccountAttestations",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 24,
-                "type": "STArray"
-            }
-        ],
-        [
-            "AuthAccounts",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 25,
-                "type": "STArray"
-            }
         ]
     ],
     "LEDGER_ENTRY_TYPES": {
-        "AMM": 121,
         "AccountRoot": 97,
         "Amendments": 102,
         "Any": -3,
-        "Bridge": 105,
         "Check": 67,
         "Child": -2,
         "Contract": 99,
         "DepositPreauth": 112,
         "DirectoryNode": 100,
         "Escrow": 117,
         "FeeSettings": 115,
@@ -2631,23 +2139,17 @@
         "NFTokenPage": 80,
         "NegativeUNL": 78,
         "Nickname": 110,
         "Offer": 111,
         "PayChannel": 120,
         "RippleState": 114,
         "SignerList": 83,
-        "Ticket": 84,
-        "XChainClaimID": 113,
-        "XChainCreateAccountClaimID": 116
+        "Ticket": 84
     },
     "TRANSACTION_RESULTS": {
-        "tecAMM_BALANCE": 163,
-        "tecAMM_FAILED": 164,
-        "tecAMM_INVALID_TOKENS": 165,
-        "tecBAD_XCHAIN_TRANSFER_ISSUE": 171,
         "tecCANT_ACCEPT_OWN_NFTOKEN_OFFER": 158,
         "tecCLAIM": 100,
         "tecCRYPTOCONDITION_ERROR": 146,
         "tecDIR_FULL": 121,
         "tecDST_TAG_NEEDED": 143,
         "tecDUPLICATE": 149,
         "tecEXPIRED": 148,
@@ -2681,37 +2183,19 @@
         "tecNO_SUITABLE_NFTOKEN_PAGE": 155,
         "tecNO_TARGET": 138,
         "tecOBJECT_NOT_FOUND": 160,
         "tecOVERSIZE": 145,
         "tecOWNERS": 132,
         "tecPATH_DRY": 128,
         "tecPATH_PARTIAL": 101,
-        "tecPRECISION_LOSS": 188,
-        "tecREQUIRES_FLAG": 187,
         "tecTOO_SOON": 152,
         "tecUNFUNDED": 129,
         "tecUNFUNDED_ADD": 102,
-        "tecUNFUNDED_AMM": 162,
         "tecUNFUNDED_OFFER": 103,
         "tecUNFUNDED_PAYMENT": 104,
-        "tecXCHAIN_ACCOUNT_CREATE_PAST": 182,
-        "tecXCHAIN_ACCOUNT_CREATE_TOO_MANY": 183,
-        "tecXCHAIN_BAD_CLAIM_ID": 173,
-        "tecXCHAIN_BAD_PUBLIC_KEY_ACCOUNT_PAIR": 186,
-        "tecXCHAIN_CLAIM_NO_QUORUM": 174,
-        "tecXCHAIN_CREATE_ACCOUNT_NONXRP_ISSUE": 176,
-        "tecXCHAIN_INSUFF_CREATE_AMOUNT": 181,
-        "tecXCHAIN_NO_CLAIM_ID": 172,
-        "tecXCHAIN_NO_SIGNERS_LIST": 179,
-        "tecXCHAIN_PAYMENT_FAILED": 184,
-        "tecXCHAIN_PROOF_UNKNOWN_KEY": 175,
-        "tecXCHAIN_REWARD_MISMATCH": 178,
-        "tecXCHAIN_SELF_COMMIT": 185,
-        "tecXCHAIN_SENDING_ACCOUNT_MISMATCH": 180,
-        "tecXCHAIN_WRONG_CHAIN": 177,
         "tefALREADY": -198,
         "tefBAD_ADD_AUTH": -197,
         "tefBAD_AUTH": -196,
         "tefBAD_AUTH_MASTER": -183,
         "tefBAD_LEDGER": -195,
         "tefBAD_QUORUM": -185,
         "tefBAD_SIGNATURE": -186,
@@ -2741,15 +2225,14 @@
         "telFAILED_PROCESSING": -395,
         "telINSUF_FEE_P": -394,
         "telLOCAL_ERROR": -399,
         "telNETWORK_ID_MAKES_TX_NON_CANONICAL": -384,
         "telNO_DST_PARTIAL": -393,
         "telREQUIRES_NETWORK_ID": -385,
         "telWRONG_NETWORK": -386,
-        "temBAD_AMM_TOKENS": -261,
         "temBAD_AMOUNT": -298,
         "temBAD_CURRENCY": -297,
         "temBAD_EXPIRATION": -296,
         "temBAD_FEE": -295,
         "temBAD_ISSUER": -294,
         "temBAD_LIMIT": -293,
         "temBAD_NFTOKEN_TRANSFER_FEE": -262,
@@ -2766,61 +2249,49 @@
         "temBAD_SEQUENCE": -283,
         "temBAD_SIGNATURE": -282,
         "temBAD_SIGNER": -272,
         "temBAD_SRC_ACCOUNT": -281,
         "temBAD_TICK_SIZE": -269,
         "temBAD_TRANSFER_RATE": -280,
         "temBAD_WEIGHT": -270,
-        "temBAD_XCHAIN_PROOF": -258,
         "temCANNOT_PREAUTH_SELF": -267,
         "temDISABLED": -273,
         "temDST_IS_SRC": -279,
         "temDST_NEEDED": -278,
-        "temEQUAL_DOOR_ACCOUNTS": -259,
         "temINVALID": -277,
         "temINVALID_ACCOUNT_ID": -268,
         "temINVALID_COUNT": -266,
         "temINVALID_FLAG": -276,
         "temMALFORMED": -299,
         "temREDUNDANT": -275,
         "temRIPPLE_EMPTY": -274,
         "temSEQ_AND_TICKET": -263,
-        "temSIDECHAIN_BAD_ISSUES": -257,
-        "temSIDECHAIN_NONDOOR_OWNER": -256,
         "temUNCERTAIN": -265,
         "temUNKNOWN": -264,
-        "temXCHAIN_BRIDGE_BAD_MIN_ACCOUNT_CREATE_AMOUNT": -255,
-        "temXCHAIN_BRIDGE_BAD_REWARD_AMOUNT": -254,
-        "temXCHAIN_TOO_MANY_ATTESTATIONS": -253,
         "terFUNDS_SPENT": -98,
         "terINSUF_FEE_B": -97,
         "terLAST": -91,
         "terNO_ACCOUNT": -96,
-        "terNO_AMM": -87,
         "terNO_AUTH": -95,
         "terNO_LINE": -94,
         "terNO_RIPPLE": -90,
         "terOWNERS": -93,
         "terPRE_SEQ": -92,
         "terPRE_TICKET": -88,
         "terQUEUED": -89,
         "terRETRY": -99,
         "tesSUCCESS": 0
     },
     "TRANSACTION_TYPES": {
-        "AMMBid": 39,
-        "AMMCreate": 35,
-        "AMMDeposit": 36,
-        "AMMVote": 38,
-        "AMMWithdraw": 37,
         "AccountDelete": 21,
         "AccountSet": 3,
         "CheckCancel": 18,
         "CheckCash": 17,
         "CheckCreate": 16,
+        "Clawback": 30,
         "Contract": 9,
         "DepositPreauth": 19,
         "EnableAmendment": 100,
         "EscrowCancel": 4,
         "EscrowCreate": 1,
         "EscrowFinish": 2,
         "Invalid": -1,
@@ -2839,33 +2310,24 @@
         "SetFee": 101,
         "SetHook": 22,
         "SetRegularKey": 5,
         "SignerListSet": 12,
         "TicketCancel": 11,
         "TicketCreate": 10,
         "TrustSet": 20,
-        "UNLModify": 102,
-        "XChainAccountCreateCommit": 44,
-        "XChainAddAccountCreateAttestation": 46,
-        "XChainAddClaimAttestation": 45,
-        "XChainClaim": 43,
-        "XChainCommit": 42,
-        "XChainCreateBridge": 40,
-        "XChainCreateClaimID": 41,
-        "XChainModifyBridge": 47
+        "UNLModify": 102
     },
     "TYPES": {
         "AccountID": 8,
         "Amount": 6,
         "Blob": 7,
         "Done": -1,
         "Hash128": 4,
         "Hash160": 17,
         "Hash256": 5,
-        "Issue": 24,
         "LedgerEntry": 10002,
         "Metadata": 10004,
         "NotPresent": 0,
         "PathSet": 18,
         "STArray": 15,
         "STObject": 14,
         "Transaction": 10001,
@@ -2875,11 +2337,10 @@
         "UInt384": 22,
         "UInt512": 23,
         "UInt64": 3,
         "UInt8": 16,
         "UInt96": 20,
         "Unknown": -2,
         "Validation": 10003,
-        "Vector256": 19,
-        "XChainBridge": 25
+        "Vector256": 19
     }
 }
```

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/definitions.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/definitions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_header.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/field_header.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,11 +44,7 @@
                 header.append(self.field_code)
         elif self.field_code < 16:
             header += [self.field_code, self.type_code]
         else:
             header += [0, self.type_code, self.field_code]
 
         return bytes(header)
-
-    def __repr__(self: FieldHeader) -> str:
-        """Print a string representation of a FieldHeader (for debugging)."""
-        return f"FieldHeader({self.type_code}, {self.field_code})"
```

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_info.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/field_info.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/definitions/field_instance.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/definitions/field_instance.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/field_id_codec.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/field_id_codec.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/main.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Codec for encoding objects into the XRP Ledger's canonical binary format and
 decoding them.
 """
 
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, cast
 
 from typing_extensions import Final
 
 from xrpl.core.binarycodec.binary_wrappers.binary_parser import BinaryParser
 from xrpl.core.binarycodec.types.account_id import AccountID
-from xrpl.core.binarycodec.types.amount import Amount
 from xrpl.core.binarycodec.types.hash256 import Hash256
 from xrpl.core.binarycodec.types.st_object import STObject
 from xrpl.core.binarycodec.types.uint64 import UInt64
 
 
 def _num_to_bytes(num: int) -> bytes:
     return (num).to_bytes(4, byteorder="big", signed=False)
@@ -64,19 +63,15 @@
         json: A JSON-like dictionary representation of a Claim.
 
     Returns:
         The binary-encoded claim, ready to be signed.
     """
     prefix = _PAYMENT_CHANNEL_CLAIM_PREFIX
     channel = Hash256.from_value(json["channel"])
-
-    if isinstance(json["amount"], str):
-        amount: Union[Amount, UInt64] = UInt64.from_value(int(json["amount"]))
-    else:
-        amount = Amount.from_value(json["amount"])
+    amount = UInt64.from_value(int(json["amount"]))
 
     buffer = prefix + bytes(channel) + bytes(amount)
     return buffer.hex().upper()
 
 
 def encode_for_multisigning(json: Dict[str, Any], signing_account: str) -> str:
     """
```

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/__init__.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,36 @@
 from xrpl.core.binarycodec.types.amount import Amount
 from xrpl.core.binarycodec.types.blob import Blob
 from xrpl.core.binarycodec.types.currency import Currency
 from xrpl.core.binarycodec.types.hash import Hash
 from xrpl.core.binarycodec.types.hash128 import Hash128
 from xrpl.core.binarycodec.types.hash160 import Hash160
 from xrpl.core.binarycodec.types.hash256 import Hash256
-from xrpl.core.binarycodec.types.issue import Issue
 from xrpl.core.binarycodec.types.path_set import PathSet
 from xrpl.core.binarycodec.types.st_array import STArray
 from xrpl.core.binarycodec.types.st_object import STObject
 from xrpl.core.binarycodec.types.uint import UInt
 from xrpl.core.binarycodec.types.uint8 import UInt8
 from xrpl.core.binarycodec.types.uint16 import UInt16
 from xrpl.core.binarycodec.types.uint32 import UInt32
 from xrpl.core.binarycodec.types.uint64 import UInt64
 from xrpl.core.binarycodec.types.vector256 import Vector256
-from xrpl.core.binarycodec.types.xchain_bridge import XChainBridge
 
 __all__ = [
     "AccountID",
     "Amount",
     "Blob",
     "Currency",
     "Hash",
     "Hash128",
     "Hash160",
     "Hash256",
-    "Issue",
     "PathSet",
     "STObject",
     "STArray",
     "UInt",
     "UInt8",
     "UInt16",
     "UInt32",
     "UInt64",
     "Vector256",
-    "XChainBridge",
 ]
```

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/account_id.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/account_id.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/amount.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/amount.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/blob.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/blob.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/currency.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/currency.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/hash.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash128.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/hash128.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash160.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/hash160.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/hash256.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/hash256.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/issue.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/vector256.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,82 @@
-"""Codec for serializing and deserializing issued currency fields."""
-
+"""Codec for serializing and deserializing vectors of Hash256."""
 from __future__ import annotations
 
-from typing import Any, Dict, Optional, Type, Union
+from typing import List, Optional, Type
+
+from typing_extensions import Final
 
+from xrpl.core.binarycodec import XRPLBinaryCodecException
 from xrpl.core.binarycodec.binary_wrappers.binary_parser import BinaryParser
-from xrpl.core.binarycodec.exceptions import XRPLBinaryCodecException
-from xrpl.core.binarycodec.types.account_id import AccountID
-from xrpl.core.binarycodec.types.currency import Currency
+from xrpl.core.binarycodec.types.hash256 import Hash256
 from xrpl.core.binarycodec.types.serialized_type import SerializedType
-from xrpl.models.currencies import XRP as XRPModel
-from xrpl.models.currencies import IssuedCurrency as IssuedCurrencyModel
 
+_HASH_LENGTH_BYTES: Final[int] = 32
 
-class Issue(SerializedType):
-    """Codec for serializing and deserializing issued currency fields."""
 
-    def __init__(self: Issue, buffer: bytes) -> None:
-        """
-        Construct an Issue from given bytes.
+class Vector256(SerializedType):
+    """Codec for serializing and deserializing vectors of Hash256."""
 
-        Args:
-            buffer: The byte buffer that will be used to store the serialized
-                encoding of this field.
-        """
+    def __init__(self: Vector256, buffer: bytes) -> None:
+        """Construct a Vector256."""
         super().__init__(buffer)
 
     @classmethod
-    def from_value(cls: Type[Issue], value: Dict[str, str]) -> Issue:
-        """
-        Construct an Issue object from a string or dictionary representation
-        of an issued currency.
+    def from_value(cls: Type[Vector256], value: List[str]) -> Vector256:
+        """Construct a Vector256 from a list of strings.
 
         Args:
-            value: The dictionary to construct an Issue object from.
+            value: A list of hashes encoded as hex strings.
 
         Returns:
-            An Issue object constructed from value.
+            A Vector256 object representing these hashes.
 
         Raises:
-            XRPLBinaryCodecException: If the Issue representation is invalid.
+            XRPLBinaryCodecException: If the supplied value is of the wrong type.
         """
-        if XRPModel.is_dict_of_model(value):
-            currency_bytes = bytes(Currency.from_value(value["currency"]))
-            return cls(currency_bytes)
-
-        if IssuedCurrencyModel.is_dict_of_model(value):
-            currency_bytes = bytes(Currency.from_value(value["currency"]))
-            issuer_bytes = bytes(AccountID.from_value(value["issuer"]))
-            return cls(currency_bytes + issuer_bytes)
-
-        raise XRPLBinaryCodecException(
-            "Invalid type to construct an Issue: expected str or dict,"
-            f" received {value.__class__.__name__}."
-        )
+        if not isinstance(value, list):
+            raise XRPLBinaryCodecException(
+                "Invalid type to construct a Vector256: expected list,"
+                " received {value.__class__.__name__}."
+            )
+
+        byte_list = []
+        for string in value:
+            byte_list.append(bytes(Hash256.from_value(string)))
+        return cls(b"".join(byte_list))
 
     @classmethod
     def from_parser(
-        cls: Type[Issue],
-        parser: BinaryParser,
-        length_hint: Optional[int] = None,
-    ) -> Issue:
-        """
-        Construct an Issue object from an existing BinaryParser.
+        cls: Type[Vector256], parser: BinaryParser, length_hint: Optional[int] = None
+    ) -> SerializedType:
+        """Construct a Vector256 from a BinaryParser.
 
         Args:
-            parser: The parser to construct the Issue object from.
+            parser: The parser to construct a Vector256 from.
             length_hint: The number of bytes to consume from the parser.
 
         Returns:
-            The Issue object constructed from a parser.
+            A Vector256 object.
         """
-        currency = Currency.from_parser(parser)
-        if currency.to_json() == "XRP":
-            return cls(bytes(currency))
-
-        issuer = parser.read(20)  # the length in bytes of an account ID
-        return cls(bytes(currency) + issuer)
+        byte_list = []
+        num_bytes = length_hint if length_hint is not None else len(parser)
+        num_hashes = num_bytes // _HASH_LENGTH_BYTES
+        for i in range(num_hashes):
+            byte_list.append(bytes(Hash256.from_parser(parser)))
+        return cls(b"".join(byte_list))
 
-    def to_json(self: Issue) -> Union[str, Dict[Any, Any]]:
-        """
-        Returns the JSON representation of an issued currency.
+    def to_json(self: Vector256) -> List[str]:
+        """Return a list of hashes encoded as hex strings.
 
         Returns:
-            The JSON representation of an Issue.
-        """
-        parser = BinaryParser(str(self))
-        currency: Union[str, Dict[Any, Any]] = Currency.from_parser(parser).to_json()
-        if currency == "XRP":
-            return {"currency": currency}
+            The JSON representation of this Vector256.
 
-        issuer = AccountID.from_parser(parser)
-        return {"currency": currency, "issuer": issuer.to_json()}
+        Raises:
+            XRPLBinaryCodecException: If the number of bytes in the buffer
+                                        is not a multiple of the hash length.
+        """
+        if len(self.buffer) % _HASH_LENGTH_BYTES != 0:
+            raise XRPLBinaryCodecException("Invalid bytes for Vector256.")
+        hash_list = []
+        for i in range(0, len(self.buffer), _HASH_LENGTH_BYTES):
+            hash_list.append(self.buffer[i : i + _HASH_LENGTH_BYTES].hex().upper())
+        return hash_list
```

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/path_set.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/path_set.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/serialized_type.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/serialized_type.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_array.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/st_array.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/st_object.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/st_object.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint16.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint16.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint32.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint32.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint64.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint64.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/binarycodec/types/uint8.py` & `xrpl_py-2.2.0/xrpl/core/binarycodec/types/uint8.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/keypairs/crypto_implementation.py` & `xrpl_py-2.2.0/xrpl/core/keypairs/crypto_implementation.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/keypairs/ed25519.py` & `xrpl_py-2.2.0/xrpl/core/keypairs/ed25519.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/keypairs/helpers.py` & `xrpl_py-2.2.0/xrpl/core/keypairs/helpers.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/keypairs/main.py` & `xrpl_py-2.2.0/xrpl/core/keypairs/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/core/keypairs/secp256k1.py` & `xrpl_py-2.2.0/xrpl/core/keypairs/secp256k1.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/ledger/main.py` & `xrpl_py-2.2.0/xrpl/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/__init__.py` & `xrpl_py-2.2.0/xrpl/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """Top-level exports for the models package."""
 from xrpl.models import amounts, currencies, requests, transactions
 from xrpl.models.amounts import *  # noqa: F401, F403
-from xrpl.models.auth_account import AuthAccount
 from xrpl.models.currencies import *  # noqa: F401, F403
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.path import Path, PathStep
 from xrpl.models.requests import *  # noqa: F401, F403
 from xrpl.models.response import Response
 from xrpl.models.transactions import *  # noqa: F401, F403
 from xrpl.models.transactions.pseudo_transactions import *  # noqa: F401, F403
-from xrpl.models.xchain_bridge import XChainBridge
 
 __all__ = [
     "XRPLModelException",
     "amounts",
     *amounts.__all__,
-    "AuthAccount",
     "currencies",
     *currencies.__all__,
     "requests",
     *requests.__all__,
     "transactions",
     *transactions.__all__,
     *transactions.pseudo_transactions.__all__,
     "Path",
     "PathStep",
     "Response",
-    "XChainBridge",
 ]
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/amounts/amount.py` & `xrpl_py-2.2.0/xrpl/models/amounts/amount.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/amounts/issued_currency_amount.py` & `xrpl_py-2.2.0/xrpl/models/amounts/issued_currency_amount.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/base_model.py` & `xrpl_py-2.2.0/xrpl/models/base_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 import re
 from abc import ABC
 from dataclasses import dataclass, fields
 from enum import Enum
 from typing import Any, Dict, List, Pattern, Type, TypeVar, Union, cast, get_type_hints
 
-from typing_extensions import Final, Literal, get_args, get_origin
+from typing_extensions import Final, get_args, get_origin
 
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.required import REQUIRED
 from xrpl.models.types import XRPL_VALUE_TYPE
 
 # this regex splits words based on one of three cases:
 #
@@ -28,39 +28,29 @@
 # PascalCase like "Amount"
 _CAMEL_CASE_TYPICAL: Final[str] = "[A-Z][^A-Z]*"
 #
 # combining the above together into one regex:
 _CAMEL_TO_SNAKE_CASE_REGEX: Final[Pattern[str]] = re.compile(
     f"(?:{_CAMEL_CASE_LEADING_LOWER}|{_CAMEL_CASE_ABBREVIATION}|{_CAMEL_CASE_TYPICAL})"
 )
-
-# This is used to make exceptions when converting dictionary keys to xrpl JSON
-# keys. We snake case keys, but some keys are abbreviations.
-ABBREVIATIONS: Final[Dict[str, str]] = {
-    "amm": "AMM",
-    "id": "ID",
-    "lp": "LP",
-    "nftoken": "NFToken",
-    "unl": "UNL",
-    "uri": "URI",
-    "xchain": "XChain",
-}
+# used for converting special substrings inside CamelCase fields
+SPECIAL_CAMELCASE_STRINGS = ["NFToken"]
 
 BM = TypeVar("BM", bound="BaseModel")  # any type inherited from BaseModel
 
 
 def _key_to_json(field: str) -> str:
     """
     Transforms camelCase or PascalCase to snake_case. For example:
         1. 'TransactionType' becomes 'transaction_type'
         2. 'value' remains 'value'
         3. 'URI' becomes 'uri'
     """
     # convert all special CamelCase substrings to capitalized strings
-    for spec_str in ABBREVIATIONS.values():
+    for spec_str in SPECIAL_CAMELCASE_STRINGS:
         if spec_str in field:
             field = field.replace(spec_str, spec_str.capitalize())
 
     return "_".join(
         [word.lower() for word in _CAMEL_TO_SNAKE_CASE_REGEX.findall(field)]
     )
 
@@ -174,18 +164,14 @@
             # param_type is Any (e.g. will accept anything)
             return param_value
 
         if isinstance(param_type, type) and isinstance(param_value, param_type):
             # expected an object, received the correct object
             return param_value
 
-        if get_origin(param_type) == Literal:
-            if param_value in get_args(param_type):
-                return param_value
-
         if (
             isinstance(param_type, type)
             and issubclass(param_type, Enum)
             and param_value in list(param_type)
         ):
             # expected an Enum and received a valid value for it.
             # for some reason required for string enums.
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/currencies/issued_currency.py` & `xrpl_py-2.2.0/xrpl/models/currencies/issued_currency.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/currencies/xrp.py` & `xrpl_py-2.2.0/xrpl/models/currencies/xrp.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,7 @@
         """
         # import needed here to avoid circular dependency
         from xrpl.utils.xrp_conversions import xrp_to_drops
 
         if isinstance(value, str):
             return xrp_to_drops(float(value))
         return xrp_to_drops(value)
-
-    def __repr__(self: XRP) -> str:
-        """
-        Generate string representation of XRP.
-
-        Returns:
-            A string representation of XRP currency.
-        """
-        return "XRP()"
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/flags.py` & `xrpl_py-2.2.0/xrpl/models/flags.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,30 +13,14 @@
         "tf_require_dest_tag": 0x00010000,
         "tf_optional_dest_tag": 0x00020000,
         "tf_require_auth": 0x00040000,
         "tf_optional_auth": 0x00080000,
         "tf_disallow_xrp": 0x00100000,
         "tf_allow_xrp": 0x00200000,
     },
-    "AMMDeposit": {
-        "tf_lp_token": 0x00010000,
-        "tf_single_asset": 0x00080000,
-        "tf_two_asset": 0x00100000,
-        "tf_one_asset_lp_token": 0x00200000,
-        "tf_limit_lp_token": 0x00400000,
-    },
-    "AMMWithdraw": {
-        "tf_lp_token": 0x00010000,
-        "tf_withdraw_all": 0x00020000,
-        "tf_one_asset_withdraw_all": 0x00040000,
-        "tf_single_asset": 0x00080000,
-        "tf_two_asset": 0x00100000,
-        "tf_one_asset_lp_token": 0x00200000,
-        "tf_limit_lp_token": 0x00400000,
-    },
     "NFTokenCreateOffer": {
         "tf_sell_token": 0x00000001,
     },
     "NFTokenMint": {
         "tf_burnable": 0x00000001,
         "tf_only_xrp": 0x00000002,
         "tf_trustline": 0x00000004,
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/nested_model.py` & `xrpl_py-2.2.0/xrpl/models/nested_model.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/path.py` & `xrpl_py-2.2.0/xrpl/models/path.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/__init__.py` & `xrpl_py-2.2.0/xrpl/models/requests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Request models."""
-from xrpl.models.auth_account import AuthAccount
 from xrpl.models.path import PathStep
 from xrpl.models.requests.account_channels import AccountChannels
 from xrpl.models.requests.account_currencies import AccountCurrencies
 from xrpl.models.requests.account_info import AccountInfo
 from xrpl.models.requests.account_lines import AccountLines
 from xrpl.models.requests.account_nfts import AccountNFTs
 from xrpl.models.requests.account_objects import AccountObjects, AccountObjectType
 from xrpl.models.requests.account_offers import AccountOffers
 from xrpl.models.requests.account_tx import AccountTx
-from xrpl.models.requests.amm_info import AMMInfo
 from xrpl.models.requests.book_offers import BookOffers
 from xrpl.models.requests.channel_authorize import ChannelAuthorize
 from xrpl.models.requests.channel_verify import ChannelVerify
 from xrpl.models.requests.deposit_authorized import DepositAuthorized
 from xrpl.models.requests.fee import Fee
 from xrpl.models.requests.gateway_balances import GatewayBalances
 from xrpl.models.requests.generic_request import GenericRequest
@@ -52,16 +50,14 @@
     "AccountInfo",
     "AccountLines",
     "AccountNFTs",
     "AccountObjects",
     "AccountObjectType",
     "AccountOffers",
     "AccountTx",
-    "AMMInfo",
-    "AuthAccount",
     "BookOffers",
     "ChannelAuthorize",
     "ChannelVerify",
     "DepositAuthorized",
     "Fee",
     "GatewayBalances",
     "GenericRequest",
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/account_channels.py` & `xrpl_py-2.2.0/xrpl/models/requests/account_channels.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/account_currencies.py` & `xrpl_py-2.2.0/xrpl/models/requests/account_currencies.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/account_info.py` & `xrpl_py-2.2.0/xrpl/models/requests/account_info.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/account_lines.py` & `xrpl_py-2.2.0/xrpl/models/requests/account_lines.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/account_nfts.py` & `xrpl_py-2.2.0/xrpl/models/requests/account_nfts.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/account_objects.py` & `xrpl_py-2.2.0/xrpl/models/requests/account_objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,26 +14,23 @@
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 class AccountObjectType(str, Enum):
     """Represents the object types that an AccountObjectsRequest can ask for."""
 
-    BRIDGE = "bridge"
     CHECK = "check"
     DEPOSIT_PREAUTH = "deposit_preauth"
     ESCROW = "escrow"
-    NFT_OFFER = "nft_offer"
     OFFER = "offer"
     PAYMENT_CHANNEL = "payment_channel"
     SIGNER_LIST = "signer_list"
     STATE = "state"
     TICKET = "ticket"
-    XCHAIN_OWNED_CREATE_ACCOUNT_CLAIM_ID = "xchain_owned_create_account_claim_id"
-    XCHAIN_OWNED_CLAIM_ID = "xchain_owned_claim_id"
+    NFT_OFFER = "nft_offer"
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class AccountObjects(Request, LookupByLedgerRequest):
     """
     This request returns the raw ledger format for all objects owned by an account.
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/account_offers.py` & `xrpl_py-2.2.0/xrpl/models/requests/account_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/account_tx.py` & `xrpl_py-2.2.0/xrpl/models/requests/account_tx.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/amm_info.py` & `xrpl_py-2.2.0/xrpl/models/requests/manifest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-"""This request retrieves information about an AMM instance."""
-from __future__ import annotations
-
+"""
+The manifest method reports the current
+"manifest" information for a given validator
+public key. The "manifest" is the public portion
+of that validator's configured token.
+"""
 from dataclasses import dataclass, field
-from typing import Dict
 
-from xrpl.models.currencies import Currency
 from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AMMInfo(Request):
+class Manifest(Request):
     """
-    This request retrieves information about an AMM instance.
-
-    Must provide Asset and Asset2 params.
+    The manifest method reports the current
+    "manifest" information for a given validator
+    public key. The "manifest" is the public portion
+    of that validator's configured token.
     """
 
-    asset: Currency = REQUIRED  # type: ignore
-    """
-    Specifies one of the pool assets (XRP or token) of the AMM instance.
+    method: RequestMethod = field(default=RequestMethod.MANIFEST, init=False)
+    public_key: str = REQUIRED  # type: ignore
     """
+    This field is required.
 
-    asset2: Currency = REQUIRED  # type: ignore
+    :meta hide-value:
     """
-    Specifies the other pool asset of the AMM instance.
-    """
-
-    method: RequestMethod = field(default=RequestMethod.AMM_INFO, init=False)
-
-    def _get_errors(self: AMMInfo) -> Dict[str, str]:
-        errors = super()._get_errors()
-        return errors
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/book_offers.py` & `xrpl_py-2.2.0/xrpl/models/requests/book_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/channel_authorize.py` & `xrpl_py-2.2.0/xrpl/models/requests/channel_authorize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 The channel_authorize method creates a signature that can
-be used to redeem a specific amount from a payment channel.
+be used to redeem a specific amount of XRP from a payment channel.
 
 Warning: Do not send secret keys to untrusted servers or through unsecured network
 connections. (This includes the secret, seed, seed_hex, or passphrase fields of this
 request.) You should only use this method on a secure, encrypted network connection to
 a server you run or fully trust with your funds. Otherwise, eavesdroppers could use
 your secret key to sign claims and take all the money from this payment channel and
 anything else using the same key pair. See
@@ -14,26 +14,25 @@
 """
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, Optional
 
 from xrpl.constants import CryptoAlgorithm
-from xrpl.models.amounts import Amount
 from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class ChannelAuthorize(Request):
     """
     The channel_authorize method creates a signature that can
-    be used to redeem a specific amount from a payment channel.
+    be used to redeem a specific amount of XRP from a payment channel.
 
     Warning: Do not send secret keys to untrusted servers or through unsecured network
     connections. (This includes the secret, seed, seed_hex, or passphrase fields of
     this request.) You should only use this method on a secure, encrypted network
     connection to a server you run or fully trust with your funds. Otherwise,
     eavesdroppers could use your secret key to sign claims and take all the money from
     this payment channel and anything else using the same key pair. See
@@ -47,15 +46,15 @@
     channel_id: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    amount: Amount = REQUIRED  # type: ignore
+    amount: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
     secret: Optional[str] = None
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/channel_verify.py` & `xrpl_py-2.2.0/xrpl/models/requests/ledger_closed.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,37 @@
 """
-The channel_verify method checks the validity of a
-signature that can be used to redeem a specific amount
-from a payment channel.
+The ledger_closed method returns the unique
+identifiers of the most recently closed ledger.
+(This ledger is not necessarily validated and
+immutable yet.)
 """
 from dataclasses import dataclass, field
 
-from xrpl.models.amounts import Amount
 from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class ChannelVerify(Request):
+class LedgerClosed(Request):
     """
-    The channel_verify method checks the validity of a
-    signature that can be used to redeem a specific amount
-    from a payment channel.
+    The ledger_closed method returns the unique
+    identifiers of the most recently closed ledger.
+    (This ledger is not necessarily validated and
+    immutable yet.)
     """
 
-    method: RequestMethod = field(default=RequestMethod.CHANNEL_VERIFY, init=False)
-    channel_id: str = REQUIRED  # type: ignore
+    method: RequestMethod = field(default=RequestMethod.LEDGER_CLOSED, init=False)
+    ledger_hash: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
-    amount: Amount = REQUIRED  # type: ignore
-    """
-    This field is required.
-
-    :meta hide-value:
-    """
-
-    public_key: str = REQUIRED  # type: ignore
-    """
-    This field is required.
-
-    :meta hide-value:
-    """
-
-    signature: str = REQUIRED  # type: ignore
+    ledger_index: int = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/deposit_authorized.py` & `xrpl_py-2.2.0/xrpl/models/requests/deposit_authorized.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/fee.py` & `xrpl_py-2.2.0/xrpl/models/requests/fee.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/gateway_balances.py` & `xrpl_py-2.2.0/xrpl/models/requests/gateway_balances.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/generic_request.py` & `xrpl_py-2.2.0/xrpl/models/requests/generic_request.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/ledger.py` & `xrpl_py-2.2.0/xrpl/models/requests/ledger.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_closed.py` & `xrpl_py-2.2.0/xrpl/models/requests/nft_info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 """
-The ledger_closed method returns the unique
-identifiers of the most recently closed ledger.
-(This ledger is not necessarily validated and
-immutable yet.)
+The `nft_info` method retrieves all the information about the
+NFToken
 """
 from dataclasses import dataclass, field
 
-from xrpl.models.requests.request import Request, RequestMethod
+from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class LedgerClosed(Request):
+class NFTInfo(Request, LookupByLedgerRequest):
     """
-    The ledger_closed method returns the unique
-    identifiers of the most recently closed ledger.
-    (This ledger is not necessarily validated and
-    immutable yet.)
+    The `nft_info` method retrieves all the information about the
+    NFToken
     """
 
-    method: RequestMethod = field(default=RequestMethod.LEDGER_CLOSED, init=False)
-    ledger_hash: str = REQUIRED  # type: ignore
+    method: RequestMethod = field(default=RequestMethod.NFT_INFO, init=False)
+    nft_id: str = REQUIRED  # type: ignore
     """
-    This field is required.
-
-    :meta hide-value:
-    """
-
-    ledger_index: int = REQUIRED  # type: ignore
-    """
-    This field is required.
+    The unique identifier of an NFToken.
+    The request returns information of this NFToken. This value is required.
 
     :meta hide-value:
     """
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_current.py` & `xrpl_py-2.2.0/xrpl/models/requests/ledger_current.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_data.py` & `xrpl_py-2.2.0/xrpl/models/requests/ledger_data.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/ledger_entry.py` & `xrpl_py-2.2.0/xrpl/models/requests/ledger_entry.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 from xrpl.models.base_model import BaseModel
-from xrpl.models.currencies import Currency
 from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 class LedgerEntryType(str, Enum):
     """Identifiers for on-ledger objects."""
@@ -129,15 +128,15 @@
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class RippleState(BaseModel):
-    """Required fields for requesting a RippleState if not querying by object ID."""
+    """Required fields for requesting a RippleState."""
 
     accounts: List[str] = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
@@ -149,15 +148,18 @@
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class Ticket(BaseModel):
-    """Required fields for requesting a Ticket if not querying by object ID."""
+    """
+    Required fields for requesting a Ticket, if not querying by
+    object ID.
+    """
 
     owner: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
@@ -168,41 +170,14 @@
 
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class XChainClaimID(BaseModel):
-    """Required fields for requesting an XChainClaimID if not querying by object ID."""
-
-    locking_chain_door: str
-    locking_chain_issue: Currency
-    issuing_chain_door: str
-    issuing_chain_issue: Currency
-    xchain_claim_id: Union[int, str]
-
-
-@require_kwargs_on_init
-@dataclass(frozen=True)
-class XChainCreateAccountClaimID(BaseModel):
-    """
-    Required fields for requesting an XChainCreateAccountClaimID if not querying by
-    object ID.
-    """
-
-    locking_chain_door: str
-    locking_chain_issue: Currency
-    issuing_chain_door: str
-    issuing_chain_issue: Currency
-    xchain_create_account_claim_id: Union[int, str]
-
-
-@require_kwargs_on_init
-@dataclass(frozen=True)
 class LedgerEntry(Request, LookupByLedgerRequest):
     """
     The ledger_entry method returns a single ledger
     object from the XRP Ledger in its raw format.
     See ledger format for information on the
     different types of objects you can retrieve.
     `See ledger entry <https://xrpl.org/ledger_entry.html>`_
@@ -215,20 +190,14 @@
     deposit_preauth: Optional[Union[str, DepositPreauth]] = None
     directory: Optional[Union[str, Directory]] = None
     escrow: Optional[Union[str, Escrow]] = None
     offer: Optional[Union[str, Offer]] = None
     payment_channel: Optional[str] = None
     ripple_state: Optional[RippleState] = None
     ticket: Optional[Union[str, Ticket]] = None
-    bridge_account: Optional[str] = None
-    xchain_claim_id: Optional[Union[str, XChainClaimID]] = None
-    xchain_create_account_claim_id: Optional[
-        Union[str, XChainCreateAccountClaimID]
-    ] = None
-
     binary: bool = False
     nft_page: Optional[str] = None
     """Must be the object ID of the NFToken page, as hexadecimal"""
 
     def _get_errors(self: LedgerEntry) -> Dict[str, str]:
         errors = super()._get_errors()
         query_params = [
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/nft_buy_offers.py` & `xrpl_py-2.2.0/xrpl/models/requests/nft_buy_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/nft_history.py` & `xrpl_py-2.2.0/xrpl/models/requests/nft_history.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/nft_sell_offers.py` & `xrpl_py-2.2.0/xrpl/models/requests/nft_sell_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/no_ripple_check.py` & `xrpl_py-2.2.0/xrpl/models/requests/no_ripple_check.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/path_find.py` & `xrpl_py-2.2.0/xrpl/models/requests/path_find.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/ping.py` & `xrpl_py-2.2.0/xrpl/models/requests/ping.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/random.py` & `xrpl_py-2.2.0/xrpl/models/requests/random.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/request.py` & `xrpl_py-2.2.0/xrpl/models/requests/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,14 @@
     SERVER_INFO = "server_info"
     SERVER_STATE = "server_state"
 
     # utility methods
     PING = "ping"
     RANDOM = "random"
 
-    # amm methods
-    AMM_INFO = "amm_info"
-
     # generic unknown/unsupported request
     # (there is no XRPL analog, this model is specific to xrpl-py)
     GENERIC_REQUEST = "zzgeneric_request"
 
 
 R = TypeVar("R", bound="Request")
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/ripple_path_find.py` & `xrpl_py-2.2.0/xrpl/models/requests/ripple_path_find.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/server_info.py` & `xrpl_py-2.2.0/xrpl/models/requests/server_info.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/server_state.py` & `xrpl_py-2.2.0/xrpl/models/requests/server_state.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/sign.py` & `xrpl_py-2.2.0/xrpl/models/requests/sign.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/sign_and_submit.py` & `xrpl_py-2.2.0/xrpl/models/requests/sign_and_submit.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/sign_for.py` & `xrpl_py-2.2.0/xrpl/models/requests/sign_for.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/submit.py` & `xrpl_py-2.2.0/xrpl/models/requests/submit.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/submit_multisigned.py` & `xrpl_py-2.2.0/xrpl/models/requests/submit_multisigned.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/submit_only.py` & `xrpl_py-2.2.0/xrpl/models/requests/submit_only.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/subscribe.py` & `xrpl_py-2.2.0/xrpl/models/requests/subscribe.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/transaction_entry.py` & `xrpl_py-2.2.0/xrpl/models/requests/transaction_entry.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/tx.py` & `xrpl_py-2.2.0/xrpl/models/requests/tx.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/requests/unsubscribe.py` & `xrpl_py-2.2.0/xrpl/models/requests/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/response.py` & `xrpl_py-2.2.0/xrpl/models/response.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/account_delete.py` & `xrpl_py-2.2.0/xrpl/models/transactions/account_delete.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/account_set.py` & `xrpl_py-2.2.0/xrpl/models/transactions/account_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,17 @@
 
     ASF_DISABLE_INCOMING_PAYCHAN = 14
     """Disallow other accounts from creating PayChannels directed at this account."""
 
     ASF_DISABLE_INCOMING_TRUSTLINE = 15
     """Disallow other accounts from creating Trustlines directed at this account."""
 
+    ASF_ALLOW_TRUSTLINE_CLAWBACK = 16
+    """Allow trustline clawback feature"""
+
 
 class AccountSetFlag(int, Enum):
     """
     Enum for AccountSet Transaction Flags.
 
     Transactions of the AccountSet type support additional values in the Flags field.
     This enum represents those options.
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/amm_bid.py` & `xrpl_py-2.2.0/xrpl/models/transactions/check_cash.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,58 @@
-"""Model for AMMBid transaction type."""
-from __future__ import annotations
+"""Model for CheckCash transaction type."""
+from __future__ import annotations  # Requires Python 3.7+
 
 from dataclasses import dataclass, field
-from typing import Dict, List, Optional
-
-from typing_extensions import Final
+from typing import Dict, Optional
 
 from xrpl.models.amounts import Amount
-from xrpl.models.auth_account import AuthAccount
-from xrpl.models.currencies import Currency
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
-_MAX_AUTH_ACCOUNTS: Final[int] = 4
-
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AMMBid(Transaction):
-    """
-    AMMBid is used to place a bid for the auction slot of obtaining trading advantages
-    of an AMM instance.
-
-    An AMM instance auctions off the trading advantages to users (arbitrageurs) at a
-    discounted TradingFee for a 24 hour slot.
+class CheckCash(Transaction):
     """
-
-    asset: Currency = REQUIRED  # type: ignore
-    """
-    Specifies one of the pool assets (XRP or token) of the AMM instance.
+    Represents a `CheckCash transaction <https://xrpl.org/checkcash.html>`_,
+    which redeems a Check object to receive up to the amount authorized by the
+    corresponding CheckCreate transaction. Only the Destination address of a
+    Check can cash it.
     """
 
-    asset2: Currency = REQUIRED  # type: ignore
-    """
-    Specifies the other pool asset of the AMM instance.
+    check_id: str = REQUIRED  # type: ignore
     """
+    The ID of the `Check ledger object
+    <https://xrpl.org/check.html>`_ to cash, as a 64-character
+    hexadecimal string. This field is required.
 
-    bid_min: Optional[Amount] = None
-    """
-    This field represents the minimum price that the bidder wants to pay for the slot.
-    It is specified in units of LPToken. If specified let MinSlotPrice be X and let
-    the slot-price computed by price scheduling algorithm be Y, then bidder always pays
-    the max(X, Y).
+    :meta hide-value:
     """
 
-    bid_max: Optional[Amount] = None
+    amount: Optional[Amount] = None
     """
-    This field represents the maximum price that the bidder wants to pay for the slot.
-    It is specified in units of LPToken.
+    Redeem the Check for exactly this amount, if possible. The currency must
+    match that of the SendMax of the corresponding CheckCreate transaction.
+    You must provide either this field or ``DeliverMin``.
     """
 
-    auth_accounts: Optional[List[AuthAccount]] = None
+    deliver_min: Optional[Amount] = None
     """
-    This field represents an array of XRPL account IDs that are authorized to trade
-    at the discounted fee against the AMM instance.
-    A maximum of four accounts can be provided.
+    Redeem the Check for at least this amount and for as much as possible.
+    The currency must match that of the ``SendMax`` of the corresponding
+    CheckCreate transaction. You must provide either this field or ``Amount``.
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.AMM_BID,
+        default=TransactionType.CHECK_CASH,
         init=False,
     )
 
-    def _get_errors(self: AMMBid) -> Dict[str, str]:
-        return {
-            key: value
-            for key, value in {
-                **super()._get_errors(),
-                "auth_accounts": self._get_auth_accounts_error(),
-            }.items()
-            if value is not None
-        }
-
-    def _get_auth_accounts_error(self: AMMBid) -> Optional[str]:
-        if (
-            self.auth_accounts is not None
-            and len(self.auth_accounts) > _MAX_AUTH_ACCOUNTS
-        ):
-            return f"Length must not be greater than {_MAX_AUTH_ACCOUNTS}"
-        return None
+    def _get_errors(self: CheckCash) -> Dict[str, str]:
+        errors = super()._get_errors()
+        if not (self.amount is None) ^ (self.deliver_min is None):
+            errors[
+                "CheckCash"
+            ] = "either amount or deliver_min must be set but not both"
+        return errors
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/amm_create.py` & `xrpl_py-2.2.0/xrpl/models/transactions/nftoken_cancel_offer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,58 @@
-"""Model for AMMCreate transaction type."""
+"""Model for NFTokenCancelOffer transaction type."""
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
-from typing_extensions import Final
-
-from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
-AMM_MAX_TRADING_FEE: Final[int] = 1000
-
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AMMCreate(Transaction):
-    """
-    AMMCreate is used to create AccountRoot and the corresponding AMM
-    ledger entries.
-    This allows for the creation of only one AMM instance per unique asset pair.
+class NFTokenCancelOffer(Transaction):
     """
+    The NFTokenCancelOffer transaction deletes existing NFTokenOffer objects.
+    It is useful if you want to free up space on your account to lower your
+    reserve requirement.
 
-    amount: Amount = REQUIRED  # type: ignore
-    """
-    Specifies one of the pool assets (XRP or token) of the AMM instance.
-    This field is required.
+    The transaction can be executed by the account that originally created
+    the NFTokenOffer, the account in the `Recipient` field of the NFTokenOffer
+    (if present), or any account if the NFTokenOffer has an `Expiration` and
+    the NFTokenOffer has already expired.
     """
 
-    amount2: Amount = REQUIRED  # type: ignore
-    """
-    Specifies the other pool asset of the AMM instance. This field is required.
+    nftoken_offers: List[str] = REQUIRED  # type: ignore
     """
+    An array of identifiers of NFTokenOffer objects that should be cancelled
+    by this transaction.
 
-    trading_fee: int = REQUIRED  # type: ignore
-    """
-    Specifies the fee, in basis point, to be charged
-    to the traders for the trades executed against the AMM instance.
-    Trading fee is a percentage of the trading volume.
-    Valid values for this field are between 0 and 1000 inclusive.
-    A value of 1 is equivalent to 1/10 bps or 0.001%, allowing trading fee
-    between 0% and 1%. This field is required.
+    It is an error if an entry in this list points to an
+    object that is not an NFTokenOffer object. It is not an
+    error if an entry in this list points to an object that
+    does not exist. This field is required.
+
+    :meta hide-value:
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.AMM_CREATE,
+        default=TransactionType.NFTOKEN_CANCEL_OFFER,
         init=False,
     )
 
-    def _get_errors(self: AMMCreate) -> Dict[str, str]:
+    def _get_errors(self: NFTokenCancelOffer) -> Dict[str, str]:
         return {
             key: value
             for key, value in {
                 **super()._get_errors(),
-                "trading_fee": self._get_trading_fee_error(),
+                "nftoken_offers": self._get_nftoken_offers_error(),
             }.items()
             if value is not None
         }
 
-    def _get_trading_fee_error(self: AMMCreate) -> Optional[str]:
-        if self.trading_fee < 0 or self.trading_fee > AMM_MAX_TRADING_FEE:
-            return f"Must be between 0 and {AMM_MAX_TRADING_FEE}"
+    def _get_nftoken_offers_error(self: NFTokenCancelOffer) -> Optional[str]:
+        if len(self.nftoken_offers) < 1:
+            return "Must specify at least one NFTokenOffer to cancel"
         return None
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/check_cancel.py` & `xrpl_py-2.2.0/xrpl/models/transactions/check_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/check_cash.py` & `xrpl_py-2.2.0/xrpl/models/transactions/check_create.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,63 @@
-"""Model for CheckCash transaction type."""
-from __future__ import annotations  # Requires Python 3.7+
-
+"""Model for CheckCreate transaction type."""
 from dataclasses import dataclass, field
-from typing import Dict, Optional
+from typing import Optional
 
 from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class CheckCash(Transaction):
+class CheckCreate(Transaction):
+    """
+    Represents a `CheckCreate <https://xrpl.org/checkcreate.html>`_ transaction,
+    which creates a Check object. A Check object is a deferred payment
+    that can be cashed by its intended destination. The sender of this
+    transaction is the sender of the Check.
     """
-    Represents a `CheckCash transaction <https://xrpl.org/checkcash.html>`_,
-    which redeems a Check object to receive up to the amount authorized by the
-    corresponding CheckCreate transaction. Only the Destination address of a
-    Check can cash it.
+
+    destination: str = REQUIRED  # type: ignore
+    """
+    The address of the `account
+    <https://xrpl.org/accounts.html>`_ that can cash the Check. This field is
+    required.
+
+    :meta hide-value:
     """
 
-    check_id: str = REQUIRED  # type: ignore
+    send_max: Amount = REQUIRED  # type: ignore
     """
-    The ID of the `Check ledger object
-    <https://xrpl.org/check.html>`_ to cash, as a 64-character
-    hexadecimal string. This field is required.
+    Maximum amount of source token the Check is allowed to debit the
+    sender, including transfer fees on non-XRP tokens. The Check can only
+    credit the destination with the same token (from the same issuer, for
+    non-XRP tokens). This field is required.
 
     :meta hide-value:
     """
 
-    amount: Optional[Amount] = None
+    destination_tag: Optional[int] = None
     """
-    Redeem the Check for exactly this amount, if possible. The currency must
-    match that of the SendMax of the corresponding CheckCreate transaction.
-    You must provide either this field or ``DeliverMin``.
+    An arbitrary `destination tag
+    <https://xrpl.org/source-and-destination-tags.html>`_ that
+    identifies the reason for the Check, or a hosted recipient to pay.
     """
 
-    deliver_min: Optional[Amount] = None
+    expiration: Optional[int] = None
     """
-    Redeem the Check for at least this amount and for as much as possible.
-    The currency must match that of the ``SendMax`` of the corresponding
-    CheckCreate transaction. You must provide either this field or ``Amount``.
+    Time after which the Check is no longer valid, in seconds since the
+    Ripple Epoch.
+    """
+
+    invoice_id: Optional[str] = None
+    """
+    Arbitrary 256-bit hash representing a specific reason or identifier for
+    this Check.
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.CHECK_CASH,
+        default=TransactionType.CHECK_CREATE,
         init=False,
     )
-
-    def _get_errors(self: CheckCash) -> Dict[str, str]:
-        errors = super()._get_errors()
-        if not (self.amount is None) ^ (self.deliver_min is None):
-            errors[
-                "CheckCash"
-            ] = "either amount or deliver_min must be set but not both"
-        return errors
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/check_create.py` & `xrpl_py-2.2.0/xrpl/models/transactions/payment_channel_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,75 @@
-"""Model for CheckCreate transaction type."""
+"""Model for PaymentChannelCreate transaction type."""
 from dataclasses import dataclass, field
 from typing import Optional
 
 from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class CheckCreate(Transaction):
+class PaymentChannelCreate(Transaction):
     """
-    Represents a `CheckCreate <https://xrpl.org/checkcreate.html>`_ transaction,
-    which creates a Check object. A Check object is a deferred payment
-    that can be cashed by its intended destination. The sender of this
-    transaction is the sender of the Check.
+    Represents a `PaymentChannelCreate
+    <https://xrpl.org/paymentchannelcreate.html>`_ transaction, which creates a
+    `payment channel <https://xrpl.org/payment-channels.html>`_ and funds it with
+    XRP. The sender of this transaction is the "source address" of the payment
+    channel.
     """
 
-    destination: str = REQUIRED  # type: ignore
+    amount: Amount = REQUIRED  # type: ignore
     """
-    The address of the `account
-    <https://xrpl.org/accounts.html>`_ that can cash the Check. This field is
+    The amount of XRP, in drops, to set aside in this channel. This field is
     required.
 
     :meta hide-value:
     """
 
-    send_max: Amount = REQUIRED  # type: ignore
+    destination: str = REQUIRED  # type: ignore
     """
-    Maximum amount of source token the Check is allowed to debit the
-    sender, including transfer fees on non-XRP tokens. The Check can only
-    credit the destination with the same token (from the same issuer, for
-    non-XRP tokens). This field is required.
+    The account that can receive XRP from this channel, also known as the
+    "destination address" of the channel. Cannot be the same as the sender.
+    This field is required.
 
     :meta hide-value:
     """
 
-    destination_tag: Optional[int] = None
+    settle_delay: int = REQUIRED  # type: ignore
     """
-    An arbitrary `destination tag
-    <https://xrpl.org/source-and-destination-tags.html>`_ that
-    identifies the reason for the Check, or a hosted recipient to pay.
+    The amount of time, in seconds, the source address must wait between
+    requesting to close the channel and fully closing it. This field is
+    required.
+
+    :meta hide-value:
     """
 
-    expiration: Optional[int] = None
+    public_key: str = REQUIRED  # type: ignore
     """
-    Time after which the Check is no longer valid, in seconds since the
-    Ripple Epoch.
+    The public key of the key pair that the source will use to authorize
+    claims against this  channel, as hexadecimal. This can be any valid
+    secp256k1 or Ed25519 public key. This field is required.
+
+    :meta hide-value:
+    """
+
+    cancel_after: Optional[int] = None
+    """
+    An immutable expiration time for the channel, in seconds since the Ripple
+    Epoch. The channel can be closed sooner than this but cannot remain open
+    later than this time.
     """
 
-    invoice_id: Optional[str] = None
+    destination_tag: Optional[int] = None
     """
-    Arbitrary 256-bit hash representing a specific reason or identifier for
-    this Check.
+    An arbitrary `destination tag
+    <https://xrpl.org/source-and-destination-tags.html>`_ that
+    identifies the reason for the Payment Channel, or a hosted recipient to pay.
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.CHECK_CREATE,
+        default=TransactionType.PAYMENT_CHANNEL_CREATE,
         init=False,
     )
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/deposit_preauth.py` & `xrpl_py-2.2.0/xrpl/models/transactions/deposit_preauth.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_cancel.py` & `xrpl_py-2.2.0/xrpl/models/transactions/escrow_cancel.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class EscrowCancel(Transaction):
     """
     Represents an `EscrowCancel <https://xrpl.org/escrowcancel.html>`_
-    transaction, which returns escrowed amount to the sender after the Escrow has
+    transaction, which returns escrowed XRP to the sender after the Escrow has
     expired.
     """
 
     owner: str = REQUIRED  # type: ignore
     """
     The address of the account that funded the Escrow. This field is required.
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_create.py` & `xrpl_py-2.2.0/xrpl/models/transactions/escrow_finish.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,66 @@
-"""Model for EscrowCreate transaction type."""
+"""Model for EscrowFinish transaction type."""
 from __future__ import annotations  # Requires Python 3.7+
 
 from dataclasses import dataclass, field
 from typing import Dict, Optional
 
-from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class EscrowCreate(Transaction):
+class EscrowFinish(Transaction):
     """
-    Represents an `EscrowCreate <https://xrpl.org/escrowcreate.html>`_
-    transaction, which locks up amount until a specific time or condition is met.
+    Represents an `EscrowFinish <https://xrpl.org/escrowfinish.html>`_
+    transaction, delivers XRP from a held payment to the recipient.
     """
 
-    amount: Amount = REQUIRED  # type: ignore
+    owner: str = REQUIRED  # type: ignore
     """
-    Amount to deduct from the sender's balance and escrow. Once escrowed, the
-    amount can either go to the Destination address (after the FinishAfter time)
-    or returned to the sender (after the CancelAfter time). This field is required.
+    The source account that funded the Escrow. This field is required.
 
     :meta hide-value:
     """
 
-    destination: str = REQUIRED  # type: ignore
+    offer_sequence: int = REQUIRED  # type: ignore
     """
-    The address that should receive the escrowed amount when the time or
-    condition is met. This field is required.
+    Transaction sequence (or Ticket number) of the EscrowCreate transaction
+    that created the Escrow. This field is required.
 
     :meta hide-value:
     """
 
-    destination_tag: Optional[int] = None
-    """
-    An arbitrary `destination tag
-    <https://xrpl.org/source-and-destination-tags.html>`_ that
-    identifies the reason for the Escrow, or a hosted recipient to pay.
-    """
-
-    cancel_after: Optional[int] = None
-    """
-    The time, in seconds since the Ripple Epoch, when this escrow expires.
-    This value is immutable; the funds can only be returned the sender after
-    this time.
-    """
-
-    finish_after: Optional[int] = None
+    condition: Optional[str] = None
     """
-    The time, in seconds since the Ripple Epoch, when the escrowed amount can
-    be released to the recipient. This value is immutable; the funds cannot
-    move until this time is reached.
+    The previously-supplied `PREIMAGE-SHA-256 crypto-condition
+    <https://tools.ietf.org/html/draft-thomas-crypto-conditions-04#section-8.1.>`_
+    of the Escrow, if any, as hexadecimal.
     """
 
-    condition: Optional[str] = None
+    fulfillment: Optional[str] = None
     """
-    Hex value representing a `PREIMAGE-SHA-256 crypto-condition
-    <https://tools.ietf.org/html/draft-thomas-crypto-conditions-04#section-8.1.>`_
-    The funds can only be delivered to the recipient if this condition is
-    fulfilled.
+    The `PREIMAGE-SHA-256 crypto-condition fulfillment
+    <https://tools.ietf.org/html/draft-thomas-crypto-conditions-04#section-8.1.4.>`_
+    matching the Escrow's condition, if any, as hexadecimal.
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.ESCROW_CREATE,
+        default=TransactionType.ESCROW_FINISH,
         init=False,
     )
 
-    def _get_errors(self: EscrowCreate) -> Dict[str, str]:
+    def _get_errors(self: EscrowFinish) -> Dict[str, str]:
         errors = super()._get_errors()
-        if (
-            self.cancel_after is not None
-            and self.finish_after is not None
-            and self.finish_after >= self.cancel_after
-        ):
+        if self.condition and not self.fulfillment:
+            errors[
+                "fulfillment"
+            ] = "If condition is specified, fulfillment must also be specified."
+        if self.fulfillment and not self.condition:
             errors[
-                "EscrowCreate"
-            ] = "The finish_after time must be before the cancel_after time."
+                "condition"
+            ] = "If fulfillment is specified, condition must also be specified."
 
         return errors
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/escrow_finish.py` & `xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/unl_modify.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,71 @@
-"""Model for EscrowFinish transaction type."""
-from __future__ import annotations  # Requires Python 3.7+
+"""Model for UNLModify pseudo-transaction type."""
+
+from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Dict, Optional
+from typing import Dict
 
 from xrpl.models.required import REQUIRED
-from xrpl.models.transactions.transaction import Transaction
-from xrpl.models.transactions.types import TransactionType
+from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
+    PseudoTransaction,
+)
+from xrpl.models.transactions.types import PseudoTransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class EscrowFinish(Transaction):
+class UNLModify(PseudoTransaction):
     """
-    Represents an `EscrowFinish <https://xrpl.org/escrowfinish.html>`_
-    transaction, delivers XRP from a held payment to the recipient.
+    A UNLModify pseudo-transaction marks a change to the `Negative UNL
+    <https://xrpl.org/negative-unl.html>`_, indicating that a trusted validator has
+    gone offline or come back online.
     """
 
-    owner: str = REQUIRED  # type: ignore
+    ledger_sequence: int = REQUIRED  # type: ignore
     """
-    The source account that funded the Escrow. This field is required.
+    The ledger index where this pseudo-transaction appears. This distinguishes the
+    pseudo-transaction from other occurrences of the same change.
+    This field is required.
 
     :meta hide-value:
     """
 
-    offer_sequence: int = REQUIRED  # type: ignore
+    unl_modify_disabling: int = REQUIRED  # type: ignore
     """
-    Transaction sequence (or Ticket number) of the EscrowCreate transaction
-    that created the Escrow. This field is required.
+    If 1, this change represents adding a validator to the Negative UNL. If 0, this
+    change represents removing a validator from the Negative UNL. (No other values
+    are allowed.) This field is required.
 
     :meta hide-value:
     """
 
-    condition: Optional[str] = None
-    """
-    The previously-supplied `PREIMAGE-SHA-256 crypto-condition
-    <https://tools.ietf.org/html/draft-thomas-crypto-conditions-04#section-8.1.>`_
-    of the Escrow, if any, as hexadecimal.
+    unl_modify_validator: str = REQUIRED  # type: ignore
     """
+    The validator to add or remove, as identified by its master public key.
+    This field is required.
 
-    fulfillment: Optional[str] = None
-    """
-    The `PREIMAGE-SHA-256 crypto-condition fulfillment
-    <https://tools.ietf.org/html/draft-thomas-crypto-conditions-04#section-8.1.4.>`_
-    matching the Escrow's condition, if any, as hexadecimal.
+    :meta hide-value:
     """
 
-    transaction_type: TransactionType = field(
-        default=TransactionType.ESCROW_FINISH,
+    transaction_type: PseudoTransactionType = field(
+        default=PseudoTransactionType.UNL_MODIFY,
         init=False,
     )
 
-    def _get_errors(self: EscrowFinish) -> Dict[str, str]:
+    flags: int = 0
+    """
+    The Flags value of the EnableAmendment pseudo-transaction indicates the status
+    of the amendment at the time of the ledger including the pseudo-transaction.
+    A Flags value of 0 (no flags) or an omitted Flags field indicates that the
+    amendment has been enabled, and applies to all ledgers afterward.
+    """
+
+    def _get_errors(self: UNLModify) -> Dict[str, str]:
         errors = super()._get_errors()
-        if self.condition and not self.fulfillment:
-            errors[
-                "fulfillment"
-            ] = "If condition is specified, fulfillment must also be specified."
-        if self.fulfillment and not self.condition:
+        if self.unl_modify_disabling not in {0, 1}:
             errors[
-                "condition"
-            ] = "If fulfillment is specified, condition must also be specified."
+                "unl_modify_disabling"
+            ] = "`unl_modify_disabling` is not equal to 0 or 1."
 
         return errors
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/metadata.py` & `xrpl_py-2.2.0/xrpl/models/transactions/metadata.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_accept_offer.py` & `xrpl_py-2.2.0/xrpl/models/transactions/nftoken_accept_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_burn.py` & `xrpl_py-2.2.0/xrpl/models/transactions/nftoken_burn.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_create_offer.py` & `xrpl_py-2.2.0/xrpl/models/transactions/nftoken_create_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/nftoken_mint.py` & `xrpl_py-2.2.0/xrpl/models/transactions/nftoken_mint.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/offer_cancel.py` & `xrpl_py-2.2.0/xrpl/models/transactions/offer_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/offer_create.py` & `xrpl_py-2.2.0/xrpl/models/transactions/offer_create.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/payment.py` & `xrpl_py-2.2.0/xrpl/models/transactions/payment.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_claim.py` & `xrpl_py-2.2.0/xrpl/models/transactions/payment_channel_claim.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Model for PaymentChannelClaim transaction type."""
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional
 
-from xrpl.models.amounts import Amount
 from xrpl.models.flags import FlagInterface
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
@@ -27,22 +26,22 @@
     channel can use this flag.
     """
 
     TF_CLOSE = 0x00020000
     """
     Request to close the channel. Only the channel source and destination addresses
     can use this flag. This flag closes the channel immediately if it has no more
-    funds allocated to it after processing the current claim, or if the destination
+    XRP allocated to it after processing the current claim, or if the destination
     address uses it. If the source address uses this flag when the channel still
-    holds a value, this schedules the channel to close after `SettleDelay` seconds have
+    holds XRP, this schedules the channel to close after `SettleDelay` seconds have
     passed. (Specifically, this sets the `Expiration` of the channel to the close
     time of the previous ledger plus the channel's `SettleDelay` time, unless the
     channel already has an earlier `Expiration` time.) If the destination address
-    uses this flag when the channel still holds an amount, any amount that remains
-    after processing the claim is returned to the source address.
+    uses this flag when the channel still holds XRP, any XRP that remains after
+    processing the claim is returned to the source address.
     """
 
 
 class PaymentChannelClaimFlagInterface(FlagInterface):
     """
     Transactions of the PaymentChannelClaim type support additional values in the Flags
     field. This TypedDict represents those options.
@@ -56,41 +55,38 @@
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class PaymentChannelClaim(Transaction):
     """
     Represents a `PaymentChannelClaim <https://xrpl.org/paymentchannelclaim.html>`_
-    transaction, which claims an amount from a `payment channel
+    transaction, which claims XRP from a `payment channel
     <https://xrpl.org/payment-channels.html>`_, adjusts
     channel's expiration, or both. This transaction can be used differently
     depending on the transaction sender's role in the specified channel.
     """
 
     channel: str = REQUIRED  # type: ignore
     """
     The unique ID of the payment channel, as a 64-character hexadecimal
     string. This field is required.
 
     :meta hide-value:
     """
 
-    balance: Optional[Amount] = None
+    balance: Optional[str] = None
     """
-    Total amount delivered by this channel after processing this claim. Required
-    to deliver amount. Must be more than the total amount delivered by the channel
-    so far, but not greater than the Amount of the signed claim. Must be provided
-    except when closing the channel.
+    The cumulative amount of XRP to have delivered through this channel after
+    processing this claim. Required unless closing the channel.
     """
 
-    amount: Optional[Amount] = None
+    amount: Optional[str] = None
     """
-    The amount authorized by the Signature. This must match the amount in the signed
-    message. This is the cumulative amount that can be dispensed by the channel,
-    including amounts previously redeemed. Required unless closing the channel.
+    The cumulative amount of XRP that has been authorized to deliver by the
+    attached claim signature. Required unless closing the channel.
     """
 
     signature: Optional[str] = None
     """
     The signature of the claim, as hexadecimal. This signature must be
     verifiable for the this channel and the given ``public_key`` and ``amount``
     values. May be omitted if closing the channel or if the sender of this
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_create.py` & `xrpl_py-2.2.0/xrpl/models/transactions/payment_channel_fund.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,49 @@
-"""Model for PaymentChannelCreate transaction type."""
+"""Model for a PaymentChannelFund transaction type."""
 from dataclasses import dataclass, field
 from typing import Optional
 
-from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class PaymentChannelCreate(Transaction):
+class PaymentChannelFund(Transaction):
     """
-    Represents a `PaymentChannelCreate
-    <https://xrpl.org/paymentchannelcreate.html>`_ transaction, which creates a
-    `payment channel <https://xrpl.org/payment-channels.html>`_ and funds it with
-    an amount. The sender of this transaction is the "source address" of the payment
-    channel.
+    Represents a `PaymentChannelFund <https://xrpl.org/paymentchannelfund.html>`_
+    transaction, adds additional XRP to an open `payment channel
+    <https://xrpl.org/payment-channels.html>`_, and optionally updates the
+    expiration time of the channel. Only the source address
+    of the channel can use this transaction.
     """
 
-    amount: Amount = REQUIRED  # type: ignore
+    channel: str = REQUIRED  # type: ignore
     """
-    Amount to deduct from the sender's balance and set aside in this channel.
-    While the channel is open, the amount can only go to the Destination address.
-    When the channel closes, any unclaimed amount is returned to the source
-    address's balance. This field is required.
+    The unique ID of the payment channel, as a 64-character hexadecimal
+    string. This field is required.
 
     :meta hide-value:
     """
 
-    destination: str = REQUIRED  # type: ignore
+    amount: str = REQUIRED  # type: ignore
     """
-    The account that can receive amounts from this channel, also known as the
-    "destination address" of the channel. Cannot be the same as the sender.
-    This field is required.
-
-    :meta hide-value:
-    """
-
-    settle_delay: int = REQUIRED  # type: ignore
-    """
-    The amount of time, in seconds, the source address must wait between
-    requesting to close the channel and fully closing it. This field is
+    The amount of XRP, in drops, to add to the channel. This field is
     required.
 
     :meta hide-value:
     """
 
-    public_key: str = REQUIRED  # type: ignore
-    """
-    The public key of the key pair that the source will use to authorize
-    claims against this  channel, as hexadecimal. This can be any valid
-    secp256k1 or Ed25519 public key. This field is required.
-
-    :meta hide-value:
-    """
-
-    cancel_after: Optional[int] = None
-    """
-    An immutable expiration time for the channel, in seconds since the Ripple
-    Epoch. The channel can be closed sooner than this but cannot remain open
-    later than this time.
-    """
-
-    destination_tag: Optional[int] = None
+    expiration: Optional[int] = None
     """
-    An arbitrary `destination tag
-    <https://xrpl.org/source-and-destination-tags.html>`_ that
-    identifies the reason for the Payment Channel, or a hosted recipient to pay.
+    A new mutable expiration time to set for the channel, in seconds since the
+    Ripple Epoch. This must be later than the existing expiration time of the
+    channel or later than the current time plus the settle delay of the channel.
+    This is separate from the immutable ``cancel_after`` time.
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.PAYMENT_CHANNEL_CREATE,
+        default=TransactionType.PAYMENT_CHANNEL_FUND,
         init=False,
     )
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/payment_channel_fund.py` & `xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/set_fee.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,63 @@
-"""Model for a PaymentChannelFund transaction type."""
+"""Model for SetFee pseudo-transaction type."""
+
 from dataclasses import dataclass, field
 from typing import Optional
 
-from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
-from xrpl.models.transactions.transaction import Transaction
-from xrpl.models.transactions.types import TransactionType
+from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
+    PseudoTransaction,
+)
+from xrpl.models.transactions.types import PseudoTransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class PaymentChannelFund(Transaction):
+class SetFee(PseudoTransaction):
+    """
+    A SetFee pseudo-transaction marks a change in `transaction cost
+    <https://xrpl.org/transaction-cost.html>`_ or `reserve requirements
+    <https://xrpl.org/reserves.html>`_ as a result of `Fee Voting
+    <https://xrpl.org/fee-voting.html>`_.
+    """
+
+    base_fee: str = REQUIRED  # type: ignore
     """
-    Represents a `PaymentChannelFund <https://xrpl.org/paymentchannelfund.html>`_
-    transaction, adds additional amount to an open `payment channel
-    <https://xrpl.org/payment-channels.html>`_, and optionally updates the
-    expiration time of the channel. Only the source address
-    of the channel can use this transaction.
+    The charge, in drops of XRP, for the reference transaction, as hex. (This is the
+    transaction cost before scaling for load.) This field is required.
+
+    :meta hide-value:
+    """
+
+    reference_fee_units: int = REQUIRED  # type: ignore
+    """
+    The cost, in fee units, of the reference transaction. This field is required.
+
+    :meta hide-value:
     """
 
-    channel: str = REQUIRED  # type: ignore
+    reserve_base: int = REQUIRED  # type: ignore
     """
-    The unique ID of the payment channel, as a 64-character hexadecimal
-    string. This field is required.
+    The base reserve, in drops. This field is required.
 
     :meta hide-value:
     """
 
-    amount: Amount = REQUIRED  # type: ignore
+    reserve_increment: int = REQUIRED  # type: ignore
     """
-    Amount to add to the channel. Must be a positive amount. This field is required.
+    The incremental reserve, in drops. This field is required.
 
     :meta hide-value:
     """
 
-    expiration: Optional[int] = None
+    ledger_sequence: Optional[int] = None
     """
-    A new mutable expiration time to set for the channel, in seconds since the
-    Ripple Epoch. This must be later than the existing expiration time of the
-    channel or later than the current time plus the settle delay of the channel.
-    This is separate from the immutable ``cancel_after`` time.
+    The index of the ledger version where this pseudo-transaction appears. This
+    distinguishes the pseudo-transaction from other occurrences of the same change.
+    This field is omitted for some historical SetFee pseudo-transactions.
     """
 
-    transaction_type: TransactionType = field(
-        default=TransactionType.PAYMENT_CHANNEL_FUND,
+    transaction_type: PseudoTransactionType = field(
+        default=PseudoTransactionType.SET_FEE,
         init=False,
     )
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py` & `xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py` & `xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py` & `xrpl_py-2.2.0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py` & `xrpl_py-2.2.0/xrpl/models/transactions/trust_set.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,87 @@
-"""Model for SetFee pseudo-transaction type."""
+"""
+Represents a TrustSet transaction on the XRP Ledger.
+Creates or modifies a trust line linking two accounts.
 
+`See TrustSet <https://xrpl.org/trustset.html>`_
+"""
 from dataclasses import dataclass, field
+from enum import Enum
 from typing import Optional
 
+from xrpl.models.amounts import IssuedCurrencyAmount
+from xrpl.models.flags import FlagInterface
 from xrpl.models.required import REQUIRED
-from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
-    PseudoTransaction,
-)
-from xrpl.models.transactions.types import PseudoTransactionType
+from xrpl.models.transactions.transaction import Transaction
+from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
-@require_kwargs_on_init
-@dataclass(frozen=True)
-class SetFee(PseudoTransaction):
+class TrustSetFlag(int, Enum):
     """
-    A SetFee pseudo-transaction marks a change in `transaction cost
-    <https://xrpl.org/transaction-cost.html>`_ or `reserve requirements
-    <https://xrpl.org/reserves.html>`_ as a result of `Fee Voting
-    <https://xrpl.org/fee-voting.html>`_.
+    Transactions of the TrustSet type support additional values in the Flags field.
+    This enum represents those options.
     """
 
-    base_fee: str = REQUIRED  # type: ignore
+    TF_SET_AUTH = 0x00010000
     """
-    The charge, in drops of XRP, for the reference transaction, as hex. (This is the
-    transaction cost before scaling for load.) This field is required.
-
-    :meta hide-value:
+    Authorize the other party to hold
+    `currency issued by this account <https://xrpl.org/tokens.html>`_.
+    (No effect unless using the `asfRequireAuth AccountSet flag
+    <https://xrpl.org/accountset.html#accountset-flags>`_.) Cannot be unset.
     """
 
-    reference_fee_units: int = REQUIRED  # type: ignore
+    TF_SET_NO_RIPPLE = 0x00020000
+    """
+    Enable the No Ripple flag, which blocks
+    `rippling <https://xrpl.org/rippling.html>`_ between two trust
+    lines of the same currency if this flag is enabled on both.
     """
-    The cost, in fee units, of the reference transaction. This field is required.
 
-    :meta hide-value:
+    TF_CLEAR_NO_RIPPLE = 0x00040000
+    """Disable the No Ripple flag, allowing rippling on this trust line."""
+
+    TF_SET_FREEZE = 0x00100000
+    """Freeze the trust line."""
+
+    TF_CLEAR_FREEZE = 0x00200000
+    """Unfreeze the trust line."""
+
+
+class TrustSetFlagInterface(FlagInterface):
     """
+    Transactions of the TrustSet type support additional values in the Flags field.
+    This TypedDict represents those options.
+    """
+
+    TF_SET_AUTH: bool
+    TF_SET_NO_RIPPLE: bool
+    TF_CLEAR_NO_RIPPLE: bool
+    TF_SET_FREEZE: bool
+    TF_CLEAR_FREEZE: bool
+
 
-    reserve_base: int = REQUIRED  # type: ignore
+@require_kwargs_on_init
+@dataclass(frozen=True)
+class TrustSet(Transaction):
     """
-    The base reserve, in drops. This field is required.
+    Represents a TrustSet transaction on the XRP Ledger.
+    Creates or modifies a trust line linking two accounts.
 
-    :meta hide-value:
+    `See TrustSet <https://xrpl.org/trustset.html>`_
     """
 
-    reserve_increment: int = REQUIRED  # type: ignore
+    limit_amount: IssuedCurrencyAmount = REQUIRED  # type: ignore
     """
-    The incremental reserve, in drops. This field is required.
+    This field is required.
 
     :meta hide-value:
     """
 
-    ledger_sequence: Optional[int] = None
-    """
-    The index of the ledger version where this pseudo-transaction appears. This
-    distinguishes the pseudo-transaction from other occurrences of the same change.
-    This field is omitted for some historical SetFee pseudo-transactions.
-    """
+    quality_in: Optional[int] = None
+
+    quality_out: Optional[int] = None
 
-    transaction_type: PseudoTransactionType = field(
-        default=PseudoTransactionType.SET_FEE,
+    transaction_type: TransactionType = field(
+        default=TransactionType.TRUST_SET,
         init=False,
     )
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py` & `xrpl_py-2.2.0/xrpl/models/transactions/escrow_create.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,83 @@
-"""Model for UNLModify pseudo-transaction type."""
-
-from __future__ import annotations
+"""Model for EscrowCreate transaction type."""
+from __future__ import annotations  # Requires Python 3.7+
 
 from dataclasses import dataclass, field
-from typing import Dict
+from typing import Dict, Optional
 
+from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
-from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
-    PseudoTransaction,
-)
-from xrpl.models.transactions.types import PseudoTransactionType
+from xrpl.models.transactions.transaction import Transaction
+from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class UNLModify(PseudoTransaction):
+class EscrowCreate(Transaction):
     """
-    A UNLModify pseudo-transaction marks a change to the `Negative UNL
-    <https://xrpl.org/negative-unl.html>`_, indicating that a trusted validator has
-    gone offline or come back online.
+    Represents an `EscrowCreate <https://xrpl.org/escrowcreate.html>`_
+    transaction, which locks up XRP until a specific time or condition is met.
     """
 
-    ledger_sequence: int = REQUIRED  # type: ignore
+    amount: Amount = REQUIRED  # type: ignore
     """
-    The ledger index where this pseudo-transaction appears. This distinguishes the
-    pseudo-transaction from other occurrences of the same change.
-    This field is required.
+    Amount of XRP, in drops, to deduct from the sender's balance and set
+    aside in escrow. This field is required.
 
     :meta hide-value:
     """
 
-    unl_modify_disabling: int = REQUIRED  # type: ignore
+    destination: str = REQUIRED  # type: ignore
     """
-    If 1, this change represents adding a validator to the Negative UNL. If 0, this
-    change represents removing a validator from the Negative UNL. (No other values
-    are allowed.) This field is required.
+    The address that should receive the escrowed XRP when the time or
+    condition is met. This field is required.
 
     :meta hide-value:
     """
 
-    unl_modify_validator: str = REQUIRED  # type: ignore
+    destination_tag: Optional[int] = None
+    """
+    An arbitrary `destination tag
+    <https://xrpl.org/source-and-destination-tags.html>`_ that
+    identifies the reason for the Escrow, or a hosted recipient to pay.
     """
-    The validator to add or remove, as identified by its master public key.
-    This field is required.
 
-    :meta hide-value:
+    cancel_after: Optional[int] = None
+    """
+    The time, in seconds since the Ripple Epoch, when this escrow expires.
+    This value is immutable; the funds can only be returned the sender after
+    this time.
     """
 
-    transaction_type: PseudoTransactionType = field(
-        default=PseudoTransactionType.UNL_MODIFY,
-        init=False,
-    )
+    finish_after: Optional[int] = None
+    """
+    The time, in seconds since the Ripple Epoch, when the escrowed XRP can
+    be released to the recipient. This value is immutable; the funds cannot
+    move until this time is reached.
+    """
 
-    flags: int = 0
+    condition: Optional[str] = None
     """
-    The Flags value of the EnableAmendment pseudo-transaction indicates the status
-    of the amendment at the time of the ledger including the pseudo-transaction.
-    A Flags value of 0 (no flags) or an omitted Flags field indicates that the
-    amendment has been enabled, and applies to all ledgers afterward.
+    Hex value representing a `PREIMAGE-SHA-256 crypto-condition
+    <https://tools.ietf.org/html/draft-thomas-crypto-conditions-04#section-8.1.>`_
+    The funds can only be delivered to the recipient if this condition is
+    fulfilled.
     """
 
-    def _get_errors(self: UNLModify) -> Dict[str, str]:
+    transaction_type: TransactionType = field(
+        default=TransactionType.ESCROW_CREATE,
+        init=False,
+    )
+
+    def _get_errors(self: EscrowCreate) -> Dict[str, str]:
         errors = super()._get_errors()
-        if self.unl_modify_disabling not in {0, 1}:
+        if (
+            self.cancel_after is not None
+            and self.finish_after is not None
+            and self.finish_after >= self.cancel_after
+        ):
             errors[
-                "unl_modify_disabling"
-            ] = "`unl_modify_disabling` is not equal to 0 or 1."
+                "EscrowCreate"
+            ] = "The finish_after time must be before the cancel_after time."
 
         return errors
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/set_regular_key.py` & `xrpl_py-2.2.0/xrpl/models/transactions/set_regular_key.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/signer_list_set.py` & `xrpl_py-2.2.0/xrpl/models/transactions/signer_list_set.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/ticket_create.py` & `xrpl_py-2.2.0/xrpl/models/transactions/ticket_create.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/transaction.py` & `xrpl_py-2.2.0/xrpl/models/transactions/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 from hashlib import sha512
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 from typing_extensions import Final
 
 from xrpl.core.binarycodec import decode, encode
 from xrpl.models.amounts import IssuedCurrencyAmount
-from xrpl.models.base_model import ABBREVIATIONS, BaseModel
+from xrpl.models.base_model import BaseModel
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.flags import check_false_flag_definition, interface_to_flag_list
 from xrpl.models.nested_model import NestedModel
 from xrpl.models.requests import PathStep
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.types import PseudoTransactionType, TransactionType
 from xrpl.models.types import XRPL_VALUE_TYPE
 from xrpl.models.utils import require_kwargs_on_init
 
 _TRANSACTION_HASH_PREFIX: Final[int] = 0x54584E00
-
-# special cases that should not be snake cased and only contain primitive members
-_LOWER_CASE_MODELS: List[Type[BaseModel]] = [
-    IssuedCurrencyAmount,
-    PathStep,
-]
+# This is used to make exceptions when converting dictionary keys to xrpl JSON
+# keys. We snake case keys, but some keys are abbreviations.
+_ABBREVIATIONS: Final[Dict[str, str]] = {
+    "unl": "UNL",
+    "id": "ID",
+    "uri": "URI",
+    "nftoken": "NFToken",
+}
 
 
 def transaction_json_to_binary_codec_form(
     dictionary: Dict[str, XRPL_VALUE_TYPE]
 ) -> Dict[str, XRPL_VALUE_TYPE]:
     """
     Returns a new dictionary in which the keys have been formatted as CamelCase and
@@ -50,43 +52,36 @@
 
 def _key_to_tx_json(key: str) -> str:
     """
     Transforms snake_case to PascalCase. For example:
         1. 'transaction_type' becomes 'TransactionType'
         2. 'URI' becomes 'uri'
 
-    Known abbreviations (example 2 above) need to be enumerated in ABBREVIATIONS.
+    Known abbreviations (example 2 above) need to be enumerated in _ABBREVIATIONS.
     """
     return "".join(
         [
-            ABBREVIATIONS[word] if word in ABBREVIATIONS else word.capitalize()
+            _ABBREVIATIONS[word] if word in _ABBREVIATIONS else word.capitalize()
             for word in key.split("_")
         ]
     )
 
 
 def _value_to_tx_json(value: XRPL_VALUE_TYPE) -> XRPL_VALUE_TYPE:
-    if isinstance(value, dict) and "auth_account" in value:
-        return _auth_account_value_to_tx_json(value)
-    if any([model.is_dict_of_model(value) for model in _LOWER_CASE_MODELS]):
+    # IssuedCurrencyAmount and PathStep are special cases and should not be snake cased
+    # and only contain primitive members
+    if IssuedCurrencyAmount.is_dict_of_model(value) or PathStep.is_dict_of_model(value):
         return value
     if isinstance(value, dict):
         return transaction_json_to_binary_codec_form(value)
     if isinstance(value, list):
         return [_value_to_tx_json(sub_value) for sub_value in value]
     return value
 
 
-def _auth_account_value_to_tx_json(value: Dict[str, Any]) -> Dict[str, Any]:
-    return {
-        _key_to_tx_json(key): transaction_json_to_binary_codec_form(val)
-        for (key, val) in value.items()
-    }
-
-
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class Memo(NestedModel):
     """
     An arbitrary piece of data attached to a transaction. A transaction can
     have multiple Memo objects as an array in the Memos field.
     Must contain one or more of ``memo_data``, ``memo_format``, and
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/transactions/xchain_account_create_commit.py` & `xrpl_py-2.2.0/xrpl/models/requests/channel_verify.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,49 @@
-"""Model for a XChainAccountCreateCommit transaction type."""
-
-from __future__ import annotations
-
+"""
+The channel_verify method checks the validity of a
+signature that can be used to redeem a specific amount of
+XRP from a payment channel.
+"""
 from dataclasses import dataclass, field
-from typing import Dict
 
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
-from xrpl.models.transactions.transaction import Transaction
-from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
-from xrpl.models.xchain_bridge import XChainBridge
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class XChainAccountCreateCommit(Transaction):
+class ChannelVerify(Request):
     """
-    Represents a XChainAccountCreateCommit transaction on the XRP Ledger.
-    The XChainAccountCreateCommit transaction creates a new account on one of
-    the chains a bridge connects, which serves as the bridge entrance for that
-    chain.
+    The channel_verify method checks the validity of a
+    signature that can be used to redeem a specific amount of
+    XRP from a payment channel.
     """
 
-    xchain_bridge: XChainBridge = REQUIRED  # type: ignore
+    method: RequestMethod = field(default=RequestMethod.CHANNEL_VERIFY, init=False)
+    channel_id: str = REQUIRED  # type: ignore
     """
-    The bridge to create accounts for. This field is required.
+    This field is required.
 
     :meta hide-value:
     """
 
-    signature_reward: str = REQUIRED  # type: ignore
+    amount: str = REQUIRED  # type: ignore
     """
-    The amount, in XRP, to be used to reward the witness servers for providing
-    signatures. This must match the amount on the ``Bridge`` ledger object. This
-    field is required.
+    This field is required.
 
     :meta hide-value:
     """
 
-    destination: str = REQUIRED  # type: ignore
+    public_key: str = REQUIRED  # type: ignore
     """
-    The destination account on the destination chain. This field is required.
+    This field is required.
 
     :meta hide-value:
     """
 
-    amount: str = REQUIRED  # type: ignore
+    signature: str = REQUIRED  # type: ignore
     """
-    The amount, in XRP, to use for account creation. This must be greater than
-    or equal to the ``MinAccountCreateAmount`` specified in the ``Bridge``
-    ledger object. This field is required.
+    This field is required.
 
     :meta hide-value:
     """
-
-    transaction_type: TransactionType = field(
-        default=TransactionType.XCHAIN_ACCOUNT_CREATE_COMMIT,
-        init=False,
-    )
-
-    def _get_errors(self: XChainAccountCreateCommit) -> Dict[str, str]:
-        errors = super()._get_errors()
-
-        if self.signature_reward != REQUIRED and not self.signature_reward.isnumeric():
-            errors["signature_reward"] = "`signature_reward` must be numeric."
-
-        if self.amount != REQUIRED and not self.amount.isnumeric():
-            errors["amount"] = "`amount` must be numeric."
-
-        return errors
```

### Comparing `xrpl_py-2.1.0b0/xrpl/models/types.py` & `xrpl_py-2.2.0/xrpl/models/types.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/models/utils.py` & `xrpl_py-2.2.0/xrpl/models/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/transaction/__init__.py` & `xrpl_py-2.2.0/xrpl/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/transaction/main.py` & `xrpl_py-2.2.0/xrpl/transaction/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/transaction/multisign.py` & `xrpl_py-2.2.0/xrpl/transaction/multisign.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/transaction/reliable_submission.py` & `xrpl_py-2.2.0/xrpl/transaction/reliable_submission.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/__init__.py` & `xrpl_py-2.2.0/xrpl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/get_nftoken_id.py` & `xrpl_py-2.2.0/xrpl/utils/get_nftoken_id.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/parse_nftoken_id.py` & `xrpl_py-2.2.0/xrpl/utils/parse_nftoken_id.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/str_conversions.py` & `xrpl_py-2.2.0/xrpl/utils/str_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/time_conversions.py` & `xrpl_py-2.2.0/xrpl/utils/time_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_balance_changes.py` & `xrpl_py-2.2.0/xrpl/utils/txn_parser/get_balance_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_final_balances.py` & `xrpl_py-2.2.0/xrpl/utils/txn_parser/get_final_balances.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/get_order_book_changes.py` & `xrpl_py-2.2.0/xrpl/utils/txn_parser/get_order_book_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/__init__.py` & `xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/balance_parser.py` & `xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/balance_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/nodes.py` & `xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/nodes.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py` & `xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/order_book_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/parser.py` & `xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/parser.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/txn_parser/utils/types.py` & `xrpl_py-2.2.0/xrpl/utils/txn_parser/utils/types.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/utils/xrp_conversions.py` & `xrpl_py-2.2.0/xrpl/utils/xrp_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/wallet/main.py` & `xrpl_py-2.2.0/xrpl/wallet/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/xrpl/wallet/wallet_generation.py` & `xrpl_py-2.2.0/xrpl/wallet/wallet_generation.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.1.0b0/PKG-INFO` & `xrpl_py-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrpl-py
-Version: 2.1.0b0
+Version: 2.2.0
 Summary: A complete Python library for interacting with the XRP ledger
 Home-page: https://github.com/XRPLF/xrpl-py
 License: ISC
 Keywords: xrp,xrpl,cryptocurrency
 Author: Mayukha Vadari
 Author-email: mvadari@ripple.com
 Requires-Python: >=3.7,<4.0
@@ -28,54 +28,62 @@
 Project-URL: Repository, https://github.com/XRPLF/xrpl-py
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)
 
 # xrpl-py
 
-A pure Python implementation for interacting with the XRP Ledger, the `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing, by providing native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.
+A pure Python implementation for interacting with the [XRP Ledger](https://xrpl.org/). 
 
+The `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing. It also provides native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.
 
+As an example, this is how you would use this library to send a payment on testnet:
 
 ```py
-# create a network client
+from xrpl.account import get_balance
 from xrpl.clients import JsonRpcClient
+from xrpl.models import Payment, Tx
+from xrpl.transaction import submit_and_wait
+from xrpl.wallet import generate_faucet_wallet
+
+# Create a client to connect to the test network
 client = JsonRpcClient("https://s.altnet.rippletest.net:51234")
 
-# create a wallet on the testnet
-from xrpl.wallet import generate_faucet_wallet
-test_wallet = generate_faucet_wallet(client)
-print(test_wallet)
-public_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56
-private_key: -HIDDEN-
-address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
-
-# look up account info
-from xrpl.models import AccountInfo
-acct_info = AccountInfo(
-    account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
-    ledger_index="current",
-    queue=True,
-    strict=True,
+# Create two wallets to send money between on the test network
+wallet1 = generate_faucet_wallet(client, debug=True)
+wallet2 = generate_faucet_wallet(client, debug=True)
+
+# Both balances should be zero since nothing has been sent yet
+print("Balances of wallets before Payment tx")
+print(get_balance(wallet1.address, client))
+print(get_balance(wallet2.address, client))
+
+# Create a Payment transaction from wallet1 to wallet2
+payment_tx = Payment(
+    account=wallet1.address,
+    amount="1000",
+    destination=wallet2.address,
 )
-response = client.request(acct_info)
-result = response.result
-import json
-print(json.dumps(result["account_data"], indent=4, sort_keys=True))
-# {
-#     "Account": "rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
-#     "Balance": "1000000000",
-#     "Flags": 0,
-#     "LedgerEntryType": "AccountRoot",
-#     "OwnerCount": 0,
-#     "PreviousTxnID": "73CD4A37537A992270AAC8472F6681F44E400CBDE04EC8983C34B519F56AB107",
-#     "PreviousTxnLgrSeq": 16233962,
-#     "Sequence": 16233962,
-#     "index": "FD66EC588B52712DCE74831DCB08B24157DC3198C29A0116AA64D310A58512D7"
-# }
+
+# Submit the payment to the network and wait to see a response
+#   Behind the scenes, this fills in fields which can be looked up automatically like the fee.
+#   It also signs the transaction with wallet1 to prove you own the account you're paying from.
+payment_response = submit_and_wait(payment_tx, client, wallet1)
+print("Transaction was submitted")
+
+# Create a "Tx" request to look up the transaction on the ledger
+tx_response = client.request(Tx(transaction=payment_response.result["hash"]))
+
+# Check whether the transaction was actually validated on ledger
+print("Validated:", tx_response.result["validated"])
+
+# Check balances after 1000 drops (.001 XRP) was sent from wallet1 to wallet2
+print("Balances of wallets after Payment tx:")
+print(get_balance(wallet1.address, client))
+print(get_balance(wallet2.address, client))
 ```
 
 [![Downloads](https://pepy.tech/badge/xrpl-py/month)](https://pepy.tech/project/xrpl-py/month)
 [![Contributors](https://img.shields.io/github/contributors/xpring-eng/xrpl-py.svg)](https://github.com/xpring-eng/xrpl-py/graphs/contributors)
 
 ## Installation and supported versions
 
@@ -346,14 +354,17 @@
         is_test_network=True,
     )
 )
 print(testnet_xaddress)
 # T7QDemmxnuN7a52A62nx2fxGPWcRahLCf3qaswfrsNW9Lps
 ```
 
+## Migrating
+
+If you're currently using `xrpl-py` version 1, you can use [this guide to migrate to v2](https://xrpl.org/blog/2023/xrpl-py-2.0-release.html).
 
 ## Contributing
 
 If you want to contribute to this project, see [CONTRIBUTING.md].
 
 ### Mailing Lists
```

