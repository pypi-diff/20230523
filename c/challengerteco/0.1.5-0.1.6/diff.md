# Comparing `tmp/challengerteco-0.1.5.tar.gz` & `tmp/challengerteco-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "challengerteco-0.1.5.tar", max compression
+gzip compressed data, was "challengerteco-0.1.6.tar", max compression
```

## Comparing `challengerteco-0.1.5.tar` & `challengerteco-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.5/README.md
--rw-r--r--   0        0        0    82996 2023-05-03 21:27:30.164715 challengerteco-0.1.5/challengerteco/Challenger.py
--rw-r--r--   0        0        0       86 2023-04-20 16:51:54.029080 challengerteco-0.1.5/challengerteco/__init__.py
--rw-r--r--   0        0        0      315 2023-05-03 21:27:35.981367 challengerteco-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 challengerteco-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.6/README.md
+-rw-r--r--   0        0        0    83011 2023-05-23 12:19:45.530008 challengerteco-0.1.6/challengerteco/Challenger.py
+-rw-r--r--   0        0        0       86 2023-04-20 16:51:54.029080 challengerteco-0.1.6/challengerteco/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-23 12:19:56.379947 challengerteco-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 challengerteco-0.1.6/PKG-INFO
```

### Comparing `challengerteco-0.1.5/challengerteco/Challenger.py` & `challengerteco-0.1.6/challengerteco/Challenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1591,17 +1591,18 @@
 
             Nombre_Modelo = 'LGBM_PRODUCTIVO' + str(Corrida)
             Productivo_scaler_train, Productivo__model_train = self.EntrenarModeloPandas('LGBM', train_undersampled_df, self.PORCENTAJE_TRAINING, self.MODELO_PRODUCTIVO_param_test, Nombre_Modelo)
 
         elif self.MODELO_PRODUCTIVO == 'XGB':
 
             Nombre_Modelo = 'XGB_PRODUCTIVO' + str(Corrida)
-            Productivo_scaler_train, Productivo__model_train, XGB_trainingData_Score, XGB_testingData_Score = self.EntrenarModeloPandas('XGB', train_undersampled_df, self.PORCENTAJE_TRAINING, self.MODELO_PRODUCTIVO_param_test, Nombre_Modelo)
+            Productivo_scaler_train, Productivo__model_train = self.EntrenarModeloPandas('XGB', train_undersampled_df, self.PORCENTAJE_TRAINING, self.MODELO_PRODUCTIVO_param_test, Nombre_Modelo)
+            # XGB_trainingData_Score, XGB_testingData_Score
 
-            self.CalcularDeciles(XGB_trainingData_Score, XGB_testingData_Score)
+            # self.CalcularDeciles(XGB_trainingData_Score, XGB_testingData_Score)
 
         if self.TIENE_TESTING == True:
             print( 'Testing ')
             if self.MODELO_PRODUCTIVO == 'RF' or self.MODELO_PRODUCTIVO == 'GB':
 
                 self.TestingModeloSpark(self.MODELO_PRODUCTIVO, testing_df_m1, Productivo_Model_train, Nombre_Modelo + ' TESTING MES1', self.PERIODO_TEST1)
                 self.TestingModeloSpark(self.MODELO_PRODUCTIVO, testing_df_m2, Productivo_Model_train, Nombre_Modelo + ' TESTING MES2', self.PERIODO_TEST2)
```

