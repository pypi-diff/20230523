# Comparing `tmp/circuitgraph-0.2.0.tar.gz` & `tmp/circuitgraph-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitgraph-0.2.0.tar", last modified: Sat Apr 23 00:48:12 2022, max compression
+gzip compressed data, was "circuitgraph-0.2.1.tar", last modified: Tue May 23 21:11:16 2023, max compression
```

## Comparing `circuitgraph-0.2.0.tar` & `circuitgraph-0.2.1.tar`

### file list

```diff
@@ -1,116 +1,118 @@
-drwxr-xr-x   0 rubenpurdy   (501) staff       (20)        0 2022-04-23 00:48:12.855887 circuitgraph-0.2.0/
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     1068 2020-07-18 23:56:21.000000 circuitgraph-0.2.0/LICENSE
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      176 2022-01-03 22:51:58.000000 circuitgraph-0.2.0/MANIFEST.in
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     5114 2022-04-23 00:48:12.855750 circuitgraph-0.2.0/PKG-INFO
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     4442 2022-04-23 00:48:02.000000 circuitgraph-0.2.0/README.md
-drwxr-xr-x   0 rubenpurdy   (501) staff       (20)        0 2022-04-23 00:48:12.821660 circuitgraph-0.2.0/circuitgraph/
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      897 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/__init__.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    34709 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/circuit.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    12089 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/io.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     4815 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/logic.py
-drwxr-xr-x   0 rubenpurdy   (501) staff       (20)        0 2022-04-23 00:48:12.851523 circuitgraph-0.2.0/circuitgraph/netlists/
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    94820 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/adder.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   984420 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/arbiter.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    80430 2022-01-03 22:51:58.000000 circuitgraph-0.2.0/circuitgraph/netlists/b17_C.bench
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  1628354 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/b17_Cg.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  3861844 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/b18_Cg.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  8691867 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/b19_Cg.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    80368 2022-01-03 22:51:58.000000 circuitgraph-0.2.0/circuitgraph/netlists/b20_C.bench
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   560245 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/b20_Cg.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   130719 2022-01-03 22:51:58.000000 circuitgraph-0.2.0/circuitgraph/netlists/b22_C.bench
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   856502 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/b22_Cg.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   668180 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/banyan_128.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    39301 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/banyan_16.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  1615295 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/banyan_256.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   106925 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/banyan_32.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   273913 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/banyan_64.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    12498 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/banyan_8.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   139422 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/bar.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    23905 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c1355.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    24949 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c1355g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      528 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c17.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      412 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c17_assign.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      279 2022-01-03 22:51:59.000000 circuitgraph-0.2.0/circuitgraph/netlists/c17_gates.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      541 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c17g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    23072 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c1908.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    23600 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c1908g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    42020 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c2670.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    41968 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c2670g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    48577 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c3540.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    56515 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c3540g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     7958 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c432.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     8499 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c432g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     8555 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c499.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    25550 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c499g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    80744 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c5315.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    88196 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c5315g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   109221 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c6288.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   151400 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c6288g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   117054 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c7552.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    97420 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c7552g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    15128 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c880.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    20247 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/c880g.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    48921 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/cavlc.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    12692 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/ctrl.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    26839 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/dec.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  4616674 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/div.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    85410 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/i2c.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    15347 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/int2float.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  2130192 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/log2.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   237622 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/max.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  3748449 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/memctrl.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  1940713 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/multiplier.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      263 2022-01-03 22:51:59.000000 circuitgraph-0.2.0/circuitgraph/netlists/mux_2.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      580 2022-01-03 22:51:59.000000 circuitgraph-0.2.0/circuitgraph/netlists/mux_4.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    72752 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/priority_ckt.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    19828 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/router.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    87526 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/s13207.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     1045 2022-01-18 17:37:09.000000 circuitgraph-0.2.0/circuitgraph/netlists/s27.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    14179 2022-01-03 22:51:59.000000 circuitgraph-0.2.0/circuitgraph/netlists/s27_unrolled_4.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   319256 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/sin.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  1690730 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/sqrt.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  1544659 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/square.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      388 2022-01-03 22:51:59.000000 circuitgraph-0.2.0/circuitgraph/netlists/switch.v
--rw-r--r--   0 rubenpurdy   (501) staff       (20)  1160385 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/netlists/voter.v
-drwxr-xr-x   0 rubenpurdy   (501) staff       (20)        0 2022-04-23 00:48:12.852730 circuitgraph-0.2.0/circuitgraph/parsing/
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      235 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/parsing/__init__.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     5778 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/parsing/fast_verilog.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     2466 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/parsing/verilog.lark
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    12124 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/parsing/verilog.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     7663 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/props.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    12822 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/sat.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    34952 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/tx.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     7231 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/circuitgraph/utils.py
-drwxr-xr-x   0 rubenpurdy   (501) staff       (20)        0 2022-04-23 00:48:12.822367 circuitgraph-0.2.0/circuitgraph.egg-info/
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     5114 2022-04-23 00:48:12.000000 circuitgraph-0.2.0/circuitgraph.egg-info/PKG-INFO
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     2887 2022-04-23 00:48:12.000000 circuitgraph-0.2.0/circuitgraph.egg-info/SOURCES.txt
--rw-r--r--   0 rubenpurdy   (501) staff       (20)        1 2022-04-23 00:48:12.000000 circuitgraph-0.2.0/circuitgraph.egg-info/dependency_links.txt
--rw-r--r--   0 rubenpurdy   (501) staff       (20)       14 2022-04-23 00:48:12.000000 circuitgraph-0.2.0/circuitgraph.egg-info/requires.txt
--rw-r--r--   0 rubenpurdy   (501) staff       (20)       13 2022-04-23 00:48:12.000000 circuitgraph-0.2.0/circuitgraph.egg-info/top_level.txt
-drwxr-xr-x   0 rubenpurdy   (501) staff       (20)        0 2022-04-23 00:48:12.854698 circuitgraph-0.2.0/docs/
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    18076 2022-04-23 00:13:54.000000 circuitgraph-0.2.0/docs/analysis.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   149007 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/circuit.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    99015 2020-07-18 23:56:21.000000 circuitgraph-0.2.0/docs/circuitgraph.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    14961 2020-07-18 23:56:21.000000 circuitgraph-0.2.0/docs/circuitgraph.png
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    10497 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/index.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    41653 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/io.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    52431 2020-08-07 19:38:59.000000 circuitgraph-0.2.0/docs/locks.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    22973 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/logic.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      987 2022-01-03 22:52:00.000000 circuitgraph-0.2.0/docs/paper.bib
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     5290 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/paper.md
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    29504 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/props.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    41591 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/sat.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    75315 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/transform.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)   102020 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/tx.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    27960 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/docs/utils.html
--rw-r--r--   0 rubenpurdy   (501) staff       (20)       38 2022-04-23 00:48:12.855936 circuitgraph-0.2.0/setup.cfg
--rw-r--r--   0 rubenpurdy   (501) staff       (20)      961 2022-04-23 00:47:52.000000 circuitgraph-0.2.0/setup.py
-drwxr-xr-x   0 rubenpurdy   (501) staff       (20)        0 2022-04-23 00:48:12.855569 circuitgraph-0.2.0/tests/
--rw-r--r--   0 rubenpurdy   (501) staff       (20)        0 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/tests/__init__.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    18614 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/tests/test_circuit.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     8326 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/tests/test_io.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     3431 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/tests/test_logic.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     4608 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/tests/test_props.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     5872 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/tests/test_sat.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)    19247 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/tests/test_tx.py
--rw-r--r--   0 rubenpurdy   (501) staff       (20)     1559 2022-04-23 00:32:30.000000 circuitgraph-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 rpurdy   (2663604) users      (100)        0 2023-05-23 21:11:16.714817 circuitgraph-0.2.1/
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     1068 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/LICENSE
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      176 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/MANIFEST.in
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     5077 2023-05-23 21:11:16.712817 circuitgraph-0.2.1/PKG-INFO
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     4442 2023-05-23 20:39:49.000000 circuitgraph-0.2.1/README.md
+drwxr-xr-x   0 rpurdy   (2663604) users      (100)        0 2023-05-23 21:11:14.132765 circuitgraph-0.2.1/circuitgraph/
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      940 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/circuitgraph/__init__.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    34718 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/circuitgraph/circuit.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    12211 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/circuitgraph/io.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     4815 2023-03-29 13:35:20.000000 circuitgraph-0.2.1/circuitgraph/logic.py
+drwxr-xr-x   0 rpurdy   (2663604) users      (100)        0 2023-05-23 21:11:16.431812 circuitgraph-0.2.1/circuitgraph/netlists/
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    94820 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/adder.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   984420 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/arbiter.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    80430 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/b17_C.bench
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  1628354 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/b17_Cg.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  3861844 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/b18_Cg.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  8691867 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/b19_Cg.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    80368 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/b20_C.bench
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   560245 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/b20_Cg.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   130719 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/b22_C.bench
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   856502 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/b22_Cg.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   668180 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/banyan_128.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    39301 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/banyan_16.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  1615295 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/banyan_256.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   106925 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/banyan_32.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   273913 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/banyan_64.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    12498 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/banyan_8.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   139422 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/bar.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    23905 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c1355.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    24949 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c1355g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      528 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c17.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      412 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c17_assign.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      279 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c17_gates.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      541 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c17g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    23072 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c1908.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    23600 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c1908g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    42020 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c2670.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    41968 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c2670g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    48577 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c3540.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    56515 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c3540g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     7958 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c432.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     8499 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c432g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     8555 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c499.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    25550 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c499g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    80744 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c5315.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    88196 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c5315g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   109221 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c6288.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   151400 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c6288g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   117054 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c7552.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    97420 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c7552g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    15128 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c880.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    20247 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/c880g.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    48921 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/cavlc.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    12692 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/ctrl.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    26839 2022-05-01 23:56:06.000000 circuitgraph-0.2.1/circuitgraph/netlists/dec.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  4616674 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/div.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    85410 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/i2c.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    15347 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/int2float.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  2130192 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/log2.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   237622 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/max.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  3748449 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/memctrl.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  1940713 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/multiplier.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      263 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/mux_2.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      580 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/mux_4.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    72752 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/priority_ckt.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    19828 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/router.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    58858 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/circuitgraph/netlists/s13207.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     1045 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/s27.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    14179 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/s27_unrolled_4.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   592826 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/circuitgraph/netlists/s38417.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   531993 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/circuitgraph/netlists/s38584.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   319256 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/sin.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  1690730 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/sqrt.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  1544659 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/square.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      388 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/switch.v
+-rw-r--r--   0 rpurdy   (2663604) users      (100)  1160385 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/netlists/voter.v
+drwxr-xr-x   0 rpurdy   (2663604) users      (100)        0 2023-05-23 21:11:16.491813 circuitgraph-0.2.1/circuitgraph/parsing/
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      235 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/parsing/__init__.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     5778 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/parsing/fast_verilog.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     2466 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/circuitgraph/parsing/verilog.lark
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    12654 2023-03-13 17:20:47.000000 circuitgraph-0.2.1/circuitgraph/parsing/verilog.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     8408 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/circuitgraph/props.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    13286 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/circuitgraph/sat.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    38608 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/circuitgraph/tx.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     7240 2023-04-26 13:45:38.000000 circuitgraph-0.2.1/circuitgraph/utils.py
+drwxr-xr-x   0 rpurdy   (2663604) users      (100)        0 2023-05-23 21:11:14.137765 circuitgraph-0.2.1/circuitgraph.egg-info/
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     5077 2023-05-23 21:11:13.000000 circuitgraph-0.2.1/circuitgraph.egg-info/PKG-INFO
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     2949 2023-05-23 21:11:14.000000 circuitgraph-0.2.1/circuitgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 rpurdy   (2663604) users      (100)        1 2023-05-23 21:11:13.000000 circuitgraph-0.2.1/circuitgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 rpurdy   (2663604) users      (100)       14 2023-05-23 21:11:13.000000 circuitgraph-0.2.1/circuitgraph.egg-info/requires.txt
+-rw-r--r--   0 rpurdy   (2663604) users      (100)       13 2023-05-23 21:11:13.000000 circuitgraph-0.2.1/circuitgraph.egg-info/top_level.txt
+drwxr-xr-x   0 rpurdy   (2663604) users      (100)        0 2023-05-23 21:11:16.699817 circuitgraph-0.2.1/docs/
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    18076 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/docs/analysis.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   149044 2023-05-23 21:04:34.000000 circuitgraph-0.2.1/docs/circuit.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    99015 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/docs/circuitgraph.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    14961 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/docs/circuitgraph.png
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    10541 2023-05-23 21:04:34.000000 circuitgraph-0.2.1/docs/index.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    41878 2023-05-23 21:04:34.000000 circuitgraph-0.2.1/docs/io.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    52431 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/docs/locks.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    22973 2023-05-23 21:04:21.000000 circuitgraph-0.2.1/docs/logic.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      987 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/docs/paper.bib
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     5290 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/docs/paper.md
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    31885 2023-05-23 21:04:34.000000 circuitgraph-0.2.1/docs/props.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    42908 2023-05-23 21:04:34.000000 circuitgraph-0.2.1/docs/sat.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    75315 2022-05-01 23:56:07.000000 circuitgraph-0.2.1/docs/transform.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)   113392 2023-05-23 21:04:34.000000 circuitgraph-0.2.1/docs/tx.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    27979 2023-05-23 21:04:34.000000 circuitgraph-0.2.1/docs/utils.html
+-rw-r--r--   0 rpurdy   (2663604) users      (100)       38 2023-05-23 21:11:16.715818 circuitgraph-0.2.1/setup.cfg
+-rw-r--r--   0 rpurdy   (2663604) users      (100)      983 2023-05-23 20:56:08.000000 circuitgraph-0.2.1/setup.py
+drwxr-xr-x   0 rpurdy   (2663604) users      (100)        0 2023-05-23 21:11:16.710817 circuitgraph-0.2.1/tests/
+-rw-r--r--   0 rpurdy   (2663604) users      (100)        0 2022-10-12 14:28:44.000000 circuitgraph-0.2.1/tests/__init__.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    18614 2023-02-01 14:45:50.000000 circuitgraph-0.2.1/tests/test_circuit.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     7068 2023-03-13 17:20:47.000000 circuitgraph-0.2.1/tests/test_io.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     3431 2022-10-13 14:51:22.000000 circuitgraph-0.2.1/tests/test_logic.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     5055 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/tests/test_props.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     5872 2022-10-13 14:51:23.000000 circuitgraph-0.2.1/tests/test_sat.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)    20739 2023-03-13 17:20:55.000000 circuitgraph-0.2.1/tests/test_tx.py
+-rw-r--r--   0 rpurdy   (2663604) users      (100)     1559 2022-10-13 14:51:23.000000 circuitgraph-0.2.1/tests/test_utils.py
```

### Comparing `circuitgraph-0.2.0/LICENSE` & `circuitgraph-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/PKG-INFO` & `circuitgraph-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: circuitgraph
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tools for working with boolean circuits as graphs.
 Home-page: https://github.com/circuitgraph/circuitgraph
 Author: Ruben Purdy, Joseph Sweeney
 Author-email: rpurdy@andrew.cmu.edu, joesweeney@cmu.edu
-License: UNKNOWN
 Project-URL: Documentation, https://circuitgraph.github.io/circuitgraph/
 Project-URL: Source, https://github.com/circuitgraph/circuitgraph
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -42,15 +40,15 @@
 cg.to_file(c, '/path/to/output/circuit.v')
 ```
 
 The documentation can be found [here](https://circuitgraph.github.io/circuitgraph/).
 
 ## Installation
 
-CircuitGraph requires Python3.6 or greater
+CircuitGraph requires Python3.7 or greater
 The easiest way to install is via PyPi:
 ```shell
 pip install circuitgraph
 ```
 To install from the release, download and:
 ```shell
 pip install circuitgraph-<release>.tar.gz
@@ -121,9 +119,7 @@
   year={2020}
 }
 ```
 
 ## Acknowledgements
 
 Circuitgraph icon designed by [ncasti](https://github.com/ncasti).
-
-
```

### Comparing `circuitgraph-0.2.0/README.md` & `circuitgraph-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 cg.to_file(c, '/path/to/output/circuit.v')
 ```
 
 The documentation can be found [here](https://circuitgraph.github.io/circuitgraph/).
 
 ## Installation
 
-CircuitGraph requires Python3.6 or greater
+CircuitGraph requires Python3.7 or greater
 The easiest way to install is via PyPi:
 ```shell
 pip install circuitgraph
 ```
 To install from the release, download and:
 ```shell
 pip install circuitgraph-<release>.tar.gz
```

### Comparing `circuitgraph-0.2.0/circuitgraph/__init__.py` & `circuitgraph-0.2.1/circuitgraph/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,10 +19,17 @@
 from circuitgraph.circuit import (
     BlackBox,
     Circuit,
     primitive_gates,
     addable_types,
     supported_types,
 )
-from circuitgraph.io import dc_flops, from_file, from_lib, genus_flops, to_file
+from circuitgraph.io import (
+    generic_flop,
+    dc_flops,
+    from_file,
+    from_lib,
+    genus_flops,
+    to_file,
+)
 from circuitgraph.utils import lint, visualize
 from circuitgraph import logic, props, sat, tx, utils
```

### Comparing `circuitgraph-0.2.0/circuitgraph/circuit.py` & `circuitgraph-0.2.1/circuitgraph/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         """
         return Circuit(
             graph=self.graph.copy(), name=self.name, blackboxes=self.blackboxes.copy()
         )
 
     def set_type(self, ns, t):
         """
-        Return node(s) type(s).
+        Set the type of a node or nodes.
 
         Parameters
         ----------
         ns : str or iterable of str
                 Node.
         t : str
                 Type.
```

### Comparing `circuitgraph-0.2.0/circuitgraph/io.py` & `circuitgraph-0.2.1/circuitgraph/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Functions for reading/writing CircuitGraphs."""
 import re
 from pathlib import Path
 
 from circuitgraph import BlackBox, Circuit
 from circuitgraph.parsing import fast_parse_verilog_netlist, parse_verilog_netlist
 
+generic_flop = BlackBox("ff", ["clk", "d"], ["q"])
+
 genus_flops = [
     BlackBox("flopd", ["CK", "D"], ["Q"]),
     BlackBox("fflopd", ["CK", "D"], ["Q"]),
     BlackBox("flopdrs", ["CK", "D", "R", "S"], ["Q"]),
     BlackBox("fflopdrs", ["CK", "D", "R", "S"], ["Q"]),
 ]
 
@@ -94,15 +96,15 @@
 
     Returns
     -------
     Circuit
             the parsed circuit.
 
     """
-    bbs = [BlackBox("ff", ["CK", "D"], ["Q"])]
+    bbs = [BlackBox("ff", ["CK", "D"], ["Q"])] + genus_flops + dc_flops
     [path] = Path(__file__).parent.absolute().glob(f"netlists/{name}.*")
     return from_file(path, name, blackboxes=bbs)
 
 
 def bench_to_circuit(netlist, name):
     """
     Create a new Circuit from a netlist string.
@@ -331,15 +333,16 @@
                     fanin = f" {symbol} ".join(fanin)
                     if c.type(n) in ["xnor", "nor", "nand"]:
                         insts.append(f"assign {n} = ~({fanin})")
                     else:
                         insts.append(f"assign {n} = {fanin}")
             else:
                 fanin = ", ".join(fanin)
-                insts.append(f"{c.type(n)} g_{len(insts)} " f"({n}, {fanin})")
+                gate_name = c.uid(f"g_{len(insts)}")
+                insts.append(f"{c.type(n)} {gate_name}({n}, {fanin})")
         elif c.type(n) in ["0", "1", "x"]:
             insts.append(f"assign {n} = 1'b{c.type(n)}")
             wires.append(n)
         elif c.type(n) in ["input", "bb_input", "bb_output"]:
             pass
         else:
             raise ValueError(f"unknown gate type: {c.type(n)}")
```

### Comparing `circuitgraph-0.2.0/circuitgraph/logic.py` & `circuitgraph-0.2.1/circuitgraph/logic.py`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/adder.v` & `circuitgraph-0.2.1/circuitgraph/netlists/adder.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/arbiter.v` & `circuitgraph-0.2.1/circuitgraph/netlists/arbiter.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/b17_C.bench` & `circuitgraph-0.2.1/circuitgraph/netlists/b17_C.bench`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/b17_Cg.v` & `circuitgraph-0.2.1/circuitgraph/netlists/b17_Cg.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/b18_Cg.v` & `circuitgraph-0.2.1/circuitgraph/netlists/b18_Cg.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/b19_Cg.v` & `circuitgraph-0.2.1/circuitgraph/netlists/b19_Cg.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/b20_C.bench` & `circuitgraph-0.2.1/circuitgraph/netlists/b20_C.bench`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/b20_Cg.v` & `circuitgraph-0.2.1/circuitgraph/netlists/b20_Cg.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/b22_C.bench` & `circuitgraph-0.2.1/circuitgraph/netlists/b22_C.bench`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/b22_Cg.v` & `circuitgraph-0.2.1/circuitgraph/netlists/b22_Cg.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/banyan_128.v` & `circuitgraph-0.2.1/circuitgraph/netlists/banyan_128.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/banyan_16.v` & `circuitgraph-0.2.1/circuitgraph/netlists/banyan_16.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/banyan_256.v` & `circuitgraph-0.2.1/circuitgraph/netlists/banyan_256.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/banyan_32.v` & `circuitgraph-0.2.1/circuitgraph/netlists/banyan_32.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/banyan_64.v` & `circuitgraph-0.2.1/circuitgraph/netlists/banyan_64.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/banyan_8.v` & `circuitgraph-0.2.1/circuitgraph/netlists/banyan_8.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/bar.v` & `circuitgraph-0.2.1/circuitgraph/netlists/bar.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c1355.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c1355.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c1355g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c1355g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c17.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c17.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c17g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c17g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c1908.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c1908.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c1908g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c1908g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c2670.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c2670.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c2670g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c2670g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c3540.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c3540.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c3540g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c3540g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c432.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c432.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c432g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c432g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c499.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c499.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c499g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c499g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c5315.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c5315.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c5315g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c5315g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c6288.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c6288.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c6288g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c6288g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c7552.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c7552.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c7552g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c7552g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c880.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c880.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/c880g.v` & `circuitgraph-0.2.1/circuitgraph/netlists/c880g.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/cavlc.v` & `circuitgraph-0.2.1/circuitgraph/netlists/cavlc.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/ctrl.v` & `circuitgraph-0.2.1/circuitgraph/netlists/ctrl.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/dec.v` & `circuitgraph-0.2.1/circuitgraph/netlists/dec.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/div.v` & `circuitgraph-0.2.1/circuitgraph/netlists/div.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/i2c.v` & `circuitgraph-0.2.1/circuitgraph/netlists/i2c.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/int2float.v` & `circuitgraph-0.2.1/circuitgraph/netlists/int2float.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/log2.v` & `circuitgraph-0.2.1/circuitgraph/netlists/log2.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/max.v` & `circuitgraph-0.2.1/circuitgraph/netlists/max.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/memctrl.v` & `circuitgraph-0.2.1/circuitgraph/netlists/memctrl.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/multiplier.v` & `circuitgraph-0.2.1/circuitgraph/netlists/multiplier.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/mux_4.v` & `circuitgraph-0.2.1/circuitgraph/netlists/mux_4.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/priority_ckt.v` & `circuitgraph-0.2.1/circuitgraph/netlists/priority_ckt.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/router.v` & `circuitgraph-0.2.1/circuitgraph/netlists/router.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/s27.v` & `circuitgraph-0.2.1/circuitgraph/netlists/s27.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/s27_unrolled_4.v` & `circuitgraph-0.2.1/circuitgraph/netlists/s27_unrolled_4.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/sin.v` & `circuitgraph-0.2.1/circuitgraph/netlists/sin.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/sqrt.v` & `circuitgraph-0.2.1/circuitgraph/netlists/sqrt.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/square.v` & `circuitgraph-0.2.1/circuitgraph/netlists/square.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/netlists/voter.v` & `circuitgraph-0.2.1/circuitgraph/netlists/voter.v`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/parsing/fast_verilog.py` & `circuitgraph-0.2.1/circuitgraph/parsing/fast_verilog.py`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/parsing/verilog.lark` & `circuitgraph-0.2.1/circuitgraph/parsing/verilog.lark`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/circuitgraph/parsing/verilog.py` & `circuitgraph-0.2.1/circuitgraph/parsing/verilog.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         self.text = text
         self.blackboxes = blackboxes
         self.warnings = warnings
         self.error_on_warning = error_on_warning
         self.tie_0 = self.c.add("tie_0", "0")
         self.tie_1 = self.c.add("tie_1", "1")
         self.tie_x = self.c.add("tie_x", "x")
+        self.gate_expressions = set()
         self.io = set()
         self.inputs = set()
         self.outputs = set()
         self.wires = set()
 
     # Helper functions
     def add_node(self, n, node_type, fanin=None, fanout=None, uid=False):
@@ -279,15 +280,18 @@
         [identifier, expression] = identifier_and_expression
         return {identifier: expression}
 
     # 5. Behavioral Statements
     def assignment(self, lvalue_and_expression):
         [lvalue, expression] = lvalue_and_expression
         if lvalue not in [self.tie_0, self.tie_1, self.tie_x]:
-            self.add_node(lvalue, "buf", fanin=expression)
+            if expression in self.gate_expressions:
+                self.c.relabel({expression: str(lvalue)})
+            else:
+                self.add_node(lvalue, "buf", fanin=expression)
 
     # 6. Specify Section
 
     # 7. Expressions
     def expression(self, s):
         return s[0]
 
@@ -298,38 +302,50 @@
         return self.tie_1
 
     def constant_x(self, value):
         return self.tie_x
 
     def not_gate(self, items):
         io = "_".join(items)
-        return self.add_node(f"not_{io}", "not", fanin=items[0], uid=True)
+        node = self.add_node(f"not_{io}", "not", fanin=items[0], uid=True)
+        self.gate_expressions.add(node)
+        return node
 
     def xor_gate(self, items):
         io = "_".join(items)
-        return self.add_node(f"xor_{io}", "xor", fanin=[items[0], items[1]], uid=True)
+        node = self.add_node(f"xor_{io}", "xor", fanin=[items[0], items[1]], uid=True)
+        self.gate_expressions.add(node)
+        return node
 
     def xnor_gate(self, items):
         io = "_".join(items)
-        return self.add_node(f"xnor_{io}", "xnor", fanin=[items[0], items[1]], uid=True)
+        node = self.add_node(f"xnor_{io}", "xnor", fanin=[items[0], items[1]], uid=True)
+        self.gate_expressions.add(node)
+        return node
 
     def and_gate(self, items):
         io = "_".join(items)
-        return self.add_node(f"and_{io}", "and", fanin=[items[0], items[1]], uid=True)
+        node = self.add_node(f"and_{io}", "and", fanin=[items[0], items[1]], uid=True)
+        self.gate_expressions.add(node)
+        return node
 
     def or_gate(self, items):
         io = "_".join(items)
-        return self.add_node(f"or_{io}", "or", fanin=[items[0], items[1]], uid=True)
+        node = self.add_node(f"or_{io}", "or", fanin=[items[0], items[1]], uid=True)
+        self.gate_expressions.add(node)
+        return node
 
     def ternary(self, items):
         io = "_".join(items)
         n = self.add_node(f"mux_n_{io}", "not", fanin=items[0], uid=True)
         a0 = self.add_node(f"mux_a0_{io}", "and", fanin=[n, items[2]], uid=True)
         a1 = self.add_node(f"mux_a1_{io}", "and", fanin=[items[0], items[1]], uid=True)
-        return self.add_node(f"mux_o_{io}", "or", fanin=[a0, a1], uid=True)
+        node = self.add_node(f"mux_o_{io}", "or", fanin=[a0, a1], uid=True)
+        self.gate_expressions.add(node)
+        return node
 
 
 def parse_verilog_netlist(netlist, blackboxes, warnings=False, error_on_warning=False):
     """
     Parse a verilog netlist into a Circuit.
 
     Parameters
```

### Comparing `circuitgraph-0.2.0/circuitgraph/props.py` & `circuitgraph-0.2.1/circuitgraph/props.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Compute the influences at node(s).
 
     Parameters
     ----------
     c : Circuit
             Circuit to compute influence for.
     ns : str or list of str
-            Node(s) to compute average sensitivity for.
+            Node(s) to compute influence for.
     supergates : bool
             If True, break computation into supergates.
     approx : bool
             Compute approximate model count using approxmc.
     log_dir: str or pathlib.Path
             Directory to store approxmc logs in.
     kwargs: Keyword arguments
@@ -69,18 +69,25 @@
         def mc(circuit, startpoint, endpoints=None):
             i = cg.tx.sensitization_transform(circuit, startpoint, endpoints)
             if approx:
                 log_file = None
                 if log_dir:
                     log_file = log_dir / f"{s}.approxmc.log"
                     count = cg.sat.approx_model_count(
-                        i, {"sat": True}, log_file=log_file, **kwargs,
+                        i,
+                        {"sat": True},
+                        log_file=log_file,
+                        **kwargs,
                     )
                 else:
-                    count = cg.sat.approx_model_count(i, {"sat": True}, **kwargs,)
+                    count = cg.sat.approx_model_count(
+                        i,
+                        {"sat": True},
+                        **kwargs,
+                    )
             else:
                 count = cg.sat.model_count(i, {"sat": True})
             return count
 
         influences = {}
 
         if supergates:
@@ -258,7 +265,34 @@
     # get count with node true and other inputs fixed
     if approx:
         count = cg.sat.approx_model_count(subc, {n: True}, **kwargs)
     else:
         count = cg.sat.model_count(subc, {n: True})
 
     return count / (2 ** len(subc.startpoints()))
+
+
+def levelize(c):
+    """
+    Levelize a circuit.
+
+    Compute the logical level of each gate in the circuit.
+
+    Parameters
+    ----------
+    c: Circuit
+            Input circuit.
+
+    Returns
+    -------
+    dict of str:int
+            Mapping of gate names to levels.
+    """
+    if c.is_cyclic():
+        raise ValueError("Cannot levelize cyclic circuit")
+
+    levels = {n: 0 for n in c.inputs() | c.filter_type(("0", "1", "x"))}
+    for n in c.topo_sort():
+        if n in levels:
+            continue
+        levels[n] = max(levels[fi] for fi in c.fanin(n)) + 1
+    return levels
```

### Comparing `circuitgraph-0.2.0/circuitgraph/sat.py` & `circuitgraph-0.2.1/circuitgraph/sat.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,55 +43,64 @@
 
 def remap(clauses, offset):
     """Remap clauses of a formula."""
     new_clauses = [[v + offset if v > 0 else v - offset for v in c] for c in clauses]
     return new_clauses
 
 
-def construct_solver(c, assumptions=None, engine="cadical"):
+def construct_solver(c, assumptions=None, solver_cls=None, solver_args=None):
     """
     Construct a SAT solver instance with the given circuit and assumptions.
 
     Parameters
     ----------
     c : Circuit
             Circuit to encode.
     assumptions : dict of str:int
             Assumptions to add to solver.
+    solver_cls : pysat.Solver
+            The class of solver to use. If None, `Cadical` is used.
+    solver_args : dict of str:Any
+            Arguments to pass into the solver constructor. For `Glucose`
+            solvers, this should include `'incr': True` to set incremental
+            mode.
 
     Returns
     -------
-    solver : pysat.Cadical
+    solver : pysat.Solver
             SAT solver instance.
     variables : pysat.IDPool
             Solver variable mapping.
 
     """
-    try:
-        from pysat.solvers import Cadical, Glucose4, Lingeling
-    except ImportError as e:
-        raise ImportError(
-            "Install 'python-sat' to use satisfiability functionality"
-        ) from e
+    if not solver_cls:
+        try:
+            from pysat.solvers import Cadical153
+
+            solver_cls = Cadical153
+        except ImportError:
+            try:
+                from pysat.solvers import Cadical
+
+                solver_cls = Cadical
+            except ImportError as e:
+                raise ImportError(
+                    "Install 'python-sat' to use satisfiability functionality"
+                ) from e
 
     formula, variables = cnf(c)
     if assumptions:
         for n in assumptions.keys():
             if n not in c:
                 raise ValueError(f"Node '{n}' in assumptions is not in circuit")
         add_assumptions(formula, variables, assumptions)
 
-    if engine == "cadical":
-        solver = Cadical(bootstrap_with=formula)
-    elif engine == "glucose":
-        solver = Glucose4(bootstrap_with=formula, incr=True)
-    elif engine == "lingeling":
-        solver = Lingeling(bootstrap_with=formula)
-    else:
-        raise ValueError(f"unsupported solver: {engine}")
+    if not solver_args:
+        solver_args = {}
+    solver = solver_cls(bootstrap_with=formula, **solver_args)
     return solver, variables
 
 
 def cnf(c):
     """
     Convert circuit to CNF using the Tseitin transformation.
 
@@ -362,15 +371,22 @@
             cmd.append(f"--seed={seed}")
         if not detach_xor:
             cmd.append("--detachxor=0")
         cmd.append(tmp.name)
         with open(log_file, "w+") if log_file else tempfile.NamedTemporaryFile(
             prefix=f"circuitgraph_approxmc_{c.name}_log", mode="w+"
         ) as f:
-            subprocess.run(cmd, stdout=f, stderr=f, check=True, text=True)
+            subprocess.run(
+                cmd,
+                stdout=f,
+                stderr=f,
+                check=True,
+                encoding="utf8",
+                universal_newlines=True,
+            )
             f.seek(0)
             result = f.read()
 
     # parse results
     m = re.search(r"s mc (\d+)", result)
     if not m:
         raise ValueError(f"approxmc produced unexpected result:\n\n{result}")
```

### Comparing `circuitgraph-0.2.0/circuitgraph/tx.py` & `circuitgraph-0.2.1/circuitgraph/tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,14 +401,49 @@
                     replace_gate,
                     output_netlist,
                 )
 
     return cg.io.verilog_to_circuit(output_netlist, c.name, fast=fast_parsing)
 
 
+def aig(c):
+    """
+    Transform a circuit into and and-inverter graph.
+
+    Parameters
+    ----------
+    c: Circuit
+            The circuit to transform to an AIG.
+
+    Returns
+    -------
+    Circuit
+            The AIG circuit.
+
+    """
+    with NamedTemporaryFile(
+        prefix="circuitgraph_aig_input", suffix=".v", mode="w"
+    ) as tmp_in:
+        cg.to_file(c, tmp_in.name)
+        with NamedTemporaryFile(
+            prefix="circuitgraph_aig_output", suffix=".v", mode="r"
+        ) as tmp_out:
+            execute = (
+                f"read_verilog {tmp_in.name}; aigmap; "
+                "opt; "
+                f"write_verilog -noattr {tmp_out.name}"
+            )
+            subprocess.run(
+                ["yosys", "-p", execute], stdout=subprocess.DEVNULL, check=True
+            )
+            c = cg.from_file(tmp_out.name)
+    # c = remove_bufs(c)
+    return c
+
+
 def ternary(c):
     """
     Encode the circuit with ternary values.
 
     The ternary circuit adds a second net for each net in the original circuit.
     The second net encodes a don't care, or X, value. That net being high
     corresponds to a don't care value on original net. If the second net is
@@ -486,15 +521,15 @@
                 add_connected_nodes=True,
                 allow_redefinition=True,
             )
         elif c.type(n) in ["xor", "xnor"]:
             t.add(
                 mapping[n],
                 "or",
-                fanin=(mapping[p] for p in c.fanin(n)),
+                fanin=[mapping[p] for p in c.fanin(n)],
                 output=c.is_output(n),
                 add_connected_nodes=True,
                 allow_redefinition=True,
             )
         elif c.type(n) in ["0", "1"]:
             t.add(mapping[n], "0", output=c.is_output(n), allow_redefinition=True)
         elif c.type(n) in ["input"]:
@@ -846,24 +881,24 @@
     Reduce the maximum fanin of circuit gates to k.
 
     Parameters
     ----------
     c : Circuit
             Input circuit.
     k : str
-            Maximum fanin. (k > 2)
+            Maximum fanin. (k >= 2)
 
     Returns
     -------
     Circuit
             Output circuit.
 
     """
     if k < 2:
-        raise ValueError("maximum fanin, k, must be > 2")
+        raise ValueError(f"'k' must be >= 2, not '{k}'")
 
     gatemap = {
         "and": "and",
         "nand": "and",
         "or": "or",
         "nor": "or",
         "xor": "xor",
@@ -886,14 +921,54 @@
                 uid=True,
             )
             i += 1
 
     return ck
 
 
+def limit_fanout(c, k):
+    """
+    Reduce the maximum fanout of circuit gates to k.
+
+    Parameters
+    ----------
+    c : Circuit
+            Input circuit.
+    k : str
+            Maximum fanout. (k >= 2)
+
+    Returns
+    -------
+    Circuit
+            Output circuit.
+
+    """
+    if k < 2:
+        raise ValueError(f"'k' must be >= 2, not '{k}'")
+
+    ck = c.copy()
+    for n in ck.nodes():
+        i = 0
+        while len(ck.fanout(n)) > k:
+            fo = ck.fanout(n)
+            f0 = fo.pop()
+            f1 = fo.pop()
+            ck.disconnect(n, [f0, f1])
+            ck.add(
+                f"{n}_limit_fanout_{i}",
+                "buf",
+                fanin=n,
+                fanout=[f0, f1],
+                uid=True,
+            )
+            i += 1
+
+    return ck
+
+
 def acyclic_unroll(c):
     """
     Unroll a cyclic circuit to remove cycles.
 
     Parameters
     ----------
     c: Circuit
@@ -1116,7 +1191,72 @@
                 if i in other_supergate.nodes() - other_supergate.inputs():
                     g.add_edge(other_output, output)
 
     sorted_supergate_circuits = []
     for node in nx.topological_sort(g):
         sorted_supergate_circuits.append(minimal_supergate_circuits[node])
     return sorted_supergate_circuits
+
+
+def insert_registers(
+    c,
+    num_stages,
+    ff=cg.generic_flop,
+    d_port="d",
+    q_port="q",
+    other_flop_io={"clk": "clk"},
+    q_suffix="_cg_insert_reg_q_",
+):
+    """
+    Insert pipeline registers into a combinational design.
+
+    Parameters
+    ----------
+    c: circuitgraph.Circuit
+            The circuit to insert registers into.
+    num_stages: int
+            The number of stages to add.
+    ff: circuitgraph.BlackBox
+            The flip flop blackbox to use.
+    d_port: str
+            The d port on the flip flop blackbox.
+    q_port: str
+            The q port on the flip flop blackbox.
+    other_flop_io: dict of str:str
+            Other io to connect on the flop (e.g. clk, rst ports).
+            Dict maps circuit nodes to flop ports. If a node is
+            present in the dict but not in the circuit, it will be
+            added as an input.
+    q_suffix: str
+            Inserted q nodes are named with the suffix `{q_suffix}{i}` where
+            `i` is the level the flop is inserted at.
+
+    Returns
+    -------
+    circuitgraph.Circuit
+            The circuit with added registers.
+
+    """
+    c_reg = c.copy()
+    nodes_at_depths = []
+    max_depth = 0
+    for n in c_reg:
+        depth = c_reg.fanin_depth(n)
+        while depth >= len(nodes_at_depths):
+            nodes_at_depths.append([])
+        nodes_at_depths[depth].append(n)
+        if depth > max_depth:
+            max_depth = depth
+
+    depth_inc = round(max_depth / (num_stages + 1))
+    for n in other_flop_io:
+        if n not in c_reg:
+            c_reg.add(n, "input")
+    for i in range(depth_inc, max_depth, depth_inc):
+        for n in nodes_at_depths[i]:
+            fanout = c_reg.fanout(n)
+            c_reg.disconnect(n, fanout)
+            q = c_reg.add(f"{n}{q_suffix}{i}", "buf", uid=True, fanout=fanout)
+            conns = {d_port: n, q_port: q}
+            conns.update(other_flop_io)
+            c_reg.add_blackbox(ff, f"ff_{n}", conns)
+    return c_reg
```

### Comparing `circuitgraph-0.2.0/circuitgraph/utils.py` & `circuitgraph-0.2.1/circuitgraph/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             tmp_in.write(bytes(bb_verilog, "ascii"))
             tmp_in.flush()
 
         cmd = [
             "yosys",
             "-p",
             f"read_verilog {tmp_in.name}; "
-            f"show -format {fmt} -prefix {prefix} {c.name}",
+            f"show -stretch -format {fmt} -prefix {prefix} {c.name}",
         ]
         subprocess.run(cmd, stdout=stdout, check=True)
 
     # Remove intermediate dot files if necessary
     if fmt != "dot":
         prefix.with_suffix(".dot").unlink()
```

### Comparing `circuitgraph-0.2.0/circuitgraph.egg-info/PKG-INFO` & `circuitgraph-0.2.1/circuitgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: circuitgraph
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tools for working with boolean circuits as graphs.
 Home-page: https://github.com/circuitgraph/circuitgraph
 Author: Ruben Purdy, Joseph Sweeney
 Author-email: rpurdy@andrew.cmu.edu, joesweeney@cmu.edu
-License: UNKNOWN
 Project-URL: Documentation, https://circuitgraph.github.io/circuitgraph/
 Project-URL: Source, https://github.com/circuitgraph/circuitgraph
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -42,15 +40,15 @@
 cg.to_file(c, '/path/to/output/circuit.v')
 ```
 
 The documentation can be found [here](https://circuitgraph.github.io/circuitgraph/).
 
 ## Installation
 
-CircuitGraph requires Python3.6 or greater
+CircuitGraph requires Python3.7 or greater
 The easiest way to install is via PyPi:
 ```shell
 pip install circuitgraph
 ```
 To install from the release, download and:
 ```shell
 pip install circuitgraph-<release>.tar.gz
@@ -121,9 +119,7 @@
   year={2020}
 }
 ```
 
 ## Acknowledgements
 
 Circuitgraph icon designed by [ncasti](https://github.com/ncasti).
-
-
```

### Comparing `circuitgraph-0.2.0/circuitgraph.egg-info/SOURCES.txt` & `circuitgraph-0.2.1/circuitgraph.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 circuitgraph/netlists/mux_2.v
 circuitgraph/netlists/mux_4.v
 circuitgraph/netlists/priority_ckt.v
 circuitgraph/netlists/router.v
 circuitgraph/netlists/s13207.v
 circuitgraph/netlists/s27.v
 circuitgraph/netlists/s27_unrolled_4.v
+circuitgraph/netlists/s38417.v
+circuitgraph/netlists/s38584.v
 circuitgraph/netlists/sin.v
 circuitgraph/netlists/sqrt.v
 circuitgraph/netlists/square.v
 circuitgraph/netlists/switch.v
 circuitgraph/netlists/voter.v
 circuitgraph/parsing/__init__.py
 circuitgraph/parsing/fast_verilog.py
```

### Comparing `circuitgraph-0.2.0/docs/analysis.html` & `circuitgraph-0.2.1/docs/analysis.html`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/docs/circuit.html` & `circuitgraph-0.2.1/docs/circuit.html`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
         &#34;&#34;&#34;
         return Circuit(
             graph=self.graph.copy(), name=self.name, blackboxes=self.blackboxes.copy()
         )
 
     def set_type(self, ns, t):
         &#34;&#34;&#34;
-        Return node(s) type(s).
+        Set the type of a node or nodes.
 
         Parameters
         ----------
         ns : str or iterable of str
                 Node.
         t : str
                 Type.
@@ -1790,15 +1790,15 @@
         &#34;&#34;&#34;
         return Circuit(
             graph=self.graph.copy(), name=self.name, blackboxes=self.blackboxes.copy()
         )
 
     def set_type(self, ns, t):
         &#34;&#34;&#34;
-        Return node(s) type(s).
+        Set the type of a node or nodes.
 
         Parameters
         ----------
         ns : str or iterable of str
                 Node.
         t : str
                 Type.
@@ -4216,29 +4216,29 @@
         self.graph.nodes[n][&#34;output&#34;] = output</code></pre>
 </details>
 </dd>
 <dt id="circuitgraph.circuit.Circuit.set_type"><code class="name flex">
 <span>def <span class="ident">set_type</span></span>(<span>self, ns, t)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Return node(s) type(s).</p>
+<div class="desc"><p>Set the type of a node or nodes.</p>
 <h2 id="parameters">Parameters</h2>
 <dl>
 <dt><strong><code>ns</code></strong> :&ensp;<code>str</code> or <code>iterable</code> of <code>str</code></dt>
 <dd>Node.</dd>
 <dt><strong><code>t</code></strong> :&ensp;<code>str</code></dt>
 <dd>Type.</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def set_type(self, ns, t):
     &#34;&#34;&#34;
-    Return node(s) type(s).
+    Set the type of a node or nodes.
 
     Parameters
     ----------
     ns : str or iterable of str
             Node.
     t : str
             Type.
@@ -4634,8 +4634,8 @@
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc"><cite>pdoc</cite> 0.10.0</a>.</p>
 </footer>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -315,15 +315,15 @@
         return Circuit(
             graph=self.graph.copy(), name=self.name,
 blackboxes=self.blackboxes.copy()
         )
 
     def set_type(self, ns, t):
         """
-        Return node(s) type(s).
+        Set the type of a node or nodes.
 
         Parameters
         ----------
         ns : str or iterable of str
                 Node.
         t : str
                 Type.
@@ -1716,15 +1716,15 @@
               return Circuit(
                   graph=self.graph.copy(), name=self.name,
       blackboxes=self.blackboxes.copy()
               )
 
           def set_type(self, ns, t):
               """
-              Return node(s) type(s).
+              Set the type of a node or nodes.
 
               Parameters
               ----------
               ns : str or iterable of str
                       Node.
               t : str
                       Type.
@@ -3902,24 +3902,24 @@
 
                 """
                 if isinstance(ns, str):
                     ns = [ns]
                 for n in ns:
                     self.graph.nodes[n]["output"] = output
         def set_type(self, ns, t)
-            Return node(s) type(s).
+            Set the type of a node or nodes.
             ***** Parameters *****
               ns :&ensp;str or iterable of str
                   Node.
               t :&ensp;str
                   Type.
               Expand source code
             def set_type(self, ns, t):
                 """
-                Return node(s) type(s).
+                Set the type of a node or nodes.
 
                 Parameters
                 ----------
                 ns : str or iterable of str
                         Node.
                 t : str
                         Type.
```

### Comparing `circuitgraph-0.2.0/docs/circuitgraph.html` & `circuitgraph-0.2.1/docs/circuitgraph.html`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/docs/circuitgraph.png` & `circuitgraph-0.2.1/docs/circuitgraph.png`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/docs/index.html` & `circuitgraph-0.2.1/docs/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,22 @@
 from circuitgraph.circuit import (
     BlackBox,
     Circuit,
     primitive_gates,
     addable_types,
     supported_types,
 )
-from circuitgraph.io import dc_flops, from_file, from_lib, genus_flops, to_file
+from circuitgraph.io import (
+    generic_flop,
+    dc_flops,
+    from_file,
+    from_lib,
+    genus_flops,
+    to_file,
+)
 from circuitgraph.utils import lint, visualize
 from circuitgraph import logic, props, sat, tx, utils</code></pre>
 </details>
 </section>
 <section>
 <h2 class="section-title" id="header-submodules">Sub-modules</h2>
 <dl>
@@ -138,8 +145,8 @@
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc"><cite>pdoc</cite> 0.10.0</a>.</p>
 </footer>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -39,15 +39,22 @@
 from circuitgraph.circuit import (
     BlackBox,
     Circuit,
     primitive_gates,
     addable_types,
     supported_types,
 )
-from circuitgraph.io import dc_flops, from_file, from_lib, genus_flops, to_file
+from circuitgraph.io import (
+    generic_flop,
+    dc_flops,
+    from_file,
+    from_lib,
+    genus_flops,
+    to_file,
+)
 from circuitgraph.utils import lint, visualize
 from circuitgraph import logic, props, sat, tx, utils
 
 ***** Sub-modules *****
   circuitgraph.circuit
       Class for circuit graphs â¦
   circuitgraph.io
```

### Comparing `circuitgraph-0.2.0/docs/io.html` & `circuitgraph-0.2.1/docs/io.html`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 <pre><code class="python">&#34;&#34;&#34;Functions for reading/writing CircuitGraphs.&#34;&#34;&#34;
 import re
 from pathlib import Path
 
 from circuitgraph import BlackBox, Circuit
 from circuitgraph.parsing import fast_parse_verilog_netlist, parse_verilog_netlist
 
+generic_flop = BlackBox(&#34;ff&#34;, [&#34;clk&#34;, &#34;d&#34;], [&#34;q&#34;])
+
 genus_flops = [
     BlackBox(&#34;flopd&#34;, [&#34;CK&#34;, &#34;D&#34;], [&#34;Q&#34;]),
     BlackBox(&#34;fflopd&#34;, [&#34;CK&#34;, &#34;D&#34;], [&#34;Q&#34;]),
     BlackBox(&#34;flopdrs&#34;, [&#34;CK&#34;, &#34;D&#34;, &#34;R&#34;, &#34;S&#34;], [&#34;Q&#34;]),
     BlackBox(&#34;fflopdrs&#34;, [&#34;CK&#34;, &#34;D&#34;, &#34;R&#34;, &#34;S&#34;], [&#34;Q&#34;]),
 ]
 
@@ -123,15 +125,15 @@
 
     Returns
     -------
     Circuit
             the parsed circuit.
 
     &#34;&#34;&#34;
-    bbs = [BlackBox(&#34;ff&#34;, [&#34;CK&#34;, &#34;D&#34;], [&#34;Q&#34;])]
+    bbs = [BlackBox(&#34;ff&#34;, [&#34;CK&#34;, &#34;D&#34;], [&#34;Q&#34;])] + genus_flops + dc_flops
     [path] = Path(__file__).parent.absolute().glob(f&#34;netlists/{name}.*&#34;)
     return from_file(path, name, blackboxes=bbs)
 
 
 def bench_to_circuit(netlist, name):
     &#34;&#34;&#34;
     Create a new Circuit from a netlist string.
@@ -360,15 +362,16 @@
                     fanin = f&#34; {symbol} &#34;.join(fanin)
                     if c.type(n) in [&#34;xnor&#34;, &#34;nor&#34;, &#34;nand&#34;]:
                         insts.append(f&#34;assign {n} = ~({fanin})&#34;)
                     else:
                         insts.append(f&#34;assign {n} = {fanin}&#34;)
             else:
                 fanin = &#34;, &#34;.join(fanin)
-                insts.append(f&#34;{c.type(n)} g_{len(insts)} &#34; f&#34;({n}, {fanin})&#34;)
+                gate_name = c.uid(f&#34;g_{len(insts)}&#34;)
+                insts.append(f&#34;{c.type(n)} {gate_name}({n}, {fanin})&#34;)
         elif c.type(n) in [&#34;0&#34;, &#34;1&#34;, &#34;x&#34;]:
             insts.append(f&#34;assign {n} = 1&#39;b{c.type(n)}&#34;)
             wires.append(n)
         elif c.type(n) in [&#34;input&#34;, &#34;bb_input&#34;, &#34;bb_output&#34;]:
             pass
         else:
             raise ValueError(f&#34;unknown gate type: {c.type(n)}&#34;)
@@ -679,15 +682,16 @@
                     fanin = f&#34; {symbol} &#34;.join(fanin)
                     if c.type(n) in [&#34;xnor&#34;, &#34;nor&#34;, &#34;nand&#34;]:
                         insts.append(f&#34;assign {n} = ~({fanin})&#34;)
                     else:
                         insts.append(f&#34;assign {n} = {fanin}&#34;)
             else:
                 fanin = &#34;, &#34;.join(fanin)
-                insts.append(f&#34;{c.type(n)} g_{len(insts)} &#34; f&#34;({n}, {fanin})&#34;)
+                gate_name = c.uid(f&#34;g_{len(insts)}&#34;)
+                insts.append(f&#34;{c.type(n)} {gate_name}({n}, {fanin})&#34;)
         elif c.type(n) in [&#34;0&#34;, &#34;1&#34;, &#34;x&#34;]:
             insts.append(f&#34;assign {n} = 1&#39;b{c.type(n)}&#34;)
             wires.append(n)
         elif c.type(n) in [&#34;input&#34;, &#34;bb_input&#34;, &#34;bb_output&#34;]:
             pass
         else:
             raise ValueError(f&#34;unknown gate type: {c.type(n)}&#34;)
@@ -835,15 +839,15 @@
 
     Returns
     -------
     Circuit
             the parsed circuit.
 
     &#34;&#34;&#34;
-    bbs = [BlackBox(&#34;ff&#34;, [&#34;CK&#34;, &#34;D&#34;], [&#34;Q&#34;])]
+    bbs = [BlackBox(&#34;ff&#34;, [&#34;CK&#34;, &#34;D&#34;], [&#34;Q&#34;])] + genus_flops + dc_flops
     [path] = Path(__file__).parent.absolute().glob(f&#34;netlists/{name}.*&#34;)
     return from_file(path, name, blackboxes=bbs)</code></pre>
 </details>
 </dd>
 <dt id="circuitgraph.io.to_file"><code class="name flex">
 <span>def <span class="ident">to_file</span></span>(<span>c, path, fmt='verilog', behavioral=False)</span>
 </code></dt>
@@ -1026,8 +1030,8 @@
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc"><cite>pdoc</cite> 0.10.0</a>.</p>
 </footer>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -12,14 +12,16 @@
 import re
 from pathlib import Path
 
 from circuitgraph import BlackBox, Circuit
 from circuitgraph.parsing import fast_parse_verilog_netlist,
 parse_verilog_netlist
 
+generic_flop = BlackBox("ff", ["clk", "d"], ["q"])
+
 genus_flops = [
     BlackBox("flopd", ["CK", "D"], ["Q"]),
     BlackBox("fflopd", ["CK", "D"], ["Q"]),
     BlackBox("flopdrs", ["CK", "D", "R", "S"], ["Q"]),
     BlackBox("fflopdrs", ["CK", "D", "R", "S"], ["Q"]),
 ]
 
@@ -105,15 +107,15 @@
 
     Returns
     -------
     Circuit
             the parsed circuit.
 
     """
-    bbs = [BlackBox("ff", ["CK", "D"], ["Q"])]
+    bbs = [BlackBox("ff", ["CK", "D"], ["Q"])] + genus_flops + dc_flops
     [path] = Path(__file__).parent.absolute().glob(f"netlists/{name}.*")
     return from_file(path, name, blackboxes=bbs)
 
 
 def bench_to_circuit(netlist, name):
     """
     Create a new Circuit from a netlist string.
@@ -351,15 +353,16 @@
                     fanin = f" {symbol} ".join(fanin)
                     if c.type(n) in ["xnor", "nor", "nand"]:
                         insts.append(f"assign {n} = ~({fanin})")
                     else:
                         insts.append(f"assign {n} = {fanin}")
             else:
                 fanin = ", ".join(fanin)
-                insts.append(f"{c.type(n)} g_{len(insts)} " f"({n}, {fanin})")
+                gate_name = c.uid(f"g_{len(insts)}")
+                insts.append(f"{c.type(n)} {gate_name}({n}, {fanin})")
         elif c.type(n) in ["0", "1", "x"]:
             insts.append(f"assign {n} = 1'b{c.type(n)}")
             wires.append(n)
         elif c.type(n) in ["input", "bb_input", "bb_output"]:
             pass
         else:
             raise ValueError(f"unknown gate type: {c.type(n)}")
@@ -640,16 +643,16 @@
                           fanin = f" {symbol} ".join(fanin)
                           if c.type(n) in ["xnor", "nor", "nand"]:
                               insts.append(f"assign {n} = ~({fanin})")
                           else:
                               insts.append(f"assign {n} = {fanin}")
                   else:
                       fanin = ", ".join(fanin)
-                      insts.append(f"{c.type(n)} g_{len(insts)} " f"({n},
-      {fanin})")
+                      gate_name = c.uid(f"g_{len(insts)}")
+                      insts.append(f"{c.type(n)} {gate_name}({n}, {fanin})")
               elif c.type(n) in ["0", "1", "x"]:
                   insts.append(f"assign {n} = 1'b{c.type(n)}")
                   wires.append(n)
               elif c.type(n) in ["input", "bb_input", "bb_output"]:
                   pass
               else:
                   raise ValueError(f"unknown gate type: {c.type(n)}")
@@ -776,15 +779,15 @@
 
           Returns
           -------
           Circuit
                   the parsed circuit.
 
           """
-          bbs = [BlackBox("ff", ["CK", "D"], ["Q"])]
+          bbs = [BlackBox("ff", ["CK", "D"], ["Q"])] + genus_flops + dc_flops
           [path] = Path(__file__).parent.absolute().glob(f"netlists/{name}.*")
           return from_file(path, name, blackboxes=bbs)
   def to_file(c, path, fmt='verilog', behavioral=False)
       Write a Circuit to a Verilog file.
       ***** Parameters *****
         c :&ensp;Circut
             the circuit
```

### Comparing `circuitgraph-0.2.0/docs/locks.html` & `circuitgraph-0.2.1/docs/locks.html`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/docs/logic.html` & `circuitgraph-0.2.1/docs/logic.html`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/docs/paper.bib` & `circuitgraph-0.2.1/docs/paper.bib`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/docs/paper.md` & `circuitgraph-0.2.1/docs/paper.md`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/docs/props.html` & `circuitgraph-0.2.1/docs/props.html`

 * *Files 10% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     Compute the influences at node(s).
 
     Parameters
     ----------
     c : Circuit
             Circuit to compute influence for.
     ns : str or list of str
-            Node(s) to compute average sensitivity for.
+            Node(s) to compute influence for.
     supergates : bool
             If True, break computation into supergates.
     approx : bool
             Compute approximate model count using approxmc.
     log_dir: str or pathlib.Path
             Directory to store approxmc logs in.
     kwargs: Keyword arguments
@@ -114,18 +114,25 @@
         def mc(circuit, startpoint, endpoints=None):
             i = cg.tx.sensitization_transform(circuit, startpoint, endpoints)
             if approx:
                 log_file = None
                 if log_dir:
                     log_file = log_dir / f&#34;{s}.approxmc.log&#34;
                     count = cg.sat.approx_model_count(
-                        i, {&#34;sat&#34;: True}, log_file=log_file, **kwargs,
+                        i,
+                        {&#34;sat&#34;: True},
+                        log_file=log_file,
+                        **kwargs,
                     )
                 else:
-                    count = cg.sat.approx_model_count(i, {&#34;sat&#34;: True}, **kwargs,)
+                    count = cg.sat.approx_model_count(
+                        i,
+                        {&#34;sat&#34;: True},
+                        **kwargs,
+                    )
             else:
                 count = cg.sat.model_count(i, {&#34;sat&#34;: True})
             return count
 
         influences = {}
 
         if supergates:
@@ -302,15 +309,42 @@
 
     # get count with node true and other inputs fixed
     if approx:
         count = cg.sat.approx_model_count(subc, {n: True}, **kwargs)
     else:
         count = cg.sat.model_count(subc, {n: True})
 
-    return count / (2 ** len(subc.startpoints()))</code></pre>
+    return count / (2 ** len(subc.startpoints()))
+
+
+def levelize(c):
+    &#34;&#34;&#34;
+    Levelize a circuit.
+
+    Compute the logical level of each gate in the circuit.
+
+    Parameters
+    ----------
+    c: Circuit
+            Input circuit.
+
+    Returns
+    -------
+    dict of str:int
+            Mapping of gate names to levels.
+    &#34;&#34;&#34;
+    if c.is_cyclic():
+        raise ValueError(&#34;Cannot levelize cyclic circuit&#34;)
+
+    levels = {n: 0 for n in c.inputs() | c.filter_type((&#34;0&#34;, &#34;1&#34;, &#34;x&#34;))}
+    for n in c.topo_sort():
+        if n in levels:
+            continue
+        levels[n] = max(levels[fi] for fi in c.fanin(n)) + 1
+    return levels</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
@@ -396,15 +430,15 @@
 <dd>
 <div class="desc"><p>Compute the influences at node(s).</p>
 <h2 id="parameters">Parameters</h2>
 <dl>
 <dt><strong><code>c</code></strong> :&ensp;<code>Circuit</code></dt>
 <dd>Circuit to compute influence for.</dd>
 <dt><strong><code>ns</code></strong> :&ensp;<code>str</code> or <code>list</code> of <code>str</code></dt>
-<dd>Node(s) to compute average sensitivity for.</dd>
+<dd>Node(s) to compute influence for.</dd>
 <dt><strong><code>supergates</code></strong> :&ensp;<code>bool</code></dt>
 <dd>If True, break computation into supergates.</dd>
 <dt><strong><code>approx</code></strong> :&ensp;<code>bool</code></dt>
 <dd>Compute approximate model count using approxmc.</dd>
 <dt><strong><code>log_dir</code></strong> :&ensp;<code>str</code> or <code>pathlib.Path</code></dt>
 <dd>Directory to store approxmc logs in.</dd>
 <dt><strong><code>kwargs</code></strong> :&ensp;<code>Keyword arguments</code></dt>
@@ -425,15 +459,15 @@
     Compute the influences at node(s).
 
     Parameters
     ----------
     c : Circuit
             Circuit to compute influence for.
     ns : str or list of str
-            Node(s) to compute average sensitivity for.
+            Node(s) to compute influence for.
     supergates : bool
             If True, break computation into supergates.
     approx : bool
             Compute approximate model count using approxmc.
     log_dir: str or pathlib.Path
             Directory to store approxmc logs in.
     kwargs: Keyword arguments
@@ -465,18 +499,25 @@
         def mc(circuit, startpoint, endpoints=None):
             i = cg.tx.sensitization_transform(circuit, startpoint, endpoints)
             if approx:
                 log_file = None
                 if log_dir:
                     log_file = log_dir / f&#34;{s}.approxmc.log&#34;
                     count = cg.sat.approx_model_count(
-                        i, {&#34;sat&#34;: True}, log_file=log_file, **kwargs,
+                        i,
+                        {&#34;sat&#34;: True},
+                        log_file=log_file,
+                        **kwargs,
                     )
                 else:
-                    count = cg.sat.approx_model_count(i, {&#34;sat&#34;: True}, **kwargs,)
+                    count = cg.sat.approx_model_count(
+                        i,
+                        {&#34;sat&#34;: True},
+                        **kwargs,
+                    )
             else:
                 count = cg.sat.model_count(i, {&#34;sat&#34;: True})
             return count
 
         influences = {}
 
         if supergates:
@@ -516,14 +557,61 @@
         all_influences[n] = influences
 
     if len(all_influences) == 1:
         (all_influences,) = all_influences.values()
     return all_influences</code></pre>
 </details>
 </dd>
+<dt id="circuitgraph.props.levelize"><code class="name flex">
+<span>def <span class="ident">levelize</span></span>(<span>c)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Levelize a circuit.</p>
+<p>Compute the logical level of each gate in the circuit.</p>
+<h2 id="parameters">Parameters</h2>
+<dl>
+<dt><strong><code>c</code></strong> :&ensp;<code>Circuit</code></dt>
+<dd>Input circuit.</dd>
+</dl>
+<h2 id="returns">Returns</h2>
+<dl>
+<dt><code>dict</code> of <code>str:int</code></dt>
+<dd>Mapping of gate names to levels.</dd>
+</dl></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def levelize(c):
+    &#34;&#34;&#34;
+    Levelize a circuit.
+
+    Compute the logical level of each gate in the circuit.
+
+    Parameters
+    ----------
+    c: Circuit
+            Input circuit.
+
+    Returns
+    -------
+    dict of str:int
+            Mapping of gate names to levels.
+    &#34;&#34;&#34;
+    if c.is_cyclic():
+        raise ValueError(&#34;Cannot levelize cyclic circuit&#34;)
+
+    levels = {n: 0 for n in c.inputs() | c.filter_type((&#34;0&#34;, &#34;1&#34;, &#34;x&#34;))}
+    for n in c.topo_sort():
+        if n in levels:
+            continue
+        levels[n] = max(levels[fi] for fi in c.fanin(n)) + 1
+    return levels</code></pre>
+</details>
+</dd>
 <dt id="circuitgraph.props.sensitivity"><code class="name flex">
 <span>def <span class="ident">sensitivity</span></span>(<span>c, n)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Calculate the sensitivity of node <code>n</code> with respect to its startpoints.</p>
 <h2 id="parameters">Parameters</h2>
 <dl>
@@ -708,23 +796,24 @@
 <ul id="index">
 <li><h3>Super-module</h3>
 <ul>
 <li><code><a title="circuitgraph" href="index.html">circuitgraph</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-functions">Functions</a></h3>
-<ul class="">
+<ul class="two-column">
 <li><code><a title="circuitgraph.props.avg_sensitivity" href="#circuitgraph.props.avg_sensitivity">avg_sensitivity</a></code></li>
 <li><code><a title="circuitgraph.props.influence" href="#circuitgraph.props.influence">influence</a></code></li>
+<li><code><a title="circuitgraph.props.levelize" href="#circuitgraph.props.levelize">levelize</a></code></li>
 <li><code><a title="circuitgraph.props.sensitivity" href="#circuitgraph.props.sensitivity">sensitivity</a></code></li>
 <li><code><a title="circuitgraph.props.sensitize" href="#circuitgraph.props.sensitize">sensitize</a></code></li>
 <li><code><a title="circuitgraph.props.signal_probability" href="#circuitgraph.props.signal_probability">signal_probability</a></code></li>
 </ul>
 </li>
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc"><cite>pdoc</cite> 0.10.0</a>.</p>
 </footer>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -54,15 +54,15 @@
     Compute the influences at node(s).
 
     Parameters
     ----------
     c : Circuit
             Circuit to compute influence for.
     ns : str or list of str
-            Node(s) to compute average sensitivity for.
+            Node(s) to compute influence for.
     supergates : bool
             If True, break computation into supergates.
     approx : bool
             Compute approximate model count using approxmc.
     log_dir: str or pathlib.Path
             Directory to store approxmc logs in.
     kwargs: Keyword arguments
@@ -94,19 +94,25 @@
         def mc(circuit, startpoint, endpoints=None):
             i = cg.tx.sensitization_transform(circuit, startpoint, endpoints)
             if approx:
                 log_file = None
                 if log_dir:
                     log_file = log_dir / f"{s}.approxmc.log"
                     count = cg.sat.approx_model_count(
-                        i, {"sat": True}, log_file=log_file, **kwargs,
+                        i,
+                        {"sat": True},
+                        log_file=log_file,
+                        **kwargs,
                     )
                 else:
-                    count = cg.sat.approx_model_count(i, {"sat": True},
-**kwargs,)
+                    count = cg.sat.approx_model_count(
+                        i,
+                        {"sat": True},
+                        **kwargs,
+                    )
             else:
                 count = cg.sat.model_count(i, {"sat": True})
             return count
 
         influences = {}
 
         if supergates:
@@ -287,14 +293,41 @@
     if approx:
         count = cg.sat.approx_model_count(subc, {n: True}, **kwargs)
     else:
         count = cg.sat.model_count(subc, {n: True})
 
     return count / (2 ** len(subc.startpoints()))
 
+
+def levelize(c):
+    """
+    Levelize a circuit.
+
+    Compute the logical level of each gate in the circuit.
+
+    Parameters
+    ----------
+    c: Circuit
+            Input circuit.
+
+    Returns
+    -------
+    dict of str:int
+            Mapping of gate names to levels.
+    """
+    if c.is_cyclic():
+        raise ValueError("Cannot levelize cyclic circuit")
+
+    levels = {n: 0 for n in c.inputs() | c.filter_type(("0", "1", "x"))}
+    for n in c.topo_sort():
+        if n in levels:
+            continue
+        levels[n] = max(levels[fi] for fi in c.fanin(n)) + 1
+    return levels
+
 ***** Functions *****
   def avg_sensitivity(c, ns, supergates=False, approx=True, log_dir=None,
   **kwargs)
       Calculate the average sensitivity node(s) ns.
       Return the average sensitivity (equal to total influence) of node(s) with
       respect to startpoints.
       ***** Parameters *****
@@ -362,15 +395,15 @@
           return total_influences
   def influence(c, ns, supergates=False, approx=True, log_dir=None, **kwargs)
       Compute the influences at node(s).
       ***** Parameters *****
         c :&ensp;Circuit
             Circuit to compute influence for.
         ns :&ensp;str or list of str
-            Node(s) to compute average sensitivity for.
+            Node(s) to compute influence for.
         supergates :&ensp;bool
             If True, break computation into supergates.
         approx :&ensp;bool
             Compute approximate model count using approxmc.
         log_dir :&ensp;str or pathlib.Path
             Directory to store approxmc logs in.
         kwargs :&ensp;Keyword arguments
@@ -386,15 +419,15 @@
           Compute the influences at node(s).
 
           Parameters
           ----------
           c : Circuit
                   Circuit to compute influence for.
           ns : str or list of str
-                  Node(s) to compute average sensitivity for.
+                  Node(s) to compute influence for.
           supergates : bool
                   If True, break computation into supergates.
           approx : bool
                   Compute approximate model count using approxmc.
           log_dir: str or pathlib.Path
                   Directory to store approxmc logs in.
           kwargs: Keyword arguments
@@ -429,19 +462,25 @@
                   i = cg.tx.sensitization_transform(circuit, startpoint,
       endpoints)
                   if approx:
                       log_file = None
                       if log_dir:
                           log_file = log_dir / f"{s}.approxmc.log"
                           count = cg.sat.approx_model_count(
-                              i, {"sat": True}, log_file=log_file, **kwargs,
+                              i,
+                              {"sat": True},
+                              log_file=log_file,
+                              **kwargs,
                           )
                       else:
-                          count = cg.sat.approx_model_count(i, {"sat": True},
-      **kwargs,)
+                          count = cg.sat.approx_model_count(
+                              i,
+                              {"sat": True},
+                              **kwargs,
+                          )
                   else:
                       count = cg.sat.model_count(i, {"sat": True})
                   return count
 
               influences = {}
 
               if supergates:
@@ -481,14 +520,49 @@
                       influences[s] = mc(c, s, n) / (2 ** len(sp))
 
               all_influences[n] = influences
 
           if len(all_influences) == 1:
               (all_influences,) = all_influences.values()
           return all_influences
+  def levelize(c)
+      Levelize a circuit.
+      Compute the logical level of each gate in the circuit.
+      ***** Parameters *****
+        c :&ensp;Circuit
+            Input circuit.
+      ***** Returns *****
+        dict of str:int
+            Mapping of gate names to levels.
+        Expand source code
+      def levelize(c):
+          """
+          Levelize a circuit.
+
+          Compute the logical level of each gate in the circuit.
+
+          Parameters
+          ----------
+          c: Circuit
+                  Input circuit.
+
+          Returns
+          -------
+          dict of str:int
+                  Mapping of gate names to levels.
+          """
+          if c.is_cyclic():
+              raise ValueError("Cannot levelize cyclic circuit")
+
+          levels = {n: 0 for n in c.inputs() | c.filter_type(("0", "1", "x"))}
+          for n in c.topo_sort():
+              if n in levels:
+                  continue
+              levels[n] = max(levels[fi] for fi in c.fanin(n)) + 1
+          return levels
   def sensitivity(c, n)
       Calculate the sensitivity of node n with respect to its startpoints.
       ***** Parameters *****
         c :&ensp;Circuit
             Circuit to compute sensitivity for
         n :&ensp;str
             Node to compute sensitivity for.
@@ -624,12 +698,13 @@
 ****** Index ******
     * Examples
     * **** Super-module ****
           o circuitgraph
     * **** Functions ****
           o avg_sensitivity
           o influence
+          o levelize
           o sensitivity
           o sensitize
           o signal_probability
 
 Generated by pdoc0.10.0.
```

### Comparing `circuitgraph-0.2.0/docs/sat.html` & `circuitgraph-0.2.1/docs/sat.html`

 * *Files 4% similar despite different names*

```diff
@@ -93,55 +93,64 @@
 
 def remap(clauses, offset):
     &#34;&#34;&#34;Remap clauses of a formula.&#34;&#34;&#34;
     new_clauses = [[v + offset if v &gt; 0 else v - offset for v in c] for c in clauses]
     return new_clauses
 
 
-def construct_solver(c, assumptions=None, engine=&#34;cadical&#34;):
+def construct_solver(c, assumptions=None, solver_cls=None, solver_args=None):
     &#34;&#34;&#34;
     Construct a SAT solver instance with the given circuit and assumptions.
 
     Parameters
     ----------
     c : Circuit
             Circuit to encode.
     assumptions : dict of str:int
             Assumptions to add to solver.
+    solver_cls : pysat.Solver
+            The class of solver to use. If None, `Cadical` is used.
+    solver_args : dict of str:Any
+            Arguments to pass into the solver constructor. For `Glucose`
+            solvers, this should include `&#39;incr&#39;: True` to set incremental
+            mode.
 
     Returns
     -------
-    solver : pysat.Cadical
+    solver : pysat.Solver
             SAT solver instance.
     variables : pysat.IDPool
             Solver variable mapping.
 
     &#34;&#34;&#34;
-    try:
-        from pysat.solvers import Cadical, Glucose4, Lingeling
-    except ImportError as e:
-        raise ImportError(
-            &#34;Install &#39;python-sat&#39; to use satisfiability functionality&#34;
-        ) from e
+    if not solver_cls:
+        try:
+            from pysat.solvers import Cadical153
+
+            solver_cls = Cadical153
+        except ImportError:
+            try:
+                from pysat.solvers import Cadical
+
+                solver_cls = Cadical
+            except ImportError as e:
+                raise ImportError(
+                    &#34;Install &#39;python-sat&#39; to use satisfiability functionality&#34;
+                ) from e
 
     formula, variables = cnf(c)
     if assumptions:
         for n in assumptions.keys():
             if n not in c:
                 raise ValueError(f&#34;Node &#39;{n}&#39; in assumptions is not in circuit&#34;)
         add_assumptions(formula, variables, assumptions)
 
-    if engine == &#34;cadical&#34;:
-        solver = Cadical(bootstrap_with=formula)
-    elif engine == &#34;glucose&#34;:
-        solver = Glucose4(bootstrap_with=formula, incr=True)
-    elif engine == &#34;lingeling&#34;:
-        solver = Lingeling(bootstrap_with=formula)
-    else:
-        raise ValueError(f&#34;unsupported solver: {engine}&#34;)
+    if not solver_args:
+        solver_args = {}
+    solver = solver_cls(bootstrap_with=formula, **solver_args)
     return solver, variables
 
 
 def cnf(c):
     &#34;&#34;&#34;
     Convert circuit to CNF using the Tseitin transformation.
 
@@ -412,15 +421,22 @@
             cmd.append(f&#34;--seed={seed}&#34;)
         if not detach_xor:
             cmd.append(&#34;--detachxor=0&#34;)
         cmd.append(tmp.name)
         with open(log_file, &#34;w+&#34;) if log_file else tempfile.NamedTemporaryFile(
             prefix=f&#34;circuitgraph_approxmc_{c.name}_log&#34;, mode=&#34;w+&#34;
         ) as f:
-            subprocess.run(cmd, stdout=f, stderr=f, check=True, text=True)
+            subprocess.run(
+                cmd,
+                stdout=f,
+                stderr=f,
+                check=True,
+                encoding=&#34;utf8&#34;,
+                universal_newlines=True,
+            )
             f.seek(0)
             result = f.read()
 
     # parse results
     m = re.search(r&#34;s mc (\d+)&#34;, result)
     if not m:
         raise ValueError(f&#34;approxmc produced unexpected result:\n\n{result}&#34;)
@@ -650,15 +666,22 @@
             cmd.append(f&#34;--seed={seed}&#34;)
         if not detach_xor:
             cmd.append(&#34;--detachxor=0&#34;)
         cmd.append(tmp.name)
         with open(log_file, &#34;w+&#34;) if log_file else tempfile.NamedTemporaryFile(
             prefix=f&#34;circuitgraph_approxmc_{c.name}_log&#34;, mode=&#34;w+&#34;
         ) as f:
-            subprocess.run(cmd, stdout=f, stderr=f, check=True, text=True)
+            subprocess.run(
+                cmd,
+                stdout=f,
+                stderr=f,
+                check=True,
+                encoding=&#34;utf8&#34;,
+                universal_newlines=True,
+            )
             f.seek(0)
             result = f.read()
 
     # parse results
     m = re.search(r&#34;s mc (\d+)&#34;, result)
     if not m:
         raise ValueError(f&#34;approxmc produced unexpected result:\n\n{result}&#34;)
@@ -789,77 +812,92 @@
         else:
             raise ValueError(f&#34;Unknown gate type &#39;{n_type}&#39;&#34;)
 
     return formula, variables</code></pre>
 </details>
 </dd>
 <dt id="circuitgraph.sat.construct_solver"><code class="name flex">
-<span>def <span class="ident">construct_solver</span></span>(<span>c, assumptions=None, engine='cadical')</span>
+<span>def <span class="ident">construct_solver</span></span>(<span>c, assumptions=None, solver_cls=None, solver_args=None)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Construct a SAT solver instance with the given circuit and assumptions.</p>
 <h2 id="parameters">Parameters</h2>
 <dl>
 <dt><strong><code>c</code></strong> :&ensp;<code>Circuit</code></dt>
 <dd>Circuit to encode.</dd>
 <dt><strong><code>assumptions</code></strong> :&ensp;<code>dict</code> of <code>str:int</code></dt>
 <dd>Assumptions to add to solver.</dd>
+<dt><strong><code>solver_cls</code></strong> :&ensp;<code>pysat.Solver</code></dt>
+<dd>The class of solver to use. If None, <code>Cadical</code> is used.</dd>
+<dt><strong><code>solver_args</code></strong> :&ensp;<code>dict</code> of <code>str:Any</code></dt>
+<dd>Arguments to pass into the solver constructor. For <code>Glucose</code>
+solvers, this should include <code>'incr': True</code> to set incremental
+mode.</dd>
 </dl>
 <h2 id="returns">Returns</h2>
 <dl>
-<dt><strong><code>solver</code></strong> :&ensp;<code>pysat.Cadical</code></dt>
+<dt><strong><code>solver</code></strong> :&ensp;<code>pysat.Solver</code></dt>
 <dd>SAT solver instance.</dd>
 <dt><strong><code>variables</code></strong> :&ensp;<code>pysat.IDPool</code></dt>
 <dd>Solver variable mapping.</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def construct_solver(c, assumptions=None, engine=&#34;cadical&#34;):
+<pre><code class="python">def construct_solver(c, assumptions=None, solver_cls=None, solver_args=None):
     &#34;&#34;&#34;
     Construct a SAT solver instance with the given circuit and assumptions.
 
     Parameters
     ----------
     c : Circuit
             Circuit to encode.
     assumptions : dict of str:int
             Assumptions to add to solver.
+    solver_cls : pysat.Solver
+            The class of solver to use. If None, `Cadical` is used.
+    solver_args : dict of str:Any
+            Arguments to pass into the solver constructor. For `Glucose`
+            solvers, this should include `&#39;incr&#39;: True` to set incremental
+            mode.
 
     Returns
     -------
-    solver : pysat.Cadical
+    solver : pysat.Solver
             SAT solver instance.
     variables : pysat.IDPool
             Solver variable mapping.
 
     &#34;&#34;&#34;
-    try:
-        from pysat.solvers import Cadical, Glucose4, Lingeling
-    except ImportError as e:
-        raise ImportError(
-            &#34;Install &#39;python-sat&#39; to use satisfiability functionality&#34;
-        ) from e
+    if not solver_cls:
+        try:
+            from pysat.solvers import Cadical153
+
+            solver_cls = Cadical153
+        except ImportError:
+            try:
+                from pysat.solvers import Cadical
+
+                solver_cls = Cadical
+            except ImportError as e:
+                raise ImportError(
+                    &#34;Install &#39;python-sat&#39; to use satisfiability functionality&#34;
+                ) from e
 
     formula, variables = cnf(c)
     if assumptions:
         for n in assumptions.keys():
             if n not in c:
                 raise ValueError(f&#34;Node &#39;{n}&#39; in assumptions is not in circuit&#34;)
         add_assumptions(formula, variables, assumptions)
 
-    if engine == &#34;cadical&#34;:
-        solver = Cadical(bootstrap_with=formula)
-    elif engine == &#34;glucose&#34;:
-        solver = Glucose4(bootstrap_with=formula, incr=True)
-    elif engine == &#34;lingeling&#34;:
-        solver = Lingeling(bootstrap_with=formula)
-    else:
-        raise ValueError(f&#34;unsupported solver: {engine}&#34;)
+    if not solver_args:
+        solver_args = {}
+    solver = solver_cls(bootstrap_with=formula, **solver_args)
     return solver, variables</code></pre>
 </details>
 </dd>
 <dt id="circuitgraph.sat.model_count"><code class="name flex">
 <span>def <span class="ident">model_count</span></span>(<span>c, assumptions=None)</span>
 </code></dt>
 <dd>
@@ -1017,8 +1055,8 @@
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc"><cite>pdoc</cite> 0.10.0</a>.</p>
 </footer>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -73,56 +73,65 @@
 def remap(clauses, offset):
     """Remap clauses of a formula."""
     new_clauses = [[v + offset if v > 0 else v - offset for v in c] for c in
 clauses]
     return new_clauses
 
 
-def construct_solver(c, assumptions=None, engine="cadical"):
+def construct_solver(c, assumptions=None, solver_cls=None, solver_args=None):
     """
     Construct a SAT solver instance with the given circuit and assumptions.
 
     Parameters
     ----------
     c : Circuit
             Circuit to encode.
     assumptions : dict of str:int
             Assumptions to add to solver.
+    solver_cls : pysat.Solver
+            The class of solver to use. If None, `Cadical` is used.
+    solver_args : dict of str:Any
+            Arguments to pass into the solver constructor. For `Glucose`
+            solvers, this should include `'incr': True` to set incremental
+            mode.
 
     Returns
     -------
-    solver : pysat.Cadical
+    solver : pysat.Solver
             SAT solver instance.
     variables : pysat.IDPool
             Solver variable mapping.
 
     """
-    try:
-        from pysat.solvers import Cadical, Glucose4, Lingeling
-    except ImportError as e:
-        raise ImportError(
-            "Install 'python-sat' to use satisfiability functionality"
-        ) from e
+    if not solver_cls:
+        try:
+            from pysat.solvers import Cadical153
+
+            solver_cls = Cadical153
+        except ImportError:
+            try:
+                from pysat.solvers import Cadical
+
+                solver_cls = Cadical
+            except ImportError as e:
+                raise ImportError(
+                    "Install 'python-sat' to use satisfiability functionality"
+                ) from e
 
     formula, variables = cnf(c)
     if assumptions:
         for n in assumptions.keys():
             if n not in c:
                 raise ValueError(f"Node '{n}' in assumptions is not in
 circuit")
         add_assumptions(formula, variables, assumptions)
 
-    if engine == "cadical":
-        solver = Cadical(bootstrap_with=formula)
-    elif engine == "glucose":
-        solver = Glucose4(bootstrap_with=formula, incr=True)
-    elif engine == "lingeling":
-        solver = Lingeling(bootstrap_with=formula)
-    else:
-        raise ValueError(f"unsupported solver: {engine}")
+    if not solver_args:
+        solver_args = {}
+    solver = solver_cls(bootstrap_with=formula, **solver_args)
     return solver, variables
 
 
 def cnf(c):
     """
     Convert circuit to CNF using the Tseitin transformation.
 
@@ -409,15 +418,22 @@
             cmd.append(f"--seed={seed}")
         if not detach_xor:
             cmd.append("--detachxor=0")
         cmd.append(tmp.name)
         with open(log_file, "w+") if log_file else tempfile.NamedTemporaryFile(
             prefix=f"circuitgraph_approxmc_{c.name}_log", mode="w+"
         ) as f:
-            subprocess.run(cmd, stdout=f, stderr=f, check=True, text=True)
+            subprocess.run(
+                cmd,
+                stdout=f,
+                stderr=f,
+                check=True,
+                encoding="utf8",
+                universal_newlines=True,
+            )
             f.seek(0)
             result = f.read()
 
     # parse results
     m = re.search(r"s mc (\d+)", result)
     if not m:
         raise ValueError(f"approxmc produced unexpected result:\n\n{result}")
@@ -633,16 +649,22 @@
               if not detach_xor:
                   cmd.append("--detachxor=0")
               cmd.append(tmp.name)
               with open(log_file, "w+") if log_file else
       tempfile.NamedTemporaryFile(
                   prefix=f"circuitgraph_approxmc_{c.name}_log", mode="w+"
               ) as f:
-                  subprocess.run(cmd, stdout=f, stderr=f, check=True,
-      text=True)
+                  subprocess.run(
+                      cmd,
+                      stdout=f,
+                      stderr=f,
+                      check=True,
+                      encoding="utf8",
+                      universal_newlines=True,
+                  )
                   f.seek(0)
                   result = f.read()
 
           # parse results
           m = re.search(r"s mc (\d+)", result)
           if not m:
               raise ValueError(f"approxmc produced unexpected result:\n\n
@@ -769,70 +791,87 @@
                   formula.append([variables.id(n)])
               elif n_type in ["bb_output", "input"]:
                   formula.append([variables.id(n), -variables.id(n)])
               else:
                   raise ValueError(f"Unknown gate type '{n_type}'")
 
           return formula, variables
-  def construct_solver(c, assumptions=None, engine='cadical')
+  def construct_solver(c, assumptions=None, solver_cls=None, solver_args=None)
       Construct a SAT solver instance with the given circuit and assumptions.
       ***** Parameters *****
         c :&ensp;Circuit
             Circuit to encode.
         assumptions :&ensp;dict of str:int
             Assumptions to add to solver.
+        solver_cls :&ensp;pysat.Solver
+            The class of solver to use. If None, Cadical is used.
+        solver_args :&ensp;dict of str:Any
+            Arguments to pass into the solver constructor. For Glucose solvers,
+            this should include 'incr': True to set incremental mode.
       ***** Returns *****
-        solver :&ensp;pysat.Cadical
+        solver :&ensp;pysat.Solver
             SAT solver instance.
         variables :&ensp;pysat.IDPool
             Solver variable mapping.
         Expand source code
-      def construct_solver(c, assumptions=None, engine="cadical"):
+      def construct_solver(c, assumptions=None, solver_cls=None,
+      solver_args=None):
           """
           Construct a SAT solver instance with the given circuit and
       assumptions.
 
           Parameters
           ----------
           c : Circuit
                   Circuit to encode.
           assumptions : dict of str:int
                   Assumptions to add to solver.
+          solver_cls : pysat.Solver
+                  The class of solver to use. If None, `Cadical` is used.
+          solver_args : dict of str:Any
+                  Arguments to pass into the solver constructor. For `Glucose`
+                  solvers, this should include `'incr': True` to set
+      incremental
+                  mode.
 
           Returns
           -------
-          solver : pysat.Cadical
+          solver : pysat.Solver
                   SAT solver instance.
           variables : pysat.IDPool
                   Solver variable mapping.
 
           """
-          try:
-              from pysat.solvers import Cadical, Glucose4, Lingeling
-          except ImportError as e:
-              raise ImportError(
-                  "Install 'python-sat' to use satisfiability functionality"
-              ) from e
+          if not solver_cls:
+              try:
+                  from pysat.solvers import Cadical153
+
+                  solver_cls = Cadical153
+              except ImportError:
+                  try:
+                      from pysat.solvers import Cadical
+
+                      solver_cls = Cadical
+                  except ImportError as e:
+                      raise ImportError(
+                          "Install 'python-sat' to use satisfiability
+      functionality"
+                      ) from e
 
           formula, variables = cnf(c)
           if assumptions:
               for n in assumptions.keys():
                   if n not in c:
                       raise ValueError(f"Node '{n}' in assumptions is not in
       circuit")
               add_assumptions(formula, variables, assumptions)
 
-          if engine == "cadical":
-              solver = Cadical(bootstrap_with=formula)
-          elif engine == "glucose":
-              solver = Glucose4(bootstrap_with=formula, incr=True)
-          elif engine == "lingeling":
-              solver = Lingeling(bootstrap_with=formula)
-          else:
-              raise ValueError(f"unsupported solver: {engine}")
+          if not solver_args:
+              solver_args = {}
+          solver = solver_cls(bootstrap_with=formula, **solver_args)
           return solver, variables
   def model_count(c, assumptions=None)
       Determine the number of solutions to circuit.
       ***** Parameters *****
         c :&ensp;Circuit
             Input circuit.
         assumptions :&ensp;dict of str:int
```

### Comparing `circuitgraph-0.2.0/docs/transform.html` & `circuitgraph-0.2.1/docs/transform.html`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/docs/tx.html` & `circuitgraph-0.2.1/docs/tx.html`

 * *Files 3% similar despite different names*

```diff
@@ -436,14 +436,49 @@
                     replace_gate,
                     output_netlist,
                 )
 
     return cg.io.verilog_to_circuit(output_netlist, c.name, fast=fast_parsing)
 
 
+def aig(c):
+    &#34;&#34;&#34;
+    Transform a circuit into and and-inverter graph.
+
+    Parameters
+    ----------
+    c: Circuit
+            The circuit to transform to an AIG.
+
+    Returns
+    -------
+    Circuit
+            The AIG circuit.
+
+    &#34;&#34;&#34;
+    with NamedTemporaryFile(
+        prefix=&#34;circuitgraph_aig_input&#34;, suffix=&#34;.v&#34;, mode=&#34;w&#34;
+    ) as tmp_in:
+        cg.to_file(c, tmp_in.name)
+        with NamedTemporaryFile(
+            prefix=&#34;circuitgraph_aig_output&#34;, suffix=&#34;.v&#34;, mode=&#34;r&#34;
+        ) as tmp_out:
+            execute = (
+                f&#34;read_verilog {tmp_in.name}; aigmap; &#34;
+                &#34;opt; &#34;
+                f&#34;write_verilog -noattr {tmp_out.name}&#34;
+            )
+            subprocess.run(
+                [&#34;yosys&#34;, &#34;-p&#34;, execute], stdout=subprocess.DEVNULL, check=True
+            )
+            c = cg.from_file(tmp_out.name)
+    # c = remove_bufs(c)
+    return c
+
+
 def ternary(c):
     &#34;&#34;&#34;
     Encode the circuit with ternary values.
 
     The ternary circuit adds a second net for each net in the original circuit.
     The second net encodes a don&#39;t care, or X, value. That net being high
     corresponds to a don&#39;t care value on original net. If the second net is
@@ -521,15 +556,15 @@
                 add_connected_nodes=True,
                 allow_redefinition=True,
             )
         elif c.type(n) in [&#34;xor&#34;, &#34;xnor&#34;]:
             t.add(
                 mapping[n],
                 &#34;or&#34;,
-                fanin=(mapping[p] for p in c.fanin(n)),
+                fanin=[mapping[p] for p in c.fanin(n)],
                 output=c.is_output(n),
                 add_connected_nodes=True,
                 allow_redefinition=True,
             )
         elif c.type(n) in [&#34;0&#34;, &#34;1&#34;]:
             t.add(mapping[n], &#34;0&#34;, output=c.is_output(n), allow_redefinition=True)
         elif c.type(n) in [&#34;input&#34;]:
@@ -881,24 +916,24 @@
     Reduce the maximum fanin of circuit gates to k.
 
     Parameters
     ----------
     c : Circuit
             Input circuit.
     k : str
-            Maximum fanin. (k &gt; 2)
+            Maximum fanin. (k &gt;= 2)
 
     Returns
     -------
     Circuit
             Output circuit.
 
     &#34;&#34;&#34;
     if k &lt; 2:
-        raise ValueError(&#34;maximum fanin, k, must be &gt; 2&#34;)
+        raise ValueError(f&#34;&#39;k&#39; must be &gt;= 2, not &#39;{k}&#39;&#34;)
 
     gatemap = {
         &#34;and&#34;: &#34;and&#34;,
         &#34;nand&#34;: &#34;and&#34;,
         &#34;or&#34;: &#34;or&#34;,
         &#34;nor&#34;: &#34;or&#34;,
         &#34;xor&#34;: &#34;xor&#34;,
@@ -921,14 +956,54 @@
                 uid=True,
             )
             i += 1
 
     return ck
 
 
+def limit_fanout(c, k):
+    &#34;&#34;&#34;
+    Reduce the maximum fanout of circuit gates to k.
+
+    Parameters
+    ----------
+    c : Circuit
+            Input circuit.
+    k : str
+            Maximum fanout. (k &gt;= 2)
+
+    Returns
+    -------
+    Circuit
+            Output circuit.
+
+    &#34;&#34;&#34;
+    if k &lt; 2:
+        raise ValueError(f&#34;&#39;k&#39; must be &gt;= 2, not &#39;{k}&#39;&#34;)
+
+    ck = c.copy()
+    for n in ck.nodes():
+        i = 0
+        while len(ck.fanout(n)) &gt; k:
+            fo = ck.fanout(n)
+            f0 = fo.pop()
+            f1 = fo.pop()
+            ck.disconnect(n, [f0, f1])
+            ck.add(
+                f&#34;{n}_limit_fanout_{i}&#34;,
+                &#34;buf&#34;,
+                fanin=n,
+                fanout=[f0, f1],
+                uid=True,
+            )
+            i += 1
+
+    return ck
+
+
 def acyclic_unroll(c):
     &#34;&#34;&#34;
     Unroll a cyclic circuit to remove cycles.
 
     Parameters
     ----------
     c: Circuit
@@ -1150,15 +1225,80 @@
                 other_supergate = minimal_supergate_circuits[other_output]
                 if i in other_supergate.nodes() - other_supergate.inputs():
                     g.add_edge(other_output, output)
 
     sorted_supergate_circuits = []
     for node in nx.topological_sort(g):
         sorted_supergate_circuits.append(minimal_supergate_circuits[node])
-    return sorted_supergate_circuits</code></pre>
+    return sorted_supergate_circuits
+
+
+def insert_registers(
+    c,
+    num_stages,
+    ff=cg.generic_flop,
+    d_port=&#34;d&#34;,
+    q_port=&#34;q&#34;,
+    other_flop_io={&#34;clk&#34;: &#34;clk&#34;},
+    q_suffix=&#34;_cg_insert_reg_q_&#34;,
+):
+    &#34;&#34;&#34;
+    Insert pipeline registers into a combinational design.
+
+    Parameters
+    ----------
+    c: circuitgraph.Circuit
+            The circuit to insert registers into.
+    num_stages: int
+            The number of stages to add.
+    ff: circuitgraph.BlackBox
+            The flip flop blackbox to use.
+    d_port: str
+            The d port on the flip flop blackbox.
+    q_port: str
+            The q port on the flip flop blackbox.
+    other_flop_io: dict of str:str
+            Other io to connect on the flop (e.g. clk, rst ports).
+            Dict maps circuit nodes to flop ports. If a node is
+            present in the dict but not in the circuit, it will be
+            added as an input.
+    q_suffix: str
+            Inserted q nodes are named with the suffix `{q_suffix}{i}` where
+            `i` is the level the flop is inserted at.
+
+    Returns
+    -------
+    circuitgraph.Circuit
+            The circuit with added registers.
+
+    &#34;&#34;&#34;
+    c_reg = c.copy()
+    nodes_at_depths = []
+    max_depth = 0
+    for n in c_reg:
+        depth = c_reg.fanin_depth(n)
+        while depth &gt;= len(nodes_at_depths):
+            nodes_at_depths.append([])
+        nodes_at_depths[depth].append(n)
+        if depth &gt; max_depth:
+            max_depth = depth
+
+    depth_inc = round(max_depth / (num_stages + 1))
+    for n in other_flop_io:
+        if n not in c_reg:
+            c_reg.add(n, &#34;input&#34;)
+    for i in range(depth_inc, max_depth, depth_inc):
+        for n in nodes_at_depths[i]:
+            fanout = c_reg.fanout(n)
+            c_reg.disconnect(n, fanout)
+            q = c_reg.add(f&#34;{n}{q_suffix}{i}&#34;, &#34;buf&#34;, uid=True, fanout=fanout)
+            conns = {d_port: n, q_port: q}
+            conns.update(other_flop_io)
+            c_reg.add_blackbox(ff, f&#34;ff_{n}&#34;, conns)
+    return c_reg</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
@@ -1285,25 +1425,179 @@
 
     cg.lint(acyc)
     if acyc.is_cyclic():
         raise ValueError(&#34;Circuit still cyclic&#34;)
     return acyc</code></pre>
 </details>
 </dd>
+<dt id="circuitgraph.tx.aig"><code class="name flex">
+<span>def <span class="ident">aig</span></span>(<span>c)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Transform a circuit into and and-inverter graph.</p>
+<h2 id="parameters">Parameters</h2>
+<dl>
+<dt><strong><code>c</code></strong> :&ensp;<code>Circuit</code></dt>
+<dd>The circuit to transform to an AIG.</dd>
+</dl>
+<h2 id="returns">Returns</h2>
+<dl>
+<dt><code>Circuit</code></dt>
+<dd>The AIG circuit.</dd>
+</dl></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def aig(c):
+    &#34;&#34;&#34;
+    Transform a circuit into and and-inverter graph.
+
+    Parameters
+    ----------
+    c: Circuit
+            The circuit to transform to an AIG.
+
+    Returns
+    -------
+    Circuit
+            The AIG circuit.
+
+    &#34;&#34;&#34;
+    with NamedTemporaryFile(
+        prefix=&#34;circuitgraph_aig_input&#34;, suffix=&#34;.v&#34;, mode=&#34;w&#34;
+    ) as tmp_in:
+        cg.to_file(c, tmp_in.name)
+        with NamedTemporaryFile(
+            prefix=&#34;circuitgraph_aig_output&#34;, suffix=&#34;.v&#34;, mode=&#34;r&#34;
+        ) as tmp_out:
+            execute = (
+                f&#34;read_verilog {tmp_in.name}; aigmap; &#34;
+                &#34;opt; &#34;
+                f&#34;write_verilog -noattr {tmp_out.name}&#34;
+            )
+            subprocess.run(
+                [&#34;yosys&#34;, &#34;-p&#34;, execute], stdout=subprocess.DEVNULL, check=True
+            )
+            c = cg.from_file(tmp_out.name)
+    # c = remove_bufs(c)
+    return c</code></pre>
+</details>
+</dd>
+<dt id="circuitgraph.tx.insert_registers"><code class="name flex">
+<span>def <span class="ident">insert_registers</span></span>(<span>c, num_stages, ff=&lt;circuitgraph.circuit.BlackBox object&gt;, d_port='d', q_port='q', other_flop_io={'clk': 'clk'}, q_suffix='_cg_insert_reg_q_')</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Insert pipeline registers into a combinational design.</p>
+<h2 id="parameters">Parameters</h2>
+<dl>
+<dt><strong><code>c</code></strong> :&ensp;<code>circuitgraph.Circuit</code></dt>
+<dd>The circuit to insert registers into.</dd>
+<dt><strong><code>num_stages</code></strong> :&ensp;<code>int</code></dt>
+<dd>The number of stages to add.</dd>
+<dt><strong><code>ff</code></strong> :&ensp;<code>circuitgraph.BlackBox</code></dt>
+<dd>The flip flop blackbox to use.</dd>
+<dt><strong><code>d_port</code></strong> :&ensp;<code>str</code></dt>
+<dd>The d port on the flip flop blackbox.</dd>
+<dt><strong><code>q_port</code></strong> :&ensp;<code>str</code></dt>
+<dd>The q port on the flip flop blackbox.</dd>
+<dt><strong><code>other_flop_io</code></strong> :&ensp;<code>dict</code> of <code>str:str</code></dt>
+<dd>Other io to connect on the flop (e.g. clk, rst ports).
+Dict maps circuit nodes to flop ports. If a node is
+present in the dict but not in the circuit, it will be
+added as an input.</dd>
+<dt><strong><code>q_suffix</code></strong> :&ensp;<code>str</code></dt>
+<dd>Inserted q nodes are named with the suffix <code>{q_suffix}{i}</code> where
+<code>i</code> is the level the flop is inserted at.</dd>
+</dl>
+<h2 id="returns">Returns</h2>
+<dl>
+<dt><code>circuitgraph.Circuit</code></dt>
+<dd>The circuit with added registers.</dd>
+</dl></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def insert_registers(
+    c,
+    num_stages,
+    ff=cg.generic_flop,
+    d_port=&#34;d&#34;,
+    q_port=&#34;q&#34;,
+    other_flop_io={&#34;clk&#34;: &#34;clk&#34;},
+    q_suffix=&#34;_cg_insert_reg_q_&#34;,
+):
+    &#34;&#34;&#34;
+    Insert pipeline registers into a combinational design.
+
+    Parameters
+    ----------
+    c: circuitgraph.Circuit
+            The circuit to insert registers into.
+    num_stages: int
+            The number of stages to add.
+    ff: circuitgraph.BlackBox
+            The flip flop blackbox to use.
+    d_port: str
+            The d port on the flip flop blackbox.
+    q_port: str
+            The q port on the flip flop blackbox.
+    other_flop_io: dict of str:str
+            Other io to connect on the flop (e.g. clk, rst ports).
+            Dict maps circuit nodes to flop ports. If a node is
+            present in the dict but not in the circuit, it will be
+            added as an input.
+    q_suffix: str
+            Inserted q nodes are named with the suffix `{q_suffix}{i}` where
+            `i` is the level the flop is inserted at.
+
+    Returns
+    -------
+    circuitgraph.Circuit
+            The circuit with added registers.
+
+    &#34;&#34;&#34;
+    c_reg = c.copy()
+    nodes_at_depths = []
+    max_depth = 0
+    for n in c_reg:
+        depth = c_reg.fanin_depth(n)
+        while depth &gt;= len(nodes_at_depths):
+            nodes_at_depths.append([])
+        nodes_at_depths[depth].append(n)
+        if depth &gt; max_depth:
+            max_depth = depth
+
+    depth_inc = round(max_depth / (num_stages + 1))
+    for n in other_flop_io:
+        if n not in c_reg:
+            c_reg.add(n, &#34;input&#34;)
+    for i in range(depth_inc, max_depth, depth_inc):
+        for n in nodes_at_depths[i]:
+            fanout = c_reg.fanout(n)
+            c_reg.disconnect(n, fanout)
+            q = c_reg.add(f&#34;{n}{q_suffix}{i}&#34;, &#34;buf&#34;, uid=True, fanout=fanout)
+            conns = {d_port: n, q_port: q}
+            conns.update(other_flop_io)
+            c_reg.add_blackbox(ff, f&#34;ff_{n}&#34;, conns)
+    return c_reg</code></pre>
+</details>
+</dd>
 <dt id="circuitgraph.tx.limit_fanin"><code class="name flex">
 <span>def <span class="ident">limit_fanin</span></span>(<span>c, k)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Reduce the maximum fanin of circuit gates to k.</p>
 <h2 id="parameters">Parameters</h2>
 <dl>
 <dt><strong><code>c</code></strong> :&ensp;<code>Circuit</code></dt>
 <dd>Input circuit.</dd>
 <dt><strong><code>k</code></strong> :&ensp;<code>str</code></dt>
-<dd>Maximum fanin. (k &gt; 2)</dd>
+<dd>Maximum fanin. (k &gt;= 2)</dd>
 </dl>
 <h2 id="returns">Returns</h2>
 <dl>
 <dt><code>Circuit</code></dt>
 <dd>Output circuit.</dd>
 </dl></div>
 <details class="source">
@@ -1315,24 +1609,24 @@
     Reduce the maximum fanin of circuit gates to k.
 
     Parameters
     ----------
     c : Circuit
             Input circuit.
     k : str
-            Maximum fanin. (k &gt; 2)
+            Maximum fanin. (k &gt;= 2)
 
     Returns
     -------
     Circuit
             Output circuit.
 
     &#34;&#34;&#34;
     if k &lt; 2:
-        raise ValueError(&#34;maximum fanin, k, must be &gt; 2&#34;)
+        raise ValueError(f&#34;&#39;k&#39; must be &gt;= 2, not &#39;{k}&#39;&#34;)
 
     gatemap = {
         &#34;and&#34;: &#34;and&#34;,
         &#34;nand&#34;: &#34;and&#34;,
         &#34;or&#34;: &#34;or&#34;,
         &#34;nor&#34;: &#34;or&#34;,
         &#34;xor&#34;: &#34;xor&#34;,
@@ -1355,14 +1649,75 @@
                 uid=True,
             )
             i += 1
 
     return ck</code></pre>
 </details>
 </dd>
+<dt id="circuitgraph.tx.limit_fanout"><code class="name flex">
+<span>def <span class="ident">limit_fanout</span></span>(<span>c, k)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Reduce the maximum fanout of circuit gates to k.</p>
+<h2 id="parameters">Parameters</h2>
+<dl>
+<dt><strong><code>c</code></strong> :&ensp;<code>Circuit</code></dt>
+<dd>Input circuit.</dd>
+<dt><strong><code>k</code></strong> :&ensp;<code>str</code></dt>
+<dd>Maximum fanout. (k &gt;= 2)</dd>
+</dl>
+<h2 id="returns">Returns</h2>
+<dl>
+<dt><code>Circuit</code></dt>
+<dd>Output circuit.</dd>
+</dl></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def limit_fanout(c, k):
+    &#34;&#34;&#34;
+    Reduce the maximum fanout of circuit gates to k.
+
+    Parameters
+    ----------
+    c : Circuit
+            Input circuit.
+    k : str
+            Maximum fanout. (k &gt;= 2)
+
+    Returns
+    -------
+    Circuit
+            Output circuit.
+
+    &#34;&#34;&#34;
+    if k &lt; 2:
+        raise ValueError(f&#34;&#39;k&#39; must be &gt;= 2, not &#39;{k}&#39;&#34;)
+
+    ck = c.copy()
+    for n in ck.nodes():
+        i = 0
+        while len(ck.fanout(n)) &gt; k:
+            fo = ck.fanout(n)
+            f0 = fo.pop()
+            f1 = fo.pop()
+            ck.disconnect(n, [f0, f1])
+            ck.add(
+                f&#34;{n}_limit_fanout_{i}&#34;,
+                &#34;buf&#34;,
+                fanin=n,
+                fanout=[f0, f1],
+                uid=True,
+            )
+            i += 1
+
+    return ck</code></pre>
+</details>
+</dd>
 <dt id="circuitgraph.tx.miter"><code class="name flex">
 <span>def <span class="ident">miter</span></span>(<span>c0, c1=None, startpoints=None, endpoints=None)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Create a miter circuit.</p>
 <h2 id="parameters">Parameters</h2>
 <dl>
@@ -2562,15 +2917,15 @@
                 add_connected_nodes=True,
                 allow_redefinition=True,
             )
         elif c.type(n) in [&#34;xor&#34;, &#34;xnor&#34;]:
             t.add(
                 mapping[n],
                 &#34;or&#34;,
-                fanin=(mapping[p] for p in c.fanin(n)),
+                fanin=[mapping[p] for p in c.fanin(n)],
                 output=c.is_output(n),
                 add_connected_nodes=True,
                 allow_redefinition=True,
             )
         elif c.type(n) in [&#34;0&#34;, &#34;1&#34;]:
             t.add(mapping[n], &#34;0&#34;, output=c.is_output(n), allow_redefinition=True)
         elif c.type(n) in [&#34;input&#34;]:
@@ -2698,15 +3053,18 @@
 <ul>
 <li><code><a title="circuitgraph" href="index.html">circuitgraph</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-functions">Functions</a></h3>
 <ul class="">
 <li><code><a title="circuitgraph.tx.acyclic_unroll" href="#circuitgraph.tx.acyclic_unroll">acyclic_unroll</a></code></li>
+<li><code><a title="circuitgraph.tx.aig" href="#circuitgraph.tx.aig">aig</a></code></li>
+<li><code><a title="circuitgraph.tx.insert_registers" href="#circuitgraph.tx.insert_registers">insert_registers</a></code></li>
 <li><code><a title="circuitgraph.tx.limit_fanin" href="#circuitgraph.tx.limit_fanin">limit_fanin</a></code></li>
+<li><code><a title="circuitgraph.tx.limit_fanout" href="#circuitgraph.tx.limit_fanout">limit_fanout</a></code></li>
 <li><code><a title="circuitgraph.tx.miter" href="#circuitgraph.tx.miter">miter</a></code></li>
 <li><code><a title="circuitgraph.tx.relabel" href="#circuitgraph.tx.relabel">relabel</a></code></li>
 <li><code><a title="circuitgraph.tx.sensitivity_transform" href="#circuitgraph.tx.sensitivity_transform">sensitivity_transform</a></code></li>
 <li><code><a title="circuitgraph.tx.sensitization_transform" href="#circuitgraph.tx.sensitization_transform">sensitization_transform</a></code></li>
 <li><code><a title="circuitgraph.tx.sequential_unroll" href="#circuitgraph.tx.sequential_unroll">sequential_unroll</a></code></li>
 <li><code><a title="circuitgraph.tx.strip_blackboxes" href="#circuitgraph.tx.strip_blackboxes">strip_blackboxes</a></code></li>
 <li><code><a title="circuitgraph.tx.strip_inputs" href="#circuitgraph.tx.strip_inputs">strip_inputs</a></code></li>
@@ -2722,8 +3080,8 @@
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc"><cite>pdoc</cite> 0.10.0</a>.</p>
 </footer>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -424,14 +424,49 @@
                     replace_gate,
                     output_netlist,
                 )
 
     return cg.io.verilog_to_circuit(output_netlist, c.name, fast=fast_parsing)
 
 
+def aig(c):
+    """
+    Transform a circuit into and and-inverter graph.
+
+    Parameters
+    ----------
+    c: Circuit
+            The circuit to transform to an AIG.
+
+    Returns
+    -------
+    Circuit
+            The AIG circuit.
+
+    """
+    with NamedTemporaryFile(
+        prefix="circuitgraph_aig_input", suffix=".v", mode="w"
+    ) as tmp_in:
+        cg.to_file(c, tmp_in.name)
+        with NamedTemporaryFile(
+            prefix="circuitgraph_aig_output", suffix=".v", mode="r"
+        ) as tmp_out:
+            execute = (
+                f"read_verilog {tmp_in.name}; aigmap; "
+                "opt; "
+                f"write_verilog -noattr {tmp_out.name}"
+            )
+            subprocess.run(
+                ["yosys", "-p", execute], stdout=subprocess.DEVNULL, check=True
+            )
+            c = cg.from_file(tmp_out.name)
+    # c = remove_bufs(c)
+    return c
+
+
 def ternary(c):
     """
     Encode the circuit with ternary values.
 
     The ternary circuit adds a second net for each net in the original circuit.
     The second net encodes a don't care, or X, value. That net being high
     corresponds to a don't care value on original net. If the second net is
@@ -513,15 +548,15 @@
                 add_connected_nodes=True,
                 allow_redefinition=True,
             )
         elif c.type(n) in ["xor", "xnor"]:
             t.add(
                 mapping[n],
                 "or",
-                fanin=(mapping[p] for p in c.fanin(n)),
+                fanin=[mapping[p] for p in c.fanin(n)],
                 output=c.is_output(n),
                 add_connected_nodes=True,
                 allow_redefinition=True,
             )
         elif c.type(n) in ["0", "1"]:
             t.add(mapping[n], "0", output=c.is_output(n),
 allow_redefinition=True)
@@ -884,24 +919,24 @@
     Reduce the maximum fanin of circuit gates to k.
 
     Parameters
     ----------
     c : Circuit
             Input circuit.
     k : str
-            Maximum fanin. (k > 2)
+            Maximum fanin. (k >= 2)
 
     Returns
     -------
     Circuit
             Output circuit.
 
     """
     if k < 2:
-        raise ValueError("maximum fanin, k, must be > 2")
+        raise ValueError(f"'k' must be >= 2, not '{k}'")
 
     gatemap = {
         "and": "and",
         "nand": "and",
         "or": "or",
         "nor": "or",
         "xor": "xor",
@@ -924,14 +959,54 @@
                 uid=True,
             )
             i += 1
 
     return ck
 
 
+def limit_fanout(c, k):
+    """
+    Reduce the maximum fanout of circuit gates to k.
+
+    Parameters
+    ----------
+    c : Circuit
+            Input circuit.
+    k : str
+            Maximum fanout. (k >= 2)
+
+    Returns
+    -------
+    Circuit
+            Output circuit.
+
+    """
+    if k < 2:
+        raise ValueError(f"'k' must be >= 2, not '{k}'")
+
+    ck = c.copy()
+    for n in ck.nodes():
+        i = 0
+        while len(ck.fanout(n)) > k:
+            fo = ck.fanout(n)
+            f0 = fo.pop()
+            f1 = fo.pop()
+            ck.disconnect(n, [f0, f1])
+            ck.add(
+                f"{n}_limit_fanout_{i}",
+                "buf",
+                fanin=n,
+                fanout=[f0, f1],
+                uid=True,
+            )
+            i += 1
+
+    return ck
+
+
 def acyclic_unroll(c):
     """
     Unroll a cyclic circuit to remove cycles.
 
     Parameters
     ----------
     c: Circuit
@@ -1159,14 +1234,79 @@
                     g.add_edge(other_output, output)
 
     sorted_supergate_circuits = []
     for node in nx.topological_sort(g):
         sorted_supergate_circuits.append(minimal_supergate_circuits[node])
     return sorted_supergate_circuits
 
+
+def insert_registers(
+    c,
+    num_stages,
+    ff=cg.generic_flop,
+    d_port="d",
+    q_port="q",
+    other_flop_io={"clk": "clk"},
+    q_suffix="_cg_insert_reg_q_",
+):
+    """
+    Insert pipeline registers into a combinational design.
+
+    Parameters
+    ----------
+    c: circuitgraph.Circuit
+            The circuit to insert registers into.
+    num_stages: int
+            The number of stages to add.
+    ff: circuitgraph.BlackBox
+            The flip flop blackbox to use.
+    d_port: str
+            The d port on the flip flop blackbox.
+    q_port: str
+            The q port on the flip flop blackbox.
+    other_flop_io: dict of str:str
+            Other io to connect on the flop (e.g. clk, rst ports).
+            Dict maps circuit nodes to flop ports. If a node is
+            present in the dict but not in the circuit, it will be
+            added as an input.
+    q_suffix: str
+            Inserted q nodes are named with the suffix `{q_suffix}{i}` where
+            `i` is the level the flop is inserted at.
+
+    Returns
+    -------
+    circuitgraph.Circuit
+            The circuit with added registers.
+
+    """
+    c_reg = c.copy()
+    nodes_at_depths = []
+    max_depth = 0
+    for n in c_reg:
+        depth = c_reg.fanin_depth(n)
+        while depth >= len(nodes_at_depths):
+            nodes_at_depths.append([])
+        nodes_at_depths[depth].append(n)
+        if depth > max_depth:
+            max_depth = depth
+
+    depth_inc = round(max_depth / (num_stages + 1))
+    for n in other_flop_io:
+        if n not in c_reg:
+            c_reg.add(n, "input")
+    for i in range(depth_inc, max_depth, depth_inc):
+        for n in nodes_at_depths[i]:
+            fanout = c_reg.fanout(n)
+            c_reg.disconnect(n, fanout)
+            q = c_reg.add(f"{n}{q_suffix}{i}", "buf", uid=True, fanout=fanout)
+            conns = {d_port: n, q_port: q}
+            conns.update(other_flop_io)
+            c_reg.add_blackbox(ff, f"ff_{n}", conns)
+    return c_reg
+
 ***** Functions *****
   def acyclic_unroll(c)
       Unroll a cyclic circuit to remove cycles.
       ***** Parameters *****
         c :&ensp;Circuit
             Circuit to unroll.
       ***** Returns *****
@@ -1280,44 +1420,178 @@
           for o in c.outputs():
               acyc.add(o, "buf", fanin=f"c{i}_{o}", output=True)
 
           cg.lint(acyc)
           if acyc.is_cyclic():
               raise ValueError("Circuit still cyclic")
           return acyc
+  def aig(c)
+      Transform a circuit into and and-inverter graph.
+      ***** Parameters *****
+        c :&ensp;Circuit
+            The circuit to transform to an AIG.
+      ***** Returns *****
+        Circuit
+            The AIG circuit.
+        Expand source code
+      def aig(c):
+          """
+          Transform a circuit into and and-inverter graph.
+
+          Parameters
+          ----------
+          c: Circuit
+                  The circuit to transform to an AIG.
+
+          Returns
+          -------
+          Circuit
+                  The AIG circuit.
+
+          """
+          with NamedTemporaryFile(
+              prefix="circuitgraph_aig_input", suffix=".v", mode="w"
+          ) as tmp_in:
+              cg.to_file(c, tmp_in.name)
+              with NamedTemporaryFile(
+                  prefix="circuitgraph_aig_output", suffix=".v", mode="r"
+              ) as tmp_out:
+                  execute = (
+                      f"read_verilog {tmp_in.name}; aigmap; "
+                      "opt; "
+                      f"write_verilog -noattr {tmp_out.name}"
+                  )
+                  subprocess.run(
+                      ["yosys", "-p", execute], stdout=subprocess.DEVNULL,
+      check=True
+                  )
+                  c = cg.from_file(tmp_out.name)
+          # c = remove_bufs(c)
+          return c
+  def insert_registers(c, num_stages, ff=<circuitgraph.circuit.BlackBox
+  object>, d_port='d', q_port='q', other_flop_io={'clk': 'clk'},
+  q_suffix='_cg_insert_reg_q_')
+      Insert pipeline registers into a combinational design.
+      ***** Parameters *****
+        c :&ensp;circuitgraph.Circuit
+            The circuit to insert registers into.
+        num_stages :&ensp;int
+            The number of stages to add.
+        ff :&ensp;circuitgraph.BlackBox
+            The flip flop blackbox to use.
+        d_port :&ensp;str
+            The d port on the flip flop blackbox.
+        q_port :&ensp;str
+            The q port on the flip flop blackbox.
+        other_flop_io :&ensp;dict of str:str
+            Other io to connect on the flop (e.g. clk, rst ports). Dict maps
+            circuit nodes to flop ports. If a node is present in the dict but
+            not in the circuit, it will be added as an input.
+        q_suffix :&ensp;str
+            Inserted q nodes are named with the suffix {q_suffix}{i} where i is
+            the level the flop is inserted at.
+      ***** Returns *****
+        circuitgraph.Circuit
+            The circuit with added registers.
+        Expand source code
+      def insert_registers(
+          c,
+          num_stages,
+          ff=cg.generic_flop,
+          d_port="d",
+          q_port="q",
+          other_flop_io={"clk": "clk"},
+          q_suffix="_cg_insert_reg_q_",
+      ):
+          """
+          Insert pipeline registers into a combinational design.
+
+          Parameters
+          ----------
+          c: circuitgraph.Circuit
+                  The circuit to insert registers into.
+          num_stages: int
+                  The number of stages to add.
+          ff: circuitgraph.BlackBox
+                  The flip flop blackbox to use.
+          d_port: str
+                  The d port on the flip flop blackbox.
+          q_port: str
+                  The q port on the flip flop blackbox.
+          other_flop_io: dict of str:str
+                  Other io to connect on the flop (e.g. clk, rst ports).
+                  Dict maps circuit nodes to flop ports. If a node is
+                  present in the dict but not in the circuit, it will be
+                  added as an input.
+          q_suffix: str
+                  Inserted q nodes are named with the suffix `{q_suffix}{i}`
+      where
+                  `i` is the level the flop is inserted at.
+
+          Returns
+          -------
+          circuitgraph.Circuit
+                  The circuit with added registers.
+
+          """
+          c_reg = c.copy()
+          nodes_at_depths = []
+          max_depth = 0
+          for n in c_reg:
+              depth = c_reg.fanin_depth(n)
+              while depth >= len(nodes_at_depths):
+                  nodes_at_depths.append([])
+              nodes_at_depths[depth].append(n)
+              if depth > max_depth:
+                  max_depth = depth
+
+          depth_inc = round(max_depth / (num_stages + 1))
+          for n in other_flop_io:
+              if n not in c_reg:
+                  c_reg.add(n, "input")
+          for i in range(depth_inc, max_depth, depth_inc):
+              for n in nodes_at_depths[i]:
+                  fanout = c_reg.fanout(n)
+                  c_reg.disconnect(n, fanout)
+                  q = c_reg.add(f"{n}{q_suffix}{i}", "buf", uid=True,
+      fanout=fanout)
+                  conns = {d_port: n, q_port: q}
+                  conns.update(other_flop_io)
+                  c_reg.add_blackbox(ff, f"ff_{n}", conns)
+          return c_reg
   def limit_fanin(c, k)
       Reduce the maximum fanin of circuit gates to k.
       ***** Parameters *****
         c :&ensp;Circuit
             Input circuit.
         k :&ensp;str
-            Maximum fanin. (k > 2)
+            Maximum fanin. (k >= 2)
       ***** Returns *****
         Circuit
             Output circuit.
         Expand source code
       def limit_fanin(c, k):
           """
           Reduce the maximum fanin of circuit gates to k.
 
           Parameters
           ----------
           c : Circuit
                   Input circuit.
           k : str
-                  Maximum fanin. (k > 2)
+                  Maximum fanin. (k >= 2)
 
           Returns
           -------
           Circuit
                   Output circuit.
 
           """
           if k < 2:
-              raise ValueError("maximum fanin, k, must be > 2")
+              raise ValueError(f"'k' must be >= 2, not '{k}'")
 
           gatemap = {
               "and": "and",
               "nand": "and",
               "or": "or",
               "nor": "or",
               "xor": "xor",
@@ -1338,14 +1612,63 @@
                       fanin=[f0, f1],
                       fanout=n,
                       uid=True,
                   )
                   i += 1
 
           return ck
+  def limit_fanout(c, k)
+      Reduce the maximum fanout of circuit gates to k.
+      ***** Parameters *****
+        c :&ensp;Circuit
+            Input circuit.
+        k :&ensp;str
+            Maximum fanout. (k >= 2)
+      ***** Returns *****
+        Circuit
+            Output circuit.
+        Expand source code
+      def limit_fanout(c, k):
+          """
+          Reduce the maximum fanout of circuit gates to k.
+
+          Parameters
+          ----------
+          c : Circuit
+                  Input circuit.
+          k : str
+                  Maximum fanout. (k >= 2)
+
+          Returns
+          -------
+          Circuit
+                  Output circuit.
+
+          """
+          if k < 2:
+              raise ValueError(f"'k' must be >= 2, not '{k}'")
+
+          ck = c.copy()
+          for n in ck.nodes():
+              i = 0
+              while len(ck.fanout(n)) > k:
+                  fo = ck.fanout(n)
+                  f0 = fo.pop()
+                  f1 = fo.pop()
+                  ck.disconnect(n, [f0, f1])
+                  ck.add(
+                      f"{n}_limit_fanout_{i}",
+                      "buf",
+                      fanin=n,
+                      fanout=[f0, f1],
+                      uid=True,
+                  )
+                  i += 1
+
+          return ck
   def miter(c0, c1=None, startpoints=None, endpoints=None)
       Create a miter circuit.
       ***** Parameters *****
         c0 :&ensp;Circuit
             First circuit.
         c1 :&ensp;Circuit
             Optional second circuit, if None c0 is mitered with itself.
@@ -2466,15 +2789,15 @@
                       add_connected_nodes=True,
                       allow_redefinition=True,
                   )
               elif c.type(n) in ["xor", "xnor"]:
                   t.add(
                       mapping[n],
                       "or",
-                      fanin=(mapping[p] for p in c.fanin(n)),
+                      fanin=[mapping[p] for p in c.fanin(n)],
                       output=c.is_output(n),
                       add_connected_nodes=True,
                       allow_redefinition=True,
                   )
               elif c.type(n) in ["0", "1"]:
                   t.add(mapping[n], "0", output=c.is_output(n),
       allow_redefinition=True)
@@ -2579,15 +2902,18 @@
        GitHub
 ****** Index ******
     * Examples
     * **** Super-module ****
           o circuitgraph
     * **** Functions ****
           o acyclic_unroll
+          o aig
+          o insert_registers
           o limit_fanin
+          o limit_fanout
           o miter
           o relabel
           o sensitivity_transform
           o sensitization_transform
           o sequential_unroll
           o strip_blackboxes
           o strip_inputs
```

### Comparing `circuitgraph-0.2.0/docs/utils.html` & `circuitgraph-0.2.1/docs/utils.html`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             tmp_in.write(bytes(bb_verilog, &#34;ascii&#34;))
             tmp_in.flush()
 
         cmd = [
             &#34;yosys&#34;,
             &#34;-p&#34;,
             f&#34;read_verilog {tmp_in.name}; &#34;
-            f&#34;show -format {fmt} -prefix {prefix} {c.name}&#34;,
+            f&#34;show -stretch -format {fmt} -prefix {prefix} {c.name}&#34;,
         ]
         subprocess.run(cmd, stdout=stdout, check=True)
 
     # Remove intermediate dot files if necessary
     if fmt != &#34;dot&#34;:
         prefix.with_suffix(&#34;.dot&#34;).unlink()
 
@@ -625,15 +625,15 @@
             tmp_in.write(bytes(bb_verilog, &#34;ascii&#34;))
             tmp_in.flush()
 
         cmd = [
             &#34;yosys&#34;,
             &#34;-p&#34;,
             f&#34;read_verilog {tmp_in.name}; &#34;
-            f&#34;show -format {fmt} -prefix {prefix} {c.name}&#34;,
+            f&#34;show -stretch -format {fmt} -prefix {prefix} {c.name}&#34;,
         ]
         subprocess.run(cmd, stdout=stdout, check=True)
 
     # Remove intermediate dot files if necessary
     if fmt != &#34;dot&#34;:
         prefix.with_suffix(&#34;.dot&#34;).unlink()</code></pre>
 </details>
@@ -672,8 +672,8 @@
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc"><cite>pdoc</cite> 0.10.0</a>.</p>
 </footer>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -81,15 +81,15 @@
             tmp_in.write(bytes(bb_verilog, "ascii"))
             tmp_in.flush()
 
         cmd = [
             "yosys",
             "-p",
             f"read_verilog {tmp_in.name}; "
-            f"show -format {fmt} -prefix {prefix} {c.name}",
+            f"show -stretch -format {fmt} -prefix {prefix} {c.name}",
         ]
         subprocess.run(cmd, stdout=stdout, check=True)
 
     # Remove intermediate dot files if necessary
     if fmt != "dot":
         prefix.with_suffix(".dot").unlink()
 
@@ -557,15 +557,15 @@
                   tmp_in.write(bytes(bb_verilog, "ascii"))
                   tmp_in.flush()
 
               cmd = [
                   "yosys",
                   "-p",
                   f"read_verilog {tmp_in.name}; "
-                  f"show -format {fmt} -prefix {prefix} {c.name}",
+                  f"show -stretch -format {fmt} -prefix {prefix} {c.name}",
               ]
               subprocess.run(cmd, stdout=stdout, check=True)
 
           # Remove intermediate dot files if necessary
           if fmt != "dot":
               prefix.with_suffix(".dot").unlink()
        GitHub
```

### Comparing `circuitgraph-0.2.0/setup.py` & `circuitgraph-0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="circuitgraph",
-    version="0.2.0",
+    version="0.2.1",
     author="Ruben Purdy, Joseph Sweeney",
     author_email="rpurdy@andrew.cmu.edu, joesweeney@cmu.edu",
     description="Tools for working with boolean circuits as graphs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/circuitgraph/circuitgraph",
     project_urls={
@@ -20,9 +20,12 @@
     packages=["circuitgraph", "circuitgraph.parsing"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
-    install_requires=["lark", "networkx",],
+    install_requires=[
+        "lark",
+        "networkx",
+    ],
 )
```

### Comparing `circuitgraph-0.2.0/tests/test_circuit.py` & `circuitgraph-0.2.1/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/tests/test_io.py` & `circuitgraph-0.2.1/tests/test_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,80 +32,44 @@
         self.assertTrue(live)
         different_output = cg.sat.solve(m, assumptions={"sat": True})
         self.assertFalse(different_output)
 
     def test_verilog(self):
         g = cg.from_file(f"{self.test_path}/test_correct_io.v")
 
-        self.assertSetEqual(
-            g.nodes(),
-            {
-                "G1",
-                "G2",
-                "G3",
-                "G4",
-                "G5_0",
-                "G5_1",
-                "G17",
-                "G18",
-                "G19",
-                "G20",
-                "G21",
-                "G22_0",
-                "G22_1",
-                "G8_0",
-                "G8_1",
-                "and_G1_G2",
-                "tie_0",
-                "tie_1",
-                "not_G2",
-                "xor_G3_G4",
-                "and_G8_0_G5_0",
-                "xor_G17_and_G8_0_G5_0",
-                "and_and_G1_G2_xor_G3_G4",
-                "and_G1_or_not_G2_tie_1",
-                "or_not_G2_tie_1",
-            },
-        )
-        self.assertSetEqual(g.fanin("G8_0"), {"G1", "G3"})
-        self.assertSetEqual(g.fanin("G17"), {"G8_1", "tie_1"})
-        self.assertEqual(g.type("G8_1"), "buf")
-        self.assertEqual(g.fanin("G8_1"), {"tie_1"})
-
-        self.assertEqual(g.type("G8_0"), "nand")
-        self.assertEqual(g.type("G17"), "nor")
-        self.assertEqual(g.type("G18"), "and")
-        self.assertTrue(g.is_output("G18"))
-        self.assertEqual(g.type("G22_0"), "xor")
-        self.assertTrue(g.is_output("G22_0"))
-        self.assertEqual(g.type("tie_1"), "1")
-        self.assertEqual(g.type("tie_0"), "0")
-
-        self.assertSetEqual(g.fanin("G19"), {"and_and_G1_G2_xor_G3_G4"})
-        self.assertSetEqual(
-            g.fanin("and_and_G1_G2_xor_G3_G4"), {"and_G1_G2", "xor_G3_G4"}
-        )
-        self.assertSetEqual(g.fanin("and_G1_G2"), {"G1", "G2"})
-        self.assertSetEqual(g.fanin("xor_G3_G4"), {"G3", "G4"})
-        self.assertSetEqual(g.fanin("G20"), {"xor_G17_and_G8_0_G5_0"})
-        self.assertSetEqual(
-            g.fanin("xor_G17_and_G8_0_G5_0"), {"G17", "and_G8_0_G5_0"},
-        )
-        self.assertSetEqual(g.fanin("and_G8_0_G5_0"), {"G8_0", "G5_0"})
-        self.assertSetEqual(g.fanin("G22_1"), {"and_G1_or_not_G2_tie_1"})
-        self.assertSetEqual(
-            g.fanin("and_G1_or_not_G2_tie_1"), {"G1", "or_not_G2_tie_1"}
-        )
-        self.assertSetEqual(g.fanin("or_not_G2_tie_1"), {"not_G2", "tie_1"})
-        self.assertSetEqual(g.fanin("not_G2"), {"G2"})
-
-        self.assertSetEqual(g.inputs(), {"G1", "G2", "G3", "G4", "G5_0", "G5_1"})
-        self.assertSetEqual(
-            g.outputs(), {"G17", "G18", "G19", "G20", "G21", "G22_0", "G22_1"},
-        )
+        c = cg.Circuit()
+        c.add("G1", "input")
+        c.add("G2", "input")
+        c.add("G3", "input")
+        c.add("G4", "input")
+        c.add("G5_0", "input")
+        c.add("G5_1", "input")
+
+        c.add("tie_1", "1")
+        c.add("tie_0", "0")
+
+        c.add("G8_0", "nand", fanin=["G1", "G3"])
+        c.add("G8_1", "buf", fanin="tie_1")
+        c.add("G17", "nor", fanin=["G8_1", "tie_1"], output=True)
+        c.add("G18", "and", fanin=["G2", "G5_0"], output=True)
+        c.add("G22_0", "xor", fanin=["G5_1", "G4"], output=True)
+
+        c.add("G3_xor_G4", "xor", fanin=["G3", "G4"])
+        c.add("G2_and_G3_xor_G4", "and", fanin=["G2", "G3_xor_G4"])
+        c.add("G19", "and", fanin=["G1", "G2_and_G3_xor_G4"], output=True)
+        c.add("G8_0_and_G5_0", "and", fanin=["G8_0", "G5_0"])
+        c.add("G20", "xor", fanin=["G17", "G8_0_and_G5_0"], output=True)
+        c.add("G21", "buf", fanin="tie_0", output=True)
+        c.add("G22_1", "buf", fanin=["G1"], output=True)
+
+        m = cg.tx.miter(g, c)
+        live = cg.sat.solve(m)
+        self.assertTrue(live)
+        different_output = cg.sat.solve(m, assumptions={"sat": True})
+        self.assertFalse(different_output)
 
     def test_fast_verilog(self):
         g = cg.from_file(f"{self.test_path}/../c432.v")
         gf = cg.from_file(f"{self.test_path}/../c432.v", fast=True)
         self.assertSetEqual(g.inputs(), gf.inputs())
         self.assertSetEqual(g.outputs(), gf.outputs())
         self.assertSetEqual(g.nodes(), gf.nodes())
```

### Comparing `circuitgraph-0.2.0/tests/test_logic.py` & `circuitgraph-0.2.1/tests/test_logic.py`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/tests/test_sat.py` & `circuitgraph-0.2.1/tests/test_sat.py`

 * *Files identical despite different names*

### Comparing `circuitgraph-0.2.0/tests/test_tx.py` & `circuitgraph-0.2.1/tests/test_tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,36 @@
         self.assertEqual(len(cu.outputs()), len(c.outputs()) * num_unroll)
 
     def test_sequential_unroll_initial_values(self):
         c = cg.from_lib("s27")
         num_unroll = 4
         initial_values = {f: str(random.getrandbits(1)) for f in c.blackboxes}
         cu, io_map = cg.tx.sequential_unroll(
-            c, num_unroll, "D", "Q", ["CK"], initial_values=initial_values,
+            c,
+            num_unroll,
+            "D",
+            "Q",
+            ["CK"],
+            initial_values=initial_values,
         )
         self.assertEqual(len(cu.inputs()), (len(c.inputs()) - 1) * num_unroll)
         self.assertEqual(len(cu.outputs()), len(c.outputs()) * num_unroll)
         for k, v in initial_values.items():
             self.assertEqual(cu.type(io_map[f"{k}_Q"][0]), v)
 
     def test_sequential_unroll_add_flop_outputs(self):
         c = cg.from_lib("s27")
         num_unroll = 4
         cu, _ = cg.tx.sequential_unroll(
-            c, num_unroll, "D", "Q", ["CK"], add_flop_outputs=True,
+            c,
+            num_unroll,
+            "D",
+            "Q",
+            ["CK"],
+            add_flop_outputs=True,
         )
         self.assertEqual(
             len(cu.inputs()), (len(c.inputs()) - 1) * num_unroll + len(c.blackboxes)
         )
         self.assertEqual(
             len(cu.outputs()), (len(c.outputs()) + len(c.blackboxes)) * num_unroll
         )
@@ -148,15 +158,16 @@
         different_output = cg.sat.solve(m, assumptions={"sat": True})
         self.assertTrue(different_output)
 
     def test_subcircuit(self):
         c17 = cg.from_lib("c17")
         sc = cg.tx.subcircuit(c17, c17.transitive_fanin("N22") | {"N22"})
         self.assertSetEqual(
-            sc.nodes(), {"N22", "N10", "N16", "N1", "N3", "N2", "N11", "N6"},
+            sc.nodes(),
+            {"N22", "N10", "N16", "N1", "N3", "N2", "N11", "N6"},
         )
         self.assertSetEqual(
             sc.edges(),
             {
                 ("N10", "N22"),
                 ("N16", "N22"),
                 ("N1", "N10"),
@@ -272,14 +283,29 @@
         m = cg.tx.miter(self.s27, s)
         live = cg.sat.solve(m)
         self.assertTrue(live)
         different_output = cg.sat.solve(m, assumptions={"sat": True})
         self.assertFalse(different_output)
         shutil.rmtree(tmpdir)
 
+    @unittest.skipIf(shutil.which("yosys") is None, "Yosys is not installed")
+    def test_aig(self):
+        aig = cg.tx.aig(self.c432)
+        m = cg.tx.miter(self.c432, aig)
+        live = cg.sat.solve(m)
+        self.assertTrue(live)
+        different_output = cg.sat.solve(m, assumptions={"sat": True})
+        self.assertFalse(different_output)
+        for node in aig:
+            self.assertTrue(aig.type(node) in ["input", "and", "not"])
+            if aig.type(node) == "and":
+                self.assertTrue(len(aig.fanin(node)) == 2)
+            elif aig.type(node) == "not":
+                self.assertTrue(len(aig.fanin(node)) == 1)
+
     def test_ternary(self):
         # Test AND gate behavior
         c = cg.Circuit()
         c.add("i0", "input")
         c.add("i1", "input")
         c.add("g0", "and", fanin=["i0", "i1"], output=True)
 
@@ -394,14 +420,34 @@
         # check conversion
         m = cg.tx.miter(c, ck)
         self.assertFalse(cg.sat.solve(m, assumptions={"sat": True}))
 
         for n in ck:
             self.assertTrue(len(ck.fanin(n)) <= k)
 
+    def test_limit_fanout(self):
+        k = 2
+        c = cg.from_lib("c1355")
+
+        any_greater = False
+        for n in c:
+            if len(c.fanout(n)) > k:
+                any_greater = True
+                break
+        self.assertTrue(any_greater)
+
+        ck = cg.tx.limit_fanout(c, k)
+
+        # check conversion
+        m = cg.tx.miter(c, ck)
+        self.assertFalse(cg.sat.solve(m, assumptions={"sat": True}))
+
+        for n in ck:
+            self.assertTrue(len(ck.fanout(n)) <= k)
+
     def test_acyclic_unroll(self):
         c = cg.Circuit()
         c.add("a", "input")
 
         c.add("g1", "and", fanin=["a"], output=True)
         c.add("g2", "buf", fanin=["g1"])
         # Add feedback edge
@@ -524,7 +570,12 @@
             for node in supergate.nodes():
                 if any(n in supergate for n in c.fanin(node)):
                     self.assertTrue(c.fanin(node).issubset(supergate.nodes()))
             # Check all inputs are disjoint
             for n0 in supergate.inputs():
                 for n1 in supergate.inputs() - {n0}:
                     self.assertFalse(c.transitive_fanin(n0) & c.transitive_fanin(n1))
+
+    def test_insert_registers(self):
+        c = cg.from_lib("c880")
+        c_reg = cg.tx.insert_registers(c, 2, q_suffix="_cg_insert_reg_q_")
+        # FIXME: Simulate to check if c_reg still behaves like c
```

### Comparing `circuitgraph-0.2.0/tests/test_utils.py` & `circuitgraph-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

