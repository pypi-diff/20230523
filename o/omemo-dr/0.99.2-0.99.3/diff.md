# Comparing `tmp/omemo-dr-0.99.2.tar.gz` & `tmp/omemo-dr-0.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omemo-dr-0.99.2.tar", last modified: Sat May 13 17:04:49 2023, max compression
+gzip compressed data, was "omemo-dr-0.99.3.tar", last modified: Mon May 22 23:25:27 2023, max compression
```

## Comparing `omemo-dr-0.99.2.tar` & `omemo-dr-0.99.3.tar`

### file list

```diff
@@ -1,206 +1,205 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.074070 omemo-dr-0.99.2/
--rw-rw-rw-   0 root         (0) root         (0)    35122 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    43030 2023-05-13 17:04:49.074070 omemo-dr-0.99.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1962 2023-05-11 21:04:20.000000 omemo-dr-0.99.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.046067 omemo-dr-0.99.2/curve25519/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.046067 omemo-dr-0.99.2/curve25519/curve/
--rw-rw-rw-   0 root         (0) root         (0)    31932 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/curve25519-donna.c
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/curve25519-donna.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.054068 omemo-dr-0.99.2/curve25519/curve/ed25519/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.058068 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/compare.c
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/compare.h
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/convert.c
--rw-rw-rw-   0 root         (0) root         (0)     1624 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/crypto_additions.h
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/crypto_hash_sha512.h
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/curve_sigs.c
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/curve_sigs.h
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ed_sigs.c
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ed_sigs.h
--rw-rw-rw-   0 root         (0) root         (0)     2236 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/elligator.c
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/fe_edy_to_montx.c
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/fe_isequal.c
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/fe_isreduced.c
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/fe_mont_rhs.c
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/fe_montx_to_edy.c
--rw-rw-rw-   0 root         (0) root         (0)     1355 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/fe_sqrt.c
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ge_isneutral.c
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ge_montx_to_p3.c
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ge_neg.c
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ge_p3_to_montx.c
--rw-rw-rw-   0 root         (0) root         (0)     3141 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ge_scalarmult.c
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ge_scalarmult_cofactor.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.062069 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_constants.h
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_crypto_additions.h
--rw-rw-rw-   0 root         (0) root         (0)     2660 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_labelset.h
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h
--rw-rw-rw-   0 root         (0) root         (0)     1821 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_x.h
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/keygen.c
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/keygen.h
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/open_modified.c
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/sc_clamp.c
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/sc_cmov.c
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/sc_neg.c
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/sign_modified.c
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/utility.c
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/utility.h
--rw-rw-rw-   0 root         (0) root         (0)     2367 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/xeddsa.c
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/xeddsa.h
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/zeroize.c
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/additions/zeroize.h
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/api.h
--rw-rw-rw-   0 root         (0) root         (0)    76457 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/base.h
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/base2.h
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/d.h
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/d2.h
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe.h
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_0.c
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_1.c
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_add.c
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_cmov.c
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_copy.c
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_frombytes.c
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_invert.c
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_isnegative.c
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_isnonzero.c
--rw-rw-rw-   0 root         (0) root         (0)    10744 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_mul.c
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_neg.c
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_pow22523.c
--rw-rw-rw-   0 root         (0) root         (0)     5980 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_sq.c
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_sq2.c
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_sub.c
--rw-rw-rw-   0 root         (0) root         (0)     3189 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/fe_tobytes.c
--rw-rw-rw-   0 root         (0) root         (0)     2869 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge.h
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_add.c
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_add.h
--rw-rw-rw-   0 root         (0) root         (0)     2371 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_double_scalarmult.c
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_frombytes.c
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_madd.c
--rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_madd.h
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_msub.c
--rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_msub.h
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p1p1_to_p2.c
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p1p1_to_p3.c
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p2_0.c
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p2_dbl.c
--rw-rw-rw-   0 root         (0) root         (0)     1476 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p2_dbl.h
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p3_0.c
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p3_dbl.c
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p3_to_cached.c
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p3_to_p2.c
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p3_tobytes.c
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_precomp_0.c
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_scalarmult_base.c
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_sub.c
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_sub.h
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/ge_tobytes.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.062069 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_int32.h
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_int64.h
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_sign.h
--rw-rw-rw-   0 root         (0) root         (0)     2034 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_uint32.h
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_uint64.h
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.062069 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_sha512/
--rw-rw-rw-   0 root         (0) root         (0)     6416 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_sha512/blocks.c
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_sha512/hash.c
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/open.c
--rw-rw-rw-   0 root         (0) root         (0)     5518 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/pow22523.h
--rw-rw-rw-   0 root         (0) root         (0)     5527 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/pow225521.h
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/sc.h
--rw-rw-rw-   0 root         (0) root         (0)    12494 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/sc_muladd.c
--rw-rw-rw-   0 root         (0) root         (0)     8139 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/sc_reduce.c
--rw-rw-rw-   0 root         (0) root         (0)      817 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/sign.c
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/sqrtm1.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.062069 omemo-dr-0.99.2/curve25519/curve/ed25519/tests/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/tests/internal_fast_tests.h
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/curve25519/curve/ed25519/tests/internal_slow_tests.h
--rw-rw-rw-   0 root         (0) root         (0)     8040 2023-04-09 19:22:07.000000 omemo-dr-0.99.2/curve25519/curve25519module.c
--rw-rw-rw-   0 root         (0) root         (0)     4767 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-13 17:04:49.074070 omemo-dr-0.99.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-03-26 20:37:13.000000 omemo-dr-0.99.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.042067 omemo-dr-0.99.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.062069 omemo-dr-0.99.2/src/omemo_dr/
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-13 17:02:26.000000 omemo-dr-0.99.2/src/omemo_dr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2254 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/src/omemo_dr/aes.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.066069 omemo-dr-0.99.2/src/omemo_dr/curve/
--rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/src/omemo_dr/curve/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.066069 omemo-dr-0.99.2/src/omemo_dr/ecc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/src/omemo_dr/ecc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/ecc/curve.py
--rw-rw-rw-   0 root         (0) root         (0)     2713 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/ecc/djbec.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-08 20:42:25.000000 omemo-dr-0.99.2/src/omemo_dr/ecc/ec.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/ecc/eckeypair.py
--rw-rw-rw-   0 root         (0) root         (0)     1252 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/src/omemo_dr/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/identitykey.py
--rw-rw-rw-   0 root         (0) root         (0)     1556 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/identitykeypair.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.066069 omemo-dr-0.99.2/src/omemo_dr/kdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/src/omemo_dr/kdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/src/omemo_dr/kdf/derivedmessagesecrets.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/src/omemo_dr/kdf/derivedrootsecrets.py
--rw-rw-rw-   0 root         (0) root         (0)     1736 2023-05-11 18:26:34.000000 omemo-dr-0.99.2/src/omemo_dr/kdf/hkdf.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/src/omemo_dr/kdf/messagekeys.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-07 15:19:42.000000 omemo-dr-0.99.2/src/omemo_dr/observable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.066069 omemo-dr-0.99.2/src/omemo_dr/protocol/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/src/omemo_dr/protocol/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/src/omemo_dr/protocol/ciphertextmessage.py
--rw-rw-rw-   0 root         (0) root         (0)     4076 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/protocol/omemo_keyexchange.py
--rw-rw-rw-   0 root         (0) root         (0)     5152 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/protocol/omemo_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/protocol/omemo_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5046 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/protocol/prekeywhispermessage.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/protocol/whisper_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4943 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/protocol/whispermessage.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/src/omemo_dr/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.070070 omemo-dr-0.99.2/src/omemo_dr/ratchet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/src/omemo_dr/ratchet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/ratchet/aliceparameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-11 18:26:34.000000 omemo-dr-0.99.2/src/omemo_dr/ratchet/bobparameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/ratchet/chainkey.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2023-05-11 18:26:34.000000 omemo-dr-0.99.2/src/omemo_dr/ratchet/ratchetingsession.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-05-06 21:36:18.000000 omemo-dr-0.99.2/src/omemo_dr/ratchet/rootkey.py
--rw-rw-rw-   0 root         (0) root         (0)    19091 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/session_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5487 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/sessionbuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    10889 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/sessioncipher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.070070 omemo-dr-0.99.2/src/omemo_dr/state/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/src/omemo_dr/state/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2812 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/state/prekeybundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/state/prekeyrecord.py
--rw-rw-rw-   0 root         (0) root         (0)     2991 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/state/sessionrecord.py
--rw-rw-rw-   0 root         (0) root         (0)    12879 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/state/sessionstate.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/state/signedprekeyrecord.py
--rw-rw-rw-   0 root         (0) root         (0)     5950 2023-05-11 19:26:44.000000 omemo-dr-0.99.2/src/omemo_dr/state/storage_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4777 2023-05-07 10:04:54.000000 omemo-dr-0.99.2/src/omemo_dr/state/store.py
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/structs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.070070 omemo-dr-0.99.2/src/omemo_dr/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/src/omemo_dr/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/src/omemo_dr/util/byteutil.py
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-05-07 18:48:15.000000 omemo-dr-0.99.2/src/omemo_dr/util/keyhelper.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-07 18:48:15.000000 omemo-dr-0.99.2/src/omemo_dr/util/logging.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/src/omemo_dr/util/medium.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.066069 omemo-dr-0.99.2/src/omemo_dr.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43030 2023-05-13 17:04:49.000000 omemo-dr-0.99.2/src/omemo_dr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6870 2023-05-13 17:04:49.000000 omemo-dr-0.99.2/src/omemo_dr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 17:04:49.000000 omemo-dr-0.99.2/src/omemo_dr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-13 17:04:49.000000 omemo-dr-0.99.2/src/omemo_dr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-13 17:04:49.000000 omemo-dr-0.99.2/src/omemo_dr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.070070 omemo-dr-0.99.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2023-05-06 21:18:55.000000 omemo-dr-0.99.2/tests/inmemoryidentitykeystore.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/tests/inmemoryprekeystore.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/tests/inmemorysessionstore.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/tests/inmemorysignedprekeystore.py
--rw-rw-rw-   0 root         (0) root         (0)     3512 2023-05-06 21:18:55.000000 omemo-dr-0.99.2/tests/inmemorystore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.070070 omemo-dr-0.99.2/tests/kdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/tests/kdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9676 2023-05-11 18:26:34.000000 omemo-dr-0.99.2/tests/kdf/test_hkdf.py
--rw-rw-rw-   0 root         (0) root         (0)    10416 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/tests/test_sessionbuilder.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2023-05-11 18:26:34.000000 omemo-dr-0.99.2/tests/test_sessioncipher.py
--rw-rw-rw-   0 root         (0) root         (0)     9315 2023-05-10 21:35:36.000000 omemo-dr-0.99.2/tests/test_sigs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 17:04:49.070070 omemo-dr-0.99.2/tests/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.2/tests/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-03 19:53:25.000000 omemo-dr-0.99.2/tests/util/test_byteutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/
+-rw-rw-rw-   0 root         (0) root         (0)    35122 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    43030 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2023-05-11 21:04:20.000000 omemo-dr-0.99.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.260476 omemo-dr-0.99.3/curve25519/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.260476 omemo-dr-0.99.3/curve25519/curve/
+-rw-rw-rw-   0 root         (0) root         (0)    31932 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/curve25519-donna.c
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/curve25519-donna.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.276477 omemo-dr-0.99.3/curve25519/curve/ed25519/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.280478 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/compare.c
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/compare.h
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/convert.c
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/crypto_additions.h
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/crypto_hash_sha512.h
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/curve_sigs.c
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/curve_sigs.h
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ed_sigs.c
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ed_sigs.h
+-rw-rw-rw-   0 root         (0) root         (0)     2236 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/elligator.c
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_edy_to_montx.c
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_isequal.c
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_isreduced.c
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_mont_rhs.c
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_montx_to_edy.c
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_sqrt.c
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_isneutral.c
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_montx_to_p3.c
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_neg.c
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_p3_to_montx.c
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_scalarmult.c
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_scalarmult_cofactor.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.284478 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_constants.h
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_crypto_additions.h
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_labelset.h
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_x.h
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/keygen.c
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/keygen.h
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/open_modified.c
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sc_clamp.c
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sc_cmov.c
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sc_neg.c
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sign_modified.c
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/utility.c
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/utility.h
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/xeddsa.c
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/xeddsa.h
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/zeroize.c
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/zeroize.h
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/api.h
+-rw-rw-rw-   0 root         (0) root         (0)    76457 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/base.h
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/base2.h
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/d.h
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/d2.h
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe.h
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_0.c
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_1.c
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_add.c
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_cmov.c
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_copy.c
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_frombytes.c
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_invert.c
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_isnegative.c
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_isnonzero.c
+-rw-rw-rw-   0 root         (0) root         (0)    10744 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_mul.c
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_neg.c
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_pow22523.c
+-rw-rw-rw-   0 root         (0) root         (0)     5980 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sq.c
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sq2.c
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sub.c
+-rw-rw-rw-   0 root         (0) root         (0)     3189 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_tobytes.c
+-rw-rw-rw-   0 root         (0) root         (0)     2869 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge.h
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_add.c
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_add.h
+-rw-rw-rw-   0 root         (0) root         (0)     2371 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_double_scalarmult.c
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_frombytes.c
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_madd.c
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_madd.h
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_msub.c
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_msub.h
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p1p1_to_p2.c
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p1p1_to_p3.c
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p2_0.c
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p2_dbl.c
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p2_dbl.h
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_0.c
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_dbl.c
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_to_cached.c
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_to_p2.c
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_tobytes.c
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_precomp_0.c
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_scalarmult_base.c
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_sub.c
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_sub.h
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_tobytes.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.284478 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_int32.h
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_int64.h
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_sign.h
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_uint32.h
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_uint64.h
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.284478 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/
+-rw-rw-rw-   0 root         (0) root         (0)     6416 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/blocks.c
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/hash.c
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/open.c
+-rw-rw-rw-   0 root         (0) root         (0)     5518 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/pow22523.h
+-rw-rw-rw-   0 root         (0) root         (0)     5527 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/pow225521.h
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sc.h
+-rw-rw-rw-   0 root         (0) root         (0)    12494 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sc_muladd.c
+-rw-rw-rw-   0 root         (0) root         (0)     8139 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sc_reduce.c
+-rw-rw-rw-   0 root         (0) root         (0)      817 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sign.c
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sqrtm1.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.284478 omemo-dr-0.99.3/curve25519/curve/ed25519/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/tests/internal_fast_tests.h
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/tests/internal_slow_tests.h
+-rw-rw-rw-   0 root         (0) root         (0)     8040 2023-04-09 19:22:07.000000 omemo-dr-0.99.3/curve25519/curve25519module.c
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2023-05-18 19:49:38.000000 omemo-dr-0.99.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.260476 omemo-dr-0.99.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.288478 omemo-dr-0.99.3/src/omemo_dr/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-22 23:23:19.000000 omemo-dr-0.99.3/src/omemo_dr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2254 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-20 17:36:45.000000 omemo-dr-0.99.3/src/omemo_dr/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.288478 omemo-dr-0.99.3/src/omemo_dr/curve/
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/curve/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.288478 omemo-dr-0.99.3/src/omemo_dr/ecc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/curve.py
+-rw-rw-rw-   0 root         (0) root         (0)     2713 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/djbec.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-08 20:42:25.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/ec.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/eckeypair.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-05-20 18:34:28.000000 omemo-dr-0.99.3/src/omemo_dr/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/identitykey.py
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/identitykeypair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.292479 omemo-dr-0.99.3/src/omemo_dr/kdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/derivedmessagesecrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/derivedrootsecrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/hkdf.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/messagekeys.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-07 15:19:42.000000 omemo-dr-0.99.3/src/omemo_dr/observable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.292479 omemo-dr-0.99.3/src/omemo_dr/protocol/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/ciphertextmessage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4076 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_keyexchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     5152 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5046 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/prekeywhispermessage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/whisper_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4943 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/whispermessage.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.292479 omemo-dr-0.99.3/src/omemo_dr/ratchet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/aliceparameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/bobparameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/chainkey.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/ratchetingsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-05-06 21:36:18.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/rootkey.py
+-rw-rw-rw-   0 root         (0) root         (0)    19094 2023-05-20 17:44:31.000000 omemo-dr-0.99.3/src/omemo_dr/session_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5487 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/sessionbuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10889 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/sessioncipher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.292479 omemo-dr-0.99.3/src/omemo_dr/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/state/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-05-20 18:34:28.000000 omemo-dr-0.99.3/src/omemo_dr/state/prekeybundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/prekeyrecord.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/sessionrecord.py
+-rw-rw-rw-   0 root         (0) root         (0)    12879 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/sessionstate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/signedprekeyrecord.py
+-rw-rw-rw-   0 root         (0) root         (0)     5950 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/storage_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4690 2023-05-20 17:44:31.000000 omemo-dr-0.99.3/src/omemo_dr/state/store.py
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/structs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/src/omemo_dr/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/util/byteutil.py
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-05-20 17:44:31.000000 omemo-dr-0.99.3/src/omemo_dr/util/keyhelper.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-07 18:48:15.000000 omemo-dr-0.99.3/src/omemo_dr/util/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.288478 omemo-dr-0.99.3/src/omemo_dr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43030 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6842 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2023-05-18 19:27:25.000000 omemo-dr-0.99.3/tests/inmemoryidentitykeystore.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/tests/inmemoryprekeystore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/tests/inmemorysessionstore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/tests/inmemorysignedprekeystore.py
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2023-05-06 21:18:55.000000 omemo-dr-0.99.3/tests/inmemorystore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/tests/kdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/tests/kdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/tests/kdf/test_hkdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    10416 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/tests/test_sessionbuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/tests/test_sessioncipher.py
+-rw-rw-rw-   0 root         (0) root         (0)     9315 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/tests/test_sigs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/tests/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/tests/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/tests/util/test_byteutil.py
```

### Comparing `omemo-dr-0.99.2/LICENSE` & `omemo-dr-0.99.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/PKG-INFO` & `omemo-dr-0.99.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omemo-dr
-Version: 0.99.2
+Version: 0.99.3
 Summary: OMEMO Double Ratchet
 Author: Philipp Hörist
 Author-email: philipp@hoerist.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `omemo-dr-0.99.2/README.md` & `omemo-dr-0.99.3/README.md`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/curve25519-donna.c` & `omemo-dr-0.99.3/curve25519/curve/curve25519-donna.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/compare.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/compare.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/convert.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/convert.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/crypto_additions.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/crypto_additions.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/curve_sigs.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/curve_sigs.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/curve_sigs.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/curve_sigs.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ed_sigs.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ed_sigs.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/elligator.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/elligator.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/fe_sqrt.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_sqrt.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ge_montx_to_p3.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_montx_to_p3.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/ge_scalarmult.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_scalarmult.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_labelset.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_labelset.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/generalized/gen_x.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_x.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/keygen.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/keygen.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/open_modified.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/open_modified.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/sc_neg.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sc_neg.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/sign_modified.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sign_modified.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/utility.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/utility.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/xeddsa.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/xeddsa.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/additions/xeddsa.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/xeddsa.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/base.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/base.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/base2.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/base2.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe_add.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_add.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe_cmov.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_cmov.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe_frombytes.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_frombytes.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe_mul.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_mul.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe_neg.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_neg.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe_sq.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sq.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe_sq2.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sq2.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe_sub.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sub.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/fe_tobytes.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_tobytes.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/ge.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/ge.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/ge_add.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_add.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/ge_double_scalarmult.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_double_scalarmult.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/ge_frombytes.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_frombytes.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/ge_madd.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_madd.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/ge_msub.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_msub.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/ge_p2_dbl.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p2_dbl.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/ge_scalarmult_base.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_scalarmult_base.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/ge_sub.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_sub.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_sign.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_sign.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_sha512/blocks.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/blocks.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/nacl_sha512/hash.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/hash.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/open.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/open.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/pow22523.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/pow22523.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/pow225521.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/pow225521.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/sc_muladd.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/sc_muladd.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/sc_reduce.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/sc_reduce.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/sign.c` & `omemo-dr-0.99.3/curve25519/curve/ed25519/sign.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/tests/internal_fast_tests.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/tests/internal_fast_tests.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve/ed25519/tests/internal_slow_tests.h` & `omemo-dr-0.99.3/curve25519/curve/ed25519/tests/internal_slow_tests.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/curve25519/curve25519module.c` & `omemo-dr-0.99.3/curve25519/curve25519module.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/pyproject.toml` & `omemo-dr-0.99.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -111,20 +111,23 @@
   "C416", # Unnecessary `list` comprehension (rewrite using `list()`)
   "E501", # Line too long (x > y characters)
   "N802", # Function name `loadSignedPreKeys` should be lowercase
   "N803", # Argument name `signedPreKeyId` should be lowercase
   "N806", # Variable `x` in function should be lowercase
   "N815", # Variable `messageKeys` in class scope should not be mixedCase
   "N818",   # Exception name should be named with an Error suffix
+  "PGH003",  # Use specific rule codes when ignoring type issues
   "PLR0913", # Too many arguments to function call (x/y)
   "PLR0915", # Too many statements (57/50)
   "PLR2004", # Magic value used in comparison, consider replacing x with a constant variable
   "RUF001", # AmbiguousUnicodeCharacterString
   "S101",   # Use of `assert` detected
   "S110", # `try`-`except`-`pass` detected, consider logging the exception
+  "S311", # Standard pseudo-random generators are not suitable for cryptographic purposes
+  "S603", # check for execution of untrusted input
   "SIM108", # Use ternary operator
   "SIM110", # Use any()` instead of `for` loop
   "SIM118", # Don’t use .keys()
   "UP004", # Class inherits from `object`
   "UP007",  # Use X | Y for type annotations
   "UP008", # Use `super()` instead of `super(__class__, self)`
   "UP031", # Use format specifiers instead of percent format
```

### Comparing `omemo-dr-0.99.2/setup.py` & `omemo-dr-0.99.3/setup.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/aes.py` & `omemo-dr-0.99.3/src/omemo_dr/aes.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/curve/__init__.py` & `omemo-dr-0.99.3/src/omemo_dr/curve/__init__.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/ecc/curve.py` & `omemo-dr-0.99.3/src/omemo_dr/ecc/curve.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/ecc/djbec.py` & `omemo-dr-0.99.3/src/omemo_dr/ecc/djbec.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/exceptions.py` & `omemo-dr-0.99.3/src/omemo_dr/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,7 +69,11 @@
 
 class InvalidMessage(Exception):
     pass
 
 
 class DuplicateMessage(Exception):
     pass
+
+
+class BundleValidationError(Exception):
+    pass
```

### Comparing `omemo-dr-0.99.2/src/omemo_dr/identitykey.py` & `omemo-dr-0.99.3/src/omemo_dr/identitykey.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/identitykeypair.py` & `omemo-dr-0.99.3/src/omemo_dr/identitykeypair.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/kdf/derivedmessagesecrets.py` & `omemo-dr-0.99.3/src/omemo_dr/kdf/derivedmessagesecrets.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/kdf/hkdf.py` & `omemo-dr-0.99.3/src/omemo_dr/kdf/hkdf.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/observable.py` & `omemo-dr-0.99.3/src/omemo_dr/observable.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/protocol/omemo_keyexchange.py` & `omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_keyexchange.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/protocol/omemo_message.py` & `omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_message.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/protocol/omemo_pb2.py` & `omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_pb2.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/protocol/prekeywhispermessage.py` & `omemo-dr-0.99.3/src/omemo_dr/protocol/prekeywhispermessage.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/protocol/whisper_pb2.py` & `omemo-dr-0.99.3/src/omemo_dr/protocol/whisper_pb2.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/protocol/whispermessage.py` & `omemo-dr-0.99.3/src/omemo_dr/protocol/whispermessage.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/ratchet/aliceparameters.py` & `omemo-dr-0.99.3/src/omemo_dr/ratchet/aliceparameters.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/ratchet/bobparameters.py` & `omemo-dr-0.99.3/src/omemo_dr/ratchet/bobparameters.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/ratchet/chainkey.py` & `omemo-dr-0.99.3/src/omemo_dr/ratchet/chainkey.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/ratchet/ratchetingsession.py` & `omemo-dr-0.99.3/src/omemo_dr/ratchet/ratchetingsession.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/ratchet/rootkey.py` & `omemo-dr-0.99.3/src/omemo_dr/ratchet/rootkey.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/session_manager.py` & `omemo-dr-0.99.3/src/omemo_dr/session_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,19 +67,19 @@
 
         for address, device in self._storage.get_active_device_tuples():
             self._log.info("Load device from storage: %s - %s", address, device)
             self.add_device(address, device)
 
     def _generate_keys(self) -> int:
         identity_key_pair = KeyHelper.generate_identity_key_pair()
-        our_device_id = KeyHelper.get_random_sequence(2147483647)
+        our_device_id = KeyHelper.get_random_int()
         self._storage.set_our_identity(our_device_id, identity_key_pair)
 
         signed_pre_key = KeyHelper.generate_signed_pre_key(
-            identity_key_pair, KeyHelper.get_random_sequence(65536)
+            identity_key_pair, KeyHelper.get_random_int()
         )
         self._storage.store_signed_pre_key(signed_pre_key.get_id(), signed_pre_key)
 
         self._generate_pre_keys(self._config.default_prekey_amount)
 
         return our_device_id
 
@@ -376,21 +376,20 @@
     def _cycle_signed_pre_key(self, ik_pair: IdentityKeyPair) -> None:
         # Publish every spk_cycle_seconds a new SignedPreKey
         # Delete all existing SignedPreKeys that are older
         # then spk_archive_seconds
 
         # if spk_cycle_seconds is reached, generate a new SignedPreKey
         now = int(time.time())
-        timestamp = self._storage.get_signed_pre_key_timestamp(
-            self._storage.get_current_signed_pre_key_id()
-        )
+        current_spk_id = self._storage.get_current_signed_pre_key_id()
+        timestamp = self._storage.get_signed_pre_key_timestamp(current_spk_id)
 
         if int(timestamp) < now - self._config.spk_cycle_seconds:
             spk = KeyHelper.generate_signed_pre_key(
-                ik_pair, self._storage.get_next_signed_pre_key_id()
+                ik_pair, KeyHelper.get_next_signed_pre_key_id(current_spk_id)
             )
             self._storage.store_signed_pre_key(spk.get_id(), spk)
             self._log.debug("Cycled SignedPreKey")
 
         # Delete all SignedPreKeys that are older than spk_archive_seconds
         timestamp = now - self._config.spk_archive_seconds
         self._storage.remove_old_signed_pre_keys(timestamp)
```

### Comparing `omemo-dr-0.99.2/src/omemo_dr/sessionbuilder.py` & `omemo-dr-0.99.3/src/omemo_dr/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/sessioncipher.py` & `omemo-dr-0.99.3/src/omemo_dr/sessioncipher.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/state/prekeybundle.py` & `omemo-dr-0.99.3/src/omemo_dr/state/prekeybundle.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+from ..const import MAX_INT
 from ..const import NS_OMEMO_2
 from ..const import NS_OMEMO_TMP
 from ..ecc.djbec import CurvePublicKey
 from ..ecc.djbec import EdPublicKey
-from ..exceptions import InvalidKeyException
+from ..exceptions import BundleValidationError
 from ..identitykey import IdentityKey
 from ..structs import OMEMOBundleProto
 
 
 class PreKeyBundle:
     def __init__(
         self,
@@ -38,18 +39,27 @@
 
         ns = bundle.namespace
         if ns == NS_OMEMO_TMP:
             ik_pub = CurvePublicKey.from_bytes(bundle.ik)
         elif ns == NS_OMEMO_2:
             ik_pub = EdPublicKey.from_bytes(bundle.ik).to_curve()
         else:
-            raise InvalidKeyException("Unknown namespace on bundle: %s", ns)
+            raise BundleValidationError("Unknown namespace on bundle: %s", ns)
 
         ik = IdentityKey(ik_pub)
 
+        if not 1 <= bundle.device_id <= MAX_INT:
+            raise BundleValidationError("Device id out of range")
+
+        if not 1 <= prekey["id"] <= MAX_INT:
+            raise BundleValidationError("Prekey id out of range")
+
+        if not 1 <= bundle.spk["id"] <= MAX_INT:
+            raise BundleValidationError("Signed pre key id out of range")
+
         return cls(
             bundle.device_id,
             bundle.namespace,
             prekey["id"],
             otpk,
             bundle.spk["id"],
             spk,
```

### Comparing `omemo-dr-0.99.2/src/omemo_dr/state/prekeyrecord.py` & `omemo-dr-0.99.3/src/omemo_dr/state/prekeyrecord.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/state/sessionrecord.py` & `omemo-dr-0.99.3/src/omemo_dr/state/sessionrecord.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/state/sessionstate.py` & `omemo-dr-0.99.3/src/omemo_dr/state/sessionstate.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/state/signedprekeyrecord.py` & `omemo-dr-0.99.3/src/omemo_dr/state/signedprekeyrecord.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/state/storage_pb2.py` & `omemo-dr-0.99.3/src/omemo_dr/state/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/state/store.py` & `omemo-dr-0.99.3/src/omemo_dr/state/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,18 +113,14 @@
         pass
 
     @abc.abstractmethod
     def get_current_signed_pre_key_id(self) -> int:
         pass
 
     @abc.abstractmethod
-    def get_next_signed_pre_key_id(self) -> int:
-        pass
-
-    @abc.abstractmethod
     def get_signed_pre_key_timestamp(self, signed_pre_key_id: int) -> int:
         pass
 
     @abc.abstractmethod
     def remove_old_signed_pre_keys(self, timestamp: int) -> None:
         pass
```

### Comparing `omemo-dr-0.99.2/src/omemo_dr/structs.py` & `omemo-dr-0.99.3/src/omemo_dr/structs.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/util/byteutil.py` & `omemo-dr-0.99.3/src/omemo_dr/util/byteutil.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/src/omemo_dr/util/keyhelper.py` & `omemo-dr-0.99.3/src/omemo_dr/util/keyhelper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
-import binascii
-import math
-import os
+import random
 import time
 
+from ..const import MAX_INT
 from ..ecc.curve import Curve
 from ..identitykey import IdentityKey
 from ..identitykeypair import IdentityKeyPair
 from ..state.prekeyrecord import PreKeyRecord
 from ..state.signedprekeyrecord import SignedPreKeyRecord
-from .medium import Medium
 
 
 class KeyHelper:
     @staticmethod
     def generate_identity_key_pair() -> IdentityKeyPair:
         """
         Generate an identity key pair. Clients should only do this once,
@@ -23,43 +21,31 @@
         """
         key_pair = Curve.generate_key_pair()
         public_key = IdentityKey(key_pair.get_public_key())
         identity_key_pair = IdentityKeyPair.new(public_key, key_pair.get_private_key())
         return identity_key_pair
 
     @staticmethod
-    def generate_device_id() -> int:
-        """
-        Generate a registration ID.  Clients should only do this once,
-        at install time.
-        """
-        regId = KeyHelper.get_random_sequence()
-        return regId
-
-    @staticmethod
-    def get_random_sequence(max: int = 4294967296) -> int:
-        size = int(math.log(max) / math.log(2)) / 8
-        rand = os.urandom(int(size))
-        randh = binascii.hexlify(rand)
-        return int(randh, 16)
+    def get_random_int() -> int:
+        return random.randint(1, MAX_INT)
 
     @staticmethod
     def generate_pre_keys(start: int, count: int) -> list[PreKeyRecord]:
         """
         Generate a list of PreKeys.  Clients should do this at install time, and
         subsequently any time the list of PreKeys stored on the server runs low.
 
         PreKey IDs are shorts, so they will eventually be repeated.
         Clients should store PreKeys in a circular buffer, so that they are
         repeated as infrequently as possible.
         """
         results: list[PreKeyRecord] = []
         start -= 1
         for i in range(0, count):
-            pre_key_id = ((start + i) % (Medium.MAX_VALUE - 1)) + 1
+            pre_key_id = ((start + i) % MAX_INT) + 1
             results.append(PreKeyRecord.new(pre_key_id, Curve.generate_key_pair()))
 
         return results
 
     @staticmethod
     def generate_signed_pre_key(
         identity_key_pair: IdentityKeyPair, signed_pre_key_id: int
@@ -70,7 +56,11 @@
         )
 
         spk = SignedPreKeyRecord.new(
             signed_pre_key_id, int(round(time.time() * 1000)), key_pair, signature
         )
 
         return spk
+
+    @staticmethod
+    def get_next_signed_pre_key_id(current_id: int) -> int:
+        return current_id % MAX_INT + 1
```

### Comparing `omemo-dr-0.99.2/src/omemo_dr.egg-info/PKG-INFO` & `omemo-dr-0.99.3/src/omemo_dr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omemo-dr
-Version: 0.99.2
+Version: 0.99.3
 Summary: OMEMO Double Ratchet
 Author: Philipp Hörist
 Author-email: philipp@hoerist.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `omemo-dr-0.99.2/src/omemo_dr.egg-info/SOURCES.txt` & `omemo-dr-0.99.3/src/omemo_dr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,14 @@
 src/omemo_dr/state/signedprekeyrecord.py
 src/omemo_dr/state/storage_pb2.py
 src/omemo_dr/state/store.py
 src/omemo_dr/util/__init__.py
 src/omemo_dr/util/byteutil.py
 src/omemo_dr/util/keyhelper.py
 src/omemo_dr/util/logging.py
-src/omemo_dr/util/medium.py
 tests/__init__.py
 tests/inmemoryidentitykeystore.py
 tests/inmemoryprekeystore.py
 tests/inmemorysessionstore.py
 tests/inmemorysignedprekeystore.py
 tests/inmemorystore.py
 tests/test_sessionbuilder.py
```

### Comparing `omemo-dr-0.99.2/tests/inmemoryidentitykeystore.py` & `omemo-dr-0.99.3/tests/inmemoryidentitykeystore.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self) -> None:
         self.trusted_keys: dict[str, IdentityKey] = {}
         identity_key_pair_keys = Curve.generate_key_pair()
         self.identity_key_pair = IdentityKeyPair.new(
             IdentityKey(identity_key_pair_keys.get_public_key()),
             identity_key_pair_keys.get_private_key(),
         )
-        self.our_device_id = KeyHelper.generate_device_id()
+        self.our_device_id = KeyHelper.get_random_int()
 
     def get_identity_key_pair(self) -> IdentityKeyPair:
         return self.identity_key_pair
 
     def get_our_device_id(self) -> int:
         return self.our_device_id
```

### Comparing `omemo-dr-0.99.2/tests/inmemoryprekeystore.py` & `omemo-dr-0.99.3/tests/inmemoryprekeystore.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/tests/inmemorysessionstore.py` & `omemo-dr-0.99.3/tests/inmemorysessionstore.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/tests/inmemorysignedprekeystore.py` & `omemo-dr-0.99.3/tests/inmemorysignedprekeystore.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/tests/inmemorystore.py` & `omemo-dr-0.99.3/tests/inmemorystore.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/tests/kdf/test_hkdf.py` & `omemo-dr-0.99.3/tests/kdf/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/tests/test_sessionbuilder.py` & `omemo-dr-0.99.3/tests/test_sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/tests/test_sessioncipher.py` & `omemo-dr-0.99.3/tests/test_sessioncipher.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.2/tests/test_sigs.py` & `omemo-dr-0.99.3/tests/test_sigs.py`

 * *Files identical despite different names*

