# Comparing `tmp/openpnm-3.1.2.tar.gz` & `tmp/openpnm-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpnm-3.1.2.tar", last modified: Sat Feb 11 17:33:19 2023, max compression
+gzip compressed data, was "openpnm-3.2.0.tar", last modified: Tue Jul 25 03:58:12 2023, max compression
```

## Comparing `openpnm-3.1.2.tar` & `openpnm-3.2.0.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.253656 openpnm-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-11 17:32:29.000000 openpnm-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-02-11 17:33:19.253656 openpnm-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-02-11 17:32:29.000000 openpnm-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.229656 openpnm-3.1.2/openpnm/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.229656 openpnm-3.1.2/openpnm/_skgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.229656 openpnm-3.1.2/openpnm/_skgraph/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/_bcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/_cubic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/_delaunay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/_fcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/_gabriel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/_voronoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/_voronoi_delaunay_dual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.229656 openpnm-3.1.2/openpnm/_skgraph/generators/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18008 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/generators/tools/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.229656 openpnm-3.1.2/openpnm/_skgraph/io/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/io/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.233656 openpnm-3.1.2/openpnm/_skgraph/operations/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/operations/_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/operations/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/operations/_unary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.233656 openpnm-3.1.2/openpnm/_skgraph/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/queries/QuickUnion.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/queries/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/queries/_qupc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.233656 openpnm-3.1.2/openpnm/_skgraph/simulations/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/simulations/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/simulations/_percolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.233656 openpnm-3.1.2/openpnm/_skgraph/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/tools/GraphBundle.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/tools/_coords_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    30275 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/tools/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.233656 openpnm-3.1.2/openpnm/_skgraph/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/_skgraph/visualization/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.233656 openpnm-3.1.2/openpnm/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_advection_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_drainage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_fickian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_fourier_conduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    22249 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_invasion_percolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_ohmic_conduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_reactive_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_stokes_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_transient_advection_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_transient_fickian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_transient_reactive_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/algorithms/_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.233656 openpnm-3.1.2/openpnm/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/contrib/_multiphase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/contrib/_transient_multiphysics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.233656 openpnm-3.1.2/openpnm/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17642 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/core/_base2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29045 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/core/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    19967 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/core/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.233656 openpnm-3.1.2/openpnm/integrators/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/integrators/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/integrators/_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.237656 openpnm-3.1.2/openpnm/io/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_comsol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_jsongraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_marock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_networkx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_paraview.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_pergeos.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_porespy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_salome.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_statoil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_stl.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/io/_xdmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.237656 openpnm-3.1.2/openpnm/models/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/_doctxt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.237656 openpnm-3.1.2/openpnm/models/collections/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.237656 openpnm-3.1.2/openpnm/models/collections/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/geometry/circles_and_rectangles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/geometry/cones_and_cylinders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/geometry/cubes_and_cuboids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/geometry/pyramids_and_cuboids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/geometry/spheres_and_cylinders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/geometry/squares_and_rectangles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/geometry/trapezoids_and_rectangles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.237656 openpnm-3.1.2/openpnm/models/collections/network/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.237656 openpnm-3.1.2/openpnm/models/collections/phase/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/phase/air.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/phase/gas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/phase/liquid.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/phase/mercury.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/phase/water.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.237656 openpnm-3.1.2/openpnm/models/collections/physics/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/physics/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/collections/physics/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.237656 openpnm-3.1.2/openpnm/models/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/_geodocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.237656 openpnm-3.1.2/openpnm/models/geometry/conduit_lengths/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/conduit_lengths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/conduit_lengths/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/diffusive_size_factors/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/diffusive_size_factors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/diffusive_size_factors/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/hydraulic_size_factors/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/hydraulic_size_factors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/hydraulic_size_factors/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/pore_cross_sectional_area/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_cross_sectional_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_cross_sectional_area/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/pore_seed/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_seed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_seed/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/pore_size/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_size/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_size/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/pore_surface_area/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_surface_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_surface_area/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/pore_volume/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/pore_volume/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_capillary_shape_factor/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_capillary_shape_factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_capillary_shape_factor/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_centroid/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_centroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_centroid/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_cross_sectional_area/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_cross_sectional_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_cross_sectional_area/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_endpoints/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_length/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_length/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_length/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_perimeter/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_perimeter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_perimeter/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_seed/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_seed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_seed/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_size/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_size/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_size/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_surface_area/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_surface_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_surface_area/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_vector/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_vector/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/geometry/throat_volume/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/geometry/throat_volume/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.241656 openpnm-3.1.2/openpnm/models/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/misc/_basic_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/misc/_neighbor_lookups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/misc/_simple_equations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/misc/_statistical_distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/network/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/network/_health.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/network/_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/_phasedocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/critical_props/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/critical_props/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/critical_props/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/density/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/density/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/diffusivity/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/diffusivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/diffusivity/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/heat_capacity/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/heat_capacity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/heat_capacity/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/misc/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/mixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/mixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/mixtures/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/partition_coefficient/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/partition_coefficient/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/partition_coefficient/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/surface_tension/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/surface_tension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/surface_tension/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/thermal_conductivity/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/thermal_conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/thermal_conductivity/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/vapor_pressure/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/vapor_pressure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/vapor_pressure/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/phase/viscosity/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/viscosity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/phase/viscosity/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/physics/ad_dif_conductance/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/ad_dif_conductance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/ad_dif_conductance/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/physics/capillary_pressure/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/capillary_pressure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/capillary_pressure/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/physics/diffusive_conductance/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/diffusive_conductance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/diffusive_conductance/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/physics/electrical_conductance/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/electrical_conductance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/electrical_conductance/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/physics/hydraulic_conductance/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/hydraulic_conductance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/hydraulic_conductance/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/physics/meniscus/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/meniscus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/meniscus/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.245656 openpnm-3.1.2/openpnm/models/physics/multiphase/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/multiphase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/multiphase/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.249656 openpnm-3.1.2/openpnm/models/physics/source_terms/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/source_terms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23165 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/source_terms/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.249656 openpnm-3.1.2/openpnm/models/physics/thermal_conductance/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/thermal_conductance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/models/physics/thermal_conductance/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.249656 openpnm-3.1.2/openpnm/network/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/_bcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/_cubic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/_cubic_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/_delaunay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/_delaunay_voronoi_dual.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/_fcc.py
--rw-r--r--   0 runner    (1001) docker     (123)    33980 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/network/_voronoi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.249656 openpnm-3.1.2/openpnm/phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/phase/_air.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/phase/_mercury.py
--rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/phase/_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/phase/_phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/phase/_species.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/phase/_water.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.249656 openpnm-3.1.2/openpnm/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/solvers/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/solvers/_pardiso.py
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/solvers/_petsc.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/solvers/_pyamg.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/solvers/_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.249656 openpnm-3.1.2/openpnm/topotools/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/topotools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/topotools/_graphtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/topotools/_perctools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43970 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/topotools/_topotools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.249656 openpnm-3.1.2/openpnm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/utils/_health.py
--rw-r--r--   0 runner    (1001) docker     (123)    20360 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/utils/_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/utils/_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/utils/_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.249656 openpnm-3.1.2/openpnm/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/visualization/_conduit_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-02-11 17:32:29.000000 openpnm-3.1.2/openpnm/visualization/_plottools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:33:19.229656 openpnm-3.1.2/openpnm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-02-11 17:33:19.000000 openpnm-3.1.2/openpnm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-02-11 17:33:19.000000 openpnm-3.1.2/openpnm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 17:33:19.000000 openpnm-3.1.2/openpnm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 17:33:19.000000 openpnm-3.1.2/openpnm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-11 17:33:19.000000 openpnm-3.1.2/openpnm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-11 17:33:19.000000 openpnm-3.1.2/openpnm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-11 17:33:19.253656 openpnm-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-11 17:32:29.000000 openpnm-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.312032 openpnm-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-25 03:57:13.000000 openpnm-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-25 03:58:12.312032 openpnm-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-25 03:57:13.000000 openpnm-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.292032 openpnm-3.2.0/openpnm/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.292032 openpnm-3.2.0/openpnm/_skgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.292032 openpnm-3.2.0/openpnm/_skgraph/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/_bcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/_cubic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/_delaunay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/_fcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/_gabriel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/_voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/_voronoi_delaunay_dual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.292032 openpnm-3.2.0/openpnm/_skgraph/generators/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18008 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/generators/tools/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.292032 openpnm-3.2.0/openpnm/_skgraph/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/io/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.292032 openpnm-3.2.0/openpnm/_skgraph/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/operations/_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/operations/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/operations/_unary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.292032 openpnm-3.2.0/openpnm/_skgraph/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/queries/QuickUnion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/queries/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/queries/_qupc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.292032 openpnm-3.2.0/openpnm/_skgraph/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/simulations/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/simulations/_percolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.296032 openpnm-3.2.0/openpnm/_skgraph/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/tools/GraphBundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/tools/_coords_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30275 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/tools/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.296032 openpnm-3.2.0/openpnm/_skgraph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/_skgraph/visualization/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.296032 openpnm-3.2.0/openpnm/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_advection_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_drainage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_fickian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_fourier_conduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22208 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_invasion_percolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_ohmic_conduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_reactive_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_stokes_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_transient_advection_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_transient_fickian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_transient_reactive_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/algorithms/_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.296032 openpnm-3.2.0/openpnm/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/contrib/_multiphase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/contrib/_transient_multiphysics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.296032 openpnm-3.2.0/openpnm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/core/_base2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29045 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/core/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19967 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/core/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.296032 openpnm-3.2.0/openpnm/integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/integrators/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/integrators/_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_comsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_jsongraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_marock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_networkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_paraview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_pergeos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_porespy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_salome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_statoil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/io/_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/_doctxt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/collections/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/geometry/circles_and_rectangles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/geometry/cones_and_cylinders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/geometry/cubes_and_cuboids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/geometry/pyramids_and_cuboids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/geometry/spheres_and_cylinders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/geometry/squares_and_rectangles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/geometry/trapezoids_and_rectangles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/collections/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/collections/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/phase/air.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/phase/gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/phase/liquid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/phase/mercury.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/phase/water.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/collections/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/physics/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/collections/physics/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/_geodocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/conduit_lengths/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/conduit_lengths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/conduit_lengths/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/diffusive_size_factors/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/diffusive_size_factors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/diffusive_size_factors/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/hydraulic_size_factors/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/hydraulic_size_factors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/hydraulic_size_factors/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/pore_cross_sectional_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_cross_sectional_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_cross_sectional_area/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/pore_seed/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_seed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_seed/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/pore_size/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_size/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/pore_surface_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_surface_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_surface_area/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/pore_volume/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/pore_volume/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/throat_capillary_shape_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_capillary_shape_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_capillary_shape_factor/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/throat_centroid/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_centroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_centroid/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.300032 openpnm-3.2.0/openpnm/models/geometry/throat_cross_sectional_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_cross_sectional_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_cross_sectional_area/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/geometry/throat_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_endpoints/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/geometry/throat_length/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_length/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_length/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/geometry/throat_perimeter/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_perimeter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_perimeter/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/geometry/throat_seed/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_seed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_seed/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/geometry/throat_size/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_size/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/geometry/throat_surface_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_surface_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_surface_area/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/geometry/throat_vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_vector/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/geometry/throat_volume/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/geometry/throat_volume/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/misc/_basic_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/misc/_neighbor_lookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/misc/_simple_equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/misc/_statistical_distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/network/_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/network/_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/_phasedocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/critical_props/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/critical_props/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/critical_props/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/density/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/density/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/diffusivity/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/diffusivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/diffusivity/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/heat_capacity/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/heat_capacity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/heat_capacity/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/misc/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/mixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/mixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/mixtures/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/partition_coefficient/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/partition_coefficient/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/partition_coefficient/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/surface_tension/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/surface_tension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/surface_tension/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/thermal_conductivity/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/thermal_conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/thermal_conductivity/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.304032 openpnm-3.2.0/openpnm/models/phase/vapor_pressure/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/vapor_pressure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/vapor_pressure/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/phase/viscosity/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/viscosity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/phase/viscosity/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/ad_dif_conductance/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/ad_dif_conductance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/ad_dif_conductance/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/capillary_pressure/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/capillary_pressure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/capillary_pressure/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/diffusive_conductance/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/diffusive_conductance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/diffusive_conductance/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/electrical_conductance/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/electrical_conductance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/electrical_conductance/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/hydraulic_conductance/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/hydraulic_conductance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/hydraulic_conductance/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/meniscus/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/meniscus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/meniscus/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/multiphase/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/multiphase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/multiphase/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/source_terms/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/source_terms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23165 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/source_terms/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/models/physics/thermal_conductance/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/thermal_conductance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/models/physics/thermal_conductance/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/_bcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/_cubic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/_cubic_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/_delaunay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/_delaunay_voronoi_dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/_fcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36223 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/network/_voronoi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/phase/_air.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/phase/_mercury.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/phase/_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/phase/_phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/phase/_species.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/phase/_water.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.308032 openpnm-3.2.0/openpnm/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/solvers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/solvers/_pardiso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/solvers/_petsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/solvers/_pyamg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/solvers/_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.312032 openpnm-3.2.0/openpnm/topotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/topotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/topotools/_graphtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/topotools/_perctools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44445 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/topotools/_topotools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.312032 openpnm-3.2.0/openpnm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/utils/_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/utils/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/utils/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/utils/_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.312032 openpnm-3.2.0/openpnm/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/visualization/_conduit_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34647 2023-07-25 03:57:13.000000 openpnm-3.2.0/openpnm/visualization/_plottools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:58:12.292032 openpnm-3.2.0/openpnm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-25 03:58:12.000000 openpnm-3.2.0/openpnm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-07-25 03:58:12.000000 openpnm-3.2.0/openpnm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 03:58:12.000000 openpnm-3.2.0/openpnm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 03:58:12.000000 openpnm-3.2.0/openpnm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-25 03:58:12.000000 openpnm-3.2.0/openpnm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 03:58:12.000000 openpnm-3.2.0/openpnm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-25 03:58:12.312032 openpnm-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-25 03:57:13.000000 openpnm-3.2.0/setup.py
```

### Comparing `openpnm-3.1.2/LICENSE` & `openpnm-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/PKG-INFO` & `openpnm-3.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,93 @@
 Metadata-Version: 2.1
 Name: openpnm
-Version: 3.1.2
+Version: 3.2.0
 Summary: A framework for conducting pore network modeling simulations of multiphase transport in porous materials
 Home-page: http://openpnm.org
 Author: OpenPNM Team
 Author-email: jgostick@uwaterloo.ca
 License: UNKNOWN
 Download-URL: https://github.com/PMEAL/OpenPNM/
 Project-URL: Documentation, https://openpnm.org
 Project-URL: Source, https://github.com/PMEAL/OpenPNM
 Project-URL: Tracker, https://github.com/PMEAL/OpenPNM/issues
-Description: [![](https://github.com/PMEAL/OpenPNM/actions/workflows/nightly.yml/badge.svg)](https://github.com/PMEAL/OpenPNM/actions/workflows/nightly.yml)
-        [![](https://codecov.io/gh/PMEAL/OpenPNM/branch/dev/graph/badge.svg)](https://codecov.io/gh/PMEAL/OpenPNM)
-        [![](https://img.shields.io/badge/Documentation-Read-blue.svg)](https://pmeal.github.io/OpenPNM/)
-        [![](https://badge.fury.io/py/openpnm.svg)](https://pypi.python.org/pypi/openpnm)
-        [![](https://anaconda.org/conda-forge/openpnm/badges/installer/conda.svg)](https://anaconda.org/conda-forge/openpnm)
-        
-        -----
-        
-        > VERSION 3.0 of OpenPNM is now out. All the [examples on the website](https://openpnm.org/_examples/index.html) are now using the features and idioms of V3. For a description of the main changes please see our [recent blog post](http://pmeal.com/posts/2022-10-10-notebook-post/). 
-        
-        # Overview of OpenPNM
-        
-        *OpenPNM* is a comprehensive framework for performing pore network simulations of porous materials.
-        
-        ## More Information
-        
-        For more details about the package can be found in the [on-line documentation](https://openpnm.org)
-        
-        ## Installation and Requirements
-        
-        ### Preferred method
-        The preferred way of installing OpenPNM is through [Anaconda Cloud](https://anaconda.org/conda-forge/openpnm) using:
-        
-        ```
-        conda install -c conda-forge openpnm
-        ```
-        
-        ### Alternative method
-        OpenPNM can also be installed from the [Python Package Index](https://pypi.org/project/openpnm/) using:
-        
-        ```
-        pip install openpnm
-        ```
-        
-        However, we don't recommend installing using `pip` since `pypardiso`, which is a blazing fast direct solver, is not available for Windows users who use Python 3.7+.
-        
-        ### For developers
-        For developers who intend to change the source code or contribute to OpenPNM, the source code can be downloaded from [Github](https://github.com/pmeal/OpenPNM/) and installed by running:
-        
-        ```
-        pip install -e 'path/to/downloaded/files'
-        ```
-        
-        The advantage to installing from the source code is that you can edit the files and have access to your changes each time you import *OpenPNM*.
-        
-        OpenPNM requires the *Scipy Stack* (Numpy, Scipy, Matplotlib, etc), which is most conveniently obtained by installing the [Anaconda Distribution](https://conda.io/docs/user-guide/install/download.html).
-        
-        ## Asking Questions and Getting Help
-        
-        Github now has a [Discussions](https://github.com/PMEAL/OpenPNM/discussions) function, which works similarly to [stack overflow](https://www.stackoverflow.com).  Please post your question in the [Q&A category](https://github.com/PMEAL/OpenPNM/discussions?discussions_q=category%3AQ%26A) so devs or users can provide answers, vote on accepted answers, improve on each other's answers, and generally discuss things. Most importantly, all answers are searchable so eventually, once enough questions have been posted and answered, you can find what you're looking for with a simple search.
-        
-        ## Contact
-        
-        OpenPNM is developed by the Porous Materials Engineering and Analysis Lab [(PMEAL)](http://pmeal.com), in the [Department of Chemical Engineering](https://uwaterloo.ca/chemical-engineering/) at the [University of Waterloo](https://uwaterloo.ca/) in Waterloo, Ontario, Canada.
-        
-        The lead developer for this project is Prof. Jeff Gostick (jgostick@gmail.com).
-        
-        ## Acknowledgements
-        
-        OpenPNM is grateful to [CANARIE](https://canarie.ca) for their generous funding over the past few years.  We would also like to acknowledge the support of [NSERC of Canada](https://www.nserc-crsng.gc.ca/) for funding many of the student that have contributed to OpenPNM since it's inception in 2011.
-        
-        ## Citation
-        
-        If you use OpenPNM in a publication, please cite the following paper:
-        
-        > _Gostick et al._ "**OpenPNM: a pore network modeling package.**" Computing in Science & Engineering 18, no. 4 (2016): 60-74.
-        > [doi:10.1109/MCSE.2016.49](https://ieeexplore.ieee.org/document/7478437)
-        
-        Also, we ask that you "star" :star: this repository so we can track the number of users who are interested in this project, which is helpful for securing future grant funding.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![](https://github.com/PMEAL/OpenPNM/actions/workflows/nightly.yml/badge.svg)](https://github.com/PMEAL/OpenPNM/actions/workflows/nightly.yml)
+[![](https://codecov.io/gh/PMEAL/OpenPNM/branch/dev/graph/badge.svg)](https://codecov.io/gh/PMEAL/OpenPNM)
+[![](https://img.shields.io/badge/Documentation-Read-blue.svg)](https://pmeal.github.io/OpenPNM/)
+[![](https://badge.fury.io/py/openpnm.svg)](https://pypi.python.org/pypi/openpnm)
+[![](https://anaconda.org/conda-forge/openpnm/badges/installer/conda.svg)](https://anaconda.org/conda-forge/openpnm)
+
+-----
+
+> VERSION 3.0 of OpenPNM is now out. All the [examples on the website](https://openpnm.org/_examples/index.html) are now using the features and idioms of V3. For a description of the main changes please see our [recent blog post](http://pmeal.com/posts/2022-10-10-notebook-post/). 
+
+# Overview of OpenPNM
+
+*OpenPNM* is a comprehensive framework for performing pore network simulations of porous materials.
+
+## More Information
+
+For more details about the package can be found in the [on-line documentation](https://openpnm.org)
+
+## Installation and Requirements
+
+### Preferred method
+The preferred way of installing OpenPNM is through [Anaconda Cloud](https://anaconda.org/conda-forge/openpnm) using:
+
+```
+conda install -c conda-forge openpnm
+```
+
+### Alternative method
+OpenPNM can also be installed from the [Python Package Index](https://pypi.org/project/openpnm/) using:
+
+```
+pip install openpnm
+```
+
+However, we don't recommend installing using `pip` since `pypardiso`, which is a blazing fast direct solver, is not available for Windows users who use Python 3.7+.
+
+### For developers
+For developers who intend to change the source code or contribute to OpenPNM, the source code can be downloaded from [Github](https://github.com/pmeal/OpenPNM/) and installed by running:
+
+```
+pip install -e 'path/to/downloaded/files'
+```
+
+The advantage to installing from the source code is that you can edit the files and have access to your changes each time you import *OpenPNM*.
+
+OpenPNM requires the *Scipy Stack* (Numpy, Scipy, Matplotlib, etc), which is most conveniently obtained by installing the [Anaconda Distribution](https://conda.io/docs/user-guide/install/download.html).
+
+## Asking Questions and Getting Help
+
+Github now has a [Discussions](https://github.com/PMEAL/OpenPNM/discussions) function, which works similarly to [stack overflow](https://www.stackoverflow.com).  Please post your question in the [Q&A category](https://github.com/PMEAL/OpenPNM/discussions?discussions_q=category%3AQ%26A) so devs or users can provide answers, vote on accepted answers, improve on each other's answers, and generally discuss things. Most importantly, all answers are searchable so eventually, once enough questions have been posted and answered, you can find what you're looking for with a simple search.
+
+## Contact
+
+OpenPNM is developed by the Porous Materials Engineering and Analysis Lab [(PMEAL)](http://pmeal.com), in the [Department of Chemical Engineering](https://uwaterloo.ca/chemical-engineering/) at the [University of Waterloo](https://uwaterloo.ca/) in Waterloo, Ontario, Canada.
+
+The lead developer for this project is Prof. Jeff Gostick (jgostick@gmail.com).
+
+## Acknowledgements
+
+OpenPNM is grateful to [CANARIE](https://canarie.ca) for their generous funding over the past few years.  We would also like to acknowledge the support of [NSERC of Canada](https://www.nserc-crsng.gc.ca/) for funding many of the student that have contributed to OpenPNM since it's inception in 2011.
+
+## Citation
+
+If you use OpenPNM in a publication, please cite the following paper:
+
+> _Gostick et al._ "**OpenPNM: a pore network modeling package.**" Computing in Science & Engineering 18, no. 4 (2016): 60-74.
+> [doi:10.1109/MCSE.2016.49](https://ieeexplore.ieee.org/document/7478437)
+
+Also, we ask that you "star" :star: this repository so we can track the number of users who are interested in this project, which is helpful for securing future grant funding.
+
+
```

### Comparing `openpnm-3.1.2/README.md` & `openpnm-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/__init__.py` & `openpnm-3.2.0/openpnm/__init__.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/__init__.py` & `openpnm-3.2.0/openpnm/_skgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/generators/_bcc.py` & `openpnm-3.2.0/openpnm/_skgraph/generators/_bcc.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/generators/_cubic.py` & `openpnm-3.2.0/openpnm/_skgraph/generators/_cubic.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/generators/_delaunay.py` & `openpnm-3.2.0/openpnm/_skgraph/generators/_delaunay.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import scipy.spatial as sptl
 from openpnm._skgraph.generators import tools
 from openpnm._skgraph.tools import tri_to_am, isoutside
 from openpnm._skgraph.operations import trim_nodes
 
 
-def delaunay(points, shape=[1, 1, 1], reflect=False,
+def delaunay(points, shape=[1, 1, 1], reflect=False, trim=True,
              node_prefix='node', edge_prefix='edge'):
     r"""
     Generate a network based on Delaunay triangulation of random points
 
     Parameters
     ----------
     points : array_like or int
@@ -18,14 +18,17 @@
     shape : array_like
         Indicates the size and shape of the domain
     reflect : boolean, optional (default = ``False``)
         If ``True`` then points are reflected across each face of the domain
         prior to performing the tessellation. These reflected points are
         automatically trimmed.  Enabling this behavior prevents long-range
         connections between surface pores.
+    trim : boolean, optional (default = ``True``)
+        If ``True`` then any points laying outside the domain are removed. This is
+        mostly only useful if ``reflect=True``.
 
     Returns
     -------
     network : dict
         A dictionary containing 'node.coords' and 'edge.conns'
     tri : Delaunay tessellation object
         The Delaunay tessellation object produced by ``scipy.spatial.Delaunay``
@@ -33,11 +36,11 @@
     points = tools.parse_points(points=points, shape=shape, reflect=reflect)
     mask = ~np.all(points == 0, axis=0)
     tri = sptl.Delaunay(points=points[:, mask])
     coo = tri_to_am(tri)
     d = {}
     d[node_prefix+'.coords'] = points
     d[edge_prefix+'.conns'] = np.vstack((coo.row, coo.col)).T
-    if reflect:
+    if trim:
         trim = isoutside(d, shape=shape)
         d = trim_nodes(network=d, inds=np.where(trim)[0])
     return d, tri
```

### Comparing `openpnm-3.1.2/openpnm/_skgraph/generators/_fcc.py` & `openpnm-3.2.0/openpnm/_skgraph/generators/_fcc.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/generators/_gabriel.py` & `openpnm-3.2.0/openpnm/_skgraph/generators/_gabriel.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/generators/_template.py` & `openpnm-3.2.0/openpnm/_skgraph/generators/_template.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/generators/_voronoi.py` & `openpnm-3.2.0/openpnm/_skgraph/generators/_voronoi.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/generators/_voronoi_delaunay_dual.py` & `openpnm-3.2.0/openpnm/_skgraph/generators/_voronoi_delaunay_dual.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/generators/tools/_funcs.py` & `openpnm-3.2.0/openpnm/_skgraph/generators/tools/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/operations/_binary.py` & `openpnm-3.2.0/openpnm/_skgraph/operations/_binary.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/operations/_unary.py` & `openpnm-3.2.0/openpnm/_skgraph/operations/_unary.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,21 +41,21 @@
     # extending in this function occurs on the 1st axis.
     g = network
     node_prefix = tools.get_node_prefix(g)
     coords = np.atleast_2d(new_coords)
     Nnew = coords.shape[0]
     for k, v in g.items():
         if k.startswith(node_prefix):
-            blank = np.repeat(v[:1, ...], Nnew, axis=0)
             dval = None
             for t in settings.missing_values.keys():
                 if v.dtype == t:
                     dval = settings.missing_values[t]
+            blank = np.repeat(v[:1, ...], Nnew, axis=0)*dval
             blank.fill(dval)
-            g[k] = np.concatenate((v, blank), axis=0)
+            g[k] = np.concatenate((v, blank), axis=0).astype(v.dtype)
     # Lastly, overwrite the -Nnew elements of coords with the given values
     g[node_prefix+'.coords'][-Nnew:] = np.array(coords)
     return g
 
 
 def add_edges(network, new_conns):
     r"""
@@ -85,21 +85,21 @@
     # extending in this function occurs on the 1st axis.
     g = network
     edge_prefix = tools.get_edge_prefix(g)
     conns = np.atleast_2d(new_conns)
     Nnew = conns.shape[0]
     for k, v in g.items():
         if k.startswith(edge_prefix):
-            blank = np.repeat(v[:1, ...], Nnew, axis=0)
             dval = None
             for t in settings.missing_values.keys():
                 if v.dtype == t:
                     dval = settings.missing_values[t]
+            blank = np.repeat(v[:1, ...], Nnew, axis=0)*dval
             blank.fill(dval)
-            g[k] = np.concatenate((v, blank), axis=0)
+            g[k] = np.concatenate((v, blank), axis=0).astype(v.dtype)
     # Lastly, overwrite the -Nnew elements of coords with the given values
     g[edge_prefix+'.conns'][-Nnew:] = np.array(conns)
     return g
 
 
 def trim_edges(network, inds):
     r"""
```

### Comparing `openpnm-3.1.2/openpnm/_skgraph/queries/_funcs.py` & `openpnm-3.2.0/openpnm/_skgraph/queries/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/queries/_qupc.py` & `openpnm-3.2.0/openpnm/_skgraph/queries/_qupc.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/simulations/_percolation.py` & `openpnm-3.2.0/openpnm/_skgraph/simulations/_percolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from collections import namedtuple
+
 import numpy as np
 import scipy.sparse as sprs
 from scipy.sparse import csgraph
-from collections import namedtuple
-from openpnm._skgraph.operations import split_edges
 
+from openpnm._skgraph.operations import split_edges
 
 __all__ = [
     'trim_disconnected_clusters',
     'ispercolating',
     'remove_isolated_clusters',
     'bond_percolation',
     'site_percolation',
@@ -112,16 +113,14 @@
 
 
 def mixed_percolation(
     conns,
     occupied_sites,
     occupied_bonds
 ):  # pragma: no cover
-    r"""
-    """
     new_conns = split_edges(conns)[0]
     new_sites = np.hstack((occupied_sites, occupied_bonds))
     s, b = site_percolation(conns=new_conns, occupied_sites=new_sites)
     s_labels = s[:occupied_sites.shape[0]]
     b_labels = s[occupied_sites.shape[0]:]
     return s_labels, b_labels
```

### Comparing `openpnm-3.1.2/openpnm/_skgraph/tools/_coords_transforms.py` & `openpnm-3.2.0/openpnm/_skgraph/tools/_coords_transforms.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/tools/_funcs.py` & `openpnm-3.2.0/openpnm/_skgraph/tools/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/_skgraph/visualization/_funcs.py` & `openpnm-3.2.0/openpnm/_skgraph/visualization/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_advection_diffusion.py` & `openpnm-3.2.0/openpnm/algorithms/_advection_diffusion.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_algorithm.py` & `openpnm-3.2.0/openpnm/algorithms/_algorithm.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_drainage.py` & `openpnm-3.2.0/openpnm/algorithms/_drainage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from collections import namedtuple
+
 import numpy as np
 from tqdm.auto import tqdm
-from collections import namedtuple
-from openpnm.algorithms import Algorithm
-from openpnm.utils import Docorator, TypedSet
+
 from openpnm._skgraph.simulations import (
     bond_percolation,
-    site_percolation,
     find_connected_clusters,
+    site_percolation,
 )
-
+from openpnm.algorithms import Algorithm
+from openpnm.utils import Docorator, TypedSet
 
 docstr = Docorator()
 
 
 __all__ = ['Drainage']
 
 
@@ -37,14 +38,15 @@
     throat_entry_pressure = 'throat.entry_pressure'
     pore_volume = 'pore.volume'
     throat_volume = 'throat.volume'
     variable_props = TypedSet()
 
 
 class Drainage(Algorithm):
+    """A class to simulate drainage."""
 
     def __init__(self, phase, name='drainage_?', **kwargs):
         super().__init__(name=name, **kwargs)
         self.settings._update(DrainageSettings())
         self.settings['phase'] = phase.name
         self['pore.bc.inlet'] = False
         self['pore.bc.outlet'] = False
@@ -269,16 +271,17 @@
         data = pc_curve(np.array(pc), np.array(s))
         return data
 
 
 # %%
 # def run_examples():
 if __name__ == '__main__':
-    import openpnm as op
     import matplotlib.pyplot as plt
+
+    import openpnm as op
     plt.rcParams['figure.facecolor'] = 'darkgrey'
     plt.rcParams['axes.facecolor'] = 'grey'
 
     np.random.seed(0)
     Nx, Ny, Nz = 10, 10, 1
     pn = op.network.Cubic([Nx, Ny, Nz], spacing=1e-5)
     pn.add_model_collection(op.models.collections.geometry.spheres_and_cylinders)
```

### Comparing `openpnm-3.1.2/openpnm/algorithms/_fickian_diffusion.py` & `openpnm-3.2.0/openpnm/algorithms/_fickian_diffusion.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_fourier_conduction.py` & `openpnm-3.2.0/openpnm/algorithms/_fourier_conduction.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_invasion_percolation.py` & `openpnm-3.2.0/openpnm/algorithms/_invasion_percolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-import logging
 import heapq as hq
+import logging
+from collections import namedtuple
+
 import numpy as np
-from numba import njit, jit
+from numba import jit, njit
 from tqdm.auto import tqdm
-from collections import namedtuple
-from openpnm.utils import Docorator
-from openpnm.algorithms import Algorithm
-from openpnm._skgraph.simulations import (
-    bond_percolation,
-    site_percolation,
-)
-from openpnm._skgraph.queries import (
-    qupc_initialize,
-    qupc_update,
-    qupc_reduce,
-)
 
+from openpnm._skgraph.queries import qupc_initialize, qupc_reduce, qupc_update
+from openpnm._skgraph.simulations import bond_percolation, site_percolation
+from openpnm.algorithms import Algorithm
+from openpnm.utils import Docorator
 
 __all__ = [
     'InvasionPercolation',
 ]
 
 
 logger = logging.getLogger(__name__)
@@ -350,22 +344,22 @@
         self['pore.invasion_sequence'][self['pore.trapped']] = -1
         self['throat.invasion_sequence'][self['throat.trapped']] = -1
         # Set any residual pores within trapped clusters back to untrapped
         # self['pore.trapped'][self['pore.residual']] = False
         # self['throat.trapped'][self['throat.residual']] = False
 
 
-@jit
-def _find_trapped_pores(inv_seq, indices, indptr, outlets):  # pragma: no cover
+@jit(forceobj=True)
+def _find_trapped_pores(inv_seq, indices, indptr, outlets):
     Np = len(inv_seq)
     sorted_seq = np.vstack((inv_seq.astype(np.int_), np.arange(Np, dtype=np.int_))).T
     sorted_seq = sorted_seq[sorted_seq[:, 0].argsort()][::-1]
     cluster = -np.ones(Np, dtype=np.int_)
-    trapped_pores = np.zeros(Np, dtype=np.bool_)
-    trapped_clusters = np.zeros(Np, dtype=np.bool_)
+    trapped_pores = np.zeros(Np, dtype=bool)
+    trapped_clusters = np.zeros(Np, dtype=bool)
     # cluster_map = qupc_initialize(Np)
     cluster_map = np.arange(Np, dtype=np.int_)
     next_cluster_num = 0
     i = -1
     for step, pore in sorted_seq:
         i += 1
         step, pore = sorted_seq[i, :]
@@ -467,17 +461,18 @@
         if len(queue) == 0:
             break
     return t_inv, p_inv, p_inv_t
 
 
 # %%
 if __name__ == '__main__':
-    import openpnm as op
     import matplotlib.pyplot as plt
 
+    import openpnm as op
+
     np.random.seed(0)
     Nx, Ny, Nz = 25, 25, 1
     pn = op.network.Cubic(shape=[Nx, Ny, Nz], spacing=1e-4)
     pn.add_model_collection(op.models.collections.geometry.spheres_and_cylinders)
     pn.regenerate_models()
     pn['pore.volume@left'] = 0.0
     # op.topotools.trim(pn, pores=[380, 395])
```

### Comparing `openpnm-3.1.2/openpnm/algorithms/_ohmic_conduction.py` & `openpnm-3.2.0/openpnm/algorithms/_ohmic_conduction.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_reactive_transport.py` & `openpnm-3.2.0/openpnm/algorithms/_reactive_transport.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_solution.py` & `openpnm-3.2.0/openpnm/algorithms/_solution.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_stokes_flow.py` & `openpnm-3.2.0/openpnm/algorithms/_stokes_flow.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_transient_advection_diffusion.py` & `openpnm-3.2.0/openpnm/algorithms/_transient_advection_diffusion.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_transient_reactive_transport.py` & `openpnm-3.2.0/openpnm/algorithms/_transient_reactive_transport.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/algorithms/_transport.py` & `openpnm-3.2.0/openpnm/algorithms/_transport.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/contrib/_multiphase.py` & `openpnm-3.2.0/openpnm/contrib/_multiphase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
+
 import numpy as np
+
 import openpnm.models.misc as misc
 from openpnm.phase import Phase as Phase
 from openpnm.utils import Docorator, TypedSet
 
-
 logger = logging.getLogger(__name__)
 docstr = Docorator()
 
 
 __all__ = [
     'MultiPhase',
     'multiphase_diffusion',
@@ -299,15 +300,15 @@
 
 def multiphase_diffusion(phase,
                          pore_diffusivity="pore.diffusivity",
                          throat_diffusivity="throat.diffusivity",
                          size_factors="throat.diffusive_size_factors",
                          partition_coef_global="throat.partition_coef.global"):
     r"""
-    Calculates the diffusive conductance of conduits in network.
+    Calculates the diffusive conductance of conduits for multiphase systems.
 
     Parameters
     ----------
     %(phase)s
     pore_diffusivity : str
         %(dict_blurb)s pore diffusivity
     throat_diffusivity : str
```

### Comparing `openpnm-3.1.2/openpnm/contrib/_transient_multiphysics.py` & `openpnm-3.2.0/openpnm/contrib/_transient_multiphysics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
+
 import numpy as np
-from openpnm.utils import Docorator
-from openpnm.integrators import ScipyRK45
+
 from openpnm.algorithms import Algorithm
 from openpnm.algorithms._solution import SolutionContainer, TransientSolution
-
+from openpnm.integrators import ScipyRK45
+from openpnm.utils import Docorator
 
 logger = logging.getLogger(__name__)
 docstr = Docorator()
 
 
 __all__ = [
     'TransientMultiPhysics',
@@ -42,15 +43,15 @@
         self._algs = algorithms
 
     def run(self, x0, tspan, saveat=None, integrator=None):
         """
         Runs all of the transient algorithms simultaneoulsy and returns the
         solution.
 
-        Parameters steal from transient reactive transport
+        Parameters
         ----------
         x0 : ndarray or float
             Array (or scalar) containing initial condition values.
         tspan : array_like
             Tuple (or array) containing the integration time span.
         saveat : array_like or float, optional
             If an array is passed, it signifies the time points at which
```

### Comparing `openpnm-3.1.2/openpnm/core/__init__.py` & `openpnm-3.2.0/openpnm/core/__init__.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/core/_base2.py` & `openpnm-3.2.0/openpnm/core/_base2.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,17 @@
 
         # Intercept parameters
         if key.startswith('param'):
             _, key = key.split('.', 1)
             self._params[key] = value
             return
 
+        if not (key.startswith('pore.') or key.startswith('throat.')):
+            raise Exception("All dict names must start with pore, throat, or param")
+
         # Intercept @ symbol
         if '@' in key:
             element, prop = key.split('@')[0].split('.', 1)
             domain = key.split('@')[1]
             locs = super().__getitem__(f'{element}.{domain}')
             try:
                 vals = self[f'{element}.{prop}']
@@ -189,27 +192,51 @@
             super().__delitem__(key)
         except KeyError:
             d = self[key]  # If key is a nested dict, get all values
             for item in d.keys():
                 super().__delitem__(f'{key}.{item}')
 
     def pop(self, *args):
+        r"""
+        """
         v = super().pop(*args)
         if v is None:
             try:
                 d = self[args[0]]
                 v = {}
                 for item in d.keys():
                     key = f'{args[0]}.{item}'
                     v[key] = super().pop(key)
             except KeyError:
                 pass
         return v
 
     def clear(self, mode=None):
+        r"""
+        Clears or deletes certain things from object. If no arguments are provided
+        it defaults to the normal `dict` behavior.
+
+        Parameters
+        ----------
+        mode : str
+            Controls which things are to be deleted. Options are:
+
+            =========== ============================================================
+            `mode`        Description
+            =========== ============================================================
+            'props'     Deletes all pore and throat properties (i.e numerical data)
+                        in the object's dictionary (except 'pore.coords' and
+                        'throat.conns' if it is a network object).
+            'labels'    Deletes all labels (i.e. boolean data) in the object's
+                        dictionary.
+            'models'    Delete are pore and throat properties that were produced
+                        by a pore-scale model.
+            =========== ============================================================
+
+        """
         if mode is None:
             super().clear()
         else:
             if isinstance(mode, str):
                 mode = [mode]
             if 'props' in mode:
                 for item in self.props():
@@ -305,18 +332,28 @@
     def _del_settings(self):
         self._settings = None
 
     settings = property(fget=_get_settings, fset=_set_settings, fdel=_del_settings)
 
     @property
     def network(self):
+        r"""
+        Shortcut to retrieve a handle to the network object associated with the
+        calling object
+        """
         return self.project.network
 
     @property
     def params(self):
+        r"""
+        This attribute stores 'scalar' data that can be used by pore-scale models.
+        For instance, if a model calls for `temperature` you can specify
+        `pore.temperature` if every pore might have a different value, or
+        `param.temperature` if a single value prevails everywhere.
+        """
         return self._params
 
     def _count(self, element):
         if element == 'pore':
             try:
                 return self['pore.coords'].shape[0]
             except KeyError:
@@ -329,26 +366,38 @@
             except KeyError:
                 for k, v in self.items():
                     if k.startswith('throat.'):
                         return v.shape[0]
 
     @property
     def Nt(self):
+        r"""
+        Shortcut to retrieve the number of throats in the domain
+        """
         return self._count('throat')
 
     @property
     def Np(self):
+        r"""
+        Shortcut to retrieve the number of pores in the domain
+        """
         return self._count('pore')
 
     @property
     def Ts(self):
+        r"""
+        Shortcut to retrieve the indices of *all* throats
+        """
         return np.arange(self._count('throat'))
 
     @property
     def Ps(self):
+        r"""
+        Shortcut to retrieve the indices of *all* pores
+        """
         return np.arange(self._count('pore'))
 
     def _tomask(self, element, indices):
         return self.to_mask(**{element+'s': indices})
 
     def to_mask(self, pores=None, throats=None):
         r"""
```

### Comparing `openpnm-3.1.2/openpnm/core/_mixins.py` & `openpnm-3.2.0/openpnm/core/_mixins.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/core/_models.py` & `openpnm-3.2.0/openpnm/core/_models.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/integrators/_scipy.py` & `openpnm-3.2.0/openpnm/integrators/_scipy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from scipy.integrate import solve_ivp
-from openpnm.integrators import Integrator
+
 from openpnm.algorithms._solution import TransientSolution
+from openpnm.integrators import Integrator
 
 __all__ = ['ScipyRK45']
 
 
 class ScipyRK45(Integrator):
-    """Brief description of 'ScipyRK45'"""
+    """Integrator class based on SciPy's implementation of RK45"""
 
     def __init__(self, atol=1e-6, rtol=1e-6, verbose=False, linsolver=None):
         self.atol = atol
         self.rtol = rtol
         self.verbose = verbose
         self.linsolver = linsolver
```

### Comparing `openpnm-3.1.2/openpnm/io/__init__.py` & `openpnm-3.2.0/openpnm/io/__init__.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_comsol.py` & `openpnm-3.2.0/openpnm/io/_comsol.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_csv.py` & `openpnm-3.2.0/openpnm/io/_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from openpnm.io._pandas import project_to_pandas, network_to_pandas
-from openpnm.io import _parse_filename
-from openpnm.utils import Project
-from pandas import read_table
 import re
+
 import numpy as np
+from pandas import read_table
+
+from openpnm.io import _parse_filename
+from openpnm.io._pandas import network_to_pandas, project_to_pandas
+from openpnm.utils import Project
 
 
 def project_to_csv(project, filename=''):
     r"""
     Save all the pore and throat data on the Network and Phase objects to a CSV
     file
 
@@ -23,24 +25,26 @@
     if filename == '':
         filename = project.name
     fname = _parse_filename(filename=filename, ext='csv')
     df.to_csv(fname, index=False)
 
 
 def network_to_csv(network, filename=''):
+    """Exports a network to a CSV file."""
     proj = Project()
     proj.append(network)
     df = network_to_pandas(network=network, join=True, delim='.')
     if filename == '':
         filename = network.name
     fname = _parse_filename(filename=filename, ext='csv')
     df.to_csv(fname, index=False)
 
 
 def network_from_csv(filename):
+    """Loads a network from a CSV file."""
     from openpnm.network import Network
     fname = _parse_filename(filename=filename, ext='csv')
 
     a = read_table(filepath_or_buffer=fname,
                    sep=',',
                    skipinitialspace=True,
                    index_col=False,
```

### Comparing `openpnm-3.1.2/openpnm/io/_dict.py` & `openpnm-3.2.0/openpnm/io/_dict.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_hdf5.py` & `openpnm-3.2.0/openpnm/io/_hdf5.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_jsongraph.py` & `openpnm-3.2.0/openpnm/io/_jsongraph.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_marock.py` & `openpnm-3.2.0/openpnm/io/_marock.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_networkx.py` & `openpnm-3.2.0/openpnm/io/_networkx.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_pandas.py` & `openpnm-3.2.0/openpnm/io/_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 from pandas import DataFrame
+
 from openpnm.io import project_to_dict
-from openpnm.utils import sanitize_dict, Project
+from openpnm.utils import Project, sanitize_dict
 
 
 def network_to_pandas(network, join=False, delim='.'):
+    """Converts network data to a Pandas DataFrame."""
     proj = Project()
     proj.append(network)
     # Initialize pore and throat data dictionary using Dict class
     pdata = project_to_dict(project=proj, element='pore',
                             flatten=True, categorize_by=[], delim=delim)
     tdata = project_to_dict(project=proj, element='throat',
                             flatten=True, categorize_by=[], delim=delim)
```

### Comparing `openpnm-3.1.2/openpnm/io/_paraview.py` & `openpnm-3.2.0/openpnm/io/_paraview.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_pergeos.py` & `openpnm-3.2.0/openpnm/io/_pergeos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
+
 import numpy as np
+
 from openpnm.io import _parse_filename
 from openpnm.network import Network
 
-
 logger = logging.getLogger(__name__)
 
 
 def network_to_pergeos(network, filename=''):
-    r"""
-    """
     # avoid printing truncated array
     np.set_printoptions(threshold=np.inf)
 
     # Ensure network has PerGeos' expected properties
     if 'pore.EqRadius' not in network.props():
         try:
             network['pore.EqRadius'] = network['pore.diameter']/2
@@ -110,14 +109,15 @@
     fname = _parse_filename(filename=filename, ext='am')
     with open(fname, 'w') as f:
         f.write(''.join(s))
 
 
 def network_from_pergeos(filename):
     r"""
+    Loads a network from a PerGeos file.
 
     Notes
     -----
     PerGeos is the format used by the Avizo software. See `here for more
     details <https://cases.pergeos.com/>`_.
     """
     net = {}
```

### Comparing `openpnm-3.1.2/openpnm/io/_porespy.py` & `openpnm-3.2.0/openpnm/io/_porespy.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_salome.py` & `openpnm-3.2.0/openpnm/io/_salome.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_statoil.py` & `openpnm-3.2.0/openpnm/io/_statoil.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_stl.py` & `openpnm-3.2.0/openpnm/io/_stl.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_utils.py` & `openpnm-3.2.0/openpnm/io/_utils.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/io/_vtk.py` & `openpnm-3.2.0/openpnm/io/_vtk.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     point_data_node = piece_node.find("PointData")
     cell_data_node = piece_node.find("CellData")
     for key in key_list:
         array = am[key]
         if array.dtype == "O":
             logger.warning(key + " has dtype object," + " will not write to file")
         else:
-            if array.dtype == np.bool:
+            if array.dtype == bool:
                 array = array.astype(int)
             if np.any(np.isnan(array)):
                 if fill_nans is None:
                     logger.warning(key + " has nans," + " will not write to file")
                     continue
                 else:
                     array[np.isnan(array)] = fill_nans
```

### Comparing `openpnm-3.1.2/openpnm/io/_xdmf.py` & `openpnm-3.2.0/openpnm/io/_xdmf.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/_doctxt.py` & `openpnm-3.2.0/openpnm/models/_doctxt.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/geometry/circles_and_rectangles.py` & `openpnm-3.2.0/openpnm/models/collections/geometry/circles_and_rectangles.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/geometry/cones_and_cylinders.py` & `openpnm-3.2.0/openpnm/models/collections/geometry/cones_and_cylinders.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/geometry/cubes_and_cuboids.py` & `openpnm-3.2.0/openpnm/models/collections/geometry/cubes_and_cuboids.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/geometry/pyramids_and_cuboids.py` & `openpnm-3.2.0/openpnm/models/collections/geometry/pyramids_and_cuboids.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/geometry/spheres_and_cylinders.py` & `openpnm-3.2.0/openpnm/models/collections/geometry/spheres_and_cylinders.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/geometry/squares_and_rectangles.py` & `openpnm-3.2.0/openpnm/models/collections/geometry/squares_and_rectangles.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/geometry/trapezoids_and_rectangles.py` & `openpnm-3.2.0/openpnm/models/collections/geometry/trapezoids_and_rectangles.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/phase/air.py` & `openpnm-3.2.0/openpnm/models/collections/phase/air.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/phase/gas.py` & `openpnm-3.2.0/openpnm/models/collections/phase/gas.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/phase/liquid.py` & `openpnm-3.2.0/openpnm/models/collections/phase/liquid.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/phase/mercury.py` & `openpnm-3.2.0/openpnm/models/collections/phase/mercury.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/phase/water.py` & `openpnm-3.2.0/openpnm/models/collections/phase/water.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/collections/physics/standard.py` & `openpnm-3.2.0/openpnm/models/collections/physics/standard.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/__init__.py` & `openpnm-3.2.0/openpnm/models/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/_geodocs.py` & `openpnm-3.2.0/openpnm/models/geometry/_geodocs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/conduit_lengths/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/conduit_lengths/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/diffusive_size_factors/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/diffusive_size_factors/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/hydraulic_size_factors/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/hydraulic_size_factors/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/pore_cross_sectional_area/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/pore_cross_sectional_area/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/pore_seed/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/pore_seed/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/pore_size/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/pore_size/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/pore_surface_area/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/pore_surface_area/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/pore_volume/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/pore_volume/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_capillary_shape_factor/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_capillary_shape_factor/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_cross_sectional_area/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_cross_sectional_area/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_endpoints/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_endpoints/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_length/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_length/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_perimeter/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_perimeter/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_seed/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_seed/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_size/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_size/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_surface_area/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_surface_area/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_vector/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_vector/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/geometry/throat_volume/_funcs.py` & `openpnm-3.2.0/openpnm/models/geometry/throat_volume/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/misc/__init__.py` & `openpnm-3.2.0/openpnm/models/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/misc/_basic_math.py` & `openpnm-3.2.0/openpnm/models/misc/_basic_math.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/misc/_neighbor_lookups.py` & `openpnm-3.2.0/openpnm/models/misc/_neighbor_lookups.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/misc/_simple_equations.py` & `openpnm-3.2.0/openpnm/models/misc/_simple_equations.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/misc/_statistical_distributions.py` & `openpnm-3.2.0/openpnm/models/misc/_statistical_distributions.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,32 +110,37 @@
     loc = mean if mean is not None else loc
     seeds = network[seeds]
     value = spts.norm.ppf(q=seeds, scale=scale, loc=loc)
     return value
 
 
 @_doctxt
-def generic_distribution(network, seeds, func):
+def generic_distribution(network, seeds, func, **kwargs):
     r"""
-    Accepts an 'rv_frozen' object from the Scipy.stats submodule and returns
+    Accepts an object from the Scipy.stats submodule and returns
     values from the distribution for the given seeds
 
-    This uses the ``ppf`` method of the stats object
+
 
     Parameters
     ----------
     %(network)s
     seeds : str (dict key)
         %(dict_blurb) seed
     func : object
-        A 'rv_frozen' object from the scipy.stats library with all of the
-        parameters pre-specified.
+        An object from the scipy.stats library. Can be a 'frozen' object, where all
+        the parameters were specified upon creation, or a handle to an unintialized
+        object. In the latter case the parameters for the distribution should be
+        provided as keyword arguments.
 
     Returns
     -------
+    values : ndarray
+        An ndarray of either Np or Nt length, with values taken from the supplied
+        distribution.
 
     Examples
     --------
     The following code illustrates the process of obtaining a 'frozen' Scipy
     stats object and adding it as a model:
 
     .. plot::
@@ -157,14 +162,16 @@
                     func=stats_obj)
 
        plt.hist(stats_obj.ppf(q=numpy.random.rand(1000)), bins=50)
 
        plt.show()
 
     """
+    if hasattr(func, 'freeze'):
+        func = func.freeze(**kwargs)
     seeds = network[seeds]
     value = func.ppf(seeds)
     return value
 
 
 @_doctxt
 def random(network, element, seed=None, num_range=[0, 1]):
```

### Comparing `openpnm-3.1.2/openpnm/models/network/_health.py` & `openpnm-3.2.0/openpnm/models/network/_health.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/network/_topology.py` & `openpnm-3.2.0/openpnm/models/network/_topology.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/__init__.py` & `openpnm-3.2.0/openpnm/models/phase/__init__.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/_phasedocs.py` & `openpnm-3.2.0/openpnm/models/phase/_phasedocs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from matplotlib.docstring import Substitution
 
-
 __all__ = [
     '_phasedocs',
 ]
 
 
 _phasedocs = Substitution(
     phase=
```

### Comparing `openpnm-3.1.2/openpnm/models/phase/critical_props/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/critical_props/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/density/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/density/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/diffusivity/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/diffusivity/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/heat_capacity/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/heat_capacity/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/misc/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/misc/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/mixtures/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/mixtures/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/partition_coefficient/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/partition_coefficient/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/surface_tension/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/surface_tension/_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from openpnm.models.phase import _phasedocs
 
+from openpnm.models.phase import _phasedocs
 
 __all__ = [
     "water_correlation",
     "liquid_pure_bb",
     "liquid_mixture_wsd",
 ]
 
@@ -113,20 +113,22 @@
     r"""
     Computes the surface tension of a liqiud mixture with its own vapor using
     the correlation in [1]
 
     Parameters
     ----------
     %(phase)s
-    %(sigmas)s
     %(rhos)s
     %(MWs)s
+    %(sigmas)s
 
     Returns
     -------
+    sigma : ndarray
+        A numpy ndarray containing surface tension values
 
     References
     ----------
     [1] Winterfeld, Scriven, and Davis
 
     """
     sigmas = phase.get_comp_vals(sigmas)
```

### Comparing `openpnm-3.1.2/openpnm/models/phase/thermal_conductivity/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/thermal_conductivity/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/vapor_pressure/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/vapor_pressure/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/phase/viscosity/_funcs.py` & `openpnm-3.2.0/openpnm/models/phase/viscosity/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/_utils.py` & `openpnm-3.2.0/openpnm/models/physics/_utils.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/ad_dif_conductance/_funcs.py` & `openpnm-3.2.0/openpnm/models/physics/ad_dif_conductance/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/capillary_pressure/_funcs.py` & `openpnm-3.2.0/openpnm/models/physics/capillary_pressure/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/diffusive_conductance/_funcs.py` & `openpnm-3.2.0/openpnm/models/physics/diffusive_conductance/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/electrical_conductance/_funcs.py` & `openpnm-3.2.0/openpnm/models/physics/electrical_conductance/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/hydraulic_conductance/_funcs.py` & `openpnm-3.2.0/openpnm/models/physics/hydraulic_conductance/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/meniscus/_funcs.py` & `openpnm-3.2.0/openpnm/models/physics/meniscus/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/multiphase/_funcs.py` & `openpnm-3.2.0/openpnm/models/physics/multiphase/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/source_terms/_funcs.py` & `openpnm-3.2.0/openpnm/models/physics/source_terms/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/models/physics/thermal_conductance/_funcs.py` & `openpnm-3.2.0/openpnm/models/physics/thermal_conductance/_funcs.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/network/_bcc.py` & `openpnm-3.2.0/openpnm/network/_bcc.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/network/_cubic.py` & `openpnm-3.2.0/openpnm/network/_cubic.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
     def __init__(self, shape, spacing=[1, 1, 1], connectivity=6, **kwargs):
         super().__init__(**kwargs)
         net = skgr.generators.cubic(shape=shape, spacing=spacing,
                                     connectivity=connectivity,
                                     node_prefix='pore', edge_prefix='throat')
         self.update(net)
+        self._post_init()
         self["pore.surface"] = skgr.tools.find_surface_nodes_cubic(self)
         Ps = self["pore.surface"]
         self["throat.surface"] = np.all(Ps[self["throat.conns"]], axis=1)
         self.update(skgr.generators.tools.label_faces_cubic(self))
 
     def add_boundary_pores(self, labels=["top", "bottom", "front",
                                          "back", "left", "right"],
```

### Comparing `openpnm-3.1.2/openpnm/network/_cubic_template.py` & `openpnm-3.2.0/openpnm/network/_cubic_template.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/network/_delaunay.py` & `openpnm-3.2.0/openpnm/network/_delaunay.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,22 @@
         ========== ============================================================
         shape      result
         ========== ============================================================
         [x, y, z]  A 3D cubic domain of dimension x, y and z
         [x, y, 0]  A 2D square domain of size x by y
         ========== ============================================================
 
-    trim : bool, optional
-        If ``True`` (default) then all vertices laying outside the domain will
-        be removed. This is only useful if ``reflect=True``.
     reflect : bool, optional
-        If ``True`` (default) then the base points will be reflected across
+        If ``True`` then the base points will be reflected across
         all the faces of the domain prior to performing the tessellation. This
         feature is best combined with ``trim=True`` to prevent unreasonably long
         connections between points on the surfaces.
+    trim : bool, optional
+        If ``True`` (default) then all vertices laying outside the domain will
+        be removed. This is only useful if ``reflect=True``.
 
     %(Network.parameters)s
 
     Notes
     -----
     It is also possible to generate circular ``[r, 0]``, cylindrical ``[r, z]``, and
     spherical domains ``[r]``, but this feature does not quite work as desired.
@@ -51,11 +51,14 @@
 
     """
 
     def __init__(self, shape, points, reflect=True, trim=True, **kwargs):
         super().__init__(**kwargs)
         net, tri = delaunay(points=points,
                             shape=shape,
+                            reflect=reflect,
+                            trim=trim,
                             node_prefix='pore',
                             edge_prefix='throat')
         self.update(net)
+        self._post_init()
         self.tri = tri
```

### Comparing `openpnm-3.1.2/openpnm/network/_delaunay_voronoi_dual.py` & `openpnm-3.2.0/openpnm/network/_delaunay_voronoi_dual.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,21 +26,23 @@
         shape      result
         ========== ============================================================
         [x, y, z]  A 3D cubic domain of dimension x, y and z
         [x, y, 0]  A 2D square domain of size x by y
         ========== ============================================================
 
     trim : bool, optional
-        If ``True`` (default) then all vertices laying outside the domain will
+        If ``True`` then all vertices laying outside the domain will
         be removed. This is only useful if ``reflect=True``.
     reflect : bool, optional
-        If ``True`` (default) then the base points will be reflected across
+        If ``True`` then the base points will be reflected across
         all the faces of the domain prior to performing the tessellation. This
-        feature is best combined with ``trim=True`` to prevent unreasonably long
-        connections between points on the surfaces.
+        feature is best combined with ``trim=True``.
+    relaxation : int
+        The number of time to iteratively relax the base points by moving them to
+        the centroid of their respective Voronoi hulls. The default it 0.
 
     %(Network.parameters)s
 
     Notes
     -----
     A Delaunay tessellation is performed on a set of base points then the
     corresponding Voronoi diagram is generated.  Finally, each Delaunay node
@@ -48,22 +50,33 @@
     between the two networks.
 
     All pores and throats are labelled according to their network (i.e.
     'pore.delaunay'), so they can be each assigned to a different Geometry.
 
     """
 
-    def __init__(self, shape, points, trim=True, reflect=True, **kwargs):
+    def __init__(
+        self,
+        shape,
+        points,
+        trim=True,
+        reflect=True,
+        relaxation=0,
+        **kwargs
+    ):
         super().__init__(**kwargs)
         net, vor, tri = voronoi_delaunay_dual(shape=shape,
                                               points=points,
                                               trim=trim,
+                                              reflect=reflect,
+                                              relaxation=relaxation,
                                               node_prefix='pore',
                                               edge_prefix='throat')
         self.update(net)
+        self._post_init()
         self.vor = vor
         self.tri = tri
 
     def find_throat_facets(self, throats=None):
         r"""
         Finds the indicies of the Voronoi nodes that define the facet or
         ridge between the Delaunay nodes connected by the given throat.
```

### Comparing `openpnm-3.1.2/openpnm/network/_demo.py` & `openpnm-3.2.0/openpnm/network/_demo.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/network/_fcc.py` & `openpnm-3.2.0/openpnm/network/_fcc.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,28 +46,27 @@
         shape = np.array(shape)
         if np.any(shape < 2):
             raise Exception('FCC lattice networks must have at least 2 '
                             'pores in all directions')
         net = fcc(shape=shape, spacing=spacing,
                   node_prefix='pore', edge_prefix='throat')
         self.update(net)
-        # Deal with labels
-        Ts = self.find_neighbor_throats(pores=self.pores('corner'),
-                                        mode='xnor')
-        self['throat.corner_to_corner'] = False
-        self['throat.corner_to_corner'][Ts] = True
-        Ts = self.find_neighbor_throats(pores=self.pores('face'))
-        self['throat.corner_to_face'] = False
-        self['throat.corner_to_face'][Ts] = True
+        # Add labels
+        Ts1 = np.all(self['pore.corner'][self.conns], axis=1)
+        self['throat.corner_to_corner'] = Ts1
+        Ts2 = np.all(self['pore.face'][self.conns], axis=1)
+        self['throat.face_to_face'] = Ts2
+        self['throat.corner_to_face'] = ~(Ts1 + Ts2)
 
-        # Finally scale network to specified spacing
         topotools.label_faces(self)
-        Ps = self.pores(['left', 'right', 'top', 'bottom', 'front', 'back'])
+        Ps = self.pores(['xmin', 'xmax', 'ymin', 'ymax', 'zmin', 'zmax'])
         Ps = self.to_mask(pores=Ps)
         self['pore.surface'] = Ps
+
+        # Finally scale network to specified spacing
         self['pore.coords'] *= np.array(spacing)
 
     def add_boundary_pores(self, labels, spacing):
         r"""
         Add boundary pores to the specified faces of the network
 
         Pores are offset from the faces by 1/2 of the given ``spacing``,
```

### Comparing `openpnm-3.1.2/openpnm/network/_network.py` & `openpnm-3.2.0/openpnm/network/_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,21 @@
                        regen_mode='deferred',
                        domain='all')
         self.add_model(propname='throat.spacing',
                        model=mods.pore_to_pore_distance,
                        regen_mode='deferred',
                        domain='all')
 
+    def _post_init(self, *args, **kwargs):
+        # A collection of functions to run after initialization of a network
+        topotools.label_faces(self, label=None)
+        drop = ['pore.left', 'pore.right', 'pore.front', 'pore.back',
+                'pore.bottom', 'pore.top']
+        [self.pop(item) for item in list(self.keys()) if item in drop]
+
     def __setitem__(self, key, value):
         if key == 'throat.conns':
             if np.any(value[:, 0] > value[:, 1]):
                 logger.warning('Converting throat.conns to be upper triangular')
                 value = np.sort(value, axis=1)
         super().__setitem__(key, value)
 
@@ -819,14 +826,69 @@
                 temp = []
                 for item in Ps_within_r:
                     temp.append(np.array(item, dtype=np.int64)[mask[item]])
                 Pn = temp
         return Pn
 
     @property
+    def info(self):
+        hr = '―' * 78
+        errmsg = '--------- ! --------- ! ---------\n'
+        pad = 45
+        lines = hr + '\n'
+        # ---
+        lines += 'Number of pores | throats: '.ljust(pad)
+        lines += f"{self.Np} | {self.Nt} \n"
+        # ---
+        lines += 'Pore Coordination (min | mean | max): '.ljust(pad)
+        try:
+            x = self['pore.coordination_number']
+            lines += f"{x.min():.3E} | {x.mean():.3E} | {x.max():.3E} \n"
+        except KeyError:
+            lines += errmsg
+        # ---
+        lines += 'Pore Diameter (min | mean | max): '.ljust(pad)
+        try:
+            x = self['pore.diameter']
+            lines += f"{x.min():.3E} | {x.mean():.3E} | {x.max():.3E} \n"
+        except KeyError:
+            lines += errmsg
+        # ---
+        lines += 'Pore Spacing (min | mean | max): '.ljust(pad)
+        try:
+            x = self['throat.spacing']
+            lines += f"{x.min():.3E} | {x.mean():.3E} | {x.max():.3E} \n"
+        except KeyError:
+            lines += errmsg
+        # ---
+        lines += 'Throat Diameter (min | mean | max): '.ljust(pad)
+        try:
+            x = self['throat.diameter']
+            lines += f"{x.min():.3E} | {x.mean():.3E} | {x.max():.3E} \n"
+        except KeyError:
+            lines += errmsg
+        # ---
+        lines += 'Throat Length (min | mean | max): '.ljust(pad)
+        try:
+            x = self['throat.length']
+            lines += f"{x.min():.3E} | {x.mean():.3E} | {x.max():.3E} \n"
+        except KeyError:
+            lines += errmsg
+        # ---
+        lines += 'Throat Volume (min | mean | max): '.ljust(pad)
+        try:
+            x = self['throat.volume']
+            lines += f"{x.min():.3E} | {x.mean():.3E} | {x.max():.3E} \n"
+        except KeyError:
+            lines += errmsg
+        # ---
+        lines += hr
+        print(lines)
+
+    @property
     def conns(self):
         r"""Returns the connectivity matrix of the network."""
         return self['throat.conns']
 
     @property
     def coords(self):
         r"""Returns the list of pore coordinates of the network."""
```

### Comparing `openpnm-3.1.2/openpnm/network/_voronoi.py` & `openpnm-3.2.0/openpnm/network/_voronoi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from openpnm.network import Network
 from openpnm.utils import Docorator
+from openpnm.topotools import label_faces
 from openpnm._skgraph.generators import voronoi
 
 
 docstr = Docorator()
 __all__ = ['Voronoi']
 
 
@@ -26,21 +27,24 @@
         shape      result
         ========== ============================================================
         [x, y, z]  A 3D cubic domain of dimension x, y and z
         [x, y, 0]  A 2D square domain of size x by y
         ========== ============================================================
 
     trim : bool, optional
-        If ``True`` (default) then all Voronoi vertices laying outside the domain
+        If ``True`` then all Voronoi vertices laying outside the domain
         will be removed.
     reflect : bool, optional
-        If ``True`` (default) then the base points will be reflected across
+        If ``True`` then the base points will be reflected across
         all the faces of the domain prior to performing the tessellation. This
         feature is best combined with ``trim=True`` to make nice flat faces
         on all sides of the domain.
+    relaxation : int
+        The number of time to iteratively relax the base points by moving them to
+        the centroid of their respective Voronoi hulls. The default it 0.
 
     %(Network.parameters)s
 
     Notes
     -----
     These points are used by the Voronoi tessellation, meaning these points will
     each lie in the center of a Voronoi cell, so they will not be the pore centers.
@@ -53,16 +57,27 @@
     conducted in cartesian coordinates, so the circular and spherical surfaces
     have artifacts. Scipy recently added the ability to do tessellations on
     spherical surfaces, for geological applications, but this is not flexible
     enough, yet.
 
     """
 
-    def __init__(self, shape, points, trim=True, reflect=True, **kwargs):
+    def __init__(
+        self,
+        shape,
+        points,
+        trim=True,
+        reflect=True,
+        relaxation=0,
+        **kwargs
+    ):
         super().__init__(**kwargs)
         net, vor = voronoi(points=points,
                            shape=shape,
                            trim=trim,
+                           reflect=reflect,
+                           relaxation=relaxation,
                            node_prefix='pore',
                            edge_prefix='throat')
         self.update(net)
+        self._post_init()
         self.vor = vor
```

### Comparing `openpnm-3.1.2/openpnm/phase/__init__.py` & `openpnm-3.2.0/openpnm/phase/__init__.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/phase/_air.py` & `openpnm-3.2.0/openpnm/phase/_air.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/phase/_mercury.py` & `openpnm-3.2.0/openpnm/phase/_mercury.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/phase/_mixture.py` & `openpnm-3.2.0/openpnm/phase/_mixture.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-import numpy as np
 import logging
-from openpnm.phase import Phase
-from openpnm.models.phase.mixtures import mole_summation
-from openpnm.models.collections.phase import standard_liquid_mixture
-from openpnm.models.collections.phase import standard_gas_mixture
-from openpnm.models.collections.phase import binary_gas_mixture
-from openpnm.utils import HealthDict
-from openpnm.utils import Docorator, Workspace
-from openpnm.utils import get_printable_props, get_printable_labels
 
+import numpy as np
+
+from openpnm.models.collections.phase import (
+    binary_gas_mixture,
+    standard_gas_mixture,
+    standard_liquid_mixture,
+)
+from openpnm.models.phase.mixtures import mole_summation
+from openpnm.phase import Phase
+from openpnm.utils import (
+    Docorator,
+    HealthDict,
+    Workspace,
+    get_printable_labels,
+    get_printable_props,
+)
 
 logger = logging.getLogger(__name__)
 docstr = Docorator()
 ws = Workspace()
 
 
 __all__ = [
@@ -340,15 +347,15 @@
                 return self['pore.mole_fraction' + '.' + compname]
         else:
             self['pore.mole_fraction.' + compname] = y
 
 
 class BinaryGas(GasMixture):
     r"""
-    A `GasMixture` class that has a predefined set of models for computing the
+    A ``GasMixture`` class that has a predefined set of models for computing the
     properties of the mixture as a function of composition.
 
     The number of components is capped at 2 (i.e. binary) since the calculation
     of diffusion coefficients using the Lennard-Jones method in the `chemicals`
     package only works for binary mixtures.
     """
 
@@ -370,35 +377,35 @@
                 except KeyError:
                     pass
         super().__setitem__(key, value)
 
 
 class StandardLiquidMixture(LiquidMixture):
     r"""
-    A `LiquidMixture` class that also has a predefined suite of models for
+    A ``LiquidMixture`` class that also has a predefined suite of models for
     computing the properties of the mixture as a function of composition.
 
     The models are taken from the `chemicals` package and can be viewed with
-    `print(liq_mix.models)`, where `liq_mix` is an instance of this class.
+    ``print(liq_mix.models)``, where `liq_mix` is an instance of this class.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.add_model_collection(standard_liquid_mixture)
         # Running models doesn't make sense as compositions are not set yet
         # self.regenerate_models()
 
 
 class StandardGasMixture(GasMixture):
     r"""
-    A `GasMixture` class that also has a predefined suite of models for
+    A ``GasMixture`` class that also has a predefined suite of models for
     computing the properties of the mixture as a function of composition.
 
     The models are taken from the `chemicals` package and can be viewed with
-    `print(gas_mix.models)`, where `gas_mix` is an instance of this class.
+    ``print(gas_mix.models)``, where `gas_mix` is an instance of this class.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.add_model_collection(standard_gas_mixture)
         # Running models doesn't make sense as compositions are not set yet
         # self.regenerate_models()
```

### Comparing `openpnm-3.1.2/openpnm/phase/_phase.py` & `openpnm-3.2.0/openpnm/phase/_phase.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/phase/_species.py` & `openpnm-3.2.0/openpnm/phase/_species.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
-from openpnm.phase import Phase, _fetch_chemical_props
-from openpnm.models.collections.phase import standard_liquid
-from openpnm.models.collections.phase import standard_gas
 
+from openpnm.models.collections.phase import standard_gas, standard_liquid
+from openpnm.phase import Phase, _fetch_chemical_props
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
     'Species',
     'StandardGas',
@@ -53,20 +52,22 @@
                 for comp in item.components.values():
                     if self is comp:
                         return item
         logger.warn("No mixture phase found for this species")
 
 
 class StandardLiquid(Species):
+    """A ``Species`` object with built-in standard liquid-phase models."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.add_model_collection(standard_liquid)
         self.regenerate_models()
 
 
 class StandardGas(Species):
+    """A ``Species`` object with built-in standard gas-phase models."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.add_model_collection(standard_gas)
         self.regenerate_models()
```

### Comparing `openpnm-3.1.2/openpnm/phase/_water.py` & `openpnm-3.2.0/openpnm/phase/_water.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/solvers/_base.py` & `openpnm-3.2.0/openpnm/solvers/_base.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/solvers/_petsc.py` & `openpnm-3.2.0/openpnm/solvers/_petsc.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/solvers/_scipy.py` & `openpnm-3.2.0/openpnm/solvers/_scipy.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/topotools/_graphtools.py` & `openpnm-3.2.0/openpnm/topotools/_graphtools.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/topotools/_perctools.py` & `openpnm-3.2.0/openpnm/topotools/_perctools.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/topotools/_topotools.py` & `openpnm-3.2.0/openpnm/topotools/_topotools.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,35 +337,44 @@
         default is 0.
     label : str
         An identifying label to isolate the pores on the faces of the network.
         The default is 'surface'.  Surface pores can be found using
         ``find_surface_pores``.
 
     """
-    label = label.split('.', 1)[-1]
-    if 'pore.'+label not in network.labels():
-        find_surface_pores(network, label=label)
-    Psurf = network['pore.'+label]
+    if label is not None:
+        label = label.split('.', 1)[-1]
+        if 'pore.'+label not in network.labels():
+            find_surface_pores(network, label=label)
+        Psurf = network['pore.'+label]
+    else:
+        Psurf = True  # So it will "do nothing" below
     crds = network['pore.coords']
     xmin, xmax = np.amin(crds[:, 0]), np.amax(crds[:, 0])
     xspan = xmax - xmin
     ymin, ymax = np.amin(crds[:, 1]), np.amax(crds[:, 1])
     yspan = ymax - ymin
     zmin, zmax = np.amin(crds[:, 2]), np.amax(crds[:, 2])
     zspan = zmax - zmin
     dims = dimensionality(network)
     if dims[0]:
         network['pore.left'] = (crds[:, 0] <= (xmin + tol*xspan)) * Psurf
+        network['pore.xmin'] = np.copy(network['pore.left'])
         network['pore.right'] = (crds[:, 0] >= (xmax - tol*xspan)) * Psurf
+        network['pore.xmax'] = np.copy(network['pore.right'])
     if dims[1]:
         network['pore.front'] = (crds[:, 1] <= (ymin + tol*yspan)) * Psurf
+        network['pore.ymin'] = np.copy(network['pore.front'])
         network['pore.back'] = (crds[:, 1] >= (ymax - tol*yspan)) * Psurf
+        network['pore.ymax'] = np.copy(network['pore.back'])
     if dims[2]:
-        network['pore.top'] = (crds[:, 2] >= (zmax - tol*zspan)) * Psurf
         network['pore.bottom'] = (crds[:, 2] <= (zmin + tol*zspan)) * Psurf
+        network['pore.zmin'] = np.copy(network['pore.bottom'])
+        network['pore.top'] = (crds[:, 2] >= (zmax - tol*zspan)) * Psurf
+        network['pore.zmax'] = np.copy(network['pore.top'])
 
 
 def find_surface_pores(network, markers=None, label='surface'):
     r"""
     Find the pores on the surface of the domain by performing a Delaunay
     triangulation between the network pores and some external ``markers``. All
     pores connected to these external marker points are considered surface
```

### Comparing `openpnm-3.1.2/openpnm/utils/__init__.py` & `openpnm-3.2.0/openpnm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/utils/_health.py` & `openpnm-3.2.0/openpnm/utils/_health.py`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/openpnm/utils/_misc.py` & `openpnm-3.2.0/openpnm/utils/_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os
+import functools
 import inspect
+import os
 import warnings
-import functools
+from collections.abc import Iterable
+
 import numpy as np
+import numpy.lib.recfunctions as rf
 import scipy.sparse as sparse
-from collections.abc import Iterable
 from docrep import DocstringProcessor
-import numpy.lib.recfunctions as rf
-
 
 __all__ = [
     'Docorator',
     'PrintableList',
     'PrintableDict',
     'HealthDict',
     'NestedDict',
@@ -28,14 +28,15 @@
     'struct_to_dict',
     'get_printable_props',
     'get_printable_labels',
 ]
 
 
 class Docorator(DocstringProcessor):
+    """OpenPNM's customized docstring processor."""
 
     __instance__ = None
 
     def __new__(cls, *args, **kwargs):
         if Docorator.__instance__ is None:
             Docorator.__instance__ = DocstringProcessor()
```

### Comparing `openpnm-3.1.2/openpnm/utils/_project.py` & `openpnm-3.2.0/openpnm/utils/_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-import re
-import pickle
 import logging
+import pickle
+import re
 import uuid
-import numpy as np
 from copy import deepcopy
 from datetime import datetime
-from openpnm.utils import Workspace, SettingsAttr
 
+import numpy as np
+
+from openpnm.utils import SettingsAttr, Workspace
 
 ws = Workspace()
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
     'Project',
     'SimpleList',
 ]
 
 
 class SimpleList:
+    """A simple list class that prevents duplicates, and more!"""
     def __init__(self, data=None):
         if (data is not None):
             self._list = list(data)
         else:
             self._list = list()
 
     def __repr__(self):  # pragma: no cover
```

### Comparing `openpnm-3.1.2/openpnm/utils/_settings.py` & `openpnm-3.2.0/openpnm/utils/_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 from copy import deepcopy
-from openpnm.utils import PrintableDict
 
+from openpnm.utils import PrintableDict
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
     'TypedMixin',
     'TypedSet',
     'TypedList',
     'SettingsAttr',
 ]
 
 
 class TypedMixin:
-    """Brief explanation of 'TypedMixin'"""
+    """Based class for enforcing types on lists and sets."""
 
     def __init__(self, iterable=[], types=[]):
         self._types = types
         if iterable:
             super().__init__(iterable)
             self._set_types()
 
@@ -41,27 +41,23 @@
     def _check_type(self, value):
         if (type(value) not in self.types) and (len(self.types) > 0):
             raise TypeError("This list cannot accept values of type "
                             + f"{type(value)}")
 
 
 class TypedSet(TypedMixin, set):
-    """Brief explanation of 'TypedSet'"""
+    """A set that enforces all elements have the same type."""
 
     def add(self, item):
         self._check_type(item)
         super().add(item)
 
 
 class TypedList(TypedMixin, list):
-    """
-    A list that enforces all elements have the same type.
-
-    The allowed type or types are set during
-    """
+    """A list that enforces all elements have the same type."""
 
     def __setitem__(self, ind, value):
         self._check_type(value)
         super().__setitem__(ind, value)
 
     def append(self, value):
         self._check_type(value)
```

### Comparing `openpnm-3.1.2/openpnm/utils/_workspace.py` & `openpnm-3.2.0/openpnm/utils/_workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import re
 import logging
 import pickle
+import re
 from datetime import datetime
 from uuid import uuid4
-from openpnm.utils import SettingsAttr
 
+from openpnm.utils import SettingsAttr
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("openpnm")
 
 __all__ = ['Workspace']
 
 
 class WorkspaceSettings(SettingsAttr):
     r"""
 
@@ -39,18 +39,30 @@
                 may be unable to continue running.
         ======= ==============================================================
     """
     default_solver = 'PardisoSpsolve'
 
     @property
     def loglevel(self):
-        return logger.level
+        return self._loglevel
 
     @loglevel.setter
     def loglevel(self, value):
+        if isinstance(value, str):
+            options = {
+                "TRACE": 5,
+                "DEBUG": 10,
+                "INFO": 20,
+                "SUCESS": 25,
+                "WARNING": 30,
+                "ERROR": 40,
+                "CRITICAL": 50
+            }
+            value = options[value]
+        self._loglevel = value
         logger.setLevel(value)
 
 
 class Workspace(dict):
     r"""
     The Workspace object provides the highest level of adminstrative
     control over active OpenPNM sessions.
```

### Comparing `openpnm-3.1.2/openpnm/visualization/_conduit_visualizer.py` & `openpnm-3.2.0/openpnm/visualization/_conduit_visualizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib.patches import Circle, Polygon, Rectangle
 from matplotlib.collections import PatchCollection
-import matplotlib.pyplot as plt
-from openpnm.topotools import find_connected_sites
-from openpnm.network import Network
-from openpnm.models.geometry import throat_length, throat_endpoints
-from openpnm._skgraph.tools import rotate_coords
+from matplotlib.patches import Circle, Polygon, Rectangle
 
+from openpnm._skgraph.tools import rotate_coords
+from openpnm.models.geometry import throat_endpoints, throat_length
+from openpnm.network import Network
+from openpnm.topotools import find_connected_sites
 
 __all__ = [
     'draw_conduit',
 ]
 
 
 def draw_conduit(network, throat):
+    """Draws a subset of a network given throat numbers."""
     pn = network
     P1, P2 = find_connected_sites(g=pn, bonds=throat)
     new_net = Network(coords=pn.coords[[P1, P2], :], conns=np.atleast_2d([0, 1]))
     new_net.regenerate_models()
     new_net['pore.diameter'] = pn['pore.diameter'][[P1, P2]]
     new_net['throat.diameter'] = [pn['throat.diameter'][throat]]
     new_net['throat.length'] = throat_length.circles_and_rectangles(new_net)
```

### Comparing `openpnm-3.1.2/openpnm/visualization/_plottools.py` & `openpnm-3.2.0/openpnm/visualization/_plottools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+import logging
+
+import matplotlib.pyplot as plt
 import numpy as np
-import openpnm as op
-from tqdm.auto import tqdm
 from matplotlib.pyplot import cm
-import matplotlib.pyplot as plt
+from tqdm.auto import tqdm
+
+import openpnm as op
+
+logger = logging.getLogger(__name__)
 
 
 __all__ = [
     'plot_connections',
     'plot_coordinates',
     'plot_networkx',
     'plot_tutorial',
@@ -105,17 +110,18 @@
     ...                                       ax=ax,
     ...                                       color='r')  # plot boundary throats in red
 
     """
     import matplotlib.pyplot as plt
     from matplotlib import cm
     from matplotlib import colors as mcolors
-    from mpl_toolkits.mplot3d import Axes3D
     from matplotlib.collections import LineCollection
+    from mpl_toolkits.mplot3d import Axes3D
     from mpl_toolkits.mplot3d.art3d import Line3DCollection
+
     from openpnm.topotools import dimensionality
 
     Ts = network.Ts if throats is None else network._parse_indices(throats)
     dim = dimensionality(network)
     ThreeD = True if dim.sum() == 3 else False
     # Add a dummy axis for 1D networks
     if dim.sum() == 1:
@@ -143,17 +149,23 @@
     if 'c' in kwargs.keys():
         color = kwargs.pop('c')
     color = mcolors.to_rgb(color) + tuple([alpha])
     # Override colors with color_by if given
     if color_by is not None:
         if len(color_by) != len(Ts):
             color_by = color_by[Ts]
+        if not np.all(np.isfinite(color_by)):
+            color_by[~np.isfinite(color_by)] = 0
+            logger.warning('nans or infs found in color_by array, setting to 0')
         color = cm.get_cmap(name=cmap)(color_by / color_by.max())
         color[:, 3] = alpha
     if size_by is not None:
+        if not np.all(np.isfinite(size_by)):
+            size_by[~np.isfinite(size_by)] = 0
+            logger.warning('nans or infs found in size_by array, setting to 0')
         linewidth = size_by / size_by.max() * linewidth
 
     if ThreeD:
         lc = Line3DCollection(throat_pos, colors=color, cmap=cmap,
                               linestyles=linestyle, linewidths=linewidth,
                               antialiaseds=np.ones_like(network.Ts), **kwargs)
     else:
@@ -194,15 +206,17 @@
         are specified then all are shown.
     ax : Matplotlib axis handle
         If ``ax`` is supplied, then the coordinates will be overlaid.
         This enables the plotting of multiple different sets of pores as
         well as throat connections from ``plot_connections``.
     size_by : str or array_like
         An ndarray of pore values (e.g. alg['pore.concentration']). These
-        values are normalized by scaled by ``markersize``.
+        values are normalized by scaled by ``markersize``.  Note that this controls
+        the marker *area*, so if you want the markers to be proportional to diameter
+        you should do `size_by=net['pore.diameter']**2`.
     color_by : str or array_like
         An ndarray of pore values (e.g. alg['pore.concentration']).
     cmap : str or cmap object
         The matplotlib colormap to use if specfying a pore property
         for ``color_by``
     color : str
         A matplotlib named color (e.g. 'r' for red).
@@ -256,14 +270,15 @@
     ...                                       color='r',
     ...                                       ax=ax)  # plot boundary pores in red
 
     """
     import matplotlib.pyplot as plt
     from matplotlib import cm
     from mpl_toolkits.mplot3d import Axes3D
+
     from openpnm.topotools import dimensionality
 
     Ps = network.Ps if pores is None else network._parse_indices(pores)
 
     dim = dimensionality(network)
     ThreeD = True if dim.sum() == 3 else False
     # Add a dummy axis for 1D networks
@@ -293,16 +308,22 @@
     # Parse formatting kwargs
     if 'c' in kwargs.keys():
         color = kwargs.pop('c')
     if 's' in kwargs.keys():
         markersize = kwargs.pop('s')
     if color_by is not None:
         color_by = color_by[Ps]
+        if not np.all(np.isfinite(color_by)):
+            color_by[~np.isfinite(color_by)] = 0
+            logger.warning('nans or infs found in color_by array, setting to 0')
         color = cm.get_cmap(name=cmap)(color_by / color_by.max())
     if size_by is not None:
+        if not np.all(np.isfinite(size_by)):
+            size_by[~np.isfinite(size_by)] = 0
+            logger.warning('nans or infs found in size_by array, setting to 0')
         markersize = size_by / size_by.max() * markersize
 
     if ThreeD:
         sc = ax.scatter(X, Y, Z,
                         c=color,
                         s=markersize,
                         marker=marker,
@@ -361,15 +382,15 @@
                   plot_throats=True,
                   labels=None,
                   colors=None,
                   scale=1,
                   ax=None,
                   alpha=1.0):  # pragma: no cover
     r"""
-    Creates a pretty 2d plot for 2d OpenPNM networks.
+    Creates a pretty 2D plot for 2D OpenPNM networks.
 
     Parameters
     ----------
     network : Network
     plot_throats : bool, optional
         Plots throats as well as pores, if True.
     labels : list, optional
@@ -382,15 +403,16 @@
         Matplotlib axes object
     alpha: float, optional
         Transparency value, 1 is opaque and 0 is transparent
 
     """
     import matplotlib.pyplot as plt
     from matplotlib.collections import PathCollection
-    from networkx import Graph, draw_networkx_nodes, draw_networkx_edges
+    from networkx import Graph, draw_networkx_edges, draw_networkx_nodes
+
     from openpnm.topotools import dimensionality
 
     dims = dimensionality(network)
     if dims.sum() > 2:
         raise Exception("NetworkX plotting only works for 2D networks.")
     temp = network['pore.coords'].T[dims].squeeze()
     if dims.sum() == 1:
@@ -449,27 +471,35 @@
         if isinstance(item, PathCollection) and id(item) not in temp:
             item.set_sizes(markersize)
 
     return gplot
 
 
 def plot_tutorial(network,
+                  pore_labels=None,
+                  throat_labels=None,
                   font_size=12,
                   line_width=2,
                   node_color='b',
                   edge_color='r',
                   node_size=500):  # pragma: no cover
     r"""
     Generate a network plot suitable for tutorials and explanations.
 
     Parameters
     ----------
     network : Network
         The network to plot, should be 2D, since the z-coordinate will be
         ignored.
+    pore_labels : array_like
+        A list of values to use for labeling the pores. If not provided then pore
+        index is used.
+    throat_labels : array_like
+        A list of values to use for labeling the throat. If not provided then throat
+        index is used.
     font_size : int
         Size of font to use for labels.
     line_width : int
         Thickness of edge lines and node borders.
     node_color : str
         Color of node border.
     edge_color : str
@@ -478,22 +508,30 @@
         Size of node circle.
 
     Returns
     -------
     g : NetworkX plot object
 
     """
-    import networkx as nx
     import matplotlib.pyplot as plt
+    import networkx as nx
+
     from openpnm.io import network_to_networkx
 
     G = network_to_networkx(network=network)
     pos = {i: network['pore.coords'][i, 0:2] for i in network.Ps}
-    labels = {i: i for i in network.Ps}
-    edge_labels = {tuple(network['throat.conns'][i, :]): i for i in network.Ts}
+    if pore_labels is None:
+        labels = {i: i for i in network.Ps}
+    else:
+        labels = {i: pore_labels[i] for i in network.Ps}
+    if throat_labels is None:
+        edge_labels = {tuple(network['throat.conns'][i, :]): i for i in network.Ts}
+    else:
+        edge_labels = {tuple(network['throat.conns'][i, :]): throat_labels[i]
+                       for i in network.Ts}
 
     gplot = nx.draw_networkx_nodes(G, pos,
                                    node_size=node_size,
                                    node_color='w',
                                    edgecolors=node_color,
                                    linewidths=line_width)
     nx.draw_networkx_edges(
@@ -667,16 +705,16 @@
 
     Notes
     -----
     (1) The generated voxel image is labeled with 0s, 1s and 2s signifying
     solid phase, pores, and throats respectively.
 
     """
-    from skimage.morphology import cube, ball
-    from porespy.tools import overlay, insert_cylinder
+    from porespy.tools import insert_cylinder, overlay
+    from skimage.morphology import ball, cube
     xyz = network["pore.coords"]
     cn = network["throat.conns"]
 
     # Distance bounding box from the network by a fixed amount
     delta = network["pore.diameter"].mean() / 2
     if isinstance(network, op.network.Cubic):
         try:
@@ -810,14 +848,15 @@
     pore_color=None,
     pore_size=None,
     throat_color=None,
     throat_size=None,
     bgcolor='grey',
 ):
     r"""
+    Creates a pretty network plot using VisPy.
 
     Parameters
     ----------
     network
     """
     try:
         from vispy import scene
```

### Comparing `openpnm-3.1.2/openpnm.egg-info/PKG-INFO` & `openpnm-3.2.0/openpnm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,93 @@
 Metadata-Version: 2.1
 Name: openpnm
-Version: 3.1.2
+Version: 3.2.0
 Summary: A framework for conducting pore network modeling simulations of multiphase transport in porous materials
 Home-page: http://openpnm.org
 Author: OpenPNM Team
 Author-email: jgostick@uwaterloo.ca
 License: UNKNOWN
 Download-URL: https://github.com/PMEAL/OpenPNM/
 Project-URL: Documentation, https://openpnm.org
 Project-URL: Source, https://github.com/PMEAL/OpenPNM
 Project-URL: Tracker, https://github.com/PMEAL/OpenPNM/issues
-Description: [![](https://github.com/PMEAL/OpenPNM/actions/workflows/nightly.yml/badge.svg)](https://github.com/PMEAL/OpenPNM/actions/workflows/nightly.yml)
-        [![](https://codecov.io/gh/PMEAL/OpenPNM/branch/dev/graph/badge.svg)](https://codecov.io/gh/PMEAL/OpenPNM)
-        [![](https://img.shields.io/badge/Documentation-Read-blue.svg)](https://pmeal.github.io/OpenPNM/)
-        [![](https://badge.fury.io/py/openpnm.svg)](https://pypi.python.org/pypi/openpnm)
-        [![](https://anaconda.org/conda-forge/openpnm/badges/installer/conda.svg)](https://anaconda.org/conda-forge/openpnm)
-        
-        -----
-        
-        > VERSION 3.0 of OpenPNM is now out. All the [examples on the website](https://openpnm.org/_examples/index.html) are now using the features and idioms of V3. For a description of the main changes please see our [recent blog post](http://pmeal.com/posts/2022-10-10-notebook-post/). 
-        
-        # Overview of OpenPNM
-        
-        *OpenPNM* is a comprehensive framework for performing pore network simulations of porous materials.
-        
-        ## More Information
-        
-        For more details about the package can be found in the [on-line documentation](https://openpnm.org)
-        
-        ## Installation and Requirements
-        
-        ### Preferred method
-        The preferred way of installing OpenPNM is through [Anaconda Cloud](https://anaconda.org/conda-forge/openpnm) using:
-        
-        ```
-        conda install -c conda-forge openpnm
-        ```
-        
-        ### Alternative method
-        OpenPNM can also be installed from the [Python Package Index](https://pypi.org/project/openpnm/) using:
-        
-        ```
-        pip install openpnm
-        ```
-        
-        However, we don't recommend installing using `pip` since `pypardiso`, which is a blazing fast direct solver, is not available for Windows users who use Python 3.7+.
-        
-        ### For developers
-        For developers who intend to change the source code or contribute to OpenPNM, the source code can be downloaded from [Github](https://github.com/pmeal/OpenPNM/) and installed by running:
-        
-        ```
-        pip install -e 'path/to/downloaded/files'
-        ```
-        
-        The advantage to installing from the source code is that you can edit the files and have access to your changes each time you import *OpenPNM*.
-        
-        OpenPNM requires the *Scipy Stack* (Numpy, Scipy, Matplotlib, etc), which is most conveniently obtained by installing the [Anaconda Distribution](https://conda.io/docs/user-guide/install/download.html).
-        
-        ## Asking Questions and Getting Help
-        
-        Github now has a [Discussions](https://github.com/PMEAL/OpenPNM/discussions) function, which works similarly to [stack overflow](https://www.stackoverflow.com).  Please post your question in the [Q&A category](https://github.com/PMEAL/OpenPNM/discussions?discussions_q=category%3AQ%26A) so devs or users can provide answers, vote on accepted answers, improve on each other's answers, and generally discuss things. Most importantly, all answers are searchable so eventually, once enough questions have been posted and answered, you can find what you're looking for with a simple search.
-        
-        ## Contact
-        
-        OpenPNM is developed by the Porous Materials Engineering and Analysis Lab [(PMEAL)](http://pmeal.com), in the [Department of Chemical Engineering](https://uwaterloo.ca/chemical-engineering/) at the [University of Waterloo](https://uwaterloo.ca/) in Waterloo, Ontario, Canada.
-        
-        The lead developer for this project is Prof. Jeff Gostick (jgostick@gmail.com).
-        
-        ## Acknowledgements
-        
-        OpenPNM is grateful to [CANARIE](https://canarie.ca) for their generous funding over the past few years.  We would also like to acknowledge the support of [NSERC of Canada](https://www.nserc-crsng.gc.ca/) for funding many of the student that have contributed to OpenPNM since it's inception in 2011.
-        
-        ## Citation
-        
-        If you use OpenPNM in a publication, please cite the following paper:
-        
-        > _Gostick et al._ "**OpenPNM: a pore network modeling package.**" Computing in Science & Engineering 18, no. 4 (2016): 60-74.
-        > [doi:10.1109/MCSE.2016.49](https://ieeexplore.ieee.org/document/7478437)
-        
-        Also, we ask that you "star" :star: this repository so we can track the number of users who are interested in this project, which is helpful for securing future grant funding.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![](https://github.com/PMEAL/OpenPNM/actions/workflows/nightly.yml/badge.svg)](https://github.com/PMEAL/OpenPNM/actions/workflows/nightly.yml)
+[![](https://codecov.io/gh/PMEAL/OpenPNM/branch/dev/graph/badge.svg)](https://codecov.io/gh/PMEAL/OpenPNM)
+[![](https://img.shields.io/badge/Documentation-Read-blue.svg)](https://pmeal.github.io/OpenPNM/)
+[![](https://badge.fury.io/py/openpnm.svg)](https://pypi.python.org/pypi/openpnm)
+[![](https://anaconda.org/conda-forge/openpnm/badges/installer/conda.svg)](https://anaconda.org/conda-forge/openpnm)
+
+-----
+
+> VERSION 3.0 of OpenPNM is now out. All the [examples on the website](https://openpnm.org/_examples/index.html) are now using the features and idioms of V3. For a description of the main changes please see our [recent blog post](http://pmeal.com/posts/2022-10-10-notebook-post/). 
+
+# Overview of OpenPNM
+
+*OpenPNM* is a comprehensive framework for performing pore network simulations of porous materials.
+
+## More Information
+
+For more details about the package can be found in the [on-line documentation](https://openpnm.org)
+
+## Installation and Requirements
+
+### Preferred method
+The preferred way of installing OpenPNM is through [Anaconda Cloud](https://anaconda.org/conda-forge/openpnm) using:
+
+```
+conda install -c conda-forge openpnm
+```
+
+### Alternative method
+OpenPNM can also be installed from the [Python Package Index](https://pypi.org/project/openpnm/) using:
+
+```
+pip install openpnm
+```
+
+However, we don't recommend installing using `pip` since `pypardiso`, which is a blazing fast direct solver, is not available for Windows users who use Python 3.7+.
+
+### For developers
+For developers who intend to change the source code or contribute to OpenPNM, the source code can be downloaded from [Github](https://github.com/pmeal/OpenPNM/) and installed by running:
+
+```
+pip install -e 'path/to/downloaded/files'
+```
+
+The advantage to installing from the source code is that you can edit the files and have access to your changes each time you import *OpenPNM*.
+
+OpenPNM requires the *Scipy Stack* (Numpy, Scipy, Matplotlib, etc), which is most conveniently obtained by installing the [Anaconda Distribution](https://conda.io/docs/user-guide/install/download.html).
+
+## Asking Questions and Getting Help
+
+Github now has a [Discussions](https://github.com/PMEAL/OpenPNM/discussions) function, which works similarly to [stack overflow](https://www.stackoverflow.com).  Please post your question in the [Q&A category](https://github.com/PMEAL/OpenPNM/discussions?discussions_q=category%3AQ%26A) so devs or users can provide answers, vote on accepted answers, improve on each other's answers, and generally discuss things. Most importantly, all answers are searchable so eventually, once enough questions have been posted and answered, you can find what you're looking for with a simple search.
+
+## Contact
+
+OpenPNM is developed by the Porous Materials Engineering and Analysis Lab [(PMEAL)](http://pmeal.com), in the [Department of Chemical Engineering](https://uwaterloo.ca/chemical-engineering/) at the [University of Waterloo](https://uwaterloo.ca/) in Waterloo, Ontario, Canada.
+
+The lead developer for this project is Prof. Jeff Gostick (jgostick@gmail.com).
+
+## Acknowledgements
+
+OpenPNM is grateful to [CANARIE](https://canarie.ca) for their generous funding over the past few years.  We would also like to acknowledge the support of [NSERC of Canada](https://www.nserc-crsng.gc.ca/) for funding many of the student that have contributed to OpenPNM since it's inception in 2011.
+
+## Citation
+
+If you use OpenPNM in a publication, please cite the following paper:
+
+> _Gostick et al._ "**OpenPNM: a pore network modeling package.**" Computing in Science & Engineering 18, no. 4 (2016): 60-74.
+> [doi:10.1109/MCSE.2016.49](https://ieeexplore.ieee.org/document/7478437)
+
+Also, we ask that you "star" :star: this repository so we can track the number of users who are interested in this project, which is helpful for securing future grant funding.
+
+
```

### Comparing `openpnm-3.1.2/openpnm.egg-info/SOURCES.txt` & `openpnm-3.2.0/openpnm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpnm-3.1.2/setup.py` & `openpnm-3.2.0/setup.py`

 * *Files identical despite different names*

