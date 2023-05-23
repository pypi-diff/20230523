# Comparing `tmp/qm-sim-0.1.0.tar.gz` & `tmp/qm-sim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qm-sim-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "qm-sim-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `qm-sim-0.1.0.tar` & `qm-sim-0.1.1.tar`

### file list

```diff
@@ -1,2033 +1,59 @@
--rw-r--r--   0        0        0      679 2022-11-09 12:37:21.000000 qm-sim-0.1.0/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 qm-sim-0.1.0/.gitignore
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 qm-sim-0.1.0/.gitmodules
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 qm-sim-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 qm-sim-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 qm-sim-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 qm-sim-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      315 2022-11-09 12:37:21.000000 qm-sim-0.1.0/CMakeLists.txt
--rwxr-xr-x   0        0        0      804 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/make.bat
--rw-r--r--   0        0        0      658 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1285 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/source/api.rst
--rw-r--r--   0        0        0     1175 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0     1105 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/source/contribution.rst
--rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/source/examples.rst
--rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 qm-sim-0.1.0/docs/source/usage.rst
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 qm-sim-0.1.0/examples/01_zero_potential.py
--rw-r--r--   0        0        0      629 2022-11-09 12:37:21.000000 qm-sim-0.1.0/examples/02_quadratic_potential.py
--rw-r--r--   0        0        0      763 2022-11-09 12:37:21.000000 qm-sim-0.1.0/examples/03_2D_potential.py
--rw-r--r--   0        0        0     1699 2022-11-09 12:37:21.000000 qm-sim-0.1.0/examples/04_adiabatic_evolution.py
--rw-r--r--   0        0        0      705 2022-11-09 12:37:21.000000 qm-sim-0.1.0/examples/05_temporal_evolution.py
--rw-r--r--   0        0        0     1378 2022-11-09 12:37:21.000000 qm-sim-0.1.0/examples/06_2D_temporal_evolution.py
--rw-r--r--   0        0        0     1447 2022-11-09 12:37:21.000000 qm-sim-0.1.0/examples/07_hydrogen_atom.py
--rw-r--r--   0        0        0      228 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/.clang-format
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/.git
--rw-r--r--   0        0        0      354 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/.gitignore
--rw-r--r--   0        0        0     2813 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/.gitlab/issue_templates/Bug Report.md
--rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/.gitlab/issue_templates/Feature Request.md
--rw-r--r--   0        0        0     1420 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/.gitlab/merge_request_templates/Merge Request Template.md
--rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/.gitlab-ci.yml
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/.hgeol
--rw-r--r--   0        0        0    29859 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/analyze-blocking-sizes.cpp
--rw-r--r--   0        0        0     1449 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/basicbench.cxxlist
--rw-r--r--   0        0        0     1142 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/basicbenchmark.cpp
--rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/basicbenchmark.h
--rw-r--r--   0        0        0    11810 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/bench_gemm.cpp
--rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/bench_move_semantics.cpp
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/bench_multi_compilers.sh
--rw-r--r--   0        0        0    11982 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/bench_norm.cpp
--rw-r--r--   0        0        0     2243 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/bench_reverse.cpp
--rw-r--r--   0        0        0      338 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/bench_sum.cpp
--rw-r--r--   0        0        0      663 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/bench_unrolling
--rw-r--r--   0        0        0     6532 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchBlasGemm.cpp
--rw-r--r--   0        0        0     3689 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchCholesky.cpp
--rw-r--r--   0        0        0     6000 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchEigenSolver.cpp
--rw-r--r--   0        0        0     2921 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchFFT.cpp
--rw-r--r--   0        0        0     3732 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchGeometry.cpp
--rw-r--r--   0        0        0    22936 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchmark-blocking-sizes.cpp
--rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchmark.cpp
--rw-r--r--   0        0        0     1227 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchmark_suite
--rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchmarkSlice.cpp
--rw-r--r--   0        0        0      676 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchmarkX.cpp
--rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchmarkXcwise.cpp
--rw-r--r--   0        0        0     4081 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/BenchSparseUtil.h
--rw-r--r--   0        0        0     4685 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/BenchTimer.h
--rw-r--r--   0        0        0     2621 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/BenchUtil.h
--rw-r--r--   0        0        0     5328 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/benchVecAdd.cpp
--rw-r--r--   0        0        0     3519 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_aat_product.hh
--rw-r--r--   0        0        0     3499 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_ata_product.hh
--rw-r--r--   0        0        0     3804 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_atv_product.hh
--rw-r--r--   0        0        0     3498 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_axpby.hh
--rw-r--r--   0        0        0     3479 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_axpy.hh
--rw-r--r--   0        0        0     3330 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_cholesky.hh
--rw-r--r--   0        0        0     3588 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_ger.hh
--rw-r--r--   0        0        0     5831 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_hessenberg.hh
--rw-r--r--   0        0        0     3275 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_lu_decomp.hh
--rw-r--r--   0        0        0     3734 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_lu_solve.hh
--rw-r--r--   0        0        0     4036 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_matrix_matrix_product.hh
--rw-r--r--   0        0        0     4134 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_matrix_matrix_product_bis.hh
--rw-r--r--   0        0        0     4142 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_matrix_vector_product.hh
--rw-r--r--   0        0        0     3313 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_partial_lu.hh
--rw-r--r--   0        0        0     3135 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_rot.hh
--rw-r--r--   0        0        0     3830 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_symv.hh
--rw-r--r--   0        0        0     3797 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_syr2.hh
--rw-r--r--   0        0        0     3562 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_trisolve.hh
--rw-r--r--   0        0        0     4226 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_trisolve_matrix.hh
--rw-r--r--   0        0        0     4072 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/action_trmm.hh
--rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/actions/basic_actions.hh
--rw-r--r--   0        0        0      969 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindACML.cmake
--rw-r--r--   0        0        0     1321 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindATLAS.cmake
--rw-r--r--   0        0        0      812 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindBLAZE.cmake
--rw-r--r--   0        0        0     1098 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindBlitz.cmake
--rw-r--r--   0        0        0      669 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindCBLAS.cmake
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindGMM.cmake
--rw-r--r--   0        0        0     1297 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindMKL.cmake
--rw-r--r--   0        0        0      818 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindMTL4.cmake
--rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindOPENBLAS.cmake
--rw-r--r--   0        0        0     2432 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/FindTvmet.cmake
--rw-r--r--   0        0        0     1346 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
--rw-r--r--   0        0        0     2889 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/CMakeLists.txt
--rw-r--r--   0        0        0    18449 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/COPYING
--rw-r--r--   0        0        0     1387 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/action_settings.txt
--rw-r--r--   0        0        0      901 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/CMakeLists.txt
--rw-r--r--   0        0        0     2311 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/gnuplot_common_settings.hh
--rw-r--r--   0        0        0     2149 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/go_mean
--rw-r--r--   0        0        0     5488 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/mean.cxx
--rw-r--r--   0        0        0     1918 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/mk_gnuplot_script.sh
--rw-r--r--   0        0        0      981 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/mk_mean_script.sh
--rw-r--r--   0        0        0     1796 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/mk_new_gnuplot.sh
--rw-r--r--   0        0        0      990 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/perlib_plot_settings.txt
--rw-r--r--   0        0        0     3556 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/regularize.cxx
--rw-r--r--   0        0        0     5310 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/smooth.cxx
--rw-r--r--   0        0        0     1755 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/data/smooth_all.sh
--rw-r--r--   0        0        0     4995 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/bench.hh
--rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/bench_parameter.hh
--rw-r--r--   0        0        0     6990 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/btl.hh
--rw-r--r--   0        0        0     1532 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/init/init_function.hh
--rw-r--r--   0        0        0     2359 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/init/init_matrix.hh
--rw-r--r--   0        0        0     1453 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/init/init_vector.hh
--rw-r--r--   0        0        0     2358 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/static/bench_static.hh
--rw-r--r--   0        0        0     2014 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
--rw-r--r--   0        0        0     2279 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/static/static_size_generator.hh
--rw-r--r--   0        0        0     2067 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
--rw-r--r--   0        0        0     3041 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
--rw-r--r--   0        0        0     3668 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
--rw-r--r--   0        0        0     3721 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/timers/portable_timer.hh
--rw-r--r--   0        0        0     2387 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
--rw-r--r--   0        0        0     2600 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/timers/STL_timer.hh
--rw-r--r--   0        0        0     3035 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
--rw-r--r--   0        0        0     5540 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/timers/x86_timer.hh
--rw-r--r--   0        0        0     1728 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/utils/size_lin_log.hh
--rw-r--r--   0        0        0     1700 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/utils/size_log.hh
--rw-r--r--   0        0        0     2835 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/utils/utilities.h
--rw-r--r--   0        0        0     2289 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/generic_bench/utils/xy_file.hh
--rw-r--r--   0        0        0    35833 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/BLAS/blas.h
--rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/BLAS/blas_interface.hh
--rw-r--r--   0        0        0     4958 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/BLAS/blas_interface_impl.hh
--rw-r--r--   0        0        0     1707 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/BLAS/c_interface_base.h
--rw-r--r--   0        0        0     1515 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/BLAS/CMakeLists.txt
--rw-r--r--   0        0        0     3033 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/BLAS/main.cpp
--rw-r--r--   0        0        0     4263 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/blaze/blaze_interface.hh
--rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/blaze/CMakeLists.txt
--rw-r--r--   0        0        0     1676 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/blaze/main.cpp
--rw-r--r--   0        0        0     4276 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/blitz/blitz_interface.hh
--rw-r--r--   0        0        0     5556 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
--rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/blitz/btl_blitz.cpp
--rw-r--r--   0        0        0     1431 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/blitz/btl_tiny_blitz.cpp
--rw-r--r--   0        0        0      395 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/blitz/CMakeLists.txt
--rw-r--r--   0        0        0     3206 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/blitz/tiny_blitz_interface.hh
--rw-r--r--   0        0        0     1710 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
--rw-r--r--   0        0        0      787 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen2/CMakeLists.txt
--rw-r--r--   0        0        0     5319 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen2/eigen2_interface.hh
--rw-r--r--   0        0        0     1843 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen2/main_adv.cpp
--rw-r--r--   0        0        0     1239 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen2/main_linear.cpp
--rw-r--r--   0        0        0     1419 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen2/main_matmat.cpp
--rw-r--r--   0        0        0     1492 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen2/main_vecmat.cpp
--rw-r--r--   0        0        0     1710 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
--rw-r--r--   0        0        0     3272 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen3/CMakeLists.txt
--rw-r--r--   0        0        0     8429 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen3/eigen3_interface.hh
--rw-r--r--   0        0        0     1843 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen3/main_adv.cpp
--rw-r--r--   0        0        0     1320 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen3/main_linear.cpp
--rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen3/main_matmat.cpp
--rw-r--r--   0        0        0     1483 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/eigen3/main_vecmat.cpp
--rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/gmm/CMakeLists.txt
--rw-r--r--   0        0        0     4318 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/gmm/gmm_interface.hh
--rw-r--r--   0        0        0     5556 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
--rw-r--r--   0        0        0     2164 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/gmm/main.cpp
--rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/mtl4/.kdbgrc.main
--rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/mtl4/CMakeLists.txt
--rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/mtl4/main.cpp
--rw-r--r--   0        0        0     4354 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/mtl4/mtl4_interface.hh
--rw-r--r--   0        0        0     5556 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/STL/CMakeLists.txt
--rw-r--r--   0        0        0     1870 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/STL/main.cpp
--rw-r--r--   0        0        0     6079 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/STL/STL_interface.hh
--rw-r--r--   0        0        0     2174 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/tensors/CMakeLists.txt
--rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/tensors/main_linear.cpp
--rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/tensors/main_matmat.cpp
--rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/tensors/main_vecmat.cpp
--rw-r--r--   0        0        0     3295 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/tensors/tensor_interface.hh
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/tvmet/CMakeLists.txt
--rw-r--r--   0        0        0     1500 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/tvmet/main.cpp
--rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/tvmet/tvmet_interface.hh
--rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/ublas/CMakeLists.txt
--rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/ublas/main.cpp
--rw-r--r--   0        0        0     4482 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/libs/ublas/ublas_interface.hh
--rw-r--r--   0        0        0     6601 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/btl/README
--rw-r--r--   0        0        0     3370 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/check_cache_queries.cpp
--rw-r--r--   0        0        0     6592 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/dense_solvers.cpp
--rw-r--r--   0        0        0     7438 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/eig33.cpp
--rw-r--r--   0        0        0     3433 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/geometry.cpp
--rw-r--r--   0        0        0     6669 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/changesets.txt
--rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/gemm.cpp
--rw-r--r--   0        0        0     1449 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/gemm_common.h
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/gemm_settings.txt
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/gemm_square_settings.txt
--rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/gemv.cpp
--rw-r--r--   0        0        0     1450 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/gemv_common.h
--rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/gemv_settings.txt
--rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/gemv_square_settings.txt
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/gemvt.cpp
--rw-r--r--   0        0        0     2567 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/lazy_gemm.cpp
--rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/lazy_gemm_settings.txt
--rw-r--r--   0        0        0      313 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/llt.cpp
--rw-r--r--   0        0        0     2805 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/make_plot.sh
--rw-r--r--   0        0        0     3854 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/resources/chart_footer.html
--rw-r--r--   0        0        0    14820 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/resources/chart_header.html
--rw-r--r--   0        0        0       28 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/resources/footer.html
--rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/resources/header.html
--rw-r--r--   0        0        0   151724 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/resources/s1.js
--rw-r--r--   0        0        0   241320 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/resources/s2.js
--rw-r--r--   0        0        0     4273 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/run.sh
--rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/runall.sh
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/trmv_lo.cpp
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/trmv_lot.cpp
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/trmv_up.cpp
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/perf_monitoring/trmv_upt.cpp
--rw-r--r--   0        0        0     3375 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/product_threshold.cpp
--rw-r--r--   0        0        0     6253 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/quat_slerp.cpp
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/quatmul.cpp
--rw-r--r--   0        0        0     2063 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/README.txt
--rw-r--r--   0        0        0     6476 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/sparse_cholesky.cpp
--rw-r--r--   0        0        0     5288 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/sparse_dense_product.cpp
--rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/sparse_lu.cpp
--rw-r--r--   0        0        0     9322 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/sparse_product.cpp
--rw-r--r--   0        0        0     3519 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/sparse_randomsetter.cpp
--rw-r--r--   0        0        0    14246 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/sparse_setter.cpp
--rw-r--r--   0        0        0     2451 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/sparse_transpose.cpp
--rw-r--r--   0        0        0     6334 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/sparse_trisolver.cpp
--rw-r--r--   0        0        0     3179 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/spbench/CMakeLists.txt
--rw-r--r--   0        0        0     4100 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/spbench/sp_solver.cpp
--rw-r--r--   0        0        0     1886 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/spbench/spbench.dtd
--rw-r--r--   0        0        0     3491 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/spbench/spbenchsolver.cpp
--rw-r--r--   0        0        0    18740 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/spbench/spbenchsolver.h
--rw-r--r--   0        0        0     3920 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/spbench/spbenchstyle.h
--rw-r--r--   0        0        0     2924 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/spbench/test_sparseLU.cpp
--rw-r--r--   0        0        0     6329 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/spmv.cpp
--rw-r--r--   0        0        0     1634 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/benchmark.h
--rw-r--r--   0        0        0     7071 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/benchmark_main.cc
--rw-r--r--   0        0        0     1428 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/contraction_benchmarks_cpu.cc
--rw-r--r--   0        0        0      759 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/eigen_sycl_bench.sh
--rw-r--r--   0        0        0      654 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/eigen_sycl_bench_contract.sh
--rw-r--r--   0        0        0     2221 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/README
--rw-r--r--   0        0        0    20112 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/tensor_benchmarks.h
--rw-r--r--   0        0        0     6432 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/tensor_benchmarks_cpu.cc
--rw-r--r--   0        0        0     3458 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/tensor_benchmarks_fp16_gpu.cu
--rw-r--r--   0        0        0     3448 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/tensor_benchmarks_gpu.cu
--rw-r--r--   0        0        0     6413 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/tensor_benchmarks_sycl.cc
--rw-r--r--   0        0        0    11660 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/tensors/tensor_contract_sycl_bench.cc
--rw-r--r--   0        0        0     1259 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/bench/vdw_new.cpp
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/BandTriangularSolver.h
--rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/CMakeLists.txt
--rw-r--r--   0        0        0     4822 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/common.h
--rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/complex_double.cpp
--rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/complex_single.cpp
--rw-r--r--   0        0        0     1539 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/double.cpp
--rw-r--r--   0        0        0    15595 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/chbmv.c
--rw-r--r--   0        0        0    13464 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/chpmv.c
--rw-r--r--   0        0        0     2394 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/complexdots.c
--rw-r--r--   0        0        0    19592 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/ctbmv.c
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/d_cnjg.c
--rw-r--r--   0        0        0      681 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/datatypes.h
--rw-r--r--   0        0        0     5183 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/drotm.c
--rw-r--r--   0        0        0     6486 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/drotmg.c
--rw-r--r--   0        0        0    10554 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/dsbmv.c
--rw-r--r--   0        0        0     8391 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/dspmv.c
--rw-r--r--   0        0        0    12085 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/dtbmv.c
--rw-r--r--   0        0        0     3093 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/lsame.c
--rw-r--r--   0        0        0      111 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/r_cnjg.c
--rw-r--r--   0        0        0     5118 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/srotm.c
--rw-r--r--   0        0        0     6351 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/srotmg.c
--rw-r--r--   0        0        0    10578 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/ssbmv.c
--rw-r--r--   0        0        0     8367 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/sspmv.c
--rw-r--r--   0        0        0    12071 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/stbmv.c
--rw-r--r--   0        0        0    15632 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/zhbmv.c
--rw-r--r--   0        0        0    13498 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/zhpmv.c
--rw-r--r--   0        0        0    19620 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/f2c/ztbmv.c
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/fortran/complexdots.f
--rw-r--r--   0        0        0     1652 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/GeneralRank1Update.h
--rw-r--r--   0        0        0     5757 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/level1_cplx_impl.h
--rw-r--r--   0        0        0     4036 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/level1_impl.h
--rw-r--r--   0        0        0     4389 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/level1_real_impl.h
--rw-r--r--   0        0        0    12583 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/level2_cplx_impl.h
--rw-r--r--   0        0        0    25725 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/level2_impl.h
--rw-r--r--   0        0        0    10805 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/level2_real_impl.h
--rw-r--r--   0        0        0    38747 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/level3_impl.h
--rw-r--r--   0        0        0     2089 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/PackedSelfadjointProduct.h
--rw-r--r--   0        0        0     3344 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/PackedTriangularMatrixVector.h
--rw-r--r--   0        0        0     3279 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/PackedTriangularSolverVector.h
--rw-r--r--   0        0        0     2225 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/Rank2Update.h
--rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/README.txt
--rw-r--r--   0        0        0      785 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/single.cpp
--rw-r--r--   0        0        0    32834 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/cblat1.f
--rw-r--r--   0        0        0     1581 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/cblat2.dat
--rw-r--r--   0        0        0   119936 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/cblat2.f
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/cblat3.dat
--rw-r--r--   0        0        0   135042 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/cblat3.f
--rw-r--r--   0        0        0      988 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/CMakeLists.txt
--rw-r--r--   0        0        0    45885 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/dblat1.f
--rw-r--r--   0        0        0     1500 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/dblat2.dat
--rw-r--r--   0        0        0   115511 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/dblat2.f
--rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/dblat3.dat
--rw-r--r--   0        0        0   107135 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/dblat3.f
--rw-r--r--   0        0        0     1061 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/runblastest.sh
--rw-r--r--   0        0        0    44410 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/sblat1.f
--rw-r--r--   0        0        0     1500 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/sblat2.dat
--rw-r--r--   0        0        0   115427 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/sblat2.f
--rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/sblat3.dat
--rw-r--r--   0        0        0   107045 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/sblat3.f
--rw-r--r--   0        0        0    32839 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/zblat1.f
--rw-r--r--   0        0        0     1581 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/zblat2.dat
--rw-r--r--   0        0        0   120290 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/zblat2.f
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/zblat3.dat
--rw-r--r--   0        0        0   135497 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/testing/zblat3.f
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/blas/xerbla.cpp
--rw-r--r--   0        0        0     3649 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/ci/build.gitlab-ci.yml
--rw-r--r--   0        0        0     6856 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/ci/CTest2JUnit.xsl
--rw-r--r--   0        0        0     2921 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/ci/README.md
--rw-r--r--   0        0        0     2777 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/ci/smoketests.gitlab-ci.yml
--rw-r--r--   0        0        0     6745 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/ci/test.gitlab-ci.yml
--rw-r--r--   0        0        0     2221 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/ComputeCppCompilerChecks.cmake
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/ComputeCppIRMap.cmake
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/Eigen3Config.cmake.in
--rw-r--r--   0        0        0     3303 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/EigenConfigureTesting.cmake
--rw-r--r--   0        0        0     2559 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/EigenSmokeTestList.cmake
--rw-r--r--   0        0        0    28854 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/EigenTesting.cmake
--rw-r--r--   0        0        0     1236 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/EigenUninstall.cmake
--rw-r--r--   0        0        0      874 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindAccelerate.cmake
--rw-r--r--   0        0        0      537 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindAdolc.cmake
--rw-r--r--   0        0        0    13563 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindBLASEXT.cmake
--rw-r--r--   0        0        0     2502 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindCHOLMOD.cmake
--rw-r--r--   0        0        0     2301 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindCLANG_FORMAT.cmake
--rw-r--r--   0        0        0    17140 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindComputeCpp.cmake
--rw-r--r--   0        0        0     2456 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindDPCPP.cmake
--rw-r--r--   0        0        0     2903 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindFFTW.cmake
--rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindGMP.cmake
--rw-r--r--   0        0        0      869 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindGoogleHash.cmake
--rw-r--r--   0        0        0    12061 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindHWLOC.cmake
--rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindKLU.cmake
--rw-r--r--   0        0        0     9234 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindMetis.cmake
--rw-r--r--   0        0        0     2715 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindMPFR.cmake
--rw-r--r--   0        0        0     3627 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindMPREAL.cmake
--rw-r--r--   0        0        0    23864 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindPASTIX.cmake
--rw-r--r--   0        0        0    14839 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindPTSCOTCH.cmake
--rw-r--r--   0        0        0    12404 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindSCOTCH.cmake
--rw-r--r--   0        0        0     1182 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindSPQR.cmake
--rw-r--r--   0        0        0     2552 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindStandardMathLibrary.cmake
--rw-r--r--   0        0        0     2358 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindSuperLU.cmake
--rw-r--r--   0        0        0     5284 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindTriSYCL.cmake
--rw-r--r--   0        0        0     1715 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/FindUMFPACK.cmake
--rw-r--r--   0        0        0      928 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/cmake/RegexUtils.cmake
--rw-r--r--   0        0        0    28394 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/CMakeLists.txt
--rw-r--r--   0        0        0    11564 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/COPYING.APACHE
--rw-r--r--   0        0        0     1543 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/COPYING.BSD
--rw-r--r--   0        0        0    27032 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/COPYING.LGPL
--rw-r--r--   0        0        0     2244 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/COPYING.MINPACK
--rw-r--r--   0        0        0    17100 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/COPYING.MPL2
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/COPYING.README
--rw-r--r--   0        0        0      601 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/CTestConfig.cmake
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/CTestCustom.cmake.in
--rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/debug/gdb/__init__.py
--rw-r--r--   0        0        0    10637 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/debug/gdb/printers.py
--rw-r--r--   0        0        0     9526 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/debug/lldb/eigenlldb.py
--rw-r--r--   0        0        0    11661 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/debug/msvc/eigen.natvis
--rw-r--r--   0        0        0     7566 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/debug/msvc/eigen_autoexp_part.dat
--rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/CMakeLists.txt
--rw-r--r--   0        0        0      483 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/mandelbrot/CMakeLists.txt
--rw-r--r--   0        0        0     7722 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/mandelbrot/mandelbrot.cpp
--rw-r--r--   0        0        0     1959 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/mandelbrot/mandelbrot.h
--rw-r--r--   0        0        0      346 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/mandelbrot/README
--rw-r--r--   0        0        0     4343 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/mix_eigen_and_c/binary_library.cpp
--rw-r--r--   0        0        0     3417 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/mix_eigen_and_c/binary_library.h
--rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/mix_eigen_and_c/example.c
--rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/mix_eigen_and_c/README
--rw-r--r--   0        0        0     6245 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/camera.cpp
--rw-r--r--   0        0        0     3553 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/camera.h
--rw-r--r--   0        0        0      722 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/CMakeLists.txt
--rw-r--r--   0        0        0     4100 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/gpuhelper.cpp
--rw-r--r--   0        0        0     7384 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/gpuhelper.h
--rw-r--r--   0        0        0     4047 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/icosphere.cpp
--rw-r--r--   0        0        0      899 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/icosphere.h
--rw-r--r--   0        0        0    19848 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/quaternion_demo.cpp
--rw-r--r--   0        0        0     2749 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/quaternion_demo.h
--rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/README
--rw-r--r--   0        0        0     1815 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/trackball.cpp
--rw-r--r--   0        0        0      985 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/demos/opengl/trackball.h
--rw-r--r--   0        0        0    11391 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/AsciiQuickReference.txt
--rw-r--r--   0        0        0     2477 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/B01_Experimental.dox
--rw-r--r--   0        0        0     6461 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/ClassHierarchy.dox
--rw-r--r--   0        0        0     4921 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/CMakeLists.txt
--rw-r--r--   0        0        0    19292 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/CoeffwiseMathFunctionsTable.dox
--rw-r--r--   0        0        0     4543 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/CustomizingEigen_CustomScalar.dox
--rw-r--r--   0        0        0     1371 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/CustomizingEigen_InheritingMatrix.dox
--rw-r--r--   0        0        0     3744 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/CustomizingEigen_NullaryExpr.dox
--rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/CustomizingEigen_Plugins.dox
--rw-r--r--   0        0        0     5063 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/DenseDecompositionBenchmark.dox
--rw-r--r--   0        0        0    87853 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/Doxyfile.in
--rw-r--r--   0        0        0    13478 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/eigen_navtree_hacks.js
--rw-r--r--   0        0        0     8355 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/Eigen_Silly_Professor_64x64.png
--rw-r--r--   0        0        0     4785 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/eigendoxy.css
--rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/eigendoxy_footer.html.in
--rw-r--r--   0        0        0     2304 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/eigendoxy_header.html.in
--rw-r--r--   0        0        0     5515 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/eigendoxy_layout.xml.in
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/eigendoxy_tabs.css
--rw-r--r--   0        0        0       36 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/.krazy
--rw-r--r--   0        0        0      771 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/class_Block.cpp
--rw-r--r--   0        0        0      489 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/class_CwiseBinaryOp.cpp
--rw-r--r--   0        0        0      568 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/class_CwiseUnaryOp.cpp
--rw-r--r--   0        0        0      384 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
--rw-r--r--   0        0        0      731 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/class_FixedBlock.cpp
--rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/class_FixedReshaped.cpp
--rw-r--r--   0        0        0      700 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/class_FixedVectorBlock.cpp
--rw-r--r--   0        0        0      604 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/class_Reshaped.cpp
--rw-r--r--   0        0        0      802 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/class_VectorBlock.cpp
--rw-r--r--   0        0        0      514 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/CMakeLists.txt
--rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/CustomizingEigen_Inheritance.cpp
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Cwise_erf.cpp
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Cwise_erfc.cpp
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Cwise_lgamma.cpp
--rw-r--r--   0        0        0      272 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/DenseBase_middleCols_int.cpp
--rw-r--r--   0        0        0      272 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/DenseBase_middleRows_int.cpp
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/DenseBase_template_int_middleCols.cpp
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/DenseBase_template_int_middleRows.cpp
--rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/function_taking_eigenbase.cpp
--rw-r--r--   0        0        0      625 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/function_taking_ref.cpp
--rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/make_circulant.cpp
--rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/make_circulant.cpp.entry
--rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/make_circulant.cpp.evaluator
--rw-r--r--   0        0        0      611 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/make_circulant.cpp.expression
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/make_circulant.cpp.main
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/make_circulant.cpp.preamble
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/make_circulant.cpp.traits
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/make_circulant2.cpp
--rw-r--r--   0        0        0     4404 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/matrixfree_cg.cpp
--rw-r--r--   0        0        0     2535 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/nullary_indexing.cpp
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/QuickStart_example.cpp
--rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/QuickStart_example2_dynamic.cpp
--rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/QuickStart_example2_fixed.cpp
--rw-r--r--   0        0        0      729 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TemplateKeyword_flexible.cpp
--rw-r--r--   0        0        0      542 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TemplateKeyword_simple.cpp
--rw-r--r--   0        0        0      495 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/tut_arithmetic_add_sub.cpp
--rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/tut_arithmetic_dot_cross.cpp
--rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/tut_arithmetic_matrix_mul.cpp
--rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/tut_arithmetic_redux_basic.cpp
--rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/tut_arithmetic_scalar_mul_div.cpp
--rw-r--r--   0        0        0      349 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/tut_matrix_coefficient_accessors.cpp
--rw-r--r--   0        0        0      495 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/tut_matrix_resize.cpp
--rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/tut_matrix_resize_fixed_size.cpp
--rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ArrayClass_accessors.cpp
--rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ArrayClass_addition.cpp
--rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
--rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ArrayClass_interop.cpp
--rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
--rw-r--r--   0        0        0      234 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ArrayClass_mult.cpp
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
--rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_BlockOperations_colrow.cpp
--rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_BlockOperations_corner.cpp
--rw-r--r--   0        0        0      433 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_BlockOperations_print_block.cpp
--rw-r--r--   0        0        0      362 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_BlockOperations_vector.cpp
--rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_PartialLU_solve.cpp
--rw-r--r--   0        0        0      433 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
--rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
--rw-r--r--   0        0        0      381 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
--rw-r--r--   0        0        0      260 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
--rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
--rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
--rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
--rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
--rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
--rw-r--r--   0        0        0      690 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_simple_example_dynamic_size.cpp
--rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/Tutorial_simple_example_fixed_size.cpp
--rw-r--r--   0        0        0     1669 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialInplaceLU.cpp
--rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialLinAlgComputeTwice.cpp
--rw-r--r--   0        0        0      373 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialLinAlgExComputeSolveError.cpp
--rw-r--r--   0        0        0      401 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
--rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialLinAlgExSolveLDLT.cpp
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialLinAlgInverseDeterminant.cpp
--rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialLinAlgRankRevealing.cpp
--rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
--rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialLinAlgSetThreshold.cpp
--rw-r--r--   0        0        0      455 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/examples/TutorialLinAlgSVDSolve.cpp
--rw-r--r--   0        0        0     1944 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/FixedSizeVectorizable.dox
--rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/ftv2node.png
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/ftv2pnode.png
--rw-r--r--   0        0        0    13675 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/FunctionsTakingEigenTypes.dox
--rw-r--r--   0        0        0     5557 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/HiPerformance.dox
--rw-r--r--   0        0        0     3911 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/InplaceDecomposition.dox
--rw-r--r--   0        0        0    31085 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/InsideEigenExample.dox
--rw-r--r--   0        0        0     3224 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/LeastSquares.dox
--rw-r--r--   0        0        0     6953 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/Manual.dox
--rw-r--r--   0        0        0      777 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/MatrixfreeSolverExample.dox
--rw-r--r--   0        0        0     5753 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/NewExpressionType.dox
--rw-r--r--   0        0        0     1957 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/Overview.dox
--rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/PassingByValue.dox
--rw-r--r--   0        0        0     7167 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/Pitfalls.dox
--rw-r--r--   0        0        0    13773 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/PreprocessorDirectives.dox
--rw-r--r--   0        0        0    30712 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/QuickReference.dox
--rw-r--r--   0        0        0     6684 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/QuickStartGuide.dox
--rw-r--r--   0        0        0       36 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/.krazy
--rw-r--r--   0        0        0      215 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/AngleAxis_mimic_euler.cpp
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Array_initializer_list_23_cxx11.cpp
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Array_initializer_list_vector_cxx11.cpp
--rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Array_variadic_ctor_cxx11.cpp
--rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/BiCGSTAB_simple.cpp
--rw-r--r--   0        0        0      421 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/BiCGSTAB_step_by_step.cpp
--rw-r--r--   0        0        0      748 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/class_FullPivLU.cpp
--rw-r--r--   0        0        0     1298 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/CMakeLists.txt
--rw-r--r--   0        0        0      332 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/ColPivHouseholderQR_solve.cpp
--rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/compile_snippet.cpp.in
--rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/ComplexEigenSolver_compute.cpp
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
--rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
--rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/ComplexSchur_compute.cpp
--rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/ComplexSchur_matrixT.cpp
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/ComplexSchur_matrixU.cpp
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_abs.cpp
--rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_abs2.cpp
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_acos.cpp
--rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_arg.cpp
--rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_array_atan2_array.cpp
--rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_array_power_array.cpp
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_asin.cpp
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_atan.cpp
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_boolean_and.cpp
--rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_boolean_not.cpp
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_boolean_or.cpp
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_boolean_xor.cpp
--rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_ceil.cpp
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_cos.cpp
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_cosh.cpp
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_cube.cpp
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_equal_equal.cpp
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_exp.cpp
--rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_floor.cpp
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_greater.cpp
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_greater_equal.cpp
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_inverse.cpp
--rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_isFinite.cpp
--rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_isInf.cpp
--rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_isNaN.cpp
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_less.cpp
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_less_equal.cpp
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_log.cpp
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_log10.cpp
--rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_max.cpp
--rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_min.cpp
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_minus.cpp
--rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_minus_equal.cpp
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_not_equal.cpp
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_plus.cpp
--rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_plus_equal.cpp
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_pow.cpp
--rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_product.cpp
--rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_quotient.cpp
--rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_rint.cpp
--rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_round.cpp
--rw-r--r--   0        0        0       87 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_scalar_power_array.cpp
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_sign.cpp
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_sin.cpp
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_sinh.cpp
--rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_slash_equal.cpp
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_sqrt.cpp
--rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_square.cpp
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_tan.cpp
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_tanh.cpp
--rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Cwise_times_equal.cpp
--rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/DenseBase_LinSpaced.cpp
--rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/DenseBase_LinSpaced_seq_deprecated.cpp
--rw-r--r--   0        0        0      428 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/DenseBase_LinSpacedInt.cpp
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/DenseBase_setLinSpaced.cpp
--rw-r--r--   0        0        0      374 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/DirectionWise_hnormalized.cpp
--rw-r--r--   0        0        0      190 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/DirectionWise_replicate.cpp
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/DirectionWise_replicate_int.cpp
--rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/EigenSolver_compute.cpp
--rw-r--r--   0        0        0      816 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/EigenSolver_eigenvalues.cpp
--rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/EigenSolver_eigenvectors.cpp
--rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
--rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/FullPivHouseholderQR_solve.cpp
--rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/FullPivLU_image.cpp
--rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/FullPivLU_kernel.cpp
--rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/FullPivLU_solve.cpp
--rw-r--r--   0        0        0      463 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/GeneralizedEigenSolver.cpp
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/HessenbergDecomposition_compute.cpp
--rw-r--r--   0        0        0      399 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/HessenbergDecomposition_matrixH.cpp
--rw-r--r--   0        0        0      491 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
--rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/HouseholderQR_householderQ.cpp
--rw-r--r--   0        0        0      366 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/HouseholderQR_solve.cpp
--rw-r--r--   0        0        0     1347 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
--rw-r--r--   0        0        0      617 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/IOFormat.cpp
--rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Jacobi_makeGivens.cpp
--rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Jacobi_makeJacobi.cpp
--rw-r--r--   0        0        0      623 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/JacobiSVD_basic.cpp
--rw-r--r--   0        0        0      196 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/LeastSquaresNormalEquations.cpp
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/LeastSquaresQR.cpp
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/LLT_example.cpp
--rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/LLT_solve.cpp
--rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Map_general_stride.cpp
--rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Map_inner_stride.cpp
--rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Map_outer_stride.cpp
--rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Map_placement_new.cpp
--rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Map_simple.cpp
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_initializer_list_23_cxx11.cpp
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_initializer_list_vector_cxx11.cpp
--rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_Map_stride.cpp
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_resize_int.cpp
--rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_resize_int_int.cpp
--rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_resize_int_NoChange.cpp
--rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_resize_NoChange_int.cpp
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_setConstant_int.cpp
--rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_setConstant_int_int.cpp
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_setIdentity_int_int.cpp
--rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_setOnes_int.cpp
--rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_setOnes_int_int.cpp
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_setRandom_int.cpp
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_setRandom_int_int.cpp
--rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_setZero_int.cpp
--rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_setZero_int_int.cpp
--rw-r--r--   0        0        0      107 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Matrix_variadic_ctor_cxx11.cpp
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_adjoint.cpp
--rw-r--r--   0        0        0      530 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_all.cpp
--rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_applyOnTheLeft.cpp
--rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_applyOnTheRight.cpp
--rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_array.cpp
--rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_array_const.cpp
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_asDiagonal.cpp
--rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_block_int_int.cpp
--rw-r--r--   0        0        0      255 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_block_int_int_int_int.cpp
--rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
--rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_bottomRows_int.cpp
--rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cast.cpp
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_col.cpp
--rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_colwise.cpp
--rw-r--r--   0        0        0      483 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_colwise_iterator_cxx11.cpp
--rw-r--r--   0        0        0      423 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
--rw-r--r--   0        0        0      329 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseAbs.cpp
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseAbs2.cpp
--rw-r--r--   0        0        0       97 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseArg.cpp
--rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseEqual.cpp
--rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseInverse.cpp
--rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseMax.cpp
--rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseMin.cpp
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseNotEqual.cpp
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseProduct.cpp
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseQuotient.cpp
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseSign.cpp
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_cwiseSqrt.cpp
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_diagonal.cpp
--rw-r--r--   0        0        0      275 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_diagonal_int.cpp
--rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_diagonal_template_int.cpp
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_eigenvalues.cpp
--rw-r--r--   0        0        0      231 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_end_int.cpp
--rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_eval.cpp
--rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
--rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_hnormalized.cpp
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_homogeneous.cpp
--rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_identity.cpp
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_identity_int_int.cpp
--rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_inverse.cpp
--rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_isDiagonal.cpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_isIdentity.cpp
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_isOnes.cpp
--rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_isOrthogonal.cpp
--rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_isUnitary.cpp
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_isZero.cpp
--rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_leftCols_int.cpp
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_noalias.cpp
--rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_ones.cpp
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_ones_int.cpp
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_ones_int_int.cpp
--rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_operatorNorm.cpp
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_prod.cpp
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_random.cpp
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_random_int.cpp
--rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_random_int_int.cpp
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_replicate.cpp
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_replicate_int_int.cpp
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_reshaped_auto.cpp
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_reshaped_fixed.cpp
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_reshaped_int_int.cpp
--rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_reshaped_to_vector.cpp
--rw-r--r--   0        0        0      415 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_reverse.cpp
--rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_rightCols_int.cpp
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_row.cpp
--rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_rowwise.cpp
--rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_segment_int_int.cpp
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_select.cpp
--rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_selfadjointView.cpp
--rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_set.cpp
--rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_setIdentity.cpp
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_setOnes.cpp
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_setRandom.cpp
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_setZero.cpp
--rw-r--r--   0        0        0      231 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_start_int.cpp
--rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_bottomRows.cpp
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_end.cpp
--rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
--rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
--rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
--rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
--rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
--rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
--rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
--rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_leftCols.cpp
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_rightCols.cpp
--rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_segment.cpp
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_start.cpp
--rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_template_int_topRows.cpp
--rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
--rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_topRows_int.cpp
--rw-r--r--   0        0        0      422 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_transpose.cpp
--rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_triangularView.cpp
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_zero.cpp
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_zero_int.cpp
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/MatrixBase_zero_int_int.cpp
--rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/PartialPivLU_solve.cpp
--rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/PartialRedux_count.cpp
--rw-r--r--   0        0        0      179 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/PartialRedux_maxCoeff.cpp
--rw-r--r--   0        0        0      179 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/PartialRedux_minCoeff.cpp
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/PartialRedux_norm.cpp
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/PartialRedux_prod.cpp
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/PartialRedux_squaredNorm.cpp
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/PartialRedux_sum.cpp
--rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/RealQZ_compute.cpp
--rw-r--r--   0        0        0      349 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/RealSchur_compute.cpp
--rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
--rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
--rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
--rw-r--r--   0        0        0      197 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
--rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
--rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
--rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
--rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
--rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointView_eigenvalues.cpp
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SelfAdjointView_operatorNorm.cpp
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Slicing_arrayexpr.cpp
--rw-r--r--   0        0        0      381 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Slicing_custom_padding_cxx11.cpp
--rw-r--r--   0        0        0      171 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Slicing_rawarray_cxx11.cpp
--rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Slicing_stdvector_cxx11.cpp
--rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/SparseMatrix_coeffs.cpp
--rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/TopicAliasing_block.cpp
--rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/TopicAliasing_block_correct.cpp
--rw-r--r--   0        0        0      611 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/TopicAliasing_cwise.cpp
--rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/TopicAliasing_mult1.cpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/TopicAliasing_mult2.cpp
--rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/TopicAliasing_mult3.cpp
--rw-r--r--   0        0        0      107 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/TopicAliasing_mult4.cpp
--rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/TopicAliasing_mult5.cpp
--rw-r--r--   0        0        0      543 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/TopicStorageOrders_example.cpp
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Triangular_solve.cpp
--rw-r--r--   0        0        0      401 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tridiagonalization_compute.cpp
--rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
--rw-r--r--   0        0        0      565 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tridiagonalization_diagonal.cpp
--rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tridiagonalization_householderCoefficients.cpp
--rw-r--r--   0        0        0      402 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tridiagonalization_packedMatrix.cpp
--rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
--rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/tut_arithmetic_redux_minmax.cpp
--rw-r--r--   0        0        0      193 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
--rw-r--r--   0        0        0      289 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/tut_arithmetic_transpose_inplace.cpp
--rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/tut_matrix_assignment_resizing.cpp
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
--rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
--rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
--rw-r--r--   0        0        0      898 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_commainit_01.cpp
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_commainit_01b.cpp
--rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_commainit_02.cpp
--rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_Map_rowmajor.cpp
--rw-r--r--   0        0        0      917 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_Map_using.cpp
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_range_for_loop_1d_cxx11.cpp
--rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_range_for_loop_2d_cxx11.cpp
--rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_reshaped_vs_resize_1.cpp
--rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_reshaped_vs_resize_2.cpp
--rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
--rw-r--r--   0        0        0      622 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_SlicingCol.cpp
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_SlicingVec.cpp
--rw-r--r--   0        0        0      152 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_solve_matrix_inverse.cpp
--rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_solve_multiple_rhs.cpp
--rw-r--r--   0        0        0      381 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
--rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_solve_singular.cpp
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_solve_triangular.cpp
--rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_solve_triangular_inplace.cpp
--rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_std_sort.cpp
--rw-r--r--   0        0        0      223 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Tutorial_std_sort_rows_cxx11.cpp
--rw-r--r--   0        0        0      546 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/Vectorwise_reverse.cpp
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/snippets/VectorwiseOp_homogeneous.cpp
--rw-r--r--   0        0        0    20421 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/SparseLinearSystems.dox
--rw-r--r--   0        0        0     8586 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/SparseQuickReference.dox
--rw-r--r--   0        0        0     1020 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/special_examples/CMakeLists.txt
--rw-r--r--   0        0        0      338 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/special_examples/random_cpp11.cpp
--rw-r--r--   0        0        0     1222 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/special_examples/Tutorial_sparse_example.cpp
--rw-r--r--   0        0        0     1620 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/special_examples/Tutorial_sparse_example_details.cpp
--rw-r--r--   0        0        0     3996 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/StlContainers.dox
--rw-r--r--   0        0        0     4205 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/StorageOrders.dox
--rw-r--r--   0        0        0     7178 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/StructHavingEigenMembers.dox
--rw-r--r--   0        0        0     6290 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TemplateKeyword.dox
--rw-r--r--   0        0        0    10506 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicAliasing.dox
--rw-r--r--   0        0        0     5393 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicAssertions.dox
--rw-r--r--   0        0        0     1970 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicCMakeGuide.dox
--rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicEigenExpressionTemplates.dox
--rw-r--r--   0        0        0     6411 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicLazyEvaluation.dox
--rw-r--r--   0        0        0     9355 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicLinearAlgebraDecompositions.dox
--rw-r--r--   0        0        0     3816 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicMultithreading.dox
--rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicResizing.dox
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicScalarTypes.dox
--rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TopicVectorization.dox
--rw-r--r--   0        0        0     2606 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/tutorial.cpp
--rw-r--r--   0        0        0     7062 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialAdvancedInitialization.dox
--rw-r--r--   0        0        0     8715 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialArrayClass.dox
--rw-r--r--   0        0        0     8530 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialBlockOperations.dox
--rw-r--r--   0        0        0     9973 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialGeometry.dox
--rw-r--r--   0        0        0    12159 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialLinearAlgebra.dox
--rw-r--r--   0        0        0     4074 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialMapClass.dox
--rw-r--r--   0        0        0    10176 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialMatrixArithmetic.dox
--rw-r--r--   0        0        0    14244 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialMatrixClass.dox
--rw-r--r--   0        0        0    12272 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialReductionsVisitorsBroadcasting.dox
--rw-r--r--   0        0        0     3069 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialReshape.dox
--rw-r--r--   0        0        0     8525 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialSlicingIndexing.dox
--rw-r--r--   0        0        0    20886 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialSparse.dox
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialSparse_example_details.dox
--rw-r--r--   0        0        0     2208 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/TutorialSTL.dox
--rw-r--r--   0        0        0     8870 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/UnalignedArrayAssert.dox
--rw-r--r--   0        0        0     6979 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/UsingBlasLapackBackends.dox
--rw-r--r--   0        0        0     6226 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/UsingIntelMKL.dox
--rw-r--r--   0        0        0     1885 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/UsingNVCC.dox
--rw-r--r--   0        0        0     2980 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/doc/WrongStackAlignment.dox
--rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/AccelerateSupport
--rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/Cholesky
--rw-r--r--   0        0        0     1948 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/CholmodSupport
--rw-r--r--   0        0        0    13755 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/Core
--rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/Dense
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/Eigen
--rw-r--r--   0        0        0     1837 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/Eigenvalues
--rw-r--r--   0        0        0     1999 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/Geometry
--rw-r--r--   0        0        0      858 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/Householder
--rw-r--r--   0        0        0     2150 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/IterativeLinearSolvers
--rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/Jacobi
--rw-r--r--   0        0        0     1430 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/KLUSupport
--rw-r--r--   0        0        0     1260 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/LU
--rw-r--r--   0        0        0     1026 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/MetisSupport
--rw-r--r--   0        0        0     2521 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/OrderingMethods
--rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/PardisoSupport
--rw-r--r--   0        0        0     1800 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/PaStiXSupport
--rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/QR
--rw-r--r--   0        0        0      939 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/QtAlignedMalloc
--rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/Sparse
--rw-r--r--   0        0        0     1272 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/SparseCholesky
--rw-r--r--   0        0        0     2281 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/SparseCore
--rw-r--r--   0        0        0     1814 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/SparseLU
--rw-r--r--   0        0        0     1231 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/SparseQR
--rw-r--r--   0        0        0     1175 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/SPQRSupport
--rw-r--r--   0        0        0    15556 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/AccelerateSupport/AccelerateSupport.h
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/AccelerateSupport/InternalHeaderCheck.h
--rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Cholesky/InternalHeaderCheck.h
--rw-r--r--   0        0        0    25585 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0        0        0    19268 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0        0        0     5249 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
--rw-r--r--   0        0        0    26160 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/CholmodSupport/InternalHeaderCheck.h
--rw-r--r--   0        0        0    21012 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0        0        0     3682 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0        0        0   132371 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0        0        0     7005 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0        0        0    28847 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rw-r--r--   0        0        0    14743 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h
--rw-r--r--   0        0        0    93878 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h
--rw-r--r--   0        0        0   122156 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
--rw-r--r--   0        0        0    15345 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0        0        0     6631 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0        0        0    85764 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0        0        0     2721 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
--rw-r--r--   0        0        0    16179 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0        0        0    48993 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h
--rw-r--r--   0        0        0     9743 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0        0        0   113404 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0        0        0    26977 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h
--rw-r--r--   0        0        0    58036 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h
--rw-r--r--   0        0        0    57343 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX512/TrsmUnrolls.inc
--rw-r--r--   0        0        0     6286 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
--rw-r--r--   0        0        0    35460 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0        0        0     5410 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0        0        0    95692 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0        0        0     4714 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0        0        0    40357 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0        0        0     1795 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0        0        0     3650 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
--rw-r--r--   0        0        0    18252 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/GPU/Complex.h
--rw-r--r--   0        0        0     2840 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0        0        0    59998 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0        0        0     9996 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/GPU/Tuple.h
--rw-r--r--   0        0        0     2378 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
--rw-r--r--   0        0        0      714 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
--rw-r--r--   0        0        0    18095 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0        0        0    16442 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0        0        0    34884 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
--rw-r--r--   0        0        0    22579 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0        0        0    10162 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0        0        0     4674 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0        0        0   197647 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0        0        0    52747 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
--rw-r--r--   0        0        0     1949 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h
--rw-r--r--   0        0        0    13882 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0        0        0     5042 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-r--r--   0        0        0    74525 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0        0        0     4090 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
--rw-r--r--   0        0        0     1215 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0        0        0    21938 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0        0        0     1442 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
--rw-r--r--   0        0        0     7702 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0        0        0    12882 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0        0        0    16636 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0        0        0    22694 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0        0        0     2756 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
--rw-r--r--   0        0        0    16801 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0        0        0     8162 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-r--r--   0        0        0    37978 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
--rw-r--r--   0        0        0    11048 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0        0        0    16805 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Array.h
--rw-r--r--   0        0        0     8480 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0        0        0     7089 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0        0        0     2866 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Assign.h
--rw-r--r--   0        0        0    12688 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0        0        0    42923 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/AssignEvaluator.h
--rw-r--r--   0        0        0    14427 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0        0        0    19711 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Block.h
--rw-r--r--   0        0        0     4990 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0        0        0     6258 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0        0        0     7247 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0        0        0    65587 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0        0        0     4915 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0        0        0     7941 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0        0        0    38789 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0        0        0     8233 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0        0        0     4031 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0        0        0     6417 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0        0        0    31995 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/DenseBase.h
--rw-r--r--   0        0        0    25123 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0        0        0    29625 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0        0        0     9862 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Diagonal.h
--rw-r--r--   0        0        0    18269 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0        0        0    11728 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Dot.h
--rw-r--r--   0        0        0     6039 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/EigenBase.h
--rw-r--r--   0        0        0     5038 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0        0        0     6627 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0        0        0    24044 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0        0        0     9757 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0        0        0     4820 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0        0        0      671 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0        0        0    43491 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/functors/UnaryFunctors.h
--rw-r--r--   0        0        0     5952 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0        0        0    22092 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0        0        0    49425 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0        0        0    12273 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/IndexedView.h
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/InternalHeaderCheck.h
--rw-r--r--   0        0        0     3629 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Inverse.h
--rw-r--r--   0        0        0     8479 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/IO.h
--rw-r--r--   0        0        0     7297 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Map.h
--rw-r--r--   0        0        0    11521 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/MapBase.h
--rw-r--r--   0        0        0    63370 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0        0        0    13680 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0        0        0    24976 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Matrix.h
--rw-r--r--   0        0        0    24291 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0        0        0     3196 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/NestByValue.h
--rw-r--r--   0        0        0     3767 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/NoAlias.h
--rw-r--r--   0        0        0    13231 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/NumTraits.h
--rw-r--r--   0        0        0     9520 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0        0        0    21378 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0        0        0    49640 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0        0        0     7507 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Product.h
--rw-r--r--   0        0        0    56336 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0        0        0   144201 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0        0        0    20346 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0        0        0     5269 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0        0        0    16138 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0        0        0     7120 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0        0        0    22265 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0        0        0     6543 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0        0        0     5425 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0        0        0    21889 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0        0        0    11904 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0        0        0    10157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0        0        0     5366 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0        0        0     6266 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0        0        0     4172 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0        0        0    21454 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0        0        0    14223 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0        0        0    15005 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0        0        0    10865 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0        0        0    19539 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0        0        0     6913 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0        0        0     5928 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/products/TriangularSolverVector.h
--rw-r--r--   0        0        0     7967 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Random.h
--rw-r--r--   0        0        0    19732 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Redux.h
--rw-r--r--   0        0        0    18152 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Ref.h
--rw-r--r--   0        0        0     5779 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Replicate.h
--rw-r--r--   0        0        0    17438 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Reshaped.h
--rw-r--r--   0        0        0     4438 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0        0        0     7771 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Reverse.h
--rw-r--r--   0        0        0     6348 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Select.h
--rw-r--r--   0        0        0    15273 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0        0        0     1782 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0        0        0    16363 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h
--rw-r--r--   0        0        0     7092 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Solve.h
--rw-r--r--   0        0        0     6136 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/SolverBase.h
--rw-r--r--   0        0        0     9569 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0        0        0     8942 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/StableNorm.h
--rw-r--r--   0        0        0    21710 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/StlIterators.h
--rw-r--r--   0        0        0     4572 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Stride.h
--rw-r--r--   0        0        0     2871 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Swap.h
--rw-r--r--   0        0        0    18135 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Transpose.h
--rw-r--r--   0        0        0    13991 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Transpositions.h
--rw-r--r--   0        0        0    39146 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0        0        0     6377 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/Assert.h
--rw-r--r--   0        0        0    26921 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0        0        0    19869 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0        0        0    22782 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/Constants.h
--rw-r--r--   0        0        0     6362 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0        0        0    15655 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0        0        0     6468 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0        0        0     9819 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/IntegralConstant.h
--rw-r--r--   0        0        0    49336 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/Macros.h
--rw-r--r--   0        0        0    50828 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/Memory.h
--rw-r--r--   0        0        0    20758 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/Meta.h
--rw-r--r--   0        0        0     4444 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0        0        0     1426 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0        0        0     1515 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0        0        0     8030 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/Serializer.h
--rw-r--r--   0        0        0     5611 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0        0        0    10116 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0        0        0    36138 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/util/XprHelper.h
--rw-r--r--   0        0        0     3556 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0        0        0    35956 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0        0        0    16972 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Core/Visitor.h
--rw-r--r--   0        0        0    12837 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0        0        0    17784 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0        0        0     4307 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0        0        0    23630 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0        0        0    17691 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0        0        0     9980 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0        0        0    14748 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/InternalHeaderCheck.h
--rw-r--r--   0        0        0     5771 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0        0        0    24417 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0        0        0    21715 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0        0        0     3765 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0        0        0    36080 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0        0        0     4229 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0        0        0    23216 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
--rw-r--r--   0        0        0    19463 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0        0        0     8688 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0        0        0     6152 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
--rw-r--r--   0        0        0     3776 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0        0        0    21155 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0        0        0    12281 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/InternalHeaderCheck.h
--rw-r--r--   0        0        0    11585 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0        0        0    10079 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0        0        0    35142 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0        0        0     7099 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0        0        0     8307 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0        0        0     7285 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0        0        0    63864 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/Transform.h
--rw-r--r--   0        0        0     7886 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/Translation.h
--rw-r--r--   0        0        0     6400 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Geometry/Umeyama.h
--rw-r--r--   0        0        0     4933 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0        0        0     5612 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Householder/Householder.h
--rw-r--r--   0        0        0    24225 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Householder/HouseholderSequence.h
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Householder/InternalHeaderCheck.h
--rw-r--r--   0        0        0     7035 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0        0        0     7100 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0        0        0     9088 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0        0        0    15587 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0        0        0    15431 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/IterativeLinearSolvers/InternalHeaderCheck.h
--rw-r--r--   0        0        0    13861 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0        0        0     7600 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0        0        0     4364 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
--rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Jacobi/InternalHeaderCheck.h
--rw-r--r--   0        0        0    17096 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/Jacobi/Jacobi.h
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/KLUSupport/InternalHeaderCheck.h
--rw-r--r--   0        0        0    11971 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/KLUSupport/KLUSupport.h
--rw-r--r--   0        0        0    14185 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/LU/arch/InverseSize4.h
--rw-r--r--   0        0        0     3707 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/LU/Determinant.h
--rw-r--r--   0        0        0    33213 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/LU/InternalHeaderCheck.h
--rw-r--r--   0        0        0    16148 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0        0        0    22687 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0        0        0     4260 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
--rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/MetisSupport/InternalHeaderCheck.h
--rw-r--r--   0        0        0     4763 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/MetisSupport/MetisSupport.h
--rw-r--r--   0        0        0    31000 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/misc/blas.h
--rw-r--r--   0        0        0     3033 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/misc/Image.h
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/misc/InternalHeaderCheck.h
--rw-r--r--   0        0        0     2859 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/misc/Kernel.h
--rw-r--r--   0        0        0     7986 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/misc/lapack.h
--rw-r--r--   0        0        0  1074696 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/misc/lapacke.h
--rw-r--r--   0        0        0     6726 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/misc/lapacke_helpers.h
--rw-r--r--   0        0        0      491 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/misc/lapacke_mangling.h
--rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0        0        0    16578 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0        0        0    63544 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0        0        0      159 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/OrderingMethods/InternalHeaderCheck.h
--rw-r--r--   0        0        0     5439 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/OrderingMethods/Ordering.h
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/PardisoSupport/InternalHeaderCheck.h
--rw-r--r--   0        0        0    20671 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
--rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/PaStiXSupport/InternalHeaderCheck.h
--rw-r--r--   0        0        0    22964 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
--rw-r--r--   0        0        0    14906 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0        0        0    23373 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0        0        0    60390 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0        0        0     4942 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0        0        0     6104 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0        0        0    12277 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/InternalHeaderCheck.h
--rw-r--r--   0        0        0     6817 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0        0        0     3993 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0        0        0     7040 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/plugins/ReshapedMethods.h
--rw-r--r--   0        0        0    27434 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0        0        0     8229 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0        0        0    25568 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0        0        0    29631 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0        0        0    19159 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0        0        0     3089 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/QR/InternalHeaderCheck.h
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCholesky/InternalHeaderCheck.h
--rw-r--r--   0        0        0    24951 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0        0        0     6042 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
--rw-r--r--   0        0        0    11086 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0        0        0     7813 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0        0        0    12941 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/InternalHeaderCheck.h
--rw-r--r--   0        0        0    11677 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0        0        0    24702 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0        0        0     6729 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0        0        0    22893 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0        0        0    26234 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0        0        0     4945 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0        0        0    13763 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0        0        0     5984 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0        0        0     3216 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0        0        0     1156 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0        0        0    12921 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0        0        0    70795 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0        0        0    17680 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0        0        0    11660 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0        0        0     7715 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0        0        0     1786 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0        0        0    15865 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0        0        0    26133 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0        0        0     4689 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0        0        0     8902 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0        0        0     3305 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0        0        0     6633 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0        0        0     6858 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0        0        0    18550 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0        0        0     8380 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0        0        0    10007 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseCore/TriangularSolver.h
--rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/InternalHeaderCheck.h
--rw-r--r--   0        0        0    35833 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0        0        0     6931 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0        0        0     6801 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0        0        0     3826 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0        0        0     5752 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0        0        0     7866 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0        0        0     8603 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0        0        0     9324 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0        0        0     4719 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0        0        0     3010 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
--rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0        0        0    13120 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0        0        0     2167 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0        0        0     4407 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseQR/InternalHeaderCheck.h
--rw-r--r--   0        0        0    29944 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SparseQR/SparseQR.h
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SPQRSupport/InternalHeaderCheck.h
--rw-r--r--   0        0        0    12259 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
--rw-r--r--   0        0        0     2841 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/StlSupport/details.h
--rw-r--r--   0        0        0     2014 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SuperLUSupport/InternalHeaderCheck.h
--rw-r--r--   0        0        0    35387 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
--rw-r--r--   0        0        0    63680 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0        0        0     7062 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SVD/BDCSVD_LAPACKE.h
--rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SVD/InternalHeaderCheck.h
--rw-r--r--   0        0        0    36043 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0        0        0     6106 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0        0        0    19651 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0        0        0    16598 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/SVD/UpperBidiagonalization.h
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/UmfPackSupport/InternalHeaderCheck.h
--rw-r--r--   0        0        0    25140 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
--rw-r--r--   0        0        0      824 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/StdDeque
--rw-r--r--   0        0        0      752 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/StdList
--rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/StdVector
--rw-r--r--   0        0        0     2307 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/SuperLUSupport
--rw-r--r--   0        0        0     1669 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/SVD
--rw-r--r--   0        0        0     1422 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/Eigen/UmfPackSupport
--rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/eigen3.pc.in
--rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/bdcsvd_int.cpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
--rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/block_on_const_type_actually_const_0.cpp
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/block_on_const_type_actually_const_1.cpp
--rw-r--r--   0        0        0     2454 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/CMakeLists.txt
--rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/colpivqr_int.cpp
--rw-r--r--   0        0        0      260 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/const_qualified_block_method_retval_0.cpp
--rw-r--r--   0        0        0      255 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/const_qualified_block_method_retval_1.cpp
--rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/const_qualified_diagonal_method_retval.cpp
--rw-r--r--   0        0        0      256 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/const_qualified_transpose_method_retval.cpp
--rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/cwiseunaryview_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0      243 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/diagonal_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/eigensolver_cplx.cpp
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/eigensolver_int.cpp
--rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/failtest_sanity_check.cpp
--rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/fullpivlu_int.cpp
--rw-r--r--   0        0        0      272 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/fullpivqr_int.cpp
--rw-r--r--   0        0        0      197 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/initializer_list_1.cpp
--rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/initializer_list_2.cpp
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/jacobisvd_int.cpp
--rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/ldlt_int.cpp
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/llt_int.cpp
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
--rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
--rw-r--r--   0        0        0      285 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
--rw-r--r--   0        0        0      329 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
--rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
--rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/map_on_const_type_actually_const_0.cpp
--rw-r--r--   0        0        0      256 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/map_on_const_type_actually_const_1.cpp
--rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/partialpivlu_int.cpp
--rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/qr_int.cpp
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/ref_1.cpp
--rw-r--r--   0        0        0      228 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/ref_2.cpp
--rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/ref_3.cpp
--rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/ref_4.cpp
--rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/ref_5.cpp
--rw-r--r--   0        0        0      256 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/selfadjointview_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/sparse_ref_1.cpp
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/sparse_ref_2.cpp
--rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/sparse_ref_3.cpp
--rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/sparse_ref_4.cpp
--rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/sparse_ref_5.cpp
--rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/sparse_storage_mismatch.cpp
--rw-r--r--   0        0        0      231 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/swap_1.cpp
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/swap_2.cpp
--rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/ternary_1.cpp
--rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/ternary_2.cpp
--rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/transpose_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/failtest/triangularview_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0     1180 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/INSTALL
--rw-r--r--   0        0        0     2277 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/cholesky.inc
--rw-r--r--   0        0        0     2947 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/clacgv.f
--rw-r--r--   0        0        0     2437 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/cladiv.f
--rw-r--r--   0        0        0     6527 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/clarf.f
--rw-r--r--   0        0        0    24195 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/clarfb.f
--rw-r--r--   0        0        0     5547 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/clarfg.f
--rw-r--r--   0        0        0    10778 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/clarft.f
--rw-r--r--   0        0        0    11940 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/CMakeLists.txt
--rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/complex_double.cpp
--rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/complex_single.cpp
--rw-r--r--   0        0        0     3097 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/dladiv.f
--rw-r--r--   0        0        0     5448 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/dlamch.f
--rw-r--r--   0        0        0     2618 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/dlapy2.f
--rw-r--r--   0        0        0     2848 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/dlapy3.f
--rw-r--r--   0        0        0     6394 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/dlarf.f
--rw-r--r--   0        0        0    23511 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/dlarfb.f
--rw-r--r--   0        0        0     5142 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/dlarfg.f
--rw-r--r--   0        0        0    10548 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/dlarft.f
--rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/double.cpp
--rw-r--r--   0        0        0     1334 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/dsecnd_NONE.f
--rw-r--r--   0        0        0     1888 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/eigenvalues.inc
--rw-r--r--   0        0        0     3075 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/ilaclc.f
--rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/ilaclr.f
--rw-r--r--   0        0        0     3070 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/iladlc.f
--rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/iladlr.f
--rw-r--r--   0        0        0     3059 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/ilaslc.f
--rw-r--r--   0        0        0     3109 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/ilaslr.f
--rw-r--r--   0        0        0     3080 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/ilazlc.f
--rw-r--r--   0        0        0     3131 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/ilazlr.f
--rw-r--r--   0        0        0      906 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/lapack_common.h
--rw-r--r--   0        0        0     2744 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/lu.inc
--rw-r--r--   0        0        0     1310 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/second_NONE.f
--rw-r--r--   0        0        0      579 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/single.cpp
--rw-r--r--   0        0        0     3025 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/sladiv.f
--rw-r--r--   0        0        0     5453 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/slamch.f
--rw-r--r--   0        0        0     2594 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/slapy2.f
--rw-r--r--   0        0        0     2812 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/slapy3.f
--rw-r--r--   0        0        0     6344 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/slarf.f
--rw-r--r--   0        0        0    23490 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/slarfb.f
--rw-r--r--   0        0        0     5104 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/slarfg.f
--rw-r--r--   0        0        0    10509 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/slarft.f
--rw-r--r--   0        0        0     5027 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/svd.inc
--rw-r--r--   0        0        0     2955 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/zlacgv.f
--rw-r--r--   0        0        0     2461 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/zladiv.f
--rw-r--r--   0        0        0     6510 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/zlarf.f
--rw-r--r--   0        0        0    24272 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/zlarfb.f
--rw-r--r--   0        0        0     5562 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/zlarfg.f
--rw-r--r--   0        0        0    10780 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/lapack/zlarft.f
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/README.md
--rw-r--r--   0        0        0      599 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/buildtests.in
--rw-r--r--   0        0        0     1618 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/cdashtesting.cmake.in
--rw-r--r--   0        0        0      691 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/check.in
--rw-r--r--   0        0        0      334 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/CMakeLists.txt
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/debug.in
--rw-r--r--   0        0        0     6616 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/eigen_gen_credits.cpp
--rw-r--r--   0        0        0      762 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/eigen_gen_docs
--rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/eigen_gen_split_test_help.cmake
--rw-r--r--   0        0        0     1034 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/eigen_monitor_perf.sh
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/release.in
--rw-r--r--   0        0        0     2437 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/scripts/relicense.py
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/signature_of_eigen3_matrix_library
--rw-r--r--   0        0        0     4684 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/accelerate_support.cpp
--rw-r--r--   0        0        0     9655 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/adjoint.cpp
--rw-r--r--   0        0        0     5979 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/AnnoyingScalar.h
--rw-r--r--   0        0        0    40907 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/array_cwise.cpp
--rw-r--r--   0        0        0    15498 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/array_for_matrix.cpp
--rw-r--r--   0        0        0      993 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/array_of_string.cpp
--rw-r--r--   0        0        0     2423 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/array_replicate.cpp
--rw-r--r--   0        0        0     6587 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/array_reverse.cpp
--rw-r--r--   0        0        0     2503 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/bandmatrix.cpp
--rw-r--r--   0        0        0    13942 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/basicstuff.cpp
--rw-r--r--   0        0        0     8267 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/bdcsvd.cpp
--rw-r--r--   0        0        0    18260 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/bfloat16_float.cpp
--rw-r--r--   0        0        0     1507 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/bicgstab.cpp
--rw-r--r--   0        0        0     6544 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/blasutil.cpp
--rw-r--r--   0        0        0    15545 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/block.cpp
--rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/boostmultiprec.cpp
--rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/bug1213.cpp
--rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/bug1213.h
--rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/bug1213_main.cpp
--rw-r--r--   0        0        0    18872 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/cholesky.cpp
--rw-r--r--   0        0        0     3446 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/cholmod_support.cpp
--rw-r--r--   0        0        0    16634 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/CMakeLists.txt
--rw-r--r--   0        0        0     3268 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/commainitializer.cpp
--rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/conjugate_gradient.cpp
--rw-r--r--   0        0        0     5536 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/conservative_resize.cpp
--rw-r--r--   0        0        0     2389 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/constexpr.cpp
--rw-r--r--   0        0        0     2660 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/constructor.cpp
--rw-r--r--   0        0        0     6565 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/corners.cpp
--rw-r--r--   0        0        0     2097 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/ctorleak.cpp
--rw-r--r--   0        0        0     7394 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/dense_storage.cpp
--rw-r--r--   0        0        0     5252 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/denseLM.cpp
--rw-r--r--   0        0        0     2341 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/determinant.cpp
--rw-r--r--   0        0        0     4220 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/diagonal.cpp
--rw-r--r--   0        0        0     5867 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/diagonal_matrix_variadic_ctor.cpp
--rw-r--r--   0        0        0     8994 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/diagonalmatrices.cpp
--rw-r--r--   0        0        0     2291 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/dontalign.cpp
--rw-r--r--   0        0        0     5116 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/dynalloc.cpp
--rw-r--r--   0        0        0     2261 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/eigen2support.cpp
--rw-r--r--   0        0        0     6397 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/eigensolver_complex.cpp
--rw-r--r--   0        0        0     5550 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/eigensolver_generalized_real.cpp
--rw-r--r--   0        0        0     9706 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/eigensolver_generic.cpp
--rw-r--r--   0        0        0    11700 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/eigensolver_selfadjoint.cpp
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/evaluator_common.h
--rw-r--r--   0        0        0    21682 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/evaluators.cpp
--rw-r--r--   0        0        0     1965 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/exceptions.cpp
--rw-r--r--   0        0        0     5355 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/fastmath.cpp
--rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/first_aligned.cpp
--rw-r--r--   0        0        0    18613 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/geo_alignedbox.cpp
--rw-r--r--   0        0        0     3701 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/geo_eulerangles.cpp
--rw-r--r--   0        0        0     5595 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/geo_homogeneous.cpp
--rw-r--r--   0        0        0     7496 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/geo_hyperplane.cpp
--rw-r--r--   0        0        0     6304 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/geo_orthomethods.cpp
--rw-r--r--   0        0        0     5099 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/geo_parametrizedline.cpp
--rw-r--r--   0        0        0    11837 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/geo_quaternion.cpp
--rw-r--r--   0        0        0    27097 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/geo_transformations.cpp
--rw-r--r--   0        0        0    16624 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/gpu_basic.cu
--rw-r--r--   0        0        0     5531 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/gpu_common.h
--rw-r--r--   0        0        0     4857 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/gpu_example.cu
--rw-r--r--   0        0        0    18324 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/gpu_test_helper.h
--rw-r--r--   0        0        0    15059 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/half_float.cpp
--rw-r--r--   0        0        0     2466 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/hessenberg.cpp
--rw-r--r--   0        0        0    10266 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/householder.cpp
--rw-r--r--   0        0        0     2645 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/incomplete_cholesky.cpp
--rw-r--r--   0        0        0    19109 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/indexed_view.cpp
--rw-r--r--   0        0        0    13212 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/initializer_list_construction.cpp
--rw-r--r--   0        0        0     3990 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/inplace_decomposition.cpp
--rw-r--r--   0        0        0     5903 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/integer_types.cpp
--rw-r--r--   0        0        0     4815 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/inverse.cpp
--rw-r--r--   0        0        0     1904 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/io.cpp
--rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/is_same_dense.cpp
--rw-r--r--   0        0        0     3152 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/jacobi.cpp
--rw-r--r--   0        0        0     9530 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/jacobisvd.cpp
--rw-r--r--   0        0        0      987 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/klu_support.cpp
--rw-r--r--   0        0        0     6277 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/linearstructure.cpp
--rw-r--r--   0        0        0     1536 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/lscg.cpp
--rw-r--r--   0        0        0     9327 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/lu.cpp
--rw-r--r--   0        0        0    33661 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/main.h
--rw-r--r--   0        0        0     8342 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/mapped_matrix.cpp
--rw-r--r--   0        0        0     7648 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/mapstaticmethods.cpp
--rw-r--r--   0        0        0    11835 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/mapstride.cpp
--rw-r--r--   0        0        0     5854 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/meta.cpp
--rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/metis_support.cpp
--rw-r--r--   0        0        0     1835 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/miscmatrices.cpp
--rw-r--r--   0        0        0    17072 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/mixingtypes.cpp
--rw-r--r--   0        0        0     1114 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/MovableScalar.h
--rw-r--r--   0        0        0      659 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/mpl2only.cpp
--rw-r--r--   0        0        0     1421 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/nestbyvalue.cpp
--rw-r--r--   0        0        0     4458 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/nesting_ops.cpp
--rw-r--r--   0        0        0     8928 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/nomalloc.cpp
--rw-r--r--   0        0        0    13244 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/nullary.cpp
--rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/num_dimensions.cpp
--rw-r--r--   0        0        0    11929 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/numext.cpp
--rw-r--r--   0        0        0      606 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/OffByOneScalar.h
--rw-r--r--   0        0        0    64959 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/packetmath.cpp
--rw-r--r--   0        0        0     9644 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/packetmath_test_shared.h
--rw-r--r--   0        0        0      984 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/pardiso_support.cpp
--rw-r--r--   0        0        0     1956 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/pastix_support.cpp
--rw-r--r--   0        0        0     7212 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/permutationmatrices.cpp
--rw-r--r--   0        0        0     3054 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/prec_inverse_4x4.cpp
--rw-r--r--   0        0        0    13740 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product.h
--rw-r--r--   0        0        0    16101 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_extra.cpp
--rw-r--r--   0        0        0     5694 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_large.cpp
--rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_mmtr.cpp
--rw-r--r--   0        0        0    11197 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_notemporary.cpp
--rw-r--r--   0        0        0     3596 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_selfadjoint.cpp
--rw-r--r--   0        0        0    13838 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_small.cpp
--rw-r--r--   0        0        0     6258 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_symm.cpp
--rw-r--r--   0        0        0     8073 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_syrk.cpp
--rw-r--r--   0        0        0     7058 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_trmm.cpp
--rw-r--r--   0        0        0     4340 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_trmv.cpp
--rw-r--r--   0        0        0     6229 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/product_trsolve.cpp
--rw-r--r--   0        0        0     4965 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/qr.cpp
--rw-r--r--   0        0        0    14167 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/qr_colpivoting.cpp
--rw-r--r--   0        0        0     5768 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/qr_fullpivoting.cpp
--rw-r--r--   0        0        0     4777 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/qtvector.cpp
--rw-r--r--   0        0        0     4596 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/rand.cpp
--rw-r--r--   0        0        0     5261 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/random_matrix.cpp
--rw-r--r--   0        0        0     9549 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/random_matrix_helper.h
--rw-r--r--   0        0        0     6988 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/random_without_cast_overflow.h
--rw-r--r--   0        0        0     3224 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/real_qz.cpp
--rw-r--r--   0        0        0     8422 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/redux.cpp
--rw-r--r--   0        0        0    13894 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/ref.cpp
--rw-r--r--   0        0        0    11561 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/reshape.cpp
--rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/resize.cpp
--rw-r--r--   0        0        0     5492 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/rvalue_types.cpp
--rw-r--r--   0        0        0      635 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/SafeScalar.h
--rw-r--r--   0        0        0     3738 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/schur_complex.cpp
--rw-r--r--   0        0        0     4120 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/schur_real.cpp
--rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/selfadjoint.cpp
--rw-r--r--   0        0        0     7631 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/serializer.cpp
--rw-r--r--   0        0        0     2614 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/simplicial_cholesky.cpp
--rw-r--r--   0        0        0     2085 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sizeof.cpp
--rw-r--r--   0        0        0     2703 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sizeoverflow.cpp
--rw-r--r--   0        0        0     7388 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/skew_symmetric_matrix3.cpp
--rw-r--r--   0        0        0     1518 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/smallvectors.cpp
--rw-r--r--   0        0        0     1935 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/solverbase.h
--rw-r--r--   0        0        0     5001 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparse.h
--rw-r--r--   0        0        0    34378 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparse_basic.cpp
--rw-r--r--   0        0        0    13054 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparse_block.cpp
--rw-r--r--   0        0        0    11458 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparse_permutations.cpp
--rw-r--r--   0        0        0    27742 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparse_product.cpp
--rw-r--r--   0        0        0     6245 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparse_ref.cpp
--rw-r--r--   0        0        0    25548 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparse_solver.h
--rw-r--r--   0        0        0     5267 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparse_solvers.cpp
--rw-r--r--   0        0        0     7143 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparse_vector.cpp
--rw-r--r--   0        0        0     4916 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparseLM.cpp
--rw-r--r--   0        0        0     1794 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparselu.cpp
--rw-r--r--   0        0        0     4736 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/sparseqr.cpp
--rw-r--r--   0        0        0     1820 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/special_numbers.cpp
--rw-r--r--   0        0        0   165510 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/split_test_helper.h
--rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/spqr_support.cpp
--rw-r--r--   0        0        0    10624 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/stable_norm.cpp
--rw-r--r--   0        0        0     4390 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/stddeque.cpp
--rw-r--r--   0        0        0     4896 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/stddeque_overload.cpp
--rw-r--r--   0        0        0     4362 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/stdlist.cpp
--rw-r--r--   0        0        0     6044 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/stdlist_overload.cpp
--rw-r--r--   0        0        0     5274 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/stdvector.cpp
--rw-r--r--   0        0        0     5175 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/stdvector_overload.cpp
--rw-r--r--   0        0        0    19180 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/stl_iterators.cpp
--rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/superlu_support.cpp
--rw-r--r--   0        0        0    25334 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/svd_common.h
--rw-r--r--   0        0        0     4228 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/svd_fill.h
--rw-r--r--   0        0        0     3385 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/swap.cpp
--rw-r--r--   0        0        0     2630 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/symbolic_index.cpp
--rw-r--r--   0        0        0    12123 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/triangular.cpp
--rw-r--r--   0        0        0     5103 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/tuple_test.cpp
--rw-r--r--   0        0        0     1971 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/type_alias.cpp
--rw-r--r--   0        0        0     6042 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/umeyama.cpp
--rw-r--r--   0        0        0     1205 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/umfpack_support.cpp
--rw-r--r--   0        0        0     2625 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/unalignedcount.cpp
--rw-r--r--   0        0        0     1455 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/unaryviewstride.cpp
--rw-r--r--   0        0        0     1759 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/upperbidiagonalization.cpp
--rw-r--r--   0        0        0    20639 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/vectorization_logic.cpp
--rw-r--r--   0        0        0     9841 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/vectorwiseop.cpp
--rw-r--r--   0        0        0    11299 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/visitor.cpp
--rw-r--r--   0        0        0     3837 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/test/zerosized.cpp
--rw-r--r--   0        0        0     4029 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/bench/bench_svd.cpp
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/CMakeLists.txt
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/CMakeLists.txt
--rw-r--r--   0        0        0     5460 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/eigendoxy_layout.xml.in
--rw-r--r--   0        0        0     2158 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/BVH_Example.cpp
--rw-r--r--   0        0        0      760 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/CMakeLists.txt
--rw-r--r--   0        0        0     1893 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/EulerAngles.cpp
--rw-r--r--   0        0        0     2640 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/FFT.cpp
--rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/MatrixExponential.cpp
--rw-r--r--   0        0        0      492 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/MatrixFunction.cpp
--rw-r--r--   0        0        0      390 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/MatrixLogarithm.cpp
--rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/MatrixPower.cpp
--rw-r--r--   0        0        0      441 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/MatrixPower_optimal.cpp
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/MatrixSine.cpp
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/MatrixSinh.cpp
--rw-r--r--   0        0        0      450 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/MatrixSquareRoot.cpp
--rw-r--r--   0        0        0     2445 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/PolynomialSolver1.cpp
--rw-r--r--   0        0        0      655 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/PolynomialUtils1.cpp
--rw-r--r--   0        0        0     1105 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/SYCL/CMakeLists.txt
--rw-r--r--   0        0        0     2614 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/examples/SYCL/CwiseMul.cpp
--rw-r--r--   0        0        0      909 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/Overview.dox
--rw-r--r--   0        0        0     1163 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/snippets/CMakeLists.txt
--rw-r--r--   0        0        0      354 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/doc/SYCL.dox
--rw-r--r--   0        0        0     4608 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/AdolcForward
--rw-r--r--   0        0        0     6609 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/AlignedVector3
--rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/ArpackSupport
--rw-r--r--   0        0        0     1264 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/AutoDiff
--rw-r--r--   0        0        0     5618 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/BVH
--rw-r--r--   0        0        0      643 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CMakeLists.txt
--rw-r--r--   0        0        0      315 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/CMakeLists.txt
--rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/InternalHeaderCheck.h
--rw-r--r--   0        0        0    66408 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/README.md
--rw-r--r--   0        0        0    18852 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
--rw-r--r--   0        0        0    12774 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
--rw-r--r--   0        0        0    10567 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
--rw-r--r--   0        0        0    59936 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
--rw-r--r--   0        0        0    62499 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
--rw-r--r--   0        0        0    43060 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
--rw-r--r--   0        0        0    19986 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
--rw-r--r--   0        0        0    16067 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
--rw-r--r--   0        0        0    46087 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
--rw-r--r--   0        0        0     2786 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
--rw-r--r--   0        0        0      231 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
--rw-r--r--   0        0        0    64733 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
--rw-r--r--   0        0        0    24623 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
--rw-r--r--   0        0        0    90282 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
--rw-r--r--   0        0        0    72343 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
--rw-r--r--   0        0        0    19263 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
--rw-r--r--   0        0        0    49963 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
--rw-r--r--   0        0        0    28213 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
--rw-r--r--   0        0        0     8894 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
--rw-r--r--   0        0        0    13468 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
--rw-r--r--   0        0        0     5071 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
--rw-r--r--   0        0        0     4052 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
--rw-r--r--   0        0        0    15104 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
--rw-r--r--   0        0        0    44386 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
--rw-r--r--   0        0        0    15932 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
--rw-r--r--   0        0        0     4723 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
--rw-r--r--   0        0        0    16763 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
--rw-r--r--   0        0        0     8813 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
--rw-r--r--   0        0        0    41570 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
--rw-r--r--   0        0        0    29629 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
--rw-r--r--   0        0        0    16410 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
--rw-r--r--   0        0        0    25020 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
--rw-r--r--   0        0        0    10734 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
--rw-r--r--   0        0        0     8963 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
--rw-r--r--   0        0        0     8552 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
--rw-r--r--   0        0        0    15709 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
--rw-r--r--   0        0        0    11166 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
--rw-r--r--   0        0        0     1387 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
--rw-r--r--   0        0        0     4260 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
--rw-r--r--   0        0        0     1336 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
--rw-r--r--   0        0        0    28585 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
--rw-r--r--   0        0        0    24840 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
--rw-r--r--   0        0        0     9375 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
--rw-r--r--   0        0        0     2771 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
--rw-r--r--   0        0        0     9275 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
--rw-r--r--   0        0        0    13680 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
--rw-r--r--   0        0        0     8010 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
--rw-r--r--   0        0        0     3397 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
--rw-r--r--   0        0        0     9248 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
--rw-r--r--   0        0        0     8666 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
--rw-r--r--   0        0        0    44329 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
--rw-r--r--   0        0        0    28931 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
--rw-r--r--   0        0        0    11740 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
--rw-r--r--   0        0        0    12729 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
--rw-r--r--   0        0        0    47928 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
--rw-r--r--   0        0        0    42060 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
--rw-r--r--   0        0        0    30734 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
--rw-r--r--   0        0        0    13137 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
--rw-r--r--   0        0        0    17315 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
--rw-r--r--   0        0        0    20668 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
--rw-r--r--   0        0        0    25764 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
--rw-r--r--   0        0        0    18556 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
--rw-r--r--   0        0        0     5509 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
--rw-r--r--   0        0        0    13932 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
--rw-r--r--   0        0        0    10477 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
--rw-r--r--   0        0        0     9758 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
--rw-r--r--   0        0        0     7833 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
--rw-r--r--   0        0        0    30645 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
--rw-r--r--   0        0        0    11188 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/InternalHeaderCheck.h
--rw-r--r--   0        0        0     9360 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
--rw-r--r--   0        0        0    13389 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
--rw-r--r--   0        0        0    21746 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
--rw-r--r--   0        0        0     2218 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
--rw-r--r--   0        0        0     9406 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
--rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/InternalHeaderCheck.h
--rw-r--r--   0        0        0    17599 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
--rw-r--r--   0        0        0     9637 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
--rw-r--r--   0        0        0     1287 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
--rw-r--r--   0        0        0    11669 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
--rw-r--r--   0        0        0     1766 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
--rw-r--r--   0        0        0      627 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
--rw-r--r--   0        0        0    23400 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
--rw-r--r--   0        0        0     3569 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
--rw-r--r--   0        0        0     9185 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/util/EmulateArray.h
--rw-r--r--   0        0        0     4336 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
--rw-r--r--   0        0        0     4322 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/Tensor
--rw-r--r--   0        0        0     1224 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/TensorSymmetry
--rw-r--r--   0        0        0     2126 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/CXX11/ThreadPool
--rw-r--r--   0        0        0     1169 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/EulerAngles
--rw-r--r--   0        0        0    15671 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/FFT
--rw-r--r--   0        0        0     3156 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/IterativeSolvers
--rw-r--r--   0        0        0      897 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/KroneckerProduct
--rw-r--r--   0        0        0     1293 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/LevenbergMarquardt
--rw-r--r--   0        0        0    18448 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/MatrixFunctions
--rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/MoreVectorization
--rw-r--r--   0        0        0     7869 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/MPRealSupport
--rw-r--r--   0        0        0    15562 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/NNLS
--rw-r--r--   0        0        0     6109 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/NonLinearOptimization
--rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/NumericalDiff
--rw-r--r--   0        0        0    19400 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/OpenGLSupport
--rw-r--r--   0        0        0     4886 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/Polynomials
--rw-r--r--   0        0        0      969 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/Skyline
--rw-r--r--   0        0        0     1752 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/SparseExtra
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/SpecialFunctions
--rw-r--r--   0        0        0     1031 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/Splines
--rw-r--r--   0        0        0     2628 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
--rw-r--r--   0        0        0    29910 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
--rw-r--r--   0        0        0     9287 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/AutoDiff/InternalHeaderCheck.h
--rw-r--r--   0        0        0    13307 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/BVH/BVAlgorithms.h
--rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/BVH/InternalHeaderCheck.h
--rw-r--r--   0        0        0     9427 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/BVH/KdBVH.h
--rw-r--r--   0        0        0    29903 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Eigenvalues/InternalHeaderCheck.h
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
--rw-r--r--   0        0        0    15760 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/EulerAngles/EulerAngles.h
--rw-r--r--   0        0        0    11957 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/EulerAngles/EulerSystem.h
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/EulerAngles/InternalHeaderCheck.h
--rw-r--r--   0        0        0     9522 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/FFT/ei_fftw_impl.h
--rw-r--r--   0        0        0     9705 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/FFT/ei_imklfft_impl.h
--rw-r--r--   0        0        0    13718 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
--rw-r--r--   0        0        0     2730 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/FFT/ei_pocketfft_impl.h
--rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/FFT/InternalHeaderCheck.h
--rw-r--r--   0        0        0    11761 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/BiCGSTABL.h
--rw-r--r--   0        0        0     5548 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
--rw-r--r--   0        0        0    18299 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
--rw-r--r--   0        0        0    10582 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/GMRES.h
--rw-r--r--   0        0        0    14996 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/IDRS.h
--rw-r--r--   0        0        0    17342 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/IDRSTABL.h
--rw-r--r--   0        0        0     2648 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/InternalHeaderCheck.h
--rw-r--r--   0        0        0     5552 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/IterationController.h
--rw-r--r--   0        0        0    12679 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/MINRES.h
--rw-r--r--   0        0        0     6083 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/IterativeSolvers/Scaling.h
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/KroneckerProduct/InternalHeaderCheck.h
--rw-r--r--   0        0        0    10475 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
--rw-r--r--   0        0        0     2246 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
--rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/LevenbergMarquardt/InternalHeaderCheck.h
--rw-r--r--   0        0        0    13731 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
--rw-r--r--   0        0        0     2565 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
--rw-r--r--   0        0        0     6888 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
--rw-r--r--   0        0        0     5237 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
--rw-r--r--   0        0        0     7031 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/MatrixFunctions/InternalHeaderCheck.h
--rw-r--r--   0        0        0    17103 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
--rw-r--r--   0        0        0    23265 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
--rw-r--r--   0        0        0    17961 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
--rw-r--r--   0        0        0    24165 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
--rw-r--r--   0        0        0    14605 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
--rw-r--r--   0        0        0     2262 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
--rw-r--r--   0        0        0      175 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/MoreVectorization/InternalHeaderCheck.h
--rw-r--r--   0        0        0     3157 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
--rw-r--r--   0        0        0     1968 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/chkder.h
--rw-r--r--   0        0        0     2023 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/covar.h
--rw-r--r--   0        0        0     3442 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
--rw-r--r--   0        0        0     2342 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
--rw-r--r--   0        0        0    20482 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/InternalHeaderCheck.h
--rw-r--r--   0        0        0    22830 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
--rw-r--r--   0        0        0     9447 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
--rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
--rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
--rw-r--r--   0        0        0     3220 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
--rw-r--r--   0        0        0     1449 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NumericalDiff/InternalHeaderCheck.h
--rw-r--r--   0        0        0     4188 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
--rw-r--r--   0        0        0     8394 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Polynomials/Companion.h
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Polynomials/InternalHeaderCheck.h
--rw-r--r--   0        0        0    16101 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
--rw-r--r--   0        0        0     4987 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
--rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Skyline/InternalHeaderCheck.h
--rw-r--r--   0        0        0    11755 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
--rw-r--r--   0        0        0    31949 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Skyline/SkylineMatrix.h
--rw-r--r--   0        0        0     8035 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
--rw-r--r--   0        0        0    11029 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Skyline/SkylineProduct.h
--rw-r--r--   0        0        0     8238 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Skyline/SkylineStorage.h
--rw-r--r--   0        0        0     3280 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Skyline/SkylineUtil.h
--rw-r--r--   0        0        0    41397 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
--rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SparseExtra/InternalHeaderCheck.h
--rw-r--r--   0        0        0    12349 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SparseExtra/MarketIO.h
--rw-r--r--   0        0        0     7853 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
--rw-r--r--   0        0        0    12235 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SparseExtra/RandomSetter.h
--rw-r--r--   0        0        0     8884 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SparseExtra/SparseInverse.h
--rw-r--r--   0        0        0     1538 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
--rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
--rw-r--r--   0        0        0     1690 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
--rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
--rw-r--r--   0        0        0    11233 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
--rw-r--r--   0        0        0     2312 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
--rw-r--r--   0        0        0     1317 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
--rw-r--r--   0        0        0    10339 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
--rw-r--r--   0        0        0     2830 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
--rw-r--r--   0        0        0    12456 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
--rw-r--r--   0        0        0     2648 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
--rw-r--r--   0        0        0    71569 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
--rw-r--r--   0        0        0     4162 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
--rw-r--r--   0        0        0     2594 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
--rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/InternalHeaderCheck.h
--rw-r--r--   0        0        0     7899 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
--rw-r--r--   0        0        0     3183 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
--rw-r--r--   0        0        0    11504 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
--rw-r--r--   0        0        0     2995 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
--rw-r--r--   0        0        0    60874 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
--rw-r--r--   0        0        0     3830 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
--rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Splines/InternalHeaderCheck.h
--rw-r--r--   0        0        0    18851 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Splines/Spline.h
--rw-r--r--   0        0        0    16976 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Splines/SplineFitting.h
--rw-r--r--   0        0        0     4441 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/Eigen/src/Splines/SplineFwd.h
--rw-r--r--   0        0        0     1926 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/README.txt
--rw-r--r--   0        0        0     2487 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/alignedvector3.cpp
--rw-r--r--   0        0        0    11295 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/autodiff.cpp
--rw-r--r--   0        0        0     3015 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/autodiff_scalar.cpp
--rw-r--r--   0        0        0    16779 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/bessel_functions.cpp
--rw-r--r--   0        0        0     1246 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/bicgstabl.cpp
--rw-r--r--   0        0        0     7412 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/BVH.cpp
--rw-r--r--   0        0        0    15234 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/CMakeLists.txt
--rw-r--r--   0        0        0     4129 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_eventcount.cpp
--rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_maxsizevector.cpp
--rw-r--r--   0        0        0    19097 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_meta.cpp
--rw-r--r--   0        0        0     5219 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_non_blocking_thread_pool.cpp
--rw-r--r--   0        0        0     7256 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_runqueue.cpp
--rw-r--r--   0        0        0     9395 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_argmax.cpp
--rw-r--r--   0        0        0     8951 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_argmax_gpu.cu
--rw-r--r--   0        0        0    10176 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_argmax_sycl.cpp
--rw-r--r--   0        0        0     9790 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_assign.cpp
--rw-r--r--   0        0        0    22954 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_block_access.cpp
--rw-r--r--   0        0        0    32740 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_block_eval.cpp
--rw-r--r--   0        0        0    16303 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_block_io.cpp
--rw-r--r--   0        0        0     5852 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
--rw-r--r--   0        0        0     9599 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_broadcasting.cpp
--rw-r--r--   0        0        0    18061 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_builtins_sycl.cpp
--rw-r--r--   0        0        0     2499 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_cast_float16_gpu.cu
--rw-r--r--   0        0        0     5694 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_casts.cpp
--rw-r--r--   0        0        0    13475 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_chipping.cpp
--rw-r--r--   0        0        0    26781 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_chipping_sycl.cpp
--rw-r--r--   0        0        0     2075 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_comparisons.cpp
--rw-r--r--   0        0        0     2973 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu
--rw-r--r--   0        0        0     6822 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_complex_gpu.cu
--rw-r--r--   0        0        0     4767 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_concatenation.cpp
--rw-r--r--   0        0        0     8591 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_concatenation_sycl.cpp
--rw-r--r--   0        0        0     1722 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_const.cpp
--rw-r--r--   0        0        0     8084 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_contract_gpu.cu
--rw-r--r--   0        0        0    48547 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_contract_sycl.cpp
--rw-r--r--   0        0        0    23777 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_contraction.cpp
--rw-r--r--   0        0        0     5531 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_convolution.cpp
--rw-r--r--   0        0        0    20502 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_convolution_sycl.cpp
--rw-r--r--   0        0        0     2486 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_custom_index.cpp
--rw-r--r--   0        0        0     3322 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_custom_op.cpp
--rw-r--r--   0        0        0     6976 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_custom_op_sycl.cpp
--rw-r--r--   0        0        0    15516 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_device.cu
--rw-r--r--   0        0        0     4875 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_device_sycl.cpp
--rw-r--r--   0        0        0     2666 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_dimension.cpp
--rw-r--r--   0        0        0     1039 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_empty.cpp
--rw-r--r--   0        0        0    31479 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_executor.cpp
--rw-r--r--   0        0        0    14745 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_expr.cpp
--rw-r--r--   0        0        0    13973 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_fft.cpp
--rw-r--r--   0        0        0     7513 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_fixed_size.cpp
--rw-r--r--   0        0        0     2246 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_forced_eval.cpp
--rw-r--r--   0        0        0     3538 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
--rw-r--r--   0        0        0     2357 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_generator.cpp
--rw-r--r--   0        0        0     5879 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_generator_sycl.cpp
--rw-r--r--   0        0        0    61025 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_gpu.cu
--rw-r--r--   0        0        0     6096 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_ifft.cpp
--rw-r--r--   0        0        0     3993 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_image_op_sycl.cpp
--rw-r--r--   0        0        0    36846 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_image_patch.cpp
--rw-r--r--   0        0        0    63203 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_image_patch_sycl.cpp
--rw-r--r--   0        0        0    19020 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_index_list.cpp
--rw-r--r--   0        0        0     2190 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_inflation.cpp
--rw-r--r--   0        0        0     5237 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_inflation_sycl.cpp
--rw-r--r--   0        0        0     4276 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_intdiv.cpp
--rw-r--r--   0        0        0     5568 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_io.cpp
--rw-r--r--   0        0        0     1700 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_layout_swap.cpp
--rw-r--r--   0        0        0     4856 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp
--rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_lvalue.cpp
--rw-r--r--   0        0        0     8289 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_map.cpp
--rw-r--r--   0        0        0     1039 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_math.cpp
--rw-r--r--   0        0        0     3982 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_math_sycl.cpp
--rw-r--r--   0        0        0     1554 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_mixed_indices.cpp
--rw-r--r--   0        0        0    18737 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_morphing.cpp
--rw-r--r--   0        0        0    17935 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_morphing_sycl.cpp
--rw-r--r--   0        0        0     1810 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_move.cpp
--rw-r--r--   0        0        0     1853 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_notification.cpp
--rw-r--r--   0        0        0    22370 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_of_bfloat16_gpu.cu
--rw-r--r--   0        0        0     3413 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_of_complex.cpp
--rw-r--r--   0        0        0     2535 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_of_const_values.cpp
--rw-r--r--   0        0        0    21711 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_of_float16_gpu.cu
--rw-r--r--   0        0        0     3918 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_of_strings.cpp
--rw-r--r--   0        0        0     2745 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_padding.cpp
--rw-r--r--   0        0        0     5834 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_padding_sycl.cpp
--rw-r--r--   0        0        0     5671 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_patch.cpp
--rw-r--r--   0        0        0     9634 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_patch_sycl.cpp
--rw-r--r--   0        0        0     2599 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_random.cpp
--rw-r--r--   0        0        0     2441 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_random_gpu.cu
--rw-r--r--   0        0        0     3174 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_random_sycl.cpp
--rw-r--r--   0        0        0    16487 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_reduction.cpp
--rw-r--r--   0        0        0     5564 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_reduction_gpu.cu
--rw-r--r--   0        0        0    43159 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_reduction_sycl.cpp
--rw-r--r--   0        0        0     6970 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_ref.cpp
--rw-r--r--   0        0        0     5475 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_reverse.cpp
--rw-r--r--   0        0        0     9536 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_reverse_sycl.cpp
--rw-r--r--   0        0        0     1548 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_roundings.cpp
--rw-r--r--   0        0        0     3088 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_scan.cpp
--rw-r--r--   0        0        0     2654 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_scan_gpu.cu
--rw-r--r--   0        0        0     6517 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_scan_sycl.cpp
--rw-r--r--   0        0        0     7975 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_shuffling.cpp
--rw-r--r--   0        0        0     4382 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_shuffling_sycl.cpp
--rw-r--r--   0        0        0     9951 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_simple.cpp
--rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_striding.cpp
--rw-r--r--   0        0        0     7277 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_striding_sycl.cpp
--rw-r--r--   0        0        0     1977 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_sugar.cpp
--rw-r--r--   0        0        0    15189 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_sycl.cpp
--rw-r--r--   0        0        0    59897 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_symmetry.cpp
--rw-r--r--   0        0        0     4386 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_thread_local.cpp
--rw-r--r--   0        0        0    26212 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_thread_pool.cpp
--rw-r--r--   0        0        0     5301 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_trace.cpp
--rw-r--r--   0        0        0     5917 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_uint128.cpp
--rw-r--r--   0        0        0     4704 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_volume_patch.cpp
--rw-r--r--   0        0        0    12194 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp
--rw-r--r--   0        0        0     1310 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/dgmres.cpp
--rw-r--r--   0        0        0     9919 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/EulerAngles.cpp
--rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/FFT.cpp
--rw-r--r--   0        0        0    10124 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/fft_test_shared.h
--rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/FFTW.cpp
--rw-r--r--   0        0        0     3963 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/forward_adolc.cpp
--rw-r--r--   0        0        0     1276 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/gmres.cpp
--rw-r--r--   0        0        0      969 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/idrs.cpp
--rw-r--r--   0        0        0     1084 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/idrstabl.cpp
--rw-r--r--   0        0        0     9323 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/kronecker_product.cpp
--rw-r--r--   0        0        0    58270 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/levenberg_marquardt.cpp
--rw-r--r--   0        0        0     4558 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/matrix_exponential.cpp
--rw-r--r--   0        0        0     7674 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/matrix_function.cpp
--rw-r--r--   0        0        0     2173 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/matrix_functions.h
--rw-r--r--   0        0        0     7346 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/matrix_power.cpp
--rw-r--r--   0        0        0     1081 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/matrix_square_root.cpp
--rw-r--r--   0        0        0     1702 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/minres.cpp
--rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/mklfft.cpp
--rw-r--r--   0        0        0     2505 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/mpreal_support.cpp
--rw-r--r--   0        0        0    16108 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/NNLS.cpp
--rw-r--r--   0        0        0    67623 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/NonLinearOptimization.cpp
--rw-r--r--   0        0        0     2976 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/NumericalDiff.cpp
--rw-r--r--   0        0        0    19237 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/openglsupport.cpp
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/pocketfft.cpp
--rw-r--r--   0        0        0     7718 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/polynomialsolver.cpp
--rw-r--r--   0        0        0     3695 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/polynomialutils.cpp
--rw-r--r--   0        0        0     9462 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/sparse_extra.cpp
--rw-r--r--   0        0        0    23366 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/special_functions.cpp
--rw-r--r--   0        0        0     6492 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/special_packetmath.cpp
--rw-r--r--   0        0        0     8810 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/eigen/unsupported/test/splines.cpp
--rw-r--r--   0        0        0     3817 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/.clang-format
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/.codecov.yml
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/.git
--rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/.github/workflows/Basic.yml
--rw-r--r--   0        0        0      481 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/.github/workflows/checkformat.yml
--rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/.gitignore
--rw-r--r--   0        0        0     2135 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/.travis.yml
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/AUTHORS.md
--rw-r--r--   0        0        0     6259 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/benchmark/ArpackFun.h
--rw-r--r--   0        0        0     2553 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/benchmark/Cpp.cpp
--rw-r--r--   0        0        0     9721 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/benchmark/F77.cpp
--rw-r--r--   0        0        0     4631 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/benchmark/main.cpp
--rw-r--r--   0        0        0      674 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/benchmark/Makefile
--rw-r--r--   0        0        0     2414 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/benchmark/result_analyzer.R
--rw-r--r--   0        0        0     1343 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/benchmark/timer.h
--rw-r--r--   0        0        0     4984 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/benchmark/wrapper.f
--rw-r--r--   0        0        0    14871 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/CHANGELOG.md
--rw-r--r--   0        0        0     2224 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/cmake/FindCLANG_FORMAT.cmake
--rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/cmake/spectra-config.cmake.in
--rw-r--r--   0        0        0     3427 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/CMakeLists.txt
--rw-r--r--   0        0        0   117216 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/doxygen/Doxyfile
--rw-r--r--   0        0        0     8481 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/doxygen/Overview.md
--rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/examples/CMakeLists.txt
--rw-r--r--   0        0        0     1152 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/examples/DavidsonSymEigs_example.cpp
--rw-r--r--   0        0        0     3160 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/examples/DavidsonSymEigs_example.md
--rw-r--r--   0        0        0    19269 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/contrib/LOBPCGSolver.h
--rw-r--r--   0        0        0     6132 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/contrib/PartialSVDSolver.h
--rw-r--r--   0        0        0     3429 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/DavidsonSymEigsSolver.h
--rw-r--r--   0        0        0    18718 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/GenEigsBase.h
--rw-r--r--   0        0        0     6914 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/GenEigsComplexShiftSolver.h
--rw-r--r--   0        0        0     3603 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/GenEigsRealShiftSolver.h
--rw-r--r--   0        0        0     5382 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/GenEigsSolver.h
--rw-r--r--   0        0        0     6825 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/JDSymEigsBase.h
--rw-r--r--   0        0        0    11229 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/Arnoldi.h
--rw-r--r--   0        0        0    18033 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/BKLDLT.h
--rw-r--r--   0        0        0    15208 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/DoubleShiftQR.h
--rw-r--r--   0        0        0     6453 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/Lanczos.h
--rw-r--r--   0        0        0     5847 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/Orthogonalization.h
--rw-r--r--   0        0        0     4602 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/RitzPairs.h
--rw-r--r--   0        0        0     3484 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/SearchSpace.h
--rw-r--r--   0        0        0     8006 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/TridiagEigen.h
--rw-r--r--   0        0        0    12764 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/UpperHessenbergEigen.h
--rw-r--r--   0        0        0    28787 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/UpperHessenbergQR.h
--rw-r--r--   0        0        0    17124 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/LinAlg/UpperHessenbergSchur.h
--rw-r--r--   0        0        0     4226 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/DenseCholesky.h
--rw-r--r--   0        0        0     4152 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/DenseGenComplexShiftSolve.h
--rw-r--r--   0        0        0     3464 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/DenseGenMatProd.h
--rw-r--r--   0        0        0     3462 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/DenseGenRealShiftSolve.h
--rw-r--r--   0        0        0     3559 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/DenseSymMatProd.h
--rw-r--r--   0        0        0     3753 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/DenseSymShiftSolve.h
--rw-r--r--   0        0        0     4059 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/internal/ArnoldiOp.h
--rw-r--r--   0        0        0     2766 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h
--rw-r--r--   0        0        0     3268 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h
--rw-r--r--   0        0        0     2635 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h
--rw-r--r--   0        0        0     2414 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h
--rw-r--r--   0        0        0     2797 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h
--rw-r--r--   0        0        0     4462 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/SparseCholesky.h
--rw-r--r--   0        0        0     4469 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/SparseGenComplexShiftSolve.h
--rw-r--r--   0        0        0     3577 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/SparseGenMatProd.h
--rw-r--r--   0        0        0     3816 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/SparseGenRealShiftSolve.h
--rw-r--r--   0        0        0     4816 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/SparseRegularInverse.h
--rw-r--r--   0        0        0     3803 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/SparseSymMatProd.h
--rw-r--r--   0        0        0     4103 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/SparseSymShiftSolve.h
--rw-r--r--   0        0        0    10422 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/MatOp/SymShiftInvert.h
--rw-r--r--   0        0        0    15582 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/SymEigsBase.h
--rw-r--r--   0        0        0     7974 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/SymEigsShiftSolver.h
--rw-r--r--   0        0        0     6229 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/SymEigsSolver.h
--rw-r--r--   0        0        0    21918 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/SymGEigsShiftSolver.h
--rw-r--r--   0        0        0    13480 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/SymGEigsSolver.h
--rw-r--r--   0        0        0     1249 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/Util/CompInfo.h
--rw-r--r--   0        0        0      987 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/Util/GEigsMode.h
--rw-r--r--   0        0        0     9208 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/Util/SelectionRule.h
--rw-r--r--   0        0        0     2940 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/Util/SimpleRandom.h
--rw-r--r--   0        0        0     2464 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/Util/TypeTraits.h
--rw-r--r--   0        0        0      572 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/include/Spectra/Util/Version.h
--rw-r--r--   0        0        0    17098 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/LICENSE
--rw-r--r--   0        0        0     3940 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/MIGRATION.md
--rw-r--r--   0        0        0    10387 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/README.md
--rw-r--r--   0        0        0     2023 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/BKLDLT.cpp
--rw-r--r--   0        0        0   675140 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/catch.hpp
--rw-r--r--   0        0        0     1320 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/CMakeLists.txt
--rw-r--r--   0        0        0     3377 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/DavidsonSymEigs.cpp
--rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/DenseGenMatProd.cpp
--rw-r--r--   0        0        0      984 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/DenseSymMatProd.cpp
--rw-r--r--   0        0        0     3372 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/Eigen.cpp
--rw-r--r--   0        0        0     4442 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/GenEigs.cpp
--rw-r--r--   0        0        0     5064 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/GenEigsComplexShift.cpp
--rw-r--r--   0        0        0     4707 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/GenEigsRealShift.cpp
--rw-r--r--   0        0        0     1181 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/JDSymEigsBase.cpp
--rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/JDSymEigsDPRConstructor.cpp
--rw-r--r--   0        0        0     1654 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/Makefile
--rw-r--r--   0        0        0     2184 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/Orthogonalization.cpp
--rw-r--r--   0        0        0     5901 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/QR.cpp
--rw-r--r--   0        0        0     1282 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/RitzPairs.cpp
--rw-r--r--   0        0        0     2246 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/Schur.cpp
--rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/SearchSpace.cpp
--rw-r--r--   0        0        0     1687 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/SparseGenMatProd.cpp
--rw-r--r--   0        0        0     1774 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/SparseSymMatProd.cpp
--rw-r--r--   0        0        0     2940 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/SVD.cpp
--rw-r--r--   0        0        0     4232 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/SymEigs.cpp
--rw-r--r--   0        0        0     4905 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/SymEigsShift.cpp
--rw-r--r--   0        0        0     5761 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/SymGEigsCholesky.cpp
--rw-r--r--   0        0        0     4155 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/SymGEigsRegInv.cpp
--rw-r--r--   0        0        0    11616 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/SymGEigsShift.cpp
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 qm-sim-0.1.0/lib/spectra/test/tests-main.cpp
--rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 qm-sim-0.1.0/LICENSE
--rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 qm-sim-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2214 2022-11-09 12:37:21.000000 qm-sim-0.1.0/README.md
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 qm-sim-0.1.0/setup.cfg
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/__init__.py
--rw-r--r--   0        0        0      120 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/__init__.py
--rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/CMakeLists.txt
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/eigen/__init__.py
--rw-r--r--   0        0        0      735 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/eigen/CMakeLists.txt
--rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/eigen/include/eigensolver.hpp
--rw-r--r--   0        0        0     1495 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/eigen/include/HamiltonianBase.hpp
--rw-r--r--   0        0        0      534 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/eigen/scripts/generate_init.py
--rw-r--r--   0        0        0     1029 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/eigen/src/eigensolver.cpp
--rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/eigen/src/HamiltonianBase.cpp
--rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/eigen/wrapper/CMakeLists.txt
--rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/cpp/eigen/wrapper/py_interface.cpp
--rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/eigensolvers/__init__.py
--rw-r--r--   0        0        0     1384 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/eigensolvers/pytorch_eigen.py
--rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/eigensolvers/scipy_eigen.py
--rw-r--r--   0        0        0      300 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/hamiltonian/__init__.py
--rw-r--r--   0        0        0    14377 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/hamiltonian/spatial_hamiltonian.py
--rw-r--r--   0        0        0      660 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/nature_constants.py
--rw-r--r--   0        0        0     3618 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/plot.py
--rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/spatial_derivative/__init__.py
--rw-r--r--   0        0        0     6919 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/spatial_derivative/cartesian.py
--rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/temporal_solver/__init__.py
--rw-r--r--   0        0        0     3321 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/temporal_solver/base.py
--rw-r--r--   0        0        0     2281 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/temporal_solver/crank_nicolson.py
--rw-r--r--   0        0        0     1569 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/temporal_solver/leapfrog.py
--rw-r--r--   0        0        0     2160 2022-11-09 12:37:21.000000 qm-sim-0.1.0/src/qm_sim/temporal_solver/scipy_solvers.py
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/test_eigensolvers/__init__.py
--rw-r--r--   0        0        0     3771 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/test_eigensolvers/scipy_backend.py
--rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/test_eigensolvers/test_eigensolvers.py
--rw-r--r--   0        0        0     4884 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tests/test_hamiltonian.py
--rw-r--r--   0        0        0  2014437 2022-11-09 12:37:21.000000 qm-sim-0.1.0/tmp.png
--rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 qm-sim-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0      623 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.github/workflows/build_package.yml
+-rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.github/workflows/linting.yml
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.gitignore
+-rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 qm-sim-0.1.1/.gitmodules
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 qm-sim-0.1.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 qm-sim-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2648 2022-11-09 12:37:21.000000 qm-sim-0.1.1/README.md
+-rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1219 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0      120 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/api.rst
+-rw-r--r--   0        0        0     1160 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/contribution.rst
+-rw-r--r--   0        0        0      869 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/examples.rst
+-rw-r--r--   0        0        0      553 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 qm-sim-0.1.1/docs/source/usage.rst
+-rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/01_zero_potential.py
+-rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/02_quadratic_potential.py
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/03_2D_potential.py
+-rw-r--r--   0        0        0     1643 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/04_adiabatic_evolution.py
+-rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/05_temporal_evolution.py
+-rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/06_2D_temporal_evolution.py
+-rw-r--r--   0        0        0     1405 2022-11-09 12:37:21.000000 qm-sim-0.1.1/examples/07_hydrogen_atom.py
+-rw-r--r--   0        0        0     1519 2022-11-09 12:37:21.000000 qm-sim-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 qm-sim-0.1.1/setup.cfg
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/__init__.py
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/__init__.py
+-rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/CMakeLists.txt
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/__init__.py
+-rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/include/HamiltonianBase.hpp
+-rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/include/eigensolver.hpp
+-rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/scripts/generate_init.py
+-rw-r--r--   0        0        0     2436 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/src/HamiltonianBase.cpp
+-rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/src/eigensolver.cpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/wrapper/CMakeLists.txt
+-rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/cpp/eigen/wrapper/py_interface.cpp
+-rw-r--r--   0        0        0      824 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/eigensolvers/__init__.py
+-rw-r--r--   0        0        0     1342 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/eigensolvers/pytorch_eigen.py
+-rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/eigensolvers/scipy_eigen.py
+-rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/hamiltonian/__init__.py
+-rw-r--r--   0        0        0    14888 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/hamiltonian/spatial_hamiltonian.py
+-rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/nature_constants.py
+-rw-r--r--   0        0        0     3571 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/plot.py
+-rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/spatial_derivative/__init__.py
+-rw-r--r--   0        0        0     6820 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/spatial_derivative/cartesian.py
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/__init__.py
+-rw-r--r--   0        0        0     3295 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/base.py
+-rw-r--r--   0        0        0     2261 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/crank_nicolson.py
+-rw-r--r--   0        0        0     1582 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/leapfrog.py
+-rw-r--r--   0        0        0     2114 2022-11-09 12:37:21.000000 qm-sim-0.1.1/src/qm_sim/temporal_solver/scipy_solvers.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/test_eigensolvers/__init__.py
+-rw-r--r--   0        0        0     3655 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/test_eigensolvers/scipy_backend.py
+-rw-r--r--   0        0        0     3890 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/test_eigensolvers/test_eigensolvers.py
+-rw-r--r--   0        0        0     4630 2022-11-09 12:37:21.000000 qm-sim-0.1.1/tests/test_hamiltonian.py
+-rw-r--r--   0        0        0     3918 2022-11-09 12:37:21.000000 qm-sim-0.1.1/PKG-INFO
```

### Comparing `qm-sim-0.1.0/docs/make.bat` & `qm-sim-0.1.1/docs/make.bat`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=source
-set BUILDDIR=build
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=source
+set BUILDDIR=build
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.https://www.sphinx-doc.org/
+	exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `qm-sim-0.1.0/docs/Makefile` & `qm-sim-0.1.1/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = source
-BUILDDIR      = build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = source
+BUILDDIR      = build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `qm-sim-0.1.0/docs/source/conf.py` & `qm-sim-0.1.1/docs/source/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-
-project = 'QM sim'
-copyright = '2023, Viljar Femoen'
-author = 'Viljar Femoen'
-release = '0.0.3'
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = [
-    'sphinx.ext.duration',
-    'sphinx.ext.doctest',
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.viewcode',
-]
-
-
-autosummary_generate = True  # Turn on sphinx.ext.autosummary
-
-templates_path = ['_templates']
-exclude_patterns = []
-
-
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-html_theme = 'sphinx_rtd_theme'
-html_static_path = ['_static']
-
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+
+project = 'QM sim'
+copyright = '2023, Viljar Femoen'
+author = 'Viljar Femoen'
+release = '0.1.1'
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = [
+    'sphinx.ext.duration',
+    'sphinx.ext.doctest',
+    'sphinx.ext.autodoc',
+    'sphinx.ext.autosummary',
+    'sphinx.ext.viewcode',
+    'sphinx_mdinclude'
+]
+
+
+autosummary_generate = True  # Turn on sphinx.ext.autosummary
+
+templates_path = ['_templates']
+exclude_patterns = []
+
+
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+
+html_theme = 'sphinx_rtd_theme'
+html_static_path = ['_static']
+
```

### Comparing `qm-sim-0.1.0/docs/source/contribution.rst` & `qm-sim-0.1.1/docs/source/contribution.rst`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Contribution
-============
-
-To contribute, please open a pull request to the :code:`dev`-branch on `GitHub <https://www.github.com/viljarjf/QM_sim/pulls>`_.
-
-The following is an example of how to set up VS Code for development, adapt to your IDE of choice.
-
-TL;DR:
------- 
-
-:code:`pip install -e .`
-
-Requirements
-------------
-
-- VS Code with the Python extension
-- Python 3.10 or above
-
-Setup
------
-
-1. Clone the repo recursively and open the repo in VS Code. If not cloned recursively, initialize the submodules with :code:`git submodule update --init`
-2. Press f1, and run :code:`Python: Create Environment`. Select :code:`.venv`
-3. Open a new terminal, which should automatically use the virtual environment. If not, run :code:`.venv\\Scripts\\activate` on Windows, or :code:`source .venv/bin/activate` on Unix
-4. In the same terminal, run :code:`pip install -e .[test]` to install the current directory in an editable state, and the testing utility Pytest
-5. To run tests, press f1 and run :code:`Python: Configure Tests`. Choose :code:`pytest`. Run tests in the testing menu
+Contribution
+============
+
+To contribute, please open a pull request to the :code:`dev`-branch on `GitHub <https://www.github.com/viljarjf/QM_sim/pulls>`_.
+
+The following is an example of how to set up VS Code for development, adapt to your IDE of choice.
+
+TL;DR:
+------ 
+
+:code:`pip install -e .`
+
+Requirements
+------------
+
+- VS Code with the Python extension
+- Python 3.10 or above
+
+Setup
+-----
+
+1. Clone the repo recursively and open the repo in VS Code. If not cloned recursively, initialize the submodules with :code:`git submodule update --init`
+2. Press f1, and run :code:`Python: Create Environment`. Select :code:`.venv`
+3. Open a new terminal, which should automatically use the virtual environment. If not, run :code:`.venv\\Scripts\\activate` on Windows, or :code:`source .venv/bin/activate` on Unix
+4. In the same terminal, run :code:`pip install -e .[test]` to install the current directory in an editable state, and the testing utility Pytest
+5. To run tests, press f1 and run :code:`Python: Configure Tests`. Choose :code:`pytest`. Run tests in the testing menu
```

### Comparing `qm-sim-0.1.0/examples/03_2D_potential.py` & `qm-sim-0.1.1/examples/03_2D_potential.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""
-
-Calculate and plot eigenstates in a 2D potential
-
-"""
-from qm_sim.hamiltonian import Hamiltonian
-from qm_sim.nature_constants import m_e, e_0
-
-import numpy as np
-
-N = (200, 200)          # Discretisation point count
-L = (8e-9, 8e-9)        # System size in meters
-m = m_e                 # Mass of the particle, here chosen as electron mass
-n = 4                   # The amount of eigenstates to find
-
-# Set hamiltonian
-H = Hamiltonian(N, L, m)
-
-# Set potential. Here, a square well is used, with dV = 0.15 eV
-V = 0.15*e_0 * np.ones(N)
-V[
-    N[0] // 2 - N[0] // 5 : N[0] // 2 + N[0] // 5, 
-    N[1] // 2 - N[1] // 5 : N[1] // 2 + N[1] // 5
-] = 0
-H.V = V
-
-# Plot potential
-H.plot_potential()
-
-# Plot eigenstate
-H.plot_eigen(n)
+"""
+
+Calculate and plot eigenstates in a 2D potential
+
+"""
+from qm_sim.hamiltonian import Hamiltonian
+from qm_sim.nature_constants import m_e, e_0
+
+import numpy as np
+
+N = (200, 200)          # Discretisation point count
+L = (8e-9, 8e-9)        # System size in meters
+m = m_e                 # Mass of the particle, here chosen as electron mass
+n = 4                   # The amount of eigenstates to find
+
+# Set hamiltonian
+H = Hamiltonian(N, L, m)
+
+# Set potential. Here, a square well is used, with dV = 0.15 eV
+V = 0.15*e_0 * np.ones(N)
+V[
+    N[0] // 2 - N[0] // 5 : N[0] // 2 + N[0] // 5, 
+    N[1] // 2 - N[1] // 5 : N[1] // 2 + N[1] // 5
+] = 0
+H.V = V
+
+# Plot potential
+H.plot_potential()
+
+# Plot eigenstate
+H.plot_eigen(n)
```

### Comparing `qm-sim-0.1.0/examples/04_adiabatic_evolution.py` & `qm-sim-0.1.1/examples/04_adiabatic_evolution.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import matplotlib.pyplot as plt
-import numpy as np
-from matplotlib.animation import FuncAnimation
-from scipy.special import expit
-
-from qm_sim.hamiltonian import Hamiltonian
-from qm_sim.nature_constants import e_0, m_e
-
-s = 100
-N = (s, s)              # Discretisation point count
-L = (8e-9, 8e-9)        # System size in meters
-m = m_e                 # Mass of the particle, here chosen as electron mass
-n = 4                   # The amount of eigenstates to find
-steps = 100
-
-
-H = Hamiltonian(N, L, m)
-
-# Set potential. Here, a square well is used, with dV = 0.15 eV
-x,y = np.linspace(-L[0]/2,L[0]/2, N[0]), np.linspace(-L[0]/2,L[0]/2, N[1])
-X, Y = np.meshgrid(x,y)
-
-# Smoothed rectangular time-dependent potential, assymetric to avoid degeneracy 
-def V(t):
-    a = 0.15*e_0*expit(5*10**9*(X-2e-9 + 1e-11*t)) + 0.15*e_0*expit(-5*10**9*(X+2e-9-1e-11*t))
-    b = 0.15*e_0*expit(5*10**9*(Y-2.5e-9 - 1e-11*t)) + 0.15*e_0*expit(-5*10**9*(Y+2.5e-9+1e-11*t))
-    return np.where(a+b>0.15*e_0,0.15*e_0,a+b)
-
-H.V = V
-
-# Solve the system
-energies, states = H.eigen(n)
-# Choose energy to follow
-E = energies[1]
-
-# Evolve adiabatically
-Energies, psi = H.adiabatic_evolution(E_n=E, t0=0, dt=1, steps=steps)
-
-# Create animation
-fig, (ax, ax2) = plt.subplots(1,2)
-im = ax.matshow(psi[:,:,0]**2)
-im2 = ax2.matshow(V(0).T)
-ims = [im,im2]
-
-def init():
-    im.set_data(psi[:,:,0]**2)
-    im2.set_data(V(0).T)
-    return im
-
-def update(j):
-    ims[0].set_data(psi[:,:,j]**2)
-    ims[1].set_data(V(j).T)
-    return ims
-
-anim = FuncAnimation(fig, func=update, init_func=init, frames=steps, interval=50, blit=False, repeat = True, repeat_delay = 1000)
-plt.show()
+import matplotlib.pyplot as plt
+import numpy as np
+from matplotlib.animation import FuncAnimation
+from scipy.special import expit
+
+from qm_sim.hamiltonian import Hamiltonian
+from qm_sim.nature_constants import e_0, m_e
+
+s = 100
+N = (s, s)              # Discretisation point count
+L = (8e-9, 8e-9)        # System size in meters
+m = m_e                 # Mass of the particle, here chosen as electron mass
+n = 4                   # The amount of eigenstates to find
+steps = 100
+
+
+H = Hamiltonian(N, L, m)
+
+# Set potential. Here, a square well is used, with dV = 0.15 eV
+x,y = np.linspace(-L[0]/2,L[0]/2, N[0]), np.linspace(-L[0]/2,L[0]/2, N[1])
+X, Y = np.meshgrid(x,y)
+
+# Smoothed rectangular time-dependent potential, assymetric to avoid degeneracy 
+def V(t):
+    a = 0.15*e_0*expit(5*10**9*(X-2e-9 + 1e-11*t)) + 0.15*e_0*expit(-5*10**9*(X+2e-9-1e-11*t))
+    b = 0.15*e_0*expit(5*10**9*(Y-2.5e-9 - 1e-11*t)) + 0.15*e_0*expit(-5*10**9*(Y+2.5e-9+1e-11*t))
+    return np.where(a+b>0.15*e_0,0.15*e_0,a+b)
+
+H.V = V
+
+# Solve the system
+energies, states = H.eigen(n)
+# Choose energy to follow
+E = energies[1]
+
+# Evolve adiabatically
+Energies, psi = H.adiabatic_evolution(E_n=E, t0=0, dt=1, steps=steps)
+
+# Create animation
+fig, (ax, ax2) = plt.subplots(1,2)
+im = ax.matshow(psi[:,:,0]**2)
+im2 = ax2.matshow(V(0).T)
+ims = [im,im2]
+
+def init():
+    im.set_data(psi[:,:,0]**2)
+    im2.set_data(V(0).T)
+    return im
+
+def update(j):
+    ims[0].set_data(psi[:,:,j]**2)
+    ims[1].set_data(V(j).T)
+    return ims
+
+anim = FuncAnimation(fig, func=update, init_func=init, frames=steps, interval=50, blit=False, repeat = True, repeat_delay = 1000)
+plt.show()
```

### Comparing `qm-sim-0.1.0/examples/06_2D_temporal_evolution.py` & `qm-sim-0.1.1/examples/06_2D_temporal_evolution.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import numpy as np
-
-from qm_sim.hamiltonian import Hamiltonian
-from qm_sim.nature_constants import e_0, m_e
-from scipy.signal import convolve2d
-
-N = (100, 100)          # Discretisation point count
-L = (15e-9, 15e-9)      # System size in meters
-m = m_e                 # Mass of the particle, here chosen as electron mass
-t_end = 100e-15         # Simulation time
-dt = 1e-16              # Simulation data storage stepsize
-
-# Initialize the hamiltonian.
-H = Hamiltonian(N, L, m, temporal_scheme="scipy-Runge-Kutta 3(2)")
-
-# Set the potential. Use a cool elipse cross that rotates over time
-a = 2e-9
-b = 5e-9
-x = np.linspace(-L[0]/2, L[0]/2, N[0])
-y = np.linspace(-L[1]/2, L[1]/2, N[1])
-X, Y = np.meshgrid(x, y)
-def V(theta: float) -> np.ndarray:
-    ct, st = np.cos(theta), np.sin(theta)
-
-    V = np.ones(N) * e_0
-    V[((X*ct + Y*st) / a)**2 + ((X*st - Y*ct) / b)**2 <= 1] = 0
-    V[((X*ct + Y*st) / b)**2 + ((X*st - Y*ct) / a)**2 <= 1] = 0
-
-    # Smooth out transition 
-    n = 5
-    kernel = np.ones((n,n)) / n**2
-    V = convolve2d(V, kernel, mode="same", boundary="wrap")
-    return V
-    
-H.V = lambda t: V(1e14*t)
-
-# Set initial condition to a
-# superposition of third and fourth eigenstate
-_, psi = H.eigen(4)
-psi_0 = 1/2**0.5 * (psi[2] + psi[3])
-
-# Plot
-H.plot_potential()
-H.plot_eigen(4)
-H.plot_temporal(t_end, dt, psi_0)
+import numpy as np
+
+from qm_sim.hamiltonian import Hamiltonian
+from qm_sim.nature_constants import e_0, m_e
+from scipy.signal import convolve2d
+
+N = (100, 100)          # Discretisation point count
+L = (15e-9, 15e-9)      # System size in meters
+m = m_e                 # Mass of the particle, here chosen as electron mass
+t_end = 100e-15         # Simulation time
+dt = 1e-16              # Simulation data storage stepsize
+
+# Initialize the hamiltonian.
+H = Hamiltonian(N, L, m, temporal_scheme="scipy-Runge-Kutta 3(2)")
+
+# Set the potential. Use a cool elipse cross that rotates over time
+a = 2e-9
+b = 5e-9
+x = np.linspace(-L[0]/2, L[0]/2, N[0])
+y = np.linspace(-L[1]/2, L[1]/2, N[1])
+X, Y = np.meshgrid(x, y)
+def V(theta: float) -> np.ndarray:
+    ct, st = np.cos(theta), np.sin(theta)
+
+    V = np.ones(N) * e_0
+    V[((X*ct + Y*st) / a)**2 + ((X*st - Y*ct) / b)**2 <= 1] = 0
+    V[((X*ct + Y*st) / b)**2 + ((X*st - Y*ct) / a)**2 <= 1] = 0
+
+    # Smooth out transition 
+    n = 5
+    kernel = np.ones((n,n)) / n**2
+    V = convolve2d(V, kernel, mode="same", boundary="wrap")
+    return V
+    
+H.V = lambda t: V(1e14*t)
+
+# Set initial condition to a
+# superposition of third and fourth eigenstate
+_, psi = H.eigen(4)
+psi_0 = 1/2**0.5 * (psi[2] + psi[3])
+
+# Plot
+H.plot_potential()
+H.plot_eigen(4)
+H.plot_temporal(t_end, dt, psi_0)
```

### Comparing `qm-sim-0.1.0/examples/07_hydrogen_atom.py` & `qm-sim-0.1.1/examples/07_hydrogen_atom.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# NOTE: this example uses skimage, available with:
-# `pip install scikit-image`
-from skimage import measure
-
-import numpy as np
-import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-
-from qm_sim.hamiltonian import Hamiltonian
-from qm_sim.nature_constants import e_0, 𝜀_0, m_e, m_p
-
-N = (60, 60, 60)            # Discretisation point count
-L = (1e-9, 1e-9, 1e-9)      # System size in meters
-m = m_e * m_p / (m_e + m_p) # Mass of the particle, here the reduced mass of the system
-
-nx, ny = 2, 2               # Used for the plot
-n = nx * ny                 # Number of orbitals to find
-
-# Initialize the hamiltonian.
-H = Hamiltonian(N, L, m)
-
-# Define the potential: -e^2 / (4*pi*𝜀_0*r)
-x, y, z = np.meshgrid(*(np.linspace(-L[i]/2, L[i]/2, N[i]) for i in range(3)))
-r = (x**2 + y**2 + z**2)**0.5
-H.V = -e_0**2 / (4 * np.pi * 𝜀_0 * r)
-
-# Find a couple eigenvalues
-energies, orbitals = H.eigen(n)
-orbitals = np.abs(orbitals**2)
-
-# Plot a iso-surface of each orbital
-plt.figure()
-plots = []
-for i in range(n):
-    iso_val = np.mean(orbitals[i])
-    vertices, faces, _, _ = measure.marching_cubes(orbitals[i], iso_val, spacing=L)
-    ax = plt.subplot(ny, nx, i+1, projection='3d')
-    plots.append(ax.plot_trisurf(vertices[:, 0], vertices[:,1], faces, vertices[:, 2],
-                    cmap='Spectral', lw=1))
-    plt.title(f"E = {energies[i] :.2e}")
-plt.tight_layout()
-plt.show()
+# NOTE: this example uses skimage, available with:
+# `pip install scikit-image`
+from skimage import measure
+
+import numpy as np
+import matplotlib.pyplot as plt
+from mpl_toolkits.mplot3d import Axes3D
+
+from qm_sim.hamiltonian import Hamiltonian
+from qm_sim.nature_constants import e_0, 𝜀_0, m_e, m_p
+
+N = (60, 60, 60)            # Discretisation point count
+L = (1e-9, 1e-9, 1e-9)      # System size in meters
+m = m_e * m_p / (m_e + m_p) # Mass of the particle, here the reduced mass of the system
+
+nx, ny = 2, 2               # Used for the plot
+n = nx * ny                 # Number of orbitals to find
+
+# Initialize the hamiltonian.
+H = Hamiltonian(N, L, m)
+
+# Define the potential: -e^2 / (4*pi*𝜀_0*r)
+x, y, z = np.meshgrid(*(np.linspace(-L[i]/2, L[i]/2, N[i]) for i in range(3)))
+r = (x**2 + y**2 + z**2)**0.5
+H.V = -e_0**2 / (4 * np.pi * 𝜀_0 * r)
+
+# Find a couple eigenvalues
+energies, orbitals = H.eigen(n)
+orbitals = np.abs(orbitals**2)
+
+# Plot a iso-surface of each orbital
+plt.figure()
+plots = []
+for i in range(n):
+    iso_val = np.mean(orbitals[i])
+    vertices, faces, _, _ = measure.marching_cubes(orbitals[i], iso_val, spacing=L)
+    ax = plt.subplot(ny, nx, i+1, projection='3d')
+    plots.append(ax.plot_trisurf(vertices[:, 0], vertices[:,1], faces, vertices[:, 2],
+                    cmap='Spectral', lw=1))
+    plt.title(f"E = {energies[i] :.2e}")
+plt.tight_layout()
+plt.show()
```

### Comparing `qm-sim-0.1.0/README.md` & `qm-sim-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,70 @@
-# QM_sim
-
-Python library for simulation of quantum mechanical systems.
-
-[![.github/workflows/build_docs.yml](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml/badge.svg?branch=main&event=page_build)](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml)
-
-## Features 
-- 1D, 2D, and 3D systems
-- Choice of finite difference scheme
-- Zero and periodic boundary conditions
-- Stationary and temporal solutions
-- Plots
-
-## Planned features
-- Transfer matrix for transmission ect.
-- Testing
-
-## Installation
-
-`pip install qm-sim`
-
-To be able to use the [PyTorch](https://pytorch.org/) backend for eigenvalue calculations, run the following command: 
-
-`pip install qm-sim .[torch]`
-
-This will install the cpu-version of the package. To run GPU calculations, install the version for your system at the [PyTorch website](https://pytorch.org/get-started/locally/) instead.
-
-## Usage
-
-Examples are provided in the `examples/`-folder.
-These are enumerated with increasing level of simulation complexity.
-
-## Contribution
-
-To contribute, please open a pull request to the `dev`-branch on [GitHub](https://www.github.com/viljarjf/QM_sim/pulls).
-
-The following is an example of how to set up VS Code for development, adapt to your IDE of choice.
-
-TL;DR: 
-- `pip install -e .` to install in an editable state
-- `pip install .` to (re)compile the C++ (subsequent python file edits will not be recognized before another reinstall)
-
-### Requirements
-- VS Code
-    - Python extension
-- Python 3.10 or above
-
-### Setup
-1. Clone the repo recursively and open the repo in VS Code. If not cloned recursively, initialize the submodules with `git submodule update --init`
-2. Press f1, and run `Python: Create Environment`. Select `.venv`
-3. Open a new terminal, which should automatically use the virtual environment. If not, run `.venv\Scripts\activate` on Windows, or `source .venv/bin/activate` on Unix
-4. In the same terminal, run `pip install -e .[test]` to install the current directory in an editable state, and the testing utility Pytest
-5. To run tests, press f1 and run `Python: Configure Tests`. Choose `pytest`. Run tests in the testing menu
+# QM_sim
+
+Python library for simulation of quantum mechanical systems.
+
+[![Build docs](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml/badge.svg)](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml)
+
+[//]: # (This is a comment. This comment should be on line 7. If this changes, also change the hard-coded line number for the start-line for the mdinclude at the top of docs/source/index.rst )
+
+## Features 
+- 1D, 2D, and 3D systems
+- Choice of finite difference scheme
+- Zero and periodic boundary conditions
+- Stationary and temporal solutions
+- Plots
+
+## Planned features
+- Transfer matrix for transmission ect.
+- Proper testing
+
+[//]: # (This is a comment. This comment should be on line 20. If this changes, also change the hard-coded line number for the end-line for the mdinclude at the top of docs/source/index.rst )
+
+## Installation
+
+`pip install qm-sim`
+
+To be able to use the [PyTorch](https://pytorch.org/) backend for eigenvalue calculations, run the following command: 
+
+`pip install qm-sim[torch]`
+
+This will install the cpu-version of the package. To run GPU calculations, install the version for your system at the [PyTorch website](https://pytorch.org/get-started/locally/) instead.
+
+## Usage
+
+Examples are provided in the `examples/`-folder.
+These are enumerated with increasing level of simulation complexity.
+
+## Contribution
+
+To contribute, please open a pull request to the `dev`-branch on [GitHub](https://www.github.com/viljarjf/QM_sim/pulls).
+
+### Linting
+
+When opening a PR, a linting check is performed.
+To ensure your contribution passes the checks, you can run the following
+
+~~~bash
+$ pip install .[linting]
+$ black src/qm_sim
+$ isort src -m 3 --trailing-comma
+$ pylint src --fail-under=7
+~~~
+
+### Setup
+
+The following is an example of how to set up VS Code for development, adapt to your IDE of choice.
+
+TL;DR: 
+- `pip install -e .` to install in an editable state
+
+**Requirements**
+- VS Code
+    - Python extension
+- Python 3.10 or above
+
+**Steps**
+1. Clone the repo recursively and open the repo in VS Code. If not cloned recursively, initialize the submodules with `git submodule update --init`
+2. Press f1, and run `Python: Create Environment`. Select `.venv`
+3. Open a new terminal, which should automatically use the virtual environment. If not, run `.venv\Scripts\activate` on Windows, or `source .venv/bin/activate` on Unix
+4. In the same terminal, run `pip install -e .[test]` to install the current directory in an editable state, and the testing utility Pytest
+5. To run tests, press f1 and run `Python: Configure Tests`. Choose `pytest`. Run tests in the testing menu
```

### Comparing `qm-sim-0.1.0/src/qm_sim/cpp/eigen/CMakeLists.txt` & `qm-sim-0.1.1/src/qm_sim/cpp/eigen/CMakeLists.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-cmake_minimum_required(VERSION 3.16.3)
-
-find_package(Python3 REQUIRED)
-
-# Sourcefiles for the library
-add_library(eigen STATIC 
-    src/HamiltonianBase.cpp
-    src/eigensolver.cpp
-    )
-
-# Include directories for the library, also add external libraries
-target_include_directories(eigen 
-    PUBLIC include
-    PUBLIC ${PROJECT_SOURCE_DIR}/lib/eigen
-    PUBLIC ${PROJECT_SOURCE_DIR}/lib/spectra/include
-    )
-
-# Necessary for parallelization
-set_property(TARGET eigen PROPERTY CXX_STANDARD 20)
-
-add_custom_command( # Generate __init__.py file
-    TARGET eigen
-    COMMAND ${Python3_EXECUTABLE} scripts/generate_init.py eigen_wrapper
-    WORKING_DIRECTORY ${CMAKE_CURRENT_LIST_DIR}
-)
-
+cmake_minimum_required(VERSION 3.16.3)
+
+find_package(Python3 REQUIRED)
+
+# Sourcefiles for the library
+add_library(eigen STATIC 
+    src/HamiltonianBase.cpp
+    src/eigensolver.cpp
+    )
+
+# Include directories for the library, also add external libraries
+target_include_directories(eigen 
+    PUBLIC include
+    PUBLIC ${PROJECT_SOURCE_DIR}/lib/eigen
+    PUBLIC ${PROJECT_SOURCE_DIR}/lib/spectra/include
+    )
+
+# Necessary for parallelization
+set_property(TARGET eigen PROPERTY CXX_STANDARD 20)
+
+add_custom_command( # Generate __init__.py file
+    TARGET eigen
+    COMMAND ${Python3_EXECUTABLE} scripts/generate_init.py eigen_wrapper
+    WORKING_DIRECTORY ${CMAKE_CURRENT_LIST_DIR}
+)
+
 add_subdirectory(wrapper)
```

### Comparing `qm-sim-0.1.0/src/qm_sim/cpp/eigen/include/HamiltonianBase.hpp` & `qm-sim-0.1.1/src/qm_sim/cpp/eigen/include/HamiltonianBase.hpp`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-#include <vector>
-#include <Eigen/Core>
-
-class HamiltonianBase
-{
-    std::vector<int> N;
-    std::vector<double> L;
-    int ndim;
-
-    double m;
-
-    std::vector<double> stencil;
-
-    std::vector<double> V;
-
-    // -hbar^2 / 2m dx^2 for each dimension, in reduced units
-    std::vector<double> h0;
-
-    // Vector from 0 to n where i_vec[i] = i
-    std::vector<int> i_vec;
-
-    template <typename arr_in, typename arr_out>
-    void matrix_multiply(arr_in &x_in, arr_out &y_out) const;
-
-public:
-    using Scalar = double;  // A typedef named "Scalar" is required
-
-    /**
-     * @brief Construct a new Hamiltonian Base object
-     * 
-     * @param N discretisation count for each dimension
-     * @param L System size in each dimension, units of nanometer
-     * @param stencil Laplacian discretisation scheme
-     * @param m particle mass, units of electron mass
-     */
-    HamiltonianBase(std::vector<int> N, std::vector<double> L, std::vector<double> stencil, double m = 1.0);
-
-    const int rows() const {
-        int out = 1;
-        for (int i = 0; i < this->ndim; i++){
-            out *= this->N[i];
-        }
-        return out;
-    };
-    const int cols() const { return this->rows(); };
-
-    // Set the potential of the system.
-    // units eV
-    void set_potential(std::vector<double> V){this->V = V;};
-    
-    void perform_op(const double *x_in, double *y_out) const;
-
-    Eigen::VectorXd as_operator(Eigen::VectorXd x_in);
-};
+#include <vector>
+#include <Eigen/Core>
+
+class HamiltonianBase
+{
+    std::vector<int> N;
+    std::vector<double> L;
+    int ndim;
+
+    double m;
+
+    std::vector<double> stencil;
+
+    std::vector<double> V;
+
+    // -hbar^2 / 2m dx^2 for each dimension, in reduced units
+    std::vector<double> h0;
+
+    // Vector from 0 to n where i_vec[i] = i
+    std::vector<int> i_vec;
+
+    template <typename arr_in, typename arr_out>
+    void matrix_multiply(arr_in &x_in, arr_out &y_out) const;
+
+public:
+    using Scalar = double;  // A typedef named "Scalar" is required
+
+    /**
+     * @brief Construct a new Hamiltonian Base object
+     * 
+     * @param N discretisation count for each dimension
+     * @param L System size in each dimension, units of nanometer
+     * @param stencil Laplacian discretisation scheme
+     * @param m particle mass, units of electron mass
+     */
+    HamiltonianBase(std::vector<int> N, std::vector<double> L, std::vector<double> stencil, double m = 1.0);
+
+    const int rows() const {
+        int out = 1;
+        for (int i = 0; i < this->ndim; i++){
+            out *= this->N[i];
+        }
+        return out;
+    };
+    const int cols() const { return this->rows(); };
+
+    // Set the potential of the system.
+    // units eV
+    void set_potential(std::vector<double> V){this->V = V;};
+    
+    void perform_op(const double *x_in, double *y_out) const;
+
+    Eigen::VectorXd as_operator(Eigen::VectorXd x_in);
+};
```

### Comparing `qm-sim-0.1.0/src/qm_sim/cpp/eigen/src/HamiltonianBase.cpp` & `qm-sim-0.1.1/src/qm_sim/cpp/eigen/src/HamiltonianBase.cpp`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-#include "HamiltonianBase.hpp"
-#include <iostream>
-#include <execution>
-
-
-HamiltonianBase::HamiltonianBase(std::vector<int> N, std::vector<double> L, std::vector<double> stencil, double m) : 
-N{N}, L{L}, stencil{stencil}, m{m} {
-    this->ndim = L.size();
-    for (int i = 0; i < this->rows(); i++){
-        this->V.push_back(0.0);
-    }
-    double dx;
-    for(int dim = 0; dim < ndim; dim++){
-        dx = this->L[dim] / this->N[dim];
-        // - hbar^2 / 2m dx^2 in units of electron mass, eV, and nm, 
-        // according to wolfram alpha
-        this->h0.push_back(
-            -0.0380998212 / (this->m * dx * dx)
-        );
-    }
-    for(int i = 0; i < this->rows(); i++){this->i_vec.push_back(i);}
-
-}
-
-template <typename arr_in, typename arr_out>
-void HamiltonianBase::matrix_multiply( arr_in &x_in, arr_out &y_out) const {
-    int n = this->rows();
-    for (int i = 0; i < n; i++){
-        y_out[i] = this->V[i] * x_in[i];
-    }
-
-    double h0_dim;
-    int offset = 1;
-    for (int dim = 0; dim < this->ndim; dim++){
-
-        // 1 / dx^2
-        h0_dim = this->h0[dim];
-
-        auto stencil = this->stencil;
-        // y_i = x_i (*) stencil
-        // stencil usually has more terms, so it can be e.g.
-        // y_i = stencil[1]*x_i-1 + stencil[0]*x_i + stencil[1]*x_i+1
-        std::for_each(
-            std::execution::par,
-            std::begin(this->i_vec),
-            std::end(this->i_vec),
-            [=,  &y_out](int i)
-            {
-            double stencil_sum, stencil_el;
-            stencil_sum = x_in[i] * stencil[0];
-            for (int j = 1; j < stencil.size(); j++){
-                stencil_el = stencil[j];
-                // account for current dimension
-                j *= offset;
-                // range-check the x-vector
-                if ((i + j) < n){
-                    stencil_sum += x_in[i + j] * stencil_el;
-                }
-                if ((i - j) >= 0){
-                    stencil_sum += x_in[i - j] * stencil_el;
-                }
-            }
-            y_out[i] += h0_dim * stencil_sum;
-        }); // end of parfor
-        offset *= this->N[dim];
-    }
-}
-
-void HamiltonianBase::perform_op(const double *x_in, double *y_out) const {
-    this->matrix_multiply<const double *, double *>(x_in, y_out);
-}
-
-Eigen::VectorXd HamiltonianBase::as_operator(Eigen::VectorXd x_in){
-    Eigen::VectorXd y_out {x_in.size()};
-    this->matrix_multiply(x_in, y_out);
-    return y_out;
-}
+#include "HamiltonianBase.hpp"
+#include <iostream>
+#include <execution>
+
+
+HamiltonianBase::HamiltonianBase(std::vector<int> N, std::vector<double> L, std::vector<double> stencil, double m) : 
+N{N}, L{L}, stencil{stencil}, m{m} {
+    this->ndim = L.size();
+    for (int i = 0; i < this->rows(); i++){
+        this->V.push_back(0.0);
+    }
+    double dx;
+    for(int dim = 0; dim < ndim; dim++){
+        dx = this->L[dim] / this->N[dim];
+        // - hbar^2 / 2m dx^2 in units of electron mass, eV, and nm, 
+        // according to wolfram alpha
+        this->h0.push_back(
+            -0.0380998212 / (this->m * dx * dx)
+        );
+    }
+    for(int i = 0; i < this->rows(); i++){this->i_vec.push_back(i);}
+
+}
+
+template <typename arr_in, typename arr_out>
+void HamiltonianBase::matrix_multiply( arr_in &x_in, arr_out &y_out) const {
+    int n = this->rows();
+    for (int i = 0; i < n; i++){
+        y_out[i] = this->V[i] * x_in[i];
+    }
+
+    double h0_dim;
+    int offset = 1;
+    for (int dim = 0; dim < this->ndim; dim++){
+
+        // 1 / dx^2
+        h0_dim = this->h0[dim];
+
+        auto stencil = this->stencil;
+        // y_i = x_i (*) stencil
+        // stencil usually has more terms, so it can be e.g.
+        // y_i = stencil[1]*x_i-1 + stencil[0]*x_i + stencil[1]*x_i+1
+        std::for_each(
+            std::execution::par,
+            std::begin(this->i_vec),
+            std::end(this->i_vec),
+            [=,  &y_out](int i)
+            {
+            double stencil_sum, stencil_el;
+            stencil_sum = x_in[i] * stencil[0];
+            for (int j = 1; j < stencil.size(); j++){
+                stencil_el = stencil[j];
+                // account for current dimension
+                j *= offset;
+                // range-check the x-vector
+                if ((i + j) < n){
+                    stencil_sum += x_in[i + j] * stencil_el;
+                }
+                if ((i - j) >= 0){
+                    stencil_sum += x_in[i - j] * stencil_el;
+                }
+            }
+            y_out[i] += h0_dim * stencil_sum;
+        }); // end of parfor
+        offset *= this->N[dim];
+    }
+}
+
+void HamiltonianBase::perform_op(const double *x_in, double *y_out) const {
+    this->matrix_multiply<const double *, double *>(x_in, y_out);
+}
+
+Eigen::VectorXd HamiltonianBase::as_operator(Eigen::VectorXd x_in){
+    Eigen::VectorXd y_out {x_in.size()};
+    this->matrix_multiply(x_in, y_out);
+    return y_out;
+}
```

### Comparing `qm-sim-0.1.0/src/qm_sim/cpp/eigen/wrapper/py_interface.cpp` & `qm-sim-0.1.1/src/qm_sim/cpp/eigen/wrapper/py_interface.cpp`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-#include "eigensolver.hpp"
-#include "HamiltonianBase.hpp"
-
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
-#include <pybind11/eigen.h>
-
-namespace py = pybind11;
-
-PYBIND11_MODULE(eigen_wrapper, m) {
-    m.doc() = "Interface to call Eigen C++ functions from python";
-
-    m.def("eigen", &eigen, "Calculate eigenvaues of the Hamiltonian", py::return_value_policy::copy);
-
-    py::class_<HamiltonianBase>(m, "Hamiltonian")
-        .def(py::init<std::vector<int>, std::vector<double>, std::vector<double>, double>())
-        .def("set_potential", &HamiltonianBase::set_potential )
-        .def("as_operator", &HamiltonianBase::as_operator);
-}
+#include "eigensolver.hpp"
+#include "HamiltonianBase.hpp"
+
+#include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
+#include <pybind11/eigen.h>
+
+namespace py = pybind11;
+
+PYBIND11_MODULE(eigen_wrapper, m) {
+    m.doc() = "Interface to call Eigen C++ functions from python";
+
+    m.def("eigen", &eigen, "Calculate eigenvaues of the Hamiltonian", py::return_value_policy::copy);
+
+    py::class_<HamiltonianBase>(m, "Hamiltonian")
+        .def(py::init<std::vector<int>, std::vector<double>, std::vector<double>, double>())
+        .def("set_potential", &HamiltonianBase::set_potential )
+        .def("as_operator", &HamiltonianBase::as_operator);
+}
```

### Comparing `qm-sim-0.1.0/src/qm_sim/eigensolvers/pytorch_eigen.py` & `qm-sim-0.1.1/src/qm_sim/eigensolvers/pytorch_eigen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-"""
-PyTorch backend for finding eigenstates
-"""
-
-import numpy as np
-import torch
-from scipy import sparse as sp
-
-PYTORCH_DEVICE = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-
-def torch_get_eigen(mat: sp.dia_matrix, n: int, shape: tuple[int], **kwargs):
-    """Calculate :code:`n` eigenvalues of :code:`mat`. Reshape output to :code:`shape`
-
-    :param mat: Matrix to calculate eigenvectors and -values for
-    :type mat: sp.dia_matrix
-    :param n: Amount of eigenvectors and -values to calculate
-    :type n: int
-    :param shape: Output shape for eigenvectors
-    :type shape: tuple[int]
-    :return: eigenvalues, eigenvectors
-    :rtype: tuple[np.ndarray(shape = (:code:`n`)), np.ndarray(shape = (:code:`n`, :code:`shape`)]
-    """
-    H = spmatrix_to_tensor(mat)
-    v, w = torch.lobpcg(H, k=n, largest=False)
-    w = w.cpu().numpy()
-    w = np.array([w[:, i].reshape(shape, order="F") for i in range(n)])
-    return v, w
-
-
-def spmatrix_to_tensor(mat: sp.spmatrix) -> torch.Tensor:
-    """
-    Convert a sparse diagonal scipy matrix to a sparse pytorch tensor.
-    """
-
-    coo = mat.tocoo()
-    values = coo.data
-    indices = np.vstack((coo.row, coo.col))
-
-    i = torch.from_numpy(indices)
-    v = torch.from_numpy(values)
-    shape = coo.shape
-
-    return torch.sparse_coo_tensor(i, v, shape, device=PYTORCH_DEVICE)
+"""
+PyTorch backend for finding eigenstates
+"""
+
+import numpy as np
+import torch
+from scipy import sparse as sp
+
+PYTORCH_DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+
+def torch_get_eigen(mat: sp.dia_matrix, n: int, shape: tuple[int], **kwargs):
+    """Calculate :code:`n` eigenvalues of :code:`mat`. Reshape output to :code:`shape`
+
+    :param mat: Matrix to calculate eigenvectors and -values for
+    :type mat: sp.dia_matrix
+    :param n: Amount of eigenvectors and -values to calculate
+    :type n: int
+    :param shape: Output shape for eigenvectors
+    :type shape: tuple[int]
+    :return: eigenvalues, eigenvectors
+    :rtype: tuple[np.ndarray(shape = (:code:`n`)), np.ndarray(shape = (:code:`n`, :code:`shape`)]
+    """
+    H = spmatrix_to_tensor(mat)
+    v, w = torch.lobpcg(H, k=n, largest=False)
+    w = w.cpu().numpy()
+    w = np.array([w[:, i].reshape(shape, order="F") for i in range(n)])
+    return v, w
+
+
+def spmatrix_to_tensor(mat: sp.spmatrix) -> torch.Tensor:
+    """
+    Convert a sparse diagonal scipy matrix to a sparse pytorch tensor.
+    """
+
+    coo = mat.tocoo()
+    values = coo.data
+    indices = np.vstack((coo.row, coo.col))
+
+    i = torch.from_numpy(indices)
+    v = torch.from_numpy(values)
+    shape = coo.shape
+
+    return torch.sparse_coo_tensor(i, v, shape, device=PYTORCH_DEVICE)
```

### Comparing `qm-sim-0.1.0/src/qm_sim/eigensolvers/scipy_eigen.py` & `qm-sim-0.1.1/src/qm_sim/eigensolvers/scipy_eigen.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,80 @@
-"""
-
-Use the scipy backend eigen solver to skip some overhead
-
-"""
-from scipy._lib._threadsafety import ReentrancyLock
-from scipy.sparse.linalg._eigen.arpack.arpack import _SymmetricArpackParams
-from scipy import sparse as sp
-from scipy.sparse.linalg import eigsh
-import numpy as np
-
-def scipy_get_eigen(mat: sp.dia_matrix, n: int, shape: tuple[int], **kwargs) -> tuple[np.ndarray, np.ndarray]:
-    """Calculate :code:`n` eigenvalues of :code:`mat`. Reshape output to :code:`shape`
-
-    :param mat: Matrix to calculate eigenvectors and -values for
-    :type mat: sp.dia_matrix
-    :param n: Amount of eigenvectors and -values to calculate
-    :type n: int
-    :param shape: Output shape for eigenvectors
-    :type shape: tuple[int]
-    :return: eigenvalues, eigenvectors
-    :rtype: tuple[np.ndarray(shape = (:code:`n`)), np.ndarray(shape = (:code:`n`, :code:`shape`)]
-    """
-    if kwargs.get("sigma") is None:
-        v, w = _eigsh(mat._mul_vector, mat.shape[0], 
-            mat.dtype, k=n, **kwargs)
-    else:
-        # Fallback to default solver
-        v, w = eigsh(mat, k=n, which="SA", **kwargs)
-
-    # Reshape into system shape.
-    # Arrays returned from eigsh are fortran ordered
-    w = np.array([w[:, i].reshape(shape, order="F") for i in range(n)])
-    return v, w
-
-
-def _eigsh(A_OP, n, dtype, k=6, sigma=None, which='SA', v0=None,
-          ncv=None, maxiter=None, tol=0, return_eigenvectors=True,
-          ):
-    """Copied from the scipy sourcecode, removing some overhead.
-    See https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.linalg.eigsh.html
-    """
-    mode = 1
-    M_matvec = None
-    Minv_matvec = None
-    params = _SymmetricArpackParams(n, k, dtype.char, A_OP, mode,
-                                    M_matvec, Minv_matvec, sigma,
-                                    ncv, v0, maxiter, which, tol)
-
-    with ReentrancyLock("Nested calls to eigs/eighs not allowed: "
-        "ARPACK is not re-entrant"):
-        while not params.converged:
-            params.iterate()
-
-        return params.extract(return_eigenvectors)    
+"""
+
+Use the scipy backend eigen solver to skip some overhead
+
+"""
+import numpy as np
+from scipy import sparse as sp
+from scipy._lib._threadsafety import ReentrancyLock
+from scipy.sparse.linalg import eigsh
+from scipy.sparse.linalg._eigen.arpack.arpack import _SymmetricArpackParams
+
+
+def scipy_get_eigen(
+    mat: sp.dia_matrix, n: int, shape: tuple[int], **kwargs
+) -> tuple[np.ndarray, np.ndarray]:
+    """Calculate :code:`n` eigenvalues of :code:`mat`. Reshape output to :code:`shape`
+
+    :param mat: Matrix to calculate eigenvectors and -values for
+    :type mat: sp.dia_matrix
+    :param n: Amount of eigenvectors and -values to calculate
+    :type n: int
+    :param shape: Output shape for eigenvectors
+    :type shape: tuple[int]
+    :return: eigenvalues, eigenvectors
+    :rtype: tuple[np.ndarray(shape = (:code:`n`)), np.ndarray(shape = (:code:`n`, :code:`shape`)]
+    """
+    if kwargs.get("sigma") is None:
+        v, w = _eigsh(mat._mul_vector, mat.shape[0], mat.dtype, k=n, **kwargs)
+    else:
+        # Fallback to default solver
+        v, w = eigsh(mat, k=n, which="SA", **kwargs)
+
+    # Reshape into system shape.
+    # Arrays returned from eigsh are fortran ordered
+    w = np.array([w[:, i].reshape(shape, order="F") for i in range(n)])
+    return v, w
+
+
+def _eigsh(
+    A_OP,
+    n,
+    dtype,
+    k=6,
+    sigma=None,
+    which="SA",
+    v0=None,
+    ncv=None,
+    maxiter=None,
+    tol=0,
+    return_eigenvectors=True,
+):
+    """Copied from the scipy sourcecode, removing some overhead.
+    See https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.linalg.eigsh.html
+    """
+    mode = 1
+    M_matvec = None
+    Minv_matvec = None
+    params = _SymmetricArpackParams(
+        n,
+        k,
+        dtype.char,
+        A_OP,
+        mode,
+        M_matvec,
+        Minv_matvec,
+        sigma,
+        ncv,
+        v0,
+        maxiter,
+        which,
+        tol,
+    )
+
+    with ReentrancyLock(
+        "Nested calls to eigs/eighs not allowed: ARPACK is not re-entrant"
+    ):
+        while not params.converged:
+            params.iterate()
+
+        return params.extract(return_eigenvectors)
```

### Comparing `qm-sim-0.1.0/src/qm_sim/hamiltonian/spatial_hamiltonian.py` & `qm-sim-0.1.1/src/qm_sim/hamiltonian/spatial_hamiltonian.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,391 +1,429 @@
-"""
-
-Real-space discretized Hamiltonian class, with solving and plotting functionality
-
-"""
-
-from typing import Callable, Any
-
-import numpy as np
-from scipy.sparse import dia_matrix
-from tqdm import tqdm
-
-from ..nature_constants import h_bar
-from .. import plot
-from ..spatial_derivative import get_scheme_order
-from ..spatial_derivative.cartesian import nabla, laplacian
-from ..temporal_solver import TemporalSolver, get_temporal_solver
-from ..eigensolvers import get_eigensolver
-from scipy.sparse.linalg import eigsh as adiabatic_eigsh
-
-
-class SpatialHamiltonian:
-
-    def __init__(self, N: tuple, L: tuple, m: float | np.ndarray, 
-        spatial_scheme: str = "three-point", temporal_scheme: str = "leapfrog",
-        eigensolver: str = "scipy", verbose: bool = True, boundary_condition: str = "zero"):
-        """Non-stationary Hamiltonian in real space.
-
-        :param N: Discretization count along each axis
-        :type N: tuple
-        :param L: System size along each axis
-        :type L: tuple
-        :param m: Mass of the particle in the system. 
-            Can be constant (float) or vary in the simulation area (array).
-            If an array is used, :code:`m.shape == N` must hold
-        :type m: float | np.ndarray
-        :param spatial_scheme: Finite difference scheme for spatial derivative. 
-            Options are: 
-            
-            - three-point
-            - five-point
-            - seven-point
-            - nine-point
-
-            Defaults to "three-point"
-        :type spatial_scheme: str, optional
-        :param temporal_scheme: Finite difference scheme for temporal derivative.
-            Options are:
-
-            - crank-nicolson
-            - leapfrog
-            - scipy-Runge-Kutta 5(4)
-            - scipy-Runge-Kutta 3(2)
-            - scipy-DOP853
-            - scipy-backwards-differentiation
-
-            Defaults to "leapfrog"
-        :type temporal_scheme: str, optional
-        :param eigensolver: Choose which eigensolver backend to use.
-            Options are:
-
-            - scipy
-            - torch (optional dependency, must be installed)
-
-            Defaults to "scipy"
-        :type eigensolver: str, optional
-        :param verbose: Option to display calculation and iteration info during runtime.
-            Defaults to True
-        :type verbose: bool, optional
-        :param boundary_condition: Which boundary condition to apply.
-            Options are:
-
-            - zero
-            - periodic
-
-            Defaults to "zero"
-        :type boundary_condition: str, optional
-        """
-       
-        if len(N) != len(L):
-            raise ValueError("`N`and `L`must have same length")
-        
-        self.N = tuple(N)
-        self.L = tuple(L)
-        self._dim = len(N)
-        self.delta = [Li / Ni for Li, Ni in zip(L, N)]
-        
-        self.eigensolver = get_eigensolver(eigensolver)
-        if self.eigensolver is None:
-            raise ValueError(f"Eigensolver {eigensolver} not found")
-
-        order = get_scheme_order(spatial_scheme)
-        if order is None:
-            raise ValueError("Requested finite difference is invalid")
-
-        # Handle non-isotropic effective mass
-        if isinstance(m, np.ndarray) and np.all(m == m.flat[0]):
-            m = m.flatten()[0]
-        if isinstance(m, np.ndarray):
-            print("Warning: Continuity is NOT satisfied (yet) with non-isotropic mass")
-            if m.shape != self.N:
-                raise ValueError(f"Inconsistent shape of `m`: {m.shape}, should be {self.N}")
-            m_inv = 1 / m.flatten()
-
-            _n = nabla(N, L, order=order, boundary_condition=boundary_condition)
-            _n2 = laplacian(N, L, order=order, boundary_condition=boundary_condition)
-
-            # nabla m_inv nabla + m_inv nabla^2
-            _n.data *= _n @ m_inv   # First term
-            _n2.data *= m_inv       # Second term
-            self.mat = _n + _n2
-        else:
-            self.mat = laplacian(N, L, order=order, boundary_condition=boundary_condition)
-            self.mat *= 1/m
-        
-        self._centerline_index = list(self.mat.offsets).index(0)
-        self._default_data = None
-
-        # Prefactor in hamiltonian.
-        # Is either float or array, depending on `m`
-        h0 = -h_bar**2 / 2
-        
-        # Multiplying the diagonal data directly is easier
-        # if we have non-constant mass
-        self.mat.data *= h0
-
-        # static zero potential by default
-        self._V = lambda t: np.zeros(shape = N)
-
-        self.verbose = verbose
-
-        self._temporal_solver = get_temporal_solver(temporal_scheme)
-    
-    @property
-    def V(self) -> Callable[[float], np.ndarray]:
-        """Potential as a function of time
-
-        :return: input time, output potential. Output must have same shape as systme
-        :rtype: Callable[[float], np.ndarray]
-        """
-        return self._V
-
-    @V.setter
-    def V(self, V: np.ndarray | Callable[[float], np.ndarray]):
-        """Set a (potentially time dependent) potential for the QM-system's Hamiltonian
-
-        :param V: The energetic value of the potential at a given point associated with given array indices,
-                if callable, the call variable will represent a changable parameter (usually time) with a 
-                return type identical to the static case where V is an np.ndarray
-        :type V: np.ndarray | Callable[[float], np.ndarray]
-        """
-        if not callable(V):
-            # Avoid the lambda func referring to itself
-            array_V = V
-            V = lambda t: array_V
-        
-        if V(0).shape != self.shape:
-            raise ValueError(f"Inconsistent shape. Shape must be {self.shape}")
-
-        self._V = V
-
-    def eigen(self, n: int, t: float = 0, **kwargs) -> tuple[np.ndarray, np.ndarray]:
-        """Calculate the n smallest eigenenergies and the corresponding eigenstates of the hamiltonian
-
-        :param n: Amount of eigenenergies/states to output
-        :type n: int
-        :param t: If the potential is time-dependent, solves the Time-independent Schrödinger eq. as if it was frozen at time t.
-            Does nothing if potential is time-independent.
-            Defaults to 0
-        :type t: float, optional
-        :return: 
-            - Eigenenergies
-            - Normalised eigenstates
-
-        :rtype: tuple[np.ndarray(shape = (n)), np.ndarray(shape = (n, N))]
-        """
-
-        # The adiabatic solver uses some features of the eigensolver
-        # not exposed by the `self.eigensolver` function
-        if kwargs.pop("is_adiabatic", False):
-            E, psi = adiabatic_eigsh(self(t), k=n, **kwargs)
-            psi = np.array([psi[:, i].reshape(self.N, order="F") for i in range(n)])
-        else:
-            E, psi = self.eigensolver(self(t), n, self.N)
-
-        # calculate normalisation factor
-        nf = [psi[i, :]**2 for i in range(n)]
-        for i, (L, N) in enumerate(zip(self.L, self.N)):
-            dx = L / N
-            for j in range(n):
-                nf[j] = np.trapz(nf[j], dx=dx)
-        # normalise
-        for i in range(n):
-            psi[i] /= nf[i]**0.5
-        return E, psi
-
-
-    def adiabatic_evolution(self, E_n: float, t0: float, dt : float, steps: int) -> tuple[np.ndarray, np.ndarray]:
-        """Adiabatically evolve an eigenstate with a slowly varying time-dependent potential with
-        energy (close to) E_n using the Adiabatic approximation. 
-        https://en.wikipedia.org/wiki/Adiabatic_theorem
-
-        Note: This is only valid given that the adiabatic theorem holds, ie. no degeneracy and a gap between 
-        eigenvalues. Current implementation assumes this holds and does not check if it does (yet?). 
-        There is no mathematical guarantee (yet?) that the iterative solver will "hug" the correct eigenvector
-        at every step, but it should be good if V varies smoothly enough and dt is small enough. 
-        
-
-        :param E_n: The Eigenvalue for you want to adiabatically evolve
-        :type E_n: float
-        :param t0: Starting time for time-evolution
-        :type t0: float
-        :param dt: The (small) time parameter increment used to update the eigenstate temporally
-        :type dt: float
-        :param steps: Number of increments.
-        :type steps: int
-        :return: (E(t), Psi(t)), Time evolution of the eigenstate.
-        :rtype: tuple[np.ndarray(shape = steps), np.ndarray(shape = (N, steps))]
-        """
-        Psi_t = np.empty(shape = (*self.N,steps+1))
-        En_t = np.empty(steps+1)
-        t = t0
-
-        # initialize
-        _, Psi_t[:, :, 0] = self.eigen(1, t, sigma=E_n, is_adiabatic=True)
-        En_t[0] = E_n
-
-        for i in tqdm(range(1, steps+1), desc="Adiabatic evolution", disable=not self.verbose):
-            t += dt
-            En_t[i], Psi_t[:,:,i] = self.eigen( 1, t,
-                # smartly condition eigsolver to "hug" the single eigenvalue solution; eigenvector and eigenvalue should be
-                # far closer to the previous one than any other if the adiabatic theorem is fulfilled
-                sigma=En_t[i-1],
-                v0=-Psi_t[:,:,i-1],
-                is_adiabatic=True
-            )
-        return En_t, Psi_t
-
-    def temporal_evolution(self, t0: float, t_final: float, dt_storage: float = None, 
-        psi_0: np.ndarray = None) -> tuple[np.ndarray, np.ndarray]:
-
-
-        # Default: superposition of 1st and 2nd eigenstate
-        if psi_0 is None:
-            _, psi = self.eigen(2)
-            psi_0 = 2**-0.5 * (psi[0] + psi[1])
-        
-        # Calculate a good dt from von Neumann analysis of the leapfrog scheme
-        # NOTE: this assumes the temporal part is at most 4x the static part,
-        #       and that the potential takes its maximum somwhere at t=t0
-        V_max = np.max(self.V(t0) * 4)
-        V_min = np.min(self.V(t0) * 4)
-
-        E_max = max(
-            abs(V_min),
-            abs(V_max + 4 * np.max(self.mat.data)),
-            )
-        dt = 0.25 * h_bar / E_max
-
-        # solve
-        f = lambda t: 1/(1j * h_bar) * self.__call__(t)
-        solver = self._temporal_solver(f, self.shape)
-        t, psi = solver.iterate(psi_0.astype(np.complex128), t0, 
-            t_final, dt, dt_storage, self.verbose)
-
-        return t, psi
-    temporal_evolution.__doc__ = TemporalSolver.iterate.__doc__
-
-
-    def plot_eigen(self, n: int, t: float = 0):
-        """Calculate and plot :code:`n` eigenstates at time :code:`t`
-
-        :param n: Amount of eigenstates to plot
-        :type n: int
-        :param t: Time at which to find eigenstates, defaults to 0
-        :type t: float, optional
-        """
-        E, psi = self.eigen(n, t)
-        plot.eigen(E, psi)
-
-
-    def plot_temporal(self, t_final: float, dt: float, psi_0: np.ndarray = None, t0: float = 0):
-        """Plot the temporal evolution of the eigenstates
-
-        :param t_final: Simulation end time
-        :type t_final: float
-        :param dt: Simulation time between each timestep
-        :type dt: float
-        :param psi_0: Initial state, defaults to None
-        :type psi_0: np.ndarray, optional
-        :param t0: Simulation start time, defaults to 0
-        :type t0: float, optional
-        """
-        t, psi = self.temporal_evolution(t0, t_final, dt, psi_0)
-        plot.temporal(t, psi, self.V)
-
-
-    def plot_potential(self, t: float = 0):
-        """Plot the potential at a given time
-
-        :param t: Time at which to plot, defaults to 0
-        :type t: float, optional
-        """
-        plot.potential(self.V(t))
-
-    def __add__(self, other: np.ndarray) -> dia_matrix:
-        """Add a vector to the main diagonal, and return the matrix
-
-        :param other: Array to add to the main diagonal
-        :type other: np.ndarray
-        :return: Matrix data, i.e. NOT a Hamiltonian object
-        :rtype: dia_matrix
-        """
-        if self._default_data is None:
-            self._default_data = self.mat.data.copy()
-    
-        self.mat.data = self._default_data.copy()
-        self.mat.data[self._centerline_index, :] += other.flatten()
-        return self.mat
-    
-    def __call__(self, t: float) -> dia_matrix:
-        """Get the matrix at a given time
-
-        :param t: Time at which to get the matrix at
-        :type t: float
-        :return: Matrix data, i.e. NOT a Hamiltonian object
-        :rtype: dia_matrix
-        """
-        return self + self.V(t)
-    
-    @property
-    def shape(self) -> tuple[int]:
-        """System shape
-
-        :return: Tuple with discretization count along each axis
-        :rtype: tuple[int]
-        """
-        return self.N
-
-    @property
-    def N_total(self) -> int:
-        """Total amount of discretization points
-
-        :return: Discretization point count
-        :rtype: int
-        """
-        i = 1
-        for j in self.N:
-            i *= j
-        return i
-    
-    @property
-    def ndim(self) -> int:
-        """System dimensionallity
-
-        :return: Amount of dimensions in the system
-        :rtype: int
-        """
-        return len(self.N)
-
-    def __matmul__(self, other: Any) -> Any:
-        """Matrix multiplication with the underlying data
-
-        :param other: matrix to multiply with
-        :type other: Any
-        :return: Matrix product
-        :rtype: Any
-        """
-        return self.mat @ other
-    
-    def _fast_matmul_op(self, t: float = 0) -> Callable[[Any], np.ndarray]:
-        """Evaluate the Hamiltonian at a given time, 
-        and return a matrix-vector multiplication function
-
-        :param t: Time at which to evaluate the Hamiltonian, defaults to 0
-        :type t: float, optional
-        :return: Fast matrix-vector multiplication function
-        :rtype: Callable[[Any], np.ndarray]
-        """
-        mat = self(t)
-        return mat._mul_vector
-    
-    def asarray(self) -> np.ndarray:
-        """Return the data matrix as a dense array
-
-        :return: Dense array of the discretized Hamiltonian
-        :rtype: np.ndarray
-        """
-        return self.mat.toarray()
-    
-   
+"""
+
+Real-space discretized Hamiltonian class, with solving and plotting functionality
+
+"""
+
+from collections.abc import Iterable
+from typing import Any, Callable
+
+import numpy as np
+from scipy.sparse import dia_matrix
+from scipy.sparse.linalg import eigsh as adiabatic_eigsh
+from tqdm import tqdm
+
+from .. import plot
+from ..eigensolvers import get_eigensolver
+from ..nature_constants import h_bar
+from ..spatial_derivative import get_scheme_order
+from ..spatial_derivative.cartesian import laplacian, nabla
+from ..temporal_solver import TemporalSolver, get_temporal_solver
+
+
+class SpatialHamiltonian:
+    def __init__(
+        self,
+        N: tuple[int] | int,
+        L: tuple[float] | float,
+        m: float | np.ndarray,
+        spatial_scheme: str = "three-point",
+        temporal_scheme: str = "leapfrog",
+        eigensolver: str = "scipy",
+        verbose: bool = True,
+        boundary_condition: str = "zero",
+    ):
+        """Non-stationary Hamiltonian in real space.
+
+        :param N: Discretization count along each axis
+        :type N: tuple[int] | int
+        :param L: System size along each axis
+        :type L: tuple[float] | float
+        :param m: Mass of the particle in the system.
+            Can be constant (float) or vary in the simulation area (array).
+            If an array is used, :code:`m.shape == N` must hold
+        :type m: float | np.ndarray
+        :param spatial_scheme: Finite difference scheme for spatial derivative.
+            Options are:
+
+            - three-point
+            - five-point
+            - seven-point
+            - nine-point
+
+            Defaults to "three-point"
+        :type spatial_scheme: str, optional
+        :param temporal_scheme: Finite difference scheme for temporal derivative.
+            Options are:
+
+            - crank-nicolson
+            - leapfrog
+            - scipy-Runge-Kutta 5(4)
+            - scipy-Runge-Kutta 3(2)
+            - scipy-DOP853
+            - scipy-backwards-differentiation
+
+            Defaults to "leapfrog"
+        :type temporal_scheme: str, optional
+        :param eigensolver: Choose which eigensolver backend to use.
+            Options are:
+
+            - scipy
+            - torch (optional dependency, must be installed)
+
+            Defaults to "scipy"
+        :type eigensolver: str, optional
+        :param verbose: Option to display calculation and iteration info during runtime.
+            Defaults to True
+        :type verbose: bool, optional
+        :param boundary_condition: Which boundary condition to apply.
+            Options are:
+
+            - zero
+            - periodic
+
+            Defaults to "zero"
+        :type boundary_condition: str, optional
+        """
+        # 1D inputs
+        if isinstance(N, int):
+            N = (N,)
+        if isinstance(L, (float, int)):
+            L = (L,)
+
+        # Allow any iterable that can be converted to a tuple
+        if isinstance(N, Iterable):
+            N = tuple(N)
+        if isinstance(L, Iterable):
+            L = tuple(L)
+
+        # Check type
+        if not isinstance(N, tuple) or not all(isinstance(i, int) for i in N):
+            raise ValueError(f"Param `N` must be int or tuple of ints, got {type(N)}")
+        if not isinstance(L, tuple) or not all(isinstance(i, (float, int)) for i in L):
+            raise ValueError(f"Param `L` must be float or tuple, got {type(L)}")
+
+        if len(N) != len(L):
+            raise ValueError("`N`and `L`must have same length")
+
+        self.N = N
+        self.L = L
+
+        self.eigensolver = get_eigensolver(eigensolver)
+        if self.eigensolver is None:
+            raise ValueError(f"Eigensolver {eigensolver} not found")
+
+        order = get_scheme_order(spatial_scheme)
+        if order is None:
+            raise ValueError("Requested finite difference is invalid")
+
+        self._dim = len(N)
+        self.delta = [Li / Ni for Li, Ni in zip(L, N)]
+
+        # Handle non-isotropic effective mass
+        if isinstance(m, np.ndarray) and np.all(m == m.flat[0]):
+            m = m.flatten()[0]
+        if isinstance(m, np.ndarray):
+            print("Warning: Continuity is NOT satisfied (yet) with non-isotropic mass")
+            if m.shape != self.N:
+                raise ValueError(
+                    f"Inconsistent shape of `m`: {m.shape}, should be {self.N}"
+                )
+            m_inv = 1 / m.flatten()
+
+            _n = nabla(N, L, order=order, boundary_condition=boundary_condition)
+            _n2 = laplacian(N, L, order=order, boundary_condition=boundary_condition)
+
+            # nabla m_inv nabla + m_inv nabla^2
+            _n.data *= _n @ m_inv  # First term
+            _n2.data *= m_inv  # Second term
+            self.mat = _n + _n2
+        else:
+            self.mat = laplacian(
+                N, L, order=order, boundary_condition=boundary_condition
+            )
+            self.mat *= 1 / m
+
+        self._centerline_index = list(self.mat.offsets).index(0)
+        self._default_data = None
+
+        # Multiply the laplacian with the remaining factors
+        self.mat.data *= -(h_bar**2) / 2
+
+        # static zero potential by default
+        self._V = lambda t: np.zeros(shape=N)
+
+        self.verbose = verbose
+
+        self._temporal_solver = get_temporal_solver(temporal_scheme)
+
+    @property
+    def V(self) -> Callable[[float], np.ndarray]:
+        """Potential as a function of time
+
+        :return: input time, output potential. Output must have same shape as systme
+        :rtype: Callable[[float], np.ndarray]
+        """
+        return self._V
+
+    @V.setter
+    def V(self, V: np.ndarray | Callable[[float], np.ndarray]):
+        """Set a (potentially time dependent) potential for the QM-system's Hamiltonian
+
+        :param V: The energetic value of the potential at a given point associated with
+            given array indices,
+            if callable, the call variable will represent a changable parameter
+            (usually time) with a return type identical to the static case where V is an np.ndarray
+        :type V: np.ndarray | Callable[[float], np.ndarray]
+        """
+        if not callable(V):
+            # Avoid the lambda func referring to itself
+            array_V = V
+            V = lambda t: array_V
+
+        if V(0).shape != self.shape:
+            raise ValueError(f"Inconsistent shape. Shape must be {self.shape}")
+
+        self._V = V
+
+    def eigen(self, n: int, t: float = 0, **kwargs) -> tuple[np.ndarray, np.ndarray]:
+        """Calculate the n smallest eigenenergies and the corresponding eigenstates of
+        the hamiltonian
+
+        :param n: Amount of eigenenergies/states to output
+        :type n: int
+        :param t: If the potential is time-dependent, solves the Time-independent
+            Schrödinger eq. as if it was frozen at time t.
+            Does nothing if potential is time-independent.
+            Defaults to 0
+        :type t: float, optional
+        :return:
+            - Eigenenergies
+            - Normalised eigenstates
+
+        :rtype: tuple[np.ndarray(shape = (n)), np.ndarray(shape = (n, N))]
+        """
+
+        # The adiabatic solver uses some features of the eigensolver
+        # not exposed by the `self.eigensolver` function
+        if kwargs.pop("is_adiabatic", False):
+            E, psi = adiabatic_eigsh(self(t), k=n, **kwargs)
+            psi = np.array([psi[:, i].reshape(self.N, order="F") for i in range(n)])
+        else:
+            E, psi = self.eigensolver(self(t), n, self.N)
+
+        # calculate normalisation factor
+        normalisation_factor = [psi[i, :] ** 2 for i in range(n)]
+        for i, (L, N) in enumerate(zip(self.L, self.N)):
+            dx = L / N
+            for j in range(n):
+                normalisation_factor[j] = np.trapz(normalisation_factor[j], dx=dx)
+        # normalise
+        for i in range(n):
+            psi[i] /= normalisation_factor[i] ** 0.5
+        return E, psi
+
+    def adiabatic_evolution(
+        self, E_n: float, t0: float, dt: float, steps: int
+    ) -> tuple[np.ndarray, np.ndarray]:
+        """Adiabatically evolve an eigenstate with a slowly varying time-dependent potential with
+        energy (close to) :code:`E_n` using the Adiabatic approximation.
+        https://en.wikipedia.org/wiki/Adiabatic_theorem
+
+        Note: This is only valid given that the adiabatic theorem holds, ie. no degeneracy and a
+        gap betweeneigenvalues. Current implementation assumes this holds and does not check if
+        it does (yet?).
+        There is no mathematical guarantee (yet?) that the iterative solver will "hug" the
+        correct eigenvector at every step, but it should be good if V varies smoothly enough and
+        :code:`dt` is small enough.
+
+
+        :param E_n: The Eigenvalue for you want to adiabatically evolve
+        :type E_n: float
+        :param t0: Starting time for time-evolution
+        :type t0: float
+        :param dt: The (small) time parameter increment used to update the eigenstate temporally
+        :type dt: float
+        :param steps: Number of increments.
+        :type steps: int
+        :return: (E(t), Psi(t)), Time evolution of the eigenstate.
+        :rtype: tuple[np.ndarray(shape = steps), np.ndarray(shape = (N, steps))]
+        """
+        Psi_t = np.empty(shape=(*self.N, steps + 1))
+        En_t = np.empty(steps + 1)
+        t = t0
+
+        # initialize
+        _, Psi_t[:, :, 0] = self.eigen(1, t, sigma=E_n, is_adiabatic=True)
+        En_t[0] = E_n
+
+        for i in tqdm(
+            range(1, steps + 1), desc="Adiabatic evolution", disable=not self.verbose
+        ):
+            t += dt
+            En_t[i], Psi_t[:, :, i] = self.eigen(
+                1,
+                t,
+                # smartly condition eigsolver to "hug" the single eigenvalue solution;
+                # eigenvector and eigenvalue should be far closer to the previous one
+                # than any other if the adiabatic theorem is fulfilled
+                sigma=En_t[i - 1],
+                v0=-Psi_t[:, :, i - 1],
+                is_adiabatic=True,
+            )
+        return En_t, Psi_t
+
+    def temporal_evolution(
+        self,
+        t0: float,
+        t_final: float,
+        dt_storage: float = None,
+        psi_0: np.ndarray = None,
+    ) -> tuple[np.ndarray, np.ndarray]:
+        # Default: superposition of 1st and 2nd eigenstate
+        if psi_0 is None:
+            _, psi = self.eigen(2)
+            psi_0 = 2**-0.5 * (psi[0] + psi[1])
+
+        # Calculate a good dt from von Neumann analysis of the leapfrog scheme
+        # NOTE: this assumes the temporal part is at most 4x the static part,
+        #       and that the potential takes its maximum somwhere at t=t0
+        V_max = np.max(self.V(t0) * 4)
+        V_min = np.min(self.V(t0) * 4)
+
+        E_max = max(
+            abs(V_min),
+            abs(V_max + 4 * np.max(self.mat.data)),
+        )
+        dt = 0.25 * h_bar / E_max
+
+        # solve
+        func = lambda t: 1 / (1j * h_bar) * self.__call__(t)
+        solver = self._temporal_solver(func, self.shape)
+        t, psi = solver.iterate(
+            psi_0.astype(np.complex128), t0, t_final, dt, dt_storage, self.verbose
+        )
+
+        return t, psi
+
+    temporal_evolution.__doc__ = TemporalSolver.iterate.__doc__
+
+    def plot_eigen(self, n: int, t: float = 0):
+        """Calculate and plot :code:`n` eigenstates at time :code:`t`
+
+        :param n: Amount of eigenstates to plot
+        :type n: int
+        :param t: Time at which to find eigenstates, defaults to 0
+        :type t: float, optional
+        """
+        E, psi = self.eigen(n, t)
+        plot.eigen(E, psi)
+
+    def plot_temporal(
+        self, t_final: float, dt: float, psi_0: np.ndarray = None, t0: float = 0
+    ):
+        """Plot the temporal evolution of the eigenstates
+
+        :param t_final: Simulation end time
+        :type t_final: float
+        :param dt: Simulation time between each timestep
+        :type dt: float
+        :param psi_0: Initial state, defaults to None
+        :type psi_0: np.ndarray, optional
+        :param t0: Simulation start time, defaults to 0
+        :type t0: float, optional
+        """
+        t, psi = self.temporal_evolution(t0, t_final, dt, psi_0)
+        plot.temporal(t, psi, self.V)
+
+    def plot_potential(self, t: float = 0):
+        """Plot the potential at a given time
+
+        :param t: Time at which to plot, defaults to 0
+        :type t: float, optional
+        """
+        plot.potential(self.V(t))
+
+    def __add__(self, other: np.ndarray) -> dia_matrix:
+        """Add a vector to the main diagonal, and return the matrix
+
+        :param other: Array to add to the main diagonal
+        :type other: np.ndarray
+        :return: Matrix data, i.e. NOT a Hamiltonian object
+        :rtype: dia_matrix
+        """
+        if self._default_data is None:
+            self._default_data = self.mat.data.copy()
+
+        self.mat.data = self._default_data.copy()
+        self.mat.data[self._centerline_index, :] += other.flatten()
+        return self.mat
+
+    def __call__(self, t: float) -> dia_matrix:
+        """Get the matrix at a given time
+
+        :param t: Time at which to get the matrix at
+        :type t: float
+        :return: Matrix data, i.e. NOT a Hamiltonian object
+        :rtype: dia_matrix
+        """
+        return self + self.V(t)
+
+    @property
+    def shape(self) -> tuple[int]:
+        """System shape
+
+        :return: Tuple with discretization count along each axis
+        :rtype: tuple[int]
+        """
+        return self.N
+
+    @property
+    def N_total(self) -> int:
+        """Total amount of discretization points
+
+        :return: Discretization point count
+        :rtype: int
+        """
+        i = 1
+        for j in self.N:
+            i *= j
+        return i
+
+    @property
+    def ndim(self) -> int:
+        """System dimensionallity
+
+        :return: Amount of dimensions in the system
+        :rtype: int
+        """
+        return len(self.N)
+
+    def __matmul__(self, other: Any) -> Any:
+        """Matrix multiplication with the underlying data
+
+        :param other: matrix to multiply with
+        :type other: Any
+        :return: Matrix product
+        :rtype: Any
+        """
+        return self.mat @ other
+
+    def _fast_matmul_op(self, t: float = 0) -> Callable[[Any], np.ndarray]:
+        """Evaluate the Hamiltonian at a given time,
+        and return a matrix-vector multiplication function
+
+        :param t: Time at which to evaluate the Hamiltonian, defaults to 0
+        :type t: float, optional
+        :return: Fast matrix-vector multiplication function
+        :rtype: Callable[[Any], np.ndarray]
+        """
+        mat = self(t)
+        return mat._mul_vector
+
+    def asarray(self) -> np.ndarray:
+        """Return the data matrix as a dense array
+
+        :return: Dense array of the discretized Hamiltonian
+        :rtype: np.ndarray
+        """
+        return self.mat.toarray()
```

### Comparing `qm-sim-0.1.0/src/qm_sim/spatial_derivative/cartesian.py` & `qm-sim-0.1.1/src/qm_sim/spatial_derivative/cartesian.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,207 +1,228 @@
-
-import numpy as np
-from scipy import sparse as sp
-
-
-def nabla(N: tuple[int], L: tuple[float], order: int = 2, dtype: type = np.float64, 
-          boundary_condition: str = "zero") -> sp.dia_matrix:
-    """Finite difference derivative in cartesian coordinates.
-    Uses central stencil.
-
-    Example: approximate the derivative of sin(x).
-
-    >>> from qm_sim.spatial_derivative.cartesian import nabla
-    >>> import numpy as np
-    >>> N = (1000,)
-    >>> L = (2*np.pi,)
-    >>> n = nabla( N, L, boundary_condition="periodic")
-    >>> x = np.linspace( 0, L[0], N[0], endpoint=False )
-    >>> y = np.sin(x)
-    >>> np.allclose(n @ y, np.cos(x)) # The analytical solution is cos(x)
-    True
-
-    :param N: Discretization count along each axis
-    :type N: tuple[int]
-    :param L: System size along each axis
-    :type L: tuple[float]
-    :param order: Numerical order of the differentiation scheme.
-        Options are:
-
-            - 2
-            - 4
-            - 6
-            - 8
-
-        Defaults to 2.
-    :type order: int, optional
-    :param dtype: datatype of matrix. 
-        Defaults to np.float64
-    :type dtype: type, optional
-    :raises NotImplementedError: if requested order is not available
-    :return: Discretized derivative matrix
-    :rtype: sp.dia_matrix
-    :param boundary_condition: Which boundary condition to apply.
-            Options are:
-
-            - zero
-            - periodic
-
-            Defaults to "zero"
-    :type boundary_condition: str, optional
-    """
-    # Lookup for first half of stencil. 
-    # A 0 is appended for the central element, 
-    # and the rest is mirrored with a sign change later
-    match order:
-        case 2:
-            stencil = [-1/2]
-        case 4:
-            stencil = [1/12, -2/3]
-        case 6:
-            stencil = [-1/60, 3/20, -3/4]
-        case 8:
-            stencil = [1/280, -4/105, 1/5, -4/5]
-        case _:
-            raise NotImplementedError(f"Finite difference scheme not found for {order = }")
-    stencil += [0]
-
-    stencil = _mirror_sign_list(stencil)
-    return _matrix_from_central_stencil(stencil, 1, N, L, dtype, boundary_condition)
-
-
-def laplacian(N: tuple[int], L: tuple[float], order: int = 2, dtype: type = np.float64, 
-              boundary_condition: str = "zero") -> sp.dia_matrix:
-    """Finite difference double derivative in cartesian coordinates.
-    Uses central stencil
-
-    Example: approximate the second derivative of sin(x).
-
-    >>> from qm_sim.spatial_derivative.cartesian import laplacian
-    >>> import numpy as np
-    >>> N = (1000,)
-    >>> L = (2*np.pi,)
-    >>> n = laplacian( N, L, boundary_condition="periodic" )
-    >>> x = np.linspace( 0, L[0], N[0], endpoint=False)
-    >>> y = np.sin(x)
-    >>> np.allclose(n @ y, -np.sin(x)) # The analytical solution is -sin(x)
-    True
-
-    :param N: Discretization count along each axis
-    :type N: tuple[int]
-    :param L: System size along each axis
-    :type L: tuple[float]
-    :param order: Numerical order of the differentiation scheme.
-        Options are:
-
-            - 2
-            - 4
-            - 6
-            - 8
-
-        Defaults to 2.
-    :type order: int, optional
-    :param dtype: datatype of matrix. 
-        Defaults to np.float64
-    :type dtype: type, optional
-    :raises NotImplementedError: if requested order is not available
-    :return: Discretized derivative matrix
-    :rtype: sp.dia_matrix
-    :param boundary_condition: Which boundary condition to apply.
-            Options are:
-
-            - zero
-            - periodic
-
-            Defaults to "zero"
-    :type boundary_condition: str, optional
-    """
-    # lookup the first half of the stencil, to be mirrored later
-    match order:
-        case 2:
-            stencil = [1, -2]
-        case 4:
-            stencil = [-1/12, 4/3, -5/2]
-        case 6:
-            stencil = [1/90, -3/20, 3/2, -49/18]
-        case 8:
-            stencil = [-1/560, 8/315, -1/5, 8/5, -205/72]
-        case _:
-            raise NotImplementedError(f"Finite difference scheme not found for {order = }")
-    
-    stencil = _mirror_list(stencil)
-    return _matrix_from_central_stencil(stencil, 2, N, L, dtype, boundary_condition)
-    
-
-def _matrix_from_central_stencil(stencil: list[float], power: int, 
-                         N: tuple[int], L: tuple[float], dtype: type, 
-                         boundary_condition: str = "zero") -> sp.dia_matrix:
-    """
-    Creates a full matrix from a central stencil. Determines indices from stencil
-    """
-
-    available_boundary_conditions = ["zero", "periodic"]
-    if boundary_condition not in available_boundary_conditions:
-        raise ValueError(f"Invalid boundary condition: {boundary_condition}. Options are: " 
-                         + ", ".join(available_boundary_conditions))
-
-    if boundary_condition == "zero":
-        indices = np.arange(len(stencil)) - len(stencil) // 2
-        axis_indices = [indices for _ in N]
-
-    elif boundary_condition == "periodic":
-        indices = np.arange(len(stencil)) - len(stencil) // 2
-        # There might be different sizes for each axis.
-        # Therefore, we keep the updated indices for each axis
-        periodic_indices = [list() for _ in N]
-        periodic_stencil = []
-        for i, ind in enumerate(indices):
-            # Lower diagonals
-            if ind < 0:
-                for i, n in enumerate(N):
-                    periodic_indices[i].append(-n - ind)
-                periodic_stencil.append(stencil[i])
-            # Upper diagonals
-            elif ind > 0:
-                for i, n in enumerate(N):
-                    periodic_indices[i].append(n - ind)
-                periodic_stencil.append(stencil[i])
-            # Also keep the central diagonals
-            else:
-                for i in range(len(N)):
-                    periodic_indices[i] += list(indices)
-                periodic_stencil += stencil
-        axis_indices = np.array(periodic_indices)
-        stencil = np.array(periodic_stencil)
-
-    mat = np.zeros((1,1))    
-    for l, n, indices in zip(L, N, axis_indices):
-        h = l / n
-        next_mat = 1/h**power * sp.diags(
-            stencil,
-            indices,
-            shape=(n, n),
-            dtype=dtype,
-            format="dia"
-            )
-        mat = sp.kronsum(mat, next_mat, format="dia")
-
-    return mat
-
-
-def _mirror_list(l: list) -> list:
-    """
-    Mirror a list around the final element.
-
-    Example: [a, b, c] -> [a, b, c, b, a]
-    """
-    return l + l[-2::-1]
-
-
-def _mirror_sign_list(l: list) -> list:
-    """
-    Mirror a list around the final element,
-    and flip the sign of each new element.
-
-    Example: [-a, b, c] -> [-a, b, c, -b, a]
-    """
-    return l + [-i for i in l[-2::-1]]
+import numpy as np
+from scipy import sparse as sp
+
+
+def nabla(
+    N: tuple[int],
+    L: tuple[float],
+    order: int = 2,
+    dtype: type = np.float64,
+    boundary_condition: str = "zero",
+) -> sp.dia_matrix:
+    """Finite difference derivative in cartesian coordinates.
+    Uses central stencil.
+
+    Example: approximate the derivative of sin(x).
+
+    >>> from qm_sim.spatial_derivative.cartesian import nabla
+    >>> import numpy as np
+    >>> N = (1000,)
+    >>> L = (2*np.pi,)
+    >>> n = nabla( N, L, boundary_condition="periodic")
+    >>> x = np.linspace( 0, L[0], N[0], endpoint=False )
+    >>> y = np.sin(x)
+    >>> np.allclose(n @ y, np.cos(x)) # The analytical solution is cos(x)
+    True
+
+    :param N: Discretization count along each axis
+    :type N: tuple[int]
+    :param L: System size along each axis
+    :type L: tuple[float]
+    :param order: Numerical order of the differentiation scheme.
+        Options are:
+
+            - 2
+            - 4
+            - 6
+            - 8
+
+        Defaults to 2.
+    :type order: int, optional
+    :param dtype: datatype of matrix.
+        Defaults to np.float64
+    :type dtype: type, optional
+    :raises NotImplementedError: if requested order is not available
+    :return: Discretized derivative matrix
+    :rtype: sp.dia_matrix
+    :param boundary_condition: Which boundary condition to apply.
+            Options are:
+
+            - zero
+            - periodic
+
+            Defaults to "zero"
+    :type boundary_condition: str, optional
+    """
+    # Lookup for first half of stencil.
+    # A 0 is appended for the central element,
+    # and the rest is mirrored with a sign change later
+    match order:
+        case 2:
+            stencil = [-1 / 2]
+        case 4:
+            stencil = [1 / 12, -2 / 3]
+        case 6:
+            stencil = [-1 / 60, 3 / 20, -3 / 4]
+        case 8:
+            stencil = [1 / 280, -4 / 105, 1 / 5, -4 / 5]
+        case _:
+            raise NotImplementedError(
+                f"Finite difference scheme not found for {order = }"
+            )
+    stencil += [0]
+
+    stencil = _mirror_sign_list(stencil)
+    return _matrix_from_central_stencil(stencil, 1, N, L, dtype, boundary_condition)
+
+
+def laplacian(
+    N: tuple[int],
+    L: tuple[float],
+    order: int = 2,
+    dtype: type = np.float64,
+    boundary_condition: str = "zero",
+) -> sp.dia_matrix:
+    """Finite difference double derivative in cartesian coordinates.
+    Uses central stencil
+
+    Example: approximate the second derivative of sin(x).
+
+    >>> from qm_sim.spatial_derivative.cartesian import laplacian
+    >>> import numpy as np
+    >>> N = (1000,)
+    >>> L = (2*np.pi,)
+    >>> n = laplacian( N, L, boundary_condition="periodic" )
+    >>> x = np.linspace( 0, L[0], N[0], endpoint=False)
+    >>> y = np.sin(x)
+    >>> np.allclose(n @ y, -np.sin(x)) # The analytical solution is -sin(x)
+    True
+
+    :param N: Discretization count along each axis
+    :type N: tuple[int]
+    :param L: System size along each axis
+    :type L: tuple[float]
+    :param order: Numerical order of the differentiation scheme.
+        Options are:
+
+            - 2
+            - 4
+            - 6
+            - 8
+
+        Defaults to 2.
+    :type order: int, optional
+    :param dtype: datatype of matrix.
+        Defaults to np.float64
+    :type dtype: type, optional
+    :raises NotImplementedError: if requested order is not available
+    :return: Discretized derivative matrix
+    :rtype: sp.dia_matrix
+    :param boundary_condition: Which boundary condition to apply.
+            Options are:
+
+            - zero
+            - periodic
+
+            Defaults to "zero"
+    :type boundary_condition: str, optional
+    """
+    # lookup the first half of the stencil, to be mirrored later
+    match order:
+        case 2:
+            stencil = [1, -2]
+        case 4:
+            stencil = [-1 / 12, 4 / 3, -5 / 2]
+        case 6:
+            stencil = [1 / 90, -3 / 20, 3 / 2, -49 / 18]
+        case 8:
+            stencil = [-1 / 560, 8 / 315, -1 / 5, 8 / 5, -205 / 72]
+        case _:
+            raise NotImplementedError(
+                f"Finite difference scheme not found for {order = }"
+            )
+
+    stencil = _mirror_list(stencil)
+    return _matrix_from_central_stencil(stencil, 2, N, L, dtype, boundary_condition)
+
+
+def _matrix_from_central_stencil(
+    stencil: list[float],
+    power: int,
+    N: tuple[int],
+    L: tuple[float],
+    dtype: type,
+    boundary_condition: str = "zero",
+) -> sp.dia_matrix:
+    """
+    Creates a full matrix from a central stencil. Determines indices from stencil
+    """
+
+    available_boundary_conditions = ["zero", "periodic"]
+    if boundary_condition not in available_boundary_conditions:
+        raise ValueError(
+            f"Invalid boundary condition: {boundary_condition}. Options are: "
+            + ", ".join(available_boundary_conditions)
+        )
+
+    if boundary_condition == "zero":
+        indices = np.arange(len(stencil)) - len(stencil) // 2
+        axis_indices = [indices for _ in N]
+
+    elif boundary_condition == "periodic":
+        indices = np.arange(len(stencil)) - len(stencil) // 2
+        # There might be different sizes for each axis.
+        # Therefore, we keep the updated indices for each axis
+        periodic_indices = [list() for _ in N]
+        periodic_stencil = []
+        for i, ind in enumerate(indices):
+            # Lower diagonals
+            if ind < 0:
+                for i, n in enumerate(N):
+                    periodic_indices[i].append(-n - ind)
+                periodic_stencil.append(stencil[i])
+            # Upper diagonals
+            elif ind > 0:
+                for i, n in enumerate(N):
+                    periodic_indices[i].append(n - ind)
+                periodic_stencil.append(stencil[i])
+            # Also keep the central diagonals
+            else:
+                for i in range(len(N)):
+                    periodic_indices[i] += list(indices)
+                periodic_stencil += stencil
+        axis_indices = np.array(periodic_indices)
+        stencil = np.array(periodic_stencil)
+
+    mat = np.zeros((1, 1))
+    for l, n, indices in zip(L, N, axis_indices):
+        h = l / n
+        next_mat = sp.diags(
+            stencil,
+            indices,
+            shape=(n, n),
+            dtype=dtype,
+            format="dia",
+        )
+        next_mat *= 1 / h**power
+        mat = sp.kronsum(mat, next_mat, format="dia")
+
+    return mat
+
+
+def _mirror_list(l: list) -> list:
+    """
+    Mirror a list around the final element.
+
+    Example: [a, b, c] -> [a, b, c, b, a]
+    """
+    return l + l[-2::-1]
+
+
+def _mirror_sign_list(l: list) -> list:
+    """
+    Mirror a list around the final element,
+    and flip the sign of each new element.
+
+    Example: [-a, b, c] -> [-a, b, c, -b, a]
+    """
+    return l + [-i for i in l[-2::-1]]
```

### Comparing `qm-sim-0.1.0/src/qm_sim/temporal_solver/base.py` & `qm-sim-0.1.1/src/qm_sim/temporal_solver/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,114 @@
-from abc import ABC, abstractmethod
-from typing import Callable
-
-import numpy as np
-from tqdm import tqdm
-
-from ..nature_constants import h_bar
-
-# Dict to store subclasses of TemporalSolver
-_SCHEMES = {}
-
-
-class TemporalSolver(ABC):
-    """Class to solve :math:`y' = H(y)`"""
-
-    #: Name of the solver
-    name: str
-
-    #: Integration order
-    order: int
-
-    #: Is the method explicit or implicit?
-    explicit: bool
-
-    #: Is the method stable? 
-    #: If only conditionally stable, this will be true 
-    #: and :code:`dt` will be forced into its stable range
-    stable: bool
-
-    _skip_registration: bool = False
-
-    def __init__(self, H: Callable[[float], np.ndarray], output_shape: tuple[int] = None):
-        """Initialize a temporal solver
-
-        :param H: Function of time, representing the temporal derivative at that time
-        :type H: Callable[[float], np.ndarray]
-        :param output_shape: Expected shape of the solution, defaults to None
-        :type output_shape: tuple[int], optional
-        """
-
-        self.H = H
-
-        if output_shape is None:
-            output_shape = self.H(0).shape
-        self.output_shape = output_shape
-
-    def tqdm(self, t_start: float, t_end: float, enable: bool) -> tqdm:
-        pbar = tqdm(desc=self.name + " solver", total=t_end - t_start, disable=not enable)
-        pbar.bar_format = "{l_bar}{bar}| {n:#.02g}/{total:#.02g}"
-
-        # Add func to update with t, not dt
-        pbar.progress = lambda t: pbar.update(t - pbar.n)
-
-        return pbar
-
-
-    @abstractmethod
-    def iterate(self, v_0: np.ndarray, t0: float, t_final: float, 
-        dt: float, dt_storage: float = None, verbose: bool = True) -> tuple[np.ndarray, np.ndarray]:
-        """
-        Iterate the time propagation scheme.
-        Store the current state every :code:`dt_storage`
-
-        Args:
-            t_final (float): 
-                End time for calculations
-            dt_storage (float, optional): 
-                Data storage period. 
-                If None, store each calculation :code:`dt`
-                Defaults to None.
-
-        Returns:
-            np.ndarray:
-                Time values, shape (:code:`n`,) for :code:`n` storage times
-            np.ndarray:
-                State at times stored in the other output. shape (:code:`n`, :code:`H`.shape)
-        """
-        pass
-
-    def __init_subclass__(cls):
-        """Register subclasses of :class:`TemporalSolver`
-
-        """
-        if cls._skip_registration:
-            return
-        # Register new subclasses of TemporalSolver
-        if _SCHEMES.get(cls.name) is None:
-            _SCHEMES[cls.name] = cls
-        else:
-            raise ValueError("Cannot have two schemes with the same name")
-
-
-def get_temporal_solver(scheme: str) -> type[TemporalSolver]:
-    """Get a solver from its name, if it exists
-
-    :param scheme: Name of the solver
-    :type scheme: str
-    :raises ValueError: If the scheme does not exist
-    :return: A temporal solver class, NOT an instance
-    :rtype: type[TemporalSolver]
-    """
-    if scheme in _SCHEMES.keys():
-        return _SCHEMES[scheme]
-    raise ValueError(f"Scheme {scheme} not found. Options are:\n" 
-        + "\n".join(_SCHEMES.keys()))
+from abc import ABC, abstractmethod
+from typing import Callable
+
+import numpy as np
+from tqdm import tqdm
+
+from ..nature_constants import h_bar
+
+# Dict to store subclasses of TemporalSolver
+_SCHEMES = {}
+
+
+class TemporalSolver(ABC):
+    """Class to solve :math:`y' = H(y)`"""
+
+    #: Name of the solver
+    name: str
+
+    #: Integration order
+    order: int
+
+    #: Is the method explicit or implicit?
+    explicit: bool
+
+    #: Is the method stable?
+    #: If only conditionally stable, this will be true
+    #: and :code:`dt` will be forced into its stable range
+    stable: bool
+
+    _skip_registration: bool = False
+
+    def __init__(
+        self, H: Callable[[float], np.ndarray], output_shape: tuple[int] = None
+    ):
+        """Initialize a temporal solver
+
+        :param H: Function of time, representing the temporal derivative at that time
+        :type H: Callable[[float], np.ndarray]
+        :param output_shape: Expected shape of the solution, defaults to None
+        :type output_shape: tuple[int], optional
+        """
+
+        self.H = H
+
+        if output_shape is None:
+            output_shape = self.H(0).shape
+        self.output_shape = output_shape
+
+    def tqdm(self, t_start: float, t_end: float, enable: bool) -> tqdm:
+        pbar = tqdm(
+            desc=self.name + " solver", total=t_end - t_start, disable=not enable
+        )
+        pbar.bar_format = "{l_bar}{bar}| {n:#.02g}/{total:#.02g}"
+
+        # Add func to update with t, not dt
+        pbar.progress = lambda t: pbar.update(t - pbar.n)
+
+        return pbar
+
+    @abstractmethod
+    def iterate(
+        self,
+        v_0: np.ndarray,
+        t0: float,
+        t_final: float,
+        dt: float,
+        dt_storage: float = None,
+        verbose: bool = True,
+    ) -> tuple[np.ndarray, np.ndarray]:
+        """
+        Iterate the time propagation scheme.
+        Store the current state every :code:`dt_storage`
+
+        Args:
+            t_final (float):
+                End time for calculations
+            dt_storage (float, optional):
+                Data storage period.
+                If None, store each calculation :code:`dt`
+                Defaults to None.
+
+        Returns:
+            np.ndarray:
+                Time values, shape (:code:`n`,) for :code:`n` storage times
+            np.ndarray:
+                State at times stored in the other output. shape (:code:`n`, :code:`H`.shape)
+        """
+        pass
+
+    def __init_subclass__(cls):
+        """Register subclasses of :class:`TemporalSolver`"""
+        if cls._skip_registration:
+            return
+        # Register new subclasses of TemporalSolver
+        if _SCHEMES.get(cls.name) is None:
+            _SCHEMES[cls.name] = cls
+        else:
+            raise ValueError("Cannot have two schemes with the same name")
+
+
+def get_temporal_solver(scheme: str) -> type[TemporalSolver]:
+    """Get a solver from its name, if it exists
+
+    :param scheme: Name of the solver
+    :type scheme: str
+    :raises ValueError: If the scheme does not exist
+    :return: A temporal solver class, NOT an instance
+    :rtype: type[TemporalSolver]
+    """
+    if scheme in _SCHEMES.keys():
+        return _SCHEMES[scheme]
+    raise ValueError(
+        f"Scheme {scheme} not found. Options are:\n" + "\n".join(_SCHEMES.keys())
+    )
```

### Comparing `qm-sim-0.1.0/src/qm_sim/temporal_solver/crank_nicolson.py` & `qm-sim-0.1.1/src/qm_sim/temporal_solver/crank_nicolson.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,77 @@
-from typing import Callable
-
-import numpy as np
-from scipy.linalg import solve_banded
-from scipy.sparse import dia_matrix
-
-from .base import TemporalSolver
-
-
-def I_plus_aH(a: complex, H: dia_matrix) -> dia_matrix:
-    """Return I + aH, where :code:`I`is the unit matrix and :code:`a` is constant"""
-    out = H.copy().astype(np.complex128)
-    out.data *= a
-    zero_ind = list(out.offsets).index(0)
-    out.data[zero_ind] += 1
-    return out
-
-class CrankNicolson(TemporalSolver):
-    order = 2
-    explicit = False
-    stable = True
-    name = "crank-nicolson"
-
-    def __init__(self, H: Callable[[float], np.ndarray], output_shape: tuple[int] = None):
-        TemporalSolver.__init__(self, H, output_shape)
-        if len(self.output_shape) != 1:
-            raise ValueError("Crank-Nicolson solver only supports 1D systems")
-
-    def iterate(self, v_0: np.ndarray, t0: float, t_final: float, 
-        dt: float, dt_storage: float = None, verbose: bool = True) -> tuple[np.ndarray, np.ndarray]:
-
-        if dt_storage is None:
-            dt_storage = dt
-
-        H = self.H
-        prefactor = dt/2
-
-        tn = t0
-        psi_n = v_0
-
-        t = [tn]
-        psi = [psi_n]
-
-        with self.tqdm(t0, t_final, verbose) as pbar:
-            while tn < t_final:
-
-                # psi^n+1 = psi^n + dt/2*(F^n+1 + F^n)
-                # F^n = 1/ihbar * H^n @ psi^n
-                # => psi^n+1 = psi^n + dt/2ihbar*(H^n+1 @ psi^n+1 + H^n @ psi^n)
-                # (I - dt/2ihbar*(H^n+1) @ psi^n+1 = (I + dt/2ihbar*H^n) @ psi^n
-
-                lhs = I_plus_aH(-prefactor, H(tn + dt))
-                rhs = I_plus_aH(prefactor, H(tn)) @ psi_n
-                
-                # Reformulate the solve_banded function in terms of the dia_matrix class
-                psi_n = solve_banded(
-                    (-lhs.offsets[0], lhs.offsets[-1]),
-                    lhs.data[::-1, :],
-                    rhs,
-                    )
-
-                pbar.update(dt)
-                tn += dt
-
-                # store data every :code:`dt_storage`seconds
-                if tn // dt_storage > len(psi):
-                    psi.append(psi_n)
-                    t.append(tn)
-        return np.array(t), np.array(psi)
+from typing import Callable
+
+import numpy as np
+from scipy.linalg import solve_banded
+from scipy.sparse import dia_matrix
+
+from .base import TemporalSolver
+
+
+def I_plus_aH(a: complex, H: dia_matrix) -> dia_matrix:
+    """Return I + aH, where :code:`I`is the unit matrix and :code:`a` is constant"""
+    out = H.copy().astype(np.complex128)
+    out.data *= a
+    zero_ind = list(out.offsets).index(0)
+    out.data[zero_ind] += 1
+    return out
+
+
+class CrankNicolson(TemporalSolver):
+    order = 2
+    explicit = False
+    stable = True
+    name = "crank-nicolson"
+
+    def __init__(
+        self, H: Callable[[float], np.ndarray], output_shape: tuple[int] = None
+    ):
+        TemporalSolver.__init__(self, H, output_shape)
+        if len(self.output_shape) != 1:
+            raise ValueError("Crank-Nicolson solver only supports 1D systems")
+
+    def iterate(
+        self,
+        v_0: np.ndarray,
+        t0: float,
+        t_final: float,
+        dt: float,
+        dt_storage: float = None,
+        verbose: bool = True,
+    ) -> tuple[np.ndarray, np.ndarray]:
+        if dt_storage is None:
+            dt_storage = dt
+
+        H = self.H
+        prefactor = dt / 2
+
+        tn = t0
+        psi_n = v_0
+
+        t = [tn]
+        psi = [psi_n]
+
+        with self.tqdm(t0, t_final, verbose) as pbar:
+            while tn < t_final:
+                # psi^n+1 = psi^n + dt/2*(F^n+1 + F^n)
+                # F^n = 1/ihbar * H^n @ psi^n
+                # => psi^n+1 = psi^n + dt/2ihbar*(H^n+1 @ psi^n+1 + H^n @ psi^n)
+                # (I - dt/2ihbar*(H^n+1) @ psi^n+1 = (I + dt/2ihbar*H^n) @ psi^n
+
+                lhs = I_plus_aH(-prefactor, H(tn + dt))
+                rhs = I_plus_aH(prefactor, H(tn)) @ psi_n
+
+                # Reformulate the solve_banded function in terms of the dia_matrix class
+                psi_n = solve_banded(
+                    (-lhs.offsets[0], lhs.offsets[-1]),
+                    lhs.data[::-1, :],
+                    rhs,
+                )
+
+                pbar.update(dt)
+                tn += dt
+
+                # store data every :code:`dt_storage`seconds
+                if tn // dt_storage > len(psi):
+                    psi.append(psi_n)
+                    t.append(tn)
+        return np.array(t), np.array(psi)
```

### Comparing `qm-sim-0.1.0/src/qm_sim/temporal_solver/leapfrog.py` & `qm-sim-0.1.1/src/qm_sim/temporal_solver/leapfrog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-import numpy as np
-
-from .base import TemporalSolver
-
-
-class Leapfrog(TemporalSolver):
-    order = 2
-    explicit = True
-    stable = True # conditionally stable, dt is chosen accordingly
-    name = "leapfrog"
-    def iterate(self, v_0: np.ndarray, t0: float, t_final: float, 
-        dt: float, dt_storage: float = None, verbose: bool = True) -> tuple[np.ndarray, np.ndarray]:
-
-        # Override initial condition to preserve 2nd order accuracy
-        # psi_0 = psi_half - c*H_half*psi_half
-        # psi_1 = psi_half + c*H_half*psi_half
-        # c = dt / (2i*hbar)
-
-        if dt_storage is None:
-            dt_storage = dt
-
-        H = self.H
-
-        psi_half = v_0.flatten()
-        psi_0 = psi_half - dt / 2 * (H(t0 + dt/2) @ psi_half)
-        psi_1 = psi_half + dt / 2 * (H(t0 + dt/2) @ psi_half)
-
-        tn = t0 + dt/2
-
-        psi = [psi_1.reshape(self.output_shape)]
-        t = [tn]
-        with self.tqdm(t0, t_final, verbose) as pbar:
-            while tn < t_final:
-
-                # psi^n+1 = psi^n-1 + 2*dt*F^n
-                # F^n = 1/ihbar * H^n @ psi^n
-                # H^n = H0 + V^n
-
-                psi_2 = 2*dt * (H(tn) @ psi_1) + psi_0
-                psi_0, psi_1 = psi_1, psi_2
-
-                pbar.update(dt)
-                tn += dt
-
-                # store data every :code:`dt_storage`seconds
-                if tn // dt_storage > len(psi):
-                    psi.append(psi_0.reshape(self.output_shape))
-                    t.append(tn)
-        return np.array(t), np.array(psi)
+import numpy as np
+
+from .base import TemporalSolver
+
+
+class Leapfrog(TemporalSolver):
+    order = 2
+    explicit = True
+    stable = True  # conditionally stable, dt is chosen accordingly
+    name = "leapfrog"
+
+    def iterate(
+        self,
+        v_0: np.ndarray,
+        t0: float,
+        t_final: float,
+        dt: float,
+        dt_storage: float = None,
+        verbose: bool = True,
+    ) -> tuple[np.ndarray, np.ndarray]:
+        # Override initial condition to preserve 2nd order accuracy
+        # psi_0 = psi_half - c*H_half*psi_half
+        # psi_1 = psi_half + c*H_half*psi_half
+        # c = dt / (2i*hbar)
+
+        if dt_storage is None:
+            dt_storage = dt
+
+        H = self.H
+
+        psi_half = v_0.flatten()
+        psi_0 = psi_half - dt / 2 * (H(t0 + dt / 2) @ psi_half)
+        psi_1 = psi_half + dt / 2 * (H(t0 + dt / 2) @ psi_half)
+
+        tn = t0 + dt / 2
+
+        psi = [psi_1.reshape(self.output_shape)]
+        t = [tn]
+        with self.tqdm(t0, t_final, verbose) as pbar:
+            while tn < t_final:
+                # psi^n+1 = psi^n-1 + 2*dt*F^n
+                # F^n = 1/ihbar * H^n @ psi^n
+                # H^n = H0 + V^n
+
+                psi_2 = 2 * dt * (H(tn) @ psi_1) + psi_0
+                psi_0, psi_1 = psi_1, psi_2
+
+                pbar.update(dt)
+                tn += dt
+
+                # store data every :code:`dt_storage`seconds
+                if tn // dt_storage > len(psi):
+                    psi.append(psi_0.reshape(self.output_shape))
+                    t.append(tn)
+        return np.array(t), np.array(psi)
```

### Comparing `qm-sim-0.1.0/src/qm_sim/temporal_solver/scipy_solvers.py` & `qm-sim-0.1.1/src/qm_sim/temporal_solver/scipy_solvers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,98 @@
-import numpy as np
-from scipy.integrate import solve_ivp
-
-from .base import TemporalSolver
-
-
-class ScipySolver(TemporalSolver):
-    """Base class for scipy's :code:`solve_ivp`-based solvers"""
-
-    #: Name of the :code:`solve_ivp` method
-    method: str
-
-    _skip_registration = True
-
-    def iterate(self, v_0: np.ndarray, t0: float, t_final: float, 
-        dt: float, dt_storage: float = None, verbose: bool = True) -> tuple[np.ndarray, np.ndarray]:
-        
-        pbar = self.tqdm(t0, t_final, verbose)
-
-        # Precalculate the coefficient for negligible speedup
-
-        def ode_fun(t, y):
-            pbar.progress(t)
-            return self.H(t) @ y
-
-        sol = solve_ivp(
-            ode_fun, 
-            [t0, t_final], 
-            v_0.flatten(), 
-            t_eval=np.arange(t0, t_final, dt_storage),
-            first_step=dt,
-            method=self.method,
-            )
-        t = sol.t
-        psi = [sol.y[:, i].reshape(*self.output_shape) for i in range(len(t))]
-
-        return t, np.array(psi)
-    
-    def __init_subclass__(cls):
-        cls.name = "scipy-" + cls.name
-        cls._skip_registration = False
-        return super().__init_subclass__()
-
-class RungeKutta45(ScipySolver):
-    order = 5
-    explicit = True
-    stable = True
-    name = "Runge-Kutta 5(4)"
-    method = "RK45"
-
-class RungeKutta23(ScipySolver):
-    order = 3
-    explicit = True
-    stable = True
-    name = "Runge-Kutta 3(2)"
-    method = "RK23"
-
-class DOP853(ScipySolver):
-    order = 8
-    explicit = True
-    stable = True
-    name = "DOP853"
-    method = "DOP853"
-
-# Solver does not support complex numbers
-# class Radau(ScipySolver):
-#     order = 5
-#     explicit = False
-#     stable = True
-#     name = "radau"
-#     method = "Radau"
-
-class BDF(ScipySolver):
-    order = None
-    explicit = False
-    stable = True
-    name = "backwards-differentiation"
-    method = "BDF"
-
-# Solver does not support complex numbers
-# class LSODA(ScipySolver):
-#     order = None
-#     explicit = None
-#     stable = None
-#     name = "fortran LSODA"
-#     method = "LSODA"
+import numpy as np
+from scipy.integrate import solve_ivp
+
+from .base import TemporalSolver
+
+
+class ScipySolver(TemporalSolver):
+    """Base class for scipy's :code:`solve_ivp`-based solvers"""
+
+    #: Name of the :code:`solve_ivp` method
+    method: str
+
+    _skip_registration = True
+
+    def iterate(
+        self,
+        v_0: np.ndarray,
+        t0: float,
+        t_final: float,
+        dt: float,
+        dt_storage: float = None,
+        verbose: bool = True,
+    ) -> tuple[np.ndarray, np.ndarray]:
+        pbar = self.tqdm(t0, t_final, verbose)
+
+        # Precalculate the coefficient for negligible speedup
+
+        def ode_fun(t, y):
+            pbar.progress(t)
+            return self.H(t) @ y
+
+        sol = solve_ivp(
+            ode_fun,
+            [t0, t_final],
+            v_0.flatten(),
+            t_eval=np.arange(t0, t_final, dt_storage),
+            first_step=dt,
+            method=self.method,
+        )
+        t = sol.t
+        psi = [sol.y[:, i].reshape(*self.output_shape) for i in range(len(t))]
+
+        return t, np.array(psi)
+
+    def __init_subclass__(cls):
+        cls.name = "scipy-" + cls.name
+        cls._skip_registration = False
+        return super().__init_subclass__()
+
+
+class RungeKutta45(ScipySolver):
+    order = 5
+    explicit = True
+    stable = True
+    name = "Runge-Kutta 5(4)"
+    method = "RK45"
+
+
+class RungeKutta23(ScipySolver):
+    order = 3
+    explicit = True
+    stable = True
+    name = "Runge-Kutta 3(2)"
+    method = "RK23"
+
+
+class DOP853(ScipySolver):
+    order = 8
+    explicit = True
+    stable = True
+    name = "DOP853"
+    method = "DOP853"
+
+
+# Solver does not support complex numbers
+# class Radau(ScipySolver):
+#     order = 5
+#     explicit = False
+#     stable = True
+#     name = "radau"
+#     method = "Radau"
+
+
+class BDF(ScipySolver):
+    order = None
+    explicit = False
+    stable = True
+    name = "backwards-differentiation"
+    method = "BDF"
+
+
+# Solver does not support complex numbers
+# class LSODA(ScipySolver):
+#     order = None
+#     explicit = None
+#     stable = None
+#     name = "fortran LSODA"
+#     method = "LSODA"
```

### Comparing `qm-sim-0.1.0/tests/test_eigensolvers/scipy_backend.py` & `qm-sim-0.1.1/tests/test_eigensolvers/scipy_backend.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-import numba
-import numpy as np
-
-from typing import Callable
-
-from scipy._lib._threadsafety import ReentrancyLock
-from scipy.sparse.linalg._eigen.arpack.arpack import _SymmetricArpackParams, _UnsymmetricArpackParams
-
-
-def eigsh(A_OP, n, dtype, k=6, sigma=None, which='LM', v0=None,
-          ncv=None, maxiter=None, tol=0, return_eigenvectors=True,
-          ):
-    mode = 1
-    M_matvec = None
-    Minv_matvec = None
-    params = _SymmetricArpackParams(n, k, dtype.char, A_OP, mode,
-                                    M_matvec, Minv_matvec, sigma,
-                                    ncv, v0, maxiter, which, tol)
-
-    with ReentrancyLock("Nested calls to eigs/eighs not allowed: "
-        "ARPACK is not re-entrant"):
-        while not params.converged:
-            params.iterate()
-
-        return params.extract(return_eigenvectors)
-
-def eigs(A_OP, n, dtype, k=6, sigma=None, which='LM', v0=None,
-          ncv=None, maxiter=None, tol=0, return_eigenvectors=True,
-          ):
-    mode = 1
-    M_matvec = None
-    Minv_matvec = None
-    params = _UnsymmetricArpackParams(n, k, dtype.char, A_OP, mode,
-                                    M_matvec, Minv_matvec, sigma,
-                                    ncv, v0, maxiter, which, tol)
-
-    with ReentrancyLock("Nested calls to eigs/eighs not allowed: "
-        "ARPACK is not re-entrant"):
-        while not params.converged:
-            params.iterate()
-
-        return params.extract(return_eigenvectors)
-
-class TestHam:
-    def __init__(self, N, L, stencil, m = 1.0):
-        self.N = np.array(N)
-        self.L = np.array(L)
-        self.stencil = np.array(stencil)
-        self.m = m
-        self.ndim = len(N)
-        self.V = np.zeros(self.n)
-        self.h0 = np.array([-0.0380998212 / (m * (l/n)**2) for l, n in zip(L, N)])
-    
-    def set_potential(self, V: list | np.ndarray):
-        if isinstance(V, list):
-            self.V = np.array(V)
-        else:
-            self.V = V.copy()
-
-    @property
-    def n(self) -> int:
-        res = 1
-        for n in self.N:
-            res *= n
-        return res
-    
-    def matop(self) -> Callable[[np.ndarray], np.ndarray]:
-        V = self.V
-        ndim = self.ndim
-        h0 = self.h0
-        n = self.n
-        stencil = self.stencil
-        N = self.N
-
-        @numba.njit(parallel=True)
-        def scipy_numba_matop(x_in: np.ndarray) -> np.ndarray:
-
-            y_out = V.copy()
-
-            offset = 1
-            
-            for dim in range(ndim):
-
-                #  1 / dx^2
-                h0_dim = h0[dim]
-
-                #  y_i = x_i (*) stencil
-                #  stencil usually has more terms, so it can be e.g.
-                #  y_i = stencil[1]*x_i-1 + stencil[0]*x_i + stencil[1]*x_i+1
-                for i in numba.prange(n):
-                    stencil_sum = x_in[i] * stencil[0]
-                    for j, el in enumerate(stencil):
-                        # enumerate(stencil, start=1) fails with jit
-                        if j == 0:
-                            continue
-                        #  account for current dimension
-                        j *= offset
-                        #  range-check the x-vector
-                        if ((i + j) < n):
-                            stencil_sum += x_in[i + j] * el
-                        
-                        if ((i - j) >= 0):
-                            stencil_sum += x_in[i - j] * el
-                        
-                    y_out[i] += h0_dim * stencil_sum
-
-                offset *= N[dim]
-
-            return y_out
-        
-        # compile
-        scipy_numba_matop(np.zeros(self.N).flatten())
-        
-        return scipy_numba_matop
-
-    
+import numba
+import numpy as np
+
+from typing import Callable
+
+from scipy._lib._threadsafety import ReentrancyLock
+from scipy.sparse.linalg._eigen.arpack.arpack import _SymmetricArpackParams, _UnsymmetricArpackParams
+
+
+def eigsh(A_OP, n, dtype, k=6, sigma=None, which='LM', v0=None,
+          ncv=None, maxiter=None, tol=0, return_eigenvectors=True,
+          ):
+    mode = 1
+    M_matvec = None
+    Minv_matvec = None
+    params = _SymmetricArpackParams(n, k, dtype.char, A_OP, mode,
+                                    M_matvec, Minv_matvec, sigma,
+                                    ncv, v0, maxiter, which, tol)
+
+    with ReentrancyLock("Nested calls to eigs/eighs not allowed: "
+        "ARPACK is not re-entrant"):
+        while not params.converged:
+            params.iterate()
+
+        return params.extract(return_eigenvectors)
+
+def eigs(A_OP, n, dtype, k=6, sigma=None, which='LM', v0=None,
+          ncv=None, maxiter=None, tol=0, return_eigenvectors=True,
+          ):
+    mode = 1
+    M_matvec = None
+    Minv_matvec = None
+    params = _UnsymmetricArpackParams(n, k, dtype.char, A_OP, mode,
+                                    M_matvec, Minv_matvec, sigma,
+                                    ncv, v0, maxiter, which, tol)
+
+    with ReentrancyLock("Nested calls to eigs/eighs not allowed: "
+        "ARPACK is not re-entrant"):
+        while not params.converged:
+            params.iterate()
+
+        return params.extract(return_eigenvectors)
+
+class TestHam:
+    def __init__(self, N, L, stencil, m = 1.0):
+        self.N = np.array(N)
+        self.L = np.array(L)
+        self.stencil = np.array(stencil)
+        self.m = m
+        self.ndim = len(N)
+        self.V = np.zeros(self.n)
+        self.h0 = np.array([-0.0380998212 / (m * (l/n)**2) for l, n in zip(L, N)])
+    
+    def set_potential(self, V: list | np.ndarray):
+        if isinstance(V, list):
+            self.V = np.array(V)
+        else:
+            self.V = V.copy()
+
+    @property
+    def n(self) -> int:
+        res = 1
+        for n in self.N:
+            res *= n
+        return res
+    
+    def matop(self) -> Callable[[np.ndarray], np.ndarray]:
+        V = self.V
+        ndim = self.ndim
+        h0 = self.h0
+        n = self.n
+        stencil = self.stencil
+        N = self.N
+
+        @numba.njit(parallel=True)
+        def scipy_numba_matop(x_in: np.ndarray) -> np.ndarray:
+
+            y_out = V.copy()
+
+            offset = 1
+            
+            for dim in range(ndim):
+
+                #  1 / dx^2
+                h0_dim = h0[dim]
+
+                #  y_i = x_i (*) stencil
+                #  stencil usually has more terms, so it can be e.g.
+                #  y_i = stencil[1]*x_i-1 + stencil[0]*x_i + stencil[1]*x_i+1
+                for i in numba.prange(n):
+                    stencil_sum = x_in[i] * stencil[0]
+                    for j, el in enumerate(stencil):
+                        # enumerate(stencil, start=1) fails with jit
+                        if j == 0:
+                            continue
+                        #  account for current dimension
+                        j *= offset
+                        #  range-check the x-vector
+                        if ((i + j) < n):
+                            stencil_sum += x_in[i + j] * el
+                        
+                        if ((i - j) >= 0):
+                            stencil_sum += x_in[i - j] * el
+                        
+                    y_out[i] += h0_dim * stencil_sum
+
+                offset *= N[dim]
+
+            return y_out
+        
+        # compile
+        scipy_numba_matop(np.zeros(self.N).flatten())
+        
+        return scipy_numba_matop
+
+
```

### Comparing `qm-sim-0.1.0/PKG-INFO` & `qm-sim-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm-sim
-Version: 0.1.0
+Version: 0.1.1
 Summary: Quantum mechanics simulation library
 Author-Email: Viljar Femoen <author@example.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,65 +18,87 @@
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: matplotlib>=3.6
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: sphinx-mdinclude; extra == "docs"
+Requires-Dist: black; extra == "linting"
+Requires-Dist: isort; extra == "linting"
+Requires-Dist: pylint; extra == "linting"
 Provides-Extra: test
 Provides-Extra: torch
 Provides-Extra: docs
+Provides-Extra: linting
 Description-Content-Type: text/markdown
 
 # QM_sim
 
 Python library for simulation of quantum mechanical systems.
 
-[![.github/workflows/build_docs.yml](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml/badge.svg?branch=main&event=page_build)](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml)
+[![Build docs](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml/badge.svg)](https://github.com/viljarjf/QM_sim/actions/workflows/build_docs.yml)
+
+[//]: # (This is a comment. This comment should be on line 7. If this changes, also change the hard-coded line number for the start-line for the mdinclude at the top of docs/source/index.rst )
 
 ## Features 
 - 1D, 2D, and 3D systems
 - Choice of finite difference scheme
 - Zero and periodic boundary conditions
 - Stationary and temporal solutions
 - Plots
 
 ## Planned features
 - Transfer matrix for transmission ect.
-- Testing
+- Proper testing
+
+[//]: # (This is a comment. This comment should be on line 20. If this changes, also change the hard-coded line number for the end-line for the mdinclude at the top of docs/source/index.rst )
 
 ## Installation
 
 `pip install qm-sim`
 
 To be able to use the [PyTorch](https://pytorch.org/) backend for eigenvalue calculations, run the following command: 
 
-`pip install qm-sim .[torch]`
+`pip install qm-sim[torch]`
 
 This will install the cpu-version of the package. To run GPU calculations, install the version for your system at the [PyTorch website](https://pytorch.org/get-started/locally/) instead.
 
 ## Usage
 
 Examples are provided in the `examples/`-folder.
 These are enumerated with increasing level of simulation complexity.
 
 ## Contribution
 
 To contribute, please open a pull request to the `dev`-branch on [GitHub](https://www.github.com/viljarjf/QM_sim/pulls).
 
+### Linting
+
+When opening a PR, a linting check is performed.
+To ensure your contribution passes the checks, you can run the following
+
+~~~bash
+$ pip install .[linting]
+$ black src/qm_sim
+$ isort src -m 3 --trailing-comma
+$ pylint src --fail-under=7
+~~~
+
+### Setup
+
 The following is an example of how to set up VS Code for development, adapt to your IDE of choice.
 
 TL;DR: 
 - `pip install -e .` to install in an editable state
-- `pip install .` to (re)compile the C++ (subsequent python file edits will not be recognized before another reinstall)
 
-### Requirements
+**Requirements**
 - VS Code
     - Python extension
 - Python 3.10 or above
 
-### Setup
+**Steps**
 1. Clone the repo recursively and open the repo in VS Code. If not cloned recursively, initialize the submodules with `git submodule update --init`
 2. Press f1, and run `Python: Create Environment`. Select `.venv`
 3. Open a new terminal, which should automatically use the virtual environment. If not, run `.venv\Scripts\activate` on Windows, or `source .venv/bin/activate` on Unix
 4. In the same terminal, run `pip install -e .[test]` to install the current directory in an editable state, and the testing utility Pytest
 5. To run tests, press f1 and run `Python: Configure Tests`. Choose `pytest`. Run tests in the testing menu
```

