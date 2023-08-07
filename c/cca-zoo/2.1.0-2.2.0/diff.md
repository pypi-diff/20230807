# Comparing `tmp/cca_zoo-2.1.0.tar.gz` & `tmp/cca_zoo-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cca_zoo-2.1.0.tar", max compression
+gzip compressed data, was "cca_zoo-2.2.0.tar", max compression
```

## Comparing `cca_zoo-2.1.0.tar` & `cca_zoo-2.2.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0     1069 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/LICENSE
--rw-r--r--   0        0        0     3999 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/README.md
--rw-r--r--   0        0        0      325 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/__init__.py
--rw-r--r--   0        0        0     7517 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/_base/__init__.py
--rw-r--r--   0        0        0       76 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/data/__init__.py
--rw-r--r--   0        0        0     3176 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/data/deep.py
--rw-r--r--   0        0        0     7074 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/data/simulated.py
--rw-r--r--   0        0        0      598 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/__init__.py
--rw-r--r--   0        0        0     5270 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_base.py
--rw-r--r--   0        0        0      426 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/__init__.py
--rw-r--r--   0        0        0     1777 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca.py
--rw-r--r--   0        0        0     2342 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
--rw-r--r--   0        0        0     2401 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_ey.py
--rw-r--r--   0        0        0     1275 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_gh.py
--rw-r--r--   0        0        0     2240 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_noi.py
--rw-r--r--   0        0        0     2539 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_sdl.py
--rw-r--r--   0        0        0     1681 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_svd.py
--rw-r--r--   0        0        0      676 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dgcca.py
--rw-r--r--   0        0        0      784 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dtcca.py
--rw-r--r--   0        0        0      123 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/__init__.py
--rw-r--r--   0        0        0     1449 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/_base.py
--rw-r--r--   0        0        0     2481 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/_dccae.py
--rw-r--r--   0        0        0     5339 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/_dvcca.py
--rw-r--r--   0        0        0     2051 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/_generative/_splitae.py
--rw-r--r--   0        0        0     9528 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/architectures.py
--rw-r--r--   0        0        0      337 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/callbacks.py
--rw-r--r--   0        0        0     1931 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/metrics.py
--rw-r--r--   0        0        0     8808 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/deep/objectives.py
--rw-r--r--   0        0        0      816 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/__init__.py
--rw-r--r--   0        0        0     1577 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_dummy.py
--rw-r--r--   0        0        0     3093 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gcca.py
--rw-r--r--   0        0        0      241 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/__init__.py
--rw-r--r--   0        0        0     8646 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_ey.py
--rw-r--r--   0        0        0     2223 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_gh.py
--rw-r--r--   0        0        0     1757 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_gradient.py
--rw-r--r--   0        0        0     1713 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_stochasticpls.py
--rw-r--r--   0        0        0     1738 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_gradient/_svd.py
--rw-r--r--   0        0        0     6599 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_grcca.py
--rw-r--r--   0        0        0      364 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/__init__.py
--rw-r--r--   0        0        0     7635 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_altmaxvar.py
--rw-r--r--   0        0        0    12323 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_base.py
--rw-r--r--   0        0        0     2459 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_deflation.py
--rw-r--r--   0        0        0    13319 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_elasticnet.py
--rw-r--r--   0        0        0     3789 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_incrementalpls.py
--rw-r--r--   0        0        0     3261 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_pls_als.py
--rw-r--r--   0        0        0     6728 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_admm.py
--rw-r--r--   0        0        0     4181 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_parkhomenko.py
--rw-r--r--   0        0        0     7258 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_pmd.py
--rw-r--r--   0        0        0     4461 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_span.py
--rw-r--r--   0        0        0     3813 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_iterative/_swcca.py
--rw-r--r--   0        0        0    10291 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_mcca.py
--rw-r--r--   0        0        0     3086 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_partialcca.py
--rw-r--r--   0        0        0     1621 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_pcacca.py
--rw-r--r--   0        0        0    11322 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_pls.py
--rw-r--r--   0        0        0     4216 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_prcca.py
--rw-r--r--   0        0        0     2722 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_search.py
--rw-r--r--   0        0        0     4716 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/linear/_tcca.py
--rw-r--r--   0        0        0      269 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/model_selection/__init__.py
--rw-r--r--   0        0        0    11669 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/model_selection/_search.py
--rw-r--r--   0        0        0    18413 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/model_selection/_validation.py
--rw-r--r--   0        0        0      108 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/__init__.py
--rw-r--r--   0        0        0     5066 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/_gradkcca.py
--rw-r--r--   0        0        0    12301 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/_kcca.py
--rw-r--r--   0        0        0     6378 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/_ncca.py
--rw-r--r--   0        0        0     6280 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/nonparametric/_scca_hsic.py
--rw-r--r--   0        0        0       80 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/probabilistic/__init__.py
--rw-r--r--   0        0        0     4561 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/probabilistic/_probabilisticcca.py
--rw-r--r--   0        0        0      129 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/utils/__init__.py
--rw-r--r--   0        0        0     1581 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/utils/check_values.py
--rw-r--r--   0        0        0       52 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/visualisation/__init__.py
--rw-r--r--   0        0        0    15027 2023-07-02 02:30:32.782160 cca_zoo-2.1.0/cca_zoo/visualisation/plotter.py
--rw-r--r--   0        0        0     1167 2023-07-02 02:30:33.022161 cca_zoo-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     5266 1970-01-01 00:00:00.000000 cca_zoo-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/LICENSE
+-rw-r--r--   0        0        0     4261 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/README.md
+-rw-r--r--   0        0        0      333 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/__init__.py
+-rw-r--r--   0        0        0     7578 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/_base.py
+-rw-r--r--   0        0        0       63 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/data/__init__.py
+-rw-r--r--   0        0        0     3176 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/data/deep.py
+-rw-r--r--   0        0        0     7426 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/data/simulated.py
+-rw-r--r--   0        0        0      598 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/__init__.py
+-rw-r--r--   0        0        0     5270 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_base.py
+-rw-r--r--   0        0        0      426 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/__init__.py
+-rw-r--r--   0        0        0     1777 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca.py
+-rw-r--r--   0        0        0     2342 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
+-rw-r--r--   0        0        0     2401 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_ey.py
+-rw-r--r--   0        0        0     1275 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_gh.py
+-rw-r--r--   0        0        0     2240 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_noi.py
+-rw-r--r--   0        0        0     2539 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_sdl.py
+-rw-r--r--   0        0        0     1681 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_svd.py
+-rw-r--r--   0        0        0      676 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dgcca.py
+-rw-r--r--   0        0        0      784 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dtcca.py
+-rw-r--r--   0        0        0      123 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_generative/__init__.py
+-rw-r--r--   0        0        0     1449 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_generative/_base.py
+-rw-r--r--   0        0        0     2481 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_generative/_dccae.py
+-rw-r--r--   0        0        0     5339 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_generative/_dvcca.py
+-rw-r--r--   0        0        0     2051 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/_generative/_splitae.py
+-rw-r--r--   0        0        0     9528 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/architectures.py
+-rw-r--r--   0        0        0      337 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/callbacks.py
+-rw-r--r--   0        0        0     1900 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/metrics.py
+-rw-r--r--   0        0        0     8808 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/deep/objectives.py
+-rw-r--r--   0        0        0      820 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/linear/__init__.py
+-rw-r--r--   0        0        0     1577 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/linear/_dummy.py
+-rw-r--r--   0        0        0     3093 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/linear/_gcca.py
+-rw-r--r--   0        0        0      242 2023-08-07 13:23:10.785838 cca_zoo-2.2.0/cca_zoo/linear/_gradient/__init__.py
+-rw-r--r--   0        0        0    15543 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_gradient/_base.py
+-rw-r--r--   0        0        0     6692 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_gradient/_ey.py
+-rw-r--r--   0        0        0     2226 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_gradient/_gh.py
+-rw-r--r--   0        0        0     1704 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_gradient/_stochasticpls.py
+-rw-r--r--   0        0        0     1717 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_gradient/_svd.py
+-rw-r--r--   0        0        0     6599 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_grcca.py
+-rw-r--r--   0        0        0      367 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/__init__.py
+-rw-r--r--   0        0        0     8089 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_altmaxvar.py
+-rw-r--r--   0        0        0     6112 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_base.py
+-rw-r--r--   0        0        0     2641 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_deflation.py
+-rw-r--r--   0        0        0     8764 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_elastic.py
+-rw-r--r--   0        0        0     4008 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_incrementalpls.py
+-rw-r--r--   0        0        0     1663 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_pls_als.py
+-rw-r--r--   0        0        0     7032 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_scca_admm.py
+-rw-r--r--   0        0        0     2222 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0        0        0     3682 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_scca_pmd.py
+-rw-r--r--   0        0        0     3642 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_scca_span.py
+-rw-r--r--   0        0        0     3910 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_iterative/_swcca.py
+-rw-r--r--   0        0        0    10267 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_mcca.py
+-rw-r--r--   0        0        0     3086 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_partialcca.py
+-rw-r--r--   0        0        0     1621 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_pcacca.py
+-rw-r--r--   0        0        0    11323 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_pls.py
+-rw-r--r--   0        0        0     4216 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_prcca.py
+-rw-r--r--   0        0        0     2674 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_search.py
+-rw-r--r--   0        0        0     4716 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/linear/_tcca.py
+-rw-r--r--   0        0        0      269 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0        0        0     4008 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/model_selection/_search.py
+-rw-r--r--   0        0        0    17241 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/model_selection/_validation.py
+-rw-r--r--   0        0        0      108 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/nonparametric/__init__.py
+-rw-r--r--   0        0        0    12301 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/nonparametric/_kcca.py
+-rw-r--r--   0        0        0     6382 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/nonparametric/_ncca.py
+-rw-r--r--   0        0        0     5732 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/nonparametric/_scca_hsic.py
+-rw-r--r--   0        0        0     1917 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/preprocessing/__init__.py
+-rw-r--r--   0        0        0       80 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/probabilistic/__init__.py
+-rw-r--r--   0        0        0     6323 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/probabilistic/_probabilisticcca.py
+-rw-r--r--   0        0        0     4647 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/sequential.py
+-rw-r--r--   0        0        0      129 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/utils/__init__.py
+-rw-r--r--   0        0        0     1581 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/utils/check_values.py
+-rw-r--r--   0        0        0       52 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/visualisation/__init__.py
+-rw-r--r--   0        0        0    15026 2023-08-07 13:23:10.789838 cca_zoo-2.2.0/cca_zoo/visualisation/plotter.py
+-rw-r--r--   0        0        0     1177 2023-08-07 13:23:11.029840 cca_zoo-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5528 1970-01-01 00:00:00.000000 cca_zoo-2.2.0/PKG-INFO
```

### Comparing `cca_zoo-2.1.0/LICENSE` & `cca_zoo-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/README.md` & `cca_zoo-2.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,36 @@
+<div align="center">
+
+<img src="docs/source/cca-zoo-logo.jpg" alt="drawing" width="200"/>
+
+# CCA-Zoo
+
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
 [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
-![Build Status](https://github.com/jameschapman19/cca_zoo/actions/workflows/python-package.yml/badge.svg)
+![Build Status](https://github.com/jameschapman19/cca_zoo/actions/workflows/changes.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/cca-zoo/badge/?version=latest)](https://cca-zoo.readthedocs.io/en/latest/?badge=latest)
 [![version](https://img.shields.io/pypi/v/cca-zoo)](https://pypi.org/project/cca-zoo/)
 [![downloads](https://img.shields.io/pypi/dm/cca-zoo)](https://pypi.org/project/cca-zoo/)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03823/status.svg)](https://doi.org/10.21105/joss.03823)
 
-# CCA-Zoo
+
+</div>
 
 `cca-zoo` is a collection of linear, kernel, and deep methods for canonical correlation analysis of multiview data.
 Where possible it follows the `scikit-learn`/`mvlearn` APIs and models therefore have `fit`/`transform`/`fit_transform`
 methods as standard.
 
+## Table of Contents
+
+- [Installation](#installation)
+- [Documentation](#documentation)
+- [Citation](#citation)
+- [Contributions](#contributions)
+- [Sources](#sources)
+
 ## Installation
 
 You can install cca-zoo with pip or poetry. cca-zoo has an optional probabilistic feature that you can enable with the [probabilistic] suffix.
 
 To install cca-zoo with pip, run one of the following commands in your terminal:
 
 ```bash
```

### Comparing `cca_zoo-2.1.0/cca_zoo/_base/__init__.py` & `cca_zoo-2.2.0/cca_zoo/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 from abc import abstractmethod
-from typing import Union, Iterable
+from typing import Iterable, Union
 
 import numpy as np
 from sklearn.base import BaseEstimator, MultiOutputMixin, RegressorMixin
 from sklearn.utils import check_random_state
 from sklearn.utils.validation import FLOAT_DTYPES, check_is_fitted
 
 
@@ -149,17 +149,20 @@
             all_corrs.append(
                 np.diag(
                     np.corrcoef(x.T, y.T)[
                         : self.latent_dimensions, self.latent_dimensions :
                     ]
                 )
             )
-        all_corrs = np.array(all_corrs).reshape(
-            (self.n_views_, self.n_views_, self.latent_dimensions)
-        )
+        try:
+            all_corrs = np.array(all_corrs).reshape(
+                (self.n_views_, self.n_views_, self.latent_dimensions)
+            )
+        except:
+            print()
         return all_corrs
 
     def score(self, views: Iterable[np.ndarray], y=None, **kwargs):
         """
         Returns the average pairwise correlation between the views
 
         Parameters
```

### Comparing `cca_zoo-2.1.0/cca_zoo/data/deep.py` & `cca_zoo-2.2.0/cca_zoo/data/deep.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/data/simulated.py` & `cca_zoo-2.2.0/cca_zoo/data/simulated.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,19 @@
         # Generate a covariance matrix for a single view based on its structure
         if view_structure == "identity":
             # Use an identity matrix as the covariance matrix
             cov = np.eye(view_features)
         elif view_structure == "random":
             # Use a random positive definite matrix as the covariance matrix
             cov = make_spd_matrix(view_features)
+        # scale variance in each dimension to 1 while keeping the covariance matrix positive definite. Multiply rows by inverse of
+        # square root of diagonal matrix of eigenvalues and multiply columns by square root of diagonal matrix of eigenvalues
+        var = np.diag(cov)
+        cov = cov / np.sqrt(var)
+        cov = cov.T / np.sqrt(var)
         return cov
 
     def _generate_joint_covariance(self, covs):
         # Generate a joint covariance matrix for all views by stacking the view covariances and adding cross-covariances
         cov = block_diag(*covs)
         splits = np.concatenate(([0], np.cumsum(self.view_features)))
         for i, j in itertools.combinations(range(len(splits) - 1), 2):
```

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/__init__.py` & `cca_zoo-2.2.0/cca_zoo/deep/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from . import architectures, callbacks, objectives
 from ._discriminative import (
     DCCA,
     DCCA_EY,
     DCCA_GH,
-    DCCA_SVD,
     DCCA_NOI,
     DCCA_SDL,
+    DCCA_SVD,
+    DGCCA,
     DTCCA,
     BarlowTwins,
-    DGCCA,
 )
 from ._generative import DCCAE, DVCCA, SplitAE
 
 __all__ = [
     "DCCA",
     "DCCAE",
     "DCCA_NOI",
```

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_base.py` & `cca_zoo-2.2.0/cca_zoo/deep/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca.py` & `cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py` & `cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_ey.py` & `cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_ey.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_gh.py` & `cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_noi.py` & `cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_noi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_sdl.py` & `cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_sdl.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dcca_svd.py` & `cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dcca_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_discriminative/_dgcca.py` & `cca_zoo-2.2.0/cca_zoo/deep/_discriminative/_dtcca.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from ._dcca import DCCA
 from .. import objectives
+from ._dcca import DCCA
 
 
-class DGCCA(DCCA):
+class DTCCA(DCCA):
     """
-    A class used to fit a DGCCA model.
+    A class used to fit a DTCCA model.
 
-    Is just a thin wrapper round DCCA with the DGCCA objective
+    Is just a thin wrapper round DCCA with the DTCCA objective
 
     References
     ----------
-
+    Wong, Hok Shing, et al. "Deep Tensor CCA for Multi-view Learning." IEEE Transactions on Big Data (2021).
 
     """
 
     def __init__(
         self,
         latent_dimensions: int,
         encoders=None,
         r: float = 0,
         eps: float = 1e-5,
         **kwargs
     ):
-        # Call the parent class constructor with the DGCCA objective function
+        # Call the parent class constructor with the DTCCA objective function
         super().__init__(
             latent_dimensions=latent_dimensions,
-            objective=objectives.GCCA,
+            objective=objectives.TCCA,
             encoders=encoders,
             r=r,
             eps=eps,
             **kwargs
         )
```

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_generative/_base.py` & `cca_zoo-2.2.0/cca_zoo/deep/_generative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_generative/_dccae.py` & `cca_zoo-2.2.0/cca_zoo/deep/_generative/_dccae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_generative/_dvcca.py` & `cca_zoo-2.2.0/cca_zoo/deep/_generative/_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/_generative/_splitae.py` & `cca_zoo-2.2.0/cca_zoo/deep/_generative/_splitae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/architectures.py` & `cca_zoo-2.2.0/cca_zoo/deep/architectures.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/metrics.py` & `cca_zoo-2.2.0/cca_zoo/deep/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import torch
 from torchmetrics import Metric
 
 from cca_zoo.deep.objectives import _demean, inv_sqrtm
 
 
 class MCCA(Metric):
-    def __init__(self):
-        super().__init__(dist_sync_on_step=False, compute_on_step=False)
+    def __init__(
+        self,
+    ):
+        super().__init__()
         self.add_state("representations", default=[], persistent=False)
 
     def update(self, representations: Iterable[torch.Tensor] = None):
         for i, representation in enumerate(representations):
             if len(self.representations) < len(representations):
                 self.representations.append([representation])
             else:
```

### Comparing `cca_zoo-2.1.0/cca_zoo/deep/objectives.py` & `cca_zoo-2.2.0/cca_zoo/deep/objectives.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/__init__.py` & `cca_zoo-2.2.0/cca_zoo/linear/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from ._mcca import MCCA, CCA, rCCA
-from ._pls import PLS, MPLS
 from ._gcca import GCCA
+from ._gradient import CCAEY, CCAGH, CCASVD, PLSEY, PLSSVD, PLSStochasticPower
 from ._grcca import GRCCA
-from ._partialcca import PartialCCA
-from ._prcca import PRCCA
-from ._tcca import TCCA
-from ._pcacca import PCACCA
 from ._iterative import (
-    AltMaxVar,
-    SCCA_IPLS,
-    ElasticCCA,
     PLS_ALS,
+    SCCA_IPLS,
     SCCA_PMD,
+    # AltMaxVar,
+    ElasticCCA,
     SCCA_Parkhomenko,
     SCCA_Span,
 )
-from ._gradient import CCAEY, PLSEY, CCAGH, CCASVD, PLSSVD, PLSStochasticPower
+from ._mcca import CCA, MCCA, rCCA
+from ._partialcca import PartialCCA
+from ._pcacca import PCACCA
+from ._pls import MPLS, PLS
+from ._prcca import PRCCA
+from ._tcca import TCCA
 
 __all__ = [
     "MCCA",
     "CCA",
     "rCCA",
     "PLS",
     "MPLS",
     "GCCA",
     "GRCCA",
     "PartialCCA",
     "PRCCA",
     "TCCA",
     "PCACCA",
-    "AltMaxVar",
+    # "AltMaxVar",
     "SCCA_IPLS",
     "ElasticCCA",
     "PLS_ALS",
     "SCCA_PMD",
     "SCCA_Parkhomenko",
     "SCCA_Span",
     "CCAEY",
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_dummy.py` & `cca_zoo-2.2.0/cca_zoo/linear/_dummy.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_gcca.py` & `cca_zoo-2.2.0/cca_zoo/linear/_gcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_gradient/_ey.py` & `cca_zoo-2.2.0/cca_zoo/linear/_gradient/_ey.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Union
 
 import numpy as np
 import torch
 
-from cca_zoo.linear._iterative._base import BaseIterative
-from cca_zoo.linear._gradient._gradient import GradientLoop
+from cca_zoo.linear._gradient._base import BaseGradientModel, BaseLoop
 from cca_zoo.linear._pls import PLSMixin
 
 
-class CCAEY(BaseIterative):
+class CCAEY(BaseGradientModel):
     """
     A class used to fit Regularized CCA by Delta-EigenGame
 
     Parameters
     ----------
     latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
@@ -68,15 +67,15 @@
             patience=patience,
             track=track,
             verbose=verbose,
         )
         # ensure dataloader_kwargs['shuffle'] is True
         self.dataloader_kwargs["shuffle"] = True
 
-    def _get_module(self, weights=None, k=None):
+    def _get_pl_module(self, weights=None, k=None):
         return EYLoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="cca",
             tracking=self.track,
@@ -84,90 +83,30 @@
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
 class PLSEY(CCAEY, PLSMixin):
-    """
-    A class used to fit Regularized CCA by Delta-EigenGame
-
-    Parameters
-    ----------
-    latent_dimensions : int, optional
-        Number of latent dimensions to use, by default 1
-    copy_data : bool, optional
-        Whether to copy the data, by default True
-    random_state : int, optional
-        Random state to use, by default None
-    accept_sparse : bool, optional
-        Whether to accept sparse data, by default None
-    batch_size : int, optional
-        Batch size to use, by default 1
-    epochs : int, optional
-        Number of epochs to use, by default 1
-    learning_rate : float, optional
-        Learning rate to use, by default 0.01
-
-    References
-    ----------
-    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A GeneralizedDeflation EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
-    """
-
-    def __init__(
-        self,
-        latent_dimensions: int = 1,
-        copy_data=True,
-        random_state=None,
-        tol=1e-9,
-        accept_sparse=None,
-        batch_size=None,
-        epochs=1,
-        learning_rate=1,
-        initialization: Union[str, callable] = "random",
-        dataloader_kwargs=None,
-        convergence_checking=False,
-        patience=10,
-        track=False,
-        verbose=False,
-    ):
-        super().__init__(
-            latent_dimensions=latent_dimensions,
-            copy_data=copy_data,
-            accept_sparse=accept_sparse,
-            random_state=random_state,
-            tol=tol,
-            batch_size=batch_size,
-            epochs=epochs,
-            learning_rate=learning_rate,
-            initialization=initialization,
-            dataloader_kwargs=dataloader_kwargs,
-            convergence_checking=convergence_checking,
-            patience=patience,
-            track=track,
-            verbose=verbose,
-        )
-        self.previous_views = None
-
-    def _get_module(self, weights=None, k=None):
+    def _get_pl_module(self, weights=None, k=None):
         return EYLoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="pls",
             tracking=self.track,
             convergence_checking=self.convergence_checking,
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
-class EYLoop(GradientLoop):
+class EYLoop(BaseLoop):
     def __init__(
         self,
         weights=None,
         k=None,
         learning_rate=1e-3,
         optimizer_kwargs=None,
         objective="cca",
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_gradient/_gh.py` & `cca_zoo-2.2.0/cca_zoo/linear/_gradient/_gh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 
 from cca_zoo.linear._gradient._ey import CCAEY, EYLoop
 
 
 class CCAGH(CCAEY):
-    def _get_module(self, weights=None, k=None):
+    def _get_pl_module(self, weights=None, k=None):
         return GHALoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="cca",
             tracking=self.track,
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_gradient/_stochasticpls.py` & `cca_zoo-2.2.0/cca_zoo/linear/_gradient/_stochasticpls.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import torch
 
+from cca_zoo.linear._gradient._base import BaseLoop
 from cca_zoo.linear._gradient._ey import PLSEY
-from cca_zoo.linear._gradient._gradient import GradientLoop
 from cca_zoo.linear._pls import PLSMixin
 
 
 class PLSStochasticPower(PLSEY, PLSMixin):
-    def _get_module(self, weights=None, k=None):
+    def _get_pl_module(self, weights=None, k=None):
         return StochasticPowerLoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
-class StochasticPowerLoop(GradientLoop):
+class StochasticPowerLoop(BaseLoop):
     def __init__(
         self,
         weights=None,
         k=None,
         learning_rate=1e-3,
         optimizer_kwargs=None,
         tracking=False,
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_gradient/_svd.py` & `cca_zoo-2.2.0/cca_zoo/linear/_gradient/_svd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-from typing import Union
-
 import torch
 
-
-from cca_zoo.linear._gradient._ey import EYLoop, CCAEY
+from cca_zoo.linear._gradient._ey import CCAEY, EYLoop
 from cca_zoo.linear._pls import PLSMixin
 
 
 class CCASVD(CCAEY):
-    def _get_module(self, weights=None, k=None):
+    def _get_pl_module(self, weights=None, k=None):
         return SVDLoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="cca",
             tracking=self.track,
@@ -20,15 +17,15 @@
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
 class PLSSVD(CCASVD, PLSMixin):
-    def _get_module(self, weights=None, k=None):
+    def _get_pl_module(self, weights=None, k=None):
         return SVDLoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="pls",
             tracking=self.track,
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_grcca.py` & `cca_zoo-2.2.0/cca_zoo/linear/_grcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_altmaxvar.py` & `cca_zoo-2.2.0/cca_zoo/linear/_iterative/_altmaxvar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-from typing import Iterable, Union
-
-import numpy as np
-import torch
-
-from cca_zoo.linear._iterative._base import BaseIterative, BaseLoop
-from cca_zoo.utils import _process_parameter
-
-
-class AltMaxVar(BaseIterative):
-    def __init__(
-        self,
-        latent_dimensions=1,
-        copy_data=True,
-        random_state=None,
-        epochs=100,
-        tol=1e-3,
-        proximal="L1",
-        positive=False,
-        initialization="uniform",
-        tau: Union[Iterable[float], float] = None,
-        proximal_params: Iterable[dict] = None,
-        gamma=0.1,
-        learning_rate=1e-2,
-        T=100,
-        trainer_kwargs=None,
-        convergence_checking=None,
-        track=None,
-        verbose=False,
-    ):
-        super().__init__(
-            latent_dimensions=latent_dimensions,
-            copy_data=copy_data,
-            random_state=random_state,
-            tol=tol,
-            epochs=epochs,
-            convergence_checking=convergence_checking,
-            track=track,
-            verbose=verbose,
-            trainer_kwargs=trainer_kwargs,
-            initialization=initialization,
-        )
-        self.tau = tau
-        self.proximal = proximal
-        self.proximal_params = proximal_params
-        self.gamma = gamma
-        self.learning_rate = learning_rate
-        self.T = T
-        self.positive = positive
-        # set trainer kwargs accelerator to 'cpu'
-        self.trainer_kwargs["accelerator"] = "cpu"
-
-    def _get_module(self, weights=None, k=None):
-        return AltMaxVarLoop(
-            weights=weights,
-            k=k,
-            gamma=self.gamma,
-            T=self.T,
-            proximal_operators=self.proximal_operators,
-            learning_rate=self.learning_rate,
-            convergence_checking=self.convergence_checking,
-            track=self.track,
-        )
-
-    def _check_params(self):
-        self.proximal = _process_parameter(
-            "proximal", self.proximal, "L1", self.n_views_
-        )
-        self.positive = _process_parameter(
-            "positive", self.positive, False, self.n_views_
-        )
-        self.tau = _process_parameter("tau", self.tau, 0, self.n_views_)
-        self.sigma = self.tau
-        self.proximal_operators = [
-            self._get_proximal(view) for view in range(self.n_views_)
-        ]
-
-    def _get_proximal(self, view):
-        if callable(self.proximal[view]):
-            params = self.proximal_params[view] or {}
-        else:
-            params = {
-                "sigma": self.sigma[view],
-                "positive": self.positive[view],
-            }
-        return _proximal_operators(self.proximal[view], **params)
-
-    def _more_tags(self):
-        return {"multiview": True}
-
-
-class AltMaxVarLoop(BaseLoop):
-    def __init__(
-        self,
-        weights,
-        k=None,
-        gamma=0.1,
-        T=100,
-        proximal_operators=None,
-        learning_rate=1e-3,
-        convergence_checking=None,
-        track=None,
-    ):
-        super().__init__(
-            weights=weights,
-            k=k,
-            convergence_checking=convergence_checking,
-            tracking=track,
-        )
-        self.gamma = gamma
-        self.proximal_operators = proximal_operators
-        self.T = T
-        self.learning_rate = learning_rate
-
-    def forward(self, views: list) -> list:
-        # views detach and numpy
-        views = [view.detach().numpy() for view in views]
-        return [view @ weight for view, weight in zip(views, self.weights)]
-
-    def _get_target(self, scores):
-        if hasattr(self, "G"):
-            R = self.gamma * scores.mean(axis=0) + (1 - self.gamma) * self.G
-        else:
-            R = scores.mean(axis=0)
-        U, S, Vt = np.linalg.svd(R, full_matrices=False)
-        G = U @ Vt
-        return G / np.sqrt(np.diag(np.atleast_1d(np.cov(G, rowvar=False))))
-
-    def objective(self, views, scores, weights) -> int:
-        least_squares = (np.linalg.norm(scores - self.G, axis=(1, 2)) ** 2).sum()
-        regularization = np.array(
-            [self.proximal_operators[view](weights[view]) for view in range(len(views))]
-        ).sum()
-        return least_squares + regularization
-
-    def training_step(self, batch, batch_idx):
-        scores = np.stack(self(batch["views"]))
-        self.G = self._get_target(scores)
-        old_weights = self.weights.copy()
-        for i, view in enumerate(batch["views"]):
-            view = view.detach().numpy()
-            t = 0
-            prev_weights = None
-            converged = False
-            while t < self.T and not converged:
-                grad = view.T @ (view @ self.weights[i] - self.G) / view.shape[0]
-                # update the weights using the gradient descent and proximal operator
-                self.weights[i] -= self.learning_rate * grad
-                self.weights[i] = self.proximal_operators[i].prox(
-                    self.weights[i], self.learning_rate
-                )
-                # check if the weights have changed significantly from the previous iteration
-                if prev_weights is not None and np.allclose(
-                    self.weights[i], prev_weights
-                ):
-                    # if yes, set converged to True and break the loop
-                    converged = True
-                # update the previous weights for the next iteration
-                prev_weights = self.weights[i].copy()
-                t += 1
-
-        # if track or convergence_checking is enabled, compute the objective function
-        if self.tracking or self.convergence_checking:
-            objective = self.objective(batch["views"], scores, self.weights)
-            # check that the maximum change in weights is smaller than the tolerance times the maximum absolute value of the weights
-            weights_change = torch.tensor(
-                np.max(
-                    [
-                        np.max(np.abs(old_weights[i] - self.weights[i]))
-                        / np.max(np.abs(self.weights[i]))
-                        for i in range(len(self.weights))
-                    ]
-                )
-            )
-            return {"loss": torch.tensor(objective), "weights_change": weights_change}
-
-
-from pyproximal import (
-    L0,
-    L0Ball,
-    L1,
-    L1Ball,
-    L2,
-    L21,
-    L21_plus_L1,
-    Nuclear,
-    NuclearBall,
-    Log,
-    Log1,
-    Euclidean,
-    EuclideanBall,
-)
-
-PROXIMAL_OPERATORS = {
-    "L0": L0,
-    "L0Ball": L0Ball,
-    "L1": L1,
-    "L1Ball": L1Ball,
-    "L2": L2,
-    "L21": L21,
-    "L21_plus_L1": L21_plus_L1,
-    "Nuclear": Nuclear,
-    "NuclearBall": NuclearBall,
-    "Log": Log,
-    "Log1": Log1,
-    "Euclidean": Euclidean,
-    "EuclideanBall": EuclideanBall,
-}
-
-PROXIMAL_PARAMS = {
-    "Dummy": (),
-    "L0": frozenset(["sigma"]),
-    "L0Ball": frozenset(["radius"]),
-    "L1": frozenset(["sigma"]),
-    "L1Ball": frozenset(["n", "radius"]),
-    "L2": frozenset(["sigma"]),
-    "L21": frozenset(["ndim", "sigma"]),
-    "L21_plus_L1": frozenset(["sigma", "rho"]),
-    "TV": frozenset(["sigma", "isotropic", "dims"]),
-    "Nuclear": frozenset(["dim", "sigma"]),
-    "NuclearBall": frozenset(["dims", "radius"]),
-    "Log": frozenset(["sigma", "gamma"]),
-    "Log1": frozenset(["sigma", "delta"]),
-    "Euclidean": frozenset(["sigma"]),
-    "TVL1": frozenset(["sigma", "shape", "l1_ratio"]),
-}
-
-
-def _proximal_operators(proximal, filter_params=True, **params):
-    if proximal in PROXIMAL_OPERATORS:
-        if filter_params:
-            params = {k: params[k] for k in params if k in PROXIMAL_PARAMS[proximal]}
-        return PROXIMAL_OPERATORS[proximal](**params)
-    elif callable(proximal):
-        return proximal(**params)
+# from typing import Iterable, Union
+#
+# import numpy as np
+# import torch
+#
+# from cca_zoo.linear._iterative._base import BaseIterative, BaseLoop
+# from cca_zoo.utils import _process_parameter
+#
+# #
+# class AltMaxVar(BaseIterative):
+#     def __init__(
+#         self,
+#         latent_dimensions=1,
+#         copy_data=True,
+#         random_state=None,
+#         epochs=100,
+#         tol=1e-3,
+#         proximal="L1",
+#         positive=False,
+#         initialization="uniform",
+#         tau: Union[Iterable[float], float] = None,
+#         proximal_params: Iterable[dict] = None,
+#         gamma=0.1,
+#         learning_rate=1e-2,
+#         T=100,
+#         trainer_kwargs=None,
+#         convergence_checking=None,
+#         track=None,
+#         verbose=False,
+#     ):
+#         super().__init__(
+#             latent_dimensions=latent_dimensions,
+#             copy_data=copy_data,
+#             random_state=random_state,
+#             tol=tol,
+#             epochs=epochs,
+#             convergence_checking=convergence_checking,
+#             track=track,
+#             verbose=verbose,
+#             trainer_kwargs=trainer_kwargs,
+#             initialization=initialization,
+#         )
+#         self.tau = tau
+#         self.proximal = proximal
+#         self.proximal_params = proximal_params
+#         self.gamma = gamma
+#         self.learning_rate = learning_rate
+#         self.T = T
+#         self.positive = positive
+#         # set trainer kwargs accelerator to 'cpu'
+#         self.trainer_kwargs["accelerator"] = "cpu"
+#
+#     def _get_pl_module(self, weights=None, k=None):
+#         return AltMaxVarLoop(
+#             weights=weights,
+#             k=k,
+#             gamma=self.gamma,
+#             T=self.T,
+#             proximal_operators=self.proximal_operators,
+#             learning_rate=self.learning_rate,
+#             convergence_checking=self.convergence_checking,
+#             track=self.track,
+#         )
+#
+#     def _check_params(self):
+#         self.proximal = _process_parameter(
+#             "proximal", self.proximal, "L1", self.n_views_
+#         )
+#         self.positive = _process_parameter(
+#             "positive", self.positive, False, self.n_views_
+#         )
+#         self.tau = _process_parameter("tau", self.tau, 0, self.n_views_)
+#         self.sigma = self.tau
+#         self.proximal_operators = [
+#             self._get_proximal(view) for view in range(self.n_views_)
+#         ]
+#
+#     def _get_proximal(self, view):
+#         if callable(self.proximal[view]):
+#             params = self.proximal_params[view] or {}
+#         else:
+#             params = {
+#                 "sigma": self.sigma[view],
+#                 "positive": self.positive[view],
+#             }
+#         return _proximal_operators(self.proximal[view], **params)
+#
+#     def _more_tags(self):
+#         return {"multiview": True}
+#
+#
+# class AltMaxVarLoop(BaseLoop):
+#     def __init__(
+#         self,
+#         weights,
+#         k=None,
+#         gamma=0.1,
+#         T=100,
+#         proximal_operators=None,
+#         learning_rate=1e-3,
+#         convergence_checking=None,
+#         track=None,
+#     ):
+#         super().__init__(
+#             weights=weights,
+#             k=k,
+#             convergence_checking=convergence_checking,
+#             tracking=track,
+#         )
+#         self.gamma = gamma
+#         self.proximal_operators = proximal_operators
+#         self.T = T
+#         self.learning_rate = learning_rate
+#
+#     def forward(self, views: list) -> list:
+#         # views detach and numpy
+#         views = [view.detach().numpy() for view in views]
+#         return [view @ weight for view, weight in zip(views, self.weights)]
+#
+#     def _get_target(self, scores):
+#         if hasattr(self, "G"):
+#             R = self.gamma * scores.mean(axis=0) + (1 - self.gamma) * self.G
+#         else:
+#             R = scores.mean(axis=0)
+#         U, S, Vt = np.linalg.svd(R, full_matrices=False)
+#         G = U @ Vt
+#         return G / np.sqrt(np.diag(np.atleast_1d(np.cov(G, rowvar=False))))
+#
+#     def objective(self, views, scores, weights) -> int:
+#         least_squares = (np.linalg.norm(scores - self.G, axis=(1, 2)) ** 2).sum()
+#         regularization = np.array(
+#             [self.proximal_operators[view](weights[view]) for view in range(len(views))]
+#         ).sum()
+#         return least_squares + regularization
+#
+#     def training_step(self, batch, batch_idx):
+#         scores = np.stack(self(batch["views"]))
+#         self.G = self._get_target(scores)
+#         old_weights = self.weights.copy()
+#         for i, view in enumerate(batch["views"]):
+#             view = view.detach().numpy()
+#             t = 0
+#             prev_weights = None
+#             converged = False
+#             while t < self.T and not converged:
+#                 grad = view.T @ (view @ self.weights[i] - self.G) / view.shape[0]
+#                 # update the weights using the gradient descent and proximal operator
+#                 self.weights[i] -= self.learning_rate * grad
+#                 self.weights[i] = self.proximal_operators[i].prox(
+#                     self.weights[i], self.learning_rate
+#                 )
+#                 # check if the weights have changed significantly from the previous iteration
+#                 if prev_weights is not None and np.allclose(
+#                     self.weights[i], prev_weights
+#                 ):
+#                     # if yes, set converged to True and break the loop
+#                     converged = True
+#                 # update the previous weights for the next iteration
+#                 prev_weights = self.weights[i].copy()
+#                 t += 1
+#
+#         # if track or convergence_checking is enabled, compute the objective function
+#         if self.tracking or self.convergence_checking:
+#             objective = self.objective(batch["views"], scores, self.weights)
+#             # check that the maximum change in weights is smaller than the tolerance times the maximum absolute value of the weights
+#             weights_change = torch.tensor(
+#                 np.max(
+#                     [
+#                         np.max(np.abs(old_weights[i] - self.weights[i]))
+#                         / np.max(np.abs(self.weights[i]))
+#                         for i in range(len(self.weights))
+#                     ]
+#                 )
+#             )
+#             return {"loss": torch.tensor(objective), "weights_change": weights_change}
+#
+#
+# from pyproximal import (
+#     L0,
+#     L1,
+#     L2,
+#     L21,
+#     Euclidean,
+#     EuclideanBall,
+#     L0Ball,
+#     L1Ball,
+#     L21_plus_L1,
+#     Log,
+#     Log1,
+#     Nuclear,
+#     NuclearBall,
+# )
+#
+# PROXIMAL_OPERATORS = {
+#     "L0": L0,
+#     "L0Ball": L0Ball,
+#     "L1": L1,
+#     "L1Ball": L1Ball,
+#     "L2": L2,
+#     "L21": L21,
+#     "L21_plus_L1": L21_plus_L1,
+#     "Nuclear": Nuclear,
+#     "NuclearBall": NuclearBall,
+#     "Log": Log,
+#     "Log1": Log1,
+#     "Euclidean": Euclidean,
+#     "EuclideanBall": EuclideanBall,
+# }
+#
+# PROXIMAL_PARAMS = {
+#     "Dummy": (),
+#     "L0": frozenset(["sigma"]),
+#     "L0Ball": frozenset(["radius"]),
+#     "L1": frozenset(["sigma"]),
+#     "L1Ball": frozenset(["n", "radius"]),
+#     "L2": frozenset(["sigma"]),
+#     "L21": frozenset(["ndim", "sigma"]),
+#     "L21_plus_L1": frozenset(["sigma", "rho"]),
+#     "TV": frozenset(["sigma", "isotropic", "dims"]),
+#     "Nuclear": frozenset(["dim", "sigma"]),
+#     "NuclearBall": frozenset(["dims", "radius"]),
+#     "Log": frozenset(["sigma", "gamma"]),
+#     "Log1": frozenset(["sigma", "delta"]),
+#     "Euclidean": frozenset(["sigma"]),
+#     "TVL1": frozenset(["sigma", "shape", "l1_ratio"]),
+# }
+#
+#
+# def _proximal_operators(proximal, filter_params=True, **params):
+#     if proximal in PROXIMAL_OPERATORS:
+#         if filter_params:
+#             params = {k: params[k] for k in params if k in PROXIMAL_PARAMS[proximal]}
+#         return PROXIMAL_OPERATORS[proximal](**params)
+#     elif callable(proximal):
+#         return proximal(**params)
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_base.py` & `cca_zoo-2.2.0/cca_zoo/linear/_gradient/_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,159 @@
+# filter warnings from pytorch_lightning
+import warnings
 from abc import abstractmethod
-from typing import Iterable, List, Optional, Union, Any
+from typing import Any, Iterable, List, Optional, Union
 
 import numpy as np
 import pytorch_lightning as pl
+import torch
 from lightning_fabric.utilities.warnings import PossibleUserWarning
 from pytorch_lightning.callbacks import Callback, EarlyStopping
 from torch.utils import data
 from torch.utils.data import DataLoader
 
-from cca_zoo.data.deep import NumpyDataset
-from cca_zoo.linear._pls import MPLS
-from cca_zoo.linear._mcca import MCCA
-
 from cca_zoo._base import BaseModel
+from cca_zoo.data.deep import NumpyDataset
 from cca_zoo.linear._dummy import DummyCCA, DummyPLS
-import torch
-
-# filter warnings from pytorch_lightning
-import warnings
-
-warnings.filterwarnings("ignore", category=UserWarning)
-warnings.filterwarnings("ignore", category=PossibleUserWarning)
-
-
-def supress_device_warnings():
-    import logging
+from cca_zoo.linear._mcca import MCCA
+from cca_zoo.linear._pls import MPLS
 
-    rank_zero_logger = logging.getLogger("pytorch_lightning.utilities.rank_zero")
-    rank_zero_logger.disabled = True
+# warnings.filterwarnings("ignore", category=UserWarning)
+# warnings.filterwarnings("ignore", category=PossibleUserWarning)
+#
+#
+# def supress_device_warnings():
+#     import logging
+#
+#     rank_zero_logger = logging.getLogger("pytorch_lightning.utilities.rank_zero")
+#     rank_zero_logger.disabled = True
+#
+#
+# supress_device_warnings()
 
 
 # Default Trainer kwargs
 DEFAULT_TRAINER_KWARGS = dict(
     enable_checkpointing=False,
-    logger=False,
+    logger=True,
     enable_model_summary=False,
     enable_progress_bar=True,
 )
 
 DEFAULT_LOADER_KWARGS = dict(
-    num_workers=0, pin_memory=True, drop_last=False, shuffle=False
+    num_workers=0, pin_memory=False, drop_last=False, shuffle=False
 )
 
 
-class BaseIterative(BaseModel):
+class BaseLoop(pl.LightningModule):
+    """A base class for CCA loops.
+
+    Attributes:
+        weights (torch.nn.ParameterList): The CCA weights as torch parameters.
+        tracking (bool): Whether to track the objective value during training.
+        convergence_checking (bool): Whether to check the convergence condition during training.
+        optimizer_kwargs (dict): The keyword arguments for the optimizer constructor.
+        learning_rate (float): The learning rate for the optimizer.
+    """
+
+    def __init__(
+        self,
+        weights: Optional[List[np.ndarray]] = None,
+        k: Optional[int] = None,
+        tracking: bool = False,
+        convergence_checking: bool = False,
+        optimizer_kwargs: Optional[dict] = None,
+        learning_rate: float = 1e-3,
+    ) -> None:
+        """Initialize the BaseLoop object.
+
+        Args:
+            weights (Optional[List[np.ndarray]], optional): The initial weights for the CCA loop, by default None
+            k (Optional[int], optional): The current component, by default None
+            tracking (bool, optional): Whether to track the objective value during training, by default False
+            convergence_checking (bool, optional): Whether to check the convergence condition during training, by default False
+            optimizer_kwargs (Optional[dict], optional): The keyword arguments for the optimizer constructor, by default None
+            learning_rate (float, optional): The learning rate for the optimizer, by default 1e-3
+        """
+        super().__init__()
+        if k is not None:
+            self.weights = [weight[:, k] for weight in weights]
+        else:
+            self.weights = weights
+        self.tracking = tracking
+        self.convergence_checking = convergence_checking
+        # Set the weights attribute as torch parameters with gradients
+        self.weights = [
+            torch.nn.Parameter(torch.from_numpy(weight), requires_grad=True)
+            for weight in self.weights
+        ]
+        self.weights = torch.nn.ParameterList(self.weights)
+        # Set the optimizer keyword arguments attribute with default values if none provided
+        self.optimizer_kwargs = optimizer_kwargs or {}
+        self.learning_rate = learning_rate
+
+    def forward(self, views: List[torch.Tensor]) -> List[torch.Tensor]:
+        """Perform a forward pass on the input views.
+
+        Args:
+            views (List[torch.Tensor]): The input views as torch tensors.
+
+        Returns:
+            List[torch.Tensor]: The output views as torch tensors.
+        """
+        return [view @ weight for view, weight in zip(views, self.weights)]
+
+    def configure_optimizers(self) -> torch.optim.Optimizer:
+        """Configure the optimizer for the loop.
+
+        Returns:
+            torch.optim.Optimizer: The optimizer object.
+        """
+        # construct optimizer using optimizer_kwargs
+        optimizer_name = self.optimizer_kwargs.get("optimizer", "Adam")
+        kwargs = self.optimizer_kwargs.copy()
+        kwargs.pop("optimizer", None)
+        optimizer = getattr(torch.optim, optimizer_name)(
+            self.weights, lr=self.learning_rate, **kwargs
+        )
+        return optimizer
+
+    def on_fit_end(self) -> None:
+        """Perform some actions after the fit ends.
+
+        For example, convert the weights from torch parameters to numpy arrays.
+        """
+        # if self.weights are torch parameters, convert them to numpy arrays
+        if isinstance(self.weights, torch.nn.ParameterList):
+            # weights to numpy arrays from torch parameters
+            weights = [weight.detach().cpu().numpy() for weight in self.weights]
+            del self.weights
+            self.weights = weights
+
+    def objective(self, *args, **kwargs) -> float:
+        """Compute the objective value for the loop.
+
+        This method should be implemented by subclasses.
+
+        Returns:
+            float: The objective value.
+
+        Raises:
+            NotImplementedError: If the method is not implemented by subclasses.
+        """
+        raise NotImplementedError
+
+
+class BaseGradientModel(BaseModel):
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         tol=1e-3,
-        deflation="cca",
         accept_sparse=None,
         batch_size=None,
         dataloader_kwargs=None,
         epochs=1,
         val_split=None,
         learning_rate=1,
         initialization: Union[str, callable] = "random",
@@ -76,19 +175,14 @@
         self.epochs = epochs
         # validate the split
         if val_split is not None:
             if val_split <= 0 or val_split >= 1:
                 raise ValueError("Validation split must be between 0 and 1")
         self.val_split = val_split
         self.learning_rate = learning_rate
-        # validate the deflation method
-        if deflation not in ["cca", "pls"]:
-            raise ValueError("Deflation method must be one of ['cca','pls']")
-        else:
-            self.deflation = deflation
         # validate the initialization method
         if initialization not in ["random", "uniform", "unregularized", "pls"]:
             raise ValueError(
                 "Initialization method must be one of ['random', 'uniform', 'unregularized', 'pls']"
             )
         else:
             self.initialization = initialization
@@ -110,41 +204,41 @@
             self.callbacks.append(
                 TrackingCallback(monitor=self.track, verbose=self.verbose)
             )
         self.dataloader_kwargs = dataloader_kwargs or DEFAULT_LOADER_KWARGS
         self.trainer_kwargs = trainer_kwargs or DEFAULT_TRAINER_KWARGS
 
     @abstractmethod
-    def _get_module(self, weights=None, k=None):
-        """Get the CCA module for training.
+    def _get_pl_module(self, weights=None, k=None) -> BaseLoop:
+        """Get model specific loop module for training.
 
         Parameters
         ----------
         weights : list of np.ndarray, optional
             The initial weights for the CCA module, by default None
         k : int, optional
             The current component, by default None
 
         Returns
         -------
         pl.LightningModule
             The CCA module object
         """
-        pass
+        raise NotImplementedError
 
     def fit(self, views: Iterable[np.ndarray], y=None, **kwargs):
         self._validate_data(views)
         self._check_params()
         self._initialize(views)
         self.weights = self._fit(views)
         return self
 
     def _fit(self, views: Iterable[np.ndarray]):
         train_dataloader, val_dataloader = self.get_dataloader(views)
-        loop = self._get_module(weights=self.weights)
+        loop = self._get_pl_module(weights=self.weights)
         # make a trainer
         trainer = pl.Trainer(
             max_epochs=self.epochs,
             callbacks=self.callbacks,
             **self.trainer_kwargs,
         )
         trainer.fit(loop, train_dataloader, val_dataloader)
@@ -209,41 +303,14 @@
         self.weights = [weights.astype(np.float32) for weights in self.weights]
 
     def _more_tags(self):
         # Indicate that this class is for multiview data
         return {"iterative": True}
 
 
-class BaseLoop(pl.LightningModule):
-    def __init__(
-        self,
-        weights=None,
-        k=None,
-        tracking=False,
-        convergence_checking=False,
-    ):
-        super().__init__()
-        if k is not None:
-            self.weights = [weight[:, k] for weight in weights]
-        else:
-            self.weights = weights
-        self.automatic_optimization = False
-        self.tracking = tracking
-        self.convergence_checking = convergence_checking
-
-    def configure_optimizers(self):
-        pass
-
-    def objective(self, *args, **kwargs) -> float:
-        raise NotImplementedError
-
-    def forward(self, views: list) -> list:
-        return [view @ weight for view, weight in zip(views, self.weights)]
-
-
 def _default_initializer(initialization, random_state, latent_dims, pls):
     if pls:
         if initialization == "random":
             initializer = DummyPLS(
                 latent_dims, random_state=random_state, uniform=False
             )
         elif initialization == "uniform":
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_deflation.py` & `cca_zoo-2.2.0/cca_zoo/linear/_iterative/_deflation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,88 @@
 from typing import Iterable
 
 import numpy as np
 import pytorch_lightning as pl
+from sklearn import clone
 from tqdm import tqdm
 
 
+# Import tqdm and deflate_views
+from tqdm import tqdm
+
+
+# Define DeflationMixin class
 class DeflationMixin:
-    def _fit(self, views: Iterable[np.ndarray]):
-        # if views is a tuple then convert to a list
+    # Define fit method
+    def fit(self, views: Iterable[np.ndarray], y=None, **kwargs):
+        self._validate_data(views)
+        # Convert views to list if tuple
         if isinstance(views, tuple):
             views = list(views)
-        # tqdm for each latent dimension
+        # Initialize weights list
+        self.weights = [
+            np.empty((view.shape[1], self.latent_dimensions)) for view in views
+        ]
+        # Loop over latent dimensions
         for k in tqdm(
-            range(self.latent_dimensions), desc="Latent Dimension", leave=False
+            range(self.latent_dimensions),
+            desc="Latent Dimension",
+            position=0,
+            leave=True,
         ):
-            train_dataloader, val_dataloader = self.get_dataloader(views)
-            loop = self._get_module(weights=self.weights, k=k)
-            # make a trainer
-            trainer = pl.Trainer(
-                max_epochs=self.epochs, callbacks=self.callbacks, **self.trainer_kwargs
-            )
-            trainer.fit(loop, train_dataloader, val_dataloader)
-            # return the weights from the module. They will need to be changed from torch tensors to numpy arrays
-            weights = loop.weights
-            for i, (view, weight) in enumerate(zip(views, weights)):
-                self.weights[i][:, k] = weight
-                views[i] = self._deflate(view, weight)
-            # if loop has tracked the objective, return the objective
-            if hasattr(loop, "epoch_objective"):
-                self.objective = loop.epoch_objective
-        return self.weights
-
-    def _deflate(self, residual: np.ndarray, weights: np.ndarray) -> np.ndarray:
-        """Deflate view residual by CCA deflation.
-
-        Parameters
-        ----------
-        residual : np.ndarray
-            The current residual data matrix for a view
-        weights : np.ndarray
-            The current CCA weights for a view
-
-        Returns
-        -------
-        np.ndarray
-            The deflated residual data matrix for a view
-
-        Raises
-        ------
-        ValueError
-            If deflation method is not one of ["cca", "pls"]
-        """
-        # Compute the score vector for a view
-        score = residual @ weights
-
-        # Deflate the residual by different methods based on the deflation attribute
-        if self.deflation == "cca":
-            return residual - np.outer(score, score) @ residual / np.dot(score, score)
-        elif self.deflation == "pls":
-            return residual - np.outer(score, weights)
-        else:
-            raise ValueError(
-                f"Invalid deflation method: {self.deflation}. "
-                f"Must be one of ['cca', 'pls']."
-            )
+            # clone self but with only one latent dimension and _fit
+            component_weights = clone(self).set_params(latent_dimensions=1)._fit(views)
+            # Append component_weights to weights list
+            for i, weight in enumerate(component_weights):
+                self.weights[i][:, k] = weight.squeeze()
+            # Deflate views using component_weights
+            views = deflate_views(views, component_weights)
+        # Return self
+        return self
+
+
+def deflate_views(residuals: Iterable[np.ndarray], weights: Iterable[np.ndarray]):
+    """Deflate the residuals by CCA deflation.
+
+    Parameters
+    ----------
+    residuals : Iterable[np.ndarray]
+        The current residual data matrices for each view
+    weights : Iterable[np.ndarray]
+        The current CCA weights for each view
+
+    Returns
+    -------
+    Iterable[np.ndarray]
+        The deflated residual data matrices for each view
+    """
+    # Deflate the residuals for each view
+    return [
+        deflate_view(residual, weight) for residual, weight in zip(residuals, weights)
+    ]
+
+
+def deflate_view(residual: np.ndarray, weights: np.ndarray) -> np.ndarray:
+    """Deflate view residual by CCA deflation.
+
+    Parameters
+    ----------
+    residual : np.ndarray
+        The current residual data matrix for a view
+    weights : np.ndarray
+        The current CCA weights for a view
+
+    Returns
+    -------
+    np.ndarray
+        The deflated residual data matrix for a view
+
+    Raises
+    ------
+    ValueError
+        If deflation method is not one of ["cca", "pls"]
+    """
+    # Compute the score vector for a view
+    score = residual @ weights
+
+    # Deflate the residual by different methods based on the deflation attribute
+    return residual - residual @ np.outer(weights, weights) / (weights.T @ weights)
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_incrementalpls.py` & `cca_zoo-2.2.0/cca_zoo/linear/_iterative/_incrementalpls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from typing import Union
-
-import numpy as np
-
-from cca_zoo.linear._iterative._base import BaseIterative
-
-
-class IncrementalPLS(BaseIterative):
-    r"""
-    A class used to fit Incremental PLS
-
-    Parameters
-    ----------
-    latent_dimensions : int, optional
-        Number of latent dimensions to use, by default 1
-    copy_data : bool, optional
-        Whether to copy the data, by default True
-    random_state : int, optional
-        Random state to use, by default None
-    accept_sparse : bool, optional
-        Whether to accept sparse data, by default None
-    batch_size : int, optional
-        Batch size to use, by default 1
-    epochs : int, optional
-        Number of epochs to use, by default 1
-    simple : bool, optional
-        Whether to use the simple update, by default False
-
-    References
-    ----------
-    Arora, Raman, et al. "Stochastic optimization for PCA and PLS." 2012 50th Annual Allerton Conference on Communication, Control, and Computing (Allerton). IEEE, 2012.
-    """
-
-    def __init__(
-        self,
-        latent_dimensions: int = 1,
-        copy_data=True,
-        random_state=None,
-        accept_sparse=None,
-        batch_size=1,
-        epochs=1,
-        simple=False,
-        initialization: Union[str, callable] = "random",
-    ):
-        super().__init__(
-            latent_dimensions=latent_dimensions,
-            copy_data=copy_data,
-            accept_sparse=accept_sparse,
-            random_state=random_state,
-            batch_size=batch_size,
-            epochs=epochs,
-            initialization=initialization,
-        )
-        self.simple = simple
-
-    def _update(self, views):
-        if not hasattr(self, "S"):
-            self.S = np.zeros(self.latent_dimensions)
-            self.count = 0
-        if self.simple:
-            self.simple_update(views)
-        else:
-            self.incremental_update(views)
-        return False
-
-    def incremental_update(self, views):
-        hats = np.stack([view @ weight for view, weight in zip(views, self.weights)])
-        orths = [
-            view - hat @ weight.T
-            for view, weight, hat in zip(views, self.weights, hats)
-        ]
-        self.incrsvd(hats, orths)
-
-    def simple_update(self, views):
-        if not hasattr(self, "M"):
-            self.M = np.zeros((views[0].shape[1], views[1].shape[1]))
-        self.M = (
-            views[0].T @ views[1]
-            + self.weights[0] @ np.diag(self.S) @ self.weights[1].T
-        )
-        U, S, Vt = np.linalg.svd(self.M)
-        self.weights[0] = U[:, : self.latent_dimensions]
-        self.weights[1] = Vt.T[:, : self.latent_dimensions]
-        self.S = S[: self.latent_dimensions]
-
-    def incrsvd(self, hats, orths):
-        Q = np.vstack(
-            (
-                np.hstack(
-                    (
-                        np.diag(self.S) + hats[0].T @ hats[1],
-                        np.linalg.norm(orths[1], axis=1).T * hats[0].T,
-                    )
-                ),
-                np.hstack(
-                    (
-                        (np.linalg.norm(orths[0], axis=1).T * hats[1].T).T,
-                        np.atleast_2d(
-                            np.linalg.norm(orths[0], axis=1, keepdims=True)
-                            @ np.linalg.norm(orths[1], axis=1, keepdims=True).T
-                        ),
-                    )
-                ),
-            )
-        )
-        U, S, Vt = np.linalg.svd(Q)
-        self.weights[0] = (
-            np.hstack((self.weights[0], orths[0].T / np.linalg.norm(orths[0])))
-            @ U[:, : self.latent_dimensions]
-        )
-        self.weights[1] = (
-            np.hstack((self.weights[1], orths[1].T / np.linalg.norm(orths[1])))
-            @ Vt.T[:, : self.latent_dimensions]
-        )
-        self.S = S[: self.latent_dimensions]
+# from typing import Union
+#
+# import numpy as np
+#
+# from cca_zoo.linear._iterative._base import BaseIterative
+#
+#
+# class IncrementalPLS(BaseIterative):
+#     r"""
+#     A class used to fit Incremental PLS
+#
+#     Parameters
+#     ----------
+#     latent_dimensions : int, optional
+#         Number of latent dimensions to use, by default 1
+#     copy_data : bool, optional
+#         Whether to copy the data, by default True
+#     random_state : int, optional
+#         Random state to use, by default None
+#     accept_sparse : bool, optional
+#         Whether to accept sparse data, by default None
+#     batch_size : int, optional
+#         Batch size to use, by default 1
+#     epochs : int, optional
+#         Number of epochs to use, by default 1
+#     simple : bool, optional
+#         Whether to use the simple update, by default False
+#
+#     References
+#     ----------
+#     Arora, Raman, et al. "Stochastic optimization for PCA and PLS." 2012 50th Annual Allerton Conference on Communication, Control, and Computing (Allerton). IEEE, 2012.
+#     """
+#
+#     def __init__(
+#         self,
+#         latent_dimensions: int = 1,
+#         copy_data=True,
+#         random_state=None,
+#         accept_sparse=None,
+#         batch_size=1,
+#         epochs=1,
+#         simple=False,
+#         initialization: Union[str, callable] = "random",
+#     ):
+#         super().__init__(
+#             latent_dimensions=latent_dimensions,
+#             copy_data=copy_data,
+#             accept_sparse=accept_sparse,
+#             random_state=random_state,
+#             batch_size=batch_size,
+#             epochs=epochs,
+#             initialization=initialization,
+#         )
+#         self.simple = simple
+#
+#     def _update(self, views):
+#         if not hasattr(self, "S"):
+#             self.S = np.zeros(self.latent_dimensions)
+#             self.count = 0
+#         if self.simple:
+#             self.simple_update(views)
+#         else:
+#             self.incremental_update(views)
+#         return False
+#
+#     def incremental_update(self, views):
+#         hats = np.stack([view @ weight for view, weight in zip(views, self.weights)])
+#         orths = [
+#             view - hat @ weight.T
+#             for view, weight, hat in zip(views, self.weights, hats)
+#         ]
+#         self.incrsvd(hats, orths)
+#
+#     def simple_update(self, views):
+#         if not hasattr(self, "M"):
+#             self.M = np.zeros((views[0].shape[1], views[1].shape[1]))
+#         self.M = (
+#             views[0].T @ views[1]
+#             + self.weights[0] @ np.diag(self.S) @ self.weights[1].T
+#         )
+#         U, S, Vt = np.linalg.svd(self.M)
+#         self.weights[0] = U[:, : self.latent_dimensions]
+#         self.weights[1] = Vt.T[:, : self.latent_dimensions]
+#         self.S = S[: self.latent_dimensions]
+#
+#     def incrsvd(self, hats, orths):
+#         Q = np.vstack(
+#             (
+#                 np.hstack(
+#                     (
+#                         np.diag(self.S) + hats[0].T @ hats[1],
+#                         np.linalg.norm(orths[1], axis=1).T * hats[0].T,
+#                     )
+#                 ),
+#                 np.hstack(
+#                     (
+#                         (np.linalg.norm(orths[0], axis=1).T * hats[1].T).T,
+#                         np.atleast_2d(
+#                             np.linalg.norm(orths[0], axis=1, keepdims=True)
+#                             @ np.linalg.norm(orths[1], axis=1, keepdims=True).T
+#                         ),
+#                     )
+#                 ),
+#             )
+#         )
+#         U, S, Vt = np.linalg.svd(Q)
+#         self.weights[0] = (
+#             np.hstack((self.weights[0], orths[0].T / np.linalg.norm(orths[0])))
+#             @ U[:, : self.latent_dimensions]
+#         )
+#         self.weights[1] = (
+#             np.hstack((self.weights[1], orths[1].T / np.linalg.norm(orths[1])))
+#             @ Vt.T[:, : self.latent_dimensions]
+#         )
+#         self.S = S[: self.latent_dimensions]
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_admm.py` & `cca_zoo-2.2.0/cca_zoo/linear/_iterative/_scca_admm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,190 +1,189 @@
-from typing import Iterable, Union
-
-import numpy as np
-
-from cca_zoo.utils import _process_parameter
-from ._base import BaseIterative, BaseLoop
-from ._deflation import DeflationMixin
-
-
-class SCCA_ADMM(BaseIterative, DeflationMixin):
-    r"""
-    Fits a sparse CCA model by alternating ADMM for two or more views.
-
-    .. math::
-
-        w_{opt}=\underset{w}{\mathrm{argmax}}\{\sum_i\sum_{j\neq i} \|X_iw_i-X_jw_j\|^2 + \|w_i\|_1\}\\
-
-        \text{subject to:}
-
-        w_i^TX_i^TX_iw_i=1
-
-    Parameters
-    ----------
-    latent_dimensions : int, default=1
-        Number of latent dimensions to use in the model.
-    copy_data : bool, default=True
-        Whether to copy the data or overwrite it.
-    random_state : int, default=None
-        Random seed for initialisation.
-    deflation : str, default="cca"
-        Deflation method to use. Options are "cca" and "pls".
-    tau : float or list of floats, default=None
-        Regularisation parameter. If a single float is given, the same value is used for all views.
-        If a list of floats is given, the values are used for each view.
-    mu : float or list of floats, default=None
-        Regularisation parameter. If a single float is given, the same value is used for all views.
-        If a list of floats is given, the values are used for each view.
-    lam : float or list of floats, default=None
-        Regularisation parameter. If a single float is given, the same value is used for all views.
-        If a list of floats is given, the values are used for each view.
-    eta : float or list of floats, default=None
-        Regularisation parameter. If a single float is given, the same value is used for all views.
-        If a list of floats is given, the values are used for each view.
-    tol : float, default=1e-9
-        Tolerance for convergence.
-
-    References
-    ----------
-    Suo, Xiaotong, et al. "Sparse canonical correlation analysis." arXiv preprint arXiv:1705.10865 (2017).
-
-    Examples
-    --------
-    >>> from cca_zoo.linear import SCCA_ADMM
-    >>> import numpy as np
-    >>> rng=np.random.RandomState(0)
-    >>> X1 = rng.random((10,5))
-    >>> X2 = rng.random((10,5))
-    >>> model = SCCA_ADMM(random_state=0,tau=[1e-1,1e-1])
-    >>> model.fit((X1,X2)).score((X1,X2))
-    array([0.84348183])
-    """
-
-    def __init__(
-        self,
-        latent_dimensions: int = 1,
-        copy_data=True,
-        random_state=None,
-        deflation="cca",
-        tau: Union[Iterable[float], float] = None,
-        mu: Union[Iterable[float], float] = None,
-        lam: Union[Iterable[float], float] = None,
-        eta: Union[Iterable[float], float] = None,
-        initialization: Union[str, callable] = "pls",
-        tol: float = 1e-3,
-    ):
-        self.tau = tau
-        self.mu = mu
-        self.lam = lam
-        self.eta = eta
-        super().__init__(
-            latent_dimensions=latent_dimensions,
-            copy_data=copy_data,
-            initialization=initialization,
-            tol=tol,
-            random_state=random_state,
-            deflation=deflation,
-        )
-
-    def _check_params(self):
-        self.tau = _process_parameter("tau", self.tau, 0, self.n_views_)
-        self.lam = _process_parameter("lam", self.lam, 1, self.n_views_)
-        self.eta = _process_parameter("eta", self.eta, 0, self.n_views_)
-
-    def _get_module(self, weights=None, k=None):
-        return SCCA_ADMM_PL(
-            weights=weights,
-            k=k,
-            tau=self.tau,
-            lam=self.lam,
-            eta=self.eta,
-            n_samples_=self.n_samples_,
-            n_views_=self.n_views_,
-        )
-
-
-class SCCA_ADMM_PL(BaseLoop):
-    def __init__(
-        self,
-        weights,
-        k=None,
-        n_samples_=None,
-        n_views_=None,
-        tau=None,
-        eta=None,
-        lam=None,
-        mu=None,
-    ):
-        super().__init__(weights=weights, k=k)
-        self.eta = [np.ones(n_samples_) * eta for eta in eta]
-        self.z = [np.ones(n_samples_)] * n_views_
-        self.mu = mu
-
-    def training_step(self, batch, batch_idx):
-        views = batch["views"]
-        scores = np.stack(self(views))
-        for view_index, view in enumerate(views):
-            targets = np.ma.array(scores, mask=False)
-            targets.mask[view_index] = True
-            gradient = views[view_index].T @ targets.sum(axis=0).filled()
-            mu = self.mu[view_index]
-            lam = self.lam[view_index]
-            N = views[view_index].shape[0]
-            unnorm_z = []
-            norm_eta = []
-            norm_weights = []
-            norm_proj = []
-            for _ in range(self.max_iter):
-                # We multiply 'tau' by N in order to make regularisation match across the different sparse cca methods
-                self.weights[view_index] = self._prox_mu_f(
-                    self.weights[view_index]
-                    - mu
-                    / lam
-                    * views[view_index].T
-                    @ (
-                        views[view_index] @ self.weights[view_index]
-                        - self.z[view_index]
-                        + self.eta[view_index]
-                    ),
-                    mu,
-                    gradient,
-                    N * self.tau[view_index],
-                )
-                unnorm_z.append(
-                    np.linalg.norm(
-                        views[view_index] @ self.weights[view_index]
-                        + self.eta[view_index]
-                    )
-                )
-                self.z[view_index] = self._prox_lam_g(
-                    views[view_index] @ self.weights[view_index] + self.eta[view_index]
-                )
-                self.eta[view_index] = (
-                    self.eta[view_index]
-                    + views[view_index] @ self.weights[view_index]
-                    - self.z[view_index]
-                )
-                norm_eta.append(np.linalg.norm(self.eta[view_index]))
-                norm_proj.append(
-                    np.linalg.norm(views[view_index] @ self.weights[view_index])
-                )
-                norm_weights.append(np.linalg.norm(self.weights[view_index], 1))
-
-    def _prox_mu_f(self, x, mu, c, tau):
-        u_update = x.copy()
-        mask_1 = x + (mu * c) > mu * tau
-        # if mask_1.sum()>0:
-        u_update[mask_1] = x[mask_1] + mu * (c[mask_1] - tau)
-        mask_2 = x + (mu * c) < -mu * tau
-        # if mask_2.sum() > 0:
-        u_update[mask_2] = x[mask_2] + mu * (c[mask_2] + tau)
-        mask_3 = ~(mask_1 | mask_2)
-        u_update[mask_3] = 0
-        return u_update
-
-    def _prox_lam_g(self, x):
-        norm = np.linalg.norm(x)
-        if norm < 1:
-            return x
-        else:
-            return x / max(1, norm)
+# from typing import Iterable, Union
+#
+# import numpy as np
+#
+# from cca_zoo.utils import _process_parameter
+#
+# from ._base import BaseIterative, BaseLoop
+# from ._deflation import DeflationMixin
+#
+#
+# class SCCA_ADMM(BaseIterative, DeflationMixin):
+#     r"""
+#     Fits a sparse CCA model by alternating ADMM for two or more views.
+#
+#     .. math::
+#
+#         w_{opt}=\underset{w}{\mathrm{argmax}}\{\sum_i\sum_{j\neq i} \|X_iw_i-X_jw_j\|^2 + \|w_i\|_1\}\\
+#
+#         \text{subject to:}
+#
+#         w_i^TX_i^TX_iw_i=1
+#
+#     Parameters
+#     ----------
+#     latent_dimensions : int, default=1
+#         Number of latent dimensions to use in the model.
+#     copy_data : bool, default=True
+#         Whether to copy the data or overwrite it.
+#     random_state : int, default=None
+#         Random seed for initialisation.
+#     deflation : str, default="cca"
+#         Deflation method to use. Options are "cca" and "pls".
+#     tau : float or list of floats, default=None
+#         Regularisation parameter. If a single float is given, the same value is used for all views.
+#         If a list of floats is given, the values are used for each view.
+#     mu : float or list of floats, default=None
+#         Regularisation parameter. If a single float is given, the same value is used for all views.
+#         If a list of floats is given, the values are used for each view.
+#     lam : float or list of floats, default=None
+#         Regularisation parameter. If a single float is given, the same value is used for all views.
+#         If a list of floats is given, the values are used for each view.
+#     eta : float or list of floats, default=None
+#         Regularisation parameter. If a single float is given, the same value is used for all views.
+#         If a list of floats is given, the values are used for each view.
+#     tol : float, default=1e-9
+#         Tolerance for convergence.
+#
+#     References
+#     ----------
+#     Suo, Xiaotong, et al. "Sparse canonical correlation analysis." arXiv preprint arXiv:1705.10865 (2017).
+#
+#     Examples
+#     --------
+#     >>> from cca_zoo.linear import SCCA_ADMM
+#     >>> import numpy as np
+#     >>> rng=np.random.RandomState(0)
+#     >>> X1 = rng.random((10,5))
+#     >>> X2 = rng.random((10,5))
+#     >>> model = SCCA_ADMM(random_state=0,tau=[1e-1,1e-1])
+#     >>> model.fit((X1,X2)).score((X1,X2))
+#     array([0.84348183])
+#     """
+#
+#     def __init__(
+#         self,
+#         latent_dimensions: int = 1,
+#         copy_data=True,
+#         random_state=None,
+#         tau: Union[Iterable[float], float] = None,
+#         mu: Union[Iterable[float], float] = None,
+#         lam: Union[Iterable[float], float] = None,
+#         eta: Union[Iterable[float], float] = None,
+#         initialization: Union[str, callable] = "pls",
+#         tol: float = 1e-3,
+#     ):
+#         self.tau = tau
+#         self.mu = mu
+#         self.lam = lam
+#         self.eta = eta
+#         super().__init__(
+#             latent_dimensions=latent_dimensions,
+#             copy_data=copy_data,
+#             initialization=initialization,
+#             tol=tol,
+#             random_state=random_state,
+#         )
+#
+#     def _check_params(self):
+#         self.tau = _process_parameter("tau", self.tau, 0, self.n_views_)
+#         self.lam = _process_parameter("lam", self.lam, 1, self.n_views_)
+#         self.eta = _process_parameter("eta", self.eta, 0, self.n_views_)
+#
+#     def _get_pl_module(self, weights=None, k=None):
+#         return SCCA_ADMM_PL(
+#             weights=weights,
+#             k=k,
+#             tau=self.tau,
+#             lam=self.lam,
+#             eta=self.eta,
+#             n_samples_=self.n_samples_,
+#             n_views_=self.n_views_,
+#         )
+#
+#
+# class SCCA_ADMM_PL(BaseLoop):
+#     def __init__(
+#         self,
+#         weights,
+#         k=None,
+#         n_samples_=None,
+#         n_views_=None,
+#         tau=None,
+#         eta=None,
+#         lam=None,
+#         mu=None,
+#     ):
+#         super().__init__(weights=weights, k=k)
+#         self.eta = [np.ones(n_samples_) * eta for eta in eta]
+#         self.z = [np.ones(n_samples_)] * n_views_
+#         self.mu = mu
+#
+#     def training_step(self, batch, batch_idx):
+#         views = batch["views"]
+#         scores = np.stack(self(views))
+#         for view_index, view in enumerate(views):
+#             targets = np.ma.array(scores, mask=False)
+#             targets.mask[view_index] = True
+#             gradient = views[view_index].T @ targets.sum(axis=0).filled()
+#             mu = self.mu[view_index]
+#             lam = self.lam[view_index]
+#             N = views[view_index].shape[0]
+#             unnorm_z = []
+#             norm_eta = []
+#             norm_weights = []
+#             norm_proj = []
+#             for _ in range(self.max_iter):
+#                 # We multiply 'tau' by N in order to make regularisation match across the different sparse cca methods
+#                 self.weights[view_index] = self._prox_mu_f(
+#                     self.weights[view_index]
+#                     - mu
+#                     / lam
+#                     * views[view_index].T
+#                     @ (
+#                         views[view_index] @ self.weights[view_index]
+#                         - self.z[view_index]
+#                         + self.eta[view_index]
+#                     ),
+#                     mu,
+#                     gradient,
+#                     N * self.tau[view_index],
+#                 )
+#                 unnorm_z.append(
+#                     np.linalg.norm(
+#                         views[view_index] @ self.weights[view_index]
+#                         + self.eta[view_index]
+#                     )
+#                 )
+#                 self.z[view_index] = self._prox_lam_g(
+#                     views[view_index] @ self.weights[view_index] + self.eta[view_index]
+#                 )
+#                 self.eta[view_index] = (
+#                     self.eta[view_index]
+#                     + views[view_index] @ self.weights[view_index]
+#                     - self.z[view_index]
+#                 )
+#                 norm_eta.append(np.linalg.norm(self.eta[view_index]))
+#                 norm_proj.append(
+#                     np.linalg.norm(views[view_index] @ self.weights[view_index])
+#                 )
+#                 norm_weights.append(np.linalg.norm(self.weights[view_index], 1))
+#
+#     def _prox_mu_f(self, x, mu, c, tau):
+#         u_update = x.copy()
+#         mask_1 = x + (mu * c) > mu * tau
+#         # if mask_1.sum()>0:
+#         u_update[mask_1] = x[mask_1] + mu * (c[mask_1] - tau)
+#         mask_2 = x + (mu * c) < -mu * tau
+#         # if mask_2.sum() > 0:
+#         u_update[mask_2] = x[mask_2] + mu * (c[mask_2] + tau)
+#         mask_3 = ~(mask_1 | mask_2)
+#         u_update[mask_3] = 0
+#         return u_update
+#
+#     def _prox_lam_g(self, x):
+#         norm = np.linalg.norm(x)
+#         if norm < 1:
+#             return x
+#         else:
+#             return x / max(1, norm)
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_scca_span.py` & `cca_zoo-2.2.0/cca_zoo/linear/_iterative/_scca_span.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Iterable, Union
-
-import numpy as np
-
-from cca_zoo.linear._iterative._base import BaseIterative, BaseLoop
+from cca_zoo.linear._search import support_threshold
+from typing import Union, Iterable
+from cca_zoo.linear._iterative._base import BaseIterative
 from cca_zoo.linear._iterative._deflation import DeflationMixin
-from cca_zoo.linear._search import _delta_search, support_threshold
+from cca_zoo.linear._search import _delta_search
 from cca_zoo.utils import _process_parameter
+import numpy as np
 
 
 class SCCA_Span(DeflationMixin, BaseIterative):
     r"""
     Fits a Sparse CCA model using SpanCCA.
 
     .. math::
@@ -19,53 +18,40 @@
         \text{subject to:}
 
         w_i^TX_i^TX_iw_i=1
 
     References
     ----------
     Asteris, Megasthenis, et al. "A simple and provable algorithm for sparse diagonal CCA." International Conference on Machine Learning. PMLR, 2016.
-
-
-    Examples
-    --------
-    >>> from cca_zoo.linear import SCCA_Span
-    >>> import numpy as np
-    >>> rng=np.random.RandomState(0)
-    >>> X1 = rng.random((10,5))
-    >>> X2 = rng.random((10,5))
-    >>> model = SCCA_Span(regularisation="l0", tau=[2, 2])
-    >>> model.fit((X1,X2)).score((X1,X2))
-    array([0.84556666])
     """
 
     def __init__(
         self,
         latent_dimensions: int = 1,
         epochs: int = 100,
         copy_data=True,
-        initialization: str = "uniform",
+        initialization: str = "pls",
         tol: float = 1e-3,
         regularisation="l0",
         tau: Union[Iterable[Union[float, int]], Union[float, int]] = None,
         rank=1,
         positive: Union[Iterable[bool], bool] = None,
         random_state=None,
-        deflation="cca",
-        verbose=0,
+        verbose=True,
+        early_stopping=False,
     ):
         super().__init__(
             latent_dimensions=latent_dimensions,
             epochs=epochs,
             copy_data=copy_data,
             initialization=initialization,
             tol=tol,
             random_state=random_state,
-            deflation=deflation,
             verbose=verbose,
-            trainer_kwargs={"accelerator": "cpu"},
+            early_stopping=early_stopping,
         )
         self.tau = tau
         self.regularisation = regularisation
         self.rank = rank
         self.positive = positive
 
     def _check_params(self):
@@ -78,66 +64,42 @@
         elif self.regularisation == "l1":
             self.update = _delta_search
         self.tau = _process_parameter("tau", self.tau, 0, self.n_views_)
         self.positive = _process_parameter(
             "positive", self.positive, False, self.n_views_
         )
 
-    def _get_module(self, weights=None, k=None):
-        return SpanLoop(
-            weights=weights,
-            k=k,
-            regularisation=self.regularisation,
-            tau=self.tau,
-            positive=self.positive,
-            rank=self.rank,
-            random_state=self.random_state,
-        )
-
-
-class SpanLoop(BaseLoop):
-    def __init__(
-        self,
-        weights,
-        k=None,
-        regularisation="l0",
-        tau=None,
-        positive=False,
-        rank=1,
-        random_state=None,
-    ):
-        super().__init__(weights=weights, k=k)
-        self.regularisation = regularisation
-        self.tau = tau
-        self.positive = positive
-        if self.regularisation == "l0":
-            self.update = support_threshold
-        elif self.regularisation == "l1":
-            self.update = _delta_search
-        self.rank = rank
-        self.random_state = random_state
+    def _update_weights(self, views: np.ndarray, i: int) -> None:
+        """Update the weights for the i-th component.
 
-    def training_step(self, batch, batch_idx):
-        # if P, _D, Q not initialised, initialise them
+        Args:
+            views (np.ndarray): The input views as numpy arrays.
+            i (int): The index of the component.
+        """
+        # if P, D, Q not initialised, initialise them
         if getattr(self, "P", None) is None:
-            self._initialize(batch["views"])
-        c = self.random_state.randn(self.rank)
-        c /= np.linalg.norm(c)
-        a = self.P @ np.diag(self.D) @ c
-        u = self.update(a, self.tau[0])
-        u /= np.linalg.norm(u)
-        b = self.Q @ np.diag(self.D) @ self.P.T @ u
-        v = self.update(b, self.tau[1])
-        v /= np.linalg.norm(v)
-        if b.T @ v > self.max_obj:
-            self.max_obj = b.T @ v
-            self.weights[0] = u
-            self.weights[1] = v
+            self._initialize_variables(views)
+        if i == 0:
+            # generate a random vector c
+            c = np.random.randn(self.rank)
+            c /= np.linalg.norm(c)
+            # compute a = P D c
+            a = self.P @ np.diag(self.D) @ c
+            # apply the update function to a with tau[0]
+            u = self.update(a, self.tau[0])
+            u /= np.linalg.norm(u)
+            # update the objective value and the weights if improved
+            return u[:, np.newaxis]
+        elif i == 1:
+            b = self.Q @ np.diag(self.D) @ self.P.T @ self.weights[0]
+            v = self.update(b, self.tau[1])
+            v /= np.linalg.norm(v)
+            return v
 
-    def _initialize(self, views):
-        self.max_obj = 0
+    def _initialize_variables(self, views):
+        self.max_obj = [0, 0]
         cov = views[0].T @ views[1] / views[0].shape[0]
         # Perform SVD on im and obtain individual matrices
         P, D, Q = np.linalg.svd(cov, full_matrices=True)
         self.P = P[:, : self.rank]
         self.D = D[: self.rank]
         self.Q = Q[: self.rank, :].T
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_iterative/_swcca.py` & `cca_zoo-2.2.0/cca_zoo/linear/_iterative/_swcca.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,109 +1,105 @@
-from itertools import combinations
-from typing import Iterable, Union
-
-import numpy as np
-
-from cca_zoo.linear._iterative._base import BaseIterative
-from cca_zoo.linear._iterative._deflation import DeflationMixin
-from cca_zoo.linear._search import _delta_search, support_threshold
-from cca_zoo.utils import _process_parameter
-
-
-class SWCCA(BaseIterative, DeflationMixin):
-    r"""
-    A class used to fit SWCCA model
-
-    References
-    ----------
-    .. Wenwen, M. I. N., L. I. U. Juan, and Shihua Zhang. "Sparse Weighted Canonical Correlation Analysis." Chinese Journal of Electronics 27.3 (2018): 459-466.
-
-    Examples
-    --------
-    >>> from cca_zoo.linear import SWCCA
-    >>> import numpy as np
-    >>> rng=np.random.RandomState(0)
-    >>> X1 = rng.random((10,5))
-    >>> X2 = rng.random((10,5))
-    >>> model = SWCCA(regularisation='l0',tau=[2, 2], sample_support=5, random_state=0)
-    >>> model.fit((X1,X2)).score((X1,X2))
-    array([0.61620969])
-    """
-
-    def __init__(
-        self,
-        scale: bool = True,
-        centre=True,
-        copy_data=True,
-        random_state=None,
-        max_iter: int = 500,
-        initialization: str = "random",
-        tol: float = 1e-3,
-        regularisation="l0",
-        tau: Union[Iterable[Union[float, int]], Union[float, int]] = None,
-        sample_support=None,
-        positive=False,
-        verbose=0,
-    ):
-        self.tau = tau
-        self.sample_support = sample_support
-        if regularisation == "l0":
-            self.update = support_threshold
-        elif regularisation == "l1":
-            self.update = _delta_search
-        self.regularisation = regularisation
-        self.positive = positive
-        super().__init__(
-            latent_dims=1,
-            scale=scale,
-            centre=centre,
-            copy_data=copy_data,
-            max_iter=max_iter,
-            initialization=initialization,
-            tol=tol,
-            random_state=random_state,
-            verbose=verbose,
-        )
-
-    def _check_params(self):
-        if self.sample_support is None:
-            self.sample_support = self.n
-        self.tau = _process_parameter("tau", self.tau, 2, self.n_views)
-        self.positive = _process_parameter(
-            "positive", self.positive, False, self.n_views
-        )
-
-    def _initialize(self, views):
-        self.sample_weights = np.ones(self.n)
-        self.sample_weights /= np.linalg.norm(self.sample_weights)
-
-    def _update(self, views, scores, weights):
-        # Update each view using loop update function
-        for view_index, view in enumerate(views):
-            targets = np.ma.array(scores, mask=False)
-            targets.mask[view_index] = True
-            weights[view_index] = (
-                views[view_index] * self.sample_weights[:, np.newaxis]
-            ).T @ targets.sum(axis=0).filled()
-            weights[view_index] = self.update(
-                weights[view_index],
-                self.tau[view_index],
-                positive=self.positive[view_index],
-            )
-            weights[view_index] /= np.linalg.norm(weights[view_index])
-            if view_index == self.n_views - 1:
-                self.sample_weights = self._update_sample_weights(scores)
-            scores[view_index] = views[view_index] @ weights[view_index]
-        return scores, weights
-
-    def _update_sample_weights(self, scores):
-        w = scores.prod(axis=0)
-        sample_weights = support_threshold(w, self.sample_support)
-        sample_weights /= np.linalg.norm(sample_weights)
-        return sample_weights
-
-    def _objective(self, views, scores, weights) -> int:
-        # default objective is correlation
-        obj = 0
-        for score_i, score_j in combinations(scores, 2):
-            obj += (score_i * self.sample_weights).T @ score_j
-        return obj
+# from itertools import combinations
+# from typing import Iterable, Union
+#
+# import numpy as np
+#
+# from cca_zoo.linear._iterative._base import BaseIterative
+# from cca_zoo.linear._iterative._deflation import DeflationMixin
+# from cca_zoo.linear._search import _delta_search, support_threshold
+# from cca_zoo.utils import _process_parameter
+#
+#
+# class SWCCA(BaseIterative, DeflationMixin):
+#     r"""
+#     A class used to fit SWCCA model
+#
+#     References
+#     ----------
+#     .. Wenwen, M. I. N., L. I. U. Juan, and Shihua Zhang. "Sparse Weighted Canonical Correlation Analysis." Chinese Journal of Electronics 27.3 (2018): 459-466.
+#
+#     Examples
+#     --------
+#     >>> from cca_zoo.linear import SWCCA
+#     >>> import numpy as np
+#     >>> rng=np.random.RandomState(0)
+#     >>> X1 = rng.random((10,5))
+#     >>> X2 = rng.random((10,5))
+#     >>> model = SWCCA(regularisation='l0',tau=[2, 2], sample_support=5, random_state=0)
+#     >>> model.fit((X1,X2)).score((X1,X2))
+#     array([0.61620969])
+#     """
+#
+#     def __init__(
+#         self,
+#         copy_data=True,
+#         random_state=None,
+#         max_iter: int = 500,
+#         initialization: str = "random",
+#         tol: float = 1e-3,
+#         regularisation="l0",
+#         tau: Union[Iterable[Union[float, int]], Union[float, int]] = None,
+#         sample_support=None,
+#         positive=False,
+#         verbose=0,
+#     ):
+#         self.tau = tau
+#         self.sample_support = sample_support
+#         if regularisation == "l0":
+#             self.update = support_threshold
+#         elif regularisation == "l1":
+#             self.update = _delta_search
+#         self.regularisation = regularisation
+#         self.positive = positive
+#         super().__init__(
+#             latent_dims=1,
+#             copy_data=copy_data,
+#             max_iter=max_iter,
+#             initialization=initialization,
+#             tol=tol,
+#             random_state=random_state,
+#             verbose=verbose,
+#         )
+#
+#     def _check_params(self):
+#         if self.sample_support is None:
+#             self.sample_support = self.n
+#         self.tau = _process_parameter("tau", self.tau, 2, self.n_views)
+#         self.positive = _process_parameter(
+#             "positive", self.positive, False, self.n_views
+#         )
+#
+#     def _initialize(self, views):
+#         self.sample_weights = np.ones(self.n)
+#         self.sample_weights /= np.linalg.norm(self.sample_weights)
+#
+#     def _update(self, views, scores, weights):
+#         # Update each view using loop update function
+#         for view_index, view in enumerate(views):
+#             targets = np.ma.array(scores, mask=False)
+#             targets.mask[view_index] = True
+#             weights[view_index] = (
+#                 views[view_index] * self.sample_weights[:, np.newaxis]
+#             ).T @ targets.sum(axis=0).filled()
+#             weights[view_index] = self.update(
+#                 weights[view_index],
+#                 self.tau[view_index],
+#                 positive=self.positive[view_index],
+#             )
+#             weights[view_index] /= np.linalg.norm(weights[view_index])
+#             if view_index == self.n_views - 1:
+#                 self.sample_weights = self._update_sample_weights(scores)
+#             scores[view_index] = views[view_index] @ weights[view_index]
+#         return scores, weights
+#
+#     def _update_sample_weights(self, scores):
+#         w = scores.prod(axis=0)
+#         sample_weights = support_threshold(w, self.sample_support)
+#         sample_weights /= np.linalg.norm(sample_weights)
+#         return sample_weights
+#
+#     def _objective(self, views, scores, weights) -> int:
+#         # default objective is correlation
+#         obj = 0
+#         for score_i, score_j in combinations(scores, 2):
+#             obj += (score_i * self.sample_weights).T @ score_j
+#         return obj
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_mcca.py` & `cca_zoo-2.2.0/cca_zoo/linear/_mcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Iterable, Union
 
 import numpy as np
-from scipy.linalg import block_diag
-from scipy.linalg import eigh
+from scipy.linalg import block_diag, eigh
 from sklearn.decomposition import PCA
 
 from cca_zoo._base import BaseModel
 from cca_zoo.utils import _process_parameter
 
 
 class MCCA(BaseModel):
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_partialcca.py` & `cca_zoo-2.2.0/cca_zoo/linear/_partialcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_pcacca.py` & `cca_zoo-2.2.0/cca_zoo/linear/_pcacca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_pls.py` & `cca_zoo-2.2.0/cca_zoo/linear/_pls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from cca_zoo.linear._mcca import rCCA, MCCA
 from typing import Iterable
 
 import numpy as np
 
+from cca_zoo.linear._mcca import MCCA, rCCA
+
 
 def reduce_dims(x):
     U, S, _ = np.linalg.svd(x, full_matrices=False)
     return U @ np.diag(S)
 
 
 class PLSMixin:
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_prcca.py` & `cca_zoo-2.2.0/cca_zoo/linear/_prcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_search.py` & `cca_zoo-2.2.0/cca_zoo/linear/_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
-
 from scipy.optimize import minimize
 
 
-def _delta_search(w, c):
+def _delta_search(w, c, tol=1e-8):
     """
     Searches for threshold delta such that the 1-norm of weights w is less than or equal to c and the 2-norm is equal to 1.
     Parameters
     ----------
     w : numpy array
         weights found by one power method iteration
     c : float
@@ -40,36 +39,32 @@
 
     # Find the minimum of f using scipy minimization function
     # You can specify the method or let the function choose the best one for you
     # You can also pass other parameters like tol, maxiter, etc.
     # bound x to be between 0 and 1
 
     # try some different methods until one gets result.success == True
-    result = minimize(f, x0=0, bounds=[(0, 1)], method="L-BFGS-B")
+    result = minimize(f, x0=0, bounds=[(0, 1)], method="L-BFGS-B", tol=tol)
     if not result.success:
-        result = minimize(f, x0=0, bounds=[(0, 1)], method="TNC")
+        result = minimize(f, x0=0, bounds=[(0, 1)], method="TNC", tol=tol)
     if not result.success:
-        result = minimize(f, x0=0, bounds=[(0, 1)], method="SLSQP")
+        result = minimize(f, x0=0, bounds=[(0, 1)], method="SLSQP", tol=tol)
     if not result.success:
-        result = minimize(f, x0=0, bounds=[(0, 1)], method="trust-constr")
+        result = minimize(f, x0=0, bounds=[(0, 1)], method="trust-constr", tol=tol)
 
     # Check if the solution is valid and converged
     if result.success:
         # Get the optimal delta from the result object
         delta = result.x
 
         # Apply soft thresholding to the weights with optimal delta
         coef = np.where(w - delta > 0, w - delta, 0) - np.where(
             -w - delta > 0, -w - delta, 0
         )
 
-        # if all coefficients are zero
-        if np.sum(coef**2) == 0:
-            print()
-
         # Normalize the coefficients to unit length if nonzero
         coef /= np.linalg.norm(coef)
 
         # Return updated weights
         return coef
 
     else:
```

### Comparing `cca_zoo-2.1.0/cca_zoo/linear/_tcca.py` & `cca_zoo-2.2.0/cca_zoo/linear/_tcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/model_selection/_validation.py` & `cca_zoo-2.2.0/cca_zoo/model_selection/_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import itertools
 
 import numpy as np
-from joblib import Parallel
 from mvlearn.compose import SimpleSplitter
 from sklearn import clone
 from sklearn.base import is_classifier
 from sklearn.metrics import check_scoring
-from sklearn.model_selection import check_cv
-from sklearn.model_selection import cross_validate as cross_validate_
+from sklearn.model_selection import cross_validate as cross_validate_, check_cv
 from sklearn.model_selection import learning_curve as learning_curve_
+from sklearn.model_selection._validation import _permutation_test_score, _shuffle
 from sklearn.pipeline import Pipeline
-from sklearn.utils import _safe_indexing, check_random_state, indexable
-from sklearn.utils.fixes import delayed
-from sklearn.utils.metaestimators import _safe_split
-from sklearn.utils.validation import _check_fit_params
+from sklearn.utils import indexable, check_random_state
+from sklearn.utils.parallel import Parallel, delayed
 
 
 def default_scoring(estimator, scoring, views):
     if callable(scoring):
         return scoring
     elif scoring is None:
         if len(views) > 2:
@@ -121,15 +118,15 @@
               as in '2*n_jobs'
 
     :Example:
 
     """
     estimator = Pipeline(
         [
-            ("splitter", SimpleSplitter([X_.shape[1] for X_ in views])),
+            ("splitter", SimpleSplitter([view.shape[1] for view in views])),
             ("estimator", clone(estimator)),
         ]
     )
     ret = cross_validate_(
         estimator,
         np.hstack(views),
         y=y,
@@ -223,81 +220,56 @@
     :param verbose: int, default=0
         The verbosity level.
     :param fit_params: dict, default=None
         Parameters to pass to the fit method of the estimator.
         .. versionadded:: 0.24
 
     """
-    scorer = default_scoring(estimator, scoring, views)
     estimator = Pipeline(
         [
-            ("splitter", SimpleSplitter([X_.shape[1] for X_ in views])),
+            ("splitter", SimpleSplitter([view.shape[1] for view in views])),
             ("estimator", clone(estimator)),
         ]
     )
-    views, y, groups = indexable(np.hstack(views), y, groups)
 
+    if y is None:
+        y = np.zeros(views[0].shape[0])
+    X = np.hstack(views)
+    X, y, groups = indexable(X, y, groups)
     cv = check_cv(cv, y, classifier=is_classifier(estimator))
-
+    if scoring is None:
+        scoring = default_scoring(estimator, scoring, views)
+    scorer = check_scoring(estimator, scoring=scoring)
     random_state = check_random_state(random_state)
 
     # We clone the estimator to make sure that all the folds are
     # independent, and that it is pickle-able.
     score = _permutation_test_score(
-        clone(estimator), views, y, groups, cv, scorer, fit_params=fit_params
+        clone(estimator), X, y, groups, cv, scorer, fit_params=fit_params
     )
     permutation_scores = Parallel(n_jobs=n_jobs, verbose=verbose)(
         delayed(_permutation_test_score)(
             clone(estimator),
-            _shuffle(views, groups, random_state, estimator["splitter"]),
+            np.hstack((_shuffle(views[0], groups, random_state), *views[1:])),
             y,
             groups,
             cv,
             scorer,
             fit_params=fit_params,
         )
         for _ in range(n_permutations)
     )
     permutation_scores = np.array(permutation_scores)
-    pvalue = (np.sum(permutation_scores >= score, axis=0) + 1.0) / (n_permutations + 1)
+    pvalue = (np.sum(permutation_scores >= score) + 1.0) / (n_permutations + 1)
     return score, permutation_scores, pvalue
 
 
-def _permutation_test_score(estimator, X, y, groups, cv, scorer, fit_params):
-    """Auxiliary function for permutation_test_score"""
-    # Adjust length of sample weights
-    fit_params = fit_params if fit_params is not None else {}
-    avg_score = []
-    for train, test in cv.split(X, y, groups):
-        X_train, y_train = _safe_split(estimator, X, y, train)
-        X_test, y_test = _safe_split(estimator, X, y, test, train)
-        fit_params = _check_fit_params(X, fit_params, train)
-        estimator.fit(X_train, y_train, **fit_params)
-        avg_score.append(scorer(estimator, X_test, y_test))
-    return np.mean(avg_score, axis=0)
-
-
-def _shuffle(X, groups, random_state, splitter):
-    """Return a shuffled copy of y eventually shuffle among same groups."""
-    X = splitter.fit_transform(X)
-    for i, X_ in enumerate(X):
-        if groups is None:
-            indices = random_state.permutation(len(X_))
-        else:
-            indices = np.arange(len(groups))
-            for group in np.unique(groups):
-                this_mask = groups == group
-                indices[this_mask] = random_state.permutation(indices[this_mask])
-        X[i] = _safe_indexing(X_, indices)
-    return np.hstack(X)
-
-
 def learning_curve(
     estimator,
-    views,
+    X,
     y=None,
     groups=None,
     train_sizes=np.linspace(0.1, 1.0, 5),
     cv=None,
     scoring=None,
     exploit_incremental_learning=False,
     n_jobs=None,
@@ -390,21 +362,21 @@
     :param fit_params: dict, default=None
         Parameters to pass to the fit method of the estimator.
         .. versionadded:: 0.24
 
     """
     estimator = Pipeline(
         [
-            ("splitter", SimpleSplitter([X_.shape[1] for X_ in views])),
+            ("splitter", SimpleSplitter([X_.shape[1] for X_ in X])),
             ("estimator", clone(estimator)),
         ]
     )
     return learning_curve_(
         estimator,
-        np.hstack(views),
+        np.hstack(X),
         y,
         groups=groups,
         train_sizes=train_sizes,
         cv=cv,
         scoring=scoring,
         exploit_incremental_learning=exploit_incremental_learning,
         n_jobs=n_jobs,
```

### Comparing `cca_zoo-2.1.0/cca_zoo/nonparametric/_gradkcca.py` & `cca_zoo-2.2.0/cca_zoo/nonparametric/_scca_hsic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,140 +1,162 @@
 from typing import Iterable, Union
 
 import numpy as np
 import numpy.linalg as la
-from sklearn.kernel_approximation import Nystroem
-from sklearn.metrics import pairwise_kernels
+from sklearn.preprocessing import KernelCenterer
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.linear._iterative._base import BaseIterative
-from cca_zoo.nonparametric._kcca import KernelMixin
+from _gradkcca import GradKCCA
 from cca_zoo.utils import _process_parameter
 
 
-class GradKCCA(BaseIterative, KernelMixin):
+class SCCA_HSIC(GradKCCA):
     """
     References
     ----------
-    [1] Viivi Uurtio, Sahely Bhadra, and Juho Rousu. Large-scale sparse kernel canonical correlation analysis. In Kamalika Chaudhuri and Ruslan Salakhutdinov, editors, Proceedings of the 36th International Conference on Machine Learning, volume 97 of Proceedings of Machine Learning Research, pages 6383–6391, Long Beach, California, USA, 09–15 Jun 2019. PMLR.
+    [1] Uurtio, V., Bhadra, S., Rousu, J. Sparse Non-Linear CCA through Hilbert-Schmidt Independence Criterion. IEEE International Conference on Data Mining (ICDM 2018), to appear
 
     """
 
     def __init__(
         self,
         latent_dimensions: int = 1,
         scale: bool = True,
         centre=True,
         copy_data=True,
         random_state=None,
         proj: Union[Iterable[float], float] = "l1",
-        kernel: Iterable[Union[float, callable]] = None,
         gamma: Iterable[float] = None,
-        degree: Iterable[float] = None,
         coef0: Iterable[float] = None,
-        kernel_params: Iterable[dict] = None,
         repetitions=5,
         initialization: Union[str, callable] = "random",
         nystrom=False,
         nystrom_components=100,
+        c=1,
     ):
         super().__init__(
             latent_dimensions=latent_dimensions,
             scale=scale,
             centre=centre,
             copy_data=copy_data,
             random_state=random_state,
             initialization=initialization,
+            proj=proj,
+            gamma=gamma,
+            coef0=coef0,
+            kernel="rbf",
+            repetitions=repetitions,
+            nystrom=nystrom,
+            nystrom_components=nystrom_components,
         )
-        self.proj = proj
-        self.kernel_params = kernel_params
-        self.gamma = gamma
-        self.coef0 = coef0
-        self.kernel = kernel
-        self.degree = degree
-        self.repetitions = repetitions
-        self.nystrom = nystrom
-        self.nystrom_components = nystrom_components
+        self.c = c
 
     def _check_params(self):
-        self.proj = _process_parameter("proj", self.proj, "l1", self.n_views)
-        self.kernel = _process_parameter("kernel", self.kernel, "linear", self.n_views)
-        self.gamma = _process_parameter("gamma", self.gamma, None, self.n_views)
-        self.coef0 = _process_parameter("coef0", self.coef0, 1, self.n_views)
-        self.degree = _process_parameter("degree", self.degree, 1, self.n_views)
-        self.nystrom_components = _process_parameter(
-            "nystrom components", self.nystrom_components, 100, self.n_views
-        )
+        self.proj = _process_parameter("proj", self.proj, None, self.n_views_)
+        self.kernel = _process_parameter("kernel", self.kernel, "linear", self.n_views_)
+        self.gamma = _process_parameter("gamma", self.gamma, None, self.n_views_)
+        self.coef0 = _process_parameter("coef0", self.coef0, 1, self.n_views_)
+        self.degree = _process_parameter("degree", self.degree, 1, self.n_views_)
+        self.c = _process_parameter("c", self.c, 1, self.n_views_)
+
+    def _objective(self, views, scores, weights) -> int:
+        N = scores[0].shape[0]
+        return np.trace(scores[0] @ scores[1]).sum() / (N - 1) ** 2
 
-    def backracking_line_search(self, w, gw, stp, X, K, obj_old, view_index):
+    def backracking_line_search(self, w, gw, stp, X, cKv, obj_old, view_index):
         while True:
             w_new = w + gw * stp
-            w_new = w_new / la.norm(w_new)
-            Kw_new = self._get_kernel(view_index, X, w_new[None, :])
-            obj_new = self._objective(None, (Kw_new, K), None)
+            if self.proj[view_index] == "l1":
+                w_new = self._proj_l1(w_new, self.c[view_index])
+            elif self.proj[view_index] == "l2":
+                w_new = self._proj_l2(w_new, self.c[view_index])
+            else:
+                raise ValueError(
+                    "projection {self.proj[view_index]} not supported. Pass a generator implementing this method"
+                )
+            Kw = self._get_kernel(view_index, X @ w_new[:, None])
+            obj_new = self._objective(None, (Kw, cKv), None)
             if obj_new > obj_old + 1e-4 * np.abs(obj_old):
-                w = w_new
-                break
+                return w_new
             elif stp < 1e-7:
-                w = w_new
-                break
+                return w
             else:
                 stp /= 2
-        return w
-
-    def _objective(self, views, scores, weights) -> int:
-        return (
-            scores[0].T
-            @ scores[1]
-            / (np.sqrt(scores[0].T @ scores[0]) * np.sqrt(scores[1].T @ scores[1]))
-        )
-
-    def _proj_l1(self, v, b):
-        assert b > 0
-        if la.norm(v, 1) < b:
-            return v
-        u = -np.sort(-np.abs(v))
-        sv = np.cumsum(u)
-        r = np.where(u > (sv - b) / np.arange(1, u.shape[0] + 1))
-        if len(r[-1]) > 0:
-            rho = r[-1][-1]
-            tau = (sv[rho] - b) / rho
-            theta = np.maximum(0, tau)
-            return np.sign(v) * np.maximum(np.abs(v) - theta, 0)
-        else:
-            return v
-
-    def _proj_l2(self, v, b):
-        return v / la.norm(v) / b
 
     def _update(self, views, scores, weights):
-        scores = [
-            self._get_kernel(i, view, weights[i][None, :])
+        flipped_idxs = [1, 0]
+        K = [
+            self._get_kernel(i, view @ weights[i][:, None])
             for i, view in enumerate(views)
         ]
-        obj_old = self._objective(views, scores, weights)
-        for view_index, view in enumerate(views):
-            # TODO gradients
-            grad = 0
+        cK = [KernelCenterer().fit_transform(K_) for K_ in K]
+        weights = [
+            self._proj_l2(w, self.c[view_index]) for view_index, w in enumerate(weights)
+        ]
+        for view_index, (view, flipped_idx) in enumerate(zip(views, flipped_idxs)):
+            obj_old = self._objective(views, (K[view_index], cK[flipped_idx]), weights)
+            grad = gradf_gauss_sgd(
+                K[view_index],
+                cK[flipped_idx],
+                view,
+                self.gamma[view_index],
+                weights[view_index],
+            )
             gamma = la.norm(grad)
             weights[view_index] = self.backracking_line_search(
                 weights[view_index],
                 grad,
                 gamma,
                 view,
-                scores[view_index],
+                cK[flipped_idx],
                 obj_old,
                 view_index,
             )
-            if self.proj[view_index] == "l1":
-                weights[view_index] = self._proj_l1(
-                    weights[view_index], self.c[view_index]
-                )
-            elif self.proj[view_index] == "l2":
-                weights[view_index] = self._proj_l2(
-                    weights[view_index], self.c[view_index]
-                )
-            else:
-                raise ValueError(
-                    "projection {self.proj[view_index]} not supported. Pass a generator implementing this method"
-                )
-        return scores, weights
+            K[view_index] = self._get_kernel(
+                view_index, view @ weights[view_index][:, None]
+            )
+            cK[view_index] = KernelCenterer().fit_transform(K[view_index])
+        return K, weights
+
+    def transform(self, views: Iterable[np.ndarray], **kwargs):
+        """
+
+        Parameters
+        ----------
+        views : list/tuple of numpy arrays or array likes with the same number of rows (samples)
+        kwargs : any additional keyword arguments required by the given model
+
+        Returns
+        -------
+        transformed_views : list of numpy arrays
+
+        """
+        check_is_fitted(self, attributes=["weights"])
+        transformed_views = []
+        for i, (view) in enumerate(views):
+            transformed_view = view @ self.weights[i]
+            transformed_views.append(transformed_view)
+        return transformed_views
+
+
+def gradf_gauss_sgd(K1, cK2, X, a, u):
+    if a is None:
+        a = 1 / X.shape[1]
+    N = K1.shape[0]
+    temp = 0
+    id1 = np.argsort(np.random.rand(N))[: int(N / 10)]
+    id2 = np.argsort(np.random.rand(N))[: int(N / 10)]
+    for i in id1:
+        for j in id2:
+            temp += (
+                K1[i, j] * cK2[i, j] * np.outer(X[i, :] - X[j, :], X[i, :] - X[j, :])
+            )
+    return -(2 * a * u.T @ temp).T
+
+
+def generate_data(n, p, q):
+    X = np.random.uniform(-1, 1, [n, p])
+    Y = np.random.uniform(-1, 1, [n, q])
+    Y[:, 2] = X[:, 2] + X[:, 3] - Y[:, 3] + np.random.normal(0, 0.05, n)
+    # Y[:,2] = np.power(views[:,2] + views[:,3],3) - Y[:,3] + np.random.normal(0,0.05,n)
+    # Y[:,4] = np.exp(views[:,4] + views[:,5]) - Y[:,5] + np.random.normal(0,0.05,n)
+    return X, Y
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cca_zoo-2.1.0/cca_zoo/nonparametric/_kcca.py` & `cca_zoo-2.2.0/cca_zoo/nonparametric/_kcca.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Iterable, Union
 
 import numpy as np
 from scipy.linalg import block_diag
 from sklearn.metrics import pairwise_kernels
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.utils import _process_parameter
 from cca_zoo.linear._gcca import GCCA
 from cca_zoo.linear._mcca import MCCA
 from cca_zoo.linear._tcca import TCCA
+from cca_zoo.utils import _process_parameter
 
 
 class KernelMixin:
     def _check_params(self):
         self.kernel = _process_parameter("kernel", self.kernel, "linear", self.n_views_)
         self.gamma = _process_parameter("gamma", self.gamma, None, self.n_views_)
         self.coef0 = _process_parameter("coef0", self.coef0, 1, self.n_views_)
```

### Comparing `cca_zoo-2.1.0/cca_zoo/nonparametric/_ncca.py` & `cca_zoo-2.2.0/cca_zoo/nonparametric/_ncca.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         return St[0] @ self.g * (1 / self.S), St[1] @ self.f * (1 / self.S)
 
     def _get_kernel(self, view, X, Y=None):
         # Get the gamma parameter for the RBF kernel
         params = {
             "gamma": self.gamma[view],
         }
-        # Compute the pairwise kernel values between X and Y using the specified kernel function and parameters
+        # Compute the pairwise kernel values between views and Y using the specified kernel function and parameters
         return pairwise_kernels(
             X, Y, metric=self.kernel[view], filter_params=True, **params
         )
 
 
 def fill_w(kernels, inds):
     # Create an empty matrix with the same shape as kernels
```

### Comparing `cca_zoo-2.1.0/cca_zoo/probabilistic/_probabilisticcca.py` & `cca_zoo-2.2.0/cca_zoo/probabilistic/_probabilisticcca.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,52 @@
 from typing import Iterable
 
+import numpy as np
+import numpyro
+from jax.random import PRNGKey
+from sklearn.utils.validation import check_is_fitted
+
+from cca_zoo._base import BaseModel
+
+from typing import Iterable
+
 import jax.numpy as jnp
 import numpy as np
 import numpyro
 import numpyro.distributions as dist
 from jax.random import PRNGKey
 from numpyro.infer import MCMC, NUTS, Predictive
 from sklearn.utils.validation import check_is_fitted
 
 from cca_zoo._base import BaseModel
 
 
 class ProbabilisticCCA(BaseModel):
     """
-    A class used to fit a Probabilistic CCA. Not quite the same due to using VI methods rather than EM
+    A class used to fit a Probabilistic CCA model using variational inference.
+
+    Probabilistic CCA is a generative model that assumes each view of data is generated from a shared latent variable z and some view-specific parameters (mu: mean, psi: covariance, W: weight matrix). The model can be written as:
+
+    z ~ N(0, I)
+    x_i ~ N(W_i z + mu_i, psi_i)
+
+    The model parameters and the latent variables are inferred using MCMC sampling with the NUTS algorithm.
 
     Parameters
     ----------
     latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random state, by default 0
     num_samples : int, optional
-        Number of samples to use in VI, by default 100
+        Number of samples to use in MCMC, by default 100
     num_warmup : int, optional
-        Number of warmup samples to use in VI, by default 100
+        Number of warmup samples to use in MCMC, by default 100
 
 
     References
     ----------
     Bach, Francis R., and Michael I. Jordan. "A probabilistic interpretation of canonical correlation analysis." (2005).
     Wang, Chong. "Variational Bayesian approach to canonical correlation analysis." IEEE Transactions on Neural Networks 18.3 (2007): 905-910.
 
@@ -50,35 +66,56 @@
             accept_sparse=False,
             random_state=random_state,
         )
         self.num_samples = num_samples
         self.num_warmup = num_warmup
         self.rng_key = PRNGKey(random_state)
 
-    def fit(self, views: Iterable[np.ndarray], y=None, **kwargs):
+    def fit(self, views: Iterable[np.ndarray], y=None):
         """
-        Infer the parameters (mu: mean, psi: within view variance) and latent variables (z) of the generative CCA model
+        Infer the parameters and latent variables of the Probabilistic CCA model.
 
-        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
+        Parameters
+        ----------
+        views : Iterable[np.ndarray]
+            A list or tuple of numpy arrays or array likes with the same number of rows (samples)
+
+        Returns
+        -------
+        self : object
+            Returns the instance itself.
         """
+        # Initialize a NUTS sampler with the model function
         nuts_kernel = NUTS(self._model)
+        # Run MCMC sampling with the specified number of samples and warmup steps
         self.mcmc = MCMC(
             nuts_kernel, num_samples=self.num_samples, num_warmup=self.num_warmup
         )
+        # Run the sampler on the data and store the posterior samples
         self.mcmc.run(self.rng_key, views)
         self.posterior_samples = self.mcmc.get_samples()
         return self
 
-    def transform(self, views: Iterable[np.ndarray], y=None, **kwargs):
+    def transform(self, views: Iterable[np.ndarray], y=None):
         """
-        Predict the latent variables that generate the data in views using the sampled model parameters
+        Predict the latent variables that generate the data in views using the sampled model parameters.
 
-        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
+        Parameters
+        ----------
+        views : Iterable[np.ndarray]
+            A list or tuple of numpy arrays or array likes with the same number of rows (samples)
+
+        Returns
+        -------
+        z : np.ndarray
+            An array of shape (n_samples, latent_dimensions) containing the predicted latent variables for each sample.
         """
+        # Check if the model has been fitted
         check_is_fitted(self, attributes=["posterior_samples"])
+        # Use the predictive function to generate samples of z from the posterior distribution
         return Predictive(self._model, self.posterior_samples, return_sites=["z"])(
             self.rng_key, views
         )["z"]
 
     def _model(self, views: Iterable[np.ndarray]):
         n = views[0].shape[0]
         p = [view.shape[1] for view in views]
@@ -119,9 +156,20 @@
                     obs=X_,
                 )
                 for i, (X_, psi_, mu_, W_) in enumerate(
                     zip(views, psi, mu, self.weights_list)
                 )
             ]
 
+    def transform(self, views: Iterable[np.ndarray], y=None, **kwargs):
+        """
+        Predict the latent variables that generate the data in views using the sampled model parameters
+
+        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
+        """
+        check_is_fitted(self, attributes=["posterior_samples"])
+        return Predictive(self._model, self.posterior_samples, return_sites=["z"])(
+            self.rng_key, views
+        )["z"]
+
     def _more_tags(self):
         return {"probabilistic": True}
```

### Comparing `cca_zoo-2.1.0/cca_zoo/utils/check_values.py` & `cca_zoo-2.2.0/cca_zoo/utils/check_values.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.1.0/cca_zoo/visualisation/plotter.py` & `cca_zoo-2.2.0/cca_zoo/visualisation/plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Code to generate explained covariance scree plots from cca-zoo models
 """
 
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mtick
 import numpy as np
 import pandas as pd
-
 import seaborn as sns
 
 
 # Define a class that takes the dataset object as an argument
 class Plotter:
     def plot_scores_single(
         self,
```

### Comparing `cca_zoo-2.1.0/pyproject.toml` & `cca_zoo-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cca-zoo"
-version = "2.1.0"
+version = "2.2.0"
 description = "Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework"
 authors = ["jameschapman <james.chapman.19@ucl.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jameschapman19/cca_zoo"
 keywords = ["cca"]
 
@@ -36,12 +36,12 @@
 black = "*"
 flake8 = "*"
 codecov = "*"
 pytest-cov = "*"
 
 
 [tool.poetry.extras]
-probabilistic = ["jax", "numpyro", "arviz"]
+probabilistic = ["jax", "numpyro", "arviz", "funsor"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cca_zoo-2.1.0/PKG-INFO` & `cca_zoo-2.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca-zoo
-Version: 2.1.0
+Version: 2.2.0
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 License: MIT
 Keywords: cca
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 Requires-Python: >=3.8,<4.0.0
@@ -28,28 +28,43 @@
 Requires-Dist: tensorly
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; sys_platform == "darwin"
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; sys_platform == "linux"
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; sys_platform == "win32"
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
+<div align="center">
+
+<img src="docs/source/cca-zoo-logo.jpg" alt="drawing" width="200"/>
+
+# CCA-Zoo
+
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
 [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
-![Build Status](https://github.com/jameschapman19/cca_zoo/actions/workflows/python-package.yml/badge.svg)
+![Build Status](https://github.com/jameschapman19/cca_zoo/actions/workflows/changes.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/cca-zoo/badge/?version=latest)](https://cca-zoo.readthedocs.io/en/latest/?badge=latest)
 [![version](https://img.shields.io/pypi/v/cca-zoo)](https://pypi.org/project/cca-zoo/)
 [![downloads](https://img.shields.io/pypi/dm/cca-zoo)](https://pypi.org/project/cca-zoo/)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03823/status.svg)](https://doi.org/10.21105/joss.03823)
 
-# CCA-Zoo
+
+</div>
 
 `cca-zoo` is a collection of linear, kernel, and deep methods for canonical correlation analysis of multiview data.
 Where possible it follows the `scikit-learn`/`mvlearn` APIs and models therefore have `fit`/`transform`/`fit_transform`
 methods as standard.
 
+## Table of Contents
+
+- [Installation](#installation)
+- [Documentation](#documentation)
+- [Citation](#citation)
+- [Contributions](#contributions)
+- [Sources](#sources)
+
 ## Installation
 
 You can install cca-zoo with pip or poetry. cca-zoo has an optional probabilistic feature that you can enable with the [probabilistic] suffix.
 
 To install cca-zoo with pip, run one of the following commands in your terminal:
 
 ```bash
```

