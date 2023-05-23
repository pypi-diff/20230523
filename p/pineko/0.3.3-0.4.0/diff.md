# Comparing `tmp/pineko-0.3.3.tar.gz` & `tmp/pineko-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pineko-0.3.3.tar", max compression
+gzip compressed data, was "pineko-0.4.0.tar", max compression
```

## Comparing `pineko-0.3.3.tar` & `pineko-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0     2248 2023-02-15 16:41:15.680436 pineko-0.3.3/README.md
--rw-r--r--   0        0        0     3339 2023-02-15 16:41:53.392685 pineko-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       89 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/__init__.py
--rw-r--r--   0        0        0     5683 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/check.py
--rw-r--r--   0        0        0      117 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/cli/__init__.py
--rw-r--r--   0        0        0      237 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/cli/_base.py
--rw-r--r--   0        0        0     2957 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/cli/check.py
--rw-r--r--   0        0        0     1529 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/cli/compare.py
--rw-r--r--   0        0        0     2158 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/cli/convolute.py
--rw-r--r--   0        0        0     1205 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/cli/opcard.py
--rw-r--r--   0        0        0     1558 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/cli/scaffold.py
--rw-r--r--   0        0        0     3418 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/cli/theory_.py
--rw-r--r--   0        0        0     1633 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/comparator.py
--rw-r--r--   0        0        0     3700 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/configs.py
--rw-r--r--   0        0        0     1031 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/ekompatibility.py
--rw-r--r--   0        0        0     7244 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/evolve.py
--rw-r--r--   0        0        0     2035 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/parser.py
--rw-r--r--   0        0        0     2534 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/scaffold.py
--rw-r--r--   0        0        0    13955 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/theory.py
--rw-r--r--   0        0        0     1734 2023-02-15 16:41:15.684435 pineko-0.3.3/src/pineko/theory_card.py
--rw-r--r--   0        0        0       49 2023-02-15 16:41:53.392685 pineko-0.3.3/src/pineko/version.py
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 pineko-0.3.3/setup.py
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 pineko-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-23 14:39:56.669124 pineko-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2248 2023-05-23 14:39:56.669124 pineko-0.4.0/README.md
+-rw-r--r--   0        0        0     3341 2023-05-23 14:44:37.762009 pineko-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/__init__.py
+-rw-r--r--   0        0        0     5596 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/check.py
+-rw-r--r--   0        0        0      134 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/__init__.py
+-rw-r--r--   0        0        0      237 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/_base.py
+-rw-r--r--   0        0        0     3289 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/check.py
+-rw-r--r--   0        0        0     1529 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/compare.py
+-rw-r--r--   0        0        0     2158 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/convolute.py
+-rw-r--r--   0        0        0      850 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/gen_sv.py
+-rw-r--r--   0        0        0     1083 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/kfactor.py
+-rw-r--r--   0        0        0     1205 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/opcard.py
+-rw-r--r--   0        0        0     1558 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/scaffold.py
+-rw-r--r--   0        0        0     3822 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/cli/theory_.py
+-rw-r--r--   0        0        0     1639 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/comparator.py
+-rw-r--r--   0        0        0     3700 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/configs.py
+-rw-r--r--   0        0        0     1022 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/ekompatibility.py
+-rw-r--r--   0        0        0     7957 2023-05-23 14:39:56.669124 pineko-0.4.0/src/pineko/evolve.py
+-rw-r--r--   0        0        0    13751 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/kfactor.py
+-rw-r--r--   0        0        0     2035 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/parser.py
+-rw-r--r--   0        0        0     2534 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/scaffold.py
+-rw-r--r--   0        0        0    10171 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/scale_variations.py
+-rw-r--r--   0        0        0    14799 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/theory.py
+-rw-r--r--   0        0        0     1734 2023-05-23 14:39:56.673124 pineko-0.4.0/src/pineko/theory_card.py
+-rw-r--r--   0        0        0       49 2023-05-23 14:44:37.762009 pineko-0.4.0/src/pineko/version.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 pineko-0.4.0/PKG-INFO
```

### Comparing `pineko-0.3.3/README.md` & `pineko-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pineko-0.3.3/pyproject.toml` & `pineko-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pineko"
-version = "0.3.3"
+version = "0.4.0"
 description = "Combine PineAPPL grids and EKOs into FK tables"
 readme = "README.md"
 authors = [
   "Alessandro Candido <alessandro.candido@mi.infn.it>",
   "Andrea Barontini <andrea.barontini@mi.infn.it>",
   "Felix Hekhorn <felix.hekhorn@mi.infn.it>",
 ]
@@ -19,17 +19,17 @@
   "Topic :: Scientific/Engineering :: Physics",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
 repository = "https://github.com/N3PDF/pineko"
 packages = [{ include = "pineko", from = "src" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-eko = "^0.12.0"
-pineappl = "^0.5.9"
+python = ">=3.8,<3.12"
+eko = "^0.13.2"
+pineappl = { version = "^0.6.0a17", allow-prereleases = true }
 PyYAML = "^6.0"
 numpy = "^1.21.0"
 pandas = "^1.4.1"
 rich = "^12.5.1"
 click = "^8.0.4"
 tomli = "^2.0.1"
 # docs dependencies (for readthedocs, https://github.com/readthedocs/readthedocs.org/issues/4912#issuecomment-664002569)
@@ -50,17 +50,14 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 pytest-env = "^0.6.2"
 pylint = "^2.11.1"
 
-[tool.poetry.group.dev]
-optional = true
-
 [tool.poetry.group.dev.dependencies]
 pdbpp = "^0.10.3"
 ipython = "^8.0"
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-rtd-theme", "sphinxcontrib-bibtex"]
```

### Comparing `pineko-0.3.3/src/pineko/cli/compare.py` & `pineko-0.4.0/src/pineko/cli/compare.py`

 * *Files identical despite different names*

### Comparing `pineko-0.3.3/src/pineko/cli/convolute.py` & `pineko-0.4.0/src/pineko/cli/convolute.py`

 * *Files identical despite different names*

### Comparing `pineko-0.3.3/src/pineko/cli/opcard.py` & `pineko-0.4.0/src/pineko/cli/opcard.py`

 * *Files identical despite different names*

### Comparing `pineko-0.3.3/src/pineko/cli/scaffold.py` & `pineko-0.4.0/src/pineko/cli/scaffold.py`

 * *Files identical despite different names*

### Comparing `pineko-0.3.3/src/pineko/cli/theory_.py` & `pineko-0.4.0/src/pineko/cli/theory_.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,7 +89,16 @@
 )
 @click.option("--overwrite", is_flag=True, help="Allow files to be overwritten")
 def fks(theory_id, datasets, pdf, silent, clear_logs, overwrite):
     """Compute FK tables in all datasets."""
     theory.TheoryBuilder(
         theory_id, datasets, silent=silent, clear_logs=clear_logs, overwrite=overwrite
     ).fks(pdf)
+
+
+@theory_.command()
+@click.argument("theory_id", type=click.INT)
+@click.argument("datasets", type=click.STRING, nargs=-1)
+@click.option("--flavors", "-f", default=5, help="Number of active flavors")
+def ren_sv_grids(theory_id, datasets, flavors):
+    """Construct new grids with renormalization scale variations included."""
+    theory.TheoryBuilder(theory_id, datasets).construct_ren_sv_grids(flavors)
```

### Comparing `pineko-0.3.3/src/pineko/comparator.py` & `pineko-0.4.0/src/pineko/comparator.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     df : pd.DataFrame
         comparison table
     """
     import lhapdf  # pylint: disable=import-error
 
     pdfset = lhapdf.mkPDF(pdf, 0)
     pdgid = int(pdfset.set().get_entry("Particle"))
-    order_mask = pineappl.grid.Order.create_mask(pine.orders(), max_as, max_al)
+    order_mask = pineappl.grid.Order.create_mask(pine.orders(), max_as, max_al, True)
     before = np.array(
         pine.convolute_with_one(
             pdgid,
             pdfset.xfxQ2,
             pdfset.alphasQ2,
             order_mask=order_mask,
             xi=((xir, xif),),
```

### Comparing `pineko-0.3.3/src/pineko/configs.py` & `pineko-0.4.0/src/pineko/configs.py`

 * *Files identical despite different names*

### Comparing `pineko-0.3.3/src/pineko/ekompatibility.py` & `pineko-0.4.0/src/pineko/ekompatibility.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,18 +18,18 @@
         a minimal object, with all and only the information consumed by PineAPPL
 
     """
     oldgrid = {}
     oldgrid["Q2grid"] = {}
     for q2, op in operator.items():
         oldop = dict(operators=op.operator)
-        oldgrid["Q2grid"][q2] = oldop
+        oldgrid["Q2grid"][q2[0]] = oldop
 
     oldgrid["q2_ref"] = operator.mu20
-    oldgrid["targetpids"] = operator.rotations.targetpids
-    oldgrid["targetgrid"] = operator.rotations.targetgrid.raw
+    oldgrid["targetpids"] = operator.bases.targetpids
+    oldgrid["targetgrid"] = operator.bases.targetgrid.raw
     # The EKO contains the rotation matrix but we pass the list of
     # evol basis pids to pineappl.
     oldgrid["inputpids"] = basis_rotation.evol_basis_pids
-    oldgrid["inputgrid"] = operator.rotations.inputgrid.raw
+    oldgrid["inputgrid"] = operator.bases.inputgrid.raw
 
     return oldgrid
```

### Comparing `pineko-0.3.3/src/pineko/evolve.py` & `pineko-0.4.0/src/pineko/evolve.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import numpy as np
 import pineappl
 import rich
 import rich.box
 import rich.panel
 import yaml
 from eko.io.types import ScaleVariationsMethod
+from eko.matchings import Atlas, nf_default
+from eko.quantities import heavy_quarks
 
 from . import check, comparator, ekompatibility, version
 
 
 def sv_scheme(tcard):
     """Infere the factorization scale_variation scheme to be used from the theory card.
 
@@ -94,33 +96,50 @@
     -------
     x_grid : np.ndarray
         written x grid
     q2_grid : np.ndarray
         written Q2 grid
 
     """
+    # Add a +1 to the orders for the difference in convention between nnpdf and pineappl
+    is_fns = int(check.is_fonll_b(tcard["FNS"], pineappl_grid.lumi()))
+    max_as = 1 + tcard["PTO"] + is_fns
+    max_al = 1 + tcard["QED"]
+    # ... in order to create a mask ...
+    order_mask = pineappl.grid.Order.create_mask(
+        pineappl_grid.orders(), max_as, max_al, True
+    )
+    # ... to get the x and muF grids for the eko
+    evol_info = pineappl_grid.evolve_info(order_mask)
+    muf2_grid = evol_info.fac1
     operators_card = copy.deepcopy(default_card)
-    x_grid, _pids, _mur2_grid, muf2_grid = pineappl_grid.axes()
     sv_method = sv_scheme(tcard)
-    xif = 1.0 if sv_method == "expanded" else tcard["XIF"]
+    xif = 1.0 if sv_method is not None else tcard["XIF"]
     operators_card["configs"]["scvar_method"] = sv_method
     q2_grid = (xif * xif * muf2_grid).tolist()
-    operators_card["_mugrid"] = np.sqrt(q2_grid).tolist()
-    # If we are computing and integrability FK we want to add a single
-    # x point to the xgrid and decrease the interpolation polynonial
-    # degree to 1
+    masses = np.array([tcard["mc"], tcard["mb"], tcard["mt"]]) ** 2
+    thresholds_ratios = np.array([tcard["kcThr"], tcard["kbThr"], tcard["ktThr"]]) ** 2
+    for q in range(tcard["MaxNfPdf"] + 1, 6 + 1):
+        thresholds_ratios[q - 4] = np.inf
+    atlas = Atlas(
+        matching_scales=heavy_quarks.MatchingScales(masses * thresholds_ratios),
+        origin=(tcard["Q0"] ** 2, tcard["nf0"]),
+    )
+    operators_card["mugrid"] = [
+        (float(np.sqrt(q2)), int(nf_default(q2, atlas))) for q2 in q2_grid
+    ]
     if "integrability_version" in pineappl_grid.key_values():
+        x_grid = evol_info.x1
+        x_grid = np.append(x_grid, 1.0)
         operators_card["configs"]["interpolation_polynomial_degree"] = 1
-        x_grid_int = copy.deepcopy(x_grid.tolist())
-        x_grid_int.append(1.0)
-        operators_card["rotations"]["_targetgrid"] = list(x_grid_int)
+        operators_card["xgrid"] = x_grid.tolist()
 
     with open(card_path, "w", encoding="UTF-8") as f:
         yaml.safe_dump(operators_card, f)
-    return x_grid, q2_grid
+    return operators_card["xgrid"], q2_grid
 
 
 def evolve_grid(
     grid,
     operators,
     fktable_path,
     max_as,
@@ -149,61 +168,58 @@
     xif : float
         factorization scale variation
     assumptions : str
         assumptions on the flavor dimension
     comparison_pdf : None or str
         if given, a comparison table (with / without evolution) will be printed
     """
-    x_grid, _pids, mur2_grid, _muf2_grid = grid.axes()
-    sv_method = None
-    if operators.operator_card.configs.scvar_method is not None:
-        sv_method = operators.operator_card.configs.scvar_method.name
-    xif = 1.0 if sv_method == "EXPANDED" else xif
+    order_mask = pineappl.grid.Order.create_mask(grid.orders(), max_as, max_al, True)
+    evol_info = grid.evolve_info(order_mask)
+    x_grid = evol_info.x1
+    mur2_grid = evol_info.ren1
+    xif = 1.0 if operators.operator_card.configs.scvar_method is not None else xif
     tcard = operators.theory_card
     opcard = operators.operator_card
     # rotate the targetgrid
+    if "integrability_version" in grid.key_values():
+        x_grid = np.append(x_grid, 1.0)
     eko.io.manipulate.xgrid_reshape(
         operators, targetgrid=eko.interpolation.XGrid(x_grid)
     )
-    check.check_grid_and_eko_compatible(grid, operators, xif)
+    check.check_grid_and_eko_compatible(grid, operators, xif, max_as, max_al)
     # rotate to evolution (if doable and necessary)
-    if np.allclose(operators.rotations.inputpids, br.flavor_basis_pids):
+    if np.allclose(operators.bases.inputpids, br.flavor_basis_pids):
         eko.io.manipulate.to_evol(operators)
     # Here we are checking if the EKO contains the rotation matrix (flavor to evol)
-    elif not np.allclose(operators.rotations.inputpids, br.rotate_flavor_to_evolution):
+    elif not np.allclose(operators.bases.inputpids, br.rotate_flavor_to_evolution):
         raise ValueError("The EKO is neither in flavor nor in evolution basis.")
-    # do it
-    order_mask = pineappl.grid.Order.create_mask(grid.orders(), max_as, max_al)
-    # This is really the facto scale grid only for scheme A and C
-    muf2_grid = operators.mu2grid
     # PineAPPL wants alpha_s = 4*pi*a_s
     # remember that we already accounted for xif in the opcard generation
     evmod = eko.couplings.couplings_mod_ev(opcard.configs.evolution_method)
     # Couplings ask for the square of the masses
-    quark_masses = [(x.value) ** 2 for x in tcard.quark_masses]
+    thresholds_ratios = np.power(tcard.heavy.matching_ratios, 2.0)
+    for q in range(tcard.couplings.max_num_flavs + 1, 6 + 1):
+        thresholds_ratios[q - 4] = np.inf
     sc = eko.couplings.Couplings(
         tcard.couplings,
         tcard.order,
         evmod,
-        quark_masses,
-        hqm_scheme=tcard.quark_masses_scheme,
-        thresholds_ratios=np.power(list(iter(tcard.matching)), 2.0),
+        masses=[(x.value) ** 2 for x in tcard.heavy.masses],
+        hqm_scheme=tcard.heavy.masses_scheme,
+        thresholds_ratios=thresholds_ratios.tolist(),
     )
-    # If we are computing scheme A we also need to pass fact_scale.
-
     # To compute the alphas values we are first reverting the factorization scale shift
     # and then obtaining the renormalization scale using xir.
     alphas_values = [
         4.0
         * np.pi
         * sc.a_s(
-            xir * xir * muf2 / xif / xif,
-            fact_scale=muf2 if sv_method == "EXPONENTIATED" else None,
+            xir * xir * mur2,
         )
-        for muf2 in muf2_grid
+        for mur2 in mur2_grid
     ]
     # We need to use ekompatibility in order to pass a dictionary to pineappl
     fktable = grid.evolve(
         ekompatibility.pineappl_layout(operators),
         xir * xir * mur2_grid,
         alphas_values,
         "evol",
```

### Comparing `pineko-0.3.3/src/pineko/parser.py` & `pineko-0.4.0/src/pineko/parser.py`

 * *Files identical despite different names*

### Comparing `pineko-0.3.3/src/pineko/scaffold.py` & `pineko-0.4.0/src/pineko/scaffold.py`

 * *Files identical despite different names*

### Comparing `pineko-0.3.3/src/pineko/theory.py` & `pineko-0.4.0/src/pineko/theory.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,29 @@
 import eko
 import eko.io.legacy
 import numpy as np
 import pineappl
 import rich
 import yaml
 
-from . import check, configs, evolve, parser, theory_card
+from . import check, configs, evolve, parser, scale_variations, theory_card
 
 logger = logging.getLogger(__name__)
 
 
+def check_scvar_evolve(grid, max_as, max_al, kind: check.Scale):
+    """Check scale variations and central orders consistency."""
+    available, max_as_effective = check.contains_sv(grid, max_as, max_al, kind)
+    if max_as == max_as_effective:
+        if available is check.AvailableAtMax.SCVAR:
+            raise ValueError("Central order is not available but sv order is.")
+    if max_as < max_as_effective and available is not check.AvailableAtMax.BOTH:
+        raise ValueError("No available central order or sv order.")
+
+
 class TheoryBuilder:
     """Common builder application to create the ingredients for a theory.
 
     Parameters
     ----------
     theory_id : int
         theory identifier
@@ -36,14 +46,15 @@
     overwrite : bool
         allow files to be overwritten instead of skipping
     """
 
     def __init__(
         self, theory_id, datasets, silent=False, clear_logs=False, overwrite=False
     ):
+        """Initialize theory object."""
         self.theory_id = theory_id
         self.datasets = datasets
         self.silent = silent
         self.clear_logs = clear_logs
         self.overwrite = overwrite
 
     @property
@@ -310,14 +321,16 @@
         new_theory = legacy_class.new_theory
         new_op = eko.io.runcards.OperatorCard.from_dict(ocard)
         eko_filename = self.ekos_path() / f"{name}.tar"
         if eko_filename.exists():
             if not self.overwrite:
                 rich.print(f"Skipping existing operator {eko_filename}")
                 return
+            else:
+                eko_filename.unlink()
         # do it!
         logger.info("Start computation of %s", name)
         start_time = time.perf_counter()
         # Actual computation of the EKO
         eko.runner.solve(new_theory, new_op, eko_filename)
         logger.info(
             "Finished computation of %s - took %f s",
@@ -374,26 +387,18 @@
             tcard["FNS"],
             grid.lumi(),
         ):
             max_as += 1
         max_al = 0
         # check for sv
         if not np.isclose(xir, 1.0):
-            is_ren_as, is_ren_al = check.contains_ren(grid, max_as, max_al)
-            if not (is_ren_as and is_ren_al):
-                raise ValueError(
-                    "Renormalization scale variations are not available for this grid"
-                )
+            check_scvar_evolve(grid, max_as, max_al, check.Scale.REN)
         if sv_method is None:
             if not np.isclose(xif, 1.0):
-                is_fact_as, is_fact_al = check.contains_fact(grid, max_as, max_al)
-                if not (is_fact_as and is_fact_al):
-                    raise ValueError(
-                        "Factorization scale variations are not available for this grid"
-                    )
+                check_scvar_evolve(grid, max_as, max_al, check.Scale.FACT)
         # loading ekos
         with eko.EKO.edit(eko_filename) as operators:
             # Obtain the assumptions hash
             assumptions = theory_card.construct_assumptions(tcard)
             # do it!
             logger.info("Start computation of %s", name)
             logger.info(
@@ -442,7 +447,18 @@
         ----------
         pdf : str
             comparison PDF
         """
         tcard = theory_card.load(self.theory_id)
         self.fks_path.mkdir(exist_ok=True)
         self.iterate(self.fk, tcard=tcard, pdf=pdf)
+
+    def construct_ren_sv_grids(self, flavors):
+        """Construct renormalization scale variations terms for all the grids in a dataset."""
+        tcard = theory_card.load(self.theory_id)
+        self.iterate(self.construct_ren_sv_grid, tcard=tcard, flavors=flavors)
+
+    def construct_ren_sv_grid(self, name, grid_path, tcard, flavors):
+        """Construct renormalization scale variations terms for a grid."""
+        max_as = int(tcard["PTO"])
+        rich.print(f"Computing renormalization scale variations for {name}")
+        scale_variations.compute_ren_sv_grid(grid_path, max_as, flavors)
```

### Comparing `pineko-0.3.3/src/pineko/theory_card.py` & `pineko-0.4.0/src/pineko/theory_card.py`

 * *Files identical despite different names*

### Comparing `pineko-0.3.3/setup.py` & `pineko-0.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pineko
+Version: 0.4.0
+Summary: Combine PineAPPL grids and EKOs into FK tables
+Home-page: https://github.com/N3PDF/pineko
+Author: Alessandro Candido
+Author-email: alessandro.candido@mi.infn.it
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Provides-Extra: docs
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: Sphinx (>=4.3.2,<5.0.0) ; extra == "docs"
+Requires-Dist: click (>=8.0.4,<9.0.0)
+Requires-Dist: eko (>=0.13.2,<0.14.0)
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: pandas (>=1.4.1,<2.0.0)
+Requires-Dist: pineappl (>=0.6.0a17,<0.7.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex (>=2.4.1,<3.0.0) ; extra == "docs"
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Project-URL: Repository, https://github.com/N3PDF/pineko
+Description-Content-Type: text/markdown
+
+<p align="center">
+  <a href="https://pineko.readthedocs.io/"><img alt="PINEKO" src="https://raw.githubusercontent.com/N3PDF/pineko/main/docs/source/img/Logo.png" width=200></a>
+</p>
+
+<p align="center">
+  <a href="https://github.com/N3PDF/pineko/actions/workflows/unittests.yml"><img alt="Tests" src="https://github.com/N3PDF/pineko/actions/workflows/unittests.yml/badge.svg" /></a>
+  <a href="https://pineko.readthedocs.io/en/latest/?badge=latest"><img alt="Docs" src="https://readthedocs.org/projects/pineko/badge/?version=latest"></a>
+  <a href="https://codecov.io/gh/NNPDF/pineko"><img src="https://codecov.io/gh/NNPDF/pineko/branch/main/graph/badge.svg" /></a>
+  <a href="https://www.codefactor.io/repository/github/nnpdf/pineko"><img src="https://www.codefactor.io/repository/github/nnpdf/pineko/badge" alt="CodeFactor" /></a>
+</p>
+
+PINEKO is a Python module to produce fktables from interpolation grids and EKOs.
+
+## Installation
+PINEKO is available via
+- PyPI: <a href="https://pypi.org/project/pineko/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pineko"/></a>
+```bash
+pip install pineko
+```
+
+### Development
+
+If you want to install from source you can run
+```bash
+git clone git@github.com:N3PDF/pineko.git
+cd pineko
+poetry install
+```
+
+To setup `poetry`, and other tools, see [Contribution
+Guidelines](https://github.com/N3PDF/pineko/blob/main/.github/CONTRIBUTING.md).
+
+## Documentation
+- The documentation is available here: <a href="https://pineko.readthedocs.io/en/latest/"><img alt="Docs" src="https://readthedocs.org/projects/pineko/badge/?version=latest"></a>
+- To build the documentation from source run
+```bash
+cd docs
+poetry run make html
+```
+
+## Tests and benchmarks
+- To run unit test you can do
+```bash
+poetry run pytest
+```
+
+## Contributing
+- Your feedback is welcome! If you want to report a (possible) bug or want to ask for a new feature, please raise an issue: <a href="https://github.com/N3PDF/pineko/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/N3PDF/pineko"/></a>
+- Please follow our [Code of Conduct](https://github.com/N3PDF/pineko/blob/main/.github/CODE_OF_CONDUCT.md) and read the
+  [Contribution Guidelines](https://github.com/N3PDF/pineko/blob/main/.github/CONTRIBUTING.md)
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['pineko', 'pineko.cli']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'click>=8.0.4,<9.0.0',
- 'eko>=0.12.0,<0.13.0',
- 'numpy>=1.21.0,<2.0.0',
- 'pandas>=1.4.1,<2.0.0',
- 'pineappl>=0.5.9,<0.6.0',
- 'rich>=12.5.1,<13.0.0',
- 'tomli>=2.0.1,<3.0.0']
-
-extras_require = \
-{'docs': ['Sphinx>=4.3.2,<5.0.0',
-          'sphinx-rtd-theme>=1.0.0,<2.0.0',
-          'sphinxcontrib-bibtex>=2.4.1,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['pineko = pineko:command']}
-
-setup_kwargs = {
-    'name': 'pineko',
-    'version': '0.3.3',
-    'description': 'Combine PineAPPL grids and EKOs into FK tables',
-    'long_description': '<p align="center">\n  <a href="https://pineko.readthedocs.io/"><img alt="PINEKO" src="https://raw.githubusercontent.com/N3PDF/pineko/main/docs/source/img/Logo.png" width=200></a>\n</p>\n\n<p align="center">\n  <a href="https://github.com/N3PDF/pineko/actions/workflows/unittests.yml"><img alt="Tests" src="https://github.com/N3PDF/pineko/actions/workflows/unittests.yml/badge.svg" /></a>\n  <a href="https://pineko.readthedocs.io/en/latest/?badge=latest"><img alt="Docs" src="https://readthedocs.org/projects/pineko/badge/?version=latest"></a>\n  <a href="https://codecov.io/gh/NNPDF/pineko"><img src="https://codecov.io/gh/NNPDF/pineko/branch/main/graph/badge.svg" /></a>\n  <a href="https://www.codefactor.io/repository/github/nnpdf/pineko"><img src="https://www.codefactor.io/repository/github/nnpdf/pineko/badge" alt="CodeFactor" /></a>\n</p>\n\nPINEKO is a Python module to produce fktables from interpolation grids and EKOs.\n\n## Installation\nPINEKO is available via\n- PyPI: <a href="https://pypi.org/project/pineko/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pineko"/></a>\n```bash\npip install pineko\n```\n\n### Development\n\nIf you want to install from source you can run\n```bash\ngit clone git@github.com:N3PDF/pineko.git\ncd pineko\npoetry install\n```\n\nTo setup `poetry`, and other tools, see [Contribution\nGuidelines](https://github.com/N3PDF/pineko/blob/main/.github/CONTRIBUTING.md).\n\n## Documentation\n- The documentation is available here: <a href="https://pineko.readthedocs.io/en/latest/"><img alt="Docs" src="https://readthedocs.org/projects/pineko/badge/?version=latest"></a>\n- To build the documentation from source run\n```bash\ncd docs\npoetry run make html\n```\n\n## Tests and benchmarks\n- To run unit test you can do\n```bash\npoetry run pytest\n```\n\n## Contributing\n- Your feedback is welcome! If you want to report a (possible) bug or want to ask for a new feature, please raise an issue: <a href="https://github.com/N3PDF/pineko/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/N3PDF/pineko"/></a>\n- Please follow our [Code of Conduct](https://github.com/N3PDF/pineko/blob/main/.github/CODE_OF_CONDUCT.md) and read the\n  [Contribution Guidelines](https://github.com/N3PDF/pineko/blob/main/.github/CONTRIBUTING.md)\n',
-    'author': 'Alessandro Candido',
-    'author_email': 'alessandro.candido@mi.infn.it',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/N3PDF/pineko',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['pineko', 'pineko.cli'] package_data = \ {'': ['*']}
-install_requires = \ ['PyYAML>=6.0,<7.0', 'click>=8.0.4,<9.0.0',
-'eko>=0.12.0,<0.13.0', 'numpy>=1.21.0,<2.0.0', 'pandas>=1.4.1,<2.0.0',
-'pineappl>=0.5.9,<0.6.0', 'rich>=12.5.1,<13.0.0', 'tomli>=2.0.1,<3.0.0']
-extras_require = \ {'docs': ['Sphinx>=4.3.2,<5.0.0', 'sphinx-rtd-
-theme>=1.0.0,<2.0.0', 'sphinxcontrib-bibtex>=2.4.1,<3.0.0']} entry_points = \
-{'console_scripts': ['pineko = pineko:command']} setup_kwargs = { 'name':
-'pineko', 'version': '0.3.3', 'description': 'Combine PineAPPL grids and EKOs
-into FK tables', 'long_description': '
-                                 \n [PINEKO]\n
-\n\n
- \n [Tests]\n [Docs]\n [https://codecov.io/gh/NNPDF/pineko/branch/main/graph/
-                          badge.svg]\n [CodeFactor]\n
-\n\nPINEKO is a Python module to produce fktables from interpolation grids and
-EKOs.\n\n## Installation\nPINEKO is available via\n- PyPI: [PyPI]\n```bash\npip
-install pineko\n```\n\n### Development\n\nIf you want to install from source
-you can run\n```bash\ngit clone git@github.com:N3PDF/pineko.git\ncd
-pineko\npoetry install\n```\n\nTo setup `poetry`, and other tools, see
-[Contribution\nGuidelines](https://github.com/N3PDF/pineko/blob/main/.github/
-CONTRIBUTING.md).\n\n## Documentation\n- The documentation is available here:
-[Docs]\n- To build the documentation from source run\n```bash\ncd docs\npoetry
-run make html\n```\n\n## Tests and benchmarks\n- To run unit test you can
-do\n```bash\npoetry run pytest\n```\n\n## Contributing\n- Your feedback is
-welcome! If you want to report a (possible) bug or want to ask for a new
-feature, please raise an issue: [GitHub_issues]\n- Please follow our [Code of
-Conduct](https://github.com/N3PDF/pineko/blob/main/.github/CODE_OF_CONDUCT.md)
-and read the\n [Contribution Guidelines](https://github.com/N3PDF/pineko/blob/
-main/.github/CONTRIBUTING.md)\n', 'author': 'Alessandro Candido',
-'author_email': 'alessandro.candido@mi.infn.it', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/N3PDF/pineko',
-'package_dir': package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'entry_points': entry_points, 'python_requires': '>=3.8,<3.11', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: pineko Version: 0.4.0 Summary: Combine PineAPPL
+grids and EKOs into FK tables Home-page: https://github.com/N3PDF/pineko
+Author: Alessandro Candido Author-email: alessandro.candido@mi.infn.it
+Requires-Python: >=3.8,<3.12 Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics Provides-Extra: docs
+Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: Sphinx (>=4.3.2,<5.0.0) ;
+extra == "docs" Requires-Dist: click (>=8.0.4,<9.0.0) Requires-Dist: eko
+(>=0.13.2,<0.14.0) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-Dist: pandas
+(>=1.4.1,<2.0.0) Requires-Dist: pineappl (>=0.6.0a17,<0.7.0) Requires-Dist:
+rich (>=12.5.1,<13.0.0) Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ;
+extra == "docs" Requires-Dist: sphinxcontrib-bibtex (>=2.4.1,<3.0.0) ; extra ==
+"docs" Requires-Dist: tomli (>=2.0.1,<3.0.0) Project-URL: Repository, https://
+github.com/N3PDF/pineko Description-Content-Type: text/markdown
+                                   [PINEKO]
+[Tests] [Docs] [https://codecov.io/gh/NNPDF/pineko/branch/main/graph/badge.svg]
+                                 [CodeFactor]
+PINEKO is a Python module to produce fktables from interpolation grids and
+EKOs. ## Installation PINEKO is available via - PyPI: [PyPI] ```bash pip
+install pineko ``` ### Development If you want to install from source you can
+run ```bash git clone git@github.com:N3PDF/pineko.git cd pineko poetry install
+``` To setup `poetry`, and other tools, see [Contribution Guidelines](https://
+github.com/N3PDF/pineko/blob/main/.github/CONTRIBUTING.md). ## Documentation -
+The documentation is available here: [Docs] - To build the documentation from
+source run ```bash cd docs poetry run make html ``` ## Tests and benchmarks -
+To run unit test you can do ```bash poetry run pytest ``` ## Contributing -
+Your feedback is welcome! If you want to report a (possible) bug or want to ask
+for a new feature, please raise an issue: [GitHub_issues] - Please follow our
+[Code of Conduct](https://github.com/N3PDF/pineko/blob/main/.github/
+CODE_OF_CONDUCT.md) and read the [Contribution Guidelines](https://github.com/
+N3PDF/pineko/blob/main/.github/CONTRIBUTING.md)
```

