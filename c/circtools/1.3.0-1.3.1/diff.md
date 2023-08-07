# Comparing `tmp/circtools-1.3.0.tar.gz` & `tmp/circtools-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/circtools-1.3.0.tar", last modified: Tue May 23 23:59:09 2023, max compression
+gzip compressed data, was "circtools-1.3.1.tar", last modified: Mon Aug  7 18:26:35 2023, max compression
```

## Comparing `circtools-1.3.0.tar` & `circtools-1.3.1.tar`

### file list

```diff
@@ -1,239 +1,239 @@
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    35147 2022-06-17 23:38:57.000000 circtools-1.3.0/LICENSE
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      196 2023-03-10 01:23:32.000000 circtools-1.3.0/MANIFEST.in
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9770 2023-05-23 23:59:09.000000 circtools-1.3.0/PKG-INFO
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     8830 2023-03-14 18:30:52.000000 circtools-1.3.0/README.rst
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2023-03-10 00:17:31.000000 circtools-1.3.0/circtools/__init__.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/circ_module/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/circ_module/__init__.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3183 2022-07-29 21:01:07.000000 circtools-1.3.0/circtools/circ_module/circ_template.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/circtest/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/circtest/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6214 2023-03-21 00:23:22.000000 circtools-1.3.0/circtools/circtest/circtest.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    49652 2023-05-23 21:41:07.000000 circtools-1.3.0/circtools/circtools.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/circtest/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       28 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/contrib/circtest/.Rbuildignore
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      569 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/contrib/circtest/.gitignore
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      478 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/DESCRIPTION
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      151 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/NAMESPACE
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/circtest/R/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2500 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/Circ.filter.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6106 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/Circ.linePlot.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7248 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/Circ.ratioplot.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5286 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/Circ.test.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4428 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/HostGeneCount.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4296 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/documentData.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1696 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/summarySE.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6938 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/README.md
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/circtest/data/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3611 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/data/Circ.rda
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3031 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/data/Coordinates.rda
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4386 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/data/Linear.rda
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/circtest/man/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1972 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1442 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.filter.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1925 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.lineplot.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1813 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.ratioplot.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1427 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.test.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      549 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Coordinates.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      903 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/HostGeneCount.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1958 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Linear.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      717 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/read_one_scanBam.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      762 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/read_scanBam.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      266 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/summarySE.Rd
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      112 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/.Rbuildignore
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1387 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/CONDUCT.md
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      846 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/DESCRIPTION
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    34904 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/LICENSE
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      410 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/NAMESPACE
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       19 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/NEWS.md
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/R/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      143 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/data.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     8497 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/design.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3590 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/plotting.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3535 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/select.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1888 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/settings.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2708 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/transform.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      442 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/utils.R
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1596 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/README.Rmd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3215 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/README.md
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       43 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/_pkgdown.yml
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    38348 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/LICENSE.html
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    26375 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage.html
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/figure-html/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)   160986 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-10-1.png
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)   119338 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-7-1.png
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3572 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/index.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3492 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/authors.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9664 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/index.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2798 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/jquery.sticky-kit.min.js
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      810 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/link.svg
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/news/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3803 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/news/index.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2828 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/pkgdown.css
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1085 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/pkgdown.js
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4619 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/addSeq.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7074 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/bcl6exons.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9876 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/design.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5976 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/diagnose.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4262 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/extractExonPairs.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7328 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/index.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4606 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/p3Settings.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3684 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/p3Version.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4088 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/plotSegments.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    11416 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/primerSize.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    11461 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/primerTm.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4391 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/primersToList.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    10879 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/productSize.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3819 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/reexports.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4797 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/runPrimer3.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4613 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/selectPairs.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5918 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/seqSettings.html
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4439 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/toGRanges.html
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/inst/
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      373 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/dangle.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      548 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/dangle.ds
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      994 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1017 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1856 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      699 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2667 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2592 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2751 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2643 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      815 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      873 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      194 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/triloop_i.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      160 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/triloop_i.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2486 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2720 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2135 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2463 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2135 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2494 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      441 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/loops.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      692 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/loops.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1057 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stack.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1056 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stack.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1144 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1109 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      913 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      824 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      192 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/triloop.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      128 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/triloop.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      890 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      950 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.dh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1184 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.ds
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1152 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack_tm_inf.ds
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)   312896 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_core_Darwin_64
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)   239308 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_core_Linux_32
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)   994360 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_core_Linux_64
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3331 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_v1_1_4_default_settings.txt
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/man/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      600 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/addSeq.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      350 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/bcl6exons.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1163 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/design.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      662 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/diagnose.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      345 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/extractExonPairs.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      503 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/p3Settings.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      207 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/p3Version.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      298 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/plotSegments.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      605 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/primerSize.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      638 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/primerTm.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      435 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/primersToList.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      492 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/productSize.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      397 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/reexports.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      582 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/runPrimer3.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      528 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/selectPairs.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1163 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/seqSettings.Rd
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      404 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/toGRanges.Rd
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/vignettes/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6488 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/vignettes/Usage.Rmd
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/detect/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    20587 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/Circ_nonCirc_Exon_Match.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7245 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/CombineCounts.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5230 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/IntervalTree.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/__init__.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     8673 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/circAnnotate.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5913 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/circFilter.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    39917 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/detect.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    11374 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/findcircRNA.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5745 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/fix2chimera.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    13103 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/genecount.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/enrichment/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/enrichment/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    56944 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/enrichment/enrichment_check.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/exon_usage/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/exon_usage/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5907 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/exon_usage/exon_usage.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/primex/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/primex/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    27288 2023-03-21 01:10:49.000000 circtools-1.3.0/circtools/primex/primex.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/quickcheck/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/quickcheck/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5440 2023-03-21 00:50:01.000000 circtools-1.3.0/circtools/quickcheck/quickcheck.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/reconstruct/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/__init__.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7926 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/detect_skipped_exons.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6747 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/detect_splicing_variants.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5077 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/extract_reads.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    17026 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/get_coverage_profile.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6805 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/get_mate_information.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4147 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/get_readnames_from_DCC.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    27401 2023-03-21 20:18:54.000000 circtools-1.3.0/circtools/reconstruct/guided_denovo_circle_structure_parallel.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3771 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/permutate_motifs.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2622 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/proportion_of_fully_covered_circRNAs.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    18178 2023-03-21 18:20:04.000000 circtools-1.3.0/circtools/reconstruct/reconstruct.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2732 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/replace_ids_with_names.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     8423 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/write_fasta_for_fimo.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/scripts/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2023-03-10 00:17:31.000000 circtools-1.3.0/circtools/scripts/__init__.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      983 2023-03-10 01:50:40.000000 circtools-1.3.0/circtools/scripts/bash_runner.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6910 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_circtest_wrapper.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    22665 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_enrich_visualization.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    21557 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_exon_wrapper.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5214 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_generate_flanking_introns.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1595 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_generate_intron_gtf.sh
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1019 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_merge_enrich_results.sh
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     8398 2023-03-20 04:04:13.000000 circtools-1.3.0/circtools/scripts/circtools_primex_formatter.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5071 2023-03-06 20:37:07.000000 circtools-1.3.0/circtools/scripts/circtools_primex_wrapper.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    15182 2023-03-20 03:02:00.000000 circtools-1.3.0/circtools/scripts/circtools_quickcheck_wrapper.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1488 2023-03-21 18:36:38.000000 circtools-1.3.0/circtools/scripts/circtools_reconstruct_coverage_graph.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     8495 2023-03-21 18:36:39.000000 circtools-1.3.0/circtools/scripts/circtools_reconstruct_summarized_coverage_profiles.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     2225 2023-03-21 18:13:25.000000 circtools-1.3.0/circtools/scripts/circtools_reconstruct_summary_graphs.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    12125 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_reconstruct_visualization.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    10905 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/scripts/circtools_sirna_formatter.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     8784 2023-03-10 00:30:08.000000 circtools-1.3.0/circtools/scripts/create_igv_script.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6813 2023-03-10 00:32:59.000000 circtools-1.3.0/circtools/scripts/create_igv_script_from_gene_names.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     7098 2023-03-10 00:32:59.000000 circtools-1.3.0/circtools/scripts/create_igv_script_from_position_list.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    11775 2023-03-10 00:33:48.000000 circtools-1.3.0/circtools/scripts/detect_new_exons_from_fuchs_data.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     3722 2023-03-21 18:15:46.000000 circtools-1.3.0/circtools/scripts/install_R_dependencies.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1066 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/install_add_to_bashrc.sh
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)      922 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/install_create_r_environ.sh
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1451 2023-03-14 19:06:55.000000 circtools-1.3.0/circtools/scripts/install_external.sh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2907 2023-03-21 18:22:31.000000 circtools-1.3.0/circtools/scripts/r_runner.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1203 2023-03-19 02:39:54.000000 circtools-1.3.0/circtools/scripts/wonderdump
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/sirna/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/sirna/__init__.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    40141 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/sirna/sirna.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9770 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/PKG-INFO
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9826 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/SOURCES.txt
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        1 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/dependency_links.txt
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1552 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/entry_points.txt
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        1 2022-08-03 17:38:24.000000 circtools-1.3.0/circtools.egg-info/not-zip-safe
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      150 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/requires.txt
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       10 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/top_level.txt
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       94 2023-03-10 18:13:54.000000 circtools-1.3.0/pyproject.toml
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2830 2023-05-23 23:59:09.000000 circtools-1.3.0/setup.cfg
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)       69 2023-02-13 23:45:49.000000 circtools-1.3.0/setup.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.083248 circtools-1.3.1/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    35147 2022-06-17 23:38:57.000000 circtools-1.3.1/LICENSE
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      196 2023-03-10 01:23:32.000000 circtools-1.3.1/MANIFEST.in
+-rw-rw-r--   0 tjakobi   (1001) tjakobi   (1001)    11195 2023-08-07 18:26:35.083248 circtools-1.3.1/PKG-INFO
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     8832 2023-05-24 00:12:15.000000 circtools-1.3.1/README.rst
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.055248 circtools-1.3.1/circtools/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2023-03-10 00:17:31.000000 circtools-1.3.1/circtools/__init__.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.059248 circtools-1.3.1/circtools/circ_module/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/circ_module/__init__.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3183 2022-07-29 21:01:07.000000 circtools-1.3.1/circtools/circ_module/circ_template.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.059248 circtools-1.3.1/circtools/circtest/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/circtest/__init__.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     6214 2023-03-21 00:23:22.000000 circtools-1.3.1/circtools/circtest/circtest.py
+-rw-rw-r--   0 tjakobi   (1001) tjakobi   (1001)    49652 2023-08-07 18:24:52.000000 circtools-1.3.1/circtools/circtools.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.055248 circtools-1.3.1/circtools/contrib/
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.059248 circtools-1.3.1/circtools/contrib/circtest/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)       28 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/contrib/circtest/.Rbuildignore
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      569 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/contrib/circtest/.gitignore
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      478 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/DESCRIPTION
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      151 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/NAMESPACE
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.059248 circtools-1.3.1/circtools/contrib/circtest/R/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2500 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/R/Circ.filter.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     6106 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/R/Circ.linePlot.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     7248 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/R/Circ.ratioplot.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     5286 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/R/Circ.test.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4428 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/R/HostGeneCount.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4296 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/R/documentData.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1696 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/R/summarySE.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     6938 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/README.md
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.059248 circtools-1.3.1/circtools/contrib/circtest/data/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3611 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/data/Circ.rda
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3031 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/data/Coordinates.rda
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4386 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/data/Linear.rda
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.059248 circtools-1.3.1/circtools/contrib/circtest/man/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1972 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/Circ.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1442 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/Circ.filter.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1925 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/Circ.lineplot.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1813 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/Circ.ratioplot.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1427 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/Circ.test.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      549 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/Coordinates.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      903 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/HostGeneCount.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1958 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/Linear.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      717 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/read_one_scanBam.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      762 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/read_scanBam.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      266 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/circtest/man/summarySE.Rd
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.063248 circtools-1.3.1/circtools/contrib/primex/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      112 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/.Rbuildignore
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1387 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/CONDUCT.md
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      846 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/DESCRIPTION
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    34904 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/LICENSE
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      410 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/NAMESPACE
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)       19 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/NEWS.md
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.063248 circtools-1.3.1/circtools/contrib/primex/R/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      143 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/R/data.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     8497 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/R/design.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3590 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/R/plotting.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3535 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/R/select.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1888 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/R/settings.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2708 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/R/transform.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      442 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/R/utils.R
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1596 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/README.Rmd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3215 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/README.md
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)       43 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/_pkgdown.yml
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.063248 circtools-1.3.1/circtools/contrib/primex/docs/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    38348 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/LICENSE.html
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.063248 circtools-1.3.1/circtools/contrib/primex/docs/articles/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    26375 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/articles/Usage.html
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.055248 circtools-1.3.1/circtools/contrib/primex/docs/articles/Usage_files/
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.063248 circtools-1.3.1/circtools/contrib/primex/docs/articles/Usage_files/figure-html/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)   160986 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-10-1.png
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)   119338 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-7-1.png
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3572 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/articles/index.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3492 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/authors.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     9664 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/index.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2798 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/jquery.sticky-kit.min.js
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      810 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/link.svg
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.063248 circtools-1.3.1/circtools/contrib/primex/docs/news/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3803 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/news/index.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2828 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/pkgdown.css
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1085 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/pkgdown.js
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.067248 circtools-1.3.1/circtools/contrib/primex/docs/reference/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4619 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/addSeq.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     7074 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/bcl6exons.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     9876 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/design.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     5976 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/diagnose.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4262 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/extractExonPairs.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     7328 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/index.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4606 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/p3Settings.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3684 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/p3Version.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4088 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/plotSegments.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    11416 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/primerSize.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    11461 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/primerTm.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4391 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/primersToList.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    10879 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/productSize.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3819 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/reexports.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4797 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/runPrimer3.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4613 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/selectPairs.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     5918 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/seqSettings.html
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4439 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/docs/reference/toGRanges.html
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.055248 circtools-1.3.1/circtools/contrib/primex/inst/
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.071248 circtools-1.3.1/circtools/contrib/primex/inst/primer3/
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.071248 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      373 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/dangle.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      548 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/dangle.ds
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.075248 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      994 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1017 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1856 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      699 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2667 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2592 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2751 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2643 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      815 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      873 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      194 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/triloop_i.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      160 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/triloop_i.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2486 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2720 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2135 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2463 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2135 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2494 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      441 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/loops.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      692 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/loops.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1057 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/stack.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1056 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/stack.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1144 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1109 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      913 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      824 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      192 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/triloop.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      128 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/triloop.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      890 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tstack.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      950 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.dh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1184 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.ds
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1152 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tstack_tm_inf.ds
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)   312896 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_core_Darwin_64
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)   239308 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_core_Linux_32
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)   994360 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_core_Linux_64
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3331 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_v1_1_4_default_settings.txt
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.075248 circtools-1.3.1/circtools/contrib/primex/man/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      600 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/addSeq.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      350 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/bcl6exons.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1163 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/design.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      662 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/diagnose.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      345 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/extractExonPairs.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      503 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/p3Settings.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      207 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/p3Version.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      298 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/plotSegments.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      605 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/primerSize.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      638 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/primerTm.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      435 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/primersToList.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      492 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/productSize.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      397 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/reexports.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      582 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/runPrimer3.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      528 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/selectPairs.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1163 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/seqSettings.Rd
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      404 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/man/toGRanges.Rd
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.075248 circtools-1.3.1/circtools/contrib/primex/vignettes/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     6488 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/contrib/primex/vignettes/Usage.Rmd
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.079248 circtools-1.3.1/circtools/detect/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    20587 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/Circ_nonCirc_Exon_Match.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     7245 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/CombineCounts.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     5230 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/IntervalTree.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/__init__.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     8673 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/circAnnotate.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     5913 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/circFilter.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    39917 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/detect.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    11374 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/findcircRNA.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     5745 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/fix2chimera.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    13103 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/detect/genecount.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.079248 circtools-1.3.1/circtools/enrichment/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/enrichment/__init__.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)    56944 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/enrichment/enrichment_check.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.079248 circtools-1.3.1/circtools/exon_usage/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/exon_usage/__init__.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     5907 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/exon_usage/exon_usage.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.079248 circtools-1.3.1/circtools/primex/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/primex/__init__.py
+-rwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)    27288 2023-08-07 18:24:47.000000 circtools-1.3.1/circtools/primex/primex.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.079248 circtools-1.3.1/circtools/quickcheck/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/quickcheck/__init__.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     5440 2023-03-21 00:50:01.000000 circtools-1.3.1/circtools/quickcheck/quickcheck.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.079248 circtools-1.3.1/circtools/reconstruct/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/__init__.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     7926 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/detect_skipped_exons.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     6747 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/detect_splicing_variants.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     5077 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/extract_reads.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    17026 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/get_coverage_profile.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     6805 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/get_mate_information.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     4147 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/get_readnames_from_DCC.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    27401 2023-03-21 20:18:54.000000 circtools-1.3.1/circtools/reconstruct/guided_denovo_circle_structure_parallel.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     3771 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/permutate_motifs.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2622 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/proportion_of_fully_covered_circRNAs.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)    18178 2023-03-21 18:20:04.000000 circtools-1.3.1/circtools/reconstruct/reconstruct.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2732 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/replace_ids_with_names.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     8423 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/reconstruct/write_fasta_for_fimo.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.083248 circtools-1.3.1/circtools/scripts/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2023-03-10 00:17:31.000000 circtools-1.3.1/circtools/scripts/__init__.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      983 2023-03-10 01:50:40.000000 circtools-1.3.1/circtools/scripts/bash_runner.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     6910 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/scripts/circtools_circtest_wrapper.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)    22665 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/scripts/circtools_enrich_visualization.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)    21557 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/scripts/circtools_exon_wrapper.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     5214 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/scripts/circtools_generate_flanking_introns.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     1595 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/scripts/circtools_generate_intron_gtf.sh
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     1019 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/scripts/circtools_merge_enrich_results.sh
+-rwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)     8398 2023-08-07 18:24:47.000000 circtools-1.3.1/circtools/scripts/circtools_primex_formatter.R
+-rwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)     5071 2023-08-07 18:24:47.000000 circtools-1.3.1/circtools/scripts/circtools_primex_wrapper.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)    15182 2023-03-20 03:02:00.000000 circtools-1.3.1/circtools/scripts/circtools_quickcheck_wrapper.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     1488 2023-03-21 18:36:38.000000 circtools-1.3.1/circtools/scripts/circtools_reconstruct_coverage_graph.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     8495 2023-03-21 18:36:39.000000 circtools-1.3.1/circtools/scripts/circtools_reconstruct_summarized_coverage_profiles.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     2225 2023-03-21 18:13:25.000000 circtools-1.3.1/circtools/scripts/circtools_reconstruct_summary_graphs.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)    12125 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/scripts/circtools_reconstruct_visualization.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)    10905 2023-03-06 20:38:19.000000 circtools-1.3.1/circtools/scripts/circtools_sirna_formatter.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     8784 2023-03-10 00:30:08.000000 circtools-1.3.1/circtools/scripts/create_igv_script.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     6813 2023-03-10 00:32:59.000000 circtools-1.3.1/circtools/scripts/create_igv_script_from_gene_names.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     7098 2023-03-10 00:32:59.000000 circtools-1.3.1/circtools/scripts/create_igv_script_from_position_list.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)    11775 2023-03-10 00:33:48.000000 circtools-1.3.1/circtools/scripts/detect_new_exons_from_fuchs_data.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     2846 2023-08-01 23:28:15.000000 circtools-1.3.1/circtools/scripts/install_R_dependencies.R
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     1066 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/scripts/install_add_to_bashrc.sh
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)      922 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/scripts/install_create_r_environ.sh
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     1451 2023-03-14 19:06:55.000000 circtools-1.3.1/circtools/scripts/install_external.sh
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     2907 2023-03-21 18:22:31.000000 circtools-1.3.1/circtools/scripts/r_runner.py
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)     1203 2023-03-19 02:39:54.000000 circtools-1.3.1/circtools/scripts/wonderdump
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.083248 circtools-1.3.1/circtools/sirna/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        0 2022-06-17 23:38:57.000000 circtools-1.3.1/circtools/sirna/__init__.py
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    40141 2023-03-06 20:38:18.000000 circtools-1.3.1/circtools/sirna/sirna.py
+drwxrwxr-x   0 tjakobi   (1001) tjakobi   (1001)        0 2023-08-07 18:26:35.059248 circtools-1.3.1/circtools.egg-info/
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)    11195 2023-08-07 18:26:35.000000 circtools-1.3.1/circtools.egg-info/PKG-INFO
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     9826 2023-08-07 18:26:35.000000 circtools-1.3.1/circtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        1 2023-08-07 18:26:35.000000 circtools-1.3.1/circtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)     1553 2023-08-07 18:26:35.000000 circtools-1.3.1/circtools.egg-info/entry_points.txt
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)        1 2022-08-03 17:38:24.000000 circtools-1.3.1/circtools.egg-info/not-zip-safe
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)      150 2023-08-07 18:26:35.000000 circtools-1.3.1/circtools.egg-info/requires.txt
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)       10 2023-08-07 18:26:35.000000 circtools-1.3.1/circtools.egg-info/top_level.txt
+-rw-r--r--   0 tjakobi   (1001) tjakobi   (1001)       94 2023-03-10 18:13:54.000000 circtools-1.3.1/pyproject.toml
+-rw-rw-r--   0 tjakobi   (1001) tjakobi   (1001)     2830 2023-08-07 18:26:35.083248 circtools-1.3.1/setup.cfg
+-rwxr-xr-x   0 tjakobi   (1001) tjakobi   (1001)       69 2023-02-13 23:45:49.000000 circtools-1.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `circtools-1.3.0/LICENSE` & `circtools-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/PKG-INFO` & `circtools-1.3.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: circtools
-Version: 1.3.0
-Summary: circtools - a circular RNA toolbox
-Home-page: https://github.com/jakobilab/circtools
-Author: Tobias Jakobi
-Author-email: tjakobi@arizona.edu
-License: GNU General Public License (GPL)
-Project-URL: Bug Reports, https://github.com/jakobilab/circtools/issues
-Project-URL: Jakobi Lab, https://jakobilab.org
-Project-URL: Source, https://github.com/jakobilab/circtools
-Project-URL: Documentation, https://docs.circ.tools
-Keywords: circRNA,circular RNA bioinformatics
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-
 **circtools**
 ======================================================================
 
 **a one-stop software solution for circular RNA research**
 
 .. figure:: https://raw.githubusercontent.com/jakobilab/circtools/master/docs/img/circtools_200px.png
    :alt: circtools
@@ -177,18 +154,18 @@
     :target: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml
 
 .. |docker| image:: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml/badge.svg?branch=master
     :alt: Docker Build
     :scale: 100%
     :target: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml
 
-.. |zenodo| image:: https://zenodo.org/badge/83248654.svg
+.. |zenodo| image:: https://zenodo.org/badge/498448368.svg
     :alt: Zenodo DOI link
     :scale: 100%
-    :target: https://zenodo.org/badge/latestdoi/83248654
+    :target: https://zenodo.org/badge/latestdoi/498448368
 
 .. |downloads| image:: https://pepy.tech/badge/circtools
     :alt: Python Package Index Downloads
     :scale: 100%
     :target: https://pepy.tech/project/circtools
 
 .. |pypi| image:: https://badge.fury.io/py/circtools.svg
```

### Comparing `circtools-1.3.0/README.rst` & `circtools-1.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,174 +1,198 @@
-**circtools**
-======================================================================
-
-**a one-stop software solution for circular RNA research**
-
-.. figure:: https://raw.githubusercontent.com/jakobilab/circtools/master/docs/img/circtools_200px.png
-   :alt: circtools
-
-|docs| |build| |docker| |zenodo| |downloads| |pypi|
-
-Introduction
--------------
-
-Circular RNAs (circRNAs) originate through back-splicing events from linear primary transcripts, are resistant to exonucleases, typically not polyadenylated, and have been shown to be highly specific for cell type and developmental stage. Although few circular RNA molecules have been shown to exhibit miRNA sponge function, for the vast majority of circRNAs however, their function is yet to be determined.
-
-The prediction of circular RNAs is a multi-stage bioinformatics process starting with raw sequencing data and usually ending with a list of potential circRNA candidates which, depending on tissue and condition may contain hundreds to thousands of potential circRNAs. While there already exist a number of tools for the prediction process (e.g. `DCC <https://github.com/dieterich-lab/DCC>`__ and `CircTest <https://github.com/dieterich-lab/CircTest>`__), publicly available downstream analysis tools are rare.
-
-We developed **circtools**, a modular, Python3-based framework for circRNA-related tools that unifies several functionalities in single command line driven software. The command line follows the `circtools subcommand` standard that is employed in samtools or bedtools. Currently, circtools includes modules for detecting and reconstructing circRNAs,
-a quick check of circRNA mapping results, RBP enrichment screenings, circRNA primer design, statistical testing, and an exon usage module.
-
-
-
-Documentation
--------------
-
-Click `here <https://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
-
-Installation
-------------
-
-The ``circtools`` package is written in Python 3 (supporting Python 3.7 - 3.10). It requires only a small number of external dependencies, namely standard bioinformatics tools:
-
--  `bedtools (>= 2.27.1) <https://bedtools.readthedocs.io/en/latest/content/installation.html>`__
-   [RBP enrichment module, installed automatically]
--  `R (>= 4.0) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-22-04>`__
-   [Data visualization and data processing]
-
-Installation is managed through ``pip3 install circtools`` or ``python3 setup.py
-install`` when installed from the cloned GitHub repository. No sudo access is
-required if the installation is executed with ``--user`` which will install the
-package in a user-writeable folder. The binaries should be installed
-to ``/home/$user/.local/bin/`` in case of Debian-based systems.
-
-``circtools`` was developed and tested on Debian Buster, but should also
-run with any other distribution.
-
-The installation can be performed directly from Pypi:
-
-.. code-block:: console
-
-    # install circtools
-    pip install numpy # required for HTSeq, a dependency of circtools
-    pip install circtools
-
-    # install R packages for circtools
-    circtools_install_R_dependencies
-
-Additionally, this repository offers the latest development version:
-
-.. code-block:: console
-
-    pip install numpy # required for HTSeq, a dependency of circtools
-    pip install git+https://github.com/jakobilab/circtools.git
-
-The primer-design module as well as the exon analysis and circRNA testing module
-require a working installation of `R <https://cran.r-project.org/>`__ with
-`BioConductor <https://www.bioconductor.org/install/>`__. All R packages
-required can be automatically installed during the setup. Please see the
-`"Installing circtools" <http://docs.circ.tools/en/latest/Installation.html>`__
-chapter of the main circtools documentation for more detailed installation instructions.
-
-Modules
--------
-
-Circtools currently offers seven modules:
-
-detect `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Detect.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``detect`` command is an interface to
-`DCC <https://github.com/dieterich-lab/DCC>`__, developed at the
-Dieterich Lab. The module allows to detect circRNAs from RNA sequencing
-data. The module is the foundation of all other steps for the circtools
-work flow. All parameters supplied to circtools will be directly passed
-to DCC.
-
-quickcheck `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Quickcheck.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The quickcheck module of circtools is an easy way to check the results
-of a DCC run for problems and to quickly assess the number of circRNAs
-in a given experiment. The module needs the mapping log files produced
-by STAR as well as the directory with the DCC results. The module than
-generates a series of figures in PDF format to assess the results.
-
-reconstruct `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Reconstruct.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``reconstruct`` command is an interface to
-`FUCHS <https://github.com/dieterich-lab/FUCHS>`__. FUCHS is employing
-DCC-generated data to reconstruct circRNA structures. All parameters
-supplied to circtools will be directly passed to FUCHS.
-
-circtest `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Circtest.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``circtest`` command is an interface to
-`CircTest <https://github.com/dieterich-lab/CircTest>`__. The module a a
-very convenient way to employ statistical testing to circRNA candidates
-generated with DCC without having to write an R script for each new
-experiment. For detailed information on the implementation itself take a
-look at the `CircTest
-documentation <https://github.com/dieterich-lab/CircTest>`__. In
-essence, the module allows dynamic grouping of the columns (samples) in
-the DCC data.
-
-exon `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Exon.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The exon module of circtools employs the `ballgown R
-package <https://www.bioconductor.org/packages/release/bioc/html/ballgown.html>`__
-to combine data generated with DCC and circtest with ballgown-compatible
-``stringtie`` output or cufflinks output converted via
-`tablemaker <https://github.com/leekgroup/tablemaker>`__ in order get
-deeper insights into differential exon usage within circRNA candidates.
-
-enrich `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Enrichment.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``enrichment`` module may be used to identify circRNAs enriched for
-specific RNA binding proteins (RBP) based on DCC-identified circRNAs and
-processed
-`eCLIP <http://www.nature.com/nmeth/journal/v13/n6/full/nmeth.3810.html>`__
-data. For K526 and HepG2 cell lines plenty of this data is available
-through the
-`ENCODE <https://www.encodeproject.org/search/?type=Experiment&assay_title=eCLIP>`__
-project.
-
-primer `(detailed documentation) <https://circtools.readthedocs.io/en/latest/primer.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``primer`` command is used to design and visualize primers required
-for follow up wet lab experiments to verify circRNA candidates.
-
-
-.. |docs| image:: https://readthedocs.org/projects/circtools/badge/?version=latest
-    :alt: Documentation Status
-    :scale: 100%
-    :target: https://circtools.readthedocs.io/en/latest/?badge=latest
-
-.. |build| image:: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml/badge.svg?branch=master
-    :alt: CI Status
-    :scale: 100%
-    :target: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml
-
-.. |docker| image:: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml/badge.svg?branch=master
-    :alt: Docker Build
-    :scale: 100%
-    :target: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml
-
-.. |zenodo| image:: https://zenodo.org/badge/83248654.svg
-    :alt: Zenodo DOI link
-    :scale: 100%
-    :target: https://zenodo.org/badge/latestdoi/83248654
-
-.. |downloads| image:: https://pepy.tech/badge/circtools
-    :alt: Python Package Index Downloads
-    :scale: 100%
-    :target: https://pepy.tech/project/circtools
-
-.. |pypi| image:: https://badge.fury.io/py/circtools.svg
-    :alt: Python package version
-    :scale: 100%
-    :target: https://badge.fury.io/py/circtools
+Metadata-Version: 2.1
+Name: circtools
+Version: 1.3.1
+Summary: circtools - a circular RNA toolbox
+Home-page: https://github.com/jakobilab/circtools
+Author: Tobias Jakobi
+Author-email: tjakobi@arizona.edu
+License: GNU General Public License (GPL)
+Project-URL: Bug Reports, https://github.com/jakobilab/circtools/issues
+Project-URL: Jakobi Lab, https://jakobilab.org
+Project-URL: Source, https://github.com/jakobilab/circtools
+Project-URL: Documentation, https://docs.circ.tools
+Description: **circtools**
+        ======================================================================
+        
+        **a one-stop software solution for circular RNA research**
+        
+        .. figure:: https://raw.githubusercontent.com/jakobilab/circtools/master/docs/img/circtools_200px.png
+           :alt: circtools
+        
+        |docs| |build| |docker| |zenodo| |downloads| |pypi|
+        
+        Introduction
+        -------------
+        
+        Circular RNAs (circRNAs) originate through back-splicing events from linear primary transcripts, are resistant to exonucleases, typically not polyadenylated, and have been shown to be highly specific for cell type and developmental stage. Although few circular RNA molecules have been shown to exhibit miRNA sponge function, for the vast majority of circRNAs however, their function is yet to be determined.
+        
+        The prediction of circular RNAs is a multi-stage bioinformatics process starting with raw sequencing data and usually ending with a list of potential circRNA candidates which, depending on tissue and condition may contain hundreds to thousands of potential circRNAs. While there already exist a number of tools for the prediction process (e.g. `DCC <https://github.com/dieterich-lab/DCC>`__ and `CircTest <https://github.com/dieterich-lab/CircTest>`__), publicly available downstream analysis tools are rare.
+        
+        We developed **circtools**, a modular, Python3-based framework for circRNA-related tools that unifies several functionalities in single command line driven software. The command line follows the `circtools subcommand` standard that is employed in samtools or bedtools. Currently, circtools includes modules for detecting and reconstructing circRNAs,
+        a quick check of circRNA mapping results, RBP enrichment screenings, circRNA primer design, statistical testing, and an exon usage module.
+        
+        
+        
+        Documentation
+        -------------
+        
+        Click `here <https://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
+        
+        Installation
+        ------------
+        
+        The ``circtools`` package is written in Python 3 (supporting Python 3.7 - 3.10). It requires only a small number of external dependencies, namely standard bioinformatics tools:
+        
+        -  `bedtools (>= 2.27.1) <https://bedtools.readthedocs.io/en/latest/content/installation.html>`__
+           [RBP enrichment module, installed automatically]
+        -  `R (>= 4.0) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-22-04>`__
+           [Data visualization and data processing]
+        
+        Installation is managed through ``pip3 install circtools`` or ``python3 setup.py
+        install`` when installed from the cloned GitHub repository. No sudo access is
+        required if the installation is executed with ``--user`` which will install the
+        package in a user-writeable folder. The binaries should be installed
+        to ``/home/$user/.local/bin/`` in case of Debian-based systems.
+        
+        ``circtools`` was developed and tested on Debian Buster, but should also
+        run with any other distribution.
+        
+        The installation can be performed directly from Pypi:
+        
+        .. code-block:: console
+        
+            # install circtools
+            pip install numpy # required for HTSeq, a dependency of circtools
+            pip install circtools
+        
+            # install R packages for circtools
+            circtools_install_R_dependencies
+        
+        Additionally, this repository offers the latest development version:
+        
+        .. code-block:: console
+        
+            pip install numpy # required for HTSeq, a dependency of circtools
+            pip install git+https://github.com/jakobilab/circtools.git
+        
+        The primer-design module as well as the exon analysis and circRNA testing module
+        require a working installation of `R <https://cran.r-project.org/>`__ with
+        `BioConductor <https://www.bioconductor.org/install/>`__. All R packages
+        required can be automatically installed during the setup. Please see the
+        `"Installing circtools" <http://docs.circ.tools/en/latest/Installation.html>`__
+        chapter of the main circtools documentation for more detailed installation instructions.
+        
+        Modules
+        -------
+        
+        Circtools currently offers seven modules:
+        
+        detect `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Detect.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``detect`` command is an interface to
+        `DCC <https://github.com/dieterich-lab/DCC>`__, developed at the
+        Dieterich Lab. The module allows to detect circRNAs from RNA sequencing
+        data. The module is the foundation of all other steps for the circtools
+        work flow. All parameters supplied to circtools will be directly passed
+        to DCC.
+        
+        quickcheck `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Quickcheck.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The quickcheck module of circtools is an easy way to check the results
+        of a DCC run for problems and to quickly assess the number of circRNAs
+        in a given experiment. The module needs the mapping log files produced
+        by STAR as well as the directory with the DCC results. The module than
+        generates a series of figures in PDF format to assess the results.
+        
+        reconstruct `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Reconstruct.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``reconstruct`` command is an interface to
+        `FUCHS <https://github.com/dieterich-lab/FUCHS>`__. FUCHS is employing
+        DCC-generated data to reconstruct circRNA structures. All parameters
+        supplied to circtools will be directly passed to FUCHS.
+        
+        circtest `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Circtest.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``circtest`` command is an interface to
+        `CircTest <https://github.com/dieterich-lab/CircTest>`__. The module a a
+        very convenient way to employ statistical testing to circRNA candidates
+        generated with DCC without having to write an R script for each new
+        experiment. For detailed information on the implementation itself take a
+        look at the `CircTest
+        documentation <https://github.com/dieterich-lab/CircTest>`__. In
+        essence, the module allows dynamic grouping of the columns (samples) in
+        the DCC data.
+        
+        exon `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Exon.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The exon module of circtools employs the `ballgown R
+        package <https://www.bioconductor.org/packages/release/bioc/html/ballgown.html>`__
+        to combine data generated with DCC and circtest with ballgown-compatible
+        ``stringtie`` output or cufflinks output converted via
+        `tablemaker <https://github.com/leekgroup/tablemaker>`__ in order get
+        deeper insights into differential exon usage within circRNA candidates.
+        
+        enrich `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Enrichment.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``enrichment`` module may be used to identify circRNAs enriched for
+        specific RNA binding proteins (RBP) based on DCC-identified circRNAs and
+        processed
+        `eCLIP <http://www.nature.com/nmeth/journal/v13/n6/full/nmeth.3810.html>`__
+        data. For K526 and HepG2 cell lines plenty of this data is available
+        through the
+        `ENCODE <https://www.encodeproject.org/search/?type=Experiment&assay_title=eCLIP>`__
+        project.
+        
+        primer `(detailed documentation) <https://circtools.readthedocs.io/en/latest/primer.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``primer`` command is used to design and visualize primers required
+        for follow up wet lab experiments to verify circRNA candidates.
+        
+        
+        .. |docs| image:: https://readthedocs.org/projects/circtools/badge/?version=latest
+            :alt: Documentation Status
+            :scale: 100%
+            :target: https://circtools.readthedocs.io/en/latest/?badge=latest
+        
+        .. |build| image:: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml/badge.svg?branch=master
+            :alt: CI Status
+            :scale: 100%
+            :target: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml
+        
+        .. |docker| image:: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml/badge.svg?branch=master
+            :alt: Docker Build
+            :scale: 100%
+            :target: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml
+        
+        .. |zenodo| image:: https://zenodo.org/badge/498448368.svg
+            :alt: Zenodo DOI link
+            :scale: 100%
+            :target: https://zenodo.org/badge/latestdoi/498448368
+        
+        .. |downloads| image:: https://pepy.tech/badge/circtools
+            :alt: Python Package Index Downloads
+            :scale: 100%
+            :target: https://pepy.tech/project/circtools
+        
+        .. |pypi| image:: https://badge.fury.io/py/circtools.svg
+            :alt: Python package version
+            :scale: 100%
+            :target: https://badge.fury.io/py/circtools
+        
+Keywords: circRNA,circular RNA bioinformatics
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
```

### Comparing `circtools-1.3.0/circtools/circ_module/circ_template.py` & `circtools-1.3.1/circtools/circ_module/circ_template.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/circtest/circtest.py` & `circtools-1.3.1/circtools/circtest/circtest.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/circtools.py` & `circtools-1.3.1/circtools/circtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
 import os.path
 import sys
 
 # global settings
-version = "1.3.0"
+version = "1.3.1"
 program_name = "circtools"
 
 
 # samtools/git like parsing from http://chase-seibert.github.io/blog/2014/03/21/python-multilevel-argparse.html
 
 
 def main():
```

### Comparing `circtools-1.3.0/circtools/contrib/circtest/.gitignore` & `circtools-1.3.1/circtools/contrib/circtest/.gitignore`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/R/Circ.filter.R` & `circtools-1.3.1/circtools/contrib/circtest/R/Circ.filter.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/R/Circ.linePlot.R` & `circtools-1.3.1/circtools/contrib/circtest/R/Circ.linePlot.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/R/Circ.ratioplot.R` & `circtools-1.3.1/circtools/contrib/circtest/R/Circ.ratioplot.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/R/Circ.test.R` & `circtools-1.3.1/circtools/contrib/circtest/R/Circ.test.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/R/HostGeneCount.R` & `circtools-1.3.1/circtools/contrib/circtest/R/HostGeneCount.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/R/documentData.R` & `circtools-1.3.1/circtools/contrib/circtest/R/documentData.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/R/summarySE.R` & `circtools-1.3.1/circtools/contrib/circtest/R/summarySE.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/README.md` & `circtools-1.3.1/circtools/contrib/circtest/README.md`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/data/Circ.rda` & `circtools-1.3.1/circtools/contrib/circtest/data/Circ.rda`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/data/Coordinates.rda` & `circtools-1.3.1/circtools/contrib/circtest/data/Coordinates.rda`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/data/Linear.rda` & `circtools-1.3.1/circtools/contrib/circtest/data/Linear.rda`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/Circ.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/Circ.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/Circ.filter.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/Circ.filter.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/Circ.lineplot.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/Circ.lineplot.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/Circ.ratioplot.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/Circ.ratioplot.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/Circ.test.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/Circ.test.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/Coordinates.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/Coordinates.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/HostGeneCount.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/HostGeneCount.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/Linear.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/Linear.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/read_one_scanBam.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/read_one_scanBam.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/circtest/man/read_scanBam.Rd` & `circtools-1.3.1/circtools/contrib/circtest/man/read_scanBam.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/CONDUCT.md` & `circtools-1.3.1/circtools/contrib/primex/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/DESCRIPTION` & `circtools-1.3.1/circtools/contrib/primex/DESCRIPTION`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/LICENSE` & `circtools-1.3.1/circtools/contrib/primex/LICENSE`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/R/design.R` & `circtools-1.3.1/circtools/contrib/primex/R/design.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/R/plotting.R` & `circtools-1.3.1/circtools/contrib/primex/R/plotting.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/R/select.R` & `circtools-1.3.1/circtools/contrib/primex/R/select.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/R/settings.R` & `circtools-1.3.1/circtools/contrib/primex/R/settings.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/R/transform.R` & `circtools-1.3.1/circtools/contrib/primex/R/transform.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/README.Rmd` & `circtools-1.3.1/circtools/contrib/primex/README.Rmd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/README.md` & `circtools-1.3.1/circtools/contrib/primex/README.md`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/LICENSE.html` & `circtools-1.3.1/circtools/contrib/primex/docs/LICENSE.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage.html` & `circtools-1.3.1/circtools/contrib/primex/docs/articles/Usage.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-10-1.png` & `circtools-1.3.1/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-10-1.png`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-7-1.png` & `circtools-1.3.1/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-7-1.png`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/articles/index.html` & `circtools-1.3.1/circtools/contrib/primex/docs/articles/index.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/authors.html` & `circtools-1.3.1/circtools/contrib/primex/docs/authors.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/index.html` & `circtools-1.3.1/circtools/contrib/primex/docs/index.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/jquery.sticky-kit.min.js` & `circtools-1.3.1/circtools/contrib/primex/docs/jquery.sticky-kit.min.js`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/link.svg` & `circtools-1.3.1/circtools/contrib/primex/docs/link.svg`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/news/index.html` & `circtools-1.3.1/circtools/contrib/primex/docs/news/index.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/pkgdown.css` & `circtools-1.3.1/circtools/contrib/primex/docs/pkgdown.css`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/pkgdown.js` & `circtools-1.3.1/circtools/contrib/primex/docs/pkgdown.js`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/addSeq.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/addSeq.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/bcl6exons.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/bcl6exons.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/design.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/design.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/diagnose.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/diagnose.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/extractExonPairs.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/extractExonPairs.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/index.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/index.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/p3Settings.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/p3Settings.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/p3Version.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/p3Version.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/plotSegments.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/plotSegments.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/primerSize.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/primerSize.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/primerTm.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/primerTm.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/primersToList.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/primersToList.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/productSize.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/productSize.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/reexports.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/reexports.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/runPrimer3.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/runPrimer3.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/selectPairs.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/selectPairs.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/seqSettings.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/seqSettings.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/docs/reference/toGRanges.html` & `circtools-1.3.1/circtools/contrib/primex/docs/reference/toGRanges.html`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/dangle.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/dangle.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/loops.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/loops.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stack.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/stack.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stack.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/stack.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tstack.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.dh` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.dh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack_tm_inf.ds` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_config/tstack_tm_inf.ds`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_core_Darwin_64` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_core_Darwin_64`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_core_Linux_32` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_core_Linux_32`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_core_Linux_64` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_core_Linux_64`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_v1_1_4_default_settings.txt` & `circtools-1.3.1/circtools/contrib/primex/inst/primer3/primer3_v1_1_4_default_settings.txt`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/man/addSeq.Rd` & `circtools-1.3.1/circtools/contrib/primex/man/addSeq.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/man/design.Rd` & `circtools-1.3.1/circtools/contrib/primex/man/design.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/man/diagnose.Rd` & `circtools-1.3.1/circtools/contrib/primex/man/diagnose.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/man/primerSize.Rd` & `circtools-1.3.1/circtools/contrib/primex/man/primerSize.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/man/primerTm.Rd` & `circtools-1.3.1/circtools/contrib/primex/man/primerTm.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/man/runPrimer3.Rd` & `circtools-1.3.1/circtools/contrib/primex/man/runPrimer3.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/man/selectPairs.Rd` & `circtools-1.3.1/circtools/contrib/primex/man/selectPairs.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/man/seqSettings.Rd` & `circtools-1.3.1/circtools/contrib/primex/man/seqSettings.Rd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/contrib/primex/vignettes/Usage.Rmd` & `circtools-1.3.1/circtools/contrib/primex/vignettes/Usage.Rmd`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/detect/Circ_nonCirc_Exon_Match.py` & `circtools-1.3.1/circtools/detect/Circ_nonCirc_Exon_Match.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/detect/CombineCounts.py` & `circtools-1.3.1/circtools/detect/CombineCounts.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/detect/IntervalTree.py` & `circtools-1.3.1/circtools/detect/IntervalTree.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/detect/circAnnotate.py` & `circtools-1.3.1/circtools/detect/circAnnotate.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/detect/circFilter.py` & `circtools-1.3.1/circtools/detect/circFilter.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/detect/detect.py` & `circtools-1.3.1/circtools/detect/detect.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/detect/findcircRNA.py` & `circtools-1.3.1/circtools/detect/findcircRNA.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/detect/fix2chimera.py` & `circtools-1.3.1/circtools/detect/fix2chimera.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/detect/genecount.py` & `circtools-1.3.1/circtools/detect/genecount.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/enrichment/enrichment_check.py` & `circtools-1.3.1/circtools/enrichment/enrichment_check.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/exon_usage/exon_usage.py` & `circtools-1.3.1/circtools/exon_usage/exon_usage.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/primex/primex.py` & `circtools-1.3.1/circtools/primex/primex.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/quickcheck/quickcheck.py` & `circtools-1.3.1/circtools/quickcheck/quickcheck.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/detect_skipped_exons.py` & `circtools-1.3.1/circtools/reconstruct/detect_skipped_exons.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/detect_splicing_variants.py` & `circtools-1.3.1/circtools/reconstruct/detect_splicing_variants.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/extract_reads.py` & `circtools-1.3.1/circtools/reconstruct/extract_reads.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/get_coverage_profile.py` & `circtools-1.3.1/circtools/reconstruct/get_coverage_profile.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/get_mate_information.py` & `circtools-1.3.1/circtools/reconstruct/get_mate_information.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/get_readnames_from_DCC.py` & `circtools-1.3.1/circtools/reconstruct/get_readnames_from_DCC.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/guided_denovo_circle_structure_parallel.py` & `circtools-1.3.1/circtools/reconstruct/guided_denovo_circle_structure_parallel.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/permutate_motifs.py` & `circtools-1.3.1/circtools/reconstruct/permutate_motifs.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/proportion_of_fully_covered_circRNAs.py` & `circtools-1.3.1/circtools/reconstruct/proportion_of_fully_covered_circRNAs.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/reconstruct.py` & `circtools-1.3.1/circtools/reconstruct/reconstruct.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/replace_ids_with_names.py` & `circtools-1.3.1/circtools/reconstruct/replace_ids_with_names.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/reconstruct/write_fasta_for_fimo.py` & `circtools-1.3.1/circtools/reconstruct/write_fasta_for_fimo.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/bash_runner.py` & `circtools-1.3.1/circtools/scripts/bash_runner.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_circtest_wrapper.R` & `circtools-1.3.1/circtools/scripts/circtools_circtest_wrapper.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_enrich_visualization.R` & `circtools-1.3.1/circtools/scripts/circtools_enrich_visualization.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_exon_wrapper.R` & `circtools-1.3.1/circtools/scripts/circtools_exon_wrapper.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_generate_flanking_introns.py` & `circtools-1.3.1/circtools/scripts/circtools_generate_flanking_introns.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_generate_intron_gtf.sh` & `circtools-1.3.1/circtools/scripts/circtools_generate_intron_gtf.sh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_merge_enrich_results.sh` & `circtools-1.3.1/circtools/scripts/circtools_merge_enrich_results.sh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_primex_formatter.R` & `circtools-1.3.1/circtools/scripts/circtools_primex_formatter.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_primex_wrapper.R` & `circtools-1.3.1/circtools/scripts/circtools_primex_wrapper.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_quickcheck_wrapper.R` & `circtools-1.3.1/circtools/scripts/circtools_quickcheck_wrapper.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_reconstruct_coverage_graph.R` & `circtools-1.3.1/circtools/scripts/circtools_reconstruct_coverage_graph.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_reconstruct_summarized_coverage_profiles.R` & `circtools-1.3.1/circtools/scripts/circtools_reconstruct_summarized_coverage_profiles.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_reconstruct_summary_graphs.R` & `circtools-1.3.1/circtools/scripts/circtools_reconstruct_summary_graphs.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_reconstruct_visualization.R` & `circtools-1.3.1/circtools/scripts/circtools_reconstruct_visualization.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/circtools_sirna_formatter.R` & `circtools-1.3.1/circtools/scripts/circtools_sirna_formatter.R`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/create_igv_script.py` & `circtools-1.3.1/circtools/scripts/create_igv_script.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/create_igv_script_from_gene_names.py` & `circtools-1.3.1/circtools/scripts/create_igv_script_from_gene_names.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/create_igv_script_from_position_list.py` & `circtools-1.3.1/circtools/scripts/create_igv_script_from_position_list.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/detect_new_exons_from_fuchs_data.py` & `circtools-1.3.1/circtools/scripts/detect_new_exons_from_fuchs_data.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/install_R_dependencies.R` & `circtools-1.3.1/circtools/scripts/install_R_dependencies.R`

 * *Files 14% similar despite different names*

```diff
@@ -80,53 +80,32 @@
 }
 message("")
 message("Installation will start in 10 seconds.")
 message("Press ctrl+c to cancel.")
 message("")
 
 countdown(10)
-
-message("")
-message("Now installing R CircTest and primex R packages.")
 message("")
 
-install.packages(paste0(base_path,"/contrib/primex"),
-                         repos = NULL,
-                          type = "source")
-
-
-install.packages(paste0(base_path,"/contrib/circtest"),
-                         repos = NULL,
-                          type = "source")
-
-q()
 
 if (
     majorVersion >= 4
     || ( majorVersion == 3 && minorVersion >= 6 )
 ){
     if (!requireNamespace("BiocManager", quietly = TRUE))
         install.packages("BiocManager")
 
-        local({r <- getOption("repos")
-             r["CRAN"] <- "https://cran.microsoft.com/"
-             options(repos=r)
-        })
 
         if (length(pkgs) > 0)
             BiocManager::install(pkgs)
 
 } else {
     source("https://bioconductor.org/biocLite.R")
     biocLite()
 
-    local({r <- getOption("repos")
-         r["CRAN"] <- "https://cran.microsoft.com/"
-         options(repos=r)
-    })
 
     if (length(pkgs) > 0)
         biocLite(pkgs)
 }
 
 # load devtools library
 library(devtools)
@@ -141,12 +120,7 @@
 
 
 install.packages(paste0(base_path,"/contrib/circtest"),
                          repos = NULL,
                           type = "source")
 
 
-# # install CircTest from the Dieterich Lab GitHub page from master branch
-# install_github("dieterich-lab/CircTest", ref = "master")
-#
-# # install primex from the Dieterich Lab GitHub page from master branch
-# install_github("dieterich-lab/primex", ref = "master")
```

### Comparing `circtools-1.3.0/circtools/scripts/install_add_to_bashrc.sh` & `circtools-1.3.1/circtools/scripts/install_add_to_bashrc.sh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/install_create_r_environ.sh` & `circtools-1.3.1/circtools/scripts/install_create_r_environ.sh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/install_external.sh` & `circtools-1.3.1/circtools/scripts/install_external.sh`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/r_runner.py` & `circtools-1.3.1/circtools/scripts/r_runner.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/scripts/wonderdump` & `circtools-1.3.1/circtools/scripts/wonderdump`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools/sirna/sirna.py` & `circtools-1.3.1/circtools/sirna/sirna.py`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools.egg-info/PKG-INFO` & `circtools-1.3.1/circtools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,197 +1,198 @@
 Metadata-Version: 2.1
 Name: circtools
-Version: 1.3.0
+Version: 1.3.1
 Summary: circtools - a circular RNA toolbox
 Home-page: https://github.com/jakobilab/circtools
 Author: Tobias Jakobi
 Author-email: tjakobi@arizona.edu
 License: GNU General Public License (GPL)
 Project-URL: Bug Reports, https://github.com/jakobilab/circtools/issues
 Project-URL: Jakobi Lab, https://jakobilab.org
 Project-URL: Source, https://github.com/jakobilab/circtools
 Project-URL: Documentation, https://docs.circ.tools
+Description: **circtools**
+        ======================================================================
+        
+        **a one-stop software solution for circular RNA research**
+        
+        .. figure:: https://raw.githubusercontent.com/jakobilab/circtools/master/docs/img/circtools_200px.png
+           :alt: circtools
+        
+        |docs| |build| |docker| |zenodo| |downloads| |pypi|
+        
+        Introduction
+        -------------
+        
+        Circular RNAs (circRNAs) originate through back-splicing events from linear primary transcripts, are resistant to exonucleases, typically not polyadenylated, and have been shown to be highly specific for cell type and developmental stage. Although few circular RNA molecules have been shown to exhibit miRNA sponge function, for the vast majority of circRNAs however, their function is yet to be determined.
+        
+        The prediction of circular RNAs is a multi-stage bioinformatics process starting with raw sequencing data and usually ending with a list of potential circRNA candidates which, depending on tissue and condition may contain hundreds to thousands of potential circRNAs. While there already exist a number of tools for the prediction process (e.g. `DCC <https://github.com/dieterich-lab/DCC>`__ and `CircTest <https://github.com/dieterich-lab/CircTest>`__), publicly available downstream analysis tools are rare.
+        
+        We developed **circtools**, a modular, Python3-based framework for circRNA-related tools that unifies several functionalities in single command line driven software. The command line follows the `circtools subcommand` standard that is employed in samtools or bedtools. Currently, circtools includes modules for detecting and reconstructing circRNAs,
+        a quick check of circRNA mapping results, RBP enrichment screenings, circRNA primer design, statistical testing, and an exon usage module.
+        
+        
+        
+        Documentation
+        -------------
+        
+        Click `here <https://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
+        
+        Installation
+        ------------
+        
+        The ``circtools`` package is written in Python 3 (supporting Python 3.7 - 3.10). It requires only a small number of external dependencies, namely standard bioinformatics tools:
+        
+        -  `bedtools (>= 2.27.1) <https://bedtools.readthedocs.io/en/latest/content/installation.html>`__
+           [RBP enrichment module, installed automatically]
+        -  `R (>= 4.0) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-22-04>`__
+           [Data visualization and data processing]
+        
+        Installation is managed through ``pip3 install circtools`` or ``python3 setup.py
+        install`` when installed from the cloned GitHub repository. No sudo access is
+        required if the installation is executed with ``--user`` which will install the
+        package in a user-writeable folder. The binaries should be installed
+        to ``/home/$user/.local/bin/`` in case of Debian-based systems.
+        
+        ``circtools`` was developed and tested on Debian Buster, but should also
+        run with any other distribution.
+        
+        The installation can be performed directly from Pypi:
+        
+        .. code-block:: console
+        
+            # install circtools
+            pip install numpy # required for HTSeq, a dependency of circtools
+            pip install circtools
+        
+            # install R packages for circtools
+            circtools_install_R_dependencies
+        
+        Additionally, this repository offers the latest development version:
+        
+        .. code-block:: console
+        
+            pip install numpy # required for HTSeq, a dependency of circtools
+            pip install git+https://github.com/jakobilab/circtools.git
+        
+        The primer-design module as well as the exon analysis and circRNA testing module
+        require a working installation of `R <https://cran.r-project.org/>`__ with
+        `BioConductor <https://www.bioconductor.org/install/>`__. All R packages
+        required can be automatically installed during the setup. Please see the
+        `"Installing circtools" <http://docs.circ.tools/en/latest/Installation.html>`__
+        chapter of the main circtools documentation for more detailed installation instructions.
+        
+        Modules
+        -------
+        
+        Circtools currently offers seven modules:
+        
+        detect `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Detect.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``detect`` command is an interface to
+        `DCC <https://github.com/dieterich-lab/DCC>`__, developed at the
+        Dieterich Lab. The module allows to detect circRNAs from RNA sequencing
+        data. The module is the foundation of all other steps for the circtools
+        work flow. All parameters supplied to circtools will be directly passed
+        to DCC.
+        
+        quickcheck `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Quickcheck.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The quickcheck module of circtools is an easy way to check the results
+        of a DCC run for problems and to quickly assess the number of circRNAs
+        in a given experiment. The module needs the mapping log files produced
+        by STAR as well as the directory with the DCC results. The module than
+        generates a series of figures in PDF format to assess the results.
+        
+        reconstruct `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Reconstruct.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``reconstruct`` command is an interface to
+        `FUCHS <https://github.com/dieterich-lab/FUCHS>`__. FUCHS is employing
+        DCC-generated data to reconstruct circRNA structures. All parameters
+        supplied to circtools will be directly passed to FUCHS.
+        
+        circtest `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Circtest.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``circtest`` command is an interface to
+        `CircTest <https://github.com/dieterich-lab/CircTest>`__. The module a a
+        very convenient way to employ statistical testing to circRNA candidates
+        generated with DCC without having to write an R script for each new
+        experiment. For detailed information on the implementation itself take a
+        look at the `CircTest
+        documentation <https://github.com/dieterich-lab/CircTest>`__. In
+        essence, the module allows dynamic grouping of the columns (samples) in
+        the DCC data.
+        
+        exon `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Exon.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The exon module of circtools employs the `ballgown R
+        package <https://www.bioconductor.org/packages/release/bioc/html/ballgown.html>`__
+        to combine data generated with DCC and circtest with ballgown-compatible
+        ``stringtie`` output or cufflinks output converted via
+        `tablemaker <https://github.com/leekgroup/tablemaker>`__ in order get
+        deeper insights into differential exon usage within circRNA candidates.
+        
+        enrich `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Enrichment.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``enrichment`` module may be used to identify circRNAs enriched for
+        specific RNA binding proteins (RBP) based on DCC-identified circRNAs and
+        processed
+        `eCLIP <http://www.nature.com/nmeth/journal/v13/n6/full/nmeth.3810.html>`__
+        data. For K526 and HepG2 cell lines plenty of this data is available
+        through the
+        `ENCODE <https://www.encodeproject.org/search/?type=Experiment&assay_title=eCLIP>`__
+        project.
+        
+        primer `(detailed documentation) <https://circtools.readthedocs.io/en/latest/primer.html>`__
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        The ``primer`` command is used to design and visualize primers required
+        for follow up wet lab experiments to verify circRNA candidates.
+        
+        
+        .. |docs| image:: https://readthedocs.org/projects/circtools/badge/?version=latest
+            :alt: Documentation Status
+            :scale: 100%
+            :target: https://circtools.readthedocs.io/en/latest/?badge=latest
+        
+        .. |build| image:: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml/badge.svg?branch=master
+            :alt: CI Status
+            :scale: 100%
+            :target: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml
+        
+        .. |docker| image:: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml/badge.svg?branch=master
+            :alt: Docker Build
+            :scale: 100%
+            :target: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml
+        
+        .. |zenodo| image:: https://zenodo.org/badge/498448368.svg
+            :alt: Zenodo DOI link
+            :scale: 100%
+            :target: https://zenodo.org/badge/latestdoi/498448368
+        
+        .. |downloads| image:: https://pepy.tech/badge/circtools
+            :alt: Python Package Index Downloads
+            :scale: 100%
+            :target: https://pepy.tech/project/circtools
+        
+        .. |pypi| image:: https://badge.fury.io/py/circtools.svg
+            :alt: Python package version
+            :scale: 100%
+            :target: https://badge.fury.io/py/circtools
+        
 Keywords: circRNA,circular RNA bioinformatics
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-
-**circtools**
-======================================================================
-
-**a one-stop software solution for circular RNA research**
-
-.. figure:: https://raw.githubusercontent.com/jakobilab/circtools/master/docs/img/circtools_200px.png
-   :alt: circtools
-
-|docs| |build| |docker| |zenodo| |downloads| |pypi|
-
-Introduction
--------------
-
-Circular RNAs (circRNAs) originate through back-splicing events from linear primary transcripts, are resistant to exonucleases, typically not polyadenylated, and have been shown to be highly specific for cell type and developmental stage. Although few circular RNA molecules have been shown to exhibit miRNA sponge function, for the vast majority of circRNAs however, their function is yet to be determined.
-
-The prediction of circular RNAs is a multi-stage bioinformatics process starting with raw sequencing data and usually ending with a list of potential circRNA candidates which, depending on tissue and condition may contain hundreds to thousands of potential circRNAs. While there already exist a number of tools for the prediction process (e.g. `DCC <https://github.com/dieterich-lab/DCC>`__ and `CircTest <https://github.com/dieterich-lab/CircTest>`__), publicly available downstream analysis tools are rare.
-
-We developed **circtools**, a modular, Python3-based framework for circRNA-related tools that unifies several functionalities in single command line driven software. The command line follows the `circtools subcommand` standard that is employed in samtools or bedtools. Currently, circtools includes modules for detecting and reconstructing circRNAs,
-a quick check of circRNA mapping results, RBP enrichment screenings, circRNA primer design, statistical testing, and an exon usage module.
-
-
-
-Documentation
--------------
-
-Click `here <https://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
-
-Installation
-------------
-
-The ``circtools`` package is written in Python 3 (supporting Python 3.7 - 3.10). It requires only a small number of external dependencies, namely standard bioinformatics tools:
-
--  `bedtools (>= 2.27.1) <https://bedtools.readthedocs.io/en/latest/content/installation.html>`__
-   [RBP enrichment module, installed automatically]
--  `R (>= 4.0) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-22-04>`__
-   [Data visualization and data processing]
-
-Installation is managed through ``pip3 install circtools`` or ``python3 setup.py
-install`` when installed from the cloned GitHub repository. No sudo access is
-required if the installation is executed with ``--user`` which will install the
-package in a user-writeable folder. The binaries should be installed
-to ``/home/$user/.local/bin/`` in case of Debian-based systems.
-
-``circtools`` was developed and tested on Debian Buster, but should also
-run with any other distribution.
-
-The installation can be performed directly from Pypi:
-
-.. code-block:: console
-
-    # install circtools
-    pip install numpy # required for HTSeq, a dependency of circtools
-    pip install circtools
-
-    # install R packages for circtools
-    circtools_install_R_dependencies
-
-Additionally, this repository offers the latest development version:
-
-.. code-block:: console
-
-    pip install numpy # required for HTSeq, a dependency of circtools
-    pip install git+https://github.com/jakobilab/circtools.git
-
-The primer-design module as well as the exon analysis and circRNA testing module
-require a working installation of `R <https://cran.r-project.org/>`__ with
-`BioConductor <https://www.bioconductor.org/install/>`__. All R packages
-required can be automatically installed during the setup. Please see the
-`"Installing circtools" <http://docs.circ.tools/en/latest/Installation.html>`__
-chapter of the main circtools documentation for more detailed installation instructions.
-
-Modules
--------
-
-Circtools currently offers seven modules:
-
-detect `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Detect.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``detect`` command is an interface to
-`DCC <https://github.com/dieterich-lab/DCC>`__, developed at the
-Dieterich Lab. The module allows to detect circRNAs from RNA sequencing
-data. The module is the foundation of all other steps for the circtools
-work flow. All parameters supplied to circtools will be directly passed
-to DCC.
-
-quickcheck `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Quickcheck.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The quickcheck module of circtools is an easy way to check the results
-of a DCC run for problems and to quickly assess the number of circRNAs
-in a given experiment. The module needs the mapping log files produced
-by STAR as well as the directory with the DCC results. The module than
-generates a series of figures in PDF format to assess the results.
-
-reconstruct `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Reconstruct.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``reconstruct`` command is an interface to
-`FUCHS <https://github.com/dieterich-lab/FUCHS>`__. FUCHS is employing
-DCC-generated data to reconstruct circRNA structures. All parameters
-supplied to circtools will be directly passed to FUCHS.
-
-circtest `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Circtest.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``circtest`` command is an interface to
-`CircTest <https://github.com/dieterich-lab/CircTest>`__. The module a a
-very convenient way to employ statistical testing to circRNA candidates
-generated with DCC without having to write an R script for each new
-experiment. For detailed information on the implementation itself take a
-look at the `CircTest
-documentation <https://github.com/dieterich-lab/CircTest>`__. In
-essence, the module allows dynamic grouping of the columns (samples) in
-the DCC data.
-
-exon `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Exon.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The exon module of circtools employs the `ballgown R
-package <https://www.bioconductor.org/packages/release/bioc/html/ballgown.html>`__
-to combine data generated with DCC and circtest with ballgown-compatible
-``stringtie`` output or cufflinks output converted via
-`tablemaker <https://github.com/leekgroup/tablemaker>`__ in order get
-deeper insights into differential exon usage within circRNA candidates.
-
-enrich `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Enrichment.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``enrichment`` module may be used to identify circRNAs enriched for
-specific RNA binding proteins (RBP) based on DCC-identified circRNAs and
-processed
-`eCLIP <http://www.nature.com/nmeth/journal/v13/n6/full/nmeth.3810.html>`__
-data. For K526 and HepG2 cell lines plenty of this data is available
-through the
-`ENCODE <https://www.encodeproject.org/search/?type=Experiment&assay_title=eCLIP>`__
-project.
-
-primer `(detailed documentation) <https://circtools.readthedocs.io/en/latest/primer.html>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``primer`` command is used to design and visualize primers required
-for follow up wet lab experiments to verify circRNA candidates.
-
-
-.. |docs| image:: https://readthedocs.org/projects/circtools/badge/?version=latest
-    :alt: Documentation Status
-    :scale: 100%
-    :target: https://circtools.readthedocs.io/en/latest/?badge=latest
-
-.. |build| image:: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml/badge.svg?branch=master
-    :alt: CI Status
-    :scale: 100%
-    :target: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml
-
-.. |docker| image:: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml/badge.svg?branch=master
-    :alt: Docker Build
-    :scale: 100%
-    :target: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml
-
-.. |zenodo| image:: https://zenodo.org/badge/83248654.svg
-    :alt: Zenodo DOI link
-    :scale: 100%
-    :target: https://zenodo.org/badge/latestdoi/83248654
-
-.. |downloads| image:: https://pepy.tech/badge/circtools
-    :alt: Python Package Index Downloads
-    :scale: 100%
-    :target: https://pepy.tech/project/circtools
-
-.. |pypi| image:: https://badge.fury.io/py/circtools.svg
-    :alt: Python package version
-    :scale: 100%
-    :target: https://badge.fury.io/py/circtools
```

### Comparing `circtools-1.3.0/circtools.egg-info/SOURCES.txt` & `circtools-1.3.1/circtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circtools-1.3.0/circtools.egg-info/entry_points.txt` & `circtools-1.3.1/circtools.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 circtools_sirna_formatter = circtools.scripts.r_runner:circtools_sirna_formatter
 create_igv_script = circtools.scripts.create_igv_script:main
 create_igv_script_from_gene_names = circtools.scripts.create_igv_script_from_gene_names:main
 create_igv_script_from_position_list = circtools.scripts.create_igv_script_from_position_list:main
 detect_new_exons_from_fuchs_data = circtools.scripts.detect_new_exons_from_fuchs_data:main
 guided_denovo_circle_structure = circtools.reconstruct.guided_denovo_circle_structure_parallel:main
 wonderdump = circtools.scripts.bash_runner:wonderdump
+
```

### Comparing `circtools-1.3.0/setup.cfg` & `circtools-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = circtools
 description = circtools - a circular RNA toolbox
-version = 1.3.0
+version = 1.3.1
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/jakobilab/circtools
 author = Tobias Jakobi
 author_email = tjakobi@arizona.edu
 license = GNU General Public License (GPL)
 license_files = LICENSE.rst
```

