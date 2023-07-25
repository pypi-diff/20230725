# Comparing `tmp/rio_tiler-5.0.3.tar.gz` & `tmp/rio_tiler-6.0.0.tar.gz`

## Comparing `rio_tiler-5.0.3.tar` & `rio_tiler-6.0.0.tar`

### file list

```diff
@@ -1,197 +1,197 @@
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/__init__.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/colormap.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/constants.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/errors.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/expression.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/logger.py
--rw-r--r--   0        0        0    25874 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/models.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/py.typed
--rw-r--r--   0        0        0    21013 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/reader.py
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/tasks.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/types.py
--rw-r--r--   0        0        0    21907 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/accent.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/accent_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/afmhot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/afmhot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/autumn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/autumn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/binary.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/binary_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/blues.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/blues_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bone.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bone_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/brbg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/brbg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/brg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/brg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bupu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bupu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bwr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bwr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cfastie.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cividis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cividis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cmrmap.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cmrmap_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cool.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cool_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/coolwarm.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/coolwarm_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/copper.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/copper_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cubehelix.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cubehelix_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/dark2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/dark2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/flag.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/flag_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_earth.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_earth_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_heat.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_heat_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_ncar.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_ncar_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_stern.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_stern_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_yarg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_yarg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/greens.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/greens_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/greys.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/greys_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/hot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/hot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/hsv.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/hsv_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/inferno.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/inferno_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/jet.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/jet_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/magma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/magma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/nipy_spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/nipy_spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ocean.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ocean_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/oranges.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/oranges_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/orrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/orrd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/paired.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/paired_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pastel1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pastel1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pastel2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pastel2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pink.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pink_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/piyg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/piyg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/plasma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/plasma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/prgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/prgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/prism.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/prism_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pubu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pubu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pubugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pubugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/puor.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/puor_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/purd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/purd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/purples.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/purples_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdgy.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdgy_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdpu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdpu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdylbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdylbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/reds.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/reds_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rplumbo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/schwarzwald.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/seismic.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/seismic_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set3.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set3_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/spring.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/spring_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/summer.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/summer_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab10.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab10_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20b.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20b_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20c.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20c_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/terrain.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/terrain_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/twilight.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_shifted.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_shifted_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/viridis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/viridis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/winter.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/winter_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/wistia.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/wistia_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylgnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylgnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylorbr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylorbr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylorrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylorrd_r.npy
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/__init__.py
--rw-r--r--   0        0        0    44738 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/base.py
--rw-r--r--   0        0        0    32170 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/rasterio.py
--rw-r--r--   0        0        0    10091 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/stac.py
--rw-r--r--   0        0        0    16046 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/xarray.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/__init__.py
--rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/reader.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/methods/__init__.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/methods/base.py
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/methods/defaults.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/.gitignore
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/AUTHORS.txt
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/LICENSE
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/README.md
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/pyproject.toml
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/PKG-INFO
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/__init__.py
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/colormap.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/constants.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/errors.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/expression.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/logger.py
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/models.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/py.typed
+-rw-r--r--   0        0        0    21013 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/reader.py
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/tasks.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/types.py
+-rw-r--r--   0        0        0    21907 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/accent.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/accent_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/afmhot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/afmhot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/autumn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/autumn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/binary.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/binary_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/blues.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/blues_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/bone.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/bone_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/brbg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/brbg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/brg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/brg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/bugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/bugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/bupu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/bupu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/bwr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/bwr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/cfastie.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/cividis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/cividis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/cmrmap.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/cmrmap_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/cool.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/cool_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/coolwarm.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/coolwarm_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/copper.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/copper_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/cubehelix.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/cubehelix_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/dark2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/dark2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/flag.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/flag_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_earth.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_earth_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_heat.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_heat_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_ncar.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_ncar_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_stern.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_stern_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_yarg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gist_yarg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gnuplot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gnuplot2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gnuplot2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gnuplot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/greens.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/greens_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/greys.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/greys_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/hot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/hot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/hsv.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/hsv_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/inferno.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/inferno_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/jet.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/jet_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/magma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/magma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/nipy_spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/nipy_spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ocean.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ocean_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/oranges.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/oranges_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/orrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/orrd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/paired.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/paired_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pastel1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pastel1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pastel2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pastel2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pink.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pink_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/piyg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/piyg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/plasma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/plasma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/prgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/prgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/prism.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/prism_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pubu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pubu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pubugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/pubugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/puor.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/puor_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/purd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/purd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/purples.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/purples_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdgy.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdgy_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdpu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdpu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdylbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdylbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rdylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/reds.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/reds_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/rplumbo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/schwarzwald.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/seismic.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/seismic_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/set1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/set1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/set2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/set2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/set3.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/set3_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/spring.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/spring_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/summer.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/summer_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/tab10.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/tab10_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/tab20.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/tab20_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/tab20b.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/tab20b_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/tab20c.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/tab20c_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/terrain.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/terrain_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/twilight.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/twilight_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/twilight_shifted.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/twilight_shifted_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/viridis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/viridis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/winter.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/winter_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/wistia.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/wistia_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ylgnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ylgnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ylorbr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ylorbr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ylorrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/cmap_data/ylorrd_r.npy
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/io/__init__.py
+-rw-r--r--   0        0        0    44738 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/io/base.py
+-rw-r--r--   0        0        0    32171 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/io/rasterio.py
+-rw-r--r--   0        0        0    10091 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/io/stac.py
+-rw-r--r--   0        0        0    16046 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/io/xarray.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/mosaic/__init__.py
+-rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/mosaic/reader.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/mosaic/methods/__init__.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/mosaic/methods/base.py
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/rio_tiler/mosaic/methods/defaults.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/.gitignore
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/AUTHORS.txt
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/LICENSE
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/README.md
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 rio_tiler-6.0.0/PKG-INFO
```

### Comparing `rio_tiler-5.0.3/rio_tiler/colormap.py` & `rio_tiler-6.0.0/rio_tiler/colormap.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/errors.py` & `rio_tiler-6.0.0/rio_tiler/errors.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/expression.py` & `rio_tiler-6.0.0/rio_tiler/expression.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/models.py` & `rio_tiler-6.0.0/rio_tiler/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """rio-tiler models."""
 
 import itertools
 import warnings
-from enum import Enum
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple, Union
 
 import attr
 import numpy
 from affine import Affine
 from color_operations import parse_operations, scale_dtype, to_math_type
 from pydantic import BaseModel
 from rasterio import windows
@@ -36,33 +35,23 @@
     linear_rescale,
     non_alpha_indexes,
     render,
     resize_array,
 )
 
 
-class NodataTypes(str, Enum):
-    """rio-tiler Nodata types."""
-
-    Alpha = "Alpha"
-    Mask = "Mask"
-    Internal = "Internal"
-    Nodata = "Nodata"
-    Empty = "None"
-
-
-class RioTilerBaseModel(BaseModel):
-    """Base Model for rio-tiler models."""
+class RioTilerBaseModel:
+    """Provides dictionary access for pydantic models, for backwards compatability."""
 
     def __getitem__(self, item):
-        """Keep `getter` access for compatibility."""
+        """Access item like in Dict."""
         return self.__dict__[item]
 
 
-class Bounds(RioTilerBaseModel):
+class Bounds(RioTilerBaseModel, BaseModel):
     """Dataset Bounding box"""
 
     bounds: BoundingBox
 
 
 class SpatialInfo(Bounds):
     """Dataset SpatialInfo"""
@@ -73,28 +62,24 @@
 
 class Info(SpatialInfo):
     """Dataset Info."""
 
     band_metadata: List[Tuple[str, Dict]]
     band_descriptions: List[Tuple[str, str]]
     dtype: str
-    nodata_type: NodataTypes
-    colorinterp: Optional[List[str]]
-    scale: Optional[float]
-    offset: Optional[float]
-    colormap: Optional[GDALColorMapType]
+    nodata_type: Literal["Alpha", "Mask", "Internal", "Nodata", "None"]
+    colorinterp: Optional[List[str]] = None
+    scale: Optional[float] = None
+    offset: Optional[float] = None
+    colormap: Optional[GDALColorMapType] = None
 
-    class Config:
-        """Config for model."""
+    model_config = {"extra": "allow"}
 
-        extra = "allow"
-        use_enum_values = True
 
-
-class BandStatistics(RioTilerBaseModel):
+class BandStatistics(RioTilerBaseModel, BaseModel):
     """Band statistics"""
 
     min: float
     max: float
     mean: float
     count: float
     sum: float
@@ -104,18 +89,15 @@
     minority: float
     unique: float
     histogram: List[List[NumType]]
     valid_percent: float
     masked_pixels: float
     valid_pixels: float
 
-    class Config:
-        """Config for model."""
-
-        extra = "allow"  # We allow extra values for `percentiles_{}`
+    model_config = {"extra": "allow"}
 
 
 def to_coordsbbox(bbox) -> Optional[BoundingBox]:
     """Convert bbox to CoordsBbox nameTuple."""
     return BoundingBox(*bbox) if bbox else None
```

### Comparing `rio_tiler-5.0.3/rio_tiler/profiles.py` & `rio_tiler-6.0.0/rio_tiler/profiles.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/reader.py` & `rio_tiler-6.0.0/rio_tiler/reader.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/tasks.py` & `rio_tiler-6.0.0/rio_tiler/tasks.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/types.py` & `rio_tiler-6.0.0/rio_tiler/types.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/utils.py` & `rio_tiler-6.0.0/rio_tiler/utils.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/__init__.py` & `rio_tiler-6.0.0/rio_tiler/cmap_data/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/accent.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/accent.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/accent_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/accent_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/afmhot.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/afmhot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/afmhot_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/afmhot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/autumn.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/autumn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/autumn_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/autumn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/binary.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/binary.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/binary_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/binary_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/blues.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/blues.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/blues_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/blues_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/bone.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/bone.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/bone_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/bone_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/brbg.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/brbg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/brbg_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/brbg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/brg.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/brg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/brg_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/brg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/bugn.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/bugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/bugn_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/bugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/bupu.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/bupu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/bupu_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/bupu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/bwr.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/bwr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/bwr_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/bwr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/cfastie.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/cfastie.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/cividis.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/cividis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/cividis_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/cividis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/cmrmap.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/cmrmap.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/cmrmap_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/cmrmap_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/cool.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/cool.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/cool_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/cool_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/coolwarm.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/coolwarm.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/coolwarm_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/coolwarm_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/copper.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/copper.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/copper_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/copper_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/cubehelix.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/cubehelix.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/cubehelix_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/cubehelix_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/dark2.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/dark2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/dark2_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/dark2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/flag.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/flag.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/flag_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/flag_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_earth.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_earth.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_earth_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_earth_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_gray.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_gray_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_heat.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_heat.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_heat_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_heat_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_ncar.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_ncar.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_ncar_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_ncar_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_rainbow.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_rainbow_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_stern.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_stern.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_stern_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_stern_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_yarg.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_yarg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_yarg_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gist_yarg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gnbu.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gnbu_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gnuplot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot2.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gnuplot2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot2_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gnuplot2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gnuplot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gray.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/gray_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/greens.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/greens.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/greens_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/greens_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/greys.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/greys.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/greys_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/greys_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/hot.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/hot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/hot_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/hot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/hsv.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/hsv.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/hsv_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/hsv_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/inferno.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/inferno.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/inferno_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/inferno_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/jet.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/jet.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/jet_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/jet_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/magma.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/magma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/magma_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/magma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/nipy_spectral.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/nipy_spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/nipy_spectral_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/nipy_spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ocean.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ocean.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ocean_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ocean_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/oranges.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/oranges.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/oranges_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/oranges_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/orrd.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/orrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/orrd_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/orrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/paired.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/paired.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/paired_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/paired_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pastel1.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pastel1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pastel1_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pastel1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pastel2.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pastel2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pastel2_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pastel2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pink.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pink.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pink_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pink_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/piyg.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/piyg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/piyg_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/piyg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/plasma.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/plasma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/plasma_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/plasma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/prgn.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/prgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/prgn_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/prgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/prism.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/prism.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/prism_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/prism_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pubu.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pubu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pubu_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pubu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pubugn.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pubugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/pubugn_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/pubugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/puor.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/puor.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/puor_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/puor_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/purd.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/purd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/purd_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/purd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/purples.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/purples.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/purples_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/purples_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rainbow.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rainbow_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdbu.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdbu_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdgy.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdgy.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdgy_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdgy_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdpu.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdpu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdpu_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdpu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdylbu.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdylbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdylbu_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdylbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdylgn.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rdylgn_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rdylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/reds.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/reds.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/reds_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/reds_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/rplumbo.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/rplumbo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/schwarzwald.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/schwarzwald.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/seismic.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/seismic.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/seismic_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/seismic_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/set1.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/set1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/set1_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/set1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/set2.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/set2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/set2_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/set2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/set3.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/set3.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/set3_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/set3_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/spectral.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/spectral_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/spring.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/spring.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/spring_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/spring_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/summer.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/summer.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/summer_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/summer_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/tab10.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/tab10.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/tab10_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/tab10_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/tab20.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/tab20_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20b.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/tab20b.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20b_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/tab20b_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20c.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/tab20c.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20c_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/tab20c_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/terrain.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/terrain.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/terrain_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/terrain_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/twilight.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/twilight.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/twilight_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_shifted.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/twilight_shifted.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_shifted_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/twilight_shifted_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/viridis.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/viridis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/viridis_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/viridis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/winter.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/winter.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/winter_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/winter_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/wistia.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/wistia.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/wistia_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/wistia_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ylgn.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ylgn_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ylgnbu.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ylgnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ylgnbu_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ylgnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ylorbr.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ylorbr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ylorbr_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ylorbr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ylorrd.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ylorrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/cmap_data/ylorrd_r.npy` & `rio_tiler-6.0.0/rio_tiler/cmap_data/ylorrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/io/base.py` & `rio_tiler-6.0.0/rio_tiler/io/base.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/io/rasterio.py` & `rio_tiler-6.0.0/rio_tiler/io/rasterio.py`

 * *Files 1% similar despite different names*

```diff
@@ -570,15 +570,15 @@
                 category=NotGeoreferencedWarning,
                 module="rasterio",
             )
             cutline_mask = rasterize(
                 [shape],
                 out_shape=(img.height, img.width),
                 transform=img.transform,
-                all_touched=True,  # Necesary for matching masks at different resolutions
+                all_touched=True,  # Mandatory for matching masks at different resolutions
                 default_value=0,
                 fill=1,
                 dtype="uint8",
             ).astype("bool")
 
         img.cutline_mask = cutline_mask
         img.array.mask = numpy.where(~cutline_mask, img.array.mask, True)
```

### Comparing `rio_tiler-5.0.3/rio_tiler/io/stac.py` & `rio_tiler-6.0.0/rio_tiler/io/stac.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/io/xarray.py` & `rio_tiler-6.0.0/rio_tiler/io/xarray.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/mosaic/reader.py` & `rio_tiler-6.0.0/rio_tiler/mosaic/reader.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/mosaic/methods/__init__.py` & `rio_tiler-6.0.0/rio_tiler/mosaic/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/mosaic/methods/base.py` & `rio_tiler-6.0.0/rio_tiler/mosaic/methods/base.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/rio_tiler/mosaic/methods/defaults.py` & `rio_tiler-6.0.0/rio_tiler/mosaic/methods/defaults.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/.gitignore` & `rio_tiler-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/LICENSE` & `rio_tiler-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/README.md` & `rio_tiler-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.3/pyproject.toml` & `rio_tiler-6.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 dynamic = ["version"]
 dependencies = [
     "attrs",
     "cachetools",
     "httpx",
     "numexpr",
     "numpy",
-    "morecantile>=4.0,<5.0",
-    "pydantic",
+    "morecantile>=5.0,<6.0",
+    "pydantic~=2.0",
     "pystac>=0.5.4",
     "rasterio>=1.3.0",
     "color-operations",
     "importlib_resources>=1.1.0; python_version < '3.9'",
 ]
 
 [project.optional-dependencies]
```

### Comparing `rio_tiler-5.0.3/PKG-INFO` & `rio_tiler-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-tiler
-Version: 5.0.3
+Version: 6.0.0
 Summary: User friendly Rasterio plugin to read raster datasets.
 Project-URL: Homepage, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Documentation, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Issues, https://github.com/cogeotiff/rio-tiler/issues
 Project-URL: Source, https://github.com/cogeotiff/rio-tiler
 Project-URL: Changelog, https://cogeotiff.github.io/rio-tiler/release-notes/
 Author-email: Vincent Sarago <vincent@developmentseed.com>
@@ -50,18 +50,18 @@
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: cachetools
 Requires-Dist: color-operations
 Requires-Dist: httpx
 Requires-Dist: importlib-resources>=1.1.0; python_version < '3.9'
-Requires-Dist: morecantile<5.0,>=4.0
+Requires-Dist: morecantile<6.0,>=5.0
 Requires-Dist: numexpr
 Requires-Dist: numpy
-Requires-Dist: pydantic
+Requires-Dist: pydantic~=2.0
 Requires-Dist: pystac>=0.5.4
 Requires-Dist: rasterio>=1.3.0
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-jupyter; extra == 'docs'
```

