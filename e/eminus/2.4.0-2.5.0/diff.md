# Comparing `tmp/eminus-2.4.0.tar.gz` & `tmp/eminus-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eminus-2.4.0.tar", last modified: Tue May 23 10:05:07 2023, max compression
+gzip compressed data, was "eminus-2.5.0.tar", last modified: Mon Jul 10 15:14:27 2023, max compression
```

## Comparing `eminus-2.4.0.tar` & `eminus-2.5.0.tar`

### file list

```diff
@@ -1,373 +1,373 @@
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.042773 eminus-2.4.0/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5775 2023-05-23 09:48:52.000000 eminus-2.4.0/CHANGELOG.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10173 2022-05-25 09:24:55.000000 eminus-2.4.0/LICENSE
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       61 2023-05-17 14:03:34.000000 eminus-2.4.0/MANIFEST.in
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3820 2023-05-23 10:05:07.042773 eminus-2.4.0/PKG-INFO
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1518 2023-05-05 09:27:44.000000 eminus-2.4.0/README.md
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      980 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      778 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    15551 2023-05-22 16:23:17.000000 eminus-2.4.0/eminus/atoms.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4831 2023-05-22 14:40:40.000000 eminus-2.4.0/eminus/config.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6977 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/data.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    12188 2023-05-22 16:46:01.000000 eminus-2.4.0/eminus/dft.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3254 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/domains.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10042 2023-05-22 11:47:34.000000 eminus-2.4.0/eminus/energies.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus/extras/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      324 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/extras/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/extras/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6549 2023-05-20 10:20:21.000000 eminus-2.4.0/eminus/extras/fods.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4519 2023-05-19 14:49:21.000000 eminus-2.4.0/eminus/extras/libxc.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6361 2023-05-22 14:35:23.000000 eminus-2.4.0/eminus/extras/torch.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8502 2023-05-20 15:15:32.000000 eminus-2.4.0/eminus/extras/viewer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6353 2023-05-05 09:27:14.000000 eminus-2.4.0/eminus/gth.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus/io/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      260 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/io/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1240 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/io/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5785 2023-05-17 14:01:39.000000 eminus-2.4.0/eminus/io/cube.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3688 2023-05-17 16:25:40.000000 eminus-2.4.0/eminus/io/gth.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3442 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/io/json.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4052 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/io/pdb.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3264 2023-05-17 14:01:39.000000 eminus-2.4.0/eminus/io/xyz.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10633 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/localizer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2700 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/logger.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    13656 2023-05-22 11:47:48.000000 eminus-2.4.0/eminus/minimizer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8614 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/operators.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4007 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/orbitals.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2629 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/potentials.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus/psp/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       56 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/__init__.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.026773 eminus-2.4.0/eminus/psp/pade/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ac-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ac-q29
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ag-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ag-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ag-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Al-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Am-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Am-q35
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ar-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/As-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/At-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Au-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Au-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Au-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/B-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      372 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ba-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ba-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Be-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Be-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Bi-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Bk-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Bk-q37
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Br-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/C-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ca-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ca-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cd-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cd-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ce-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cf-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cf-q38
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cl-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cm-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cm-q36
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Co-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Co-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cr-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cr-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cs-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      370 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cs-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cu-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cu-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cu-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Dy-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Er-q22
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Es-q21
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Es-q39
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Eu-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/F-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Fe-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Fe-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Fm-q22
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Fm-q40
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ga-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ga-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Gd-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ge-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       88 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/H-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       89 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/He-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Hf-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Hg-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Hg-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ho-q21
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      414 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/I-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/In-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/In-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ir-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ir-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/K-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      297 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/K-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Kr-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      473 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/La-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Li-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Li-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Lr-q25
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Lr-q43
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Lu-q25
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Md-q23
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Md-q41
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      168 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mg-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mg-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mn-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mn-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mo-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mo-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/N-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Na-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      166 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Na-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Nb-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Nb-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Nd-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      232 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ne-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ni-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ni-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/No-q24
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/No-q42
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Np-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Np-q33
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/O-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Os-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Os-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/P-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pa-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pa-q31
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pb-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pd-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pd-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pm-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Po-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pr-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pt-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pt-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pu-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pu-q34
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rb-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      334 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rb-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Re-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Re-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rh-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rh-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rn-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ru-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ru-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/S-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sb-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sc-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sc-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Se-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Si-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sm-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sn-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sr-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sr-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ta-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ta-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tb-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tc-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tc-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Te-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Th-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Th-q30
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ti-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ti-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tl-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tl-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tm-q23
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/U-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/U-q32
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      340 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/V-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      404 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/V-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      502 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/W-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      389 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/W-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Xe-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      406 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Y-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Y-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Yb-q24
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zn-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zn-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zn-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zr-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      486 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zr-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      842 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/__init__.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.038773 eminus-2.4.0/eminus/psp/pbe/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ac-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ac-q29
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      475 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ag-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ag-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Al-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Am-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Am-q35
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ar-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/As-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/At-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Au-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      571 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Au-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/B-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      359 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ba-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      107 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Be-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Bi-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Bi-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Bk-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Bk-q37
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Br-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/C-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      323 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ca-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      475 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cd-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ce-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      465 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ce-q30
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cf-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cf-q38
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cl-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cm-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cm-q36
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Co-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cr-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      358 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cs-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cu-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cu-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Dy-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Er-q22
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Es-q21
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Es-q39
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Eu-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/F-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Fe-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Fm-q22
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Fm-q40
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ga-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ga-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Gd-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ge-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       76 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/H-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       77 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/He-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Hf-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Hg-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ho-q21
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      402 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/I-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      475 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/In-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/In-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ir-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ir-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      285 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/K-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Kr-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      364 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/La-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      107 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Li-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Lr-q25
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Lr-q43
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Lu-q25
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Md-q23
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Md-q41
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      155 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Mg-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      200 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Mg-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Mn-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Mo-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/N-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      200 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Na-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      154 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Na-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Nb-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Nd-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      220 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ne-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ni-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/No-q24
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/No-q42
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Np-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Np-q33
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/O-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Os-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Os-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      204 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/P-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pa-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pa-q31
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pb-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pb-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pd-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pd-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pm-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Po-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pr-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pt-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      586 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pt-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pu-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pu-q34
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      322 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Rb-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Re-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Re-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Rh-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Rh-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Rn-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ru-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ru-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      204 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/S-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sb-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sc-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Se-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Si-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sm-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sn-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      323 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sr-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ta-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ta-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tb-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tc-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Te-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Th-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Th-q30
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ti-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tl-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tl-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tm-q23
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      626 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/U-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      630 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/U-q14_old
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      626 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/U-q32
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      327 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/V-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      489 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/W-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      377 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/W-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Xe-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      393 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Y-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Yb-q24
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Zn-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Zn-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Zr-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      843 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    12469 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/scf.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     9555 2023-05-22 13:25:09.000000 eminus-2.4.0/eminus/tools.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3048 2023-05-05 09:27:14.000000 eminus-2.4.0/eminus/units.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5521 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/utils.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1473 2023-05-23 09:48:58.000000 eminus-2.4.0/eminus/version.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.042773 eminus-2.4.0/eminus/xc/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      789 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      360 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4348 2023-05-17 14:59:59.000000 eminus-2.4.0/eminus/xc/gga_c_chachiyo.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4415 2023-05-17 22:17:28.000000 eminus-2.4.0/eminus/xc/gga_c_pbe.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1240 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/gga_c_pbe_sol.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2695 2023-05-17 22:16:05.000000 eminus-2.4.0/eminus/xc/gga_x_chachiyo.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4334 2023-05-17 16:20:03.000000 eminus-2.4.0/eminus/xc/gga_x_pbe.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1225 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/gga_x_pbe_sol.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3200 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_chachiyo.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1952 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_chachiyo_mod.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3467 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_pw.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1224 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_pw_mod.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3084 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_vwn.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1646 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_x.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/utils.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus.egg-info/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3820 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/PKG-INFO
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     7893 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/SOURCES.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/dependency_links.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2022-09-27 12:14:58.000000 eminus-2.4.0/eminus.egg-info/not-zip-safe
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      330 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/requires.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        7 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/top_level.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       86 2023-05-05 09:27:44.000000 eminus-2.4.0/pyproject.toml
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       38 2023-05-23 10:05:07.042773 eminus-2.4.0/setup.cfg
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3436 2023-05-05 09:27:44.000000 eminus-2.4.0/setup.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-07-10 15:14:27.178795 eminus-2.5.0/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     7913 2023-07-10 14:45:14.000000 eminus-2.5.0/CHANGELOG.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10173 2022-05-25 09:24:55.000000 eminus-2.5.0/LICENSE
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       61 2023-07-06 11:35:29.000000 eminus-2.5.0/MANIFEST.in
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5494 2023-07-10 15:14:27.178795 eminus-2.5.0/PKG-INFO
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1541 2023-07-07 09:39:45.000000 eminus-2.5.0/README.md
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-07-10 15:14:27.150795 eminus-2.5.0/eminus/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1041 2023-06-02 09:17:14.000000 eminus-2.5.0/eminus/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      800 2023-07-06 08:18:39.000000 eminus-2.5.0/eminus/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    15744 2023-07-05 14:03:51.000000 eminus-2.5.0/eminus/atoms.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4885 2023-07-05 14:04:32.000000 eminus-2.5.0/eminus/config.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6977 2023-07-05 13:56:17.000000 eminus-2.5.0/eminus/data.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     9990 2023-07-06 13:56:58.000000 eminus-2.5.0/eminus/dft.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3230 2023-07-05 13:56:06.000000 eminus-2.5.0/eminus/domains.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10721 2023-07-05 13:56:04.000000 eminus-2.5.0/eminus/energies.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-07-10 15:14:27.150795 eminus-2.5.0/eminus/extras/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      324 2023-05-05 09:27:44.000000 eminus-2.5.0/eminus/extras/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-07-05 13:55:46.000000 eminus-2.5.0/eminus/extras/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6549 2023-07-05 13:55:54.000000 eminus-2.5.0/eminus/extras/fods.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5720 2023-07-05 13:55:51.000000 eminus-2.5.0/eminus/extras/libxc.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6361 2023-07-05 13:55:50.000000 eminus-2.5.0/eminus/extras/torch.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10675 2023-07-10 13:36:58.000000 eminus-2.5.0/eminus/extras/viewer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6010 2023-07-05 13:56:20.000000 eminus-2.5.0/eminus/gga.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6462 2023-07-05 13:56:19.000000 eminus-2.5.0/eminus/gth.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-07-10 15:14:27.150795 eminus-2.5.0/eminus/io/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      260 2023-05-05 09:27:44.000000 eminus-2.5.0/eminus/io/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1280 2023-07-05 13:55:45.000000 eminus-2.5.0/eminus/io/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5768 2023-07-10 12:16:44.000000 eminus-2.5.0/eminus/io/cube.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3685 2023-07-05 13:55:57.000000 eminus-2.5.0/eminus/io/gth.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3442 2023-07-06 14:28:09.000000 eminus-2.5.0/eminus/io/json.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4107 2023-07-05 13:55:56.000000 eminus-2.5.0/eminus/io/pdb.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3485 2023-07-05 13:55:55.000000 eminus-2.5.0/eminus/io/xyz.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10840 2023-07-06 14:29:14.000000 eminus-2.5.0/eminus/localizer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2750 2023-07-05 14:04:51.000000 eminus-2.5.0/eminus/logger.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    17565 2023-07-06 13:22:48.000000 eminus-2.5.0/eminus/minimizer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8603 2023-07-06 13:24:54.000000 eminus-2.5.0/eminus/operators.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4046 2023-07-05 13:56:02.000000 eminus-2.5.0/eminus/orbitals.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2682 2023-07-05 13:55:58.000000 eminus-2.5.0/eminus/potentials.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-07-10 15:14:27.150795 eminus-2.5.0/eminus/psp/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       56 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/__init__.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-07-10 15:14:27.166795 eminus-2.5.0/eminus/psp/pade/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ac-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ac-q29
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ag-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ag-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ag-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Al-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Am-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Am-q35
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ar-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/As-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/At-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Au-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Au-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Au-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/B-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      372 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ba-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ba-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Be-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Be-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Bi-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Bk-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Bk-q37
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Br-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/C-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ca-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ca-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cd-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cd-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ce-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cf-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cf-q38
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cl-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cm-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cm-q36
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Co-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Co-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cr-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cr-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cs-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      370 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cs-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cu-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cu-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Cu-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Dy-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Er-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Es-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Es-q39
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Eu-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/F-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Fe-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Fe-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Fm-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Fm-q40
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ga-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ga-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Gd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ge-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       88 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/H-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       89 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/He-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Hf-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Hg-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Hg-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ho-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      414 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/I-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/In-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/In-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ir-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ir-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/K-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      297 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/K-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Kr-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      473 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/La-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Li-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Li-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Lr-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Lr-q43
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Lu-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Md-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Md-q41
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      168 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Mg-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Mg-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Mn-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Mn-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Mo-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Mo-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/N-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Na-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      166 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Na-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Nb-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Nb-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Nd-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      232 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ne-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ni-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ni-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/No-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/No-q42
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Np-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Np-q33
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/O-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Os-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Os-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/P-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pa-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pa-q31
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pb-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pd-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pm-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Po-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pr-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pt-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pt-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pu-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Pu-q34
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Rb-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      334 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Rb-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Re-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Re-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Rh-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Rh-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Rn-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ru-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ru-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/S-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Sb-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Sc-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Sc-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Se-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Si-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Sm-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Sn-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Sr-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Sr-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ta-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ta-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Tb-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Tc-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Tc-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Te-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Th-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Th-q30
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ti-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Ti-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Tl-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Tl-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Tm-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/U-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/U-q32
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      340 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/V-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      404 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/V-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      502 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/W-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      389 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/W-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Xe-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      406 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Y-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Y-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Yb-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Zn-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Zn-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Zn-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Zr-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      486 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/Zr-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      842 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pade/__init__.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-07-10 15:14:27.178795 eminus-2.5.0/eminus/psp/pbe/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ac-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ac-q29
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      475 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ag-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ag-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Al-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Am-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Am-q35
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ar-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/As-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/At-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Au-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      571 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Au-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/B-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      359 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ba-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      107 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Be-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Bi-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Bi-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Bk-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Bk-q37
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Br-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/C-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      323 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ca-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      475 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cd-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ce-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      465 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ce-q30
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cf-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cf-q38
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cl-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cm-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cm-q36
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Co-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cr-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      358 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cs-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cu-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Cu-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Dy-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Er-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Es-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Es-q39
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Eu-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/F-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Fe-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Fm-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Fm-q40
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ga-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ga-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Gd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ge-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       76 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/H-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       77 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/He-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Hf-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Hg-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ho-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      402 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/I-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      475 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/In-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/In-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ir-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ir-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      285 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/K-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Kr-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      364 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/La-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      107 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Li-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Lr-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Lr-q43
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Lu-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Md-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Md-q41
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      155 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Mg-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      200 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Mg-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Mn-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Mo-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/N-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      200 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Na-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      154 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Na-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Nb-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Nd-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      220 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ne-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ni-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/No-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/No-q42
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Np-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Np-q33
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/O-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Os-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Os-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      204 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/P-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pa-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pa-q31
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pb-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pb-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pd-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pm-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Po-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pr-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pt-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      586 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pt-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pu-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Pu-q34
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      322 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Rb-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Re-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Re-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Rh-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Rh-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Rn-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ru-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ru-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      204 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/S-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Sb-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Sc-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Se-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Si-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Sm-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Sn-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      323 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Sr-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ta-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ta-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Tb-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Tc-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Te-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Th-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Th-q30
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Ti-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Tl-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Tl-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Tm-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      626 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/U-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      630 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/U-q14_old
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      626 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/U-q32
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      327 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/V-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      489 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/W-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      377 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/W-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Xe-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      393 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Y-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Yb-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Zn-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Zn-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/Zr-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      843 2023-07-06 10:29:28.000000 eminus-2.5.0/eminus/psp/pbe/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    13969 2023-07-05 14:05:10.000000 eminus-2.5.0/eminus/scf.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    11829 2023-07-05 13:56:15.000000 eminus-2.5.0/eminus/tools.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3058 2023-07-05 13:56:13.000000 eminus-2.5.0/eminus/units.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5999 2023-07-06 08:20:55.000000 eminus-2.5.0/eminus/utils.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1431 2023-07-10 14:45:23.000000 eminus-2.5.0/eminus/version.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-07-10 15:14:27.178795 eminus-2.5.0/eminus/xc/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      789 2023-05-17 14:03:34.000000 eminus-2.5.0/eminus/xc/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      387 2023-07-05 13:55:43.000000 eminus-2.5.0/eminus/xc/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4103 2023-07-05 13:55:33.000000 eminus-2.5.0/eminus/xc/gga_c_chachiyo.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4132 2023-07-05 13:55:41.000000 eminus-2.5.0/eminus/xc/gga_c_pbe.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1358 2023-07-05 13:55:35.000000 eminus-2.5.0/eminus/xc/gga_c_pbe_sol.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2424 2023-07-05 13:55:32.000000 eminus-2.5.0/eminus/xc/gga_x_chachiyo.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3911 2023-07-05 13:55:40.000000 eminus-2.5.0/eminus/xc/gga_x_pbe.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1343 2023-07-05 13:55:34.000000 eminus-2.5.0/eminus/xc/gga_x_pbe_sol.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2813 2023-07-05 13:55:31.000000 eminus-2.5.0/eminus/xc/lda_c_chachiyo.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1910 2023-07-05 13:57:17.000000 eminus-2.5.0/eminus/xc/lda_c_chachiyo_mod.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3198 2023-07-05 13:55:42.000000 eminus-2.5.0/eminus/xc/lda_c_pw.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1342 2023-07-05 13:55:37.000000 eminus-2.5.0/eminus/xc/lda_c_pw_mod.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2846 2023-07-05 13:55:39.000000 eminus-2.5.0/eminus/xc/lda_c_vwn.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1438 2023-07-05 13:55:49.000000 eminus-2.5.0/eminus/xc/lda_x.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10894 2023-07-05 13:55:48.000000 eminus-2.5.0/eminus/xc/utils.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-07-10 15:14:27.150795 eminus-2.5.0/eminus.egg-info/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5494 2023-07-10 15:14:27.000000 eminus-2.5.0/eminus.egg-info/PKG-INFO
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     7878 2023-07-10 15:14:27.000000 eminus-2.5.0/eminus.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-07-10 15:14:27.000000 eminus-2.5.0/eminus.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      284 2023-07-10 15:14:27.000000 eminus-2.5.0/eminus.egg-info/requires.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        7 2023-07-10 15:14:27.000000 eminus-2.5.0/eminus.egg-info/top_level.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2052 2023-07-07 14:54:17.000000 eminus-2.5.0/pyproject.toml
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       38 2023-07-10 15:14:27.178795 eminus-2.5.0/setup.cfg
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3264 2023-07-06 11:41:42.000000 eminus-2.5.0/setup.py
```

### Comparing `eminus-2.4.0/CHANGELOG.md` & `eminus-2.5.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,67 @@
 Changelog
 =========
 
+v2.5.0 - Jul 10, 2023
+---------------------
+- New features
+   - Add meta-GGA functionals!
+      - Use all meta-GGAs that don't need a Laplacian from Libxc using pylibxc or PySCF
+   - Improved minimizer
+      - Add new auto minimizer that functions like pccg but can fallback to sd steps
+      - Add Dai-Yuan conjugate-gradient form
+      - Fancier-looking output from the minimizer
+      - Option to converge the gradient norm
+      - Print <S^2> after an unrestricted calculation
+      - Add eigenenergies to the debug output
+   - Improved file viewer
+      - Support PDB files
+      - Allow usage outside of notebooks
+- Updated docs
+   - Update the introduction page in the documentation
+   - Upload the HTML coverage report
+- Coding style
+   - Simplify H function
+   - Simplify minimizer module
+   - Reduce McCabe code complexity
+   - Switch linter from flake8 to Ruff
+   - Comply with different linting rules, e.g., use triple-quotes in docstrings
+   - More tests and more coverage
+- Miscellaneous
+   - Performance fix by using precomputed values correctly
+   - Improve GGA performance
+   - Do an unpaired calculation automatically if the system is unpaired
+   - Option to use a symmetric initial guess, i.e., the same guess for both spin channels
+   - Add trajectory keyword to XYZ and PDB writer to append geometries
+   - Read the field data from CUBE files
+   - New functions for the
+      - Electron localization function (ELF)
+      - Positive-definite kinetic energy density
+      - Reduced density gradient
+      - Expectation value of S^2 and the multiplicity calculated from it
+   - Option to set a path to directories containing GTH pseudopotential files
+   - The SCF class now contains the xc_type and is_converged variables
+   - Support functional parsing using pylibxc
+   - Allow using custom densities when using the atoms viewer
+   - Remove Gaussian initial guess
+   - Remove exc_only keyword from functionals since it was basically unused
+   - Fix GTH files not being installed when using the PyPI version
+   - Fix mapping of field entries with the respective real-space coordinate
+   - Fix GGA SIC evaluation
+
+----
+
 v2.4.0 - May 23, 2023
 ---------------------
 - New features
    - Add GGA functionals!
       - Add internal PBE, PBEsol, and Chachiyo functionals
       - Option to use all GGAs from Libxc using pylibxc or PySCF
 - Miscellaneous
-   - Add Thomas-Fermi and von Weizsäcker kinetic energy density functions
+   - Add Thomas-Fermi and von Weizsaecker kinetic energy density functions
    - Rewrite functionals for better readability
    - Fix Torch operators in some edge cases
    - Merge configuration files in tox.ini
    - Update minimum versions of dependencies
 
 ----
 
@@ -67,15 +116,15 @@
    - Update logo typography
 - Updated docs
    - Add a nomenclature page of commonly used variables
    - Remove the package name from the module headings
    - Document members of classes
 - Coding style
    - More secure coding practices
-   - Remov the usage of eval, exec, and pickle
+   - Remove the usage of eval, exec, and pickle
 - Miscellaneous
    - Rename save and load to write_json and read_json
    - Fix PW spin-polarized functional
    - Align Chachiyo functional with Libxc
    - Add a germanium solid example
    - Add a recenter method to the Atoms and SCF class
    - Use pc-1 over pc-0 in the PyCOM extra
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eminus-2.4.0/LICENSE` & `eminus-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/README.md` & `eminus-2.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-![eminus logo](https://gitlab.com/wangenau/eminus/-/raw/main/docs/logo/eminus_logo.png)
+![eminus logo](https://gitlab.com/wangenau/eminus/-/raw/main/docs/_static/logo/eminus_logo.png)
 
 # eminus
 [![pypi](https://img.shields.io/pypi/v/eminus?color=1a962b)](https://pypi.org/project/eminus)
-[![language](https://img.shields.io/badge/language-Python3-green)](https://www.python.org)
-[![license](https://img.shields.io/badge/license-APACHE2-lightgrey)](https://gitlab.com/wangenau/eminus/-/blob/main/LICENSE)
-[![coverage](https://gitlab.com/wangenau/eminus/badges/main/coverage.svg)](https://gitlab.com/wangenau/eminus/-/graphs/main/charts)
-[![DOI](https://zenodo.org/badge/431079841.svg)](https://zenodo.org/badge/latestdoi/431079841)
+[![coverage](https://gitlab.com/wangenau/eminus/badges/main/coverage.svg)](https://wangenau.gitlab.io/eminus/htmlcov)
+[![python](https://img.shields.io/pypi/pyversions/eminus?color=green)](https://wangenau.gitlab.io/eminus/installation.html)
+[![license](https://img.shields.io/badge/license-Apache2.0-yellowgreen)](https://wangenau.gitlab.io/eminus/license.html)
+[![doi](https://zenodo.org/badge/431079841.svg)](https://zenodo.org/badge/latestdoi/431079841)
 
 The eminus package is a plane wave density functional theory (DFT) code.
 It is built upon the [DFT++](https://arxiv.org/abs/cond-mat/9909130) pragmas, that aim to let programming languages and theory coincide.
 The goal is to create a simple code that is easy to read and easy to extend while using minimal dependencies.
 
 ## Documentation
```

### Comparing `eminus-2.4.0/eminus/README.md` & `eminus-2.5.0/eminus/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | :------------: | :---------: |
 | atoms.py       | Atoms class definition |
 | config.py      | Consolidated configuration module |
 | data.py        | Atom specific data |
 | dft.py         | DFT routines |
 | domains.py     | Domain generation |
 | energies.py    | Energy object and calculation |
+| gga.py         | Functions needed for GGAs and meta-GGAs |
 | gth.py         | GTH pseudopotential functions |
 | localizer.py   | Localization routines |
 | logger.py      | Logging configuration |
 | minimizer.py   | Minimization algorithms |
 | operators.py   | Plane-wave basis-set dependent operators |
 | orbitals.py    | Orbital generation workflows |
 | potentials.py  | Miscellaneous (pseudo-)potentials |
```

### Comparing `eminus-2.4.0/eminus/__init__.py` & `eminus-2.5.0/eminus/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 #!/usr/bin/env python3
-'''eminus - A plane wave density functional theory code.
+"""eminus - A plane wave density functional theory code.
 
 Minimal usage example to do a DFT calculation for helium::
 
    from eminus import Atoms, SCF
-   atoms = Atoms('He', [0, 0, 0])
+   atoms = Atoms('He', (0, 0, 0))
    SCF(atoms).run()
-'''
+"""
 from . import config
 from .atoms import Atoms
 from .dft import get_epsilon, get_psi
-from .io import (read, read_cube, read_json, read_xyz, write, write_cube, write_json, write_pdb,
-                 write_xyz)
+from .io import (
+    read,
+    read_cube,
+    read_json,
+    read_xyz,
+    write,
+    write_cube,
+    write_json,
+    write_pdb,
+    write_xyz,
+)
 from .logger import log
 from .scf import RSCF, SCF, USCF
 from .version import __version__, info
 
 __all__ = ['config', 'Atoms', 'get_epsilon', 'get_psi', 'info', 'log', 'read', 'read_cube',
            'read_json', 'read_xyz', 'RSCF', 'SCF', 'USCF', 'write', 'write_cube', 'write_json',
            'write_pdb', 'write_xyz', '__version__']
```

### Comparing `eminus-2.4.0/eminus/atoms.py` & `eminus-2.5.0/eminus/atoms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 #!/usr/bin/env python3
-'''Atoms class definition.'''
+"""Atoms class definition."""
 import re
 
 import numpy as np
 from scipy.fft import next_fast_len
 from scipy.linalg import det, eig, inv, norm
 
 from . import config, operators
 from .io import read_gth
 from .logger import create_logger, get_level, log
 from .tools import center_of_mass, cutoff2gridspacing, inertia_tensor
 
 
 class Atoms:
-    '''Atoms object that holds all system and cell parameters.
+    """Atoms object that holds all system and cell parameters.
 
     Args:
         atom (str | list | tuple): Atom symbols.
 
-            Examples: 'CH4'; ['C', 'H', 'H', 'H', 'H']; ('C', 'H', 'H', 'H', 'H')
+            Example: 'CH4'; ['C', 'H', 'H', 'H', 'H']; ('C', 'H', 'H', 'H', 'H')
         X (list | tuple | ndarray): Atom positions.
 
-            Examples: (0, 0, 0); array([0, 0, 0]); [[0, 0, 0], [1, 1, 1]];
+            Example: (0, 0, 0); array([0, 0, 0]); [[0, 0, 0], [1, 1, 1]];
 
     Keyword Args:
         a (float | list | tuple | ndarray): Cell size or vacuum size.
 
             A cuboidal box with the same side lengths will be created.
 
-            Examples: 10; [10, 10, 10]; (7, 8, 9),
+            Example: 10; [10, 10, 10]; (7, 8, 9),
             Default: 20 Bohr (ca. 10.5 Angstrom).
         ecut (float | None): Cut-off energy.
 
             None will disable the G-Vector truncation (needs a separate s).
             Default: 30 Hartree (ca. 816 eV).
         Z (int | list | tuple | ndarray | dict | str | None): Valence charge per atom.
 
@@ -75,17 +75,18 @@
 
             Can be one of 'CRITICAL', 'ERROR', 'WARNING', 'INFO', or 'DEBUG'.
             An integer value can be used as well, where larger numbers mean more output, starting
             from 0.
             None will use the default global logger value 'WARNING'.
 
             Default: None
-    '''
-    def __init__(self, atom, X, a=20, ecut=30, Z=None, s=None, center=False, Nspin=2, f=None,
+    """
+    def __init__(self, atom, X, a=20, ecut=30, Z=None, s=None, center=False, Nspin=None, f=None,
                  Nstate=None, verbose=None):
+        """Initialize the Atoms object."""
         self.atom = atom      # Atom symbols
         self.X = X            # Atom positions
         self.a = a            # Cell/Vacuum size
         self.ecut = ecut      # Cut-off energy
         self.Z = Z            # Valence charges
         self.s = s            # Cell sampling
         self.center = center  # Center molecule in cell
@@ -104,65 +105,65 @@
         if verbose is not None:
             self.verbose = verbose
         else:
             self.verbose = log.verbose
         self.initialize()
 
     def clear(self):
-        '''Initialize and clear parameters that will be built out of the inputs.'''
+        """Initialize and clear parameters that will be built out of the inputs."""
         self.r = None          # Sample points in cell
         self.G = None          # G-vectors
         self.G2 = None         # Squared magnitudes of G-vectors
         self.active = None     # Mask for active G-vectors
         self.G2c = None        # Truncated squared magnitudes of G-vectors
         self.Sf = None         # Structure factor
         self.is_built = False  # Flag to determine if the object was built or not
         return self
 
     def initialize(self):
-        '''Validate inputs and update them if necessary.'''
+        """Validate inputs and update them if necessary."""
         self._set_atom()
         self._set_charge()
         self._set_cell_size()
         self._set_positions()
         self._set_sampling()
         return self
 
     def build(self):
-        '''Build all necessary parameters.'''
+        """Build all necessary parameters."""
         self._set_states(self.Nspin)
         M, N = self._get_index_matrices()
         self._set_cell(M)
         self._set_G(N)
         self._set_operators()
         self.is_built = True
         return self
 
     kernel = build
 
     def recenter(self, center=None):
-        '''Recenter the system inside the cell.
+        """Recenter the system inside the cell.
 
         Keyword Args:
             center (float | list | tuple | ndarray | None): Point to center the system around.
-        '''
+        """
         com = center_of_mass(self.X)
         if center is None:
             self.X = self.X - (com - self.a / 2)
         else:
             center = np.asarray(center)
             self.X = self.X - (com - center)
 
         # Recalculate the structure factor since it depends on the atom positions
         _, N = self._get_index_matrices()
         self._set_G(N)
         return self
 
     def _set_atom(self):
-        '''Validate the atom input and calculate the number of atoms.'''
+        """Validate the atom input and calculate the number of atoms."""
         # Quick option to set the charge for single atoms
         if isinstance(self.atom, str) and '-q' in self.atom:
             atom, Z = self.atom.split('-q')
             self.atom = [atom]
             self.Z = np.asarray(list(Z), dtype=int)
         # If a string is given for atom symbols convert them to a list of strings
         if isinstance(self.atom, str):
@@ -180,47 +181,50 @@
             self.atom = atom
 
         # Get the number of atoms
         self.Natoms = len(self.atom)
         return
 
     def _set_charge(self):
-        '''Validate the Z input and calculate charges if necessary.'''
+        """Validate the Z input and calculate charges if necessary."""
         # If only one charge is given, assume it is the charge for every atom
         if isinstance(self.Z, (int, np.integer)):
             self.Z = [self.Z] * self.Natoms
         if isinstance(self.Z, dict):
             self.Z = [self.Z[ia] for ia in self.atom]
         if isinstance(self.Z, (list, tuple)):
             self.Z = np.asarray(self.Z)
 
         # If no charge is given, use the ionic charge from the GTH files
         if self.Z is None or isinstance(self.Z, str):
             if isinstance(self.Z, str):
-                xc = self.Z.lower()
+                if self.Z.lower() in ('pade', 'pbe'):
+                    psp_path = self.Z.lower()
+                else:
+                    psp_path = self.Z
             else:
-                xc = 'pbe'
+                psp_path = 'pbe'
             Z = []
             for ia in range(self.Natoms):
-                gth_dict = read_gth(self.atom[ia], xc=xc)
+                gth_dict = read_gth(self.atom[ia], psp_path=psp_path)
                 Z.append(gth_dict['Zion'])
             self.Z = np.asarray(Z)
         return
 
     def _set_cell_size(self):
-        '''Validate the a input.'''
+        """Validate the a input."""
         # Do this early on, since it is needed in many functions
         if isinstance(self.a, (int, np.integer, float, np.floating)):
             self.a = self.a * np.ones(3)
         if isinstance(self.a, (list, tuple)):
             self.a = np.asarray(self.a)
         return
 
     def _set_positions(self):
-        '''Validate the X and center input and center the system if desired.'''
+        """Validate the X and center input and center the system if desired."""
         # We need atom positions as an two-dimensional array
         self.X = np.atleast_2d(self.X)
         if isinstance(self.center, str):
             self.center = self.center.lower()
 
         # Center system such that the geometric inertia tensor will be diagonal
         # Rotate before shifting!
@@ -234,15 +238,15 @@
         if self.center is True or self.center == 'shift':
             X = self.X
             com = center_of_mass(X)
             self.X = X - (com - self.a / 2)
         return
 
     def _set_sampling(self):
-        '''Validate the s input and calculate it if necessary.'''
+        """Validate the s input and calculate it if necessary."""
         # Make sampling dependent of ecut if no sampling is given
         if self.s is None:
             try:
                 s = np.int_(self.a / cutoff2gridspacing(self.ecut))
             except TypeError:
                 self.log.exception('No ecut provided, please enter a valid s.')
                 raise
@@ -256,19 +260,19 @@
         if isinstance(self.s, (int, np.integer)):
             self.s = self.s * np.ones(3, dtype=int)
         if isinstance(self.s, (list, tuple)):
             self.s = np.asarray(self.s)
         return
 
     def _set_states(self, Nspin):
-        '''Validate the f and Nstate input and calculate the states if necessary.
+        """Validate the f and Nstate input and calculate the states if necessary.
 
         Args:
             Nspin (int | None): Number of spin states.
-        '''
+        """
         # Use a spin-paired calculation for an even number of electrons
         if Nspin is None:
             if np.sum(self.Z) % 2 == 0:
                 Nspin = 1
             else:
                 Nspin = 2
         # Make sure Nspin is an integer
@@ -305,100 +309,100 @@
             self.Nstate = int(np.ceil(Ztot / 2))
             self.f = self.f * np.ones((self.Nspin, self.Nstate))
             # Subtract the leftovers from the last spin state
             self.f[-1, -1] -= np.sum(self.Z) % 2
         return
 
     def _get_index_matrices(self):
-        '''Build index matrices M and N to build the real and reciprocal space samplings.
+        """Build index matrices M and N to build the real and reciprocal space samplings.
 
         The matrices are using C ordering (the last index is the fastest).
 
         Returns:
             tuple[ndarray, ndarray]: Index matrices.
-        '''
+        """
         # Build index matrix M
         ms = np.arange(np.prod(self.s))
         m1 = np.floor(ms / (self.s[2] * self.s[1])) % self.s[0]
         m2 = np.floor(ms / self.s[2]) % self.s[1]
         m3 = ms % self.s[2]
         M = np.column_stack((m1, m2, m3))
 
         # Build index matrix N
-        n1 = m3 - (m3 > self.s[2] / 2) * self.s[2]
+        n1 = m1 - (m1 > self.s[0] / 2) * self.s[0]
         n2 = m2 - (m2 > self.s[1] / 2) * self.s[1]
-        n3 = m1 - (m1 > self.s[0] / 2) * self.s[0]
+        n3 = m3 - (m3 > self.s[2] / 2) * self.s[2]
         N = np.column_stack((n1, n2, n3))
         return M, N
 
     def _set_cell(self, M):
-        '''Build cell and create the respective sampling.
+        """Build cell and create the respective sampling.
 
         Args:
             M (ndarray): Index matrix.
-        '''
+        """
         # Build a cuboidal cell and calculate its volume
         R = self.a * np.eye(3)
         self.R = R
         self.Omega = np.abs(det(R))
         # Build real-space sampling points
         self.r = M @ inv(np.diag(self.s)) @ R.T
         return
 
     def _set_G(self, N):
-        '''Build G-vectors, build squared magnitudes G2, and generate the active space.
+        """Build G-vectors, build squared magnitudes G2, and generate the active space.
 
         Args:
             N (ndarray): Index matrix.
-        '''
+        """
         # Build G-vectors
         G = 2 * np.pi * N @ inv(self.R)
         self.G = G
         # Calculate squared-magnitudes of G-vectors
         G2 = norm(G, axis=1)**2
         self.G2 = G2
 
         # Calculate the G2 restriction
         if self.ecut is not None:
-            active = np.nonzero(G2 <= 2 * self.ecut)
+            active = np.nonzero(2 * self.ecut >= G2)
         else:
             active = np.nonzero(G2 >= 0)  # Trivial condition to produce the right shape
         self.active = active
         self.G2c = G2[active]
 
         # Calculate the structure factor per atom
         self.Sf = np.exp(1j * G @ self.X.T).T
         return
 
     def _set_operators(self):
-        '''Set operators of an Atoms class instance at runtime.'''
+        """Set operators of an Atoms class instance at runtime."""
         for op in ('O', 'L', 'Linv', 'K', 'T'):
             setattr(type(self), op, getattr(operators, op))
         fft_operators = ('I', 'J', 'Idag', 'Jdag')
         # Use the Torch operators if desired, or the default ones otherwise
         if config.use_torch:
             from .extras import torch
             for op in fft_operators:
                 setattr(type(self), op, getattr(torch, op))
         else:
             for op in fft_operators:
                 setattr(type(self), op, getattr(operators, op))
         return
 
     def __repr__(self):
-        '''Print the parameters stored in the Atoms object.'''
-        out = 'Atom\tCharge\tPosition'
+        """Print the parameters stored in the Atoms object."""
+        out = 'Atom  Charge  Position'
         for i in range(self.Natoms):
-            out += f'\n{self.atom[i]}\t{self.Z[i]}\t' \
+            out += f'\n{self.atom[i]:>3}   {self.Z[i]:>5}   ' \
                    f'{self.X[i, 0]:10.5f}  {self.X[i, 1]:10.5f}  {self.X[i, 2]:10.5f}'
         return out
 
     @property
     def verbose(self):
-        '''Verbosity level.'''
+        """Verbosity level."""
         return self._verbose
 
     @verbose.setter
     def verbose(self, level):
         self._verbose = get_level(level)
         self.log.verbose = self._verbose
         return
```

### Comparing `eminus-2.4.0/eminus/config.py` & `eminus-2.5.0/eminus/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 #!/usr/bin/env python3
-'''Consolidated configuration module.'''
+"""Consolidated configuration module."""
 import os
 import sys
 
 from .logger import log
 
 
 class ConfigClass():
-    '''Configuration class holding user specifiable variables.
+    """Configuration class holding user specifiable variables.
 
     An instance of this class will be set as the same name as this module. This will effectively
     make this module a singleton data class.
-    '''
+    """
     def __init__(self):
+        """Initialize the ConfigClass object."""
         self.use_torch = True     # Use the faster Torch FFTs if available
         self.use_gpu = False      # Disable GPU by default, since it was slower in my tests
         self.use_pylibxc = True   # Use Libxc over PySCF if available
         self.threads = None       # Read threads from environment variables by default
         self.verbose = 'INFO'     # Only display warnings and worse by default
         return
 
     @property
     def use_torch(self):
-        '''Weather to use Torch or SciPy if Torch is installed.'''
+        """Weather to use Torch or SciPy if Torch is installed."""
         # Add the logic in the getter method so it does not run on initialization since importing
         # Torch is rather slow
         if self._use_torch:
             try:
                 import torch  # noqa: F401
                 return True
             except ImportError:
@@ -36,29 +37,29 @@
     @use_torch.setter
     def use_torch(self, value):
         self._use_torch = value
         return
 
     @property
     def use_gpu(self):
-        '''Weather to use Torch on the GPU if available.'''
+        """Weather to use Torch on the GPU if available."""
         # Only use GPU if Torch is available
         if self.use_torch and self._use_gpu:
             import torch
             return torch.cuda.is_available()
         return False
 
     @use_gpu.setter
     def use_gpu(self, value):
         self._use_gpu = value
         return
 
     @property
     def use_pylibxc(self):
-        '''Weather to use pylibxc or PySCF for functionals if both are installed.'''
+        """Weather to use pylibxc or PySCF for functionals if both are installed."""
         if self._use_pylibxc:
             try:
                 import pylibxc  # noqa: F401
                 return True
             except ImportError:
                 pass
         return False
@@ -66,15 +67,15 @@
     @use_pylibxc.setter
     def use_pylibxc(self, value):
         self._use_pylibxc = value
         return
 
     @property
     def threads(self):
-        '''Number of threads used in FFT calculations.'''
+        """Number of threads used in FFT calculations."""
         if self._threads is None:
             try:
                 if self.use_torch:
                     import torch
                     return torch.get_num_threads()
                 else:
                     # Read the OMP threads for the default operators
@@ -88,29 +89,29 @@
         self._threads = value
         if isinstance(value, int):
             if self.use_torch:
                 import torch
                 return torch.set_num_threads(value)
             else:
                 os.environ['OMP_NUM_THREADS'] = str(value)
-        return
+        return None
 
     @property
     def verbose(self):
-        '''Logger verbosity level.'''
+        """Logger verbosity level."""
         return log.verbose
 
     @verbose.setter
     def verbose(self, value):
         # Logic in setter to run it on initialization
         log.verbose = value
         return
 
     def info(self):
-        '''Print configuration and performance information.'''
+        """Print configuration and performance information."""
         print('--- Configuration infos ---')
         print(f'Global verbosity : {self.verbose}')
         # Only print if PySCF or pylibxc is installed
         if not self.use_pylibxc:
             try:
                 import pyscf  # noqa: F401
                 print('Libxc backend    : PySCF')
```

### Comparing `eminus-2.4.0/eminus/data.py` & `eminus-2.5.0/eminus/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-'''Atomic data collections.'''
+"""Atomic data collections."""
 
 # Map atom symbols and atom numbers
 SYMBOL2NUMBER = {
     'X': 0,
     'H': 1,
     'He': 2,
     'Li': 3,
```

### Comparing `eminus-2.4.0/eminus/dft.py` & `eminus-2.5.0/eminus/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,387 +1,418 @@
 #!/usr/bin/env python3
-'''Main DFT functions based on the DFT++ formulation.'''
+"""Various tools to check physical properties."""
 import numpy as np
-from numpy.random import Generator, SFC64
-from scipy.linalg import eig, eigh, eigvalsh, inv, norm, sqrtm
+from numpy.linalg import norm
+from scipy.optimize import minimize_scalar
 
-from .gth import calc_Vnonloc
-from .utils import handle_spin_gracefully, pseudo_uniform
-from .xc import get_vxc
+from .dft import get_epsilon
+from .gga import get_grad_field, get_tau
+from .logger import log
 
 
-def solve_poisson(atoms, n):
-    '''Solve the Poisson equation.
+def cutoff2gridspacing(E):
+    """Convert plane wave energy cut-off to a real-space grid spacing.
 
-    Reference: Comput. Phys. Commun. 128, 1.
+    Reference: Phys. Rev. B 54, 14362.
 
     Args:
-        atoms: Atoms object.
-        n (ndarray): Real-space electronic density.
+        E (float): Energy in Hartree.
 
     Returns:
-        ndarray: Hartree field.
-    '''
-    # phi = -4 pi Linv(O(J(n)))
-    return -4 * np.pi * atoms.Linv(atoms.O(atoms.J(n)))
+        float: Grid spacing in Bohr.
+    """
+    return np.pi / np.sqrt(2 * E)
 
 
-def get_n_total(atoms, Y, n_spin=None):
-    '''Calculate the total electronic density.
+def gridspacing2cutoff(h):
+    """Convert real-space grid spacing to plane wave energy cut-off.
 
-    Reference: Comput. Phys. Commun. 128, 1.
+    Reference: Phys. Rev. B 54, 14362.
 
     Args:
-        atoms: Atoms object.
-        Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
-
-    Keyword Args:
-        n_spin (ndarray): Real-space electronic densities per spin channel.
+        h (float): Grid spacing in Bohr.
 
     Returns:
-        ndarray: Electronic density.
-    '''
-    # Return the total density in the spin-paired case
-    if n_spin is not None:
-        return np.sum(n_spin, axis=0)
-
-    # n = (IW) F (IW)dag
-    Yrs = atoms.I(Y)
-    n = np.zeros(len(atoms.r))
-    for spin in range(atoms.Nspin):
-        n += np.sum(atoms.f[spin] * np.real(Yrs[spin].conj() * Yrs[spin]), axis=1)
-    return n
+        float: Cut-off in Hartree.
+    """
+    return 0.5 * (np.pi / h)**2
 
 
-def get_n_spin(atoms, Y, n=None):
-    '''Calculate the electronic density per spin channel.
-
-    Reference: Comput. Phys. Commun. 128, 1.
+def center_of_mass(coords, masses=None):
+    """Calculate the center of mass for a set of coordinates and masses.
 
     Args:
-        atoms: Atoms object.
-        Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
+        coords (ndarray): Array of real-space coordinates.
 
     Keyword Args:
-        n (ndarray): Real-space electronic density.
+        masses (ndarray): Mass or weight for each coordinate.
 
     Returns:
-        ndarray: Electronic densities per spin channel.
-    '''
-    # Return the total density in the spin-paired case
-    if n is not None and atoms.Nspin == 1:
-        return np.atleast_2d(n)
+        ndarray: Center of mass.
+    """
+    if masses is None:
+        masses = np.ones(len(coords))
 
-    Yrs = atoms.I(Y)
-    n = np.empty((atoms.Nspin, len(atoms.r)))
-    for spin in range(atoms.Nspin):
-        n[spin] = np.sum(atoms.f[spin] * np.real(Yrs[spin].conj() * Yrs[spin]), axis=1)
-    return n
+    return np.sum(masses * coords.T, axis=1) / np.sum(masses)
 
 
-def get_n_single(atoms, Y):
-    '''Calculate the single-electron densities.
+def orbital_center(object, psirs):
+    """Calculate the orbital center of masses, e.g., from localized orbitals.
 
     Args:
-        atoms: Atoms object.
-        Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
+        object: Atoms or SCF object.
+        psirs (ndarray): Set of orbitals in real-space.
 
     Returns:
-        ndarray: Single-electron densities.
-    '''
-    Yrs = atoms.I(Y)
-    n = np.empty((atoms.Nspin, len(atoms.r), atoms.Nstate))
+        bool: Center of masses.
+    """
+    try:
+        atoms = object.atoms
+    except AttributeError:
+        atoms = object
+
+    coms = [np.array([])] * 2
+    Ncom = psirs.shape[2]
     for spin in range(atoms.Nspin):
-        n[spin] = atoms.f[spin] * np.real(Yrs[spin].conj() * Yrs[spin])
-    return n
+        coms_spin = np.empty((Ncom, 3))
+
+        # Square orbitals
+        psi2 = np.real(psirs[spin].conj() * psirs[spin])
+        for i in range(Ncom):
+            coms_spin[i] = center_of_mass(atoms.r, psi2[:, i])
+        coms[spin] = coms_spin
+    return coms
 
 
-def get_grad_n_spin(atoms, n_spin):
-    '''Calculate the gradient of densities per spin channel.
+def inertia_tensor(coords, masses=None):
+    """Calculate the inertia tensor for a set of coordinates and masses.
+
+    Reference: https://en.wikipedia.org/wiki/Moment_of_inertia
 
     Args:
-        atoms: Atoms object.
-        n_spin (ndarray): Real-space electronic densities per spin channel.
+        coords (ndarray): Array of real-space coordinates.
+
+    Keyword Args:
+        masses (ndarray): Mass or weight for each coordinate.
 
     Returns:
-        ndarray: Gradients of densities per spin channel.
-    '''
-    dn_spin = np.empty((atoms.Nspin, len(atoms.r), 3))
-    for spin in range(atoms.Nspin):
-        Gn = 1j * atoms.G * atoms.J(n_spin[spin])[:, None]
-        for i in range(3):
-            dn_spin[spin, :, i] = np.real(atoms.I(Gn[:, i]))
-    return dn_spin
+        ndarray: Inertia tensor.
+    """
+    if masses is None:
+        masses = np.ones(len(coords))
+
+    # The inertia tensor for a set of point masses can be calculated with simple summation
+    # https://en.wikipedia.org/wiki/Moment_of_inertia#Definition_2
+    I = np.empty((3, 3))
+    I[0, 0] = np.sum(masses * (coords[:, 1]**2 + coords[:, 2]**2))
+    I[1, 1] = np.sum(masses * (coords[:, 0]**2 + coords[:, 2]**2))
+    I[2, 2] = np.sum(masses * (coords[:, 0]**2 + coords[:, 1]**2))
+
+    I[0, 1] = I[1, 0] = -np.sum(masses * (coords[:, 0] * coords[:, 1]))
+    I[0, 2] = I[2, 0] = -np.sum(masses * (coords[:, 0] * coords[:, 2]))
+    I[1, 2] = I[2, 1] = -np.sum(masses * (coords[:, 1] * coords[:, 2]))
+    return I
+
 
+def get_dipole(scf, n=None):
+    """Calculate the electric dipole moment.
 
-@handle_spin_gracefully
-def orth(atoms, W):
-    '''Orthogonalize coefficient matrix W.
+    This function does not account for periodcity, it may be a good idea to center the system.
 
-    Reference: Comput. Phys. Commun. 128, 1.
+    Reference: J. Chem. Phys. 155, 224109.
 
     Args:
-        atoms: Atoms object.
-        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
+        scf: SCF object.
+
+    Keyword Args:
+        n (float): Real-space electronic density.
 
     Returns:
-        ndarray: Orthogonalized wave functions.
-    '''
-    # Y = W (Wdag O(W))^-0.5
-    return W @ inv(sqrtm(W.conj().T @ atoms.O(W)))
+        ndarray: Electric dipole moment in e * Bohr.
+    """
+    atoms = scf.atoms
+    if n is None:
+        n = scf.n
+    if scf.n is None:
+        log.error('There is no density to calculate a dipole.')
+        return 0
+
+    # Diple moment: mu = \sum Z X - \int n(r) r dr
+    mu = np.array([0, 0, 0], dtype=float)
+    for i in range(atoms.Natoms):
+        mu += atoms.Z[i] * atoms.X[i]
+
+    dV = atoms.Omega / np.prod(atoms.s)
+    for dim in range(3):
+        mu[dim] -= dV * np.sum(n * atoms.r[:, dim])
+    return mu
 
 
-def get_grad(scf, spin, W, *args, **kwargs):
-    '''Calculate the energy gradient with respect to W.
+def get_ip(scf):
+    """Calculate the ionization potential by calculating the negative HOMO energy.
 
-    Reference: Comput. Phys. Commun. 128, 1.
+    Reference: Physica 1, 104.
 
     Args:
         scf: SCF object.
-        spin (int): Spin variable to track weather to calculate the gradient for spin up or down.
-        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
-        ndarray: Gradient.
-    '''
-    atoms = scf.atoms
-    F = np.diag(atoms.f[spin])
-    HW = H(scf, spin, W, *args, **kwargs)
-    WHW = W[spin].conj().T @ HW
-    # U = Wdag O(W)
-    OW = atoms.O(W[spin])
-    U = W[spin].conj().T @ OW
-    invU = inv(U)
-    U12 = sqrtm(invU)
-    # Htilde = U^-0.5 Wdag H(W) U^-0.5
-    Ht = U12 @ WHW @ U12
-    # grad E = H(W) - O(W) U^-1 (Wdag H(W)) (U^-0.5 F U^-0.5) + O(W) (U^-0.5 Q(Htilde F - F Htilde))
-    return (HW - (OW @ invU) @ WHW) @ (U12 @ F @ U12) + OW @ (U12 @ Q(Ht @ F - F @ Ht, U))
-
+        float: Ionization potential in Hartree.
+    """
+    epsilon = get_epsilon(scf, scf.W)
+    # Add up spin states
+    epsilon = np.sum(epsilon, axis=0)
+    return -epsilon[-1]
 
-def H(scf, spin, W, Y=None, n=None, n_spin=None, dn_spin=None, phi=None, vxc=None, vsigma=None):
-    '''Left-hand side of the eigenvalue equation.
 
-    Reference: Comput. Phys. Commun. 128, 1.
+def check_ortho(object, func, eps=1e-9):
+    """Check the orthogonality condition for a set of functions.
 
     Args:
-        scf: SCF object.
-        spin (int): Spin variable to track weather to calculate the gradient for spin up or down.
-        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
+        object: Atoms or SCF object.
+        func (ndarray): Discretized set of functions.
 
     Keyword Args:
-        Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
-        n (ndarray): Real-space electronic density.
-        n_spin (ndarray): Real-space electronic densities per spin channel.
-        dn_spin (ndarray): Real-space gradient of densities per spin channel.
-        phi (ndarray): Hartree field.
-        vxc (ndarray): Exchange-correlation potential.
-        vsigma (ndarray): Contracted gradient potential derivative.
+        eps (float): Tolerance for the condition.
 
     Returns:
-        ndarray: Hamiltonian applied on W.
-    '''
-    atoms = scf.atoms
-    # One can calculate everything from W,
-    # but one can also use already computed results to save time
-    if Y is None:
-        Y = orth(atoms, W)
-    if n_spin is None:
-        n_spin = get_n_spin(atoms, Y, n)
-    if dn_spin is None and scf.psp == 'pbe':
-        dn_spin = get_grad_n_spin(atoms, n_spin)
-    if n is None:
-        n = get_n_total(atoms, Y, n_spin)
-    if phi is None:
-        phi = solve_poisson(atoms, n)
-    if vxc is None or (vsigma is None and scf.psp == 'pbe'):
-        vxc, vsigma = get_vxc(scf.xc, n_spin, atoms.Nspin, dn_spin)
-
-    # We get the full potential in the functional definition (different to the DFT++ notation)
-    # Applay the gradient correction to the potential if a GGA functional is used
-    if scf.psp == 'pbe':
-        vxc = gradient_correction(atoms, dn_spin, vxc, vsigma)
-    # Normally Vxc = Jdag(O(J(exc))) + diag(exc') Jdag(O(J(n)))
-    Vxc = atoms.Jdag(atoms.O(atoms.J(vxc[spin])))
-    # Vkin = -0.5 L(W)
-    Vkin_psi = -0.5 * atoms.L(W[spin])
-    # Veff = Jdag(Vion) + Jdag(O(J(vxc))) + Jdag(O(phi))
-    Veff = scf.Vloc + Vxc + atoms.Jdag(atoms.O(phi))
-    Vnonloc_psi = calc_Vnonloc(scf, W[spin])
-    # H = Vkin + Idag(diag(Veff))I + Vnonloc
-    # Diag(a) * B can be written as a * B if a is a column vector
-    return Vkin_psi + atoms.Idag(Veff[:, None] * atoms.I(W[spin])) + Vnonloc_psi
-
-
-def gradient_correction(atoms, dn_spin, vxc, vsigma):
-    '''Calculate the gradient corrected exchange-correlation potential.
-
-    Reference: Chem. Phys. Lett. 199, 557.
-
-    Args:
-        atoms: Atoms object.
-        dn_spin (ndarray): Real-space gradient of densities per spin channel.
-        vxc (ndarray): Exchange-correlation potential.
-        vsigma (ndarray): Contracted gradient potential derivative.
-
-    Returns:
-        ndarray: Gradient corrected potential.
-    '''
-    # sigma is |dn|^2, while vsigma is n * d exc/d sigma
-    h = np.zeros_like(dn_spin)
-    if atoms.Nspin == 1:
-        # In the unpolarized case we have no spin mixing and only one spin density
-        h[0] = 2 * vsigma[0][:, None] * dn_spin[0]
-    else:
-        # In the polarized case we would get for spin up (and similar for spin down)
-        # Vxc_u = vxc_u - Nabla dot (2 vsigma_uu * dn_u + vsigma_ud * dn_d)
-        # h is the expression in the brackets
-        h[0] = 2 * vsigma[0][:, None] * dn_spin[0] + vsigma[1][:, None] * dn_spin[1]
-        h[1] = 2 * vsigma[2][:, None] * dn_spin[1] + vsigma[1][:, None] * dn_spin[0]
-
-    # Calculate Nabla dot h
-    divh = np.zeros_like(vxc)
+        bool: Orthogonality status for the set of functions.
+    """
+    func = np.atleast_3d(func)
+    try:
+        atoms = object.atoms
+    except AttributeError:
+        atoms = object
+    # It makes no sense to calculate anything for only one function
+    if atoms.Nstate == 1:
+        log.warning('Need at least two functions to check their orthogonality.')
+        return True
+
+    # We integrate over our cell, the integration borders then become a=0 and b=cell length
+    # The integration prefactor dV is (b-a)/n, with n as the sampling
+    # For a 3d integral we have to multiply for every direction
+    dV = atoms.Omega / np.prod(atoms.s)
+
+    ortho_bool = True
+    # Check the condition for every combination
+    # Orthogonality condition: \int func1^* func2 dr = 0
     for spin in range(atoms.Nspin):
-        Gh = np.empty((len(atoms.G2), 3), dtype=complex)
-        for i in range(3):
-            Gh[:, i] = atoms.J(h[spin, :, i])
-        Gdivh = 1j * np.sum(atoms.G * Gh, axis=1)
-        divh[spin] = np.real(atoms.I(Gdivh))
+        for i in range(atoms.Nstate):
+            for j in range(i + 1, atoms.Nstate):
+                res = dV * np.sum(func[spin, :, i].conj() * func[spin, :, j])
+                tmp_bool = abs(res) < eps
+                ortho_bool *= tmp_bool
+                log.debug(f'Function {i} and {j}:\nValue: {res:.7f}\nOrthogonal: {tmp_bool}')
+    log.info(f'Orthogonal: {ortho_bool}')
+    return ortho_bool
 
-    # Subtract the gradient correction
-    return vxc - divh
 
+def check_norm(object, func, eps=1e-9):
+    """Check the normalization condition for a set of functions.
 
-def Q(inp, U):
-    '''Operator needed to calculate gradients with non-constant occupations.
+    Args:
+        object: Atoms or SCF object.
+        func (ndarray): Discretized set of functions.
+
+    Keyword Args:
+        eps (float): Tolerance for the condition.
+
+    Returns:
+        bool: Normalization status for the set of functions.
+    """
+    func = np.atleast_3d(func)
+    try:
+        atoms = object.atoms
+    except AttributeError:
+        atoms = object
+    # We integrate over our cell, the integration borders then become a=0 and b=cell length
+    # The integration prefactor dV is (b-a)/n, with n as the sampling
+    # For a 3d integral we have to multiply for every direction
+    dV = atoms.Omega / np.prod(atoms.s)
+
+    norm_bool = True
+    # Check the condition for every function
+    # Normality condition: \int func^* func dr = 1
+    for spin in range(atoms.Nspin):
+        for i in range(atoms.Nstate):
+            res = dV * np.sum(func[spin, :, i].conj() * func[spin, :, i])
+            tmp_bool = abs(1 - res) < eps
+            norm_bool *= tmp_bool
+            log.debug(f'Function {i}:\nValue: {res:.7f}\nNormalized: {tmp_bool}')
+    log.info(f'Normalized: {norm_bool}')
+    return norm_bool
 
-    Reference: Comput. Phys. Commun. 128, 1.
+
+def check_orthonorm(object, func):
+    """Check the orthonormality conditions for a set of functions.
 
     Args:
-        inp (ndarray): Coefficients input array.
-        U (ndarray): Overlap of wave functions.
+        object: Atoms or SCF object.
+        func (ndarray): Discretized set of functions.
 
     Returns:
-        ndarray: Q operator result.
-    '''
-    mu, V = eig(U)
-    mu = mu[:, None]
-    denom = np.sqrt(mu) @ np.ones((1, len(mu)))
-    denom2 = denom + denom.conj().T
-    return V @ ((V.conj().T @ inp @ V) / denom2) @ V.conj().T
+        bool: Orthonormality status for the set of functions.
+    """
+    try:
+        atoms = object.atoms
+    except AttributeError:
+        atoms = object
+    ortho_bool = check_ortho(atoms, func)
+    norm_bool = check_norm(atoms, func)
+    log.info(f'Orthonormal: {ortho_bool * norm_bool}')
+    return ortho_bool * norm_bool
 
 
-def get_psi(scf, W, n=None):
-    '''Calculate eigenstates from H.
+def get_isovalue(n, percent=85):
+    """Find an isovalue that contains a percentage of the electronic density.
 
-    Reference: Comput. Phys. Commun. 128, 1.
+    Reference: J. Chem. Phys. 158, 164102.
 
     Args:
-        scf: SCF object.
-        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
+        n (float): Real-space electronic density.
 
     Keyword Args:
-        n (ndarray): Real-space electronic density.
+        percent (float): Amount of density that should be contained.
 
     Returns:
-        ndarray: Eigenstates in reciprocal space.
-    '''
-    atoms = scf.atoms
-    Y = orth(atoms, W)
-    psi = np.empty_like(Y)
-    for spin in range(atoms.Nspin):
-        mu = Y[spin].conj().T @ H(scf, spin, W=Y, n=n)
-        _, D = eigh(mu)
-        psi[spin] = Y[spin] @ D
-    return psi
+        float: Isovalue that contains the specified percentage of the density.
+    """
+    def deviation(isovalue):
+        """Wrapper function for finding the isovalue by minimization."""
+        n_mask = np.sum(n[n > isovalue])
+        return abs(percent - (n_mask / n_ref) * 100)
+
+    # Integrated density
+    n_ref = np.sum(n)
+    # Finding the isovalue is an optimization problem, minimizing the deviation above
+    # The problem is bound by zero (no density) and the maximum value in n
+    res = minimize_scalar(deviation, bounds=(0, np.max(n)), method='bounded')
+    return res.x
 
 
-def get_epsilon(scf, W, n=None):
-    '''Calculate eigenvalues from H.
+def get_tautf(scf):
+    """Calculate the Thomas-Fermi kinetic energy densities per spin.
 
-    Reference: Comput. Phys. Commun. 128, 1.
+    Reference: Phys. Lett. B 63, 395.
 
     Args:
         scf: SCF object.
-        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
-
-    Keyword Args:
-        n (ndarray): Real-space electronic density.
 
     Returns:
-        ndarray: Eigenvalues.
-    '''
+        ndarray: Real space Thomas-Fermi kinetic energy density.
+    """
     atoms = scf.atoms
-    Y = orth(atoms, W)
-    epsilon = np.empty((atoms.Nspin, atoms.Nstate))
-    for spin in range(atoms.Nspin):
-        mu = Y[spin].conj().T @ H(scf, spin, W=Y, n=n)
-        epsilon[spin] = np.sort(eigvalsh(mu))
-    return epsilon
+    # Use the definition with a division by two
+    tautf = 3 / 10 * (atoms.Nspin * 3 * np.pi**2)**(2 / 3) * scf.n_spin**(5 / 3)
+
+    log.debug(f'Calculated Ekin:  {scf.energies.Ekin:.6f} Eh')
+    log.debug(f'Integrated tautf: {np.sum(tautf) * atoms.Omega / np.prod(atoms.s):.6f} Eh')
+    return tautf
 
 
-def guess_random(scf, complex=True):
-    '''Generate random initial-guess coefficients as starting values.
+def get_tauw(scf):
+    """Calculate the von Weizsaecker kinetic energy densities per spin.
+
+    Reference: Z. Phys. 96, 431.
 
     Args:
         scf: SCF object.
 
-    Keyword Args:
-        complex (bool): Use complex numbers for the random guess.
-
     Returns:
-        ndarray: Initial-guess orthogonal wave functions in reciprocal space.
-    '''
+        ndarray: Real space von Weizsaecker kinetic energy density.
+    """
     atoms = scf.atoms
-
-    seed = 42
-    rng = Generator(SFC64(seed))
-    if complex:
-        W = rng.standard_normal((atoms.Nspin, len(atoms.G2c), atoms.Nstate)) + \
-            1j * rng.standard_normal((atoms.Nspin, len(atoms.G2c), atoms.Nstate))
+    if scf.dn_spin is None:
+        dn_spin = get_grad_field(atoms, scf.n_spin)
     else:
-        W = rng.standard_normal((atoms.Nspin, len(atoms.G2c), atoms.Nstate))
-    return orth(atoms, W)
+        dn_spin = scf.dn_spin
+    dn2 = norm(dn_spin, axis=2)**2
+    # Use the definition with a division by two
+    tauw = dn2 / (8 * scf.n_spin)
+
+    # For one- and two-electron systems the integrated KED has to be the same as the calculated KE
+    log.debug(f'Calculated Ekin: {scf.energies.Ekin:.6f} Eh')
+    log.debug(f'Integrated tauw: {np.sum(tauw) * atoms.Omega / np.prod(atoms.s):.6f} Eh')
+    return tauw
 
 
-def guess_gaussian(scf, complex=True):
-    '''Generate initial-guess coefficients using normalized Gaussians as starting values.
+def get_elf(scf):
+    """Calculate the electron localization function.
+
+    Reference: J. Chem. Phys. 92, 5397.
 
     Args:
         scf: SCF object.
 
-    Keyword Args:
-        complex (bool): Use complex numbers for the random guess.
+    Returns:
+        ndarray: Real space electron localization function.
+    """
+    D = get_tau(scf.atoms, scf.Y) - get_tauw(scf)
+    D0 = get_tautf(scf)
+    X = D / D0
+    return 1 / (1 + X**2)
+
+
+def get_reduced_gradient(scf, eps=0):
+    """Calculate the reduced density gradient s.
+
+    Reference: Phys. Rev. Lett. 78, 1396.
+
+    Args:
+        scf: SCF object.
+
+    Kwargs:
+        eps (float): Threshold of the density where s should be truncated.
 
     Returns:
-        ndarray: Initial-guess orthogonal wave functions in reciprocal space.
-    '''
+        ndarray: Real space educed density gradient.
+    """
     atoms = scf.atoms
-    # Start with randomized wave functions
-    W = guess_random(scf, complex=complex)
+    if scf.dn_spin is None:
+        dn_spin = get_grad_field(atoms, scf.n_spin)
+    else:
+        dn_spin = scf.dn_spin
+    norm_dn = norm(np.sum(dn_spin, axis=0), axis=1)
 
-    sigma = 0.5
-    normal = (2 * np.pi * sigma**2)**(3 / 2)
-    # Calculate a density from normalized Gauss functions
-    n = np.zeros(len(atoms.r)) + 1e-15  # Add a small epsilon to prevent divisions by zero in exc
-    for ia in range(atoms.Natoms):
-        r = norm(atoms.r - atoms.X[ia], axis=1)
-        n += atoms.Z[ia] * np.exp(-r**2 / (2 * sigma**2)) / normal
-    # Calculate the eigenfunctions
-    return get_psi(scf, W, n)
+    kf = (3 * np.pi**2 * scf.n)**(1 / 3)
+    with np.errstate(divide='ignore', invalid='ignore'):
+        s = norm_dn / (2 * kf * scf.n)
+    s[scf.n < eps] = 0
+    return s
 
 
-def guess_pseudo(scf, seed=1234):
-    '''Generate initial-guess coefficients using pseudo-random starting values.
+def get_spin_squared(scf):
+    """Calculate the expectation value of the squared spin operator <S^2>.
+
+    Reference: Appl. Phys. Express 12, 115506.
 
     Args:
         scf: SCF object.
 
-    Keyword Args:
-        seed (int): Seed to initialize the random number generator.
-
     Returns:
-        ndarray: Initial-guess orthogonal wave functions in reciprocal space.
-    '''
+        float: The DFT value for <S^2>.
+    """
     atoms = scf.atoms
-    W = pseudo_uniform((atoms.Nspin, len(atoms.G2c), atoms.Nstate), seed=seed)
-    return orth(atoms, W)
+    # <S^2> for a restricted calculation is always zero
+    if atoms.Nspin == 1:
+        return 0
+
+    rhoXr = scf.n_spin[0] - scf.n_spin[1]
+    rhoXr[rhoXr < 0] = 0
+    rhoX = np.sum(rhoXr) * atoms.Omega / np.prod(atoms.s)
+    SX = 0.5 * (np.sum(scf.n_spin[0]) - np.sum(scf.n_spin[1])) * atoms.Omega / np.prod(atoms.s)
+    return SX * (SX + 1) + rhoX
+
+
+def get_multiplicity(scf):
+    """Calculate the multiplicity from <S^2>.
+
+    Args:
+        scf: SCF object.
+
+    Returns:
+        float: Multiplicity 2S+1.
+    """
+    S2 = get_spin_squared(scf)
+    # <S^2> = S(S+1) = S^2+S+0.25-0.25 = (S+0.5)^2-0.25 => S = sqrt(<S^2>+0.25)-0.5
+    S = np.sqrt(S2 + 0.25) - 0.5
+    return 2 * S + 1
```

### Comparing `eminus-2.4.0/eminus/domains.py` & `eminus-2.5.0/eminus/domains.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 #!/usr/bin/env python3
-'''Functions to generate masks to restrict real-space fields to domains.'''
+"""Functions to restrict real-space fields to domains."""
 import numpy as np
 from scipy.linalg import norm
 
 from .tools import center_of_mass
 
 
 def domain_cuboid(object, length, centers=None):
-    '''Generate a mask for a cuboidal real-space domain.
+    """Generate a mask for a cuboidal real-space domain.
 
     Args:
         object: Atoms or SCF object.
         length (int | float | list | ndarray): Side length or lengths of the cuboid.
 
     Keyword Args:
         centers (ndarray): Center of the cuboid.
 
             Defaults to the geometric center of mass of the system. For multiple coordinates,
             multiple domains will be merged.
 
     Returns:
         ndarray: Boolean mask.
-    '''
+    """
     try:
         atoms = object.atoms
     except AttributeError:
         atoms = object
 
     if isinstance(length, (int, float)):
         length = length * np.ones(3)
     if centers is None:
         centers = center_of_mass(atoms.X)
-    centers = np.asanyarray(centers)
+    centers = np.asarray(centers)
     # Handle each dimension seperately and add them together
     if centers.ndim == 1:
         mask1 = np.abs(centers[0] - atoms.r[:, 0]) < length[0]
         mask2 = np.abs(centers[1] - atoms.r[:, 1]) < length[1]
         mask3 = np.abs(centers[2] - atoms.r[:, 2]) < length[2]
         mask = mask1 & mask2 & mask3
     else:
@@ -45,68 +45,68 @@
             mask2 = np.abs(center[1] - atoms.r[:, 1]) < length[1]
             mask3 = np.abs(center[2] - atoms.r[:, 2]) < length[2]
             mask = mask | (mask1 & mask2 & mask3)
     return mask
 
 
 def domain_isovalue(field, isovalue):
-    '''Generate a mask for an isovalue real-space domain.
+    """Generate a mask for an isovalue real-space domain.
 
     Args:
         field (ndarray): Real-space field data.
         isovalue (float): Isovalue for the truncation.
 
     Returns:
         ndarray: Boolean mask.
-    '''
+    """
     return np.abs(field) > isovalue
 
 
 def domain_sphere(object, radius, centers=None):
-    '''Generate a mask for a spherical real-space domain.
+    """Generate a mask for a spherical real-space domain.
 
     Args:
         object: Atoms or SCF object.
         radius (float): Radius of the sphere.
 
     Keyword Args:
         centers (ndarray): Center of the sphere.
 
             Defaults to the geometric center of mass of the system. For multiple coordinates,
             multiple domains will be merged.
 
     Returns:
         ndarray: Boolean mask.
-    '''
+    """
     try:
         atoms = object.atoms
     except AttributeError:
         atoms = object
 
     if centers is None:
         centers = center_of_mass(atoms.X)
-    centers = np.asanyarray(centers)
+    centers = np.asarray(centers)
     if centers.ndim == 1:
         mask = norm(centers - atoms.r, axis=1) < radius
     else:
         mask = np.zeros(len(atoms.r), dtype=bool)
         for center in centers:
             mask_tmp = norm(center - atoms.r, axis=1) < radius
             mask = mask | mask_tmp
     return mask
 
 
 def truncate(field, mask):
-    '''Truncate field data for a given mask.
+    """Truncate field data for a given mask.
 
     This will not return a smaller array but set all truncated values to zero.
 
     Args:
         field (ndarray): Real-space field data.
         mask (ndarray): Boolean mask.
 
     Returns:
         ndarray: Boolean mask.
-    '''
+    """
     field_trunc = np.copy(field)
     field_trunc[~mask] = 0
     return field_trunc
```

### Comparing `eminus-2.4.0/eminus/energies.py` & `eminus-2.5.0/eminus/energies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,158 +1,158 @@
 #!/usr/bin/env python3
-'''Calculate different energy contributions.'''
+"""Calculate different energy contributions."""
 import dataclasses
 
 import numpy as np
 from scipy.linalg import inv, norm
 from scipy.special import erfc
 
-from .dft import get_grad_n_spin, get_n_single, solve_poisson
+from .dft import get_grad_field, get_n_single, solve_poisson
+from .gga import get_tau
 from .xc import get_exc
 
 
 @dataclasses.dataclass
 class Energy:
-    '''Energy class to save energy contributions in one place.'''
+    """Energy class to save energy contributions in one place."""
     Ekin: float = 0     #: Kinetic energy.
     Ecoul: float = 0    #: Coulomb energy.
     Exc: float = 0      #: Exchange-correlation energy.
     Eloc: float = 0     #: Local energy.
     Enonloc: float = 0  #: Non-local energy.
     Eewald: float = 0   #: Ewald energy.
     Esic: float = 0     #: Self-interaction correction energy.
 
     @property
     def Etot(self):
-        '''Total energy is the sum of all energy contributions.'''
+        """Total energy is the sum of all energy contributions."""
         return sum(getattr(self, ie.name) for ie in dataclasses.fields(self))
 
     def __repr__(self):
-        '''Print the energies stored in the Energy object.'''
+        """Print the energies stored in the Energy object."""
         out = ''
         for ie in dataclasses.fields(self):
             energy = getattr(self, ie.name)
             if energy != 0:
-                out += f'{ie.name.ljust(8)}: {energy:+.9f} Eh\n'
+                out += f'{ie.name:<8}: {energy:+.9f} Eh\n'
         return f'{out}{"-" * 25}\nEtot    : {self.Etot:+.9f} Eh'
 
 
 def get_E(scf):
-    '''Calculate energy contributions and update energies needed in one SCF step.
+    """Calculate energy contributions and update energies needed in one SCF step.
 
     Args:
         scf: SCF object.
 
     Returns:
         float: Total energy.
-    '''
+    """
     scf.energies.Ekin = get_Ekin(scf.atoms, scf.Y)
     scf.energies.Ecoul = get_Ecoul(scf.atoms, scf.n, scf.phi)
-    scf.energies.Exc = get_Exc(scf, scf.n, scf.exc, scf.atoms.Nspin)
+    scf.energies.Exc = get_Exc(scf, scf.n, scf.exc, Nspin=scf.atoms.Nspin)
     scf.energies.Eloc = get_Eloc(scf, scf.n)
     scf.energies.Enonloc = get_Enonloc(scf, scf.Y)
     return scf.energies.Etot
 
 
 def get_Ekin(atoms, Y):
-    '''Calculate the kinetic energy.
+    """Calculate the kinetic energy.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
 
     Returns:
         float: Kinetic energy in Hartree.
-    '''
+    """
     # Ekin = -0.5 Tr(F Wdag L(W))
     Ekin = 0
     for spin in range(atoms.Nspin):
         F = np.diag(atoms.f[spin])
         Ekin += -0.5 * np.trace(F @ Y[spin].conj().T @ atoms.L(Y[spin]))
     return np.real(Ekin)
 
 
 def get_Ecoul(atoms, n, phi=None):
-    '''Calculate the Coulomb energy.
+    """Calculate the Coulomb energy.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
-        phi (ndarray): Hartree ﬁeld.
+        phi (ndarray): Hartree field.
 
     Returns:
         float: Coulomb energy in Hartree.
-    '''
+    """
     if phi is None:
         phi = solve_poisson(atoms, n)
     # Ecoul = 0.5 (J(n))dag O(phi)
     return np.real(0.5 * n @ atoms.Jdag(atoms.O(phi)))
 
 
-def get_Exc(scf, n, exc=None, n_spin=None, dn_spin=None, Nspin=2):
-    '''Calculate the exchange-correlation energy.
+def get_Exc(scf, n, exc=None, n_spin=None, dn_spin=None, tau=None, Nspin=2):
+    """Calculate the exchange-correlation energy.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         scf: SCF object.
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
         exc (ndarray): Exchange-correlation energy density.
         n_spin (ndarray): Real-space electronic densities per spin channel.
         dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        tau (ndarray): Real-space kinetic energy densities per spin channel.
         Nspin (int): Number of spin states.
 
     Returns:
         float: Exchange-correlation energy in Hartree.
-    '''
+    """
     atoms = scf.atoms
     if exc is None:
-        if dn_spin is None and scf.psp == 'pbe':
-            dn_spin = get_grad_n_spin(atoms, n_spin)
-        exc = get_exc(scf.xc, n_spin, Nspin, dn_spin)
+        exc = get_exc(scf.xc, n_spin, Nspin, dn_spin, tau)
     # Exc = (J(n))dag O(J(exc))
     return np.real(n @ atoms.Jdag(atoms.O(atoms.J(exc))))
 
 
 def get_Eloc(scf, n):
-    '''Calculate the local energy contribution.
+    """Calculate the local energy contribution.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         scf: SCF object.
         n (ndarray): Real-space electronic density.
 
     Returns:
         float: Local energy contribution in Hartree.
-    '''
+    """
     return np.real(scf.Vloc.conj().T @ n)
 
 
 # Adapted from https://github.com/f-fathurrahman/PWDFT.jl/blob/master/src/calc_energies.jl
 def get_Enonloc(scf, Y):
-    '''Calculate the non-local GTH energy contribution.
+    """Calculate the non-local GTH energy contribution.
 
     Reference: Phys. Rev. B 54, 1703.
 
     Args:
         scf: SCF object.
         Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
 
     Returns:
         float: Non-local GTH energy contribution in Hartree.
-    '''
+    """
     atoms = scf.atoms
 
     Enonloc = 0
     if scf.NbetaNL > 0:  # Only calculate non-local potential if necessary
         for spin in range(atoms.Nspin):
             betaNL_psi = (Y[spin].conj().T @ scf.betaNL).conj()
 
@@ -169,40 +169,33 @@
                                 enl += hij * betaNL_psi[:, ibeta].conj() * betaNL_psi[:, jbeta]
             Enonloc += np.sum(atoms.f[spin] * enl)
     # We have to multiply with the cell volume, because of different orthogonalization methods
     return np.real(Enonloc * atoms.Omega)
 
 
 def get_Eewald(atoms, gcut=2, gamma=1e-8):
-    '''Calculate the Ewald energy.
+    """Calculate the Ewald energy.
 
     Reference: J. Chem. Theory Comput. 10, 381.
 
     Args:
         atoms: Atoms object.
 
     Keyword Args:
         gcut (float): G-vector cut-off.
         gamma (float): Error tolerance.
 
     Returns:
         float: Ewald energy in Hartree.
-    '''
+    """
     # For a plane wave code we have multiple contributions for the Ewald energy
     # Namely, a sum from contributions from real-space, reciprocal space,
     # the self energy, (the dipole term [neglected]), and an additional electroneutrality term
     def get_index_vectors(s):
-        '''Create all index vectors of periodic images.
-
-        Args:
-            s (ndarray): Number of images per lattice vector.
-
-        Returns:
-            ndarray: Index matrix.
-        '''
+        """Create index vectors of s periodic images."""
         m1 = np.arange(-s[0], s[0] + 1)
         m2 = np.arange(-s[1], s[1] + 1)
         m3 = np.arange(-s[2], s[2] + 1)
         M = np.transpose(np.meshgrid(m1, m2, m3)).reshape(-1, 3)
         # Delete the [0, 0, 0] element, to prevent checking for it in every loop
         return M[~np.all(M == 0, axis=1)]
 
@@ -256,43 +249,61 @@
             GX = np.sum(G * dX, axis=1)
             # Add the reciprocal space contribution
             Eewald += ZiZj * np.sum(prefactor * np.cos(GX))
     return Eewald
 
 
 def get_Esic(scf, Y, n_single=None):
-    '''Calculate the Perdew-Zunger self-interaction energy.
+    """Calculate the Perdew-Zunger self-interaction energy.
 
     Reference: Phys. Rev. B 23, 5048.
 
     Args:
         scf: SCF object.
         Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
 
     Keyword Args:
         n_single (ndarray): Single-electron densities.
 
     Returns:
         float: PZ self-interaction energy.
-    '''
+    """
     atoms = scf.atoms
     # E_PZ-SIC = \sum_i Ecoul[n_i] + Exc[n_i, 0]
     if n_single is None:
         n_single = get_n_single(atoms, Y)
 
     Esic = 0
     for i in range(atoms.Nstate):
         for spin in range(atoms.Nspin):
             if atoms.f[spin, i] > 0:
                 # Create normalized single-particle densities in the form of electronic densities
                 # per spin channel, since spin-polarized functionals expect this form
-                ni = np.zeros((2, len(n_single[0])))
+                ni = np.zeros((2, len(atoms.r)))
                 # Normalize single-particle densities to 1
                 ni[0] = n_single[spin, :, i] / atoms.f[spin, i]
 
+                # Get the gradient of the single-particle density
+                if 'gga' in scf.xc_type:
+                    dni = np.zeros((2, len(atoms.r), 3))
+                    dni[0] = get_grad_field(atoms, ni)[0]
+                else:
+                    dni = None
+
+                # Get the kinetic energy density of the corresponding orbital
+                if scf.xc_type == 'meta-gga':
+                    # Use only one orbital for the calculation
+                    Ytmp = np.zeros_like(Y)
+                    Ytmp[0, :, 0] = Y[spin, :, i]
+                    taui = np.zeros_like(ni)
+                    # We also have to normalize to one again
+                    taui[0] = get_tau(atoms, Y)[0] / atoms.f[spin, i]
+                else:
+                    taui = None
+
                 coul = get_Ecoul(atoms, ni[0])
                 # The exchange part for a SIC correction has to be spin-polarized
-                xc = get_Exc(scf, ni[0], n_spin=ni, Nspin=2)
+                xc = get_Exc(scf, ni[0], n_spin=ni, dn_spin=dni, tau=taui, Nspin=2)
                 # SIC energy is scaled by the occupation number
                 Esic += (coul + xc) * atoms.f[spin, i]
     scf.energies.Esic = Esic
     return Esic
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eminus-2.4.0/eminus/extras/__init__.py` & `eminus-2.5.0/eminus/extras/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
-'''Extra functions that need additional dependencies to work.
+"""Extra functions that need additional dependencies to work.
 
 To also install all additional dependencies, use::
 
     pip install eminus[all]
 
 Alternativle, you can only install selected extras using the respective name:
 
 * :mod:`~eminus.extras.fods`
 * :mod:`~eminus.extras.libxc`
 * :mod:`~eminus.extras.torch`
 * :mod:`~eminus.extras.viewer`
-'''
+"""
 from .fods import get_fods, remove_core_fods, split_fods
 from .libxc import libxc_functional
 from .viewer import view, view_atoms, view_file
 
 __all__ = ['get_fods', 'libxc_functional', 'remove_core_fods', 'split_fods', 'view', 'view_atoms',
            'view_file']
```

### Comparing `eminus-2.4.0/eminus/extras/fods.py` & `eminus-2.5.0/eminus/extras/fods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
-'''Fermi-orbital descriptor generation.'''
+"""Fermi-orbital descriptor generation."""
 import numpy as np
 from scipy.linalg import norm
 
 from ..data import SYMBOL2NUMBER
 from ..logger import log
 from ..units import bohr2ang
 
 
 def get_localized_orbitals(mf, Nspin, loc, Nit=1000, seed=1234):
-    '''Generate localized orbitals with an additional simple stability analysis.
+    """Generate localized orbitals with an additional simple stability analysis.
 
     Same as implemented in PyFLOSIC2.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         mf: PySCF SCF object.
@@ -22,15 +22,15 @@
 
     Keyword Args:
         Nit (int): Number of tries to get a solution with positive eigenvalues.
         seed (int): Seed to initialize the random number generator.
 
     Returns:
         list: Localized occupied orbital coefficients per spin channel.
-    '''
+    """
     rng = np.random.default_rng(seed=seed)
     from pyscf.lo import boys, edmiston, pipek
     loc_dict = {'ER': edmiston.EdmistonRuedenberg,
                 'FB': boys.Boys,
                 'GPM': pipek.PipekMezey,
                 'PM': pipek.PipekMezey}
 
@@ -58,45 +58,45 @@
             noise = rng.normal(scale=5e-4, size=tmp_orb.shape)
             localizer.mo_coeff = tmp_orb + noise
         loc_orb.append(tmp_orb)
     return loc_orb
 
 
 def get_fods(object, basis='pc-1', loc='FB', elec_symbols=None):
-    '''Generate FOD positions using the PyCOM method.
+    """Generate FOD positions using the PyCOM method.
 
     Reference: J. Comput. Chem. 40, 2843.
 
     Args:
         object: Atoms or SCF object.
 
     Keyword Args:
         basis (str): Basis set for the DFT calculation.
         loc (str): Localization method (case insensitive).
         elec_symbols (list): Identifier for up and down FODs.
 
     Returns:
         ndarray: FOD positions.
-    '''
+    """
     try:
         from pyscf.gto import Mole
-        from pyscf.scf import UKS, RKS
+        from pyscf.scf import RKS, UKS
     except ImportError:
         log.exception('Necessary dependencies not found. To use this module, '
                       'install them with "pip install eminus[fods]".\n\n')
         raise
 
     try:
         atoms = object.atoms
     except AttributeError:
         atoms = object
     loc = loc.upper()
 
     if elec_symbols is None:
-        elec_symbols = ['X', 'He']
+        elec_symbols = ('X', 'He')
         if 'He' in atoms.atom and atoms.Nspin == 2:
             log.warning('You need to modify "elec_symbols" to calculate helium in the spin-'
                         'polarized case.')
 
     # Convert to Angstrom for PySCF
     X = bohr2ang(atoms.X)
     # Build the PySCF input format
@@ -127,28 +127,28 @@
         phi = ao @ loc_orb[s]
         dens = phi.conj() * phi * mf.grids.weights[:, None]
         loc_com.append(dens.T @ mf.grids.coords)
     return loc_com
 
 
 def split_fods(atom, X, elec_symbols=None):
-    '''Split atom and FOD coordinates.
+    """Split atom and FOD coordinates.
 
     Args:
         atom (list): Atom symbols.
         X (ndarray): Atom positions.
 
     Keyword Args:
         elec_symbols (list): Identifier for up and down FODs.
 
     Returns:
         tuple[list, ndarray, list]: Atom types, the respective coordinates, and FOD positions.
-    '''
+    """
     if elec_symbols is None:
-        elec_symbols = ['X', 'He']
+        elec_symbols = ('X', 'He')
 
     X_fod_up = []
     X_fod_dn = []
     # Iterate in reverted order, because we may delete elements
     for ia in range(len(X) - 1, -1, -1):
         if atom[ia] in elec_symbols:
             if atom[ia] in elec_symbols[0]:
@@ -159,23 +159,23 @@
             del atom[ia]
 
     X_fod = [np.asarray(X_fod_up), np.asarray(X_fod_dn)]
     return atom, X, X_fod
 
 
 def remove_core_fods(object, fods):
-    '''Remove core FODs from a set of FOD coordinates.
+    """Remove core FODs from a set of FOD coordinates.
 
     Args:
         object: Atoms or SCF object.
         fods (list): FOD positions.
 
     Returns:
         ndarray: Valence FOD positions.
-    '''
+    """
     try:
         atoms = object.atoms
     except AttributeError:
         atoms = object
 
     # If the number of valence electrons is the same as the number of FODs, do nothing
     if atoms.Nspin == 1 and len(fods[0]) * 2 == np.sum(atoms.f[0]):
```

### Comparing `eminus-2.4.0/eminus/extras/libxc.py` & `eminus-2.5.0/eminus/extras/libxc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 #!/usr/bin/env python3
-'''Interface to use Libxc functionals.
+"""Interface to use Libxc functionals.
 
 For a list of available functionals, see: https://www.tddft.org/programs/libxc/functionals
 
 One can install pylibxc by compiling Libxc according to:
 https://tddft.org/programs/libxc/installation/#python-library
 
 Alternatively, one can use the PySCF Libxc interface with::
 
     pip install eminus[libxc]
-'''
+"""
 import numpy as np
 from scipy.linalg import norm
 
 from .. import config
 from ..logger import log
 
 
-def libxc_functional(xc, n_spin, Nspin, dn_spin=None):
-    '''Handle Libxc exchange-correlation functionals via pylibxc.
+def libxc_functional(xc, n_spin, Nspin, dn_spin=None, tau=None):
+    """Handle Libxc exchange-correlation functionals via pylibxc.
 
     Only LDA and GGA functionals can be used.
+
     Reference: SoftwareX 7, 1.
 
     Args:
         xc (str | int): Exchange or correlation identifier.
         n_spin (ndarray): Real-space electronic densities per spin channel.
         Nspin (int): Number of spin states.
 
     Keyword Args:
         dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        tau (ndarray): Real-space kinetic energy densities per spin channel.
 
     Returns:
-        tuple[ndarray, ndarray]: Exchange-correlation energy density and potential.
-    '''
+        tuple[ndarray, ndarray, ndarray, ndarray]: Exch.-corr. energy density and potentials.
+    """
     try:
         assert config.use_pylibxc
         from pylibxc import LibXCFunctional
     except (ImportError, AssertionError):
-        return pyscf_functional(xc, n_spin, Nspin, dn_spin)
+        return pyscf_functional(xc, n_spin, Nspin, dn_spin, tau)
 
     # Libxc functionals have one integer and one string identifier
     try:
         func = LibXCFunctional(int(xc), Nspin)
     except ValueError:
         func = LibXCFunctional(xc, Nspin)
 
@@ -53,62 +55,87 @@
         # The gradients have to be reshaped as well, but also squared
         if Nspin == 1:
             dn2 = norm(dn_spin, axis=2)**2
         else:
             # For the spin-polairzed case the gradients of spin-up and -down are mixed together
             dn2 = np.vstack((norm(dn_spin[0], axis=1)**2, np.sum(dn_spin[0] * dn_spin[1], axis=1),
                             norm(dn_spin[1], axis=1)**2))
-        out = func.compute({'rho': n_spin.T.ravel(), 'sigma': dn2.T.ravel()})
+        if tau is None:
+            out = func.compute({'rho': n_spin.T.ravel(), 'sigma': dn2.T.ravel()})
+        else:
+            out = func.compute({'rho': n_spin.T.ravel(), 'sigma': dn2.T.ravel(),
+                                'tau': tau.T.ravel()})
     # zk is a column vector, flatten it to a 1d row vector
     exc = out['zk'].ravel()
+
     # vrho (and vsigma) is exactly transposed from what we need
     vxc = out['vrho'].T
     if dn_spin is not None:
-        vsigma = out['vsigma'].T
-        return exc, vxc, np.atleast_2d(vsigma)
-    return exc, vxc, None
+        vsigma = np.atleast_2d(out['vsigma'].T)
+        if tau is not None:
+            vtau = out['vtau'].T
+            return exc, vxc, vsigma, vtau
+        return exc, vxc, vsigma, None
+    return exc, vxc, None, None
 
 
-def pyscf_functional(xc, n_spin, Nspin, dn_spin=None):
-    '''Handle Libxc exchange-correlation functionals via PySCF.
+def pyscf_functional(xc, n_spin, Nspin, dn_spin=None, tau=None):
+    """Handle Libxc exchange-correlation functionals via PySCF.
 
     Only LDA and GGA functionals can be used.
+
     Reference: WIREs Comput. Mol. Sci. 8, e1340.
 
     Args:
         xc (str | int): Exchange or correlation identifier.
         n_spin (ndarray): Real-space electronic densities per spin channel.
         Nspin (int): Number of spin states.
 
     Keyword Args:
         dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        tau (ndarray): Real-space kinetic energy densities per spin channel.
 
     Returns:
-        tuple[ndarray, ndarray]: Exchange-correlation energy density and potential.
-    '''
+        tuple[ndarray, ndarray, ndarray, ndarray]: Exch.-corr. energy density and potentials.
+    """
     try:
         from pyscf.dft.libxc import eval_xc
     except ImportError:
         log.exception('Necessary dependencies not found. To use this module, '
                       'install them with "pip install eminus[libxc]".\n\n')
         raise
 
-    # The function also returns fxc and kxc (higher derivatives) that are not needed at this point
-    # Spin in PySCF is the number of unpaired electrons, not the number of spin channels
     if dn_spin is None:
         # For LDAs we only need the spin densities that are already in the needed shape
-        exc, vxc, _, _ = eval_xc(xc, n_spin, spin=Nspin - 1)
-        # The first entry of vxc is vrho as a 1d array for Nspin=1 and as a column array for Nspin=2
-        return exc, np.atleast_2d(vxc[0].T), None
+        rho = n_spin
     else:
-        # For GGAs we have to append the density gradients
-        # The input "density" rho is sorted as (n,grad_x n,grad_y n,grad_z n)
-        if Nspin == 1:
-            # For spin-paired systems we have to remove the spin indexing, i.e., the outermost shape
-            rho = np.vstack((n_spin[0], dn_spin[0].T))
+        if tau is None:
+            # For GGAs we have to append the density gradients
+            # The input "density" rho is sorted as (n,grad_x n,grad_y n,grad_z n)
+            if Nspin == 1:
+                # For spin-paired systems we have to remove the spin indexing (the outermost shape)
+                rho = np.vstack((n_spin[0], dn_spin[0].T))
+            else:
+                rho = np.array([np.vstack((n_spin[0], dn_spin[0].T)),
+                                np.vstack((n_spin[1], dn_spin[1].T))])
         else:
-            rho = np.array([np.vstack((n_spin[0], dn_spin[0].T)),
-                            np.vstack((n_spin[1], dn_spin[1].T))])
-        exc, vxc, _, _ = eval_xc(xc, rho, spin=Nspin - 1)
-        # The second entry of the second entry is vsigma
-        # vsigma can be a 1d or 2d array depending on the spin, reshape it as needed
-        return exc, np.atleast_2d(vxc[0].T), np.atleast_2d(vxc[1].T)
+            # For meta-GGAs we have to append the kinetic energy densities as well
+            # The input "density" rho is sorted as (n,grad_x n,grad_y n,grad_z n,lapl,tau)
+            # We do not support meta-GGAs with a dependency of the laplacian so set it to zero
+            lapl = np.zeros(len(n_spin[0]))
+            if Nspin == 1:
+                rho = np.vstack((n_spin[0], dn_spin[0].T, lapl, tau[0]))
+            else:
+                rho = np.array([np.vstack((n_spin[0], dn_spin[0].T, lapl, tau[0])),
+                                np.vstack((n_spin[1], dn_spin[1].T, lapl, tau[1]))])
+
+    # Spin in PySCF is the number of unpaired electrons, not the number of spin channels
+    exc, vxc, _, _ = eval_xc(xc, rho, spin=Nspin - 1)
+    # The first entry of vxc is vrho
+    # The second entry of the second entry is vsigma
+    # The fourth entry of the second entry is vtau (the third would be vlapl)
+    # These arrays are 1d for Nspin=1 and a 2d column array for Nspin=2, reshape them as needed
+    if dn_spin is not None:
+        if tau is not None:
+            return exc, np.atleast_2d(vxc[0].T), np.atleast_2d(vxc[1].T), np.atleast_2d(vxc[3].T)
+        return exc, np.atleast_2d(vxc[0].T), np.atleast_2d(vxc[1].T), None
+    return exc, np.atleast_2d(vxc[0].T), None, None
```

### Comparing `eminus-2.4.0/eminus/extras/torch.py` & `eminus-2.5.0/eminus/extras/torch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-'''Implementation of operators using Torch FFT functions.
+"""Implementation of operators using Torch FFT functions.
 
 For more details see :mod:`~eminus.operators`.
 
 For installation instructions see https://pytorch.org/get-started/locally/.
 
 This implementation is focused on speed, rather than readability since these operators need the
 most time in most calculations. Notable differences to the default operators are:
@@ -13,30 +13,30 @@
 * Explicitly implement Idag and Jdag for one function call less and direct normalization
 * Optional GPU calculations
 
 In my tests the overhead to move the arrays to the GPU and back is not worth it, so it is disabled
 by default.
 
 Reference: Adv. Neural. Inf. Process Syst. 32, 8024.
-'''
+"""
 import numpy as np
 
 from .. import config
 
 
 def I(atoms, W):
-    '''Backwards transformation from reciprocal space to real-space.
+    """Backwards transformation from reciprocal space to real-space.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     import torch
     n = np.prod(atoms.s)
     s = tuple(atoms.s)
 
     if W.ndim < 3:
         if len(W) == len(atoms.G2):
             Wfft = W
@@ -67,26 +67,26 @@
         Wfft = Wfft.view((atoms.Nspin,) + s + (atoms.Nstate,))
         Finv = torch.fft.ifftn(Wfft, s=s, norm='forward', dim=(1, 2, 3)).view(atoms.Nspin, n,
                                                                               atoms.Nstate)
     return Finv.detach().cpu().numpy()
 
 
 def J(atoms, W, full=True):
-    '''Forward transformation from real-space to reciprocal space.
+    """Forward transformation from real-space to reciprocal space.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Keyword Args:
         full (bool): Wether to transform in the full or in the active space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     import torch
     n = np.prod(atoms.s)
     s = tuple(atoms.s)
 
     Wfft = torch.from_numpy(np.copy(W))
     if config.use_gpu:
         Wfft = Wfft.cuda()
@@ -106,26 +106,26 @@
         if F.ndim < 3:
             return F[atoms.active]
         return F[:, atoms.active[0]]
     return F
 
 
 def Idag(atoms, W, full=False):
-    '''Conjugated backwards transformation from real-space to reciprocal space.
+    """Conjugated backwards transformation from real-space to reciprocal space.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Keyword Args:
         full (bool): Wether to transform in the full or in the active space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     import torch
     n = np.prod(atoms.s)
     s = tuple(atoms.s)
 
     Wfft = torch.from_numpy(np.copy(W))
     if config.use_gpu:
         Wfft = Wfft.cuda()
@@ -145,23 +145,23 @@
         if F.ndim < 3:
             return F[atoms.active]
         return F[:, atoms.active[0]]
     return F
 
 
 def Jdag(atoms, W):
-    '''Conjugated forward transformation from reciprocal space to real-space.
+    """Conjugated forward transformation from reciprocal space to real-space.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     import torch
     n = np.prod(atoms.s)
     s = tuple(atoms.s)
 
     if W.ndim < 3:
         if len(W) == len(atoms.G2):
             Wfft = W
```

### Comparing `eminus-2.4.0/eminus/extras/viewer.py` & `eminus-2.5.0/eminus/extras/viewer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 #!/usr/bin/env python3
-'''Viewer functions for Jupyter notebooks.'''
+"""Viewer functions for Jupyter notebooks."""
+import io
+import pathlib
+
 import numpy as np
 
-from .fods import split_fods
 from ..data import COVALENT_RADII, CPK_COLORS
 from ..io import create_pdb_str, read_cube, read_xyz
 from ..logger import log
 from ..tools import get_isovalue
+from .fods import split_fods
 
 
 def view(*args, **kwargs):
-    '''Unified display function.'''
+    """Unified display function."""
     if isinstance(args[0], str):
         return view_file(*args, **kwargs)
     else:
         return view_atoms(*args, **kwargs)
 
 
 def view_atoms(object, extra=None, plot_n=False, percent=85, surfaces=20):
-    '''Display atoms and 3D-coordinates, e.g., FODs or grid points, or even densities.
+    """Display atoms and 3D-coordinates, e.g., FODs or grid points, or even densities.
+
+    Reference: https://plotly.com/python/
 
     Args:
         object: Atoms or SCF object.
 
     Keyword Args:
         extra (ndarray | list ): Extra coordinates or FODs to display.
         plot_n (bool): Weather to plot the electronic density (only for executed scf objects).
         percent (float): Amount of density that should be contained.
         surfaces (int): Number of surfaces to display in density plots (reduce for performance).
 
     Returns:
         None.
-    '''
+    """
     try:
         import plotly.graph_objects as go
     except ImportError:
         log.exception('Necessary dependencies not found. To use this module, '
                       'install them with "pip install eminus[viewer]".\n\n')
         raise
     try:
@@ -75,74 +80,83 @@
             extra_data = go.Scatter3d(x=extra[:, 0], y=extra[:, 1], z=extra[:, 2],
                                       name='Coordinates',
                                       mode='markers',
                                       marker={'size': 1, 'color': 'red'})
             fig.add_trace(extra_data)
 
     # A density can be plotted for an scf object
-    if plot_n:
-        try:
-            den_data = go.Volume(x=atoms.r[:, 0], y=atoms.r[:, 1], z=atoms.r[:, 2], value=object.n,
-                                 name='Density',
-                                 colorbar_title=f'Density ({percent}%)',
-                                 colorscale='Inferno',
-                                 isomin=get_isovalue(object.n, percent=percent),
-                                 isomax=np.max(object.n),
-                                 surface_count=surfaces,
-                                 opacity=0.1,
-                                 showlegend=True)
-            fig.add_trace(den_data)
-            # Move colorbar to the left
-            fig.data[-1].colorbar.x = -0.15
-        except (AttributeError, TypeError):
-            log.warning('Density plots are only possible for executed SCF objects.')
+    if isinstance(plot_n, np.ndarray) or plot_n:
+        # Plot a given array or use the density from an scf object
+        if isinstance(plot_n, np.ndarray):
+            density = plot_n
+        else:
+            density = object.n
+        den_data = go.Volume(x=atoms.r[:, 0], y=atoms.r[:, 1], z=atoms.r[:, 2], value=density,
+                             name='Density',
+                             colorbar_title=f'Density ({percent}%)',
+                             colorscale='Inferno',
+                             isomin=get_isovalue(density, percent=percent),
+                             isomax=np.max(density),
+                             surface_count=surfaces,
+                             opacity=0.1,
+                             showlegend=True)
+        fig.add_trace(den_data)
+        # Move colorbar to the left
+        fig.data[-1].colorbar.x = -0.15
 
     # Theming
     fig.update_layout(scene={'xaxis': {'range': [0, atoms.a[0]], 'title': 'x [a<sub>0</sub>]'},
                              'yaxis': {'range': [0, atoms.a[1]], 'title': 'y [a<sub>0</sub>]'},
                              'zaxis': {'range': [0, atoms.a[2]], 'title': 'z [a<sub>0</sub>]'},
                              'aspectmode': 'cube'},
                       legend={'itemsizing': 'constant', 'title': 'Selection'},
                       hoverlabel_bgcolor='black',
                       template='none')
     fig.show()
     return
 
 
 def view_file(filename, isovalue=0.01, gui=False, elec_symbols=None, **kwargs):
-    '''Display molecules and orbitals.
+    """Display molecules and orbitals.
 
     Reference: Bioinformatics 34, 1241.
 
     Args:
         filename (str): Input file path/name. This can be either a cube or xyz file.
 
     Keyword Args:
         isovalue (float): Isovalue for sizing orbitals.
         gui (bool): Turn on the NGLView GUI.
         elec_symbols (list): Identifier for up and down FODs.
 
+    Keyword Args:
+        **kwargs: Throwaway arguments.
+
     Returns:
         NGLWidget: Viewable object.
-    '''
+    """
     try:
-        from nglview import NGLWidget, TextStructure
+        from nglview import NGLWidget, TextStructure, write_html
     except ImportError:
         log.exception('Necessary dependencies not found. To use this module, '
                       'install them with "pip install eminus[viewer]".\n\n')
         raise
 
     if elec_symbols is None:
-        elec_symbols = ['X', 'He']
-
+        elec_symbols = ('X', 'He')
     if isinstance(isovalue, str):
         isovalue = float(isovalue)
+
     view = NGLWidget(**kwargs)
     view._set_size('400px', '400px')
+    # Set the gui to the view
+    if gui:
+        view.gui_style = 'ngl'
 
+    # Handle XYZ files
     if filename.endswith('.xyz'):
         # Atoms
         atom, X = read_xyz(filename)
         atom, X, X_fod = split_fods(atom, X, elec_symbols)
         view.add_component(TextStructure(create_pdb_str(atom, X)))
         view[0].clear()
         view[0].add_ball_and_stick()
@@ -155,18 +169,18 @@
         # Spin down FODs
         if len(X_fod[1]) > 0:
             view.add_component(TextStructure(create_pdb_str([elec_symbols[1]] * len(X_fod[1]),
                                X_fod[1])))
             view[2].clear()
             view[2].add_ball_and_stick(f'_{elec_symbols[1]}', color='green', radius=0.1)
         view.center()
-
-    if filename.endswith('.cube'):
+    # Handle CUBE files
+    elif filename.endswith('.cube'):
         # Atoms and cell
-        atom, X, _, a, _ = read_cube(filename)
+        atom, X, _, a, _, _ = read_cube(filename)
         atom, X, X_fod = split_fods(atom, X, elec_symbols)
         view.add_component(TextStructure(create_pdb_str(atom, X, a)))
         view[0].clear()
         view[0].add_ball_and_stick()
         view.add_unitcell()
         view.center()
         # Spin up
@@ -196,8 +210,56 @@
             view[3].add_ball_and_stick(f'_{elec_symbols[0]}', color='red', radius=0.1)
         # Spin down FODs
         if len(X_fod[1]) > 0:
             view.add_component(TextStructure(create_pdb_str([elec_symbols[1]] * len(X_fod[1]),
                                X_fod[1])))
             view[4].clear()
             view[4].add_ball_and_stick(f'_{elec_symbols[1]}', color='green', radius=0.1)
-    return view.display(gui=gui)
+    # Handle other files (mainly PDB)
+    else:
+        # If no xyz or cube file is used try a more generic file viewer
+        ext = pathlib.Path(filename).suffix.replace('.', '')
+        # It seems that only pdb works with this method
+        if ext != 'pdb':
+            log.warning('Only XYZ, CUBE, and PDB files are support, but others might work.')
+        with open(filename, 'r') as fh:
+            view.add_component(fh, ext=ext)
+        view[0].clear()
+        view[0].add_ball_and_stick()
+        view.center()
+
+    # Check if the function has been executed in a notebook
+    # If yes, just return the view
+    if executed_in_notebook():
+        return view
+    # Otherwise the viewer would display nothing
+    # But if plotly is installed on can write the view to a StringIO object and display it with the
+    # smart open_html_in_browser function from plotly that automatically opens a new browser tab
+    try:
+        from plotly.io._base_renderers import open_html_in_browser
+        # Use StringIO object instead of a temporary file
+        with io.StringIO() as html:
+            write_html(html, view)
+            open_html_in_browser(html.getvalue())
+    except ImportError:
+        log.exception('This function only works in notebooks or with Plotly installed.')
+    return None
+
+
+def executed_in_notebook():
+    """Check if the code runs in a notebook.
+
+    Reference: https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
+
+    Returns:
+        bool: Weather in a notebook or not.
+    """
+    try:
+        shell = get_ipython().__class__.__name__
+        if shell == 'ZMQInteractiveShell':  # Jupyter notebook or qtconsole
+            return True
+        elif shell == 'TerminalInteractiveShell':  # Terminal running IPython
+            return False
+        else:  # Other type
+            return False
+    except NameError:
+        return False
```

### Comparing `eminus-2.4.0/eminus/gth.py` & `eminus-2.5.0/eminus/gth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
-'''Utilities to use Goedecker, Teter, and Hutter (GTH) pseudopotentials.'''
+"""Utilities to use Goedecker, Teter, and Hutter pseudopotentials."""
 import numpy as np
 
 from .logger import log
 from .utils import Ylm_real
 
 
 def init_gth_loc(scf):
-    '''Initialize parameters to calculate local contributions of GTH pseudopotentials.
+    """Initialize parameters to calculate local contributions of GTH pseudopotentials.
 
     Reference: Phys. Rev. B 54, 1703.
 
     Args:
         scf: SCF object.
 
     Returns:
         ndarray: Local GTH potential contribution.
-    '''
+    """
     atoms = scf.atoms
     species = set(atoms.atom)
     omega = 1  # Normally this would be det(atoms.R), but Arias notation is off by this factor
 
     Vloc = np.zeros_like(atoms.G2)
     for isp in species:
         psp = scf.GTH[isp]
@@ -50,24 +50,24 @@
                 Sf += atoms.Sf[ia]
         Vloc += np.real(atoms.J(Vsp * Sf))
     return Vloc
 
 
 # Adapted from https://github.com/f-fathurrahman/PWDFT.jl/blob/master/src/PsPotNL.jl
 def init_gth_nonloc(scf):
-    '''Initialize parameters to calculate non-local contributions of GTH pseudopotentials.
+    """Initialize parameters to calculate non-local contributions of GTH pseudopotentials.
 
     Reference: Phys. Rev. B 54, 1703.
 
     Args:
         scf: SCF object.
 
     Returns:
         tuple[int, ndarray, ndarray]: NbetaNL, prj2beta, and betaNL.
-    '''
+    """
     atoms = scf.atoms
     prj2beta = np.zeros((3, atoms.Natoms, 4, 7), dtype=int)
     prj2beta += -1  # Set to an invalid index
 
     NbetaNL = 0
     for ia in range(atoms.Natoms):
         psp = scf.GTH[atoms.atom[ia]]
@@ -92,62 +92,63 @@
                     betaNL[:, ibeta] = (-1j)**l * Ylm_real(l, m, g) * \
                         eval_proj_G(psp, l, iprj + 1, Gm, atoms.Omega) * Sf
                     ibeta += 1
     return NbetaNL, prj2beta, betaNL
 
 
 # Adapted from https://github.com/f-fathurrahman/PWDFT.jl/blob/master/src/op_V_Ps_nloc.jl
-def calc_Vnonloc(scf, W):
-    '''Calculate the non-local pseudopotential, applied on the basis functions W.
+def calc_Vnonloc(scf, spin, W):
+    """Calculate the non-local pseudopotential, applied on the basis functions W.
 
     Reference: Phys. Rev. B 54, 1703.
 
     Args:
         scf: SCF object.
+        spin (int): Spin variable to track weather to do the calculation for spin up or down.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: Non-local GTH potential contribution.
-    '''
+    """
     atoms = scf.atoms
 
-    Vpsi = np.zeros_like(W, dtype=complex)
+    Vpsi = np.zeros_like(W[spin], dtype=complex)
     if scf.NbetaNL > 0:  # Only calculate non-local potential if necessary
-        betaNL_psi = (W.conj().T @ scf.betaNL).conj()
+        betaNL_psi = (W[spin].conj().T @ scf.betaNL).conj()
 
         for ia in range(atoms.Natoms):
             psp = scf.GTH[atoms.atom[ia]]
             for l in range(psp['lmax']):
                 for m in range(-l, l + 1):
                     for iprj in range(psp['Nproj_l'][l]):
                         ibeta = scf.prj2beta[iprj, ia, l, m + psp['lmax'] - 1] - 1
                         for jprj in range(psp['Nproj_l'][l]):
                             jbeta = scf.prj2beta[jprj, ia, l, m + psp['lmax'] - 1] - 1
                             hij = psp['h'][l, iprj, jprj]
-                            Vpsi += hij * betaNL_psi[:, jbeta] * scf.betaNL[:, ibeta][:, None]
+                            Vpsi += hij * betaNL_psi[:, jbeta] * scf.betaNL[:, ibeta, None]
     # We have to multiply with the cell volume, because of different orthogonalization methods
     return Vpsi * atoms.Omega
 
 
 # Adapted from https://github.com/f-fathurrahman/PWDFT.jl/blob/master/src/PsPot_GTH.jl
 def eval_proj_G(psp, l, iprj, Gm, Omega):
-    '''Evaluate GTH projector functions in G-space.
+    """Evaluate GTH projector functions in G-space.
 
     Reference: Phys. Rev. B 54, 1703.
 
     Args:
         psp (dict): GTH parameters.
         l (int): Angular momentum number.
         iprj (int): Nproj_l index.
         Gm (ndarray): Magnitude of G-vectors.
         Omega (float): Unit cell volume.
 
     Returns:
         ndarray: GTH projector.
-    '''
+    """
     rrl = psp['rp'][l]
     Gr2 = (Gm * rrl)**2
 
     prefactor = 4 * np.pi**(5 / 4) * np.sqrt(2**(l + 1) * rrl**(2 * l + 3) / Omega)
     Vprj = prefactor * np.exp(-0.5 * Gr2)
 
     if l == 0:  # s-channel
@@ -169,9 +170,9 @@
             return 1 / np.sqrt(15) * Gm**2 * Vprj
         elif iprj == 2:
             return (2 / 3) / np.sqrt(105) * Gm**2 * (7 - Gr2) * Vprj
     elif l == 3:  # f-channel
         # Only one projector
         return 1 / np.sqrt(105) * Gm**3 * Vprj
 
-    log.error(f'No projector found for l={l}')
-    return
+    log.error(f'No projector found for l={l}.')
+    return None
```

### Comparing `eminus-2.4.0/eminus/io/__init__.py` & `eminus-2.5.0/eminus/io/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 #!/usr/bin/env python3
-'''File input and output functionalities.'''
+"""File input and output functionalities."""
+from ..logger import log
 from .cube import read_cube, write_cube
 from .gth import read_gth
 from .json import read_json, write_json
 from .pdb import create_pdb_str, write_pdb
 from .xyz import read_xyz, write_xyz
-from ..logger import log
 
 __all__ = ['create_pdb_str', 'read', 'read_cube', 'read_gth', 'read_json', 'read_xyz', 'write',
            'write_cube', 'write_json', 'write_pdb', 'write_xyz']
 
 
 def read(*args, **kwargs):
-    '''Unified file reader function.'''
+    """Unified file reader function."""
     if args[0].endswith('.json'):
         return read_json(*args, **kwargs)
     elif args[0].endswith('.xyz'):
         return read_xyz(*args, **kwargs)
     elif args[0].endswith('.cube'):
         return read_cube(*args, **kwargs)
     else:
         log.error('No viable file ending found.')
+        return None
 
 
 def write(*args, **kwargs):
-    '''Unified file writer function.'''
+    """Unified file writer function."""
     if args[1].endswith('.json'):
         return write_json(*args, **kwargs)
     elif args[1].endswith('.xyz'):
         return write_xyz(*args, **kwargs)
     elif args[1].endswith('.cube'):
         return write_cube(*args, **kwargs)
     elif args[1].endswith('.pdb'):
         return write_pdb(*args, **kwargs)
     else:
         log.error('No viable file ending found.')
+        return None
```

### Comparing `eminus-2.4.0/eminus/io/cube.py` & `eminus-2.5.0/eminus/io/cube.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,79 @@
 #!/usr/bin/env python3
-'''CUBE file handling.'''
+"""CUBE file handling."""
 import textwrap
 import time
 
 import numpy as np
 
 from ..data import NUMBER2SYMBOL, SYMBOL2NUMBER
 from ..logger import log
 from ..version import __version__
 
 
 def read_cube(filename):
-    '''Load atom and cell data from cube files.
+    """Load atom and cell data from cube files.
 
     There is no standard for cube files. The following format has been used.
     File format definition: https://h5cube-spec.readthedocs.io/en/latest/cubeformat.html
 
     Args:
         filename (str): cube input file path/name.
 
     Returns:
-        tuple[list, ndarray, float, ndarray, int]: Species, positions, charges, cell size, sampling.
-    '''
+        tuple[list, ndarray, float, ndarray, int, ndarray]:
+        Species, positions, charges, cell size, sampling, and field array.
+    """
     if not filename.endswith('.cube'):
         filename += '.cube'
 
     # Atomic units and a cuboidal cell that starts at (0,0,0) are assumed.
     with open(filename, 'r') as fh:
         lines = fh.readlines()
 
         # The first and second line can contain comments, print them if available
         comment = f'{lines[0].strip()}\n{lines[1].strip()}'
         if comment:
-            log.info(f'XYZ file comment: "{comment}"')
+            log.info(f'CUBE file comment: "{comment}"')
 
         # Line 4 to 6 contain the sampling per axis, and the cell basis vectors with length a/s
         # A cuboidal cell is assumed, so only use the diagonal entries
         s = np.empty(3, dtype=int)
         a = np.empty(3)
         for i, line in enumerate(lines[3:6]):
             line_split = line.strip().split()
             s[i] = line_split[0]
             a[i] = s[i] * np.float_(line_split[i + 1])
 
         atom = []
         X = []
         Z = []
         # Following lines contain atom positions with the format: atom-id charge x-pos y-pos z-pos
+        offset = 0
         for line in lines[6:]:
             line_split = line.strip().split()
             # If the first value is not a (positive) integer, we have reached the field data
             if not line_split[0].isdigit():
                 break
             atom.append(NUMBER2SYMBOL[int(line_split[0])])
             Z.append(float(line_split[1]))
             X.append(np.float_(line_split[2:5]))
-
+            offset += 1
     X = np.asarray(X)
-    return atom, X, Z, a, s
+
+    # The rest of the data is the field data
+    # Split the strings, flatten the lists of lists, and convert to a float numpy array
+    field_list = [l.split() for l in lines[6 + offset:]]
+    field_list = [item for sublist in field_list for item in sublist]
+    field = np.asarray(field_list, dtype=float)
+    return atom, X, Z, a, s, field
 
 
 def write_cube(object, filename, field, fods=None, elec_symbols=None):
-    '''Generate cube files from given field data.
+    """Generate cube files from given field data.
 
     There is no standard for cube files. The following format has been used to work with VESTA.
     File format definition: https://h5cube-spec.readthedocs.io/en/latest/cubeformat.html
 
     Args:
         object: Atoms or SCF object.
         filename (str): cube output file path/name.
@@ -73,41 +81,32 @@
 
     Keyword Args:
         fods (list): FOD coordinates to write.
         elec_symbols (list): Identifier for up and down FODs.
 
     Returns:
         None.
-    '''
+    """
     # Atomic units are assumed, so there is no need for conversion.
     try:
         atoms = object.atoms
     except AttributeError:
         atoms = object
 
     if not filename.endswith('.cube'):
         filename += '.cube'
 
     if elec_symbols is None:
-        elec_symbols = ['X', 'He']
+        elec_symbols = ('X', 'He')
         if 'He' in atoms.atom and atoms.Nspin == 2:
             log.warning('You need to modify "elec_symbols" to write helium with FODs in the spin-'
                         'polarized case.')
 
-    # Our field data has been created in a different order than needed for cube files
-    # (triple loop over z,y,x instead of x,y,z), so rearrange it with some index magic.
-    idx = []
-    for Nx in range(atoms.s[0]):
-        for Ny in range(atoms.s[1]):
-            for Nz in range(atoms.s[2]):
-                idx.append(Nx + Ny * atoms.s[0] + Nz * atoms.s[0] * atoms.s[1])
-    idx = np.asarray(idx)
-
     # Make sure we have real valued data in the correct order
-    field = np.real(field[idx])
+    field = np.real(field)
 
     with open(filename, 'w') as fp:
         # The first two lines have to be a comment.
         # Print information about the file and program, and the file creation time.
         fp.write(f'File generated with eminus {__version__} on {time.ctime()}\n\n')
         # Number of atoms (int), and origin of the coordinate system (float)
         # The origin is normally at 0,0,0 but we could move our box, so take the minimum
```

### Comparing `eminus-2.4.0/eminus/io/gth.py` & `eminus-2.5.0/eminus/io/gth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 #!/usr/bin/env python3
-'''GTH file handling.'''
+"""GTH file handling."""
 import inspect
 import pathlib
 
 import numpy as np
 
 from ..logger import log
 
 
-def read_gth(atom, charge=None, xc='pade', psp_path=None):
-    '''Read GTH files for a given atom.
+def read_gth(atom, charge=None, psp_path='pade'):
+    """Read GTH files for a given atom.
 
     Reference: Phys. Rev. B 54, 1703.
 
     Args:
         atom (str): Atom name.
 
     Keyword Args:
         charge (int): Valence charge.
-        xc (str): Weather to use the pade or the pbe pseudopotential files.
-        psp_path (str): Path to GTH pseudopotential files. Defaults to installation_path/psp/.
+        psp_path (str): Path to GTH pseudopotential files. Defaults to installation_path/psp/pade.
 
     Returns:
         dict: GTH parameters.
-    '''
-    if psp_path is None:
+    """
+    if psp_path in ('pade', 'pbe'):
         file_path = pathlib.Path(inspect.getfile(inspect.currentframe())).parent
-        psp_path = file_path.parent.joinpath(f'psp/{xc}')
+        file_path = file_path.parent.joinpath(f'psp/{psp_path}')
+    else:
+        file_path = pathlib.Path(psp_path)
 
     if charge is not None:
-        f_psp = psp_path.joinpath(f'{atom}-q{charge}')
+        f_psp = file_path.joinpath(f'{atom}-q{charge}')
     else:
-        files = sorted(psp_path.glob(f'{atom}-q*'))
+        files = sorted(file_path.glob(f'{atom}-q*'))
         try:
             f_psp = pathlib.Path(files[0])
         except IndexError:
-            log.warning(f'There is no GTH pseudopotential in {psp_path} for "{atom}"')
+            log.warning(f'There is no GTH pseudopotential in "{file_path}" for "{atom}".')
             return mock_gth()
         if len(files) > 1:
             log.info(f'Multiple pseudopotentials found for "{atom}". '
                      f'Continue with "{f_psp.name}".')
 
     psp = {}
     cloc = np.zeros(4)
@@ -75,25 +76,25 @@
                 for jtmp in range(3):
                     for ktmp in range(i, 3):
                         h[i, ktmp, jtmp] = h[i, jtmp, ktmp]
             psp['rp'] = rp  # Projector radius for each angular momentum
             psp['Nproj_l'] = Nproj_l  # Number of non-local projectors
             psp['h'] = h  # Projector coupling coefficients per AM channel
     except FileNotFoundError:
-        log.warning(f'There is no GTH pseudopotential for "{f_psp.name}"')
+        log.warning(f'There is no GTH pseudopotential for "{f_psp.name}".')
         return mock_gth()
     return psp
 
 
 def mock_gth():
-    '''Create a mock dictionary with all-zeros, for atom species with no pseudopotential file.
+    """Create a mock dictionary with all-zeros, for atom species with no pseudopotential file.
 
     Returns:
         dict: GTH parameters (all zero).
-    '''
+    """
     return {
         'Zion': 0,
         'rloc': 0,
         'cloc': np.zeros(4),
         'lmax': 0,
         'rp': np.zeros(4),
         'Nproj_l': np.zeros(4, dtype=int),
```

### Comparing `eminus-2.4.0/eminus/io/json.py` & `eminus-2.5.0/eminus/io/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python3
-'''JSON file handling.'''
+"""JSON file handling."""
 import base64
 import copy
 import json
 
 import numpy as np
 
 
 def read_json(filename):
-    '''Load objects from a JSON file.
+    """Load objects from a JSON file.
 
     Args:
         filename (str): json input file path/name.
 
     Returns:
         Class object.
-    '''
+    """
     import eminus
 
     def custom_object_hook(dct):
-        '''Custom JSON object hook to create eminus classes after deserialization.'''
+        """Custom JSON object hook to create eminus classes after deserialization."""
         # ndarrays are base64 encoded, decode and recreate
         if isinstance(dct, dict) and '__ndarray__' in dct:
             data = base64.b64decode(dct['__ndarray__'])
             return np.frombuffer(data, dct['dtype']).reshape(dct['shape'])
 
         # Create a simple eminus objects and set all attributes afterwards
         # Explicitly call objects with verbosity since the logger is created at instantiation
@@ -56,24 +56,24 @@
         filename += '.json'
 
     with open(filename, 'r') as fh:
         return json.load(fh, object_hook=custom_object_hook)
 
 
 def write_json(object, filename):
-    '''Save objects in a JSON file.
+    """Save objects in a JSON file.
 
     Args:
         object: Class object.
         filename (str): json output file path/name.
-    '''
+    """
     import eminus
 
     class CustomEncoder(json.JSONEncoder):
-        '''Custom JSON encoder class to serialize eminus classes.'''
+        """Custom JSON encoder class to serialize eminus classes."""
         def default(self, obj):
             # ndarrays are not json serializable, encode them as base64 to save them
             if isinstance(obj, np.ndarray):
                 data = base64.b64encode(obj.copy(order='C')).decode('utf-8')
                 return {'__ndarray__': data, 'dtype': str(obj.dtype), 'shape': obj.shape}
 
             # If obj is a Atoms or SCF class dump them as a dictionary
```

### Comparing `eminus-2.4.0/eminus/io/pdb.py` & `eminus-2.5.0/eminus/io/pdb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 #!/usr/bin/env python3
-'''PDB file handling.'''
+"""PDB file handling."""
 import numpy as np
 
 from ..logger import log
 from ..units import bohr2ang
 
 
-def write_pdb(object, filename, fods=None, elec_symbols=None):
-    '''Generate pdb files from atoms objects.
+def write_pdb(object, filename, fods=None, elec_symbols=None, trajectory=False):
+    """Generate pdb files from atoms objects.
 
     See :func:`~eminus.io.pdb.create_pdb_str` for more information about the pdb file format.
 
     Args:
         object: Atoms or SCF object.
         filename (str): pdb output file path/name.
 
     Keyword Args:
         fods (list): FOD coordinates to write.
         elec_symbols (list): Identifier for up and down FODs.
+        trajectory (bool): Allow appending to a file to create trajectories.
 
     Returns:
         None.
-    '''
+    """
     try:
         atoms = object.atoms
     except AttributeError:
         atoms = object
 
     if not filename.endswith('.pdb'):
         filename += '.pdb'
 
     if elec_symbols is None:
-        elec_symbols = ['X', 'He']
+        elec_symbols = ('X', 'He')
         if 'He' in atoms.atom and atoms.Nspin == 2:
             log.warning('You need to modify "elec_symbols" to write helium with FODs in the spin-'
                         'polarized case.')
 
     atom = atoms.atom
     X = atoms.X
     if fods is not None:
         if len(fods[0]) != 0:
             atom = atom + [elec_symbols[0]] * len(fods[0])
             X = np.vstack((X, fods[0]))
         if len(fods) > 1 and len(fods[1]) != 0:
             atom = atom + [elec_symbols[1]] * len(fods[1])
             X = np.vstack((X, fods[1]))
 
-    with open(filename, 'w') as fp:
+    # Append to a file when using the trajectory keyword
+    if trajectory:
+        mode = 'a'
+    else:
+        mode = 'w'
+
+    with open(filename, mode) as fp:
         fp.write(create_pdb_str(atom, X, a=atoms.a))
     return
 
 
 def create_pdb_str(atom, X, a=None):
-    '''Convert atom symbols and positions to the pdb format.
+    """Convert atom symbols and positions to the pdb format.
 
     File format definitions:
         CRYST1: https://www.wwpdb.org/documentation/file-format-content/format33/sect8.html#CRYST1
 
         ATOM: https://www.wwpdb.org/documentation/file-format-content/format33/sect9.html#ATOM
 
     Args:
@@ -64,53 +71,53 @@
         X (ndarray): Atom positions.
 
     Keyword Args:
         a (float): Cell size.
 
     Returns:
         str: pdb file format.
-    '''
+    """
     # Convert Bohr to Angstrom
     X = bohr2ang(X)
     if a is not None:
         a = bohr2ang(a)
 
     # pdb files have specific numbers of characters for every data with changing justification
     # Write everything explicitly down to not loose track of line lengths
     pdb = ''
     # Create data for a cuboidal cell
     if a is not None:
-        pdb += 'CRYST1'                 # 1-6 "CRYST1"
-        pdb += f'{a[0]:9.3f}'.rjust(9)  # 7-15 a
-        pdb += f'{a[1]:9.3f}'.rjust(9)  # 16-24 b
-        pdb += f'{a[2]:9.3f}'.rjust(9)  # 25-33 c
-        pdb += f'{90:7.2f}'.rjust(7)    # 34-40 alpha
-        pdb += f'{90:7.2f}'.rjust(7)    # 41-47 beta
-        pdb += f'{90:7.2f}'.rjust(7)    # 48-54 gamma
+        pdb += 'CRYST1'          # 1-6 "CRYST1"
+        pdb += f'{a[0]:>9,.3f}'  # 7-15 a
+        pdb += f'{a[1]:>9,.3f}'  # 16-24 b
+        pdb += f'{a[2]:>9,.3f}'  # 25-33 c
+        pdb += f'{90:>7,.2f}'    # 34-40 alpha
+        pdb += f'{90:>7,.2f}'    # 41-47 beta
+        pdb += f'{90:>7,.2f}'    # 48-54 gamma
         pdb += ' '
-        pdb += 'P 1'.ljust(11)          # 56-66 Space group
-        # pdb += '1'.rjust(4)           # 67-70 Z value
+        pdb += 'P 1        '     # 56-66 Space group
+        # pdb += '   1'          # 67-70 Z value
         pdb += '\n'
 
     # Create molecule data
     pdb += 'MODEL 1'
     for ia in range(len(atom)):
-        pdb += '\nATOM  '                   # 1-6 "ATOM"
-        pdb += f'{ia + 1}'.rjust(5)         # 7-11 Atom serial number
+        pdb += '\nATOM  '            # 1-6 "ATOM"
+        pdb += f'{ia + 1:>5}'        # 7-11 Atom serial number
         pdb += ' '
-        pdb += f'{atom[ia]}'.rjust(4)       # 13-16 Atom name
-        pdb += ' '                          # 17 Alternate location indicator
-        pdb += 'MOL'                        # 18-20 Residue name
+        pdb += f'{atom[ia]:>4}'      # 13-16 Atom name
+        pdb += ' '                   # 17 Alternate location indicator
+        pdb += 'MOL'                 # 18-20 Residue name
         pdb += ' '
-        pdb += ' '                          # 22 Chain identifier
-        pdb += '1'.rjust(4)                 # 23-26 Residue sequence number
-        pdb += ' '                          # 27 Code for insertions of residues
+        pdb += ' '                   # 22 Chain identifier
+        pdb += '   1'                # 23-26 Residue sequence number
+        pdb += ' '                   # 27 Code for insertions of residues
         pdb += '   '
-        pdb += f'{X[ia, 0]:8.3f}'.rjust(8)  # 31-38 X orthogonal coordinate
-        pdb += f'{X[ia, 1]:8.3f}'.rjust(8)  # 39-46 Y orthogonal coordinate
-        pdb += f'{X[ia, 2]:8.3f}'.rjust(8)  # 47-54 Z orthogonal coordinate
-        pdb += f'{1:6.2f}'.rjust(6)         # 55-60 Occupancy
-        pdb += f'{0:6.2f}'.rjust(6)         # 61-66 Temperature factor
+        pdb += f'{X[ia, 0]:>8,.3f}'  # 31-38 X orthogonal coordinate
+        pdb += f'{X[ia, 1]:>8,.3f}'  # 39-46 Y orthogonal coordinate
+        pdb += f'{X[ia, 2]:>8,.3f}'  # 47-54 Z orthogonal coordinate
+        pdb += f'{1:>6,.2f}'         # 55-60 Occupancy
+        pdb += f'{0:>6,.2f}'         # 61-66 Temperature factor
         pdb += '          '
-        pdb += f'{atom[ia]}'.rjust(2)       # 77-78 Element symbol
-        # pdb += '  '                       # 79-80 Charge
-    return f'{pdb}\nENDMDL'
+        pdb += f'{atom[ia]:>2}'      # 77-78 Element symbol
+        # pdb += '  '                # 79-80 Charge
+    return f'{pdb}\nENDMDL\n'
```

### Comparing `eminus-2.4.0/eminus/io/xyz.py` & `eminus-2.5.0/eminus/io/xyz.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python3
-'''XYZ file handling.'''
+"""XYZ file handling."""
 import time
 
 import numpy as np
 
 from ..logger import log
 from ..units import ang2bohr, bohr2ang
 from ..version import __version__
 
 
 def read_xyz(filename):
-    '''Load atom species and positions from xyz files.
+    """Load atom species and positions from xyz files.
 
     File format definition: https://openbabel.org/wiki/XYZ_%28format%29
 
     Args:
         filename (str): xyz input file path/name.
 
     Returns:
         tuple[list, ndarray]: Atom species and positions.
-    '''
+    """
     if not filename.endswith('.xyz'):
         filename += '.xyz'
 
     with open(filename, 'r') as fh:
         lines = fh.readlines()
 
         # The first line contains the number of atoms
@@ -43,50 +43,57 @@
             X.append(np.float_(line_split[1:4]))
 
     # xyz files are in Angstrom, so convert to Bohr
     X = ang2bohr(np.asarray(X))
     return atom, X
 
 
-def write_xyz(object, filename, fods=None, elec_symbols=None):
-    '''Generate xyz files from atoms objects.
+def write_xyz(object, filename, fods=None, elec_symbols=None, trajectory=False):
+    """Generate xyz files from atoms objects.
 
     File format definition: https://openbabel.org/wiki/XYZ_%28format%29
 
     Args:
         object: Atoms or SCF object.
         filename (str): xyz output file path/name.
 
     Keyword Args:
         fods (list): FOD coordinates to write.
         elec_symbols (list): Identifier for up and down FODs.
+        trajectory (bool): Allow appending to a file to create trajectories.
 
     Returns:
         None.
-    '''
+    """
     try:
         atoms = object.atoms
     except AttributeError:
         atoms = object
 
     if not filename.endswith('.xyz'):
         filename += '.xyz'
 
     # Convert the coordinates from atomic units to Angstrom
     X = bohr2ang(atoms.X)
     if fods is not None:
         fods = [bohr2ang(i) for i in fods]
 
     if elec_symbols is None:
-        elec_symbols = ['X', 'He']
+        elec_symbols = ('X', 'He')
         if 'He' in atoms.atom and atoms.Nspin == 2:
             log.warning('You need to modify "elec_symbols" to write helium with FODs in the spin-'
                         'polarized case.')
 
-    with open(filename, 'w') as fp:
+    # Append to a file when using the trajectory keyword
+    if trajectory:
+        mode = 'a'
+    else:
+        mode = 'w'
+
+    with open(filename, mode) as fp:
         # The first line contains the number of atoms.
         # If we add FOD coordinates, add them to the count.
         if fods is None:
             fp.write(f'{atoms.Natoms}\n')
         else:
             fp.write(f'{atoms.Natoms + sum([len(i) for i in fods])}\n')
         # The second line can contains a comment.
```

### Comparing `eminus-2.4.0/eminus/localizer.py` & `eminus-2.5.0/eminus/localizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 #!/usr/bin/env python3
-'''Utilities to localize and analyze orbitals.'''
+"""Utilities to localize and analyze orbitals."""
 import numpy as np
 from scipy.linalg import eig, expm, norm
 from scipy.stats import unitary_group
 
 from .logger import log
 from .utils import handle_spin_gracefully
 
 
 def eval_psi(atoms, psi, r):
-    '''Evaluate orbitals at given coordinate points.
+    """Evaluate orbitals at given coordinate points.
 
     Args:
         atoms: Atoms object.
         psi (ndarray): Set of orbitals in reciprocal space.
         r (ndarray): Real-space positions.
 
     Returns:
         ndarray: Values of psi at points r.
-    '''
+    """
     # Shift the evaluation point to (0,0,0), because we always have a lattice point there
     psi_T = atoms.T(psi, -r)
     psi_Trs = atoms.I(psi_T)
     # The zero entry is always the value at point (0,0,0)
     return psi_Trs[0]
 
 
 def get_R(atoms, psi, fods):
-    '''Calculate transformation matrix to build Fermi orbitals.
+    """Calculate transformation matrix to build Fermi orbitals.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         atoms: Atoms object.
         psi (ndarray): Set of orbitals in reciprocal space.
         fods (list): Fermi-orbital descriptors.
 
     Returns:
         ndarray: Transformation matrix R.
-    '''
+    """
     # We only calculate occupied orbitals, so a zero matrix is enough
     R = np.empty((len(fods), len(fods)), dtype=complex)
 
     for i in range(len(fods)):
         # Get the value at one FOD position for all psi
         psi_fod = eval_psi(atoms, psi, fods[i])
         sum_psi_fod = np.sqrt(np.sum(psi_fod.conj() * psi_fod))
         for j in range(len(fods)):
             R[i, j] = psi_fod[j].conj() / sum_psi_fod
     return R
 
 
 def get_FO(atoms, psi, fods):
-    '''Calculate Fermi orbitals from Kohn-Sham orbitals.
+    """Calculate Fermi orbitals from Kohn-Sham orbitals.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         atoms: Atoms object.
         psi (ndarray): Set of orbitals in reciprocal space.
         fods (list): Fermi-orbital descriptors.
 
     Returns:
         ndarray: Real-space Fermi orbitals.
-    '''
+    """
     fo = np.zeros((atoms.Nspin, len(atoms.r), atoms.Nstate), dtype=complex)
 
     # Transform psi to real-space
     psi_rs = atoms.I(psi)
     for spin in range(atoms.Nspin):
         # Get the transformation matrix R
         R = get_R(atoms, psi[spin], fods[spin])
@@ -75,188 +75,188 @@
             for j in range(atoms.Nstate):
                 fo[spin, :, i] += R[i, j] * psi_rs[spin, :, j]
     return fo
 
 
 @handle_spin_gracefully
 def get_S(atoms, psirs):
-    '''Calculate overlap matrix between orbitals.
+    """Calculate overlap matrix between orbitals.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         atoms: Atoms object.
         psirs (ndarray): Set of orbitals in real-space.
 
     Returns:
         ndarray: Overlap matrix S.
-    '''
+    """
     # Overlap elements: S_ij = \int psi_i^* psi_j dr
     S = np.empty((atoms.Nstate, atoms.Nstate), dtype=complex)
 
     dV = atoms.Omega / np.prod(atoms.s)
     for i in range(atoms.Nstate):
         for j in range(atoms.Nstate):
             S[i, j] = dV * np.sum(psirs[:, i].conj() * psirs[:, j])
     return S
 
 
 def get_FLO(atoms, psi, fods):
-    '''Calculate Fermi-Löwdin orbitals by orthonormalizing Fermi orbitals.
+    """Calculate Fermi-Loewdin orbitals by orthonormalizing Fermi orbitals.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         atoms: Atoms object.
         psi (ndarray): Set of orbitals in reciprocal space.
         fods (list): Fermi-orbital descriptors.
 
     Returns:
-        ndarray: Real-space Fermi-Löwdin orbitals.
-    '''
+        ndarray: Real-space Fermi-Loewdin orbitals.
+    """
     fo = get_FO(atoms, psi, fods)
     flo = np.empty((atoms.Nspin, len(atoms.r), atoms.Nstate), dtype=complex)
 
     for spin in range(atoms.Nspin):
         # Calculate the overlap matrix for FOs
         S = get_S(atoms, fo[spin])
         # Calculate eigenvalues and eigenvectors
         Q, T = eig(S)
-        # Löwdins symmetric orthonormalization method
+        # Loewdins symmetric orthonormalization method
         Q12 = np.diag(1 / np.sqrt(Q))
         flo[spin] = fo[spin] @ (T @ Q12 @ T.T)
     return flo
 
 
 @handle_spin_gracefully
 def wannier_cost(atoms, psirs):
-    '''Calculate the Wannier cost function, namely the orbital variance. Equivalent to Foster-Boys.
+    """Calculate the Wannier cost function, namely the orbital variance. Equivalent to Foster-Boys.
 
     This function does not account for periodcity, it may be a good idea to center the system.
 
     Reference: J. Chem. Phys. 137, 224114.
 
     Args:
         atoms: Atoms object.
         psirs (ndarray): Set of orbitals in real-space.
 
     Returns:
         ndarray: Variance per orbital.
-    '''
+    """
     # Variance = \int psi r^2 psi - (\int psi r psi)^2
     centers = wannier_center(atoms, psirs)
     moments = second_moment(atoms, psirs)
     costs = moments - norm(centers, axis=1)**2
     log.debug(f'Centers:\n{centers}\nMoments:\n{moments}')
     log.info(f'Costs:\n{costs}')
     return costs
 
 
 @handle_spin_gracefully
 def wannier_center(atoms, psirs):
-    '''Calculate Wannier centers, i.e., the expectation values of r.
+    """Calculate Wannier centers, i.e., the expectation values of r.
 
     Reference: J. Chem. Phys. 137, 224114.
 
     Args:
         atoms: Atoms object.
         psirs (ndarray): Set of orbitals in real-space.
 
     Returns:
         ndarray: Wannier centers per orbital.
-    '''
+    """
     dV = atoms.Omega / np.prod(atoms.s)
 
     centers = np.empty((atoms.Nstate, 3))
     for i in range(atoms.Nstate):
         for dim in range(3):
             centers[i, dim] = dV * np.real(np.sum(psirs[:, i].conj() * atoms.r[:, dim] *
                                            psirs[:, i], axis=0))
     return centers
 
 
 @handle_spin_gracefully
 def second_moment(atoms, psirs):
-    '''Calculate the second moments, i.e., the expectation values of r^2.
+    """Calculate the second moments, i.e., the expectation values of r^2.
 
     Reference: J. Chem. Phys. 137, 224114.
 
     Args:
         atoms: Atoms object.
         psirs (ndarray): Set of orbitals in real-space.
 
     Returns:
         ndarray: Second moments per orbital.
-    '''
+    """
     dV = atoms.Omega / np.prod(atoms.s)
     r2 = norm(atoms.r, axis=1)**2
 
     moments = np.empty(atoms.Nstate)
     for i in range(atoms.Nstate):
         moments[i] = dV * np.real(np.sum(psirs[:, i].conj() * r2 * psirs[:, i], axis=0))
     return moments
 
 
 @handle_spin_gracefully
 def wannier_supercell_matrices(atoms, psirs):
-    '''Calculate matrices for the supercell Wannier localization.
+    """Calculate matrices for the supercell Wannier localization.
 
     Reference: Phys. Rev. B 59, 9703.
 
     Args:
         atoms: Atoms object.
         psirs (ndarray): Set of orbitals in real-space.
 
     Returns:
         tuple[ndarray, ndarray, ndarray]: Matrices X, Y, and Z.
-    '''
+    """
     dV = atoms.Omega / np.prod(atoms.s)
     # Similar to the expectation value of r, but accounting for periodicity
     X = (psirs.conj().T * np.exp(-1j * 2 * np.pi * atoms.r[:, 0] / atoms.a[0])) @ psirs
     Y = (psirs.conj().T * np.exp(-1j * 2 * np.pi * atoms.r[:, 1] / atoms.a[1])) @ psirs
     Z = (psirs.conj().T * np.exp(-1j * 2 * np.pi * atoms.r[:, 2] / atoms.a[2])) @ psirs
     return X * dV, Y * dV, Z * dV
 
 
 def wannier_supercell_cost(X, Y, Z):
-    '''Calculate the supercell Wannier cost.
+    """Calculate the supercell Wannier cost.
 
     This is an equivalent criterion to the spread criterion, but not the same. This cost function
     will be maximized instead of the minimization of the spread.
 
     Reference: Phys. Rev. B 59, 9703.
 
     Args:
         X (ndarray): Calculation specific matrix.
         Y (ndarray): Calculation specific matrix.
         Z (ndarray): Calculation specific matrix.
 
     Returns:
         float: Supercell Wannier cost.
-    '''
+    """
     X2 = np.abs(np.diagonal(X))**2
     Y2 = np.abs(np.diagonal(Y))**2
     Z2 = np.abs(np.diagonal(Z))**2
     return np.sum(X2 + Y2 + Z2)
 
 
 def wannier_supercell_grad(atoms, X, Y, Z):
-    '''Calculate the supercell Wannier gradient.
+    """Calculate the supercell Wannier gradient.
 
     Reference: Phys. Rev. B 59, 9703.
 
     Args:
         atoms: Atoms object.
         X (ndarray): Calculation specific matrix.
         Y (ndarray): Calculation specific matrix.
         Z (ndarray): Calculation specific matrix.
 
     Returns:
         ndarray: Supercell Wannier gradient.
-    '''
+    """
     x = np.zeros((atoms.Nstate, atoms.Nstate), dtype=complex)
     y = np.zeros((atoms.Nstate, atoms.Nstate), dtype=complex)
     z = np.zeros((atoms.Nstate, atoms.Nstate), dtype=complex)
     # Just the indexed gradient from the paper, without fancy optimization
     for n in range(atoms.Nstate):
         for m in range(atoms.Nstate):
             x[m, n] = X[n, m] * (X[n, n].conj() - X[m, m].conj()) \
@@ -265,16 +265,16 @@
                 - Y[m, n].conj() * (Y[m, m] - Y[n, n])
             z[m, n] = Z[n, m] * (Z[n, n].conj() - Z[m, m].conj()) \
                 - Z[m, n].conj() * (Z[m, m] - Z[n, n])
     return x + y + z
 
 
 @handle_spin_gracefully
-def get_wannier(atoms, psirs, Nit=10000, conv_tol=1e-7, mu=0.25, random_guess=False):
-    '''Steepest descent supercell Wannier localization.
+def get_wannier(atoms, psirs, Nit=10000, conv_tol=1e-7, mu=0.25, random_guess=False, seed=None):
+    """Steepest descent supercell Wannier localization.
 
     This function is rather sensitive to the starting point, thus it is a good idea to start from
     already localized orbitals.
 
     This optimizes the given orbitals under unitary constraint matrices, see
     IEEE Trans. Signal Process. 56, 1134.
 
@@ -285,26 +285,28 @@
         psirs (ndarray): Set of orbitals in real-space.
 
     Keyword Args:
         Nit (int): Number of iterations.
         conv_tol (float): Convergence tolerance.
         mu (float): Step size.
         random_guess (bool): Weather to use a random unitary starting guess or the identity.
+        seed (int | None): Seed to get a reproducible random guess.
 
     Returns:
         ndarray: Localized orbitals.
-    '''
+    """
     X, Y, Z = wannier_supercell_matrices(atoms, psirs)  # Calculate matrices only once
     # The initial unitary transformation is the identity or a random unitary matrix
     if random_guess and atoms.Nstate > 1:
-        U = unitary_group.rvs(atoms.Nstate)
+        U = unitary_group.rvs(atoms.Nstate, random_state=seed)
     else:
         U = np.eye(atoms.Nstate)
     costs = [0]  # Add a zero to the costs to allow the sign evaluation in the first iteration
 
+    atoms.log.debug(f'{"Iteration":<11}{"Cost [a0^2]":<13}{"dCost [a0^2]":<13}')
     for i in range(Nit):
         sign = 1
         costs.append(wannier_supercell_cost(X, Y, Z))
         if abs(costs[-2] - costs[-1]) < conv_tol:
             atoms.log.info(f'Wannier localizer converged after {i} iterations.')
             break
         # If the cost function gets smaller, change the direction
@@ -319,13 +321,14 @@
         expA_pos, expA_neg = expm(A), expm(-A)
         # Update total rotation
         U = U @ expA_pos
         # Update matrices
         X = expA_neg @ X @ expA_pos
         Y = expA_neg @ Y @ expA_pos
         Z = expA_neg @ Z @ expA_pos
-        atoms.log.debug(f'Iteration: {i} \tCost: {costs[-1]}')
+
+        atoms.log.debug(f'{i:>8}   {costs[-1]:<+13,.6f}{costs[-2] - costs[-1]:<+13,.4e}')
 
     if len(costs) > 1 and abs(costs[-2] - costs[-1]) > conv_tol:
         atoms.log.warning('Wannier localizer not converged!')
     # Return the localized orbitals by rotating them
     return psirs @ U
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eminus-2.4.0/eminus/logger.py` & `eminus-2.5.0/eminus/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 #!/usr/bin/env python3
-'''Logger initialization and configuration.'''
+"""Logger initialization and configuration."""
 import logging
 import sys
 
 
 class CustomLogger(logging.Logger):
-    '''Custom logger for the usage outside of classes.
+    """Custom logger for the usage outside of classes.
 
     This is just a basic logger, but with an added verbose property.
 
     Args:
         name (str): Logger name.
-    '''
+    """
     def __init__(self, name):
+        """Initialize the CustomLogger object."""
         super().__init__(name)
 
     @property
     def verbose(self):
-        '''Verbosity level.'''
+        """Verbosity level."""
         return self._verbose
 
     @verbose.setter
     def verbose(self, level):
         self._verbose = get_level(level)
         self.setLevel(self._verbose)
 
 
 class CustomFormatter(logging.Formatter):
-    '''Custom logger formatter.'''
+    """Custom logger formatter."""
     def format(self, record):
-        '''Use different formatting for different logging levels.
+        """Use different formatting for different logging levels.
 
         Args:
             record: LogRecord object.
-        '''
+        """
         if record.levelno >= logging.WARNING:
             # Print the level name for errors and warning
             self._style._fmt = '%(levelname)s: %(msg)s'
         else:
             # But not for infos and debug messages
             self._style._fmt = '%(msg)s'
         return super().format(record)
@@ -54,32 +55,32 @@
 formatter = CustomFormatter()
 handler = logging.StreamHandler(sys.stdout)
 handler.setFormatter(formatter)
 logging.root.addHandler(handler)
 
 
 def create_logger(object):
-    '''Create a logger unique to an object.
+    """Create a logger unique to an object.
 
     Args:
         object: Instance of a class.
-    '''
+    """
     # Use ID of object to create a unique logger
     # Without this setting the verbosity in one instance would affect other instances
     local_log = logging.getLogger(str(id(object)))
     local_log.verbose = log.verbose
     return local_log
 
 
 def get_level(verbose):
-    '''Validate logging levels.
+    """Validate logging levels.
 
     Args:
         verbose (int | str): Level of output (case insensitive).
-    '''
+    """
     log_levels = {
         0: 'CRITICAL',
         1: 'ERROR',
         2: 'WARNING',
         3: 'INFO',
         4: 'DEBUG'
     }
@@ -89,19 +90,19 @@
         level = log_levels.get(verbose, 'DEBUG')
     else:
         level = verbose.upper()
     return level
 
 
 def name(newname):
-    '''Add a name to functions without evaluating them for better logging.
+    """Add a name to functions without evaluating them for better logging.
 
     Args:
         newname (str): Function name.
 
     Returns:
         Callable: Decorator.
-    '''
+    """
     def decorator(f):
         f.__name__ = newname
         return f
     return decorator
```

### Comparing `eminus-2.4.0/eminus/operators.py` & `eminus-2.5.0/eminus/operators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-'''Basis set dependent operators for a plane wave basis.
+"""Basis set dependent operators for a plane wave basis.
 
 These operators act on discretized wave functions, i.e., the arrays W.
 
 These W are column vectors. This has been chosen to let theory and code coincide, e.g.,
 W^dagger W becomes :code:`W.conj().T @ W`.
 
 The downside is that the i-th state will be accessed with W[:, i] instead of W[i].
@@ -18,75 +18,78 @@
 5. the active reciprocal space
 6. the active reciprocal space (1d)
 
 The active space is the truncated reciprocal space by restricting it with a sphere given by ecut.
 
 Every spin dependence will be handled with handle_spin_gracefully by calling the operators for each
 spin individually.
-'''
+"""
 import numpy as np
 from scipy.fft import fftn, ifftn
 
 from . import config
 from .utils import handle_spin_gracefully
 
 
 # Spin handling is trivial for this operator
 def O(atoms, W):
-    '''Overlap operator.
+    """Overlap operator.
 
     This operator acts on the options 3, 4, 5, and 6.
+
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     return atoms.Omega * W
 
 
 @handle_spin_gracefully
 def L(atoms, W):
-    '''Laplacian operator.
+    """Laplacian operator.
 
     This operator acts on the options 3 and 5.
+
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     # G2 is a normal 1d row vector, reshape it so it can be applied to the column vector W
     if len(W) == len(atoms.G2c):
         G2 = atoms.G2c[:, None]
     else:
         G2 = atoms.G2[:, None]
     return -atoms.Omega * G2 * W
 
 
 @handle_spin_gracefully
 def Linv(atoms, W):
-    '''Inverse Laplacian operator.
+    """Inverse Laplacian operator.
 
     This operator acts on the options 3 and 4.
+
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     # Ignore the division by zero for the first elements
     with np.errstate(divide='ignore', invalid='ignore'):
         if W.ndim == 1:
             # One could do some proper indexing with [1:] but indexing is slow
             out = W / (atoms.G2 * -atoms.Omega)
             out[0] = 0
         else:
@@ -95,26 +98,27 @@
             out = W / (G2 * -atoms.Omega)
             out[0, :] = 0
     return out
 
 
 @handle_spin_gracefully
 def I(atoms, W):
-    '''Backwards transformation from reciprocal space to real-space.
+    """Backwards transformation from reciprocal space to real-space.
 
     This operator acts on the options 3, 4, 5, and 6.
+
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     n = np.prod(atoms.s)
 
     # If W is in the full space do nothing with W
     if len(W) == len(atoms.G2):
         Wfft = np.copy(W)
     else:
         # Fill with zeros if W is in the active space
@@ -140,29 +144,30 @@
         Finv = ifftn(Wfft, workers=config.threads, overwrite_x=True, norm='forward',
                      axes=(0, 1, 2)).reshape((n, atoms.Nstate))
     return Finv
 
 
 @handle_spin_gracefully
 def J(atoms, W, full=True):
-    '''Forward transformation from real-space to reciprocal space.
+    """Forward transformation from real-space to reciprocal space.
 
     This operator acts on the options 1 and 2.
+
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Keyword Args:
         full (bool): Wether to transform in the full or in the active space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     n = np.prod(atoms.s)
     Wfft = np.copy(W)
 
     # `workers` sets the number of threads the FFT operates on
     # `overwrite_x` allows writing in Wfft, but since we do not need Wfft later on, we can set this
     # for a little bit of extra performance
     # Normally, we would have to divide by n in the end for the correct normalization, but we can
@@ -180,89 +185,90 @@
     if not full:
         return F[atoms.active]
     return F
 
 
 @handle_spin_gracefully
 def Idag(atoms, W, full=False):
-    '''Conjugated backwards transformation from real-space to reciprocal space.
+    """Conjugated backwards transformation from real-space to reciprocal space.
 
     This operator acts on the options 1 and 2.
+
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Keyword Args:
         full (bool): Wether to transform in the full or in the active space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     n = np.prod(atoms.s)
     F = J(atoms, W, full)
     return F * n
 
 
 @handle_spin_gracefully
 def Jdag(atoms, W):
-    '''Conjugated forward transformation from reciprocal space to real-space.
+    """Conjugated forward transformation from reciprocal space to real-space.
 
     This operator acts on the options 3, 4, 5, and 6.
+
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     n = np.prod(atoms.s)
     Finv = I(atoms, W)
     return Finv / n
 
 
 @handle_spin_gracefully
 def K(atoms, W):
-    '''Preconditioning operator.
+    """Preconditioning operator.
 
     This operator acts on the options 3 and 5.
+
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
-    # G2 is a normal 1d row vector, reshape it so it can be applied to the column vector W
-    if len(W) == len(atoms.G2c):
-        G2 = atoms.G2c[:, None]
-    else:
-        G2 = atoms.G2[:, None]
-    return W / (1 + G2)
+    """
+    # G2c is a normal 1d row vector, reshape it so it can be applied to the column vector W
+    return W / (1 + atoms.G2c[:, None])
 
 
 @handle_spin_gracefully
 def T(atoms, W, dr):
-    '''Translation operator.
+    """Translation operator.
 
     This operator acts on the options 5 and 6.
 
+    Reference: https://ccrma.stanford.edu/~jos/st/Shift_Theorem.html
+
     Args:
         atoms: Atoms object.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
         dr (ndarray): Real-space shift.
 
     Returns:
         ndarray: The operator applied on W.
-    '''
+    """
     # Do the shift by multiplying a phase factor, given by the shift theorem
     if len(W) == len(atoms.G2c):
         G = atoms.G[atoms.active]
     else:
         G = atoms.G
     factor = np.exp(-1j * G @ dr)
     # factor is a normal 1d row vector, reshape it so it can be applied to the column vector W
```

### Comparing `eminus-2.4.0/eminus/orbitals.py` & `eminus-2.5.0/eminus/orbitals.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 #!/usr/bin/env python3
-'''Workflow functions that combine functions to generate orbitals.'''
+"""Workflow functions that combine functions to generate orbitals."""
 from .dft import get_psi
 from .io import write_cube
 from .localizer import get_FLO, get_FO, get_wannier
 from .logger import log
 
 
 def KSO(scf, write_cubes=False, **kwargs):
-    '''Generate Kohn-Sham orbitals and optionally save them as cube files.
+    """Generate Kohn-Sham orbitals and optionally save them as cube files.
 
     Reference: Phys. Rev. 140, A1133.
 
     Args:
         scf: SCF object.
 
     Keyword Args:
         write_cubes (bool): Write orbitals to cube files.
+        **kwargs: Throwaway arguments.
 
     Returns:
         ndarray: Real-space Kohn-Sham orbitals.
-    '''
+    """
     atoms = scf.atoms
 
     # Calculate eigenfunctions and transform to real-space
     kso = atoms.I(get_psi(scf, scf.W))
     if write_cubes:
         cube_writer(atoms, 'KSO', kso)
     return kso
 
 
 def FO(scf, write_cubes=False, fods=None):
-    '''Generate Fermi orbitals and optionally save them as cube files.
+    """Generate Fermi orbitals and optionally save them as cube files.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         scf: SCF object.
 
     Keyword Args:
         write_cubes (bool): Write orbitals to cube files.
         fods (list): Fermi-orbital descriptors.
 
     Returns:
         ndarray: Real-space Fermi orbitals.
-    '''
+    """
     # Lazy import extras
     from .extras.fods import get_fods, remove_core_fods
     atoms = scf.atoms
 
     # Calculate eigenfunctions
     kso = get_psi(scf, scf.W)
     if fods is None:
@@ -58,28 +59,28 @@
     fo = get_FO(atoms, kso, fods)
     if write_cubes:
         cube_writer(atoms, 'FO', fo)
     return fo
 
 
 def FLO(scf, write_cubes=False, fods=None):
-    '''Generate Fermi-Löwdin orbitals and optionally save them as cube files.
+    """Generate Fermi-Loewdin orbitals and optionally save them as cube files.
 
     Reference: J. Chem. Phys. 153, 084104.
 
     Args:
         scf: SCF object.
 
     Keyword Args:
         write_cubes (bool): Write orbitals to cube files.
         fods (list): Fermi-orbital descriptors.
 
     Returns:
-        ndarray: Real-space Fermi-Löwdin orbitals.
-    '''
+        ndarray: Real-space Fermi-Loewdin orbitals.
+    """
     # Lazy import extras
     from .extras.fods import get_fods, remove_core_fods
     atoms = scf.atoms
 
     # Calculate eigenfunctions
     kso = get_psi(scf, scf.W)
     if fods is None:
@@ -90,28 +91,28 @@
     flo = get_FLO(atoms, kso, fods)
     if write_cubes:
         cube_writer(atoms, 'FLO', flo)
     return flo
 
 
 def WO(scf, write_cubes=False, precondition=True):
-    '''Generate Wannier orbitals and optionally save them as cube files.
+    """Generate Wannier orbitals and optionally save them as cube files.
 
     Reference: Phys. Rev. B 59, 9703.
 
     Args:
         scf: SCF object.
 
     Keyword Args:
         write_cubes (bool): Write orbitals to cube files.
         precondition (bool): Precondition by calculating FLOs as the initial guess.
 
     Returns:
         ndarray: Real-space Wannier orbitals.
-    '''
+    """
     atoms = scf.atoms
 
     # Calculate eigenfunctions/initial guess orbitals and transform to real-space
     if precondition:
         psi = FLO(scf)
     else:
         psi = atoms.I(get_psi(scf, scf.W))
@@ -119,21 +120,21 @@
     wo = get_wannier(atoms, psi)
     if write_cubes:
         cube_writer(atoms, 'WO', wo)
     return wo
 
 
 def cube_writer(atoms, type, orbitals):
-    '''Simple cube file writer function.
+    """Simple cube file writer function.
 
     Args:
         atoms: Atoms object.
         type (str): Orbital type for the cube file names.
         orbitals (ndarray): Real-space orbitals.
-    '''
+    """
     # Create the system name
     name = ''
     for ia in sorted(set(atoms.atom)):
         # Skip the number of atoms if it is equal to one
         na = atoms.atom.count(ia)
         name += f'{ia}{na if na > 1 else ""}'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eminus-2.4.0/eminus/potentials.py` & `eminus-2.5.0/eminus/potentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 #!/usr/bin/env python3
-'''Collection of miscellaneous potentials.'''
+"""Collection of miscellaneous potentials."""
 import numpy as np
 from scipy.linalg import norm
 
 from .logger import log
 
 
 def harmonic(atoms):
-    '''Harmonic potential.
+    """Harmonic potential.
 
     Can be used for quantum dot calculations.
 
     Args:
         atoms: Atoms object.
 
     Returns:
         ndarray: Harmonic potential in reciprocal space.
-    '''
+    """
     freq = 2
     dr = norm(atoms.r - np.sum(atoms.R, axis=1) / 2, axis=1)
     Vharm = 0.5 * freq**2 * dr**2
     return atoms.Jdag(atoms.O(atoms.J(Vharm)))
 
 
 def coulomb(atoms):
-    '''All-electron Coulomb potential.
+    """All-electron Coulomb potential.
+
+    Reference: Bull. Lebedev Phys. Inst. 42, 329.
 
     Args:
         atoms: Atoms object.
 
     Returns:
         ndarray: Coulomb potential in reciprocal space.
-    '''
+    """
     Z = atoms.Z[0]  # Potential should only be used for same species
 
     # Ignore the division by zero for the first elements
     # One could do some proper indexing with [1:] but indexing is slow
     with np.errstate(divide='ignore', invalid='ignore'):
         Vcoul = -4 * np.pi * Z / atoms.G2
     Vcoul[0] = 0
 
     Sf = np.sum(atoms.Sf, axis=0)
     return atoms.J(Vcoul * Sf)
 
 
 def ge(atoms):
-    '''Starkloff-Joannopoulos local pseudopotential for germanium.
+    """Starkloff-Joannopoulos local pseudopotential for germanium.
 
     Fourier-transformed by Tomas Arias.
+
     Reference: Phys. Rev. B 16, 5212.
 
     Args:
         atoms: Atoms object.
 
     Returns:
         ndarray: Germanium pseudopotential in reciprocal space.
-    '''
+    """
     Z = 4  # Potential should only be used for germanium
     lamda = 18.5
     rc = 1.052
     Gm = np.sqrt(atoms.G2)
     Vps = np.empty_like(atoms.G2)
 
     with np.errstate(divide='ignore', invalid='ignore'):
@@ -76,26 +79,26 @@
          np.sum((-1)**n * np.exp(-lamda * rc * n) / n**2)))
 
     Sf = np.sum(atoms.Sf, axis=0)
     return atoms.J(Vps * Sf)
 
 
 def init_pot(scf):
-    '''Handle and initialize potentials.
+    """Handle and initialize potentials.
 
     Args:
         scf: SCF object.
 
     Returns:
         ndarray: Potential in reciprocal space.
-    '''
+    """
     try:
         pot = IMPLEMENTED[scf.pot](scf.atoms)
     except KeyError:
-        log.exception(f'No potential found for "{scf.pot}"')
+        log.exception(f'No potential found for "{scf.pot}".')
         raise
     return pot
 
 
 IMPLEMENTED = {
     'harmonic': harmonic,
     'coulomb': coulomb,
```

### Comparing `eminus-2.4.0/eminus/psp/pade/Ac-q11` & `eminus-2.5.0/eminus/psp/pade/Ac-q11`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Ac-q29` & `eminus-2.5.0/eminus/psp/pade/Ac-q29`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Am-q17` & `eminus-2.5.0/eminus/psp/pade/Am-q17`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Am-q35` & `eminus-2.5.0/eminus/psp/pade/Am-q35`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Bk-q19` & `eminus-2.5.0/eminus/psp/pade/Bk-q19`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Bk-q37` & `eminus-2.5.0/eminus/psp/pade/Bk-q37`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Cf-q20` & `eminus-2.5.0/eminus/psp/pade/Cf-q20`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Cf-q38` & `eminus-2.5.0/eminus/psp/pade/Cf-q38`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Cm-q18` & `eminus-2.5.0/eminus/psp/pade/Cm-q18`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Cm-q36` & `eminus-2.5.0/eminus/psp/pade/Cm-q36`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Es-q21` & `eminus-2.5.0/eminus/psp/pade/Es-q21`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Es-q39` & `eminus-2.5.0/eminus/psp/pade/Es-q39`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Fm-q22` & `eminus-2.5.0/eminus/psp/pade/Fm-q22`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Fm-q40` & `eminus-2.5.0/eminus/psp/pade/Fm-q40`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Lr-q25` & `eminus-2.5.0/eminus/psp/pade/Lr-q25`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Lr-q43` & `eminus-2.5.0/eminus/psp/pade/Lr-q43`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Md-q23` & `eminus-2.5.0/eminus/psp/pade/Md-q23`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Md-q41` & `eminus-2.5.0/eminus/psp/pade/Md-q41`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/No-q24` & `eminus-2.5.0/eminus/psp/pade/No-q24`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/No-q42` & `eminus-2.5.0/eminus/psp/pade/No-q42`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Np-q15` & `eminus-2.5.0/eminus/psp/pade/Np-q15`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Np-q33` & `eminus-2.5.0/eminus/psp/pade/Np-q33`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Pa-q13` & `eminus-2.5.0/eminus/psp/pade/Pa-q13`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Pa-q31` & `eminus-2.5.0/eminus/psp/pade/Pa-q31`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Pu-q16` & `eminus-2.5.0/eminus/psp/pade/Pu-q16`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Pu-q34` & `eminus-2.5.0/eminus/psp/pade/Pu-q34`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Th-q12` & `eminus-2.5.0/eminus/psp/pade/Th-q12`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/Th-q30` & `eminus-2.5.0/eminus/psp/pade/Th-q30`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/U-q14` & `eminus-2.5.0/eminus/psp/pade/U-q14`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/U-q32` & `eminus-2.5.0/eminus/psp/pade/U-q32`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pade/__init__.py` & `eminus-2.5.0/eminus/psp/pbe/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
-'''PADE GTH pseudopotential files.
+"""PBE GTH pseudopotential files.
 
-Reference: Phys. Rev. B 54, 1703.
-'''
+Reference: Theor. Chem. Acc. 114, 145.
+"""
 
 if __name__ == '__main__':
     import inspect
     import pathlib
     import shutil
     import urllib.request
     import zipfile
@@ -16,13 +16,13 @@
     # Download files
     url = f'https://github.com/cp2k/cp2k-data/archive/refs/heads/{file}'
     urllib.request.urlretrieve(url, file)  # noqa: S310
     # Unpack files
     with zipfile.ZipFile(file, 'r') as fzip:
         fzip.extractall()
     # Move files
-    pade_path = psp_path.joinpath('cp2k-data-master/potentials/Goedecker/cp2k/pade')
-    for f in pade_path.iterdir():
+    gth_path = psp_path.joinpath('cp2k-data-master/potentials/Goedecker/cp2k/pbe')
+    for f in gth_path.iterdir():
         shutil.move(f, psp_path.joinpath(f.name))
     # Cleanup
     psp_path.joinpath(file).unlink()
     shutil.rmtree('cp2k-data-master')
```

### Comparing `eminus-2.4.0/eminus/psp/pbe/Ac-q11` & `eminus-2.5.0/eminus/psp/pbe/Ac-q11`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Ac-q29` & `eminus-2.5.0/eminus/psp/pbe/Ac-q29`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Am-q17` & `eminus-2.5.0/eminus/psp/pbe/Am-q17`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Am-q35` & `eminus-2.5.0/eminus/psp/pbe/Am-q35`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Au-q19` & `eminus-2.5.0/eminus/psp/pbe/Au-q19`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Bk-q19` & `eminus-2.5.0/eminus/psp/pbe/Bk-q19`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Bk-q37` & `eminus-2.5.0/eminus/psp/pbe/Bk-q37`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Cf-q20` & `eminus-2.5.0/eminus/psp/pbe/Cf-q20`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Cf-q38` & `eminus-2.5.0/eminus/psp/pbe/Cf-q38`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Cm-q18` & `eminus-2.5.0/eminus/psp/pbe/Cm-q18`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Cm-q36` & `eminus-2.5.0/eminus/psp/pbe/Cm-q36`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Es-q21` & `eminus-2.5.0/eminus/psp/pbe/Es-q21`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Es-q39` & `eminus-2.5.0/eminus/psp/pbe/Es-q39`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Fm-q22` & `eminus-2.5.0/eminus/psp/pbe/Fm-q22`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Fm-q40` & `eminus-2.5.0/eminus/psp/pbe/Fm-q40`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Lr-q25` & `eminus-2.5.0/eminus/psp/pbe/Lr-q25`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Lr-q43` & `eminus-2.5.0/eminus/psp/pbe/Lr-q43`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Md-q23` & `eminus-2.5.0/eminus/psp/pbe/Md-q23`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Md-q41` & `eminus-2.5.0/eminus/psp/pbe/Md-q41`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/No-q24` & `eminus-2.5.0/eminus/psp/pbe/No-q24`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/No-q42` & `eminus-2.5.0/eminus/psp/pbe/No-q42`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Np-q15` & `eminus-2.5.0/eminus/psp/pbe/Np-q15`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Np-q33` & `eminus-2.5.0/eminus/psp/pbe/Np-q33`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Pa-q13` & `eminus-2.5.0/eminus/psp/pbe/Pa-q13`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Pa-q31` & `eminus-2.5.0/eminus/psp/pbe/Pa-q31`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Pt-q18` & `eminus-2.5.0/eminus/psp/pbe/Pt-q18`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Pu-q16` & `eminus-2.5.0/eminus/psp/pbe/Pu-q16`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Pu-q34` & `eminus-2.5.0/eminus/psp/pbe/Pu-q34`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Th-q12` & `eminus-2.5.0/eminus/psp/pbe/Th-q12`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/Th-q30` & `eminus-2.5.0/eminus/psp/pbe/Th-q30`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/U-q14` & `eminus-2.5.0/eminus/psp/pbe/U-q14`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/U-q14_old` & `eminus-2.5.0/eminus/psp/pbe/U-q14_old`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/U-q32` & `eminus-2.5.0/eminus/psp/pbe/U-q32`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/psp/pbe/__init__.py` & `eminus-2.5.0/eminus/psp/pade/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
-'''PBE GTH pseudopotential files.
+"""PADE GTH pseudopotential files.
 
-Reference: Theor. Chem. Acc. 114, 145.
-'''
+Reference: Phys. Rev. B 54, 1703.
+"""
 
 if __name__ == '__main__':
     import inspect
     import pathlib
     import shutil
     import urllib.request
     import zipfile
@@ -16,13 +16,13 @@
     # Download files
     url = f'https://github.com/cp2k/cp2k-data/archive/refs/heads/{file}'
     urllib.request.urlretrieve(url, file)  # noqa: S310
     # Unpack files
     with zipfile.ZipFile(file, 'r') as fzip:
         fzip.extractall()
     # Move files
-    gth_path = psp_path.joinpath('cp2k-data-master/potentials/Goedecker/cp2k/pbe')
-    for f in gth_path.iterdir():
+    pade_path = psp_path.joinpath('cp2k-data-master/potentials/Goedecker/cp2k/pade')
+    for f in pade_path.iterdir():
         shutil.move(f, psp_path.joinpath(f.name))
     # Cleanup
     psp_path.joinpath(file).unlink()
     shutil.rmtree('cp2k-data-master')
```

### Comparing `eminus-2.4.0/eminus/scf.py` & `eminus-2.5.0/eminus/scf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!/usr/bin/env python3
-'''SCF class definition.'''
+"""SCF class definition."""
 import copy
 import logging
 import time
 
 import numpy as np
 
-from .dft import guess_gaussian, guess_pseudo, guess_random
+from .dft import get_epsilon, guess_pseudo, guess_random
 from .energies import Energy, get_Eewald, get_Esic
 from .gth import init_gth_loc, init_gth_nonloc
 from .io import read_gth
 from .logger import create_logger, get_level
-from .minimizer import IMPLEMENTED
+from .minimizer import IMPLEMENTED as all_minimizer
+from .potentials import IMPLEMENTED as all_potentials
 from .potentials import init_pot
-from .tools import center_of_mass
+from .tools import center_of_mass, get_spin_squared
 from .version import info
-from .xc import parse_functionals, parse_psp
+from .xc import parse_functionals, parse_xc_type
 
 
 class SCF:
-    '''Perform direct minimizations.
+    """Perform direct minimizations.
 
     Args:
         atoms: Atoms object.
 
     Keyword Args:
         xc (str): Comma-separated exchange-correlation functional description (case insensitive).
 
@@ -33,54 +34,65 @@
             Default: 'lda,vwn'
         pot (str): Type of pseudopotential (case insensitive).
 
             Example: 'GTH'; 'harmonic'; 'Coulomb'; 'Ge',
             Default: 'gth'
         guess (str): Initial guess method for the basis functions (case insensitive).
 
-            Example: 'Gauss'; 'gaussian'; 'random'; 'rand',
-            Default: 'gaussian'
+            Example: 'random'; 'rand'; 'pseudo',
+            Default: 'random'
         etol (float): Convergence tolerance of the total energy.
 
             Default: 1e-7
+        gradtol (float): Convergence tolerance of the gradient norm.
+
+            Disabled by default. This tolerance will only be used in conjugate gradient methods.
+
+            Default: None
         cgform (int): Conjugated-gradient form for the pccg minimization.
 
-            1 for Fletcher-Reeves, 2 for Polak-Ribiere, and 3 for Hestenes-Stiefel.
+            1 for Fletcher-Reeves, 2 for Polak-Ribiere, 3 for Hestenes-Stiefel, and 4 for Dai-Yuan
 
             Default: 1
+        sic (bool): Calculate the Kohn-Sham Perdew-Zunger SIC energy at the end of the SCF step.
+
+            Default: False
+        symmetric (bool): Weather to use the same initial guess for both spin channels.
+
+            Default: False
         min (dict | None): Dictionary to set the order and number of steps per minimization method.
 
             Example: {'sd': 10, 'pccg': 100}; {'pccg': 10, 'lm': 25, 'pclm': 50},
             Default: None (will default to {'pccg': 250})
-        sic (bool): Calculate the Kohn-Sham Perdew-Zunger SIC energy at the end of the SCF step.
-
-            Default: False
         verbose (int | str): Level of output (case insensitive).
 
             Can be one of 'CRITICAL', 'ERROR', 'WARNING', 'INFO', or 'DEBUG'.
             An integer value can be used as well, where larger numbers mean more output, starting
             from 0.
 
             Default: 'info'
-    '''
-    def __init__(self, atoms, xc='lda,vwn', pot='gth', guess='gaussian', etol=1e-7, cgform=1,
-                 sic=False, min=None, verbose=None):
-        self.atoms = atoms             # Atoms object
-        self.xc = xc.lower()           # Exchange-correlation functional
-        self.pot = pot.lower()         # Used pseudopotential
-        self.guess = guess.lower()     # Initial wave functions guess
-        self.etol = etol               # Total energy convergence tolerance
-        self.cgform = cgform           # Conjugate gradient form
-        self.sic = sic                 # Calculate the sic energy
-        self.min = min                 # Minimization methods
+    """
+    def __init__(self, atoms, xc='lda,vwn', pot='gth', guess='random', etol=1e-7, gradtol=None,
+                 cgform=1, sic=False, symmetric=False, min=None, verbose=None):
+        """Initialize the SCF object."""
+        self.atoms = atoms          # Atoms object
+        self.xc = xc.lower()        # Exchange-correlation functional
+        self.pot = pot              # Used pseudopotential
+        self.guess = guess.lower()  # Initial wave functions guess
+        self.etol = etol            # Total energy convergence tolerance
+        self.gradtol = gradtol      # Gradient norm convergence tolerance
+        self.cgform = cgform        # Conjugate gradient form
+        self.sic = sic              # Calculate the sic energy
+        self.symmetric = symmetric  # Use the same initial guess for both spin channels
+        self.min = min              # Minimization methods
 
         # Set min here, better not use mutable data types in signatures
         if self.min is None:
             # For systems with bad convergence throw in some sd steps
-            self.min = {'sd': 25, 'pccg': 250}
+            self.min = {'auto': 250}
 
         # Initialize logger
         self.log = create_logger(self)
         if verbose is None:
             self.verbose = atoms.verbose
         else:
             self.verbose = verbose
@@ -88,128 +100,133 @@
         # Set up final and intermediate results
         self.W = None             # Basis functions
         self.n = None             # Electronic density
         self.energies = Energy()  # Energy object that holds energy contributions
         self.clear()
 
         # Parameters that will be built out of the inputs
-        self.GTH = {}             # Dictionary of GTH parameters per atom species
-        self.Vloc = None          # Local pseudopotential contribution
-        self.NbetaNL = 0          # Number of projector functions for the non-local gth potential
-        self.prj2beta = None      # Index matrix to map to the correct projector function
-        self.betaNL = None        # Atomic-centered projector functions
-        self.psp = None           # Type of GTH pseudopotential that will be used
-        self.print_precision = 6  # Precision of the energy in the minimizer logger
+        self.GTH = {}              # Dictionary of GTH parameters per atom species
+        self.Vloc = None           # Local pseudopotential contribution
+        self.NbetaNL = 0           # Number of projector functions for the non-local gth potential
+        self.prj2beta = None       # Index matrix to map to the correct projector function
+        self.betaNL = None         # Atomic-centered projector functions
+        self.xc_type = None        # Type of functional that will be used
+        self.psp = None            # Type of GTH pseudopotential that will be used
+        self.is_converged = False  # Flag to determine if the object was converged or not
         self.initialize()
 
     def clear(self):
-        '''Initialize and clear intermediate results.'''
-        self.Y = None        # Orthogonal wave functions
-        self.n_spin = None   # Electronic densities per spin
-        self.dn_spin = None  # Gradient of electronic densities per spin
-        self.phi = None      # Hartree field
-        self.exc = None      # Exchange-correlation energy density
-        self.vxc = None      # Exchange-correlation potential
-        self.vsigma = None   # n times d exc/d |dn|^2
-        self.precomputed = {'Y': self.Y, 'n': self.n, 'n_spin': self.n_spin,
-                            'dn_spin': self.dn_spin, 'phi': self.phi, 'vxc': self.vxc,
-                            'vsigma': self.vsigma}
+        """Initialize and clear intermediate results."""
+        self.Y = None          # Orthogonal wave functions
+        self.n_spin = None     # Electronic densities per spin
+        self.dn_spin = None    # Gradient of electronic densities per spin
+        self.tau = None        # Kinetic energy densities per spin
+        self.phi = None        # Hartree field
+        self.exc = None        # Exchange-correlation energy density
+        self.vxc = None        # Exchange-correlation potential
+        self.vsigma = None     # n times d exc/d |dn|^2
+        self.vtau = None       # d exc/d tau
+        self.precomputed = {}  # Dictionary of precomputed values not to be saved
         return self
 
     def initialize(self):
-        '''Validate inputs, update them and build all necessary parameters.'''
+        """Validate inputs, update them and build all necessary parameters."""
         self.xc = parse_functionals(self.xc)
-        self.psp = parse_psp(self.xc)
+        self.xc_type = parse_xc_type(self.xc)
         # Build the atoms object if necessary and make a copy
         # This way the atoms object in scf is independent but we ensure that both atoms are build
         if not self.atoms.is_built:
             self.atoms = copy.copy(self.atoms.build())
         else:
             self.atoms = copy.copy(self.atoms)
         self._set_potential()
         self._init_W()
-        self.print_precision = int(abs(np.log10(self.etol))) + 1
         return self
 
     def run(self, **kwargs):
-        '''Run the self-consistent field (SCF) calculation.'''
+        """Run the self-consistent field (SCF) calculation."""
         if self.log.level <= logging.DEBUG:
             info()
         self.log.debug(f'\n--- System information ---\n{self.atoms}\n'
-                       f'Spin handling: {"un" if self.atoms.Nspin == 1 else ""}polarized\n'
+                       f'Spin handling: {"un" if self.atoms.Nspin == 2 else ""}restricted\n'
                        f'Number of states: {self.atoms.Nstate}\n'
                        f'Occupation per state:\n{self.atoms.f}\n'
-                       f'\n--- Cell information ---\nSide lengths: {self.atoms.a} Bohr\n'
+                       f'\n--- Cell information ---\nSide lengths: {self.atoms.a} a0\n'
                        f'Sampling per axis: {self.atoms.s}\n'
-                       f'Cut-off energy: {self.atoms.ecut} Hartree\n'
-                       f'Compression: {len(self.atoms.G2) / len(self.atoms.G2c):.5f}\n'
+                       f'Cut-off energy: {self.atoms.ecut} Eh\n'
+                       f'Compression: {len(self.atoms.G2c) / len(self.atoms.G2):.5f}\n'
                        f'\n--- Calculation information ---\n{self}\n\n--- SCF data ---')
 
         # Calculate Ewald energy that only depends on the system geometry
         self.energies.Eewald = get_Eewald(self.atoms)
 
         if 'mock_xc' in self.xc:
             self.log.warning('Usage of mock functional detected.')
 
         # Start minimization procedures
         Etots = []
         minimizer_log = {}
         for imin in self.min:
             try:
-                self.log.info(f'Start {IMPLEMENTED[imin].__name__}...')
+                self.log.info(f'Start {all_minimizer[imin].__name__}...')
             except KeyError:
-                self.log.exception(f'No minimizer found for "{imin}"')
+                self.log.exception(f'No minimizer found for "{imin}".')
                 raise
             start = time.perf_counter()
-            Elist = IMPLEMENTED[imin](self, self.min[imin], **kwargs)  # Call minimizer
+            Elist = all_minimizer[imin](self, self.min[imin], **kwargs)  # Call minimizer
             end = time.perf_counter()
             minimizer_log[imin] = {}  # Create an entry for the current minimizer
             minimizer_log[imin]['time'] = end - start  # Save time in dictionary
             minimizer_log[imin]['iter'] = len(Elist)  # Save iterations in dictionary
             Etots += Elist  # Append energies from minimizer
             # Do not start other minimizations if one converged
-            if len(Etots) > 1 and abs(Etots[-2] - Etots[-1]) < self.etol:
+            if self.is_converged:
                 break
-        if len(Etots) > 1 and abs(Etots[-2] - Etots[-1]) < self.etol:
+        if self.is_converged:
             self.log.info(f'SCF converged after {len(Etots)} iterations.')
         else:
             self.log.warning('SCF not converged!')
 
         # Print SCF data
         self.log.debug('\n--- SCF results ---')
         t_tot = 0
         for imin in minimizer_log:
             N = minimizer_log[imin]['iter']
             t = minimizer_log[imin]['time']
             t_tot += t
             self.log.debug(f'Minimizer: {imin}'
-                           f'\nIterations:\t{N}'
-                           f'\nTime:\t\t{t:.5f} s'
-                           f'\nTime/Iteration:\t{t / N:.5f} s')
+                           f'\nIterations: {N}'
+                           f'\nTime: {t:.5f} s'
+                           f'\nTime/Iteration: {t / N:.5f} s')
         self.log.info(f'Total SCF time: {t_tot:.5f} s')
 
         # Calculate SIC energy if desired
         if self.sic:
             self.energies.Esic = get_Esic(self, self.Y)
 
+        # Print the S^2 expecation value for unrestricted calculations
+        if self.atoms.Nspin == 2:
+            self.log.info(f'<S^2> = {get_spin_squared(self):.6e}')
         # Print energy data
         if self.log.level <= logging.DEBUG:
-            self.log.debug(f'\n--- Energy data ---\n{self.energies}')
+            self.log.debug('\n--- Energy data ---\n'
+                           f'Eigenenergies:\n{get_epsilon(self, self.W)}\n'
+                           f'\n{self.energies}')
         else:
-            self.log.info(f'Total energy: {self.energies.Etot:.9f} Eh')
+            self.log.info(f'Etot = {self.energies.Etot:.9f} Eh')
         return self.energies.Etot
 
     kernel = run
 
     def recenter(self, center=None):
-        '''Recenter the system inside the cell.
+        """Recenter the system inside the cell.
 
         Keyword Args:
             center (float | list | tuple | ndarray | None): Point to center the system around.
-        '''
+        """
         # Get the COM before centering the atoms
         com = center_of_mass(self.atoms.X)
 
         # Run the recenter method of the atoms object
         self.atoms.recenter(center=center)
 
         if center is None:
@@ -228,80 +245,97 @@
         # Recalculate the pseudopotential since it depends on the structure factor
         self._set_potential()
         # Clear intermediate results to make sure no one uses the unshifted results
         self.clear()
         return self
 
     def _set_potential(self):
-        '''Build the potential.'''
+        """Build the potential."""
         atoms = self.atoms
+
+        # If pot is no supported potential it can be a path to a directory containing GTH files
+        if self.pot.lower() != 'gth' and self.pot.lower() not in all_potentials:
+            self.psp = self.pot
+            self.pot = 'gth'
+        else:
+            self.pot = self.pot.lower()
+            if 'gga' in self.xc_type:
+                self.psp = 'pbe'
+            else:
+                self.psp = 'pade'
+
         if self.pot == 'gth':
             for ia in range(atoms.Natoms):
-                self.GTH[atoms.atom[ia]] = read_gth(atoms.atom[ia], atoms.Z[ia], xc=self.psp)
+                self.GTH[atoms.atom[ia]] = read_gth(atoms.atom[ia], atoms.Z[ia], psp_path=self.psp)
             # Set up the local and non-local part
             self.Vloc = init_gth_loc(self)
             self.NbetaNL, self.prj2beta, self.betaNL = init_gth_nonloc(self)
         else:
             self.Vloc = init_pot(self)
         return
 
     def _init_W(self):
-        '''Initialize wave functions.'''
-        if self.guess in ('gauss', 'gaussian'):
-            # Start with gaussians at atom positions
-            self.W = guess_gaussian(self, complex=True)
-        elif self.guess in ('rand', 'random'):
+        """Initialize wave functions."""
+        if self.guess in ('rand', 'random'):
             # Start with randomized, complex basis functions with a random seed
-            self.W = guess_random(self, complex=True)
+            self.W = guess_random(self, symmetric=self.symmetric)
         elif self.guess in ('pseudo', 'pseudo_rand', 'pseudo_random'):
             # Start with pseudo-random numbers, mostly to compare with SimpleDFT
-            self.W = guess_pseudo(self, seed=1234)
+            self.W = guess_pseudo(self, symmetric=self.symmetric)
         else:
-            self.log.error(f'No guess found for "{self.guess}"')
+            self.log.error(f'No guess found for "{self.guess}".')
         return
 
     def __repr__(self):
-        '''Print the parameters stored in the SCF object.'''
+        """Print the parameters stored in the SCF object."""
         # Use chr(10) to create a linebreak since backslashes are not allowed in f-strings
         return f'XC functionals: {self.xc}\n' \
                f'Potential: {self.pot}\n' \
                f'{f"GTH files: {self.psp}" + chr(10) if self.pot == "gth" else ""}' \
                f'Starting guess: {self.guess}\n' \
-               f'Convergence tolerance: {self.etol}\n' \
+               f'Symmetric guess: {self.symmetric}\n' \
+               f'Energy convergence tolerance: {self.etol} Eh\n' \
+               f'Gradient convergence tolerance: {self.gradtol}\n' \
                f'Non-local contribution: {self.NbetaNL > 0}'
 
     @property
     def verbose(self):
-        '''Verbosity level.'''
+        """Verbosity level."""
         return self._verbose
 
     @verbose.setter
     def verbose(self, level):
         self._verbose = get_level(level)
         self.log.verbose = self._verbose
         return
 
 
 class RSCF(SCF):
-    '''SCF class for spin-paired systems.
+    """SCF class for spin-paired systems.
 
     Inherited from :class:`eminus.scf.SCF`.
-    '''
+
+    In difference to the SCF class, this class will not build the original Atoms object, only the
+    one attributed to the class.
+    """
     def initialize(self):
-        '''Validate inputs, update them and build all necessary parameters.'''
+        """Validate inputs, update them and build all necessary parameters."""
         self.atoms = copy.copy(self.atoms)
         self.atoms._set_states(Nspin=1)
         super().initialize()
         return self
 
 
 class USCF(SCF):
-    '''SCF class for spin-polarized systems.
+    """SCF class for spin-polarized systems.
 
     Inherited from :class:`eminus.scf.SCF`.
-    '''
+
+    In difference to the SCF class, this class will not build the original Atoms object, only the
+    one attributed to the class.
+    """
     def initialize(self):
-        '''Validate inputs, update them and build all necessary parameters.'''
+        """Validate inputs, update them and build all necessary parameters."""
         self.atoms = copy.copy(self.atoms)
         self.atoms._set_states(Nspin=2)
         super().initialize()
         return self
```

### Comparing `eminus-2.4.0/eminus/tools.py` & `eminus-2.5.0/eminus/dft.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,327 +1,320 @@
 #!/usr/bin/env python3
-'''Various tools to check physical properties.'''
+"""Main DFT functions based on the DFT++ formulation."""
 import numpy as np
-from numpy.linalg import norm
-from scipy.optimize import minimize_scalar
+from numpy.random import Generator, SFC64
+from scipy.linalg import eig, eigh, eigvalsh, inv, sqrtm
 
-from .dft import get_epsilon, get_grad_n_spin
-from .logger import log
+from .gga import calc_Vtau, get_grad_field, get_tau, gradient_correction
+from .gth import calc_Vnonloc
+from .utils import handle_spin_gracefully, pseudo_uniform
+from .xc import get_vxc
 
 
-def cutoff2gridspacing(E):
-    '''Convert plane wave energy cut-off to a real-space grid spacing.
+def solve_poisson(atoms, n):
+    """Solve the Poisson equation.
 
-    Reference: Phys. Rev. B 54, 14362.
+    Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
-        E (float): Energy in Hartree.
+        atoms: Atoms object.
+        n (ndarray): Real-space electronic density.
 
     Returns:
-        float: Grid spacing in Bohr.
-    '''
-    return np.pi / np.sqrt(2 * E)
+        ndarray: Hartree field.
+    """
+    # phi = -4 pi Linv(O(J(n)))
+    return -4 * np.pi * atoms.Linv(atoms.O(atoms.J(n)))
 
 
-def gridspacing2cutoff(h):
-    '''Convert real-space grid spacing to plane wave energy cut-off.
+def get_n_total(atoms, Y, n_spin=None):
+    """Calculate the total electronic density.
 
-    Reference: Phys. Rev. B 54, 14362.
+    Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
-        h (float): Grid spacing in Bohr.
+        atoms: Atoms object.
+        Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
+
+    Keyword Args:
+        n_spin (ndarray): Real-space electronic densities per spin channel.
 
     Returns:
-        float: Cut-off in Hartree.
-    '''
-    return 0.5 * (np.pi / h)**2
+        ndarray: Electronic density.
+    """
+    # Return the total density in the spin-paired case
+    if n_spin is not None:
+        return np.sum(n_spin, axis=0)
+
+    # n = (IW) F (IW)dag
+    Yrs = atoms.I(Y)
+    n = np.zeros(len(atoms.r))
+    for spin in range(atoms.Nspin):
+        n += np.sum(atoms.f[spin] * np.real(Yrs[spin].conj() * Yrs[spin]), axis=1)
+    return n
 
 
-def center_of_mass(coords, masses=None):
-    '''Calculate the center of mass for a set of coordinates and masses.
+def get_n_spin(atoms, Y):
+    """Calculate the electronic density per spin channel.
 
-    Args:
-        coords (ndarray): Array of real-space coordinates.
+    Reference: Comput. Phys. Commun. 128, 1.
 
-    Keyword Args:
-        masses (ndarray): Mass or weight for each coordinate.
+    Args:
+        atoms: Atoms object.
+        Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
 
     Returns:
-        ndarray: Center of mass.
-    '''
-    if masses is None:
-        masses = np.ones(len(coords))
-
-    return np.sum(masses * coords.T, axis=1) / np.sum(masses)
+        ndarray: Electronic densities per spin channel.
+    """
+    Yrs = atoms.I(Y)
+    n = np.empty((atoms.Nspin, len(atoms.r)))
+    for spin in range(atoms.Nspin):
+        n[spin] = np.sum(atoms.f[spin] * np.real(Yrs[spin].conj() * Yrs[spin]), axis=1)
+    return n
 
 
-def orbital_center(object, psirs):
-    '''Calculate the orbital center of masses, e.g., from localized orbitals.
+def get_n_single(atoms, Y):
+    """Calculate the single-electron densities.
 
     Args:
-        object: Atoms or SCF object.
-        psirs (ndarray): Set of orbitals in real-space.
+        atoms: Atoms object.
+        Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
 
     Returns:
-        bool: Center of masses.
-    '''
-    try:
-        atoms = object.atoms
-    except AttributeError:
-        atoms = object
-
-    coms = [np.array([])] * 2
-    Ncom = psirs.shape[2]
+        ndarray: Single-electron densities.
+    """
+    Yrs = atoms.I(Y)
+    n = np.empty((atoms.Nspin, len(atoms.r), atoms.Nstate))
     for spin in range(atoms.Nspin):
-        coms_spin = np.empty((Ncom, 3))
+        n[spin] = atoms.f[spin] * np.real(Yrs[spin].conj() * Yrs[spin])
+    return n
 
-        # Square orbitals
-        psi2 = np.real(psirs[spin, :, :].conj() * psirs[spin, :, :])
-        for i in range(Ncom):
-            coms_spin[i] = center_of_mass(atoms.r, psi2[:, i])
-        coms[spin] = coms_spin
-    return coms
 
+@handle_spin_gracefully
+def orth(atoms, W):
+    """Orthogonalize coefficient matrix W.
 
-def inertia_tensor(coords, masses=None):
-    '''Calculate the inertia tensor for a set of coordinates and masses.
+    Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
-        coords (ndarray): Array of real-space coordinates.
-
-    Keyword Args:
-        masses (ndarray): Mass or weight for each coordinate.
+        atoms: Atoms object.
+        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
-        ndarray: Inertia tensor.
-    '''
-    if masses is None:
-        masses = np.ones(len(coords))
-
-    # The inertia tensor for a set of point masses can be calculated with simple summation
-    # https://en.wikipedia.org/wiki/Moment_of_inertia#Definition_2
-    I = np.empty((3, 3))
-    I[0, 0] = np.sum(masses * (coords[:, 1]**2 + coords[:, 2]**2))
-    I[1, 1] = np.sum(masses * (coords[:, 0]**2 + coords[:, 2]**2))
-    I[2, 2] = np.sum(masses * (coords[:, 0]**2 + coords[:, 1]**2))
+        ndarray: Orthogonalized wave functions.
+    """
+    # Y = W (Wdag O(W))^-0.5
+    return W @ inv(sqrtm(W.conj().T @ atoms.O(W)))
 
-    I[0, 1] = I[1, 0] = -np.sum(masses * (coords[:, 0] * coords[:, 1]))
-    I[0, 2] = I[2, 0] = -np.sum(masses * (coords[:, 0] * coords[:, 2]))
-    I[1, 2] = I[2, 1] = -np.sum(masses * (coords[:, 1] * coords[:, 2]))
-    return I
 
+def get_grad(scf, spin, W, **kwargs):
+    """Calculate the energy gradient with respect to W.
 
-def get_dipole(scf, n=None):
-    '''Calculate the electric dipole moment.
-
-    This function does not account for periodcity, it may be a good idea to center the system.
-
-    Reference: J. Chem. Phys. 155, 224109.
+    Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         scf: SCF object.
+        spin (int): Spin variable to track weather to do the calculation for spin up or down.
+        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Keyword Args:
-        n (float): Real-space electronic density.
+        **kwargs: See :func:`H`.
 
     Returns:
-        ndarray: Electric dipole moment in e * Bohr.
-    '''
+        ndarray: Gradient.
+    """
     atoms = scf.atoms
-    if n is None:
-        n = scf.n
-    if scf.n is None:
-        log.error('There is no density to calculate a dipole.')
-        return 0
-
-    # Diple moment: mu = \sum Z X - \int n(r) r dr
-    mu = np.array([0, 0, 0], dtype=float)
-    for i in range(atoms.Natoms):
-        mu += atoms.Z[i] * atoms.X[i]
-
-    dV = atoms.Omega / np.prod(atoms.s)
-    for dim in range(3):
-        mu[dim] -= dV * np.sum(n * atoms.r[:, dim])
-    return mu
+    F = np.diag(atoms.f[spin])
+    HW = H(scf, spin, W, **kwargs)
+    WHW = W[spin].conj().T @ HW
+    # U = Wdag O(W)
+    OW = atoms.O(W[spin])
+    U = W[spin].conj().T @ OW
+    invU = inv(U)
+    U12 = sqrtm(invU)
+    # Htilde = U^-0.5 Wdag H(W) U^-0.5
+    Ht = U12 @ WHW @ U12
+    # grad E = H(W) - O(W) U^-1 (Wdag H(W)) (U^-0.5 F U^-0.5) + O(W) (U^-0.5 Q(Htilde F - F Htilde))
+    return (HW - (OW @ invU) @ WHW) @ (U12 @ F @ U12) + OW @ (U12 @ Q(Ht @ F - F @ Ht, U))
 
 
-def get_ip(scf):
-    '''Calculate the ionization potential by calculating the negative HOMO energy.
+def H(scf, spin, W, dn_spin=None, phi=None, vxc=None, vsigma=None, vtau=None):
+    """Left-hand side of the eigenvalue equation.
 
-    Reference: Physica 1, 104.
+    Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         scf: SCF object.
+        spin (int): Spin variable to track weather to do the calculation for spin up or down.
+        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
+
+    Keyword Args:
+        dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        phi (ndarray): Hartree field.
+        vxc (ndarray): Exchange-correlation potential.
+        vsigma (ndarray): Contracted gradient potential derivative.
+        vtau (ndarray): Kinetic energy gradient potential derivative.
 
     Returns:
-        float: Ionization potential in Hartree.
-    '''
-    epsilon = get_epsilon(scf, scf.W)
-    # Add up spin states
-    epsilon = np.sum(epsilon, axis=0)
-    return -epsilon[-1]
+        ndarray: Hamiltonian applied on W.
+    """
+    atoms = scf.atoms
 
+    # If dn_spin is None all other keyword arguments are None by design
+    # In that case precompute values from the SCF class
+    if dn_spin is None:
+        dn_spin, phi, vxc, vsigma, vtau = H_precompute(scf, W)
+
+    # This calculate the representation in the reciprocal space
+    Gvxc = atoms.J(vxc[spin])
+    # Calculate the gradient correction to the potential if a GGA functional is used
+    if 'gga' in scf.xc_type:
+        Gvxc = Gvxc - gradient_correction(atoms, spin, dn_spin, vsigma)
+    # Vkin = -0.5 L(W)
+    Vkin_psi = -0.5 * atoms.L(W[spin])
+    # Veff = Jdag(Vion) + Jdag(O(J(vxc))) + Jdag(O(phi))
+    # We get the full potential in the functional definition (different to the DFT++ notation)
+    # Normally Vxc = Jdag(O(J(exc))) + diag(exc') Jdag(O(J(n))) (for LDA functionals)
+    Veff = scf.Vloc + atoms.Jdag(atoms.O(Gvxc + phi))
+    Vnonloc_psi = calc_Vnonloc(scf, spin, W)
+    Vtau_psi = calc_Vtau(scf, spin, W, vtau)
+    # H = Vkin + Idag(diag(Veff))I + Vnonloc (+ Vtau)
+    # Diag(a) * B can be written as a * B if a is a column vector
+    return Vkin_psi + atoms.Idag(Veff[:, None] * atoms.I(W[spin])) + Vnonloc_psi + Vtau_psi
 
-def check_ortho(object, func, eps=1e-9):
-    '''Check the orthogonality condition for a set of functions.
 
-    Args:
-        object: Atoms or SCF object.
-        func (ndarray): Discretized set of functions.
+def H_precompute(scf, W):
+    """Create precomputed values as intermediate results.
 
-    Keyword Args:
-        eps (float): Tolerance for the condition.
+    Args:
+        scf: SCF object.
+        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
-        bool: Orthogonality status for the set of functions.
-    '''
-    func = np.atleast_3d(func)
-    try:
-        atoms = object.atoms
-    except AttributeError:
-        atoms = object
-    # It makes no sense to calculate anything for only one function
-    if atoms.Nstate == 1:
-        log.warning('Need at least two functions to check their orthogonality.')
-        return True
-
-    # We integrate over our cell, the integration borders then become a=0 and b=cell length
-    # The integration prefactor dV is (b-a)/n, with n as the sampling
-    # For a 3d integral we have to multiply for every direction
-    dV = atoms.Omega / np.prod(atoms.s)
-
-    ortho_bool = True
-    # Check the condition for every combination
-    # Orthogonality condition: \int func1^* func2 dr = 0
-    for spin in range(atoms.Nspin):
-        for i in range(atoms.Nstate):
-            for j in range(i + 1, atoms.Nstate):
-                res = dV * np.sum(func[spin, :, i].conj() * func[spin, :, j])
-                tmp_bool = abs(res) < eps
-                ortho_bool *= tmp_bool
-                log.debug(f'Function {i} and {j}:\n\tValue: {res:.7f}\n\tOrthogonal: {tmp_bool}')
-    log.info(f'Orthogonal: {ortho_bool}')
-    return ortho_bool
+        tuple[ndarray, ndarray, ndarray, ndarray, ndarray]: dn_spin, phi, vxc, vsigma, and vtau
+    """
+    # We are calculating everything here over both spin channels
+    # In theory we would be fine/faster by only calculating the currently used spin channel
+    atoms = scf.atoms
+    Y = orth(atoms, W)
+    n_spin = get_n_spin(atoms, Y)
+    n = get_n_total(atoms, Y, n_spin)
+    if 'gga' in scf.xc_type:
+        dn_spin = get_grad_field(atoms, n_spin)
+    else:
+        dn_spin = None
+    if scf.xc_type == 'meta-gga':
+        tau = get_tau(atoms, Y)
+    else:
+        tau = None
+    phi = solve_poisson(atoms, n)
+    vxc, vsigma, vtau = get_vxc(scf.xc, n_spin, atoms.Nspin, dn_spin, tau)
+    return dn_spin, phi, vxc, vsigma, vtau
 
 
-def check_norm(object, func, eps=1e-9):
-    '''Check the normalization condition for a set of functions.
+def Q(inp, U):
+    """Operator needed to calculate gradients with non-constant occupations.
 
-    Args:
-        object: Atoms or SCF object.
-        func (ndarray): Discretized set of functions.
+    Reference: Comput. Phys. Commun. 128, 1.
 
-    Keyword Args:
-        eps (float): Tolerance for the condition.
+    Args:
+        inp (ndarray): Coefficients input array.
+        U (ndarray): Overlap of wave functions.
 
     Returns:
-        bool: Normalization status for the set of functions.
-    '''
-    func = np.atleast_3d(func)
-    try:
-        atoms = object.atoms
-    except AttributeError:
-        atoms = object
-    # We integrate over our cell, the integration borders then become a=0 and b=cell length
-    # The integration prefactor dV is (b-a)/n, with n as the sampling
-    # For a 3d integral we have to multiply for every direction
-    dV = atoms.Omega / np.prod(atoms.s)
-
-    norm_bool = True
-    # Check the condition for every function
-    # Normality condition: \int func^* func dr = 1
-    for spin in range(atoms.Nspin):
-        for i in range(atoms.Nstate):
-            res = dV * np.sum(func[spin, :, i].conj() * func[spin, :, i])
-            tmp_bool = abs(1 - res) < eps
-            norm_bool *= tmp_bool
-            log.debug(f'Function {i}:\n\tValue: {res:.7f}\n\tNormalized: {tmp_bool}')
-    log.info(f'Normalized: {norm_bool}')
-    return norm_bool
+        ndarray: Q operator result.
+    """
+    mu, V = eig(U)
+    mu = mu[:, None]
+    denom = np.sqrt(mu) @ np.ones((1, len(mu)))
+    denom2 = denom + denom.conj().T
+    return V @ ((V.conj().T @ inp @ V) / denom2) @ V.conj().T
+
 
+def get_psi(scf, W):
+    """Calculate eigenstates from H.
 
-def check_orthonorm(object, func):
-    '''Check the orthonormality conditions for a set of functions.
+    Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
-        object: Atoms or SCF object.
-        func (ndarray): Discretized set of functions.
+        scf: SCF object.
+        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
-        bool: Orthonormality status for the set of functions.
-    '''
-    try:
-        atoms = object.atoms
-    except AttributeError:
-        atoms = object
-    ortho_bool = check_ortho(atoms, func)
-    norm_bool = check_norm(atoms, func)
-    log.info(f'Orthonormal: {ortho_bool * norm_bool}')
-    return ortho_bool * norm_bool
+        ndarray: Eigenstates in reciprocal space.
+    """
+    atoms = scf.atoms
+    Y = orth(atoms, W)
+    psi = np.empty_like(Y)
+    for spin in range(atoms.Nspin):
+        mu = Y[spin].conj().T @ H(scf, spin, Y)
+        _, D = eigh(mu)
+        psi[spin] = Y[spin] @ D
+    return psi
 
 
-def get_isovalue(n, percent=85):
-    '''Find an isovalue that contains a specified percentage of the electronic density.
+def get_epsilon(scf, W):
+    """Calculate eigenvalues from H.
 
-    Args:
-        n (float): Real-space electronic density.
+    Reference: Comput. Phys. Commun. 128, 1.
 
-    Keyword Args:
-        percent (float): Amount of density that should be contained.
+    Args:
+        scf: SCF object.
+        W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Returns:
-        float: Isovalue that contains the specified percentage of the density.
-    '''
-    def deviation(isovalue):
-        n_mask = np.sum(n[n > isovalue])
-        return abs(percent - (n_mask / n_ref) * 100)
-
-    # Integrated density
-    n_ref = np.sum(n)
-    # Finding the isovalue is an optimization problem, minimizing the deviation above
-    # The problem is bound by zero (no density) and the maximum value in n
-    res = minimize_scalar(deviation, bounds=(0, np.max(n)), method='bounded')
-    return res.x
-
+        ndarray: Eigenvalues.
+    """
+    atoms = scf.atoms
+    Y = orth(atoms, W)
+    epsilon = np.empty((atoms.Nspin, atoms.Nstate))
+    for spin in range(atoms.Nspin):
+        mu = Y[spin].conj().T @ H(scf, spin, Y)
+        epsilon[spin] = np.sort(eigvalsh(mu))
+    return epsilon
 
-def get_tautf(scf):
-    '''Calculate the Thomas-Fermi kinetic energy densities per spin.
 
-    Reference: Phys. Lett. B 63, 395.
+def guess_random(scf, seed=42, symmetric=False):
+    """Generate random initial-guess coefficients as starting values.
 
     Args:
         scf: SCF object.
 
+    Keyword Args:
+        seed (int): Seed to initialize the random number generator.
+        symmetric (bool): Weather to use the same guess for both spin channels.
+
     Returns:
-        ndarray: Real space Thomas-Fermi kinetic energy density.
-    '''
+        ndarray: Initial-guess orthogonal wave functions in reciprocal space.
+    """
     atoms = scf.atoms
-    tautf = 3 / 10 * (atoms.Nspin * 3 * np.pi**2)**(2 / 3) * scf.n_spin**(5 / 3)
-
-    log.debug(f'Calculated Ekin:  {scf.energies.Ekin:.6f} Eh')
-    log.debug(f'Integrated tautf: {np.sum(tautf) * atoms.Omega / np.prod(atoms.s):.6f} Eh')
-    return tautf
-
+    rng = Generator(SFC64(seed))
+    if symmetric:
+        W = rng.standard_normal((len(atoms.G2c), atoms.Nstate)) + \
+            1j * rng.standard_normal((len(atoms.G2c), atoms.Nstate))
+        W = np.array([W] * atoms.Nspin)
+    else:
+        W = rng.standard_normal((atoms.Nspin, len(atoms.G2c), atoms.Nstate)) + \
+            1j * rng.standard_normal((atoms.Nspin, len(atoms.G2c), atoms.Nstate))
+    return orth(atoms, W)
 
-def get_tauw(scf):
-    '''Calculate the von Weizsäcker kinetic energy densities per spin.
 
-    Reference: Z. Phys. 96, 431.
+def guess_pseudo(scf, seed=1234, symmetric=False):
+    """Generate initial-guess coefficients using pseudo-random starting values.
 
     Args:
         scf: SCF object.
 
+    Keyword Args:
+        seed (int): Seed to initialize the random number generator.
+        symmetric (bool): Weather to use the same guess for both spin channels.
+
     Returns:
-        ndarray: Real space von Weizsäcker kinetic energy density.
-    '''
+        ndarray: Initial-guess orthogonal wave functions in reciprocal space.
+    """
     atoms = scf.atoms
-    if scf.dn_spin is None:
-        dn_spin = get_grad_n_spin(atoms, scf.n_spin)
+    if symmetric:
+        W = pseudo_uniform((1, len(atoms.G2c), atoms.Nstate), seed=seed)
+        W = np.array([W[0]] * atoms.Nspin)
     else:
-        dn_spin = scf.dn_spin
-    dn2 = norm(dn_spin, axis=2)**2
-    tauw = dn2 / (8 * scf.n_spin)
-
-    # For one- and two-electron systems the integrated KED has to be the same as the calculated KE
-    log.debug(f'Calculated Ekin:  {scf.energies.Ekin:.6f} Eh')
-    log.debug(f'Integrated tauw:  {np.sum(tauw) * atoms.Omega / np.prod(atoms.s):.6f} Eh')
-    return tauw
+        W = pseudo_uniform((atoms.Nspin, len(atoms.G2c), atoms.Nstate), seed=seed)
+    return orth(atoms, W)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eminus-2.4.0/eminus/units.py` & `eminus-2.5.0/eminus/units.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,157 +1,157 @@
 #!/usr/bin/env python3
-'''Collection of constants and unit conversion functions.
+"""Collection of constants and unit conversion functions.
 
 For more about atomic units, see: https://en.wikipedia.org/wiki/Hartree_atomic_units
-'''
+"""
 # Ha in eV (https://en.wikipedia.org/wiki/Hartree)
 electronvolt = eV = 27.211386245988
 # Ha in kcal/mol (https://en.wikipedia.org/wiki/Hartree)
 kcalmol = 627.5094740631
-# a0 in Å (https://en.wikipedia.org/wiki/Bohr_radius)
+# a0 in Angstrom (https://en.wikipedia.org/wiki/Bohr_radius)
 Angstrom = A = 0.529177210903
-# e * a0 in D (https://en.wikipedia.org/wiki/Hartree_atomic_units)
+# e * a0 in Debye (https://en.wikipedia.org/wiki/Hartree_atomic_units)
 Debye = D = 2.541746473
 
 
 def ha2ev(E):
-    '''Convert Hartree to electronvolt.
+    """Convert Hartree to electronvolt.
 
     Args:
         E (float | ndarray): Energy in Hartree.
 
     Returns:
         float | ndarray: Energy in electronvolt.
-    '''
+    """
     return E * electronvolt
 
 
 def ev2ha(E):
-    '''Convert electronvolt to Hartree.
+    """Convert electronvolt to Hartree.
 
     Args:
         E (float | ndarray): Energy in electronvolt.
 
     Returns:
         float | ndarray: Energy in Hartree.
-    '''
+    """
     return E / electronvolt
 
 
 def ha2kcalmol(E):
-    '''Convert Hartree to kcal/mol.
+    """Convert Hartree to kcal/mol.
 
     Args:
         E (float | ndarray): Energy in Hartree.
 
     Returns:
         float | ndarray: Energy in kcal/mol.
-    '''
+    """
     return E * kcalmol
 
 
 def kcalmol2ha(E):
-    '''Convert kcal/mol to Hartree.
+    """Convert kcal/mol to Hartree.
 
     Args:
         E (float | ndarray): Energy in kcal/mol.
 
     Returns:
         float | ndarray: Energy in Hartree.
-    '''
+    """
     return E / kcalmol
 
 
 def ev2kcalmol(E):
-    '''Convert electronvolt to kcal/mol.
+    """Convert electronvolt to kcal/mol.
 
     Args:
         E (float | ndarray): Energy in electronvolt.
 
     Returns:
         float | ndarray: Energy in kcal/mol.
-    '''
+    """
     return ha2kcalmol(ev2ha(E))
 
 
 def kcalmol2ev(E):
-    '''Convert kcal/mol to electronvolt.
+    """Convert kcal/mol to electronvolt.
 
     Args:
         E (float | ndarray): Energy in kcal/mol.
 
     Returns:
         float | ndarray: Energy in electronvolt.
-    '''
+    """
     return ha2ev(kcalmol2ha(E))
 
 
 def ha2ry(E):
-    '''Convert Hartree to Rydberg.
+    """Convert Hartree to Rydberg.
 
     Args:
         E (float | ndarray): Energy in Hartree.
 
     Returns:
         float | ndarray: Energy in Rydberg.
-    '''
+    """
     return 2 * E
 
 
 def ry2ha(E):
-    '''Convert Rydberg to Hartree.
+    """Convert Rydberg to Hartree.
 
     Args:
         E (float | ndarray): Energy in Rydberg.
 
     Returns:
         float | ndarray: Energy in Hartree.
-    '''
+    """
     return E / 2
 
 
 def ang2bohr(r):
-    '''Convert Angstrom to Bohr.
+    """Convert Angstrom to Bohr.
 
     Args:
         r (float | ndarray): Length in Angstrom.
 
     Returns:
         float | ndarray: Length in Bohr.
-    '''
+    """
     return r / Angstrom
 
 
 def bohr2ang(r):
-    '''Convert Bohr to Angstrom.
+    """Convert Bohr to Angstrom.
 
     Args:
         r (float | ndarray): Length in Bohr.
 
     Returns:
         float | ndarray: Length in Angstrom.
-    '''
+    """
     return r * Angstrom
 
 
 def ebohr2d(p):
-    '''Convert e * Bohr to Debye.
+    """Convert e * Bohr to Debye.
 
     Args:
         p (float | ndarray): Electric dipole moment in e * Bohr.
 
     Returns:
         float | ndarray: Electric dipole moment in Debye.
-    '''
+    """
     return p * Debye
 
 
 def d2ebohr(p):
-    '''Convert Debye to e * Bohr.
+    """Convert Debye to e * Bohr.
 
     Args:
         p (float | ndarray): Electric dipole moment in Debye.
 
     Returns:
         float | ndarray: Electric dipole moment in e * Bohr.
-    '''
+    """
     return p / Debye
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eminus-2.4.0/eminus/utils.py` & `eminus-2.5.0/eminus/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 #!/usr/bin/env python3
-'''Linear algebra calculation utilities.'''
+"""Linear algebra calculation utilities."""
 import functools
 
 import numpy as np
 from scipy.linalg import norm
 
 from .logger import log
 
 
 def dotprod(a, b):
-    '''Efficiently calculate the expression a * b.
+    """Efficiently calculate the expression a * b.
 
     Add an extra check to make sure the result is never zero since this function is used as a
     denominator in minimizers.
 
     Args:
         a (ndarray): Array of vectors.
         b (ndarray): Array of vectors.
 
     Returns:
         float: The expressions result
-    '''
+    """
     eps = 1e-15  # 2.22e-16 is the range of float64 machine precision
     # The dot product of complex vectors looks like the expression below, but this is slow
     # res = np.real(np.trace(a.conj().T @ b))
     # We can calculate the trace faster by taking the sum of the Hadamard product
     res = np.sum(a.conj() * b)
     if abs(res) < eps:
         return eps
     return np.real(res)
 
 
-def Ylm_real(l, m, G):
-    '''Calculate real spherical harmonics from cartesian coordinates.
+def Ylm_real(l, m, G):  # noqa: C901
+    """Calculate real spherical harmonics from cartesian coordinates.
+
+    Reference: https://scipython.com/blog/visualizing-the-real-forms-of-the-spherical-harmonics/
 
     Args:
         l (int): Angular momentum number.
         m (int): Magnetic quantum number.
         G (ndarray): Recipocal lattice vector or array of lattice vectors.
 
     Returns:
         ndarray: Real spherical harmonics.
-    '''
+    """
     eps = 1e-9
     # Account for single vectors
     G = np.atleast_2d(G)
 
     # No need to calculate more for l=0
     if l == 0:
         return 0.5 * np.sqrt(1 / np.pi) * np.ones(len(G))
@@ -96,61 +98,80 @@
         elif m == 1:
             return 0.25 * np.sqrt(21 / 2 / np.pi) * sin_theta * (5 * cos_theta**2 - 1) * np.cos(phi)
         elif m == 2:
             return 0.25 * np.sqrt(105 / np.pi) * sin_theta**2 * cos_theta * np.cos(2 * phi)
         elif m == 3:
             return 0.25 * np.sqrt(35 / 2 / np.pi) * sin_theta**3 * np.cos(3 * phi)
 
-    log.error(f'No definition found for Ylm({l}, {m})')
-    return
+    log.error(f'No definition found for Ylm({l}, {m}).')
+    return None
 
 
 def handle_spin_gracefully(func):
-    '''Handle spin calculating the function for each channel seperately.
+    """Handle spin calculating the function for each channel seperately.
 
     This can only be applied if the only spin-dependent indexing is the wave function W.
 
     Implementing the explicit handling of spin adds an extra layer of complexity where one has to
     loop over the spin states in many places. We can hide this complexity using this decorator while
     still supporting many usecases, e.g., the operators previously act on arrays containing wave
     functions of all states and of one state only. This decorator maintains this functionality and
     adds the option to act on arrays containing wave functions of all spins and all states as well.
 
     Args:
         func (Callable): Function that acts on spin-states.
 
     Returns:
         Callable: Decorator.
-    '''
+    """
     @functools.wraps(func)
     def decorator(object, W, *args, **kwargs):
         if W.ndim == 3:
             # If one is brave enough one could add multiprocessing over spin states right here
             return np.asarray([func(object, Wspin, *args, **kwargs) for Wspin in W])
         return func(object, W, *args, **kwargs)
     return decorator
 
 
 def pseudo_uniform(size, seed=1234):
-    '''Lehmer random number generator, following MINSTD.
+    """Lehmer random number generator, following MINSTD.
 
     Reference: Commun. ACM. 12, 85.
 
     Args:
         size (tuple): Dimension of the array to create.
 
     Keyword Args:
         seed (int): Seed to initialize the random number generator.
 
     Returns:
         ndarray: Array with (pseudo) random numbers.
-    '''
+    """
     W = np.zeros(size, dtype=complex)
     mult = 48271
     mod = (2**31) - 1
     x = (seed * mult + 1) % mod
     for i in range(size[0]):
         for j in range(size[1]):
             for k in range(size[2]):
                 x = (x * mult + 1) % mod
                 W[i, j, k] = x / mod
     return W
+
+
+def add_maybe_none(a, b):
+    """Add a and b together, when one or both can potentially be None.
+
+    Args:
+        a (ndarray): Array.
+        b (ndarray): Array.
+
+    Returns:
+        ndarray: Sum of a and b.
+    """
+    if a is None and b is None:
+        return None
+    if a is None:
+        return b
+    if b is None:
+        return a
+    return a + b
```

### Comparing `eminus-2.4.0/eminus/version.py` & `eminus-2.5.0/eminus/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #!/usr/bin/env python3
-'''Package version number and version info function.'''
+"""Package version number and version info function."""
 import importlib
 import platform
 import sys
 
-__version__ = '2.4.0'
+__version__ = '2.5.0'
 logo = (' ___ _____ _ ___ _ _ ___ \n'
         '| -_|     | |   | | |_ -|\n'
         '|___|_|_|_|_|_|_|___|___|\n')
 
 
 def info():
-    '''Print version numbers and availability of packages.'''
+    """Print version numbers and availability of packages."""
     dependencies = ('numpy', 'scipy')
     extras = ('torch', 'pyscf', 'plotly', 'nglview')
-    dev = ('notebook', 'pylibxc', 'pytest', 'flake8', 'sphinx', 'furo')
+    dev = ('notebook', 'pylibxc', 'pytest', 'sphinx', 'furo')
 
     print(logo)
     print('--- Platform infos ---'
-          f'\nPlatform  : {platform.system()} {platform.machine()}'
-          f'\nRelease   : {platform.release()} {platform.version()}'
+          f'\nPlatform : {platform.system()} {platform.machine()}'
+          f'\nRelease  : {platform.release()} {platform.version()}'
           '\n\n--- Version infos ---'
-          f'\npython    : {sys.version.split()[0]}'
-          f'\neminus    : {__version__}')
+          f'\npython   : {sys.version.split()[0]}'
+          f'\neminus   : {__version__}')
     for pkg in dependencies + extras + dev:
         try:
             module = importlib.import_module(pkg)
             try:
-                print(f'{pkg.ljust(10)}: {module.__version__}')
+                print(f'{pkg:<9}: {module.__version__}')
             except AttributeError:
                 # pylibxc does not use the standard version identifier
-                print(f'{pkg.ljust(10)}: {module.version.__version__}')
+                print(f'{pkg:<9}: {module.version.__version__}')
         except ModuleNotFoundError:
             if pkg in dependencies:
-                print(f'{pkg.ljust(10)}: Dependency not installed')
+                print(f'{pkg:<9}: Dependency not installed')
             elif pkg in extras:
-                print(f'{pkg.ljust(10)}: Extra not installed')
+                print(f'{pkg:<9}: Extra not installed')
     return
 
 
 if __name__ == '__main__':
     info()
```

### Comparing `eminus-2.4.0/eminus/xc/README.md` & `eminus-2.5.0/eminus/xc/README.md`

 * *Files identical despite different names*

### Comparing `eminus-2.4.0/eminus/xc/gga_c_chachiyo.py` & `eminus-2.5.0/eminus/xc/gga_c_chachiyo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/env python3
-'''Chachiyo GGA correlation.
+"""Chachiyo GGA correlation.
 
 Reference: Comput. Theor. Chem. 1172, 112669.
-'''
+"""
 import numpy as np
 from numpy.linalg import norm
 
 from .lda_c_chachiyo_mod import chachiyo_scaling_mod as weight_function
 
 
-def gga_c_chachiyo(n, exc_only=False, dn_spin=None, **kwargs):
-    '''Chachiyo parametrization of the correlation functional (spin-paired).
+def gga_c_chachiyo(n, dn_spin=None, **kwargs):
+    """Chachiyo parametrization of the correlation functional (spin-paired).
 
     Corresponds to the functional with the label GGA_C_CHACHIYO and ID 309 in Libxc.
+
     Reference: Comput. Theor. Chem. 1172, 112669.
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
         dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray, ndarray]: Chachiyo correlation energy density, potential and vsigma.
-    '''
+    """
     h = 0.06672632  # 0.5 * 0.00847 * 16 * (3 / np.pi)**(1 / 3)
 
     # ### Start lda_c_chachiyo_mod ### #
     a = -0.01554535  # (np.log(2) - 1) / (2 * np.pi**2)
     b = 20.4562557
 
     rs = (3 / (4 * np.pi * n))**(1 / 3)
@@ -39,74 +40,71 @@
     # ### End lda_c_chachiyo_mod ### #
 
     norm_dn = norm(dn_spin[0], axis=1)
     t = (np.pi / 3)**(1 / 6) / 4 * norm_dn / n**(7 / 6)
     t2 = t**2
     gec = 1 + t2
     expgec = gec**(h / ec)
-    if exc_only:
-        return ec * expgec, None, None
 
     # ### Start lda_c_chachiyo_mod ### #
     vc = ec + a * b * (2 + rs) / (3 * (b + b * rs + rs2))
     # ### End lda_c_chachiyo_mod ### #
 
     term1 = h * (1 - 1 / gec)
     term2 = h * np.log(gec) * (1 - vc / ec)
     gvc = (vc - 7 / 3 * term1 + term2) * expgec
 
     vsigmac = n * expgec * term1 / norm_dn**2
     return ec * expgec, np.array([gvc]), np.array([vsigmac])
 
 
-def gga_c_chachiyo_spin(n, zeta, exc_only=False, dn_spin=None, **kwargs):
-    '''Chachiyo parametrization of the correlation functional (spin-polarized).
+def gga_c_chachiyo_spin(n, zeta, dn_spin=None, **kwargs):
+    """Chachiyo parametrization of the correlation functional (spin-polarized).
 
     Corresponds to the functional with the label GGA_C_CHACHIYO and ID 309 in Libxc.
+
     Reference: Comput. Theor. Chem. 1172, 112669.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
         dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray, ndarray]: Chachiyo correlation energy density, potential and vsigma.
-    '''
+    """
     h = 0.06672632  # 0.5 * 0.00847 * 16 * (3 / np.pi)**(1 / 3)
 
     # ### Start lda_c_chachiyo_spin_mod ### #
     a0 = -0.01554535   # (np.log(2) - 1) / (2 * np.pi**2)
     a1 = -0.007772675  # (np.log(2) - 1) / (4 * np.pi**2)
     b0 = 20.4562557
     b1 = 27.4203609
 
     rs = (3 / (4 * np.pi * n))**(1 / 3)
     rs2 = rs**2
 
-    fzeta, dfdzeta = weight_function(zeta, exc_only=exc_only)
+    fzeta, dfdzeta = weight_function(zeta)
 
     ec0inner = 1 + b0 / rs + b0 / rs2
     ec1inner = 1 + b1 / rs + b1 / rs2
     ec0 = a0 * np.log(ec0inner)
     ec1 = a1 * np.log(ec1inner)
 
     ec = ec0 + (ec1 - ec0) * fzeta
     # ### End lda_c_chachiyo_spin_mod ### #
 
     norm_dn = norm(dn_spin[0] + dn_spin[1], axis=1)
     t = (np.pi / 3)**(1 / 6) / 4 * norm_dn / n**(7 / 6)
     t2 = t**2
     gec = 1 + t2
     expgec = gec**(h / ec)
-    if exc_only:
-        return ec * expgec, None, None
 
     # ### Start lda_c_chachiyo_spin_mod ### #
     factor = -1 / rs2 - 2 / rs**3
     dec0drs = a0 / ec0inner * b0 * factor
     dec1drs = a1 / ec1inner * b1 * factor
     decdrs = dec0drs + (dec1drs - dec0drs) * fzeta
     # prefactor = ec - rs / 3 * decdrs
```

### Comparing `eminus-2.4.0/eminus/xc/gga_c_pbe.py` & `eminus-2.5.0/eminus/xc/gga_c_pbe.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,91 @@
 #!/usr/bin/env python3
-'''Perdew-Burke-Ernzerhof GGA correlation.
+"""Perdew-Burke-Ernzerhof GGA correlation.
 
 Reference: Phys. Rev. Lett. 78, 1396.
-'''
+"""
 import numpy as np
 from numpy.linalg import norm
 
 from .lda_c_pw_mod import lda_c_pw_mod, lda_c_pw_mod_spin
 
 
-def gga_c_pbe(n, beta=0.06672455060314922, exc_only=False, dn_spin=None, **kwargs):
-    '''Perdew-Burke-Ernzerhof parametrization of the correlation functional (spin-paired).
+def gga_c_pbe(n, beta=0.06672455060314922, dn_spin=None, **kwargs):
+    """Perdew-Burke-Ernzerhof parametrization of the correlation functional (spin-paired).
 
     Corresponds to the functional with the label GGA_C_PBE and ID 130 in Libxc.
+
     Reference: Phys. Rev. Lett. 78, 1396.
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
         beta (float): Functional parameter.
-        exc_only (bool): Only calculate the exchange-correlation energy density.
         dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray, ndarray]: PBE correlation energy density, potential, and vsigma.
-    '''
+    """
     gamma = (1 - np.log(2)) / np.pi**2
 
     pi34 = (3 / (4 * np.pi))**(1 / 3)
     rs = pi34 * n**(-1 / 3)
     norm_dn = norm(dn_spin[0], axis=1)
-    ec, vc, _ = lda_c_pw_mod(n, exc_only=exc_only, **kwargs)
+    ec, vc, _ = lda_c_pw_mod(n, **kwargs)
 
     kf = (9 / 4 * np.pi)**(1 / 3) / rs
     ks = np.sqrt(4 * kf / np.pi)
     divt = 2 * ks * n
     t = norm_dn / divt
     expec = np.exp(-ec / gamma)
     A = beta / (gamma * (expec - 1))
     t2 = t**2
     At2 = A * t2
     A2t4 = At2**2
     divsum = 1 + At2 + A2t4
     div = (1 + At2) / divsum
     nolog = 1 + beta / gamma * t2 * div
     gec = gamma * np.log(nolog)
-    if exc_only:
-        return ec + gec, None, None
 
     factor = A2t4 * (2 + At2) / divsum**2
     dgec = beta * t2 / nolog * (-7 / 3 * div - factor * (A * expec * (vc - ec) / beta - 7 / 3))
     gvc = gec + dgec
 
     vsigmac = beta / (divt * ks) * (div - factor) / nolog
     return ec + gec, np.array([vc + gvc]), np.array([0.5 * vsigmac])
 
 
-def gga_c_pbe_spin(n, zeta, beta=0.06672455060314922, exc_only=False, dn_spin=None, **kwargs):
-    '''Perdew-Burke-Ernzerhof parametrization of the correlation functional (spin-polarized).
+def gga_c_pbe_spin(n, zeta, beta=0.06672455060314922, dn_spin=None, **kwargs):
+    """Perdew-Burke-Ernzerhof parametrization of the correlation functional (spin-polarized).
 
     Corresponds to the functional with the label GGA_C_PBE and ID 130 in Libxc.
+
     Reference: Phys. Rev. Lett. 78, 1396.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Keyword Args:
         beta (float): Functional parameter.
-        exc_only (bool): Only calculate the exchange-correlation energy density.
         dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray, ndarray]: PBE correlation energy density, potential, and vsigma.
-    '''
+    """
     gamma = (1 - np.log(2)) / np.pi**2
 
     pi34 = (3 / (4 * np.pi))**(1 / 3)
     rs = pi34 * n**(-1 / 3)
     norm_dn = norm(dn_spin[0] + dn_spin[1], axis=1)
-    ec, vc, _ = lda_c_pw_mod_spin(n, zeta, exc_only=exc_only, **kwargs)
-    if not exc_only:
-        vcup, vcdw = vc
+    ec, vc, _ = lda_c_pw_mod_spin(n, zeta, **kwargs)
+    vcup, vcdw = vc
 
     kf = (9 / 4 * np.pi)**(1 / 3) / rs
     ks = np.sqrt(4 * kf / np.pi)
     phi = ((1 + zeta)**(2 / 3) + (1 - zeta)**(2 / 3)) / 2
     phi2 = phi**2
     phi3 = phi2 * phi
     t = norm_dn / (2 * phi * ks * n)
@@ -95,16 +94,14 @@
     t2 = t**2
     At2 = A * t2
     A2t4 = At2**2
     divsum = 1 + At2 + A2t4
     div = (1 + At2) / divsum
     nolog = 1 + beta / gamma * t2 * div
     gec = gamma * phi3 * np.log(nolog)
-    if exc_only:
-        return ec + gec, None, None
 
     # Handle divisions by zero
     with np.errstate(divide='ignore', invalid='ignore'):
         dfz = ((1 + zeta)**(-1 / 3) - (1 - zeta)**(-1 / 3)) / 3
     dfz = np.nan_to_num(dfz, nan=0, posinf=0, neginf=0)
     factor = A2t4 * (2 + At2) / divsum**2
     bfpre = expec / phi3
```

### Comparing `eminus-2.4.0/eminus/xc/gga_c_pbe_sol.py` & `eminus-2.5.0/eminus/xc/gga_c_pbe_sol.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 #!/usr/bin/env python3
-'''Perdew-Burke-Ernzerhof GGA correlation for solids and surfaces.
+"""Perdew-Burke-Ernzerhof GGA correlation for solids and surfaces.
 
 Reference: Phys. Rev. Lett. 102, 039902.
-'''
+"""
 from .gga_c_pbe import gga_c_pbe, gga_c_pbe_spin
 
 
 def gga_c_pbe_sol(n, **kwargs):
-    '''Perdew-Burke-Ernzerhof solid parametrization of the correlation functional (spin-paired).
+    """Perdew-Burke-Ernzerhof solid parametrization of the correlation functional (spin-paired).
 
     Corresponds to the functional with the label GGA_C_PBE_SOL and ID 133 in Libxc.
+
     Reference: Phys. Rev. Lett. 102, 039902.
 
     Args:
         n (ndarray): Real-space electronic density.
 
+    Keyword Args:
+        **kwargs: Throwaway arguments.
+
     Returns:
         tuple[ndarray, ndarray, ndarray]: PBE correlation energy density, potential, and vsigma.
-    '''
+    """
     return gga_c_pbe(n, beta=0.046, **kwargs)
 
 
 def gga_c_pbe_sol_spin(n, zeta, **kwargs):
-    '''Perdew-Burke-Ernzerhof solid parametrization of the correlation functional (spin-polarized).
+    """Perdew-Burke-Ernzerhof solid parametrization of the correlation functional (spin-polarized).
 
     Corresponds to the functional with the label GGA_C_PBE_SOL and ID 133 in Libxc.
+
     Reference: Phys. Rev. Lett. 102, 039902.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
+    Keyword Args:
+        **kwargs: Throwaway arguments.
+
     Returns:
         tuple[ndarray, ndarray, ndarray]: PBE correlation energy density, potential, and vsigma.
-    '''
+    """
     return gga_c_pbe_spin(n, zeta, beta=0.046, **kwargs)
```

### Comparing `eminus-2.4.0/eminus/xc/gga_x_chachiyo.py` & `eminus-2.5.0/eminus/xc/gga_x_chachiyo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 #!/usr/bin/env python3
-'''Chachiyo GGA exchange.
+"""Chachiyo GGA exchange.
 
 Reference: Molecules 25, 3485.
-'''
+"""
 import numpy as np
 from numpy.linalg import norm
 
 from .lda_x import lda_x
 
 
-def gga_x_chachiyo(n, exc_only=False, dn_spin=None, **kwargs):
-    '''Chachiyo parametrization of the exchange functional (spin-paired).
+def gga_x_chachiyo(n, dn_spin=None, **kwargs):
+    """Chachiyo parametrization of the exchange functional (spin-paired).
 
     Corresponds to the functional with the label GGA_X_CHACHIYO and ID 298 in Libxc.
+
     Reference: Molecules 25, 3485.
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
         dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray, ndarray]: Chachiyo exchange energy density, potential, and vsigma.
-    '''
+    """
     norm_dn = norm(dn_spin[0], axis=1)
     ex, vx, _ = lda_x(n, **kwargs)
 
     x = norm_dn / n**(4 / 3) * 2 / 9 * (np.pi / 3)**(1 / 3)
     x1 = x + 1
     logx1 = np.log(x1)
     div = 3 * x + np.pi**2
     tmpgex = 3 * x**2 + np.pi**2 * logx1
     gex = tmpgex / (div * logx1)
-    if exc_only:
-        return ex * gex, None, None
 
     term1 = 8 * ex / tmpgex * (x**2 + x * np.pi**2 / (6 * x1)) + \
         2 / 3 * norm_dn / n * (1 / div + 1 / (3 * logx1 * x1))
     gvx = (1 + 1 / 3) * ex - term1
 
     vsigmax = n * 3 * term1 / (8 * norm_dn**2)
     return ex * gex, np.array([gvx]) * gex, np.array([vsigmax]) * gex
 
 
-def gga_x_chachiyo_spin(n, zeta, exc_only=False, dn_spin=None, **kwargs):
-    '''Chachiyo parametrization of the exchange functional (spin-polarized).
+def gga_x_chachiyo_spin(n, zeta, dn_spin=None, **kwargs):
+    """Chachiyo parametrization of the exchange functional (spin-polarized).
 
     Corresponds to the functional with the label GGA_X_CHACHIYO and ID 298 in Libxc.
+
     Reference: Molecules 25, 3485.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
         dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray, ndarray]: Chachiyo exchange energy density, potential, and vsigma.
-    '''
+    """
     # Use the spin-scaling relationship Exc(n_up, n_down)=(Exc(2 n_up)+Exc(2 n_down))/2
     n_up = zeta * n + n   # 2 * n_up
     n_dw = -zeta * n + n  # 2 * n_down
-    ex_up, vx_up, vsigma_up = gga_x_chachiyo(n_up, exc_only, np.array([2 * dn_spin[0]]), **kwargs)
-    ex_dw, vx_dw, vsigma_dw = gga_x_chachiyo(n_dw, exc_only, np.array([2 * dn_spin[1]]), **kwargs)
-    if exc_only:
-        return 0.5 * (ex_up * n_up + ex_dw * n_dw) / n, None, None
+    ex_up, vx_up, vsigma_up = gga_x_chachiyo(n_up, np.array([2 * dn_spin[0]]), **kwargs)
+    ex_dw, vx_dw, vsigma_dw = gga_x_chachiyo(n_dw, np.array([2 * dn_spin[1]]), **kwargs)
 
     vsigmax = np.array([2 * vsigma_up, np.zeros_like(vsigma_up), 2 * vsigma_dw])
     return 0.5 * (ex_up * n_up + ex_dw * n_dw) / n, np.array([vx_up, vx_dw]), vsigmax
```

### Comparing `eminus-2.4.0/eminus/xc/gga_x_pbe_sol.py` & `eminus-2.5.0/eminus/xc/gga_x_pbe_sol.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 #!/usr/bin/env python3
-'''Perdew-Burke-Ernzerhof GGA exchange for solids and surfaces.
+"""Perdew-Burke-Ernzerhof GGA exchange for solids and surfaces.
 
 Reference: Phys. Rev. Lett. 102, 039902.
-'''
+"""
 from .gga_x_pbe import gga_x_pbe, gga_x_pbe_spin
 
 
 def gga_x_pbe_sol(n, **kwargs):
-    '''Perdew-Burke-Ernzerhof solid parametrization of the exchange functional (spin-paired).
+    """Perdew-Burke-Ernzerhof solid parametrization of the exchange functional (spin-paired).
 
     Corresponds to the functional with the label GGA_X_PBE_SOL and ID 116 in Libxc.
+
     Reference: Phys. Rev. Lett. 102, 039902.
 
     Args:
         n (ndarray): Real-space electronic density.
 
+    Keyword Args:
+        **kwargs: Throwaway arguments.
+
     Returns:
         tuple[ndarray, ndarray, ndarray]: PBE exchange energy density, potential, and vsigma.
-    '''
+    """
     return gga_x_pbe(n, mu=10 / 81, **kwargs)
 
 
 def gga_x_pbe_sol_spin(n, zeta, **kwargs):
-    '''Perdew-Burke-Ernzerhof solid parametrization of the exchange functional (spin-polarized).
+    """Perdew-Burke-Ernzerhof solid parametrization of the exchange functional (spin-polarized).
 
     Corresponds to the functional with the label GGA_X_PBE_SOL and ID 116 in Libxc.
+
     Reference: Phys. Rev. Lett. 102, 039902.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
+    Keyword Args:
+        **kwargs: Throwaway arguments.
+
     Returns:
         tuple[ndarray, ndarray, ndarray]: PBE exchange energy density, potential, and vsigma.
-    '''
+    """
     return gga_x_pbe_spin(n, zeta, mu=10 / 81, **kwargs)
```

### Comparing `eminus-2.4.0/eminus/xc/lda_c_chachiyo.py` & `eminus-2.5.0/eminus/xc/lda_c_chachiyo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,102 +1,95 @@
 #!/usr/bin/env python3
-'''Chachiyo LDA correlation.
+"""Chachiyo LDA correlation.
 
 Reference: J. Chem. Phys. 145, 021101.
-'''
+"""
 import numpy as np
 
 
-def lda_c_chachiyo(n, exc_only=False, **kwargs):
-    '''Chachiyo parametrization of the correlation functional (spin-paired).
+def lda_c_chachiyo(n, **kwargs):
+    """Chachiyo parametrization of the correlation functional (spin-paired).
 
     Corresponds to the functional with the label LDA_C_CHACHIYO and ID 287 in Libxc.
+
     Reference: J. Chem. Phys. 145, 021101.
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray]: Chachiyo correlation energy density and potential.
-    '''
+    """
     a = -0.01554535  # (np.log(2) - 1) / (2 * np.pi**2)
     b = 20.4562557
 
     rs = (3 / (4 * np.pi * n))**(1 / 3)
     rs2 = rs**2
     ecinner = 1 + b / rs + b / rs2
 
     ec = a * np.log(ecinner)
-    if exc_only:
-        return ec, None, None
 
     vc = ec + a * b * (2 + rs) / (3 * (b + b * rs + rs2))
     return ec, np.array([vc]), None
 
 
-def chachiyo_scaling(zeta, exc_only=False):
-    '''Weighting factor between the paramagnetic and the ferromagnetic case.
+def chachiyo_scaling(zeta):
+    """Weighting factor between the paramagnetic and the ferromagnetic case.
 
     Reference: J. Chem. Phys. 145, 021101.
 
     Args:
         zeta (ndarray): Relative spin polarization.
 
-    Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
-
     Returns:
         tuple[ndarray, ndarray]: Weighting factor and its derivative.
-    '''
+    """
     fzeta = ((1 + zeta)**(4 / 3) + (1 - zeta)**(4 / 3) - 2) / (2 * (2**(1 / 3) - 1))
-    if exc_only:
-        return fzeta, None
 
     dfdzeta = (2 * (1 - zeta)**(1 / 3) - 2 * (1 + zeta)**(1 / 3)) / (3 - 3 * 2**(1 / 3))
     return fzeta, dfdzeta
 
 
-def lda_c_chachiyo_spin(n, zeta, weight_function=chachiyo_scaling, exc_only=False, **kwargs):
-    '''Chachiyo parametrization of the correlation functional (spin-polarized).
+def lda_c_chachiyo_spin(n, zeta, weight_function=chachiyo_scaling, **kwargs):
+    """Chachiyo parametrization of the correlation functional (spin-polarized).
 
     Corresponds to the functional with the label LDA_C_CHACHIYO and ID 287 in Libxc.
+
     Reference: J. Chem. Phys. 145, 021101.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Keyword Args:
         weight_function (Callable): Functional function.
-        exc_only (bool): Only calculate the exchange-correlation energy density.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray]: Chachiyo correlation energy density and potential.
-    '''
+    """
     a0 = -0.01554535   # (np.log(2) - 1) / (2 * np.pi**2)
     a1 = -0.007772675  # (np.log(2) - 1) / (4 * np.pi**2)
     b0 = 20.4562557
     b1 = 27.4203609
 
     rs = (3 / (4 * np.pi * n))**(1 / 3)
     rs2 = rs**2
 
-    fzeta, dfdzeta = weight_function(zeta, exc_only=exc_only)
+    fzeta, dfdzeta = weight_function(zeta)
 
     ec0inner = 1 + b0 / rs + b0 / rs2
     ec1inner = 1 + b1 / rs + b1 / rs2
     ec0 = a0 * np.log(ec0inner)
     ec1 = a1 * np.log(ec1inner)
 
     ec = ec0 + (ec1 - ec0) * fzeta
-    if exc_only:
-        return ec, None, None
 
     factor = -1 / rs2 - 2 / rs**3
     dec0drs = a0 / ec0inner * b0 * factor
     dec1drs = a1 / ec1inner * b1 * factor
     decdrs = dec0drs + (dec1drs - dec0drs) * fzeta
     prefactor = ec - rs / 3 * decdrs
     decdf = (ec1 - ec0) * dfdzeta
```

### Comparing `eminus-2.4.0/eminus/xc/lda_c_chachiyo_mod.py` & `eminus-2.5.0/eminus/xc/lda_c_chachiyo_mod.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 #!/usr/bin/env python3
-'''Modified Chachiyo LDA correlation.
+"""Modified Chachiyo LDA correlation.
 
 Reference: Comput. Theor. Chem. 1172, 112669.
-'''
+"""
 from .lda_c_chachiyo import lda_c_chachiyo, lda_c_chachiyo_spin
 
 
 def lda_c_chachiyo_mod(n, **kwargs):
-    '''Modified Chachiyo parametrization of the correlation functional (spin-paired).
+    """Modified Chachiyo parametrization of the correlation functional (spin-paired).
 
     Corresponds to the functional with the label LDA_C_CHACHIYO_MOD and ID 307 in Libxc.
+
     Reference: Comput. Theor. Chem. 1172, 112669.
 
     Args:
         n (ndarray): Real-space electronic density.
 
+    Keyword Args:
+        **kwargs: Throwaway arguments.
+
     Returns:
         tuple[ndarray, ndarray]: Chachiyo correlation energy density and potential.
-    '''
+    """
     # Same as lda_c_chachiyo
     return lda_c_chachiyo(n, **kwargs)
 
 
-def chachiyo_scaling_mod(zeta, exc_only=False):
-    '''Modified weighting factor between the paramagnetic and the ferromagnetic case.
+def chachiyo_scaling_mod(zeta):
+    """Modified weighting factor between the paramagnetic and the ferromagnetic case.
 
     Reference: Comput. Theor. Chem. 1172, 112669.
 
     Args:
         zeta (ndarray): Relative spin polarization.
 
-    Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
-
     Returns:
         tuple[ndarray, ndarray]: Weighting factor and its derivative.
-    '''
+    """
     gzeta = ((1 + zeta)**(2 / 3) + (1 - zeta)**(2 / 3)) / 2
     fzeta = 2 * (1 - gzeta**3)
-    if exc_only:
-        return fzeta, None
 
     dfdzeta = -2 * gzeta**2 * (1 / (1 + zeta)**(1 / 3) - 1 / (1 - zeta)**(1 / 3))
     return fzeta, dfdzeta
 
 
 def lda_c_chachiyo_mod_spin(n, zeta, **kwargs):
-    '''Modified Chachiyo parametrization of the correlation functional (spin-polarized).
+    """Modified Chachiyo parametrization of the correlation functional (spin-polarized).
 
     Corresponds to the functional with the label LDA_C_CHACHIYO_MOD and ID 307 in Libxc.
+
     Reference: Comput. Theor. Chem. 1172, 112669.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
+    Keyword Args:
+        **kwargs: Throwaway arguments.
+
     Returns:
         tuple[ndarray, ndarray]: Chachiyo correlation energy density and potential.
-    '''
+    """
     return lda_c_chachiyo_spin(n, zeta, weight_function=chachiyo_scaling_mod, **kwargs)
```

### Comparing `eminus-2.4.0/eminus/xc/lda_c_pw.py` & `eminus-2.5.0/eminus/xc/lda_c_pw.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,86 @@
 #!/usr/bin/env python3
-'''Perdew-Wang LDA correlation.
+"""Perdew-Wang LDA correlation.
 
 Reference: Phys. Rev. B 45, 13244.
-'''
+"""
 import numpy as np
 
 
-def lda_c_pw(n, A=0.031091, a1=0.2137, b1=7.5957, b2=3.5876, b3=1.6382, b4=0.49294, exc_only=False,
-             **kwargs):
-    '''Perdew-Wang parametrization of the correlation functional (spin-paired).
+def lda_c_pw(n, A=0.031091, a1=0.2137, b1=7.5957, b2=3.5876, b3=1.6382, b4=0.49294, **kwargs):
+    """Perdew-Wang parametrization of the correlation functional (spin-paired).
 
     Corresponds to the functional with the label LDA_C_PW and ID 12 in Libxc.
+
     Reference: Phys. Rev. B 45, 13244.
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
         A (float): Functional parameter.
         a1 (float): Functional parameter.
         b1 (float): Functional parameter.
         b2 (float): Functional parameter.
         b3 (float): Functional parameter.
         b4 (float): Functional parameter.
-        exc_only (bool): Only calculate the exchange-correlation energy density.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray]: PW correlation energy density and potential.
-    '''
+    """
     rs = (3 / (4 * np.pi * n))**(1 / 3)
     rs12 = np.sqrt(rs)
     rs32 = rs * rs12
     rs2 = rs**2
 
     om = 2 * A * (b1 * rs12 + b2 * rs + b3 * rs32 + b4 * rs2)
     olog = np.log(1 + 1 / om)
     ec = -2 * A * (1 + a1 * rs) * olog
-    if exc_only:
-        return ec, None, None
 
     dom = 2 * A * (0.5 * b1 * rs12 + b2 * rs + 1.5 * b3 * rs32 + 2 * b4 * rs2)
     vc = -2 * A * (1 + 2 / 3 * a1 * rs) * olog - 2 / 3 * A * (1 + a1 * rs) * dom / (om * (om + 1))
     return ec, np.array([vc]), None
 
 
-def lda_c_pw_spin(n, zeta, A=(0.031091, 0.015545, 0.016887), fzeta0=1.709921, exc_only=False,
-                  **kwargs):
-    '''Perdew-Wang parametrization of the correlation functional (spin-polarized).
+def lda_c_pw_spin(n, zeta, A=(0.031091, 0.015545, 0.016887), fzeta0=1.709921, **kwargs):
+    """Perdew-Wang parametrization of the correlation functional (spin-polarized).
 
     Corresponds to the functional with the label LDA_C_PW and ID 12 in Libxc.
+
     Reference: Phys. Rev. B 45, 13244.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Keyword Args:
         A (tuple): Functional parameters.
         fzeta0 (float): Functional parameter.
-        exc_only (bool): Only calculate the exchange-correlation energy density.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray]: PW correlation energy density and potential.
-    '''
+    """
     a1 = (0.2137, 0.20548, 0.11125)
     b1 = (7.5957, 14.1189, 10.357)
     b2 = (3.5876, 6.1977, 3.6231)
     b3 = (1.6382, 3.3662, 0.88026)
     b4 = (0.49294, 0.62517, 0.49671)
 
-    ec0, vc0, _ = lda_c_pw(n, A[0], a1[0], b1[0], b2[0], b3[0], b4[0], exc_only)  # Unpolarized
-    ec1, vc1, _ = lda_c_pw(n, A[1], a1[1], b1[1], b2[1], b3[1], b4[1], exc_only)  # Polarized
-    ac, dac, _ = lda_c_pw(n, A[2], a1[2], b1[2], b2[2], b3[2], b4[2], exc_only)   # Spin stiffness
+    ec0, vc0, _ = lda_c_pw(n, A[0], a1[0], b1[0], b2[0], b3[0], b4[0])  # Unpolarized
+    ec1, vc1, _ = lda_c_pw(n, A[1], a1[1], b1[1], b2[1], b3[1], b4[1])  # Polarized
+    ac, dac, _ = lda_c_pw(n, A[2], a1[2], b1[2], b2[2], b3[2], b4[2])   # Spin stiffness
     ac = -ac  # The PW spin interpolation parametrizes -ac instead of ac
 
     fzeta = ((1 + zeta)**(4 / 3) + (1 - zeta)**(4 / 3) - 2) / (2**(4 / 3) - 2)
     zeta3 = zeta**3
     zeta4 = zeta3 * zeta
 
     ec = ec0 + ac * fzeta * (1 - zeta4) / fzeta0 + (ec1 - ec0) * fzeta * zeta4
-    if exc_only:
-        return ec, None, None
 
     dac = -dac  # Also change the sign for the derivative
     dfzeta = ((1 + zeta)**(1 / 3) - (1 - zeta)**(1 / 3)) * 4 / (3 * (2**(4 / 3) - 2))
     factor1 = vc0 + dac * fzeta * (1 - zeta4) / fzeta0 + (vc1 - vc0) * fzeta * zeta4
     factor2 = (ac / fzeta0 * (dfzeta * (1 - zeta4) - 4 * fzeta * zeta3) +
                (ec1 - ec0) * (dfzeta * zeta4 + 4 * fzeta * zeta3))
```

### Comparing `eminus-2.4.0/eminus/xc/lda_c_pw_mod.py` & `eminus-2.5.0/eminus/xc/lda_c_pw_mod.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 #!/usr/bin/env python3
-'''Modified Perdew-Wang LDA correlation.
+"""Modified Perdew-Wang LDA correlation.
 
 Reference: Phys. Rev. B 45, 13244.
-'''
+"""
 from .lda_c_pw import lda_c_pw, lda_c_pw_spin
 
 
 def lda_c_pw_mod(n, **kwargs):
-    '''Modified Perdew-Wang parametrization of the correlation functional (spin-paired).
+    """Modified Perdew-Wang parametrization of the correlation functional (spin-paired).
 
     Corresponds to the functional with the label LDA_C_PW_MOD and ID 13 in Libxc.
+
     Reference: Phys. Rev. B 45, 13244.
 
     Args:
         n (ndarray): Real-space electronic density.
 
+    Keyword Args:
+        **kwargs: Throwaway arguments.
+
     Returns:
         tuple[ndarray, ndarray]: PW correlation energy density and potential.
-    '''
+    """
     return lda_c_pw(n, A=0.0310907, **kwargs)
 
 
 def lda_c_pw_mod_spin(n, zeta, **kwargs):
-    '''Modified Perdew-Wang parametrization of the correlation functional (spin-polarized).
+    """Modified Perdew-Wang parametrization of the correlation functional (spin-polarized).
 
     Corresponds to the functional with the label LDA_C_PW_MOD and ID 13 in Libxc.
+
     Reference: Phys. Rev. B 45, 13244.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
+    Keyword Args:
+        **kwargs: Throwaway arguments.
+
     Returns:
         tuple[ndarray, ndarray]: PW correlation energy density and potential.
-    '''
+    """
     return lda_c_pw_spin(n, zeta, A=(0.0310907, 0.01554535, 0.0168869),
                          fzeta0=1.709920934161365617563962776245, **kwargs)
```

### Comparing `eminus-2.4.0/eminus/xc/lda_c_vwn.py` & `eminus-2.5.0/eminus/xc/lda_c_vwn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,86 @@
 #!/usr/bin/env python3
-'''Vosko-Wilk-Nusair LDA correlation.
+"""Vosko-Wilk-Nusair LDA correlation.
 
 Reference: Phys. Rev. B 22, 3812.
-'''
+"""
 import numpy as np
 
 
-def lda_c_vwn(n, A=0.0310907, b=3.72744, c=12.9352, x0=-0.10498, exc_only=False, **kwargs):
-    '''Vosko-Wilk-Nusair parametrization of the correlation functional (spin-paired).
+def lda_c_vwn(n, A=0.0310907, b=3.72744, c=12.9352, x0=-0.10498, **kwargs):
+    """Vosko-Wilk-Nusair parametrization of the correlation functional (spin-paired).
 
     Corresponds to the functional with the label LDA_C_VWN and ID 7 in Libxc.
+
     Reference: Phys. Rev. B 22, 3812.
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
         A (float): Functional parameter.
         b (float): Functional parameter.
         c (float): Functional parameter.
         x0 (float): Functional parameter.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray]: VWN correlation energy density and potential.
-    '''
+    """
     rs = (3 / (4 * np.pi * n))**(1 / 3)
 
     x = np.sqrt(rs)
     X = rs + b * x + c
     Q = np.sqrt(4 * c - b**2)
     fx0 = b * x0 / (x0**2 + b * x0 + c)
     f3 = 2 * (2 * x0 + b) / Q
     tx = 2 * x + b
     tanx = np.arctan(Q / tx)
 
     ec = A * (np.log(rs / X) + 2 * b / Q * tanx - fx0 * (np.log((x - x0)**2 / X) + f3 * tanx))
-    if exc_only:
-        return ec, None, None
 
     tt = tx**2 + Q**2
     vc = ec - x * A / 6 * (2 / x - tx / X - 4 * b / tt -
                            fx0 * (2 / (x - x0) - tx / X - 4 * (2 * x0 + b) / tt))
     return ec, np.array([vc]), None
 
 
-def lda_c_vwn_spin(n, zeta, exc_only=False, **kwargs):
-    '''Vosko-Wilk-Nusair parametrization of the correlation functional (spin-polarized).
+def lda_c_vwn_spin(n, zeta, **kwargs):
+    """Vosko-Wilk-Nusair parametrization of the correlation functional (spin-polarized).
 
     Corresponds to the functional with the label LDA_C_VWN and ID 7 in Libxc.
+
     Reference: Phys. Rev. B 22, 3812.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray]: VWN correlation energy density and potential.
-    '''
+    """
     A = (0.0310907, 0.01554535, -1 / (6 * np.pi**2))
     b = (3.72744, 7.06042, 1.13107)
     c = (12.9352, 18.0578, 13.0045)
     x0 = (-0.10498, -0.325, -0.0047584)
 
-    ec0, vc0, _ = lda_c_vwn(n, A[0], b[0], c[0], x0[0], exc_only)  # Paramagnetic
-    ec1, vc1, _ = lda_c_vwn(n, A[1], b[1], c[1], x0[1], exc_only)  # Ferromagnetic
-    ac, dac, _ = lda_c_vwn(n, A[2], b[2], c[2], x0[2], exc_only)   # Spin stiffness
+    ec0, vc0, _ = lda_c_vwn(n, A[0], b[0], c[0], x0[0])  # Paramagnetic
+    ec1, vc1, _ = lda_c_vwn(n, A[1], b[1], c[1], x0[1])  # Ferromagnetic
+    ac, dac, _ = lda_c_vwn(n, A[2], b[2], c[2], x0[2])   # Spin stiffness
 
     d2fzeta0 = 4 / 9 / (2**(1 / 3) - 1)
     fzeta = 0.5 * ((1 + zeta)**(4 / 3) + (1 - zeta)**(4 / 3) - 2) / (2**(1 / 3) - 1)
     zeta4 = zeta**4
     fzetaz4 = fzeta * zeta4
     De = ec1 - ec0 - ac / d2fzeta0
 
     ec = ec0 + ac / d2fzeta0 * fzeta + De * fzetaz4
-    if exc_only:
-        return ec, None, None
 
     dfzeta = 4 / 6 * ((1 + zeta)**(1 / 3) - (1 - zeta)**(1 / 3)) / (2**(1 / 3) - 1)
     dec1 = vc0 + dac / d2fzeta0 * fzeta + (vc1 - vc0 - dac / d2fzeta0) * fzetaz4
     dec2 = ac / d2fzeta0 * dfzeta + De * (4 * zeta**3 * fzeta + zeta4 * dfzeta)
 
     vcup = dec1 + (1 - zeta) * dec2
     vcdw = dec1 - (1 + zeta) * dec2
```

### Comparing `eminus-2.4.0/eminus/xc/lda_x.py` & `eminus-2.5.0/eminus/xc/lda_x.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 #!/usr/bin/env python3
-'''Slater LDA exchange.
+"""Slater LDA exchange.
 
 Reference: Phys. Rev. 81, 385.
-'''
+"""
 import numpy as np
 
 
-def lda_x(n, exc_only=False, **kwargs):
-    '''Slater exchange functional (spin-paired).
+def lda_x(n, **kwargs):
+    """Slater exchange functional (spin-paired).
 
     Corresponds to the functional with the label LDA_X and ID 1 in Libxc.
+
     Reference: Phys. Rev. 81, 385.
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray]: Exchange energy density and potential.
-    '''
+    """
     f = -3 / 4 * (3 / (2 * np.pi))**(2 / 3)
     rs = (3 / (4 * np.pi * n))**(1 / 3)
 
     ex = f / rs
-    if exc_only:
-        return ex, None, None
 
     vx = 4 / 3 * ex
     return ex, np.array([vx]), None
 
 
-def lda_x_spin(n, zeta, exc_only=False, **kwargs):
-    '''Slater exchange functional (spin-polarized).
+def lda_x_spin(n, zeta, **kwargs):
+    """Slater exchange functional (spin-polarized).
 
     Corresponds to the functional with the label LDA_X and ID 1 in Libxc.
+
     Reference: Phys. Rev. 81, 385.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Keyword Args:
-        exc_only (bool): Only calculate the exchange-correlation energy density.
+        **kwargs: Throwaway arguments.
 
     Returns:
         tuple[ndarray, ndarray]: Exchange energy density and potential.
-    '''
+    """
     f = -3 / 4 * (3 / np.pi)**(1 / 3)
 
     rho13p = ((1 + zeta) * n)**(1 / 3)
     rho13m = ((1 - zeta) * n)**(1 / 3)
 
     exup = f * rho13p
     exdw = f * rho13m
     ex = 0.5 * ((1 + zeta) * exup + (1 - zeta) * exdw)
-    if exc_only:
-        return ex, None, None
 
     vxup = 4 / 3 * exup
     vxdw = 4 / 3 * exdw
     return ex, np.array([vxup, vxdw]), None
```

### Comparing `eminus-2.4.0/eminus.egg-info/SOURCES.txt` & `eminus-2.5.0/eminus.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 eminus/__init__.py
 eminus/atoms.py
 eminus/config.py
 eminus/data.py
 eminus/dft.py
 eminus/domains.py
 eminus/energies.py
+eminus/gga.py
 eminus/gth.py
 eminus/localizer.py
 eminus/logger.py
 eminus/minimizer.py
 eminus/operators.py
 eminus/orbitals.py
 eminus/potentials.py
@@ -23,15 +24,14 @@
 eminus/tools.py
 eminus/units.py
 eminus/utils.py
 eminus/version.py
 eminus.egg-info/PKG-INFO
 eminus.egg-info/SOURCES.txt
 eminus.egg-info/dependency_links.txt
-eminus.egg-info/not-zip-safe
 eminus.egg-info/requires.txt
 eminus.egg-info/top_level.txt
 eminus/extras/README.md
 eminus/extras/__init__.py
 eminus/extras/fods.py
 eminus/extras/libxc.py
 eminus/extras/torch.py
```

### Comparing `eminus-2.4.0/setup.py` & `eminus-2.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
-'''Setup file to make eminus installable.
+"""Setup file to make eminus installable.
 
 For a full list of options see the documentation:
 https://setuptools.pypa.io/en/latest/references/keywords.html
-'''
+"""
 import re
 
 from setuptools import find_packages, setup
 
 with open('eminus/version.py', 'r') as fh:
     version = re.search(r"__version__ = '(.*?)'", fh.read()).group(1)
 
@@ -25,23 +25,21 @@
         'nglview>=2.6.5',  # Molecule and isosurface viewer
         'plotly>=4.5'      # Grid visualization
     ]
 }
 extras['fods'] = extras['libxc']  # PyCOM FOD guessing method uses PySCF
 extras['all'] = [dep for values in extras.values() for dep in values]
 extras['dev'] = [
-    'coverage>=4.4',             # Generate coverage reports
-    'flake8>=3.7',               # Style guide checker
-    'flake8-docstrings>=1.4',    # Docstring style guide extension
-    'flake8-import-order>=0.9',  # Import statement style guide extension
-    'furo>=2022.02.14.1',        # Documentation theme
-    'notebook',                  # Run and convert notebooks to HTML
-    'pytest>=5.4',               # Test utilities
-    'pytest-cov>=2.6.1',         # Collect test coverage data
-    'sphinx>=4'                  # Documentation builder
+    'coverage>=4.4',       # Generate coverage reports
+    'furo>=2022.02.14.1',  # Documentation theme
+    'notebook',            # Run and convert notebooks to HTML
+    'pytest>=5.4',         # Test utilities
+    'pytest-cov>=2.6.1',   # Collect test coverage data
+    'ruff>=0.0.276',       # Style guide checker
+    'sphinx>=4'            # Documentation builder
 ]
 
 setup(
     name='eminus',
     version=version,
     description='A plane wave density functional theory code.',
     long_description=long_description,
@@ -72,19 +70,19 @@
         'Topic :: Education',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Physics',
         'Topic :: Software Development'
     ],
     license='APACHE2.0',
+    include_package_data=True,
     install_requires=[
         'numpy>=1.17',
         'scipy>=1.6'
     ],
-    zip_safe=False,
     extras_require=extras,
     python_requires='>=3.7',
     project_urls={
         'Bug Tracker': 'https://gitlab.com/wangenau/eminus/-/issues',
         'Changelog': 'https://wangenau.gitlab.io/eminus/changelog.html',
         'Documentation': 'https://wangenau.gitlab.io/eminus',
         'Source code': 'https://gitlab.com/wangenau/eminus'
```

