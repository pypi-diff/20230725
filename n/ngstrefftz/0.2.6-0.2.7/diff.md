# Comparing `tmp/ngstrefftz-0.2.6.tar.gz` & `tmp/ngstrefftz-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngstrefftz-0.2.6.tar", last modified: Sun Jul  9 01:40:56 2023, max compression
+gzip compressed data, was "ngstrefftz-0.2.7.tar", last modified: Tue Jul 25 13:50:36 2023, max compression
```

## Comparing `ngstrefftz-0.2.6.tar` & `ngstrefftz-0.2.7.tar`

### file list

```diff
@@ -1,156 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.727278 ngstrefftz-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.711278 ngstrefftz-0.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.715278 ngstrefftz-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-09 01:40:56.727278 ngstrefftz-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.715278 ngstrefftz-0.2.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.715278 ngstrefftz-0.2.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/_static/breadcrumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.715278 ngstrefftz-0.2.6/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/_static/css/mytheme.css
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/contrib.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/docu.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.715278 ngstrefftz-0.2.6/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/embTrefftz-adv.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/embTrefftz-helm.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/embTrefftz-poi.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/embTrefftz-stokes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/embTrefftz-wave.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/embTrefftz.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/helmholtz.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/laplace.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/qtwave.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/tunfitted.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/twave.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/notebooks/twavetents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.715278 ngstrefftz-0.2.6/docs/paper/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/paper/codemeta.json
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.711278 ngstrefftz-0.2.6/external_dependencies/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.715278 ngstrefftz-0.2.6/external_dependencies/ngstents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.711278 ngstrefftz-0.2.6/external_dependencies/ngstents/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.715278 ngstrefftz-0.2.6/external_dependencies/ngstents/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.711278 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/advection/
--rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/advection/advection2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/burgers/
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/burgers/burgers1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/burgers/burgers2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/euler/
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/euler/euler2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/maxwell/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/tents/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/tents/draw3dtent.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/tents/draw3dvertex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/wave/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/wave/horn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/wave/wave2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/demo/wave/wave3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/doc/StartPitching.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/doc/figs/
--rw-r--r--   0 runner    (1001) docker     (123)    57380 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/doc/figs/dag.png
--rw-r--r--   0 runner    (1001) docker     (123)    91865 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/doc/figs/map.png
--rw-r--r--   0 runner    (1001) docker     (123)    70062 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/doc/figs/subtents.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/py/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/py/conslaw/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/py/conslaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.719278 ngstrefftz-0.2.6/external_dependencies/ngstents/py/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/py/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/py/utils/_drawtents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/py/utils/_drawtents2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.723278 ngstrefftz-0.2.6/external_dependencies/ngstents/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/advection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/burgers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   133375 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/concurrentqueue.h
--rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/conservationlaw.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/euler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/maxwell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/paralleldepend.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/python_conslaw.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/python_tents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/symbolic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31227 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    47212 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/tents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/tents.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/tentsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/tentsolver_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/vis3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/vis3d.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/src/wave.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.723278 ngstrefftz-0.2.6/external_dependencies/ngstents/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_burgers_2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_causal_tents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_conslaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_tent_height_2D.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-09 01:40:10.000000 ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_tentlayers.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 01:40:56.727278 ngstrefftz-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.727278 ngstrefftz-0.2.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/airy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/diffopmapped.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25740 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/embtrefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/embtrefftz.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/intrule4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/mesh1dtents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/mesh1dtents.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/monomialfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/monomialfespace.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.727278 ngstrefftz-0.2.6/src/ngstrefftz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-09 01:40:56.000000 ngstrefftz-0.2.6/src/ngstrefftz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-09 01:40:56.000000 ngstrefftz-0.2.6/src/ngstrefftz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:40:56.000000 ngstrefftz-0.2.6/src/ngstrefftz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 01:40:56.000000 ngstrefftz-0.2.6/src/ngstrefftz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 01:40:56.000000 ngstrefftz-0.2.6/src/ngstrefftz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/planewavefe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/planewavefe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/python_trefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    48909 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/scalarmappedfe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/scalarmappedfe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/specialcoefficientfunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/specialcoefficientfunction.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    38072 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/trefftzfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/trefftzfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/twavetents.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/src/twavetents.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:40:56.727278 ngstrefftz-0.2.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/test/embt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/test/tents.py
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/test/trefftz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-09 01:40:09.000000 ngstrefftz-0.2.6/test/twave.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.351942 ngstrefftz-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.323941 ngstrefftz-0.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.327941 ngstrefftz-0.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-25 13:50:36.351942 ngstrefftz-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.327941 ngstrefftz-0.2.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.327941 ngstrefftz-0.2.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/_static/breadcrumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.327941 ngstrefftz-0.2.7/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/_static/css/mytheme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/docu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.327941 ngstrefftz-0.2.7/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/embTrefftz-adv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/embTrefftz-helm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/embTrefftz-poi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/embTrefftz-stokes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/embTrefftz-wave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/embTrefftz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/helmholtz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/laplace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/qtwave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/tunfitted.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/twave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/notebooks/twavetents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.327941 ngstrefftz-0.2.7/docs/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/paper/codemeta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.323941 ngstrefftz-0.2.7/external_dependencies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.327941 ngstrefftz-0.2.7/external_dependencies/ngstents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.323941 ngstrefftz-0.2.7/external_dependencies/ngstents/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.331941 ngstrefftz-0.2.7/external_dependencies/ngstents/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.323941 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.331941 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/advection/
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/advection/advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.331941 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/burgers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/burgers/burgers1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/burgers/burgers2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.331941 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/euler/
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/euler/euler2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.331941 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/maxwell/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.331941 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.335941 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/tents/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/tents/draw3dtent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/tents/draw3dvertex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.335941 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/wave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/wave/horn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/wave/wave2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/demo/wave/wave3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.335941 ngstrefftz-0.2.7/external_dependencies/ngstents/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/doc/StartPitching.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.335941 ngstrefftz-0.2.7/external_dependencies/ngstents/doc/figs/
+-rw-r--r--   0 runner    (1001) docker     (123)    57380 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/doc/figs/dag.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91865 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/doc/figs/map.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70062 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/doc/figs/subtents.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.335941 ngstrefftz-0.2.7/external_dependencies/ngstents/py/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.335941 ngstrefftz-0.2.7/external_dependencies/ngstents/py/conslaw/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/py/conslaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.335941 ngstrefftz-0.2.7/external_dependencies/ngstents/py/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/py/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/py/utils/_drawtents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/py/utils/_drawtents2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.343942 ngstrefftz-0.2.7/external_dependencies/ngstents/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/advection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/burgers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   133375 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/concurrentqueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/conservationlaw.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/maxwell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/paralleldepend.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/python_conslaw.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/python_tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/symbolic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31227 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    47212 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/tents.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/tentsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/tentsolver_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/vis3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/vis3d.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/src/wave.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.343942 ngstrefftz-0.2.7/external_dependencies/ngstents/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_burgers_2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_causal_tents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_conslaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_tent_height_2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-25 13:49:54.000000 ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_tentlayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:50:36.351942 ngstrefftz-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.347942 ngstrefftz-0.2.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/airy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/diffopmapped.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25740 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/embtrefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/embtrefftz.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/intrule4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/mesh1dtents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/mesh1dtents.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/monomialfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/monomialfespace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.347942 ngstrefftz-0.2.7/src/ngstrefftz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-25 13:50:36.000000 ngstrefftz-0.2.7/src/ngstrefftz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-25 13:50:36.000000 ngstrefftz-0.2.7/src/ngstrefftz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:50:36.000000 ngstrefftz-0.2.7/src/ngstrefftz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 13:50:36.000000 ngstrefftz-0.2.7/src/ngstrefftz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 13:50:36.000000 ngstrefftz-0.2.7/src/ngstrefftz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/planewavefe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/planewavefe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/python_trefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    48909 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/scalarmappedfe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/scalarmappedfe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/specialcoefficientfunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/specialcoefficientfunction.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38072 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/trefftzfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/trefftzfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/twavetents.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/src/twavetents.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:50:36.351942 ngstrefftz-0.2.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/test/embt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/test/tents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-25 13:49:53.000000 ngstrefftz-0.2.7/test/trefftz.py
```

### Comparing `ngstrefftz-0.2.6/.github/workflows/build.yml` & `ngstrefftz-0.2.7/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -201,30 +201,34 @@
              jupyter nbextension install --user --py webgui_jupyter_widgets
              jupyter nbextension enable --user --py webgui_jupyter_widgets            
       - name: Build and Commit
         uses: sphinx-notes/pages@v2
         with:
           repository_path: 'NGSTrefftz'
           #requirements_path: ./docs/requirements.txt
-      - name: Push changes
-        uses: ad-m/github-push-action@master
-        if: github.event_name == 'release' && github.event.action == 'created'
-        with:
-          directory: 'NGSTrefftz'
-          github_token: ${{ secrets.GITHUB_TOKEN }}
-          branch: gh-pages
       - run: tree -d .
       - name: Upload
-        uses: actions/upload-artifact@v1
+        uses: actions/upload-pages-artifact@v2
         with:
-          name: gh-page
           path: 'NGSTrefftz/'
-      - name: Debugging 
-        if: ${{ failure() }}
-        run: cat /tmp/sphinx*
+                
+  deploy-docs:
+    needs: docs
+    permissions:
+      pages: write      # to deploy to Pages
+      id-token: write   # to verify the deployment originates from an appropriate source
+    environment:
+      name: github-pages
+      url: ${{ steps.deployment.outputs.page_url }}
+    runs-on: ubuntu-latest
+    if: github.event_name == 'release' && github.event.action == 'created'
+    steps:
+      - name: Deploy to GitHub Pages
+        id: deployment
+        uses: actions/deploy-pages@v2
 
   paper:
     runs-on: ubuntu-latest
     name: Paper Draft
     steps:
       - name: Checkout
         uses: actions/checkout@v3
```

### Comparing `ngstrefftz-0.2.6/.github/workflows/build_pip.sh` & `ngstrefftz-0.2.7/.github/workflows/build_pip.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.2.7/.github/workflows/build_pip_mac.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.2.7/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/CONTRIBUTING.md` & `ngstrefftz-0.2.7/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -53,7 +53,13 @@
    git rebase --interactive --fork-point main <your-feature-name> 
    ```
 
 5. Push your topic branch up to your fork and [open a Pull Request](https://help.github.com/articles/using-pull-requests/).
 
 **IMPORTANT**: By submitting a patch, you agree to allow the project owners to license your work under the terms of the *LGPL License*.
 
+## Code format
+
+A code style file is provided in the repo to be used with `clang-format`. All c++ files should be formated using this style, to quickly apply it to all files use
+   ```bash
+   find src/ -iname *.hpp -o -iname *.cpp | xargs clang-format -style='file:.clang-format' -i
+   ```
```

### Comparing `ngstrefftz-0.2.6/Dockerfile` & `ngstrefftz-0.2.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/LICENSE` & `ngstrefftz-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/PKG-INFO` & `ngstrefftz-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.2.6
+Version: 0.2.7
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
```

### Comparing `ngstrefftz-0.2.6/README.md` & `ngstrefftz-0.2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 ⚠️ Feb, 2022: If you are using NGSolve nightly releases: [NGSolve@eda758d](https://github.com/NGSolve/ngsolve/commit/eda758d99483888851913d8a5c9aff4d0cbc9cc2) breaks a dependency and [NGSolve@3d52ecd](https://github.com/NGSolve/ngsolve/commit/3d52ecd615f2b7c409219eebaba99288ea19c1bc) produces import issue. Make sure to update ngstrefftz submodules and move to newest ngsolve version, at least [NGSolve@5839a09](https://github.com/NGSolve/ngsolve/commit/5839a09810235a938bd85807d8e638d3a0b6c69d).
 
 🚀 Jan, 2022: NGSTrefftz is now available via pip! 
 
 🚀 Nov, 2021: NGSTrefftz now comes in a docker and with binder notebooks! 
 
 ## Papers using the code
+* *Trefftz Discontinuous Galerkin discretization for the Stokes problem*  
+Philip L. Lederer, Christoph Lehrenfeld, Paul Stocker  
+[![arXiv](https://img.shields.io/badge/arXiv-2306.14600-b31b1b.svg)](https://arxiv.org/abs/2306.14600)
 * *Unfitted Trefftz discontinuous Galerkin methods for elliptic boundary value problems*  
 Fabian Heimann, Christoph Lehrenfeld, Paul Stocker, Henry von Wahl  
 [![arXiv](https://img.shields.io/badge/arXiv-2212.12236-b31b1b.svg)](https://arxiv.org/abs/2212.12236)
 * *Embedded Trefftz discontinuous Galerkin methods*  
 Christoph Lehrenfeld, Paul Stocker   
 [![arXiv](https://img.shields.io/badge/arXiv-2201.07041-b31b1b.svg)](https://arxiv.org/abs/2201.07041)
 * *A space-time quasi-Trefftz DG method for the wave equation with piecewise-smooth coefficients*
```

### Comparing `ngstrefftz-0.2.6/docs/conf.py` & `ngstrefftz-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/docu.rst` & `ngstrefftz-0.2.7/docs/docu.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/index.rst` & `ngstrefftz-0.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/intro.rst` & `ngstrefftz-0.2.7/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/embTrefftz-adv.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/embTrefftz-adv.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/embTrefftz-helm.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/embTrefftz-helm.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/embTrefftz-poi.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/embTrefftz-poi.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/embTrefftz-stokes.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/embTrefftz-stokes.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/embTrefftz-wave.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/embTrefftz-wave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/embTrefftz.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/embTrefftz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/helmholtz.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/helmholtz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/index.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/laplace.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/laplace.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/qtwave.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/qtwave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/tunfitted.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/tunfitted.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/twave.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/twave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/notebooks/twavetents.ipynb` & `ngstrefftz-0.2.7/docs/notebooks/twavetents.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/paper/codemeta.json` & `ngstrefftz-0.2.7/docs/paper/codemeta.json`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/paper/paper.bib` & `ngstrefftz-0.2.7/docs/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/paper/paper.md` & `ngstrefftz-0.2.7/docs/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/docs/requirements.txt` & `ngstrefftz-0.2.7/docs/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -100,10 +100,10 @@
 typing_extensions==4.4.0
 urllib3==1.26.12
 wcwidth==0.2.5
 webencodings==0.5.1
 webgui-jupyter-widgets==0.2.14
 websocket-client==1.4.1
 widgetsnbextension==4.0.3
-
+scipy>=1.11.1 
 xfem>=2.1.2303
 ngstrefftz>=0.2.3
```

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/.github/workflows/build.yml` & `ngstrefftz-0.2.7/external_dependencies/ngstents/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/README.md` & `ngstrefftz-0.2.7/external_dependencies/ngstents/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/advection/advection2d.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/advection/advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/advection/advection2d_periodic.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/advection/advection2d_periodic.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/burgers/burgers1d.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/burgers/burgers1d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/burgers/burgers2d.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/burgers/burgers2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/euler/euler2d.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/euler/euler2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/maxwell/maxwell3d.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/maxwell/maxwell3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/tents/draw3dtent.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/tents/draw3dtent.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/tents/draw3dvertex.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/tents/draw3dvertex.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/wave/horn.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/wave/horn.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/wave/wave2d.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/wave/wave2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/demo/wave/wave3d.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/demo/wave/wave3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/doc/StartPitching.ipynb` & `ngstrefftz-0.2.7/external_dependencies/ngstents/doc/StartPitching.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/doc/figs/dag.png` & `ngstrefftz-0.2.7/external_dependencies/ngstents/doc/figs/dag.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/doc/figs/map.png` & `ngstrefftz-0.2.7/external_dependencies/ngstents/doc/figs/map.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/doc/figs/subtents.png` & `ngstrefftz-0.2.7/external_dependencies/ngstents/doc/figs/subtents.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/py/conslaw/__init__.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/py/conslaw/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/py/utils/_drawtents.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/py/utils/_drawtents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/py/utils/_drawtents2d.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/py/utils/_drawtents2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/CMakeLists.txt` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/advection.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/advection.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/burgers.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/burgers.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/concurrentqueue.h` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/concurrentqueue.h`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/conservationlaw.hpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/conservationlaw.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/euler.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/euler.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/maxwell.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/maxwell.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/paralleldepend.hpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/paralleldepend.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/python_conslaw.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/python_conslaw.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/python_tents.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/python_tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/symbolic.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/symbolic.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/tents.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/tents.hpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/tents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/tentsolver.hpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/tentsolver.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/tentsolver_impl.hpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/tentsolver_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/vis3d.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/vis3d.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/vis3d.hpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/vis3d.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/src/wave.cpp` & `ngstrefftz-0.2.7/external_dependencies/ngstents/src/wave.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_burgers_2D.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_burgers_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_causal_tents.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_causal_tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_conslaw.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_conslaw.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_tent_height_2D.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_tent_height_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/external_dependencies/ngstents/tests/test_tentlayers.py` & `ngstrefftz-0.2.7/external_dependencies/ngstents/tests/test_tentlayers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/setup.py` & `ngstrefftz-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/CMakeLists.txt` & `ngstrefftz-0.2.7/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/__init__.py` & `ngstrefftz-0.2.7/src/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,32 +18,32 @@
         u,v = fes.TnT()
         a = BilinearForm(fes)
         a += SymbolicBFI(u*v)
         a.Assemble()
         wavefront = self.GetWavefront()
         ipfct=IntegrationPointFunction(initmesh,intrule,wavefront)
         f = LinearForm(fes)
-        f += SymbolicLFI(ipfct*v, intrule=intrule)
+        f += SymbolicLFI(ipfct*v).SetIntegrationRule(eltyp,intrule)
         f.Assemble()
-        U.vec.data = a.mat.Inverse() * f.vec
+        U.vec.data = a.mat.Inverse(inverse='sparsecholesky') * f.vec
         # return gfu
     else:
         fes = L2(initmesh, order=order-1)**(D+1)
         u,v = fes.TnT()
         wavefront = self.GetWavefront()
         a = BilinearForm(fes)
         a += SymbolicBFI(u*v)
         a.Assemble()
 
         sirsize = int(wavefront.Width()/(D+1))
+        f = LinearForm(fes)
         for d in range(D+1):
             ipfct=IntegrationPointFunction(initmesh,intrule,wavefront[:,d*sirsize:(d+1)*sirsize])
-            f = LinearForm(fes)
-            f += SymbolicLFI(ipfct*v[d], intrule=intrule)
-            f.Assemble()
+            f += SymbolicLFI(ipfct*v[d]).SetIntegrationRule(eltyp,intrule)
+        f.Assemble()
         U.vec.data = a.mat.Inverse() * f.vec
 
 
 setattr(TWaveTents1, 'GetWave', GetWave)
 setattr(TWaveTents2, 'GetWave', GetWave)
 setattr(TWaveTents3, 'GetWave', GetWave)
 setattr(QTWaveTents1, 'GetWave', GetWave)
```

### Comparing `ngstrefftz-0.2.6/src/airy.cpp` & `ngstrefftz-0.2.7/src/airy.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/diffopmapped.hpp` & `ngstrefftz-0.2.7/src/diffopmapped.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/embtrefftz.cpp` & `ngstrefftz-0.2.7/src/embtrefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/embtrefftz.hpp` & `ngstrefftz-0.2.7/src/embtrefftz.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/intrule4.cpp` & `ngstrefftz-0.2.7/src/intrule4.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/mesh1dtents.cpp` & `ngstrefftz-0.2.7/src/mesh1dtents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/monomialfespace.cpp` & `ngstrefftz-0.2.7/src/monomialfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/monomialfespace.hpp` & `ngstrefftz-0.2.7/src/monomialfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/ngstrefftz.egg-info/PKG-INFO` & `ngstrefftz-0.2.7/src/ngstrefftz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.2.6
+Version: 0.2.7
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
```

### Comparing `ngstrefftz-0.2.6/src/ngstrefftz.egg-info/SOURCES.txt` & `ngstrefftz-0.2.7/src/ngstrefftz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -116,9 +116,8 @@
 src/ngstrefftz.egg-info/PKG-INFO
 src/ngstrefftz.egg-info/SOURCES.txt
 src/ngstrefftz.egg-info/dependency_links.txt
 src/ngstrefftz.egg-info/requires.txt
 src/ngstrefftz.egg-info/top_level.txt
 test/embt.py
 test/tents.py
-test/trefftz.py
-test/twave.py
+test/trefftz.py
```

### Comparing `ngstrefftz-0.2.6/src/planewavefe.cpp` & `ngstrefftz-0.2.7/src/planewavefe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/planewavefe.hpp` & `ngstrefftz-0.2.7/src/planewavefe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/python_trefftz.cpp` & `ngstrefftz-0.2.7/src/python_trefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/scalarmappedfe.cpp` & `ngstrefftz-0.2.7/src/scalarmappedfe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/scalarmappedfe.hpp` & `ngstrefftz-0.2.7/src/scalarmappedfe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/specialcoefficientfunction.cpp` & `ngstrefftz-0.2.7/src/specialcoefficientfunction.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -29,14 +29,20 @@
       values (i, 0) = Evaluate (ir[i]);
   }
 
   IntegrationPointFunction ::IntegrationPointFunction (
       shared_ptr<MeshAccess> mesh, IntegrationRule &intrule, Vector<> ipdata)
       : CoefficientFunction (1)
   {
+    this->ma = mesh;
+    this->intrule.SetSize (intrule.Size ());
+    for (size_t i = 0; i < intrule.Size (); i++)
+      this->intrule[i] = (intrule)[i];
+    this->intrule.SetDim (intrule.Dim ());
+
     values.resize (mesh->GetNE ());
     int elnr = 0;
     for (auto &vec : values)
       {
         vec.resize (intrule.GetNIP ());
         for (size_t i = 0; i < vec.size (); i++)
           {
@@ -47,14 +53,20 @@
       }
   }
 
   IntegrationPointFunction ::IntegrationPointFunction (
       shared_ptr<MeshAccess> mesh, IntegrationRule &intrule, Matrix<> ipdata)
       : CoefficientFunction (1)
   {
+    this->ma = mesh;
+    this->intrule.SetSize (intrule.Size ());
+    for (size_t i = 0; i < intrule.Size (); i++)
+      this->intrule[i] = (intrule)[i];
+    this->intrule.SetDim (intrule.Dim ());
+
     values.resize (mesh->GetNE ());
     int elnr = 0;
     for (auto &vec : values)
       {
         vec.resize (intrule.GetNIP ());
         for (size_t i = 0; i < vec.size (); i++)
           {
@@ -89,14 +101,59 @@
             cout << values[i][j] << ", ";
           }
         cout << endl;
       }
     cout << endl;
   }
 
+  vector<vector<double>> IntegrationPointFunction ::Export ()
+  {
+    LocalHeap lh (1000 * 1000 * 100, "export intpointfct");
+
+    vector<vector<double>> pointnvalues;
+    pointnvalues.resize (ma->GetNE () * intrule.GetNIP ());
+    for (size_t elnr = 0; elnr < ma->GetNE (); elnr++)
+      {
+        switch (ma->GetDimension ())
+          {
+          case 2:
+            {
+              MappedIntegrationRule<2, 2> mir (intrule,
+                                               ma->GetTrafo (elnr, lh), lh);
+              for (auto mip : mir)
+                {
+                  auto &vec = pointnvalues[elnr * intrule.GetNIP ()
+                                           + mip.GetIPNr ()];
+                  vec.resize (3);
+                  for (int i = 0; i < 2; i++)
+                    vec[i] = mip.Point ()[i];
+                  vec[2] = values[elnr][mip.GetIPNr ()];
+                }
+              break;
+            }
+          case 3:
+            {
+              MappedIntegrationRule<3, 3> mir (intrule,
+                                               ma->GetTrafo (elnr, lh), lh);
+              for (auto mip : mir)
+                {
+                  auto &vec = pointnvalues[elnr * intrule.GetNIP ()
+                                           + mip.GetIPNr ()];
+                  vec.resize (4);
+                  for (int i = 0; i < 3; i++)
+                    vec[i] = mip.Point ()[i];
+                  vec[3] = values[elnr][mip.GetIPNr ()];
+                }
+              break;
+            }
+          }
+      }
+    return pointnvalues;
+  }
+
   WeightedRadiusFunction ::WeightedRadiusFunction (
       shared_ptr<MeshAccess> mesh, shared_ptr<CoefficientFunction> wavespeedcf)
       : CoefficientFunction (1)
   {
     LocalHeap lh (1000 * 1000 * 100);
     values.SetSize (mesh->GetNE ());
     for (size_t elnr = 0; elnr < mesh->GetNE (); elnr++)
@@ -232,15 +289,16 @@
             }),
             py::arg ("mesh"), py::arg ("intrule"), py::arg ("Vector"))
       .def (py::init ([] (shared_ptr<MeshAccess> mesh,
                           IntegrationRule &intrule, Matrix<> data) {
               return new IntegrationPointFunction (mesh, intrule, data);
             }),
             py::arg ("mesh"), py::arg ("intrule"), py::arg ("Matrix"))
-      .def ("PrintTable", &IntegrationPointFunction::PrintTable);
+      .def ("PrintTable", &IntegrationPointFunction::PrintTable)
+      .def ("Export", &IntegrationPointFunction::Export);
 
   py::class_<WeightedRadiusFunction, shared_ptr<WeightedRadiusFunction>,
              CoefficientFunction> (m, "WeightedRadiusFunction")
       .def (py::init ([] (shared_ptr<MeshAccess> mesh,
                           shared_ptr<CoefficientFunction> wavespeedcf) {
               return new WeightedRadiusFunction (mesh, wavespeedcf);
             }),
```

### Comparing `ngstrefftz-0.2.6/src/specialcoefficientfunction.hpp` & `ngstrefftz-0.2.7/src/specialcoefficientfunction.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -35,22 +35,25 @@
                                   FlatMatrix<double> values) const;
   };
 
   class IntegrationPointFunction : public CoefficientFunction
   {
   private:
     vector<vector<double>> values;
+    shared_ptr<MeshAccess> ma;
+    IntegrationRule intrule;
 
   public:
     IntegrationPointFunction (shared_ptr<MeshAccess> mesh,
                               IntegrationRule &intrule, Vector<> ipdata);
     IntegrationPointFunction (shared_ptr<MeshAccess> mesh,
                               IntegrationRule &intrule, Matrix<> ipdata);
     virtual double Evaluate (const BaseMappedIntegrationPoint &ip) const;
     void PrintTable ();
+    vector<vector<double>> Export ();
   };
 
   class WeightedRadiusFunction : public CoefficientFunction
   {
   private:
     Vector<> values;
```

### Comparing `ngstrefftz-0.2.6/src/trefftzfespace.cpp` & `ngstrefftz-0.2.7/src/trefftzfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/trefftzfespace.hpp` & `ngstrefftz-0.2.7/src/trefftzfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/twavetents.cpp` & `ngstrefftz-0.2.7/src/twavetents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/src/twavetents.hpp` & `ngstrefftz-0.2.7/src/twavetents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/test/embt.py` & `ngstrefftz-0.2.7/test/embt.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/test/tents.py` & `ngstrefftz-0.2.7/test/tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.2.6/test/trefftz.py` & `ngstrefftz-0.2.7/test/trefftz.py`

 * *Files identical despite different names*

