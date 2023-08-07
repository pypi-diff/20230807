# Comparing `tmp/dns-lexicon-3.9.4.tar.gz` & `tmp/dns-lexicon-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dns-lexicon-3.9.4.tar", max compression
+gzip compressed data, was "dns-lexicon-3.9.5.tar", max compression
```

## Comparing `dns-lexicon-3.9.4.tar` & `dns-lexicon-3.9.5.tar`

### file list

```diff
@@ -1,96 +1,97 @@
--rw-r--r--   0        0        0     1082 2022-02-14 23:27:53.822654 dns-lexicon-3.9.4/LICENSE
--rw-r--r--   0        0        0     7576 2022-02-14 23:27:53.822654 dns-lexicon-3.9.4/README.rst
--rw-r--r--   0        0        0      100 2022-02-14 23:27:53.822654 dns-lexicon-3.9.4/lexicon/__init__.py
--rw-r--r--   0        0        0     4302 2022-02-14 23:27:53.822654 dns-lexicon-3.9.4/lexicon/cli.py
--rw-r--r--   0        0        0     5545 2022-02-14 23:27:53.822654 dns-lexicon-3.9.4/lexicon/client.py
--rw-r--r--   0        0        0    15590 2022-02-14 23:27:53.822654 dns-lexicon-3.9.4/lexicon/config.py
--rw-r--r--   0        0        0     1173 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/conftest.py
--rw-r--r--   0        0        0     1973 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/discovery.py
--rw-r--r--   0        0        0      469 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/exceptions.py
--rw-r--r--   0        0        0     3405 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/parser.py
--rw-r--r--   0        0        0       88 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/__init__.py
--rw-r--r--   0        0        0     8095 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/aliyun.py
--rw-r--r--   0        0        0     6602 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/aurora.py
--rw-r--r--   0        0        0     9562 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/auto.py
--rw-r--r--   0        0        0    13916 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/azure.py
--rw-r--r--   0        0        0     8018 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/base.py
--rw-r--r--   0        0        0     8160 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/cloudflare.py
--rw-r--r--   0        0        0     8480 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/cloudns.py
--rw-r--r--   0        0        0     6636 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/cloudxns.py
--rw-r--r--   0        0        0     8059 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/conoha.py
--rw-r--r--   0        0        0    10184 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/constellix.py
--rw-r--r--   0        0        0     6411 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/ddns.py
--rw-r--r--   0        0        0     5269 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/digitalocean.py
--rw-r--r--   0        0        0     9612 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/dinahosting.py
--rw-r--r--   0        0        0     8488 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/directadmin.py
--rw-r--r--   0        0        0     7917 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/dnsimple.py
--rw-r--r--   0        0        0     7967 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/dnsmadeeasy.py
--rw-r--r--   0        0        0     4726 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/dnspark.py
--rw-r--r--   0        0        0     5607 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/dnspod.py
--rw-r--r--   0        0        0     8038 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/dreamhost.py
--rw-r--r--   0        0        0    10276 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/dynu.py
--rw-r--r--   0        0        0     5400 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/easydns.py
--rw-r--r--   0        0        0    18721 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/easyname.py
--rw-r--r--   0        0        0     9029 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/euserv.py
--rw-r--r--   0        0        0     5829 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/exoscale.py
--rw-r--r--   0        0        0    20642 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/gandi.py
--rw-r--r--   0        0        0    11044 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/gehirn.py
--rw-r--r--   0        0        0     5566 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/glesys.py
--rw-r--r--   0        0        0    13763 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/godaddy.py
--rw-r--r--   0        0        0    21795 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/googleclouddns.py
--rw-r--r--   0        0        0    13059 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/gransy.py
--rw-r--r--   0        0        0    10782 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/gratisdns.py
--rw-r--r--   0        0        0     9057 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/henet.py
--rw-r--r--   0        0        0     7560 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/hetzner.py
--rw-r--r--   0        0        0     9267 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/hostingde.py
--rw-r--r--   0        0        0     6782 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/hover.py
--rw-r--r--   0        0        0    13978 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/infoblox.py
--rw-r--r--   0        0        0     6243 2022-02-14 23:27:53.826654 dns-lexicon-3.9.4/lexicon/providers/infomaniak.py
--rw-r--r--   0        0        0     7679 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/internetbs.py
--rw-r--r--   0        0        0     7405 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/inwx.py
--rw-r--r--   0        0        0    12740 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/joker.py
--rw-r--r--   0        0        0     5439 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/linode.py
--rw-r--r--   0        0        0     5660 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/linode4.py
--rw-r--r--   0        0        0     5583 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/localzone.py
--rw-r--r--   0        0        0     4850 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/luadns.py
--rw-r--r--   0        0        0     5628 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/memset.py
--rw-r--r--   0        0        0    10918 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/mythicbeasts.py
--rw-r--r--   0        0        0    17678 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/namecheap.py
--rw-r--r--   0        0        0     5524 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/namesilo.py
--rw-r--r--   0        0        0     7063 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/netcup.py
--rw-r--r--   0        0        0     6218 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/nfsn.py
--rw-r--r--   0        0        0     5139 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/njalla.py
--rw-r--r--   0        0        0     9181 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/nsone.py
--rw-r--r--   0        0        0    12267 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/oci.py
--rw-r--r--   0        0        0     7161 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/onapp.py
--rw-r--r--   0        0        0     8515 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/online.py
--rw-r--r--   0        0        0     8357 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/ovh.py
--rw-r--r--   0        0        0    10087 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/plesk.py
--rw-r--r--   0        0        0     4896 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/pointhq.py
--rw-r--r--   0        0        0     9890 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/powerdns.py
--rw-r--r--   0        0        0     9893 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/rackspace.py
--rw-r--r--   0        0        0     5281 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/rage4.py
--rw-r--r--   0        0        0     8325 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/rcodezero.py
--rw-r--r--   0        0        0    13549 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/route53.py
--rw-r--r--   0        0        0     7744 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/safedns.py
--rw-r--r--   0        0        0     8087 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/sakuracloud.py
--rw-r--r--   0        0        0     5085 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/softlayer.py
--rw-r--r--   0        0        0     9287 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/transip.py
--rw-r--r--   0        0        0    10016 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/ultradns.py
--rw-r--r--   0        0        0    25184 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/valuedomain.py
--rw-r--r--   0        0        0     6402 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/vercel.py
--rw-r--r--   0        0        0     6872 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/vultr.py
--rw-r--r--   0        0        0    12408 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/webgo.py
--rw-r--r--   0        0        0     6007 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/yandex.py
--rw-r--r--   0        0        0      626 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/zeit.py
--rw-r--r--   0        0        0     6493 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/zilore.py
--rw-r--r--   0        0        0     6937 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/providers/zonomi.py
--rw-r--r--   0        0        0        0 2022-02-14 23:27:53.830654 dns-lexicon-3.9.4/lexicon/tests/__init__.py
--rw-r--r--   0        0        0     6582 2022-02-14 23:27:53.834654 dns-lexicon-3.9.4/lexicon/tests/test_client.py
--rw-r--r--   0        0        0     4494 2022-02-14 23:27:53.834654 dns-lexicon-3.9.4/lexicon/tests/test_config.py
--rw-r--r--   0        0        0     9449 2022-02-14 23:27:53.834654 dns-lexicon-3.9.4/lexicon/tests/test_library.py
--rw-r--r--   0        0        0     2148 2022-02-14 23:27:53.834654 dns-lexicon-3.9.4/lexicon/tests/test_output.py
--rw-r--r--   0        0        0     1305 2022-02-14 23:27:53.834654 dns-lexicon-3.9.4/lexicon/tests/test_parser.py
--rw-r--r--   0        0        0     2365 2022-02-14 23:27:53.834654 dns-lexicon-3.9.4/pyproject.toml
--rw-r--r--   0        0        0     8943 2022-02-14 23:28:02.474014 dns-lexicon-3.9.4/setup.py
--rw-r--r--   0        0        0     9358 2022-02-14 23:28:02.474745 dns-lexicon-3.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/LICENSE
+-rw-r--r--   0        0        0     7616 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/README.rst
+-rw-r--r--   0        0        0      100 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/__init__.py
+-rw-r--r--   0        0        0     4302 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/cli.py
+-rw-r--r--   0        0        0     5584 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/client.py
+-rw-r--r--   0        0        0    15590 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/config.py
+-rw-r--r--   0        0        0     1173 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/conftest.py
+-rw-r--r--   0        0        0     1973 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/discovery.py
+-rw-r--r--   0        0        0      469 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/exceptions.py
+-rw-r--r--   0        0        0     3405 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/parser.py
+-rw-r--r--   0        0        0       88 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/providers/__init__.py
+-rw-r--r--   0        0        0     8095 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/providers/aliyun.py
+-rw-r--r--   0        0        0     6602 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/providers/aurora.py
+-rw-r--r--   0        0        0     9562 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/providers/auto.py
+-rw-r--r--   0        0        0    13916 2022-04-19 10:33:53.855407 dns-lexicon-3.9.5/lexicon/providers/azure.py
+-rw-r--r--   0        0        0     8018 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/base.py
+-rw-r--r--   0        0        0     8160 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/cloudflare.py
+-rw-r--r--   0        0        0     8480 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/cloudns.py
+-rw-r--r--   0        0        0     6636 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/cloudxns.py
+-rw-r--r--   0        0        0     8059 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/conoha.py
+-rw-r--r--   0        0        0    10184 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/constellix.py
+-rw-r--r--   0        0        0     6411 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/ddns.py
+-rw-r--r--   0        0        0     5269 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/digitalocean.py
+-rw-r--r--   0        0        0     9612 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/dinahosting.py
+-rw-r--r--   0        0        0     8488 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/directadmin.py
+-rw-r--r--   0        0        0     7917 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/dnsimple.py
+-rw-r--r--   0        0        0     7967 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/dnsmadeeasy.py
+-rw-r--r--   0        0        0     4726 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/dnspark.py
+-rw-r--r--   0        0        0     5607 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/dnspod.py
+-rw-r--r--   0        0        0     8038 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/dreamhost.py
+-rw-r--r--   0        0        0    10276 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/dynu.py
+-rw-r--r--   0        0        0     5400 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/easydns.py
+-rw-r--r--   0        0        0    18721 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/easyname.py
+-rw-r--r--   0        0        0     9029 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/euserv.py
+-rw-r--r--   0        0        0     5829 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/exoscale.py
+-rw-r--r--   0        0        0    20642 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/gandi.py
+-rw-r--r--   0        0        0    11044 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/gehirn.py
+-rw-r--r--   0        0        0     5566 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/glesys.py
+-rw-r--r--   0        0        0    13763 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/godaddy.py
+-rw-r--r--   0        0        0    21795 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/googleclouddns.py
+-rw-r--r--   0        0        0    13059 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/gransy.py
+-rw-r--r--   0        0        0    10782 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/gratisdns.py
+-rw-r--r--   0        0        0     9057 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/henet.py
+-rw-r--r--   0        0        0     7560 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/hetzner.py
+-rw-r--r--   0        0        0     9267 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/hostingde.py
+-rw-r--r--   0        0        0     6782 2022-04-19 10:33:53.859407 dns-lexicon-3.9.5/lexicon/providers/hover.py
+-rw-r--r--   0        0        0    13978 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/infoblox.py
+-rw-r--r--   0        0        0     6243 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/infomaniak.py
+-rw-r--r--   0        0        0     7679 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/internetbs.py
+-rw-r--r--   0        0        0     7405 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/inwx.py
+-rw-r--r--   0        0        0    12665 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/joker.py
+-rw-r--r--   0        0        0     5439 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/linode.py
+-rw-r--r--   0        0        0     5660 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/linode4.py
+-rw-r--r--   0        0        0     5583 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/localzone.py
+-rw-r--r--   0        0        0     4850 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/luadns.py
+-rw-r--r--   0        0        0     5628 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/memset.py
+-rw-r--r--   0        0        0     8880 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/misaka.py
+-rw-r--r--   0        0        0    10918 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/mythicbeasts.py
+-rw-r--r--   0        0        0    17678 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/namecheap.py
+-rw-r--r--   0        0        0     5524 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/namesilo.py
+-rw-r--r--   0        0        0     7063 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/netcup.py
+-rw-r--r--   0        0        0     6218 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/nfsn.py
+-rw-r--r--   0        0        0     5139 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/njalla.py
+-rw-r--r--   0        0        0     9181 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/nsone.py
+-rw-r--r--   0        0        0    12267 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/oci.py
+-rw-r--r--   0        0        0     7161 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/onapp.py
+-rw-r--r--   0        0        0     8515 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/online.py
+-rw-r--r--   0        0        0     8357 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/ovh.py
+-rw-r--r--   0        0        0    10087 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/plesk.py
+-rw-r--r--   0        0        0     4896 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/pointhq.py
+-rw-r--r--   0        0        0     9890 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/powerdns.py
+-rw-r--r--   0        0        0     9893 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/rackspace.py
+-rw-r--r--   0        0        0     5281 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/rage4.py
+-rw-r--r--   0        0        0     8325 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/rcodezero.py
+-rw-r--r--   0        0        0    13549 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/route53.py
+-rw-r--r--   0        0        0     7744 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/safedns.py
+-rw-r--r--   0        0        0     8087 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/sakuracloud.py
+-rw-r--r--   0        0        0     5085 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/softlayer.py
+-rw-r--r--   0        0        0     9287 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/transip.py
+-rw-r--r--   0        0        0    10016 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/ultradns.py
+-rw-r--r--   0        0        0    25184 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/valuedomain.py
+-rw-r--r--   0        0        0     6402 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/vercel.py
+-rw-r--r--   0        0        0     6872 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/vultr.py
+-rw-r--r--   0        0        0    12408 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/webgo.py
+-rw-r--r--   0        0        0     6721 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/yandex.py
+-rw-r--r--   0        0        0      626 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/zeit.py
+-rw-r--r--   0        0        0     6493 2022-04-19 10:33:53.863407 dns-lexicon-3.9.5/lexicon/providers/zilore.py
+-rw-r--r--   0        0        0     6937 2022-04-19 10:33:53.867408 dns-lexicon-3.9.5/lexicon/providers/zonomi.py
+-rw-r--r--   0        0        0        0 2022-04-19 10:33:53.867408 dns-lexicon-3.9.5/lexicon/tests/__init__.py
+-rw-r--r--   0        0        0     6582 2022-04-19 10:33:53.867408 dns-lexicon-3.9.5/lexicon/tests/test_client.py
+-rw-r--r--   0        0        0     4494 2022-04-19 10:33:53.867408 dns-lexicon-3.9.5/lexicon/tests/test_config.py
+-rw-r--r--   0        0        0     9449 2022-04-19 10:33:53.867408 dns-lexicon-3.9.5/lexicon/tests/test_library.py
+-rw-r--r--   0        0        0     2148 2022-04-19 10:33:53.867408 dns-lexicon-3.9.5/lexicon/tests/test_output.py
+-rw-r--r--   0        0        0     1305 2022-04-19 10:33:53.867408 dns-lexicon-3.9.5/lexicon/tests/test_parser.py
+-rw-r--r--   0        0        0     2365 2022-04-19 10:33:53.871408 dns-lexicon-3.9.5/pyproject.toml
+-rw-r--r--   0        0        0     8984 2022-04-19 10:34:03.664346 dns-lexicon-3.9.5/setup.py
+-rw-r--r--   0        0        0     9398 2022-04-19 10:34:03.665019 dns-lexicon-3.9.5/PKG-INFO
```

### Comparing `dns-lexicon-3.9.4/LICENSE` & `dns-lexicon-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/README.rst` & `dns-lexicon-3.9.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 - `Internet.bs <https://internetbs.net/ResellerRegistrarDomainNameAPI>`_
 - `INWX <https://www.inwx.de/en/offer/api>`_
 - `Joker.com <https://joker.com/faq/index.php?action=show&cat=39>`_
 - `Linode <https://www.linode.com/api/dns>`_
 - `Linode v4 <https://developers.linode.com/api/docs/v4#tag/Domains>`_
 - `LuaDNS <http://www.luadns.com/api.html>`_
 - `Memset <https://www.memset.com/apidocs/methods_dns.html>`_
+- `Misaka.io <https://misaka.io/dns/>`_
 - `Mythic Beasts (v2 API) <https://www.mythic-beasts.com/support/api/dnsv2>`_
 - `Njalla <https://njal.la/api/>`_
 - `Namecheap <https://www.namecheap.com/support/api/methods.aspx>`_
 - `Namesilo <https://www.namesilo.com/api_reference.php>`_
 - `Netcup <https://ccp.netcup.net/run/webservice/servers/endpoint.php>`_
 - NFSN (NearlyFreeSpeech)
 - `NS1 <https://ns1.com/api/>`_
```

### Comparing `dns-lexicon-3.9.4/lexicon/cli.py` & `dns-lexicon-3.9.5/lexicon/cli.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/client.py` & `dns-lexicon-3.9.5/lexicon/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Main module of Lexicon. Defines the Client class, that holds all Lexicon logic."""
 import importlib
 import logging
 import os
-from typing import Dict, List, Optional, Type, Union
+from typing import Dict, List, Optional, Type, Union, cast
 
 import tldextract  # type: ignore
 
 from lexicon import config as helper_config
 from lexicon import discovery
 from lexicon.exceptions import ProviderNotAvailableError
 from lexicon.providers.base import Provider
@@ -38,15 +38,17 @@
             domain_extractor = tldextract.TLDExtract(
                 cache_dir=_get_tldextract_cache_path(), include_psl_private_domains=True
             )
         except TypeError:
             domain_extractor = tldextract.TLDExtract(
                 cache_file=_get_tldextract_cache_path(), include_psl_private_domains=True  # type: ignore
             )
-        domain_parts = domain_extractor(self.config.resolve("lexicon:domain"))
+        domain_parts = domain_extractor(
+            cast(str, self.config.resolve("lexicon:domain"))
+        )
         runtime_config["domain"] = f"{domain_parts.domain}.{domain_parts.suffix}"
 
         delegated = self.config.resolve("lexicon:delegated")
         if delegated:
             # handle delegated domain
             delegated = str(delegated).rstrip(".")
             initial_domain = str(runtime_config.get("domain"))
```

### Comparing `dns-lexicon-3.9.4/lexicon/config.py` & `dns-lexicon-3.9.5/lexicon/config.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/conftest.py` & `dns-lexicon-3.9.5/lexicon/conftest.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/discovery.py` & `dns-lexicon-3.9.5/lexicon/discovery.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/parser.py` & `dns-lexicon-3.9.5/lexicon/parser.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/aliyun.py` & `dns-lexicon-3.9.5/lexicon/providers/aliyun.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/aurora.py` & `dns-lexicon-3.9.5/lexicon/providers/aurora.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/auto.py` & `dns-lexicon-3.9.5/lexicon/providers/auto.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/azure.py` & `dns-lexicon-3.9.5/lexicon/providers/azure.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/base.py` & `dns-lexicon-3.9.5/lexicon/providers/base.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/cloudflare.py` & `dns-lexicon-3.9.5/lexicon/providers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/cloudns.py` & `dns-lexicon-3.9.5/lexicon/providers/cloudns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/cloudxns.py` & `dns-lexicon-3.9.5/lexicon/providers/cloudxns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/conoha.py` & `dns-lexicon-3.9.5/lexicon/providers/conoha.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/constellix.py` & `dns-lexicon-3.9.5/lexicon/providers/constellix.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/ddns.py` & `dns-lexicon-3.9.5/lexicon/providers/ddns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/digitalocean.py` & `dns-lexicon-3.9.5/lexicon/providers/digitalocean.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/dinahosting.py` & `dns-lexicon-3.9.5/lexicon/providers/dinahosting.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/directadmin.py` & `dns-lexicon-3.9.5/lexicon/providers/directadmin.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/dnsimple.py` & `dns-lexicon-3.9.5/lexicon/providers/dnsimple.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/dnsmadeeasy.py` & `dns-lexicon-3.9.5/lexicon/providers/dnsmadeeasy.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/dnspark.py` & `dns-lexicon-3.9.5/lexicon/providers/dnspark.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/dnspod.py` & `dns-lexicon-3.9.5/lexicon/providers/dnspod.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/dreamhost.py` & `dns-lexicon-3.9.5/lexicon/providers/dreamhost.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/dynu.py` & `dns-lexicon-3.9.5/lexicon/providers/dynu.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/easydns.py` & `dns-lexicon-3.9.5/lexicon/providers/easydns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/easyname.py` & `dns-lexicon-3.9.5/lexicon/providers/easyname.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/euserv.py` & `dns-lexicon-3.9.5/lexicon/providers/euserv.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/exoscale.py` & `dns-lexicon-3.9.5/lexicon/providers/exoscale.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/gandi.py` & `dns-lexicon-3.9.5/lexicon/providers/gandi.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/gehirn.py` & `dns-lexicon-3.9.5/lexicon/providers/gehirn.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/glesys.py` & `dns-lexicon-3.9.5/lexicon/providers/glesys.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/godaddy.py` & `dns-lexicon-3.9.5/lexicon/providers/godaddy.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/googleclouddns.py` & `dns-lexicon-3.9.5/lexicon/providers/googleclouddns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/gransy.py` & `dns-lexicon-3.9.5/lexicon/providers/gransy.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/gratisdns.py` & `dns-lexicon-3.9.5/lexicon/providers/gratisdns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/henet.py` & `dns-lexicon-3.9.5/lexicon/providers/henet.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/hetzner.py` & `dns-lexicon-3.9.5/lexicon/providers/hetzner.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/hostingde.py` & `dns-lexicon-3.9.5/lexicon/providers/hostingde.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/hover.py` & `dns-lexicon-3.9.5/lexicon/providers/hover.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/infoblox.py` & `dns-lexicon-3.9.5/lexicon/providers/infoblox.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/infomaniak.py` & `dns-lexicon-3.9.5/lexicon/providers/infomaniak.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/internetbs.py` & `dns-lexicon-3.9.5/lexicon/providers/internetbs.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/inwx.py` & `dns-lexicon-3.9.5/lexicon/providers/inwx.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/joker.py` & `dns-lexicon-3.9.5/lexicon/providers/joker.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,21 +58,21 @@
         super(Provider, self).__init__(config)
         self.domain_id = None
         self._session_id = None
 
     def _authenticate(self):
         auth_token = self._get_provider_option("auth_token")
 
-        response = requests.get(API_BASE_URL + "/login", params={"api-key": auth_token})
+        response = requests.post(API_BASE_URL + "/login", data={"api-key": auth_token})
 
         result = _process_response(response)
         self._session_id = result.headers["Auth-Sid"]
 
-        response = self._get(
-            "/query-domain-list", query_params={"pattern": self.domain, "showstatus": 1}
+        response = self._post(
+            "/query-domain-list", data={"pattern": self.domain, "showstatus": 1}
         )
 
         if not response.data:
             raise AuthenticationError(
                 f"Domain {self.domain} is not registered with this account."
             )
 
@@ -83,25 +83,25 @@
         if len(set(domain_status).difference(["production", "lock", "autorenew"])) > 0:
             raise AuthenticationError(
                 f"Current status for domain {self.domain} is: {items[2]}"
             )
 
         self.domain_id = self.domain
 
-    def _request(self, action="GET", url="/", data=None, query_params=None):
-        if not query_params:
-            query_params = {}
+    def _request(self, action="POST", url="/", data=None, query_params=None):
+        if not data:
+            data = {}
 
-        query_params["auth-sid"] = self._session_id
+        data["auth-sid"] = self._session_id
 
-        response = requests.get(API_BASE_URL + url, params=query_params)
+        response = requests.post(API_BASE_URL + url, data=data)
         return _process_response(response)
 
     def _list_records(self, rtype=None, name=None, content=None):
-        response = self._get("/dns-zone-get", query_params={"domain": self.domain_id})
+        response = self._post("/dns-zone-get", data={"domain": self.domain_id})
         zone_data = _extract_zonedata(response.data)
 
         zone_data = [entry for entry in zone_data if entry["type"]]
 
         if rtype:
             zone_data = [entry for entry in zone_data if entry["type"] == rtype]
         if name:
@@ -132,15 +132,15 @@
 
     def _create_record(self, rtype, name, content):
         if not rtype or not name or not content:
             raise Exception(
                 "Error, rtype, name and content are mandatory to create a record."
             )
 
-        response = self._get("/dns-zone-get", query_params={"domain": self.domain_id})
+        response = self._post("/dns-zone-get", data={"domain": self.domain_id})
         zonedata = _extract_zonedata(response.data)
 
         new_entry = {
             "label": self._relative_name(name),
             "type": rtype,
             "pri": 0,
             "target": content,
@@ -168,15 +168,15 @@
 
     def _update_record(self, identifier, rtype=None, name=None, content=None):
         if not identifier and not (rtype and name):
             raise Exception(
                 "Error, either identifier or rtype + name are mandatory to update a record."
             )
 
-        response = self._get("/dns-zone-get", query_params={"domain": self.domain_id})
+        response = self._post("/dns-zone-get", data={"domain": self.domain_id})
         zonedata = _extract_zonedata(response.data)
 
         selector_info = (
             f"identifier={identifier}" if identifier else f"type={rtype},name={name}"
         )
 
         if identifier:
@@ -215,15 +215,15 @@
 
     def _delete_record(self, identifier=None, rtype=None, name=None, content=None):
         if not identifier and not rtype:
             raise Exception(
                 "Error, either rtype or identifier are mandatory to delete a record."
             )
 
-        response = self._get("/dns-zone-get", query_params={"domain": self.domain_id})
+        response = self._post("/dns-zone-get", data={"domain": self.domain_id})
         zonedata = _extract_zonedata(response.data)
 
         if identifier:
             zonedata = [
                 entry for entry in zonedata if self._identifier(entry) != identifier
             ]
         else:
@@ -263,17 +263,17 @@
                     line = f"{line} {entry['valid-from']} {entry['valid-to']}"
 
                 if entry["parameters"] is not None:
                     line = f"{line} {entry['parameters']}"
 
                 data.append(line)
 
-        self._get(
+        self._post(
             "/dns-zone-put",
-            query_params={"domain": self.domain_id, "zone": "\n".join(data)},
+            data={"domain": self.domain_id, "zone": "\n".join(data)},
         )
 
     def _identifier(self, record):
         if "raw" in record:
             return None
 
         digest = hashes.Hash(hashes.SHA256(), backend=default_backend())
```

### Comparing `dns-lexicon-3.9.4/lexicon/providers/linode.py` & `dns-lexicon-3.9.5/lexicon/providers/linode.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/linode4.py` & `dns-lexicon-3.9.5/lexicon/providers/linode4.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/localzone.py` & `dns-lexicon-3.9.5/lexicon/providers/localzone.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/luadns.py` & `dns-lexicon-3.9.5/lexicon/providers/luadns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/memset.py` & `dns-lexicon-3.9.5/lexicon/providers/memset.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/mythicbeasts.py` & `dns-lexicon-3.9.5/lexicon/providers/mythicbeasts.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/namecheap.py` & `dns-lexicon-3.9.5/lexicon/providers/namecheap.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/namesilo.py` & `dns-lexicon-3.9.5/lexicon/providers/namesilo.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/netcup.py` & `dns-lexicon-3.9.5/lexicon/providers/netcup.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/nfsn.py` & `dns-lexicon-3.9.5/lexicon/providers/nfsn.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/njalla.py` & `dns-lexicon-3.9.5/lexicon/providers/njalla.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/nsone.py` & `dns-lexicon-3.9.5/lexicon/providers/nsone.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/oci.py` & `dns-lexicon-3.9.5/lexicon/providers/oci.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/onapp.py` & `dns-lexicon-3.9.5/lexicon/providers/onapp.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/online.py` & `dns-lexicon-3.9.5/lexicon/providers/online.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/ovh.py` & `dns-lexicon-3.9.5/lexicon/providers/ovh.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/plesk.py` & `dns-lexicon-3.9.5/lexicon/providers/plesk.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/pointhq.py` & `dns-lexicon-3.9.5/lexicon/providers/pointhq.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/powerdns.py` & `dns-lexicon-3.9.5/lexicon/providers/powerdns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/rackspace.py` & `dns-lexicon-3.9.5/lexicon/providers/rackspace.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/rage4.py` & `dns-lexicon-3.9.5/lexicon/providers/rage4.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/rcodezero.py` & `dns-lexicon-3.9.5/lexicon/providers/rcodezero.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/route53.py` & `dns-lexicon-3.9.5/lexicon/providers/route53.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/safedns.py` & `dns-lexicon-3.9.5/lexicon/providers/safedns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/sakuracloud.py` & `dns-lexicon-3.9.5/lexicon/providers/sakuracloud.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/softlayer.py` & `dns-lexicon-3.9.5/lexicon/providers/softlayer.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/transip.py` & `dns-lexicon-3.9.5/lexicon/providers/transip.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/ultradns.py` & `dns-lexicon-3.9.5/lexicon/providers/ultradns.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/valuedomain.py` & `dns-lexicon-3.9.5/lexicon/providers/valuedomain.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/vercel.py` & `dns-lexicon-3.9.5/lexicon/providers/vercel.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/vultr.py` & `dns-lexicon-3.9.5/lexicon/providers/vultr.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/webgo.py` & `dns-lexicon-3.9.5/lexicon/providers/webgo.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/yandex.py` & `dns-lexicon-3.9.5/lexicon/providers/yandex.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,19 +68,34 @@
                 and "next" in payload["links"]["pages"]
             ):
                 next_url = payload["links"]["pages"]["next"]
             else:
                 next_url = None
 
             for record in payload["records"]:
+                if record["type"] == "MX":
+                    assembled_content = f"{record['priority']} {record['content']}"
+                if record["type"] == "SRV":
+                    if "target" in record:
+                        srv_target = record["target"]
+                    else:
+                        srv_target = record["content"]
+                    assembled_content = f"{record['priority']} {record['weight']} {record['port']} {srv_target}"
+                else:
+                    assembled_content = record.get("content")
+                record_name = (
+                    f"{record['subdomain']}.{self.domain_id}"
+                    if record["subdomain"] != "@"
+                    else self.domain_id
+                )
                 processed_record = {
                     "type": record["type"],
-                    "name": f"{record['subdomain']}.{self.domain_id}",
+                    "name": record_name,
                     "ttl": record["ttl"],
-                    "content": record.get("content"),
+                    "content": assembled_content,
                     "id": record["record_id"],
                 }
                 records.append(processed_record)
 
         if rtype:
             records = [record for record in records if record["type"] == rtype]
         if name:
```

### Comparing `dns-lexicon-3.9.4/lexicon/providers/zeit.py` & `dns-lexicon-3.9.5/lexicon/providers/zeit.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/zilore.py` & `dns-lexicon-3.9.5/lexicon/providers/zilore.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/providers/zonomi.py` & `dns-lexicon-3.9.5/lexicon/providers/zonomi.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/tests/test_client.py` & `dns-lexicon-3.9.5/lexicon/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/tests/test_config.py` & `dns-lexicon-3.9.5/lexicon/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/tests/test_library.py` & `dns-lexicon-3.9.5/lexicon/tests/test_library.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/tests/test_output.py` & `dns-lexicon-3.9.5/lexicon/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/lexicon/tests/test_parser.py` & `dns-lexicon-3.9.5/lexicon/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `dns-lexicon-3.9.4/pyproject.toml` & `dns-lexicon-3.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dns-lexicon"
-version = "3.9.4"
+version = "3.9.5"
 description = "Manipulate DNS records on various DNS providers in a standardized/agnostic way"
 license = "MIT"
 keywords = [
     "dns", "lexicon", "dns-lexicon", "dehydrated", "letsencrypt",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `dns-lexicon-3.9.4/setup.py` & `dns-lexicon-3.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
  'softlayer': ['softlayer>=5']}
 
 entry_points = \
 {'console_scripts': ['lexicon = lexicon.cli:main']}
 
 setup_kwargs = {
     'name': 'dns-lexicon',
-    'version': '3.9.4',
+    'version': '3.9.5',
     'description': 'Manipulate DNS records on various DNS providers in a standardized/agnostic way',
-    'long_description': '============\n|logo_named|\n============\n\nManipulate DNS records on various DNS providers in a standardized/agnostic way.\n\n|build_status| |coverage_status| |docker_pulls| |pypy_version| |pypy_python_support| |github_license|\n\n.. |logo_named| image:: https://raw.githubusercontent.com/AnalogJ/lexicon/master/docs/images/logo_named.svg\n    :alt: Lexicon\n\n.. |build_status| image:: https://dev.azure.com/AnalogJ/lexicon/_apis/build/status/AnalogJ.lexicon?branchName=master\n    :target: https://dev.azure.com/AnalogJ/lexicon/_build/latest?definitionId=1&branchName=master\n\n.. |coverage_status| image:: https://coveralls.io/repos/github/AnalogJ/lexicon/badge.svg\n    :target: https://coveralls.io/github/AnalogJ/lexicon?branch=master\n\n.. |docker_pulls| image:: https://img.shields.io/docker/pulls/analogj/lexicon.svg\n    :target: https://hub.docker.com/r/analogj/lexicon\n\n.. |pypy_version| image:: https://img.shields.io/pypi/v/dns-lexicon.svg\n    :target: https://pypi.python.org/pypi/dns-lexicon\n\n.. |pypy_python_support| image:: https://img.shields.io/pypi/pyversions/dns-lexicon.svg\n    :target: https://pypi.python.org/pypi/dns-lexicon\n\n.. |github_license| image:: https://img.shields.io/github/license/AnalogJ/lexicon.svg\n    :target: https://github.com/AnalogJ/lexicon/blob/master/LICENSE\n\n.. contents:: Table of Contents\n   :local:\n\n.. tag:intro-begin\n\nWhy using Lexicon?\n==================\n\nLexicon provides a way to manipulate DNS records on multiple DNS providers in a standardized way.\n\nLexicon can be used as:\n\n- a CLI tool:\n\n.. code-block:: bash\n\n    # Create a TXT entry in domain.net zone hosted by CloudFlare\n    lexicon cloudflare create domain.net TXT --name foo --content bar\n\n- or a Python library:\n\n.. code-block:: python\n\n    # Create a TXT entry in domain.net zone hosted by CloudFlare\n    from lexicon.client import Client\n    from lexicon.config import ConfigResolver\n\n    action = {\n        "provider_name" : "cloudflare",\n        "action": "create",\n        "domain": "domain.net",\n        "type": "TXT",\n        "name": "foo",\n        "content": "bar",\n    }\n    config = ConfigResolver().with_env().with_dict(action)\n    Client(config).execute()\n\nLexicon was designed to be used in automation, specifically letsencrypt.\n\n* `Generating Intranet & Private Network SSL Certificates using Lets Encrypt & Lexicon <http://blog.thesparktree.com/post/138999997429/generating-intranet-and-private-network-ssl>`_\n\nSupported providers\n===================\n\nOnly DNS providers who have an API can be supported by `lexicon`.\n\nThe current supported providers are:\n\n- `Aliyun.com <https://help.aliyun.com/document_detail/29739.html>`_\n- `AuroraDNS <https://www.pcextreme.com/aurora/dns>`_\n- `AWS Route53 <https://docs.aws.amazon.com/Route53/latest/APIReference/Welcome.html>`_\n- `Azure DNS <https://docs.microsoft.com/en-us/rest/api/dns/>`_\n- `Cloudflare <https://api.cloudflare.com/#endpoints>`_\n- `ClouDNS <https://www.cloudns.net/wiki/article/56/>`_\n- `CloudXNS <https://www.cloudxns.net/Support/lists/cid/17.html>`_\n- `ConoHa <https://www.conoha.jp/docs/>`_\n- `Constellix <https://api-docs.constellix.com/?version=latest>`_\n- `DigitalOcean <https://developers.digitalocean.com/documentation/v2/#create-a-new-domain>`_\n- `Dinahosting <https://en.dinahosting.com/api>`_\n- `DirectAdmin <https://www.directadmin.com/features.php?id=504>`_\n- DNSimple `v1 <https://developer.dnsimple.com/>`_, `v2 <https://developer.dnsimple.com/v2/>`_\n- `DnsMadeEasy <https://api-docs.dnsmadeeasy.com/?version=latest>`_\n- `DNSPark <https://dnspark.zendesk.com/entries/31210577-REST-API-DNS-Documentation>`_\n- `DNSPod <https://support.dnspod.cn/Support/api>`_\n- `Dreamhost <https://help.dreamhost.com/hc/en-us/articles/217560167-API_overview>`_\n- `Dynu <https://www.dynu.com/Support/API>`_\n- `EasyDNS <http://docs.sandbox.rest.easydns.net/>`_\n- `Easyname <https://www.easyname.com/en>`_\n- `EUserv <https://support.euserv.com/api-doc/>`_\n- `ExoScale <https://community.exoscale.com/documentation/dns/api/>`_\n- Gandi `RPC (old) <http://doc.rpc.gandi.net>`_ / `LiveAPI <http://doc.livedns.gandi.net/>`_\n- `Gehirn <https://support.gehirn.jp/apidocs/gis/dns/index.html>`_\n- `Glesys <https://github.com/glesys/API/wiki/>`_\n- `GoDaddy <https://developer.godaddy.com/getstarted#access>`_\n- `Google Cloud DNS <https://cloud.google.com/dns/api/v1/>`_\n- `Gransy (sites subreg.cz, regtons.com and regnames.eu) <https://subreg.cz/manual/>`_\n- `Hover <https://hoverapi.docs.apiary.io/>`_\n- `Hurricane Electric DNS <https://dns.he.net/>`_\n- `Hetzner <https://dns.hetzner.com/api-docs/>`_\n- `Infoblox <https://docs.infoblox.com/display/ILP/Infoblox+Documentation+Portal>`_\n- `Infomaniak <https://www.infomaniak.com>`_\n- `Internet.bs <https://internetbs.net/ResellerRegistrarDomainNameAPI>`_\n- `INWX <https://www.inwx.de/en/offer/api>`_\n- `Joker.com <https://joker.com/faq/index.php?action=show&cat=39>`_\n- `Linode <https://www.linode.com/api/dns>`_\n- `Linode v4 <https://developers.linode.com/api/docs/v4#tag/Domains>`_\n- `LuaDNS <http://www.luadns.com/api.html>`_\n- `Memset <https://www.memset.com/apidocs/methods_dns.html>`_\n- `Mythic Beasts (v2 API) <https://www.mythic-beasts.com/support/api/dnsv2>`_\n- `Njalla <https://njal.la/api/>`_\n- `Namecheap <https://www.namecheap.com/support/api/methods.aspx>`_\n- `Namesilo <https://www.namesilo.com/api_reference.php>`_\n- `Netcup <https://ccp.netcup.net/run/webservice/servers/endpoint.php>`_\n- NFSN (NearlyFreeSpeech)\n- `NS1 <https://ns1.com/api/>`_\n- `OnApp <https://docs.onapp.com/display/55API/OnApp+5.5+API+Guide>`_\n- Online\n- `OVH <https://api.ovh.com/>`_\n- `Plesk <https://docs.plesk.com/en-US/onyx/api-rpc/about-xml-api.28709/>`_\n- `PointHQ <https://pointhq.com/api/docs>`_\n- `PowerDNS <https://doc.powerdns.com/md/httpapi/api_spec/>`_\n- `Rackspace <https://developer.rackspace.com/docs/cloud-dns/v1/developer-guide/>`_\n- `Rage4 <https://gbshouse.uservoice.com/knowledgebase/articles/109834-rage4-dns-developers-api>`_\n- `RcodeZero <https://my.rcodezero.at/api-doc>`_\n- `RFC2136 <https://en.wikipedia.org/wiki/Dynamic_DNS>`_\n- `Sakura Cloud by SAKURA Internet Inc. <https://developer.sakura.ad.jp/cloud/api/1.1/>`_\n- `SafeDNS by UKFast <https://developers.ukfast.io/documentation/safedns>`_\n- `SoftLayer <https://sldn.softlayer.com/article/REST#HTTP_Request_Types>`_\n- `Transip <https://api.transip.nl/rest/docs.html>`_\n- `UltraDNS <https://ultra-portalstatic.ultradns.com/static/docs/REST-API_User_Guide.pdf>`_\n- `Value-Domain <https://www.value-domain.com/service/api/>`_\n- `Vercel <https://vercel.com/docs/api#endpoints/dns>`_\n- `Vultr <https://www.vultr.com/api/#tag/dns>`_\n- `WebGo <https://www.webgo.de/>`_\n- `Yandex <https://tech.yandex.com/domain/doc/reference/dns-add-docpage/>`_\n- `Zilore <https://zilore.com/en/help/api>`_\n- `Zonomi <http://zonomi.com/app/dns/dyndns.jsp>`_\n\n.. tag:intro-end\n\nDocumentation\n=============\n\nOnline documentation (user guide, configuration reference) is available in the `Lexicon documentation`_.\n\nFor a quick start, please have a look in particular at the `User guide`_.\n\n.. _Lexicon documentation: https://dns-lexicon.readthedocs.io\n.. _User guide: https://dns-lexicon.readthedocs.io/en/latest/user_guide.html\n\nContributing\n============\n\nIf you want to help in the Lexicon development, you are welcome!\n\nPlease have a look at the `Developer guide`_ page to know how to start.\n\n.. _Developer guide: https://dns-lexicon.readthedocs.io/en/latest/developer_guide.html\n\nLicensing\n=========\n\n- MIT\n- Logo_: transform by Mike Rowe from the Noun Project\n\n.. _Logo: https://thenounproject.com/term/transform/397964\n',
+    'long_description': '============\n|logo_named|\n============\n\nManipulate DNS records on various DNS providers in a standardized/agnostic way.\n\n|build_status| |coverage_status| |docker_pulls| |pypy_version| |pypy_python_support| |github_license|\n\n.. |logo_named| image:: https://raw.githubusercontent.com/AnalogJ/lexicon/master/docs/images/logo_named.svg\n    :alt: Lexicon\n\n.. |build_status| image:: https://dev.azure.com/AnalogJ/lexicon/_apis/build/status/AnalogJ.lexicon?branchName=master\n    :target: https://dev.azure.com/AnalogJ/lexicon/_build/latest?definitionId=1&branchName=master\n\n.. |coverage_status| image:: https://coveralls.io/repos/github/AnalogJ/lexicon/badge.svg\n    :target: https://coveralls.io/github/AnalogJ/lexicon?branch=master\n\n.. |docker_pulls| image:: https://img.shields.io/docker/pulls/analogj/lexicon.svg\n    :target: https://hub.docker.com/r/analogj/lexicon\n\n.. |pypy_version| image:: https://img.shields.io/pypi/v/dns-lexicon.svg\n    :target: https://pypi.python.org/pypi/dns-lexicon\n\n.. |pypy_python_support| image:: https://img.shields.io/pypi/pyversions/dns-lexicon.svg\n    :target: https://pypi.python.org/pypi/dns-lexicon\n\n.. |github_license| image:: https://img.shields.io/github/license/AnalogJ/lexicon.svg\n    :target: https://github.com/AnalogJ/lexicon/blob/master/LICENSE\n\n.. contents:: Table of Contents\n   :local:\n\n.. tag:intro-begin\n\nWhy using Lexicon?\n==================\n\nLexicon provides a way to manipulate DNS records on multiple DNS providers in a standardized way.\n\nLexicon can be used as:\n\n- a CLI tool:\n\n.. code-block:: bash\n\n    # Create a TXT entry in domain.net zone hosted by CloudFlare\n    lexicon cloudflare create domain.net TXT --name foo --content bar\n\n- or a Python library:\n\n.. code-block:: python\n\n    # Create a TXT entry in domain.net zone hosted by CloudFlare\n    from lexicon.client import Client\n    from lexicon.config import ConfigResolver\n\n    action = {\n        "provider_name" : "cloudflare",\n        "action": "create",\n        "domain": "domain.net",\n        "type": "TXT",\n        "name": "foo",\n        "content": "bar",\n    }\n    config = ConfigResolver().with_env().with_dict(action)\n    Client(config).execute()\n\nLexicon was designed to be used in automation, specifically letsencrypt.\n\n* `Generating Intranet & Private Network SSL Certificates using Lets Encrypt & Lexicon <http://blog.thesparktree.com/post/138999997429/generating-intranet-and-private-network-ssl>`_\n\nSupported providers\n===================\n\nOnly DNS providers who have an API can be supported by `lexicon`.\n\nThe current supported providers are:\n\n- `Aliyun.com <https://help.aliyun.com/document_detail/29739.html>`_\n- `AuroraDNS <https://www.pcextreme.com/aurora/dns>`_\n- `AWS Route53 <https://docs.aws.amazon.com/Route53/latest/APIReference/Welcome.html>`_\n- `Azure DNS <https://docs.microsoft.com/en-us/rest/api/dns/>`_\n- `Cloudflare <https://api.cloudflare.com/#endpoints>`_\n- `ClouDNS <https://www.cloudns.net/wiki/article/56/>`_\n- `CloudXNS <https://www.cloudxns.net/Support/lists/cid/17.html>`_\n- `ConoHa <https://www.conoha.jp/docs/>`_\n- `Constellix <https://api-docs.constellix.com/?version=latest>`_\n- `DigitalOcean <https://developers.digitalocean.com/documentation/v2/#create-a-new-domain>`_\n- `Dinahosting <https://en.dinahosting.com/api>`_\n- `DirectAdmin <https://www.directadmin.com/features.php?id=504>`_\n- DNSimple `v1 <https://developer.dnsimple.com/>`_, `v2 <https://developer.dnsimple.com/v2/>`_\n- `DnsMadeEasy <https://api-docs.dnsmadeeasy.com/?version=latest>`_\n- `DNSPark <https://dnspark.zendesk.com/entries/31210577-REST-API-DNS-Documentation>`_\n- `DNSPod <https://support.dnspod.cn/Support/api>`_\n- `Dreamhost <https://help.dreamhost.com/hc/en-us/articles/217560167-API_overview>`_\n- `Dynu <https://www.dynu.com/Support/API>`_\n- `EasyDNS <http://docs.sandbox.rest.easydns.net/>`_\n- `Easyname <https://www.easyname.com/en>`_\n- `EUserv <https://support.euserv.com/api-doc/>`_\n- `ExoScale <https://community.exoscale.com/documentation/dns/api/>`_\n- Gandi `RPC (old) <http://doc.rpc.gandi.net>`_ / `LiveAPI <http://doc.livedns.gandi.net/>`_\n- `Gehirn <https://support.gehirn.jp/apidocs/gis/dns/index.html>`_\n- `Glesys <https://github.com/glesys/API/wiki/>`_\n- `GoDaddy <https://developer.godaddy.com/getstarted#access>`_\n- `Google Cloud DNS <https://cloud.google.com/dns/api/v1/>`_\n- `Gransy (sites subreg.cz, regtons.com and regnames.eu) <https://subreg.cz/manual/>`_\n- `Hover <https://hoverapi.docs.apiary.io/>`_\n- `Hurricane Electric DNS <https://dns.he.net/>`_\n- `Hetzner <https://dns.hetzner.com/api-docs/>`_\n- `Infoblox <https://docs.infoblox.com/display/ILP/Infoblox+Documentation+Portal>`_\n- `Infomaniak <https://www.infomaniak.com>`_\n- `Internet.bs <https://internetbs.net/ResellerRegistrarDomainNameAPI>`_\n- `INWX <https://www.inwx.de/en/offer/api>`_\n- `Joker.com <https://joker.com/faq/index.php?action=show&cat=39>`_\n- `Linode <https://www.linode.com/api/dns>`_\n- `Linode v4 <https://developers.linode.com/api/docs/v4#tag/Domains>`_\n- `LuaDNS <http://www.luadns.com/api.html>`_\n- `Memset <https://www.memset.com/apidocs/methods_dns.html>`_\n- `Misaka.io <https://misaka.io/dns/>`_\n- `Mythic Beasts (v2 API) <https://www.mythic-beasts.com/support/api/dnsv2>`_\n- `Njalla <https://njal.la/api/>`_\n- `Namecheap <https://www.namecheap.com/support/api/methods.aspx>`_\n- `Namesilo <https://www.namesilo.com/api_reference.php>`_\n- `Netcup <https://ccp.netcup.net/run/webservice/servers/endpoint.php>`_\n- NFSN (NearlyFreeSpeech)\n- `NS1 <https://ns1.com/api/>`_\n- `OnApp <https://docs.onapp.com/display/55API/OnApp+5.5+API+Guide>`_\n- Online\n- `OVH <https://api.ovh.com/>`_\n- `Plesk <https://docs.plesk.com/en-US/onyx/api-rpc/about-xml-api.28709/>`_\n- `PointHQ <https://pointhq.com/api/docs>`_\n- `PowerDNS <https://doc.powerdns.com/md/httpapi/api_spec/>`_\n- `Rackspace <https://developer.rackspace.com/docs/cloud-dns/v1/developer-guide/>`_\n- `Rage4 <https://gbshouse.uservoice.com/knowledgebase/articles/109834-rage4-dns-developers-api>`_\n- `RcodeZero <https://my.rcodezero.at/api-doc>`_\n- `RFC2136 <https://en.wikipedia.org/wiki/Dynamic_DNS>`_\n- `Sakura Cloud by SAKURA Internet Inc. <https://developer.sakura.ad.jp/cloud/api/1.1/>`_\n- `SafeDNS by UKFast <https://developers.ukfast.io/documentation/safedns>`_\n- `SoftLayer <https://sldn.softlayer.com/article/REST#HTTP_Request_Types>`_\n- `Transip <https://api.transip.nl/rest/docs.html>`_\n- `UltraDNS <https://ultra-portalstatic.ultradns.com/static/docs/REST-API_User_Guide.pdf>`_\n- `Value-Domain <https://www.value-domain.com/service/api/>`_\n- `Vercel <https://vercel.com/docs/api#endpoints/dns>`_\n- `Vultr <https://www.vultr.com/api/#tag/dns>`_\n- `WebGo <https://www.webgo.de/>`_\n- `Yandex <https://tech.yandex.com/domain/doc/reference/dns-add-docpage/>`_\n- `Zilore <https://zilore.com/en/help/api>`_\n- `Zonomi <http://zonomi.com/app/dns/dyndns.jsp>`_\n\n.. tag:intro-end\n\nDocumentation\n=============\n\nOnline documentation (user guide, configuration reference) is available in the `Lexicon documentation`_.\n\nFor a quick start, please have a look in particular at the `User guide`_.\n\n.. _Lexicon documentation: https://dns-lexicon.readthedocs.io\n.. _User guide: https://dns-lexicon.readthedocs.io/en/latest/user_guide.html\n\nContributing\n============\n\nIf you want to help in the Lexicon development, you are welcome!\n\nPlease have a look at the `Developer guide`_ page to know how to start.\n\n.. _Developer guide: https://dns-lexicon.readthedocs.io/en/latest/developer_guide.html\n\nLicensing\n=========\n\n- MIT\n- Logo_: transform by Mike Rowe from the Noun Project\n\n.. _Logo: https://thenounproject.com/term/transform/397964\n',
     'author': 'Jason Kulatunga',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/AnalogJ/lexicon',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dns-lexicon-3.9.4/PKG-INFO` & `dns-lexicon-3.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dns-lexicon
-Version: 3.9.4
+Version: 3.9.5
 Summary: Manipulate DNS records on various DNS providers in a standardized/agnostic way
 Home-page: https://github.com/AnalogJ/lexicon
 License: MIT
 Keywords: dns,lexicon,dns-lexicon,dehydrated,letsencrypt
 Author: Jason Kulatunga
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -155,14 +155,15 @@
 - `Internet.bs <https://internetbs.net/ResellerRegistrarDomainNameAPI>`_
 - `INWX <https://www.inwx.de/en/offer/api>`_
 - `Joker.com <https://joker.com/faq/index.php?action=show&cat=39>`_
 - `Linode <https://www.linode.com/api/dns>`_
 - `Linode v4 <https://developers.linode.com/api/docs/v4#tag/Domains>`_
 - `LuaDNS <http://www.luadns.com/api.html>`_
 - `Memset <https://www.memset.com/apidocs/methods_dns.html>`_
+- `Misaka.io <https://misaka.io/dns/>`_
 - `Mythic Beasts (v2 API) <https://www.mythic-beasts.com/support/api/dnsv2>`_
 - `Njalla <https://njal.la/api/>`_
 - `Namecheap <https://www.namecheap.com/support/api/methods.aspx>`_
 - `Namesilo <https://www.namesilo.com/api_reference.php>`_
 - `Netcup <https://ccp.netcup.net/run/webservice/servers/endpoint.php>`_
 - NFSN (NearlyFreeSpeech)
 - `NS1 <https://ns1.com/api/>`_
```

