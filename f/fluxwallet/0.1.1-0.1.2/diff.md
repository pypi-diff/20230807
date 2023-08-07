# Comparing `tmp/fluxwallet-0.1.1.tar.gz` & `tmp/fluxwallet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxwallet-0.1.1.tar", max compression
+gzip compressed data, was "fluxwallet-0.1.2.tar", max compression
```

## Comparing `fluxwallet-0.1.1.tar` & `fluxwallet-0.1.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1488 2023-08-06 19:16:07.377691 fluxwallet-0.1.1/LICENSE
--rw-r--r--   0        0        0      122 2023-08-06 19:16:46.490951 fluxwallet-0.1.1/README.md
--rw-r--r--   0        0        0     1178 2023-07-15 06:48:47.681778 fluxwallet-0.1.1/fluxwallet/__init__.py
--rw-r--r--   0        0        0    26527 2023-08-06 19:22:11.578367 fluxwallet-0.1.1/fluxwallet/blocks.py
--rw-r--r--   0        0        0        5 2023-08-06 19:45:44.752788 fluxwallet-0.1.1/fluxwallet/config/VERSION
--rw-r--r--   0        0        0      976 2023-02-23 22:29:07.335521 fluxwallet-0.1.1/fluxwallet/config/__init__.py
--rw-r--r--   0        0        0    13610 2023-07-15 06:48:47.683549 fluxwallet-0.1.1/fluxwallet/config/config.py
--rw-r--r--   0        0        0     2773 2023-02-23 22:29:07.335272 fluxwallet-0.1.1/fluxwallet/config/opcodes.py
--rw-r--r--   0        0        0     1501 2023-02-23 22:29:07.337318 fluxwallet-0.1.1/fluxwallet/config/secp256k1.py
--rw-r--r--   0        0        0     2268 2023-07-15 06:48:47.684240 fluxwallet-0.1.1/fluxwallet/data/config.ini
--rw-r--r--   0        0        0     1821 2023-02-23 22:29:07.345332 fluxwallet-0.1.1/fluxwallet/data/config.ini.unittest
--rw-r--r--   0        0        0    18913 2023-02-23 22:29:07.346897 fluxwallet-0.1.1/fluxwallet/data/networks.json
--rw-r--r--   0        0        0    11174 2023-02-23 22:29:07.348271 fluxwallet-0.1.1/fluxwallet/data/providers.examples.json
--rw-r--r--   0        0        0    11938 2023-02-23 22:29:07.346345 fluxwallet-0.1.1/fluxwallet/data/providers.json
--rw-r--r--   0        0        0    12858 2023-02-23 22:29:07.347348 fluxwallet-0.1.1/fluxwallet/data/providers.old.json
--rw-r--r--   0        0        0    26648 2023-07-15 06:48:47.684740 fluxwallet-0.1.1/fluxwallet/db.py
--rw-r--r--   0        0        0    11102 2023-08-06 19:22:11.458158 fluxwallet-0.1.1/fluxwallet/db_cache.py
--rw-r--r--   0        0        0    31155 2023-08-06 19:22:11.435664 fluxwallet-0.1.1/fluxwallet/db_new.py
--rw-r--r--   0        0        0    36470 2023-07-18 09:52:07.945700 fluxwallet-0.1.1/fluxwallet/encoding.py
--rw-r--r--   0        0        0    12246 2023-07-15 06:48:47.687032 fluxwallet-0.1.1/fluxwallet/flux_transaction.py
--rw-r--r--   0        0        0   104013 2023-07-15 06:48:47.688171 fluxwallet-0.1.1/fluxwallet/keys.py
--rw-r--r--   0        0        0     4181 2023-07-15 06:48:47.688896 fluxwallet-0.1.1/fluxwallet/main.py
--rw-r--r--   0        0        0    10073 2023-07-15 06:48:47.689606 fluxwallet-0.1.1/fluxwallet/mnemonic.py
--rw-r--r--   0        0        0    10870 2023-07-15 06:48:47.690030 fluxwallet-0.1.1/fluxwallet/networks.py
--rw-r--r--   0        0        0      657 2023-02-23 22:29:07.338292 fluxwallet-0.1.1/fluxwallet/pyproject.toml
--rw-r--r--   0        0        0    42380 2023-02-23 22:29:07.344038 fluxwallet-0.1.1/fluxwallet/scripts.py
--rw-r--r--   0        0        0     1688 2023-02-23 22:29:07.352259 fluxwallet-0.1.1/fluxwallet/services/__init__.py
--rw-r--r--   0        0        0     7465 2023-02-23 22:29:07.363317 fluxwallet-0.1.1/fluxwallet/services/authproxy.py
--rw-r--r--   0        0        0     5544 2023-07-15 06:48:47.690785 fluxwallet-0.1.1/fluxwallet/services/baseclient.py
--rw-r--r--   0        0        0     8956 2023-07-15 06:48:47.691571 fluxwallet-0.1.1/fluxwallet/services/bcoin.py
--rw-r--r--   0        0        0    10124 2023-07-15 06:48:47.692183 fluxwallet-0.1.1/fluxwallet/services/bitaps.py
--rw-r--r--   0        0        0    14566 2023-07-15 06:48:47.692700 fluxwallet-0.1.1/fluxwallet/services/bitcoind.py
--rw-r--r--   0        0        0     4276 2023-07-15 06:48:47.693408 fluxwallet-0.1.1/fluxwallet/services/bitcoinlibtest.py
--rw-r--r--   0        0        0     3871 2023-07-15 06:48:47.693828 fluxwallet-0.1.1/fluxwallet/services/bitflyer.py
--rw-r--r--   0        0        0     8548 2023-07-15 06:48:47.694517 fluxwallet-0.1.1/fluxwallet/services/bitgo.py
--rw-r--r--   0        0        0     8305 2023-07-15 06:48:47.695190 fluxwallet-0.1.1/fluxwallet/services/blockchaininfo.py
--rw-r--r--   0        0        0    11632 2023-07-15 06:48:47.695980 fluxwallet-0.1.1/fluxwallet/services/blockchair.py
--rw-r--r--   0        0        0     9697 2023-07-15 06:48:47.696430 fluxwallet-0.1.1/fluxwallet/services/blockcypher.py
--rw-r--r--   0        0        0    10014 2023-07-15 06:48:47.697175 fluxwallet-0.1.1/fluxwallet/services/blocksmurfer.py
--rw-r--r--   0        0        0    11214 2023-07-15 06:48:47.697596 fluxwallet-0.1.1/fluxwallet/services/blockstream.py
--rw-r--r--   0        0        0     8038 2023-07-15 06:48:47.698276 fluxwallet-0.1.1/fluxwallet/services/chainso.py
--rw-r--r--   0        0        0     6617 2023-07-15 06:48:47.699096 fluxwallet-0.1.1/fluxwallet/services/cryptoid.py
--rw-r--r--   0        0        0    11149 2023-07-15 06:48:47.699788 fluxwallet-0.1.1/fluxwallet/services/dashd.py
--rw-r--r--   0        0        0     9930 2023-07-15 06:48:47.700474 fluxwallet-0.1.1/fluxwallet/services/dogecoind.py
--rw-r--r--   0        0        0     8440 2023-07-15 06:48:47.701139 fluxwallet-0.1.1/fluxwallet/services/insightdash.py
--rw-r--r--   0        0        0     8757 2023-07-15 06:48:47.701506 fluxwallet-0.1.1/fluxwallet/services/litecoinblockexplorer.py
--rw-r--r--   0        0        0    14616 2023-07-15 06:48:47.701928 fluxwallet-0.1.1/fluxwallet/services/litecoind.py
--rw-r--r--   0        0        0     8496 2023-07-15 06:48:47.702300 fluxwallet-0.1.1/fluxwallet/services/litecoreio.py
--rw-r--r--   0        0        0     9911 2023-07-15 06:48:47.702991 fluxwallet-0.1.1/fluxwallet/services/mempool.py
--rw-r--r--   0        0        0    15467 2023-08-06 19:22:11.777530 fluxwallet-0.1.1/fluxwallet/services/runonflux.py
--rw-r--r--   0        0        0    63045 2023-08-06 19:22:11.726164 fluxwallet-0.1.1/fluxwallet/services/services.py
--rw-r--r--   0        0        0      860 2023-02-23 22:29:07.332236 fluxwallet-0.1.1/fluxwallet/tools/__init__.py
--rw-r--r--   0        0        0    21208 2023-08-06 19:22:11.600656 fluxwallet-0.1.1/fluxwallet/tools/clw.py
--rw-r--r--   0        0        0      912 2023-02-23 22:29:07.331711 fluxwallet-0.1.1/fluxwallet/tools/mnemonic_key_create.py
--rw-r--r--   0        0        0     1789 2023-07-15 06:48:47.705851 fluxwallet-0.1.1/fluxwallet/tools/sign_raw.py
--rw-r--r--   0        0        0     5581 2023-08-06 19:22:11.607966 fluxwallet-0.1.1/fluxwallet/tools/wallet_multisig_2of3.py
--rw-r--r--   0        0        0   105100 2023-08-06 19:22:11.527807 fluxwallet-0.1.1/fluxwallet/transactions.py
--rw-r--r--   0        0        0    18023 2023-06-19 07:46:39.603630 fluxwallet-0.1.1/fluxwallet/values.py
--rw-r--r--   0        0        0      335 2023-08-06 19:22:11.639567 fluxwallet-0.1.1/fluxwallet/wallet/__init__.py
--rw-r--r--   0        0        0      269 2023-07-18 13:43:47.906642 fluxwallet-0.1.1/fluxwallet/wallet/errors.py
--rw-r--r--   0        0        0    11262 2023-08-06 19:22:11.658490 fluxwallet-0.1.1/fluxwallet/wallet/helpers.py
--rw-r--r--   0        0        0   192780 2023-08-06 19:22:11.686653 fluxwallet-0.1.1/fluxwallet/wallet/wallet.py
--rw-r--r--   0        0        0    15470 2023-07-15 07:25:58.876062 fluxwallet-0.1.1/fluxwallet/wallet/wallet_key.py
--rw-r--r--   0        0        0    29547 2023-08-06 19:22:11.694119 fluxwallet-0.1.1/fluxwallet/wallet/wallet_transaction.py
--rw-r--r--   0        0        0    34652 2023-08-06 19:22:11.649043 fluxwallet-0.1.1/fluxwallet/wallet/wallet_transaction_old.py
--rw-r--r--   0        0        0   224929 2023-07-15 06:48:47.711692 fluxwallet-0.1.1/fluxwallet/wallets.py
--rw-r--r--   0        0        0    12026 2023-07-15 06:48:47.712013 fluxwallet-0.1.1/fluxwallet/wallets_new.py
--rw-r--r--   0        0        0     8192 2023-02-23 22:29:07.329820 fluxwallet-0.1.1/fluxwallet/wordlist/chinese_simplified.txt
--rw-r--r--   0        0        0     8192 2023-02-23 22:29:07.328782 fluxwallet-0.1.1/fluxwallet/wordlist/chinese_traditional.txt
--rw-r--r--   0        0        0    16254 2023-02-23 22:29:07.331114 fluxwallet-0.1.1/fluxwallet/wordlist/dutch.txt
--rw-r--r--   0        0        0    13116 2023-02-23 22:29:07.330170 fluxwallet-0.1.1/fluxwallet/wordlist/english.txt
--rw-r--r--   0        0        0    16777 2023-02-23 22:29:07.329539 fluxwallet-0.1.1/fluxwallet/wordlist/french.txt
--rw-r--r--   0        0        0    16033 2023-02-23 22:29:07.330837 fluxwallet-0.1.1/fluxwallet/wordlist/italian.txt
--rw-r--r--   0        0        0    26423 2023-02-23 22:29:07.329237 fluxwallet-0.1.1/fluxwallet/wordlist/japanese.txt
--rw-r--r--   0        0        0    13996 2023-02-23 22:29:07.330546 fluxwallet-0.1.1/fluxwallet/wordlist/spanish.txt
--rw-r--r--   0        0        0      649 2023-08-06 19:45:53.455943 fluxwallet-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 fluxwallet-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-08-06 19:16:07.377691 fluxwallet-0.1.2/LICENSE
+-rw-r--r--   0        0        0      122 2023-08-06 19:16:46.490951 fluxwallet-0.1.2/README.md
+-rw-r--r--   0        0        0     1183 2023-08-06 19:56:55.903976 fluxwallet-0.1.2/fluxwallet/__init__.py
+-rw-r--r--   0        0        0    26527 2023-08-06 19:22:11.578367 fluxwallet-0.1.2/fluxwallet/blocks.py
+-rw-r--r--   0        0        0        5 2023-08-06 20:17:09.856137 fluxwallet-0.1.2/fluxwallet/config/VERSION
+-rw-r--r--   0        0        0      976 2023-02-23 22:29:07.335521 fluxwallet-0.1.2/fluxwallet/config/__init__.py
+-rw-r--r--   0        0        0    13610 2023-07-15 06:48:47.683549 fluxwallet-0.1.2/fluxwallet/config/config.py
+-rw-r--r--   0        0        0     2773 2023-02-23 22:29:07.335272 fluxwallet-0.1.2/fluxwallet/config/opcodes.py
+-rw-r--r--   0        0        0     1501 2023-02-23 22:29:07.337318 fluxwallet-0.1.2/fluxwallet/config/secp256k1.py
+-rw-r--r--   0        0        0     2268 2023-07-15 06:48:47.684240 fluxwallet-0.1.2/fluxwallet/data/config.ini
+-rw-r--r--   0        0        0     1821 2023-02-23 22:29:07.345332 fluxwallet-0.1.2/fluxwallet/data/config.ini.unittest
+-rw-r--r--   0        0        0    18913 2023-02-23 22:29:07.346897 fluxwallet-0.1.2/fluxwallet/data/networks.json
+-rw-r--r--   0        0        0    11174 2023-02-23 22:29:07.348271 fluxwallet-0.1.2/fluxwallet/data/providers.examples.json
+-rw-r--r--   0        0        0    11938 2023-02-23 22:29:07.346345 fluxwallet-0.1.2/fluxwallet/data/providers.json
+-rw-r--r--   0        0        0    12858 2023-02-23 22:29:07.347348 fluxwallet-0.1.2/fluxwallet/data/providers.old.json
+-rw-r--r--   0        0        0    26648 2023-07-15 06:48:47.684740 fluxwallet-0.1.2/fluxwallet/db.py
+-rw-r--r--   0        0        0    11102 2023-08-06 19:22:11.458158 fluxwallet-0.1.2/fluxwallet/db_cache.py
+-rw-r--r--   0        0        0    31155 2023-08-06 19:22:11.435664 fluxwallet-0.1.2/fluxwallet/db_new.py
+-rw-r--r--   0        0        0    36470 2023-07-18 09:52:07.945700 fluxwallet-0.1.2/fluxwallet/encoding.py
+-rw-r--r--   0        0        0    12246 2023-07-15 06:48:47.687032 fluxwallet-0.1.2/fluxwallet/flux_transaction.py
+-rw-r--r--   0        0        0   104013 2023-07-15 06:48:47.688171 fluxwallet-0.1.2/fluxwallet/keys.py
+-rw-r--r--   0        0        0     4181 2023-07-15 06:48:47.688896 fluxwallet-0.1.2/fluxwallet/main.py
+-rw-r--r--   0        0        0    10073 2023-07-15 06:48:47.689606 fluxwallet-0.1.2/fluxwallet/mnemonic.py
+-rw-r--r--   0        0        0    10870 2023-07-15 06:48:47.690030 fluxwallet-0.1.2/fluxwallet/networks.py
+-rw-r--r--   0        0        0      657 2023-02-23 22:29:07.338292 fluxwallet-0.1.2/fluxwallet/pyproject.toml
+-rw-r--r--   0        0        0    42380 2023-02-23 22:29:07.344038 fluxwallet-0.1.2/fluxwallet/scripts.py
+-rw-r--r--   0        0        0     1688 2023-02-23 22:29:07.352259 fluxwallet-0.1.2/fluxwallet/services/__init__.py
+-rw-r--r--   0        0        0     7465 2023-02-23 22:29:07.363317 fluxwallet-0.1.2/fluxwallet/services/authproxy.py
+-rw-r--r--   0        0        0     5544 2023-07-15 06:48:47.690785 fluxwallet-0.1.2/fluxwallet/services/baseclient.py
+-rw-r--r--   0        0        0     8956 2023-07-15 06:48:47.691571 fluxwallet-0.1.2/fluxwallet/services/bcoin.py
+-rw-r--r--   0        0        0    10124 2023-07-15 06:48:47.692183 fluxwallet-0.1.2/fluxwallet/services/bitaps.py
+-rw-r--r--   0        0        0    14566 2023-07-15 06:48:47.692700 fluxwallet-0.1.2/fluxwallet/services/bitcoind.py
+-rw-r--r--   0        0        0     4276 2023-07-15 06:48:47.693408 fluxwallet-0.1.2/fluxwallet/services/bitcoinlibtest.py
+-rw-r--r--   0        0        0     3871 2023-07-15 06:48:47.693828 fluxwallet-0.1.2/fluxwallet/services/bitflyer.py
+-rw-r--r--   0        0        0     8548 2023-07-15 06:48:47.694517 fluxwallet-0.1.2/fluxwallet/services/bitgo.py
+-rw-r--r--   0        0        0     8305 2023-07-15 06:48:47.695190 fluxwallet-0.1.2/fluxwallet/services/blockchaininfo.py
+-rw-r--r--   0        0        0    11632 2023-07-15 06:48:47.695980 fluxwallet-0.1.2/fluxwallet/services/blockchair.py
+-rw-r--r--   0        0        0     9697 2023-07-15 06:48:47.696430 fluxwallet-0.1.2/fluxwallet/services/blockcypher.py
+-rw-r--r--   0        0        0    10014 2023-07-15 06:48:47.697175 fluxwallet-0.1.2/fluxwallet/services/blocksmurfer.py
+-rw-r--r--   0        0        0    11214 2023-07-15 06:48:47.697596 fluxwallet-0.1.2/fluxwallet/services/blockstream.py
+-rw-r--r--   0        0        0     8038 2023-07-15 06:48:47.698276 fluxwallet-0.1.2/fluxwallet/services/chainso.py
+-rw-r--r--   0        0        0     6617 2023-07-15 06:48:47.699096 fluxwallet-0.1.2/fluxwallet/services/cryptoid.py
+-rw-r--r--   0        0        0    11149 2023-07-15 06:48:47.699788 fluxwallet-0.1.2/fluxwallet/services/dashd.py
+-rw-r--r--   0        0        0     9930 2023-07-15 06:48:47.700474 fluxwallet-0.1.2/fluxwallet/services/dogecoind.py
+-rw-r--r--   0        0        0     8440 2023-07-15 06:48:47.701139 fluxwallet-0.1.2/fluxwallet/services/insightdash.py
+-rw-r--r--   0        0        0     8757 2023-07-15 06:48:47.701506 fluxwallet-0.1.2/fluxwallet/services/litecoinblockexplorer.py
+-rw-r--r--   0        0        0    14616 2023-07-15 06:48:47.701928 fluxwallet-0.1.2/fluxwallet/services/litecoind.py
+-rw-r--r--   0        0        0     8496 2023-07-15 06:48:47.702300 fluxwallet-0.1.2/fluxwallet/services/litecoreio.py
+-rw-r--r--   0        0        0     9911 2023-07-15 06:48:47.702991 fluxwallet-0.1.2/fluxwallet/services/mempool.py
+-rw-r--r--   0        0        0    15467 2023-08-06 19:22:11.777530 fluxwallet-0.1.2/fluxwallet/services/runonflux.py
+-rw-r--r--   0        0        0    63045 2023-08-06 19:22:11.726164 fluxwallet-0.1.2/fluxwallet/services/services.py
+-rw-r--r--   0        0        0      860 2023-02-23 22:29:07.332236 fluxwallet-0.1.2/fluxwallet/tools/__init__.py
+-rw-r--r--   0        0        0    21208 2023-08-06 19:22:11.600656 fluxwallet-0.1.2/fluxwallet/tools/clw.py
+-rw-r--r--   0        0        0      912 2023-02-23 22:29:07.331711 fluxwallet-0.1.2/fluxwallet/tools/mnemonic_key_create.py
+-rw-r--r--   0        0        0     1789 2023-07-15 06:48:47.705851 fluxwallet-0.1.2/fluxwallet/tools/sign_raw.py
+-rw-r--r--   0        0        0     5581 2023-08-06 19:22:11.607966 fluxwallet-0.1.2/fluxwallet/tools/wallet_multisig_2of3.py
+-rw-r--r--   0        0        0   105100 2023-08-06 19:22:11.527807 fluxwallet-0.1.2/fluxwallet/transactions.py
+-rw-r--r--   0        0        0    18023 2023-06-19 07:46:39.603630 fluxwallet-0.1.2/fluxwallet/values.py
+-rw-r--r--   0        0        0      218 2023-08-06 19:59:52.997937 fluxwallet-0.1.2/fluxwallet/wallet/__init__.py
+-rw-r--r--   0        0        0      269 2023-07-18 13:43:47.906642 fluxwallet-0.1.2/fluxwallet/wallet/errors.py
+-rw-r--r--   0        0        0    11262 2023-08-06 19:22:11.658490 fluxwallet-0.1.2/fluxwallet/wallet/helpers.py
+-rw-r--r--   0        0        0   192780 2023-08-06 19:22:11.686653 fluxwallet-0.1.2/fluxwallet/wallet/wallet.py
+-rw-r--r--   0        0        0    15470 2023-07-15 07:25:58.876062 fluxwallet-0.1.2/fluxwallet/wallet/wallet_key.py
+-rw-r--r--   0        0        0    29547 2023-08-06 19:22:11.694119 fluxwallet-0.1.2/fluxwallet/wallet/wallet_transaction.py
+-rw-r--r--   0        0        0    34652 2023-08-06 19:22:11.649043 fluxwallet-0.1.2/fluxwallet/wallet/wallet_transaction_old.py
+-rw-r--r--   0        0        0   224929 2023-07-15 06:48:47.711692 fluxwallet-0.1.2/fluxwallet/wallets.py
+-rw-r--r--   0        0        0    12026 2023-07-15 06:48:47.712013 fluxwallet-0.1.2/fluxwallet/wallets_new.py
+-rw-r--r--   0        0        0     8192 2023-02-23 22:29:07.329820 fluxwallet-0.1.2/fluxwallet/wordlist/chinese_simplified.txt
+-rw-r--r--   0        0        0     8192 2023-02-23 22:29:07.328782 fluxwallet-0.1.2/fluxwallet/wordlist/chinese_traditional.txt
+-rw-r--r--   0        0        0    16254 2023-02-23 22:29:07.331114 fluxwallet-0.1.2/fluxwallet/wordlist/dutch.txt
+-rw-r--r--   0        0        0    13116 2023-02-23 22:29:07.330170 fluxwallet-0.1.2/fluxwallet/wordlist/english.txt
+-rw-r--r--   0        0        0    16777 2023-02-23 22:29:07.329539 fluxwallet-0.1.2/fluxwallet/wordlist/french.txt
+-rw-r--r--   0        0        0    16033 2023-02-23 22:29:07.330837 fluxwallet-0.1.2/fluxwallet/wordlist/italian.txt
+-rw-r--r--   0        0        0    26423 2023-02-23 22:29:07.329237 fluxwallet-0.1.2/fluxwallet/wordlist/japanese.txt
+-rw-r--r--   0        0        0    13996 2023-02-23 22:29:07.330546 fluxwallet-0.1.2/fluxwallet/wordlist/spanish.txt
+-rw-r--r--   0        0        0      649 2023-08-06 20:17:20.023127 fluxwallet-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 fluxwallet-0.1.2/PKG-INFO
```

### Comparing `fluxwallet-0.1.1/LICENSE` & `fluxwallet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/__init__.py` & `fluxwallet-0.1.2/fluxwallet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 # import fluxwallet.blocks
 import fluxwallet.encoding
 import fluxwallet.keys
 import fluxwallet.mnemonic
-import fluxwallet.tools
+
+# import fluxwallet.tools
 import fluxwallet.transactions
 import fluxwallet.values
 import fluxwallet.wallet
 
 __all__ = [
     "keys",
     "transactions",
     "wallets",
     "encoding",
     "mnemonic",
-    "tools",
+    # "tools",
     "blocks",
     "values",
 ]
```

### Comparing `fluxwallet-0.1.1/fluxwallet/blocks.py` & `fluxwallet-0.1.2/fluxwallet/blocks.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/config/__init__.py` & `fluxwallet-0.1.2/fluxwallet/config/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/config/config.py` & `fluxwallet-0.1.2/fluxwallet/config/config.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/config/opcodes.py` & `fluxwallet-0.1.2/fluxwallet/config/opcodes.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/config/secp256k1.py` & `fluxwallet-0.1.2/fluxwallet/config/secp256k1.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/data/config.ini` & `fluxwallet-0.1.2/fluxwallet/data/config.ini`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/data/config.ini.unittest` & `fluxwallet-0.1.2/fluxwallet/data/config.ini.unittest`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/data/networks.json` & `fluxwallet-0.1.2/fluxwallet/data/networks.json`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/data/providers.examples.json` & `fluxwallet-0.1.2/fluxwallet/data/providers.examples.json`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/data/providers.json` & `fluxwallet-0.1.2/fluxwallet/data/providers.json`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/data/providers.old.json` & `fluxwallet-0.1.2/fluxwallet/data/providers.old.json`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/db.py` & `fluxwallet-0.1.2/fluxwallet/db.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/db_cache.py` & `fluxwallet-0.1.2/fluxwallet/db_cache.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/db_new.py` & `fluxwallet-0.1.2/fluxwallet/db_new.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/encoding.py` & `fluxwallet-0.1.2/fluxwallet/encoding.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/flux_transaction.py` & `fluxwallet-0.1.2/fluxwallet/flux_transaction.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/keys.py` & `fluxwallet-0.1.2/fluxwallet/keys.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/main.py` & `fluxwallet-0.1.2/fluxwallet/main.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/mnemonic.py` & `fluxwallet-0.1.2/fluxwallet/mnemonic.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/networks.py` & `fluxwallet-0.1.2/fluxwallet/networks.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/pyproject.toml` & `fluxwallet-0.1.2/fluxwallet/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/scripts.py` & `fluxwallet-0.1.2/fluxwallet/scripts.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/__init__.py` & `fluxwallet-0.1.2/fluxwallet/services/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/authproxy.py` & `fluxwallet-0.1.2/fluxwallet/services/authproxy.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/baseclient.py` & `fluxwallet-0.1.2/fluxwallet/services/baseclient.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/bcoin.py` & `fluxwallet-0.1.2/fluxwallet/services/bcoin.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/bitaps.py` & `fluxwallet-0.1.2/fluxwallet/services/bitaps.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/bitcoind.py` & `fluxwallet-0.1.2/fluxwallet/services/bitcoind.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/bitcoinlibtest.py` & `fluxwallet-0.1.2/fluxwallet/services/bitcoinlibtest.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/bitflyer.py` & `fluxwallet-0.1.2/fluxwallet/services/bitflyer.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/bitgo.py` & `fluxwallet-0.1.2/fluxwallet/services/bitgo.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/blockchaininfo.py` & `fluxwallet-0.1.2/fluxwallet/services/blockchaininfo.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/blockchair.py` & `fluxwallet-0.1.2/fluxwallet/services/blockchair.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/blockcypher.py` & `fluxwallet-0.1.2/fluxwallet/services/blockcypher.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/blocksmurfer.py` & `fluxwallet-0.1.2/fluxwallet/services/blocksmurfer.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/blockstream.py` & `fluxwallet-0.1.2/fluxwallet/services/blockstream.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/chainso.py` & `fluxwallet-0.1.2/fluxwallet/services/chainso.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/cryptoid.py` & `fluxwallet-0.1.2/fluxwallet/services/cryptoid.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/dashd.py` & `fluxwallet-0.1.2/fluxwallet/services/dashd.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/dogecoind.py` & `fluxwallet-0.1.2/fluxwallet/services/dogecoind.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/insightdash.py` & `fluxwallet-0.1.2/fluxwallet/services/insightdash.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/litecoinblockexplorer.py` & `fluxwallet-0.1.2/fluxwallet/services/litecoinblockexplorer.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/litecoind.py` & `fluxwallet-0.1.2/fluxwallet/services/litecoind.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/litecoreio.py` & `fluxwallet-0.1.2/fluxwallet/services/litecoreio.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/mempool.py` & `fluxwallet-0.1.2/fluxwallet/services/mempool.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/runonflux.py` & `fluxwallet-0.1.2/fluxwallet/services/runonflux.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/services/services.py` & `fluxwallet-0.1.2/fluxwallet/services/services.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/tools/__init__.py` & `fluxwallet-0.1.2/fluxwallet/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/tools/clw.py` & `fluxwallet-0.1.2/fluxwallet/tools/clw.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/tools/mnemonic_key_create.py` & `fluxwallet-0.1.2/fluxwallet/tools/mnemonic_key_create.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/tools/sign_raw.py` & `fluxwallet-0.1.2/fluxwallet/tools/sign_raw.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/tools/wallet_multisig_2of3.py` & `fluxwallet-0.1.2/fluxwallet/tools/wallet_multisig_2of3.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/transactions.py` & `fluxwallet-0.1.2/fluxwallet/transactions.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/values.py` & `fluxwallet-0.1.2/fluxwallet/values.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wallet/helpers.py` & `fluxwallet-0.1.2/fluxwallet/wallet/helpers.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wallet/wallet.py` & `fluxwallet-0.1.2/fluxwallet/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wallet/wallet_key.py` & `fluxwallet-0.1.2/fluxwallet/wallet/wallet_key.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wallet/wallet_transaction.py` & `fluxwallet-0.1.2/fluxwallet/wallet/wallet_transaction.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wallet/wallet_transaction_old.py` & `fluxwallet-0.1.2/fluxwallet/wallet/wallet_transaction_old.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wallets.py` & `fluxwallet-0.1.2/fluxwallet/wallets.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wallets_new.py` & `fluxwallet-0.1.2/fluxwallet/wallets_new.py`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wordlist/chinese_simplified.txt` & `fluxwallet-0.1.2/fluxwallet/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wordlist/chinese_traditional.txt` & `fluxwallet-0.1.2/fluxwallet/wordlist/chinese_traditional.txt`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wordlist/dutch.txt` & `fluxwallet-0.1.2/fluxwallet/wordlist/dutch.txt`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wordlist/english.txt` & `fluxwallet-0.1.2/fluxwallet/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wordlist/french.txt` & `fluxwallet-0.1.2/fluxwallet/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wordlist/italian.txt` & `fluxwallet-0.1.2/fluxwallet/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wordlist/japanese.txt` & `fluxwallet-0.1.2/fluxwallet/wordlist/japanese.txt`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/fluxwallet/wordlist/spanish.txt` & `fluxwallet-0.1.2/fluxwallet/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `fluxwallet-0.1.1/pyproject.toml` & `fluxwallet-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "fluxwallet"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Wallet implementation for Flux"
 authors = ["David White <dr.white.nz@gmail.com>"]
 license = "bsd 3-clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 # requests = "^2.25.0"
 httpx = "^0.24.1"
 aiosqlite = "^0.19.0"
 fastecdsa = { version = "^2.2.1", markers = "sys_platform != 'win32'" }
 ecdsa = { version = "^0.17", platform = "win32" }
 pycryptodome = "^3.14.1"
-SQLAlchemy = "^1.4.28"
+SQLAlchemy = "^2.0.19"
 numpy = "^1.21.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fluxwallet-0.1.1/PKG-INFO` & `fluxwallet-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fluxwallet
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Wallet implementation for Flux
 License: bsd 3-clause
 Author: David White
 Author-email: dr.white.nz@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: SQLAlchemy (>=1.4.28,<2.0.0)
+Requires-Dist: SQLAlchemy (>=2.0.19,<3.0.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: ecdsa (>=0.17,<0.18) ; sys_platform == "win32"
 Requires-Dist: fastecdsa (>=2.2.1,<3.0.0) ; sys_platform != "win32"
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pycryptodome (>=3.14.1,<4.0.0)
 Description-Content-Type: text/markdown
```

