# Comparing `tmp/gensum-0.1.2.tar.gz` & `tmp/gensum-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gensum-0.1.2.tar", last modified: Tue May 23 05:36:04 2023, max compression
+gzip compressed data, was "gensum-0.1.3.tar", last modified: Tue May 23 12:55:02 2023, max compression
```

## Comparing `gensum-0.1.2.tar` & `gensum-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:36:04.402031 gensum-0.1.2/
--rw-r--r--   0 abriel     (503) staff       (20)    11357 2023-05-18 19:51:17.000000 gensum-0.1.2/LICENSE
--rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 05:36:04.401847 gensum-0.1.2/PKG-INFO
--rw-r--r--   0 abriel     (503) staff       (20)     4400 2023-05-23 05:21:24.000000 gensum-0.1.2/README.md
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:36:04.400894 gensum-0.1.2/gensum/
--rw-r--r--   0 abriel     (503) staff       (20)       29 2023-05-19 16:34:03.000000 gensum-0.1.2/gensum/__init__.py
--rw-r--r--   0 abriel     (503) staff       (20)    15514 2023-05-23 05:29:46.000000 gensum-0.1.2/gensum/gensum.py
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:36:04.401634 gensum-0.1.2/gensum.egg-info/
--rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/PKG-INFO
--rw-r--r--   0 abriel     (503) staff       (20)      226 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/SOURCES.txt
--rw-r--r--   0 abriel     (503) staff       (20)        1 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/dependency_links.txt
--rw-r--r--   0 abriel     (503) staff       (20)       20 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/requires.txt
--rw-r--r--   0 abriel     (503) staff       (20)        7 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/top_level.txt
--rw-r--r--   0 abriel     (503) staff       (20)      500 2023-05-23 05:30:26.000000 gensum-0.1.2/pyproject.toml
--rw-r--r--   0 abriel     (503) staff       (20)       38 2023-05-23 05:36:04.402077 gensum-0.1.2/setup.cfg
--rw-r--r--   0 abriel     (503) staff       (20)      834 2023-05-23 05:30:21.000000 gensum-0.1.2/setup.py
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 12:55:02.431439 gensum-0.1.3/
+-rw-r--r--   0 abriel     (503) staff       (20)    11357 2023-05-18 19:51:17.000000 gensum-0.1.3/LICENSE
+-rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 12:55:02.431257 gensum-0.1.3/PKG-INFO
+-rw-r--r--   0 abriel     (503) staff       (20)     4400 2023-05-23 05:21:24.000000 gensum-0.1.3/README.md
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 12:55:02.430252 gensum-0.1.3/gensum/
+-rw-r--r--   0 abriel     (503) staff       (20)       29 2023-05-19 16:34:03.000000 gensum-0.1.3/gensum/__init__.py
+-rw-r--r--   0 abriel     (503) staff       (20)    15273 2023-05-23 12:51:30.000000 gensum-0.1.3/gensum/gensum.py
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 12:55:02.431036 gensum-0.1.3/gensum.egg-info/
+-rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 12:55:02.000000 gensum-0.1.3/gensum.egg-info/PKG-INFO
+-rw-r--r--   0 abriel     (503) staff       (20)      226 2023-05-23 12:55:02.000000 gensum-0.1.3/gensum.egg-info/SOURCES.txt
+-rw-r--r--   0 abriel     (503) staff       (20)        1 2023-05-23 12:55:02.000000 gensum-0.1.3/gensum.egg-info/dependency_links.txt
+-rw-r--r--   0 abriel     (503) staff       (20)       20 2023-05-23 12:55:02.000000 gensum-0.1.3/gensum.egg-info/requires.txt
+-rw-r--r--   0 abriel     (503) staff       (20)        7 2023-05-23 12:55:02.000000 gensum-0.1.3/gensum.egg-info/top_level.txt
+-rw-r--r--   0 abriel     (503) staff       (20)      500 2023-05-23 12:54:36.000000 gensum-0.1.3/pyproject.toml
+-rw-r--r--   0 abriel     (503) staff       (20)       38 2023-05-23 12:55:02.431490 gensum-0.1.3/setup.cfg
+-rw-r--r--   0 abriel     (503) staff       (20)      834 2023-05-23 12:54:45.000000 gensum-0.1.3/setup.py
```

### Comparing `gensum-0.1.2/LICENSE` & `gensum-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gensum-0.1.2/PKG-INFO` & `gensum-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensum
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generative Summarization for Data Augmentation
 Home-page: https://github.com/aaronbriel/gensum
 Author: Aaron Briel
 Author-email: aaronbriel@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gensum-0.1.2/README.md` & `gensum-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gensum-0.1.2/gensum/gensum.py` & `gensum-0.1.3/gensum/gensum.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,16 @@
         self.threshold = threshold
         self.multiproc = multiproc
         self.prompt = prompt
         self.llm = llm
         self.model = model
         self.temperature = temperature
         self.debug = debug
-        self.append_index = 0
-        self.df_append = None
+        # self.append_index = 0
+        # self.df_append = None
         self.generator = Generator(llm=llm, model=model)
         
         # If threshold not specified, set to median count for all classifiers
         # to prevent outliers from skewing results
         if self.threshold is None:
             self.threshold = int(self.df['intent'].value_counts().median())
         
@@ -178,71 +178,70 @@
         of rows. Initializes all feature values of said array to 0 to 
         accommodate future one-hot encoding of features. Loops over each 
         feature then executes loop to number of rows needed to be appended for
         oversampling to reach needed amount for given feature.
         
         :return: Dataframe appended with augmented samples to make 
             underrepresented features match the count of the majority features.
-        """
+        """        
+        df_augment = pd.DataFrame()
         append_counts = self.get_append_counts()
-        # Create append dataframe with length of all rows to be appended
-        self.df_append = pd.DataFrame(
-            index=np.arange(sum(append_counts.values())), 
-            columns=self.df.columns)
 
         for classifier_value in self.classifier_values:
             num_to_append = append_counts[classifier_value]
-            # Incrementally append based on value-specific append count
-            for num in range(
-                self.append_index, 
-                self.append_index + num_to_append):
-                self.process_generative_summarization(
-                    classifier_value, num_to_append, num)
-
-            # Updating index for insertion into shared appended dataframe to 
-            # preserve indexing in multiprocessing situation
-            self.append_index += num_to_append
+            if num_to_append > 0:
+                logger.info(f"Appending {num_to_append} rows for " + 
+                            f"'{classifier_value}' classifier value")
+                append_data = self.process_generative_summarization(
+                    classifier_value, num_to_append)
+                df_append = pd.DataFrame(append_data)
+                df_augment = pd.concat(
+                    [df_augment, df_append], ignore_index=True)
+            else:
+                logger.info(f"No rows to append for {classifier_value}")
 
-        if len(self.df_append) == 0:
+        if len(df_augment) == 0:
             logger.warning("No rows to append, returning empty DataFrame.")
             
-        return self.df_append
+        return df_augment
 
     def process_generative_summarization(
             self, 
             classifier_value: str,
             num_to_append: int, 
-            num: int,
-            multiplier: int = 4):
+            multiplier: int = 4) -> List[Dict[str, str]]:
         """
         Samples a subset of rows (with replacement if necessary) from main 
         dataframe where classifier is the specified value. The subset is then 
         passed as a list to a generative summarizer to generate a new data 
-        entry for the append count, augmenting said dataframe with rows to 
-        essentially oversample underrepresented data.
+        entry for the append count, augmenting dict to oversample 
+        underrepresented data.
         
         :param classifier_value: Classifier value to filter on
         :param num_to_append: Number of rows to append for given classifier value
-        :param num: Count of place in gen_sum_augment loop
         :multiplier: Multiplier used to decide if replacement is necessary
         """
+        append_data = []
+        
         # Replacing SUMMARY_COUNT with number of texts to summarize
         self.prompt = self.prompt.replace("SUMMARY_COUNT", str(num_to_append))
-        # Pulling rows for specified feature
         df_value = self.df[self.df[self.classifier] == classifier_value]
         # Only use replacement if there is a substantial sample count
         replace = True if len(df_value) < self.num_samples * multiplier else False
+        
         df_sample = df_value.sample(self.num_samples, replace=replace)
         text_to_summarize = df_sample[:self.num_samples][self.text_column].tolist()
         new_texts = self.get_generative_summarization(text_to_summarize)
         
-        # Breaking up summarization into separate sentences and appending each
-        for new_text in new_texts.split('\n'):
-            self.df_append.at[num, self.text_column] = new_text
-            self.df_append.at[num, self.classifier] = classifier_value
+        for text in new_texts.split("\n"):
+            append_data.append(
+                {self.text_column: text, 
+                 self.classifier: classifier_value})
+            
+        return append_data
 
     def get_value_counts(self) -> Dict[str, int]:
         """
         Gets dictionary of classifier values and their respective counts
 
         :return: Dictionary containing count of each unique classifier value
         """
@@ -363,18 +362,18 @@
     
     return min_word_count, max_word_count
 
 
 def main():
     # Sample usage
     start = time.time()
-    csv = 'path_to_csv'
+    csv = 'data/intent_sample_dataset.csv'
     df = pd.read_csv(csv)
     augmentor = Augmentor(df, text_column='text', classifier='intent')
     df_augmented = augmentor.gen_sum_augment()
     df_augmented.to_csv(csv.replace(
         '.csv', '-augmented.csv'), encoding='utf-8', index=False)
-    logger.info(f"Runtime: {(time.time() - start)/60} minutes")
+    logger.info(f"Runtime: {time.time() - start} seconds")
     
 
 if __name__ == "__main__":
     main()
```

### Comparing `gensum-0.1.2/gensum.egg-info/PKG-INFO` & `gensum-0.1.3/gensum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensum
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generative Summarization for Data Augmentation
 Home-page: https://github.com/aaronbriel/gensum
 Author: Aaron Briel
 Author-email: aaronbriel@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gensum-0.1.2/setup.py` & `gensum-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 PACKAGE_NAME = 'gensum'
 AUTHOR = 'Aaron Briel'
 AUTHOR_EMAIL = 'aaronbriel@gmail.com'
 URL = 'https://github.com/aaronbriel/gensum'
 
 LICENSE = 'Apache License 2.0'
 DESCRIPTION = 'Generative Summarization for Data Augmentation'
```

