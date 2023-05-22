# Comparing `tmp/edamame-0.52.tar.gz` & `tmp/edamame-0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.52.tar", last modified: Sat May 13 13:15:46 2023, max compression
+gzip compressed data, was "edamame-0.53.tar", last modified: Mon May 22 22:03:42 2023, max compression
```

## Comparing `edamame-0.52.tar` & `edamame-0.53.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-13 13:15:46.075268 edamame-0.52/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.52/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11935 2023-05-13 13:15:46.074796 edamame-0.52/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10181 2023-05-06 16:05:55.000000 edamame-0.52/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-13 13:15:46.066016 edamame-0.52/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-13 12:08:29.000000 edamame-0.52/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-13 13:15:46.069674 edamame-0.52/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.52/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22267 2023-05-13 12:08:26.000000 edamame-0.52/edamame/classifier/classification.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6106 2023-05-06 15:22:05.000000 edamame-0.52/edamame/classifier/diagnose.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-13 13:15:46.072200 edamame-0.52/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.52/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.52/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-06 14:05:21.000000 edamame-0.52/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-13 13:15:46.073908 edamame-0.52/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.52/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.52/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22034 2023-05-13 12:08:20.000000 edamame-0.52/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-13 13:15:46.067921 edamame-0.52/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11935 2023-05-13 13:15:46.000000 edamame-0.52/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-13 13:15:46.000000 edamame-0.52/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-13 13:15:46.000000 edamame-0.52/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-13 13:15:46.000000 edamame-0.52/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-13 13:15:46.000000 edamame-0.52/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-13 12:08:12.000000 edamame-0.52/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-13 13:15:46.075361 edamame-0.52/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.168505 edamame-0.53/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.53/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11959 2023-05-22 22:03:42.168115 edamame-0.53/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10205 2023-05-22 22:01:40.000000 edamame-0.53/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.158633 edamame-0.53/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-22 22:01:51.000000 edamame-0.53/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.162581 edamame-0.53/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.53/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22537 2023-05-22 21:51:22.000000 edamame-0.53/edamame/classifier/classification.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8611 2023-05-22 22:01:19.000000 edamame-0.53/edamame/classifier/diagnose.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.164985 edamame-0.53/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.53/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.53/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-22 20:40:47.000000 edamame-0.53/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.167001 edamame-0.53/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.53/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.53/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22034 2023-05-13 12:08:20.000000 edamame-0.53/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-22 22:03:42.160761 edamame-0.53/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11959 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-22 22:03:42.000000 edamame-0.53/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-22 22:01:47.000000 edamame-0.53/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-22 22:03:42.168618 edamame-0.53/setup.cfg
```

### Comparing `edamame-0.52/LICENSE` & `edamame-0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.52/PKG-INFO` & `edamame-0.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.52
+Version: 0.53
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -225,12 +225,12 @@
 classifier_metrics(svm_upload, X_train_s, y_train)
 ```
 
 <hr>
 
 ## Todos
 
-* Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
-
+* Add the rocauc method to the ClassifierDiagnose class. 
+* Update example notebooks.
```

### Comparing `edamame-0.52/README.md` & `edamame-0.53/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -192,12 +192,12 @@
 classifier_metrics(svm_upload, X_train_s, y_train)
 ```
 
 <hr>
 
 ## Todos
 
-* Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
-
+* Add the rocauc method to the ClassifierDiagnose class. 
+* Update example notebooks.
```

### Comparing `edamame-0.52/edamame/classifier/classification.py` & `edamame-0.53/edamame/classifier/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,20 +256,21 @@
         grid_svm_c = GridSearchCV(svm_c, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
         grid_svm_c.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
         self.__svm_fit = grid_svm_c.best_estimator_
         return self.__svm_fit
 
 
-    def model_metrics(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all') -> None:
+    def model_metrics(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all', confusion_matrix: bool = True) -> None:
         """
         Display classification metrics (confusion matrix and classification report) for specified or all trained models.
 
         Args:
             model_name (Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"]): The name of the model to display the metrics for. Defaults to 'all'.
+            confusion_matrix (bool): Whether to display the confusion matrix. Defaults to True.
 
         Returns:
             None
 
         Example:
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
@@ -283,44 +284,46 @@
                 if model_list[model_dct[key]].__class__.__name__ == 'dict':
                         display(f'unable to show {key} model metrics')
                 else:
                     title = f'### {key} model metrics:'
                     display(Markdown(title))
                     y_pred_train = model_list[model_dct[key]].predict(self.X_train)
                     y_pred_test = model_list[model_dct[key]].predict(self.X_test)
-                    plt.figure(figsize=(10,4))
-                    plt.subplot(121)
-                    sns.heatmap(confusion_matrix(self.y_train, y_pred_train), annot=True, fmt="2.0f")
-                    plt.title(f'{key} train')
-                    plt.subplot(122)
-                    sns.heatmap(confusion_matrix(self.y_test, y_pred_test), annot=True, fmt="2.0f")
-                    plt.title(f'{key} test')
-                    plt.show()
+                    if confusion_matrix:
+                        plt.figure(figsize=(10,4))
+                        plt.subplot(121)
+                        sns.heatmap(confusion_matrix(self.y_train, y_pred_train), annot=True, fmt="2.0f")
+                        plt.title(f'{key} train')
+                        plt.subplot(122)
+                        sns.heatmap(confusion_matrix(self.y_test, y_pred_test), annot=True, fmt="2.0f")
+                        plt.title(f'{key} test')
+                        plt.show()
                     title = f'#### Train classification report'
                     display(Markdown(title))
                     print(classification_report(self.y_train, y_pred_train))
                     title = f'#### Test classification report'
                     display(Markdown(title))
                     print(classification_report(self.y_test, y_pred_test))
         else:
             if model_list[model_dct[model_name]].__class__.__name__ == 'dict':
                 display(f'unable to show {model_name} model metrics')
             else:
                 title = f'### {model_name} model metrics:'
                 display(Markdown(title))
                 y_pred_train = model_list[model_dct[model_name]].predict(self.X_train)
                 y_pred_test = model_list[model_dct[model_name]].predict(self.X_test)
-                plt.figure(figsize=(10,4))
-                plt.subplot(121)
-                sns.heatmap(confusion_matrix(self.y_train, y_pred_train), annot=True, fmt="2.0f")
-                plt.title(f'{model_name} train')
-                plt.subplot(122)
-                sns.heatmap(confusion_matrix(self.y_test, y_pred_test), annot=True, fmt="2.0f")
-                plt.title(f'{model_name} test')
-                plt.show()
+                if confusion_matrix: 
+                    plt.figure(figsize=(10,4))
+                    plt.subplot(121)
+                    sns.heatmap(confusion_matrix(self.y_train, y_pred_train), annot=True, fmt="2.0f")
+                    plt.title(f'{model_name} train')
+                    plt.subplot(122)
+                    sns.heatmap(confusion_matrix(self.y_test, y_pred_test), annot=True, fmt="2.0f")
+                    plt.title(f'{model_name} test')
+                    plt.show()
                 title = f'#### Train classification report'
                 display(Markdown(title))
                 print(classification_report(self.y_train, y_pred_train))
                 title = f'#### Test classification report'
                 display(Markdown(title))
                 print(classification_report(self.y_test, y_pred_test))
```

### Comparing `edamame-0.52/edamame/eda/__init__.py` & `edamame-0.53/edamame/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `edamame-0.52/edamame/eda/eda.py` & `edamame-0.53/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.52/edamame/eda/tools.py` & `edamame-0.53/edamame/eda/tools.py`

 * *Files identical despite different names*

### Comparing `edamame-0.52/edamame/regressor/diagnose.py` & `edamame-0.53/edamame/regressor/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.52/edamame/regressor/regression.py` & `edamame-0.53/edamame/regressor/regression.py`

 * *Files identical despite different names*

### Comparing `edamame-0.52/edamame.egg-info/PKG-INFO` & `edamame-0.53/edamame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.52
+Version: 0.53
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -225,12 +225,12 @@
 classifier_metrics(svm_upload, X_train_s, y_train)
 ```
 
 <hr>
 
 ## Todos
 
-* Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
-
+* Add the rocauc method to the ClassifierDiagnose class. 
+* Update example notebooks.
```

### Comparing `edamame-0.52/pyproject.toml` & `edamame-0.53/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.52"
+version = "0.53"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

