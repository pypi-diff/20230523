# Comparing `tmp/spherical-functions-2022.4.1.tar.gz` & `tmp/spherical_functions-2022.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spherical-functions-2022.4.1.tar", max compression
+gzip compressed data, was "spherical_functions-2022.4.2.tar", max compression
```

## Comparing `spherical-functions-2022.4.1.tar` & `spherical_functions-2022.4.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1078 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/LICENSE
--rw-r--r--   0        0        0     7446 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/README.md
--rw-r--r--   0        0        0     1054 2022-04-01 16:14:56.563004 spherical-functions-2022.4.1/pyproject.toml
--rw-r--r--   0        0        0    13720 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH/__init__.py
--rw-r--r--   0        0        0     6639 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH_grids/__init__.py
--rw-r--r--   0        0        0     6756 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH_grids/algebra.py
--rw-r--r--   0        0        0     9059 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH_grids/ufuncs.py
--rw-r--r--   0        0        0     2746 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH_grids/utilities.py
--rw-r--r--   0        0        0     9513 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH_modes/__init__.py
--rw-r--r--   0        0        0    11783 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH_modes/algebra.py
--rw-r--r--   0        0        0    14859 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH_modes/derivatives.py
--rw-r--r--   0        0        0     9154 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH_modes/ufuncs.py
--rw-r--r--   0        0        0     5237 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/SWSH_modes/utilities.py
--rw-r--r--   0        0        0    17712 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/WignerD/WignerDRecursion.py
--rw-r--r--   0        0        0    30163 2022-04-01 16:13:40.445537 spherical-functions-2022.4.1/spherical_functions/WignerD/__init__.py
--rw-r--r--   0        0        0   749400 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/Wigner_coefficients.npy
--rw-r--r--   0        0        0    11312 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/__init__.py
--rw-r--r--   0        0        0     2537 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/_generate_coefficients.py
--rw-r--r--   0        0        0    17240 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/binomial_coefficients.npy
--rw-r--r--   0        0        0    17240 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/ladder_operator_coefficients.npy
--rw-r--r--   0        0        0     9583 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/mode_conversions.py
--rw-r--r--   0        0        0     4410 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/multiplication.py
--rw-r--r--   0        0        0     4995 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/recursions/__init__.py
--rw-r--r--   0        0        0     3328 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/recursions/associated_legendre_functions.py
--rw-r--r--   0        0        0     2743 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/recursions/complex_powers.py
--rw-r--r--   0        0        0    14029 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/recursions/wigner3j.py
--rw-r--r--   0        0        0    19158 2022-04-01 16:13:40.449537 spherical-functions-2022.4.1/spherical_functions/recursions/wignerH.py
--rw-r--r--   0        0        0     8643 2022-04-01 16:14:58.671704 spherical-functions-2022.4.1/setup.py
--rw-r--r--   0        0        0     8250 2022-04-01 16:14:58.672312 spherical-functions-2022.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-23 04:37:19.383263 spherical_functions-2022.4.2/LICENSE
+-rw-r--r--   0        0        0     6895 2023-05-23 04:37:19.383263 spherical_functions-2022.4.2/README.md
+-rw-r--r--   0        0        0     1055 2023-05-23 04:37:54.934874 spherical_functions-2022.4.2/pyproject.toml
+-rw-r--r--   0        0        0    13720 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH/__init__.py
+-rw-r--r--   0        0        0     6639 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH_grids/__init__.py
+-rw-r--r--   0        0        0     6756 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH_grids/algebra.py
+-rw-r--r--   0        0        0     9059 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH_grids/ufuncs.py
+-rw-r--r--   0        0        0     2746 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH_grids/utilities.py
+-rw-r--r--   0        0        0     9513 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH_modes/__init__.py
+-rw-r--r--   0        0        0    11783 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH_modes/algebra.py
+-rw-r--r--   0        0        0    14859 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH_modes/derivatives.py
+-rw-r--r--   0        0        0     9154 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH_modes/ufuncs.py
+-rw-r--r--   0        0        0     5237 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/SWSH_modes/utilities.py
+-rw-r--r--   0        0        0    17712 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/WignerD/WignerDRecursion.py
+-rw-r--r--   0        0        0    30163 2023-05-23 04:37:19.387260 spherical_functions-2022.4.2/spherical_functions/WignerD/__init__.py
+-rw-r--r--   0        0        0   749400 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/Wigner_coefficients.npy
+-rw-r--r--   0        0        0    11312 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/__init__.py
+-rw-r--r--   0        0        0     2537 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/_generate_coefficients.py
+-rw-r--r--   0        0        0    17240 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/binomial_coefficients.npy
+-rw-r--r--   0        0        0    17240 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/ladder_operator_coefficients.npy
+-rw-r--r--   0        0        0     9583 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/mode_conversions.py
+-rw-r--r--   0        0        0     4410 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/multiplication.py
+-rw-r--r--   0        0        0     4995 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/recursions/__init__.py
+-rw-r--r--   0        0        0     3328 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/recursions/associated_legendre_functions.py
+-rw-r--r--   0        0        0     2743 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/recursions/complex_powers.py
+-rw-r--r--   0        0        0    14029 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/recursions/wigner3j.py
+-rw-r--r--   0        0        0    19158 2023-05-23 04:37:19.391257 spherical_functions-2022.4.2/spherical_functions/recursions/wignerH.py
+-rw-r--r--   0        0        0     7744 1970-01-01 00:00:00.000000 spherical_functions-2022.4.2/PKG-INFO
```

### Comparing `spherical-functions-2022.4.1/LICENSE` & `spherical_functions-2022.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/README.md` & `spherical_functions-2022.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,466 +1,431 @@
-00000000: 2320 5370 6865 7269 6361 6c20 4675 6e63  # Spherical Func
-00000010: 7469 6f6e 7320 3c61 2068 7265 663d 2268  tions <a href="h
-00000020: 7474 7073 3a2f 2f74 7261 7669 732d 6369  ttps://travis-ci
-00000030: 2e6f 7267 2f6d 6f62 6c65 2f73 7068 6572  .org/moble/spher
-00000040: 6963 616c 5f66 756e 6374 696f 6e73 223e  ical_functions">
-00000050: 3c69 6d67 2061 6c69 676e 3d22 7269 6768  <img align="righ
-00000060: 7422 2068 7370 6163 653d 2233 2220 616c  t" hspace="3" al
-00000070: 743d 2253 7461 7475 7320 6f66 2061 7574  t="Status of aut
-00000080: 6f6d 6174 6963 2062 7569 6c64 2061 6e64  omatic build and
-00000090: 2074 6573 7420 7375 6974 6522 2073 7263   test suite" src
-000000a0: 3d22 6874 7470 733a 2f2f 7472 6176 6973  ="https://travis
-000000b0: 2d63 692e 6f72 672f 6d6f 626c 652f 7370  -ci.org/moble/sp
-000000c0: 6865 7269 6361 6c5f 6675 6e63 7469 6f6e  herical_function
-000000d0: 732e 7376 673f 6272 616e 6368 3d6d 6173  s.svg?branch=mas
-000000e0: 7465 7222 3e3c 2f61 3e20 3c61 2068 7265  ter"></a> <a hre
-000000f0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000100: 622e 636f 6d2f 6d6f 626c 652f 7370 6865  b.com/moble/sphe
-00000110: 7269 6361 6c5f 6675 6e63 7469 6f6e 732f  rical_functions/
-00000120: 626c 6f62 2f6d 6173 7465 722f 4c49 4345  blob/master/LICE
-00000130: 4e53 4522 3e3c 696d 6720 616c 6967 6e3d  NSE"><img align=
-00000140: 2272 6967 6874 2220 6873 7061 6365 3d22  "right" hspace="
-00000150: 3322 2061 6c74 3d22 4d49 5420 6c69 6365  3" alt="MIT lice
-00000160: 6e73 6522 2073 7263 3d22 6874 7470 733a  nse" src="https:
-00000170: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000180: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
-00000190: 6d6f 626c 652f 6f75 745f 6f66 5f63 6f72  moble/out_of_cor
-000001a0: 655f 6666 742e 7376 6722 3e3c 2f61 3e0a  e_fft.svg"></a>.
-000001b0: 0a7c 204e 4f54 453a 2054 6869 7320 7061  .| NOTE: This pa
-000001c0: 636b 6167 6520 7769 6c6c 2073 7469 6c6c  ckage will still
-000001d0: 2062 6520 6d61 696e 7461 696e 6564 2c20   be maintained, 
-000001e0: 6275 7420 2a61 6374 6976 652a 2064 6576  but *active* dev
-000001f0: 656c 6f70 6d65 6e74 2068 6173 206d 6f76  elopment has mov
-00000200: 6564 2074 6f20 7468 6520 5b60 7370 6865  ed to the [`sphe
-00000210: 7269 6361 6c60 5d28 6874 7470 733a 2f2f  rical`](https://
-00000220: 6769 7468 7562 2e63 6f6d 2f6d 6f62 6c65  github.com/moble
-00000230: 2f73 7068 6572 6963 616c 2920 7061 636b  /spherical) pack
-00000240: 6167 652e 2020 5768 696c 6520 7468 6973  age.  While this
-00000250: 2070 6163 6b61 6765 2077 6f72 6b73 2077   package works w
-00000260: 656c 6c20 666f 7220 e284 9320 2861 6b61  ell for ... (aka
-00000270: 2065 6c6c 2c20 4c2c 206a 2c20 6f72 204a   ell, L, j, or J
-00000280: 2920 7661 6c75 6573 2075 7020 746f 2061  ) values up to a
-00000290: 726f 756e 6420 3235 2c20 6572 726f 7273  round 25, errors
-000002a0: 2073 7461 7274 2074 6f20 6275 696c 6420   start to build 
-000002b0: 7261 7069 646c 7920 616e 6420 7475 726e  rapidly and turn
-000002c0: 2069 6e74 6f20 4e61 4e73 2061 726f 756e   into NaNs aroun
-000002d0: 6420 3330 2e20 2054 6865 2060 7370 6865  d 30.  The `sphe
-000002e0: 7269 6361 6c60 2070 6163 6b61 6765 2063  rical` package c
-000002f0: 616e 2072 6561 6469 6c79 2068 616e 646c  an readily handl
-00000300: 6520 7661 6c75 6573 2075 7020 746f 2061  e values up to a
-00000310: 7420 6c65 6173 7420 3130 3030 2c20 7769  t least 1000, wi
-00000320: 7468 2061 6363 7572 6163 7920 636c 6f73  th accuracy clos
-00000330: 6520 746f 20e2 8493 2074 696d 6573 206d  e to ... times m
-00000340: 6163 6869 6e65 2070 7265 6369 7369 6f6e  achine precision
-00000350: 2e20 20e2 8094 4d69 6b65 207c 0a7c 202d  .  ...Mike |.| -
-00000360: 2d2d 207c 0a0a 0a50 7974 686f 6e2f 6e75  -- |...Python/nu
-00000370: 6d62 6120 7061 636b 6167 6520 666f 7220  mba package for 
-00000380: 6576 616c 7561 7469 6e67 2061 6e64 2074  evaluating and t
-00000390: 7261 6e73 666f 726d 696e 6720 5769 676e  ransforming Wign
-000003a0: 6572 2773 20f0 9d94 8720 6d61 7472 6963  er's .... matric
-000003b0: 6573 2c0a 5769 676e 6572 2773 2033 2d6a  es,.Wigner's 3-j
-000003c0: 2073 796d 626f 6c73 2c20 616e 6420 7370   symbols, and sp
-000003d0: 696e 2d77 6569 6768 7465 6420 2861 6e64  in-weighted (and
-000003e0: 2073 6361 6c61 7229 2073 7068 6572 6963   scalar) spheric
-000003f0: 616c 2068 6172 6d6f 6e69 6373 2e0a 5468  al harmonics..Th
-00000400: 6573 6520 6675 6e63 7469 6f6e 7320 6172  ese functions ar
-00000410: 6520 6576 616c 7561 7465 6420 6469 7265  e evaluated dire
-00000420: 6374 6c79 2069 6e20 7465 726d 7320 6f66  ctly in terms of
-00000430: 2071 7561 7465 726e 696f 6e73 2c20 6173   quaternions, as
-00000440: 2077 656c 6c20 6173 2069 6e0a 7468 6520   well as in.the 
-00000450: 6d6f 7265 2073 7461 6e64 6172 6420 666f  more standard fo
-00000460: 726d 7320 6f66 2073 7068 6572 6963 616c  rms of spherical
-00000470: 2063 6f6f 7264 696e 6174 6573 2061 6e64   coordinates and
-00000480: 2045 756c 6572 0a61 6e67 6c65 732e 3c73   Euler.angles.<s
-00000490: 7570 3e5b 315d 2823 312d 6575 6c65 722d  up>[1](#1-euler-
-000004a0: 616e 676c 6573 2d61 7265 2d61 7766 756c  angles-are-awful
-000004b0: 293c 2f73 7570 3e0a 0a54 6865 2063 6f6e  )</sup>..The con
-000004c0: 7665 6e74 696f 6e73 2066 6f72 2074 6869  ventions for thi
-000004d0: 7320 7061 636b 6167 6520 6172 6520 6465  s package are de
-000004e0: 7363 7269 6265 6420 696e 2064 6574 6169  scribed in detai
-000004f0: 6c20 6f6e 0a5b 7468 6973 2070 6167 655d  l on.[this page]
-00000500: 2868 7474 703a 2f2f 6d6f 626c 652e 6769  (http://moble.gi
-00000510: 7468 7562 2e69 6f2f 7370 6865 7269 6361  thub.io/spherica
-00000520: 6c5f 6675 6e63 7469 6f6e 732f 292e 0a0a  l_functions/)...
-00000530: 2323 2044 6570 656e 6465 6e63 6965 730a  ## Dependencies.
-00000540: 0a54 6865 206f 6e6c 7920 7472 7565 2072  .The only true r
-00000550: 6571 7569 7265 6d65 6e74 7320 666f 7220  equirements for 
-00000560: 7468 6973 2063 6f64 6520 6172 6520 6070  this code are `p
-00000570: 7974 686f 6e60 2061 6e64 2074 6865 2070  ython` and the p
-00000580: 7974 686f 6e20 7061 636b 6167 650a 606e  ython package.`n
-00000590: 756d 7079 602c 2061 7320 7765 6c6c 2061  umpy`, as well a
-000005a0: 7320 6d79 2061 6363 6f6d 7061 6e79 696e  s my accompanyin
-000005b0: 670a 5b60 7175 6174 6572 6e69 6f6e 605d  g.[`quaternion`]
-000005c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000005d0: 636f 6d2f 6d6f 626c 652f 7175 6174 6572  com/moble/quater
-000005e0: 6e69 6f6e 2920 7061 636b 6167 6520 2869  nion) package (i
-000005f0: 6e73 7461 6c6c 6174 696f 6e20 6f66 0a77  nstallation of.w
-00000600: 6869 6368 2069 7320 7368 6f77 6e20 6265  hich is shown be
-00000610: 6c6f 7729 2e0a 0a48 6f77 6576 6572 2c20  low)...However, 
-00000620: 7468 6973 2070 6163 6b61 6765 2063 616e  this package can
-00000630: 2061 7574 6f6d 6174 6963 616c 6c79 2075   automatically u
-00000640: 7365 0a5b 606e 756d 6261 605d 2868 7474  se.[`numba`](htt
-00000650: 703a 2f2f 6e75 6d62 612e 7079 6461 7461  p://numba.pydata
-00000660: 2e6f 7267 2f29 2c20 7768 6963 6820 7573  .org/), which us
-00000670: 6573 205b 4c4c 564d 5d28 6874 7470 3a2f  es [LLVM](http:/
-00000680: 2f6c 6c76 6d2e 6f72 672f 2920 746f 0a63  /llvm.org/) to.c
-00000690: 6f6d 7069 6c65 2070 7974 686f 6e20 636f  ompile python co
-000006a0: 6465 2074 6f20 6d61 6368 696e 6520 636f  de to machine co
-000006b0: 6465 2c20 6163 6365 6c65 7261 7469 6e67  de, accelerating
-000006c0: 206d 6f73 7420 6e75 6d65 7269 6361 6c20   most numerical 
-000006d0: 6675 6e63 7469 6f6e 7320 6279 0a66 6163  functions by.fac
-000006e0: 746f 7273 206f 6620 616e 7977 6865 7265  tors of anywhere
-000006f0: 2066 726f 6d20 3220 746f 2032 3030 302e   from 2 to 2000.
-00000700: 2020 4974 2069 7320 2a70 6f73 7369 626c    It is *possibl
-00000710: 652a 2074 6f20 7275 6e20 7468 6520 636f  e* to run the co
-00000720: 6465 2077 6974 686f 7574 0a60 6e75 6d62  de without.`numb
-00000730: 6160 2c20 6275 7420 7468 6520 6d6f 7374  a`, but the most
-00000740: 2069 6d70 6f72 7461 6e74 2066 756e 6374   important funct
-00000750: 696f 6e73 2061 7265 2072 6f75 6768 6c79  ions are roughly
-00000760: 2031 3020 7469 6d65 7320 736c 6f77 6572   10 times slower
-00000770: 2077 6974 686f 7574 0a69 742e 0a0a 5468   without.it...Th
-00000780: 6520 6f6e 6c79 2064 7261 7762 6163 6b20  e only drawback 
-00000790: 6f66 2060 6e75 6d62 6160 2069 7320 7468  of `numba` is th
-000007a0: 6174 2069 7420 6973 206e 6f6e 7472 6976  at it is nontriv
-000007b0: 6961 6c20 746f 2069 6e73 7461 6c6c 206f  ial to install o
-000007c0: 6e20 6974 7320 6f77 6e2e 0a46 6f72 7475  n its own..Fortu
-000007d0: 6e61 7465 6c79 2c20 7468 6520 6265 7374  nately, the best
-000007e0: 2070 7974 686f 6e20 696e 7374 616c 6c65   python installe
-000007f0: 722c 0a5b 6061 6e61 636f 6e64 6160 5d28  r,.[`anaconda`](
-00000800: 6874 7470 3a2f 2f63 6f6e 7469 6e75 756d  http://continuum
-00000810: 2e69 6f2f 646f 776e 6c6f 6164 7329 2c20  .io/downloads), 
-00000820: 6d61 6b65 7320 6974 2074 7269 7669 616c  makes it trivial
-00000830: 2e20 204a 7573 7420 696e 7374 616c 6c0a  .  Just install.
-00000840: 7468 6520 6d61 696e 2060 616e 6163 6f6e  the main `anacon
-00000850: 6461 6020 7061 636b 6167 652e 0a0a 4966  da` package...If
-00000860: 2079 6f75 2070 7265 6665 7220 7468 6520   you prefer the 
-00000870: 736d 616c 6c65 7220 646f 776e 6c6f 6164  smaller download
-00000880: 2073 697a 6520 6f66 0a5b 606d 696e 6963   size of.[`minic
-00000890: 6f6e 6461 605d 2868 7474 703a 2f2f 636f  onda`](http://co
-000008a0: 6e64 612e 7079 6461 7461 2e6f 7267 2f6d  nda.pydata.org/m
-000008b0: 696e 6963 6f6e 6461 2e68 746d 6c29 2028  iniconda.html) (
-000008c0: 7768 6963 6820 636f 6d65 7320 7769 7468  which comes with
-000008d0: 206e 6f0a 6578 7472 6173 2062 6579 6f6e   no.extras beyon
-000008e0: 6420 7079 7468 6f6e 292c 2079 6f75 276c  d python), you'l
-000008f0: 6c20 616c 736f 2068 6176 6520 746f 2072  l also have to r
-00000900: 756e 2074 6869 7320 636f 6d6d 616e 643a  un this command:
-00000910: 0a0a 6060 6073 680a 636f 6e64 6120 696e  ..```sh.conda in
-00000920: 7374 616c 6c20 7069 7020 6e75 6d70 7920  stall pip numpy 
-00000930: 6e75 6d62 610a 6060 600a 0a0a 2323 2049  numba.```...## I
-00000940: 6e73 7461 6c6c 6174 696f 6e0a 0a41 7373  nstallation..Ass
-00000950: 756d 696e 6720 796f 7520 7573 6520 6063  uming you use `c
-00000960: 6f6e 6461 6020 746f 206d 616e 6167 6520  onda` to manage 
-00000970: 796f 7572 2070 7974 686f 6e20 696e 7374  your python inst
-00000980: 616c 6c61 7469 6f6e 2028 6c69 6b65 2061  allation (like a
-00000990: 6e79 2073 616e 650a 7079 7468 6f6e 2075  ny sane.python u
-000009a0: 7365 7229 2c20 796f 7520 6361 6e20 696e  ser), you can in
-000009b0: 7374 616c 6c20 7468 6973 2070 6163 6b61  stall this packa
-000009c0: 6765 2073 696d 706c 7920 6173 0a0a 6060  ge simply as..``
-000009d0: 6073 680a 636f 6e64 6120 696e 7374 616c  `sh.conda instal
-000009e0: 6c20 2d63 2063 6f6e 6461 2d66 6f72 6765  l -c conda-forge
-000009f0: 2073 7068 6572 6963 616c 5f66 756e 6374   spherical_funct
-00000a00: 696f 6e73 0a60 6060 0a0a 5468 6973 2073  ions.```..This s
-00000a10: 686f 756c 6420 6175 746f 6d61 7469 6361  hould automatica
-00000a20: 6c6c 7920 646f 776e 6c6f 6164 2061 6e64  lly download and
-00000a30: 2069 6e73 7461 6c6c 2074 6865 2070 6163   install the pac
-00000a40: 6b61 6765 0a5b 6071 7561 7465 726e 696f  kage.[`quaternio
-00000a50: 6e60 5d28 6874 7470 733a 2f2f 6769 7468  n`](https://gith
-00000a60: 7562 2e63 6f6d 2f6d 6f62 6c65 2f71 7561  ub.com/moble/qua
-00000a70: 7465 726e 696f 6e29 2c20 6f6e 2077 6869  ternion), on whi
-00000a80: 6368 2074 6869 7320 7061 636b 6167 650a  ch this package.
-00000a90: 6465 7065 6e64 732e 0a0a 416c 7465 726e  depends...Altern
-00000aa0: 6174 6976 656c 792c 2069 6620 796f 7520  atively, if you 
-00000ab0: 7072 6566 6572 2074 6f20 7573 6520 6070  prefer to use `p
-00000ac0: 6970 6020 2877 6865 7468 6572 206f 7220  ip` (whether or 
-00000ad0: 6e6f 7420 796f 7520 7573 6520 6063 6f6e  not you use `con
-00000ae0: 6461 6029 2c20 796f 750a 6361 6e20 616c  da`), you.can al
-00000af0: 736f 2064 6f0a 0a60 6060 7368 0a70 6970  so do..```sh.pip
-00000b00: 2069 6e73 7461 6c6c 2067 6974 2b67 6974   install git+git
-00000b10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d6f  ://github.com/mo
-00000b20: 626c 652f 7175 6174 6572 6e69 6f6e 0a70  ble/quaternion.p
-00000b30: 6970 2069 6e73 7461 6c6c 2067 6974 2b67  ip install git+g
-00000b40: 6974 3a2f 2f67 6974 6875 622e 636f 6d2f  it://github.com/
-00000b50: 6d6f 626c 652f 7370 6865 7269 6361 6c5f  moble/spherical_
-00000b60: 6675 6e63 7469 6f6e 730a 6060 600a 0a4f  functions.```..O
-00000b70: 722c 2069 6620 796f 7520 7265 6675 7365  r, if you refuse
-00000b80: 2074 6f20 7573 6520 6063 6f6e 6461 602c   to use `conda`,
-00000b90: 2079 6f75 206d 6967 6874 2077 616e 7420   you might want 
-00000ba0: 746f 2069 6e73 7461 6c6c 2069 6e73 6964  to install insid
-00000bb0: 6520 796f 7572 2068 6f6d 650a 6469 7265  e your home.dire
-00000bc0: 6374 6f72 7920 7769 7468 6f75 7420 726f  ctory without ro
-00000bd0: 6f74 2070 7269 7669 6c65 6765 732e 2020  ot privileges.  
-00000be0: 2841 6e61 636f 6e64 6120 646f 6573 2074  (Anaconda does t
-00000bf0: 6869 7320 6279 2064 6566 6175 6c74 2061  his by default a
-00000c00: 6e79 7761 792e 290a 5468 6973 2069 7320  nyway.).This is 
-00000c10: 646f 6e65 2062 7920 6164 6469 6e67 2060  done by adding `
-00000c20: 2d2d 7573 6572 6020 746f 2074 6865 2061  --user` to the a
-00000c30: 626f 7665 2063 6f6d 6d61 6e64 733a 0a0a  bove commands:..
-00000c40: 6060 6073 680a 7069 7020 696e 7374 616c  ```sh.pip instal
-00000c50: 6c20 2d2d 7573 6572 2067 6974 2b67 6974  l --user git+git
-00000c60: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d6f  ://github.com/mo
-00000c70: 626c 652f 7175 6174 6572 6e69 6f6e 0a70  ble/quaternion.p
-00000c80: 6970 2069 6e73 7461 6c6c 202d 2d75 7365  ip install --use
-00000c90: 7220 6769 742b 6769 743a 2f2f 6769 7468  r git+git://gith
-00000ca0: 7562 2e63 6f6d 2f6d 6f62 6c65 2f73 7068  ub.com/moble/sph
-00000cb0: 6572 6963 616c 5f66 756e 6374 696f 6e73  erical_functions
-00000cc0: 0a60 6060 0a0a 4669 6e61 6c6c 792c 2074  .```..Finally, t
-00000cd0: 6865 7265 2773 2061 6c73 6f20 7468 6520  here's also the 
-00000ce0: 6675 6c6c 7920 6d61 6e75 616c 206f 7074  fully manual opt
-00000cf0: 696f 6e20 6f66 206a 7573 7420 646f 776e  ion of just down
-00000d00: 6c6f 6164 696e 6720 626f 7468 2063 6f64  loading both cod
-00000d10: 650a 7265 706f 7369 746f 7269 6573 2c20  e.repositories, 
-00000d20: 6368 616e 6769 6e67 2074 6f20 7468 6520  changing to the 
-00000d30: 636f 6465 2064 6972 6563 746f 7279 2c20  code directory, 
-00000d40: 616e 6420 6973 7375 696e 670a 0a60 6060  and issuing..```
-00000d50: 7368 0a70 7974 686f 6e20 7365 7475 702e  sh.python setup.
-00000d60: 7079 2069 6e73 7461 6c6c 0a60 6060 0a0a  py install.```..
-00000d70: 5468 6973 2073 686f 756c 6420 776f 726b  This should work
-00000d80: 2072 6567 6172 646c 6573 7320 6f66 2074   regardless of t
-00000d90: 6865 2069 6e73 7461 6c6c 6174 696f 6e20  he installation 
-00000da0: 6d65 7468 6f64 2c20 6173 206c 6f6e 6720  method, as long 
-00000db0: 6173 2079 6f75 2068 6176 6520 610a 636f  as you have a.co
-00000dc0: 6d70 696c 6572 2068 616e 6769 6e67 2061  mpiler hanging a
-00000dd0: 726f 756e 642e 0a0a 0a23 2320 5573 6167  round....## Usag
-00000de0: 650a 0a46 6972 7374 2c20 7765 2073 686f  e..First, we sho
-00000df0: 7720 6120 7665 7279 2073 696d 706c 6520  w a very simple 
-00000e00: 6578 616d 706c 6520 6f66 2075 7361 6765  example of usage
-00000e10: 2077 6974 6820 4575 6c65 7220 616e 676c   with Euler angl
-00000e20: 6573 2c20 7468 6f75 6768 2069 740a 6272  es, though it.br
-00000e30: 6561 6b73 206d 7920 6865 6172 7420 746f  eaks my heart to
-00000e40: 2064 6f20 736f 3a3c 7375 703e 5b31 5d28   do so:<sup>[1](
-00000e50: 2365 756c 6572 2d61 6e67 6c65 732d 6172  #euler-angles-ar
-00000e60: 652d 6177 6675 6c29 3c2f 7375 703e 0a0a  e-awful)</sup>..
-00000e70: 6060 6070 7974 686f 6e0a 3e3e 3e20 696d  ```python.>>> im
-00000e80: 706f 7274 2073 7068 6572 6963 616c 5f66  port spherical_f
-00000e90: 756e 6374 696f 6e73 2061 7320 7366 0a3e  unctions as sf.>
-00000ea0: 3e3e 2061 6c70 6861 2c20 6265 7461 2c20  >> alpha, beta, 
-00000eb0: 6761 6d6d 6120 3d20 302e 312c 2030 2e32  gamma = 0.1, 0.2
-00000ec0: 2c20 302e 330a 3e3e 3e20 656c 6c2c 6d70  , 0.3.>>> ell,mp
-00000ed0: 2c6d 203d 2033 2c32 2c31 0a3e 3e3e 2073  ,m = 3,2,1.>>> s
-00000ee0: 662e 5769 676e 6572 5f44 5f65 6c65 6d65  f.Wigner_D_eleme
-00000ef0: 6e74 2861 6c70 6861 2c20 6265 7461 2c20  nt(alpha, beta, 
-00000f00: 6761 6d6d 612c 2065 6c6c 2c20 6d70 2c20  gamma, ell, mp, 
-00000f10: 6d29 0a0a 6060 600a 0a4f 6620 636f 7572  m)..```..Of cour
-00000f20: 7365 2c20 6974 2773 2061 6c77 6179 7320  se, it's always 
-00000f30: 6265 7474 6572 2074 6f20 7573 6520 756e  better to use un
-00000f40: 6974 2071 7561 7465 726e 696f 6e73 2074  it quaternions t
-00000f50: 6f20 6465 7363 7269 6265 2072 6f74 6174  o describe rotat
-00000f60: 696f 6e73 3a0a 0a60 6060 7079 7468 6f6e  ions:..```python
-00000f70: 0a3e 3e3e 2069 6d70 6f72 7420 6e75 6d70  .>>> import nump
-00000f80: 7920 6173 206e 700a 3e3e 3e20 696d 706f  y as np.>>> impo
-00000f90: 7274 2071 7561 7465 726e 696f 6e0a 3e3e  rt quaternion.>>
-00000fa0: 3e20 5220 3d20 6e70 2e71 7561 7465 726e  > R = np.quatern
-00000fb0: 696f 6e28 312c 322c 332c 3429 2e6e 6f72  ion(1,2,3,4).nor
-00000fc0: 6d61 6c69 7a65 6428 290a 3e3e 3e20 656c  malized().>>> el
-00000fd0: 6c2c 6d70 2c6d 203d 2033 2c32 2c31 0a3e  l,mp,m = 3,2,1.>
-00000fe0: 3e3e 2073 662e 5769 676e 6572 5f44 5f65  >> sf.Wigner_D_e
-00000ff0: 6c65 6d65 6e74 2852 2c20 656c 6c2c 206d  lement(R, ell, m
-00001000: 702c 206d 290a 0a60 6060 0a0a 4966 2079  p, m)..```..If y
-00001010: 6f75 206e 6565 6420 746f 2063 616c 6375  ou need to calcu
-00001020: 6c61 7465 2076 616c 7565 7320 6f66 2074  late values of t
-00001030: 6865 20f0 9d94 873c 7375 703e 28e2 8493  he ....<sup>(...
-00001040: 293c 2f73 7570 3e20 6d61 7472 6978 2065  )</sup> matrix e
-00001050: 6c65 6d65 6e74 7320 666f 7220 6d61 6e79  lements for many
-00001060: 0a76 616c 7565 7320 6f66 2028 e284 932c  .values of (...,
-00001070: 206d 272c 206d 292c 2069 7420 6973 206d   m', m), it is m
-00001080: 6f72 6520 6566 6669 6369 656e 7420 746f  ore efficient to
-00001090: 2064 6f20 736f 2061 6c6c 2061 7420 6f6e   do so all at on
-000010a0: 6365 2e20 2054 6865 2066 6f6c 6c6f 7769  ce.  The followi
-000010b0: 6e67 0a63 616c 6375 6c61 7465 7320 616c  ng.calculates al
-000010c0: 6c20 6d6f 6465 7320 666f 7220 e284 9320  l modes for ... 
-000010d0: 6672 6f6d 2032 2074 6f20 3820 2869 6e63  from 2 to 8 (inc
-000010e0: 6c75 7369 7665 293a 0a0a 6060 6070 7974  lusive):..```pyt
-000010f0: 686f 6e0a 3e3e 3e20 696e 6469 6365 7320  hon.>>> indices 
-00001100: 3d20 6e70 2e61 7272 6179 285b 5b65 6c6c  = np.array([[ell
-00001110: 2c6d 702c 6d5d 2066 6f72 2065 6c6c 2069  ,mp,m] for ell i
-00001120: 6e20 7261 6e67 6528 322c 3929 0a2e 2e2e  n range(2,9)....
-00001130: 2066 6f72 206d 7020 696e 2072 616e 6765   for mp in range
-00001140: 282d 656c 6c2c 2065 6c6c 2b31 2920 666f  (-ell, ell+1) fo
-00001150: 7220 6d20 696e 2072 616e 6765 282d 656c  r m in range(-el
-00001160: 6c2c 2065 6c6c 2b31 295d 290a 3e3e 3e20  l, ell+1)]).>>> 
-00001170: 7366 2e57 6967 6e65 725f 445f 656c 656d  sf.Wigner_D_elem
-00001180: 656e 7428 522c 2069 6e64 6963 6573 290a  ent(R, indices).
-00001190: 0a60 6060 0a0a 4669 6e61 6c6c 792c 2069  .```..Finally, i
-000011a0: 6620 796f 7520 7265 616c 6c79 206e 6565  f you really nee
-000011b0: 6420 746f 2070 7574 2074 6865 2070 6564  d to put the ped
-000011c0: 616c 2074 6f20 7468 6520 6d65 7461 6c2c  al to the metal,
-000011d0: 2061 6e64 2061 7265 2077 696c 6c69 6e67   and are willing
-000011e0: 2074 6f0a 6775 6172 616e 7465 6520 7468   to.guarantee th
-000011f0: 6174 2074 6865 2069 6e70 7574 2061 7267  at the input arg
-00001200: 756d 656e 7473 2061 7265 2063 6f72 7265  uments are corre
-00001210: 6374 2c20 796f 7520 6361 6e20 7573 6520  ct, you can use 
-00001220: 6120 7370 6563 6961 6c20 6869 6464 656e  a special hidden
-00001230: 0a66 6f72 6d20 6f66 2074 6865 2066 756e  .form of the fun
-00001240: 6374 696f 6e3a 0a0a 6060 6070 7974 686f  ction:..```pytho
-00001250: 6e0a 3e3e 3e20 7366 2e5f 5769 676e 6572  n.>>> sf._Wigner
-00001260: 5f44 5f65 6c65 6d65 6e74 2852 2e61 2c20  _D_element(R.a, 
-00001270: 522e 622c 2069 6e64 6963 6573 2c20 656c  R.b, indices, el
-00001280: 656d 656e 7473 290a 0a60 6060 0a0a 4865  ements)..```..He
-00001290: 7265 2c20 6052 2e61 6020 616e 6420 6052  re, `R.a` and `R
-000012a0: 2e62 6020 6172 6520 7468 6520 7477 6f20  .b` are the two 
-000012b0: 636f 6d70 6c65 7820 7061 7274 7320 6f66  complex parts of
-000012c0: 2074 6865 2071 7561 7465 726e 696f 6e20   the quaternion 
-000012d0: 6465 6669 6e65 6420 6f6e 0a5b 7468 6973  defined on.[this
-000012e0: 2070 6167 655d 2868 7474 703a 2f2f 6d6f   page](http://mo
-000012f0: 626c 652e 6769 7468 7562 2e69 6f2f 7370  ble.github.io/sp
-00001300: 6865 7269 6361 6c5f 6675 6e63 7469 6f6e  herical_function
-00001310: 732f 2920 2874 686f 7567 6820 7468 6520  s/) (though the 
-00001320: 7573 6572 206e 6565 640a 6e6f 7420 6361  user need.not ca
-00001330: 7265 2061 626f 7574 2074 6861 7429 2e20  re about that). 
-00001340: 2054 6865 2060 696e 6469 6365 7360 2076   The `indices` v
-00001350: 6172 6961 626c 6520 6973 2061 7373 756d  ariable is assum
-00001360: 6564 2074 6f20 6265 2061 0a74 776f 2d64  ed to be a.two-d
-00001370: 696d 656e 7369 6f6e 616c 2061 7272 6179  imensional array
-00001380: 206f 6620 696e 7465 6765 7273 2c20 7768   of integers, wh
-00001390: 6572 6520 7468 6520 7365 636f 6e64 2064  ere the second d
-000013a0: 696d 656e 7369 6f6e 2068 6173 2073 697a  imension has siz
-000013b0: 6520 7468 7265 652c 0a72 6570 7265 7365  e three,.represe
-000013c0: 6e74 696e 6720 7468 6520 28e2 8493 2c20  nting the (..., 
-000013d0: 6d27 2c20 6d29 2069 6e64 6963 6573 2e20  m', m) indices. 
-000013e0: 2054 6869 7320 6176 6f69 6473 2063 6572   This avoids cer
-000013f0: 7461 696e 2073 6f6d 6577 6861 7420 736c  tain somewhat sl
-00001400: 6f77 6572 0a70 7572 652d 7079 7468 6f6e  ower.pure-python
-00001410: 206f 7065 7261 7469 6f6e 7320 696e 766f   operations invo
-00001420: 6c76 696e 6720 6172 6775 6d65 6e74 2063  lving argument c
-00001430: 6865 636b 696e 672c 2072 6573 6861 7069  hecking, reshapi
-00001440: 6e67 2c20 6574 632e 2020 5468 650a 6065  ng, etc.  The.`e
-00001450: 6c65 6d65 6e74 7360 2076 6172 6961 626c  lements` variabl
-00001460: 6520 6d75 7374 2062 6520 6120 6f6e 652d  e must be a one-
-00001470: 6469 6d65 6e73 696f 6e61 6c20 6172 7261  dimensional arra
-00001480: 7920 6f66 2063 6f6d 706c 6578 206e 756d  y of complex num
-00001490: 6265 7273 2028 6361 6e20 6265 0a75 6e69  bers (can be.uni
-000014a0: 6e69 7469 616c 697a 6564 292c 2077 6869  nitialized), whi
-000014b0: 6368 2077 696c 6c20 6265 2072 6570 6c61  ch will be repla
-000014c0: 6365 6420 7769 7468 2074 6865 2063 6f72  ced with the cor
-000014d0: 7265 7370 6f6e 6469 6e67 2076 616c 7565  responding value
-000014e0: 7320 6f6e 2072 6574 7572 6e2e 0a41 6761  s on return..Aga
-000014f0: 696e 2c20 686f 7765 7665 722c 2074 6865  in, however, the
-00001500: 7265 2069 7320 6e6f 2069 6e70 7574 2064  re is no input d
-00001510: 696d 656e 7369 6f6e 2063 6865 636b 696e  imension checkin
-00001520: 6720 6865 7265 2c20 736f 2069 6620 796f  g here, so if yo
-00001530: 7520 6769 7665 2062 6164 0a69 6e70 7574  u give bad.input
-00001540: 732c 2062 6568 6176 696f 7220 636f 756c  s, behavior coul
-00001550: 6420 7261 6e67 6520 6672 6f6d 2073 696c  d range from sil
-00001560: 656e 746c 7920 7772 6f6e 6720 746f 2065  ently wrong to e
-00001570: 7863 6570 7469 6f6e 7320 746f 2073 6567  xceptions to seg
-00001580: 6d65 6e74 6174 696f 6e0a 6661 756c 7473  mentation.faults
-00001590: 2e20 2043 6176 6561 7420 656d 7074 6f72  .  Caveat emptor
-000015a0: 2e0a 0a0a 2323 2041 636b 6e6f 776c 6564  ....## Acknowled
-000015b0: 676d 656e 7473 0a0a 4920 7665 7279 206d  gments..I very m
-000015c0: 7563 6820 6170 7072 6563 6961 7465 2042  uch appreciate B
-000015d0: 6172 7279 2057 6172 6465 6c6c 2773 2068  arry Wardell's h
-000015e0: 656c 7020 696e 2073 6f72 7469 6e67 206f  elp in sorting o
-000015f0: 7574 2074 6865 2072 656c 6174 696f 6e73  ut the relations
-00001600: 6869 7073 0a62 6574 7765 656e 206d 7920  hips.between my 
-00001610: 636f 6e76 656e 7469 6f6e 7320 616e 6420  conventions and 
-00001620: 7468 6f73 6520 6f66 206f 7468 6572 2070  those of other p
-00001630: 656f 706c 6520 616e 6420 736f 6674 7761  eople and softwa
-00001640: 7265 2070 6163 6b61 6765 730a 2865 7370  re packages.(esp
-00001650: 6563 6961 6c6c 7920 4d61 7468 656d 6174  ecially Mathemat
-00001660: 6963 6127 7320 6372 617a 7920 636f 6e76  ica's crazy conv
-00001670: 656e 7469 6f6e 7329 2e0a 0a54 6869 7320  entions)...This 
-00001680: 636f 6465 2069 732c 206f 6620 636f 7572  code is, of cour
-00001690: 7365 2c20 686f 7374 6564 206f 6e20 6769  se, hosted on gi
-000016a0: 7468 7562 2e20 2042 6563 6175 7365 2069  thub.  Because i
-000016b0: 7420 6973 2061 6e20 6f70 656e 2d73 6f75  t is an open-sou
-000016c0: 7263 650a 7072 6f6a 6563 742c 2074 6865  rce.project, the
-000016d0: 2068 6f73 7469 6e67 2069 7320 6672 6565   hosting is free
-000016e0: 2c20 616e 6420 616c 6c20 7468 6520 776f  , and all the wo
-000016f0: 6e64 6572 6675 6c20 6665 6174 7572 6573  nderful features
-00001700: 206f 6620 6769 7468 7562 2061 7265 0a61   of github are.a
-00001710: 7661 696c 6162 6c65 2c20 696e 636c 7564  vailable, includ
-00001720: 696e 6720 6672 6565 2077 696b 6920 7370  ing free wiki sp
-00001730: 6163 6520 616e 6420 7765 6220 7061 6765  ace and web page
-00001740: 2068 6f73 7469 6e67 2c20 7075 6c6c 2072   hosting, pull r
-00001750: 6571 7565 7374 732c 2061 0a6e 6963 6520  equests, a.nice 
-00001760: 696e 7465 7266 6163 6520 746f 2074 6865  interface to the
-00001770: 2067 6974 206c 6f67 732c 2065 7463 2e0a   git logs, etc..
-00001780: 0a45 7665 7279 2063 6861 6e67 6520 696e  .Every change in
-00001790: 2074 6869 7320 636f 6465 2069 730a 5b61   this code is.[a
-000017a0: 756f 6d61 7469 6361 6c6c 7920 7465 7374  uomatically test
-000017b0: 6564 5d28 6874 7470 733a 2f2f 7472 6176  ed](https://trav
-000017c0: 6973 2d63 692e 6f72 672f 6d6f 626c 652f  is-ci.org/moble/
-000017d0: 7370 6865 7269 6361 6c5f 6675 6e63 7469  spherical_functi
-000017e0: 6f6e 7329 206f 6e0a 5b54 7261 7669 732d  ons) on.[Travis-
-000017f0: 4349 5d28 6874 7470 733a 2f2f 7472 6176  CI](https://trav
-00001800: 6973 2d63 692e 6f72 672f 292e 2020 5468  is-ci.org/).  Th
-00001810: 6973 2069 7320 6120 6672 6565 2073 6572  is is a free ser
-00001820: 7669 6365 2028 666f 7220 6f70 656e 2d73  vice (for open-s
-00001830: 6f75 7263 650a 7072 6f6a 6563 7473 206c  ource.projects l
-00001840: 696b 6520 7468 6973 206f 6e65 292c 2077  ike this one), w
-00001850: 6869 6368 2069 6e74 6567 7261 7465 7320  hich integrates 
-00001860: 6265 6175 7469 6675 6c6c 7920 7769 7468  beautifully with
-00001870: 2067 6974 6875 622c 2064 6574 6563 7469   github, detecti
-00001880: 6e67 0a65 6163 6820 636f 6d6d 6974 2061  ng.each commit a
-00001890: 6e64 2061 7574 6f6d 6174 6963 616c 6c79  nd automatically
-000018a0: 2072 652d 7275 6e6e 696e 6720 7468 6520   re-running the 
-000018b0: 7465 7374 732e 2020 5468 6520 636f 6465  tests.  The code
-000018c0: 2069 7320 646f 776e 6c6f 6164 6564 2061   is downloaded a
-000018d0: 6e64 0a69 6e73 7461 6c6c 6564 2066 7265  nd.installed fre
-000018e0: 7368 2065 6163 6820 7469 6d65 2c20 616e  sh each time, an
-000018f0: 6420 7468 656e 2074 6573 7465 642c 206f  d then tested, o
-00001900: 6e20 7079 7468 6f6e 2032 2e37 2c20 332e  n python 2.7, 3.
-00001910: 342c 2061 6e64 2033 2e35 2e20 2054 6869  4, and 3.5.  Thi
-00001920: 730a 656e 7375 7265 7320 7468 6174 206e  s.ensures that n
-00001930: 6f20 6368 616e 6765 2049 206d 616b 6520  o change I make 
-00001940: 746f 2074 6865 2063 6f64 6520 6272 6561  to the code brea
-00001950: 6b73 2065 6974 6865 7220 696e 7374 616c  ks either instal
-00001960: 6c61 7469 6f6e 206f 7220 616e 7920 6f66  lation or any of
-00001970: 0a74 6865 2066 6561 7475 7265 7320 7468  .the features th
-00001980: 6174 2049 2068 6176 6520 7772 6974 7465  at I have writte
-00001990: 6e20 7465 7374 7320 666f 722e 0a0a 4669  n tests for...Fi
-000019a0: 6e61 6c6c 792c 2074 6865 2063 6f64 6520  nally, the code 
-000019b0: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
-000019c0: 2063 6f6d 7069 6c65 642c 2061 6e64 2074   compiled, and t
-000019d0: 6865 2062 696e 6172 6965 7320 686f 7374  he binaries host
-000019e0: 6564 2066 6f72 0a64 6f77 6e6c 6f61 6420  ed for.download 
-000019f0: 6279 2060 636f 6e64 6160 206f 6e20 5b61  by `conda` on [a
-00001a00: 6e61 636f 6e64 612e 6f72 675d 2868 7474  naconda.org](htt
-00001a10: 7073 3a2f 2f61 6e61 636f 6e64 612e 6f72  ps://anaconda.or
-00001a20: 672f 6d6f 626c 652f 7175 6174 6572 6e69  g/moble/quaterni
-00001a30: 6f6e 292e 0a54 6869 7320 6973 2061 6c73  on)..This is als
-00001a40: 6f20 6120 6672 6565 2073 6572 7669 6365  o a free service
-00001a50: 2066 6f72 206f 7065 6e2d 736f 7572 6365   for open-source
-00001a60: 2070 726f 6a65 6374 7320 6c69 6b65 2074   projects like t
-00001a70: 6869 7320 6f6e 652e 0a0a 5468 6520 776f  his one...The wo
-00001a80: 726b 206f 6620 6372 6561 7469 6e67 2074  rk of creating t
-00001a90: 6869 7320 636f 6465 2077 6173 2073 7570  his code was sup
-00001aa0: 706f 7274 6564 2069 6e20 7061 7274 2062  ported in part b
-00001ab0: 7920 7468 6520 5368 6572 6d61 6e20 4661  y the Sherman Fa
-00001ac0: 6972 6368 696c 640a 466f 756e 6461 7469  irchild.Foundati
-00001ad0: 6f6e 2061 6e64 2062 7920 4e53 4620 4772  on and by NSF Gr
-00001ae0: 616e 7473 204e 6f2e 2050 4859 2d31 3330  ants No. PHY-130
-00001af0: 3631 3235 2061 6e64 2041 5354 2d31 3333  6125 and AST-133
-00001b00: 3331 3239 2e0a 0a0a 3c62 722f 3e0a 2d2d  3129....<br/>.--
-00001b10: 2d0a 2323 2323 2323 203c 7375 703e 313c  -.###### <sup>1<
-00001b20: 2f73 7570 3e20 4575 6c65 7220 616e 676c  /sup> Euler angl
-00001b30: 6573 2061 7265 2061 7766 756c 0a0a 4575  es are awful..Eu
-00001b40: 6c65 7220 616e 676c 6573 2061 7265 2070  ler angles are p
-00001b50: 7265 7474 7920 6d75 6368 0a5b 7468 6520  retty much.[the 
-00001b60: 776f 7273 7420 7468 696e 6773 2065 7665  worst things eve
-00001b70: 725d 2868 7474 703a 2f2f 6d6f 626c 652e  r](http://moble.
-00001b80: 6769 7468 7562 2e69 6f2f 7370 6865 7269  github.io/spheri
-00001b90: 6361 6c5f 6675 6e63 7469 6f6e 732f 2365  cal_functions/#e
-00001ba0: 756c 6572 2d61 6e67 6c65 7329 0a61 6e64  uler-angles).and
-00001bb0: 2069 7420 6d61 6b65 7320 6d65 2066 6565   it makes me fee
-00001bc0: 6c20 6261 6420 6576 656e 2073 7570 706f  l bad even suppo
-00001bd0: 7274 696e 6720 7468 656d 2e20 2051 7561  rting them.  Qua
-00001be0: 7465 726e 696f 6e73 2061 7265 0a66 6173  ternions are.fas
-00001bf0: 7465 722c 206d 6f72 6520 6163 6375 7261  ter, more accura
-00001c00: 7465 2c20 6261 7369 6361 6c6c 7920 6672  te, basically fr
-00001c10: 6565 206f 6620 7369 6e67 756c 6172 6974  ee of singularit
-00001c20: 6965 732c 206d 6f72 650a 696e 7475 6974  ies, more.intuit
-00001c30: 6976 652c 2061 6e64 2067 656e 6572 616c  ive, and general
-00001c40: 6c79 2065 6173 6965 7220 746f 2075 6e64  ly easier to und
-00001c50: 6572 7374 616e 642e 2020 596f 7520 6361  erstand.  You ca
-00001c60: 6e20 776f 726b 2065 6e74 6972 656c 790a  n work entirely.
-00001c70: 7769 7468 6f75 7420 4575 6c65 7220 616e  without Euler an
-00001c80: 676c 6573 2028 4920 6365 7274 6169 6e6c  gles (I certainl
-00001c90: 7920 646f 292e 2020 596f 7520 6162 736f  y do).  You abso
-00001ca0: 6c75 7465 6c79 206e 6576 6572 206e 6565  lutely never nee
-00001cb0: 640a 7468 656d 2e20 2042 7574 2069 6620  d.them.  But if 
-00001cc0: 796f 7527 7265 2073 6f20 6f6c 6420 6661  you're so old fa
-00001cd0: 7368 696f 6e65 6420 7468 6174 2079 6f75  shioned that you
-00001ce0: 2072 6561 6c6c 7920 6361 6e27 7420 6769   really can't gi
-00001cf0: 7665 2074 6865 6d0a 7570 2c20 7468 6579  ve them.up, they
-00001d00: 2061 7265 2066 756c 6c79 2073 7570 706f   are fully suppo
-00001d10: 7274 6564 2e0a                           rted..
+00000000: 5b21 5b54 6573 7420 5374 6174 7573 5d28  [![Test Status](
+00000010: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000020: 6f6d 2f6d 6f62 6c65 2f73 7068 6572 6963  om/moble/spheric
+00000030: 616c 5f66 756e 6374 696f 6e73 2f77 6f72  al_functions/wor
+00000040: 6b66 6c6f 7773 2f74 6573 7473 2f62 6164  kflows/tests/bad
+00000050: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
+00000060: 2f67 6974 6875 622e 636f 6d2f 6d6f 626c  /github.com/mobl
+00000070: 652f 7370 6865 7269 6361 6c5f 6675 6e63  e/spherical_func
+00000080: 7469 6f6e 732f 6163 7469 6f6e 7329 0a5b  tions/actions).[
+00000090: 215b 5079 5049 2056 6572 7369 6f6e 5d28  ![PyPI Version](
+000000a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000000b0: 6c64 732e 696f 2f70 7970 692f 762f 7370  lds.io/pypi/v/sp
+000000c0: 6865 7269 6361 6c2d 6675 6e63 7469 6f6e  herical-function
+000000d0: 733f 636f 6c6f 723d 295d 2868 7474 7073  s?color=)](https
+000000e0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000000f0: 6563 742f 7370 6865 7269 6361 6c2d 6675  ect/spherical-fu
+00000100: 6e63 7469 6f6e 732f 290a 5b21 5b43 6f6e  nctions/).[![Con
+00000110: 6461 2056 6572 7369 6f6e 5d28 6874 7470  da Version](http
+00000120: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000130: 696f 2f63 6f6e 6461 2f76 6e2f 636f 6e64  io/conda/vn/cond
+00000140: 612d 666f 7267 652f 7370 6865 7269 6361  a-forge/spherica
+00000150: 6c5f 6675 6e63 7469 6f6e 732e 7376 673f  l_functions.svg?
+00000160: 636f 6c6f 723d 295d 2868 7474 7073 3a2f  color=)](https:/
+00000170: 2f61 6e61 636f 6e64 612e 6f72 672f 636f  /anaconda.org/co
+00000180: 6e64 612d 666f 7267 652f 7370 6865 7269  nda-forge/spheri
+00000190: 6361 6c5f 6675 6e63 7469 6f6e 7329 0a5b  cal_functions).[
+000001a0: 215b 4d49 5420 4c69 6365 6e73 655d 2868  ![MIT License](h
+000001b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000001c0: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
+000001d0: 656e 7365 2f6d 6f62 6c65 2f73 7068 6572  ense/moble/spher
+000001e0: 6963 616c 5f66 756e 6374 696f 6e73 2e73  ical_functions.s
+000001f0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000200: 6875 622e 636f 6d2f 6d6f 626c 652f 7370  hub.com/moble/sp
+00000210: 6865 7269 6361 6c5f 6675 6e63 7469 6f6e  herical_function
+00000220: 732f 626c 6f62 2f6d 6169 6e2f 4c49 4345  s/blob/main/LICE
+00000230: 4e53 4529 0a5b 215b 444f 495d 2868 7474  NSE).[![DOI](htt
+00000240: 7073 3a2f 2f7a 656e 6f64 6f2e 6f72 672f  ps://zenodo.org/
+00000250: 6261 6467 652f 3235 3538 3937 3832 2e73  badge/25589782.s
+00000260: 7667 295d 2868 7474 7073 3a2f 2f7a 656e  vg)](https://zen
+00000270: 6f64 6f2e 6f72 672f 6261 6467 652f 6c61  odo.org/badge/la
+00000280: 7465 7374 646f 692f 3235 3538 3937 3832  testdoi/25589782
+00000290: 290a 0a0a 2320 5370 6865 7269 6361 6c20  )...# Spherical 
+000002a0: 4675 6e63 7469 6f6e 730a 0a7c 204e 4f54  Functions..| NOT
+000002b0: 453a 2054 6869 7320 7061 636b 6167 6520  E: This package 
+000002c0: 7769 6c6c 2073 7469 6c6c 2062 6520 6d61  will still be ma
+000002d0: 696e 7461 696e 6564 2c20 6275 7420 2a61  intained, but *a
+000002e0: 6374 6976 652a 2064 6576 656c 6f70 6d65  ctive* developme
+000002f0: 6e74 2068 6173 206d 6f76 6564 2074 6f20  nt has moved to 
+00000300: 7468 6520 5b60 7370 6865 7269 6361 6c60  the [`spherical`
+00000310: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000320: 2e63 6f6d 2f6d 6f62 6c65 2f73 7068 6572  .com/moble/spher
+00000330: 6963 616c 2920 7061 636b 6167 652e 2020  ical) package.  
+00000340: 5768 696c 6520 7468 6973 2070 6163 6b61  While this packa
+00000350: 6765 2077 6f72 6b73 2077 656c 6c20 666f  ge works well fo
+00000360: 7220 e284 9320 2861 6b61 2065 6c6c 2c20  r ... (aka ell, 
+00000370: 4c2c 206a 2c20 6f72 204a 2920 7661 6c75  L, j, or J) valu
+00000380: 6573 2075 7020 746f 2061 726f 756e 6420  es up to around 
+00000390: 3235 2c20 6572 726f 7273 2073 7461 7274  25, errors start
+000003a0: 2074 6f20 6275 696c 6420 7261 7069 646c   to build rapidl
+000003b0: 7920 616e 6420 7475 726e 2069 6e74 6f20  y and turn into 
+000003c0: 4e61 4e73 2061 726f 756e 6420 3330 2e20  NaNs around 30. 
+000003d0: 2054 6865 2060 7370 6865 7269 6361 6c60   The `spherical`
+000003e0: 2070 6163 6b61 6765 2063 616e 2072 6561   package can rea
+000003f0: 6469 6c79 2068 616e 646c 6520 7661 6c75  dily handle valu
+00000400: 6573 2075 7020 746f 2061 7420 6c65 6173  es up to at leas
+00000410: 7420 3130 3030 2c20 7769 7468 2061 6363  t 1000, with acc
+00000420: 7572 6163 7920 636c 6f73 6520 746f 20e2  uracy close to .
+00000430: 8493 2074 696d 6573 206d 6163 6869 6e65  .. times machine
+00000440: 2070 7265 6369 7369 6f6e 2e20 20e2 8094   precision.  ...
+00000450: 4d69 6b65 207c 0a7c 202d 2d2d 207c 0a0a  Mike |.| --- |..
+00000460: 0a50 7974 686f 6e2f 6e75 6d62 6120 7061  .Python/numba pa
+00000470: 636b 6167 6520 666f 7220 6576 616c 7561  ckage for evalua
+00000480: 7469 6e67 2061 6e64 2074 7261 6e73 666f  ting and transfo
+00000490: 726d 696e 6720 5769 676e 6572 2773 20f0  rming Wigner's .
+000004a0: 9d94 8720 6d61 7472 6963 6573 2c0a 5769  ... matrices,.Wi
+000004b0: 676e 6572 2773 2033 2d6a 2073 796d 626f  gner's 3-j symbo
+000004c0: 6c73 2c20 616e 6420 7370 696e 2d77 6569  ls, and spin-wei
+000004d0: 6768 7465 6420 2861 6e64 2073 6361 6c61  ghted (and scala
+000004e0: 7229 2073 7068 6572 6963 616c 2068 6172  r) spherical har
+000004f0: 6d6f 6e69 6373 2e0a 5468 6573 6520 6675  monics..These fu
+00000500: 6e63 7469 6f6e 7320 6172 6520 6576 616c  nctions are eval
+00000510: 7561 7465 6420 6469 7265 6374 6c79 2069  uated directly i
+00000520: 6e20 7465 726d 7320 6f66 2071 7561 7465  n terms of quate
+00000530: 726e 696f 6e73 2c20 6173 2077 656c 6c20  rnions, as well 
+00000540: 6173 2069 6e0a 7468 6520 6d6f 7265 2073  as in.the more s
+00000550: 7461 6e64 6172 6420 666f 726d 7320 6f66  tandard forms of
+00000560: 2073 7068 6572 6963 616c 2063 6f6f 7264   spherical coord
+00000570: 696e 6174 6573 2061 6e64 2045 756c 6572  inates and Euler
+00000580: 0a61 6e67 6c65 732e 3c73 7570 3e5b 315d  .angles.<sup>[1]
+00000590: 2823 312d 6575 6c65 722d 616e 676c 6573  (#1-euler-angles
+000005a0: 2d61 7265 2d61 7766 756c 293c 2f73 7570  -are-awful)</sup
+000005b0: 3e0a 0a54 6865 2063 6f6e 7665 6e74 696f  >..The conventio
+000005c0: 6e73 2066 6f72 2074 6869 7320 7061 636b  ns for this pack
+000005d0: 6167 6520 6172 6520 6465 7363 7269 6265  age are describe
+000005e0: 6420 696e 2064 6574 6169 6c20 6f6e 0a5b  d in detail on.[
+000005f0: 7468 6973 2070 6167 655d 2868 7474 703a  this page](http:
+00000600: 2f2f 6d6f 626c 652e 6769 7468 7562 2e69  //moble.github.i
+00000610: 6f2f 7370 6865 7269 6361 6c5f 6675 6e63  o/spherical_func
+00000620: 7469 6f6e 732f 292e 0a0a 2323 2044 6570  tions/)...## Dep
+00000630: 656e 6465 6e63 6965 730a 0a54 6865 206f  endencies..The o
+00000640: 6e6c 7920 7472 7565 2072 6571 7569 7265  nly true require
+00000650: 6d65 6e74 7320 666f 7220 7468 6973 2063  ments for this c
+00000660: 6f64 6520 6172 6520 6070 7974 686f 6e60  ode are `python`
+00000670: 2061 6e64 2074 6865 2070 7974 686f 6e20   and the python 
+00000680: 7061 636b 6167 650a 606e 756d 7079 602c  package.`numpy`,
+00000690: 2061 7320 7765 6c6c 2061 7320 6d79 2061   as well as my a
+000006a0: 6363 6f6d 7061 6e79 696e 670a 5b60 7175  ccompanying.[`qu
+000006b0: 6174 6572 6e69 6f6e 605d 2868 7474 7073  aternion`](https
+000006c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d6f  ://github.com/mo
+000006d0: 626c 652f 7175 6174 6572 6e69 6f6e 2920  ble/quaternion) 
+000006e0: 7061 636b 6167 6520 2869 6e73 7461 6c6c  package (install
+000006f0: 6174 696f 6e20 6f66 0a77 6869 6368 2069  ation of.which i
+00000700: 7320 7368 6f77 6e20 6265 6c6f 7729 2e0a  s shown below)..
+00000710: 0a48 6f77 6576 6572 2c20 7468 6973 2070  .However, this p
+00000720: 6163 6b61 6765 2063 616e 2061 7574 6f6d  ackage can autom
+00000730: 6174 6963 616c 6c79 2075 7365 0a5b 606e  atically use.[`n
+00000740: 756d 6261 605d 2868 7474 703a 2f2f 6e75  umba`](http://nu
+00000750: 6d62 612e 7079 6461 7461 2e6f 7267 2f29  mba.pydata.org/)
+00000760: 2c20 7768 6963 6820 7573 6573 205b 4c4c  , which uses [LL
+00000770: 564d 5d28 6874 7470 3a2f 2f6c 6c76 6d2e  VM](http://llvm.
+00000780: 6f72 672f 2920 746f 0a63 6f6d 7069 6c65  org/) to.compile
+00000790: 2070 7974 686f 6e20 636f 6465 2074 6f20   python code to 
+000007a0: 6d61 6368 696e 6520 636f 6465 2c20 6163  machine code, ac
+000007b0: 6365 6c65 7261 7469 6e67 206d 6f73 7420  celerating most 
+000007c0: 6e75 6d65 7269 6361 6c20 6675 6e63 7469  numerical functi
+000007d0: 6f6e 7320 6279 0a66 6163 746f 7273 206f  ons by.factors o
+000007e0: 6620 616e 7977 6865 7265 2066 726f 6d20  f anywhere from 
+000007f0: 3220 746f 2032 3030 302e 2020 4974 2069  2 to 2000.  It i
+00000800: 7320 2a70 6f73 7369 626c 652a 2074 6f20  s *possible* to 
+00000810: 7275 6e20 7468 6520 636f 6465 2077 6974  run the code wit
+00000820: 686f 7574 0a60 6e75 6d62 6160 2c20 6275  hout.`numba`, bu
+00000830: 7420 7468 6520 6d6f 7374 2069 6d70 6f72  t the most impor
+00000840: 7461 6e74 2066 756e 6374 696f 6e73 2061  tant functions a
+00000850: 7265 2072 6f75 6768 6c79 2031 3020 7469  re roughly 10 ti
+00000860: 6d65 7320 736c 6f77 6572 2077 6974 686f  mes slower witho
+00000870: 7574 0a69 742e 0a0a 5468 6520 6f6e 6c79  ut.it...The only
+00000880: 2064 7261 7762 6163 6b20 6f66 2060 6e75   drawback of `nu
+00000890: 6d62 6160 2069 7320 7468 6174 2069 7420  mba` is that it 
+000008a0: 6973 206e 6f6e 7472 6976 6961 6c20 746f  is nontrivial to
+000008b0: 2069 6e73 7461 6c6c 206f 6e20 6974 7320   install on its 
+000008c0: 6f77 6e2e 0a46 6f72 7475 6e61 7465 6c79  own..Fortunately
+000008d0: 2c20 7468 6520 6265 7374 2070 7974 686f  , the best pytho
+000008e0: 6e20 696e 7374 616c 6c65 722c 0a5b 6061  n installer,.[`a
+000008f0: 6e61 636f 6e64 6160 5d28 6874 7470 3a2f  naconda`](http:/
+00000900: 2f63 6f6e 7469 6e75 756d 2e69 6f2f 646f  /continuum.io/do
+00000910: 776e 6c6f 6164 7329 2c20 6d61 6b65 7320  wnloads), makes 
+00000920: 6974 2074 7269 7669 616c 2e20 204a 7573  it trivial.  Jus
+00000930: 7420 696e 7374 616c 6c0a 7468 6520 6d61  t install.the ma
+00000940: 696e 2060 616e 6163 6f6e 6461 6020 7061  in `anaconda` pa
+00000950: 636b 6167 652e 0a0a 4966 2079 6f75 2070  ckage...If you p
+00000960: 7265 6665 7220 7468 6520 736d 616c 6c65  refer the smalle
+00000970: 7220 646f 776e 6c6f 6164 2073 697a 6520  r download size 
+00000980: 6f66 0a5b 606d 696e 6963 6f6e 6461 605d  of.[`miniconda`]
+00000990: 2868 7474 703a 2f2f 636f 6e64 612e 7079  (http://conda.py
+000009a0: 6461 7461 2e6f 7267 2f6d 696e 6963 6f6e  data.org/minicon
+000009b0: 6461 2e68 746d 6c29 2028 7768 6963 6820  da.html) (which 
+000009c0: 636f 6d65 7320 7769 7468 206e 6f0a 6578  comes with no.ex
+000009d0: 7472 6173 2062 6579 6f6e 6420 7079 7468  tras beyond pyth
+000009e0: 6f6e 292c 2079 6f75 206d 6179 2061 6c73  on), you may als
+000009f0: 6f20 6861 7665 2074 6f20 7275 6e20 7468  o have to run th
+00000a00: 6973 2063 6f6d 6d61 6e64 3a0a 0a60 6060  is command:..```
+00000a10: 7368 0a63 6f6e 6461 2069 6e73 7461 6c6c  sh.conda install
+00000a20: 2070 6970 206e 756d 7079 206e 756d 6261   pip numpy numba
+00000a30: 0a60 6060 0a0a 0a23 2320 496e 7374 616c  .```...## Instal
+00000a40: 6c61 7469 6f6e 0a0a 4173 7375 6d69 6e67  lation..Assuming
+00000a50: 2079 6f75 2075 7365 2060 636f 6e64 6160   you use `conda`
+00000a60: 2074 6f20 6d61 6e61 6765 2079 6f75 7220   to manage your 
+00000a70: 7079 7468 6f6e 2069 6e73 7461 6c6c 6174  python installat
+00000a80: 696f 6e20 286c 696b 6520 616e 7920 7361  ion (like any sa
+00000a90: 6e65 0a70 7974 686f 6e20 7573 6572 292c  ne.python user),
+00000aa0: 2079 6f75 2063 616e 2069 6e73 7461 6c6c   you can install
+00000ab0: 2074 6869 7320 7061 636b 6167 6520 7369   this package si
+00000ac0: 6d70 6c79 2061 730a 0a60 6060 7368 0a63  mply as..```sh.c
+00000ad0: 6f6e 6461 2069 6e73 7461 6c6c 202d 6320  onda install -c 
+00000ae0: 636f 6e64 612d 666f 7267 6520 7370 6865  conda-forge sphe
+00000af0: 7269 6361 6c5f 6675 6e63 7469 6f6e 730a  rical_functions.
+00000b00: 6060 600a 0a54 6869 7320 7368 6f75 6c64  ```..This should
+00000b10: 2061 7574 6f6d 6174 6963 616c 6c79 2064   automatically d
+00000b20: 6f77 6e6c 6f61 6420 616e 6420 696e 7374  ownload and inst
+00000b30: 616c 6c20 7468 6520 7061 636b 6167 650a  all the package.
+00000b40: 5b60 7175 6174 6572 6e69 6f6e 605d 2868  [`quaternion`](h
+00000b50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000b60: 6d2f 6d6f 626c 652f 7175 6174 6572 6e69  m/moble/quaterni
+00000b70: 6f6e 292c 206f 6e20 7768 6963 6820 7468  on), on which th
+00000b80: 6973 2070 6163 6b61 6765 0a64 6570 656e  is package.depen
+00000b90: 6473 2e0a 0a41 6c74 6572 6e61 7469 7665  ds...Alternative
+00000ba0: 6c79 2c20 6966 2079 6f75 2070 7265 6665  ly, if you prefe
+00000bb0: 7220 746f 2075 7365 2060 7069 7060 2028  r to use `pip` (
+00000bc0: 7768 6574 6865 7220 6f72 206e 6f74 2079  whether or not y
+00000bd0: 6f75 2075 7365 2060 636f 6e64 6160 292c  ou use `conda`),
+00000be0: 2079 6f75 0a63 616e 2061 6c73 6f20 646f   you.can also do
+00000bf0: 0a0a 6060 6073 680a 7079 7468 6f6e 202d  ..```sh.python -
+00000c00: 6d20 7069 7020 696e 7374 616c 6c20 7370  m pip install sp
+00000c10: 6865 7269 6361 6c2d 6675 6e63 7469 6f6e  herical-function
+00000c20: 730a 6060 600a 0a46 696e 616c 6c79 2c20  s.```..Finally, 
+00000c30: 7468 6572 6527 7320 616c 736f 2074 6865  there's also the
+00000c40: 2066 756c 6c79 206d 616e 7561 6c20 6f70   fully manual op
+00000c50: 7469 6f6e 206f 6620 6a75 7374 2064 6f77  tion of just dow
+00000c60: 6e6c 6f61 6469 6e67 2062 6f74 6820 636f  nloading both co
+00000c70: 6465 0a72 6570 6f73 6974 6f72 6965 732c  de.repositories,
+00000c80: 2063 6861 6e67 696e 6720 746f 2074 6865   changing to the
+00000c90: 2063 6f64 6520 6469 7265 6374 6f72 792c   code directory,
+00000ca0: 2061 6e64 2069 7373 7569 6e67 0a0a 6060   and issuing..``
+00000cb0: 6073 680a 7079 7468 6f6e 202d 6d20 7069  `sh.python -m pi
+00000cc0: 7020 696e 7374 616c 6c20 2e0a 6060 600a  p install ..```.
+00000cd0: 0a54 6869 7320 7368 6f75 6c64 2077 6f72  .This should wor
+00000ce0: 6b20 7265 6761 7264 6c65 7373 206f 6620  k regardless of 
+00000cf0: 7468 6520 696e 7374 616c 6c61 7469 6f6e  the installation
+00000d00: 206d 6574 686f 642c 2061 7320 6c6f 6e67   method, as long
+00000d10: 2061 7320 796f 7520 6861 7665 2061 0a63   as you have a.c
+00000d20: 6f6d 7069 6c65 7220 6861 6e67 696e 6720  ompiler hanging 
+00000d30: 6172 6f75 6e64 2e20 2048 6f77 6576 6572  around.  However
+00000d40: 2c20 7468 6973 206d 6179 2062 6520 6d6f  , this may be mo
+00000d50: 7265 206c 696b 656c 7920 746f 2074 7279  re likely to try
+00000d60: 2074 6f20 636f 6d70 696c 650a 7468 6520   to compile.the 
+00000d70: 6465 7065 6e64 656e 6369 6573 2c20 696e  dependencies, in
+00000d80: 636c 7564 696e 6720 6e75 6d70 7920 616e  cluding numpy an
+00000d90: 642f 6f72 2073 7069 6e73 6661 7374 2c20  d/or spinsfast, 
+00000da0: 7768 6963 6820 6361 6e20 6265 206d 7563  which can be muc
+00000db0: 6820 6d6f 7265 0a63 6f6d 706c 6963 6174  h more.complicat
+00000dc0: 6564 2e0a 0a0a 2323 2055 7361 6765 0a0a  ed....## Usage..
+00000dd0: 4669 7273 742c 2077 6520 7368 6f77 2061  First, we show a
+00000de0: 2076 6572 7920 7369 6d70 6c65 2065 7861   very simple exa
+00000df0: 6d70 6c65 206f 6620 7573 6167 6520 7769  mple of usage wi
+00000e00: 7468 2045 756c 6572 2061 6e67 6c65 732c  th Euler angles,
+00000e10: 2074 686f 7567 6820 6974 0a62 7265 616b   though it.break
+00000e20: 7320 6d79 2068 6561 7274 2074 6f20 646f  s my heart to do
+00000e30: 2073 6f3a 3c73 7570 3e5b 315d 2823 6575   so:<sup>[1](#eu
+00000e40: 6c65 722d 616e 676c 6573 2d61 7265 2d61  ler-angles-are-a
+00000e50: 7766 756c 293c 2f73 7570 3e0a 0a60 6060  wful)</sup>..```
+00000e60: 7079 7468 6f6e 0a3e 3e3e 2069 6d70 6f72  python.>>> impor
+00000e70: 7420 7370 6865 7269 6361 6c5f 6675 6e63  t spherical_func
+00000e80: 7469 6f6e 7320 6173 2073 660a 3e3e 3e20  tions as sf.>>> 
+00000e90: 616c 7068 612c 2062 6574 612c 2067 616d  alpha, beta, gam
+00000ea0: 6d61 203d 2030 2e31 2c20 302e 322c 2030  ma = 0.1, 0.2, 0
+00000eb0: 2e33 0a3e 3e3e 2065 6c6c 2c6d 702c 6d20  .3.>>> ell,mp,m 
+00000ec0: 3d20 332c 322c 310a 3e3e 3e20 7366 2e57  = 3,2,1.>>> sf.W
+00000ed0: 6967 6e65 725f 445f 656c 656d 656e 7428  igner_D_element(
+00000ee0: 616c 7068 612c 2062 6574 612c 2067 616d  alpha, beta, gam
+00000ef0: 6d61 2c20 656c 6c2c 206d 702c 206d 290a  ma, ell, mp, m).
+00000f00: 0a60 6060 0a0a 4f66 2063 6f75 7273 652c  .```..Of course,
+00000f10: 2069 7427 7320 616c 7761 7973 2062 6574   it's always bet
+00000f20: 7465 7220 746f 2075 7365 2075 6e69 7420  ter to use unit 
+00000f30: 7175 6174 6572 6e69 6f6e 7320 746f 2064  quaternions to d
+00000f40: 6573 6372 6962 6520 726f 7461 7469 6f6e  escribe rotation
+00000f50: 733a 0a0a 6060 6070 7974 686f 6e0a 3e3e  s:..```python.>>
+00000f60: 3e20 696d 706f 7274 206e 756d 7079 2061  > import numpy a
+00000f70: 7320 6e70 0a3e 3e3e 2069 6d70 6f72 7420  s np.>>> import 
+00000f80: 7175 6174 6572 6e69 6f6e 0a3e 3e3e 2052  quaternion.>>> R
+00000f90: 203d 206e 702e 7175 6174 6572 6e69 6f6e   = np.quaternion
+00000fa0: 2831 2c32 2c33 2c34 292e 6e6f 726d 616c  (1,2,3,4).normal
+00000fb0: 697a 6564 2829 0a3e 3e3e 2065 6c6c 2c6d  ized().>>> ell,m
+00000fc0: 702c 6d20 3d20 332c 322c 310a 3e3e 3e20  p,m = 3,2,1.>>> 
+00000fd0: 7366 2e57 6967 6e65 725f 445f 656c 656d  sf.Wigner_D_elem
+00000fe0: 656e 7428 522c 2065 6c6c 2c20 6d70 2c20  ent(R, ell, mp, 
+00000ff0: 6d29 0a0a 6060 600a 0a49 6620 796f 7520  m)..```..If you 
+00001000: 6e65 6564 2074 6f20 6361 6c63 756c 6174  need to calculat
+00001010: 6520 7661 6c75 6573 206f 6620 7468 6520  e values of the 
+00001020: f09d 9487 3c73 7570 3e28 e284 9329 3c2f  ....<sup>(...)</
+00001030: 7375 703e 206d 6174 7269 7820 656c 656d  sup> matrix elem
+00001040: 656e 7473 2066 6f72 206d 616e 790a 7661  ents for many.va
+00001050: 6c75 6573 206f 6620 28e2 8493 2c20 6d27  lues of (..., m'
+00001060: 2c20 6d29 2c20 6974 2069 7320 6d6f 7265  , m), it is more
+00001070: 2065 6666 6963 6965 6e74 2074 6f20 646f   efficient to do
+00001080: 2073 6f20 616c 6c20 6174 206f 6e63 652e   so all at once.
+00001090: 2020 5468 6520 666f 6c6c 6f77 696e 670a    The following.
+000010a0: 6361 6c63 756c 6174 6573 2061 6c6c 206d  calculates all m
+000010b0: 6f64 6573 2066 6f72 20e2 8493 2066 726f  odes for ... fro
+000010c0: 6d20 3220 746f 2038 2028 696e 636c 7573  m 2 to 8 (inclus
+000010d0: 6976 6529 3a0a 0a60 6060 7079 7468 6f6e  ive):..```python
+000010e0: 0a3e 3e3e 2069 6e64 6963 6573 203d 206e  .>>> indices = n
+000010f0: 702e 6172 7261 7928 5b5b 656c 6c2c 6d70  p.array([[ell,mp
+00001100: 2c6d 5d20 666f 7220 656c 6c20 696e 2072  ,m] for ell in r
+00001110: 616e 6765 2832 2c39 290a 2e2e 2e20 666f  ange(2,9).... fo
+00001120: 7220 6d70 2069 6e20 7261 6e67 6528 2d65  r mp in range(-e
+00001130: 6c6c 2c20 656c 6c2b 3129 2066 6f72 206d  ll, ell+1) for m
+00001140: 2069 6e20 7261 6e67 6528 2d65 6c6c 2c20   in range(-ell, 
+00001150: 656c 6c2b 3129 5d29 0a3e 3e3e 2073 662e  ell+1)]).>>> sf.
+00001160: 5769 676e 6572 5f44 5f65 6c65 6d65 6e74  Wigner_D_element
+00001170: 2852 2c20 696e 6469 6365 7329 0a0a 6060  (R, indices)..``
+00001180: 600a 0a46 696e 616c 6c79 2c20 6966 2079  `..Finally, if y
+00001190: 6f75 2072 6561 6c6c 7920 6e65 6564 2074  ou really need t
+000011a0: 6f20 7075 7420 7468 6520 7065 6461 6c20  o put the pedal 
+000011b0: 746f 2074 6865 206d 6574 616c 2c20 616e  to the metal, an
+000011c0: 6420 6172 6520 7769 6c6c 696e 6720 746f  d are willing to
+000011d0: 0a67 7561 7261 6e74 6565 2074 6861 7420  .guarantee that 
+000011e0: 7468 6520 696e 7075 7420 6172 6775 6d65  the input argume
+000011f0: 6e74 7320 6172 6520 636f 7272 6563 742c  nts are correct,
+00001200: 2079 6f75 2063 616e 2075 7365 2061 2073   you can use a s
+00001210: 7065 6369 616c 2068 6964 6465 6e0a 666f  pecial hidden.fo
+00001220: 726d 206f 6620 7468 6520 6675 6e63 7469  rm of the functi
+00001230: 6f6e 3a0a 0a60 6060 7079 7468 6f6e 0a3e  on:..```python.>
+00001240: 3e3e 2073 662e 5f57 6967 6e65 725f 445f  >> sf._Wigner_D_
+00001250: 656c 656d 656e 7428 522e 612c 2052 2e62  element(R.a, R.b
+00001260: 2c20 696e 6469 6365 732c 2065 6c65 6d65  , indices, eleme
+00001270: 6e74 7329 0a0a 6060 600a 0a48 6572 652c  nts)..```..Here,
+00001280: 2060 522e 6160 2061 6e64 2060 522e 6260   `R.a` and `R.b`
+00001290: 2061 7265 2074 6865 2074 776f 2063 6f6d   are the two com
+000012a0: 706c 6578 2070 6172 7473 206f 6620 7468  plex parts of th
+000012b0: 6520 7175 6174 6572 6e69 6f6e 2064 6566  e quaternion def
+000012c0: 696e 6564 206f 6e0a 5b74 6869 7320 7061  ined on.[this pa
+000012d0: 6765 5d28 6874 7470 3a2f 2f6d 6f62 6c65  ge](http://moble
+000012e0: 2e67 6974 6875 622e 696f 2f73 7068 6572  .github.io/spher
+000012f0: 6963 616c 5f66 756e 6374 696f 6e73 2f29  ical_functions/)
+00001300: 2028 7468 6f75 6768 2074 6865 2075 7365   (though the use
+00001310: 7220 6e65 6564 0a6e 6f74 2063 6172 6520  r need.not care 
+00001320: 6162 6f75 7420 7468 6174 292e 2020 5468  about that).  Th
+00001330: 6520 6069 6e64 6963 6573 6020 7661 7269  e `indices` vari
+00001340: 6162 6c65 2069 7320 6173 7375 6d65 6420  able is assumed 
+00001350: 746f 2062 6520 610a 7477 6f2d 6469 6d65  to be a.two-dime
+00001360: 6e73 696f 6e61 6c20 6172 7261 7920 6f66  nsional array of
+00001370: 2069 6e74 6567 6572 732c 2077 6865 7265   integers, where
+00001380: 2074 6865 2073 6563 6f6e 6420 6469 6d65   the second dime
+00001390: 6e73 696f 6e20 6861 7320 7369 7a65 2074  nsion has size t
+000013a0: 6872 6565 2c0a 7265 7072 6573 656e 7469  hree,.representi
+000013b0: 6e67 2074 6865 2028 e284 932c 206d 272c  ng the (..., m',
+000013c0: 206d 2920 696e 6469 6365 732e 2020 5468   m) indices.  Th
+000013d0: 6973 2061 766f 6964 7320 6365 7274 6169  is avoids certai
+000013e0: 6e20 736f 6d65 7768 6174 2073 6c6f 7765  n somewhat slowe
+000013f0: 720a 7075 7265 2d70 7974 686f 6e20 6f70  r.pure-python op
+00001400: 6572 6174 696f 6e73 2069 6e76 6f6c 7669  erations involvi
+00001410: 6e67 2061 7267 756d 656e 7420 6368 6563  ng argument chec
+00001420: 6b69 6e67 2c20 7265 7368 6170 696e 672c  king, reshaping,
+00001430: 2065 7463 2e20 2054 6865 0a60 656c 656d   etc.  The.`elem
+00001440: 656e 7473 6020 7661 7269 6162 6c65 206d  ents` variable m
+00001450: 7573 7420 6265 2061 206f 6e65 2d64 696d  ust be a one-dim
+00001460: 656e 7369 6f6e 616c 2061 7272 6179 206f  ensional array o
+00001470: 6620 636f 6d70 6c65 7820 6e75 6d62 6572  f complex number
+00001480: 7320 2863 616e 2062 650a 756e 696e 6974  s (can be.uninit
+00001490: 6961 6c69 7a65 6429 2c20 7768 6963 6820  ialized), which 
+000014a0: 7769 6c6c 2062 6520 7265 706c 6163 6564  will be replaced
+000014b0: 2077 6974 6820 7468 6520 636f 7272 6573   with the corres
+000014c0: 706f 6e64 696e 6720 7661 6c75 6573 206f  ponding values o
+000014d0: 6e20 7265 7475 726e 2e0a 4167 6169 6e2c  n return..Again,
+000014e0: 2068 6f77 6576 6572 2c20 7468 6572 6520   however, there 
+000014f0: 6973 206e 6f20 696e 7075 7420 6469 6d65  is no input dime
+00001500: 6e73 696f 6e20 6368 6563 6b69 6e67 2068  nsion checking h
+00001510: 6572 652c 2073 6f20 6966 2079 6f75 2067  ere, so if you g
+00001520: 6976 6520 6261 640a 696e 7075 7473 2c20  ive bad.inputs, 
+00001530: 6265 6861 7669 6f72 2063 6f75 6c64 2072  behavior could r
+00001540: 616e 6765 2066 726f 6d20 7369 6c65 6e74  ange from silent
+00001550: 6c79 2077 726f 6e67 2074 6f20 6578 6365  ly wrong to exce
+00001560: 7074 696f 6e73 2074 6f20 7365 676d 656e  ptions to segmen
+00001570: 7461 7469 6f6e 0a66 6175 6c74 732e 2020  tation.faults.  
+00001580: 4361 7665 6174 2065 6d70 746f 722e 0a0a  Caveat emptor...
+00001590: 0a23 2320 4163 6b6e 6f77 6c65 6467 6d65  .## Acknowledgme
+000015a0: 6e74 730a 0a49 2076 6572 7920 6d75 6368  nts..I very much
+000015b0: 2061 7070 7265 6369 6174 6520 4261 7272   appreciate Barr
+000015c0: 7920 5761 7264 656c 6c27 7320 6865 6c70  y Wardell's help
+000015d0: 2069 6e20 736f 7274 696e 6720 6f75 7420   in sorting out 
+000015e0: 7468 6520 7265 6c61 7469 6f6e 7368 6970  the relationship
+000015f0: 730a 6265 7477 6565 6e20 6d79 2063 6f6e  s.between my con
+00001600: 7665 6e74 696f 6e73 2061 6e64 2074 686f  ventions and tho
+00001610: 7365 206f 6620 6f74 6865 7220 7065 6f70  se of other peop
+00001620: 6c65 2061 6e64 2073 6f66 7477 6172 6520  le and software 
+00001630: 7061 636b 6167 6573 0a28 6573 7065 6369  packages.(especi
+00001640: 616c 6c79 204d 6174 6865 6d61 7469 6361  ally Mathematica
+00001650: 2773 2063 7261 7a79 2063 6f6e 7665 6e74  's crazy convent
+00001660: 696f 6e73 292e 0a0a 5468 6973 2063 6f64  ions)...This cod
+00001670: 6520 6973 2c20 6f66 2063 6f75 7273 652c  e is, of course,
+00001680: 2068 6f73 7465 6420 6f6e 2067 6974 6875   hosted on githu
+00001690: 622e 2020 4265 6361 7573 6520 6974 2069  b.  Because it i
+000016a0: 7320 616e 206f 7065 6e2d 736f 7572 6365  s an open-source
+000016b0: 0a70 726f 6a65 6374 2c20 7468 6520 686f  .project, the ho
+000016c0: 7374 696e 6720 6973 2066 7265 652c 2061  sting is free, a
+000016d0: 6e64 2061 6c6c 2074 6865 2077 6f6e 6465  nd all the wonde
+000016e0: 7266 756c 2066 6561 7475 7265 7320 6f66  rful features of
+000016f0: 2067 6974 6875 6220 6172 650a 6176 6169   github are.avai
+00001700: 6c61 626c 652c 2069 6e63 6c75 6469 6e67  lable, including
+00001710: 2066 7265 6520 7769 6b69 2073 7061 6365   free wiki space
+00001720: 2061 6e64 2077 6562 2070 6167 6520 686f   and web page ho
+00001730: 7374 696e 672c 2070 756c 6c20 7265 7175  sting, pull requ
+00001740: 6573 7473 2c20 610a 6e69 6365 2069 6e74  ests, a.nice int
+00001750: 6572 6661 6365 2074 6f20 7468 6520 6769  erface to the gi
+00001760: 7420 6c6f 6773 2c20 6574 632e 0a0a 4669  t logs, etc...Fi
+00001770: 6e61 6c6c 792c 2074 6865 2063 6f64 6520  nally, the code 
+00001780: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
+00001790: 2063 6f6d 7069 6c65 642c 2061 6e64 2074   compiled, and t
+000017a0: 6865 2062 696e 6172 6965 7320 686f 7374  he binaries host
+000017b0: 6564 2066 6f72 0a64 6f77 6e6c 6f61 6420  ed for.download 
+000017c0: 6279 2060 636f 6e64 6160 206f 6e20 5b61  by `conda` on [a
+000017d0: 6e61 636f 6e64 612e 6f72 675d 2868 7474  naconda.org](htt
+000017e0: 7073 3a2f 2f61 6e61 636f 6e64 612e 6f72  ps://anaconda.or
+000017f0: 672f 6d6f 626c 652f 7370 6865 7269 6361  g/moble/spherica
+00001800: 6c5f 6675 6e63 7469 6f6e 7329 2e0a 5468  l_functions)..Th
+00001810: 6973 2069 7320 616c 736f 2061 2066 7265  is is also a fre
+00001820: 6520 7365 7276 6963 6520 666f 7220 6f70  e service for op
+00001830: 656e 2d73 6f75 7263 6520 7072 6f6a 6563  en-source projec
+00001840: 7473 206c 696b 6520 7468 6973 206f 6e65  ts like this one
+00001850: 2e0a 0a54 6865 2077 6f72 6b20 6f66 2063  ...The work of c
+00001860: 7265 6174 696e 6720 7468 6973 2063 6f64  reating this cod
+00001870: 6520 7761 7320 7375 7070 6f72 7465 6420  e was supported 
+00001880: 696e 2070 6172 7420 6279 2074 6865 2053  in part by the S
+00001890: 6865 726d 616e 2046 6169 7263 6869 6c64  herman Fairchild
+000018a0: 0a46 6f75 6e64 6174 696f 6e20 616e 6420  .Foundation and 
+000018b0: 6279 204e 5346 2047 7261 6e74 7320 4e6f  by NSF Grants No
+000018c0: 2e20 5048 592d 3133 3036 3132 3520 616e  . PHY-1306125 an
+000018d0: 6420 4153 542d 3133 3333 3132 392e 0a0a  d AST-1333129...
+000018e0: 0a3c 6272 2f3e 0a2d 2d2d 0a23 2323 2323  .<br/>.---.#####
+000018f0: 2320 3c73 7570 3e31 3c2f 7375 703e 2045  # <sup>1</sup> E
+00001900: 756c 6572 2061 6e67 6c65 7320 6172 6520  uler angles are 
+00001910: 6177 6675 6c0a 0a45 756c 6572 2061 6e67  awful..Euler ang
+00001920: 6c65 7320 6172 6520 7072 6574 7479 206d  les are pretty m
+00001930: 7563 680a 5b74 6865 2077 6f72 7374 2074  uch.[the worst t
+00001940: 6869 6e67 7320 6576 6572 5d28 6874 7470  hings ever](http
+00001950: 3a2f 2f6d 6f62 6c65 2e67 6974 6875 622e  ://moble.github.
+00001960: 696f 2f73 7068 6572 6963 616c 5f66 756e  io/spherical_fun
+00001970: 6374 696f 6e73 2f23 6575 6c65 722d 616e  ctions/#euler-an
+00001980: 676c 6573 290a 616e 6420 6974 206d 616b  gles).and it mak
+00001990: 6573 206d 6520 6665 656c 2062 6164 2065  es me feel bad e
+000019a0: 7665 6e20 7375 7070 6f72 7469 6e67 2074  ven supporting t
+000019b0: 6865 6d2e 2020 5175 6174 6572 6e69 6f6e  hem.  Quaternion
+000019c0: 7320 6172 650a 6661 7374 6572 2c20 6d6f  s are.faster, mo
+000019d0: 7265 2061 6363 7572 6174 652c 2062 6173  re accurate, bas
+000019e0: 6963 616c 6c79 2066 7265 6520 6f66 2073  ically free of s
+000019f0: 696e 6775 6c61 7269 7469 6573 2c20 6d6f  ingularities, mo
+00001a00: 7265 0a69 6e74 7569 7469 7665 2c20 616e  re.intuitive, an
+00001a10: 6420 6765 6e65 7261 6c6c 7920 6561 7369  d generally easi
+00001a20: 6572 2074 6f20 756e 6465 7273 7461 6e64  er to understand
+00001a30: 2e20 2059 6f75 2063 616e 2077 6f72 6b20  .  You can work 
+00001a40: 656e 7469 7265 6c79 0a77 6974 686f 7574  entirely.without
+00001a50: 2045 756c 6572 2061 6e67 6c65 7320 2849   Euler angles (I
+00001a60: 2063 6572 7461 696e 6c79 2064 6f29 2e20   certainly do). 
+00001a70: 2059 6f75 2061 6273 6f6c 7574 656c 7920   You absolutely 
+00001a80: 6e65 7665 7220 6e65 6564 0a74 6865 6d2e  never need.them.
+00001a90: 2020 4275 7420 6966 2079 6f75 2772 6520    But if you're 
+00001aa0: 736f 206f 6c64 2066 6173 6869 6f6e 6564  so old fashioned
+00001ab0: 2074 6861 7420 796f 7520 7265 616c 6c79   that you really
+00001ac0: 2063 616e 2774 2067 6976 6520 7468 656d   can't give them
+00001ad0: 0a75 702c 2074 6865 7920 6172 6520 6675  .up, they are fu
+00001ae0: 6c6c 7920 7375 7070 6f72 7465 642e 0a    lly supported..
```

### Comparing `spherical-functions-2022.4.1/pyproject.toml` & `spherical_functions-2022.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "spherical-functions"
 description = "Python/numba implementation of Wigner D Matrices, spin-weighted spherical harmonics, and associated functions"
-version = "2022.4.1"
+version = "2022.4.2"
 readme = "README.md"
 license = "MIT"
 authors = ["Michael Boyle <mob22@cornell.edu>"]
 homepage = "https://github.com/moble/spherical_functions"
 packages = [{include = "spherical_functions" }]
 include = ["spherical_functions/*.npy"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 numpy = ">=1.20"
 scipy = "^1.0"
 numba = ">=0.55"
 numpy-quaternion = ">=2022"
-spinsfast = "^2022"
+spinsfast = ">=2022"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = ">=2.10.1"
 black = ">=22.1"
 sympy = ">=1.10"
 line-profiler = ">=3.5.0"
```

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH/__init__.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH_grids/__init__.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH_grids/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH_grids/algebra.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH_grids/algebra.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH_grids/ufuncs.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH_grids/ufuncs.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH_grids/utilities.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH_grids/utilities.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH_modes/__init__.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH_modes/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH_modes/algebra.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH_modes/algebra.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH_modes/derivatives.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH_modes/derivatives.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH_modes/ufuncs.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH_modes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/SWSH_modes/utilities.py` & `spherical_functions-2022.4.2/spherical_functions/SWSH_modes/utilities.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/WignerD/WignerDRecursion.py` & `spherical_functions-2022.4.2/spherical_functions/WignerD/WignerDRecursion.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/WignerD/__init__.py` & `spherical_functions-2022.4.2/spherical_functions/WignerD/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/Wigner_coefficients.npy` & `spherical_functions-2022.4.2/spherical_functions/Wigner_coefficients.npy`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/__init__.py` & `spherical_functions-2022.4.2/spherical_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/_generate_coefficients.py` & `spherical_functions-2022.4.2/spherical_functions/_generate_coefficients.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/binomial_coefficients.npy` & `spherical_functions-2022.4.2/spherical_functions/binomial_coefficients.npy`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/ladder_operator_coefficients.npy` & `spherical_functions-2022.4.2/spherical_functions/ladder_operator_coefficients.npy`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/mode_conversions.py` & `spherical_functions-2022.4.2/spherical_functions/mode_conversions.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/multiplication.py` & `spherical_functions-2022.4.2/spherical_functions/multiplication.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/recursions/__init__.py` & `spherical_functions-2022.4.2/spherical_functions/recursions/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/recursions/associated_legendre_functions.py` & `spherical_functions-2022.4.2/spherical_functions/recursions/associated_legendre_functions.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/recursions/complex_powers.py` & `spherical_functions-2022.4.2/spherical_functions/recursions/complex_powers.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/recursions/wigner3j.py` & `spherical_functions-2022.4.2/spherical_functions/recursions/wigner3j.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/spherical_functions/recursions/wignerH.py` & `spherical_functions-2022.4.2/spherical_functions/recursions/wignerH.py`

 * *Files identical despite different names*

### Comparing `spherical-functions-2022.4.1/setup.py` & `spherical_functions-2022.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,541 +1,484 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2773 7068 6572 6963 616c 5f66   \.['spherical_f
-00000050: 756e 6374 696f 6e73 272c 0a20 2773 7068  unctions',. 'sph
-00000060: 6572 6963 616c 5f66 756e 6374 696f 6e73  erical_functions
-00000070: 2e53 5753 4827 2c0a 2027 7370 6865 7269  .SWSH',. 'spheri
-00000080: 6361 6c5f 6675 6e63 7469 6f6e 732e 5357  cal_functions.SW
-00000090: 5348 5f67 7269 6473 272c 0a20 2773 7068  SH_grids',. 'sph
-000000a0: 6572 6963 616c 5f66 756e 6374 696f 6e73  erical_functions
-000000b0: 2e53 5753 485f 6d6f 6465 7327 2c0a 2027  .SWSH_modes',. '
-000000c0: 7370 6865 7269 6361 6c5f 6675 6e63 7469  spherical_functi
-000000d0: 6f6e 732e 5769 676e 6572 4427 2c0a 2027  ons.WignerD',. '
-000000e0: 7370 6865 7269 6361 6c5f 6675 6e63 7469  spherical_functi
-000000f0: 6f6e 732e 7265 6375 7273 696f 6e73 275d  ons.recursions']
-00000100: 0a0a 7061 636b 6167 655f 6461 7461 203d  ..package_data =
-00000110: 205c 0a7b 2727 3a20 5b27 2a27 5d7d 0a0a   \.{'': ['*']}..
-00000120: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000130: 203d 205c 0a5b 276e 756d 6261 3e3d 302e   = \.['numba>=0.
-00000140: 3535 272c 0a20 276e 756d 7079 2d71 7561  55',. 'numpy-qua
-00000150: 7465 726e 696f 6e3e 3d32 3032 3227 2c0a  ternion>=2022',.
-00000160: 2027 6e75 6d70 793e 3d31 2e32 3027 2c0a   'numpy>=1.20',.
-00000170: 2027 7363 6970 793e 3d31 2e30 2c3c 322e   'scipy>=1.0,<2.
-00000180: 3027 2c0a 2027 7370 696e 7366 6173 743e  0',. 'spinsfast>
-00000190: 3d32 3032 322c 3c32 3032 3327 5d0a 0a73  =2022,<2023']..s
-000001a0: 6574 7570 5f6b 7761 7267 7320 3d20 7b0a  etup_kwargs = {.
-000001b0: 2020 2020 276e 616d 6527 3a20 2773 7068      'name': 'sph
-000001c0: 6572 6963 616c 2d66 756e 6374 696f 6e73  erical-functions
-000001d0: 272c 0a20 2020 2027 7665 7273 696f 6e27  ',.    'version'
-000001e0: 3a20 2732 3032 322e 342e 3127 2c0a 2020  : '2022.4.1',.  
-000001f0: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
-00000200: 2027 5079 7468 6f6e 2f6e 756d 6261 2069   'Python/numba i
-00000210: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
-00000220: 2057 6967 6e65 7220 4420 4d61 7472 6963   Wigner D Matric
-00000230: 6573 2c20 7370 696e 2d77 6569 6768 7465  es, spin-weighte
-00000240: 6420 7370 6865 7269 6361 6c20 6861 726d  d spherical harm
-00000250: 6f6e 6963 732c 2061 6e64 2061 7373 6f63  onics, and assoc
-00000260: 6961 7465 6420 6675 6e63 7469 6f6e 7327  iated functions'
-00000270: 2c0a 2020 2020 276c 6f6e 675f 6465 7363  ,.    'long_desc
-00000280: 7269 7074 696f 6e27 3a20 2723 2053 7068  ription': '# Sph
-00000290: 6572 6963 616c 2046 756e 6374 696f 6e73  erical Functions
-000002a0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000002b0: 2f2f 7472 6176 6973 2d63 692e 6f72 672f  //travis-ci.org/
-000002c0: 6d6f 626c 652f 7370 6865 7269 6361 6c5f  moble/spherical_
-000002d0: 6675 6e63 7469 6f6e 7322 3e3c 696d 6720  functions"><img 
-000002e0: 616c 6967 6e3d 2272 6967 6874 2220 6873  align="right" hs
-000002f0: 7061 6365 3d22 3322 2061 6c74 3d22 5374  pace="3" alt="St
-00000300: 6174 7573 206f 6620 6175 746f 6d61 7469  atus of automati
-00000310: 6320 6275 696c 6420 616e 6420 7465 7374  c build and test
-00000320: 2073 7569 7465 2220 7372 633d 2268 7474   suite" src="htt
-00000330: 7073 3a2f 2f74 7261 7669 732d 6369 2e6f  ps://travis-ci.o
-00000340: 7267 2f6d 6f62 6c65 2f73 7068 6572 6963  rg/moble/spheric
-00000350: 616c 5f66 756e 6374 696f 6e73 2e73 7667  al_functions.svg
-00000360: 3f62 7261 6e63 683d 6d61 7374 6572 223e  ?branch=master">
-00000370: 3c2f 613e 203c 6120 6872 6566 3d22 6874  </a> <a href="ht
-00000380: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000390: 2f6d 6f62 6c65 2f73 7068 6572 6963 616c  /moble/spherical
-000003a0: 5f66 756e 6374 696f 6e73 2f62 6c6f 622f  _functions/blob/
-000003b0: 6d61 7374 6572 2f4c 4943 454e 5345 223e  master/LICENSE">
-000003c0: 3c69 6d67 2061 6c69 676e 3d22 7269 6768  <img align="righ
-000003d0: 7422 2068 7370 6163 653d 2233 2220 616c  t" hspace="3" al
-000003e0: 743d 224d 4954 206c 6963 656e 7365 2220  t="MIT license" 
-000003f0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000400: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000410: 7562 2f6c 6963 656e 7365 2f6d 6f62 6c65  ub/license/moble
-00000420: 2f6f 7574 5f6f 665f 636f 7265 5f66 6674  /out_of_core_fft
-00000430: 2e73 7667 223e 3c2f 613e 5c6e 5c6e 7c20  .svg"></a>\n\n| 
-00000440: 4e4f 5445 3a20 5468 6973 2070 6163 6b61  NOTE: This packa
-00000450: 6765 2077 696c 6c20 7374 696c 6c20 6265  ge will still be
-00000460: 206d 6169 6e74 6169 6e65 642c 2062 7574   maintained, but
-00000470: 202a 6163 7469 7665 2a20 6465 7665 6c6f   *active* develo
-00000480: 706d 656e 7420 6861 7320 6d6f 7665 6420  pment has moved 
-00000490: 746f 2074 6865 205b 6073 7068 6572 6963  to the [`spheric
-000004a0: 616c 605d 2868 7474 7073 3a2f 2f67 6974  al`](https://git
-000004b0: 6875 622e 636f 6d2f 6d6f 626c 652f 7370  hub.com/moble/sp
-000004c0: 6865 7269 6361 6c29 2070 6163 6b61 6765  herical) package
-000004d0: 2e20 2057 6869 6c65 2074 6869 7320 7061  .  While this pa
-000004e0: 636b 6167 6520 776f 726b 7320 7765 6c6c  ckage works well
-000004f0: 2066 6f72 20e2 8493 2028 616b 6120 656c   for ... (aka el
-00000500: 6c2c 204c 2c20 6a2c 206f 7220 4a29 2076  l, L, j, or J) v
-00000510: 616c 7565 7320 7570 2074 6f20 6172 6f75  alues up to arou
-00000520: 6e64 2032 352c 2065 7272 6f72 7320 7374  nd 25, errors st
-00000530: 6172 7420 746f 2062 7569 6c64 2072 6170  art to build rap
-00000540: 6964 6c79 2061 6e64 2074 7572 6e20 696e  idly and turn in
-00000550: 746f 204e 614e 7320 6172 6f75 6e64 2033  to NaNs around 3
-00000560: 302e 2020 5468 6520 6073 7068 6572 6963  0.  The `spheric
-00000570: 616c 6020 7061 636b 6167 6520 6361 6e20  al` package can 
-00000580: 7265 6164 696c 7920 6861 6e64 6c65 2076  readily handle v
-00000590: 616c 7565 7320 7570 2074 6f20 6174 206c  alues up to at l
-000005a0: 6561 7374 2031 3030 302c 2077 6974 6820  east 1000, with 
-000005b0: 6163 6375 7261 6379 2063 6c6f 7365 2074  accuracy close t
-000005c0: 6f20 e284 9320 7469 6d65 7320 6d61 6368  o ... times mach
-000005d0: 696e 6520 7072 6563 6973 696f 6e2e 2020  ine precision.  
-000005e0: e280 944d 696b 6520 7c5c 6e7c 202d 2d2d  ...Mike |\n| ---
-000005f0: 207c 5c6e 5c6e 5c6e 5079 7468 6f6e 2f6e   |\n\n\nPython/n
-00000600: 756d 6261 2070 6163 6b61 6765 2066 6f72  umba package for
-00000610: 2065 7661 6c75 6174 696e 6720 616e 6420   evaluating and 
-00000620: 7472 616e 7366 6f72 6d69 6e67 2057 6967  transforming Wig
-00000630: 6e65 725c 2773 20f0 9d94 8720 6d61 7472  ner\'s .... matr
-00000640: 6963 6573 2c5c 6e57 6967 6e65 725c 2773  ices,\nWigner\'s
-00000650: 2033 2d6a 2073 796d 626f 6c73 2c20 616e   3-j symbols, an
-00000660: 6420 7370 696e 2d77 6569 6768 7465 6420  d spin-weighted 
-00000670: 2861 6e64 2073 6361 6c61 7229 2073 7068  (and scalar) sph
-00000680: 6572 6963 616c 2068 6172 6d6f 6e69 6373  erical harmonics
-00000690: 2e5c 6e54 6865 7365 2066 756e 6374 696f  .\nThese functio
-000006a0: 6e73 2061 7265 2065 7661 6c75 6174 6564  ns are evaluated
-000006b0: 2064 6972 6563 746c 7920 696e 2074 6572   directly in ter
-000006c0: 6d73 206f 6620 7175 6174 6572 6e69 6f6e  ms of quaternion
-000006d0: 732c 2061 7320 7765 6c6c 2061 7320 696e  s, as well as in
-000006e0: 5c6e 7468 6520 6d6f 7265 2073 7461 6e64  \nthe more stand
-000006f0: 6172 6420 666f 726d 7320 6f66 2073 7068  ard forms of sph
-00000700: 6572 6963 616c 2063 6f6f 7264 696e 6174  erical coordinat
-00000710: 6573 2061 6e64 2045 756c 6572 5c6e 616e  es and Euler\nan
-00000720: 676c 6573 2e3c 7375 703e 5b31 5d28 2331  gles.<sup>[1](#1
-00000730: 2d65 756c 6572 2d61 6e67 6c65 732d 6172  -euler-angles-ar
-00000740: 652d 6177 6675 6c29 3c2f 7375 703e 5c6e  e-awful)</sup>\n
-00000750: 5c6e 5468 6520 636f 6e76 656e 7469 6f6e  \nThe convention
-00000760: 7320 666f 7220 7468 6973 2070 6163 6b61  s for this packa
-00000770: 6765 2061 7265 2064 6573 6372 6962 6564  ge are described
-00000780: 2069 6e20 6465 7461 696c 206f 6e5c 6e5b   in detail on\n[
-00000790: 7468 6973 2070 6167 655d 2868 7474 703a  this page](http:
-000007a0: 2f2f 6d6f 626c 652e 6769 7468 7562 2e69  //moble.github.i
-000007b0: 6f2f 7370 6865 7269 6361 6c5f 6675 6e63  o/spherical_func
-000007c0: 7469 6f6e 732f 292e 5c6e 5c6e 2323 2044  tions/).\n\n## D
-000007d0: 6570 656e 6465 6e63 6965 735c 6e5c 6e54  ependencies\n\nT
-000007e0: 6865 206f 6e6c 7920 7472 7565 2072 6571  he only true req
-000007f0: 7569 7265 6d65 6e74 7320 666f 7220 7468  uirements for th
-00000800: 6973 2063 6f64 6520 6172 6520 6070 7974  is code are `pyt
-00000810: 686f 6e60 2061 6e64 2074 6865 2070 7974  hon` and the pyt
-00000820: 686f 6e20 7061 636b 6167 655c 6e60 6e75  hon package\n`nu
-00000830: 6d70 7960 2c20 6173 2077 656c 6c20 6173  mpy`, as well as
-00000840: 206d 7920 6163 636f 6d70 616e 7969 6e67   my accompanying
-00000850: 5c6e 5b60 7175 6174 6572 6e69 6f6e 605d  \n[`quaternion`]
-00000860: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000870: 636f 6d2f 6d6f 626c 652f 7175 6174 6572  com/moble/quater
-00000880: 6e69 6f6e 2920 7061 636b 6167 6520 2869  nion) package (i
-00000890: 6e73 7461 6c6c 6174 696f 6e20 6f66 5c6e  nstallation of\n
-000008a0: 7768 6963 6820 6973 2073 686f 776e 2062  which is shown b
-000008b0: 656c 6f77 292e 5c6e 5c6e 486f 7765 7665  elow).\n\nHoweve
-000008c0: 722c 2074 6869 7320 7061 636b 6167 6520  r, this package 
-000008d0: 6361 6e20 6175 746f 6d61 7469 6361 6c6c  can automaticall
-000008e0: 7920 7573 655c 6e5b 606e 756d 6261 605d  y use\n[`numba`]
-000008f0: 2868 7474 703a 2f2f 6e75 6d62 612e 7079  (http://numba.py
-00000900: 6461 7461 2e6f 7267 2f29 2c20 7768 6963  data.org/), whic
-00000910: 6820 7573 6573 205b 4c4c 564d 5d28 6874  h uses [LLVM](ht
-00000920: 7470 3a2f 2f6c 6c76 6d2e 6f72 672f 2920  tp://llvm.org/) 
-00000930: 746f 5c6e 636f 6d70 696c 6520 7079 7468  to\ncompile pyth
-00000940: 6f6e 2063 6f64 6520 746f 206d 6163 6869  on code to machi
-00000950: 6e65 2063 6f64 652c 2061 6363 656c 6572  ne code, acceler
-00000960: 6174 696e 6720 6d6f 7374 206e 756d 6572  ating most numer
-00000970: 6963 616c 2066 756e 6374 696f 6e73 2062  ical functions b
-00000980: 795c 6e66 6163 746f 7273 206f 6620 616e  y\nfactors of an
-00000990: 7977 6865 7265 2066 726f 6d20 3220 746f  ywhere from 2 to
-000009a0: 2032 3030 302e 2020 4974 2069 7320 2a70   2000.  It is *p
-000009b0: 6f73 7369 626c 652a 2074 6f20 7275 6e20  ossible* to run 
-000009c0: 7468 6520 636f 6465 2077 6974 686f 7574  the code without
-000009d0: 5c6e 606e 756d 6261 602c 2062 7574 2074  \n`numba`, but t
-000009e0: 6865 206d 6f73 7420 696d 706f 7274 616e  he most importan
-000009f0: 7420 6675 6e63 7469 6f6e 7320 6172 6520  t functions are 
-00000a00: 726f 7567 686c 7920 3130 2074 696d 6573  roughly 10 times
-00000a10: 2073 6c6f 7765 7220 7769 7468 6f75 745c   slower without\
-00000a20: 6e69 742e 5c6e 5c6e 5468 6520 6f6e 6c79  nit.\n\nThe only
-00000a30: 2064 7261 7762 6163 6b20 6f66 2060 6e75   drawback of `nu
-00000a40: 6d62 6160 2069 7320 7468 6174 2069 7420  mba` is that it 
-00000a50: 6973 206e 6f6e 7472 6976 6961 6c20 746f  is nontrivial to
-00000a60: 2069 6e73 7461 6c6c 206f 6e20 6974 7320   install on its 
-00000a70: 6f77 6e2e 5c6e 466f 7274 756e 6174 656c  own.\nFortunatel
-00000a80: 792c 2074 6865 2062 6573 7420 7079 7468  y, the best pyth
-00000a90: 6f6e 2069 6e73 7461 6c6c 6572 2c5c 6e5b  on installer,\n[
-00000aa0: 6061 6e61 636f 6e64 6160 5d28 6874 7470  `anaconda`](http
-00000ab0: 3a2f 2f63 6f6e 7469 6e75 756d 2e69 6f2f  ://continuum.io/
-00000ac0: 646f 776e 6c6f 6164 7329 2c20 6d61 6b65  downloads), make
-00000ad0: 7320 6974 2074 7269 7669 616c 2e20 204a  s it trivial.  J
-00000ae0: 7573 7420 696e 7374 616c 6c5c 6e74 6865  ust install\nthe
-00000af0: 206d 6169 6e20 6061 6e61 636f 6e64 6160   main `anaconda`
-00000b00: 2070 6163 6b61 6765 2e5c 6e5c 6e49 6620   package.\n\nIf 
-00000b10: 796f 7520 7072 6566 6572 2074 6865 2073  you prefer the s
-00000b20: 6d61 6c6c 6572 2064 6f77 6e6c 6f61 6420  maller download 
-00000b30: 7369 7a65 206f 665c 6e5b 606d 696e 6963  size of\n[`minic
-00000b40: 6f6e 6461 605d 2868 7474 703a 2f2f 636f  onda`](http://co
-00000b50: 6e64 612e 7079 6461 7461 2e6f 7267 2f6d  nda.pydata.org/m
-00000b60: 696e 6963 6f6e 6461 2e68 746d 6c29 2028  iniconda.html) (
-00000b70: 7768 6963 6820 636f 6d65 7320 7769 7468  which comes with
-00000b80: 206e 6f5c 6e65 7874 7261 7320 6265 796f   no\nextras beyo
-00000b90: 6e64 2070 7974 686f 6e29 2c20 796f 755c  nd python), you\
-00000ba0: 276c 6c20 616c 736f 2068 6176 6520 746f  'll also have to
-00000bb0: 2072 756e 2074 6869 7320 636f 6d6d 616e   run this comman
-00000bc0: 643a 5c6e 5c6e 6060 6073 685c 6e63 6f6e  d:\n\n```sh\ncon
-00000bd0: 6461 2069 6e73 7461 6c6c 2070 6970 206e  da install pip n
-00000be0: 756d 7079 206e 756d 6261 5c6e 6060 605c  umpy numba\n```\
-00000bf0: 6e5c 6e5c 6e23 2320 496e 7374 616c 6c61  n\n\n## Installa
-00000c00: 7469 6f6e 5c6e 5c6e 4173 7375 6d69 6e67  tion\n\nAssuming
-00000c10: 2079 6f75 2075 7365 2060 636f 6e64 6160   you use `conda`
-00000c20: 2074 6f20 6d61 6e61 6765 2079 6f75 7220   to manage your 
-00000c30: 7079 7468 6f6e 2069 6e73 7461 6c6c 6174  python installat
-00000c40: 696f 6e20 286c 696b 6520 616e 7920 7361  ion (like any sa
-00000c50: 6e65 5c6e 7079 7468 6f6e 2075 7365 7229  ne\npython user)
-00000c60: 2c20 796f 7520 6361 6e20 696e 7374 616c  , you can instal
-00000c70: 6c20 7468 6973 2070 6163 6b61 6765 2073  l this package s
-00000c80: 696d 706c 7920 6173 5c6e 5c6e 6060 6073  imply as\n\n```s
-00000c90: 685c 6e63 6f6e 6461 2069 6e73 7461 6c6c  h\nconda install
-00000ca0: 202d 6320 636f 6e64 612d 666f 7267 6520   -c conda-forge 
-00000cb0: 7370 6865 7269 6361 6c5f 6675 6e63 7469  spherical_functi
-00000cc0: 6f6e 735c 6e60 6060 5c6e 5c6e 5468 6973  ons\n```\n\nThis
-00000cd0: 2073 686f 756c 6420 6175 746f 6d61 7469   should automati
-00000ce0: 6361 6c6c 7920 646f 776e 6c6f 6164 2061  cally download a
-00000cf0: 6e64 2069 6e73 7461 6c6c 2074 6865 2070  nd install the p
-00000d00: 6163 6b61 6765 5c6e 5b60 7175 6174 6572  ackage\n[`quater
-00000d10: 6e69 6f6e 605d 2868 7474 7073 3a2f 2f67  nion`](https://g
-00000d20: 6974 6875 622e 636f 6d2f 6d6f 626c 652f  ithub.com/moble/
-00000d30: 7175 6174 6572 6e69 6f6e 292c 206f 6e20  quaternion), on 
-00000d40: 7768 6963 6820 7468 6973 2070 6163 6b61  which this packa
-00000d50: 6765 5c6e 6465 7065 6e64 732e 5c6e 5c6e  ge\ndepends.\n\n
-00000d60: 416c 7465 726e 6174 6976 656c 792c 2069  Alternatively, i
-00000d70: 6620 796f 7520 7072 6566 6572 2074 6f20  f you prefer to 
-00000d80: 7573 6520 6070 6970 6020 2877 6865 7468  use `pip` (wheth
-00000d90: 6572 206f 7220 6e6f 7420 796f 7520 7573  er or not you us
-00000da0: 6520 6063 6f6e 6461 6029 2c20 796f 755c  e `conda`), you\
-00000db0: 6e63 616e 2061 6c73 6f20 646f 5c6e 5c6e  ncan also do\n\n
-00000dc0: 6060 6073 685c 6e70 6970 2069 6e73 7461  ```sh\npip insta
-00000dd0: 6c6c 2067 6974 2b67 6974 3a2f 2f67 6974  ll git+git://git
-00000de0: 6875 622e 636f 6d2f 6d6f 626c 652f 7175  hub.com/moble/qu
-00000df0: 6174 6572 6e69 6f6e 5c6e 7069 7020 696e  aternion\npip in
-00000e00: 7374 616c 6c20 6769 742b 6769 743a 2f2f  stall git+git://
-00000e10: 6769 7468 7562 2e63 6f6d 2f6d 6f62 6c65  github.com/moble
-00000e20: 2f73 7068 6572 6963 616c 5f66 756e 6374  /spherical_funct
-00000e30: 696f 6e73 5c6e 6060 605c 6e5c 6e4f 722c  ions\n```\n\nOr,
-00000e40: 2069 6620 796f 7520 7265 6675 7365 2074   if you refuse t
-00000e50: 6f20 7573 6520 6063 6f6e 6461 602c 2079  o use `conda`, y
-00000e60: 6f75 206d 6967 6874 2077 616e 7420 746f  ou might want to
-00000e70: 2069 6e73 7461 6c6c 2069 6e73 6964 6520   install inside 
-00000e80: 796f 7572 2068 6f6d 655c 6e64 6972 6563  your home\ndirec
-00000e90: 746f 7279 2077 6974 686f 7574 2072 6f6f  tory without roo
-00000ea0: 7420 7072 6976 696c 6567 6573 2e20 2028  t privileges.  (
-00000eb0: 416e 6163 6f6e 6461 2064 6f65 7320 7468  Anaconda does th
-00000ec0: 6973 2062 7920 6465 6661 756c 7420 616e  is by default an
-00000ed0: 7977 6179 2e29 5c6e 5468 6973 2069 7320  yway.)\nThis is 
-00000ee0: 646f 6e65 2062 7920 6164 6469 6e67 2060  done by adding `
-00000ef0: 2d2d 7573 6572 6020 746f 2074 6865 2061  --user` to the a
-00000f00: 626f 7665 2063 6f6d 6d61 6e64 733a 5c6e  bove commands:\n
-00000f10: 5c6e 6060 6073 685c 6e70 6970 2069 6e73  \n```sh\npip ins
-00000f20: 7461 6c6c 202d 2d75 7365 7220 6769 742b  tall --user git+
-00000f30: 6769 743a 2f2f 6769 7468 7562 2e63 6f6d  git://github.com
-00000f40: 2f6d 6f62 6c65 2f71 7561 7465 726e 696f  /moble/quaternio
-00000f50: 6e5c 6e70 6970 2069 6e73 7461 6c6c 202d  n\npip install -
-00000f60: 2d75 7365 7220 6769 742b 6769 743a 2f2f  -user git+git://
-00000f70: 6769 7468 7562 2e63 6f6d 2f6d 6f62 6c65  github.com/moble
-00000f80: 2f73 7068 6572 6963 616c 5f66 756e 6374  /spherical_funct
-00000f90: 696f 6e73 5c6e 6060 605c 6e5c 6e46 696e  ions\n```\n\nFin
-00000fa0: 616c 6c79 2c20 7468 6572 655c 2773 2061  ally, there\'s a
-00000fb0: 6c73 6f20 7468 6520 6675 6c6c 7920 6d61  lso the fully ma
-00000fc0: 6e75 616c 206f 7074 696f 6e20 6f66 206a  nual option of j
-00000fd0: 7573 7420 646f 776e 6c6f 6164 696e 6720  ust downloading 
-00000fe0: 626f 7468 2063 6f64 655c 6e72 6570 6f73  both code\nrepos
-00000ff0: 6974 6f72 6965 732c 2063 6861 6e67 696e  itories, changin
-00001000: 6720 746f 2074 6865 2063 6f64 6520 6469  g to the code di
-00001010: 7265 6374 6f72 792c 2061 6e64 2069 7373  rectory, and iss
-00001020: 7569 6e67 5c6e 5c6e 6060 6073 685c 6e70  uing\n\n```sh\np
-00001030: 7974 686f 6e20 7365 7475 702e 7079 2069  ython setup.py i
-00001040: 6e73 7461 6c6c 5c6e 6060 605c 6e5c 6e54  nstall\n```\n\nT
-00001050: 6869 7320 7368 6f75 6c64 2077 6f72 6b20  his should work 
-00001060: 7265 6761 7264 6c65 7373 206f 6620 7468  regardless of th
-00001070: 6520 696e 7374 616c 6c61 7469 6f6e 206d  e installation m
-00001080: 6574 686f 642c 2061 7320 6c6f 6e67 2061  ethod, as long a
-00001090: 7320 796f 7520 6861 7665 2061 5c6e 636f  s you have a\nco
-000010a0: 6d70 696c 6572 2068 616e 6769 6e67 2061  mpiler hanging a
-000010b0: 726f 756e 642e 5c6e 5c6e 5c6e 2323 2055  round.\n\n\n## U
-000010c0: 7361 6765 5c6e 5c6e 4669 7273 742c 2077  sage\n\nFirst, w
-000010d0: 6520 7368 6f77 2061 2076 6572 7920 7369  e show a very si
-000010e0: 6d70 6c65 2065 7861 6d70 6c65 206f 6620  mple example of 
-000010f0: 7573 6167 6520 7769 7468 2045 756c 6572  usage with Euler
-00001100: 2061 6e67 6c65 732c 2074 686f 7567 6820   angles, though 
-00001110: 6974 5c6e 6272 6561 6b73 206d 7920 6865  it\nbreaks my he
-00001120: 6172 7420 746f 2064 6f20 736f 3a3c 7375  art to do so:<su
-00001130: 703e 5b31 5d28 2365 756c 6572 2d61 6e67  p>[1](#euler-ang
-00001140: 6c65 732d 6172 652d 6177 6675 6c29 3c2f  les-are-awful)</
-00001150: 7375 703e 5c6e 5c6e 6060 6070 7974 686f  sup>\n\n```pytho
-00001160: 6e5c 6e3e 3e3e 2069 6d70 6f72 7420 7370  n\n>>> import sp
-00001170: 6865 7269 6361 6c5f 6675 6e63 7469 6f6e  herical_function
-00001180: 7320 6173 2073 665c 6e3e 3e3e 2061 6c70  s as sf\n>>> alp
-00001190: 6861 2c20 6265 7461 2c20 6761 6d6d 6120  ha, beta, gamma 
-000011a0: 3d20 302e 312c 2030 2e32 2c20 302e 335c  = 0.1, 0.2, 0.3\
-000011b0: 6e3e 3e3e 2065 6c6c 2c6d 702c 6d20 3d20  n>>> ell,mp,m = 
-000011c0: 332c 322c 315c 6e3e 3e3e 2073 662e 5769  3,2,1\n>>> sf.Wi
-000011d0: 676e 6572 5f44 5f65 6c65 6d65 6e74 2861  gner_D_element(a
-000011e0: 6c70 6861 2c20 6265 7461 2c20 6761 6d6d  lpha, beta, gamm
-000011f0: 612c 2065 6c6c 2c20 6d70 2c20 6d29 5c6e  a, ell, mp, m)\n
-00001200: 5c6e 6060 605c 6e5c 6e4f 6620 636f 7572  \n```\n\nOf cour
-00001210: 7365 2c20 6974 5c27 7320 616c 7761 7973  se, it\'s always
-00001220: 2062 6574 7465 7220 746f 2075 7365 2075   better to use u
-00001230: 6e69 7420 7175 6174 6572 6e69 6f6e 7320  nit quaternions 
-00001240: 746f 2064 6573 6372 6962 6520 726f 7461  to describe rota
-00001250: 7469 6f6e 733a 5c6e 5c6e 6060 6070 7974  tions:\n\n```pyt
-00001260: 686f 6e5c 6e3e 3e3e 2069 6d70 6f72 7420  hon\n>>> import 
-00001270: 6e75 6d70 7920 6173 206e 705c 6e3e 3e3e  numpy as np\n>>>
-00001280: 2069 6d70 6f72 7420 7175 6174 6572 6e69   import quaterni
-00001290: 6f6e 5c6e 3e3e 3e20 5220 3d20 6e70 2e71  on\n>>> R = np.q
-000012a0: 7561 7465 726e 696f 6e28 312c 322c 332c  uaternion(1,2,3,
-000012b0: 3429 2e6e 6f72 6d61 6c69 7a65 6428 295c  4).normalized()\
-000012c0: 6e3e 3e3e 2065 6c6c 2c6d 702c 6d20 3d20  n>>> ell,mp,m = 
-000012d0: 332c 322c 315c 6e3e 3e3e 2073 662e 5769  3,2,1\n>>> sf.Wi
-000012e0: 676e 6572 5f44 5f65 6c65 6d65 6e74 2852  gner_D_element(R
-000012f0: 2c20 656c 6c2c 206d 702c 206d 295c 6e5c  , ell, mp, m)\n\
-00001300: 6e60 6060 5c6e 5c6e 4966 2079 6f75 206e  n```\n\nIf you n
-00001310: 6565 6420 746f 2063 616c 6375 6c61 7465  eed to calculate
-00001320: 2076 616c 7565 7320 6f66 2074 6865 20f0   values of the .
-00001330: 9d94 873c 7375 703e 28e2 8493 293c 2f73  ...<sup>(...)</s
-00001340: 7570 3e20 6d61 7472 6978 2065 6c65 6d65  up> matrix eleme
-00001350: 6e74 7320 666f 7220 6d61 6e79 5c6e 7661  nts for many\nva
-00001360: 6c75 6573 206f 6620 28e2 8493 2c20 6d5c  lues of (..., m\
-00001370: 272c 206d 292c 2069 7420 6973 206d 6f72  ', m), it is mor
-00001380: 6520 6566 6669 6369 656e 7420 746f 2064  e efficient to d
-00001390: 6f20 736f 2061 6c6c 2061 7420 6f6e 6365  o so all at once
-000013a0: 2e20 2054 6865 2066 6f6c 6c6f 7769 6e67  .  The following
-000013b0: 5c6e 6361 6c63 756c 6174 6573 2061 6c6c  \ncalculates all
-000013c0: 206d 6f64 6573 2066 6f72 20e2 8493 2066   modes for ... f
-000013d0: 726f 6d20 3220 746f 2038 2028 696e 636c  rom 2 to 8 (incl
-000013e0: 7573 6976 6529 3a5c 6e5c 6e60 6060 7079  usive):\n\n```py
-000013f0: 7468 6f6e 5c6e 3e3e 3e20 696e 6469 6365  thon\n>>> indice
-00001400: 7320 3d20 6e70 2e61 7272 6179 285b 5b65  s = np.array([[e
-00001410: 6c6c 2c6d 702c 6d5d 2066 6f72 2065 6c6c  ll,mp,m] for ell
-00001420: 2069 6e20 7261 6e67 6528 322c 3929 5c6e   in range(2,9)\n
-00001430: 2e2e 2e20 666f 7220 6d70 2069 6e20 7261  ... for mp in ra
-00001440: 6e67 6528 2d65 6c6c 2c20 656c 6c2b 3129  nge(-ell, ell+1)
-00001450: 2066 6f72 206d 2069 6e20 7261 6e67 6528   for m in range(
-00001460: 2d65 6c6c 2c20 656c 6c2b 3129 5d29 5c6e  -ell, ell+1)])\n
-00001470: 3e3e 3e20 7366 2e57 6967 6e65 725f 445f  >>> sf.Wigner_D_
-00001480: 656c 656d 656e 7428 522c 2069 6e64 6963  element(R, indic
-00001490: 6573 295c 6e5c 6e60 6060 5c6e 5c6e 4669  es)\n\n```\n\nFi
-000014a0: 6e61 6c6c 792c 2069 6620 796f 7520 7265  nally, if you re
-000014b0: 616c 6c79 206e 6565 6420 746f 2070 7574  ally need to put
-000014c0: 2074 6865 2070 6564 616c 2074 6f20 7468   the pedal to th
-000014d0: 6520 6d65 7461 6c2c 2061 6e64 2061 7265  e metal, and are
-000014e0: 2077 696c 6c69 6e67 2074 6f5c 6e67 7561   willing to\ngua
-000014f0: 7261 6e74 6565 2074 6861 7420 7468 6520  rantee that the 
-00001500: 696e 7075 7420 6172 6775 6d65 6e74 7320  input arguments 
-00001510: 6172 6520 636f 7272 6563 742c 2079 6f75  are correct, you
-00001520: 2063 616e 2075 7365 2061 2073 7065 6369   can use a speci
-00001530: 616c 2068 6964 6465 6e5c 6e66 6f72 6d20  al hidden\nform 
-00001540: 6f66 2074 6865 2066 756e 6374 696f 6e3a  of the function:
-00001550: 5c6e 5c6e 6060 6070 7974 686f 6e5c 6e3e  \n\n```python\n>
-00001560: 3e3e 2073 662e 5f57 6967 6e65 725f 445f  >> sf._Wigner_D_
-00001570: 656c 656d 656e 7428 522e 612c 2052 2e62  element(R.a, R.b
-00001580: 2c20 696e 6469 6365 732c 2065 6c65 6d65  , indices, eleme
-00001590: 6e74 7329 5c6e 5c6e 6060 605c 6e5c 6e48  nts)\n\n```\n\nH
-000015a0: 6572 652c 2060 522e 6160 2061 6e64 2060  ere, `R.a` and `
-000015b0: 522e 6260 2061 7265 2074 6865 2074 776f  R.b` are the two
-000015c0: 2063 6f6d 706c 6578 2070 6172 7473 206f   complex parts o
-000015d0: 6620 7468 6520 7175 6174 6572 6e69 6f6e  f the quaternion
-000015e0: 2064 6566 696e 6564 206f 6e5c 6e5b 7468   defined on\n[th
-000015f0: 6973 2070 6167 655d 2868 7474 703a 2f2f  is page](http://
-00001600: 6d6f 626c 652e 6769 7468 7562 2e69 6f2f  moble.github.io/
-00001610: 7370 6865 7269 6361 6c5f 6675 6e63 7469  spherical_functi
-00001620: 6f6e 732f 2920 2874 686f 7567 6820 7468  ons/) (though th
-00001630: 6520 7573 6572 206e 6565 645c 6e6e 6f74  e user need\nnot
-00001640: 2063 6172 6520 6162 6f75 7420 7468 6174   care about that
-00001650: 292e 2020 5468 6520 6069 6e64 6963 6573  ).  The `indices
-00001660: 6020 7661 7269 6162 6c65 2069 7320 6173  ` variable is as
-00001670: 7375 6d65 6420 746f 2062 6520 615c 6e74  sumed to be a\nt
-00001680: 776f 2d64 696d 656e 7369 6f6e 616c 2061  wo-dimensional a
-00001690: 7272 6179 206f 6620 696e 7465 6765 7273  rray of integers
-000016a0: 2c20 7768 6572 6520 7468 6520 7365 636f  , where the seco
-000016b0: 6e64 2064 696d 656e 7369 6f6e 2068 6173  nd dimension has
-000016c0: 2073 697a 6520 7468 7265 652c 5c6e 7265   size three,\nre
-000016d0: 7072 6573 656e 7469 6e67 2074 6865 2028  presenting the (
-000016e0: e284 932c 206d 5c27 2c20 6d29 2069 6e64  ..., m\', m) ind
-000016f0: 6963 6573 2e20 2054 6869 7320 6176 6f69  ices.  This avoi
-00001700: 6473 2063 6572 7461 696e 2073 6f6d 6577  ds certain somew
-00001710: 6861 7420 736c 6f77 6572 5c6e 7075 7265  hat slower\npure
-00001720: 2d70 7974 686f 6e20 6f70 6572 6174 696f  -python operatio
-00001730: 6e73 2069 6e76 6f6c 7669 6e67 2061 7267  ns involving arg
-00001740: 756d 656e 7420 6368 6563 6b69 6e67 2c20  ument checking, 
-00001750: 7265 7368 6170 696e 672c 2065 7463 2e20  reshaping, etc. 
-00001760: 2054 6865 5c6e 6065 6c65 6d65 6e74 7360   The\n`elements`
-00001770: 2076 6172 6961 626c 6520 6d75 7374 2062   variable must b
-00001780: 6520 6120 6f6e 652d 6469 6d65 6e73 696f  e a one-dimensio
-00001790: 6e61 6c20 6172 7261 7920 6f66 2063 6f6d  nal array of com
-000017a0: 706c 6578 206e 756d 6265 7273 2028 6361  plex numbers (ca
-000017b0: 6e20 6265 5c6e 756e 696e 6974 6961 6c69  n be\nuninitiali
-000017c0: 7a65 6429 2c20 7768 6963 6820 7769 6c6c  zed), which will
-000017d0: 2062 6520 7265 706c 6163 6564 2077 6974   be replaced wit
-000017e0: 6820 7468 6520 636f 7272 6573 706f 6e64  h the correspond
-000017f0: 696e 6720 7661 6c75 6573 206f 6e20 7265  ing values on re
-00001800: 7475 726e 2e5c 6e41 6761 696e 2c20 686f  turn.\nAgain, ho
-00001810: 7765 7665 722c 2074 6865 7265 2069 7320  wever, there is 
-00001820: 6e6f 2069 6e70 7574 2064 696d 656e 7369  no input dimensi
-00001830: 6f6e 2063 6865 636b 696e 6720 6865 7265  on checking here
-00001840: 2c20 736f 2069 6620 796f 7520 6769 7665  , so if you give
-00001850: 2062 6164 5c6e 696e 7075 7473 2c20 6265   bad\ninputs, be
-00001860: 6861 7669 6f72 2063 6f75 6c64 2072 616e  havior could ran
-00001870: 6765 2066 726f 6d20 7369 6c65 6e74 6c79  ge from silently
-00001880: 2077 726f 6e67 2074 6f20 6578 6365 7074   wrong to except
-00001890: 696f 6e73 2074 6f20 7365 676d 656e 7461  ions to segmenta
-000018a0: 7469 6f6e 5c6e 6661 756c 7473 2e20 2043  tion\nfaults.  C
-000018b0: 6176 6561 7420 656d 7074 6f72 2e5c 6e5c  aveat emptor.\n\
-000018c0: 6e5c 6e23 2320 4163 6b6e 6f77 6c65 6467  n\n## Acknowledg
-000018d0: 6d65 6e74 735c 6e5c 6e49 2076 6572 7920  ments\n\nI very 
-000018e0: 6d75 6368 2061 7070 7265 6369 6174 6520  much appreciate 
-000018f0: 4261 7272 7920 5761 7264 656c 6c5c 2773  Barry Wardell\'s
-00001900: 2068 656c 7020 696e 2073 6f72 7469 6e67   help in sorting
-00001910: 206f 7574 2074 6865 2072 656c 6174 696f   out the relatio
-00001920: 6e73 6869 7073 5c6e 6265 7477 6565 6e20  nships\nbetween 
-00001930: 6d79 2063 6f6e 7665 6e74 696f 6e73 2061  my conventions a
-00001940: 6e64 2074 686f 7365 206f 6620 6f74 6865  nd those of othe
-00001950: 7220 7065 6f70 6c65 2061 6e64 2073 6f66  r people and sof
-00001960: 7477 6172 6520 7061 636b 6167 6573 5c6e  tware packages\n
-00001970: 2865 7370 6563 6961 6c6c 7920 4d61 7468  (especially Math
-00001980: 656d 6174 6963 615c 2773 2063 7261 7a79  ematica\'s crazy
-00001990: 2063 6f6e 7665 6e74 696f 6e73 292e 5c6e   conventions).\n
-000019a0: 5c6e 5468 6973 2063 6f64 6520 6973 2c20  \nThis code is, 
-000019b0: 6f66 2063 6f75 7273 652c 2068 6f73 7465  of course, hoste
-000019c0: 6420 6f6e 2067 6974 6875 622e 2020 4265  d on github.  Be
-000019d0: 6361 7573 6520 6974 2069 7320 616e 206f  cause it is an o
-000019e0: 7065 6e2d 736f 7572 6365 5c6e 7072 6f6a  pen-source\nproj
-000019f0: 6563 742c 2074 6865 2068 6f73 7469 6e67  ect, the hosting
-00001a00: 2069 7320 6672 6565 2c20 616e 6420 616c   is free, and al
-00001a10: 6c20 7468 6520 776f 6e64 6572 6675 6c20  l the wonderful 
-00001a20: 6665 6174 7572 6573 206f 6620 6769 7468  features of gith
-00001a30: 7562 2061 7265 5c6e 6176 6169 6c61 626c  ub are\navailabl
-00001a40: 652c 2069 6e63 6c75 6469 6e67 2066 7265  e, including fre
-00001a50: 6520 7769 6b69 2073 7061 6365 2061 6e64  e wiki space and
-00001a60: 2077 6562 2070 6167 6520 686f 7374 696e   web page hostin
-00001a70: 672c 2070 756c 6c20 7265 7175 6573 7473  g, pull requests
-00001a80: 2c20 615c 6e6e 6963 6520 696e 7465 7266  , a\nnice interf
-00001a90: 6163 6520 746f 2074 6865 2067 6974 206c  ace to the git l
-00001aa0: 6f67 732c 2065 7463 2e5c 6e5c 6e45 7665  ogs, etc.\n\nEve
-00001ab0: 7279 2063 6861 6e67 6520 696e 2074 6869  ry change in thi
-00001ac0: 7320 636f 6465 2069 735c 6e5b 6175 6f6d  s code is\n[auom
-00001ad0: 6174 6963 616c 6c79 2074 6573 7465 645d  atically tested]
-00001ae0: 2868 7474 7073 3a2f 2f74 7261 7669 732d  (https://travis-
-00001af0: 6369 2e6f 7267 2f6d 6f62 6c65 2f73 7068  ci.org/moble/sph
-00001b00: 6572 6963 616c 5f66 756e 6374 696f 6e73  erical_functions
-00001b10: 2920 6f6e 5c6e 5b54 7261 7669 732d 4349  ) on\n[Travis-CI
-00001b20: 5d28 6874 7470 733a 2f2f 7472 6176 6973  ](https://travis
-00001b30: 2d63 692e 6f72 672f 292e 2020 5468 6973  -ci.org/).  This
-00001b40: 2069 7320 6120 6672 6565 2073 6572 7669   is a free servi
-00001b50: 6365 2028 666f 7220 6f70 656e 2d73 6f75  ce (for open-sou
-00001b60: 7263 655c 6e70 726f 6a65 6374 7320 6c69  rce\nprojects li
-00001b70: 6b65 2074 6869 7320 6f6e 6529 2c20 7768  ke this one), wh
-00001b80: 6963 6820 696e 7465 6772 6174 6573 2062  ich integrates b
-00001b90: 6561 7574 6966 756c 6c79 2077 6974 6820  eautifully with 
-00001ba0: 6769 7468 7562 2c20 6465 7465 6374 696e  github, detectin
-00001bb0: 675c 6e65 6163 6820 636f 6d6d 6974 2061  g\neach commit a
-00001bc0: 6e64 2061 7574 6f6d 6174 6963 616c 6c79  nd automatically
-00001bd0: 2072 652d 7275 6e6e 696e 6720 7468 6520   re-running the 
-00001be0: 7465 7374 732e 2020 5468 6520 636f 6465  tests.  The code
-00001bf0: 2069 7320 646f 776e 6c6f 6164 6564 2061   is downloaded a
-00001c00: 6e64 5c6e 696e 7374 616c 6c65 6420 6672  nd\ninstalled fr
-00001c10: 6573 6820 6561 6368 2074 696d 652c 2061  esh each time, a
-00001c20: 6e64 2074 6865 6e20 7465 7374 6564 2c20  nd then tested, 
-00001c30: 6f6e 2070 7974 686f 6e20 322e 372c 2033  on python 2.7, 3
-00001c40: 2e34 2c20 616e 6420 332e 352e 2020 5468  .4, and 3.5.  Th
-00001c50: 6973 5c6e 656e 7375 7265 7320 7468 6174  is\nensures that
-00001c60: 206e 6f20 6368 616e 6765 2049 206d 616b   no change I mak
-00001c70: 6520 746f 2074 6865 2063 6f64 6520 6272  e to the code br
-00001c80: 6561 6b73 2065 6974 6865 7220 696e 7374  eaks either inst
-00001c90: 616c 6c61 7469 6f6e 206f 7220 616e 7920  allation or any 
-00001ca0: 6f66 5c6e 7468 6520 6665 6174 7572 6573  of\nthe features
-00001cb0: 2074 6861 7420 4920 6861 7665 2077 7269   that I have wri
-00001cc0: 7474 656e 2074 6573 7473 2066 6f72 2e5c  tten tests for.\
-00001cd0: 6e5c 6e46 696e 616c 6c79 2c20 7468 6520  n\nFinally, the 
-00001ce0: 636f 6465 2069 7320 6175 746f 6d61 7469  code is automati
-00001cf0: 6361 6c6c 7920 636f 6d70 696c 6564 2c20  cally compiled, 
-00001d00: 616e 6420 7468 6520 6269 6e61 7269 6573  and the binaries
-00001d10: 2068 6f73 7465 6420 666f 725c 6e64 6f77   hosted for\ndow
-00001d20: 6e6c 6f61 6420 6279 2060 636f 6e64 6160  nload by `conda`
-00001d30: 206f 6e20 5b61 6e61 636f 6e64 612e 6f72   on [anaconda.or
-00001d40: 675d 2868 7474 7073 3a2f 2f61 6e61 636f  g](https://anaco
-00001d50: 6e64 612e 6f72 672f 6d6f 626c 652f 7175  nda.org/moble/qu
-00001d60: 6174 6572 6e69 6f6e 292e 5c6e 5468 6973  aternion).\nThis
-00001d70: 2069 7320 616c 736f 2061 2066 7265 6520   is also a free 
-00001d80: 7365 7276 6963 6520 666f 7220 6f70 656e  service for open
-00001d90: 2d73 6f75 7263 6520 7072 6f6a 6563 7473  -source projects
-00001da0: 206c 696b 6520 7468 6973 206f 6e65 2e5c   like this one.\
-00001db0: 6e5c 6e54 6865 2077 6f72 6b20 6f66 2063  n\nThe work of c
-00001dc0: 7265 6174 696e 6720 7468 6973 2063 6f64  reating this cod
-00001dd0: 6520 7761 7320 7375 7070 6f72 7465 6420  e was supported 
-00001de0: 696e 2070 6172 7420 6279 2074 6865 2053  in part by the S
-00001df0: 6865 726d 616e 2046 6169 7263 6869 6c64  herman Fairchild
-00001e00: 5c6e 466f 756e 6461 7469 6f6e 2061 6e64  \nFoundation and
-00001e10: 2062 7920 4e53 4620 4772 616e 7473 204e   by NSF Grants N
-00001e20: 6f2e 2050 4859 2d31 3330 3631 3235 2061  o. PHY-1306125 a
-00001e30: 6e64 2041 5354 2d31 3333 3331 3239 2e5c  nd AST-1333129.\
-00001e40: 6e5c 6e5c 6e3c 6272 2f3e 5c6e 2d2d 2d5c  n\n\n<br/>\n---\
-00001e50: 6e23 2323 2323 2320 3c73 7570 3e31 3c2f  n###### <sup>1</
-00001e60: 7375 703e 2045 756c 6572 2061 6e67 6c65  sup> Euler angle
-00001e70: 7320 6172 6520 6177 6675 6c5c 6e5c 6e45  s are awful\n\nE
-00001e80: 756c 6572 2061 6e67 6c65 7320 6172 6520  uler angles are 
-00001e90: 7072 6574 7479 206d 7563 685c 6e5b 7468  pretty much\n[th
-00001ea0: 6520 776f 7273 7420 7468 696e 6773 2065  e worst things e
-00001eb0: 7665 725d 2868 7474 703a 2f2f 6d6f 626c  ver](http://mobl
-00001ec0: 652e 6769 7468 7562 2e69 6f2f 7370 6865  e.github.io/sphe
-00001ed0: 7269 6361 6c5f 6675 6e63 7469 6f6e 732f  rical_functions/
-00001ee0: 2365 756c 6572 2d61 6e67 6c65 7329 5c6e  #euler-angles)\n
-00001ef0: 616e 6420 6974 206d 616b 6573 206d 6520  and it makes me 
-00001f00: 6665 656c 2062 6164 2065 7665 6e20 7375  feel bad even su
-00001f10: 7070 6f72 7469 6e67 2074 6865 6d2e 2020  pporting them.  
-00001f20: 5175 6174 6572 6e69 6f6e 7320 6172 655c  Quaternions are\
-00001f30: 6e66 6173 7465 722c 206d 6f72 6520 6163  nfaster, more ac
-00001f40: 6375 7261 7465 2c20 6261 7369 6361 6c6c  curate, basicall
-00001f50: 7920 6672 6565 206f 6620 7369 6e67 756c  y free of singul
-00001f60: 6172 6974 6965 732c 206d 6f72 655c 6e69  arities, more\ni
-00001f70: 6e74 7569 7469 7665 2c20 616e 6420 6765  ntuitive, and ge
-00001f80: 6e65 7261 6c6c 7920 6561 7369 6572 2074  nerally easier t
-00001f90: 6f20 756e 6465 7273 7461 6e64 2e20 2059  o understand.  Y
-00001fa0: 6f75 2063 616e 2077 6f72 6b20 656e 7469  ou can work enti
-00001fb0: 7265 6c79 5c6e 7769 7468 6f75 7420 4575  rely\nwithout Eu
-00001fc0: 6c65 7220 616e 676c 6573 2028 4920 6365  ler angles (I ce
-00001fd0: 7274 6169 6e6c 7920 646f 292e 2020 596f  rtainly do).  Yo
-00001fe0: 7520 6162 736f 6c75 7465 6c79 206e 6576  u absolutely nev
-00001ff0: 6572 206e 6565 645c 6e74 6865 6d2e 2020  er need\nthem.  
-00002000: 4275 7420 6966 2079 6f75 5c27 7265 2073  But if you\'re s
-00002010: 6f20 6f6c 6420 6661 7368 696f 6e65 6420  o old fashioned 
-00002020: 7468 6174 2079 6f75 2072 6561 6c6c 7920  that you really 
-00002030: 6361 6e5c 2774 2067 6976 6520 7468 656d  can\'t give them
-00002040: 5c6e 7570 2c20 7468 6579 2061 7265 2066  \nup, they are f
-00002050: 756c 6c79 2073 7570 706f 7274 6564 2e5c  ully supported.\
-00002060: 6e27 2c0a 2020 2020 2761 7574 686f 7227  n',.    'author'
-00002070: 3a20 274d 6963 6861 656c 2042 6f79 6c65  : 'Michael Boyle
-00002080: 272c 0a20 2020 2027 6175 7468 6f72 5f65  ',.    'author_e
-00002090: 6d61 696c 273a 2027 6d6f 6232 3240 636f  mail': 'mob22@co
-000020a0: 726e 656c 6c2e 6564 7527 2c0a 2020 2020  rnell.edu',.    
-000020b0: 276d 6169 6e74 6169 6e65 7227 3a20 4e6f  'maintainer': No
-000020c0: 6e65 2c0a 2020 2020 276d 6169 6e74 6169  ne,.    'maintai
-000020d0: 6e65 725f 656d 6169 6c27 3a20 4e6f 6e65  ner_email': None
-000020e0: 2c0a 2020 2020 2775 726c 273a 2027 6874  ,.    'url': 'ht
-000020f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002100: 2f6d 6f62 6c65 2f73 7068 6572 6963 616c  /moble/spherical
-00002110: 5f66 756e 6374 696f 6e73 272c 0a20 2020  _functions',.   
-00002120: 2027 7061 636b 6167 6573 273a 2070 6163   'packages': pac
-00002130: 6b61 6765 732c 0a20 2020 2027 7061 636b  kages,.    'pack
-00002140: 6167 655f 6461 7461 273a 2070 6163 6b61  age_data': packa
-00002150: 6765 5f64 6174 612c 0a20 2020 2027 696e  ge_data,.    'in
-00002160: 7374 616c 6c5f 7265 7175 6972 6573 273a  stall_requires':
-00002170: 2069 6e73 7461 6c6c 5f72 6571 7569 7265   install_require
-00002180: 732c 0a20 2020 2027 7079 7468 6f6e 5f72  s,.    'python_r
-00002190: 6571 7569 7265 7327 3a20 273e 3d33 2e38  equires': '>=3.8
-000021a0: 2c3c 332e 3131 272c 0a7d 0a0a 0a73 6574  ,<3.11',.}...set
-000021b0: 7570 282a 2a73 6574 7570 5f6b 7761 7267  up(**setup_kwarg
-000021c0: 7329 0a                                  s).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7370 6865  : 2.1.Name: sphe
+00000020: 7269 6361 6c2d 6675 6e63 7469 6f6e 730a  rical-functions.
+00000030: 5665 7273 696f 6e3a 2032 3032 322e 342e  Version: 2022.4.
+00000040: 320a 5375 6d6d 6172 793a 2050 7974 686f  2.Summary: Pytho
+00000050: 6e2f 6e75 6d62 6120 696d 706c 656d 656e  n/numba implemen
+00000060: 7461 7469 6f6e 206f 6620 5769 676e 6572  tation of Wigner
+00000070: 2044 204d 6174 7269 6365 732c 2073 7069   D Matrices, spi
+00000080: 6e2d 7765 6967 6874 6564 2073 7068 6572  n-weighted spher
+00000090: 6963 616c 2068 6172 6d6f 6e69 6373 2c20  ical harmonics, 
+000000a0: 616e 6420 6173 736f 6369 6174 6564 2066  and associated f
+000000b0: 756e 6374 696f 6e73 0a48 6f6d 652d 7061  unctions.Home-pa
+000000c0: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
+000000d0: 7562 2e63 6f6d 2f6d 6f62 6c65 2f73 7068  ub.com/moble/sph
+000000e0: 6572 6963 616c 5f66 756e 6374 696f 6e73  erical_functions
+000000f0: 0a4c 6963 656e 7365 3a20 4d49 540a 4175  .License: MIT.Au
+00000100: 7468 6f72 3a20 4d69 6368 6165 6c20 426f  thor: Michael Bo
+00000110: 796c 650a 4175 7468 6f72 2d65 6d61 696c  yle.Author-email
+00000120: 3a20 6d6f 6232 3240 636f 726e 656c 6c2e  : mob22@cornell.
+00000130: 6564 750a 5265 7175 6972 6573 2d50 7974  edu.Requires-Pyt
+00000140: 686f 6e3a 203e 3d33 2e38 2c3c 332e 3132  hon: >=3.8,<3.12
+00000150: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000160: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000170: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+00000180: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
+00000190: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001b0: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
+000001c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001e0: 3a20 332e 380a 436c 6173 7369 6669 6572  : 3.8.Classifier
+000001f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000200: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000210: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000220: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000230: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000240: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+00000250: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000270: 7974 686f 6e20 3a3a 2033 2e31 310a 5265  ython :: 3.11.Re
+00000280: 7175 6972 6573 2d44 6973 743a 206e 756d  quires-Dist: num
+00000290: 6261 2028 3e3d 302e 3535 290a 5265 7175  ba (>=0.55).Requ
+000002a0: 6972 6573 2d44 6973 743a 206e 756d 7079  ires-Dist: numpy
+000002b0: 2028 3e3d 312e 3230 290a 5265 7175 6972   (>=1.20).Requir
+000002c0: 6573 2d44 6973 743a 206e 756d 7079 2d71  es-Dist: numpy-q
+000002d0: 7561 7465 726e 696f 6e20 283e 3d32 3032  uaternion (>=202
+000002e0: 3229 0a52 6571 7569 7265 732d 4469 7374  2).Requires-Dist
+000002f0: 3a20 7363 6970 7920 283e 3d31 2e30 2c3c  : scipy (>=1.0,<
+00000300: 322e 3029 0a52 6571 7569 7265 732d 4469  2.0).Requires-Di
+00000310: 7374 3a20 7370 696e 7366 6173 7420 283e  st: spinsfast (>
+00000320: 3d32 3032 3229 0a44 6573 6372 6970 7469  =2022).Descripti
+00000330: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000340: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
+00000350: 5b21 5b54 6573 7420 5374 6174 7573 5d28  [![Test Status](
+00000360: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000370: 6f6d 2f6d 6f62 6c65 2f73 7068 6572 6963  om/moble/spheric
+00000380: 616c 5f66 756e 6374 696f 6e73 2f77 6f72  al_functions/wor
+00000390: 6b66 6c6f 7773 2f74 6573 7473 2f62 6164  kflows/tests/bad
+000003a0: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
+000003b0: 2f67 6974 6875 622e 636f 6d2f 6d6f 626c  /github.com/mobl
+000003c0: 652f 7370 6865 7269 6361 6c5f 6675 6e63  e/spherical_func
+000003d0: 7469 6f6e 732f 6163 7469 6f6e 7329 0a5b  tions/actions).[
+000003e0: 215b 5079 5049 2056 6572 7369 6f6e 5d28  ![PyPI Version](
+000003f0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000400: 6c64 732e 696f 2f70 7970 692f 762f 7370  lds.io/pypi/v/sp
+00000410: 6865 7269 6361 6c2d 6675 6e63 7469 6f6e  herical-function
+00000420: 733f 636f 6c6f 723d 295d 2868 7474 7073  s?color=)](https
+00000430: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000440: 6563 742f 7370 6865 7269 6361 6c2d 6675  ect/spherical-fu
+00000450: 6e63 7469 6f6e 732f 290a 5b21 5b43 6f6e  nctions/).[![Con
+00000460: 6461 2056 6572 7369 6f6e 5d28 6874 7470  da Version](http
+00000470: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000480: 696f 2f63 6f6e 6461 2f76 6e2f 636f 6e64  io/conda/vn/cond
+00000490: 612d 666f 7267 652f 7370 6865 7269 6361  a-forge/spherica
+000004a0: 6c5f 6675 6e63 7469 6f6e 732e 7376 673f  l_functions.svg?
+000004b0: 636f 6c6f 723d 295d 2868 7474 7073 3a2f  color=)](https:/
+000004c0: 2f61 6e61 636f 6e64 612e 6f72 672f 636f  /anaconda.org/co
+000004d0: 6e64 612d 666f 7267 652f 7370 6865 7269  nda-forge/spheri
+000004e0: 6361 6c5f 6675 6e63 7469 6f6e 7329 0a5b  cal_functions).[
+000004f0: 215b 4d49 5420 4c69 6365 6e73 655d 2868  ![MIT License](h
+00000500: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000510: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
+00000520: 656e 7365 2f6d 6f62 6c65 2f73 7068 6572  ense/moble/spher
+00000530: 6963 616c 5f66 756e 6374 696f 6e73 2e73  ical_functions.s
+00000540: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000550: 6875 622e 636f 6d2f 6d6f 626c 652f 7370  hub.com/moble/sp
+00000560: 6865 7269 6361 6c5f 6675 6e63 7469 6f6e  herical_function
+00000570: 732f 626c 6f62 2f6d 6169 6e2f 4c49 4345  s/blob/main/LICE
+00000580: 4e53 4529 0a5b 215b 444f 495d 2868 7474  NSE).[![DOI](htt
+00000590: 7073 3a2f 2f7a 656e 6f64 6f2e 6f72 672f  ps://zenodo.org/
+000005a0: 6261 6467 652f 3235 3538 3937 3832 2e73  badge/25589782.s
+000005b0: 7667 295d 2868 7474 7073 3a2f 2f7a 656e  vg)](https://zen
+000005c0: 6f64 6f2e 6f72 672f 6261 6467 652f 6c61  odo.org/badge/la
+000005d0: 7465 7374 646f 692f 3235 3538 3937 3832  testdoi/25589782
+000005e0: 290a 0a0a 2320 5370 6865 7269 6361 6c20  )...# Spherical 
+000005f0: 4675 6e63 7469 6f6e 730a 0a7c 204e 4f54  Functions..| NOT
+00000600: 453a 2054 6869 7320 7061 636b 6167 6520  E: This package 
+00000610: 7769 6c6c 2073 7469 6c6c 2062 6520 6d61  will still be ma
+00000620: 696e 7461 696e 6564 2c20 6275 7420 2a61  intained, but *a
+00000630: 6374 6976 652a 2064 6576 656c 6f70 6d65  ctive* developme
+00000640: 6e74 2068 6173 206d 6f76 6564 2074 6f20  nt has moved to 
+00000650: 7468 6520 5b60 7370 6865 7269 6361 6c60  the [`spherical`
+00000660: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000670: 2e63 6f6d 2f6d 6f62 6c65 2f73 7068 6572  .com/moble/spher
+00000680: 6963 616c 2920 7061 636b 6167 652e 2020  ical) package.  
+00000690: 5768 696c 6520 7468 6973 2070 6163 6b61  While this packa
+000006a0: 6765 2077 6f72 6b73 2077 656c 6c20 666f  ge works well fo
+000006b0: 7220 e284 9320 2861 6b61 2065 6c6c 2c20  r ... (aka ell, 
+000006c0: 4c2c 206a 2c20 6f72 204a 2920 7661 6c75  L, j, or J) valu
+000006d0: 6573 2075 7020 746f 2061 726f 756e 6420  es up to around 
+000006e0: 3235 2c20 6572 726f 7273 2073 7461 7274  25, errors start
+000006f0: 2074 6f20 6275 696c 6420 7261 7069 646c   to build rapidl
+00000700: 7920 616e 6420 7475 726e 2069 6e74 6f20  y and turn into 
+00000710: 4e61 4e73 2061 726f 756e 6420 3330 2e20  NaNs around 30. 
+00000720: 2054 6865 2060 7370 6865 7269 6361 6c60   The `spherical`
+00000730: 2070 6163 6b61 6765 2063 616e 2072 6561   package can rea
+00000740: 6469 6c79 2068 616e 646c 6520 7661 6c75  dily handle valu
+00000750: 6573 2075 7020 746f 2061 7420 6c65 6173  es up to at leas
+00000760: 7420 3130 3030 2c20 7769 7468 2061 6363  t 1000, with acc
+00000770: 7572 6163 7920 636c 6f73 6520 746f 20e2  uracy close to .
+00000780: 8493 2074 696d 6573 206d 6163 6869 6e65  .. times machine
+00000790: 2070 7265 6369 7369 6f6e 2e20 20e2 8094   precision.  ...
+000007a0: 4d69 6b65 207c 0a7c 202d 2d2d 207c 0a0a  Mike |.| --- |..
+000007b0: 0a50 7974 686f 6e2f 6e75 6d62 6120 7061  .Python/numba pa
+000007c0: 636b 6167 6520 666f 7220 6576 616c 7561  ckage for evalua
+000007d0: 7469 6e67 2061 6e64 2074 7261 6e73 666f  ting and transfo
+000007e0: 726d 696e 6720 5769 676e 6572 2773 20f0  rming Wigner's .
+000007f0: 9d94 8720 6d61 7472 6963 6573 2c0a 5769  ... matrices,.Wi
+00000800: 676e 6572 2773 2033 2d6a 2073 796d 626f  gner's 3-j symbo
+00000810: 6c73 2c20 616e 6420 7370 696e 2d77 6569  ls, and spin-wei
+00000820: 6768 7465 6420 2861 6e64 2073 6361 6c61  ghted (and scala
+00000830: 7229 2073 7068 6572 6963 616c 2068 6172  r) spherical har
+00000840: 6d6f 6e69 6373 2e0a 5468 6573 6520 6675  monics..These fu
+00000850: 6e63 7469 6f6e 7320 6172 6520 6576 616c  nctions are eval
+00000860: 7561 7465 6420 6469 7265 6374 6c79 2069  uated directly i
+00000870: 6e20 7465 726d 7320 6f66 2071 7561 7465  n terms of quate
+00000880: 726e 696f 6e73 2c20 6173 2077 656c 6c20  rnions, as well 
+00000890: 6173 2069 6e0a 7468 6520 6d6f 7265 2073  as in.the more s
+000008a0: 7461 6e64 6172 6420 666f 726d 7320 6f66  tandard forms of
+000008b0: 2073 7068 6572 6963 616c 2063 6f6f 7264   spherical coord
+000008c0: 696e 6174 6573 2061 6e64 2045 756c 6572  inates and Euler
+000008d0: 0a61 6e67 6c65 732e 3c73 7570 3e5b 315d  .angles.<sup>[1]
+000008e0: 2823 312d 6575 6c65 722d 616e 676c 6573  (#1-euler-angles
+000008f0: 2d61 7265 2d61 7766 756c 293c 2f73 7570  -are-awful)</sup
+00000900: 3e0a 0a54 6865 2063 6f6e 7665 6e74 696f  >..The conventio
+00000910: 6e73 2066 6f72 2074 6869 7320 7061 636b  ns for this pack
+00000920: 6167 6520 6172 6520 6465 7363 7269 6265  age are describe
+00000930: 6420 696e 2064 6574 6169 6c20 6f6e 0a5b  d in detail on.[
+00000940: 7468 6973 2070 6167 655d 2868 7474 703a  this page](http:
+00000950: 2f2f 6d6f 626c 652e 6769 7468 7562 2e69  //moble.github.i
+00000960: 6f2f 7370 6865 7269 6361 6c5f 6675 6e63  o/spherical_func
+00000970: 7469 6f6e 732f 292e 0a0a 2323 2044 6570  tions/)...## Dep
+00000980: 656e 6465 6e63 6965 730a 0a54 6865 206f  endencies..The o
+00000990: 6e6c 7920 7472 7565 2072 6571 7569 7265  nly true require
+000009a0: 6d65 6e74 7320 666f 7220 7468 6973 2063  ments for this c
+000009b0: 6f64 6520 6172 6520 6070 7974 686f 6e60  ode are `python`
+000009c0: 2061 6e64 2074 6865 2070 7974 686f 6e20   and the python 
+000009d0: 7061 636b 6167 650a 606e 756d 7079 602c  package.`numpy`,
+000009e0: 2061 7320 7765 6c6c 2061 7320 6d79 2061   as well as my a
+000009f0: 6363 6f6d 7061 6e79 696e 670a 5b60 7175  ccompanying.[`qu
+00000a00: 6174 6572 6e69 6f6e 605d 2868 7474 7073  aternion`](https
+00000a10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d6f  ://github.com/mo
+00000a20: 626c 652f 7175 6174 6572 6e69 6f6e 2920  ble/quaternion) 
+00000a30: 7061 636b 6167 6520 2869 6e73 7461 6c6c  package (install
+00000a40: 6174 696f 6e20 6f66 0a77 6869 6368 2069  ation of.which i
+00000a50: 7320 7368 6f77 6e20 6265 6c6f 7729 2e0a  s shown below)..
+00000a60: 0a48 6f77 6576 6572 2c20 7468 6973 2070  .However, this p
+00000a70: 6163 6b61 6765 2063 616e 2061 7574 6f6d  ackage can autom
+00000a80: 6174 6963 616c 6c79 2075 7365 0a5b 606e  atically use.[`n
+00000a90: 756d 6261 605d 2868 7474 703a 2f2f 6e75  umba`](http://nu
+00000aa0: 6d62 612e 7079 6461 7461 2e6f 7267 2f29  mba.pydata.org/)
+00000ab0: 2c20 7768 6963 6820 7573 6573 205b 4c4c  , which uses [LL
+00000ac0: 564d 5d28 6874 7470 3a2f 2f6c 6c76 6d2e  VM](http://llvm.
+00000ad0: 6f72 672f 2920 746f 0a63 6f6d 7069 6c65  org/) to.compile
+00000ae0: 2070 7974 686f 6e20 636f 6465 2074 6f20   python code to 
+00000af0: 6d61 6368 696e 6520 636f 6465 2c20 6163  machine code, ac
+00000b00: 6365 6c65 7261 7469 6e67 206d 6f73 7420  celerating most 
+00000b10: 6e75 6d65 7269 6361 6c20 6675 6e63 7469  numerical functi
+00000b20: 6f6e 7320 6279 0a66 6163 746f 7273 206f  ons by.factors o
+00000b30: 6620 616e 7977 6865 7265 2066 726f 6d20  f anywhere from 
+00000b40: 3220 746f 2032 3030 302e 2020 4974 2069  2 to 2000.  It i
+00000b50: 7320 2a70 6f73 7369 626c 652a 2074 6f20  s *possible* to 
+00000b60: 7275 6e20 7468 6520 636f 6465 2077 6974  run the code wit
+00000b70: 686f 7574 0a60 6e75 6d62 6160 2c20 6275  hout.`numba`, bu
+00000b80: 7420 7468 6520 6d6f 7374 2069 6d70 6f72  t the most impor
+00000b90: 7461 6e74 2066 756e 6374 696f 6e73 2061  tant functions a
+00000ba0: 7265 2072 6f75 6768 6c79 2031 3020 7469  re roughly 10 ti
+00000bb0: 6d65 7320 736c 6f77 6572 2077 6974 686f  mes slower witho
+00000bc0: 7574 0a69 742e 0a0a 5468 6520 6f6e 6c79  ut.it...The only
+00000bd0: 2064 7261 7762 6163 6b20 6f66 2060 6e75   drawback of `nu
+00000be0: 6d62 6160 2069 7320 7468 6174 2069 7420  mba` is that it 
+00000bf0: 6973 206e 6f6e 7472 6976 6961 6c20 746f  is nontrivial to
+00000c00: 2069 6e73 7461 6c6c 206f 6e20 6974 7320   install on its 
+00000c10: 6f77 6e2e 0a46 6f72 7475 6e61 7465 6c79  own..Fortunately
+00000c20: 2c20 7468 6520 6265 7374 2070 7974 686f  , the best pytho
+00000c30: 6e20 696e 7374 616c 6c65 722c 0a5b 6061  n installer,.[`a
+00000c40: 6e61 636f 6e64 6160 5d28 6874 7470 3a2f  naconda`](http:/
+00000c50: 2f63 6f6e 7469 6e75 756d 2e69 6f2f 646f  /continuum.io/do
+00000c60: 776e 6c6f 6164 7329 2c20 6d61 6b65 7320  wnloads), makes 
+00000c70: 6974 2074 7269 7669 616c 2e20 204a 7573  it trivial.  Jus
+00000c80: 7420 696e 7374 616c 6c0a 7468 6520 6d61  t install.the ma
+00000c90: 696e 2060 616e 6163 6f6e 6461 6020 7061  in `anaconda` pa
+00000ca0: 636b 6167 652e 0a0a 4966 2079 6f75 2070  ckage...If you p
+00000cb0: 7265 6665 7220 7468 6520 736d 616c 6c65  refer the smalle
+00000cc0: 7220 646f 776e 6c6f 6164 2073 697a 6520  r download size 
+00000cd0: 6f66 0a5b 606d 696e 6963 6f6e 6461 605d  of.[`miniconda`]
+00000ce0: 2868 7474 703a 2f2f 636f 6e64 612e 7079  (http://conda.py
+00000cf0: 6461 7461 2e6f 7267 2f6d 696e 6963 6f6e  data.org/minicon
+00000d00: 6461 2e68 746d 6c29 2028 7768 6963 6820  da.html) (which 
+00000d10: 636f 6d65 7320 7769 7468 206e 6f0a 6578  comes with no.ex
+00000d20: 7472 6173 2062 6579 6f6e 6420 7079 7468  tras beyond pyth
+00000d30: 6f6e 292c 2079 6f75 206d 6179 2061 6c73  on), you may als
+00000d40: 6f20 6861 7665 2074 6f20 7275 6e20 7468  o have to run th
+00000d50: 6973 2063 6f6d 6d61 6e64 3a0a 0a60 6060  is command:..```
+00000d60: 7368 0a63 6f6e 6461 2069 6e73 7461 6c6c  sh.conda install
+00000d70: 2070 6970 206e 756d 7079 206e 756d 6261   pip numpy numba
+00000d80: 0a60 6060 0a0a 0a23 2320 496e 7374 616c  .```...## Instal
+00000d90: 6c61 7469 6f6e 0a0a 4173 7375 6d69 6e67  lation..Assuming
+00000da0: 2079 6f75 2075 7365 2060 636f 6e64 6160   you use `conda`
+00000db0: 2074 6f20 6d61 6e61 6765 2079 6f75 7220   to manage your 
+00000dc0: 7079 7468 6f6e 2069 6e73 7461 6c6c 6174  python installat
+00000dd0: 696f 6e20 286c 696b 6520 616e 7920 7361  ion (like any sa
+00000de0: 6e65 0a70 7974 686f 6e20 7573 6572 292c  ne.python user),
+00000df0: 2079 6f75 2063 616e 2069 6e73 7461 6c6c   you can install
+00000e00: 2074 6869 7320 7061 636b 6167 6520 7369   this package si
+00000e10: 6d70 6c79 2061 730a 0a60 6060 7368 0a63  mply as..```sh.c
+00000e20: 6f6e 6461 2069 6e73 7461 6c6c 202d 6320  onda install -c 
+00000e30: 636f 6e64 612d 666f 7267 6520 7370 6865  conda-forge sphe
+00000e40: 7269 6361 6c5f 6675 6e63 7469 6f6e 730a  rical_functions.
+00000e50: 6060 600a 0a54 6869 7320 7368 6f75 6c64  ```..This should
+00000e60: 2061 7574 6f6d 6174 6963 616c 6c79 2064   automatically d
+00000e70: 6f77 6e6c 6f61 6420 616e 6420 696e 7374  ownload and inst
+00000e80: 616c 6c20 7468 6520 7061 636b 6167 650a  all the package.
+00000e90: 5b60 7175 6174 6572 6e69 6f6e 605d 2868  [`quaternion`](h
+00000ea0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000eb0: 6d2f 6d6f 626c 652f 7175 6174 6572 6e69  m/moble/quaterni
+00000ec0: 6f6e 292c 206f 6e20 7768 6963 6820 7468  on), on which th
+00000ed0: 6973 2070 6163 6b61 6765 0a64 6570 656e  is package.depen
+00000ee0: 6473 2e0a 0a41 6c74 6572 6e61 7469 7665  ds...Alternative
+00000ef0: 6c79 2c20 6966 2079 6f75 2070 7265 6665  ly, if you prefe
+00000f00: 7220 746f 2075 7365 2060 7069 7060 2028  r to use `pip` (
+00000f10: 7768 6574 6865 7220 6f72 206e 6f74 2079  whether or not y
+00000f20: 6f75 2075 7365 2060 636f 6e64 6160 292c  ou use `conda`),
+00000f30: 2079 6f75 0a63 616e 2061 6c73 6f20 646f   you.can also do
+00000f40: 0a0a 6060 6073 680a 7079 7468 6f6e 202d  ..```sh.python -
+00000f50: 6d20 7069 7020 696e 7374 616c 6c20 7370  m pip install sp
+00000f60: 6865 7269 6361 6c2d 6675 6e63 7469 6f6e  herical-function
+00000f70: 730a 6060 600a 0a46 696e 616c 6c79 2c20  s.```..Finally, 
+00000f80: 7468 6572 6527 7320 616c 736f 2074 6865  there's also the
+00000f90: 2066 756c 6c79 206d 616e 7561 6c20 6f70   fully manual op
+00000fa0: 7469 6f6e 206f 6620 6a75 7374 2064 6f77  tion of just dow
+00000fb0: 6e6c 6f61 6469 6e67 2062 6f74 6820 636f  nloading both co
+00000fc0: 6465 0a72 6570 6f73 6974 6f72 6965 732c  de.repositories,
+00000fd0: 2063 6861 6e67 696e 6720 746f 2074 6865   changing to the
+00000fe0: 2063 6f64 6520 6469 7265 6374 6f72 792c   code directory,
+00000ff0: 2061 6e64 2069 7373 7569 6e67 0a0a 6060   and issuing..``
+00001000: 6073 680a 7079 7468 6f6e 202d 6d20 7069  `sh.python -m pi
+00001010: 7020 696e 7374 616c 6c20 2e0a 6060 600a  p install ..```.
+00001020: 0a54 6869 7320 7368 6f75 6c64 2077 6f72  .This should wor
+00001030: 6b20 7265 6761 7264 6c65 7373 206f 6620  k regardless of 
+00001040: 7468 6520 696e 7374 616c 6c61 7469 6f6e  the installation
+00001050: 206d 6574 686f 642c 2061 7320 6c6f 6e67   method, as long
+00001060: 2061 7320 796f 7520 6861 7665 2061 0a63   as you have a.c
+00001070: 6f6d 7069 6c65 7220 6861 6e67 696e 6720  ompiler hanging 
+00001080: 6172 6f75 6e64 2e20 2048 6f77 6576 6572  around.  However
+00001090: 2c20 7468 6973 206d 6179 2062 6520 6d6f  , this may be mo
+000010a0: 7265 206c 696b 656c 7920 746f 2074 7279  re likely to try
+000010b0: 2074 6f20 636f 6d70 696c 650a 7468 6520   to compile.the 
+000010c0: 6465 7065 6e64 656e 6369 6573 2c20 696e  dependencies, in
+000010d0: 636c 7564 696e 6720 6e75 6d70 7920 616e  cluding numpy an
+000010e0: 642f 6f72 2073 7069 6e73 6661 7374 2c20  d/or spinsfast, 
+000010f0: 7768 6963 6820 6361 6e20 6265 206d 7563  which can be muc
+00001100: 6820 6d6f 7265 0a63 6f6d 706c 6963 6174  h more.complicat
+00001110: 6564 2e0a 0a0a 2323 2055 7361 6765 0a0a  ed....## Usage..
+00001120: 4669 7273 742c 2077 6520 7368 6f77 2061  First, we show a
+00001130: 2076 6572 7920 7369 6d70 6c65 2065 7861   very simple exa
+00001140: 6d70 6c65 206f 6620 7573 6167 6520 7769  mple of usage wi
+00001150: 7468 2045 756c 6572 2061 6e67 6c65 732c  th Euler angles,
+00001160: 2074 686f 7567 6820 6974 0a62 7265 616b   though it.break
+00001170: 7320 6d79 2068 6561 7274 2074 6f20 646f  s my heart to do
+00001180: 2073 6f3a 3c73 7570 3e5b 315d 2823 6575   so:<sup>[1](#eu
+00001190: 6c65 722d 616e 676c 6573 2d61 7265 2d61  ler-angles-are-a
+000011a0: 7766 756c 293c 2f73 7570 3e0a 0a60 6060  wful)</sup>..```
+000011b0: 7079 7468 6f6e 0a3e 3e3e 2069 6d70 6f72  python.>>> impor
+000011c0: 7420 7370 6865 7269 6361 6c5f 6675 6e63  t spherical_func
+000011d0: 7469 6f6e 7320 6173 2073 660a 3e3e 3e20  tions as sf.>>> 
+000011e0: 616c 7068 612c 2062 6574 612c 2067 616d  alpha, beta, gam
+000011f0: 6d61 203d 2030 2e31 2c20 302e 322c 2030  ma = 0.1, 0.2, 0
+00001200: 2e33 0a3e 3e3e 2065 6c6c 2c6d 702c 6d20  .3.>>> ell,mp,m 
+00001210: 3d20 332c 322c 310a 3e3e 3e20 7366 2e57  = 3,2,1.>>> sf.W
+00001220: 6967 6e65 725f 445f 656c 656d 656e 7428  igner_D_element(
+00001230: 616c 7068 612c 2062 6574 612c 2067 616d  alpha, beta, gam
+00001240: 6d61 2c20 656c 6c2c 206d 702c 206d 290a  ma, ell, mp, m).
+00001250: 0a60 6060 0a0a 4f66 2063 6f75 7273 652c  .```..Of course,
+00001260: 2069 7427 7320 616c 7761 7973 2062 6574   it's always bet
+00001270: 7465 7220 746f 2075 7365 2075 6e69 7420  ter to use unit 
+00001280: 7175 6174 6572 6e69 6f6e 7320 746f 2064  quaternions to d
+00001290: 6573 6372 6962 6520 726f 7461 7469 6f6e  escribe rotation
+000012a0: 733a 0a0a 6060 6070 7974 686f 6e0a 3e3e  s:..```python.>>
+000012b0: 3e20 696d 706f 7274 206e 756d 7079 2061  > import numpy a
+000012c0: 7320 6e70 0a3e 3e3e 2069 6d70 6f72 7420  s np.>>> import 
+000012d0: 7175 6174 6572 6e69 6f6e 0a3e 3e3e 2052  quaternion.>>> R
+000012e0: 203d 206e 702e 7175 6174 6572 6e69 6f6e   = np.quaternion
+000012f0: 2831 2c32 2c33 2c34 292e 6e6f 726d 616c  (1,2,3,4).normal
+00001300: 697a 6564 2829 0a3e 3e3e 2065 6c6c 2c6d  ized().>>> ell,m
+00001310: 702c 6d20 3d20 332c 322c 310a 3e3e 3e20  p,m = 3,2,1.>>> 
+00001320: 7366 2e57 6967 6e65 725f 445f 656c 656d  sf.Wigner_D_elem
+00001330: 656e 7428 522c 2065 6c6c 2c20 6d70 2c20  ent(R, ell, mp, 
+00001340: 6d29 0a0a 6060 600a 0a49 6620 796f 7520  m)..```..If you 
+00001350: 6e65 6564 2074 6f20 6361 6c63 756c 6174  need to calculat
+00001360: 6520 7661 6c75 6573 206f 6620 7468 6520  e values of the 
+00001370: f09d 9487 3c73 7570 3e28 e284 9329 3c2f  ....<sup>(...)</
+00001380: 7375 703e 206d 6174 7269 7820 656c 656d  sup> matrix elem
+00001390: 656e 7473 2066 6f72 206d 616e 790a 7661  ents for many.va
+000013a0: 6c75 6573 206f 6620 28e2 8493 2c20 6d27  lues of (..., m'
+000013b0: 2c20 6d29 2c20 6974 2069 7320 6d6f 7265  , m), it is more
+000013c0: 2065 6666 6963 6965 6e74 2074 6f20 646f   efficient to do
+000013d0: 2073 6f20 616c 6c20 6174 206f 6e63 652e   so all at once.
+000013e0: 2020 5468 6520 666f 6c6c 6f77 696e 670a    The following.
+000013f0: 6361 6c63 756c 6174 6573 2061 6c6c 206d  calculates all m
+00001400: 6f64 6573 2066 6f72 20e2 8493 2066 726f  odes for ... fro
+00001410: 6d20 3220 746f 2038 2028 696e 636c 7573  m 2 to 8 (inclus
+00001420: 6976 6529 3a0a 0a60 6060 7079 7468 6f6e  ive):..```python
+00001430: 0a3e 3e3e 2069 6e64 6963 6573 203d 206e  .>>> indices = n
+00001440: 702e 6172 7261 7928 5b5b 656c 6c2c 6d70  p.array([[ell,mp
+00001450: 2c6d 5d20 666f 7220 656c 6c20 696e 2072  ,m] for ell in r
+00001460: 616e 6765 2832 2c39 290a 2e2e 2e20 666f  ange(2,9).... fo
+00001470: 7220 6d70 2069 6e20 7261 6e67 6528 2d65  r mp in range(-e
+00001480: 6c6c 2c20 656c 6c2b 3129 2066 6f72 206d  ll, ell+1) for m
+00001490: 2069 6e20 7261 6e67 6528 2d65 6c6c 2c20   in range(-ell, 
+000014a0: 656c 6c2b 3129 5d29 0a3e 3e3e 2073 662e  ell+1)]).>>> sf.
+000014b0: 5769 676e 6572 5f44 5f65 6c65 6d65 6e74  Wigner_D_element
+000014c0: 2852 2c20 696e 6469 6365 7329 0a0a 6060  (R, indices)..``
+000014d0: 600a 0a46 696e 616c 6c79 2c20 6966 2079  `..Finally, if y
+000014e0: 6f75 2072 6561 6c6c 7920 6e65 6564 2074  ou really need t
+000014f0: 6f20 7075 7420 7468 6520 7065 6461 6c20  o put the pedal 
+00001500: 746f 2074 6865 206d 6574 616c 2c20 616e  to the metal, an
+00001510: 6420 6172 6520 7769 6c6c 696e 6720 746f  d are willing to
+00001520: 0a67 7561 7261 6e74 6565 2074 6861 7420  .guarantee that 
+00001530: 7468 6520 696e 7075 7420 6172 6775 6d65  the input argume
+00001540: 6e74 7320 6172 6520 636f 7272 6563 742c  nts are correct,
+00001550: 2079 6f75 2063 616e 2075 7365 2061 2073   you can use a s
+00001560: 7065 6369 616c 2068 6964 6465 6e0a 666f  pecial hidden.fo
+00001570: 726d 206f 6620 7468 6520 6675 6e63 7469  rm of the functi
+00001580: 6f6e 3a0a 0a60 6060 7079 7468 6f6e 0a3e  on:..```python.>
+00001590: 3e3e 2073 662e 5f57 6967 6e65 725f 445f  >> sf._Wigner_D_
+000015a0: 656c 656d 656e 7428 522e 612c 2052 2e62  element(R.a, R.b
+000015b0: 2c20 696e 6469 6365 732c 2065 6c65 6d65  , indices, eleme
+000015c0: 6e74 7329 0a0a 6060 600a 0a48 6572 652c  nts)..```..Here,
+000015d0: 2060 522e 6160 2061 6e64 2060 522e 6260   `R.a` and `R.b`
+000015e0: 2061 7265 2074 6865 2074 776f 2063 6f6d   are the two com
+000015f0: 706c 6578 2070 6172 7473 206f 6620 7468  plex parts of th
+00001600: 6520 7175 6174 6572 6e69 6f6e 2064 6566  e quaternion def
+00001610: 696e 6564 206f 6e0a 5b74 6869 7320 7061  ined on.[this pa
+00001620: 6765 5d28 6874 7470 3a2f 2f6d 6f62 6c65  ge](http://moble
+00001630: 2e67 6974 6875 622e 696f 2f73 7068 6572  .github.io/spher
+00001640: 6963 616c 5f66 756e 6374 696f 6e73 2f29  ical_functions/)
+00001650: 2028 7468 6f75 6768 2074 6865 2075 7365   (though the use
+00001660: 7220 6e65 6564 0a6e 6f74 2063 6172 6520  r need.not care 
+00001670: 6162 6f75 7420 7468 6174 292e 2020 5468  about that).  Th
+00001680: 6520 6069 6e64 6963 6573 6020 7661 7269  e `indices` vari
+00001690: 6162 6c65 2069 7320 6173 7375 6d65 6420  able is assumed 
+000016a0: 746f 2062 6520 610a 7477 6f2d 6469 6d65  to be a.two-dime
+000016b0: 6e73 696f 6e61 6c20 6172 7261 7920 6f66  nsional array of
+000016c0: 2069 6e74 6567 6572 732c 2077 6865 7265   integers, where
+000016d0: 2074 6865 2073 6563 6f6e 6420 6469 6d65   the second dime
+000016e0: 6e73 696f 6e20 6861 7320 7369 7a65 2074  nsion has size t
+000016f0: 6872 6565 2c0a 7265 7072 6573 656e 7469  hree,.representi
+00001700: 6e67 2074 6865 2028 e284 932c 206d 272c  ng the (..., m',
+00001710: 206d 2920 696e 6469 6365 732e 2020 5468   m) indices.  Th
+00001720: 6973 2061 766f 6964 7320 6365 7274 6169  is avoids certai
+00001730: 6e20 736f 6d65 7768 6174 2073 6c6f 7765  n somewhat slowe
+00001740: 720a 7075 7265 2d70 7974 686f 6e20 6f70  r.pure-python op
+00001750: 6572 6174 696f 6e73 2069 6e76 6f6c 7669  erations involvi
+00001760: 6e67 2061 7267 756d 656e 7420 6368 6563  ng argument chec
+00001770: 6b69 6e67 2c20 7265 7368 6170 696e 672c  king, reshaping,
+00001780: 2065 7463 2e20 2054 6865 0a60 656c 656d   etc.  The.`elem
+00001790: 656e 7473 6020 7661 7269 6162 6c65 206d  ents` variable m
+000017a0: 7573 7420 6265 2061 206f 6e65 2d64 696d  ust be a one-dim
+000017b0: 656e 7369 6f6e 616c 2061 7272 6179 206f  ensional array o
+000017c0: 6620 636f 6d70 6c65 7820 6e75 6d62 6572  f complex number
+000017d0: 7320 2863 616e 2062 650a 756e 696e 6974  s (can be.uninit
+000017e0: 6961 6c69 7a65 6429 2c20 7768 6963 6820  ialized), which 
+000017f0: 7769 6c6c 2062 6520 7265 706c 6163 6564  will be replaced
+00001800: 2077 6974 6820 7468 6520 636f 7272 6573   with the corres
+00001810: 706f 6e64 696e 6720 7661 6c75 6573 206f  ponding values o
+00001820: 6e20 7265 7475 726e 2e0a 4167 6169 6e2c  n return..Again,
+00001830: 2068 6f77 6576 6572 2c20 7468 6572 6520   however, there 
+00001840: 6973 206e 6f20 696e 7075 7420 6469 6d65  is no input dime
+00001850: 6e73 696f 6e20 6368 6563 6b69 6e67 2068  nsion checking h
+00001860: 6572 652c 2073 6f20 6966 2079 6f75 2067  ere, so if you g
+00001870: 6976 6520 6261 640a 696e 7075 7473 2c20  ive bad.inputs, 
+00001880: 6265 6861 7669 6f72 2063 6f75 6c64 2072  behavior could r
+00001890: 616e 6765 2066 726f 6d20 7369 6c65 6e74  ange from silent
+000018a0: 6c79 2077 726f 6e67 2074 6f20 6578 6365  ly wrong to exce
+000018b0: 7074 696f 6e73 2074 6f20 7365 676d 656e  ptions to segmen
+000018c0: 7461 7469 6f6e 0a66 6175 6c74 732e 2020  tation.faults.  
+000018d0: 4361 7665 6174 2065 6d70 746f 722e 0a0a  Caveat emptor...
+000018e0: 0a23 2320 4163 6b6e 6f77 6c65 6467 6d65  .## Acknowledgme
+000018f0: 6e74 730a 0a49 2076 6572 7920 6d75 6368  nts..I very much
+00001900: 2061 7070 7265 6369 6174 6520 4261 7272   appreciate Barr
+00001910: 7920 5761 7264 656c 6c27 7320 6865 6c70  y Wardell's help
+00001920: 2069 6e20 736f 7274 696e 6720 6f75 7420   in sorting out 
+00001930: 7468 6520 7265 6c61 7469 6f6e 7368 6970  the relationship
+00001940: 730a 6265 7477 6565 6e20 6d79 2063 6f6e  s.between my con
+00001950: 7665 6e74 696f 6e73 2061 6e64 2074 686f  ventions and tho
+00001960: 7365 206f 6620 6f74 6865 7220 7065 6f70  se of other peop
+00001970: 6c65 2061 6e64 2073 6f66 7477 6172 6520  le and software 
+00001980: 7061 636b 6167 6573 0a28 6573 7065 6369  packages.(especi
+00001990: 616c 6c79 204d 6174 6865 6d61 7469 6361  ally Mathematica
+000019a0: 2773 2063 7261 7a79 2063 6f6e 7665 6e74  's crazy convent
+000019b0: 696f 6e73 292e 0a0a 5468 6973 2063 6f64  ions)...This cod
+000019c0: 6520 6973 2c20 6f66 2063 6f75 7273 652c  e is, of course,
+000019d0: 2068 6f73 7465 6420 6f6e 2067 6974 6875   hosted on githu
+000019e0: 622e 2020 4265 6361 7573 6520 6974 2069  b.  Because it i
+000019f0: 7320 616e 206f 7065 6e2d 736f 7572 6365  s an open-source
+00001a00: 0a70 726f 6a65 6374 2c20 7468 6520 686f  .project, the ho
+00001a10: 7374 696e 6720 6973 2066 7265 652c 2061  sting is free, a
+00001a20: 6e64 2061 6c6c 2074 6865 2077 6f6e 6465  nd all the wonde
+00001a30: 7266 756c 2066 6561 7475 7265 7320 6f66  rful features of
+00001a40: 2067 6974 6875 6220 6172 650a 6176 6169   github are.avai
+00001a50: 6c61 626c 652c 2069 6e63 6c75 6469 6e67  lable, including
+00001a60: 2066 7265 6520 7769 6b69 2073 7061 6365   free wiki space
+00001a70: 2061 6e64 2077 6562 2070 6167 6520 686f   and web page ho
+00001a80: 7374 696e 672c 2070 756c 6c20 7265 7175  sting, pull requ
+00001a90: 6573 7473 2c20 610a 6e69 6365 2069 6e74  ests, a.nice int
+00001aa0: 6572 6661 6365 2074 6f20 7468 6520 6769  erface to the gi
+00001ab0: 7420 6c6f 6773 2c20 6574 632e 0a0a 4669  t logs, etc...Fi
+00001ac0: 6e61 6c6c 792c 2074 6865 2063 6f64 6520  nally, the code 
+00001ad0: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
+00001ae0: 2063 6f6d 7069 6c65 642c 2061 6e64 2074   compiled, and t
+00001af0: 6865 2062 696e 6172 6965 7320 686f 7374  he binaries host
+00001b00: 6564 2066 6f72 0a64 6f77 6e6c 6f61 6420  ed for.download 
+00001b10: 6279 2060 636f 6e64 6160 206f 6e20 5b61  by `conda` on [a
+00001b20: 6e61 636f 6e64 612e 6f72 675d 2868 7474  naconda.org](htt
+00001b30: 7073 3a2f 2f61 6e61 636f 6e64 612e 6f72  ps://anaconda.or
+00001b40: 672f 6d6f 626c 652f 7370 6865 7269 6361  g/moble/spherica
+00001b50: 6c5f 6675 6e63 7469 6f6e 7329 2e0a 5468  l_functions)..Th
+00001b60: 6973 2069 7320 616c 736f 2061 2066 7265  is is also a fre
+00001b70: 6520 7365 7276 6963 6520 666f 7220 6f70  e service for op
+00001b80: 656e 2d73 6f75 7263 6520 7072 6f6a 6563  en-source projec
+00001b90: 7473 206c 696b 6520 7468 6973 206f 6e65  ts like this one
+00001ba0: 2e0a 0a54 6865 2077 6f72 6b20 6f66 2063  ...The work of c
+00001bb0: 7265 6174 696e 6720 7468 6973 2063 6f64  reating this cod
+00001bc0: 6520 7761 7320 7375 7070 6f72 7465 6420  e was supported 
+00001bd0: 696e 2070 6172 7420 6279 2074 6865 2053  in part by the S
+00001be0: 6865 726d 616e 2046 6169 7263 6869 6c64  herman Fairchild
+00001bf0: 0a46 6f75 6e64 6174 696f 6e20 616e 6420  .Foundation and 
+00001c00: 6279 204e 5346 2047 7261 6e74 7320 4e6f  by NSF Grants No
+00001c10: 2e20 5048 592d 3133 3036 3132 3520 616e  . PHY-1306125 an
+00001c20: 6420 4153 542d 3133 3333 3132 392e 0a0a  d AST-1333129...
+00001c30: 0a3c 6272 2f3e 0a2d 2d2d 0a23 2323 2323  .<br/>.---.#####
+00001c40: 2320 3c73 7570 3e31 3c2f 7375 703e 2045  # <sup>1</sup> E
+00001c50: 756c 6572 2061 6e67 6c65 7320 6172 6520  uler angles are 
+00001c60: 6177 6675 6c0a 0a45 756c 6572 2061 6e67  awful..Euler ang
+00001c70: 6c65 7320 6172 6520 7072 6574 7479 206d  les are pretty m
+00001c80: 7563 680a 5b74 6865 2077 6f72 7374 2074  uch.[the worst t
+00001c90: 6869 6e67 7320 6576 6572 5d28 6874 7470  hings ever](http
+00001ca0: 3a2f 2f6d 6f62 6c65 2e67 6974 6875 622e  ://moble.github.
+00001cb0: 696f 2f73 7068 6572 6963 616c 5f66 756e  io/spherical_fun
+00001cc0: 6374 696f 6e73 2f23 6575 6c65 722d 616e  ctions/#euler-an
+00001cd0: 676c 6573 290a 616e 6420 6974 206d 616b  gles).and it mak
+00001ce0: 6573 206d 6520 6665 656c 2062 6164 2065  es me feel bad e
+00001cf0: 7665 6e20 7375 7070 6f72 7469 6e67 2074  ven supporting t
+00001d00: 6865 6d2e 2020 5175 6174 6572 6e69 6f6e  hem.  Quaternion
+00001d10: 7320 6172 650a 6661 7374 6572 2c20 6d6f  s are.faster, mo
+00001d20: 7265 2061 6363 7572 6174 652c 2062 6173  re accurate, bas
+00001d30: 6963 616c 6c79 2066 7265 6520 6f66 2073  ically free of s
+00001d40: 696e 6775 6c61 7269 7469 6573 2c20 6d6f  ingularities, mo
+00001d50: 7265 0a69 6e74 7569 7469 7665 2c20 616e  re.intuitive, an
+00001d60: 6420 6765 6e65 7261 6c6c 7920 6561 7369  d generally easi
+00001d70: 6572 2074 6f20 756e 6465 7273 7461 6e64  er to understand
+00001d80: 2e20 2059 6f75 2063 616e 2077 6f72 6b20  .  You can work 
+00001d90: 656e 7469 7265 6c79 0a77 6974 686f 7574  entirely.without
+00001da0: 2045 756c 6572 2061 6e67 6c65 7320 2849   Euler angles (I
+00001db0: 2063 6572 7461 696e 6c79 2064 6f29 2e20   certainly do). 
+00001dc0: 2059 6f75 2061 6273 6f6c 7574 656c 7920   You absolutely 
+00001dd0: 6e65 7665 7220 6e65 6564 0a74 6865 6d2e  never need.them.
+00001de0: 2020 4275 7420 6966 2079 6f75 2772 6520    But if you're 
+00001df0: 736f 206f 6c64 2066 6173 6869 6f6e 6564  so old fashioned
+00001e00: 2074 6861 7420 796f 7520 7265 616c 6c79   that you really
+00001e10: 2063 616e 2774 2067 6976 6520 7468 656d   can't give them
+00001e20: 0a75 702c 2074 6865 7920 6172 6520 6675  .up, they are fu
+00001e30: 6c6c 7920 7375 7070 6f72 7465 642e 0a0a  lly supported...
```

