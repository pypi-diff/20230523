# Comparing `tmp/siat-2.0.3-py3-none-any.whl.zip` & `tmp/siat-2.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1131860 bytes, number of entries: 117
+Zip file size: 1131879 bytes, number of entries: 117
 -rw-rw-rw-  2.0 fat      840 b- defN 23-Apr-10 11:29 siat/__init__.py
 -rw-rw-rw-  2.0 fat     2130 b- defN 23-Apr-10 11:29 siat/allin.py
 -rw-rw-rw-  2.0 fat      747 b- defN 23-Apr-10 11:29 siat/alpha_vantage_test.py
 -rw-rw-rw-  2.0 fat    28555 b- defN 23-Apr-10 11:29 siat/assets_liquidity.py
 -rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-10 11:29 siat/assets_liquidity_test.py
 -rw-rw-rw-  2.0 fat    10110 b- defN 23-Apr-10 11:29 siat/barrons_scraping_test.py
 -rw-rw-rw-  2.0 fat    36597 b- defN 23-Apr-10 11:29 siat/beta_adjustment.py
@@ -103,17 +103,17 @@
 -rw-rw-rw-  2.0 fat    16648 b- defN 23-Apr-18 09:06 siat/test2_graphviz.py
 -rw-rw-rw-  2.0 fat    16999 b- defN 23-Apr-14 14:38 siat/test_graphviz.py
 -rw-rw-rw-  2.0 fat    14492 b- defN 23-Apr-10 11:29 siat/transaction.py
 -rw-rw-rw-  2.0 fat    18580 b- defN 23-Apr-10 11:29 siat/transaction_test.py
 -rw-rw-rw-  2.0 fat   117953 b- defN 23-Apr-10 11:29 siat/translate-20230125.py
 -rw-rw-rw-  2.0 fat   118133 b- defN 23-Apr-10 11:29 siat/translate-20230206.py
 -rw-rw-rw-  2.0 fat   121657 b- defN 23-Apr-10 11:29 siat/translate-20230215.py
--rw-rw-rw-  2.0 fat   125046 b- defN 23-May-22 15:10 siat/translate.py
+-rw-rw-rw-  2.0 fat   125139 b- defN 23-May-23 09:39 siat/translate.py
 -rw-rw-rw-  2.0 fat     3936 b- defN 23-Apr-10 11:29 siat/universal_test.py
 -rw-rw-rw-  2.0 fat    51342 b- defN 23-May-11 00:30 siat/valuation_china.py
 -rw-rw-rw-  2.0 fat     1571 b- defN 23-Apr-10 11:29 siat/valuation_market_china_test.py
 -rw-rw-rw-  2.0 fat    14859 b- defN 23-Apr-10 11:29 siat/var_model_validation.py
--rw-rw-rw-  2.0 fat     1399 b- defN 23-May-23 02:19 siat-2.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 02:19 siat-2.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-23 02:19 siat-2.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     9354 b- defN 23-May-23 02:20 siat-2.0.3.dist-info/RECORD
-117 files, 4462589 bytes uncompressed, 1117590 bytes compressed:  75.0%
+-rw-rw-rw-  2.0 fat     1399 b- defN 23-May-23 09:48 siat-2.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 09:48 siat-2.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-23 09:48 siat-2.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     9354 b- defN 23-May-23 09:48 siat-2.0.4.dist-info/RECORD
+117 files, 4462682 bytes uncompressed, 1117609 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -333,20 +333,20 @@
 
 Filename: siat/valuation_market_china_test.py
 Comment: 
 
 Filename: siat/var_model_validation.py
 Comment: 
 
-Filename: siat-2.0.3.dist-info/METADATA
+Filename: siat-2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: siat-2.0.3.dist-info/WHEEL
+Filename: siat-2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: siat-2.0.3.dist-info/top_level.txt
+Filename: siat-2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: siat-2.0.3.dist-info/RECORD
+Filename: siat-2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siat/translate.py

```diff
@@ -909,14 +909,16 @@
         ['000044.SS','上证中盘指数'],['000046.SS','上证中小盘指数'],
         ['000045.SS','上证小盘指数'],['000004.SS','上证工业指数'],
         ['000005.SS','上证商业指数'],['000006.SS','上证地产指数'],
         ['000007.SS','上证公用指数'],['000038.SS','上证金融指数'],
         ['000057.SS','上证全指成长指数'],['000058.SS','上证全指价值指数'],
         ['000019.SS','上证治理指数'],['000048.SS','上证责任指数'],
         ['000015.SS','上证红利指数'],['899050.BJ','北证50指数'],
+        ['399006.SZ','创业板指数'],
+        ['399975.SZ','中证证券公司指数'],
         
         ['000002.SS','上证A股指数'],['000003.SS','上证B股指数'],
         ['399107.SZ','深证A股指数'],['399108.SZ','深证B股指数'],
         ['399106.SZ','深证综合指数'],['399004.SZ','深证100指数'],
         ['399012.SZ','创业板300指数'],['399991.SZ','一带一路指数'],
         
         ['399232.SZ','深证采矿业指数'],['399233.SZ','深证制造业指数'],
```

## Comparing `siat-2.0.3.dist-info/METADATA` & `siat-2.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siat
-Version: 2.0.3
+Version: 2.0.4
 Summary: Securities Investment Analysis Tools (siat)
 Home-page: https://pypi.org/project/siat/
 Author: Prof. WANG Dehong, Business School, BFSU (北京外国语大学 国际商学院 王德宏 教授)
 Author-email: wdehong2000@163.com
 License: Copyright (C) WANG Dehong, 2023. For educational purpose only!
 Platform: UNKNOWN
 Requires-Dist: pandas-datareader
```

## Comparing `siat-2.0.3.dist-info/RECORD` & `siat-2.0.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 siat/test2_graphviz.py,sha256=05w2YJuIBH0LsJjdA60EFn7rL0vCo-CA6EVJEQOXNE4,16648
 siat/test_graphviz.py,sha256=CETKpDL8PnysS-PD3fHkeAgagUxjaUl0CsXPiadQySg,16999
 siat/transaction.py,sha256=foTWS1qYXQFuzNTG2m7ec6aDgsJjzpKmyAbyxKcE8KU,14492
 siat/transaction_test.py,sha256=Z8g1LJCN4-mnUByXMUMoFmN0t105cbmsz2QmvSuIkbU,18580
 siat/translate-20230125.py,sha256=NPPSXhT38s5t9fzMvl_fvi4ckSB73ThLmZetVI-xGdU,117953
 siat/translate-20230206.py,sha256=-vtI125WyaJhmPotOpDAmclt_XnYVaWU9ByLWZ6FyYE,118133
 siat/translate-20230215.py,sha256=TJgtPE3n8IjljmZ4Pefy8dmHoNdFF-1zpML6BhA9FKE,121657
-siat/translate.py,sha256=CLlYaG_5i_UlSfNnvavb1AZtQ7Uwei8aL-9_s69TVLg,125046
+siat/translate.py,sha256=XAuODqRc9wJokiWJa0goZOJe0qsXcJxoQS4cBbYPTww,125139
 siat/universal_test.py,sha256=CDAOffW1Rvs-TcNN5giWVvHMlch1w4dp-w5SIV9jXL0,3936
 siat/valuation_china.py,sha256=gYYXeT9bBPyQ251TCsYlibWcu6JA8x-YOKqLUEeLE7U,51342
 siat/valuation_market_china_test.py,sha256=gbJ0ioauuo4koTPH6WKUkqcXiQPafnbhU5eKJ6lpdLA,1571
 siat/var_model_validation.py,sha256=zB_Skk_tmzIR15l6oAW3am4HBGVIG-eZ8gJhCdXZ8Qw,14859
-siat-2.0.3.dist-info/METADATA,sha256=kGzJju3RsFmfr8-cC75BmlU4f9QCMYUtlzY0H2sIVhc,1399
-siat-2.0.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-siat-2.0.3.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
-siat-2.0.3.dist-info/RECORD,,
+siat-2.0.4.dist-info/METADATA,sha256=l1h2KZvK8y7tA_xa-3XCz8ExeaNNTrfpNiO1re8iyPs,1399
+siat-2.0.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+siat-2.0.4.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
+siat-2.0.4.dist-info/RECORD,,
```

