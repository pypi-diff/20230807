# Comparing `tmp/symbol-shoestring-0.0.5.tar.gz` & `tmp/symbol_shoestring-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol-shoestring-0.0.5.tar", max compression
+gzip compressed data, was "symbol_shoestring-0.0.6.tar", max compression
```

## Comparing `symbol-shoestring-0.0.5.tar` & `symbol_shoestring-0.0.6.tar`

### file list

```diff
@@ -1,87 +1,86 @@
--rw-r--r--   0        0        0     9931 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/README.md
--rw-r--r--   0        0        0      879 2023-08-01 17:01:59.866488 symbol-shoestring-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/__init__.py
--rw-r--r--   0        0        0     1937 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/__main__.py
--rw-r--r--   0        0        0        0 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/__init__.py
--rw-r--r--   0        0        0     1552 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/announce_transaction.py
--rw-r--r--   0        0        0     2475 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/health.py
--rw-r--r--   0        0        0     1262 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/import_bootstrap.py
--rw-r--r--   0        0        0     1025 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/init.py
--rw-r--r--   0        0        0     1692 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/min_cosignatures_count.py
--rw-r--r--   0        0        0     1733 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/pemtool.py
--rw-r--r--   0        0        0     1569 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/renew_certificates.py
--rw-r--r--   0        0        0     5270 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/renew_voting_keys.py
--rw-r--r--   0        0        0     3071 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/reset_data.py
--rw-r--r--   0        0        0     5330 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/setup.py
--rw-r--r--   0        0        0     3332 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/signer.py
--rw-r--r--   0        0        0     2246 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/upgrade.py
--rw-r--r--   0        0        0        0 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/__init__.py
--rw-r--r--   0        0        0      594 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/peer_api.py
--rw-r--r--   0        0        0     3586 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/peer_certificate.py
--rw-r--r--   0        0        0      644 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/rest_api.py
--rw-r--r--   0        0        0     2985 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/rest_https_certificate.py
--rw-r--r--   0        0        0     1686 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/voting_keys.py
--rw-r--r--   0        0        0     1573 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/websockets.py
--rw-r--r--   0        0        0     5055 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/CertificateFactory.py
--rw-r--r--   0        0        0     3233 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/ConfigurationManager.py
--rw-r--r--   0        0        0     1656 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/FileDownloader.py
--rw-r--r--   0        0        0      360 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/FileTemplater.py
--rw-r--r--   0        0        0     1961 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/HarvesterConfigurator.py
--rw-r--r--   0        0        0      830 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/HeightGrouping.py
--rw-r--r--   0        0        0     3089 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/LinkTransactionBuilder.py
--rw-r--r--   0        0        0      655 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/MultisigAnalyzer.py
--rw-r--r--   0        0        0     2789 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/NodeDownloader.py
--rw-r--r--   0        0        0      578 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/NodeFeatures.py
--rw-r--r--   0        0        0     1412 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/NodewatchClient.py
--rw-r--r--   0        0        0     1381 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/OpensslExecutor.py
--rw-r--r--   0        0        0     3060 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/PackageResolver.py
--rw-r--r--   0        0        0     2139 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/PeerDownloader.py
--rw-r--r--   0        0        0     2372 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/PemUtils.py
--rw-r--r--   0        0        0    12793 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/Preparer.py
--rw-r--r--   0        0        0     3509 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/ShoestringConfiguration.py
--rw-r--r--   0        0        0      371 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/TransactionSerializer.py
--rw-r--r--   0        0        0     3947 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/VoterConfigurator.py
--rw-r--r--   0        0        0        0 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/__init__.py
--rw-r--r--   0        0        0    15969 2023-08-01 16:59:00.626339 symbol-shoestring-0.0.5/shoestring/lang/en/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    25392 2023-08-01 16:58:59.930338 symbol-shoestring-0.0.5/shoestring/lang/en/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      438 2023-08-01 16:59:00.618339 symbol-shoestring-0.0.5/shoestring/lang/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    18950 2023-08-01 16:59:00.338339 symbol-shoestring-0.0.5/shoestring/lang/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    18737 2023-08-01 16:58:59.638338 symbol-shoestring-0.0.5/shoestring/lang/messages.pot
--rw-r--r--   0        0        0      213 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/lang/po.header.txt
--rw-r--r--   0        0        0      270 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/delayrestapi.sh
--rw-r--r--   0        0        0      565 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/mongors.sh
--rw-r--r--   0        0        0      190 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/startBroker.sh
--rw-r--r--   0        0        0      272 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/startServer.sh
--rw-r--r--   0        0        0      102 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/wait.sh
--rw-r--r--   0        0        0     2830 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/templates/docker-compose-dual.yaml
--rw-r--r--   0        0        0      629 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/templates/docker-compose-peer.yaml
--rw-r--r--   0        0        0      299 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/templates/nginx.conf.erb
--rw-r--r--   0        0        0     1004 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/Screen.py
--rw-r--r--   0        0        0     2102 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/ScreenContainer.py
--rw-r--r--   0        0        0     1781 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/ShoestringOperation.py
--rw-r--r--   0        0        0     4774 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/TabbedView.py
--rw-r--r--   0        0        0      843 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/TitleBar.py
--rw-r--r--   0        0        0     2708 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/ValidatingTextBox.py
--rw-r--r--   0        0        0        0 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/__init__.py
--rw-r--r--   0        0        0     3664 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/__main__.py
--rw-r--r--   0        0        0     1970 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/buttons.py
--rw-r--r--   0        0        0      484 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/keybindings.py
--rw-r--r--   0        0        0     1553 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/navigation.py
--rw-r--r--   0        0        0     1635 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screen_loader.py
--rw-r--r--   0        0        0        0 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/__init__.py
--rw-r--r--   0        0        0     1890 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/certificates.py
--rw-r--r--   0        0        0      652 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/end_screen.py
--rw-r--r--   0        0        0     6498 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/harvesting.py
--rw-r--r--   0        0        0     1625 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/modal.py
--rw-r--r--   0        0        0      799 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/network_type.py
--rw-r--r--   0        0        0     2981 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/node_settings.py
--rw-r--r--   0        0        0      757 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/node_type.py
--rw-r--r--   0        0        0     6789 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/obligatory.py
--rw-r--r--   0        0        0      827 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/root_check.py
--rw-r--r--   0        0        0      799 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/voting.py
--rw-r--r--   0        0        0     1835 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/welcome.py
--rw-r--r--   0        0        0     3810 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/setup_file_generator.py
--rw-r--r--   0        0        0     1744 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/shoestring_dispatcher.py
--rw-r--r--   0        0        0     1095 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/styles.py
--rw-r--r--   0        0        0    11476 2023-08-01 17:02:08.134248 symbol-shoestring-0.0.5/setup.py
--rw-r--r--   0        0        0    11035 2023-08-01 17:02:08.137078 symbol-shoestring-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     9931 2023-08-07 17:57:05.797717 symbol_shoestring-0.0.6/README.md
+-rw-r--r--   0        0        0      960 2023-08-07 18:00:55.528109 symbol_shoestring-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 17:57:05.797717 symbol_shoestring-0.0.6/shoestring/__init__.py
+-rw-r--r--   0        0        0     1937 2023-08-07 17:57:05.797717 symbol_shoestring-0.0.6/shoestring/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-07 17:57:05.797717 symbol_shoestring-0.0.6/shoestring/commands/__init__.py
+-rw-r--r--   0        0        0     1552 2023-08-07 17:57:05.797717 symbol_shoestring-0.0.6/shoestring/commands/announce_transaction.py
+-rw-r--r--   0        0        0     2475 2023-08-07 17:57:05.797717 symbol_shoestring-0.0.6/shoestring/commands/health.py
+-rw-r--r--   0        0        0     1262 2023-08-07 17:57:05.797717 symbol_shoestring-0.0.6/shoestring/commands/import_bootstrap.py
+-rw-r--r--   0        0        0     1025 2023-08-07 17:57:05.797717 symbol_shoestring-0.0.6/shoestring/commands/init.py
+-rw-r--r--   0        0        0     1692 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/commands/min_cosignatures_count.py
+-rw-r--r--   0        0        0     1733 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/commands/pemtool.py
+-rw-r--r--   0        0        0     1569 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/commands/renew_certificates.py
+-rw-r--r--   0        0        0     5270 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/commands/renew_voting_keys.py
+-rw-r--r--   0        0        0     3071 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/commands/reset_data.py
+-rw-r--r--   0        0        0     5330 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/commands/setup.py
+-rw-r--r--   0        0        0     3332 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/commands/signer.py
+-rw-r--r--   0        0        0     2246 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/commands/upgrade.py
+-rw-r--r--   0        0        0        0 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/healthagents/__init__.py
+-rw-r--r--   0        0        0      594 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/healthagents/peer_api.py
+-rw-r--r--   0        0        0     3586 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/healthagents/peer_certificate.py
+-rw-r--r--   0        0        0      644 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/healthagents/rest_api.py
+-rw-r--r--   0        0        0     2985 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/healthagents/rest_https_certificate.py
+-rw-r--r--   0        0        0     1686 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/healthagents/voting_keys.py
+-rw-r--r--   0        0        0     1573 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/healthagents/websockets.py
+-rw-r--r--   0        0        0     5055 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/CertificateFactory.py
+-rw-r--r--   0        0        0     3233 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/ConfigurationManager.py
+-rw-r--r--   0        0        0     1656 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/FileDownloader.py
+-rw-r--r--   0        0        0      360 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/FileTemplater.py
+-rw-r--r--   0        0        0     1961 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/HarvesterConfigurator.py
+-rw-r--r--   0        0        0      830 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/HeightGrouping.py
+-rw-r--r--   0        0        0     3089 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/LinkTransactionBuilder.py
+-rw-r--r--   0        0        0      655 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/MultisigAnalyzer.py
+-rw-r--r--   0        0        0     2789 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/NodeDownloader.py
+-rw-r--r--   0        0        0      578 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/NodeFeatures.py
+-rw-r--r--   0        0        0     1412 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/NodewatchClient.py
+-rw-r--r--   0        0        0     1381 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/OpensslExecutor.py
+-rw-r--r--   0        0        0     3060 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/PackageResolver.py
+-rw-r--r--   0        0        0     2139 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/PeerDownloader.py
+-rw-r--r--   0        0        0     2372 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/PemUtils.py
+-rw-r--r--   0        0        0    12793 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/Preparer.py
+-rw-r--r--   0        0        0     3509 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/ShoestringConfiguration.py
+-rw-r--r--   0        0        0      371 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/TransactionSerializer.py
+-rw-r--r--   0        0        0     3947 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/VoterConfigurator.py
+-rw-r--r--   0        0        0        0 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/internal/__init__.py
+-rw-r--r--   0        0        0    15969 2023-08-07 17:59:07.594985 symbol_shoestring-0.0.6/shoestring/lang/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    25392 2023-08-07 17:59:07.018979 symbol_shoestring-0.0.6/shoestring/lang/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      438 2023-08-07 17:59:07.598985 symbol_shoestring-0.0.6/shoestring/lang/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    18950 2023-08-07 17:59:07.326982 symbol_shoestring-0.0.6/shoestring/lang/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    18737 2023-08-07 17:59:06.662975 symbol_shoestring-0.0.6/shoestring/lang/messages.pot
+-rw-r--r--   0        0        0      213 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/lang/po.header.txt
+-rw-r--r--   0        0        0      270 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/startup/delayrestapi.sh
+-rw-r--r--   0        0        0      565 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/startup/mongors.sh
+-rw-r--r--   0        0        0      190 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/startup/startBroker.sh
+-rw-r--r--   0        0        0      272 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/startup/startServer.sh
+-rw-r--r--   0        0        0      102 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/startup/wait.sh
+-rw-r--r--   0        0        0     2830 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/templates/docker-compose-dual.yaml
+-rw-r--r--   0        0        0      629 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/templates/docker-compose-peer.yaml
+-rw-r--r--   0        0        0      299 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/templates/nginx.conf.erb
+-rw-r--r--   0        0        0     1004 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/Screen.py
+-rw-r--r--   0        0        0     2102 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/ScreenContainer.py
+-rw-r--r--   0        0        0     1781 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/ShoestringOperation.py
+-rw-r--r--   0        0        0     4774 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/TabbedView.py
+-rw-r--r--   0        0        0      843 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/TitleBar.py
+-rw-r--r--   0        0        0     2708 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/ValidatingTextBox.py
+-rw-r--r--   0        0        0        0 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/__init__.py
+-rw-r--r--   0        0        0     3664 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/__main__.py
+-rw-r--r--   0        0        0     1970 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/buttons.py
+-rw-r--r--   0        0        0      484 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/keybindings.py
+-rw-r--r--   0        0        0     1553 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/navigation.py
+-rw-r--r--   0        0        0     1635 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screen_loader.py
+-rw-r--r--   0        0        0        0 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/__init__.py
+-rw-r--r--   0        0        0     1890 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/certificates.py
+-rw-r--r--   0        0        0      652 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/end_screen.py
+-rw-r--r--   0        0        0     6498 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/harvesting.py
+-rw-r--r--   0        0        0     1625 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/modal.py
+-rw-r--r--   0        0        0      799 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/network_type.py
+-rw-r--r--   0        0        0     2981 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/node_settings.py
+-rw-r--r--   0        0        0      757 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/node_type.py
+-rw-r--r--   0        0        0     6789 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/obligatory.py
+-rw-r--r--   0        0        0      827 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/root_check.py
+-rw-r--r--   0        0        0      799 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/voting.py
+-rw-r--r--   0        0        0     1835 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/screens/welcome.py
+-rw-r--r--   0        0        0     3810 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/setup_file_generator.py
+-rw-r--r--   0        0        0     1744 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/shoestring_dispatcher.py
+-rw-r--r--   0        0        0     1095 2023-08-07 17:57:05.801717 symbol_shoestring-0.0.6/shoestring/wizard/styles.py
+-rw-r--r--   0        0        0    11098 1970-01-01 00:00:00.000000 symbol_shoestring-0.0.6/PKG-INFO
```

### Comparing `symbol-shoestring-0.0.5/README.md` & `symbol_shoestring-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/__main__.py` & `symbol_shoestring-0.0.6/shoestring/__main__.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/announce_transaction.py` & `symbol_shoestring-0.0.6/shoestring/commands/announce_transaction.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/health.py` & `symbol_shoestring-0.0.6/shoestring/commands/health.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/import_bootstrap.py` & `symbol_shoestring-0.0.6/shoestring/commands/import_bootstrap.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/init.py` & `symbol_shoestring-0.0.6/shoestring/commands/init.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/min_cosignatures_count.py` & `symbol_shoestring-0.0.6/shoestring/commands/min_cosignatures_count.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/pemtool.py` & `symbol_shoestring-0.0.6/shoestring/commands/pemtool.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/renew_certificates.py` & `symbol_shoestring-0.0.6/shoestring/commands/renew_certificates.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/renew_voting_keys.py` & `symbol_shoestring-0.0.6/shoestring/commands/renew_voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/reset_data.py` & `symbol_shoestring-0.0.6/shoestring/commands/reset_data.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/setup.py` & `symbol_shoestring-0.0.6/shoestring/commands/setup.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/signer.py` & `symbol_shoestring-0.0.6/shoestring/commands/signer.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/commands/upgrade.py` & `symbol_shoestring-0.0.6/shoestring/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/healthagents/peer_api.py` & `symbol_shoestring-0.0.6/shoestring/healthagents/peer_api.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/healthagents/peer_certificate.py` & `symbol_shoestring-0.0.6/shoestring/healthagents/peer_certificate.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/healthagents/rest_api.py` & `symbol_shoestring-0.0.6/shoestring/healthagents/rest_api.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/healthagents/rest_https_certificate.py` & `symbol_shoestring-0.0.6/shoestring/healthagents/rest_https_certificate.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/healthagents/voting_keys.py` & `symbol_shoestring-0.0.6/shoestring/healthagents/voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/healthagents/websockets.py` & `symbol_shoestring-0.0.6/shoestring/healthagents/websockets.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/CertificateFactory.py` & `symbol_shoestring-0.0.6/shoestring/internal/CertificateFactory.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/ConfigurationManager.py` & `symbol_shoestring-0.0.6/shoestring/internal/ConfigurationManager.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/FileDownloader.py` & `symbol_shoestring-0.0.6/shoestring/internal/FileDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/HarvesterConfigurator.py` & `symbol_shoestring-0.0.6/shoestring/internal/HarvesterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/HeightGrouping.py` & `symbol_shoestring-0.0.6/shoestring/internal/HeightGrouping.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/LinkTransactionBuilder.py` & `symbol_shoestring-0.0.6/shoestring/internal/LinkTransactionBuilder.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/MultisigAnalyzer.py` & `symbol_shoestring-0.0.6/shoestring/internal/MultisigAnalyzer.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/NodeDownloader.py` & `symbol_shoestring-0.0.6/shoestring/internal/NodeDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/NodeFeatures.py` & `symbol_shoestring-0.0.6/shoestring/internal/NodeFeatures.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/NodewatchClient.py` & `symbol_shoestring-0.0.6/shoestring/internal/NodewatchClient.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/OpensslExecutor.py` & `symbol_shoestring-0.0.6/shoestring/internal/OpensslExecutor.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/PackageResolver.py` & `symbol_shoestring-0.0.6/shoestring/internal/PackageResolver.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/PeerDownloader.py` & `symbol_shoestring-0.0.6/shoestring/internal/PeerDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/PemUtils.py` & `symbol_shoestring-0.0.6/shoestring/internal/PemUtils.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/Preparer.py` & `symbol_shoestring-0.0.6/shoestring/internal/Preparer.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/ShoestringConfiguration.py` & `symbol_shoestring-0.0.6/shoestring/internal/ShoestringConfiguration.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/internal/VoterConfigurator.py` & `symbol_shoestring-0.0.6/shoestring/internal/VoterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/lang/en/LC_MESSAGES/messages.mo` & `symbol_shoestring-0.0.6/shoestring/lang/en/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-08-01 16:59+0000\n"
+"POT-Creation-Date: 2023-08-07 17:59+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `symbol-shoestring-0.0.5/shoestring/lang/en/LC_MESSAGES/messages.po` & `symbol_shoestring-0.0.6/shoestring/lang/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/lang/ja/LC_MESSAGES/messages.po` & `symbol_shoestring-0.0.6/shoestring/lang/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/lang/messages.pot` & `symbol_shoestring-0.0.6/shoestring/lang/messages.pot`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/startup/mongors.sh` & `symbol_shoestring-0.0.6/shoestring/startup/mongors.sh`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/templates/docker-compose-dual.yaml` & `symbol_shoestring-0.0.6/shoestring/templates/docker-compose-dual.yaml`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/templates/docker-compose-peer.yaml` & `symbol_shoestring-0.0.6/shoestring/templates/docker-compose-peer.yaml`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/Screen.py` & `symbol_shoestring-0.0.6/shoestring/wizard/Screen.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/ScreenContainer.py` & `symbol_shoestring-0.0.6/shoestring/wizard/ScreenContainer.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/ShoestringOperation.py` & `symbol_shoestring-0.0.6/shoestring/wizard/ShoestringOperation.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/TabbedView.py` & `symbol_shoestring-0.0.6/shoestring/wizard/TabbedView.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/TitleBar.py` & `symbol_shoestring-0.0.6/shoestring/wizard/TitleBar.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/ValidatingTextBox.py` & `symbol_shoestring-0.0.6/shoestring/wizard/ValidatingTextBox.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/__main__.py` & `symbol_shoestring-0.0.6/shoestring/wizard/__main__.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/buttons.py` & `symbol_shoestring-0.0.6/shoestring/wizard/buttons.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/navigation.py` & `symbol_shoestring-0.0.6/shoestring/wizard/navigation.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screen_loader.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screen_loader.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/certificates.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/certificates.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/end_screen.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/end_screen.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/harvesting.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/harvesting.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/modal.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/modal.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/network_type.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/network_type.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/node_settings.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/node_settings.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/node_type.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/node_type.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/obligatory.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/obligatory.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/root_check.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/root_check.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/voting.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/voting.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/screens/welcome.py` & `symbol_shoestring-0.0.6/shoestring/wizard/screens/welcome.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/setup_file_generator.py` & `symbol_shoestring-0.0.6/shoestring/wizard/setup_file_generator.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/shoestring_dispatcher.py` & `symbol_shoestring-0.0.6/shoestring/wizard/shoestring_dispatcher.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/shoestring/wizard/styles.py` & `symbol_shoestring-0.0.6/shoestring/wizard/styles.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.5/setup.py` & `symbol_shoestring-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,354 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: symbol-shoestring
+Version: 0.0.6
+Summary: Symbol Shoestring Deployment Tool
+Home-page: https://github.com/symbol/product/tree/main/tools/shoestring
+License: MIT
+Keywords: symbol,shoestring,deployment,node
+Author: Symbol Contributors
+Author-email: contributors@symbol.dev
+Maintainer: Symbol Contributors
+Maintainer-email: contributors@symbol.dev
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.5,<3.9.0)
+Requires-Dist: jinja2 (>=3.1.2,<3.2.0)
+Requires-Dist: prompt-toolkit (>=3.0.39,<3.1.0)
+Requires-Dist: pyyaml (>=6.0.1,<6.1.0)
+Requires-Dist: requests (>=2.31.0,<2.32.0)
+Requires-Dist: symbol-lightapi (>=0.0.5,<0.1.0)
+Requires-Dist: symbol-sdk-python (>=3.1.0,<3.2.0)
+Requires-Dist: websockets (>=11.0.3,<11.1.0)
+Requires-Dist: zenlog (>=1.1,<2.0)
+Project-URL: Repository, https://github.com/symbol/product/tree/main/tools/shoestring
+Description-Content-Type: text/markdown
 
-packages = \
-['shoestring',
- 'shoestring.commands',
- 'shoestring.healthagents',
- 'shoestring.internal',
- 'shoestring.wizard',
- 'shoestring.wizard.screens']
-
-package_data = \
-{'': ['*'],
- 'shoestring': ['lang/*',
-                'lang/en/LC_MESSAGES/*',
-                'lang/ja/LC_MESSAGES/*',
-                'startup/*',
-                'templates/*']}
-
-install_requires = \
-['Jinja2==3.1.2',
- 'PyYAML==6.0.1',
- 'aiohttp==3.8.5',
- 'prompt-toolkit==3.0.39',
- 'requests==2.31.0',
- 'symbol-lightapi==0.0.4',
- 'symbol-sdk-python==3.0.11',
- 'websockets==11.0.3',
- 'zenlog==1.1']
-
-setup_kwargs = {
-    'name': 'symbol-shoestring',
-    'version': '0.0.5',
-    'description': 'Symbol Shoestring Deployment Tool',
-    'long_description': '# shoestring\n\n# CLI Commands\n\n## Setup Commands\n\n### init\n\nExtracts a template shoestring configuration file from a package that the user can then customize.\n\n```\ninit [--package PACKAGE] config\n\n  config             path to shoestring configuration file\n  --package PACKAGE  Network configuration package. Possible values: (name | file:///filename | http(s)://uri) (default: mainnet)\n```\n\n### min-cosignatures-count\n\nAutomatically detects the minimum cosignatures required for an account and optionally updates the shoestring configuration file.\n\n```\nmin-cosignatures-count --config CONFIG --ca-key-path CA_KEY_PATH [--update]\n\n  --config CONFIG           path to shoestring configuration file\n  --ca-key-path CA_KEY_PATH path to main private key PEM file\n  --update                  update the shoestring configuration file\n```\n\n### import-bootstrap\n\nImports settings from a symbol-bootstap installation.\n\n\n```\nimport-bootstrap --config CONFIG --bootstrap BOOTSTRAP\n\n  --config CONFIG       path to shoestring configuration file\n  --bootstrap BOOTSTRAP path to bootstrap target directory\n```\n\n### pemtool\n\nGenerates a main private key PEM file that can be used by shoestring.\n\n```\npemtool --output OUTPUT [--input INPUT] [--ask-pass] [--force]\n\n  --output OUTPUT  output PEM key file\n  --input INPUT    input private key file (optional)\n  --ask-pass       encrypt PEM with a password (password prompt will be shown)\n  --force          overwrite output file if it already exists\n```\n\n### setup\n\nSets up a Symbol node from scratch\n\n```\nsetup \\\n    --config CONFIG \\\n    [--package PACKAGE] \\\n    [--directory DIRECTORY] \\\n    [--overrides OVERRIDES] \\\n    [--metadata METADATA] \\\n    [--security {default,paranoid,insecure}] \\\n    --ca-key-path CA_KEY_PATH\n\n  --config CONFIG           path to shoestring configuration file\n  --package PACKAGE         Network configuration package. Possible values: (name | file:///filename | http(s)://uri) (default: mainnet)\n  --directory DIRECTORY     installation directory (default: $HOME)\n  --overrides OVERRIDES     path to custom user settings\n  --metadata METADATA       custom node metadata (this is only valid for API roles)\n  --security                security mode (default: default)\n  --ca-key-path CA_KEY_PATH path to main private key PEM file\n```\n\nPlease note that only security mode "default" is supported at this time.\n\nThis command will generate a transaction that will need to be sent to the network using `announce-transaction` to update the network state.\n\n## Operational Commands\n\n### signer\n\nSigns a transaction that can then be announced to the network\n\n```\nsigner --config CONFIG --ca-key-path CA_KEY_PATH [--save] filename\n\n  filename                  transaction binary payload\n  --config CONFIG           path to shoestring configuration file\n  --ca-key-path CA_KEY_PATH path to main private key PEM file\n  --save                    save signed payload into same file as input\n```\n\n### announce-transaction\n\nAnnounces a transaction to the network.\n\n```\nannounce-transaction --config CONFIG --transaction TRANSACTION\n\n  --config CONFIG           path to shoestring configuration file\n  --transaction TRANSACTION file containing serialized transaction to send\n```\n\n### health\n\nChecks the health of the local Symbol node.\n\n\n```\nhealth [-h] --config CONFIG [--directory DIRECTORY]\n\n  --config CONFIG       path to shoestring configuration file\n  --directory DIRECTORY installation directory (default: $HOME)\n```\n\n## Upgrade Commands\n\n### upgrade\n\nUpgrades a node to the latest client version.\n\n```\nupgrade \\\n    --config CONFIG \\\n    [--package PACKAGE] \\\n    [--directory DIRECTORY] \\\n    [--overrides OVERRIDES] \\\n    [--metadata METADATA]\n\n  --config CONFIG           path to shoestring configuration file\n  --package PACKAGE         Network configuration package. Possible values: (name | file:///filename | http(s)://uri) (default: mainnet)\n  --directory DIRECTORY     installation directory (default: $HOME)\n  --overrides OVERRIDES     path to custom user settings\n  --metadata METADATA       custom node metadata (this is only valid for API roles)\n```\n\n### renew-certificates\n\nRenews peer certificates.\n\n```\nrenew-certificates --config CONFIG [--directory DIRECTORY] --ca-key-path CA_KEY_PATH [--renew-ca]\n\n  --config CONFIG           path to shoestring configuration file\n  --directory DIRECTORY     installation directory (default: $HOME)\n  --ca-key-path CA_KEY_PATH path to main private key PEM file\n  --renew-ca                renews CA certificate too\n```\n\nWhen `--renew-ca` is set, both CA and node certificates will be regenerated. Otherwise, only node certificate will be.\n\n### renew-voting-keys\n\nRenews voting keys.\n\n```\nrenew-voting-keys --config CONFIG [--directory DIRECTORY]\n\n  --config CONFIG           path to shoestring configuration file\n  --directory DIRECTORY     installation directory (default: $HOME)\n```\n\nThis command will generate a transaction that will need to be sent to the network using `announce-transaction` to update the network state.\n\n### reset-data\n\nResets blockchain state to allow a resync from scratch.\n\n```\nreset-data --config CONFIG [--directory DIRECTORY] [--purge-harvesters]\n\n  --config CONFIG           path to shoestring configuration file\n  --directory DIRECTORY     installation directory (default: $HOME)\n  --purge-harvesters        purge harvesters.dat file\n```\n\nWhen `--purge-harvesters` is set, delegates discovered using old keys will be discarded.\n\n\n## Files\n\n### Shoestring Configuration INI\n\nINI file used by shoestring to customize a Symbol node deployment.\nIt is composed of five sections: `network`, `images`, `services`, `transaction`, `imports`, `node`.\n\n#### network\n\nDescribes properties of network that deployed node should connect with.\nThese should match values in `config-network.properties` Symbol configuration file.\nIf `init` command is used, these values shouldn\'t be modified\n\n```\nname                  Network name\nidentifier            Network numeric identifier\nepochAdjustment       Network epoch adjustment\ngenerationHashSeed    Network generation hash seed\n```\n\n#### images\n\nDescribes Symbol docker images to use.\nIf `init` command is used, these values shouldn\'t be modified\n```\nclient  Catapult client docker image\nrest    REST docker image\n```\n\n#### services\n\nDescribes network services to use during deployment.\nIf `init` command is used, these values shouldn\'t be modified\n\n```\nnodewatch  URL to nodewatch service.\n```\n\n#### transactions\n\nDescribes properties of generated transactions.\nIf `init` command is used, most of these values _generally_ shouldn\'t be modified.\n`min-cosignatures-count` command can be used to automatically update `minCosignaturesCount` setting.\n\nGeneral properties:\n```\nfeeMultiplier             Min fee multiplier of generated transactions\ntimeoutHours              Timeout of generated transactions (in hours)\nminCosignaturesCount      Minimum number of cosignatures generated transactions will require\n```\n\nWhen `signer` command is signing an aggregate bonded transaction, it will additionally generate a hash lock transaction\nusing the following properties:\n```\nhashLockDuration          Hash lock duration in blocks\ncurrencyMosaicId          Network currency mosaid id\nlockedFundsPerAggregate   Locked funds per aggregate\n```\n\n#### imports\n\nDescribes keys to import.\nThese need to be manually set if there are harvesting and/or voting keys that need to be imported.\n\n```\nharvester Path to a config-harvesting.properties Symbol configuration file containing harvesting keys to import\nvoter     Path to a directory containing private_key_tree*.day files to import\n```\n\n#### node\n\nDescribes settings to customize a node.\n\n`features` supports the following:\n* `PEER` - Peer support\n* `API` - REST support\n* `HARVESTER` - Node will be configured to harvest and accept delegated harvesters\n* `VOTER` - Node will be configured to vote\n\n`caPassword` supports all available openssl passphrase options: https://www.openssl.org/docs/man3.0/man1/openssl-passphrase-options.html.\n\n```\nfeatures       One or more node features to deploy (| delimited)\nuserId         User id of node used to set process and file permissons\ngroupId        Group id of node used to set process and file permissons\ncaPassword     Password of CA (main) PEM private key file (if applicable)\napiHttps       Set to enable HTTPS REST (only applicable when features include API)\n\ncaCommonName   Common name of generated CA certificates\nnodeCommonName Common name of generated Node certificates\n```\n\n### Overrides\n\nINI file that is used to customize advanced Symbol settings.\n\nSections should have the format `[<config-short-name>.<config-section>]`.\nSection contents will then be applied to the appropriate Symbol configuration file.\n\nFor example, in order to set two custom settings:\n1. `connectTimeout` - located in the `config-node.properties` file in section `node`\n1. `maxUnlockedAccounts` - located in the `config-harvesting.properties` file in section `harvesting`\n\nThe following snippet will suffice:\n\n```ini\n[node.node]\n\nconnectTimeout = 5s\n\n[harvesting.harvesting]\n\nmaxUnlockedAccounts = 2\n```\n\nNotice that these custom settings are applied *BEFORE* shoestring updates the Symbol configuration files.\nIn cases of conflicts, the shoestring changes will take precedence.\n\n### Node Metadata\n\nJSON file that is ingested and used to replace the contents of `nodeMetadata` in rest.json.\nThis data is then accessible via the `node/metadata` REST endpoint.\nThis file is optional and only used for deployments including API role.\n\n## Prerequisites:\n\n    apt-get install python3 python3-pip openssl\n    python3 -m pip install -r requirements.txt\n\n## Temporarily (until lightapi package fix):\n\n```\ncd product/lightapi/python\n./scripts/ci/setup_lint.sh\n./scripts/ci/lint.sh\n./scripts/ci/test.sh\n\n# to run shoestring\n\nPYTHONPATH=}full path here{/product/lightapi/python python3 -m shoestring\n```\n',
-    'author': 'Symbol Contributors',
-    'author_email': 'contributors@symbol.dev',
-    'maintainer': 'Symbol Contributors',
-    'maintainer_email': 'contributors@symbol.dev',
-    'url': 'https://github.com/symbol/product/tree/main/tools/shoestring',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+# shoestring
 
+# CLI Commands
+
+## Setup Commands
+
+### init
+
+Extracts a template shoestring configuration file from a package that the user can then customize.
+
+```
+init [--package PACKAGE] config
+
+  config             path to shoestring configuration file
+  --package PACKAGE  Network configuration package. Possible values: (name | file:///filename | http(s)://uri) (default: mainnet)
+```
+
+### min-cosignatures-count
+
+Automatically detects the minimum cosignatures required for an account and optionally updates the shoestring configuration file.
+
+```
+min-cosignatures-count --config CONFIG --ca-key-path CA_KEY_PATH [--update]
+
+  --config CONFIG           path to shoestring configuration file
+  --ca-key-path CA_KEY_PATH path to main private key PEM file
+  --update                  update the shoestring configuration file
+```
+
+### import-bootstrap
+
+Imports settings from a symbol-bootstap installation.
+
+
+```
+import-bootstrap --config CONFIG --bootstrap BOOTSTRAP
+
+  --config CONFIG       path to shoestring configuration file
+  --bootstrap BOOTSTRAP path to bootstrap target directory
+```
+
+### pemtool
+
+Generates a main private key PEM file that can be used by shoestring.
+
+```
+pemtool --output OUTPUT [--input INPUT] [--ask-pass] [--force]
+
+  --output OUTPUT  output PEM key file
+  --input INPUT    input private key file (optional)
+  --ask-pass       encrypt PEM with a password (password prompt will be shown)
+  --force          overwrite output file if it already exists
+```
+
+### setup
+
+Sets up a Symbol node from scratch
+
+```
+setup \
+    --config CONFIG \
+    [--package PACKAGE] \
+    [--directory DIRECTORY] \
+    [--overrides OVERRIDES] \
+    [--metadata METADATA] \
+    [--security {default,paranoid,insecure}] \
+    --ca-key-path CA_KEY_PATH
+
+  --config CONFIG           path to shoestring configuration file
+  --package PACKAGE         Network configuration package. Possible values: (name | file:///filename | http(s)://uri) (default: mainnet)
+  --directory DIRECTORY     installation directory (default: $HOME)
+  --overrides OVERRIDES     path to custom user settings
+  --metadata METADATA       custom node metadata (this is only valid for API roles)
+  --security                security mode (default: default)
+  --ca-key-path CA_KEY_PATH path to main private key PEM file
+```
+
+Please note that only security mode "default" is supported at this time.
+
+This command will generate a transaction that will need to be sent to the network using `announce-transaction` to update the network state.
+
+## Operational Commands
+
+### signer
+
+Signs a transaction that can then be announced to the network
+
+```
+signer --config CONFIG --ca-key-path CA_KEY_PATH [--save] filename
+
+  filename                  transaction binary payload
+  --config CONFIG           path to shoestring configuration file
+  --ca-key-path CA_KEY_PATH path to main private key PEM file
+  --save                    save signed payload into same file as input
+```
+
+### announce-transaction
+
+Announces a transaction to the network.
+
+```
+announce-transaction --config CONFIG --transaction TRANSACTION
+
+  --config CONFIG           path to shoestring configuration file
+  --transaction TRANSACTION file containing serialized transaction to send
+```
+
+### health
+
+Checks the health of the local Symbol node.
+
+
+```
+health [-h] --config CONFIG [--directory DIRECTORY]
+
+  --config CONFIG       path to shoestring configuration file
+  --directory DIRECTORY installation directory (default: $HOME)
+```
+
+## Upgrade Commands
+
+### upgrade
+
+Upgrades a node to the latest client version.
+
+```
+upgrade \
+    --config CONFIG \
+    [--package PACKAGE] \
+    [--directory DIRECTORY] \
+    [--overrides OVERRIDES] \
+    [--metadata METADATA]
+
+  --config CONFIG           path to shoestring configuration file
+  --package PACKAGE         Network configuration package. Possible values: (name | file:///filename | http(s)://uri) (default: mainnet)
+  --directory DIRECTORY     installation directory (default: $HOME)
+  --overrides OVERRIDES     path to custom user settings
+  --metadata METADATA       custom node metadata (this is only valid for API roles)
+```
+
+### renew-certificates
+
+Renews peer certificates.
+
+```
+renew-certificates --config CONFIG [--directory DIRECTORY] --ca-key-path CA_KEY_PATH [--renew-ca]
+
+  --config CONFIG           path to shoestring configuration file
+  --directory DIRECTORY     installation directory (default: $HOME)
+  --ca-key-path CA_KEY_PATH path to main private key PEM file
+  --renew-ca                renews CA certificate too
+```
+
+When `--renew-ca` is set, both CA and node certificates will be regenerated. Otherwise, only node certificate will be.
+
+### renew-voting-keys
+
+Renews voting keys.
+
+```
+renew-voting-keys --config CONFIG [--directory DIRECTORY]
+
+  --config CONFIG           path to shoestring configuration file
+  --directory DIRECTORY     installation directory (default: $HOME)
+```
+
+This command will generate a transaction that will need to be sent to the network using `announce-transaction` to update the network state.
+
+### reset-data
+
+Resets blockchain state to allow a resync from scratch.
+
+```
+reset-data --config CONFIG [--directory DIRECTORY] [--purge-harvesters]
+
+  --config CONFIG           path to shoestring configuration file
+  --directory DIRECTORY     installation directory (default: $HOME)
+  --purge-harvesters        purge harvesters.dat file
+```
+
+When `--purge-harvesters` is set, delegates discovered using old keys will be discarded.
+
+
+## Files
+
+### Shoestring Configuration INI
+
+INI file used by shoestring to customize a Symbol node deployment.
+It is composed of five sections: `network`, `images`, `services`, `transaction`, `imports`, `node`.
+
+#### network
+
+Describes properties of network that deployed node should connect with.
+These should match values in `config-network.properties` Symbol configuration file.
+If `init` command is used, these values shouldn't be modified
+
+```
+name                  Network name
+identifier            Network numeric identifier
+epochAdjustment       Network epoch adjustment
+generationHashSeed    Network generation hash seed
+```
+
+#### images
+
+Describes Symbol docker images to use.
+If `init` command is used, these values shouldn't be modified
+```
+client  Catapult client docker image
+rest    REST docker image
+```
+
+#### services
+
+Describes network services to use during deployment.
+If `init` command is used, these values shouldn't be modified
+
+```
+nodewatch  URL to nodewatch service.
+```
+
+#### transactions
+
+Describes properties of generated transactions.
+If `init` command is used, most of these values _generally_ shouldn't be modified.
+`min-cosignatures-count` command can be used to automatically update `minCosignaturesCount` setting.
+
+General properties:
+```
+feeMultiplier             Min fee multiplier of generated transactions
+timeoutHours              Timeout of generated transactions (in hours)
+minCosignaturesCount      Minimum number of cosignatures generated transactions will require
+```
+
+When `signer` command is signing an aggregate bonded transaction, it will additionally generate a hash lock transaction
+using the following properties:
+```
+hashLockDuration          Hash lock duration in blocks
+currencyMosaicId          Network currency mosaid id
+lockedFundsPerAggregate   Locked funds per aggregate
+```
+
+#### imports
+
+Describes keys to import.
+These need to be manually set if there are harvesting and/or voting keys that need to be imported.
+
+```
+harvester Path to a config-harvesting.properties Symbol configuration file containing harvesting keys to import
+voter     Path to a directory containing private_key_tree*.day files to import
+```
+
+#### node
+
+Describes settings to customize a node.
+
+`features` supports the following:
+* `PEER` - Peer support
+* `API` - REST support
+* `HARVESTER` - Node will be configured to harvest and accept delegated harvesters
+* `VOTER` - Node will be configured to vote
+
+`caPassword` supports all available openssl passphrase options: https://www.openssl.org/docs/man3.0/man1/openssl-passphrase-options.html.
+
+```
+features       One or more node features to deploy (| delimited)
+userId         User id of node used to set process and file permissons
+groupId        Group id of node used to set process and file permissons
+caPassword     Password of CA (main) PEM private key file (if applicable)
+apiHttps       Set to enable HTTPS REST (only applicable when features include API)
+
+caCommonName   Common name of generated CA certificates
+nodeCommonName Common name of generated Node certificates
+```
+
+### Overrides
+
+INI file that is used to customize advanced Symbol settings.
+
+Sections should have the format `[<config-short-name>.<config-section>]`.
+Section contents will then be applied to the appropriate Symbol configuration file.
+
+For example, in order to set two custom settings:
+1. `connectTimeout` - located in the `config-node.properties` file in section `node`
+1. `maxUnlockedAccounts` - located in the `config-harvesting.properties` file in section `harvesting`
+
+The following snippet will suffice:
+
+```ini
+[node.node]
+
+connectTimeout = 5s
+
+[harvesting.harvesting]
+
+maxUnlockedAccounts = 2
+```
+
+Notice that these custom settings are applied *BEFORE* shoestring updates the Symbol configuration files.
+In cases of conflicts, the shoestring changes will take precedence.
+
+### Node Metadata
+
+JSON file that is ingested and used to replace the contents of `nodeMetadata` in rest.json.
+This data is then accessible via the `node/metadata` REST endpoint.
+This file is optional and only used for deployments including API role.
+
+## Prerequisites:
+
+    apt-get install python3 python3-pip openssl
+    python3 -m pip install -r requirements.txt
+
+## Temporarily (until lightapi package fix):
+
+```
+cd product/lightapi/python
+./scripts/ci/setup_lint.sh
+./scripts/ci/lint.sh
+./scripts/ci/test.sh
+
+# to run shoestring
+
+PYTHONPATH=}full path here{/product/lightapi/python python3 -m shoestring
+```
 
-setup(**setup_kwargs)
```

