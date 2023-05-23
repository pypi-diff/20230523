# Comparing `tmp/ppca_rs-0.4.1.tar.gz` & `tmp/ppca_rs-0.5.1.tar.gz`

## Comparing `ppca_rs-0.4.1.tar` & `ppca_rs-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,38 @@
--rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 ppca_rs-0.4.1/local_dependencies/ppca/Cargo.toml
--rw-r--r--   0     1000     1000     1055 2022-12-14 17:32:14.000000 ppca_rs-0.4.1/local_dependencies/ppca/license
--rw-r--r--   0     1000     1000     3850 2022-12-20 15:10:13.000000 ppca_rs-0.4.1/local_dependencies/ppca/readme.md
--rw-r--r--   0     1000     1000     3326 2022-12-20 15:10:13.000000 ppca_rs-0.4.1/local_dependencies/ppca/src/dataframe_adapter.rs
--rw-r--r--   0     1000     1000     6799 2023-03-29 17:07:49.000000 ppca_rs-0.4.1/local_dependencies/ppca/src/dataset.rs
--rw-r--r--   0     1000     1000     3238 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/local_dependencies/ppca/src/lib.rs
--rw-r--r--   0     1000     1000    18961 2023-03-29 17:07:49.000000 ppca_rs-0.4.1/local_dependencies/ppca/src/mix.rs
--rw-r--r--   0     1000     1000     5560 2022-12-20 15:10:13.000000 ppca_rs-0.4.1/local_dependencies/ppca/src/output_covariance.rs
--rw-r--r--   0     1000     1000    24219 2023-03-29 17:07:49.000000 ppca_rs-0.4.1/local_dependencies/ppca/src/ppca_model.rs
--rw-r--r--   0     1000     1000     3587 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/local_dependencies/ppca/src/prior.rs
--rw-r--r--   0     1000     1000    23857 2022-12-20 15:10:13.000000 ppca_rs-0.4.1/local_dependencies/ppca/src/python_bindings.rs
--rw-r--r--   0     1000     1000     4137 2023-02-06 18:10:24.000000 ppca_rs-0.4.1/local_dependencies/ppca/src/utils.rs
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 ppca_rs-0.4.1/Cargo.toml
--rw-r--r--   0     1000     1000      650 2022-12-14 17:32:14.000000 ppca_rs-0.4.1/Makefile
--rw-r--r--   0     1000     1000      186 2022-12-14 17:32:14.000000 ppca_rs-0.4.1/Pipfile
--rw-r--r--   0     1000     1000    13137 2022-12-14 17:32:14.000000 ppca_rs-0.4.1/Pipfile.lock
--rw-r--r--   0     1000     1000      667 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/examples/big_toy_model.py
--rw-r--r--   0     1000     1000      212 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/examples/empty_dimensions.py
--rw-r--r--   0     1000     1000      302 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/examples/pickling.py
--rw-r--r--   0     1000     1000      996 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/examples/ppca_mixture.py
--rw-r--r--   0     1000     1000      742 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/examples/priors.py
--rw-r--r--   0     1000     1000      611 2022-12-14 17:32:14.000000 ppca_rs-0.4.1/examples/toy_model.py
--rw-r--r--   0     1000     1000     1055 2022-12-14 17:32:14.000000 ppca_rs-0.4.1/license
--rw-r--r--   0     1000     1000      824 2023-03-29 17:07:49.000000 ppca_rs-0.4.1/pyproject.toml
--rw-r--r--   0     1000     1000    13560 2023-03-29 17:07:49.000000 ppca_rs-0.4.1/python/ppca_rs/__init__.py
--rw-r--r--   0     1000     1000    15378 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/python/ppca_rs/ppca_rs.pyi
--rw-r--r--   0     1000     1000        0 2022-12-14 17:32:14.000000 ppca_rs-0.4.1/python/ppca_rs/py.typed
--rw-r--r--   0     1000     1000     3850 2022-12-20 15:10:13.000000 ppca_rs-0.4.1/readme.md
--rw-r--r--   0     1000     1000       21 2022-12-20 15:10:13.000000 ppca_rs-0.4.1/src/lib.rs
--rw-r--r--   0     1000     1000    28508 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/src/python_bindings.rs
--rw-r--r--   0     1000     1000     3995 2022-12-23 01:49:49.000000 ppca_rs-0.4.1/src/utils.rs
--rw-r--r--   0     1000     1000    17335 2023-03-29 17:07:49.000000 ppca_rs-0.4.1/Cargo.lock
--rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 ppca_rs-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 ppca_rs-0.5.1/local_dependencies/ppca/Cargo.toml
+-rw-r--r--   0     1000     1000       43 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/local_dependencies/ppca/.cargo/config.toml
+-rw-r--r--   0     1000     1000        7 2022-12-20 15:10:13.000000 ppca_rs-0.5.1/local_dependencies/ppca/.gitignore
+-rw-r--r--   0     1000     1000     1055 2022-12-14 17:32:14.000000 ppca_rs-0.5.1/local_dependencies/ppca/license
+-rw-r--r--   0     1000     1000     3850 2022-12-20 15:10:13.000000 ppca_rs-0.5.1/local_dependencies/ppca/readme.md
+-rw-r--r--   0     1000     1000     3326 2022-12-20 15:10:13.000000 ppca_rs-0.5.1/local_dependencies/ppca/src/dataframe_adapter.rs
+-rw-r--r--   0     1000     1000     6798 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/local_dependencies/ppca/src/dataset.rs
+-rw-r--r--   0     1000     1000     3237 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/local_dependencies/ppca/src/lib.rs
+-rw-r--r--   0     1000     1000    18976 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/local_dependencies/ppca/src/mix.rs
+-rw-r--r--   0     1000     1000     5576 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/local_dependencies/ppca/src/output_covariance.rs
+-rw-r--r--   0     1000     1000    24609 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/local_dependencies/ppca/src/ppca_model.rs
+-rw-r--r--   0     1000     1000     3587 2022-12-23 01:49:49.000000 ppca_rs-0.5.1/local_dependencies/ppca/src/prior.rs
+-rw-r--r--   0     1000     1000    23856 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/local_dependencies/ppca/src/python_bindings.rs
+-rw-r--r--   0     1000     1000     4137 2023-02-06 18:10:24.000000 ppca_rs-0.5.1/local_dependencies/ppca/src/utils.rs
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 ppca_rs-0.5.1/Cargo.toml
+-rw-r--r--   0     1000     1000       43 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/.cargo/config.toml
+-rw-r--r--   0     1000     1000       70 2022-12-14 17:32:14.000000 ppca_rs-0.5.1/.gitignore
+-rw-r--r--   0     1000     1000      775 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/.vscode/settings.json
+-rw-r--r--   0     1000     1000      650 2022-12-14 17:32:14.000000 ppca_rs-0.5.1/Makefile
+-rw-r--r--   0     1000     1000      186 2022-12-14 17:32:14.000000 ppca_rs-0.5.1/Pipfile
+-rw-r--r--   0     1000     1000    13137 2022-12-14 17:32:14.000000 ppca_rs-0.5.1/Pipfile.lock
+-rw-r--r--   0     1000     1000      664 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/examples/big_toy_model.py
+-rw-r--r--   0     1000     1000      212 2022-12-23 01:49:49.000000 ppca_rs-0.5.1/examples/empty_dimensions.py
+-rw-r--r--   0     1000     1000      302 2022-12-23 01:49:49.000000 ppca_rs-0.5.1/examples/pickling.py
+-rw-r--r--   0     1000     1000      996 2022-12-23 01:49:49.000000 ppca_rs-0.5.1/examples/ppca_mixture.py
+-rw-r--r--   0     1000     1000      742 2022-12-23 01:49:49.000000 ppca_rs-0.5.1/examples/priors.py
+-rw-r--r--   0     1000     1000      612 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/examples/toy_model.py
+-rw-r--r--   0     1000     1000     1055 2022-12-14 17:32:14.000000 ppca_rs-0.5.1/license
+-rw-r--r--   0     1000     1000      824 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/pyproject.toml
+-rw-r--r--   0     1000     1000    13560 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/python/ppca_rs/__init__.py
+-rw-r--r--   0     1000     1000    15377 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/python/ppca_rs/ppca_rs.pyi
+-rw-r--r--   0     1000     1000        0 2022-12-14 17:32:14.000000 ppca_rs-0.5.1/python/ppca_rs/py.typed
+-rw-r--r--   0     1000     1000     3850 2022-12-20 15:10:13.000000 ppca_rs-0.5.1/readme.md
+-rw-r--r--   0     1000     1000       32 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/src/lib.rs
+-rw-r--r--   0     1000     1000    26602 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/src/python_bindings.rs
+-rw-r--r--   0     1000     1000      766 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/src/utils.rs
+-rw-r--r--   0     1000     1000    17909 2023-05-23 21:00:47.000000 ppca_rs-0.5.1/Cargo.lock
+-rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 ppca_rs-0.5.1/PKG-INFO
```

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/Cargo.toml` & `ppca_rs-0.5.1/local_dependencies/ppca/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ppca"
-version = "0.4.1"
+version = "0.5.1"
 edition = "2021"
 authors = ["Pedro Bittencourt Arruda <pedrobittencourt3@gmail.com>"]
 description = "Rust implementation of the Probabilistic Principal Component Analysis model"
 readme = "./readme.md"
 homepage = "https://github.com/findHotel/ppca_rs"
 repository = "https://github.com/findHotel/ppca_rs"
 license-file = "./license"
@@ -19,15 +19,15 @@
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 
 approx = "0.5.1"
 bit-vec = { version = "0.6.3", features = ["serde"] }
-nalgebra = { version = "0.31.2", features = ["serde-serialize"] }
+nalgebra = { version = "0.32.2", features = ["serde-serialize"] }
 rand = "0.8.5"
 rand_distr = "0.4.3"
-rayon = "1.5.3"
+rayon = "1.7.0"
 ndarray = "0.15.6"
-serde = { version = "1.0.147", features = ["rc"] }
-serde_derive = "1.0.147"
-ordered-float = "3.4.0"
+serde = { version = "1.0.160", features = ["rc"] }
+serde_derive = "1.0.160"
+ordered-float = "3.6.0"
```

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/license` & `ppca_rs-0.5.1/local_dependencies/ppca/license`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/readme.md` & `ppca_rs-0.5.1/local_dependencies/ppca/readme.md`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/src/dataframe_adapter.rs` & `ppca_rs-0.5.1/local_dependencies/ppca/src/dataframe_adapter.rs`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/src/dataset.rs` & `ppca_rs-0.5.1/local_dependencies/ppca/src/dataset.rs`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     /// # Panics
     ///
     /// This function panics if `idx` is out of bounds.
     pub fn is_set(&self, idx: usize) -> bool {
         self.mask.is_set(idx)
     }
 
-    /// Returns the data vector associated with this sample, subsitituting all masked values by `NaN`.
+    /// Returns the data vector associated with this sample, substituting all masked values by `NaN`.
     pub fn masked_vector(&self) -> DVector<f64> {
         self.data
             .iter()
             .copied()
             .zip(&self.mask.0)
             .map(|(value, selected)| if selected { value } else { f64::NAN })
             .collect::<Vec<_>>()
@@ -171,15 +171,15 @@
     pub fn with_weights(&self, weights: Vec<f64>) -> Dataset {
         Dataset {
             data: self.data.clone(),
             weights,
         }
     }
 
-    /// The lenght of this dataset.
+    /// The length of this dataset.
     pub fn len(&self) -> usize {
         self.data.len()
     }
 
     /// Whether this dataset is empty.
     pub fn is_empty(&self) -> bool {
         self.data.is_empty()
```

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/src/lib.rs` & `ppca_rs-0.5.1/local_dependencies/ppca/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 //! This crate implements a _Probabilistic Principal Component Analysis_ in pure Rust, based on a
 //! legacy Python version, which was just too slow for the job (even with `numpy` "C code" to spice it up!)
 //!
-//! If you want all the comfort that the Python ecossystem can provide, you are welcome to check out the
+//! If you want all the comfort that the Python ecosystem can provide, you are welcome to check out the
 //! python wrapper in [PyPI](https://pypi.org/project/ppca-rs/0.3.1/). However, if you want top performance
 //! and great debugging support, this crate is for you.
 //!
 //! To get to know more about the PPCA algorithm for missing data, please check the references below:
 //! * <https://www.robots.ox.ac.uk/~cvrg/hilary2006/ppca.pdf>: first result on Google.
 //! * <http://perception.inrialpes.fr/people/Horaud/Courses/pdf/Horaud-MLSVP9.pdf>: lecture slides, also covering
 //! PPCA mixtures.
```

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/src/mix.rs` & `ppca_rs-0.5.1/local_dependencies/ppca/src/mix.rs`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             models,
             log_weights: robust_log_softmax(log_weights),
         }))
     }
 
     /// Creates a new random __untrained__ model from a given number of PPCA modes, a latent state
     /// size, a dataset and a smoothing factor. The smoothing factor helps with overfit of rarely
-    /// occuring dimensions. If you don't care about that, set it to `0.0`.
+    /// occurring dimensions. If you don't care about that, set it to `0.0`.
     pub fn init(n_models: usize, state_size: usize, dataset: &Dataset) -> PPCAMix {
         PPCAMix::new(
             (0..n_models)
                 .map(|_| PPCAModel::init(state_size, dataset))
                 .collect(),
             vec![0.0; n_models].into(),
         )
@@ -104,30 +104,30 @@
     }
 
     /// The list of constituent PPCA models.
     pub fn models(&self) -> &[PPCAModel] {
         &self.0.models
     }
 
-    /// The log-strength (or log-_a priori_ probablilty) for each PPCA model.
+    /// The log-strength (or log-_a priori_ probability) for each PPCA model.
     pub fn log_weights(&self) -> &DVector<f64> {
         &self.0.log_weights
     }
 
-    /// The strength (or _a priori_ probablilty) for each PPCA model.
+    /// The strength (or _a priori_ probability) for each PPCA model.
     pub fn weights(&self) -> DVector<f64> {
         self.0.log_weights.map(f64::exp)
     }
 
     /// Sample a full dataset from the PPCA model and masks each entry according to a
-    /// Bernoulli (coin-toss) distribution of proability `mask_prob` of erasing the
+    /// Bernoulli (coin-toss) distribution of probability `mask_prob` of erasing the
     /// generated value.
     pub fn sample(&self, dataset_size: usize, mask_probability: f64) -> Dataset {
         let index = WeightedIndex::new(self.0.log_weights.iter().copied().map(f64::exp))
-            .expect("can create WeigtedIndex from distribution");
+            .expect("can create WeighedIndex from distribution");
         (0..dataset_size)
             .into_par_iter()
             .map(|_| {
                 let model_idx = index.sample(&mut rand::thread_rng());
                 self.0.models[model_idx].sample_one(mask_probability)
             })
             .collect()
@@ -169,15 +169,15 @@
             .data
             .par_iter()
             .zip(&dataset.weights)
             .map(|(sample, &weight)| weight * self.llk_one(sample))
             .sum::<f64>()
     }
 
-    /// Returns the _posterior_ distribution (i.e., with Baye's rule applied) for each sample in
+    /// Returns the _posterior_ distribution (i.e., with Bayes' rule applied) for each sample in
     /// the given dataset. Each row of the matrix corresponds to a categorical distribution on the
     /// probability of a sample belonging to a particular PPCA model.
     pub fn infer_cluster(&self, dataset: &Dataset) -> DMatrix<f64> {
         let rows: Vec<_> = dataset
             .data
             .par_iter()
             .map(|sample| {
@@ -284,30 +284,30 @@
 
         let (iterated_models, log_weights): (Vec<_>, Vec<f64>) = self
             .0
             .models
             .iter()
             .enumerate()
             .map(|(i, model)| {
-                // Log-posteriors for this particulat model.
+                // Log-posteriors for this particular model.
                 let log_posteriors: Vec<_> = log_posteriors
                     .par_iter()
                     .zip(&dataset.weights)
                     .filter(|&(_, &wi)| wi > 0.0)
                     .map(|(lp, &wi)| wi.ln() + lp[i])
                     .collect();
                 // Let the NaN silently propagate... everything will blow up before this
                 // is all over.
                 let max_posterior: f64 = log_posteriors
                     .par_iter()
                     .filter_map(|&xi| ordered_float::NotNan::new(xi).ok())
                     .max()
                     .expect("dataset not empty")
                     .into();
-                // Use unnormalized posteriors as weights for numerical stability. One of
+                // Use un-normalized posteriors as weights for numerical stability. One of
                 // the entries is guaranteed to be 1.0.
                 let unnorm_posteriors: Vec<_> = log_posteriors
                     .par_iter()
                     .map(|&p| f64::exp(p - max_posterior))
                     .collect();
                 let logsum_posteriors =
                     unnorm_posteriors.iter().copied().sum::<f64>().ln() + max_posterior;
@@ -358,15 +358,15 @@
         self.log_posterior
             .iter()
             .zip(&self.inferred)
             .map(|(&pi, inferred)| pi * inferred.state())
             .sum()
     }
 
-    /// The covariance matrices of the posterion distribution in the state space.
+    /// The covariance matrices of the posterior distribution in the state space.
     pub fn covariance(&self) -> DMatrix<f64> {
         let mean = self.state();
         self.inferred
             .iter()
             .zip(&self.posterior())
             .map(|(inferred, &weight)| {
                 weight
@@ -378,25 +378,25 @@
 
     /// The smoothed output values for a given output model.
     pub fn smoothed(&self, mix: &PPCAMix) -> DVector<f64> {
         self.inferred
             .iter()
             .zip(&self.posterior())
             .zip(&mix.0.models)
-            .map(|((infered, &weight), ppca)| weight * infered.smoothed(ppca))
+            .map(|((inferred, &weight), ppca)| weight * inferred.smoothed(ppca))
             .sum::<DVector<f64>>()
     }
 
     /// The extrapolated output values for a given output model and the corresponding sample.
     pub fn extrapolated(&self, mix: &PPCAMix, sample: &MaskedSample) -> DVector<f64> {
         self.inferred
             .iter()
             .zip(&self.posterior())
             .zip(&mix.0.models)
-            .map(|((infered, &weight), ppca)| weight * infered.extrapolated(ppca, sample))
+            .map(|((inferred, &weight), ppca)| weight * inferred.extrapolated(ppca, sample))
             .sum::<DVector<f64>>()
     }
 
     /// The covariance for the smoothed output values.
     ///
     /// # Note:
     ///
@@ -425,18 +425,18 @@
     /// Use this not to get lost with big matrices in the output, losing CPU, memory and hair.
     pub fn smoothed_covariance_diagonal(&self, mix: &PPCAMix) -> DVector<f64> {
         let mean = self.smoothed(mix);
         self.inferred
             .iter()
             .zip(&self.posterior())
             .zip(&mix.0.models)
-            .map(|((infered, &weight), ppca)| {
+            .map(|((inferred, &weight), ppca)| {
                 weight
-                    * (infered.smoothed_covariance_diagonal(ppca)
-                        + (infered.smoothed(ppca) - &mean).map(|v| v.powi(2)))
+                    * (inferred.smoothed_covariance_diagonal(ppca)
+                        + (inferred.smoothed(ppca) - &mean).map(|v| v.powi(2)))
             })
             .sum()
     }
 
     /// The covariance for the extraplated values for a given output model and extant values in a given
     /// sample.
     ///
@@ -471,37 +471,37 @@
         sample: &MaskedSample,
     ) -> DVector<f64> {
         let mean = self.extrapolated(mix, sample);
         self.inferred
             .iter()
             .zip(&self.posterior())
             .zip(&mix.0.models)
-            .map(|((infered, &weight), ppca)| {
+            .map(|((inferred, &weight), ppca)| {
                 weight
-                    * (infered.extrapolated_covariance_diagonal(ppca, sample)
-                        + (infered.extrapolated(ppca, sample) - &mean).map(|v| v.powi(2)))
+                    * (inferred.extrapolated_covariance_diagonal(ppca, sample)
+                        + (inferred.extrapolated(ppca, sample) - &mean).map(|v| v.powi(2)))
             })
             .sum()
     }
 
-    /// Samples from the posterior distribution of an infered sample. The sample is smoothed, that
+    /// Samples from the posterior distribution of an inferred sample. The sample is smoothed, that
     /// is, it does not include the model isotropic noise.
     pub fn posterior_sampler(&self) -> PosteriorSamplerMix {
         let index = WeightedIndex::new(self.posterior().iter().copied())
             .expect("failed to create WeightedIndex for posterior");
         let posteriors = self
             .inferred
             .iter()
             .map(InferredMasked::posterior_sampler)
             .collect::<Vec<_>>();
         PosteriorSamplerMix { index, posteriors }
     }
 }
 
-/// Samples from the posterior distribution of an infered sample. The sample is smoothed, that
+/// Samples from the posterior distribution of an inferred sample. The sample is smoothed, that
 /// is, it does not include the model isotropic noise.
 pub struct PosteriorSamplerMix {
     index: WeightedIndex<f64>,
     posteriors: Vec<ppca_model::PosteriorSampler>,
 }
 
 impl Distribution<DVector<f64>> for PosteriorSamplerMix {
```

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/src/output_covariance.rs` & `ppca_rs-0.5.1/local_dependencies/ppca/src/output_covariance.rs`

 * *Files 1% similar despite different names*

```diff
@@ -74,21 +74,21 @@
     ///
     /// # Warning: linear algebra shenanigans afoot!!
     ///
     /// Being the output covariance `sigma^2*I + C*C^T` and the estimator transform
     /// `C^T * (sigma^2*I + C*C^T)^-1`, we have a pesky inverse to calculate! Thankfully,
     /// we can use the Woodbury identity to the rescue!
     /// ```
-    /// (sigma^2*I + C*C^T)^-1 = I/sigma^2 - C/sigma^2*(I + C^T*C/sigma^2)^-1*C^T
+    /// (sigma^2*I + C*C^T)^-1 = I/sigma^2 - C/sigma^2*(I + C^T*C/sigma^2)^-1*C^T/sigma^2
     /// ```
     /// The trick is that the new inverse that we have to calculate has only the
     /// dimension of the _hidden_ state and therefore, goes much faster. The full
     /// estimator is given by:
     /// ```
-    /// C^T/sigma^2 - C^T*C/sigma^2*(I + C^T*C/sigma^2)^-1*C^T
+    /// C^T/sigma^2 - C^T*C/sigma^2*(I + C^T*C/sigma^2)^-1*C^T/sigma^2
     /// ```
     /// Which can be calculated in `O(output_length * state_length^3)`.
     pub(crate) fn estimator_transform(&self) -> DMatrix<f64> {
         (self.transform.transpose()
             - self.inner_product() * self.inner_inverse() * self.transform.transpose())
             / self.isotropic_noise.powi(2)
     }
```

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/src/ppca_model.rs` & `ppca_rs-0.5.1/local_dependencies/ppca/src/ppca_model.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 pub struct PPCAModelInner {
     output_covariance: OutputCovariance<'static>,
     mean: DVector<f64>,
 }
 
 /// A PPCA model which can infer missing values.
 ///
-/// Eeach sample for this model behaves according to the following
+/// Each sample for this model behaves according to the following
 /// statistical latent variable model.
 /// ```
 /// x ~ N(0; I(nxn))
 /// y = C * x + y0 + noise
-/// noise ~ N(0; sgima ^ 2 * I(mxm))
+/// noise ~ N(0; sigma ^ 2 * I(mxm))
 /// ```
 /// Here, `x` is the latent state, y is the observed sample, that is an affine
 /// transformation of the hidden state contaminated by isotropic noise.
 ///
 /// ## Note
 ///
 /// All arrays involved have to be of data type `float64`.
@@ -155,15 +155,15 @@
             .par_iter()
             .map(|sample| self.llk_one(sample))
             .collect::<Vec<_>>()
             .into()
     }
 
     /// Sample a single sample from the PPCA model and masks each entry according to a
-    /// Bernoulli (coin-toss) distribution of proability `mask_prob` of erasing the
+    /// Bernoulli (coin-toss) distribution of probability `mask_prob` of erasing the
     /// generated value.
     pub fn sample_one(&self, mask_prob: f64) -> MaskedSample {
         let sampled_state: DVector<f64> =
             &*self.0.output_covariance.transform * standard_noise(self.state_size()) + &self.0.mean;
         let noise: DVector<f64> =
             self.0.output_covariance.isotropic_noise * standard_noise(self.output_size());
         let mask = Mask(
@@ -177,15 +177,15 @@
         MaskedSample {
             data: mask.fillna(&(sampled_state + noise)),
             mask,
         }
     }
 
     /// Sample a full dataset from the PPCA model and masks each entry according to a
-    /// Bernoulli (coin-toss) distribution of proability `mask_prob` of erasing the
+    /// Bernoulli (coin-toss) distribution of probability `mask_prob` of erasing the
     /// generated value.
     pub fn sample(&self, dataset_size: usize, mask_prob: f64) -> Dataset {
         (0..dataset_size)
             .into_par_iter()
             .map(|_| self.sample_one(mask_prob))
             .collect()
     }
@@ -219,15 +219,15 @@
 
     /// Filters a single samples, removing noise from the extant samples and
     /// inferring the missing samples.
     pub fn smooth_one(&self, sample: &MaskedSample) -> MaskedSample {
         MaskedSample::unmasked(self.infer_one(sample).smoothed(&self))
     }
 
-    /// Filters each sample of a given datatset, removing noise from the extant samples and
+    /// Filters each sample of a given dataset, removing noise from the extant samples and
     /// inferring the missing samples.
     pub fn smooth(&self, dataset: &Dataset) -> Dataset {
         dataset
             .data
             .par_iter()
             .zip(&dataset.weights)
             .map(|(sample, &weight)| (self.smooth_one(sample), weight))
@@ -379,15 +379,15 @@
                 transform: Cow::Owned(new_transform),
                 isotropic_noise: isotropic_noise_sq.sqrt(),
             },
             mean: new_mean,
         }))
     }
 
-    /// Returns a canonical version of this model. This does not alter the log-probablility
+    /// Returns a canonical version of this model. This does not alter the log-probability
     /// function nor the quality of the training. All it does is to transform the hidden
     /// variables.
     pub fn to_canonical(&self) -> PPCAModel {
         // Yes, we can have an empty state! In these case, there is nothing to be done.
         if self.state_size() == 0 {
             return self.clone();
         }
@@ -494,15 +494,15 @@
             .map(|noiseless_output_variance| {
                 noiseless_output_variance + covariance.isotropic_noise.powi(2)
             })
             .collect::<Vec<_>>()
             .into()
     }
 
-    /// The covariance for the extraplated values for a given output model and extant values in a given
+    /// The covariance for the extrapolated values for a given output model and extant values in a given
     /// sample.
     ///
     /// # Note:
     ///
     /// Afraid of the big, fat matrix? The method `output_covariance_diagonal` might just
     /// save your life.
     pub fn extrapolated_covariance(&self, ppca: &PPCAModel, sample: &MaskedSample) -> DMatrix<f64> {
@@ -563,15 +563,15 @@
             })
             .collect::<Vec<_>>()
             .into();
 
         negative.expand(&diagonal_reduced)
     }
 
-    /// Samples from the posterior distribution of an infered sample. The sample is smoothed, that
+    /// Samples from the posterior distribution of an inferred sample. The sample is smoothed, that
     /// is, it does not include the model isotropic noise.
     pub fn posterior_sampler(&self) -> PosteriorSampler {
         let cholesky = self
             .covariance
             .clone()
             .cholesky()
             .expect("Cholesky decomposition failed");
@@ -579,32 +579,44 @@
             model: self.model.clone(),
             state: self.state.clone(),
             cholesky_l: cholesky.l(),
         }
     }
 }
 
-/// Samples from the posterior distribution of an infered sample. The sample is smoothed, that
+/// Samples from the posterior distribution of an inferred sample. The sample is smoothed, that
 /// is, it does not include the model isotropic noise.
 pub struct PosteriorSampler {
     model: PPCAModel,
     state: DVector<f64>,
     cholesky_l: DMatrix<f64>,
 }
 
 impl Distribution<DVector<f64>> for PosteriorSampler {
     fn sample<R>(&self, rng: &mut R) -> DVector<f64>
     where
         R: Rng + ?Sized,
     {
+        // State noise:
         let standard: DVector<f64> = (0..self.state.len())
             .map(|_| rand_distr::StandardNormal.sample(rng))
             .collect::<Vec<_>>()
             .into();
-        self.model.mean() + self.model.transform() * (&self.state + &self.cholesky_l * standard)
+        // Output noise:
+        let noise: DVector<f64> = (0..self.model.output_size())
+            .map(|_| {
+                let standard: f64 = rand_distr::StandardNormal.sample(rng);
+                self.model.0.output_covariance.isotropic_noise * standard
+            })
+            .collect::<Vec<_>>()
+            .into();
+
+        noise
+            + self.model.mean()
+            + self.model.transform() * (&self.state + &self.cholesky_l * standard)
     }
 }
 
 #[cfg(test)]
 mod test {
     use bit_vec::BitVec;
     use nalgebra::{dmatrix, dvector};
```

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/src/prior.rs` & `ppca_rs-0.5.1/local_dependencies/ppca/src/prior.rs`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/src/python_bindings.rs` & `ppca_rs-0.5.1/local_dependencies/ppca/src/python_bindings.rs`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
     }
 
     fn __repr__(&self, py: Python<'_>) -> String {
         format!(
             "PPCAModel(\
                 isotropic_noise={}, \
                 transform=array({}, dtype=\"float32\"), \
-                mean=narray({}, dtype=\"float32\"))",
+                mean=array({}, dtype=\"float32\"))",
             self.isotropic_noise(),
             self.transform(py),
             self.mean(py),
         )
     }
 
     fn llk(&self, py: Python<'_>, dataset: &DatasetWrapper) -> f64 {
```

### Comparing `ppca_rs-0.4.1/local_dependencies/ppca/src/utils.rs` & `ppca_rs-0.5.1/local_dependencies/ppca/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/Cargo.toml` & `ppca_rs-0.5.1/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "ppca_rs"
-version = "0.4.1"
+version = "0.5.1"
 edition = "2021"
 publish = false
 
 [package.metadata.maturin]
 python-source = "python"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ppca_rs"
 crate-type = ["staticlib"]
 
 [dependencies]
 ppca = { path = "local_dependencies/ppca" }
-pyo3 = { version = "0.17.1", features = ["extension-module"] }
-numpy = { git = "https://github.com/PyO3/rust-numpy", features = ["nalgebra"] }
+pyo3 = { version = "0.18.3", features = ["extension-module"] }
+numpy = { version = "0.18.0", features = ["nalgebra"] }
 bincode = "1.3.3"
-rayon = "1.6.1"
-nalgebra = "0.31.4"
+rayon = "1.7.0"
+nalgebra = "0.32.2"
 rand = "0.8.5"
 rand_distr = "0.4.3"
```

### Comparing `ppca_rs-0.4.1/Makefile` & `ppca_rs-0.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/Pipfile.lock` & `ppca_rs-0.5.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/examples/big_toy_model.py` & `ppca_rs-0.5.1/examples/big_toy_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 from ppca_rs import PPCAModel
 
 print("Generating model")
 
 transform = np.random.binomial(1.0, 0.1, size=(200, 16))
 real_model = PPCAModel(
-    transform=np.matrix(transform, dtype="float64").T.T,
+    transform=np.matrix(transform, dtype="float64"),
     isotropic_noise=0.1,
     mean=np.zeros((200, 1), dtype="float64"),
 )
 
-print("Generating syntetic sample")
+print("Generating synthetic sample")
 sample = real_model.sample(100_000, 0.2)
 
 print("Initializing model")
 model = PPCAModel.init(16, sample)
 
 print("Starting iterations...")
```

### Comparing `ppca_rs-0.4.1/examples/ppca_mixture.py` & `ppca_rs-0.5.1/examples/ppca_mixture.py`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/examples/priors.py` & `ppca_rs-0.5.1/examples/priors.py`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/examples/toy_model.py` & `ppca_rs-0.5.1/examples/toy_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 from ppca_rs import PPCAModel
 
 real_model = PPCAModel(
-    transform=np.matrix([[1, 1, 0], [1, 0, 1]], dtype="float64").T,
+    transform=np.array([[1, 1], [0, 1], [0, 1]], dtype="float64"),
     isotropic_noise=0.1,
-    mean=np.array([[0, 1, 0]], dtype="float64").T,
+    mean=np.array([[0], [1], [0]], dtype="float64"),
 )
 sample = real_model.sample(100, mask_prob=0.2)
 model = PPCAModel.init(2, sample)
 
 for it in range(100):
     print(f"At iteration {it + 1} PPCA llk is {model.llk(sample)}")
     model: PPCAModel = model.iterate(sample)
```

### Comparing `ppca_rs-0.4.1/license` & `ppca_rs-0.5.1/license`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/pyproject.toml` & `ppca_rs-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.13,<0.14"]
 build-backend = "maturin"
 
 [project]
 name = "ppca-rs"
-version = "0.4.1"
+version = "0.5.1"
 requires-python = ">=3.7"
 description = "Python+Rust implementation of the Probabilistic Principal Component Analysis model"
 readme = "readme.md"
 classifiers = [
     "Programming Language :: Rust",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `ppca_rs-0.4.1/python/ppca_rs/__init__.py` & `ppca_rs-0.5.1/python/ppca_rs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Literal, Optional
 
 import numpy as np
 
 
-__version__ = "0.4.1"
+__version__ = "0.5.1"
 
 
 @dataclass(frozen=True)
 class TrainMetrics:
     llk: float
     aic: float
     bic: float
```

### Comparing `ppca_rs-0.4.1/python/ppca_rs/ppca_rs.pyi` & `ppca_rs-0.5.1/python/ppca_rs/ppca_rs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 class PPCAModel:
     """
     A PPCA model: each sample for this model behaves according to the following
     statistical latent variable model.
     ```
     x ~ N(0; I(nxn))
     y = C * x + y0 + noise
-    noise ~ N(0; sgima ^ 2 * I(mxm))
+    noise ~ N(0; sigma ^ 2 * I(mxm))
     ```
     Here, `x` is the latent state, y is the observed sample, that is an affine
     transformation of the hidden state contaminated by isotropic noise.
 
     ## Note
 
     All arrays involved have to be of data type `float64`.
@@ -159,15 +159,15 @@
     isotropic_noise: float
     """The standard deviation of the noise in the output space."""
     mean: np.ndarray
     """Then center of mass of the distribution in the output space."""
     smoothing_factor: float
     """
     A factor to smooth out the `transform` matrix when there is little data for a given
-    dimension. Use this as an extra guard aginst overfitting.
+    dimension. Use this as an extra guard against over-fitting.
     """
     singular_values: np.ndarray
     """
     The relative strength of each hidden variable on the output. This is equivalent to the
     eigenvalues in the standard PCA.
     """
     output_size: int
@@ -185,30 +185,30 @@
     def dump(self) -> bytes:
         """
         Encodes the PPCA model into binary data. Use this if you want to avoid
         picking.
         """
     @staticmethod
     def init(n_states: int, smoothing_factor: float = 0.0) -> PPCAModel:
-        """Creates an uninformed random model to seed the trainment."""
+        """Creates an uninformed random model to seed the trainement."""
     def __repr__(self) -> str: ...
     def llk(self, dataset: Dataset) -> float:
         """
         Calculates the log-probability of a given masked dataset according to the current
         model.
         """
     def llks(self, dataset: Dataset) -> np.ndarray:
         """
         Calculates the log-probability of **each sample** in a given masked dataset
         according to the current model.
         """
     def sample(self, dataset_size: int, mask_prob: float) -> Dataset:
         """
         Samples random outputs from the model and masks each entry according to a
-        Bernoulli (coin-toss) distribution of proability `mask_prob` of erasing the
+        Bernoulli (coin-toss) distribution of probability `mask_prob` of erasing the
         generated value.
         """
     def infer(self, dataset: Dataset) -> InferredMasked:
         """
         Infers the hidden components for each sample in the dataset. Use this method for
         fine-grain control on the properties you want to extract from the model.
         """
@@ -230,15 +230,15 @@
     def iterate(self, dataset: Dataset) -> PPCAModel:
         """
         Makes one iteration of the EM algorithm for the PPCA over an observed dataset,
         returning the improved model.
         """
     def to_canonical(self) -> PPCAModel:
         """
-        Returns a canonical version of this model. This does not alter the log-probablility
+        Returns a canonical version of this model. This does not alter the log-probability
         function nor the quality of the training. All it does is to transform the hidden
         variables.
         """
 
 class InferredMaskedMix:
     """
     A class containing the result of the Bayesian inference step in `PPCAModel.infer`.
@@ -288,16 +288,16 @@
         """
         The covariance for the extraplated values.
         """
     def extrapolated_covariances_diagonal(
         self, model: PPCAModel, dataset: Dataset
     ) -> Dataset:
         """
-        Returns an _approximation_ of the extrapolated output covariance matrix, treating each masked
-        output as an independent normal distribution.
+        Returns an _approximation_ of the extrapolated output covariance matrix, treating each
+        masked output as an independent normal distribution.
 
         # Note
 
         Use this not to get lost with big matrices in the output, losing CPU, memory and
         hair.
         """
 
@@ -327,38 +327,38 @@
     output_size: int
     """The number of features for this model."""
     state_sizes: List[int]
     """The number of hidden values for each PPCA model in the mixture."""
     n_parameters: int
     """The total number of parameters involved in training (used for information criteria)."""
     models: List[PPCAModel]
-    """The constituent PPCA models of this PPPCA mixture."""
+    """The constituent PPCA models of this PPCA mixture."""
     log_weights: np.ndarray
     """The log-probabilities of each constituent PPCA models for this PPCA mixture."""
     weights: np.ndarray
     """The probabilities of each constituent PPCA models for this PPCA mixture."""
 
     @staticmethod
-    def load(b: bytes) -> PPCAModel:
+    def load(b: bytes) -> PPCAMix:
         """
         Loads a PPCA mixture model from binary data. Use this if you want to avoid picking.
         """
     def dump(self) -> bytes:
         """
         Encodes the PPCA mixture model into binary data. Use this if you want to avoid
         picking.
         """
     @staticmethod
     def init(
         n_models: int,
         n_states: int,
         smoothing_factor: float = 0.0,
-    ) -> PPCAModel:
+    ) -> PPCAMix:
         """
-        Creates an uninformed random model to seed the trainment. All constituent models
+        Creates an uninformed random model to seed the trainement. All constituent models
         will have the same state size.
         """
     def __repr__(self) -> str: ...
     def llk(self, dataset: Dataset) -> float:
         """
         Calculates the log-probability of a given masked dataset according to the current
         model.
@@ -367,15 +367,15 @@
         """
         Calculates the log-probability of **each sample** in a given masked dataset
         according to the current model.
         """
     def sample(self, dataset_size: int, mask_prob: float) -> Dataset:
         """
         Samples random outputs from the model and masks each entry according to a
-        Bernoulli (coin-toss) distribution of proability `mask_prob` of erasing the
+        Bernoulli (coin-toss) distribution of probability `mask_prob` of erasing the
         generated value.
         """
     def infer(self, dataset: Dataset) -> InferredMaskedMix:
         """
         Infers the hidden components for each sample in the dataset. Use this method for
         fine-grain control on the properties you want to extract from the model.
         """
@@ -397,11 +397,11 @@
     def iterate(self, dataset: Dataset) -> PPCAMix:
         """
         Makes one iteration of the EM algorithm for the PPCA mixture model over an
         observed dataset, returning a improved model.
         """
     def to_canonical(self) -> PPCAMix:
         """
-        Returns a canonical version of this model. This does not alter the log-probablility
+        Returns a canonical version of this model. This does not alter the log-probability
         function nor the quality of the training. All it does is to transform the hidden
         variables.
         """
```

### Comparing `ppca_rs-0.4.1/readme.md` & `ppca_rs-0.5.1/readme.md`

 * *Files identical despite different names*

### Comparing `ppca_rs-0.4.1/src/python_bindings.rs` & `ppca_rs-0.5.1/src/python_bindings.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-use nalgebra::{DMatrix, DMatrixSlice, DVectorSlice};
+use nalgebra::DMatrix;
 use numpy::{PyArray1, PyArray2, PyReadonlyArray1, PyReadonlyArray2, ToPyArray};
 use pyo3::{prelude::*, types::PyBytes};
 use rand_distr::Distribution;
 use rayon::prelude::*;
 
 use ppca::{
     Dataset, InferredMasked, InferredMaskedMix, MaskedSample, PPCAMix, PPCAModel, PosteriorSampler,
     PosteriorSamplerMix, Prior,
 };
 
+use crate::utils::{to_nalgebra, to_nalgebra_vector};
+
 /// This module is implemented in Rust.
 #[pymodule]
 pub fn ppca_rs(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<PriorWrapper>()?;
     m.add_class::<PPCAModelWrapper>()?;
     m.add_class::<DatasetWrapper>()?;
     m.add_class::<InferredMaskedBatch>()?;
@@ -26,15 +28,15 @@
 #[pyclass]
 #[pyo3(name = "Dataset", module = "ppca_rs")]
 struct DatasetWrapper(Dataset);
 
 #[pymethods]
 impl DatasetWrapper {
     #[new]
-    #[args(weights = "None")]
+    #[pyo3(signature = (ndarray, weights = None))]
     fn new(
         py: Python,
         ndarray: PyReadonlyArray2<f64>,
         weights: Option<PyReadonlyArray1<f64>>,
     ) -> PyResult<DatasetWrapper> {
         let n_samples = ndarray.shape()[0];
         let output_size = ndarray.shape()[1];
@@ -173,38 +175,20 @@
     pub fn new() -> PriorWrapper {
         PriorWrapper(Prior::default())
     }
 
     pub fn with_mean_prior(
         &self,
         py: Python,
-        mean: Py<PyArray1<f64>>,
+        mean: Py<PyArray2<f64>>,
         mean_covariance: Py<PyArray2<f64>>,
     ) -> PyResult<Self> {
         let new = self.0.clone().with_mean_prior(
-            (mean
-                .as_ref(py)
-                .try_readonly()?
-                .try_as_matrix()
-                .ok_or_else(|| {
-                    pyo3::exceptions::PyException::new_err(
-                        "could not convert mean ndarray to matrix",
-                    )
-                })? as DVectorSlice<f64>)
-                .into_owned(),
-            (mean_covariance
-                .as_ref(py)
-                .try_readonly()?
-                .try_as_matrix()
-                .ok_or_else(|| {
-                    pyo3::exceptions::PyException::new_err(
-                        "could not convert mean covariance ndarray to matrix",
-                    )
-                })? as DMatrixSlice<f64>)
-                .into_owned(),
+            to_nalgebra_vector(py, mean),
+            to_nalgebra(py, mean_covariance),
         );
         Ok(PriorWrapper(new))
     }
 
     pub fn with_isotropic_noise_prior(&self, alpha: f64, beta: f64) -> Self {
         let new = self.0.clone().with_isotropic_noise_prior(alpha, beta);
         PriorWrapper(new)
@@ -392,34 +376,16 @@
         py: Python<'_>,
         isotropic_noise: f64,
         transform: Py<PyArray2<f64>>,
         mean: Py<PyArray2<f64>>,
     ) -> PyResult<PPCAModelWrapper> {
         Ok(PPCAModelWrapper(PPCAModel::new(
             isotropic_noise,
-            (transform
-                .as_ref(py)
-                .try_readonly()?
-                .try_as_matrix()
-                .ok_or_else(|| {
-                    pyo3::exceptions::PyException::new_err(
-                        "could not convert transformation ndarray to matrix",
-                    )
-                })? as DMatrixSlice<f64>)
-                .into_owned(),
-            (mean
-                .as_ref(py)
-                .try_readonly()?
-                .try_as_matrix()
-                .ok_or_else(|| {
-                    pyo3::exceptions::PyException::new_err(
-                        "could not convert mean ndarray to matrix",
-                    )
-                })? as DVectorSlice<f64>)
-                .into_owned(),
+            to_nalgebra(py, transform),
+            to_nalgebra_vector(py, mean),
         )))
     }
 
     #[staticmethod]
     fn load(bytes: &PyBytes) -> PyResult<PPCAModelWrapper> {
         Ok(PPCAModelWrapper(
             bincode::deserialize(bytes.as_bytes())
@@ -933,29 +899,7 @@
                 .map(|sample| MaskedSample::unmasked(sample.sample(&mut rand::thread_rng())))
                 .collect::<Dataset>()
         });
 
         DatasetWrapper(samples)
     }
 }
-
-// #[pyclass]
-// #[pyo3(name = "DataFrameAdapter", module = "ppca_rs")]
-// #[derive(Debug, Clone)]
-// struct DataFrameAdapterWrapper(DataFrameAdapter);
-
-// #[pymethods]
-// impl DataFrameAdapterWrapper {
-//     #[staticmethod]
-//     fn build(
-//         df: &PyAny,
-//         keys: Vec<String>,
-//         dimensions: Vec<String>,
-//         metric: String,
-//     ) -> PyResult<DataFrameAdapterWrapper>{
-//         let df = crate::polars_python_hack::array_to_rust(df)?;
-
-//         Ok(DataFrameAdapterWrapper(
-//             DataFrameAdapter::build(df, keys, dimensions, metric)?
-//         ))
-//     }
-// }
```

### Comparing `ppca_rs-0.4.1/Cargo.lock` & `ppca_rs-0.5.1/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bytemuck"
-version = "1.12.3"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aaa3a8d9a1ca92e282c96a32d6511b695d7d994d1d102ba85d279f9b2756947f"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -126,17 +126,17 @@
 name = "indoc"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
 
 [[package]]
 name = "libc"
-version = "0.2.137"
+version = "0.2.140"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc7fcc620a3bff7cdd7a365be3376c97191aeaccc2a603e600951e452615bf89"
+checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -157,56 +157,56 @@
 checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
 dependencies = [
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "nalgebra"
-version = "0.31.4"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20bd243ab3dbb395b39ee730402d2e5405e448c75133ec49cc977762c4cba3d1"
+checksum = "d68d47bba83f9e2006d117a9a33af1524e655516b8919caac694427a6fb1e511"
 dependencies = [
  "approx",
  "matrixmultiply",
  "nalgebra-macros",
  "num-complex",
  "num-rational",
  "num-traits",
  "serde",
  "simba",
  "typenum",
 ]
 
 [[package]]
 name = "nalgebra-macros"
-version = "0.1.0"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01fcc0b8149b4632adc89ac3b7b31a12fb6099a0317a4eb2ebff574ef7de7218"
+checksum = "d232c68884c0c99810a5a4d333ef7e47689cfd0edc85efc9e54e1e6bf5212766"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
@@ -216,17 +216,17 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ae39348c8bc5fbd7f40c727a9925f03517afd2ab27d46702108b6a7e5414c19"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "num-integer"
@@ -267,38 +267,39 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.17.2"
-source = "git+https://github.com/PyO3/rust-numpy#2f186194ae8f92920c9871b3fec088f2266d7c43"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96b0fee4571867d318651c24f4a570c3f18408cf95f16ccb576b3ce85496a46e"
 dependencies = [
  "libc",
  "nalgebra",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "ordered-float"
-version = "3.4.0"
+version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d84eb1409416d254e4a9c8fa56cc24701755025b458f0fcd8e59e1f5f40c23bf"
+checksum = "13a384337e997e6860ffbaa83708b2ef329fd8c54cb67a5f64d421e0f943254f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
@@ -307,34 +308,34 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.4"
+version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dc9e0dc2adc1c69d09143aff38d3d30c5c3f0df0dad82e6d25547af174ebec0"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.9"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1de2e551fb905ac83f73f7aedf2f0cb4a0da7e35efa24a202a936269f1f18e1"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "ppca"
-version = "0.4.1"
+version = "0.5.1"
 dependencies = [
  "approx",
  "bit-vec",
  "nalgebra",
  "ndarray",
  "ordered-float",
  "rand",
@@ -342,15 +343,15 @@
  "rayon",
  "serde",
  "serde_derive",
 ]
 
 [[package]]
 name = "ppca_rs"
-version = "0.4.1"
+version = "0.5.1"
 dependencies = [
  "bincode",
  "nalgebra",
  "numpy",
  "ppca",
  "pyo3",
  "rand",
@@ -362,86 +363,86 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.47"
+version = "1.0.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ea3d908b0e36316caf9e9e2c4625cdde190a7e6f440d794667ed17a1855e725"
+checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.6.5",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -486,27 +487,27 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cac410af5d00ab6884528b4ab69d1e8e146e8d471201800fa1b4524126de6ad3"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
@@ -538,37 +539,37 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.147"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d193d69bae983fc11a79df82342761dfbf28a99fc8d203dca4c3c1b590948965"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.147"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f1d362ca8fc9c3e3a7484440752472d68a6caa98f1ab81d99b5dfe517cec852"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.12",
 ]
 
 [[package]]
 name = "simba"
-version = "0.7.3"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f3fd720c48c53cace224ae62bef1bbff363a70c68c4802a78b5cc6159618176"
+checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
 dependencies = [
  "approx",
  "num-complex",
  "num-traits",
  "paste",
  "wide",
 ]
@@ -577,40 +578,51 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "syn"
-version = "1.0.103"
+version = "1.0.109"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a864042229133ada95abf3b54fdc62ef5ccabe9515b64717bcb9a1919e59445d"
+checksum = "79d9531f94112cfc3e4c8f5f02cb2b58f72c97b7efd85f70203cc6d8efda5927"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
 
 [[package]]
 name = "typenum"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf81ac59edc17cc8697ff311e8f5ef2d99fcbd9817b34cec66f90b6c3dfd987"
+checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.5"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ceab39d59e4c9499d4e5a8ee0e2735b891bb7308ac83dfb4e80cad195c9f6f3"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unindent"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
 
@@ -618,71 +630,80 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wide"
-version = "0.7.5"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae41ecad2489a1655c8ef8489444b0b113c0a0c795944a3572a0931cf7d2525c"
+checksum = "b689b6c49d6549434bf944e6b0f39238cf63693cb7a147e9d887507fffa3b223"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.45.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
```

### Comparing `ppca_rs-0.4.1/PKG-INFO` & `ppca_rs-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppca-rs
-Version: 0.4.1
+Version: 0.5.1
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: cffi
 Requires-Dist: numpy
```

