# Comparing `tmp/eminus-2.3.0.tar.gz` & `tmp/eminus-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eminus-2.3.0.tar", last modified: Tue May  2 11:49:15 2023, max compression
+gzip compressed data, was "eminus-2.4.0.tar", last modified: Tue May 23 10:05:07 2023, max compression
```

## Comparing `eminus-2.3.0.tar` & `eminus-2.4.0.tar`

### file list

```diff
@@ -1,226 +1,373 @@
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.304677 eminus-2.3.0/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5289 2023-05-02 11:35:04.000000 eminus-2.3.0/CHANGELOG.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10173 2022-05-25 09:24:55.000000 eminus-2.3.0/LICENSE
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       59 2023-02-21 16:32:19.000000 eminus-2.3.0/MANIFEST.in
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3860 2023-05-02 11:49:15.304677 eminus-2.3.0/PKG-INFO
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1518 2023-04-19 09:05:34.000000 eminus-2.3.0/README.md
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.288677 eminus-2.3.0/eminus/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      980 2023-04-24 14:35:56.000000 eminus-2.3.0/eminus/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      778 2023-04-11 09:05:31.000000 eminus-2.3.0/eminus/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    15390 2023-04-21 15:03:17.000000 eminus-2.3.0/eminus/atoms.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4831 2023-04-21 14:57:11.000000 eminus-2.3.0/eminus/config.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6977 2022-12-18 16:38:36.000000 eminus-2.3.0/eminus/data.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     9949 2023-04-01 11:09:08.000000 eminus-2.3.0/eminus/dft.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3254 2023-04-18 09:14:40.000000 eminus-2.3.0/eminus/domains.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     9822 2023-04-03 13:03:22.000000 eminus-2.3.0/eminus/energies.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.288677 eminus-2.3.0/eminus/extras/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      324 2023-04-03 13:17:42.000000 eminus-2.3.0/eminus/extras/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-21 13:14:30.000000 eminus-2.3.0/eminus/extras/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6601 2023-04-27 09:30:47.000000 eminus-2.3.0/eminus/extras/fods.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2683 2023-04-17 18:01:40.000000 eminus-2.3.0/eminus/extras/libxc.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6343 2023-04-21 14:18:24.000000 eminus-2.3.0/eminus/extras/torch.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8499 2023-04-27 10:07:02.000000 eminus-2.3.0/eminus/extras/viewer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6353 2023-03-03 14:20:37.000000 eminus-2.3.0/eminus/gth.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.292677 eminus-2.3.0/eminus/io/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      260 2023-01-22 12:58:23.000000 eminus-2.3.0/eminus/io/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1240 2023-01-22 12:56:38.000000 eminus-2.3.0/eminus/io/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5761 2023-04-27 09:59:52.000000 eminus-2.3.0/eminus/io/cube.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3597 2023-05-02 11:28:01.000000 eminus-2.3.0/eminus/io/gth.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3442 2023-05-02 11:25:06.000000 eminus-2.3.0/eminus/io/json.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4052 2023-04-27 09:58:44.000000 eminus-2.3.0/eminus/io/pdb.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3240 2023-04-24 14:59:39.000000 eminus-2.3.0/eminus/io/xyz.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10633 2023-04-27 09:27:42.000000 eminus-2.3.0/eminus/localizer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2700 2023-04-20 11:20:05.000000 eminus-2.3.0/eminus/logger.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    13657 2023-04-01 10:00:08.000000 eminus-2.3.0/eminus/minimizer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8614 2023-04-20 15:29:13.000000 eminus-2.3.0/eminus/operators.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4007 2023-04-27 09:27:59.000000 eminus-2.3.0/eminus/orbitals.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.304677 eminus-2.3.0/eminus/pade/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ac-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ac-q29
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ag-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ag-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ag-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Al-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Am-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Am-q35
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ar-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/As-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/At-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Au-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Au-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Au-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/B-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      372 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ba-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ba-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Be-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Be-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Bi-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Bk-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Bk-q37
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Br-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/C-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ca-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ca-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cd-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cd-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ce-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cf-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cf-q38
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cl-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cm-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cm-q36
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Co-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Co-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cr-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cr-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cs-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      370 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cs-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cu-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cu-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Cu-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Dy-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Er-q22
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Es-q21
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Es-q39
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Eu-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/F-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Fe-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Fe-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Fm-q22
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Fm-q40
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ga-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ga-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Gd-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ge-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       88 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/H-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       89 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/He-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Hf-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Hg-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Hg-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ho-q21
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      414 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/I-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/In-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/In-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ir-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ir-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/K-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      297 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/K-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Kr-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      473 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/La-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Li-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Li-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Lr-q25
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Lr-q43
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Lu-q25
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Md-q23
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Md-q41
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      168 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mg-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mg-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mn-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mn-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mo-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Mo-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/N-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Na-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      166 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Na-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Nb-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Nb-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Nd-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      232 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ne-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ni-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ni-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/No-q24
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/No-q42
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Np-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Np-q33
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/O-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Os-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Os-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/P-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pa-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pa-q31
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pb-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pd-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pd-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pm-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Po-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pr-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pt-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pt-q18
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pu-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Pu-q34
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      316 2022-07-28 10:43:21.000000 eminus-2.3.0/eminus/pade/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rb-q1
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      334 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rb-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Re-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Re-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rh-q17
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rh-q9
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Rn-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ru-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ru-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/S-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sb-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sc-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sc-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Se-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Si-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sm-q16
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sn-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sr-q10
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Sr-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ta-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ta-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tb-q19
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tc-q15
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tc-q7
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Te-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Th-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Th-q30
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ti-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Ti-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tl-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tl-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Tm-q23
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/U-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/U-q32
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      340 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/V-q13
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      404 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/V-q5
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      502 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/W-q14
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      389 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/W-q6
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Xe-q8
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      406 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Y-q11
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Y-q3
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Yb-q24
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zn-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zn-q2
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zn-q20
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zr-q12
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      486 2023-04-20 10:00:01.000000 eminus-2.3.0/eminus/pade/Zr-q4
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      837 2023-04-20 10:02:31.000000 eminus-2.3.0/eminus/pade/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2629 2023-04-28 12:30:26.000000 eminus-2.3.0/eminus/potentials.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    11803 2023-04-21 09:21:14.000000 eminus-2.3.0/eminus/scf.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8232 2023-04-21 13:09:12.000000 eminus-2.3.0/eminus/tools.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3048 2022-11-01 10:58:37.000000 eminus-2.3.0/eminus/units.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5521 2023-04-21 10:24:50.000000 eminus-2.3.0/eminus/utils.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1473 2023-05-02 11:35:17.000000 eminus-2.3.0/eminus/version.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.304677 eminus-2.3.0/eminus/xc/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      494 2023-01-21 12:28:14.000000 eminus-2.3.0/eminus/xc/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      314 2023-01-25 09:06:37.000000 eminus-2.3.0/eminus/xc/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3169 2023-04-03 08:37:42.000000 eminus-2.3.0/eminus/xc/lda_c_chachiyo.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1923 2023-01-26 09:19:06.000000 eminus-2.3.0/eminus/xc/lda_c_chachiyo_mod.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4004 2023-04-01 11:25:27.000000 eminus-2.3.0/eminus/xc/lda_c_pw.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1221 2023-01-26 09:19:47.000000 eminus-2.3.0/eminus/xc/lda_c_pw_mod.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4269 2023-04-01 11:25:37.000000 eminus-2.3.0/eminus/xc/lda_c_vwn.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1660 2023-04-01 11:24:46.000000 eminus-2.3.0/eminus/xc/lda_x.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6165 2023-05-02 11:24:10.000000 eminus-2.3.0/eminus/xc/utils.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-02 11:49:15.288677 eminus-2.3.0/eminus.egg-info/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3860 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/PKG-INFO
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4085 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/SOURCES.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/dependency_links.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2022-09-27 12:14:58.000000 eminus-2.3.0/eminus.egg-info/not-zip-safe
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      324 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/requires.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        7 2023-05-02 11:49:15.000000 eminus-2.3.0/eminus.egg-info/top_level.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       86 2023-01-27 17:55:16.000000 eminus-2.3.0/pyproject.toml
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       38 2023-05-02 11:49:15.304677 eminus-2.3.0/setup.cfg
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3436 2023-04-21 12:36:38.000000 eminus-2.3.0/setup.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.042773 eminus-2.4.0/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5775 2023-05-23 09:48:52.000000 eminus-2.4.0/CHANGELOG.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10173 2022-05-25 09:24:55.000000 eminus-2.4.0/LICENSE
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       61 2023-05-17 14:03:34.000000 eminus-2.4.0/MANIFEST.in
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3820 2023-05-23 10:05:07.042773 eminus-2.4.0/PKG-INFO
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1518 2023-05-05 09:27:44.000000 eminus-2.4.0/README.md
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      980 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      778 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    15551 2023-05-22 16:23:17.000000 eminus-2.4.0/eminus/atoms.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4831 2023-05-22 14:40:40.000000 eminus-2.4.0/eminus/config.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6977 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/data.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    12188 2023-05-22 16:46:01.000000 eminus-2.4.0/eminus/dft.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3254 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/domains.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10042 2023-05-22 11:47:34.000000 eminus-2.4.0/eminus/energies.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus/extras/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      324 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/extras/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/extras/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6549 2023-05-20 10:20:21.000000 eminus-2.4.0/eminus/extras/fods.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4519 2023-05-19 14:49:21.000000 eminus-2.4.0/eminus/extras/libxc.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6361 2023-05-22 14:35:23.000000 eminus-2.4.0/eminus/extras/torch.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8502 2023-05-20 15:15:32.000000 eminus-2.4.0/eminus/extras/viewer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     6353 2023-05-05 09:27:14.000000 eminus-2.4.0/eminus/gth.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus/io/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      260 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/io/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1240 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/io/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5785 2023-05-17 14:01:39.000000 eminus-2.4.0/eminus/io/cube.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3688 2023-05-17 16:25:40.000000 eminus-2.4.0/eminus/io/gth.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3442 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/io/json.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4052 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/io/pdb.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3264 2023-05-17 14:01:39.000000 eminus-2.4.0/eminus/io/xyz.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10633 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/localizer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2700 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/logger.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    13656 2023-05-22 11:47:48.000000 eminus-2.4.0/eminus/minimizer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     8614 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/operators.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4007 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/orbitals.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2629 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/potentials.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus/psp/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       56 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/__init__.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.026773 eminus-2.4.0/eminus/psp/pade/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ac-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ac-q29
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ag-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ag-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ag-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Al-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Am-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Am-q35
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ar-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/As-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/At-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Au-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Au-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Au-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/B-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      372 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ba-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ba-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Be-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Be-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Bi-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Bk-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Bk-q37
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Br-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/C-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ca-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ca-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cd-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cd-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ce-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cf-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cf-q38
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cl-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cm-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cm-q36
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Co-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Co-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cr-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cr-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cs-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      370 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cs-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cu-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cu-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Cu-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Dy-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Er-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Es-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Es-q39
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Eu-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/F-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Fe-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Fe-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Fm-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Fm-q40
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ga-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ga-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Gd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ge-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       88 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/H-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       89 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/He-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Hf-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Hg-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      410 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Hg-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ho-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      414 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/I-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      488 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/In-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/In-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ir-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ir-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/K-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      297 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/K-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Kr-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      473 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/La-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      161 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Li-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      119 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Li-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Lr-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Lr-q43
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Lu-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Md-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Md-q41
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      168 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mg-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mg-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mn-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mn-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mo-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Mo-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/N-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      212 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Na-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      166 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Na-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Nb-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Nb-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Nd-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      232 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ne-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ni-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ni-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/No-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/No-q42
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Np-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Np-q33
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      150 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/O-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Os-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Os-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/P-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pa-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pa-q31
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pb-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pd-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pm-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Po-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pr-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pt-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pt-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pu-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      640 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Pu-q34
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rb-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      334 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rb-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Re-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Re-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rh-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rh-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Rn-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ru-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ru-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      216 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/S-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sb-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sc-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sc-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      400 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Se-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Si-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sm-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sn-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      336 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sr-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      425 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Sr-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      503 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ta-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ta-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tb-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tc-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      390 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tc-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Te-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Th-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      635 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Th-q30
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ti-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      405 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Ti-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      392 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tl-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tl-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Tm-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/U-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      639 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/U-q32
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      340 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/V-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      404 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/V-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      502 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/W-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      389 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/W-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      415 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Xe-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      406 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Y-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      485 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Y-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      382 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Yb-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zn-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      395 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zn-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      341 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zn-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      407 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zr-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      486 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/Zr-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      842 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pade/__init__.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.038773 eminus-2.4.0/eminus/psp/pbe/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ac-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ac-q29
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      475 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ag-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ag-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Al-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Am-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Am-q35
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ar-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/As-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/At-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Au-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      571 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Au-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/B-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      359 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ba-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      107 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Be-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Bi-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Bi-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Bk-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Bk-q37
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Br-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/C-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      323 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ca-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      475 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cd-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ce-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      465 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ce-q30
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cf-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cf-q38
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cl-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cm-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cm-q36
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Co-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cr-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      358 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cs-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cu-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Cu-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Dy-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Er-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Es-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Es-q39
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Eu-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/F-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Fe-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Fm-q22
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Fm-q40
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ga-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ga-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Gd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ge-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       76 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/H-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       77 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/He-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Hf-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Hg-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ho-q21
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      402 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/I-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      475 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/In-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/In-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ir-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ir-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      285 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/K-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Kr-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      364 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/La-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      107 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Li-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Lr-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Lr-q43
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Lu-q25
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Md-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Md-q41
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      155 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Mg-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      200 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Mg-q2
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Mn-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Mo-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/N-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      200 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Na-q1
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      154 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Na-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Nb-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Nd-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      220 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ne-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ni-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/No-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/No-q42
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Np-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Np-q33
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      138 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/O-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Os-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Os-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      204 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/P-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pa-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pa-q31
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pb-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pb-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pd-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pd-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pm-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Po-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pr-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pt-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      586 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pt-q18
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pu-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      627 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Pu-q34
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      322 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Rb-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Re-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Re-q7
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Rh-q17
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Rh-q9
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Rn-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ru-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ru-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      204 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/S-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sb-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sc-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      388 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Se-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      205 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Si-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sm-q16
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sn-q4
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      323 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Sr-q10
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      490 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ta-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      378 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ta-q5
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tb-q19
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tc-q15
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Te-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Th-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      622 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Th-q30
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Ti-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      379 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tl-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tl-q3
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Tm-q23
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      626 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/U-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      630 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/U-q14_old
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      626 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/U-q32
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      327 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/V-q13
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      489 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/W-q14
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      377 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/W-q6
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      403 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Xe-q8
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      393 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Y-q11
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      369 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Yb-q24
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Zn-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      328 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Zn-q20
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      394 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/Zr-q12
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      843 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/psp/pbe/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    12469 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/scf.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     9555 2023-05-22 13:25:09.000000 eminus-2.4.0/eminus/tools.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3048 2023-05-05 09:27:14.000000 eminus-2.4.0/eminus/units.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     5521 2023-05-05 09:27:44.000000 eminus-2.4.0/eminus/utils.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1473 2023-05-23 09:48:58.000000 eminus-2.4.0/eminus/version.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.042773 eminus-2.4.0/eminus/xc/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      789 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      360 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4348 2023-05-17 14:59:59.000000 eminus-2.4.0/eminus/xc/gga_c_chachiyo.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4415 2023-05-17 22:17:28.000000 eminus-2.4.0/eminus/xc/gga_c_pbe.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1240 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/gga_c_pbe_sol.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2695 2023-05-17 22:16:05.000000 eminus-2.4.0/eminus/xc/gga_x_chachiyo.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     4334 2023-05-17 16:20:03.000000 eminus-2.4.0/eminus/xc/gga_x_pbe.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1225 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/gga_x_pbe_sol.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3200 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_chachiyo.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1952 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_chachiyo_mod.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3467 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_pw.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1224 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_pw_mod.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3084 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_c_vwn.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1646 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/lda_x.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10217 2023-05-17 14:03:34.000000 eminus-2.4.0/eminus/xc/utils.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-05-23 10:05:07.010773 eminus-2.4.0/eminus.egg-info/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3820 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/PKG-INFO
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     7893 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2022-09-27 12:14:58.000000 eminus-2.4.0/eminus.egg-info/not-zip-safe
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      330 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/requires.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        7 2023-05-23 10:05:06.000000 eminus-2.4.0/eminus.egg-info/top_level.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       86 2023-05-05 09:27:44.000000 eminus-2.4.0/pyproject.toml
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       38 2023-05-23 10:05:07.042773 eminus-2.4.0/setup.cfg
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3436 2023-05-05 09:27:44.000000 eminus-2.4.0/setup.py
```

### Comparing `eminus-2.3.0/CHANGELOG.md` & `eminus-2.4.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changelog
 =========
 
+v2.4.0 - May 23, 2023
+---------------------
+- New features
+   - Add GGA functionals!
+      - Add internal PBE, PBEsol, and Chachiyo functionals
+      - Option to use all GGAs from Libxc using pylibxc or PySCF
+- Miscellaneous
+   - Add Thomas-Fermi and von Weizsäcker kinetic energy density functions
+   - Rewrite functionals for better readability
+   - Fix Torch operators in some edge cases
+   - Merge configuration files in tox.ini
+   - Update minimum versions of dependencies
+
+----
+
 v2.3.0 - May 02, 2023
 ---------------------
 - New features
    - Add Torch powered FFT operators as an extra
       - Up to 20% faster calculations
    - Add a consolidated configuration class
       - Easier configuration and more performance infos
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eminus-2.3.0/LICENSE` & `eminus-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/PKG-INFO` & `eminus-2.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eminus
-Version: 2.3.0
+Version: 2.4.0
 Summary: A plane wave density functional theory code.
 Home-page: https://github.com/wangenau/eminus
 Author: Wanja Timm Schulze
 Author-email: wangenau@protonmail.com
 License: APACHE2.0
 Project-URL: Bug Tracker, https://gitlab.com/wangenau/eminus/-/issues
 Project-URL: Changelog, https://wangenau.gitlab.io/eminus/changelog.html
@@ -74,22 +74,19 @@
 
 This project is licensed under the Apache 2.0 License - see the [LICENSE](https://gitlab.com/wangenau/eminus/-/blob/main/LICENSE) file for details.
 
 
 Changelog
 =========
 
-v2.3.0 - May 02, 2023
+v2.4.0 - May 23, 2023
 ---------------------
 - New features
-   - Add Torch powered FFT operators as an extra
-      - Up to 20% faster calculations
-   - Add a consolidated configuration class
-      - Easier configuration and more performance infos
-   - Add a complete test suite
-      - Add CI/CD coverage reports
-   - Nix developer shell support
+   - Add GGA functionals!
+      - Add internal PBE, PBEsol, and Chachiyo functionals
+      - Option to use all GGAs from Libxc using pylibxc or PySCF
 - Miscellaneous
-   - Rewritten FODs guess function
-   - Simplify the FOD interface in io and viewer
-   - Fix a plethora of small bugs
-   - Update Docker image to Python 3.11
+   - Add Thomas-Fermi and von Weizsäcker kinetic energy density functions
+   - Rewrite functionals for better readability
+   - Fix Torch operators in some edge cases
+   - Merge configuration files in tox.ini
+   - Update minimum versions of dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eminus-2.3.0/README.md` & `eminus-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/README.md` & `eminus-2.4.0/eminus/README.md`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/__init__.py` & `eminus-2.4.0/eminus/__init__.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/atoms.py` & `eminus-2.4.0/eminus/atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
             Examples: 10; [10, 10, 10]; (7, 8, 9),
             Default: 20 Bohr (ca. 10.5 Angstrom).
         ecut (float | None): Cut-off energy.
 
             None will disable the G-Vector truncation (needs a separate s).
             Default: 30 Hartree (ca. 816 eV).
-        Z (int | list | tuple | ndarray | dict | None): Valence charge per atom.
+        Z (int | list | tuple | ndarray | dict | str | None): Valence charge per atom.
 
             The charges should not differ for same species. None will use valence charges from GTH
             files. The same charge for every atom will be assumed for single integers.
 
             Example: 1; [4, 1, 1, 1, 1],
             Default: None
         s (int | list | tuple | ndarray | None): Real-space sampling of the cell.
@@ -190,18 +190,22 @@
             self.Z = [self.Z] * self.Natoms
         if isinstance(self.Z, dict):
             self.Z = [self.Z[ia] for ia in self.atom]
         if isinstance(self.Z, (list, tuple)):
             self.Z = np.asarray(self.Z)
 
         # If no charge is given, use the ionic charge from the GTH files
-        if self.Z is None:
+        if self.Z is None or isinstance(self.Z, str):
+            if isinstance(self.Z, str):
+                xc = self.Z.lower()
+            else:
+                xc = 'pbe'
             Z = []
             for ia in range(self.Natoms):
-                gth_dict = read_gth(self.atom[ia])
+                gth_dict = read_gth(self.atom[ia], xc=xc)
                 Z.append(gth_dict['Zion'])
             self.Z = np.asarray(Z)
         return
 
     def _set_cell_size(self):
         '''Validate the a input.'''
         # Do this early on, since it is needed in many functions
```

### Comparing `eminus-2.3.0/eminus/config.py` & `eminus-2.4.0/eminus/config.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/data.py` & `eminus-2.4.0/eminus/data.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/dft.py` & `eminus-2.4.0/eminus/dft.py`

 * *Files 15% similar despite different names*

```diff
@@ -91,14 +91,32 @@
     Yrs = atoms.I(Y)
     n = np.empty((atoms.Nspin, len(atoms.r), atoms.Nstate))
     for spin in range(atoms.Nspin):
         n[spin] = atoms.f[spin] * np.real(Yrs[spin].conj() * Yrs[spin])
     return n
 
 
+def get_grad_n_spin(atoms, n_spin):
+    '''Calculate the gradient of densities per spin channel.
+
+    Args:
+        atoms: Atoms object.
+        n_spin (ndarray): Real-space electronic densities per spin channel.
+
+    Returns:
+        ndarray: Gradients of densities per spin channel.
+    '''
+    dn_spin = np.empty((atoms.Nspin, len(atoms.r), 3))
+    for spin in range(atoms.Nspin):
+        Gn = 1j * atoms.G * atoms.J(n_spin[spin])[:, None]
+        for i in range(3):
+            dn_spin[spin, :, i] = np.real(atoms.I(Gn[:, i]))
+    return dn_spin
+
+
 @handle_spin_gracefully
 def orth(atoms, W):
     '''Orthogonalize coefficient matrix W.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
@@ -108,96 +126,135 @@
     Returns:
         ndarray: Orthogonalized wave functions.
     '''
     # Y = W (Wdag O(W))^-0.5
     return W @ inv(sqrtm(W.conj().T @ atoms.O(W)))
 
 
-def get_grad(scf, spin, W, Y=None, n=None, n_spin=None, phi=None, vxc=None):
+def get_grad(scf, spin, W, *args, **kwargs):
     '''Calculate the energy gradient with respect to W.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         scf: SCF object.
         spin (int): Spin variable to track weather to calculate the gradient for spin up or down.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
-    Keyword Args:
-        Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
-        n (ndarray): Real-space electronic density.
-        n_spin (ndarray): Real-space electronic densities per spin channel.
-        phi (ndarray): Hartree field.
-        vxc (ndarray): Exchange-correlation potential.
-
     Returns:
         ndarray: Gradient.
     '''
     atoms = scf.atoms
     F = np.diag(atoms.f[spin])
-    HW = H(scf, spin, W, Y, n, n_spin, phi, vxc)
+    HW = H(scf, spin, W, *args, **kwargs)
     WHW = W[spin].conj().T @ HW
     # U = Wdag O(W)
     OW = atoms.O(W[spin])
     U = W[spin].conj().T @ OW
     invU = inv(U)
     U12 = sqrtm(invU)
     # Htilde = U^-0.5 Wdag H(W) U^-0.5
     Ht = U12 @ WHW @ U12
     # grad E = H(W) - O(W) U^-1 (Wdag H(W)) (U^-0.5 F U^-0.5) + O(W) (U^-0.5 Q(Htilde F - F Htilde))
     return (HW - (OW @ invU) @ WHW) @ (U12 @ F @ U12) + OW @ (U12 @ Q(Ht @ F - F @ Ht, U))
 
 
-def H(scf, spin, W, Y=None, n=None, n_spin=None, phi=None, vxc=None):
+def H(scf, spin, W, Y=None, n=None, n_spin=None, dn_spin=None, phi=None, vxc=None, vsigma=None):
     '''Left-hand side of the eigenvalue equation.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         scf: SCF object.
         spin (int): Spin variable to track weather to calculate the gradient for spin up or down.
         W (ndarray): Expansion coefficients of unconstrained wave functions in reciprocal space.
 
     Keyword Args:
         Y (ndarray): Expansion coefficients of orthogonal wave functions in reciprocal space.
         n (ndarray): Real-space electronic density.
         n_spin (ndarray): Real-space electronic densities per spin channel.
+        dn_spin (ndarray): Real-space gradient of densities per spin channel.
         phi (ndarray): Hartree field.
         vxc (ndarray): Exchange-correlation potential.
+        vsigma (ndarray): Contracted gradient potential derivative.
 
     Returns:
         ndarray: Hamiltonian applied on W.
     '''
     atoms = scf.atoms
     # One can calculate everything from W,
     # but one can also use already computed results to save time
     if Y is None:
         Y = orth(atoms, W)
     if n_spin is None:
         n_spin = get_n_spin(atoms, Y, n)
+    if dn_spin is None and scf.psp == 'pbe':
+        dn_spin = get_grad_n_spin(atoms, n_spin)
     if n is None:
         n = get_n_total(atoms, Y, n_spin)
     if phi is None:
         phi = solve_poisson(atoms, n)
-    if vxc is None:
-        vxc = get_vxc(scf.xc, n_spin, atoms.Nspin)
+    if vxc is None or (vsigma is None and scf.psp == 'pbe'):
+        vxc, vsigma = get_vxc(scf.xc, n_spin, atoms.Nspin, dn_spin)
 
     # We get the full potential in the functional definition (different to the DFT++ notation)
+    # Applay the gradient correction to the potential if a GGA functional is used
+    if scf.psp == 'pbe':
+        vxc = gradient_correction(atoms, dn_spin, vxc, vsigma)
     # Normally Vxc = Jdag(O(J(exc))) + diag(exc') Jdag(O(J(n)))
     Vxc = atoms.Jdag(atoms.O(atoms.J(vxc[spin])))
     # Vkin = -0.5 L(W)
     Vkin_psi = -0.5 * atoms.L(W[spin])
     # Veff = Jdag(Vion) + Jdag(O(J(vxc))) + Jdag(O(phi))
     Veff = scf.Vloc + Vxc + atoms.Jdag(atoms.O(phi))
     Vnonloc_psi = calc_Vnonloc(scf, W[spin])
     # H = Vkin + Idag(diag(Veff))I + Vnonloc
     # Diag(a) * B can be written as a * B if a is a column vector
     return Vkin_psi + atoms.Idag(Veff[:, None] * atoms.I(W[spin])) + Vnonloc_psi
 
 
+def gradient_correction(atoms, dn_spin, vxc, vsigma):
+    '''Calculate the gradient corrected exchange-correlation potential.
+
+    Reference: Chem. Phys. Lett. 199, 557.
+
+    Args:
+        atoms: Atoms object.
+        dn_spin (ndarray): Real-space gradient of densities per spin channel.
+        vxc (ndarray): Exchange-correlation potential.
+        vsigma (ndarray): Contracted gradient potential derivative.
+
+    Returns:
+        ndarray: Gradient corrected potential.
+    '''
+    # sigma is |dn|^2, while vsigma is n * d exc/d sigma
+    h = np.zeros_like(dn_spin)
+    if atoms.Nspin == 1:
+        # In the unpolarized case we have no spin mixing and only one spin density
+        h[0] = 2 * vsigma[0][:, None] * dn_spin[0]
+    else:
+        # In the polarized case we would get for spin up (and similar for spin down)
+        # Vxc_u = vxc_u - Nabla dot (2 vsigma_uu * dn_u + vsigma_ud * dn_d)
+        # h is the expression in the brackets
+        h[0] = 2 * vsigma[0][:, None] * dn_spin[0] + vsigma[1][:, None] * dn_spin[1]
+        h[1] = 2 * vsigma[2][:, None] * dn_spin[1] + vsigma[1][:, None] * dn_spin[0]
+
+    # Calculate Nabla dot h
+    divh = np.zeros_like(vxc)
+    for spin in range(atoms.Nspin):
+        Gh = np.empty((len(atoms.G2), 3), dtype=complex)
+        for i in range(3):
+            Gh[:, i] = atoms.J(h[spin, :, i])
+        Gdivh = 1j * np.sum(atoms.G * Gh, axis=1)
+        divh[spin] = np.real(atoms.I(Gdivh))
+
+    # Subtract the gradient correction
+    return vxc - divh
+
+
 def Q(inp, U):
     '''Operator needed to calculate gradients with non-constant occupations.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         inp (ndarray): Coefficients input array.
@@ -301,15 +358,15 @@
     atoms = scf.atoms
     # Start with randomized wave functions
     W = guess_random(scf, complex=complex)
 
     sigma = 0.5
     normal = (2 * np.pi * sigma**2)**(3 / 2)
     # Calculate a density from normalized Gauss functions
-    n = np.zeros(len(atoms.r))
+    n = np.zeros(len(atoms.r)) + 1e-15  # Add a small epsilon to prevent divisions by zero in exc
     for ia in range(atoms.Natoms):
         r = norm(atoms.r - atoms.X[ia], axis=1)
         n += atoms.Z[ia] * np.exp(-r**2 / (2 * sigma**2)) / normal
     # Calculate the eigenfunctions
     return get_psi(scf, W, n)
```

### Comparing `eminus-2.3.0/eminus/domains.py` & `eminus-2.4.0/eminus/domains.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/energies.py` & `eminus-2.4.0/eminus/energies.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 '''Calculate different energy contributions.'''
 import dataclasses
 
 import numpy as np
 from scipy.linalg import inv, norm
 from scipy.special import erfc
 
-from .dft import get_n_single, solve_poisson
+from .dft import get_grad_n_spin, get_n_single, solve_poisson
 from .xc import get_exc
 
 
 @dataclasses.dataclass
 class Energy:
     '''Energy class to save energy contributions in one place.'''
     Ekin: float = 0     #: Kinetic energy.
@@ -90,34 +90,37 @@
     '''
     if phi is None:
         phi = solve_poisson(atoms, n)
     # Ecoul = 0.5 (J(n))dag O(phi)
     return np.real(0.5 * n @ atoms.Jdag(atoms.O(phi)))
 
 
-def get_Exc(scf, n, exc=None, n_spin=None, Nspin=2):
+def get_Exc(scf, n, exc=None, n_spin=None, dn_spin=None, Nspin=2):
     '''Calculate the exchange-correlation energy.
 
     Reference: Comput. Phys. Commun. 128, 1.
 
     Args:
         scf: SCF object.
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
         exc (ndarray): Exchange-correlation energy density.
         n_spin (ndarray): Real-space electronic densities per spin channel.
+        dn_spin (ndarray): Real-space gradient of densities per spin channel.
         Nspin (int): Number of spin states.
 
     Returns:
         float: Exchange-correlation energy in Hartree.
     '''
     atoms = scf.atoms
     if exc is None:
-        exc = get_exc(scf.xc, n_spin, Nspin)
+        if dn_spin is None and scf.psp == 'pbe':
+            dn_spin = get_grad_n_spin(atoms, n_spin)
+        exc = get_exc(scf.xc, n_spin, Nspin, dn_spin)
     # Exc = (J(n))dag O(J(exc))
     return np.real(n @ atoms.Jdag(atoms.O(atoms.J(exc))))
 
 
 def get_Eloc(scf, n):
     '''Calculate the local energy contribution.
```

### Comparing `eminus-2.3.0/eminus/extras/__init__.py` & `eminus-2.4.0/eminus/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/extras/fods.py` & `eminus-2.4.0/eminus/extras/fods.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,26 +57,25 @@
             # If not continue with randomly 'displaced' orbitals
             noise = rng.normal(scale=5e-4, size=tmp_orb.shape)
             localizer.mo_coeff = tmp_orb + noise
         loc_orb.append(tmp_orb)
     return loc_orb
 
 
-def get_fods(object, basis='pc-1', loc='FB', clean=True, elec_symbols=None):
+def get_fods(object, basis='pc-1', loc='FB', elec_symbols=None):
     '''Generate FOD positions using the PyCOM method.
 
     Reference: J. Comput. Chem. 40, 2843.
 
     Args:
         object: Atoms or SCF object.
 
     Keyword Args:
         basis (str): Basis set for the DFT calculation.
         loc (str): Localization method (case insensitive).
-        clean (bool): Remove log files.
         elec_symbols (list): Identifier for up and down FODs.
 
     Returns:
         ndarray: FOD positions.
     '''
     try:
         from pyscf.gto import Mole
```

### Comparing `eminus-2.3.0/eminus/extras/torch.py` & `eminus-2.4.0/eminus/extras/torch.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     Returns:
         ndarray: The operator applied on W.
     '''
     import torch
     n = np.prod(atoms.s)
     s = tuple(atoms.s)
 
-    Wfft = torch.from_numpy(W)
+    Wfft = torch.from_numpy(np.copy(W))
     if config.use_gpu:
         Wfft = Wfft.cuda()
 
     if W.ndim == 1:
         Wfft = Wfft.view(s)
         F = torch.fft.fftn(Wfft, s=s, norm='forward').view(n)
     elif W.ndim == 2:
@@ -122,29 +122,29 @@
     Returns:
         ndarray: The operator applied on W.
     '''
     import torch
     n = np.prod(atoms.s)
     s = tuple(atoms.s)
 
-    Wfft = torch.from_numpy(W)
+    Wfft = torch.from_numpy(np.copy(W))
     if config.use_gpu:
         Wfft = Wfft.cuda()
 
     if W.ndim == 1:
         Wfft = Wfft.view(s)
-        F = torch.fft.fftn(Wfft, s=s, norm='backward').view(n)
+        F = torch.fft.fftn(Wfft, s=s, norm='forward').view(n)
     elif W.ndim == 2:
         Wfft = Wfft.view(s + (atoms.Nstate,))
-        F = torch.fft.fftn(Wfft, s=s, norm='backward', dim=(0, 1, 2)).view(n, atoms.Nstate)
+        F = torch.fft.fftn(Wfft, s=s, norm='forward', dim=(0, 1, 2)).view(n, atoms.Nstate)
     else:
         Wfft = Wfft.view((atoms.Nspin,) + s + (atoms.Nstate,))
-        F = torch.fft.fftn(Wfft, s=s, norm='backward', dim=(1, 2, 3)).view(atoms.Nspin, n,
-                                                                           atoms.Nstate)
-    F = F.detach().cpu().numpy()
+        F = torch.fft.fftn(Wfft, s=s, norm='forward', dim=(1, 2, 3)).view(atoms.Nspin, n,
+                                                                          atoms.Nstate)
+    F = F.detach().cpu().numpy() * n
     if not full:
         if F.ndim < 3:
             return F[atoms.active]
         return F[:, atoms.active[0]]
     return F
 
 
@@ -180,16 +180,16 @@
 
     Wfft = torch.from_numpy(Wfft)
     if config.use_gpu:
         Wfft = Wfft.cuda()
 
     if W.ndim == 1:
         Wfft = Wfft.view(s)
-        Finv = torch.fft.ifftn(Wfft, s=s, norm='backward').view(n)
+        Finv = torch.fft.ifftn(Wfft, s=s, norm='forward').view(n)
     elif W.ndim == 2:
         Wfft = Wfft.view(s + (atoms.Nstate,))
-        Finv = torch.fft.ifftn(Wfft, s=s, norm='backward', dim=(0, 1, 2)).view(n, atoms.Nstate)
+        Finv = torch.fft.ifftn(Wfft, s=s, norm='forward', dim=(0, 1, 2)).view(n, atoms.Nstate)
     else:
         Wfft = Wfft.view((atoms.Nspin,) + s + (atoms.Nstate,))
-        Finv = torch.fft.ifftn(Wfft, s=s, norm='backward', dim=(1, 2, 3)).view(atoms.Nspin, n,
-                                                                               atoms.Nstate)
-    return Finv.detach().cpu().numpy()
+        Finv = torch.fft.ifftn(Wfft, s=s, norm='forward', dim=(1, 2, 3)).view(atoms.Nspin, n,
+                                                                              atoms.Nstate)
+    return Finv.detach().cpu().numpy() / n
```

### Comparing `eminus-2.3.0/eminus/extras/viewer.py` & `eminus-2.4.0/eminus/extras/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,39 +47,39 @@
     # Add species one by one to be able to have them named and be selectable in the legend
     # Note: The size scaling is mostly arbitray and has no meaning
     for ia in sorted(set(atoms.atom)):
         mask = np.where(np.asarray(atoms.atom) == ia)[0]
         atom_data = go.Scatter3d(x=atoms.X[mask, 0], y=atoms.X[mask, 1], z=atoms.X[mask, 2],
                                  name=ia,
                                  mode='markers',
-                                 marker=dict(size=2 * np.pi * np.sqrt(COVALENT_RADII[ia]),
-                                             color=CPK_COLORS[ia],
-                                             line={'color': 'black', 'width': 2}))
+                                 marker={'size': 2 * np.pi * np.sqrt(COVALENT_RADII[ia]),
+                                         'color': CPK_COLORS[ia],
+                                         'line': {'color': 'black', 'width': 2}})
         fig.add_trace(atom_data)
     if extra is not None:
         # If a list has been provided with the length of two it has to be FODs
         if isinstance(extra, list):
             if len(extra[0]) != 0:
                 extra_data = go.Scatter3d(x=extra[0][:, 0], y=extra[0][:, 1], z=extra[0][:, 2],
                                           name='up-FOD',
                                           mode='markers',
-                                          marker=dict(size=np.pi, color='red'))
+                                          marker={'size': np.pi, 'color': 'red'})
                 fig.add_trace(extra_data)
             if len(extra) > 1 and len(extra[1]) != 0:
                 extra_data = go.Scatter3d(x=extra[1][:, 0], y=extra[1][:, 1], z=extra[1][:, 2],
                                           name='down-FOD',
                                           mode='markers',
-                                          marker=dict(size=np.pi, color='green'))
+                                          marker={'size': np.pi, 'color': 'green'})
                 fig.add_trace(extra_data)
         # Treat extra as normal coordinates otherwise
         else:
             extra_data = go.Scatter3d(x=extra[:, 0], y=extra[:, 1], z=extra[:, 2],
                                       name='Coordinates',
                                       mode='markers',
-                                      marker=dict(size=1, color='red'))
+                                      marker={'size': 1, 'color': 'red'})
             fig.add_trace(extra_data)
 
     # A density can be plotted for an scf object
     if plot_n:
         try:
             den_data = go.Volume(x=atoms.r[:, 0], y=atoms.r[:, 1], z=atoms.r[:, 2], value=object.n,
                                  name='Density',
```

### Comparing `eminus-2.3.0/eminus/gth.py` & `eminus-2.4.0/eminus/gth.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/io/__init__.py` & `eminus-2.4.0/eminus/io/__init__.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/io/cube.py` & `eminus-2.4.0/eminus/io/cube.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
     # Atomic units and a cuboidal cell that starts at (0,0,0) are assumed.
     with open(filename, 'r') as fh:
         lines = fh.readlines()
 
         # The first and second line can contain comments, print them if available
         comment = f'{lines[0].strip()}\n{lines[1].strip()}'
-        log.info(f'XYZ file comment: "{comment}"')
+        if comment:
+            log.info(f'XYZ file comment: "{comment}"')
 
         # Line 4 to 6 contain the sampling per axis, and the cell basis vectors with length a/s
         # A cuboidal cell is assumed, so only use the diagonal entries
         s = np.empty(3, dtype=int)
         a = np.empty(3)
         for i, line in enumerate(lines[3:6]):
             line_split = line.strip().split()
```

### Comparing `eminus-2.3.0/eminus/io/gth.py` & `eminus-2.4.0/eminus/io/gth.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 import pathlib
 
 import numpy as np
 
 from ..logger import log
 
 
-def read_gth(atom, charge=None, psp_path=None):
+def read_gth(atom, charge=None, xc='pade', psp_path=None):
     '''Read GTH files for a given atom.
 
     Reference: Phys. Rev. B 54, 1703.
 
     Args:
         atom (str): Atom name.
 
     Keyword Args:
         charge (int): Valence charge.
-        psp_path (str): Path to GTH pseudopotential files. Defaults to installation_path/pade/.
+        xc (str): Weather to use the pade or the pbe pseudopotential files.
+        psp_path (str): Path to GTH pseudopotential files. Defaults to installation_path/psp/.
 
     Returns:
         dict: GTH parameters.
     '''
     if psp_path is None:
         file_path = pathlib.Path(inspect.getfile(inspect.currentframe())).parent
-        psp_path = file_path.parent.joinpath('pade')
+        psp_path = file_path.parent.joinpath(f'psp/{xc}')
 
     if charge is not None:
         f_psp = psp_path.joinpath(f'{atom}-q{charge}')
     else:
         files = sorted(psp_path.glob(f'{atom}-q*'))
         try:
             f_psp = pathlib.Path(files[0])
```

### Comparing `eminus-2.3.0/eminus/io/json.py` & `eminus-2.4.0/eminus/io/json.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/io/pdb.py` & `eminus-2.4.0/eminus/io/pdb.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/io/xyz.py` & `eminus-2.4.0/eminus/io/xyz.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         lines = fh.readlines()
 
         # The first line contains the number of atoms
         Natoms = int(lines[0].strip())
 
         # The second line can contain a comment, print it if available
         comment = lines[1].strip()
-        log.info(f'XYZ file comment: "{comment}"')
+        if comment:
+            log.info(f'XYZ file comment: "{comment}"')
 
         atom = []
         X = []
         # Following lines contain atom positions with the format: Atom x-pos y-pos z-pos
         for line in lines[2:2 + Natoms]:
             line_split = line.strip().split()
             atom.append(line_split[0])
```

### Comparing `eminus-2.3.0/eminus/localizer.py` & `eminus-2.4.0/eminus/localizer.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/logger.py` & `eminus-2.4.0/eminus/logger.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/minimizer.py` & `eminus-2.4.0/eminus/minimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 '''Minimization algorithms.'''
 import logging
 
 import numpy as np
 
-from .dft import get_grad, get_n_spin, get_n_total, orth, solve_poisson
+from .dft import get_grad, get_grad_n_spin, get_n_spin, get_n_total, orth, solve_poisson
 from .energies import get_E
 from .logger import name
 from .utils import dotprod
 from .xc import get_xc
 
 
 def scf_step(scf):
@@ -22,16 +22,18 @@
     Returns:
         float: Total energy.
     '''
     atoms = scf.atoms
     scf.Y = orth(atoms, scf.W)
     scf.n_spin = get_n_spin(atoms, scf.Y)
     scf.n = get_n_total(atoms, scf.Y, scf.n_spin)
+    if scf.psp == 'pbe':
+        scf.dn_spin = get_grad_n_spin(atoms, scf.n_spin)
     scf.phi = solve_poisson(atoms, scf.n)
-    scf.exc, scf.vxc = get_xc(scf.xc, scf.n_spin, atoms.Nspin)
+    scf.exc, scf.vxc, scf.vsigma = get_xc(scf.xc, scf.n_spin, atoms.Nspin, scf.dn_spin)
     return get_E(scf)
 
 
 def check_energies(scf, Elist, linmin='', cg=''):
     '''Check the energies for every SCF cycle and handle the output.
 
     Args:
@@ -91,15 +93,15 @@
 
     for _ in range(Nit):
         c = cost(scf)
         costs.append(c)
         if condition(scf, costs):
             break
         for spin in range(atoms.Nspin):
-            g = grad(scf, spin, scf.W, scf.Y, scf.n, scf.n_spin, scf.phi, scf.vxc)
+            g = grad(scf, spin, scf.W, **scf.precomputed)
             scf.W[spin] = scf.W[spin] - betat * g
     return costs
 
 
 @name('line minimization')
 def lm(scf, Nit, cost=scf_step, grad=get_grad, condition=check_energies, betat=3e-5):
     '''Line minimization algorithm.
@@ -139,15 +141,15 @@
 
     c = cost(scf)
     costs.append(c)
     condition(scf, costs)
 
     for _ in range(1, Nit):
         for spin in range(atoms.Nspin):
-            g = grad(scf, spin, scf.W, scf.Y, scf.n, scf.n_spin, scf.phi, scf.vxc)
+            g = grad(scf, spin, scf.W, **scf.precomputed)
             # Calculate linmin each spin seperately
             if scf.log.level <= logging.DEBUG:
                 linmin[spin] = dotprod(g, d[spin]) / \
                     np.sqrt(dotprod(g, g) * dotprod(d[spin], d[spin]))
             d[spin] = -g
             gt = grad(scf, spin, scf.W + betat * d[spin])
             beta[spin] = betat * dotprod(g, d[spin]) / dotprod(g - gt, d[spin])
@@ -200,15 +202,15 @@
 
     c = cost(scf)
     costs.append(c)
     condition(scf, costs)
 
     for _ in range(1, Nit):
         for spin in range(atoms.Nspin):
-            g = grad(scf, spin, scf.W, scf.Y, scf.n, scf.n_spin, scf.phi, scf.vxc)
+            g = grad(scf, spin, scf.W, **scf.precomputed)
             # Calculate linmin each spin seperately
             if scf.log.level <= logging.DEBUG:
                 linmin[spin] = dotprod(g, d[spin]) / \
                     np.sqrt(dotprod(g, g) * dotprod(d[spin], d[spin]))
             d[spin] = -atoms.K(g)
             gt = grad(scf, spin, scf.W + betat * d[spin])
             beta[spin] = betat * dotprod(g, d[spin]) / dotprod(g - gt, d[spin])
@@ -266,15 +268,15 @@
 
     c = cost(scf)
     costs.append(c)
     condition(scf, costs)
 
     for _ in range(1, Nit):
         for spin in range(atoms.Nspin):
-            g = grad(scf, spin, scf.W, scf.Y, scf.n, scf.n_spin, scf.phi, scf.vxc)
+            g = grad(scf, spin, scf.W, **scf.precomputed)
             # Calculate linmin and cg for each spin seperately
             if scf.log.level <= logging.DEBUG:
                 linmin[spin] = dotprod(g, d_old[spin]) / \
                     np.sqrt(dotprod(g, g) * dotprod(d_old[spin], d_old[spin]))
                 cg[spin] = dotprod(g, g_old[spin]) / \
                     np.sqrt(dotprod(g, g) * dotprod(g_old[spin], g_old[spin]))
             if scf.cgform == 1:  # Fletcher-Reeves
@@ -344,15 +346,15 @@
 
     c = cost(scf)
     costs.append(c)
     condition(scf, costs)
 
     for _ in range(1, Nit):
         for spin in range(atoms.Nspin):
-            g = grad(scf, spin, scf.W, scf.Y, scf.n, scf.n_spin, scf.phi, scf.vxc)
+            g = grad(scf, spin, scf.W, **scf.precomputed)
             # Calculate linmin and cg for each spin seperately
             if scf.log.level <= logging.DEBUG:
                 linmin[spin] = dotprod(g, d_old[spin]) / \
                     np.sqrt(dotprod(g, g) * dotprod(d_old[spin], d_old[spin]))
                 cg[spin] = dotprod(g, atoms.K(g_old[spin])) / \
                     np.sqrt(dotprod(g, atoms.K(g)) * dotprod(g_old[spin], atoms.K(g_old[spin])))
             if scf.cgform == 1:  # Fletcher-Reeves
```

### Comparing `eminus-2.3.0/eminus/operators.py` & `eminus-2.4.0/eminus/operators.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/orbitals.py` & `eminus-2.4.0/eminus/orbitals.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Ac-q11` & `eminus-2.4.0/eminus/psp/pade/Ac-q11`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Ac-q29` & `eminus-2.4.0/eminus/psp/pade/Ac-q29`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Am-q17` & `eminus-2.4.0/eminus/psp/pade/Am-q17`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Am-q35` & `eminus-2.4.0/eminus/psp/pade/Am-q35`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Bk-q19` & `eminus-2.4.0/eminus/psp/pade/Bk-q19`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Bk-q37` & `eminus-2.4.0/eminus/psp/pade/Bk-q37`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Cf-q20` & `eminus-2.4.0/eminus/psp/pade/Cf-q20`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Cf-q38` & `eminus-2.4.0/eminus/psp/pade/Cf-q38`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Cm-q18` & `eminus-2.4.0/eminus/psp/pade/Cm-q18`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Cm-q36` & `eminus-2.4.0/eminus/psp/pade/Cm-q36`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Es-q21` & `eminus-2.4.0/eminus/psp/pade/Es-q21`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Es-q39` & `eminus-2.4.0/eminus/psp/pade/Es-q39`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Fm-q22` & `eminus-2.4.0/eminus/psp/pade/Fm-q22`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Fm-q40` & `eminus-2.4.0/eminus/psp/pade/Fm-q40`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Lr-q25` & `eminus-2.4.0/eminus/psp/pade/Lr-q25`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Lr-q43` & `eminus-2.4.0/eminus/psp/pade/Lr-q43`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Md-q23` & `eminus-2.4.0/eminus/psp/pade/Md-q23`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Md-q41` & `eminus-2.4.0/eminus/psp/pade/Md-q41`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/No-q24` & `eminus-2.4.0/eminus/psp/pade/No-q24`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/No-q42` & `eminus-2.4.0/eminus/psp/pade/No-q42`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Np-q15` & `eminus-2.4.0/eminus/psp/pade/Np-q15`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Np-q33` & `eminus-2.4.0/eminus/psp/pade/Np-q33`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Pa-q13` & `eminus-2.4.0/eminus/psp/pade/Pa-q13`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Pa-q31` & `eminus-2.4.0/eminus/psp/pade/Pa-q31`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Pu-q16` & `eminus-2.4.0/eminus/psp/pade/Pu-q16`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Pu-q34` & `eminus-2.4.0/eminus/psp/pade/Pu-q34`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Th-q12` & `eminus-2.4.0/eminus/psp/pade/Th-q12`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/Th-q30` & `eminus-2.4.0/eminus/psp/pade/Th-q30`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/U-q14` & `eminus-2.4.0/eminus/psp/pade/U-q14`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/pade/U-q32` & `eminus-2.4.0/eminus/psp/pade/U-q32`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/potentials.py` & `eminus-2.4.0/eminus/potentials.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/scf.py` & `eminus-2.4.0/eminus/scf.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .gth import init_gth_loc, init_gth_nonloc
 from .io import read_gth
 from .logger import create_logger, get_level
 from .minimizer import IMPLEMENTED
 from .potentials import init_pot
 from .tools import center_of_mass
 from .version import info
-from .xc import parse_functionals
+from .xc import parse_functionals, parse_psp
 
 
 class SCF:
     '''Perform direct minimizations.
 
     Args:
         atoms: Atoms object.
@@ -93,29 +93,36 @@
 
         # Parameters that will be built out of the inputs
         self.GTH = {}             # Dictionary of GTH parameters per atom species
         self.Vloc = None          # Local pseudopotential contribution
         self.NbetaNL = 0          # Number of projector functions for the non-local gth potential
         self.prj2beta = None      # Index matrix to map to the correct projector function
         self.betaNL = None        # Atomic-centered projector functions
+        self.psp = None           # Type of GTH pseudopotential that will be used
         self.print_precision = 6  # Precision of the energy in the minimizer logger
         self.initialize()
 
     def clear(self):
         '''Initialize and clear intermediate results.'''
-        self.Y = None       # Orthogonal wave functions
-        self.n_spin = None  # Electronic densities per spin
-        self.phi = None     # Hartree field
-        self.exc = None     # Exchange-correlation energy density
-        self.vxc = None     # Exchange-correlation potential
+        self.Y = None        # Orthogonal wave functions
+        self.n_spin = None   # Electronic densities per spin
+        self.dn_spin = None  # Gradient of electronic densities per spin
+        self.phi = None      # Hartree field
+        self.exc = None      # Exchange-correlation energy density
+        self.vxc = None      # Exchange-correlation potential
+        self.vsigma = None   # n times d exc/d |dn|^2
+        self.precomputed = {'Y': self.Y, 'n': self.n, 'n_spin': self.n_spin,
+                            'dn_spin': self.dn_spin, 'phi': self.phi, 'vxc': self.vxc,
+                            'vsigma': self.vsigma}
         return self
 
     def initialize(self):
         '''Validate inputs, update them and build all necessary parameters.'''
         self.xc = parse_functionals(self.xc)
+        self.psp = parse_psp(self.xc)
         # Build the atoms object if necessary and make a copy
         # This way the atoms object in scf is independent but we ensure that both atoms are build
         if not self.atoms.is_built:
             self.atoms = copy.copy(self.atoms.build())
         else:
             self.atoms = copy.copy(self.atoms)
         self._set_potential()
@@ -225,15 +232,15 @@
         return self
 
     def _set_potential(self):
         '''Build the potential.'''
         atoms = self.atoms
         if self.pot == 'gth':
             for ia in range(atoms.Natoms):
-                self.GTH[atoms.atom[ia]] = read_gth(atoms.atom[ia], atoms.Z[ia])
+                self.GTH[atoms.atom[ia]] = read_gth(atoms.atom[ia], atoms.Z[ia], xc=self.psp)
             # Set up the local and non-local part
             self.Vloc = init_gth_loc(self)
             self.NbetaNL, self.prj2beta, self.betaNL = init_gth_nonloc(self)
         else:
             self.Vloc = init_pot(self)
         return
 
@@ -250,16 +257,18 @@
             self.W = guess_pseudo(self, seed=1234)
         else:
             self.log.error(f'No guess found for "{self.guess}"')
         return
 
     def __repr__(self):
         '''Print the parameters stored in the SCF object.'''
+        # Use chr(10) to create a linebreak since backslashes are not allowed in f-strings
         return f'XC functionals: {self.xc}\n' \
                f'Potential: {self.pot}\n' \
+               f'{f"GTH files: {self.psp}" + chr(10) if self.pot == "gth" else ""}' \
                f'Starting guess: {self.guess}\n' \
                f'Convergence tolerance: {self.etol}\n' \
                f'Non-local contribution: {self.NbetaNL > 0}'
 
     @property
     def verbose(self):
         '''Verbosity level.'''
@@ -273,28 +282,26 @@
 
 
 class RSCF(SCF):
     '''SCF class for spin-paired systems.
 
     Inherited from :class:`eminus.scf.SCF`.
     '''
-
     def initialize(self):
         '''Validate inputs, update them and build all necessary parameters.'''
         self.atoms = copy.copy(self.atoms)
         self.atoms._set_states(Nspin=1)
         super().initialize()
         return self
 
 
 class USCF(SCF):
     '''SCF class for spin-polarized systems.
 
     Inherited from :class:`eminus.scf.SCF`.
     '''
-
     def initialize(self):
         '''Validate inputs, update them and build all necessary parameters.'''
         self.atoms = copy.copy(self.atoms)
         self.atoms._set_states(Nspin=2)
         super().initialize()
         return self
```

### Comparing `eminus-2.3.0/eminus/tools.py` & `eminus-2.4.0/eminus/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 '''Various tools to check physical properties.'''
 import numpy as np
+from numpy.linalg import norm
 from scipy.optimize import minimize_scalar
 
-from .dft import get_epsilon
+from .dft import get_epsilon, get_grad_n_spin
 from .logger import log
 
 
 def cutoff2gridspacing(E):
     '''Convert plane wave energy cut-off to a real-space grid spacing.
 
     Reference: Phys. Rev. B 54, 14362.
@@ -66,22 +67,22 @@
     try:
         atoms = object.atoms
     except AttributeError:
         atoms = object
 
     coms = [np.array([])] * 2
     Ncom = psirs.shape[2]
-    for s in range(atoms.Nspin):
+    for spin in range(atoms.Nspin):
         coms_spin = np.empty((Ncom, 3))
 
         # Square orbitals
-        psi2 = np.real(psirs[s, :, :].conj() * psirs[s, :, :])
+        psi2 = np.real(psirs[spin, :, :].conj() * psirs[spin, :, :])
         for i in range(Ncom):
             coms_spin[i] = center_of_mass(atoms.r, psi2[:, i])
-        coms[s] = coms_spin
+        coms[spin] = coms_spin
     return coms
 
 
 def inertia_tensor(coords, masses=None):
     '''Calculate the inertia tensor for a set of coordinates and masses.
 
     Args:
@@ -276,7 +277,51 @@
 
     # Integrated density
     n_ref = np.sum(n)
     # Finding the isovalue is an optimization problem, minimizing the deviation above
     # The problem is bound by zero (no density) and the maximum value in n
     res = minimize_scalar(deviation, bounds=(0, np.max(n)), method='bounded')
     return res.x
+
+
+def get_tautf(scf):
+    '''Calculate the Thomas-Fermi kinetic energy densities per spin.
+
+    Reference: Phys. Lett. B 63, 395.
+
+    Args:
+        scf: SCF object.
+
+    Returns:
+        ndarray: Real space Thomas-Fermi kinetic energy density.
+    '''
+    atoms = scf.atoms
+    tautf = 3 / 10 * (atoms.Nspin * 3 * np.pi**2)**(2 / 3) * scf.n_spin**(5 / 3)
+
+    log.debug(f'Calculated Ekin:  {scf.energies.Ekin:.6f} Eh')
+    log.debug(f'Integrated tautf: {np.sum(tautf) * atoms.Omega / np.prod(atoms.s):.6f} Eh')
+    return tautf
+
+
+def get_tauw(scf):
+    '''Calculate the von Weizsäcker kinetic energy densities per spin.
+
+    Reference: Z. Phys. 96, 431.
+
+    Args:
+        scf: SCF object.
+
+    Returns:
+        ndarray: Real space von Weizsäcker kinetic energy density.
+    '''
+    atoms = scf.atoms
+    if scf.dn_spin is None:
+        dn_spin = get_grad_n_spin(atoms, scf.n_spin)
+    else:
+        dn_spin = scf.dn_spin
+    dn2 = norm(dn_spin, axis=2)**2
+    tauw = dn2 / (8 * scf.n_spin)
+
+    # For one- and two-electron systems the integrated KED has to be the same as the calculated KE
+    log.debug(f'Calculated Ekin:  {scf.energies.Ekin:.6f} Eh')
+    log.debug(f'Integrated tauw:  {np.sum(tauw) * atoms.Omega / np.prod(atoms.s):.6f} Eh')
+    return tauw
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eminus-2.3.0/eminus/units.py` & `eminus-2.4.0/eminus/units.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/utils.py` & `eminus-2.4.0/eminus/utils.py`

 * *Files identical despite different names*

### Comparing `eminus-2.3.0/eminus/version.py` & `eminus-2.4.0/eminus/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 '''Package version number and version info function.'''
 import importlib
 import platform
 import sys
 
-__version__ = '2.3.0'
+__version__ = '2.4.0'
 logo = (' ___ _____ _ ___ _ _ ___ \n'
         '| -_|     | |   | | |_ -|\n'
         '|___|_|_|_|_|_|_|___|___|\n')
 
 
 def info():
     '''Print version numbers and availability of packages.'''
```

### Comparing `eminus-2.3.0/eminus/xc/lda_c_chachiyo.py` & `eminus-2.4.0/eminus/xc/lda_c_chachiyo.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
     Returns:
         tuple[ndarray, ndarray]: Chachiyo correlation energy density and potential.
     '''
     a = -0.01554535  # (np.log(2) - 1) / (2 * np.pi**2)
     b = 20.4562557
 
-    pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 * n**(-1 / 3)
+    rs = (3 / (4 * np.pi * n))**(1 / 3)
     rs2 = rs**2
+    ecinner = 1 + b / rs + b / rs2
 
-    ec = a * np.log(1 + b / rs + b / rs2)
+    ec = a * np.log(ecinner)
     if exc_only:
-        return ec, None
+        return ec, None, None
 
     vc = ec + a * b * (2 + rs) / (3 * (b + b * rs + rs2))
-    return ec, np.array([vc])
+    return ec, np.array([vc]), None
 
 
 def chachiyo_scaling(zeta, exc_only=False):
     '''Weighting factor between the paramagnetic and the ferromagnetic case.
 
     Reference: J. Chem. Phys. 145, 021101.
 
@@ -76,27 +76,31 @@
         tuple[ndarray, ndarray]: Chachiyo correlation energy density and potential.
     '''
     a0 = -0.01554535   # (np.log(2) - 1) / (2 * np.pi**2)
     a1 = -0.007772675  # (np.log(2) - 1) / (4 * np.pi**2)
     b0 = 20.4562557
     b1 = 27.4203609
 
-    pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 * n**(-1 / 3)
+    rs = (3 / (4 * np.pi * n))**(1 / 3)
     rs2 = rs**2
 
     fzeta, dfdzeta = weight_function(zeta, exc_only=exc_only)
 
-    ec0 = a0 * np.log(1 + b0 / rs + b0 / rs2)
-    ec1 = a1 * np.log(1 + b1 / rs + b1 / rs2)
+    ec0inner = 1 + b0 / rs + b0 / rs2
+    ec1inner = 1 + b1 / rs + b1 / rs2
+    ec0 = a0 * np.log(ec0inner)
+    ec1 = a1 * np.log(ec1inner)
+
     ec = ec0 + (ec1 - ec0) * fzeta
     if exc_only:
-        return ec, None
+        return ec, None, None
 
     factor = -1 / rs2 - 2 / rs**3
-    dec0drs = a0 / (1 + b0 / rs + b0 / rs2) * b0 * factor
-    dec1drs = a1 / (1 + b1 / rs + b1 / rs2) * b1 * factor
-    prefactor = ec - rs / 3 * (dec0drs + (dec1drs - dec0drs) * fzeta)
-
-    vcup = prefactor + (ec1 - ec0) * dfdzeta * (1 - zeta)
-    vcdw = prefactor - (ec1 - ec0) * dfdzeta * (1 + zeta)
-    return ec, np.array([vcup, vcdw])
+    dec0drs = a0 / ec0inner * b0 * factor
+    dec1drs = a1 / ec1inner * b1 * factor
+    decdrs = dec0drs + (dec1drs - dec0drs) * fzeta
+    prefactor = ec - rs / 3 * decdrs
+    decdf = (ec1 - ec0) * dfdzeta
+
+    vcup = prefactor + decdf * (1 - zeta)
+    vcdw = prefactor - decdf * (1 + zeta)
+    return ec, np.array([vcup, vcdw]), None
```

### Comparing `eminus-2.3.0/eminus/xc/lda_c_chachiyo_mod.py` & `eminus-2.4.0/eminus/xc/lda_c_chachiyo_mod.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Returns:
         tuple[ndarray, ndarray]: Chachiyo correlation energy density and potential.
     '''
+    # Same as lda_c_chachiyo
     return lda_c_chachiyo(n, **kwargs)
 
 
-def chachiyo_mod_scaling(zeta, exc_only=False):
+def chachiyo_scaling_mod(zeta, exc_only=False):
     '''Modified weighting factor between the paramagnetic and the ferromagnetic case.
 
     Reference: Comput. Theor. Chem. 1172, 112669.
 
     Args:
         zeta (ndarray): Relative spin polarization.
 
@@ -53,8 +54,8 @@
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Returns:
         tuple[ndarray, ndarray]: Chachiyo correlation energy density and potential.
     '''
-    return lda_c_chachiyo_spin(n, zeta, weight_function=chachiyo_mod_scaling, **kwargs)
+    return lda_c_chachiyo_spin(n, zeta, weight_function=chachiyo_scaling_mod, **kwargs)
```

### Comparing `eminus-2.3.0/eminus/xc/lda_c_pw.py` & `eminus-2.4.0/eminus/xc/lda_c_vwn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,89 @@
 #!/usr/bin/env python3
-'''Perdew-Wang LDA correlation.
+'''Vosko-Wilk-Nusair LDA correlation.
 
-Reference: Phys. Rev. B 45, 13244.
+Reference: Phys. Rev. B 22, 3812.
 '''
 import numpy as np
 
 
-def lda_c_pw(n, a=0.031091, exc_only=False, **kwargs):
-    '''Perdew-Wang parametrization of the correlation functional (spin-paired).
+def lda_c_vwn(n, A=0.0310907, b=3.72744, c=12.9352, x0=-0.10498, exc_only=False, **kwargs):
+    '''Vosko-Wilk-Nusair parametrization of the correlation functional (spin-paired).
 
-    Corresponds to the functional with the label LDA_C_PW and ID 12 in Libxc.
-    Reference: Phys. Rev. B 45, 13244.
+    Corresponds to the functional with the label LDA_C_VWN and ID 7 in Libxc.
+    Reference: Phys. Rev. B 22, 3812.
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
-        a (float): Functional parameter.
         exc_only (bool): Only calculate the exchange-correlation energy density.
+        A (float): Functional parameter.
+        b (float): Functional parameter.
+        c (float): Functional parameter.
+        x0 (float): Functional parameter.
 
     Returns:
-        tuple[ndarray, ndarray]: PW correlation energy density and potential.
+        tuple[ndarray, ndarray]: VWN correlation energy density and potential.
     '''
-    a1 = 0.2137
-    b1 = 7.5957
-    b2 = 3.5876
-    b3 = 1.6382
-    b4 = 0.49294
-
-    pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 * n**(-1 / 3)
-    rs12 = np.sqrt(rs)
-    rs32 = rs * rs12
-    rs2 = rs**2
+    rs = (3 / (4 * np.pi * n))**(1 / 3)
 
-    om = 2 * a * (b1 * rs12 + b2 * rs + b3 * rs32 + b4 * rs2)
-    olog = np.log(1 + 1 / om)
+    x = np.sqrt(rs)
+    X = rs + b * x + c
+    Q = np.sqrt(4 * c - b**2)
+    fx0 = b * x0 / (x0**2 + b * x0 + c)
+    f3 = 2 * (2 * x0 + b) / Q
+    tx = 2 * x + b
+    tanx = np.arctan(Q / tx)
 
-    ec = -2 * a * (1 + a1 * rs) * olog
+    ec = A * (np.log(rs / X) + 2 * b / Q * tanx - fx0 * (np.log((x - x0)**2 / X) + f3 * tanx))
     if exc_only:
-        return ec, None
+        return ec, None, None
 
-    dom = 2 * a * (0.5 * b1 * rs12 + b2 * rs + 1.5 * b3 * rs32 + 2 * b4 * rs2)
-    vc = -2 * a * (1 + 2 / 3 * a1 * rs) * olog - 2 / 3 * a * (1 + a1 * rs) * dom / (om * (om + 1))
-    return ec, np.array([vc])
+    tt = tx**2 + Q**2
+    vc = ec - x * A / 6 * (2 / x - tx / X - 4 * b / tt -
+                           fx0 * (2 / (x - x0) - tx / X - 4 * (2 * x0 + b) / tt))
+    return ec, np.array([vc]), None
 
 
-def lda_c_pw_spin(n, zeta, a=(0.031091, 0.015545, 0.016887), fz0=1.709921, exc_only=False,
-                  **kwargs):
-    '''Perdew-Wang parametrization of the correlation functional (spin-polarized).
+def lda_c_vwn_spin(n, zeta, exc_only=False, **kwargs):
+    '''Vosko-Wilk-Nusair parametrization of the correlation functional (spin-polarized).
 
-    Corresponds to the functional with the label LDA_C_PW and ID 12 in Libxc.
-    Reference: Phys. Rev. B 45, 13244.
+    Corresponds to the functional with the label LDA_C_VWN and ID 7 in Libxc.
+    Reference: Phys. Rev. B 22, 3812.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Keyword Args:
-        a (tuple): Functional parameters.
-        fz0 (float): Functional parameter.
         exc_only (bool): Only calculate the exchange-correlation energy density.
 
     Returns:
-        tuple[ndarray, ndarray]: PW correlation energy density and potential.
+        tuple[ndarray, ndarray]: VWN correlation energy density and potential.
     '''
-    pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 * n**(-1 / 3)
-    zeta3 = zeta**3
-    zeta4 = zeta3 * zeta
-
-    def pw_fit(i):
-        '''Calculate correlation energies by Perdew-Wang approximation interpolation.
-
-        Args:
-            i (int): Index to choose unpolarized (0), polarized (1), or antiferromagnetic (2) fit.
-
-        Returns:
-            tuple[ndarray, ndarray]: PW fit and the derivative.
-        '''
-        a1 = (0.2137, 0.20548, 0.11125)
-        b1 = (7.5957, 14.1189, 10.357)
-        b2 = (3.5876, 6.1977, 3.6231)
-        b3 = (1.6382, 3.3662, 0.88026)
-        b4 = (0.49294, 0.62517, 0.49671)
-
-        rs12 = np.sqrt(rs)
-        rs32 = rs * rs12
-        rs2 = rs**2
-
-        om = 2 * a[i] * (b1[i] * rs12 + b2[i] * rs + b3[i] * rs32 + b4[i] * rs2)
-        olog = np.log(1 + 1 / om)
-        fit = -2 * a[i] * (1 + a1[i] * rs) * olog
-        if exc_only:
-            return fit, None
-
-        dom = 2 * a[i] * (0.5 * b1[i] * rs12 + b2[i] * rs + 1.5 * b3[i] * rs32 + 2 * b4[i] * rs2)
-        dfit = -2 * a[i] * (1 + 2 / 3 * a1[i] * rs) * olog - \
-            2 / 3 * a[i] * (1 + a1[i] * rs) * dom / (om * (om + 1))
-        return fit, dfit
-
-    ecU, vcU = pw_fit(0)  # Unpolarized
-    ecP, vcP = pw_fit(1)  # Polarized
-    ac, dac = pw_fit(2)   # Spin stiffness
+    A = (0.0310907, 0.01554535, -1 / (6 * np.pi**2))
+    b = (3.72744, 7.06042, 1.13107)
+    c = (12.9352, 18.0578, 13.0045)
+    x0 = (-0.10498, -0.325, -0.0047584)
+
+    ec0, vc0, _ = lda_c_vwn(n, A[0], b[0], c[0], x0[0], exc_only)  # Paramagnetic
+    ec1, vc1, _ = lda_c_vwn(n, A[1], b[1], c[1], x0[1], exc_only)  # Ferromagnetic
+    ac, dac, _ = lda_c_vwn(n, A[2], b[2], c[2], x0[2], exc_only)   # Spin stiffness
+
+    d2fzeta0 = 4 / 9 / (2**(1 / 3) - 1)
+    fzeta = 0.5 * ((1 + zeta)**(4 / 3) + (1 - zeta)**(4 / 3) - 2) / (2**(1 / 3) - 1)
+    zeta4 = zeta**4
+    fzetaz4 = fzeta * zeta4
+    De = ec1 - ec0 - ac / d2fzeta0
 
-    ac = -ac  # The PW spin interpolation parametrizes -ac instead of ac
-    fz = ((1 + zeta)**(4 / 3) + (1 - zeta)**(4 / 3) - 2) / (2**(4 / 3) - 2)
-
-    ec = ecU + ac * fz * (1 - zeta4) / fz0 + (ecP - ecU) * fz * zeta4
+    ec = ec0 + ac / d2fzeta0 * fzeta + De * fzetaz4
     if exc_only:
-        return ec, None
+        return ec, None, None
 
-    dac = -dac  # Also change the sign for the derivative
-    dfz = ((1 + zeta)**(1 / 3) - (1 - zeta)**(1 / 3)) * 4 / (3 * (2**(4 / 3) - 2))
-    factor1 = vcU + dac * fz * (1 - zeta4) / fz0 + (vcP - vcU) * fz * zeta4
-    factor2 = (ac / fz0 * (dfz * (1 - zeta4) - 4 * fz * zeta3) +
-               (ecP - ecU) * (dfz * zeta4 + 4 * fz * zeta3))
-
-    vcup = factor1 + factor2 * (1 - zeta)
-    vcdw = factor1 - factor2 * (1 + zeta)
-    return ec, np.array([vcup, vcdw])
+    dfzeta = 4 / 6 * ((1 + zeta)**(1 / 3) - (1 - zeta)**(1 / 3)) / (2**(1 / 3) - 1)
+    dec1 = vc0 + dac / d2fzeta0 * fzeta + (vc1 - vc0 - dac / d2fzeta0) * fzetaz4
+    dec2 = ac / d2fzeta0 * dfzeta + De * (4 * zeta**3 * fzeta + zeta4 * dfzeta)
+
+    vcup = dec1 + (1 - zeta) * dec2
+    vcdw = dec1 - (1 + zeta) * dec2
+    return ec, np.array([vcup, vcdw]), None
```

### Comparing `eminus-2.3.0/eminus/xc/lda_c_pw_mod.py` & `eminus-2.4.0/eminus/xc/lda_c_pw_mod.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Returns:
         tuple[ndarray, ndarray]: PW correlation energy density and potential.
     '''
-    return lda_c_pw(n, a=0.0310907, **kwargs)
+    return lda_c_pw(n, A=0.0310907, **kwargs)
 
 
 def lda_c_pw_mod_spin(n, zeta, **kwargs):
     '''Modified Perdew-Wang parametrization of the correlation functional (spin-polarized).
 
     Corresponds to the functional with the label LDA_C_PW_MOD and ID 13 in Libxc.
     Reference: Phys. Rev. B 45, 13244.
@@ -30,9 +30,9 @@
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Returns:
         tuple[ndarray, ndarray]: PW correlation energy density and potential.
     '''
-    return lda_c_pw_spin(n, zeta, a=(0.0310907, 0.01554535, 0.0168869),
-                         fz0=1.709920934161365617563962776245, **kwargs)
+    return lda_c_pw_spin(n, zeta, A=(0.0310907, 0.01554535, 0.0168869),
+                         fzeta0=1.709920934161365617563962776245, **kwargs)
```

### Comparing `eminus-2.3.0/eminus/xc/lda_c_vwn.py` & `eminus-2.4.0/eminus/xc/gga_c_chachiyo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,134 +1,132 @@
 #!/usr/bin/env python3
-'''Vosko-Wilk-Nusair LDA correlation.
+'''Chachiyo GGA correlation.
 
-Reference: Phys. Rev. B 22, 3812.
+Reference: Comput. Theor. Chem. 1172, 112669.
 '''
 import numpy as np
+from numpy.linalg import norm
 
+from .lda_c_chachiyo_mod import chachiyo_scaling_mod as weight_function
 
-def lda_c_vwn(n, exc_only=False, **kwargs):
-    '''Vosko-Wilk-Nusair parametrization of the correlation functional (spin-paired).
 
-    Corresponds to the functional with the label LDA_C_VWN and ID 7 in Libxc.
-    Reference: Phys. Rev. B 22, 3812.
+def gga_c_chachiyo(n, exc_only=False, dn_spin=None, **kwargs):
+    '''Chachiyo parametrization of the correlation functional (spin-paired).
+
+    Corresponds to the functional with the label GGA_C_CHACHIYO and ID 309 in Libxc.
+    Reference: Comput. Theor. Chem. 1172, 112669.
 
     Args:
         n (ndarray): Real-space electronic density.
 
     Keyword Args:
         exc_only (bool): Only calculate the exchange-correlation energy density.
+        dn_spin (ndarray): Real-space gradient of densities per spin channel.
 
     Returns:
-        tuple[ndarray, ndarray]: VWN correlation energy density and potential.
+        tuple[ndarray, ndarray, ndarray]: Chachiyo correlation energy density, potential and vsigma.
     '''
-    a = 0.0310907
-    b = 3.72744
-    c = 12.9352
-    x0 = -0.10498
-
-    pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 * n**(-1 / 3)
-
-    q = np.sqrt(4 * c - b * b)
-    f1 = 2 * b / q
-    f2 = b * x0 / (x0 * x0 + b * x0 + c)
-    f3 = 2 * (2 * x0 + b) / q
-    rs12 = np.sqrt(rs)
-    fx = rs + b * rs12 + c
-    qx = np.arctan(q / (2 * rs12 + b))
+    h = 0.06672632  # 0.5 * 0.00847 * 16 * (3 / np.pi)**(1 / 3)
 
-    ec = a * (np.log(rs / fx) + f1 * qx - f2 * (np.log((rs12 - x0)**2 / fx) + f3 * qx))
+    # ### Start lda_c_chachiyo_mod ### #
+    a = -0.01554535  # (np.log(2) - 1) / (2 * np.pi**2)
+    b = 20.4562557
+
+    rs = (3 / (4 * np.pi * n))**(1 / 3)
+    rs2 = rs**2
+    ecinner = 1 + b / rs + b / rs2
+
+    ec = a * np.log(ecinner)
+    # ### End lda_c_chachiyo_mod ### #
+
+    norm_dn = norm(dn_spin[0], axis=1)
+    t = (np.pi / 3)**(1 / 6) / 4 * norm_dn / n**(7 / 6)
+    t2 = t**2
+    gec = 1 + t2
+    expgec = gec**(h / ec)
     if exc_only:
-        return ec, None
+        return ec * expgec, None, None
+
+    # ### Start lda_c_chachiyo_mod ### #
+    vc = ec + a * b * (2 + rs) / (3 * (b + b * rs + rs2))
+    # ### End lda_c_chachiyo_mod ### #
+
+    term1 = h * (1 - 1 / gec)
+    term2 = h * np.log(gec) * (1 - vc / ec)
+    gvc = (vc - 7 / 3 * term1 + term2) * expgec
 
-    tx = 2 * rs12 + b
-    tt = tx * tx + q * q
-    vc = ec - rs12 * a / 6 * (2 / rs12 - tx / fx - 4 * b / tt -
-                              f2 * (2 / (rs12 - x0) - tx / fx - 4 * (2 * x0 + b) / tt))
-    return ec, np.array([vc])
+    vsigmac = n * expgec * term1 / norm_dn**2
+    return ec * expgec, np.array([gvc]), np.array([vsigmac])
 
 
-def lda_c_vwn_spin(n, zeta, exc_only=False, **kwargs):
-    '''Vosko-Wilk-Nusair parametrization of the correlation functional (spin-polarized).
+def gga_c_chachiyo_spin(n, zeta, exc_only=False, dn_spin=None, **kwargs):
+    '''Chachiyo parametrization of the correlation functional (spin-polarized).
 
-    Corresponds to the functional with the label LDA_C_VWN and ID 7 in Libxc.
-    Reference: Phys. Rev. B 22, 3812.
+    Corresponds to the functional with the label GGA_C_CHACHIYO and ID 309 in Libxc.
+    Reference: Comput. Theor. Chem. 1172, 112669.
 
     Args:
         n (ndarray): Real-space electronic density.
         zeta (ndarray): Relative spin polarization.
 
     Keyword Args:
         exc_only (bool): Only calculate the exchange-correlation energy density.
+        dn_spin (ndarray): Real-space gradient of densities per spin channel.
 
     Returns:
-        tuple[ndarray, ndarray]: VWN correlation energy density and potential.
+        tuple[ndarray, ndarray, ndarray]: Chachiyo correlation energy density, potential and vsigma.
     '''
-    pi34 = (3 / (4 * np.pi))**(1 / 3)
-    rs = pi34 * n**(-1 / 3)
-    zeta4 = zeta**4
-
-    cfz = 2**(4 / 3) - 2
-    iddfz0 = 9 / 8 * cfz
-    trup = 1 + zeta
-    trdw = 1 - zeta
-    trup13 = trup**(1 / 3)
-    trdw13 = trdw**(1 / 3)
-
-    def pade_fit(i):
-        '''Calculate correlation energies by Pade approximation interpolation.
-
-        Args:
-            i (int): Index to choose paramagnetic (0), ferromagnetic (1), or spin stiffness (2) fit.
-
-        Returns:
-            tuple[ndarray, ndarray]: Pade fit and the derivative.
-        '''
-        a = (0.0310907, 0.01554535, -0.01688686394039)
-        b = (3.72744, 7.06042, 1.13107)
-        c = (12.9352, 18.0578, 13.0045)
-        x0 = (-0.10498, -0.325, -0.0047584)
-        Q = (6.15199081975908, 4.73092690956011, 7.12310891781812)
-        tbQ = (1.21178334272806, 2.98479352354082, 0.31757762321188)
-        bx0fx0 = (-0.03116760867894, -0.14460061018521, -0.00041403379428)
-
-        sqrtrs = np.sqrt(rs)
-
-        xx0 = sqrtrs - x0[i]
-        Qtxb = Q[i] / (2 * sqrtrs + b[i])
-        atg = np.arctan(Qtxb)
-        fx = rs + b[i] * sqrtrs + c[i]
-        fit = a[i] * (np.log(rs / fx) + tbQ[i] * atg -
-                      bx0fx0[i] * (np.log(xx0 * xx0 / fx) + (tbQ[i] + 4 * x0[i] / Q[i]) * atg))
-        if exc_only:
-            return fit, None
-
-        txb = 2 * sqrtrs + b[i]
-        txbfx = txb / fx
-        itxbQ = 1 / (txb * txb + Q[i] * Q[i])
-        dfit = fit - a[i] / 3 + \
-            a[i] * sqrtrs / 6 * (txbfx + 4 * b[i] * itxbQ + bx0fx0[i] *
-                                 (2 / xx0 - txbfx - 4 * (b[i] + 2 * x0[i]) * itxbQ))
-        return fit, dfit
-
-    ecP, vcP = pade_fit(0)  # Paramagnetic fit
-    ecF, vcF = pade_fit(1)  # Ferromagnetic fit
-    ac, dac = pade_fit(2)   # Spin stiffness
-
-    fz = (trup13 * trup + trdw13 * trdw - 2) / cfz  # f(zeta)
-    ac *= iddfz0
-    De = ecF - ecP - ac  # e_c[F] - e_c[P] - alpha_c/(ddf/ddz(z=0))
-    fzz4 = fz * zeta4
+    h = 0.06672632  # 0.5 * 0.00847 * 16 * (3 / np.pi)**(1 / 3)
 
-    ec = ecP + ac * fz + De * fzz4
+    # ### Start lda_c_chachiyo_spin_mod ### #
+    a0 = -0.01554535   # (np.log(2) - 1) / (2 * np.pi**2)
+    a1 = -0.007772675  # (np.log(2) - 1) / (4 * np.pi**2)
+    b0 = 20.4562557
+    b1 = 27.4203609
+
+    rs = (3 / (4 * np.pi * n))**(1 / 3)
+    rs2 = rs**2
+
+    fzeta, dfdzeta = weight_function(zeta, exc_only=exc_only)
+
+    ec0inner = 1 + b0 / rs + b0 / rs2
+    ec1inner = 1 + b1 / rs + b1 / rs2
+    ec0 = a0 * np.log(ec0inner)
+    ec1 = a1 * np.log(ec1inner)
+
+    ec = ec0 + (ec1 - ec0) * fzeta
+    # ### End lda_c_chachiyo_spin_mod ### #
+
+    norm_dn = norm(dn_spin[0] + dn_spin[1], axis=1)
+    t = (np.pi / 3)**(1 / 6) / 4 * norm_dn / n**(7 / 6)
+    t2 = t**2
+    gec = 1 + t2
+    expgec = gec**(h / ec)
     if exc_only:
-        return ec, None
+        return ec * expgec, None, None
 
-    dfz = 4 / 3 * (trup13 - trdw13) / cfz  # df/dzeta
-    dac *= iddfz0
-    dec1 = vcP + dac * fz + (vcF - vcP - dac) * fzz4  # e_c-(r_s/3)*(de_c/dr_s)
-    dec2 = ac * dfz + De * (4 * zeta**3 * fz + zeta4 * dfz)  # de_c/dzeta
-
-    vcup = dec1 + (1 - zeta) * dec2
-    vcdw = dec1 - (1 + zeta) * dec2
-    return ec, np.array([vcup, vcdw])
+    # ### Start lda_c_chachiyo_spin_mod ### #
+    factor = -1 / rs2 - 2 / rs**3
+    dec0drs = a0 / ec0inner * b0 * factor
+    dec1drs = a1 / ec1inner * b1 * factor
+    decdrs = dec0drs + (dec1drs - dec0drs) * fzeta
+    # prefactor = ec - rs / 3 * decdrs
+    decdf = (ec1 - ec0) * dfdzeta
+
+    # vcup = prefactor + decdf * (1 - zeta)
+    # vcdw = prefactor - decdf * (1 + zeta)
+    # ### End lda_c_chachiyo_spin_mod ### #
+
+    dn2 = norm(dn_spin[0], axis=1)**2 + \
+        2 * np.sum(dn_spin[0] * dn_spin[1], axis=1) + \
+        norm(dn_spin[1], axis=1)**2
+    ht2divgecdn2 = (1 - 1 / gec) * h / norm_dn**2
+    term1 = -7 / 3 * ht2divgecdn2 * dn2
+    term2 = 1 - h * np.log(gec) / ec
+    prefactor = -decdrs * rs / 3
+    gvc = ec + term1 + term2 * prefactor
+    gvcup = gvc + term2 * decdf * (1 - zeta)
+    gvcdw = gvc - term2 * decdf * (1 + zeta)
+
+    vsigma = n * expgec * 2 * ht2divgecdn2
+    vsigmac = np.array([0.5 * vsigma, vsigma, 0.5 * vsigma])
+    return ec * expgec, np.array([gvcup, gvcdw]) * expgec, vsigmac
```

### Comparing `eminus-2.3.0/eminus/xc/lda_x.py` & `eminus-2.4.0/eminus/xc/lda_x.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,24 +17,23 @@
 
     Keyword Args:
         exc_only (bool): Only calculate the exchange-correlation energy density.
 
     Returns:
         tuple[ndarray, ndarray]: Exchange energy density and potential.
     '''
-    pi34 = (3 / (4 * np.pi))**(1 / 3)
     f = -3 / 4 * (3 / (2 * np.pi))**(2 / 3)
-    rs = pi34 * n**(-1 / 3)
+    rs = (3 / (4 * np.pi * n))**(1 / 3)
 
     ex = f / rs
     if exc_only:
-        return ex, None
+        return ex, None, None
 
     vx = 4 / 3 * ex
-    return ex, np.array([vx])
+    return ex, np.array([vx]), None
 
 
 def lda_x_spin(n, zeta, exc_only=False, **kwargs):
     '''Slater exchange functional (spin-polarized).
 
     Corresponds to the functional with the label LDA_X and ID 1 in Libxc.
     Reference: Phys. Rev. 81, 385.
@@ -54,12 +53,12 @@
     rho13p = ((1 + zeta) * n)**(1 / 3)
     rho13m = ((1 - zeta) * n)**(1 / 3)
 
     exup = f * rho13p
     exdw = f * rho13m
     ex = 0.5 * ((1 + zeta) * exup + (1 - zeta) * exdw)
     if exc_only:
-        return ex, None
+        return ex, None, None
 
-    vxup = 4 / 3 * f * rho13p
-    vxdw = 4 / 3 * f * rho13m
-    return ex, np.array([vxup, vxdw])
+    vxup = 4 / 3 * exup
+    vxdw = 4 / 3 * exdw
+    return ex, np.array([vxup, vxdw]), None
```

### Comparing `eminus-2.3.0/eminus/xc/utils.py` & `eminus-2.4.0/eminus/xc/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 #!/usr/bin/env python3
 '''Utility functions for exchange-correlation functionals.'''
 import numpy as np
 
+from .gga_c_chachiyo import gga_c_chachiyo, gga_c_chachiyo_spin
+from .gga_c_pbe import gga_c_pbe, gga_c_pbe_spin
+from .gga_c_pbe_sol import gga_c_pbe_sol, gga_c_pbe_sol_spin
+from .gga_x_chachiyo import gga_x_chachiyo, gga_x_chachiyo_spin
+from .gga_x_pbe import gga_x_pbe, gga_x_pbe_spin
+from .gga_x_pbe_sol import gga_x_pbe_sol, gga_x_pbe_sol_spin
 from .lda_c_chachiyo import lda_c_chachiyo, lda_c_chachiyo_spin
 from .lda_c_chachiyo_mod import lda_c_chachiyo_mod, lda_c_chachiyo_mod_spin
 from .lda_c_pw import lda_c_pw, lda_c_pw_spin
 from .lda_c_pw_mod import lda_c_pw_mod, lda_c_pw_mod_spin
 from .lda_c_vwn import lda_c_vwn, lda_c_vwn_spin
 from .lda_x import lda_x, lda_x_spin
 from ..logger import log
 
 
-def get_xc(xc, n_spin, Nspin, dens_threshold=0, exc_only=False):
+def get_xc(xc, n_spin, Nspin, dn_spin=None, dens_threshold=0, exc_only=False):
     '''Handle and get exchange-correlation functionals.
 
     Args:
         xc (list | str): Exchange and correlation identifier.
         n_spin (ndarray): Real-space electronic densities per spin channel.
         Nspin (int): Number of spin states.
 
     Keyword Args:
+        dn_spin (ndarray): Real-space gradient of densities per spin channel.
         dens_threshold (float): Do not treat densities smaller than the threshold.
         exc_only (bool): Only calculate the exchange-correlation energy density.
 
     Returns:
         tuple[ndarray, ndarray]: Exchange-correlation energy density and potential.
     '''
     if isinstance(xc, str):
@@ -32,108 +39,173 @@
 
     # Only use non-zero values of the density
     n = np.sum(n_spin, axis=0)
     nz_mask = np.where(n > dens_threshold)
     n_nz = n[nz_mask]
     # Zeta is only needed for non-zero values of the density
     zeta_nz = get_zeta(n_spin[:, nz_mask])
+    # dn_spin is only needed for non-zero values of the density
+    if dn_spin is not None:
+        dn_spin_nz = dn_spin[:, nz_mask[0], :]
+    else:
+        dn_spin_nz = None
 
     # Only import libxc interface if necessary
-    if 'libxc' in str(xc):
+    if ':' in str(xc):
         from ..extras.libxc import libxc_functional
 
     # Handle exchange part
-    if 'libxc' in f_exch:
-        f_exch = f_exch.split(':')[1]
-        ex, vx = libxc_functional(f_exch, n_spin, Nspin)
+    if ':' in f_exch:
+        f_exch = f_exch.split(':')[-1]
+        ex, vx, vsigmax = libxc_functional(f_exch, n_spin, Nspin, dn_spin)
     else:
         if Nspin == 2 and f_exch != 'mock_xc':
             f_exch += '_spin'
-        ex_nz, vx_nz = IMPLEMENTED[f_exch](n_nz, zeta=zeta_nz, Nspin=Nspin, exc_only=exc_only)
+        ex_nz, vx_nz, vsigmax_nz = IMPLEMENTED[f_exch](n_nz, zeta=zeta_nz, Nspin=Nspin,
+                                                       exc_only=exc_only, dn_spin=dn_spin_nz)
         # Map the non-zero values back to the right dimension
         ex = np.zeros_like(n)
         ex[nz_mask] = ex_nz
-        vx = np.zeros_like(n_spin)
+        # Only map vx and vsigmax if necessary
         if not exc_only:
-            for spin in range(Nspin):
-                vx[spin, nz_mask] = vx_nz[spin]
+            vx = np.zeros_like(n_spin)
+            for s in range(Nspin):
+                vx[s, nz_mask] = vx_nz[s]
+            if vsigmax_nz is not None:
+                vsigmax = np.zeros((len(vsigmax_nz), len(ex)))
+                for i in range(len(vsigmax)):
+                    vsigmax[i, nz_mask] = vsigmax_nz[i]
+            else:
+                vsigmax = None
 
     # Handle correlation part
-    if 'libxc' in f_corr:
-        f_corr = f_corr.split(':')[1]
-        ec, vc = libxc_functional(f_corr, n_spin, Nspin)
+    if ':' in f_corr:
+        f_corr = f_corr.split(':')[-1]
+        ec, vc, vsigmac = libxc_functional(f_corr, n_spin, Nspin, dn_spin)
     else:
         if Nspin == 2 and f_corr != 'mock_xc':
             f_corr += '_spin'
-        ec_nz, vc_nz = IMPLEMENTED[f_corr](n_nz, zeta=zeta_nz, Nspin=Nspin, exc_only=exc_only)
+        ec_nz, vc_nz, vsigmac_nz = IMPLEMENTED[f_corr](n_nz, zeta=zeta_nz, Nspin=Nspin,
+                                                       exc_only=exc_only, dn_spin=dn_spin_nz)
         # Map the non-zero values back to the right dimension
         ec = np.zeros_like(n)
         ec[nz_mask] = ec_nz
-        vc = np.zeros_like(n_spin)
+        # Only map vc and vsigmac if necessary
         if not exc_only:
-            for spin in range(Nspin):
-                vc[spin, nz_mask] = vc_nz[spin]
-
-    return ex + ec, vx + vc
+            vc = np.zeros_like(n_spin)
+            for s in range(Nspin):
+                vc[s, nz_mask] = vc_nz[s]
+            if vsigmac_nz is not None:
+                vsigmac = np.zeros((len(vsigmac_nz), len(ex)))
+                for i in range(len(vsigmac)):
+                    vsigmac[i, nz_mask] = vsigmac_nz[i]
+            else:
+                vsigmac = None
+
+    if exc_only:
+        return ex + ec, None, None
+    # We can not add Nones or None and array together, so do this ugly case check
+    if vsigmax is None and vsigmac is None:
+        return ex + ec, vx + vc, None
+    if vsigmax is None:
+        return ex + ec, vx + vc, vsigmac
+    if vsigmac is None:
+        return ex + ec, vx + vc, vsigmax
+    return ex + ec, vx + vc, vsigmax + vsigmac
 
 
 def get_exc(*args, **kwargs):
     '''Get the exchange-correlation energy density.
 
     This is a convenience function to interface :func:`~eminus.xc.utils.get_xc`.
     '''
-    exc, _ = get_xc(*args, **kwargs, exc_only=True)
+    exc, _, _ = get_xc(*args, **kwargs, exc_only=True)
     return exc
 
 
 def get_vxc(*args, **kwargs):
     '''Get the exchange-correlation potential.
 
     This is a convenience function to interface :func:`~eminus.xc.utils.get_xc`.
     '''
-    _, vxc = get_xc(*args, **kwargs)
-    return vxc
+    _, vxc, vsigma = get_xc(*args, **kwargs)
+    return vxc, vsigma
 
 
 def parse_functionals(xc):
     '''Parse exchange-correlation functional strings to the internal format.
 
     Args:
         xc (str): Exchange and correlation identifier, separated by a comma.
 
     Returns:
         list: Exchange and correlation string.
     '''
     # Check for combined aliases
     try:
-        xc = ALIAS[xc]
+        # Remove underscores when looking up in the dictionary
+        xc_ = xc.replace('_', '')
+        xc = ALIAS[xc_]
     except KeyError:
         pass
 
     # Parse functionals
     functionals = []
     for f in xc.split(','):
-        if 'libxc' in f or f in IMPLEMENTED:
+        if ':' in f or f in IMPLEMENTED:
             f_xc = f
-        elif f == '':
+        elif not f:
             f_xc = 'mock_xc'
         else:
             try:
-                f_xc = XC_MAP[f]
+                # Remove underscores when looking up in the dictionary
+                f_ = f.replace('_', '')
+                f_xc = XC_MAP[f_]
             except KeyError:
                 log.exception(f'No functional found for "{f}"')
                 raise
         functionals.append(f_xc)
 
     # If only one or no functional has been parsed append with mock functionals
     for _ in range(2 - len(functionals)):
         functionals.append('mock_xc')
     return functionals
 
 
+def parse_psp(xc):
+    '''Parse functional strings to identify the corresponding pseudopotential.
+
+    Args:
+        xc (list): Exchange and correlation identifier, separated by a comma.
+
+    Returns:
+        str: Pseudopotential type.
+    '''
+    xc_type = []
+    for func in xc:
+        if ':' in func:
+            from pyscf.dft.libxc import is_gga, is_hybrid_xc, is_meta_gga
+            if is_meta_gga(func.split(':')[-1]) or is_hybrid_xc(func.split(':')[-1]):
+                log.exception('meta-GGA and hybrid functionals are not implemented.')
+                raise
+            elif is_gga(func.split(':')[-1]):
+                xc_type.append('pbe')
+            else:
+                xc_type.append('pade')
+        elif 'gga' in func:
+            xc_type.append('pbe')
+        else:
+            xc_type.append('pade')
+    # When mixing functional types use the higher level of theory
+    if xc_type[0] != xc_type[1]:
+        log.warning('Found mixing of LDA and GGA functionals.')
+        return 'pbe'
+    return xc_type[0]
+
+
 def get_zeta(n_spin):
     '''Calculate the relative spin polarization.
 
     Args:
         n_spin (ndarray): Real-space electronic densities per spin channel.
 
     Returns:
@@ -152,19 +224,31 @@
         n (ndarray): Real-space electronic density.
         Nspin (int): Number of spin states.
 
     Returns:
         tuple[ndarray, ndarray]: Mock exchange-correlation energy density and potential.
     '''
     zeros = np.zeros_like(n)
-    return zeros, np.array([zeros] * Nspin)
+    return zeros, np.array([zeros] * Nspin), None
 
 
 IMPLEMENTED = {
     'mock_xc': mock_xc,
+    'gga_c_chachiyo': gga_c_chachiyo,
+    'gga_c_chachiyo_spin': gga_c_chachiyo_spin,
+    'gga_c_pbe': gga_c_pbe,
+    'gga_c_pbe_spin': gga_c_pbe_spin,
+    'gga_c_pbe_sol': gga_c_pbe_sol,
+    'gga_c_pbe_sol_spin': gga_c_pbe_sol_spin,
+    'gga_x_chachiyo': gga_x_chachiyo,
+    'gga_x_chachiyo_spin': gga_x_chachiyo_spin,
+    'gga_x_pbe': gga_x_pbe,
+    'gga_x_pbe_spin': gga_x_pbe_spin,
+    'gga_x_pbe_sol': gga_x_pbe_sol,
+    'gga_x_pbe_sol_spin': gga_x_pbe_sol_spin,
     'lda_x': lda_x,
     'lda_x_spin': lda_x_spin,
     'lda_c_pw': lda_c_pw,
     'lda_c_pw_spin': lda_c_pw_spin,
     'lda_c_pw_mod': lda_c_pw_mod,
     'lda_c_pw_mod_spin': lda_c_pw_mod_spin,
     'lda_c_vwn': lda_c_vwn,
@@ -187,22 +271,43 @@
     'vwn5': 'lda_c_vwn',
     # lda_c_pw
     '12': 'lda_c_pw',
     'pw': 'lda_c_pw',
     'pw92': 'lda_c_pw',
     # lda_c_pw_mod
     '13': 'lda_c_pw_mod',
-    'pw_mod': 'lda_c_pw_mod',
-    'pw92_mod': 'lda_c_pw_mod',
+    'pwmod': 'lda_c_pw_mod',
+    'pw92mod': 'lda_c_pw_mod',
+    # gga_x_pbe
+    '101': 'gga_x_pbe',
+    'pbex': 'gga_x_pbe',
+    # gga_x_pbe_sol
+    '116': 'gga_x_pbe_sol',
+    'pbesolx': 'gga_x_pbe_sol',
+    # gga_c_pbe
+    '130': 'gga_c_pbe',
+    'pbec': 'gga_c_pbe',
+    # gga_c_pbe_sol
+    '133': 'gga_c_pbe_sol',
+    'pbesolc': 'gga_c_pbe_sol',
     # lda_c_chachiyo
     '287': 'lda_c_chachiyo',
     'chachiyo': 'lda_c_chachiyo',
+    # gga_x_chachiyo
+    '298': 'gga_x_chachiyo',
+    'chachiyox': 'gga_x_chachiyo',
     # lda_c_chachiyo_mod
     '307': 'lda_c_chachiyo_mod',
-    'chachiyo_mod': 'lda_c_chachiyo_mod'
+    'chachiyomod': 'lda_c_chachiyo_mod',
+    # gga_c_chachiyo
+    '309': 'gga_c_chachiyo',
+    'chachiyoc': 'gga_c_chachiyo'
 }
 
 ALIAS = {
-    'spw92': 'slater,pw92_mod',
+    'spw92': 'slater,pw92mod',
     'svwn': 'slater,vwn5',
-    'svwn5': 'slater,vwn5'
+    'svwn5': 'slater,vwn5',
+    'pbe': 'pbex,pbec',
+    'pbesol': 'pbesolx,pbesolc',
+    'chachiyo': 'chachiyox,chachiyoc'
 }
```

### Comparing `eminus-2.3.0/eminus.egg-info/PKG-INFO` & `eminus-2.4.0/eminus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eminus
-Version: 2.3.0
+Version: 2.4.0
 Summary: A plane wave density functional theory code.
 Home-page: https://github.com/wangenau/eminus
 Author: Wanja Timm Schulze
 Author-email: wangenau@protonmail.com
 License: APACHE2.0
 Project-URL: Bug Tracker, https://gitlab.com/wangenau/eminus/-/issues
 Project-URL: Changelog, https://wangenau.gitlab.io/eminus/changelog.html
@@ -74,22 +74,19 @@
 
 This project is licensed under the Apache 2.0 License - see the [LICENSE](https://gitlab.com/wangenau/eminus/-/blob/main/LICENSE) file for details.
 
 
 Changelog
 =========
 
-v2.3.0 - May 02, 2023
+v2.4.0 - May 23, 2023
 ---------------------
 - New features
-   - Add Torch powered FFT operators as an extra
-      - Up to 20% faster calculations
-   - Add a consolidated configuration class
-      - Easier configuration and more performance infos
-   - Add a complete test suite
-      - Add CI/CD coverage reports
-   - Nix developer shell support
+   - Add GGA functionals!
+      - Add internal PBE, PBEsol, and Chachiyo functionals
+      - Option to use all GGAs from Libxc using pylibxc or PySCF
 - Miscellaneous
-   - Rewritten FODs guess function
-   - Simplify the FOD interface in io and viewer
-   - Fix a plethora of small bugs
-   - Update Docker image to Python 3.11
+   - Add Thomas-Fermi and von Weizsäcker kinetic energy density functions
+   - Rewrite functionals for better readability
+   - Fix Torch operators in some edge cases
+   - Merge configuration files in tox.ini
+   - Update minimum versions of dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eminus-2.3.0/setup.py` & `eminus-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
     version = re.search(r"__version__ = '(.*?)'", fh.read()).group(1)
 
 with open('README.md', 'r') as readme, open('CHANGELOG.md', 'r') as changelog:
     long_description = readme.read() + '\n\n' + changelog.read().split('\n----\n')[0]
 
 extras = {
     'libxc': [
-        'pyscf>=1.5.1'  # Libxc interface via PySCF
+        'pyscf>=1.7.3'  # Libxc interface via PySCF
     ],
     'torch': [
         'torch>=1.8'  # Faster FFT operators using Torch
     ],
     'viewer': [
         'nglview>=2.6.5',  # Molecule and isosurface viewer
-        'plotly>=4'        # Grid visualization
+        'plotly>=4.5'      # Grid visualization
     ]
 }
 extras['fods'] = extras['libxc']  # PyCOM FOD guessing method uses PySCF
 extras['all'] = [dep for values in extras.values() for dep in values]
 extras['dev'] = [
-    'coverage>=3.6',             # Generate coverage reports
+    'coverage>=4.4',             # Generate coverage reports
     'flake8>=3.7',               # Style guide checker
     'flake8-docstrings>=1.4',    # Docstring style guide extension
     'flake8-import-order>=0.9',  # Import statement style guide extension
     'furo>=2022.02.14.1',        # Documentation theme
     'notebook',                  # Run and convert notebooks to HTML
-    'pytest>=2.8',               # Test utilities
-    'pytest-cov>=0.6',           # Collect test coverage data
-    'sphinx>=5'                  # Documentation builder
+    'pytest>=5.4',               # Test utilities
+    'pytest-cov>=2.6.1',         # Collect test coverage data
+    'sphinx>=4'                  # Documentation builder
 ]
 
 setup(
     name='eminus',
     version=version,
     description='A plane wave density functional theory code.',
     long_description=long_description,
```

