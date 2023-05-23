# Comparing `tmp/itca-0.1.0.tar.gz` & `tmp/itca-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\itca-0.1.0.tar", last modified: Mon Aug 16 05:31:35 2021, max compression
+gzip compressed data, was "itca-0.1.1.tar", last modified: Tue May 23 14:33:28 2023, max compression
```

## Comparing `itca-0.1.0.tar` & `itca-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxrwx   0        0        0        0 2021-08-16 05:31:35.000000 itca-0.1.0/
--rw-rw-rw-   0        0        0     1016 2021-08-16 05:31:35.000000 itca-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      259 2021-08-16 05:16:48.000000 itca-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2021-08-16 05:31:35.000000 itca-0.1.0/itca/
--rw-rw-rw-   0        0        0      294 2021-08-16 05:01:29.000000 itca-0.1.0/itca/__init__.py
--rw-rw-rw-   0        0        0     6953 2021-08-16 05:01:29.000000 itca-0.1.0/itca/metrics.py
--rw-rw-rw-   0        0        0    17430 2021-08-16 05:01:29.000000 itca-0.1.0/itca/search.py
--rw-rw-rw-   0        0        0     9380 2021-08-16 05:01:29.000000 itca-0.1.0/itca/simulator.py
--rw-rw-rw-   0        0        0     6245 2021-08-16 05:01:29.000000 itca-0.1.0/itca/utils.py
-drwxrwxrwx   0        0        0        0 2021-08-16 05:31:35.000000 itca-0.1.0/itca.egg-info/
--rw-rw-rw-   0        0        0     1016 2021-08-16 05:31:35.000000 itca-0.1.0/itca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2021-08-16 05:31:35.000000 itca-0.1.0/itca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-16 05:31:35.000000 itca-0.1.0/itca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2021-08-16 05:31:35.000000 itca-0.1.0/itca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2021-08-16 05:31:35.000000 itca-0.1.0/itca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-16 05:31:35.000000 itca-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3268 2021-08-16 05:01:29.000000 itca-0.1.0/setup.py
+drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-05-23 14:33:28.882312 itca-0.1.1/
+-rw-r--r--   0 chzhang    (501) staff       (20)     1091 2023-05-19 13:33:06.000000 itca-0.1.1/LICENSE
+-rw-r--r--   0 chzhang    (501) staff       (20)     4093 2023-05-23 14:33:28.882175 itca-0.1.1/PKG-INFO
+-rw-r--r--   0 chzhang    (501) staff       (20)     3377 2023-05-19 13:33:06.000000 itca-0.1.1/README.md
+drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-05-23 14:33:28.876088 itca-0.1.1/itca/
+-rw-r--r--   0 chzhang    (501) staff       (20)      276 2023-05-19 13:33:06.000000 itca-0.1.1/itca/__init__.py
+drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-05-23 14:33:28.877105 itca-0.1.1/itca/datasets/
+-rw-r--r--   0 chzhang    (501) staff       (20)      278 2023-05-22 03:54:15.000000 itca-0.1.1/itca/datasets/__init__.py
+-rw-r--r--   0 chzhang    (501) staff       (20)  8118532 2023-05-22 02:02:59.000000 itca-0.1.1/itca/datasets/hydra.npz
+-rw-r--r--   0 chzhang    (501) staff       (20)     4968 2023-05-19 13:33:06.000000 itca-0.1.1/itca/metrics.py
+-rw-r--r--   0 chzhang    (501) staff       (20)    18455 2023-05-19 13:33:06.000000 itca-0.1.1/itca/search.py
+-rw-r--r--   0 chzhang    (501) staff       (20)     4254 2023-05-19 13:33:06.000000 itca-0.1.1/itca/simulation_suites.py
+-rw-r--r--   0 chzhang    (501) staff       (20)     9112 2023-05-22 04:35:43.000000 itca-0.1.1/itca/simulator.py
+-rw-r--r--   0 chzhang    (501) staff       (20)     8157 2023-05-19 13:33:06.000000 itca-0.1.1/itca/utils.py
+-rw-r--r--   0 chzhang    (501) staff       (20)     2957 2023-05-23 14:25:02.000000 itca-0.1.1/itca/visualize.py
+drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-05-23 14:33:28.876729 itca-0.1.1/itca.egg-info/
+-rw-r--r--   0 chzhang    (501) staff       (20)     4093 2023-05-23 14:33:28.000000 itca-0.1.1/itca.egg-info/PKG-INFO
+-rw-r--r--   0 chzhang    (501) staff       (20)      339 2023-05-23 14:33:28.000000 itca-0.1.1/itca.egg-info/SOURCES.txt
+-rw-r--r--   0 chzhang    (501) staff       (20)        1 2023-05-23 14:33:28.000000 itca-0.1.1/itca.egg-info/dependency_links.txt
+-rw-r--r--   0 chzhang    (501) staff       (20)       75 2023-05-23 14:33:28.000000 itca-0.1.1/itca.egg-info/requires.txt
+-rw-r--r--   0 chzhang    (501) staff       (20)        5 2023-05-23 14:33:28.000000 itca-0.1.1/itca.egg-info/top_level.txt
+-rw-r--r--   0 chzhang    (501) staff       (20)       38 2023-05-23 14:33:28.882356 itca-0.1.1/setup.cfg
+-rw-r--r--   0 chzhang    (501) staff       (20)     3347 2023-05-23 14:33:09.000000 itca-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `itca-0.1.0/itca/search.py` & `itca-0.1.1/itca/search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,453 +1,484 @@
-import abc
-import numpy as np
-from itertools import combinations
-from sklearn.model_selection import KFold
-from itca.utils import bidict, compute_y_dist
-from itca.metrics import itca
-
-
-class Node(object):
-    def __init__(self, vals, mapping):
-        self.vals = vals
-        self.mapping = mapping
-        self.children = None
-
-    def __repr__(self):
-        return "{}|ITAC={:.4f}|".format(self.mapping, np.mean(self.vals))
-
-    def add_child(self, node):
-        if self.children:
-            self.children.append(node)
-        else:
-            self.children = [node]
-
-
-class Strategy(metaclass=abc.ABCMeta):
-    def __init__(self, class_type="nominal", metric=itca):
-        """
-        Searching strategy.
-
-        Parameters
-        ----------
-        class_type: {"nominal", "ordinal", "tree"}
-            Type of classes.
-        """
-        self.class_type = class_type
-        self.metric = metric
-        self.path = None
-        self.selected = None
-
-    def __repr__(self):
-        return "{}(class_type={})".format(self.__class__.__name__, self.class_type)
-
-    @staticmethod
-    def combine_i_j(i, j, mapping):
-        """
-        Combine (merged) class labels i and j in mapping.
-
-        Parameters
-        ----------
-        i: int
-        j: int
-
-        Return
-        ------
-        next_mapping: bidict
-            mapping that combines the class i and j
-        
-        Example
-        -------
-        >>mapping = bidict({0:0, 1:1, 2:2})
-        >>self.combine_i_j(0, 1, mapping)
-        {0:0, 1:0, 2:1}
-        """
-        next_mapping = dict()
-        for key in mapping.inverse:
-            if key < j:
-                next_mapping.update({e: key for e in mapping.inverse[key]})
-            elif key > j:
-                next_mapping.update({e: key - 1 for e in mapping.inverse[key]})
-            else:
-                next_mapping.update({e: i for e in mapping.inverse[key]})
-        return bidict(next_mapping)
-
-    def next_mappings(self, mapping, class_type):
-        """
-        Generate mappings considered in the next round of search.
-
-        Parameters
-        ----------
-        mapping: bidict
-            classes combination mappings.
-
-        class_type: {"nominal", "ordinal", "tree"}
-            Type of classes.
-
-        Yields
-        ------
-        bidict
-            Mappings that are considered in the next round of search.
-
-        Raises
-        ------
-        ValueError
-            If class_type is illegal.
-        """
-        if class_type == "nominal":
-            for i, j in combinations(range(len(mapping.inverse)), 2):
-                yield self.combine_i_j(i, j, mapping)
-        elif class_type == "ordinal":
-            for i in range(len(mapping.inverse) - 1):
-                yield self.combine_i_j(i, i + 1, mapping)
-        elif class_type == "tree":
-            raise NotImplementedError(
-                "Tree-based next-mapping is not implemeted")
-        else:
-            raise ValueError(
-                "class_type must be one of \"nominal\", \"ordinal\" and \"tree\".")
-
-    def next_mappings_pruned(self, mapping, class_type, class_acc, ty_dist):
-        """
-        Generate mappings considered in the next round of search.
-
-        Parameters
-        ----------
-        mapping: bidict
-            classes combination mappings.
-
-        class_type: {"nominal", "ordinal", "tree"}
-            Type of classes.
-
-        Yields
-        ------
-        bidict
-            Mappings that are considered in the next round of search.
-
-        Raises
-        ------
-        ValueError
-            If class_type is illegal.
-        """
-
-        def compute_lb(i, j):
-            ai, aj = np.mean(class_acc[i]), np.mean(class_acc[j])
-            pi, pj = ty_dist[i], ty_dist[j]
-            return (-pi * np.log(pi) * np.mean(ai) - pj * np.log(pj) * np.mean(aj)) \
-                   / ((-pi - pj) * np.log(pi + pj))
-
-        if class_type == "nominal":
-            for i, j in combinations(range(len(mapping.inverse)), 2):
-                if compute_lb(i, j) < 1:
-                    yield self.combine_i_j(i, j, mapping)
-        elif class_type == "ordinal":
-            for i in range(len(mapping.inverse) - 1):
-                if compute_lb(i, i + 1) < 1:
-                    yield self.combine_i_j(i, i + 1, mapping)
-        elif class_type == "tree":
-            raise NotImplementedError(
-                "Tree-based next-mapping is not implemeted")
-        else:
-            raise ValueError(
-                "class_type must be one of \"nominal\", \"ordinal\" and \"tree\".")
-
-    def compute_itca(self, X, y, clf, mapping, kfolds=5, y_dist=None, return_class_acc=False):
-        """
-        Given the data and a classifier, compute ITCA through cross validation.
-
-        Parameters
-        ----------
-        X: array like of shape (n_samples, n_features)
-            The training input samples.
-
-        y: array like of shape (n_samples, )
-            The target class labels. Integers from 0 to K-1.
-
-        clf: scikit-learn like classifier 
-            Classifiers that implements the standard interfaces of `scikit-learn`, 
-            including `fit(X, y)` and `predict(X)`.
-
-        kfolds: int or sklearn.model_selection.KFold instance
-            Folds of cross validation.
-
-        y_dist: dict, optional
-            The classes distribution of y. If y_dist is None, this method will 
-            compute it automatically.
-
-        return_class_acc: bool
-            Return the class-wise accuracy.
-
-        Returns
-        -------
-        itca_cv: (kfolds, ) ndarray
-            The cross validated ITCA.ndarray of ITCA.
-        
-        class_acc: dict of accuracy of each class.
-            Accruacy of each class.
-
-        Raises
-        ------
-        ValueError
-            kf is illegal.
-        
-        ValueError
-            y_dist is illegal.
-        """
-        if isinstance(kfolds, int) and kfolds > 1:
-            kf = KFold(n_splits=kfolds, shuffle=True)
-        elif kfolds == 1:
-            pass
-        elif isinstance(kfolds, KFold):
-            kf = kfolds
-        else:
-            raise ValueError("kf must be int or sklearn.model_selection.KFold instance.")
-        if y_dist is None:
-            y_dist = compute_y_dist(y)
-        itca_cv = []
-        ty = mapping.map(y)
-        unique_ty = np.unique(ty)
-        if return_class_acc:
-            class_acc = {key: [] for key in unique_ty}
-        if kfolds == 1:
-            clf.fit(X, ty)
-            y_pred = clf.predict(X)
-            itca_cv = [self.metric(y, y_pred, mapping, y_dist)]
-        else:
-            for train_index, test_index in kf.split(X):
-                X_train, X_test = X[train_index], X[test_index]
-                ty_train, y_test = ty[train_index], y[test_index]
-                clf.fit(X_train, ty_train)
-                y_pred = clf.predict(X_test)
-                itca_cv.append(self.metric(y_test, y_pred, mapping, y_dist))
-                ty_test = ty[test_index]
-                if return_class_acc:
-                    for key in class_acc:
-                        indexes = ty_test == key
-                        class_acc[key].append(np.sum(ty_test[indexes] == y_pred[indexes]) / np.sum(indexes))
-
-        if return_class_acc:
-            return np.array(itca_cv), class_acc
-        else:
-            return np.array(itca_cv)
-
-    @abc.abstractmethod
-    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=False):
-        """
-        Search the best mapping start.
-
-        Parameters
-        ----------
-        X: array like of shape (n_samples, n_features)
-            The training input samples.
-
-        y: array like of shape (n_samples, )
-            The target class labels. Integers from 0 to K-1.
-
-        class_type: {"nominal", "ordinal", "tree"}
-            Type of classes.
-
-        clf: scikit-learn like classifier 
-            Classifiers that implements the standard interfaces of `scikit-learn`, 
-            including `fit(X, y)` and `predict(X)`.
- 
-        Return
-        ------
-        self: object
-        """
-        return self
-
-
-class GreedySearch(Strategy):
-    """
-    Search mapping with largest ITCA by greedy algorithm.
-    """
-
-    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=True):
-        unique_y = np.unique(y)
-        n_classes = len(unique_y)
-        if min(y) != 0 or max(y) != n_classes - 1:
-            raise ValueError("Labels should be between 0 to K.")
-        if kfolds > 1:
-            kf = KFold(n_splits=kfolds, shuffle=True)
-        else:
-            kf = 1
-        # compute y_dist
-        y_dist = compute_y_dist(y)
-        # construct identity mapping.
-        cur_mapping = bidict({key: key for key in range(n_classes)})
-        cur_itca = self.compute_itca(X, y, clf, cur_mapping, kfolds=kf, y_dist=y_dist)
-        cur_node = Node(cur_itca, cur_mapping)
-        self.selected = cur_node
-        self.path = cur_node
-        i = 1
-        self.counter = 0
-        while len(cur_mapping.inverse) > 2:
-            # compute itac of current mapping
-            if verbose:
-                print("Round={}|Current Mapping={}".format(i, cur_mapping))
-            next_itcas = []
-            candidate_mappings = []
-            for next_mapping in self.next_mappings(cur_mapping, self.class_type):
-                candidate_mappings.append(next_mapping)
-                self.counter += 1
-                next_itcas.append(self.compute_itca(X, y, clf, next_mapping, kfolds=kf, y_dist=y_dist))
-            # choose best mapping
-            next_ind = np.argmax([np.mean(itca) for itca in next_itcas])
-            cur_mapping = candidate_mappings[next_ind]
-            next_node = Node(next_itcas[next_ind], cur_mapping)
-            cur_node.children = [next_node]
-            cur_node = next_node
-            i += 1
-            if np.mean(cur_node.vals) > np.mean(self.selected.vals):
-                self.selected = cur_node
-            elif early_stop:
-                break
-        return self
-
-
-class GreedySearchPruned(Strategy):
-    """
-    Greedy search using the lower bound derived by class-wise accuracy to prune search space.
-    """
-
-    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=True):
-        unique_y = np.unique(y)
-        n_classes = len(unique_y)
-        if min(y) != 0 or max(y) != n_classes - 1:
-            raise ValueError("Labels should be between 0 to K.")
-        kf = KFold(n_splits=kfolds, shuffle=True)
-        # compute y_dist
-        y_dist = compute_y_dist(y)
-        # construct identity mapping.
-        cur_mapping = bidict({key: key for key in range(n_classes)})
-        cur_itca, cur_class_acc = self.compute_itca(X, y, clf, cur_mapping, kfolds=kf, y_dist=y_dist,
-                                                    return_class_acc=True)
-        cur_y_dist = compute_y_dist(cur_mapping.map(y))
-        cur_node = Node(cur_itca, cur_mapping)
-        self.selected = cur_node
-        self.path = cur_node
-        i = 1
-        self.counter = 0
-        while len(cur_mapping.inverse) > 2:
-            # compute itac of current mapping
-            if verbose:
-                print("Round={}|Current Mapping={}".format(i, cur_mapping))
-            next_itcas = []
-            next_class_accs = []
-            candidate_mappings = []
-            for next_mapping in self.next_mappings_pruned(cur_mapping, self.class_type,
-                                                          cur_class_acc, cur_y_dist):
-                candidate_mappings.append(next_mapping)
-                self.counter += 1
-                itca, class_acc = self.compute_itca(X, y, clf, next_mapping, kfolds=kf, y_dist=y_dist,
-                                                    return_class_acc=True)
-                next_itcas.append(itca)
-                next_class_accs.append(class_acc)
-            # choose best mapping
-            if len(next_itcas) == 0:
-                break
-            else:
-                next_ind = np.argmax([np.mean(itca) for itca in next_itcas])
-                cur_mapping = candidate_mappings[next_ind]
-                cur_class_acc = next_class_accs[next_ind]
-                cur_y_dist = compute_y_dist(cur_mapping.map(y))
-                next_node = Node(next_itcas[next_ind], cur_mapping)
-                cur_node.children = [next_node]
-                cur_node = next_node
-                i += 1
-                if np.mean(cur_node.vals) > np.mean(self.selected.vals):
-                    self.selected = cur_node
-        return self
-
-
-class BFSearch(Strategy):
-    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=False):
-        self.counter = 0
-
-        def bfs(visited, cur_node, kf, y_dist, i):
-            if len(cur_node.mapping.inverse) > 2:
-                for next_mapping in self.next_mappings(cur_node.mapping, self.class_type):
-                    next_fs = frozenset(next_mapping.items())
-                    if next_fs not in visited:
-                        self.counter += 1
-                        next_itca = self.compute_itca(X, y, clf, next_mapping, kf, y_dist)
-                        visited.add(next_fs)
-                        if np.mean(next_itca) > np.mean(cur_node.vals):
-                            next_node = Node(next_itca, next_mapping)
-                            cur_node.add_child(next_node)
-                            if verbose:
-                                print("Level={}|Current Mapping={}".format(i, next_mapping))
-                            if np.mean(next_itca) > np.mean(self.selected.vals):
-                                self.selected = next_node
-                            bfs(visited, next_node, kf, y_dist, i + 1)
-
-        unique_y = np.unique(y)
-        n_classes = len(unique_y)
-        if min(y) != 0 or max(y) != n_classes - 1:
-            raise ValueError("Labels should be between 0 to K.")
-        kf = KFold(n_splits=kfolds, shuffle=True)
-        # compute y_dist
-        y_dist = compute_y_dist(y)
-        # construct identity mapping.
-        cur_mapping = bidict({key: key for key in range(n_classes)})
-        cur_itca = self.compute_itca(X, y, clf, cur_mapping, kfolds=kf, y_dist=y_dist)
-        self.counter += 1
-        cur_node = Node(cur_itca, cur_mapping)
-        self.selected = cur_node
-        self.path = cur_node
-        i = 1
-        visited = set([frozenset(cur_mapping.items())])
-        # driver code
-        bfs(visited, cur_node, kf, y_dist, i)
-        self.visited = visited
-        return self
-
-
-class BFSearchPruned(Strategy):
-    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=True):
-        self.counter = 0
-        unique_y = np.unique(y)
-        n_classes = len(unique_y)
-        if min(y) != 0 or max(y) != n_classes - 1:
-            raise ValueError("Labels should be between 0 to K.")
-        kf = KFold(n_splits=kfolds, shuffle=True)
-        # compute y_dist
-        y_dist = compute_y_dist(y)
-
-        def bfs(visited, cur_node, cur_class_acc, cur_ty_dist, i):
-            if len(cur_node.mapping.inverse) > 2:
-                for next_mapping in self.next_mappings_pruned(cur_node.mapping, self.class_type,
-                                                              cur_class_acc, cur_ty_dist):
-                    next_fs = frozenset(next_mapping.items())
-                    if next_fs not in visited:
-                        self.counter += 1
-                        next_itca, next_class_acc = self.compute_itca(X, y, clf, next_mapping, kf,
-                                                                      y_dist, return_class_acc=True)
-                        visited.add(next_fs)
-                        if np.mean(next_itca) > np.mean(cur_node.vals):
-                            next_node = Node(next_itca, next_mapping)
-                            cur_node.add_child(next_node)
-                            if verbose:
-                                print("Level={}|Current Mapping={}".format(i, next_mapping))
-                            if np.mean(next_itca) > np.mean(self.selected.vals):
-                                self.selected = next_node
-                            cur_ty_dist = compute_y_dist(next_node.mapping.map(y))
-                            bfs(visited, next_node, next_class_acc, cur_ty_dist, i + 1)
-
-        # construct identity mapping.
-        cur_mapping = bidict({key: key for key in range(n_classes)})
-        cur_itca, cur_class_acc = self.compute_itca(X, y, clf, cur_mapping, kfolds=kf,
-                                                    y_dist=y_dist, return_class_acc=True)
-        self.counter += 1
-        cur_node = Node(cur_itca, cur_mapping)
-        self.selected = cur_node
-        self.path = cur_node
-        i = 1
-        visited = set([frozenset(cur_mapping.items())])
-        bfs(visited, cur_node, cur_class_acc, y_dist, i)
-        self.visited = visited
-        return self
-
-if __name__ == "__main__":
-    mapping = bidict({0: 0, 1: 0, 2: 1, 3: 2, 4: 3})
-    for m in Strategy.next_mappings(mapping, "nominal"):
-        print(m.inverse)
+import abc
+import numpy as np
+from itertools import combinations
+from sklearn.model_selection import KFold
+from itca.utils import bidict, compute_y_dist
+from itca.metrics import itca
+
+
+class Node(object):
+    def __init__(self, vals, mapping):
+        self.vals = vals
+        self.mapping = mapping
+        self.children = None
+
+    def __repr__(self):
+        return "{}|ITCA={:.4f}|".format(self.mapping, np.mean(self.vals))
+
+    def add_child(self, node):
+        if self.children:
+            self.children.append(node)
+        else:
+            self.children = [node]
+
+
+class Strategy(metaclass=abc.ABCMeta):
+    """
+    Attributes
+    ---------
+    class_type: str
+        The class tyype. It should be one of "nominal" (the class has no specific oder), "ordinal" and "tree"
+        for tree structured (not implemented for now).
+
+    metric: function
+        The function with signature (y_test, y_pred, mapping, y_dist) and outputs a real-value.
+
+
+    Methods
+    -------
+    compute_itca(self, X, y, clf, mapping, kfolds=5, y_dist=None, return_class_acc=False)
+        Given the map compute the metric value.
+
+    search(self, X, y, clf, kfolds=5, verbose=False, early_stop=True):
+        Search the best mapping start from the identitfy map.
+    """
+    def __init__(self, class_type="nominal", metric=itca):
+        """
+        Searching strategy.
+
+        Parameters
+        ----------
+        class_type: {"nominal", "ordinal", "tree"}
+            Type of classes.
+        """
+        self.class_type = class_type
+        self.metric = metric
+        self.path = None
+        self.selected = None
+
+    def __repr__(self):
+        return "{}(class_type={})".format(self.__class__.__name__, self.class_type)
+
+    @staticmethod
+    def combine_i_j(i, j, mapping):
+        """
+        Combine (merged) class labels i and j in mapping.
+
+        Parameters
+        ----------
+        i: int
+        j: int
+
+        Return
+        ------
+        next_mapping: bidict
+            mapping that combines the class i and j
+        
+        Example
+        -------
+        >>mapping = bidict({0:0, 1:1, 2:2})
+        >>self.combine_i_j(0, 1, mapping)
+        {0:0, 1:0, 2:1}
+        """
+        next_mapping = dict()
+        for key in mapping.inverse:
+            if key < j:
+                next_mapping.update({e: key for e in mapping.inverse[key]})
+            elif key > j:
+                next_mapping.update({e: key - 1 for e in mapping.inverse[key]})
+            else:
+                next_mapping.update({e: i for e in mapping.inverse[key]})
+        return bidict(next_mapping)
+
+    def next_mappings(self, mapping, class_type):
+        """
+        Generate mappings considered in the next round of search.
+
+        Parameters
+        ----------
+        mapping: bidict
+            classes combination mappings.
+
+        class_type: {"nominal", "ordinal", "tree"}
+            Type of classes.
+
+        Yields
+        ------
+        bidict
+            Mappings that are considered in the next round of search.
+
+        Raises
+        ------
+        ValueError
+            If class_type is illegal.
+        """
+        if class_type == "nominal":
+            for i, j in combinations(range(len(mapping.inverse)), 2):
+                yield self.combine_i_j(i, j, mapping)
+        elif class_type == "ordinal":
+            for i in range(len(mapping.inverse) - 1):
+                yield self.combine_i_j(i, i + 1, mapping)
+        elif class_type == "tree":
+            raise NotImplementedError(
+                "Tree-based next-mapping is not implemeted")
+        else:
+            raise ValueError(
+                "class_type must be one of \"nominal\", \"ordinal\" and \"tree\".")
+
+    def next_mappings_pruned(self, mapping, class_type, class_acc, ty_dist):
+        """
+        Generate mappings considered in the next round of search.
+
+        Parameters
+        ----------
+        mapping: bidict
+            classes combination mappings.
+
+        class_type: {"nominal", "ordinal", "tree"}
+            Type of classes.
+
+        Yields
+        ------
+        bidict
+            Mappings that are considered in the next round of search.
+
+        Raises
+        ------
+        ValueError
+            If class_type is illegal.
+        """
+
+        def compute_lb(i, j):
+            ai, aj = np.mean(class_acc[i]), np.mean(class_acc[j])
+            pi, pj = ty_dist[i], ty_dist[j]
+            return (-pi * np.log(pi) * np.mean(ai) - pj * np.log(pj) * np.mean(aj)) \
+                   / ((-pi - pj) * np.log(pi + pj))
+
+        if class_type == "nominal":
+            for i, j in combinations(range(len(mapping.inverse)), 2):
+                if compute_lb(i, j) < 1:
+                    yield self.combine_i_j(i, j, mapping)
+        elif class_type == "ordinal":
+            for i in range(len(mapping.inverse) - 1):
+                if compute_lb(i, i + 1) < 1:
+                    yield self.combine_i_j(i, i + 1, mapping)
+        elif class_type == "tree":
+            raise NotImplementedError(
+                "Tree-based next-mapping is not implemeted")
+        else:
+            raise ValueError(
+                "class_type must be one of \"nominal\", \"ordinal\" and \"tree\".")
+
+    def compute_itca(self, X, y, clf, mapping, kfolds=5, y_dist=None, return_class_acc=False, random_state=None):
+        """
+        Given the data and a classifier, compute ITCA through cross validation.
+
+        Parameters
+        ----------
+        X: array-like of shape (n_samples, n_features)
+            The training input samples.
+
+        y: array like of shape (n_samples, )
+            The target class labels. Integers from 0 to K-1.
+
+        clf: scikit-learn like classifier 
+            Classifiers that implements the standard interfaces of `scikit-learn`, 
+            including `fit(X, y)` and `predict(X)`.
+
+        kfolds: int or sklearn.model_selection.KFold instance
+            Folds of cross validation.
+
+        y_dist: dict, optional
+            The classes distribution of y. If y_dist is None, this method will 
+            compute it automatically.
+
+        return_class_acc: bool
+            Return the class-wise accuracy.
+
+        random_state: int, RandomState instance or None, optional (default=None)
+
+        Returns
+        -------
+        itca_cv: (kfolds, ) ndarray
+            The cross validated ITCA.ndarray of ITCA.
+        
+        class_acc: dict of accuracy of each class.
+            Accruacy of each class.
+
+        Raises
+        ------
+        ValueError
+            kf is illegal.
+        
+        ValueError
+            y_dist is illegal.
+        """
+        if isinstance(kfolds, int) and kfolds > 1:
+            kf = KFold(n_splits=kfolds, shuffle=True, random_state=random_state)
+        elif kfolds == 1:
+            pass
+        elif isinstance(kfolds, KFold):
+            kf = kfolds
+        else:
+            raise ValueError("kf must be int or sklearn.model_selection.KFold instance.")
+        if y_dist is None:
+            y_dist = compute_y_dist(y)
+        itca_cv = []
+        ty = mapping.map(y)
+        unique_ty = np.unique(ty)
+        if return_class_acc:
+            class_acc = {key: [] for key in unique_ty}
+        if kfolds == 1:
+            clf.fit(X, ty)
+            y_pred = clf.predict(X)
+            itca_cv = [self.metric(y, y_pred, mapping, y_dist)]
+        else:
+            for train_index, test_index in kf.split(X):
+                X_train, X_test = X[train_index], X[test_index]
+                ty_train, y_test = ty[train_index], y[test_index]
+                clf.fit(X_train, ty_train)
+                y_pred = clf.predict(X_test)
+                itca_cv.append(self.metric(y_test, y_pred, mapping, y_dist))
+                ty_test = ty[test_index]
+                if return_class_acc:
+                    for key in class_acc:
+                        indexes = ty_test == key
+                        class_acc[key].append(np.sum(ty_test[indexes] == y_pred[indexes]) / np.sum(indexes))
+
+        if return_class_acc:
+            return np.array(itca_cv), class_acc
+        else:
+            return np.array(itca_cv)
+
+    @abc.abstractmethod
+    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=False):
+        return self
+
+
+class GreedySearch(Strategy):
+    """
+    Search the class combination map that maximizes s-ITCA by greedy algorithm.
+    """
+
+    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=True, random_state=None):
+        """
+        Search the best mapping start.
+
+        Parameters
+        ----------
+        X: array like of shape (n_samples, n_features)
+            The training input samples.
+
+        y: array like of shape (n_samples, )
+            The target class labels. Integers from 0 to K-1.
+
+        clf: scikit-learn like classifier
+            Classifiers that implements the standard interfaces of `scikit-learn`,
+            including `fit(X, y)` and `predict(X)`.
+
+        random_state: int, RandomState instance or None, optional (default=None)
+
+        early_stop: bool
+            Stop when the metric cannot be improved by class combination when `early_stop` is True.
+
+        Return
+        ------
+        self: object
+        """
+        unique_y = np.unique(y)
+        n_classes = len(unique_y)
+        if min(y) != 0 or max(y) != n_classes - 1:
+            raise ValueError("Labels should be between 0 to K.")
+        if kfolds > 1:
+            kf = KFold(n_splits=kfolds, shuffle=True, random_state=random_state)
+        else:
+            kf = 1
+        # compute y_dist
+        y_dist = compute_y_dist(y)
+        # construct identity mapping.
+        cur_mapping = bidict({key: key for key in range(n_classes)})
+        cur_itca = self.compute_itca(X, y, clf, cur_mapping, kfolds=kf, y_dist=y_dist)
+        cur_node = Node(cur_itca, cur_mapping)
+        self.selected = cur_node
+        self.path = cur_node
+        i = 1
+        self.counter = 0
+        while len(cur_mapping.inverse) > 2:
+            # compute itac of current mapping
+            if verbose:
+                print("Round={}|Current Mapping={}".format(i, cur_mapping))
+            next_itcas = []
+            candidate_mappings = []
+            for next_mapping in self.next_mappings(cur_mapping, self.class_type):
+                candidate_mappings.append(next_mapping)
+                self.counter += 1
+                next_itcas.append(self.compute_itca(X, y, clf, next_mapping, kfolds=kf, y_dist=y_dist))
+            # choose best mapping
+            next_ind = np.argmax([np.mean(itca) for itca in next_itcas])
+            cur_mapping = candidate_mappings[next_ind]
+            next_node = Node(next_itcas[next_ind], cur_mapping)
+            cur_node.children = [next_node]
+            cur_node = next_node
+            i += 1
+            if np.mean(cur_node.vals) > np.mean(self.selected.vals):
+                self.selected = cur_node
+            elif early_stop:
+                break
+        return self
+
+
+class GreedySearchPruned(Strategy):
+    """
+    Search the class combination map that maximizes s-ITCA by greedy algorithm.
+    Using the lower bound derived by class-wise accuracy to prune the search space.
+    """
+
+    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=True, random_state=None):
+        unique_y = np.unique(y)
+        n_classes = len(unique_y)
+        if min(y) != 0 or max(y) != n_classes - 1:
+            raise ValueError("Labels should be between 0 to K.")
+        kf = KFold(n_splits=kfolds, shuffle=True, random_state=random_state)
+        # compute y_dist
+        y_dist = compute_y_dist(y)
+        # construct identity mapping.
+        cur_mapping = bidict({key: key for key in range(n_classes)})
+        cur_itca, cur_class_acc = self.compute_itca(X, y, clf, cur_mapping, kfolds=kf, y_dist=y_dist,
+                                                    return_class_acc=True)
+        cur_y_dist = compute_y_dist(cur_mapping.map(y))
+        cur_node = Node(cur_itca, cur_mapping)
+        self.selected = cur_node
+        self.path = cur_node
+        i = 1
+        self.counter = 0
+        while len(cur_mapping.inverse) > 2:
+            # compute itac of current mapping
+            if verbose:
+                print("Round={}|Current Mapping={}".format(i, cur_mapping))
+            next_itcas = []
+            next_class_accs = []
+            candidate_mappings = []
+            for next_mapping in self.next_mappings_pruned(cur_mapping, self.class_type,
+                                                          cur_class_acc, cur_y_dist):
+                candidate_mappings.append(next_mapping)
+                self.counter += 1
+                itca, class_acc = self.compute_itca(X, y, clf, next_mapping, kfolds=kf, y_dist=y_dist,
+                                                    return_class_acc=True)
+                next_itcas.append(itca)
+                next_class_accs.append(class_acc)
+            # choose best mapping
+            if len(next_itcas) == 0:
+                break
+            else:
+                next_ind = np.argmax([np.mean(itca) for itca in next_itcas])
+                cur_mapping = candidate_mappings[next_ind]
+                cur_class_acc = next_class_accs[next_ind]
+                cur_y_dist = compute_y_dist(cur_mapping.map(y))
+                next_node = Node(next_itcas[next_ind], cur_mapping)
+                cur_node.children = [next_node]
+                cur_node = next_node
+                i += 1
+                if np.mean(cur_node.vals) > np.mean(self.selected.vals):
+                    self.selected = cur_node
+        return self
+
+
+class BFSearch(Strategy):
+    """
+    Search the class combination map that maximizes s-ITCA by breadth-first search algorithm.
+    """
+    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=False, random_state=None):
+        self.counter = 0
+
+        def bfs(visited, cur_node, kf, y_dist, i):
+            if len(cur_node.mapping.inverse) > 2:
+                for next_mapping in self.next_mappings(cur_node.mapping, self.class_type):
+                    next_fs = frozenset(next_mapping.items())
+                    if next_fs not in visited:
+                        self.counter += 1
+                        next_itca = self.compute_itca(X, y, clf, next_mapping, kf, y_dist)
+                        visited.add(next_fs)
+                        if np.mean(next_itca) > np.mean(cur_node.vals):
+                            next_node = Node(next_itca, next_mapping)
+                            cur_node.add_child(next_node)
+                            if verbose:
+                                print("Level={}|Current Mapping={}".format(i, next_mapping))
+                            if np.mean(next_itca) > np.mean(self.selected.vals):
+                                self.selected = next_node
+                            bfs(visited, next_node, kf, y_dist, i + 1)
+
+        unique_y = np.unique(y)
+        n_classes = len(unique_y)
+        if min(y) != 0 or max(y) != n_classes - 1:
+            raise ValueError("Labels should be between 0 to K.")
+        kf = KFold(n_splits=kfolds, shuffle=True, random_state=random_state)
+        # compute y_dist
+        y_dist = compute_y_dist(y)
+        # construct identity mapping.
+        cur_mapping = bidict({key: key for key in range(n_classes)})
+        cur_itca = self.compute_itca(X, y, clf, cur_mapping, kfolds=kf, y_dist=y_dist)
+        self.counter += 1
+        cur_node = Node(cur_itca, cur_mapping)
+        self.selected = cur_node
+        self.path = cur_node
+        i = 1
+        visited = set([frozenset(cur_mapping.items())])
+        # driver code
+        bfs(visited, cur_node, kf, y_dist, i)
+        self.visited = visited
+        return self
+
+
+class BFSearchPruned(Strategy):
+    """
+    Search the class combination map that maximizes s-ITCA by breadth-first search algorithm.
+    Using the lower bound derived by class-wise accuracy to prune the search space.
+    """
+    def search(self, X, y, clf, kfolds=5, verbose=False, early_stop=True, random_state=None):
+        self.counter = 0
+        unique_y = np.unique(y)
+        n_classes = len(unique_y)
+        if min(y) != 0 or max(y) != n_classes - 1:
+            raise ValueError("Labels should be between 0 to K.")
+        kf = KFold(n_splits=kfolds, shuffle=True, random_state=random_state)
+        # compute y_dist
+        y_dist = compute_y_dist(y)
+
+        def bfs(visited, cur_node, cur_class_acc, cur_ty_dist, i):
+            if len(cur_node.mapping.inverse) > 2:
+                for next_mapping in self.next_mappings_pruned(cur_node.mapping, self.class_type,
+                                                              cur_class_acc, cur_ty_dist):
+                    next_fs = frozenset(next_mapping.items())
+                    if next_fs not in visited:
+                        self.counter += 1
+                        next_itca, next_class_acc = self.compute_itca(X, y, clf, next_mapping, kf,
+                                                                      y_dist, return_class_acc=True)
+                        visited.add(next_fs)
+                        if np.mean(next_itca) > np.mean(cur_node.vals):
+                            next_node = Node(next_itca, next_mapping)
+                            cur_node.add_child(next_node)
+                            if verbose:
+                                print("Level={}|Current Mapping={}".format(i, next_mapping))
+                            if np.mean(next_itca) > np.mean(self.selected.vals):
+                                self.selected = next_node
+                            cur_ty_dist = compute_y_dist(next_node.mapping.map(y))
+                            bfs(visited, next_node, next_class_acc, cur_ty_dist, i + 1)
+
+        # construct identity mapping.
+        cur_mapping = bidict({key: key for key in range(n_classes)})
+        cur_itca, cur_class_acc = self.compute_itca(X, y, clf, cur_mapping, kfolds=kf,
+                                                    y_dist=y_dist, return_class_acc=True)
+        self.counter += 1
+        cur_node = Node(cur_itca, cur_mapping)
+        self.selected = cur_node
+        self.path = cur_node
+        i = 1
+        visited = set([frozenset(cur_mapping.items())])
+        bfs(visited, cur_node, cur_class_acc, y_dist, i)
+        self.visited = visited
+        return self
+
+if __name__ == "__main__":
+    mapping = bidict({0: 0, 1: 0, 2: 1, 3: 2, 4: 3})
+    for m in Strategy.next_mappings(mapping, "nominal"):
+        print(m.inverse)
```

### Comparing `itca-0.1.0/setup.py` & `itca-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,115 @@
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = 'itca'
-DESCRIPTION = 'A  Data-driven Criterion to Combining Ambiguous Outcome Labels in Multi-class Classification'
-URL = 'https://github.com/messcode/stagewiseNN'
-EMAIL = 'zhangchihao11@outlook.com'
-AUTHOR = 'Chihao Zhang'
-REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.0'
-
-# What packages are required for this module to be executed?
-REQUIRED = [
-    'numpy',
-    'scikit_learn',
-]
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-
-        sys.exit()
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    install_requires=REQUIRED,
-    include_package_data=True,
-    license='MIT',
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    },
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = 'itca'
+DESCRIPTION = 'A  Data-driven Criterion to Combining Ambiguous Outcome Labels in Multi-class Classification'
+URL = 'https://github.com/JSB-UCLA/ITCA'
+EMAIL = 'zhang.dabiao11@gmail.com'
+AUTHOR = 'Chihao Zhang'
+REQUIRES_PYTHON = '>=3.6.0'
+VERSION = '0.1.1'
+
+# What packages are required for this module to be executed?
+REQUIRED = [
+    'numpy',
+    'scikit_learn',
+    'networkx',
+    'matplotlib',
+    'pygraphviz',
+]
+# what packages are optional?
+EXTRAS = {'pygraphviz': ['pygraphviz']}
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+        exec(f.read(), about)
+else:
+    about['__version__'] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+
+        sys.exit()
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    package_data={'': ['datasets/*.npz']},
+    license='MIT',
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy'
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        'upload': UploadCommand,
+    },
 )
```

