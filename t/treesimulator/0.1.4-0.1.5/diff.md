# Comparing `tmp/treesimulator-0.1.4.tar.gz` & `tmp/treesimulator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/treesimulator-0.1.4.tar", last modified: Mon Jul 18 14:14:12 2022, max compression
+gzip compressed data, was "treesimulator-0.1.5.tar", last modified: Tue May 23 12:48:08 2023, max compression
```

## Comparing `treesimulator-0.1.4.tar` & `treesimulator-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 azhukova  (1001) azhukova  (1001)        0 2022-07-18 14:14:12.000000 treesimulator-0.1.4/
-drwxrwxr-x   0 azhukova  (1001) azhukova  (1001)        0 2022-07-18 14:14:12.000000 treesimulator-0.1.4/treesimulator/
--rwxrwxr-x   0 azhukova  (1001) azhukova  (1001)     5466 2022-07-18 14:13:24.000000 treesimulator-0.1.4/treesimulator/simulate_forest.py
--rw-r--r--   0 azhukova  (1001) azhukova  (1001)     1319 2022-02-23 22:12:25.000000 treesimulator-0.1.4/treesimulator/__init__.py
--rwxrwxr-x   0 azhukova  (1001) azhukova  (1001)     3959 2022-07-18 14:13:24.000000 treesimulator-0.1.4/treesimulator/simulate_forest_bdei.py
--rwxrwxr-x   0 azhukova  (1001) azhukova  (1001)    16232 2022-07-18 13:47:35.000000 treesimulator-0.1.4/treesimulator/generator.py
--rwxrwxr-x   0 azhukova  (1001) azhukova  (1001)     9201 2022-07-18 13:11:38.000000 treesimulator-0.1.4/treesimulator/mtbd_models.py
--rwxrwxr-x   0 azhukova  (1001) azhukova  (1001)     4537 2020-06-22 12:55:33.000000 treesimulator-0.1.4/treesimulator/sequence_generator.py
--rwxrwxr-x   0 azhukova  (1001) azhukova  (1001)     3773 2022-07-18 14:13:24.000000 treesimulator-0.1.4/treesimulator/simulate_forest_bd.py
--rwxrwxr-x   0 azhukova  (1001) azhukova  (1001)     4472 2022-07-18 14:13:24.000000 treesimulator-0.1.4/treesimulator/simulate_forest_bdss.py
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     7566 2022-07-18 14:14:12.000000 treesimulator-0.1.4/PKG-INFO
--rwxr-xr-x   0 azhukova  (1001) azhukova  (1001)     1303 2022-07-18 14:13:24.000000 treesimulator-0.1.4/setup.py
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)       38 2022-07-18 14:14:12.000000 treesimulator-0.1.4/setup.cfg
-drwxrwxr-x   0 azhukova  (1001) azhukova  (1001)        0 2022-07-18 14:14:12.000000 treesimulator-0.1.4/treesimulator.egg-info/
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)      234 2022-07-18 14:14:12.000000 treesimulator-0.1.4/treesimulator.egg-info/entry_points.txt
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)      505 2022-07-18 14:14:12.000000 treesimulator-0.1.4/treesimulator.egg-info/SOURCES.txt
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     7566 2022-07-18 14:14:12.000000 treesimulator-0.1.4/treesimulator.egg-info/PKG-INFO
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)       14 2022-07-18 14:14:12.000000 treesimulator-0.1.4/treesimulator.egg-info/top_level.txt
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)        1 2022-07-18 14:14:12.000000 treesimulator-0.1.4/treesimulator.egg-info/dependency_links.txt
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)       15 2022-07-18 14:14:12.000000 treesimulator-0.1.4/treesimulator.egg-info/requires.txt
--rwxr-xr-x   0 azhukova  (1001) azhukova  (1001)     5793 2022-01-31 16:51:58.000000 treesimulator-0.1.4/README.md
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-23 12:48:08.502782 treesimulator-0.1.5/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    35823 2022-12-22 13:30:01.000000 treesimulator-0.1.5/LICENSE
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2023-05-23 12:48:08.502782 treesimulator-0.1.5/PKG-INFO
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5793 2022-12-22 13:30:01.000000 treesimulator-0.1.5/README.md
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2023-05-23 12:48:08.502782 treesimulator-0.1.5/setup.cfg
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1302 2023-05-23 12:38:30.000000 treesimulator-0.1.5/setup.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-23 12:48:08.502782 treesimulator-0.1.5/treesimulator/
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1281 2023-05-23 12:45:26.000000 treesimulator-0.1.5/treesimulator/__init__.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17829 2023-05-23 12:47:02.000000 treesimulator-0.1.5/treesimulator/generator.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    10186 2023-05-23 12:38:06.000000 treesimulator-0.1.5/treesimulator/mtbd_models.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4537 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/sequence_generator.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5466 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/simulate_forest.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3883 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/simulate_forest_bd.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4069 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/simulate_forest_bdei.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4582 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/simulate_forest_bdss.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-23 12:48:08.502782 treesimulator-0.1.5/treesimulator.egg-info/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     6340 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/PKG-INFO
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)      513 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/SOURCES.txt
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        1 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/dependency_links.txt
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)      233 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/entry_points.txt
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       15 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/requires.txt
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       14 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `treesimulator-0.1.4/treesimulator/simulate_forest.py` & `treesimulator-0.1.5/treesimulator/simulate_forest.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.4/treesimulator/__init__.py` & `treesimulator-0.1.5/treesimulator/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import os
-
-STATE = 'state'
-DIST_TO_START ='D'
-TIME_TILL_NOW = 'T'
-
-
-def save_forest(forest, nwk):
-    os.makedirs(os.path.dirname(os.path.abspath(nwk)), exist_ok=True)
-    with open(nwk, 'w+') as f:
-        for tree in forest:
-            nwk = tree.write(format=5, format_root_node=True)
-            f.write('{}\n'.format(nwk))
-
-
-def save_ltt(real_ltt, observed_ltt, ltt_file):
-    os.makedirs(os.path.dirname(os.path.abspath(ltt_file)), exist_ok=True)
-    with open(ltt_file, 'w+') as f:
-        f.write('time\treal lineages\tobserved lineages\n')
-        observed = 0
-        real = 0
-        for time in sorted(set(real_ltt.keys()) | set(observed_ltt.keys())):
-            if time in observed_ltt:
-                observed = observed_ltt[time]
-            if time in real_ltt:
-                real = real_ltt[time]
-            f.write('{}\t{}\t{}\n'.format(time, real, observed))
-
-
-def save_log(model, total_tips, T, u, log):
-    res = model.get_epidemiological_parameters()
-    res['tips'] = total_tips
-    res['time'] = T
-    res['hidden_trees'] = u
-    os.makedirs(os.path.dirname(os.path.abspath(log)), exist_ok=True)
-    with open(log, 'w+') as f:
-        f.write('{}\n'.format(','.join(res.keys())))
-        f.write('{}\n'.format(','.join(str(_) for _ in res.values())))
+import os
+
+STATE = 'state'
+DIST_TO_START ='D'
+TIME_TILL_NOW = 'T'
+
+
+def save_forest(forest, nwk):
+    os.makedirs(os.path.dirname(os.path.abspath(nwk)), exist_ok=True)
+    with open(nwk, 'w+') as f:
+        for tree in forest:
+            nwk = tree.write(format=5, format_root_node=True)
+            f.write('{}\n'.format(nwk))
+
+
+def save_ltt(real_ltt, observed_ltt, ltt_file):
+    os.makedirs(os.path.dirname(os.path.abspath(ltt_file)), exist_ok=True)
+    with open(ltt_file, 'w+') as f:
+        f.write('time\treal lineages\tobserved lineages\n')
+        observed = 0
+        real = 0
+        for time in sorted(set(real_ltt.keys()) | set(observed_ltt.keys())):
+            if time in observed_ltt:
+                observed = observed_ltt[time]
+            if time in real_ltt:
+                real = real_ltt[time]
+            f.write('{}\t{}\t{}\n'.format(time, real, observed))
+
+
+def save_log(model, total_tips, T, u, log):
+    res = model.get_epidemiological_parameters()
+    res['tips'] = total_tips
+    res['time'] = T
+    res['hidden_trees'] = u
+    os.makedirs(os.path.dirname(os.path.abspath(log)), exist_ok=True)
+    with open(log, 'w+') as f:
+        f.write('{}\n'.format(','.join(res.keys())))
+        f.write('{}\n'.format(','.join(str(_) for _ in res.values())))
```

### Comparing `treesimulator-0.1.4/treesimulator/simulate_forest_bdei.py` & `treesimulator-0.1.5/treesimulator/simulate_forest_bdei.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     logging.info('BDEI model parameters are:\n\tmu={}\n\tlambda={}\n\tpsi={}\n\tp={}'
                  .format(params.mu, params.la, params.psi, params.p))
     logging.info('Total time T={}'.format(params.T))
 
     model = BirthDeathExposedInfectiousModel(p=params.p, mu=params.mu, la=params.la, psi=params.psi)
     if params.pn and params.pn > 0:
+        logging.info('PN model parameters are:\n\tpsi_n={}\n\tp_n={}'.format(params.partner_psi, params.pn))
         model = PNModel(model=model, pn=params.pn, removal_rate=params.partner_psi)
 
     forest, (total_tips, u, T), ltt = generate(model, params.min_tips, params.max_tips, T=params.T)
 
     save_forest(forest, params.nwk)
     save_log(model, total_tips, T, u, params.log)
     if params.ltt:
```

### Comparing `treesimulator-0.1.4/treesimulator/generator.py` & `treesimulator-0.1.5/treesimulator/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import logging
 import random
-from collections import Counter
+from collections import Counter, defaultdict
 
 import numpy as np
 from ete3 import TreeNode
 
 from treesimulator import STATE, DIST_TO_START, TIME_TILL_NOW
 from treesimulator.mtbd_models import PNModel
 
 
-def simulate_tree_gillespie(model, max_time=np.inf, max_sampled=np.inf,
+def simulate_tree_gillespie(model, max_time=np.inf, min_sampled=0, max_sampled=np.inf,
                             state_feature=STATE, state_frequencies=None, ltt=False):
     """
     Simulates the tree evolution from a root over the given time based on the given model.
 
     :param state_feature: a name of the tree feature which will store node states
     :param state_frequencies: array of equilibrium frequencies of model states
         (to be used to draw the root state). If not given, will be taken from the model (by default all equal).
-    :param max_sampled: maximal number of sampling node (when reached, the simulation stops), by default infinity
+    :param min_sampled: minimal number of sampled nodes (when reached, the simulation could stop), by default 0
+    :param max_sampled: maximal number of sampled nodes (when reached, the simulation stops), by default infinity
     :type max_sampled: int
     :param max_time: time over which we generate a tree, by default infinity
     :type max_time: float
     :param model: MTBD model used to simulate the tree
     :type model: treesimulator.mtbd_models.Model
     :param ltt: whether to return LTT values as well (default False)
     :type ltt: bool
@@ -44,29 +45,42 @@
     id2time = {}
     id2parent_id = {}
     sampled_id2state = {}
     donor_id2recipient_id = {}
     id2current_id = {0: 0}
     id2state = {0: root_state}
 
-    while infectious_nums.sum() and sampled_nums.sum() < max_sampled and time < max_time:
+    # logging.info('Aiming for at most {} sampled cases over time {}'.format(max_sampled, max_time))
+
+    def sampled_enough():
+        return sampled_nums.sum() >= min_sampled
+
+    if not isinstance(model, PNModel) and max_sampled != np.inf:
+        max_sampled = int(min_sampled + np.random.random() * (max_sampled + 1 - min_sampled))
+
+    def sampled_too_much():
+        return sampled_nums.sum() > max_sampled
+
+    # If there is PN, let us keep different proportions of unsampled partners depending on time and sampled numbers
+    unsampled_partner_proportion2time = defaultdict(list)
+
+    while infectious_nums.sum() and not sampled_too_much() and time < max_time:
         # first we need to calculate rate sum
         transmission_rate_sums = model.transmission_rates.sum(axis=1) * infectious_nums
         transition_rate_sums = model.transition_rates.sum(axis=1) * infectious_nums
         removal_rate_sums = model.removal_rates * infectious_nums
         total_transmission_rate = transmission_rate_sums.sum()
         total_transition_rate = transition_rate_sums.sum()
         total_removal_rate = removal_rate_sums.sum()
         total_rate = total_transmission_rate + total_transition_rate + total_removal_rate
 
-        # now let us see when next event takes place
+        # check if we passed the time limit
         time += np.random.exponential(1 / total_rate, 1)[0]
-
-        # Check if the time is up
-        if time > max_time:
+        if time >= max_time:
+            time = max_time
             break
 
         # now let us see which event will happen
         random_event = np.random.uniform(0, 1, 1)[0] * total_rate
 
         # case 1: state transition
         if random_event < total_transition_rate:
@@ -145,17 +159,28 @@
                             i = id2state[partner_id[0]]
                             id2state[partner_id[0]] = num_states - 1
                             infectious_state2id[i].remove(partner_id)
                             infectious_state2id[num_states - 1].add(partner_id)
                             infectious_nums[i] -= 1
                             infectious_nums[num_states - 1] += 1
                             # print('\tand notified {} (in state {})'.format(partner_id, model.states[i]))
+
+                # if we could already stop, let's update unsampled partner proportion for this time
+                if sampled_enough() and isinstance(model, PNModel):
+                    unsampled_partner_proportion2time[infectious_nums[-1] / sampled_nums[-1] if sampled_nums[-1] else 1]\
+                        .append(time)
                 break
             random_event -= removal_rate_sums[i]
 
+    if isinstance(model, PNModel) and unsampled_partner_proportion2time:
+        min_unsampled_proportion = min(unsampled_partner_proportion2time.keys())
+        logging.info('At the end of the sampling period {:g}% of notified partners stayed unobserved'
+                     .format(min_unsampled_proportion * 100))
+        time = np.random.choice(unsampled_partner_proportion2time[min_unsampled_proportion], 1)[0]
+
     if max_time == np.inf:
         max_time = time
 
     root = reconstruct_tree(id2parent_id, id2time, sampled_id2state, max_time, state_feature=state_feature)
     if ltt:
         return root, reconstruct_ltt(id2parent_id, id2time)
     return root
@@ -165,14 +190,18 @@
     if not sampled_id2state:
         return None
 
     root = None
     id2node = {}
     for node_id, state in sampled_id2state.items():
         time = id2time[node_id]
+        # if there is PN it could be
+        # that we decided to stop at an earlier time when the unsampled partner proportion was lower
+        if time > max_time:
+            continue
         node = TreeNode(dist=time - (0 if node_id not in id2parent else id2time[id2parent[node_id]]), name=node_id[0])
         node.add_feature(DIST_TO_START, time)
         node.add_feature(state_feature, state)
         id2node[node_id] = node
         while node is not None and node_id in id2parent:
             parent_id = id2parent[node_id]
             if parent_id in id2node:
@@ -331,16 +360,15 @@
                 logging.info('Generated a forest of {} visible and {} hidden trees with {} sampled tips over time {}.'
                              .format(fl, u, total_tips, T))
                 return forest, (total_tips, u, T), ltt
             logging.debug('Generated a forest of {} visible and {} hidden trees with {} sampled tips over time {}.'
                           .format(fl, u, total_tips, T))
     else:
         while True:
-            max_sampled = int(min_tips + np.random.random() * (max_tips + 1 - min_tips))
-            tree, ltt = simulate_tree_gillespie(model, max_time=np.inf, max_sampled=max_sampled,
+            tree, ltt = simulate_tree_gillespie(model, max_time=np.inf, max_sampled=max_tips, min_sampled=min_tips,
                                                 state_frequencies=state_frequencies, ltt=True)
             total_tips = len(tree) if tree else 0
             if total_tips >= min_tips:
                 logging.info('Generated a tree with {} sampled tips over time {}.'
                              .format(total_tips, getattr(tree, TIME_TILL_NOW) if tree else np.inf))
                 return [tree], (total_tips, 0, getattr(tree, TIME_TILL_NOW) + tree.dist), ltt
             logging.debug('Generated a tree with {} sampled tips over time {}.'
```

### Comparing `treesimulator-0.1.4/treesimulator/mtbd_models.py` & `treesimulator-0.1.5/treesimulator/mtbd_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import numpy as np
+from scipy.optimize import fsolve
 
 EXPOSED = 'e'
 INFECTED = 'i'
 SUPERSPREADER = 's'
 
-
 SAMPLING = 'sampling'
 TRANSMISSION = 'transmission'
 TRANSITION = 'transition'
 
 
 class Model(object):
+
     def __init__(self, states=None,
-                 transition_rates=None, transmission_rates=None, removal_rates=None, ps=None,
-                 state_frequencies=None, *args, **kwargs):
+                 transition_rates=None, transmission_rates=None, removal_rates=None, ps=None, *args, **kwargs):
         super(Model, self).__init__()
         self.__states = np.array(states)
         num_states = len(self.states)
-        self.__state_freqs = ((1 / num_states) * np.ones(num_states, dtype=float)) \
-            if state_frequencies is None else np.array(state_frequencies)
         self.__ps = np.array(ps) if ps is not None else np.ones(num_states, dtype=float)
         self.__transmission_rates = np.array(transmission_rates) if transmission_rates is not None \
             else np.zeros(shape=(num_states, num_states), dtype=np.float)
         self.__transition_rates = np.array(transition_rates) if transition_rates is not None \
             else np.zeros(shape=(num_states, num_states), dtype=np.float)
         self.__removal_rates = np.array(removal_rates) if removal_rates is not None \
             else np.zeros(shape=num_states, dtype=np.float)
@@ -31,65 +29,95 @@
     def clone(self):
         return Model(self.states, self.transition_rates, self.transmission_rates, self.removal_rates, self.ps)
 
     @property
     def ps(self):
         return self.__ps
 
+    @ps.setter
+    def ps(self, ps):
+        self.__ps = ps
+
     @property
     def states(self):
         return self.__states
 
     @property
     def state_frequencies(self):
-        return self.__state_freqs
+        MU, LA, PSI = self.transition_rates, self.transmission_rates, self.removal_rates
+        m = len(self.states)
+
+        def func(PI):
+            SIGMA = PI.dot(LA.sum(axis=1) - PSI)
+            res = [PI.sum() - 1]
+            for k in range(m - 1):
+                pi_k = PI[k]
+                res.append(pi_k * SIGMA + pi_k * (PSI[k] + MU[k, :].sum()) - PI.dot(MU[:, k] + LA[:, k]))
+            return res
+
+        PI = fsolve(func, np.ones(m) / m)
+        if np.any(PI < 0) or np.any(PI > 1):
+            return np.ones(m) / m
+        return PI
 
     @property
     def transition_rates(self):
         """
         Get transition rate matrix with states as columns and rows.
 
         :return rate array
         :rtype np.array
         """
         return self.__transition_rates
 
+    @transition_rates.setter
+    def transition_rates(self, rates):
+        self.__transition_rates = rates
+
     @property
     def transmission_rates(self):
         """
         Get transmission rate matrix with states as columns and rows.
 
         :return rate array
         :rtype np.array
         """
         return self.__transmission_rates
 
+    @transmission_rates.setter
+    def transmission_rates(self, rates):
+        self.__transmission_rates = rates
+
     @property
     def removal_rates(self):
         """
         Get removal rate array with states as columns.
 
         :return rate array
         :rtype np.array
         """
         return self.__removal_rates
 
+    @removal_rates.setter
+    def removal_rates(self, rates):
+        self.__removal_rates = rates
+
     def get_name(self):
         return 'MTBD'
 
     def check_rates(self):
         n_states = len(self.states)
-        assert(self.transition_rates.shape == (n_states, n_states))
-        assert(self.transmission_rates.shape == (n_states, n_states))
-        assert(self.removal_rates.shape == (n_states,))
-        assert(self.ps.shape == (n_states,))
-        assert(np.all(self.transition_rates >= 0))
-        assert(np.all(self.transmission_rates >= 0))
-        assert(np.all(self.removal_rates >= 0))
-        assert(np.all(self.ps >= 0) and np.all(self.ps <= 1))
+        assert (self.transition_rates.shape == (n_states, n_states))
+        assert (self.transmission_rates.shape == (n_states, n_states))
+        assert (self.removal_rates.shape == (n_states,))
+        assert (self.ps.shape == (n_states,))
+        assert (np.all(self.transition_rates >= 0))
+        assert (np.all(self.transmission_rates >= 0))
+        assert (np.all(self.removal_rates >= 0))
+        assert (np.all(self.ps >= 0) and np.all(self.ps <= 1))
 
     def get_epidemiological_parameters(self):
         """Converts rate parameters to the epidemiological ones"""
         return {'transitions': self.transition_rates, 'transmissions': self.transmission_rates,
                 'removals': self.removal_rates, 'sampling': self.ps}
 
 
@@ -105,27 +133,31 @@
         mus = np.zeros(shape=(2, 2), dtype=np.float)
         mus[0, 1] = mu
         las = np.zeros(shape=(2, 2), dtype=np.float)
         las[1, 0] = la
         psis = np.zeros(shape=2, dtype=np.float)
         psis[1] = psi
 
+        Model.__init__(self, states=[EXPOSED, INFECTED],
+                       transition_rates=mus, transmission_rates=las, removal_rates=psis, ps=[0, p],
+                       *args, **kwargs)
+
+    @property
+    def state_frequencies(self):
+        mu = self.transition_rates[0, 1]
+        la = self.transmission_rates[1, 0]
+        psi = self.removal_rates[1]
         mu_plus_psi = mu + psi
         if la == psi:
             pi_i = mu / mu_plus_psi
         else:
             two_la_minus_psi = 2 * (la - psi)
             det = np.power(np.power(mu_plus_psi, 2) + 2 * mu * two_la_minus_psi, 1 / 2)
             pi_i = (det - mu_plus_psi) / two_la_minus_psi
-            if pi_i < 0 or pi_i > 1:
-                pi_i = (-det - mu_plus_psi) / two_la_minus_psi
-
-        Model.__init__(self, states=[EXPOSED, INFECTED],
-                       transition_rates=mus, transmission_rates=las, removal_rates=psis, ps=[0, p],
-                       state_frequencies=[1 - pi_i, pi_i], *args, **kwargs)
+        return np.array([1 - pi_i, pi_i])
 
     def get_name(self):
         return 'BDEI'
 
     def get_epidemiological_parameters(self):
         """Converts rate parameters to the epidemiological ones"""
         return {'R0': self.transmission_rates[1, 0] / self.removal_rates[1],
@@ -174,25 +206,30 @@
                 'transmission ratio constraint is violated: la_ss / la_ns ({}) must be equal to la_sn / la_nn ({})'
                     .format(s_ratio, n_ratio))
         las[0, 0] = la_nn
         las[0, 1] = la_ns
         las[1, 0] = la_sn
         las[1, 1] = la_ss
         psis = psi * np.ones(shape=2, dtype=np.float)
-        f = la_ss / (la_ss + la_sn)
         Model.__init__(self, states=[INFECTED, SUPERSPREADER],
-                       transmission_rates=las, removal_rates=psis, ps=[p, p],
-                       state_frequencies=[1 - f, f], *args, **kwargs)
+                       transmission_rates=las, removal_rates=psis, ps=[p, p], *args, **kwargs)
+
+    @property
+    def state_frequencies(self):
+        la_ss = self.transmission_rates[1, 1]
+        la_sn = self.transmission_rates[1, 0]
+        f = la_ss / (la_ss + la_sn)
+        return np.array([1 - f, f])
 
     def get_name(self):
         return 'BDSS'
 
     def get_epidemiological_parameters(self):
         """Converts rate parameters to the epidemiological ones"""
-        return {'R0': (self.transmission_rates[0, 0] + self.transition_rates[1, 1]) / self.removal_rates[0],
+        return {'R0': (self.transmission_rates[0, 0] + self.transmission_rates[1, 1]) / self.removal_rates[0],
                 'infectious time': 1 / self.removal_rates[1],
                 'sampling probability': self.ps[1],
                 'superspreading transmission ratio': self.transmission_rates[1, 1] / self.transmission_rates[0, 1],
                 'superspreading fraction':
                     self.transmission_rates[1, 1] / (self.transmission_rates[1, 1] + self.transmission_rates[1, 0])}
 
 
@@ -228,14 +265,14 @@
         """
         return self.removal_rates[-1]
 
     def get_name(self):
         return self.model.get_name() + '-PN'
 
     def check_p(self):
-        assert(0 <= self.__pn <= 1)
+        assert (0 <= self.__pn <= 1)
 
     def get_epidemiological_parameters(self):
         res = self.model.get_epidemiological_parameters()
         res['notification probability'] = self.pn
         res['removal time after notification'] = 1 / self.removal_rates[-1]
         return res
```

### Comparing `treesimulator-0.1.4/treesimulator/sequence_generator.py` & `treesimulator-0.1.5/treesimulator/sequence_generator.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.4/treesimulator/simulate_forest_bd.py` & `treesimulator-0.1.5/treesimulator/simulate_forest_bd.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     logging.basicConfig(level=logging.INFO, format='%(asctime)s: %(message)s', datefmt="%Y-%m-%d %H:%M:%S")
 
     logging.info('BD model parameters are:\n\tlambda={}\n\tpsi={}\n\tp={}'.format(params.la, params.psi, params.p))
     logging.info('Total time T={}'.format(params.T))
 
     model = BirthDeathModel(p=params.p, la=params.la, psi=params.psi)
     if params.pn and params.pn > 0:
+        logging.info('PN model parameters are:\n\tpsi_n={}\n\tp_n={}'.format(params.partner_psi, params.pn))
         model = PNModel(model=model, pn=params.pn, removal_rate=params.partner_psi)
 
     forest, (total_tips, u, T), ltt = generate(model, params.min_tips, params.max_tips, T=params.T)
 
     save_forest(forest, params.nwk)
     save_log(model, total_tips, T, u, params.log)
     if params.ltt:
```

### Comparing `treesimulator-0.1.4/treesimulator/simulate_forest_bdss.py` & `treesimulator-0.1.5/treesimulator/simulate_forest_bdss.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
                  .format(params.la_ss, params.la_sn, params.la_ns, params.la_nn, params.psi, params.p))
     logging.info('Total time T={}'.format(params.T))
 
     model = BirthDeathWithSuperSpreadingModel(p=params.p,
                                               la_ss=params.la_ss, la_sn=params.la_sn,
                                               la_ns=params.la_ns, la_nn=params.la_nn, psi=params.psi)
     if params.pn and params.pn > 0:
+        logging.info('PN model parameters are:\n\tpsi_n={}\n\tp_n={}'.format(params.partner_psi, params.pn))
         model = PNModel(model=model, pn=params.pn, removal_rate=params.partner_psi)
 
     forest, (total_tips, u, T), ltt = generate(model, params.min_tips, params.max_tips, T=params.T)
 
     save_forest(forest, params.nwk)
     save_log(model, total_tips, T, u, params.log)
     if params.ltt:
```

### Comparing `treesimulator-0.1.4/PKG-INFO` & `treesimulator-0.1.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,168 +1,168 @@
 Metadata-Version: 2.1
 Name: treesimulator
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.
-Home-page: https://gitlab.pasteur.fr/phylo/treesimulator
+Home-page: https://github.com/evolbioinfo/treesimulator
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
-License: UNKNOWN
-Description: # treesimulator
-        
-        Simulation of rooted phylogenetic trees under a given Multitype Birth–Death (MTBD) model.
-        The MTBD models were introduced by Stadler & Bonhoeffer [[_Philos. Trans. R. Soc. B_ 2013]](https://royalsocietypublishing.org/doi/10.1098/rstb.2012.0198).
-        
-        We pay particular interest to the classical BD model, the BD Exposed-Infectious (BDEI) model, 
-        and BD with superspreading (BDSS), 
-        as they are described in [[Voznica _et al._ 2021]]((https://www.biorxiv.org/content/10.1101/2021.03.11.435006v1)). 
-        
-        ## BD
-        3 parameters:
-        * λ -- transmission rate
-        * ψ -- removal rate
-        * p -- sampling probability upon removal
-        
-        Epidemiological parameters:
-        * R<sub>0</sub>=λ/ψ -- reproduction number
-        * 1/ψ -- infectious time
-        
-        ## BDEI
-        2 compartments: 
-        * E, exposed, i.e. infected but not yet infectious
-        * I, infectious
-        
-        4 parameters:
-        * μ -- transition rate from E to I (becoming infectious)
-        * λ -- transmission rate from I to E
-        * ψ -- removal rate of I
-        * p -- sampling probability upon removal
-        
-        Epidemiological parameters:
-        * R<sub>0</sub>=λ/ψ -- reproduction number
-        * 1/ψ -- infectious time
-        * 1/μ -- incubation period
-        
-        ## BDSS
-        2 compartments: 
-        * N, standard infectious individual
-        * S, superspreader
-        
-        6 parameters:
-        * λ<sub>nn</sub> -- transmission rate from N to N
-        * λ<sub>ns</sub> -- transmission rate from N to S
-        * λ<sub>sn</sub> -- transmission rate from S to N
-        * λ<sub>ss</sub> -- transmission rate from S to S
-        
-            (with a constraint that λ<sub>ss</sub>/λ<sub>ns</sub>=λ<sub>sn</sub>/λ<sub>nn</sub>)
-        * ψ -- removal rate of S and of N (the same)
-        * p -- sampling probability upon removal (the same for N and S)
-        
-        
-        
-        Epidemiological parameters:
-        * R<sub>0</sub>=(λ<sub>nn</sub> + λ<sub>ss</sub>)/ψ -- reproduction number
-        * 1/ψ -- infectious time
-        * X=λ<sub>ss</sub>/λ<sub>ns</sub>=λ<sub>sn</sub>/λ<sub>nn</sub> -- super-spreading transmission ratio
-        * f=λ<sub>ss</sub>/(λ<sub>sn</sub> + λ<sub>ss</sub>) -- super-spreading fraction
-        
-        ## Installation
-        To install treesimulator:
-        ```bash
-        pip3 install treesimulator
-        ```
-        
-        ## Usage
-        ### Command line 
-        
-        ## BD
-        The following command simulates a tree with 200-500 tips under BD model, with λ=0.5, ψ=0.25, p=0.5, 
-        and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
-        ```bash
-        generate_bd --min_tips 200 --max_tips 500 --la 0.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
-        ```
-        To seee detailed options, run:
-        ```bash
-        generate_bd --help
-        ```
-        
-        ## BDEI
-        The following command simulates a tree with 200-500 tips under BDEI model, with μ=1, λ=0.5, ψ=0.25, p=0.5, 
-        and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
-        ```bash
-        generate_bdei --min_tips 200 --max_tips 500 --mu 1 --la 0.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
-        ```
-        To seee detailed options, run:
-        ```bash
-        generate_bdei --help
-        ```
-        
-        
-        ## BDSS
-        The following command simulates a tree with 200-500 tips under BDSS model, 
-        with λ<sub>nn</sub>=0.1, λ<sub>ns</sub>=0.3, λ<sub>sn</sub>=0.5, λ<sub>ss</sub>=1.5, ψ=0.25, p=0.5, 
-        and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
-        ```bash
-        generate_bdss --min_tips 200 --max_tips 500 --la_nn 0.1 --la_ns 0.3 --la_sn 0.5 --la_ss 1.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
-        ```
-        To seee detailed options, run:
-        ```bash
-        generate_bdss --help
-        ```
-        
-        ## User-defined MTBD model
-        The following command simulates a tree with 200-500 tips under a generic MTBD model, with two states A and B, 
-        with μ<sub>aa</sub>=0.5, μ<sub>ab</sub>=0.6, μ<sub>ba</sub>=0.7, μ<sub>bb</sub>=0.8, 
-        λ<sub>aa</sub>=0.1, λ<sub>ab</sub>=0.2, λ<sub>ba</sub>=0.3, λ<sub>bb</sub>=0.4, 
-        ψ<sub>a</sub>=0.05, ψ<sub>b</sub>=0.08,
-        p=<sub>a</sub>0.15, p=<sub>b</sub>0.65,
-        and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
-        ```bash
-        generate_mtbd --min_tips 200 --max_tips 500 --nwk tree.nwk --log params.csv \
-        --states A B \
-        --transition_rates 0.5 0.6 0.7 0.8 \
-        --transmission_rates 0.1 0.2 0.3 0.4 \
-        --removal_rates 0.05 0.08 \
-        --sampling_probabilities 0.15 0.65
-        ```
-        To seee detailed options, run:
-        ```bash
-        generate_mtbd --help
-        ```
-        
-        
-        ### Python3
-        To simulate trees with 200-500 tips under the above models and settings:
-        ```python
-        from treesimulator.generator import generate
-        from treesimulator import save_forest
-        from treesimulator.mtbd_models import Model, BirthDeathModel, BirthDeathExposedInfectiousModel, BirthDeathWithSuperSpreadingModel
-        
-        bd_model = BirthDeathModel(p=0.5, la=0.5, psi=0.25)
-        print(bd_model.get_epidemiological_parameters())
-        [bd_tree], (bd_total_tips, _, bd_total_time) = generate(bd_model, min_tips=200, max_tips=500)
-        save_forest([bd_tree], 'BD_tree.nwk')
-        
-        bdei_model = BirthDeathExposedInfectiousModel(p=0.5, mu=1, la=0.5, psi=0.25)
-        print(bdei_model.get_epidemiological_parameters())
-        [bdei_tree], (bdei_total_tips, _, bdei_total_time) = generate(bdei_model, min_tips=200, max_tips=500)
-        save_forest([bdei_tree], 'BDEI_tree.nwk')
-        
-        bdss_model = BirthDeathWithSuperSpreadingModel(p=0.5, la_nn=0.1, la_ns=0.3, la_sn=0.5, la_ss=1.5, psi=0.25)
-        print(bdss_model.get_epidemiological_parameters())
-        [bdss_tree], (bdss_total_tips, _, bdss_total_time) = generate(bdss_model, min_tips=200, max_tips=500)
-        save_forest([bdss_tree], 'BDSS_tree.nwk')
-        
-        mtbd_model = Model(states=['A', 'B'], transition_rates=[[0.5, 0.6], [0.7, 0.8]], 
-                           transmission_rates=[[0.1, 0.2], [0.3, 0.4]],
-                           removal_rates=[0.05, 0.08], ps=[0.15, 0.65])
-        [mtbd_tree], (mtbd_total_tips, _, mtbd_total_time) = generate(mtbd_model, min_tips=200, max_tips=500)
-        save_forest([mtbd_tree], 'MTBD_tree.nwk')
-        ```
 Keywords: phylogenetics,tree generator,multitype birth-death model
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# treesimulator
+
+Simulation of rooted phylogenetic trees under a given Multitype Birth–Death (MTBD) model.
+The MTBD models were introduced by Stadler & Bonhoeffer [[_Philos. Trans. R. Soc. B_ 2013]](https://royalsocietypublishing.org/doi/10.1098/rstb.2012.0198).
+
+We pay particular interest to the classical BD model, the BD Exposed-Infectious (BDEI) model, 
+and BD with superspreading (BDSS), 
+as they are described in [[Voznica _et al._ 2021]]((https://www.biorxiv.org/content/10.1101/2021.03.11.435006v1)). 
+
+## BD
+3 parameters:
+* λ -- transmission rate
+* ψ -- removal rate
+* p -- sampling probability upon removal
+
+Epidemiological parameters:
+* R<sub>0</sub>=λ/ψ -- reproduction number
+* 1/ψ -- infectious time
+
+## BDEI
+2 compartments: 
+* E, exposed, i.e. infected but not yet infectious
+* I, infectious
+
+4 parameters:
+* μ -- transition rate from E to I (becoming infectious)
+* λ -- transmission rate from I to E
+* ψ -- removal rate of I
+* p -- sampling probability upon removal
+
+Epidemiological parameters:
+* R<sub>0</sub>=λ/ψ -- reproduction number
+* 1/ψ -- infectious time
+* 1/μ -- incubation period
+
+## BDSS
+2 compartments: 
+* N, standard infectious individual
+* S, superspreader
+
+6 parameters:
+* λ<sub>nn</sub> -- transmission rate from N to N
+* λ<sub>ns</sub> -- transmission rate from N to S
+* λ<sub>sn</sub> -- transmission rate from S to N
+* λ<sub>ss</sub> -- transmission rate from S to S
+
+    (with a constraint that λ<sub>ss</sub>/λ<sub>ns</sub>=λ<sub>sn</sub>/λ<sub>nn</sub>)
+* ψ -- removal rate of S and of N (the same)
+* p -- sampling probability upon removal (the same for N and S)
+
+
+
+Epidemiological parameters:
+* R<sub>0</sub>=(λ<sub>nn</sub> + λ<sub>ss</sub>)/ψ -- reproduction number
+* 1/ψ -- infectious time
+* X=λ<sub>ss</sub>/λ<sub>ns</sub>=λ<sub>sn</sub>/λ<sub>nn</sub> -- super-spreading transmission ratio
+* f=λ<sub>ss</sub>/(λ<sub>sn</sub> + λ<sub>ss</sub>) -- super-spreading fraction
+
+## Installation
+To install treesimulator:
+```bash
+pip3 install treesimulator
+```
+
+## Usage
+### Command line 
+
+## BD
+The following command simulates a tree with 200-500 tips under BD model, with λ=0.5, ψ=0.25, p=0.5, 
+and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
+```bash
+generate_bd --min_tips 200 --max_tips 500 --la 0.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
+```
+To seee detailed options, run:
+```bash
+generate_bd --help
+```
+
+## BDEI
+The following command simulates a tree with 200-500 tips under BDEI model, with μ=1, λ=0.5, ψ=0.25, p=0.5, 
+and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
+```bash
+generate_bdei --min_tips 200 --max_tips 500 --mu 1 --la 0.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
+```
+To seee detailed options, run:
+```bash
+generate_bdei --help
+```
+
+
+## BDSS
+The following command simulates a tree with 200-500 tips under BDSS model, 
+with λ<sub>nn</sub>=0.1, λ<sub>ns</sub>=0.3, λ<sub>sn</sub>=0.5, λ<sub>ss</sub>=1.5, ψ=0.25, p=0.5, 
+and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
+```bash
+generate_bdss --min_tips 200 --max_tips 500 --la_nn 0.1 --la_ns 0.3 --la_sn 0.5 --la_ss 1.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
+```
+To seee detailed options, run:
+```bash
+generate_bdss --help
+```
+
+## User-defined MTBD model
+The following command simulates a tree with 200-500 tips under a generic MTBD model, with two states A and B, 
+with μ<sub>aa</sub>=0.5, μ<sub>ab</sub>=0.6, μ<sub>ba</sub>=0.7, μ<sub>bb</sub>=0.8, 
+λ<sub>aa</sub>=0.1, λ<sub>ab</sub>=0.2, λ<sub>ba</sub>=0.3, λ<sub>bb</sub>=0.4, 
+ψ<sub>a</sub>=0.05, ψ<sub>b</sub>=0.08,
+p=<sub>a</sub>0.15, p=<sub>b</sub>0.65,
+and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
+```bash
+generate_mtbd --min_tips 200 --max_tips 500 --nwk tree.nwk --log params.csv \
+--states A B \
+--transition_rates 0.5 0.6 0.7 0.8 \
+--transmission_rates 0.1 0.2 0.3 0.4 \
+--removal_rates 0.05 0.08 \
+--sampling_probabilities 0.15 0.65
+```
+To seee detailed options, run:
+```bash
+generate_mtbd --help
+```
+
+
+### Python3
+To simulate trees with 200-500 tips under the above models and settings:
+```python
+from treesimulator.generator import generate
+from treesimulator import save_forest
+from treesimulator.mtbd_models import Model, BirthDeathModel, BirthDeathExposedInfectiousModel, BirthDeathWithSuperSpreadingModel
+
+bd_model = BirthDeathModel(p=0.5, la=0.5, psi=0.25)
+print(bd_model.get_epidemiological_parameters())
+[bd_tree], (bd_total_tips, _, bd_total_time) = generate(bd_model, min_tips=200, max_tips=500)
+save_forest([bd_tree], 'BD_tree.nwk')
+
+bdei_model = BirthDeathExposedInfectiousModel(p=0.5, mu=1, la=0.5, psi=0.25)
+print(bdei_model.get_epidemiological_parameters())
+[bdei_tree], (bdei_total_tips, _, bdei_total_time) = generate(bdei_model, min_tips=200, max_tips=500)
+save_forest([bdei_tree], 'BDEI_tree.nwk')
+
+bdss_model = BirthDeathWithSuperSpreadingModel(p=0.5, la_nn=0.1, la_ns=0.3, la_sn=0.5, la_ss=1.5, psi=0.25)
+print(bdss_model.get_epidemiological_parameters())
+[bdss_tree], (bdss_total_tips, _, bdss_total_time) = generate(bdss_model, min_tips=200, max_tips=500)
+save_forest([bdss_tree], 'BDSS_tree.nwk')
+
+mtbd_model = Model(states=['A', 'B'], transition_rates=[[0.5, 0.6], [0.7, 0.8]], 
+                   transmission_rates=[[0.1, 0.2], [0.3, 0.4]],
+                   removal_rates=[0.05, 0.08], ps=[0.15, 0.65])
+[mtbd_tree], (mtbd_total_tips, _, mtbd_total_time) = generate(mtbd_model, min_tips=200, max_tips=500)
+save_forest([mtbd_tree], 'MTBD_tree.nwk')
+```
```

### Comparing `treesimulator-0.1.4/setup.py` & `treesimulator-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    version='0.1.4',
+    version='0.1.5',
     description='Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.',
     author='Anna Zhukova',
     author_email='anna.zhukova@pasteur.fr',
-    url='https://gitlab.pasteur.fr/phylo/treesimulator',
+    url='https://github.com/evolbioinfo/treesimulator',
     keywords=['phylogenetics', 'tree generator', 'multitype birth-death model'],
     install_requires=['six', 'ete3', 'numpy'],
     entry_points={
             'console_scripts': [
                 'generate_bd = treesimulator.simulate_forest_bd:main',
                 'generate_bdei = treesimulator.simulate_forest_bdei:main',
                 'generate_bdss = treesimulator.simulate_forest_bdss:main',
```

### Comparing `treesimulator-0.1.4/treesimulator.egg-info/PKG-INFO` & `treesimulator-0.1.5/treesimulator.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,168 +1,168 @@
 Metadata-Version: 2.1
 Name: treesimulator
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.
-Home-page: https://gitlab.pasteur.fr/phylo/treesimulator
+Home-page: https://github.com/evolbioinfo/treesimulator
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
-License: UNKNOWN
-Description: # treesimulator
-        
-        Simulation of rooted phylogenetic trees under a given Multitype Birth–Death (MTBD) model.
-        The MTBD models were introduced by Stadler & Bonhoeffer [[_Philos. Trans. R. Soc. B_ 2013]](https://royalsocietypublishing.org/doi/10.1098/rstb.2012.0198).
-        
-        We pay particular interest to the classical BD model, the BD Exposed-Infectious (BDEI) model, 
-        and BD with superspreading (BDSS), 
-        as they are described in [[Voznica _et al._ 2021]]((https://www.biorxiv.org/content/10.1101/2021.03.11.435006v1)). 
-        
-        ## BD
-        3 parameters:
-        * λ -- transmission rate
-        * ψ -- removal rate
-        * p -- sampling probability upon removal
-        
-        Epidemiological parameters:
-        * R<sub>0</sub>=λ/ψ -- reproduction number
-        * 1/ψ -- infectious time
-        
-        ## BDEI
-        2 compartments: 
-        * E, exposed, i.e. infected but not yet infectious
-        * I, infectious
-        
-        4 parameters:
-        * μ -- transition rate from E to I (becoming infectious)
-        * λ -- transmission rate from I to E
-        * ψ -- removal rate of I
-        * p -- sampling probability upon removal
-        
-        Epidemiological parameters:
-        * R<sub>0</sub>=λ/ψ -- reproduction number
-        * 1/ψ -- infectious time
-        * 1/μ -- incubation period
-        
-        ## BDSS
-        2 compartments: 
-        * N, standard infectious individual
-        * S, superspreader
-        
-        6 parameters:
-        * λ<sub>nn</sub> -- transmission rate from N to N
-        * λ<sub>ns</sub> -- transmission rate from N to S
-        * λ<sub>sn</sub> -- transmission rate from S to N
-        * λ<sub>ss</sub> -- transmission rate from S to S
-        
-            (with a constraint that λ<sub>ss</sub>/λ<sub>ns</sub>=λ<sub>sn</sub>/λ<sub>nn</sub>)
-        * ψ -- removal rate of S and of N (the same)
-        * p -- sampling probability upon removal (the same for N and S)
-        
-        
-        
-        Epidemiological parameters:
-        * R<sub>0</sub>=(λ<sub>nn</sub> + λ<sub>ss</sub>)/ψ -- reproduction number
-        * 1/ψ -- infectious time
-        * X=λ<sub>ss</sub>/λ<sub>ns</sub>=λ<sub>sn</sub>/λ<sub>nn</sub> -- super-spreading transmission ratio
-        * f=λ<sub>ss</sub>/(λ<sub>sn</sub> + λ<sub>ss</sub>) -- super-spreading fraction
-        
-        ## Installation
-        To install treesimulator:
-        ```bash
-        pip3 install treesimulator
-        ```
-        
-        ## Usage
-        ### Command line 
-        
-        ## BD
-        The following command simulates a tree with 200-500 tips under BD model, with λ=0.5, ψ=0.25, p=0.5, 
-        and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
-        ```bash
-        generate_bd --min_tips 200 --max_tips 500 --la 0.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
-        ```
-        To seee detailed options, run:
-        ```bash
-        generate_bd --help
-        ```
-        
-        ## BDEI
-        The following command simulates a tree with 200-500 tips under BDEI model, with μ=1, λ=0.5, ψ=0.25, p=0.5, 
-        and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
-        ```bash
-        generate_bdei --min_tips 200 --max_tips 500 --mu 1 --la 0.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
-        ```
-        To seee detailed options, run:
-        ```bash
-        generate_bdei --help
-        ```
-        
-        
-        ## BDSS
-        The following command simulates a tree with 200-500 tips under BDSS model, 
-        with λ<sub>nn</sub>=0.1, λ<sub>ns</sub>=0.3, λ<sub>sn</sub>=0.5, λ<sub>ss</sub>=1.5, ψ=0.25, p=0.5, 
-        and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
-        ```bash
-        generate_bdss --min_tips 200 --max_tips 500 --la_nn 0.1 --la_ns 0.3 --la_sn 0.5 --la_ss 1.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
-        ```
-        To seee detailed options, run:
-        ```bash
-        generate_bdss --help
-        ```
-        
-        ## User-defined MTBD model
-        The following command simulates a tree with 200-500 tips under a generic MTBD model, with two states A and B, 
-        with μ<sub>aa</sub>=0.5, μ<sub>ab</sub>=0.6, μ<sub>ba</sub>=0.7, μ<sub>bb</sub>=0.8, 
-        λ<sub>aa</sub>=0.1, λ<sub>ab</sub>=0.2, λ<sub>ba</sub>=0.3, λ<sub>bb</sub>=0.4, 
-        ψ<sub>a</sub>=0.05, ψ<sub>b</sub>=0.08,
-        p=<sub>a</sub>0.15, p=<sub>b</sub>0.65,
-        and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
-        ```bash
-        generate_mtbd --min_tips 200 --max_tips 500 --nwk tree.nwk --log params.csv \
-        --states A B \
-        --transition_rates 0.5 0.6 0.7 0.8 \
-        --transmission_rates 0.1 0.2 0.3 0.4 \
-        --removal_rates 0.05 0.08 \
-        --sampling_probabilities 0.15 0.65
-        ```
-        To seee detailed options, run:
-        ```bash
-        generate_mtbd --help
-        ```
-        
-        
-        ### Python3
-        To simulate trees with 200-500 tips under the above models and settings:
-        ```python
-        from treesimulator.generator import generate
-        from treesimulator import save_forest
-        from treesimulator.mtbd_models import Model, BirthDeathModel, BirthDeathExposedInfectiousModel, BirthDeathWithSuperSpreadingModel
-        
-        bd_model = BirthDeathModel(p=0.5, la=0.5, psi=0.25)
-        print(bd_model.get_epidemiological_parameters())
-        [bd_tree], (bd_total_tips, _, bd_total_time) = generate(bd_model, min_tips=200, max_tips=500)
-        save_forest([bd_tree], 'BD_tree.nwk')
-        
-        bdei_model = BirthDeathExposedInfectiousModel(p=0.5, mu=1, la=0.5, psi=0.25)
-        print(bdei_model.get_epidemiological_parameters())
-        [bdei_tree], (bdei_total_tips, _, bdei_total_time) = generate(bdei_model, min_tips=200, max_tips=500)
-        save_forest([bdei_tree], 'BDEI_tree.nwk')
-        
-        bdss_model = BirthDeathWithSuperSpreadingModel(p=0.5, la_nn=0.1, la_ns=0.3, la_sn=0.5, la_ss=1.5, psi=0.25)
-        print(bdss_model.get_epidemiological_parameters())
-        [bdss_tree], (bdss_total_tips, _, bdss_total_time) = generate(bdss_model, min_tips=200, max_tips=500)
-        save_forest([bdss_tree], 'BDSS_tree.nwk')
-        
-        mtbd_model = Model(states=['A', 'B'], transition_rates=[[0.5, 0.6], [0.7, 0.8]], 
-                           transmission_rates=[[0.1, 0.2], [0.3, 0.4]],
-                           removal_rates=[0.05, 0.08], ps=[0.15, 0.65])
-        [mtbd_tree], (mtbd_total_tips, _, mtbd_total_time) = generate(mtbd_model, min_tips=200, max_tips=500)
-        save_forest([mtbd_tree], 'MTBD_tree.nwk')
-        ```
 Keywords: phylogenetics,tree generator,multitype birth-death model
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# treesimulator
+
+Simulation of rooted phylogenetic trees under a given Multitype Birth–Death (MTBD) model.
+The MTBD models were introduced by Stadler & Bonhoeffer [[_Philos. Trans. R. Soc. B_ 2013]](https://royalsocietypublishing.org/doi/10.1098/rstb.2012.0198).
+
+We pay particular interest to the classical BD model, the BD Exposed-Infectious (BDEI) model, 
+and BD with superspreading (BDSS), 
+as they are described in [[Voznica _et al._ 2021]]((https://www.biorxiv.org/content/10.1101/2021.03.11.435006v1)). 
+
+## BD
+3 parameters:
+* λ -- transmission rate
+* ψ -- removal rate
+* p -- sampling probability upon removal
+
+Epidemiological parameters:
+* R<sub>0</sub>=λ/ψ -- reproduction number
+* 1/ψ -- infectious time
+
+## BDEI
+2 compartments: 
+* E, exposed, i.e. infected but not yet infectious
+* I, infectious
+
+4 parameters:
+* μ -- transition rate from E to I (becoming infectious)
+* λ -- transmission rate from I to E
+* ψ -- removal rate of I
+* p -- sampling probability upon removal
+
+Epidemiological parameters:
+* R<sub>0</sub>=λ/ψ -- reproduction number
+* 1/ψ -- infectious time
+* 1/μ -- incubation period
+
+## BDSS
+2 compartments: 
+* N, standard infectious individual
+* S, superspreader
+
+6 parameters:
+* λ<sub>nn</sub> -- transmission rate from N to N
+* λ<sub>ns</sub> -- transmission rate from N to S
+* λ<sub>sn</sub> -- transmission rate from S to N
+* λ<sub>ss</sub> -- transmission rate from S to S
+
+    (with a constraint that λ<sub>ss</sub>/λ<sub>ns</sub>=λ<sub>sn</sub>/λ<sub>nn</sub>)
+* ψ -- removal rate of S and of N (the same)
+* p -- sampling probability upon removal (the same for N and S)
+
+
+
+Epidemiological parameters:
+* R<sub>0</sub>=(λ<sub>nn</sub> + λ<sub>ss</sub>)/ψ -- reproduction number
+* 1/ψ -- infectious time
+* X=λ<sub>ss</sub>/λ<sub>ns</sub>=λ<sub>sn</sub>/λ<sub>nn</sub> -- super-spreading transmission ratio
+* f=λ<sub>ss</sub>/(λ<sub>sn</sub> + λ<sub>ss</sub>) -- super-spreading fraction
+
+## Installation
+To install treesimulator:
+```bash
+pip3 install treesimulator
+```
+
+## Usage
+### Command line 
+
+## BD
+The following command simulates a tree with 200-500 tips under BD model, with λ=0.5, ψ=0.25, p=0.5, 
+and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
+```bash
+generate_bd --min_tips 200 --max_tips 500 --la 0.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
+```
+To seee detailed options, run:
+```bash
+generate_bd --help
+```
+
+## BDEI
+The following command simulates a tree with 200-500 tips under BDEI model, with μ=1, λ=0.5, ψ=0.25, p=0.5, 
+and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
+```bash
+generate_bdei --min_tips 200 --max_tips 500 --mu 1 --la 0.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
+```
+To seee detailed options, run:
+```bash
+generate_bdei --help
+```
+
+
+## BDSS
+The following command simulates a tree with 200-500 tips under BDSS model, 
+with λ<sub>nn</sub>=0.1, λ<sub>ns</sub>=0.3, λ<sub>sn</sub>=0.5, λ<sub>ss</sub>=1.5, ψ=0.25, p=0.5, 
+and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
+```bash
+generate_bdss --min_tips 200 --max_tips 500 --la_nn 0.1 --la_ns 0.3 --la_sn 0.5 --la_ss 1.5 --psi 0.25 --p 0.5 --nwk tree.nwk --log params.csv
+```
+To seee detailed options, run:
+```bash
+generate_bdss --help
+```
+
+## User-defined MTBD model
+The following command simulates a tree with 200-500 tips under a generic MTBD model, with two states A and B, 
+with μ<sub>aa</sub>=0.5, μ<sub>ab</sub>=0.6, μ<sub>ba</sub>=0.7, μ<sub>bb</sub>=0.8, 
+λ<sub>aa</sub>=0.1, λ<sub>ab</sub>=0.2, λ<sub>ba</sub>=0.3, λ<sub>bb</sub>=0.4, 
+ψ<sub>a</sub>=0.05, ψ<sub>b</sub>=0.08,
+p=<sub>a</sub>0.15, p=<sub>b</sub>0.65,
+and saves it to a file tree.nwk, while saving the parameters to a comma-separated file params.csv:
+```bash
+generate_mtbd --min_tips 200 --max_tips 500 --nwk tree.nwk --log params.csv \
+--states A B \
+--transition_rates 0.5 0.6 0.7 0.8 \
+--transmission_rates 0.1 0.2 0.3 0.4 \
+--removal_rates 0.05 0.08 \
+--sampling_probabilities 0.15 0.65
+```
+To seee detailed options, run:
+```bash
+generate_mtbd --help
+```
+
+
+### Python3
+To simulate trees with 200-500 tips under the above models and settings:
+```python
+from treesimulator.generator import generate
+from treesimulator import save_forest
+from treesimulator.mtbd_models import Model, BirthDeathModel, BirthDeathExposedInfectiousModel, BirthDeathWithSuperSpreadingModel
+
+bd_model = BirthDeathModel(p=0.5, la=0.5, psi=0.25)
+print(bd_model.get_epidemiological_parameters())
+[bd_tree], (bd_total_tips, _, bd_total_time) = generate(bd_model, min_tips=200, max_tips=500)
+save_forest([bd_tree], 'BD_tree.nwk')
+
+bdei_model = BirthDeathExposedInfectiousModel(p=0.5, mu=1, la=0.5, psi=0.25)
+print(bdei_model.get_epidemiological_parameters())
+[bdei_tree], (bdei_total_tips, _, bdei_total_time) = generate(bdei_model, min_tips=200, max_tips=500)
+save_forest([bdei_tree], 'BDEI_tree.nwk')
+
+bdss_model = BirthDeathWithSuperSpreadingModel(p=0.5, la_nn=0.1, la_ns=0.3, la_sn=0.5, la_ss=1.5, psi=0.25)
+print(bdss_model.get_epidemiological_parameters())
+[bdss_tree], (bdss_total_tips, _, bdss_total_time) = generate(bdss_model, min_tips=200, max_tips=500)
+save_forest([bdss_tree], 'BDSS_tree.nwk')
+
+mtbd_model = Model(states=['A', 'B'], transition_rates=[[0.5, 0.6], [0.7, 0.8]], 
+                   transmission_rates=[[0.1, 0.2], [0.3, 0.4]],
+                   removal_rates=[0.05, 0.08], ps=[0.15, 0.65])
+[mtbd_tree], (mtbd_total_tips, _, mtbd_total_time) = generate(mtbd_model, min_tips=200, max_tips=500)
+save_forest([mtbd_tree], 'MTBD_tree.nwk')
+```
```

### Comparing `treesimulator-0.1.4/README.md` & `treesimulator-0.1.5/README.md`

 * *Files identical despite different names*

